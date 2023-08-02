# Comparing `tmp/cubicweb-tag-2.0.0.tar.gz` & `tmp/cubicweb-tag-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-tag-2.0.0.tar", last modified: Sat Nov 26 00:05:49 2022, max compression
+gzip compressed data, was "cubicweb-tag-3.0.0.tar", last modified: Wed Aug  2 13:43:32 2023, max compression
```

## Comparing `cubicweb-tag-2.0.0.tar` & `cubicweb-tag-3.0.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 00:05:49.283548 cubicweb-tag-2.0.0/
--rw-rw-rw-   0 root         (0) root         (0)      425 2022-11-26 00:05:34.000000 cubicweb-tag-2.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2865 2022-11-26 00:05:49.283548 cubicweb-tag-2.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2435 2022-11-26 00:05:34.000000 cubicweb-tag-2.0.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 00:05:49.279548 cubicweb-tag-2.0.0/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-11-26 00:05:34.000000 cubicweb-tag-2.0.0/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      652 2022-11-26 00:05:34.000000 cubicweb-tag-2.0.0/cubicweb_tag/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 00:05:49.283548 cubicweb-tag-2.0.0/cubicweb_tag/data/
--rw-rw-rw-   0 root         (0) root         (0)     2016 2022-11-26 00:05:34.000000 cubicweb-tag-2.0.0/cubicweb_tag/data/cubes.tag.merge.js
--rw-rw-rw-   0 root         (0) root         (0)     2092 2022-11-26 00:05:34.000000 cubicweb-tag-2.0.0/cubicweb_tag/data/jquery.tagcloud.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 00:05:49.283548 cubicweb-tag-2.0.0/cubicweb_tag/doc/
--rw-rw-rw-   0 root         (0) root         (0)    10378 2022-11-26 00:05:34.000000 cubicweb-tag-2.0.0/cubicweb_tag/doc/screenshot_tags_box.png
--rw-rw-rw-   0 root         (0) root         (0)    21382 2022-11-26 00:05:34.000000 cubicweb-tag-2.0.0/cubicweb_tag/doc/screenshot_tags_cloud_box.png
--rw-rw-rw-   0 root         (0) root         (0)      735 2022-11-26 00:05:34.000000 cubicweb-tag-2.0.0/cubicweb_tag/entities.py
--rw-rw-rw-   0 root         (0) root         (0)      812 2022-11-26 00:05:34.000000 cubicweb-tag-2.0.0/cubicweb_tag/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 00:05:49.283548 cubicweb-tag-2.0.0/cubicweb_tag/i18n/
--rw-rw-rw-   0 root         (0) root         (0)     3300 2022-11-26 00:05:34.000000 cubicweb-tag-2.0.0/cubicweb_tag/i18n/en.po
--rw-rw-rw-   0 root         (0) root         (0)     4214 2022-11-26 00:05:34.000000 cubicweb-tag-2.0.0/cubicweb_tag/i18n/fr.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 00:05:49.283548 cubicweb-tag-2.0.0/cubicweb_tag/migration/
--rw-rw-rw-   0 root         (0) root         (0)       43 2022-11-26 00:05:34.000000 cubicweb-tag-2.0.0/cubicweb_tag/migration/1.0.2_Any.py
--rw-rw-rw-   0 root         (0) root         (0)       66 2022-11-26 00:05:34.000000 cubicweb-tag-2.0.0/cubicweb_tag/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)      667 2022-11-26 00:05:34.000000 cubicweb-tag-2.0.0/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)    11706 2022-11-26 00:05:34.000000 cubicweb-tag-2.0.0/cubicweb_tag/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 00:05:49.283548 cubicweb-tag-2.0.0/cubicweb_tag.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2865 2022-11-26 00:05:48.000000 cubicweb-tag-2.0.0/cubicweb_tag.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      802 2022-11-26 00:05:49.000000 cubicweb-tag-2.0.0/cubicweb_tag.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-26 00:05:48.000000 cubicweb-tag-2.0.0/cubicweb_tag.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       36 2022-11-26 00:05:48.000000 cubicweb-tag-2.0.0/cubicweb_tag.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-26 00:05:48.000000 cubicweb-tag-2.0.0/cubicweb_tag.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       25 2022-11-26 00:05:49.000000 cubicweb-tag-2.0.0/cubicweb_tag.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-11-26 00:05:49.000000 cubicweb-tag-2.0.0/cubicweb_tag.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-26 00:05:49.283548 cubicweb-tag-2.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2606 2022-11-26 00:05:34.000000 cubicweb-tag-2.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 00:05:49.283548 cubicweb-tag-2.0.0/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 00:05:49.283548 cubicweb-tag-2.0.0/test/data/
--rw-rw-rw-   0 root         (0) root         (0)        9 2022-11-26 00:05:34.000000 cubicweb-tag-2.0.0/test/data/bootstrap_cubes
--rw-rw-rw-   0 root         (0) root         (0)      137 2022-11-26 00:05:34.000000 cubicweb-tag-2.0.0/test/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1421 2022-11-26 00:05:34.000000 cubicweb-tag-2.0.0/test/unittest_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     3819 2022-11-26 00:05:34.000000 cubicweb-tag-2.0.0/test/unittest_tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 13:43:32.928487 cubicweb-tag-3.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      425 2023-08-02 13:43:11.000000 cubicweb-tag-3.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2845 2023-08-02 13:43:32.924487 cubicweb-tag-3.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2435 2023-08-02 13:43:11.000000 cubicweb-tag-3.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 13:43:32.916487 cubicweb-tag-3.0.0/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)       19 2023-08-02 13:43:11.000000 cubicweb-tag-3.0.0/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      655 2023-08-02 13:43:11.000000 cubicweb-tag-3.0.0/cubicweb_tag/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 13:43:32.920487 cubicweb-tag-3.0.0/cubicweb_tag/data/
+-rw-rw-rw-   0 root         (0) root         (0)     2016 2023-08-02 13:43:11.000000 cubicweb-tag-3.0.0/cubicweb_tag/data/cubes.tag.merge.js
+-rw-rw-rw-   0 root         (0) root         (0)     2092 2023-08-02 13:43:11.000000 cubicweb-tag-3.0.0/cubicweb_tag/data/jquery.tagcloud.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 13:43:32.920487 cubicweb-tag-3.0.0/cubicweb_tag/doc/
+-rw-rw-rw-   0 root         (0) root         (0)    10378 2023-08-02 13:43:11.000000 cubicweb-tag-3.0.0/cubicweb_tag/doc/screenshot_tags_box.png
+-rw-rw-rw-   0 root         (0) root         (0)    21382 2023-08-02 13:43:11.000000 cubicweb-tag-3.0.0/cubicweb_tag/doc/screenshot_tags_cloud_box.png
+-rw-rw-rw-   0 root         (0) root         (0)      711 2023-08-02 13:43:11.000000 cubicweb-tag-3.0.0/cubicweb_tag/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      835 2023-08-02 13:43:11.000000 cubicweb-tag-3.0.0/cubicweb_tag/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 13:43:32.920487 cubicweb-tag-3.0.0/cubicweb_tag/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)     3300 2023-08-02 13:43:11.000000 cubicweb-tag-3.0.0/cubicweb_tag/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)     4214 2023-08-02 13:43:11.000000 cubicweb-tag-3.0.0/cubicweb_tag/i18n/fr.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 13:43:32.924487 cubicweb-tag-3.0.0/cubicweb_tag/migration/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-08-02 13:43:11.000000 cubicweb-tag-3.0.0/cubicweb_tag/migration/1.0.2_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       65 2023-08-02 13:43:11.000000 cubicweb-tag-3.0.0/cubicweb_tag/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)      649 2023-08-02 13:43:11.000000 cubicweb-tag-3.0.0/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    11667 2023-08-02 13:43:11.000000 cubicweb-tag-3.0.0/cubicweb_tag/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 13:43:32.920487 cubicweb-tag-3.0.0/cubicweb_tag.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2845 2023-08-02 13:43:32.000000 cubicweb-tag-3.0.0/cubicweb_tag.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      802 2023-08-02 13:43:32.000000 cubicweb-tag-3.0.0/cubicweb_tag.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 13:43:32.000000 cubicweb-tag-3.0.0/cubicweb_tag.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-08-02 13:43:32.000000 cubicweb-tag-3.0.0/cubicweb_tag.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 13:43:32.000000 cubicweb-tag-3.0.0/cubicweb_tag.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       50 2023-08-02 13:43:32.000000 cubicweb-tag-3.0.0/cubicweb_tag.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-02 13:43:32.000000 cubicweb-tag-3.0.0/cubicweb_tag.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-02 13:43:32.928487 cubicweb-tag-3.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2573 2023-08-02 13:43:11.000000 cubicweb-tag-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 13:43:32.924487 cubicweb-tag-3.0.0/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 13:43:32.924487 cubicweb-tag-3.0.0/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-08-02 13:43:11.000000 cubicweb-tag-3.0.0/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-08-02 13:43:11.000000 cubicweb-tag-3.0.0/test/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1411 2023-08-02 13:43:11.000000 cubicweb-tag-3.0.0/test/unittest_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     3943 2023-08-02 13:43:11.000000 cubicweb-tag-3.0.0/test/unittest_tag.py
```

### Comparing `cubicweb-tag-2.0.0/PKG-INFO` & `cubicweb-tag-3.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cubicweb-tag
-Version: 2.0.0
+Version: 3.0.0
 Summary: tag component for the CubicWeb framework
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-tag
 Author: Logilab
 Author-email: contact@logilab.fr
 License: LGPL
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: JavaScript
 
 Summary
 -------
