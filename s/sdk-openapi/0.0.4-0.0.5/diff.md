# Comparing `tmp/sdk-openapi-0.0.4.tar.gz` & `tmp/sdk-openapi-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdk-openapi-0.0.4.tar", last modified: Wed Aug  2 05:52:36 2023, max compression
+gzip compressed data, was "sdk-openapi-0.0.5.tar", last modified: Wed Aug  2 14:54:51 2023, max compression
```

## Comparing `sdk-openapi-0.0.4.tar` & `sdk-openapi-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 05:52:36.845885 sdk-openapi-0.0.4/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      816 2023-08-02 05:52:36.845885 sdk-openapi-0.0.4/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      265 2023-07-24 06:43:42.000000 sdk-openapi-0.0.4/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 05:52:36.841885 sdk-openapi-0.0.4/openapi/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      180 2023-07-24 07:04:11.000000 sdk-openapi-0.0.4/openapi/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      130 2023-07-24 05:56:12.000000 sdk-openapi-0.0.4/openapi/constants.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2046 2023-08-02 05:35:47.000000 sdk-openapi-0.0.4/openapi/core.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 05:52:36.845885 sdk-openapi-0.0.4/sdk_openapi.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      816 2023-08-02 05:52:36.000000 sdk-openapi-0.0.4/sdk_openapi.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      249 2023-08-02 05:52:36.000000 sdk-openapi-0.0.4/sdk_openapi.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-08-02 05:52:36.000000 sdk-openapi-0.0.4/sdk_openapi.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-08-02 05:52:36.000000 sdk-openapi-0.0.4/sdk_openapi.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        8 2023-08-02 05:52:36.000000 sdk-openapi-0.0.4/sdk_openapi.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-08-02 05:52:36.845885 sdk-openapi-0.0.4/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      997 2023-08-02 05:48:58.000000 sdk-openapi-0.0.4/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 14:54:51.485540 sdk-openapi-0.0.5/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1208 2023-08-02 14:54:51.481540 sdk-openapi-0.0.5/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      657 2023-08-02 14:42:12.000000 sdk-openapi-0.0.5/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 14:54:51.481540 sdk-openapi-0.0.5/openapi/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      180 2023-07-24 07:04:11.000000 sdk-openapi-0.0.5/openapi/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       90 2023-08-02 14:40:26.000000 sdk-openapi-0.0.5/openapi/constants.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2111 2023-08-02 14:54:41.000000 sdk-openapi-0.0.5/openapi/core.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 14:54:51.481540 sdk-openapi-0.0.5/sdk_openapi.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1208 2023-08-02 14:54:51.000000 sdk-openapi-0.0.5/sdk_openapi.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      249 2023-08-02 14:54:51.000000 sdk-openapi-0.0.5/sdk_openapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-08-02 14:54:51.000000 sdk-openapi-0.0.5/sdk_openapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-08-02 14:54:51.000000 sdk-openapi-0.0.5/sdk_openapi.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        8 2023-08-02 14:54:51.000000 sdk-openapi-0.0.5/sdk_openapi.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-08-02 14:54:51.485540 sdk-openapi-0.0.5/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      997 2023-08-02 14:44:40.000000 sdk-openapi-0.0.5/setup.py
```

### Comparing `sdk-openapi-0.0.4/openapi/core.py` & `sdk-openapi-0.0.5/openapi/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import base64
 from httpx import AsyncClient
 from openapi.constants import *
 
+
 class Client:
     """
     OpenApi Package for interacting with OpenAPI `api.qewertyy.me`
     """
 
     def __init__(
         self
@@ -13,16 +14,16 @@
         """
         Initialize the class
         """
         self.url = BASE_URL,
         self.session = AsyncClient(
             http2=True,
             headers=SESSION_HEADERS,
-            )
-    
+        )
+
     async def palm(self, prompt: str) -> dict:
         """ 
         Get an answer from Palm 2 for the given prompt
         Example:
         >>> client = Client()
         >>> response = await client.palm("Hello, Who are you?")
         >>> print(response)
@@ -37,24 +38,25 @@
                     "content": str
                 }
         """
         params = {
             "model_id": 0,
             "prompt": prompt
         }
+        self.session.headers.update({"Content-Type": "application/json"})
         try:
             resp = await self.session.post(
-                f"{self.url}/models",
+                f"{self.url[0]}/models",
                 params=params,
             )
             return resp.json()
         except Exception as e:
             print(f"Request failed: {e}")
-    
-    async def upscale(self,image:bytes) -> bytes:
+
+    async def upscale(self, image: bytes) -> bytes:
         """ 
         Upscale an image
         Example:
         >>> client = Client()
         >>> response = await client.upscale(image)
         >>> with open('upscaled.png', 'wb') as f:
                 f.write(response.content)
@@ -64,13 +66,13 @@
         Returns:
             bytes: Upscaled image in bytes.
         """
         try:
             b = base64.b64encode(image).decode('utf-8')
             response = await self.session.post(
                 f'{self.url[0]}/upscale',
-                    data={'image_data': b},
+                data={'image_data': b},
                 timeout=None
             )
             return response.content
         except Exception as e:
-            print(f"Failed to upscale the image: {e}")
+            print(f"Failed to upscale the image: {e}")
```

### Comparing `sdk-openapi-0.0.4/setup.py` & `sdk-openapi-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def get_long_description():
     with open("README.md", encoding="UTF-8") as f:
         long_description = f.read()
         return long_description
 
 setup(
     name="sdk-openapi",
-    version="0.0.4",
+    version="0.0.5",
     author="Qewertyy",
     author_email="Qewertyy.irl@gmail.com",
     description="The python package for api.qewertyy.me",
     url="https://github.com/Qewertyy/Open-API",
     python_requires=">=3.8",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
```

