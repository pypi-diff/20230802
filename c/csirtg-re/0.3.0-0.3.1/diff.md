# Comparing `tmp/csirtg-re-0.3.0.tar.gz` & `tmp/csirtg-re-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csirtg-re-0.3.0.tar", last modified: Fri Feb 10 16:42:35 2023, max compression
+gzip compressed data, was "csirtg-re-0.3.1.tar", last modified: Wed Aug  2 00:49:40 2023, max compression
```

## Comparing `csirtg-re-0.3.0.tar` & `csirtg-re-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-02-10 16:42:35.139738 csirtg-re-0.3.0/
--rw-r--r--   0 wes        (501) staff       (20)      621 2023-01-27 19:08:31.000000 csirtg-re-0.3.0/.coveragerc
--rw-r--r--   0 wes        (501) staff       (20)    16725 2023-01-27 19:08:31.000000 csirtg-re-0.3.0/LICENSE
--rw-r--r--   0 wes        (501) staff       (20)      337 2023-01-27 19:08:31.000000 csirtg-re-0.3.0/MANIFEST.in
--rw-r--r--   0 wes        (501) staff       (20)      287 2023-02-10 16:42:35.139849 csirtg-re-0.3.0/PKG-INFO
--rw-r--r--   0 wes        (501) staff       (20)      183 2023-01-27 19:08:31.000000 csirtg-re-0.3.0/README.md
-drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-02-10 16:42:35.140553 csirtg-re-0.3.0/csirtg_re/
--rw-r--r--   0 wes        (501) staff       (20)     3062 2023-02-10 16:42:09.000000 csirtg-re-0.3.0/csirtg_re/__init__.py
--rw-r--r--   0 wes        (501) staff       (20)      497 2023-02-10 16:42:35.140614 csirtg-re-0.3.0/csirtg_re/_version.py
-drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-02-10 16:42:35.139235 csirtg-re-0.3.0/csirtg_re.egg-info/
--rw-r--r--   0 wes        (501) staff       (20)      287 2023-02-10 16:42:35.000000 csirtg-re-0.3.0/csirtg_re.egg-info/PKG-INFO
--rw-r--r--   0 wes        (501) staff       (20)      344 2023-02-10 16:42:35.000000 csirtg-re-0.3.0/csirtg_re.egg-info/SOURCES.txt
--rw-r--r--   0 wes        (501) staff       (20)        1 2023-02-10 16:42:35.000000 csirtg-re-0.3.0/csirtg_re.egg-info/dependency_links.txt
--rw-r--r--   0 wes        (501) staff       (20)       45 2023-02-10 16:42:35.000000 csirtg-re-0.3.0/csirtg_re.egg-info/entry_points.txt
--rw-r--r--   0 wes        (501) staff       (20)       10 2023-02-10 16:42:35.000000 csirtg-re-0.3.0/csirtg_re.egg-info/top_level.txt
--rw-r--r--   0 wes        (501) staff       (20)       80 2023-02-10 16:42:09.000000 csirtg-re-0.3.0/dev_requirements.txt
--rw-r--r--   0 wes        (501) staff       (20)       13 2023-01-27 19:08:31.000000 csirtg-re-0.3.0/requirements.txt
--rw-r--r--   0 wes        (501) staff       (20)      296 2023-02-10 16:42:35.140322 csirtg-re-0.3.0/setup.cfg
--rw-r--r--   0 wes        (501) staff       (20)     1314 2023-01-27 19:08:31.000000 csirtg-re-0.3.0/setup.py
-drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-02-10 16:42:35.139519 csirtg-re-0.3.0/test/
--rw-r--r--   0 wes        (501) staff       (20)     1125 2023-02-10 16:42:09.000000 csirtg-re-0.3.0/test/test_basics.py
--rw-r--r--   0 wes        (501) staff       (20)    68611 2023-01-27 19:08:31.000000 csirtg-re-0.3.0/versioneer.py
+drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-08-02 00:49:40.532223 csirtg-re-0.3.1/
+-rw-r--r--   0 wes        (501) staff       (20)      621 2023-01-27 19:08:31.000000 csirtg-re-0.3.1/.coveragerc
+-rw-r--r--   0 wes        (501) staff       (20)    16725 2023-01-27 19:08:31.000000 csirtg-re-0.3.1/LICENSE
+-rw-r--r--   0 wes        (501) staff       (20)      337 2023-01-27 19:08:31.000000 csirtg-re-0.3.1/MANIFEST.in
+-rw-r--r--   0 wes        (501) staff       (20)      287 2023-08-02 00:49:40.532269 csirtg-re-0.3.1/PKG-INFO
+-rw-r--r--   0 wes        (501) staff       (20)      183 2023-01-27 19:08:31.000000 csirtg-re-0.3.1/README.md
+drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-08-02 00:49:40.532620 csirtg-re-0.3.1/csirtg_re/
+-rw-r--r--   0 wes        (501) staff       (20)     3059 2023-08-02 00:27:28.000000 csirtg-re-0.3.1/csirtg_re/__init__.py
+-rw-r--r--   0 wes        (501) staff       (20)      497 2023-08-02 00:49:40.532651 csirtg-re-0.3.1/csirtg_re/_version.py
+drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-08-02 00:49:40.532010 csirtg-re-0.3.1/csirtg_re.egg-info/
+-rw-r--r--   0 wes        (501) staff       (20)      287 2023-08-02 00:49:40.000000 csirtg-re-0.3.1/csirtg_re.egg-info/PKG-INFO
+-rw-r--r--   0 wes        (501) staff       (20)      344 2023-08-02 00:49:40.000000 csirtg-re-0.3.1/csirtg_re.egg-info/SOURCES.txt
+-rw-r--r--   0 wes        (501) staff       (20)        1 2023-08-02 00:49:40.000000 csirtg-re-0.3.1/csirtg_re.egg-info/dependency_links.txt
+-rw-r--r--   0 wes        (501) staff       (20)       45 2023-08-02 00:49:40.000000 csirtg-re-0.3.1/csirtg_re.egg-info/entry_points.txt
+-rw-r--r--   0 wes        (501) staff       (20)       10 2023-08-02 00:49:40.000000 csirtg-re-0.3.1/csirtg_re.egg-info/top_level.txt
+-rw-r--r--   0 wes        (501) staff       (20)       80 2023-02-10 16:42:09.000000 csirtg-re-0.3.1/dev_requirements.txt
+-rw-r--r--   0 wes        (501) staff       (20)       13 2023-01-27 19:08:31.000000 csirtg-re-0.3.1/requirements.txt
+-rw-r--r--   0 wes        (501) staff       (20)      296 2023-08-02 00:49:40.532475 csirtg-re-0.3.1/setup.cfg
+-rw-r--r--   0 wes        (501) staff       (20)     1314 2023-01-27 19:08:31.000000 csirtg-re-0.3.1/setup.py
+drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-08-02 00:49:40.532126 csirtg-re-0.3.1/test/
+-rw-r--r--   0 wes        (501) staff       (20)     1228 2023-08-02 00:48:35.000000 csirtg-re-0.3.1/test/test_basics.py
+-rw-r--r--   0 wes        (501) staff       (20)    68611 2023-01-27 19:08:31.000000 csirtg-re-0.3.1/versioneer.py
```

### Comparing `csirtg-re-0.3.0/.coveragerc` & `csirtg-re-0.3.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `csirtg-re-0.3.0/LICENSE` & `csirtg-re-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `csirtg-re-0.3.0/csirtg_re/__init__.py` & `csirtg-re-0.3.1/csirtg_re/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 # http://goo.gl/Cztyn2 -- probably needs more work
 # http://stackoverflow.com/a/26987741/7205341
 # ^((xn--)?(--)?[a-zA-Z0-9-_@]+(-[a-zA-Z0-9]+)*\.)+[a-zA-Z]{2,}(--p1ai)?$
 #RE_FQDN = re.compile('^((?!-))(xn--)?[a-z0-9][a-z0-9-_\.]{0,61}[a-z0-9]{0,1}\.(xn--)?([a-z0-9\-]{1,61}|[a-z0-9-]{1,30}\.[a-z]{2,})$')
 # http://stackoverflow.com/questions/14402407/maximum-length-of-a-domain-name-without-the-http-www-com-parts
 RE_FQDN = re.compile(r'^((?!-))(xn--)?[a-zA-Z0-9][a-zA-Z0-9-_\.]{0,245}[a-zA-Z0-9]{0,1}\.(xn--)?([a-zA-Z0-9\-]{1,61}|[a-zA-Z0-9-]{1,30}\.[a-z]{2,})$')
