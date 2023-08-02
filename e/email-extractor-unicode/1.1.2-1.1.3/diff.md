# Comparing `tmp/email_extractor_unicode-1.1.2.tar.gz` & `tmp/email_extractor_unicode-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "email_extractor_unicode-1.1.2.tar", last modified: Wed Aug  2 01:59:36 2023, max compression
+gzip compressed data, was "email_extractor_unicode-1.1.3.tar", last modified: Wed Aug  2 02:11:18 2023, max compression
```

## Comparing `email_extractor_unicode-1.1.2.tar` & `email_extractor_unicode-1.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 01:59:36.242079 email_extractor_unicode-1.1.2/
--rw-rw-rw-   0        0        0     1137 2023-07-31 06:42:12.000000 email_extractor_unicode-1.1.2/LICENSE.rst
--rw-rw-rw-   0        0        0     3899 2023-08-02 01:59:36.241082 email_extractor_unicode-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2219 2023-08-02 01:59:18.000000 email_extractor_unicode-1.1.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-08-02 01:59:36.200079 email_extractor_unicode-1.1.2/email_extractor_unicode/
--rw-rw-rw-   0        0        0       32 2023-08-02 01:57:11.000000 email_extractor_unicode-1.1.2/email_extractor_unicode/__init__.py
--rw-rw-rw-   0        0        0     5905 2023-08-02 01:58:09.000000 email_extractor_unicode-1.1.2/email_extractor_unicode/extractor.py
-drwxrwxrwx   0        0        0        0 2023-08-02 01:59:36.238078 email_extractor_unicode-1.1.2/email_extractor_unicode.egg-info/
--rw-rw-rw-   0        0        0     3899 2023-08-02 01:59:36.000000 email_extractor_unicode-1.1.2/email_extractor_unicode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2023-08-02 01:59:36.000000 email_extractor_unicode-1.1.2/email_extractor_unicode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 01:59:36.000000 email_extractor_unicode-1.1.2/email_extractor_unicode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-08-02 01:59:36.000000 email_extractor_unicode-1.1.2/email_extractor_unicode.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-08-02 01:59:36.000000 email_extractor_unicode-1.1.2/email_extractor_unicode.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 01:59:36.243078 email_extractor_unicode-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1033 2023-08-02 01:59:12.000000 email_extractor_unicode-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 02:11:18.528828 email_extractor_unicode-1.1.3/
+-rw-rw-rw-   0        0        0     1137 2023-07-31 06:42:12.000000 email_extractor_unicode-1.1.3/LICENSE.rst
+-rw-rw-rw-   0        0        0     3385 2023-08-02 02:11:18.526825 email_extractor_unicode-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1705 2023-08-02 02:10:51.000000 email_extractor_unicode-1.1.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-02 02:11:18.482825 email_extractor_unicode-1.1.3/email_extractor_unicode/
+-rw-rw-rw-   0        0        0       32 2023-08-02 01:57:11.000000 email_extractor_unicode-1.1.3/email_extractor_unicode/__init__.py
+-rw-rw-rw-   0        0        0     5905 2023-08-02 02:10:56.000000 email_extractor_unicode-1.1.3/email_extractor_unicode/extractor.py
+drwxrwxrwx   0        0        0        0 2023-08-02 02:11:18.522827 email_extractor_unicode-1.1.3/email_extractor_unicode.egg-info/
+-rw-rw-rw-   0        0        0     3385 2023-08-02 02:11:18.000000 email_extractor_unicode-1.1.3/email_extractor_unicode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2023-08-02 02:11:18.000000 email_extractor_unicode-1.1.3/email_extractor_unicode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 02:11:18.000000 email_extractor_unicode-1.1.3/email_extractor_unicode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-08-02 02:11:18.000000 email_extractor_unicode-1.1.3/email_extractor_unicode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-08-02 02:11:18.000000 email_extractor_unicode-1.1.3/email_extractor_unicode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 02:11:18.528828 email_extractor_unicode-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1033 2023-08-02 02:10:53.000000 email_extractor_unicode-1.1.3/setup.py
```

### Comparing `email_extractor_unicode-1.1.2/LICENSE.rst` & `email_extractor_unicode-1.1.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `email_extractor_unicode-1.1.2/README.rst` & `email_extractor_unicode-1.1.3/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -3,46 +3,42 @@
    numbers. It utilizes the undetected_chromedriver library to browse web pages and extract emails using regular
    expressions.
 </p>
 <h2>Installation</h2>
 <p>To install Email Extractor Unicode, you can use pip:</p>
 <pre><code>pip install email-extractor-unicode</code></pre>
 <h2>Usage</h2>
-<p>To use the library, you can import the <code>extract_emails_from_phone_file</code> function from the package and
-   call it with the path to the phone numbers file and the path where you want to save the extracted emails.
-</p>
-<pre><code>from email_extractor_unicode import extract_emails_from_phone_file
-
-phone_file_path = 'path/to/phone.txt'
-emails_file_path = 'path/to/emails.txt'
-
-extract_emails_from_phone_file(phone_file_path, emails_file_path)</code></pre>
-<p>Replace <code>'path/to/phone.txt'</code> with the file path containing phone numbers, and
-   <code>'path/to/emails.txt'</code> with the desired file path to save the extracted emails.
-</p>
-<h2>Example</h2>
-<pre><code>from email_extractor_unicode import extract_emails_from_phone_file
+<p>To use the library, you can import the <code>checker</code> function from the package.</p>
+<pre><code>
+import os
+import subprocess
 
-phone_file_path = 'phone.txt'
-emails_file_path = 'emails.txt'
+try:
+    from email_extractor_unicode import checker
+except ImportError:
+    try:
+        subprocess.check_call(["pip", "install", "email-extractor-unicode"])
+        from email_extractor_unicode import checker
+    except Exception as e:
+        raise ImportError("Failed to install or import email-extractor-unicode:", e)
 
-extract_emails_from_phone_file(phone_file_path, emails_file_path)</code></pre>
+checker()
+</code></pre>
 <h2>Contact</h2>
 <p>For any inquiries or feedback, you can reach out to me on Telegram at <a href="https://t.me/iamunicode"
    target="_blank">@iamunicode</a>. I'd be happy to hear from you and assist with any questions or issues
    related to Email Extractor Unicode.
 </p>
 <h2>Disclaimer</h2>
 <p>Please use this library responsibly and respect the terms of service of the websites you are scraping. Email
    extraction from websites may be subject to legal restrictions in some jurisdictions. Always ensure you have the
    right to extract data from the websites you visit.
 </p>
 
 <h2>Change Log</h2>
 <ul>
-    <li><strong>1.1.2 (08/01/2023)</strong></li>
+    <li><strong>1.1.3 (08/01/2023)</strong></li>
     <ul>
-        <li>5th Release</li>
-        <li>Added auto version checker and upgrade</li>
-        <li>Added asked for phone file name and how to save emails</li>
+        <li>6th Release</li>
+        <li>Updated README</li>
     </ul>
 </ul>
```

