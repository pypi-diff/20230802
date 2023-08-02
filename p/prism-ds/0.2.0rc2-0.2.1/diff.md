# Comparing `tmp/prism-ds-0.2.0rc2.tar.gz` & `tmp/prism-ds-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prism-ds-0.2.0rc2.tar", last modified: Thu Jul 20 02:38:10 2023, max compression
+gzip compressed data, was "prism-ds-0.2.1.tar", last modified: Wed Aug  2 01:51:02 2023, max compression
```

## Comparing `prism-ds-0.2.0rc2.tar` & `prism-ds-0.2.1.tar`

### file list

```diff
@@ -1,473 +1,473 @@
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.452599 prism-ds-0.2.0rc2/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    11312 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc2/LICENSE
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      219 2023-05-16 12:01:01.000000 prism-ds-0.2.0rc2/MANIFEST.in
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5536 2023-07-20 02:38:10.452732 prism-ds-0.2.0rc2/PKG-INFO
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4572 2023-05-16 12:50:41.000000 prism-ds-0.2.0rc2/README.md
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.364681 prism-ds-0.2.0rc2/prism/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-17 00:34:22.000000 prism-ds-0.2.0rc2/prism/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/admin.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.365970 prism-ds-0.2.0rc2/prism/agents/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc2/prism/agents/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7762 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/agents/base.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    18549 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/agents/docker_agent.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    37974 2023-07-20 02:37:50.000000 prism-ds-0.2.0rc2/prism/agents/ec2.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      533 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc2/prism/agents/meta.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.366576 prism-ds-0.2.0rc2/prism/agents/scripts/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-05-16 12:00:13.000000 prism-ds-0.2.0rc2/prism/agents/scripts/__init__.py
--rwxr-xr-x   0 mihirtrivedi   (501) staff       (20)     3447 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/agents/scripts/apply.sh
--rwxr-xr-x   0 mihirtrivedi   (501) staff       (20)      710 2023-06-28 01:05:16.000000 prism-ds-0.2.0rc2/prism/agents/scripts/run.sh
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.369826 prism-ds-0.2.0rc2/prism/cli/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc2/prism/cli/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10729 2023-07-20 02:05:38.000000 prism-ds-0.2.0rc2/prism/cli/agent.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7470 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/cli/base.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10421 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/cli/compile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4457 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc2/prism/cli/connect.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4222 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc2/prism/cli/create_agent.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4817 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/cli/create_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4444 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc2/prism/cli/create_trigger.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5443 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/cli/graph.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5506 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc2/prism/cli/init.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     9402 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/cli/run.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      724 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/cli/spark_submit.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.370198 prism-ds-0.2.0rc2/prism/client/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    16701 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/client/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4973 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/constants.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.371033 prism-ds-0.2.0rc2/prism/decorators/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      116 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc2/prism/decorators/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7124 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc2/prism/decorators/target.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3116 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc2/prism/decorators/task.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.371213 prism-ds-0.2.0rc2/prism/docs/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       79 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/docs/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.374847 prism-ds-0.2.0rc2/prism/docs/build/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    50665 2023-07-18 21:18:50.000000 prism-ds-0.2.0rc2/prism/docs/build/311ea03002abadcdcaba.png
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6035 2023-07-18 21:18:50.000000 prism-ds-0.2.0rc2/prism/docs/build/54968a39190c43d592b9.svg
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15406 2023-07-18 21:18:50.000000 prism-ds-0.2.0rc2/prism/docs/build/737ad70b3f2d3a9b5f6e.ico
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       79 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/docs/build/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4653 2023-07-18 21:18:50.000000 prism-ds-0.2.0rc2/prism/docs/build/ce188596011a8fa32931.png
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)   560712 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/docs/build/index.html
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      961 2023-07-18 21:18:50.000000 prism-ds-0.2.0rc2/prism/docs/build/main.js.LICENSE.txt
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.375179 prism-ds-0.2.0rc2/prism/event_managers/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc2/prism/event_managers/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6081 2023-07-13 03:54:01.000000 prism-ds-0.2.0rc2/prism/event_managers/base.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7852 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/exceptions.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.379950 prism-ds-0.2.0rc2/prism/infra/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc2/prism/infra/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6833 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/infra/compiled_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    14303 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/infra/compiler.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    13388 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/infra/executor.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3900 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/infra/hooks.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2704 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/infra/manifest.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3716 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/infra/pipeline.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    17198 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/infra/project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1421 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/infra/sys_path.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2628 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/infra/task_manager.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    24529 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/main.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.382216 prism-ds-0.2.0rc2/prism/mixins/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-ds-0.2.0rc2/prism/mixins/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2405 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc2/prism/mixins/agent.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2823 2023-06-08 13:53:30.000000 prism-ds-0.2.0rc2/prism/mixins/aws.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1288 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/mixins/base.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    11668 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/mixins/compile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7301 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc2/prism/mixins/connect.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2312 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc2/prism/mixins/create_agent.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5706 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/mixins/create_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5428 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc2/prism/mixins/create_trigger.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2438 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/mixins/graph.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1107 2023-04-02 17:52:18.000000 prism-ds-0.2.0rc2/prism/mixins/run.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4232 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/mixins/sys_handler.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.383179 prism-ds-0.2.0rc2/prism/parsers/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc2/prism/parsers/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    31631 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/parsers/ast_parser.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2206 2023-07-15 21:15:27.000000 prism-ds-0.2.0rc2/prism/parsers/base.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3049 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc2/prism/parsers/yml_parser.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    22013 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/prism_logging.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.385817 prism-ds-0.2.0rc2/prism/profiles/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc2/prism/profiles/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2745 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc2/prism/profiles/adapter.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3733 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/profiles/bigquery.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15570 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/profiles/dbt.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      539 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/profiles/meta.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4567 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/profiles/postgres.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     9117 2023-07-05 11:15:15.000000 prism-ds-0.2.0rc2/prism/profiles/profile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4089 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/profiles/pyspark.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4557 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/profiles/redshift.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4176 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/profiles/snowflake.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6358 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/profiles/trino.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.386484 prism-ds-0.2.0rc2/prism/spark/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc2/prism/spark/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      439 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/spark/script.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2889 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/spark/wrapper.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1448 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/target.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5171 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc2/prism/task.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.386666 prism-ds-0.2.0rc2/prism/templates/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-17 00:55:51.000000 prism-ds-0.2.0rc2/prism/templates/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.387448 prism-ds-0.2.0rc2/prism/templates/agents/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       59 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc2/prism/templates/agents/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      233 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc2/prism/templates/agents/docker.yml
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      191 2023-05-20 15:36:38.000000 prism-ds-0.2.0rc2/prism/templates/agents/ec2.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.388294 prism-ds-0.2.0rc2/prism/templates/minimal_project/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       19 2022-08-16 12:31:03.000000 prism-ds-0.2.0rc2/prism/templates/minimal_project/.gitignore
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/templates/minimal_project/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1326 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/templates/minimal_project/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.388859 prism-ds-0.2.0rc2/prism/templates/minimal_project/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1011 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/templates/minimal_project/tasks/class_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      937 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/templates/minimal_project/tasks/decorated_task.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.389124 prism-ds-0.2.0rc2/prism/templates/profile/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       61 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/templates/profile/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.389292 prism-ds-0.2.0rc2/prism/templates/profile/bigquery/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      148 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc2/prism/templates/profile/bigquery/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.389627 prism-ds-0.2.0rc2/prism/templates/profile/dbt/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      141 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc2/prism/templates/profile/dbt/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.389904 prism-ds-0.2.0rc2/prism/templates/profile/postgres/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      180 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc2/prism/templates/profile/postgres/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.390078 prism-ds-0.2.0rc2/prism/templates/profile/pyspark/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      478 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc2/prism/templates/profile/pyspark/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.390241 prism-ds-0.2.0rc2/prism/templates/profile/redshift/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      180 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc2/prism/templates/profile/redshift/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.390481 prism-ds-0.2.0rc2/prism/templates/profile/snowflake/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      193 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc2/prism/templates/profile/snowflake/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.390701 prism-ds-0.2.0rc2/prism/templates/profile/trino/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      189 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc2/prism/templates/profile/trino/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.391420 prism-ds-0.2.0rc2/prism/templates/starter_project/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       19 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc2/prism/templates/starter_project/.gitignore
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/templates/starter_project/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.391680 prism-ds-0.2.0rc2/prism/templates/starter_project/data/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-ds-0.2.0rc2/prism/templates/starter_project/data/.exists
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.391779 prism-ds-0.2.0rc2/prism/templates/starter_project/dev/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      786 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/templates/starter_project/dev/dev.ipynb
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.391981 prism-ds-0.2.0rc2/prism/templates/starter_project/output/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-ds-0.2.0rc2/prism/templates/starter_project/output/.exists
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1112 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/templates/starter_project/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.392308 prism-ds-0.2.0rc2/prism/templates/starter_project/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1011 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/templates/starter_project/tasks/class_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      938 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/templates/starter_project/tasks/decorated_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       66 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/templates/starter_project/utils.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.394798 prism-ds-0.2.0rc2/prism/templates/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      426 2023-05-27 16:07:03.000000 prism-ds-0.2.0rc2/prism/templates/tasks/pyspark_cls.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      427 2023-05-27 16:07:03.000000 prism-ds-0.2.0rc2/prism/templates/tasks/pyspark_dec.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      426 2023-05-27 16:07:03.000000 prism-ds-0.2.0rc2/prism/templates/tasks/python_cls.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      427 2023-05-27 16:07:03.000000 prism-ds-0.2.0rc2/prism/templates/tasks/python_dec.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      155 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/templates/tasks/sql.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.395416 prism-ds-0.2.0rc2/prism/templates/triggers/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       61 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/templates/triggers/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      267 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc2/prism/templates/triggers/function.yml
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      208 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc2/prism/templates/triggers/prism_project.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.395859 prism-ds-0.2.0rc2/prism/tests/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc2/prism/tests/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.399003 prism-ds-0.2.0rc2/prism/tests/integration/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc2/prism/tests/integration/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7886 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/integration_test_class.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15381 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_client.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10484 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_compile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10444 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_connect.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6512 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_create.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4012 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_dbt.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5728 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_hooks.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4539 2023-05-30 01:42:39.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_init.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.359850 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.399672 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001_init/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001_init/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1120 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001_init/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.400135 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001_init/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1011 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001_init/tasks/class_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      938 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001_init/tasks/decorated_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       66 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001_init/utils.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.400469 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001a_init_minimal/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001a_init_minimal/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1343 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001a_init_minimal/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.400824 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001a_init_minimal/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1011 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001a_init_minimal/tasks/class_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      937 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001a_init_minimal/tasks/decorated_task.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.401105 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/002_no_project_py/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/002_no_project_py/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      772 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/002_no_project_py/functions.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.401768 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/002_no_project_py/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      825 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/002_no_project_py/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      857 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/002_no_project_py/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      857 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/002_no_project_py/modules/module03.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.402036 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/003_project_with_cycle/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/003_project_with_cycle/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.403634 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/003_project_with_cycle/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      773 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/003_project_with_cycle/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      806 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/003_project_with_cycle/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      807 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/003_project_with_cycle/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/003_project_with_cycle/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.404089 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/004_simple_project/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/004_simple_project/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.405454 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/004_simple_project/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      935 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/004_simple_project/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1027 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/004_simple_project/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      801 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/004_simple_project/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1033 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/004_simple_project/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.406175 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      772 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/functions.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.407129 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1100 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      868 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      808 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.407657 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      772 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/functions.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.408381 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1127 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      923 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      913 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module04.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.408741 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.409715 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      969 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1090 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      974 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      910 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1257 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.410064 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/007_spark_project/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/007_spark_project/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1073 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/007_spark_project/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.411306 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/007_spark_project/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1751 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/007_spark_project/tasks/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1139 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/007_spark_project/tasks/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      940 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/007_spark_project/tasks/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      636 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/007_spark_project/tasks/module04.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.411666 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/008_targets/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/008_targets/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1073 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/008_targets/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.413291 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/008_targets/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      982 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/008_targets/tasks/csv.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1548 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/008_targets/tasks/csv_iter.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1632 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/008_targets/tasks/csv_mult.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1765 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/008_targets/tasks/parquet.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      498 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/008_targets/tasks/txt.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.413546 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/009_simple_dbt_project/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/009_simple_dbt_project/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.413709 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1073 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.414212 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      569 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/tasks/bad_adapter.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      576 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/tasks/filter_customers.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.414611 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.414853 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.415269 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      934 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1059 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module02.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.415513 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      875 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      812 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.415903 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/011_bad_task_ref/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-07-09 15:09:25.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/011_bad_task_ref/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.416129 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/011_bad_task_ref/modules/
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.416718 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      934 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1067 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module02.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.416940 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      875 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      812 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/011_bad_task_ref/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/011_bad_task_ref/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.417233 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.418169 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1196 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1195 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1045 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      808 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.418521 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency_local/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency_local/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency_local/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.418952 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency_local/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1239 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency_local/tasks/local_tasks.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      597 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency_local/tasks/non_local_task.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.419285 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.420350 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1287 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/bad_adapter.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1133 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/postgres.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1871 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/snowflake.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2147 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/spark.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1073 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.420822 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/014_test_triggers_normal/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/014_test_triggers_normal/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1211 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/014_test_triggers_normal/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.421381 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/014_test_triggers_normal/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      358 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/014_test_triggers_normal/tasks/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      345 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/014_test_triggers_normal/tasks/module02.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.421798 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/015_test_triggers_no_dir/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/015_test_triggers_no_dir/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1151 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/015_test_triggers_no_dir/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.422011 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/015_test_triggers_no_dir/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      358 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/015_test_triggers_no_dir/tasks/module01.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.422549 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/016_test_triggers_error/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/016_test_triggers_error/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1211 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/016_test_triggers_error/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.422812 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/016_test_triggers_error/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      773 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/016_test_triggers_error/tasks/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/016_test_triggers_error/utils.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.423363 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/017_test_triggers_extra_key/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/017_test_triggers_extra_key/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1211 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/017_test_triggers_extra_key/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.423677 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/017_test_triggers_extra_key/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      773 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/017_test_triggers_extra_key/tasks/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/017_test_triggers_extra_key/utils.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.424203 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/018_test_triggers_no_include/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/018_test_triggers_no_include/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1211 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/018_test_triggers_no_include/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.424514 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/018_test_triggers_no_include/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      773 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/018_test_triggers_no_include/tasks/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/018_test_triggers_no_include/utils.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.424792 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/019_dec_targets/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/019_dec_targets/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1211 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/019_dec_targets/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.425111 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/019_dec_targets/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      578 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/019_dec_targets/tasks/extract.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      620 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/019_dec_targets/tasks/load.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.425531 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/020_dec_retries/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/020_dec_retries/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1211 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/020_dec_retries/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.425933 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/020_dec_retries/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      399 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/020_dec_retries/tasks/extract.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      703 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/020_dec_retries/tasks/load.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/020_dec_retries/utils.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.426219 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/021_project_with_local_tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/021_project_with_local_tasks/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/021_project_with_local_tasks/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.426564 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/021_project_with_local_tasks/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      628 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/021_project_with_local_tasks/tasks/extract.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      952 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/021_project_with_local_tasks/tasks/transform_load.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.426833 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.427342 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      388 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/tasks/extract.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      785 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/tasks/transform_load.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.428013 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/common/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/common/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      376 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/common/functions.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    54103 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_run.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    14051 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_spark_submit.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5594 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_targets.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.431035 prism-ds-0.2.0rc2/prism/tests/unit/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc2/prism/tests/unit/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.431328 prism-ds-0.2.0rc2/prism/tests/unit/dummy_modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc2/prism/tests/unit/dummy_modules/dummy_module1.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    13721 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_adapter_profile.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.431498 prism-ds-0.2.0rc2/prism/tests/unit/test_agent/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1230 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_agent/prism_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10244 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_agents.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    28403 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_dag_fns.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.431701 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       65 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.432778 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/dag_cycle/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      239 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/dag_cycle/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/dag_cycle/moduleA.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      173 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/dag_cycle/moduleB.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      150 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/dag_cycle/moduleC.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      204 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/dag_cycle/moduleD.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      204 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/dag_cycle/moduleE.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.436005 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      467 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      125 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      146 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      172 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task05.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task06.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      365 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task07.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task08.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      169 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task09.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task10.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      179 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task11.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task12.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task13.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      150 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task14.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      150 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task15.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.436777 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_3nodes/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_3nodes/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      123 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_3nodes/task01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      146 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_3nodes/task02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      145 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_3nodes/task03.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.440008 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      247 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/taskA.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      148 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/taskB.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      148 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/taskC.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/taskD.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/taskE.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.440985 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_norefs/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      251 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_norefs/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleA.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleB.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleC.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleD.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleE.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.441872 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_selfref/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      253 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_selfref/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleA.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleB.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleC.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleD.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleE.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    25008 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_ast_parser.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      405 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_import.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4992 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_jinja.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.443367 prism-ds-0.2.0rc2/prism/tests/unit/test_prism_project_py/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_prism_project_py/bad_trigger_key.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      915 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_prism_project_py/multiple_profiles.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      879 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_prism_project_py/no_profile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      909 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_prism_project_py/non_null_profile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      894 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_prism_project_py/null_profile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1000 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_prism_project_py/on_failure_triggers_only.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1000 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_prism_project_py/on_success_triggers_only.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      996 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_prism_project_py/triggers_normal.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7948 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.448652 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      133 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/cls_bad_run_extra_arg.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      117 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/cls_bad_run_missing_arg.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      125 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/cls_bad_run_no_tasks.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      123 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/cls_diff_import_structure.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      163 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/cls_if_name_main.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/cls_multiple_prism_tasks.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      118 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/cls_no_prism_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      111 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/cls_no_run_func.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      123 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/cls_one_prism_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      185 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/cls_other_classes.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      346 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/cls_task_with_target.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      329 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/cls_tasks_refs.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       92 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/dec_bad_dec_no_parentheses.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      105 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/dec_bad_run_extra_arg.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       87 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/dec_bad_run_missing_arg.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      124 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/dec_diff_decorator_structure.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      156 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/dec_multiple_prism_tasks.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       49 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/dec_no_prism_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       93 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/dec_one_prism_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/dec_other_functions.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      301 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/dec_task_with_target.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      361 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/dec_tasks_refs.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.449669 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/refd_tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      116 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/refd_tasks/func_0.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      116 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/refd_tasks/func_1.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      116 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/refd_tasks/hello.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      116 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/refd_tasks/world.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     8773 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_trigger.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.450142 prism-ds-0.2.0rc2/prism/tests/unit/test_trigger_yml/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      936 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_trigger_yml/prism_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      111 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_trigger_yml/test_fn.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.450433 prism-ds-0.2.0rc2/prism/triggers/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    19492 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/triggers/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      810 2023-05-04 14:39:42.000000 prism-ds-0.2.0rc2/prism/ui.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.452396 prism-ds-0.2.0rc2/prism_ds.egg-info/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5536 2023-07-20 02:38:10.000000 prism-ds-0.2.0rc2/prism_ds.egg-info/PKG-INFO
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    19334 2023-07-20 02:38:10.000000 prism-ds-0.2.0rc2/prism_ds.egg-info/SOURCES.txt
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        1 2023-07-20 02:38:10.000000 prism-ds-0.2.0rc2/prism_ds.egg-info/dependency_links.txt
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       44 2023-07-20 02:38:10.000000 prism-ds-0.2.0rc2/prism_ds.egg-info/entry_points.txt
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        1 2023-06-26 13:49:56.000000 prism-ds-0.2.0rc2/prism_ds.egg-info/not-zip-safe
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      550 2023-07-20 02:38:10.000000 prism-ds-0.2.0rc2/prism_ds.egg-info/requires.txt
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       11 2023-07-20 02:38:10.000000 prism-ds-0.2.0rc2/prism_ds.egg-info/top_level.txt
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      743 2022-11-12 14:33:04.000000 prism-ds-0.2.0rc2/pyproject.toml
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1754 2023-07-20 02:38:10.453360 prism-ds-0.2.0rc2/setup.cfg
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       70 2023-05-04 13:05:27.000000 prism-ds-0.2.0rc2/setup.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.623278 prism-ds-0.2.1/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    11312 2022-08-08 04:50:27.000000 prism-ds-0.2.1/LICENSE
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      219 2023-05-16 12:01:01.000000 prism-ds-0.2.1/MANIFEST.in
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5522 2023-08-02 01:51:02.623398 prism-ds-0.2.1/PKG-INFO
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4561 2023-07-20 13:03:06.000000 prism-ds-0.2.1/README.md
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.431580 prism-ds-0.2.1/prism/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-17 00:34:22.000000 prism-ds-0.2.1/prism/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/admin.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.433341 prism-ds-0.2.1/prism/agents/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-ds-0.2.1/prism/agents/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7762 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/agents/base.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    18549 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/agents/docker_agent.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    43144 2023-07-22 18:17:28.000000 prism-ds-0.2.1/prism/agents/ec2.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      533 2023-04-04 01:59:51.000000 prism-ds-0.2.1/prism/agents/meta.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.434233 prism-ds-0.2.1/prism/agents/scripts/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-05-16 12:00:13.000000 prism-ds-0.2.1/prism/agents/scripts/__init__.py
+-rwxr-xr-x   0 mihirtrivedi   (501) staff       (20)     3447 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/agents/scripts/apply.sh
+-rwxr-xr-x   0 mihirtrivedi   (501) staff       (20)      710 2023-06-28 01:05:16.000000 prism-ds-0.2.1/prism/agents/scripts/run.sh
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.437209 prism-ds-0.2.1/prism/cli/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.1/prism/cli/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10729 2023-07-22 13:39:04.000000 prism-ds-0.2.1/prism/cli/agent.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7470 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/cli/base.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10421 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/cli/compile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4457 2023-06-28 00:14:15.000000 prism-ds-0.2.1/prism/cli/connect.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4222 2023-06-28 00:14:15.000000 prism-ds-0.2.1/prism/cli/create_agent.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4817 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/cli/create_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4444 2023-06-28 00:14:15.000000 prism-ds-0.2.1/prism/cli/create_trigger.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5443 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/cli/graph.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5506 2023-06-28 00:14:15.000000 prism-ds-0.2.1/prism/cli/init.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     9402 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/cli/run.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      724 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/cli/spark_submit.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.437466 prism-ds-0.2.1/prism/client/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    16701 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/client/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4970 2023-08-02 01:20:09.000000 prism-ds-0.2.1/prism/constants.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.438182 prism-ds-0.2.1/prism/decorators/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      116 2023-05-26 22:30:47.000000 prism-ds-0.2.1/prism/decorators/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7124 2023-05-26 22:30:47.000000 prism-ds-0.2.1/prism/decorators/target.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3116 2023-05-26 22:30:47.000000 prism-ds-0.2.1/prism/decorators/task.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.438412 prism-ds-0.2.1/prism/docs/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       79 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/docs/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.442170 prism-ds-0.2.1/prism/docs/build/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    50665 2023-07-18 21:18:50.000000 prism-ds-0.2.1/prism/docs/build/311ea03002abadcdcaba.png
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6035 2023-07-18 21:18:50.000000 prism-ds-0.2.1/prism/docs/build/54968a39190c43d592b9.svg
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15406 2023-07-18 21:18:50.000000 prism-ds-0.2.1/prism/docs/build/737ad70b3f2d3a9b5f6e.ico
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       79 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/docs/build/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4653 2023-07-18 21:18:50.000000 prism-ds-0.2.1/prism/docs/build/ce188596011a8fa32931.png
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)   560712 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/docs/build/index.html
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      961 2023-07-18 21:18:50.000000 prism-ds-0.2.1/prism/docs/build/main.js.LICENSE.txt
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.442546 prism-ds-0.2.1/prism/event_managers/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.1/prism/event_managers/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6081 2023-07-13 03:54:01.000000 prism-ds-0.2.1/prism/event_managers/base.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7852 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/exceptions.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.444820 prism-ds-0.2.1/prism/infra/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.1/prism/infra/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6833 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/infra/compiled_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    14303 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/infra/compiler.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    13388 2023-08-02 01:20:09.000000 prism-ds-0.2.1/prism/infra/executor.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3900 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/infra/hooks.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2704 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/infra/manifest.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3716 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/infra/pipeline.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    17198 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/infra/project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1421 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/infra/sys_path.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2628 2023-07-31 12:18:05.000000 prism-ds-0.2.1/prism/infra/task_manager.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    24529 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/main.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.447147 prism-ds-0.2.1/prism/mixins/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-ds-0.2.1/prism/mixins/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2405 2023-04-04 01:59:51.000000 prism-ds-0.2.1/prism/mixins/agent.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3165 2023-07-22 18:17:28.000000 prism-ds-0.2.1/prism/mixins/aws.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1288 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/mixins/base.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    11668 2023-07-31 12:14:11.000000 prism-ds-0.2.1/prism/mixins/compile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7301 2023-06-28 00:14:15.000000 prism-ds-0.2.1/prism/mixins/connect.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2312 2023-06-28 00:14:15.000000 prism-ds-0.2.1/prism/mixins/create_agent.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5706 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/mixins/create_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5428 2023-06-28 00:14:15.000000 prism-ds-0.2.1/prism/mixins/create_trigger.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2438 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/mixins/graph.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1107 2023-04-02 17:52:18.000000 prism-ds-0.2.1/prism/mixins/run.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4232 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/mixins/sys_handler.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.447859 prism-ds-0.2.1/prism/parsers/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.1/prism/parsers/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    31631 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/parsers/ast_parser.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2206 2023-07-15 21:15:27.000000 prism-ds-0.2.1/prism/parsers/base.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3049 2023-04-04 01:59:51.000000 prism-ds-0.2.1/prism/parsers/yml_parser.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    22013 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/prism_logging.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.450070 prism-ds-0.2.1/prism/profiles/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.1/prism/profiles/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2745 2023-04-04 01:59:51.000000 prism-ds-0.2.1/prism/profiles/adapter.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3733 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/profiles/bigquery.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15570 2023-08-01 03:49:48.000000 prism-ds-0.2.1/prism/profiles/dbt.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      539 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/profiles/meta.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4567 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/profiles/postgres.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     9117 2023-07-05 11:15:15.000000 prism-ds-0.2.1/prism/profiles/profile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4089 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/profiles/pyspark.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4557 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/profiles/redshift.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4176 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/profiles/snowflake.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6358 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/profiles/trino.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.450596 prism-ds-0.2.1/prism/spark/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.1/prism/spark/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      439 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/spark/script.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2889 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/spark/wrapper.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1448 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/target.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5171 2023-06-28 00:14:15.000000 prism-ds-0.2.1/prism/task.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.450753 prism-ds-0.2.1/prism/templates/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-17 00:55:51.000000 prism-ds-0.2.1/prism/templates/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.451404 prism-ds-0.2.1/prism/templates/agents/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       59 2023-04-04 01:59:51.000000 prism-ds-0.2.1/prism/templates/agents/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      233 2023-04-04 01:59:51.000000 prism-ds-0.2.1/prism/templates/agents/docker.yml
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      191 2023-05-20 15:36:38.000000 prism-ds-0.2.1/prism/templates/agents/ec2.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.451978 prism-ds-0.2.1/prism/templates/minimal_project/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       19 2022-08-16 12:31:03.000000 prism-ds-0.2.1/prism/templates/minimal_project/.gitignore
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/templates/minimal_project/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1326 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/templates/minimal_project/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.452328 prism-ds-0.2.1/prism/templates/minimal_project/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1011 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/templates/minimal_project/tasks/class_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      937 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/templates/minimal_project/tasks/decorated_task.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.452496 prism-ds-0.2.1/prism/templates/profile/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       61 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/templates/profile/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.452807 prism-ds-0.2.1/prism/templates/profile/bigquery/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      148 2023-05-26 22:30:47.000000 prism-ds-0.2.1/prism/templates/profile/bigquery/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.453107 prism-ds-0.2.1/prism/templates/profile/dbt/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      141 2023-05-26 22:30:47.000000 prism-ds-0.2.1/prism/templates/profile/dbt/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.453345 prism-ds-0.2.1/prism/templates/profile/postgres/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      180 2023-05-26 22:30:47.000000 prism-ds-0.2.1/prism/templates/profile/postgres/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.453510 prism-ds-0.2.1/prism/templates/profile/pyspark/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      478 2023-05-26 22:30:47.000000 prism-ds-0.2.1/prism/templates/profile/pyspark/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.453670 prism-ds-0.2.1/prism/templates/profile/redshift/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      180 2023-05-26 22:30:47.000000 prism-ds-0.2.1/prism/templates/profile/redshift/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.453832 prism-ds-0.2.1/prism/templates/profile/snowflake/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      193 2023-05-26 22:30:47.000000 prism-ds-0.2.1/prism/templates/profile/snowflake/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.453985 prism-ds-0.2.1/prism/templates/profile/trino/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      189 2023-05-26 22:30:47.000000 prism-ds-0.2.1/prism/templates/profile/trino/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.454612 prism-ds-0.2.1/prism/templates/starter_project/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       19 2022-08-08 04:50:27.000000 prism-ds-0.2.1/prism/templates/starter_project/.gitignore
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/templates/starter_project/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.454898 prism-ds-0.2.1/prism/templates/starter_project/data/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-ds-0.2.1/prism/templates/starter_project/data/.exists
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.455007 prism-ds-0.2.1/prism/templates/starter_project/dev/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      786 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/templates/starter_project/dev/dev.ipynb
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.455174 prism-ds-0.2.1/prism/templates/starter_project/output/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-ds-0.2.1/prism/templates/starter_project/output/.exists
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1112 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/templates/starter_project/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.455454 prism-ds-0.2.1/prism/templates/starter_project/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1011 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/templates/starter_project/tasks/class_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      938 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/templates/starter_project/tasks/decorated_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       66 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/templates/starter_project/utils.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.456563 prism-ds-0.2.1/prism/templates/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      426 2023-05-27 16:07:03.000000 prism-ds-0.2.1/prism/templates/tasks/pyspark_cls.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      427 2023-05-27 16:07:03.000000 prism-ds-0.2.1/prism/templates/tasks/pyspark_dec.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      426 2023-05-27 16:07:03.000000 prism-ds-0.2.1/prism/templates/tasks/python_cls.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      427 2023-05-27 16:07:03.000000 prism-ds-0.2.1/prism/templates/tasks/python_dec.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      155 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/templates/tasks/sql.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.457052 prism-ds-0.2.1/prism/templates/triggers/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       61 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/templates/triggers/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      267 2023-04-04 01:59:51.000000 prism-ds-0.2.1/prism/templates/triggers/function.yml
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      208 2023-04-04 01:59:51.000000 prism-ds-0.2.1/prism/templates/triggers/prism_project.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.457245 prism-ds-0.2.1/prism/tests/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.1/prism/tests/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.460271 prism-ds-0.2.1/prism/tests/integration/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.1/prism/tests/integration/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7886 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/integration_test_class.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15381 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_client.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10484 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_compile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10444 2023-06-28 00:14:15.000000 prism-ds-0.2.1/prism/tests/integration/test_connect.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6512 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_create.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4012 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_dbt.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5728 2023-08-01 13:15:50.000000 prism-ds-0.2.1/prism/tests/integration/test_hooks.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4539 2023-05-30 01:42:39.000000 prism-ds-0.2.1/prism/tests/integration/test_init.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.425999 prism-ds-0.2.1/prism/tests/integration/test_projects/
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.461343 prism-ds-0.2.1/prism/tests/integration/test_projects/001_init/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/001_init/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1120 2023-08-01 03:53:18.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/001_init/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.462126 prism-ds-0.2.1/prism/tests/integration/test_projects/001_init/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1011 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/001_init/tasks/class_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      938 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/001_init/tasks/decorated_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       66 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/001_init/utils.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.462557 prism-ds-0.2.1/prism/tests/integration/test_projects/001a_init_minimal/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/001a_init_minimal/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1343 2023-08-01 03:53:18.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/001a_init_minimal/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.463131 prism-ds-0.2.1/prism/tests/integration/test_projects/001a_init_minimal/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1011 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/001a_init_minimal/tasks/class_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      937 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/001a_init_minimal/tasks/decorated_task.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.463425 prism-ds-0.2.1/prism/tests/integration/test_projects/002_no_project_py/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/002_no_project_py/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      772 2022-08-08 04:50:27.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/002_no_project_py/functions.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.464090 prism-ds-0.2.1/prism/tests/integration/test_projects/002_no_project_py/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      825 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/002_no_project_py/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      857 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/002_no_project_py/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      857 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/002_no_project_py/modules/module03.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.464365 prism-ds-0.2.1/prism/tests/integration/test_projects/003_project_with_cycle/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/003_project_with_cycle/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.464861 prism-ds-0.2.1/prism/tests/integration/test_projects/003_project_with_cycle/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      773 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/003_project_with_cycle/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      806 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/003_project_with_cycle/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      807 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/003_project_with_cycle/modules/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/003_project_with_cycle/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.465111 prism-ds-0.2.1/prism/tests/integration/test_projects/004_simple_project/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/004_simple_project/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.466439 prism-ds-0.2.1/prism/tests/integration/test_projects/004_simple_project/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      935 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/004_simple_project/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1027 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/004_simple_project/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      801 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/004_simple_project/modules/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1033 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/004_simple_project/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.467453 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_modules/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      772 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_modules/functions.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.468294 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1100 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      868 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      808 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_modules/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.471493 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      772 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/functions.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.477865 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1127 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      923 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      913 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module04.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.481120 prism-ds-0.2.1/prism/tests/integration/test_projects/006_simple_project_with_profile/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/006_simple_project_with_profile/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.486764 prism-ds-0.2.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      969 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1090 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      974 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      910 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1257 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/006_simple_project_with_profile/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.487861 prism-ds-0.2.1/prism/tests/integration/test_projects/007_spark_project/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/007_spark_project/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1073 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/007_spark_project/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.495540 prism-ds-0.2.1/prism/tests/integration/test_projects/007_spark_project/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1751 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/007_spark_project/tasks/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1139 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/007_spark_project/tasks/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      940 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/007_spark_project/tasks/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      636 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/007_spark_project/tasks/module04.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.496498 prism-ds-0.2.1/prism/tests/integration/test_projects/008_targets/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/008_targets/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1073 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/008_targets/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.504216 prism-ds-0.2.1/prism/tests/integration/test_projects/008_targets/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      982 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/008_targets/tasks/csv.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1548 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/008_targets/tasks/csv_iter.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1632 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/008_targets/tasks/csv_mult.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1765 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/008_targets/tasks/parquet.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      498 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/008_targets/tasks/txt.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.508391 prism-ds-0.2.1/prism/tests/integration/test_projects/009_simple_dbt_project/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/009_simple_dbt_project/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.508528 prism-ds-0.2.1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1073 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.509054 prism-ds-0.2.1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      569 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/tasks/bad_adapter.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      576 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/tasks/filter_customers.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.515156 prism-ds-0.2.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.515594 prism-ds-0.2.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.522136 prism-ds-0.2.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      934 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1059 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module02.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.522403 prism-ds-0.2.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      875 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      812 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.525616 prism-ds-0.2.1/prism/tests/integration/test_projects/011_bad_task_ref/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-07-09 15:09:25.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/011_bad_task_ref/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.525948 prism-ds-0.2.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.526330 prism-ds-0.2.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      934 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1067 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module02.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.526516 prism-ds-0.2.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      875 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      812 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/011_bad_task_ref/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.526820 prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.529696 prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1196 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1195 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1045 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency/modules/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      808 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency/modules/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.532132 prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency_local/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency_local/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency_local/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.540889 prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency_local/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1239 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency_local/tasks/local_tasks.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      597 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency_local/tasks/non_local_task.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.541371 prism-ds-0.2.1/prism/tests/integration/test_projects/013_hooks_sql_spark/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/013_hooks_sql_spark/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.543667 prism-ds-0.2.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1287 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/bad_adapter.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1133 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/postgres.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1871 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/snowflake.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2147 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/spark.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1073 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/013_hooks_sql_spark/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.543963 prism-ds-0.2.1/prism/tests/integration/test_projects/014_test_triggers_normal/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/014_test_triggers_normal/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1211 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/014_test_triggers_normal/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.544982 prism-ds-0.2.1/prism/tests/integration/test_projects/014_test_triggers_normal/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      358 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/014_test_triggers_normal/tasks/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      345 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/014_test_triggers_normal/tasks/module02.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.547303 prism-ds-0.2.1/prism/tests/integration/test_projects/015_test_triggers_no_dir/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/015_test_triggers_no_dir/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1151 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/015_test_triggers_no_dir/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.548605 prism-ds-0.2.1/prism/tests/integration/test_projects/015_test_triggers_no_dir/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      358 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/015_test_triggers_no_dir/tasks/module01.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.555398 prism-ds-0.2.1/prism/tests/integration/test_projects/016_test_triggers_error/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/016_test_triggers_error/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1211 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/016_test_triggers_error/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.555874 prism-ds-0.2.1/prism/tests/integration/test_projects/016_test_triggers_error/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      773 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/016_test_triggers_error/tasks/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/016_test_triggers_error/utils.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.556384 prism-ds-0.2.1/prism/tests/integration/test_projects/017_test_triggers_extra_key/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/017_test_triggers_extra_key/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1211 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/017_test_triggers_extra_key/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.556674 prism-ds-0.2.1/prism/tests/integration/test_projects/017_test_triggers_extra_key/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      773 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/017_test_triggers_extra_key/tasks/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-04-04 01:59:51.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/017_test_triggers_extra_key/utils.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.557122 prism-ds-0.2.1/prism/tests/integration/test_projects/018_test_triggers_no_include/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/018_test_triggers_no_include/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1211 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/018_test_triggers_no_include/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.559756 prism-ds-0.2.1/prism/tests/integration/test_projects/018_test_triggers_no_include/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      773 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/018_test_triggers_no_include/tasks/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-04-04 01:59:51.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/018_test_triggers_no_include/utils.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.560145 prism-ds-0.2.1/prism/tests/integration/test_projects/019_dec_targets/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-05-26 22:30:47.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/019_dec_targets/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1211 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/019_dec_targets/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.560503 prism-ds-0.2.1/prism/tests/integration/test_projects/019_dec_targets/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      578 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/019_dec_targets/tasks/extract.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      620 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/019_dec_targets/tasks/load.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.560959 prism-ds-0.2.1/prism/tests/integration/test_projects/020_dec_retries/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-05-26 22:30:47.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/020_dec_retries/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1211 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/020_dec_retries/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.561388 prism-ds-0.2.1/prism/tests/integration/test_projects/020_dec_retries/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      399 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/020_dec_retries/tasks/extract.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      703 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/020_dec_retries/tasks/load.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-05-26 22:30:47.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/020_dec_retries/utils.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.561684 prism-ds-0.2.1/prism/tests/integration/test_projects/021_project_with_local_tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/021_project_with_local_tasks/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/021_project_with_local_tasks/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.562315 prism-ds-0.2.1/prism/tests/integration/test_projects/021_project_with_local_tasks/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      687 2023-07-22 18:17:28.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/021_project_with_local_tasks/tasks/extract.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      995 2023-07-22 18:17:28.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/021_project_with_local_tasks/tasks/transform_load.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.562724 prism-ds-0.2.1/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.563033 prism-ds-0.2.1/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      388 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/tasks/extract.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      785 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/tasks/transform_load.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.563299 prism-ds-0.2.1/prism/tests/integration/test_projects/common/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/common/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      376 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/common/functions.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    54115 2023-07-22 18:17:28.000000 prism-ds-0.2.1/prism/tests/integration/test_run.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    14051 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_spark_submit.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5594 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_targets.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.568903 prism-ds-0.2.1/prism/tests/unit/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.1/prism/tests/unit/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.572845 prism-ds-0.2.1/prism/tests/unit/dummy_modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-ds-0.2.1/prism/tests/unit/dummy_modules/dummy_module1.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    13721 2023-06-28 00:14:15.000000 prism-ds-0.2.1/prism/tests/unit/test_adapter_profile.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.572963 prism-ds-0.2.1/prism/tests/unit/test_agent/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1230 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_agent/prism_project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10244 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_agents.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    28403 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_dag_fns.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.573223 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       65 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.577953 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/dag_cycle/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      239 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/dag_cycle/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/dag_cycle/moduleA.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      173 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/dag_cycle/moduleB.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      150 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/dag_cycle/moduleC.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      204 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/dag_cycle/moduleD.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      204 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/dag_cycle/moduleE.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.584243 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      467 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      125 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      146 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      172 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task05.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task06.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      365 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task07.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task08.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      169 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task09.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task10.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      179 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task11.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task12.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task13.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      150 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task14.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      150 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task15.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.584840 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_3nodes/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_3nodes/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      123 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_3nodes/task01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      146 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_3nodes/task02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      145 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_3nodes/task03.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.592323 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      247 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/taskA.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      148 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/taskB.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      148 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/taskC.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/taskD.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/taskE.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.602033 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_norefs/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      251 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_norefs/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleA.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleB.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleC.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleD.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleE.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.607573 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_selfref/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      253 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_selfref/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleA.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleB.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleC.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleD.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleE.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    25008 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_ast_parser.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      405 2022-08-08 04:50:27.000000 prism-ds-0.2.1/prism/tests/unit/test_import.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4992 2023-05-26 22:30:47.000000 prism-ds-0.2.1/prism/tests/unit/test_jinja.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.611924 prism-ds-0.2.1/prism/tests/unit/test_prism_project_py/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_prism_project_py/bad_trigger_key.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      915 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/unit/test_prism_project_py/multiple_profiles.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      879 2022-08-08 04:50:27.000000 prism-ds-0.2.1/prism/tests/unit/test_prism_project_py/no_profile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      909 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/unit/test_prism_project_py/non_null_profile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      894 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/unit/test_prism_project_py/null_profile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1000 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_prism_project_py/on_failure_triggers_only.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1000 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_prism_project_py/on_success_triggers_only.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      996 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_prism_project_py/triggers_normal.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7948 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.619099 prism-ds-0.2.1/prism/tests/unit/test_tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      133 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/cls_bad_run_extra_arg.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      117 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/cls_bad_run_missing_arg.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      125 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/cls_bad_run_no_tasks.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      123 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/cls_diff_import_structure.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      163 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/cls_if_name_main.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/cls_multiple_prism_tasks.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      118 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/cls_no_prism_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      111 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/cls_no_run_func.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      123 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/cls_one_prism_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      185 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/cls_other_classes.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      346 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/cls_task_with_target.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      329 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/cls_tasks_refs.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       92 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/dec_bad_dec_no_parentheses.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      105 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/dec_bad_run_extra_arg.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       87 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/dec_bad_run_missing_arg.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      124 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/dec_diff_decorator_structure.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      156 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/dec_multiple_prism_tasks.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       49 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/dec_no_prism_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       93 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/dec_one_prism_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/dec_other_functions.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      301 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/dec_task_with_target.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      361 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/dec_tasks_refs.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.620457 prism-ds-0.2.1/prism/tests/unit/test_tasks/refd_tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      116 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/refd_tasks/func_0.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      116 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/refd_tasks/func_1.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      116 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/refd_tasks/hello.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      116 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/refd_tasks/world.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     8773 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_trigger.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.621592 prism-ds-0.2.1/prism/tests/unit/test_trigger_yml/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      936 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_trigger_yml/prism_project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      111 2023-04-04 01:59:51.000000 prism-ds-0.2.1/prism/tests/unit/test_trigger_yml/test_fn.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.621857 prism-ds-0.2.1/prism/triggers/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    19492 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/triggers/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      810 2023-05-04 14:39:42.000000 prism-ds-0.2.1/prism/ui.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.623169 prism-ds-0.2.1/prism_ds.egg-info/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5522 2023-08-02 01:51:02.000000 prism-ds-0.2.1/prism_ds.egg-info/PKG-INFO
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    19334 2023-08-02 01:51:02.000000 prism-ds-0.2.1/prism_ds.egg-info/SOURCES.txt
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        1 2023-08-02 01:51:02.000000 prism-ds-0.2.1/prism_ds.egg-info/dependency_links.txt
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       44 2023-08-02 01:51:02.000000 prism-ds-0.2.1/prism_ds.egg-info/entry_points.txt
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        1 2023-06-26 13:49:56.000000 prism-ds-0.2.1/prism_ds.egg-info/not-zip-safe
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      564 2023-08-02 01:51:02.000000 prism-ds-0.2.1/prism_ds.egg-info/requires.txt
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       11 2023-08-02 01:51:02.000000 prism-ds-0.2.1/prism_ds.egg-info/top_level.txt
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      743 2022-11-12 14:33:04.000000 prism-ds-0.2.1/pyproject.toml
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1766 2023-08-02 01:51:02.623823 prism-ds-0.2.1/setup.cfg
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       70 2023-05-04 13:05:27.000000 prism-ds-0.2.1/setup.py
```

### Comparing `prism-ds-0.2.0rc2/LICENSE` & `prism-ds-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/PKG-INFO` & `prism-ds-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prism-ds
-Version: 0.2.0rc2
+Version: 0.2.1
 Summary: The easiest way to create data pipelines in Python.
 Author: prism founders
 Author-email: hello@runprism.com
 License: Apache-2.0
 Project-URL: homepage, https://www.runprism.com
 Project-URL: documentation, https://docs.runprism.com
 Project-URL: repository, https://github.com/runprism/prism
