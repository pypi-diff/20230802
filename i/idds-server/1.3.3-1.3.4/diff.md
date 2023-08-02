# Comparing `tmp/idds-server-1.3.3.tar.gz` & `tmp/idds-server-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idds-server-1.3.3.tar", last modified: Fri Jul 21 07:10:55 2023, max compression
+gzip compressed data, was "idds-server-1.3.4.tar", last modified: Wed Aug  2 09:00:08 2023, max compression
```

## Comparing `idds-server-1.3.3.tar` & `idds-server-1.3.4.tar`

### file list

```diff
@@ -1,274 +1,275 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.836870 idds-server-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-21 07:10:42.000000 idds-server-1.3.3/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-21 07:10:55.836870 idds-server-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-21 07:10:42.000000 idds-server-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.816870 idds-server-1.3.3/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1687 2023-07-21 07:10:42.000000 idds-server-1.3.3/bin/idds-daemon
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-21 07:10:55.000000 idds-server-1.3.3/bin/idds.wsgi
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-21 07:10:42.000000 idds-server-1.3.3/bin/idds.wsgi.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      584 2023-07-21 07:10:42.000000 idds-server-1.3.3/bin/run-idds
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-21 07:10:42.000000 idds-server-1.3.3/bin/run-idds-fake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.820870 idds-server-1.3.3/config_default/
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-21 07:10:42.000000 idds-server-1.3.3/config_default/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-21 07:10:42.000000 idds-server-1.3.3/config_default/auth.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-21 07:10:42.000000 idds-server-1.3.3/config_default/gacl
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-07-21 07:10:42.000000 idds-server-1.3.3/config_default/httpd-idds-443-py39-cc7.conf
--rwxr-xr-x   0 runner    (1001) docker     (123)     3679 2023-07-21 07:10:42.000000 idds-server-1.3.3/config_default/idds.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      125 2023-07-21 07:10:42.000000 idds-server-1.3.3/config_default/logrotate_daemon
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-21 07:10:42.000000 idds-server-1.3.3/config_default/logrotate_idds
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-21 07:10:42.000000 idds-server-1.3.3/config_default/panda.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-21 07:10:42.000000 idds-server-1.3.3/config_default/rucio.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-21 07:10:42.000000 idds-server-1.3.3/config_default/supervisord_httpd.ini
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-21 07:10:42.000000 idds-server-1.3.3/config_default/supervisord_idds.ini
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-21 07:10:42.000000 idds-server-1.3.3/config_default/supervisord_iddsfake.ini
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-21 07:10:42.000000 idds-server-1.3.3/config_default/supervisord_logrotate.ini
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-21 07:10:42.000000 idds-server-1.3.3/config_default/supervisord_syslog-ng.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.816870 idds-server-1.3.3/etc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.820870 idds-server-1.3.3/etc/idds/
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-21 07:10:42.000000 idds-server-1.3.3/etc/idds/alembic.ini.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.820870 idds-server-1.3.3/etc/idds/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-21 07:10:42.000000 idds-server-1.3.3/etc/idds/auth/auth.cfg.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.816870 idds-server-1.3.3/etc/idds/condor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.820870 idds-server-1.3.3/etc/idds/condor/client/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-21 07:10:42.000000 idds-server-1.3.3/etc/idds/condor/client/00personal_condor.config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.820870 idds-server-1.3.3/etc/idds/condor/server/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-21 07:10:42.000000 idds-server-1.3.3/etc/idds/condor/server/00personal_condor.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      811 2023-07-21 07:10:42.000000 idds-server-1.3.3/etc/idds/idds.cfg.client.template
--rwxr-xr-x   0 runner    (1001) docker     (123)     3946 2023-07-21 07:10:42.000000 idds-server-1.3.3/etc/idds/idds.cfg.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.820870 idds-server-1.3.3/etc/idds/rest/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-21 07:10:42.000000 idds-server-1.3.3/etc/idds/rest/gacl.template
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-07-21 07:10:42.000000 idds-server-1.3.3/etc/idds/rest/httpd-idds-443-py36-cc7.conf.template
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-21 07:10:42.000000 idds-server-1.3.3/etc/idds/rest/httpd-idds-443-py36-cc7_normal.conf.template
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-07-21 07:10:55.000000 idds-server-1.3.3/etc/idds/rest/httpd-idds-443-py39-cc7.conf.install_template
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-21 07:10:42.000000 idds-server-1.3.3/etc/idds/rest/httpd-idds-443-py39-cc7.conf.template
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-21 07:10:42.000000 idds-server-1.3.3/etc/idds/rest/ssl.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.820870 idds-server-1.3.3/etc/idds/supervisord.d/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-21 07:10:42.000000 idds-server-1.3.3/etc/idds/supervisord.d/idds.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.820870 idds-server-1.3.3/etc/idds/website/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-21 07:10:42.000000 idds-server-1.3.3/etc/idds/website/25-port443.conf
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-21 07:10:42.000000 idds-server-1.3.3/etc/idds/website/25-port80.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.820870 idds-server-1.3.3/etc/sql/
--rw-r--r--   0 runner    (1001) docker     (123)    25596 2023-07-21 07:10:42.000000 idds-server-1.3.3/etc/sql/oracle_11.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-21 07:10:42.000000 idds-server-1.3.3/etc/sql/oracle_11_test.sql
--rw-r--r--   0 runner    (1001) docker     (123)    22610 2023-07-21 07:10:42.000000 idds-server-1.3.3/etc/sql/oracle_19.sql
--rw-r--r--   0 runner    (1001) docker     (123)    18371 2023-07-21 07:10:42.000000 idds-server-1.3.3/etc/sql/oracle_update.sql
--rw-r--r--   0 runner    (1001) docker     (123)    18076 2023-07-21 07:10:42.000000 idds-server-1.3.3/etc/sql/postgresql.sql
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-21 07:10:42.000000 idds-server-1.3.3/etc/sql/postgresql_init.sql
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-21 07:10:42.000000 idds-server-1.3.3/etc/sql/postgresql_update.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.816870 idds-server-1.3.3/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.820870 idds-server-1.3.3/lib/idds/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.820870 idds-server-1.3.3/lib/idds/agents/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.820870 idds-server-1.3.3/lib/idds/agents/archive/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/archive/archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/archive/run_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.820870 idds-server-1.3.3/lib/idds/agents/carrier/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/carrier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/carrier/finisher.py
--rw-r--r--   0 runner    (1001) docker     (123)    24651 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/carrier/poller.py
--rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/carrier/receiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/carrier/submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    14560 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/carrier/trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)    94427 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/carrier/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.820870 idds-server-1.3.3/lib/idds/agents/clerk/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/clerk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67320 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/clerk/clerk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.824870 idds-server-1.3.3/lib/idds/agents/common/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/common/baseagent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.824870 idds-server-1.3.3/lib/idds/agents/common/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/common/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/common/cache/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.824870 idds-server-1.3.3/lib/idds/agents/common/eventbus/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/common/eventbus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/common/eventbus/baseeventbusbackend.py
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/common/eventbus/baseeventbusbackendopt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/common/eventbus/dbeventbusbackend.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/common/eventbus/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/common/eventbus/eventbus.py
--rw-r--r--   0 runner    (1001) docker     (123)    22179 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/common/eventbus/msgeventbusbackend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.824870 idds-server-1.3.3/lib/idds/agents/common/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/common/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15412 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/common/plugins/messaging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/common/timerscheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/common/timertask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.824870 idds-server-1.3.3/lib/idds/agents/conductor/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/conductor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12932 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/conductor/conductor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/conductor/consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.824870 idds-server-1.3.3/lib/idds/agents/coordinator/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/coordinator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15040 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/coordinator/coordinator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5468 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.824870 idds-server-1.3.3/lib/idds/agents/marshaller/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/marshaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/marshaller/marshaller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.824870 idds-server-1.3.3/lib/idds/agents/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40926 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/transformer/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.824870 idds-server-1.3.3/lib/idds/agents/transporter/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/transporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22626 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/agents/transporter/transporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.824870 idds-server-1.3.3/lib/idds/api/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/api/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/api/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/api/contents.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/api/processings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/api/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/api/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.824870 idds-server-1.3.3/lib/idds/core/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30689 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/core/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/core/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/core/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/core/health.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/core/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)    19011 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/core/processings.py
--rw-r--r--   0 runner    (1001) docker     (123)    20716 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/core/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/core/throttlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    33651 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/core/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/core/workprogress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.828870 idds-server-1.3.3/lib/idds/orm/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/orm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.828870 idds-server-1.3.3/lib/idds/orm/base/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/orm/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.828870 idds-server-1.3.3/lib/idds/orm/base/alembic/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/orm/base/alembic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/orm/base/alembic/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.828870 idds-server-1.3.3/lib/idds/orm/base/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/orm/base/alembic/versions/0204f391c32d_add_poll_period_in_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/orm/base/alembic/versions/53d0af715dab_add_site_throttler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/orm/base/alembic/versions/5e0aa2aa1fa3_add_fetch_status_in_contents_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/orm/base/alembic/versions/6ca0e5e466eb_update_message_null_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/orm/base/alembic/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/orm/base/alembic/versions/b0ec813021d6_add_sub_map_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/orm/base/alembic/versions/f79663a7e94e_add_external_content_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/orm/base/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)    53545 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/orm/base/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    13193 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/orm/base/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/orm/base/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/orm/base/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16744 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/orm/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/orm/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    41133 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/orm/contents.py
--rw-r--r--   0 runner    (1001) docker     (123)    11642 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/orm/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/orm/health.py
--rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/orm/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)    18139 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/orm/processings.py
--rw-r--r--   0 runner    (1001) docker     (123)    50045 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/orm/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/orm/throttlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    21562 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/orm/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/orm/workprogress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.828870 idds-server-1.3.3/lib/idds/rest/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/rest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.828870 idds-server-1.3.3/lib/idds/rest/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/rest/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/rest/v1/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/rest/v1/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/rest/v1/cacher.py
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/rest/v1/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/rest/v1/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/rest/v1/hyperparameteropt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/rest/v1/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/rest/v1/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)    28102 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/rest/v1/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/rest/v1/ping.py
--rw-r--r--   0 runner    (1001) docker     (123)    21409 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/rest/v1/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/rest/v1/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.836870 idds-server-1.3.3/lib/idds/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/activelearning_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/auth_test_script.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/cacher_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/catalog_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12118 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    22834 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/core_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/core_tests_dep_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/core_tests_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/datacarousel_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/doma_build_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/find_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/fix_content_dep_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/fix_trasnform_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/hyperparameteropt_bayesian_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/hyperparameteropt_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/hyperparameteropt_docker_local_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/hyperparameteropt_docker_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/hyperparameteropt_nevergrad_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/jsonload_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/kill_workflow_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/logs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/match_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/message_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/message_test1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/migrating_requests_v1_to_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/panda_iam_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/panda_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/performance_test_with_cx_oracle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/performance_test_with_sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/relation_map_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/rest_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/retry_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/run_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/scaling_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/set_throttlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/split_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/test_activelearning.py
--rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/test_atlaspandawork.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/test_big_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    34114 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/test_datacarousel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/test_domapanda.py
--rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/test_domapanda_lsst_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/test_domapanda_pandaclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/test_domapanda_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/test_get_dn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/test_get_request_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/test_hyperparameteropt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/test_merge_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/test_migrate_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/test_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/test_request_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/test_running_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/test_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/test_transform_collection_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/test_transform_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    28166 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/test_workflow_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)    69660 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/test_workflow_condition_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-21 07:10:42.000000 idds-server-1.3.3/lib/idds/tests/trigger_release.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-21 07:10:52.000000 idds-server-1.3.3/lib/idds/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.836870 idds-server-1.3.3/lib/idds_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-21 07:10:55.000000 idds-server-1.3.3/lib/idds_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-07-21 07:10:55.000000 idds-server-1.3.3/lib/idds_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 07:10:55.000000 idds-server-1.3.3/lib/idds_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-21 07:10:55.000000 idds-server-1.3.3/lib/idds_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-21 07:10:55.000000 idds-server-1.3.3/lib/idds_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-21 07:10:55.836870 idds-server-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-07-21 07:10:42.000000 idds-server-1.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.816870 idds-server-1.3.3/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:55.836870 idds-server-1.3.3/tools/env/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-21 07:10:42.000000 idds-server-1.3.3/tools/env/config_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-21 07:10:42.000000 idds-server-1.3.3/tools/env/config_server
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-21 07:10:42.000000 idds-server-1.3.3/tools/env/create_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-21 07:10:42.000000 idds-server-1.3.3/tools/env/create_postgres_db.sh
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-21 07:10:42.000000 idds-server-1.3.3/tools/env/destroy_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-21 07:10:42.000000 idds-server-1.3.3/tools/env/dump_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-21 07:10:52.000000 idds-server-1.3.3/tools/env/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-21 07:10:42.000000 idds-server-1.3.3/tools/env/install_env_conda.sh
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-21 07:10:42.000000 idds-server-1.3.3/tools/env/install_idds.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-21 07:10:42.000000 idds-server-1.3.3/tools/env/install_idds_full.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      152 2023-07-21 07:10:42.000000 idds-server-1.3.3/tools/env/install_packages.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-21 07:10:42.000000 idds-server-1.3.3/tools/env/merge_configmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-21 07:10:42.000000 idds-server-1.3.3/tools/env/merge_idds_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-21 07:10:42.000000 idds-server-1.3.3/tools/env/setup_dev.sh
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-21 07:10:42.000000 idds-server-1.3.3/tools/env/setup_idds.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-21 07:10:42.000000 idds-server-1.3.3/tools/env/setup_panda.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.365461 idds-server-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-02 08:59:54.000000 idds-server-1.3.4/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-02 09:00:08.365461 idds-server-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-02 08:59:54.000000 idds-server-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.341461 idds-server-1.3.4/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1687 2023-08-02 08:59:54.000000 idds-server-1.3.4/bin/idds-daemon
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-02 09:00:08.000000 idds-server-1.3.4/bin/idds.wsgi
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-02 08:59:54.000000 idds-server-1.3.4/bin/idds.wsgi.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      584 2023-08-02 08:59:54.000000 idds-server-1.3.4/bin/run-idds
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-02 08:59:54.000000 idds-server-1.3.4/bin/run-idds-fake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.341461 idds-server-1.3.4/config_default/
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-08-02 08:59:54.000000 idds-server-1.3.4/config_default/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-02 08:59:54.000000 idds-server-1.3.4/config_default/auth.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-02 08:59:54.000000 idds-server-1.3.4/config_default/gacl
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-08-02 08:59:54.000000 idds-server-1.3.4/config_default/httpd-idds-443-py39-cc7.conf
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3678 2023-08-02 08:59:54.000000 idds-server-1.3.4/config_default/idds.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      125 2023-08-02 08:59:54.000000 idds-server-1.3.4/config_default/logrotate_daemon
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-02 08:59:54.000000 idds-server-1.3.4/config_default/logrotate_idds
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-02 08:59:54.000000 idds-server-1.3.4/config_default/panda.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-02 08:59:54.000000 idds-server-1.3.4/config_default/rucio.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-08-02 08:59:54.000000 idds-server-1.3.4/config_default/supervisord_httpd.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-08-02 08:59:54.000000 idds-server-1.3.4/config_default/supervisord_idds.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-02 08:59:54.000000 idds-server-1.3.4/config_default/supervisord_iddsfake.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-08-02 08:59:54.000000 idds-server-1.3.4/config_default/supervisord_logrotate.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-08-02 08:59:54.000000 idds-server-1.3.4/config_default/supervisord_syslog-ng.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.337461 idds-server-1.3.4/etc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.345461 idds-server-1.3.4/etc/idds/
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-08-02 08:59:54.000000 idds-server-1.3.4/etc/idds/alembic.ini.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.345461 idds-server-1.3.4/etc/idds/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-08-02 08:59:54.000000 idds-server-1.3.4/etc/idds/auth/auth.cfg.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.337461 idds-server-1.3.4/etc/idds/condor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.345461 idds-server-1.3.4/etc/idds/condor/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-08-02 08:59:54.000000 idds-server-1.3.4/etc/idds/condor/client/00personal_condor.config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.345461 idds-server-1.3.4/etc/idds/condor/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-02 08:59:54.000000 idds-server-1.3.4/etc/idds/condor/server/00personal_condor.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      811 2023-08-02 08:59:54.000000 idds-server-1.3.4/etc/idds/idds.cfg.client.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3946 2023-08-02 08:59:54.000000 idds-server-1.3.4/etc/idds/idds.cfg.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.345461 idds-server-1.3.4/etc/idds/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-02 08:59:54.000000 idds-server-1.3.4/etc/idds/rest/gacl.template
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-08-02 08:59:54.000000 idds-server-1.3.4/etc/idds/rest/httpd-idds-443-py36-cc7.conf.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-08-02 08:59:54.000000 idds-server-1.3.4/etc/idds/rest/httpd-idds-443-py36-cc7_normal.conf.template
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-08-02 09:00:08.000000 idds-server-1.3.4/etc/idds/rest/httpd-idds-443-py39-cc7.conf.install_template
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-08-02 08:59:54.000000 idds-server-1.3.4/etc/idds/rest/httpd-idds-443-py39-cc7.conf.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-08-02 08:59:54.000000 idds-server-1.3.4/etc/idds/rest/ssl.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.345461 idds-server-1.3.4/etc/idds/supervisord.d/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-08-02 08:59:54.000000 idds-server-1.3.4/etc/idds/supervisord.d/idds.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.345461 idds-server-1.3.4/etc/idds/website/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-08-02 08:59:54.000000 idds-server-1.3.4/etc/idds/website/25-port443.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-08-02 08:59:54.000000 idds-server-1.3.4/etc/idds/website/25-port80.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.345461 idds-server-1.3.4/etc/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)    25596 2023-08-02 08:59:54.000000 idds-server-1.3.4/etc/sql/oracle_11.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-08-02 08:59:54.000000 idds-server-1.3.4/etc/sql/oracle_11_test.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    22610 2023-08-02 08:59:54.000000 idds-server-1.3.4/etc/sql/oracle_19.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    18371 2023-08-02 08:59:54.000000 idds-server-1.3.4/etc/sql/oracle_update.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    18076 2023-08-02 08:59:54.000000 idds-server-1.3.4/etc/sql/postgresql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-02 08:59:54.000000 idds-server-1.3.4/etc/sql/postgresql_init.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-02 08:59:54.000000 idds-server-1.3.4/etc/sql/postgresql_update.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.341461 idds-server-1.3.4/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.345461 idds-server-1.3.4/lib/idds/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.345461 idds-server-1.3.4/lib/idds/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.345461 idds-server-1.3.4/lib/idds/agents/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/archive/archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/archive/run_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.349461 idds-server-1.3.4/lib/idds/agents/carrier/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/carrier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/carrier/finisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24651 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/carrier/poller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/carrier/receiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/carrier/submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14560 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/carrier/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95469 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/carrier/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.349461 idds-server-1.3.4/lib/idds/agents/clerk/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/clerk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67320 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/clerk/clerk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.349461 idds-server-1.3.4/lib/idds/agents/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/common/baseagent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.349461 idds-server-1.3.4/lib/idds/agents/common/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/common/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/common/cache/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.349461 idds-server-1.3.4/lib/idds/agents/common/eventbus/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/common/eventbus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/common/eventbus/baseeventbusbackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/common/eventbus/baseeventbusbackendopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/common/eventbus/dbeventbusbackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/common/eventbus/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/common/eventbus/eventbus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22179 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/common/eventbus/msgeventbusbackend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.349461 idds-server-1.3.4/lib/idds/agents/common/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/common/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15412 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/common/plugins/messaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/common/timerscheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/common/timertask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.349461 idds-server-1.3.4/lib/idds/agents/conductor/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/conductor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12932 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/conductor/conductor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/conductor/consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.353461 idds-server-1.3.4/lib/idds/agents/coordinator/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/coordinator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15040 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/coordinator/coordinator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5468 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.353461 idds-server-1.3.4/lib/idds/agents/marshaller/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/marshaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/marshaller/marshaller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.353461 idds-server-1.3.4/lib/idds/agents/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40926 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/transformer/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.353461 idds-server-1.3.4/lib/idds/agents/transporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/transporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22626 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/agents/transporter/transporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.353461 idds-server-1.3.4/lib/idds/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/api/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/api/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/api/contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/api/processings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/api/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/api/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.353461 idds-server-1.3.4/lib/idds/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30689 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/core/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/core/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/core/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/core/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19011 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/core/processings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20716 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/core/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/core/throttlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33651 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/core/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/core/workprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.357461 idds-server-1.3.4/lib/idds/orm/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/orm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.357461 idds-server-1.3.4/lib/idds/orm/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/orm/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.357461 idds-server-1.3.4/lib/idds/orm/base/alembic/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/orm/base/alembic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/orm/base/alembic/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.357461 idds-server-1.3.4/lib/idds/orm/base/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/orm/base/alembic/versions/0204f391c32d_add_poll_period_in_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/orm/base/alembic/versions/53d0af715dab_add_site_throttler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/orm/base/alembic/versions/5e0aa2aa1fa3_add_fetch_status_in_contents_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/orm/base/alembic/versions/6ca0e5e466eb_update_message_null_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/orm/base/alembic/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/orm/base/alembic/versions/b0ec813021d6_add_sub_map_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/orm/base/alembic/versions/f79663a7e94e_add_external_content_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/orm/base/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53545 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/orm/base/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13193 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/orm/base/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/orm/base/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/orm/base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16744 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/orm/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/orm/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41133 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/orm/contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11642 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/orm/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/orm/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/orm/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18139 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/orm/processings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50045 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/orm/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/orm/throttlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21562 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/orm/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/orm/workprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.357461 idds-server-1.3.4/lib/idds/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/rest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.357461 idds-server-1.3.4/lib/idds/rest/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/rest/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/rest/v1/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/rest/v1/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/rest/v1/cacher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/rest/v1/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/rest/v1/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/rest/v1/hyperparameteropt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/rest/v1/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/rest/v1/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28102 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/rest/v1/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/rest/v1/ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21409 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/rest/v1/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/rest/v1/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.365461 idds-server-1.3.4/lib/idds/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/activelearning_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/auth_test_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/cacher_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/catalog_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12118 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22834 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/core_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/core_tests_dep_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/core_tests_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/datacarousel_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/doma_build_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/find_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/fix_content_dep_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/fix_trasnform_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/hyperparameteropt_bayesian_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/hyperparameteropt_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/hyperparameteropt_docker_local_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/hyperparameteropt_docker_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/hyperparameteropt_nevergrad_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/jsonload_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/kill_workflow_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/logs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/match_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/message_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/message_test1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/migrating_requests_v1_to_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/os_boto3_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/panda_iam_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/panda_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/performance_test_with_cx_oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/performance_test_with_sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/relation_map_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/rest_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/retry_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/run_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/scaling_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/set_throttlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/split_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/test_activelearning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/test_atlaspandawork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/test_big_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34114 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/test_datacarousel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/test_domapanda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/test_domapanda_lsst_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/test_domapanda_pandaclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/test_domapanda_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/test_get_dn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/test_get_request_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/test_hyperparameteropt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/test_merge_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/test_migrate_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/test_request_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/test_running_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/test_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/test_transform_collection_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/test_transform_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28166 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/test_workflow_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69660 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/test_workflow_condition_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-08-02 08:59:54.000000 idds-server-1.3.4/lib/idds/tests/trigger_release.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-02 09:00:05.000000 idds-server-1.3.4/lib/idds/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.365461 idds-server-1.3.4/lib/idds_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-02 09:00:08.000000 idds-server-1.3.4/lib/idds_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-08-02 09:00:08.000000 idds-server-1.3.4/lib/idds_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 09:00:08.000000 idds-server-1.3.4/lib/idds_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-02 09:00:08.000000 idds-server-1.3.4/lib/idds_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 09:00:08.000000 idds-server-1.3.4/lib/idds_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-02 09:00:08.365461 idds-server-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-08-02 08:59:54.000000 idds-server-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.341461 idds-server-1.3.4/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:00:08.365461 idds-server-1.3.4/tools/env/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-08-02 08:59:54.000000 idds-server-1.3.4/tools/env/config_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-08-02 08:59:54.000000 idds-server-1.3.4/tools/env/config_server
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-08-02 08:59:54.000000 idds-server-1.3.4/tools/env/create_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-08-02 08:59:54.000000 idds-server-1.3.4/tools/env/create_postgres_db.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-08-02 08:59:54.000000 idds-server-1.3.4/tools/env/destroy_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-08-02 08:59:54.000000 idds-server-1.3.4/tools/env/dump_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-08-02 09:00:05.000000 idds-server-1.3.4/tools/env/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-02 08:59:54.000000 idds-server-1.3.4/tools/env/install_env_conda.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-02 08:59:54.000000 idds-server-1.3.4/tools/env/install_idds.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-08-02 08:59:54.000000 idds-server-1.3.4/tools/env/install_idds_full.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      152 2023-08-02 08:59:54.000000 idds-server-1.3.4/tools/env/install_packages.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-08-02 08:59:54.000000 idds-server-1.3.4/tools/env/merge_configmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-08-02 08:59:54.000000 idds-server-1.3.4/tools/env/merge_idds_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-08-02 08:59:54.000000 idds-server-1.3.4/tools/env/setup_dev.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-02 08:59:54.000000 idds-server-1.3.4/tools/env/setup_idds.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-02 08:59:54.000000 idds-server-1.3.4/tools/env/setup_panda.sh
```

### Comparing `idds-server-1.3.3/LICENSE.rst` & `idds-server-1.3.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/PKG-INFO` & `idds-server-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-server
-Version: 1.3.3
+Version: 1.3.4
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-server-1.3.3/bin/idds-daemon` & `idds-server-1.3.4/bin/idds-daemon`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/bin/idds.wsgi` & `idds-server-1.3.4/bin/idds.wsgi`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/bin/idds.wsgi.template` & `idds-server-1.3.4/bin/idds.wsgi.template`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/bin/run-idds` & `idds-server-1.3.4/bin/run-idds`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/config_default/alembic.ini` & `idds-server-1.3.4/config_default/alembic.ini`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/config_default/gacl` & `idds-server-1.3.4/config_default/gacl`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/config_default/httpd-idds-443-py39-cc7.conf` & `idds-server-1.3.4/config_default/httpd-idds-443-py39-cc7.conf`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/config_default/idds.cfg` & `idds-server-1.3.4/config_default/idds.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
                                         "destination": "/topic/doma.panda_idds",
                                         "username": "user",
                                         "password": "password",
                                         "broker_timeout": 360}}
 
 # domapandawork.life_time = 86400
 domapandawork.num_retries = 0
-domapandawork.poll_panda_jobs_chunk_size = 10000
+domapandawork.poll_panda_jobs_chunk_size = 2000
 
 [conductor]
 delay = 120
 replay_times = 2
 
 threshold_to_release_messages = 1000
 random_delay = 60
```

