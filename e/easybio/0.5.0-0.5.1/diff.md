# Comparing `tmp/easybio-0.5.0.tar.gz` & `tmp/easybio-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easybio-0.5.0.tar", last modified: Tue Jul 25 05:26:55 2023, max compression
+gzip compressed data, was "easybio-0.5.1.tar", last modified: Wed Aug  2 13:38:40 2023, max compression
```

## Comparing `easybio-0.5.0.tar` & `easybio-0.5.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 lei       (1003) lei       (1004)        0 2023-07-25 05:26:55.715113 easybio-0.5.0/
--rw-rw-r--   0 lei       (1003) lei       (1004)      538 2023-07-25 05:26:55.715113 easybio-0.5.0/PKG-INFO
--rwxrwxrwx   0 lei       (1003) lei       (1004)       30 2023-07-19 17:27:09.000000 easybio-0.5.0/README.md
-drwxrwxr-x   0 lei       (1003) lei       (1004)        0 2023-07-25 05:26:55.711118 easybio-0.5.0/easyBio/
--rw-rw-r--   0 lei       (1003) lei       (1004)     3907 2023-07-22 14:54:20.000000 easybio-0.5.0/easyBio/SetupBioEnv.py
-drwxrwxr-x   0 lei       (1003) lei       (1004)        0 2023-07-25 05:26:55.715113 easybio-0.5.0/easyBio/Utils/
--rwxrwxrwx   0 lei       (1003) lei       (1004)      661 2023-07-19 17:27:08.000000 easybio-0.5.0/easyBio/Utils/__init__.py
--rwxrwxrwx   0 lei       (1003) lei       (1004)     2854 2023-07-19 17:27:08.000000 easybio-0.5.0/easyBio/Utils/downLoadBAM.py
--rwxrwxrwx   0 lei       (1003) lei       (1004)     2901 2023-07-19 17:27:08.000000 easybio-0.5.0/easyBio/Utils/downLoadSRA.py
--rwxrwxrwx   0 lei       (1003) lei       (1004)     8221 2023-07-19 17:27:08.000000 easybio-0.5.0/easyBio/Utils/download.py
--rwxrwxrwx   0 lei       (1003) lei       (1004)     4193 2023-07-19 17:27:08.000000 easybio-0.5.0/easyBio/Utils/downloadUtils.py
--rwxrwxrwx   0 lei       (1003) lei       (1004)     9077 2023-07-19 17:27:08.000000 easybio-0.5.0/easyBio/Utils/easyBioUtils.py
--rwxrwxrwx   0 lei       (1003) lei       (1004)     2216 2023-07-19 17:27:08.000000 easybio-0.5.0/easyBio/Utils/easyCellranger.py
--rwxrwxrwx   0 lei       (1003) lei       (1004)    12094 2023-07-21 16:38:47.000000 easybio-0.5.0/easyBio/Utils/gsaDownLoadUtils.py
--rwxrwxrwx   0 lei       (1003) lei       (1004)     2117 2023-07-19 17:27:08.000000 easybio-0.5.0/easyBio/Utils/netUtils.py
--rwxrwxrwx   0 lei       (1003) lei       (1004)     2594 2023-07-19 17:27:08.000000 easybio-0.5.0/easyBio/Utils/runvelocityc.py
--rwxrwxrwx   0 lei       (1003) lei       (1004)     7773 2023-07-19 17:27:08.000000 easybio-0.5.0/easyBio/Utils/toFastq.py
--rwxrwxrwx   0 lei       (1003) lei       (1004)     4019 2023-07-19 17:27:08.000000 easybio-0.5.0/easyBio/Utils/toolsUtils.py
--rwxrwxrwx   0 lei       (1003) lei       (1004)      426 2023-07-19 17:27:08.000000 easybio-0.5.0/easyBio/__init__.py
--rwxrwxrwx   0 lei       (1003) lei       (1004)     6283 2023-07-21 16:36:07.000000 easybio-0.5.0/easyBio/changeSRAName.py
--rwxrwxrwx   0 lei       (1003) lei       (1004)     2136 2023-07-19 17:27:08.000000 easybio-0.5.0/easyBio/downloadSRA.py
--rwxrwxrwx   0 lei       (1003) lei       (1004)     5153 2023-07-19 18:23:11.000000 easybio-0.5.0/easyBio/easyBio.py
--rwxrwxrwx   0 lei       (1003) lei       (1004)     2636 2023-07-21 16:35:25.000000 easybio-0.5.0/easyBio/gsaPipline.py
--rwxrwxrwx   0 lei       (1003) lei       (1004)     6740 2023-07-21 16:24:07.000000 easybio-0.5.0/easyBio/installConda copy.py
--rwxrwxrwx   0 lei       (1003) lei       (1004)     5856 2023-07-22 14:54:29.000000 easybio-0.5.0/easyBio/installConda.py
--rwxrwxrwx   0 lei       (1003) lei       (1004)     5024 2023-07-19 17:27:09.000000 easybio-0.5.0/easyBio/pipline.py
--rwxrwxrwx   0 lei       (1003) lei       (1004)     1324 2023-07-19 17:27:09.000000 easybio-0.5.0/easyBio/run_cellranger.py
--rwxrwxrwx   0 lei       (1003) lei       (1004)     1247 2023-07-19 17:27:09.000000 easybio-0.5.0/easyBio/runvelocyto.py
--rwxrwxrwx   0 lei       (1003) lei       (1004)     1454 2023-07-21 16:38:49.000000 easybio-0.5.0/easyBio/splitSRA.py
--rwxrwxrwx   0 lei       (1003) lei       (1004)     1006 2023-07-19 17:27:09.000000 easybio-0.5.0/easyBio/test.py
--rwxrwxrwx   0 lei       (1003) lei       (1004)     2671 2023-07-19 17:27:09.000000 easybio-0.5.0/easyBio/tidy.py
-drwxrwxr-x   0 lei       (1003) lei       (1004)        0 2023-07-25 05:26:55.715113 easybio-0.5.0/easybio.egg-info/
--rw-rw-r--   0 lei       (1003) lei       (1004)      538 2023-07-25 05:26:55.000000 easybio-0.5.0/easybio.egg-info/PKG-INFO
--rw-rw-r--   0 lei       (1003) lei       (1004)      887 2023-07-25 05:26:55.000000 easybio-0.5.0/easybio.egg-info/SOURCES.txt
--rw-rw-r--   0 lei       (1003) lei       (1004)        1 2023-07-25 05:26:55.000000 easybio-0.5.0/easybio.egg-info/dependency_links.txt
--rw-rw-r--   0 lei       (1003) lei       (1004)      433 2023-07-25 05:26:55.000000 easybio-0.5.0/easybio.egg-info/entry_points.txt
--rw-rw-r--   0 lei       (1003) lei       (1004)        1 2023-07-25 05:26:55.000000 easybio-0.5.0/easybio.egg-info/not-zip-safe
--rw-rw-r--   0 lei       (1003) lei       (1004)       38 2023-07-25 05:26:55.000000 easybio-0.5.0/easybio.egg-info/requires.txt
--rw-rw-r--   0 lei       (1003) lei       (1004)        8 2023-07-25 05:26:55.000000 easybio-0.5.0/easybio.egg-info/top_level.txt
--rw-rw-r--   0 lei       (1003) lei       (1004)       38 2023-07-25 05:26:55.715113 easybio-0.5.0/setup.cfg
--rwxrwxrwx   0 lei       (1003) lei       (1004)     1690 2023-07-25 05:26:06.000000 easybio-0.5.0/setup.py
+drwxrwxr-x   0 lei       (1003) lei       (1004)        0 2023-08-02 13:38:40.957392 easybio-0.5.1/
+-rw-rw-r--   0 lei       (1003) lei       (1004)      536 2023-08-02 13:38:40.957392 easybio-0.5.1/PKG-INFO
+-rwxrwxrwx   0 lei       (1003) lei       (1004)       30 2023-07-19 17:27:09.000000 easybio-0.5.1/README.md
+drwxrwxr-x   0 lei       (1003) lei       (1004)        0 2023-08-02 13:38:40.957392 easybio-0.5.1/easyBio/
+-rw-rw-r--   0 lei       (1003) lei       (1004)     3907 2023-07-22 14:54:20.000000 easybio-0.5.1/easyBio/SetupBioEnv.py
+drwxrwxr-x   0 lei       (1003) lei       (1004)        0 2023-08-02 13:38:40.957392 easybio-0.5.1/easyBio/Utils/
+-rwxrwxrwx   0 lei       (1003) lei       (1004)      661 2023-07-19 17:27:08.000000 easybio-0.5.1/easyBio/Utils/__init__.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     3127 2023-08-02 12:04:04.000000 easybio-0.5.1/easyBio/Utils/downLoadBAM.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     3319 2023-08-02 12:22:08.000000 easybio-0.5.1/easyBio/Utils/downLoadSRA.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     8419 2023-08-02 12:22:03.000000 easybio-0.5.1/easyBio/Utils/download.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     4193 2023-07-19 17:27:08.000000 easybio-0.5.1/easyBio/Utils/downloadUtils.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     9077 2023-07-19 17:27:08.000000 easybio-0.5.1/easyBio/Utils/easyBioUtils.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     2216 2023-07-19 17:27:08.000000 easybio-0.5.1/easyBio/Utils/easyCellranger.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)    12226 2023-08-02 12:05:04.000000 easybio-0.5.1/easyBio/Utils/gsaDownLoadUtils.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     2117 2023-07-19 17:27:08.000000 easybio-0.5.1/easyBio/Utils/netUtils.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     2594 2023-07-19 17:27:08.000000 easybio-0.5.1/easyBio/Utils/runvelocityc.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     7773 2023-07-19 17:27:08.000000 easybio-0.5.1/easyBio/Utils/toFastq.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     4019 2023-07-19 17:27:08.000000 easybio-0.5.1/easyBio/Utils/toolsUtils.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)      426 2023-07-19 17:27:08.000000 easybio-0.5.1/easyBio/__init__.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     6283 2023-07-21 16:36:07.000000 easybio-0.5.1/easyBio/changeSRAName.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     2136 2023-08-02 12:00:02.000000 easybio-0.5.1/easyBio/downloadSRA.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     5153 2023-07-19 18:23:11.000000 easybio-0.5.1/easyBio/easyBio.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     2906 2023-08-02 12:02:08.000000 easybio-0.5.1/easyBio/gsaPipline.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     6740 2023-07-21 16:24:07.000000 easybio-0.5.1/easyBio/installConda copy.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     5856 2023-07-22 14:54:29.000000 easybio-0.5.1/easyBio/installConda.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     5847 2023-08-02 13:00:18.000000 easybio-0.5.1/easyBio/pipline.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     1324 2023-07-19 17:27:09.000000 easybio-0.5.1/easyBio/run_cellranger.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     1247 2023-07-19 17:27:09.000000 easybio-0.5.1/easyBio/runvelocyto.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     1454 2023-07-21 16:38:49.000000 easybio-0.5.1/easyBio/splitSRA.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     1006 2023-07-19 17:27:09.000000 easybio-0.5.1/easyBio/test.py
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     2671 2023-07-19 17:27:09.000000 easybio-0.5.1/easyBio/tidy.py
+drwxrwxr-x   0 lei       (1003) lei       (1004)        0 2023-08-02 13:38:40.957392 easybio-0.5.1/easybio.egg-info/
+-rw-rw-r--   0 lei       (1003) lei       (1004)      536 2023-08-02 13:38:40.000000 easybio-0.5.1/easybio.egg-info/PKG-INFO
+-rw-rw-r--   0 lei       (1003) lei       (1004)      887 2023-08-02 13:38:40.000000 easybio-0.5.1/easybio.egg-info/SOURCES.txt
+-rw-rw-r--   0 lei       (1003) lei       (1004)        1 2023-08-02 13:38:40.000000 easybio-0.5.1/easybio.egg-info/dependency_links.txt
+-rw-rw-r--   0 lei       (1003) lei       (1004)      432 2023-08-02 13:38:40.000000 easybio-0.5.1/easybio.egg-info/entry_points.txt
+-rw-rw-r--   0 lei       (1003) lei       (1004)        1 2023-08-02 13:38:27.000000 easybio-0.5.1/easybio.egg-info/not-zip-safe
+-rw-rw-r--   0 lei       (1003) lei       (1004)       38 2023-08-02 13:38:40.000000 easybio-0.5.1/easybio.egg-info/requires.txt
+-rw-rw-r--   0 lei       (1003) lei       (1004)        8 2023-08-02 13:38:40.000000 easybio-0.5.1/easybio.egg-info/top_level.txt
+-rw-rw-r--   0 lei       (1003) lei       (1004)       38 2023-08-02 13:38:40.957392 easybio-0.5.1/setup.cfg
+-rwxrwxrwx   0 lei       (1003) lei       (1004)     1690 2023-08-02 13:19:43.000000 easybio-0.5.1/setup.py
```

### Comparing `easybio-0.5.0/PKG-INFO` & `easybio-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easybio
-Version: 0.5.0
+Version: 0.5.1
 Summary: The purpose of the creation of this package is to make bioinformatics analysis simpler.
 Home-page: https://github.com/xleizi/easyBio_conda
 Author: Lei Cui
 Author-email: cuilei798@qq.com
 Maintainer: Lei Cui
 Maintainer-email: cuilei798@qq.com
 License: MIT License
