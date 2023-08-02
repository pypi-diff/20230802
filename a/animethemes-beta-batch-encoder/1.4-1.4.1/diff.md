# Comparing `tmp/animethemes-beta-batch-encoder-1.4.tar.gz` & `tmp/animethemes-beta-batch-encoder-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animethemes-beta-batch-encoder-1.4.tar", last modified: Tue Aug  1 22:39:31 2023, max compression
+gzip compressed data, was "animethemes-beta-batch-encoder-1.4.1.tar", last modified: Wed Aug  2 13:50:45 2023, max compression
```

## Comparing `animethemes-beta-batch-encoder-1.4.tar` & `animethemes-beta-batch-encoder-1.4.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 22:39:31.091146 animethemes-beta-batch-encoder-1.4/
--rw-rw-rw-   0        0        0     1082 2023-06-16 19:11:39.000000 animethemes-beta-batch-encoder-1.4/LICENSE
--rw-rw-rw-   0        0        0     5452 2023-08-01 22:39:31.090172 animethemes-beta-batch-encoder-1.4/PKG-INFO
--rw-rw-rw-   0        0        0     4544 2023-08-01 22:38:14.000000 animethemes-beta-batch-encoder-1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 22:39:31.072147 animethemes-beta-batch-encoder-1.4/animethemes_beta_batch_encoder.egg-info/
--rw-rw-rw-   0        0        0     5452 2023-08-01 22:39:30.000000 animethemes-beta-batch-encoder-1.4/animethemes_beta_batch_encoder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      703 2023-08-01 22:39:30.000000 animethemes-beta-batch-encoder-1.4/animethemes_beta_batch_encoder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 22:39:30.000000 animethemes-beta-batch-encoder-1.4/animethemes_beta_batch_encoder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-08-01 22:39:30.000000 animethemes-beta-batch-encoder-1.4/animethemes_beta_batch_encoder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-08-01 22:39:30.000000 animethemes-beta-batch-encoder-1.4/animethemes_beta_batch_encoder.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-01 22:39:31.088137 animethemes-beta-batch-encoder-1.4/beta_batch_encoder/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:05:26.000000 animethemes-beta-batch-encoder-1.4/beta_batch_encoder/__init__.py
--rw-rw-rw-   0        0        0     8114 2023-08-01 22:09:28.000000 animethemes-beta-batch-encoder-1.4/beta_batch_encoder/__main__.py
--rw-rw-rw-   0        0        0     1280 2023-07-22 06:05:26.000000 animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_bitrate_mode.py
--rw-rw-rw-   0        0        0     2615 2023-07-22 06:05:26.000000 animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_colorspace.py
--rw-rw-rw-   0        0        0    11883 2023-08-01 22:26:28.000000 animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_encode_webm.py
--rw-rw-rw-   0        0        0     4115 2023-07-22 06:05:26.000000 animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_encoding_config.py
--rw-rw-rw-   0        0        0     8403 2023-08-01 22:34:51.000000 animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_interface.py
--rw-rw-rw-   0        0        0     2527 2023-07-22 06:05:26.000000 animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_loudnorm_filter.py
--rw-rw-rw-   0        0        0      779 2023-07-22 06:05:26.000000 animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_seek.py
--rw-rw-rw-   0        0        0     5486 2023-07-22 06:05:26.000000 animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_seek_collector.py
--rw-rw-rw-   0        0        0     6150 2023-08-01 14:29:59.000000 animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_source_file.py
--rw-rw-rw-   0        0        0     1375 2023-07-22 06:05:26.000000 animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_utils.py
--rw-rw-rw-   0        0        0       42 2023-08-01 22:39:31.091146 animethemes-beta-batch-encoder-1.4/setup.cfg
--rw-rw-rw-   0        0        0     1219 2023-08-01 22:38:57.000000 animethemes-beta-batch-encoder-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 13:50:45.643826 animethemes-beta-batch-encoder-1.4.1/
+-rw-rw-rw-   0        0        0     1082 2023-06-16 19:11:39.000000 animethemes-beta-batch-encoder-1.4.1/LICENSE
+-rw-rw-rw-   0        0        0     5454 2023-08-02 13:50:45.642828 animethemes-beta-batch-encoder-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4544 2023-08-01 22:38:14.000000 animethemes-beta-batch-encoder-1.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 13:50:45.625862 animethemes-beta-batch-encoder-1.4.1/animethemes_beta_batch_encoder.egg-info/
+-rw-rw-rw-   0        0        0     5454 2023-08-02 13:50:45.000000 animethemes-beta-batch-encoder-1.4.1/animethemes_beta_batch_encoder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      703 2023-08-02 13:50:45.000000 animethemes-beta-batch-encoder-1.4.1/animethemes_beta_batch_encoder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 13:50:45.000000 animethemes-beta-batch-encoder-1.4.1/animethemes_beta_batch_encoder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-08-02 13:50:45.000000 animethemes-beta-batch-encoder-1.4.1/animethemes_beta_batch_encoder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-08-02 13:50:45.000000 animethemes-beta-batch-encoder-1.4.1/animethemes_beta_batch_encoder.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 13:50:45.641837 animethemes-beta-batch-encoder-1.4.1/beta_batch_encoder/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:05:26.000000 animethemes-beta-batch-encoder-1.4.1/beta_batch_encoder/__init__.py
+-rw-rw-rw-   0        0        0     8114 2023-08-02 08:34:30.000000 animethemes-beta-batch-encoder-1.4.1/beta_batch_encoder/__main__.py
+-rw-rw-rw-   0        0        0     1280 2023-07-22 06:05:26.000000 animethemes-beta-batch-encoder-1.4.1/beta_batch_encoder/_bitrate_mode.py
+-rw-rw-rw-   0        0        0     2615 2023-07-22 06:05:26.000000 animethemes-beta-batch-encoder-1.4.1/beta_batch_encoder/_colorspace.py
+-rw-rw-rw-   0        0        0    11883 2023-08-02 09:17:01.000000 animethemes-beta-batch-encoder-1.4.1/beta_batch_encoder/_encode_webm.py
+-rw-rw-rw-   0        0        0     4115 2023-07-22 06:05:26.000000 animethemes-beta-batch-encoder-1.4.1/beta_batch_encoder/_encoding_config.py
+-rw-rw-rw-   0        0        0     8979 2023-08-02 09:38:46.000000 animethemes-beta-batch-encoder-1.4.1/beta_batch_encoder/_interface.py
+-rw-rw-rw-   0        0        0     2527 2023-07-22 06:05:26.000000 animethemes-beta-batch-encoder-1.4.1/beta_batch_encoder/_loudnorm_filter.py
+-rw-rw-rw-   0        0        0      779 2023-07-22 06:05:26.000000 animethemes-beta-batch-encoder-1.4.1/beta_batch_encoder/_seek.py
+-rw-rw-rw-   0        0        0     5486 2023-08-02 09:37:39.000000 animethemes-beta-batch-encoder-1.4.1/beta_batch_encoder/_seek_collector.py
+-rw-rw-rw-   0        0        0     6150 2023-08-01 14:29:59.000000 animethemes-beta-batch-encoder-1.4.1/beta_batch_encoder/_source_file.py
+-rw-rw-rw-   0        0        0     1375 2023-07-22 06:05:26.000000 animethemes-beta-batch-encoder-1.4.1/beta_batch_encoder/_utils.py
+-rw-rw-rw-   0        0        0       42 2023-08-02 13:50:45.643826 animethemes-beta-batch-encoder-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1221 2023-08-02 13:49:56.000000 animethemes-beta-batch-encoder-1.4.1/setup.py
```

### Comparing `animethemes-beta-batch-encoder-1.4/LICENSE` & `animethemes-beta-batch-encoder-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.4/PKG-INFO` & `animethemes-beta-batch-encoder-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animethemes-beta-batch-encoder
-Version: 1.4
+Version: 1.4.1
 Summary: Generate/Execute FFmpeg commands for files in acting directory
 Home-page: https://github.com/AnimeThemes/animethemes-batch-encoder
 Author: AnimeThemes
 Author-email: admin@animethemes.moe
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `animethemes-beta-batch-encoder-1.4/README.md` & `animethemes-beta-batch-encoder-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.4/animethemes_beta_batch_encoder.egg-info/PKG-INFO` & `animethemes-beta-batch-encoder-1.4.1/animethemes_beta_batch_encoder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animethemes-beta-batch-encoder
-Version: 1.4
+Version: 1.4.1
 Summary: Generate/Execute FFmpeg commands for files in acting directory
 Home-page: https://github.com/AnimeThemes/animethemes-batch-encoder
 Author: AnimeThemes
 Author-email: admin@animethemes.moe
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `animethemes-beta-batch-encoder-1.4/animethemes_beta_batch_encoder.egg-info/SOURCES.txt` & `animethemes-beta-batch-encoder-1.4.1/animethemes_beta_batch_encoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.4/beta_batch_encoder/__main__.py` & `animethemes-beta-batch-encoder-1.4.1/beta_batch_encoder/__main__.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_bitrate_mode.py` & `animethemes-beta-batch-encoder-1.4.1/beta_batch_encoder/_bitrate_mode.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_colorspace.py` & `animethemes-beta-batch-encoder-1.4.1/beta_batch_encoder/_colorspace.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_encode_webm.py` & `animethemes-beta-batch-encoder-1.4.1/beta_batch_encoder/_encode_webm.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_encoding_config.py` & `animethemes-beta-batch-encoder-1.4.1/beta_batch_encoder/_encoding_config.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_interface.py` & `animethemes-beta-batch-encoder-1.4.1/beta_batch_encoder/_interface.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import inquirer
 import logging
 import re
