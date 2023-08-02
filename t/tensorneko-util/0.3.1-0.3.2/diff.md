# Comparing `tmp/tensorneko_util-0.3.1.tar.gz` & `tmp/tensorneko_util-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorneko_util-0.3.1.tar", last modified: Fri Jul 28 09:05:53 2023, max compression
+gzip compressed data, was "tensorneko_util-0.3.2.tar", last modified: Wed Aug  2 12:19:48 2023, max compression
```

## Comparing `tensorneko_util-0.3.1.tar` & `tensorneko_util-0.3.2.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.139932 tensorneko_util-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-07-28 09:05:53.139932 tensorneko_util-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    17201 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-28 09:05:53.143932 tensorneko_util-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)     1906 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/setup_util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.099932 tensorneko_util-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.103932 tensorneko_util-0.3.1/src/tensorneko_util/
--rw-r--r--   0 runner    (1001) docker     (122)      401 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.107932 tensorneko_util-0.3.1/src/tensorneko_util/backend/
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/backend/_tqdm.py
--rw-r--r--   0 runner    (1001) docker     (122)      482 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/backend/audio_lib.py
--rw-r--r--   0 runner    (1001) docker     (122)      592 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/backend/blocking.py
--rw-r--r--   0 runner    (1001) docker     (122)     4251 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/backend/parallel.py
--rw-r--r--   0 runner    (1001) docker     (122)     2895 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/backend/visual_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.107932 tensorneko_util-0.3.1/src/tensorneko_util/debug/
--rw-r--r--   0 runner    (1001) docker     (122)      118 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/debug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1010 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/debug/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.107932 tensorneko_util-0.3.1/src/tensorneko_util/io/
--rw-r--r--   0 runner    (1001) docker     (122)      291 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      871 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/_default_backends.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.107932 tensorneko_util-0.3.1/src/tensorneko_util/io/audio/
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      463 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/audio/audio_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     1509 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/audio/audio_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)     2541 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/audio/audio_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.111932 tensorneko_util-0.3.1/src/tensorneko_util/io/hdf5/
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/hdf5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      378 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/hdf5/hdf5_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)      262 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/hdf5/hdf5_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.111932 tensorneko_util-0.3.1/src/tensorneko_util/io/image/
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2726 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/image/image_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)     6628 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/image/image_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.111932 tensorneko_util-0.3.1/src/tensorneko_util/io/json/
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2423 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/json/json_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     2196 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/json/json_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)     2213 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/json/json_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.111932 tensorneko_util-0.3.1/src/tensorneko_util/io/matlab/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/matlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      437 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/matlab/mat_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)      515 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/matlab/mat_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.115932 tensorneko_util-0.3.1/src/tensorneko_util/io/pickle/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/pickle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      429 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/pickle/pickle_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)      508 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/pickle/pickle_writer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2192 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.115932 tensorneko_util-0.3.1/src/tensorneko_util/io/text/
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      668 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/text/text_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)      698 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/text/text_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.115932 tensorneko_util-0.3.1/src/tensorneko_util/io/toml/
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/toml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      358 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/toml/toml_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)      551 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/toml/toml_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.115932 tensorneko_util-0.3.1/src/tensorneko_util/io/video/
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/video/video_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     9333 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/video/video_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)     6013 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/video/video_writer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2193 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.119932 tensorneko_util-0.3.1/src/tensorneko_util/io/yaml/
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      897 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/yaml/yaml_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)      550 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/yaml/yaml_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.119932 tensorneko_util-0.3.1/src/tensorneko_util/notebook/
--rw-r--r--   0 runner    (1001) docker     (122)      154 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      950 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/notebook/display.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.119932 tensorneko_util-0.3.1/src/tensorneko_util/preprocess/
--rw-r--r--   0 runner    (1001) docker     (122)      508 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2434 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/preprocess/crop.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.123932 tensorneko_util-0.3.1/src/tensorneko_util/preprocess/face_detector/
--rw-r--r--   0 runner    (1001) docker     (122)      339 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/preprocess/face_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2662 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/preprocess/face_detector/_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1426 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/preprocess/face_detector/abstract_face_detector.py
--rw-r--r--   0 runner    (1001) docker     (122)     1605 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/preprocess/face_detector/anime_face_detector.py
--rw-r--r--   0 runner    (1001) docker     (122)     3861 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/preprocess/face_detector/facexzoo_face_detector.py
--rw-r--r--   0 runner    (1001) docker     (122)     4396 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/preprocess/face_detector/opencv_face_detector.py
--rw-r--r--   0 runner    (1001) docker     (122)     5979 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/preprocess/ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (122)     2587 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/preprocess/image.py
--rw-r--r--   0 runner    (1001) docker     (122)     2045 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/preprocess/video.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.127932 tensorneko_util-0.3.1/src/tensorneko_util/util/
--rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/average_meter.py
--rw-r--r--   0 runner    (1001) docker     (122)     2787 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/bimap.py
--rw-r--r--   0 runner    (1001) docker     (122)     1446 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/dispatched_misc.py
--rw-r--r--   0 runner    (1001) docker     (122)     8307 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     1891 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.127932 tensorneko_util-0.3.1/src/tensorneko_util/util/eventbus/
--rw-r--r--   0 runner    (1001) docker     (122)      305 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/eventbus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8674 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/eventbus/bus.py
--rw-r--r--   0 runner    (1001) docker     (122)      336 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/eventbus/decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)      607 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/eventbus/event.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.127932 tensorneko_util-0.3.1/src/tensorneko_util/util/fp/
--rw-r--r--   0 runner    (1001) docker     (122)      398 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/fp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2384 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/fp/args.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.131932 tensorneko_util-0.3.1/src/tensorneko_util/util/fp/array/
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/fp/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/fp/array/abstract_seq.py
--rw-r--r--   0 runner    (1001) docker     (122)     4267 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/fp/array/seq.py
--rw-r--r--   0 runner    (1001) docker     (122)     9434 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/fp/array/stream.py
--rw-r--r--   0 runner    (1001) docker     (122)     2895 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/fp/func.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.131932 tensorneko_util-0.3.1/src/tensorneko_util/util/fp/monad/
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/fp/monad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3719 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/fp/monad/eval.py
--rw-r--r--   0 runner    (1001) docker     (122)      505 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/fp/monad/monad.py
--rw-r--r--   0 runner    (1001) docker     (122)     8379 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/fp/monad/option.py
--rw-r--r--   0 runner    (1001) docker     (122)     7123 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/fp/underscore.py
--rw-r--r--   0 runner    (1001) docker     (122)     5483 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/misc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1604 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/ref.py
--rw-r--r--   0 runner    (1001) docker     (122)     3222 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/server.py
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/singleton.py
--rw-r--r--   0 runner    (1001) docker     (122)     1675 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/timer.py
--rw-r--r--   0 runner    (1001) docker     (122)      558 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/type.py
--rw-r--r--   0 runner    (1001) docker     (122)     9444 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/window_merger.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-28 09:05:52.000000 tensorneko_util-0.3.1/src/tensorneko_util/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.131932 tensorneko_util-0.3.1/src/tensorneko_util/visualization/
--rw-r--r--   0 runner    (1001) docker     (122)      514 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      450 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/visualization/color.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.135932 tensorneko_util-0.3.1/src/tensorneko_util/visualization/image_browser/
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/visualization/image_browser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/visualization/image_browser/server.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.135932 tensorneko_util-0.3.1/src/tensorneko_util/visualization/image_browser/web/
--rw-r--r--   0 runner    (1001) docker     (122)     2015 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/visualization/image_browser/web/index.html
--rw-r--r--   0 runner    (1001) docker     (122)      422 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/visualization/matplotlib.py
--rw-r--r--   0 runner    (1001) docker     (122)     3189 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/visualization/multi_plots.py
--rw-r--r--   0 runner    (1001) docker     (122)      296 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/visualization/seaborn.py
--rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/visualization/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.135932 tensorneko_util-0.3.1/src/tensorneko_util/visualization/watcher/
--rw-r--r--   0 runner    (1001) docker     (122)      268 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/visualization/watcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8398 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/visualization/watcher/component.py
--rw-r--r--   0 runner    (1001) docker     (122)     5035 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/visualization/watcher/server.py
--rw-r--r--   0 runner    (1001) docker     (122)     3859 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/visualization/watcher/view.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.099932 tensorneko_util-0.3.1/src/tensorneko_util/visualization/watcher/web/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.135932 tensorneko_util-0.3.1/src/tensorneko_util/visualization/watcher/web/dist/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.135932 tensorneko_util-0.3.1/src/tensorneko_util/visualization/watcher/web/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (122)   246413 2023-07-28 09:03:33.000000 tensorneko_util-0.3.1/src/tensorneko_util/visualization/watcher/web/dist/assets/index.a66e147e.css
--rw-r--r--   0 runner    (1001) docker     (122)   979304 2023-07-28 09:03:33.000000 tensorneko_util-0.3.1/src/tensorneko_util/visualization/watcher/web/dist/assets/index.dd94979e.js
--rw-r--r--   0 runner    (1001) docker     (122)      588 2023-07-28 09:03:33.000000 tensorneko_util-0.3.1/src/tensorneko_util/visualization/watcher/web/dist/index.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.103932 tensorneko_util-0.3.1/src/tensorneko_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-07-28 09:05:53.000000 tensorneko_util-0.3.1/src/tensorneko_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4971 2023-07-28 09:05:53.000000 tensorneko_util-0.3.1/src/tensorneko_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-28 09:05:53.000000 tensorneko_util-0.3.1/src/tensorneko_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-28 09:05:53.000000 tensorneko_util-0.3.1/src/tensorneko_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-07-28 09:05:53.000000 tensorneko_util-0.3.1/src/tensorneko_util.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.139932 tensorneko_util-0.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/test/test_library_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/test/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:48.213666 tensorneko_util-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-08-02 12:19:48.213666 tensorneko_util-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    17201 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-02 12:19:48.213666 tensorneko_util-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1906 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/setup_util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:48.157660 tensorneko_util-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:48.161660 tensorneko_util-0.3.2/src/tensorneko_util/
+-rw-r--r--   0 runner    (1001) docker     (122)      401 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:48.165661 tensorneko_util-0.3.2/src/tensorneko_util/backend/
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/backend/_tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      633 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/backend/audio_lib.py
+-rw-r--r--   0 runner    (1001) docker     (122)      592 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/backend/blocking.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4251 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/backend/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3172 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/backend/visual_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:48.165661 tensorneko_util-0.3.2/src/tensorneko_util/debug/
+-rw-r--r--   0 runner    (1001) docker     (122)      118 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/debug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1010 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/debug/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:48.169661 tensorneko_util-0.3.2/src/tensorneko_util/io/
+-rw-r--r--   0 runner    (1001) docker     (122)      291 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      871 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/_default_backends.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:48.169661 tensorneko_util-0.3.2/src/tensorneko_util/io/audio/
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      463 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/audio/audio_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2666 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/audio/audio_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2541 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/audio/audio_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:48.169661 tensorneko_util-0.3.2/src/tensorneko_util/io/hdf5/
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/hdf5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      378 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/hdf5/hdf5_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      262 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/hdf5/hdf5_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:48.173662 tensorneko_util-0.3.2/src/tensorneko_util/io/image/
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2726 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/image/image_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6628 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/image/image_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:48.173662 tensorneko_util-0.3.2/src/tensorneko_util/io/json/
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2423 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/json/json_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2196 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/json/json_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2213 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/json/json_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:48.173662 tensorneko_util-0.3.2/src/tensorneko_util/io/matlab/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/matlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      437 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/matlab/mat_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/matlab/mat_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:48.177662 tensorneko_util-0.3.2/src/tensorneko_util/io/pickle/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/pickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      429 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/pickle/pickle_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      508 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/pickle/pickle_writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2192 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:48.181662 tensorneko_util-0.3.2/src/tensorneko_util/io/text/
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      668 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/text/text_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      698 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/text/text_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:48.181662 tensorneko_util-0.3.2/src/tensorneko_util/io/toml/
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/toml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      358 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/toml/toml_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      551 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/toml/toml_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:48.181662 tensorneko_util-0.3.2/src/tensorneko_util/io/video/
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/video/video_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9333 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/video/video_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6013 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/video/video_writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2193 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:48.185663 tensorneko_util-0.3.2/src/tensorneko_util/io/yaml/
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      897 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/yaml/yaml_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      550 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/io/yaml/yaml_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:48.185663 tensorneko_util-0.3.2/src/tensorneko_util/notebook/
+-rw-r--r--   0 runner    (1001) docker     (122)      154 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      950 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/notebook/display.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:48.185663 tensorneko_util-0.3.2/src/tensorneko_util/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (122)      508 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2434 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/preprocess/crop.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:48.189663 tensorneko_util-0.3.2/src/tensorneko_util/preprocess/face_detector/
+-rw-r--r--   0 runner    (1001) docker     (122)      339 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/preprocess/face_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2662 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/preprocess/face_detector/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1426 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/preprocess/face_detector/abstract_face_detector.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1605 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/preprocess/face_detector/anime_face_detector.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3861 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/preprocess/face_detector/facexzoo_face_detector.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4396 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/preprocess/face_detector/opencv_face_detector.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5979 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/preprocess/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2587 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/preprocess/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2045 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/preprocess/video.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:48.193664 tensorneko_util-0.3.2/src/tensorneko_util/util/
+-rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/util/average_meter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2787 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/util/bimap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1446 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/util/dispatched_misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8307 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/util/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1891 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/util/downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:48.193664 tensorneko_util-0.3.2/src/tensorneko_util/util/eventbus/
+-rw-r--r--   0 runner    (1001) docker     (122)      305 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/util/eventbus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8674 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/util/eventbus/bus.py
+-rw-r--r--   0 runner    (1001) docker     (122)      336 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/util/eventbus/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      607 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/util/eventbus/event.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:48.197664 tensorneko_util-0.3.2/src/tensorneko_util/util/fp/
+-rw-r--r--   0 runner    (1001) docker     (122)      398 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/util/fp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2384 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/util/fp/args.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:48.197664 tensorneko_util-0.3.2/src/tensorneko_util/util/fp/array/
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/util/fp/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/util/fp/array/abstract_seq.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4267 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/util/fp/array/seq.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9434 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/util/fp/array/stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2895 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/util/fp/func.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:48.201665 tensorneko_util-0.3.2/src/tensorneko_util/util/fp/monad/
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/util/fp/monad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3719 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/util/fp/monad/eval.py
+-rw-r--r--   0 runner    (1001) docker     (122)      505 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/util/fp/monad/monad.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8379 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/util/fp/monad/option.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7123 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/util/fp/underscore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5483 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/util/misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1604 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/util/ref.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3222 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/util/server.py
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/util/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1675 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/util/timer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      558 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/util/type.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9444 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/util/window_merger.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-08-02 12:19:47.000000 tensorneko_util-0.3.2/src/tensorneko_util/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:48.201665 tensorneko_util-0.3.2/src/tensorneko_util/visualization/
+-rw-r--r--   0 runner    (1001) docker     (122)      514 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      450 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/visualization/color.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:48.201665 tensorneko_util-0.3.2/src/tensorneko_util/visualization/image_browser/
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/visualization/image_browser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/visualization/image_browser/server.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:48.201665 tensorneko_util-0.3.2/src/tensorneko_util/visualization/image_browser/web/
+-rw-r--r--   0 runner    (1001) docker     (122)     2015 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/visualization/image_browser/web/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/visualization/matplotlib.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3189 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/visualization/multi_plots.py
+-rw-r--r--   0 runner    (1001) docker     (122)      296 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/visualization/seaborn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/visualization/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:48.205665 tensorneko_util-0.3.2/src/tensorneko_util/visualization/watcher/
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/visualization/watcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8398 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/visualization/watcher/component.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5035 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/visualization/watcher/server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3859 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/src/tensorneko_util/visualization/watcher/view.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:48.161660 tensorneko_util-0.3.2/src/tensorneko_util/visualization/watcher/web/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:48.205665 tensorneko_util-0.3.2/src/tensorneko_util/visualization/watcher/web/dist/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:48.205665 tensorneko_util-0.3.2/src/tensorneko_util/visualization/watcher/web/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (122)   246413 2023-08-02 12:17:13.000000 tensorneko_util-0.3.2/src/tensorneko_util/visualization/watcher/web/dist/assets/index.a66e147e.css
+-rw-r--r--   0 runner    (1001) docker     (122)   979304 2023-08-02 12:17:13.000000 tensorneko_util-0.3.2/src/tensorneko_util/visualization/watcher/web/dist/assets/index.dd94979e.js
+-rw-r--r--   0 runner    (1001) docker     (122)      588 2023-08-02 12:17:13.000000 tensorneko_util-0.3.2/src/tensorneko_util/visualization/watcher/web/dist/index.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:48.165661 tensorneko_util-0.3.2/src/tensorneko_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-08-02 12:19:48.000000 tensorneko_util-0.3.2/src/tensorneko_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4971 2023-08-02 12:19:48.000000 tensorneko_util-0.3.2/src/tensorneko_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 12:19:48.000000 tensorneko_util-0.3.2/src/tensorneko_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-08-02 12:19:48.000000 tensorneko_util-0.3.2/src/tensorneko_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-08-02 12:19:48.000000 tensorneko_util-0.3.2/src/tensorneko_util.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 12:19:48.213666 tensorneko_util-0.3.2/test/
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/test/test_library_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-08-02 12:16:45.000000 tensorneko_util-0.3.2/test/test_version.py
```

### Comparing `tensorneko_util-0.3.1/LICENSE` & `tensorneko_util-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/PKG-INFO` & `tensorneko_util-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorneko_util
-Version: 0.3.1
+Version: 0.3.2
 Summary: The Utils for Library TensorNeko.
 Home-page: https://github.com/ControlNet/tensorneko
 Author: ControlNet
 Author-email: smczx@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ControlNet/tensorneko/issues
 Project-URL: Source Code, https://github.com/ControlNet/tensorneko
