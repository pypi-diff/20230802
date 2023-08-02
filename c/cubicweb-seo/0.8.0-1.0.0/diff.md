# Comparing `tmp/cubicweb-seo-0.8.0.tar.gz` & `tmp/cubicweb-seo-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-seo-0.8.0.tar", last modified: Thu Nov 24 01:35:23 2022, max compression
+gzip compressed data, was "cubicweb-seo-1.0.0.tar", last modified: Wed Aug  2 12:50:19 2023, max compression
```

## Comparing `cubicweb-seo-0.8.0.tar` & `cubicweb-seo-1.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 01:35:23.430997 cubicweb-seo-0.8.0/
--rw-rw-rw-   0 root         (0) root         (0)      424 2022-11-24 01:35:10.000000 cubicweb-seo-0.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      536 2022-11-24 01:35:23.430997 cubicweb-seo-0.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       71 2022-11-24 01:35:10.000000 cubicweb-seo-0.8.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 01:35:23.430997 cubicweb-seo-0.8.0/cubicweb_seo/
--rw-rw-rw-   0 root         (0) root         (0)       96 2022-11-24 01:35:10.000000 cubicweb-seo-0.8.0/cubicweb_seo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2022-11-24 01:35:10.000000 cubicweb-seo-0.8.0/cubicweb_seo/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 01:35:23.430997 cubicweb-seo-0.8.0/cubicweb_seo/i18n/
--rw-rw-rw-   0 root         (0) root         (0)      203 2022-11-24 01:35:10.000000 cubicweb-seo-0.8.0/cubicweb_seo/i18n/en.po
--rw-rw-rw-   0 root         (0) root         (0)      203 2022-11-24 01:35:10.000000 cubicweb-seo-0.8.0/cubicweb_seo/i18n/es.po
--rw-rw-rw-   0 root         (0) root         (0)      203 2022-11-24 01:35:10.000000 cubicweb-seo-0.8.0/cubicweb_seo/i18n/fr.po
--rw-rw-rw-   0 root         (0) root         (0)    14258 2022-11-24 01:35:10.000000 cubicweb-seo-0.8.0/cubicweb_seo/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 01:35:23.430997 cubicweb-seo-0.8.0/cubicweb_seo.egg-info/
--rw-r--r--   0 root         (0) root         (0)      536 2022-11-24 01:35:22.000000 cubicweb-seo-0.8.0/cubicweb_seo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      500 2022-11-24 01:35:23.000000 cubicweb-seo-0.8.0/cubicweb_seo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-24 01:35:22.000000 cubicweb-seo-0.8.0/cubicweb_seo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       36 2022-11-24 01:35:23.000000 cubicweb-seo-0.8.0/cubicweb_seo.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-24 01:35:22.000000 cubicweb-seo-0.8.0/cubicweb_seo.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       25 2022-11-24 01:35:23.000000 cubicweb-seo-0.8.0/cubicweb_seo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-11-24 01:35:23.000000 cubicweb-seo-0.8.0/cubicweb_seo.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-24 01:35:23.430997 cubicweb-seo-0.8.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2628 2022-11-24 01:35:10.000000 cubicweb-seo-0.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 01:35:23.430997 cubicweb-seo-0.8.0/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 01:35:23.430997 cubicweb-seo-0.8.0/test/data/
--rw-rw-rw-   0 root         (0) root         (0)        4 2022-11-24 01:35:10.000000 cubicweb-seo-0.8.0/test/data/bootstrap_cubes
--rw-rw-rw-   0 root         (0) root         (0)      202 2022-11-24 01:35:10.000000 cubicweb-seo-0.8.0/test/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)    14065 2022-11-24 01:35:10.000000 cubicweb-seo-0.8.0/test/unittest_views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 12:50:19.957244 cubicweb-seo-1.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      424 2023-08-02 12:49:59.000000 cubicweb-seo-1.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      516 2023-08-02 12:50:19.957244 cubicweb-seo-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-08-02 12:49:59.000000 cubicweb-seo-1.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 12:50:19.949244 cubicweb-seo-1.0.0/cubicweb_seo/
+-rw-rw-rw-   0 root         (0) root         (0)       96 2023-08-02 12:49:59.000000 cubicweb-seo-1.0.0/cubicweb_seo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      721 2023-08-02 12:49:59.000000 cubicweb-seo-1.0.0/cubicweb_seo/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 12:50:19.957244 cubicweb-seo-1.0.0/cubicweb_seo/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-08-02 12:49:59.000000 cubicweb-seo-1.0.0/cubicweb_seo/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-08-02 12:49:59.000000 cubicweb-seo-1.0.0/cubicweb_seo/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-08-02 12:49:59.000000 cubicweb-seo-1.0.0/cubicweb_seo/i18n/fr.po
+-rw-rw-rw-   0 root         (0) root         (0)    13959 2023-08-02 12:49:59.000000 cubicweb-seo-1.0.0/cubicweb_seo/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 12:50:19.953244 cubicweb-seo-1.0.0/cubicweb_seo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      516 2023-08-02 12:50:19.000000 cubicweb-seo-1.0.0/cubicweb_seo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      500 2023-08-02 12:50:19.000000 cubicweb-seo-1.0.0/cubicweb_seo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 12:50:19.000000 cubicweb-seo-1.0.0/cubicweb_seo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-08-02 12:50:19.000000 cubicweb-seo-1.0.0/cubicweb_seo.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 12:50:19.000000 cubicweb-seo-1.0.0/cubicweb_seo.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       50 2023-08-02 12:50:19.000000 cubicweb-seo-1.0.0/cubicweb_seo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-02 12:50:19.000000 cubicweb-seo-1.0.0/cubicweb_seo.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-02 12:50:19.957244 cubicweb-seo-1.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2610 2023-08-02 12:49:59.000000 cubicweb-seo-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 12:50:19.957244 cubicweb-seo-1.0.0/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 12:50:19.957244 cubicweb-seo-1.0.0/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)        4 2023-08-02 12:49:59.000000 cubicweb-seo-1.0.0/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)      202 2023-08-02 12:49:59.000000 cubicweb-seo-1.0.0/test/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    13963 2023-08-02 12:49:59.000000 cubicweb-seo-1.0.0/test/unittest_views.py
```

### Comparing `cubicweb-seo-0.8.0/PKG-INFO` & `cubicweb-seo-1.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 Metadata-Version: 2.1
 Name: cubicweb-seo
