# Comparing `tmp/mat2-0.8.0.tar.gz` & `tmp/mat2-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mat2-0.8.0.tar", last modified: Thu Feb 28 00:21:45 2019, max compression
+gzip compressed data, was "dist/mat2-0.9.0.tar", last modified: Fri May 10 20:50:25 2019, max compression
```

## Comparing `mat2-0.8.0.tar` & `mat2-0.9.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 jvoisin   (1000) jvoisin   (1000)        0 2019-02-28 00:21:45.000000 mat2-0.8.0/
--rwxrwxr-x   0 jvoisin   (1000) jvoisin   (1000)     6360 2019-02-27 23:12:36.000000 mat2-0.8.0/mat2
--rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)     7254 2019-02-28 00:21:45.000000 mat2-0.8.0/PKG-INFO
--rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)       38 2019-02-28 00:21:45.000000 mat2-0.8.0/setup.cfg
--rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)     1104 2019-02-27 23:12:42.000000 mat2-0.8.0/setup.py
-drwxrwxr-x   0 jvoisin   (1000) jvoisin   (1000)        0 2019-02-28 00:21:45.000000 mat2-0.8.0/libmat2/
--rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)     1286 2019-02-03 18:23:28.000000 mat2-0.8.0/libmat2/abstract.py
--rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)     6648 2019-02-19 23:46:13.000000 mat2-0.8.0/libmat2/video.py
--rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)     4420 2019-02-03 19:31:00.000000 mat2-0.8.0/libmat2/images.py
--rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)     3041 2019-02-27 22:02:47.000000 mat2-0.8.0/libmat2/epub.py
--rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)     4336 2019-02-03 18:23:28.000000 mat2-0.8.0/libmat2/torrent.py
--rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)     7645 2019-02-25 14:37:42.000000 mat2-0.8.0/libmat2/archive.py
--rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)      432 2019-02-21 00:15:24.000000 mat2-0.8.0/libmat2/harmless.py
--rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)     1298 2019-02-03 18:23:28.000000 mat2-0.8.0/libmat2/__init__.py
--rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)     1925 2019-02-21 00:38:41.000000 mat2-0.8.0/libmat2/parser_factory.py
--rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)    15933 2019-02-23 19:47:39.000000 mat2-0.8.0/libmat2/office.py
--rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)     2341 2018-10-18 16:24:54.000000 mat2-0.8.0/libmat2/audio.py
--rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)     5357 2018-10-23 14:31:56.000000 mat2-0.8.0/libmat2/pdf.py
--rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)     2671 2019-02-03 19:24:38.000000 mat2-0.8.0/libmat2/exiftool.py
--rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)     6639 2019-02-27 22:52:01.000000 mat2-0.8.0/libmat2/web.py
--rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)     3651 2019-02-10 20:36:33.000000 mat2-0.8.0/libmat2/subprocess.py
-drwxrwxr-x   0 jvoisin   (1000) jvoisin   (1000)        0 2019-02-28 00:21:45.000000 mat2-0.8.0/mat2.egg-info/
--rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)        1 2019-02-28 00:21:45.000000 mat2-0.8.0/mat2.egg-info/dependency_links.txt
--rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)     7254 2019-02-28 00:21:45.000000 mat2-0.8.0/mat2.egg-info/PKG-INFO
--rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)       26 2019-02-28 00:21:45.000000 mat2-0.8.0/mat2.egg-info/requires.txt
--rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)      444 2019-02-28 00:21:45.000000 mat2-0.8.0/mat2.egg-info/SOURCES.txt
--rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)        8 2019-02-28 00:21:45.000000 mat2-0.8.0/mat2.egg-info/top_level.txt
--rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)     5323 2019-02-21 00:43:49.000000 mat2-0.8.0/README.md
+drwxrwxr-x   0 jvoisin   (1000) jvoisin   (1000)        0 2019-05-10 20:50:25.000000 mat2-0.9.0/
+-rwxrwxr-x   0 jvoisin   (1000) jvoisin   (1000)     6563 2019-05-10 20:16:04.000000 mat2-0.9.0/mat2
+-rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)     7302 2019-05-10 20:50:25.000000 mat2-0.9.0/PKG-INFO
+-rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)       38 2019-05-10 20:50:25.000000 mat2-0.9.0/setup.cfg
+-rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)     1104 2019-05-10 20:16:11.000000 mat2-0.9.0/setup.py
+drwxrwxr-x   0 jvoisin   (1000) jvoisin   (1000)        0 2019-05-10 20:50:25.000000 mat2-0.9.0/libmat2/
+-rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)     1460 2019-05-09 07:35:16.000000 mat2-0.9.0/libmat2/abstract.py
+-rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)     6648 2019-03-06 20:07:23.000000 mat2-0.9.0/libmat2/video.py
+-rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)     4420 2019-04-27 20:33:36.000000 mat2-0.9.0/libmat2/images.py
+-rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)     3024 2019-04-27 11:05:51.000000 mat2-0.9.0/libmat2/epub.py
+-rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)     4336 2019-03-06 20:07:23.000000 mat2-0.9.0/libmat2/torrent.py
+-rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)    17095 2019-05-01 15:56:30.000000 mat2-0.9.0/libmat2/archive.py
+-rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)      432 2019-02-21 00:15:24.000000 mat2-0.9.0/libmat2/harmless.py
+-rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)     1466 2019-03-30 09:33:16.000000 mat2-0.9.0/libmat2/__init__.py
+-rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)     2024 2019-05-09 07:38:56.000000 mat2-0.9.0/libmat2/parser_factory.py
+-rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)    15888 2019-04-27 11:05:51.000000 mat2-0.9.0/libmat2/office.py
+-rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)     2433 2019-05-10 19:00:41.000000 mat2-0.9.0/libmat2/audio.py
+-rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)     5357 2018-10-23 14:31:56.000000 mat2-0.9.0/libmat2/pdf.py
+-rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)     2671 2019-03-06 20:07:23.000000 mat2-0.9.0/libmat2/exiftool.py
+-rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)     6663 2019-04-14 18:34:59.000000 mat2-0.9.0/libmat2/web.py
+-rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)     3651 2019-02-10 20:36:33.000000 mat2-0.9.0/libmat2/subprocess.py
+drwxrwxr-x   0 jvoisin   (1000) jvoisin   (1000)        0 2019-05-10 20:50:25.000000 mat2-0.9.0/mat2.egg-info/
+-rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)        1 2019-05-10 20:50:25.000000 mat2-0.9.0/mat2.egg-info/dependency_links.txt
+-rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)     7302 2019-05-10 20:50:25.000000 mat2-0.9.0/mat2.egg-info/PKG-INFO
+-rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)       26 2019-05-10 20:50:25.000000 mat2-0.9.0/mat2.egg-info/requires.txt
+-rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)      444 2019-05-10 20:50:25.000000 mat2-0.9.0/mat2.egg-info/SOURCES.txt
+-rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)        8 2019-05-10 20:50:25.000000 mat2-0.9.0/mat2.egg-info/top_level.txt
+-rw-rw-r--   0 jvoisin   (1000) jvoisin   (1000)     5363 2019-03-30 09:25:17.000000 mat2-0.9.0/README.md
```

### Comparing `mat2-0.8.0/mat2` & `mat2-0.9.0/mat2`

 * *Files 6% similar despite different names*

```diff
@@ -11,32 +11,37 @@
 try:
     from libmat2 import parser_factory, UNSUPPORTED_EXTENSIONS
     from libmat2 import check_dependencies, UnknownMemberPolicy
 except ValueError as e:
     print(e)
     sys.exit(1)
 
-__version__ = '0.8.0'
+__version__ = '0.9.0'
 
 # Make pyflakes happy
 assert Tuple
 assert Union
 
 logging.basicConfig(format='%(levelname)s: %(message)s', level=logging.WARNING)
 
 
-def __check_file(filename: str, mode: int=os.R_OK) -> bool:
+def __check_file(filename: str, mode: int = os.R_OK) -> bool:
     if not os.path.exists(filename):
-        print("[-] %s is doesn't exist." % filename)
+        print("[-] %s doesn't exist." % filename)
         return False
     elif not os.path.isfile(filename):
         print("[-] %s is not a regular file." % filename)
         return False
     elif not os.access(filename, mode):
-        print("[-] %s is not readable and writeable." % filename)
+        mode_str = []  # type: List[str]
+        if mode & os.R_OK:
+            mode_str += 'readable'
+        if mode & os.W_OK:
+            mode_str += 'writeable'
+        print("[-] %s is not %s." % (filename, 'nor '.join(mode_str)))
         return False
     return True
 
 
 def create_arg_parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(description='Metadata anonymisation toolkit 2')
     parser.add_argument('files', nargs='*', help='the files to process')
@@ -45,16 +50,17 @@
     parser.add_argument('-l', '--list', action='store_true',
                         help='list all supported fileformats')
     parser.add_argument('--check-dependencies', action='store_true',
                         help='check if MAT2 has all the dependencies it needs')
     parser.add_argument('-V', '--verbose', action='store_true',
                         help='show more verbose status information')
     parser.add_argument('--unknown-members', metavar='policy', default='abort',
-                        help='how to handle unknown members of archive-style files (policy should' +
-                        ' be one of: %s)' % ', '.join(p.value for p in UnknownMemberPolicy))
+                        help='how to handle unknown members of archive-style '
+                        'files (policy should be one of: %s) [Default: abort]' %
+                        ', '.join(p.value for p in UnknownMemberPolicy))
 
 
     info = parser.add_mutually_exclusive_group()
     info.add_argument('-s', '--show', action='store_true',
                       help='list harmful metadata detectable by MAT2 without removing them')
     info.add_argument('-L', '--lightweight', action='store_true',
                       help='remove SOME metadata')
@@ -68,15 +74,15 @@
     p, mtype = parser_factory.get_parser(filename)  # type: ignore
     if p is None:
         print("[-] %s's format (%s) is not supported" % (filename, mtype))
         return
     __print_meta(filename, p.get_meta())
 
 
-def __print_meta(filename: str, metadata: dict, depth: int=1):
+def __print_meta(filename: str, metadata: dict, depth: int = 1):
     padding = " " * depth*2
     if not metadata:
         print(padding + "No metadata found")
         return
 
     print("[%s] Metadata for %s:" % ('+'*depth, filename))
 
@@ -96,15 +102,15 @@
         try:  # FIXME this is ugly.
             print(padding + "  %s: %s" % (k, v))
         except UnicodeEncodeError:
             print(padding + "  %s: harmful content" % k)
 
 
 def clean_meta(filename: str, is_lightweight: bool, policy: UnknownMemberPolicy) -> bool:
-    if not __check_file(filename, os.R_OK|os.W_OK):
+    if not __check_file(filename, os.R_OK):
         return False
 
     p, mtype = parser_factory.get_parser(filename)  # type: ignore
     if p is None:
         print("[-] %s's format (%s) is not supported" % (filename, mtype))
         return False
     p.unknown_member_policy = policy
```

### Comparing `mat2-0.8.0/PKG-INFO` & `mat2-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat2
-Version: 0.8.0
+Version: 0.9.0
 Summary: A handy tool to trash your metadata
 Home-page: https://0xacab.org/jvoisin/mat2
 Author: Julien (jvoisin) Voisin
 Author-email: julien.voisin+mat2@dustri.org
 License: UNKNOWN
 Project-URL: bugtacker, https://0xacab.org/jvoisin/mat2/issues
 Description: ```
@@ -35,15 +35,15 @@
         metadata.
         
         # Requirements
         
         - `python3-mutagen` for audio support
         - `python3-gi-cairo` and `gir1.2-poppler-0.18` for PDF support
         - `gir1.2-gdkpixbuf-2.0` for images support
-        - `FFmpeg`, optionally, for video support 
+        - `FFmpeg`, optionally, for video support
         - `libimage-exiftool-perl` for everything else
         - `bubblewrap`, optionally, for sandboxing
         
         Please note that MAT2 requires at least Python3.5, meaning that it
         doesn't run on [Debian Jessie](https://packages.debian.org/jessie/python3).
         
         # Running the test suite
@@ -75,15 +75,16 @@
           -h, --help            show this help message and exit
           -v, --version         show program's version number and exit
           -l, --list            list all supported fileformats
           --check-dependencies  check if MAT2 has all the dependencies it needs
           -V, --verbose         show more verbose status information
           --unknown-members policy
                                 how to handle unknown members of archive-style files
-                                (policy should be one of: abort, omit, keep)
+                                (policy should be one of: abort, omit, keep) [Default:
+                                abort]
           -s, --show            list harmful metadata detectable by MAT2 without
                                 removing them
           -L, --lightweight     remove SOME metadata
         ```
         
         Note that MAT2 **will not** clean files in-place, but will produce, for
         example, with a file named "myfile.png" a cleaned version named