### Comparing `idds-server-1.3.3/config_default/rucio.cfg` & `idds-server-1.3.4/config_default/rucio.cfg`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/config_default/supervisord_httpd.ini` & `idds-server-1.3.4/config_default/supervisord_httpd.ini`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/config_default/supervisord_idds.ini` & `idds-server-1.3.4/config_default/supervisord_idds.ini`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/config_default/supervisord_iddsfake.ini` & `idds-server-1.3.4/config_default/supervisord_iddsfake.ini`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/config_default/supervisord_logrotate.ini` & `idds-server-1.3.4/config_default/supervisord_logrotate.ini`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/config_default/supervisord_syslog-ng.ini` & `idds-server-1.3.4/config_default/supervisord_syslog-ng.ini`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/etc/idds/alembic.ini.template` & `idds-server-1.3.4/etc/idds/alembic.ini.template`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/etc/idds/auth/auth.cfg.template` & `idds-server-1.3.4/etc/idds/auth/auth.cfg.template`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/etc/idds/condor/client/00personal_condor.config` & `idds-server-1.3.4/etc/idds/condor/client/00personal_condor.config`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/etc/idds/condor/server/00personal_condor.config` & `idds-server-1.3.4/etc/idds/condor/server/00personal_condor.config`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/etc/idds/idds.cfg.client.template` & `idds-server-1.3.4/etc/idds/idds.cfg.client.template`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/etc/idds/idds.cfg.template` & `idds-server-1.3.4/etc/idds/idds.cfg.template`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/etc/idds/rest/gacl.template` & `idds-server-1.3.4/etc/idds/rest/gacl.template`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/etc/idds/rest/httpd-idds-443-py36-cc7.conf.template` & `idds-server-1.3.4/etc/idds/rest/httpd-idds-443-py36-cc7.conf.template`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/etc/idds/rest/httpd-idds-443-py36-cc7_normal.conf.template` & `idds-server-1.3.4/etc/idds/rest/httpd-idds-443-py36-cc7_normal.conf.template`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/etc/idds/rest/httpd-idds-443-py39-cc7.conf.install_template` & `idds-server-1.3.4/etc/idds/rest/httpd-idds-443-py39-cc7.conf.install_template`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/etc/idds/rest/httpd-idds-443-py39-cc7.conf.template` & `idds-server-1.3.4/etc/idds/rest/httpd-idds-443-py39-cc7.conf.template`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/etc/idds/rest/ssl.conf` & `idds-server-1.3.4/etc/idds/rest/ssl.conf`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/etc/idds/supervisord.d/idds.ini` & `idds-server-1.3.4/etc/idds/supervisord.d/idds.ini`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/etc/idds/website/25-port443.conf` & `idds-server-1.3.4/etc/idds/website/25-port443.conf`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/etc/sql/oracle_11.sql` & `idds-server-1.3.4/etc/sql/oracle_11.sql`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/etc/sql/oracle_11_test.sql` & `idds-server-1.3.4/etc/sql/oracle_11_test.sql`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/etc/sql/oracle_19.sql` & `idds-server-1.3.4/etc/sql/oracle_19.sql`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/etc/sql/oracle_update.sql` & `idds-server-1.3.4/etc/sql/oracle_update.sql`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/etc/sql/postgresql.sql` & `idds-server-1.3.4/etc/sql/postgresql.sql`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/etc/sql/postgresql_init.sql` & `idds-server-1.3.4/etc/sql/postgresql_init.sql`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/agents/archive/archiver.py` & `idds-server-1.3.4/lib/idds/agents/archive/archiver.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/agents/archive/run_archive.py` & `idds-server-1.3.4/lib/idds/agents/archive/run_archive.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/agents/carrier/finisher.py` & `idds-server-1.3.4/lib/idds/agents/carrier/finisher.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/agents/carrier/poller.py` & `idds-server-1.3.4/lib/idds/agents/carrier/poller.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/agents/carrier/receiver.py` & `idds-server-1.3.4/lib/idds/agents/carrier/receiver.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/agents/carrier/submitter.py` & `idds-server-1.3.4/lib/idds/agents/carrier/submitter.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/agents/carrier/trigger.py` & `idds-server-1.3.4/lib/idds/agents/carrier/trigger.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/agents/carrier/utils.py` & `idds-server-1.3.4/lib/idds/agents/carrier/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,23 +93,27 @@
         else:
             # list of content_id, status,
             if content[1] not in [ContentStatus.Available, ContentStatus.FakeAvailable]:
                 return False
     return True
 
 