@@ -85,9 +84,7 @@
   different words, or spelling.
 
 Documentation
 -------------
 
 Look in the ``doc/`` subdirectory or read
 http://www.cubicweb.org/doc/en/
-
-
```

### Comparing `cubicweb-tag-2.0.0/README.rst` & `cubicweb-tag-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-tag-2.0.0/cubicweb_tag/data/cubes.tag.merge.js` & `cubicweb-tag-3.0.0/cubicweb_tag/data/cubes.tag.merge.js`

 * *Files identical despite different names*

### Comparing `cubicweb-tag-2.0.0/cubicweb_tag/data/jquery.tagcloud.js` & `cubicweb-tag-3.0.0/cubicweb_tag/data/jquery.tagcloud.js`

 * *Files identical despite different names*

### Comparing `cubicweb-tag-2.0.0/cubicweb_tag/doc/screenshot_tags_box.png` & `cubicweb-tag-3.0.0/cubicweb_tag/doc/screenshot_tags_box.png`

 * *Files identical despite different names*

### Comparing `cubicweb-tag-2.0.0/cubicweb_tag/doc/screenshot_tags_cloud_box.png` & `cubicweb-tag-3.0.0/cubicweb_tag/doc/screenshot_tags_cloud_box.png`

 * *Files identical despite different names*

### Comparing `cubicweb-tag-2.0.0/cubicweb_tag/entities.py` & `cubicweb-tag-3.0.0/cubicweb_tag/entities.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,19 @@
 __docformat__ = "restructuredtext en"
 
 from cubicweb.entities import AnyEntity, fetch_config
 
 
 class Tag(AnyEntity):
     """customized class for Tag entities"""
