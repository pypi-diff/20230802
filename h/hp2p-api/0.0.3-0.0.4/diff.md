# Comparing `tmp/hp2p-api-0.0.3.tar.gz` & `tmp/hp2p-api-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hp2p-api-0.0.3.tar", last modified: Tue Aug  1 10:38:54 2023, max compression
+gzip compressed data, was "hp2p-api-0.0.4.tar", last modified: Wed Aug  2 10:46:11 2023, max compression
```

## Comparing `hp2p-api-0.0.3.tar` & `hp2p-api-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,27 @@
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-08-01 10:38:54.155776 hp2p-api-0.0.3/
--rw-r--r--   0 jay        (501) staff       (20)     1064 2023-06-08 04:45:47.000000 hp2p-api-0.0.3/LICENSE
--rw-r--r--   0 jay        (501) staff       (20)      345 2023-08-01 10:38:54.155660 hp2p-api-0.0.3/PKG-INFO
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-08-01 10:38:54.154811 hp2p-api-0.0.3/hp2p_api.egg-info/
--rw-r--r--   0 jay        (501) staff       (20)      345 2023-08-01 10:38:54.000000 hp2p-api-0.0.3/hp2p_api.egg-info/PKG-INFO
--rw-r--r--   0 jay        (501) staff       (20)      323 2023-08-01 10:38:54.000000 hp2p-api-0.0.3/hp2p_api.egg-info/SOURCES.txt
--rw-r--r--   0 jay        (501) staff       (20)        1 2023-08-01 10:38:54.000000 hp2p-api-0.0.3/hp2p_api.egg-info/dependency_links.txt
--rw-r--r--   0 jay        (501) staff       (20)        1 2023-08-01 10:38:54.000000 hp2p-api-0.0.3/hp2p_api.egg-info/not-zip-safe
--rw-r--r--   0 jay        (501) staff       (20)       29 2023-08-01 10:38:54.000000 hp2p-api-0.0.3/hp2p_api.egg-info/requires.txt
--rw-r--r--   0 jay        (501) staff       (20)        8 2023-08-01 10:38:54.000000 hp2p-api-0.0.3/hp2p_api.egg-info/top_level.txt
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-08-01 10:38:54.155495 hp2p-api-0.0.3/hp2papi/
--rw-r--r--   0 jay        (501) staff       (20)     1711 2023-08-01 10:38:14.000000 hp2p-api-0.0.3/hp2papi/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)     3211 2023-08-01 05:18:29.000000 hp2p-api-0.0.3/hp2papi/api.py
--rw-r--r--   0 jay        (501) staff       (20)     6023 2023-08-01 10:35:27.000000 hp2p-api-0.0.3/hp2papi/api_func.py
--rw-r--r--   0 jay        (501) staff       (20)     3654 2023-08-01 09:48:10.000000 hp2p-api-0.0.3/hp2papi/api_pb2.py
--rw-r--r--   0 jay        (501) staff       (20)     2410 2023-08-01 10:06:45.000000 hp2p-api-0.0.3/hp2papi/api_pb2_grpc.py
--rw-r--r--   0 jay        (501) staff       (20)    16704 2023-08-01 08:58:33.000000 hp2p-api-0.0.3/hp2papi/classes.py
--rw-r--r--   0 jay        (501) staff       (20)       38 2023-08-01 10:38:54.155812 hp2p-api-0.0.3/setup.cfg
--rw-r--r--   0 jay        (501) staff       (20)      572 2023-08-01 10:38:07.000000 hp2p-api-0.0.3/setup.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-08-02 10:46:11.907966 hp2p-api-0.0.4/
+-rw-r--r--   0 jay        (501) staff       (20)     1064 2023-06-08 04:45:47.000000 hp2p-api-0.0.4/LICENSE
+-rw-r--r--   0 jay        (501) staff       (20)       49 2023-08-02 10:41:01.000000 hp2p-api-0.0.4/MANIFEST.in
+-rw-r--r--   0 jay        (501) staff       (20)      345 2023-08-02 10:46:11.907751 hp2p-api-0.0.4/PKG-INFO
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-08-02 10:46:11.898609 hp2p-api-0.0.4/hp2p_api.egg-info/
+-rw-r--r--   0 jay        (501) staff       (20)      345 2023-08-02 10:46:11.000000 hp2p-api-0.0.4/hp2p_api.egg-info/PKG-INFO
+-rw-r--r--   0 jay        (501) staff       (20)      477 2023-08-02 10:46:11.000000 hp2p-api-0.0.4/hp2p_api.egg-info/SOURCES.txt
+-rw-r--r--   0 jay        (501) staff       (20)        1 2023-08-02 10:46:11.000000 hp2p-api-0.0.4/hp2p_api.egg-info/dependency_links.txt
+-rw-r--r--   0 jay        (501) staff       (20)        1 2023-08-02 10:46:11.000000 hp2p-api-0.0.4/hp2p_api.egg-info/not-zip-safe
+-rw-r--r--   0 jay        (501) staff       (20)       29 2023-08-02 10:46:11.000000 hp2p-api-0.0.4/hp2p_api.egg-info/requires.txt
+-rw-r--r--   0 jay        (501) staff       (20)        8 2023-08-02 10:46:11.000000 hp2p-api-0.0.4/hp2p_api.egg-info/top_level.txt
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-08-02 10:46:11.899189 hp2p-api-0.0.4/hp2papi/
+-rw-r--r--   0 jay        (501) staff       (20)     1711 2023-08-02 10:42:39.000000 hp2p-api-0.0.4/hp2papi/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)     3250 2023-08-01 12:05:03.000000 hp2p-api-0.0.4/hp2papi/api.py
+-rw-r--r--   0 jay        (501) staff       (20)     6873 2023-08-02 10:46:02.000000 hp2p-api-0.0.4/hp2papi/api_func.py
+-rw-r--r--   0 jay        (501) staff       (20)    16710 2023-08-01 12:27:28.000000 hp2p-api-0.0.4/hp2papi/classes.py
+-rw-r--r--   0 jay        (501) staff       (20)     1580 2023-08-02 09:51:18.000000 hp2p-api-0.0.4/hp2papi/gRpcServicer.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-08-02 10:46:11.899569 hp2p-api-0.0.4/hp2papi/pb2/
+-rw-r--r--   0 jay        (501) staff       (20)      157 2023-08-02 09:21:23.000000 hp2p-api-0.0.4/hp2papi/pb2/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)     3833 2023-08-02 09:20:44.000000 hp2p-api-0.0.4/hp2papi/pb2/api_pb2.py
+-rw-r--r--   0 jay        (501) staff       (20)     3852 2023-08-02 09:20:44.000000 hp2p-api-0.0.4/hp2papi/pb2/api_pb2_grpc.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-08-02 10:46:11.907523 hp2p-api-0.0.4/hp2papi/peer/
+-rw-r--r--   0 jay        (501) staff       (20)      274 2023-08-02 10:16:37.000000 hp2p-api-0.0.4/hp2papi/peer/clientconfig.json
+-rwxr-xr-x   0 jay        (501) staff       (20) 11989506 2023-08-02 10:16:37.000000 hp2p-api-0.0.4/hp2papi/peer/hp2p.go.peer
+-rw-r--r--   0 jay        (501) staff       (20)      520 2023-08-02 10:16:37.000000 hp2p-api-0.0.4/hp2papi/peer/peerconfig.json
+-rw-r--r--   0 jay        (501) staff       (20)       38 2023-08-02 10:46:11.908011 hp2p-api-0.0.4/setup.cfg
+-rw-r--r--   0 jay        (501) staff       (20)      603 2023-08-02 10:42:41.000000 hp2p-api-0.0.4/setup.py
```

### Comparing `hp2p-api-0.0.3/LICENSE` & `hp2p-api-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hp2p-api-0.0.3/hp2papi/__init__.py` & `hp2p-api-0.0.4/hp2papi/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,10 +47,10 @@
 #     "ModificationRequest",
 
 #     "Creation",
 # ]
 
 __all__ = []
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 __Init()
```

### Comparing `hp2p-api-0.0.3/hp2papi/api.py` & `hp2p-api-0.0.4/hp2papi/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,19 +28,19 @@
 
 @version 0.1
 @author jaylee@jayb.kr
 """
 
 from typing import Callable
 from .classes import *
-from .api_func import __CheckRequest, __Creation, __Query, __Modification, __Join, __SearchPeer, __SendData, __Leave, __Removal, __SetNotificatonListener, __SetGrpcPort, __apapap
+from .api_func import __CheckRequest, __Creation, __Query, __Modification, __Join, __SearchPeer, __SendData, __Leave, __Removal, __SetNotificatonListener, __SetGrpcPort, __Cleanup
 
 __all__ = [
     "SetGrpcPort",
-    "apapap",
+    "Cleanup",
     "Creation",
     "Query",
     "Modification",
     "Join",
     "SearchPeer",
     "SendData",
     "Leave",
@@ -50,16 +50,19 @@
 
 def SetGrpcPort(port: int) -> None:
     """
     gRPC 포트 설정
     """
     __SetGrpcPort(port)
 
-def apapap():
-    __apapap()
+def Cleanup() -> None:
+    """
+    종료
+    """
+    __Cleanup()
 
 def Creation(req: CreationRequest) -> CreationResponse:
     """
     신규 서비스 세션 생성
     """
     return __CheckRequest(req, __Creation)
```

### Comparing `hp2p-api-0.0.3/hp2papi/api_func.py` & `hp2p-api-0.0.4/hp2papi/api_func.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,43 +17,71 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
-import sys
-aaa  = sys.path
 from .classes import *
 #from collections.abc import Callable
 from typing import Callable
 import grpc
-from .api_pb2 import *
-from .api_pb2_grpc import *
-
+from concurrent import futures
+import threading
+from .pb2 import api_pb2
+from .pb2 import api_pb2_grpc
+from .gRpcServicer import Hp2pServicer
 
 __notificationListeners = dict()
 __grpcPort = 50051
+__grpcThread = None
+__grpcServer = None
 
 def __SetGrpcPort(port: int) -> None:
     global __grpcPort
     __grpcPort = port
 
 def __GrpcStart() -> None:
-    server = grpc.aio.server(grpc.ThreadPoolExecutor(max_workers=10))
-    add_Hp2pApiProtoServicer_to_server(Hp2pApiProtoServicer(), server)
-    server.add_insecure_port('[::]:' + str(__grpcPort))
-    server.start()
+    global __grpcServer
+
+    __grpcServer = grpc.server(futures.ThreadPoolExecutor(max_workers=10))
+    api_pb2_grpc.add_Hp2pApiProtoServicer_to_server(Hp2pServicer(), __grpcServer)
+    __grpcServer.add_insecure_port('[::]:' + str(__grpcPort))
+    __grpcServer.start()
     print("Python gRPC Server is running on port " + str(__grpcPort))
-    server.wait_for_termination()
+    __grpcServer.wait_for_termination()
 
 def __Init():
-    __GrpcStart()
+    global __grpcThread
+
+    __grpcThread = threading.Thread(target=__GrpcStart)
+    __grpcThread.start()
+
     print("Peer API init.")
 
+    import subprocess, os
+
+    current_file_path = os.path.abspath(__file__)
+    current_directory = os.path.dirname(current_file_path)
+    peerpath = current_directory + "/peer/hp2p.go.peer -id peer44" 
+    rslt = subprocess.run([peerpath], capture_output=True, text=True)
+    print(rslt.stdout)
+
+def __Cleanup():
+    global __grpcThread, __grpcServer
+
+    print("gRPC Server is stopping...")
+    if __grpcThread and __grpcThread.is_alive():
+        if __grpcServer:
+            __grpcServer.stop(5)
+        __grpcThread.join()
+    print("gRPC Server is stopped.")
+
+    print("Peer API cleanup.")
+
 def __CheckRequest(req: Request, func: Callable[[Request], Response]) -> Response:
     if not req or not req.mandatoryCheck():
         return Response(ResponseCode.WrongRequest)
     
     return func(req)
 
 def __Creation(req: CreationRequest) -> CreationResponse:
```

### Comparing `hp2p-api-0.0.3/hp2papi/classes.py` & `hp2p-api-0.0.4/hp2papi/classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from typing import List
 
 __all__ = [
     "ResponseCode",
     "DataType",
     "ChannelType",
     "FeatureBasedVideoMode",
+    "FeatureBasedVideoTarget",
     "AudioCodec",
     "AudioSampleRate",
     "AudioBitrate",
     "AudioChannelType",
     "TextFormat",
     "Response",
     "OverlayClosed",
@@ -241,15 +242,15 @@
     hash: str = None
     dimension: str = None
 
     def mandatoryCheck(self) -> bool:
         if not super().mandatoryCheck():
             return False
         
-        if not _check(self.target) or len(self.target) <= 0 or self.target not in FeatureBasedVideoTarget:
+        if not _check(self.target) or self.target not in FeatureBasedVideoTarget:
             return False
 
         if not _check(self.mode) or self.mode not in FeatureBasedVideoMode:
             return False
         
         if self.mode is FeatureBasedVideoMode.KeypointsDescriptionMode:
             if not _check(self.resolution):
```

### Comparing `hp2p-api-0.0.3/setup.py` & `hp2p-api-0.0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hp2p-api',
-    version='0.0.3',
+    version='0.0.4',
     description='An API for HP2P Peer',
     author='JAYB',
     author_email='jaylee@jayb.kr',
     url='https://github.com/ITU-T-SG11-Q8/Q.4102',
     install_requires=['grpcio', 'grpcio-tools', 'protobuf',],
     packages=find_packages(exclude=[]),
+    include_package_data=True,
     keywords=['hp2p', 'hp2p-api'],
     python_requires='>=3.8',
     package_data={},
     zip_safe=False,
     classifiers=[
         'Programming Language :: Python :: 3.8',
         'License :: OSI Approved :: MIT License',
```

