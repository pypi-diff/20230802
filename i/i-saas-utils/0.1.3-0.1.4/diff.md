# Comparing `tmp/i_saas_utils-0.1.3.tar.gz` & `tmp/i_saas_utils-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i_saas_utils-0.1.3.tar", max compression
+gzip compressed data, was "i_saas_utils-0.1.4.tar", max compression
```

## Comparing `i_saas_utils-0.1.3.tar` & `i_saas_utils-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     6254 2023-07-28 20:15:16.157658 i_saas_utils-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-07-28 15:49:56.000000 i_saas_utils-0.1.3/i_saas_utils/__init__.py
--rw-r--r--   0        0        0       28 2023-07-29 11:00:00.646286 i_saas_utils-0.1.3/i_saas_utils/ansible/__init__.py
--rw-r--r--   0        0        0      517 2023-07-29 11:08:59.134950 i_saas_utils-0.1.3/i_saas_utils/ansible/ansibl.py
--rw-r--r--   0        0        0       87 2023-08-01 22:29:40.238936 i_saas_utils-0.1.3/i_saas_utils/git/__init__.py
--rw-r--r--   0        0        0      494 2023-08-01 22:31:19.215972 i_saas_utils-0.1.3/i_saas_utils/git/git.py
--rw-r--r--   0        0        0     1334 2023-08-01 22:52:52.330515 i_saas_utils-0.1.3/i_saas_utils/git/git_project.py
--rw-r--r--   0        0        0     1297 2023-08-01 22:48:40.753722 i_saas_utils-0.1.3/i_saas_utils/git/git_repo.py
--rw-r--r--   0        0        0       23 2023-07-29 11:01:01.438716 i_saas_utils-0.1.3/i_saas_utils/k8s/__init__.py
--rw-r--r--   0        0        0      916 2023-07-28 21:36:56.880915 i_saas_utils-0.1.3/i_saas_utils/k8s/kube.py
--rw-r--r--   0        0        0      148 2023-08-02 08:31:41.871839 i_saas_utils-0.1.3/i_saas_utils/saas/__init__.py
--rw-r--r--   0        0        0     3038 2023-08-01 22:33:55.601333 i_saas_utils-0.1.3/i_saas_utils/saas/saas.py
--rw-r--r--   0        0        0       57 2023-07-29 11:01:01.418716 i_saas_utils-0.1.3/i_saas_utils/templates/__init__.py
--rw-r--r--   0        0        0      646 2023-07-29 19:49:55.600690 i_saas_utils-0.1.3/i_saas_utils/templates/render.py
--rw-r--r--   0        0        0       71 2023-07-29 11:01:59.506737 i_saas_utils-0.1.3/i_saas_utils/types/__init__.py
--rw-r--r--   0        0        0      386 2023-08-02 08:31:41.863839 i_saas_utils-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6765 1970-01-01 00:00:00.000000 i_saas_utils-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     6254 2023-07-28 20:15:16.157658 i_saas_utils-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-07-28 15:49:56.000000 i_saas_utils-0.1.4/i_saas_utils/__init__.py
+-rw-r--r--   0        0        0       28 2023-07-29 11:00:00.646286 i_saas_utils-0.1.4/i_saas_utils/ansible/__init__.py
+-rw-r--r--   0        0        0      517 2023-07-29 11:08:59.134950 i_saas_utils-0.1.4/i_saas_utils/ansible/ansibl.py
+-rw-r--r--   0        0        0       87 2023-08-01 22:29:40.238936 i_saas_utils-0.1.4/i_saas_utils/git/__init__.py
+-rw-r--r--   0        0        0      494 2023-08-01 22:31:19.215972 i_saas_utils-0.1.4/i_saas_utils/git/git.py
+-rw-r--r--   0        0        0     1334 2023-08-01 22:52:52.330515 i_saas_utils-0.1.4/i_saas_utils/git/git_project.py
+-rw-r--r--   0        0        0     1402 2023-08-02 09:50:52.851591 i_saas_utils-0.1.4/i_saas_utils/git/git_repo.py
+-rw-r--r--   0        0        0       23 2023-07-29 11:01:01.438716 i_saas_utils-0.1.4/i_saas_utils/k8s/__init__.py
+-rw-r--r--   0        0        0      916 2023-07-28 21:36:56.880915 i_saas_utils-0.1.4/i_saas_utils/k8s/kube.py
+-rw-r--r--   0        0        0      148 2023-08-02 08:31:41.871839 i_saas_utils-0.1.4/i_saas_utils/saas/__init__.py
+-rw-r--r--   0        0        0     3222 2023-08-02 09:50:03.799033 i_saas_utils-0.1.4/i_saas_utils/saas/saas.py
+-rw-r--r--   0        0        0       57 2023-07-29 11:01:01.418716 i_saas_utils-0.1.4/i_saas_utils/templates/__init__.py
+-rw-r--r--   0        0        0      646 2023-07-29 19:49:55.600690 i_saas_utils-0.1.4/i_saas_utils/templates/render.py
+-rw-r--r--   0        0        0       92 2023-08-02 09:32:23.015286 i_saas_utils-0.1.4/i_saas_utils/types/__init__.py
+-rw-r--r--   0        0        0      386 2023-08-02 10:02:38.993313 i_saas_utils-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6765 1970-01-01 00:00:00.000000 i_saas_utils-0.1.4/PKG-INFO
```

### Comparing `i_saas_utils-0.1.3/README.md` & `i_saas_utils-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `i_saas_utils-0.1.3/i_saas_utils/ansible/ansibl.py` & `i_saas_utils-0.1.4/i_saas_utils/ansible/ansibl.py`

 * *Files identical despite different names*