-    __regid__ = 'Tag'
-    fetch_attrs, cw_fetch_order = fetch_config(['name'])
+
+    __regid__ = "Tag"
+    fetch_attrs, cw_fetch_order = fetch_config(["name"])
 
     def closest_tags_rset(self):
-        return self._cw.execute('Any CT, COUNT(X) GROUPBY CT ORDERBY 2 DESC '
-                                'LIMIT 5 '
-                                'WHERE T tags X, T eid %(x)s, CT tags X, '
-                                'NOT CT eid %(x)s', {'x': self.eid})
+        return self._cw.execute(
+            "Any CT, COUNT(X) GROUPBY CT ORDERBY 2 DESC "
+            "LIMIT 5 "
+            "WHERE T tags X, T eid %(x)s, CT tags X, "
+            "NOT CT eid %(x)s",
+            {"x": self.eid},
+        )
```

### Comparing `cubicweb-tag-2.0.0/cubicweb_tag/i18n/en.po` & `cubicweb-tag-3.0.0/cubicweb_tag/i18n/en.po`

 * *Files identical despite different names*

### Comparing `cubicweb-tag-2.0.0/cubicweb_tag/i18n/fr.po` & `cubicweb-tag-3.0.0/cubicweb_tag/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `cubicweb-tag-2.0.0/cubicweb_tag/schema.py` & `cubicweb-tag-3.0.0/cubicweb_tag/schema.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-
 from cubicweb import _
 
 from yams.buildobjs import EntityType, String, SubjectRelation, RelationType
 
 
 class Tag(EntityType):
     """tags are used by users to mark entities.
     When you include the Tag entity, all application specific entities
     may then be tagged using the "tags" relation.
     """
-    name = String(required=True, fulltextindexed=True, unique=True,
-                  maxsize=128)
+
+    name = String(required=True, fulltextindexed=True, unique=True, maxsize=128)
     # when using this component, add the Tag tag X relation for each type that
     # should be taggeable
-    tags = SubjectRelation('Tag', description=_("tagged objects"))
+    tags = SubjectRelation("Tag", description=_("tagged objects"))
 
 
 class tags(RelationType):
     """indicates that an entity is classified by a given tag"""
```

### Comparing `cubicweb-tag-2.0.0/cubicweb_tag/views.py` & `cubicweb-tag-3.0.0/cubicweb_tag/views.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,298 +7,349 @@
 __docformat__ = "restructuredtext en"
 
 
 from cubicweb import _
 
 from logilab.mtconverter import xml_escape
 
-from cubicweb.predicates import (match_kwargs, match_form_params,
-                                 match_user_groups,
-                                 has_related_entities, one_etype_rset,
-                                 is_instance, relation_possible)
+from cubicweb.predicates import (
+    match_kwargs,
+    match_form_params,
+    match_user_groups,
+    has_related_entities,
+    one_etype_rset,
+    is_instance,
+    relation_possible,
+)
 from cubicweb import uilib, tags
 from cubicweb_web import stdmsgs, component, facet
 from cubicweb_web.views import baseviews, ajaxcontroller, xmlrss, uicfg
 
 
 _afs = uicfg.autoform_section
-_afs.tag_subject_of(('*', 'tags', '*'), formtype='main', section='hidden')
-_afs.tag_object_of(('*', 'tags', '*'), formtype='main', section='hidden')
+_afs.tag_subject_of(("*", "tags", "*"), formtype="main", section="hidden")
+_afs.tag_object_of(("*", "tags", "*"), formtype="main", section="hidden")
 
 # relations displayed by some component or box below, don't display them in
 # primary view
 _pvs = uicfg.primaryview_section
-_pvs.tag_subject_of(('*', 'tags', '*'), 'hidden')
-_pvs.tag_object_of(('*', 'tags', '*'), 'hidden')
-_pvs.tag_subject_of(('Tag', 'tags', '*'), 'relations')
-_pvs.tag_attribute(('Tag', 'name'), 'hidden')
+_pvs.tag_subject_of(("*", "tags", "*"), "hidden")
+_pvs.tag_object_of(("*", "tags", "*"), "hidden")
+_pvs.tag_subject_of(("Tag", "tags", "*"), "relations")
+_pvs.tag_attribute(("Tag", "name"), "hidden")
 
 
 class TagInContextView(baseviews.InContextView):
-    __regid__ = 'incontext'
-    __select__ = is_instance('Tag')
+    __regid__ = "incontext"
+    __select__ = is_instance("Tag")
 
     def cell_call(self, row, col):
         entity = self.cw_rset.get_entity(row, col)
-        self.w(tags.a(entity.view('textincontext'), href=entity.absolute_url(),
-                      title=uilib.cut(entity.dc_description(), 50), rel=u'tag'))
+        self.w(
+            tags.a(
+                entity.view("textincontext"),
+                href=entity.absolute_url(),
+                title=uilib.cut(entity.dc_description(), 50),
+                rel="tag",
+            )
+        )
 
 
 class TagCloudView(baseviews.OneLineView):
     """cloud view to make a link on tagged entities appearing more or less big
     according to the number of tagged entities
 
     expect a result set with tag eid in the first column and number of tagged
     objects in the second column.
     expect as well:
     * `maxsize` argument, the maximum number of tagged entities by a tag in the
       cloud
     * `etype` argument, the entity type we are filtering
     """
-    __regid__ = 'tagcloud'
-    __select__ = is_instance('Tag') & (match_kwargs('etype')
-                                       | match_form_params('etype'))
+
+    __regid__ = "tagcloud"
+    __select__ = is_instance("Tag") & (
+        match_kwargs("etype") | match_form_params("etype")
+    )
 
     need_navigation = False
     add_div_section = False  # configure View.call behaviour
 