```

### Comparing `tensorneko_util-0.3.1/README.md` & `tensorneko_util-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/setup.py` & `tensorneko_util-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/setup_util.py` & `tensorneko_util-0.3.2/setup_util.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/backend/_tqdm.py` & `tensorneko_util-0.3.2/src/tensorneko_util/backend/_tqdm.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/backend/blocking.py` & `tensorneko_util-0.3.2/src/tensorneko_util/backend/blocking.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/backend/parallel.py` & `tensorneko_util-0.3.2/src/tensorneko_util/backend/parallel.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/backend/visual_lib.py` & `tensorneko_util-0.3.2/src/tensorneko_util/backend/visual_lib.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,15 +52,23 @@
         return _VisualLibAvailability.is_pil_available
 
     @staticmethod
     def ffmpeg_available() -> bool:
         if _VisualLibAvailability.is_ffmpeg_available is None:
             ffmpeg_available = subprocess.run('ffmpeg -version', stdout=subprocess.DEVNULL,
                 stderr=subprocess.DEVNULL, shell=True).returncode == 0
-            _VisualLibAvailability.is_ffmpeg_available = ffmpeg_available
+            if ffmpeg_available:
+                try:
+                    import ffmpeg
+                    _VisualLibAvailability.is_ffmpeg_available = True
+                except ImportError:
+                    _VisualLibAvailability.is_ffmpeg_available = False
+            else:
+                _VisualLibAvailability.is_ffmpeg_available = False
+
         return _VisualLibAvailability.is_ffmpeg_available
 
     @staticmethod
     def skimage_available() -> bool:
         if _VisualLibAvailability.is_skimage_available is None:
             try:
                 import skimage
