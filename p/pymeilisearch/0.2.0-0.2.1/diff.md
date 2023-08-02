# Comparing `tmp/pymeilisearch-0.2.0.tar.gz` & `tmp/pymeilisearch-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymeilisearch-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pymeilisearch-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pymeilisearch-0.2.0.tar` & `pymeilisearch-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1089 2023-07-27 14:02:37.528799 pymeilisearch-0.2.0/LICENSE
--rw-r--r--   0        0        0     4870 2023-07-27 14:02:37.528799 pymeilisearch-0.2.0/README.rst
--rw-r--r--   0        0        0     2114 2023-07-27 14:02:37.528799 pymeilisearch-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      317 2023-07-27 14:02:37.528799 pymeilisearch-0.2.0/src/ansys/tools/meilisearch/__init__.py
--rw-r--r--   0        0        0      167 2023-07-27 14:02:37.528799 pymeilisearch-0.2.0/src/ansys/tools/meilisearch/__main__.py
--rw-r--r--   0        0        0     4082 2023-07-27 14:02:37.528799 pymeilisearch-0.2.0/src/ansys/tools/meilisearch/all_doc_indexer.py
--rw-r--r--   0        0        0     3374 2023-07-27 14:02:37.528799 pymeilisearch-0.2.0/src/ansys/tools/meilisearch/cli.py
--rw-r--r--   0        0        0     3195 2023-07-27 14:02:37.528799 pymeilisearch-0.2.0/src/ansys/tools/meilisearch/client.py
--rw-r--r--   0        0        0     4722 2023-07-27 14:02:37.528799 pymeilisearch-0.2.0/src/ansys/tools/meilisearch/create_indexes.py
--rw-r--r--   0        0        0     5353 2023-07-27 14:02:37.528799 pymeilisearch-0.2.0/src/ansys/tools/meilisearch/get_pages.py
--rw-r--r--   0        0        0     6598 2023-07-27 14:02:37.528799 pymeilisearch-0.2.0/src/ansys/tools/meilisearch/scrapper.py
--rw-r--r--   0        0        0     3283 2023-07-27 14:02:37.528799 pymeilisearch-0.2.0/src/ansys/tools/meilisearch/server.py
--rw-r--r--   0        0        0     3378 2023-07-27 14:02:37.532799 pymeilisearch-0.2.0/src/ansys/tools/meilisearch/templates/__init__.py
--rw-r--r--   0        0        0      412 2023-07-27 14:02:37.532799 pymeilisearch-0.2.0/src/ansys/tools/meilisearch/templates/default.json
--rw-r--r--   0        0        0      597 2023-07-27 14:02:37.532799 pymeilisearch-0.2.0/src/ansys/tools/meilisearch/templates/sphinx_pydata.json
--rw-r--r--   0        0        0     1349 2023-07-27 14:02:37.532799 pymeilisearch-0.2.0/src/ansys/tools/meilisearch/templates/utils.py
--rw-r--r--   0        0        0     3665 2023-07-27 14:02:37.532799 pymeilisearch-0.2.0/src/ansys/tools/meilisearch/utils.py
--rw-r--r--   0        0        0     6725 1970-01-01 00:00:00.000000 pymeilisearch-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-08-02 08:40:22.326230 pymeilisearch-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4870 2023-08-02 08:40:22.326230 pymeilisearch-0.2.1/README.rst
+-rw-r--r--   0        0        0     2114 2023-08-02 08:40:22.326230 pymeilisearch-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      317 2023-08-02 08:40:22.326230 pymeilisearch-0.2.1/src/ansys/tools/meilisearch/__init__.py
+-rw-r--r--   0        0        0      167 2023-08-02 08:40:22.326230 pymeilisearch-0.2.1/src/ansys/tools/meilisearch/__main__.py
+-rw-r--r--   0        0        0     4082 2023-08-02 08:40:22.326230 pymeilisearch-0.2.1/src/ansys/tools/meilisearch/all_doc_indexer.py
+-rw-r--r--   0        0        0     3781 2023-08-02 08:40:22.326230 pymeilisearch-0.2.1/src/ansys/tools/meilisearch/cli.py
+-rw-r--r--   0        0        0     3195 2023-08-02 08:40:22.326230 pymeilisearch-0.2.1/src/ansys/tools/meilisearch/client.py
+-rw-r--r--   0        0        0     5209 2023-08-02 08:40:22.326230 pymeilisearch-0.2.1/src/ansys/tools/meilisearch/create_indexes.py
+-rw-r--r--   0        0        0     5353 2023-08-02 08:40:22.326230 pymeilisearch-0.2.1/src/ansys/tools/meilisearch/get_pages.py
+-rw-r--r--   0        0        0     6890 2023-08-02 08:40:22.326230 pymeilisearch-0.2.1/src/ansys/tools/meilisearch/scrapper.py
+-rw-r--r--   0        0        0     3761 2023-08-02 08:40:22.326230 pymeilisearch-0.2.1/src/ansys/tools/meilisearch/server.py
+-rw-r--r--   0        0        0     3853 2023-08-02 08:40:22.326230 pymeilisearch-0.2.1/src/ansys/tools/meilisearch/templates/__init__.py
+-rw-r--r--   0        0        0      412 2023-08-02 08:40:22.326230 pymeilisearch-0.2.1/src/ansys/tools/meilisearch/templates/default.json
+-rw-r--r--   0        0        0      597 2023-08-02 08:40:22.326230 pymeilisearch-0.2.1/src/ansys/tools/meilisearch/templates/sphinx_pydata.json
+-rw-r--r--   0        0        0     1349 2023-08-02 08:40:22.326230 pymeilisearch-0.2.1/src/ansys/tools/meilisearch/templates/utils.py
+-rw-r--r--   0        0        0     3665 2023-08-02 08:40:22.326230 pymeilisearch-0.2.1/src/ansys/tools/meilisearch/utils.py
+-rw-r--r--   0        0        0     6725 1970-01-01 00:00:00.000000 pymeilisearch-0.2.1/PKG-INFO
```

### Comparing `pymeilisearch-0.2.0/LICENSE` & `pymeilisearch-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymeilisearch-0.2.0/README.rst` & `pymeilisearch-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `pymeilisearch-0.2.0/pyproject.toml` & `pymeilisearch-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "pymeilisearch"
-version = "0.2.0"
+version = "0.2.1"
 description = " A Python library for effortless indexing and searching of documentation using MeiliSearch."
 readme = "README.rst"
 requires-python = ">=3.8,<4"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
@@ -37,15 +37,15 @@
     "pytest-cov==4.1.0",
     "docker==6.1.3",
 ]
 doc = [
     "ansys-sphinx-theme==0.10.0",
     "numpydoc==1.5.0",
     "Sphinx==6.2.1",
-    "sphinx-design==0.4.1",
+    "sphinx-design==0.5.0",
     "sphinx-jinja==2.0.2",
     "sphinx-autoapi==2.1.1",
     "meilisearch==0.28.1",
     "sphinx-copybutton==0.5.2",
     "sphinx-notfound-page==0.8.3",
     "sphinx-jinja==2.0.2",
 ]
```

