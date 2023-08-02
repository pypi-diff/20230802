# Comparing `tmp/lastfm-mpris2-scrobbler-0.2.0.tar.gz` & `tmp/lastfm-mpris2-scrobbler-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lastfm-mpris2-scrobbler-0.2.0.tar", last modified: Wed Aug  2 09:23:25 2023, max compression
+gzip compressed data, was "lastfm-mpris2-scrobbler-0.2.1.tar", last modified: Wed Aug  2 10:58:52 2023, max compression
```

## Comparing `lastfm-mpris2-scrobbler-0.2.0.tar` & `lastfm-mpris2-scrobbler-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 firefly   (1000) firefly   (1000)        0 2023-08-02 09:23:25.922783 lastfm-mpris2-scrobbler-0.2.0/
--rw-rw-r--   0 firefly   (1000) firefly   (1000)     1064 2023-08-02 08:55:19.000000 lastfm-mpris2-scrobbler-0.2.0/LICENSE
--rw-rw-r--   0 firefly   (1000) firefly   (1000)     1925 2023-08-02 09:23:25.922783 lastfm-mpris2-scrobbler-0.2.0/PKG-INFO
--rw-rw-r--   0 firefly   (1000) firefly   (1000)     1628 2023-08-02 08:55:19.000000 lastfm-mpris2-scrobbler-0.2.0/README.md
-drwxrwxr-x   0 firefly   (1000) firefly   (1000)        0 2023-08-02 09:23:25.922783 lastfm-mpris2-scrobbler-0.2.0/lastfm_mpris2_scrobbler.egg-info/
--rw-rw-r--   0 firefly   (1000) firefly   (1000)     1925 2023-08-02 09:23:25.000000 lastfm-mpris2-scrobbler-0.2.0/lastfm_mpris2_scrobbler.egg-info/PKG-INFO
--rw-rw-r--   0 firefly   (1000) firefly   (1000)      388 2023-08-02 09:23:25.000000 lastfm-mpris2-scrobbler-0.2.0/lastfm_mpris2_scrobbler.egg-info/SOURCES.txt
--rw-rw-r--   0 firefly   (1000) firefly   (1000)        1 2023-08-02 09:23:25.000000 lastfm-mpris2-scrobbler-0.2.0/lastfm_mpris2_scrobbler.egg-info/dependency_links.txt
--rw-rw-r--   0 firefly   (1000) firefly   (1000)       62 2023-08-02 09:23:25.000000 lastfm-mpris2-scrobbler-0.2.0/lastfm_mpris2_scrobbler.egg-info/entry_points.txt
--rw-rw-r--   0 firefly   (1000) firefly   (1000)        1 2023-08-02 08:42:31.000000 lastfm-mpris2-scrobbler-0.2.0/lastfm_mpris2_scrobbler.egg-info/not-zip-safe
--rw-rw-r--   0 firefly   (1000) firefly   (1000)       51 2023-08-02 09:23:25.000000 lastfm-mpris2-scrobbler-0.2.0/lastfm_mpris2_scrobbler.egg-info/requires.txt
--rw-rw-r--   0 firefly   (1000) firefly   (1000)        4 2023-08-02 09:23:25.000000 lastfm-mpris2-scrobbler-0.2.0/lastfm_mpris2_scrobbler.egg-info/top_level.txt
--rw-rw-r--   0 firefly   (1000) firefly   (1000)       38 2023-08-02 09:23:25.922783 lastfm-mpris2-scrobbler-0.2.0/setup.cfg
--rw-rw-r--   0 firefly   (1000) firefly   (1000)      909 2023-08-02 09:22:51.000000 lastfm-mpris2-scrobbler-0.2.0/setup.py
-drwxrwxr-x   0 firefly   (1000) firefly   (1000)        0 2023-08-02 09:23:25.922783 lastfm-mpris2-scrobbler-0.2.0/src/
--rw-rw-r--   0 firefly   (1000) firefly   (1000)        0 2023-08-02 08:41:31.000000 lastfm-mpris2-scrobbler-0.2.0/src/__init__.py
--rw-rw-r--   0 firefly   (1000) firefly   (1000)     5582 2023-08-02 09:11:50.000000 lastfm-mpris2-scrobbler-0.2.0/src/__main__.py
+drwxrwxr-x   0 firefly   (1000) firefly   (1000)        0 2023-08-02 10:58:52.659799 lastfm-mpris2-scrobbler-0.2.1/
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)     1064 2023-08-02 08:55:19.000000 lastfm-mpris2-scrobbler-0.2.1/LICENSE
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)     2003 2023-08-02 10:58:52.659799 lastfm-mpris2-scrobbler-0.2.1/PKG-INFO
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)     1706 2023-08-02 10:55:50.000000 lastfm-mpris2-scrobbler-0.2.1/README.md
+drwxrwxr-x   0 firefly   (1000) firefly   (1000)        0 2023-08-02 10:58:52.659799 lastfm-mpris2-scrobbler-0.2.1/lastfm_mpris2_scrobbler.egg-info/
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)     2003 2023-08-02 10:58:52.000000 lastfm-mpris2-scrobbler-0.2.1/lastfm_mpris2_scrobbler.egg-info/PKG-INFO
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)      388 2023-08-02 10:58:52.000000 lastfm-mpris2-scrobbler-0.2.1/lastfm_mpris2_scrobbler.egg-info/SOURCES.txt
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)        1 2023-08-02 10:58:52.000000 lastfm-mpris2-scrobbler-0.2.1/lastfm_mpris2_scrobbler.egg-info/dependency_links.txt
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)       62 2023-08-02 10:58:52.000000 lastfm-mpris2-scrobbler-0.2.1/lastfm_mpris2_scrobbler.egg-info/entry_points.txt
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)        1 2023-08-02 08:42:31.000000 lastfm-mpris2-scrobbler-0.2.1/lastfm_mpris2_scrobbler.egg-info/not-zip-safe
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)       51 2023-08-02 10:58:52.000000 lastfm-mpris2-scrobbler-0.2.1/lastfm_mpris2_scrobbler.egg-info/requires.txt
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)        4 2023-08-02 10:58:52.000000 lastfm-mpris2-scrobbler-0.2.1/lastfm_mpris2_scrobbler.egg-info/top_level.txt
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)       38 2023-08-02 10:58:52.659799 lastfm-mpris2-scrobbler-0.2.1/setup.cfg
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)      909 2023-08-02 10:58:39.000000 lastfm-mpris2-scrobbler-0.2.1/setup.py
+drwxrwxr-x   0 firefly   (1000) firefly   (1000)        0 2023-08-02 10:58:52.659799 lastfm-mpris2-scrobbler-0.2.1/src/
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)        0 2023-08-02 08:41:31.000000 lastfm-mpris2-scrobbler-0.2.1/src/__init__.py
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)     6098 2023-08-02 10:55:16.000000 lastfm-mpris2-scrobbler-0.2.1/src/__main__.py
```

### Comparing `lastfm-mpris2-scrobbler-0.2.0/LICENSE` & `lastfm-mpris2-scrobbler-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lastfm-mpris2-scrobbler-0.2.0/PKG-INFO` & `lastfm-mpris2-scrobbler-0.2.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lastfm-mpris2-scrobbler
-Version: 0.2.0
+Version: 0.2.1
 Summary: Last.fm scrobbler via MPRIS2 in Linux
 Home-page: https://github.com/Ladbaby/lastfm-scrobbler
 Author: Ladbaby
 Author-email: Ladbabyms@outlook.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -17,15 +17,15 @@
 
 ## Features
 
 - [x] scrobble music to Last.fm if one of the conditions are met:
 
     - played for 4 mins
     - played for half the length
