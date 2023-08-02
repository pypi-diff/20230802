# Comparing `tmp/csirtg-indicator-3.0b8.tar.gz` & `tmp/csirtg-indicator-3.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/csirtg-indicator-3.0b8.tar", last modified: Sun Jun  7 13:23:38 2020, max compression
+gzip compressed data, was "dist/csirtg-indicator-3.0b9.tar", last modified: Fri Jun 12 17:59:11 2020, max compression
```

## Comparing `csirtg-indicator-3.0b8.tar` & `csirtg-indicator-3.0b9.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-07 13:23:38.362985 csirtg-indicator-3.0b8/
--rw-r--r--   0 runner    (1001) docker     (116)      662 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (116)    16725 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      313 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)      330 2020-06-07 13:23:38.362985 csirtg-indicator-3.0b8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      500 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-07 13:23:38.362985 csirtg-indicator-3.0b8/csirtg_indicator/
--rw-r--r--   0 runner    (1001) docker     (116)     5961 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/csirtg_indicator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      497 2020-06-07 13:23:38.362985 csirtg-indicator-3.0b8/csirtg_indicator/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-07 13:23:38.358984 csirtg-indicator-3.0b8/csirtg_indicator/constants/
--rw-r--r--   0 runner    (1001) docker     (116)      703 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/csirtg_indicator/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      942 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/csirtg_indicator/constants/fields.py
--rw-r--r--   0 runner    (1001) docker     (116)     1228 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/csirtg_indicator/constants/networks.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-07 13:23:38.358984 csirtg-indicator-3.0b8/csirtg_indicator/feed/
--rw-r--r--   0 runner    (1001) docker     (116)      972 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/csirtg_indicator/feed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      964 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/csirtg_indicator/feed/fqdn.py
--rw-r--r--   0 runner    (1001) docker     (116)     1034 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/csirtg_indicator/feed/ipv4.py
--rw-r--r--   0 runner    (1001) docker     (116)      645 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/csirtg_indicator/feed/ipv6.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-07 13:23:38.358984 csirtg-indicator-3.0b8/csirtg_indicator/format/
--rw-r--r--   0 runner    (1001) docker     (116)      620 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/csirtg_indicator/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      774 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/csirtg_indicator/format/bind.py
--rw-r--r--   0 runner    (1001) docker     (116)     1531 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/csirtg_indicator/format/bindrpz.py
--rw-r--r--   0 runner    (1001) docker     (116)     1636 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/csirtg_indicator/format/bro.py
--rw-r--r--   0 runner    (1001) docker     (116)      646 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/csirtg_indicator/format/csv.py
--rw-r--r--   0 runner    (1001) docker     (116)      671 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/csirtg_indicator/format/gexf.py
--rw-r--r--   0 runner    (1001) docker     (116)      566 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/csirtg_indicator/format/json.py
--rw-r--r--   0 runner    (1001) docker     (116)     2079 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/csirtg_indicator/format/snort.py
--rw-r--r--   0 runner    (1001) docker     (116)     1093 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/csirtg_indicator/format/table.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-07 13:23:38.358984 csirtg-indicator-3.0b8/csirtg_indicator/utils/
--rw-r--r--   0 runner    (1001) docker     (116)     3085 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/csirtg_indicator/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      698 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/csirtg_indicator/utils/confidence.py
--rw-r--r--   0 runner    (1001) docker     (116)     1196 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/csirtg_indicator/utils/fqdn.py
--rw-r--r--   0 runner    (1001) docker     (116)      942 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/csirtg_indicator/utils/ip.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-07 13:23:38.362985 csirtg-indicator-3.0b8/csirtg_indicator/wrappers/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/csirtg_indicator/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      520 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/csirtg_indicator/wrappers/cif.py
--rw-r--r--   0 runner    (1001) docker     (116)      480 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/csirtg_indicator/wrappers/csirtg.py
--rw-r--r--   0 runner    (1001) docker     (116)      958 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/csirtg_indicator/wrappers/dns.py
--rw-r--r--   0 runner    (1001) docker     (116)      599 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/csirtg_indicator/wrappers/farsight.py
--rw-r--r--   0 runner    (1001) docker     (116)      788 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/csirtg_indicator/wrappers/formatter.py
--rw-r--r--   0 runner    (1001) docker     (116)      619 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/csirtg_indicator/wrappers/geo.py
--rw-r--r--   0 runner    (1001) docker     (116)     1715 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/csirtg_indicator/wrappers/itypes.py
--rw-r--r--   0 runner    (1001) docker     (116)      205 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/csirtg_indicator/wrappers/peers.py
--rw-r--r--   0 runner    (1001) docker     (116)     3320 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/csirtg_indicator/wrappers/properties.py
--rw-r--r--   0 runner    (1001) docker     (116)      906 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/csirtg_indicator/wrappers/spamhaus.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-07 13:23:38.358984 csirtg-indicator-3.0b8/csirtg_indicator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      330 2020-06-07 13:23:38.000000 csirtg-indicator-3.0b8/csirtg_indicator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1890 2020-06-07 13:23:38.000000 csirtg-indicator-3.0b8/csirtg_indicator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-06-07 13:23:38.000000 csirtg-indicator-3.0b8/csirtg_indicator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       60 2020-06-07 13:23:38.000000 csirtg-indicator-3.0b8/csirtg_indicator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       69 2020-06-07 13:23:38.000000 csirtg-indicator-3.0b8/csirtg_indicator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       22 2020-06-07 13:23:38.000000 csirtg-indicator-3.0b8/csirtg_indicator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       80 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)      142 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)      317 2020-06-07 13:23:38.362985 csirtg-indicator-3.0b8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1495 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-07 13:23:38.362985 csirtg-indicator-3.0b8/test/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-07 13:23:38.362985 csirtg-indicator-3.0b8/test/format/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/test/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1030 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/test/format/test_bind.py
--rw-r--r--   0 runner    (1001) docker     (116)     1176 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/test/format/test_bindrpz.py
--rw-r--r--   0 runner    (1001) docker     (116)     1169 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/test/format/test_bro.py
--rw-r--r--   0 runner    (1001) docker     (116)      762 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/test/format/test_csv.py
--rw-r--r--   0 runner    (1001) docker     (116)      892 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/test/format/test_json.py
--rw-r--r--   0 runner    (1001) docker     (116)     1071 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/test/format/test_snort.py
--rw-r--r--   0 runner    (1001) docker     (116)      977 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/test/format/test_table.py
--rw-r--r--   0 runner    (1001) docker     (116)      538 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/test/test_asns.py
--rw-r--r--   0 runner    (1001) docker     (116)      298 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/test/test_confidence.py
--rw-r--r--   0 runner    (1001) docker     (116)      889 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/test/test_email.py
--rw-r--r--   0 runner    (1001) docker     (116)     2062 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/test/test_fqdn.py
--rw-r--r--   0 runner    (1001) docker     (116)      429 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/test/test_geo.py
--rw-r--r--   0 runner    (1001) docker     (116)     3027 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/test/test_indicator.py
--rw-r--r--   0 runner    (1001) docker     (116)     2137 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/test/test_ipv4.py
--rw-r--r--   0 runner    (1001) docker     (116)     1017 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/test/test_ipv6.py
--rw-r--r--   0 runner    (1001) docker     (116)      493 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/test/test_message.py
--rw-r--r--   0 runner    (1001) docker     (116)     2464 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/test/test_urls.py
--rw-r--r--   0 runner    (1001) docker     (116)    68611 2020-06-07 13:23:31.000000 csirtg-indicator-3.0b8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-12 17:59:11.482434 csirtg-indicator-3.0b9/
+-rw-r--r--   0 runner    (1001) docker     (116)      662 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (116)    16725 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      313 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)      330 2020-06-12 17:59:11.482434 csirtg-indicator-3.0b9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      500 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-12 17:59:11.482434 csirtg-indicator-3.0b9/csirtg_indicator/
+-rw-r--r--   0 runner    (1001) docker     (116)     5979 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/csirtg_indicator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      497 2020-06-12 17:59:11.482434 csirtg-indicator-3.0b9/csirtg_indicator/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-12 17:59:11.478434 csirtg-indicator-3.0b9/csirtg_indicator/constants/
+-rw-r--r--   0 runner    (1001) docker     (116)      703 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/csirtg_indicator/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      942 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/csirtg_indicator/constants/fields.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1228 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/csirtg_indicator/constants/networks.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-12 17:59:11.478434 csirtg-indicator-3.0b9/csirtg_indicator/feed/
+-rw-r--r--   0 runner    (1001) docker     (116)      972 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/csirtg_indicator/feed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      964 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/csirtg_indicator/feed/fqdn.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1034 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/csirtg_indicator/feed/ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (116)      645 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/csirtg_indicator/feed/ipv6.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-12 17:59:11.478434 csirtg-indicator-3.0b9/csirtg_indicator/format/
+-rw-r--r--   0 runner    (1001) docker     (116)      620 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/csirtg_indicator/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      774 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/csirtg_indicator/format/bind.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1531 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/csirtg_indicator/format/bindrpz.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1636 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/csirtg_indicator/format/bro.py
+-rw-r--r--   0 runner    (1001) docker     (116)      646 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/csirtg_indicator/format/csv.py
+-rw-r--r--   0 runner    (1001) docker     (116)      671 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/csirtg_indicator/format/gexf.py
+-rw-r--r--   0 runner    (1001) docker     (116)      566 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/csirtg_indicator/format/json.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2079 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/csirtg_indicator/format/snort.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1093 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/csirtg_indicator/format/table.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-12 17:59:11.478434 csirtg-indicator-3.0b9/csirtg_indicator/utils/
+-rw-r--r--   0 runner    (1001) docker     (116)     3085 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/csirtg_indicator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      698 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/csirtg_indicator/utils/confidence.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1196 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/csirtg_indicator/utils/fqdn.py
+-rw-r--r--   0 runner    (1001) docker     (116)      942 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/csirtg_indicator/utils/ip.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-12 17:59:11.482434 csirtg-indicator-3.0b9/csirtg_indicator/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/csirtg_indicator/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      520 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/csirtg_indicator/wrappers/cif.py
+-rw-r--r--   0 runner    (1001) docker     (116)      480 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/csirtg_indicator/wrappers/csirtg.py
+-rw-r--r--   0 runner    (1001) docker     (116)      958 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/csirtg_indicator/wrappers/dns.py
+-rw-r--r--   0 runner    (1001) docker     (116)      599 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/csirtg_indicator/wrappers/farsight.py
+-rw-r--r--   0 runner    (1001) docker     (116)      788 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/csirtg_indicator/wrappers/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (116)      619 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/csirtg_indicator/wrappers/geo.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1715 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/csirtg_indicator/wrappers/itypes.py
+-rw-r--r--   0 runner    (1001) docker     (116)      205 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/csirtg_indicator/wrappers/peers.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3320 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/csirtg_indicator/wrappers/properties.py
+-rw-r--r--   0 runner    (1001) docker     (116)      906 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/csirtg_indicator/wrappers/spamhaus.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-12 17:59:11.478434 csirtg-indicator-3.0b9/csirtg_indicator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      330 2020-06-12 17:59:11.000000 csirtg-indicator-3.0b9/csirtg_indicator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1890 2020-06-12 17:59:11.000000 csirtg-indicator-3.0b9/csirtg_indicator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-06-12 17:59:11.000000 csirtg-indicator-3.0b9/csirtg_indicator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       60 2020-06-12 17:59:11.000000 csirtg-indicator-3.0b9/csirtg_indicator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       69 2020-06-12 17:59:11.000000 csirtg-indicator-3.0b9/csirtg_indicator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       22 2020-06-12 17:59:11.000000 csirtg-indicator-3.0b9/csirtg_indicator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       80 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      142 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      317 2020-06-12 17:59:11.482434 csirtg-indicator-3.0b9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1495 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-12 17:59:11.482434 csirtg-indicator-3.0b9/test/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-12 17:59:11.482434 csirtg-indicator-3.0b9/test/format/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/test/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1030 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/test/format/test_bind.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1176 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/test/format/test_bindrpz.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1169 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/test/format/test_bro.py
+-rw-r--r--   0 runner    (1001) docker     (116)      762 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/test/format/test_csv.py
+-rw-r--r--   0 runner    (1001) docker     (116)      892 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/test/format/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1071 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/test/format/test_snort.py
+-rw-r--r--   0 runner    (1001) docker     (116)      977 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/test/format/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (116)      538 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/test/test_asns.py
+-rw-r--r--   0 runner    (1001) docker     (116)      298 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/test/test_confidence.py
+-rw-r--r--   0 runner    (1001) docker     (116)      889 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/test/test_email.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2062 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/test/test_fqdn.py
+-rw-r--r--   0 runner    (1001) docker     (116)      429 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/test/test_geo.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3027 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/test/test_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2137 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/test/test_ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1017 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/test/test_ipv6.py
+-rw-r--r--   0 runner    (1001) docker     (116)      493 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/test/test_message.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2464 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/test/test_urls.py
+-rw-r--r--   0 runner    (1001) docker     (116)    68611 2020-06-12 17:58:58.000000 csirtg-indicator-3.0b9/versioneer.py
```

### Comparing `csirtg-indicator-3.0b8/.coveragerc` & `csirtg-indicator-3.0b9/.coveragerc`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/LICENSE` & `csirtg-indicator-3.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/csirtg_indicator/__init__.py` & `csirtg-indicator-3.0b9/csirtg_indicator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             setattr(self, k, kwargs.get(k, None))
 
         self.confidence = kwargs.get('confidence', None)
         self.count = kwargs.get('count', 1)
         self.uuid = kwargs.get('uuid', str(uuid.uuid4()))
         self.group = kwargs.get('group', 'everyone')
         self.tlp = kwargs.get('tlp', 'AMBER')
-        self.asn_desc = None
+        self.asn_desc = kwargs.get('asn_desc')
 
         # incoming id
         self.iid = kwargs.get('iid')
 
         # outgoing id (if any)
         self.oid = kwargs.get('oid')
```