```

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/debug/parser.py` & `tensorneko_util-0.3.2/src/tensorneko_util/debug/parser.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/io/_default_backends.py` & `tensorneko_util-0.3.2/src/tensorneko_util/io/_default_backends.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/io/audio/audio_reader.py` & `tensorneko_util-0.3.2/src/tensorneko_util/io/audio/audio_writer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,58 @@
-from typing import Optional
+from typing import Union
 
 from .audio_data import AudioData
 from .._default_backends import _default_audio_io_backend
 from ...backend.audio_lib import AudioLib
+from ...util import dispatch
+from ...util.type import T_ARRAY
 
 
-class AudioReader:
-    """AudioReader for reading audio file"""
+class AudioWriter:
+    """AudioWriter for writing audio file"""
 
-    @staticmethod
-    def of(path: str, channel_first: bool = True, backend: Optional[AudioLib] = None) -> AudioData:
+    @classmethod
+    @dispatch
+    def to(cls, path: str, audio: AudioData, channel_first: bool = True, backend: AudioLib = None) -> None:
         """
-        Read audio tensor from given file.
+        Save wav file from :class:`~tensorneko.io.audio.audio_data.AudioData`.
 
         Args:
-            path (``str``): Path to the audio file.
-            channel_first (``bool``, optional): Whether the audio is channel first. The output shape is (C, T) if true
+            path (``str``): The path of output file.
+            audio (:class:`~tensorneko.io.audio.AudioData`): The AudioData object for output.
+            channel_first (``bool``, optional): Whether the audio is channel first. The input shape is (C, T) if true
                 and (T, C) if false. Default: True.
             backend (:class:`~tensorneko.io.audio.audio_lib.AudioLib`, optional): The audio library to use.
                 Default: pytorch.
+        """
+        return cls.to(path, audio.audio, audio.sample_rate, channel_first, backend)
+
+    @classmethod
+    @dispatch
+    def to(cls, path: str, audio: T_ARRAY, sample_rate: int = 16000, channel_first: bool = True,
+        backend: AudioLib = None
+    ):
+        """
+        Save wav file from :class:`~torch.Tensor` or :class:`~numpy.ndarray` with (C, T).
 
-        Returns:
-            :class:`~.audio_data.AudioData`: The Audio data in the file.
+        Args:
+            path (``str``): The path of output file.
+            audio (:class:`~torch.Tensor` | :class:`~numpy.ndarray`): The tensor or array of audio.
+            sample_rate (``int``, optional): The sample rate of the audio. Default: 16000.
+            channel_first (``bool``, optional): Whether the audio is channel first. The input shape is (C, T) if true
+                and (T, C) if false. Default: True.
+            backend (:class:`~tensorneko.io.audio.audio_lib.AudioLib`, optional): The audio library to use.
+                Default: pytorch.
         """
         backend = backend or _default_audio_io_backend()
 
         if backend == AudioLib.PYTORCH:
             if not AudioLib.pytorch_available():
                 raise ValueError("Torchaudio is not available.")
             import torchaudio
-            return AudioData(*torchaudio.load(path, channels_first=channel_first))
+            torchaudio.save(path, audio, sample_rate, channels_first=channel_first)
         else:
             raise ValueError("Unknown audio library: {}".format(backend))
 
-    def __new__(cls, path: str, channel_first: bool = True, backend: Optional[AudioLib] = None) -> AudioData:
-        """Alias of :meth:`~AudioReader.of`"""
-        return cls.of(path, channel_first, backend)
+    def __new__(cls, path: str, audio: Union[AudioData, T_ARRAY], *args, **kwargs):
+        """Alias to :meth:`~AudioWriter.to`"""
+        return cls.to(path, audio, *args, **kwargs)
```

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/io/audio/audio_writer.py` & `tensorneko_util-0.3.2/src/tensorneko_util/io/audio/audio_reader.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,58 +1,67 @@
-from typing import Union
+from typing import Optional
+
+import numpy as np
 
 from .audio_data import AudioData
 from .._default_backends import _default_audio_io_backend
 from ...backend.audio_lib import AudioLib