@@ -12,9 +12,7 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 
 # easyBio_conda
 easyBio_conda
-
-
```

### Comparing `easybio-0.5.0/easyBio/SetupBioEnv.py` & `easybio-0.5.1/easyBio/SetupBioEnv.py`

 * *Files identical despite different names*

### Comparing `easybio-0.5.0/easyBio/Utils/__init__.py` & `easybio-0.5.1/easyBio/Utils/__init__.py`

 * *Files identical despite different names*

### Comparing `easybio-0.5.0/easyBio/Utils/downLoadBAM.py` & `easybio-0.5.1/easyBio/Utils/downLoadBAM.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import math
 import os
 from .download import Download
 from .toolsUtils import sraMd5Cal
 
 class downLoadBAM:
-    def __init__(self, results, rawdirs: str, threads=16, bamDir="bam") -> None:
+    def __init__(self, results, rawdirs: str, threads=16, bamDir="bam", gseList=[], ShowDownloadProgress=True) -> None:
         self.results = results
         self.rawdirs = rawdirs
         self.threads = threads
+        self.gseList = gseList
+        self.ShowDownloadProgress = ShowDownloadProgress
         self.bamfolder = f"{rawdirs}/{bamDir}"
         self.makbamdirs()
         self.addBamName()
         self.getmd5Map()
         # print(self.isDownloadAll())
         # self.Download()
 
