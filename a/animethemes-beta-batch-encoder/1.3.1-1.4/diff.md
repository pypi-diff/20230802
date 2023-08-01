# Comparing `tmp/animethemes-beta-batch-encoder-1.3.1.tar.gz` & `tmp/animethemes-beta-batch-encoder-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animethemes-beta-batch-encoder-1.3.1.tar", last modified: Mon Jul  3 05:10:41 2023, max compression
+gzip compressed data, was "animethemes-beta-batch-encoder-1.4.tar", last modified: Tue Aug  1 22:39:31 2023, max compression
```

## Comparing `animethemes-beta-batch-encoder-1.3.1.tar` & `animethemes-beta-batch-encoder-1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 05:10:41.407932 animethemes-beta-batch-encoder-1.3.1/
--rw-rw-rw-   0        0        0     1082 2023-06-16 19:11:39.000000 animethemes-beta-batch-encoder-1.3.1/LICENSE
--rw-rw-rw-   0        0        0     5412 2023-07-03 05:10:41.406958 animethemes-beta-batch-encoder-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     4502 2023-07-03 04:40:29.000000 animethemes-beta-batch-encoder-1.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 05:10:41.389923 animethemes-beta-batch-encoder-1.3.1/animethemes_beta_batch_encoder.egg-info/
--rw-rw-rw-   0        0        0     5412 2023-07-03 05:10:41.000000 animethemes-beta-batch-encoder-1.3.1/animethemes_beta_batch_encoder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      703 2023-07-03 05:10:41.000000 animethemes-beta-batch-encoder-1.3.1/animethemes_beta_batch_encoder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 05:10:41.000000 animethemes-beta-batch-encoder-1.3.1/animethemes_beta_batch_encoder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-03 05:10:41.000000 animethemes-beta-batch-encoder-1.3.1/animethemes_beta_batch_encoder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-03 05:10:41.000000 animethemes-beta-batch-encoder-1.3.1/animethemes_beta_batch_encoder.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-03 05:10:41.404938 animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/
--rw-rw-rw-   0        0        0        0 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/__init__.py
--rw-rw-rw-   0        0        0     8114 2023-07-02 21:46:33.000000 animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/__main__.py
--rw-rw-rw-   0        0        0     1280 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_bitrate_mode.py
--rw-rw-rw-   0        0        0     2615 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_colorspace.py
--rw-rw-rw-   0        0        0    13543 2023-06-22 18:39:34.000000 animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_encode_webm.py
--rw-rw-rw-   0        0        0     4115 2023-06-22 08:05:47.000000 animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_encoding_config.py
--rw-rw-rw-   0        0        0     8234 2023-07-03 01:27:35.000000 animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_interface.py
--rw-rw-rw-   0        0        0     2527 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_loudnorm_filter.py
--rw-rw-rw-   0        0        0      779 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_seek.py
--rw-rw-rw-   0        0        0     5486 2023-07-03 05:08:27.000000 animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_seek_collector.py
--rw-rw-rw-   0        0        0     6594 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_source_file.py
--rw-rw-rw-   0        0        0     1375 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_utils.py
--rw-rw-rw-   0        0        0       42 2023-07-03 05:10:41.407932 animethemes-beta-batch-encoder-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1221 2023-07-03 05:10:39.000000 animethemes-beta-batch-encoder-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:39:31.091146 animethemes-beta-batch-encoder-1.4/
+-rw-rw-rw-   0        0        0     1082 2023-06-16 19:11:39.000000 animethemes-beta-batch-encoder-1.4/LICENSE
+-rw-rw-rw-   0        0        0     5452 2023-08-01 22:39:31.090172 animethemes-beta-batch-encoder-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4544 2023-08-01 22:38:14.000000 animethemes-beta-batch-encoder-1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 22:39:31.072147 animethemes-beta-batch-encoder-1.4/animethemes_beta_batch_encoder.egg-info/
+-rw-rw-rw-   0        0        0     5452 2023-08-01 22:39:30.000000 animethemes-beta-batch-encoder-1.4/animethemes_beta_batch_encoder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      703 2023-08-01 22:39:30.000000 animethemes-beta-batch-encoder-1.4/animethemes_beta_batch_encoder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 22:39:30.000000 animethemes-beta-batch-encoder-1.4/animethemes_beta_batch_encoder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-08-01 22:39:30.000000 animethemes-beta-batch-encoder-1.4/animethemes_beta_batch_encoder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-08-01 22:39:30.000000 animethemes-beta-batch-encoder-1.4/animethemes_beta_batch_encoder.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 22:39:31.088137 animethemes-beta-batch-encoder-1.4/beta_batch_encoder/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:05:26.000000 animethemes-beta-batch-encoder-1.4/beta_batch_encoder/__init__.py
+-rw-rw-rw-   0        0        0     8114 2023-08-01 22:09:28.000000 animethemes-beta-batch-encoder-1.4/beta_batch_encoder/__main__.py
+-rw-rw-rw-   0        0        0     1280 2023-07-22 06:05:26.000000 animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_bitrate_mode.py
+-rw-rw-rw-   0        0        0     2615 2023-07-22 06:05:26.000000 animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_colorspace.py
+-rw-rw-rw-   0        0        0    11883 2023-08-01 22:26:28.000000 animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_encode_webm.py
+-rw-rw-rw-   0        0        0     4115 2023-07-22 06:05:26.000000 animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_encoding_config.py
+-rw-rw-rw-   0        0        0     8403 2023-08-01 22:34:51.000000 animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_interface.py
+-rw-rw-rw-   0        0        0     2527 2023-07-22 06:05:26.000000 animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_loudnorm_filter.py
+-rw-rw-rw-   0        0        0      779 2023-07-22 06:05:26.000000 animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_seek.py
+-rw-rw-rw-   0        0        0     5486 2023-07-22 06:05:26.000000 animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_seek_collector.py
+-rw-rw-rw-   0        0        0     6150 2023-08-01 14:29:59.000000 animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_source_file.py
+-rw-rw-rw-   0        0        0     1375 2023-07-22 06:05:26.000000 animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_utils.py
+-rw-rw-rw-   0        0        0       42 2023-08-01 22:39:31.091146 animethemes-beta-batch-encoder-1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2023-08-01 22:38:57.000000 animethemes-beta-batch-encoder-1.4/setup.py
```

### Comparing `animethemes-beta-batch-encoder-1.3.1/LICENSE` & `animethemes-beta-batch-encoder-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.3.1/PKG-INFO` & `animethemes-beta-batch-encoder-1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animethemes-beta-batch-encoder
-Version: 1.3.1
+Version: 1.4
 Summary: Generate/Execute FFmpeg commands for files in acting directory
 Home-page: https://github.com/AnimeThemes/animethemes-batch-encoder
 Author: AnimeThemes
 Author-email: admin@animethemes.moe
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -81,14 +81,15 @@
 * `Custom` Apply a custom audio filter string.
 * `Fade In` Select an exponential value to apply Fade In.
 * `Fade Out` Select a start position and an exponential value to Fade Out.
 * `Mute` Select a start and end position to leave the volume at 0.
 
 **Video Filters**
 
