# Comparing `tmp/kmisc-2.1.85.tar.gz` & `tmp/kmisc-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmisc-2.1.85.tar", last modified: Wed Aug  2 14:51:39 2023, max compression
+gzip compressed data, was "dist/kmisc-2.1.9.tar", last modified: Fri Dec 17 06:53:02 2021, max compression
```

## Comparing `kmisc-2.1.85.tar` & `kmisc-2.1.9.tar`

### file list

```diff
@@ -1,14 +1,63 @@
-drwxr-xr-x   0 kage      (1000) kage      (1000)        0 2023-08-02 14:51:39.158224 kmisc-2.1.85/
--rw-rw-r--   0 kage      (1000) kage      (1000)     1066 2021-12-15 17:55:20.000000 kmisc-2.1.85/LICENSE
--rw-r--r--   0 kage      (1000) kage      (1000)     5522 2023-08-02 14:51:39.158224 kmisc-2.1.85/PKG-INFO
--rw-rw-r--   0 kage      (1000) kage      (1000)     5084 2022-02-08 03:10:22.000000 kmisc-2.1.85/README.md
-drwxr-xr-x   0 kage      (1000) kage      (1000)        0 2023-08-02 14:51:39.157224 kmisc-2.1.85/kmisc/
--rw-r--r--   0 kage      (1000) kage      (1000)   153240 2023-08-02 14:48:19.000000 kmisc-2.1.85/kmisc/__init__.py
-drwxr-xr-x   0 kage      (1000) kage      (1000)        0 2023-08-02 14:51:39.158224 kmisc-2.1.85/kmisc.egg-info/
--rw-rw-r--   0 kage      (1000) kage      (1000)     5522 2023-08-02 14:51:39.000000 kmisc-2.1.85/kmisc.egg-info/PKG-INFO
--rw-rw-r--   0 kage      (1000) kage      (1000)      175 2023-08-02 14:51:39.000000 kmisc-2.1.85/kmisc.egg-info/SOURCES.txt
--rw-rw-r--   0 kage      (1000) kage      (1000)        1 2023-08-02 14:51:39.000000 kmisc-2.1.85/kmisc.egg-info/dependency_links.txt
--rw-rw-r--   0 kage      (1000) kage      (1000)        6 2023-08-02 14:51:39.000000 kmisc-2.1.85/kmisc.egg-info/top_level.txt
--rw-rw-r--   0 kage      (1000) kage      (1000)      104 2021-12-15 17:55:20.000000 kmisc-2.1.85/pyproject.toml
--rw-r--r--   0 kage      (1000) kage      (1000)       38 2023-08-02 14:51:39.158224 kmisc-2.1.85/setup.cfg
--rw-rw-r--   0 kage      (1000) kage      (1000)     1974 2021-12-16 01:37:50.000000 kmisc-2.1.85/setup.py
+drwxrwxr-x   0 kage      (1000) kage      (1000)        0 2021-12-17 06:53:02.000000 kmisc-2.1.9/
+drwxrwxr-x   0 kage      (1000) kage      (1000)        0 2021-12-17 06:53:02.000000 kmisc-2.1.9/kmisc/
+-rw-rw-r--   0 kage      (1000) kage      (1000)     4796 2021-12-16 01:20:05.000000 kmisc-2.1.9/kmisc/Abs.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)     1958 2021-12-15 18:03:04.000000 kmisc-2.1.9/kmisc/COLOR.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)     4874 2021-12-17 06:48:29.000000 kmisc-2.1.9/kmisc/CONVERT.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)      684 2021-12-16 01:20:14.000000 kmisc-2.1.9/kmisc/Cd.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)     1825 2021-12-16 01:20:33.000000 kmisc-2.1.9/kmisc/Compress.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)      381 2021-12-15 18:04:10.000000 kmisc-2.1.9/kmisc/Copy.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)      831 2021-12-16 19:04:17.000000 kmisc-2.1.9/kmisc/Crc.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)     3116 2021-12-17 01:17:35.000000 kmisc-2.1.9/kmisc/Cut.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)     5813 2021-12-16 01:22:31.000000 kmisc-2.1.9/kmisc/DEV.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)    17066 2021-12-16 00:45:37.000000 kmisc-2.1.9/kmisc/DICT.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)     1077 2021-12-16 01:23:16.000000 kmisc-2.1.9/kmisc/DIFF.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)     1387 2021-12-16 01:22:14.000000 kmisc-2.1.9/kmisc/Delete.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)    24700 2021-12-17 02:14:23.000000 kmisc-2.1.9/kmisc/FILE.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)     4958 2021-12-16 05:14:43.000000 kmisc-2.1.9/kmisc/FIND.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)      216 2021-12-15 17:56:04.000000 kmisc-2.1.9/kmisc/FirstKey.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)     8900 2021-12-16 19:09:17.000000 kmisc-2.1.9/kmisc/GET.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)      307 2021-12-15 19:37:13.000000 kmisc-2.1.9/kmisc/GIT.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)     6439 2021-12-16 01:24:09.000000 kmisc-2.1.9/kmisc/HOST.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)    12873 2021-12-17 00:39:55.000000 kmisc-2.1.9/kmisc/IP.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)     5807 2021-12-16 19:07:46.000000 kmisc-2.1.9/kmisc/IS.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)      668 2021-12-16 01:25:14.000000 kmisc-2.1.9/kmisc/ISO.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)    10384 2021-12-16 20:00:00.000000 kmisc-2.1.9/kmisc/Import.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)     1541 2021-12-16 05:15:18.000000 kmisc-2.1.9/kmisc/Index.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)     1156 2021-12-15 17:56:04.000000 kmisc-2.1.9/kmisc/Insert.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)    10196 2021-12-17 01:20:11.000000 kmisc-2.1.9/kmisc/LIST.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)     7747 2021-12-16 01:26:26.000000 kmisc-2.1.9/kmisc/LOG.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)     1952 2021-12-17 00:22:52.000000 kmisc-2.1.9/kmisc/MAC.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)     5829 2021-12-15 17:52:07.000000 kmisc-2.1.9/kmisc/MODULE.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)   100207 2021-12-17 03:37:26.000000 kmisc-2.1.9/kmisc/Misc.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)      107 2021-12-15 17:56:04.000000 kmisc-2.1.9/kmisc/MyDir.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)    15017 2021-12-16 18:29:01.000000 kmisc-2.1.9/kmisc/Net.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)      772 2021-12-17 00:54:07.000000 kmisc-2.1.9/kmisc/OutFormat.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)     1136 2021-12-15 17:56:04.000000 kmisc-2.1.9/kmisc/Path.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)    11771 2021-12-16 05:36:43.000000 kmisc-2.1.9/kmisc/Print.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)       45 2021-12-15 17:56:04.000000 kmisc-2.1.9/kmisc/Pwd.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)     1894 2021-12-17 00:09:11.000000 kmisc-2.1.9/kmisc/Random.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)      399 2021-12-15 17:56:04.000000 kmisc-2.1.9/kmisc/Replace.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)     4080 2021-12-16 01:32:47.000000 kmisc-2.1.9/kmisc/SHELL.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)     5911 2021-12-16 05:18:44.000000 kmisc-2.1.9/kmisc/STR.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)     4457 2021-12-17 00:53:03.000000 kmisc-2.1.9/kmisc/Screen.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)     3486 2021-12-15 17:56:04.000000 kmisc-2.1.9/kmisc/Sort.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)      972 2021-12-16 23:30:58.000000 kmisc-2.1.9/kmisc/Splilt.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)     2358 2021-12-16 01:33:57.000000 kmisc-2.1.9/kmisc/TIME.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)      324 2021-12-16 01:33:44.000000 kmisc-2.1.9/kmisc/Tap.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)    10327 2021-12-16 01:34:07.000000 kmisc-2.1.9/kmisc/Type.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)     1489 2021-12-15 17:56:04.000000 kmisc-2.1.9/kmisc/Update.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)     2839 2021-12-17 06:43:00.000000 kmisc-2.1.9/kmisc/VERSION.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)     5215 2021-12-16 04:49:10.000000 kmisc-2.1.9/kmisc/WEB.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)      540 2021-12-16 01:34:50.000000 kmisc-2.1.9/kmisc/Wrap.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)      866 2021-12-16 23:35:47.000000 kmisc-2.1.9/kmisc/Xml.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)    10917 2021-12-17 06:49:34.000000 kmisc-2.1.9/kmisc/__init__.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)     2896 2021-12-15 17:51:29.000000 kmisc-2.1.9/kmisc/test.py
+drwxrwxr-x   0 kage      (1000) kage      (1000)        0 2021-12-17 06:53:02.000000 kmisc-2.1.9/kmisc.egg-info/
+-rw-rw-r--   0 kage      (1000) kage      (1000)     5597 2021-12-17 06:53:02.000000 kmisc-2.1.9/kmisc.egg-info/PKG-INFO
+-rw-rw-r--   0 kage      (1000) kage      (1000)      888 2021-12-17 06:53:02.000000 kmisc-2.1.9/kmisc.egg-info/SOURCES.txt
+-rw-rw-r--   0 kage      (1000) kage      (1000)        1 2021-12-17 06:53:02.000000 kmisc-2.1.9/kmisc.egg-info/dependency_links.txt
+-rw-rw-r--   0 kage      (1000) kage      (1000)        6 2021-12-17 06:53:02.000000 kmisc-2.1.9/kmisc.egg-info/top_level.txt
+-rw-rw-r--   0 kage      (1000) kage      (1000)     3763 2021-12-16 01:43:55.000000 kmisc-2.1.9/README.md
+-rw-rw-r--   0 kage      (1000) kage      (1000)     1974 2021-12-16 01:37:50.000000 kmisc-2.1.9/setup.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)     5597 2021-12-17 06:53:02.000000 kmisc-2.1.9/PKG-INFO
+-rw-rw-r--   0 kage      (1000) kage      (1000)       38 2021-12-17 06:53:02.000000 kmisc-2.1.9/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `kmisc-2.1.85/kmisc/__init__.py` & `kmisc-2.1.9/kmisc/Misc.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,2881 +1,426 @@
-#!/bin/python
 # -*- coding: utf-8 -*-
+#Kage park
 # Kage personal stuff
-#
+
+#######################################
+# Load All files
+#######################################
 from __future__ import print_function
-import os
-import re
-import sys
-import ast
-import ssl
-import stat
-import time
-import uuid
-import zlib
-import copy
-import smtplib
+from distutils.spawn import find_executable
+import sys,os,re,subprocess,copy
 import tarfile
-import zipfile
+import tempfile
+import traceback,inspect
+import time
+from datetime import datetime
+from os import close, remove
 import random
-import struct
-import string
-import fnmatch
-import pickle
-import tarfile
-import zipfile
+import fcntl,socket, struct
 import pickle
-import random
-import inspect
+from threading import Thread
 import base64
 import hashlib
-import importlib
-import subprocess
-import traceback
-import fcntl,socket,struct
-import json
-import email.utils
-import xml.etree.ElementTree as ET
-from sys import modules
-from sys import path as mod_path
-from sys import version_info
-from pprint import pprint
-from threading import Thread
-from datetime import datetime
-from email import encoders
-from email.mime.text import MIMEText
-from email.mime.base import MIMEBase
-from email.mime.multipart import MIMEMultipart
 from multiprocessing import Process, Queue
+
+import json
+import uuid
+import ast
+import base64
+import ssl
 from distutils.version import LooseVersion
-from kmport import *
-import kmport as kp
 
-from http.cookies import Morsel # This module for requests when you use build by pyinstaller command
+from kmisc.Import import *
+Import('zlib')
+Import('from kmisc.GET import *')
+Import('from kmisc.SHELL import SHELL')
+rshell=SHELL().Run
 
+ansi_escape = re.compile(r'\x1B\[[0-?]*[ -/]*[@-~]')
 url_group = re.compile('^(https|http|ftp)://([^/\r\n]+)(/[^\r\n]*)?')
 #log_file=None
 log_intro=3
 log_new_line='\n'
 pipe_file=None
 
 cdrom_ko=['sr_mod','cdrom','libata','ata_piix','ata_generic','usb-storage']
+def clean_ansi(data):
+    if data:
+        if isinstance(data,str):
+            return ansi_escape.sub('',data)
+        elif isinstance(data,list):
+            new_data=[]
+            for ii in data:
+                new_data.append(ansi_escape.sub('',ii))
+            return new_data
+    return data
 
-def Abs(*inps,**opts):
-    default=opts.get('default',None)
-    out=opts.get('out','auto')
-    obj=opts.get('obj',None)
-    err=opts.get('err',True)
-    def int_idx(idx,nobj,default,err,out='auto'):
-        if idx < 0:
-            if abs(idx) <= nobj:
-                if out in ['list',list]:
-                    return [nobj+idx]
-                elif out in ['tuple',tuple]:
-                    return (nobj+idx,)
-                return nobj+idx
-            elif err not in [True,'err','True']:
-                return 0
-        else:
-            if nobj > idx:
-                if out in ['list',list]:
-                    return [idx]
-                elif out in ['tuple',tuple]:
-                    return (idx,)
-                return idx
-            elif err not in [True,'err','True']:
-                return nobj-1
-        return default
-    if len(inps) > 0:
-        ss=None
-        ee=None
-        rt=[]
-        if IsNone(obj):
-            for i in inps:
-                if isinstance(i,int):
-                    rt.append(abs(i))
-                elif err in [True,'err','True']:
-                    rt.append(default)
-        elif isinstance(obj,dict):
-            keys=list(obj)
-            for idx in inps:
-                if isinstance(idx,int):
-                    int_index=int_idx(idx,len(keys),default,err)
-                    if int_index != default: rt.append(keys[int_index])
-                elif isinstance(idx,tuple) and len(idx) == 2:
-                    ss=Abs(idx[0],**opts)
-                    ee=Abs(idx[1],**opts)
-                    for i in range(ss,ee+1):
-                        rt.append(keys[i])
-                elif isinstance(idx,str):
-                    if len(idx.split(':')) == 2:
-                        ss,ee=tuple(idx.split(':'))
-                        if isinstance(ss,int) and isinstance(ee,int):
-                            for i in range(ss,ee+1):
-                                rt.append(keys[i])
-                    elif len(idx.split('-')) == 2:
-                        ss,ee=tuple(idx.split('-'))
-                        if isinstance(ss,int) and isinstance(ee,int):
-                            for i in range(ss,ee+1):
-                                rt.append(keys[i])
-                    elif len(idx.split('|')) > 1:
-                        for i in idx.split('|'): #A|B => A or B
-                            if i in keys:
-                                rt.append(i)
-                    else:
-                        rt.append(idx)
-        elif isinstance(obj,(list,tuple,str)):
-            nobj=len(obj)
-            for idx in inps:
-                if isinstance(idx,list):
-                    for ii in idx:
-                        if isinstance(ii,int):
-                            if nobj > ii:
-                                rt.append(ii)
-                            else:
-                                rt.append(OutFormat(default))
-                elif isinstance(idx,int):
-                    rt.append(int_idx(idx,nobj,default,err))
-                elif isinstance(idx,tuple) and len(idx) == 2:
-                    ss=Abs(idx[0],**opts)
-                    ee=Abs(idx[1],**opts)
-                    rt=rt+list(range(ss,ee+1))
-                elif isinstance(idx,str):
-                    try:
-                        idx=int(idx)
-                        rt.append(int_idx(idx,nobj,default,err))
-                    except:
-                        if len(idx.split(':')) == 2:
-                            ss,ee=tuple(idx.split(':'))
-                            ss=Abs(ss,**opts)
-                            ee=Abs(ee,**opts)
-                            if isinstance(ss,int) and isinstance(ee,int):
-                                rt=rt+list(range(ss,ee+1))
-                        elif len(idx.split('-')) == 2:
-                            ss,ee=tuple(idx.split('-'))
-                            ss=Abs(ss,**opts)
-                            ee=Abs(ee,**opts)
-                            if isinstance(ss,int) and isinstance(ee,int):
-                                rt=rt+list(range(ss,ee+1))
-                        elif len(idx.split('|')) > 1:
-                            for i in idx.split('|'):
-                                ss=Abs(i,obj=obj,out='raw')
-                                if isinstance(ss,int):
-                                    rt.append(ss)
-                        else:
-                            rt.append(OutFormat(default))
-        return OutFormat(rt,out=out)
-    elif obj:
-        if isinstance(obj,(list,tuple,str)):
-            return len(obj)
-        elif isinstance(obj,dict):
-            return list(obj.keys())
-    return default
-
-def Delete(*inps,**opts):
-    if len(inps) >= 2:
-        obj=inps[0]
-        keys=inps[1:]
-    elif len(inps) == 1:
-        obj=inps[0]
-        keys=opts.get('key',None)
-        if isinstance(keys,list):
-            keys=tuple(keys)
-        elif not IsNone(keys):
-            keys=(keys,)
-    default=opts.get('default',None)
-    _type=opts.get('type','index')
-
-    if isinstance(obj,(list,tuple)):
-        nobj=len(obj)
-        rt=[]
-        if _type == 'index':
-            nkeys=Abs(*tuple(keys),obj=obj,out=list)
-            for i in range(0,len(obj)):
-                if i not in nkeys:
-                    rt.append(obj[i])
-        else:
-            for i in obj:
-                if i not in keys:
-                    rt.append(i)
-        return rt
-    elif isinstance(obj,dict):
-        if isinstance(keys,(list,tuple,dict)):
-            for key in keys:
-                obj.pop(key,default)
-        else:
-            obj.pop(keys,default)
-        return obj
-    elif isinstance(obj,str):
-        nkeys=[]
-        for i in keys:
-            if isinstance(i,(tuple,str,int)):
-                tt=Abs(i,obj=obj,out=list)
-                if tt:
-                    nkeys=nkeys+tt
-        rt=''
-        for i in range(0,len(obj)):
-            if i in nkeys:
-                continue
-            rt=rt+obj[i]
-        return rt
-    return default
-
-class COLOR:
-    def __init__(self,**opts):
-       self.color_db=opts.get('color',{'blue': 34, 'grey': 30, 'yellow': 33, 'green': 32, 'cyan': 36, 'magenta': 35, 'white': 37, 'red': 31})
-       self.bg_color_db=opts.get('bg',{'cyan': 46, 'white': 47, 'grey': 40, 'yellow': 43, 'blue': 44, 'magenta': 45, 'red': 41, 'green': 42})
-       self.attr_db=opts.get('attr',{'reverse': 7, 'blink': 5,'concealed': 8, 'underline': 4, 'bold': 1})
-
-    def Color_code(self,name,default=None):
-       return self.color_db.get(name,default)
-
-    def Background_code(self,name,default=None):
-       return self.color_db.get(name,default)
-
-    def Attr_code(self,name,default=None):
-       return self.color_db.get(name,default)
-
-    def Get(self,color,mode='color',default=None):
-       color_code=None
-       if mode == 'color':
-           color_code=self.Color_code(color,default=default)
-       elif mode in ['background','bg']:
-           color_code=self.Background_code(color,default=default)
-       elif mode in ['attr','attribute']:
-           color_code=self.Attr_code(color,default=default)
-       return color_code
-
-    def String(self,msg,color,bg=False,attr=False,mode='shell'):
-       if mode in ['html','HTML']:
-           if bg:
-               return '''<p style="background-color: {}">{}</p>'''.format(format(color,msg))
-           else:
-               return '''<font color={}>{}</font>'''.format(color,msg)
-       else:
-           if bg:
-               color_code=self.Get(color,mode='bg',default=None)
-           elif attr:
-               color_code=self.Get(color,mode='attr',default=None)
-           else:
-               color_code=self.Get(color,default=None)
-           if IsNone(color_code):
-               return msg
-           if IsNone(os.getenv('ANSI_COLORS_DISABLED')):
-               reset='''\033[0m'''
-               fmt_msg='''\033[%dm%s'''
-               msg=fmt_msg % (color_code,msg)
-               return msg+reset
-
-class DIFF:
-    def __init__(self):
-        pass
-
-    def Data(self,a,sym,b,ignore=None,default=None):
-        if isinstance(ignore,(list,tuple)):
-            if a in ignore or b in ignore:
-                return default
-        elif not IsNone(ignore):
-            if eval('{} == {}'.format(a,ignore)) or eval('{} == {}'.format(b,ignore)):
-                return default
-        if sym == '==':
-            try:
-                return eval('{} == {}'.format(a,b))
-            except:
-                return default
-        elif isinstance(a,int) and isinstance(b,int):
-            try:
-                return eval('{} {} {}'.format(a,sym,b))
-            except:
-                return default
-        elif isinstance(a,str) and isinstance(b,str) and a.isdigit() and b.isdigit():
-            try:
-                return eval('{} {} {}'.format(a,sym,b))
-            except:
-                return default
-        return default
-
-    def Code(self):
-        pass
-
-    def File(self):
-        pass
-
-
-class LIST(list):
-    def __init__(self,*inps):
-        if len(inps) == 1 and isinstance(inps[0],(list,tuple)):
-            self.root=list(inps[0])
-        else:
-            self.root=list(inps)
-
-#    def __new__(cls,*inps):
-#        if len(inps) == 1 and isinstance(inps[0],(list,tuple)):
-#            return list(inps[0])
-#        else:
-#            return list(inps)
-
-    # reply self.root back to the Class's output a=List(['a']), return the data to a
-    def __repr__(self):
-        return repr(self.root)
-
-    def Convert(self,src,path=False,default=False,symbol=':white_space:',**opts):
-        if isinstance(src,str) and src:
-            if path and isinstance(symbol,str):
-                if symbol == ':white_space:':
-                    symbol='/'
-                start=0
-                if src[0] == symbol:
-                    start=1
-                if src[-1] == symbol:
-                    return src.split(symbol)[start:-1]
-                return src.split(symbol)[start:]
-            else:
-                if symbol == ':white_space:':
-                    return src.strip().split()
-                elif isinstance(symbol,str):
-                    return src.split(symbol)
-                elif isinstance(symbol,(tuple,list)):
-                    #regexPattern = '|'.join(map(re.escape,tuple(symbol)))
-                    regexPattern = Join(map(re.escape,tuple(symbol)),symbol='|')
-                    return re.split(regexPattern,src)
-                return default
-        elif isinstance(src,(list,tuple)):
-            return list(src)
-        else:
-            return [src]
- 
-    def Append(self,*inps,**opts):
-        uniq=opts.get('uniq',False)
-        symbol=opts.get('symbol',':white_space:')
-        path=opts.get('path',False)
-        default=opts.get('default',False)
-        for pp in inps:
-            if Type(pp,('bytes','str')):
-                if symbol == ':white_space:':
-                    pp=pp.strip()
-                    symbol=' '
-                if path: symbol='/'
-                for rp in Split(pp,symbol,default=[]):
-                    if rp == default: continue
-                    if uniq and rp in self.root: continue
-                    if path:
-                        if rp == '.': continue
-                        if rp == '..' and len(self.root):
-                            del self.root[-1]
-                            continue
-                    self.root.append(rp)
-            else:
-                if uniq and pp in self.root: continue
-                self.root.append(pp)
-        return self.root
-
-    def append(self,inp):
-        self.root.append(inp)
-
-    def Uniq(self,*inps,**opts):
-        symbol=opts.get('symbol',':white_space:')
-        path=opts.get('path',False)
-        default=opts.get('default',False)
-        rt=[]
-        for pp in self.root + list(inps):
-            if Type(pp,('bytes','str')):
-                if symbol == ':white_space:':
-                    pp=pp.strip()
-                    symbol=' '
-                if path: symbol='/'
-                for rp in Split(pp,symbol,default=[]):
-                    if rp not in rt and rp != default:
-                        if path:
-                            if rp == '.': continue
-                            if rp == '..' and len(rt):
-                                del rt[-1]
-                                continue
-                        rt.append(rp)
-            else:
-                if pp not in rt: rt.append(pp)
-        self.root=rt
-        return self.root
-
-    def Delete(self,*inps,**opts):
-        find=opts.get('find','index')
-        default=opts.get('default',False)
-        self.root=rm(self.root,*inps,data=True if find in ['data','element','value'] else False,default=default)
-
-    def Get(self,*inps,**opts):
-        if not inps: return self.root
-        find=opts.get('find','data')
-        default=opts.get('default',None)
-        out=opts.get('out',list)
-        err=opts.get('err',False)
-        if len(self.root) == 0 and err:
-            return default
-        rt=[]
-        if find in ['index','idx']:
-            rt=List(self.root,find=inps,mode='err' if err else 'auto',default=default)
-        else:
-            rt=List(self.root,idx=inps,mode='err' if err else 'auto',default=default)
-        if rt:
-            if out in [tuple,'tuple']:
-                return tuple(rt)
-            elif IsNone(out,chk_val=[None,'','raw']):
-                if len(rt) == 1: return rt[0]
-            return rt
-        return default
-
-    def Index(self,*inps):
-        return self.Get(*inps,find='index')
-
-    def Insert(self,*inps,**opts):
-        start=opts.get('at',0)
-        default=opts.get('default',False)
-        err=opts.get('err',False)
-        if isinstance(at,str):
-            if at in ['start','first']: self.root=list(inps)+self.root
-            if at in ['end','last']: self.root=self.root+list(inps)
-        elif len(self.root) == 0:
-            self.root=list(inps)
-        elif isinstance(start,int) and len(self.root) > start:
-            self.root=self.root[:start]+list(inps)+self.root[start:]
-        else:
-            if err:
-                return default
-            self.root=self.root+list(inps)
-
-    def Update(self,*inps,**opts):
-        at=opts.get('at',0)
-        err=opts.get('err',False)
-        default=opts.get('default',False)
-        n=len(self.root)
-        if n == 0:
-            if err is True:
-                return default
-            else:
-                self.root=list(inps)
-        elif isinstance(at,int) and n > at:
-            for i in range(0,len(inps)):
-                if n > at+i:
-                    self.root[at+i]=inps[i]
-                elif err is True:
-                    return default
-                else:
-                    self.root=self.root+list(inps)[i:]
-                    break
-        elif isinstance(at,(tuple,list)):
-            if len(inps) == len(at):
-                for i in range(0,len(at)):
-                    if isinstance(at[i],int) and n > at[i]:
-                        self.root[at[i]]=inps[i]
-                    elif err is True:
-                        return default
-                    else:
-                        self.root.append(inps[i])
+def is_cancel(func):
+    if func:
+        ttt=type(func).__name__
+        if ttt in ['function','instancemethod','method']:
+            if func(): return True
+        elif ttt  == 'bool':
+            if func : return True
+    return False
 
-    def Find(self,*inps,**opts):
-        find=opts.get('find','index')
-        default=opts.get('default',[])
-        rt=[]
-        for i in range(0,len(self.root)):
-            for j in inps:
-                j=j.replace('*','.+').replace('?','.')
-                mm=re.compile(j)
-                if bool(re.match(mm,self.root[i])):
-                    if find in ['index','idx']:
-                        rt.append(i)
-                    else:
-                        rt.append(self.root[i])
-        if len(rt):
-            return rt
-        return default
+def log_file_info(name):
+    log_file_str=''
+    if name and len(name) > 0:
+        if type(name) is str:
+            if name.split(':')[0] == 'log_file':
+                return name
+            name=name.split(',')
+        for nn in name:
+            if nn and nn != 'None':
+                if log_file_str:
+                    log_file_str='{}:{}'.format(log_file_str,nn)
+                else:
+                    log_file_str='{}'.format(nn)
+        if log_file_str:
+            return 'log_file:{}'.format(log_file_str)
 
-    def Copy(self):
-        return self.root[:]
-    def copy(self):
-        return self.root[:]
+def error_exit(msg=None):
+    if msg is not None:
+       print(msg)
+    sys.exit(-1)
 
-    def Tuple(self):
-        return tuple(self.root)
 
-    def Move2first(self,find):
-        if isinstance(find,(list,tuple)):
-            self.Delete(*find,find='data')
-            self.root=list(find)+self.root
-        else:
-            self.Delete(*(find,),find='data')
-            self.root=[find]+self.root
-        return self.root
-
-    def Move2end(self,find):
-        if isinstance(find,(list,tuple)):
-            self.Delete(*find,find='data')
-            self.root=self.root+list(find)
+def std_err(msg,direct=False):
+    if direct:
+        sys.stderr.write(msg)
+    else:
+        sys.stderr.write('{}\n'.format(msg))
+    sys.stderr.flush()
+    
+def format_time(time=0,tformat='%s',time_format='%S'):
+    if time in [0,'0',None]:
+        return datetime.now().strftime(tformat)
+    elif isinstance(time,int) or (isinstance(time,str) and time.isdigit()):
+        #if type(time) is int or (type(time) is str and time.isdigit()):
+        if time_format == '%S':
+            return datetime.fromtimestamp(int(time)).strftime(tformat)
         else:
-            self.Delete(*(find,),find='data')
-            self.root=self.root+[find]
-        return self.root
-
-    def Sort(self,reverse=False,func=None,order=None,field=None):
-        self.root=Sort(self.root,revers=revers,func=func,order=order,field=field)
-
-class STR(str):
-    def __init__(self,src,byte=None):
-        if isinstance(byte,bool):
-            if byte:
-                self.src=Bytes(src)
-            else:
-                self.src=Str(src)
-        else:
-            self.src=src
-
-    def Rand(self,length=8,strs=None,mode='*'):
-        return Random(length=length,strs=strs,mode=mode)
-
-    def Cut(self,head_len=None,body_len=None,new_line='\n',out=str):
-        if not isinstance(self.src,str):
-           self.src='''{}'''.format(self.src)
-        return Cut(self.src,head_len,body_len,new_line,out)
-
-    def Space(num=1,fill=' ',mode='space'):
-        return Space(num,fill,mode)
-
-    def Reduce(self,start=0,end=None,sym=None,default=None):
-        if isinstance(self.src,str):
-            if sym:
-                arr=self.src.split(sym)
-                if isinstance(end,int):
-                    return Join(arr[start:end],symbol=sym)
-                else:
-                    return Join(arr[start],symbol=sym)
-            else:
-                if isinstance(end,int):
-                    return self.src[start:end]
-                else:
-                    return self.src[start:]
-        return default
-
-    def Find(self,find,src='_#_',prs=None,sym='\n',pattern=True,default=[],out=None,findall=True,word=False,line_num=False,peel=None):
-        if IsNone(src,chk_val=['_#_'],chk_only=True): src=self.src
-        return FIND(src).Find(find,prs=prs,sym=sym,default=default,out=out,findall=findall,word=word,mode='value',line_num=line_num,peel=peel)
-
-    def Index(self,find,start=None,end=None,sym='\n',default=[],word=False,pattern=False,findall=False,out=None):
-        if not isinstance(self.src,str): return default
-        rt=[]
-        source=self.src.split(sym)
-        for row in range(0,len(source)):
-            for ff in self.Find(find,src=source[row],pattern=pattern,word=word,findall=findall,default=[],out=list):
-                if findall:
-                    rt=rt+[(row,[m.start() for m in re.finditer(ff,source[row])])]
-                else:
-                    idx=source[row].index(ff,start,end)
-                    if idx >= 0:
-                        rt.append((row,idx))
-        if rt:
-            if out in ['tuple',tuple]: return tuple(rt)
-            if out not in ['list',list] and len(rt) == 1 and rt[0][0] == 0: 
-                if len(rt[0][1]) == 1:return rt[0][1][0]
-                return rt[0][1]
-            return rt
-        return default
-
-    def Replace(self,replace_what,replace_to,default=None):
-        if isinstance(self.src,str):
-            if replace_what[-1] == '$' or replace_what[0] == '^':
-                return re.sub(replace_what, replace_to, self.src)
-            else:
-                head, _sep, tail = self.src.rpartition(replace_what)
-                return head + replace_to + tail
-        return default
-
-    def RemoveNewline(self,src='_#_',mode='edge',newline='\n',byte=None):
-        if IsNone(src,chk_val=['_#_'],chk_only=True): src=self.src
-        if isinstance(byte,bool):
-            if byte:
-                src=Bytes(src)
-            else:
-                src=Str(src)
-        src_a=Split(src,newline,default=False)
-        if src_a is False:
-            return src
-        if mode in ['edge','both']:
-            if not src_a[0].strip() and not src_a[-1].strip():
-                return Join(src_a[1:-1],symbol=newline)
-            elif not src_a[0].strip():
-                return Join(src_a[1:],symbol=newline)
-            elif not src_a[-1].strip():
-                return Join(src_a[:-1],symbol=newline)
-        elif mode in ['first','start',0]:
-            if not src_a[0].strip():
-                return Join(src_a[1:],symbol=newline)
-        elif mode in ['end','last',-1]:
-            if not src_a[-1].strip():
-                return Join(src_a[:-1],symbol=newline)
-        elif mode in ['*','all','everything']:
-            return Join(src_a,symbol='')
-        return src
-
-    def Wrap(self,src='_#_',space='',space_mode='space',sym='\n',default='org',NFLT=False,out=str):
-        if IsNone(src,chk_val=[None,'_#_'],chk_only=True): src=self.src
-        if isinstance(space,str): space=len(space)
-        return WrapString(src,fspace=space,nspace=space,new_line=sym,NFLT=NFLT,mode=space_mode)
-
-    def Tap(self,space='',sym='\n',default='org',NFLT=False,out=str):
-        if isinstance(space,str):
-            space=len(space)
-        return WrapString(fspace=space,nspace=space,new_line=sym,NFLT=NFLT)
-
-class CONVERT:
-    def __init__(self,src):
-        self.src=src
-
-    def Int(self,default=False):
-        return Int(self.src,default)
-
-    def Str(self,default='org'):
-        return Str(self.src,default=default,mode='force')
-
-    def Ast(self,default=False,want_type=None):
-        return TypeData(self.src,default,want_type)
-
-    def Form(self,default=False):
-        return self.Ast(default=default)
-
-    def Json(self,src='_#_',default=None):
-        if IsNone(src,chk_val=['_#_'],chk_only=True): src=self.src
-        try:
-            return json.loads(src)
-        except:
-            return default
-
-    def Mac2Str(self,case='lower',default=False):
-        return MAC(self.src).ToStr(case,default)
-
-    def Str2Mac(self,case='lower',default=False,sym=':',chk=False):
-        return MAC(self.src).FromStr(case=case,default=default,sym=sym,chk=chk)
-
-    def Size(self,unit='b:g',default=False):
-        return sizeConvert(self.src,unit=unit)
-
-    def Url(self):
-        return str2url(self.src)
-
-class MAC:
-    def __init__(self,src=None):
-        self.src=src
-
-    def IsV4(self,**opts):
-        if MacV4(self.src,**opts): return True
-        return False
-
-    def FromStr(self,case='lower',default=False,sym=':',chk=False):
-        return MacV4(self.src,case=case,default=default,symbol=sym)
-
-    def ToStr(self,case='lower',default=False):
-        return MacV4(self.src,case=case,default=default,symbol='')
-
-    def GetIfname(self):
-        if not self.FromStr(): return False
-        net_dir='/sys/class/net'
-        if os.path.isdir(net_dir):
-            dirpath,dirnames,filenames = list(os.walk(net_dir))[0]
-            for dev in dirnames:
-                fmac=cat('{}/{}/address'.format(dirpath,dev),no_end_newline=True)
-                if type(fmac) is str and fmac.strip().lower() == self.src.lower():
-                    return dev
-
-    def FromIfname(self,ifname,default=None):
-        if isinstance(ifname,str):
-            try:
-                s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-                if PyVer(3):
-                    info = fcntl.ioctl(s.fileno(), 0x8927,  struct.pack('256s', Bytes(ifname[:15],encode='utf-8')))
-                    return ':'.join(['%02x' % char for char in info[18:24]])
-                else:
-                    info = fcntl.ioctl(s.fileno(), 0x8927,  struct.pack('256s', ifname[:15]))
-                    return ':'.join(['%02x' % ord(char) for char in info[18:24]])
-            except:
-                pass
-        return default
-
-class IP:
-    def __init__(self,ip=None):
-        self.ip=ip
-
-    def GetIP(self,ip=None):
-        if IsNone(ip,chk_val=['_#_']): 
-            return self.ip
-        return ip
-
-    def IsV4(self,ip=None):
-        ip=self.GetIP(ip)
-        return True if IpV4(ip) else False
-
-    def IsBmcIp(self,ip=None,port=(623,664,443)):
-        return self.IsOpenPort(port,ip=ip)
-
-    def IsOpenPort(self,port,**opts):
-        '''
-        It connectionable port(?) like as ssh, ftp, telnet, web, ...
-        '''
-        default=opts.get('default',False)
-        ip=self.GetIP(opts.get('ip'))
-        if IpV4(ip,port=port,default=default): return True
-        return False
+            return datetime.strptime(str(time),time_format).strftime(tformat)
 
-    def IsUsedPort(self,port,ip='_#_'):
-        #if IsNone(ip,chk_val=['_#_'],chk_only=True):ip=self.ip
-        ip=self.GetIP(ip)
-        return IpV4(ip,port=port,used=True)
-
-    def Ip2Num(self,ip=None,default=False):
-        ip=self.GetIP(ip)
-        return IpV4(ip,out=int,default=default)
-
-    def Ip2Str(self,ip=None,default=False):
-        ip=self.GetIP(ip)
-        return IpV4(ip,out=str,default=default)
-
-    def Ip2hex(self,ip=None,default=False):
-        ip=self.GetIP(ip)
-        return IpV4(ip,out=hex,default=default)
-
-    def InRange(self,start_ip,end_ip,**opts):
-        ip=self.GetIP(opts.get('ip'))
-        default=opts.get('default',False)
-        startip=self.Ip2Num(start_ip)
-        myip=self.Ip2Num(ip)
-        endip=self.Ip2Num(end_ip)
-        if isinstance(startip,int) and isinstance(myip,int) and isinstance(endip,int):
-            if startip <= myip <= endip: return True
-            return False
-        return default
-
-    def LostNetwork(self,**opts):
-        ip=self.GetIP(opts.get('ip'))
-        default=opts.get('default',False)
-        timeout_sec=opts.get('timeout',1800)
-        interval=opts.get('interval',2)
-        keep_good=opts.get('keep_good',30)
-        cancel_func=opts.get('cancel_func',None)
-        log=opts.get('log',None)
-        init_time=None
-        if self.IsV4(ip):
-            if not kp.ping(ip,count=5):
-                if not kp.ping(ip,count=0,timeout=timeout_sec,keep_good=keep_good,interval=interval,cancel_func=cancel_func,log=log):
-                    return True
-            return False
-        return default
-
-    def V4(self,ip='_#_',out='str',default=False):
-        #if IsNone(ip,chk_val=['_#_'],chk_only=True): ip=self.ip
-        ip=self.GetIP(ip)
-        return IpV4(ip,out=out,default=default)
-
-    def Online(self,**opts):
-        ip=self.GetIP(opts.get('ip'))
-        default=opts.get('default',False)
-        timeout_sec=opts.get('timeout',1800)
-        interval=opts.get('interval',3)
-        keep=opts.get('keep',20)
-        cancel_func=opts.get('cancel_func',None)
-        log=opts.get('log',None)
-        time=TIME()
-        run_time=time.Int()
-        if self.IsV4(ip):
-            if log:
-                log('[',direct=True,log_level=1)
-            while True:
-                if time.Out(timeout_sec):
-                    if log:
-                        log(']\n',direct=True,log_level=1)
-                    return False,'Timeout monitor'
-                if IsCancel(cancel_func):
-                    if log:
-                        log(']\n',direct=True,log_level=1)
-                    return True,'Stopped monitor by Custom'
-                if self.Ping(ip,cancel_func=cancel_func):
-                    if (time.Int() - run_time) > keep:
-                        if log:
-                            log(']\n',direct=True,log_level=1)
-                        return True,'OK'
-                    if log:
-                        log('-',direct=True,log_level=1)
-                else:
-                    run_time=time.Int()
-                    if log:
-                        log('.',direct=True,log_level=1)
-                time.Sleep(interval)
-            if log:
-                log(']\n',direct=True,log_level=1)
-            return False,'Timeout/Unknown issue'
-        return default,'IP format error'
-
-    def Ping(self,host='_#_',count=0,interval=1,keep_good=0, timeout=0,lost_mon=False,log=None,stop_func=None,log_format='.',cancel_func=None):
-        #if IsNone(host,chk_val=['_#_'],chk_only=True): host=self.ip
-        host=self.GetIP(host)
-        return kp.ping(host,count=count,interval=interval,keep_good=keep_good,timeout=timeout,lost_mon=lost_mon,log=log,stop_func=stop_func,log_format=log_format,cancel_func=cancel_func)
-
-def IsJson(src):
+def get_caller_fcuntion_name(detail=False):
     try:
-        json.loads(src)
-        return True
+        dep=len(inspect.stack())-2
+        if detail:
+            return sys._getframe(dep).f_code.co_name,sys._getframe(dep).f_lineno,sys._getframe(dep).f_code.co_filename
+        else:
+            name=sys._getframe(dep).f_code.co_name
+            if name == '_bootstrap_inner' or name == '_run_code':
+                return sys._getframe(3).f_code.co_name
+            return name
     except:
         return False
 
-def IsXml(src):
-    firstLine=file_rw(src,out='string',read='firstline')
-    if firstLine is False:
-        filename_str=Str(src)
-        if isinstance(filename_str,str):
-            firstLine=filename_str.split('\n')[0]
-    if isinstance(firstLine,str) and firstLine.split(' ')[0] == '<?xml': return True
-    return False
-
-def IsBin(src):
-    return find_executable(src)
-
-def IsPickle(src):
-    if isinstance(src,str) and os.path.isfile(src):
-        try:
-            with open(src,'rb') as f: # Pickle Type
-                pickle.load(f)
-                return True
-        except:
-            pass
-    return False
-
-class LOG:
-    def __init__(self,**opts):
-        self.limit=opts.get('limit',3)
-        self.dbg_level=opts.get('dbg_level',None)
-        self.path=opts.get('path','/tmp')
-        self.log_file=opts.get('log_file',None)
-        self.info_file=opts.get('info_file',None)
-        self.error_file=opts.get('error_file',None)
-        self.dbg_file=opts.get('dbg_file',None)
-        self.screen=opts.get('screen',False)
-        self.date_format=opts.get('date_format','[%m/%d/%Y %H:%M:%S]')
-
-    def Format(self,*msg,**opts):
-        log_date_format=opts.get('date_format',self.date_format)
-        func_name=opts.get('func_name',None)
-        end_new_line=opts.get('end_new_line','')
-        start_new_line=opts.get('start_new_line','\n')
-        if len(msg) > 0:
-            m_str=None
-            intro=''
-            intro_space=''
-            if log_date_format:
-                intro=TIME().Format(tformat=log_date_format)+' '
-            func_name_name=type(func_name).__name__
-            if func_name_name == 'str':
-                intro=intro+'{0} '.format(func_name)
-            elif func_name is True:
-                intro=intro+'{0}() '.format(CallerName())
-            elif func_name_name in ['function','instancemethod']:
-                intro=intro+'{0}() '.format(func_name.__name__)
-            if intro:
-               for i in range(0,len(intro)):
-                   intro_space=intro_space+' '
-            for m in list(msg):
-                n=m.split('\n')
-                #if m_str is None:
-                if IsNone(m_str):
-                    m_str='{0}{1}{2}{3}'.format(start_new_line,intro,n[0],end_new_line)
-                else:
-                    m_str='{0}{1}{2}{3}{4}'.format(m_str,start_new_line,intro_space,n[0],end_new_line)
-                for nn in n[1:]:
-                    m_str='{0}{1}{2}{3}{4}'.format(m_str,start_new_line,intro_space,nn,end_new_line)
-            return m_str
-
-    def Syslogd(self,*msg,**opts):
-        syslogd=opts.get('syslogd',None)
-        if syslogd:
-            #syslog_msg=' '.join(msg)
-            syslog_msg=Join(msg,symbol=' ')
-            if syslogd in ['INFO','info']:
-                syslog.syslog(syslog.LOG_INFO,syslog_msg)
-            elif syslogd in ['KERN','kern']:
-                syslog.syslog(syslog.LOG_KERN,syslog_msg)
-            elif syslogd in ['ERR','err']:
-                syslog.syslog(syslog.LOG_ERR,syslog_msg)
-            elif syslogd in ['CRIT','crit']:
-                syslog.syslog(syslog.LOG_CRIT,syslog_msg)
-            elif syslogd in ['WARN','warn']:
-                syslog.syslog(syslog.LOG_WARNING,syslog_msg)
-            elif syslogd in ['DBG','DEBUG','dbg','debug']:
-                syslog.syslog(syslog.LOG_DEBUG,syslog_msg)
-            else:
-                syslog.syslog(syslog_msg)
-
-
-    def File(self,log_str,log_level,special_file=None):
-        log_file=None
-        if os.path.isdir(self.path):
-            if (log_level in ['dbg','debug'] or (isinstance(log_level,int) and isinstance(self.dbg_level,int) and self.dbg_level <= log_level <= self.limit)) and isinstance(self.dbg_file,str):
-                log_file=os.path.join(self.path,self.dbg_file)
-            elif log_level in ['info'] and isinstance(self.info_file,str):
-                log_file=os.path.join(self.path,self.info_file)
-            elif log_level in ['error'] and isinstance(self.error_file,str):
-                log_file=os.path.join(self.path,self.error_file)
-            elif isinstance(self.log_file,str) or isinstance(special_file,str):
-                if special_file:
-                    log_file=os.path.join(self.path,special_file)
-                elif log_level in ['dbg','debug','info','error'] or (isinstance(log_level,int) and log_level <= self.limit):
-                    log_file=os.path.join(self.path,self.log_file)
-            if log_file:
-                with open(log_file,'a+') as f:
-                    f.write(log_str)
-        return log_file
-
-    def Screen(self,log_str,log_level):
-        if log_level in ['error']:
-            sys.stderr.write(log_str)
-            sys.stderr.flush()
-        elif log_level <= self.limit:
-            sys.stdout.write(log_str)
-            sys.stdout.flush()
-
-
-    def Log(self,*msg,**opts):
-        direct=opts.get('direct',False)
-        func_name=opts.get('func_name',None)
-        date_format=opts.get('date_format','[%m/%d/%Y %H:%M:%S]')
-        start_new_line=opts.get('start_new_line','\n')
-        end_new_line=opts.get('end_new_line','')
-        log_level=opts.get('log_level',3)
-        special_file=opts.get('filename',None)
-        screen=opts.get('screen',None)
-        syslogd=opts.get('syslogd',None)
-        if msg:
-            # send log at syslogd
-            self.Syslogd(*msg,syslogd=syslogd)
-
-            #if date_format in [False,None,'','no','ignore']:
-            if IsNone(date_format,chk_val=[False,None,'','no','ignore']):
-                date_format=None
-            if IsNone(func_name,chk_val=[False,None,'','no','ignore']):
-                func_name=None
-            if direct:
-                #log_str=' '.join(msg)
-                log_str=Join(msg,symbol=' ')
-            else:
-                log_str=self.Format(*msg,func_name=func_name,date_format=date_format,end_new_line=end_new_line,start_new_line=start_new_line)
-
-            # Saving log at file
-            log_file=self.File(log_str,log_level,special_file=special_file)
-
-            # print at screen
-            if screen is True or (IsNone(screen) and self.screen is True):
-                self.Screen(log_str,log_level)
- 
-            # Send Log Data to logging function (self.log_file)
-            #if log_file is None:
-            if IsNone(log_file):
-                self.Function(log_str)
-
-    def Function(self,*msg,**opts):
-        if type(self.log_file).__name__ == 'function': 
-            log_func_arg=FunctionArgs(self.log_file,mode='all')
-            if 'args' in log_func_arg or 'varargs' in log_func_arg:
-                log_p=True
-                args=log_func_arg.get('args',[])
-                if args and len(args) <= 4 and ('direct' in args or 'log_level' in args or 'func_name' in args):
-                    tmp=[]
-                    for i in range(0,len(args)):
-                        tmp.append(i)
-                    if 'direct' in args:
-                        didx=args.index('direct')
-                        del tmp[didx]
-                        args[didx]=direct
-                    if 'log_level' in args:
-                        lidx=args.index('log_level')
-                        del tmp[lidx]
-                        args[lidx]=log_level
-                    if 'func_name' in args:
-                        lidx=args.index('func_name')
-                        del tmp[lidx]
-                        args[lidx]=func_name
-                    if 'date_format' in args:
-                        lidx=args.index('date_format')
-                        del tmp[lidx]
-                        args[lidx]=date_format
-                    args[tmp[0]]=log_str
-                    self.log_file(*args)
-                elif 'keywards' in log_func_arg:
-                    self.log_file(log_str,direct=direct,log_level=log_level,func_name=func_name,date_format=date_format)
-                elif 'defaults' in log_func_arg:
-                    if 'direct' in log_func_arg['defaults'] and 'log_level' in log_func_arg['defaults']:
-                        self.log_file(log_str,direct=direct,log_level=log_level)
-                    elif 'log_level' in log_func_arg['defaults']:
-                        self.log_file(log_str,log_level=log_level)
-                    elif 'direct' in log_func_arg['defaults']:
-                        self.log_file(log_str,direct=direct)
-                    else:
-                        self.log_file(log_str)
-                else:
-                    self.log_file(log_str)
-
-class HOST:
-    def __init__(self):
-        pass
-
-    def Name(self):
-        return socket.gethostname()
-
-    def DefaultRouteDev(self,default=None,gw=None):
-        for ii in Split(cat('/proc/net/route',no_edge=True),'\n',default=[]):
-            ii_a=ii.split()
-            #if len(ii_a) > 8 and '00000000' == ii_a[1] and '00000000' == ii_a[7]: return ii_a[0]
-            if len(ii_a) < 4 or ii_a[1] != '00000000' or not int(ii_a[3], 16) & 2:
-                #If not default route or not RTF_GATEWAY, skip it
-                continue
-            if gw:
-                if IsSame(socket.inet_ntoa(struct.pack("<L", int(ii_a[2], 16))),gw):
-                    return ii_a[0]
-            else:
-                return ii_a[0]
-        return default
-
-    def DefaultRouteIp(self,default=None):
-        for ii in Split(cat('/proc/net/route',no_edge=True),'\n'):
-            ii_a=ii.split()
-            if len(ii_a) < 4 or ii_a[1] != '00000000' or not int(ii_a[3], 16) & 2:
-                #If not default route or not RTF_GATEWAY, skip it
-                continue
-            return socket.inet_ntoa(struct.pack("<L", int(ii_a[2], 16)))
-        return default
-
-    def Ip(self,ifname=None,mac=None,default=None):
-        if IsNone(ifname):
-            if IsNone(mac) : mac=self.Mac()
-            ifname=self.DevName(mac)
-
-        if ifname:
-            if not os.path.isdir('/sys/class/net/{}'.format(ifname)):
-                return default
-            try:
-                s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-                return socket.inet_ntoa(fcntl.ioctl(
-                    s.fileno(),
-                    0x8915,  # SIOCGIFADDR
-                    struct.pack('256s', ifname[:15])
-                )[20:24])
-            except:
-                try:
-                    return os.popen('ip addr show {}'.format(ifname)).read().split("inet ")[1].split("/")[0]
-                except:
-                    return default
-        return socket.gethostbyname(socket.gethostname())
-
-    def IpmiIp(self,default=None):
-        rt=rshell('''ipmitool lan print 2>/dev/null| grep "IP Address" | grep -v Source | awk '{print $4}' ''')
-        if rt[0]:return rt[1]
-        return default
-
-    def IpmiMac(self,default=None):
-        rt=rshell(""" ipmitool lan print 2>/dev/null | grep "MAC Address" | awk """ + """ '{print $4}' """)
-        if rt[0]:return rt[1]
-        return default
-
-    def Mac(self,ip=None,dev=None,default=None,ifname=None):
-        #if dev is None and ifname: dev=ifname
-        if IsNone(dev) and ifname: dev=ifname
-        if IP(ip).IsV4():
-            dev_info=self.NetDevice()
-            for dev in dev_info.keys():
-                if self.Ip(ifname=dev) == ip:
-                    return dev_info[dev]['mac']
-        #ip or anyother input of device then getting default gw's dev
-        if IsNone(dev): dev=self.DefaultRouteDev()
-        if dev:
-            try:
-                s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-                info = fcntl.ioctl(s.fileno(), 0x8927,  struct.pack('256s', Bytes(dev[:15])))
-                return Join(['%02x' % ord(char) for char in Str(info[18:24])],symbol=':')
-            except:
-                return default
-        #return ':'.join(['{:02x}'.format((uuid.getnode() >> ele) & 0xff) for ele in range(0,8*6,8)][::-1])
-        return MAC('%012x' % uuid.getnode()).FromStr()
-
-    def DevName(self,mac=None,default=None):
-        if IsNone(mac):
-            mac=self.Mac()
-        net_dir='/sys/class/net'
-        if isinstance(mac,str) and os.path.isdir(net_dir):
-            dirpath,dirnames,filenames = list(os.walk(net_dir))[0]
-            for dev in dirnames:
-                fmac=cat('{}/{}/address'.format(dirpath,dev),no_edge=True)
-                if isinstance(fmac,str) and fmac.strip().lower() == mac.lower():
-                    return dev
-        return default
-
-    def Info(self):
-        return {
-         'host_name':self.Name(),
-         'host_ip':self.Ip(),
-         'host_mac':self.Mac(),
-         'ipmi_ip':self.IpmiIp(),
-         'ipmi_mac':self.IpmiMac(),
-         }
-
-    def NetDevice(self,name=None,default=False):
-        def _dev_info_(path,name):
-            drv=ls('{}/{}/device/driver/module/drivers'.format(path,name))
-            if drv is False:
-                drv='unknown'
-            else:
-                drv=drv[0].split(':')[1]
-            return {
-                'mac':cat('{}/{}/address'.format(path,name),no_end_newline=True),
-                'duplex':cat('{}/{}/duplex'.format(path,name),no_end_newline=True,file_only=False),
-                'mtu':cat('{}/{}/mtu'.format(path,name),no_end_newline=True),
-                'state':cat('{}/{}/operstate'.format(path,name),no_end_newline=True),
-                'speed':cat('{}/{}/speed'.format(path,name),no_end_newline=True,file_only=False),
-                'id':cat('{}/{}/ifindex'.format(path,name),no_end_newline=True),
-                'driver':drv,
-                'drv_ver':cat('{}/{}/device/driver/module/version'.format(path,name),no_end_newline=True,file_only=False,default=''),
-                }
-
-
-        net_dev={}
-        net_dir='/sys/class/net'
-        if os.path.isdir(net_dir):
-            dirpath,dirnames,filenames = list(os.walk(net_dir))[0]
-            if name:
-                if name in dirnames:
-                    net_dev[name]=_dev_info_(dirpath,name)
-            else:
-                for dev in dirnames:
-                    net_dev[dev]=_dev_info_(dirpath,dev)
-            return net_dev
-        return default
-
-    def Alive(self,ip,keep=20,interval=3,timeout=1800,default=False,log=None,cancel_func=None):
-        return IP(ip).Online(keep=keep,interval=interval,timeout=timeout,default=default,log=log,cancel_func=cancel_func)[1]
-
-    def Ping(self,ip,keep_good=10,timeout=3600):
-        return IP(ip).Ping(keep_good=10,timeout=timeout)
-
-class FILE:
-    '''
-    sub_dir  : True (Get files in recuring directory)
-    data     : True (Get File Data)
-    md5sum   : True (Get File's MD5 SUM)
-    link2file: True (Make a real file instead sym-link file)
-    '''
-    def __init__(self,*inp,**opts):
-        self.root_path=opts.get('root_path',None)
-        #if self.root_path is None: self.root_path=os.path.dirname(os.path.abspath(__file__))
-        #if self.root_path is None: self.root_path=self.Path()
-        if IsNone(self.root_path): self.root_path=self.Path()
-        info=opts.get('info',None)
-        if isinstance(info,dict):
-            self.info=info
-        else:
-            self.info={}
-            sub_dir=opts.get('sub_dir',opts.get('include_sub_dir',opts.get('include_dir',False)))#???
-            data=opts.get('data',False)
-            md5sum=opts.get('md5sum',False)
-            link2file=opts.get('link2file',False) # If True then copy file-data of sym-link file, so get it real file instead of sym-link file
-            self.filelist={}
-            for filename in inp:
-                root,flist=self.FileList(filename,sub_dir=sub_dir,dirname=True)
-                if root not in self.filelist: self.filelist[root]=[]
-                self.filelist[root]=self.filelist[root]+flist
-            for ff in self.filelist:
-                self.info.update(self.Get(ff,*self.filelist[ff],data=data,md5sum=md5sum,link2file=link2file))
-
-    def FileList(self,name,sub_dir=False,dirname=False,default=[]):
-        if isinstance(name,str):
-            if name[0] == '/':  # Start from root path
-                if os.path.isfile(name) or os.path.islink(name): return os.path.dirname(name),[os.path.basename(name)]
-                if os.path.isdir(name):
-                    if sub_dir:
-                        rt = []
-                        pwd=os.getcwd()
-                        os.chdir(name)
-                        for base, dirs, files in os.walk('.'): 
-                            if dirname: rt.extend(os.path.join(base[2:], d) for d in dirs)
-                            rt.extend(os.path.join(base[2:], f) for f in files)
-                        os.chdir(pwd)
-                        return Path(name),rt
-                    else:
-                        return Path(name),[f for f in os.listdir(name)]
-            elif self.root_path: # start from defined root path
-                #chk_path=os.path.join(self.root_path,name)
-                chk_path=Path(self.root_path,name)
-                if os.path.isfile(chk_path) or os.path.islink(chk_path): return Path(self.root_path),[name]
-                if os.path.isdir(chk_path):
-                    if sub_dir:
-                        rt = []
-                        pwd=os.getcwd()
-                        os.chdir(self.root_path) # Going to defined root path
-                        # Get recuring file list of the name (when current dir then '.')
-                        for base, dirs, files in os.walk(name):
-                            if dirname: rt.extend(os.path.join(base[2:], d) for d in dirs)
-                            rt.extend(os.path.join(base[2:], f) for f in files)
-                        os.chdir(pwd) # recover to the original path
-                        return Path(self.root_path),rt 
-                    else:
-                        if name == '.': name=''
-                        return Path(self.root_path),[os.path.join(name,f) for f in os.listdir('{}/{}'.format(self.root_path,name))]
-        return default
-
-    def CdPath(self,base,path):
-        rt=base
-        for ii in path.split('/'):
-            if ii not in rt: return False
-            rt=rt[ii]
-        return rt
-            
-    def FileName(self,filename):
-        if isinstance(filename,str):
-            filename_info=os.path.basename(filename).split('.')
-            if 'tar' in filename_info:
-                idx=filename_info.index('tar')
-            else:
-                idx=-1
-            #return '.'.join(filename_info[:idx]),'.'.join(filename_info[idx:])
-            return Join(filename_info[:idx],symbol='.'),Join(filename_info[idx:],symbol='.')
-        return None,None
-
-    def FileType(self,filename,default=False):
-        if not isinstance(filename,str) or not os.path.isfile(filename): return default
-        Import('import magic')
-        aa=magic.from_buffer(open(filename,'rb').read(2048))
-        if aa: return aa.split()[0].lower()
-        return 'unknown'
-
-    def GetInfo(self,path=None,*inps):
-        if isinstance(path,str):
-            if not self.info and os.path.exists(path):
-                data={}
-                self.MkInfo(data,path)
-            else:
-                data=self.CdPath(path)
-            if isinstance(data,dict):
-                if not inps and ' i ' in data: return data[' i ']
-                rt=[]
-                for ii in inps:
-                    if ii == 'data' and ii in data: rt.append(data[ii])
-                    if ' i ' in data and ii in data[' i ']: rt.append(data[' i '][ii])
-                return rt
-
-    def Get(self,root_path,*filenames,**opts):
-        data=opts.get('data',False)
-        md5sum=opts.get('md5sum',False)
-        link2file=opts.get('link2file',False)
-        base={}
-
-        def MkInfo(rt,filename=None,**opts):
-            #if not isinstance(rt,dict) or not isinstance(filename,str): return default
-            if ' i ' not in rt: rt[' i ']={}
-            if filename:
-                state=os.stat(filename)
-                rt[' i ']['exist']=True
-                rt[' i ']['size']=state.st_size
-                rt[' i ']['mode']=oct(state.st_mode)[-4:]
-                rt[' i ']['atime']=state.st_atime
-                rt[' i ']['mtime']=state.st_mtime
-                rt[' i ']['ctime']=state.st_ctime
-                rt[' i ']['gid']=state.st_gid
-                rt[' i ']['uid']=state.st_uid
-            if opts: rt[' i '].update(opts)
-
-        def MkPath(base,path,root_path):
-            rt=base
-            chk_dir='{}'.format(root_path)
-            for ii in path.split('/'):
-                if ii:
-                    chk_dir=Path(chk_dir,ii)
-                    if ii not in rt:
-                        rt[ii]={}
-                        if os.path.isdir(chk_dir): MkInfo(rt[ii],chk_dir,type='dir')
-                    rt=rt[ii]
-            return rt
-
-        for filename in filenames:
-            tfilename=Path(root_path,filename)
-            if os.path.exists(tfilename):
-                rt=MkPath(base,filename,root_path)
-                if os.path.islink(tfilename): # it is a Link File
-                    if os.path.isfile(filename): # it is a File
-                        if link2file:
-                            name,ext=self.FileName(tfilename)
-                            _md5=None
-                            if data or md5sum: # MD5SUM or Data
-                                filedata=self.Rw(tfilename,out='byte')
-                                if filedata[0]:
-                                    if data: rt['data']=filedata[1]
-                                    if md5sum: _md5=md5(filedata[1])
-                            MkInfo(rt,filename=tfilename,type=self.FileType(tfilename),name=name,ext=ext,md5=_md5)
-                    else:
-                        MkInfo(rt,filename=tfilename,type='link',dest=os.readlink(tfilename))
-                elif os.path.isdir(tfilename): # it is a directory
-                    MkInfo(rt,tfilename,type='dir')
-                elif os.path.isfile(tfilename): # it is a File
-                    name,ext=self.FileName(tfilename)
-                    _md5=None
-                    if data or md5sum: # MD5SUM or Data
-                        filedata=self.Rw(tfilename,out='byte')
-                        if filedata[0]:
-                            if data: rt['data']=filedata[1]
-                            if md5sum: _md5=md5(filedata[1])
-                    MkInfo(rt,filename=tfilename,type=self.FileType(tfilename),name=name,ext=ext,md5=_md5)
-            else:
-                MkInfo(rt,filename,exist=False)
-        if base:
-            return {root_path:base}
-        return {}
-
-    def GetInfoFile(self,name,roots=None): #get file info dict from Filename path
-        if IsNone(roots): roots=self.FindRP()
-        if isinstance(name,str):
-            for root in roots:
-                rt=self.info.get(root,{})
-                for ii in name.split('/'):
-                    if ii not in rt: break
-                    rt=rt[ii]
-                fileinfo=rt.get(' i ',{})
-                if fileinfo: return fileinfo
-        return False
-
-    def GetList(self,name=None,roots=None): #get file info dict from Filename path
-        if IsNone(roots): roots=self.FindRP()
-        for root in roots:
-            if isinstance(root,str):
-                rt=self.info.get(root,{})
-                if name != root:
-                    rt=self.CdPath(rt,name)
-                if isinstance(rt,dict):
-                    for ii in rt:
-                        if ii == ' i ': continue
-                        if rt[ii].get(' i ',{}).get('type') == 'dir':
-                            print(ii+'/')
-                        else:
-                            print(ii)
-        return False
-
-    def GetFileList(self,name=None,roots=None): #get file info dict from Filename path
-        if IsNone(roots): roots=self.FindRP()
-        for root in roots:
-            if isinstance(root,str):
-                rt=self.info.get(root,{})
-                if name != root:
-                    rt=self.CdPath(rt,name)
-                if isinstance(rt,dict):
-                    for ii in rt:
-                        if ii == ' i ': continue
-                        if rt[ii].get(' i ',{}).get('type') == 'dir': continue
-                        print(ii)
-        return False
-
-    def ExecFile(self,filename,bin_name=None,default=None,work_path='/tmp'):
-        # check the filename is excutable in the system bin file then return the file name
-        # if compressed file then extract the file and find bin_name file in the extracted directory
-        #   and found binary file then return then binary file path
-        # if filename is excutable file then return the file path
-        # if not found then return default value
-        exist=self.GetInfoFile(filename)
-        if exist:
-            if exist['type'] in ['elf'] and exist['mode'] == 33261:return filename
-            if self.Extract(filename,work_path=work_path):
-                if bin_name:
-                    rt=[]
-                    for ff in self.Find(work_path,filename=bin_name):
-                        if self.Info(ff).get('mode') == 33261:
-                            rt.append(ff)
-                    return rt
-        else:
-            if find_executable(filename): return filename
-        return default
-
-    def Basename(self,filename,default=False):
-        if isinstance(filename,str):return os.path.basename(filename)
-        return default
-        
-    def Dirname(self,filename,bin_name=None,default=False):
-        if not isinstance(filename,str): return default
-        if IsNone(bin_name): return os.path.dirname(filename)
-        if not isinstance(bin_name,str): return default
-        bin_info=bin_name.split('/')
-        bin_n=len(bin_info)
-        filename_info=filename.split('/')
-        filename_n=len(filename_info)
-        for ii in range(0,bin_n):
-            if filename_info[filename_n-1-ii] != bin_info[bin_n-1-ii]: return default
-        #return '/'.join(filename_info[:-bin_n])
-        return Join(filename_info[:-bin_n],symbol='/')
-
-    def Find(self,filename,default=[]):
-        if not isinstance(filename,str): return default
-        filename=os.path.basename(filename)
-        if os.path.isdir(self.root_path):
-            rt = []
-            for base, dirs, files in os.walk(self.root_path):
-                found = fnmatch.filter(files, filename)
-                rt.extend(os.path.join(base, f) for f in found)
-            return rt
-        return default
- 
-#    def Decompress(self,filename,work_path='/tmp',info={},del_org_file=False):
-#        if not info and isinstance(filename,str) and os.path.isfile(filename): info=self.Get(filename)
-#        filetype=info.get('type',None)
-#        fileext=info.get('ext',None)
-#        if filetype and fileext:
-#            # Tar stuff
-#            if fileext in ['tgz','tar','tar.gz','tar.bz2','tar.xz'] and filetype in ['gzip','tar','bzip2','lzma','xz','bz2']:
-#                tf=tarfile.open(filename)
-#                tf.extractall(work_path)
-#                tf.close()
-#            elif fileext in ['zip'] and filetype in ['compress']:
-#                with zipfile.ZipFile(filename,'r') as zf:
-#                    zf.extractall(work_path)
-#            if del_org_file: os.unline(filename)
-#            return True
-#        return False
-
-    def Rw(self,name,data=None,out='byte',append=False,read=None,overwrite=True,finfo={},file_only=True,default={'err'}):
-        if isinstance(name,str):
-            #if data is None: # Read from file
-            if IsNone(data): # Read from file
-                if os.path.isfile(name) or (not file_only and os.path.exists(name)):
-                    try:
-                        if read in ['firstread','firstline','first_line','head','readline']:
-                            with open(name,'rb') as f:
-                                data=f.readline()
-                        elif not file_only:
-                            data=os.open(name,os.O_RDONLY)
-                            os.close(data)
-                        else:
-                            with open(name,'rb') as f:
-                                data=f.read()
-                        if out in ['string','str']:
-                            return True,Str(data)
-                        else:
-                            return True,data
-                    except:
-                        pass
-                if default == {'err'}:
-                    return False,'File({}) not found'.format(name)
-                return False,default
-            else: # Write to file
-                file_path=os.path.dirname(name)
-                if not file_path or os.path.isdir(file_path): # current dir or correct directory
-                    if append:
-                        with open(name,'ab') as f:
-                            f.write(Bytes(data))
-                    elif not file_only:
-                        try:
-                            f=os.open(name,os.O_RDWR)
-                            os.write(f,data)
-                            os.close(f)
-                        except:
-                            return False,None
-                    else:
-                        with open(name,'wb') as f:
-                            f.write(Bytes(data))
-                        if isinstance(finfo,dict) and finfo: self.SetIdentity(name,**finfo)
-                        #mode=self.Mode(mode)
-                        #if mode: os.chmod(name,int(mode,base=8))
-                        #if uid and gid: os.chown(name,uid,gid)
-                        #if mtime and atime: os.utime(name,(atime,mtime))# Time update must be at last order
-                    return True,None
-                if default == {'err'}:
-                    return False,'Directory({}) not found'.format(file_path)
-                return False,default
-        if default == {'err'}:
-            return False,'Unknown type({}) filename'.format(name)
-        return False,default
-
-    def Mode(self,val,mode='chmod',default=False):
-        '''
-        convert File Mode to mask
-        mode 
-           'chmod' : default, convert to mask (os.chmod(<file>,<mask>))
-           'int'   : return to int number of oct( ex: 755 )
-           'oct'   : return oct number (string)
-           'str'   : return string (-rwxr--r--)
-        default: False
-        '''
-        def _mode_(oct_data,mode='chmod'):
-            #convert to octal to 8bit mask, int, string
-            if mode == 'chmod':
-                return int(oct_data,base=8)
-            elif mode in ['int',int]:
-                return int(oct_data.replace('o',''),base=10)
-            elif mode in ['str',str]:
-                m=[]
-                #for i in list(str(int(oct_data,base=10))):
-                t=False
-                for n,i in enumerate(str(int(oct_data.replace('o',''),base=10))):
-                    if n == 0:
-                        if i == '1': t=True
-                    if n > 0:
-                        if i == '7':
-                            m.append('rwx')
-                        elif i == '6':
-                            m.append('rw-')
-                        elif i == '5':
-                            m.append('r-x')
-                        elif i == '4':
-                            m.append('r--')
-                        elif i == '3':
-                            m.append('-wx')
-                        elif i == '2':
-                            m.append('-w-')
-                        elif i == '1':
-                            m.append('--x')
-                str_mod=Join(m,'')
-                if t: return str_mod[:-1]+'t'
-                return str_mod
-            return oct_data
-        if isinstance(val,int):
-            #if val > 511:       #stat.st_mode (32768 ~ 33279)
-            #stat.st_mode (file: 32768~36863, directory: 16384 ~ 20479)
-            if 32768 <= val <= 36863 or 16384 <= val <= 20479:   #stat.st_mode
-                #return _mode_(oct(val)[-4:],mode) # to octal number (oct(val)[-4:])
-                return _mode_(oct(val & 0o777),mode) # to octal number (oct(val)[-4:])
-            elif 511 >= val > 63:      #mask
-                return _mode_(oct(val),mode)      # to ocal number(oct(val))
-            else:
-                return _mode_('%04d'%(val),mode)      # to ocal number(oct(val))
-        else:
-            val=Str(val,default=None)
-            if isinstance(val,str):
-                val_len=len(val)
-                num=Int(val,default=None)
-                if isinstance(num,int):
-                    if 3 <= len(val) <=4 and 100 <= num <= 777: #string type of permission number(octal number)
-                        return _mode_('%04d'%(num),mode)
-                else:
-                    val_len=len(val)
-                    if 9<= val_len <=10:
-                        if val_len == 10 and val[0] in ['-','d','s']:
-                            val=val[1:]
-                    else:
-                        StdErr('Bad permission length')
-                        return default
-                    if not all(val[k] in 'rw-' for k in [0,1,3,4,6,7]):
-                        StdErr('Bad permission format (read-write)')
-                        return default
-                    if not all(val[k] in 'xs-' for k in [2,5]):
-                        StdErr('Bad permission format (execute)')
-                        return default
-                    if val[8] not in 'xt-':
-                        StdErr( 'Bad permission format (execute other)')
-                        return default
-                    m = 0
-                    if val[0] == 'r': m |= stat.S_IRUSR
-                    if val[1] == 'w': m |= stat.S_IWUSR
-                    if val[2] == 'x': m |= stat.S_IXUSR
-                    if val[2] == 's': m |= stat.S_IXUSR | stat.S_ISUID
-
-                    if val[3] == 'r': m |= stat.S_IRGRP
-                    if val[4] == 'w': m |= stat.S_IWGRP
-        if isinstance(val,int):
-            #if val > 511:       #stat.st_mode (32768 ~ 33279)
-            #stat.st_mode (file: 32768~36863, directory: 16384 ~ 20479)
-            if 32768 <= val <= 36863 or 16384 <= val <= 20479:   #stat.st_mode
-                #return _mode_(oct(val)[-4:],mode) # to octal number (oct(val)[-4:])
-                return _mode_(oct(val & 0o777),mode) # to octal number (oct(val)[-4:])
-            elif 511 >= val > 63:      #mask
-                return _mode_(oct(val),mode)      # to ocal number(oct(val))
-            else:
-                return _mode_('%04d'%(val),mode)      # to ocal number(oct(val))
-        else:
-            val=Str(val,default=None)
-            if isinstance(val,str):
-                val_len=len(val)
-                num=Int(val,default=None)
-                if isinstance(num,int):
-                    if 3 <= len(val) <=4 and 100 <= num <= 777: #string type of permission number(octal number)
-                        return _mode_('%04d'%(num),mode)
-                else:
-                    val_len=len(val)
-                    if 9<= val_len <=10:
-                        if val_len == 10 and val[0] in ['-','d','s']:
-                            val=val[1:]
-                    else:
-                        StdErr('Bad permission length')
-                        return default
-                    if not all(val[k] in 'rw-' for k in [0,1,3,4,6,7]):
-                        StdErr('Bad permission format (read-write)')
-                        return default
-                    if not all(val[k] in 'xs-' for k in [2,5]):
-                        StdErr('Bad permission format (execute)')
-                        return default
-                    if val[8] not in 'xt-':
-                        StdErr( 'Bad permission format (execute other)')
-                        return default
-                    m = 0
-                    if val[0] == 'r': m |= stat.S_IRUSR
-                    if val[1] == 'w': m |= stat.S_IWUSR
-                    if val[2] == 'x': m |= stat.S_IXUSR
-                    if val[2] == 's': m |= stat.S_IXUSR | stat.S_ISUID
-
-                    if val[3] == 'r': m |= stat.S_IRGRP
-                    if val[4] == 'w': m |= stat.S_IWGRP
-        if isinstance(val,int):
-            #if val > 511:       #stat.st_mode (32768 ~ 33279)
-            #stat.st_mode (file: 32768~36863, directory: 16384 ~ 20479)
-            if 32768 <= val <= 36863 or 16384 <= val <= 20479:   #stat.st_mode
-                #return _mode_(oct(val)[-4:],mode) # to octal number (oct(val)[-4:])
-                return _mode_(oct(val & 0o777),mode) # to octal number (oct(val)[-4:])
-            elif 511 >= val > 63:      #mask
-                return _mode_(oct(val),mode)      # to ocal number(oct(val))
-            else:
-                return _mode_('%04d'%(val),mode)      # to ocal number(oct(val))
-        else:
-            val=Str(val,default=None)
-            if isinstance(val,str):
-                val_len=len(val)
-                num=Int(val,default=None)
-                if isinstance(num,int):
-                    if 3 <= len(val) <=4 and 100 <= num <= 777: #string type of permission number(octal number)
-                        return _mode_('%04d'%(num),mode)
-                else:
-                    val_len=len(val)
-                    if 9<= val_len <=10:
-                        if val_len == 10 and val[0] in ['-','d','s']:
-                            val=val[1:]
-                    else:
-                        StdErr('Bad permission length')
-                        return default
-                    if not all(val[k] in 'rw-' for k in [0,1,3,4,6,7]):
-                        StdErr('Bad permission format (read-write)')
-                        return default
-                    if not all(val[k] in 'xs-' for k in [2,5]):
-                        StdErr('Bad permission format (execute)')
-                        return default
-                    if val[8] not in 'xt-':
-                        StdErr( 'Bad permission format (execute other)')
-                        return default
-                    m = 0
-                    if val[0] == 'r': m |= stat.S_IRUSR
-                    if val[1] == 'w': m |= stat.S_IWUSR
-                    if val[2] == 'x': m |= stat.S_IXUSR
-                    if val[2] == 's': m |= stat.S_IXUSR | stat.S_ISUID
-
-                    if val[3] == 'r': m |= stat.S_IRGRP
-                    if val[4] == 'w': m |= stat.S_IWGRP
-                    if val[5] == 'x': m |= stat.S_IXGRP
-                    if val[5] == 's': m |= stat.S_IXGRP | stat.S_ISGID
-
-                    if val[6] == 'r': m |= stat.S_IROTH
-                    if val[7] == 'w': m |= stat.S_IWOTH
-                    if val[8] == 'x': m |= stat.S_IXOTH
-                    if val[8] == 't': m |= stat.S_IXOTH | stat.S_ISVTX
-                    return _mode_(oct(m),mode)
-        return default
-
-
-    # Find filename's root path and filename according to the db
-    def FindRP(self,filename=None,default=None):
-        if isinstance(filename,str) and self.info:
-            info_keys=list(self.info.keys())
-            info_num=len(info_keys)
-            if filename[0] != '/': 
-                if info_num == 1: return info_keys[0]
-                return self.root_path
-            aa='/'
-            filename_a=filename.split('/')
-            for ii in range(1,len(filename_a)):
-                aa=Path(aa,filename_a[ii]) 
-                if aa in info_keys:
-                    #remain_path='/'.join(filename_a[ii+1:])
-                    remain_path=Join(filename_a[ii+1:],symbol='/')
-                    if info_num == 1: return aa,remain_path
-                    # if info has multi root path then check filename in the db of each root_path
-                    if self.GetInfoFile(remain_path,aa): return aa,remain_path
-        elif self.info:
-            return list(self.info.keys())
-        return default
-            
-    def ExtractRoot(self,**opts):
-        root_path=opts.get('root_path',[])
-        dirpath=opts.get('dirpath')
-        sub_dir=opts.get('sub_dir',False)
-        if isinstance(root_path,str):
-            root_path=[root_path]
-        #if not os.path.isdir(opts.get('dest')): os.makedirs(opts.get('dest'))
-        if self.Mkdir(opts.get('dest'),force=True) is False: return False
-        for rp in root_path:
-            new_dest=opts.get('dest')
-            if dirpath:
-                rt=self.CdPath(self.info[rp],dirpath)
-                if rt is False: 
-                    print('{} not found'.format(dirpath))
-                    return
-            else:
-                dirpath=''
-                rt=self.info[rp]
-
-            rinfo=rt.get(' i ',{})
-            rtype=rinfo.get('type')
-            #dir:directory,None:root directory
-            if not IsNone(rtype,chk_val=['dir',None,'']): # File / Link
-                mydest=os.path.dirname(dirpath)
-                myname=os.path.basename(dirpath)
-                if mydest:
-                    mydest=os.path.join(new_dest,mydest)
-                else:
-                    mydest=new_dest
-                #if not os.path.isdir(mydest): os.makedirs(mydest)
-                if self.Mkdir(mydest,force=True,info=rinfo) is False: return False
-                if rtype == 'link':
-                    os.symlink(rinfo['dest'],os.path.join(mydest,myname))
-                    self.SetIdentity(os.path.join(mydest,myname),**rinfo)
-                else: # File
-                    if 'data' in rt: self.Rw(Path(mydest,myname),data=rt['data'],finfo=rinfo)
-                    else: print('{} file have no data'.format(dirpath))
-#                self.SetIdentity(os.path.join(mydest,myname),**rinfo)
-            else: # directory or root DB
-                for ii in rt:
-                    if ii == ' i ': continue
-                    finfo=rt[ii].get(' i ',{})
-                    ftype=finfo.get('type')
-                    if ftype == 'dir': 
-                        mydir=os.path.join(new_dest,ii)
-                        self.Mkdir(mydir,force=True,info=finfo)
-                        #self.SetIdentity(mydir,**finfo)
-                        # Sub directory
-                        if sub_dir: self.ExtractRoot(dirpath=os.path.join(dirpath,ii),root_path=rp,dest=os.path.join(new_dest,ii),sub_dir=sub_dir)
-                        #if dmtime and datime: os.utime(mydir,(datime,dmtime)) # Time update must be at last order
-                    elif ftype == 'link':
-                        iimm=os.path.join(new_dest,ii)
-                        if not os.path.exists(iimm):
-                            os.symlink(finfo['dest'],iimm)
-                            self.SetIdentity(iimm,**finfo)
-                    else: # File
-                        if 'data' in rt[ii]: self.Rw(os.path.join(new_dest,ii),data=rt[ii]['data'],finfo=finfo)
-                        else: print('{} file have no data'.format(ii))
-
-    def Mkdir(self,path,force=False,info={}):
-        if not isinstance(path,str): return None
-        if os.path.exists(path): return None
-        if force:
-            try:
-                os.makedirs(path)
-                if isinstance(info,dict) and info: self.SetIdentity(path,**info)
-            except:
-                return False
-        else:
-            try:
-                os.mkdir(path)
-                if isinstance(info,dict) and info: self.SetIdentity(path,**info)
-            except:
-                return False
-        return True
-
-    def MkTemp(self,filename=None,suffix='-XXXXXXXX',opt='dry',base_dir='/tmp',custom=None,force=False):
-        if IsNone(filename):
-            filename=os.path.join(base_dir,Random(length=len(suffix)-1,strs=custom,mode='str'))
-        dir_name=os.path.dirname(filename)
-        file_name=os.path.basename(filename)
-        name, ext = os.path.splitext(file_name)
-        if type(suffix) is not str or force is True:
-            suffix='-XXXXXXXX'
-        num_type='.%0{}d'.format(len(suffix)-1)
-        if dir_name == '.':
-            dir_name=os.path.dirname(os.path.realpath(__file__))
-        elif dir_name == '':
-            dir_name=base_dir
-        def new_name(name,ext=None,ext2=None):
-            if ext:
-                if ext2:
-                    return '{}{}{}'.format(name,ext,ext2)
-                return '{}{}'.format(name,ext)
-            if ext2:
-                return '{}{}'.format(name,ext2)
-            return name
-        def new_dest(dest_dir,name,ext=None,force=False):
-            if os.path.isdir(dest_dir) is False:
-                return False
-            i=0
-            new_file=new_name(name,ext)
-            while True:
-                rfile=os.path.join(dest_dir,new_file)
-                if force is False and os.path.exists(rfile) is False:
-                    return rfile
-                force=False
-                if suffix:
-                    if '0' in suffix or 'n' in suffix or 'N' in suffix:
-                        if suffix[-1] not in ['0','n']:
-                            new_file=new_name(name,num_type%i,ext)
-                        else:
-                            new_file=new_name(name,ext,num_type%i)
-                    elif 'x' in suffix or 'X' in suffix:
-                        rnd_str='.{}'.format(Random(length=len(suffix)-1,mode='str'))
-                        if suffix[-1] not in ['X','x']:
-                            new_file=new_name(name,rnd_str,ext)
-                        else:
-                            new_file=new_name(name,ext,rnd_str)
-                    else:
-                        if i == 0:
-                            new_file=new_name(name,ext,'.{}'.format(suffix))
-                        else:
-                            new_file=new_name(name,ext,'.{}.{}'.format(suffix,i))
-                else:
-                    new_file=new_name(name,ext,'.{}'.format(i))
-                i+=1
-        new_dest_file=new_dest(dir_name,name,ext,force=force)
-        if opt in ['file','f']:
-           os.mknode(new_dest_file)
-        elif opt in ['dir','d','directory']:
-           os.mkdir(new_dest_file)
-        else:
-           return new_dest_file
-
-    def SetIdentity(self,path,**opts):
-        if os.path.exists(path):
-            chmod=self.Mode(opts.get('mode',None))
-            uid=opts.get('uid',None)
-            gid=opts.get('gid',None)
-            atime=opts.get('atime',None)
-            mtime=opts.get('mtime',None)
-            try:
-                if chmod: os.chmod(path,int(chmod,base=8))
-                if uid and gid: os.chown(path,uid,gid)
-                if mtime and atime: os.utime(path,(atime,mtime)) # Time update must be at last order
-            except:
-                pass
-
-    def Extract(self,*path,**opts):
-        dest=opts.get('dest',None)
-        root_path=opts.get('root_path',None)
-        sub_dir=opts.get('sub_dir',False)
-        if IsNone(dest): return False
-        if not path: 
-            self.ExtractRoot(root_path=self.FindRP(),dest=dest,sub_dir=sub_dir)
-        else:
-            for filepath in path:
-                fileRF=self.FindRP(filepath)
-                if isinstance(fileRF,tuple):
-                    root_path=[fileRF[0]]
-                    filename=fileRF[1]
-                    self.ExtractRoot(root_path=root_path,dirpath=filename,dest=dest,sub_dir=sub_dir)
-                elif isinstance(fileRF,list):
-                    self.ExtractRoot(root_path=fileRF,dest=dest,sub_dir=sub_dir)
-
-    def Save(self,filename):
-        pv=b'3'
-        if PyVer(2): pv=b'2'
-        #self.Rw(filename,data=pv+bz2.compress(pickle.dumps(self.info,protocol=2)))
-        self.Rw(filename,data=pv+Compress(pickle.dumps(self.info,protocol=2),mode='lz4'))
-
-    def Open(self,filename):
-        if not os.path.isfile(filename):
-            print('{} not found'.format(filename))
-            return False
-        data=self.Rw(filename)
-        if data[0]:
-            pv=data[1][0]
-            if pv == '3' and PyVer(2):
-                print('The data version is not matched. Please use Python3')
-                return False
-            # decompress data
-            try:
-                #dcdata=bz2.BZ2Decompressor().decompress(data[1][1:])
-                dcdata=Decompress(data[1][1:],mode='lz4')
-            except:
-                print('This is not KFILE format')
-                return False
-            try:
-                self.info=pickle.loads(dcdata) # Load data
-            except:
-                try:
-                    self.info=pickle.loads(dcdata,encoding='latin1') # Convert 2 to 3 format
-                except:
-                    print('This is not KFILE format')
-                    return False
-        else:
-            print('Can not read {}'.format(filename))
-            return False
-
-    def Cd(self,data,path,sym='/'):
-        if Type(data,'module') and data == os:
-            if isinstance(path,str):
-                data.chdir(path)
-                return data
-        else:
-            if isinstance(path,int): path='{}'.format(path)
-            for ii in path.split(sym):
-                if isinstance(data,dict):
-                    if ii in data:
-                        data=data[ii]
-                elif isinstance(data,(list,tuple)):
-                    if not isinstance(ii,str) or not ii.isdigit(): continue
-                    ii=int(ii)
-                    if len(data) > ii:
-                        data=data[ii]
-            return data
-
-    def Path(self,filename=None):
-        if filename:
-            return os.path.dirname(os.path.realpath(filename))
-        return os.path.dirname(os.path.realpath((inspect.stack()[-1])[1]))
-        #if '__file__' in globals() : return os.path.dirname(os.path.realpath(__file__))
-
-    def Rm(self,filelist):
-        if isinstance(filelist,str):
-            filelist=filelist.split(',')
-        if isinstance(filelist,(list,tuple)):
-            for ii in list(filelist):
-                if os.path.isfile(ii):
-                    os.unlink(ii)
-                else:
-                    print('not found {0}'.format(ii))
-
-class EMAIL:
-    ############################
-    # GMAIL Information
-    # server  : smtp.gmail.com
-    # SSL Port: 465
-    # user    : email address
-    # password: email password
-    ############################
-    def __init__(self,server='127.0.0.1',port=25,user=None,password=None,ssl=False,tls=False):
-        self.server=server
-        self.port=port
-        self.user=user
-        self.password=password
-        self.ssl=ssl
-        self.tls=tls
-
-    def Body(self,sender,receivers,title,msg,filename=None,html=False):
-        if isinstance(receivers,str):
-            receivers=receivers.split(',')
-        if not isinstance(receivers,list):
-            print('To mailing list issue')
-            return False
-        if filename:
-            _body=MIMEMultipart()
-            if isinstance(sender,tuple) and len(sender) == 2:
-                #format: ('NAME',EMAIL)
-                _body['From'] = email.utils.formataddr(sender)
-            else:
-                _body['From'] = sender
-            if isinstance(receivers[0],tuple) and len(receivers[0]) == 2:
-                #format: ('NAME',EMAIL)
-                _body['To'] = email.utils.formataddr(receivers[0])
-            else:
-                _body['To'] = receivers[0]
-            _body['Subject'] = title
-            if html:
-                _body.attach(MIMEText(msg, "html"))
-            else:
-                _body.attach(MIMEText(msg, "plain"))
-            with open(filename,'rb') as attachment:
-                part=MIMEBase("application", "octet-stream")
-                part.set_payload(attachment.read())
-            encoders.encode_base64(part)
-            part.add_header('Content-Disposition','attachment; filename="{filename}"')
-            _body.attach(part)
-        else:
-            if html:
-                _body=MIMEMultipart('alternative')
-                _body.attach(MIMEText(msg,'html'))
-            else:
-                _body = MIMEText(msg)
-            _body['Subject'] = title
-            if isinstance(sender,tuple) and len(sender) == 2:
-                #format: ('NAME',EMAIL)
-                _body['From'] = email.utils.formataddr(sender)
-            else:
-                _body['From'] = sender
-            if isinstance(receivers[0],tuple) and len(receivers[0]) == 2:
-                #format: ('NAME',EMAIL)
-                _body['To'] = email.utils.formataddr(receivers[0])
-            else:
-                _body['To'] = receivers[0]
-        return _body.as_string()
-
-    def Server(self):
-        if self.ssl:
-            if not self.password:
-                print('It required mail server({}) login password'.format(self.server))
-                return False
-            context = ssl.create_default_context()
-            if IsNone(self.user): self.user=sender
-            try:
-                server=smtplib.SMTP_SSL(self.server,self.port,context=context)
-                server.login(self.user, self.password)
-            except:
-                print('Login fail at the server({})'.format(self.server))
-                return False
-        else:
-            server=smtplib.SMTP(self.server,self.port)
-            if self.tls:
-                if not self.password:
-                    print('It required mail server({}) login password'.format(self.server))
-                    return False
-                if self.ssl:
-                    context = ssl.create_default_context()
-                    server.starttls(context=context)
-                else:
-                    server.starttls()
-                if IsNone(self.user): self.user=sender
-                server.login(self.user, self.password)
-        return server
-
-    #def Send(self,sender,receivers,title='Subject',msg='MSG',dbg=False,filename=None,html=False):
-    def Send(self,*receivers,**opts):
-        sender=opts.get('sender',opts.get('from','root@localhost'))
-        title=opts.get('title',opts.get('subject','Unknown Subject'))
-        msg=opts.get('msg',opts.get('body','No body'))
-        dbg=opts.get('dbg',False)
-        filename=opts.get('filename')
-        html=opts.get('html',False)
-        server=self.Server()
-        if not server: return False
-        if dbg: server.set_debuglevel(True)
-        if len(receivers) == 1 and isinstance(receivers[0],str):
-            receivers=receivers[0].split(',')
-        elif receivers:
-            receivers=list(receivers)
-        else:
-            receivers=opts.get('to',opts.get('recievers'))
-            if isinstance(receivers,str):
-                receivers=receivers.split(',')
-            elif isinstance(receivers,tuple) and len(receivers) == 2 and isinstance(receivers[0],str) and '@' not in receivers[0]:
-                receivers=[receivers]
-        email_body=self.Body(sender,receivers,title,msg,filename=filename,html=html)
-        if email_body:
-            try:
-                server.sendmail(sender, receivers, email_body)
-                server.quit()
-                return True
-            except:
-                return False
-        else:
-            print('something wrong input')
-            return False
-
-class Multiprocessor():
-    def __init__(self):
-        self.processes = []
-        self.queue = Queue()
-
-    @staticmethod
-    def _wrapper(func, queue, args, kwargs):
-        ret = func(*args, **kwargs)
-        queue.put(ret)
-
-    def run(self, func, *args, **kwargs):
-        args2 = [func, self.queue, args, kwargs]
-        p = Process(target=self._wrapper, args=args2)
-        self.processes.append(p)
-        p.start()
-
-    def wait(self):
-        rets = []
-        for p in self.processes[:]:
-            ret = self.queue.get()
-            rets.append(ret)
-            self.processes.remove(p)
-        return rets
-
-class SCREEN:
-    def Kill(self,title):
-        ids=self.Id(title)
-        if len(ids) == 1:
-            rc=rshell('''screen -X -S {} quit'''.format(ids[0]))
-            if rc[0] == 0:
-                return True
-            return False
-
-    def Monitor(self,title,ip,ipmi_user,ipmi_pass,find=[],timeout=600,session_out=10,stdout=False):
-        if type(title) is not str or not title:
-            print('no title')
-            return False
-        scr_id=self.Id(title)
-        if scr_id:
-            print('Already has the title at {}'.format(scr_id))
-            return False
-        
-        if not IP(ip).IsBmcIp(port=(623,664,443)):
-            print('{} is not ipmi ip'.format(ip))
-            return False
-
-        # if Not support SOL 
-        if self.Info(ip,ipmi_user,ipmi_pass)[0] is False:
-            print('The BMC is not support SOL function')
-            return False
-
-        cmd="ipmitool -I lanplus -H {} -U {} -P {} sol activate".format(ip,ipmi_user,ipmi_pass)
-        # Linux OS Boot (Completely kernel loaded): find=['initrd0.img','\xff']
-        # PXE Boot prompt: find=['boot:']
-        # PXE initial : find=['PXE ']
-        # DHCP initial : find=['DHCP']
-        # ex: aa=screen_monitor('test','ipmitool -I lanplus -H <bmc ip> -U ADMIN -P ADMIN sol activate',find=['initrd0.img','\xff'],timeout=300)
-        log_file=self.Log(title,cmd)
-        if not log_file: 
-            return False
-        init_time=TIME().Int()
-        mon_line=0
-        old_mon_line=-1
-        found=0
-        find_num=len(find)
-        time=TIME()
-        while True:
-            if TIME().Int() - init_time > timeout :
-                print('Monitoring timeout({} sec)'.format(timeout))
-                if self.Kill(title):
-                    os.unlink(log_file)
-                break
-            with open(log_file,'rb') as f:
-                tmp=f.read()
-            #tmp=_u_byte2str(tmp)
-            tmp=Str(tmp)
-            if stdout: print(tmp)
-                
-            if '\x1b' in tmp:
-                tmp_a=tmp.split('\x1b')
-            elif '\r\n' in tmp:
-                tmp_a=tmp.split('\r\n')
-            elif '\r' in tmp:
-                tmp_a=tmp.split('\r')
-            else:
-                tmp_a=tmp.split('\n')
-            tmp_n=len(tmp_a)
-            for ss in tmp_a[tmp_n-2:]:
-                if 'SOL Session operational' in ss:
-                    # control+c : "^C", Enter: "^M", any command "<linux command> ^M"
-                    rshell('screen -S {} -p 0 -X stuff "^M"'.format(title))
-                    if time.Out(session_out):
-                        print('maybe not updated any screen information or SOL issue (over {}seconds)'.format(session_out))
-                        if self.Kill(title):
-                            os.unlink(log_file)
-                        return False
-                    TIME().Sleep(2)
-                    continue
-            if find:
-                for ii in tmp_a[mon_line:]:
-                    if find_num == 0:
-                        print(ii)
-                    else:
-                        for ff in range(0,find_num):
-                            find_i=find[found]
-                            if ii.find(find_i) < 0:
-                                break
-                            found=found+1
-                            if found >= find_num:
-                                if self.Kill(title):
-                                    os.unlink(log_file)
-                                return True
-                if tmp_n > 1:
-                    mon_line=tmp_n -1
-                else:
-                    mon_line=tmp_n
-            else:
-                if self.Kill(title):
-                    os.unlink(log_file)
-                return True
-            TIME().Sleep(1)
-
-
-    def Id(self,title=None):
-        scs=[]
-        rc=rshell('''screen -ls''')
-        if rc[0] == 1:
-            for ii in rc[1].split('\n')[1:]:
-                jj=ii.split()
-                if len(jj) == 2:
-                    if title:
-                        zz=jj[0].split('.')
-                        if zz[1] == title:
-                            scs.append(jj[0])
-                    else:
-                        scs.append(jj[0])
-        return scs
-
-    def Log(self,title,cmd):
-        # ipmitool -I lanplus -H 172.16.114.80 -U ADMIN -P ADMIN sol activate
-        pid=os.getpid()
-        tmp_file=FILE().MkTemp('/tmp/.slc.{}_{}.cfg'.format(title,pid))
-        log_file=FILE().MkTemp('/tmp/.screen_ck_{}_{}.log'.format(title,pid))
-        if os.path.isfile(log_file):
-            log_file=''
-        with open(tmp_file,'w') as f:
-            f.write('''logfile {}\nlogfile flush 0\nlog on\n'''.format(log_file))
-        if os.path.isfile(tmp_file):
-            rc=rshell('''screen -c {} -dmSL "{}" {}'''.format(tmp_file,title,cmd))
-            if rc[0] == 0:
-                for ii in range(0,50):
-                    if os.path.isfile(log_file):
-                        os.unlink(tmp_file)
-                        return log_file
-                    TIME().Sleep(0.1)
-            elif rc[0] == 127:
-                print(rc[2])
-                return False
-
-    def Info(self,ip,ipmi_user,ipmi_pass):
-        cmd="ipmitool -I lanplus -H {} -U {} -P '{}' sol info".format(ip,ipmi_user,ipmi_pass)
-        rc=rshell(cmd)
-        enable=False
-        channel=1
-        rate=9600
-        port=623
-        if rc[0] == 0:
-            for ii in rc[1].split('\n'):
-                ii_a=ii.split()
-                if ii_a[0] == 'Enabled' and ii_a[-1] == 'true':
-                    enable=True
-                elif ii_a[0] == 'Volatile':
-                    if '.' in ii_a[-1]:
-                        try:
-                            rate=int(float(ii_a[-1]) * 1000)
-                        except:
-                            pass
-                    else:
-                        try:
-                            rate=int(ii_a[-1])
-                        except:
-                            pass
-                elif ii_a[0] == 'Payload':
-                    if ii_a[1] == 'Channel':
-                        try:
-                            channel=int(ii_a[-2])
-                        except:
-                            pass
-                    elif ii_a[1] == 'Port':
-                        try:
-                            port=int(ii_a[-1])
-                        except:
-                            pass
-        return enable,rate,channel,port,'~~~ console=ttyS1,{}'.format(rate)
-                
-####################################STRING##################################################
-def cut_string(string,max_len=None,sub_len=None,new_line='\n',front_space=False,out_format=list):
-    if TypeName(string) not in ['str','bytes']:
-        string='{0}'.format(string)
-    if not isinstance(max_len,int):
-        if out_format in [str,'str','string']: return string
-        return [string]
-
-    tmp=[]
-    space=Space(max_len-sub_len) if isinstance(sub_len,int) else ''
-    for ii in string.split(new_line):
-        ll=Cut(ii,head_len=max_len,body_len=sub_len,out=list)
-        tmp.append(Join(ll,new_line,append_front=space))
-    if out_format in [str,'str','string']: return Join(tmp,new_line)
-    return tmp
-
-####################################KEYS##################################################
-def Insert(src,*inps,**opts):
-    start=opts.pop('at',0)
-    default=opts.pop('default',False)
-    err=opts.pop('err',False)
-    force=opts.pop('force',False)
-    uniq=opts.pop('uniq',False)
-    if isinstance(src,(list,tuple,str)):
-        tuple_out=False
-        if isinstance(src,tuple) and force:
-            src=list(src)
-            tuple_out=True
-        if uniq:
-            new=[]
-            for ii in inps:
-                if ii not in src:
-                    new.append(ii)
-            inps=tuple(new)
-        if isinstance(at,str):
-            if at in ['start','first']: src=list(inps)+src
-            if at in ['end','last']: src=src+list(inps)
-        elif len(src) == 0:
-            src=list(inps)
-        elif isinstance(start,int) and len(src) > start:
-            src=src[:start]+list(inps)+src[start:]
-        else:
-            if err:
-                return default
-            src=src+list(inps)
-        if tuple_out: return tuple(src)
-    elif isinstance(src,dict):
-        for ii in inps:
-            if isinstance(ii,dict):
-                 src.update(ii)
-        if opts:
-            src.update(opts)
-    return src
-
-def FirstKey(src,default=None):
-    return Next(src,default=default)
-
-def code_error(email_func=None,email=None,email_title=None,email_server=None,log=None,log_msg='',default=None):
-    log_msg=ExceptMessage(msg=log_msg,default=default)
-    if log_msg != default:
-        if log: log('\n!!ERROR!!: {}'.format(log_msg),log_level=1)
-        if email_func and email and email_title:
-            a=email_func(email,email_title,log_msg,dj_ip=email_server)
-            TIME().Sleep(5)
-    return default
-
-def DirName(src,default=None):
-    dirname=Path(src,default=default)
-    if dirname == default: return default
-    if dirname == '': return '.'
-    return dirname
-
-def Args2Str(args,default='org'):
-    if isinstance(args,(tuple,list)):
-        args=list(args)
-        for i in range(0,len(args)):
-            if "'" in args[i]:
-                args[i]='''"{}"'''.format(args[i])
-            elif '"' in args[i]:
-                args[i]="""'{}'""".format(args[i])
-            elif ' ' in args[i]:
-                args[i]='''"{}"'''.format(args[i])
-        return ' '.join(args)
-    return args
-
-def check_value(src,find,idx=None):
-    '''Check key or value in the dict, list or tuple then True, not then False'''
-    if isinstance(src, (list,tuple,str,dict)):
-        if idx is None:
-            if find in src:
-                return True
-        else:
-            if isinstance(src,str):
-                if idx < 0:
-                    if src[idx-len(find):idx] == find:
-                        return True
-                else:
-                    if src[idx:idx+len(find)] == find:
-                        return True
-            else:
-                if Get(src,idx,out='raw') == find:
-                    return True
-    return False
-
-def Update(src,*inps,**opts):
-    at=opts.pop('at',0)
-    err=opts.pop('err',False)
-    default=opts.pop('default',False)
-    force=opts.pop('force',False)
-    sym=opts.pop('sym',None)
-    if isinstance(src,(list,tuple,str)):
-        if isinstance(src,str) and sym: src=src.split(sym)
-        tuple_out=False
-        if isinstance(src,tuple) and force:
-            src=list(src)
-            tuple_out=True
-        n=len(src)
-        if n == 0:
-            if err is True:
-                return default
-            else:
-                src=list(inps)
-        elif isinstance(at,int) and n > at:
-            for i in range(0,len(inps)):
-                if n > at+i:
-                    src[at+i]=inps[i]
-                elif err is True:
-                    return default
-                else:
-                    src=src+list(inps)[i:]
-                    break
-        elif isinstance(at,(tuple,list)):
-            if len(inps) == len(at):
-                for i in range(0,len(at)):
-                    if isinstance(at[i],int) and n > at[i]:
-                        src[at[i]]=inps[i]
-                    elif err is True:
-                        return default
-                    else:
-                        src.append(inps[i])
-        if tuple_out: return tuple(src)
-        return src
-    elif isinstance(src,dict):
-        for ii in inps:
-           if isinstance(ii,dict):
-               src.update(ii)
-        if opts:
-           src.update(opts)
-    return src
-
-def Random(length=8,strs=None,mode='*',letter='*',default=1):
-    if mode in [int,'int','num','number']:
-        if isinstance(strs,(list,tuple)) and len(strs) == 2:
-            try:
-                s=int(strs[0])
-                n=int(strs[1])
-                return random.randint(s,n)
-            except:
-                pass
-        s=0
-        n=''
-        for i in range(0,length):
-            n=n+'9'
-        if n:
-            return random.randint(s,int(n))
-        return default
-    new=''
-#    if mode in [int,'int','num']:
-#        for i in range(0,length):
-#            new='{0}{1}'.format(new,random.randint(0,9))
-#        return int(num)
-    if not isinstance(strs,str) or not strs:
-        strs=''
-        if 'alpha' in mode or mode in ['all','*']:
-            if letter == 'upper':
-                strs=string.ascii_uppercase
-            elif letter == 'lower':
-                strs=string.ascii_lowercase
-            elif letter in ['*','all']:
-                strs=string.ascii_letters
-        if 'num' in mode or mode in ['all','*']:
-            strs=strs+string.digits
-        if 'char' in mode or 'sym' in mode or mode in ['all','*']:
-            strs=strs+string.punctuation
-#        if mode in ['all','*','alphanumchar']:
-#            strs='0aA-1b+2Bc=C3d_D,4.eE?5"fF6g7G!h8H@i9#Ij$JkK%lLmMn^N&oO*p(Pq)Q/r\Rs:St;TuUv{V<wW}x[Xy>Y]z|Z'
-#        elif mode in ['alphachar']:
-#            strs='aA-b+Bc=Cd_D,.eE?"fFgG!hH@i#Ij$JkK%lLmMn^N&oO*p(Pq)Q/r\Rs:St;TuUv{V<wW}x[Xy>Y]z|Z'
-#        elif mode in ['alphanum']:
-#            strs='aA1b2BcC3dD4eE5fF6g7Gh8Hi9IjJkKlLmMnNoOpPqQrRsStTuUvVwWxXyYzZ'
-#        elif mode in ['char']:
-#            strs='-+=_,.?"!@#$%^&*()/\:;{<}x[>]|'
-#        else:
-#            strs='aAbBcCdDeEfFgGhHiIjJkKlLmMnNoOpPqQrRsStTuUvVwWxXyYzZ'
-    if not strs: strs=string.ascii_letters
-    strn=len(strs)-1
-    for i in range(0,length):
-        new='{0}{1}'.format(new,strs[random.randint(0,strn)])
-    return new
-
-def Keys(src,find=None,start=None,end=None,sym='\n',default=[],word=False,pattern=False,findall=False,out=None):
-    rt=[]
-    if isinstance(src,str,list,tuple) and find:
-        if isinstance(src,str): src=src.split(sym)
-
-        for row in range(0,len(src)):
-            for ff in FIND().Find(find,src=src[row],pattern=pattern,word=word,findall=findall,default=[],out=list):
-                if findall:
-                    rt=rt+[(row,[m.start() for m in re.finditer(ff,src[row])])]
-                else:
-                    idx=src[row].index(ff,start,end)
-                    if idx >= 0:
-                        rt.append((row,idx))
-    elif isinstance(src,dict):
-        #if find is None:
-        if IsNone(find):
-            #if out in ['raw',None] and len(src.keys()) == 1 : return list(src.keys())[0]
-            if IsNone(out,chk_val=['raw',None,'']) and len(src.keys()) == 1 : return list(src.keys())[0]
-            if out in ['tuple',tuple]: return tuple(list(src.keys()))
-            return list(src.keys())
-        # if it has found need code for recurring search at each all data and path of keys
-        # return [ (keypath,[found data]), .... ]
-    #elif Type(src,'instance','classobj'):
-    # if src is instance or classobj then search in description and made function name at key
-    if rt:
-        if out in ['tuple',tuple]: return tuple(rt)
-        if out not in ['list',list] and len(rt) == 1 and rt[0][0] == 0:
-            if len(rt[0][1]) == 1:return rt[0][1][0]
-            return rt[0][1]
-        return rt
-    return default
-
-def findXML(xmlfile,find_name=None,find_path=None,default=None,out='xmlobj',get_opt=None):
-    #<Menu name="Security">
-    #  <Setting name="Administrator Password" type="Password">
-    #    <Information>
-    #      <HasPassword>False</HasPassword>
-    #    </Information>
-    #  </Setting>
-    #</Menu>
-    #findXML(cfg_file,find_name='Administrator Password',find_path='./Information/HasPassword',out='data'))
-    # => False
-    if os.path.isfile(xmlfile):
-        try:
-            tree=ET.parse(xmlfile)
-            root=tree.getroot()
-        except:
-            return default
-    else:
-        try:
-            root=ET.fromstring(xmlfile)
-        except:
-            return default
-    def find(tr,find_name):
-        for x in tr:
-            if x.attrib.get('name') == find_name:
-                return x,x.tag
-            rt,pp=find(x,find_name)
-            if rt:
-                return rt,'{}/{}'.format(x.tag,pp)
-        return None,None
-    found_root=None
-    if find_name:
-        found=find(root,find_name)
-        if found[0]:
-             found_root=found[0]
-    if find_path and isinstance(find_path,str):
-        #ex: root.findall('./Menu/Setting/[@name="Administrator Password"]/Information/HasPassword'):
-        if not found_root: found_root=root
-        found_result=found_root.findall(find_path)
-        # <element>.tag: name, .text: data, .attrib: dict
-        rt=[]
-        if out in ['tag','name']:
-            for ii in found_result:
-                rt.append(ii.tag)
-        elif out in ['text','data']:
-            for ii in found_result:
-                if get_opt:
-                    rt.append(ii.get(get_opt,default))
-                else:
-                    rt.append(ii.text)
-        elif out in ['attrib','att']:
-            for ii in found_result:
-                rt.append(ii.attrib)
-        if rt:
-            return rt
-        else:
-            return found_result
-    else:
-        if found_root:
-            if out in ['tag','name']:
-                return found_root.tag
-            elif out in ['text','data']:
-                if get_opt:
-                    return found_root.get(get_opt,default)
-                else:
-                    return found_root.text
-            elif out in ['attrib','att']:
-                return found_root.attrib
-            return found_root
-    return default
-
-def Compress(data,mode='lz4'):
-    if mode == 'lz4':
-        Import('from lz4 import frame')
-        return frame.compress(data)
-    elif mode == 'bz2':
-        Import('import bz2')
-        return bz2.compress(data)
-
-def Decompress(data,mode='lz4',work_path='/tmp',del_org_file=False,file_info={}):
-    def FileName(filename):
-        if isinstance(filename,str):
-            filename_info=os.path.basename(filename).split('.')
-            if 'tar' in filename_info:
-                idx=filename_info.index('tar')
-            else:
-                idx=-1
-            #return '.'.join(filename_info[:idx]),'.'.join(filename_info[idx:])
-            return Join(filename_info[:idx],symbol='.'),Join(filename_info[idx:],symbol='.')
-        return None,None
-
-    def FileType(filename,default=False):
-        if not isinstance(filename,str) or not os.path.isfile(filename): return default
-        Import('import magic')
-        aa=magic.from_buffer(open(filename,'rb').read(2048))
-        if aa: return aa.split()[0].lower()
-        return 'unknown'
-
-    if mode == 'lz4':
-        Import('from lz4 import frame')
-        return frame.decompress(data)
-    elif mode == 'bz2':
-        Import('import bz2')
-        return bz2.BZ2Decompressor().decompress(data)
-    elif mode == 'file' and isinstance(data,str) and os.path.isfile(data):
-        filename,fileextfile_info=FileName(data)
-        filetype=FileType(data)
-        if filetype and fileext:
-            # Tar stuff
-            if fileext in ['tgz','tar','tar.gz','tar.bz2','tar.xz'] and filetype in ['gzip','tar','bzip2','lzma','xz','bz2']:
-                tf=tarfile.open(data)
-                tf.extractall(work_path)
-                tf.close()
-            elif fileext in ['zip'] and filetype in ['compress']:
-                with zipfile.ZipFile(data,'r') as zf:
-                    zf.extractall(work_path)
-            if del_org_file: os.unline(data)
-            return True
-
-def cat(filename,no_end_newline=False,no_edge=False,byte=False,newline='\n',no_first_newline=False,no_all_newline=False,file_only=True,default={'err'}):
-    tmp=FILE().Rw(filename,file_only=file_only,default=default)
-    tmp=Get(tmp,1)
-    if no_edge:
-        return STR(tmp).RemoveNewline(mode='edge',byte=byte,newline=newline)
-    elif no_end_newline:
-        return STR(tmp).RemoveNewline(mode='end',byte=byte,newline=newline)
-    elif no_first_newline:
-        return STR(tmp).RemoveNewline(mode='first',byte=byte,newline=newline)
-    elif no_all_newline:
-        return STR(tmp).RemoveNewline(mode='all',byte=byte,newline=newline)
-    return tmp
-
-def ls(dirname,opt=''):
-    if not IsNone(dirname) and os.path.isdir(dirname):
-        dirlist=[]
-        dirinfo_a=list(os.walk(dirname))
-        if not IsNone(dirinfo_a):
-            dirinfo=dirinfo_a[0]
-            if opt == 'd':
-                dirlist=Get(dirinfo,1)
-            elif opt == 'f':
-                dirlist=Get(dirinfo,2)
-            else:
-                dirlist=Get(dirinfo,1)+Get(dirinfo,2)
-            return dirlist
-    return False
-
-def append(src,addendum):
-    type_src=type(src)
-    type_data=type(addendum)
-    if IsNone(src):
-        if type_data is str:
-            src=''
-        elif type_data is dict:
-            src={}
-        elif type_data is list:
-            src=[]
-        elif type_data is tuple:
-            src=()
-        type_src=type(src)
-    if IsNone(addendum):
-        return src
-    if type_src == type_data:
-        if type_src is dict:
-            return src.update(addendum)
-        elif type_src in [list,tuple]:
-            src=list(src)
-            for ii in addendum:
-                if ii not in src:
-                    src.append(ii)
-            if type_src is tuple:
-                src=tuple(src)
-            return src
-        elif type_src is str:
-            return src+addendum
-    return False
-
-def is_lost(ip,**opts):
-    timeout=opts.get('timeout',opts.get('timeout_sec',1800))
-    interval=opts.get('interval',5)
-    stop_func=opts.get('stop_func',None)
-    cancel_func=opts.get('cancel_func',None)
-    log=opts.get('log',None)
-    init_time=None
-    if not ping(ip,count=3):
-        if not ping(ip,count=0,timeout=timeout,keep_good=30,interval=2,stop_func=stop_func,log=log,cancel_func=cancel_func):
-            return True,'Lost network'
-    return False,'OK'
-
-def is_comeback(ip,**opts):
-    timeout=opts.get('timeout',opts.get('timeout_sec',1800))
-    interval=opts.get('interval',3)
-    keep=opts.get('keep',20)
-    stop_func=opts.get('stop_func',None)
-    cancel_func=opts.get('cancel_func',None)
-    log=opts.get('log',None)
-    init_time=None
-    run_time=TIME().Int()
-    if IsNone(keep,chk_val=[None,'',0]):
-        return True,'N/A(Missing keep parameter data)'
-    if log:
-        log('[',direct=True,log_level=1)
-    time=TIME()
-    while True:
-        if time.Out(timeout):
-            if log:
-                log(']\n',direct=True,log_level=1)
-            return False,'Timeout monitor'
-        if IsCancel(cancel_func) or stop_func is True:
-            if log:
-                log(']\n',direct=True,log_level=1)
-            return True,'Stopped monitor by Custom'
-        if ping(ip,cancel_func=cancel_func):
-            if (TIME().Int() - run_time) > keep:
-                if log:
-                    log(']\n',direct=True,log_level=1)
-                return True,'OK'
-            if log:
-                log('-',direct=True,log_level=1)
-        else:
-            run_time=TIME().Int()
-            if log:
-                log('.',direct=True,log_level=1)
-        TIME().Sleep(interval)
-    if log:
-        log(']\n',direct=True,log_level=1)
-    return False,'Timeout/Unknown issue'
-
-def get_file(filename,**opts):
-    #return FILE(filename,**opts)
-    md5sum=opts.get('md5sum',False)
-    data=opts.get('data',False)
-    include_dir=opts.get('include_dir',False)
-    include_sub_dir=opts.get('include_sub_dir',False)
-
-    def get_file_data(filename,root_path=None):
-        rc={'name':os.path.basename(filename),'path':os.path.dirname(filename),'exist':False,'dir':False,'link':False}
-        if root_path:
-            in_filename=os.path.join(root_path,filename)
-        else:
-            in_filename=filename
-        if os.path.exists(in_filename):
-            fstat=os.stat(in_filename)
-            rc['uid']=fstat.st_uid
-            rc['gid']=fstat.st_gid
-            rc['size']=fstat.st_size
-            rc['atime']=fstat.st_atime
-            rc['mtime']=fstat.st_mtime
-            rc['ctime']=fstat.st_ctime
-            rc['inod']=fstat.st_ino
-            rc['mode']=oct(fstat.st_mode)[-4:]
-            rc['exist']=True
-            if os.path.islink(in_filename):
-                rc['link']=True
-            else:
-                rc['link']=False
-                if os.path.isdir(in_filename):
-                    rc['dir']=True
-                    rc['path']=in_filename
-                    rc['name']=''
-                else:
-                    rc['dir']=False
-                    if md5sum or data:
-                        with open(in_filename,'rb') as f:
-                            fdata=f.read()
-                        if md5sum:
-                            rc['md5']=md5(fdata)
-                        if data:
-                            rc['data']=fdata
-        return rc
-
-    rc={'exist':False,'includes':[]}
-    if type(filename) is str:
-        rc.update(get_file_data(filename))
-        if rc['dir']:
-            root_path=filename
-            real_filename=None
-        else:
-            root_path=os.path.dirname(filename)
-            real_filename=os.path.basename(filename)
-        if include_dir:
-            pwd=os.getcwd()
-            os.chdir(root_path)
-            for dirPath, subDirs, fileList in os.walk('.'):
-                for sfile in fileList:
-                    curFile=os.path.join(dirPath.replace('./',''),sfile)
-                    if curFile != real_filename:
-                        rc['includes'].append(get_file_data(curFile,root_path))
-                if include_sub_dir is False:
-                    break
-            os.chdir(pwd)
-    return rc
-
-def save_file(data,dest,filename=None):
-#    return data.Extract(dest=dest,sub_dir=True)
-    if not isinstance(data,dict) or not isinstance(dest,str) : return False
-    if os.path.isdir(dest) is False: os.system('mkdir -p {0}'.format(dest))
-    if data.get('dir'):
-        fmode=file_mode(data.get('mode'))
-        if fmode:
-            os.chmod(dest,fmode)
-    else:
-        # if file then save
-        if isinstance(filename,str) and filename:
-            new_file=os.path.join(dest,filename)
-        else:
-            new_file=os.path.join(dest,data['name'])
-        if 'data' in data:
-            with open(new_file,'wb') as f:
-                f.write(data['data'])
-        chmod_mode=file_mode(data.get('mode'))
-        if chmod_mode:
-            os.chmod(new_file,chmod_mode)
-    if 'includes' in data and data['includes']: # If include directory or files 
-        for ii in data['includes']:
-            if ii['path']:
-                sub_dir=os.path.join(dest,ii['path'])
-            else:
-                sub_dir='{}'.format(dest)
-            if os.path.isdir(sub_dir) is False: os.system('mkdir -p {}'.format(sub_dir))
-            sub_file=os.path.join(sub_dir,ii['name'])
-            with open(sub_file,'wb') as f:
-                f.write(ii['data'])
-            chmod_mode=file_mode(ii.get('mode'))
-            if chmod_mode:
-                os.chmod(sub_file,chmod_mode)
-
-#########################################################################
-def error_exit(msg=None):
-    if not IsNone(msg):
-       print(msg)
-    sys.exit(-1)
-
-
 def log_format(*msg,**opts):
     log_date_format=opts.get('date_format','[%m/%d/%Y %H:%M:%S]')
     func_name=opts.get('func_name',False)
     log_intro=opts.get('log_intro',3)
     end_new_line=opts.get('end_new_line','')
     start_new_line=opts.get('start_new_line','\n')
     if len(msg) > 0:
         m_str=None
         intro=''
         intro_space=''
         if log_date_format:
-            intro=TIME().Format(tformat=log_date_format)+' '
+            intro=format_time(tformat=log_date_format)+' '
         if func_name or log_intro > 3:
             if type(func_name) is str:
                 intro=intro+'{0} '.format(func_name)
             else:
-                intro=intro+'{0}() '.format(CallerName())
+                intro=intro+'{0}() '.format(get_caller_fcuntion_name())
         if intro:
            for i in range(0,len(intro)+1):
                intro_space=intro_space+' '
         for m in list(msg):
-            if IsNone(m_str):
+            if m_str is None:
                 m_str='{0}{1}{2}{3}'.format(start_new_line,intro,m,end_new_line)
             else:
                 m_str='{0}{1}{2}{3}{4}'.format(start_new_line,m_str,intro_space,m,end_new_line)
         return m_str
 
+def dget(dict=None,keys=None):
+    if dict is None or keys is None:
+        return False
+    tmp=dict.copy()
+    for ii in keys.split('/'):
+        if ii in tmp:
+           dtmp=tmp[ii]
+        else:
+           return False
+        tmp=dtmp
+    return tmp
+
+def dput(dic=None,keys=None,val=None,force=False,safe=True):
+    if dic is not None and keys:
+        tmp=dic
+        keys_arr=keys.split('/')
+        keys_num=len(keys_arr)
+        for ii in keys_arr[:(keys_num-1)]:
+            if ii in tmp:
+                if type(tmp[ii]) == type({}):
+                    dtmp=tmp[ii]
+                else:
+                    if tmp[ii] == None:
+                        tmp[ii]={}
+                        dtmp=tmp[ii]
+                    else:
+                        if force:
+                            vtmp=tmp[ii]
+                            tmp[ii]={vtmp:None}
+                            dtmp=tmp[ii]
+                        else:
+                            return False
+            else:
+                if force:
+                    tmp[ii]={}
+                    dtmp=tmp[ii]
+                else:
+                    return False
+            tmp=dtmp
+        if val == '_blank_':
+            val={}
+        if keys_arr[keys_num-1] in tmp.keys():
+            if safe:
+                if tmp[keys_arr[keys_num-1]]:
+                    return False
+            tmp.update({keys_arr[keys_num-1]:val})
+            return True
+        else:
+            if force:
+                tmp.update({keys_arr[keys_num-1]:val})
+                return True
+    return False
+
+def sendanmail(to,subj,msg,html=True):
+    msg='''{}'''.format(msg)
+    msg=msg.replace('"','\\"')
+    if html:
+        email_msg='''To: {0}
+Subject: {1}  
+Content-Type: text/html
+<html>
+<body>
+<pre>
+{2}
+</pre>
+</body>
+</html>'''.format(to,subj,msg)
+    else:
+        email_msg=''
+    cmd='''echo "{0}" | sendmail -t'''.format(email_msg)
+    return rshell(cmd)
+
+#def mac2str(mac,case='lower'):
+#    if is_mac4(mac):
+#        if case == 'lower':
+#            mac=mac.strip().replace(':','').replace('-','').lower()
+#        else:
+#            mac=mac.strip().replace(':','').replace('-','').upper()
+#        return mac
+#    return False
+
+#def str2mac(mac,sym=':',case='lower',chk=False):
+#    if type(mac) is str:
+#        cmac=mac.strip()
+#        if len(cmac) in [12,17]:
+#            cmac=cmac.replace(':','').replace('-','')
+#            if len(cmac) == 12:
+#                cmac=sym.join(cmac[i:i+2] for i in range(0,12,2))
+#            if case == 'lower':
+#                mac=cmac.lower()
+#            else:
+#                mac=cmac.upper()
+#    if chk:
+#        if is_mac4(mac,convert=False):
+#            return mac
+#        else:
+#            return False
+#    return mac
+
+#def is_mac4(mac=None,symbol=':',convert=True):
+#    if convert:
+#        mac=str2mac(mac,sym=symbol)
+#    if mac is None or type(mac) is not str:
+#        return False
+#    octets = mac.split(symbol)
+#    if len(octets) != 6:
+#        return False
+#    for i in octets:
+#        try:
+#           if len(i) != 2 or int(i, 16) > 255:
+#               return False
+#        except:
+#           return False
+#    return True
+
+def sreplace(pattern,sub,string):
+    return re.sub('^%s' % pattern, sub, string)
+
+def ereplace(pattern,sub,string):
+    return re.sub('%s$' % pattern, sub, string)
+
 def md5(string):
-    return hashlib.md5(Bytes(string)).hexdigest()
+    return hashlib.md5(_u_bytes(string)).hexdigest()
+
+def get_function_name():
+    return traceback.extract_stack(None, 2)[0][2]
+
+def get_pfunction_name():
+    return traceback.extract_stack(None, 3)[0][2]
 
 def ipmi_cmd(cmd,ipmi_ip=None,ipmi_user='ADMIN',ipmi_pass='ADMIN',log=None):
-    if IsNone(ipmi_ip):
+    if ipmi_ip is None:
         ipmi_str=""" ipmitool {0} """.format(cmd)
     else:
         ipmi_str=""" ipmitool -I lanplus -H {0} -U {1} -P '{2}' {3} """.format(ipmi_ip,ipmi_user,ipmi_pass,cmd)
     if log:
         log(' ipmi_cmd():{}'.format(ipmi_str),log_level=7)
     return rshell(ipmi_str)
 
-    
-def get_ipmi_mac(ipmi_ip=None,ipmi_user='ADMIN',ipmi_pass='ADMIN',loop=0):
+def get_ipmi_mac(ipmi_ip=None,ipmi_user='ADMIN',ipmi_pass='ADMIN'):
     ipmi_mac_str=None
-    if IsNone(ipmi_ip):
+    if ipmi_ip is None:
         ipmi_mac_str=""" ipmitool lan print 2>/dev/null | grep "MAC Address" | awk """
-    elif IpV4(ipmi_ip):
+    elif is_ipv4(ipmi_ip):
         ipmi_mac_str=""" ipmitool -I lanplus -H {0} -U {1} -P {2} lan print 2>/dev/null | grep "MAC Address" | awk """.format(ipmi_ip,ipmi_user,ipmi_pass)
-    if not IsNone(ipmi_mac_str):
+    if ipmi_mac_str is not None:
         ipmi_mac_str=ipmi_mac_str + """ '{print $4}' """
-        if not loop:
-            return rshell(ipmi_mac_str)
-        else:
-            for i in range(0,int(loop)):
-                mm=rshell(ipmi_mac_str)
-                if mm[1]:
-                    return mm
-                time.sleep(3)
-    return False,''
+        return rshell(ipmi_mac_str)
 
 def get_ipmi_ip():
     return rshell('''ipmitool lan print 2>/dev/null| grep "IP Address" | grep -v Source | awk '{print $4}' ''')
 
+def get_host_name():
+    return socket.gethostname()
+
+def get_host_ip(ifname=None,mac=None):
+    if ifname or mac:
+        if mac:
+            ifname=get_dev_name_from_mac(mac)
+        return get_net_dev_ip(ifname)
+    else:
+        ifname=get_default_route_dev()
+        if not ifname:
+            ifname=get_dev_name_from_mac()
+        if not ifname: ifname=get_dev_name_from_mac()
+        if ifname:
+            ip=get_net_dev_ip(ifname)
+            if ip:
+                return ip
+        return socket.gethostbyname(socket.gethostname())
+
+def get_default_route_dev():
+    for ii in cat('/proc/net/route').split('\n'):
+        ii_a=ii.split()
+        if len(ii_a) > 8 and '00000000' == ii_a[1] and '00000000' == ii_a[7]: return ii_a[0]
+
+def get_dev_name_from_mac(mac=None):
+    if mac is None:
+        mac=get_host_mac()
+    net_dir='/sys/class/net'
+    if type(mac) is str and os.path.isdir(net_dir):
+        dirpath,dirnames,filenames = list(os.walk(net_dir))[0]
+        for dev in dirnames:
+            fmac=cat('{}/{}/address'.format(dirpath,dev),no_end_newline=True)
+            if type(fmac) is str and fmac.strip().lower() == mac.lower():
+                return dev
+
+def get_dev_mac(ifname):
+    try:
+        s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+        info = fcntl.ioctl(s.fileno(), 0x8927,  struct.pack('256s', ifname[:15]))
+        return ':'.join(['%02x' % ord(char) for char in info[18:24]])
+    except:
+        return
+
+def get_host_iface():
+    if os.path.isfile('/proc/net/route'):
+        routes=cat('/proc/net/route')
+        for ii in routes.split('\n'):
+            ii_a=ii.split()
+            if ii_a[2] == '030010AC':
+                return ii_a[0]
+    
+def get_host_mac(ip=None,dev=None):
+    if is_ipv4(ip):
+        dev_info=get_net_device()
+        if isinstance(dev_info,dict):
+            for dev in dev_info.keys():
+                if get_net_dev_ip(dev) == ip:
+                    return dev_info[dev]['mac']
+    elif dev:
+        return get_dev_mac(dev)
+    else:
+        #return ':'.join(['{:02x}'.format((uuid.getnode() >> ele) & 0xff) for ele in range(0,8*6,8)][::-1])
+        return str2mac('%012x' % uuid.getnode())
+
+def get_net_dev_ip(ifname):
+    if os.path.isdir('/sys/class/net/{}'.format(ifname)) is False:
+        return False
+    try:
+        s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+        return socket.inet_ntoa(fcntl.ioctl(
+            s.fileno(),
+            0x8915,  # SIOCGIFADDR
+            struct.pack('256s', ifname[:15])
+        )[20:24])
+    except:
+        try:
+            return os.popen('ip addr show {}'.format(ifname)).read().split("inet ")[1].split("/")[0]
+        except:
+            return
+
+def get_net_device(name=None):
+    net_dev={}
+    net_dir='/sys/class/net'
+    if os.path.isdir(net_dir):
+        dirpath,dirnames,filenames = list(os.walk(net_dir))[0]
+        if name:
+            if name in dirnames:
+                drv=ls('{}/{}/device/driver/module/drivers'.format(dirpath,name))
+                if drv is False:
+                    drv='unknown'
+                else:
+                    drv=drv[0].split(':')[1]
+                net_dev[name]={
+                    'mac':cat('{}/{}/address'.format(dirpath,name),no_end_newline=True),
+                    'duplex':cat('{}/{}/duplex'.format(dirpath,name),no_end_newline=True),
+                    'mtu':cat('{}/{}/mtu'.format(dirpath,name),no_end_newline=True),
+                    'state':cat('{}/{}/operstate'.format(dirpath,name),no_end_newline=True),
+                    'speed':cat('{}/{}/speed'.format(dirpath,name),no_end_newline=True),
+                    'id':cat('{}/{}/ifindex'.format(dirpath,name),no_end_newline=True),
+                    'driver':drv,
+                    'drv_ver':cat('{}/{}/device/driver/module/version'.format(dirpath,name),no_end_newline=True),
+                    }
+        else:
+            for dev in dirnames:
+                drv=ls('{}/{}/device/driver/module/drivers'.format(dirpath,dev))
+                if drv is False:
+                    drv='unknown'
+                else:
+                    drv=drv[0].split(':')[1]
+                net_dev[dev]={
+                    'mac':cat('{}/{}/address'.format(dirpath,dev),no_end_newline=True),
+                    'duplex':cat('{}/{}/duplex'.format(dirpath,dev),no_end_newline=True),
+                    'mtu':cat('{}/{}/mtu'.format(dirpath,dev),no_end_newline=True),
+                    'state':cat('{}/{}/operstate'.format(dirpath,dev),no_end_newline=True),
+                    'speed':cat('{}/{}/speed'.format(dirpath,dev),no_end_newline=True),
+                    'id':cat('{}/{}/ifindex'.format(dirpath,dev),no_end_newline=True),
+                    'driver':drv,
+                    'drv_ver':cat('{}/{}/device/driver/module/version'.format(dirpath,dev),no_end_newline=True),
+                    }
+        return net_dev
+    else:
+        return False
+
 def make_tar(filename,filelist,ctype='gz',ignore_file=[]):
     def ignore_files(filename,ignore_files):
         if isinstance(ignore_files,(list,tuple)):
             for ii in ignore_files:
                 if isinstance(ii,str) and (ii == filename or filename.startswith(ii)): return True
         elif isinstance(ignore_files,str):
             if ignore_files == filename or filename.startswith(ignore_files): return True
@@ -2921,29 +466,750 @@
    tmp_dir_arr=tmp_dir.split('/')
    
    for ii in range(0,len(tmp_dir_arr)):
       if filepath_arr[ii] != tmp_dir_arr[ii]:
           return False
    return True
 
+
+def mktemp(filename=None,suffix='-XXXXXXXX',opt='dry',base_dir='/tmp'):
+   if filename is None:
+       filename=os.path.join(base_dir,random_str(length=len(suffix)-1,mode='str'))
+   dir_name=os.path.dirname(filename)
+   file_name=os.path.basename(filename)
+   name, ext = os.path.splitext(file_name)
+   if type(suffix) is not str:
+       suffix='-XXXXXXXX'
+   num_type='.%0{}d'.format(len(suffix)-1)
+   if dir_name == '.':
+       dir_name=os.path.dirname(os.path.realpath(__file__))
+   elif dir_name == '':
+       dir_name=base_dir
+   def new_name(name,ext=None,ext2=None):
+       if ext:
+           if ext2:
+               return '{}{}{}'.format(name,ext,ext2)
+           return '{}{}'.format(name,ext)
+       if ext2:
+           return '{}{}'.format(name,ext2)
+       return name
+   def new_dest(dest_dir,name,ext=None):
+       if os.path.isdir(dest_dir) is False:
+           return False
+       i=0
+       new_file=new_name(name,ext)
+       while True:
+           rfile=os.path.join(dest_dir,new_file)
+           if os.path.exists(rfile) is False:
+               return rfile
+           if suffix:
+               if '0' in suffix or 'n' in suffix or 'N' in suffix:
+                   if suffix[-1] not in ['0','n']:
+                       new_file=new_name(name,num_type%i,ext)
+                   else:
+                       new_file=new_name(name,ext,num_type%i)
+               elif 'x' in suffix or 'X' in suffix:
+                   rnd_str='.{}'.format(random_str(length=len(suffix)-1,mode='str'))
+                   if suffix[-1] not in ['X','x']:
+                       new_file=new_name(name,rnd_str,ext)
+                   else:
+                       new_file=new_name(name,ext,rnd_str)
+               else:
+                   if i == 0:
+                       new_file=new_name(name,ext,'.{}'.format(suffix))
+                   else:
+                       new_file=new_name(name,ext,'.{}.{}'.format(suffix,i))
+           else:
+               new_file=new_name(name,ext,'.{}'.format(i))
+           i+=1
+   new_dest_file=new_dest(dir_name,name,ext)
+   if opt in ['file','f']:
+      os.mknode(new_dest_file)
+   elif opt in ['dir','d','directory']:
+      os.mkdir(new_dest_file)
+   else:
+      return new_dest_file
+
+def isfile(filename=None):
+   if filename is None:
+      return False
+   if len(filename) == 0:
+      return False
+   if os.path.isfile(filename):
+      return True
+   return False
+
+
+#def ping(host,count=3,interval=1,keep_good=0, timeout_sec=5,lost_mon=False,log=None,stop_func=None,log_format='.',cancel_func=None):
+#    ICMP_ECHO_REQUEST = 8 # Seems to be the same on Solaris. From /usr/include/linux/icmp.h;
+#    ICMP_CODE = socket.getprotobyname('icmp')
+#    ERROR_DESCR = {
+#        1: ' - Note that ICMP messages can only be '
+#           'sent from processes running as root.',
+#        10013: ' - Note that ICMP messages can only be sent by'
+#               ' users or processes with administrator rights.'
+#        }
+# 
+#    def checksum(msg):
+#        sum = 0
+#        size = (len(msg) // 2) * 2
+#        for c in range(0,size, 2):
+#            sum = (sum + ord(msg[c + 1])*256+ord(msg[c])) & 0xffffffff
+#        if size < len(msg):
+#            sum = (sum+ord(msg[len(msg) - 1])) & 0xffffffff
+#        ra = ~((sum >> 16) + (sum & 0xffff) + (sum >> 16)) & 0xffff
+#        ra = ra >> 8 | (ra << 8 & 0xff00)
+#        return ra
+# 
+#    def mk_packet(size):
+#        """Make a new echo request packet according to size"""
+#        # Header is type (8), code (8), checksum (16), id (16), sequence (16)
+#        header = struct.pack('bbHHh', ICMP_ECHO_REQUEST, 0, 0, size, 1)
+#        #data = struct.calcsize('bbHHh') * 'Q'
+#        data = size * 'Q'
+#        my_checksum = checksum(_u_bytes2str(header) + data)
+#        header = struct.pack('bbHHh', ICMP_ECHO_REQUEST, 0,
+#                             socket.htons(my_checksum), size, 1)
+#        return header + _u_bytes(data)
+# 
+#    def receive(my_socket, ssize, stime, timeout_sec):
+#        while True:
+#            if timeout_sec <= 0:
+#                return
+#            ready = select.select([my_socket], [], [], timeout_sec)
+#            if ready[0] == []: # Timeout
+#                return
+#            received_time = time.time()
+#            packet, addr = my_socket.recvfrom(1024)
+#            type, code, checksum, gsize, seq = struct.unpack('bbHHh', packet[20:28]) # Get Header
+#            if gsize == ssize:
+#                return received_time - stime
+#            timeout_sec -= received_time - stime
+# 
+#    def pinging(ip,timeout_sec=1,size=64):
+#        try:
+#            my_socket = socket.socket(socket.AF_INET, socket.SOCK_RAW, ICMP_CODE)
+#        except socket.error as e:
+#            if e.errno in ERROR_DESCR:
+#                raise socket.error(''.join((e.args[1], ERROR_DESCR[e.errno])))
+#            raise
+#        if size in ['rnd','random']:
+#            # Maximum size for an unsigned short int c object(65535)
+#            size = int((id(timeout_sec) * random.random()) % 65535)
+#        packet = mk_packet(size)
+#        while packet:
+#            sent = my_socket.sendto(packet, (ip, 1)) # ICMP have no port, So just put dummy port 1
+#            packet = packet[sent:]
+#        delay = receive(my_socket, size, time.time(), timeout_sec)
+#        my_socket.close()
+#        if delay:
+#            return delay,size
+# 
+#    def do_ping(ip,timeout_sec=1,size=64,count=None,interval=0.7,log_format='ping',cancel_func=None,timeout_ping=1):
+#        ok=1
+#        i=1
+#        init_time=None
+#        while True:
+#            out,init_time=timeout(timeout_sec,init_time)
+#            if out:
+#                return -1,'Timeout'
+#            if is_cancel(cancel_func):
+#                return -1,'canceled'
+#            delay=pinging(ip,timeout_ping,size)
+#            if delay:
+#                ok=0
+#                if log_format == '.':
+#                    sys.stdout.write('.')
+#                    sys.stdout.flush()
+#                elif log_format == 'ping':
+#                    sys.stdout.write('{} bytes from {}: icmp_seq={} ttl={} time={} ms\n'.format(delay[1],ip,i,size,round(delay[0]*1000.0,4)))
+#                    sys.stdout.flush()
+#            else:
+#                ok=1
+#                if log_format == '.':
+#                    sys.stdout.write('x')
+#                    sys.stdout.flush()
+#                elif log_format == 'ping':
+#                    sys.stdout.write('{} icmp_seq={} timeout ({} second)\n'.format(ip,i,timeout_sec))
+#                    sys.stdout.flush()
+#            if count:
+#                count-=1
+#                if count < 1:
+#                    return ok,'{} is alive'.format(ip)
+#            i+=1
+#            time.sleep(interval)
+# 
+# 
+#    if log_format=='ping':
+#        if find_executable('ping'):
+#            os.system("ping -c {0} {1}".format(count,host))
+#        else:
+#            do_ping(host,timeout_sec=timeout_sec,size=64,count=count,log_format='ping',cancel_func=cancel_func)
+#    else:
+#        chk_sec=int_sec()
+#        log_type=type(log).__name__
+#        found_lost=False
+#        if keep_good > 0 or not count:
+#           try:
+#               timeout_sec=int(timeout_sec)
+#           except:
+#               timeout_sec=1
+#           if timeout_sec < keep_good:
+#               count=keep_good+(2*interval)
+#               timeout_sec=keep_good+5
+#           elif not count:
+#               count=timeout_sec//interval + 3
+#           elif count * interval > timeout_sec:
+#               timeout_sec=count*interval+timeout_sec
+#        good=False
+#        timeoutini=None
+#        while True:
+#           out,timeoutini=timeout(timeout_sec,init_time=timeoutini)
+#           if out:
+#               return False
+#           if is_cancel(cancel_func):
+#               log(' - Canceled ping')
+#               return False
+#           if stop_func:
+#               if log_type == 'function':
+#                   log(' - Stopped ping')
+#               return False
+#           if find_executable('ping'):
+#               rc=rshell("ping -c 1 {}".format(host))
+#           else:
+#               rc=do_ping(host,timeout_sec=1,size=64,count=count,log_format=None)
+#           if rc[0] == 0:
+#              good=True
+#              if keep_good:
+#                  if good and keep_good and int_sec() - chk_sec >= keep_good:
+#                      return True
+#              else:
+#                  return True
+#              if log_type == 'function':
+#                  log('.',direct=True,log_level=1)
+#           else:
+#              good=False
+#              chk_sec=int_sec()
+#              if log_type == 'function':
+#                  log('x',direct=True,log_level=1)
+#           time.sleep(interval)
+#           count-=1
+#        return good
+
+def get_function_args(func,mode='defaults'):
+    rc={}
+    args, varargs, keywords, defaults = inspect.getargspec(func)
+    if defaults is not None:
+        defaults=dict(zip(args[-len(defaults):], defaults))
+        del args[-len(defaults):]
+        rc['defaults']=defaults
+    if args:
+        rc['args']=args
+    if varargs:
+        rc['varargs']=varargs
+    if keywords:
+        rc['keywards']=keywords
+    if mode in ['*','all']:
+        return rc
+    if mode in rc:
+        return rc[mode]
+
+def get_function_list(objName=None,obj=None):
+    aa={}
+    if obj is None and objName is not None:
+       obj=sys.modules[objName]
+    if obj is not None:
+        for name,fobj in inspect.getmembers(obj):
+            if inspect.isfunction(fobj): # inspect.ismodule(obj) check the obj is module or not
+                aa.update({name:fobj})
+    return aa
+
+def space(space_num=0,_space_='   '):
+    space_str=''
+    for ii in range(space_num):
+        space_str='{0}{1}'.format(space_str,_space_)
+    return space_str
+
+def tap_print(string,bspace='',rc=False,NFLT=False):
+    rc_str=None
+    if type(string) is str:
+        for ii in string.split('\n'):
+            if NFLT:
+               line='%s'%(ii)
+               NFLT=False
+            else:
+               line='%s%s'%(bspace,ii)
+            if rc_str is None:
+               rc_str='%s'%(line)
+            else:
+               rc_str='%s\n%s'%(rc_str,line)
+    else:
+        rc_str='%s%s'%(bspace,string)
+
+    if rc:
+        return rc_str
+    else:
+        print(rc_str)
+
+def str_format_print(string,rc=False):
+    if type(string) is str:
+        if len(string.split("'")) > 1:
+            rc_str='"%s"'%(string)
+        else:
+            rc_str="'%s'"%(string)
+    else:
+        rc_str=string
+    if rc:
+        return rc_str
+    else:
+        print(rc_str)
+
+#def format_print(string,rc=False,num=0,bstr=None,NFLT=False):
+#    string_type=type(string)
+#    rc_str=''
+#    chk=None
+#    bspace=space(num)
+# 
+#    # Start Symbol
+#    if string_type is tuple:
+#        if bstr is None:
+#            if NFLT:
+#                rc_str='%s('%(rc_str)
+#            else:
+#                rc_str='%s%s('%(bspace,rc_str)
+#        else:
+#            rc_str='%s,\n%s%s('%(bstr,bspace,rc_str)
+#    elif string_type is list:
+#        if bstr is None:
+#            if NFLT:
+#                rc_str='%s['%(rc_str)
+#            else:
+#                rc_str='%s%s['%(bspace,rc_str)
+#        else:
+#            rc_str='%s,\n%s%s['%(bstr,bspace,rc_str)
+#    elif string_type is dict:
+#        if bstr is None:
+#            rc_str='%s{'%(rc_str)
+#        else:
+#            rc_str='%s,\n%s %s{'%(bstr,bspace,rc_str)
+#    rc_str='%s\n%s '%(rc_str,bspace)
+# 
+#    # Print string
+#    if string_type is list or string_type is tuple:
+#       for ii in list(string):
+#           ii_type=type(ii)
+#           if ii_type is tuple or ii_type is list or ii_type is dict:
+#               if not ii_type is dict:
+#                  num=num+1
+#               rc_str=format_print(ii,num=num,bstr=rc_str,rc=True)
+#           else:
+#               if chk == None:
+#                  rc_str='%s%s'%(rc_str,tap_print(str_format_print(ii,rc=True),rc=True))
+#                  chk='a'
+#               else:
+#                  rc_str='%s,\n%s'%(rc_str,tap_print(str_format_print(ii,rc=True),bspace=bspace+' ',rc=True))
+#    elif string_type is dict:
+#       for ii in string.keys():
+#           ii_type=type(string[ii])
+#           if ii_type is dict or ii_type is tuple or ii_type is list:
+#               num=num+1
+#               if ii_type is dict:
+#                   tmp=format_print(string[ii],num=num,rc=True)
+#               else:
+#                   tmp=format_print(string[ii],num=num,rc=True,NFLT=True)
+#               rc_str="%s,\n%s %s:%s"%(rc_str,bspace,str_format_print(ii,rc=True),tmp)
+#           else:
+#               if chk == None:
+#                  rc_str='%s%s'%(rc_str,tap_print("{0}:{1}".format(str_format_print(ii,rc=True),str_format_print(string[ii],rc=True)),rc=True))
+#                  chk='a'
+#               else:
+#                  rc_str='%s,\n%s'%(rc_str,tap_print("{0}:{1}".format(str_format_print(ii,rc=True),str_format_print(string[ii],rc=True)),bspace=bspace+' ',rc=True))
+# 
+#    # End symbol
+#    if string_type is tuple:
+#        rc_str='%s\n%s)'%(rc_str,bspace)
+#    elif string_type is list:
+#        rc_str='%s\n%s]'%(rc_str,bspace)
+#    elif string_type is dict:
+#        if bstr is None:
+#            rc_str='%s\n%s}'%(rc_str,bspace)
+#        else:
+#            rc_str='%s\n%s }'%(rc_str,bspace)
+# 
+#    else:
+#       rc_str=string
+# 
+#    # Output
+#    if rc:
+#       return rc_str    
+#    else:
+#       print(rc_str)
+
+
+#def str2url(string):
+#    if string is None: return ''
+#    if type(string) is str:
+#        return string.replace('+','%2B').replace('?','%3F').replace('/','%2F').replace(':','%3A').replace('=','%3D').replace(' ','+')
+#    return string
+
+def clear_version(string,sym='.'):
+    if isinstance(string,(int,str)):
+        if isinstance(string,str): string=string.strip()
+        string='{}'.format(string)
+    else:
+        return False
+    arr=string.split(sym)
+    for ii in range(len(arr)-1,0,-1):
+        if arr[ii].replace('0','') == '':
+            arr.pop(-1)
+        else:
+            break
+    return sym.join(arr)
+
+def get_key(dic=None,find=None):
+    return find_key_from_value(dic=dic,find=find)
+
+def find_key_from_value(dic=None,find=None):
+    if isinstance(dic,dict):
+        if find is None:
+            return list(dic.keys())
+        else:
+            for key,val in dic.items():
+                if val == find:
+                    return key
+    elif isinstance(dic,list) or isinstance(dic,tuple):
+        if find is None:
+            return len(dic)
+        else:
+            if find in dic:
+                return dic.index(find)
+         
+
+def random_str(length=8,strs=None,mode='*'):
+    if strs is None:
+        if mode in ['all','*','alphanumchar']:
+            strs='0aA-1b+2Bc=C3d_D,4.eE?5"fF6g7G!h8H@i9#Ij$JkK%lLmMn^N&oO*p(Pq)Q/r\Rs:St;TuUv{V<wW}x[Xy>Y]z|Z'
+        elif mode in ['alphanum']:
+            strs='aA1b2BcC3dD4eE5fF6g7Gh8Hi9IjJkKlLmMnNoOpPqQrRsStTuUvVwWxXyYzZ'
+        else:
+            strs='aAbBcCdDeEfFgGhHiIjJkKlLmMnNoOpPqQrRsStTuUvVwWxXyYzZ'
+    new=''
+    strn=len(strs)-1
+    for i in range(0,length):
+        new='{0}{1}'.format(new,strs[random.randint(0,strn)])
+    return new
+
+def power_state(ipmi_ip,ipmi_user='ADMIN',ipmi_pass='ADMIN',wait_time=60,check_status=None,monitor_time=3,log_file=None,log=None):
+    sys_status='unknown'
+    if check_status is None:
+        wait_time=3
+    for ii in range(0,wait_time):
+        power_status=ipmi_cmd(cmd='chassis power status',ipmi_ip=ipmi_ip,ipmi_user=ipmi_user,ipmi_pass=ipmi_pass,log=log)
+        if power_status[0] == 0:
+            if power_status[1] == 'Chassis Power is on':
+                sys_status='on'
+            elif power_status[1] == 'Chassis Power is off':
+                sys_status='off'
+            if (check_status and check_status == sys_status) or (check_status is None and sys_status in ['on','off']):
+                if check_status:
+                    logging("   * confirm state : {} => {}".format(sys_status,check_status),log_file=log_file,date=True,log=log,log_level=6)
+                return [True,sys_status]
+            else:
+                if check_status:
+                    logging("   - wait {}sec : {} => {}".format((wait_time - ii)*monitor_time,sys_status,check_status),log_file=log_file,date=True,log=log,log_level=6)
+        else:
+            logging("   - wait {}sec for check power state with {}:{}".format(monitor_time,ipmi_user,ipmi_pass),log_file=log_file,date=True,log=log,log_level=6)
+        sleep(monitor_time)
+    return [False,'time out']
+
+def get_boot_mode(ipmi_ip,ipmi_user,ipmi_pass,log_file=None,log=None):
+    status='No override'
+    rc=ipmi_cmd(cmd='chassis bootparam get 5',ipmi_ip=ipmi_ip,ipmi_user=ipmi_user,ipmi_pass=ipmi_pass,log=log)
+    if rc[0] == 0:
+        efi=False
+        persistent=False
+        for ii in rc[1].split('\n'):
+            if 'Options apply to all future boots' in ii:
+                persistent=True
+            elif 'BIOS EFI boot' in ii:
+                efi=True
+            elif 'Boot Device Selector :' in ii:
+                status=ii.split(':')[1]
+                break
+        if log:
+            log("Boot mode Status:{}, EFI:{}, Persistent:{}".format(status,efi,persistent),log_level=7)
+        return [status,efi,persistent]
+    else:
+        return [False,False,False]
+
+def set_boot_mode(ipmi_ip,ipmi_user,ipmi_pass,boot_mode,ipxe=False,persistent=False,log_file=None,log=None,force=False):
+    boot_mode_d=['pxe','ipxe','bios','hdd']
+    if not boot_mode in boot_mode_d:
+        return
+    if persistent:
+        if boot_mode == 'pxe' and ipxe in ['on','ON','On',True,'True']:
+            # ipmitool -I lanplus -H 172.16.105.74 -U ADMIN -P 'ADMIN' raw 0x00 0x08 0x05 0xe0 0x04 0x00 0x00 0x00
+            ipmi_cmd(cmd='raw 0x00 0x08 0x05 0xe0 0x04 0x00 0x00 0x00',ipmi_ip=ipmi_ip,ipmi_user=ipmi_user,ipmi_pass=ipmi_pass,log=log)
+            logging("Persistently Boot mode set to i{0} at {1}".format(boot_mode,ipmi_ip),log_file=log_file,date=True,log=log,log_level=7)
+        else:
+            ipmi_cmd(cmd='chassis bootdev {0} options=persistent'.format(boot_mode),ipmi_ip=ipmi_ip,ipmi_user=ipmi_user,ipmi_pass=ipmi_pass,log=log)
+            logging("Persistently Boot mode set to {0} at {1}".format(boot_mode,ipmi_ip),log_file=log_file,date=True,log=log,log_level=7)
+    else:
+        if boot_mode == 'pxe' and ipxe in ['on','ON','On',True,'True']:
+                ipmi_cmd(cmd='chassis bootdev {0} options=efiboot'.format(boot_mode),ipmi_ip=ipmi_ip,ipmi_user=ipmi_user,ipmi_pass=ipmi_pass,log=log)
+        else:
+            if force and boot_mode == 'pxe':
+                ipmi_cmd(cmd='chassis bootparam set bootflag force_pxe'.format(boot_mode),ipmi_ip=ipmi_ip,ipmi_user=ipmi_user,ipmi_pass=ipmi_pass,log=log)
+            else:
+                ipmi_cmd(cmd='chassis bootdev {0}'.format(boot_mode),ipmi_ip=ipmi_ip,ipmi_user=ipmi_user,ipmi_pass=ipmi_pass,log=log)
+        logging("Temporary Boot mode set to {0} at {1}".format(boot_mode,ipmi_ip),log_file=log_file,date=True,log=log,log_level=7)
+
+
+def do_power(ipmi_ip,ipmi_user,ipmi_pass,mode,num=2,log_file=None,log=None):
+    power_mode={'on':['chassis power on'],'off':['chassis power off'],'reset':['chassis power reset'],'off_on':['chassis power off','chassis power on'],'cycle':['chassis power cycle']}
+    if not mode in power_mode:
+        return [False,'Unknown power mode']
+    power_step=len(power_mode[mode])-1
+    for ii in range(1,int(num)+1):
+        logging("Power {} at {} (try:{}/{})".format(mode,ipmi_ip,ii,num),log_file=log_file,date=True,log=log,log_level=6)
+        for rr in list(power_mode[mode]):
+            verify_status=rr.split(' ')[-1]
+            if verify_status in ['reset','cycle']:
+                 sys_status=power_state(ipmi_ip,ipmi_user,ipmi_pass,log_file=log_file,log=log)
+                 if sys_status[0] and sys_status[1] == 'off':
+                     logging(" ! can not {} the power at {} status".format(verify_status,sys_status[1]),log_file=log_file,date=True,log=log,log_level=3)
+                     return [False,'can not {} at {} status'.format(verify_status,sys_status[1])]
+            rc=ipmi_cmd(cmd=rr,ipmi_ip=ipmi_ip,ipmi_user=ipmi_user,ipmi_pass=ipmi_pass,log=log)
+            if rc[0] == 0:
+                logging(" + Do power {}".format(verify_status),log_file=log_file,date=True,log=log,log_level=5)
+                if verify_status in ['reset','cycle']:
+                    verify_status='on'
+                    sleep(10)
+            else:
+                logging(" ! power {} fail".format(verify_status),log_file=log_file,date=True,log=log,log_level=3)
+                break
+            sys_status=power_state(ipmi_ip,ipmi_user,ipmi_pass,check_status=verify_status,log_file=log_file,log=log)
+            if sys_status[0]:
+                if sys_status[1] == verify_status:
+                    if power_step == power_mode[mode].index(rr):
+                        return sys_status + [ii]
+                sleep(5)
+            else:
+                break
+        sleep(3)
+    return [False,'time out',ii]
+
+def power_handle(ipmi_ip,mode='status',num=2,ipmi_user='ADMIN',ipmi_pass='ADMIN',boot_mode=None,order=False,ipxe=False,log_file=None,log=None,force=False):
+    # Power handle
+    if mode == 'status':
+        return power_state(ipmi_ip,ipmi_user,ipmi_pass,log_file=log_file,log=log)
+    if boot_mode:
+        if ipxe in ['on','On',True,'True']:
+            ipxe=True
+        else:
+            ipxe=False
+        if boot_mode == 'ipxe':
+            ipxe=True
+            boot_mode='pxe'
+        for ii in range(0,5):
+            aa=set_boot_mode(ipmi_ip,ipmi_user,ipmi_pass,boot_mode,persistent=order,ipxe=ipxe,log_file=log_file,log=log,force=force)
+            boot_mode_state=get_boot_mode(ipmi_ip,ipmi_user,ipmi_pass,log_file=log_file,log=log)
+            if (boot_mode == 'pxe' and boot_mode_state[0] is not False and 'PXE' in boot_mode_state[0]) and ipxe == boot_mode_state[1] and order == boot_mode_state[2]:
+                break
+            logging(" retry boot mode set {} (ipxe:{},force:{})[{}/5]".format(boot_mode,ipxe,order,ii),log_file=log_file,date=True,log=log,log_level=3)
+            time.sleep(2)
+    rc=do_power(ipmi_ip,ipmi_user,ipmi_pass,mode,num=num,log_file=log_file,log=log)
+#    if ipxe in ['on','On',True,'True']:
+#        ipxe=True
+#    if rc[0]:
+#        if boot_mode:
+#            for ii in range(0,5):
+#                set_boot_mode(ipmi_ip,ipmi_user,ipmi_pass,boot_mode,persistent=order,ipxe=ipxe,log_file=log_file,log=log)
+#                boot_mode_state=get_boot_mode(ipmi_ip,ipmi_user,ipmi_pass,log_file=log_file,log=log)
+#                if (boot_mode == 'pxe' and 'PXE' in boot_mode_state[0]) and ipxe == boot_mode_state[1] and order == boot_mode_state[2]:
+#                    break
+#                logging(" retry boot mode set {} (ipxe:{},force:{})[{}/5]".format(boot_mode,ipxe,order,ii),log_file=log_file,date=True,log=log)
+#                time.sleep(2)
+    return rc
+
+def wait_ready_system(ipmi_ip,ipmi_user='ADMIN',ipmi_pass='ADMIN',timeout_sec=1800,keep_up=45,down_monitor=300,interval=3,stop_func=None,stop_arg={},log_file=None,log=None):
+    aa="""ipmitool -I lanplus -H {0} -U {1} -P {2} sdr type Temperature 2>/dev/null""".format(ipmi_ip,ipmi_user,ipmi_pass)
+    chk=0
+    if keep_up >= timeout_sec:
+       timeout_sec=int('{}'.format(keep_up)) + 30
+    if down_monitor >= timeout_sec:
+       timeout_sec=int('{}'.format(down_monitor)) + 30
+    log_type=type(log).__name__
+    init_sec=int(datetime.now().strftime('%s'))
+    do_sec=int('{}'.format(init_sec))
+    wait_count=0
+    count_down=(down_monitor//interval)
+    max_wait=keep_up//interval
+    node_state=None
+    node_old=None
+    node_change=False
+    node_change_count=0
+
+    if count_down > 0:
+        logging("Wait until the system({}) is ready(keep {}sec)".format(ipmi_ip,keep_up),log_file=log_file,date=True,log=log,log_level=6)
+    else:
+        logging("Wait until the system({}) is ready(keep {}sec) after down(check time: {} sec)".format(ipmi_ip,keep_up,down_monitor),log_file=log_file,date=True,log=log,log_level=6)
+    while True:
+        if stop_func and type(stop_arg) is dict:
+            if stop_func(**stop_arg) is True:
+                if log_type=='function':
+                    logging("Got STOP signal",log_file=log_file,date=True,log=log,log_level=3)
+#                    log("Got STOP signal",log_level=6)
+                return [False,'Got STOP signal']
+        if do_sec - init_sec > timeout_sec and node_state == node_old:
+            if log_type=='function':
+                logging("TIme Out, node state is {}".format(node_state),log_file=log_file,date=True,log=log,log_level=3)
+#                log("Time Out, node state is {}".format(node_state),log_level=6)
+            return [False,'Time Out, node state is {}'.format(node_state)]
+        if ping(ipmi_ip,2):
+            tempc=[]
+            wrc=rshell(aa)
+            if wrc[0] == 0:
+                 for ii in wrc[1].split('\n'):
+                      if re.findall('CPU?[0-9]?.Temp',ii) or re.findall('System.Temp',ii):
+                          tempc=re.findall('(\d+) degrees',ii.split('|')[-1])
+                          if tempc:
+                              break
+                 if tempc and int(tempc[0]) > 0:
+                     node_state='up'
+                 else:
+                     node_state='down'
+                 if node_state and node_old and node_state != node_old:
+                     if node_change_count < 4:
+                         init_sec=int(datetime.now().strftime('%s'))
+                     wait_count=0
+                     count_down=(down_monitor//interval)
+                     node_change=True 
+                     node_change_count=node_change_count+1
+                 if (down_monitor == 0 or node_change) and node_state == 'up':
+                     wait_count=wait_count+1
+                     if wait_count > max_wait:
+                         logging("System ready",log_file=log_file,date=True,log=log,log_level=6)
+                         #if log_type=='function':
+                         #    log("The system ready",log_level=6)
+                         return [True,'System ready']
+                 elif down_monitor > 0 and node_change is False and node_state in ['up','down']:
+                     count_down=count_down-1
+                     if count_down < 0:
+                         logging("It did not changed state. still {}".format(node_state),log_file=log_file,date=True,log=log,log_level=3)
+                         #if log_type=='function':
+                         #    log("It did not changed state. still {}".format(node_state),log_level=6)
+                         return [False,'It did not changed state. still {}'.format(node_state)]
+                 if chk % 5 == 0:
+                     if node_state != node_old:
+                         mark='+'
+                     else:
+                         mark='-'
+                     if count_down > 0:
+                         logging(" {2} wait {1}sec for ready system({3}:{4}) at {0}".format(ipmi_ip, (timeout_sec - (do_sec - init_sec)),mark,ipmi_user,ipmi_pass),log_file=log_file,date=True,log=log,log_level=6)
+                     else:
+                         logging(" {2} wait {1}sec for ready system({3}:{4}) at {0} after down".format(ipmi_ip, (timeout_sec - (do_sec - init_sec)),mark,ipmi_user,ipmi_pass),log_file=log_file,date=True,log=log,log_level=6)
+                 node_old='{}'.format(node_state)
+            else:
+                if chk % 5 == 0:
+                    if count_down > 0:
+                        logging("Wait {1}sec for readable sensor data from the system({2}:{3}) at {0}".format(ipmi_ip, (timeout_sec - (do_sec - init_sec)),ipmi_user,ipmi_pass),log_file=log_file,date=True,log=log,log_level=6)
+                    else:
+                        logging("Wait {1}sec for readable sensor data from the system({2}:{3}) at {0} after down".format(ipmi_ip, (timeout_sec - (do_sec - init_sec)),ipmi_user,ipmi_pass),log_file=log_file,date=True,log=log,log_level=6)
+        else:
+            if chk % 5 == 0:
+                logging(" - can't ping to {0}".format(ipmi_ip),log_file=log_file,date=True,log=log,log_level=3)
+        chk=chk+1
+        sleep(interval)
+        do_sec=int(datetime.now().strftime('%s'))
+    if log_type=='function':
+        logging("Unknown status",log_file=log_file,date=True,log=log,log_level=6)
+#        log("Unknown status",log_level=6)
+    return [None,'Unknown status']
+
+#def get_lanmode(smcipmitool_file,smcipmitool_opt):
+#    if smcipmitool_file is not None and smcipmitool_opt is not None:
+#        lanmode_info=rshell('''java -jar {0}/{1} {2}'''.format(tool_path,os.path.basename(smcipmitool_file),smcipmitool_opt))
+#        if lanmode_info[0] == 144:
+#            a=re.compile('Current LAN interface is \[ (\w.*) \]').findall(lanmode_info[1])
+#            if len(a) == 1:
+#                return a[0]
+#    return
+
 def git_ver(git_dir=None):
-    if not IsNone(git_dir) and os.path.isdir('{0}/.git'.format(git_dir)):
+    if git_dir is not None and os.path.isdir('{0}/.git'.format(git_dir)):
         gver=rshell('''cd {0} && git describe --tags'''.format(git_dir))
         if gver[0] == 0:
             return gver[1]
 
 def load_kmod(modules,re_load=False):
     if type(modules) is str:
         modules=modules.split(',')
     for ii in modules:
         if re_load:
             os.system('lsmod | grep {0} >& /dev/null && modprobe -r {0}'.format(ii.replace('-','_')))
         os.system('lsmod | grep {0} >& /dev/null || modprobe --ignore-install {1} || modprobe {1} || modprobe -ib {1}'.format(ii.replace('-','_'),ii))
         #os.system('lsmod | grep {0} >& /dev/null || modprobe -i -f {1}'.format(ii.split('-')[0],ii))
 
+def reduce_string(string,symbol=' ',snum=0,enum=None):
+    if type(string) is str:
+        arr=string.split(symbol)
+    strs=None
+    if enum is None:
+        enum=len(arr)
+    for ii in range(snum,enum):
+        if strs is None:
+            strs='{0}'.format(arr[ii])
+        else:
+            strs='{0} {1}'.format(strs,arr[ii])
+    return strs
+
+def findstr(string,find,prs=None,split_symbol='\n',patern=True):
+    # Patern return selection (^: First(0), $: End(-1), <int>: found item index)
+    found=[]
+    if not isinstance(string,str): return []
+    if split_symbol:
+        string_a=string.split(split_symbol)
+    else:
+        string_a=[string]
+    for nn in string_a:
+        if isinstance(find,(list,tuple)):
+            find=list(find)
+        else:
+            find=[find]
+        for ff in find:
+            if patern:
+                aa=re.compile(ff).findall(nn)
+                for mm in aa:
+                    if isinstance(mm,tuple):
+                        if prs == '^':
+                            found.append(mm[0])
+                        elif prs == '$':
+                            found.append(mm[-1])
+                        elif isinstance(prs,int):
+                            found.append(mm[prs])
+                        else:
+                            found.append(mm)
+                    else:
+                        found.append(mm)
+            else:
+                find_a=ff.split('*')
+                if len(find_a[0]) > 0:
+                    if find_a[0] != nn[:len(find_a[0])]:
+                        chk=False
+                if len(find_a[-1]) > 0:
+                    if find_a[-1] != nn[-len(find_a[-1]):]:
+                        chk=False
+                for ii in find_a[1:-1]:
+                    if ii not in nn:
+                        chk=False
+                if chk:
+                    found.append(nn)
+    return found
+
 def find_cdrom_dev(size=None):
     load_kmod(['sr_mod','cdrom','libata','ata_piix','ata_generic','usb-storage'])
     if os.path.isdir('/sys/block') is False:
         return
     for r, d, f in os.walk('/sys/block'):
         for dd in d:
             for rrr,ddd,fff in os.walk(os.path.join(r,dd)):
@@ -2952,55 +1218,26 @@
                         removable=fp.read()
                     if '1' in removable:
                         if os.path.isfile('{0}/device/model'.format(rrr)):
                             with open('{0}/device/model'.format(rrr),'r') as fpp:
                                 model=fpp.read()
                             for ii in ['CDROM','DVD-ROM','DVD-RW']:
                                 if ii in model:
-                                    if IsNone(size):
+                                    if size is None:
                                         return '/dev/{0}'.format(dd)
                                     else:
                                         if os.path.exists('{}/size'.format(rrr)):
                                             with open('{}/size'.format(rrr),'r') as fss:
                                                 block_size=fss.read()
                                                 dev_size=int(block_size) * 512
                                                 if dev_size == int(size):
                                                     return '/dev/{0}'.format(dd)
 
-def find_usb_dev(size=None,max_size=None):
-    rc=[]
-    load_kmod(modules=['usb-storage'])
-    if os.path.isdir('/sys/block') is False:
-        return
-    for r, d, f in os.walk('/sys/block'):
-        for dd in d:
-            for rrr,ddd,fff in os.walk(os.path.join(r,dd)):
-                if 'removable' in fff:
-                    removable=cat('{0}/removable'.format(rrr),no_edge=True)
-                    if removable:
-                        if IsSame('1',removable):
-                            if IsNone(size):
-                                if max_size:
-                                    file_size=cat('{0}/size'.format(rrr),no_edge=True)
-                                    if file_size:
-                                        dev_size=int(file_size) * 512
-                                        if dev_size <= int(max_size):
-                                            rc.append('/dev/{0}'.format(dd))
-                                else:
-                                    rc.append('/dev/{0}'.format(dd))
-                            else:
-                                file_size=cat('{0}/size'.format(rrr),no_edge=True)
-                                if file_size:
-                                    dev_size=int(file_size) * 512
-                                    if dev_size == int(size):
-                                        rc.append('/dev/{0}'.format(dd))
-    return rc
-
 #def ipmi_sol(ipmi_ip,ipmi_user,ipmi_pass):
-#    if IpV4(ipmi_ip):
+#    if is_ipv4(ipmi_ip):
 #        rshell('''ipmitool -I lanplus -H {} -U {} -P {} sol info'''.format(ipmi_ip,ipmi_user,ipmi_pass))
 #Set in progress                 : set-complete
 #Enabled                         : true
 #Force Encryption                : false
 #Force Authentication            : false
 #Privilege Level                 : OPERATOR
 #Character Accumulate Level (ms) : 0
@@ -3008,139 +1245,195 @@
 #Retry Count                     : 0
 #Retry Interval (ms)             : 0
 #Volatile Bit Rate (kbps)        : 115.2
 #Non-Volatile Bit Rate (kbps)    : 115.2
 #Payload Channel                 : 1 (0x01)
 #Payload Port                    : 623
 
-def net_send_data(sock,data,key='kg',enc=False,timeout=0,close=False):
-    # if close=True then just send data and close socket
-    # if close=False then it need close socket code
-    # ex)
-    #      aa=net_send_data(sock,.....)
-    #      if aa[0] is True: sock.close()
+#def _u_str2int(val,encode='utf-8'):
+#    if is_py3():
+#        if type(val) is bytes:
+#            return int(val.hex(),16)
+#        else:
+#            return int(_u_bytes(val,encode=encode).hex(),16)
+#    return int(val.encode('hex'),16)
+
+#def _u_bytes(val,encode='utf-8'):
+#    def _bytes_(val,encode):
+#        try:
+#            if is_py3():
+#                if type(val) is bytes:
+#                    return val
+#                else:
+#                    return bytes(val,encode)
+#            return bytes(val) # if change to decode then network packet broken
+#        except:
+#            return val
+#    tuple_data=False
+#    if isinstance(val,tuple):
+#        val=list(val)
+#        tuple_data=True
+#    if isinstance(val,list):
+#        for i in range(0,len(val)):
+#            val[i]=_bytes_(val[i],encode)
+#        if tuple_data:
+#            return tuple(val)
+#        else:
+#            return val
+#    else:
+#        return _bytes_(val,encode)
+
+#def _u_bytes2str(val,encode='latin1'):
+#    return _u_byte2str(val,encode=encode)
+
+#def _u_byte2str(val,encode='windows-1252'):
+#def _u_byte2str(val,encode='latin1'):
+#    #return val.decode(encode) # this is original
+#    def _byte2str_(val,encode):
+#        type_val=type(val)
+#        if is_py3() and type_val is bytes:
+#            return val.decode(encode)
+#        elif type_val.__name__ == 'unicode':
+#            return val.encode(encode)
+#        return val
+#    tuple_data=False
+#    if isinstance(val,tuple):
+#        val=list(val)
+#        tuple_data=True
+#    if isinstance(val,list):
+#        for i in range(0,len(val)):
+#            val[i]=_byte2str_(val[i],encode)
+#        if tuple_data:
+#            return tuple(val)
+#        else:
+#            return val
+#    else:
+#        return _byte2str_(val,encode)
+
+def net_send_data(sock,data,key='kg',enc=False,timeout=0):
     if type(sock).__name__ in ['socket','_socketobject','SSLSocket'] and data and type(key) is str and len(key) > 0 and len(key) < 7:
-        start_time=TIME().Int()
+        start_time=now()
         # encode code here
         if timeout > 0:
             sock.settimeout(timeout)
-        nkey=Bytes2Int(key,encode='utf-8',default='org')
+        nkey=_u_str2int(key)
         pdata=pickle.dumps(data,protocol=2) # common 2.x & 3.x version : protocol=2
-        data_type=Bytes(type(data).__name__[0])
+        data_type=_u_bytes(type(data).__name__[0])
         if enc and key:
             # encode code here
-            #enc_tf=Bytes('t') # Now not code here. So, everything to 'f'
+            #enc_tf=_u_bytes('t') # Now not code here. So, everything to 'f'
             #pdata=encode(key,pdata)
-            enc_tf=Bytes('f')
+            enc_tf=_u_bytes('f')
         else:
-            enc_tf=Bytes('f')
+            enc_tf=_u_bytes('f')
         ndata=struct.pack('>IssI',len(pdata),data_type,enc_tf,nkey)+pdata
         try:
             sock.sendall(ndata)
-            if close: sock.close()
             return True,'OK'
         except:
-            if close:
-                if sock: sock.close()
             if timeout > 0:
                 #timeout=sock.gettimeout()
-                if TIME().Int() - start_time > timeout-1:
+                if now() - start_time > timeout-1:
                     #Timeout
                     return False,'Sending Socket Timeout'
     return False,'Sending Fail'
 
-def net_receive_data(sock,key='kg',progress=None,retry=0,retry_timeout=30,progress_msg=None):
+def _dict(pk={},add=False,**var):
+    for key in var.keys():
+        if key in pk:
+            pk.update({key:var[key]})
+        else:
+            if add:
+                pk[key]=var[key]
+            else:
+                return False
+    return pk
+
+def net_receive_data(sock,key='kg',progress=None,retry=0,retry_timeout=30):
     # decode code here
-    def recvall(sock,count,progress=False,progress_msg=None): # Packet
+    def recvall(sock,count,progress=False): # Packet
         buf = b''
         file_size_d=int('{0}'.format(count))
-        #if progress: print('\n')
+        if progress: print('\n')
         tn=0
         newbuf=None
         while count:
             if progress:
-                if progress_msg:
-                    StdOut('\r{} [ {} % ]'.format(progress_msg,int((file_size_d-count) / file_size_d * 100)))
-                else:
-                    StdOut('\rDownloading... [ {} % ]'.format(int((file_size_d-count) / file_size_d * 100)))
+                sys.stdout.write('\rDownloading... [ {} % ]'.format(int((file_size_d-count) / file_size_d * 100)))
+                sys.stdout.flush()
             try:
                 newbuf = sock.recv(count)
             except socket.error as e:
                 if tn < retry:
                     print("[ERROR] timeout value:{} retry: {}/{}\n{}".format(sock.gettimeout(),tn,retry,e))
                     tn+=1
-                    TIME().Sleep(1)
+                    time.sleep(1)
                     sock.settimeout(retry_timeout)
                     continue
                 if e == 'timed out':
                     return 'timeout',e
             if not newbuf: return True,None #maybe something socket issue.
             buf += newbuf
             count -= len(newbuf)
         if progress: 
-            if progress_msg:
-                StdOut('\r{} [ 100 % ]\n'.format(progress_msg))
-            else:
-                StdOut('\rDownloading... [ 100 % ]\n')
+            sys.stdout.write('\rDownloading... [ 100 % ]\n')
+            sys.stdout.flush()
         return True,buf
     ok,head=recvall(sock,10)
     if krc(ok,chk=True):
         if head:
             try:
-                #st_head=struct.unpack('>IssI',Bytes(head))
-                st_head=struct.unpack('>IssI',Bytes(head))
+                st_head=struct.unpack('>IssI',_u_bytes(head))
             except:
                 return [False,'Fail for read header({})'.format(head)]
-            if st_head[3] == Bytes2Int(key,encode='utf-8',default='org'):
-                # File not found Error log size is 57. So if 57 then ignore progress
-                if st_head[0] == 57: progress=False
-                ok,data=recvall(sock,st_head[0],progress=progress,progress_msg=progress_msg)
+            if st_head[3] == _u_str2int(key):
+                ok,data=recvall(sock,st_head[0],progress=progress)
                 if krc(ok,chk=True):
                     if st_head[2] == 't':
                         # decode code here
                         # data=decode(data)
                         pass
                     if data: return [st_head[1],pickle.loads(data)]
                     return [True,None]
                 else:
                     return [ok,data]
             else:
                 return [False,'Wrong key']
         return ['lost','Connection lost']
-    return [ok,head]
+    return ok,head
 
-def net_put_and_get_data(IP,data,PORT=8805,key='kg',timeout=3,try_num=1,try_wait=[0,5],progress=None,enc=False,upacket=None,SSLC=False,log=True,progress_msg=None):
+def net_put_and_get_data(IP,data,PORT=8805,key='kg',timeout=3,try_num=1,try_wait=[0,5],progress=None,enc=False,upacket=None,SSLC=False,log=True):
     sent=False,'Unknown issue'
     for ii in range(0,try_num):
         if upacket: # Update packet function for number of try information ([#/<total #>])
             data=upacket('ntry',[ii+1,try_num],data)
-        start_time=TIME().Int()
+        start_time=now()
         sock=net_get_socket(IP,PORT,timeout=timeout,SSLC=SSLC)
         if try_num > 0: 
             rtry_wait=(timeout//try_num)+1
         else:
             rtry_wait=try_wait
         sent=False,'Unknown issue'
         try:
             sent=net_send_data(sock,data,key=key,enc=enc)
         except:
-            os.system("""[ -f /tmp/.{0}.{1}.crt ] && rm -f /tmp/.{0}.{1}.crt""".format(IP,PORT))
+            os.system("""[ -f /tmp/.{0}.{1}.crt ] && rm -f /tmp/.{0}.{1}.crt""".format(host,port))
         if sent[0]:
-            nrcd=net_receive_data(sock,key=key,progress=progress,progress_msg=progress_msg)
+            nrcd=net_receive_data(sock,key=key,progress=progress)
             return nrcd
         else:
             if timeout >0:
-                if TIME().Int() - start_time >= timeout-1:
+                if now() - start_time >= timeout-1:
                     return [False,'Socket Send Timeout']
                 #return [False,'Data protocol version mismatch']
         if sock: sock.close()
         if try_num > 1:
             if log:
                 print('try send data ... [{}/{}]'.format(ii+1,try_num))
-            TIME().Sleep(try_wait)
+            sleep(try_wait)
     return [False,'Send fail({}) :\n{}'.format(sent[1],data)]
 
 def net_get_socket(host,port,timeout=3,dbg=0,SSLC=False): # host : Host name or IP
     try:
         af, socktype, proto, canonname, sa = socket.getaddrinfo(host, port, socket.AF_UNSPEC, socket.SOCK_STREAM)[0]
     except:
         print('Can not get network informatin of {}:{}'.format(host,port))
@@ -3156,28 +1449,28 @@
     if SSLC:
         for i in range(0,5):
             icertfile='/tmp/.{}.{}.crt'.format(host,port)
             try:
                 cert=ssl.get_server_certificate((host,port))
             except:
                 os.system('rm -f /tmp/.{}.{}.crt'.format(host,port))
-                TIME().Sleep(1)
+                time.sleep(1)
                 continue
             f=open(icertfile,'w')
             f.write(cert)
             f.close()
-            TIME().Sleep(0.3)
+            time.sleep(0.3)
             try:
                 soc=ssl.wrap_socket(soc,ca_certs=icertfile,cert_reqs=ssl.CERT_REQUIRED)
                 soc.connect((host,port))
                 return soc
             except socket.error as msg:
                 if dbg > 3:
                     print(msg)
-                TIME().Sleep(1)
+                time.sleep(1)
     ########################
     else:
         try:
             soc.connect(sa)
             return soc
         except socket.error as msg:
             if dbg > 3:
@@ -3229,47 +1522,195 @@
         ssl_conn=ssl_wrap(conn,certfile,keyfile=keyfile)
         rc=main_func_name(ssl_conn, ip, port, log_file)
     else:
         rc=main_func_name(conn, ip, port, log_file)
     ssoc.close()
     return rc
 
+def sleep(try_wait=None):
+    try_wait_type=type(try_wait)
+    if try_wait in [None,True]:
+        time.sleep(1)
+    elif try_wait_type is list:
+        if len(try_wait) == 2:
+            try:
+                time.sleep(random.randint(int(try_wait[0]),int(try_wait[1])))
+            except:
+                time.sleep(1)
+        else:
+            try:
+                time.sleep(int(try_wait[0]))
+            except:
+                time.sleep(1)
+    elif try_wait_type is str:
+        if try_wait.isdigit():
+            time.sleep(int(try_wait))
+    else:
+        try:
+            time.sleep(try_wait)
+        except:
+            time.sleep(1)
+
+def check_work_dir(work_dir,make=False,ntry=1,try_wait=[1,3]):
+    for ii in range(0,ntry):
+        if os.path.isdir(work_dir):
+            return True
+        else:
+            if make:
+                try:
+                    os.makedirs(work_dir)
+                    return True
+                except:
+                    sleep(try_wait)
+    return False
+
+#def get_file(filename,**opts):
+#    md5sum=opts.get('md5sum',False)
+#    data=opts.get('data',False)
+#    include_dir=opts.get('include_dir',False)
+#    include_sub_dir=opts.get('include_sub_dir',False)
+# 
+#    def get_file_data(filename,root_path=None):
+#        rc={'name':os.path.basename(filename),'path':os.path.dirname(filename),'exist':False,'dir':False,'link':False}
+#        if root_path:
+#            in_filename=os.path.join(root_path,filename)
+#        else:
+#            in_filename=filename
+#        if os.path.exists(in_filename):
+#            fstat=os.stat(in_filename)
+#            rc['uid']=fstat.st_uid
+#            rc['gid']=fstat.st_gid
+#            rc['size']=fstat.st_size
+#            rc['atime']=fstat.st_atime
+#            rc['mtime']=fstat.st_mtime
+#            rc['ctime']=fstat.st_ctime
+#            rc['inod']=fstat.st_ino
+#            rc['mode']=oct(fstat.st_mode)[-4:]
+#            rc['exist']=True
+#            if os.path.islink(in_filename):
+#                rc['link']=True
+#            else:
+#                rc['link']=False
+#                if os.path.isdir(in_filename):
+#                    rc['dir']=True
+#                    rc['path']=in_filename
+#                    rc['name']=''
+#                else:
+#                    rc['dir']=False
+#                    if md5sum or data:
+#                        with open(in_filename,'rb') as f:
+#                            fdata=f.read()
+#                        if md5sum:
+#                            rc['md5']=md5(fdata)
+#                        if data:
+#                            rc['data']=fdata
+#        return rc
+# 
+#    rc={'exist':False,'includes':[]}
+#    if type(filename) is str:
+#        rc.update(get_file_data(filename))
+#        if rc['dir']:
+#            root_path=filename
+#            real_filename=None
+#        else:
+#            root_path=os.path.dirname(filename)
+#            real_filename=os.path.basename(filename)
+#        if include_dir:
+#            pwd=os.getcwd()
+#            os.chdir(root_path)
+#            for dirPath, subDirs, fileList in os.walk('.'):
+#                for sfile in fileList:
+#                    curFile=os.path.join(dirPath.replace('./',''),sfile)
+#                    if curFile != real_filename:
+#                        rc['includes'].append(get_file_data(curFile,root_path))
+#                if include_sub_dir is False:
+#                    break
+#            os.chdir(pwd)
+#    return rc
+        
+#def save_file(data,dest):
+#    if not isinstance(data,dict) or not isinstance(dest,str) : return False
+#    if os.path.isdir(dest) is False: os.system('mkdir -p {0}'.format(dest))
+#    if data.get('dir'):
+#        fmode=file_mode(data.get('mode'))
+#        if fmode:
+#            os.chmod(dest,fmode)
+#    else:
+#        # if file then save
+#        new_file=os.path.join(dest,data['name'])
+#        if 'data' in data:
+#            with open(new_file,'wb') as f:
+#                f.write(data['data'])
+#        chmod_mode=file_mode(data.get('mode'))
+#        if chmod_mode:
+#            os.chmod(new_file,chmod_mode)
+#    if 'includes' in data and data['includes']: # If include directory or files 
+#        for ii in data['includes']:
+#            if ii['path']:
+#                sub_dir=os.path.join(dest,ii['path'])
+#            else:
+#                sub_dir='{}'.format(dest)
+#            if os.path.isdir(sub_dir) is False: os.system('mkdir -p {}'.format(sub_dir))
+#            sub_file=os.path.join(sub_dir,ii['name'])
+#            with open(sub_file,'wb') as f:
+#                f.write(ii['data'])
+#            chmod_mode=file_mode(ii.get('mode'))
+#            if chmod_mode:
+#                os.chmod(sub_file,chmod_mode)
+
+
+def get_node_info():
+    host_ip=get_host_ip()
+    return {
+         'host_name':get_host_name(),
+         'host_ip':host_ip,
+         'host_mac':get_host_mac(ip=host_ip),
+         'ipmi_ip':get_ipmi_ip()[1],
+         'ipmi_mac':get_ipmi_mac()[1],
+         }
+
+def int_sec():
+    return int(datetime.now().strftime('%s'))
+
+def now():
+    return int_sec()
+
 def kmp(mp={},func=None,name=None,timeout=0,quit=False,log_file=None,log_screen=True,log_raw=False, argv=[],queue=None):
     # Clean
     for n in [k for k in mp]:
         if quit is True:
             if n != 'log':
                 mp[n]['mp'].terminate()
                 if 'log' in mp:
                     mp['log']['queue'].put('\nterminate function {}'.format(n))
         else:
-            if mp[n]['timeout'] > 0 and TIME().Int() > mp[n]['timeout']:
+            if mp[n]['timeout'] > 0 and int_sec() > mp[n]['timeout']:
                 mp[n]['mp'].terminate()
                 if 'log' in mp:
                     mp['log']['queue'].put('\ntimeout function {}'.format(n))
         if not mp[n]['mp'].is_alive():
             del mp[n]
     if quit is True and 'log' in mp:
         mp['log']['queue'].put('\nterminate function log')
-        TIME().Sleep(2)
+        time.sleep(2)
         mp['log']['mp'].terminate()
         return
 
     # LOG
     def logging(ql,log_file=None,log_screen=True,raw=False):
         while True:
             #if not ql.empty():
             if ql.empty():
-                TIME().Sleep(0.01)
+                time.sleep(0.01)
             else:
                 ll=ql.get()
                 if raw:
                     log_msg=ll
                 else:
-                    log_msg='{} : {}\n'.format(TIME().Now().strftime('%m-%d-%Y %H:%M:%S'),ll)
+                    log_msg='{} : {}\n'.format(datetime.now().strftime('%m-%d-%Y %H:%M:%S'),ll)
                 if type(log_msg) is not str:
                     log_msg='{}'.format(log_msg)
                 if log_file and os.path.isdir(os.path.dirname(log_file)):
                     with open(log_file,'a') as f:
                         f.write('{}'.format(log_msg))
                 if log_screen:
                     sys.stdout.write(log_msg)
@@ -3277,47 +1718,47 @@
 
     if 'log' not in mp or not mp['log']['mp'].is_alive():
         #log=multiprocessing.Queue()
         log=Queue()
         #lqp=multiprocessing.Process(name='log',target=logging,args=(log,log_file,log_screen,log_raw,))
         lqp=Process(name='log',target=logging,args=(log,log_file,log_screen,log_raw,))
         lqp.daemon = True
-        mp.update({'log':{'mp':lqp,'start':TIME().Int(),'timeout':0,'queue':log}})
+        mp.update({'log':{'mp':lqp,'start':int_sec(),'timeout':0,'queue':log}})
         lqp.start()
 
     # Functions
     if func:
-        if IsNone(name):
+        if name is None:
             name=func.__name__
         if name not in mp:
             if argv:
                 #mf=multiprocessing.Process(name=name,target=func,args=tuple(argv))
                 mf=Process(name=name,target=func,args=tuple(argv))
             else:
                 #mf=multiprocessing.Process(name=name,target=func)
                 mf=Process(name=name,target=func)
             if timeout > 0:
-                timeout=TIME().Int()+timeout
+                timeout=int_sec()+timeout
             
 #            for aa in argv:
 #                if type(aa).__name__ == 'Queue':
 #                    mp.update({name:{'mp':mf,'timeout':timeout,'start':now(),'queue':aa}})
             if name not in mp:
                 if queue and type(queue).__name__ == 'Queue':
-                    mp.update({name:{'mp':mf,'timeout':timeout,'start':TIME().Int(),'queue':queue}})
+                    mp.update({name:{'mp':mf,'timeout':timeout,'start':int_sec(),'queue':queue}})
                 else:
-                    mp.update({name:{'mp':mf,'timeout':timeout,'start':TIME().Int()}})
+                    mp.update({name:{'mp':mf,'timeout':timeout,'start':int_sec()}})
             mf.start()
     return mp
 
 def key_remove_pass(filename):
     rshell('openssl rsa -in {0}.key -out {0}.nopass.key'.format(filename))
 
 def cert_file(keyfile,certfile,C='US',ST='CA',L='San Jose',O='KGC',OU='KG',CN=None,EMAIL=None,days=365,passwd=None,mode='gen'):
-    if IsNone(keyfile) and IsNone(certfile):
+    if keyfile is None and certfile is None:
         return None,None
     if mode == 'remove':
         rc=rshell('openssl rsa -in {0} -out {0}.nopass'.format(keyfile))
         if rc[0] == 0:
             if os.path.isfile('{}'.format(certfile)):
                 return '{}.nopass'.format(keyfile),certfile
             else:
@@ -3351,92 +1792,285 @@
                 # gen KEY
                 rc=rshell('openssl genrsa -aes256 -out {0} 2048'.format(keyfile))
             else:
                 #print('openssl genrsa -out {0} 2048'.format(keyfile))
                 rc=rshell('openssl genrsa -out {0} 2048'.format(keyfile))
         if (os.path.isfile(keyfile) and os.path.isfile(certfile) is False) or rc[0] == 0:
             # gen CSR
+    #        time.sleep(0.1)
             os.system('''rm -f {}'''.format(certfile))
             os.system('''rm -f {}.csr'''.format(keyfile))
             rrc=rshell('openssl req -new -key {0} -out {0}.csr {1}'.format(keyfile,subj))
             if rrc[0] == 0:
                 # gen cert
                 #print('openssl x509 -req -days {1} -in {0}.csr -signkey {0} -out {2}'.format(keyfile,days,certfile))
+#                time.sleep(0.1)
                 rrrc=rshell('openssl x509 -req -days {1} -in {0}.csr -signkey {0} -out {2}'.format(keyfile,days,certfile))
                 if rrrc[0] == 0:
                     # check
 #                    print(rshell('openssl x509 -text -noout -in {}'.format(certfile))[1])
+#                    time.sleep(3)
                     return keyfile,certfile
     else:
         key_file=None
         crt_file=None
         if os.path.isfile(keyfile):
             key_file=keyfile
         if os.path.isfile(certfile):
             crt_file=certfile
         return key_file,crt_file
     return None,None
 
+def rreplace(source_string, replace_what, replace_with):
+    head, _sep, tail = source_string.rpartition(replace_what)
+    return head + replace_with + tail
+
 def net_put_data(IP,data,PORT=8805,key='kg',timeout=3,try_num=1,try_wait=[1,10],progress=None,enc=False,upacket=None,dbg=0,wait_time=3,SSLC=False):
     sent=False,'Unknown issue'
     for ii in range(0,try_num):
         if upacket: # Update packet function for number of try information ([#/<total #>])
             data=upacket('ntry',[ii+1,try_num],data)
         sock=net_get_socket(IP,PORT,timeout=timeout,dbg=dbg,SSLC=SSLC)
         
         if sock is False:
             if dbg >= 3:
                 print('Can not get socket data [{}/{}], wait {}s'.format(ii+1,try_num,wait_time))
             else:
                 sys.stdout.write('.')
                 sys.stdout.flush()
-            TIME().Sleep(wait_time)
+            time.sleep(wait_time)
             continue
         sent=False,'Unknown issue'
         try:
             sent=net_send_data(sock,data,key=key,enc=enc)
         except:
             print('send fail, try again ... [{}/{}]'.format(ii+1,try_num))
         if sent[0]:
             if sock:
                 sock.close()
             return [True,'sent']
         if try_num > 1:
-            wait_time=Random(length=0,strs=try_wait,mode='int')
+            wait_time=make_second(try_wait)
             if dbg >= 3:
                 print('try send data ... [{}/{}], wait {}s'.format(ii+1,try_num,wait_time))
-            TIME().Sleep(wait_time)
+            time.sleep(wait_time)
     return [False,'Send fail({}) :\n{}'.format(sent[1],data)]
 
 
+def make_second(try_wait=None):
+    wait_time=1
+    if try_wait:
+        try_wait_type=type(try_wait)
+        if try_wait_type is list:
+            if len(try_wait) == 1:
+                wait_time=int(try_wait[0])
+            else:
+                wait_time=random.randint(int(try_wait[0]),int(try_wait[-1]))
+        elif try_wait_type is str:
+            if try_wait.isdigit():
+                wait_time=int(try_wait)
+        elif try_wait_type is int:
+            wait_time=try_wait
+    return wait_time
+
+#def web_server_ip(request):
+#    return request.get_host().split(':')
+
+#def web_client_ip(request):
+#    x_forwarded_for = request.META.get('HTTP_X_FORWARDED_FOR')
+#    if x_forwarded_for:
+#        ip = x_forwarded_for.split(',')[0]
+#    else:
+#        ip = request.META.get('REMOTE_ADDR')
+#    return ip
+
+#def web_session(request):
+#    return request.session._get_or_create_session_key()
+
+#def web_req(host_url=None,**opts):
+# 
+#    # remove SSL waring error message (test)
+#    requests.packages.urllib3.disable_warnings() 
+# 
+#    mode=opts.get('mode','get')
+#    max_try=opts.get('max_try',3)
+#    auth=opts.get('auth',None)
+#    user=opts.get('user',None)
+#    ip=opts.get('ip',None)
+#    port=opts.get('port',None)
+#    passwd=opts.get('passwd',None)
+#    timeout_sec=opts.get('timeout',None)
+#    https=opts.get('https',False)
+#    verify=opts.get('verify',True)
+#    request_url=opts.get('request_url',None)
+#    log=opts.get('log',None)
+#    log_level=opts.get('log_level',8)
+#    logfile=opts.get('logfile',None)
+#    if https:
+#        verify=False
+#    if auth is None and user and passwd:
+#        if type(user) is not str or type(passwd) is not str:
+#            printf("user='<user>',passwd='<pass>' : format(each string)",dsp='e',log=log,log_level=log_level,logfile=logfile)
+#            return False,"user='<user>',passwd='<pass>' : format(each string)"
+#        auth=(user,passwd)
+#    if auth and type(auth) is not tuple:
+#        printf("auth=('<user>','<pass>') : format(tuple)",dsp='e',log=log,log_level=log_level,logfile=logfile)
+#        return False,"auth=('<user>','<pass>') : format(tuple)"
+#    data=opts.get('data',None) # dictionary format
+#    if data and type(data) is not dict:
+#        printf("data={'<key>':'<val>',...} : format(dict)",dsp='e',log=log,log_level=log_level,logfile=logfile)
+#        return False,"data={'<key>':'<val>',...} : format(dict)"
+#    json_data=opts.get('json',None) # dictionary format
+#    if json_data and type(json_data) is not dict:
+#        printf("data={'<key>':'<val>',...} : format(dict)",dsp='e',log=log,log_level=log_level,logfile=logfile)
+#        return False,"json={'<key>':'<val>',...} : format(dict)"
+#    files=opts.get('files',None) # dictionary format
+#    if files and type(files) is not dict:
+#        printf("files = { '<file parameter name>': (<filename>, open(<filename>,'rb'))} : format(dict)",dsp='e',log=log,log_level=log_level,logfile=logfile)
+#        return False,"files = { '<file parameter name>': (<filename>, open(<filename>,'rb'))} : format(dict)"
+#    if isinstance(host_url,str):
+#        chk_dest=re.compile('http[s]://([a-zA-Z0-9.]*)[:/]').findall(host_url)
+#        if len(chk_dest): chk_dest=chk_dest[0]
+#        if host_url.find('https://') == 0:
+#            verify=False
+#    elif ip:
+#        chk_dest='{}'.format(ip)
+#        if verify:
+#            host_url='http://{}'.format(ip)
+#        else:
+#            host_url='https://{}'.format(ip)
+#        if port:
+#            host_url='{}:{}'.format(host_url,port)
+#        if request_url:
+#            host_url='{}/{}'.format(host_url,request_url)
+#    else:
+#        return False,'host_url or ip not found'    
+#    if chk_dest:
+#        if not ping(chk_dest,timeout_sec=3):
+#            return False,'Can not access to destination({})'.format(chk_dest)
+#    ss = requests.Session()
+#    for j in range(0,max_try):
+#        if mode == 'post':
+#            try:
+#                r =ss.post(host_url,verify=verify,auth=auth,data=data,files=files,timeout=timeout_sec,json=json_data)
+#                return True,r
+#            except:
+#                pass
+#        else:
+#            try:
+#                r =ss.get(host_url,verify=verify,auth=auth,data=data,files=files,timeout=timeout_sec,json=json_data)
+#                return True,r
+#            except:
+#                pass
+#        #except requests.exceptions.RequestException as e:
+#        host_url_a=host_url.split('/')[2]
+#        server_a=host_url_a.split(':')
+#        if len(server_a) == 1:
+#            printf("Server({}) has no response (wait {}/{} (10s))".format(server_a[0],j,max_try),dsp='e',log=log,log_level=log_level,logfile=logfile)
+#        else:
+#            printf("Server({}:{}) has no response (wait {}/{} (10s))".format(server_a[0],server_a[1],j,max_try),dsp='e',log=log,log_level=log_level,logfile=logfile)
+#        time.sleep(10)
+#    return False,'TimeOut'
+
+def check_value(src,find,idx=None):
+    '''Check key or value in the dict, list or tuple then True, not then False'''
+    if isinstance(src, (list,tuple,str,dict)):
+        if idx is None:
+            for i in src:
+                if IsSame(i,find): return True
+        else:
+            if isinstance(src,str):
+                if idx < 0:
+                    if src[idx-len(find):idx] == find:
+                        return True
+                else:
+                    if src[idx:idx+len(find)] == find:
+                        return True
+            else:
+                if Get(src,idx,out='raw') == find:
+                    return True
+    return False
+
+#def Get(*inps,**opts):
+#    default=opts.get('default',None)
+#    out=opts.get('out',None)
+#    err=opts.get('err',True)
+#    check=opts.get('check',(str,list,tuple,dict))
+#    key=None
+#    if len(inps) >= 2:
+#        src=inps[0]
+#        key=inps[1:]
+#    elif len(inps) == 1:
+#        src=inps[0]
+#        key=opts.get('key',None)
+#        if isinstance(key,list):
+#            key=tuple(key)
+#        elif key is not None:
+#            key=(key,)
+#    rc=[]
+#    if key is None:
+#        if err in [True,'err','True']:
+#            return OutFormat(default,out=out)
+#        return OutFormat(src,out=out)
+#    if isinstance(src,tuple(check)):
+#        if isinstance(src,(str,list,tuple)) and len(src)>0:
+#            for kk in Abs(*key,obj=src,out=list,default=[None],err=False):
+#                if kk is None:
+#                    if err != 'ignore':
+#                        rc.append(default)
+#                else:
+#                    rc.append(src[kk])
+#            if not rc and err in [True,'err','True']:
+#                return OutFormat(default,out=out)
+#            return OutFormat(rc,out=out)
+#        elif isinstance(src,dict) and len(src) > 0:
+#            nkeys=Abs(*key,obj=src,out=list,default=[None],err=False)
+#            if nkeys:
+#                for kk in Abs(*key,obj=src,out=list,default=[None],err=False):
+#                    rr=src.get(kk,default)
+#                    if rr == default:
+#                        if err != 'ignore':
+#                            rc.append(rr)
+#                    else:
+#                        rc.append(rr)
+#                if not rc and err in [True,'err','True']:
+#                    return OutFormat(default,out=out)
+#                return OutFormat(rc,out=out)
+#            return src.get(key[0],default)
+#    elif type(src).__name__ in ['instance','classobj']:
+#        if isinstance(key,(list,tuple,dict)):
+#            for kk in key:
+#                rc.append(getattr(src,kk,default))
+#            if not rc and err in [True,'err','True']:
+#                return OutFormat(default,out=out)
+#            return OutFormat(rc,out=out)
+#        return getattr(src,key,default)
+#    if err in [True,'err','True']:
+#        return OutFormat(default,out=out)
+#    return OutFormat(src,out=out)
+
+
+def get_value(src,key=None,default=None,check=[str,list,tuple,dict]):
+    return Get(src,key,default=default,check=check)
+
 def encode(string):
     enc='{0}'.format(string)
     tmp=zlib.compress(enc.encode("utf-8"))
     return '{0}'.format(base64.b64encode(tmp).decode('utf-8'))
 
 def decode(string):
     if type(string) is str:
         dd=zlib.decompress(base64.b64decode(string))
         return '{0}'.format(dd.decode("utf-8"))
     return string
 
-def get_node_info(loop=0):
-    host_ip=get_host_ip()
-    return {
-         'host_name':get_host_name(),
-         'host_ip':host_ip,
-         'host_mac':get_host_mac(ip=host_ip),
-         'ipmi_mac':get_ipmi_mac(loop=loop)[1],
-         'ipmi_ip':get_ipmi_ip()[1],
-         }
-
 def mount_samba(url,user,passwd,mount_point):
     if os.path.isdir(mount_point) is False:
         os.system('sudo mkdir -p {0}'.format(mount_point))
-        TIME().Sleep(1)
+        time.sleep(1)
     if os.path.isdir(mount_point) is False:
         return False,'can not make a {} directory'.format(mount_point),'can not make a {} directory'.format(mount_point),0,0,None,None
     if 'smb://' in url:
         url_a=url.split('/')
         url_m=len(url_a)
         iso_file=url_a[-1]
         new_url=''
@@ -3459,39 +2093,296 @@
 def umount(mount_point,del_dir=False):
     rc=rshell('''[ -d {0} ] && sudo mountpoint {0} && sleep 1 && sudo umount {0} && sleep 1'''.format(mount_point))
     if rc[0] == 0 and del_dir:
         os.system('[ -d {0} ] && sudo rmdir {0}'.format(mount_point))
     return rc
 
 def is_xml(filename):
-    firstLine_i=FILE().Rw(filename,out='string',read='firstline')
+    firstLine_i=file_rw(filename,out='string',read='firstline')
     if krc(firstLine_i,chk=True):
-        firstLine=Get(firstLine_i,1)
+        firstLine=get_value(firstLine_i,1)
     else:
         filename_str=_u_byte2str(filename)
         if isinstance(filename_str,str):
             firstLine=filename_str.split('\n')[0]
     if isinstance(firstLine,str) and firstLine.split(' ')[0] == '<?xml':
         return True
     return False
 
+def krc(rt,chk='_',rtd={'GOOD':[True,'True','Good','Ok','Pass',{'OK'},0],'FAIL':[False,'False','Fail',{'FAL'}],'NONE':[None,'None','N/A',{'NA'}],'IGNO':['IGNO','Ignore',{'IGN'}],'ERRO':['ERR','Error','error','erro','ERRO',{'ERR'}],'WARN':['Warn','warn',{'WAR'}],'UNKN':['Unknown','UNKN',{'UNK'}],'JUMP':['Jump',{'JUMP'}],'TOUT':['timeout','TimeOut','time out','Time Out','TMOUT','TOUT',{'TOUT'}],'REVD':['cancel','Cancel','CANCEL','REV','REVD','Revoked','revoked','revoke','Revoke',{'REVD'}],'LOST':['lost','connection lost','Connection Lost','Connection lost','CONNECTION LOST',{'LOST'}]},default=False):
+    def trans(irt):
+        type_irt=type(irt)
+        for ii in rtd:
+            for jj in rtd[ii]:
+                if type(jj) == type_irt and ((type_irt is str and jj.lower() == irt.lower()) or jj == irt):
+                    return ii
+        return 'UNKN'
+    rtc=Get(rt,'0|rc',out='raw',err='ignore',check=(list,tuple,dict))
+    nrtc=trans(rtc)
+    if chk != '_':
+        if not isinstance(chk,list): chk=[chk]
+        for cc in chk:
+            if trans(cc) == nrtc:
+                return True
+            if nrtc == 'UNKN' and default == 'org':
+                return rtc
+        if default == 'org': return rt
+        return default
+    return nrtc
+
+def replacestr(data,org,new):
+    if isinstance(data,str):
+        if not isinstance(org,str): org=_u_bytes2str(org)
+        if not isinstance(new,str): new=_u_bytes2str(new)
+    elif isinstance(data,bytes):
+        if not isinstance(org,bytes): org=_u_bytes(org)
+        if not isinstance(new,bytes): new=_u_bytes(new)
+#    if not isinstance(data,bytes):
+#        data=_u_bytes(data)
+#    if not isinstance(org,bytes):
+#        org=_u_bytes(org)
+#    if not isinstance(new,bytes):
+#        new=_u_bytes(new)
+    return data.replace(org,new)
+
+def check_version(a,sym,b):
+    a=clear_version(a)
+    b=clear_version(b)
+    if a is False or b is False:
+        return False
+    if sym == '>':
+        if LooseVersion(a) > LooseVersion(b):
+            return True
+    elif sym == '>=':
+        if LooseVersion(a) >= LooseVersion(b):
+            return True
+    elif sym == '==':
+        if LooseVersion(a) == LooseVersion(b):
+            return True
+    elif sym == '<=':
+        if LooseVersion(a) <= LooseVersion(b):
+            return True
+    elif sym == '<':
+        if LooseVersion(a) < LooseVersion(b):
+            return True
+    return False
+    
 def get_iso_uid(filename):
     if type(filename) is not str:
         return False,None,None
     if os.path.exists(filename):
         uid_cmd='''sudo /usr/sbin/blkid {}'''.format(filename)
         rc=rshell(uid_cmd)
         if rc[0] == 0:
-            uid_str='{0}_{1}'.format(FIND(rc[1]).Find('UUID="(\w.*)" L'),FIND(rc[1]).Find('LABEL="(\w.*)" T')).replace(' ','_')
+            uid_str='{0}_{1}'.format(findstr(rc[1],'UUID="(\w.*)" L')[0],findstr(rc[1],'LABEL="(\w.*)" T')[0]).replace(' ','_')
             file_info=get_file(filename)
             file_size=file_info.get('size',None)
             return True,uid_str,file_size
         return False,rc[1],None
     return False,'{} not found'.format(filename),None
 
+def find_usb_dev(size=None,max_size=None):
+    rc=[]
+    load_kmod(modules=['usb-storage'])
+    if os.path.isdir('/sys/block') is False:
+        return
+    for r, d, f in os.walk('/sys/block'):
+        for dd in d:
+            for rrr,ddd,fff in os.walk(os.path.join(r,dd)):
+                if 'removable' in fff:
+                    removable=cat('{0}/removable'.format(rrr))
+                    if removable:
+                        if '1' in removable:
+                            if size is None:
+                                if max_size:
+                                    file_size=cat('{0}/size'.format(rrr))
+                                    if file_size:
+                                        dev_size=int(file_size) * 512
+                                        if dev_size <= int(max_size):
+                                            rc.append('/dev/{0}'.format(dd))
+                                else:
+                                    rc.append('/dev/{0}'.format(dd))
+                            else:
+                                file_size=cat('{0}/size'.format(rrr))
+                                if file_size:
+                                    dev_size=int(file_size) * 512
+                                    if dev_size == int(size):
+                                        rc.append('/dev/{0}'.format(dd))
+    return rc
+
+def get_my_directory():
+    return os.path.dirname(os.path.realpath(__file__))
+
+def is_json_format(data):
+    try:
+        json.loads(data)
+        return True
+    except:
+        return False
+
+def Abs(*inps,**opts):
+    default=opts.get('default',None)
+    out=opts.get('out','auto')
+    obj=opts.get('obj',None)
+    err=opts.get('err',True)
+ 
+    def int_idx(idx,nobj,default,err,out='auto'):
+        if idx < 0:
+            if abs(idx) <= nobj:
+                if out in ['list',list]:
+                    return [nobj+idx]
+                elif out in ['tuple',tuple]:
+                    return (nobj+idx,)
+                return nobj+idx
+            elif err not in [True,'err','True']:
+                return 0
+        else:
+            if nobj > idx:
+                if out in ['list',list]:
+                    return [idx]
+                elif out in ['tuple',tuple]:
+                    return (idx,)
+                return idx
+            elif err not in [True,'err','True']:
+                return nobj-1
+        return default
+    if len(inps) > 0:
+        ss=None
+        ee=None
+        rt=[]
+        if obj is None:
+            for i in inps:
+                if isinstance(i,int):
+                    rt.append(abs(i))
+                elif err in [True,'err','True']:
+                    rt.append(default)
+        elif isinstance(obj,dict):
+            keys=list(obj)
+            for idx in inps:
+                if isinstance(idx,int):
+                    rt.append(keys[int_idx(idx,len(keys),default,err)])
+                elif isinstance(idx,tuple) and len(idx) == 2:
+                    ss=Abs(idx[0],**opts)
+                    ee=Abs(idx[1],**opts)
+                    for i in range(ss,ee+1):
+                        rt.append(keys[i])
+                elif isinstance(idx,str):
+                    try:
+                        idx=int(idx)
+                        rt.append(int_idx(idx,len(keys),default,err))
+                    except:
+                        if len(idx.split(':')) == 2:
+                            ss,ee=tuple(idx.split(':'))
+                            if isinstance(ss,int) and isinstance(ee,int):
+                                for i in range(ss,ee+1):
+                                    rt.append(keys[i])
+                        elif len(idx.split('-')) == 2:
+                            ss,ee=tuple(idx.split('-'))
+                            if isinstance(ss,int) and isinstance(ee,int):
+                                for i in range(ss,ee+1):
+                                    rt.append(keys[i])
+                        elif len(idx.split('|')) > 1:
+                            rt=rt+idx.split('|')
+        elif isinstance(obj,(list,tuple,str)):
+            nobj=len(obj)
+            for idx in inps:
+                if isinstance(idx,list):
+                    for ii in idx:
+                        if isinstance(ii,int):
+                            if nobj > ii:
+                                rt.append(ii)
+                            else:
+                                rt.append(OutFormat(default))
+                elif isinstance(idx,int):
+                    rt.append(int_idx(idx,nobj,default,err))
+                elif isinstance(idx,tuple) and len(idx) == 2:
+                    ss=Abs(idx[0],**opts)
+                    ee=Abs(idx[1],**opts)
+                    rt=rt+list(range(ss,ee+1))
+                elif isinstance(idx,str):
+                    try:
+                        idx=int(idx)
+                        rt.append(int_idx(idx,nobj,default,err))
+                    except:
+                        if len(idx.split(':')) == 2:
+                            ss,ee=tuple(idx.split(':'))
+                            ss=Abs(ss,**opts)
+                            ee=Abs(ee,**opts)
+                            if isinstance(ss,int) and isinstance(ee,int):
+                                rt=rt+list(range(ss,ee+1))
+                        elif len(idx.split('-')) == 2:
+                            ss,ee=tuple(idx.split('-'))
+                            ss=Abs(ss,**opts)
+                            ee=Abs(ee,**opts)
+                            if isinstance(ss,int) and isinstance(ee,int):
+                                rt=rt+list(range(ss,ee+1))
+                        elif len(idx.split('|')) > 1:
+                            for i in idx.split('|'):
+                                ss=Abs(i,obj=obj,out='raw')
+                                if isinstance(ss,int):
+                                    rt.append(ss)
+                        else:
+                            rt.append(OutFormat(default))
+        return OutFormat(rt,out=out)
+    elif obj:
+        if isinstance(obj,(list,tuple,str)):
+            return len(obj)
+        elif isinstance(obj,dict):
+            return list(obj.keys())
+    return default
+
+def Delete(*inps,**opts):
+    if len(inps) >= 2:
+        obj=inps[0]
+        keys=inps[1:]
+    elif len(inps) == 1:
+        obj=inps[0]
+        keys=opts.get('key',None)
+        if isinstance(keys,list):
+            keys=tuple(keys)
+        elif keys is not None:
+            keys=(keys,)
+    default=opts.get('default',None)
+    _type=opts.get('type','index')
+   
+    if isinstance(obj,(list,tuple)):
+        nobj=len(obj)
+        rt=[]
+        if _type == 'index':
+            nkeys=Abs(*tuple(keys),obj=obj,out=list)
+            for i in range(0,len(obj)):
+                if i not in nkeys:
+                    rt.append(obj[i])
+        else:
+            for i in obj:
+                if i not in keys:
+                    rt.append(i)
+        return rt
+    elif isinstance(obj,dict):
+        if isinstance(keys,(list,tuple,dict)):
+            for key in keys:
+                obj.pop(key,default)
+        else:
+            obj.pop(keys,default)
+        return obj
+    elif isinstance(obj,str):
+        nkeys=[]
+        for i in keys:
+            if isinstance(i,(tuple,str,int)):
+                tt=Abs(i,obj=obj,out=list)
+                if tt:
+                    nkeys=nkeys+tt
+        rt=''
+        for i in range(0,len(obj)):
+            if i in nkeys:
+                continue
+            rt=rt+obj[i]
+        return rt
+    return default
+
 def alive(out=None):
     aa=rshell('uptime')
     if aa[0] == 0:
         aa_a=aa[1].split()
         if len(aa_a) > 2: 
             if ':' in aa_a[2]:
                 if out in ['sec','second','seconds',int]:
@@ -3517,438 +2408,211 @@
                 else:
                     return aa_a[2]+'d'
     if out in ['sec','second','seconds',int]:
         return -1
     else:
         return 'unknown'
 
+
+class Multiprocessor():
+    def __init__(self):
+        self.processes = []
+        self.queue = Queue()
+
+    @staticmethod
+    def _wrapper(func, queue, args, kwargs):
+        ret = func(*args, **kwargs)
+        queue.put(ret)
+
+    def run(self, func, *args, **kwargs):
+        args2 = [func, self.queue, args, kwargs]
+        p = Process(target=self._wrapper, args=args2)
+        self.processes.append(p)
+        p.start()
+
+    def wait(self):
+        rets = []
+        for p in self.processes[:]:
+            ret = self.queue.get()
+            rets.append(ret)
+            self.processes.remove(p)
+        return rets
+
+def IsSame(src,chk_val,sense=False):
+    def _IsSame_(src,chk,sense):
+        src_type=type(src).__name__
+        chk_type=type(chk).__name__
+        if src_type == 'bytes' or chk_type == 'bytes':
+            if chk_type=='int': chk='{}'.format(chk)
+            if isinstance(chk,str):
+                if sense:
+                    chk=_u_bytes(chk)
+                else:
+                    chk=_u_bytes(chk).lower()
+            elif not sense:
+                chk=chk.lower()
+            if src_type=='int': src='{}'.format(src)
+            if isinstance(src,str):
+                if sense:
+                    src=_u_bytes(src)
+                else:
+                    src=_u_bytes(src).lower()
+            elif not sense:
+                src=src.lower()
+            if src == chk: return True
+        else:
+            if src_type == 'str' and src.isdigit(): src=int(src)
+            if chk_type == 'str' and chk.isdigit(): chk=int(chk)
+            if not sense and isinstance(src,str) and isinstance(chk,str):
+                if src.lower() == chk.lower(): return True
+            elif src == chk:
+                return True
+        return False
+    if isinstance(src,(list,tuple)) and isinstance(chk_val,(list,tuple)):
+        for j in src:
+            ok=False
+            for i in chk_val:
+                aa=_IsSame_(j,i,sense)
+                if aa is True:
+                    ok=True
+                    break
+            if ok is False: return False
+        for j in chk_val:
+            ok=False
+            for i in src:
+                aa=_IsSame_(j,i,sense)
+                if aa is True:
+                    ok=True
+                    break
+            if ok is False: return False
+        return True
+    else:
+        if isinstance(chk_val,(list,tuple)):
+            for i in chk_val:
+                aa=_IsSame_(src,i,sense)
+                if aa is True: return True
+            return False
+        else:
+            return _IsSame_(src,chk_val,sense)
+
+def ddict(*inps,**opts):
+    out={}
+    for ii in inps:
+        if isinstance(ii,dict):
+            out.update(ii)
+    if opts:
+        out.update(opts)
+    return out
+
+def fdict(src,keys):
+    if isinstance(src,dict) and isinstance(keys,list):
+        new_out={}
+        for kk in keys:
+            new_out[kk]=src.get(kk)
+        return new_out
+
+def is_function(find,src=None):
+    if src is None: 
+        if isinstance(find,str):
+            find=sys.modules.get(find)
+        return inspect.isfunction(find)
+    aa=[]
+    if not isinstance(find,str): find=find.__name__
+    if isinstance(src,str):
+        src=sys.modules.get(src)
+    if inspect.ismodule(src) or inspect.isclass(src):
+        for name,fobj in inspect.getmembers(src):
+            if inspect.isfunction(fobj): # inspect.ismodule(obj) check the obj is module or not
+                aa.append(name)
+    else:
+        for name,fobj in inspect.getmembers(src):
+            if inspect.ismethod(fobj): # inspect.ismodule(obj) check the obj is module or not
+                aa.append(name)
+    if find in aa: return True
+    return False
+
 def pipe_msg(**opts):
     m={}
     if not pipe_file: return False
     if os.path.isfile(pipe_file):
         with open(pipe_file,'rb') as f:
-            buf=f.read()
-        try:
-            m=pickle.loads(buf)
-        except:
-            pass
+            m=pickle.load(f)
     if opts:
         m.update(opts)
         with open(pipe_file,'wb') as f:
             pickle.dump(m,f, protocol=pickle.HIGHEST_PROTOCOL)
     else:
         return m
 
+def is_same(a,b,sense=False):
+    return IsSame(a,b,sense=sense)
+#    if isinstance(a,(list,tuple)) and len(a) == 1:
+#        a=a[0]
+#    if isinstance(b,(list,tuple)) and len(b) == 1:
+#        b=b[0]
+#    if isinstance(a,str) and a.isdigit():
+#        a=int(a)
+#    if isinstance(b,str) and b.isdigit():
+#        b=int(b)
+#    if sense is False and isinstance(a,str) and isinstance(b,str):
+#        if a.lower() == b.lower(): return True
+#    elif a == b: 
+#        return True
+#    return False
+    
 def Try(cmd):
     try:
         return True,cmd
     except:
         e=sys.exc_info()[0]
         return False,{'err':e}
 
-#################################################################
-def gen_random_string(length=8,letter='*',digits=True,symbols=True,custom=''):
-    mode='alpha'
-    if digits:mode=mode+'num'
-    if symbols:mode=mode+'char'
-    return Random(length=length,strs=custom,mode=mode,letter=letter)
-
-def TypeData(src,default='org',want_type=None,spliter=None):
-    '''Convert (input)data to want type (ex: str -> list, int, ...), can not convert to type then return False'''
-    if want_type is str and spliter and isinstance(src,(list,tuple)):
-        return spliter.join(src)
-    elif want_type is str and not isinstance(src,str):
-        return '''{}'''.format(src)
-    elif want_type is int and not isinstance(src,int):
-        try:
-            return int(src)
-        except:
-            if default in ['org',{'org'}]: return src
-            return default
-    elif want_type in [list,tuple] and isinstance(src,str) and isinstance(spliter,str):
-        if want_type is tuple:
-            return tuple(src.split(spliter))
-        return src.split(spliter)
-    elif want_type is tuple and isinstance(src,(list,dict)):
-        if isinstance(src,dict):
-            if spliter == 'key':
-                return tuple(src.keys())
-            elif spliter == 'value':
-                return tuple(src.values())
-            else:
-                return tuple(src.items())
-        return tuple(src)
-    elif want_type is list and isinstance(src,(tuple,dict)):
-        if isinstance(src,dict):
-            if spliter == 'key':
-                return list(src.keys())
-            elif spliter == 'value':
-                return list(src.values())
-            else:
-                return list(src.items())
-        return list(src)
-    elif want_type:
-        if isinstance(src,want_type):
-            return src
-    if isinstance(src,str):
-        try:
-            return ast.literal_eval(src)
-        except:
-            try:
-                return json.loads(src)
-            except:
-                pass
-    if default in ['org',{'org'}]: return src
-    return default
-
-def sizeConvert(sz=None,unit='b:g'):
-    try:
-        sz=int(sz)
-    except:
-        return default
-    unit_a=unit.lower().split(':')
-    if len(unit_a) != 2:
-        return False
-    def inc(sz):
-        return '%.1f'%(float(sz) / 1024)
-    def dec(sz):
-        return int(sz) * 1024
-    sunit=unit_a[0]
-    eunit=unit_a[1]
-    unit_m=['b','k','m','g','t','p']
-    si=unit_m.index(sunit)
-    ei=unit_m.index(eunit)
-    h=ei-si
-    for i in range(0,abs(h)):
-        if h > 0:
-            sz=inc(sz)
-        else:
-            sz=dec(sz)
-    return sz
-
-############################################
-#Temporary function
-############################################
-def compare(a,sym,b,ignore=None):
-    if type(a) is not int or type(b) is not int:
-        return False
-    if not IsNone(ignore):
-        if eval('{} == {}'.format(a,ignore)) or eval('{} == {}'.format(b,ignore)):
-            return False
-    return eval('{} {} {}'.format(a,sym,b))
-
-def dput(dic=None,keys=None,val=None,force=False,safe=True):
-    if not IsNone(dic) and keys:
-        tmp=dic
-        keys_arr=keys.split('/')
-        keys_num=len(keys_arr)
-        for ii in keys_arr[:(keys_num-1)]:
-            if ii in tmp:
-                if type(tmp[ii]) == type({}):
-                    dtmp=tmp[ii]
-                else:
-                    if IsNone(tmp[ii]):
-                        tmp[ii]={}
-                        dtmp=tmp[ii]
-                    else:
-                        if force:
-                            vtmp=tmp[ii]
-                            tmp[ii]={vtmp:None}
-                            dtmp=tmp[ii]
-                        else:
-                            return False
-            else:
-                if force:
-                    tmp[ii]={}
-                    dtmp=tmp[ii]
-                else:
-                    return False
-            tmp=dtmp
-        if val == '_blank_':
-            val={}
-        if keys_arr[keys_num-1] in tmp.keys():
-            if safe:
-                if tmp[keys_arr[keys_num-1]]:
-                    return False
-            tmp.update({keys_arr[keys_num-1]:val})
-            return True
-        else:
-            if force:
-                tmp.update({keys_arr[keys_num-1]:val})
-                return True
-    return False
-
-def dget(dict=None,keys=None):
-    if IsNone(dict) or IsNone(keys):
-        return False
-    tmp=dict.copy()
-    keys_path=keys.split('/')
-    if keys_path[0] == '': keys_path=keys_path[1:]
-    for ii in keys.split('/'):
-        if ii in tmp:
-           dtmp=tmp[ii]
-        else:
-           return False
-        tmp=dtmp
-    return tmp
-
-def isfile(filename=None):
-   if Type(filename,'str',data=True) and os.path.isfile(filename):
-      return True
-   return False
 
-def str_format_print(string,rc=False):
-    if type(string) is str:
-        if len(string.split("'")) > 1:
-            rc_str='"%s"'%(string)
-        else:
-            rc_str="'%s'"%(string)
-    else:
-        rc_str=string
-    if rc:
-        return rc_str
-    else:
-        print(rc_str)
-
-def reduce_string(string,symbol=' ',snum=0,enum=None):
-    string_a=Cut(string,symbol=symbol,out=list)
-    sidx=FixIndex(string_a,snum)
-    eidx=FixIndex(string_a,enum if isinstance(enum,int) else len(string_a))
-    return Join(string_a[sidx:edix],' ')
-
-def sreplace(pattern,sub,string):
-    return re.sub('^%s' % pattern, sub, string)
-
-def ereplace(pattern,sub,string):
-    return re.sub('%s$' % pattern, sub, string)
+def list_index(src,step):
+    if isinstance(src,(list,tuple,str,dict)) and isinstance(step,int):
+        if step < 0:
+            if len(src) > abs(step):
+                step=len(src)-abs(step)
+            else:
+                step=0
+        else:
+            if len(src) <= step: step=len(src)-1
+        return step
+    return 0
+
+def Next(src,step=0,out=None,default='org'):
+    if isinstance(src,(list,tuple,dict)):
+        step=list_index(src,step)
+        iterator=iter(src)
+        for i in range(-1,step):
+            rt=next(iterator)
+        return OutFormat(rt,out=out)
+    elif isinstance(src,str):
+        step=list_index(src,step)
+        if len(src) == 0:
+            return ''
+        elif len(src) >= 0 or len(src) <= step:
+            return OutFormat(src[step],out=out)
 
-def rreplace(source_string, replace_what, replace_with):
-    head, _sep, tail = source_string.rpartition(replace_what)
-    return head + replace_with + tail
+    if default == 'org': return src
+    OutFormat(default,out=out)
 
-def argtype(arg,want='_',get_data=['_']):
-    type_arg=type(arg)
-    if want in get_data:
-        if type_arg.__name__ == 'Request':
-            return arg.method.lower()
-        return type_arg.__name__.lower()
-    if Type(want,str):
-        if type_arg.__name__ == 'Request':
-            if want.upper() == 'REQUEST' or want.upper() == arg.method:
-                return True
-            return False
-        else:
-            if type_arg.__name__.lower() == want.lower():
-                return True
+def code_error(email_func=None,email=None,email_title=None,email_server=None,log=None,log_msg='',default=None):
+    e=sys.exc_info()[0]
+    er=traceback.format_exc()
+    if log_msg:
+        log_msg='{}\n\n*SYS ERR:\n{}\n\n*FORM ERR:\n{}'.format(log_msg,e,er)
     else:
-        if type_arg == want:
-            return True
-    return False
-
-def Lower(src,default='org'):
-    if isinstance(src,str): return src.lower()
-    if default in ['org',{'org'}]: return src
+        log_msg='*SYS ERR:\n{}\n\n*FORM ERR:\n{}'.format(e,er)
+    if log: log('\n!!ERROR!!: {}'.format(log_msg),log_level=1)
+    if email_func and email and email_title:
+        a=email_func(email,email_title,log_msg,dj_ip=email_server)
+    time.sleep(5)
     return default
 
-def Upper(src,default='org'):
-    if isinstance(src,str): return src.upper()
-    if default in ['org',{'org'}]: return src
-    return default
-############################################
-#Temporary function map for replacement
-############################################
-def sendanmail(to,subj,msg,html=True):
-    Email=EMAIL()
-    return Email.Send(to,sender='root@sumtester.supermicro.com',title=subj,msg=msg,html=html)
-
-def mktemp(filename=None,suffix='-XXXXXXXX',opt='dry',base_dir='/tmp',force=False):
-    return FILE().MkTemp(filename=filename,suffix=suffix,opt=opt,base_dir=base_dir,force=force)
-
-def get_host_name():
-    return HOST().Name()
-
-def get_host_ip(ifname=None,mac=None):
-    return HOST().Ip(ifname,mac)
-
-def get_default_route_dev():
-    return HOST().DefaultRouteDev()
-
-def get_dev_name_from_mac(mac=None):
-    return HOST().DevName(mac)
-
-def get_dev_mac(ifname):
-    return HOST().Mac(dev=ifname)
-
-def get_host_iface():
-    return HOST().DefaultRouteDev()
-
-def get_host_mac(ip=None,dev=None):
-    return HOST().Mac(ip=ip,dev=dev)
-
-def get_net_dev_ip(ifname):
-    return HOST().Ip(ifname=ifname)
-
-def get_net_device(name=None):
-    return HOST().NetDevice(name)
-
-def get_my_directory(cwd=None):
-    return FILE().Path(cwd)
-
-def str2url(string):
-    return WEB().str2url(string)
-
-def web_server_ip(request):
-    return WEB(request).GetIP(mode='server')
-
-def web_client_ip(request):
-    return WEB(request).GetIP(mode='client')
-
-def web_req(host_url=None,**opts):
-    return WEB().Request(host_url,**opts)
-
-def web_session(request):
-    return WEB(request).Session()
-
-def file_rw(name,data=None,out='string',append=False,read=None,overwrite=True):
-    return FILE().Rw(name,data=data,out=out,append=append,read=read,overwrite=overwrite,finfo={})
-
-def rm_file(filelist):
-    return FILE().Rm(filelist)
-
-def screen_kill(self,title):
-    return SCREEN().Kill(title)
-
-def screen_monitor(title,ip,ipmi_user,ipmi_pass,find=[],timeout_sec=600,session_out=10):
-    return SCREEN().Monitor(title,ip,ipmi_user,ipmi_pass,find=find,timeout=timeout_sec,session_out=session_out)
-
-def screen_id(title=None):
-    return SCREEN().Id(title)
-
-def screen_logging(title,cmd):
-    return SCREEN().Log(title,cmd)
-
-def now():
-    return TIME().Int()
-
-def int_sec():
-    return TIME().Int()
-
-def get_function_args(func,mode='defaults'):
-    return FunctionArgs(func,mode=mode)
-
-def Var(src,obj=None,default=None,mode='all',VarType=None):
-    return Variable(src=src,obj=obj,parent=0,default=default,mode=mode,VarType=VarType)
-
-def get_data(data,key=None,ekey=None,default=None,method=None,strip=True,find=[],out_form=None):
-    return Get(data,key=key,ekey=ekey,default=default,method=method,strip=strip,find=find,out_form=out_form,peel=True)
-
-def is_function(find,src=None):
-    return IsFunction(src,find=find)
-
-def get_caller_fcuntion_name(detail=False):
-    return CallerName(detail=detail)
-
-def get_function_list(obj=None):
-    return FunctionList(obj)
-
-def get_pfunction_name():
-    return FunctionName(parent=1)
-
-def get_function_name():
-    return FunctionName()
-
-def clean_ansi(src):
-    return CleanAnsi(src)
-
 def move2first(item,pool):
-    return LIST(pool).Move2first(item)
-
-def Pwd(cwd=None):
-    return FILE().Path(cwd)
-
-def check_version(a,sym,b):
-    return CompVersion(a,sym,b)
-
-def integer(a,default=0):
-    return Int(a,default=default)
-
-def list2str(arr):
-    return Join(arr,symbol=' ')
-
-def _u_str2int(val,encode='utf-8'):
-    return Bytes2Int(val,encode=encode,default='org')
-
-def _u_bytes(val,encode='utf-8'):
-    return Bytes(val,encode=encode)
-
-def _u_bytes2str(val,encode='latin1'):
-    return Str(val,encode=encode)
-
-def _u_byte2str(val,encode='latin1'):
-    return Str(val,encode=encode)
-
-def append2list(*inps,**opts):
-    return LIST(inps[0]).Append(*inps[1:],**opts)
-
-def get_value(src,key=None,default=None,check=[str,list,tuple,dict],err=False):
-    return Get(src,key,default=default,_type_=check,err=err)
-
-def logging(*msg,**opts):
-    return printf(*msg,**opts)
-
-def is_py3():
-    return PyVer(3)
-
-def ip2num(ip):
-    return IpV4(ip,out='int')
-
-def is_ipv4(ipaddr=None):
-    return True if IpV4(ipaddr) else False
-
-def is_bmc_ipv4(ipaddr,port=(623,664,443)):
-    return True if IpV4(ipaddr,port=port) else False
-
-def is_port_ip(ipaddr,port):
-    return True if IpV4(ipaddr,port=port) else False
-
-def ipv4(ipaddr=None,chk=False):
-    return IpV4(ipaddr)
-
-def ip_in_range(ip,start,end):
-    return IP(ip).InRange(start,end)
-
-def string2data(src,default='org',want_type=None,spliter=None):
-    return TypeData(src,default,want_type,spliter)
-
-def mac2str(mac,case='lower'):
-    return MacV4(mac,case=case)
-
-def str2mac(mac,sym=':',case='lower',chk=False):
-    return MacV4(mac,symbol=sym,case=case)
-
-def is_mac4(mac=None,symbol=':',convert=True):
-    return True if MacV4(mac,symbol=symbol) else False
-
-def Wrap(src,space='',space_mode='space',sym='\n',default=None,NFLT=False,out=str):
-    if isinstance(space,str): space=len(space)
-    return WrapString(src,fspace=space,nspace=space,new_line=sym,NFLT=NFLT,mode=space_mode,default=default,out=out)
-
-def ddict(*inps,**opts):
-    return Dict(*inps,**opts)
-
-def replacestr(data,org,new):
-    return Replace(data,org,new)
-
-def findstr(string,find,prs=None,split_symbol='\n',patern=True):
-    return FIND(string).Find(find,sym=split_symbol,prs=prs,peel=False)
-
-def get_key(dic=None,find=None):
-    return GetKey(dic,find=find)
-
-def find_key_from_value(dic=None,find=None):
-    return GetKey(dic,find=find)
-
-def is_cancel(func):
-    return IsCancel(func)
+    if item:
+        if type(pool) is list and item in pool:
+            pool.remove(item)
+        return [item]+pool
+    return pool
 
-def file_mode(val):
-    return FILE().Mode(val)
```

### Comparing `kmisc-2.1.85/setup.py` & `kmisc-2.1.9/setup.py`

 * *Files identical despite different names*