@@ -27,15 +27,15 @@
 Provides-Extra: pyspark
 Provides-Extra: dbt
 Provides-Extra: docker
 Provides-Extra: testing
 License-File: LICENSE
 
 <p align="center">
-  <img src="https://github.com/runprism/prism/raw/main/.github/prism_logo_light.png" alt="prism logo" width="350"/>
+  <img src="https://github.com/runprism/prism/raw/main/.github/Logo.png" alt="prism logo" height="100"/>
 </p>
 <p align="center">
     <a href="https://pypi.python.org/pypi/prism-ds/" alt="PyPI version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/prism-ds?color=2081c1&labelColor=090422"></a>
     <a href="https://pepy.tech/badge/prism-ds/" alt="Downloads">
         <img src="https://static.pepy.tech/personalized-badge/prism-ds?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads"/>
     </a>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: prism-ds Version: 0.2.0rc2 Summary: The easiest way
-to create data pipelines in Python. Author: prism founders Author-email:
+Metadata-Version: 2.1 Name: prism-ds Version: 0.2.1 Summary: The easiest way to
+create data pipelines in Python. Author: prism founders Author-email:
 hello@runprism.com License: Apache-2.0 Project-URL: homepage, https://
 www.runprism.com Project-URL: documentation, https://docs.runprism.com Project-
 URL: repository, https://github.com/runprism/prism Platform: unix Platform:
 linux Platform: osx Platform: win32 Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Requires-Python: >=3.7
