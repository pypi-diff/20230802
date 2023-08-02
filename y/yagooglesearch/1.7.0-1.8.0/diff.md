# Comparing `tmp/yagooglesearch-1.7.0.tar.gz` & `tmp/yagooglesearch-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yagooglesearch-1.7.0.tar", last modified: Sat Jun 10 20:22:24 2023, max compression
+gzip compressed data, was "yagooglesearch-1.8.0.tar", last modified: Wed Aug  2 01:50:07 2023, max compression
```

## Comparing `yagooglesearch-1.7.0.tar` & `yagooglesearch-1.8.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 brennon   (1000) brennon   (1000)        0 2023-06-10 20:22:24.020382 yagooglesearch-1.7.0/
--rw-rw-r--   0 brennon   (1000) brennon   (1000)     1515 2021-08-25 20:22:21.000000 yagooglesearch-1.7.0/LICENSE
--rw-rw-r--   0 brennon   (1000) brennon   (1000)    10959 2023-06-10 20:22:24.020382 yagooglesearch-1.7.0/PKG-INFO
--rw-rw-r--   0 brennon   (1000) brennon   (1000)    10494 2023-06-10 19:53:41.000000 yagooglesearch-1.7.0/README.md
--rw-rw-r--   0 brennon   (1000) brennon   (1000)       38 2023-06-10 20:22:24.020382 yagooglesearch-1.7.0/setup.cfg
--rw-rw-r--   0 brennon   (1000) brennon   (1000)      827 2023-06-10 20:20:26.000000 yagooglesearch-1.7.0/setup.py
-drwxrwxr-x   0 brennon   (1000) brennon   (1000)        0 2023-06-10 20:22:24.020382 yagooglesearch-1.7.0/yagooglesearch/
--rw-rw-r--   0 brennon   (1000) brennon   (1000)    24042 2023-06-10 19:53:41.000000 yagooglesearch-1.7.0/yagooglesearch/__init__.py
--rw-rw-r--   0 brennon   (1000) brennon   (1000)    94251 2021-08-23 21:04:38.000000 yagooglesearch-1.7.0/yagooglesearch/user_agents.txt
-drwxrwxr-x   0 brennon   (1000) brennon   (1000)        0 2023-06-10 20:22:24.020382 yagooglesearch-1.7.0/yagooglesearch.egg-info/
--rw-rw-r--   0 brennon   (1000) brennon   (1000)    10959 2023-06-10 20:22:24.000000 yagooglesearch-1.7.0/yagooglesearch.egg-info/PKG-INFO
--rw-rw-r--   0 brennon   (1000) brennon   (1000)      273 2023-06-10 20:22:24.000000 yagooglesearch-1.7.0/yagooglesearch.egg-info/SOURCES.txt
--rw-rw-r--   0 brennon   (1000) brennon   (1000)        1 2023-06-10 20:22:24.000000 yagooglesearch-1.7.0/yagooglesearch.egg-info/dependency_links.txt
--rw-rw-r--   0 brennon   (1000) brennon   (1000)       55 2023-06-10 20:22:24.000000 yagooglesearch-1.7.0/yagooglesearch.egg-info/requires.txt
--rw-rw-r--   0 brennon   (1000) brennon   (1000)       15 2023-06-10 20:22:24.000000 yagooglesearch-1.7.0/yagooglesearch.egg-info/top_level.txt
+drwxrwxr-x   0 brennon   (1000) brennon   (1000)        0 2023-08-02 01:50:07.168615 yagooglesearch-1.8.0/
+-rw-rw-r--   0 brennon   (1000) brennon   (1000)     1515 2021-08-25 20:22:21.000000 yagooglesearch-1.8.0/LICENSE
+-rw-rw-r--   0 brennon   (1000) brennon   (1000)    10959 2023-08-02 01:50:07.168615 yagooglesearch-1.8.0/PKG-INFO
+-rw-rw-r--   0 brennon   (1000) brennon   (1000)    10494 2023-08-01 18:50:43.000000 yagooglesearch-1.8.0/README.md
+-rw-rw-r--   0 brennon   (1000) brennon   (1000)       38 2023-08-02 01:50:07.168615 yagooglesearch-1.8.0/setup.cfg
+-rw-rw-r--   0 brennon   (1000) brennon   (1000)      827 2023-08-02 01:48:53.000000 yagooglesearch-1.8.0/setup.py
+drwxrwxr-x   0 brennon   (1000) brennon   (1000)        0 2023-08-02 01:50:07.168615 yagooglesearch-1.8.0/yagooglesearch/
+-rw-rw-r--   0 brennon   (1000) brennon   (1000)    25143 2023-08-02 01:48:53.000000 yagooglesearch-1.8.0/yagooglesearch/__init__.py
+-rw-rw-r--   0 brennon   (1000) brennon   (1000)    94251 2021-08-23 21:04:38.000000 yagooglesearch-1.8.0/yagooglesearch/user_agents.txt
+drwxrwxr-x   0 brennon   (1000) brennon   (1000)        0 2023-08-02 01:50:07.168615 yagooglesearch-1.8.0/yagooglesearch.egg-info/
+-rw-rw-r--   0 brennon   (1000) brennon   (1000)    10959 2023-08-02 01:50:07.000000 yagooglesearch-1.8.0/yagooglesearch.egg-info/PKG-INFO
+-rw-rw-r--   0 brennon   (1000) brennon   (1000)      273 2023-08-02 01:50:07.000000 yagooglesearch-1.8.0/yagooglesearch.egg-info/SOURCES.txt
+-rw-rw-r--   0 brennon   (1000) brennon   (1000)        1 2023-08-02 01:50:07.000000 yagooglesearch-1.8.0/yagooglesearch.egg-info/dependency_links.txt
+-rw-rw-r--   0 brennon   (1000) brennon   (1000)       55 2023-08-02 01:50:07.000000 yagooglesearch-1.8.0/yagooglesearch.egg-info/requires.txt
+-rw-rw-r--   0 brennon   (1000) brennon   (1000)       15 2023-08-02 01:50:07.000000 yagooglesearch-1.8.0/yagooglesearch.egg-info/top_level.txt
```

### Comparing `yagooglesearch-1.7.0/LICENSE` & `yagooglesearch-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yagooglesearch-1.7.0/PKG-INFO` & `yagooglesearch-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yagooglesearch
-Version: 1.7.0
+Version: 1.8.0
 Summary: A Python library for executing intelligent, realistic-looking, and tunable Google searches.
 Home-page: https://github.com/opsdisk/yagooglesearch
 Author: Brennon Thomas
 Author-email: info@opsdisk.com
 License: BSD 3-Clause "New" or "Revised" License
 Keywords: python google search googlesearch
 Platform: UNKNOWN