-Version: 0.8.0
+Version: 1.0.0
 Summary: search engine optimisation with robotstxt and sitemaps
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-seo
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: JavaScript
 
 Summary
 -------
 search engine optimisation with robotstxt and sitemaps
-
-
```

### Comparing `cubicweb-seo-0.8.0/cubicweb_seo/views.py` & `cubicweb-seo-1.0.0/cubicweb_seo/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # copyright 2012-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
@@ -93,15 +92,15 @@
 
     __regid__ = "robotstxt"
     content_type = "text/plain"
     templatable = False
     __select__ = none_rset()
 
     def call(self):
-        self.w("Sitemap: %s\n\n" % self._cw.build_url("sitemap.xml"))
+        self.w(f"Sitemap: {self._cw.build_url('sitemap.xml')}\n\n")
         if (
             "robotstxt" in self._cw.vreg
         ):  # XXX or make sure it exists by creating it in this cube...
             for rule in self._cw.vreg["robotstxt"].possible_objects(self._cw):
                 self.w(rule.stanza())
                 self.w("\n")
 
@@ -153,39 +152,39 @@
 
     __regid__ = "sitemapxml"
     content_type = "text/xml"
     templatable = False
     __select__ = none_rset()
 
     def add_url(self, url, lastmod=None, chfreq=None, priority=None):
-        self.w("<url><loc>%s</loc>" % url)
+        self.w(f"<url><loc>{url}</loc>")
         if lastmod:
-            self.w("<lastmod>%s</lastmod>" % lastmod.strftime("%Y-%m-%d"))
+            self.w(f"<lastmod>{lastmod.strftime('%Y-%m-%d')}</lastmod>")
         if chfreq:
             if chfreq in CHANGEFREQS:
-                self.w("<changefreq>%s</changefreq>" % chfreq)
+                self.w(f"<changefreq>{chfreq}</changefreq>")
             else:
                 self.error(
                     "url %s gave %s that is not a valid changefreq according to http://sitemaps.org"
                     % (url, chfreq)
                 )
         if priority:
             if 0 <= float(priority) <= 1:
-                self.w("<priority>%.2f</priority>" % priority)
+                self.w(f"<priority>{priority:.2f}</priority>")
             else:
                 self.error(
                     "url %s gave %s which is not a valid priority according to http://sitemaps.org"
                     % (url, priority)
                 )
         self.w("</url>")
 
     def call(self):
         # XXX have a look at databnf/file/stable/sitemap.py for cases where the sitemap file is
         # too big (>10Mb) or has too many entries (>50k)
-        self.w('<?xml version="1.0" encoding="%s"?>\n' % self._cw.encoding)
+        self.w(f'<?xml version="1.0" encoding="{self._cw.encoding}"?>\n')
         self.w('<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">')
         self.add_url(self._cw.base_url())
         if (
             "sitemap" in self._cw.vreg
         ):  # XXX or make sure it exists by creating it in this cube...
             count = 0
             for rule in self._cw.vreg["sitemap"].possible_objects(self._cw):
@@ -198,19 +197,18 @@
                                 "too many items for this sitemap (limit is 50,000)"
                             )
                             break
                     if count > 50000:
                         break
                 except Unauthorized as exc:
                     self.info(
-                        "sitemap rule %s raised Unauthorized: %s"
-                        % (rule.__regid__, exc)
+                        f"sitemap rule {rule.__regid__} raised Unauthorized: {exc}"
                     )
                 except Exception:
-                    self.exception("sitemap rule %s raised exception" % rule.__regid__)
+                    self.exception(f"sitemap rule {rule.__regid__} raised exception")
         else:
             self.debug("no sitemap registry found")
         self.w("</urlset>")
 
 
 class GzippedSitemap(Sitemaps):
     """Allows to download a Gzipped sitemap.xml."""
@@ -219,40 +217,38 @@
     content_type = "application/gzip"
     binary = True
     http_cache_manager = httpcache.EntityHTTPCacheManager
     add_to_breadcrumbs = False
 
     def add_url(self, buf, url, lastmod=None, chfreq=None, priority=None):
         buf.write("<url>")
-        buf.write(
-            "<loc>{0}</loc>".format(urllib.parse.quote(url.encode("utf-8"), safe=":/"))
-        )
+        buf.write(f"<loc>{urllib.parse.quote(url.encode('utf-8'), safe=':/')}</loc>")
         if lastmod:
-            buf.write("<lastmod>{0}</lastmod>".format(lastmod.strftime("%Y-%m-%d")))
+            buf.write(f"<lastmod>{lastmod.strftime('%Y-%m-%d')}</lastmod>")
         if chfreq:
             if chfreq in CHANGEFREQS:
-                buf.write("<changefreq>{0}</changefreq>".format(chfreq))
+                buf.write(f"<changefreq>{chfreq}</changefreq>")
             else:
                 self.error(
                     "url %s gave %s which is not a valid changefreq according to "
                     "http://sitemaps.org" % (url, chfreq)
                 )
         if priority:
             if 0 <= float(priority) <= 1:
-                buf.write("<priority>{0}</priority>".format(priority))
+                buf.write(f"<priority>{priority}</priority>")
             else:
                 self.error(
                     "url %s gave %s which is not a valid priority according to "
                     "http://sitemaps.org" % (url, priority)
                 )
         buf.write("</url>")
 
     def call(self):
         buf = StringIO()
