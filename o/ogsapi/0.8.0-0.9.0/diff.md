# Comparing `tmp/ogsapi-0.8.0.tar.gz` & `tmp/ogsapi-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogsapi-0.8.0.tar", last modified: Wed Aug  2 03:15:40 2023, max compression
+gzip compressed data, was "ogsapi-0.9.0.tar", last modified: Wed Aug  2 06:33:29 2023, max compression
```

## Comparing `ogsapi-0.8.0.tar` & `ogsapi-0.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 03:15:40.919396 ogsapi-0.8.0/
--rw-rw-rw-   0 root         (0) root         (0)    35082 2023-08-02 03:15:28.000000 ogsapi-0.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5557 2023-08-02 03:15:40.918396 ogsapi-0.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5123 2023-08-02 03:15:28.000000 ogsapi-0.8.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      632 2023-08-02 03:15:28.000000 ogsapi-0.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-02 03:15:40.919396 ogsapi-0.8.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 03:15:40.914396 ogsapi-0.8.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 03:15:40.917396 ogsapi-0.8.0/src/ogsapi/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-02 03:15:28.000000 ogsapi-0.8.0/src/ogsapi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18255 2023-08-02 03:15:28.000000 ogsapi-0.8.0/src/ogsapi/client.py
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-08-02 03:15:28.000000 ogsapi-0.8.0/src/ogsapi/ogs_api_exception.py
--rw-rw-rw-   0 root         (0) root         (0)     1153 2023-08-02 03:15:28.000000 ogsapi-0.8.0/src/ogsapi/ogscredentials.py
--rw-rw-rw-   0 root         (0) root         (0)    14976 2023-08-02 03:15:28.000000 ogsapi-0.8.0/src/ogsapi/ogsgame.py
--rw-rw-rw-   0 root         (0) root         (0)     4209 2023-08-02 03:15:28.000000 ogsapi-0.8.0/src/ogsapi/ogsrestapi.py
--rw-rw-rw-   0 root         (0) root         (0)     6345 2023-08-02 03:15:28.000000 ogsapi-0.8.0/src/ogsapi/ogssocket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 03:15:40.918396 ogsapi-0.8.0/src/ogsapi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5557 2023-08-02 03:15:40.000000 ogsapi-0.8.0/src/ogsapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      395 2023-08-02 03:15:40.000000 ogsapi-0.8.0/src/ogsapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 03:15:40.000000 ogsapi-0.8.0/src/ogsapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-08-02 03:15:40.000000 ogsapi-0.8.0/src/ogsapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-02 03:15:40.000000 ogsapi-0.8.0/src/ogsapi.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 03:15:40.918396 ogsapi-0.8.0/src/tests/
--rw-rw-rw-   0 root         (0) root         (0)      903 2023-08-02 03:15:28.000000 ogsapi-0.8.0/src/tests/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 06:33:29.464506 ogsapi-0.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35082 2023-08-02 06:33:17.000000 ogsapi-0.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5557 2023-08-02 06:33:29.464506 ogsapi-0.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5123 2023-08-02 06:33:17.000000 ogsapi-0.9.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-08-02 06:33:17.000000 ogsapi-0.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-02 06:33:29.464506 ogsapi-0.9.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 06:33:29.460506 ogsapi-0.9.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 06:33:29.462506 ogsapi-0.9.0/src/ogsapi/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-02 06:33:17.000000 ogsapi-0.9.0/src/ogsapi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18444 2023-08-02 06:33:17.000000 ogsapi-0.9.0/src/ogsapi/client.py
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-08-02 06:33:17.000000 ogsapi-0.9.0/src/ogsapi/ogs_api_exception.py
+-rw-rw-rw-   0 root         (0) root         (0)     1153 2023-08-02 06:33:17.000000 ogsapi-0.9.0/src/ogsapi/ogscredentials.py
+-rw-rw-rw-   0 root         (0) root         (0)    14106 2023-08-02 06:33:17.000000 ogsapi-0.9.0/src/ogsapi/ogsgame.py
+-rw-rw-rw-   0 root         (0) root         (0)     4209 2023-08-02 06:33:17.000000 ogsapi-0.9.0/src/ogsapi/ogsrestapi.py
+-rw-rw-rw-   0 root         (0) root         (0)     6503 2023-08-02 06:33:17.000000 ogsapi-0.9.0/src/ogsapi/ogssocket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 06:33:29.463506 ogsapi-0.9.0/src/ogsapi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5557 2023-08-02 06:33:29.000000 ogsapi-0.9.0/src/ogsapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      395 2023-08-02 06:33:29.000000 ogsapi-0.9.0/src/ogsapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 06:33:29.000000 ogsapi-0.9.0/src/ogsapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-02 06:33:29.000000 ogsapi-0.9.0/src/ogsapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-02 06:33:29.000000 ogsapi-0.9.0/src/ogsapi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 06:33:29.463506 ogsapi-0.9.0/src/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1138 2023-08-02 06:33:17.000000 ogsapi-0.9.0/src/tests/test.py
```

### Comparing `ogsapi-0.8.0/LICENSE` & `ogsapi-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ogsapi-0.8.0/PKG-INFO` & `ogsapi-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogsapi
-Version: 0.8.0
+Version: 0.9.0
 Summary: An API Wrapper for online-go.com, an online Go / Baduk server
 Author-email: Dakota Marshall <me@dakotamarshall.net>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ogsapi-0.8.0/README.md` & `ogsapi-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ogsapi-0.8.0/pyproject.toml` & `ogsapi-0.9.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "setuptools>=42",
   "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ogsapi"