-    onload_js = '''
+    onload_js = """
 jQuery(document).tagcloud.defaults = {
   size: {start: 0.8, end: 2.5, unit: "em"},
   color: {start: "#333", end: "#FF7700"}
 };
 jQuery("#tagcloud a").tagcloud();
-'''
+"""
 
     def call(self, *args, **kwargs):
-        self._cw.add_js('jquery.tagcloud.js')
+        self._cw.add_js("jquery.tagcloud.js")
         self._cw.html_headers.add_onload(self.onload_js)
-        self.w(u'<div id="tagcloud">')
-        super(TagCloudView, self).call(*args, **kwargs)
-        self.w(u'</div>')
+        self.w('<div id="tagcloud">')
+        super().call(*args, **kwargs)
+        self.w("</div>")
 
     def cell_call(self, row, col, etype=None, **kwargs):
         if etype is None:
-            etype = self._cw.form['etype']
+            etype = self._cw.form["etype"]
         entity = self.cw_rset.get_entity(row, col)
         mysize = self.cw_rset[row][1]
         # generate url according to where it is called from eg. when browsing
         # blogs the tag box should point to Blogs tagged by...
-        rql = 'Any X WHERE T tags X, T eid %s, X is %s' % (entity.eid, etype)
+        rql = f"Any X WHERE T tags X, T eid {entity.eid}, X is {etype}"
         # XXX rel=mysize, can't we set rel='tag %s' % mysize to get back the
         #     'tag' rel?
-        self.w(tags.a(entity.name, rel=mysize,
-                      href=self._cw.build_url('view', rql=rql)) + u' ')
+        self.w(
+            tags.a(entity.name, rel=mysize, href=self._cw.build_url("view", rql=rql))
+            + " "
+        )
 
 
 # simple boxes #################################################################
 
+
 class ClosestTagsBox(component.EntityCtxComponent):
-    __regid__ = 'closest_tags_box'
-    __select__ = component.EntityCtxComponent.__select__ & is_instance('Tag',)
+    __regid__ = "closest_tags_box"
+    __select__ = component.EntityCtxComponent.__select__ & is_instance(
+        "Tag",
+    )
     order = 25
-    title = _('closest tags')
+    title = _("closest tags")
 
     def init_rendering(self):
         self.closest_tags = self.entity.closest_tags_rset()
         if not self.closest_tags:
             raise component.EmptyComponent()
 
     def render_body(self, w):
-        self._cw.view('incontext', self.closest_tags, w=w)
+        self._cw.view("incontext", self.closest_tags, w=w)
 
 
 class SimilarityBox(component.EntityCtxComponent):
     """layout closest entities (ie. entities that share tags)"""
-    __regid__ = 'similarity_box'
-    __select__ = (component.EntityCtxComponent.__select__
-                  & has_related_entities('tags', 'object', 'Tag'))
+
+    __regid__ = "similarity_box"
+    __select__ = component.EntityCtxComponent.__select__ & has_related_entities(
+        "tags", "object", "Tag"
+    )
     order = 21
-    rql = ('Any Y,COUNT(T) GROUPBY Y ORDERBY 2 DESC %s '
-           'WHERE X eid %%(x)s, T tags X, T tags Y, NOT Y eid %%(x)s')
+    rql = (
+        "Any Y,COUNT(T) GROUPBY Y ORDERBY 2 DESC %s "
+        "WHERE X eid %%(x)s, T tags X, T tags Y, NOT Y eid %%(x)s"
+    )
 
     def init_rendering(self):
-        self.cw_rset = self._cw.execute(self.rql % ('LIMIT 5'),
-                                        {'x': self.entity.eid})
+        self.cw_rset = self._cw.execute(self.rql % ("LIMIT 5"), {"x": self.entity.eid})
         if not self.cw_rset:
             raise component.EmptyComponent()
 
     def render_title(self, w):
         if self.cw_rset.rowcount == 1:
-            w(self._cw._('similar entity'))
+            w(self._cw._("similar entity"))
         else:
-            w(self._cw._('similar entities'))
+            w(self._cw._("similar entities"))
 
     def render_body(self, w):
-        self._cw.view('outofcontext', self.cw_rset, w=w)
-        rql = self.rql % '' % {'x': self.entity.eid}
-        title = self._cw._('entities similar to %s') % self.entity.dc_title()
-        url = self._cw.build_url('view', rql=rql,
-                                 vtitle=title)
-        w(u'<div>[%s]</div>' % tags.a(self._cw._('see all'), href=url))
+        self._cw.view("outofcontext", self.cw_rset, w=w)
+        title = self._cw._("entities similar to %s") % self.entity.dc_title()
+        url = self._cw.build_url("view", rql=self.rql, vtitle=title)
+        w(f"<div>[{tags.a(self._cw._('see all'), href=url)}]</div>")
 
 
 class TagsCloudBox(component.CtxComponent):
-    """display a box with tag cloud for """
-    __regid__ = 'tagcloud_box'
-    __select__ = (component.CtxComponent.__select__ & one_etype_rset() &
-                  relation_possible('tags', 'object', 'Tag'))
+    """display a box with tag cloud for"""
+
+    __regid__ = "tagcloud_box"
+    __select__ = (
+        component.CtxComponent.__select__
+        & one_etype_rset()
+        & relation_possible("tags", "object", "Tag")
+    )
 
     visible = False  # disabled by default
     order = 30
-    title = _('Tag_plural')
-    context = 'left'
+    title = _("Tag_plural")
+    context = "left"
 
     def init_rendering(self):
         self.etype = next(iter(self.cw_rset.column_types(0)))
         self.cw_rset = self._cw.execute(
-            'Any T,COUNT(X),TN GROUPBY T,TN LIMIT 30'
-            'WHERE X is %s, T tags X, T name TN' % self.etype)
+            "Any T,COUNT(X),TN GROUPBY T,TN LIMIT 30"
+            "WHERE X is %s, T tags X, T name TN" % self.etype
+        )
         if not self.cw_rset:
             raise component.EmptyComponent()
 
     def render_body(self, w):
-        self._cw.view('tagcloud', self.cw_rset, etype=self.etype, w=w)
-        rql = ('Any T,COUNT(X),TN GROUPBY T,TN '
-               'WHERE X is %s, T tags X, T name TN' % self.etype)
-        url = xml_escape(self._cw.build_url(rql=rql, vid='tagcloud', etype=self.etype))
-        w(u'<div>[%s]</div>' % tags.a(self._cw._('see all tags'), href=url))
+        self._cw.view("tagcloud", self.cw_rset, etype=self.etype, w=w)
+        rql = (
+            "Any T,COUNT(X),TN GROUPBY T,TN "
+            "WHERE X is %s, T tags X, T name TN" % self.etype
+        )
+        url = xml_escape(self._cw.build_url(rql=rql, vid="tagcloud", etype=self.etype))
+        w(f"<div>[{tags.a(self._cw._('see all tags'), href=url)}]</div>")
 
 
 # the tags box #################################################################
 
+
 class TagsBox(component.AjaxEditRelationCtxComponent):
     """the tag box: control tag of taggeable entity providing an easy way to
     add/remove tag
     """
-    __regid__ = 'tags_box'
 
-    rtype = 'tags'
-    role = 'object'
-    target_etype = 'Tag'
+    __regid__ = "tags_box"
+
+    rtype = "tags"
+    role = "object"
+    target_etype = "Tag"
 
     order = 20
 
-    added_msg = _('entity has been tagged')
-    removed_msg = _('tag has been removed')
+    added_msg = _("entity has been tagged")
+    removed_msg = _("tag has been removed")
 
-    fname_vocabulary = 'unrelated_tags'
-    fname_validate = 'tag_entity'
-    fname_remove = 'untag_entity'
+    fname_vocabulary = "unrelated_tags"
+    fname_validate = "tag_entity"
+    fname_remove = "untag_entity"
 
 
-@ajaxcontroller.ajaxfunc(output_type='json')
+@ajaxcontroller.ajaxfunc(output_type="json")
 def unrelated_tags(self, eid):
     """return tag unrelated to an entity"""
-    rql = 'Any N ORDERBY N WHERE T is Tag, T name N, NOT T tags X, X eid %(x)s'
-    return [name for (name,) in self._cw.execute(rql, {'x': eid})]
+    rql = "Any N ORDERBY N WHERE T is Tag, T name N, NOT T tags X, X eid %(x)s"
+    return [name for (name,) in self._cw.execute(rql, {"x": eid})]
 
 
 @ajaxcontroller.ajaxfunc
 def tag_entity(self, eid, taglist):
     execute = self._cw.execute
     # get list of tag for this entity
-    tagged_by = set(tagname for (tagname,) in
-                    execute('Any N WHERE T name N, T tags X, X eid %(x)s',
-                            {'x': eid}))
+    tagged_by = {
+        tagname
+        for (tagname,) in execute(
+            "Any N WHERE T name N, T tags X, X eid %(x)s", {"x": eid}
+        )
+    }
     for tagname in taglist:
         tagname = tagname.strip()
         if not tagname or tagname in tagged_by:
             continue
-        tagrset = execute('Tag T WHERE T name %(name)s', {'name': tagname})
+        tagrset = execute("Tag T WHERE T name %(name)s", {"name": tagname})
         if tagrset:
-            rql = 'SET T tags X WHERE T eid %(t)s, X eid %(x)s'
-            execute(rql, {'t': tagrset[0][0], 'x': eid})
+            rql = "SET T tags X WHERE T eid %(t)s, X eid %(x)s"
+            execute(rql, {"t": tagrset[0][0], "x": eid})
         else:
-            rql = 'INSERT Tag T: T name %(name)s, T tags X WHERE X eid %(x)s'
-            execute(rql, {'name': tagname, 'x': eid})
+            rql = "INSERT Tag T: T name %(name)s, T tags X WHERE X eid %(x)s"
+            execute(rql, {"name": tagname, "x": eid})
 
 
 @ajaxcontroller.ajaxfunc
 def untag_entity(self, eid, tageid):
-    rql = 'DELETE T tags X WHERE T eid %(t)s, X eid %(x)s'
-    self._cw.execute(rql, {'t': tageid, 'x': eid})
+    rql = "DELETE T tags X WHERE T eid %(t)s, X eid %(x)s"
+    self._cw.execute(rql, {"t": tageid, "x": eid})
 
 
 # the merge tags component #####################################################
 
+
 class MergeComponent(component.EntityCtxComponent):
-    __regid__ = 'mergetag'
-    __select__ = (component.EntityCtxComponent.__select__ &
-                  is_instance('Tag') & match_user_groups('managers'))
-    context = 'navcontentbottom'
-    title = _('merge tags')
+    __regid__ = "mergetag"
+    __select__ = (
+        component.EntityCtxComponent.__select__
+        & is_instance("Tag")
+        & match_user_groups("managers")
+    )
+    context = "navcontentbottom"
+    title = _("merge tags")
 
     def render_body(self, w):
-        self._cw.add_js(('cubes.tag.merge.js', 'cubicweb.widgets.js'))
+        self._cw.add_js(("cubes.tag.merge.js", "cubicweb.widgets.js"))
         entity = self.entity
-        w(u'<div id="tagmergeformholder%s">' % entity.eid)
-        w(u'<h5>%s</h5>' % self._cw._('Enter a tag name'))
-        w(u'<input  type="hidden" id="tageid" value="%s"/>' % entity.eid)
-        w(u'<input id="acmergetag" type="text" class="widget" cubicweb:dataurl="%s" '
-          u'cubicweb:loadtype="auto" cubicweb:wdgtype="RestrictedSuggestField" />'
-          % xml_escape(self._cw.build_url('json', fname='unrelated_merge_tags',
-                                          arg=entity.eid)))
-        w(u'<div id="tagged_entities_holder"></div>')
-        w(u'<div id="sgformbuttons" class="hidden">')
-        w(u'<input class="validateButton" type="button" value="%s" onclick="javascript:mergeTags(%s);"/>'
-          % (self._cw._('merge (keeping %s)') % xml_escape(entity.dc_title()), entity.eid))
-        w(u'<input class="validateButton" type="button" value="%s" onclick="javascript:cancelSelectedMergeTag(%s)"/>'
-          % (self._cw._(stdmsgs.BUTTON_CANCEL[0]), entity.eid))
-        w(u'</div>')
-        w(u'</div>')
+        w(f'<div id="tagmergeformholder{entity.eid}">')
+        w(f"<h5>{self._cw._('Enter a tag name')}</h5>")
+        w(f'<input  type="hidden" id="tageid" value="{entity.eid}"/>')
+        w(
+            '<input id="acmergetag" type="text" class="widget" cubicweb:dataurl="%s" '
+            'cubicweb:loadtype="auto" cubicweb:wdgtype="RestrictedSuggestField" />'
+            % xml_escape(
+                self._cw.build_url("json", fname="unrelated_merge_tags", arg=entity.eid)
+            )
+        )
+        w('<div id="tagged_entities_holder"></div>')
+        w('<div id="sgformbuttons" class="hidden">')
+        w(
+            '<input class="validateButton" type="button" value="%s" onclick="javascript:mergeTags(%s);"/>'
+            % (
+                self._cw._("merge (keeping %s)") % xml_escape(entity.dc_title()),
+                entity.eid,
+            )
+        )
+        w(
+            '<input class="validateButton" type="button" value="%s" onclick="javascript:cancelSelectedMergeTag(%s)"/>'
+            % (self._cw._(stdmsgs.BUTTON_CANCEL[0]), entity.eid)
+        )
+        w("</div>")
+        w("</div>")
 
 
-@ajaxcontroller.ajaxfunc(output_type='json')
+@ajaxcontroller.ajaxfunc(output_type="json")
 def unrelated_merge_tags(self, eid):
     """return tag unrelated to an entity"""
-    rql = 'Any N ORDERBY N WHERE T is Tag, T name N, NOT T eid %(x)s'
-    return [name for (name,) in self._cw.execute(rql, {'x': eid})]
+    rql = "Any N ORDERBY N WHERE T is Tag, T name N, NOT T eid %(x)s"
+    return [name for (name,) in self._cw.execute(rql, {"x": eid})]
 
 
-@ajaxcontroller.ajaxfunc(output_type='xhtml')
+@ajaxcontroller.ajaxfunc(output_type="xhtml")
 def tagged_entity_html(self, name):
-    rset = self._cw.execute('Any X ORDERBY X DESC LIMIT 10 WHERE T tags X, '
-                            'T name %(x)s', {'x': name})
+    rset = self._cw.execute(
+        "Any X ORDERBY X DESC LIMIT 10 WHERE T tags X, " "T name %(x)s", {"x": name}
+    )
     html = []
     if rset:
         html.append('<div id="taggedEntities">')
         # FIXME - add test to go through select_view
-        view = self._cw.vreg['views'].select('list', self._cw, rset=rset)
-        html.append(view.render(title=self._cw._('linked entities:')))
-        html.append(u'</div>')
+        view = self._cw.vreg["views"].select("list", self._cw, rset=rset)
+        html.append(view.render(title=self._cw._("linked entities:")))
+        html.append("</div>")
         # html.append(self._cw.view('list', rset))
     else:
-        html.append('<div>%s</div>' % _('no entities related to this tag'))
-        view = self._cw.vreg['views'].select('null', self._cw, rset=rset)
-    return u' '.join(html)
+        html.append(f"<div>{_('no entities related to this tag')}</div>")
+        view = self._cw.vreg["views"].select("null", self._cw, rset=rset)
+    return " ".join(html)
 
 
-@ajaxcontroller.ajaxfunc(output_type='xhtml')
+@ajaxcontroller.ajaxfunc(output_type="xhtml")
 def merge_tags(self, eid, mergetag_name):
-    mergetag_name = mergetag_name.strip(',')  # XXX
-    self._cw.execute('SET T tags X WHERE T1 tags X, NOT T tags X, '
-                     'T eid %(x)s, T1 name %(name)s',
-                     {'x': eid, 'name': mergetag_name})
-    self._cw.execute('DELETE Tag T WHERE T name %(name)s', {'name': mergetag_name})
+    mergetag_name = mergetag_name.strip(",")  # XXX
+    self._cw.execute(
+        "SET T tags X WHERE T1 tags X, NOT T tags X, " "T eid %(x)s, T1 name %(name)s",
+        {"x": eid, "name": mergetag_name},
+    )
+    self._cw.execute("DELETE Tag T WHERE T name %(name)s", {"name": mergetag_name})
     # FIXME - add test to go through select_view
-    view = self._cw.vreg['views'].select('primary', self._cw,
-                                         rset=self._cw.eid_rset(eid))
+    view = self._cw.vreg["views"].select(
+        "primary", self._cw, rset=self._cw.eid_rset(eid)
+    )
     return view.render()
 
 
 # facets, ui adapter ###########################################################
 
+
 class TagsFacet(facet.RelationFacet):
-    __regid__ = 'tags-facet'
-    rtype = 'tags'
-    role = 'object'
-    target_attr = 'name'
+    __regid__ = "tags-facet"
+    rtype = "tags"
+    role = "object"
+    target_attr = "name"
 
 
 class TagIFeedAdapter(xmlrss.IFeedAdapter):
-    __select__ = is_instance('Tag')
+    __select__ = is_instance("Tag")
 
     def rss_feed_url(self):
-        rql = ('Any X ORDERBY CD DESC LIMIT 15 WHERE '
-               'T tags X, T eid %s, X modification_date CD') % self.entity.eid
-        return self._cw.build_url(rql=rql, vid='rss', vtitle=self.entity.dc_title())
+        rql = (
+            "Any X ORDERBY CD DESC LIMIT 15 WHERE "
+            "T tags X, T eid %s, X modification_date CD"
+        ) % self.entity.eid
+        return self._cw.build_url(rql=rql, vid="rss", vtitle=self.entity.dc_title())
```

### Comparing `cubicweb-tag-2.0.0/cubicweb_tag.egg-info/PKG-INFO` & `cubicweb-tag-3.0.0/cubicweb_tag.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cubicweb-tag
-Version: 2.0.0
+Version: 3.0.0
 Summary: tag component for the CubicWeb framework
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-tag
 Author: Logilab
 Author-email: contact@logilab.fr
 License: LGPL
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: JavaScript
 
 Summary
 -------
@@ -85,9 +84,7 @@
   different words, or spelling.
 
 Documentation
 -------------
 
 Look in the ``doc/`` subdirectory or read
 http://www.cubicweb.org/doc/en/
-
-
```

### Comparing `cubicweb-tag-2.0.0/cubicweb_tag.egg-info/SOURCES.txt` & `cubicweb-tag-3.0.0/cubicweb_tag.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-tag-2.0.0/setup.py` & `cubicweb-tag-3.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # pylint: disable=W0142,W0403,W0404,W0613,W0622,W0622,W0704,R0904,C0103,E0611
 #
-# copyright 2003-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2003-2023 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr/ -- mailto:contact@logilab.fr
 #
 # This file is part of a CubicWeb cube.
 #
 # CubicWeb is free software: you can redistribute it and/or modify it under the
 # terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
@@ -26,58 +26,56 @@
 from setuptools import find_packages, setup
 
 
 here = dirname(__file__)
 
 # load metadata from the __pkginfo__.py file so there is no risk of conflict
 # see https://packaging.python.org/en/latest/single_source_version.html
-pkginfo = join(here, 'cubicweb_tag', '__pkginfo__.py')
+pkginfo = join(here, "cubicweb_tag", "__pkginfo__.py")
 __pkginfo__ = {}
 with open(pkginfo) as f:
     exec(f.read(), __pkginfo__)
 
 # get required metadatas
-distname = __pkginfo__['distname']
-version = __pkginfo__['version']
-license = __pkginfo__['license']
-description = __pkginfo__['description']
-web = __pkginfo__['web']
-author = __pkginfo__['author']
-author_email = __pkginfo__['author_email']
-classifiers = __pkginfo__['classifiers']
+distname = __pkginfo__["distname"]
+version = __pkginfo__["version"]
+license = __pkginfo__["license"]
+description = __pkginfo__["description"]
+web = __pkginfo__["web"]
+author = __pkginfo__["author"]
+author_email = __pkginfo__["author_email"]
+classifiers = __pkginfo__["classifiers"]
 
-with open(join(here, 'README.rst')) as f:
+with open(join(here, "README.rst")) as f:
     long_description = f.read()
 
 # get optional metadatas
-data_files = __pkginfo__.get('data_files', None)
-dependency_links = __pkginfo__.get('dependency_links', ())
+data_files = __pkginfo__.get("data_files", None)
+dependency_links = __pkginfo__.get("dependency_links", ())
 
 requires = {}
 for entry in ("__depends__",):  # "__recommends__"):
     requires.update(__pkginfo__.get(entry, {}))
 
-install_requires = ["{0} {1}".format(d, v and v or "").strip()
-                    for d, v in requires.items()]
+install_requires = [f"{d} {v and v or ''}".strip() for d, v in requires.items()]
 
 
 setup(
     name=distname,
     version=version,
     license=license,
     description=description,
     long_description=long_description,
     author=author,
     author_email=author_email,
     url=web,
     classifiers=classifiers,
-    packages=find_packages(exclude=['test']),
+    packages=find_packages(exclude=["test"]),
     install_requires=install_requires,
     include_package_data=True,
     entry_points={
-        'cubicweb.cubes': [
-            'tag=cubicweb_tag',
+        "cubicweb.cubes": [
+            "tag=cubicweb_tag",
         ],
     },
-
     zip_safe=False,
 )
```

### Comparing `cubicweb-tag-2.0.0/test/unittest_tag.py` & `cubicweb-tag-3.0.0/test/unittest_tag.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,76 +1,86 @@
-from cubicweb.devtools.testlib import CubicWebTC
+from cubicweb_web.devtools.testlib import WebCWTC
 
 
-class TagEntityTC(CubicWebTC):
-
+class TagEntityTC(WebCWTC):
     def setup_database(self):
         with self.admin_access.repo_cnx() as cnx:
-            self.tag = cnx.create_entity('Tag', name=u'x').eid
-            self.tag2 = cnx.create_entity('Tag', name=u'y').eid
+            self.tag = cnx.create_entity("Tag", name="x").eid
+            self.tag2 = cnx.create_entity("Tag", name="y").eid
             cnx.execute('SET T tags TT WHERE T name "x", TT name "y"')
             cnx.commit()
 
     def test_dc_title(self):
         with self.admin_access.client_cnx() as cnx:
             tag = cnx.entity_from_eid(self.tag)
-            self.assertEqual(tag.dc_title(), 'x')
+            self.assertEqual(tag.dc_title(), "x")
 
     def test_views_dont_fail(self):
         with self.admin_access.web_request() as req:
             tag = req.entity_from_eid(self.tag)
-            tag.view('incontext')
-            tag.view('primary')
+            tag.view("incontext")
+            tag.view("primary")
 
     def test_boxes_dont_fail(self):
         def w(string, *args, escape=True):
             return string % args if args else string
 
         with self.admin_access.web_request() as req:
             tag = req.entity_from_eid(self.tag)
             tag2 = req.entity_from_eid(self.tag2)
-            self.vreg['ctxcomponents'].select('tags_box', req, rset=tag.cw_rset).render(w)
-            self.vreg['ctxcomponents'].select('similarity_box', req, rset=tag2.cw_rset).render(w)
-            self.vreg['ctxcomponents'].select('tagcloud_box', req, rset=tag.cw_rset).render(w)
+            self.vreg["ctxcomponents"].select("tags_box", req, rset=tag.cw_rset).render(
+                w
+            )
+            self.vreg["ctxcomponents"].select(
+                "similarity_box", req, rset=tag2.cw_rset
+            ).render(w)
+            self.vreg["ctxcomponents"].select(
+                "tagcloud_box", req, rset=tag.cw_rset
+            ).render(w)
 
     def test_json_dont_fail(self):
         with self.admin_access.web_request() as req:
             tag = req.entity_from_eid(self.tag)
-            self.vreg['ajax-func'].select('tagged_entity_html', req)(u'x')
-            self.vreg['ajax-func'].select('tagged_entity_html', req, rset=tag.cw_rset)(u'x')
-            entity = req.create_entity('Tag', name=u'main')
-            self.vreg['ajax-func'].select('merge_tags', req)(entity.eid, u'x')
-            self.vreg['ajax-func'].select('unrelated_merge_tags', req)(entity.eid)
+            self.vreg["ajax-func"].select("tagged_entity_html", req)("x")
+            self.vreg["ajax-func"].select("tagged_entity_html", req, rset=tag.cw_rset)(
+                "x"
+            )
+            entity = req.create_entity("Tag", name="main")
+            self.vreg["ajax-func"].select("merge_tags", req)(entity.eid, "x")
+            self.vreg["ajax-func"].select("unrelated_merge_tags", req)(entity.eid)
 
     def test_closest_tags(self):
         with self.admin_access.client_cnx() as cnx:
-            cnx.create_entity('Tag', name=u'main')
-            cnx.create_entity('Tag', name=u'tag1')
-            cnx.create_entity('Tag', name=u'tag2')
-            cnx.create_entity('Tag', name=u'tag3')
-            cnx.create_entity('Tag', name=u'tag4')
-            cnx.create_entity('BlogEntry', title=u"news", content=u"cubicweb c'est beau")
-            cnx.create_entity('BlogEntry', title=u"yes", content=u"la vie est belle")
-            cnx.create_entity('BlogEntry', title=u"realy", content=u"trallalla")
-            cnx.create_entity('BlogEntry', title=u"no", content=u"c'est vrai")
+            cnx.create_entity("Tag", name="main")
+            cnx.create_entity("Tag", name="tag1")
+            cnx.create_entity("Tag", name="tag2")
+            cnx.create_entity("Tag", name="tag3")
+            cnx.create_entity("Tag", name="tag4")
+            cnx.create_entity("BlogEntry", title="news", content="cubicweb c'est beau")
+            cnx.create_entity("BlogEntry", title="yes", content="la vie est belle")
+            cnx.create_entity("BlogEntry", title="realy", content="trallalla")
+            cnx.create_entity("BlogEntry", title="no", content="c'est vrai")
             cnx.execute('SET T tags B WHERE T name "main" , B title "news"')
             cnx.execute('SET T tags B WHERE T name "main" , B title "yes"')
             cnx.execute('SET T tags B WHERE T name "main" , B title "realy"')
             cnx.execute('SET T tags B WHERE T name "tag1" , B title "news"')
             cnx.execute('SET T tags B WHERE T name "tag1" , B title "yes"')
             cnx.execute('SET T tags B WHERE T name "tag1" , B title "realy"')
             cnx.execute('SET T tags B WHERE T name "tag2" , B title "news"')
             cnx.execute('SET T tags B WHERE T name "tag2" , B title "yes"')
             cnx.execute('SET T tags B WHERE T name "tag3" , B title "realy"')
             cnx.execute('SET T tags B WHERE T name "tag4" , B title "no"')
-            compare_tag = cnx.execute('Tag T WHERE T name %(name)s', {'name': u'main'}).get_entity(0, 0)
+            compare_tag = cnx.execute(
+                "Tag T WHERE T name %(name)s", {"name": "main"}
+            ).get_entity(0, 0)
             rset = compare_tag.closest_tags_rset()
             closest_list = [x.name for x in rset.entities()]
-            self.assertEqual(closest_list[0], u'tag1')
-            self.assertEqual(closest_list[1], u'tag2')
-            self.assertEqual(closest_list[2], u'tag3')
-            self.assertTrue(u'tag4' not in closest_list)
+            self.assertEqual(closest_list[0], "tag1")
+            self.assertEqual(closest_list[1], "tag2")
+            self.assertEqual(closest_list[2], "tag3")
+            self.assertTrue("tag4" not in closest_list)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     import unittest
+
     unittest.main()
```