@@ -26,16 +28,17 @@
 
     def makbamdirs(self):
         os.makedirs(self.bamfolder, exist_ok=True)
 
     def getmd5Map(self):
         self.md5List = {}
         for result in self.results:
-            bammd5 = result["submitted_md5"].split(";")[0]
-            self.md5List[result["bamName"]] = bammd5
+            if result["sample_alias"] in self.gseList or self.ShowDownloadProgress == []:
+                bammd5 = result["submitted_md5"].split(";")[0]
+                self.md5List[result["bamName"]] = bammd5
         print(self.md5List)
         return self.md5List
 
     def isDownloadAll(self):
         exitCount = sum(1 for study in self.results if os.path.exists(
             f"{self.bamfolder}/{study['bamName']}"))
         return exitCount == len(self.results)
@@ -70,10 +73,10 @@
             downloadStu = False
             srcCount = 0
             while not downloadStu:
                 srcCount += 1
                 bam_ftp = f"https://sra-pub-src-{srcCount}.s3.amazonaws.com/{run_accession}/{bamName}.1"
                 print(bam_ftp)
                 download = Download(bam_ftp, dirs=self.bamfolder, fileName=f"{bamName}",
-                                    threadNum=self.threads, limitTime=60000)
+                                    threadNum=self.threads, limitTime=60000, ShowDownloadProgress=self.ShowDownloadProgress)
                 downloadStu = download.start() if srcCount < 10 else True
         return False
