# Comparing `tmp/langBOTs-0.0.2.tar.gz` & `tmp/langBOTs-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langBOTs-0.0.2.tar", last modified: Wed Aug  2 14:22:42 2023, max compression
+gzip compressed data, was "langBOTs-0.0.3.tar", last modified: Wed Aug  2 14:35:29 2023, max compression
```

## Comparing `langBOTs-0.0.2.tar` & `langBOTs-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 14:22:42.498839 langBOTs-0.0.2/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1061 2023-08-02 14:04:38.000000 langBOTs-0.0.2/LICENSE.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      537 2023-08-02 14:22:42.498839 langBOTs-0.0.2/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      846 2023-08-02 13:25:09.000000 langBOTs-0.0.2/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 14:22:42.494839 langBOTs-0.0.2/langBOTs/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-08-02 06:40:02.000000 langBOTs-0.0.2/langBOTs/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1964 2023-08-02 13:39:54.000000 langBOTs-0.0.2/langBOTs/api.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1509 2023-08-02 11:12:34.000000 langBOTs-0.0.2/langBOTs/chain.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      239 2023-08-02 06:39:00.000000 langBOTs-0.0.2/langBOTs/main.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1941 2023-08-02 13:10:25.000000 langBOTs-0.0.2/langBOTs/query.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3725 2023-08-02 10:21:08.000000 langBOTs-0.0.2/langBOTs/scrapsplitvec.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 14:22:42.498839 langBOTs-0.0.2/langBOTs.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      537 2023-08-02 14:22:42.000000 langBOTs-0.0.2/langBOTs.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      315 2023-08-02 14:22:42.000000 langBOTs-0.0.2/langBOTs.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-08-02 14:22:42.000000 langBOTs-0.0.2/langBOTs.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      110 2023-08-02 14:22:42.000000 langBOTs-0.0.2/langBOTs.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-08-02 14:22:42.000000 langBOTs-0.0.2/langBOTs.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       79 2023-08-02 14:22:42.498839 langBOTs-0.0.2/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1155 2023-08-02 14:22:35.000000 langBOTs-0.0.2/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 14:35:29.146839 langBOTs-0.0.3/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1061 2023-08-02 14:04:38.000000 langBOTs-0.0.3/LICENSE.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1422 2023-08-02 14:35:29.146839 langBOTs-0.0.3/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      844 2023-08-02 14:25:44.000000 langBOTs-0.0.3/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 14:35:29.146839 langBOTs-0.0.3/langBOTs/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-08-02 06:40:02.000000 langBOTs-0.0.3/langBOTs/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1964 2023-08-02 13:39:54.000000 langBOTs-0.0.3/langBOTs/api.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1509 2023-08-02 11:12:34.000000 langBOTs-0.0.3/langBOTs/chain.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      239 2023-08-02 06:39:00.000000 langBOTs-0.0.3/langBOTs/main.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1941 2023-08-02 13:10:25.000000 langBOTs-0.0.3/langBOTs/query.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3725 2023-08-02 10:21:08.000000 langBOTs-0.0.3/langBOTs/scrapsplitvec.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 14:35:29.146839 langBOTs-0.0.3/langBOTs.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1422 2023-08-02 14:35:29.000000 langBOTs-0.0.3/langBOTs.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      315 2023-08-02 14:35:29.000000 langBOTs-0.0.3/langBOTs.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-08-02 14:35:29.000000 langBOTs-0.0.3/langBOTs.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      110 2023-08-02 14:35:29.000000 langBOTs-0.0.3/langBOTs.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-08-02 14:35:29.000000 langBOTs-0.0.3/langBOTs.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      804 2023-08-02 14:35:29.146839 langBOTs-0.0.3/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1155 2023-08-02 14:35:04.000000 langBOTs-0.0.3/setup.py
```

### Comparing `langBOTs-0.0.2/LICENSE.txt` & `langBOTs-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langBOTs-0.0.2/README.md` & `langBOTs-0.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-
-
 LangBOTs
 
 # Foobar
 
 A silly library which combines scraping, langchain and flask.
 Inspired by [prompt engineering](https://www.youtube.com/@engineerprompt)
```

### Comparing `langBOTs-0.0.2/langBOTs/api.py` & `langBOTs-0.0.3/langBOTs/api.py`

 * *Files identical despite different names*

### Comparing `langBOTs-0.0.2/langBOTs/chain.py` & `langBOTs-0.0.3/langBOTs/chain.py`

 * *Files identical despite different names*

### Comparing `langBOTs-0.0.2/langBOTs/query.py` & `langBOTs-0.0.3/langBOTs/query.py`

 * *Files identical despite different names*

### Comparing `langBOTs-0.0.2/langBOTs/scrapsplitvec.py` & `langBOTs-0.0.3/langBOTs/scrapsplitvec.py`

 * *Files identical despite different names*

### Comparing `langBOTs-0.0.2/setup.py` & `langBOTs-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='langBOTs',
-    version='0.0.2',
+    version='0.0.3',
     author='Rajat S',
     description='Scrape, Langchain, Deploy !',
     url = 'https://github.com/gapirajat/langBOTs',
     packages=find_packages(),
     install_requires=[
         # List any dependencies your package requires here
         'langchain',
```

