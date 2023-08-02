# Comparing `tmp/sharepoint_v1_api-0.1.3.tar.gz` & `tmp/sharepoint_v1_api-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharepoint_v1_api-0.1.3.tar", last modified: Thu Jan 12 09:45:34 2023, max compression
+gzip compressed data, was "sharepoint_v1_api-0.1.4.tar", last modified: Wed Aug  2 14:23:55 2023, max compression
```

## Comparing `sharepoint_v1_api-0.1.3.tar` & `sharepoint_v1_api-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 abkl      (1000) abkl      (1000)        0 2023-01-12 09:45:34.749477 sharepoint_v1_api-0.1.3/
--rw-r--r--   0 abkl      (1000) abkl      (1000)     1073 2022-11-04 13:15:48.000000 sharepoint_v1_api-0.1.3/LICENSE
--rw-r--r--   0 abkl      (1000) abkl      (1000)       26 2022-11-04 13:15:48.000000 sharepoint_v1_api-0.1.3/MANIFEST.in
--rw-r--r--   0 abkl      (1000) abkl      (1000)     3202 2023-01-12 09:45:34.749477 sharepoint_v1_api-0.1.3/PKG-INFO
--rw-r--r--   0 abkl      (1000) abkl      (1000)     2076 2023-01-12 09:45:12.000000 sharepoint_v1_api-0.1.3/README.md
--rw-r--r--   0 abkl      (1000) abkl      (1000)      103 2022-11-04 13:15:48.000000 sharepoint_v1_api-0.1.3/pyproject.toml
--rw-r--r--   0 abkl      (1000) abkl      (1000)       38 2023-01-12 09:45:34.749477 sharepoint_v1_api-0.1.3/setup.cfg
--rw-r--r--   0 abkl      (1000) abkl      (1000)      780 2023-01-12 09:45:13.000000 sharepoint_v1_api-0.1.3/setup.py
-drwxr-xr-x   0 abkl      (1000) abkl      (1000)        0 2023-01-12 09:45:34.749477 sharepoint_v1_api-0.1.3/sharepoint_api/
--rw-r--r--   0 abkl      (1000) abkl      (1000)    25824 2023-01-10 09:48:41.000000 sharepoint_v1_api-0.1.3/sharepoint_api/SharePointAPI.py
--rw-r--r--   0 abkl      (1000) abkl      (1000)     3227 2023-01-11 13:07:22.000000 sharepoint_v1_api-0.1.3/sharepoint_api/SharePointList.py
--rw-r--r--   0 abkl      (1000) abkl      (1000)     5008 2023-01-10 08:50:33.000000 sharepoint_v1_api-0.1.3/sharepoint_api/SharePointListItem.py
--rw-r--r--   0 abkl      (1000) abkl      (1000)     1605 2022-11-04 13:15:48.000000 sharepoint_v1_api-0.1.3/sharepoint_api/SharePointLists.py
--rw-r--r--   0 abkl      (1000) abkl      (1000)     1249 2022-11-04 13:15:48.000000 sharepoint_v1_api-0.1.3/sharepoint_api/SharePointTimeRegistration.py
--rw-r--r--   0 abkl      (1000) abkl      (1000)      721 2022-11-04 13:15:48.000000 sharepoint_v1_api-0.1.3/sharepoint_api/SharePointUser.py
--rw-r--r--   0 abkl      (1000) abkl      (1000)      672 2022-11-04 13:15:48.000000 sharepoint_v1_api-0.1.3/sharepoint_api/SharePointUserList.py
--rw-r--r--   0 abkl      (1000) abkl      (1000)       40 2022-11-04 13:15:48.000000 sharepoint_v1_api-0.1.3/sharepoint_api/__init__.py
-drwxr-xr-x   0 abkl      (1000) abkl      (1000)        0 2023-01-12 09:45:34.749477 sharepoint_v1_api-0.1.3/sharepoint_v1_api.egg-info/
--rw-r--r--   0 abkl      (1000) abkl      (1000)     3202 2023-01-12 09:45:34.000000 sharepoint_v1_api-0.1.3/sharepoint_v1_api.egg-info/PKG-INFO
--rw-r--r--   0 abkl      (1000) abkl      (1000)      535 2023-01-12 09:45:34.000000 sharepoint_v1_api-0.1.3/sharepoint_v1_api.egg-info/SOURCES.txt
--rw-r--r--   0 abkl      (1000) abkl      (1000)        1 2023-01-12 09:45:34.000000 sharepoint_v1_api-0.1.3/sharepoint_v1_api.egg-info/dependency_links.txt
--rw-r--r--   0 abkl      (1000) abkl      (1000)       23 2023-01-12 09:45:34.000000 sharepoint_v1_api-0.1.3/sharepoint_v1_api.egg-info/requires.txt
--rw-r--r--   0 abkl      (1000) abkl      (1000)       15 2023-01-12 09:45:34.000000 sharepoint_v1_api-0.1.3/sharepoint_v1_api.egg-info/top_level.txt
+drwxr-xr-x   0 abkl      (1000) abkl      (1000)        0 2023-08-02 14:23:55.942253 sharepoint_v1_api-0.1.4/
+-rw-r--r--   0 abkl      (1000) abkl      (1000)     1073 2022-11-04 13:15:48.000000 sharepoint_v1_api-0.1.4/LICENSE
+-rw-r--r--   0 abkl      (1000) abkl      (1000)       26 2022-11-04 13:15:48.000000 sharepoint_v1_api-0.1.4/MANIFEST.in
+-rw-r--r--   0 abkl      (1000) abkl      (1000)     2518 2023-08-02 14:23:55.942253 sharepoint_v1_api-0.1.4/PKG-INFO
+-rw-r--r--   0 abkl      (1000) abkl      (1000)     2076 2023-08-02 13:46:59.000000 sharepoint_v1_api-0.1.4/README.md
+-rw-r--r--   0 abkl      (1000) abkl      (1000)      103 2022-11-04 13:15:48.000000 sharepoint_v1_api-0.1.4/pyproject.toml
+-rw-r--r--   0 abkl      (1000) abkl      (1000)       38 2023-08-02 14:23:55.942253 sharepoint_v1_api-0.1.4/setup.cfg
+-rw-r--r--   0 abkl      (1000) abkl      (1000)      780 2023-08-02 13:46:40.000000 sharepoint_v1_api-0.1.4/setup.py
+drwxr-xr-x   0 abkl      (1000) abkl      (1000)        0 2023-08-02 14:23:55.942253 sharepoint_v1_api-0.1.4/sharepoint_api/
+-rw-r--r--   0 abkl      (1000) abkl      (1000)    27076 2023-08-02 14:14:30.000000 sharepoint_v1_api-0.1.4/sharepoint_api/SharePointAPI.py
+-rw-r--r--   0 abkl      (1000) abkl      (1000)     3352 2023-08-02 14:02:03.000000 sharepoint_v1_api-0.1.4/sharepoint_api/SharePointList.py
+-rw-r--r--   0 abkl      (1000) abkl      (1000)     5146 2023-07-31 11:24:48.000000 sharepoint_v1_api-0.1.4/sharepoint_api/SharePointListItem.py
+-rw-r--r--   0 abkl      (1000) abkl      (1000)     1605 2022-11-04 13:15:48.000000 sharepoint_v1_api-0.1.4/sharepoint_api/SharePointLists.py
+-rw-r--r--   0 abkl      (1000) abkl      (1000)     1249 2022-11-04 13:15:48.000000 sharepoint_v1_api-0.1.4/sharepoint_api/SharePointTimeRegistration.py
+-rw-r--r--   0 abkl      (1000) abkl      (1000)      721 2022-11-04 13:15:48.000000 sharepoint_v1_api-0.1.4/sharepoint_api/SharePointUser.py
+-rw-r--r--   0 abkl      (1000) abkl      (1000)      672 2022-11-04 13:15:48.000000 sharepoint_v1_api-0.1.4/sharepoint_api/SharePointUserList.py
+-rw-r--r--   0 abkl      (1000) abkl      (1000)       40 2022-11-04 13:15:48.000000 sharepoint_v1_api-0.1.4/sharepoint_api/__init__.py
+drwxr-xr-x   0 abkl      (1000) abkl      (1000)        0 2023-08-02 14:23:55.942253 sharepoint_v1_api-0.1.4/sharepoint_v1_api.egg-info/
+-rw-r--r--   0 abkl      (1000) abkl      (1000)     2518 2023-08-02 14:23:55.000000 sharepoint_v1_api-0.1.4/sharepoint_v1_api.egg-info/PKG-INFO
+-rw-r--r--   0 abkl      (1000) abkl      (1000)      535 2023-08-02 14:23:55.000000 sharepoint_v1_api-0.1.4/sharepoint_v1_api.egg-info/SOURCES.txt
+-rw-r--r--   0 abkl      (1000) abkl      (1000)        1 2023-08-02 14:23:55.000000 sharepoint_v1_api-0.1.4/sharepoint_v1_api.egg-info/dependency_links.txt
+-rw-r--r--   0 abkl      (1000) abkl      (1000)       23 2023-08-02 14:23:55.000000 sharepoint_v1_api-0.1.4/sharepoint_v1_api.egg-info/requires.txt
+-rw-r--r--   0 abkl      (1000) abkl      (1000)       15 2023-08-02 14:23:55.000000 sharepoint_v1_api-0.1.4/sharepoint_v1_api.egg-info/top_level.txt
```

### Comparing `sharepoint_v1_api-0.1.3/LICENSE` & `sharepoint_v1_api-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sharepoint_v1_api-0.1.3/PKG-INFO` & `sharepoint_v1_api-0.1.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,97 +1,96 @@
 Metadata-Version: 2.1
 Name: sharepoint_v1_api
