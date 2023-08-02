# Comparing `tmp/MeUtils-2023.7.7.15.3.6.tar.gz` & `tmp/MeUtils-2023.8.2.13.20.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MeUtils-2023.7.7.15.3.6.tar", last modified: Fri Jul  7 07:03:06 2023, max compression
+gzip compressed data, was "MeUtils-2023.8.2.13.20.11.tar", last modified: Wed Aug  2 05:20:12 2023, max compression
```

## Comparing `MeUtils-2023.7.7.15.3.6.tar` & `MeUtils-2023.8.2.13.20.11.tar`

### file list

```diff
@@ -1,553 +1,576 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.948479 MeUtils-2023.7.7.15.3.6/
--rw-r--r--   0 betterme   (501) staff       (20)     1204 2023-05-22 06:35:12.000000 MeUtils-2023.7.7.15.3.6/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)    11357 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      249 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/MANIFEST.in
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.836333 MeUtils-2023.7.7.15.3.6/MeUtils.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     1892 2023-07-07 07:03:06.000000 MeUtils-2023.7.7.15.3.6/MeUtils.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)    18628 2023-07-07 07:03:06.000000 MeUtils-2023.7.7.15.3.6/MeUtils.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-07-07 07:03:06.000000 MeUtils-2023.7.7.15.3.6/MeUtils.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)      193 2023-07-07 07:03:06.000000 MeUtils-2023.7.7.15.3.6/MeUtils.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1039 2023-07-07 07:03:06.000000 MeUtils-2023.7.7.15.3.6/MeUtils.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)       17 2023-07-07 07:03:06.000000 MeUtils-2023.7.7.15.3.6/MeUtils.egg-info/top_level.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1892 2023-07-07 07:03:06.948305 MeUtils-2023.7.7.15.3.6/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1067 2023-05-04 03:00:27.000000 MeUtils-2023.7.7.15.3.6/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      105 2023-06-12 01:19:08.000000 MeUtils-2023.7.7.15.3.6/TODO.md
--rw-r--r--   0 betterme   (501) staff       (20)      684 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/clear_git_history.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      289 2023-05-26 11:03:24.000000 MeUtils-2023.7.7.15.3.6/git_init.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.841564 MeUtils-2023.7.7.15.3.6/meutils/
--rw-r--r--   0 betterme   (501) staff       (20)      348 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1850 2023-04-11 05:47:45.000000 MeUtils-2023.7.7.15.3.6/meutils/_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.841988 MeUtils-2023.7.7.15.3.6/meutils/ai_audio/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-17 05:51:24.000000 MeUtils-2023.7.7.15.3.6/meutils/ai_audio/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      637 2023-05-17 05:56:24.000000 MeUtils-2023.7.7.15.3.6/meutils/ai_audio/asr.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.842473 MeUtils-2023.7.7.15.3.6/meutils/ai_cv/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-18 08:11:56.000000 MeUtils-2023.7.7.15.3.6/meutils/ai_cv/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      263 2023-05-18 08:11:56.000000 MeUtils-2023.7.7.15.3.6/meutils/ai_cv/ocr.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.845000 MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/
--rw-r--r--   0 betterme   (501) staff       (20)     6927 2023-06-30 13:22:13.000000 MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/SplitSentence.py
--rw-r--r--   0 betterme   (501) staff       (20)    13489 2023-05-21 05:19:20.000000 MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/Untitled-1(1).py
--rw-r--r--   0 betterme   (501) staff       (20)      244 2023-04-25 06:23:09.000000 MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2295 2023-04-10 08:57:58.000000 MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/_lda.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.845689 MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/_textsplitter/
--rw-r--r--   0 betterme   (501) staff       (20)      287 2023-05-22 01:52:50.000000 MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/_textsplitter/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     6673 2023-05-21 05:10:54.000000 MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/_textsplitter/chinese_text_splitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     2282 2023-05-21 05:27:40.000000 MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/_textsplitter/text_split.py
--rw-r--r--   0 betterme   (501) staff       (20)     1111 2023-06-06 06:44:28.000000 MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/lda.py
--rw-r--r--   0 betterme   (501) staff       (20)     2560 2023-06-05 05:29:27.000000 MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/ner.py
--rw-r--r--   0 betterme   (501) staff       (20)      963 2023-07-04 08:24:23.000000 MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/sentence_transformers.py
--rw-r--r--   0 betterme   (501) staff       (20)     2111 2023-06-30 13:18:15.000000 MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/textsplitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     3542 2023-06-05 05:29:27.000000 MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/word_segmentation.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.848251 MeUtils-2023.7.7.15.3.6/meutils/ann/
--rw-r--r--   0 betterme   (501) staff       (20)      781 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/ann/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     1389 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/ann/README_gensim.md
--rw-r--r--   0 betterme   (501) staff       (20)      240 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/ann/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     9161 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/ann/ann.py
--rw-r--r--   0 betterme   (501) staff       (20)     5662 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/ann/ann_faiss.py
--rw-r--r--   0 betterme   (501) staff       (20)      965 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/ann/ann_gensim.py
--rw-r--r--   0 betterme   (501) staff       (20)     1002 2023-05-16 06:47:06.000000 MeUtils-2023.7.7.15.3.6/meutils/ann/ann_inmemory.py
--rw-r--r--   0 betterme   (501) staff       (20)      458 2023-05-19 06:06:57.000000 MeUtils-2023.7.7.15.3.6/meutils/ann/ann_qdrant.py
--rw-r--r--   0 betterme   (501) staff       (20)     1171 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/ann/ann_service.py
--rw-r--r--   0 betterme   (501) staff       (20)     4743 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/ann/ann_v1.py
--rw-r--r--   0 betterme   (501) staff       (20)     1927 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/ann/cli.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.848634 MeUtils-2023.7.7.15.3.6/meutils/ann/examples/
--rw-r--r--   0 betterme   (501) staff       (20)     1476 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/ann/examples/client.py
--rw-r--r--   0 betterme   (501) staff       (20)      463 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/ann/examples/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      238 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/ann/milvus.py
--rw-r--r--   0 betterme   (501) staff       (20)     1076 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/ann/shake_demo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.848851 MeUtils-2023.7.7.15.3.6/meutils/asyncio_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      243 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/asyncio_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     6839 2023-07-07 07:01:54.000000 MeUtils-2023.7.7.15.3.6/meutils/cache_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.849634 MeUtils-2023.7.7.15.3.6/meutils/cachedir/
--rw-r--r--   0 betterme   (501) staff       (20)    32768 2023-07-06 12:37:19.000000 MeUtils-2023.7.7.15.3.6/meutils/cachedir/cache.db
--rw-r--r--   0 betterme   (501) staff       (20)    32768 2023-07-06 12:37:19.000000 MeUtils-2023.7.7.15.3.6/meutils/cachedir/cache.db-shm
--rw-r--r--   0 betterme   (501) staff       (20)    98912 2023-07-06 12:37:51.000000 MeUtils-2023.7.7.15.3.6/meutils/cachedir/cache.db-wal
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.851249 MeUtils-2023.7.7.15.3.6/meutils/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2828 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)      738 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/clis/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)     2234 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/clis/cron.py
--rw-r--r--   0 betterme   (501) staff       (20)      595 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/clis/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     1517 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/clis/gunicorn.conf.py
--rw-r--r--   0 betterme   (501) staff       (20)      619 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/clis/monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)     1018 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/clis/nesc.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.852109 MeUtils-2023.7.7.15.3.6/meutils/cmds/
--rw-r--r--   0 betterme   (501) staff       (20)     1185 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/cmds/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      293 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/cmds/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      458 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/cmds/cmd.py
--rw-r--r--   0 betterme   (501) staff       (20)     1734 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/cmds/hdfs_cmd.py
--rw-r--r--   0 betterme   (501) staff       (20)      629 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/cmds/subprocess_demo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.852414 MeUtils-2023.7.7.15.3.6/meutils/coding/
--rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/coding/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      942 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/coding/find132.py
--rw-r--r--   0 betterme   (501) staff       (20)    10338 2023-07-06 09:14:28.000000 MeUtils-2023.7.7.15.3.6/meutils/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.852772 MeUtils-2023.7.7.15.3.6/meutils/comp_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      361 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/comp_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1705 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/comp_utils/reverse_metric.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.861386 MeUtils-2023.7.7.15.3.6/meutils/data/
--rw-r--r--   0 betterme   (501) staff       (20) 10062565 2022-11-07 06:01:38.000000 MeUtils-2023.7.7.15.3.6/meutils/data/SimHei.ttf
--rw-r--r--   0 betterme   (501) staff       (20)       19 2023-07-07 07:03:06.000000 MeUtils-2023.7.7.15.3.6/meutils/data/VERSION
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/data/_FLAG
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/data/_SUCCESS
--rw-r--r--   0 betterme   (501) staff       (20)      243 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/data/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      600 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/data/coordinate.py
--rw-r--r--   0 betterme   (501) staff       (20)     2514 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/date_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.866395 MeUtils-2023.7.7.15.3.6/meutils/db/
--rw-r--r--   0 betterme   (501) staff       (20)     1507 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/db/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     7396 2023-06-30 01:59:42.000000 MeUtils-2023.7.7.15.3.6/meutils/db/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2337 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/db/mongo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2168 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/db/neo4j.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.870025 MeUtils-2023.7.7.15.3.6/meutils/decorators/
--rw-r--r--   0 betterme   (501) staff       (20)      238 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/decorators/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     1681 2023-05-25 09:49:50.000000 MeUtils-2023.7.7.15.3.6/meutils/decorators/__ai.py
--rw-r--r--   0 betterme   (501) staff       (20)     3284 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/decorators/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1837 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/decorators/catch.py
--rw-r--r--   0 betterme   (501) staff       (20)     7099 2023-07-03 09:51:08.000000 MeUtils-2023.7.7.15.3.6/meutils/decorators/common.py
--rw-r--r--   0 betterme   (501) staff       (20)    15570 2023-04-06 06:24:58.000000 MeUtils-2023.7.7.15.3.6/meutils/decorators/decorator.py
--rw-r--r--   0 betterme   (501) staff       (20)      754 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/decorators/decorator_demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      527 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/decorators/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2115 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/decorators/feishu.py
--rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/decorators/retry.py
--rw-r--r--   0 betterme   (501) staff       (20)     1678 2023-04-04 15:22:58.000000 MeUtils-2023.7.7.15.3.6/meutils/decorators/scheduler.py
--rw-r--r--   0 betterme   (501) staff       (20)     3640 2023-05-15 10:32:24.000000 MeUtils-2023.7.7.15.3.6/meutils/dist_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.871277 MeUtils-2023.7.7.15.3.6/meutils/docarray_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-18 06:24:19.000000 MeUtils-2023.7.7.15.3.6/meutils/docarray_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      977 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/docarray_utils/demo_es.py
--rw-r--r--   0 betterme   (501) staff       (20)     1341 2023-04-26 13:37:46.000000 MeUtils-2023.7.7.15.3.6/meutils/docarray_utils/demo_hnsw.py
--rw-r--r--   0 betterme   (501) staff       (20)      985 2023-04-27 02:39:23.000000 MeUtils-2023.7.7.15.3.6/meutils/docarray_utils/in_memory.py
--rw-r--r--   0 betterme   (501) staff       (20)     1058 2023-04-27 01:04:00.000000 MeUtils-2023.7.7.15.3.6/meutils/docarray_utils/改造下hnsw.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.871673 MeUtils-2023.7.7.15.3.6/meutils/easy_search/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/easy_search/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2217 2023-05-25 08:27:44.000000 MeUtils-2023.7.7.15.3.6/meutils/easy_search/es.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.872805 MeUtils-2023.7.7.15.3.6/meutils/fileparser/
--rw-r--r--   0 betterme   (501) staff       (20)     1975 2023-05-30 05:34:49.000000 MeUtils-2023.7.7.15.3.6/meutils/fileparser/PDF抽取.py
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-18 08:38:53.000000 MeUtils-2023.7.7.15.3.6/meutils/fileparser/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-18 08:32:11.000000 MeUtils-2023.7.7.15.3.6/meutils/fileparser/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-05-18 08:39:22.000000 MeUtils-2023.7.7.15.3.6/meutils/fileparser/common.py
--rw-r--r--   0 betterme   (501) staff       (20)      263 2023-05-18 08:39:36.000000 MeUtils-2023.7.7.15.3.6/meutils/fileparser/pdf.py
--rw-r--r--   0 betterme   (501) staff       (20)     2393 2023-04-04 15:30:40.000000 MeUtils-2023.7.7.15.3.6/meutils/hash_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)      969 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/import_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.873569 MeUtils-2023.7.7.15.3.6/meutils/init/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-04-27 08:58:17.000000 MeUtils-2023.7.7.15.3.6/meutils/init/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1303 2023-06-04 08:38:47.000000 MeUtils-2023.7.7.15.3.6/meutils/init/evn.py
--rw-r--r--   0 betterme   (501) staff       (20)    12884 2023-07-06 01:18:39.000000 MeUtils-2023.7.7.15.3.6/meutils/init/oo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.875181 MeUtils-2023.7.7.15.3.6/meutils/io/
--rw-r--r--   0 betterme   (501) staff       (20)     2107 2023-04-13 02:51:32.000000 MeUtils-2023.7.7.15.3.6/meutils/io/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      409 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/io/file.py
--rw-r--r--   0 betterme   (501) staff       (20)     2319 2023-05-30 01:57:16.000000 MeUtils-2023.7.7.15.3.6/meutils/io/image.py
--rw-r--r--   0 betterme   (501) staff       (20)     8605 2023-06-26 01:26:21.000000 MeUtils-2023.7.7.15.3.6/meutils/io/tf_io.py
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/io/x.yml
--rw-r--r--   0 betterme   (501) staff       (20)      708 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/jinja_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     2512 2023-04-02 12:55:05.000000 MeUtils-2023.7.7.15.3.6/meutils/log_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.876625 MeUtils-2023.7.7.15.3.6/meutils/notice/
--rw-r--r--   0 betterme   (501) staff       (20)      837 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/notice/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2403 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/notice/emails.py
--rw-r--r--   0 betterme   (501) staff       (20)      703 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/notice/feishu.py
--rw-r--r--   0 betterme   (501) staff       (20)      953 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/notice/file_post.py
--rw-r--r--   0 betterme   (501) staff       (20)     2511 2023-06-13 09:13:04.000000 MeUtils-2023.7.7.15.3.6/meutils/notice/wechat.py
--rw-r--r--   0 betterme   (501) staff       (20)     3215 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/notice/wechat_.py
--rw-r--r--   0 betterme   (501) staff       (20)     6983 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/notice/wecom.py
--rw-r--r--   0 betterme   (501) staff       (20)     1102 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/notice/weekmeet.py
--rw-r--r--   0 betterme   (501) staff       (20)     2962 2023-05-16 06:23:15.000000 MeUtils-2023.7.7.15.3.6/meutils/np_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.878597 MeUtils-2023.7.7.15.3.6/meutils/office_automation/
--rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/office_automation/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      508 2023-03-27 04:08:21.000000 MeUtils-2023.7.7.15.3.6/meutils/office_automation/doc.py
--rw-r--r--   0 betterme   (501) staff       (20)     1538 2023-04-28 07:14:17.000000 MeUtils-2023.7.7.15.3.6/meutils/office_automation/pdf.py
--rw-r--r--   0 betterme   (501) staff       (20)    11894 2023-03-20 03:17:38.000000 MeUtils-2023.7.7.15.3.6/meutils/office_automation/pdm.py
--rw-r--r--   0 betterme   (501) staff       (20)    13502 2023-03-21 06:30:39.000000 MeUtils-2023.7.7.15.3.6/meutils/office_automation/pdm_run.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.879554 MeUtils-2023.7.7.15.3.6/meutils/office_automation/report/
--rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/office_automation/report/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)   736444 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/office_automation/投资管理系统O3.2_交易组.pdm
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.880861 MeUtils-2023.7.7.15.3.6/meutils/other/
--rw-r--r--   0 betterme   (501) staff       (20)      996 2023-07-04 01:28:59.000000 MeUtils-2023.7.7.15.3.6/meutils/other/__demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/other/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.882639 MeUtils-2023.7.7.15.3.6/meutils/other/aiomultiprocess/
--rw-r--r--   0 betterme   (501) staff       (20)      416 2023-07-04 01:05:39.000000 MeUtils-2023.7.7.15.3.6/meutils/other/aiomultiprocess/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)       22 2023-07-04 01:01:15.000000 MeUtils-2023.7.7.15.3.6/meutils/other/aiomultiprocess/__version__.py
--rw-r--r--   0 betterme   (501) staff       (20)     7835 2023-07-04 01:01:15.000000 MeUtils-2023.7.7.15.3.6/meutils/other/aiomultiprocess/core.py
--rw-r--r--   0 betterme   (501) staff       (20)    11688 2023-07-04 01:01:15.000000 MeUtils-2023.7.7.15.3.6/meutils/other/aiomultiprocess/pool.py
--rw-r--r--   0 betterme   (501) staff       (20)     2573 2023-07-04 01:01:15.000000 MeUtils-2023.7.7.15.3.6/meutils/other/aiomultiprocess/scheduler.py
--rw-r--r--   0 betterme   (501) staff       (20)     1037 2023-07-04 01:01:15.000000 MeUtils-2023.7.7.15.3.6/meutils/other/aiomultiprocess/types.py
--rw-r--r--   0 betterme   (501) staff       (20)    23121 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/other/besttable.py
--rw-r--r--   0 betterme   (501) staff       (20)    44366 2023-03-21 05:16:40.000000 MeUtils-2023.7.7.15.3.6/meutils/other/crontab.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.883513 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/
--rw-r--r--   0 betterme   (501) staff       (20)      334 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.886675 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/
--rw-r--r--   0 betterme   (501) staff       (20)       59 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1561 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/annlite.py
--rw-r--r--   0 betterme   (501) staff       (20)      581 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/base.py
--rw-r--r--   0 betterme   (501) staff       (20)     2088 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/chunk.py
--rw-r--r--   0 betterme   (501) staff       (20)     8448 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/document.py
--rw-r--r--   0 betterme   (501) staff       (20)      715 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/elastic.py
--rw-r--r--   0 betterme   (501) staff       (20)     1736 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/match.py
--rw-r--r--   0 betterme   (501) staff       (20)     1111 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/memory.py
--rw-r--r--   0 betterme   (501) staff       (20)     1486 2023-04-21 00:49:09.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/milvus.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.891498 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/
--rw-r--r--   0 betterme   (501) staff       (20)     2465 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5114 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/content.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.891921 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/dataloader/
--rw-r--r--   0 betterme   (501) staff       (20)     2939 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/dataloader/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2419 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/dataloader/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     2966 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/delitem.py
--rw-r--r--   0 betterme   (501) staff       (20)     7175 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/embed.py
--rw-r--r--   0 betterme   (501) staff       (20)      649 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/empty.py
--rw-r--r--   0 betterme   (501) staff       (20)    21535 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/evaluation.py
--rw-r--r--   0 betterme   (501) staff       (20)    13576 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     1845 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/getattr.py
--rw-r--r--   0 betterme   (501) staff       (20)     4237 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/getitem.py
--rw-r--r--   0 betterme   (501) staff       (20)     3803 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/group.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.893500 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    14676 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/binary.py
--rw-r--r--   0 betterme   (501) staff       (20)     2588 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/common.py
--rw-r--r--   0 betterme   (501) staff       (20)     4181 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/csv.py
--rw-r--r--   0 betterme   (501) staff       (20)     1317 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/dataframe.py
--rw-r--r--   0 betterme   (501) staff       (20)     9193 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/from_gen.py
--rw-r--r--   0 betterme   (501) staff       (20)     3223 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/json.py
--rw-r--r--   0 betterme   (501) staff       (20)     1348 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/pbar.py
--rw-r--r--   0 betterme   (501) staff       (20)    10591 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/pushpull.py
--rw-r--r--   0 betterme   (501) staff       (20)     4762 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/match.py
--rw-r--r--   0 betterme   (501) staff       (20)    15464 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/parallel.py
--rw-r--r--   0 betterme   (501) staff       (20)    20479 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/plot.py
--rw-r--r--   0 betterme   (501) staff       (20)     3910 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/post.py
--rw-r--r--   0 betterme   (501) staff       (20)     1243 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/pydantic.py
--rw-r--r--   0 betterme   (501) staff       (20)     4129 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/reduce.py
--rw-r--r--   0 betterme   (501) staff       (20)     1612 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/sample.py
--rw-r--r--   0 betterme   (501) staff       (20)     8834 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/setitem.py
--rw-r--r--   0 betterme   (501) staff       (20)      833 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/strawberry.py
--rw-r--r--   0 betterme   (501) staff       (20)     1086 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/text.py
--rw-r--r--   0 betterme   (501) staff       (20)     9638 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/traverse.py
--rw-r--r--   0 betterme   (501) staff       (20)      733 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/opensearch.py
--rw-r--r--   0 betterme   (501) staff       (20)     1806 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/qdrant.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.894237 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/queryset/
--rw-r--r--   0 betterme   (501) staff       (20)       64 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/queryset/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     8771 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/queryset/lookup.py
--rw-r--r--   0 betterme   (501) staff       (20)     3680 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/queryset/parser.py
--rw-r--r--   0 betterme   (501) staff       (20)      647 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/redis.py
--rw-r--r--   0 betterme   (501) staff       (20)     1232 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/sqlite.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.894525 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.895446 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/annlite/
--rw-r--r--   0 betterme   (501) staff       (20)      473 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/annlite/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     4062 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/annlite/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     2078 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/annlite/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     2365 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/annlite/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     4541 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/annlite/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     1424 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/annlite/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.896430 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/base/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/base/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     3861 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/base/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)    12782 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/base/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2078 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/base/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     2680 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/base/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.897354 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/elastic/
--rw-r--r--   0 betterme   (501) staff       (20)      473 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/elastic/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     9847 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/elastic/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     5811 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/elastic/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4746 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/elastic/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     3838 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/elastic/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.898243 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/memory/
--rw-r--r--   0 betterme   (501) staff       (20)      437 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/memory/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2751 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/memory/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     8505 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/memory/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     2453 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/memory/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2046 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/memory/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.899108 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/milvus/
--rw-r--r--   0 betterme   (501) staff       (20)      315 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/milvus/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    12584 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/milvus/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     1897 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/milvus/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4492 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/milvus/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2772 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/milvus/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.900182 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/opensearch/
--rw-r--r--   0 betterme   (501) staff       (20)      491 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/opensearch/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    10803 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/opensearch/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     6436 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/opensearch/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4491 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/opensearch/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     3913 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/opensearch/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.901466 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/qdrant/
--rw-r--r--   0 betterme   (501) staff       (20)     1492 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/qdrant/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     9051 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/qdrant/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     4457 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/qdrant/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4441 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/qdrant/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)      161 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/qdrant/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     2085 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/qdrant/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.902386 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/redis/
--rw-r--r--   0 betterme   (501) staff       (20)      313 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/redis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     7368 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/redis/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     6653 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/redis/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4303 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/redis/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2662 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/redis/seqlike.py
--rw-r--r--   0 betterme   (501) staff       (20)       88 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/registry.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.903304 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/sqlite/
--rw-r--r--   0 betterme   (501) staff       (20)      520 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/sqlite/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     4894 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/sqlite/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     2783 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/sqlite/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2279 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/sqlite/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     2735 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/sqlite/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.904334 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/weaviate/
--rw-r--r--   0 betterme   (501) staff       (20)      479 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/weaviate/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    14786 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/weaviate/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     7830 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/weaviate/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     3285 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/weaviate/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2834 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/weaviate/seqlike.py
--rw-r--r--   0 betterme   (501) staff       (20)     1689 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/weaviate.py
--rw-r--r--   0 betterme   (501) staff       (20)     4806 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/base.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.905394 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/dataclasses/
--rw-r--r--   0 betterme   (501) staff       (20)       80 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/dataclasses/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      633 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/dataclasses/enums.py
--rw-r--r--   0 betterme   (501) staff       (20)     1063 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/dataclasses/getter.py
--rw-r--r--   0 betterme   (501) staff       (20)     2920 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/dataclasses/setter.py
--rw-r--r--   0 betterme   (501) staff       (20)     9205 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/dataclasses/types.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.906491 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/
--rw-r--r--   0 betterme   (501) staff       (20)     4881 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5422 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/data.py
--rw-r--r--   0 betterme   (501) staff       (20)    12146 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/generators.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.910431 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/
--rw-r--r--   0 betterme   (501) staff       (20)     1779 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5775 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/_property.py
--rw-r--r--   0 betterme   (501) staff       (20)      856 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/attribute.py
--rw-r--r--   0 betterme   (501) staff       (20)     2987 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/audio.py
--rw-r--r--   0 betterme   (501) staff       (20)     1988 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/blob.py
--rw-r--r--   0 betterme   (501) staff       (20)      866 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/content.py
--rw-r--r--   0 betterme   (501) staff       (20)     2034 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/convert.py
--rw-r--r--   0 betterme   (501) staff       (20)      701 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/dump.py
--rw-r--r--   0 betterme   (501) staff       (20)     2942 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/featurehash.py
--rw-r--r--   0 betterme   (501) staff       (20)     2749 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)    19532 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/image.py
--rw-r--r--   0 betterme   (501) staff       (20)     5080 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/mesh.py
--rw-r--r--   0 betterme   (501) staff       (20)     8677 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/multimodal.py
--rw-r--r--   0 betterme   (501) staff       (20)    14400 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/plot.py
--rw-r--r--   0 betterme   (501) staff       (20)     6281 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/porting.py
--rw-r--r--   0 betterme   (501) staff       (20)     2930 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/property.py
--rw-r--r--   0 betterme   (501) staff       (20)      839 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/protobuf.py
--rw-r--r--   0 betterme   (501) staff       (20)     2891 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/pydantic.py
--rw-r--r--   0 betterme   (501) staff       (20)     1120 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/rich_embedding.py
--rw-r--r--   0 betterme   (501) staff       (20)     2601 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/strawberry.py
--rw-r--r--   0 betterme   (501) staff       (20)     6782 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/sugar.py
--rw-r--r--   0 betterme   (501) staff       (20)     4811 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/text.py
--rw-r--r--   0 betterme   (501) staff       (20)     5987 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/video.py
--rw-r--r--   0 betterme   (501) staff       (20)     2277 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/pydantic_model.py
--rw-r--r--   0 betterme   (501) staff       (20)     2691 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/strawberry_type.py
--rw-r--r--   0 betterme   (501) staff       (20)    15985 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/helper.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.911152 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.912094 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/distance/
--rw-r--r--   0 betterme   (501) staff       (20)     4465 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/distance/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2990 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/distance/numpy.py
--rw-r--r--   0 betterme   (501) staff       (20)     2107 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/distance/paddle.py
--rw-r--r--   0 betterme   (501) staff       (20)     2287 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/distance/tensorflow.py
--rw-r--r--   0 betterme   (501) staff       (20)     1950 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/distance/torch.py
--rw-r--r--   0 betterme   (501) staff       (20)     6289 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/evaluation.py
--rw-r--r--   0 betterme   (501) staff       (20)     3205 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     9093 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/ndarray.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.912379 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/proto/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/proto/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      173 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/proto/docarray_pb2.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.912713 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/proto/io/
--rw-r--r--   0 betterme   (501) staff       (20)     3132 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/proto/io/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5231 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/proto/io/ndarray.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.913091 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/proto/pb/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/proto/pb/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     4228 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/proto/pb/docarray_pb2.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.913419 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/proto/pb2/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/proto/pb2/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     7490 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/proto/pb2/docarray_pb2.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.913627 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/resources/
--rw-r--r--   0 betterme   (501) staff       (20)     4404 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/resources/ci-vendors.json
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.913819 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/resources/embedding-projector/
--rw-r--r--   0 betterme   (501) staff       (20)   494360 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/resources/embedding-projector/index.html.gz
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.914714 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/score/
--rw-r--r--   0 betterme   (501) staff       (20)      258 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/score/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      977 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/score/data.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.915181 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/score/mixins/
--rw-r--r--   0 betterme   (501) staff       (20)      194 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/score/mixins/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1097 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/score/mixins/property.py
--rw-r--r--   0 betterme   (501) staff       (20)      174 2023-04-18 09:06:43.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/score/mixins/representer.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.915335 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/typing/
--rw-r--r--   0 betterme   (501) staff       (20)     2187 2023-04-21 04:31:21.000000 MeUtils-2023.7.7.15.3.6/meutils/other/docarray/typing/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.917774 MeUtils-2023.7.7.15.3.6/meutils/pandas_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/pandas_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1228 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/pandas_utils/opt.py
--rw-r--r--   0 betterme   (501) staff       (20)     6300 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/pandas_utils/pd_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     2846 2023-04-13 02:51:32.000000 MeUtils-2023.7.7.15.3.6/meutils/path_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     6084 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/pd_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     8435 2023-07-04 01:07:58.000000 MeUtils-2023.7.7.15.3.6/meutils/pipe.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.919552 MeUtils-2023.7.7.15.3.6/meutils/plot_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/plot_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      265 2023-05-09 07:50:11.000000 MeUtils-2023.7.7.15.3.6/meutils/plot_utils/common.py
--rw-r--r--   0 betterme   (501) staff       (20)      732 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/plot_utils/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2611 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/plot_utils/echarts.py
--rw-r--r--   0 betterme   (501) staff       (20)    11980 2023-05-09 07:49:05.000000 MeUtils-2023.7.7.15.3.6/meutils/plot_utils/embedding_plot.py
--rw-r--r--   0 betterme   (501) staff       (20)     3610 2023-04-24 07:54:55.000000 MeUtils-2023.7.7.15.3.6/meutils/plot_utils/mecharts.py
--rw-r--r--   0 betterme   (501) staff       (20)    19326 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/plot_utils/metrics.py
--rw-r--r--   0 betterme   (501) staff       (20)     2449 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/plot_utils/plot_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.920881 MeUtils-2023.7.7.15.3.6/meutils/request_utils/
--rw-r--r--   0 betterme   (501) staff       (20)     2461 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/request_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1503 2023-04-21 05:45:54.000000 MeUtils-2023.7.7.15.3.6/meutils/request_utils/crawler.py
--rw-r--r--   0 betterme   (501) staff       (20)     1767 2023-03-30 02:00:48.000000 MeUtils-2023.7.7.15.3.6/meutils/request_utils/download.py
--rw-r--r--   0 betterme   (501) staff       (20)     1334 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/request_utils/results.py
--rw-r--r--   0 betterme   (501) staff       (20)      417 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/request_utils/wechat.py
--rw-r--r--   0 betterme   (501) staff       (20)      644 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/request_utils/公网ip.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.921558 MeUtils-2023.7.7.15.3.6/meutils/serving/
--rw-r--r--   0 betterme   (501) staff       (20)       22 2023-04-28 03:00:12.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 02:50:45.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2478 2023-05-11 08:02:45.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/_fastapi.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.922145 MeUtils-2023.7.7.15.3.6/meutils/serving/fastapi/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.922666 MeUtils-2023.7.7.15.3.6/meutils/serving/fastapi/__demo/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-29 01:58:15.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/fastapi/__demo/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1444 2023-06-01 01:17:23.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/fastapi/__demo/异步任务.py
--rw-r--r--   0 betterme   (501) staff       (20)      290 2023-05-26 07:01:26.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/fastapi/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2119 2023-07-03 09:53:08.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/fastapi/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.923251 MeUtils-2023.7.7.15.3.6/meutils/serving/fastapi/errors/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-25 10:51:34.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/fastapi/errors/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      277 2023-05-25 10:51:34.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/fastapi/errors/http_error.py
--rw-r--r--   0 betterme   (501) staff       (20)      825 2023-05-25 10:51:34.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/fastapi/errors/validation_error.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.924238 MeUtils-2023.7.7.15.3.6/meutils/serving/gui/
--rw-r--r--   0 betterme   (501) staff       (20)       10 2023-04-18 07:29:22.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/gui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1658 2023-03-21 01:20:09.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/gui/bar.py
--rw-r--r--   0 betterme   (501) staff       (20)     1273 2023-04-18 07:21:04.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/gui/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      210 2023-03-21 01:26:30.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/gui/run.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.924495 MeUtils-2023.7.7.15.3.6/meutils/serving/jina/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.925805 MeUtils-2023.7.7.15.3.6/meutils/serving/jina/__demo/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-16 11:10:26.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/jina/__demo/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      889 2023-06-06 10:44:06.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/jina/__demo/client.py
--rw-r--r--   0 betterme   (501) staff       (20)    13659 2023-05-18 02:37:48.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/jina/__demo/flow.svg
--rw-r--r--   0 betterme   (501) staff       (20)     2011 2023-05-18 02:37:46.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/jina/__demo/server.py
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-16 11:10:26.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/jina/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.926341 MeUtils-2023.7.7.15.3.6/meutils/serving/jina/executors/
--rw-r--r--   0 betterme   (501) staff       (20)     1805 2023-06-07 05:33:04.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/jina/executors/SentenceEncoder.py
--rw-r--r--   0 betterme   (501) staff       (20)     1384 2023-06-06 11:14:22.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/jina/executors/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.926898 MeUtils-2023.7.7.15.3.6/meutils/serving/jina/nlp_serving/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-17 01:14:50.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/jina/nlp_serving/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1079 2023-06-06 07:52:01.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/jina/nlp_serving/word_segmentation.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.928337 MeUtils-2023.7.7.15.3.6/meutils/serving/st_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      290 2023-04-28 10:26:48.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/st_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      826 2023-05-15 04:13:53.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/st_utils/_test.py
--rw-r--r--   0 betterme   (501) staff       (20)     7163 2023-05-30 01:47:36.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/st_utils/common.py
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-05-15 03:46:21.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/st_utils/conf.yaml
--rw-r--r--   0 betterme   (501) staff       (20)      218 2023-04-28 10:38:28.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/st_utils/run.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.929416 MeUtils-2023.7.7.15.3.6/meutils/serving/webui/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.929916 MeUtils-2023.7.7.15.3.6/meutils/serving/webui/.streamlit/
--rw-r--r--   0 betterme   (501) staff       (20)     7586 2023-03-24 08:27:34.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/webui/.streamlit/_config.toml
--rw-r--r--   0 betterme   (501) staff       (20)      511 2023-03-24 08:27:34.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/webui/.streamlit/config.toml
--rw-r--r--   0 betterme   (501) staff       (20)     1756 2023-05-22 09:24:56.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/webui/_2_词性标注与实体识别.py
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-21 09:09:55.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/webui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      508 2023-05-22 10:05:43.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/webui/_🏆_主页.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.930615 MeUtils-2023.7.7.15.3.6/meutils/serving/webui/pages/
--rw-r--r--   0 betterme   (501) staff       (20)     1943 2023-05-22 10:51:26.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/webui/pages/_1_分词.py
--rw-r--r--   0 betterme   (501) staff       (20)     1714 2023-05-22 10:56:06.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/webui/pages/_2_词性标注与实体识别.py
--rw-r--r--   0 betterme   (501) staff       (20)     2424 2023-05-22 10:48:03.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/webui/pages/_3_文本匹配.py
--rwxr--r--   0 betterme   (501) staff       (20)      252 2023-05-22 10:17:52.000000 MeUtils-2023.7.7.15.3.6/meutils/serving/webui/run.sh
--rw-r--r--   0 betterme   (501) staff       (20)      956 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/sftp.py
--rw-r--r--   0 betterme   (501) staff       (20)      796 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/sk_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     1398 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/smooth_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.930918 MeUtils-2023.7.7.15.3.6/meutils/spark/
--rw-r--r--   0 betterme   (501) staff       (20)      576 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/spark/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.931887 MeUtils-2023.7.7.15.3.6/meutils/str_utils/
--rw-r--r--   0 betterme   (501) staff       (20)     1258 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/str_utils/Translator.py
--rw-r--r--   0 betterme   (501) staff       (20)     6655 2023-05-17 05:26:27.000000 MeUtils-2023.7.7.15.3.6/meutils/str_utils/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.932637 MeUtils-2023.7.7.15.3.6/meutils/str_utils/__translater/
--rw-r--r--   0 betterme   (501) staff       (20)      277 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/str_utils/__translater/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1408 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/str_utils/__translater/tencent.py
--rw-r--r--   0 betterme   (501) staff       (20)     1238 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/str_utils/__translater/translater.py
--rw-r--r--   0 betterme   (501) staff       (20)     1168 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/str_utils/__translater/youdao.py
--rw-r--r--   0 betterme   (501) staff       (20)     1095 2023-06-12 09:51:25.000000 MeUtils-2023.7.7.15.3.6/meutils/str_utils/json_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)      926 2023-04-09 12:05:21.000000 MeUtils-2023.7.7.15.3.6/meutils/str_utils/regular_expression.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.935181 MeUtils-2023.7.7.15.3.6/meutils/templates/
--rw-r--r--   0 betterme   (501) staff       (20)      349 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      291 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      224 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/demo.conf
--rw-r--r--   0 betterme   (501) staff       (20)      578 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/demo.j2
--rw-r--r--   0 betterme   (501) staff       (20)      808 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      536 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/demox.py
--rw-r--r--   0 betterme   (501) staff       (20)     2416 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/df_html.j2
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.937767 MeUtils-2023.7.7.15.3.6/meutils/templates/dockerfiles/
--rw-r--r--   0 betterme   (501) staff       (20)      112 2023-03-21 05:16:40.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/dockerfiles/Dockerfile
--rw-r--r--   0 betterme   (501) staff       (20)      170 2023-03-21 05:16:40.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/dockerfiles/Dockerfile_me
--rw-r--r--   0 betterme   (501) staff       (20)      217 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/dockerfiles/Dockerfile_milvus
--rw-r--r--   0 betterme   (501) staff       (20)      245 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/dockerfiles/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      712 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/dockerfiles/docker_build_push.py
--rwxr-xr-x   0 betterme   (501) staff       (20)      386 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/dockerfiles/docker_push.sh
--rw-r--r--   0 betterme   (501) staff       (20)     2266 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/hegui.py
--rw-r--r--   0 betterme   (501) staff       (20)      540 2023-06-29 07:13:14.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/markmap.html
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.937963 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/
--rw-r--r--   0 betterme   (501) staff       (20)      831 2022-05-05 05:21:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/cookiecutter.json
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.942277 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.editorconfig
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.942441 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/
--rw-r--r--   0 betterme   (501) staff       (20)      342 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 betterme   (501) staff       (20)     1198 2023-05-31 00:59:56.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      842 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      178 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     4010 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst
--rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     5987 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      351 2021-09-04 06:53:23.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2516 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)      704 2023-04-18 10:20:21.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     1738 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.945014 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      632 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)      702 2021-09-14 08:44:31.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2022-04-18 06:25:28.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     5157 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)      388 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1410 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst
--rw-r--r--   0 betterme   (501) staff       (20)      829 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/usage.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.945168 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/
--rw-r--r--   0 betterme   (501) staff       (20)      234 2021-09-04 07:26:59.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/demo.py
--rwxr--r--   0 betterme   (501) staff       (20)      244 2022-05-05 05:24:52.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/git_init.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2021-09-01 08:44:34.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)        8 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)      302 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements_dev.txt
--rw-r--r--   0 betterme   (501) staff       (20)      549 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     2532 2022-04-19 09:34:52.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.945528 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       61 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2315 2021-09-03 02:32:04.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py
--rw-r--r--   0 betterme   (501) staff       (20)      678 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.945852 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/
--rw-r--r--   0 betterme   (501) staff       (20)      273 2022-04-18 06:39:54.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.946369 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2021-08-31 05:12:27.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2022-04-27 09:56:07.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      591 2022-04-27 09:56:07.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)       19 2021-09-03 02:19:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}.py
--rw-r--r--   0 betterme   (501) staff       (20)    11496 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/tpl.docx
--rw-r--r--   0 betterme   (501) staff       (20)      537 2023-06-29 07:15:57.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/x.html
--rw-r--r--   0 betterme   (501) staff       (20)   172819 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/templates/合规日报模板.docx
--rw-r--r--   0 betterme   (501) staff       (20)      590 2023-05-08 05:49:55.000000 MeUtils-2023.7.7.15.3.6/meutils/todo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.947430 MeUtils-2023.7.7.15.3.6/meutils/tools/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/tools/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1383 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/tools/cprint.py
--rw-r--r--   0 betterme   (501) staff       (20)     2392 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/tools/machine_monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)      929 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/tools/monitor.yml
--rw-r--r--   0 betterme   (501) staff       (20)     1064 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/tools/seize.py
--rw-r--r--   0 betterme   (501) staff       (20)     1255 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/tools/service_monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)      429 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/tools/sys_monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)      360 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/typings.py
--rw-r--r--   0 betterme   (501) staff       (20)      396 2023-07-06 12:39:08.000000 MeUtils-2023.7.7.15.3.6/meutils/x.py
--rw-r--r--   0 betterme   (501) staff       (20)     2438 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/meutils/zk_utils.py
--rwxr-xr-x   0 betterme   (501) staff       (20)      526 2023-05-15 03:11:01.000000 MeUtils-2023.7.7.15.3.6/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)      351 2023-06-28 06:59:00.000000 MeUtils-2023.7.7.15.3.6/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)       21 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/requirements_ai.txt
--rw-r--r--   0 betterme   (501) staff       (20)       20 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/requirements_ann.txt
--rw-r--r--   0 betterme   (501) staff       (20)       46 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/requirements_app.txt
--rw-r--r--   0 betterme   (501) staff       (20)       52 2023-06-02 06:00:11.000000 MeUtils-2023.7.7.15.3.6/requirements_db.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-05-18 08:43:00.000000 MeUtils-2023.7.7.15.3.6/requirements_fileparser.txt
--rw-r--r--   0 betterme   (501) staff       (20)        6 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/requirements_office.txt
--rw-r--r--   0 betterme   (501) staff       (20)       65 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/requirements_pd.txt
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/requirements_plot.txt
--rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/requirements_plus.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-07-07 07:03:06.948033 MeUtils-2023.7.7.15.3.6/scripts/
--rwxr-xr-x   0 betterme   (501) staff       (20)      251 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/scripts/demo.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      274 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/scripts/killall.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      233 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/scripts/py_sh.sh
--rw-r--r--   0 betterme   (501) staff       (20)       53 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/scripts/yum.sh
--rw-r--r--   0 betterme   (501) staff       (20)       38 2023-07-07 07:03:06.948536 MeUtils-2023.7.7.15.3.6/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     2307 2023-03-20 02:44:39.000000 MeUtils-2023.7.7.15.3.6/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.103077 MeUtils-2023.8.2.13.20.11/
+-rw-r--r--   0 betterme   (501) staff       (20)     6148 2023-04-14 02:46:19.000000 MeUtils-2023.8.2.13.20.11/.DS_Store
+-rw-r--r--   0 betterme   (501) staff       (20)     1204 2023-05-22 06:35:12.000000 MeUtils-2023.8.2.13.20.11/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)    11357 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      249 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/MANIFEST.in
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.015581 MeUtils-2023.8.2.13.20.11/MeUtils.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     1894 2023-08-02 05:20:11.000000 MeUtils-2023.8.2.13.20.11/MeUtils.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)    19508 2023-08-02 05:20:11.000000 MeUtils-2023.8.2.13.20.11/MeUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-08-02 05:20:11.000000 MeUtils-2023.8.2.13.20.11/MeUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      193 2023-08-02 05:20:11.000000 MeUtils-2023.8.2.13.20.11/MeUtils.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1049 2023-08-02 05:20:11.000000 MeUtils-2023.8.2.13.20.11/MeUtils.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       17 2023-08-02 05:20:11.000000 MeUtils-2023.8.2.13.20.11/MeUtils.egg-info/top_level.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1894 2023-08-02 05:20:12.102906 MeUtils-2023.8.2.13.20.11/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1067 2023-05-04 03:00:27.000000 MeUtils-2023.8.2.13.20.11/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1612 2023-07-20 08:15:27.000000 MeUtils-2023.8.2.13.20.11/TODO.md
+-rw-r--r--   0 betterme   (501) staff       (20)      684 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/clear_git_history.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      291 2023-07-27 03:02:44.000000 MeUtils-2023.8.2.13.20.11/git_init.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.018485 MeUtils-2023.8.2.13.20.11/meutils/
+-rw-r--r--   0 betterme   (501) staff       (20)      348 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1850 2023-04-11 05:47:45.000000 MeUtils-2023.8.2.13.20.11/meutils/_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.018751 MeUtils-2023.8.2.13.20.11/meutils/ai_audio/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-17 05:51:24.000000 MeUtils-2023.8.2.13.20.11/meutils/ai_audio/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      637 2023-05-17 05:56:24.000000 MeUtils-2023.8.2.13.20.11/meutils/ai_audio/asr.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.019030 MeUtils-2023.8.2.13.20.11/meutils/ai_cv/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-18 08:11:56.000000 MeUtils-2023.8.2.13.20.11/meutils/ai_cv/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      263 2023-05-18 08:11:56.000000 MeUtils-2023.8.2.13.20.11/meutils/ai_cv/ocr.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.020222 MeUtils-2023.8.2.13.20.11/meutils/ai_nlp/
+-rw-r--r--   0 betterme   (501) staff       (20)     6927 2023-06-30 13:22:13.000000 MeUtils-2023.8.2.13.20.11/meutils/ai_nlp/SplitSentence.py
+-rw-r--r--   0 betterme   (501) staff       (20)    13489 2023-05-21 05:19:20.000000 MeUtils-2023.8.2.13.20.11/meutils/ai_nlp/Untitled-1(1).py
+-rw-r--r--   0 betterme   (501) staff       (20)      244 2023-04-25 06:23:09.000000 MeUtils-2023.8.2.13.20.11/meutils/ai_nlp/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2295 2023-04-10 08:57:58.000000 MeUtils-2023.8.2.13.20.11/meutils/ai_nlp/_lda.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.020655 MeUtils-2023.8.2.13.20.11/meutils/ai_nlp/_textsplitter/
+-rw-r--r--   0 betterme   (501) staff       (20)      287 2023-05-22 01:52:50.000000 MeUtils-2023.8.2.13.20.11/meutils/ai_nlp/_textsplitter/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6673 2023-05-21 05:10:54.000000 MeUtils-2023.8.2.13.20.11/meutils/ai_nlp/_textsplitter/chinese_text_splitter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2282 2023-05-21 05:27:40.000000 MeUtils-2023.8.2.13.20.11/meutils/ai_nlp/_textsplitter/text_split.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1111 2023-06-06 06:44:28.000000 MeUtils-2023.8.2.13.20.11/meutils/ai_nlp/lda.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2560 2023-07-25 08:50:49.000000 MeUtils-2023.8.2.13.20.11/meutils/ai_nlp/ner.py
+-rw-r--r--   0 betterme   (501) staff       (20)      963 2023-07-04 08:24:23.000000 MeUtils-2023.8.2.13.20.11/meutils/ai_nlp/sentence_transformers.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2111 2023-06-30 13:18:15.000000 MeUtils-2023.8.2.13.20.11/meutils/ai_nlp/textsplitter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3542 2023-06-05 05:29:27.000000 MeUtils-2023.8.2.13.20.11/meutils/ai_nlp/word_segmentation.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.022470 MeUtils-2023.8.2.13.20.11/meutils/ann/
+-rw-r--r--   0 betterme   (501) staff       (20)      781 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/ann/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1389 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/ann/README_gensim.md
+-rw-r--r--   0 betterme   (501) staff       (20)      240 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/ann/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9161 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/ann/ann.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5662 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/ann/ann_faiss.py
+-rw-r--r--   0 betterme   (501) staff       (20)      965 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/ann/ann_gensim.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1002 2023-05-16 06:47:06.000000 MeUtils-2023.8.2.13.20.11/meutils/ann/ann_inmemory.py
+-rw-r--r--   0 betterme   (501) staff       (20)      458 2023-05-19 06:06:57.000000 MeUtils-2023.8.2.13.20.11/meutils/ann/ann_qdrant.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1171 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/ann/ann_service.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4743 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/ann/ann_v1.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1927 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/ann/cli.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.022741 MeUtils-2023.8.2.13.20.11/meutils/ann/examples/
+-rw-r--r--   0 betterme   (501) staff       (20)     1476 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/ann/examples/client.py
+-rw-r--r--   0 betterme   (501) staff       (20)      463 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/ann/examples/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      238 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/ann/milvus.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1076 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/ann/shake_demo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.022874 MeUtils-2023.8.2.13.20.11/meutils/asyncio_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      243 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/asyncio_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8771 2023-07-31 06:00:38.000000 MeUtils-2023.8.2.13.20.11/meutils/cache_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.024099 MeUtils-2023.8.2.13.20.11/meutils/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2828 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)      738 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/clis/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2234 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/clis/cron.py
+-rw-r--r--   0 betterme   (501) staff       (20)      595 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/clis/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1517 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/clis/gunicorn.conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      619 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/clis/monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1018 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/clis/nesc.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.024801 MeUtils-2023.8.2.13.20.11/meutils/cmds/
+-rw-r--r--   0 betterme   (501) staff       (20)     1185 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/cmds/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      293 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/cmds/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      458 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/cmds/cmd.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1734 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/cmds/hdfs_cmd.py
+-rw-r--r--   0 betterme   (501) staff       (20)      629 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/cmds/subprocess_demo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.025124 MeUtils-2023.8.2.13.20.11/meutils/coding/
+-rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/coding/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      942 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/coding/find132.py
+-rw-r--r--   0 betterme   (501) staff       (20)    10778 2023-08-02 00:43:22.000000 MeUtils-2023.8.2.13.20.11/meutils/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.025461 MeUtils-2023.8.2.13.20.11/meutils/comp_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      361 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/comp_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1705 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/comp_utils/reverse_metric.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.033862 MeUtils-2023.8.2.13.20.11/meutils/data/
+-rw-r--r--   0 betterme   (501) staff       (20) 10062565 2022-11-07 06:01:38.000000 MeUtils-2023.8.2.13.20.11/meutils/data/SimHei.ttf
+-rw-r--r--   0 betterme   (501) staff       (20)       19 2023-08-02 05:20:11.000000 MeUtils-2023.8.2.13.20.11/meutils/data/VERSION
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/data/_FLAG
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/data/_SUCCESS
+-rw-r--r--   0 betterme   (501) staff       (20)      243 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/data/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      600 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/data/coordinate.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2514 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/date_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.034399 MeUtils-2023.8.2.13.20.11/meutils/db/
+-rw-r--r--   0 betterme   (501) staff       (20)     1507 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/db/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     7396 2023-06-30 01:59:42.000000 MeUtils-2023.8.2.13.20.11/meutils/db/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2337 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/db/mongo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2168 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/db/neo4j.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.038691 MeUtils-2023.8.2.13.20.11/meutils/decorators/
+-rw-r--r--   0 betterme   (501) staff       (20)      238 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/decorators/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1681 2023-05-25 09:49:50.000000 MeUtils-2023.8.2.13.20.11/meutils/decorators/__ai.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3284 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/decorators/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1837 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/decorators/catch.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6482 2023-07-25 08:50:49.000000 MeUtils-2023.8.2.13.20.11/meutils/decorators/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)    15570 2023-04-06 06:24:58.000000 MeUtils-2023.8.2.13.20.11/meutils/decorators/decorator.py
+-rw-r--r--   0 betterme   (501) staff       (20)      754 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/decorators/decorator_demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      527 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/decorators/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2115 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/decorators/feishu.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2741 2023-07-28 07:07:38.000000 MeUtils-2023.8.2.13.20.11/meutils/decorators/retry.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1678 2023-04-04 15:22:58.000000 MeUtils-2023.8.2.13.20.11/meutils/decorators/scheduler.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3640 2023-05-15 10:32:24.000000 MeUtils-2023.8.2.13.20.11/meutils/dist_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.039392 MeUtils-2023.8.2.13.20.11/meutils/docarray_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-18 06:24:19.000000 MeUtils-2023.8.2.13.20.11/meutils/docarray_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      977 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/docarray_utils/demo_es.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1341 2023-04-26 13:37:46.000000 MeUtils-2023.8.2.13.20.11/meutils/docarray_utils/demo_hnsw.py
+-rw-r--r--   0 betterme   (501) staff       (20)      985 2023-04-27 02:39:23.000000 MeUtils-2023.8.2.13.20.11/meutils/docarray_utils/in_memory.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1058 2023-04-27 01:04:00.000000 MeUtils-2023.8.2.13.20.11/meutils/docarray_utils/改造下hnsw.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.039667 MeUtils-2023.8.2.13.20.11/meutils/easy_search/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/easy_search/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2230 2023-07-28 09:02:34.000000 MeUtils-2023.8.2.13.20.11/meutils/easy_search/es.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.040569 MeUtils-2023.8.2.13.20.11/meutils/fileparser/
+-rw-r--r--   0 betterme   (501) staff       (20)     1975 2023-05-30 05:34:49.000000 MeUtils-2023.8.2.13.20.11/meutils/fileparser/PDF抽取.py
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-18 08:38:53.000000 MeUtils-2023.8.2.13.20.11/meutils/fileparser/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      284 2023-07-12 04:10:53.000000 MeUtils-2023.8.2.13.20.11/meutils/fileparser/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1025 2023-07-12 06:55:12.000000 MeUtils-2023.8.2.13.20.11/meutils/fileparser/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.041326 MeUtils-2023.8.2.13.20.11/meutils/fileparser/filetype/
+-rw-r--r--   0 betterme   (501) staff       (20)      223 2023-05-18 08:40:53.000000 MeUtils-2023.8.2.13.20.11/meutils/fileparser/filetype/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      803 2023-05-18 08:40:53.000000 MeUtils-2023.8.2.13.20.11/meutils/fileparser/filetype/__main__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2122 2023-05-18 08:40:53.000000 MeUtils-2023.8.2.13.20.11/meutils/fileparser/filetype/filetype.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2947 2023-05-18 08:40:53.000000 MeUtils-2023.8.2.13.20.11/meutils/fileparser/filetype/helpers.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3288 2023-05-18 08:40:53.000000 MeUtils-2023.8.2.13.20.11/meutils/fileparser/filetype/match.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.042829 MeUtils-2023.8.2.13.20.11/meutils/fileparser/filetype/types/
+-rw-r--r--   0 betterme   (501) staff       (20)     2085 2023-05-18 08:40:53.000000 MeUtils-2023.8.2.13.20.11/meutils/fileparser/filetype/types/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      498 2023-05-18 08:40:53.000000 MeUtils-2023.8.2.13.20.11/meutils/fileparser/filetype/types/application.py
+-rw-r--r--   0 betterme   (501) staff       (20)    17006 2023-05-18 08:40:53.000000 MeUtils-2023.8.2.13.20.11/meutils/fileparser/filetype/types/archive.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4960 2023-05-18 08:40:53.000000 MeUtils-2023.8.2.13.20.11/meutils/fileparser/filetype/types/audio.py
+-rw-r--r--   0 betterme   (501) staff       (20)      647 2023-05-18 08:40:53.000000 MeUtils-2023.8.2.13.20.11/meutils/fileparser/filetype/types/base.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7513 2023-05-18 08:40:53.000000 MeUtils-2023.8.2.13.20.11/meutils/fileparser/filetype/types/document.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2924 2023-05-18 08:40:53.000000 MeUtils-2023.8.2.13.20.11/meutils/fileparser/filetype/types/font.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9130 2023-05-18 08:40:53.000000 MeUtils-2023.8.2.13.20.11/meutils/fileparser/filetype/types/image.py
+-rw-r--r--   0 betterme   (501) staff       (20)      958 2023-05-18 08:40:53.000000 MeUtils-2023.8.2.13.20.11/meutils/fileparser/filetype/types/isobmff.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5371 2023-05-18 08:40:53.000000 MeUtils-2023.8.2.13.20.11/meutils/fileparser/filetype/types/video.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2089 2023-05-18 08:40:53.000000 MeUtils-2023.8.2.13.20.11/meutils/fileparser/filetype/utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)      285 2023-07-15 07:06:30.000000 MeUtils-2023.8.2.13.20.11/meutils/fileparser/filetype.py
+-rw-r--r--   0 betterme   (501) staff       (20)      263 2023-05-18 08:39:36.000000 MeUtils-2023.8.2.13.20.11/meutils/fileparser/pdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4037 2023-07-17 10:15:11.000000 MeUtils-2023.8.2.13.20.11/meutils/fileparser/表格抽取.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2393 2023-04-04 15:30:40.000000 MeUtils-2023.8.2.13.20.11/meutils/hash_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)      969 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/import_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.043327 MeUtils-2023.8.2.13.20.11/meutils/init/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-04-27 08:58:17.000000 MeUtils-2023.8.2.13.20.11/meutils/init/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1559 2023-07-26 06:41:28.000000 MeUtils-2023.8.2.13.20.11/meutils/init/evn.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12884 2023-07-06 01:18:39.000000 MeUtils-2023.8.2.13.20.11/meutils/init/oo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.044185 MeUtils-2023.8.2.13.20.11/meutils/io/
+-rw-r--r--   0 betterme   (501) staff       (20)     2107 2023-04-13 02:51:32.000000 MeUtils-2023.8.2.13.20.11/meutils/io/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      409 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/io/file.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2319 2023-05-30 01:57:16.000000 MeUtils-2023.8.2.13.20.11/meutils/io/image.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8605 2023-06-26 01:26:21.000000 MeUtils-2023.8.2.13.20.11/meutils/io/tf_io.py
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/io/x.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      708 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/jinja_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2512 2023-04-02 12:55:05.000000 MeUtils-2023.8.2.13.20.11/meutils/log_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.045551 MeUtils-2023.8.2.13.20.11/meutils/notice/
+-rw-r--r--   0 betterme   (501) staff       (20)      837 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/notice/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2403 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/notice/emails.py
+-rw-r--r--   0 betterme   (501) staff       (20)      703 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/notice/feishu.py
+-rw-r--r--   0 betterme   (501) staff       (20)      953 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/notice/file_post.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2511 2023-06-13 09:13:04.000000 MeUtils-2023.8.2.13.20.11/meutils/notice/wechat.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3215 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/notice/wechat_.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6983 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/notice/wecom.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1102 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/notice/weekmeet.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2962 2023-05-16 06:23:15.000000 MeUtils-2023.8.2.13.20.11/meutils/np_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.046559 MeUtils-2023.8.2.13.20.11/meutils/office_automation/
+-rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/office_automation/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      508 2023-03-27 04:08:21.000000 MeUtils-2023.8.2.13.20.11/meutils/office_automation/doc.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1528 2023-07-25 10:06:46.000000 MeUtils-2023.8.2.13.20.11/meutils/office_automation/pdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11894 2023-03-20 03:17:38.000000 MeUtils-2023.8.2.13.20.11/meutils/office_automation/pdm.py
+-rw-r--r--   0 betterme   (501) staff       (20)    13502 2023-03-21 06:30:39.000000 MeUtils-2023.8.2.13.20.11/meutils/office_automation/pdm_run.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.047175 MeUtils-2023.8.2.13.20.11/meutils/office_automation/report/
+-rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/office_automation/report/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)   736444 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/office_automation/投资管理系统O3.2_交易组.pdm
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.048139 MeUtils-2023.8.2.13.20.11/meutils/other/
+-rw-r--r--   0 betterme   (501) staff       (20)      996 2023-07-04 01:28:59.000000 MeUtils-2023.8.2.13.20.11/meutils/other/__demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/other/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.049155 MeUtils-2023.8.2.13.20.11/meutils/other/aiomultiprocess/
+-rw-r--r--   0 betterme   (501) staff       (20)      416 2023-07-04 01:05:39.000000 MeUtils-2023.8.2.13.20.11/meutils/other/aiomultiprocess/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)       22 2023-07-04 01:01:15.000000 MeUtils-2023.8.2.13.20.11/meutils/other/aiomultiprocess/__version__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7835 2023-07-04 01:01:15.000000 MeUtils-2023.8.2.13.20.11/meutils/other/aiomultiprocess/core.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11688 2023-07-04 01:01:15.000000 MeUtils-2023.8.2.13.20.11/meutils/other/aiomultiprocess/pool.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2573 2023-07-04 01:01:15.000000 MeUtils-2023.8.2.13.20.11/meutils/other/aiomultiprocess/scheduler.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1037 2023-07-04 01:01:15.000000 MeUtils-2023.8.2.13.20.11/meutils/other/aiomultiprocess/types.py
+-rw-r--r--   0 betterme   (501) staff       (20)    23121 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/other/besttable.py
+-rw-r--r--   0 betterme   (501) staff       (20)    44366 2023-03-21 05:16:40.000000 MeUtils-2023.8.2.13.20.11/meutils/other/crontab.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.049779 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/
+-rw-r--r--   0 betterme   (501) staff       (20)      334 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.052257 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/
+-rw-r--r--   0 betterme   (501) staff       (20)       59 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1561 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/annlite.py
+-rw-r--r--   0 betterme   (501) staff       (20)      581 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/base.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2088 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/chunk.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8448 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/document.py
+-rw-r--r--   0 betterme   (501) staff       (20)      715 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/elastic.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1736 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/match.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1111 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/memory.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1486 2023-04-21 00:49:09.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/milvus.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.056068 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/
+-rw-r--r--   0 betterme   (501) staff       (20)     2465 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5114 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/content.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.056645 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/dataloader/
+-rw-r--r--   0 betterme   (501) staff       (20)     2939 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/dataloader/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2419 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/dataloader/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2966 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/delitem.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7175 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/embed.py
+-rw-r--r--   0 betterme   (501) staff       (20)      649 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/empty.py
+-rw-r--r--   0 betterme   (501) staff       (20)    21535 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/evaluation.py
+-rw-r--r--   0 betterme   (501) staff       (20)    13576 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1845 2023-04-18 09:06:43.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/getattr.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4237 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/getitem.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3803 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/group.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.059135 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/io/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/io/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    14676 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/io/binary.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2588 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/io/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4181 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/io/csv.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1317 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/io/dataframe.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9193 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/io/from_gen.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3223 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/io/json.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1348 2023-04-18 09:06:43.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/io/pbar.py
+-rw-r--r--   0 betterme   (501) staff       (20)    10591 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/io/pushpull.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4762 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/match.py
+-rw-r--r--   0 betterme   (501) staff       (20)    15464 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/parallel.py
+-rw-r--r--   0 betterme   (501) staff       (20)    20479 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/plot.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3910 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/post.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1243 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/pydantic.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4129 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/reduce.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1612 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/sample.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8834 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/setitem.py
+-rw-r--r--   0 betterme   (501) staff       (20)      833 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/strawberry.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1086 2023-04-18 09:06:43.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/text.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9638 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/traverse.py
+-rw-r--r--   0 betterme   (501) staff       (20)      733 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/opensearch.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1806 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/qdrant.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.059743 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/queryset/
+-rw-r--r--   0 betterme   (501) staff       (20)       64 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/queryset/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8771 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/queryset/lookup.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3680 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/queryset/parser.py
+-rw-r--r--   0 betterme   (501) staff       (20)      647 2023-04-18 09:06:43.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/redis.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1232 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/sqlite.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.059988 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.061464 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/annlite/
+-rw-r--r--   0 betterme   (501) staff       (20)      473 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/annlite/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4062 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/annlite/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2078 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/annlite/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2365 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/annlite/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4541 2023-04-18 09:06:43.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/annlite/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1424 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/annlite/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.062533 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/base/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/base/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3861 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/base/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12782 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/base/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2078 2023-04-18 09:06:43.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/base/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2680 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/base/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.063582 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/elastic/
+-rw-r--r--   0 betterme   (501) staff       (20)      473 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/elastic/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9847 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/elastic/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5811 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/elastic/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4746 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/elastic/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3838 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/elastic/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.064737 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/memory/
+-rw-r--r--   0 betterme   (501) staff       (20)      437 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/memory/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2751 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/memory/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8505 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/memory/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2453 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/memory/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2046 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/memory/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.065753 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/milvus/
+-rw-r--r--   0 betterme   (501) staff       (20)      315 2023-04-18 09:06:43.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/milvus/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12584 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/milvus/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1897 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/milvus/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4492 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/milvus/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2772 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/milvus/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.066769 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/opensearch/
+-rw-r--r--   0 betterme   (501) staff       (20)      491 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/opensearch/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    10803 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/opensearch/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6436 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/opensearch/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4491 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/opensearch/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3913 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/opensearch/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.068055 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/qdrant/
+-rw-r--r--   0 betterme   (501) staff       (20)     1492 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/qdrant/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9051 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/qdrant/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4457 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/qdrant/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4441 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/qdrant/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)      161 2023-04-18 09:06:43.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/qdrant/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2085 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/qdrant/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.068988 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/redis/
+-rw-r--r--   0 betterme   (501) staff       (20)      313 2023-04-18 09:06:43.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/redis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7368 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/redis/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6653 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/redis/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4303 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/redis/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2662 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/redis/seqlike.py
+-rw-r--r--   0 betterme   (501) staff       (20)       88 2023-04-18 09:06:43.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/registry.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.069887 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/sqlite/
+-rw-r--r--   0 betterme   (501) staff       (20)      520 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/sqlite/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4894 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/sqlite/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2783 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/sqlite/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2279 2023-04-18 09:06:43.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/sqlite/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2735 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/sqlite/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.070901 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/weaviate/
+-rw-r--r--   0 betterme   (501) staff       (20)      479 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/weaviate/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    14786 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/weaviate/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7830 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/weaviate/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3285 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/weaviate/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2834 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/weaviate/seqlike.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1689 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/weaviate.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4806 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/base.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.071656 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/dataclasses/
+-rw-r--r--   0 betterme   (501) staff       (20)       80 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/dataclasses/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      633 2023-04-18 09:06:43.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/dataclasses/enums.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1063 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/dataclasses/getter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2920 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/dataclasses/setter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9205 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/dataclasses/types.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.072360 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/
+-rw-r--r--   0 betterme   (501) staff       (20)     4881 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5422 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/data.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12146 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/generators.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.075646 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/
+-rw-r--r--   0 betterme   (501) staff       (20)     1779 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5775 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/_property.py
+-rw-r--r--   0 betterme   (501) staff       (20)      856 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/attribute.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2987 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/audio.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1988 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/blob.py
+-rw-r--r--   0 betterme   (501) staff       (20)      866 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/content.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2034 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/convert.py
+-rw-r--r--   0 betterme   (501) staff       (20)      701 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/dump.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2942 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/featurehash.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2749 2023-04-18 09:06:43.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)    19532 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/image.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5080 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/mesh.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8677 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/multimodal.py
+-rw-r--r--   0 betterme   (501) staff       (20)    14400 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/plot.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6281 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/porting.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2930 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/property.py
+-rw-r--r--   0 betterme   (501) staff       (20)      839 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/protobuf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2891 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/pydantic.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1120 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/rich_embedding.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2601 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/strawberry.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6782 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/sugar.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4811 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/text.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5987 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/video.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2277 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/pydantic_model.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2691 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/strawberry_type.py
+-rw-r--r--   0 betterme   (501) staff       (20)    15985 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/helper.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.076143 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/math/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/math/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.076777 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/math/distance/
+-rw-r--r--   0 betterme   (501) staff       (20)     4465 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/math/distance/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2990 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/math/distance/numpy.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2107 2023-04-18 09:06:43.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/math/distance/paddle.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2287 2023-04-18 09:06:43.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/math/distance/tensorflow.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1950 2023-04-18 09:06:43.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/math/distance/torch.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6289 2023-04-18 09:06:43.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/math/evaluation.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3205 2023-04-18 09:06:43.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/math/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9093 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/math/ndarray.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.077011 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/proto/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/proto/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      173 2023-04-18 09:06:43.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/proto/docarray_pb2.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.077269 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/proto/io/
+-rw-r--r--   0 betterme   (501) staff       (20)     3132 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/proto/io/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5231 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/proto/io/ndarray.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.077497 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/proto/pb/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/proto/pb/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4228 2023-04-18 09:06:43.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/proto/pb/docarray_pb2.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.077725 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/proto/pb2/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/proto/pb2/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7490 2023-04-18 09:06:43.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/proto/pb2/docarray_pb2.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.077853 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/resources/
+-rw-r--r--   0 betterme   (501) staff       (20)     4404 2023-04-18 09:06:43.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/resources/ci-vendors.json
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.077980 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/resources/embedding-projector/
+-rw-r--r--   0 betterme   (501) staff       (20)   494360 2023-04-18 09:06:43.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/resources/embedding-projector/index.html.gz
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.079262 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/score/
+-rw-r--r--   0 betterme   (501) staff       (20)      258 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/score/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      977 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/score/data.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.079695 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/score/mixins/
+-rw-r--r--   0 betterme   (501) staff       (20)      194 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/score/mixins/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1097 2023-04-18 09:06:43.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/score/mixins/property.py
+-rw-r--r--   0 betterme   (501) staff       (20)      174 2023-04-18 09:06:43.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/score/mixins/representer.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.079834 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/typing/
+-rw-r--r--   0 betterme   (501) staff       (20)     2187 2023-04-21 04:31:21.000000 MeUtils-2023.8.2.13.20.11/meutils/other/docarray/typing/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.080251 MeUtils-2023.8.2.13.20.11/meutils/pandas_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/pandas_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1228 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/pandas_utils/opt.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6300 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/pandas_utils/pd_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2846 2023-04-13 02:51:32.000000 MeUtils-2023.8.2.13.20.11/meutils/path_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6084 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/pd_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9335 2023-07-27 08:48:25.000000 MeUtils-2023.8.2.13.20.11/meutils/pipe.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.081327 MeUtils-2023.8.2.13.20.11/meutils/plot_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/plot_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      265 2023-05-09 07:50:11.000000 MeUtils-2023.8.2.13.20.11/meutils/plot_utils/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)      732 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/plot_utils/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2611 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/plot_utils/echarts.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11980 2023-05-09 07:49:05.000000 MeUtils-2023.8.2.13.20.11/meutils/plot_utils/embedding_plot.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3610 2023-04-24 07:54:55.000000 MeUtils-2023.8.2.13.20.11/meutils/plot_utils/mecharts.py
+-rw-r--r--   0 betterme   (501) staff       (20)    19326 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/plot_utils/metrics.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2449 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/plot_utils/plot_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.081598 MeUtils-2023.8.2.13.20.11/meutils/queues/
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-07-20 02:35:53.000000 MeUtils-2023.8.2.13.20.11/meutils/queues/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1704 2023-07-20 03:22:15.000000 MeUtils-2023.8.2.13.20.11/meutils/queues/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.082450 MeUtils-2023.8.2.13.20.11/meutils/request_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)     3375 2023-07-27 05:15:39.000000 MeUtils-2023.8.2.13.20.11/meutils/request_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1503 2023-04-21 05:45:54.000000 MeUtils-2023.8.2.13.20.11/meutils/request_utils/crawler.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1767 2023-03-30 02:00:48.000000 MeUtils-2023.8.2.13.20.11/meutils/request_utils/download.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1334 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/request_utils/results.py
+-rw-r--r--   0 betterme   (501) staff       (20)      417 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/request_utils/wechat.py
+-rw-r--r--   0 betterme   (501) staff       (20)      644 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/request_utils/公网ip.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.082852 MeUtils-2023.8.2.13.20.11/meutils/serving/
+-rw-r--r--   0 betterme   (501) staff       (20)       22 2023-04-28 03:00:12.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 02:50:45.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2478 2023-05-11 08:02:45.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/_fastapi.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.083134 MeUtils-2023.8.2.13.20.11/meutils/serving/fastapi/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.083452 MeUtils-2023.8.2.13.20.11/meutils/serving/fastapi/__demo/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-29 01:58:15.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/fastapi/__demo/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1444 2023-06-01 01:17:23.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/fastapi/__demo/异步任务.py
+-rw-r--r--   0 betterme   (501) staff       (20)      290 2023-05-26 07:01:26.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/fastapi/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2106 2023-07-24 09:52:55.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/fastapi/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.083895 MeUtils-2023.8.2.13.20.11/meutils/serving/fastapi/errors/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-25 10:51:34.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/fastapi/errors/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      277 2023-05-25 10:51:34.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/fastapi/errors/http_error.py
+-rw-r--r--   0 betterme   (501) staff       (20)      825 2023-05-25 10:51:34.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/fastapi/errors/validation_error.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.084501 MeUtils-2023.8.2.13.20.11/meutils/serving/gui/
+-rw-r--r--   0 betterme   (501) staff       (20)       10 2023-04-18 07:29:22.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/gui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1658 2023-03-21 01:20:09.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/gui/bar.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1273 2023-04-18 07:21:04.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/gui/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      210 2023-03-21 01:26:30.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/gui/run.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.084661 MeUtils-2023.8.2.13.20.11/meutils/serving/jina/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.085759 MeUtils-2023.8.2.13.20.11/meutils/serving/jina/__demo/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-16 11:10:26.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/jina/__demo/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      889 2023-06-06 10:44:06.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/jina/__demo/client.py
+-rw-r--r--   0 betterme   (501) staff       (20)    14055 2023-07-24 05:52:25.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/jina/__demo/flow.svg
+-rw-r--r--   0 betterme   (501) staff       (20)      926 2023-07-24 06:13:28.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/jina/__demo/s.py
+-rw-r--r--   0 betterme   (501) staff       (20)      953 2023-07-24 06:17:01.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/jina/__demo/s2.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2113 2023-07-24 06:04:10.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/jina/__demo/server.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1160 2023-07-19 06:57:16.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/jina/__demo/test.py
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-16 11:10:26.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/jina/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.086549 MeUtils-2023.8.2.13.20.11/meutils/serving/jina/executors/
+-rw-r--r--   0 betterme   (501) staff       (20)     1805 2023-06-07 05:33:04.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/jina/executors/SentenceEncoder.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1831 2023-07-17 10:23:25.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/jina/executors/SentenceEncoder_.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1384 2023-06-06 11:14:22.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/jina/executors/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1093 2023-07-24 06:57:00.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/jina/executors/base.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.086847 MeUtils-2023.8.2.13.20.11/meutils/serving/jina/nlp_serving/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-17 01:14:50.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/jina/nlp_serving/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1079 2023-06-06 07:52:01.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/jina/nlp_serving/word_segmentation.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.087497 MeUtils-2023.8.2.13.20.11/meutils/serving/st_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      290 2023-04-28 10:26:48.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/st_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      826 2023-05-15 04:13:53.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/st_utils/_test.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7163 2023-05-30 01:47:36.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/st_utils/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-05-15 03:46:21.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/st_utils/conf.yaml
+-rw-r--r--   0 betterme   (501) staff       (20)      218 2023-04-28 10:38:28.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/st_utils/run.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.088113 MeUtils-2023.8.2.13.20.11/meutils/serving/webui/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.088449 MeUtils-2023.8.2.13.20.11/meutils/serving/webui/.streamlit/
+-rw-r--r--   0 betterme   (501) staff       (20)     7586 2023-03-24 08:27:34.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/webui/.streamlit/_config.toml
+-rw-r--r--   0 betterme   (501) staff       (20)      511 2023-03-24 08:27:34.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/webui/.streamlit/config.toml
+-rw-r--r--   0 betterme   (501) staff       (20)     1756 2023-05-22 09:24:56.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/webui/_2_词性标注与实体识别.py
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-21 09:09:55.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/webui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      508 2023-05-22 10:05:43.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/webui/_🏆_主页.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.088947 MeUtils-2023.8.2.13.20.11/meutils/serving/webui/pages/
+-rw-r--r--   0 betterme   (501) staff       (20)     1943 2023-05-22 10:51:26.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/webui/pages/_1_分词.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1714 2023-05-22 10:56:06.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/webui/pages/_2_词性标注与实体识别.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2424 2023-05-22 10:48:03.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/webui/pages/_3_文本匹配.py
+-rwxr--r--   0 betterme   (501) staff       (20)      252 2023-05-22 10:17:52.000000 MeUtils-2023.8.2.13.20.11/meutils/serving/webui/run.sh
+-rw-r--r--   0 betterme   (501) staff       (20)      956 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/sftp.py
+-rw-r--r--   0 betterme   (501) staff       (20)      796 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/sk_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1398 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/smooth_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.089104 MeUtils-2023.8.2.13.20.11/meutils/spark/
+-rw-r--r--   0 betterme   (501) staff       (20)      576 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/spark/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.089672 MeUtils-2023.8.2.13.20.11/meutils/str_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)     1258 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/str_utils/Translator.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6655 2023-05-17 05:26:27.000000 MeUtils-2023.8.2.13.20.11/meutils/str_utils/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.090198 MeUtils-2023.8.2.13.20.11/meutils/str_utils/__translater/
+-rw-r--r--   0 betterme   (501) staff       (20)      277 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/str_utils/__translater/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1408 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/str_utils/__translater/tencent.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1238 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/str_utils/__translater/translater.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1168 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/str_utils/__translater/youdao.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1095 2023-06-12 09:51:25.000000 MeUtils-2023.8.2.13.20.11/meutils/str_utils/json_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)      926 2023-04-09 12:05:21.000000 MeUtils-2023.8.2.13.20.11/meutils/str_utils/regular_expression.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.091896 MeUtils-2023.8.2.13.20.11/meutils/templates/
+-rw-r--r--   0 betterme   (501) staff       (20)      349 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      291 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      224 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/demo.conf
+-rw-r--r--   0 betterme   (501) staff       (20)      578 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/demo.j2
+-rw-r--r--   0 betterme   (501) staff       (20)      808 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      536 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/demox.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2416 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/df_html.j2
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.093239 MeUtils-2023.8.2.13.20.11/meutils/templates/dockerfiles/
+-rw-r--r--   0 betterme   (501) staff       (20)      112 2023-03-21 05:16:40.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/dockerfiles/Dockerfile
+-rw-r--r--   0 betterme   (501) staff       (20)      170 2023-03-21 05:16:40.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/dockerfiles/Dockerfile_me
+-rw-r--r--   0 betterme   (501) staff       (20)      217 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/dockerfiles/Dockerfile_milvus
+-rw-r--r--   0 betterme   (501) staff       (20)      245 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/dockerfiles/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      712 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/dockerfiles/docker_build_push.py
+-rwxr-xr-x   0 betterme   (501) staff       (20)      386 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/dockerfiles/docker_push.sh
+-rw-r--r--   0 betterme   (501) staff       (20)     2266 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/hegui.py
+-rw-r--r--   0 betterme   (501) staff       (20)      540 2023-06-29 07:13:14.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/markmap.html
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.093401 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/
+-rw-r--r--   0 betterme   (501) staff       (20)      831 2022-05-05 05:21:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/cookiecutter.json
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.096697 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2021-09-03 02:19:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.editorconfig
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.096903 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/
+-rw-r--r--   0 betterme   (501) staff       (20)      342 2021-09-03 02:19:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1198 2023-05-31 00:59:56.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      842 2021-09-03 02:19:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      178 2021-09-03 02:19:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     4010 2021-09-03 02:19:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     5987 2021-09-03 02:19:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      351 2021-09-04 06:53:23.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2516 2021-09-03 02:19:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)      704 2023-04-18 10:20:21.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1738 2021-09-03 02:19:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.099358 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      632 2021-09-03 02:19:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)      702 2021-09-14 08:44:31.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2022-04-18 06:25:28.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     5157 2021-09-03 02:19:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2021-09-03 02:19:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      388 2021-09-03 02:19:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1410 2021-09-03 02:19:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      829 2021-09-03 02:19:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2021-09-03 02:19:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/usage.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.099499 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/
+-rw-r--r--   0 betterme   (501) staff       (20)      234 2021-09-04 07:26:59.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/demo.py
+-rwxr--r--   0 betterme   (501) staff       (20)      244 2022-05-05 05:24:52.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/git_init.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2021-09-01 08:44:34.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2021-09-03 02:19:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      302 2021-09-03 02:19:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements_dev.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      549 2021-09-03 02:19:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     2532 2022-04-19 09:34:52.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.099769 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       61 2021-09-03 02:19:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2315 2021-09-03 02:32:04.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py
+-rw-r--r--   0 betterme   (501) staff       (20)      678 2021-09-03 02:19:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.100176 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 betterme   (501) staff       (20)      273 2022-04-18 06:39:54.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.101022 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2021-08-31 05:12:27.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2022-04-27 09:56:07.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      591 2022-04-27 09:56:07.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)       19 2021-09-03 02:19:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11496 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/tpl.docx
+-rw-r--r--   0 betterme   (501) staff       (20)      537 2023-06-29 07:15:57.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/x.html
+-rw-r--r--   0 betterme   (501) staff       (20)   172819 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/templates/合规日报模板.docx
+-rw-r--r--   0 betterme   (501) staff       (20)      590 2023-05-08 05:49:55.000000 MeUtils-2023.8.2.13.20.11/meutils/todo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.102120 MeUtils-2023.8.2.13.20.11/meutils/tools/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/tools/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1383 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/tools/cprint.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2392 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/tools/machine_monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)      929 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/tools/monitor.yml
+-rw-r--r--   0 betterme   (501) staff       (20)     1064 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/tools/seize.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1255 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/tools/service_monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)      429 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/tools/sys_monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2438 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/meutils/zk_utils.py
+-rwxr-xr-x   0 betterme   (501) staff       (20)      526 2023-05-15 03:11:01.000000 MeUtils-2023.8.2.13.20.11/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)      369 2023-07-07 09:51:37.000000 MeUtils-2023.8.2.13.20.11/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       21 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/requirements_ai.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       20 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/requirements_ann.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       46 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/requirements_app.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       52 2023-06-02 06:00:11.000000 MeUtils-2023.8.2.13.20.11/requirements_db.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-05-18 08:43:00.000000 MeUtils-2023.8.2.13.20.11/requirements_fileparser.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        6 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/requirements_office.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       65 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/requirements_pd.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/requirements_plot.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/requirements_plus.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-02 05:20:12.102667 MeUtils-2023.8.2.13.20.11/scripts/
+-rwxr-xr-x   0 betterme   (501) staff       (20)      251 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/scripts/demo.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      274 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/scripts/killall.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      233 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/scripts/py_sh.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       53 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/scripts/yum.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2023-08-02 05:20:12.103128 MeUtils-2023.8.2.13.20.11/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     2307 2023-03-20 02:44:39.000000 MeUtils-2023.8.2.13.20.11/setup.py
```

### Comparing `MeUtils-2023.7.7.15.3.6/.gitignore` & `MeUtils-2023.8.2.13.20.11/.gitignore`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/LICENSE` & `MeUtils-2023.8.2.13.20.11/LICENSE`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/MeUtils.egg-info/PKG-INFO` & `MeUtils-2023.8.2.13.20.11/MeUtils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MeUtils
-Version: 2023.7.7.15.3.6
+Version: 2023.8.2.13.20.11
 Summary: description
 Home-page: https://github.com/yuanjie-ai/MeUtils
 Author: yuanjie
 Author-email: 313303303@qq.com
 Maintainer: yuanjie
 Maintainer-email: 313303303@qq.com
 License: MIT License
