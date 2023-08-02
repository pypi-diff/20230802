# Comparing `tmp/indieweb_rocks-0.0.2.tar.gz` & `tmp/indieweb_rocks-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indieweb_rocks-0.0.2.tar", max compression
+gzip compressed data, was "indieweb_rocks-0.0.3.tar", max compression
```

## Comparing `indieweb_rocks-0.0.2.tar` & `indieweb_rocks-0.0.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0    18992 2023-08-02 00:07:18.037441 indieweb_rocks-0.0.2/indieweb_rocks/__init__.py
--rw-r--r--   0        0        0    13024 2023-08-02 03:18:39.694204 indieweb_rocks-0.0.2/indieweb_rocks/__web__.py
--rw-r--r--   0        0        0     1563 2023-01-27 00:43:56.404286 indieweb_rocks-0.0.2/indieweb_rocks/static/cc/by.svg
--rw-r--r--   0        0        0     2573 2023-01-27 00:43:56.404286 indieweb_rocks-0.0.2/indieweb_rocks/static/cc/cc.svg
--rw-r--r--   0        0        0     1955 2023-01-27 00:43:56.396285 indieweb_rocks-0.0.2/indieweb_rocks/static/cc/nc-eu.svg
--rw-r--r--   0        0        0     1537 2023-01-27 00:43:56.400285 indieweb_rocks-0.0.2/indieweb_rocks/static/cc/nc-jp.svg
--rw-r--r--   0        0        0     1985 2023-01-27 00:43:56.396285 indieweb_rocks-0.0.2/indieweb_rocks/static/cc/nc.svg
--rw-r--r--   0        0        0     1304 2023-01-27 00:43:56.396285 indieweb_rocks-0.0.2/indieweb_rocks/static/cc/nd.svg
--rw-r--r--   0        0        0     1959 2023-01-27 00:43:56.404286 indieweb_rocks-0.0.2/indieweb_rocks/static/cc/pd.svg
--rw-r--r--   0        0        0     1647 2023-01-27 00:43:56.404286 indieweb_rocks-0.0.2/indieweb_rocks/static/cc/remix.svg
--rw-r--r--   0        0        0     1801 2023-01-27 00:43:56.404286 indieweb_rocks-0.0.2/indieweb_rocks/static/cc/sa.svg
--rw-r--r--   0        0        0     2902 2023-01-27 00:43:56.400285 indieweb_rocks-0.0.2/indieweb_rocks/static/cc/sampling.plus.svg
--rw-r--r--   0        0        0     3304 2023-01-27 00:43:56.408285 indieweb_rocks-0.0.2/indieweb_rocks/static/cc/sampling.svg
--rw-r--r--   0        0        0     1891 2023-01-27 00:43:56.400285 indieweb_rocks-0.0.2/indieweb_rocks/static/cc/share.svg
--rw-r--r--   0        0        0     2210 2023-01-27 00:43:56.400285 indieweb_rocks-0.0.2/indieweb_rocks/static/cc/zero.svg
--rw-r--r--   0        0        0     7406 2023-01-27 00:43:56.396285 indieweb_rocks-0.0.2/indieweb_rocks/static/favicon.ico
--rw-r--r--   0        0        0    12004 2023-01-27 00:43:56.408285 indieweb_rocks-0.0.2/indieweb_rocks/static/microformats.png
--rw-r--r--   0        0        0     2437 2023-01-27 00:43:56.408285 indieweb_rocks-0.0.2/indieweb_rocks/static/screen.css
--rw-r--r--   0        0        0     1493 2023-01-27 00:43:56.420286 indieweb_rocks-0.0.2/indieweb_rocks/templates/__init__.py
--rw-r--r--   0        0        0      871 2023-01-27 00:43:56.436286 indieweb_rocks-0.0.2/indieweb_rocks/templates/a11y.html
--rw-r--r--   0        0        0      346 2023-08-01 22:40:18.444018 indieweb_rocks-0.0.2/indieweb_rocks/templates/about.html
--rw-r--r--   0        0        0      279 2023-01-27 00:43:56.424286 indieweb_rocks-0.0.2/indieweb_rocks/templates/categories.html
--rw-r--r--   0        0        0      147 2023-01-27 00:43:56.428286 indieweb_rocks-0.0.2/indieweb_rocks/templates/commons.html
--rw-r--r--   0        0        0       51 2023-01-27 00:43:56.428286 indieweb_rocks-0.0.2/indieweb_rocks/templates/crawl_enqueued.html
--rw-r--r--   0        0        0      310 2023-01-27 00:43:56.428286 indieweb_rocks-0.0.2/indieweb_rocks/templates/crawler.html
--rw-r--r--   0        0        0       81 2023-01-27 00:43:56.416286 indieweb_rocks-0.0.2/indieweb_rocks/templates/domain_suffix_does_not_exist.html
--rw-r--r--   0        0        0      277 2023-01-27 00:43:56.412286 indieweb_rocks-0.0.2/indieweb_rocks/templates/faq.html
--rw-r--r--   0        0        0      157 2023-01-27 00:43:56.416286 indieweb_rocks-0.0.2/indieweb_rocks/templates/featured.html
--rw-r--r--   0        0        0       84 2023-01-27 00:43:56.412286 indieweb_rocks-0.0.2/indieweb_rocks/templates/features.html
--rw-r--r--   0        0        0      623 2023-01-27 00:43:56.412286 indieweb_rocks-0.0.2/indieweb_rocks/templates/indieauth.html
--rw-r--r--   0        0        0     5234 2023-07-28 01:03:35.446929 indieweb_rocks-0.0.2/indieweb_rocks/templates/landing.html
--rw-r--r--   0        0        0     1555 2023-01-27 00:43:56.432286 indieweb_rocks-0.0.2/indieweb_rocks/templates/map.html
--rw-r--r--   0        0        0       29 2023-01-27 00:43:56.440286 indieweb_rocks-0.0.2/indieweb_rocks/templates/page.html
--rw-r--r--   0        0        0      439 2023-01-27 00:43:56.436286 indieweb_rocks-0.0.2/indieweb_rocks/templates/people.html
--rw-r--r--   0        0        0       86 2023-01-27 00:43:56.424286 indieweb_rocks-0.0.2/indieweb_rocks/templates/posts.html
--rw-r--r--   0        0        0       40 2023-01-27 00:43:56.420286 indieweb_rocks-0.0.2/indieweb_rocks/templates/privacy.html
--rw-r--r--   0        0        0      267 2023-08-02 01:55:27.257599 indieweb_rocks-0.0.2/indieweb_rocks/templates/results.html
--rw-r--r--   0        0        0      232 2023-01-27 00:43:56.432286 indieweb_rocks-0.0.2/indieweb_rocks/templates/screens.html
--rw-r--r--   0        0        0      724 2023-01-27 00:43:56.424286 indieweb_rocks-0.0.2/indieweb_rocks/templates/silo.html
--rw-r--r--   0        0        0      326 2023-01-27 00:43:56.428286 indieweb_rocks-0.0.2/indieweb_rocks/templates/silos.html
--rw-r--r--   0        0        0    25694 2023-07-28 01:15:27.823266 indieweb_rocks-0.0.2/indieweb_rocks/templates/site.html
--rw-r--r--   0        0        0       94 2023-01-27 00:43:56.428286 indieweb_rocks-0.0.2/indieweb_rocks/templates/site_not_responding.html
--rw-r--r--   0        0        0      363 2023-01-27 00:43:56.436286 indieweb_rocks-0.0.2/indieweb_rocks/templates/sites.html
--rw-r--r--   0        0        0       59 2023-01-27 00:43:56.424286 indieweb_rocks-0.0.2/indieweb_rocks/templates/stats.html
--rw-r--r--   0        0        0     2103 2023-08-01 22:51:48.378265 indieweb_rocks-0.0.2/indieweb_rocks/templates/template.html
--rw-r--r--   0        0        0       42 2023-01-27 00:43:56.416286 indieweb_rocks-0.0.2/indieweb_rocks/templates/terms.html
--rw-r--r--   0        0        0     2547 2023-01-27 00:43:56.420286 indieweb_rocks-0.0.2/indieweb_rocks/templates/the_street.html
--rw-r--r--   0        0        0      106 2023-01-27 00:43:56.432286 indieweb_rocks-0.0.2/indieweb_rocks/templates/toolbox/representative_card.html
--rw-r--r--   0        0        0      106 2023-01-27 00:43:56.432286 indieweb_rocks-0.0.2/indieweb_rocks/templates/toolbox/representative_feed.html
--rw-r--r--   0        0        0     4101 2023-01-27 00:43:56.412286 indieweb_rocks-0.0.2/indieweb_rocks/utils.py
--rw-r--r--   0        0        0     1352 2023-08-02 03:32:01.901665 indieweb_rocks-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1119 1970-01-01 00:00:00.000000 indieweb_rocks-0.0.2/setup.py
--rw-r--r--   0        0        0      772 1970-01-01 00:00:00.000000 indieweb_rocks-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    18992 2023-08-02 00:07:18.037441 indieweb_rocks-0.0.3/indieweb_rocks/__init__.py
+-rw-r--r--   0        0        0    13024 2023-08-02 03:18:39.694204 indieweb_rocks-0.0.3/indieweb_rocks/__web__.py
+-rw-r--r--   0        0        0     1563 2023-01-27 00:43:56.404286 indieweb_rocks-0.0.3/indieweb_rocks/static/cc/by.svg
+-rw-r--r--   0        0        0     2573 2023-01-27 00:43:56.404286 indieweb_rocks-0.0.3/indieweb_rocks/static/cc/cc.svg
+-rw-r--r--   0        0        0     1955 2023-01-27 00:43:56.396285 indieweb_rocks-0.0.3/indieweb_rocks/static/cc/nc-eu.svg
+-rw-r--r--   0        0        0     1537 2023-01-27 00:43:56.400285 indieweb_rocks-0.0.3/indieweb_rocks/static/cc/nc-jp.svg
+-rw-r--r--   0        0        0     1985 2023-01-27 00:43:56.396285 indieweb_rocks-0.0.3/indieweb_rocks/static/cc/nc.svg
+-rw-r--r--   0        0        0     1304 2023-01-27 00:43:56.396285 indieweb_rocks-0.0.3/indieweb_rocks/static/cc/nd.svg
+-rw-r--r--   0        0        0     1959 2023-01-27 00:43:56.404286 indieweb_rocks-0.0.3/indieweb_rocks/static/cc/pd.svg
+-rw-r--r--   0        0        0     1647 2023-01-27 00:43:56.404286 indieweb_rocks-0.0.3/indieweb_rocks/static/cc/remix.svg
+-rw-r--r--   0        0        0     1801 2023-01-27 00:43:56.404286 indieweb_rocks-0.0.3/indieweb_rocks/static/cc/sa.svg
+-rw-r--r--   0        0        0     2902 2023-01-27 00:43:56.400285 indieweb_rocks-0.0.3/indieweb_rocks/static/cc/sampling.plus.svg
+-rw-r--r--   0        0        0     3304 2023-01-27 00:43:56.408285 indieweb_rocks-0.0.3/indieweb_rocks/static/cc/sampling.svg
+-rw-r--r--   0        0        0     1891 2023-01-27 00:43:56.400285 indieweb_rocks-0.0.3/indieweb_rocks/static/cc/share.svg
+-rw-r--r--   0        0        0     2210 2023-01-27 00:43:56.400285 indieweb_rocks-0.0.3/indieweb_rocks/static/cc/zero.svg
+-rw-r--r--   0        0        0     7406 2023-01-27 00:43:56.396285 indieweb_rocks-0.0.3/indieweb_rocks/static/favicon.ico
+-rw-r--r--   0        0        0    12004 2023-01-27 00:43:56.408285 indieweb_rocks-0.0.3/indieweb_rocks/static/microformats.png
+-rw-r--r--   0        0        0     2437 2023-01-27 00:43:56.408285 indieweb_rocks-0.0.3/indieweb_rocks/static/screen.css
+-rw-r--r--   0        0        0     1493 2023-01-27 00:43:56.420286 indieweb_rocks-0.0.3/indieweb_rocks/templates/__init__.py
+-rw-r--r--   0        0        0      871 2023-01-27 00:43:56.436286 indieweb_rocks-0.0.3/indieweb_rocks/templates/a11y.html
+-rw-r--r--   0        0        0      346 2023-08-01 22:40:18.444018 indieweb_rocks-0.0.3/indieweb_rocks/templates/about.html
+-rw-r--r--   0        0        0      279 2023-01-27 00:43:56.424286 indieweb_rocks-0.0.3/indieweb_rocks/templates/categories.html
+-rw-r--r--   0        0        0      147 2023-01-27 00:43:56.428286 indieweb_rocks-0.0.3/indieweb_rocks/templates/commons.html
+-rw-r--r--   0        0        0       51 2023-01-27 00:43:56.428286 indieweb_rocks-0.0.3/indieweb_rocks/templates/crawl_enqueued.html
+-rw-r--r--   0        0        0      310 2023-01-27 00:43:56.428286 indieweb_rocks-0.0.3/indieweb_rocks/templates/crawler.html
+-rw-r--r--   0        0        0       81 2023-01-27 00:43:56.416286 indieweb_rocks-0.0.3/indieweb_rocks/templates/domain_suffix_does_not_exist.html
+-rw-r--r--   0        0        0      277 2023-01-27 00:43:56.412286 indieweb_rocks-0.0.3/indieweb_rocks/templates/faq.html
+-rw-r--r--   0        0        0      157 2023-01-27 00:43:56.416286 indieweb_rocks-0.0.3/indieweb_rocks/templates/featured.html
+-rw-r--r--   0        0        0       84 2023-01-27 00:43:56.412286 indieweb_rocks-0.0.3/indieweb_rocks/templates/features.html
+-rw-r--r--   0        0        0      623 2023-01-27 00:43:56.412286 indieweb_rocks-0.0.3/indieweb_rocks/templates/indieauth.html
+-rw-r--r--   0        0        0     5234 2023-07-28 01:03:35.446929 indieweb_rocks-0.0.3/indieweb_rocks/templates/landing.html
+-rw-r--r--   0        0        0     1555 2023-01-27 00:43:56.432286 indieweb_rocks-0.0.3/indieweb_rocks/templates/map.html
+-rw-r--r--   0        0        0       29 2023-01-27 00:43:56.440286 indieweb_rocks-0.0.3/indieweb_rocks/templates/page.html
+-rw-r--r--   0        0        0      439 2023-01-27 00:43:56.436286 indieweb_rocks-0.0.3/indieweb_rocks/templates/people.html
+-rw-r--r--   0        0        0       86 2023-01-27 00:43:56.424286 indieweb_rocks-0.0.3/indieweb_rocks/templates/posts.html
+-rw-r--r--   0        0        0       40 2023-01-27 00:43:56.420286 indieweb_rocks-0.0.3/indieweb_rocks/templates/privacy.html
+-rw-r--r--   0        0        0      267 2023-08-02 01:55:27.257599 indieweb_rocks-0.0.3/indieweb_rocks/templates/results.html
+-rw-r--r--   0        0        0      232 2023-01-27 00:43:56.432286 indieweb_rocks-0.0.3/indieweb_rocks/templates/screens.html
+-rw-r--r--   0        0        0      724 2023-01-27 00:43:56.424286 indieweb_rocks-0.0.3/indieweb_rocks/templates/silo.html
+-rw-r--r--   0        0        0      326 2023-01-27 00:43:56.428286 indieweb_rocks-0.0.3/indieweb_rocks/templates/silos.html
+-rw-r--r--   0        0        0    25694 2023-07-28 01:15:27.823266 indieweb_rocks-0.0.3/indieweb_rocks/templates/site.html
+-rw-r--r--   0        0        0       94 2023-01-27 00:43:56.428286 indieweb_rocks-0.0.3/indieweb_rocks/templates/site_not_responding.html
+-rw-r--r--   0        0        0      363 2023-01-27 00:43:56.436286 indieweb_rocks-0.0.3/indieweb_rocks/templates/sites.html
+-rw-r--r--   0        0        0       59 2023-01-27 00:43:56.424286 indieweb_rocks-0.0.3/indieweb_rocks/templates/stats.html
+-rw-r--r--   0        0        0     2103 2023-08-01 22:51:48.378265 indieweb_rocks-0.0.3/indieweb_rocks/templates/template.html
+-rw-r--r--   0        0        0       42 2023-01-27 00:43:56.416286 indieweb_rocks-0.0.3/indieweb_rocks/templates/terms.html
+-rw-r--r--   0        0        0     2547 2023-01-27 00:43:56.420286 indieweb_rocks-0.0.3/indieweb_rocks/templates/the_street.html
+-rw-r--r--   0        0        0      106 2023-01-27 00:43:56.432286 indieweb_rocks-0.0.3/indieweb_rocks/templates/toolbox/representative_card.html
+-rw-r--r--   0        0        0      106 2023-01-27 00:43:56.432286 indieweb_rocks-0.0.3/indieweb_rocks/templates/toolbox/representative_feed.html
+-rw-r--r--   0        0        0     4101 2023-01-27 00:43:56.412286 indieweb_rocks-0.0.3/indieweb_rocks/utils.py
+-rw-r--r--   0        0        0     1352 2023-08-02 03:46:03.319342 indieweb_rocks-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1119 1970-01-01 00:00:00.000000 indieweb_rocks-0.0.3/setup.py
+-rw-r--r--   0        0        0      772 1970-01-01 00:00:00.000000 indieweb_rocks-0.0.3/PKG-INFO
```

### Comparing `indieweb_rocks-0.0.2/indieweb_rocks/__init__.py` & `indieweb_rocks-0.0.3/indieweb_rocks/__init__.py`

 * *Files identical despite different names*

### Comparing `indieweb_rocks-0.0.2/indieweb_rocks/__web__.py` & `indieweb_rocks-0.0.3/indieweb_rocks/__web__.py`

 * *Files identical despite different names*

### Comparing `indieweb_rocks-0.0.2/indieweb_rocks/static/cc/by.svg` & `indieweb_rocks-0.0.3/indieweb_rocks/static/cc/by.svg`

 * *Files identical despite different names*

### Comparing `indieweb_rocks-0.0.2/indieweb_rocks/static/cc/cc.svg` & `indieweb_rocks-0.0.3/indieweb_rocks/static/cc/cc.svg`

 * *Files identical despite different names*

### Comparing `indieweb_rocks-0.0.2/indieweb_rocks/static/cc/nc-eu.svg` & `indieweb_rocks-0.0.3/indieweb_rocks/static/cc/nc-eu.svg`

 * *Files identical despite different names*

### Comparing `indieweb_rocks-0.0.2/indieweb_rocks/static/cc/nc-jp.svg` & `indieweb_rocks-0.0.3/indieweb_rocks/static/cc/nc-jp.svg`

 * *Files identical despite different names*

### Comparing `indieweb_rocks-0.0.2/indieweb_rocks/static/cc/nc.svg` & `indieweb_rocks-0.0.3/indieweb_rocks/static/cc/nc.svg`

 * *Files identical despite different names*

### Comparing `indieweb_rocks-0.0.2/indieweb_rocks/static/cc/nd.svg` & `indieweb_rocks-0.0.3/indieweb_rocks/static/cc/nd.svg`

 * *Files identical despite different names*

### Comparing `indieweb_rocks-0.0.2/indieweb_rocks/static/cc/pd.svg` & `indieweb_rocks-0.0.3/indieweb_rocks/static/cc/pd.svg`

 * *Files identical despite different names*

### Comparing `indieweb_rocks-0.0.2/indieweb_rocks/static/cc/remix.svg` & `indieweb_rocks-0.0.3/indieweb_rocks/static/cc/remix.svg`

 * *Files identical despite different names*

### Comparing `indieweb_rocks-0.0.2/indieweb_rocks/static/cc/sa.svg` & `indieweb_rocks-0.0.3/indieweb_rocks/static/cc/sa.svg`

 * *Files identical despite different names*

### Comparing `indieweb_rocks-0.0.2/indieweb_rocks/static/cc/sampling.plus.svg` & `indieweb_rocks-0.0.3/indieweb_rocks/static/cc/sampling.plus.svg`

 * *Files identical despite different names*

### Comparing `indieweb_rocks-0.0.2/indieweb_rocks/static/cc/sampling.svg` & `indieweb_rocks-0.0.3/indieweb_rocks/static/cc/sampling.svg`

 * *Files identical despite different names*

### Comparing `indieweb_rocks-0.0.2/indieweb_rocks/static/cc/share.svg` & `indieweb_rocks-0.0.3/indieweb_rocks/static/cc/share.svg`

 * *Files identical despite different names*

### Comparing `indieweb_rocks-0.0.2/indieweb_rocks/static/cc/zero.svg` & `indieweb_rocks-0.0.3/indieweb_rocks/static/cc/zero.svg`

 * *Files identical despite different names*

### Comparing `indieweb_rocks-0.0.2/indieweb_rocks/static/favicon.ico` & `indieweb_rocks-0.0.3/indieweb_rocks/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `indieweb_rocks-0.0.2/indieweb_rocks/static/microformats.png` & `indieweb_rocks-0.0.3/indieweb_rocks/static/microformats.png`

 * *Files identical despite different names*