```

### Comparing `prism-ds-0.2.0rc2/README.md` & `prism-ds-0.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center">
-  <img src="https://github.com/runprism/prism/raw/main/.github/prism_logo_light.png" alt="prism logo" width="350"/>
+  <img src="https://github.com/runprism/prism/raw/main/.github/Logo.png" alt="prism logo" height="100"/>
 </p>
 <p align="center">
     <a href="https://pypi.python.org/pypi/prism-ds/" alt="PyPI version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/prism-ds?color=2081c1&labelColor=090422"></a>
     <a href="https://pepy.tech/badge/prism-ds/" alt="Downloads">
         <img src="https://static.pepy.tech/personalized-badge/prism-ds?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads"/>
     </a>
```

### Comparing `prism-ds-0.2.0rc2/prism/admin.py` & `prism-ds-0.2.1/prism/admin.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/agents/base.py` & `prism-ds-0.2.1/prism/agents/base.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/agents/docker_agent.py` & `prism-ds-0.2.1/prism/agents/docker_agent.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/agents/ec2.py` & `prism-ds-0.2.1/prism/agents/ec2.py`

 * *Files 10% similar despite different names*

```diff
@@ -117,14 +117,91 @@
 
         args:
             data: data to write to JSON
         """
         with open(Path(prism.constants.INTERNAL_FOLDER) / 'ec2.json', 'w') as f:
             json.dump(data, f)
 
+    def update_json(self, data: Dict[str, Dict[str, Any]]):
+        """
+        Update ~/.prism/ec2.json
+
+        args:
+            ...
+        """
+        json_path = Path(prism.constants.INTERNAL_FOLDER) / 'ec2.json'
+        if not json_path.is_file():
+            self.write_json(data)
+            return data
+        else:
+            with open(json_path, 'r') as f:
+                json_data = json.loads(f.read())
+            f.close()
+
+            # Update the data
+            for key in ["resources", "files"]:
+                if key in list(data.keys()):
+                    json_data[key].update(data[key])
+
+            # Write the json
+            self.write_json(json_data)
+            return json_data
+
+    def delete_resources_in_json(self) -> Dict[str, str]:
+        """
+        Delete all resources found in the JSON
+        """
+        del_resources: Dict[str, str] = {}
+        json_path = Path(prism.constants.INTERNAL_FOLDER) / 'ec2.json'
+        if not json_path.is_file():
+            return del_resources
+        else:
+            with open(json_path, 'r') as f:
+                json_data = json.loads(f.read())
+            f.close()
+
+            # Resources and files
+            resources = json_data["resources"]
+            files = json_data["files"]
+
+            # Key name
+            if "key_name" in resources.keys():
+                pem_key_path = files["pem_key_path"]
+                self.ec2_client.delete_key_pair(
+                    KeyName=resources["key_name"]
+                )
+                os.unlink(str(pem_key_path))
+                del_resources["PEM key"] = resources["key_name"]
+
+            # Instance
+            if "instance_id" in resources.keys():
+                self.ec2_client.terminate_instances(
+                    InstanceIds=[resources["instance_id"]]
+                )
+                del_resources["instance"] = resources["instance_id"]
+
+            # Security group
+            if "security_group_id" in resources.keys():
+                while True:
+                    try:
+                        self.ec2_client.delete_security_group(
+                            GroupId=resources["security_group_id"]
+                        )
+                        break
+                    except botocore.exceptions.ClientError as e:
+                        if "DependencyViolation" in str(e):
+                            time.sleep(5)
+                        else:
+                            raise e
+
+                del_resources["security group"] = resources["security_group_id"]
+
+        os.unlink(json_path)
+        return del_resources
+
     def is_valid_conf(self, agent_conf: Dict[str, Any]):
         """
         A EC2 agent should be formatted as follows:
 
         agent:
           type: ec2
           pem_key_path: <path to PEM key>
