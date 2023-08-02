# Comparing `tmp/IxNetwork-9.0.1915.16-py2.py3-none-any.whl.zip` & `tmp/IxNetwork-9.30.2212.7-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,13 @@
-Zip file size: 25136 bytes, number of entries: 13
--rw-r--r--  2.0 unx    10709 b- defN 19-Jul-24 22:46 IxNetwork/IxNetwork.py
--rw-r--r--  2.0 unx    22359 b- defN 19-Jul-24 22:46 IxNetwork/IxNetworkLegacy.py
--rw-r--r--  2.0 unx    47080 b- defN 19-Jul-24 22:46 IxNetwork/IxNetworkSecure.py
--rw-r--r--  2.0 unx     1173 b- defN 19-Jul-24 22:46 IxNetwork/__init__.py
--rw-r--r--  2.0 unx      122 b- defN 19-Jul-24 22:46 IxNetwork/requirements.txt
--rw-r--r--  2.0 unx     2647 b- defN 19-Jul-24 23:34 IxNetwork-9.0.1915.16.dist-info/DESCRIPTION.rst
--rw-r--r--  2.0 unx     1079 b- defN 19-Jul-24 23:34 IxNetwork-9.0.1915.16.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     1565 b- defN 19-Jul-24 23:34 IxNetwork-9.0.1915.16.dist-info/metadata.json
--rw-r--r--  2.0 unx       10 b- defN 19-Jul-24 23:34 IxNetwork-9.0.1915.16.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 19-Jul-24 23:34 IxNetwork-9.0.1915.16.dist-info/zip-safe
--rw-r--r--  2.0 unx      110 b- defN 19-Jul-24 23:34 IxNetwork-9.0.1915.16.dist-info/WHEEL
--rw-r--r--  2.0 unx     4198 b- defN 19-Jul-24 23:34 IxNetwork-9.0.1915.16.dist-info/METADATA
--rw-r--r--  2.0 unx     1156 b- defN 19-Jul-24 23:34 IxNetwork-9.0.1915.16.dist-info/RECORD
-13 files, 92209 bytes uncompressed, 23206 bytes compressed:  74.8%
+Zip file size: 23224 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat    10840 b- defN 23-Jul-27 06:41 IxNetwork/IxNetwork.py
+-rw-rw-rw-  2.0 fat    22532 b- defN 23-Jul-27 06:41 IxNetwork/IxNetworkLegacy.py
+-rw-rw-rw-  2.0 fat    47860 b- defN 23-Jul-27 06:41 IxNetwork/IxNetworkSecure.py
+-rw-rw-rw-  2.0 fat     1173 b- defN 23-Jul-27 06:41 IxNetwork/__init__.py
+-rw-rw-rw-  2.0 fat      122 b- defN 23-Jul-27 06:41 IxNetwork/requirements.txt
+-rw-rw-rw-  2.0 fat     1079 b- defN 23-Aug-02 19:38 IxNetwork-9.30.2212.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4334 b- defN 23-Aug-02 19:38 IxNetwork-9.30.2212.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Aug-02 19:38 IxNetwork-9.30.2212.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Aug-02 19:38 IxNetwork-9.30.2212.7.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Aug-02 19:38 IxNetwork-9.30.2212.7.dist-info/zip-safe
+?rw-rw-r--  2.0 fat      933 b- defN 23-Aug-02 19:38 IxNetwork-9.30.2212.7.dist-info/RECORD
+11 files, 88995 bytes uncompressed, 21638 bytes compressed:  75.7%
```

## zipnote {}

```diff
@@ -9,32 +9,26 @@
 
 Filename: IxNetwork/__init__.py
 Comment: 
 
 Filename: IxNetwork/requirements.txt
 Comment: 
 
-Filename: IxNetwork-9.0.1915.16.dist-info/DESCRIPTION.rst
+Filename: IxNetwork-9.30.2212.7.dist-info/LICENSE
 Comment: 
 
-Filename: IxNetwork-9.0.1915.16.dist-info/LICENSE.txt
+Filename: IxNetwork-9.30.2212.7.dist-info/METADATA
 Comment: 
 