```

### Comparing `yagooglesearch-1.7.0/README.md` & `yagooglesearch-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `yagooglesearch-1.7.0/setup.py` & `yagooglesearch-1.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yagooglesearch",
-    version="1.7.0",
+    version="1.8.0",
     author="Brennon Thomas",
     author_email="info@opsdisk.com",
     description="A Python library for executing intelligent, realistic-looking, and tunable Google searches.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/opsdisk/yagooglesearch",
     packages=setuptools.find_packages(),
```

### Comparing `yagooglesearch-1.7.0/yagooglesearch/__init__.py` & `yagooglesearch-1.8.0/yagooglesearch/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Third party Python libraries.
 from bs4 import BeautifulSoup
 import requests
 
 # Custom Python libraries.
 
-__version__ = "1.7.0"
+__version__ = "1.8.0"
 
 # Logging
 ROOT_LOGGER = logging.getLogger("yagooglesearch")
 # ISO 8601 datetime format by default.
 LOG_FORMATTER = logging.Formatter("%(asctime)s [%(threadName)-12.12s] [%(levelname)s] %(message)s")
 
 # Setup file logging.
@@ -34,21 +34,33 @@
 # Load the list of valid user agents from the install folder.  The search order is:
 # 1) user_agents.txt
 # 2) default USER_AGENT
 install_folder = os.path.abspath(os.path.split(__file__)[0])
 
 try:
     user_agents_file = os.path.join(install_folder, "user_agents.txt")