### Comparing `csirtg-indicator-3.0b8/csirtg_indicator/constants/__init__.py` & `csirtg-indicator-3.0b9/csirtg_indicator/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/csirtg_indicator/constants/fields.py` & `csirtg-indicator-3.0b9/csirtg_indicator/constants/fields.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/csirtg_indicator/constants/networks.py` & `csirtg-indicator-3.0b9/csirtg_indicator/constants/networks.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/csirtg_indicator/feed/__init__.py` & `csirtg-indicator-3.0b9/csirtg_indicator/feed/__init__.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/csirtg_indicator/feed/fqdn.py` & `csirtg-indicator-3.0b9/csirtg_indicator/feed/fqdn.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/csirtg_indicator/feed/ipv4.py` & `csirtg-indicator-3.0b9/csirtg_indicator/feed/ipv4.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/csirtg_indicator/feed/ipv6.py` & `csirtg-indicator-3.0b9/csirtg_indicator/feed/ipv6.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/csirtg_indicator/format/__init__.py` & `csirtg-indicator-3.0b9/csirtg_indicator/format/__init__.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/csirtg_indicator/format/bind.py` & `csirtg-indicator-3.0b9/csirtg_indicator/format/bind.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/csirtg_indicator/format/bindrpz.py` & `csirtg-indicator-3.0b9/csirtg_indicator/format/bindrpz.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/csirtg_indicator/format/bro.py` & `csirtg-indicator-3.0b9/csirtg_indicator/format/bro.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/csirtg_indicator/format/csv.py` & `csirtg-indicator-3.0b9/csirtg_indicator/format/csv.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/csirtg_indicator/format/gexf.py` & `csirtg-indicator-3.0b9/csirtg_indicator/format/gexf.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/csirtg_indicator/format/json.py` & `csirtg-indicator-3.0b9/csirtg_indicator/format/json.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/csirtg_indicator/format/snort.py` & `csirtg-indicator-3.0b9/csirtg_indicator/format/snort.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/csirtg_indicator/format/table.py` & `csirtg-indicator-3.0b9/csirtg_indicator/format/table.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/csirtg_indicator/utils/__init__.py` & `csirtg-indicator-3.0b9/csirtg_indicator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/csirtg_indicator/utils/confidence.py` & `csirtg-indicator-3.0b9/csirtg_indicator/utils/confidence.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/csirtg_indicator/utils/fqdn.py` & `csirtg-indicator-3.0b9/csirtg_indicator/utils/fqdn.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/csirtg_indicator/utils/ip.py` & `csirtg-indicator-3.0b9/csirtg_indicator/utils/ip.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/csirtg_indicator/wrappers/cif.py` & `csirtg-indicator-3.0b9/csirtg_indicator/wrappers/cif.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/csirtg_indicator/wrappers/dns.py` & `csirtg-indicator-3.0b9/csirtg_indicator/wrappers/dns.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/csirtg_indicator/wrappers/farsight.py` & `csirtg-indicator-3.0b9/csirtg_indicator/wrappers/farsight.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/csirtg_indicator/wrappers/formatter.py` & `csirtg-indicator-3.0b9/csirtg_indicator/wrappers/formatter.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/csirtg_indicator/wrappers/geo.py` & `csirtg-indicator-3.0b9/csirtg_indicator/wrappers/geo.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/csirtg_indicator/wrappers/itypes.py` & `csirtg-indicator-3.0b9/csirtg_indicator/wrappers/itypes.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/csirtg_indicator/wrappers/properties.py` & `csirtg-indicator-3.0b9/csirtg_indicator/wrappers/properties.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/csirtg_indicator/wrappers/spamhaus.py` & `csirtg-indicator-3.0b9/csirtg_indicator/wrappers/spamhaus.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/csirtg_indicator.egg-info/SOURCES.txt` & `csirtg-indicator-3.0b9/csirtg_indicator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/setup.py` & `csirtg-indicator-3.0b9/setup.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/test/format/test_bind.py` & `csirtg-indicator-3.0b9/test/format/test_bind.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/test/format/test_bindrpz.py` & `csirtg-indicator-3.0b9/test/format/test_bindrpz.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/test/format/test_bro.py` & `csirtg-indicator-3.0b9/test/format/test_bro.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/test/format/test_csv.py` & `csirtg-indicator-3.0b9/test/format/test_csv.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/test/format/test_json.py` & `csirtg-indicator-3.0b9/test/format/test_json.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/test/format/test_snort.py` & `csirtg-indicator-3.0b9/test/format/test_snort.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/test/format/test_table.py` & `csirtg-indicator-3.0b9/test/format/test_table.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/test/test_asns.py` & `csirtg-indicator-3.0b9/test/test_asns.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/test/test_email.py` & `csirtg-indicator-3.0b9/test/test_email.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/test/test_fqdn.py` & `csirtg-indicator-3.0b9/test/test_fqdn.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/test/test_indicator.py` & `csirtg-indicator-3.0b9/test/test_indicator.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/test/test_ipv4.py` & `csirtg-indicator-3.0b9/test/test_ipv4.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/test/test_ipv6.py` & `csirtg-indicator-3.0b9/test/test_ipv6.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/test/test_urls.py` & `csirtg-indicator-3.0b9/test/test_urls.py`

 * *Files identical despite different names*

### Comparing `csirtg-indicator-3.0b8/versioneer.py` & `csirtg-indicator-3.0b9/versioneer.py`

 * *Files identical despite different names*