### Comparing `pymeilisearch-0.2.0/src/ansys/tools/meilisearch/all_doc_indexer.py` & `pymeilisearch-0.2.1/src/ansys/tools/meilisearch/all_doc_indexer.py`

 * *Files identical despite different names*

### Comparing `pymeilisearch-0.2.0/src/ansys/tools/meilisearch/cli.py` & `pymeilisearch-0.2.1/src/ansys/tools/meilisearch/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -34,17 +34,24 @@
 @click.option(
     "--orgs",
     required=False,
     default=[],
     help="GitHub organizations to scrape public URLs from.",
     multiple=True,
 )
+@click.option(
+    "--stop_urls",
+    required=False,
+    default=[],
+    help="The stop urls to stop scraping.",
+    multiple=True,
+)
 @click.argument("source", type=click.Choice(["html", "url", "github"]))
 @click.argument("location")
-def upload(template, index, source, location, cname, port, orgs):
+def upload(template, index, source, location, cname, port, orgs, stop_urls):
     """Upload documents or a website using a template and index.
 
     Parameters
     ----------
     template : str
         Name of the template to use or the path to where the template
         file is located. Available templates are ``sphinx_pydata`` and ``default``.
@@ -59,14 +66,18 @@
         CNAME that hosts the documents. While supplying a CNAME
         is optional, doing so is recommended for scraping documents
         on the local host.
     port : int
         Port that the localhost is connected on.
     orgs : str or list[str]
         One or more GitHub organizations to scrape public GitHub pages from.
+    stop_urls : str or list[str], default: None
+        A list of stop points when scraping URLs. If specified, crawling
+        will stop when encountering any URL containing any of the strings
+        in this list.
 
     Notes
     -----
     Ensure that these environment variables are set:
 
     - ``MEILISEARCH_HOST_URL``: URL for the Meilisearch host
     - ``MEILISEARCH_API_KEY``: API key (admin) for the Meilisearch host
@@ -74,26 +85,26 @@
       (if running in a GitHub CI/CD environment)
     """
 
     if source == "html":
         location = pathlib.Path.cwd() / location
         os.environ["DOCUMENTATION_CNAME"] = cname
         os.environ["DOCUMENTATION_PORT"] = str(port)
