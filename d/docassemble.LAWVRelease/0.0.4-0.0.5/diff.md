# Comparing `tmp/docassemble.LAWVRelease-0.0.4.tar.gz` & `tmp/docassemble.LAWVRelease-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docassemble.LAWVRelease-0.0.4.tar", last modified: Wed Aug  2 14:00:17 2023, max compression
+gzip compressed data, was "docassemble.LAWVRelease-0.0.5.tar", last modified: Wed Aug  2 14:02:25 2023, max compression
```

## Comparing `docassemble.LAWVRelease-0.0.4.tar` & `docassemble.LAWVRelease-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2023-08-02 14:00:17.581851 docassemble.LAWVRelease-0.0.4/
--rw-r--r--   0 www-data    (33) www-data    (33)     1087 2023-08-02 14:00:16.000000 docassemble.LAWVRelease-0.0.4/LICENSE
--rw-r--r--   0 www-data    (33) www-data    (33)       18 2023-08-02 14:00:16.000000 docassemble.LAWVRelease-0.0.4/MANIFEST.in
--rw-r--r--   0 www-data    (33) www-data    (33)      412 2023-08-02 14:00:17.581851 docassemble.LAWVRelease-0.0.4/PKG-INFO
--rw-r--r--   0 www-data    (33) www-data    (33)      103 2023-08-02 14:00:16.000000 docassemble.LAWVRelease-0.0.4/README.md
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2023-08-02 14:00:17.573851 docassemble.LAWVRelease-0.0.4/docassemble/
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2023-08-02 14:00:17.577851 docassemble.LAWVRelease-0.0.4/docassemble/LAWVRelease/
--rw-r--r--   0 www-data    (33) www-data    (33)       22 2023-08-02 14:00:16.000000 docassemble.LAWVRelease-0.0.4/docassemble/LAWVRelease/__init__.py
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2023-08-02 14:00:17.573851 docassemble.LAWVRelease-0.0.4/docassemble/LAWVRelease/data/
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2023-08-02 14:00:17.577851 docassemble.LAWVRelease-0.0.4/docassemble/LAWVRelease/data/questions/
--rw-r--r--   0 www-data    (33) www-data    (33)     5834 2023-01-06 17:49:45.000000 docassemble.LAWVRelease-0.0.4/docassemble/LAWVRelease/data/questions/lawv_release.yml
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2023-08-02 14:00:17.577851 docassemble.LAWVRelease-0.0.4/docassemble/LAWVRelease/data/sources/
--rw-r--r--   0 www-data    (33) www-data    (33)      134 2023-08-02 14:00:16.000000 docassemble.LAWVRelease-0.0.4/docassemble/LAWVRelease/data/sources/README.md
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2023-08-02 14:00:17.577851 docassemble.LAWVRelease-0.0.4/docassemble/LAWVRelease/data/static/
--rw-r--r--   0 www-data    (33) www-data    (33)      105 2023-08-02 14:00:16.000000 docassemble.LAWVRelease-0.0.4/docassemble/LAWVRelease/data/static/README.md
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2023-08-02 14:00:17.577851 docassemble.LAWVRelease-0.0.4/docassemble/LAWVRelease/data/templates/
--rw-r--r--   0 www-data    (33) www-data    (33)      102 2023-08-02 14:00:16.000000 docassemble.LAWVRelease-0.0.4/docassemble/LAWVRelease/data/templates/README.md
--rw-r--r--   0 www-data    (33) www-data    (33)   467785 2023-01-06 19:56:36.000000 docassemble.LAWVRelease-0.0.4/docassemble/LAWVRelease/data/templates/lawv_release.pdf
--rw-r--r--   0 www-data    (33) www-data    (33)       57 2023-08-02 14:00:16.000000 docassemble.LAWVRelease-0.0.4/docassemble/__init__.py
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2023-08-02 14:00:17.577851 docassemble.LAWVRelease-0.0.4/docassemble.LAWVRelease.egg-info/
--rw-r--r--   0 www-data    (33) www-data    (33)      412 2023-08-02 14:00:17.000000 docassemble.LAWVRelease-0.0.4/docassemble.LAWVRelease.egg-info/PKG-INFO
--rw-r--r--   0 www-data    (33) www-data    (33)      652 2023-08-02 14:00:17.000000 docassemble.LAWVRelease-0.0.4/docassemble.LAWVRelease.egg-info/SOURCES.txt
--rw-r--r--   0 www-data    (33) www-data    (33)        1 2023-08-02 14:00:17.000000 docassemble.LAWVRelease-0.0.4/docassemble.LAWVRelease.egg-info/dependency_links.txt
--rw-r--r--   0 www-data    (33) www-data    (33)       12 2023-08-02 14:00:17.000000 docassemble.LAWVRelease-0.0.4/docassemble.LAWVRelease.egg-info/namespace_packages.txt
--rw-r--r--   0 www-data    (33) www-data    (33)        1 2023-08-02 14:00:17.000000 docassemble.LAWVRelease-0.0.4/docassemble.LAWVRelease.egg-info/not-zip-safe
--rw-r--r--   0 www-data    (33) www-data    (33)       12 2023-08-02 14:00:17.000000 docassemble.LAWVRelease-0.0.4/docassemble.LAWVRelease.egg-info/top_level.txt
--rw-r--r--   0 www-data    (33) www-data    (33)       79 2023-08-02 14:00:17.581851 docassemble.LAWVRelease-0.0.4/setup.cfg
--rw-r--r--   0 www-data    (33) www-data    (33)     2468 2023-08-02 14:00:16.000000 docassemble.LAWVRelease-0.0.4/setup.py
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2023-08-02 14:02:25.023707 docassemble.LAWVRelease-0.0.5/
+-rw-r--r--   0 www-data    (33) www-data    (33)     1087 2023-08-02 14:02:16.000000 docassemble.LAWVRelease-0.0.5/LICENSE
+-rw-r--r--   0 www-data    (33) www-data    (33)       18 2023-08-02 14:02:16.000000 docassemble.LAWVRelease-0.0.5/MANIFEST.in
+-rw-r--r--   0 www-data    (33) www-data    (33)      412 2023-08-02 14:02:25.023707 docassemble.LAWVRelease-0.0.5/PKG-INFO
+-rw-r--r--   0 www-data    (33) www-data    (33)      103 2023-08-02 14:02:16.000000 docassemble.LAWVRelease-0.0.5/README.md
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2023-08-02 14:02:25.019707 docassemble.LAWVRelease-0.0.5/docassemble/
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2023-08-02 14:02:25.019707 docassemble.LAWVRelease-0.0.5/docassemble/LAWVRelease/
+-rw-r--r--   0 www-data    (33) www-data    (33)       22 2023-08-02 14:02:16.000000 docassemble.LAWVRelease-0.0.5/docassemble/LAWVRelease/__init__.py
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2023-08-02 14:02:25.015707 docassemble.LAWVRelease-0.0.5/docassemble/LAWVRelease/data/
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2023-08-02 14:02:25.019707 docassemble.LAWVRelease-0.0.5/docassemble/LAWVRelease/data/questions/
+-rw-r--r--   0 www-data    (33) www-data    (33)     5843 2023-08-02 14:01:41.000000 docassemble.LAWVRelease-0.0.5/docassemble/LAWVRelease/data/questions/lawv_release.yml
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2023-08-02 14:02:25.019707 docassemble.LAWVRelease-0.0.5/docassemble/LAWVRelease/data/sources/
+-rw-r--r--   0 www-data    (33) www-data    (33)      134 2023-08-02 14:02:16.000000 docassemble.LAWVRelease-0.0.5/docassemble/LAWVRelease/data/sources/README.md
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2023-08-02 14:02:25.019707 docassemble.LAWVRelease-0.0.5/docassemble/LAWVRelease/data/static/
+-rw-r--r--   0 www-data    (33) www-data    (33)      105 2023-08-02 14:02:16.000000 docassemble.LAWVRelease-0.0.5/docassemble/LAWVRelease/data/static/README.md
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2023-08-02 14:02:25.019707 docassemble.LAWVRelease-0.0.5/docassemble/LAWVRelease/data/templates/
+-rw-r--r--   0 www-data    (33) www-data    (33)      102 2023-08-02 14:02:16.000000 docassemble.LAWVRelease-0.0.5/docassemble/LAWVRelease/data/templates/README.md
+-rw-r--r--   0 www-data    (33) www-data    (33)   467785 2023-01-06 19:56:36.000000 docassemble.LAWVRelease-0.0.5/docassemble/LAWVRelease/data/templates/lawv_release.pdf
+-rw-r--r--   0 www-data    (33) www-data    (33)       57 2023-08-02 14:02:16.000000 docassemble.LAWVRelease-0.0.5/docassemble/__init__.py
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2023-08-02 14:02:25.019707 docassemble.LAWVRelease-0.0.5/docassemble.LAWVRelease.egg-info/
+-rw-r--r--   0 www-data    (33) www-data    (33)      412 2023-08-02 14:02:24.000000 docassemble.LAWVRelease-0.0.5/docassemble.LAWVRelease.egg-info/PKG-INFO
+-rw-r--r--   0 www-data    (33) www-data    (33)      652 2023-08-02 14:02:24.000000 docassemble.LAWVRelease-0.0.5/docassemble.LAWVRelease.egg-info/SOURCES.txt
+-rw-r--r--   0 www-data    (33) www-data    (33)        1 2023-08-02 14:02:24.000000 docassemble.LAWVRelease-0.0.5/docassemble.LAWVRelease.egg-info/dependency_links.txt
+-rw-r--r--   0 www-data    (33) www-data    (33)       12 2023-08-02 14:02:24.000000 docassemble.LAWVRelease-0.0.5/docassemble.LAWVRelease.egg-info/namespace_packages.txt
+-rw-r--r--   0 www-data    (33) www-data    (33)        1 2023-08-02 14:02:24.000000 docassemble.LAWVRelease-0.0.5/docassemble.LAWVRelease.egg-info/not-zip-safe
+-rw-r--r--   0 www-data    (33) www-data    (33)       12 2023-08-02 14:02:24.000000 docassemble.LAWVRelease-0.0.5/docassemble.LAWVRelease.egg-info/top_level.txt
+-rw-r--r--   0 www-data    (33) www-data    (33)       79 2023-08-02 14:02:25.023707 docassemble.LAWVRelease-0.0.5/setup.cfg
+-rw-r--r--   0 www-data    (33) www-data    (33)     2468 2023-08-02 14:02:16.000000 docassemble.LAWVRelease-0.0.5/setup.py
```

### Comparing `docassemble.LAWVRelease-0.0.4/LICENSE` & `docassemble.LAWVRelease-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `docassemble.LAWVRelease-0.0.4/docassemble/LAWVRelease/data/questions/lawv_release.yml` & `docassemble.LAWVRelease-0.0.5/docassemble/LAWVRelease/data/questions/lawv_release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   description: |
     This interview allows advocates to generate and email
     a release of information to a client and receive a signed
     copy back.
   authors:
     - name: Dane W. Henry, Esq.
       organization: Legal Aid of West Virginia, Inc.
-  revision_date: 2020-12-04
+  revision_date: 2023-08-02
 ---
 objects:
   - a: Individual
   - c: Individual
   - endpoint: DADict
 ---
 mandatory: True
@@ -117,15 +117,15 @@
   Email Sent - Done for now
 subquestion: |
   An email has been sent to ${ c.email } for them to 
   review the terms and sign.  Once signed, a copy will
   be sent to your email: ${ a.email }
 action buttons:
   - label: Leave
-    action: https://www.lawv.net
+    action: https://legalaidwv.org/
     color: warning
     icon: sign-out-alt
 need:
   - attorney_setup
 ---
 ga id: releaseComplete
 event: final_screen
@@ -137,15 +137,15 @@
   
   A copy will be sent to your email: ${ c.email }.
   % else:
   There was a problem sending the e-mail.
   % endif
 action buttons:
   - label: Exit
-    action: https://www.lawv.net
+    action: https://legalaidwv.org/
     color: danger
     icon: sign-out-alt
 ---
 code: |
   client_emailed = send_email(to=c,attachments=lawv_release,template=see_attached)
 ---
 code: |
@@ -155,15 +155,15 @@
 event: challenge_fail
 question: |
   It appears you encountered a problem
 subquestion: |  
   Reason: ${ failure_reason }  
 action buttons:
   - label: Exit
-    action: https://www.lawv.net
+    action: https://legalaidwv.org/
     color: danger
     icon: sign-out-alt
 ---
 template: notification
 subject: |
   A document is awaiting your signature.
 content: |
```

### Comparing `docassemble.LAWVRelease-0.0.4/docassemble/LAWVRelease/data/templates/lawv_release.pdf` & `docassemble.LAWVRelease-0.0.5/docassemble/LAWVRelease/data/templates/lawv_release.pdf`

 * *Files identical despite different names*

### Comparing `docassemble.LAWVRelease-0.0.4/docassemble.LAWVRelease.egg-info/SOURCES.txt` & `docassemble.LAWVRelease-0.0.5/docassemble.LAWVRelease.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docassemble.LAWVRelease-0.0.4/setup.py` & `docassemble.LAWVRelease-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                         break
                 if bad_name:
                     continue
                 out.setdefault(package, []).append(prefix+name)
     return out
 
 setup(name='docassemble.LAWVRelease',
-      version='0.0.4',
+      version='0.0.5',
       description=('A docassemble extension.'),
       long_description='# docassemble.LAWVRelease\n\nA docassemble extension.\n\n## Author\n\nSystem Administrator, dhenry@lawv.net\n\n',
       long_description_content_type='text/markdown',
       author='System Administrator',
       author_email='dhenry@lawv.net',
       license='The MIT License (MIT)',
       url='https://docassemble.org',
```

