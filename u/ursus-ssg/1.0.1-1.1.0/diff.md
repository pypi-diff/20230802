# Comparing `tmp/ursus_ssg-1.0.1.tar.gz` & `tmp/ursus_ssg-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ursus_ssg-1.0.1.tar", last modified: Tue Mar 21 09:58:11 2023, max compression
+gzip compressed data, was "ursus_ssg-1.1.0.tar", last modified: Wed Aug  2 10:27:46 2023, max compression
```

## Comparing `ursus_ssg-1.0.1.tar` & `ursus_ssg-1.1.0.tar`

### file list

```diff
@@ -1,37 +1,41 @@
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-03-21 09:58:11.614082 ursus_ssg-1.0.1/
--rw-r--r--   0 nicolas    (501) staff       (20)    10588 2023-03-21 09:58:11.612810 ursus_ssg-1.0.1/PKG-INFO
--rw-r--r--   0 nicolas    (501) staff       (20)    10316 2023-03-21 09:54:02.000000 ursus_ssg-1.0.1/README.md
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-03-21 09:58:11.521278 ursus_ssg-1.0.1/bin/
--rwxr-xr-x   0 nicolas    (501) staff       (20)     2405 2023-03-21 09:18:00.000000 ursus_ssg-1.0.1/bin/ursus
--rw-r--r--   0 nicolas    (501) staff       (20)       38 2023-03-21 09:58:11.614615 ursus_ssg-1.0.1/setup.cfg
--rw-r--r--   0 nicolas    (501) staff       (20)     1003 2023-03-21 09:57:29.000000 ursus_ssg-1.0.1/setup.py
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-03-21 09:58:11.533141 ursus_ssg-1.0.1/ursus/
--rw-------   0 nicolas    (501) staff       (20)        0 2023-02-09 19:20:47.000000 ursus_ssg-1.0.1/ursus/__init__.py
--rw-r--r--   0 nicolas    (501) staff       (20)     3485 2023-03-21 09:18:02.000000 ursus_ssg-1.0.1/ursus/config.py
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-03-21 09:58:11.566303 ursus_ssg-1.0.1/ursus/context_processors/
--rw-r--r--   0 nicolas    (501) staff       (20)      876 2023-03-21 09:18:04.000000 ursus_ssg-1.0.1/ursus/context_processors/__init__.py
--rw-------   0 nicolas    (501) staff       (20)     1114 2023-01-27 10:29:38.000000 ursus_ssg-1.0.1/ursus/context_processors/get_entries.py
--rw-r--r--   0 nicolas    (501) staff       (20)     1553 2023-03-21 09:18:06.000000 ursus_ssg-1.0.1/ursus/context_processors/git_date.py
--rw-r--r--   0 nicolas    (501) staff       (20)    12585 2023-03-21 09:18:08.000000 ursus_ssg-1.0.1/ursus/context_processors/markdown.py
--rw-------   0 nicolas    (501) staff       (20)     1203 2023-02-09 19:54:39.000000 ursus_ssg-1.0.1/ursus/context_processors/related.py
--rw-r--r--   0 nicolas    (501) staff       (20)      636 2023-03-21 09:18:09.000000 ursus_ssg-1.0.1/ursus/context_processors/stale.py
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-03-21 09:58:11.570543 ursus_ssg-1.0.1/ursus/generators/
--rw-r--r--   0 nicolas    (501) staff       (20)     1891 2023-03-21 09:18:10.000000 ursus_ssg-1.0.1/ursus/generators/__init__.py
--rw-r--r--   0 nicolas    (501) staff       (20)     2146 2023-03-21 09:18:11.000000 ursus_ssg-1.0.1/ursus/generators/static.py
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-03-21 09:58:11.578700 ursus_ssg-1.0.1/ursus/linters/
--rw-r--r--   0 nicolas    (501) staff       (20)     1824 2023-03-21 09:18:12.000000 ursus_ssg-1.0.1/ursus/linters/__init__.py
--rw-r--r--   0 nicolas    (501) staff       (20)     5304 2023-03-21 09:18:13.000000 ursus_ssg-1.0.1/ursus/linters/markdown.py
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-03-21 09:58:11.592773 ursus_ssg-1.0.1/ursus/renderers/
--rw-------   0 nicolas    (501) staff       (20)      628 2023-02-09 22:09:00.000000 ursus_ssg-1.0.1/ursus/renderers/__init__.py
--rw-r--r--   0 nicolas    (501) staff       (20)     2658 2023-03-21 09:18:14.000000 ursus_ssg-1.0.1/ursus/renderers/image.py
--rw-------   0 nicolas    (501) staff       (20)     9914 2023-03-21 09:17:37.000000 ursus_ssg-1.0.1/ursus/renderers/jinja.py
--rw-r--r--   0 nicolas    (501) staff       (20)     2083 2023-03-21 09:20:43.000000 ursus_ssg-1.0.1/ursus/renderers/lunr.py
--rw-r--r--   0 nicolas    (501) staff       (20)     1049 2023-03-21 09:18:16.000000 ursus_ssg-1.0.1/ursus/renderers/static.py
--rw-r--r--   0 nicolas    (501) staff       (20)    10828 2023-03-21 09:18:18.000000 ursus_ssg-1.0.1/ursus/utils.py
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-03-21 09:58:11.609471 ursus_ssg-1.0.1/ursus_ssg.egg-info/
--rw-r--r--   0 nicolas    (501) staff       (20)    10588 2023-03-21 09:58:11.000000 ursus_ssg-1.0.1/ursus_ssg.egg-info/PKG-INFO
--rw-r--r--   0 nicolas    (501) staff       (20)      730 2023-03-21 09:58:11.000000 ursus_ssg-1.0.1/ursus_ssg.egg-info/SOURCES.txt
--rw-r--r--   0 nicolas    (501) staff       (20)        1 2023-03-21 09:58:11.000000 ursus_ssg-1.0.1/ursus_ssg.egg-info/dependency_links.txt
--rw-r--r--   0 nicolas    (501) staff       (20)        1 2023-03-21 09:19:18.000000 ursus_ssg-1.0.1/ursus_ssg.egg-info/not-zip-safe
--rw-r--r--   0 nicolas    (501) staff       (20)      192 2023-03-21 09:58:11.000000 ursus_ssg-1.0.1/ursus_ssg.egg-info/requires.txt
--rw-r--r--   0 nicolas    (501) staff       (20)        6 2023-03-21 09:58:11.000000 ursus_ssg-1.0.1/ursus_ssg.egg-info/top_level.txt
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-08-02 10:27:46.281055 ursus_ssg-1.1.0/
+-rw-r--r--   0 nicolas    (501) staff       (20)    12463 2023-08-02 10:27:46.280921 ursus_ssg-1.1.0/PKG-INFO
+-rw-r--r--   0 nicolas    (501) staff       (20)    12191 2023-08-02 10:26:53.000000 ursus_ssg-1.1.0/README.md
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-08-02 10:27:46.275459 ursus_ssg-1.1.0/bin/
+-rwxr-xr-x   0 nicolas    (501) staff       (20)     2363 2023-05-24 19:39:22.000000 ursus_ssg-1.1.0/bin/ursus
+-rw-r--r--   0 nicolas    (501) staff       (20)       38 2023-08-02 10:27:46.281098 ursus_ssg-1.1.0/setup.cfg
+-rw-r--r--   0 nicolas    (501) staff       (20)     1294 2023-08-02 08:42:08.000000 ursus_ssg-1.1.0/setup.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-08-02 10:27:46.276339 ursus_ssg-1.1.0/ursus/
+-rw-r--r--   0 nicolas    (501) staff       (20)     1554 2023-05-24 18:21:49.000000 ursus_ssg-1.1.0/ursus/__init__.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     4274 2023-06-28 10:41:08.000000 ursus_ssg-1.1.0/ursus/config.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-08-02 10:27:46.277990 ursus_ssg-1.1.0/ursus/context_processors/
+-rw-r--r--   0 nicolas    (501) staff       (20)     1096 2023-06-25 13:27:40.000000 ursus_ssg-1.1.0/ursus/context_processors/__init__.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     2523 2023-07-17 10:08:25.000000 ursus_ssg-1.1.0/ursus/context_processors/get_entries.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     1609 2023-04-07 09:59:42.000000 ursus_ssg-1.1.0/ursus/context_processors/git_date.py
+-rw-r--r--   0 nicolas    (501) staff       (20)      785 2023-06-23 08:56:06.000000 ursus_ssg-1.1.0/ursus/context_processors/image.py
+-rw-r--r--   0 nicolas    (501) staff       (20)    16385 2023-08-02 08:34:26.000000 ursus_ssg-1.1.0/ursus/context_processors/markdown.py
+-rw-------   0 nicolas    (501) staff       (20)     1203 2023-04-30 06:26:51.000000 ursus_ssg-1.1.0/ursus/context_processors/related.py
+-rw-r--r--   0 nicolas    (501) staff       (20)      636 2023-03-21 09:18:09.000000 ursus_ssg-1.1.0/ursus/context_processors/stale.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-08-02 10:27:46.278260 ursus_ssg-1.1.0/ursus/generators/
+-rw-r--r--   0 nicolas    (501) staff       (20)     1904 2023-07-02 10:01:21.000000 ursus_ssg-1.1.0/ursus/generators/__init__.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     2122 2023-05-02 14:07:06.000000 ursus_ssg-1.1.0/ursus/generators/static.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-08-02 10:27:46.278716 ursus_ssg-1.1.0/ursus/linters/
+-rw-r--r--   0 nicolas    (501) staff       (20)     1169 2023-05-24 17:47:41.000000 ursus_ssg-1.1.0/ursus/linters/__init__.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     1222 2023-04-11 15:59:59.000000 ursus_ssg-1.1.0/ursus/linters/images.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     6742 2023-04-11 14:46:36.000000 ursus_ssg-1.1.0/ursus/linters/markdown.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-08-02 10:27:46.279853 ursus_ssg-1.1.0/ursus/renderers/
+-rw-------   0 nicolas    (501) staff       (20)      628 2023-02-09 22:09:00.000000 ursus_ssg-1.1.0/ursus/renderers/__init__.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     2078 2023-06-23 08:56:07.000000 ursus_ssg-1.1.0/ursus/renderers/image.py
+-rw-r--r--   0 nicolas    (501) staff       (20)    11290 2023-07-16 18:24:21.000000 ursus_ssg-1.1.0/ursus/renderers/jinja.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     2154 2023-05-24 18:29:01.000000 ursus_ssg-1.1.0/ursus/renderers/lunr.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     1043 2023-06-20 10:47:27.000000 ursus_ssg-1.1.0/ursus/renderers/sass.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     1057 2023-04-11 14:46:55.000000 ursus_ssg-1.1.0/ursus/renderers/static.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     1476 2023-05-16 20:18:11.000000 ursus_ssg-1.1.0/ursus/server.py
+-rw-r--r--   0 nicolas    (501) staff       (20)    11661 2023-06-29 08:08:10.000000 ursus_ssg-1.1.0/ursus/utils.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-08-02 10:27:46.280727 ursus_ssg-1.1.0/ursus_ssg.egg-info/
+-rw-r--r--   0 nicolas    (501) staff       (20)    12463 2023-08-02 10:27:46.000000 ursus_ssg-1.1.0/ursus_ssg.egg-info/PKG-INFO
+-rw-r--r--   0 nicolas    (501) staff       (20)      828 2023-08-02 10:27:46.000000 ursus_ssg-1.1.0/ursus_ssg.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)        1 2023-08-02 10:27:46.000000 ursus_ssg-1.1.0/ursus_ssg.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)        1 2023-08-02 08:41:25.000000 ursus_ssg-1.1.0/ursus_ssg.egg-info/not-zip-safe
+-rw-r--r--   0 nicolas    (501) staff       (20)      320 2023-08-02 10:27:46.000000 ursus_ssg-1.1.0/ursus_ssg.egg-info/requires.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)        6 2023-08-02 10:27:46.000000 ursus_ssg-1.1.0/ursus_ssg.egg-info/top_level.txt
```

### Comparing `ursus_ssg-1.0.1/PKG-INFO` & `ursus_ssg-1.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: ursus_ssg
-Version: 1.0.1
+Version: 1.1.0
 Summary: Static site generator
 Home-page: http://github.com/nicbou/ursus
 Author: Nicolas Bouliane
 Author-email: contact@nicolasbouliane.com
 License: MIT
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # Ursus
 