```

### Comparing `MeUtils-2023.7.7.15.3.6/MeUtils.egg-info/SOURCES.txt` & `MeUtils-2023.8.2.13.20.11/MeUtils.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+.DS_Store
 .gitignore
 LICENSE
 MANIFEST.in
 README.md
 TODO.md
 clear_git_history.sh
 git_init.sh
@@ -37,16 +38,14 @@
 meutils/path_utils.py
 meutils/pd_utils.py
 meutils/pipe.py
 meutils/sftp.py
 meutils/sk_utils.py
 meutils/smooth_utils.py
 meutils/todo.py
-meutils/typings.py
-meutils/x.py
 meutils/zk_utils.py
 meutils/ai_audio/__init__.py
 meutils/ai_audio/asr.py
 meutils/ai_cv/__init__.py
 meutils/ai_cv/ocr.py
 meutils/ai_nlp/SplitSentence.py
 meutils/ai_nlp/Untitled-1(1).py
@@ -72,17 +71,14 @@
 meutils/ann/ann_v1.py
 meutils/ann/cli.py
 meutils/ann/milvus.py
 meutils/ann/shake_demo.py
 meutils/ann/examples/client.py
 meutils/ann/examples/demo.py
 meutils/asyncio_utils/__init__.py
-meutils/cachedir/cache.db
-meutils/cachedir/cache.db-shm
-meutils/cachedir/cache.db-wal
 meutils/clis/README.md
 meutils/clis/__init__.py
 meutils/clis/cli.py
 meutils/clis/conf.py
 meutils/clis/cron.py
 meutils/clis/demo.py
 meutils/clis/gunicorn.conf.py