-from ...util import dispatch
-from ...util.type import T_ARRAY
 
 
-class AudioWriter:
-    """AudioWriter for writing audio file"""
+class AudioReader:
+    """AudioReader for reading audio file"""
 
-    @classmethod
-    @dispatch
-    def to(cls, path: str, audio: AudioData, channel_first: bool = True, backend: AudioLib = None) -> None:
+    @staticmethod
+    def of(path: str, channel_first: bool = True, backend: Optional[AudioLib] = None) -> AudioData:
         """
-        Save wav file from :class:`~tensorneko.io.audio.audio_data.AudioData`.
+        Read audio tensor from given file.
 
         Args:
-            path (``str``): The path of output file.
-            audio (:class:`~tensorneko.io.audio.AudioData`): The AudioData object for output.
-            channel_first (``bool``, optional): Whether the audio is channel first. The input shape is (C, T) if true
+            path (``str``): Path to the audio file.
+            channel_first (``bool``, optional): Whether the audio is channel first. The output shape is (C, T) if true
                 and (T, C) if false. Default: True.
             backend (:class:`~tensorneko.io.audio.audio_lib.AudioLib`, optional): The audio library to use.
                 Default: pytorch.
-        """
-        return cls.to(path, audio.audio, audio.sample_rate, channel_first, backend)
 