-        local_host_scraping(index, template, location, port)
+        local_host_scraping(index, template, location, port, stop_urls)
 
     elif source == "url":
-        scrap_web_page(index, location, template)
+        scrap_web_page(index, location, template, stop_urls)
 
     elif source == "github":
         public_gh_pages_urls = get_public_urls(orgs)
-        if template == "sphinx-pydata":
+        if template == "sphinx_pydata":
             urls = get_sphinx_urls(public_gh_pages_urls)
-            create_sphinx_indexes(urls)
+            create_sphinx_indexes(urls, stop_urls)
         else:
-            create_sphinx_indexes(public_gh_pages_urls)
+            create_sphinx_indexes(public_gh_pages_urls, stop_urls)
 
     else:
         click.echo(f"Invalid source: {source}. Must be 'html', 'url', or 'github'.")
 
 
 @main.command()
 def version():
```

### Comparing `pymeilisearch-0.2.0/src/ansys/tools/meilisearch/client.py` & `pymeilisearch-0.2.1/src/ansys/tools/meilisearch/client.py`

 * *Files identical despite different names*

### Comparing `pymeilisearch-0.2.0/src/ansys/tools/meilisearch/create_indexes.py` & `pymeilisearch-0.2.1/src/ansys/tools/meilisearch/create_indexes.py`

 * *Files 11% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 
     """
     return {repo: url for repo, url in urls.items() if is_sphinx(url)}
 
 
 def create_sphinx_indexes(
     sphinx_urls,
+    stop_urls=None,
     meilisearch_host_url=None,
     meilisearch_api_key=None,
 ):
     """Create an index for each public GitHub page that was generated using Sphinx.
 
     The unique name created for the index (``index_uid``) matches ``<repo>-sphinx-docs``,
     with a ``'-'`` instead of a ``'/'`` in the repository name. For example, the unique
@@ -71,14 +72,18 @@
     The unique name for an index is always lowercase.
 
     Parameters
     ----------
     sphinx_urls : dict
         Dictionary where keys are repository names that use Sphinx and values are
         their URLs.
+    stop_urls : str or list[str], default: None
+        A list of stop points when scraping URLs. If specified, crawling
+        will stop when encountering any URL containing any of the strings
+        in this list.
     meilisearch_host_url : str, default: None
         URL for the Meilisarch host.
     meilisearch_api_key : str, default: None
         API key (admin) for the Meilisearch host.
 
     Notes
     -----
@@ -99,34 +104,40 @@
         if not index_uid in index_uids:
             response = client.client.create_index(index_uid, {"primaryKey": "objectID"})
             document_utils._wait_task(response.task_uid)
         swap_response = client.client.swap_indexes([{"indexes": [temp_index_uid, index_uid]}])
         client.client.index(temp_index_uid).delete()
 
 
-def scrap_web_page(index_uid, url, templates, meilisearch_host_url=None, meilisearch_api_key=None):
+def scrap_web_page(
+    index_uid, url, templates, stop_urls=None, meilisearch_host_url=None, meilisearch_api_key=None
+):
     """
     Scrape a web page and index its content in Meilisearch.
 
     Parameters
     ----------
     index_uid : str
         Unique name to give to the Meilisearch index.
     url : str
         URL of the web page to scrape.
     templates : str or list[str]
         One or more templates to use to know what content is to
         be scraped. Available templates are ``sphinx_pydata`` and ``default``.
+    stop_urls : str or list[str], default: None
+        A list of stop points when scraping URLs. If specified, crawling
+        will stop when encountering any URL containing any of the strings
+        in this list.
     meilisearch_host_url : str, default: None
         URL for the Meilisarch host.
     meilisearch_api_key : str, default: None
         API key (admin) for the Meilisearch host.
     """
     client = MeilisearchClient(meilisearch_host_url, meilisearch_api_key)
     web_scraper = WebScraper(meilisearch_host_url, meilisearch_api_key)
-    web_scraper.scrape_url(url, index_uid, templates)
+    web_scraper.scrape_url(url, index_uid, templates, stop_urls)
     document_utils = MeilisearchUtils(client)
     stats = client.client.get_all_stats()
     index_uids = list(stats["indexes"].keys())
     if index_uid not in index_uids:
         response = client.client.create_index(index_uid, {"primaryKey": "objectID"})
         document_utils._wait_task(response["taskUid"])
```

