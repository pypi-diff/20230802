# Comparing `tmp/ogsapi-0.7.3.tar.gz` & `tmp/ogsapi-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogsapi-0.7.3.tar", last modified: Fri Jul 14 05:31:21 2023, max compression
+gzip compressed data, was "ogsapi-0.8.0.tar", last modified: Wed Aug  2 03:15:40 2023, max compression
```

## Comparing `ogsapi-0.7.3.tar` & `ogsapi-0.8.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 05:31:21.215380 ogsapi-0.7.3/
--rw-rw-rw-   0 root         (0) root         (0)    35082 2023-07-14 05:31:08.000000 ogsapi-0.7.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5557 2023-07-14 05:31:21.215380 ogsapi-0.7.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5123 2023-07-14 05:31:08.000000 ogsapi-0.7.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)      632 2023-07-14 05:31:08.000000 ogsapi-0.7.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 05:31:21.215380 ogsapi-0.7.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 05:31:21.212380 ogsapi-0.7.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 05:31:21.214380 ogsapi-0.7.3/src/ogsapi/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-14 05:31:08.000000 ogsapi-0.7.3/src/ogsapi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18160 2023-07-14 05:31:08.000000 ogsapi-0.7.3/src/ogsapi/client.py
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-07-14 05:31:08.000000 ogsapi-0.7.3/src/ogsapi/ogs_api_exception.py
--rw-rw-rw-   0 root         (0) root         (0)     1153 2023-07-14 05:31:08.000000 ogsapi-0.7.3/src/ogsapi/ogscredentials.py
--rw-rw-rw-   0 root         (0) root         (0)    14974 2023-07-14 05:31:08.000000 ogsapi-0.7.3/src/ogsapi/ogsgame.py
--rw-rw-rw-   0 root         (0) root         (0)     4088 2023-07-14 05:31:08.000000 ogsapi-0.7.3/src/ogsapi/ogsrestapi.py
--rw-rw-rw-   0 root         (0) root         (0)     6395 2023-07-14 05:31:08.000000 ogsapi-0.7.3/src/ogsapi/ogssocket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 05:31:21.214380 ogsapi-0.7.3/src/ogsapi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5557 2023-07-14 05:31:21.000000 ogsapi-0.7.3/src/ogsapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      395 2023-07-14 05:31:21.000000 ogsapi-0.7.3/src/ogsapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 05:31:21.000000 ogsapi-0.7.3/src/ogsapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-14 05:31:21.000000 ogsapi-0.7.3/src/ogsapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-14 05:31:21.000000 ogsapi-0.7.3/src/ogsapi.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 05:31:21.215380 ogsapi-0.7.3/src/tests/
--rw-rw-rw-   0 root         (0) root         (0)      903 2023-07-14 05:31:08.000000 ogsapi-0.7.3/src/tests/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 03:15:40.919396 ogsapi-0.8.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35082 2023-08-02 03:15:28.000000 ogsapi-0.8.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5557 2023-08-02 03:15:40.918396 ogsapi-0.8.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5123 2023-08-02 03:15:28.000000 ogsapi-0.8.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-08-02 03:15:28.000000 ogsapi-0.8.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-02 03:15:40.919396 ogsapi-0.8.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 03:15:40.914396 ogsapi-0.8.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 03:15:40.917396 ogsapi-0.8.0/src/ogsapi/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-02 03:15:28.000000 ogsapi-0.8.0/src/ogsapi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18255 2023-08-02 03:15:28.000000 ogsapi-0.8.0/src/ogsapi/client.py
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-08-02 03:15:28.000000 ogsapi-0.8.0/src/ogsapi/ogs_api_exception.py
+-rw-rw-rw-   0 root         (0) root         (0)     1153 2023-08-02 03:15:28.000000 ogsapi-0.8.0/src/ogsapi/ogscredentials.py
+-rw-rw-rw-   0 root         (0) root         (0)    14976 2023-08-02 03:15:28.000000 ogsapi-0.8.0/src/ogsapi/ogsgame.py
+-rw-rw-rw-   0 root         (0) root         (0)     4209 2023-08-02 03:15:28.000000 ogsapi-0.8.0/src/ogsapi/ogsrestapi.py
+-rw-rw-rw-   0 root         (0) root         (0)     6345 2023-08-02 03:15:28.000000 ogsapi-0.8.0/src/ogsapi/ogssocket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 03:15:40.918396 ogsapi-0.8.0/src/ogsapi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5557 2023-08-02 03:15:40.000000 ogsapi-0.8.0/src/ogsapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      395 2023-08-02 03:15:40.000000 ogsapi-0.8.0/src/ogsapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 03:15:40.000000 ogsapi-0.8.0/src/ogsapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-02 03:15:40.000000 ogsapi-0.8.0/src/ogsapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-02 03:15:40.000000 ogsapi-0.8.0/src/ogsapi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 03:15:40.918396 ogsapi-0.8.0/src/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      903 2023-08-02 03:15:28.000000 ogsapi-0.8.0/src/tests/test.py
```

### Comparing `ogsapi-0.7.3/LICENSE` & `ogsapi-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ogsapi-0.7.3/PKG-INFO` & `ogsapi-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogsapi
-Version: 0.7.3
+Version: 0.8.0
 Summary: An API Wrapper for online-go.com, an online Go / Baduk server
 Author-email: Dakota Marshall <me@dakotamarshall.net>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ogsapi-0.7.3/README.md` & `ogsapi-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `ogsapi-0.7.3/pyproject.toml` & `ogsapi-0.8.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "setuptools>=42",
   "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ogsapi"
-version = "0.7.3"
+version = "0.8.0"
 authors = [
   { name="Dakota Marshall", email="me@dakotamarshall.net" },
 ]
 description = "An API Wrapper for online-go.com, an online Go / Baduk server"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `ogsapi-0.7.3/src/ogsapi/client.py` & `ogsapi-0.8.0/src/ogsapi/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from .ogssocket import OGSSocket
 from .ogsrestapi import OGSRestAPI
 from .ogs_api_exception import OGSApiException
 
 
 # TODO: This will eventually need to be moved to `termination-api` instead of `/api/v1/`
 # TODO: Should probably implement a user class that contains all user info and functions