@@ -412,22 +489,34 @@
         response = ec2_client.create_security_group(
             GroupName=instance_name,
             Description=f'VPC for {instance_name} EC2 agent',
             VpcId=vpc_id
         )
         security_group_id = response['GroupId']
 
-        # IP address
-        external_ip = urllib.request.urlopen('https://ident.me').read().decode('utf8')
-        self.add_ingress_rule(
-            ec2_client,
-            security_group_id,
-            external_ip
-        )
-        return security_group_id, vpc_id
+        # Add an ingress rule
+        try:
+            external_ip = urllib.request.urlopen('https://ident.me').read().decode('utf8')  # noqa: E501
+            self.add_ingress_rule(
+                ec2_client,
+                security_group_id,
+                external_ip
+            )
+            return security_group_id, vpc_id
+
+        # If we encounter an error, first delete the newly created security group. Then
+        # raise the exception.
+        except Exception as e:
+
+            # The security group shouldn't be attached to an instance at this point, so
+            # we are safe to just delete it.
+            ec2_client.delete_security_group(
+                GroupId=security_group_id
+            )
+            raise e
 
     def check_ingress_ip(self,
         ec2_client: Any,
         security_group_id: str
     ):
         """
         Confirm that the ingress rule for `security_group_id` allows for SSH traffic
@@ -493,184 +582,208 @@
             ec2_resource: Boto3 AWS EC2 resource
             instance_id: EC2 instance ID
             instance_name: name of EC2 instance
             instance_type: EC2 instance types
         returns:
             EC2 response
         """
