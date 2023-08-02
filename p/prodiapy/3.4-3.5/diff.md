# Comparing `tmp/prodiapy-3.4.tar.gz` & `tmp/prodiapy-3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodiapy-3.4.tar", last modified: Tue Jul 11 10:59:15 2023, max compression
+gzip compressed data, was "prodiapy-3.5.tar", last modified: Wed Aug  2 10:28:30 2023, max compression
```

## Comparing `prodiapy-3.4.tar` & `prodiapy-3.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 10:59:15.430193 prodiapy-3.4/
--rw-rw-rw-   0        0        0    11558 2023-07-11 07:13:20.000000 prodiapy-3.4/LICENSE
--rw-rw-rw-   0        0        0     1671 2023-07-11 10:59:15.429186 prodiapy-3.4/PKG-INFO
--rw-rw-rw-   0        0        0     1454 2023-07-11 10:56:25.000000 prodiapy-3.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 10:59:15.412528 prodiapy-3.4/prodia/
--rw-rw-rw-   0        0        0      141 2023-07-11 10:54:17.000000 prodiapy-3.4/prodia/__init__.py
--rw-rw-rw-   0        0        0    14642 2023-07-11 10:45:12.000000 prodiapy-3.4/prodia/async_prodia.py
--rw-rw-rw-   0        0        0     3809 2023-07-11 09:19:46.000000 prodiapy-3.4/prodia/constants.py
--rw-rw-rw-   0        0        0      340 2023-07-11 07:13:20.000000 prodiapy-3.4/prodia/exceptions.py
--rw-rw-rw-   0        0        0    13150 2023-07-11 10:54:17.000000 prodiapy-3.4/prodia/sync_prodia.py
--rw-rw-rw-   0        0        0      332 2023-07-11 09:31:48.000000 prodiapy-3.4/prodia/templates.py
--rw-rw-rw-   0        0        0     2637 2023-07-11 09:34:16.000000 prodiapy-3.4/prodia/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:59:15.428170 prodiapy-3.4/prodiapy.egg-info/
--rw-rw-rw-   0        0        0     1671 2023-07-11 10:59:15.000000 prodiapy-3.4/prodiapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-07-11 10:59:15.000000 prodiapy-3.4/prodiapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 10:59:15.000000 prodiapy-3.4/prodiapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-07-11 10:59:15.000000 prodiapy-3.4/prodiapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-11 10:59:15.000000 prodiapy-3.4/prodiapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 10:59:15.430193 prodiapy-3.4/setup.cfg
--rw-rw-rw-   0        0        0      425 2023-07-11 10:54:17.000000 prodiapy-3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:28:30.766147 prodiapy-3.5/
+-rw-rw-rw-   0        0        0    11558 2023-07-11 07:13:20.000000 prodiapy-3.5/LICENSE
+-rw-rw-rw-   0        0        0     1783 2023-08-02 10:28:30.765106 prodiapy-3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1518 2023-08-02 09:02:38.000000 prodiapy-3.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 10:28:30.748810 prodiapy-3.5/prodia/
+-rw-rw-rw-   0        0        0      141 2023-08-02 08:56:29.000000 prodiapy-3.5/prodia/__init__.py
+-rw-rw-rw-   0        0        0    12160 2023-08-01 18:12:35.000000 prodiapy-3.5/prodia/async_prodia.py
+-rw-rw-rw-   0        0        0     3151 2023-08-01 18:12:35.000000 prodiapy-3.5/prodia/constants.py
+-rw-rw-rw-   0        0        0      340 2023-07-11 07:13:20.000000 prodiapy-3.5/prodia/exceptions.py
+-rw-rw-rw-   0        0        0    10859 2023-08-02 10:18:15.000000 prodiapy-3.5/prodia/sync_prodia.py
+-rw-rw-rw-   0        0        0      912 2023-08-01 18:03:48.000000 prodiapy-3.5/prodia/templates.py
+-rw-rw-rw-   0        0        0     1837 2023-08-01 18:12:35.000000 prodiapy-3.5/prodia/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:28:30.763542 prodiapy-3.5/prodiapy.egg-info/
+-rw-rw-rw-   0        0        0     1783 2023-08-02 10:28:30.000000 prodiapy-3.5/prodiapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-08-02 10:28:30.000000 prodiapy-3.5/prodiapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 10:28:30.000000 prodiapy-3.5/prodiapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-08-02 10:28:30.000000 prodiapy-3.5/prodiapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-02 10:28:30.000000 prodiapy-3.5/prodiapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 10:28:30.766147 prodiapy-3.5/setup.cfg
+-rw-rw-rw-   0        0        0      469 2023-08-02 09:07:20.000000 prodiapy-3.5/setup.py
```

### Comparing `prodiapy-3.4/LICENSE` & `prodiapy-3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `prodiapy-3.4/PKG-INFO` & `prodiapy-3.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 Metadata-Version: 2.1
 Name: prodiapy
-Version: 3.4
+Version: 3.5
 Summary: Prodia API Python Wrapper
+Home-page: https://github.com/zenafey/prodiapy
 Author: zenafey
 Author-email: zenafey@eugw.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # prodiapy
 This module makes generation of image by Prodia API easier
 
+[Full Documentation](https://prodiapy.readme.io/)
+
 ### Installation 
 ```