-# TODO: Break REST API functions into their own class, leaving the OGSClient class to be the interface for the user client
 
 class OGSClient:
     """Connect to and interact with the OGS REST API and SocketIO API.
 
     Examples:
         >>> from ogsapi.client import OGSClient
         >>> ogs = OGSClient(
@@ -24,37 +23,31 @@
         Connected to socket, authenticating
 
     Args:
         client_id (str): Client ID from OGS
         client_secret (str): Client Secret from OGS
         username (str): Username of OGS account
         password (str): Password of OGS account
-        debug (bool, optional): Enable debug logging. Defaults to False.        
+        debug (bool, optional): Enable debug logging. Defaults to False.
+        dev (bool, optional): Use the development API. Defaults to False.    
 
     Attributes:
         credentials (OGSCredentials): Credentials object containing all credentials
         api (OGSRestAPI): REST API connection to OGS
         sock (OGSSocket): SocketIO connection to OGS
 
     """
     def __init__(self, client_id, client_secret, username, password, debug: bool = False, dev: bool = False):
 
         self.credentials = OGSCredentials(client_id=client_id, client_secret=client_secret,
                                           username=username, password=password)
         self.api = OGSRestAPI(self.credentials,dev=dev)
         self.sock = OGSSocket(self.credentials, debug=debug)
-        self.sock.connect()
-
         self.credentials.user_id = self.user_vitals()
 
-    def __del__(self):
-        # Disconnect the OGSSocket instance if it exists
-        if hasattr(self, 'sock') and self.sock is not None:
-            self.sock.disconnect()
-
     # User Specific Resources: /me
 
     def user_vitals(self):
         """Get the user's vitals.
         
         Returns:
             response (dict): JSON response from the endpoint
@@ -187,15 +180,15 @@
         Returns:
             player_data (dict): Player data returned from the endpoint
         """
 
         endpoint = '/players/'
         return self.api.call_rest_endpoint('GET', endpoint=endpoint, params={'username' : player_username}).json()['results'][0]
 
-    # TODO: Need to make these customizable 
+    # TODO: This needs to be using a dataclass to make challenge customization easier
     def create_challenge(self, player_username: str = None, **game_settings):
         """Create either an open challenge or a challenge to a specific player.
         The time control settings are built depending on which time control is used.
         Make sure that you pass the correct time control settings for the time control you want to use.
         The other time control settings will be ignored.
         
         Examples:
@@ -441,7 +434,15 @@
             game_id (str): ID of the game to get SGF of.
         
         Returns:
             response (str): SGF of the game
         """
         endpoint = f'/games/{game_id}/sgf'
         return self.api.call_rest_endpoint('GET', endpoint).text