-def is_all_contents_terminated(contents):
+def is_all_contents_terminated(contents, terminated=False):
+    terminated_status = [ContentStatus.Available, ContentStatus.FakeAvailable,
+                         ContentStatus.FinalFailed, ContentStatus.Missing]
+    if terminated:
+        terminated_status = [ContentStatus.Available, ContentStatus.FakeAvailable, ContentStatus.Failed,
+                             ContentStatus.FinalFailed, ContentStatus.Missing]
+
     for content in contents:
         if type(content) is dict:
-            if content['substatus'] not in [ContentStatus.Available, ContentStatus.FakeAvailable,
-                                            ContentStatus.FinalFailed, ContentStatus.Missing]:
+            if content['substatus'] not in terminated_status:
                 return False
         else:
-            if content[1] not in [ContentStatus.Available, ContentStatus.FakeAvailable,
-                                  ContentStatus.FinalFailed, ContentStatus.Missing]:
+            if content[1] not in terminated_status:
                 return False
     return True
 
 
 def is_input_dependency_terminated(input_dependency):
     if type(input_dependency) is dict:
         if input_dependency['substatus'] in [ContentStatus.Available, ContentStatus.FakeAvailable,
@@ -118,26 +122,30 @@
     else:
         if input_dependency[1] in [ContentStatus.Available, ContentStatus.FakeAvailable,
                                    ContentStatus.FinalFailed, ContentStatus.Missing]:
             return True
     return False
 
 
-def is_all_contents_terminated_but_not_available(inputs):
+def is_all_contents_terminated_but_not_available(inputs, terminated=False):
+    terminated_status = [ContentStatus.Available, ContentStatus.FakeAvailable,
+                         ContentStatus.FinalFailed, ContentStatus.Missing]
+    if terminated:
+        terminated_status = [ContentStatus.Available, ContentStatus.FakeAvailable, ContentStatus.Failed,
+                             ContentStatus.FinalFailed, ContentStatus.Missing]
+
     all_contents_available = True
     for content in inputs:
         if type(content) is dict:
-            if content['substatus'] not in [ContentStatus.Available, ContentStatus.FakeAvailable,
-                                            ContentStatus.FinalFailed, ContentStatus.Missing]:
+            if content['substatus'] not in terminated_status:
                 return False
             if content['substatus'] not in [ContentStatus.Available]:
                 all_contents_available = False
         else:
-            if content[1] not in [ContentStatus.Available, ContentStatus.FakeAvailable,
-                                  ContentStatus.FinalFailed, ContentStatus.Missing]:
+            if content[1] not in terminated_status:
                 return False
             if content[1] not in [ContentStatus.Available]:
                 all_contents_available = False
     if all_contents_available:
         return False
     return True
 
@@ -553,15 +561,15 @@
         sub_map_id = content['sub_map_id']
         if sub_map_id not in input_output_sub_maps:
             input_output_sub_maps[sub_map_id] = {'inputs': [], 'outputs': [], 'logs': [], 'inputs_dependency': []}
         input_output_sub_maps[sub_map_id]['logs'].append(content)
     return input_output_sub_maps
 
 
-def get_updated_contents_by_input_output_maps(input_output_maps=None, logger=None, log_prefix=''):
+def get_updated_contents_by_input_output_maps(input_output_maps=None, terminated=False, logger=None, log_prefix=''):
     updated_contents, updated_contents_full_input, updated_contents_full_output = [], [], []
     updated_contents_full_input_deps = []
     new_update_contents = []
 
     status_to_check = [ContentStatus.Available, ContentStatus.FakeAvailable, ContentStatus.FinalFailed,
                        ContentStatus.Missing, ContentStatus.Failed, ContentStatus.Lost,
                        ContentStatus.Deleted]
@@ -611,15 +619,15 @@
             inputs_sub = input_output_sub_maps[sub_map_id]['inputs']
             outputs_sub = input_output_sub_maps[sub_map_id]['outputs']
             inputs_dependency_sub = input_output_sub_maps[sub_map_id]['inputs_dependency']
 
             input_content_update_status = None
             if is_all_contents_available(inputs_dependency_sub):
                 input_content_update_status = ContentStatus.Available
-            elif is_all_contents_terminated(inputs_dependency_sub):
+            elif is_all_contents_terminated(inputs_dependency_sub, terminated):
                 input_content_update_status = ContentStatus.Missing
             if input_content_update_status:
                 for content in inputs_sub:
                     if content['substatus'] != input_content_update_status:
                         u_content = {'content_id': content['content_id'],
                                      'status': input_content_update_status,
                                      'substatus': input_content_update_status}
@@ -635,15 +643,15 @@
                                                'coll_id': content['coll_id']}
                         new_update_contents.append(u_content_substatus)
 
             output_content_update_status = None
             if is_all_contents_available(inputs_sub):
                 # wait for the job to finish
                 pass
