# Comparing `tmp/sentenai-1.6.5.0.tar.gz` & `tmp/sentenai-1.6.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sentenai-1.6.5.0.tar", last modified: Wed Jul 19 20:12:48 2023, max compression
+gzip compressed data, was "dist/sentenai-1.6.5.1.tar", last modified: Wed Aug  2 19:52:16 2023, max compression
```

## Comparing `sentenai-1.6.5.0.tar` & `sentenai-1.6.5.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-07-19 20:12:48.000000 sentenai-1.6.5.0/
--rw-r--r--   0 xnomagichash   (501) staff       (20)      598 2021-12-01 20:18:24.000000 sentenai-1.6.5.0/.coveragerc
--rw-r--r--   0 xnomagichash   (501) staff       (20)       57 2021-12-01 20:18:24.000000 sentenai-1.6.5.0/.editorconfig
--rw-r--r--   0 xnomagichash   (501) staff       (20)     1115 2022-10-20 02:44:17.000000 sentenai-1.6.5.0/.gitignore
--rw-r--r--   0 xnomagichash   (501) staff       (20)      190 2021-12-01 20:18:24.000000 sentenai-1.6.5.0/.travis.yml
--rw-r--r--   0 xnomagichash   (501) staff       (20)     1514 2021-12-01 20:18:24.000000 sentenai-1.6.5.0/LICENSE
--rw-r--r--   0 xnomagichash   (501) staff       (20)      193 2021-12-01 20:18:24.000000 sentenai-1.6.5.0/Makefile
--rw-r--r--   0 xnomagichash   (501) staff       (20)      670 2023-07-19 20:12:48.000000 sentenai-1.6.5.0/PKG-INFO
--rw-r--r--   0 xnomagichash   (501) staff       (20)      781 2021-12-01 20:18:24.000000 sentenai-1.6.5.0/README.md
--rw-r--r--   0 xnomagichash   (501) staff       (20)      141 2021-12-01 20:18:24.000000 sentenai-1.6.5.0/requirements.txt
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-07-19 20:12:48.000000 sentenai-1.6.5.0/sentenai/
--rw-r--r--   0 xnomagichash   (501) staff       (20)    10058 2023-07-19 20:09:35.000000 sentenai-1.6.5.0/sentenai/__init__.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     9678 2023-06-15 14:40:26.000000 sentenai-1.6.5.0/sentenai/api.py
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-07-19 20:12:48.000000 sentenai-1.6.5.0/sentenai/stream/
--rw-r--r--   0 xnomagichash   (501) staff       (20)       59 2023-05-04 20:20:46.000000 sentenai-1.6.5.0/sentenai/stream/__init__.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     5141 2022-03-25 18:39:40.000000 sentenai-1.6.5.0/sentenai/stream/events.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     2284 2023-06-20 01:41:51.000000 sentenai-1.6.5.0/sentenai/stream/metadata.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)    24342 2023-07-19 20:11:34.000000 sentenai-1.6.5.0/sentenai/stream/streams.py
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-07-19 20:12:48.000000 sentenai-1.6.5.0/sentenai/tests/
--rw-r--r--   0 xnomagichash   (501) staff       (20)        0 2021-12-01 20:18:24.000000 sentenai-1.6.5.0/sentenai/tests/__init__.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)      468 2021-12-01 20:18:24.000000 sentenai-1.6.5.0/sentenai/tests/conftest.py
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-07-19 20:12:48.000000 sentenai-1.6.5.0/sentenai/tests/streams/
--rw-r--r--   0 xnomagichash   (501) staff       (20)        0 2021-12-01 20:18:24.000000 sentenai-1.6.5.0/sentenai/tests/streams/__init__.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)        0 2021-12-01 20:18:24.000000 sentenai-1.6.5.0/sentenai/tests/streams/__init__.py-e
--rw-r--r--   0 xnomagichash   (501) staff       (20)      924 2021-12-01 20:18:24.000000 sentenai-1.6.5.0/sentenai/tests/streams/test_stream.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)      924 2021-12-01 20:18:24.000000 sentenai-1.6.5.0/sentenai/tests/streams/test_stream.py-e
--rw-r--r--   0 xnomagichash   (501) staff       (20)      231 2021-12-01 20:18:24.000000 sentenai-1.6.5.0/sentenai/tests/test_client.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     4032 2021-12-01 20:18:24.000000 sentenai-1.6.5.0/sentenai/tests/test_events.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     1289 2021-12-01 20:18:24.000000 sentenai-1.6.5.0/sentenai/tests/test_fields.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)      543 2021-12-01 20:18:24.000000 sentenai-1.6.5.0/sentenai/tests/test_streams.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     1357 2021-12-01 20:18:24.000000 sentenai-1.6.5.0/sentenai/tests/test_views.py
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-07-19 20:12:48.000000 sentenai-1.6.5.0/sentenai.egg-info/
--rw-r--r--   0 xnomagichash   (501) staff       (20)      670 2023-07-19 20:12:47.000000 sentenai-1.6.5.0/sentenai.egg-info/PKG-INFO
--rw-r--r--   0 xnomagichash   (501) staff       (20)      926 2023-07-19 20:12:48.000000 sentenai-1.6.5.0/sentenai.egg-info/SOURCES.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)        1 2023-07-19 20:12:47.000000 sentenai-1.6.5.0/sentenai.egg-info/dependency_links.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)       68 2023-07-19 20:12:48.000000 sentenai-1.6.5.0/sentenai.egg-info/requires.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)        9 2023-07-19 20:12:48.000000 sentenai-1.6.5.0/sentenai.egg-info/top_level.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)       79 2023-07-19 20:12:48.000000 sentenai-1.6.5.0/setup.cfg
--rw-r--r--   0 xnomagichash   (501) staff       (20)      980 2023-07-19 20:11:48.000000 sentenai-1.6.5.0/setup.py
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-07-19 20:12:48.000000 sentenai-1.6.5.0/tests/
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-07-19 20:12:48.000000 sentenai-1.6.5.0/tests/flare/
--rw-r--r--   0 xnomagichash   (501) staff       (20)    16087 2021-12-01 20:18:24.000000 sentenai-1.6.5.0/tests/flare/test_ast.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)      448 2021-12-01 20:18:24.000000 sentenai-1.6.5.0/tests/flare/test_merge.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     6372 2021-12-01 20:18:24.000000 sentenai-1.6.5.0/tests/flare/test_queries.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     1954 2021-12-01 20:18:24.000000 sentenai-1.6.5.0/tests/flare/test_stream_construction.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     5702 2021-12-01 20:18:24.000000 sentenai-1.6.5.0/tests/test_api.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)      386 2021-12-01 20:18:24.000000 sentenai-1.6.5.0/tests/test_utils.py
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-08-02 19:52:16.000000 sentenai-1.6.5.1/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      598 2021-12-01 20:18:24.000000 sentenai-1.6.5.1/.coveragerc
+-rw-r--r--   0 xnomagichash   (501) staff       (20)       57 2021-12-01 20:18:24.000000 sentenai-1.6.5.1/.editorconfig
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     1115 2022-10-20 02:44:17.000000 sentenai-1.6.5.1/.gitignore
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      190 2021-12-01 20:18:24.000000 sentenai-1.6.5.1/.travis.yml
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     1514 2021-12-01 20:18:24.000000 sentenai-1.6.5.1/LICENSE
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      193 2021-12-01 20:18:24.000000 sentenai-1.6.5.1/Makefile
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      670 2023-08-02 19:52:16.000000 sentenai-1.6.5.1/PKG-INFO
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      781 2021-12-01 20:18:24.000000 sentenai-1.6.5.1/README.md
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      141 2021-12-01 20:18:24.000000 sentenai-1.6.5.1/requirements.txt
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-08-02 19:52:16.000000 sentenai-1.6.5.1/sentenai/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)    10837 2023-07-20 20:49:40.000000 sentenai-1.6.5.1/sentenai/__init__.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     9678 2023-06-15 14:40:26.000000 sentenai-1.6.5.1/sentenai/api.py
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-08-02 19:52:16.000000 sentenai-1.6.5.1/sentenai/stream/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)       59 2023-05-04 20:20:46.000000 sentenai-1.6.5.1/sentenai/stream/__init__.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     5141 2022-03-25 18:39:40.000000 sentenai-1.6.5.1/sentenai/stream/events.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     2284 2023-06-20 01:41:51.000000 sentenai-1.6.5.1/sentenai/stream/metadata.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)    24507 2023-08-02 14:10:46.000000 sentenai-1.6.5.1/sentenai/stream/streams.py
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-08-02 19:52:16.000000 sentenai-1.6.5.1/sentenai/tests/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)        0 2021-12-01 20:18:24.000000 sentenai-1.6.5.1/sentenai/tests/__init__.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      468 2021-12-01 20:18:24.000000 sentenai-1.6.5.1/sentenai/tests/conftest.py
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-08-02 19:52:16.000000 sentenai-1.6.5.1/sentenai/tests/streams/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)        0 2021-12-01 20:18:24.000000 sentenai-1.6.5.1/sentenai/tests/streams/__init__.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)        0 2021-12-01 20:18:24.000000 sentenai-1.6.5.1/sentenai/tests/streams/__init__.py-e
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      924 2021-12-01 20:18:24.000000 sentenai-1.6.5.1/sentenai/tests/streams/test_stream.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      924 2021-12-01 20:18:24.000000 sentenai-1.6.5.1/sentenai/tests/streams/test_stream.py-e
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      231 2021-12-01 20:18:24.000000 sentenai-1.6.5.1/sentenai/tests/test_client.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     4032 2021-12-01 20:18:24.000000 sentenai-1.6.5.1/sentenai/tests/test_events.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     1289 2021-12-01 20:18:24.000000 sentenai-1.6.5.1/sentenai/tests/test_fields.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      543 2021-12-01 20:18:24.000000 sentenai-1.6.5.1/sentenai/tests/test_streams.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     1357 2021-12-01 20:18:24.000000 sentenai-1.6.5.1/sentenai/tests/test_views.py
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-08-02 19:52:16.000000 sentenai-1.6.5.1/sentenai.egg-info/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      670 2023-08-02 19:52:16.000000 sentenai-1.6.5.1/sentenai.egg-info/PKG-INFO
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      926 2023-08-02 19:52:16.000000 sentenai-1.6.5.1/sentenai.egg-info/SOURCES.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)        1 2023-08-02 19:52:16.000000 sentenai-1.6.5.1/sentenai.egg-info/dependency_links.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)       68 2023-08-02 19:52:16.000000 sentenai-1.6.5.1/sentenai.egg-info/requires.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)        9 2023-08-02 19:52:16.000000 sentenai-1.6.5.1/sentenai.egg-info/top_level.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)       79 2023-08-02 19:52:16.000000 sentenai-1.6.5.1/setup.cfg
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      980 2023-08-02 19:52:07.000000 sentenai-1.6.5.1/setup.py
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-08-02 19:52:16.000000 sentenai-1.6.5.1/tests/
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-08-02 19:52:16.000000 sentenai-1.6.5.1/tests/flare/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)    16087 2021-12-01 20:18:24.000000 sentenai-1.6.5.1/tests/flare/test_ast.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      448 2021-12-01 20:18:24.000000 sentenai-1.6.5.1/tests/flare/test_merge.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     6372 2021-12-01 20:18:24.000000 sentenai-1.6.5.1/tests/flare/test_queries.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     1954 2021-12-01 20:18:24.000000 sentenai-1.6.5.1/tests/flare/test_stream_construction.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     5702 2021-12-01 20:18:24.000000 sentenai-1.6.5.1/tests/test_api.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      386 2021-12-01 20:18:24.000000 sentenai-1.6.5.1/tests/test_utils.py
```

### Comparing `sentenai-1.6.5.0/.coveragerc` & `sentenai-1.6.5.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.5.0/.gitignore` & `sentenai-1.6.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.5.0/LICENSE` & `sentenai-1.6.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.5.0/PKG-INFO` & `sentenai-1.6.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentenai
-Version: 1.6.5.0
+Version: 1.6.5.1
 Summary: Client library for Sentenai
 Home-page: https://github.com/sentenai/py-sentenai
 Author: Sentenai, Inc.
 Author-email: info@sentenai.com
 License: BSD
 Keywords: sentenai cloud sensor database
 Platform: UNKNOWN