@@ -125,15 +121,33 @@
 meutils/docarray_utils/改造下hnsw.py
 meutils/easy_search/__init__.py
 meutils/easy_search/es.py
 meutils/fileparser/PDF抽取.py
 meutils/fileparser/README.md
 meutils/fileparser/__init__.py
 meutils/fileparser/common.py
+meutils/fileparser/filetype.py
 meutils/fileparser/pdf.py
+meutils/fileparser/表格抽取.py
+meutils/fileparser/filetype/__init__.py
+meutils/fileparser/filetype/__main__.py
+meutils/fileparser/filetype/filetype.py
+meutils/fileparser/filetype/helpers.py
+meutils/fileparser/filetype/match.py
+meutils/fileparser/filetype/utils.py
+meutils/fileparser/filetype/types/__init__.py
+meutils/fileparser/filetype/types/application.py
+meutils/fileparser/filetype/types/archive.py
+meutils/fileparser/filetype/types/audio.py
+meutils/fileparser/filetype/types/base.py
+meutils/fileparser/filetype/types/document.py
+meutils/fileparser/filetype/types/font.py
+meutils/fileparser/filetype/types/image.py
+meutils/fileparser/filetype/types/isobmff.py
+meutils/fileparser/filetype/types/video.py
 meutils/init/__init__.py
 meutils/init/evn.py
 meutils/init/oo.py
 meutils/io/__init__.py
 meutils/io/file.py
 meutils/io/image.py
 meutils/io/tf_io.py
@@ -334,14 +348,16 @@
 meutils/plot_utils/common.py
 meutils/plot_utils/demo.py
 meutils/plot_utils/echarts.py
 meutils/plot_utils/embedding_plot.py
 meutils/plot_utils/mecharts.py
 meutils/plot_utils/metrics.py
 meutils/plot_utils/plot_utils.py
+meutils/queues/__init__.py
+meutils/queues/common.py
 meutils/request_utils/__init__.py
 meutils/request_utils/crawler.py
 meutils/request_utils/download.py
 meutils/request_utils/results.py
 meutils/request_utils/wechat.py
 meutils/request_utils/公网ip.py
 meutils/serving/README.md
@@ -358,17 +374,22 @@
 meutils/serving/gui/bar.py
 meutils/serving/gui/demo.py
 meutils/serving/gui/run.sh
 meutils/serving/jina/__init__.py
 meutils/serving/jina/__demo/__init__.py
 meutils/serving/jina/__demo/client.py
 meutils/serving/jina/__demo/flow.svg
+meutils/serving/jina/__demo/s.py
+meutils/serving/jina/__demo/s2.py
 meutils/serving/jina/__demo/server.py
+meutils/serving/jina/__demo/test.py
 meutils/serving/jina/executors/SentenceEncoder.py
+meutils/serving/jina/executors/SentenceEncoder_.py
 meutils/serving/jina/executors/__init__.py
+meutils/serving/jina/executors/base.py
 meutils/serving/jina/nlp_serving/__init__.py
 meutils/serving/jina/nlp_serving/word_segmentation.py
 meutils/serving/st_utils/__init__.py
 meutils/serving/st_utils/_test.py
 meutils/serving/st_utils/common.py
 meutils/serving/st_utils/conf.yaml
 meutils/serving/st_utils/run.sh
```

### Comparing `MeUtils-2023.7.7.15.3.6/MeUtils.egg-info/requires.txt` & `MeUtils-2023.8.2.13.20.11/MeUtils.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -17,53 +17,54 @@
 pyyaml
 wget
 requests
 tenacity
 lxml
 pydantic
 schedule
+diskcache
 
 [ai]
 faiss-gpu
 gensim
 
 [all]
-missingno
-gensim
-pandas_summary
-pymupd
-fastapi[all]
-pretty_errors
-reportlab
-iteration_utilities
 streamlit
-jmespath
 seaborn
-thriftpy2
-jieba
-redis-py-cluster
-polars
 pandas-profiling[notebook]
-cachetools
-asyncmy
-faiss-cpu
 pyarrow
+uvicorn
+pymilvus
+missingno
+simplejson
+jinja2
+polars
+sqlalchemy
+asyncmy
+gensim
+geopy
+iteration_utilities
+schedule
+pretty_errors
 thefuck
+thriftpy2
+faiss-cpu
 dataframe_image
+pandas_summary
+jmespath
 pymysql
-jinja2
-uvicorn
-pymongo
 faiss-gpu
+jieba
+pymongo
+redis-py-cluster
+cachetools
+fastapi[all]
+reportlab
+pymupd
 filetype
-schedule
-sqlalchemy
-simplejson
-geopy
-pymilvus
 
 [ann]
 pymilvus
 faiss-cpu
 
 [app]
 fastapi[all]
```

### Comparing `MeUtils-2023.7.7.15.3.6/PKG-INFO` & `MeUtils-2023.8.2.13.20.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MeUtils
-Version: 2023.7.7.15.3.6
+Version: 2023.8.2.13.20.11
 Summary: description
 Home-page: https://github.com/yuanjie-ai/MeUtils
 Author: yuanjie
 Author-email: 313303303@qq.com
 Maintainer: yuanjie
 Maintainer-email: 313303303@qq.com
 License: MIT License
```

### Comparing `MeUtils-2023.7.7.15.3.6/README.md` & `MeUtils-2023.8.2.13.20.11/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/clear_git_history.sh` & `MeUtils-2023.8.2.13.20.11/clear_git_history.sh`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/_utils.py` & `MeUtils-2023.8.2.13.20.11/meutils/_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/ai_audio/asr.py` & `MeUtils-2023.8.2.13.20.11/meutils/ai_audio/asr.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/SplitSentence.py` & `MeUtils-2023.8.2.13.20.11/meutils/ai_nlp/SplitSentence.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/Untitled-1(1).py` & `MeUtils-2023.8.2.13.20.11/meutils/ai_nlp/Untitled-1(1).py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/_lda.py` & `MeUtils-2023.8.2.13.20.11/meutils/ai_nlp/_lda.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/_textsplitter/chinese_text_splitter.py` & `MeUtils-2023.8.2.13.20.11/meutils/ai_nlp/_textsplitter/chinese_text_splitter.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/_textsplitter/text_split.py` & `MeUtils-2023.8.2.13.20.11/meutils/ai_nlp/_textsplitter/text_split.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/lda.py` & `MeUtils-2023.8.2.13.20.11/meutils/ai_nlp/lda.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/ner.py` & `MeUtils-2023.8.2.13.20.11/meutils/ai_nlp/ner.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/sentence_transformers.py` & `MeUtils-2023.8.2.13.20.11/meutils/ai_nlp/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/textsplitter.py` & `MeUtils-2023.8.2.13.20.11/meutils/ai_nlp/textsplitter.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/ai_nlp/word_segmentation.py` & `MeUtils-2023.8.2.13.20.11/meutils/ai_nlp/word_segmentation.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/ann/README.md` & `MeUtils-2023.8.2.13.20.11/meutils/ann/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/ann/README_gensim.md` & `MeUtils-2023.8.2.13.20.11/meutils/ann/README_gensim.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/ann/ann.py` & `MeUtils-2023.8.2.13.20.11/meutils/ann/ann.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/ann/ann_faiss.py` & `MeUtils-2023.8.2.13.20.11/meutils/ann/ann_faiss.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/ann/ann_gensim.py` & `MeUtils-2023.8.2.13.20.11/meutils/ann/ann_gensim.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/ann/ann_inmemory.py` & `MeUtils-2023.8.2.13.20.11/meutils/ann/ann_inmemory.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/ann/ann_service.py` & `MeUtils-2023.8.2.13.20.11/meutils/ann/ann_service.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/ann/ann_v1.py` & `MeUtils-2023.8.2.13.20.11/meutils/ann/ann_v1.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/ann/cli.py` & `MeUtils-2023.8.2.13.20.11/meutils/ann/cli.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/ann/examples/client.py` & `MeUtils-2023.8.2.13.20.11/meutils/ann/examples/client.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/ann/shake_demo.py` & `MeUtils-2023.8.2.13.20.11/meutils/ann/shake_demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/clis/cli.py` & `MeUtils-2023.8.2.13.20.11/meutils/clis/cli.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/clis/conf.py` & `MeUtils-2023.8.2.13.20.11/meutils/clis/conf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/clis/cron.py` & `MeUtils-2023.8.2.13.20.11/meutils/clis/cron.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/clis/demo.py` & `MeUtils-2023.8.2.13.20.11/meutils/clis/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/clis/gunicorn.conf.py` & `MeUtils-2023.8.2.13.20.11/meutils/clis/gunicorn.conf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/clis/monitor.py` & `MeUtils-2023.8.2.13.20.11/meutils/clis/monitor.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/clis/nesc.py` & `MeUtils-2023.8.2.13.20.11/meutils/clis/nesc.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/cmds/README.md` & `MeUtils-2023.8.2.13.20.11/meutils/cmds/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/cmds/hdfs_cmd.py` & `MeUtils-2023.8.2.13.20.11/meutils/cmds/hdfs_cmd.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/cmds/subprocess_demo.py` & `MeUtils-2023.8.2.13.20.11/meutils/cmds/subprocess_demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/coding/find132.py` & `MeUtils-2023.8.2.13.20.11/meutils/coding/find132.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/common.py` & `MeUtils-2023.8.2.13.20.11/meutils/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,69 +20,64 @@
 import zipfile
 import datetime
 import operator
 import inspect
 import textwrap
 import socket
 import warnings
+
+warnings.filterwarnings("ignore")
+
+import functools
 import argparse
 import traceback
+import threading
 import multiprocessing
 import base64
 import shutil
 import random
 import asyncio
 import importlib
 import itertools
 import pickle
 import textwrap
 import subprocess
 import wget
 import yaml
 import fire
 import typer
+import json
 import joblib
 import requests
 import wrapt
 import sklearn
 import numpy as np
 import pandas as pd
 
-if not hasattr(typing, 'Literal'):
-    import typing
-    import typing_extensions
-
-    Literal = typing_extensions.Literal
-    typing.Literal = Literal
-
 from typing import *
 from pathlib import Path
+from queue import Queue
 from pprint import pprint
 from abc import abstractmethod
 from dataclasses import dataclass
-from functools import reduce, lru_cache, cached_property, partial
+from functools import reduce, lru_cache, partial
+
 from collections import Counter, OrderedDict
 from concurrent.futures import ThreadPoolExecutor, ProcessPoolExecutor
 
 import matplotlib.pyplot as plt
 from matplotlib.font_manager import FontProperties
 
 plt.rcParams['axes.unicode_minus'] = False
 
 from loguru import logger
 # logger.remove()
 # logger.add(sys.stderr,
 #            format='<green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green> | <level>{level: <4}</level> - <level>{message}</level>')
 
-from dotenv import load_dotenv
-
-load_dotenv(
-    os.getenv('EVN', "/Users/betterme/PycharmProjects/AI/.env"),  # EVN=传入绝对路径 todo: 自定义 .env.secret
-    verbose=True
-)
 
 from tqdm.auto import tqdm
 
 tqdm.pandas()
 
 from pydantic import BaseModel, Field
 from faker import Faker  # https://www.cnblogs.com/aichixigua12/p/13236092.html
@@ -97,58 +92,70 @@
 from meutils.other.crontab import CronTab
 from meutils.other.besttable import Besttable
 
 # ME
 from meutils._utils import *
 from meutils.init.evn import *
 from meutils.init.oo import __O000OO0O0000OO00O
-from meutils.decorators import decorator, args, singleton, timer, background, background_task
 from meutils.hash_utils import murmurhash
-from meutils.path_utils import get_module_path, get_resolve_path, sys_path_append, path2list, get_config
 from meutils.cache_utils import ttl_cache, disk_cache, diskcache
+from meutils.decorators import decorator, args, singleton, timer, background, background_task
+from meutils.path_utils import get_module_path, get_resolve_path, sys_path_append, path2list, get_config
 
+lock = threading.Lock()
 __O000OO0O0000OO00O()
 
-try:
-    import orjson as json  # dumps 结果是字节型
-
-    json.dumps = partial(json.dumps, option=json.OPT_NON_STR_KEYS)
-
-
-except ImportError:
-    import json
+from dotenv import load_dotenv
 
-try:
-    from IPython.core.interactiveshell import InteractiveShell
+load_dotenvs = lambda dotenv_paths: [load_dotenv(p, verbose=True) for p in dotenv_paths]
 
-    InteractiveShell.ast_node_interactivity = "all"  # 多行输出
-except ImportError:
-    pass
-
-try:
-    from rich import print as rprint
-except ImportError:
-    pass
+load_dotenv(
+    os.getenv('EVN', "/Users/betterme/PycharmProjects/AI/.env"),  # EVN=传入绝对路径 todo: 自定义 .env.secret
+    verbose=True
+)
 
 cli = typer.Typer(name="MeUtils CLI")
-warnings.filterwarnings("ignore")
 
 # 常量
 CPU_NUM = os.cpu_count()
 FONT = FontProperties(fname=get_resolve_path('./data/SimHei.ttf', __file__))
 
 HOST_NAME = DOMAIN_NAME = LOCAL_HOST = LOCAL = HOST = PORT = ''
+
 try:
+    if not hasattr(typing, 'Literal'):
+        import typing
+        import typing_extensions
+
+        Literal = typing_extensions.Literal
+        typing.Literal = Literal
+
+    if not hasattr(functools, 'cached_property'):
+        from cached_property import cached_property
+    else:
+        from functools import cached_property
+
+    from IPython.core.interactiveshell import InteractiveShell
+
+    InteractiveShell.ast_node_interactivity = "all"  # 多行输出
+
+    from rich import print as rprint
+
     HOST_NAME = socket.gethostname()
     DOMAIN_NAME = socket.getfqdn(HOST_NAME)
 
     with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as _st:
         _st.connect(('10.255.255.255', 1))
         HOST, PORT = _st.getsockname()
-except:
+
+    # import orjson as json  # dumps 结果是字节型
+    # json.dumps = partial(json.dumps, option=json.OPT_NON_STR_KEYS)
+
+
+except ImportError:
     pass
 
 
 def _bar(current, total, width=100):
     """https://www.jb51.net/article/232232.htm"""
 
     i = int(current / total * 100)
@@ -341,20 +348,14 @@
 
     logger.debug("销毁全局变量: " + list4log(keys))
     for key in keys:
         del globals()[key]
     return keys
 
 
-def any2list(l, type=str):
-    if isinstance(l, type):
-        l = [l]
-    return l
-
-
 def show_code(func):
     sourcelines, _ = inspect.getsourcelines(func)
     _ = textwrap.dedent("".join(sourcelines))
     print(_)
     return _
 
 
@@ -377,21 +378,28 @@
     namespace = namespace or {}
     exec(source, namespace)
     namespace.pop('__builtins__')
     return namespace  # output
 
 
 def pkl_dump(obj, file):
-    with open(file, 'wb') as f:
-        return pickle.dump(obj, f)
+    with lock:
+        try:
+            with open(file, 'wb') as f:
+                return pickle.dump(obj, f)
+        except IOError:
+            return False
 
 
 def pkl_load(file):
-    with open(file, 'rb') as f:
-        return pickle.load(f)
+    try:
+        with open(file, 'rb') as f:
+            return pickle.load(f)
+    except IOError:
+        return False
 
 
 class MeBackgroundTasks(object):
     """
     def func(x):
         print(f'Sleeping: {x}')
         time.sleep(x)
@@ -403,15 +411,16 @@
     bk.add_task(func, x=3)
     """
 
     def __init__(self, max_workers=None, thread_name_prefix='🐶BackgroundTasks'):
         self.pool = ThreadPoolExecutor(max_workers, thread_name_prefix)
 
     def add_task(self, func, *args, **kwargs):
-        self.pool.submit(func, *args, **kwargs)  # pool.map(fn, *iterables, timeout=None, chunksize=1)
+        future = self.pool.submit(func, *args, **kwargs)  # pool.map(fn, *iterables, timeout=None, chunksize=1)
+        future.add_done_callback(lambda x: logger.error(future.exception()) if future.exception() else None)
 
 
 background_tasks = MeBackgroundTasks()
 
 # import uuid
 # uuid.uuid4().hex
 # attrs = [attr for attr in dir(i) if not callable(getattr(i, attr)) and not attr.startswith("__")]
```

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/comp_utils/reverse_metric.py` & `MeUtils-2023.8.2.13.20.11/meutils/comp_utils/reverse_metric.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/data/SimHei.ttf` & `MeUtils-2023.8.2.13.20.11/meutils/data/SimHei.ttf`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/data/coordinate.py` & `MeUtils-2023.8.2.13.20.11/meutils/data/coordinate.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/date_utils.py` & `MeUtils-2023.8.2.13.20.11/meutils/date_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/db/README.md` & `MeUtils-2023.8.2.13.20.11/meutils/db/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/db/__init__.py` & `MeUtils-2023.8.2.13.20.11/meutils/db/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/db/mongo.py` & `MeUtils-2023.8.2.13.20.11/meutils/db/mongo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/db/neo4j.py` & `MeUtils-2023.8.2.13.20.11/meutils/db/neo4j.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/decorators/__ai.py` & `MeUtils-2023.8.2.13.20.11/meutils/decorators/__ai.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/decorators/__init__.py` & `MeUtils-2023.8.2.13.20.11/meutils/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/decorators/catch.py` & `MeUtils-2023.8.2.13.20.11/meutils/decorators/catch.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/decorators/common.py` & `MeUtils-2023.8.2.13.20.11/meutils/decorators/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import sys
 import time
 import schedule
 import threading
 import traceback
 
 from loguru import logger
-
+from tqdm.auto import tqdm
 from concurrent.futures import ThreadPoolExecutor, ProcessPoolExecutor
 from contextlib import contextmanager
 
 # ME
 from meutils.decorators.decorator import decorator
 
 
@@ -150,55 +150,20 @@
 @decorator
 def timeout(func, seconds=1, *args, **kwargs):
     future = ThreadPoolExecutor(1).submit(func, *args, **kwargs)
     return future.result(timeout=seconds)
 
 
 @decorator
-def background_task(func, max_workers=3, *args, **kwargs):
-    """通过全局变量回收结果
-        @backend
-        def func(x):
-            import time
-            print(time.time())
-            time.sleep(3)
-            print(time.time())
-
-        @backend
-        def func():
-            global d
-            d = {}
-            while 1:
-                import time
-                time.sleep(3)
-                d['t'] = time.ctime() # 后台更新全局变量
-
-        from meutils.decorators import backend
-
-        d = {}
-        @backend
-        def task(task_id):
-            d[task_id] = time.time()
-
-        def create_task(task_id):
-            task(task_id)
-
-
-        for i in range(10):
-            create_task(i)
-
-    @param func:
-    @param args:
-    @param kwargs:
-    @return:
-    """
+def background_task(func, max_workers=1, *args, **kwargs):
     # pool.shutdown(wait=False)  # 不等待
     # pool.shutdown(wait=True)  # 等待
     pool = ThreadPoolExecutor(max_workers=max_workers, thread_name_prefix='🐶')
     future = pool.submit(func, *args, **kwargs)  # pool.map(fun4, ips)
+    future.add_done_callback(lambda x: logger.error(future.exception()) if future.exception() else None)
     return future.running()  # future.done()
 
 
 background = background_task
 
 
 # @backend
```

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/decorators/decorator.py` & `MeUtils-2023.8.2.13.20.11/meutils/decorators/decorator.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/decorators/decorator_demo.py` & `MeUtils-2023.8.2.13.20.11/meutils/decorators/decorator_demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/decorators/demo.py` & `MeUtils-2023.8.2.13.20.11/meutils/decorators/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/decorators/feishu.py` & `MeUtils-2023.8.2.13.20.11/meutils/decorators/feishu.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/decorators/scheduler.py` & `MeUtils-2023.8.2.13.20.11/meutils/decorators/scheduler.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/dist_utils.py` & `MeUtils-2023.8.2.13.20.11/meutils/dist_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/docarray_utils/demo_es.py` & `MeUtils-2023.8.2.13.20.11/meutils/docarray_utils/demo_es.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/docarray_utils/demo_hnsw.py` & `MeUtils-2023.8.2.13.20.11/meutils/docarray_utils/demo_hnsw.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/docarray_utils/in_memory.py` & `MeUtils-2023.8.2.13.20.11/meutils/docarray_utils/in_memory.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/docarray_utils/改造下hnsw.py` & `MeUtils-2023.8.2.13.20.11/meutils/docarray_utils/改造下hnsw.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/easy_search/es.py` & `MeUtils-2023.8.2.13.20.11/meutils/easy_search/es.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     def create_index(self, df: pd.DataFrame, schema, procs=4, limitmb=1024 * 2):
         self.ix = self.storage.create_index(schema, indexname=self.indexname)
         writer = self.ix.writer(procs=procs, multisegment=True, limitmb=limitmb)
         for fields in tqdm(df.to_dict(orient='records'), 'Create Index'):
             writer.add_document(**fields)
         writer.commit()
 
-    def find(self, defaultfield, querystring, limit=5, weighting=scoring.BM25F, **kwargs):
+    def find(self, querystring, defaultfield: str ='text', limit=5, weighting=scoring.BM25F, **kwargs):
         """
 
         @param defaultfield:
         @param querystring:
         @param limit:
         @param weighting: scoring.BM25F or scoring.TF_IDF()
         @param kwargs:
```

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/fileparser/PDF抽取.py` & `MeUtils-2023.8.2.13.20.11/meutils/fileparser/PDF抽取.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/hash_utils.py` & `MeUtils-2023.8.2.13.20.11/meutils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/import_utils.py` & `MeUtils-2023.8.2.13.20.11/meutils/import_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/init/evn.py` & `MeUtils-2023.8.2.13.20.11/meutils/init/evn.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 # @Software     : PyCharm
 # @Description  : 
 
 import os
 
 # 环境变量配置
 os.environ['JINA_HIDE_SURVEY'] = '1'
-os.environ["TOKENIZERS_PARALLELISM"] = "true"
-os.environ['OPEN_API_BASE'] = 'https://api.openai-proxy.com/v1'
+os.environ['TOKENIZERS_PARALLELISM'] = "true"
+os.environ['MOMENTO_AUTH_TOKEN'] = 'eyJlbmRwb2ludCI6ImNlbGwtNC11cy13ZXN0LTItMS5wcm9kLmEubW9tZW50b2hxLmNvbSIsImFwaV9rZXkiOiJleUpoYkdjaU9pSklVekkxTmlKOS5leUp6ZFdJaU9pSXpNVE16TURNek1ETkFjWEV1WTI5dElpd2lkbVZ5SWpveExDSndJam9pUTBGQlBTSjkuSVRlX01ZRnBoVTBVb1I0SkdKOU92QXZ4dUJUOHBiQnpDWWlhZjlkZFYwdyJ9'
 
 # LLM
 os.environ['LLM_ROLE'] = '你扮演的角色是ChatLLM大模型，是由Betterme开发，基于ChatLLM-1000B模型训练的。'
 os.environ['PROMPT_TEMPLATE'] = """
 {role}
 根据以下信息，简洁、专业地回答用户的问题。如果无法得到答案，请回复：“根据已知信息无法回答该问题”或“没有提供足够的信息”。请勿编造信息，答案必须使用中文。
 已知信息：
@@ -29,12 +29,13 @@
 # {role}
 # 请根据以下<>中的信息简洁、专业地回答问题。
 # 信息：<{context}>
 # 问题：{question}
 # 如果无法从中得到答案，请回答“根据已知信息无法回答该问题”或“没有提供足够的信息”。请使用中文回答，不允许添加编造内容。
 # """
 
-
+# MODELSCOPE_CACHE
+# PPNLP
 if __name__ == '__main__':
     from pprint import pprint
 
     pprint(os.environ['PROMPT_TEMPLATE'])