-pip install prodiapy==3.4
+pip install prodiapy==3.5
 ```
 For using this script you need to get your Prodia api key, you can make it on https://app.prodia.com/api
 
 
 ### Example of txt2img usage
 ```python
-import prodia
+from prodia import Client, Model
 
 key = "your-prodia-key"
 
-client = prodia.Client(api_key=key)
+client = Client(api_key=key)
 
-image = client.txt2img(prompt="kittens on cloud", model="dreamlike-diffusion-2.0.safetensors [fdcf65e7]")
+image = client.txt2img(prompt="kittens on cloud", model="Realistic_Vision_V4.0.safetensors [29a7afaa]")
 print(image.url)
 ```
-`image` variable will be a class with attributes:
+`image` class attributes:
 
 - url - url of generated image
 - payload - used payload
 - response - retrieved response
 - seed() - function that return seed of generated image
 - pnginfo() - function that return a dict with pnginfo of image
+- load()/ aload() - function to get image as BytesIO and its async version
 
 
 
 # HuggingFace Demo
 
 https://huggingface.co/spaces/zenafey/prodia
 
@@ -51,15 +55,14 @@
 git clone https://github.com/zenafey/prodiapy
 cd prodiapy
 python tk_gui.py
 ```
 ![image](https://github.com/zenafey/prodiapy/assets/118455214/ff949765-307a-4460-87b9-c1a255f169c9)
 
 
-[Full Documentation](https://prodiapy.readme.io/)
 
 Feel free to join out [Discord server](https://discord.gg/PtdHCVysfj) and ask question!
 
 ![7eacddcb-3a45-4114-b731-3cd7af9522e1](https://user-images.githubusercontent.com/118455214/233359979-80274381-10dd-4ced-b7fa-d45437ef5bce.png)
```

### Comparing `prodiapy-3.4/README.md` & `prodiapy-3.5/prodiapy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,49 @@
+Metadata-Version: 2.1
+Name: prodiapy
+Version: 3.5
+Summary: Prodia API Python Wrapper
+Home-page: https://github.com/zenafey/prodiapy
+Author: zenafey
+Author-email: zenafey@eugw.ru
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # prodiapy
 This module makes generation of image by Prodia API easier
 
+[Full Documentation](https://prodiapy.readme.io/)
+
 ### Installation 
 ```
-pip install prodiapy==3.4
+pip install prodiapy==3.5
 ```
 For using this script you need to get your Prodia api key, you can make it on https://app.prodia.com/api
 
 
 ### Example of txt2img usage
 ```python
-import prodia
+from prodia import Client, Model
 
 key = "your-prodia-key"
 
-client = prodia.Client(api_key=key)
+client = Client(api_key=key)
 
-image = client.txt2img(prompt="kittens on cloud", model="dreamlike-diffusion-2.0.safetensors [fdcf65e7]")
+image = client.txt2img(prompt="kittens on cloud", model="Realistic_Vision_V4.0.safetensors [29a7afaa]")
 print(image.url)
 ```
-`image` variable will be a class with attributes:
+`image` class attributes:
 
 - url - url of generated image
 - payload - used payload
 - response - retrieved response
 - seed() - function that return seed of generated image
 - pnginfo() - function that return a dict with pnginfo of image
+- load()/ aload() - function to get image as BytesIO and its async version
 
 
 
 # HuggingFace Demo
 
 https://huggingface.co/spaces/zenafey/prodia
 
@@ -41,15 +55,14 @@
 git clone https://github.com/zenafey/prodiapy
 cd prodiapy
 python tk_gui.py
 ```
 ![image](https://github.com/zenafey/prodiapy/assets/118455214/ff949765-307a-4460-87b9-c1a255f169c9)
 
 
-[Full Documentation](https://prodiapy.readme.io/)
 
 Feel free to join out [Discord server](https://discord.gg/PtdHCVysfj) and ask question!
 
 ![7eacddcb-3a45-4114-b731-3cd7af9522e1](https://user-images.githubusercontent.com/118455214/233359979-80274381-10dd-4ced-b7fa-d45437ef5bce.png)
```

### Comparing `prodiapy-3.4/prodia/async_prodia.py` & `prodiapy-3.5/prodia/async_prodia.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 from .constants import *
 from .utils import *
 from .exceptions import *
 from .templates import *
 import aiohttp
 import asyncio
-import time
 
 
 class AsyncClient:
-    def __init__(self, api_key: str = None, delay: int = 1):
+    def __init__(self, api_key: str = None, delay: int = 0.5):
         if api_key is None:
             raise ClientError(
                 "\n\n\nNo API key provided, please get API key from https://app.prodia.com/ and try again\nExample of usage:\n\nclient = prodia.Client(api_key='xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx')")
         self.key = api_key
-        self.base = Endpoint.base
         self.delay = delay
 
+    async def model_list(self):
+        headers = {
+            "accept": "application/json",
+            "X-Prodia-Key": self.key
+        }
+        async with aiohttp.ClientSession() as session:
+            async with session.get(Endpoint.models, headers=headers) as response:
+                if response.status != 200:
+                    error(f"Prodia API returned error({response.status})\nDetails: {response.text}")
+                    return None
+                resp_json = await response.json()
+                for model in resp_json:
+                    print(model)
+                return resp_json
+
     async def txt2img(self, model: str = Model.SD_V15.value[0], prompt: str = None,
                       negative_prompt: str = "badly drawn, blurry, low quality",
                       steps: int = 30, cfg_scale: float = 9.5, seed: int = -1, upscale: bool = False,
                       sampler: str = "DDIM", aspect_ratio: str = "square"):
         if is_empty_or_whitespace(prompt):
             raise InvalidParameter("\n\n\nPrompt cannot be empty or whitespace")
-        if validate_ratio(aspect_ratio):
-            raise InvalidParameter(
-                f"\n\n\nEntered aspect_ratio isnt valid\nvalid ratios:\n['square', 'portrait', 'landscape']\nYou provided: {aspect_ratio}")
         if validate_sampler(sampler):
-            warn(
-                f"The sampler you used probably does not exist\nYour sampler: {sampler}\nAvailable: {[v.value[0] for v in Sampler]}")
+            warn(f"The sampler you used probably does not exist\nYour sampler: {sampler}\nAvailable: {[v.value for v in Sampler]}")
         if validate_model(model):
-            warn(f"The model you used probably does not exist\nYour model: {model}")
-        if validate_steps(steps):
-            raise InvalidParameter(f"\n\n\nsteps must be between 1 and 50\nYour value: {steps}")
-        if validate_cfg(cfg_scale):
-            raise InvalidParameter(f"\n\n\ncfg_scale must be between 1.0 and 20.0\nYour value: {cfg_scale}")
-        if "bool" not in str(type(upscale)):
-            raise InvalidParameter("\n\n\nupscale value must be boolean:\nTrue, False")
+            warn(f"The model you used probably does not exist, check available models list by using client.model_list()\nYour model: {model}")
         payload = {
             "prompt": prompt,
             "model": model,
             "sampler": sampler,
             "negative_prompt": negative_prompt,
             "steps": steps,
             "cfg_scale": cfg_scale,
@@ -52,75 +55,62 @@
             "content-type": "application/json",
             "X-Prodia-Key": self.key
         }
         headers_retrieve = {
             "accept": "application/json",
             "X-Prodia-Key": self.key
         }
-        start_time = time.time()
+        start = asyncio.get_event_loop().time()
         print(f"txt2img with params: {payload}")
 
         async with aiohttp.ClientSession() as session:
-            async with session.post(self.base+"/job", json=payload, headers=headers_create) as response:
-                try:
-                    response_json = await response.json()
-                    job_id = response_json['job']
-                except Exception as e:
-                    if response.status == 400:
-                        raise InvalidParameter(
-                            f"\n\n\nProdia API raised Invalid Generation Parameters error(400), check payload for None or invalid parameters\n\nResponse:\n\n{response.text}")
-                    else:
-                        raise UnknownError(
-                            f"\n\n\nProdia API returned unknown error: {e}\n\nResponse:\n\n{response.text}")
+            async with session.post(Endpoint.txt2img, json=payload, headers=headers_create) as response:
+                if response.status != 200:
+                    error(f"Prodia API returned error({response.status})\nDetails: {response.text}")
+                    return None
+
+                response_json = await response.json()
+                job_id = response_json['job']
 
                 await asyncio.sleep(self.delay)
 
                 while True:
-                    elapsed_time = time.time() - start_time
+                    elapsed_time = asyncio.get_event_loop().time() - start
                     print(f"txt2img time elapsed: {elapsed_time:.2f}", end="\r")
-                    async with session.get(self.base + f"/job/{job_id}", headers=headers_retrieve) as response_retrieve:
-                        try:
-                            response_retrieve_json = await response_retrieve.json()
-                            status = response_retrieve_json['status']
-                        except Exception as e:
-                            if response_retrieve.text == "Invalid Generation Parameters":
-                                raise InvalidParameter(
-                                    f"\n\n\nProdia API raise Invalid Generation Parameters error, check payload for None or invalid parameters\n\nResponse:\n\n{response_retrieve.text}")
-                            else:
-                                raise UnknownError(f"\n\n\nProdia API returned unknown error: {e}\n\nResponse:\n\n{response_retrieve.text}")
+                    async with session.get(Endpoint.retrieve.format(job_id), headers=headers_retrieve) as response_retrieve:
+                        if response_retrieve.status != 200:
+                            error(f"Prodia API returned error({response_retrieve.status})\nDetails: {response_retrieve.text}")
+                            return None
+
+                        response_retrieve_json = await response_retrieve.json()
+                        status = response_retrieve_json['status']
+
                         if status == "succeeded":
                             print(f"\nImage {job_id} generated!")
                             image_url = response_retrieve_json['imageUrl']
-                            return ProdiaResponse(image_url, payload, response_retrieve_json)
+                            return ProdiaResponse(image_url, payload, response_retrieve_json, elapsed_time)
                         elif status == "queued":
                             await asyncio.sleep(self.delay)
                         elif status == "generating":
                             await asyncio.sleep(self.delay)
                         else:
                             failed(f"\nGeneration of {job_id} failed or another error occurred: {status}")
-                            return status
+                            return ProdiaFailed
     async def img2img(self, imageUrl:str=None, model: str = Model.SD_V15.value[0], prompt:str=None, negative_prompt:str="badly drawn, blurry, low quality",
                       steps:int=30, denoising_strength:float=0.5, cfg_scale:float=9.5, seed:int=-1, upscale:bool=False, sampler: str = "DDIM"):
         if is_empty_or_whitespace(prompt):
             raise InvalidParameter("\n\n\nPrompt cannot be empty or whitespace")
+        warn("Make sure that you used right url")
         if imageUrl is None:
             error("imageUrl not specified")
             return
         if validate_sampler(sampler):
-            warn(f"The sampler you used probably does not exist\nYour sampler: {sampler}\nAvailable: {[v.value[0] for v in Sampler]}")
+            warn(f"The sampler you used probably does not exist\nYour sampler: {sampler}\nAvailable: {[v.value for v in Sampler]}")
         if validate_model(model):
-            warn(f"The model you used probably does not exist\nYour model: {model}")
-        if validate_steps(steps):
-            raise InvalidParameter(f"\n\n\nSteps must be between 1 and 50\nYour value: {steps}")
-        if validate_cfg(cfg_scale):
-            raise InvalidParameter(f"\n\n\nCFG scale must be between 1.0 and 20.0\nYour value: {cfg_scale}")
-        if validate_denoise(denoising_strength):
-            raise InvalidParameter(f"\n\n\nDenoising Strength must be between 0.1 and 0.9\nYour value: {denoising_strength}")
-        if "bool" not in str(type(upscale)):
-            raise InvalidParameter("\n\n\nUpscale value must be boolean:\nTrue, False")
+            warn(f"The model you used probably does not exist, check available models list by using client.model_list()\nYour model: {model}")
         payload = {
             "imageUrl": imageUrl,
             "prompt": prompt,
             "model": model,
             "sampler": sampler,
             "negative_prompt": negative_prompt,
             "steps": steps,
@@ -134,94 +124,70 @@
             "content-type": "application/json",
             "X-Prodia-Key": self.key
         }
         headers_retrieve = {
             "accept": "application/json",
             "X-Prodia-Key": self.key
         }
-        start_time = time.time()
+        start = asyncio.get_event_loop().time()
         print(f"img2img with params:\n{payload}")
 
         async with aiohttp.ClientSession() as session:
-            async with session.post(self.base+"/transform", json=payload, headers=headers_create) as response:
-                try:
-                    response_json = await response.json()
-                    job_id = response_json['job']
-                except Exception as e:
-                    if response.status == 400:
-                        raise InvalidParameter(
-                            f"\n\n\nProdia API raised Invalid Generation Parameters error(400), check payload for None or invalid parameters\n\nResponse:\n\n{response.text}")
-                    else:
-                        raise UnknownError(
-                            f"\n\n\nProdia API returned unknown error: {e}\n\nResponse:\n\n{response.text}")
+            async with session.post(Endpoint.img2img, json=payload, headers=headers_create) as response:
+                if response.status != 200:
+                    error(f"Prodia API returned error({response.status})\nDetails: {response.text}")
+                    return None
+
+                response_json = await response.json()
+                job_id = response_json['job']
 
                 await asyncio.sleep(self.delay)
 
                 while True:
-                    elapsed_time = time.time() - start_time
+                    elapsed_time = asyncio.get_event_loop().time() - start
                     print(f"img2img time elapsed: {elapsed_time:.2f}", end="\r")
-                    async with session.get(self.base + f"/job/{job_id}", headers=headers_retrieve) as response_retrieve:
-                        try:
-                            response_retrieve_json = await response_retrieve.json()
-                            status = response_retrieve_json['status']
-                        except Exception as e:
-                            if response_retrieve.text == "Invalid Generation Parameters":
-                                raise InvalidParameter(
-                                    f"\n\n\nProdia API raise Invalid Generation Parameters error, check payload for None or invalid parameters\n\nResponse:\n\n{response_retrieve.text}")
-                            else:
-                                raise UnknownError(
-                                    f"\n\n\nProdia API returned unknown error: {e}\n\nResponse:\n\n{response_retrieve.text}")
+                    async with session.get(Endpoint.retrieve.format(job_id), headers=headers_retrieve) as response_retrieve:
+                        if response_retrieve.status != 200:
+                            error(f"\nProdia API returned error({response_retrieve.status})\nDetails: {response_retrieve.text}")
+                            return None
+
+                        response_retrieve_json = await response_retrieve.json()
+                        status = response_retrieve_json['status']
+
                         if status == "succeeded":
                             print(f"\nImage {job_id} generated!")
                             image_url = response_retrieve_json['imageUrl']
-                            return ProdiaResponse(image_url, payload, response_retrieve_json)
+                            return ProdiaResponse(image_url, payload, response_retrieve_json, elapsed_time)
                         elif status == "queued":
                             await asyncio.sleep(self.delay)
                         elif status == "generating":
                             await asyncio.sleep(self.delay)
                         else:
                             failed(f"\nGeneration of {job_id} failed or another error occurred: {status}")
-                            return status
+                            return ProdiaFailed
 
 
-        ###DEPRECATED###
-
-    async def controlnet(self, imageUrl:str=None, model: Model = Model.REALISTICVS_V14, controlnet_model: Control = Control.CANNY, prompt:str=None, negative_prompt:str="badly drawn, blurry, low quality",
-                      steps:int=30, cfg_scale:float=9.5, seed:int=-1, sampler: Sampler = Sampler.DDIM):
+    async def controlnet(self, imageUrl:str=None, model: Model = Model.SD_V15.value[0], controlnet_model: Control = Control.SOFT_EDGE.value[0], prompt:str=None, negative_prompt:str="badly drawn, blurry, low quality",
+                      steps:int=30, cfg_scale:float=9.5, seed:int=-1, sampler: str = "DDIM"):
         warn("THIS METHOD IS BETA AND UNSTABLE! USE IT AT YOUR OWN RISK")
         warn("Make sure that you used right url")
         if imageUrl is None:
             error("imageUrl not specified")
             return
         if is_empty_or_whitespace(prompt):
             raise InvalidParameter("\n\n\nPrompt cannot be empty or whitespace")
         if validate_sampler(sampler):
-            warn(f"The sampler you used probably does not exist\nYour sampler: {sampler}\nAvailable: {[v.value[0] for v in Sampler]}")
+            warn(f"The sampler you used probably does not exist\nYour sampler: {sampler}\nAvailable: {[v.value for v in Sampler]}")
         if validate_model(model):
             warn(f"The model you used probably does not exist\nYour model: {model}")
         if validate_control(controlnet_model):
-            warn(f"The controlnet_model you used probably does not exist\nYour model: {model}")
-        if validate_steps(steps):
-            raise InvalidParameter(f"\n\n\nSteps must be between 1 and 50\nYour value: {steps}")
-        if validate_cfg(cfg_scale):
-            raise InvalidParameter(f"\n\n\nCFG scale must be between 1.0 and 20.0\nYour value: {steps}")
-        try:
-            model = model.value[0]
-        except:
-            model = model
-        try:
-            controlnet_model = controlnet_model.value[0]
-        except:
-            controlnet_model = controlnet_model
-        try:
-            sampler = sampler.value[0]
-        except:
-            sampler = sampler
+            warn(f"The controlnet_model you used probably does not exist, check available models list by using client.model_list()\nYour model: {model}")
+
         payload = {
-            "imageUrl":imageUrl,
+            "imageUrl": imageUrl,
             "prompt": prompt,
             "model": model,
             "controlnet_model": controlnet_model,
             "sampler": sampler,
             "negative_prompt": negative_prompt,
             "steps": steps,
             "cfg_scale": cfg_scale,
@@ -232,46 +198,45 @@
             "content-type": "application/json",
             "X-Prodia-Key": self.key
         }
         headers_retrieve = {
             "accept": "application/json",
             "X-Prodia-Key": self.key
         }
+        start = asyncio.get_event_loop().time()
         print(f"controlnet with params:\n{payload}")
-        response = requests.post(self.base + "/controlnet", json=payload, headers=headers_create)
-        try:
-            job_id = response.json()['job']
-        except Exception as e:
-            if response.text == "Invalid Generation Parameters":
-                raise InvalidParameter(f"\n\n\nProdia API raise Invalid Generation Parameters error, check payload for None or invalid parameters\n\nResponse:\n\n{response.text}")
-            else:
-                raise UnknownError(f"\n\n\nProdia API returned unknown error: {e}\n\nResponse:\n\n{response.text}")
-        await asyncio.sleep(3)
-
-        working = True
-        while working is True:
-            response_retrieve = requests.get(self.base +f"/job/{job_id}", headers=headers_retrieve)
-            try:
-                status = response_retrieve.json()['status']
-            except Exception as e:
-                if response_retrieve.text == "Invalid Generation Parameters":
-                    raise InvalidParameter(
-                        f"\n\n\nProdia API raise Invalid Generation Parameters error, check payload for None or invalid parameters\n\nResponse:\n\n{response_retrieve.text}")
-                else:
-                    raise UnknownError(f"\n\n\nProdia API returned unknown error: {e}\n\nResponse:\n\n{response_retrieve.text}")
-            if status == "succeeded":
-                print(f"Image {job_id} generated!")
-                image_url = response_retrieve.json()['imageUrl']
-                class prodia_response:
-                    url = image_url
-                    seed = get_seed(image_url)
-                    pnginfo = get_pnginfo(image_url)
-                return prodia_response
-            elif status == "queued":
-                print("Still working...")
-                await asyncio.sleep(2)
-            elif status == "generating":
-                print("Still working...")
-                await asyncio.sleep(2)
-            else:
-                failed(f"Generation of {job_id} failed or another error occurred: {status}")
-                return status
+
+        async with aiohttp.ClientSession() as session:
+            async with session.post(Endpoint.controlnet, json=payload, headers=headers_create) as response:
+                if response.status != 200:
+                    error(f"Prodia API returned error({response.status})\nDetails: {response.text}")
+                    return None
+
+                response_json = await response.json()
+                job_id = response_json['job']
+
+                await asyncio.sleep(self.delay)
+
+                while True:
+                    elapsed_time = asyncio.get_event_loop().time() - start
+                    print(f"controlnet time elapsed: {elapsed_time:.2f}", end="\r")
+                    async with session.get(Endpoint.retrieve.format(job_id),
+                                           headers=headers_retrieve) as response_retrieve:
+                        if response_retrieve.status != 200:
+                            error(
+                                f"\nProdia API returned error({response_retrieve.status})\nDetails: {response_retrieve.text}")
+                            return None
+
+                        response_retrieve_json = await response_retrieve.json()
+                        status = response_retrieve_json['status']
+
+                        if status == "succeeded":
+                            print(f"\nImage {job_id} generated!")
+                            image_url = response_retrieve_json['imageUrl']
+                            return ProdiaResponse(image_url, payload, response_retrieve_json, elapsed_time)
+                        elif status == "queued":
+                            await asyncio.sleep(self.delay)
+                        elif status == "generating":
+                            await asyncio.sleep(self.delay)
+                        else:
+                            failed(f"\nGeneration of {job_id} failed or another error occurred: {status}")
+                            return ProdiaFailed
```

### Comparing `prodiapy-3.4/prodia/utils.py` & `prodiapy-3.5/prodia/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -30,71 +30,45 @@
         f.write(response.content)
 
 def is_empty_or_whitespace(s):
     if s is None:
         return True
     return all(c.isspace() for c in s)
 
-def validate_ratio(ratio):
-    if ratio not in [ratio for ratio in Ratio] and ratio not in [ratio.value[0] for ratio in Ratio]:
-        return True
-    else:
-        return False
+
 
 def validate_sampler(sampler):
-    if sampler not in [v for v in Sampler] and sampler not in [v.value[0] for v in Sampler]:
+    if sampler not in [v.value for v in Sampler]:
         return True
     else:
         return False
 
 def validate_model(model):
-    if model not in [v for v in Model] and model not in [v.value[0] for v in Model]:
+    if model not in [v.value[0] for v in Model]:
         return True
     else:
         return False
 
 def validate_control(model):
-    if model not in [v for v in Control] and model not in [v.value[0] for v in Control]:
-        return True
-    else:
-        return False
-
-
-def validate_steps(steps):
-    if steps < 1 or steps > 50:
-        return True
-    else:
-        return False
-
-def validate_cfg(cfg_scale):
-    if cfg_scale < 1.0 or cfg_scale > 20.0:
-        return True
-    else:
-        return False
-
-def validate_denoise(ds):
-    if ds < 0.1 or ds > 0.9:
+    if model not in [v.value[0] for v in Control]:
         return True
     else:
         return False
 
 def error(msg):
     print(Fore.RED + f"ERROR: {msg}" + Fore.RESET)
 
 def warn(msg):
     print(Fore.YELLOW + f"WARNING: {msg}" + Fore.RESET)
 
 def failed(msg):
     print(Fore.RED + f"FAILED: {msg}" + Fore.RESET)
 
-def models():
-    for model in Model:
-        print(f"{model.value[0]} - {model.value[1]} - {model.value[2]}")
 
 def controlnet_models():
     for model in Control:
         print(f"{model.value[0]} - {model.value[1]} - {model.value[2]}")
 
 def samplers():
     for sampler in Sampler:
-        print(f"{sampler.value[0]} - {sampler.value[1]}")
+        print(f"{sampler.value}")
```

### Comparing `prodiapy-3.4/prodiapy.egg-info/PKG-INFO` & `prodiapy-3.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,38 @@
-Metadata-Version: 2.1
-Name: prodiapy
-Version: 3.4
-Summary: Prodia API Python Wrapper
-Author: zenafey
-Author-email: zenafey@eugw.ru
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # prodiapy
 This module makes generation of image by Prodia API easier
 
+[Full Documentation](https://prodiapy.readme.io/)
+
 ### Installation 
 ```
-pip install prodiapy==3.4
+pip install prodiapy==3.5
 ```
 For using this script you need to get your Prodia api key, you can make it on https://app.prodia.com/api
 
 
 ### Example of txt2img usage
 ```python
-import prodia
+from prodia import Client, Model
 
 key = "your-prodia-key"
 
-client = prodia.Client(api_key=key)
+client = Client(api_key=key)
 
-image = client.txt2img(prompt="kittens on cloud", model="dreamlike-diffusion-2.0.safetensors [fdcf65e7]")
+image = client.txt2img(prompt="kittens on cloud", model="Realistic_Vision_V4.0.safetensors [29a7afaa]")
 print(image.url)
 ```
-`image` variable will be a class with attributes:
+`image` class attributes:
 
 - url - url of generated image
 - payload - used payload
 - response - retrieved response
 - seed() - function that return seed of generated image
 - pnginfo() - function that return a dict with pnginfo of image
+- load()/ aload() - function to get image as BytesIO and its async version
 
 
 
 # HuggingFace Demo
 
 https://huggingface.co/spaces/zenafey/prodia
 
@@ -51,15 +44,14 @@
 git clone https://github.com/zenafey/prodiapy
 cd prodiapy
 python tk_gui.py
 ```
 ![image](https://github.com/zenafey/prodiapy/assets/118455214/ff949765-307a-4460-87b9-c1a255f169c9)
 
 
-[Full Documentation](https://prodiapy.readme.io/)
 
 Feel free to join out [Discord server](https://discord.gg/PtdHCVysfj) and ask question!
 
 ![7eacddcb-3a45-4114-b731-3cd7af9522e1](https://user-images.githubusercontent.com/118455214/233359979-80274381-10dd-4ced-b7fa-d45437ef5bce.png)
```