```

### Comparing `easybio-0.5.0/easyBio/Utils/downLoadSRA.py` & `easybio-0.5.1/easyBio/Utils/downLoadSRA.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import math
 import os
 from .download import Download
 from .toolsUtils import sraMd5Cal
 
 class downLoadSRA:
-    def __init__(self, results, rawdirs: str, threads=16, sraDir="sra") -> None:
+    def __init__(self, results, rawdirs: str, threads=16, 
+                 sraDir="sra", gseList=[], ShowDownloadProgress=True) -> None:
         self.results = results
         self.rawdirs = rawdirs
         self.threads = threads
+        self.gseList = gseList
+        self.ShowDownloadProgress = ShowDownloadProgress
         self.srafolder = f"{rawdirs}/{sraDir}"
         self.maksradirs()
         self.addSRAName()
         self.getmd5Map()
         self.getSample_aliasList()
         # print(self.isDownloadAll())
         # self.DownloadBam()
@@ -28,22 +31,24 @@
         os.makedirs(self.srafolder, exist_ok=True)
 
     def getmd5Map(self):
         self.md5List = {}
         for result in self.results:
             sra_md5 = result["sra_md5"]
             if sra_md5 != "":
-                self.md5List[result["sraName"]] = sra_md5
+                if result["sample_alias"] in self.gseList or self.ShowDownloadProgress == []:
+                    self.md5List[result["sraName"]] = sra_md5
         print(self.md5List)
         return self.md5List
     
     def getSample_aliasList(self):
         sample_aliasList = {}
         for result in self.results:
-            sample_aliasList[result["sraName"]] = result["sample_alias"]
+            if result["sample_alias"] in self.gseList or self.ShowDownloadProgress == []:
+                sample_aliasList[result["sraName"]] = result["sample_alias"]
         self.sampleMap = sample_aliasList
         return self.sampleMap
     
     def isDownloadAll(self):
         exitCount = sum(1 for study in self.results if os.path.exists(
             f"{self.srafolder}/{study['run_accession']}.sra"))
         return exitCount == len(self.results)
@@ -73,11 +78,12 @@
         for study in self.results:
             run_accession = study["run_accession"]
             print("\033[33mrun_accession: {}\033[0m".format(run_accession))
             # sra_md5 = study["sra_md5"]
             bam_ftp = f"https://sra-pub-run-odp.s3.amazonaws.com/sra/{run_accession}/{run_accession}"
             print(bam_ftp)
             download = Download(bam_ftp, dirs=self.srafolder, fileName=f"{run_accession}.sra",
-                                threadNum=self.threads, limitTime=60000)
+                                threadNum=self.threads, limitTime=60000, 
+                                ShowDownloadProgress=self.ShowDownloadProgress)
             download.start()
 
         return False
```

### Comparing `easybio-0.5.0/easyBio/Utils/download.py` & `easybio-0.5.1/easyBio/Utils/download.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,27 +9,30 @@
 from time import time
 import urllib.parse
 
 from .toolsUtils import getNowTime
 
 
 class Download:
-    def __init__(self, url: str, fileName: str = None, dirs: str = None, perPartSize: int = 1024*1024*10, threadNum: int = 5, limitTime=3000) -> None:
+    def __init__(self, url: str, fileName: str = None, dirs: str = None, 
+                 perPartSize: int = 1024*1024*10, threadNum: int = 5, limitTime=3000,
+                 ShowDownloadProgress=True) -> None:
         """
         初始化
         @url：文件链接
         @fileName：文件名(默认从链接中获取)
         @perPartSize：单线程下载大小(默认10MB)
         @threadNum：线程数(默认5)
         @limitTime：单线程1%进度限制时间,超时重新执行该线程(ms)
         """
         self.url = url
         self.perPartSize = perPartSize
         self.threadNum = threadNum
         self.limitTime = limitTime
+        self.ShowDownloadProgress = ShowDownloadProgress
         if (not fileName):
             self.fileName = self.getFileName()
         else:
             self.fileName = fileName
         if (not dirs):
             self.dirs = self.getdirs()
         else:
@@ -90,16 +93,17 @@
         """
         indexTip = f"{index}/{self.partNum-1}"  # 分块位置提示
         totalSize = end-start+1  # 分块总大小
         needDownSize = self.preDownload(index, totalSize)  # 分块剩余大小
 
         if (needDownSize == 0):  # 分块已下载
             # print(f"[{indexTip}][{start}-{end}]下载完成")
-            print(
-                "\033[1;32m[{}][{}-{}] Download completed\033[0m".format(indexTip, start, end))
+            if self.ShowDownloadProgress:
+                print(
+                    "\033[1;32m[{}][{}-{}] Download completed\033[0m".format(indexTip, start, end))
             return
         if (totalSize != needDownSize):  # 分块已存在,追加模式
             file = open(f"{self.dirs}/temp/{self.fileName}_{index}", mode="ba")
         else:  # 分块未存在，新建模式
             file = open(f"{self.dirs}/temp/{self.fileName}_{index}", mode="bw")
 
         currentSize = 0  # 已经下载大小
@@ -127,16 +131,16 @@
                             # print(f"[{divTime}ms][{indexTip}][{progress}%]超时，重新下载---{getNowTime()}")
                             print("\033[1;31m[{}ms][{}][{}%] Timeout, downloading again---{}\033[0m".format(
                                 divTime, indexTip, progress, getNowTime()))
                             file.close()
                             break
                         else:
                             startTime = int(time()*1000)
-                            print(
-                                f"[{divTime}ms][{indexTip}][{progress}%]downloading---{getNowTime()}")
+                            if self.ShowDownloadProgress:
+                                print(f"[{divTime}ms][{indexTip}][{progress}%]downloading---{getNowTime()}")
         if (reDownload):
             self.download(index, start, end)
         else:
             print(f"[{indexTip}][{start}-{end}]下载完成---{getNowTime()}")
 
     def checkParts(self, partList: list) -> bool:
         """