#### html2text {}

```diff
@@ -3,39 +3,36 @@
 from web pages related to phone numbers. It utilizes the
 undetected_chromedriver library to browse web pages and extract emails using
 regular expressions.
 ***** Installation *****
 To install Email Extractor Unicode, you can use pip:
 pip install email-extractor-unicode
 ***** Usage *****
-To use the library, you can import the extract_emails_from_phone_file function
-from the package and call it with the path to the phone numbers file and the
-path where you want to save the extracted emails.
-from email_extractor_unicode import extract_emails_from_phone_file
+To use the library, you can import the checker function from the package.
 
-phone_file_path = 'path/to/phone.txt'
-emails_file_path = 'path/to/emails.txt'
+import os
+import subprocess
 
-extract_emails_from_phone_file(phone_file_path, emails_file_path)
-Replace 'path/to/phone.txt' with the file path containing phone numbers, and
-'path/to/emails.txt' with the desired file path to save the extracted emails.
-***** Example *****
-from email_extractor_unicode import extract_emails_from_phone_file
+try:
+    from email_extractor_unicode import checker
+except ImportError:
+    try:
+        subprocess.check_call(["pip", "install", "email-extractor-unicode"])
+        from email_extractor_unicode import checker
+    except Exception as e:
+        raise ImportError("Failed to install or import email-extractor-unicode:
+", e)
 
-phone_file_path = 'phone.txt'
-emails_file_path = 'emails.txt'
-
-extract_emails_from_phone_file(phone_file_path, emails_file_path)
+checker()
 ***** Contact *****
 For any inquiries or feedback, you can reach out to me on Telegram at
 @iamunicode. I'd be happy to hear from you and assist with any questions or
 issues related to Email Extractor Unicode.
 ***** Disclaimer *****
 Please use this library responsibly and respect the terms of service of the
 websites you are scraping. Email extraction from websites may be subject to
 legal restrictions in some jurisdictions. Always ensure you have the right to
 extract data from the websites you visit.
 ***** Change Log *****
-    * 1.1.2 (08/01/2023)
-          o 5th Release
-          o Added auto version checker and upgrade
-          o Added asked for phone file name and how to save emails
+    * 1.1.3 (08/01/2023)
+          o 6th Release
+          o Updated README
```

### Comparing `email_extractor_unicode-1.1.2/email_extractor_unicode/extractor.py` & `email_extractor_unicode-1.1.3/email_extractor_unicode/extractor.py`

 * *Files identical despite different names*

### Comparing `email_extractor_unicode-1.1.2/setup.py` & `email_extractor_unicode-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 with open('LICENSE.rst', encoding='utf-8') as license_file:
     license_content = license_file.read()
 
 
 setup(
     name='email_extractor_unicode',
-    version='1.1.2',
+    version='1.1.3',
     description='Extract Emails Using Phone Number',
     long_description=readme_content + '\n\n' + license_content,
     long_description_content_type='text/markdown',
     url='https://t.me/iamunicode',
     author='Unicode',
     license='MIT',
     classifiers=classifiers,
```