-Filename: IxNetwork-9.0.1915.16.dist-info/metadata.json
+Filename: IxNetwork-9.30.2212.7.dist-info/WHEEL
 Comment: 
 
-Filename: IxNetwork-9.0.1915.16.dist-info/top_level.txt
+Filename: IxNetwork-9.30.2212.7.dist-info/top_level.txt
 Comment: 
 
-Filename: IxNetwork-9.0.1915.16.dist-info/zip-safe
+Filename: IxNetwork-9.30.2212.7.dist-info/zip-safe
 Comment: 
 
-Filename: IxNetwork-9.0.1915.16.dist-info/WHEEL
-Comment: 
-
-Filename: IxNetwork-9.0.1915.16.dist-info/METADATA
-Comment: 
-
-Filename: IxNetwork-9.0.1915.16.dist-info/RECORD
+Filename: IxNetwork-9.30.2212.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## IxNetwork/IxNetwork.py

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# Copyright 1997 - 2019 by IXIA Keysight
+# Copyright 1997 - 2023 by IXIA Keysight
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
@@ -26,25 +26,30 @@
 import socket
 import select
 from datetime import datetime
 
 class IxNetError(Exception):
     '''Default IxNet error'''
 
+def major(ver):
+    major1 = ver.split(".")[0]
+    major2 = ver.split(".")[1]
+    #return ver
+    return major1 + "." + major2
 
 from . import IxNetworkLegacy
 
 
 class IxNet(object):
     """
     Set the IxNet object up
     """
 
     def __init__(self):
-        self._version = '9.00.1915.16'
+        self._version = '9.30.2212.7'
         self.OK = '::ixNet::OK'
         self.ERROR = '::ixNet::ERROR'
         self._transportType = None
         self.__ixNetworkSecure = None
         self._noApiKey = '00000000000000000000000000000000'
         self.__ixNetworkLegacy = IxNetworkLegacy.IxNet()
         self._debug = None
```

## IxNetwork/IxNetworkLegacy.py

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# Copyright 1997 - 2019 by IXIA Keysight
+# Copyright 1997 - 2023 by IXIA Keysight
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
@@ -61,15 +61,15 @@
         self._decoratedResult = list()
         self._filename = None
         self._debug = False
         self._async = False
         self._timeout = None
         self._transportType = 'TclSocket'
         self._OK = '::ixNet::OK'
-        self._version = '9.00.1915.16'
+        self._version = '9.30.2212.7'
 
     def setDebug(self, debug):
         self._debug = debug
         return self
 
     def getRoot(self):
         return self._root
@@ -166,15 +166,18 @@
                 elif name is not None:
                     nameValuePairs[name] = str(arg)
                     name = None
             if '-port' not in nameValuePairs:
                 nameValuePairs['-port'] = 8009
             port = int(nameValuePairs['-port'])
 
-            options = '-clientusername ' + getpass.getuser()
+            if '-clientusername' in nameValuePairs:
+                options = '-clientusername ' +  nameValuePairs['-clientusername']
+            else:
+                options = '-clientusername ' + getpass.getuser()
             if '-serverusername' in nameValuePairs:
                 options += ' -serverusername ' + nameValuePairs['-serverusername']
                 serverusername = nameValuePairs['-serverusername']
             if '-connectTimeout' in nameValuePairs:
                 options += ' -connectTimeout ' + nameValuePairs['-connectTimeout']
             if '-applicationVersion' in nameValuePairs:
                 options += ' -applicationVersion ' + nameValuePairs['-applicationVersion']
@@ -540,15 +543,15 @@
             except :
                 self._decoratedResult[0] = self._decoratedResult[0].replace('\01', '').replace('\r\\n', '')
                 return eval(''.join(self._decoratedResult))
         else:
             return ''.join(self._decoratedResult)
 
     def _CheckClientVersion(self):
-        if self._version != self.getVersion():
+        if  major(self._version) != major(self.getVersion()):
             print('WARNING: IxNetwork Python library version {0} is not matching the IxNetwork client version {1}'.format(self._version, self.getVersion()))
 
 
     def _log(self, msg):
         if self._debug:
             dt = datetime.now().strftime("%a %b %d %X %Y")
             if (len(msg) > 1024):
```