+import sys
 
 class Interface:
     # Time Duration Specification: https://ffmpeg.org/ffmpeg-utils.html#time-duration-syntax
     time_pattern = re.compile('^([0-5]?\d:){1,2}[0-5]?\d(?=\.\d+$|$)|\d+(?=\.\d+$|$)')
 
     # Validations
     validate_time = lambda _, x: all(Interface.time_pattern.match(y) for y in x.split(','))
@@ -12,42 +13,58 @@
     validate_encoding_modes = lambda _, x: all(y.strip().upper() in ['VBR', 'CBR', 'CQ'] for y in x.split(','))
 
     # Prompt the user for text questions
     def prompt_text(message, validate=lambda _, x: x):
         question = [inquirer.Text('text', message=message, validate=validate)]
         answer = inquirer.prompt(question)
 
+        if answer is None:
+            return 'NoName'
+
         logging.debug(f'[Interface.prompt_text] answer["text"]: \'{answer["text"]}\'')
 
         return answer['text']
     
     # Prompt the user for time questions
-    def prompt_time(message):
-        question = [inquirer.Text('time', message=message, validate=Interface.validate_time)]
+    def prompt_time(message, validate=validate_time):
+        question = [inquirer.Text('time', message=message, validate=validate)]
         answer = inquirer.prompt(question)
 