### Comparing `pymeilisearch-0.2.0/src/ansys/tools/meilisearch/get_pages.py` & `pymeilisearch-0.2.1/src/ansys/tools/meilisearch/get_pages.py`

 * *Files identical despite different names*

### Comparing `pymeilisearch-0.2.0/src/ansys/tools/meilisearch/scrapper.py` & `pymeilisearch-0.2.1/src/ansys/tools/meilisearch/scrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,24 +42,29 @@
         ----------
         url : str
             URL for the web page to scrape.
         template : str
             Template file for rendering.
         index_uid : str
             Unique name of the Meilisearch index.
+        stop_urls : str or list[str], default: None
+            A list of stop points when scraping URLs. If specified, crawling
+            will stop when encountering any URL containing any of the strings
+            in this list.
 
         Returns
         -------
         str
             Name of the temporary configuration file that was created.
         """
         temp_config_file = get_temp_file_name(".json")
         render_template(
             template, url, temp_config_file, index_uid=index_uid, stop_urls_default=stop_urls
         )
+        print(temp_config_file)
         return temp_config_file
 
     def _scrape_url_command(self, temp_config_file):
         """
         Scrape the URL for a web page.
 
         Parameters
@@ -124,15 +129,15 @@
                 raise ValueError(
                     f'URLs must start with "https://" or "http://". Instead, "{url}" was returned.'
                 )
             response = requests.get(url)
             if response.status_code != 200:
                 raise RuntimeError(f'URL "{url}" returned status code {response.status_code}')
 
-    def scrape_url(self, url, index_uid, template=None, verbose=False):
+    def scrape_url(self, url, index_uid, template=None, stop_urls=None, verbose=False):
         """Scrape a URL for a web page using the active Meilisearch host.
 
         This method generates a single unique name for a single URL.
 
         Parameters
         ----------
         url : str
@@ -148,15 +153,15 @@
         -------
         int
             Number of hits from the URL for the web page.
         """
         self._check_url(url)
         template = get_template(url) if template is None else template
 