### Comparing `indieweb_rocks-0.0.2/indieweb_rocks/static/screen.css` & `indieweb_rocks-0.0.3/indieweb_rocks/static/screen.css`

 * *Files identical despite different names*

### Comparing `indieweb_rocks-0.0.2/indieweb_rocks/templates/__init__.py` & `indieweb_rocks-0.0.3/indieweb_rocks/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `indieweb_rocks-0.0.2/indieweb_rocks/templates/a11y.html` & `indieweb_rocks-0.0.3/indieweb_rocks/templates/a11y.html`

 * *Files identical despite different names*

### Comparing `indieweb_rocks-0.0.2/indieweb_rocks/templates/indieauth.html` & `indieweb_rocks-0.0.3/indieweb_rocks/templates/indieauth.html`

 * *Files identical despite different names*

### Comparing `indieweb_rocks-0.0.2/indieweb_rocks/templates/landing.html` & `indieweb_rocks-0.0.3/indieweb_rocks/templates/landing.html`

 * *Files identical despite different names*

### Comparing `indieweb_rocks-0.0.2/indieweb_rocks/templates/map.html` & `indieweb_rocks-0.0.3/indieweb_rocks/templates/map.html`

 * *Files identical despite different names*

### Comparing `indieweb_rocks-0.0.2/indieweb_rocks/templates/silo.html` & `indieweb_rocks-0.0.3/indieweb_rocks/templates/silo.html`

 * *Files identical despite different names*