## IxNetwork/IxNetworkSecure.py

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# Copyright 1997 - 2019 by IXIA Keysight
+# Copyright 1997 - 2023 by IXIA Keysight
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
@@ -94,14 +94,15 @@
     raise ImportError('Cannot load required dependencies: {0}.\nPlease run pip install -r requirements.txt.'.format(', '.join(missingDependencies)))
 missingDependencies = None
 
 try: unicode = unicode
 except NameError: unicode = str
 
 from .IxNetwork import IxNetError 
+from .IxNetwork import major
 
 class IxNetAuthenticationError(Exception):
     '''IxNet authentication error'''
 
 class IxNet(object):
     """
     Set the IxNet object up
@@ -123,15 +124,15 @@
         self._buffer = False
         self._sendBuffer = list()
         self._decoratedResult = list()
         self._noApiKey = '00000000000000000000000000000000'
         self._async = False
         self._timeout = None
         self._transportType = 'WebSocket'
-        self._version = '9.00.1915.16'
+        self._version = '9.30.2212.7'
         self.OK = '::ixNet::OK'
         self.ERROR = '::ixNet::ERROR'
         self.VERIFY_CERT = False
         # session parameters
         self._connectionInfo = {
             'port': None,
             'verb': None,
@@ -189,15 +190,15 @@
                 username = args[0]
                 password = args[1]
         else:
             username = sessionArgs['-username']
             password = sessionArgs['-password']
 
         try:
-            auth = self._restSend('POST', url, payload={'username': username, 'password': password}, timeout=180)
+            auth = self._restSend('POST', url, payload={'username': username, 'password': password, 'ignorePolicy': True}, timeout=180)
         except IxNetAuthenticationError:
             e = sys.exc_info()[1]
             msg = 'Unable to get API key from {host}:{port}. Error: IxNetAuthenticationError: {err}.\n'.format(host=hostname, port=port, err=e.args[0])
             msg += 'Please check the getApiKey command arguments.\n '
             msg += 'An example of a correct method call is:\n\t'
             msg += 'ixNet.getApiKey(<hostname>, "-username", <username>, "-password", <password> [,"-port", <443>] [, "-apiKeyFile", <api.key>])'
             raise IxNetError(msg)
@@ -323,15 +324,16 @@
             '-version': '5.30',
             '-connectTimeout': 450,
             '-allowOnlyOneConnection': False,
             '-apiKey': '',
             '-apiKeyFile': 'api.key',
             '-product': 'ixnrest',
             '-clientusername' : getpass.getuser(),
-            '-serverusername': None
+            '-serverusername': None,
+            '-heartBeat': 'true',
         }
 
         connectArgs = self._getArgMap(default_args, *args)
         connectArgs['-sessionId'] = int(connectArgs['-sessionId'])
         connectArgs['-connectTimeout'] = int(connectArgs['-connectTimeout'])
         connectArgs['-allowOnlyOneConnection'] = self._parseAsBool(connectArgs['-allowOnlyOneConnection'])
 
@@ -429,14 +431,15 @@
             self._websocket.settimeout(900)
             result = self._sendRecv('ixNet', 'connect',
                 '-version', connectArgs['-version'],
                 '-clientType', 'python',
                 '-clientId', connectArgs.get('-clientId'),
                 '-closeServerOnDisconnect', closeServerOnDisconnectBool,
                 '-clientUsername', connectArgs['-clientusername'],
+                '-heartBeat', connectArgs['-heartBeat'],
                 '-apiKey', self._headers['X-Api-Key'])
 
             self._checkClientVersion()
 
             return result
         except:
             e = sys.exc_info()[1]
@@ -617,15 +620,15 @@
         self._connectionInfo['verb'] = verb
 
         self._connectionInfo['wsVerb'] = ''
         if verb == 'http':
             self._connectionInfo['wsVerb'] = 'ws' 
         else:
             self._connectionInfo['wsVerb'] = 'wss'
-        m = re.match('\[(?P<hostname>.*)\]', hostname)
+        m = re.match(r'\[(?P<hostname>.*)\]', hostname)
         if m:
             self._connectionInfo['hostname'] = m.group('hostname')
         else:
             self._connectionInfo['hostname'] = hostname
         self._connectionInfo['port'] = port
         self._connectionInfo['url'] = url
 
@@ -638,15 +641,15 @@
         attempts = 0
         for connectionParams in params:
             url = self._createUrl(connectionParams[0], hostname, connectionParams[1])
 
             try:
                 url = self._restGetRedirect(url, timeout=30)
                 if store:
-                    m = re.match('(?P<verb>https?)://(?P<hostname>[^/]+):(?P<port>\d+)', url)
+                    m = re.match(r'(?P<verb>https?)://(?P<hostname>[^/]+):(?P<port>\d+)', url)
                     if m:
                         port = m.group('port')
                     else:
                         m = re.match('(?P<verb>https?)://(?P<hostname>[^/:]+)', url)
                         port = 443
                         if m.group('verb') == 'http':
                             port = 80  
@@ -934,30 +937,47 @@
             return self.OK
         else:
             return self._recv()
 
     def _send(self, content):
         try:
             if type(content) is str:
+                self._log("sendin = %s " %(content))    
                 content = content.encode('ascii')
             self._websocket.send(content)
         except (Exception):
             e = sys.exc_info()[1]
             self._close()
             raise IxNetError('Connection to the remote IxNetwork instance has been closed:' + str(e))
 
     def _recv(self):
         self._decoratedResult = list()
         responseBuffer = str()
+
+        # Heart beat message trap here .
+        try :
+            while True :
+                responseBuffer = self._websocket.recv()
+                if responseBuffer not in ['<0010><0100>', b'<0010><0100>']:
+                    break
+                else :
+                    self._log("got heart beat message ...")
+            # end while
+        except :
+            self._log("warning! error in mesage heart beat message processing ...")
+            pass
+        # end of heartbeat message processing             
+    
         try:
-            responseBuffer = self._websocket.recv().decode('ascii')
+            responseBuffer = responseBuffer.decode('ascii')
         except:
             e = sys.exc_info()[1]
             self._close()
             raise IxNetError('Connection to the remote IxNetwork instance has been closed:' + str(e))
+
         try:
             commandId = None
             contentLength = int(0)
             while len(responseBuffer) > 0:
                 startIndex = int(responseBuffer.find('<'))
                 stopIndex = int(responseBuffer.find('>'))
                 if startIndex != -1 and stopIndex != -1:
@@ -982,14 +1002,15 @@
                         self._restSend('GET', file_url, fid=fid)
                     finally:
                         if fid is not None:
                             fid.close()
                 elif commandId == 9:
                     self._decoratedResult = responseBuffer[stopIndex : stopIndex + contentLength]
                 responseBuffer = responseBuffer[stopIndex + contentLength :]
+            # end while
         except:
             e = sys.exc_info()[1]
             raise IxNetError(self._formatAsIxNetError(str(e)))
         self._log(' '.join(['Received:', ''.join(self._decoratedResult)]))
 
         if self._evalResult == self._evalError:
             raise IxNetError(''.join(self._decoratedResult))
@@ -997,15 +1018,15 @@
         if len(self._decoratedResult) > 0 and self._decoratedResult[0].startswith('\01'):
             return eval(''.join(self._decoratedResult[1:]))
         else:
             return ''.join(self._decoratedResult)
 
     def _checkClientVersion(self):
         version = self.getVersion()
-        if self._version != version:
+        if major(self._version)!= major(version):
             print('WARNING: IxNetwork Python library version {0} does not match the IxNetwork server version {1}'.format(self._version, version))
 
     def _isConnected(self, raiseError=False):
         if self._websocket is None:
             if raiseError is True:
                 raise IxNetError('not connected')
             else:
```

## Comparing `IxNetwork-9.0.1915.16.dist-info/LICENSE.txt` & `IxNetwork-9.30.2212.7.dist-info/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 MIT License
 
 
-Copyright 1997 - 2019 by IXIA Keysight
+Copyright 1997 - 2023 by IXIA Keysight
 
 
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