-            elif is_all_contents_terminated_but_not_available(inputs_sub):
+            elif is_all_contents_terminated_but_not_available(inputs_sub, terminated):
                 output_content_update_status = ContentStatus.Missing
             if output_content_update_status:
                 for content in outputs_sub:
                     if content['substatus'] != output_content_update_status:
                         u_content = {'content_id': content['content_id'],
                                      'status': output_content_update_status,
                                      'substatus': output_content_update_status}
@@ -1133,15 +1141,20 @@
         to_triggered_contents = core_catalog.get_update_contents_from_others_by_dep_id(request_id=request_id, transform_id=transform_id)
         core_catalog.update_contents(to_triggered_contents)
         logger.debug(log_prefix + "update_contents_from_others_by_dep_id done")
 
         input_output_maps = get_input_output_maps(transform_id, work)
         logger.debug(log_prefix + "input_output_maps.keys[:2]: %s" % str(list(input_output_maps.keys())[:2]))
 
-        updated_contents_ret = get_updated_contents_by_input_output_maps(input_output_maps=input_output_maps, logger=logger, log_prefix=log_prefix)
+        terminated_processing = False
+        terminated_status = [ProcessingStatus.Finished, ProcessingStatus.Failed, ProcessingStatus.SubFinished,
+                             ProcessingStatus.Terminating, ProcessingStatus.Cancelled]
+        if processing['status'] in terminated_status or processing['substatus'] in terminated_status:
+            terminated_processing = True
+        updated_contents_ret = get_updated_contents_by_input_output_maps(input_output_maps=input_output_maps, terminated=terminated_processing, logger=logger, log_prefix=log_prefix)
 
         updated_contents, updated_contents_full_input, updated_contents_full_output, updated_contents_full_input_deps, new_update_contents = updated_contents_ret
         logger.debug(log_prefix + "handle_trigger_processing: updated_contents[:3] %s" % (updated_contents[:3]))
 
         if updated_contents_full_input:
             # if the content is updated by receiver, here is the place to broadcast the messages
             msgs = generate_messages(request_id, transform_id, workload_id, work, msg_type='file',
@@ -1554,15 +1567,15 @@
             coll_status[content['coll_id']]['ext_files'] += 1
 
             if content['status'] in [ContentStatus.Available, ContentStatus.Mapped,
                                      ContentStatus.Available.value, ContentStatus.Mapped.value,
                                      ContentStatus.FakeAvailable, ContentStatus.FakeAvailable.value]:
                 coll_status[content['coll_id']]['processed_ext_files'] += 1
             # elif content['status'] in [ContentStatus.Failed, ContentStatus.FinalFailed]:
-            elif content['status'] in [ContentStatus.FinalFailed]:
+            elif content['status'] in [ContentStatus.Failed, ContentStatus.FinalFailed]:
                 coll_status[content['coll_id']]['failed_ext_files'] += 1
             elif content['status'] in [ContentStatus.Lost, ContentStatus.Deleted, ContentStatus.Missing]:
                 coll_status[content['coll_id']]['missing_ext_files'] += 1
 
     input_collections = work.get_input_collections(poll_externel=True)
     output_collections = work.get_output_collections()
     log_collections = work.get_log_collections()
@@ -1677,24 +1690,29 @@
         else:
             work.status = WorkStatus.SubFinished
 
 
 def sync_processing(processing, agent_attributes, terminate=False, abort=False, logger=None, log_prefix=""):
     logger = get_logger()
 
+    terminated_status = [ProcessingStatus.Finished, ProcessingStatus.Failed, ProcessingStatus.SubFinished,
+                         ProcessingStatus.Terminating, ProcessingStatus.Cancelled]
+
     request_id = processing['request_id']
     transform_id = processing['transform_id']
     workload_id = processing['workload_id']
 
     proc = processing['processing_metadata']['processing']
     work = proc.work
     work.set_agent_attributes(agent_attributes, processing)
 
     messages = []
     input_output_maps = get_input_output_maps(transform_id, work)
+    if processing['substatus'] in terminated_status or processing['substatus'] in terminated_status:
+        terminate = True
     update_collections, all_updates_flushed, msgs = sync_collection_status(request_id, transform_id, workload_id, work,
                                                                            input_output_maps=input_output_maps,
                                                                            close_collection=True, abort=abort, terminate=terminate)
 
     messages += msgs
 
     sync_work_status(request_id, transform_id, workload_id, work)
```

### Comparing `idds-server-1.3.3/lib/idds/agents/clerk/clerk.py` & `idds-server-1.3.4/lib/idds/agents/clerk/clerk.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/agents/common/baseagent.py` & `idds-server-1.3.4/lib/idds/agents/common/baseagent.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/agents/common/cache/redis.py` & `idds-server-1.3.4/lib/idds/agents/common/cache/redis.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/agents/common/eventbus/baseeventbusbackend.py` & `idds-server-1.3.4/lib/idds/agents/common/eventbus/baseeventbusbackend.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/agents/common/eventbus/baseeventbusbackendopt.py` & `idds-server-1.3.4/lib/idds/agents/common/eventbus/baseeventbusbackendopt.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/agents/common/eventbus/dbeventbusbackend.py` & `idds-server-1.3.4/lib/idds/agents/common/eventbus/dbeventbusbackend.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/agents/common/eventbus/eventbus.py` & `idds-server-1.3.4/lib/idds/agents/common/eventbus/eventbus.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/agents/common/eventbus/msgeventbusbackend.py` & `idds-server-1.3.4/lib/idds/agents/common/eventbus/msgeventbusbackend.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/agents/common/plugins/messaging.py` & `idds-server-1.3.4/lib/idds/agents/common/plugins/messaging.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/agents/common/timerscheduler.py` & `idds-server-1.3.4/lib/idds/agents/common/timerscheduler.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/agents/common/timertask.py` & `idds-server-1.3.4/lib/idds/agents/common/timertask.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/agents/conductor/conductor.py` & `idds-server-1.3.4/lib/idds/agents/conductor/conductor.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/agents/conductor/consumer.py` & `idds-server-1.3.4/lib/idds/agents/conductor/consumer.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/agents/coordinator/coordinator.py` & `idds-server-1.3.4/lib/idds/agents/coordinator/coordinator.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/agents/main.py` & `idds-server-1.3.4/lib/idds/agents/main.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/agents/marshaller/marshaller.py` & `idds-server-1.3.4/lib/idds/agents/marshaller/marshaller.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/agents/transformer/transformer.py` & `idds-server-1.3.4/lib/idds/agents/transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/agents/transporter/transporter.py` & `idds-server-1.3.4/lib/idds/agents/transporter/transporter.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/api/catalog.py` & `idds-server-1.3.4/lib/idds/api/catalog.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/api/collections.py` & `idds-server-1.3.4/lib/idds/api/collections.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/api/contents.py` & `idds-server-1.3.4/lib/idds/api/contents.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/api/processings.py` & `idds-server-1.3.4/lib/idds/api/processings.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/api/requests.py` & `idds-server-1.3.4/lib/idds/api/requests.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/api/transforms.py` & `idds-server-1.3.4/lib/idds/api/transforms.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/core/catalog.py` & `idds-server-1.3.4/lib/idds/core/catalog.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/core/commands.py` & `idds-server-1.3.4/lib/idds/core/commands.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/core/events.py` & `idds-server-1.3.4/lib/idds/core/events.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/core/health.py` & `idds-server-1.3.4/lib/idds/core/health.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/core/messages.py` & `idds-server-1.3.4/lib/idds/core/messages.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/core/processings.py` & `idds-server-1.3.4/lib/idds/core/processings.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/core/requests.py` & `idds-server-1.3.4/lib/idds/core/requests.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/core/throttlers.py` & `idds-server-1.3.4/lib/idds/core/throttlers.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/core/transforms.py` & `idds-server-1.3.4/lib/idds/core/transforms.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/core/workprogress.py` & `idds-server-1.3.4/lib/idds/core/workprogress.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/orm/base/alembic/env.py` & `idds-server-1.3.4/lib/idds/orm/base/alembic/env.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/orm/base/alembic/versions/0204f391c32d_add_poll_period_in_message.py` & `idds-server-1.3.4/lib/idds/orm/base/alembic/versions/0204f391c32d_add_poll_period_in_message.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/orm/base/alembic/versions/53d0af715dab_add_site_throttler.py` & `idds-server-1.3.4/lib/idds/orm/base/alembic/versions/53d0af715dab_add_site_throttler.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/orm/base/alembic/versions/5e0aa2aa1fa3_add_fetch_status_in_contents_update.py` & `idds-server-1.3.4/lib/idds/orm/base/alembic/versions/5e0aa2aa1fa3_add_fetch_status_in_contents_update.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/orm/base/alembic/versions/6ca0e5e466eb_update_message_null_constraints.py` & `idds-server-1.3.4/lib/idds/orm/base/alembic/versions/6ca0e5e466eb_update_message_null_constraints.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/orm/base/alembic/versions/b0ec813021d6_add_sub_map_id.py` & `idds-server-1.3.4/lib/idds/orm/base/alembic/versions/b0ec813021d6_add_sub_map_id.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/orm/base/alembic/versions/f79663a7e94e_add_external_content_id.py` & `idds-server-1.3.4/lib/idds/orm/base/alembic/versions/f79663a7e94e_add_external_content_id.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/orm/base/enum.py` & `idds-server-1.3.4/lib/idds/orm/base/enum.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/orm/base/models.py` & `idds-server-1.3.4/lib/idds/orm/base/models.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/orm/base/session.py` & `idds-server-1.3.4/lib/idds/orm/base/session.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/orm/base/types.py` & `idds-server-1.3.4/lib/idds/orm/base/types.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/orm/base/utils.py` & `idds-server-1.3.4/lib/idds/orm/base/utils.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/orm/collections.py` & `idds-server-1.3.4/lib/idds/orm/collections.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/orm/commands.py` & `idds-server-1.3.4/lib/idds/orm/commands.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/orm/contents.py` & `idds-server-1.3.4/lib/idds/orm/contents.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/orm/events.py` & `idds-server-1.3.4/lib/idds/orm/events.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/orm/health.py` & `idds-server-1.3.4/lib/idds/orm/health.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/orm/messages.py` & `idds-server-1.3.4/lib/idds/orm/messages.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/orm/processings.py` & `idds-server-1.3.4/lib/idds/orm/processings.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/orm/requests.py` & `idds-server-1.3.4/lib/idds/orm/requests.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/orm/throttlers.py` & `idds-server-1.3.4/lib/idds/orm/throttlers.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/orm/transforms.py` & `idds-server-1.3.4/lib/idds/orm/transforms.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/orm/workprogress.py` & `idds-server-1.3.4/lib/idds/orm/workprogress.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/rest/v1/app.py` & `idds-server-1.3.4/lib/idds/rest/v1/app.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/rest/v1/auth.py` & `idds-server-1.3.4/lib/idds/rest/v1/auth.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/rest/v1/cacher.py` & `idds-server-1.3.4/lib/idds/rest/v1/cacher.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/rest/v1/catalog.py` & `idds-server-1.3.4/lib/idds/rest/v1/catalog.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/rest/v1/controller.py` & `idds-server-1.3.4/lib/idds/rest/v1/controller.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/rest/v1/hyperparameteropt.py` & `idds-server-1.3.4/lib/idds/rest/v1/hyperparameteropt.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/rest/v1/logs.py` & `idds-server-1.3.4/lib/idds/rest/v1/logs.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/rest/v1/messages.py` & `idds-server-1.3.4/lib/idds/rest/v1/messages.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/rest/v1/monitor.py` & `idds-server-1.3.4/lib/idds/rest/v1/monitor.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/rest/v1/ping.py` & `idds-server-1.3.4/lib/idds/rest/v1/ping.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/rest/v1/requests.py` & `idds-server-1.3.4/lib/idds/rest/v1/requests.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/rest/v1/utils.py` & `idds-server-1.3.4/lib/idds/rest/v1/utils.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/activelearning_test.py` & `idds-server-1.3.4/lib/idds/tests/activelearning_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/auth_test_script.py` & `idds-server-1.3.4/lib/idds/tests/auth_test_script.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/cacher_test.py` & `idds-server-1.3.4/lib/idds/tests/cacher_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/catalog_test.py` & `idds-server-1.3.4/lib/idds/tests/catalog_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/client_test.py` & `idds-server-1.3.4/lib/idds/tests/client_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/common.py` & `idds-server-1.3.4/lib/idds/tests/common.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/core_tests.py` & `idds-server-1.3.4/lib/idds/tests/core_tests.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/core_tests_dep_id.py` & `idds-server-1.3.4/lib/idds/tests/core_tests_dep_id.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/core_tests_stat.py` & `idds-server-1.3.4/lib/idds/tests/core_tests_stat.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/datacarousel_test.py` & `idds-server-1.3.4/lib/idds/tests/datacarousel_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/doma_build_test.py` & `idds-server-1.3.4/lib/idds/tests/doma_build_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/find_dependencies.py` & `idds-server-1.3.4/lib/idds/tests/find_dependencies.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/fix_content_dep_id.py` & `idds-server-1.3.4/lib/idds/tests/fix_content_dep_id.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/fix_trasnform_name.py` & `idds-server-1.3.4/lib/idds/tests/fix_trasnform_name.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/hyperparameteropt_bayesian_test.py` & `idds-server-1.3.4/lib/idds/tests/hyperparameteropt_bayesian_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/hyperparameteropt_client_test.py` & `idds-server-1.3.4/lib/idds/tests/hyperparameteropt_client_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/hyperparameteropt_docker_local_test.py` & `idds-server-1.3.4/lib/idds/tests/hyperparameteropt_docker_local_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/hyperparameteropt_docker_test.py` & `idds-server-1.3.4/lib/idds/tests/hyperparameteropt_docker_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/hyperparameteropt_nevergrad_test.py` & `idds-server-1.3.4/lib/idds/tests/hyperparameteropt_nevergrad_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/jsonload_test.py` & `idds-server-1.3.4/lib/idds/tests/jsonload_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/kill_workflow_task.py` & `idds-server-1.3.4/lib/idds/tests/kill_workflow_task.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/logs_test.py` & `idds-server-1.3.4/lib/idds/tests/logs_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/match_test.py` & `idds-server-1.3.4/lib/idds/tests/match_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/message_test.py` & `idds-server-1.3.4/lib/idds/tests/message_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/message_test1.py` & `idds-server-1.3.4/lib/idds/tests/message_test1.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/migrating_requests_v1_to_v2.py` & `idds-server-1.3.4/lib/idds/tests/migrating_requests_v1_to_v2.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/panda_iam_test.py` & `idds-server-1.3.4/lib/idds/tests/panda_iam_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/panda_test.py` & `idds-server-1.3.4/lib/idds/tests/panda_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,22 @@
 os.environ['PANDA_BEHIND_REAL_LB'] = "1"
 # os.environ['PANDA_URL'] = 'http://rubin-panda-server-dev.slac.stanford.edu:80/server/panda'
 # os.environ['PANDA_URL_SSL'] = 'https://rubin-panda-server-dev.slac.stanford.edu:8443/server/panda'
 
 from pandaclient import Client  # noqa E402
 
 
+task_ids = [160871, 160873, 160874, 160872, 160875]
+for task_id in task_ids:
+    print("retry %s" % task_id)
+    ret = Client.retryTask(task_id, verbose=True)
+    print(ret)
+
+sys.exit(0)
+
 task_ids = [i for i in range(157023, 157050)]
 task_ids = []
 for task_id in task_ids:
     print("Killing %s" % task_id)
     ret = Client.killTask(task_id)
     print(ret)
```

### Comparing `idds-server-1.3.3/lib/idds/tests/performance_test_with_cx_oracle.py` & `idds-server-1.3.4/lib/idds/tests/performance_test_with_cx_oracle.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/performance_test_with_sqlalchemy.py` & `idds-server-1.3.4/lib/idds/tests/performance_test_with_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/relation_map_test.py` & `idds-server-1.3.4/lib/idds/tests/relation_map_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/rest_test.py` & `idds-server-1.3.4/lib/idds/tests/rest_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/run_sql.py` & `idds-server-1.3.4/lib/idds/tests/run_sql.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/scaling_checks.py` & `idds-server-1.3.4/lib/idds/tests/scaling_checks.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/split_messages.py` & `idds-server-1.3.4/lib/idds/tests/split_messages.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/test_activelearning.py` & `idds-server-1.3.4/lib/idds/tests/test_activelearning.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/test_atlaspandawork.py` & `idds-server-1.3.4/lib/idds/tests/test_atlaspandawork.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/test_auth.py` & `idds-server-1.3.4/lib/idds/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/test_big_request.py` & `idds-server-1.3.4/lib/idds/tests/test_big_request.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/test_catalog.py` & `idds-server-1.3.4/lib/idds/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/test_client.py` & `idds-server-1.3.4/lib/idds/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/test_datacarousel.py` & `idds-server-1.3.4/lib/idds/tests/test_datacarousel.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/test_domapanda.py` & `idds-server-1.3.4/lib/idds/tests/test_domapanda.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,16 @@
 
 task_queue = 'DOMA_LSST_GOOGLE_TEST'
 # task_queue = 'DOMA_LSST_GOOGLE_MERGE'
 # task_queue = 'SLAC_TEST'
 # task_queue = 'DOMA_LSST_SLAC_TEST'
 task_queue = 'SLAC_Rubin'
 # task_queue = 'SLAC_Rubin_Extra_Himem_32Cores'
+# task_queue = 'SLAC_Rubin_Merge'
+# task_queue = 'SLAC_TEST'
 
 # task_cloud = 'EU'
 # task_queue = 'CC-IN2P3_TEST'
 
 # task_cloud = 'EU'
 # task_queue = 'LANCS_TEST'
```

### Comparing `idds-server-1.3.3/lib/idds/tests/test_domapanda_lsst_workflow.py` & `idds-server-1.3.4/lib/idds/tests/test_domapanda_lsst_workflow.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/test_domapanda_pandaclient.py` & `idds-server-1.3.4/lib/idds/tests/test_domapanda_pandaclient.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/test_domapanda_workflow.py` & `idds-server-1.3.4/lib/idds/tests/test_domapanda_workflow.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/test_get_dn.py` & `idds-server-1.3.4/lib/idds/tests/test_get_dn.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/test_get_request_info.py` & `idds-server-1.3.4/lib/idds/tests/test_get_request_info.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/test_hyperparameteropt.py` & `idds-server-1.3.4/lib/idds/tests/test_hyperparameteropt.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/test_logger.py` & `idds-server-1.3.4/lib/idds/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/test_merge_dict.py` & `idds-server-1.3.4/lib/idds/tests/test_merge_dict.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/test_migrate_requests.py` & `idds-server-1.3.4/lib/idds/tests/test_migrate_requests.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,16 @@
     # atlas
     atlas_host = 'https://aipanda181.cern.ch:443/idds'  # noqa F841
     # doma google
     doma_google_host = 'https://34.133.138.229:443/idds'  # noqa F841
 
     slac_k8s_dev_host = 'https://rubin-panda-idds-dev.slac.stanford.edu:8443/idds'  # noqa F841
 
+    slac_k8s_prod_host = 'https://usdf-panda-idds.slac.stanford.edu:8443/idds'  # noqa F841
+
     cern_k8s_dev_host = 'https://panda-idds-dev.cern.ch/idds'  # noqa F841
 
     # cm1 = ClientManager(host=atlas_host)
     cm1 = ClientManager(host=doma_host)
     # cm1 = ClientManager(host=slac_k8s_dev_host)
     # reqs = cm1.get_requests(request_id=290)
     # old_request_id = 298163
@@ -65,18 +67,19 @@
     # old_request_id = 1
     # for old_request_id in [152]:
     # for old_request_id in [60]:    # noqa E115
     # for old_request_id in [200]:    # noqa E115
     for old_request_id in old_request_ids:    # noqa E115  # doma 183
         reqs = cm1.get_requests(request_id=old_request_id, with_metadata=True)
 
-        cm2 = ClientManager(host=dev_host)
+        # cm2 = ClientManager(host=dev_host)
         # cm2 = ClientManager(host=doma_host)
         # cm2 = ClientManager(host=atlas_host)
         # cm2 = ClientManager(host=slac_k8s_dev_host)
+        cm2 = ClientManager(host=slac_k8s_prod_host)
         # cm2 = ClientManager(host=cern_k8s_dev_host)
         # print(reqs)
 
         print("num requests: %s" % len(reqs))
         for req in reqs[:1]:
             # print(req)
             # workflow = req['request_metadata']['workflow']
```

### Comparing `idds-server-1.3.3/lib/idds/tests/test_request_transform.py` & `idds-server-1.3.4/lib/idds/tests/test_request_transform.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/test_requests.py` & `idds-server-1.3.4/lib/idds/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/test_running_data.py` & `idds-server-1.3.4/lib/idds/tests/test_running_data.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/test_scaling.py` & `idds-server-1.3.4/lib/idds/tests/test_scaling.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/test_transform_collection_content.py` & `idds-server-1.3.4/lib/idds/tests/test_transform_collection_content.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/test_transform_processing.py` & `idds-server-1.3.4/lib/idds/tests/test_transform_processing.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/test_workflow.py` & `idds-server-1.3.4/lib/idds/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/test_workflow_condition.py` & `idds-server-1.3.4/lib/idds/tests/test_workflow_condition.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/test_workflow_condition_v2.py` & `idds-server-1.3.4/lib/idds/tests/test_workflow_condition_v2.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds/tests/trigger_release.py` & `idds-server-1.3.4/lib/idds/tests/trigger_release.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/lib/idds_server.egg-info/PKG-INFO` & `idds-server-1.3.4/lib/idds_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-server
-Version: 1.3.3
+Version: 1.3.4
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-server-1.3.3/lib/idds_server.egg-info/SOURCES.txt` & `idds-server-1.3.4/lib/idds_server.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -167,14 +167,15 @@
 lib/idds/tests/jsonload_test.py
 lib/idds/tests/kill_workflow_task.py
 lib/idds/tests/logs_test.py
 lib/idds/tests/match_test.py
 lib/idds/tests/message_test.py
 lib/idds/tests/message_test1.py
 lib/idds/tests/migrating_requests_v1_to_v2.py
+lib/idds/tests/os_boto3_test.py
 lib/idds/tests/panda_iam_test.py
 lib/idds/tests/panda_test.py
 lib/idds/tests/performance_test_with_cx_oracle.py
 lib/idds/tests/performance_test_with_sqlalchemy.py
 lib/idds/tests/relation_map_test.py
 lib/idds/tests/rest_test.py
 lib/idds/tests/retry_processing.py
```

### Comparing `idds-server-1.3.3/setup.py` & `idds-server-1.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/tools/env/config_monitor.py` & `idds-server-1.3.4/tools/env/config_monitor.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/tools/env/create_database.py` & `idds-server-1.3.4/tools/env/create_database.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/tools/env/destroy_database.py` & `idds-server-1.3.4/tools/env/destroy_database.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/tools/env/dump_database.py` & `idds-server-1.3.4/tools/env/dump_database.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/tools/env/environment.yml` & `idds-server-1.3.4/tools/env/environment.yml`

 * *Files 1% similar despite different names*

```diff
@@ -28,10 +28,10 @@
   - cryptography
   - redis
   - alembic
   - deepdiff
   - pyzmq
   - oic
   - lsst-ctrl-bps
-  - idds-common==1.3.3
-  - idds-workflow==1.3.3
-  - idds-client==1.3.3
+  - idds-common==1.3.4
+  - idds-workflow==1.3.4
+  - idds-client==1.3.4
```

### Comparing `idds-server-1.3.3/tools/env/install_env_conda.sh` & `idds-server-1.3.4/tools/env/install_env_conda.sh`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/tools/env/install_idds_full.sh` & `idds-server-1.3.4/tools/env/install_idds_full.sh`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/tools/env/merge_configmap.py` & `idds-server-1.3.4/tools/env/merge_configmap.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/tools/env/merge_idds_configs.py` & `idds-server-1.3.4/tools/env/merge_idds_configs.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/tools/env/setup_dev.sh` & `idds-server-1.3.4/tools/env/setup_dev.sh`

 * *Files identical despite different names*

### Comparing `idds-server-1.3.3/tools/env/setup_panda.sh` & `idds-server-1.3.4/tools/env/setup_panda.sh`

 * *Files identical despite different names*