-RE_URI_SCHEMES = re.compile(r'^(https?|ftp)://')
+RE_URI_SCHEMES = re.compile(r'^(https?|ftp)')
 RE_EMAIL = re.compile(r'^[_a-zA-Z0-9-\!\#\$\%\&\'\*\+\-\/\=\?\^\_\`\{\|\}\~]+(\.[_a-zA-Z0-9-\!\#\$\%\&\'\*\+\-\/\=\?\^\_\`\{\|\}\~]+)*@[a-zA-Z0-9-]+(\.[a-zA-Z0-9-]+)*(\.[a-zA-Z]{2,8})$')
 RE_ASN = re.compile(r'^(AS|as)[0-9]{1,6}$')
 
 RE_HASH = {
     'uuid': re.compile(r'^[0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{12}$'),
     'md5': re.compile(r'^[a-fA-F0-9]{32}$'),
     'sha1': re.compile(r'^[a-fA-F0-9]{40}$'),
```

### Comparing `csirtg-re-0.3.0/setup.py` & `csirtg-re-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `csirtg-re-0.3.0/test/test_basics.py` & `csirtg-re-0.3.1/test/test_basics.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,17 @@
     'a95c530a7af5f492a74499e70578d150': 'md5',
     "http://example.com": "url",
     "https://example.com": "url",
     "1.1.1.0/8": "ipv4",
     "bc1qjm4zu6rcg7a00ws26qr6u08dq35r3sj70yrj2e": "btc",
     "bc1qjm4zu6rcg7a00ws26qr6u08dq35r": "btc",
     "cve-2021-27104": "cve",
-    "WES@barely3am.com": "email"
+    "WES@barely3am.com": "email",
+    "1b2a30776df64fbd7299bd588e21573891dcecbe": "sha1",
+    "https://www.church.com/terms.htm": "url"
 }
 
 
 def test_re():
     for i in INDICATORS:
         assert get(i) == INDICATORS[i]
```

### Comparing `csirtg-re-0.3.0/versioneer.py` & `csirtg-re-0.3.1/versioneer.py`

 * *Files identical despite different names*