-Version: 0.1.3
-Summary: UNKNOWN
-Home-page: UNKNOWN
+Version: 0.1.4
 Author: Aske Bluhme Klok
 License: MIT
-Description: # sharepoint_v1_api
-        
-        Version 0.1.3
-        
-        # Setup
-        
-        
-        ```python
-        from sharepoint_api.SharePointAPI import SharePointAPI as SP
-        
-        creds = {
-            "username": "",
-            "password": "",
-            "sharepoint_url": "",
-            'proxies': {}
-        }
-        
-        sp = SP._compact_init(creds)
-        ```
-        
-        ## Get lists in a sharepoint_site
-        ```python
-        # Get an overview of all lists in a sharepoint_site
-        sharepoint_site_name = "NAME_OF_YOUR_SITE"
-        sp_lists = sp.get_lists(sharepoint_site_name)
-        print(sp_lists)
-        
-        # Load one of the lists by name
-        list_name = 'Sager'
-        cases_list = sp_lists.get_list(list_name)
-        print(cases_list.Title)
-        ```
-        
-        # Get items in a list
-        ```python
-        # When loading a list the top 1000 items will be retrieved
-        sharepoint_site_name = "NAME_OF_YOUR_SITE"
-        list_name = 'Sager'
-        cases_list = sp.get_list_by_name(sharepoint_site_name, list_name)
-        print(cases_list.all_items)
-        
-        # If the list is contains more items, it may be necesarry to use a filter
-        # Filters can be formatted as shown below
-        filters = ' and '.join([
-                "(TeamId == '3')",
-                "(Status == '11 - Modtaget')",
-                "((Status != '90 - Lukket') and (Status != '91 - Afvist') and (Status != '92 - Duplikeret') and (Status != '93 - Annulleret'))"
-                ])
-        cases_list = sp.get_list_by_name(sharepoint_site_name, list_name, filters)
-        print(cases_list.all_items)
-        ```
-        
-        # Add certificates files to a certificate list
-        ```python
-        # Set sharepoint_site name
-        sharepoint_site_name = "NAME_OF_YOUR_SITE"
-        
-        # Set name of certificates (use Certifikater if danish)
-        list_name = 'Certificates'
-        cert_list = sp.get_list_by_name(sharepoint_site_name, list_name)
-        
-        # The certificate metadata (such as name, expiry date and such)
-        data = {
-         "Title": "My Certificate Name",
-         "ExpiryDate": "2020-11-25"
-        }
-        
-        # Create the certificate item
-        item = sp.create_item(sharepoint_site_name, cert_list, data)
-        
-        # Attach the file
-        file_name = 'my_file.txt'
-        file_path = 'path/to/my_file.txt'
-        item.attach_item(file_name, file_path)
-        
-        
-        # Attach another file
-        file_name = 'mysecondfile.txt'
-        file_path = 'path/to/mysecondfile.txt'
-        attach_file("mysecondfile.txt", sharepoint_site_name, cert_list, item)
-        ```
 Keywords: Sharepoint
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9.2
+Requires-Python: >=3.6.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# sharepoint_v1_api
+
+Version 0.1.4
+
+# Setup
+
+
+```python
+from sharepoint_api.SharePointAPI import SharePointAPI as SP
+
+creds = {
+    "username": "",
+    "password": "",
+    "sharepoint_url": "",
+    'proxies': {}
+}
+
+sp = SP._compact_init(creds)
+```
+
+## Get lists in a sharepoint_site
+```python
+# Get an overview of all lists in a sharepoint_site
+sharepoint_site_name = "NAME_OF_YOUR_SITE"
+sp_lists = sp.get_lists(sharepoint_site_name)
+print(sp_lists)
+
+# Load one of the lists by name
+list_name = 'Sager'
+cases_list = sp_lists.get_list(list_name)
+print(cases_list.Title)
+```
+
+# Get items in a list
+```python
+# When loading a list the top 1000 items will be retrieved
+sharepoint_site_name = "NAME_OF_YOUR_SITE"
+list_name = 'Sager'
+cases_list = sp.get_list_by_name(sharepoint_site_name, list_name)
+print(cases_list.all_items)
+
+# If the list is contains more items, it may be necesarry to use a filter
+# Filters can be formatted as shown below
+filters = ' and '.join([
+        "(TeamId == '3')",
+        "(Status == '11 - Modtaget')",
+        "((Status != '90 - Lukket') and (Status != '91 - Afvist') and (Status != '92 - Duplikeret') and (Status != '93 - Annulleret'))"
+        ])
+cases_list = sp.get_list_by_name(sharepoint_site_name, list_name, filters)
+print(cases_list.all_items)
+```
+
+# Add certificates files to a certificate list
+```python
+# Set sharepoint_site name
+sharepoint_site_name = "NAME_OF_YOUR_SITE"
+
+# Set name of certificates (use Certifikater if danish)
+list_name = 'Certificates'
+cert_list = sp.get_list_by_name(sharepoint_site_name, list_name)
+
+# The certificate metadata (such as name, expiry date and such)
+data = {
+ "Title": "My Certificate Name",
+ "ExpiryDate": "2020-11-25"
+}
+
+# Create the certificate item
+item = sp.create_item(sharepoint_site_name, cert_list, data)
+
+# Attach the file
+file_name = 'my_file.txt'
+file_path = 'path/to/my_file.txt'
+item.attach_item(file_name, file_path)
+
+
+# Attach another file
+file_name = 'mysecondfile.txt'
+file_path = 'path/to/mysecondfile.txt'
+attach_file("mysecondfile.txt", sharepoint_site_name, cert_list, item)
+```
```

### Comparing `sharepoint_v1_api-0.1.3/README.md` & `sharepoint_v1_api-0.1.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # sharepoint_v1_api
 
