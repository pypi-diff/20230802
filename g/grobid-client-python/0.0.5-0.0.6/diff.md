# Comparing `tmp/grobid_client_python-0.0.5.tar.gz` & `tmp/grobid_client_python-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grobid_client_python-0.0.5.tar", last modified: Sun Mar  5 19:00:52 2023, max compression
+gzip compressed data, was "grobid_client_python-0.0.6.tar", last modified: Wed Aug  2 13:06:12 2023, max compression
```

## Comparing `grobid_client_python-0.0.5.tar` & `grobid_client_python-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-03-05 19:00:52.045967 grobid_client_python-0.0.5/
--rwxrwxr-x   0 lopez     (1000) lopez     (1000)    11184 2023-03-05 18:59:18.000000 grobid_client_python-0.0.5/LICENSE
--rw-rw-r--   0 lopez     (1000) lopez     (1000)     9817 2023-03-05 19:00:52.045967 grobid_client_python-0.0.5/PKG-INFO
-drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-03-05 19:00:52.045967 grobid_client_python-0.0.5/grobid_client/
--rw-rw-r--   0 lopez     (1000) lopez     (1000)        0 2021-04-21 20:34:41.000000 grobid_client_python-0.0.5/grobid_client/__init__.py
--rw-rw-r--   0 lopez     (1000) lopez     (1000)     6009 2023-03-05 18:40:32.000000 grobid_client_python-0.0.5/grobid_client/client.py
--rw-rw-r--   0 lopez     (1000) lopez     (1000)    16699 2023-03-05 18:59:00.000000 grobid_client_python-0.0.5/grobid_client/grobid_client.py
-drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-03-05 19:00:52.045967 grobid_client_python-0.0.5/grobid_client_python.egg-info/
--rw-rw-r--   0 lopez     (1000) lopez     (1000)     9817 2023-03-05 19:00:51.000000 grobid_client_python-0.0.5/grobid_client_python.egg-info/PKG-INFO
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      363 2023-03-05 19:00:52.000000 grobid_client_python-0.0.5/grobid_client_python.egg-info/SOURCES.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)        1 2023-03-05 19:00:51.000000 grobid_client_python-0.0.5/grobid_client_python.egg-info/dependency_links.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)       67 2023-03-05 19:00:51.000000 grobid_client_python-0.0.5/grobid_client_python.egg-info/entry_points.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)        9 2023-03-05 19:00:51.000000 grobid_client_python-0.0.5/grobid_client_python.egg-info/requires.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)       14 2023-03-05 19:00:51.000000 grobid_client_python-0.0.5/grobid_client_python.egg-info/top_level.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)       38 2023-03-05 19:00:52.045967 grobid_client_python-0.0.5/setup.cfg
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      662 2023-03-05 18:59:06.000000 grobid_client_python-0.0.5/setup.py
+drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-08-02 13:06:12.325337 grobid_client_python-0.0.6/
+-rwxrwxr-x   0 lopez     (1000) lopez     (1000)    11184 2023-03-05 18:59:18.000000 grobid_client_python-0.0.6/LICENSE
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)     9838 2023-08-02 13:06:12.321337 grobid_client_python-0.0.6/PKG-INFO
+drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-08-02 13:06:12.317337 grobid_client_python-0.0.6/grobid_client/
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)        0 2021-04-21 20:34:41.000000 grobid_client_python-0.0.6/grobid_client/__init__.py
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)     6009 2023-03-05 18:40:32.000000 grobid_client_python-0.0.6/grobid_client/client.py
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)    16720 2023-08-02 12:49:30.000000 grobid_client_python-0.0.6/grobid_client/grobid_client.py
+drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-08-02 13:06:12.321337 grobid_client_python-0.0.6/grobid_client_python.egg-info/
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)     9838 2023-08-02 13:06:11.000000 grobid_client_python-0.0.6/grobid_client_python.egg-info/PKG-INFO
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      363 2023-08-02 13:06:12.000000 grobid_client_python-0.0.6/grobid_client_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)        1 2023-08-02 13:06:11.000000 grobid_client_python-0.0.6/grobid_client_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)       67 2023-08-02 13:06:11.000000 grobid_client_python-0.0.6/grobid_client_python.egg-info/entry_points.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)        9 2023-08-02 13:06:11.000000 grobid_client_python-0.0.6/grobid_client_python.egg-info/requires.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)       14 2023-08-02 13:06:11.000000 grobid_client_python-0.0.6/grobid_client_python.egg-info/top_level.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)       38 2023-08-02 13:06:12.325337 grobid_client_python-0.0.6/setup.cfg
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      662 2023-08-02 13:06:01.000000 grobid_client_python-0.0.6/setup.py
```

### Comparing `grobid_client_python-0.0.5/LICENSE` & `grobid_client_python-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `grobid_client_python-0.0.5/PKG-INFO` & `grobid_client_python-0.0.6/grobid_client_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: grobid_client_python
-Version: 0.0.5
+Name: grobid-client-python
+Version: 0.0.6
 Summary: Simple python client for GROBID REST services
 Home-page: https://github.com/kermitt2/grobid_client_python
 Author: kermitt2
 License: LICENSE
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -96,25 +96,25 @@
 
 Examples:
 
 ```console
 > grobid_client --input ~/tmp/in2 --output ~/tmp/out processFulltextDocument
 ```
 
-This command will process all the PDF files present under the input directory recursively (files with extension `.pdf` only) with the `processFulltextDocument` service of GROBID, and write the resulting XML TEI files under the output directory, reusing the file name with a different file extension (`.tei.xml`), using the default `10` concurrent workers. 
+This command will process all the PDF files present under the input directory recursively (files with extension `.pdf` only) with the `processFulltextDocument` service of GROBID, and write the resulting XML TEI files under the output directory, reusing the file name with a different file extension (`.grobid.tei.xml`), using the default `10` concurrent workers. 
 
 If `--output` is omitted, the resulting XML TEI documents will be produced alongside the PDF in the `--input` directory.
 
 ```console
 > grobid_client --input ~/tmp/in2 --output ~/tmp/out --n 20 processHeaderDocument
 ```
 
-This command will process all the PDF files present in the input directory (files with extension `.pdf` only) with the `processHeaderDocument` service of GROBID, and write the resulting XML TEI files under the output directory, reusing the file name with a different file extension (`.tei.xml`), using `20` concurrent workers. 
+This command will process all the PDF files present in the input directory (files with extension `.pdf` only) with the `processHeaderDocument` service of GROBID, and write the resulting XML TEI files under the output directory, reusing the file name with a different file extension (`.grobid.tei.xml`), using `20` concurrent workers. 
 
-By default if an existing `.tei.xml` file is present in the output directory corresponding to a PDF in the input directory, this PDF will be skipped to avoid reprocessing several times the same PDF. To force the processing of PDF and over-write of existing TEI files, use the parameter `--force`.   
+By default if an existing `.grobid.tei.xml` file is present in the output directory corresponding to a PDF in the input directory, this PDF will be skipped to avoid reprocessing several times the same PDF. To force the processing of PDF and over-write of existing TEI files, use the parameter `--force`.   
 
 `processCitationList` does not take a repertory of PDF as input, but a repertory of `.txt` files, with one reference raw string per line, for example:
 
 ```console
 > grobid_client --input resources/test_txt/ --output resources/test_out/ --n 20 processCitationList
 ```
```