-        # Data to write
-        data = {}
+        # Wrap the whole thing in a single try-except block
+        try:
 
-        # Check resources
-        resources = self.check_resources(ec2_client, instance_name, instance_id)
+            # Data to write
+            data = {}
 
-        # Log prefix
-        log_prefix = f"{prism.ui.AGENT_EVENT}{instance_name}{prism.ui.AGENT_WHICH_BUILD}[build]{prism.ui.RESET}"  # noqa: E501
+            # Check resources
+            resources = self.check_resources(ec2_client, instance_name, instance_id)
 
-        def _create_exception(resource):
-            return prism.exceptions.AwsException('\n'.join([
-                f"{resource} exists, but ~/.prism/ec2.json file not found! This only happens if:",  # noqa: E501
-                f"    1. You manually created the {resource}",
-                "    2. You deleted ~/.prism/ec2.json",
-                f"Delete the {resource} from EC2 and try again!"
-            ]))
-
-        # Create PEM key pair
-        if resources["key_pair"] is None:
-            pem_key_path = self.create_key_pair(
-                ec2_client,
-                key_name=instance_name,
-            )
-            log_instance_name = f"{prism.ui.MAGENTA}{instance_name}{prism.ui.RESET}"
-            prism.prism_logging.DEFAULT_LOGGER.agent(  # type: ignore
-                f"{log_prefix} | Created key pair {log_instance_name}"
-            )
-        else:
-            # If the key-pair exists, then the location of the PEM key path should be
-            # contained in ~/.prism/ec2.json. If it isn't, then either:
-            #   1. The user manually created the key pair
-            #   2. The user deleted ~/.prism/ec2.json
-            if not Path(prism.constants.INTERNAL_FOLDER / 'ec2.json').is_file():
-                raise _create_exception("key-pair")
-            pem_key_path = self.pem_key_path
-
-            # Log
-            log_instance_name = f"{prism.ui.MAGENTA}{instance_name}{prism.ui.RESET}"  # noqa: E501
-            log_instance_path = f"{prism.ui.MAGENTA}{str(pem_key_path)}{prism.ui.RESET}"  # noqa: E501
-            prism.prism_logging.DEFAULT_LOGGER.agent(  # type: ignore
-                f"{log_prefix} | Using existing key-pair {log_instance_name} at {log_instance_path}"  # noqa: E501
-            )
+            # Log prefix
+            log_prefix = f"{prism.ui.AGENT_EVENT}{instance_name}{prism.ui.AGENT_WHICH_BUILD}[build]{prism.ui.RESET}"  # noqa: E501
 
-        # Security group
-        if resources["security_group"] is None:
-            security_group_id, vpc_id = self.create_new_security_group(
-                ec2_client,
-                instance_name
-            )
+            def _create_exception(resource):
+                return prism.exceptions.AwsException('\n'.join([
+                    f"{resource} exists, but ~/.prism/ec2.json file not found! This only happens if:",  # noqa: E501
+                    f"    1. You manually created the {resource}",
+                    "    2. You deleted ~/.prism/ec2.json",
+                    f"Delete the {resource} from EC2 and try again!"
+                ]))
+
+            # Create PEM key pair
+            if resources["key_pair"] is None:
+                pem_key_path = self.create_key_pair(
+                    ec2_client,
+                    key_name=instance_name,
+                )
+                log_instance_name = f"{prism.ui.MAGENTA}{instance_name}{prism.ui.RESET}"
+                prism.prism_logging.DEFAULT_LOGGER.agent(  # type: ignore
+                    f"{log_prefix} | Created key pair {log_instance_name}"
+                )
 
-            # Log
-            log_security_group_id = f"{prism.ui.MAGENTA}{security_group_id}{prism.ui.RESET}"  # noqa: E501
-            log_vpc_id = f"{prism.ui.MAGENTA}{vpc_id}{prism.ui.RESET}"  # noqa: E501
-            prism.prism_logging.DEFAULT_LOGGER.agent(  # type: ignore
-                f"{log_prefix} | Created security group with ID {log_security_group_id} in VPC {log_vpc_id}"  # noqa: E501
-            )
-        else:
-            if not Path(prism.constants.INTERNAL_FOLDER / 'ec2.json').is_file():
-                raise _create_exception("security group")
+                # Write the data to the JSON
+                data = {
+                    "resources": {"key_name": instance_name},
+                    "files": {"pem_key_path": str(pem_key_path)}
+                }
+                self.update_json(data)
+            else:
 
-            # Log
-            security_group_id = self.security_group_id
-            self.check_ingress_ip(ec2_client, security_group_id)
-            log_security_group_id = f"{prism.ui.MAGENTA}{security_group_id}{prism.ui.RESET}"  # noqa: E501
-            prism.prism_logging.DEFAULT_LOGGER.agent(  # type: ignore
-                f"{log_prefix} | Using existing security group {log_security_group_id}"
-            )
+                # If the key-pair exists, then the location of the PEM key path should
+                # be contained in ~/.prism/ec2.json. If it isn't, then either:
+                #   1. The user manually created the key pair
+                #   2. The user deleted ~/.prism/ec2.json
+                if not Path(prism.constants.INTERNAL_FOLDER / 'ec2.json').is_file():
+                    raise _create_exception("key-pair")
+                pem_key_path = self.pem_key_path
 
-        # Log instance ID template
-        log_instance_id_template = f"{prism.ui.MAGENTA}{{instance_id}}{prism.ui.RESET}"
+                # Log
+                log_instance_name = f"{prism.ui.MAGENTA}{instance_name}{prism.ui.RESET}"  # noqa: E501
+                log_instance_path = f"{prism.ui.MAGENTA}{str(pem_key_path)}{prism.ui.RESET}"  # noqa: E501
+                prism.prism_logging.DEFAULT_LOGGER.agent(  # type: ignore
+                    f"{log_prefix} | Using existing key-pair {log_instance_name} at {log_instance_path}"  # noqa: E501
+                )
 
-        # Instance
-        if resources["instance"] is None:
-            instance = ec2_resource.create_instances(
-                InstanceType=instance_type,
-                KeyName=instance_name,
-                MinCount=1,
-                MaxCount=1,
-                ImageId="ami-0889a44b331db0194",
-                TagSpecifications=[
-                    {
-                        'ResourceType': 'instance',
-                        'Tags': [
-                            {
-                                'Key': 'Name',
-                                'Value': instance_name
-                            },
-                        ]
-                    },
-                ],
-                SecurityGroupIds=[
-                    security_group_id
-                ]
-            )
-            instance_id = instance[0].id
+            # Security group
+            if resources["security_group"] is None:
+                security_group_id, vpc_id = self.create_new_security_group(
+                    ec2_client,
+                    instance_name
+                )
 