```

### Comparing `sentenai-1.6.5.0/README.md` & `sentenai-1.6.5.1/README.md`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.5.0/sentenai/__init__.py` & `sentenai-1.6.5.1/sentenai/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,28 +204,42 @@
                 else:
                     resp = self._post(json=f'({tspl}) when {self._when}', params=params, headers={'Accept': 'application/cbor'})
 
                     
                 t = resp.headers['type']
                 if resp.headers['content-type'] == 'application/cbor':
                     o = 0
+                    hasOrigin = False
                     if 'origin' in resp.headers:
                         o = int(np.datetime64(resp.headers['origin'][:-1], 'ns').astype(int))
+                        hasOrigin = True
                     d = cbor2.loads(resp.content)
                     data = []
-                    if t != 'event':
-                        for evt in d:
-                            ts =  np.datetime64(o + evt[0], 'ns')
-                            end = np.datetime64(o + evt[0] + evt[1], 'ns')
-                            data.append({'start': ts, 'end': end, 'value': evt[2]})
+                    if hasOrigin:
+                        if t != 'event':
+                            for evt in d:
+                                ts =  np.datetime64(o + evt[0], 'ns')
+                                end = np.datetime64(o + evt[0] + evt[1], 'ns')
+                                data.append({'start': ts, 'end': end, 'value': evt[2]})
+                        else:
+                            for evt in d:
+                                ts =  np.datetime64(o + evt[0], 'ns')
+                                end = np.datetime64(o + evt[0] + evt[1], 'ns')
+                                data.append({'start': ts, 'end': end})
                     else:
-                        for evt in d:
-                            ts =  np.datetime64(o + evt[0], 'ns')
-                            end = np.datetime64(o + evt[0] + evt[1], 'ns')
-                            data.append({'start': ts, 'end': end})
+                        if t != 'event':
+                            for evt in d:
+                                ts =  np.timedelta64(evt[0], 'ns')
+                                end = np.timedelta64(evt[0] + evt[1], 'ns')
+                                data.append({'start': ts, 'end': end, 'value': evt[2]})
+                        else:
+                            for evt in d:
+                                ts =  np.timedelta64(evt[0], 'ns')
+                                end = np.timedelta64(evt[0] + evt[1], 'ns')
+                                data.append({'start': ts, 'end': end})
                     results.append(data)
                 else:
                     data = resp.json()
                     if isinstance(data, list):
                         for evt in data:
                             if type(evt['start']) is int:
                                 evt['start'] = np.timedelta64(evt['start'], 'ns')
```

