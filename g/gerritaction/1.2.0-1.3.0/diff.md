# Comparing `tmp/gerritaction-1.2.0.tar.gz` & `tmp/gerritaction-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gerritaction-1.2.0.tar", last modified: Mon Apr 18 14:25:07 2022, max compression
+gzip compressed data, was "gerritaction-1.3.0.tar", last modified: Wed Aug  2 02:16:26 2023, max compression
```

## Comparing `gerritaction-1.2.0.tar` & `gerritaction-1.3.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 lemonjia  (1000) lemonjia  (1000)        0 2022-04-18 14:25:07.024749 gerritaction-1.2.0/
--rw-rw-r--   0 lemonjia  (1000) lemonjia  (1000)    11357 2022-04-18 14:18:07.000000 gerritaction-1.2.0/LICENSE
--rw-rw-r--   0 lemonjia  (1000) lemonjia  (1000)       69 2022-04-18 14:18:07.000000 gerritaction-1.2.0/MANIFEST.in
--rw-rw-r--   0 lemonjia  (1000) lemonjia  (1000)     3283 2022-04-18 14:25:07.024749 gerritaction-1.2.0/PKG-INFO
--rw-rw-r--   0 lemonjia  (1000) lemonjia  (1000)     2652 2022-04-18 14:21:21.000000 gerritaction-1.2.0/README.md
--rw-rw-r--   0 lemonjia  (1000) lemonjia  (1000)      223 2022-04-18 14:18:07.000000 gerritaction-1.2.0/action.py
-drwxrwxr-x   0 lemonjia  (1000) lemonjia  (1000)        0 2022-04-18 14:25:07.024749 gerritaction-1.2.0/gerritaction/
--rw-rw-r--   0 lemonjia  (1000) lemonjia  (1000)        0 2022-04-18 14:18:07.000000 gerritaction-1.2.0/gerritaction/__init__.py
--rw-rw-r--   0 lemonjia  (1000) lemonjia  (1000)      226 2022-04-18 14:18:07.000000 gerritaction-1.2.0/gerritaction/__version__.py
-drwxrwxr-x   0 lemonjia  (1000) lemonjia  (1000)        0 2022-04-18 14:25:07.024749 gerritaction-1.2.0/gerritaction/action/
--rw-rw-r--   0 lemonjia  (1000) lemonjia  (1000)        0 2022-04-18 14:18:07.000000 gerritaction-1.2.0/gerritaction/action/__init__.py
--rw-rw-r--   0 lemonjia  (1000) lemonjia  (1000)     2895 2022-04-18 14:18:07.000000 gerritaction-1.2.0/gerritaction/action/action.py
-drwxrwxr-x   0 lemonjia  (1000) lemonjia  (1000)        0 2022-04-18 14:25:07.024749 gerritaction-1.2.0/gerritaction/cmd/
--rw-rw-r--   0 lemonjia  (1000) lemonjia  (1000)        0 2022-04-18 14:18:07.000000 gerritaction-1.2.0/gerritaction/cmd/__init__.py
--rw-rw-r--   0 lemonjia  (1000) lemonjia  (1000)     1262 2022-04-18 14:18:07.000000 gerritaction-1.2.0/gerritaction/cmd/argument.py
--rw-rw-r--   0 lemonjia  (1000) lemonjia  (1000)      273 2022-04-18 14:18:07.000000 gerritaction-1.2.0/gerritaction/cmd/banner.py
-drwxrwxr-x   0 lemonjia  (1000) lemonjia  (1000)        0 2022-04-18 14:25:07.024749 gerritaction-1.2.0/gerritaction/config/
--rw-rw-r--   0 lemonjia  (1000) lemonjia  (1000)        0 2022-04-18 14:18:07.000000 gerritaction-1.2.0/gerritaction/config/__init__.py
--rw-rw-r--   0 lemonjia  (1000) lemonjia  (1000)     1799 2022-04-18 14:18:07.000000 gerritaction-1.2.0/gerritaction/config/config.py
-drwxrwxr-x   0 lemonjia  (1000) lemonjia  (1000)        0 2022-04-18 14:25:07.024749 gerritaction-1.2.0/gerritaction/gerrit/
--rw-rw-r--   0 lemonjia  (1000) lemonjia  (1000)        0 2022-04-18 14:18:07.000000 gerritaction-1.2.0/gerritaction/gerrit/__init__.py
--rw-rw-r--   0 lemonjia  (1000) lemonjia  (1000)     8863 2022-04-18 14:18:07.000000 gerritaction-1.2.0/gerritaction/gerrit/gerrit.py
-drwxrwxr-x   0 lemonjia  (1000) lemonjia  (1000)        0 2022-04-18 14:25:07.024749 gerritaction-1.2.0/gerritaction/logger/
--rw-rw-r--   0 lemonjia  (1000) lemonjia  (1000)        0 2022-04-18 14:18:07.000000 gerritaction-1.2.0/gerritaction/logger/__init__.py
--rw-rw-r--   0 lemonjia  (1000) lemonjia  (1000)     1608 2022-04-18 14:22:17.000000 gerritaction-1.2.0/gerritaction/logger/logger.py
--rw-rw-r--   0 lemonjia  (1000) lemonjia  (1000)      877 2022-04-18 14:18:07.000000 gerritaction-1.2.0/gerritaction/main.py
-drwxrwxr-x   0 lemonjia  (1000) lemonjia  (1000)        0 2022-04-18 14:25:07.024749 gerritaction-1.2.0/gerritaction/proto/
--rw-rw-r--   0 lemonjia  (1000) lemonjia  (1000)        0 2022-04-18 14:18:07.000000 gerritaction-1.2.0/gerritaction/proto/__init__.py
--rw-rw-r--   0 lemonjia  (1000) lemonjia  (1000)      351 2022-04-18 14:18:07.000000 gerritaction-1.2.0/gerritaction/proto/proto.py
-drwxrwxr-x   0 lemonjia  (1000) lemonjia  (1000)        0 2022-04-18 14:25:07.024749 gerritaction-1.2.0/gerritaction.egg-info/
--rw-rw-r--   0 lemonjia  (1000) lemonjia  (1000)     3283 2022-04-18 14:25:06.000000 gerritaction-1.2.0/gerritaction.egg-info/PKG-INFO
--rw-rw-r--   0 lemonjia  (1000) lemonjia  (1000)      777 2022-04-18 14:25:06.000000 gerritaction-1.2.0/gerritaction.egg-info/SOURCES.txt
--rw-rw-r--   0 lemonjia  (1000) lemonjia  (1000)        1 2022-04-18 14:25:06.000000 gerritaction-1.2.0/gerritaction.egg-info/dependency_links.txt
--rw-rw-r--   0 lemonjia  (1000) lemonjia  (1000)       56 2022-04-18 14:25:06.000000 gerritaction-1.2.0/gerritaction.egg-info/entry_points.txt
--rw-rw-r--   0 lemonjia  (1000) lemonjia  (1000)        1 2022-04-18 14:25:06.000000 gerritaction-1.2.0/gerritaction.egg-info/not-zip-safe
--rw-rw-r--   0 lemonjia  (1000) lemonjia  (1000)      107 2022-04-18 14:25:06.000000 gerritaction-1.2.0/gerritaction.egg-info/requires.txt
--rw-rw-r--   0 lemonjia  (1000) lemonjia  (1000)       13 2022-04-18 14:25:06.000000 gerritaction-1.2.0/gerritaction.egg-info/top_level.txt
--rw-rw-r--   0 lemonjia  (1000) lemonjia  (1000)       67 2022-04-18 14:25:07.024749 gerritaction-1.2.0/setup.cfg
--rw-rw-r--   0 lemonjia  (1000) lemonjia  (1000)     1470 2022-04-18 14:18:07.000000 gerritaction-1.2.0/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 02:16:26.794526 gerritaction-1.3.0/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11357 2023-08-02 02:08:33.000000 gerritaction-1.3.0/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       69 2023-08-02 02:08:33.000000 gerritaction-1.3.0/MANIFEST.in
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3277 2023-08-02 02:16:26.798526 gerritaction-1.3.0/PKG-INFO
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     2666 2023-08-02 02:13:03.000000 gerritaction-1.3.0/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      223 2023-08-02 02:13:20.000000 gerritaction-1.3.0/action.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 02:16:26.790526 gerritaction-1.3.0/gerritaction/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-08-02 02:13:20.000000 gerritaction-1.3.0/gerritaction/__init__.py
+-rw-r--r--   0 codespace  (1000) codespace  (1000)      226 2023-08-02 02:13:20.000000 gerritaction-1.3.0/gerritaction/__version__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 02:16:26.794526 gerritaction-1.3.0/gerritaction/action/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-08-02 02:13:20.000000 gerritaction-1.3.0/gerritaction/action/__init__.py
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     3121 2023-08-02 02:13:20.000000 gerritaction-1.3.0/gerritaction/action/action.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 02:16:26.794526 gerritaction-1.3.0/gerritaction/cmd/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-08-02 02:13:20.000000 gerritaction-1.3.0/gerritaction/cmd/__init__.py
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     1276 2023-08-02 02:13:20.000000 gerritaction-1.3.0/gerritaction/cmd/argument.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      273 2023-08-02 02:13:20.000000 gerritaction-1.3.0/gerritaction/cmd/banner.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 02:16:26.794526 gerritaction-1.3.0/gerritaction/config/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-08-02 02:13:20.000000 gerritaction-1.3.0/gerritaction/config/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1799 2023-08-02 02:13:20.000000 gerritaction-1.3.0/gerritaction/config/config.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 02:16:26.794526 gerritaction-1.3.0/gerritaction/gerrit/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-08-02 02:13:20.000000 gerritaction-1.3.0/gerritaction/gerrit/__init__.py
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     9545 2023-08-02 02:14:13.000000 gerritaction-1.3.0/gerritaction/gerrit/gerrit.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 02:16:26.794526 gerritaction-1.3.0/gerritaction/logger/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-08-02 02:13:20.000000 gerritaction-1.3.0/gerritaction/logger/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1608 2023-08-02 02:13:20.000000 gerritaction-1.3.0/gerritaction/logger/logger.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      877 2023-08-02 02:13:20.000000 gerritaction-1.3.0/gerritaction/main.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 02:16:26.794526 gerritaction-1.3.0/gerritaction/proto/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-08-02 02:13:20.000000 gerritaction-1.3.0/gerritaction/proto/__init__.py
+-rw-r--r--   0 codespace  (1000) codespace  (1000)      387 2023-08-02 02:13:20.000000 gerritaction-1.3.0/gerritaction/proto/proto.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 02:16:26.790526 gerritaction-1.3.0/gerritaction.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3277 2023-08-02 02:16:26.000000 gerritaction-1.3.0/gerritaction.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      777 2023-08-02 02:16:26.000000 gerritaction-1.3.0/gerritaction.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-08-02 02:16:26.000000 gerritaction-1.3.0/gerritaction.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       56 2023-08-02 02:16:26.000000 gerritaction-1.3.0/gerritaction.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-08-02 02:16:26.000000 gerritaction-1.3.0/gerritaction.egg-info/not-zip-safe
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      107 2023-08-02 02:16:26.000000 gerritaction-1.3.0/gerritaction.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       13 2023-08-02 02:16:26.000000 gerritaction-1.3.0/gerritaction.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       67 2023-08-02 02:16:26.798526 gerritaction-1.3.0/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1470 2023-08-02 02:13:20.000000 gerritaction-1.3.0/setup.py
```

### Comparing `gerritaction-1.2.0/LICENSE` & `gerritaction-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gerritaction-1.2.0/PKG-INFO` & `gerritaction-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: gerritaction
-Version: 1.2.0
+Version: 1.3.0
 Summary: Gerrit Action
 Home-page: https://github.com/craftslab/gerritaction