-        temp_config_file = self._load_and_render_template(url, template, index_uid)
+        temp_config_file = self._load_and_render_template(url, template, index_uid, stop_urls)
         output = self._scrape_url_command(temp_config_file)
 
         n_hits = self._parse_output(output)
         if verbose:
             print(output)
         return n_hits
```

### Comparing `pymeilisearch-0.2.0/src/ansys/tools/meilisearch/server.py` & `pymeilisearch-0.2.1/src/ansys/tools/meilisearch/server.py`

 * *Files 7% similar despite different names*

```diff
@@ -61,56 +61,64 @@
         """
         Wait for the server thread to complete.
         """
         if self.server_thread:
             self.server_thread.join()
 
 
-def scrape_website(index_uid, templates, directory, port):
+def scrape_website(index_uid, templates, directory, port, stop_urls):
     """
     Scrape the website by collecting the URLs of web pages in the specified directory.
 
     Parameters
     ----------
     index_uid : str
         Unique name to assign to the Meilisearch index.
     templates : str, list[str]
         One or more templates to use. Available templates are ``sphinx_pydata``
         and ``default``.
     directory : str
         Directory containing the website.
     port : int
         Port number to serve the website on.
+    stop_urls : str or list[str], default: None
+        A list of stop points when scraping URLs. If specified, crawling
+        will stop when encountering any URL containing any of the strings
+        in this list.
     """
     base_url = f"http://localhost:{port}"
     files = directory.rglob("*.html")
     urls = [f"{base_url}/{file.relative_to(directory).as_posix()}" for file in files]
 
-    scrap_web_page(index_uid, urls, templates)
+    scrap_web_page(index_uid, urls, templates, stop_urls)
 
 
-def local_host_scraping(index_uid, templates, directory, port):
+def local_host_scraping(index_uid, templates, directory, port, stop_urls):
     """
     Perform localhost scraping by serving the directory and scraping its content.
 
     Parameters
     ----------
     index_uid : str
         Unique name to give to the Meilisearch index.
     templates : str, list[str]
         One or more templates to use. Available templates are ``sphinx_pydata``
         and ``default``.
     directory : str
         Directory to serve and scrape.
     port : int
         Port number to listen on.
+    stop_urls : str or list[str], default: None
+        A list of stop points when scraping URLs. If specified, crawling
+        will stop when encountering any URL containing any of the strings
+        in this list.
     """
     # Start serving the website in a separate thread
     website_server = WebsiteServer(directory, port)
     website_server.start_serving()
 
     # Scrape the website
-    scrape_website(index_uid, templates, directory, port)
+    scrape_website(index_uid, templates, directory, port, stop_urls)
 
     # Stop serving the website
     website_server.stop_serving()
     website_server.join()
```

### Comparing `pymeilisearch-0.2.0/src/ansys/tools/meilisearch/templates/__init__.py` & `pymeilisearch-0.2.1/src/ansys/tools/meilisearch/templates/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     path_out : str
         Path to write the rendered template to.
     index_uid : str, default: None
         Unique name for the custom index to use. This unique name is the
         URL without the ``https://``. The default is ``None``, in which
         case the unique name of the first URL specified for the ``urls``
         parameter is used.
-    stop_urls_default : list[str], default: ['_sources', '_downloads', '_static', '_images', '.doctree']
+    stop_urls_default : str or list[str], default: ['_sources', '_downloads', '_static', '_images', '.doctree']
         A list of stop points when scraping URLs. If specified, crawling
         will stop when encountering any URL containing any of the strings
         in this list. The default is ['_sources', '_downloads', '_static', '_images', '.doctree'].
 
     Returns
     -------
     str
@@ -67,38 +67,48 @@
         template_path = DEFAULT_TEMPLATE
     else:
         template_path = pathlib.Path(template)
 
     if not template_path.exists():
         raise FileNotFoundError(f"Unable to locate a template at {template_path}.")
 
+    if isinstance(urls, str):
+        urls = [urls]
+
     if template == "sphinx_pydata":