-Version 0.1.3
+Version 0.1.4
 
 # Setup
 
 
 ```python
 from sharepoint_api.SharePointAPI import SharePointAPI as SP
```

### Comparing `sharepoint_v1_api-0.1.3/setup.py` & `sharepoint_v1_api-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 
 with open("README.md", "r") as readme_file:
     long_description = readme_file.read()
 
 packages = ["sharepoint_api"]
 
 setup(
@@ -21,9 +21,9 @@
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     keywords="Sharepoint",
     packages=packages,
     install_requires=["requests", "requests-ntlm"],
-    python_requires=">=3.9.2"
+    python_requires=">=3.6.8"
 )
```

### Comparing `sharepoint_v1_api-0.1.3/sharepoint_api/SharePointAPI.py` & `sharepoint_v1_api-0.1.4/sharepoint_api/SharePointAPI.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,16 @@
             "sharepoint_url": ""
         }
         '''
 
         username = credentials['username']
         password = credentials['password']
         sharepoint_url = credentials['sharepoint_url']
-        proxies = {} if 'proxies' not in credentials else credentials['proxies']
+        proxies = {
+        } if 'proxies' not in credentials else credentials['proxies']
 
         sharepoint_api = object.__new__(SharePointAPI)
         sharepoint_api.__init__(username, password, sharepoint_url, proxies)
 
         return sharepoint_api
 
     def __init__(self, username: str, password: str, sharepoint_url: str, proxies: dict):
@@ -76,14 +77,49 @@
             print('Exiting.')
             raise ConnectionError
         elif r.status_code not in [200, 201, 204]:
             print('Failed to connect: ', r.status_code)
             print('Exiting.')
             raise ConnectionError
         return r
+    
+    def _api_put_call(self, url, put_data, form_digest_value=None, merge=False):
+        headers = {
+            'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:71.0) Gecko/20100101 Firefox/71.0',
+            'accept': 'application/json;odata=verbose',
+            'Content-type': 'application/json; charset=utf-8',
+            'Cache-Control': 'no-cache',
+            'Connection': 'keep-alive',
+            'Accept-Encoding': 'gzip, deflate, br',
+            'Content-Length': str(len(f'{put_data}')),
+            'X-RequestDigest': f'{form_digest_value}',
+            'If-Match': '*'
+        }
+        if merge:
+            headers['X-HTTP-Method'] = 'MERGE'
+
+        r = requests.put(url,
+                          auth=HttpNtlmAuth(self.username, self.password), headers=headers, json=put_data, proxies=self.proxies)
+
+        if r.status_code == 400:
+            print('Failed to connect: ', r.status_code)
+            print(r.text)
+            print('Exiting.')
+            raise ConnectionError
+        elif r.status_code == 404:
+            print('Failed to connect: ', r.status_code)
+            print(r.request.url)
+            print(r.request.body)
+            print('Exiting.')
+            raise ConnectionError
+        elif r.status_code not in [200, 201, 204]:
+            print('Failed to connect: ', r.status_code)
+            print('Exiting.')
+            raise ConnectionError
+        return r
 
     def _api_attachment_call(self, url, post_data, form_digest_value=None, overwrite=False, x_http_method=None):
         headers = {
             'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:71.0) Gecko/20100101 Firefox/71.0',
             'accept': 'application/json;odata=verbose',
             'X-RequestDigest': f'{form_digest_value}'
         }
@@ -194,15 +230,15 @@
             Returns a list of lists from a given sharepoint_site
         '''
         r = self._api_get_call(
             f'{self.sharepoint_url}/cases/{sharepoint_site}/_api/Web/Lists')
 
         _lists = []
         for list_props in r.json()["d"]["results"]:
-            _lists.append(SharePointList(sharepoint_site, list_props))
+            _lists.append(SharePointList(self, sharepoint_site, list_props))
 
         return SharePointLists(_lists)
 
     def get_list(self, sharepoint_site, sp_list, filters=None, top=1000, view_path=None, SPListType: SharePointList = SharePointList) -> SharePointList:
         '''
             Returns a list from a given sharepoint_site using its guid
 
@@ -213,21 +249,21 @@
         '''
 
         # Uses either guid or SharePointList
         if isinstance(sp_list, SharePointList):
             guid = sp_list.guid
             r = self._api_get_call(
                 f'{self.sharepoint_url}/cases/{sharepoint_site}/_api/Web/Lists(guid\'{guid}\')')
-            sp_list = SPListType(sharepoint_site, r.json()["d"])
+            sp_list = SPListType(self, sharepoint_site, r.json()["d"])
 
         elif isinstance(sp_list, str):
             guid = sp_list
             r = self._api_get_call(
                 f'{self.sharepoint_url}/cases/{sharepoint_site}/_api/Web/Lists(guid\'{guid}\')')
-            sp_list = SPListType(sharepoint_site, r.json()["d"])
+            sp_list = SPListType(self, sharepoint_site, r.json()["d"])
         else:
             sys.exit(1)
 
         arguments = []
 
         if filters is not None:
             if not isinstance(filters, list):