-Download-URL: https://github.com/craftslab/gerritaction/archive/v1.2.0.tar.gz
+Download-URL: https://github.com/craftslab/gerritaction/archive/v1.3.0.tar.gz
 Author: Jia Jia
 Author-email: angersax@sina.com
 License: Apache-2.0
 Keywords: gerrit,action
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -70,15 +69,15 @@
 Gerrit Action
 
 optional arguments:
   -h, --help            show this help message and exit
   --config-file CONFIG_FILE
                         config file (.yml)
   --gerrit-action GERRIT_ACTION
-                        gerrit action (add-reviewer:account-id,... delete-reviewer:account-id,... add-attention:account-id,... remove-attention:account-id,... approve-change:Code-Review=+2,... submit-change)
+                        gerrit action (add-reviewer:account-id,... delete-reviewer:account-id,... add-attention:account-id,... remove-attention:account-id,... approve-change:Code-Review=+2,... delete-change submit-change)
   --gerrit-query GERRIT_QUERY
                         gerrit query (status:open since:2021-01-01 until:2021-01-02)
   -v, --version         show program's version number and exit
 ```
 
 
 
@@ -105,9 +104,7 @@
 ```
 
 
 
 ## License
 
 Project License can be found [here](LICENSE).
-
-
```

### Comparing `gerritaction-1.2.0/README.md` & `gerritaction-1.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 Gerrit Action
 
 optional arguments:
   -h, --help            show this help message and exit
   --config-file CONFIG_FILE
                         config file (.yml)
   --gerrit-action GERRIT_ACTION