```

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/init/oo.py` & `MeUtils-2023.8.2.13.20.11/meutils/init/oo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/io/__init__.py` & `MeUtils-2023.8.2.13.20.11/meutils/io/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/io/image.py` & `MeUtils-2023.8.2.13.20.11/meutils/io/image.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/io/tf_io.py` & `MeUtils-2023.8.2.13.20.11/meutils/io/tf_io.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/jinja_utils.py` & `MeUtils-2023.8.2.13.20.11/meutils/jinja_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/log_utils.py` & `MeUtils-2023.8.2.13.20.11/meutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/notice/__init__.py` & `MeUtils-2023.8.2.13.20.11/meutils/notice/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/notice/emails.py` & `MeUtils-2023.8.2.13.20.11/meutils/notice/emails.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/notice/feishu.py` & `MeUtils-2023.8.2.13.20.11/meutils/notice/feishu.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/notice/file_post.py` & `MeUtils-2023.8.2.13.20.11/meutils/notice/file_post.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/notice/wechat.py` & `MeUtils-2023.8.2.13.20.11/meutils/notice/wechat.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/notice/wechat_.py` & `MeUtils-2023.8.2.13.20.11/meutils/notice/wechat_.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/notice/wecom.py` & `MeUtils-2023.8.2.13.20.11/meutils/notice/wecom.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/notice/weekmeet.py` & `MeUtils-2023.8.2.13.20.11/meutils/notice/weekmeet.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/np_utils.py` & `MeUtils-2023.8.2.13.20.11/meutils/np_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/office_automation/pdf.py` & `MeUtils-2023.8.2.13.20.11/meutils/office_automation/pdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # @Project      : MeUtils.
 # @File         : pdf
 # @Time         : 2022/6/30 下午3:41
 # @Author       : yuanjie
 # @WeChat       : meutils
 # @Software     : PyCharm
 # @Description  :
-import os
 
 from meutils.pipe import *
 
 
 def extract_text(file_or_text):
     import fitz  # pymupdf 速度更快
```

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/office_automation/pdm.py` & `MeUtils-2023.8.2.13.20.11/meutils/office_automation/pdm.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/office_automation/pdm_run.py` & `MeUtils-2023.8.2.13.20.11/meutils/office_automation/pdm_run.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/office_automation/投资管理系统O3.2_交易组.pdm` & `MeUtils-2023.8.2.13.20.11/meutils/office_automation/投资管理系统O3.2_交易组.pdm`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/__demo.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/__demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/aiomultiprocess/core.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/aiomultiprocess/core.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/aiomultiprocess/pool.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/aiomultiprocess/pool.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/aiomultiprocess/scheduler.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/aiomultiprocess/scheduler.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/aiomultiprocess/types.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/aiomultiprocess/types.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/besttable.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/besttable.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/crontab.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/crontab.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/annlite.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/annlite.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/base.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/base.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/chunk.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/chunk.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/document.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/document.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/elastic.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/elastic.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/match.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/match.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/memory.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/memory.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/milvus.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/milvus.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/__init__.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/content.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/content.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/dataloader/__init__.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/dataloader/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/dataloader/helper.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/dataloader/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/delitem.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/delitem.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/embed.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/embed.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/empty.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/empty.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/evaluation.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/evaluation.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/find.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/getattr.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/getattr.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/getitem.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/getitem.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/group.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/group.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/binary.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/io/binary.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/common.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/io/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/csv.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/io/csv.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/dataframe.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/io/dataframe.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/from_gen.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/io/from_gen.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/json.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/io/json.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/pbar.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/io/pbar.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/io/pushpull.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/io/pushpull.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/match.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/match.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/parallel.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/parallel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/plot.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/plot.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/post.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/post.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/pydantic.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/pydantic.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/reduce.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/reduce.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/sample.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/sample.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/setitem.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/setitem.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/strawberry.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/strawberry.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/text.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/text.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/mixins/traverse.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/mixins/traverse.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/opensearch.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/opensearch.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/qdrant.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/qdrant.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/queryset/lookup.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/queryset/lookup.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/queryset/parser.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/queryset/parser.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/redis.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/redis.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/sqlite.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/sqlite.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/annlite/backend.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/annlite/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/annlite/find.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/annlite/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/annlite/getsetdel.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/annlite/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/annlite/helper.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/annlite/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/annlite/seqlike.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/annlite/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/base/backend.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/base/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/base/getsetdel.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/base/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/base/helper.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/base/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/base/seqlike.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/base/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/elastic/backend.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/elastic/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/elastic/find.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/elastic/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/elastic/getsetdel.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/elastic/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/elastic/seqlike.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/elastic/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/memory/backend.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/memory/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/memory/find.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/memory/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/memory/getsetdel.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/memory/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/memory/seqlike.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/memory/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/milvus/backend.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/milvus/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/milvus/find.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/milvus/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/milvus/getsetdel.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/milvus/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/milvus/seqlike.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/milvus/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/opensearch/backend.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/opensearch/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/opensearch/find.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/opensearch/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/opensearch/getsetdel.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/opensearch/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/opensearch/seqlike.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/opensearch/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/qdrant/__init__.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/qdrant/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/qdrant/backend.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/qdrant/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/qdrant/find.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/qdrant/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/qdrant/getsetdel.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/qdrant/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/qdrant/seqlike.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/qdrant/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/redis/backend.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/redis/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/redis/find.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/redis/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/redis/getsetdel.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/redis/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/redis/seqlike.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/redis/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/sqlite/__init__.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/sqlite/backend.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/sqlite/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/sqlite/getsetdel.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/sqlite/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/sqlite/helper.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/sqlite/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/sqlite/seqlike.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/sqlite/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/weaviate/backend.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/weaviate/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/weaviate/find.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/weaviate/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/weaviate/getsetdel.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/weaviate/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/storage/weaviate/seqlike.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/storage/weaviate/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/array/weaviate.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/array/weaviate.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/base.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/base.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/dataclasses/enums.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/dataclasses/enums.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/dataclasses/getter.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/dataclasses/getter.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/dataclasses/setter.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/dataclasses/setter.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/dataclasses/types.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/dataclasses/types.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/__init__.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/data.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/data.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/generators.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/generators.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/__init__.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/_property.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/_property.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/attribute.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/attribute.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/audio.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/audio.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/blob.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/blob.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/content.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/content.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/convert.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/convert.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/dump.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/dump.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/featurehash.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/featurehash.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/helper.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/image.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/image.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/mesh.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/mesh.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/multimodal.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/multimodal.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/plot.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/plot.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/porting.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/porting.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/property.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/property.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/protobuf.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/protobuf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/pydantic.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/pydantic.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/rich_embedding.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/rich_embedding.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/strawberry.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/strawberry.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/sugar.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/sugar.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/text.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/text.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/mixins/video.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/mixins/video.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/pydantic_model.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/pydantic_model.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/document/strawberry_type.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/document/strawberry_type.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/helper.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/distance/__init__.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/math/distance/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/distance/numpy.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/math/distance/numpy.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/distance/paddle.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/math/distance/paddle.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/distance/tensorflow.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/math/distance/tensorflow.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/distance/torch.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/math/distance/torch.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/evaluation.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/math/evaluation.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/helper.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/math/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/math/ndarray.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/math/ndarray.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/proto/io/__init__.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/proto/io/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/proto/io/ndarray.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/proto/io/ndarray.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/proto/pb/docarray_pb2.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/proto/pb/docarray_pb2.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/proto/pb2/docarray_pb2.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/proto/pb2/docarray_pb2.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/resources/ci-vendors.json` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/resources/ci-vendors.json`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/resources/embedding-projector/index.html.gz` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/resources/embedding-projector/index.html.gz`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/score/data.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/score/data.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/score/mixins/property.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/score/mixins/property.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/other/docarray/typing/__init__.py` & `MeUtils-2023.8.2.13.20.11/meutils/other/docarray/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/pandas_utils/opt.py` & `MeUtils-2023.8.2.13.20.11/meutils/pandas_utils/opt.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/pandas_utils/pd_utils.py` & `MeUtils-2023.8.2.13.20.11/meutils/pandas_utils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/path_utils.py` & `MeUtils-2023.8.2.13.20.11/meutils/path_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/pd_utils.py` & `MeUtils-2023.8.2.13.20.11/meutils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/pipe.py` & `MeUtils-2023.8.2.13.20.11/meutils/pipe.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 # @File         : pipe_utils
 # @Time         : 2020/11/12 11:35 上午
 # @Author       : yuanjie
 # @Email        : meutils@qq.com
 # @Software     : PyCharm
 # @Description  : 
 
-import functools
-
 from meutils.common import *
 
 
 class Pipe(object):
     """I am very like a linux pipe"""
 
     def __init__(self, function):
@@ -59,15 +57,15 @@
 xdrop_ = Pipe(lambda iterable, func=None: list(itertools.dropwhile(func, iterable)))
 
 # itertools: https://blog.csdn.net/weixin_43193719/article/details/87536371
 xchain = Pipe(lambda iterable: itertools.chain(*iterable))
 xchain_ = Pipe(lambda iterable: list(itertools.chain(*iterable)))
 
 xenumerate = Pipe(lambda iterable, start=0: enumerate(iterable, start))
-xenumerate_ = Pipe(lambda iterable, start=0: enumerate(iterable, start))
+xenumerate_ = Pipe(lambda iterable, start=0: list(enumerate(iterable, start)))
 
 xshuffle = Pipe(lambda l, n_samples=None: sklearn.utils.shuffle(l, n_samples=n_samples))
 
 # dateframe dfs
 """多个df: 
 dfs = (
     Path('.').glob('demo*.txt') | xmap(lambda p: pd.read_csv(p, chunksize=2, names=['id'])) | xchain
@@ -133,14 +131,44 @@
     if keep_order:
         return list(OrderedDict.fromkeys(iterable))  # 移除列表中的重复元素(保持有序)
     else:
         return list(set(iterable))
 
 
 @Pipe
+def xUnique_plus(iterable, key_fn: Callable = None):
+    from joblib.hashing import hash
+    hash_dict = {}
+
+    for element in iterable:
+        if key_fn:
+            key = key_fn(element)
+        else:
+            key = element
+        hash_dict[hash(key)] = element
+    return list(hash_dict.values())
+
+
+@Pipe
+def xBloomFilter(iterable, bloom=None):
+    """
+        def bloom_add(iterable):
+        bloom = pkl_load('bloom')
+        for i in iterable:
+            bloom.add(i)
+        pkl_dump(bloom, 'bloom')
+    """
+    from pybloom_live import ScalableBloomFilter, BloomFilter
+    bloom = bloom or ScalableBloomFilter(10 ** 6)
+    for i in iterable:
+        bloom.add(i)
+    return bloom
+
+
+@Pipe
 def xbar4iter(iterable: list, func, batch_size=1, show_bar=True) -> list:
     """func 入参出参都是 list"""
     l = []
     _ = iterable | xgroup(batch_size)
     if show_bar: _ = tqdm(_)
     for i in _:
         l += func(i)
@@ -179,48 +207,49 @@
     """hash分组"""
     dic = {}
     for v in ls:
         dic.setdefault(murmurhash(v, bins=bins), []).append(v)
     return list(dic.values())
 
 
-# multiple
 @Pipe
 def xJobs(iterable, func, n_jobs=3):
     """支持匿名函数"""
     if n_jobs > 1:
         delayed_function = joblib.delayed(func)
         return joblib.Parallel(n_jobs=n_jobs)(delayed_function(arg) for arg in iterable)
         # yield from joblib.Parallel(n_jobs=n_jobs)(delayed_function(arg) for arg in iterable)
     else:
         return list(map(func, iterable))
 
 
 @Pipe
-def xThreadPoolExecutor(iterable, func, max_workers=5):
-    """
-    with ThreadPoolExecutor(max_workers) as pool:
-        pool.map(func, iterable)
-    """
+def xThreadPoolExecutor(iterable, func, max_workers=5, desc="Processing", unit="it"):
     if max_workers > 1:
-        with ThreadPoolExecutor(max_workers) as pool:
-            return pool.map(func, iterable)
+        total = len(iterable) if hasattr(iterable, '__len__') else None
+
+        with ThreadPoolExecutor(max_workers) as pool, tqdm(total=total, desc=desc, unit=unit) as pbar:
+            for i in pool.map(func, iterable):
+                yield i
+                pbar.update()
+
     else:
         return map(func, iterable)
 
 
 @Pipe
-def xProcessPoolExecutor(iterable, func, max_workers=5):
-    """
-    with ProcessPoolExecutor(max_workers) as pool:
-        pool.map(func, iterable)
-    """
+def xProcessPoolExecutor(iterable, func, max_workers=5, desc="Processing", unit="it"):
     if max_workers > 1:
-        with ProcessPoolExecutor(max_workers) as pool:
-            return pool.map(func, iterable)
+        total = len(iterable) if hasattr(iterable, '__len__') else None
+
+        with ProcessPoolExecutor(max_workers) as pool, tqdm(total=total, desc=desc, unit=unit) as pbar:
+            for i in pool.map(func, iterable):
+                yield i
+                pbar.update()
+
     else:
         return map(func, iterable)
 
 
 @Pipe
 def xDictValues(keys, dic: dict, default=None):
     return tuple(dic.get(k, default) for k in keys)
@@ -251,15 +280,14 @@
 
     """
     loop = asyncio.get_event_loop()
     _ = asyncio.gather(*tasks, return_exceptions=return_exceptions)  # asyncio.wait(tasks)
     return loop.run_until_complete(_)
 
 
-
 if __name__ == '__main__':
     @Pipe
     def xfunc1(x):
         _ = x.split()
         print(_)
         return _
```

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/plot_utils/demo.py` & `MeUtils-2023.8.2.13.20.11/meutils/plot_utils/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/plot_utils/echarts.py` & `MeUtils-2023.8.2.13.20.11/meutils/plot_utils/echarts.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/plot_utils/embedding_plot.py` & `MeUtils-2023.8.2.13.20.11/meutils/plot_utils/embedding_plot.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/plot_utils/mecharts.py` & `MeUtils-2023.8.2.13.20.11/meutils/plot_utils/mecharts.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/plot_utils/metrics.py` & `MeUtils-2023.8.2.13.20.11/meutils/plot_utils/metrics.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/plot_utils/plot_utils.py` & `MeUtils-2023.8.2.13.20.11/meutils/plot_utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/request_utils/__init__.py` & `MeUtils-2023.8.2.13.20.11/meutils/request_utils/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,14 +28,34 @@
         'User-Agent': 'Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) '
                       'Chrome/63.0.3239.132 Safari/537.36 QIHU 360SE '
     }
     r = requests.request(method, url, **{**_kwargs, **kwargs})
     r.encoding = encoding if encoding else r.apparent_encoding
 
     return r.json() if return_json else r
+# def _create_retry_decorator(embeddings: OpenAIEmbeddings) -> Callable[[Any], Any]:
+#     import openai
+#
+#     min_seconds = 4
+#     max_seconds = 10
+#     # Wait 2^x * 1 second between each retry starting with
+#     # 4 seconds, then up to 10 seconds, then 10 seconds afterwards
+#     return retry(
+#         reraise=True,
+#         stop=stop_after_attempt(embeddings.max_retries),
+#         wait=wait_exponential(multiplier=1, min=min_seconds, max=max_seconds),
+#         retry=(
+#             retry_if_exception_type(openai.error.Timeout)
+#             | retry_if_exception_type(openai.error.APIError)
+#             | retry_if_exception_type(openai.error.APIConnectionError)
+#             | retry_if_exception_type(openai.error.RateLimitError)
+#             | retry_if_exception_type(openai.error.ServiceUnavailableError)
+#         ),
+#         before_sleep=before_sleep_log(logger, logging.WARNING),
+#     )
 
 
 @retry(wait=wait_fixed(3),  # 重试之前等待3秒
        stop=stop_after_delay(7) | stop_after_attempt(3),  # 同时满足用 | 没毛病：重试7秒重试3次
        retry_error_callback=lambda log: logger.error(log),
        reraise=True)
 def request(url=None, json=None, parser=lambda x: x, encoding=None, **kwargs):
```

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/request_utils/crawler.py` & `MeUtils-2023.8.2.13.20.11/meutils/request_utils/crawler.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/request_utils/download.py` & `MeUtils-2023.8.2.13.20.11/meutils/request_utils/download.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/request_utils/results.py` & `MeUtils-2023.8.2.13.20.11/meutils/request_utils/results.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/request_utils/公网ip.py` & `MeUtils-2023.8.2.13.20.11/meutils/request_utils/公网ip.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/serving/_fastapi.py` & `MeUtils-2023.8.2.13.20.11/meutils/serving/_fastapi.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/serving/fastapi/__demo/异步任务.py` & `MeUtils-2023.8.2.13.20.11/meutils/serving/fastapi/__demo/异步任务.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/serving/fastapi/common.py` & `MeUtils-2023.8.2.13.20.11/meutils/serving/fastapi/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 from fastapi import FastAPI, APIRouter
 from fastapi.exceptions import RequestValidationError, HTTPException
 from starlette.middleware.cors import CORSMiddleware
 
 from meutils.serving.fastapi.errors.http_error import http_error_handler
 from meutils.serving.fastapi.errors.validation_error import http422_error_handler
 
-router = APIRouter()
-
 
 class App(FastAPI):
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
         self.add_middleware(
@@ -30,16 +28,16 @@
             allow_credentials=True,
             allow_methods=['*'],
             allow_headers=['*'],
         )
         self.add_exception_handler(HTTPException, http_error_handler)
         self.add_exception_handler(RequestValidationError, http422_error_handler)
 
-    def include_router(self, router, **kwargs):
-        self.router.include_router(router, **kwargs)  # prefix=''
+    def include_router(self, router, prefix='', **kwargs):
+        super().include_router(router, prefix=prefix, **kwargs)
 
     def run(self, app=None, host="0.0.0.0", port=8000, workers=1, access_log=True, reload=False, **kwargs):
         """
 
         :param app:   app字符串可开启热更新 reload
         :param host:
         :param port:
```

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/serving/fastapi/errors/validation_error.py` & `MeUtils-2023.8.2.13.20.11/meutils/serving/fastapi/errors/validation_error.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/serving/gui/bar.py` & `MeUtils-2023.8.2.13.20.11/meutils/serving/gui/bar.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/serving/gui/demo.py` & `MeUtils-2023.8.2.13.20.11/meutils/serving/gui/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/serving/jina/__demo/client.py` & `MeUtils-2023.8.2.13.20.11/meutils/serving/jina/__demo/client.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/serving/jina/__demo/flow.svg` & `MeUtils-2023.8.2.13.20.11/meutils/serving/jina/__demo/flow.svg`

 * *Files 6% similar despite different names*

```diff
@@ -60,795 +60,820 @@
 000003b0: 6d73 222c 7665 7264 616e 612c 6172 6961  ms",verdana,aria
 000003c0: 6c2c 7361 6e73 2d73 6572 6966 3b63 6f6c  l,sans-serif;col
 000003d0: 6f72 3a23 3333 333b 7d23 6d65 726d 6169  or:#333;}#mermai
 000003e0: 642d 7376 6720 2e63 6c75 7374 6572 2d6c  d-svg .cluster-l
 000003f0: 6162 656c 2074 6578 747b 6669 6c6c 3a72  abel text{fill:r
 00000400: 6762 2830 2c20 302c 2030 293b 7d23 6d65  gb(0, 0, 0);}#me
 00000410: 726d 6169 642d 7376 6720 2e63 6c75 7374  rmaid-svg .clust