```

### Comparing `mat2-0.8.0/setup.py` & `mat2-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mat2",
-    version='0.8.0',
+    version='0.9.0',
     author="Julien (jvoisin) Voisin",
     author_email="julien.voisin+mat2@dustri.org",
     description="A handy tool to trash your metadata",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://0xacab.org/jvoisin/mat2",
     python_requires = '>=3.5.0',
```

### Comparing `mat2-0.8.0/libmat2/video.py` & `mat2-0.9.0/libmat2/video.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 from . import exiftool
 from . import subprocess
 
 
 class AbstractFFmpegParser(exiftool.ExiftoolParser):
     """ Abstract parser for all FFmpeg-based ones, mainly for video. """
     # Some fileformats have mandatory metadata fields
-    meta_key_value_whitelist = {}  # type: Dict[str, Union[str, int]]
+    meta_key_value_allowlist = {}  # type: Dict[str, Union[str, int]]
 
     def remove_all(self) -> bool:
-        if self.meta_key_value_whitelist:
+        if self.meta_key_value_allowlist:
             logging.warning('The format of "%s" (%s) has some mandatory '
                             'metadata fields; mat2 filled them with standard '
                             'data.', self.filename, ', '.join(self.mimetypes))
         cmd = [_get_ffmpeg_path(),
                '-i', self.filename,      # input file
                '-y',                     # overwrite existing output file
                '-map', '0',              # copy everything all streams from input to output
@@ -41,48 +41,48 @@
         return True
 
     def get_meta(self) -> Dict[str, Union[str, dict]]:
         meta = super().get_meta()
 
         ret = dict()  # type: Dict[str, Union[str, dict]]
         for key, value in meta.items():
-            if key in self.meta_key_value_whitelist.keys():
-                if value == self.meta_key_value_whitelist[key]:
+            if key in self.meta_key_value_allowlist.keys():
+                if value == self.meta_key_value_allowlist[key]:
                     continue
             ret[key] = value
         return ret
 
 
 class WMVParser(AbstractFFmpegParser):
     mimetypes = {'video/x-ms-wmv', }
-    meta_whitelist = {'AudioChannels', 'AudioCodecID', 'AudioCodecName',
+    meta_allowlist = {'AudioChannels', 'AudioCodecID', 'AudioCodecName',
                       'ErrorCorrectionType', 'AudioSampleRate', 'DataPackets',
                       'Directory', 'Duration', 'ExifToolVersion',
                       'FileAccessDate', 'FileInodeChangeDate', 'FileLength',
                       'FileModifyDate', 'FileName', 'FilePermissions',
                       'FileSize', 'FileType', 'FileTypeExtension',
                       'FrameCount', 'FrameRate', 'ImageHeight', 'ImageSize',
                       'ImageWidth', 'MIMEType', 'MaxBitrate', 'MaxPacketSize',
                       'Megapixels', 'MinPacketSize', 'Preroll', 'SendDuration',
                       'SourceFile', 'StreamNumber', 'VideoCodecName', }
-    meta_key_value_whitelist = {  # some metadata are mandatory :/
+    meta_key_value_allowlist = {  # some metadata are mandatory :/
         'AudioCodecDescription': '',
         'CreationDate': '0000:00:00 00:00:00Z',
         'FileID': '00000000-0000-0000-0000-000000000000',
         'Flags': 2,  # FIXME: What is this? Why 2?
         'ModifyDate': '0000:00:00 00:00:00',
         'TimeOffset': '0 s',
         'VideoCodecDescription': '',
         'StreamType': 'Audio',
         }
 
 
 class AVIParser(AbstractFFmpegParser):
     mimetypes = {'video/x-msvideo', }
-    meta_whitelist = {'SourceFile', 'ExifToolVersion', 'FileName', 'Directory',
+    meta_allowlist = {'SourceFile', 'ExifToolVersion', 'FileName', 'Directory',
                       'FileSize', 'FileModifyDate', 'FileAccessDate',
                       'FileInodeChangeDate', 'FilePermissions', 'FileType',
                       'FileTypeExtension', 'MIMEType', 'FrameRate', 'MaxDataRate',
                       'FrameCount', 'StreamCount', 'StreamType', 'VideoCodec',
                       'VideoFrameRate', 'VideoFrameCount', 'Quality',
                       'SampleSize', 'BMPVersion', 'ImageWidth', 'ImageHeight',
                       'Planes', 'BitDepth', 'Compression', 'ImageLength',
@@ -94,26 +94,26 @@
                       'AudioSampleRate', 'Encoding', 'NumChannels',
                       'SampleRate', 'AvgBytesPerSec', 'BitsPerSample',
                       'Duration', 'ImageSize', 'Megapixels'}
 
 
 class MP4Parser(AbstractFFmpegParser):
     mimetypes = {'video/mp4', }
-    meta_whitelist = {'AudioFormat', 'AvgBitrate', 'Balance', 'TrackDuration',
+    meta_allowlist = {'AudioFormat', 'AvgBitrate', 'Balance', 'TrackDuration',
                       'XResolution', 'YResolution', 'ExifToolVersion',
                       'FileAccessDate', 'FileInodeChangeDate', 'FileModifyDate',
                       'FileName', 'FilePermissions', 'MIMEType', 'FileType',
                       'FileTypeExtension', 'Directory', 'ImageWidth',
                       'ImageSize', 'ImageHeight', 'FileSize', 'SourceFile',
                       'BitDepth', 'Duration', 'AudioChannels',
                       'AudioBitsPerSample', 'AudioSampleRate', 'Megapixels',
                       'MovieDataSize', 'VideoFrameRate', 'MediaTimeScale',
                       'SourceImageHeight', 'SourceImageWidth',
                       'MatrixStructure', 'MediaDuration'}
-    meta_key_value_whitelist = {  # some metadata are mandatory :/
+    meta_key_value_allowlist = {  # some metadata are mandatory :/
         'CreateDate': '0000:00:00 00:00:00',
         'CurrentTime': '0 s',
         'MediaCreateDate': '0000:00:00 00:00:00',
         'MediaLanguageCode': 'und',
         'MediaModifyDate': '0000:00:00 00:00:00',
         'ModifyDate': '0000:00:00 00:00:00',
         'OpColor': '0 0 0',
```

### Comparing `mat2-0.8.0/libmat2/images.py` & `mat2-0.9.0/libmat2/images.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from . import exiftool
 
 # Make pyflakes happy
 assert Set
 
 class PNGParser(exiftool.ExiftoolParser):
     mimetypes = {'image/png', }
-    meta_whitelist = {'SourceFile', 'ExifToolVersion', 'FileName',
+    meta_allowlist = {'SourceFile', 'ExifToolVersion', 'FileName',
                       'Directory', 'FileSize', 'FileModifyDate',
                       'FileAccessDate', 'FileInodeChangeDate',
                       'FilePermissions', 'FileType', 'FileTypeExtension',
                       'MIMEType', 'ImageWidth', 'BitDepth', 'ColorType',
                       'Compression', 'Filter', 'Interlace', 'BackgroundColor',
                       'ImageSize', 'Megapixels', 'ImageHeight'}
 
@@ -40,15 +40,15 @@
         surface = cairo.ImageSurface.create_from_png(self.filename)
         surface.write_to_png(self.output_filename)
         return True
 
 
 class GIFParser(exiftool.ExiftoolParser):
     mimetypes = {'image/gif'}
-    meta_whitelist = {'AnimationIterations', 'BackgroundColor', 'BitsPerPixel',
+    meta_allowlist = {'AnimationIterations', 'BackgroundColor', 'BitsPerPixel',
                       'ColorResolutionDepth', 'Directory', 'Duration',
                       'ExifToolVersion', 'FileAccessDate',
                       'FileInodeChangeDate', 'FileModifyDate', 'FileName',
                       'FilePermissions', 'FileSize', 'FileType',
                       'FileTypeExtension', 'FrameCount', 'GIFVersion',
                       'HasColorMap', 'ImageHeight', 'ImageSize', 'ImageWidth',
                       'MIMEType', 'Megapixels', 'SourceFile',}
@@ -82,28 +82,28 @@
         pixbuf.savev(self.output_filename, type=extension[1:], option_keys=[], option_values=[])
         return True
 
 
 class JPGParser(GdkPixbufAbstractParser):
     _type = 'jpeg'
     mimetypes = {'image/jpeg'}
-    meta_whitelist = {'SourceFile', 'ExifToolVersion', 'FileName',
+    meta_allowlist = {'SourceFile', 'ExifToolVersion', 'FileName',
                       'Directory', 'FileSize', 'FileModifyDate',
                       'FileAccessDate', "FileInodeChangeDate",
                       'FilePermissions', 'FileType', 'FileTypeExtension',
                       'MIMEType', 'ImageWidth', 'ImageSize', 'BitsPerSample',
                       'ColorComponents', 'EncodingProcess', 'JFIFVersion',
                       'ResolutionUnit', 'XResolution', 'YCbCrSubSampling',
                       'YResolution', 'Megapixels', 'ImageHeight'}
 
 
 class TiffParser(GdkPixbufAbstractParser):
     _type = 'tiff'
     mimetypes = {'image/tiff'}
-    meta_whitelist = {'Compression', 'ExifByteOrder', 'ExtraSamples',
+    meta_allowlist = {'Compression', 'ExifByteOrder', 'ExtraSamples',
                       'FillOrder', 'PhotometricInterpretation',
                       'PlanarConfiguration', 'RowsPerStrip', 'SamplesPerPixel',
                       'StripByteCounts', 'StripOffsets', 'BitsPerSample',
                       'Directory', 'ExifToolVersion', 'FileAccessDate',
                       'FileInodeChangeDate', 'FileModifyDate', 'FileName',
                       'FilePermissions', 'FileSize', 'FileType',
                       'FileTypeExtension', 'ImageHeight', 'ImageSize',
```

### Comparing `mat2-0.8.0/libmat2/epub.py` & `mat2-0.9.0/libmat2/epub.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import re
 import uuid
 import xml.etree.ElementTree as ET  # type: ignore
 
 from . import archive, office
 
-class EPUBParser(archive.ArchiveBasedAbstractParser):
+class EPUBParser(archive.ZipParser):
     mimetypes = {'application/epub+zip', }
     metadata_namespace = '{http://purl.org/dc/elements/1.1/}'
 
     def __init__(self, filename):
         super().__init__(filename)
         self.files_to_keep = set(map(re.compile, {  # type: ignore
             'META-INF/container.xml',
```

### Comparing `mat2-0.8.0/libmat2/torrent.py` & `mat2-0.9.0/libmat2/torrent.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,34 +2,34 @@
 from typing import Union, Tuple, Dict
 
 from . import abstract
 
 
 class TorrentParser(abstract.AbstractParser):
     mimetypes = {'application/x-bittorrent', }
-    whitelist = {b'announce', b'announce-list', b'info'}
+    allowlist = {b'announce', b'announce-list', b'info'}
 
     def __init__(self, filename):
         super().__init__(filename)
         with open(self.filename, 'rb') as f:
             self.dict_repr = _BencodeHandler().bdecode(f.read())
         if self.dict_repr is None:
             raise ValueError
 
     def get_meta(self) -> Dict[str, Union[str, dict]]:
         metadata = {}
         for key, value in self.dict_repr.items():
-            if key not in self.whitelist:
+            if key not in self.allowlist:
                 metadata[key.decode('utf-8')] = value
         return metadata
 
     def remove_all(self) -> bool:
         cleaned = dict()
         for key, value in self.dict_repr.items():
-            if key in self.whitelist:
+            if key in self.allowlist:
                 cleaned[key] = value
         with open(self.output_filename, 'wb') as f:
             f.write(_BencodeHandler().bencode(cleaned))
         self.dict_repr = cleaned  # since we're stateful
         return True
```

### Comparing `mat2-0.8.0/libmat2/__init__.py` & `mat2-0.9.0/libmat2/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,35 +26,43 @@
     '.wsdl',
     '.xpdl',
     '.xsd',
     '.xsl',
     }
 
 DEPENDENCIES = {
-    'cairo': 'Cairo',
-    'gi': 'PyGobject',
-    'gi.repository.GdkPixbuf': 'GdkPixbuf from PyGobject',
-    'gi.repository.Poppler': 'Poppler from PyGobject',
-    'gi.repository.GLib': 'GLib from PyGobject',
-    'mutagen': 'Mutagen',
+    'Cairo': 'cairo',
+    'PyGobject': 'gi',
+    'GdkPixbuf from PyGobject': 'gi.repository.GdkPixbuf',
+    'Poppler from PyGobject': 'gi.repository.Poppler',
+    'GLib from PyGobject': 'gi.repository.GLib',
+    'Mutagen': 'mutagen',
     }
 
+CMD_DEPENDENCIES = {
+    'Exiftool': exiftool._get_exiftool_path,
+    'Ffmpeg': video._get_ffmpeg_path,
+    }
 
 def check_dependencies() -> Dict[str, bool]:
     ret = collections.defaultdict(bool)  # type: Dict[str, bool]
 
-    ret['Exiftool'] = bool(exiftool._get_exiftool_path())
-    ret['Ffmpeg'] = bool(video._get_ffmpeg_path())
-
     for key, value in DEPENDENCIES.items():
-        ret[value] = True
+        ret[key] = True
         try:
-            importlib.import_module(key)
+            importlib.import_module(value)
         except ImportError:  # pragma: no cover
-            ret[value] = False  # pragma: no cover
+            ret[key] = False  # pragma: no cover
+
+    for k, v in CMD_DEPENDENCIES.items():
+        ret[k] = True
+        try:
+            v()
+        except RuntimeError:  # pragma: no cover
+            ret[k] = False
 
     return ret
 
 
 @enum.unique
 class UnknownMemberPolicy(enum.Enum):
     ABORT = 'abort'
```

### Comparing `mat2-0.8.0/libmat2/parser_factory.py` & `mat2-0.9.0/libmat2/parser_factory.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,21 +3,18 @@
 import os
 import mimetypes
 import importlib
 from typing import TypeVar, List, Tuple, Optional
 
 from . import abstract, UNSUPPORTED_EXTENSIONS
 
-assert Tuple  # make pyflakes happy
-
 T = TypeVar('T', bound='abstract.AbstractParser')
 
 mimetypes.add_type('application/epub+zip', '.epub')
-# EPUB Navigation Control XML File
-mimetypes.add_type('application/x-dtbncx+xml', '.ncx')
+mimetypes.add_type('application/x-dtbncx+xml', '.ncx')  # EPUB Navigation Control XML File
 
 
 def __load_all_parsers():
     """ Loads every parser in a dynamic way """
     current_dir = os.path.dirname(__file__)
     for fname in glob.glob(os.path.join(current_dir, '*.py')):
         if fname.endswith('abstract.py'):
@@ -39,21 +36,25 @@
     def __get_parsers(cls):
         return cls.__subclasses__() + \
             [g for s in cls.__subclasses__() for g in __get_parsers(s)]
     return __get_parsers(abstract.AbstractParser)
 
 
 def get_parser(filename: str) -> Tuple[Optional[T], Optional[str]]:
-    """ Return the appropriate parser for a giver filename. """
+    """ Return the appropriate parser for a given filename. """
     mtype, _ = mimetypes.guess_type(filename)
 
     _, extension = os.path.splitext(filename)
     if extension.lower() in UNSUPPORTED_EXTENSIONS:
         return None, mtype
 
+    if mtype == 'application/x-tar':
+        if extension[1:] in ('bz2', 'gz', 'xz'):
+            mtype = mtype + '+' + extension[1:]
+
     for parser_class in _get_parsers():  # type: ignore
         if mtype in parser_class.mimetypes:
             try:
                 return parser_class(filename), mtype
             except ValueError as e:
                 logging.info("Got an exception when trying to instanciate "
                              "%s for %s: %s", parser_class, filename, e)
```

### Comparing `mat2-0.8.0/libmat2/office.py` & `mat2-0.9.0/libmat2/office.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import re
 import zipfile
 from typing import Dict, Set, Pattern, Tuple, Any
 
 import xml.etree.ElementTree as ET  # type: ignore
 
-from .archive import ArchiveBasedAbstractParser
+from .archive import ZipParser
 
 # pylint: disable=line-too-long
 
 # Make pyflakes happy
 assert Set
 assert Pattern
 
@@ -39,15 +39,15 @@
     for c in tree.getroot():
         c[:] = sorted(c, key=lambda child: (child.tag, child.get('desc')))
 
     tree.write(full_path, xml_declaration=True)
     return True
 
 
-class MSOfficeParser(ArchiveBasedAbstractParser):
+class MSOfficeParser(ZipParser):
     mimetypes = {
         'application/vnd.openxmlformats-officedocument.wordprocessingml.document',
         'application/vnd.openxmlformats-officedocument.spreadsheetml.sheet',
         'application/vnd.openxmlformats-officedocument.presentationml.presentation'
     }
     content_types_to_keep = {
         'application/vnd.openxmlformats-officedocument.wordprocessingml.endnotes+xml',  # /word/endnotes.xml
@@ -85,26 +85,26 @@
             r'^customXml/',
             r'webSettings\.xml$',
             r'^docProps/custom\.xml$',
             r'^word/printerSettings/',
             r'^word/theme',
             r'^word/people\.xml$',
 
-            # we have a whitelist in self.files_to_keep,
+            # we have an allowlist in self.files_to_keep,
             # so we can trash everything else
             r'^word/_rels/',
         }))
 
         if self.__fill_files_to_keep_via_content_types() is False:
             raise ValueError
 
     def __fill_files_to_keep_via_content_types(self) -> bool:
         """ There is a suer-handy `[Content_Types].xml` file
         in MS Office archives, describing what each other file contains.
-        The self.content_types_to_keep member contains a type whitelist,
+        The self.content_types_to_keep member contains a type allowlist,
         so we're using it to fill the self.files_to_keep one.
         """
         with zipfile.ZipFile(self.filename) as zin:
             if '[Content_Types].xml' not in zin.namelist():
                 return False
             xml_data = zin.read('[Content_Types].xml')
 
@@ -216,15 +216,15 @@
 
         removed_fnames = set()
         with zipfile.ZipFile(self.filename) as zin:
             for fname in [item.filename for item in zin.infolist()]:
                 for file_to_omit in self.files_to_omit:
                     if file_to_omit.search(fname):
                         matches = map(lambda r: r.search(fname), self.files_to_keep)
-                        if any(matches):  # the file is whitelisted
+                        if any(matches):  # the file is in the allowlist
                             continue
                         removed_fnames.add(fname)
                         break
 
         root = tree.getroot()
         for item in root.findall('{%s}Override' % namespace['']):
             name = item.attrib['PartName'][1:]  # remove the leading '/'
@@ -308,15 +308,15 @@
                 results = re.findall(r"<(.+)>(.+)</\1>", f.read(), re.I|re.M)
                 return {k:v for (k, v) in results}
             except (TypeError, UnicodeDecodeError):
                 # We didn't manage to parse the xml file
                 return {file_path: 'harmful content', }
 
 
-class LibreOfficeParser(ArchiveBasedAbstractParser):
+class LibreOfficeParser(ZipParser):
     mimetypes = {
         'application/vnd.oasis.opendocument.text',
         'application/vnd.oasis.opendocument.spreadsheet',
         'application/vnd.oasis.opendocument.presentation',
         'application/vnd.oasis.opendocument.graphics',
         'application/vnd.oasis.opendocument.chart',
         'application/vnd.oasis.opendocument.formula',
```

### Comparing `mat2-0.8.0/libmat2/audio.py` & `mat2-0.9.0/libmat2/audio.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 class MP3Parser(MutagenParser):
     mimetypes = {'audio/mpeg', }
 
     def get_meta(self) -> Dict[str, Union[str, dict]]:
         metadata = {}  # type: Dict[str, Union[str, dict]]
         meta = mutagen.File(self.filename).tags
         for key in meta:
+            if not hasattr(meta[key], 'text'):  # pragma: no cover
+                continue
             metadata[key.rstrip(' \t\r\n\0')] = ', '.join(map(str, meta[key].text))
         return metadata
 
 
 class OGGParser(MutagenParser):
     mimetypes = {'audio/ogg', }
```

### Comparing `mat2-0.8.0/libmat2/pdf.py` & `mat2-0.9.0/libmat2/pdf.py`

 * *Files identical despite different names*

### Comparing `mat2-0.8.0/libmat2/exiftool.py` & `mat2-0.9.0/libmat2/exiftool.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 
 
 class ExiftoolParser(abstract.AbstractParser):
     """ Exiftool is often the easiest way to get all the metadata
     from a import file, hence why several parsers are re-using its `get_meta`
     method.
     """
-    meta_whitelist = set()  # type: Set[str]
+    meta_allowlist = set()  # type: Set[str]
 
     def get_meta(self) -> Dict[str, Union[str, dict]]:
         out = subprocess.run([_get_exiftool_path(), '-json', self.filename],
                              input_filename=self.filename,
                              check=True, stdout=subprocess.PIPE).stdout
         meta = json.loads(out.decode('utf-8'))[0]
-        for key in self.meta_whitelist:
+        for key in self.meta_allowlist:
             meta.pop(key, None)
         return meta
 
     def _lightweight_cleanup(self) -> bool:
         if os.path.exists(self.output_filename):
             try:
                 # exiftool can't force output to existing files
```

### Comparing `mat2-0.8.0/libmat2/web.py` & `mat2-0.9.0/libmat2/web.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,85 +33,85 @@
                     metadata[k.strip(string.whitespace + '*')] = v.strip()
                 except ValueError:
                     metadata['harmful data'] = line.strip()
         return metadata
 
 
 class AbstractHTMLParser(abstract.AbstractParser):
-    tags_blacklist = set()  # type: Set[str]
+    tags_blocklist = set()  # type: Set[str]
     # In some html/xml-based formats some tags are mandatory,
-    # so we're keeping them, but are discaring their content
-    tags_required_blacklist = set()  # type: Set[str]
+    # so we're keeping them, but are discarding their content
+    tags_required_blocklist = set()  # type: Set[str]
 
     def __init__(self, filename):
         super().__init__(filename)
-        self.__parser = _HTMLParser(self.filename, self.tags_blacklist,
-                                    self.tags_required_blacklist)
+        self.__parser = _HTMLParser(self.filename, self.tags_blocklist,
+                                    self.tags_required_blocklist)
         with open(filename, encoding='utf-8') as f:
             self.__parser.feed(f.read())
         self.__parser.close()
 
     def get_meta(self) -> Dict[str, Any]:
         return self.__parser.get_meta()
 
     def remove_all(self) -> bool:
         return self.__parser.remove_all(self.output_filename)
 
 
 class HTMLParser(AbstractHTMLParser):
-    mimetypes = {'text/html', }
-    tags_blacklist = {'meta', }
-    tags_required_blacklist = {'title', }
+    mimetypes = {'text/html', 'application/xhtml+xml'}
+    tags_blocklist = {'meta', }
+    tags_required_blocklist = {'title', }
 
 
 class DTBNCXParser(AbstractHTMLParser):
     mimetypes = {'application/x-dtbncx+xml', }
-    tags_required_blacklist = {'title', 'doctitle', 'meta'}
+    tags_required_blocklist = {'title', 'doctitle', 'meta'}
 
 
 class _HTMLParser(parser.HTMLParser):
     """Python doesn't have a validating html parser in its stdlib, so
     we're using an internal queue to track all the opening/closing tags,
     and hoping for the best.
 
     Moreover, the parser.HTMLParser call doesn't provide a get_endtag_text
     method, so we have to use get_starttag_text instead, put its result in a
     LIFO, and transform it in a closing tag when needed.
 
     Also, gotcha: the `tag` parameters are always in lowercase.
     """
-    def __init__(self, filename, blacklisted_tags, required_blacklisted_tags):
+    def __init__(self, filename, blocklisted_tags, required_blocklisted_tags):
         super().__init__()
         self.filename = filename
         self.__textrepr = ''
         self.__meta = {}
         self.__validation_queue = []  # type: List[str]
 
         # We're using counters instead of booleans, to handle nested tags
         self.__in_dangerous_but_required_tag = 0
         self.__in_dangerous_tag = 0
 
-        if required_blacklisted_tags & blacklisted_tags:  # pragma: nocover
+        if required_blocklisted_tags & blocklisted_tags:  # pragma: nocover
             raise ValueError("There is an overlap between %s and %s" % (
-                required_blacklisted_tags, blacklisted_tags))
-        self.tag_required_blacklist = required_blacklisted_tags
-        self.tag_blacklist = blacklisted_tags
+                required_blocklisted_tags, blocklisted_tags))
+        self.tag_required_blocklist = required_blocklisted_tags
+        self.tag_blocklist = blocklisted_tags
 
     def handle_starttag(self, tag: str, attrs: List[Tuple[str, str]]):
         original_tag = self.get_starttag_text()
         self.__validation_queue.append(original_tag)
 
-        if tag in self.tag_blacklist:
+        if tag in self.tag_blocklist:
             self.__in_dangerous_tag += 1
 
         if self.__in_dangerous_tag == 0:
             if self.__in_dangerous_but_required_tag == 0:
                 self.__textrepr += original_tag
 
-        if tag in self.tag_required_blacklist:
+        if tag in self.tag_required_blocklist:
             self.__in_dangerous_but_required_tag += 1
 
     def handle_endtag(self, tag: str):
         if not self.__validation_queue:
             raise ValueError("The closing tag %s doesn't have a corresponding "
                              "opening one in %s." % (tag, self.filename))
 
@@ -119,40 +119,40 @@
         previous_tag = previous_tag[1:-1]  # remove < and >
         previous_tag = previous_tag.split(' ')[0]  # remove attributes
         if tag != previous_tag.lower():
             raise ValueError("The closing tag %s doesn't match the previous "
                              "tag %s in %s" %
                              (tag, previous_tag, self.filename))
 
-        if tag in self.tag_required_blacklist:
+        if tag in self.tag_required_blocklist:
             self.__in_dangerous_but_required_tag -= 1
 
         if self.__in_dangerous_tag == 0:
             if self.__in_dangerous_but_required_tag == 0:
                 # There is no `get_endtag_text()` method :/
                 self.__textrepr += '</' + previous_tag + '>'
 
-        if tag in self.tag_blacklist:
+        if tag in self.tag_blocklist:
             self.__in_dangerous_tag -= 1
 
     def handle_data(self, data: str):
         if self.__in_dangerous_but_required_tag == 0:
             if self.__in_dangerous_tag == 0:
                 if data.strip():
                     self.__textrepr += escape(data)
 
     def handle_startendtag(self, tag: str, attrs: List[Tuple[str, str]]):
-        if tag in self.tag_required_blacklist | self.tag_blacklist:
+        if tag in self.tag_required_blocklist | self.tag_blocklist:
             meta = {k:v for k, v in attrs}
             name = meta.get('name', 'harmful metadata')
             content = meta.get('content', 'harmful data')
             self.__meta[name] = content
 
             if self.__in_dangerous_tag == 0:
-                if tag in self.tag_required_blacklist:
+                if tag in self.tag_required_blocklist:
                     self.__textrepr += '<' + tag + ' />'
                 return
 
         if self.__in_dangerous_tag == 0:
             if self.__in_dangerous_but_required_tag == 0:
                 self.__textrepr += self.get_starttag_text()
```

### Comparing `mat2-0.8.0/libmat2/subprocess.py` & `mat2-0.9.0/libmat2/subprocess.py`

 * *Files identical despite different names*

### Comparing `mat2-0.8.0/mat2.egg-info/PKG-INFO` & `mat2-0.9.0/mat2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat2
-Version: 0.8.0
+Version: 0.9.0
 Summary: A handy tool to trash your metadata
 Home-page: https://0xacab.org/jvoisin/mat2
 Author: Julien (jvoisin) Voisin
 Author-email: julien.voisin+mat2@dustri.org
 License: UNKNOWN
 Project-URL: bugtacker, https://0xacab.org/jvoisin/mat2/issues
 Description: ```
@@ -35,15 +35,15 @@
         metadata.
         
         # Requirements
         
         - `python3-mutagen` for audio support
         - `python3-gi-cairo` and `gir1.2-poppler-0.18` for PDF support
         - `gir1.2-gdkpixbuf-2.0` for images support
-        - `FFmpeg`, optionally, for video support 
+        - `FFmpeg`, optionally, for video support
         - `libimage-exiftool-perl` for everything else
         - `bubblewrap`, optionally, for sandboxing
         
         Please note that MAT2 requires at least Python3.5, meaning that it
         doesn't run on [Debian Jessie](https://packages.debian.org/jessie/python3).
         
         # Running the test suite
@@ -75,15 +75,16 @@
           -h, --help            show this help message and exit
           -v, --version         show program's version number and exit
           -l, --list            list all supported fileformats
           --check-dependencies  check if MAT2 has all the dependencies it needs
           -V, --verbose         show more verbose status information
           --unknown-members policy
                                 how to handle unknown members of archive-style files
-                                (policy should be one of: abort, omit, keep)
+                                (policy should be one of: abort, omit, keep) [Default:
+                                abort]
           -s, --show            list harmful metadata detectable by MAT2 without
                                 removing them
           -L, --lightweight     remove SOME metadata
         ```
         
         Note that MAT2 **will not** clean files in-place, but will produce, for
         example, with a file named "myfile.png" a cleaned version named
```

### Comparing `mat2-0.8.0/README.md` & `mat2-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -61,273 +61,276 @@
 000003c0: 6420 6067 6972 312e 322d 706f 7070 6c65  d `gir1.2-popple
 000003d0: 722d 302e 3138 6020 666f 7220 5044 4620  r-0.18` for PDF 
 000003e0: 7375 7070 6f72 740a 2d20 6067 6972 312e  support.- `gir1.
 000003f0: 322d 6764 6b70 6978 6275 662d 322e 3060  2-gdkpixbuf-2.0`
 00000400: 2066 6f72 2069 6d61 6765 7320 7375 7070   for images supp
 00000410: 6f72 740a 2d20 6046 466d 7065 6760 2c20  ort.- `FFmpeg`, 
 00000420: 6f70 7469 6f6e 616c 6c79 2c20 666f 7220  optionally, for 
-00000430: 7669 6465 6f20 7375 7070 6f72 7420 0a2d  video support .-
-00000440: 2060 6c69 6269 6d61 6765 2d65 7869 6674   `libimage-exift
-00000450: 6f6f 6c2d 7065 726c 6020 666f 7220 6576  ool-perl` for ev
-00000460: 6572 7974 6869 6e67 2065 6c73 650a 2d20  erything else.- 
-00000470: 6062 7562 626c 6577 7261 7060 2c20 6f70  `bubblewrap`, op
-00000480: 7469 6f6e 616c 6c79 2c20 666f 7220 7361  tionally, for sa
-00000490: 6e64 626f 7869 6e67 0a0a 506c 6561 7365  ndboxing..Please
-000004a0: 206e 6f74 6520 7468 6174 204d 4154 3220   note that MAT2 
-000004b0: 7265 7175 6972 6573 2061 7420 6c65 6173  requires at leas
-000004c0: 7420 5079 7468 6f6e 332e 352c 206d 6561  t Python3.5, mea
-000004d0: 6e69 6e67 2074 6861 7420 6974 0a64 6f65  ning that it.doe
-000004e0: 736e 2774 2072 756e 206f 6e20 5b44 6562  sn't run on [Deb
-000004f0: 6961 6e20 4a65 7373 6965 5d28 6874 7470  ian Jessie](http
-00000500: 733a 2f2f 7061 636b 6167 6573 2e64 6562  s://packages.deb
-00000510: 6961 6e2e 6f72 672f 6a65 7373 6965 2f70  ian.org/jessie/p
-00000520: 7974 686f 6e33 292e 0a0a 2320 5275 6e6e  ython3)...# Runn
-00000530: 696e 6720 7468 6520 7465 7374 2073 7569  ing the test sui
-00000540: 7465 0a0a 6060 6062 6173 680a 2420 7079  te..```bash.$ py
-00000550: 7468 6f6e 3320 2d6d 2075 6e69 7474 6573  thon3 -m unittes
-00000560: 7420 6469 7363 6f76 6572 202d 760a 6060  t discover -v.``
-00000570: 600a 0a41 6e64 2069 6620 796f 7520 7761  `..And if you wa
-00000580: 6e74 2074 6f20 7365 6520 7468 6520 636f  nt to see the co
-00000590: 7665 7261 6765 3a0a 0a60 6060 6261 7368  verage:..```bash
-000005a0: 0a24 2070 7974 686f 6e33 2d63 6f76 6572  .$ python3-cover
-000005b0: 6167 6520 7275 6e20 2d2d 6272 616e 6368  age run --branch
-000005c0: 202d 6d20 756e 6974 7465 7374 2064 6973   -m unittest dis
-000005d0: 636f 7665 7220 2d73 2074 6573 7473 2f0a  cover -s tests/.
-000005e0: 2420 7079 7468 6f6e 332d 636f 7665 7261  $ python3-covera
-000005f0: 6765 2072 6570 6f72 7420 2d2d 696e 636c  ge report --incl
-00000600: 7564 6520 2d6d 202d 2d69 6e63 6c75 6465  ude -m --include
-00000610: 202f 6c69 626d 6174 322f 2a27 0a60 6060   /libmat2/*'.```
-00000620: 0a0a 2320 486f 7720 746f 2075 7365 204d  ..# How to use M
-00000630: 4154 320a 0a60 6060 6261 7368 0a75 7361  AT2..```bash.usa
-00000640: 6765 3a20 6d61 7432 205b 2d68 5d20 5b2d  ge: mat2 [-h] [-
-00000650: 765d 205b 2d6c 5d20 5b2d 2d63 6865 636b  v] [-l] [--check
-00000660: 2d64 6570 656e 6465 6e63 6965 735d 205b  -dependencies] [
-00000670: 2d56 5d0a 2020 2020 2020 2020 2020 2020  -V].            
-00000680: 5b2d 2d75 6e6b 6e6f 776e 2d6d 656d 6265  [--unknown-membe
-00000690: 7273 2070 6f6c 6963 795d 205b 2d73 207c  rs policy] [-s |
-000006a0: 202d 4c5d 0a20 2020 2020 2020 2020 2020   -L].           
-000006b0: 205b 6669 6c65 7320 5b66 696c 6573 202e   [files [files .
-000006c0: 2e2e 5d5d 0a0a 4d65 7461 6461 7461 2061  ..]]..Metadata a
-000006d0: 6e6f 6e79 6d69 7361 7469 6f6e 2074 6f6f  nonymisation too
-000006e0: 6c6b 6974 2032 0a0a 706f 7369 7469 6f6e  lkit 2..position
-000006f0: 616c 2061 7267 756d 656e 7473 3a0a 2020  al arguments:.  
-00000700: 6669 6c65 7320 2020 2020 2020 2020 2020  files           
-00000710: 2020 2020 2020 7468 6520 6669 6c65 7320        the files 
-00000720: 746f 2070 726f 6365 7373 0a0a 6f70 7469  to process..opti
-00000730: 6f6e 616c 2061 7267 756d 656e 7473 3a0a  onal arguments:.
-00000740: 2020 2d68 2c20 2d2d 6865 6c70 2020 2020    -h, --help    
-00000750: 2020 2020 2020 2020 7368 6f77 2074 6869          show thi
-00000760: 7320 6865 6c70 206d 6573 7361 6765 2061  s help message a
-00000770: 6e64 2065 7869 740a 2020 2d76 2c20 2d2d  nd exit.  -v, --
-00000780: 7665 7273 696f 6e20 2020 2020 2020 2020  version         
-00000790: 7368 6f77 2070 726f 6772 616d 2773 2076  show program's v
-000007a0: 6572 7369 6f6e 206e 756d 6265 7220 616e  ersion number an
-000007b0: 6420 6578 6974 0a20 202d 6c2c 202d 2d6c  d exit.  -l, --l
-000007c0: 6973 7420 2020 2020 2020 2020 2020 206c  ist            l
-000007d0: 6973 7420 616c 6c20 7375 7070 6f72 7465  ist all supporte
-000007e0: 6420 6669 6c65 666f 726d 6174 730a 2020  d fileformats.  
-000007f0: 2d2d 6368 6563 6b2d 6465 7065 6e64 656e  --check-dependen
-00000800: 6369 6573 2020 6368 6563 6b20 6966 204d  cies  check if M
-00000810: 4154 3220 6861 7320 616c 6c20 7468 6520  AT2 has all the 
-00000820: 6465 7065 6e64 656e 6369 6573 2069 7420  dependencies it 
-00000830: 6e65 6564 730a 2020 2d56 2c20 2d2d 7665  needs.  -V, --ve
-00000840: 7262 6f73 6520 2020 2020 2020 2020 7368  rbose         sh
-00000850: 6f77 206d 6f72 6520 7665 7262 6f73 6520  ow more verbose 
-00000860: 7374 6174 7573 2069 6e66 6f72 6d61 7469  status informati
-00000870: 6f6e 0a20 202d 2d75 6e6b 6e6f 776e 2d6d  on.  --unknown-m
-00000880: 656d 6265 7273 2070 6f6c 6963 790a 2020  embers policy.  
+00000430: 7669 6465 6f20 7375 7070 6f72 740a 2d20  video support.- 
+00000440: 606c 6962 696d 6167 652d 6578 6966 746f  `libimage-exifto
+00000450: 6f6c 2d70 6572 6c60 2066 6f72 2065 7665  ol-perl` for eve
+00000460: 7279 7468 696e 6720 656c 7365 0a2d 2060  rything else.- `
+00000470: 6275 6262 6c65 7772 6170 602c 206f 7074  bubblewrap`, opt
+00000480: 696f 6e61 6c6c 792c 2066 6f72 2073 616e  ionally, for san
+00000490: 6462 6f78 696e 670a 0a50 6c65 6173 6520  dboxing..Please 
+000004a0: 6e6f 7465 2074 6861 7420 4d41 5432 2072  note that MAT2 r
+000004b0: 6571 7569 7265 7320 6174 206c 6561 7374  equires at least
+000004c0: 2050 7974 686f 6e33 2e35 2c20 6d65 616e   Python3.5, mean
+000004d0: 696e 6720 7468 6174 2069 740a 646f 6573  ing that it.does
+000004e0: 6e27 7420 7275 6e20 6f6e 205b 4465 6269  n't run on [Debi
+000004f0: 616e 204a 6573 7369 655d 2868 7474 7073  an Jessie](https
+00000500: 3a2f 2f70 6163 6b61 6765 732e 6465 6269  ://packages.debi
+00000510: 616e 2e6f 7267 2f6a 6573 7369 652f 7079  an.org/jessie/py
+00000520: 7468 6f6e 3329 2e0a 0a23 2052 756e 6e69  thon3)...# Runni
+00000530: 6e67 2074 6865 2074 6573 7420 7375 6974  ng the test suit
+00000540: 650a 0a60 6060 6261 7368 0a24 2070 7974  e..```bash.$ pyt
+00000550: 686f 6e33 202d 6d20 756e 6974 7465 7374  hon3 -m unittest
+00000560: 2064 6973 636f 7665 7220 2d76 0a60 6060   discover -v.```
+00000570: 0a0a 416e 6420 6966 2079 6f75 2077 616e  ..And if you wan
+00000580: 7420 746f 2073 6565 2074 6865 2063 6f76  t to see the cov
+00000590: 6572 6167 653a 0a0a 6060 6062 6173 680a  erage:..```bash.
+000005a0: 2420 7079 7468 6f6e 332d 636f 7665 7261  $ python3-covera
+000005b0: 6765 2072 756e 202d 2d62 7261 6e63 6820  ge run --branch 
+000005c0: 2d6d 2075 6e69 7474 6573 7420 6469 7363  -m unittest disc
+000005d0: 6f76 6572 202d 7320 7465 7374 732f 0a24  over -s tests/.$
+000005e0: 2070 7974 686f 6e33 2d63 6f76 6572 6167   python3-coverag
+000005f0: 6520 7265 706f 7274 202d 2d69 6e63 6c75  e report --inclu
+00000600: 6465 202d 6d20 2d2d 696e 636c 7564 6520  de -m --include 
+00000610: 2f6c 6962 6d61 7432 2f2a 270a 6060 600a  /libmat2/*'.```.
+00000620: 0a23 2048 6f77 2074 6f20 7573 6520 4d41  .# How to use MA
+00000630: 5432 0a0a 6060 6062 6173 680a 7573 6167  T2..```bash.usag
+00000640: 653a 206d 6174 3220 5b2d 685d 205b 2d76  e: mat2 [-h] [-v
+00000650: 5d20 5b2d 6c5d 205b 2d2d 6368 6563 6b2d  ] [-l] [--check-
+00000660: 6465 7065 6e64 656e 6369 6573 5d20 5b2d  dependencies] [-
+00000670: 565d 0a20 2020 2020 2020 2020 2020 205b  V].            [
+00000680: 2d2d 756e 6b6e 6f77 6e2d 6d65 6d62 6572  --unknown-member
+00000690: 7320 706f 6c69 6379 5d20 5b2d 7320 7c20  s policy] [-s | 
+000006a0: 2d4c 5d0a 2020 2020 2020 2020 2020 2020  -L].            
+000006b0: 5b66 696c 6573 205b 6669 6c65 7320 2e2e  [files [files ..
+000006c0: 2e5d 5d0a 0a4d 6574 6164 6174 6120 616e  .]]..Metadata an
+000006d0: 6f6e 796d 6973 6174 696f 6e20 746f 6f6c  onymisation tool
+000006e0: 6b69 7420 320a 0a70 6f73 6974 696f 6e61  kit 2..positiona
+000006f0: 6c20 6172 6775 6d65 6e74 733a 0a20 2066  l arguments:.  f
+00000700: 696c 6573 2020 2020 2020 2020 2020 2020  iles            
+00000710: 2020 2020 2074 6865 2066 696c 6573 2074       the files t
+00000720: 6f20 7072 6f63 6573 730a 0a6f 7074 696f  o process..optio
+00000730: 6e61 6c20 6172 6775 6d65 6e74 733a 0a20  nal arguments:. 
+00000740: 202d 682c 202d 2d68 656c 7020 2020 2020   -h, --help     
+00000750: 2020 2020 2020 2073 686f 7720 7468 6973         show this
+00000760: 2068 656c 7020 6d65 7373 6167 6520 616e   help message an
+00000770: 6420 6578 6974 0a20 202d 762c 202d 2d76  d exit.  -v, --v
+00000780: 6572 7369 6f6e 2020 2020 2020 2020 2073  ersion         s
+00000790: 686f 7720 7072 6f67 7261 6d27 7320 7665  how program's ve
+000007a0: 7273 696f 6e20 6e75 6d62 6572 2061 6e64  rsion number and
+000007b0: 2065 7869 740a 2020 2d6c 2c20 2d2d 6c69   exit.  -l, --li
+000007c0: 7374 2020 2020 2020 2020 2020 2020 6c69  st            li
+000007d0: 7374 2061 6c6c 2073 7570 706f 7274 6564  st all supported
+000007e0: 2066 696c 6566 6f72 6d61 7473 0a20 202d   fileformats.  -
+000007f0: 2d63 6865 636b 2d64 6570 656e 6465 6e63  -check-dependenc
+00000800: 6965 7320 2063 6865 636b 2069 6620 4d41  ies  check if MA
+00000810: 5432 2068 6173 2061 6c6c 2074 6865 2064  T2 has all the d
+00000820: 6570 656e 6465 6e63 6965 7320 6974 206e  ependencies it n
+00000830: 6565 6473 0a20 202d 562c 202d 2d76 6572  eeds.  -V, --ver
+00000840: 626f 7365 2020 2020 2020 2020 2073 686f  bose         sho
+00000850: 7720 6d6f 7265 2076 6572 626f 7365 2073  w more verbose s
+00000860: 7461 7475 7320 696e 666f 726d 6174 696f  tatus informatio
+00000870: 6e0a 2020 2d2d 756e 6b6e 6f77 6e2d 6d65  n.  --unknown-me
+00000880: 6d62 6572 7320 706f 6c69 6379 0a20 2020  mbers policy.   
 00000890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008a0: 2020 2020 2020 686f 7720 746f 2068 616e        how to han
-000008b0: 646c 6520 756e 6b6e 6f77 6e20 6d65 6d62  dle unknown memb
-000008c0: 6572 7320 6f66 2061 7263 6869 7665 2d73  ers of archive-s
-000008d0: 7479 6c65 2066 696c 6573 0a20 2020 2020  tyle files.     
+000008a0: 2020 2020 2068 6f77 2074 6f20 6861 6e64       how to hand
+000008b0: 6c65 2075 6e6b 6e6f 776e 206d 656d 6265  le unknown membe
+000008c0: 7273 206f 6620 6172 6368 6976 652d 7374  rs of archive-st
+000008d0: 796c 6520 6669 6c65 730a 2020 2020 2020  yle files.      
 000008e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008f0: 2020 2028 706f 6c69 6379 2073 686f 756c     (policy shoul
-00000900: 6420 6265 206f 6e65 206f 663a 2061 626f  d be one of: abo
-00000910: 7274 2c20 6f6d 6974 2c20 6b65 6570 290a  rt, omit, keep).
-00000920: 2020 2d73 2c20 2d2d 7368 6f77 2020 2020    -s, --show    
-00000930: 2020 2020 2020 2020 6c69 7374 2068 6172          list har
-00000940: 6d66 756c 206d 6574 6164 6174 6120 6465  mful metadata de
-00000950: 7465 6374 6162 6c65 2062 7920 4d41 5432  tectable by MAT2
-00000960: 2077 6974 686f 7574 0a20 2020 2020 2020   without.       
-00000970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000980: 2072 656d 6f76 696e 6720 7468 656d 0a20   removing them. 
-00000990: 202d 4c2c 202d 2d6c 6967 6874 7765 6967   -L, --lightweig
-000009a0: 6874 2020 2020 2072 656d 6f76 6520 534f  ht     remove SO
-000009b0: 4d45 206d 6574 6164 6174 610a 6060 600a  ME metadata.```.
-000009c0: 0a4e 6f74 6520 7468 6174 204d 4154 3220  .Note that MAT2 
-000009d0: 2a2a 7769 6c6c 206e 6f74 2a2a 2063 6c65  **will not** cle
-000009e0: 616e 2066 696c 6573 2069 6e2d 706c 6163  an files in-plac
-000009f0: 652c 2062 7574 2077 696c 6c20 7072 6f64  e, but will prod
-00000a00: 7563 652c 2066 6f72 0a65 7861 6d70 6c65  uce, for.example
-00000a10: 2c20 7769 7468 2061 2066 696c 6520 6e61  , with a file na
-00000a20: 6d65 6420 226d 7966 696c 652e 706e 6722  med "myfile.png"
-00000a30: 2061 2063 6c65 616e 6564 2076 6572 7369   a cleaned versi
-00000a40: 6f6e 206e 616d 6564 0a22 6d79 6669 6c65  on named."myfile
-00000a50: 2e63 6c65 616e 6564 2e70 6e67 222e 0a0a  .cleaned.png"...
-00000a60: 2320 4e6f 7465 7320 6162 6f75 7420 6465  # Notes about de
-00000a70: 7465 6374 696e 6720 6d65 7461 6461 7461  tecting metadata
-00000a80: 0a0a 5768 696c 6520 4d41 5432 2069 7320  ..While MAT2 is 
-00000a90: 646f 696e 6720 6974 7320 7665 7279 2062  doing its very b
-00000aa0: 6573 7420 746f 2064 6973 706c 6179 206d  est to display m
-00000ab0: 6574 6164 6174 6120 7768 656e 2074 6865  etadata when the
-00000ac0: 2060 2d2d 7368 6f77 6020 666c 6167 2069   `--show` flag i
-00000ad0: 730a 7061 7373 6564 2c20 6974 2064 6f65  s.passed, it doe
-00000ae0: 736e 2774 206d 6561 6e20 7468 6174 2061  sn't mean that a
-00000af0: 2066 696c 6520 6973 2063 6c65 616e 2066   file is clean f
-00000b00: 726f 6d20 616e 7920 6d65 7461 6461 7461  rom any metadata
-00000b10: 2069 6620 4d41 5432 2064 6f65 736e 2774   if MAT2 doesn't
-00000b20: 0a73 686f 7720 616e 792e 2054 6865 7265  .show any. There
-00000b30: 2069 7320 6e6f 2072 656c 6961 626c 6520   is no reliable 
-00000b40: 7761 7920 746f 2064 6574 6563 7420 6576  way to detect ev
-00000b50: 6572 7920 7369 6e67 6c65 2070 6f73 7369  ery single possi
-00000b60: 626c 6520 6d65 7461 6461 7461 2066 6f72  ble metadata for
-00000b70: 0a63 6f6d 706c 6578 2066 696c 6520 666f  .complex file fo
-00000b80: 726d 6174 732e 0a0a 5468 6973 2069 7320  rmats...This is 
-00000b90: 7768 7920 796f 7520 7368 6f75 6c64 6e27  why you shouldn'
-00000ba0: 7420 7265 6c79 206f 6e20 6d65 7461 6461  t rely on metada
-00000bb0: 7461 2773 2070 7265 7365 6e63 6520 746f  ta's presence to
-00000bc0: 2064 6563 6964 6520 6966 2079 6f75 7220   decide if your 
-00000bd0: 6669 6c65 206d 7573 740a 6265 2063 6c65  file must.be cle
-00000be0: 616e 6564 206f 7220 6e6f 742e 0a0a 2320  aned or not...# 
-00000bf0: 4e6f 7465 7320 6162 6f75 7420 7468 6520  Notes about the 
-00000c00: 6c69 6768 7477 6569 6768 7420 6d6f 6465  lightweight mode
-00000c10: 0a0a 4279 2064 6566 6175 6c74 2c20 6d61  ..By default, ma
-00000c20: 7432 206d 6967 6874 2061 6c74 6572 2061  t2 might alter a
-00000c30: 2062 6974 2074 6865 2064 6174 6120 6f66   bit the data of
-00000c40: 2079 6f75 7220 6669 6c65 732c 2069 6e20   your files, in 
-00000c50: 6f72 6465 7220 746f 2072 656d 6f76 650a  order to remove.
-00000c60: 6173 206d 7563 6820 6d65 7461 6461 7461  as much metadata
-00000c70: 2061 7320 706f 7373 6962 6c65 2e20 466f   as possible. Fo
-00000c80: 7220 6578 616d 706c 652c 2074 6578 7473  r example, texts
-00000c90: 2069 6e20 5044 4620 6d69 6768 7420 6e6f   in PDF might no
-00000ca0: 7420 6265 2073 656c 6563 7461 626c 6520  t be selectable 
-00000cb0: 616e 796d 6f72 652c 0a63 6f6d 7072 6573  anymore,.compres
-00000cc0: 7365 6420 696d 6167 6573 206d 6967 6874  sed images might
-00000cd0: 2067 6574 2063 6f6d 7072 6573 7365 6420   get compressed 
-00000ce0: 6167 6169 6e2c 20e2 80a6 0a53 696e 6365  again, ....Since
-00000cf0: 2073 6f6d 6520 7573 6572 7320 6d69 6768   some users migh
-00000d00: 7420 6265 2077 696c 6c69 6e67 2074 6f20  t be willing to 
-00000d10: 7472 6164 6520 736f 6d65 206d 6574 6164  trade some metad
-00000d20: 6174 6127 7320 7072 6573 656e 6365 2069  ata's presence i
-00000d30: 6e20 6578 6368 616e 6765 0a6f 6620 7468  n exchange.of th
-00000d40: 6520 6775 6172 616e 7465 6520 7468 6174  e guarantee that
-00000d50: 206d 6174 3220 776f 6e27 7420 6d6f 6469   mat2 won't modi
-00000d60: 6679 2074 6865 2064 6174 6120 6f66 2074  fy the data of t
-00000d70: 6865 6972 2066 696c 6573 2c20 7468 6572  heir files, ther
-00000d80: 6520 6973 2074 6865 0a60 2d4c 6020 666c  e is the.`-L` fl
-00000d90: 6167 2074 6861 7420 7072 6563 6973 656c  ag that precisel
-00000da0: 7920 646f 6573 2074 6861 742e 0a0a 2320  y does that...# 
-00000db0: 5265 6c61 7465 6420 736f 6674 7761 7265  Related software
-00000dc0: 0a0a 2d20 5468 6520 6669 7273 7420 6974  ..- The first it
-00000dd0: 6572 6174 696f 6e20 6f66 205b 4d41 545d  eration of [MAT]
-00000de0: 2868 7474 7073 3a2f 2f6d 6174 2e62 6f75  (https://mat.bou
-00000df0: 6d2e 6f72 6729 0a2d 205b 4578 6966 746f  m.org).- [Exifto
-00000e00: 6f6c 5d28 6874 7470 733a 2f2f 736e 6f2e  ol](https://sno.
-00000e10: 7068 792e 7175 6565 6e73 752e 6361 2f7e  phy.queensu.ca/~
-00000e20: 7068 696c 2f65 7869 6674 6f6f 6c2f 6d61  phil/exiftool/ma
-00000e30: 7429 0a2d 205b 7064 662d 7265 6461 6374  t).- [pdf-redact
-00000e40: 2d74 6f6f 6c73 5d28 6874 7470 733a 2f2f  -tools](https://
-00000e50: 6769 7468 7562 2e63 6f6d 2f66 6972 7374  github.com/first
-00000e60: 6c6f 6f6b 6d65 6469 612f 7064 662d 7265  lookmedia/pdf-re
-00000e70: 6461 6374 2d74 6f6f 6c73 292c 2074 6861  dact-tools), tha
-00000e80: 740a 0974 7269 6573 2074 6f20 6465 616c  t..tries to deal
-00000e90: 2077 6974 6820 2a70 7269 6e74 6572 2064   with *printer d
-00000ea0: 6f74 732a 2074 6f6f 2e0a 2d20 5b70 6466  ots* too..- [pdf
-00000eb0: 7061 7261 6e6f 6961 5d28 6874 7470 733a  paranoia](https:
-00000ec0: 2f2f 6769 7468 7562 2e63 6f6d 2f6b 616e  //github.com/kan
-00000ed0: 7a75 7265 2f70 6466 7061 7261 6e6f 6961  zure/pdfparanoia
-00000ee0: 292c 2074 6861 7420 7265 6d6f 7665 730a  ), that removes.
-00000ef0: 0977 6174 6572 6d61 726b 7320 6672 6f6d  .watermarks from
-00000f00: 2050 4446 2e0a 2d20 5b53 6372 616d 626c   PDF..- [Scrambl
-00000f10: 6564 2045 7869 665d 2868 7474 7073 3a2f  ed Exif](https:/
-00000f20: 2f66 2d64 726f 6964 2e6f 7267 2f70 6163  /f-droid.org/pac
-00000f30: 6b61 6765 732f 636f 6d2e 6a61 7273 696c  kages/com.jarsil
-00000f40: 696f 2e61 6e64 726f 6964 2e73 6372 616d  io.android.scram
-00000f50: 626c 6564 6567 6773 6966 2f29 2c0a 0961  bledeggsif/),..a
-00000f60: 6e20 6f70 656e 2d73 6f75 7263 6520 416e  n open-source An
-00000f70: 6472 6f69 6420 6170 706c 6963 6174 696f  droid applicatio
-00000f80: 6e20 746f 2072 656d 6f76 6520 6d65 7461  n to remove meta
-00000f90: 6461 7461 2066 726f 6d20 7069 6374 7572  data from pictur
-00000fa0: 6573 2e0a 0a23 2043 6f6e 7461 6374 0a0a  es...# Contact..
-00000fb0: 4966 2070 6f73 7369 626c 652c 2075 7365  If possible, use
-00000fc0: 2074 6865 205b 6973 7375 6573 2073 7973   the [issues sys
-00000fd0: 7465 6d5d 2868 7474 7073 3a2f 2f30 7861  tem](https://0xa
-00000fe0: 6361 622e 6f72 672f 6a76 6f69 7369 6e2f  cab.org/jvoisin/
-00000ff0: 6d61 7432 2f69 7373 7565 7329 0a6f 7220  mat2/issues).or 
-00001000: 7468 6520 5b6d 6169 6c69 6e67 206c 6973  the [mailing lis
-00001010: 745d 2868 7474 7073 3a2f 2f6d 6169 6c6d  t](https://mailm
-00001020: 616e 2e62 6f75 6d2e 6f72 672f 6c69 7374  an.boum.org/list
-00001030: 696e 666f 2f6d 6174 2d64 6576 290a 5368  info/mat-dev).Sh
-00001040: 6f75 6c64 2061 206d 6f72 6520 7072 6976  ould a more priv
-00001050: 6174 6520 636f 6e74 6163 7420 6265 206e  ate contact be n
-00001060: 6565 6465 6420 2865 672e 2066 6f72 2072  eeded (eg. for r
-00001070: 6570 6f72 7469 6e67 2073 6563 7572 6974  eporting securit
-00001080: 7920 6973 7375 6573 292c 0a79 6f75 2063  y issues),.you c
-00001090: 616e 2065 6d61 696c 204a 756c 6965 6e20  an email Julien 
-000010a0: 286a 766f 6973 696e 2920 566f 6973 696e  (jvoisin) Voisin
-000010b0: 2061 7420 606a 756c 6965 6e2e 766f 6973   at `julien.vois
-000010c0: 696e 2b6d 6174 3240 6475 7374 7269 2e6f  in+mat2@dustri.o
-000010d0: 7267 602c 0a75 7369 6e67 2074 6865 2067  rg`,.using the g
-000010e0: 7067 206b 6579 2060 3946 4344 4545 3945  pg key `9FCDEE9E
-000010f0: 3141 3338 3146 3331 3145 4136 3241 3734  1A381F311EA62A74
-00001100: 3034 4430 3431 4538 3137 3139 3031 4343  04D041E8171901CC
-00001110: 602e 0a0a 2320 4c69 6365 6e73 650a 0a54  `...# License..T
-00001120: 6869 7320 7072 6f67 7261 6d20 6973 2066  his program is f
-00001130: 7265 6520 736f 6674 7761 7265 3a20 796f  ree software: yo
-00001140: 7520 6361 6e20 7265 6469 7374 7269 6275  u can redistribu
-00001150: 7465 2069 7420 616e 642f 6f72 206d 6f64  te it and/or mod
-00001160: 6966 790a 6974 2075 6e64 6572 2074 6865  ify.it under the
-00001170: 2074 6572 6d73 206f 6620 7468 6520 474e   terms of the GN
-00001180: 5520 4c65 7373 6572 2047 656e 6572 616c  U Lesser General
-00001190: 2050 7562 6c69 6320 4c69 6365 6e73 6520   Public License 
-000011a0: 6173 2070 7562 6c69 7368 6564 2062 790a  as published by.
-000011b0: 7468 6520 4672 6565 2053 6f66 7477 6172  the Free Softwar
-000011c0: 6520 466f 756e 6461 7469 6f6e 2c20 6569  e Foundation, ei
-000011d0: 7468 6572 2076 6572 7369 6f6e 2033 206f  ther version 3 o
-000011e0: 6620 7468 6520 4c69 6365 6e73 652c 206f  f the License, o
-000011f0: 720a 2861 7420 796f 7572 206f 7074 696f  r.(at your optio
-00001200: 6e29 2061 6e79 206c 6174 6572 2076 6572  n) any later ver
-00001210: 7369 6f6e 2e0a 0a54 6869 7320 7072 6f67  sion...This prog
-00001220: 7261 6d20 6973 2064 6973 7472 6962 7574  ram is distribut
-00001230: 6564 2069 6e20 7468 6520 686f 7065 2074  ed in the hope t
-00001240: 6861 7420 6974 2077 696c 6c20 6265 2075  hat it will be u
-00001250: 7365 6675 6c2c 0a62 7574 2057 4954 484f  seful,.but WITHO
-00001260: 5554 2041 4e59 2057 4152 5241 4e54 593b  UT ANY WARRANTY;
-00001270: 2077 6974 686f 7574 2065 7665 6e20 7468   without even th
-00001280: 6520 696d 706c 6965 6420 7761 7272 616e  e implied warran
-00001290: 7479 206f 660a 4d45 5243 4841 4e54 4142  ty of.MERCHANTAB
-000012a0: 494c 4954 5920 6f72 2046 4954 4e45 5353  ILITY or FITNESS
-000012b0: 2046 4f52 2041 2050 4152 5449 4355 4c41   FOR A PARTICULA
-000012c0: 5220 5055 5250 4f53 452e 2020 5365 6520  R PURPOSE.  See 
-000012d0: 7468 650a 474e 5520 4765 6e65 7261 6c20  the.GNU General 
-000012e0: 5075 626c 6963 204c 6963 656e 7365 2066  Public License f
-000012f0: 6f72 206d 6f72 6520 6465 7461 696c 732e  or more details.
-00001300: 0a0a 596f 7520 7368 6f75 6c64 2068 6176  ..You should hav
-00001310: 6520 7265 6365 6976 6564 2061 2063 6f70  e received a cop
-00001320: 7920 6f66 2074 6865 2047 4e55 204c 6573  y of the GNU Les
-00001330: 7365 7220 4765 6e65 7261 6c20 5075 626c  ser General Publ
-00001340: 6963 204c 6963 656e 7365 0a61 6c6f 6e67  ic License.along
-00001350: 2077 6974 6820 7468 6973 2070 726f 6772   with this progr
-00001360: 616d 2e20 2049 6620 6e6f 742c 2073 6565  am.  If not, see
-00001370: 203c 6874 7470 3a2f 2f77 7777 2e67 6e75   <http://www.gnu
-00001380: 2e6f 7267 2f6c 6963 656e 7365 732f 3e2e  .org/licenses/>.
-00001390: 0a0a 436f 7079 7269 6768 7420 3230 3138  ..Copyright 2018
-000013a0: 204a 756c 6965 6e20 286a 766f 6973 696e   Julien (jvoisin
-000013b0: 2920 566f 6973 696e 203c 6a75 6c69 656e  ) Voisin <julien
-000013c0: 2e76 6f69 7369 6e2b 6d61 7432 4064 7573  .voisin+mat2@dus
-000013d0: 7472 692e 6f72 673e 0a43 6f70 7972 6967  tri.org>.Copyrig
-000013e0: 6874 2032 3031 3620 4d61 7269 6520 526f  ht 2016 Marie Ro
-000013f0: 7365 2066 6f72 204d 4154 3227 7320 6c6f  se for MAT2's lo
-00001400: 676f 0a0a 2320 5468 616e 6b73 0a0a 4d41  go..# Thanks..MA
-00001410: 5432 2077 6f75 6c64 6e27 7420 6578 6973  T2 wouldn't exis
-00001420: 7420 7769 7468 6f75 743a 0a0a 2d20 7468  t without:..- th
-00001430: 6520 5b47 6f6f 676c 6520 5375 6d6d 6572  e [Google Summer
-00001440: 206f 6620 436f 6465 5d28 6874 7470 733a   of Code](https:
-00001450: 2f2f 7375 6d6d 6572 6f66 636f 6465 2e77  //summerofcode.w
-00001460: 6974 6867 6f6f 676c 652e 636f 6d2f 293b  ithgoogle.com/);
-00001470: 0a2d 2074 6865 2066 696e 6520 7065 6f70  .- the fine peop
-00001480: 6c65 2066 726f 6d20 5b54 6169 6c73 5d28  le from [Tails](
-00001490: 2068 7474 7073 3a2f 2f74 6169 6c73 2e62   https://tails.b
-000014a0: 6f75 6d2e 6f72 6729 3b0a 2d20 6672 6965  oum.org);.- frie
-000014b0: 6e64 730a 0a4d 616e 7920 7468 616e 6b73  nds..Many thanks
-000014c0: 2074 6f20 7468 656d 210a 0a               to them!..
+000008f0: 2020 2870 6f6c 6963 7920 7368 6f75 6c64    (policy should
+00000900: 2062 6520 6f6e 6520 6f66 3a20 6162 6f72   be one of: abor
+00000910: 742c 206f 6d69 742c 206b 6565 7029 205b  t, omit, keep) [
+00000920: 4465 6661 756c 743a 0a20 2020 2020 2020  Default:.       
+00000930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000940: 2061 626f 7274 5d0a 2020 2d73 2c20 2d2d   abort].  -s, --
+00000950: 7368 6f77 2020 2020 2020 2020 2020 2020  show            
+00000960: 6c69 7374 2068 6172 6d66 756c 206d 6574  list harmful met
+00000970: 6164 6174 6120 6465 7465 6374 6162 6c65  adata detectable
+00000980: 2062 7920 4d41 5432 2077 6974 686f 7574   by MAT2 without
+00000990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000009a0: 2020 2020 2020 2020 2072 656d 6f76 696e           removin
+000009b0: 6720 7468 656d 0a20 202d 4c2c 202d 2d6c  g them.  -L, --l
+000009c0: 6967 6874 7765 6967 6874 2020 2020 2072  ightweight     r
+000009d0: 656d 6f76 6520 534f 4d45 206d 6574 6164  emove SOME metad
+000009e0: 6174 610a 6060 600a 0a4e 6f74 6520 7468  ata.```..Note th
+000009f0: 6174 204d 4154 3220 2a2a 7769 6c6c 206e  at MAT2 **will n
+00000a00: 6f74 2a2a 2063 6c65 616e 2066 696c 6573  ot** clean files
+00000a10: 2069 6e2d 706c 6163 652c 2062 7574 2077   in-place, but w
+00000a20: 696c 6c20 7072 6f64 7563 652c 2066 6f72  ill produce, for
+00000a30: 0a65 7861 6d70 6c65 2c20 7769 7468 2061  .example, with a
+00000a40: 2066 696c 6520 6e61 6d65 6420 226d 7966   file named "myf
+00000a50: 696c 652e 706e 6722 2061 2063 6c65 616e  ile.png" a clean
+00000a60: 6564 2076 6572 7369 6f6e 206e 616d 6564  ed version named
+00000a70: 0a22 6d79 6669 6c65 2e63 6c65 616e 6564  ."myfile.cleaned
+00000a80: 2e70 6e67 222e 0a0a 2320 4e6f 7465 7320  .png"...# Notes 
+00000a90: 6162 6f75 7420 6465 7465 6374 696e 6720  about detecting 
+00000aa0: 6d65 7461 6461 7461 0a0a 5768 696c 6520  metadata..While 
+00000ab0: 4d41 5432 2069 7320 646f 696e 6720 6974  MAT2 is doing it
+00000ac0: 7320 7665 7279 2062 6573 7420 746f 2064  s very best to d
+00000ad0: 6973 706c 6179 206d 6574 6164 6174 6120  isplay metadata 
+00000ae0: 7768 656e 2074 6865 2060 2d2d 7368 6f77  when the `--show
+00000af0: 6020 666c 6167 2069 730a 7061 7373 6564  ` flag is.passed
+00000b00: 2c20 6974 2064 6f65 736e 2774 206d 6561  , it doesn't mea
+00000b10: 6e20 7468 6174 2061 2066 696c 6520 6973  n that a file is
+00000b20: 2063 6c65 616e 2066 726f 6d20 616e 7920   clean from any 
+00000b30: 6d65 7461 6461 7461 2069 6620 4d41 5432  metadata if MAT2
+00000b40: 2064 6f65 736e 2774 0a73 686f 7720 616e   doesn't.show an
+00000b50: 792e 2054 6865 7265 2069 7320 6e6f 2072  y. There is no r
+00000b60: 656c 6961 626c 6520 7761 7920 746f 2064  eliable way to d
+00000b70: 6574 6563 7420 6576 6572 7920 7369 6e67  etect every sing
+00000b80: 6c65 2070 6f73 7369 626c 6520 6d65 7461  le possible meta
+00000b90: 6461 7461 2066 6f72 0a63 6f6d 706c 6578  data for.complex
+00000ba0: 2066 696c 6520 666f 726d 6174 732e 0a0a   file formats...
+00000bb0: 5468 6973 2069 7320 7768 7920 796f 7520  This is why you 
+00000bc0: 7368 6f75 6c64 6e27 7420 7265 6c79 206f  shouldn't rely o
+00000bd0: 6e20 6d65 7461 6461 7461 2773 2070 7265  n metadata's pre
+00000be0: 7365 6e63 6520 746f 2064 6563 6964 6520  sence to decide 
+00000bf0: 6966 2079 6f75 7220 6669 6c65 206d 7573  if your file mus
+00000c00: 740a 6265 2063 6c65 616e 6564 206f 7220  t.be cleaned or 
+00000c10: 6e6f 742e 0a0a 2320 4e6f 7465 7320 6162  not...# Notes ab
+00000c20: 6f75 7420 7468 6520 6c69 6768 7477 6569  out the lightwei
+00000c30: 6768 7420 6d6f 6465 0a0a 4279 2064 6566  ght mode..By def
+00000c40: 6175 6c74 2c20 6d61 7432 206d 6967 6874  ault, mat2 might
+00000c50: 2061 6c74 6572 2061 2062 6974 2074 6865   alter a bit the
+00000c60: 2064 6174 6120 6f66 2079 6f75 7220 6669   data of your fi
+00000c70: 6c65 732c 2069 6e20 6f72 6465 7220 746f  les, in order to
+00000c80: 2072 656d 6f76 650a 6173 206d 7563 6820   remove.as much 
+00000c90: 6d65 7461 6461 7461 2061 7320 706f 7373  metadata as poss
+00000ca0: 6962 6c65 2e20 466f 7220 6578 616d 706c  ible. For exampl
+00000cb0: 652c 2074 6578 7473 2069 6e20 5044 4620  e, texts in PDF 
+00000cc0: 6d69 6768 7420 6e6f 7420 6265 2073 656c  might not be sel
+00000cd0: 6563 7461 626c 6520 616e 796d 6f72 652c  ectable anymore,
+00000ce0: 0a63 6f6d 7072 6573 7365 6420 696d 6167  .compressed imag
+00000cf0: 6573 206d 6967 6874 2067 6574 2063 6f6d  es might get com
+00000d00: 7072 6573 7365 6420 6167 6169 6e2c 20e2  pressed again, .
+00000d10: 80a6 0a53 696e 6365 2073 6f6d 6520 7573  ...Since some us
+00000d20: 6572 7320 6d69 6768 7420 6265 2077 696c  ers might be wil
+00000d30: 6c69 6e67 2074 6f20 7472 6164 6520 736f  ling to trade so
+00000d40: 6d65 206d 6574 6164 6174 6127 7320 7072  me metadata's pr
+00000d50: 6573 656e 6365 2069 6e20 6578 6368 616e  esence in exchan
+00000d60: 6765 0a6f 6620 7468 6520 6775 6172 616e  ge.of the guaran
+00000d70: 7465 6520 7468 6174 206d 6174 3220 776f  tee that mat2 wo
+00000d80: 6e27 7420 6d6f 6469 6679 2074 6865 2064  n't modify the d
+00000d90: 6174 6120 6f66 2074 6865 6972 2066 696c  ata of their fil
+00000da0: 6573 2c20 7468 6572 6520 6973 2074 6865  es, there is the
+00000db0: 0a60 2d4c 6020 666c 6167 2074 6861 7420  .`-L` flag that 
+00000dc0: 7072 6563 6973 656c 7920 646f 6573 2074  precisely does t
+00000dd0: 6861 742e 0a0a 2320 5265 6c61 7465 6420  hat...# Related 
+00000de0: 736f 6674 7761 7265 0a0a 2d20 5468 6520  software..- The 
+00000df0: 6669 7273 7420 6974 6572 6174 696f 6e20  first iteration 
+00000e00: 6f66 205b 4d41 545d 2868 7474 7073 3a2f  of [MAT](https:/
+00000e10: 2f6d 6174 2e62 6f75 6d2e 6f72 6729 0a2d  /mat.boum.org).-
+00000e20: 205b 4578 6966 746f 6f6c 5d28 6874 7470   [Exiftool](http
+00000e30: 733a 2f2f 736e 6f2e 7068 792e 7175 6565  s://sno.phy.quee
+00000e40: 6e73 752e 6361 2f7e 7068 696c 2f65 7869  nsu.ca/~phil/exi
+00000e50: 6674 6f6f 6c2f 6d61 7429 0a2d 205b 7064  ftool/mat).- [pd
+00000e60: 662d 7265 6461 6374 2d74 6f6f 6c73 5d28  f-redact-tools](
+00000e70: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000e80: 6f6d 2f66 6972 7374 6c6f 6f6b 6d65 6469  om/firstlookmedi
+00000e90: 612f 7064 662d 7265 6461 6374 2d74 6f6f  a/pdf-redact-too
+00000ea0: 6c73 292c 2074 6861 740a 0974 7269 6573  ls), that..tries
+00000eb0: 2074 6f20 6465 616c 2077 6974 6820 2a70   to deal with *p
+00000ec0: 7269 6e74 6572 2064 6f74 732a 2074 6f6f  rinter dots* too
+00000ed0: 2e0a 2d20 5b70 6466 7061 7261 6e6f 6961  ..- [pdfparanoia
+00000ee0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000ef0: 2e63 6f6d 2f6b 616e 7a75 7265 2f70 6466  .com/kanzure/pdf
+00000f00: 7061 7261 6e6f 6961 292c 2074 6861 7420  paranoia), that 
+00000f10: 7265 6d6f 7665 730a 0977 6174 6572 6d61  removes..waterma
+00000f20: 726b 7320 6672 6f6d 2050 4446 2e0a 2d20  rks from PDF..- 
+00000f30: 5b53 6372 616d 626c 6564 2045 7869 665d  [Scrambled Exif]
+00000f40: 2868 7474 7073 3a2f 2f66 2d64 726f 6964  (https://f-droid
+00000f50: 2e6f 7267 2f70 6163 6b61 6765 732f 636f  .org/packages/co
+00000f60: 6d2e 6a61 7273 696c 696f 2e61 6e64 726f  m.jarsilio.andro
+00000f70: 6964 2e73 6372 616d 626c 6564 6567 6773  id.scrambledeggs
+00000f80: 6966 2f29 2c0a 0961 6e20 6f70 656e 2d73  if/),..an open-s
+00000f90: 6f75 7263 6520 416e 6472 6f69 6420 6170  ource Android ap
+00000fa0: 706c 6963 6174 696f 6e20 746f 2072 656d  plication to rem
+00000fb0: 6f76 6520 6d65 7461 6461 7461 2066 726f  ove metadata fro
+00000fc0: 6d20 7069 6374 7572 6573 2e0a 0a23 2043  m pictures...# C
+00000fd0: 6f6e 7461 6374 0a0a 4966 2070 6f73 7369  ontact..If possi
+00000fe0: 626c 652c 2075 7365 2074 6865 205b 6973  ble, use the [is
+00000ff0: 7375 6573 2073 7973 7465 6d5d 2868 7474  sues system](htt
+00001000: 7073 3a2f 2f30 7861 6361 622e 6f72 672f  ps://0xacab.org/
+00001010: 6a76 6f69 7369 6e2f 6d61 7432 2f69 7373  jvoisin/mat2/iss
+00001020: 7565 7329 0a6f 7220 7468 6520 5b6d 6169  ues).or the [mai
+00001030: 6c69 6e67 206c 6973 745d 2868 7474 7073  ling list](https
+00001040: 3a2f 2f6d 6169 6c6d 616e 2e62 6f75 6d2e  ://mailman.boum.
+00001050: 6f72 672f 6c69 7374 696e 666f 2f6d 6174  org/listinfo/mat
+00001060: 2d64 6576 290a 5368 6f75 6c64 2061 206d  -dev).Should a m
+00001070: 6f72 6520 7072 6976 6174 6520 636f 6e74  ore private cont
+00001080: 6163 7420 6265 206e 6565 6465 6420 2865  act be needed (e
+00001090: 672e 2066 6f72 2072 6570 6f72 7469 6e67  g. for reporting
+000010a0: 2073 6563 7572 6974 7920 6973 7375 6573   security issues
+000010b0: 292c 0a79 6f75 2063 616e 2065 6d61 696c  ),.you can email
+000010c0: 204a 756c 6965 6e20 286a 766f 6973 696e   Julien (jvoisin
+000010d0: 2920 566f 6973 696e 2061 7420 606a 756c  ) Voisin at `jul
+000010e0: 6965 6e2e 766f 6973 696e 2b6d 6174 3240  ien.voisin+mat2@
+000010f0: 6475 7374 7269 2e6f 7267 602c 0a75 7369  dustri.org`,.usi
+00001100: 6e67 2074 6865 2067 7067 206b 6579 2060  ng the gpg key `
+00001110: 3946 4344 4545 3945 3141 3338 3146 3331  9FCDEE9E1A381F31
+00001120: 3145 4136 3241 3734 3034 4430 3431 4538  1EA62A7404D041E8
+00001130: 3137 3139 3031 4343 602e 0a0a 2320 4c69  171901CC`...# Li
+00001140: 6365 6e73 650a 0a54 6869 7320 7072 6f67  cense..This prog
+00001150: 7261 6d20 6973 2066 7265 6520 736f 6674  ram is free soft
+00001160: 7761 7265 3a20 796f 7520 6361 6e20 7265  ware: you can re
+00001170: 6469 7374 7269 6275 7465 2069 7420 616e  distribute it an
+00001180: 642f 6f72 206d 6f64 6966 790a 6974 2075  d/or modify.it u
+00001190: 6e64 6572 2074 6865 2074 6572 6d73 206f  nder the terms o
+000011a0: 6620 7468 6520 474e 5520 4c65 7373 6572  f the GNU Lesser
+000011b0: 2047 656e 6572 616c 2050 7562 6c69 6320   General Public 
+000011c0: 4c69 6365 6e73 6520 6173 2070 7562 6c69  License as publi
+000011d0: 7368 6564 2062 790a 7468 6520 4672 6565  shed by.the Free
+000011e0: 2053 6f66 7477 6172 6520 466f 756e 6461   Software Founda
+000011f0: 7469 6f6e 2c20 6569 7468 6572 2076 6572  tion, either ver
+00001200: 7369 6f6e 2033 206f 6620 7468 6520 4c69  sion 3 of the Li
+00001210: 6365 6e73 652c 206f 720a 2861 7420 796f  cense, or.(at yo
+00001220: 7572 206f 7074 696f 6e29 2061 6e79 206c  ur option) any l
+00001230: 6174 6572 2076 6572 7369 6f6e 2e0a 0a54  ater version...T
+00001240: 6869 7320 7072 6f67 7261 6d20 6973 2064  his program is d
+00001250: 6973 7472 6962 7574 6564 2069 6e20 7468  istributed in th
+00001260: 6520 686f 7065 2074 6861 7420 6974 2077  e hope that it w
+00001270: 696c 6c20 6265 2075 7365 6675 6c2c 0a62  ill be useful,.b
+00001280: 7574 2057 4954 484f 5554 2041 4e59 2057  ut WITHOUT ANY W
+00001290: 4152 5241 4e54 593b 2077 6974 686f 7574  ARRANTY; without
+000012a0: 2065 7665 6e20 7468 6520 696d 706c 6965   even the implie
+000012b0: 6420 7761 7272 616e 7479 206f 660a 4d45  d warranty of.ME
+000012c0: 5243 4841 4e54 4142 494c 4954 5920 6f72  RCHANTABILITY or
+000012d0: 2046 4954 4e45 5353 2046 4f52 2041 2050   FITNESS FOR A P
+000012e0: 4152 5449 4355 4c41 5220 5055 5250 4f53  ARTICULAR PURPOS
+000012f0: 452e 2020 5365 6520 7468 650a 474e 5520  E.  See the.GNU 
+00001300: 4765 6e65 7261 6c20 5075 626c 6963 204c  General Public L
+00001310: 6963 656e 7365 2066 6f72 206d 6f72 6520  icense for more 
+00001320: 6465 7461 696c 732e 0a0a 596f 7520 7368  details...You sh
+00001330: 6f75 6c64 2068 6176 6520 7265 6365 6976  ould have receiv
+00001340: 6564 2061 2063 6f70 7920 6f66 2074 6865  ed a copy of the
+00001350: 2047 4e55 204c 6573 7365 7220 4765 6e65   GNU Lesser Gene
+00001360: 7261 6c20 5075 626c 6963 204c 6963 656e  ral Public Licen
+00001370: 7365 0a61 6c6f 6e67 2077 6974 6820 7468  se.along with th
+00001380: 6973 2070 726f 6772 616d 2e20 2049 6620  is program.  If 
+00001390: 6e6f 742c 2073 6565 203c 6874 7470 3a2f  not, see <http:/
+000013a0: 2f77 7777 2e67 6e75 2e6f 7267 2f6c 6963  /www.gnu.org/lic
+000013b0: 656e 7365 732f 3e2e 0a0a 436f 7079 7269  enses/>...Copyri
+000013c0: 6768 7420 3230 3138 204a 756c 6965 6e20  ght 2018 Julien 
+000013d0: 286a 766f 6973 696e 2920 566f 6973 696e  (jvoisin) Voisin
+000013e0: 203c 6a75 6c69 656e 2e76 6f69 7369 6e2b   <julien.voisin+
+000013f0: 6d61 7432 4064 7573 7472 692e 6f72 673e  mat2@dustri.org>
+00001400: 0a43 6f70 7972 6967 6874 2032 3031 3620  .Copyright 2016 
+00001410: 4d61 7269 6520 526f 7365 2066 6f72 204d  Marie Rose for M
+00001420: 4154 3227 7320 6c6f 676f 0a0a 2320 5468  AT2's logo..# Th
+00001430: 616e 6b73 0a0a 4d41 5432 2077 6f75 6c64  anks..MAT2 would
+00001440: 6e27 7420 6578 6973 7420 7769 7468 6f75  n't exist withou
+00001450: 743a 0a0a 2d20 7468 6520 5b47 6f6f 676c  t:..- the [Googl
+00001460: 6520 5375 6d6d 6572 206f 6620 436f 6465  e Summer of Code
+00001470: 5d28 6874 7470 733a 2f2f 7375 6d6d 6572  ](https://summer
+00001480: 6f66 636f 6465 2e77 6974 6867 6f6f 676c  ofcode.withgoogl
+00001490: 652e 636f 6d2f 293b 0a2d 2074 6865 2066  e.com/);.- the f
+000014a0: 696e 6520 7065 6f70 6c65 2066 726f 6d20  ine people from 
+000014b0: 5b54 6169 6c73 5d28 2068 7474 7073 3a2f  [Tails]( https:/
+000014c0: 2f74 6169 6c73 2e62 6f75 6d2e 6f72 6729  /tails.boum.org)
+000014d0: 3b0a 2d20 6672 6965 6e64 730a 0a4d 616e  ;.- friends..Man
+000014e0: 7920 7468 616e 6b73 2074 6f20 7468 656d  y thanks to them
+000014f0: 210a 0a                                  !..
```

