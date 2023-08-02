# Comparing `tmp/abstract_audio-0.0.0.2-py3-none-any.whl.zip` & `tmp/abstract_audio-0.0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 16395 bytes, number of entries: 17
+Zip file size: 16445 bytes, number of entries: 17
 -rw-r--r--  2.0 unx        1 b- defN 23-Aug-02 07:34 abstract_audio/__init__.py
 -rw-r--r--  2.0 unx     4975 b- defN 23-Aug-02 07:34 abstract_audio/abstract_audio.py
--rw-r--r--  2.0 unx    11315 b- defN 23-Aug-02 08:09 abstract_audio/speech_to_text_gui.py
+-rw-r--r--  2.0 unx    11433 b- defN 23-Aug-02 08:12 abstract_audio/speech_to_text_gui.py
 -rw-r--r--  2.0 unx      292 b- defN 23-Aug-02 07:34 abstract_audio/audio_player/__init__.py
 -rw-r--r--  2.0 unx     4176 b- defN 23-Aug-02 07:34 abstract_audio/audio_player/abstractaudioplayer.py
 -rw-r--r--  2.0 unx     2317 b- defN 23-Aug-02 07:34 abstract_audio/audio_player/audioplayer_linux.py
 -rw-r--r--  2.0 unx     1059 b- defN 23-Aug-02 07:34 abstract_audio/audio_player/audioplayer_macos.py
 -rw-r--r--  2.0 unx     1606 b- defN 23-Aug-02 07:34 abstract_audio/audio_player/audioplayer_windows.py
 -rw-r--r--  2.0 unx      292 b- defN 23-Aug-02 07:34 audio_player/__init__.py
 -rw-r--r--  2.0 unx     4176 b- defN 23-Aug-02 07:34 audio_player/abstractaudioplayer.py
 -rw-r--r--  2.0 unx     2317 b- defN 23-Aug-02 07:34 audio_player/audioplayer_linux.py
 -rw-r--r--  2.0 unx     1059 b- defN 23-Aug-02 07:34 audio_player/audioplayer_macos.py
 -rw-r--r--  2.0 unx     1606 b- defN 23-Aug-02 07:34 audio_player/audioplayer_windows.py
--rw-r--r--  2.0 unx     5152 b- defN 23-Aug-02 08:10 abstract_audio-0.0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-02 08:10 abstract_audio-0.0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Aug-02 08:10 abstract_audio-0.0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1560 b- defN 23-Aug-02 08:10 abstract_audio-0.0.0.2.dist-info/RECORD
-17 files, 42010 bytes uncompressed, 13775 bytes compressed:  67.2%
+-rw-r--r--  2.0 unx     5152 b- defN 23-Aug-02 08:13 abstract_audio-0.0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-02 08:13 abstract_audio-0.0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Aug-02 08:13 abstract_audio-0.0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1560 b- defN 23-Aug-02 08:13 abstract_audio-0.0.0.3.dist-info/RECORD
+17 files, 42128 bytes uncompressed, 13825 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -33,20 +33,20 @@
 
 Filename: audio_player/audioplayer_macos.py
 Comment: 
 
 Filename: audio_player/audioplayer_windows.py
 Comment: 
 
-Filename: abstract_audio-0.0.0.2.dist-info/METADATA
+Filename: abstract_audio-0.0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: abstract_audio-0.0.0.2.dist-info/WHEEL
+Filename: abstract_audio-0.0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: abstract_audio-0.0.0.2.dist-info/top_level.txt
+Filename: abstract_audio-0.0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: abstract_audio-0.0.0.2.dist-info/RECORD
+Filename: abstract_audio-0.0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## abstract_audio/speech_to_text_gui.py