-00000420: 6572 2d6c 6162 656c 2073 7061 6e7b 636f  er-label span{co
-00000430: 6c6f 723a 7267 6228 302c 2030 2c20 3029  lor:rgb(0, 0, 0)
-00000440: 3b7d 236d 6572 6d61 6964 2d73 7667 202e  ;}#mermaid-svg .
-00000450: 6c61 6265 6c20 7465 7874 2c23 6d65 726d  label text,#merm
-00000460: 6169 642d 7376 6720 7370 616e 7b66 696c  aid-svg span{fil
-00000470: 6c3a 2333 3333 3b63 6f6c 6f72 3a23 3333  l:#333;color:#33
-00000480: 333b 7d23 6d65 726d 6169 642d 7376 6720  3;}#mermaid-svg 
-00000490: 2e6e 6f64 6520 7265 6374 2c23 6d65 726d  .node rect,#merm
-000004a0: 6169 642d 7376 6720 2e6e 6f64 6520 6369  aid-svg .node ci
-000004b0: 7263 6c65 2c23 6d65 726d 6169 642d 7376  rcle,#mermaid-sv
-000004c0: 6720 2e6e 6f64 6520 656c 6c69 7073 652c  g .node ellipse,
-000004d0: 236d 6572 6d61 6964 2d73 7667 202e 6e6f  #mermaid-svg .no
-000004e0: 6465 2070 6f6c 7967 6f6e 2c23 6d65 726d  de polygon,#merm
-000004f0: 6169 642d 7376 6720 2e6e 6f64 6520 7061  aid-svg .node pa
-00000500: 7468 7b66 696c 6c3a 2333 3243 3843 443b  th{fill:#32C8CD;
-00000510: 7374 726f 6b65 3a23 6666 663b 7374 726f  stroke:#fff;stro
-00000520: 6b65 2d77 6964 7468 3a31 7078 3b7d 236d  ke-width:1px;}#m
-00000530: 6572 6d61 6964 2d73 7667 202e 6e6f 6465  ermaid-svg .node
-00000540: 202e 6c61 6265 6c7b 7465 7874 2d61 6c69   .label{text-ali
-00000550: 676e 3a63 656e 7465 723b 7d23 6d65 726d  gn:center;}#merm
-00000560: 6169 642d 7376 6720 2e6e 6f64 652e 636c  aid-svg .node.cl
-00000570: 6963 6b61 626c 657b 6375 7273 6f72 3a70  ickable{cursor:p
-00000580: 6f69 6e74 6572 3b7d 236d 6572 6d61 6964  ointer;}#mermaid
-00000590: 2d73 7667 202e 6172 726f 7768 6561 6450  -svg .arrowheadP
-000005a0: 6174 687b 6669 6c6c 3a75 6e64 6566 696e  ath{fill:undefin
-000005b0: 6564 3b7d 236d 6572 6d61 6964 2d73 7667  ed;}#mermaid-svg
-000005c0: 202e 6564 6765 5061 7468 202e 7061 7468   .edgePath .path
-000005d0: 7b73 7472 6f6b 653a 2361 3664 3864 613b  {stroke:#a6d8da;
-000005e0: 7374 726f 6b65 2d77 6964 7468 3a32 2e30  stroke-width:2.0
-000005f0: 7078 3b7d 236d 6572 6d61 6964 2d73 7667  px;}#mermaid-svg
-00000600: 202e 666c 6f77 6368 6172 742d 6c69 6e6b   .flowchart-link
-00000610: 7b73 7472 6f6b 653a 2361 3664 3864 613b  {stroke:#a6d8da;
-00000620: 6669 6c6c 3a6e 6f6e 653b 7d23 6d65 726d  fill:none;}#merm
-00000630: 6169 642d 7376 6720 2e65 6467 654c 6162  aid-svg .edgeLab
-00000640: 656c 7b62 6163 6b67 726f 756e 642d 636f  el{background-co
-00000650: 6c6f 723a 6873 6c28 2d31 3230 2c20 3025  lor:hsl(-120, 0%
-00000660: 2c20 3130 3025 293b 7465 7874 2d61 6c69  , 100%);text-ali
-00000670: 676e 3a63 656e 7465 723b 7d23 6d65 726d  gn:center;}#merm
-00000680: 6169 642d 7376 6720 2e65 6467 654c 6162  aid-svg .edgeLab
-00000690: 656c 2072 6563 747b 6f70 6163 6974 793a  el rect{opacity:
-000006a0: 302e 353b 6261 636b 6772 6f75 6e64 2d63  0.5;background-c
-000006b0: 6f6c 6f72 3a68 736c 282d 3132 302c 2030  olor:hsl(-120, 0
-000006c0: 252c 2031 3030 2529 3b66 696c 6c3a 6873  %, 100%);fill:hs
-000006d0: 6c28 2d31 3230 2c20 3025 2c20 3130 3025  l(-120, 0%, 100%
-000006e0: 293b 7d23 6d65 726d 6169 642d 7376 6720  );}#mermaid-svg 
-000006f0: 2e63 6c75 7374 6572 2072 6563 747b 6669  .cluster rect{fi
-00000700: 6c6c 3a23 4545 4544 4537 3843 3b73 7472  ll:#EEEDE78C;str
-00000710: 6f6b 653a 6e6f 6e65 3b73 7472 6f6b 652d  oke:none;stroke-
-00000720: 7769 6474 683a 3170 783b 7d23 6d65 726d  width:1px;}#merm
-00000730: 6169 642d 7376 6720 2e63 6c75 7374 6572  aid-svg .cluster
-00000740: 2074 6578 747b 6669 6c6c 3a72 6762 2830   text{fill:rgb(0
-00000750: 2c20 302c 2030 293b 7d23 6d65 726d 6169  , 0, 0);}#mermai
-00000760: 642d 7376 6720 2e63 6c75 7374 6572 2073  d-svg .cluster s
-00000770: 7061 6e7b 636f 6c6f 723a 7267 6228 302c  pan{color:rgb(0,
-00000780: 2030 2c20 3029 3b7d 236d 6572 6d61 6964   0, 0);}#mermaid
-00000790: 2d73 7667 2064 6976 2e6d 6572 6d61 6964  -svg div.mermaid
-000007a0: 546f 6f6c 7469 707b 706f 7369 7469 6f6e  Tooltip{position
-000007b0: 3a61 6273 6f6c 7574 653b 7465 7874 2d61  :absolute;text-a
-000007c0: 6c69 676e 3a63 656e 7465 723b 6d61 782d  lign:center;max-
-000007d0: 7769 6474 683a 3230 3070 783b 7061 6464  width:200px;padd
-000007e0: 696e 673a 3270 783b 666f 6e74 2d66 616d  ing:2px;font-fam
-000007f0: 696c 793a 2274 7265 6275 6368 6574 206d  ily:"trebuchet m
-00000800: 7322 2c76 6572 6461 6e61 2c61 7269 616c  s",verdana,arial
-00000810: 2c73 616e 732d 7365 7269 663b 666f 6e74  ,sans-serif;font
-00000820: 2d73 697a 653a 3132 7078 3b62 6163 6b67  -size:12px;backg
-00000830: 726f 756e 643a 6873 6c28 3138 302c 2030  round:hsl(180, 0
-00000840: 252c 2031 3030 2529 3b62 6f72 6465 723a  %, 100%);border:
-00000850: 3170 7820 736f 6c69 6420 756e 6465 6669  1px solid undefi
-00000860: 6e65 643b 626f 7264 6572 2d72 6164 6975  ned;border-radiu
-00000870: 733a 3270 783b 706f 696e 7465 722d 6576  s:2px;pointer-ev
-00000880: 656e 7473 3a6e 6f6e 653b 7a2d 696e 6465  ents:none;z-inde
-00000890: 783a 3130 303b 7d23 6d65 726d 6169 642d  x:100;}#mermaid-
-000008a0: 7376 6720 2e66 6c6f 7763 6861 7274 5469  svg .flowchartTi
-000008b0: 746c 6554 6578 747b 7465 7874 2d61 6e63  tleText{text-anc
-000008c0: 686f 723a 6d69 6464 6c65 3b66 6f6e 742d  hor:middle;font-
-000008d0: 7369 7a65 3a31 3870 783b 6669 6c6c 3a23  size:18px;fill:#
-000008e0: 3333 333b 7d23 6d65 726d 6169 642d 7376  333;}#mermaid-sv
-000008f0: 6720 3a72 6f6f 747b 2d2d 6d65 726d 6169  g :root{--mermai
-00000900: 642d 666f 6e74 2d66 616d 696c 793a 2274  d-font-family:"t
-00000910: 7265 6275 6368 6574 206d 7322 2c76 6572  rebuchet ms",ver
-00000920: 6461 6e61 2c61 7269 616c 2c73 616e 732d  dana,arial,sans-
-00000930: 7365 7269 663b 7d23 6d65 726d 6169 642d  serif;}#mermaid-
-00000940: 7376 6720 2e49 4e53 5045 4354 2667 743b  svg .INSPECT&gt;
-00000950: 2a7b 7374 726f 6b65 3a23 4632 3943 3946  *{stroke:#F29C9F
-00000960: 2169 6d70 6f72 7461 6e74 3b7d 236d 6572  !important;}#mer
-00000970: 6d61 6964 2d73 7667 202e 494e 5350 4543  maid-svg .INSPEC
-00000980: 5420 7370 616e 7b73 7472 6f6b 653a 2346  T span{stroke:#F
-00000990: 3239 4339 4621 696d 706f 7274 616e 743b  29C9F!important;
-000009a0: 7d23 6d65 726d 6169 642d 7376 6720 2e4a  }#mermaid-svg .J
-000009b0: 4f49 4e5f 494e 5350 4543 5426 6774 3b2a  OIN_INSPECT&gt;*
-000009c0: 7b73 7472 6f6b 653a 2346 3239 4339 4621  {stroke:#F29C9F!
-000009d0: 696d 706f 7274 616e 743b 7d23 6d65 726d  important;}#merm
-000009e0: 6169 642d 7376 6720 2e4a 4f49 4e5f 494e  aid-svg .JOIN_IN
-000009f0: 5350 4543 5420 7370 616e 7b73 7472 6f6b  SPECT span{strok
-00000a00: 653a 2346 3239 4339 4621 696d 706f 7274  e:#F29C9F!import
-00000a10: 616e 743b 7d23 6d65 726d 6169 642d 7376  ant;}#mermaid-sv
-00000a20: 6720 2e47 4154 4557 4159 2667 743b 2a7b  g .GATEWAY&gt;*{
-00000a30: 6669 6c6c 3a6e 6f6e 6521 696d 706f 7274  fill:none!import
-00000a40: 616e 743b 636f 6c6f 723a 2330 3030 2169  ant;color:#000!i
-00000a50: 6d70 6f72 7461 6e74 3b73 7472 6f6b 653a  mportant;stroke:
-00000a60: 6e6f 6e65 2169 6d70 6f72 7461 6e74 3b7d  none!important;}
-00000a70: 236d 6572 6d61 6964 2d73 7667 202e 4741  #mermaid-svg .GA
-00000a80: 5445 5741 5920 7370 616e 7b66 696c 6c3a  TEWAY span{fill:
-00000a90: 6e6f 6e65 2169 6d70 6f72 7461 6e74 3b63  none!important;c
-00000aa0: 6f6c 6f72 3a23 3030 3021 696d 706f 7274  olor:#000!import
-00000ab0: 616e 743b 7374 726f 6b65 3a6e 6f6e 6521  ant;stroke:none!
-00000ac0: 696d 706f 7274 616e 743b 7d23 6d65 726d  important;}#merm
-00000ad0: 6169 642d 7376 6720 2e47 4154 4557 4159  aid-svg .GATEWAY
-00000ae0: 2074 7370 616e 7b66 696c 6c3a 2330 3030   tspan{fill:#000
-00000af0: 2169 6d70 6f72 7461 6e74 3b7d 236d 6572  !important;}#mer
-00000b00: 6d61 6964 2d73 7667 202e 494e 5350 4543  maid-svg .INSPEC
-00000b10: 545f 4155 585f 5041 5353 2667 743b 2a7b  T_AUX_PASS&gt;*{
-00000b20: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
-00000b30: 3a32 2032 2169 6d70 6f72 7461 6e74 3b7d  :2 2!important;}
-00000b40: 236d 6572 6d61 6964 2d73 7667 202e 494e  #mermaid-svg .IN
-00000b50: 5350 4543 545f 4155 585f 5041 5353 2073  SPECT_AUX_PASS s
-00000b60: 7061 6e7b 7374 726f 6b65 2d64 6173 6861  pan{stroke-dasha
-00000b70: 7272 6179 3a32 2032 2169 6d70 6f72 7461  rray:2 2!importa
-00000b80: 6e74 3b7d 236d 6572 6d61 6964 2d73 7667  nt;}#mermaid-svg
-00000b90: 202e 4845 4144 5441 494c 2667 743b 2a7b   .HEADTAIL&gt;*{
-00000ba0: 6669 6c6c 3a23 3332 4338 4344 3144 2169  fill:#32C8CD1D!i
-00000bb0: 6d70 6f72 7461 6e74 3b7d 236d 6572 6d61  mportant;}#merma
-00000bc0: 6964 2d73 7667 202e 4845 4144 5441 494c  id-svg .HEADTAIL
-00000bd0: 2073 7061 6e7b 6669 6c6c 3a23 3332 4338   span{fill:#32C8
-00000be0: 4344 3144 2169 6d70 6f72 7461 6e74 3b7d  CD1D!important;}
-00000bf0: 236d 6572 6d61 6964 2d73 7667 202e 4558  #mermaid-svg .EX
-00000c00: 5445 524e 414c 2667 743b 2a7b 6669 6c6c  TERNAL&gt;*{fill
-00000c10: 3a23 6666 6621 696d 706f 7274 616e 743b  :#fff!important;
-00000c20: 7374 726f 6b65 3a23 3332 4338 4344 2169  stroke:#32C8CD!i
-00000c30: 6d70 6f72 7461 6e74 3b7d 236d 6572 6d61  mportant;}#merma
-00000c40: 6964 2d73 7667 202e 4558 5445 524e 414c  id-svg .EXTERNAL
-00000c50: 2073 7061 6e7b 6669 6c6c 3a23 6666 6621   span{fill:#fff!
-00000c60: 696d 706f 7274 616e 743b 7374 726f 6b65  important;stroke
-00000c70: 3a23 3332 4338 4344 2169 6d70 6f72 7461  :#32C8CD!importa
-00000c80: 6e74 3b7d 3c2f 7374 796c 653e 3c67 3e3c  nt;}</style><g><
-00000c90: 6d61 726b 6572 2069 643d 2266 6c6f 7763  marker id="flowc
-00000ca0: 6861 7274 2d70 6f69 6e74 456e 6422 2063  hart-pointEnd" c
-00000cb0: 6c61 7373 3d22 6d61 726b 6572 2066 6c6f  lass="marker flo
-00000cc0: 7763 6861 7274 2220 7669 6577 426f 783d  wchart" viewBox=
-00000cd0: 2230 2030 2031 3220 3230 2220 7265 6658  "0 0 12 20" refX
-00000ce0: 3d22 3130 2220 7265 6659 3d22 3522 206d  ="10" refY="5" m
-00000cf0: 6172 6b65 7255 6e69 7473 3d22 7573 6572  arkerUnits="user
-00000d00: 5370 6163 654f 6e55 7365 2220 6d61 726b  SpaceOnUse" mark
-00000d10: 6572 5769 6474 683d 2231 3222 206d 6172  erWidth="12" mar
-00000d20: 6b65 7248 6569 6768 743d 2231 3222 206f  kerHeight="12" o
-00000d30: 7269 656e 743d 2261 7574 6f22 3e3c 7061  rient="auto"><pa
-00000d40: 7468 2064 3d22 4d20 3020 3020 4c20 3130  th d="M 0 0 L 10
-00000d50: 2035 204c 2030 2031 3020 7a22 2063 6c61   5 L 0 10 z" cla
-00000d60: 7373 3d22 6172 726f 774d 6172 6b65 7250  ss="arrowMarkerP
-00000d70: 6174 6822 2073 7479 6c65 3d22 7374 726f  ath" style="stro
-00000d80: 6b65 2d77 6964 7468 3a20 313b 2073 7472  ke-width: 1; str
-00000d90: 6f6b 652d 6461 7368 6172 7261 793a 2031  oke-dasharray: 1
-00000da0: 2c20 303b 223e 3c2f 7061 7468 3e3c 2f6d  , 0;"></path></m
-00000db0: 6172 6b65 723e 3c6d 6172 6b65 7220 6964  arker><marker id
-00000dc0: 3d22 666c 6f77 6368 6172 742d 706f 696e  ="flowchart-poin
-00000dd0: 7453 7461 7274 2220 636c 6173 733d 226d  tStart" class="m
-00000de0: 6172 6b65 7220 666c 6f77 6368 6172 7422  arker flowchart"
-00000df0: 2076 6965 7742 6f78 3d22 3020 3020 3130   viewBox="0 0 10
-00000e00: 2031 3022 2072 6566 583d 2230 2220 7265   10" refX="0" re
-00000e10: 6659 3d22 3522 206d 6172 6b65 7255 6e69  fY="5" markerUni
-00000e20: 7473 3d22 7573 6572 5370 6163 654f 6e55  ts="userSpaceOnU
-00000e30: 7365 2220 6d61 726b 6572 5769 6474 683d  se" markerWidth=
-00000e40: 2231 3222 206d 6172 6b65 7248 6569 6768  "12" markerHeigh
-00000e50: 743d 2231 3222 206f 7269 656e 743d 2261  t="12" orient="a
-00000e60: 7574 6f22 3e3c 7061 7468 2064 3d22 4d20  uto"><path d="M 
-00000e70: 3020 3520 4c20 3130 2031 3020 4c20 3130  0 5 L 10 10 L 10
-00000e80: 2030 207a 2220 636c 6173 733d 2261 7272   0 z" class="arr
-00000e90: 6f77 4d61 726b 6572 5061 7468 2220 7374  owMarkerPath" st
-00000ea0: 796c 653d 2273 7472 6f6b 652d 7769 6474  yle="stroke-widt
-00000eb0: 683a 2031 3b20 7374 726f 6b65 2d64 6173  h: 1; stroke-das
-00000ec0: 6861 7272 6179 3a20 312c 2030 3b22 3e3c  harray: 1, 0;"><
-00000ed0: 2f70 6174 683e 3c2f 6d61 726b 6572 3e3c  /path></marker><
-00000ee0: 6d61 726b 6572 2069 643d 2266 6c6f 7763  marker id="flowc
-00000ef0: 6861 7274 2d63 6972 636c 6545 6e64 2220  hart-circleEnd" 
-00000f00: 636c 6173 733d 226d 6172 6b65 7220 666c  class="marker fl
-00000f10: 6f77 6368 6172 7422 2076 6965 7742 6f78  owchart" viewBox
-00000f20: 3d22 3020 3020 3130 2031 3022 2072 6566  ="0 0 10 10" ref
-00000f30: 583d 2231 3122 2072 6566 593d 2235 2220  X="11" refY="5" 
-00000f40: 6d61 726b 6572 556e 6974 733d 2275 7365  markerUnits="use
-00000f50: 7253 7061 6365 4f6e 5573 6522 206d 6172  rSpaceOnUse" mar
-00000f60: 6b65 7257 6964 7468 3d22 3131 2220 6d61  kerWidth="11" ma
-00000f70: 726b 6572 4865 6967 6874 3d22 3131 2220  rkerHeight="11" 
-00000f80: 6f72 6965 6e74 3d22 6175 746f 223e 3c63  orient="auto"><c
-00000f90: 6972 636c 6520 6378 3d22 3522 2063 793d  ircle cx="5" cy=
-00000fa0: 2235 2220 723d 2235 2220 636c 6173 733d  "5" r="5" class=
-00000fb0: 2261 7272 6f77 4d61 726b 6572 5061 7468  "arrowMarkerPath
-00000fc0: 2220 7374 796c 653d 2273 7472 6f6b 652d  " style="stroke-
-00000fd0: 7769 6474 683a 2031 3b20 7374 726f 6b65  width: 1; stroke
-00000fe0: 2d64 6173 6861 7272 6179 3a20 312c 2030  -dasharray: 1, 0
-00000ff0: 3b22 3e3c 2f63 6972 636c 653e 3c2f 6d61  ;"></circle></ma
-00001000: 726b 6572 3e3c 6d61 726b 6572 2069 643d  rker><marker id=
-00001010: 2266 6c6f 7763 6861 7274 2d63 6972 636c  "flowchart-circl
-00001020: 6553 7461 7274 2220 636c 6173 733d 226d  eStart" class="m
-00001030: 6172 6b65 7220 666c 6f77 6368 6172 7422  arker flowchart"
-00001040: 2076 6965 7742 6f78 3d22 3020 3020 3130   viewBox="0 0 10
-00001050: 2031 3022 2072 6566 583d 222d 3122 2072   10" refX="-1" r
-00001060: 6566 593d 2235 2220 6d61 726b 6572 556e  efY="5" markerUn
-00001070: 6974 733d 2275 7365 7253 7061 6365 4f6e  its="userSpaceOn
-00001080: 5573 6522 206d 6172 6b65 7257 6964 7468  Use" markerWidth
-00001090: 3d22 3131 2220 6d61 726b 6572 4865 6967  ="11" markerHeig
-000010a0: 6874 3d22 3131 2220 6f72 6965 6e74 3d22  ht="11" orient="
-000010b0: 6175 746f 223e 3c63 6972 636c 6520 6378  auto"><circle cx
-000010c0: 3d22 3522 2063 793d 2235 2220 723d 2235  ="5" cy="5" r="5
-000010d0: 2220 636c 6173 733d 2261 7272 6f77 4d61  " class="arrowMa
-000010e0: 726b 6572 5061 7468 2220 7374 796c 653d  rkerPath" style=
-000010f0: 2273 7472 6f6b 652d 7769 6474 683a 2031  "stroke-width: 1
-00001100: 3b20 7374 726f 6b65 2d64 6173 6861 7272  ; stroke-dasharr
-00001110: 6179 3a20 312c 2030 3b22 3e3c 2f63 6972  ay: 1, 0;"></cir
-00001120: 636c 653e 3c2f 6d61 726b 6572 3e3c 6d61  cle></marker><ma
-00001130: 726b 6572 2069 643d 2266 6c6f 7763 6861  rker id="flowcha
-00001140: 7274 2d63 726f 7373 456e 6422 2063 6c61  rt-crossEnd" cla
-00001150: 7373 3d22 6d61 726b 6572 2063 726f 7373  ss="marker cross
-00001160: 2066 6c6f 7763 6861 7274 2220 7669 6577   flowchart" view
-00001170: 426f 783d 2230 2030 2031 3120 3131 2220  Box="0 0 11 11" 
-00001180: 7265 6658 3d22 3132 2220 7265 6659 3d22  refX="12" refY="
-00001190: 352e 3222 206d 6172 6b65 7255 6e69 7473  5.2" markerUnits
-000011a0: 3d22 7573 6572 5370 6163 654f 6e55 7365  ="userSpaceOnUse
-000011b0: 2220 6d61 726b 6572 5769 6474 683d 2231  " markerWidth="1
-000011c0: 3122 206d 6172 6b65 7248 6569 6768 743d  1" markerHeight=
-000011d0: 2231 3122 206f 7269 656e 743d 2261 7574  "11" orient="aut
-000011e0: 6f22 3e3c 7061 7468 2064 3d22 4d20 312c  o"><path d="M 1,
-000011f0: 3120 6c20 392c 3920 4d20 3130 2c31 206c  1 l 9,9 M 10,1 l
-00001200: 202d 392c 3922 2063 6c61 7373 3d22 6172   -9,9" class="ar
-00001210: 726f 774d 6172 6b65 7250 6174 6822 2073  rowMarkerPath" s
-00001220: 7479 6c65 3d22 7374 726f 6b65 2d77 6964  tyle="stroke-wid
-00001230: 7468 3a20 323b 2073 7472 6f6b 652d 6461  th: 2; stroke-da
-00001240: 7368 6172 7261 793a 2031 2c20 303b 223e  sharray: 1, 0;">
-00001250: 3c2f 7061 7468 3e3c 2f6d 6172 6b65 723e  </path></marker>
-00001260: 3c6d 6172 6b65 7220 6964 3d22 666c 6f77  <marker id="flow
-00001270: 6368 6172 742d 6372 6f73 7353 7461 7274  chart-crossStart
-00001280: 2220 636c 6173 733d 226d 6172 6b65 7220  " class="marker 
-00001290: 6372 6f73 7320 666c 6f77 6368 6172 7422  cross flowchart"
-000012a0: 2076 6965 7742 6f78 3d22 3020 3020 3131   viewBox="0 0 11
-000012b0: 2031 3122 2072 6566 583d 222d 3122 2072   11" refX="-1" r
-000012c0: 6566 593d 2235 2e32 2220 6d61 726b 6572  efY="5.2" marker
-000012d0: 556e 6974 733d 2275 7365 7253 7061 6365  Units="userSpace
-000012e0: 4f6e 5573 6522 206d 6172 6b65 7257 6964  OnUse" markerWid
-000012f0: 7468 3d22 3131 2220 6d61 726b 6572 4865  th="11" markerHe
-00001300: 6967 6874 3d22 3131 2220 6f72 6965 6e74  ight="11" orient
-00001310: 3d22 6175 746f 223e 3c70 6174 6820 643d  ="auto"><path d=
-00001320: 224d 2031 2c31 206c 2039 2c39 204d 2031  "M 1,1 l 9,9 M 1
-00001330: 302c 3120 6c20 2d39 2c39 2220 636c 6173  0,1 l -9,9" clas
-00001340: 733d 2261 7272 6f77 4d61 726b 6572 5061  s="arrowMarkerPa
-00001350: 7468 2220 7374 796c 653d 2273 7472 6f6b  th" style="strok
-00001360: 652d 7769 6474 683a 2032 3b20 7374 726f  e-width: 2; stro
-00001370: 6b65 2d64 6173 6861 7272 6179 3a20 312c  ke-dasharray: 1,
-00001380: 2030 3b22 3e3c 2f70 6174 683e 3c2f 6d61   0;"></path></ma
-00001390: 726b 6572 3e3c 6720 636c 6173 733d 2272  rker><g class="r
-000013a0: 6f6f 7422 3e3c 6720 636c 6173 733d 2263  oot"><g class="c
-000013b0: 6c75 7374 6572 7322 3e3c 2f67 3e3c 6720  lusters"></g><g 
-000013c0: 636c 6173 733d 2265 6467 6550 6174 6873  class="edgePaths
-000013d0: 223e 3c70 6174 6820 643d 224d 3734 2e37  "><path d="M74.7
-000013e0: 3138 3735 2c31 3239 4c37 382e 3838 3534  1875,129L78.8854
-000013f0: 3136 3636 3636 3636 3637 2c31 3239 4338  1666666667,129C8
-00001400: 332e 3035 3230 3833 3333 3333 3333 3333  3.05208333333333
-00001410: 2c31 3239 2c39 312e 3338 3534 3136 3636  ,129,91.38541666
-00001420: 3636 3636 3637 2c31 3239 2c39 392e 3731  666667,129,99.71
-00001430: 3837 352c 3132 3943 3130 382e 3035 3230  875,129C108.0520
-00001440: 3833 3333 3333 3333 3333 2c31 3239 2c31  8333333333,129,1
-00001450: 3136 2e33 3835 3431 3636 3636 3636 3636  16.3854166666666
-00001460: 372c 3132 392c 3132 302e 3535 3230 3833  7,129,120.552083
-00001470: 3333 3333 3333 3333 2c31 3239 4c31 3234  33333333,129L124
-00001480: 2e37 3138 3735 2c31 3239 2220 6964 3d22  .71875,129" id="
-00001490: 4c2d 6761 7465 7761 7973 7461 7274 2d45  L-gatewaystart-E
-000014a0: 2d30 2220 636c 6173 733d 2220 6564 6765  -0" class=" edge
-000014b0: 2d74 6869 636b 6e65 7373 2d6e 6f72 6d61  -thickness-norma
-000014c0: 6c20 6564 6765 2d70 6174 7465 726e 2d73  l edge-pattern-s
-000014d0: 6f6c 6964 2066 6c6f 7763 6861 7274 2d6c  olid flowchart-l
-000014e0: 696e 6b20 4c53 2d67 6174 6577 6179 7374  ink LS-gatewayst
-000014f0: 6172 7420 4c45 2d45 2220 7374 796c 653d  art LE-E" style=
-00001500: 2266 696c 6c3a 6e6f 6e65 3b22 206d 6172  "fill:none;" mar
-00001510: 6b65 722d 656e 643d 2275 726c 2823 666c  ker-end="url(#fl
-00001520: 6f77 6368 6172 742d 706f 696e 7445 6e64  owchart-pointEnd
-00001530: 2922 3e3c 2f70 6174 683e 3c70 6174 6820  )"></path><path 
-00001540: 643d 224d 3139 382e 3239 3638 3735 2c31  d="M198.296875,1
-00001550: 3734 2e38 3435 3631 3839 3135 3135 3939  74.8456189151599
-00001560: 354c 3230 322e 3436 3335 3431 3636 3636  5L202.4635416666
-00001570: 3636 3636 2c31 3830 2e30 3338 3031 3537  6666,180.0380157
-00001580: 3632 3633 3333 4332 3036 2e36 3330 3230  626333C206.63020
-00001590: 3833 3333 3333 3333 342c 3138 352e 3233  833333334,185.23
-000015a0: 3034 3132 3631 3031 3036 3634 2c32 3134  041261010664,214
-000015b0: 2e39 3633 3534 3136 3636 3636 3636 362c  .96354166666666,
-000015c0: 3139 352e 3631 3532 3036 3330 3530 3533  195.615206305053
-000015d0: 3333 2c32 3233 2e32 3936 3837 352c 3230  33,223.296875,20
-000015e0: 302e 3830 3736 3033 3135 3235 3236 3637  0.80760315252667
-000015f0: 4332 3331 2e36 3330 3230 3833 3333 3333  C231.63020833333
-00001600: 3333 342c 3230 362c 3233 392e 3936 3335  334,206,239.9635
-00001610: 3431 3636 3636 3636 3636 2c32 3036 2c32  4166666666,206,2
-00001620: 3434 2e31 3330 3230 3833 3333 3333 3333  44.1302083333333
-00001630: 342c 3230 364c 3234 382e 3239 3638 3735  4,206L248.296875
-00001640: 2c32 3036 2220 6964 3d22 4c2d 452d 4545  ,206" id="L-E-EE
-00001650: 2d30 2220 636c 6173 733d 2220 6564 6765  -0" class=" edge
-00001660: 2d74 6869 636b 6e65 7373 2d6e 6f72 6d61  -thickness-norma
-00001670: 6c20 6564 6765 2d70 6174 7465 726e 2d73  l edge-pattern-s
-00001680: 6f6c 6964 2066 6c6f 7763 6861 7274 2d6c  olid flowchart-l
-00001690: 696e 6b20 4c53 2d45 204c 452d 4545 2220  ink LS-E LE-EE" 
-000016a0: 7374 796c 653d 2266 696c 6c3a 6e6f 6e65  style="fill:none
-000016b0: 3b22 206d 6172 6b65 722d 656e 643d 2275  ;" marker-end="u
-000016c0: 726c 2823 666c 6f77 6368 6172 742d 706f  rl(#flowchart-po
-000016d0: 696e 7445 6e64 2922 3e3c 2f70 6174 683e  intEnd)"></path>
-000016e0: 3c70 6174 6820 643d 224d 3139 382e 3239  <path d="M198.29
-000016f0: 3638 3735 2c38 332e 3135 3433 3831 3038  6875,83.15438108
-00001700: 3438 3430 3035 4c32 3032 2e34 3633 3534  484005L202.46354
-00001710: 3136 3636 3636 3636 362c 3737 2e39 3631  166666666,77.961
-00001720: 3938 3432 3337 3336 3637 4332 3036 2e36  9842373667C206.6
-00001730: 3330 3230 3833 3333 3333 3333 342c 3732  3020833333334,72
-00001740: 2e37 3639 3538 3733 3839 3839 3333 372c  .76958738989337,
-00001750: 3231 342e 3936 3335 3431 3636 3636 3636  214.963541666666
-00001760: 3636 2c36 322e 3338 3437 3933 3639 3439  66,62.3847936949
-00001770: 3436 3639 2c32 3233 2e33 3131 3139 3739  4669,223.3111979
-00001780: 3136 3636 3636 362c 3537 2e31 3932 3339  1666666,57.19239
-00001790: 3638 3437 3437 3333 3443 3233 312e 3635  684747334C231.65
-000017a0: 3838 3534 3136 3636 3636 3636 2c35 322c  885416666666,52,
-000017b0: 3234 302e 3032 3038 3333 3333 3333 3333  240.020833333333
-000017c0: 3334 2c35 322c 3234 342e 3230 3138 3232  34,52,244.201822
-000017d0: 3931 3636 3636 3636 2c35 324c 3234 382e  91666666,52L248.
-000017e0: 3338 3238 3132 352c 3532 2220 6964 3d22  3828125,52" id="
-000017f0: 4c2d 452d 6578 6563 7574 6f72 322d 3022  L-E-executor2-0"
-00001800: 2063 6c61 7373 3d22 2065 6467 652d 7468   class=" edge-th
-00001810: 6963 6b6e 6573 732d 6e6f 726d 616c 2065  ickness-normal e
-00001820: 6467 652d 7061 7474 6572 6e2d 736f 6c69  dge-pattern-soli
-00001830: 6420 666c 6f77 6368 6172 742d 6c69 6e6b  d flowchart-link
-00001840: 204c 532d 4520 4c45 2d65 7865 6375 746f   LS-E LE-executo
-00001850: 7232 2220 7374 796c 653d 2266 696c 6c3a  r2" style="fill:
-00001860: 6e6f 6e65 3b22 206d 6172 6b65 722d 656e  none;" marker-en
-00001870: 643d 2275 726c 2823 666c 6f77 6368 6172  d="url(#flowchar
-00001880: 742d 706f 696e 7445 6e64 2922 3e3c 2f70  t-pointEnd)"></p
-00001890: 6174 683e 3c70 6174 6820 643d 224d 3333  ath><path d="M33
-000018a0: 302e 3433 3735 2c32 3036 4c33 3334 2e36  0.4375,206L334.6
-000018b0: 3034 3136 3636 3636 3636 3637 2c32 3036  041666666667,206
-000018c0: 4333 3338 2e37 3730 3833 3333 3333 3333  C338.77083333333
-000018d0: 3333 2c32 3036 2c33 3437 2e31 3034 3136  33,206,347.10416
-000018e0: 3636 3636 3636 3637 2c32 3036 2c33 3535  66666667,206,355
-000018f0: 2e34 3337 352c 3230 3643 3336 332e 3737  .4375,206C363.77
-00001900: 3038 3333 3333 3333 3333 332c 3230 362c  08333333333,206,
-00001910: 3337 322e 3130 3431 3636 3636 3636 3636  372.104166666666
-00001920: 372c 3230 362c 3337 362e 3237 3038 3333  7,206,376.270833
-00001930: 3333 3333 3333 332c 3230 364c 3338 302e  3333333,206L380.
-00001940: 3433 3735 2c32 3036 2220 6964 3d22 4c2d  4375,206" id="L-
-00001950: 4545 2d65 7865 6375 746f 7233 2d30 2220  EE-executor3-0" 
-00001960: 636c 6173 733d 2220 6564 6765 2d74 6869  class=" edge-thi
-00001970: 636b 6e65 7373 2d6e 6f72 6d61 6c20 6564  ckness-normal ed
-00001980: 6765 2d70 6174 7465 726e 2d73 6f6c 6964  ge-pattern-solid
-00001990: 2066 6c6f 7763 6861 7274 2d6c 696e 6b20   flowchart-link 
-000019a0: 4c53 2d45 4520 4c45 2d65 7865 6375 746f  LS-EE LE-executo
-000019b0: 7233 2220 7374 796c 653d 2266 696c 6c3a  r3" style="fill:
-000019c0: 6e6f 6e65 3b22 206d 6172 6b65 722d 656e  none;" marker-en
-000019d0: 643d 2275 726c 2823 666c 6f77 6368 6172  d="url(#flowchar
-000019e0: 742d 706f 696e 7445 6e64 2922 3e3c 2f70  t-pointEnd)"></p
-000019f0: 6174 683e 3c70 6174 6820 643d 224d 3436  ath><path d="M46
-00001a00: 322e 3430 3632 352c 3230 364c 3436 362e  2.40625,206L466.
-00001a10: 3537 3239 3136 3636 3636 3636 372c 3230  5729166666667,20
-00001a20: 3643 3437 302e 3733 3935 3833 3333 3333  6C470.7395833333
-00001a30: 3333 332c 3230 362c 3437 392e 3037 3239  333,206,479.0729
-00001a40: 3136 3636 3636 3636 372c 3230 362c 3438  166666667,206,48
-00001a50: 372e 3430 3632 352c 3230 3643 3439 352e  7.40625,206C495.
-00001a60: 3733 3935 3833 3333 3333 3333 332c 3230  7395833333333,20
-00001a70: 362c 3530 342e 3037 3239 3136 3636 3636  6,504.0729166666
-00001a80: 3636 372c 3230 362c 3530 382e 3233 3935  667,206,508.2395
-00001a90: 3833 3333 3333 3333 332c 3230 364c 3531  833333333,206L51
-00001aa0: 322e 3430 3632 352c 3230 3622 2069 643d  2.40625,206" id=
-00001ab0: 224c 2d65 7865 6375 746f 7233 2d67 6174  "L-executor3-gat
-00001ac0: 6577 6179 656e 642d 3022 2063 6c61 7373  ewayend-0" class
-00001ad0: 3d22 2065 6467 652d 7468 6963 6b6e 6573  =" edge-thicknes
-00001ae0: 732d 6e6f 726d 616c 2065 6467 652d 7061  s-normal edge-pa
-00001af0: 7474 6572 6e2d 736f 6c69 6420 666c 6f77  ttern-solid flow
-00001b00: 6368 6172 742d 6c69 6e6b 204c 532d 6578  chart-link LS-ex
-00001b10: 6563 7574 6f72 3320 4c45 2d67 6174 6577  ecutor3 LE-gatew
-00001b20: 6179 656e 6422 2073 7479 6c65 3d22 6669  ayend" style="fi
-00001b30: 6c6c 3a6e 6f6e 653b 2220 6d61 726b 6572  ll:none;" marker
-00001b40: 2d65 6e64 3d22 7572 6c28 2366 6c6f 7763  -end="url(#flowc
-00001b50: 6861 7274 2d70 6f69 6e74 456e 6429 223e  hart-pointEnd)">
-00001b60: 3c2f 7061 7468 3e3c 2f67 3e3c 6720 636c  </path></g><g cl
-00001b70: 6173 733d 2265 6467 654c 6162 656c 7322  ass="edgeLabels"
-00001b80: 3e3c 6720 636c 6173 733d 2265 6467 654c  ><g class="edgeL
-00001b90: 6162 656c 223e 3c67 2063 6c61 7373 3d22  abel"><g class="
-00001ba0: 6c61 6265 6c22 2074 7261 6e73 666f 726d  label" transform
-00001bb0: 3d22 7472 616e 736c 6174 6528 302c 2030  ="translate(0, 0
-00001bc0: 2922 3e3c 666f 7265 6967 6e4f 626a 6563  )"><foreignObjec
-00001bd0: 7420 7769 6474 683d 2230 2220 6865 6967  t width="0" heig
-00001be0: 6874 3d22 3022 3e3c 6469 7620 786d 6c6e  ht="0"><div xmln
-00001bf0: 733d 2268 7474 703a 2f2f 7777 772e 7733  s="http://www.w3
-00001c00: 2e6f 7267 2f31 3939 392f 7868 746d 6c22  .org/1999/xhtml"
-00001c10: 2073 7479 6c65 3d22 6469 7370 6c61 793a   style="display:
-00001c20: 2069 6e6c 696e 652d 626c 6f63 6b3b 2077   inline-block; w
-00001c30: 6869 7465 2d73 7061 6365 3a20 6e6f 7772  hite-space: nowr
-00001c40: 6170 3b22 3e3c 7370 616e 2063 6c61 7373  ap;"><span class
-00001c50: 3d22 6564 6765 4c61 6265 6c22 3e3c 2f73  ="edgeLabel"></s
-00001c60: 7061 6e3e 3c2f 6469 763e 3c2f 666f 7265  pan></div></fore
-00001c70: 6967 6e4f 626a 6563 743e 3c2f 673e 3c2f  ignObject></g></
-00001c80: 673e 3c67 2063 6c61 7373 3d22 6564 6765  g><g class="edge
-00001c90: 4c61 6265 6c22 3e3c 6720 636c 6173 733d  Label"><g class=
-00001ca0: 226c 6162 656c 2220 7472 616e 7366 6f72  "label" transfor
-00001cb0: 6d3d 2274 7261 6e73 6c61 7465 2830 2c20  m="translate(0, 
-00001cc0: 3029 223e 3c66 6f72 6569 676e 4f62 6a65  0)"><foreignObje
-00001cd0: 6374 2077 6964 7468 3d22 3022 2068 6569  ct width="0" hei
-00001ce0: 6768 743d 2230 223e 3c64 6976 2078 6d6c  ght="0"><div xml
-00001cf0: 6e73 3d22 6874 7470 3a2f 2f77 7777 2e77  ns="http://www.w
-00001d00: 332e 6f72 672f 3139 3939 2f78 6874 6d6c  3.org/1999/xhtml
-00001d10: 2220 7374 796c 653d 2264 6973 706c 6179  " style="display
-00001d20: 3a20 696e 6c69 6e65 2d62 6c6f 636b 3b20  : inline-block; 
-00001d30: 7768 6974 652d 7370 6163 653a 206e 6f77  white-space: now
-00001d40: 7261 703b 223e 3c73 7061 6e20 636c 6173  rap;"><span clas
-00001d50: 733d 2265 6467 654c 6162 656c 223e 3c2f  s="edgeLabel"></
-00001d60: 7370 616e 3e3c 2f64 6976 3e3c 2f66 6f72  span></div></for
-00001d70: 6569 676e 4f62 6a65 6374 3e3c 2f67 3e3c  eignObject></g><
-00001d80: 2f67 3e3c 6720 636c 6173 733d 2265 6467  /g><g class="edg
-00001d90: 654c 6162 656c 223e 3c67 2063 6c61 7373  eLabel"><g class
-00001da0: 3d22 6c61 6265 6c22 2074 7261 6e73 666f  ="label" transfo
-00001db0: 726d 3d22 7472 616e 736c 6174 6528 302c  rm="translate(0,
-00001dc0: 2030 2922 3e3c 666f 7265 6967 6e4f 626a   0)"><foreignObj
-00001dd0: 6563 7420 7769 6474 683d 2230 2220 6865  ect width="0" he
-00001de0: 6967 6874 3d22 3022 3e3c 6469 7620 786d  ight="0"><div xm
-00001df0: 6c6e 733d 2268 7474 703a 2f2f 7777 772e  lns="http://www.
-00001e00: 7733 2e6f 7267 2f31 3939 392f 7868 746d  w3.org/1999/xhtm
-00001e10: 6c22 2073 7479 6c65 3d22 6469 7370 6c61  l" style="displa
-00001e20: 793a 2069 6e6c 696e 652d 626c 6f63 6b3b  y: inline-block;
-00001e30: 2077 6869 7465 2d73 7061 6365 3a20 6e6f   white-space: no
-00001e40: 7772 6170 3b22 3e3c 7370 616e 2063 6c61  wrap;"><span cla
-00001e50: 7373 3d22 6564 6765 4c61 6265 6c22 3e3c  ss="edgeLabel"><
-00001e60: 2f73 7061 6e3e 3c2f 6469 763e 3c2f 666f  /span></div></fo
-00001e70: 7265 6967 6e4f 626a 6563 743e 3c2f 673e  reignObject></g>
-00001e80: 3c2f 673e 3c67 2063 6c61 7373 3d22 6564  </g><g class="ed
-00001e90: 6765 4c61 6265 6c22 3e3c 6720 636c 6173  geLabel"><g clas
-00001ea0: 733d 226c 6162 656c 2220 7472 616e 7366  s="label" transf
-00001eb0: 6f72 6d3d 2274 7261 6e73 6c61 7465 2830  orm="translate(0
-00001ec0: 2c20 3029 223e 3c66 6f72 6569 676e 4f62  , 0)"><foreignOb
-00001ed0: 6a65 6374 2077 6964 7468 3d22 3022 2068  ject width="0" h
-00001ee0: 6569 6768 743d 2230 223e 3c64 6976 2078  eight="0"><div x
-00001ef0: 6d6c 6e73 3d22 6874 7470 3a2f 2f77 7777  mlns="http://www
-00001f00: 2e77 332e 6f72 672f 3139 3939 2f78 6874  .w3.org/1999/xht
-00001f10: 6d6c 2220 7374 796c 653d 2264 6973 706c  ml" style="displ
-00001f20: 6179 3a20 696e 6c69 6e65 2d62 6c6f 636b  ay: inline-block
-00001f30: 3b20 7768 6974 652d 7370 6163 653a 206e  ; white-space: n
-00001f40: 6f77 7261 703b 223e 3c73 7061 6e20 636c  owrap;"><span cl
-00001f50: 6173 733d 2265 6467 654c 6162 656c 223e  ass="edgeLabel">
-00001f60: 3c2f 7370 616e 3e3c 2f64 6976 3e3c 2f66  </span></div></f
-00001f70: 6f72 6569 676e 4f62 6a65 6374 3e3c 2f67  oreignObject></g
-00001f80: 3e3c 2f67 3e3c 6720 636c 6173 733d 2265  ></g><g class="e
-00001f90: 6467 654c 6162 656c 223e 3c67 2063 6c61  dgeLabel"><g cla
-00001fa0: 7373 3d22 6c61 6265 6c22 2074 7261 6e73  ss="label" trans
-00001fb0: 666f 726d 3d22 7472 616e 736c 6174 6528  form="translate(
-00001fc0: 302c 2030 2922 3e3c 666f 7265 6967 6e4f  0, 0)"><foreignO
-00001fd0: 626a 6563 7420 7769 6474 683d 2230 2220  bject width="0" 
-00001fe0: 6865 6967 6874 3d22 3022 3e3c 6469 7620  height="0"><div 
-00001ff0: 786d 6c6e 733d 2268 7474 703a 2f2f 7777  xmlns="http://ww
-00002000: 772e 7733 2e6f 7267 2f31 3939 392f 7868  w.w3.org/1999/xh
-00002010: 746d 6c22 2073 7479 6c65 3d22 6469 7370  tml" style="disp
-00002020: 6c61 793a 2069 6e6c 696e 652d 626c 6f63  lay: inline-bloc
-00002030: 6b3b 2077 6869 7465 2d73 7061 6365 3a20  k; white-space: 
-00002040: 6e6f 7772 6170 3b22 3e3c 7370 616e 2063  nowrap;"><span c
-00002050: 6c61 7373 3d22 6564 6765 4c61 6265 6c22  lass="edgeLabel"
-00002060: 3e3c 2f73 7061 6e3e 3c2f 6469 763e 3c2f  ></span></div></
-00002070: 666f 7265 6967 6e4f 626a 6563 743e 3c2f  foreignObject></
-00002080: 673e 3c2f 673e 3c2f 673e 3c67 2063 6c61  g></g></g><g cla
-00002090: 7373 3d22 6e6f 6465 7322 3e3c 6720 636c  ss="nodes"><g cl
-000020a0: 6173 733d 2272 6f6f 7422 2074 7261 6e73  ass="root" trans
-000020b0: 666f 726d 3d22 7472 616e 736c 6174 6528  form="translate(
-000020c0: 3337 322e 3933 3735 2c20 3134 3629 223e  372.9375, 146)">
-000020d0: 3c67 2063 6c61 7373 3d22 636c 7573 7465  <g class="cluste
-000020e0: 7273 223e 3c67 2063 6c61 7373 3d22 636c  rs"><g class="cl
-000020f0: 7573 7465 7220 4445 504c 4f59 4d45 4e54  uster DEPLOYMENT
-00002100: 2044 4550 4c4f 594d 454e 5420 4445 504c   DEPLOYMENT DEPL
-00002110: 4f59 4d45 4e54 2044 4550 4c4f 594d 454e  OYMENT DEPLOYMEN
-00002120: 5422 2069 643d 2265 7865 6375 746f 7233  T" id="executor3
-00002130: 223e 3c72 6563 7420 7374 796c 653d 2222  "><rect style=""
-00002140: 2072 783d 2230 2220 7279 3d22 3022 2078   rx="0" ry="0" x
-00002150: 3d22 3822 2079 3d22 3822 2077 6964 7468  ="8" y="8" width
-00002160: 3d22 3831 2e39 3638 3735 2220 6865 6967  ="81.96875" heig
-00002170: 6874 3d22 3130 3422 3e3c 2f72 6563 743e  ht="104"></rect>
-00002180: 3c67 2063 6c61 7373 3d22 636c 7573 7465  <g class="cluste
-00002190: 722d 6c61 6265 6c22 2074 7261 6e73 666f  r-label" transfo
-000021a0: 726d 3d22 7472 616e 736c 6174 6528 3133  rm="translate(13
-000021b0: 2e31 3438 3433 3735 2c20 3829 223e 3c66  .1484375, 8)"><f
-000021c0: 6f72 6569 676e 4f62 6a65 6374 2077 6964  oreignObject wid
-000021d0: 7468 3d22 3731 2e36 3731 3837 3522 2068  th="71.671875" h
-000021e0: 6569 6768 743d 2231 3922 3e3c 6469 7620  eight="19"><div 
-000021f0: 786d 6c6e 733d 2268 7474 703a 2f2f 7777  xmlns="http://ww
-00002200: 772e 7733 2e6f 7267 2f31 3939 392f 7868  w.w3.org/1999/xh
-00002210: 746d 6c22 2073 7479 6c65 3d22 6469 7370  tml" style="disp
-00002220: 6c61 793a 2069 6e6c 696e 652d 626c 6f63  lay: inline-bloc
-00002230: 6b3b 2077 6869 7465 2d73 7061 6365 3a20  k; white-space: 
-00002240: 6e6f 7772 6170 3b22 3e3c 7370 616e 2063  nowrap;"><span c
-00002250: 6c61 7373 3d22 6e6f 6465 4c61 6265 6c22  lass="nodeLabel"
-00002260: 3e65 7865 6375 746f 7233 3c2f 7370 616e  >executor3</span
-00002270: 3e3c 2f64 6976 3e3c 2f66 6f72 6569 676e  ></div></foreign
-00002280: 4f62 6a65 6374 3e3c 2f67 3e3c 2f67 3e3c  Object></g></g><
-00002290: 2f67 3e3c 6720 636c 6173 733d 2265 6467  /g><g class="edg
-000022a0: 6550 6174 6873 223e 3c2f 673e 3c67 2063  ePaths"></g><g c
-000022b0: 6c61 7373 3d22 6564 6765 4c61 6265 6c73  lass="edgeLabels
-000022c0: 223e 3c2f 673e 3c67 2063 6c61 7373 3d22  "></g><g class="
-000022d0: 6e6f 6465 7322 3e3c 6720 636c 6173 733d  nodes"><g class=
-000022e0: 226e 6f64 6520 6465 6661 756c 7420 706f  "node default po
-000022f0: 6422 2069 643d 2266 6c6f 7763 6861 7274  d" id="flowchart
-00002300: 2d65 7865 6375 746f 7233 2f72 6570 2d30  -executor3/rep-0
-00002310: 2d33 3122 2074 7261 6e73 666f 726d 3d22  -31" transform="
-00002320: 7472 616e 736c 6174 6528 3438 2e39 3834  translate(48.984
-00002330: 3337 352c 2036 3029 223e 3c72 6563 7420  375, 60)"><rect 
-00002340: 636c 6173 733d 2262 6173 6963 206c 6162  class="basic lab
-00002350: 656c 2d63 6f6e 7461 696e 6572 2220 7374  el-container" st
-00002360: 796c 653d 2222 2072 783d 2230 2220 7279  yle="" rx="0" ry
-00002370: 3d22 3022 2078 3d22 2d31 352e 3938 3433  ="0" x="-15.9843
-00002380: 3735 2220 793d 222d 3137 2220 7769 6474  75" y="-17" widt
-00002390: 683d 2233 312e 3936 3837 3522 2068 6569  h="31.96875" hei
-000023a0: 6768 743d 2233 3422 3e3c 2f72 6563 743e  ght="34"></rect>
-000023b0: 3c67 2063 6c61 7373 3d22 6c61 6265 6c22  <g class="label"
-000023c0: 2073 7479 6c65 3d22 2220 7472 616e 7366   style="" transf
-000023d0: 6f72 6d3d 2274 7261 6e73 6c61 7465 282d  orm="translate(-
-000023e0: 382e 3438 3433 3735 2c20 2d39 2e35 2922  8.484375, -9.5)"
-000023f0: 3e3c 666f 7265 6967 6e4f 626a 6563 7420  ><foreignObject 
-00002400: 7769 6474 683d 2231 362e 3936 3837 3522  width="16.96875"
-00002410: 2068 6569 6768 743d 2231 3922 3e3c 6469   height="19"><di
-00002420: 7620 786d 6c6e 733d 2268 7474 703a 2f2f  v xmlns="http://
-00002430: 7777 772e 7733 2e6f 7267 2f31 3939 392f  www.w3.org/1999/
-00002440: 7868 746d 6c22 2073 7479 6c65 3d22 6469  xhtml" style="di
-00002450: 7370 6c61 793a 2069 6e6c 696e 652d 626c  splay: inline-bl
-00002460: 6f63 6b3b 2077 6869 7465 2d73 7061 6365  ock; white-space
-00002470: 3a20 6e6f 7772 6170 3b22 3e3c 7370 616e  : nowrap;"><span
-00002480: 2063 6c61 7373 3d22 6e6f 6465 4c61 6265   class="nodeLabe
-00002490: 6c22 3e45 323c 2f73 7061 6e3e 3c2f 6469  l">E2</span></di
-000024a0: 763e 3c2f 666f 7265 6967 6e4f 626a 6563  v></foreignObjec
-000024b0: 743e 3c2f 673e 3c2f 673e 3c2f 673e 3c2f  t></g></g></g></
-000024c0: 673e 3c67 2063 6c61 7373 3d22 726f 6f74  g><g class="root
-000024d0: 2220 7472 616e 7366 6f72 6d3d 2274 7261  " transform="tra
-000024e0: 6e73 6c61 7465 2832 3430 2e38 3832 3831  nslate(240.88281
-000024f0: 3235 2c20 2d38 2922 3e3c 6720 636c 6173  25, -8)"><g clas
-00002500: 733d 2263 6c75 7374 6572 7322 3e3c 6720  s="clusters"><g 
-00002510: 636c 6173 733d 2263 6c75 7374 6572 2044  class="cluster D
-00002520: 4550 4c4f 594d 454e 5420 4445 504c 4f59  EPLOYMENT DEPLOY
-00002530: 4d45 4e54 2220 6964 3d22 6578 6563 7574  MENT" id="execut
-00002540: 6f72 3222 3e3c 7265 6374 2073 7479 6c65  or2"><rect style
-00002550: 3d22 2220 7278 3d22 3022 2072 793d 2230  ="" rx="0" ry="0
-00002560: 2220 783d 2238 2220 793d 2238 2220 7769  " x="8" y="8" wi
-00002570: 6474 683d 2238 312e 3936 3837 3522 2068  dth="81.96875" h
-00002580: 6569 6768 743d 2231 3034 223e 3c2f 7265  eight="104"></re
-00002590: 6374 3e3c 6720 636c 6173 733d 2263 6c75  ct><g class="clu
-000025a0: 7374 6572 2d6c 6162 656c 2220 7472 616e  ster-label" tran
-000025b0: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
-000025c0: 2831 332e 3134 3834 3337 352c 2038 2922  (13.1484375, 8)"
-000025d0: 3e3c 666f 7265 6967 6e4f 626a 6563 7420  ><foreignObject 
-000025e0: 7769 6474 683d 2237 312e 3637 3138 3735  width="71.671875
-000025f0: 2220 6865 6967 6874 3d22 3139 223e 3c64  " height="19"><d
-00002600: 6976 2078 6d6c 6e73 3d22 6874 7470 3a2f  iv xmlns="http:/
-00002610: 2f77 7777 2e77 332e 6f72 672f 3139 3939  /www.w3.org/1999
-00002620: 2f78 6874 6d6c 2220 7374 796c 653d 2264  /xhtml" style="d
-00002630: 6973 706c 6179 3a20 696e 6c69 6e65 2d62  isplay: inline-b
-00002640: 6c6f 636b 3b20 7768 6974 652d 7370 6163  lock; white-spac
-00002650: 653a 206e 6f77 7261 703b 223e 3c73 7061  e: nowrap;"><spa
-00002660: 6e20 636c 6173 733d 226e 6f64 654c 6162  n class="nodeLab
-00002670: 656c 223e 6578 6563 7574 6f72 323c 2f73  el">executor2</s
-00002680: 7061 6e3e 3c2f 6469 763e 3c2f 666f 7265  pan></div></fore
-00002690: 6967 6e4f 626a 6563 743e 3c2f 673e 3c2f  ignObject></g></
-000026a0: 673e 3c2f 673e 3c67 2063 6c61 7373 3d22  g></g><g class="
-000026b0: 6564 6765 5061 7468 7322 3e3c 2f67 3e3c  edgePaths"></g><
-000026c0: 6720 636c 6173 733d 2265 6467 654c 6162  g class="edgeLab
-000026d0: 656c 7322 3e3c 2f67 3e3c 6720 636c 6173  els"></g><g clas
-000026e0: 733d 226e 6f64 6573 223e 3c67 2063 6c61  s="nodes"><g cla
-000026f0: 7373 3d22 6e6f 6465 2064 6566 6175 6c74  ss="node default
-00002700: 2070 6f64 2220 6964 3d22 666c 6f77 6368   pod" id="flowch
-00002710: 6172 742d 6578 6563 7574 6f72 322f 7265  art-executor2/re
-00002720: 702d 302d 3330 2220 7472 616e 7366 6f72  p-0-30" transfor
-00002730: 6d3d 2274 7261 6e73 6c61 7465 2834 382e  m="translate(48.
-00002740: 3938 3433 3735 2c20 3630 2922 3e3c 7265  984375, 60)"><re
-00002750: 6374 2063 6c61 7373 3d22 6261 7369 6320  ct class="basic 
-00002760: 6c61 6265 6c2d 636f 6e74 6169 6e65 7222  label-container"
-00002770: 2073 7479 6c65 3d22 2220 7278 3d22 3022   style="" rx="0"
-00002780: 2072 793d 2230 2220 783d 222d 3135 2e39   ry="0" x="-15.9
-00002790: 3834 3337 3522 2079 3d22 2d31 3722 2077  84375" y="-17" w
-000027a0: 6964 7468 3d22 3331 2e39 3638 3735 2220  idth="31.96875" 
-000027b0: 6865 6967 6874 3d22 3334 223e 3c2f 7265  height="34"></re
-000027c0: 6374 3e3c 6720 636c 6173 733d 226c 6162  ct><g class="lab
-000027d0: 656c 2220 7374 796c 653d 2222 2074 7261  el" style="" tra
-000027e0: 6e73 666f 726d 3d22 7472 616e 736c 6174  nsform="translat
-000027f0: 6528 2d38 2e34 3834 3337 352c 202d 392e  e(-8.484375, -9.
-00002800: 3529 223e 3c66 6f72 6569 676e 4f62 6a65  5)"><foreignObje
-00002810: 6374 2077 6964 7468 3d22 3136 2e39 3638  ct width="16.968
-00002820: 3735 2220 6865 6967 6874 3d22 3139 223e  75" height="19">
-00002830: 3c64 6976 2078 6d6c 6e73 3d22 6874 7470  <div xmlns="http
-00002840: 3a2f 2f77 7777 2e77 332e 6f72 672f 3139  ://www.w3.org/19
-00002850: 3939 2f78 6874 6d6c 2220 7374 796c 653d  99/xhtml" style=
-00002860: 2264 6973 706c 6179 3a20 696e 6c69 6e65  "display: inline
-00002870: 2d62 6c6f 636b 3b20 7768 6974 652d 7370  -block; white-sp
-00002880: 6163 653a 206e 6f77 7261 703b 223e 3c73  ace: nowrap;"><s
-00002890: 7061 6e20 636c 6173 733d 226e 6f64 654c  pan class="nodeL
-000028a0: 6162 656c 223e 4531 3c2f 7370 616e 3e3c  abel">E1</span><
-000028b0: 2f64 6976 3e3c 2f66 6f72 6569 676e 4f62  /div></foreignOb
-000028c0: 6a65 6374 3e3c 2f67 3e3c 2f67 3e3c 2f67  ject></g></g></g
-000028d0: 3e3c 2f67 3e3c 6720 636c 6173 733d 2272  ></g><g class="r
-000028e0: 6f6f 7422 2074 7261 6e73 666f 726d 3d22  oot" transform="
-000028f0: 7472 616e 736c 6174 6528 3234 302e 3739  translate(240.79
-00002900: 3638 3735 2c20 3134 3629 223e 3c67 2063  6875, 146)"><g c
-00002910: 6c61 7373 3d22 636c 7573 7465 7273 223e  lass="clusters">
-00002920: 3c67 2063 6c61 7373 3d22 636c 7573 7465  <g class="cluste
-00002930: 7220 4445 504c 4f59 4d45 4e54 2044 4550  r DEPLOYMENT DEP
-00002940: 4c4f 594d 454e 5420 4445 504c 4f59 4d45  LOYMENT DEPLOYME
-00002950: 4e54 2044 4550 4c4f 594d 454e 5422 2069  NT DEPLOYMENT" i
-00002960: 643d 2245 4522 3e3c 7265 6374 2073 7479  d="EE"><rect sty
-00002970: 6c65 3d22 2220 7278 3d22 3022 2072 793d  le="" rx="0" ry=
-00002980: 2230 2220 783d 2238 2220 793d 2238 2220  "0" x="8" y="8" 
-00002990: 7769 6474 683d 2238 322e 3134 3036 3235  width="82.140625
-000029a0: 2220 6865 6967 6874 3d22 3130 3422 3e3c  " height="104"><
-000029b0: 2f72 6563 743e 3c67 2063 6c61 7373 3d22  /rect><g class="
-000029c0: 636c 7573 7465 722d 6c61 6265 6c22 2074  cluster-label" t
-000029d0: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
-000029e0: 6174 6528 3430 2e35 2c20 3829 223e 3c66  ate(40.5, 8)"><f
-000029f0: 6f72 6569 676e 4f62 6a65 6374 2077 6964  oreignObject wid
-00002a00: 7468 3d22 3137 2e31 3430 3632 3522 2068  th="17.140625" h
-00002a10: 6569 6768 743d 2231 3922 3e3c 6469 7620  eight="19"><div 
-00002a20: 786d 6c6e 733d 2268 7474 703a 2f2f 7777  xmlns="http://ww
-00002a30: 772e 7733 2e6f 7267 2f31 3939 392f 7868  w.w3.org/1999/xh
-00002a40: 746d 6c22 2073 7479 6c65 3d22 6469 7370  tml" style="disp
-00002a50: 6c61 793a 2069 6e6c 696e 652d 626c 6f63  lay: inline-bloc
-00002a60: 6b3b 2077 6869 7465 2d73 7061 6365 3a20  k; white-space: 
-00002a70: 6e6f 7772 6170 3b22 3e3c 7370 616e 2063  nowrap;"><span c
-00002a80: 6c61 7373 3d22 6e6f 6465 4c61 6265 6c22  lass="nodeLabel"
-00002a90: 3e45 453c 2f73 7061 6e3e 3c2f 6469 763e  >EE</span></div>
-00002aa0: 3c2f 666f 7265 6967 6e4f 626a 6563 743e  </foreignObject>
-00002ab0: 3c2f 673e 3c2f 673e 3c2f 673e 3c67 2063  </g></g></g><g c
-00002ac0: 6c61 7373 3d22 6564 6765 5061 7468 7322  lass="edgePaths"
-00002ad0: 3e3c 2f67 3e3c 6720 636c 6173 733d 2265  ></g><g class="e
-00002ae0: 6467 654c 6162 656c 7322 3e3c 2f67 3e3c  dgeLabels"></g><
-00002af0: 6720 636c 6173 733d 226e 6f64 6573 223e  g class="nodes">
-00002b00: 3c67 2063 6c61 7373 3d22 6e6f 6465 2064  <g class="node d
-00002b10: 6566 6175 6c74 2070 6f64 2220 6964 3d22  efault pod" id="
-00002b20: 666c 6f77 6368 6172 742d 4545 2f72 6570  flowchart-EE/rep
-00002b30: 2d30 2d32 3922 2074 7261 6e73 666f 726d  -0-29" transform
-00002b40: 3d22 7472 616e 736c 6174 6528 3439 2e30  ="translate(49.0
-00002b50: 3730 3331 3235 2c20 3630 2922 3e3c 7265  703125, 60)"><re
-00002b60: 6374 2063 6c61 7373 3d22 6261 7369 6320  ct class="basic 
-00002b70: 6c61 6265 6c2d 636f 6e74 6169 6e65 7222  label-container"
-00002b80: 2073 7479 6c65 3d22 2220 7278 3d22 3022   style="" rx="0"
-00002b90: 2072 793d 2230 2220 783d 222d 3136 2e30   ry="0" x="-16.0
-00002ba0: 3730 3331 3235 2220 793d 222d 3137 2220  703125" y="-17" 
-00002bb0: 7769 6474 683d 2233 322e 3134 3036 3235  width="32.140625
-00002bc0: 2220 6865 6967 6874 3d22 3334 223e 3c2f  " height="34"></
-00002bd0: 7265 6374 3e3c 6720 636c 6173 733d 226c  rect><g class="l
-00002be0: 6162 656c 2220 7374 796c 653d 2222 2074  abel" style="" t
-00002bf0: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
-00002c00: 6174 6528 2d38 2e35 3730 3331 3235 2c20  ate(-8.5703125, 
-00002c10: 2d39 2e35 2922 3e3c 666f 7265 6967 6e4f  -9.5)"><foreignO
-00002c20: 626a 6563 7420 7769 6474 683d 2231 372e  bject width="17.
-00002c30: 3134 3036 3235 2220 6865 6967 6874 3d22  140625" height="
-00002c40: 3139 223e 3c64 6976 2078 6d6c 6e73 3d22  19"><div xmlns="
-00002c50: 6874 7470 3a2f 2f77 7777 2e77 332e 6f72  http://www.w3.or
-00002c60: 672f 3139 3939 2f78 6874 6d6c 2220 7374  g/1999/xhtml" st
-00002c70: 796c 653d 2264 6973 706c 6179 3a20 696e  yle="display: in
-00002c80: 6c69 6e65 2d62 6c6f 636b 3b20 7768 6974  line-block; whit
-00002c90: 652d 7370 6163 653a 206e 6f77 7261 703b  e-space: nowrap;
-00002ca0: 223e 3c73 7061 6e20 636c 6173 733d 226e  "><span class="n
-00002cb0: 6f64 654c 6162 656c 223e 4545 3c2f 7370  odeLabel">EE</sp
-00002cc0: 616e 3e3c 2f64 6976 3e3c 2f66 6f72 6569  an></div></forei
-00002cd0: 676e 4f62 6a65 6374 3e3c 2f67 3e3c 2f67  gnObject></g></g
-00002ce0: 3e3c 2f67 3e3c 2f67 3e3c 6720 636c 6173  ></g></g><g clas
-00002cf0: 733d 2272 6f6f 7422 2074 7261 6e73 666f  s="root" transfo
-00002d00: 726d 3d22 7472 616e 736c 6174 6528 3131  rm="translate(11
-00002d10: 372e 3231 3837 352c 2036 3929 223e 3c67  7.21875, 69)"><g
-00002d20: 2063 6c61 7373 3d22 636c 7573 7465 7273   class="clusters
-00002d30: 223e 3c67 2063 6c61 7373 3d22 636c 7573  "><g class="clus
-00002d40: 7465 7220 4445 504c 4f59 4d45 4e54 2044  ter DEPLOYMENT D
-00002d50: 4550 4c4f 594d 454e 5420 4445 504c 4f59  EPLOYMENT DEPLOY
-00002d60: 4d45 4e54 2044 4550 4c4f 594d 454e 5420  MENT DEPLOYMENT 
-00002d70: 4445 504c 4f59 4d45 4e54 2044 4550 4c4f  DEPLOYMENT DEPLO
-00002d80: 594d 454e 5422 2069 643d 2245 223e 3c72  YMENT" id="E"><r
-00002d90: 6563 7420 7374 796c 653d 2222 2072 783d  ect style="" rx=
-00002da0: 2230 2220 7279 3d22 3022 2078 3d22 3822  "0" ry="0" x="8"
-00002db0: 2079 3d22 3822 2077 6964 7468 3d22 3733   y="8" width="73
-00002dc0: 2e35 3738 3132 3522 2068 6569 6768 743d  .578125" height=
-00002dd0: 2231 3034 223e 3c2f 7265 6374 3e3c 6720  "104"></rect><g 
-00002de0: 636c 6173 733d 2263 6c75 7374 6572 2d6c  class="cluster-l
-00002df0: 6162 656c 2220 7472 616e 7366 6f72 6d3d  abel" transform=
-00002e00: 2274 7261 6e73 6c61 7465 2834 302e 352c  "translate(40.5,
-00002e10: 2038 2922 3e3c 666f 7265 6967 6e4f 626a   8)"><foreignObj
-00002e20: 6563 7420 7769 6474 683d 2238 2e35 3738  ect width="8.578
-00002e30: 3132 3522 2068 6569 6768 743d 2231 3922  125" height="19"
-00002e40: 3e3c 6469 7620 786d 6c6e 733d 2268 7474  ><div xmlns="htt
-00002e50: 703a 2f2f 7777 772e 7733 2e6f 7267 2f31  p://www.w3.org/1
-00002e60: 3939 392f 7868 746d 6c22 2073 7479 6c65  999/xhtml" style
-00002e70: 3d22 6469 7370 6c61 793a 2069 6e6c 696e  ="display: inlin
-00002e80: 652d 626c 6f63 6b3b 2077 6869 7465 2d73  e-block; white-s
-00002e90: 7061 6365 3a20 6e6f 7772 6170 3b22 3e3c  pace: nowrap;"><
-00002ea0: 7370 616e 2063 6c61 7373 3d22 6e6f 6465  span class="node
-00002eb0: 4c61 6265 6c22 3e45 3c2f 7370 616e 3e3c  Label">E</span><
-00002ec0: 2f64 6976 3e3c 2f66 6f72 6569 676e 4f62  /div></foreignOb
-00002ed0: 6a65 6374 3e3c 2f67 3e3c 2f67 3e3c 2f67  ject></g></g></g
-00002ee0: 3e3c 6720 636c 6173 733d 2265 6467 6550  ><g class="edgeP
-00002ef0: 6174 6873 223e 3c2f 673e 3c67 2063 6c61  aths"></g><g cla
-00002f00: 7373 3d22 6564 6765 4c61 6265 6c73 223e  ss="edgeLabels">
-00002f10: 3c2f 673e 3c67 2063 6c61 7373 3d22 6e6f  </g><g class="no
-00002f20: 6465 7322 3e3c 6720 636c 6173 733d 226e  des"><g class="n
-00002f30: 6f64 6520 6465 6661 756c 7420 706f 6422  ode default pod"
-00002f40: 2069 643d 2266 6c6f 7763 6861 7274 2d45   id="flowchart-E
-00002f50: 2f72 6570 2d30 2d32 3822 2074 7261 6e73  /rep-0-28" trans
-00002f60: 666f 726d 3d22 7472 616e 736c 6174 6528  form="translate(
-00002f70: 3434 2e37 3839 3036 3235 2c20 3630 2922  44.7890625, 60)"
-00002f80: 3e3c 7265 6374 2063 6c61 7373 3d22 6261  ><rect class="ba
-00002f90: 7369 6320 6c61 6265 6c2d 636f 6e74 6169  sic label-contai
-00002fa0: 6e65 7222 2073 7479 6c65 3d22 2220 7278  ner" style="" rx
-00002fb0: 3d22 3022 2072 793d 2230 2220 783d 222d  ="0" ry="0" x="-
-00002fc0: 3131 2e37 3839 3036 3235 2220 793d 222d  11.7890625" y="-
-00002fd0: 3137 2220 7769 6474 683d 2232 332e 3537  17" width="23.57
-00002fe0: 3831 3235 2220 6865 6967 6874 3d22 3334  8125" height="34
-00002ff0: 223e 3c2f 7265 6374 3e3c 6720 636c 6173  "></rect><g clas
-00003000: 733d 226c 6162 656c 2220 7374 796c 653d  s="label" style=
-00003010: 2222 2074 7261 6e73 666f 726d 3d22 7472  "" transform="tr
-00003020: 616e 736c 6174 6528 2d34 2e32 3839 3036  anslate(-4.28906
-00003030: 3235 2c20 2d39 2e35 2922 3e3c 666f 7265  25, -9.5)"><fore
-00003040: 6967 6e4f 626a 6563 7420 7769 6474 683d  ignObject width=
-00003050: 2238 2e35 3738 3132 3522 2068 6569 6768  "8.578125" heigh
-00003060: 743d 2231 3922 3e3c 6469 7620 786d 6c6e  t="19"><div xmln
-00003070: 733d 2268 7474 703a 2f2f 7777 772e 7733  s="http://www.w3
-00003080: 2e6f 7267 2f31 3939 392f 7868 746d 6c22  .org/1999/xhtml"
-00003090: 2073 7479 6c65 3d22 6469 7370 6c61 793a   style="display:
-000030a0: 2069 6e6c 696e 652d 626c 6f63 6b3b 2077   inline-block; w
-000030b0: 6869 7465 2d73 7061 6365 3a20 6e6f 7772  hite-space: nowr
-000030c0: 6170 3b22 3e3c 7370 616e 2063 6c61 7373  ap;"><span class
-000030d0: 3d22 6e6f 6465 4c61 6265 6c22 3e45 3c2f  ="nodeLabel">E</
-000030e0: 7370 616e 3e3c 2f64 6976 3e3c 2f66 6f72  span></div></for
-000030f0: 6569 676e 4f62 6a65 6374 3e3c 2f67 3e3c  eignObject></g><
-00003100: 2f67 3e3c 2f67 3e3c 2f67 3e3c 6720 636c  /g></g></g><g cl
-00003110: 6173 733d 226e 6f64 6520 6465 6661 756c  ass="node defaul
-00003120: 7420 4741 5445 5741 5922 2069 643d 2266  t GATEWAY" id="f
-00003130: 6c6f 7763 6861 7274 2d67 6174 6577 6179  lowchart-gateway
-00003140: 7374 6172 742d 3332 2220 7472 616e 7366  start-32" transf
-00003150: 6f72 6d3d 2274 7261 6e73 6c61 7465 2833  orm="translate(3
-00003160: 372e 3335 3933 3735 2c20 3132 3929 223e  7.359375, 129)">
-00003170: 3c72 6563 7420 636c 6173 733d 2262 6173  <rect class="bas
-00003180: 6963 206c 6162 656c 2d63 6f6e 7461 696e  ic label-contain
-00003190: 6572 2220 7374 796c 653d 2222 2072 783d  er" style="" rx=
-000031a0: 2230 2220 7279 3d22 3022 2078 3d22 2d33  "0" ry="0" x="-3
-000031b0: 372e 3335 3933 3735 2220 793d 222d 3137  7.359375" y="-17
-000031c0: 2220 7769 6474 683d 2237 342e 3731 3837  " width="74.7187
-000031d0: 3522 2068 6569 6768 743d 2233 3422 3e3c  5" height="34"><
-000031e0: 2f72 6563 743e 3c67 2063 6c61 7373 3d22  /rect><g class="
-000031f0: 6c61 6265 6c22 2073 7479 6c65 3d22 2220  label" style="" 
-00003200: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
-00003210: 6c61 7465 282d 3239 2e38 3539 3337 352c  late(-29.859375,
-00003220: 202d 392e 3529 223e 3c66 6f72 6569 676e   -9.5)"><foreign
-00003230: 4f62 6a65 6374 2077 6964 7468 3d22 3539  Object width="59
-00003240: 2e37 3138 3735 2220 6865 6967 6874 3d22  .71875" height="
-00003250: 3139 223e 3c64 6976 2078 6d6c 6e73 3d22  19"><div xmlns="
-00003260: 6874 7470 3a2f 2f77 7777 2e77 332e 6f72  http://www.w3.or
-00003270: 672f 3139 3939 2f78 6874 6d6c 2220 7374  g/1999/xhtml" st
-00003280: 796c 653d 2264 6973 706c 6179 3a20 696e  yle="display: in
-00003290: 6c69 6e65 2d62 6c6f 636b 3b20 7768 6974  line-block; whit
-000032a0: 652d 7370 6163 653a 206e 6f77 7261 703b  e-space: nowrap;
-000032b0: 223e 3c73 7061 6e20 636c 6173 733d 226e  "><span class="n
-000032c0: 6f64 654c 6162 656c 223e 6761 7465 7761  odeLabel">gatewa
-000032d0: 793c 2f73 7061 6e3e 3c2f 6469 763e 3c2f  y</span></div></
-000032e0: 666f 7265 6967 6e4f 626a 6563 743e 3c2f  foreignObject></
-000032f0: 673e 3c2f 673e 3c67 2063 6c61 7373 3d22  g></g><g class="
-00003300: 6e6f 6465 2064 6566 6175 6c74 2047 4154  node default GAT
-00003310: 4557 4159 2220 6964 3d22 666c 6f77 6368  EWAY" id="flowch
-00003320: 6172 742d 6761 7465 7761 7965 6e64 2d34  art-gatewayend-4
-00003330: 3122 2074 7261 6e73 666f 726d 3d22 7472  1" transform="tr
-00003340: 616e 736c 6174 6528 3534 392e 3736 3536  anslate(549.7656
-00003350: 3235 2c20 3230 3629 223e 3c72 6563 7420  25, 206)"><rect 
-00003360: 636c 6173 733d 2262 6173 6963 206c 6162  class="basic lab
-00003370: 656c 2d63 6f6e 7461 696e 6572 2220 7374  el-container" st
-00003380: 796c 653d 2222 2072 783d 2230 2220 7279  yle="" rx="0" ry
-00003390: 3d22 3022 2078 3d22 2d33 372e 3335 3933  ="0" x="-37.3593
-000033a0: 3735 2220 793d 222d 3137 2220 7769 6474  75" y="-17" widt
-000033b0: 683d 2237 342e 3731 3837 3522 2068 6569  h="74.71875" hei
-000033c0: 6768 743d 2233 3422 3e3c 2f72 6563 743e  ght="34"></rect>
-000033d0: 3c67 2063 6c61 7373 3d22 6c61 6265 6c22  <g class="label"
-000033e0: 2073 7479 6c65 3d22 2220 7472 616e 7366   style="" transf
-000033f0: 6f72 6d3d 2274 7261 6e73 6c61 7465 282d  orm="translate(-
-00003400: 3239 2e38 3539 3337 352c 202d 392e 3529  29.859375, -9.5)
-00003410: 223e 3c66 6f72 6569 676e 4f62 6a65 6374  "><foreignObject
-00003420: 2077 6964 7468 3d22 3539 2e37 3138 3735   width="59.71875
-00003430: 2220 6865 6967 6874 3d22 3139 223e 3c64  " height="19"><d
-00003440: 6976 2078 6d6c 6e73 3d22 6874 7470 3a2f  iv xmlns="http:/
-00003450: 2f77 7777 2e77 332e 6f72 672f 3139 3939  /www.w3.org/1999
-00003460: 2f78 6874 6d6c 2220 7374 796c 653d 2264  /xhtml" style="d
-00003470: 6973 706c 6179 3a20 696e 6c69 6e65 2d62  isplay: inline-b
-00003480: 6c6f 636b 3b20 7768 6974 652d 7370 6163  lock; white-spac
-00003490: 653a 206e 6f77 7261 703b 223e 3c73 7061  e: nowrap;"><spa
-000034a0: 6e20 636c 6173 733d 226e 6f64 654c 6162  n class="nodeLab
-000034b0: 656c 223e 6761 7465 7761 793c 2f73 7061  el">gateway</spa
-000034c0: 6e3e 3c2f 6469 763e 3c2f 666f 7265 6967  n></div></foreig
-000034d0: 6e4f 626a 6563 743e 3c2f 673e 3c2f 673e  nObject></g></g>
-000034e0: 3c2f 673e 3c2f 673e 3c2f 673e 3c73 7479  </g></g></g><sty
-000034f0: 6c65 3e40 696d 706f 7274 2075 726c 2822  le>@import url("
-00003500: 6874 7470 733a 2f2f 6364 6e6a 732e 636c  https://cdnjs.cl
-00003510: 6f75 6466 6c61 7265 2e63 6f6d 2f61 6a61  oudflare.com/aja
-00003520: 782f 6c69 6273 2f66 6f6e 742d 6177 6573  x/libs/font-awes
-00003530: 6f6d 652f 352e 3135 2e32 2f63 7373 2f61  ome/5.15.2/css/a
-00003540: 6c6c 2e6d 696e 2e63 7373 2229 3b3c 2f73  ll.min.css");</s
-00003550: 7479 6c65 3e3c 2f73 7667 3e              tyle></svg>
+00000420: 6572 2d6c 6162 656c 2073 7061 6e2c 236d  er-label span,#m
+00000430: 6572 6d61 6964 2d73 7667 2070 7b63 6f6c  ermaid-svg p{col
+00000440: 6f72 3a72 6762 2830 2c20 302c 2030 293b  or:rgb(0, 0, 0);
+00000450: 7d23 6d65 726d 6169 642d 7376 6720 2e6c  }#mermaid-svg .l
+00000460: 6162 656c 2074 6578 742c 236d 6572 6d61  abel text,#merma
+00000470: 6964 2d73 7667 2073 7061 6e2c 236d 6572  id-svg span,#mer
+00000480: 6d61 6964 2d73 7667 2070 7b66 696c 6c3a  maid-svg p{fill:
+00000490: 2333 3333 3b63 6f6c 6f72 3a23 3333 333b  #333;color:#333;
+000004a0: 7d23 6d65 726d 6169 642d 7376 6720 2e6e  }#mermaid-svg .n
+000004b0: 6f64 6520 7265 6374 2c23 6d65 726d 6169  ode rect,#mermai
+000004c0: 642d 7376 6720 2e6e 6f64 6520 6369 7263  d-svg .node circ
+000004d0: 6c65 2c23 6d65 726d 6169 642d 7376 6720  le,#mermaid-svg 
+000004e0: 2e6e 6f64 6520 656c 6c69 7073 652c 236d  .node ellipse,#m
+000004f0: 6572 6d61 6964 2d73 7667 202e 6e6f 6465  ermaid-svg .node
+00000500: 2070 6f6c 7967 6f6e 2c23 6d65 726d 6169   polygon,#mermai
+00000510: 642d 7376 6720 2e6e 6f64 6520 7061 7468  d-svg .node path
+00000520: 7b66 696c 6c3a 2333 3243 3843 443b 7374  {fill:#32C8CD;st
+00000530: 726f 6b65 3a23 6666 663b 7374 726f 6b65  roke:#fff;stroke
+00000540: 2d77 6964 7468 3a31 7078 3b7d 236d 6572  -width:1px;}#mer
+00000550: 6d61 6964 2d73 7667 202e 666c 6f77 6368  maid-svg .flowch
+00000560: 6172 742d 6c61 6265 6c20 7465 7874 7b74  art-label text{t
+00000570: 6578 742d 616e 6368 6f72 3a6d 6964 646c  ext-anchor:middl
+00000580: 653b 7d23 6d65 726d 6169 642d 7376 6720  e;}#mermaid-svg 
+00000590: 2e6e 6f64 6520 2e6c 6162 656c 7b74 6578  .node .label{tex
+000005a0: 742d 616c 6967 6e3a 6365 6e74 6572 3b7d  t-align:center;}
+000005b0: 236d 6572 6d61 6964 2d73 7667 202e 6e6f  #mermaid-svg .no
+000005c0: 6465 2e63 6c69 636b 6162 6c65 7b63 7572  de.clickable{cur
+000005d0: 736f 723a 706f 696e 7465 723b 7d23 6d65  sor:pointer;}#me
+000005e0: 726d 6169 642d 7376 6720 2e61 7272 6f77  rmaid-svg .arrow
+000005f0: 6865 6164 5061 7468 7b66 696c 6c3a 2330  headPath{fill:#0
+00000600: 6230 6230 623b 7d23 6d65 726d 6169 642d  b0b0b;}#mermaid-
+00000610: 7376 6720 2e65 6467 6550 6174 6820 2e70  svg .edgePath .p
+00000620: 6174 687b 7374 726f 6b65 3a23 6136 6438  ath{stroke:#a6d8
+00000630: 6461 3b73 7472 6f6b 652d 7769 6474 683a  da;stroke-width:
+00000640: 322e 3070 783b 7d23 6d65 726d 6169 642d  2.0px;}#mermaid-
+00000650: 7376 6720 2e66 6c6f 7763 6861 7274 2d6c  svg .flowchart-l
+00000660: 696e 6b7b 7374 726f 6b65 3a23 6136 6438  ink{stroke:#a6d8
+00000670: 6461 3b66 696c 6c3a 6e6f 6e65 3b7d 236d  da;fill:none;}#m
+00000680: 6572 6d61 6964 2d73 7667 202e 6564 6765  ermaid-svg .edge
+00000690: 4c61 6265 6c7b 6261 636b 6772 6f75 6e64  Label{background
+000006a0: 2d63 6f6c 6f72 3a68 736c 282d 3132 302c  -color:hsl(-120,
+000006b0: 2030 252c 2031 3030 2529 3b74 6578 742d   0%, 100%);text-
+000006c0: 616c 6967 6e3a 6365 6e74 6572 3b7d 236d  align:center;}#m
+000006d0: 6572 6d61 6964 2d73 7667 202e 6564 6765  ermaid-svg .edge
+000006e0: 4c61 6265 6c20 7265 6374 7b6f 7061 6369  Label rect{opaci
+000006f0: 7479 3a30 2e35 3b62 6163 6b67 726f 756e  ty:0.5;backgroun
+00000700: 642d 636f 6c6f 723a 6873 6c28 2d31 3230  d-color:hsl(-120
+00000710: 2c20 3025 2c20 3130 3025 293b 6669 6c6c  , 0%, 100%);fill
+00000720: 3a68 736c 282d 3132 302c 2030 252c 2031  :hsl(-120, 0%, 1
+00000730: 3030 2529 3b7d 236d 6572 6d61 6964 2d73  00%);}#mermaid-s
+00000740: 7667 202e 6c61 6265 6c42 6b67 7b62 6163  vg .labelBkg{bac
+00000750: 6b67 726f 756e 642d 636f 6c6f 723a 7267  kground-color:rg
+00000760: 6261 2832 3535 2c20 3235 352c 2032 3535  ba(255, 255, 255
+00000770: 2c20 302e 3529 3b7d 236d 6572 6d61 6964  , 0.5);}#mermaid
+00000780: 2d73 7667 202e 636c 7573 7465 7220 7265  -svg .cluster re
+00000790: 6374 7b66 696c 6c3a 2345 4545 4445 3738  ct{fill:#EEEDE78
+000007a0: 433b 7374 726f 6b65 3a6e 6f6e 653b 7374  C;stroke:none;st
+000007b0: 726f 6b65 2d77 6964 7468 3a31 7078 3b7d  roke-width:1px;}
+000007c0: 236d 6572 6d61 6964 2d73 7667 202e 636c  #mermaid-svg .cl
+000007d0: 7573 7465 7220 7465 7874 7b66 696c 6c3a  uster text{fill:
+000007e0: 7267 6228 302c 2030 2c20 3029 3b7d 236d  rgb(0, 0, 0);}#m
+000007f0: 6572 6d61 6964 2d73 7667 202e 636c 7573  ermaid-svg .clus
+00000800: 7465 7220 7370 616e 2c23 6d65 726d 6169  ter span,#mermai
+00000810: 642d 7376 6720 707b 636f 6c6f 723a 7267  d-svg p{color:rg
+00000820: 6228 302c 2030 2c20 3029 3b7d 236d 6572  b(0, 0, 0);}#mer
+00000830: 6d61 6964 2d73 7667 2064 6976 2e6d 6572  maid-svg div.mer
+00000840: 6d61 6964 546f 6f6c 7469 707b 706f 7369  maidTooltip{posi
+00000850: 7469 6f6e 3a61 6273 6f6c 7574 653b 7465  tion:absolute;te
+00000860: 7874 2d61 6c69 676e 3a63 656e 7465 723b  xt-align:center;
+00000870: 6d61 782d 7769 6474 683a 3230 3070 783b  max-width:200px;
+00000880: 7061 6464 696e 673a 3270 783b 666f 6e74  padding:2px;font
+00000890: 2d66 616d 696c 793a 2274 7265 6275 6368  -family:"trebuch
+000008a0: 6574 206d 7322 2c76 6572 6461 6e61 2c61  et ms",verdana,a
+000008b0: 7269 616c 2c73 616e 732d 7365 7269 663b  rial,sans-serif;
+000008c0: 666f 6e74 2d73 697a 653a 3132 7078 3b62  font-size:12px;b
+000008d0: 6163 6b67 726f 756e 643a 6873 6c28 3138  ackground:hsl(18
+000008e0: 302c 2030 252c 2031 3030 2529 3b62 6f72  0, 0%, 100%);bor
+000008f0: 6465 723a 3170 7820 736f 6c69 6420 6e6f  der:1px solid no
+00000900: 6e65 3b62 6f72 6465 722d 7261 6469 7573  ne;border-radius
+00000910: 3a32 7078 3b70 6f69 6e74 6572 2d65 7665  :2px;pointer-eve
+00000920: 6e74 733a 6e6f 6e65 3b7a 2d69 6e64 6578  nts:none;z-index
+00000930: 3a31 3030 3b7d 236d 6572 6d61 6964 2d73  :100;}#mermaid-s
+00000940: 7667 202e 666c 6f77 6368 6172 7454 6974  vg .flowchartTit
+00000950: 6c65 5465 7874 7b74 6578 742d 616e 6368  leText{text-anch
+00000960: 6f72 3a6d 6964 646c 653b 666f 6e74 2d73  or:middle;font-s
+00000970: 697a 653a 3138 7078 3b66 696c 6c3a 2333  ize:18px;fill:#3
+00000980: 3333 3b7d 236d 6572 6d61 6964 2d73 7667  33;}#mermaid-svg
+00000990: 203a 726f 6f74 7b2d 2d6d 6572 6d61 6964   :root{--mermaid
+000009a0: 2d66 6f6e 742d 6661 6d69 6c79 3a22 7472  -font-family:"tr
+000009b0: 6562 7563 6865 7420 6d73 222c 7665 7264  ebuchet ms",verd
+000009c0: 616e 612c 6172 6961 6c2c 7361 6e73 2d73  ana,arial,sans-s
+000009d0: 6572 6966 3b7d 236d 6572 6d61 6964 2d73  erif;}#mermaid-s
+000009e0: 7667 202e 494e 5350 4543 5426 6774 3b2a  vg .INSPECT&gt;*
+000009f0: 7b73 7472 6f6b 653a 2346 3239 4339 4621  {stroke:#F29C9F!
+00000a00: 696d 706f 7274 616e 743b 7d23 6d65 726d  important;}#merm
+00000a10: 6169 642d 7376 6720 2e49 4e53 5045 4354  aid-svg .INSPECT
+00000a20: 2073 7061 6e7b 7374 726f 6b65 3a23 4632   span{stroke:#F2
+00000a30: 3943 3946 2169 6d70 6f72 7461 6e74 3b7d  9C9F!important;}
+00000a40: 236d 6572 6d61 6964 2d73 7667 202e 4a4f  #mermaid-svg .JO
+00000a50: 494e 5f49 4e53 5045 4354 2667 743b 2a7b  IN_INSPECT&gt;*{
+00000a60: 7374 726f 6b65 3a23 4632 3943 3946 2169  stroke:#F29C9F!i
+00000a70: 6d70 6f72 7461 6e74 3b7d 236d 6572 6d61  mportant;}#merma
+00000a80: 6964 2d73 7667 202e 4a4f 494e 5f49 4e53  id-svg .JOIN_INS
+00000a90: 5045 4354 2073 7061 6e7b 7374 726f 6b65  PECT span{stroke
+00000aa0: 3a23 4632 3943 3946 2169 6d70 6f72 7461  :#F29C9F!importa
+00000ab0: 6e74 3b7d 236d 6572 6d61 6964 2d73 7667  nt;}#mermaid-svg
+00000ac0: 202e 4741 5445 5741 5926 6774 3b2a 7b66   .GATEWAY&gt;*{f
+00000ad0: 696c 6c3a 6e6f 6e65 2169 6d70 6f72 7461  ill:none!importa
+00000ae0: 6e74 3b63 6f6c 6f72 3a23 3030 3021 696d  nt;color:#000!im
+00000af0: 706f 7274 616e 743b 7374 726f 6b65 3a6e  portant;stroke:n
+00000b00: 6f6e 6521 696d 706f 7274 616e 743b 7d23  one!important;}#
+00000b10: 6d65 726d 6169 642d 7376 6720 2e47 4154  mermaid-svg .GAT
+00000b20: 4557 4159 2073 7061 6e7b 6669 6c6c 3a6e  EWAY span{fill:n
+00000b30: 6f6e 6521 696d 706f 7274 616e 743b 636f  one!important;co
+00000b40: 6c6f 723a 2330 3030 2169 6d70 6f72 7461  lor:#000!importa
+00000b50: 6e74 3b73 7472 6f6b 653a 6e6f 6e65 2169  nt;stroke:none!i
+00000b60: 6d70 6f72 7461 6e74 3b7d 236d 6572 6d61  mportant;}#merma
+00000b70: 6964 2d73 7667 202e 4741 5445 5741 5920  id-svg .GATEWAY 
+00000b80: 7473 7061 6e7b 6669 6c6c 3a23 3030 3021  tspan{fill:#000!
+00000b90: 696d 706f 7274 616e 743b 7d23 6d65 726d  important;}#merm
+00000ba0: 6169 642d 7376 6720 2e49 4e53 5045 4354  aid-svg .INSPECT
+00000bb0: 5f41 5558 5f50 4153 5326 6774 3b2a 7b73  _AUX_PASS&gt;*{s
+00000bc0: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
+00000bd0: 3220 3221 696d 706f 7274 616e 743b 7d23  2 2!important;}#
+00000be0: 6d65 726d 6169 642d 7376 6720 2e49 4e53  mermaid-svg .INS
+00000bf0: 5045 4354 5f41 5558 5f50 4153 5320 7370  PECT_AUX_PASS sp
+00000c00: 616e 7b73 7472 6f6b 652d 6461 7368 6172  an{stroke-dashar
+00000c10: 7261 793a 3220 3221 696d 706f 7274 616e  ray:2 2!importan
+00000c20: 743b 7d23 6d65 726d 6169 642d 7376 6720  t;}#mermaid-svg 
+00000c30: 2e48 4541 4454 4149 4c26 6774 3b2a 7b66  .HEADTAIL&gt;*{f
+00000c40: 696c 6c3a 2333 3243 3843 4431 4421 696d  ill:#32C8CD1D!im
+00000c50: 706f 7274 616e 743b 7d23 6d65 726d 6169  portant;}#mermai
+00000c60: 642d 7376 6720 2e48 4541 4454 4149 4c20  d-svg .HEADTAIL 
+00000c70: 7370 616e 7b66 696c 6c3a 2333 3243 3843  span{fill:#32C8C
+00000c80: 4431 4421 696d 706f 7274 616e 743b 7d23  D1D!important;}#
+00000c90: 6d65 726d 6169 642d 7376 6720 2e45 5854  mermaid-svg .EXT
+00000ca0: 4552 4e41 4c26 6774 3b2a 7b66 696c 6c3a  ERNAL&gt;*{fill:
+00000cb0: 2366 6666 2169 6d70 6f72 7461 6e74 3b73  #fff!important;s
+00000cc0: 7472 6f6b 653a 2333 3243 3843 4421 696d  troke:#32C8CD!im
+00000cd0: 706f 7274 616e 743b 7d23 6d65 726d 6169  portant;}#mermai
+00000ce0: 642d 7376 6720 2e45 5854 4552 4e41 4c20  d-svg .EXTERNAL 
+00000cf0: 7370 616e 7b66 696c 6c3a 2366 6666 2169  span{fill:#fff!i
+00000d00: 6d70 6f72 7461 6e74 3b73 7472 6f6b 653a  mportant;stroke:
+00000d10: 2333 3243 3843 4421 696d 706f 7274 616e  #32C8CD!importan
+00000d20: 743b 7d3c 2f73 7479 6c65 3e3c 673e 3c6d  t;}</style><g><m
+00000d30: 6172 6b65 7220 6964 3d22 666c 6f77 6368  arker id="flowch
+00000d40: 6172 742d 706f 696e 7445 6e64 2220 636c  art-pointEnd" cl
+00000d50: 6173 733d 226d 6172 6b65 7220 666c 6f77  ass="marker flow
+00000d60: 6368 6172 7422 2076 6965 7742 6f78 3d22  chart" viewBox="
+00000d70: 3020 3020 3130 2031 3022 2072 6566 583d  0 0 10 10" refX=
+00000d80: 2231 3022 2072 6566 593d 2235 2220 6d61  "10" refY="5" ma
+00000d90: 726b 6572 556e 6974 733d 2275 7365 7253  rkerUnits="userS
+00000da0: 7061 6365 4f6e 5573 6522 206d 6172 6b65  paceOnUse" marke
+00000db0: 7257 6964 7468 3d22 3132 2220 6d61 726b  rWidth="12" mark
+00000dc0: 6572 4865 6967 6874 3d22 3132 2220 6f72  erHeight="12" or
+00000dd0: 6965 6e74 3d22 6175 746f 223e 3c70 6174  ient="auto"><pat
+00000de0: 6820 643d 224d 2030 2030 204c 2031 3020  h d="M 0 0 L 10 
+00000df0: 3520 4c20 3020 3130 207a 2220 636c 6173  5 L 0 10 z" clas
+00000e00: 733d 2261 7272 6f77 4d61 726b 6572 5061  s="arrowMarkerPa
+00000e10: 7468 2220 7374 796c 653d 2273 7472 6f6b  th" style="strok
+00000e20: 652d 7769 6474 683a 2031 3b20 7374 726f  e-width: 1; stro
+00000e30: 6b65 2d64 6173 6861 7272 6179 3a20 312c  ke-dasharray: 1,
+00000e40: 2030 3b22 3e3c 2f70 6174 683e 3c2f 6d61   0;"></path></ma
+00000e50: 726b 6572 3e3c 6d61 726b 6572 2069 643d  rker><marker id=
+00000e60: 2266 6c6f 7763 6861 7274 2d70 6f69 6e74  "flowchart-point
+00000e70: 5374 6172 7422 2063 6c61 7373 3d22 6d61  Start" class="ma
+00000e80: 726b 6572 2066 6c6f 7763 6861 7274 2220  rker flowchart" 
+00000e90: 7669 6577 426f 783d 2230 2030 2031 3020  viewBox="0 0 10 
+00000ea0: 3130 2220 7265 6658 3d22 3022 2072 6566  10" refX="0" ref
+00000eb0: 593d 2235 2220 6d61 726b 6572 556e 6974  Y="5" markerUnit
+00000ec0: 733d 2275 7365 7253 7061 6365 4f6e 5573  s="userSpaceOnUs
+00000ed0: 6522 206d 6172 6b65 7257 6964 7468 3d22  e" markerWidth="
+00000ee0: 3132 2220 6d61 726b 6572 4865 6967 6874  12" markerHeight
+00000ef0: 3d22 3132 2220 6f72 6965 6e74 3d22 6175  ="12" orient="au
+00000f00: 746f 223e 3c70 6174 6820 643d 224d 2030  to"><path d="M 0
+00000f10: 2035 204c 2031 3020 3130 204c 2031 3020   5 L 10 10 L 10 
+00000f20: 3020 7a22 2063 6c61 7373 3d22 6172 726f  0 z" class="arro
+00000f30: 774d 6172 6b65 7250 6174 6822 2073 7479  wMarkerPath" sty
+00000f40: 6c65 3d22 7374 726f 6b65 2d77 6964 7468  le="stroke-width
+00000f50: 3a20 313b 2073 7472 6f6b 652d 6461 7368  : 1; stroke-dash
+00000f60: 6172 7261 793a 2031 2c20 303b 223e 3c2f  array: 1, 0;"></
+00000f70: 7061 7468 3e3c 2f6d 6172 6b65 723e 3c6d  path></marker><m
+00000f80: 6172 6b65 7220 6964 3d22 666c 6f77 6368  arker id="flowch
+00000f90: 6172 742d 6369 7263 6c65 456e 6422 2063  art-circleEnd" c
+00000fa0: 6c61 7373 3d22 6d61 726b 6572 2066 6c6f  lass="marker flo
+00000fb0: 7763 6861 7274 2220 7669 6577 426f 783d  wchart" viewBox=
+00000fc0: 2230 2030 2031 3020 3130 2220 7265 6658  "0 0 10 10" refX
+00000fd0: 3d22 3131 2220 7265 6659 3d22 3522 206d  ="11" refY="5" m
+00000fe0: 6172 6b65 7255 6e69 7473 3d22 7573 6572  arkerUnits="user
+00000ff0: 5370 6163 654f 6e55 7365 2220 6d61 726b  SpaceOnUse" mark
+00001000: 6572 5769 6474 683d 2231 3122 206d 6172  erWidth="11" mar
+00001010: 6b65 7248 6569 6768 743d 2231 3122 206f  kerHeight="11" o
+00001020: 7269 656e 743d 2261 7574 6f22 3e3c 6369  rient="auto"><ci
+00001030: 7263 6c65 2063 783d 2235 2220 6379 3d22  rcle cx="5" cy="
+00001040: 3522 2072 3d22 3522 2063 6c61 7373 3d22  5" r="5" class="
+00001050: 6172 726f 774d 6172 6b65 7250 6174 6822  arrowMarkerPath"
+00001060: 2073 7479 6c65 3d22 7374 726f 6b65 2d77   style="stroke-w
+00001070: 6964 7468 3a20 313b 2073 7472 6f6b 652d  idth: 1; stroke-
+00001080: 6461 7368 6172 7261 793a 2031 2c20 303b  dasharray: 1, 0;
+00001090: 223e 3c2f 6369 7263 6c65 3e3c 2f6d 6172  "></circle></mar
+000010a0: 6b65 723e 3c6d 6172 6b65 7220 6964 3d22  ker><marker id="
+000010b0: 666c 6f77 6368 6172 742d 6369 7263 6c65  flowchart-circle
+000010c0: 5374 6172 7422 2063 6c61 7373 3d22 6d61  Start" class="ma
+000010d0: 726b 6572 2066 6c6f 7763 6861 7274 2220  rker flowchart" 
+000010e0: 7669 6577 426f 783d 2230 2030 2031 3020  viewBox="0 0 10 
+000010f0: 3130 2220 7265 6658 3d22 2d31 2220 7265  10" refX="-1" re
+00001100: 6659 3d22 3522 206d 6172 6b65 7255 6e69  fY="5" markerUni
+00001110: 7473 3d22 7573 6572 5370 6163 654f 6e55  ts="userSpaceOnU
+00001120: 7365 2220 6d61 726b 6572 5769 6474 683d  se" markerWidth=
+00001130: 2231 3122 206d 6172 6b65 7248 6569 6768  "11" markerHeigh
+00001140: 743d 2231 3122 206f 7269 656e 743d 2261  t="11" orient="a
+00001150: 7574 6f22 3e3c 6369 7263 6c65 2063 783d  uto"><circle cx=
+00001160: 2235 2220 6379 3d22 3522 2072 3d22 3522  "5" cy="5" r="5"
+00001170: 2063 6c61 7373 3d22 6172 726f 774d 6172   class="arrowMar
+00001180: 6b65 7250 6174 6822 2073 7479 6c65 3d22  kerPath" style="
+00001190: 7374 726f 6b65 2d77 6964 7468 3a20 313b  stroke-width: 1;
+000011a0: 2073 7472 6f6b 652d 6461 7368 6172 7261   stroke-dasharra
+000011b0: 793a 2031 2c20 303b 223e 3c2f 6369 7263  y: 1, 0;"></circ
+000011c0: 6c65 3e3c 2f6d 6172 6b65 723e 3c6d 6172  le></marker><mar
+000011d0: 6b65 7220 6964 3d22 666c 6f77 6368 6172  ker id="flowchar
+000011e0: 742d 6372 6f73 7345 6e64 2220 636c 6173  t-crossEnd" clas
+000011f0: 733d 226d 6172 6b65 7220 6372 6f73 7320  s="marker cross 
+00001200: 666c 6f77 6368 6172 7422 2076 6965 7742  flowchart" viewB
+00001210: 6f78 3d22 3020 3020 3131 2031 3122 2072  ox="0 0 11 11" r
+00001220: 6566 583d 2231 3222 2072 6566 593d 2235  efX="12" refY="5
+00001230: 2e32 2220 6d61 726b 6572 556e 6974 733d  .2" markerUnits=
+00001240: 2275 7365 7253 7061 6365 4f6e 5573 6522  "userSpaceOnUse"
+00001250: 206d 6172 6b65 7257 6964 7468 3d22 3131   markerWidth="11
+00001260: 2220 6d61 726b 6572 4865 6967 6874 3d22  " markerHeight="
+00001270: 3131 2220 6f72 6965 6e74 3d22 6175 746f  11" orient="auto
+00001280: 223e 3c70 6174 6820 643d 224d 2031 2c31  "><path d="M 1,1
+00001290: 206c 2039 2c39 204d 2031 302c 3120 6c20   l 9,9 M 10,1 l 
+000012a0: 2d39 2c39 2220 636c 6173 733d 2261 7272  -9,9" class="arr
+000012b0: 6f77 4d61 726b 6572 5061 7468 2220 7374  owMarkerPath" st
+000012c0: 796c 653d 2273 7472 6f6b 652d 7769 6474  yle="stroke-widt
+000012d0: 683a 2032 3b20 7374 726f 6b65 2d64 6173  h: 2; stroke-das
+000012e0: 6861 7272 6179 3a20 312c 2030 3b22 3e3c  harray: 1, 0;"><
+000012f0: 2f70 6174 683e 3c2f 6d61 726b 6572 3e3c  /path></marker><
+00001300: 6d61 726b 6572 2069 643d 2266 6c6f 7763  marker id="flowc
+00001310: 6861 7274 2d63 726f 7373 5374 6172 7422  hart-crossStart"
+00001320: 2063 6c61 7373 3d22 6d61 726b 6572 2063   class="marker c
+00001330: 726f 7373 2066 6c6f 7763 6861 7274 2220  ross flowchart" 
+00001340: 7669 6577 426f 783d 2230 2030 2031 3120  viewBox="0 0 11 
+00001350: 3131 2220 7265 6658 3d22 2d31 2220 7265  11" refX="-1" re
+00001360: 6659 3d22 352e 3222 206d 6172 6b65 7255  fY="5.2" markerU
+00001370: 6e69 7473 3d22 7573 6572 5370 6163 654f  nits="userSpaceO
+00001380: 6e55 7365 2220 6d61 726b 6572 5769 6474  nUse" markerWidt
+00001390: 683d 2231 3122 206d 6172 6b65 7248 6569  h="11" markerHei
+000013a0: 6768 743d 2231 3122 206f 7269 656e 743d  ght="11" orient=
+000013b0: 2261 7574 6f22 3e3c 7061 7468 2064 3d22  "auto"><path d="
+000013c0: 4d20 312c 3120 6c20 392c 3920 4d20 3130  M 1,1 l 9,9 M 10
+000013d0: 2c31 206c 202d 392c 3922 2063 6c61 7373  ,1 l -9,9" class
+000013e0: 3d22 6172 726f 774d 6172 6b65 7250 6174  ="arrowMarkerPat
+000013f0: 6822 2073 7479 6c65 3d22 7374 726f 6b65  h" style="stroke
+00001400: 2d77 6964 7468 3a20 323b 2073 7472 6f6b  -width: 2; strok
+00001410: 652d 6461 7368 6172 7261 793a 2031 2c20  e-dasharray: 1, 
+00001420: 303b 223e 3c2f 7061 7468 3e3c 2f6d 6172  0;"></path></mar
+00001430: 6b65 723e 3c67 2063 6c61 7373 3d22 726f  ker><g class="ro
+00001440: 6f74 223e 3c67 2063 6c61 7373 3d22 636c  ot"><g class="cl
+00001450: 7573 7465 7273 223e 3c2f 673e 3c67 2063  usters"></g><g c
+00001460: 6c61 7373 3d22 6564 6765 5061 7468 7322  lass="edgePaths"
+00001470: 3e3c 7061 7468 2064 3d22 4d37 342e 3731  ><path d="M74.71
+00001480: 3837 352c 3132 394c 3738 2e38 3835 3431  875,129L78.88541
+00001490: 3636 3636 3636 3636 372c 3132 3943 3833  666666667,129C83
+000014a0: 2e30 3532 3038 3333 3333 3333 3333 332c  .05208333333333,
+000014b0: 3132 392c 3931 2e33 3835 3431 3636 3636  129,91.385416666
+000014c0: 3636 3636 372c 3132 392c 3939 2e37 3138  66667,129,99.718
+000014d0: 3735 2c31 3239 4331 3038 2e30 3532 3038  75,129C108.05208
+000014e0: 3333 3333 3333 3333 332c 3132 392c 3131  333333333,129,11
+000014f0: 362e 3338 3534 3136 3636 3636 3636 3637  6.38541666666667
+00001500: 2c31 3239 2c31 3230 2e35 3532 3038 3333  ,129,120.5520833
+00001510: 3333 3333 3333 332c 3132 394c 3132 342e  3333333,129L124.
+00001520: 3731 3837 352c 3132 3922 2069 643d 224c  71875,129" id="L
+00001530: 2d67 6174 6577 6179 7374 6172 742d 452d  -gatewaystart-E-
+00001540: 3022 2063 6c61 7373 3d22 2065 6467 652d  0" class=" edge-
+00001550: 7468 6963 6b6e 6573 732d 6e6f 726d 616c  thickness-normal
+00001560: 2065 6467 652d 7061 7474 6572 6e2d 736f   edge-pattern-so
+00001570: 6c69 6420 666c 6f77 6368 6172 742d 6c69  lid flowchart-li
+00001580: 6e6b 204c 532d 6761 7465 7761 7973 7461  nk LS-gatewaysta
+00001590: 7274 204c 452d 4522 2073 7479 6c65 3d22  rt LE-E" style="
+000015a0: 6669 6c6c 3a6e 6f6e 653b 2220 6d61 726b  fill:none;" mark
+000015b0: 6572 2d65 6e64 3d22 7572 6c28 2366 6c6f  er-end="url(#flo
+000015c0: 7763 6861 7274 2d70 6f69 6e74 456e 6429  wchart-pointEnd)
+000015d0: 223e 3c2f 7061 7468 3e3c 7061 7468 2064  "></path><path d
+000015e0: 3d22 4d31 3938 2e32 3936 3837 352c 3137  ="M198.296875,17
+000015f0: 342e 3834 3536 3138 3931 3531 3539 3935  4.84561891515995
+00001600: 4c32 3032 2e34 3633 3534 3136 3636 3636  L202.46354166666
+00001610: 3636 362c 3138 302e 3033 3830 3135 3736  666,180.03801576
+00001620: 3236 3333 3343 3230 362e 3633 3032 3038  26333C206.630208
+00001630: 3333 3333 3333 3334 2c31 3835 2e32 3330  33333334,185.230
+00001640: 3431 3236 3130 3130 3636 342c 3231 342e  41261010664,214.
+00001650: 3936 3335 3431 3636 3636 3636 3636 2c31  96354166666666,1
+00001660: 3935 2e36 3135 3230 3633 3035 3035 3333  95.6152063050533
+00001670: 332c 3232 332e 3239 3638 3735 2c32 3030  3,223.296875,200
+00001680: 2e38 3037 3630 3331 3532 3532 3636 3743  .80760315252667C
+00001690: 3233 312e 3633 3032 3038 3333 3333 3333  231.630208333333
+000016a0: 3334 2c32 3036 2c32 3339 2e39 3633 3534  34,206,239.96354
+000016b0: 3136 3636 3636 3636 362c 3230 362c 3234  166666666,206,24
+000016c0: 342e 3133 3032 3038 3333 3333 3333 3334  4.13020833333334
+000016d0: 2c32 3036 4c32 3438 2e32 3936 3837 352c  ,206L248.296875,
+000016e0: 3230 3622 2069 643d 224c 2d45 2d45 452d  206" id="L-E-EE-
+000016f0: 3022 2063 6c61 7373 3d22 2065 6467 652d  0" class=" edge-
+00001700: 7468 6963 6b6e 6573 732d 6e6f 726d 616c  thickness-normal
+00001710: 2065 6467 652d 7061 7474 6572 6e2d 736f   edge-pattern-so
+00001720: 6c69 6420 666c 6f77 6368 6172 742d 6c69  lid flowchart-li
+00001730: 6e6b 204c 532d 4520 4c45 2d45 4522 2073  nk LS-E LE-EE" s
+00001740: 7479 6c65 3d22 6669 6c6c 3a6e 6f6e 653b  tyle="fill:none;
+00001750: 2220 6d61 726b 6572 2d65 6e64 3d22 7572  " marker-end="ur
+00001760: 6c28 2366 6c6f 7763 6861 7274 2d70 6f69  l(#flowchart-poi
+00001770: 6e74 456e 6429 223e 3c2f 7061 7468 3e3c  ntEnd)"></path><
+00001780: 7061 7468 2064 3d22 4d31 3938 2e32 3936  path d="M198.296
+00001790: 3837 352c 3833 2e31 3534 3338 3130 3834  875,83.154381084
+000017a0: 3834 3030 354c 3230 322e 3436 3335 3431  84005L202.463541
+000017b0: 3636 3636 3636 3636 2c37 372e 3936 3139  66666666,77.9619
+000017c0: 3834 3233 3733 3636 3743 3230 362e 3633  842373667C206.63
+000017d0: 3032 3038 3333 3333 3333 3334 2c37 322e  020833333334,72.
+000017e0: 3736 3935 3837 3338 3938 3933 3337 2c32  76958738989337,2
+000017f0: 3134 2e39 3633 3534 3136 3636 3636 3636  14.9635416666666
+00001800: 362c 3632 2e33 3834 3739 3336 3934 3934  6,62.38479369494
+00001810: 3636 392c 3232 332e 3331 3131 3937 3931  669,223.31119791
+00001820: 3636 3636 3636 2c35 372e 3139 3233 3936  666666,57.192396
+00001830: 3834 3734 3733 3334 4332 3331 2e36 3538  84747334C231.658
+00001840: 3835 3431 3636 3636 3636 362c 3532 2c32  85416666666,52,2
+00001850: 3430 2e30 3230 3833 3333 3333 3333 3333  40.0208333333333
+00001860: 342c 3532 2c32 3434 2e32 3031 3832 3239  4,52,244.2018229
+00001870: 3136 3636 3636 362c 3532 4c32 3438 2e33  1666666,52L248.3
+00001880: 3832 3831 3235 2c35 3222 2069 643d 224c  828125,52" id="L
+00001890: 2d45 2d65 7865 6375 746f 7232 2d30 2220  -E-executor2-0" 
+000018a0: 636c 6173 733d 2220 6564 6765 2d74 6869  class=" edge-thi
+000018b0: 636b 6e65 7373 2d6e 6f72 6d61 6c20 6564  ckness-normal ed
+000018c0: 6765 2d70 6174 7465 726e 2d73 6f6c 6964  ge-pattern-solid
+000018d0: 2066 6c6f 7763 6861 7274 2d6c 696e 6b20   flowchart-link 
+000018e0: 4c53 2d45 204c 452d 6578 6563 7574 6f72  LS-E LE-executor
+000018f0: 3222 2073 7479 6c65 3d22 6669 6c6c 3a6e  2" style="fill:n
+00001900: 6f6e 653b 2220 6d61 726b 6572 2d65 6e64  one;" marker-end
+00001910: 3d22 7572 6c28 2366 6c6f 7763 6861 7274  ="url(#flowchart
+00001920: 2d70 6f69 6e74 456e 6429 223e 3c2f 7061  -pointEnd)"></pa
+00001930: 7468 3e3c 7061 7468 2064 3d22 4d33 3330  th><path d="M330
+00001940: 2e34 3337 352c 3230 364c 3333 342e 3630  .4375,206L334.60
+00001950: 3431 3636 3636 3636 3636 372c 3230 3643  41666666667,206C
+00001960: 3333 382e 3737 3038 3333 3333 3333 3333  338.770833333333
+00001970: 332c 3230 362c 3334 372e 3130 3431 3636  3,206,347.104166
+00001980: 3636 3636 3636 372c 3230 362c 3335 352e  6666667,206,355.
+00001990: 3433 3735 2c32 3036 4333 3633 2e37 3730  4375,206C363.770
+000019a0: 3833 3333 3333 3333 3333 2c32 3036 2c33  8333333333,206,3
+000019b0: 3732 2e31 3034 3136 3636 3636 3636 3637  72.1041666666667
+000019c0: 2c32 3036 2c33 3736 2e32 3730 3833 3333  ,206,376.2708333
+000019d0: 3333 3333 3333 2c32 3036 4c33 3830 2e34  333333,206L380.4
+000019e0: 3337 352c 3230 3622 2069 643d 224c 2d45  375,206" id="L-E
+000019f0: 452d 6578 6563 7574 6f72 332d 3022 2063  E-executor3-0" c
+00001a00: 6c61 7373 3d22 2065 6467 652d 7468 6963  lass=" edge-thic
+00001a10: 6b6e 6573 732d 6e6f 726d 616c 2065 6467  kness-normal edg
+00001a20: 652d 7061 7474 6572 6e2d 736f 6c69 6420  e-pattern-solid 
+00001a30: 666c 6f77 6368 6172 742d 6c69 6e6b 204c  flowchart-link L
+00001a40: 532d 4545 204c 452d 6578 6563 7574 6f72  S-EE LE-executor
+00001a50: 3322 2073 7479 6c65 3d22 6669 6c6c 3a6e  3" style="fill:n
+00001a60: 6f6e 653b 2220 6d61 726b 6572 2d65 6e64  one;" marker-end
+00001a70: 3d22 7572 6c28 2366 6c6f 7763 6861 7274  ="url(#flowchart
+00001a80: 2d70 6f69 6e74 456e 6429 223e 3c2f 7061  -pointEnd)"></pa
+00001a90: 7468 3e3c 7061 7468 2064 3d22 4d34 3632  th><path d="M462
+00001aa0: 2e34 3036 3235 2c32 3036 4c34 3636 2e35  .40625,206L466.5
+00001ab0: 3732 3931 3636 3636 3636 3637 2c32 3036  729166666667,206
+00001ac0: 4334 3730 2e37 3339 3538 3333 3333 3333  C470.73958333333
+00001ad0: 3333 2c32 3036 2c34 3739 2e30 3732 3931  33,206,479.07291
+00001ae0: 3636 3636 3636 3637 2c32 3036 2c34 3837  66666667,206,487
+00001af0: 2e34 3036 3235 2c32 3036 4334 3935 2e37  .40625,206C495.7
+00001b00: 3339 3538 3333 3333 3333 3333 2c32 3036  395833333333,206
+00001b10: 2c35 3034 2e30 3732 3931 3636 3636 3636  ,504.07291666666
+00001b20: 3637 2c32 3036 2c35 3038 2e32 3339 3538  67,206,508.23958
+00001b30: 3333 3333 3333 3333 2c32 3036 4c35 3132  33333333,206L512
+00001b40: 2e34 3036 3235 2c32 3036 2220 6964 3d22  .40625,206" id="
+00001b50: 4c2d 6578 6563 7574 6f72 332d 6761 7465  L-executor3-gate
+00001b60: 7761 7965 6e64 2d30 2220 636c 6173 733d  wayend-0" class=
+00001b70: 2220 6564 6765 2d74 6869 636b 6e65 7373  " edge-thickness
+00001b80: 2d6e 6f72 6d61 6c20 6564 6765 2d70 6174  -normal edge-pat
+00001b90: 7465 726e 2d73 6f6c 6964 2066 6c6f 7763  tern-solid flowc
+00001ba0: 6861 7274 2d6c 696e 6b20 4c53 2d65 7865  hart-link LS-exe
+00001bb0: 6375 746f 7233 204c 452d 6761 7465 7761  cutor3 LE-gatewa
+00001bc0: 7965 6e64 2220 7374 796c 653d 2266 696c  yend" style="fil
+00001bd0: 6c3a 6e6f 6e65 3b22 206d 6172 6b65 722d  l:none;" marker-
+00001be0: 656e 643d 2275 726c 2823 666c 6f77 6368  end="url(#flowch
+00001bf0: 6172 742d 706f 696e 7445 6e64 2922 3e3c  art-pointEnd)"><
+00001c00: 2f70 6174 683e 3c2f 673e 3c67 2063 6c61  /path></g><g cla
+00001c10: 7373 3d22 6564 6765 4c61 6265 6c73 223e  ss="edgeLabels">
+00001c20: 3c67 2063 6c61 7373 3d22 6564 6765 4c61  <g class="edgeLa
+00001c30: 6265 6c22 3e3c 6720 636c 6173 733d 226c  bel"><g class="l
+00001c40: 6162 656c 2220 7472 616e 7366 6f72 6d3d  abel" transform=
+00001c50: 2274 7261 6e73 6c61 7465 2830 2c20 3029  "translate(0, 0)
+00001c60: 223e 3c66 6f72 6569 676e 4f62 6a65 6374  "><foreignObject
+00001c70: 2077 6964 7468 3d22 3022 2068 6569 6768   width="0" heigh
+00001c80: 743d 2230 223e 3c64 6976 2078 6d6c 6e73  t="0"><div xmlns
+00001c90: 3d22 6874 7470 3a2f 2f77 7777 2e77 332e  ="http://www.w3.
+00001ca0: 6f72 672f 3139 3939 2f78 6874 6d6c 2220  org/1999/xhtml" 
+00001cb0: 7374 796c 653d 2264 6973 706c 6179 3a20  style="display: 
+00001cc0: 696e 6c69 6e65 2d62 6c6f 636b 3b20 7768  inline-block; wh
+00001cd0: 6974 652d 7370 6163 653a 206e 6f77 7261  ite-space: nowra
+00001ce0: 703b 223e 3c73 7061 6e20 636c 6173 733d  p;"><span class=
+00001cf0: 2265 6467 654c 6162 656c 223e 3c2f 7370  "edgeLabel"></sp
+00001d00: 616e 3e3c 2f64 6976 3e3c 2f66 6f72 6569  an></div></forei
+00001d10: 676e 4f62 6a65 6374 3e3c 2f67 3e3c 2f67  gnObject></g></g
+00001d20: 3e3c 6720 636c 6173 733d 2265 6467 654c  ><g class="edgeL
+00001d30: 6162 656c 223e 3c67 2063 6c61 7373 3d22  abel"><g class="
+00001d40: 6c61 6265 6c22 2074 7261 6e73 666f 726d  label" transform
+00001d50: 3d22 7472 616e 736c 6174 6528 302c 2030  ="translate(0, 0
+00001d60: 2922 3e3c 666f 7265 6967 6e4f 626a 6563  )"><foreignObjec
+00001d70: 7420 7769 6474 683d 2230 2220 6865 6967  t width="0" heig
+00001d80: 6874 3d22 3022 3e3c 6469 7620 786d 6c6e  ht="0"><div xmln
+00001d90: 733d 2268 7474 703a 2f2f 7777 772e 7733  s="http://www.w3
+00001da0: 2e6f 7267 2f31 3939 392f 7868 746d 6c22  .org/1999/xhtml"
+00001db0: 2073 7479 6c65 3d22 6469 7370 6c61 793a   style="display:
+00001dc0: 2069 6e6c 696e 652d 626c 6f63 6b3b 2077   inline-block; w
+00001dd0: 6869 7465 2d73 7061 6365 3a20 6e6f 7772  hite-space: nowr
+00001de0: 6170 3b22 3e3c 7370 616e 2063 6c61 7373  ap;"><span class
+00001df0: 3d22 6564 6765 4c61 6265 6c22 3e3c 2f73  ="edgeLabel"></s
+00001e00: 7061 6e3e 3c2f 6469 763e 3c2f 666f 7265  pan></div></fore
+00001e10: 6967 6e4f 626a 6563 743e 3c2f 673e 3c2f  ignObject></g></
+00001e20: 673e 3c67 2063 6c61 7373 3d22 6564 6765  g><g class="edge
+00001e30: 4c61 6265 6c22 3e3c 6720 636c 6173 733d  Label"><g class=
+00001e40: 226c 6162 656c 2220 7472 616e 7366 6f72  "label" transfor
+00001e50: 6d3d 2274 7261 6e73 6c61 7465 2830 2c20  m="translate(0, 
+00001e60: 3029 223e 3c66 6f72 6569 676e 4f62 6a65  0)"><foreignObje
+00001e70: 6374 2077 6964 7468 3d22 3022 2068 6569  ct width="0" hei
+00001e80: 6768 743d 2230 223e 3c64 6976 2078 6d6c  ght="0"><div xml
+00001e90: 6e73 3d22 6874 7470 3a2f 2f77 7777 2e77  ns="http://www.w
+00001ea0: 332e 6f72 672f 3139 3939 2f78 6874 6d6c  3.org/1999/xhtml
+00001eb0: 2220 7374 796c 653d 2264 6973 706c 6179  " style="display
+00001ec0: 3a20 696e 6c69 6e65 2d62 6c6f 636b 3b20  : inline-block; 
+00001ed0: 7768 6974 652d 7370 6163 653a 206e 6f77  white-space: now
+00001ee0: 7261 703b 223e 3c73 7061 6e20 636c 6173  rap;"><span clas
+00001ef0: 733d 2265 6467 654c 6162 656c 223e 3c2f  s="edgeLabel"></
+00001f00: 7370 616e 3e3c 2f64 6976 3e3c 2f66 6f72  span></div></for
+00001f10: 6569 676e 4f62 6a65 6374 3e3c 2f67 3e3c  eignObject></g><
+00001f20: 2f67 3e3c 6720 636c 6173 733d 2265 6467  /g><g class="edg
+00001f30: 654c 6162 656c 223e 3c67 2063 6c61 7373  eLabel"><g class
+00001f40: 3d22 6c61 6265 6c22 2074 7261 6e73 666f  ="label" transfo
+00001f50: 726d 3d22 7472 616e 736c 6174 6528 302c  rm="translate(0,
+00001f60: 2030 2922 3e3c 666f 7265 6967 6e4f 626a   0)"><foreignObj
+00001f70: 6563 7420 7769 6474 683d 2230 2220 6865  ect width="0" he
+00001f80: 6967 6874 3d22 3022 3e3c 6469 7620 786d  ight="0"><div xm
+00001f90: 6c6e 733d 2268 7474 703a 2f2f 7777 772e  lns="http://www.
+00001fa0: 7733 2e6f 7267 2f31 3939 392f 7868 746d  w3.org/1999/xhtm
+00001fb0: 6c22 2073 7479 6c65 3d22 6469 7370 6c61  l" style="displa
+00001fc0: 793a 2069 6e6c 696e 652d 626c 6f63 6b3b  y: inline-block;
+00001fd0: 2077 6869 7465 2d73 7061 6365 3a20 6e6f   white-space: no
+00001fe0: 7772 6170 3b22 3e3c 7370 616e 2063 6c61  wrap;"><span cla
+00001ff0: 7373 3d22 6564 6765 4c61 6265 6c22 3e3c  ss="edgeLabel"><
+00002000: 2f73 7061 6e3e 3c2f 6469 763e 3c2f 666f  /span></div></fo
+00002010: 7265 6967 6e4f 626a 6563 743e 3c2f 673e  reignObject></g>
+00002020: 3c2f 673e 3c67 2063 6c61 7373 3d22 6564  </g><g class="ed
+00002030: 6765 4c61 6265 6c22 3e3c 6720 636c 6173  geLabel"><g clas
+00002040: 733d 226c 6162 656c 2220 7472 616e 7366  s="label" transf
+00002050: 6f72 6d3d 2274 7261 6e73 6c61 7465 2830  orm="translate(0
+00002060: 2c20 3029 223e 3c66 6f72 6569 676e 4f62  , 0)"><foreignOb
+00002070: 6a65 6374 2077 6964 7468 3d22 3022 2068  ject width="0" h
+00002080: 6569 6768 743d 2230 223e 3c64 6976 2078  eight="0"><div x
+00002090: 6d6c 6e73 3d22 6874 7470 3a2f 2f77 7777  mlns="http://www
+000020a0: 2e77 332e 6f72 672f 3139 3939 2f78 6874  .w3.org/1999/xht
+000020b0: 6d6c 2220 7374 796c 653d 2264 6973 706c  ml" style="displ
+000020c0: 6179 3a20 696e 6c69 6e65 2d62 6c6f 636b  ay: inline-block
+000020d0: 3b20 7768 6974 652d 7370 6163 653a 206e  ; white-space: n
+000020e0: 6f77 7261 703b 223e 3c73 7061 6e20 636c  owrap;"><span cl
+000020f0: 6173 733d 2265 6467 654c 6162 656c 223e  ass="edgeLabel">
+00002100: 3c2f 7370 616e 3e3c 2f64 6976 3e3c 2f66  </span></div></f
+00002110: 6f72 6569 676e 4f62 6a65 6374 3e3c 2f67  oreignObject></g
+00002120: 3e3c 2f67 3e3c 2f67 3e3c 6720 636c 6173  ></g></g><g clas
+00002130: 733d 226e 6f64 6573 223e 3c67 2063 6c61  s="nodes"><g cla
+00002140: 7373 3d22 726f 6f74 2220 7472 616e 7366  ss="root" transf
+00002150: 6f72 6d3d 2274 7261 6e73 6c61 7465 2833  orm="translate(3
+00002160: 3732 2e39 3337 352c 2031 3436 2922 3e3c  72.9375, 146)"><
+00002170: 6720 636c 6173 733d 2263 6c75 7374 6572  g class="cluster
+00002180: 7322 3e3c 6720 636c 6173 733d 2263 6c75  s"><g class="clu
+00002190: 7374 6572 2044 4550 4c4f 594d 454e 5420  ster DEPLOYMENT 
+000021a0: 4445 504c 4f59 4d45 4e54 2044 4550 4c4f  DEPLOYMENT DEPLO
+000021b0: 594d 454e 5420 4445 504c 4f59 4d45 4e54  YMENT DEPLOYMENT
+000021c0: 2066 6c6f 7763 6861 7274 2d6c 6162 656c   flowchart-label
+000021d0: 2220 6964 3d22 6578 6563 7574 6f72 3322  " id="executor3"
+000021e0: 3e3c 7265 6374 2073 7479 6c65 3d22 2220  ><rect style="" 
+000021f0: 7278 3d22 3022 2072 793d 2230 2220 783d  rx="0" ry="0" x=
+00002200: 2238 2220 793d 2238 2220 7769 6474 683d  "8" y="8" width=
+00002210: 2238 312e 3936 3837 3522 2068 6569 6768  "81.96875" heigh
+00002220: 743d 2231 3034 223e 3c2f 7265 6374 3e3c  t="104"></rect><
+00002230: 6720 636c 6173 733d 2263 6c75 7374 6572  g class="cluster
+00002240: 2d6c 6162 656c 2220 7472 616e 7366 6f72  -label" transfor
+00002250: 6d3d 2274 7261 6e73 6c61 7465 2831 332e  m="translate(13.
+00002260: 3134 3834 3337 352c 2038 2922 3e3c 666f  1484375, 8)"><fo
+00002270: 7265 6967 6e4f 626a 6563 7420 7769 6474  reignObject widt
+00002280: 683d 2237 312e 3637 3138 3735 2220 6865  h="71.671875" he
+00002290: 6967 6874 3d22 3139 223e 3c64 6976 2078  ight="19"><div x
+000022a0: 6d6c 6e73 3d22 6874 7470 3a2f 2f77 7777  mlns="http://www
+000022b0: 2e77 332e 6f72 672f 3139 3939 2f78 6874  .w3.org/1999/xht
+000022c0: 6d6c 2220 7374 796c 653d 2264 6973 706c  ml" style="displ
+000022d0: 6179 3a20 696e 6c69 6e65 2d62 6c6f 636b  ay: inline-block
+000022e0: 3b20 7768 6974 652d 7370 6163 653a 206e  ; white-space: n
+000022f0: 6f77 7261 703b 223e 3c73 7061 6e20 636c  owrap;"><span cl
+00002300: 6173 733d 226e 6f64 654c 6162 656c 223e  ass="nodeLabel">
+00002310: 6578 6563 7574 6f72 333c 2f73 7061 6e3e  executor3</span>
+00002320: 3c2f 6469 763e 3c2f 666f 7265 6967 6e4f  </div></foreignO
+00002330: 626a 6563 743e 3c2f 673e 3c2f 673e 3c2f  bject></g></g></
+00002340: 673e 3c67 2063 6c61 7373 3d22 6564 6765  g><g class="edge
+00002350: 5061 7468 7322 3e3c 2f67 3e3c 6720 636c  Paths"></g><g cl
+00002360: 6173 733d 2265 6467 654c 6162 656c 7322  ass="edgeLabels"
+00002370: 3e3c 2f67 3e3c 6720 636c 6173 733d 226e  ></g><g class="n
+00002380: 6f64 6573 223e 3c67 2063 6c61 7373 3d22  odes"><g class="
+00002390: 6e6f 6465 2064 6566 6175 6c74 2070 6f64  node default pod
+000023a0: 2066 6c6f 7763 6861 7274 2d6c 6162 656c   flowchart-label
+000023b0: 2220 6964 3d22 666c 6f77 6368 6172 742d  " id="flowchart-
+000023c0: 6578 6563 7574 6f72 332f 7265 702d 302d  executor3/rep-0-
+000023d0: 3331 2220 7472 616e 7366 6f72 6d3d 2274  31" transform="t
+000023e0: 7261 6e73 6c61 7465 2834 382e 3938 3433  ranslate(48.9843
+000023f0: 3735 2c20 3630 2922 3e3c 7265 6374 2063  75, 60)"><rect c
+00002400: 6c61 7373 3d22 6261 7369 6320 6c61 6265  lass="basic labe
+00002410: 6c2d 636f 6e74 6169 6e65 7222 2073 7479  l-container" sty
+00002420: 6c65 3d22 2220 7278 3d22 3022 2072 793d  le="" rx="0" ry=
+00002430: 2230 2220 783d 222d 3135 2e39 3834 3337  "0" x="-15.98437
+00002440: 3522 2079 3d22 2d31 3722 2077 6964 7468  5" y="-17" width
+00002450: 3d22 3331 2e39 3638 3735 2220 6865 6967  ="31.96875" heig
+00002460: 6874 3d22 3334 223e 3c2f 7265 6374 3e3c  ht="34"></rect><
+00002470: 6720 636c 6173 733d 226c 6162 656c 2220  g class="label" 
+00002480: 7374 796c 653d 2222 2074 7261 6e73 666f  style="" transfo
+00002490: 726d 3d22 7472 616e 736c 6174 6528 2d38  rm="translate(-8
+000024a0: 2e34 3834 3337 352c 202d 392e 3529 223e  .484375, -9.5)">
+000024b0: 3c72 6563 743e 3c2f 7265 6374 3e3c 666f  <rect></rect><fo
+000024c0: 7265 6967 6e4f 626a 6563 7420 7769 6474  reignObject widt
+000024d0: 683d 2231 362e 3936 3837 3522 2068 6569  h="16.96875" hei
+000024e0: 6768 743d 2231 3922 3e3c 6469 7620 786d  ght="19"><div xm
+000024f0: 6c6e 733d 2268 7474 703a 2f2f 7777 772e  lns="http://www.
+00002500: 7733 2e6f 7267 2f31 3939 392f 7868 746d  w3.org/1999/xhtm
+00002510: 6c22 2073 7479 6c65 3d22 6469 7370 6c61  l" style="displa
+00002520: 793a 2069 6e6c 696e 652d 626c 6f63 6b3b  y: inline-block;
+00002530: 2077 6869 7465 2d73 7061 6365 3a20 6e6f   white-space: no
+00002540: 7772 6170 3b22 3e3c 7370 616e 2063 6c61  wrap;"><span cla
+00002550: 7373 3d22 6e6f 6465 4c61 6265 6c22 3e45  ss="nodeLabel">E
+00002560: 323c 2f73 7061 6e3e 3c2f 6469 763e 3c2f  2</span></div></
+00002570: 666f 7265 6967 6e4f 626a 6563 743e 3c2f  foreignObject></
+00002580: 673e 3c2f 673e 3c2f 673e 3c2f 673e 3c67  g></g></g></g><g
+00002590: 2063 6c61 7373 3d22 726f 6f74 2220 7472   class="root" tr
+000025a0: 616e 7366 6f72 6d3d 2274 7261 6e73 6c61  ansform="transla
+000025b0: 7465 2832 3430 2e38 3832 3831 3235 2c20  te(240.8828125, 
+000025c0: 2d38 2922 3e3c 6720 636c 6173 733d 2263  -8)"><g class="c
+000025d0: 6c75 7374 6572 7322 3e3c 6720 636c 6173  lusters"><g clas
+000025e0: 733d 2263 6c75 7374 6572 2044 4550 4c4f  s="cluster DEPLO
+000025f0: 594d 454e 5420 4445 504c 4f59 4d45 4e54  YMENT DEPLOYMENT
+00002600: 2066 6c6f 7763 6861 7274 2d6c 6162 656c   flowchart-label
+00002610: 2220 6964 3d22 6578 6563 7574 6f72 3222  " id="executor2"
+00002620: 3e3c 7265 6374 2073 7479 6c65 3d22 2220  ><rect style="" 
+00002630: 7278 3d22 3022 2072 793d 2230 2220 783d  rx="0" ry="0" x=
+00002640: 2238 2220 793d 2238 2220 7769 6474 683d  "8" y="8" width=
+00002650: 2238 312e 3936 3837 3522 2068 6569 6768  "81.96875" heigh
+00002660: 743d 2231 3034 223e 3c2f 7265 6374 3e3c  t="104"></rect><
+00002670: 6720 636c 6173 733d 2263 6c75 7374 6572  g class="cluster
+00002680: 2d6c 6162 656c 2220 7472 616e 7366 6f72  -label" transfor
+00002690: 6d3d 2274 7261 6e73 6c61 7465 2831 332e  m="translate(13.
+000026a0: 3134 3834 3337 352c 2038 2922 3e3c 666f  1484375, 8)"><fo
+000026b0: 7265 6967 6e4f 626a 6563 7420 7769 6474  reignObject widt
+000026c0: 683d 2237 312e 3637 3138 3735 2220 6865  h="71.671875" he
+000026d0: 6967 6874 3d22 3139 223e 3c64 6976 2078  ight="19"><div x
+000026e0: 6d6c 6e73 3d22 6874 7470 3a2f 2f77 7777  mlns="http://www
+000026f0: 2e77 332e 6f72 672f 3139 3939 2f78 6874  .w3.org/1999/xht
+00002700: 6d6c 2220 7374 796c 653d 2264 6973 706c  ml" style="displ
+00002710: 6179 3a20 696e 6c69 6e65 2d62 6c6f 636b  ay: inline-block
+00002720: 3b20 7768 6974 652d 7370 6163 653a 206e  ; white-space: n
+00002730: 6f77 7261 703b 223e 3c73 7061 6e20 636c  owrap;"><span cl
+00002740: 6173 733d 226e 6f64 654c 6162 656c 223e  ass="nodeLabel">
+00002750: 6578 6563 7574 6f72 323c 2f73 7061 6e3e  executor2</span>
+00002760: 3c2f 6469 763e 3c2f 666f 7265 6967 6e4f  </div></foreignO
+00002770: 626a 6563 743e 3c2f 673e 3c2f 673e 3c2f  bject></g></g></
+00002780: 673e 3c67 2063 6c61 7373 3d22 6564 6765  g><g class="edge
+00002790: 5061 7468 7322 3e3c 2f67 3e3c 6720 636c  Paths"></g><g cl
+000027a0: 6173 733d 2265 6467 654c 6162 656c 7322  ass="edgeLabels"
+000027b0: 3e3c 2f67 3e3c 6720 636c 6173 733d 226e  ></g><g class="n
+000027c0: 6f64 6573 223e 3c67 2063 6c61 7373 3d22  odes"><g class="
+000027d0: 6e6f 6465 2064 6566 6175 6c74 2070 6f64  node default pod
+000027e0: 2066 6c6f 7763 6861 7274 2d6c 6162 656c   flowchart-label
+000027f0: 2220 6964 3d22 666c 6f77 6368 6172 742d  " id="flowchart-
+00002800: 6578 6563 7574 6f72 322f 7265 702d 302d  executor2/rep-0-
+00002810: 3330 2220 7472 616e 7366 6f72 6d3d 2274  30" transform="t
+00002820: 7261 6e73 6c61 7465 2834 382e 3938 3433  ranslate(48.9843
+00002830: 3735 2c20 3630 2922 3e3c 7265 6374 2063  75, 60)"><rect c
+00002840: 6c61 7373 3d22 6261 7369 6320 6c61 6265  lass="basic labe
+00002850: 6c2d 636f 6e74 6169 6e65 7222 2073 7479  l-container" sty
+00002860: 6c65 3d22 2220 7278 3d22 3022 2072 793d  le="" rx="0" ry=
+00002870: 2230 2220 783d 222d 3135 2e39 3834 3337  "0" x="-15.98437
+00002880: 3522 2079 3d22 2d31 3722 2077 6964 7468  5" y="-17" width
+00002890: 3d22 3331 2e39 3638 3735 2220 6865 6967  ="31.96875" heig
+000028a0: 6874 3d22 3334 223e 3c2f 7265 6374 3e3c  ht="34"></rect><
+000028b0: 6720 636c 6173 733d 226c 6162 656c 2220  g class="label" 
+000028c0: 7374 796c 653d 2222 2074 7261 6e73 666f  style="" transfo
+000028d0: 726d 3d22 7472 616e 736c 6174 6528 2d38  rm="translate(-8
+000028e0: 2e34 3834 3337 352c 202d 392e 3529 223e  .484375, -9.5)">
+000028f0: 3c72 6563 743e 3c2f 7265 6374 3e3c 666f  <rect></rect><fo
+00002900: 7265 6967 6e4f 626a 6563 7420 7769 6474  reignObject widt
+00002910: 683d 2231 362e 3936 3837 3522 2068 6569  h="16.96875" hei
+00002920: 6768 743d 2231 3922 3e3c 6469 7620 786d  ght="19"><div xm
+00002930: 6c6e 733d 2268 7474 703a 2f2f 7777 772e  lns="http://www.
+00002940: 7733 2e6f 7267 2f31 3939 392f 7868 746d  w3.org/1999/xhtm
+00002950: 6c22 2073 7479 6c65 3d22 6469 7370 6c61  l" style="displa
+00002960: 793a 2069 6e6c 696e 652d 626c 6f63 6b3b  y: inline-block;
+00002970: 2077 6869 7465 2d73 7061 6365 3a20 6e6f   white-space: no
+00002980: 7772 6170 3b22 3e3c 7370 616e 2063 6c61  wrap;"><span cla
+00002990: 7373 3d22 6e6f 6465 4c61 6265 6c22 3e45  ss="nodeLabel">E
+000029a0: 313c 2f73 7061 6e3e 3c2f 6469 763e 3c2f  1</span></div></
+000029b0: 666f 7265 6967 6e4f 626a 6563 743e 3c2f  foreignObject></
+000029c0: 673e 3c2f 673e 3c2f 673e 3c2f 673e 3c67  g></g></g></g><g
+000029d0: 2063 6c61 7373 3d22 726f 6f74 2220 7472   class="root" tr
+000029e0: 616e 7366 6f72 6d3d 2274 7261 6e73 6c61  ansform="transla
+000029f0: 7465 2832 3430 2e37 3936 3837 352c 2031  te(240.796875, 1
+00002a00: 3436 2922 3e3c 6720 636c 6173 733d 2263  46)"><g class="c
+00002a10: 6c75 7374 6572 7322 3e3c 6720 636c 6173  lusters"><g clas
+00002a20: 733d 2263 6c75 7374 6572 2044 4550 4c4f  s="cluster DEPLO
+00002a30: 594d 454e 5420 4445 504c 4f59 4d45 4e54  YMENT DEPLOYMENT
+00002a40: 2044 4550 4c4f 594d 454e 5420 4445 504c   DEPLOYMENT DEPL
+00002a50: 4f59 4d45 4e54 2066 6c6f 7763 6861 7274  OYMENT flowchart
+00002a60: 2d6c 6162 656c 2220 6964 3d22 4545 223e  -label" id="EE">
+00002a70: 3c72 6563 7420 7374 796c 653d 2222 2072  <rect style="" r
+00002a80: 783d 2230 2220 7279 3d22 3022 2078 3d22  x="0" ry="0" x="
+00002a90: 3822 2079 3d22 3822 2077 6964 7468 3d22  8" y="8" width="
+00002aa0: 3832 2e31 3430 3632 3522 2068 6569 6768  82.140625" heigh
+00002ab0: 743d 2231 3034 223e 3c2f 7265 6374 3e3c  t="104"></rect><
+00002ac0: 6720 636c 6173 733d 2263 6c75 7374 6572  g class="cluster
+00002ad0: 2d6c 6162 656c 2220 7472 616e 7366 6f72  -label" transfor
+00002ae0: 6d3d 2274 7261 6e73 6c61 7465 2834 302e  m="translate(40.
+00002af0: 352c 2038 2922 3e3c 666f 7265 6967 6e4f  5, 8)"><foreignO
+00002b00: 626a 6563 7420 7769 6474 683d 2231 372e  bject width="17.
+00002b10: 3134 3036 3235 2220 6865 6967 6874 3d22  140625" height="
+00002b20: 3139 223e 3c64 6976 2078 6d6c 6e73 3d22  19"><div xmlns="
+00002b30: 6874 7470 3a2f 2f77 7777 2e77 332e 6f72  http://www.w3.or
+00002b40: 672f 3139 3939 2f78 6874 6d6c 2220 7374  g/1999/xhtml" st
+00002b50: 796c 653d 2264 6973 706c 6179 3a20 696e  yle="display: in
+00002b60: 6c69 6e65 2d62 6c6f 636b 3b20 7768 6974  line-block; whit
+00002b70: 652d 7370 6163 653a 206e 6f77 7261 703b  e-space: nowrap;
+00002b80: 223e 3c73 7061 6e20 636c 6173 733d 226e  "><span class="n
+00002b90: 6f64 654c 6162 656c 223e 4545 3c2f 7370  odeLabel">EE</sp
+00002ba0: 616e 3e3c 2f64 6976 3e3c 2f66 6f72 6569  an></div></forei
+00002bb0: 676e 4f62 6a65 6374 3e3c 2f67 3e3c 2f67  gnObject></g></g
+00002bc0: 3e3c 2f67 3e3c 6720 636c 6173 733d 2265  ></g><g class="e
+00002bd0: 6467 6550 6174 6873 223e 3c2f 673e 3c67  dgePaths"></g><g
+00002be0: 2063 6c61 7373 3d22 6564 6765 4c61 6265   class="edgeLabe
+00002bf0: 6c73 223e 3c2f 673e 3c67 2063 6c61 7373  ls"></g><g class
+00002c00: 3d22 6e6f 6465 7322 3e3c 6720 636c 6173  ="nodes"><g clas
+00002c10: 733d 226e 6f64 6520 6465 6661 756c 7420  s="node default 
+00002c20: 706f 6420 666c 6f77 6368 6172 742d 6c61  pod flowchart-la
+00002c30: 6265 6c22 2069 643d 2266 6c6f 7763 6861  bel" id="flowcha
+00002c40: 7274 2d45 452f 7265 702d 302d 3239 2220  rt-EE/rep-0-29" 
+00002c50: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
+00002c60: 6c61 7465 2834 392e 3037 3033 3132 352c  late(49.0703125,
+00002c70: 2036 3029 223e 3c72 6563 7420 636c 6173   60)"><rect clas
+00002c80: 733d 2262 6173 6963 206c 6162 656c 2d63  s="basic label-c
+00002c90: 6f6e 7461 696e 6572 2220 7374 796c 653d  ontainer" style=
+00002ca0: 2222 2072 783d 2230 2220 7279 3d22 3022  "" rx="0" ry="0"
+00002cb0: 2078 3d22 2d31 362e 3037 3033 3132 3522   x="-16.0703125"
+00002cc0: 2079 3d22 2d31 3722 2077 6964 7468 3d22   y="-17" width="
+00002cd0: 3332 2e31 3430 3632 3522 2068 6569 6768  32.140625" heigh
+00002ce0: 743d 2233 3422 3e3c 2f72 6563 743e 3c67  t="34"></rect><g
+00002cf0: 2063 6c61 7373 3d22 6c61 6265 6c22 2073   class="label" s
+00002d00: 7479 6c65 3d22 2220 7472 616e 7366 6f72  tyle="" transfor
+00002d10: 6d3d 2274 7261 6e73 6c61 7465 282d 382e  m="translate(-8.
+00002d20: 3537 3033 3132 352c 202d 392e 3529 223e  5703125, -9.5)">
+00002d30: 3c72 6563 743e 3c2f 7265 6374 3e3c 666f  <rect></rect><fo
+00002d40: 7265 6967 6e4f 626a 6563 7420 7769 6474  reignObject widt
+00002d50: 683d 2231 372e 3134 3036 3235 2220 6865  h="17.140625" he
+00002d60: 6967 6874 3d22 3139 223e 3c64 6976 2078  ight="19"><div x
+00002d70: 6d6c 6e73 3d22 6874 7470 3a2f 2f77 7777  mlns="http://www
+00002d80: 2e77 332e 6f72 672f 3139 3939 2f78 6874  .w3.org/1999/xht
+00002d90: 6d6c 2220 7374 796c 653d 2264 6973 706c  ml" style="displ
+00002da0: 6179 3a20 696e 6c69 6e65 2d62 6c6f 636b  ay: inline-block
+00002db0: 3b20 7768 6974 652d 7370 6163 653a 206e  ; white-space: n
+00002dc0: 6f77 7261 703b 223e 3c73 7061 6e20 636c  owrap;"><span cl
+00002dd0: 6173 733d 226e 6f64 654c 6162 656c 223e  ass="nodeLabel">
+00002de0: 4545 3c2f 7370 616e 3e3c 2f64 6976 3e3c  EE</span></div><
+00002df0: 2f66 6f72 6569 676e 4f62 6a65 6374 3e3c  /foreignObject><
+00002e00: 2f67 3e3c 2f67 3e3c 2f67 3e3c 2f67 3e3c  /g></g></g></g><
+00002e10: 6720 636c 6173 733d 2272 6f6f 7422 2074  g class="root" t
+00002e20: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
+00002e30: 6174 6528 3131 372e 3231 3837 352c 2036  ate(117.21875, 6
+00002e40: 3929 223e 3c67 2063 6c61 7373 3d22 636c  9)"><g class="cl
+00002e50: 7573 7465 7273 223e 3c67 2063 6c61 7373  usters"><g class
+00002e60: 3d22 636c 7573 7465 7220 4445 504c 4f59  ="cluster DEPLOY
+00002e70: 4d45 4e54 2044 4550 4c4f 594d 454e 5420  MENT DEPLOYMENT 
+00002e80: 4445 504c 4f59 4d45 4e54 2044 4550 4c4f  DEPLOYMENT DEPLO
+00002e90: 594d 454e 5420 4445 504c 4f59 4d45 4e54  YMENT DEPLOYMENT
+00002ea0: 2044 4550 4c4f 594d 454e 5420 666c 6f77   DEPLOYMENT flow
+00002eb0: 6368 6172 742d 6c61 6265 6c22 2069 643d  chart-label" id=
+00002ec0: 2245 223e 3c72 6563 7420 7374 796c 653d  "E"><rect style=
+00002ed0: 2222 2072 783d 2230 2220 7279 3d22 3022  "" rx="0" ry="0"
+00002ee0: 2078 3d22 3822 2079 3d22 3822 2077 6964   x="8" y="8" wid
+00002ef0: 7468 3d22 3733 2e35 3738 3132 3522 2068  th="73.578125" h
+00002f00: 6569 6768 743d 2231 3034 223e 3c2f 7265  eight="104"></re
+00002f10: 6374 3e3c 6720 636c 6173 733d 2263 6c75  ct><g class="clu
+00002f20: 7374 6572 2d6c 6162 656c 2220 7472 616e  ster-label" tran
+00002f30: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
+00002f40: 2834 302e 352c 2038 2922 3e3c 666f 7265  (40.5, 8)"><fore
+00002f50: 6967 6e4f 626a 6563 7420 7769 6474 683d  ignObject width=
+00002f60: 2238 2e35 3738 3132 3522 2068 6569 6768  "8.578125" heigh
+00002f70: 743d 2231 3922 3e3c 6469 7620 786d 6c6e  t="19"><div xmln
+00002f80: 733d 2268 7474 703a 2f2f 7777 772e 7733  s="http://www.w3
+00002f90: 2e6f 7267 2f31 3939 392f 7868 746d 6c22  .org/1999/xhtml"
+00002fa0: 2073 7479 6c65 3d22 6469 7370 6c61 793a   style="display:
+00002fb0: 2069 6e6c 696e 652d 626c 6f63 6b3b 2077   inline-block; w
+00002fc0: 6869 7465 2d73 7061 6365 3a20 6e6f 7772  hite-space: nowr
+00002fd0: 6170 3b22 3e3c 7370 616e 2063 6c61 7373  ap;"><span class
+00002fe0: 3d22 6e6f 6465 4c61 6265 6c22 3e45 3c2f  ="nodeLabel">E</
+00002ff0: 7370 616e 3e3c 2f64 6976 3e3c 2f66 6f72  span></div></for
+00003000: 6569 676e 4f62 6a65 6374 3e3c 2f67 3e3c  eignObject></g><
+00003010: 2f67 3e3c 2f67 3e3c 6720 636c 6173 733d  /g></g><g class=
+00003020: 2265 6467 6550 6174 6873 223e 3c2f 673e  "edgePaths"></g>
+00003030: 3c67 2063 6c61 7373 3d22 6564 6765 4c61  <g class="edgeLa
+00003040: 6265 6c73 223e 3c2f 673e 3c67 2063 6c61  bels"></g><g cla
+00003050: 7373 3d22 6e6f 6465 7322 3e3c 6720 636c  ss="nodes"><g cl
+00003060: 6173 733d 226e 6f64 6520 6465 6661 756c  ass="node defaul
+00003070: 7420 706f 6420 666c 6f77 6368 6172 742d  t pod flowchart-
+00003080: 6c61 6265 6c22 2069 643d 2266 6c6f 7763  label" id="flowc
+00003090: 6861 7274 2d45 2f72 6570 2d30 2d32 3822  hart-E/rep-0-28"
+000030a0: 2074 7261 6e73 666f 726d 3d22 7472 616e   transform="tran
+000030b0: 736c 6174 6528 3434 2e37 3839 3036 3235  slate(44.7890625
+000030c0: 2c20 3630 2922 3e3c 7265 6374 2063 6c61  , 60)"><rect cla
+000030d0: 7373 3d22 6261 7369 6320 6c61 6265 6c2d  ss="basic label-
+000030e0: 636f 6e74 6169 6e65 7222 2073 7479 6c65  container" style
+000030f0: 3d22 2220 7278 3d22 3022 2072 793d 2230  ="" rx="0" ry="0
+00003100: 2220 783d 222d 3131 2e37 3839 3036 3235  " x="-11.7890625
+00003110: 2220 793d 222d 3137 2220 7769 6474 683d  " y="-17" width=
+00003120: 2232 332e 3537 3831 3235 2220 6865 6967  "23.578125" heig
+00003130: 6874 3d22 3334 223e 3c2f 7265 6374 3e3c  ht="34"></rect><
+00003140: 6720 636c 6173 733d 226c 6162 656c 2220  g class="label" 
+00003150: 7374 796c 653d 2222 2074 7261 6e73 666f  style="" transfo
+00003160: 726d 3d22 7472 616e 736c 6174 6528 2d34  rm="translate(-4
+00003170: 2e32 3839 3036 3235 2c20 2d39 2e35 2922  .2890625, -9.5)"
+00003180: 3e3c 7265 6374 3e3c 2f72 6563 743e 3c66  ><rect></rect><f
+00003190: 6f72 6569 676e 4f62 6a65 6374 2077 6964  oreignObject wid
+000031a0: 7468 3d22 382e 3537 3831 3235 2220 6865  th="8.578125" he
+000031b0: 6967 6874 3d22 3139 223e 3c64 6976 2078  ight="19"><div x
+000031c0: 6d6c 6e73 3d22 6874 7470 3a2f 2f77 7777  mlns="http://www
+000031d0: 2e77 332e 6f72 672f 3139 3939 2f78 6874  .w3.org/1999/xht
+000031e0: 6d6c 2220 7374 796c 653d 2264 6973 706c  ml" style="displ
+000031f0: 6179 3a20 696e 6c69 6e65 2d62 6c6f 636b  ay: inline-block
+00003200: 3b20 7768 6974 652d 7370 6163 653a 206e  ; white-space: n
+00003210: 6f77 7261 703b 223e 3c73 7061 6e20 636c  owrap;"><span cl
+00003220: 6173 733d 226e 6f64 654c 6162 656c 223e  ass="nodeLabel">
+00003230: 453c 2f73 7061 6e3e 3c2f 6469 763e 3c2f  E</span></div></
+00003240: 666f 7265 6967 6e4f 626a 6563 743e 3c2f  foreignObject></
+00003250: 673e 3c2f 673e 3c2f 673e 3c2f 673e 3c67  g></g></g></g><g
+00003260: 2063 6c61 7373 3d22 6e6f 6465 2064 6566   class="node def
+00003270: 6175 6c74 2047 4154 4557 4159 2066 6c6f  ault GATEWAY flo
+00003280: 7763 6861 7274 2d6c 6162 656c 2220 6964  wchart-label" id
+00003290: 3d22 666c 6f77 6368 6172 742d 6761 7465  ="flowchart-gate
+000032a0: 7761 7973 7461 7274 2d33 3222 2074 7261  waystart-32" tra
+000032b0: 6e73 666f 726d 3d22 7472 616e 736c 6174  nsform="translat
+000032c0: 6528 3337 2e33 3539 3337 352c 2031 3239  e(37.359375, 129
+000032d0: 2922 3e3c 7265 6374 2063 6c61 7373 3d22  )"><rect class="
+000032e0: 6261 7369 6320 6c61 6265 6c2d 636f 6e74  basic label-cont
+000032f0: 6169 6e65 7222 2073 7479 6c65 3d22 2220  ainer" style="" 
+00003300: 7278 3d22 3022 2072 793d 2230 2220 783d  rx="0" ry="0" x=
+00003310: 222d 3337 2e33 3539 3337 3522 2079 3d22  "-37.359375" y="
+00003320: 2d31 3722 2077 6964 7468 3d22 3734 2e37  -17" width="74.7
+00003330: 3138 3735 2220 6865 6967 6874 3d22 3334  1875" height="34
+00003340: 223e 3c2f 7265 6374 3e3c 6720 636c 6173  "></rect><g clas
+00003350: 733d 226c 6162 656c 2220 7374 796c 653d  s="label" style=
+00003360: 2222 2074 7261 6e73 666f 726d 3d22 7472  "" transform="tr
+00003370: 616e 736c 6174 6528 2d32 392e 3835 3933  anslate(-29.8593
+00003380: 3735 2c20 2d39 2e35 2922 3e3c 7265 6374  75, -9.5)"><rect
+00003390: 3e3c 2f72 6563 743e 3c66 6f72 6569 676e  ></rect><foreign
+000033a0: 4f62 6a65 6374 2077 6964 7468 3d22 3539  Object width="59
+000033b0: 2e37 3138 3735 2220 6865 6967 6874 3d22  .71875" height="
+000033c0: 3139 223e 3c64 6976 2078 6d6c 6e73 3d22  19"><div xmlns="
+000033d0: 6874 7470 3a2f 2f77 7777 2e77 332e 6f72  http://www.w3.or
+000033e0: 672f 3139 3939 2f78 6874 6d6c 2220 7374  g/1999/xhtml" st
+000033f0: 796c 653d 2264 6973 706c 6179 3a20 696e  yle="display: in
+00003400: 6c69 6e65 2d62 6c6f 636b 3b20 7768 6974  line-block; whit
+00003410: 652d 7370 6163 653a 206e 6f77 7261 703b  e-space: nowrap;
+00003420: 223e 3c73 7061 6e20 636c 6173 733d 226e  "><span class="n
+00003430: 6f64 654c 6162 656c 223e 6761 7465 7761  odeLabel">gatewa
+00003440: 793c 2f73 7061 6e3e 3c2f 6469 763e 3c2f  y</span></div></
+00003450: 666f 7265 6967 6e4f 626a 6563 743e 3c2f  foreignObject></
+00003460: 673e 3c2f 673e 3c67 2063 6c61 7373 3d22  g></g><g class="
+00003470: 6e6f 6465 2064 6566 6175 6c74 2047 4154  node default GAT
+00003480: 4557 4159 2066 6c6f 7763 6861 7274 2d6c  EWAY flowchart-l
+00003490: 6162 656c 2220 6964 3d22 666c 6f77 6368  abel" id="flowch
+000034a0: 6172 742d 6761 7465 7761 7965 6e64 2d34  art-gatewayend-4
+000034b0: 3122 2074 7261 6e73 666f 726d 3d22 7472  1" transform="tr
+000034c0: 616e 736c 6174 6528 3534 392e 3736 3536  anslate(549.7656
+000034d0: 3235 2c20 3230 3629 223e 3c72 6563 7420  25, 206)"><rect 
+000034e0: 636c 6173 733d 2262 6173 6963 206c 6162  class="basic lab
+000034f0: 656c 2d63 6f6e 7461 696e 6572 2220 7374  el-container" st
+00003500: 796c 653d 2222 2072 783d 2230 2220 7279  yle="" rx="0" ry
+00003510: 3d22 3022 2078 3d22 2d33 372e 3335 3933  ="0" x="-37.3593
+00003520: 3735 2220 793d 222d 3137 2220 7769 6474  75" y="-17" widt
+00003530: 683d 2237 342e 3731 3837 3522 2068 6569  h="74.71875" hei
+00003540: 6768 743d 2233 3422 3e3c 2f72 6563 743e  ght="34"></rect>
+00003550: 3c67 2063 6c61 7373 3d22 6c61 6265 6c22  <g class="label"
+00003560: 2073 7479 6c65 3d22 2220 7472 616e 7366   style="" transf
+00003570: 6f72 6d3d 2274 7261 6e73 6c61 7465 282d  orm="translate(-
+00003580: 3239 2e38 3539 3337 352c 202d 392e 3529  29.859375, -9.5)
+00003590: 223e 3c72 6563 743e 3c2f 7265 6374 3e3c  "><rect></rect><
+000035a0: 666f 7265 6967 6e4f 626a 6563 7420 7769  foreignObject wi
+000035b0: 6474 683d 2235 392e 3731 3837 3522 2068  dth="59.71875" h
+000035c0: 6569 6768 743d 2231 3922 3e3c 6469 7620  eight="19"><div 
+000035d0: 786d 6c6e 733d 2268 7474 703a 2f2f 7777  xmlns="http://ww
+000035e0: 772e 7733 2e6f 7267 2f31 3939 392f 7868  w.w3.org/1999/xh
+000035f0: 746d 6c22 2073 7479 6c65 3d22 6469 7370  tml" style="disp
+00003600: 6c61 793a 2069 6e6c 696e 652d 626c 6f63  lay: inline-bloc
+00003610: 6b3b 2077 6869 7465 2d73 7061 6365 3a20  k; white-space: 
+00003620: 6e6f 7772 6170 3b22 3e3c 7370 616e 2063  nowrap;"><span c
+00003630: 6c61 7373 3d22 6e6f 6465 4c61 6265 6c22  lass="nodeLabel"
+00003640: 3e67 6174 6577 6179 3c2f 7370 616e 3e3c  >gateway</span><
+00003650: 2f64 6976 3e3c 2f66 6f72 6569 676e 4f62  /div></foreignOb
+00003660: 6a65 6374 3e3c 2f67 3e3c 2f67 3e3c 2f67  ject></g></g></g
+00003670: 3e3c 2f67 3e3c 2f67 3e3c 7374 796c 653e  ></g></g><style>
+00003680: 4069 6d70 6f72 7420 7572 6c28 2268 7474  @import url("htt
+00003690: 7073 3a2f 2f63 646e 6a73 2e63 6c6f 7564  ps://cdnjs.cloud
+000036a0: 666c 6172 652e 636f 6d2f 616a 6178 2f6c  flare.com/ajax/l
+000036b0: 6962 732f 666f 6e74 2d61 7765 736f 6d65  ibs/font-awesome
+000036c0: 2f36 2e34 2e30 2f63 7373 2f61 6c6c 2e6d  /6.4.0/css/all.m
+000036d0: 696e 2e63 7373 2229 3b3c 2f73 7479 6c65  in.css");</style
+000036e0: 3e3c 2f73 7667 3e                        ></svg>
```

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/serving/jina/__demo/server.py` & `MeUtils-2023.8.2.13.20.11/meutils/serving/jina/__demo/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,23 +55,29 @@
 #     .add(uses=E2, needs=['E1'])
 # )
 
 # f = Flow(port=8501, protocol=['GRPC']).add(uses=MyExec).add(uses=Cut)
 # f = Flow(port=[8500, 8501], protocol=['GRPC', 'HTTP']).add(uses=MyExec)  # .add(uses=Cut).add(uses=Read)
 f123.plot('flow.svg')
 
-with f1, f2, f12, f123:
-    # 测试
-    r = f1.post('/', DocumentArray.empty(1))
-    print(r.texts)
-    r = f2.post('/e1', DocumentArray.empty(2))
-    print(r.texts)
-    r = f12.post('/e2', DocumentArray.empty(12))
-    print(r.texts)
-    r = f123.post('/', DocumentArray.empty(3))
-    print(r.texts)
-    # r = f123.post('/', [1,2,3])
-    # backend server forever
-    f123.block()
 
-# with Deployment(name='myexec1', uses=MyExec) as dep:
-#     dep.post(on='/bar', inputs=Document(), on_done=print)
+
+if __name__ == '__main__':
+
+    with f1, f2, f12, f123:
+        # 测试
+        r = f1.post('/', DocumentArray.empty(1))
+        print(r.texts)
+        r = f2.post('/e1', DocumentArray.empty(2))
+        print(r.texts)
+        # r = f12.post('/e2', DocumentArray.empty(12))
+        # print(r.texts)
+        # r = f123.post('/', DocumentArray.empty(3))
+        # print(r.texts)
+        # r = f123.post('/', [1,2,3])
+        # backend server forever
+        # f123.block()
+
+    # with Deployment(name='myexec1', uses=MyExec) as dep:
+    #     dep.post(on='/bar', inputs=Document(), on_done=print)
+
+
```

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/serving/jina/executors/SentenceEncoder.py` & `MeUtils-2023.8.2.13.20.11/meutils/serving/jina/executors/SentenceEncoder.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/serving/jina/executors/__init__.py` & `MeUtils-2023.8.2.13.20.11/meutils/serving/jina/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/serving/jina/nlp_serving/word_segmentation.py` & `MeUtils-2023.8.2.13.20.11/meutils/serving/jina/nlp_serving/word_segmentation.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/serving/st_utils/_test.py` & `MeUtils-2023.8.2.13.20.11/meutils/serving/st_utils/_test.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/serving/st_utils/common.py` & `MeUtils-2023.8.2.13.20.11/meutils/serving/st_utils/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/serving/webui/.streamlit/_config.toml` & `MeUtils-2023.8.2.13.20.11/meutils/serving/webui/.streamlit/_config.toml`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/serving/webui/_2_词性标注与实体识别.py` & `MeUtils-2023.8.2.13.20.11/meutils/serving/webui/_2_词性标注与实体识别.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/serving/webui/pages/_1_分词.py` & `MeUtils-2023.8.2.13.20.11/meutils/serving/webui/pages/_1_分词.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/serving/webui/pages/_2_词性标注与实体识别.py` & `MeUtils-2023.8.2.13.20.11/meutils/serving/webui/pages/_2_词性标注与实体识别.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/serving/webui/pages/_3_文本匹配.py` & `MeUtils-2023.8.2.13.20.11/meutils/serving/webui/pages/_3_文本匹配.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/sftp.py` & `MeUtils-2023.8.2.13.20.11/meutils/sftp.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/sk_utils.py` & `MeUtils-2023.8.2.13.20.11/meutils/sk_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/smooth_utils.py` & `MeUtils-2023.8.2.13.20.11/meutils/smooth_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/spark/__init__.py` & `MeUtils-2023.8.2.13.20.11/meutils/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/str_utils/Translator.py` & `MeUtils-2023.8.2.13.20.11/meutils/str_utils/Translator.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/str_utils/__init__.py` & `MeUtils-2023.8.2.13.20.11/meutils/str_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/str_utils/__translater/tencent.py` & `MeUtils-2023.8.2.13.20.11/meutils/str_utils/__translater/tencent.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/str_utils/__translater/translater.py` & `MeUtils-2023.8.2.13.20.11/meutils/str_utils/__translater/translater.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/str_utils/__translater/youdao.py` & `MeUtils-2023.8.2.13.20.11/meutils/str_utils/__translater/youdao.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/str_utils/json_utils.py` & `MeUtils-2023.8.2.13.20.11/meutils/str_utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/str_utils/regular_expression.py` & `MeUtils-2023.8.2.13.20.11/meutils/str_utils/regular_expression.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/templates/demo.j2` & `MeUtils-2023.8.2.13.20.11/meutils/templates/demo.j2`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/templates/demo.py` & `MeUtils-2023.8.2.13.20.11/meutils/templates/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/templates/demox.py` & `MeUtils-2023.8.2.13.20.11/meutils/templates/demox.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/templates/df_html.j2` & `MeUtils-2023.8.2.13.20.11/meutils/templates/df_html.j2`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/templates/dockerfiles/docker_build_push.py` & `MeUtils-2023.8.2.13.20.11/meutils/templates/dockerfiles/docker_build_push.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/templates/hegui.py` & `MeUtils-2023.8.2.13.20.11/meutils/templates/hegui.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/templates/markmap.html` & `MeUtils-2023.8.2.13.20.11/meutils/templates/markmap.html`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/cookiecutter.json` & `MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore` & `MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml` & `MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst` & `MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE` & `MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile` & `MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md` & `MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst` & `MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile` & `MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md` & `MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py` & `MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst` & `MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat` & `MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg` & `MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py` & `MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py` & `MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini` & `MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py` & `MeUtils-2023.8.2.13.20.11/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/templates/tpl.docx` & `MeUtils-2023.8.2.13.20.11/meutils/templates/tpl.docx`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/templates/x.html` & `MeUtils-2023.8.2.13.20.11/meutils/templates/x.html`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/templates/合规日报模板.docx` & `MeUtils-2023.8.2.13.20.11/meutils/templates/合规日报模板.docx`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/todo.py` & `MeUtils-2023.8.2.13.20.11/meutils/todo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/tools/cprint.py` & `MeUtils-2023.8.2.13.20.11/meutils/tools/cprint.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/tools/machine_monitor.py` & `MeUtils-2023.8.2.13.20.11/meutils/tools/machine_monitor.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/tools/monitor.yml` & `MeUtils-2023.8.2.13.20.11/meutils/tools/monitor.yml`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/tools/seize.py` & `MeUtils-2023.8.2.13.20.11/meutils/tools/seize.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/tools/service_monitor.py` & `MeUtils-2023.8.2.13.20.11/meutils/tools/service_monitor.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/meutils/zk_utils.py` & `MeUtils-2023.8.2.13.20.11/meutils/zk_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/pypi.sh` & `MeUtils-2023.8.2.13.20.11/pypi.sh`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.7.7.15.3.6/setup.py` & `MeUtils-2023.8.2.13.20.11/setup.py`

 * *Files identical despite different names*