-            # Log
-            prism.prism_logging.DEFAULT_LOGGER.agent(  # type: ignore
-                f"{log_prefix} | Created EC2 instance with ID {log_instance_id_template.format(instance_id=instance_id)}"  # noqa: E501
-            )
-            time.sleep(1)
-        else:
-            if not Path(prism.constants.INTERNAL_FOLDER / 'ec2.json').is_file():
-                raise _create_exception("instance")
-            instance_id = self.instance_id
-
-            # Log
-            prism.prism_logging.DEFAULT_LOGGER.agent(  # type: ignore
-                f"{log_prefix} | Using existing EC2 instance with ID {log_instance_id_template.format(instance_id=instance_id)}"  # noqa: E501
-            )
+                # Log
+                log_security_group_id = f"{prism.ui.MAGENTA}{security_group_id}{prism.ui.RESET}"  # noqa: E501
+                log_vpc_id = f"{prism.ui.MAGENTA}{vpc_id}{prism.ui.RESET}"  # noqa: E501
+                prism.prism_logging.DEFAULT_LOGGER.agent(  # type: ignore
+                    f"{log_prefix} | Created security group with ID {log_security_group_id} in VPC {log_vpc_id}"  # noqa: E501
+                )
 
-        # Instance data
-        resp = self.check_instance_data(ec2_client, instance_id)
+                # Write the data to the JSON
+                data = {
+                    "resources": {"security_group_id": security_group_id},
+                }
+                self.update_json(data)
+            else:
+                if not Path(prism.constants.INTERNAL_FOLDER / 'ec2.json').is_file():
+                    raise _create_exception("security group")
 
-        # If the instance exists but its key-name is not `instance_name` (this really
-        # should never happen unless the user manually creates an EC2 instance that has
-        # the same name), then raise an error
-        if len(resp.keys()) > 0 and resp["key_name"] != instance_name:
-            raise prism.exceptions.AwsException(
-                f"unrecognized key `{resp['key_name']}`...the agent requires key `{instance_name}.pem`"  # noqa: E501
-            )
+                # Log
+                security_group_id = self.security_group_id
+                self.check_ingress_ip(ec2_client, security_group_id)
+                log_security_group_id = f"{prism.ui.MAGENTA}{security_group_id}{prism.ui.RESET}"  # noqa: E501
+                prism.prism_logging.DEFAULT_LOGGER.agent(  # type: ignore
+                    f"{log_prefix} | Using existing security group {log_security_group_id}"  # noqa: E501
+                )
+
+            # Log instance ID template
+            log_instance_id_template = f"{prism.ui.MAGENTA}{{instance_id}}{prism.ui.RESET}"  # noqa: E501
 
-        # If the instance exists and is running, then just return
-        elif len(resp.keys()) > 0 and resp["state"] in [State.PENDING, State.RUNNING]:
-            while resp["state"] == State.PENDING:
+            # Instance
+            if resources["instance"] is None:
+                instance = ec2_resource.create_instances(
+                    InstanceType=instance_type,
+                    KeyName=instance_name,
+                    MinCount=1,
+                    MaxCount=1,
+                    ImageId="ami-0889a44b331db0194",
+                    TagSpecifications=[
+                        {
+                            'ResourceType': 'instance',
+                            'Tags': [
+                                {
+                                    'Key': 'Name',
+                                    'Value': instance_name
+                                },
+                            ]
+                        },
+                    ],
+                    SecurityGroupIds=[
+                        security_group_id
+                    ]
+                )
+                instance_id = instance[0].id
 
                 # Log
-                log_pending_status = f"{prism.ui.YELLOW}pending{prism.ui.RESET}"
                 prism.prism_logging.DEFAULT_LOGGER.agent(  # type: ignore
-                    f"{log_prefix} | Instance {log_instance_id_template.format(instance_id=instance_id)} is `{log_pending_status}`... checking again in 5 seconds"  # noqa: E501
+                    f"{log_prefix} | Created EC2 instance with ID {log_instance_id_template.format(instance_id=instance_id)}"  # noqa: E501
                 )