-version = "0.8.0"
+version = "0.9.0"
 authors = [
   { name="Dakota Marshall", email="me@dakotamarshall.net" },
 ]
 description = "An API Wrapper for online-go.com, an online Go / Baduk server"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `ogsapi-0.8.0/src/ogsapi/client.py` & `ogsapi-0.9.0/src/ogsapi/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -435,14 +435,19 @@
         
         Returns:
             response (str): SGF of the game
         """
         endpoint = f'/games/{game_id}/sgf'
         return self.api.call_rest_endpoint('GET', endpoint).text
 
-    def socket_connect(self):
-        """Connect to the socket."""
+    def socket_connect(self, callback_handler):
+        """Connect to the socket.
+        
+        Args:
+            callback_handler (Callable): Callback function to send socket events to.
+        """
+        self.sock.callback_handler = callback_handler
         self.sock.connect()
 
     def socket_disconnect(self):
         """Disconnect from the socket. You will need to do this before exiting your program, Or else it will hang and require a keyboard interrupt."""
         self.sock.disconnect()
```

### Comparing `ogsapi-0.8.0/src/ogsapi/ogscredentials.py` & `ogsapi-0.9.0/src/ogsapi/ogscredentials.py`

 * *Files identical despite different names*

### Comparing `ogsapi-0.8.0/src/ogsapi/ogsgame.py` & `ogsapi-0.9.0/src/ogsapi/ogsgame.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 class OGSGame:
     """OGSGame class for handling games connected via the OGSSocket.
     
     Args:
         game_socket (OGSSocket): OGSSocket object to connect to the game.
         game_id (str): ID of the game to connect to.
         credentials (OGSCredentials): OGSCredentials object containing tokens for authentication to the Socket
+        callback_handler (Callable): Callback handler function to send events to the user.
         
     Attributes:
         socket (OGSSocket): OGSSocket object to connect to the game.
         game_id (str): ID of the game to connect to.
         credentials (OGSCredentials): OGSCredentials object containing tokens for authentication to the Socket
+        callback_handler (Callable): Callback handler function to send events to the user.
         name (str): Name of the game.
         private (bool): Whether the game is private or not.
         white_player (dict): Dictionary containing information about the white player.
         black_player (dict): Dictionary containing information about the black player.
         ranked (bool): Whether the game is ranked or not.
         handicap (int): Handicap of the game.
         komi (float): Komi of the game.
@@ -34,20 +36,21 @@
         callback_func (dict): Dictionary containing the callback functions.
 
     """
     # Class for handling each OGSGame connected via the OGSSocket
     # To receive data from the game, use the callback function to register functions to be called when data is received.
     # on_move and on_clock are required for the game to function properly, on_undo is only for handling undo requests
     