```diff
@@ -229,8 +229,9 @@
     change_glob('voice', '')
     change_glob('voice_value', '')
     write_to_file(filepath='voice.txt', contents='')
     change_glob('silence_kill',False)
     change_glob('recording',False)
     
     return gui()
+window_mgr,bridge,script_name = abstract_gui.create_window_manager(script_name="speech_to_text",global_var=globals())
```

## Comparing `abstract_audio-0.0.0.2.dist-info/METADATA` & `abstract_audio-0.0.0.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-audio
-Version: 0.0.0.2
+Version: 0.0.0.3
 Summary: This module provides functionalities to capture and manipulate audio input from a microphone and save them into a text file. It uses an abstract GUI to display the state of audio recording and playback..
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_audio
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `abstract_audio-0.0.0.2.dist-info/RECORD` & `abstract_audio-0.0.0.3.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 abstract_audio/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
 abstract_audio/abstract_audio.py,sha256=39lbpELuvtLY720emYh6rBr55TXhCnnjtaGaamXpahs,4975
-abstract_audio/speech_to_text_gui.py,sha256=oX1vwajEWMAyDXajjtKz18eN0ArGhEVIGmR7qnapKgo,11315
+abstract_audio/speech_to_text_gui.py,sha256=P5wVv8fL_UUaj4Qo-RXbASIEVgINgec-aD9Yp74jfMw,11433
 abstract_audio/audio_player/__init__.py,sha256=2FW7Gm0xqHBGgmfYZYPxryNZcT-9A79oKtg93qPx810,292
 abstract_audio/audio_player/abstractaudioplayer.py,sha256=n3lYvu8jbafRjnU6xTkCGxIQ1C3bCqLwDWa6RrwWD9E,4176
 abstract_audio/audio_player/audioplayer_linux.py,sha256=lN3gQne3NfLaPglVE-jCIrtdJyP4zbBwv94t22qETVU,2317
 abstract_audio/audio_player/audioplayer_macos.py,sha256=WjJpWic2mLyw27YZCrNYaL8Qz3p1oBQdrM0VMVNrq60,1059
 abstract_audio/audio_player/audioplayer_windows.py,sha256=oz2vDShN9GxXGokj3-CSBkZc071QqHM_AEFSL6uoOS4,1606
 audio_player/__init__.py,sha256=2FW7Gm0xqHBGgmfYZYPxryNZcT-9A79oKtg93qPx810,292
 audio_player/abstractaudioplayer.py,sha256=n3lYvu8jbafRjnU6xTkCGxIQ1C3bCqLwDWa6RrwWD9E,4176
 audio_player/audioplayer_linux.py,sha256=lN3gQne3NfLaPglVE-jCIrtdJyP4zbBwv94t22qETVU,2317
 audio_player/audioplayer_macos.py,sha256=WjJpWic2mLyw27YZCrNYaL8Qz3p1oBQdrM0VMVNrq60,1059
 audio_player/audioplayer_windows.py,sha256=oz2vDShN9GxXGokj3-CSBkZc071QqHM_AEFSL6uoOS4,1606
-abstract_audio-0.0.0.2.dist-info/METADATA,sha256=nMWaW74abG9Z1JkNQwDDpwabd_ptsXh6nhB1XkDAc-Y,5152
-abstract_audio-0.0.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-abstract_audio-0.0.0.2.dist-info/top_level.txt,sha256=AjNH1oOAm0OYbOPstMTm60kYYja4k8rKA1BAyzqtQ5w,15
-abstract_audio-0.0.0.2.dist-info/RECORD,,
+abstract_audio-0.0.0.3.dist-info/METADATA,sha256=oOL3ZaQD_Kj_ryQ3jo0MNqYEOKBp2P9ikQOC4wZAEBg,5152
+abstract_audio-0.0.0.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+abstract_audio-0.0.0.3.dist-info/top_level.txt,sha256=AjNH1oOAm0OYbOPstMTm60kYYja4k8rKA1BAyzqtQ5w,15
+abstract_audio-0.0.0.3.dist-info/RECORD,,
```