+
+    def socket_connect(self):
+        """Connect to the socket."""
+        self.sock.connect()
+
+    def socket_disconnect(self):
+        """Disconnect from the socket. You will need to do this before exiting your program, Or else it will hang and require a keyboard interrupt."""
+        self.sock.disconnect()
```

### Comparing `ogsapi-0.7.3/src/ogsapi/ogscredentials.py` & `ogsapi-0.8.0/src/ogsapi/ogscredentials.py`

 * *Files identical despite different names*

### Comparing `ogsapi-0.7.3/src/ogsapi/ogsgame.py` & `ogsapi-0.8.0/src/ogsapi/ogsgame.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,22 +4,20 @@
 
 class OGSGame:
     """OGSGame class for handling games connected via the OGSSocket.
     
     Args:
         game_socket (OGSSocket): OGSSocket object to connect to the game.
         game_id (str): ID of the game to connect to.
-        auth_data (dict): Authentication data for the game.
-        user_data (dict): User data for the game.
+        credentials (OGSCredentials): OGSCredentials object containing tokens for authentication to the Socket
         
     Attributes:
         socket (OGSSocket): OGSSocket object to connect to the game.
         game_id (str): ID of the game to connect to.
-        auth_data (dict): Authentication data for the game.
-        user_data (dict): User data for the game.
+        credentials (OGSCredentials): OGSCredentials object containing tokens for authentication to the Socket
         name (str): Name of the game.
         private (bool): Whether the game is private or not.
         white_player (dict): Dictionary containing information about the white player.
         black_player (dict): Dictionary containing information about the black player.
         ranked (bool): Whether the game is ranked or not.
         handicap (int): Handicap of the game.
         komi (float): Komi of the game.
```

### Comparing `ogsapi-0.7.3/src/ogsapi/ogsrestapi.py` & `ogsapi-0.8.0/src/ogsapi/ogsrestapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,10 +89,11 @@
 
         if 299 >= response.status_code >= 200:
             return response
 
         raise OGSApiException(f"{response.status_code}: {response.reason}")
 
     def get_auth_data(self):
+        """Get the auth data from the OGS API and save it to the credentials object for use in the socket connection."""
         auth_data = self.call_rest_endpoint('GET', '/ui/config').json()
         self.credentials.chat_auth = auth_data['chat_auth']
         self.credentials.user_jwt = auth_data['user_jwt']
```

### Comparing `ogsapi-0.7.3/src/ogsapi/ogssocket.py` & `ogsapi-0.8.0/src/ogsapi/ogssocket.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,27 +5,25 @@
 from .ogscredentials import OGSCredentials
 from .ogsgame import OGSGame
 
 class OGSSocket:
     """OGS Socket Class for handling SocketIO connections to OGS
     
     Args:
-        bearer_token (str): The bearer token to use for authentication
+        credentials (OGSCredentials): OGSCredentials object containing tokens for authentication to the Socket
         debug (bool, optional): Enable debug logging. Defaults to False.
     
     Attributes:
         clock_drift (float): The clock drift of the socket
         clock_latency (float): The clock latency of the socket
         last_ping (int): The last ping time of the socket
         last_issued_ping (int): The last time a ping was issued
         games (dict[OGSGame]): A dict of connected game objects
-        bearer_token (str): The bearer token used for authentication
         client_callbacks (dict): A dict of socket level callbacks
-        auth_data (dict): The auth data returned from the OGS API
-        user_data (dict): The user data returned from the OGS API
+        credentials (OGSCredentials): OGSCredentials object containing tokens for authentication to the Socket
         socket (socketio.Client): The socketio client object
         
     """
 
     def __init__(self, credentials: OGSCredentials, debug: bool = False):
         # Clock Settings
         self.clock_drift = 0.0
```

### Comparing `ogsapi-0.7.3/src/ogsapi.egg-info/PKG-INFO` & `ogsapi-0.8.0/src/ogsapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogsapi
-Version: 0.7.3
+Version: 0.8.0
 Summary: An API Wrapper for online-go.com, an online Go / Baduk server
 Author-email: Dakota Marshall <me@dakotamarshall.net>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ogsapi-0.7.3/src/tests/test.py` & `ogsapi-0.8.0/src/tests/test.py`

 * *Files identical despite different names*