+        if answer is None:
+            return ''
+
         logging.debug(f'[Interface.prompt_time] answer["time"]: \'{answer["time"]}\'')
 
         return answer['time']
 
     # Prompt the user for our mode options to run to the user
     def choose_mode():
         modes = [('Generate commands', 1), ('Execute commands', 2), ('Generate and execute commands', 3)]
         question = [inquirer.List('mode', message='Mode (Enter)', choices=modes)]
         answer = inquirer.prompt(question)
 
+        if answer is None:
+            sys.exit()
+
         logging.debug(f'[Interface.choose_mode] answer["mode"]: \'{answer["mode"]}\'')
 
         return answer['mode']
     
     # Prompt the user for source files to choose
     def choose_source_files(source_files):
         question = [inquirer.Checkbox('source_files', message='Source Files (Space to select)', choices=source_files)]
         answer = inquirer.prompt(question)
 
+        if answer is None:
+            sys.exit()
+
+        if len(answer['source_files']) == 0:
+            logging.error('Select at least one file')
+            sys.exit()
+
         logging.debug(f'[Interface.choose_source_files] answer["source_files"]: \'{answer["source_files"]}\'')
 
         return answer['source_files']
       
     # Prompt the user for audio filters options
     def audio_filters_options(output_name):
         audio_filters = {
@@ -65,15 +82,18 @@
         }
 
         while not audio_filters['Exit']:
             print(f'\n\033[92mOutput Name: {output_name}\033[0m')
             question = [inquirer.List('audio_filters', message='Audio Filters (Enter)', choices=list(audio_filters.keys()))]
             answer = inquirer.prompt(question)
 
-            if answer['audio_filters'] == 'Fade In':
+            if answer is None:
+                audio_filters['Exit'] = True
+
+            elif answer['audio_filters'] == 'Fade In':
                 audio_filters['Fade In'] = Interface.prompt_time('Exponential Value').strip() or '0'
 
             elif answer['audio_filters'] == 'Fade Out':
                 audio_filters['Fade Out']['Start Time'] = Interface.prompt_time('Start Time').strip() or '0'
                 audio_filters['Fade Out']['Exp'] = Interface.prompt_time('Exponential Value').strip() or '0'
                      
             elif answer['audio_filters'] == 'Mute':
@@ -109,31 +129,34 @@
         )
 
         return ','.join(audio_filters_list)
     
     # Prompt the user for our list of video filters
     def video_filters(encoding_config):
         video_filters_options = {
-            'No Filters': 'no-vf',
+            'No Filters': None,
             'scale=-1:720': '720p',
             'scale=-1:720,hqdn3d=0:0:3:3,gradfun,unsharp': 'filtered-720p',
             'hqdn3d=0:0:3:3,gradfun,unsharp': 'filtered',
             'hqdn3d=0:0:3:3': 'lightdenoise',
             'hqdn3d=1.5:1.5:6:6': 'heavydenoise',
             'unsharp': 'unsharp',
             'Custom': 'custom'
         }
         
         if encoding_config.include_unfiltered:
-            encoding_config.video_filters.append(('no-vf', 'No Filters'))
+            encoding_config.video_filters.append((None, 'No Filters'))
 
         question = [inquirer.Checkbox('video_filters', message='Select Video Filters (Space to select)',
                                       choices=video_filters_options.keys(), default=[tp[1] for tp in encoding_config.video_filters])]
         answer = inquirer.prompt(question)
 
+        if answer is None:
+            return encoding_config
+
         tp_list = [(name, filter_string) for filter_string, name in video_filters_options.items() if filter_string in answer['video_filters']]
 
         if 'Custom' in answer['video_filters']:
             tp_list.remove(('custom', 'Custom'))
             custom_video_filters = Interface.prompt_text('Custom Video Filters (Separate with ",," if more than one)').split(',,')
             tp_list.extend([(f'custom{i + 1}', value) for i, value in enumerate(custom_video_filters)])
 
@@ -155,14 +178,17 @@
             inquirer.Confirm('limit_size_enable', message=f'Limit Size Enable?', default=limit_size_enable),
             inquirer.Text('crfs', message='CRFs', default=','.join(crfs), validate=Interface.validate_crfs),
             inquirer.Text('encoding_modes', message='Encoding Modes', default=','.join(encoding_modes), validate=Interface.validate_encoding_modes)
         ]
 
         answer = inquirer.prompt(questions)
 
+        if answer is None:
+            return encoding_config
+
         encoding_config.create_preview = answer['create_preview']
         encoding_config.limit_size_enable = answer['limit_size_enable']
         encoding_config.crfs = answer['crfs'].split(',')
         encoding_config.encoding_modes = answer['encoding_modes'].split(',')
 
         logging.debug(
             f'[Interface.custom_options] '
```

### Comparing `animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_loudnorm_filter.py` & `animethemes-beta-batch-encoder-1.4.1/beta_batch_encoder/_loudnorm_filter.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_seek.py` & `animethemes-beta-batch-encoder-1.4.1/beta_batch_encoder/_seek.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_seek_collector.py` & `animethemes-beta-batch-encoder-1.4.1/beta_batch_encoder/_seek_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,31 +23,31 @@
     # Validations for our prompts
     validate_seek = lambda _, x: \
         len(x.strip()) == 0 \
         or all(SeekCollector.time_pattern.match(y) for y in x.split(',')) \
         and SeekCollector.start_positions in [len(x.split(',')), 0]
 
     validate_output_name = lambda _, x: \
-        len(x.strip()) == 0 \
-        or all(SeekCollector.filename_pattern.match(y) and not y.strip() in SeekCollector.all_output_names for y in x.split(',')) \
+        len(x.strip()) > 0 \
+        and all(SeekCollector.filename_pattern.match(y) and not y.strip() in SeekCollector.all_output_names for y in x.split(',')) \
         and SeekCollector.start_positions == len(x.split(',')) 
 
     def __init__(self, source_file):
         self.source_file = source_file
         self.start_positions = SeekCollector.prompt_time('Start time(s)')
         self.end_positions = SeekCollector.prompt_time('End time(s)')
         self.output_names = SeekCollector.prompt_output_name()
         self.new_audio_filters = SeekCollector.prompt_new_audio_filters(self)
 
     # Prompt the user for our list of starting/ending positions of our WebMs
     # For starting positions, a blank input value is the 0 position of the source file
     # For ending positions, a blank input value is the end position of the source file
     @staticmethod
     def prompt_time(prompt_text):
-        positions = Interface.prompt_text(prompt_text, validate=SeekCollector.validate_seek).split(',')
+        positions = Interface.prompt_time(prompt_text, validate=SeekCollector.validate_seek).split(',')
         if prompt_text == 'Start time(s)':
             SeekCollector.start_positions = len(positions)
 
         return positions
 
     # Prompt the user for our list of name for our passlog/WebMs
     @staticmethod
```

### Comparing `animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_source_file.py` & `animethemes-beta-batch-encoder-1.4.1/beta_batch_encoder/_source_file.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.4/beta_batch_encoder/_utils.py` & `animethemes-beta-batch-encoder-1.4.1/beta_batch_encoder/_utils.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.4/setup.py` & `animethemes-beta-batch-encoder-1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='animethemes-beta-batch-encoder',
-    version='1.4',
+    version='1.4.1',
     author='AnimeThemes',
     author_email='admin@animethemes.moe',
     url='https://github.com/AnimeThemes/animethemes-batch-encoder',
     description='Generate/Execute FFmpeg commands for files in acting directory',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