-    with open(user_agents_file) as fh:
+    with open(user_agents_file, "r") as fh:
         user_agents_list = [_.strip() for _ in fh.readlines()]
 
 except Exception:
     user_agents_list = [USER_AGENT]
 
 
+# Load the list of result languages.  Compiled by viewing the source code at https://www.google.com/advanced_search for
+# the supported languages.
+try:
+    result_languages_file = os.path.join(install_folder, "result_languages.txt")
+    with open(result_languages_file, "r") as fh:
+        result_languages_list = [_.strip().split("=")[0] for _ in fh.readlines()]
+
+except Exception as e:
+    print(f"There was an issue loading the result languages file.  Exception: {e}")
+    result_languages_list = []
+
+
 def get_tbs(from_date, to_date):
     """Helper function to format the tbs parameter dates.  Note that verbatim mode also uses the &tbs= parameter, but
     this function is just for customized search periods.
 
     :param datetime.date from_date: Python date object, e.g. datetime.date(2021, 1, 1)
     :param datetime.date to_date: Python date object, e.g. datetime.date(2021, 6, 1)
 
@@ -65,15 +77,16 @@
 
 
 class SearchClient:
     def __init__(
         self,
         query,
         tld="com",
-        lang="en",
+        lang_html_ui="en",
+        lang_result="lang_en",
         tbs="0",
         safe="off",
         start=0,
         num=100,
         country="",
         extra_params=None,
         max_search_result_urls_to_return=100,
@@ -88,15 +101,16 @@
         verbose_output=False,
         google_exemption=None,
     ):
         """
         SearchClient
         :param str query: Query string.  Must NOT be url-encoded.
         :param str tld: Top level domain.
-        :param str lang: Language.
+        :param str lang_html_ui: HTML User Interface language.
+        :param str lang_result: Search result language.
         :param str tbs: Verbatim search or time limits (e.g., "qdr:h" => last hour, "qdr:d" => last 24 hours, "qdr:m"
             => last month).
         :param str safe: Safe search.
         :param int start: First page of results to retrieve.
         :param int num: Max number of results to pull back per page.  Capped at 100 by Google.
         :param str country: Country or region to focus the search on.  Similar to changing the TLD, but does not yield
             exactly the same results.  Only Google knows why...