+* `No Filters` Add a line without filter
 * `scale=-1:720` Add downscale to 720p
 * `scale=-1:720,hqdn3d=0:0:3:3,gradfun,unsharp` Add downscale to 720p and filters by AnimeThemes
 * `hqdn3d=0:0:3:3,gradfun,unsharp` Add filters by AnimeThemes
 * `hqdn3d=0:0:3:3` Add lightdenoise filter
 * `hqdn3d=1.5:1.5:6:6` Add heavydenoise filter
 * `unsharp` Add unsharp filter
 * `Custom` Apply a custom video filter string.
```

### Comparing `animethemes-beta-batch-encoder-1.3.1/README.md` & `animethemes-beta-batch-encoder-1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 * `Custom` Apply a custom audio filter string.
 * `Fade In` Select an exponential value to apply Fade In.
 * `Fade Out` Select a start position and an exponential value to Fade Out.
 * `Mute` Select a start and end position to leave the volume at 0.
 
 **Video Filters**
 
+* `No Filters` Add a line without filter
 * `scale=-1:720` Add downscale to 720p
 * `scale=-1:720,hqdn3d=0:0:3:3,gradfun,unsharp` Add downscale to 720p and filters by AnimeThemes
 * `hqdn3d=0:0:3:3,gradfun,unsharp` Add filters by AnimeThemes
 * `hqdn3d=0:0:3:3` Add lightdenoise filter
 * `hqdn3d=1.5:1.5:6:6` Add heavydenoise filter
 * `unsharp` Add unsharp filter
 * `Custom` Apply a custom video filter string.