### Comparing `sentenai-1.6.5.0/sentenai/api.py` & `sentenai-1.6.5.1/sentenai/api.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.5.0/sentenai/stream/events.py` & `sentenai-1.6.5.1/sentenai/stream/events.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.5.0/sentenai/stream/metadata.py` & `sentenai-1.6.5.1/sentenai/stream/metadata.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.5.0/sentenai/stream/streams.py` & `sentenai-1.6.5.1/sentenai/stream/streams.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,33 +86,36 @@
    
     def items(self):
         return iter([(k, self[k]) for k in self])
 
     def values(self):
         return iter([self[k] for k in self])
 
-    def graph(self, path=None):
+    def graph(self, path=None, limit=-1):
         import treelib
         t = treelib.Tree()
         root = t.create_node(path[-1] if path else self.name, path[-1] if path else self.name, data={})
-        r = self._get("graph", *(path or []))
+        ps = {}
+        if limit >= 0:
+            ps['limit'] = limit
+        r = self._get("graph", *(path or []), params=ps)
         if r.status_code != 200:
             raise SentenaiError("Invalid Response")
         data = r.json()
         for node in sorted(data, key=lambda x: x[0]):
             parent = root
             x = [path[-1] if path else self.name]
             for link in node[0][len(path) - 2 if path else 0:]:
                 x.append(link)
                 nid = "/".join(x)
                 if nid in t:
                     continue
                 else:
                     pid = "/".join(x[:-1]) 