-- [ ] scrobble now playing status
+- [x] update now playing status
 - [ ] offline storage support
 
 ## Alternatives
 
 If you'd like a scrobbler similar to this, there're some choices. I recommand taking a look at [scrobblez](https://github.com/YodaEmbedding/scrobblez), which is more functional (at least for now).
 
 Also, although [rescrobbled](https://github.com/InputUsername/rescrobbled) may also work, in my case it raised "Dbus error: argument type mismatch".
@@ -40,26 +40,23 @@
 
 ```bash
 playerctl --list-all
 ```
 
 ## Installation
 
+The package is now available via PyPI
+
 ```bash
-pip install -r requirements.txt
+pip install lastfm-mpris2-scrobbler
 ```
 
 ## Configurations
 
-```bash
-cp config.yaml.example config.yaml
-vim config.yaml
-```
-
-details can be found in the config file
+The program expect a `config.yaml` file, example and detailed information can be found in `config.yaml.example`
 
 ## Usage
 
 ```bash
-python main.py config.yaml
+lastfm-mpris2-scrobbler PATH_TO_YOUR_CONFIG/config.yaml
 ```
```

### Comparing `lastfm-mpris2-scrobbler-0.2.0/README.md` & `lastfm-mpris2-scrobbler-0.2.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 ## Features
 
 - [x] scrobble music to Last.fm if one of the conditions are met:
 
     - played for 4 mins
     - played for half the length
-- [ ] scrobble now playing status
+- [x] update now playing status
 - [ ] offline storage support
 
 ## Alternatives
 
 If you'd like a scrobbler similar to this, there're some choices. I recommand taking a look at [scrobblez](https://github.com/YodaEmbedding/scrobblez), which is more functional (at least for now).
 
 Also, although [rescrobbled](https://github.com/InputUsername/rescrobbled) may also work, in my case it raised "Dbus error: argument type mismatch".
@@ -29,26 +29,23 @@
 
 ```bash
 playerctl --list-all
 ```
 
 ## Installation
 
+The package is now available via PyPI
+
 ```bash
-pip install -r requirements.txt
+pip install lastfm-mpris2-scrobbler
 ```
 
 ## Configurations
 
-```bash
-cp config.yaml.example config.yaml
-vim config.yaml
-```
-
-details can be found in the config file
+The program expect a `config.yaml` file, example and detailed information can be found in `config.yaml.example`
 
 ## Usage
 
 ```bash
-python main.py config.yaml
+lastfm-mpris2-scrobbler PATH_TO_YOUR_CONFIG/config.yaml
 ```
```

### Comparing `lastfm-mpris2-scrobbler-0.2.0/lastfm_mpris2_scrobbler.egg-info/PKG-INFO` & `lastfm-mpris2-scrobbler-0.2.1/lastfm_mpris2_scrobbler.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lastfm-mpris2-scrobbler
-Version: 0.2.0
+Version: 0.2.1
 Summary: Last.fm scrobbler via MPRIS2 in Linux
 Home-page: https://github.com/Ladbaby/lastfm-scrobbler
 Author: Ladbaby
 Author-email: Ladbabyms@outlook.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -17,15 +17,15 @@
 
 ## Features
 
 - [x] scrobble music to Last.fm if one of the conditions are met:
 
     - played for 4 mins
     - played for half the length
-- [ ] scrobble now playing status
+- [x] update now playing status
 - [ ] offline storage support
 
 ## Alternatives
 
 If you'd like a scrobbler similar to this, there're some choices. I recommand taking a look at [scrobblez](https://github.com/YodaEmbedding/scrobblez), which is more functional (at least for now).
 
 Also, although [rescrobbled](https://github.com/InputUsername/rescrobbled) may also work, in my case it raised "Dbus error: argument type mismatch".
@@ -40,26 +40,23 @@
 
 ```bash
 playerctl --list-all
 ```
 
 ## Installation
 
+The package is now available via PyPI
+
 ```bash
-pip install -r requirements.txt
+pip install lastfm-mpris2-scrobbler
 ```
 
 ## Configurations
 
-```bash
-cp config.yaml.example config.yaml
-vim config.yaml
-```
-
-details can be found in the config file
+The program expect a `config.yaml` file, example and detailed information can be found in `config.yaml.example`
 
 ## Usage
 
 ```bash
-python main.py config.yaml
+lastfm-mpris2-scrobbler PATH_TO_YOUR_CONFIG/config.yaml
 ```
```

### Comparing `lastfm-mpris2-scrobbler-0.2.0/setup.py` & `lastfm-mpris2-scrobbler-0.2.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 root = path.abspath(path.dirname(__file__))
 with open(path.join(root, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='lastfm-mpris2-scrobbler',
-    version='0.2.0',
+    version='0.2.1',
     description="Last.fm scrobbler via MPRIS2 in Linux",
     url="https://github.com/Ladbaby/lastfm-scrobbler",
     author="Ladbaby",
     author_email="Ladbabyms@outlook.com",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `lastfm-mpris2-scrobbler-0.2.0/src/__main__.py` & `lastfm-mpris2-scrobbler-0.2.1/src/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         self.total_played_time = 0
         self.last_observation_timestamp = get_unix_timestamp()
         self.trackid = ""
         self.if_scrobbled = False
         self.update_status(metadata_dict, playback_status, self.last_observation_timestamp)
 
     def handle_multiple_artists(self, artist_array):
-        # trying to convert artist array into a single string
+        # convert artist array into a single string
         return ", ".join(artist_array)
     
     def update_status(self, metadata_dict, playback_status, timestamp):
         # time length of the current song in seconds
         self.length = int(metadata_dict["mpris:length"] / 1000000)
         # image file path
         self.artUrl = str(metadata_dict["mpris:artUrl"])
@@ -52,14 +52,15 @@
 class Scrobbler:
     def __init__(self, **kwargs):
         self.logger = logging.getLogger("dbus-scrobbler")
         coloredlogs.install(level="DEBUG", logger=self.logger)
 
         self.player_dict = {}
 
+        # TODO: handle network error
         self.network = pylast.LastFMNetwork(
             api_key=kwargs["api_key"],
             api_secret=kwargs["api_secret"],
             username=kwargs["user_name"],
             password_hash=kwargs["password_hash"],
         )
         self.user = self.network.get_user(kwargs["user_name"])
@@ -84,14 +85,22 @@
                 else:
                     self.player_dict[uri] = PlayerState(p.Metadata, p.PlaybackStatus)
         for uri in last_observation_uri_list:
             del self.player_dict[uri]
 
     def scrobble_all_players(self):
         for uri, player_obj in self.player_dict.items():
+            if player_obj.playback_status == "Playing":
+                self.network.update_now_playing(
+                    artist=player_obj.artist,
+                    title=player_obj.title,
+                    album=player_obj.album,
+                    album_artist=player_obj.albumArtist,
+                    track_number=player_obj.trackNumber,
+                )
             if player_obj.total_played_time >= min(self.scrobble_time_threshold, int(player_obj.length / 2)) and not player_obj.if_scrobbled:
                 self.network.scrobble(
                     artist=player_obj.artist, 
                     title=player_obj.title,
                     timestamp=player_obj.last_observation_timestamp,
                     album=player_obj.album,
                     album_artist=player_obj.albumArtist,
@@ -107,14 +116,17 @@
                 self.logger.debug("trackNumber: " + str(player_obj.trackNumber))
                 self.logger.debug("duration: " + str(int(player_obj.length)))
                 self.logger.debug("played time: " + str(int(player_obj.total_played_time)))
             else:
                 # self.logger.debug("scrobble condition unmet")
                 pass
 
+    def update_now_playing(self):
+        pass
+
 @click.command()
 @click.argument("config_file")
 def main(config_file):
     from dbus.mainloop.glib import DBusGMainLoop
     import yaml
 
     dbus_loop = DBusGMainLoop(set_as_default=True)
@@ -122,13 +134,16 @@
     # load config
     with open(config_file, "r") as file:
         config = yaml.safe_load(file)
 
     scrobbler = Scrobbler(**config)
 
     while True:
-        scrobbler.connect_to_all_players()
-        scrobbler.scrobble_all_players()
+        try: 
+            scrobbler.connect_to_all_players()
+            scrobbler.scrobble_all_players()
+        except Exception as e:
+            pass
         time.sleep(5)
 
 if __name__ == "__main__":
     main()
```

