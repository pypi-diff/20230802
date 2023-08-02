# Comparing `tmp/propelauth-py-3.1.3.tar.gz` & `tmp/propelauth-py-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "propelauth-py-3.1.3.tar", last modified: Tue Jun  6 16:20:34 2023, max compression
+gzip compressed data, was "propelauth-py-3.1.4.tar", last modified: Wed Aug  2 17:48:15 2023, max compression
```

## Comparing `propelauth-py-3.1.3.tar` & `propelauth-py-3.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:20:34.581476 propelauth-py-3.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-06 16:20:25.000000 propelauth-py-3.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-06 16:20:34.581476 propelauth-py-3.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-06 16:20:25.000000 propelauth-py-3.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:20:34.581476 propelauth-py-3.1.3/propelauth_py/
--rw-r--r--   0 runner    (1001) docker     (123)    15365 2023-06-06 16:20:25.000000 propelauth-py-3.1.3/propelauth_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30324 2023-06-06 16:20:25.000000 propelauth-py-3.1.3/propelauth_py/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-06-06 16:20:25.000000 propelauth-py-3.1.3/propelauth_py/auth_fns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-06 16:20:25.000000 propelauth-py-3.1.3/propelauth_py/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-06 16:20:25.000000 propelauth-py-3.1.3/propelauth_py/jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-06-06 16:20:25.000000 propelauth-py-3.1.3/propelauth_py/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-06 16:20:25.000000 propelauth-py-3.1.3/propelauth_py/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:20:34.581476 propelauth-py-3.1.3/propelauth_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-06 16:20:34.000000 propelauth-py-3.1.3/propelauth_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-06 16:20:34.000000 propelauth-py-3.1.3/propelauth_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 16:20:34.000000 propelauth-py-3.1.3/propelauth_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-06 16:20:34.000000 propelauth-py-3.1.3/propelauth_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-06 16:20:34.000000 propelauth-py-3.1.3/propelauth_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 16:20:34.581476 propelauth-py-3.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-06 16:20:25.000000 propelauth-py-3.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:48:15.803007 propelauth-py-3.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-02 17:48:06.000000 propelauth-py-3.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-08-02 17:48:15.803007 propelauth-py-3.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-02 17:48:06.000000 propelauth-py-3.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:48:15.803007 propelauth-py-3.1.4/propelauth_py/
+-rw-r--r--   0 runner    (1001) docker     (123)    15514 2023-08-02 17:48:06.000000 propelauth-py-3.1.4/propelauth_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30585 2023-08-02 17:48:06.000000 propelauth-py-3.1.4/propelauth_py/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-08-02 17:48:06.000000 propelauth-py-3.1.4/propelauth_py/auth_fns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-08-02 17:48:06.000000 propelauth-py-3.1.4/propelauth_py/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-02 17:48:06.000000 propelauth-py-3.1.4/propelauth_py/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-08-02 17:48:06.000000 propelauth-py-3.1.4/propelauth_py/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-02 17:48:06.000000 propelauth-py-3.1.4/propelauth_py/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:48:15.803007 propelauth-py-3.1.4/propelauth_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-08-02 17:48:15.000000 propelauth-py-3.1.4/propelauth_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-08-02 17:48:15.000000 propelauth-py-3.1.4/propelauth_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:48:15.000000 propelauth-py-3.1.4/propelauth_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 17:48:15.000000 propelauth-py-3.1.4/propelauth_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-02 17:48:15.000000 propelauth-py-3.1.4/propelauth_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 17:48:15.803007 propelauth-py-3.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-02 17:48:06.000000 propelauth-py-3.1.4/setup.py
```

### Comparing `propelauth-py-3.1.3/LICENSE` & `propelauth-py-3.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.3/PKG-INFO` & `propelauth-py-3.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propelauth-py
-Version: 3.1.3
+Version: 3.1.4
 Summary: A python authentication library
 Home-page: https://github.com/propelauth/propelauth-py
 Author: PropelAuth
 Author-email: support@propelauth.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propelauth-py Version: 3.1.3 Summary: A python