-                        gerrit action (add-reviewer:account-id,... delete-reviewer:account-id,... add-attention:account-id,... remove-attention:account-id,... approve-change:Code-Review=+2,... submit-change)
+                        gerrit action (add-reviewer:account-id,... delete-reviewer:account-id,... add-attention:account-id,... remove-attention:account-id,... approve-change:Code-Review=+2,... delete-change submit-change)
   --gerrit-query GERRIT_QUERY
                         gerrit query (status:open since:2021-01-01 until:2021-01-02)
   -v, --version         show program's version number and exit
 ```
```

### Comparing `gerritaction-1.2.0/gerritaction/action/action.py` & `gerritaction-1.3.0/gerritaction/action/action.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,18 +52,25 @@
         for change in self._changes:
             _ = self._gerrit.approve_change(change, labels)
 
     def _submit_change(self):
         for change in self._changes:
             _ = self._gerrit.submit_change(change)
 
+    def _delete_change(self):
+        for change in self._changes:
+            _ = self._gerrit.delete_change(change)
+
     def run(self):
         for item in self._config.gerrit_action.split(Separator.GROUP):
             if len(item.split(Separator.ACTION)) > 2:
                 raise ActionException("action invalid")
+            if Proto.DELETE_CHANGE in item:
+                self._delete_change()
+                continue
             if Proto.SUBMIT_CHANGE in item:
                 self._submit_change()
                 continue
             action, content = item.split(Separator.ACTION)
             if action == Proto.ADD_REVIEWER:
                 self._add_reviewer(content.split(Separator.CONTENT))
             elif action == Proto.DELETE_REVIEWER:
```

### Comparing `gerritaction-1.2.0/gerritaction/cmd/argument.py` & `gerritaction-1.3.0/gerritaction/cmd/argument.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             help="config file (.yml)",
             required=True,
         )
         self._parser.add_argument(
             "--gerrit-action",
             action="store",
             dest="gerrit_action",
-            help="gerrit action (add-reviewer:account-id,... delete-reviewer:account-id,... add-attention:account-id,... remove-attention:account-id,... approve-change:Code-Review=+2,... submit-change)",
+            help="gerrit action (add-reviewer:account-id,... delete-reviewer:account-id,... add-attention:account-id,... remove-attention:account-id,... approve-change:Code-Review=+2,... delete-change submit-change)",
             required=True,
         )
         self._parser.add_argument(
             "--gerrit-query",
             action="store",
             dest="gerrit_query",
             help="gerrit query (status:open since:2021-01-01 until:2021-01-02)",
```

### Comparing `gerritaction-1.2.0/gerritaction/config/config.py` & `gerritaction-1.3.0/gerritaction/config/config.py`

 * *Files identical despite different names*

### Comparing `gerritaction-1.2.0/gerritaction/gerrit/gerrit.py` & `gerritaction-1.3.0/gerritaction/gerrit/gerrit.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,14 +218,33 @@
             Logger.error(
                 "failed to approve change %s by account %s"
                 % (change["_number"], self._user)
             )
             return None
         return json.loads(response.text.replace(")]}'", ""))
 
+    def delete_change(self, change):
+        if len(self._pass) != 0 and len(self._user) != 0:
+            response = requests.delete(
+                url=self._url + "/changes/" + str(change["_number"]),
+                auth=(self._user, self._pass),
+                json=None,
+            )
+        else:
+            response = requests.delete(
+                url=self._url + "/changes/" + str(change["_number"]),
+                json=None,
+            )
+        if response.status_code != requests.codes.ok:
+            Logger.error(
+                "failed to delete change %s by account %s"
+                % (change["_number"], self._user)
+            )
+        return None
+
     def submit_change(self, change):
         if len(self._pass) != 0 and len(self._user) != 0:
             response = requests.post(
                 url=self._url
                 + "/changes/"
                 + str(change["_number"])
                 + "/revisions/"
```

### Comparing `gerritaction-1.2.0/gerritaction/logger/logger.py` & `gerritaction-1.3.0/gerritaction/logger/logger.py`

 * *Files identical despite different names*

### Comparing `gerritaction-1.2.0/gerritaction/main.py` & `gerritaction-1.3.0/gerritaction/main.py`

 * *Files identical despite different names*

### Comparing `gerritaction-1.2.0/gerritaction.egg-info/PKG-INFO` & `gerritaction-1.3.0/gerritaction.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: gerritaction
-Version: 1.2.0
+Version: 1.3.0
 Summary: Gerrit Action
 Home-page: https://github.com/craftslab/gerritaction
-Download-URL: https://github.com/craftslab/gerritaction/archive/v1.2.0.tar.gz
+Download-URL: https://github.com/craftslab/gerritaction/archive/v1.3.0.tar.gz
 Author: Jia Jia
 Author-email: angersax@sina.com
 License: Apache-2.0
 Keywords: gerrit,action
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -70,15 +69,15 @@
 Gerrit Action
 
 optional arguments:
   -h, --help            show this help message and exit
   --config-file CONFIG_FILE
                         config file (.yml)
   --gerrit-action GERRIT_ACTION
-                        gerrit action (add-reviewer:account-id,... delete-reviewer:account-id,... add-attention:account-id,... remove-attention:account-id,... approve-change:Code-Review=+2,... submit-change)
+                        gerrit action (add-reviewer:account-id,... delete-reviewer:account-id,... add-attention:account-id,... remove-attention:account-id,... approve-change:Code-Review=+2,... delete-change submit-change)
   --gerrit-query GERRIT_QUERY
                         gerrit query (status:open since:2021-01-01 until:2021-01-02)
   -v, --version         show program's version number and exit
 ```
 
 
 
@@ -105,9 +104,7 @@
 ```
 
 
 
 ## License
 
 Project License can be found [here](LICENSE).
-
-
```

### Comparing `gerritaction-1.2.0/gerritaction.egg-info/SOURCES.txt` & `gerritaction-1.3.0/gerritaction.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gerritaction-1.2.0/setup.py` & `gerritaction-1.3.0/setup.py`

 * *Files identical despite different names*