-    def __init__(self, game_socket: Callable, credentials: OGSCredentials, game_id):
+    def __init__(self, game_socket: Callable, credentials: OGSCredentials, game_id, callback_handler: Callable):
         self.socket = game_socket
         self.game_id = game_id
         # Define callback functions from the API
         self._game_call_backs()
         self.credentials = credentials
+        self.callback_handler = callback_handler
         # Connect to the game
         self.connect()
 
         # Define relevant game data
         self.name: str = None
         self.private: bool = None
         self.white_player: dict = {
@@ -86,44 +89,40 @@
             'on_undo_accepted': None,
             'on_undo_canceled': None,
         }
 
     def __del__(self):
         self.disconnect()
 
-    def register_callback(self, event: str, callback: Callable):
-        """Register a callback function for receiving data from the API.
+    # def register_callback(self, event: str, callback: Callable):
+    #     """Register a callback function for receiving data from the API.
         
-        Args:
-            event (str): Event to register the callback function for.
-                Accepted events are:
-                    - on_move
-                    - on_clock
-                    - on_phase_change
-                    - on_undo_requested
-                    - on_undo_accepted
-                    - on_undo_canceled
-            callback (Callable): Callback function to register.   
-        """
-        self.callback_func[event] = callback
+    #     Args:
+    #         event (str): Event to register the callback function for.
+    #             Accepted events are:
+    #                 - on_move
+    #                 - on_clock
+    #                 - on_phase_change
+    #                 - on_undo_requested
+    #                 - on_undo_accepted
+    #                 - on_undo_canceled
+    #         callback (Callable): Callback function to register.   
+    #     """
+    #     self.callback_func[event] = callback
 
     # Low level socket functions
     def _game_call_backs(self):
 
+        # TODO: Need to create a game board state and have this update it
         @self.socket.on(f'game/{self.game_id}/move')
         def _on_game_move(data):
-            print(f"Got move: {data}")
-            try:
-                self.callback_func['on_move'](data)
-            except TypeError as e:
-                raise OGSApiException("Callback function 'on_move' must be Type Callable") from e
-            
+            self.callback_handler(data)
+
         @self.socket.on(f'game/{self.game_id}/gamedata')
         def _on_game_data(data):
-            print(f'Got Gamedata for game {self.game_id}: {data}')
 
             # Set important game data
             self.game_data = data
             self.name = data['game_name']
             self.private = data['private']
             self.white_player = data['players']['white']
             self.black_player = data['players']['black']
@@ -138,15 +137,14 @@
             self.move_list = data['moves']
             self.initial_state = data['initial_state']
             self.start_time = data['start_time']
 
         @self.socket.on(f'game/{self.game_id}/clock')
         def _on_game_clock(data):
             #TODO: Need to create a game clock and sync clock with this event