+Metadata-Version: 2.1 Name: propelauth-py Version: 3.1.4 Summary: A python
 authentication library Home-page: https://github.com/propelauth/propelauth-py
 Author: PropelAuth Author-email: support@propelauth.com License: MIT Platform:
 UNKNOWN Description-Content-Type: text/markdown License-File: LICENSE #
 PropelAuth Python SDK
       [https://propelauth-logos.s3.us-west-2.amazonaws.com/logo-only.png]
 A python library for managing authentication, backed by [PropelAuth](https://
 www.propelauth.com/?utm_campaign=github-python). [PropelAuth](https://
```

### Comparing `propelauth-py-3.1.3/README.md` & `propelauth-py-3.1.4/README.md`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.3/propelauth_py/__init__.py` & `propelauth-py-3.1.4/propelauth_py/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,24 +112,25 @@
                                      include_orgs)
 
     def fetch_users_in_org(org_id, page_size=10, page_number=0, include_orgs=False):
         return _fetch_users_in_org(auth_url, integration_api_key, org_id, page_size, page_number, include_orgs)
 
     def create_user(email, email_confirmed=False, send_email_to_confirm_email_address=True,
                     ask_user_to_update_password_on_login=False,
-                    password=None, username=None, first_name=None, last_name=None):
+                    password=None, username=None, first_name=None, last_name=None,
+                    properties=None):
         return _create_user(auth_url, integration_api_key, email, email_confirmed, send_email_to_confirm_email_address,
                             ask_user_to_update_password_on_login,
-                            password, username, first_name, last_name)
+                            password, username, first_name, last_name, properties)
 
     def update_user_email(user_id, new_email, require_email_confirmation):
         return _update_user_email(auth_url, integration_api_key, user_id, new_email, require_email_confirmation)
 
-    def update_user_metadata(user_id, username=None, first_name=None, last_name=None, metadata=None):
-        return _update_user_metadata(auth_url, integration_api_key, user_id, username, first_name, last_name, metadata)
+    def update_user_metadata(user_id, username=None, first_name=None, last_name=None, metadata=None, properties=None):
+        return _update_user_metadata(auth_url, integration_api_key, user_id, username, first_name, last_name, metadata, properties)
 
     def update_user_password(user_id, password, ask_user_to_update_password_on_login=False):
         return _update_user_password(auth_url, integration_api_key, user_id, password, ask_user_to_update_password_on_login)
 
     def create_magic_link(email, redirect_to_url=None, expires_in_hours=None, create_new_user_if_one_doesnt_exist=None):
         return _create_magic_link(auth_url, integration_api_key, email, redirect_to_url, expires_in_hours,
                                   create_new_user_if_one_doesnt_exist)
@@ -137,20 +138,21 @@
     def create_access_token(user_id, duration_in_minutes):
         return _create_access_token(auth_url, integration_api_key, user_id, duration_in_minutes)
 
     def migrate_user_from_external_source(email, email_confirmed,
                                           existing_user_id=None, existing_password_hash=None,
                                           existing_mfa_base32_encoded_secret=None,
                                           ask_user_to_update_password_on_login=False,
-                                          enabled=None, first_name=None, last_name=None, username=None):
+                                          enabled=None, first_name=None, last_name=None, username=None,
+                                          properties=None):
         return _migrate_user_from_external_source(auth_url, integration_api_key, email, email_confirmed,
                                                   existing_user_id, existing_password_hash,
                                                   existing_mfa_base32_encoded_secret,
                                                   ask_user_to_update_password_on_login,
-                                                  enabled, first_name, last_name, username)
+                                                  enabled, first_name, last_name, username, properties)
 
     def create_org(name):
         return _create_org(auth_url, integration_api_key, name)
 
     def update_org_metadata(org_id, name=None, can_setup_saml=None, metadata=None):
         return _update_org_metadata(auth_url, integration_api_key, org_id, name, can_setup_saml, metadata)
```

### Comparing `propelauth-py-3.1.3/propelauth_py/api.py` & `propelauth-py-3.1.4/propelauth_py/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,53 +204,57 @@
         raise RuntimeError("Unknown error when fetching users in org")
 
     return response.json()
 
 
 def _create_user(auth_url, integration_api_key, email, email_confirmed, send_email_to_confirm_email_address,
                  ask_user_to_update_password_on_login,
-                 password, username, first_name, last_name):
+                 password, username, first_name, last_name, properties):
     url = auth_url + "/api/backend/v1/user/"
     json = {"email": email, "email_confirmed": email_confirmed,
             "send_email_to_confirm_email_address": send_email_to_confirm_email_address,
             "ask_user_to_update_password_on_login": ask_user_to_update_password_on_login}
     if password is not None:
         json["password"] = password
     if username is not None:
         json["username"] = username
     if first_name is not None:
         json["first_name"] = first_name
     if last_name is not None:
         json["last_name"] = last_name
+    if properties is not None:
+        json["properties"] = properties
     response = requests.post(url, json=json, auth=_ApiKeyAuth(integration_api_key))
     if response.status_code == 401:
         raise ValueError("integration_api_key is incorrect")
     elif response.status_code == 400:
         raise CreateUserException(response.json())
     elif not response.ok:
         raise RuntimeError("Unknown error when creating user")
 
     return response.json()
 
 
 def _update_user_metadata(auth_url, integration_api_key, user_id, username=None, first_name=None, last_name=None,
-                          metadata=None):
+                          metadata=None, properties=None):
     if not _is_valid_id(user_id):
         return False
 
     url = auth_url + "/api/backend/v1/user/{}".format(user_id)
     json = {}
     if username is not None:
         json["username"] = username
     if first_name is not None:
         json["first_name"] = first_name
     if last_name is not None:
         json["last_name"] = last_name
     if metadata is not None:
         json["metadata"] = metadata