-                    t.create_node(link, nid, parent=pid, data={'type': node[1]})
+                    t.create_node(link, nid, parent=pid, data={'id': node[1], 'type': node[2], 'children': node[3], 'indexes': node[4]})
         return t
 
 
     @property
     def meta(self):
         raise NotImplemented("metadata not implemented on databases.")
         return Metadata(self)
@@ -440,16 +443,16 @@
                 columns = co + [x for x in list(self) if x not in exclude],
                 ).astype({
                     'start': np.dtype('datetime64[ns]'),
                     'end': np.dtype('datetime64[ns]')
                 })
 
 
-    def graph(self):
-        return self._parent.graph(self._path)
+    def graph(self, limit=-1):
+        return self._parent.graph(self._path, limit)
 
     @property
     def source(self):
         r = self._get()
         if r.status_code == 200:
             info = r.json()
             if not info:
```

### Comparing `sentenai-1.6.5.0/sentenai/tests/streams/test_stream.py` & `sentenai-1.6.5.1/sentenai/tests/streams/test_stream.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.5.0/sentenai/tests/streams/test_stream.py-e` & `sentenai-1.6.5.1/sentenai/tests/streams/test_stream.py-e`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.5.0/sentenai/tests/test_events.py` & `sentenai-1.6.5.1/sentenai/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.5.0/sentenai/tests/test_fields.py` & `sentenai-1.6.5.1/sentenai/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.5.0/sentenai/tests/test_streams.py` & `sentenai-1.6.5.1/sentenai/tests/test_streams.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.5.0/sentenai/tests/test_views.py` & `sentenai-1.6.5.1/sentenai/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.5.0/sentenai.egg-info/PKG-INFO` & `sentenai-1.6.5.1/sentenai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentenai
-Version: 1.6.5.0
+Version: 1.6.5.1
 Summary: Client library for Sentenai
 Home-page: https://github.com/sentenai/py-sentenai
 Author: Sentenai, Inc.
 Author-email: info@sentenai.com
 License: BSD
 Keywords: sentenai cloud sensor database
 Platform: UNKNOWN
```

### Comparing `sentenai-1.6.5.0/sentenai.egg-info/SOURCES.txt` & `sentenai-1.6.5.1/sentenai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.5.0/setup.py` & `sentenai-1.6.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='sentenai',
-    version='1.6.5.0',
+    version='1.6.5.1',
     description='Client library for Sentenai',
     long_description="",
     url='https://github.com/sentenai/py-sentenai',
 
     author='Sentenai, Inc.',
     author_email='info@sentenai.com',
```

### Comparing `sentenai-1.6.5.0/tests/flare/test_ast.py` & `sentenai-1.6.5.1/tests/flare/test_ast.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.5.0/tests/flare/test_queries.py` & `sentenai-1.6.5.1/tests/flare/test_queries.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.5.0/tests/flare/test_stream_construction.py` & `sentenai-1.6.5.1/tests/flare/test_stream_construction.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.5.0/tests/test_api.py` & `sentenai-1.6.5.1/tests/test_api.py`

 * *Files identical despite different names*