```

### Comparing `animethemes-beta-batch-encoder-1.3.1/animethemes_beta_batch_encoder.egg-info/PKG-INFO` & `animethemes-beta-batch-encoder-1.4/animethemes_beta_batch_encoder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animethemes-beta-batch-encoder
-Version: 1.3.1
+Version: 1.4
 Summary: Generate/Execute FFmpeg commands for files in acting directory
 Home-page: https://github.com/AnimeThemes/animethemes-batch-encoder
 Author: AnimeThemes
 Author-email: admin@animethemes.moe
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -81,14 +81,15 @@
 * `Custom` Apply a custom audio filter string.
 * `Fade In` Select an exponential value to apply Fade In.
 * `Fade Out` Select a start position and an exponential value to Fade Out.
 * `Mute` Select a start and end position to leave the volume at 0.
 
 **Video Filters**
 
+* `No Filters` Add a line without filter
 * `scale=-1:720` Add downscale to 720p
 * `scale=-1:720,hqdn3d=0:0:3:3,gradfun,unsharp` Add downscale to 720p and filters by AnimeThemes
 * `hqdn3d=0:0:3:3,gradfun,unsharp` Add filters by AnimeThemes
 * `hqdn3d=0:0:3:3` Add lightdenoise filter
 * `hqdn3d=1.5:1.5:6:6` Add heavydenoise filter
 * `unsharp` Add unsharp filter
 * `Custom` Apply a custom video filter string.
```

### Comparing `animethemes-beta-batch-encoder-1.3.1/animethemes_beta_batch_encoder.egg-info/SOURCES.txt` & `animethemes-beta-batch-encoder-1.4/animethemes_beta_batch_encoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/__main__.py` & `animethemes-beta-batch-encoder-1.4/beta_batch_encoder/__main__.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_bitrate_mode.py` & `animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_bitrate_mode.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_colorspace.py` & `animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_colorspace.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_encode_webm.py` & `animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_encode_webm.py`

 * *Files 13% similar despite different names*

```diff
@@ -150,15 +150,15 @@
     @staticmethod
     def get_video_filters(config_filter=None):
         video_filters = []
 
         if config_filter is not None:
             video_filters.append(config_filter)
 
-        if not video_filters or len(video_filters[0].strip()) == 0:
+        if not video_filters or len(video_filters[0].strip()) == 0 or 'No Filters' in video_filters:
             return ''
 
         return ' -vf ' + ','.join(video_filters)
 
     # Build unique WebM filename for encodes
     def get_webm_filename(self, crf=None, cbr_bitrate=None, filter_name=None):
         webm_filename = self.seek.output_name
@@ -187,56 +187,38 @@
         
         if encoding_config.create_preview:
             file_commands.append(self.preview_seek(webm_filename=self.get_webm_filename()))
 
         for encoding_mode in encoding_config.encoding_modes:
             if BitrateMode.CBR.name == encoding_mode.upper():
                 file_commands.append(self.get_first_pass(BitrateMode.CBR, threads=encoding_config.threads))
-                if encoding_config.include_unfiltered:
-                    file_commands.append(self.get_second_pass(BitrateMode.CBR,
-                                                              threads=encoding_config.threads,
-                                                              video_filters=EncodeWebM.get_video_filters(),
-                                                              limit_size_enable=encoding_config.limit_size_enable,
-                                                              webm_filename=self.get_webm_filename(
-                                                                  cbr_bitrate=self.cbr_bitrate)))
                 for filter_name, filter_value in encoding_config.video_filters:
                     file_commands.append(self.get_second_pass(BitrateMode.CBR,
                                                               threads=encoding_config.threads,
                                                               video_filters=EncodeWebM.get_video_filters(
                                                                   config_filter=filter_value),
                                                               limit_size_enable=encoding_config.limit_size_enable,
                                                               webm_filename=self.get_webm_filename(
                                                                   cbr_bitrate=self.cbr_bitrate,
                                                                   filter_name=filter_name)))
             elif BitrateMode.VBR.name == encoding_mode.upper():
                 for crf in encoding_config.crfs:
                     file_commands.append(self.get_first_pass(BitrateMode.VBR, crf=crf, threads=encoding_config.threads))
-                    if encoding_config.include_unfiltered:
-                        file_commands.append(
-                            self.get_second_pass(BitrateMode.VBR, crf=crf, threads=encoding_config.threads, video_filters=EncodeWebM.get_video_filters(),
-                                                 limit_size_enable=encoding_config.limit_size_enable,
-                                                 webm_filename=self.get_webm_filename(crf=crf)))
                     for filter_name, filter_value in encoding_config.video_filters:
                         file_commands.append(self.get_second_pass(BitrateMode.VBR, crf=crf,
                                                                   threads=encoding_config.threads,
                                                                   video_filters=EncodeWebM.get_video_filters(
                                                                       config_filter=filter_value),
                                                                   limit_size_enable=encoding_config.limit_size_enable,
                                                                   webm_filename=self.get_webm_filename(
                                                                       crf=crf,
                                                                       filter_name=filter_name)))
             elif BitrateMode.CQ.name == encoding_mode.upper():
                 for crf in encoding_config.crfs:
                     file_commands.append(self.get_first_pass(BitrateMode.CQ, crf=crf, threads=encoding_config.threads))