-                resp = self.check_instance_data(
-                    ec2_client,
-                    instance_id
+                time.sleep(1)
+            else:
+                if not Path(prism.constants.INTERNAL_FOLDER / 'ec2.json').is_file():
+                    raise _create_exception("instance")
+                instance_id = self.instance_id
+
+                # Log
+                prism.prism_logging.DEFAULT_LOGGER.agent(  # type: ignore
+                    f"{log_prefix} | Using existing EC2 instance with ID {log_instance_id_template.format(instance_id=instance_id)}"  # noqa: E501
                 )
-                time.sleep(5)
 
-        # If the state exiss but has stopped, then restart it
-        elif len(resp.keys()) > 0 and resp["state"] in [State.STOPPED, State.STOPPING]:
-            self.restart_instance(
-                ec2_client,
-                resp["state"],
-                resp["instance_id"]
-            )
+            # Instance data
+            resp = self.check_instance_data(ec2_client, instance_id)
 
-        # Write data
-        data = {
-            "resources": {
-                "instance_id": instance_id,
-                "public_dns_name": resp["public_dns_name"],
-                "security_group_id": security_group_id,
-                "key_name": instance_name,
-                "state": resp["state"]
-            },
-            "files": {
-                "pem_key_path": str(pem_key_path)
-            }
-        }
-        self.write_json(data)
+            # If the instance exists but its key-name is not `instance_name` (this
+            # really should never happen unless the user manually creates an EC2
+            # instance that has the same name), then raise an error
+            if len(resp.keys()) > 0 and resp["key_name"] != instance_name:
+                raise prism.exceptions.AwsException(
+                    f"unrecognized key `{resp['key_name']}`...the agent requires key `{instance_name}.pem`"  # noqa: E501
+                )
+
+            # If the instance exists and is running, then just return
+            elif len(resp.keys()) > 0 and resp["state"] in [State.PENDING, State.RUNNING]:  # noqa: E501
+                while resp["state"] == State.PENDING:
+
+                    # Log
+                    log_pending_status = f"{prism.ui.YELLOW}pending{prism.ui.RESET}"
+                    prism.prism_logging.DEFAULT_LOGGER.agent(  # type: ignore
+                        f"{log_prefix} | Instance {log_instance_id_template.format(instance_id=instance_id)} is `{log_pending_status}`... checking again in 5 seconds"  # noqa: E501
+                    )
+                    resp = self.check_instance_data(
+                        ec2_client,
+                        instance_id
+                    )
+                    time.sleep(5)
+
+            # If the state exiss but has stopped, then restart it
+            elif len(resp.keys()) > 0 and resp["state"] in [State.STOPPED, State.STOPPING]:  # noqa: E501
+                self.restart_instance(
+                    ec2_client,
+                    resp["state"],
+                    resp["instance_id"]
+                )
 
-        # Update class attributes
-        self.instance_id = instance_id
-        self.public_dns_name = resp["public_dns_name"]
-        self.security_group_id = security_group_id
-        self.key_name = instance_name
-        self.state = resp["state"]
-        self.pem_key_path = pem_key_path
+            # Write data
+            data = {
+                "resources": {
+                    "instance_id": instance_id,  # type: ignore
+                    "public_dns_name": resp["public_dns_name"],
+                    "state": resp["state"]
+                },
+            }
+            data = self.update_json(data)
 
-        # Return the data
-        return data
+            # Update class attributes
+            self.instance_id = instance_id
+            self.public_dns_name = resp["public_dns_name"]
+            self.security_group_id = security_group_id
+            self.key_name = instance_name
+            self.state = resp["state"]
+            self.pem_key_path = pem_key_path
+
+            # Return the data
+            return data
+
+        # If an error occurs, delete whatever resources may have been created
+        except Exception as e:
+            deleted_resources = self.delete_resources_in_json()
+
+            # Log the deleted resources
+            log_prefix = f"{prism.ui.AGENT_EVENT}{self.instance_name}{prism.ui.RED}[delete]{prism.ui.RESET}"  # noqa: E501
+            for rs_name, rs_id in deleted_resources.items():
+                prism.prism_logging.DEFAULT_LOGGER.agent(  # type: ignore
+                    f"{log_prefix} | Deleting {rs_name} `{rs_id}`"
+                )
+            raise e
 
     def parse_profile_paths(self,
         project: PrismProject
     ):
         """
         Certain profiles require the user to point to specific files or directories. If
         these profiles exist in the user's project, then we need to parse those paths
@@ -896,42 +1009,55 @@
             self.instance_id,
             self.instance_name,
             instance_type
         )
 
         # The `create_instance` command is blocking — it won't finish until the instance
         # is up and running.
-        user = "ec2-user"
-        public_dns_name = data["resources"]["public_dns_name"]
-        pem_key_path = data["files"]["pem_key_path"]
-
-        # Build the shell command
-        cmd = [
-            '/bin/sh', self.AGENT_APPLY_SCRIPT,
-            '-r', str(requirements_txt_path),
-            '-p', str(pem_key_path),
-            '-u', user,
-            '-n', public_dns_name,
-            '-d', str(self.project.project_dir),
-            '-c', project_paths_cli,
-            '-e', env_cli,
-        ]
-
-        # Open a subprocess and stream the logs
-        _, err, returncode = self.stream_logs(cmd, prism.ui.AGENT_WHICH_BUILD, "build")
+        try:
+            user = "ec2-user"
+            public_dns_name = data["resources"]["public_dns_name"]
+            pem_key_path = data["files"]["pem_key_path"]
+
+            # Build the shell command
+            cmd = [
+                '/bin/sh', self.AGENT_APPLY_SCRIPT,
+                '-r', str(requirements_txt_path),
+                '-p', str(pem_key_path),
+                '-u', user,
+                '-n', public_dns_name,
+                '-d', str(self.project.project_dir),
+                '-c', project_paths_cli,
+                '-e', env_cli,
+            ]
 
-        # Log anything from stderr that was printed in the project
-        for line in err.readlines():
-            prism.prism_logging.DEFAULT_LOGGER.agent(  # type: ignore
-                f"{prism.ui.AGENT_EVENT}{self.instance_name}{prism.ui.AGENT_WHICH_BUILD}[build]{prism.ui.RESET} | {line.rstrip()}"  # noqa: E501
+            # Open a subprocess and stream the logs
+            _, err, returncode = self.stream_logs(
+                cmd, prism.ui.AGENT_WHICH_BUILD, "build"
             )
 
-        # Return the returncode. Return a dictionary in order to avoid confusing this
-        # output with the output of an event manager.
-        return {"return_code": returncode}
+            # Log anything from stderr that was printed in the project
+            for line in err.readlines():
+                prism.prism_logging.DEFAULT_LOGGER.agent(  # type: ignore
+                    f"{prism.ui.AGENT_EVENT}{self.instance_name}{prism.ui.AGENT_WHICH_BUILD}[build]{prism.ui.RESET} | {line.rstrip()}"  # noqa: E501
+                )
+
+            # If the return code is non-zero, then an error occurred. Delete all of the
+            # resources so that the user can try again.
+            if returncode != 0:
+                self.delete()
+
+            # Return the returncode. Return a dictionary in order to avoid confusing
+            # this output with the output of an event manager.
+            return {"return_code": returncode}
+
+        # If we encounter any sort of error, delete the resources first and then raise
+        except Exception as e:
+            self.delete()
+            raise e
 
     def run(self):
         """
         Run the project using the EC2 agent
         """
         # Full command
         full_cmd = self.construct_command()
```

### Comparing `prism-ds-0.2.0rc2/prism/agents/meta.py` & `prism-ds-0.2.1/prism/agents/meta.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/agents/scripts/apply.sh` & `prism-ds-0.2.1/prism/agents/scripts/apply.sh`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/agents/scripts/run.sh` & `prism-ds-0.2.1/prism/agents/scripts/run.sh`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/cli/agent.py` & `prism-ds-0.2.1/prism/cli/agent.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/cli/base.py` & `prism-ds-0.2.1/prism/cli/base.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/cli/compile.py` & `prism-ds-0.2.1/prism/cli/compile.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/cli/connect.py` & `prism-ds-0.2.1/prism/cli/connect.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/cli/create_agent.py` & `prism-ds-0.2.1/prism/cli/create_agent.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/cli/create_task.py` & `prism-ds-0.2.1/prism/cli/create_task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/cli/create_trigger.py` & `prism-ds-0.2.1/prism/cli/create_trigger.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/cli/graph.py` & `prism-ds-0.2.1/prism/cli/graph.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/cli/init.py` & `prism-ds-0.2.1/prism/cli/init.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/cli/run.py` & `prism-ds-0.2.1/prism/cli/run.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/cli/spark_submit.py` & `prism-ds-0.2.1/prism/cli/spark_submit.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/client/__init__.py` & `prism-ds-0.2.1/prism/client/__init__.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/constants.py` & `prism-ds-0.2.1/prism/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 #############
 # Constants #
 #############
 
 # Version number
-VERSION = '0.2.0rc2'
+VERSION = '0.2.1'
 
 # Root directory of project
 ROOT_DIR = str(Path(os.path.dirname(__file__)).parent)
 
 # Files to ignore when instantiating Prism project
 IGNORE_FILES = ["__pycache__", '*checkpoint.ipynb', '.ipynb_checkpoints']
```

### Comparing `prism-ds-0.2.0rc2/prism/decorators/target.py` & `prism-ds-0.2.1/prism/decorators/target.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/decorators/task.py` & `prism-ds-0.2.1/prism/decorators/task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/docs/build/311ea03002abadcdcaba.png` & `prism-ds-0.2.1/prism/docs/build/311ea03002abadcdcaba.png`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/docs/build/54968a39190c43d592b9.svg` & `prism-ds-0.2.1/prism/docs/build/54968a39190c43d592b9.svg`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/docs/build/737ad70b3f2d3a9b5f6e.ico` & `prism-ds-0.2.1/prism/docs/build/737ad70b3f2d3a9b5f6e.ico`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/docs/build/ce188596011a8fa32931.png` & `prism-ds-0.2.1/prism/docs/build/ce188596011a8fa32931.png`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/docs/build/index.html` & `prism-ds-0.2.1/prism/docs/build/index.html`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/docs/build/main.js.LICENSE.txt` & `prism-ds-0.2.1/prism/docs/build/main.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/event_managers/base.py` & `prism-ds-0.2.1/prism/event_managers/base.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/exceptions.py` & `prism-ds-0.2.1/prism/exceptions.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/infra/compiled_task.py` & `prism-ds-0.2.1/prism/infra/compiled_task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/infra/compiler.py` & `prism-ds-0.2.1/prism/infra/compiler.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/infra/executor.py` & `prism-ds-0.2.1/prism/infra/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     ) -> base_event_manager.EventManagerOutput:
         """
         Callback used to get results of task execution in Pool
         """
         # Keep track of current module in tasks manager
         if isinstance(task_manager, PrismTaskManager):
             task_manager.curr_module = re.sub(
-                r'\.py$', '', task.task_relative_path.name
+                r'\.py$', '', str(task.task_relative_path)
             )
 
         # Keep track of events
         event_list: List[Event] = []
         if task_manager == 0:
             return base_event_manager.EventManagerOutput(0, None, event_list)
         task_name = task.task_var_name
```

### Comparing `prism-ds-0.2.0rc2/prism/infra/hooks.py` & `prism-ds-0.2.1/prism/infra/hooks.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/infra/manifest.py` & `prism-ds-0.2.1/prism/infra/manifest.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/infra/pipeline.py` & `prism-ds-0.2.1/prism/infra/pipeline.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/infra/project.py` & `prism-ds-0.2.1/prism/infra/project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/infra/sys_path.py` & `prism-ds-0.2.1/prism/infra/sys_path.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/infra/task_manager.py` & `prism-ds-0.2.1/prism/infra/task_manager.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/main.py` & `prism-ds-0.2.1/prism/main.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/mixins/agent.py` & `prism-ds-0.2.1/prism/mixins/agent.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/mixins/aws.py` & `prism-ds-0.2.1/prism/mixins/aws.py`

 * *Files 10% similar despite different names*

```diff
@@ -71,16 +71,27 @@
         response = ec2_client.create_key_pair(
             KeyName=key_name,
             KeyType="rsa",
             KeyFormat="pem"
         )
         if not Path(directory).is_dir():
             Path(directory).mkdir(parents=True)
-        with open(Path(directory / f"{key_name}.pem"), 'w') as f:
-            f.write(response["KeyMaterial"])
+
+        # Write the key to a local file
+        try:
+            with open(Path(directory / f"{key_name}.pem"), 'w') as f:
+                f.write(response["KeyMaterial"])
+
+        # If the path already exists and cannot be edited, then raise the exception. But
+        # first, delete the newly created key pair.
+        except Exception as e:
+            ec2_client.delete_key_pair(
+                KeyName=key_name
+            )
+            raise e
 
         # Change the permissions
         os.chmod(Path(directory / f"{key_name}.pem"), stat.S_IREAD)
 
         # We'll need to persist the location of the PEM key across runs. For example,
         # let's say a user calls `agent apply` and creates the key-pair and EC2
         # instance. When they call `agent run`, we will need to use the PEM key created
```

### Comparing `prism-ds-0.2.0rc2/prism/mixins/base.py` & `prism-ds-0.2.1/prism/mixins/base.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/mixins/compile.py` & `prism-ds-0.2.1/prism/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/mixins/connect.py` & `prism-ds-0.2.1/prism/mixins/connect.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/mixins/create_agent.py` & `prism-ds-0.2.1/prism/mixins/create_agent.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/mixins/create_task.py` & `prism-ds-0.2.1/prism/mixins/create_task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/mixins/create_trigger.py` & `prism-ds-0.2.1/prism/mixins/create_trigger.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/mixins/graph.py` & `prism-ds-0.2.1/prism/mixins/graph.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/mixins/run.py` & `prism-ds-0.2.1/prism/mixins/run.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/mixins/sys_handler.py` & `prism-ds-0.2.1/prism/mixins/sys_handler.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/parsers/ast_parser.py` & `prism-ds-0.2.1/prism/parsers/ast_parser.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/parsers/base.py` & `prism-ds-0.2.1/prism/parsers/base.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/parsers/yml_parser.py` & `prism-ds-0.2.1/prism/parsers/yml_parser.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/prism_logging.py` & `prism-ds-0.2.1/prism/prism_logging.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/profiles/adapter.py` & `prism-ds-0.2.1/prism/profiles/adapter.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/profiles/bigquery.py` & `prism-ds-0.2.1/prism/profiles/bigquery.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/profiles/dbt.py` & `prism-ds-0.2.1/prism/profiles/dbt.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/profiles/meta.py` & `prism-ds-0.2.1/prism/profiles/meta.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/profiles/postgres.py` & `prism-ds-0.2.1/prism/profiles/postgres.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/profiles/profile.py` & `prism-ds-0.2.1/prism/profiles/profile.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/profiles/pyspark.py` & `prism-ds-0.2.1/prism/profiles/pyspark.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/profiles/redshift.py` & `prism-ds-0.2.1/prism/profiles/redshift.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/profiles/snowflake.py` & `prism-ds-0.2.1/prism/profiles/snowflake.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/profiles/trino.py` & `prism-ds-0.2.1/prism/profiles/trino.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/spark/wrapper.py` & `prism-ds-0.2.1/prism/spark/wrapper.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/target.py` & `prism-ds-0.2.1/prism/target.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/task.py` & `prism-ds-0.2.1/prism/task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/templates/minimal_project/prism_project.py` & `prism-ds-0.2.1/prism/templates/minimal_project/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/templates/minimal_project/tasks/class_task.py` & `prism-ds-0.2.1/prism/templates/minimal_project/tasks/class_task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/templates/minimal_project/tasks/decorated_task.py` & `prism-ds-0.2.1/prism/templates/minimal_project/tasks/decorated_task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/templates/starter_project/dev/dev.ipynb` & `prism-ds-0.2.1/prism/templates/starter_project/dev/dev.ipynb`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/templates/starter_project/prism_project.py` & `prism-ds-0.2.1/prism/templates/starter_project/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/templates/starter_project/tasks/class_task.py` & `prism-ds-0.2.1/prism/templates/starter_project/tasks/class_task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/templates/starter_project/tasks/decorated_task.py` & `prism-ds-0.2.1/prism/templates/starter_project/tasks/decorated_task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/integration_test_class.py` & `prism-ds-0.2.1/prism/tests/integration/integration_test_class.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_client.py` & `prism-ds-0.2.1/prism/tests/integration/test_client.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_compile.py` & `prism-ds-0.2.1/prism/tests/integration/test_compile.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_connect.py` & `prism-ds-0.2.1/prism/tests/integration/test_connect.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_create.py` & `prism-ds-0.2.1/prism/tests/integration/test_create.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_dbt.py` & `prism-ds-0.2.1/prism/tests/integration/test_dbt.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_hooks.py` & `prism-ds-0.2.1/prism/tests/integration/test_hooks.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_init.py` & `prism-ds-0.2.1/prism/tests/integration/test_init.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001_init/prism_project.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/001_init/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001_init/tasks/class_task.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/001_init/tasks/class_task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001_init/tasks/decorated_task.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/001_init/tasks/decorated_task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001a_init_minimal/prism_project.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/001a_init_minimal/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001a_init_minimal/tasks/class_task.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/001a_init_minimal/tasks/class_task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001a_init_minimal/tasks/decorated_task.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/001a_init_minimal/tasks/decorated_task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/002_no_project_py/functions.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/002_no_project_py/functions.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/002_no_project_py/modules/module01.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/002_no_project_py/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/002_no_project_py/modules/module02.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/002_no_project_py/modules/module02.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/002_no_project_py/modules/module03.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/002_no_project_py/modules/module03.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/003_project_with_cycle/modules/module01.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/003_project_with_cycle/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/003_project_with_cycle/modules/module02.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/003_project_with_cycle/modules/module02.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/003_project_with_cycle/modules/module03.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/003_project_with_cycle/modules/module03.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/003_project_with_cycle/prism_project.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/003_project_with_cycle/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/004_simple_project/modules/module01.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/004_simple_project/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/004_simple_project/modules/module02.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/004_simple_project/modules/module02.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/004_simple_project/modules/module03.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/004_simple_project/modules/module03.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/004_simple_project/prism_project.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/004_simple_project/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/functions.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_modules/functions.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module01.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module02.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module02.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module03.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module03.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module04.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module04.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/prism_project.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_modules/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/functions.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/functions.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/prism_project.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module01.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module02.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module02.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module03.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module03.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module04.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module04.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module01.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module02.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module02.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module03.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module03.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module04.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module04.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/prism_project.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/006_simple_project_with_profile/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/007_spark_project/prism_project.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/007_spark_project/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/007_spark_project/tasks/module01.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/007_spark_project/tasks/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/007_spark_project/tasks/module02.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/007_spark_project/tasks/module02.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/007_spark_project/tasks/module03.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/007_spark_project/tasks/module03.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/007_spark_project/tasks/module04.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/007_spark_project/tasks/module04.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/008_targets/prism_project.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/008_targets/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/008_targets/tasks/csv.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/008_targets/tasks/csv.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/008_targets/tasks/csv_iter.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/008_targets/tasks/csv_iter.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/008_targets/tasks/csv_mult.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/008_targets/tasks/csv_mult.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/008_targets/tasks/parquet.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/008_targets/tasks/parquet.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/prism_project.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/tasks/bad_adapter.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/tasks/bad_adapter.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/tasks/filter_customers.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/tasks/filter_customers.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module01.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module02.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module02.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/module03.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/module03.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/module04.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/module04.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/prism_project.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module01.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module02.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module02.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/module03.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/module03.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/011_bad_task_ref/modules/module04.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/module04.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/011_bad_task_ref/prism_project.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/011_bad_task_ref/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency/modules/module01.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency/modules/module02.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency/modules/module02.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency/modules/module03.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency/modules/module03.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency/modules/module04.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency/modules/module04.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency/prism_project.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency_local/prism_project.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency_local/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency_local/tasks/local_tasks.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency_local/tasks/local_tasks.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency_local/tasks/non_local_task.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency_local/tasks/non_local_task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/bad_adapter.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/bad_adapter.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/postgres.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/postgres.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/snowflake.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/snowflake.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/spark.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/spark.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/prism_project.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/013_hooks_sql_spark/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/014_test_triggers_normal/prism_project.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/014_test_triggers_normal/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/015_test_triggers_no_dir/prism_project.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/015_test_triggers_no_dir/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/016_test_triggers_error/prism_project.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/016_test_triggers_error/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/016_test_triggers_error/tasks/module01.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/016_test_triggers_error/tasks/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/017_test_triggers_extra_key/prism_project.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/017_test_triggers_extra_key/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/017_test_triggers_extra_key/tasks/module01.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/017_test_triggers_extra_key/tasks/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/018_test_triggers_no_include/prism_project.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/018_test_triggers_no_include/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/018_test_triggers_no_include/tasks/module01.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/018_test_triggers_no_include/tasks/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/019_dec_targets/prism_project.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/019_dec_targets/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/019_dec_targets/tasks/extract.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/019_dec_targets/tasks/extract.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/019_dec_targets/tasks/load.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/019_dec_targets/tasks/load.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/020_dec_retries/prism_project.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/020_dec_retries/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/020_dec_retries/tasks/load.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/020_dec_retries/tasks/load.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/021_project_with_local_tasks/prism_project.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/021_project_with_local_tasks/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/021_project_with_local_tasks/tasks/extract.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/021_project_with_local_tasks/tasks/extract.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,8 +29,9 @@
         )
     ]
 )
 def extract(tasks, hooks):
     api_url = "https://restcountries.com/v3.1/all"
     resp = requests.get(api_url, verify=False)
     data = json.loads(resp.text)
+    data = sorted(data, key=lambda x: x["name"]["common"])
     return data
```

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/021_project_with_local_tasks/tasks/transform_load.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/021_project_with_local_tasks/tasks/transform_load.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     independent_countries = []
     for c in data:
         try:
             if c["independent"]:
                 independent_countries.append(c)
         except KeyError:
             continue
-    return independent_countries
+    return sorted(independent_countries, key=lambda x: x["name"]["common"])
 
 
 @task(
     targets=[
         target(
             type=prism.target.JSON,
             loc=Path(prism_project.OUTPUT / 'independent_countries.json')
```

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/prism_project.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/tasks/transform_load.py` & `prism-ds-0.2.1/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/tasks/transform_load.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_run.py` & `prism-ds-0.2.1/prism/tests/integration/test_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -1335,16 +1335,16 @@
         # Check output
         self.assertTrue(Path(wkdir / 'output' / 'all_countries.json').is_file())
         self.assertTrue(Path(wkdir / 'output' / 'independent_countries.json').is_file())
         with open(Path(wkdir / 'output' / 'all_countries.json'), 'r') as f:
             all_countries = json.loads(f.read())
         with open(Path(wkdir / 'output' / 'independent_countries.json'), 'r') as f:
             independent_countries = json.loads(f.read())
-        self.assertEqual(all_countries[-1]["name"]["common"], "Guinea-Bissau")
-        self.assertEqual(independent_countries[0]["name"]["common"], "Jordan")
+        self.assertEqual(all_countries[-1]["name"]["common"], "Åland Islands")
+        self.assertEqual(independent_countries[0]["name"]["common"], "Afghanistan")
 
         # Remove the .compiled directory, if it exists
         self._remove_compiled_dir(wkdir)
 
         # Remove all files in the output directory
         self._remove_files_in_output(wkdir)
 
@@ -1394,15 +1394,15 @@
         # Check output
         self.assertTrue(Path(wkdir / 'output' / 'all_countries.json').is_file())
         self.assertFalse(
             Path(wkdir / 'output' / 'independent_countries.json').is_file()
         )
         with open(Path(wkdir / 'output' / 'all_countries.json'), 'r') as f:
             all_countries = json.loads(f.read())
-        self.assertEqual(all_countries[-1]["name"]["common"], "Guinea-Bissau")
+        self.assertEqual(all_countries[-1]["name"]["common"], "Åland Islands")
 
         # ------------------------------------------
         # Now, execute transform_load
 
         # Update logger streamer
         new_streamer = StringIO()
         string_stream_handler.setStream(new_streamer)
@@ -1423,15 +1423,15 @@
             _run_task_end_events('TaskSuccessfulEndEvent')
         self.assertEqual(' | '.join(expected_events), run_results)
 
         # Check output
         self.assertTrue(Path(wkdir / 'output' / 'independent_countries.json').is_file())
         with open(Path(wkdir / 'output' / 'independent_countries.json'), 'r') as f:
             independent_countries = json.loads(f.read())
-        self.assertEqual(independent_countries[0]["name"]["common"], "Jordan")
+        self.assertEqual(independent_countries[0]["name"]["common"], "Afghanistan")
 
         # Remove the .compiled directory, if it exists
         self._remove_compiled_dir(wkdir)
 
         # Remove all files in the output directory
         self._remove_files_in_output(wkdir)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_spark_submit.py` & `prism-ds-0.2.1/prism/tests/integration/test_spark_submit.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/integration/test_targets.py` & `prism-ds-0.2.1/prism/tests/integration/test_targets.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/unit/test_adapter_profile.py` & `prism-ds-0.2.1/prism/tests/unit/test_adapter_profile.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/unit/test_agent/prism_project.py` & `prism-ds-0.2.1/prism/tests/unit/test_agent/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/unit/test_agents.py` & `prism-ds-0.2.1/prism/tests/unit/test_agents.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/unit/test_all_dag_fns.py` & `prism-ds-0.2.1/prism/tests/unit/test_all_dag_fns.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/unit/test_ast_parser.py` & `prism-ds-0.2.1/prism/tests/unit/test_ast_parser.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/unit/test_jinja.py` & `prism-ds-0.2.1/prism/tests/unit/test_jinja.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/unit/test_prism_project_py/bad_trigger_key.py` & `prism-ds-0.2.1/prism/tests/unit/test_prism_project_py/bad_trigger_key.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/unit/test_prism_project_py/multiple_profiles.py` & `prism-ds-0.2.1/prism/tests/unit/test_prism_project_py/multiple_profiles.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/unit/test_prism_project_py/no_profile.py` & `prism-ds-0.2.1/prism/tests/unit/test_prism_project_py/no_profile.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/unit/test_prism_project_py/non_null_profile.py` & `prism-ds-0.2.1/prism/tests/unit/test_prism_project_py/non_null_profile.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/unit/test_prism_project_py/null_profile.py` & `prism-ds-0.2.1/prism/tests/unit/test_prism_project_py/null_profile.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/unit/test_prism_project_py/on_failure_triggers_only.py` & `prism-ds-0.2.1/prism/tests/unit/test_prism_project_py/on_failure_triggers_only.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/unit/test_prism_project_py/on_success_triggers_only.py` & `prism-ds-0.2.1/prism/tests/unit/test_prism_project_py/on_success_triggers_only.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/unit/test_prism_project_py/triggers_normal.py` & `prism-ds-0.2.1/prism/tests/unit/test_prism_project_py/triggers_normal.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/unit/test_project.py` & `prism-ds-0.2.1/prism/tests/unit/test_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/unit/test_trigger.py` & `prism-ds-0.2.1/prism/tests/unit/test_trigger.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/tests/unit/test_trigger_yml/prism_project.py` & `prism-ds-0.2.1/prism/tests/unit/test_trigger_yml/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/triggers/__init__.py` & `prism-ds-0.2.1/prism/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism/ui.py` & `prism-ds-0.2.1/prism/ui.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism_ds.egg-info/PKG-INFO` & `prism-ds-0.2.1/prism_ds.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prism-ds
-Version: 0.2.0rc2
+Version: 0.2.1
 Summary: The easiest way to create data pipelines in Python.
 Author: prism founders
 Author-email: hello@runprism.com
 License: Apache-2.0
 Project-URL: homepage, https://www.runprism.com
 Project-URL: documentation, https://docs.runprism.com
 Project-URL: repository, https://github.com/runprism/prism
@@ -27,15 +27,15 @@
 Provides-Extra: pyspark
 Provides-Extra: dbt
 Provides-Extra: docker
 Provides-Extra: testing
 License-File: LICENSE
 
 <p align="center">
-  <img src="https://github.com/runprism/prism/raw/main/.github/prism_logo_light.png" alt="prism logo" width="350"/>
+  <img src="https://github.com/runprism/prism/raw/main/.github/Logo.png" alt="prism logo" height="100"/>
 </p>
 <p align="center">
     <a href="https://pypi.python.org/pypi/prism-ds/" alt="PyPI version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/prism-ds?color=2081c1&labelColor=090422"></a>
     <a href="https://pepy.tech/badge/prism-ds/" alt="Downloads">
         <img src="https://static.pepy.tech/personalized-badge/prism-ds?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads"/>
     </a>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: prism-ds Version: 0.2.0rc2 Summary: The easiest way
-to create data pipelines in Python. Author: prism founders Author-email:
+Metadata-Version: 2.1 Name: prism-ds Version: 0.2.1 Summary: The easiest way to
+create data pipelines in Python. Author: prism founders Author-email:
 hello@runprism.com License: Apache-2.0 Project-URL: homepage, https://
 www.runprism.com Project-URL: documentation, https://docs.runprism.com Project-
 URL: repository, https://github.com/runprism/prism Platform: unix Platform:
 linux Platform: osx Platform: win32 Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Requires-Python: >=3.7
```

### Comparing `prism-ds-0.2.0rc2/prism_ds.egg-info/SOURCES.txt` & `prism-ds-0.2.1/prism_ds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/prism_ds.egg-info/requires.txt` & `prism-ds-0.2.1/prism_ds.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 [bigquery]
 google-api-python-client>=2
 google-auth>=2
 google-cloud-bigquery>=2
 db-dtypes>=1
 
 [dbt]
-dbt-core>=1
+dbt-core<1.6.0,>=1
 
 [docker]
 docker>=6.0
 
 [postgres]
 psycopg2-binary>=2.9
 
@@ -35,14 +35,14 @@
 psycopg2-binary>=2.9
 
 [snowflake]
 snowflake-connector-python>=2
 pyarrow<10.1.0,>=10.0.1
 
 [testing]
-dbt-snowflake>=1
+dbt-snowflake<1.6.0,>=1
 pytest>=7
 fastparquet<1,>=0.8
 tox>=3.24
 
 [trino]
 trino>=0.319
```

### Comparing `prism-ds-0.2.0rc2/pyproject.toml` & `prism-ds-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc2/setup.cfg` & `prism-ds-0.2.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [metadata]
 name = prism-ds
 description = The easiest way to create data pipelines in Python.
 long_description_content_type = text/markdown
 long_description = file: README.md
-version = 0.2.0rc2
+version = 0.2.1
 author = prism founders
 author_email = hello@runprism.com
 license = Apache-2.0
-license_file = LICENSE
+license_files = LICENSE
 platforms = unix, linux, osx, win32
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
@@ -55,19 +55,19 @@
 postgres = 
 	psycopg2-binary>=2.9
 trino = 
 	trino>=0.319
 pyspark = 
 	pyspark>=3
 dbt = 
-	dbt-core>=1
+	dbt-core>=1,<1.6.0
 docker = 
 	docker>=6.0
 testing = 
-	dbt-snowflake>=1
+	dbt-snowflake>=1,<1.6.0
 	pytest>=7
 	fastparquet>=0.8,<1
 	tox>=3.24
 
 [options.entry_points]
 console_scripts = 
 	prism = prism.main:invoke
```