-        stop_urls = [f"{urls[-1].rstrip('/')}/{segment}" for segment in STOP_SPHINX_URLS]
+        # Check if the first URL contains "localhost"
+        if "localhost" in urls[0]:
+            stop_base_url = urls[0].rsplit("/", 1)[0]
+        else:
+            stop_base_url = urls[-1].rstrip("/")
+
+        # Generate stop_urls without using urljoin
+        stop_urls = [f"{stop_base_url}/{segment}" for segment in STOP_SPHINX_URLS]
+
+        # Check if stop_urls_default is not None and generate stop_urls_default_list
         if stop_urls_default is not None:
+            if isinstance(stop_urls_default, str):
+                stop_urls_default = [stop_urls_default]
+
             stop_urls.extend(
-                f"{urls[-1].rstrip('/')}{stop_url_default}"
-                for stop_url_default in stop_urls_default
+                [f"{stop_base_url}/{stop_url_default}" for stop_url_default in stop_urls_default]
             )
-    else:
-        stop_urls = [stop_urls_default]
 
     template_str = template_path.read_text()
     template = Template(template_str)
 
-    # Ensure urls is a list
-    if isinstance(urls, str):
-        urls = [urls]
-
     # Use the first url as index_uid if none is provided
     if index_uid is None:
         index_uid = urls[0].replace("https://", "")
 
     # Add stop_urls to the url
-
-    start_url = json.dumps(urls)
+    start_urls = [
+        url for url in urls if not any(url.startswith(stop_url) for stop_url in stop_urls)
+    ]
+    start_url = json.dumps(start_urls)
     stop_url = json.dumps(stop_urls)
 
     # Render the template
     rendered_template = template.render(index_uid=index_uid, start_url=start_url, stop_url=stop_url)
 
     # Write the rendered template to a file
     path_out = pathlib.Path(path_out)
```

### Comparing `pymeilisearch-0.2.0/src/ansys/tools/meilisearch/templates/sphinx_pydata.json` & `pymeilisearch-0.2.1/src/ansys/tools/meilisearch/templates/sphinx_pydata.json`

 * *Files identical despite different names*

### Comparing `pymeilisearch-0.2.0/src/ansys/tools/meilisearch/templates/utils.py` & `pymeilisearch-0.2.1/src/ansys/tools/meilisearch/templates/utils.py`

 * *Files identical despite different names*

### Comparing `pymeilisearch-0.2.0/src/ansys/tools/meilisearch/utils.py` & `pymeilisearch-0.2.1/src/ansys/tools/meilisearch/utils.py`

 * *Files identical despite different names*

### Comparing `pymeilisearch-0.2.0/PKG-INFO` & `pymeilisearch-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeilisearch
-Version: 0.2.0
+Version: 0.2.1
 Summary:  A Python library for effortless indexing and searching of documentation using MeiliSearch.
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAnsys Core Team <pyansys.core@ansys.com>
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,15 @@
 Requires-Dist: jinja2>=3.1.2
 Requires-Dist: meilisearch>=0.24.0
 Requires-Dist: click>=8
 Requires-Dist: pymeilisearch-scraper==0.1.1
 Requires-Dist: ansys-sphinx-theme==0.10.0 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
 Requires-Dist: Sphinx==6.2.1 ; extra == "doc"
-Requires-Dist: sphinx-design==0.4.1 ; extra == "doc"
+Requires-Dist: sphinx-design==0.5.0 ; extra == "doc"
 Requires-Dist: sphinx-jinja==2.0.2 ; extra == "doc"
 Requires-Dist: sphinx-autoapi==2.1.1 ; extra == "doc"
 Requires-Dist: meilisearch==0.28.1 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
 Requires-Dist: sphinx-notfound-page==0.8.3 ; extra == "doc"
 Requires-Dist: sphinx-jinja==2.0.2 ; extra == "doc"
 Requires-Dist: pytest==7.4.0 ; extra == "tests"
```