### Comparing `indieweb_rocks-0.0.2/indieweb_rocks/templates/site.html` & `indieweb_rocks-0.0.3/indieweb_rocks/templates/site.html`

 * *Files identical despite different names*

### Comparing `indieweb_rocks-0.0.2/indieweb_rocks/templates/template.html` & `indieweb_rocks-0.0.3/indieweb_rocks/templates/template.html`

 * *Files identical despite different names*

### Comparing `indieweb_rocks-0.0.2/indieweb_rocks/templates/the_street.html` & `indieweb_rocks-0.0.3/indieweb_rocks/templates/the_street.html`

 * *Files identical despite different names*

### Comparing `indieweb_rocks-0.0.2/indieweb_rocks/utils.py` & `indieweb_rocks-0.0.3/indieweb_rocks/utils.py`

 * *Files identical despite different names*

### Comparing `indieweb_rocks-0.0.2/pyproject.toml` & `indieweb_rocks-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "indieweb.rocks"
-version = "0.0.2"
+version = "0.0.3"
 description = "directory/validator of personal websites"
 authors = ["Angelo Gladding <angelo@ragt.ag>"]
 license = "0BSD"
 
 [tool.poetry.plugins."websites"]
 indieweb_rocks = "indieweb_rocks.__web__:app"
```

### Comparing `indieweb_rocks-0.0.2/setup.py` & `indieweb_rocks-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
  'webint>=0.0']
 
 entry_points = \
 {'websites': ['indieweb_rocks = indieweb_rocks.__web__:app']}
 
 setup_kwargs = {
     'name': 'indieweb-rocks',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': 'directory/validator of personal websites',
     'long_description': 'None',
     'author': 'Angelo Gladding',
     'author_email': 'angelo@ragt.ag',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `indieweb_rocks-0.0.2/PKG-INFO` & `indieweb_rocks-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indieweb-rocks
-Version: 0.0.2
+Version: 0.0.3
 Summary: directory/validator of personal websites
 License: 0BSD
 Author: Angelo Gladding
 Author-email: angelo@ragt.ag
 Requires-Python: >=3.10,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