```

### Comparing `easybio-0.5.0/easyBio/Utils/downloadUtils.py` & `easybio-0.5.1/easyBio/Utils/downloadUtils.py`

 * *Files identical despite different names*

### Comparing `easybio-0.5.0/easyBio/Utils/easyBioUtils.py` & `easybio-0.5.1/easyBio/Utils/easyBioUtils.py`

 * *Files identical despite different names*

### Comparing `easybio-0.5.0/easyBio/Utils/easyCellranger.py` & `easybio-0.5.1/easyBio/Utils/easyCellranger.py`

 * *Files identical despite different names*

### Comparing `easybio-0.5.0/easyBio/Utils/gsaDownLoadUtils.py` & `easybio-0.5.1/easyBio/Utils/gsaDownLoadUtils.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,21 +12,22 @@
 
 from .toolsUtils import sraMd5Cal
 from .download import Download
 from .netUtils import requestGet
 from .easyCellranger import easyCellranger
 
 class gsaProject:
-    def __init__(self, inputName: str, dirs_path="./") -> None:
+    def __init__(self, inputName: str, dirs_path="./", ShowDownloadProgress=True) -> None:
         if inputName.startswith("PRJCA"):
             pjurl = f"https://ngdc.cncb.ac.cn/gsa-human/hra/getAjax/searchByPrjAccession?prjAccession={inputName}"
             hra = requestGet(pjurl).json()["listHras"][0]["accession"]
         elif inputName.startswith("HRA"):
             hra = inputName
         self.hra = hra
+        self.ShowDownloadProgress = ShowDownloadProgress
         self.getStudyId()
         # self.readExcel()
         # self.getAccList()
         print("hra:", hra)
         self.dirs_path = f"{dirs_path}/{inputName}"
         self.raw_path = f"{self.dirs_path}/raw"
         self.fq_path = f"{self.raw_path}/fq"
@@ -132,15 +133,15 @@
                 check = self.downloadCheck()
                 while not check:
                     for FileLink in self.fileLinkList:
                         fileurl = f"https://download.cncb{FileLink[18:]}"
                         items = FileLink.split("/")
                         fileName = items[len(items)-1]
                         download = Download(fileurl, dirs=self.fq_path, fileName=fileName,
-                                            threadNum=threads, limitTime=60000)
+                                            threadNum=threads, limitTime=60000, ShowDownloadProgress=self.ShowDownloadProgress)
                         download.start()
                     check = self.downloadCheck()
                 neededDown = self.fileMd5Check()
             try:
                 shutil.rmtree(f"{self.fq_path}/temp")
             except:
                 pass