-    @classmethod
-    @dispatch
-    def to(cls, path: str, audio: T_ARRAY, sample_rate: int = 16000, channel_first: bool = True,
-        backend: AudioLib = None
-    ):
-        """
-        Save wav file from :class:`~torch.Tensor` or :class:`~numpy.ndarray` with (C, T).
-
-        Args:
-            path (``str``): The path of output file.
-            audio (:class:`~torch.Tensor` | :class:`~numpy.ndarray`): The tensor or array of audio.
-            sample_rate (``int``, optional): The sample rate of the audio. Default: 16000.
-            channel_first (``bool``, optional): Whether the audio is channel first. The input shape is (C, T) if true
-                and (T, C) if false. Default: True.
-            backend (:class:`~tensorneko.io.audio.audio_lib.AudioLib`, optional): The audio library to use.
-                Default: pytorch.
+        Returns:
+            :class:`~.audio_data.AudioData`: The Audio data in the file.
         """
         backend = backend or _default_audio_io_backend()
 
         if backend == AudioLib.PYTORCH:
             if not AudioLib.pytorch_available():
                 raise ValueError("Torchaudio is not available.")
             import torchaudio
-            torchaudio.save(path, audio, sample_rate, channels_first=channel_first)
+            return AudioData(*torchaudio.load(path, channels_first=channel_first))
+        elif backend == AudioLib.FFMPEG:
+            if not AudioLib.ffmpeg_available():
+                raise ValueError("FFmpeg is not available.")
+            import ffmpeg
+
+            for stream in ffmpeg.probe(path)["streams"]:
+                if stream["codec_type"] == "audio":
+                    sample_rate = int(stream["sample_rate"])
+                    channel = int(stream["channels"])
+                    break
+            else:
+                raise RuntimeError("No audio stream found.")
+
+            try:
+                out, _ = (
+                    ffmpeg.input(path, threads=0)
+                    .output("-", format="s16le", acodec="pcm_s16le")
+                    .run(cmd=["ffmpeg", "-nostdin"], capture_stdout=True, capture_stderr=True)
+                )
+            except ffmpeg.Error as e:
+                raise RuntimeError(f"Failed to load audio: {e.stderr.decode()}") from e
+
+            arr = np.frombuffer(out, np.int16).flatten().astype(np.float32) / 32768.0
+            arr = arr.reshape(-1, channel)
+            arr = arr.T if channel_first else arr
+
+            return AudioData(arr, sample_rate)
         else:
             raise ValueError("Unknown audio library: {}".format(backend))
 
