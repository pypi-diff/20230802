# Comparing `tmp/neon-phal-plugin-reset-0.2.2a1.tar.gz` & `tmp/neon-phal-plugin-reset-0.2.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-phal-plugin-reset-0.2.2a1.tar", last modified: Fri Jul 28 23:21:16 2023, max compression
+gzip compressed data, was "neon-phal-plugin-reset-0.2.2a2.tar", last modified: Wed Aug  2 18:39:31 2023, max compression
```

## Comparing `neon-phal-plugin-reset-0.2.2a1.tar` & `neon-phal-plugin-reset-0.2.2a2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:21:16.666323 neon-phal-plugin-reset-0.2.2a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-28 23:21:12.000000 neon-phal-plugin-reset-0.2.2a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-28 23:21:12.000000 neon-phal-plugin-reset-0.2.2a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-28 23:21:16.666323 neon-phal-plugin-reset-0.2.2a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-28 23:21:12.000000 neon-phal-plugin-reset-0.2.2a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:21:16.666323 neon-phal-plugin-reset-0.2.2a1/neon_phal_plugin_reset/
--rw-r--r--   0 runner    (1001) docker     (123)    14765 2023-07-28 23:21:12.000000 neon-phal-plugin-reset-0.2.2a1/neon_phal_plugin_reset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-28 23:21:12.000000 neon-phal-plugin-reset-0.2.2a1/neon_phal_plugin_reset/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-07-28 23:21:12.000000 neon-phal-plugin-reset-0.2.2a1/neon_phal_plugin_reset/create_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-28 23:21:12.000000 neon-phal-plugin-reset-0.2.2a1/neon_phal_plugin_reset/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:21:16.666323 neon-phal-plugin-reset-0.2.2a1/neon_phal_plugin_reset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-28 23:21:16.000000 neon-phal-plugin-reset-0.2.2a1/neon_phal_plugin_reset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-28 23:21:16.000000 neon-phal-plugin-reset-0.2.2a1/neon_phal_plugin_reset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 23:21:16.000000 neon-phal-plugin-reset-0.2.2a1/neon_phal_plugin_reset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-28 23:21:16.000000 neon-phal-plugin-reset-0.2.2a1/neon_phal_plugin_reset.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-28 23:21:16.000000 neon-phal-plugin-reset-0.2.2a1/neon_phal_plugin_reset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 23:21:16.000000 neon-phal-plugin-reset-0.2.2a1/neon_phal_plugin_reset.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:21:16.666323 neon-phal-plugin-reset-0.2.2a1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-28 23:21:12.000000 neon-phal-plugin-reset-0.2.2a1/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 23:21:16.666323 neon-phal-plugin-reset-0.2.2a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-07-28 23:21:12.000000 neon-phal-plugin-reset-0.2.2a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:39:31.078090 neon-phal-plugin-reset-0.2.2a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-08-02 18:39:27.000000 neon-phal-plugin-reset-0.2.2a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 18:39:27.000000 neon-phal-plugin-reset-0.2.2a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-02 18:39:31.078090 neon-phal-plugin-reset-0.2.2a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-08-02 18:39:27.000000 neon-phal-plugin-reset-0.2.2a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:39:31.074089 neon-phal-plugin-reset-0.2.2a2/neon_phal_plugin_reset/
+-rw-r--r--   0 runner    (1001) docker     (123)    14765 2023-08-02 18:39:27.000000 neon-phal-plugin-reset-0.2.2a2/neon_phal_plugin_reset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-08-02 18:39:27.000000 neon-phal-plugin-reset-0.2.2a2/neon_phal_plugin_reset/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-08-02 18:39:27.000000 neon-phal-plugin-reset-0.2.2a2/neon_phal_plugin_reset/create_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-08-02 18:39:27.000000 neon-phal-plugin-reset-0.2.2a2/neon_phal_plugin_reset/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:39:31.078090 neon-phal-plugin-reset-0.2.2a2/neon_phal_plugin_reset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-02 18:39:31.000000 neon-phal-plugin-reset-0.2.2a2/neon_phal_plugin_reset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 18:39:31.000000 neon-phal-plugin-reset-0.2.2a2/neon_phal_plugin_reset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 18:39:31.000000 neon-phal-plugin-reset-0.2.2a2/neon_phal_plugin_reset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-02 18:39:31.000000 neon-phal-plugin-reset-0.2.2a2/neon_phal_plugin_reset.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-02 18:39:31.000000 neon-phal-plugin-reset-0.2.2a2/neon_phal_plugin_reset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 18:39:31.000000 neon-phal-plugin-reset-0.2.2a2/neon_phal_plugin_reset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:39:31.078090 neon-phal-plugin-reset-0.2.2a2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-02 18:39:27.000000 neon-phal-plugin-reset-0.2.2a2/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 18:39:31.078090 neon-phal-plugin-reset-0.2.2a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-08-02 18:39:27.000000 neon-phal-plugin-reset-0.2.2a2/setup.py
```

### Comparing `neon-phal-plugin-reset-0.2.2a1/LICENSE.md` & `neon-phal-plugin-reset-0.2.2a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-reset-0.2.2a1/PKG-INFO` & `neon-phal-plugin-reset-0.2.2a2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-reset
-Version: 0.2.2a1
+Version: 0.2.2a2
 Summary: Device Reset Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-reset
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-phal-plugin-reset-0.2.2a1/README.md` & `neon-phal-plugin-reset-0.2.2a2/README.md`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-reset-0.2.2a1/neon_phal_plugin_reset/__init__.py` & `neon-phal-plugin-reset-0.2.2a2/neon_phal_plugin_reset/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-reset-0.2.2a1/neon_phal_plugin_reset/config.py` & `neon-phal-plugin-reset-0.2.2a2/neon_phal_plugin_reset/config.py`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-reset-0.2.2a1/neon_phal_plugin_reset/create_media.py` & `neon-phal-plugin-reset-0.2.2a2/neon_phal_plugin_reset/create_media.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,21 +21,22 @@
 # CONTRIBUTORS  BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-from tempfile import mkstemp
 
 import psutil