```

### Comparing `easybio-0.5.0/easyBio/Utils/netUtils.py` & `easybio-0.5.1/easyBio/Utils/netUtils.py`

 * *Files identical despite different names*

### Comparing `easybio-0.5.0/easyBio/Utils/runvelocityc.py` & `easybio-0.5.1/easyBio/Utils/runvelocityc.py`

 * *Files identical despite different names*

### Comparing `easybio-0.5.0/easyBio/Utils/toFastq.py` & `easybio-0.5.1/easyBio/Utils/toFastq.py`

 * *Files identical despite different names*

### Comparing `easybio-0.5.0/easyBio/Utils/toolsUtils.py` & `easybio-0.5.1/easyBio/Utils/toolsUtils.py`

 * *Files identical despite different names*

### Comparing `easybio-0.5.0/easyBio/changeSRAName.py` & `easybio-0.5.1/easyBio/changeSRAName.py`

 * *Files identical despite different names*

### Comparing `easybio-0.5.0/easyBio/downloadSRA.py` & `easybio-0.5.1/easyBio/downloadSRA.py`

 * *Files identical despite different names*

### Comparing `easybio-0.5.0/easyBio/easyBio.py` & `easybio-0.5.1/easyBio/easyBio.py`

 * *Files identical despite different names*

### Comparing `easybio-0.5.0/easyBio/gsaPipline.py` & `easybio-0.5.1/easyBio/gsaPipline.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,28 +30,31 @@
                         default="", help="otherItem for cellranger")
     parser.add_argument("-rmf", "--rmsk_file", type=str,
                         help="Path to the hg38_rmsk.gtf file")
     parser.add_argument("-gtf", "--gtf_file", type=str,
                         help="Path to the Homo_sapiens.GRCh38.109.gtf file")
     parser.add_argument("-vm", "--max_memory", type=int,
                         default=200, help="Maximum memory in GB (default: 200)")
-
+    parser.add_argument("-sdp", "--ShowDownloadProgress", type=bool, default=True,
+                        help="Whether to show the download progress")
 
     args = parser.parse_args()
     inputName = args.inputName
     dirs = args.dirs
     threads = args.threads
     db_path = args.db_path
     expectcellnum = args.expectcellnum
     rmsk_file = args.rmsk_file
     gtf_file = args.gtf_file
     max_memory = args.max_memory
     otherItem = args.other_Item
+    ShowDownloadProgress = args.ShowDownloadProgress
 
-    gsap = gsaProject(inputName=inputName, dirs_path=dirs)
+    gsap = gsaProject(inputName=inputName, dirs_path=dirs,
+                      ShowDownloadProgress=ShowDownloadProgress)
     gsap.downloadFiles(threads=threads, copy=True)
     gsap.renamegsa()
     
     print("\033[1;33m{}\033[0m".format("*" * 80))   # 黄
     gsap.cellrangerRun(db_path, expectcellnum, otherItem)
     print("\033[1;33m{}\033[0m".format("*" * 80))   # 黄
```

### Comparing `easybio-0.5.0/easyBio/installConda copy.py` & `easybio-0.5.1/easyBio/installConda copy.py`

 * *Files identical despite different names*

### Comparing `easybio-0.5.0/easyBio/installConda.py` & `easybio-0.5.1/easyBio/installConda.py`

 * *Files identical despite different names*

### Comparing `easybio-0.5.0/easyBio/pipline.py` & `easybio-0.5.1/easyBio/pipline.py`

 * *Files 21% similar despite different names*

```diff
@@ -23,16 +23,19 @@
     parser = argparse.ArgumentParser(
         description="Process GSE number, directory and threads")
     parser.add_argument("-g", "--gsenumber", help="GSE number")
     parser.add_argument("-d", "--dirs", default=os.getcwd(),
                         help="Directory (default: current directory)")
     parser.add_argument("-t", "--threads", type=int, default=num_threads,
                         help="Number of threads (default: your cpucounts)")