-    def __new__(cls, path: str, audio: Union[AudioData, T_ARRAY], *args, **kwargs):
-        """Alias to :meth:`~AudioWriter.to`"""
-        return cls.to(path, audio, *args, **kwargs)
+    def __new__(cls, path: str, channel_first: bool = True, backend: Optional[AudioLib] = None) -> AudioData:
+        """Alias of :meth:`~AudioReader.of`"""
+        return cls.of(path, channel_first, backend)
```

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/io/image/image_reader.py` & `tensorneko_util-0.3.2/src/tensorneko_util/io/image/image_reader.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/io/image/image_writer.py` & `tensorneko_util-0.3.2/src/tensorneko_util/io/image/image_writer.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/io/json/json_data.py` & `tensorneko_util-0.3.2/src/tensorneko_util/io/json/json_data.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/io/json/json_reader.py` & `tensorneko_util-0.3.2/src/tensorneko_util/io/json/json_reader.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/io/json/json_writer.py` & `tensorneko_util-0.3.2/src/tensorneko_util/io/json/json_writer.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/io/matlab/mat_writer.py` & `tensorneko_util-0.3.2/src/tensorneko_util/io/matlab/mat_writer.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/io/reader.py` & `tensorneko_util-0.3.2/src/tensorneko_util/io/reader.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/io/text/text_reader.py` & `tensorneko_util-0.3.2/src/tensorneko_util/io/text/text_reader.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/io/text/text_writer.py` & `tensorneko_util-0.3.2/src/tensorneko_util/io/text/text_writer.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/io/toml/toml_writer.py` & `tensorneko_util-0.3.2/src/tensorneko_util/io/toml/toml_writer.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/io/video/video_data.py` & `tensorneko_util-0.3.2/src/tensorneko_util/io/video/video_data.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/io/video/video_reader.py` & `tensorneko_util-0.3.2/src/tensorneko_util/io/video/video_reader.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/io/video/video_writer.py` & `tensorneko_util-0.3.2/src/tensorneko_util/io/video/video_writer.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/io/writer.py` & `tensorneko_util-0.3.2/src/tensorneko_util/io/writer.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/io/yaml/yaml_reader.py` & `tensorneko_util-0.3.2/src/tensorneko_util/io/yaml/yaml_reader.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/io/yaml/yaml_writer.py` & `tensorneko_util-0.3.2/src/tensorneko_util/io/yaml/yaml_writer.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/notebook/display.py` & `tensorneko_util-0.3.2/src/tensorneko_util/notebook/display.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/preprocess/crop.py` & `tensorneko_util-0.3.2/src/tensorneko_util/preprocess/crop.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/preprocess/face_detector/_utils.py` & `tensorneko_util-0.3.2/src/tensorneko_util/preprocess/face_detector/_utils.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/preprocess/face_detector/abstract_face_detector.py` & `tensorneko_util-0.3.2/src/tensorneko_util/preprocess/face_detector/abstract_face_detector.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/preprocess/face_detector/anime_face_detector.py` & `tensorneko_util-0.3.2/src/tensorneko_util/preprocess/face_detector/anime_face_detector.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/preprocess/face_detector/facexzoo_face_detector.py` & `tensorneko_util-0.3.2/src/tensorneko_util/preprocess/face_detector/facexzoo_face_detector.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/preprocess/face_detector/opencv_face_detector.py` & `tensorneko_util-0.3.2/src/tensorneko_util/preprocess/face_detector/opencv_face_detector.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/preprocess/ffmpeg.py` & `tensorneko_util-0.3.2/src/tensorneko_util/preprocess/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/preprocess/image.py` & `tensorneko_util-0.3.2/src/tensorneko_util/preprocess/image.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/preprocess/video.py` & `tensorneko_util-0.3.2/src/tensorneko_util/preprocess/video.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/util/__init__.py` & `tensorneko_util-0.3.2/src/tensorneko_util/util/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/util/average_meter.py` & `tensorneko_util-0.3.2/src/tensorneko_util/util/average_meter.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/util/bimap.py` & `tensorneko_util-0.3.2/src/tensorneko_util/util/bimap.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/util/dispatched_misc.py` & `tensorneko_util-0.3.2/src/tensorneko_util/util/dispatched_misc.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/util/dispatcher.py` & `tensorneko_util-0.3.2/src/tensorneko_util/util/dispatcher.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/util/downloader.py` & `tensorneko_util-0.3.2/src/tensorneko_util/util/downloader.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/util/eventbus/bus.py` & `tensorneko_util-0.3.2/src/tensorneko_util/util/eventbus/bus.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/util/eventbus/event.py` & `tensorneko_util-0.3.2/src/tensorneko_util/util/eventbus/event.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/util/fp/args.py` & `tensorneko_util-0.3.2/src/tensorneko_util/util/fp/args.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/util/fp/array/abstract_seq.py` & `tensorneko_util-0.3.2/src/tensorneko_util/util/fp/array/abstract_seq.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/util/fp/array/seq.py` & `tensorneko_util-0.3.2/src/tensorneko_util/util/fp/array/seq.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/util/fp/array/stream.py` & `tensorneko_util-0.3.2/src/tensorneko_util/util/fp/array/stream.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/util/fp/func.py` & `tensorneko_util-0.3.2/src/tensorneko_util/util/fp/func.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/util/fp/monad/eval.py` & `tensorneko_util-0.3.2/src/tensorneko_util/util/fp/monad/eval.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/util/fp/monad/option.py` & `tensorneko_util-0.3.2/src/tensorneko_util/util/fp/monad/option.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/util/fp/underscore.py` & `tensorneko_util-0.3.2/src/tensorneko_util/util/fp/underscore.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/util/misc.py` & `tensorneko_util-0.3.2/src/tensorneko_util/util/misc.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/util/ref.py` & `tensorneko_util-0.3.2/src/tensorneko_util/util/ref.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/util/server.py` & `tensorneko_util-0.3.2/src/tensorneko_util/util/server.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/util/singleton.py` & `tensorneko_util-0.3.2/src/tensorneko_util/util/singleton.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/util/timer.py` & `tensorneko_util-0.3.2/src/tensorneko_util/util/timer.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/util/type.py` & `tensorneko_util-0.3.2/src/tensorneko_util/util/type.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/util/window_merger.py` & `tensorneko_util-0.3.2/src/tensorneko_util/util/window_merger.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/visualization/__init__.py` & `tensorneko_util-0.3.2/src/tensorneko_util/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/visualization/image_browser/server.py` & `tensorneko_util-0.3.2/src/tensorneko_util/visualization/image_browser/server.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/visualization/image_browser/web/index.html` & `tensorneko_util-0.3.2/src/tensorneko_util/visualization/image_browser/web/index.html`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/visualization/multi_plots.py` & `tensorneko_util-0.3.2/src/tensorneko_util/visualization/multi_plots.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/visualization/tensorboard.py` & `tensorneko_util-0.3.2/src/tensorneko_util/visualization/tensorboard.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/visualization/watcher/component.py` & `tensorneko_util-0.3.2/src/tensorneko_util/visualization/watcher/component.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/visualization/watcher/server.py` & `tensorneko_util-0.3.2/src/tensorneko_util/visualization/watcher/server.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/visualization/watcher/view.py` & `tensorneko_util-0.3.2/src/tensorneko_util/visualization/watcher/view.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/visualization/watcher/web/dist/assets/index.a66e147e.css` & `tensorneko_util-0.3.2/src/tensorneko_util/visualization/watcher/web/dist/assets/index.a66e147e.css`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/visualization/watcher/web/dist/assets/index.dd94979e.js` & `tensorneko_util-0.3.2/src/tensorneko_util/visualization/watcher/web/dist/assets/index.dd94979e.js`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util/visualization/watcher/web/dist/index.html` & `tensorneko_util-0.3.2/src/tensorneko_util/visualization/watcher/web/dist/index.html`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util.egg-info/PKG-INFO` & `tensorneko_util-0.3.2/src/tensorneko_util.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorneko-util
-Version: 0.3.1
+Version: 0.3.2
 Summary: The Utils for Library TensorNeko.
 Home-page: https://github.com/ControlNet/tensorneko
 Author: ControlNet
 Author-email: smczx@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ControlNet/tensorneko/issues
 Project-URL: Source Code, https://github.com/ControlNet/tensorneko
```

### Comparing `tensorneko_util-0.3.1/src/tensorneko_util.egg-info/SOURCES.txt` & `tensorneko_util-0.3.2/src/tensorneko_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.1/test/test_version.py` & `tensorneko_util-0.3.2/test/test_version.py`

 * *Files identical despite different names*