@@ -293,15 +329,15 @@
             cases = []
             for case in data_dict['cases']:
                 settings = case["settings"]
                 versions = None if "versions" not in case else case["versions"]
                 cases.append(SPListType.SPItem(
                     self, sharepoint_site, guid, settings, versions))
 
-            return SPListType(sharepoint_site, data_dict['Settings'], cases)
+            return SPListType(self, sharepoint_site, data_dict['Settings'], cases)
         except FileNotFoundError as err:
             print(f"File '{file_name}' was not found")
             raise err
         except Exception as err:
             raise err
 
     # SP Item
@@ -329,15 +365,15 @@
         # Uses either guid or SharePointList
         if isinstance(sp_list, SharePointList):
             guid = sp_list.guid
         elif isinstance(sp_list, str):
             guid = sp_list
             r = self._api_get_call(
                 f'{self.sharepoint_url}/cases/{sharepoint_site}/_api/Web/Lists(guid\'{guid}\')')
-            sp_list = SharePointList(
+            sp_list = SharePointList(self,
                 sharepoint_site, r.json()["d"]["results"][0])
 
         r = self._api_post_call(
             f'{self.sharepoint_url}/cases/{sharepoint_site}/_api/contextinfo', {})
 
         form_digest_value = r.json(
         )["d"]["GetContextWebInformation"]["FormDigestValue"]
@@ -357,31 +393,29 @@
             item_id: The id of the item
             data: Data to push to the item
         '''
         if isinstance(sp_list, SharePointList):
             guid = sp_list.guid
         elif isinstance(sp_list, str):
             guid = sp_list
-            r = self._api_get_call(
-                f'{self.sharepoint_url}/cases/{sharepoint_site}/_api/Web/Lists(guid\'{guid}\')')
-            sp_list = SharePointList(
-                sharepoint_site, r.json()["d"]["results"][0])
         else:
             raise TypeError(
                 'Only "SharePointList" and "str" types are allowed')
 
         r = self._api_post_call(
             f'{self.sharepoint_url}/cases/{sharepoint_site}/_api/contextinfo', {})
 
         form_digest_value = r.json(
         )["d"]["GetContextWebInformation"]["FormDigestValue"]
 
         r = self._api_post_call(
             f'{self.sharepoint_url}/cases/{sharepoint_site}/_api/Web/Lists(guid\'{guid}\')/items({item_id})', data, form_digest_value, merge=True)
 
+        return r
+
     def attach_file(self, sharepoint_site, sp_list, item, file_name, file_content) -> dict:
         # Uses either guid or SharePointList
         if isinstance(sp_list, SharePointList):
             guid = sp_list.guid
         elif isinstance(sp_list, str):
             guid = sp_list
         else:
```

### Comparing `sharepoint_v1_api-0.1.3/sharepoint_api/SharePointList.py` & `sharepoint_v1_api-0.1.4/sharepoint_api/SharePointList.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,16 @@
     sharepoint_site = None
     SPItem = SharePointListItem
 
     CHANGE_DETECTED = False
     SAVE_ON_CHANGE = False
     JSON_FILENAME = None
 
-    def __init__(self, sharepoint_site, settings: dict = None, items: List[SPItem] = None):
+    def __init__(self, sp, sharepoint_site, settings: dict = None, items: List[SPItem] = None):
+        self.sp = sp
         self.sharepoint_site = sharepoint_site
         self.settings = settings
         self.append_items(items)
 
     def __str__(self):
         items = ''
         for _, _item in self.all_items.items():
@@ -69,14 +70,17 @@
             for item in items:
                 item._list = self
                 self._items[item.Id] = item
 
         elif isinstance(items, self.SPItem):
             items._list = self
             self.all_items[items.Id] = items
+    
+    def create_item(self, data):
+        self.sp.create_item(self.sharepoint_site, self, data)
 
     def get_item_by_name(self, name):
         '''
         '''
         items = {}
         for item_id, item in self._items.items():
             if name == item.Title:
```

### Comparing `sharepoint_v1_api-0.1.3/sharepoint_api/SharePointListItem.py` & `sharepoint_v1_api-0.1.4/sharepoint_api/SharePointListItem.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,16 +68,17 @@
         self.sp.attach_file(self.sharepoint_site, self.list, self, file_name, file_content)
 
     def versions_select_fields(self, select_fields=[]) -> list:
         if not self._versions:
             self._versions = self.sp.get_item_versions(self.sharepoint_site, self.list_guid, self.Id, select_fields) 
         return self._versions
 
-    
-
+    def update_fields(self, data):
+        self.sp.update_item(self.sharepoint_site,
+                            self.list_guid, self.Id, data)
 
 class SharepointSiteCase(SharePointListItem):
     
     @property
     def AssignmentType(self) -> str:
         return self.settings['AssignmentType']
```

### Comparing `sharepoint_v1_api-0.1.3/sharepoint_api/SharePointLists.py` & `sharepoint_v1_api-0.1.4/sharepoint_api/SharePointLists.py`

 * *Files identical despite different names*

### Comparing `sharepoint_v1_api-0.1.3/sharepoint_api/SharePointTimeRegistration.py` & `sharepoint_v1_api-0.1.4/sharepoint_api/SharePointTimeRegistration.py`

 * *Files identical despite different names*

### Comparing `sharepoint_v1_api-0.1.3/sharepoint_api/SharePointUser.py` & `sharepoint_v1_api-0.1.4/sharepoint_api/SharePointUser.py`

 * *Files identical despite different names*

### Comparing `sharepoint_v1_api-0.1.3/sharepoint_api/SharePointUserList.py` & `sharepoint_v1_api-0.1.4/sharepoint_api/SharePointUserList.py`

 * *Files identical despite different names*

### Comparing `sharepoint_v1_api-0.1.3/sharepoint_v1_api.egg-info/SOURCES.txt` & `sharepoint_v1_api-0.1.4/sharepoint_v1_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