-        buf.write('<?xml version="1.0" encoding="{0}"?>\n'.format(self._cw.encoding))
+        buf.write(f'<?xml version="1.0" encoding="{self._cw.encoding}"?>\n')
         buf.write('<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">')
         self.add_url(buf, self._cw.base_url())
         if (
             "sitemap" in self._cw.vreg
         ):  # XXX or make sure it exists by creating it in this cube...
             count = 0
             for rule in self._cw.vreg["sitemap"].possible_objects(self._cw):
@@ -265,19 +261,18 @@
                                 "too many items for this sitemap (limit is 50,000)"
                             )
                             break
                     if count > 50000:
                         break
                 except Unauthorized as exc:
                     self.info(
-                        "sitemap rule %s raised Unauthorized: %s"
-                        % (rule.__regid__, exc)
+                        f"sitemap rule {rule.__regid__} raised Unauthorized: {exc}"
                     )
                 except Exception:
-                    self.exception("sitemap rule %s raised exception" % rule.__regid__)
+                    self.exception(f"sitemap rule {rule.__regid__} raised exception")
         else:
             self.debug("no sitemap registry found")
         buf.write("</urlset>")
         with tempfile.NamedTemporaryFile(delete=False) as f:
             with gzip.open(f.name, mode="wb") as gz:
                 gz.write(buf.getvalue().encode("utf-8"))
         self._cw.set_content_type(
@@ -305,34 +300,28 @@
     add_to_breadcrumbs = False
 
     def new_sitemap_buffer(self, index=False):
         """Create a new buffer storing content about a Sitemap file in memory.
 
         If ``index`` is True, start a buffer for a Sitemap index file."""
         buf = StringIO()
-        buf.write('<?xml version="1.0" encoding="{0}"?>\n'.format(self._cw.encoding))
+        buf.write(f'<?xml version="1.0" encoding="{self._cw.encoding}"?>\n')
         tagname = "urlset" if not index else "sitemapindex"
-        buf.write(
-            '<{0} xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">'.format(tagname)
-        )
+        buf.write(f'<{tagname} xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">')
         return buf
 
     def save_partial_sitemap(self, sitemap_buf, fname, index_buf):
         """Save content in ``sitemap_buf`` into ``fname``, and add an index entry in
         ``index_buf``."""
         sitemap_buf.write("</urlset>")
         with gzip.open(fname, mode="wb") as gz:
             gz.write(sitemap_buf.getvalue().encode("utf-8"))
         index_buf.write("<sitemap>")
-        index_buf.write(
-            "<loc>{0}</loc>".format(self._cw.build_url(os.path.basename(fname)))
-        )
-        index_buf.write(
-            "<lastmod>{0}</lastmod>".format(date.today().strftime("%y-%m-%d"))
-        )
+        index_buf.write(f"<loc>{self._cw.build_url(os.path.basename(fname))}</loc>")
+        index_buf.write(f"<lastmod>{date.today().strftime('%y-%m-%d')}</lastmod>")
         index_buf.write("</sitemap>")
 
     def save_sitemap_index(self, index_buf, index_fname):
         """Save content in ``sitemap_buf`` into ``fname``, and add an index entry in
         ``index_buf``."""
         index_buf.write("</sitemapindex>")
         with gzip.open(index_fname, mode="wb") as gz:
@@ -358,19 +347,18 @@
                             )
                             file_number += 1
                             buf = self.new_sitemap_buffer()
                             entries = 1
                         self.add_url(buf, *item)
                 except Unauthorized as exc:
                     self.info(
-                        "sitemap rule %s raised Unauthorized: %s"
-                        % (rule.__regid__, exc)
+                        f"sitemap rule {rule.__regid__} raised Unauthorized: {exc}"
                     )
                 except Exception:
-                    self.exception("sitemap rule %s raised exception" % rule.__regid__)
+                    self.exception(f"sitemap rule {rule.__regid__} raised exception")
             self.save_partial_sitemap(buf, fname_templ.format(file_number), index_buf)
             self.save_sitemap_index(index_buf, index_fname)
         else:
             self.debug("no sitemap registry found")
         with tempfile.NamedTemporaryFile(delete=False) as f:
             with zipfile.ZipFile(f.name, mode="w") as zf:
                 zf.write(index_fname, os.path.basename(index_fname))
```

### Comparing `cubicweb-seo-0.8.0/cubicweb_seo.egg-info/PKG-INFO` & `cubicweb-seo-1.0.0/cubicweb_seo.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 Metadata-Version: 2.1
 Name: cubicweb-seo
-Version: 0.8.0
+Version: 1.0.0
 Summary: search engine optimisation with robotstxt and sitemaps
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-seo
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: JavaScript
 
 Summary
 -------
 search engine optimisation with robotstxt and sitemaps
-
-
```

### Comparing `cubicweb-seo-0.8.0/setup.py` & `cubicweb-seo-1.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,17 +52,15 @@
 # get optional metadatas
 data_files = __pkginfo__.get("data_files", None)
 dependency_links = __pkginfo__.get("dependency_links", ())
 
 requires = {}
 for entry in ("__depends__",):  # "__recommends__"):
     requires.update(__pkginfo__.get(entry, {}))
-install_requires = [
-    "{0} {1}".format(d, v and v or "").strip() for d, v in requires.items()
-]
+install_requires = [f"{d} {v and v or ''}".strip() for d, v in requires.items()]
 
 
 setup(
     name=distname,
     version=version,
     license=license,
     description=description,
```

### Comparing `cubicweb-seo-0.8.0/test/unittest_views.py` & `cubicweb-seo-1.0.0/test/unittest_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,26 +19,25 @@
 from io import BytesIO
 from datetime import date, datetime
 import gzip
 import os
 import tempfile
 import zipfile
 
+from cubicweb_web.devtools.testlib import WebCWTC
 from lxml import etree
 
-from cubicweb.devtools.testlib import CubicWebTC
-
 from cubicweb_seo.views import SitemapRule
 
 SITEMAP_NS = "{http://www.sitemaps.org/schemas/sitemap/0.9}"
 
 
 def _sitemap_tag(tag_name):
     """Return the complete tag_name in the Sitemap XML namespace from the given short one."""
-    return "{0}{1}".format(SITEMAP_NS, tag_name)
+    return f"{SITEMAP_NS}{tag_name}"
 
 
 #
 # Test sitemap rules for the test schema.py in test/data
 #
 
 _TITLEDTHING_PRIORITY = 1.0
@@ -58,15 +57,15 @@
 
 
 #
 # Mixin to parse Sitemap XML
 #
 
 
-class SitemapXMLCheckMixin(object):
+class SitemapXMLCheckMixin:
     def assertSitemapContains(
         self,
         sitemap_data,
         expected_url,
         expected_lastmod=None,
         expected_priority=None,
         expected_chfreq=None,
@@ -95,45 +94,45 @@
                 _sitemap_tag("changefreq")
             ) != str(expected_chfreq):
                 continue
             if url_node.findtext(_sitemap_tag("loc")) == expected_url:
                 break
         else:
             raise AssertionError(
-                "Not found in Sitemap: {0} (lastmod={1!r}, priority={2!r}, "
-                "chfreq={3!r})".format(
+                "Not found in Sitemap: {} (lastmod={!r}, priority={!r}, "
+                "chfreq={!r})".format(
                     expected_url, expected_lastmod, expected_priority, expected_chfreq
                 )
             )
 
     def assertSitemapLengthEqual(self, sitemap_data, expected_length):
         """Return True if the Sitemap data has the correct number of entries."""
         root_node = etree.fromstring(sitemap_data)
         length = len(list(root_node.findall(_sitemap_tag("url"))))
         if length != expected_length:
             raise AssertionError(
-                "Sitemap length is {0} (expected: {1})".format(length, expected_length)
+                f"Sitemap length is {length} (expected: {expected_length})"
             )
 
     def assertIndexContains(self, index_data, expected_url):
         """Return True if the given URL is found in the Sitemap index data."""
         root_node = etree.fromstring(index_data)
         for url_node in root_node.findall(_sitemap_tag("sitemap")):
             if url_node.findtext(_sitemap_tag("loc")) == expected_url:
                 break
         else:
-            raise AssertionError("Not found in Sitemap index: {0}".format(expected_url))
+            raise AssertionError(f"Not found in Sitemap index: {expected_url}")
 
 
 #
 # Actual test cases
 #
 
 
-class SitemapViewTC(SitemapXMLCheckMixin, CubicWebTC):
+class SitemapViewTC(SitemapXMLCheckMixin, WebCWTC):
     """Test about the ``sitemapxml`` view."""
 
     def test_sitemap_view_one_entity(self):
         """Check that an XML sitemap is correctly generated with one entity."""
         with self.temporary_appobjects(TitledThingSitemapRule):
             with self.admin_access.repo_cnx() as cnx:
                 thing = cnx.create_entity("TitledThing", title="A thing")
@@ -195,15 +194,15 @@
                     sitemap_data, thing1.absolute_url(), thing1.modification_date
                 )
                 self.assertSitemapContains(
                     sitemap_data, thing2.absolute_url(), thing2.modification_date
                 )
 
 
-class GzippedSitemapViewTC(SitemapXMLCheckMixin, CubicWebTC):
+class GzippedSitemapViewTC(SitemapXMLCheckMixin, WebCWTC):
     """Test about the ``sitemapxmlgz`` view."""
 
     def test_gz_sitemap_view(self):
         """Check that a Gzipped XML sitemap is correctly generated."""
         with self.temporary_appobjects(TitledThingSitemapRule):
             with self.admin_access.repo_cnx() as cnx:
                 thing = cnx.create_entity("TitledThing", title="A thing")
@@ -223,21 +222,21 @@
                     thing.absolute_url(),
                     thing.modification_date,
                     _TITLEDTHING_PRIORITY,
                     _TITLEDTHING_CHFREQ,
                 )
 
 