+    if properties is not None:
+        json["properties"] = properties
 
     response = requests.put(url, json=json, auth=_ApiKeyAuth(integration_api_key))
     if response.status_code == 401:
         raise ValueError("integration_api_key is incorrect")
     elif response.status_code == 400:
         raise UpdateUserMetadataException(response.json())
     elif response.status_code == 404:
@@ -349,27 +353,29 @@
     return response.json()
 
 
 def _migrate_user_from_external_source(auth_url, integration_api_key, email, email_confirmed,
                                        existing_user_id=None, existing_password_hash=None,
                                        existing_mfa_base32_encoded_secret=None,
                                        ask_user_to_update_password_on_login=False,
-                                       enabled=None, first_name=None, last_name=None, username=None):
+                                       enabled=None, first_name=None, last_name=None, username=None,
+                                       properties=None):
     url = auth_url + "/api/backend/v1/migrate_user/"
     json = {
         "email": email,
         "email_confirmed": email_confirmed,
         "existing_user_id": existing_user_id,
         "existing_password_hash": existing_password_hash,
         "existing_mfa_base32_encoded_secret": existing_mfa_base32_encoded_secret,
         "ask_user_to_update_password_on_login": ask_user_to_update_password_on_login,
         "enabled": enabled,
         "first_name": first_name,
         "last_name": last_name,
-        "username": username
+        "username": username,
+        "properties": properties
     }
 
     response = requests.post(url, json=json, auth=_ApiKeyAuth(integration_api_key))
     if response.status_code == 401:
         raise ValueError("integration_api_key is incorrect")
     elif response.status_code == 400:
         raise BadRequestException(response.json())