-Ursus is the static site generator used by [All About Berlin](https://allaboutberlin.com). It turns Markdown files and [Jinja](https://jinja.palletsprojects.com/) templates into a static website.
+Ursus is the static site generator used by [All About Berlin](https://allaboutberlin.com) and my [personal website](https://nicolasbouliane.com). It turns Markdown files and [Jinja](https://jinja.palletsprojects.com/) templates into a static website.
+
+It also renders images in different sizes, renders SCSS, minifies JS and generates Lunr.js search indexes.
 
 This project is in active use and development.
 
 ## Setup
 
 ### Installation
 
@@ -23,265 +25,407 @@
 
 ```bash
 pip install ursus-ssg
 ```
 
 ### Getting started
 
-By default, Ursus looks for content in `./content`, and templates in `./templates`. It generates a website under `./output`.
+Call `ursus` to generate a static website. Call `ursus --help` to see the command line options it supports.
+
+By default, Ursus looks for 3 directories, relative to the current directory:
 
-Call `ursus` to build the project. Call `ursus --help` to see the command line options it supports.
+- It looks for content in `./content`
+- It looks for page templates in `./templates`
+- It generates a static website in `./output`
 
-Here is a simple piece of content. Save it under `./content/posts/first-post.md`.
+For example, create a markdown file and save it as `./content/posts/first-post.md`.
 
 ```markdown
 ---
-Title: Hello world!
-Description: This is an example page
-Date_created: 2022-10-10
+title: Hello world!
+description: This is an example page
+date_created: 2022-10-10
 ---
 
 ## Hello beautiful world
 
 *This* is a template. Pretty cool eh?
 ```
 
-Here is a simple template. Save it under `./templates/posts/entry.html.jinja`. 
+Then, create a page template and save it as `./templates/posts/entry.html.jinja`. 
 
 ```
 <!DOCTYPE html>
 <html>
 <head>
     <title>{{ entry.title }}</title>
     <meta name="description" content="{{ entry.description }}">
 </head>
 <body>
     {{ entry.body }}
+
+    Created on {{ entry.date_created }}
 </body>
 </html>
 ```
 
-Call `ursus` to generate this website. It will create `./output/posts/first-post.html`.
+Your project should now look like this:
+
+```
+my-website/ <- You are here
+├─ content/
+│  └─ posts/
+│     └─ first-post.md
+└─ templates/
+   └─ posts/
+      └─ entry.html.jinja
+```
+
+Call `ursus` to generate a statuc website. It will create `./output/posts/first-post.html`.
 
 ### Configuring Ursus
 
-You can configure Ursus by creating a `ursus_config.py` file at the root of your project. When you call `ursus`, it will load this configuration.
+To configure Ursus, create a configuration file.
 
 ```python
 # Example Ursus config file
+# Find all configuration options in `ursus/config.py`.
 from ursus.config import config
 
 config.content_path = Path(__file__).parent / 'blog'
 config.templates_path = Path(__file__).parent / 'templates'
 config.output_path = Path(__file__).parent.parent / 'dist'
 
 config.site_url = 'https://allaboutberlin.com'
 
 config.minify_js = True
 config.minify_css = True
 ```
 
-You can find all configuration options in `ursus/config.py`.
+If you call your configuration file `ursus_config.py`, Ursus loads it automatically.
+
+```
+my-website/
+├─ ursus_config.py
+├─ content/
+└─ templates/
+```
 
-You can give your config a different name, and load it with the `-c` argument:
+You can also load a configuration file with the `-w` argument.
 
 ```bash
-ursus -c path/to/config.py
+ursus -c /path/to/config.py
 ```
 
-## Basic concepts
+### Watching for changes
 
-### Content and Entries
+Ursus can rebuild your website when the content or templates change.
 
-**Content** is what fills your website: text, images, videos, PDFs. A single piece of content is called an **Entry**. The location of the Content is set by `config.content_path`. By default, it's under `./content`.
+```bash
+# Rebuild when content or templates change
+ursus -w
+ursus --watch
+```
 
-Content is usually *rendered* to create a working website. Some content (like Markdown files) is rendered with Templates, and other (like images) is converted to a different file format.
+It can only rebuild the pages that changed. This is much faster, but it does not work perfectly.
 
-### Templates
+```bash
+# Only rebuild the pages that changed
+ursus -wf
+ursus --watch --fast
+```
 
-**Templates** are used to render your Content. They are the theme of your website. The same templates can be applied to different Entries, or even reused for a different website. They are kept in a separate directory.
+### Serving the website
 
-For example, a template can be the HTML that makes up the page around your content: the header, sidebar, and footer.
+Ursus can serve the website it generates. This is useful for testing.
 
-The location of the Templates is set by `config.templates_path`. By default, it's under `./templates`. You can have a different `templates_path` for each Generator.
+```bash
+# Serve the static website on port 80
+ursus -s
+ursus --serve 80
+```
 
-For example:
+This is not meant for production. Use nginx, Caddy or some other static file server for that.
 
-- HTML templates that wrap a nice theme around your Content.
-- Images and other static assets that are part of the website's theme
+## How Ursus works
 
-### Output
+1. **Context processors** generate the context used to render templates. The context is just a big dictionary.
+2. **Renderers** use the context and the templates to render the parts of the final website: pages, thumbnails, static assets, etc.
 
-This is the final static website generated by Ursus.
+### Content
 
-The location of the Output is set by `config.output_path`. By default, it's under `./output`.
+**Content** is what fills your website: text, images, videos, PDFs. Content is usually *rendered* to create a working website. Some content (like Markdown files) is rendered with Templates, and other (like images) is converted to a different file format.
 
-## How Ursus works
+Ursus looks for content in `./content`, unless you change `config.content_path`.
 
-ContextProcessors transform the context, which is a dict with information about each of your Entries. Renderers use the context to know which pages to create, and what content to put in the templates.
+### Entries
 
-In the example above, your context would look like this:
+A single piece of content is called an **Entry**. This can be a single image, a single markdown file, etc.
 
-```
+Each Entry has a **URI**. This is the Entry's unique identifier. The URI is the Entry's path relative to the content directory. For example, the URI of `./content/posts/first-post.md` is `posts/first-post.md`.
+
+### Context
+
+The **Context** contains the information needed to render your website. It's just a big dictionary, and you can put anything in it.
+
+`context['entries']` contains is a dictionary of all your entries. The key is the Entry URI.
+
+**Context processors** each add specific data to the context. For example, `MarkdownProcessor` adds your `.md` content to `context.entries`.
+
+```python
+# Example context
 {
     'entries': {
         'posts/first-post.md': {
             'title': 'Hello world!',
             'description': 'This is an example page',
-            'body': '<h2>Hello beautiful world</h2><p>...'
-        }
+            'date_created': datetime(2022, 10, 10),
+            'body': '<h2>Hello beautiful world</h2><p>...',
+        },
+        'posts/second-post.md': {
+            # ...
+        },
     },
-    'get_entries': function
-    'globals': {},
+    # Context processors can add more things to the context
+    'blog_title': 'Example blog',
+    'site_url': 'https://example.com/blog',
 }
 ```
 
-### Generators
+### Templates
 
-A **Generator** takes your Content and your Templates and produces an Output. It's a recipe to turn your content into a final result. The default **StaticSiteGenerator** generates a static website. You can write your own Generator to output an eBook, a PDF, or anything else.
+**Templates** are used to render your Content. They are the theme of your website. Jinja templates, Javascript, CSS and theme images belong in the templates directory.
+
+Ursus looks for templates in `./templates`, unless you change `config.templates_path`.
+
+### Renderers
 
-#### StaticSiteGenerator
+**Renderers** use the Context and the Templates to generate parts of your static website. For example, `JinjaRenderer` renders Jinja templates, `ImageTransformRenderer` converts and resizes your images, and `StaticAssetRenderer` copies your static assets.
 
-Generates a static website.
+### Output
+
+This is the final static website generated by Ursus. Ursus generates a static website in `./output`, unless you change `config.output_path`.
 
-### Context processors
+The content of the output directory is ready to be served by any static file server.
 
-The context is a big object that is used to render templates.
+## How context processors work
 
-A **ContextProcessor** fills this context object, or transforms its existing contents.
+Context processors transform the context, which is a dict with information about each of your Entries.
 
-For example, the **MarkdownProcessor** generates the entry context out of a markdown file.
+Context processors ignore file and directory names that start with `.` or `_`. For example, `./content/_drafts/hello.md` and `./content/posts/_post-draft.md` are ignored.
 
-Only Entries with matching ContextProcessors are rendered. Entry or directory names that start with `.` or `_` are not rendered. You can use this to create drafts.
+### MarkdownProcessor
 
-#### MarkdownProcessor
+The `MarkdownProcessor` creates context for all `.md` files in `content_path`. The markdown content is in the `body` attribute.
 
-The `MarkdownProcessor` creates context for all `.md` files in `content_path`.
+```python
+{
+    'entries': {
+        'posts/first-post.md': {
+            'title': 'Hello world!',
+            'description': 'This is an example page',
+            'date_created': datetime(2022, 10, 10),
+            'body': '<h2>Hello beautiful world</h2><p>...',
+        },
+        # ...
+    },
+}
+```
 
 It makes a few changes to the default markdown output:
 
-- Lazyload images (`loading=lazy`)
-- Convert images to `<figure>` tags when appropriate
-- Jinja tags (`{{ ... }}` and `{% ... %}`) are rendered as-is. You can use the, to `{% include %}` template parts and `{{ variables }}` in your content.
-- Set the `srcset` to load responsive images from the `image_transforms` config.
 - Put the front matter in the context
-    - `Related_*` keys are replaced by a list of related entry dicts
-    - `Date_` keys are converted to `datetime` objects
+    - `related_*` keys are replaced by a list of related entry dicts
+    - `date_` keys are converted to `datetime` objects
+    - Other attributes are added to the entry object.
+- Use responsive images based on `config.image_transforms` settings.
+- `<img>` are converted to `<figure>` or `<picture>` tags when appropriate.
+- Images are lazy-loaded with the `loading=lazy` attribute.
+- Jinja tags (`{{ ... }}` and `{% ... %}`) are rendered as-is. You can use `{% include %}` and `{{ variables }}` in your content.
 
-#### GetEntriesProcessor
+### GetEntriesProcessor
 
 The `GetEntriesProcessor` adds a `get_entries` method to the context. It's used to get a list of entries of a certain type, and sort it.
 
 ```jinja
-{% set posts = get_entries('posts', sort_by='date_created', reverse=True) %}
+{% set posts = get_entries('posts', filter_by=filter_function, sort_by='date_created', reverse=True) %}
+
+{% for post in posts %}
+...
 ```
 
-### Renderers
+### GitDateProcessor
 
-**Renderer**s create content that make up the Output. In other words, they turn your content files into pages, correctly-sized images, RSS feeds, etc.
+Adds the `date_updated` attribute to all Entries. It uses the file's last commit date.
+
+```python
+{
+    'entries': {
+        'posts/first-post.md': {
+            'date_updated': datetime(2022, 10, 10),
+            # ...
+        },
+        # ...
+    },
+}
+```
 
-#### ImageTransformRenderer
+### ImageProcessor
 
-Renders images in `content_path` with a few changes:
+Adds images and PDFs Entries to the context. Dimensions and image transforms are added to each Entry. Use in combination with `config.image_transforms`.
 
-- Images are compressed and optimized.
-- Images are resized according to the `image_transforms`. The images are shrunk if needed, but never stretched.
+```python
+{
+    'entries': {
+        'images/hello.jpg': {
+            'width': 320,
+            'height': 240,
+            'image_transforms': [
+                {
+                    'is_default': True,
+                    'input_mimetype': 'image/jpeg',
+                    'output_mimetype': 'image/webp',
+                    # ...
+                },
+                # ...
+            ]
+        },
+        # ...
+    },
+}
+```
+
+## How renderers work
+
+Renderers use context and templates to generate parts of the static website.
+
+A **Generator** takes your Content and your Templates and produces an Output. It's a recipe to turn your content into a final result. The default **StaticSiteGenerator** generates a static website. You can write your own Generator to output an eBook, a PDF, or anything else.
+
+### ImageTransformRenderer
+
+Renders images in your content directory.
+
+- Images are converted and resized according to `config.image_transforms`.
 - Files that can't be transformed (PDF to PDF) are copied as-is to the output directory.
 - Images that can't be resized (SVG to anything) are copied as-is to the output directory.
 - Image EXIF data is removed.
 
-This renderer does nothing unless `image_transforms` is set:
+This renderer does nothing unless `config.image_transforms` is set:
+
 ```python
+from ursus.config import config
+
 config.image_transforms = {
-    # ...
-    'image_transforms': {
-        # Default transform used as <img> src
-        # Saved as ./output/path/to/image.jpg
-        '': {
-            'max_size': (3200, 4800),
-        },
-        # Saved as ./output/path/to/image.jpg and .webp
-        'thumbnails': {
-            'exclude': ('*.pdf', '*.svg'),  # glob patterns
-            'max_size': (400, 400),
-            'output_types': ('original', 'webp'),
-        },
-        # Only previews PDF files in specific locations
-        # Saved as ./output/path/to/image.webp and .png
-        'pdfPreviews': {
-            'include': ('documents/*.pdf', 'forms/*.pdf'),  # glob patterns
-            'max_size': (300, 500),
-            'output_types': ('webp', 'png'),
-        }
+    # ./content/images/test.jpg
+    # ---> ./output/images/test.jpg
+    # ./content/images/test.pdf
+    # ---> ./output/images/test.pdf
+    '': {
+        'include': ('images/*', 'documents/*'),
+        'output_types': ('original'),
+    },
+    # ./content/images/test.jpg
+    # ---> ./output/images/content2x/test.jpg
+    # ---> ./output/images/content2x/test.webp
+    'content2x': {
+        'include': ('images/*', 'illustrations/*'),
+        'exclude': ('*.pdf', '*.svg'),
+        'max_size': (800, 1200),
+        'output_types': ('webp', 'original'),
+    },
+    # ./content/documents/test.pdf
+    # ---> ./output/documents/pdfPreviews/test.png
+    # ---> ./output/documents/pdfPreviews/test.webp
+    'pdfPreviews': {
+        'include': 'documents/*',
+        'max_size': (300, 500),
+        'output_types': ('webp', 'png'),
     },
-    # ...
 }
 ```
 
-#### JinjaRenderer
-
-Renders Content into Jinja templates using the context made by ContextProcessors.
+### JinjaRenderer
 
-A Template called `./output/hello-world.html.jinja` will be rendered as `./output/hello-world.html`. The template has access to anything you put in the context, including the `entries` dict, and the `get_entries` method.
+Renders `*.jinja` files in the templates directory.
 
-A Template called `./output/posts/entry.html.jinja` will render all Entries under `./content/posts/*.md` and save them under `./output/posts/*.html`. The template has access to an `entry` variable.
+The output file has the same name and relative path as the template, but the `.jinja` extension is removed.
 
-Only Templates with the `.jinja` extension are rendered. Files or directory names that start with `.` or `_` are not rendered.
+```
+my-website/
+├─ templates/
+│  ├─ contact.html.jinja
+│  ├─ sitemap.xml.jinja
+│  └─ posts/
+│     └─ index.html.jinja
+└─ output/
+   ├─ contact.html
+   ├─ sitemap.xml
+   └─ posts/
+      └─ index.html
+```
 
-Files named `entry.*.jinja` are rendered once for each Entry with the same path. For example, `./templates/posts/entry.html.jinja` will render `./content/posts/hello-world.md`, `./content/posts/foo.md` and `./content/posts/bar.md`. The output path is the entry name with the extension replaced. If `./templates/posts/entry.html.jinja` renders `./templates/posts/hello-world.md`, the output file is `./output/posts/hello-world.html`.
+Files named `entry.*.jinja` will render every entry with the same relative path.
 
-All template files with the `.jinja` extension will be rendered. For example, `./templates/posts/index.html.jinja` will be rendered as `./output/posts/index.html`. Files starting with `_` are ignored.
+```
+my-website/
+├─ content/
+│  └─ posts/
+│     ├─ first-post.md
+│     ├─ second-post.md
+│     └─ _draft.md
+├─ templates/
+│  └─ posts/
+│     └─ entry.html.jinja
+└─ output/
+   └─ posts/
+      ├─ first-post.html
+      └─ second-post.html
+```
 
-The output path is the template name without the `.jinja` extension. For example, `index.html.jinja` will be rendered as `index.html`.
+Files or directory names that start with `.` or `_` are not rendered.
 
-#### StaticAssetRenderer
+```
+my-website/
+├─ content/
+│  └─ posts/
+│     ├─ hello-world.md
+│     ├─ .hidden.md
+│     └─ _drafts
+│        └─ not-rendered.md
+├─ templates/
+│  └─ posts/
+│     └─ entry.html.jinja
+└─ output/
+   └─ posts/
+      └─ hello-world.html
+```
 
-Simply copies static assets (CSS, JS, images, etc.) under `./templates` to the same subdirectory in `./output`. Files starting with `.` are ignored. Files and directories starting with `_` are ignored.
+### StaticAssetRenderer
 
-It uses hard links instead of copying files. It's faster and it saves space.
+Copies all files under `./templates` except `.jinja` files to the same subdirectory in `./output`. Files starting with `.` are ignored. Files and directories starting with `_` are ignored.
 
-## Getting started
+```
+my-website/
+├─ templates/
+│  ├─ _ignored.jpg
+│  ├─ styles.css
+│  ├─ images/
+│  │  └─ hello.png
+│  └─ js/
+│     └─ test.js
+└─ output/
+   ├─ styles.css
+   ├─ images/
+   │  └─ hello.png
+   └─ js/
+      └─ test.js
+```
 
-1. **Create a directory** for your project. This is a sensible structure, because it works automatically with the default configuration:
-    ```
-    example_site/
-    ├── ursus_config.py  # By default, Ursus will use this config file
-    ├── templates/  # By default, Ursus will use this templates directory
-    │   ├── index.html.jinja
-    │   ├── css/
-    │   │   └──style.css
-    │   ├── js/
-    │   │   └──scripts.js
-    │   ├── fonts/
-    │   │   ├── open-sans.svg
-    │   │   ├── open-sans.ttf
-    │   │   └── open-sans.woff
-    │   └── posts/
-    │       ├── index.html.jinja
-    │       └── entry.html.jinja
-    └── content/  # By default, Ursus will use this content directory
-        ├── posts/
-        │   ├── first-post.md
-        │   ├── foo.md
-        │   └── bar.md
-        └── images/
-            └── example.png
-    ```
-2. **Create a config file for your website.** You can copy `ursus/default_config.py`. If you call your config `ursus_config.py` and place it in your project root, it will be loaded automatically. Otherwise you must call ursus with the `-c` argument. If no config is set, Ursus will use the defaults set in `ursus/default_config.py`.
-3. **Call the `ursus` command.**
+It uses hard links instead of copying files, so it does not use extra disk space.
 
-#### Building from Sublime Text
+## How generators work
 
-You can configure Sublime Text to run Ursus when you press Cmd + B:
+Generators bring it all together. A generator takes all of your files, and generates some final product. There is only `StaticSiteGenerator`, which generates a static website. Custom generators could generate a book or a slideshow from the same content and templates.
 
-```json
-// Sublime user settings or project config
-{
-    // ...
-    "build_systems": [{
-        "cmd": ["ursus", "-c", "$project_path/path/to/ursus_config.py"],
-        "name": "Ursus",
-    }],
-    // ...
-}
+## How linters work
 
-```
+Ursus supports linter. They verify the content when `ursus lint` is called. You can find examples in `ursus/linters`.
```

### Comparing `ursus_ssg-1.0.1/README.md` & `ursus_ssg-1.1.0/ursus_ssg.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,23 @@
+Metadata-Version: 2.1
+Name: ursus-ssg
+Version: 1.1.0
+Summary: Static site generator
+Home-page: http://github.com/nicbou/ursus
+Author: Nicolas Bouliane
+Author-email: contact@nicolasbouliane.com
+License: MIT
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+
 # Ursus
 
-Ursus is the static site generator used by [All About Berlin](https://allaboutberlin.com). It turns Markdown files and [Jinja](https://jinja.palletsprojects.com/) templates into a static website.
+Ursus is the static site generator used by [All About Berlin](https://allaboutberlin.com) and my [personal website](https://nicolasbouliane.com). It turns Markdown files and [Jinja](https://jinja.palletsprojects.com/) templates into a static website.
+
+It also renders images in different sizes, renders SCSS, minifies JS and generates Lunr.js search indexes.
 
 This project is in active use and development.
 
 ## Setup
 
 ### Installation
 
@@ -12,265 +25,407 @@
 
 ```bash
 pip install ursus-ssg
 ```
 
 ### Getting started
 
-By default, Ursus looks for content in `./content`, and templates in `./templates`. It generates a website under `./output`.
+Call `ursus` to generate a static website. Call `ursus --help` to see the command line options it supports.
+
+By default, Ursus looks for 3 directories, relative to the current directory:
 
-Call `ursus` to build the project. Call `ursus --help` to see the command line options it supports.
+- It looks for content in `./content`
+- It looks for page templates in `./templates`
+- It generates a static website in `./output`
 
-Here is a simple piece of content. Save it under `./content/posts/first-post.md`.
+For example, create a markdown file and save it as `./content/posts/first-post.md`.
 
 ```markdown
 ---
-Title: Hello world!
-Description: This is an example page
-Date_created: 2022-10-10
+title: Hello world!
+description: This is an example page
+date_created: 2022-10-10
 ---
 
 ## Hello beautiful world
 
 *This* is a template. Pretty cool eh?
 ```
 
-Here is a simple template. Save it under `./templates/posts/entry.html.jinja`. 
+Then, create a page template and save it as `./templates/posts/entry.html.jinja`. 
 
 ```
 <!DOCTYPE html>
 <html>
 <head>
     <title>{{ entry.title }}</title>
     <meta name="description" content="{{ entry.description }}">
 </head>
 <body>
     {{ entry.body }}
+
+    Created on {{ entry.date_created }}
 </body>
 </html>
 ```
 
-Call `ursus` to generate this website. It will create `./output/posts/first-post.html`.
+Your project should now look like this:
+
+```
+my-website/ <- You are here
+├─ content/
+│  └─ posts/
+│     └─ first-post.md
+└─ templates/
+   └─ posts/
+      └─ entry.html.jinja
+```
+
+Call `ursus` to generate a statuc website. It will create `./output/posts/first-post.html`.
 
 ### Configuring Ursus
 
-You can configure Ursus by creating a `ursus_config.py` file at the root of your project. When you call `ursus`, it will load this configuration.
+To configure Ursus, create a configuration file.
 
 ```python
 # Example Ursus config file
+# Find all configuration options in `ursus/config.py`.
 from ursus.config import config
 
 config.content_path = Path(__file__).parent / 'blog'
 config.templates_path = Path(__file__).parent / 'templates'
 config.output_path = Path(__file__).parent.parent / 'dist'
 
 config.site_url = 'https://allaboutberlin.com'
 
 config.minify_js = True
 config.minify_css = True
 ```
 
-You can find all configuration options in `ursus/config.py`.
+If you call your configuration file `ursus_config.py`, Ursus loads it automatically.
+
+```
+my-website/
+├─ ursus_config.py
+├─ content/
+└─ templates/
+```
 
-You can give your config a different name, and load it with the `-c` argument:
+You can also load a configuration file with the `-w` argument.
 
 ```bash
-ursus -c path/to/config.py
+ursus -c /path/to/config.py
 ```
 
-## Basic concepts
+### Watching for changes
 
-### Content and Entries
+Ursus can rebuild your website when the content or templates change.
 
-**Content** is what fills your website: text, images, videos, PDFs. A single piece of content is called an **Entry**. The location of the Content is set by `config.content_path`. By default, it's under `./content`.
+```bash
+# Rebuild when content or templates change
+ursus -w
+ursus --watch
+```
 
-Content is usually *rendered* to create a working website. Some content (like Markdown files) is rendered with Templates, and other (like images) is converted to a different file format.
+It can only rebuild the pages that changed. This is much faster, but it does not work perfectly.
 
-### Templates
+```bash
+# Only rebuild the pages that changed
+ursus -wf
+ursus --watch --fast
+```
 
-**Templates** are used to render your Content. They are the theme of your website. The same templates can be applied to different Entries, or even reused for a different website. They are kept in a separate directory.
+### Serving the website
 
-For example, a template can be the HTML that makes up the page around your content: the header, sidebar, and footer.
+Ursus can serve the website it generates. This is useful for testing.
 
-The location of the Templates is set by `config.templates_path`. By default, it's under `./templates`. You can have a different `templates_path` for each Generator.
+```bash
+# Serve the static website on port 80
+ursus -s
+ursus --serve 80
+```
 
-For example:
+This is not meant for production. Use nginx, Caddy or some other static file server for that.
 
-- HTML templates that wrap a nice theme around your Content.
-- Images and other static assets that are part of the website's theme
+## How Ursus works
 
-### Output
+1. **Context processors** generate the context used to render templates. The context is just a big dictionary.
+2. **Renderers** use the context and the templates to render the parts of the final website: pages, thumbnails, static assets, etc.
 
-This is the final static website generated by Ursus.
+### Content
 
-The location of the Output is set by `config.output_path`. By default, it's under `./output`.
+**Content** is what fills your website: text, images, videos, PDFs. Content is usually *rendered* to create a working website. Some content (like Markdown files) is rendered with Templates, and other (like images) is converted to a different file format.
 
-## How Ursus works
+Ursus looks for content in `./content`, unless you change `config.content_path`.
 
-ContextProcessors transform the context, which is a dict with information about each of your Entries. Renderers use the context to know which pages to create, and what content to put in the templates.
+### Entries
 
-In the example above, your context would look like this:
+A single piece of content is called an **Entry**. This can be a single image, a single markdown file, etc.
 
-```
+Each Entry has a **URI**. This is the Entry's unique identifier. The URI is the Entry's path relative to the content directory. For example, the URI of `./content/posts/first-post.md` is `posts/first-post.md`.
+
+### Context
+
+The **Context** contains the information needed to render your website. It's just a big dictionary, and you can put anything in it.
+
+`context['entries']` contains is a dictionary of all your entries. The key is the Entry URI.
+
+**Context processors** each add specific data to the context. For example, `MarkdownProcessor` adds your `.md` content to `context.entries`.
+
+```python
+# Example context
 {
     'entries': {
         'posts/first-post.md': {
             'title': 'Hello world!',
             'description': 'This is an example page',
-            'body': '<h2>Hello beautiful world</h2><p>...'
-        }
+            'date_created': datetime(2022, 10, 10),
+            'body': '<h2>Hello beautiful world</h2><p>...',
+        },
+        'posts/second-post.md': {
+            # ...
+        },
     },
-    'get_entries': function
-    'globals': {},
+    # Context processors can add more things to the context
+    'blog_title': 'Example blog',
+    'site_url': 'https://example.com/blog',
 }
 ```
 
-### Generators
+### Templates
 
-A **Generator** takes your Content and your Templates and produces an Output. It's a recipe to turn your content into a final result. The default **StaticSiteGenerator** generates a static website. You can write your own Generator to output an eBook, a PDF, or anything else.
+**Templates** are used to render your Content. They are the theme of your website. Jinja templates, Javascript, CSS and theme images belong in the templates directory.
+
+Ursus looks for templates in `./templates`, unless you change `config.templates_path`.
+
+### Renderers
+
+**Renderers** use the Context and the Templates to generate parts of your static website. For example, `JinjaRenderer` renders Jinja templates, `ImageTransformRenderer` converts and resizes your images, and `StaticAssetRenderer` copies your static assets.
 
-#### StaticSiteGenerator
+### Output
 
-Generates a static website.
+This is the final static website generated by Ursus. Ursus generates a static website in `./output`, unless you change `config.output_path`.
 
-### Context processors
+The content of the output directory is ready to be served by any static file server.
 
-The context is a big object that is used to render templates.
+## How context processors work
 
-A **ContextProcessor** fills this context object, or transforms its existing contents.
+Context processors transform the context, which is a dict with information about each of your Entries.
 
-For example, the **MarkdownProcessor** generates the entry context out of a markdown file.
+Context processors ignore file and directory names that start with `.` or `_`. For example, `./content/_drafts/hello.md` and `./content/posts/_post-draft.md` are ignored.
 
-Only Entries with matching ContextProcessors are rendered. Entry or directory names that start with `.` or `_` are not rendered. You can use this to create drafts.
+### MarkdownProcessor
 
-#### MarkdownProcessor
+The `MarkdownProcessor` creates context for all `.md` files in `content_path`. The markdown content is in the `body` attribute.
 
-The `MarkdownProcessor` creates context for all `.md` files in `content_path`.
+```python
+{
+    'entries': {
+        'posts/first-post.md': {
+            'title': 'Hello world!',
+            'description': 'This is an example page',
+            'date_created': datetime(2022, 10, 10),
+            'body': '<h2>Hello beautiful world</h2><p>...',
+        },
+        # ...
+    },
+}
+```
 
 It makes a few changes to the default markdown output:
 
-- Lazyload images (`loading=lazy`)
-- Convert images to `<figure>` tags when appropriate
-- Jinja tags (`{{ ... }}` and `{% ... %}`) are rendered as-is. You can use the, to `{% include %}` template parts and `{{ variables }}` in your content.
-- Set the `srcset` to load responsive images from the `image_transforms` config.
 - Put the front matter in the context
-    - `Related_*` keys are replaced by a list of related entry dicts
-    - `Date_` keys are converted to `datetime` objects
+    - `related_*` keys are replaced by a list of related entry dicts
+    - `date_` keys are converted to `datetime` objects
+    - Other attributes are added to the entry object.
+- Use responsive images based on `config.image_transforms` settings.
+- `<img>` are converted to `<figure>` or `<picture>` tags when appropriate.
+- Images are lazy-loaded with the `loading=lazy` attribute.
+- Jinja tags (`{{ ... }}` and `{% ... %}`) are rendered as-is. You can use `{% include %}` and `{{ variables }}` in your content.
 
-#### GetEntriesProcessor
+### GetEntriesProcessor
 
 The `GetEntriesProcessor` adds a `get_entries` method to the context. It's used to get a list of entries of a certain type, and sort it.
 
 ```jinja
-{% set posts = get_entries('posts', sort_by='date_created', reverse=True) %}
+{% set posts = get_entries('posts', filter_by=filter_function, sort_by='date_created', reverse=True) %}
+
+{% for post in posts %}
+...
 ```
 
-### Renderers
+### GitDateProcessor
+
+Adds the `date_updated` attribute to all Entries. It uses the file's last commit date.
 
-**Renderer**s create content that make up the Output. In other words, they turn your content files into pages, correctly-sized images, RSS feeds, etc.
+```python
+{
+    'entries': {
+        'posts/first-post.md': {
+            'date_updated': datetime(2022, 10, 10),
+            # ...
+        },
+        # ...
+    },
+}
+```
+
+### ImageProcessor
+
+Adds images and PDFs Entries to the context. Dimensions and image transforms are added to each Entry. Use in combination with `config.image_transforms`.
+
+```python
+{
+    'entries': {
+        'images/hello.jpg': {
+            'width': 320,
+            'height': 240,
+            'image_transforms': [
+                {
+                    'is_default': True,
+                    'input_mimetype': 'image/jpeg',
+                    'output_mimetype': 'image/webp',
+                    # ...
+                },
+                # ...
+            ]
+        },
+        # ...
+    },
+}
+```
 
-#### ImageTransformRenderer
+## How renderers work
 
-Renders images in `content_path` with a few changes:
+Renderers use context and templates to generate parts of the static website.
 
-- Images are compressed and optimized.
-- Images are resized according to the `image_transforms`. The images are shrunk if needed, but never stretched.
+A **Generator** takes your Content and your Templates and produces an Output. It's a recipe to turn your content into a final result. The default **StaticSiteGenerator** generates a static website. You can write your own Generator to output an eBook, a PDF, or anything else.
+
+### ImageTransformRenderer
+
+Renders images in your content directory.
+
+- Images are converted and resized according to `config.image_transforms`.
 - Files that can't be transformed (PDF to PDF) are copied as-is to the output directory.
 - Images that can't be resized (SVG to anything) are copied as-is to the output directory.
 - Image EXIF data is removed.
 
-This renderer does nothing unless `image_transforms` is set:
+This renderer does nothing unless `config.image_transforms` is set:
+
 ```python
+from ursus.config import config
+
 config.image_transforms = {
-    # ...
-    'image_transforms': {
-        # Default transform used as <img> src
-        # Saved as ./output/path/to/image.jpg
-        '': {
-            'max_size': (3200, 4800),
-        },
-        # Saved as ./output/path/to/image.jpg and .webp
-        'thumbnails': {
-            'exclude': ('*.pdf', '*.svg'),  # glob patterns
-            'max_size': (400, 400),
-            'output_types': ('original', 'webp'),
-        },
-        # Only previews PDF files in specific locations
-        # Saved as ./output/path/to/image.webp and .png
-        'pdfPreviews': {
-            'include': ('documents/*.pdf', 'forms/*.pdf'),  # glob patterns
-            'max_size': (300, 500),
-            'output_types': ('webp', 'png'),
-        }
+    # ./content/images/test.jpg
+    # ---> ./output/images/test.jpg
+    # ./content/images/test.pdf
+    # ---> ./output/images/test.pdf
+    '': {
+        'include': ('images/*', 'documents/*'),
+        'output_types': ('original'),
+    },
+    # ./content/images/test.jpg
+    # ---> ./output/images/content2x/test.jpg
+    # ---> ./output/images/content2x/test.webp
+    'content2x': {
+        'include': ('images/*', 'illustrations/*'),
+        'exclude': ('*.pdf', '*.svg'),
+        'max_size': (800, 1200),
+        'output_types': ('webp', 'original'),
+    },
+    # ./content/documents/test.pdf
+    # ---> ./output/documents/pdfPreviews/test.png
+    # ---> ./output/documents/pdfPreviews/test.webp
+    'pdfPreviews': {
+        'include': 'documents/*',
+        'max_size': (300, 500),
+        'output_types': ('webp', 'png'),
     },
-    # ...
 }
 ```
 
-#### JinjaRenderer
+### JinjaRenderer
 
-Renders Content into Jinja templates using the context made by ContextProcessors.
+Renders `*.jinja` files in the templates directory.
 
-A Template called `./output/hello-world.html.jinja` will be rendered as `./output/hello-world.html`. The template has access to anything you put in the context, including the `entries` dict, and the `get_entries` method.
+The output file has the same name and relative path as the template, but the `.jinja` extension is removed.
 
-A Template called `./output/posts/entry.html.jinja` will render all Entries under `./content/posts/*.md` and save them under `./output/posts/*.html`. The template has access to an `entry` variable.
-
-Only Templates with the `.jinja` extension are rendered. Files or directory names that start with `.` or `_` are not rendered.
+```
+my-website/
+├─ templates/
+│  ├─ contact.html.jinja
+│  ├─ sitemap.xml.jinja
+│  └─ posts/
+│     └─ index.html.jinja
+└─ output/
+   ├─ contact.html
+   ├─ sitemap.xml
+   └─ posts/
+      └─ index.html
+```
 
-Files named `entry.*.jinja` are rendered once for each Entry with the same path. For example, `./templates/posts/entry.html.jinja` will render `./content/posts/hello-world.md`, `./content/posts/foo.md` and `./content/posts/bar.md`. The output path is the entry name with the extension replaced. If `./templates/posts/entry.html.jinja` renders `./templates/posts/hello-world.md`, the output file is `./output/posts/hello-world.html`.
+Files named `entry.*.jinja` will render every entry with the same relative path.
 
-All template files with the `.jinja` extension will be rendered. For example, `./templates/posts/index.html.jinja` will be rendered as `./output/posts/index.html`. Files starting with `_` are ignored.
+```
+my-website/
+├─ content/
+│  └─ posts/
+│     ├─ first-post.md
+│     ├─ second-post.md
+│     └─ _draft.md
+├─ templates/
+│  └─ posts/
+│     └─ entry.html.jinja
+└─ output/
+   └─ posts/
+      ├─ first-post.html
+      └─ second-post.html
+```
 
-The output path is the template name without the `.jinja` extension. For example, `index.html.jinja` will be rendered as `index.html`.
+Files or directory names that start with `.` or `_` are not rendered.
 
-#### StaticAssetRenderer
+```
+my-website/
+├─ content/
+│  └─ posts/
+│     ├─ hello-world.md
+│     ├─ .hidden.md
+│     └─ _drafts
+│        └─ not-rendered.md
+├─ templates/
+│  └─ posts/
+│     └─ entry.html.jinja
+└─ output/
+   └─ posts/
+      └─ hello-world.html
+```
 
-Simply copies static assets (CSS, JS, images, etc.) under `./templates` to the same subdirectory in `./output`. Files starting with `.` are ignored. Files and directories starting with `_` are ignored.
+### StaticAssetRenderer
 
-It uses hard links instead of copying files. It's faster and it saves space.
+Copies all files under `./templates` except `.jinja` files to the same subdirectory in `./output`. Files starting with `.` are ignored. Files and directories starting with `_` are ignored.
 
-## Getting started
+```
+my-website/
+├─ templates/
+│  ├─ _ignored.jpg
+│  ├─ styles.css
+│  ├─ images/
+│  │  └─ hello.png
+│  └─ js/
+│     └─ test.js
+└─ output/
+   ├─ styles.css
+   ├─ images/
+   │  └─ hello.png
+   └─ js/
+      └─ test.js
+```
 
-1. **Create a directory** for your project. This is a sensible structure, because it works automatically with the default configuration:
-    ```
-    example_site/
-    ├── ursus_config.py  # By default, Ursus will use this config file
-    ├── templates/  # By default, Ursus will use this templates directory
-    │   ├── index.html.jinja
-    │   ├── css/
-    │   │   └──style.css
-    │   ├── js/
-    │   │   └──scripts.js
-    │   ├── fonts/
-    │   │   ├── open-sans.svg
-    │   │   ├── open-sans.ttf
-    │   │   └── open-sans.woff
-    │   └── posts/
-    │       ├── index.html.jinja
-    │       └── entry.html.jinja
-    └── content/  # By default, Ursus will use this content directory
-        ├── posts/
-        │   ├── first-post.md
-        │   ├── foo.md
-        │   └── bar.md
-        └── images/
-            └── example.png
-    ```
-2. **Create a config file for your website.** You can copy `ursus/default_config.py`. If you call your config `ursus_config.py` and place it in your project root, it will be loaded automatically. Otherwise you must call ursus with the `-c` argument. If no config is set, Ursus will use the defaults set in `ursus/default_config.py`.
-3. **Call the `ursus` command.**
+It uses hard links instead of copying files, so it does not use extra disk space.
 
-#### Building from Sublime Text
+## How generators work
 
-You can configure Sublime Text to run Ursus when you press Cmd + B:
+Generators bring it all together. A generator takes all of your files, and generates some final product. There is only `StaticSiteGenerator`, which generates a static website. Custom generators could generate a book or a slideshow from the same content and templates.
 
-```json
-// Sublime user settings or project config
-{
-    // ...
-    "build_systems": [{
-        "cmd": ["ursus", "-c", "$project_path/path/to/ursus_config.py"],
-        "name": "Ursus",
-    }],
-    // ...
-}
+## How linters work
 
-```
+Ursus supports linter. They verify the content when `ursus lint` is called. You can find examples in `ursus/linters`.
```

### Comparing `ursus_ssg-1.0.1/bin/ursus` & `ursus_ssg-1.1.0/bin/ursus`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,16 @@
 #!/usr/bin/env python
 from pathlib import Path
-from ursus.utils import import_class, load_config, get_files_in_path
+from ursus import build, lint
 from ursus.config import config
-from watchdog.observers import Observer
+from ursus.server import serve_async
+from ursus.utils import import_module_or_path
 import argparse
 import coloredlogs
-import time
-
-
-def build(watch_for_changes: bool = False):
-    """Runs ursus and builds a static website
-
-    Args:
-        watch_for_changes (bool, optional): Keep running, and rebuild when content or templates change
-    """
-    generator = import_class(config.generator)()
-    generator.generate()
-
-    if watch_for_changes:
-        observer = Observer()
-
-        for path in generator.get_watched_paths():
-            observer.schedule(generator.get_observer_event_handler(), path, recursive=True)
-        observer.start()
-        try:
-            while True:
-                time.sleep(1)
-        finally:
-            observer.stop()
-            observer.join()
-
-
-def lint():
-    """Lints the content for errors"""
-    linters = [import_class(linter_path)() for linter_path in config.linters]
-
-    for file_path in sorted(get_files_in_path(config.content_path)):
-        for linter in linters:
-            linter.lint(file_path, fix_errors=False)
+import logging
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(
         prog='ursus',
         description='Static site generator',
         epilog='Made with ❤️ in Berlin'
@@ -61,23 +30,45 @@
         '-w', '--watch', action='store_true',
         help="Regenerate files when <content_path> and <templates_path> change."
     )
     parser.add_argument(
         '-f', '--fast', action='store_true',
         help="Fast rebuilds. Prefer faster page rebuilds to completeness. Related pages might not be reloaded."
     )
+    parser.add_argument(
+        '-s', '--serve', dest='port', nargs='?', const=80, default=None,
+        help="Start a static file server, and serve the generated website on the given port. The default port is 80."
+    )
+    parser.add_argument(
+        'files', type=Path, nargs='*',
+        help="Only lint the given file(s)"
+    )
     args = parser.parse_args()
 
     if args.config:
-        load_config(args.config)
+        import_module_or_path(args.config)
     elif Path('./ursus_config.py').exists():
-        load_config('ursus_config.py')
+        import_module_or_path('ursus_config.py')
 
     if args.fast:
         config.fast_rebuilds = True
 
     coloredlogs.install(**config.logging)
 
+    if args.config:
+        logging.info(f"Loaded config from {args.config}")
+    elif Path('./ursus_config.py').exists():
+        logging.info("Loaded config from ./ursus_config.py")
+    else:
+        logging.warning("No config supplied. Using default config.")
+
+    logging.info(f"Content path: {str(config.content_path)}")
+    logging.info(f"Templates path: {str(config.templates_path)}")
+    logging.info(f"Output path: {str(config.output_path)}")
+
+    if args.port:
+        serve_async(args.port)
+
     if args.action == 'build':
         build(args.watch)
     elif args.action == 'lint':
-        lint()
+        lint(files_to_lint=args.files or None)
```

### Comparing `ursus_ssg-1.0.1/setup.py` & `ursus_ssg-1.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name='ursus_ssg',
-    version='1.0.1',
+    version='1.1.0',
     description='Static site generator',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='http://github.com/nicbou/ursus',
     author='Nicolas Bouliane',
     author_email='contact@nicolasbouliane.com',
     license='MIT',
     packages=find_packages(),
     scripts=['bin/ursus'],
-    python_requires='>=3.10',
+    python_requires='>=3.11',
     install_requires=[
         'coloredlogs==15.0.1',
         'GitPython==3.1.30',
+        'imagesize==1.4.1',
         'Jinja2==3.1.2',
+        'jinja2-simple-tags==0.5.0',
+        'libsass==0.22.0',
         'lunr==0.6.2',
-        'Markdown==3.4.1',
+        # 'Markdown==3.4.3',
+        # Use main branch when github.com/Python-Markdown/markdown/pull/1354/ is merged
+        'Markdown @ git+https://github.com/nicbou/markdown.git@nicbou-patch-1',
         'MarkupSafe==2.1.1',
         'ordered-set==4.1.0',
         'PyMuPDF==1.21.1',
         'Pillow==9.4.0',  # Pillow-simd is much faster, but requires binaries to be installed separately.
         'watchdog==2.2.1',
+        'requests==2.31.0',
         'rjsmin==1.2.1',
         'rcssmin==1.1.1',
     ],
     zip_safe=False,
-)
+)
```

### Comparing `ursus_ssg-1.0.1/ursus/config.py` & `ursus_ssg-1.1.0/ursus/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,23 +26,34 @@
     # The base URL prepended to all markdown [[wikilinks]], without a trailing slash.
     # For example, https://allaboutberlin.com/glossary
     wikilinks_base_url: str = '/'
     wikilinks_url_suffix: str = ''
     wikilinks_url_builder: callable = None
     wikilinks_html_class: str = None
 
+    # The CSS class of Markdown list items with a checkbox ("- [ ] list item")
+    # Sets the class of the <li> and the <input type="checkbox">
+    checkbox_list_item_class: str = None
+    checkbox_list_item_input_class: str = None
+
+    # If set, all Markdown tables are wrapped with a div that has this class.
+    table_wrapper_class: str = None
+
     # Minify Javascript and CSS
     minify_js: bool = False
     minify_css: bool = False
 
     # Rebuilds the output faster by only rebuilding templates for the changed files.
     # Related pages (like index pages) will not be rebuild, even though they could change.
     # If false, the pages that definitely changed are still rebuilt before others.
     fast_rebuilds: bool = False
 
+    # Sets the <img sizes=""> attribute for your content images
+    image_default_sizes: str = None
+
     # Transforms applied to your content images
     image_transforms: dict = field(default_factory=default_image_transforms)
 
     """
     Parametres to generate a search index for lunr.js
     Example:
     {
@@ -60,32 +71,38 @@
     lunr_index_output_path: Path = Path('search-index.json')  # Relative to output_path
 
     generator: str = 'ursus.generators.static.StaticSiteGenerator'
 
     # The processors that update the context with extra data
     context_processors: tuple = (
         'ursus.context_processors.stale.StaleEntriesProcessor',
+        'ursus.context_processors.image.ImageProcessor',
         'ursus.context_processors.markdown.MarkdownProcessor',
         'ursus.context_processors.get_entries.GetEntriesProcessor',
         'ursus.context_processors.related.RelatedEntriesProcessor',
         # 'ursus.context_processors.git_date.GitDateProcessor',
     )
     context_globals: dict = field(default_factory=dict)
 
     # The renderers that take your templates and content, and populate the output dir
     renderers: tuple = (
         'ursus.renderers.static.StaticAssetRenderer',
         'ursus.renderers.image.ImageTransformRenderer',
         'ursus.renderers.jinja.JinjaRenderer',
         'ursus.renderers.lunr.LunrIndexRenderer',
+        'ursus.renderers.sass.SassRenderer',
     )
 
     # Linters look for errors in your content
     linters: tuple = (
-        'ursus.linters.markdown.MarkdownLinksLinter',
+        'ursus.linters.markdown.MarkdownLinkTextsLinter',
+        'ursus.linters.markdown.MarkdownLinkTitlesLinter',
+        'ursus.linters.markdown.MarkdownInternalLinksLinter',
+        'ursus.linters.markdown.MarkdownExternalLinksLinter',
+        'ursus.linters.images.UnusedImagesLinter',
     )
 
     # Filter functions available in Jinja templates. The key is the filter name, and the value is a function
     jinja_filters = {}
 
     logging = {
         'datefmt': '%Y-%m-%d %H:%M:%S',
```

### Comparing `ursus_ssg-1.0.1/ursus/context_processors/__init__.py` & `ursus_ssg-1.1.0/ursus/context_processors/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 from ursus.utils import get_files_in_path
 from ursus.config import config
 
 
 class ContextProcessor:
     def process(self, context: dict, changed_files: set = None) -> dict:
+        """Transforms the context and returns it. The context is used to render templates.
+
+        Args:
+            context (dict): An object that represents all data used to render templates
+                (website info, blog posts, utility functions, etc.)
+            changed_files (set, optional): A list of files that changed since the last context update.
+
+        Returns:
+            dict: The updated context
+        """
         return context
 
 
 class EntryContextProcessor(ContextProcessor):
     def process(self, context: dict, changed_files: set = None) -> dict:
         for file_path in get_files_in_path(config.content_path, changed_files):
             entry_uri = str(file_path)
-            entry = context['entries'].get(entry_uri, {})
-            context['entries'][entry_uri] = self.process_entry(entry_uri, entry)
-
-            assert context['entries'][entry_uri] is not None, \
-                "{type(self).__name__}.process_entry is returning None instead of the entry context."
-
+            context['entries'].setdefault(entry_uri, {})
+            self.process_entry(context, entry_uri)
         return context
 
-    def process_entry(self, entry_uri: str, entry_context: dict) -> dict:
+    def process_entry(self, context: dict, entry_uri: str):
         raise NotImplementedError
```

### Comparing `ursus_ssg-1.0.1/ursus/context_processors/git_date.py` & `ursus_ssg-1.1.0/ursus/context_processors/git_date.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         except ValueError:
             return None
 
     def process(self, context: dict, changed_files: set = None) -> dict:
         if not config.fast_rebuilds:
             for commit in self.repo.iter_commits("master"):
                 commit_date = datetime.fromtimestamp(commit.authored_date)
-                for file in commit.stats.files.keys():
+                for file in self.repo.git.show(commit.hexsha, name_only=True, diff_filter='ACMR').split('\n'):
                     entry_uri = self.commit_path_to_entry_uri(file)
                     if entry_uri and entry_uri in context['entries']:
                         entry = context['entries'][entry_uri]
                         if not entry.get('date_updated') or commit_date > entry['date_updated']:
                             entry['date_updated'] = commit_date
 
         for entry in context['entries'].values():
```

### Comparing `ursus_ssg-1.0.1/ursus/context_processors/markdown.py` & `ursus_ssg-1.1.0/ursus/context_processors/markdown.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,26 +5,73 @@
 from markdown.extensions.smarty import SubstituteTextPattern
 from markdown.extensions.toc import TocExtension, slugify
 from markdown.extensions.wikilinks import WikiLinkExtension, build_url
 from markdown.inlinepatterns import SimpleTagPattern
 from markdown.postprocessors import RawHtmlPostprocessor
 from markdown.preprocessors import Preprocessor
 from markdown.treeprocessors import Treeprocessor, InlineProcessor
+from markdown.extensions.codehilite import CodeHiliteExtension
 from pathlib import Path
 from ursus.config import config
 from ursus.utils import make_figure_element, make_picture_element
 from xml.etree import ElementTree
 import logging
 import markdown
 import re
 
 
 logger = logging.getLogger(__name__)
 
 
+class TaskListProcessor(Treeprocessor):
+    box_checked = '[x] '
+    box_unchecked = '[ ] '
+
+    def run(self, root):
+        for li in root.iter(tag='li'):
+            text = (li.text or "")
+
+            if text.lower().startswith((self.box_checked, self.box_unchecked)):
+                is_checked = text.lower().startswith(self.box_checked)
+
+                checkbox = ElementTree.Element("input", {'type': 'checkbox'})
+                if is_checked:
+                    checkbox.attrib['checked'] = 'checked'
+                if self.md.getConfig('checkbox_class'):
+                    checkbox.attrib['class'] = self.md.getConfig('checkbox_class')
+
+                checkbox.tail = li.text.removeprefix(self.box_checked if is_checked else self.box_unchecked)
+                li.text = ''
+                li.insert(0, checkbox)
+                if self.md.getConfig('list_item_class'):
+                    css_classes = set(li.attrib.get('class', '').split())
+                    css_classes.update(self.md.getConfig('list_item_class').split())
+                    li.attrib['class'] = " ".join(css_classes)
+
+        return root
+
+
+class TaskListExtension(Extension):
+    """
+    Adds github-flavored markdown todo lists:
+
+    * [ ] Unchecked item
+    * [x] Checked item
+    """
+    def __init__(self, **kwargs):
+        self.config = {
+            "list_item_class": ['', 'CSS class to add to the <li> element'],
+            "checkbox_class": ['', 'CSS class to add to the checkbox <input>'],
+        }
+        super().__init__(**kwargs)
+
+    def extendMarkdown(self, md):
+        md.treeprocessors.register(TaskListProcessor(self), "gfm-tasklist", 100)
+
+
 class TypographyExtension(Extension):
     """
     Minor typographic improvements
     """
     def extendMarkdown(self, md):
         inline_processor = InlineProcessor(md)
 
@@ -124,17 +171,14 @@
 
 class ResponsiveImageProcessor(Treeprocessor):
     allowed_parents = (
         'a', 'p', 'pre', 'ul', 'ol', 'dl', 'div', 'blockquote', 'noscript', 'section', 'nav', 'article',
         'aside', 'header', 'footer', 'table', 'form', 'fieldset', 'menu', 'canvas', 'details'
     )
 
-    def __init__(self, md):
-        super().__init__(md)
-
     def _swap_element(self, parent, old, new):
         """
         Replaces `old` element with `new` in `parent` element
         """
         for index, element in enumerate(parent):
             if element == old:
                 parent[index] = new
@@ -142,15 +186,15 @@
                 return
 
     def _upgrade_img(self, img, parents):
         # Create <picture> with <source> for the different image types and sizes
         # Only apply to local images
         img_src = img.attrib.get('src')
         if img_src.startswith('/') or img_src.startswith(config.site_url + '/'):
-            image_path = Path(img_src.removeprefix(config.site_url).removeprefix('/'))
+            image_uri = img_src.removeprefix(config.site_url).removeprefix('/')
 
             parent = parents[0]
             grandparent = parents[1]
 
             def has_single_child(element):
                 return len(element) == 1 and not element.text
 
@@ -188,15 +232,15 @@
                 element_to_swap = parent
                 containing_element = grandparent
 
             # This element does not allow a <figure>. Just use a <picture>.
             elif parent.tag not in self.allowed_parents:
                 image_maker = make_picture_element
 
-            image = image_maker(image_path, config.output_path, img_attrs, a_attrs)
+            image = image_maker(self.md.context, image_uri, img_attrs, a_attrs, sizes=config.image_default_sizes)
 
             self._swap_element(containing_element, element_to_swap, image)
 
     def run(self, root):
         parent_map = {}
         for parent in root.iter():
             for child in parent:
@@ -226,14 +270,61 @@
         self.reset()
         md.treeprocessors.register(ResponsiveImageProcessor(md), 'figure', 0)
 
     def reset(self):
         pass
 
 
+class WrappedTableProcessor(Treeprocessor):
+    """
+    Wrap tables in a <div> to allow scrollable tables on mobile.
+    """
+    def wrap_table(self, table, parent):
+        wrapper = ElementTree.Element('div', attrib={
+            'class': self.md.getConfig('table_wrapper_class')
+        })
+        wrapper.append(table)
+
+        for index, element in enumerate(parent):
+            if element == table:
+                parent[index] = wrapper
+                wrapper.tail = table.tail
+                return
+
+    def run(self, root):
+        parent_map = {}
+        for parent in root.iter():
+            for child in parent:
+                parent_map[child] = parent
+
+        for table in root.iter('table'):
+            child = table
+            parents = []
+            while parent := parent_map.get(child):
+                parents.append(parent)
+                child = parent
+
+            self.wrap_table(table, parents[0])
+
+
+class WrappedTableExtension(Extension):
+    """
+    Tables are wrapped in a <div>
+    """
+    def __init__(self, **kwargs):
+        self.config = {
+            "table_wrapper_class": ['', 'CSS class to add to the <div> element that wraps the table'],
+        }
+        super().__init__(**kwargs)
+
+    def extendMarkdown(self, md):
+        if self.getConfig('table_wrapper_class'):
+            md.treeprocessors.register(WrappedTableProcessor(self), 'wrappedtable', 0)
+
+
 class SuperscriptExtension(Extension):
     """
     ^text^ is converted to <sup>text</sup>
     """
 
     # match ^, at least one character that is not ^, and ^ again
     SUPERSCRIPT_RE = r"(\^)([^\^]+)\2"
@@ -257,15 +348,15 @@
         container.set("id", "footnotes")
         summary = ElementTree.SubElement(container, "summary")
         summary.text = "Sources and footnotes"
         ol = ElementTree.SubElement(container, "ol")
 
         surrogate_parent = ElementTree.Element("div")
 
-        backlink_title = self.getConfig("BACKLINK_TITLE")
+        backlink_title = self.getConfig("BACKLINK_TITLE").replace("%d", "{}")
 
         for index, id in enumerate(self.footnotes.keys(), start=1):
             li = ElementTree.SubElement(ol, "li")
             li.set("id", self.makeFootnoteId(id))
             # Parse footnote with surrogate parent as li cannot be used.
             # List block handlers have special logic to deal with li.
             # When we are done parsing, we will copy everything over to li.
@@ -298,57 +389,71 @@
     return slugify(value.lstrip(' 0123456789'), separator, keep_unicode)
 
 
 class MarkdownProcessor(EntryContextProcessor):
     def __init__(self):
         super().__init__()
 
-        self.markdown = markdown.Markdown(extensions=[
-            'fenced_code',
-            'meta',
-            'tables',
-            TocExtension(slugify=patched_slugify),
-            CustomFootnotesExtension(BACKLINK_TEXT="⤴"),
-            JinjaExtension(),
-            SuperscriptExtension(),
-            TypographyExtension(),
-            CurrencyExtension(),
-            ResponsiveImagesExtension(),
-            WikiLinkExtension(
-                base_url=config.wikilinks_base_url + '/',
-                end_url=config.wikilinks_url_suffix,
-                build_url=config.wikilinks_url_builder or build_url,
-                html_class=config.wikilinks_html_class,
-            ),
-        ])
+        self.markdown = markdown.Markdown(
+            output_format='html',
+            extensions=[
+                'fenced_code',
+                'meta',
+                'tables',
+                'smarty',
+                CodeHiliteExtension(guess_lang=False),
+                TocExtension(slugify=patched_slugify),
+                CustomFootnotesExtension(BACKLINK_TEXT="⤴"),
+                JinjaExtension(),
+                SuperscriptExtension(),
+                TypographyExtension(),
+                CurrencyExtension(),
+                ResponsiveImagesExtension(),
+                WikiLinkExtension(
+                    base_url=config.wikilinks_base_url + '/',
+                    end_url=config.wikilinks_url_suffix,
+                    build_url=config.wikilinks_url_builder or build_url,
+                    html_class=config.wikilinks_html_class,
+                ),
+                TaskListExtension(
+                    list_item_class=config.checkbox_list_item_class,
+                    checkbox_class=config.checkbox_list_item_input_class,
+                ),
+                WrappedTableExtension(
+                    table_wrapper_class=config.table_wrapper_class,
+                )
+            ]
+        )
 
     def _parse_metadata(self, raw_metadata):
         metadata = {}
         for key, value in raw_metadata.items():
             if len(value) == 0:
                 continue
             if len(value) == 1:
                 value = value[0]
 
             if key.startswith('date_'):
                 value = datetime.strptime(value, '%Y-%m-%d')
 
             if key.startswith('related_'):
-                values = [v.strip() for v in value.split(',')]
+                if type(value) == list:
+                    values = list(filter(bool, [v.strip() for v in value]))
+                else:
+                    values = [v.strip() for v in value.split(',')]
                 value = values if len(values) > 1 else values[0]
 
             metadata[key] = value
         return metadata
 
-    def process_entry(self, entry_uri: str, entry_context: dict) -> dict:
+    def process_entry(self, context: dict, entry_uri: str):
         if entry_uri.endswith('.md'):
             with (config.content_path / entry_uri).open(encoding='utf-8') as f:
+                self.markdown.context = context
                 html = self.markdown.reset().convert(f.read())
 
-            entry_context.update({
+            context['entries'][entry_uri].update({
                 **self._parse_metadata(self.markdown.Meta),
                 'body': html,
                 'table_of_contents': self.markdown.toc_tokens,
                 'url': f"{config.site_url}/{str(Path(entry_uri).with_suffix(config.html_url_extension))}",
             })
-
-        return entry_context
```

### Comparing `ursus_ssg-1.0.1/ursus/context_processors/related.py` & `ursus_ssg-1.1.0/ursus/context_processors/related.py`

 * *Files identical despite different names*

### Comparing `ursus_ssg-1.0.1/ursus/context_processors/stale.py` & `ursus_ssg-1.1.0/ursus/context_processors/stale.py`

 * *Files identical despite different names*

### Comparing `ursus_ssg-1.0.1/ursus/generators/__init__.py` & `ursus_ssg-1.1.0/ursus/generators/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,38 +23,39 @@
         if self.debounce_timer:
             self.debounce_timer.cancel()
         self.debounce_timer = threading.Timer(0.5, self.on_file_changes)
         self.debounce_timer.start()
 
     def dispatch(self, event):
         if event.event_type in ('created', 'modified', 'moved', 'deleted'):
-            logger.info(f"File {event.event_type}: {event.src_path}")
             self.queued_events.add(event)
             self.reschedule_rebuild()
 
     def on_file_changes(self):
         if self.is_rebuilding:
             self.reschedule_rebuild()
             return
 
         self.is_rebuilding = True
+
         changed_files = set(Path(event.src_path) for event in self.queued_events)
         changed_files.update([Path(e.dest_path) for e in self.queued_events if e.event_type == 'moved'])
         self.queued_events.clear()
-        self.generator.on_file_changes(changed_files)
+        if len(changed_files):
+            try:
+                self.generator.on_file_changes(changed_files)
+            except:
+                logging.exception("Could not generate site")
         self.is_rebuilding = False
 
 
 class Generator:
     def generate(self, changed_files: set = None):
         raise NotImplementedError
 
-    def lint(self):
-        raise NotImplementedError
-
     def get_watched_paths(self):
         return [config.content_path, ]
 
     def get_observer_event_handler(self) -> FileSystemEventHandler:
         return GeneratorObserverEventHandler(generator=self)
 
     def on_file_changes(self, changed_files: set):
```

### Comparing `ursus_ssg-1.0.1/ursus/generators/static.py` & `ursus_ssg-1.1.0/ursus/generators/static.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from ursus.config import config
-from ursus.utils import import_class, get_files_in_path
+from ursus.utils import import_class
 from . import Generator
 import logging
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -39,31 +39,28 @@
         """
         if config.fast_rebuilds and changed_files is not None:
             logger.info("Updating context...")
         else:
             logger.info("Building context...")
 
         for context_processor in self.context_processors:
+            logger.debug(f"Processing context with {type(context_processor).__name__}")
             self.context = context_processor.process(self.context, changed_files)
 
         """
         Render entries and other templates
         """
         files_to_keep = set()
         for renderer in self.renderers:
+            logger.debug(f"Rendering entries with {type(renderer).__name__}")
             files_to_keep.update(renderer.render(self.context, changed_files))
 
         """
         Delete output files older than this build. This is how stale output files are deleted.
         """
         if not config.fast_rebuilds:
             for file in config.output_path.rglob('*'):
                 if file.is_file() and file.relative_to(config.output_path) not in files_to_keep:
                     logger.warning(f"Deleting stale output file {str(file.relative_to(config.output_path))}")
                     file.unlink()
 
         logger.info("Done.")
-
-    def lint(self):
-        for file_path in get_files_in_path(config.content_path):
-            for linter in config.linters:
-                errors = linter.lint(file)
```

### Comparing `ursus_ssg-1.0.1/ursus/renderers/__init__.py` & `ursus_ssg-1.1.0/ursus/renderers/__init__.py`

 * *Files identical despite different names*

### Comparing `ursus_ssg-1.0.1/ursus/renderers/image.py` & `ursus_ssg-1.1.0/ursus/renderers/image.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,61 +1,50 @@
 from . import Renderer
 from PIL import Image
 from ursus.config import config
-from ursus.utils import get_files_in_path, make_image_thumbnail, make_pdf_thumbnail, is_image, is_pdf, is_svg, \
-    copy_file, get_image_transforms
+from ursus.utils import make_image_thumbnail, make_pdf_thumbnail, is_pdf, is_svg, copy_file
 import logging
 
 
 logger = logging.getLogger(__name__)
 
 
 class ImageTransformRenderer(Renderer):
     """
     Resizes images and generate PDF thumbnails
     """
     def __init__(self):
         super().__init__()
 
-    def get_files_to_transform(self):
-        return [
-            f for f in get_files_in_path(config.content_path)
-            if is_image(config.content_path / f) or is_pdf(config.content_path / f)
-        ]
-
     def render(self, context: dict, changed_files: set = None) -> set:
         logger.info("Rendering image transforms...")
 
         files_to_keep = set()
 
-        for input_path in self.get_files_to_transform():
-            abs_input_path = config.content_path / input_path
-            has_changed = changed_files is None or abs_input_path in changed_files
+        for entry_uri, entry in context['entries'].items():
+            abs_file_path = config.content_path / entry_uri
 
-            for transform in get_image_transforms(input_path):
+            for transform in entry.get('transforms', []):
                 output_path = transform['output_path']
                 abs_output_path = config.output_path / output_path
                 max_size = transform['max_size']
 
+                has_changed = changed_files is None or abs_file_path in changed_files
                 if has_changed and not abs_output_path.exists():
-                    if is_pdf(abs_input_path):
+                    if is_pdf(abs_file_path):
                         if abs_output_path.suffix.lower() == '.pdf':
-                            logger.info('Copying %s to %s', str(input_path), str(output_path))
-                            copy_file(abs_input_path, abs_output_path)
-                        else:
-                            logger.info('Generating %s preview as %s', str(input_path), str(output_path))
-                            make_pdf_thumbnail(config.content_path / input_path, max_size, abs_output_path)
-                    elif is_svg(abs_input_path):
-                        if abs_output_path.suffix.lower() == '.svg':
-                            logger.info('Copying %s to %s', str(input_path), str(output_path))
-                            copy_file(abs_input_path, abs_output_path)
+                            logger.info('Copying %s to %s', entry_uri, str(output_path))
+                            copy_file(abs_file_path, abs_output_path)
                         else:
-                            logger.warning(f"Can't convert {str(input_path)} to {abs_output_path.suffix}. Ignoring.")
-                            continue
+                            logger.info('Generating %s preview as %s', entry_uri, str(output_path))
+                            make_pdf_thumbnail(abs_file_path, max_size, abs_output_path)
+                    elif is_svg(abs_file_path):
+                        logger.info('Copying %s to %s', entry_uri, str(output_path))
+                        copy_file(abs_file_path, abs_output_path)
                     else:
-                        logger.info('Converting %s to %s', str(input_path), str(output_path))
-                        with Image.open(abs_input_path) as pil_image:
+                        logger.info('Converting %s to %s', entry_uri, str(output_path))
+                        with Image.open(abs_file_path) as pil_image:
                             make_image_thumbnail(pil_image, max_size, abs_output_path)
 
                 files_to_keep.add(output_path)
 
         return files_to_keep
```

### Comparing `ursus_ssg-1.0.1/ursus/renderers/jinja.py` & `ursus_ssg-1.1.0/ursus/renderers/jinja.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from . import Renderer
 from jinja2 import Environment, FileSystemLoader, nodes, pass_context, select_autoescape, StrictUndefined
 from jinja2.exceptions import TemplateSyntaxError
 from jinja2.ext import Extension, do
+from jinja2.meta import find_referenced_templates
+from jinja2_simple_tags import StandaloneTag, ContainerTag
+from markdown.serializers import to_html_string
 from markupsafe import Markup
 from ordered_set import OrderedSet
 from pathlib import Path
 from rjsmin import jsmin
 from rcssmin import cssmin
 from ursus.config import config
 from ursus.utils import get_files_in_path, make_picture_element, is_ignored_file
-from xml.etree import ElementTree
 import logging
+import sass
 
 
 logger = logging.getLogger(__name__)
 
 
 class JsLoaderExtension(Extension):
     """
@@ -42,132 +45,142 @@
         else:
             body = parser.parse_statements(["name:endjs"], drop_needle=True)
             return nodes.CallBlock(
                 self.call_method("_queue_js"), [], [], body
             ).set_lineno(token.lineno)
 
     def _render_js(self, caller):
-        output = "".join(self.environment.js_fragments)
+        output = "\n".join(self.environment.js_fragments)
         if config.minify_js:
             output = jsmin(output)
         self.environment.js_fragments.clear()
         return Markup(output)
 
     def _queue_js(self, caller):
         self.environment.js_fragments.add(caller())
         return ''
 
 
-class CssLoaderExtension(Extension):
+class CssLoaderExtension(ContainerTag):
     """
     Jinja extension. Adds the {% css %} tag.
 
     All CSS code in {% css %} tags is minified if config.minify_css is True.
     """
     tags = {"css"}
+    safe_output = True
 
-    def __init__(self, environment):
-        super().__init__(environment)
-        environment.extend(js_fragments=OrderedSet())
-
-    def parse(self, parser):
-        token = next(parser.stream)
-
-        if token.test('name:css'):
-            body = parser.parse_statements(["name:endcss"], drop_needle=True)
-            return nodes.CallBlock(
-                self.call_method("_render_css"), [], [], body
-            ).set_lineno(token.lineno)
-
-    def _render_css(self, caller):
+    def render(self, caller):
         output = caller()
         if config.minify_css:
             output = cssmin(output)
         return Markup(output)
 
 
-class ResponsiveImageExtension(Extension):
-    """Jinja extension. Adds {% image 'relative/path/to/original.jpg' %} tag.
+class ScssLoaderExtension(ContainerTag):
+    """
+    Jinja extension. Adds the {% scss %} tag.
 
-    This tag is replaced by a responsive <picture> element. The correct image transforms for the given source image are
-    used.
+    All Sass code in {% scss %} tags is converted to CSS.
+    It's also minified if config.minify_css is True.
     """
-    tags = {"image"}
+    tags = {"scss"}
+    safe_output = True
 
-    def __init__(self, environment):
-        super().__init__(environment)
-        environment.extend(js_fragments=OrderedSet())
+    def __init__(self, *args, **kwargs):
+        self.scss_cache = {}
 
-    def parse(self, parser):
-        token = next(parser.stream)
+    def render(self, caller):
+        scss_code = caller()
+        if scss_code not in self.scss_cache:
+            self.scss_cache[scss_code] = Markup(
+                sass.compile(
+                    string=scss_code,
+                    output_style='compressed' if config.minify_css else 'nested',
+                    include_paths=[str(config.templates_path)],
+                )
+            )
+        return self.scss_cache[scss_code]
 
-        args = [parser.parse_expression()]
 
-        if parser.stream.skip_if("comma"):
-            args.append(parser.parse_expression())
-        else:
-            args.append(nodes.Const(None))
+class ResponsiveImageExtension(StandaloneTag):
+    """Jinja extension. Adds {% image %} tag.
 
-        call = self.call_method('_render_image', args)
-        return nodes.Output([nodes.MarkSafe(call)]).set_lineno(token.lineno)
+    Usage: {% image 'relative/path/to/original.jpg' img_class='a_css_class' sizes='(min-width: 600px) 160px, 320px' %}
 
-    @pass_context
-    def _render_image(self, context, image_path, image_class):
-        img_attrs = {'class': image_class} if image_class else {}
-        output = make_picture_element(
-            original_path=Path(image_path),
-            output_path=config.output_path,
-            img_attrs=img_attrs,
-        )
-        return Markup(ElementTree.tostring(output, encoding='unicode'))
+    This tag is replaced by a responsive <picture> element. The correct image transforms for the given source image are
+    used.
+    """
+    tags = {"image"}
+    safe_output = True
+
+    def render(self, image_entry_uri, css_class=None, alt=None, sizes=None):
+        img_attrs = {}
+
+        if css_class:
+            img_attrs['class'] = css_class
+        if alt:
+            img_attrs['alt'] = alt
+
+        # Render the same way as Python Markdown does, for consistency
+        return to_html_string(make_picture_element(self.context, image_entry_uri, img_attrs, sizes))
 
 
 @pass_context
 def render_filter(context, value):
     return context.eval_ctx.environment.from_string(value).render(**context)
 
 
 def is_entry_template(template_path: Path) -> bool:
     return template_path.with_suffix('').stem == 'entry'
 
 
 def template_can_render_entry(template_path: Path, entry_uri: str) -> bool:
-    return entry_uri.startswith(str(template_path.parent) + '/')
+    return Path(entry_uri).parent == template_path.parent
 
 
 class JinjaRenderer(Renderer):
     """
     Renders all .jinja templates in the templates directory, unless their name starts with '_'.
     """
     def __init__(self):
         super().__init__()
         self.template_environment = Environment(
             loader=FileSystemLoader(config.templates_path),
-            extensions=[do, JsLoaderExtension, CssLoaderExtension, ResponsiveImageExtension],
+            extensions=[do, JsLoaderExtension, CssLoaderExtension, ScssLoaderExtension, ResponsiveImageExtension],
             autoescape=select_autoescape(),
             undefined=StrictUndefined
         )
         self.template_environment.filters['render'] = render_filter
         self.template_environment.filters.update(config.jinja_filters)
 
+    def get_child_templates(self, template_path: Path):
+        dependencies = set()
+        with (config.templates_path / template_path).open() as template_file:
+            ast = self.template_environment.parse(template_file.read())
+        child_template_paths = [Path(t.removeprefix('/')) for t in find_referenced_templates(ast)]
+        for child_template_path in child_template_paths:
+            dependencies.add(child_template_path)
+            dependencies.update(self.get_child_templates(child_template_path))
+        return dependencies
+
     def render_template(self, template_path: Path, context: dict, output_path: Path):
         """Returns an entry into a template, and saves it under output_path
         Args:
             template_path (Path): Path to the template to use, relative to output_path.
             context (dict): Context object used to render the template.
             output_path (str): Path of the generated file, relative to the output_path.
         """
         logger.info('Rendering %s', str(output_path))
         abs_output_path = config.output_path / output_path
         abs_output_path.parent.mkdir(parents=True, exist_ok=True)
         template = self.template_environment.get_template(str(template_path))
         try:
             template.stream(**context).dump(str(abs_output_path))
         except TemplateSyntaxError:
-            print(context.get('entry', {}).get('body'))
             raise
         return output_path
 
     def get_entry_output_path(self, template_path: Path, entry_uri: str) -> Path:
         """Gets the path where the rendered template will be saved
         Args:
             template_path (Path): Template used to render the entry
@@ -185,15 +198,16 @@
             context (dict): Context object used to render the template.
             entry_uri (str): URI of the entry to render
         Returns:
             Path: Path of the generated file, relative to the output_path.
         """
         specific_context = {
             **context,
-            'entry': context['entries'][entry_uri]
+            'entry': context['entries'][entry_uri],
+            'entry_uri': entry_uri,
         }
         output_path = self.get_entry_output_path(template_path, entry_uri)
         return self.render_template(template_path, specific_context, output_path)
 
     def render(self, context: dict, changed_files: set = None) -> set:
         template_paths = get_files_in_path(config.templates_path, suffix='.jinja')
 
@@ -204,28 +218,41 @@
         changed_templates = set()
         for file in (changed_files or set()):
             if not (file.exists() and file.is_file()):
                 continue
 
             if file.is_relative_to(config.content_path) and not is_ignored_file(file, config.content_path):
                 changed_entry_uris.add(str(file.relative_to(config.content_path)))
-            elif file.is_relative_to(config.templates_path) and not is_ignored_file(file, config.templates_path):
+            elif file.is_relative_to(config.templates_path):
                 changed_templates.add(file.relative_to(config.templates_path))
             else:
                 continue
 
+        if changed_files is not None and config.fast_rebuilds:
+            # Also rerender templates that depend on the changed templates (_style.css > _layout.html > index.html)
+            changed_parent_templates = set()
+            for template_path in template_paths:
+                dependencies = self.get_child_templates(template_path)
+                for changed_template in changed_templates:
+                    if changed_template in dependencies:
+                        logger.info(f"{template_path} is affected by {changed_template} change")
+                        changed_parent_templates.add(template_path)
+            changed_templates.update(changed_parent_templates)
+
         # Process edited entries
         for entry_uri in changed_entry_uris:
             for tp in template_paths:
                 if is_entry_template(tp) and template_can_render_entry(tp, entry_uri):
                     render_queue.add(('entry', tp, entry_uri))
 
         # Process edited templates
         for template_path in changed_templates:
-            if is_entry_template(template_path):
+            if is_ignored_file(config.templates_path / template_path, config.templates_path):
+                continue
+            elif is_entry_template(template_path):
                 for entry_uri in context['entries']:
                     if template_can_render_entry(template_path, entry_uri):
                         render_queue.add(('entry', template_path, entry_uri))
             else:
                 render_queue.add(('template', template_path, template_path.with_suffix('')))
 
         # Process everything else
```

### Comparing `ursus_ssg-1.0.1/ursus/renderers/lunr.py` & `ursus_ssg-1.1.0/ursus/renderers/lunr.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,19 @@
     - 'documents': A dict of entry URI to documents that can be used to render
         search results (titles, URLs, excerpts, etc.)
     """
     def __init__(self):
         super().__init__()
 
     def render(self, context: dict, changed_files: set = None) -> set:
+        if config.fast_rebuilds:
+            return set()
+
         index_output_path = config.output_path / config.lunr_index_output_path
-        logger.info(f"Generating search index at {index_output_path}")
+        logger.info(f"Generating search index at {config.lunr_index_output_path}")
 
         indexed_documents = []
         returned_documents = {}
 
         for index in config.lunr_indexes.get('indexes', []):
             for entry_uri, entry in context['entries'].items():
                 if Path(entry_uri).match(index['uri_pattern']):
```

### Comparing `ursus_ssg-1.0.1/ursus/renderers/static.py` & `ursus_ssg-1.1.0/ursus/renderers/static.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     Copies static assets in `templates_path` to `output_path`.
     """
     ignored_suffixes = ('.jinja', )
 
     def get_assets_to_copy(self, changed_files: set = None):
         return [
             f for f in get_files_in_path(config.templates_path)
-            if f.suffix not in self.ignored_suffixes
+            if f.suffix.lower() not in self.ignored_suffixes
         ]
 
     def render(self, context: dict, changed_files: set = None) -> set:
         files_to_keep = set()
         for asset_path in self.get_assets_to_copy():
             abs_output_path = config.output_path / asset_path
```

### Comparing `ursus_ssg-1.0.1/ursus/utils.py` & `ursus_ssg-1.1.0/ursus/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 from importlib import import_module
 from pathlib import Path
 from PIL import Image
 from typing import Iterator
 from ursus.config import config
 from xml.etree import ElementTree
 import fitz
+import imagesize
+import logging
 import shutil
 import sys
 
 
+log_colors = {
+    logging.DEBUG: '',
+    logging.INFO: '\033[37m\033[0;100m',
+    logging.WARNING: '\033[1;90m\033[43m',
+    logging.ERROR: '\033[37m\033[41m',
+    logging.CRITICAL: '\033[37m\033[41m',
+}
+
+
 def import_class(import_path):
     module_name, class_name = import_path.rsplit('.', 1)
     module = import_module(module_name)
     return getattr(module, class_name)
 
 
-def load_config(module_or_path: str) -> dict:
+def import_module_or_path(module_or_path: str) -> dict:
     """
-    Imports the `config` variable from a Python file or a Python module
+    Imports a module (path.to.module.class or path/to/module.py)
 
     Args:
-        module_or_path (str): path.to.config.module, or path/to/config.py
-
-    Returns:
-        dict: The ursus config at this location
+        module_or_path (str): path.to.module, or path/to/module.py
     """
     file_path = Path(module_or_path)
     if file_path.exists():
         sys.path.append(str(file_path.parent))
-        module = import_module(file_path.with_suffix('').name)
-    else:
-        module = import_module(module_or_path)
+        return import_module(file_path.with_suffix('').name)
+    return import_module(module_or_path)
 
-    return getattr(module, 'config')
 
-
-def is_ignored_file(path: Path, root_path: Path = None) -> bool:
+def is_ignored_file(path: Path, root_path: Path) -> bool:
     """Returns whether a file should be ignored by ursus.
     Args:
         path (Path): Path to the file
-        root_path (Path, optional): Root path. The name of parent directories above root_path are not considered.
+        root_path (Path): Root path. The name of parent directories above root_path are not considered.
 
     Returns:
         bool: True if the file or any of its parents (up to root_path) start with _ or .
     """
     return (
         path.stem.startswith(('_', '.'))
         or any([
@@ -91,14 +96,36 @@
     Returns:
         bool: Whether this file is an SVG image
     """
     assert path.is_absolute(), 'is_svg must be called with an absolute path'
     return path.is_file() and path.suffix.lower() == '.svg'
 
 
+def is_raster_image(path: Path):
+    return is_image(path) and not is_svg(path)
+
+
+def get_image_size(path: Path):
+    """
+    Args:
+        path (Path): The absolute Path to an image
+    Returns:
+        tuple: The image width and height as a tuple
+    """
+    try:
+        width, height = imagesize.get(path)
+        if width == height == -1:
+            logging.debug(f"Can't get image size, trying again with Pillow: {path}")
+            with Image.open(path) as pil_image:
+                width, height = pil_image.size
+        return width, height
+    except Exception as e:
+        raise Exception(f"Invalid image size: {path}") from e
+
+
 def get_files_in_path(path: Path, whitelist: set = None, suffix: str = None) -> list[Path]:
     """
     Returns a list of valid, visible files under a given path.
 
     Args:
         path (Path): The path under which to find files
         whitelist (set, optional): Only include files that are part of this whitelist
@@ -114,15 +141,19 @@
             elif f.is_absolute() and f.is_relative_to(path):
                 files.append(f)
     else:
         files = path.rglob('[!._]*' + (suffix or ''))
 
     return [
         f.relative_to(path) for f in files
-        if f.is_file() and not is_ignored_file(f, path)
+        if (
+            f.is_file()
+            and not is_ignored_file(f, path)
+            and suffix in (None, f.suffix)
+        )
     ]
 
 
 def copy_file(input_path: Path, output_path: Path):
     """Copies a file
 
     Args:
@@ -177,15 +208,15 @@
 
 
 def get_image_transforms(original_path: Path) -> Iterator[dict]:
     """
     Yields a list of image transforms that apply to a file.
 
     Args:
-        original_path (Path): Path of the original file/image to transform
+        original_path (Path): Path of the original file/image to transform, relative to config.content_path
 
     Yields:
         Iterator[dict]: A list of image transforms that apply to this file.
     """
     suffix_to_mimetype = {
         '.apng': 'image/apng',
         '.avif': 'image/avif',
@@ -194,14 +225,16 @@
         '.jpeg': 'image/jpeg',
         '.pdf': 'application/pdf',
         '.png': 'image/png',
         '.svg': 'image/svg+xml',
         '.webp': 'image/webp',
     }
 
+    assert not original_path.is_absolute(), "original_path must be a relative path"
+
     for key, transform in config.image_transforms.items():
         includes = transform.get('include', ['*'])
         includes = [includes] if isinstance(includes, str) else includes
 
         excludes = transform.get('exclude', [])
         excludes = [excludes] if isinstance(excludes, str) else excludes
 
@@ -218,97 +251,92 @@
                 for t in transform.get('output_types', ['original'])
             ])
 
             for suffix in output_suffixes:
                 if suffix == original_path.suffix.lower():
                     output_image_path = original_path
                 else:
-                    if original_path.suffix.lower() == '.svg':
+                    if is_svg(config.content_path / original_path):
                         # .svg images are not be converted
                         continue
 
                     output_image_path = original_path.with_suffix(suffix)
 
                 yield {
                     **transform,
                     'is_default': key == '',
                     'input_mimetype': suffix_to_mimetype[original_path.suffix.lower()],
                     'output_mimetype': suffix_to_mimetype[output_image_path.suffix.lower()],
                     'output_path': output_image_path.parent / key / output_image_path.name,  # It works if key is empty
                 }
 
 
-def make_picture_element(original_path: Path, output_path: Path, img_attrs={}):
+def make_picture_element(context: dict, entry_uri: str, img_attrs={}, sizes=None):
     """
     Creates a responsive HTML <picture> element
     """
     # Mimetypes with broad support that don't require their own <source> element
     standard_mimetypes = ('image/png', 'image/jpeg', 'image/svg+xml')
 
     # TODO: SVG? PDF?
     default_src = None
 
     # Build a list of srcsets grouped by mimetype
     sources_by_mimetype = {}
-    for transform in get_image_transforms(original_path):
+    for transform in context['entries'][entry_uri]['transforms']:
         width = transform['max_size'][0]
         mimetype = transform['output_mimetype']
 
         if mimetype.startswith('image/'):
             srcset_part = f"{config.site_url}/{str(transform['output_path'])} {width}w"
             sources_by_mimetype.setdefault(mimetype, [])
             sources_by_mimetype[mimetype].append(srcset_part)
 
             if not default_src and mimetype in standard_mimetypes:
                 default_src = transform['output_path']
 
     # Create a <picture> with <source type="" srcset=""> for each mimetype
     picture = ElementTree.Element('picture')
     for mimetype, srcset_elements in sources_by_mimetype.items():
-        source = ElementTree.Element('source', attrib={
+        source = ElementTree.SubElement(picture, 'source', attrib={
             'type': mimetype,
             'srcset': ", ".join(srcset_elements)
         })
-        picture.append(source)
+        if sizes:
+            source.attrib['sizes'] = sizes
 
     # Add an <img> with the default image to the <picture>
-    img = ElementTree.Element('img', attrib=img_attrs)
-    assert default_src is not None, f"default_src is None for {original_path}"
-
-    # The output image might not exist yet, so we use the source's dimensions
-    abs_original_path = config.content_path / original_path
-    if abs_original_path.suffix not in ('.svg', '.pdf'):
-        with Image.open(abs_original_path) as pil_image:
-            width, height = pil_image.size
-            img.attrib['width'] = str(width)
-            img.attrib['height'] = str(height)
+    img = ElementTree.SubElement(picture, 'img', attrib=img_attrs)
+    assert default_src is not None, f"default_src is None for {entry_uri}"
+    if 'width' in context['entries'][entry_uri]:
+        img.attrib['width'] = str(context['entries'][entry_uri]['width'])
+    if 'height' in context['entries'][entry_uri]:
+        img.attrib['height'] = str(context['entries'][entry_uri]['height'])
     img.attrib['loading'] = 'lazy'
     img.attrib['src'] = f"{config.site_url}/{str(default_src)}"
 
-    picture.append(img)
-
     return picture
 
 
-def make_figure_element(original_path: Path, output_path: Path, img_attrs={}, a_attrs=None):
+def make_figure_element(context: dict, entry_uri: str, img_attrs={}, a_attrs=None, sizes=None):
     """
     Creates a responsive HTML <figure> element with the image title as <figcaption>. Returns a simple <picture> if there
     is no title.
     """
-    image = make_picture_element(original_path, output_path, img_attrs)
+    image = make_picture_element(context, entry_uri, img_attrs, sizes=sizes)
     if a_attrs and a_attrs.get('href'):
         a_attrs['target'] = '_blank'
         wrapped_image = ElementTree.Element('a', a_attrs)
         wrapped_image.append(image)
     else:
         wrapped_image = image
 
     if not img_attrs.get('title'):
         return wrapped_image
 
     figure = ElementTree.Element('figure')
     figure.append(wrapped_image)
-    figcaption = ElementTree.Element('figcaption')
+
+    figcaption = ElementTree.SubElement(figure, 'figcaption')
     figcaption.text = img_attrs['title']
-    figure.append(figcaption)
 
     return figure
```

### Comparing `ursus_ssg-1.0.1/ursus_ssg.egg-info/PKG-INFO` & `ursus_ssg-1.1.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,12 @@
-Metadata-Version: 2.1
-Name: ursus-ssg
-Version: 1.0.1
-Summary: Static site generator
-Home-page: http://github.com/nicbou/ursus
-Author: Nicolas Bouliane
-Author-email: contact@nicolasbouliane.com
-License: MIT
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-
 # Ursus
 
-Ursus is the static site generator used by [All About Berlin](https://allaboutberlin.com). It turns Markdown files and [Jinja](https://jinja.palletsprojects.com/) templates into a static website.
+Ursus is the static site generator used by [All About Berlin](https://allaboutberlin.com) and my [personal website](https://nicolasbouliane.com). It turns Markdown files and [Jinja](https://jinja.palletsprojects.com/) templates into a static website.
+
+It also renders images in different sizes, renders SCSS, minifies JS and generates Lunr.js search indexes.
 
 This project is in active use and development.
 
 ## Setup
 
 ### Installation
 
@@ -23,265 +14,407 @@
 
 ```bash
 pip install ursus-ssg
 ```
 
 ### Getting started
 
-By default, Ursus looks for content in `./content`, and templates in `./templates`. It generates a website under `./output`.
+Call `ursus` to generate a static website. Call `ursus --help` to see the command line options it supports.
+
+By default, Ursus looks for 3 directories, relative to the current directory:
 
-Call `ursus` to build the project. Call `ursus --help` to see the command line options it supports.
+- It looks for content in `./content`
+- It looks for page templates in `./templates`
+- It generates a static website in `./output`
 
-Here is a simple piece of content. Save it under `./content/posts/first-post.md`.
+For example, create a markdown file and save it as `./content/posts/first-post.md`.
 
 ```markdown
 ---
-Title: Hello world!
-Description: This is an example page
-Date_created: 2022-10-10
+title: Hello world!
+description: This is an example page
+date_created: 2022-10-10
 ---
 
 ## Hello beautiful world
 
 *This* is a template. Pretty cool eh?
 ```
 
-Here is a simple template. Save it under `./templates/posts/entry.html.jinja`. 
+Then, create a page template and save it as `./templates/posts/entry.html.jinja`. 
 
 ```
 <!DOCTYPE html>
 <html>
 <head>
     <title>{{ entry.title }}</title>
     <meta name="description" content="{{ entry.description }}">
 </head>
 <body>
     {{ entry.body }}
+
+    Created on {{ entry.date_created }}
 </body>
 </html>
 ```
 
-Call `ursus` to generate this website. It will create `./output/posts/first-post.html`.
+Your project should now look like this:
+
+```
+my-website/ <- You are here
+├─ content/
+│  └─ posts/
+│     └─ first-post.md
+└─ templates/
+   └─ posts/
+      └─ entry.html.jinja
+```
+
+Call `ursus` to generate a statuc website. It will create `./output/posts/first-post.html`.
 
 ### Configuring Ursus
 
-You can configure Ursus by creating a `ursus_config.py` file at the root of your project. When you call `ursus`, it will load this configuration.
+To configure Ursus, create a configuration file.
 
 ```python
 # Example Ursus config file
+# Find all configuration options in `ursus/config.py`.
 from ursus.config import config
 
 config.content_path = Path(__file__).parent / 'blog'
 config.templates_path = Path(__file__).parent / 'templates'
 config.output_path = Path(__file__).parent.parent / 'dist'
 
 config.site_url = 'https://allaboutberlin.com'
 
 config.minify_js = True
 config.minify_css = True
 ```
 
-You can find all configuration options in `ursus/config.py`.
+If you call your configuration file `ursus_config.py`, Ursus loads it automatically.
+
+```
+my-website/
+├─ ursus_config.py
+├─ content/
+└─ templates/
+```
 
-You can give your config a different name, and load it with the `-c` argument:
+You can also load a configuration file with the `-w` argument.
 
 ```bash
-ursus -c path/to/config.py
+ursus -c /path/to/config.py
 ```
 
-## Basic concepts
+### Watching for changes
 
-### Content and Entries
+Ursus can rebuild your website when the content or templates change.
 
-**Content** is what fills your website: text, images, videos, PDFs. A single piece of content is called an **Entry**. The location of the Content is set by `config.content_path`. By default, it's under `./content`.
+```bash
+# Rebuild when content or templates change
+ursus -w
+ursus --watch
+```
 
-Content is usually *rendered* to create a working website. Some content (like Markdown files) is rendered with Templates, and other (like images) is converted to a different file format.
+It can only rebuild the pages that changed. This is much faster, but it does not work perfectly.
 
-### Templates
+```bash
+# Only rebuild the pages that changed
+ursus -wf
+ursus --watch --fast
+```
 
-**Templates** are used to render your Content. They are the theme of your website. The same templates can be applied to different Entries, or even reused for a different website. They are kept in a separate directory.
+### Serving the website
 
-For example, a template can be the HTML that makes up the page around your content: the header, sidebar, and footer.
+Ursus can serve the website it generates. This is useful for testing.
 
-The location of the Templates is set by `config.templates_path`. By default, it's under `./templates`. You can have a different `templates_path` for each Generator.
+```bash
+# Serve the static website on port 80
+ursus -s
+ursus --serve 80
+```
 
-For example:
+This is not meant for production. Use nginx, Caddy or some other static file server for that.
 
-- HTML templates that wrap a nice theme around your Content.
-- Images and other static assets that are part of the website's theme
+## How Ursus works
 
-### Output
+1. **Context processors** generate the context used to render templates. The context is just a big dictionary.
+2. **Renderers** use the context and the templates to render the parts of the final website: pages, thumbnails, static assets, etc.
 
-This is the final static website generated by Ursus.
+### Content
 
-The location of the Output is set by `config.output_path`. By default, it's under `./output`.
+**Content** is what fills your website: text, images, videos, PDFs. Content is usually *rendered* to create a working website. Some content (like Markdown files) is rendered with Templates, and other (like images) is converted to a different file format.
 
-## How Ursus works
+Ursus looks for content in `./content`, unless you change `config.content_path`.
 
-ContextProcessors transform the context, which is a dict with information about each of your Entries. Renderers use the context to know which pages to create, and what content to put in the templates.
+### Entries
 
-In the example above, your context would look like this:
+A single piece of content is called an **Entry**. This can be a single image, a single markdown file, etc.
 
-```
+Each Entry has a **URI**. This is the Entry's unique identifier. The URI is the Entry's path relative to the content directory. For example, the URI of `./content/posts/first-post.md` is `posts/first-post.md`.
+
+### Context
+
+The **Context** contains the information needed to render your website. It's just a big dictionary, and you can put anything in it.
+
+`context['entries']` contains is a dictionary of all your entries. The key is the Entry URI.
+
+**Context processors** each add specific data to the context. For example, `MarkdownProcessor` adds your `.md` content to `context.entries`.
+
+```python
+# Example context
 {
     'entries': {
         'posts/first-post.md': {
             'title': 'Hello world!',
             'description': 'This is an example page',
-            'body': '<h2>Hello beautiful world</h2><p>...'
-        }
+            'date_created': datetime(2022, 10, 10),
+            'body': '<h2>Hello beautiful world</h2><p>...',
+        },
+        'posts/second-post.md': {
+            # ...
+        },
     },
-    'get_entries': function
-    'globals': {},
+    # Context processors can add more things to the context
+    'blog_title': 'Example blog',
+    'site_url': 'https://example.com/blog',
 }
 ```
 
-### Generators
+### Templates
 
-A **Generator** takes your Content and your Templates and produces an Output. It's a recipe to turn your content into a final result. The default **StaticSiteGenerator** generates a static website. You can write your own Generator to output an eBook, a PDF, or anything else.
+**Templates** are used to render your Content. They are the theme of your website. Jinja templates, Javascript, CSS and theme images belong in the templates directory.
 
-#### StaticSiteGenerator
+Ursus looks for templates in `./templates`, unless you change `config.templates_path`.
 
-Generates a static website.
+### Renderers
+
+**Renderers** use the Context and the Templates to generate parts of your static website. For example, `JinjaRenderer` renders Jinja templates, `ImageTransformRenderer` converts and resizes your images, and `StaticAssetRenderer` copies your static assets.
 
-### Context processors
+### Output
 
-The context is a big object that is used to render templates.
+This is the final static website generated by Ursus. Ursus generates a static website in `./output`, unless you change `config.output_path`.
 
-A **ContextProcessor** fills this context object, or transforms its existing contents.
+The content of the output directory is ready to be served by any static file server.
 
-For example, the **MarkdownProcessor** generates the entry context out of a markdown file.
+## How context processors work
 
-Only Entries with matching ContextProcessors are rendered. Entry or directory names that start with `.` or `_` are not rendered. You can use this to create drafts.
+Context processors transform the context, which is a dict with information about each of your Entries.
 
-#### MarkdownProcessor
+Context processors ignore file and directory names that start with `.` or `_`. For example, `./content/_drafts/hello.md` and `./content/posts/_post-draft.md` are ignored.
 
-The `MarkdownProcessor` creates context for all `.md` files in `content_path`.
+### MarkdownProcessor
+
+The `MarkdownProcessor` creates context for all `.md` files in `content_path`. The markdown content is in the `body` attribute.
+
+```python
+{
+    'entries': {
+        'posts/first-post.md': {
+            'title': 'Hello world!',
+            'description': 'This is an example page',
+            'date_created': datetime(2022, 10, 10),
+            'body': '<h2>Hello beautiful world</h2><p>...',
+        },
+        # ...
+    },
+}
+```
 
 It makes a few changes to the default markdown output:
 
-- Lazyload images (`loading=lazy`)
-- Convert images to `<figure>` tags when appropriate
-- Jinja tags (`{{ ... }}` and `{% ... %}`) are rendered as-is. You can use the, to `{% include %}` template parts and `{{ variables }}` in your content.
-- Set the `srcset` to load responsive images from the `image_transforms` config.
 - Put the front matter in the context
-    - `Related_*` keys are replaced by a list of related entry dicts
-    - `Date_` keys are converted to `datetime` objects
+    - `related_*` keys are replaced by a list of related entry dicts
+    - `date_` keys are converted to `datetime` objects
+    - Other attributes are added to the entry object.
+- Use responsive images based on `config.image_transforms` settings.
+- `<img>` are converted to `<figure>` or `<picture>` tags when appropriate.
+- Images are lazy-loaded with the `loading=lazy` attribute.
+- Jinja tags (`{{ ... }}` and `{% ... %}`) are rendered as-is. You can use `{% include %}` and `{{ variables }}` in your content.
 
-#### GetEntriesProcessor
+### GetEntriesProcessor
 
 The `GetEntriesProcessor` adds a `get_entries` method to the context. It's used to get a list of entries of a certain type, and sort it.
 
 ```jinja
-{% set posts = get_entries('posts', sort_by='date_created', reverse=True) %}
+{% set posts = get_entries('posts', filter_by=filter_function, sort_by='date_created', reverse=True) %}
+
+{% for post in posts %}
+...
 ```
 
-### Renderers
+### GitDateProcessor
 
-**Renderer**s create content that make up the Output. In other words, they turn your content files into pages, correctly-sized images, RSS feeds, etc.
+Adds the `date_updated` attribute to all Entries. It uses the file's last commit date.
+
+```python
+{
+    'entries': {
+        'posts/first-post.md': {
+            'date_updated': datetime(2022, 10, 10),
+            # ...
+        },
+        # ...
+    },
+}
+```
 
-#### ImageTransformRenderer
+### ImageProcessor
 
-Renders images in `content_path` with a few changes:
+Adds images and PDFs Entries to the context. Dimensions and image transforms are added to each Entry. Use in combination with `config.image_transforms`.
 
-- Images are compressed and optimized.
-- Images are resized according to the `image_transforms`. The images are shrunk if needed, but never stretched.
+```python
+{
+    'entries': {
+        'images/hello.jpg': {
+            'width': 320,
+            'height': 240,
+            'image_transforms': [
+                {
+                    'is_default': True,
+                    'input_mimetype': 'image/jpeg',
+                    'output_mimetype': 'image/webp',
+                    # ...
+                },
+                # ...
+            ]
+        },
+        # ...
+    },
+}
+```
+
+## How renderers work
+
+Renderers use context and templates to generate parts of the static website.
+
+A **Generator** takes your Content and your Templates and produces an Output. It's a recipe to turn your content into a final result. The default **StaticSiteGenerator** generates a static website. You can write your own Generator to output an eBook, a PDF, or anything else.
+
+### ImageTransformRenderer
+
+Renders images in your content directory.
+
+- Images are converted and resized according to `config.image_transforms`.
 - Files that can't be transformed (PDF to PDF) are copied as-is to the output directory.
 - Images that can't be resized (SVG to anything) are copied as-is to the output directory.
 - Image EXIF data is removed.
 
-This renderer does nothing unless `image_transforms` is set:
+This renderer does nothing unless `config.image_transforms` is set:
+
 ```python
+from ursus.config import config
+
 config.image_transforms = {
-    # ...
-    'image_transforms': {
-        # Default transform used as <img> src
-        # Saved as ./output/path/to/image.jpg
-        '': {
-            'max_size': (3200, 4800),
-        },
-        # Saved as ./output/path/to/image.jpg and .webp
-        'thumbnails': {
-            'exclude': ('*.pdf', '*.svg'),  # glob patterns
-            'max_size': (400, 400),
-            'output_types': ('original', 'webp'),
-        },
-        # Only previews PDF files in specific locations
-        # Saved as ./output/path/to/image.webp and .png
-        'pdfPreviews': {
-            'include': ('documents/*.pdf', 'forms/*.pdf'),  # glob patterns
-            'max_size': (300, 500),
-            'output_types': ('webp', 'png'),
-        }
+    # ./content/images/test.jpg
+    # ---> ./output/images/test.jpg
+    # ./content/images/test.pdf
+    # ---> ./output/images/test.pdf
+    '': {
+        'include': ('images/*', 'documents/*'),
+        'output_types': ('original'),
+    },
+    # ./content/images/test.jpg
+    # ---> ./output/images/content2x/test.jpg
+    # ---> ./output/images/content2x/test.webp
+    'content2x': {
+        'include': ('images/*', 'illustrations/*'),
+        'exclude': ('*.pdf', '*.svg'),
+        'max_size': (800, 1200),
+        'output_types': ('webp', 'original'),
+    },
+    # ./content/documents/test.pdf
+    # ---> ./output/documents/pdfPreviews/test.png
+    # ---> ./output/documents/pdfPreviews/test.webp
+    'pdfPreviews': {
+        'include': 'documents/*',
+        'max_size': (300, 500),
+        'output_types': ('webp', 'png'),
     },
-    # ...
 }
 ```
 
-#### JinjaRenderer
-
-Renders Content into Jinja templates using the context made by ContextProcessors.
+### JinjaRenderer
 
-A Template called `./output/hello-world.html.jinja` will be rendered as `./output/hello-world.html`. The template has access to anything you put in the context, including the `entries` dict, and the `get_entries` method.
+Renders `*.jinja` files in the templates directory.
 
-A Template called `./output/posts/entry.html.jinja` will render all Entries under `./content/posts/*.md` and save them under `./output/posts/*.html`. The template has access to an `entry` variable.
+The output file has the same name and relative path as the template, but the `.jinja` extension is removed.
 
-Only Templates with the `.jinja` extension are rendered. Files or directory names that start with `.` or `_` are not rendered.
+```
+my-website/
+├─ templates/
+│  ├─ contact.html.jinja
+│  ├─ sitemap.xml.jinja
+│  └─ posts/
+│     └─ index.html.jinja
+└─ output/
+   ├─ contact.html
+   ├─ sitemap.xml
+   └─ posts/
+      └─ index.html
+```
 
-Files named `entry.*.jinja` are rendered once for each Entry with the same path. For example, `./templates/posts/entry.html.jinja` will render `./content/posts/hello-world.md`, `./content/posts/foo.md` and `./content/posts/bar.md`. The output path is the entry name with the extension replaced. If `./templates/posts/entry.html.jinja` renders `./templates/posts/hello-world.md`, the output file is `./output/posts/hello-world.html`.
+Files named `entry.*.jinja` will render every entry with the same relative path.
 
-All template files with the `.jinja` extension will be rendered. For example, `./templates/posts/index.html.jinja` will be rendered as `./output/posts/index.html`. Files starting with `_` are ignored.
+```
+my-website/
+├─ content/
+│  └─ posts/
+│     ├─ first-post.md
+│     ├─ second-post.md
+│     └─ _draft.md
+├─ templates/
+│  └─ posts/
+│     └─ entry.html.jinja
+└─ output/
+   └─ posts/
+      ├─ first-post.html
+      └─ second-post.html
+```
 
-The output path is the template name without the `.jinja` extension. For example, `index.html.jinja` will be rendered as `index.html`.
+Files or directory names that start with `.` or `_` are not rendered.
 
-#### StaticAssetRenderer
+```
+my-website/
+├─ content/
+│  └─ posts/
+│     ├─ hello-world.md
+│     ├─ .hidden.md
+│     └─ _drafts
+│        └─ not-rendered.md
+├─ templates/
+│  └─ posts/
+│     └─ entry.html.jinja
+└─ output/
+   └─ posts/
+      └─ hello-world.html
+```
 
-Simply copies static assets (CSS, JS, images, etc.) under `./templates` to the same subdirectory in `./output`. Files starting with `.` are ignored. Files and directories starting with `_` are ignored.
+### StaticAssetRenderer
 
-It uses hard links instead of copying files. It's faster and it saves space.
+Copies all files under `./templates` except `.jinja` files to the same subdirectory in `./output`. Files starting with `.` are ignored. Files and directories starting with `_` are ignored.
 
-## Getting started
+```
+my-website/
+├─ templates/
+│  ├─ _ignored.jpg
+│  ├─ styles.css
+│  ├─ images/
+│  │  └─ hello.png
+│  └─ js/
+│     └─ test.js
+└─ output/
+   ├─ styles.css
+   ├─ images/
+   │  └─ hello.png
+   └─ js/
+      └─ test.js
+```
 
-1. **Create a directory** for your project. This is a sensible structure, because it works automatically with the default configuration:
-    ```
-    example_site/
-    ├── ursus_config.py  # By default, Ursus will use this config file
-    ├── templates/  # By default, Ursus will use this templates directory
-    │   ├── index.html.jinja
-    │   ├── css/
-    │   │   └──style.css
-    │   ├── js/
-    │   │   └──scripts.js
-    │   ├── fonts/
-    │   │   ├── open-sans.svg
-    │   │   ├── open-sans.ttf
-    │   │   └── open-sans.woff
-    │   └── posts/
-    │       ├── index.html.jinja
-    │       └── entry.html.jinja
-    └── content/  # By default, Ursus will use this content directory
-        ├── posts/
-        │   ├── first-post.md
-        │   ├── foo.md
-        │   └── bar.md
-        └── images/
-            └── example.png
-    ```
-2. **Create a config file for your website.** You can copy `ursus/default_config.py`. If you call your config `ursus_config.py` and place it in your project root, it will be loaded automatically. Otherwise you must call ursus with the `-c` argument. If no config is set, Ursus will use the defaults set in `ursus/default_config.py`.
-3. **Call the `ursus` command.**
+It uses hard links instead of copying files, so it does not use extra disk space.
 
-#### Building from Sublime Text
+## How generators work
 
-You can configure Sublime Text to run Ursus when you press Cmd + B:
+Generators bring it all together. A generator takes all of your files, and generates some final product. There is only `StaticSiteGenerator`, which generates a static website. Custom generators could generate a book or a slideshow from the same content and templates.
 
-```json
-// Sublime user settings or project config
-{
-    // ...
-    "build_systems": [{
-        "cmd": ["ursus", "-c", "$project_path/path/to/ursus_config.py"],
-        "name": "Ursus",
-    }],
-    // ...
-}
+## How linters work
 
-```
+Ursus supports linter. They verify the content when `ursus lint` is called. You can find examples in `ursus/linters`.
```

### Comparing `ursus_ssg-1.0.1/ursus_ssg.egg-info/SOURCES.txt` & `ursus_ssg-1.1.0/ursus_ssg.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 README.md
 setup.py
 bin/ursus
 ursus/__init__.py
 ursus/config.py
+ursus/server.py
 ursus/utils.py
 ursus/context_processors/__init__.py
 ursus/context_processors/get_entries.py
 ursus/context_processors/git_date.py
+ursus/context_processors/image.py
 ursus/context_processors/markdown.py
 ursus/context_processors/related.py
 ursus/context_processors/stale.py
 ursus/generators/__init__.py
 ursus/generators/static.py
 ursus/linters/__init__.py
+ursus/linters/images.py
 ursus/linters/markdown.py
 ursus/renderers/__init__.py
 ursus/renderers/image.py
 ursus/renderers/jinja.py
 ursus/renderers/lunr.py
+ursus/renderers/sass.py
 ursus/renderers/static.py
 ursus_ssg.egg-info/PKG-INFO
 ursus_ssg.egg-info/SOURCES.txt
 ursus_ssg.egg-info/dependency_links.txt
 ursus_ssg.egg-info/not-zip-safe
 ursus_ssg.egg-info/requires.txt
 ursus_ssg.egg-info/top_level.txt
```