+import shutil
 
+from tempfile import mkstemp
 from subprocess import run, PIPE, Popen
-from os import close
-from os.path import exists
+from os import close, remove
+from os.path import exists, isfile
 from typing import List, Optional
 
 import requests
 from ovos_utils.log import LOG
 
 
 def get_drive_mountpoints(drive: str = "/dev/sdb") -> List[str]:
@@ -75,19 +76,23 @@
     an output file for use on low-memory systems
     """
     image_url = image_url or "https://2222.us/app/files/neon_images/pi/" \
                              "mycroft_mark_2/recommended_mark_2.img.xz"
     if not cache_file:
         fp, cache_file = mkstemp()
         close(fp)
+    download_file = f"{cache_file}.part"
     LOG.debug(f"Downloading {image_url} to {cache_file}")
     try:
         with requests.get(image_url, stream=True) as stream:
-            with open(cache_file, 'wb') as f:
+            with open(download_file, 'wb') as f:
                 for chunk in stream.iter_content(4096):
                     if chunk:
                         f.write(chunk)
+        shutil.move(download_file, cache_file)
     except Exception as e:
         LOG.exception(e)
+        if isfile(download_file):
+            remove(download_file)
         return None
     LOG.debug(f"Download Complete")
     return cache_file
```

### Comparing `neon-phal-plugin-reset-0.2.2a1/neon_phal_plugin_reset/version.py` & `neon-phal-plugin-reset-0.2.2a2/neon_phal_plugin_reset/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.2.2a1"
+__version__ = "0.2.2a2"
```

### Comparing `neon-phal-plugin-reset-0.2.2a1/neon_phal_plugin_reset.egg-info/PKG-INFO` & `neon-phal-plugin-reset-0.2.2a2/neon_phal_plugin_reset.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-reset
-Version: 0.2.2a1
+Version: 0.2.2a2
 Summary: Device Reset Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-reset
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-phal-plugin-reset-0.2.2a1/setup.py` & `neon-phal-plugin-reset-0.2.2a2/setup.py`

 * *Files identical despite different names*