-            print(f'Got Clock: {data}')
 
             # Define clock parameters based on time control
             # TODO: This expects us to receive the clock AFTER the game data, 
             # which may not always the case  
             match self.time_control['time_control']:
                 case 'byoyomi':
                     self.clock = {
@@ -192,58 +190,39 @@
                     self.clock = {
                         'current_player': data['current_player'],
                         'last_move': data['last_move'],
                         'expiration': data['expiration']
                     }
             
             # Call the on_clock callback
-            try:
-                self.callback_func['on_clock'](self.clock)
-            except TypeError as e:
-                raise OGSApiException("Callback function 'on_clock' must be Type Callable") from e
+            self.callback_handler(event_name="clock", data=data)
 
         @self.socket.on(f'game/{self.game_id}/phase')
         def _on_game_phase(data):
-            print(f"Got Phase Change: {data}")
             self.phase = data
-            try:
-                self.callback_func['on_phase_change'](self.phase)
-            except TypeError as e:
-                raise OGSApiException("Callback function 'on_phase_change' must be Type Callable") from e
+            self.callback_handler(event_name="phase", data=data)
 
         @self.socket.on(f'game/{self.game_id}/latency')
         def _on_game_latency(data):
-            print(f'Got Latency: {data}')
             self.latency = data['latency']
+            self.callback_handler(event_name="latency", data=data)
 
         @self.socket.on(f'game/{self.game_id}/undo_requested')
         def _on_undo_requested(data):
             #TODO: Handle This 
-            print(f'Got Undo Request: {data}')
-            try:
-                self.callback_func['on_undo_requested'](data)
-            except TypeError as e:
-                raise OGSApiException("Callback function 'on_undo_requested' must be Type Callable") from e
+            self.callback_handler(event_name="undo_requested", data=data)
         
         @self.socket.on(f'game/{self.game_id}/undo_accepted')
         def _on_undo_accepted(data):
             #TODO: Handle This
-            print(f'Got Accepted Undo: {data}')
-            try:
-                self.callback_func['on_undo_accepted'](data)
-            except TypeError as e:
-                raise OGSApiException("Callback function 'on_undo_accepted' must be Type Callable") from e
+            self.callback_handler(event_name="undo_accepted", data=data)
         
         @self.socket.on(f'game/{self.game_id}/undo_canceled')
         def _on_undo_canceled(data):
-            print(f"Got Canceled Undo: {data}")
-            try:
-                self.callback_func['on_undo_canceled'](data)
-            except TypeError as e:
-                raise OGSApiException("Callback function 'on_undo_canceled' must be Type Callable") from e
+            self.callback_handler(event_name="undo_canceled", data=data)
     
     # Send functions
     def connect(self):
         """Connect to the game"""
         print(f"Connecting to game {self.game_id}")
         self.socket.emit(event="game/connect", data={'game_id': self.game_id, 'player_id': self.credentials.user_id, 'chat': False})
```

### Comparing `ogsapi-0.8.0/src/ogsapi/ogsrestapi.py` & `ogsapi-0.9.0/src/ogsapi/ogsrestapi.py`

 * *Files identical despite different names*

### Comparing `ogsapi-0.8.0/src/ogsapi/ogssocket.py` & `ogsapi-0.9.0/src/ogsapi/ogssocket.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,18 +29,15 @@
         self.clock_drift = 0.0
         self.clock_latency = 0.0
         self.last_ping = 0
         self.last_issued_ping = 0
         # Dict of connected game objects
         self.games = {}
         # Socket level callbacks
-        self.client_callbacks = {
-            'notification': None,
-            'error': None,
-        }
+        self.callback_handler = lambda event_name, data: None
         self.credentials = credentials
         self.socket = socketio.Client(logger=debug, engineio_logger=False)
 
     def __del__(self):
         self.disconnect()
 
     def connect(self):
@@ -48,26 +45,26 @@
         self.socket_callbacks()
         print("Connecting to Websocket")
         try:
             self.socket.connect('https://online-go.com/socket.io/?EIO=4', transports='websocket', headers={"Authorization" : f"Bearer {self.credentials.access_token}"})
         except Exception as e:
             raise OGSApiException("Failed to connect to OGS Websocket") from e
 
-    def register_callback(self, event: str, callback: Callable):
-        """Register a callback function for receiving data from the API.
+    # def register_callback(self, event: str, callback: Callable):
+    #     """Register a callback function for receiving data from the API.
         
-        Args:
-            event (str): Event to register the callback function for.
-                Accepted events are:
-                    - notification
-                    - chat
-                    - error
-            callback (Callable): Callback function to register.   
-        """
-        self.client_callbacks[event]: OGSGame = callback
+    #     Args:
+    #         event (str): Event to register the callback function for.
+    #             Accepted events are:
+    #                 - notification
+    #                 - chat
+    #                 - error
+    #         callback (Callable): Callback function to register.   
+    #     """
+    #     self.client_callbacks[event]: OGSGame = callback
 
     # Listens to events received from the socket via the decorators, and calls the appropriate function
     def socket_callbacks(self):
         """Set the callback functions for the socket"""
 
         @self.socket.on('connect')
         def authenticate():
@@ -91,34 +88,30 @@
             self.clock_drift = drift / 1000
             self.last_ping = now / 1000
             print(f"Got pong: {data}")
         
         @self.socket.on('active_game')
         def on_active_game(data):
             """Called when an active game is received on the socket"""
-            print(f"Got active game: {data}")
+            self.callback_handler(event_name="active_game", data=data)
 
         @self.socket.on('notification')
         def on_notification(data):
             """Called when a notification is received on the socket"""
-            print(f"Got notification: {data}")
+            self.callback_handler(event_name="notification", data=data)
 
         @self.socket.on('ERROR')
         def on_error(data):
             """Called when an error is received from the server"""
-            print(f"Got error: {data}")
-            try:
-                self.client_callbacks['error'](data)
-            except TypeError as e:
-                raise OGSApiException("Callback function 'error' must be Type Callable") from e
+            self.callback_handler(event_name="ERROR", data=data)
 
         @self.socket.on('*')
         def catch_all(event, data):
             """Catch all for events"""
-            print(f"Got Event: {event} \n {data}")
+            self.callback_handler(event_name=event, data=data)
 
     # Get info on connected server
     def host_info(self):
         """Get the host info of the socket"""
         self.socket.emit(event="hostinfo", namespace='/')
         print("Emit hostinfo")
     
@@ -130,25 +123,27 @@
         """Connect to the notification socket"""
         self.socket.emit(event="notification/connect", data={"auth": self.credentials.notification_auth, "player_id": self.credentials.user_id, "username": self.credentials.username})
     
     def chat_connect(self):
         """Connect to the chat socket"""
         self.socket.emit(event="chat/connect", data={"auth": self.credentials.chat_auth, "player_id": self.credentials.user_id, "username": self.credentials.username})
 
-    def game_connect(self, game_id: int):
+    def game_connect(self, game_id: int, callback_handler: Callable = None):
         """Connect to a game
         
         Args:
             game_id (int): The id of the game to connect to
+            callback_handler (Callable, optional): The callback handler for the game. Defaults to the callback_handler of the socket.
             
         Returns:
             OGSGame (OGSGame): The game object
         """
-
-        self.games[game_id] = OGSGame(game_socket=self.socket, game_id=game_id, credentials=self.credentials)
+        if callback_handler is None:
+            callback_handler = self.callback_handler
+        self.games[game_id] = OGSGame(game_socket=self.socket, game_id=game_id, credentials=self.credentials, callback_handler=callback_handler)
 
         return self.games[game_id]
 
     def game_disconnect(self, game_id: int):
         """Disconnect from a game
         
         Args:
```

### Comparing `ogsapi-0.8.0/src/ogsapi.egg-info/PKG-INFO` & `ogsapi-0.9.0/src/ogsapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogsapi
-Version: 0.8.0
+Version: 0.9.0
 Summary: An API Wrapper for online-go.com, an online Go / Baduk server
 Author-email: Dakota Marshall <me@dakotamarshall.net>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ogsapi-0.8.0/src/tests/test.py` & `ogsapi-0.9.0/src/tests/test.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,9 +20,14 @@
             self.fail("Failed to import OGSClient")
 
     def test_authentication(self):
         self.client = OGSClient(self.client_id, self.client_secret, self.username, self.password)
         self.assertIsNotNone(self.client.credentials.access_token)
         self.assertIsNotNone(self.client.credentials.refresh_token)
 
+    def test_websocket(self):
+        self.client = OGSClient(self.client_id, self.client_secret, self.username, self.password)
+        self.client.socket_connect(lambda event_name, data: None)
+        self.client.socket_disconnect()
+
 if __name__ == '__main__':
     unittest.main()
```