@@ -123,15 +137,16 @@
 
         :rtype: List of str
         :return: List of URLs found or list of {"rank", "title", "description", "url"}
         """
 
         self.query = urllib.parse.quote_plus(query)
         self.tld = tld
-        self.lang = lang
+        self.lang_html_ui = lang_html_ui
+        self.lang_result = lang_result.lower()
         self.tbs = tbs
         self.safe = safe
         self.start = start
         self.num = num
         self.country = country
         self.extra_params = extra_params
         self.max_search_result_urls_to_return = max_search_result_urls_to_return
@@ -146,14 +161,21 @@
         self.verbose_output = verbose_output
         self.google_exemption = google_exemption
 
         # Assign log level.
         ROOT_LOGGER.setLevel((6 - self.verbosity) * 10)
 
         # Argument checks.
+        if self.lang_result not in result_languages_list:
+            ROOT_LOGGER.error(
+                f"{self.lang_result} is not a valid language result.  See {result_languages_file} for the list of valid "
+                'languages.  Setting lang_result to "lang_en".'
+            )
+            self.lang_result = "lang_en"
+
         if self.num > 100:
             ROOT_LOGGER.warning("The largest value allowed by Google for num is 100.  Setting num to 100.")
             self.num = 100
 
         # Populate cookies with GOOGLE_ABUSE_EXEMPTION if it is provided.  Otherwise, initialize cookies to None.
         # It will be updated with each request in get_page().
         if self.google_exemption:
@@ -167,14 +189,15 @@
             "cr",
             "hl",
             "num",
             "q",
             "safe",
             "start",
             "tbs",
+            "lr",
         )
 
         # Default user agent, unless instructed by the user to change it.
         if not user_agent:
             self.user_agent = self.assign_random_user_agent()
 
         # Update the URLs with the initial SearchClient attributes.
@@ -211,36 +234,36 @@
         """Update search URLs being used."""
 
         # URL templates to make Google searches.
         self.url_home = f"https://www.google.{self.tld}/"
 
         # First search requesting the default 10 search results.
         self.url_search = (
-            f"https://www.google.{self.tld}/search?hl={self.lang}&"
+            f"https://www.google.{self.tld}/search?hl={self.lang_html_ui}&lr={self.lang_result}&"
             f"q={self.query}&btnG=Google+Search&tbs={self.tbs}&safe={self.safe}&"
             f"cr={self.country}&filter=0"
         )
 
         # Subsequent searches starting at &start= and retrieving 10 search results at a time.
         self.url_next_page = (
-            f"https://www.google.{self.tld}/search?hl={self.lang}&"
+            f"https://www.google.{self.tld}/search?hl={self.lang_html_ui}&lr={self.lang_result}&"
             f"q={self.query}&start={self.start}&tbs={self.tbs}&safe={self.safe}&"
             f"cr={self.country}&filter=0"
         )
 
         # First search requesting more than the default 10 search results.
         self.url_search_num = (
-            f"https://www.google.{self.tld}/search?hl={self.lang}&"
+            f"https://www.google.{self.tld}/search?hl={self.lang_html_ui}&lr={self.lang_result}&"
             f"q={self.query}&num={self.num}&btnG=Google+Search&tbs={self.tbs}&"
             f"safe={self.safe}&cr={self.country}&filter=0"
         )
 
         # Subsequent searches starting at &start= and retrieving &num= search results at a time.
         self.url_next_page_num = (
-            f"https://www.google.{self.tld}/search?hl={self.lang}&"
+            f"https://www.google.{self.tld}/search?hl={self.lang_html_ui}&lr={self.lang_result}&"
             f"q={self.query}&start={self.start}&num={self.num}&tbs={self.tbs}&"
             f"safe={self.safe}&cr={self.country}&filter=0"
         )
 
     def assign_random_user_agent(self):
         """Assign a random user agent string.
 
@@ -454,18 +477,16 @@
             else:
                 if self.num == 10:
                     url = self.url_search
                 else:
                     url = self.url_search_num
 
             # Append extra GET parameters to the URL.  This is done on every iteration because we're rebuilding the
-            # entire URL at the end of this loop.
+            # entire URL at the end of this loop.  The keys and values are not URL encoded.
             for key, value in self.extra_params.items():
-                key = urllib.parse.quote_plus(key)
-                value = urllib.parse.quote_plus(value)
                 url += f"&{key}={value}"
 
             # Request Google search results.
             html = self.get_page(url)
 
             # HTTP 429 message returned from get_page() function, add "HTTP_429_DETECTED" to the set and return to the
             # calling script.
```

### Comparing `yagooglesearch-1.7.0/yagooglesearch/user_agents.txt` & `yagooglesearch-1.8.0/yagooglesearch/user_agents.txt`

 * *Files identical despite different names*

### Comparing `yagooglesearch-1.7.0/yagooglesearch.egg-info/PKG-INFO` & `yagooglesearch-1.8.0/yagooglesearch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yagooglesearch
-Version: 1.7.0
+Version: 1.8.0
 Summary: A Python library for executing intelligent, realistic-looking, and tunable Google searches.
 Home-page: https://github.com/opsdisk/yagooglesearch
 Author: Brennon Thomas
 Author-email: info@opsdisk.com
 License: BSD 3-Clause "New" or "Revised" License
 Keywords: python google search googlesearch
 Platform: UNKNOWN
```

