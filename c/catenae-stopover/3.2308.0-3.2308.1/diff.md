# Comparing `tmp/catenae_stopover-3.2308.0-py3-none-any.whl.zip` & `tmp/catenae_stopover-3.2308.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 9340 bytes, number of entries: 12
--rw-r--r--  2.0 unx     2088 b- defN 23-Aug-02 17:07 catenae/__init__.py
--rw-r--r--  2.0 unx    18068 b- defN 23-Aug-02 17:46 catenae/catenae.py
+Zip file size: 9336 bytes, number of entries: 12
+-rw-r--r--  2.0 unx     2088 b- defN 23-Aug-02 18:07 catenae/__init__.py
+-rw-r--r--  2.0 unx    18057 b- defN 23-Aug-02 18:07 catenae/catenae.py
 -rw-r--r--  2.0 unx      390 b- defN 23-Aug-02 17:07 catenae/errors.py
 -rw-r--r--  2.0 unx      636 b- defN 23-Aug-02 17:00 catenae/health.py
 -rw-r--r--  2.0 unx      568 b- defN 23-Aug-02 17:19 catenae/logger.py
 -rw-r--r--  2.0 unx     2096 b- defN 23-Aug-02 17:02 catenae/queue.py
 -rw-r--r--  2.0 unx     2027 b- defN 23-Aug-02 17:08 catenae/threading.py
 -rw-r--r--  2.0 unx     1060 b- defN 23-Aug-02 17:06 catenae/utils.py
--rw-r--r--  2.0 unx      824 b- defN 23-Aug-02 17:52 catenae_stopover-3.2308.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-02 17:52 catenae_stopover-3.2308.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Aug-02 17:52 catenae_stopover-3.2308.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      938 b- defN 23-Aug-02 17:52 catenae_stopover-3.2308.0.dist-info/RECORD
-12 files, 28795 bytes uncompressed, 7774 bytes compressed:  73.0%
+-rw-r--r--  2.0 unx      824 b- defN 23-Aug-02 18:10 catenae_stopover-3.2308.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-02 18:10 catenae_stopover-3.2308.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Aug-02 18:10 catenae_stopover-3.2308.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      938 b- defN 23-Aug-02 18:10 catenae_stopover-3.2308.1.dist-info/RECORD
+12 files, 28784 bytes uncompressed, 7770 bytes compressed:  73.0%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: catenae/threading.py
 Comment: 
 
 Filename: catenae/utils.py
 Comment: 
 
-Filename: catenae_stopover-3.2308.0.dist-info/METADATA
+Filename: catenae_stopover-3.2308.1.dist-info/METADATA
 Comment: 
 
-Filename: catenae_stopover-3.2308.0.dist-info/WHEEL
+Filename: catenae_stopover-3.2308.1.dist-info/WHEEL
 Comment: 
 
-Filename: catenae_stopover-3.2308.0.dist-info/top_level.txt
+Filename: catenae_stopover-3.2308.1.dist-info/top_level.txt
 Comment: 
 
-Filename: catenae_stopover-3.2308.0.dist-info/RECORD
+Filename: catenae_stopover-3.2308.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## catenae/__init__.py

```diff
@@ -12,8 +12,8 @@
     '    ◼◼◼              ◼◼◼    ◼◼◼         ◼◼       ◼◼◼               ◼◼◼ ◼◼◼   ◼◼◼       ◼◼◼    ◼◼◼      ◼◼◼             \n'  # noqa: E501
     '  ◼◼◼               ◼◼◼      ◼◼◼        ◼◼     ◼◼◼◼◼◼◼◼◼◼◼◼◼◼◼◼◼◼  ◼◼◼  ◼◼◼  ◼◼◼      ◼◼◼      ◼◼◼   ◼◼◼◼◼◼◼◼◼◼◼◼◼◼◼◼◼◼\n'  # noqa: E501
     '    ◼◼◼            ◼◼◼        ◼◼◼       ◼◼       ◼◼◼               ◼◼◼    ◼◼ ◼◼◼     ◼◼◼        ◼◼◼    ◼◼◼             \n'  # noqa: E501
     '      ◼◼◼         ◼◼◼          ◼◼◼      ◼◼         ◼◼◼             ◼◼◼     ◼◼◼◼◼    ◼◼◼          ◼◼◼     ◼◼◼           \n'  # noqa: E501
     '        ◼◼◼      ◼◼◼            ◼◼◼     ◼◼           ◼◼◼           ◼◼◼      ◼◼◼◼   ◼◼◼            ◼◼◼      ◼◼◼         \n'  # noqa: E501
     '          ◼◼◼   ◼◼◼              ◼◼◼    ◼◼             ◼◼◼         ◼◼◼       ◼◼◼  ◼◼◼              ◼◼◼       ◼◼◼       \n'  # noqa: E501
 )
-__version__ = '3.2308.0'
+__version__ = '3.2308.1'
```