### Comparing `i_saas_utils-0.1.3/i_saas_utils/git/git_project.py` & `i_saas_utils-0.1.4/i_saas_utils/git/git_project.py`

 * *Files identical despite different names*

### Comparing `i_saas_utils-0.1.3/i_saas_utils/git/git_repo.py` & `i_saas_utils-0.1.4/i_saas_utils/git/git_repo.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,18 +25,20 @@
         self,
     ):
         self.repo.git.push("--set-upstream", "origin", self.repo.active_branch)
 
     def create_mr(
         self,
         title: str,
-        source_branch: str,
+        source_branch: str | None = None,
         description: str = "",
         target_branch: str | None = None,
     ):
+        if source_branch is None:
+            source_branch = self.repo.active_branch.name
         if target_branch is None:
             target_branch = self.default_branch
 
         return self.project.mergerequests.create(
             {
                 "source_branch": source_branch,
                 "target_branch": target_branch,
```

### Comparing `i_saas_utils-0.1.3/i_saas_utils/k8s/kube.py` & `i_saas_utils-0.1.4/i_saas_utils/k8s/kube.py`

 * *Files identical despite different names*

### Comparing `i_saas_utils-0.1.3/i_saas_utils/saas/saas.py` & `i_saas_utils-0.1.4/i_saas_utils/saas/saas.py`

 * *Files 5% similar despite different names*

```diff
@@ -105,7 +105,13 @@
             chat_id = self.default_chat_id
 
         payload = {"chat_id": chat_id, "text": message}
         response = requests.post(self.url, data=payload)
 
         if response.status_code != 200:
             raise Exception(f"Can't send notify - {response.text}")
+
+
+def generate_service_name(
+    namespace: str = "", env: str = "", type: str = "", uniq_name: str = ""
+):
+    return "-".join(filter(lambda x: x, [namespace, uniq_name, type, env]))
```

### Comparing `i_saas_utils-0.1.3/i_saas_utils/templates/render.py` & `i_saas_utils-0.1.4/i_saas_utils/templates/render.py`

 * *Files identical despite different names*

### Comparing `i_saas_utils-0.1.3/PKG-INFO` & `i_saas_utils-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i-saas-utils
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Fedorov Stepan
 Author-email: fedorov.stepan2@wb.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dnspython (>=2.4.1,<3.0.0)
```