-class ZippedSitemapsViewTC(SitemapXMLCheckMixin, CubicWebTC):
+class ZippedSitemapsViewTC(SitemapXMLCheckMixin, WebCWTC):
     """Test about the ``massive-sitemaps`` view."""
 
     def create_many_things(self, cnx, n):
         """Create as many as ``n`` ``NamedThing`` using the given connection."""
         for i in range(n):
-            cnx.create_entity("NamedThing", name="Thing {0}".format(i))
+            cnx.create_entity("NamedThing", name=f"Thing {i}")
             if i % 1000 == 0:
                 print(i)
         cnx.commit()
 
     def extract_file(self, fname):
         """Extract the given ZIP file and return list of extracted filenames."""
         tmpdir = tempfile.gettempdir()
@@ -252,17 +251,15 @@
         return sitemaps
 
     def clean(self, zip_fname, gz_number):
         """Remove temporary files."""
         os.remove(zip_fname)
         os.remove(os.path.join(tempfile.gettempdir(), "sitemap.xml.gz"))
         for i in range(1, gz_number):
-            os.remove(
-                os.path.join(tempfile.gettempdir(), "sitemap{0}.xml.gz".format(i))
-            )
+            os.remove(os.path.join(tempfile.gettempdir(), f"sitemap{i}.xml.gz"))
 
     def test_zip_sitemaps_view_one_file(self):
         """Check that a bunch of XML sitemaps is correctly generated and archived in a ZIP file."""
         with self.temporary_appobjects(TitledThingSitemapRule):
             with self.admin_access.repo_cnx() as cnx:
                 thing = cnx.create_entity("TitledThing", title="A thing")
                 cnx.commit()
```