## catenae/catenae.py

```diff
@@ -263,24 +263,24 @@
     ):
         with self._locks['start_stop']:
             if self._started:
                 return
 
         if not startup_text:
             print(catenae.text_logo)
+        else:
+            self.logger.log(startup_text)
+
         self.logger.log(f'catenae  v{catenae.__version__}')
         self.logger.log(f'stopover v{stopover.__version__}')
 
         self.logger.log(
             f'configuration:\n{utils.dump_dict_pretty(self._config)}'
         )
 
-        if startup_text:
-            self.logger.log(startup_text)
-
         with self._locks['start_stop']:
             self._started = True
 
         if setup_kwargs is None:
             setup_kwargs = {}
         self.setup(**setup_kwargs)
```

## Comparing `catenae_stopover-3.2308.0.dist-info/METADATA` & `catenae_stopover-3.2308.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catenae-stopover
-Version: 3.2308.0
+Version: 3.2308.1
 Summary: Catenae 3 – Microservices Framework for Stopover
 Home-page: https://github.com/catenae
 Author: Rodrigo Martínez
 Author-email: dev@brunneis.com
 License: GNU General Public License v3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

## Comparing `catenae_stopover-3.2308.0.dist-info/RECORD` & `catenae_stopover-3.2308.1.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-catenae/__init__.py,sha256=jCF0TZaWX1M_yCDT-4Wdgk0nFVxmnhzoB4zZfAUg7II,2088
-catenae/catenae.py,sha256=h0z_AbgECOfU-J-PboK-ATsp_5R3arfLMZWm5MUfZxk,18068
+catenae/__init__.py,sha256=-PyRN_7ApE4x5oqSbptB3j1hhNCk2Cq_C9-ZxOmmyRI,2088
+catenae/catenae.py,sha256=NyQR0mw68CS2sgVuw7jwkRAVMtDAJDp7_Lv8ezN2u04,18057
 catenae/errors.py,sha256=FvbeToyM4f07ZgJe0rRsuNBs-TR5O7V0bh-qCL29BSs,390
 catenae/health.py,sha256=EznwORvPvG-HXXgCXDkC57wydpkwNgZdvjs5557le6I,636
 catenae/logger.py,sha256=ik9q4oslzt8DZzHUSj1rPGMiKVHjFslJ7W0WigdhgaQ,568
 catenae/queue.py,sha256=qpEP2wy2icStRdKqHmN9fQxxLDRNcVpybHLXmFKGZ1k,2096
 catenae/threading.py,sha256=4HW-WyCL4H5gCNWSErn7gqdeRSW337i8989S6nfzVGs,2027
 catenae/utils.py,sha256=HYSNgDxx8WEAomYSjizutAZIyvi5do6XUYoivyAPVJk,1060
-catenae_stopover-3.2308.0.dist-info/METADATA,sha256=pWiJG11Sa6IfOs2HjXoGq_KUzo24yTFMMYETfaFnzQQ,824
-catenae_stopover-3.2308.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-catenae_stopover-3.2308.0.dist-info/top_level.txt,sha256=8E6E0SqL9fHRQOOIaHVm5xJyTIBR5BqQiu04oOmV2YQ,8
-catenae_stopover-3.2308.0.dist-info/RECORD,,
+catenae_stopover-3.2308.1.dist-info/METADATA,sha256=NN7vPqvq8At8_vkU_Ywqf553QYm7QahhyJ7CEZU2aac,824
+catenae_stopover-3.2308.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+catenae_stopover-3.2308.1.dist-info/top_level.txt,sha256=8E6E0SqL9fHRQOOIaHVm5xJyTIBR5BqQiu04oOmV2YQ,8
+catenae_stopover-3.2308.1.dist-info/RECORD,,
```