-    parser.add_argument("-df", "--DownloadFirst", type=bool, default=False,
+    parser.add_argument("-df", "--DownloadFirst", action='store_true',
                         help="Download sra data first")
+    parser.add_argument("-dl", "--DownloadList", help="The GSM list to Download")
+    parser.add_argument("-hdp", "--HideDownloadProgress", action='store_true',
+                    help="Whether to show the download progress")
     parser.add_argument("-k", "--kind", default="--split-files",
                         help="Zhe kind of split")
     parser.add_argument("-l", "--list_file", help="matching list")
     parser.add_argument("-db", "--db_path", required=True,
                         help="Path to the gene reference file (required)")
     parser.add_argument("-ec", "--expectcellnum", type=int, default=3000,
                         help="Expected cell number for running cellranger (default: 3000)")
@@ -53,36 +56,47 @@
     db_path = args.db_path
     expectcellnum = args.expectcellnum
     list_file = args.list_file
     rmsk_file = args.rmsk_file
     gtf_file = args.gtf_file
     max_memory = args.max_memory
     otherItem = args.other_Item
+    DownloadList = args.DownloadList
     downloadFist = args.DownloadFirst
+    showDownloadProgress = not args.HideDownloadProgress
     
+    print(downloadFist)
+    print(showDownloadProgress)
+    print(max_memory)
     gList = gsenumberList.split(",")
     print(gList)
+    gseList = []
+    if DownloadList != None:
+        gseList = DownloadList.split(",")
+    print(gseList)
     
     if downloadFist:
         for gsenumber in gList:
             rawdirs = f"{dirs}/{gsenumber}/raw"
             # folder = f"{rawdirs}/sra"
             # os.makedirs(folder, exist_ok=True)
 
             # print("\033[1;33m{}\033[0m".format(folder))   # 黄
 
             # 下载 SRA 数据
             results = getProResults(gsenumber)
 
-            ds = downLoadSRA(results, rawdirs, threads)
+            ds = downLoadSRA(results, rawdirs, threads, gseList=gseList,
+                             ShowDownloadProgress=showDownloadProgress)
             print(ds.md5List)
             print(ds.sampleMap)
             
             if ds.md5List == {}:
-                db = downLoadBAM(results, rawdirs, threads)
+                db = downLoadBAM(results, rawdirs, threads, gseList=gseList,
+                                 ShowDownloadProgress=showDownloadProgress)
                 db.Download()
             else:
                ds.Download()
             print("\033[1;33m{}\033[0m".format("*" * 80))   # 黄
 
     for gsenumber in gList:
         rawdirs = f"{dirs}/{gsenumber}/raw"
@@ -90,19 +104,21 @@
         # os.makedirs(folder, exist_ok=True)
 
         # print("\033[1;33m{}\033[0m".format(folder))   # 黄
 
         # 下载 SRA 数据
         results = getProResults(gsenumber)
 
-        ds = downLoadSRA(results, rawdirs, threads)
+        ds = downLoadSRA(results, rawdirs, threads,
+                         ShowDownloadProgress=showDownloadProgress)
         print(ds.md5List)
 
         if ds.md5List == {}:
-            db = downLoadBAM(results, rawdirs, threads)
+            db = downLoadBAM(results, rawdirs, threads,
+                             ShowDownloadProgress=showDownloadProgress)
             db.Download()
             tofq = toFastq(db.bamfolder, type="bam", FastqDir=f"{rawdirs}/fq", threads=threads)
             tofq.BAMtoFastq(f"{rawdirs}/tofq")
             # exit()
         else:
             ds.Download()
             tofq = toFastq(ds.srafolder, FastqDir=f"{rawdirs}/fq", threads=threads)
```

### Comparing `easybio-0.5.0/easyBio/run_cellranger.py` & `easybio-0.5.1/easyBio/run_cellranger.py`

 * *Files identical despite different names*

### Comparing `easybio-0.5.0/easyBio/runvelocyto.py` & `easybio-0.5.1/easyBio/runvelocyto.py`

 * *Files identical despite different names*

### Comparing `easybio-0.5.0/easyBio/splitSRA.py` & `easybio-0.5.1/easyBio/splitSRA.py`

 * *Files identical despite different names*

### Comparing `easybio-0.5.0/easyBio/test.py` & `easybio-0.5.1/easyBio/test.py`

 * *Files identical despite different names*

### Comparing `easybio-0.5.0/easyBio/tidy.py` & `easybio-0.5.1/easyBio/tidy.py`

 * *Files identical despite different names*

### Comparing `easybio-0.5.0/easybio.egg-info/PKG-INFO` & `easybio-0.5.1/easybio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easybio
-Version: 0.5.0
+Version: 0.5.1
 Summary: The purpose of the creation of this package is to make bioinformatics analysis simpler.
 Home-page: https://github.com/xleizi/easyBio_conda
 Author: Lei Cui
 Author-email: cuilei798@qq.com
 Maintainer: Lei Cui
 Maintainer-email: cuilei798@qq.com
 License: MIT License
@@ -12,9 +12,7 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 
 # easyBio_conda
 easyBio_conda
-
-
```

### Comparing `easybio-0.5.0/easybio.egg-info/SOURCES.txt` & `easybio-0.5.1/easybio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easybio-0.5.0/setup.py` & `easybio-0.5.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 
-VERSION = '0.5.0'
+VERSION = '0.5.1'
 
 setup(
     name='easybio',  # package name
     version=VERSION,  # package version
     author='Lei Cui',
     author_email='cuilei798@qq.com',
     maintainer='Lei Cui',
```