```

### Comparing `propelauth-py-3.1.3/propelauth_py/auth_fns.py` & `propelauth-py-3.1.4/propelauth_py/auth_fns.py`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.3/propelauth_py/errors.py` & `propelauth-py-3.1.4/propelauth_py/errors.py`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.3/propelauth_py/jwt.py` & `propelauth-py-3.1.4/propelauth_py/jwt.py`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.3/propelauth_py/user.py` & `propelauth-py-3.1.4/propelauth_py/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from propelauth_py.errors import UnauthorizedException
 
 
 class User:
     def __init__(self, user_id, org_id_to_org_member_info, email, first_name=None, last_name=None, username=None,
-                 legacy_user_id=None, impersonator_user_id=None, metadata=None):
+                 legacy_user_id=None, impersonator_user_id=None, metadata=None, properties=None):
         self.user_id = user_id
         self.org_id_to_org_member_info = org_id_to_org_member_info
         self.email = email
         self.first_name = first_name
         self.last_name = last_name
         self.username = username
         self.legacy_user_id = legacy_user_id
         self.impersonator_user_id = impersonator_user_id
         self.metadata = metadata
+        self.properties = properties
 
     def __eq__(self, other):
         if isinstance(other, User):
             return self.user_id == other.user_id and self.org_id_to_org_member_info == other.org_id_to_org_member_info \
                 and self.legacy_user_id == other.legacy_user_id and self.impersonator_user_id == other.impersonator_user_id \
                 and self.email == other.email and self.first_name == other.first_name and self.last_name == other.last_name \
-                and self.username == other.username and self.metadata == other.metadata
+                and self.username == other.username and self.metadata == other.metadata and self.properties == other.properties
 
         return False
 
     def is_impersonated(self):
         """returns true if the user is impersonated"""
         return self.impersonator_user_id is not None
 
@@ -99,8 +100,9 @@
     org_id_to_org_member_info = _to_org_member_info(decoded_token.get("org_id_to_org_member_info"))
     return User(user_id, org_id_to_org_member_info, decoded_token.get("email"),
                 first_name=decoded_token.get("first_name"),
                 last_name=decoded_token.get("last_name"),
                 username=decoded_token.get("username"),
                 legacy_user_id=decoded_token.get("legacy_user_id"),
                 impersonator_user_id=decoded_token.get("impersonator_user_id"),
-                metadata=decoded_token.get("metadata"))
+                metadata=decoded_token.get("metadata"),
+                properties=decoded_token.get("properties"))
```

### Comparing `propelauth-py-3.1.3/propelauth_py.egg-info/PKG-INFO` & `propelauth-py-3.1.4/propelauth_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propelauth-py
-Version: 3.1.3
+Version: 3.1.4
 Summary: A python authentication library
 Home-page: https://github.com/propelauth/propelauth-py
 Author: PropelAuth
 Author-email: support@propelauth.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propelauth-py Version: 3.1.3 Summary: A python
+Metadata-Version: 2.1 Name: propelauth-py Version: 3.1.4 Summary: A python
 authentication library Home-page: https://github.com/propelauth/propelauth-py
 Author: PropelAuth Author-email: support@propelauth.com License: MIT Platform:
 UNKNOWN Description-Content-Type: text/markdown License-File: LICENSE #
 PropelAuth Python SDK
       [https://propelauth-logos.s3.us-west-2.amazonaws.com/logo-only.png]
 A python library for managing authentication, backed by [PropelAuth](https://
 www.propelauth.com/?utm_campaign=github-python). [PropelAuth](https://
```

### Comparing `propelauth-py-3.1.3/setup.py` & `propelauth-py-3.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # See https://pytest-runner.readthedocs.io/en/latest/#conditional-requirement
 needs_pytest = {'pytest', 'test', 'ptr'}.intersection(sys.argv)
 pytest_runner = ['pytest-runner'] if needs_pytest else []
 
 setup(
     name="propelauth-py",
-    version="3.1.3",
+    version="3.1.4",
     description="A python authentication library",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/propelauth/propelauth-py",
     packages=find_packages(include=["propelauth_py"]),
     author="PropelAuth",
     author_email="support@propelauth.com",
```