-                    if encoding_config.include_unfiltered:
-                        file_commands.append(
-                            self.get_second_pass(BitrateMode.CQ, crf=crf, threads=encoding_config.threads, video_filters=self.get_video_filters(),
-                                                 limit_size_enable=encoding_config.limit_size_enable,
-                                                 webm_filename=self.get_webm_filename(crf=crf,
-                                                                                      cbr_bitrate=self.cbr_bitrate)))
                     for filter_name, filter_value in encoding_config.video_filters:
                         file_commands.append(self.get_second_pass(BitrateMode.CQ, crf=crf,
                                                                   threads=encoding_config.threads,
                                                                   video_filters=EncodeWebM.get_video_filters(
                                                                       config_filter=filter_value),
                                                                   limit_size_enable=encoding_config.limit_size_enable,
                                                                   webm_filename=self.get_webm_filename(
```

### Comparing `animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_encoding_config.py` & `animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_encoding_config.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_interface.py` & `animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,22 +109,26 @@
         )
 
         return ','.join(audio_filters_list)
     
     # Prompt the user for our list of video filters
     def video_filters(encoding_config):
         video_filters_options = {
+            'No Filters': 'no-vf',
             'scale=-1:720': '720p',
             'scale=-1:720,hqdn3d=0:0:3:3,gradfun,unsharp': 'filtered-720p',
             'hqdn3d=0:0:3:3,gradfun,unsharp': 'filtered',
             'hqdn3d=0:0:3:3': 'lightdenoise',
             'hqdn3d=1.5:1.5:6:6': 'heavydenoise',
             'unsharp': 'unsharp',
             'Custom': 'custom'
         }
+        
+        if encoding_config.include_unfiltered:
+            encoding_config.video_filters.append(('no-vf', 'No Filters'))
 
         question = [inquirer.Checkbox('video_filters', message='Select Video Filters (Space to select)',
                                       choices=video_filters_options.keys(), default=[tp[1] for tp in encoding_config.video_filters])]
         answer = inquirer.prompt(question)
 
         tp_list = [(name, filter_string) for filter_string, name in video_filters_options.items() if filter_string in answer['video_filters']]
```

### Comparing `animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_loudnorm_filter.py` & `animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_loudnorm_filter.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_seek.py` & `animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_seek.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_seek_collector.py` & `animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_seek_collector.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_source_file.py` & `animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_source_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -127,27 +127,13 @@
                 selected_stream = int(input(prompt_text))
                 if selected_stream in streams:
                     return selected_stream
                 logging.error('Stream selection is invalid')
             except ValueError:
                 logging.error('Stream selection must be an integer')
 
-    # Include the source file candidate?
-    @staticmethod
-    def yes_or_no(file):
-        yes = {'yes', 'y', ''}
-        no = {'no', 'n'}
-        while True:
-            choice = input(f'Include file \'{file}\': ').lower()
-            if choice in yes:
-                return True
-            elif choice in no:
-                return False
-            else:
-                logging.error('Please respond with \'y\' or \'n\'')
-
     # If our source file audio stream is not a 2-channel stereo layout, we need to resample it before normalization
     def apply_audio_resampling(self, audio_filters):
         channels = int(self.audio_format['streams'][0].get('channels', 2))
         channel_layout = self.audio_format['streams'][0].get('channel_layout', 'stereo')
         if channels != 2 or channel_layout != 'stereo':
             audio_filters.append('aresample=ochl=stereo')
```

### Comparing `animethemes-beta-batch-encoder-1.3.1/beta_batch_encoder/_utils.py` & `animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_utils.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.3.1/setup.py` & `animethemes-beta-batch-encoder-1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='animethemes-beta-batch-encoder',
-    version='1.3.1',
+    version='1.4',
     author='AnimeThemes',
     author_email='admin@animethemes.moe',
     url='https://github.com/AnimeThemes/animethemes-batch-encoder',
     description='Generate/Execute FFmpeg commands for files in acting directory',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