### Comparing `grobid_client_python-0.0.5/grobid_client/client.py` & `grobid_client_python-0.0.6/grobid_client/client.py`

 * *Files identical despite different names*

### Comparing `grobid_client_python-0.0.5/grobid_client/grobid_client.py` & `grobid_client_python-0.0.6/grobid_client/grobid_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,21 +75,21 @@
             print("GROBID server is up and running")
 
     def _output_file_name(self, input_file, input_path, output):
         # we use ntpath here to be sure it will work on Windows too
         if output is not None:
             input_file_name = str(os.path.relpath(os.path.abspath(input_file), input_path))
             filename = os.path.join(
-                output, os.path.splitext(input_file_name)[0] + ".tei.xml"
+                output, os.path.splitext(input_file_name)[0] + ".grobid.tei.xml"
             )
         else:
             input_file_name = ntpath.basename(input_file)
             filename = os.path.join(
                 ntpath.dirname(input_file),
-                os.path.splitext(input_file_name)[0] + ".tei.xml",
+                os.path.splitext(input_file_name)[0] + ".grobid.tei.xml",
             )
 
         return filename
 
     def process(
         self,
         service,
@@ -213,15 +213,15 @@
             filename = self._output_file_name(input_file, input_path, output)
 
             if status != 200 or text is None:
                 print("Processing of", input_file, "failed with error", str(status), ",", text)
                 # writing error file with suffixed error code
                 try:
                     pathlib.Path(os.path.dirname(filename)).mkdir(parents=True, exist_ok=True)
-                    with open(filename.replace(".tei.xml", "_"+str(status)+".txt"), 'w', encoding='utf8') as tei_file:
+                    with open(filename.replace(".grobid.tei.xml", "_"+str(status)+".txt"), 'w', encoding='utf8') as tei_file:
                         if text is not None:
                             tei_file.write(text)
                         else:
                             tei_file.write("")
                 except OSError:
                     print("Writing resulting TEI XML file", filename, "failed")
             else:
```

### Comparing `grobid_client_python-0.0.5/grobid_client_python.egg-info/PKG-INFO` & `grobid_client_python-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: grobid-client-python
-Version: 0.0.5
+Name: grobid_client_python
+Version: 0.0.6
 Summary: Simple python client for GROBID REST services
 Home-page: https://github.com/kermitt2/grobid_client_python
 Author: kermitt2
 License: LICENSE
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -96,25 +96,25 @@
 
 Examples:
 
 ```console
 > grobid_client --input ~/tmp/in2 --output ~/tmp/out processFulltextDocument
 ```
 
-This command will process all the PDF files present under the input directory recursively (files with extension `.pdf` only) with the `processFulltextDocument` service of GROBID, and write the resulting XML TEI files under the output directory, reusing the file name with a different file extension (`.tei.xml`), using the default `10` concurrent workers. 
+This command will process all the PDF files present under the input directory recursively (files with extension `.pdf` only) with the `processFulltextDocument` service of GROBID, and write the resulting XML TEI files under the output directory, reusing the file name with a different file extension (`.grobid.tei.xml`), using the default `10` concurrent workers. 
 
 If `--output` is omitted, the resulting XML TEI documents will be produced alongside the PDF in the `--input` directory.
 
 ```console
 > grobid_client --input ~/tmp/in2 --output ~/tmp/out --n 20 processHeaderDocument
 ```
 
-This command will process all the PDF files present in the input directory (files with extension `.pdf` only) with the `processHeaderDocument` service of GROBID, and write the resulting XML TEI files under the output directory, reusing the file name with a different file extension (`.tei.xml`), using `20` concurrent workers. 
+This command will process all the PDF files present in the input directory (files with extension `.pdf` only) with the `processHeaderDocument` service of GROBID, and write the resulting XML TEI files under the output directory, reusing the file name with a different file extension (`.grobid.tei.xml`), using `20` concurrent workers. 
 
-By default if an existing `.tei.xml` file is present in the output directory corresponding to a PDF in the input directory, this PDF will be skipped to avoid reprocessing several times the same PDF. To force the processing of PDF and over-write of existing TEI files, use the parameter `--force`.   
+By default if an existing `.grobid.tei.xml` file is present in the output directory corresponding to a PDF in the input directory, this PDF will be skipped to avoid reprocessing several times the same PDF. To force the processing of PDF and over-write of existing TEI files, use the parameter `--force`.   
 
 `processCitationList` does not take a repertory of PDF as input, but a repertory of `.txt` files, with one reference raw string per line, for example:
 
 ```console
 > grobid_client --input resources/test_txt/ --output resources/test_out/ --n 20 processCitationList
 ```
```

### Comparing `grobid_client_python-0.0.5/setup.py` & `grobid_client_python-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(name='grobid_client_python',
-      version='0.0.5',
+      version='0.0.6',
       description='Simple python client for GROBID REST services',
       author='kermitt2',
       long_description=open("Readme.md", encoding='utf-8').read(),
       long_description_content_type="text/markdown",
       url="https://github.com/kermitt2/grobid_client_python",
       packages=find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests"]),
       install_requires=['requests'],
```

