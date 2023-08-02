# Comparing `tmp/cubicweb-addressbook-1.9.1.tar.gz` & `tmp/cubicweb-addressbook-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cubicweb-addressbook-1.9.1.tar", last modified: Wed May 11 14:46:53 2016, max compression
+gzip compressed data, was "cubicweb-addressbook-2.0.0.tar", last modified: Wed Aug  2 13:01:55 2023, max compression
```

## Comparing `cubicweb-addressbook-1.9.1.tar` & `cubicweb-addressbook-2.0.0.tar`

### file list

```diff
@@ -1,25 +1,41 @@
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2016-05-11 14:46:53.000000 cubicweb-addressbook-1.9.1/
--rw-r--r--   0 narval     (111) narval     (116)     1521 2016-05-11 14:34:39.000000 cubicweb-addressbook-1.9.1/schema.py
--rw-r--r--   0 narval     (111) narval     (116)     2954 2016-05-11 14:34:39.000000 cubicweb-addressbook-1.9.1/views.py
--rw-r--r--   0 narval     (111) narval     (116)     1354 2016-05-11 14:34:39.000000 cubicweb-addressbook-1.9.1/hooks.py
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2016-05-11 14:46:53.000000 cubicweb-addressbook-1.9.1/schema/
--rw-r--r--   0 narval     (111) narval     (116)      824 2016-05-11 14:34:39.000000 cubicweb-addressbook-1.9.1/schema/_regproc.postgres.sql
--rw-r--r--   0 narval     (111) narval     (116)      229 2016-05-11 14:34:39.000000 cubicweb-addressbook-1.9.1/README
--rw-r--r--   0 narval     (111) narval     (116)     1553 2016-05-11 14:34:39.000000 cubicweb-addressbook-1.9.1/__pkginfo__.py
--rw-rw-r--   0 narval     (111) narval     (116)      583 2016-05-11 14:46:53.000000 cubicweb-addressbook-1.9.1/PKG-INFO
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2016-05-11 14:46:53.000000 cubicweb-addressbook-1.9.1/test/
--rw-r--r--   0 narval     (111) narval     (116)      365 2016-05-11 14:34:39.000000 cubicweb-addressbook-1.9.1/test/test_addressbook.py
--rw-r--r--   0 narval     (111) narval     (116)      896 2016-05-11 14:34:39.000000 cubicweb-addressbook-1.9.1/__init__.py
--rw-r--r--   0 narval     (111) narval     (116)     7094 2016-05-11 14:34:39.000000 cubicweb-addressbook-1.9.1/setup.py
--rw-r--r--   0 narval     (111) narval     (116)     1524 2016-05-11 14:34:39.000000 cubicweb-addressbook-1.9.1/entities.py
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2016-05-11 14:46:53.000000 cubicweb-addressbook-1.9.1/i18n/
--rw-r--r--   0 narval     (111) narval     (116)     2212 2016-05-11 14:34:39.000000 cubicweb-addressbook-1.9.1/i18n/es.po
--rw-r--r--   0 narval     (111) narval     (116)     2823 2016-05-11 14:34:39.000000 cubicweb-addressbook-1.9.1/i18n/fr.po
--rw-r--r--   0 narval     (111) narval     (116)     2650 2016-05-11 14:34:39.000000 cubicweb-addressbook-1.9.1/i18n/en.po
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2016-05-11 14:46:53.000000 cubicweb-addressbook-1.9.1/migration/
--rw-r--r--   0 narval     (111) narval     (116)      116 2016-05-11 14:34:39.000000 cubicweb-addressbook-1.9.1/migration/1.5.0_Any.py
--rw-r--r--   0 narval     (111) narval     (116)      211 2016-05-11 14:34:39.000000 cubicweb-addressbook-1.9.1/migration/1.2.1_Any.py
--rw-r--r--   0 narval     (111) narval     (116)       73 2016-05-11 14:34:39.000000 cubicweb-addressbook-1.9.1/migration/1.6.2_Any.py
--rw-r--r--   0 narval     (111) narval     (116)       66 2016-05-11 14:34:39.000000 cubicweb-addressbook-1.9.1/migration/postcreate.py
--rw-r--r--   0 narval     (111) narval     (116)       43 2016-05-11 14:34:39.000000 cubicweb-addressbook-1.9.1/migration/1.6.3_Any.py
--rw-r--r--   0 narval     (111) narval     (116)       54 2016-05-11 14:34:39.000000 cubicweb-addressbook-1.9.1/migration/1.2.4_Any.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 13:01:55.340126 cubicweb-addressbook-2.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      430 2023-08-02 13:01:18.000000 cubicweb-addressbook-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      664 2023-08-02 13:01:55.340126 cubicweb-addressbook-2.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      229 2023-08-02 13:01:18.000000 cubicweb-addressbook-2.0.0/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      727 2023-08-02 13:01:19.000000 cubicweb-addressbook-2.0.0/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 13:01:55.328126 cubicweb-addressbook-2.0.0/cubicweb_addressbook/
+-rw-rw-rw-   0 root         (0) root         (0)      937 2023-08-02 13:01:19.000000 cubicweb-addressbook-2.0.0/cubicweb_addressbook/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      727 2023-08-02 13:01:19.000000 cubicweb-addressbook-2.0.0/cubicweb_addressbook/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1497 2023-08-02 13:01:19.000000 cubicweb-addressbook-2.0.0/cubicweb_addressbook/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1382 2023-08-02 13:01:19.000000 cubicweb-addressbook-2.0.0/cubicweb_addressbook/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 13:01:55.336126 cubicweb-addressbook-2.0.0/cubicweb_addressbook/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)     2650 2023-08-02 13:01:19.000000 cubicweb-addressbook-2.0.0/cubicweb_addressbook/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)     2212 2023-08-02 13:01:19.000000 cubicweb-addressbook-2.0.0/cubicweb_addressbook/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)     2823 2023-08-02 13:01:19.000000 cubicweb-addressbook-2.0.0/cubicweb_addressbook/i18n/fr.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 13:01:55.340126 cubicweb-addressbook-2.0.0/cubicweb_addressbook/migration/
+-rw-rw-rw-   0 root         (0) root         (0)      223 2023-08-02 13:01:19.000000 cubicweb-addressbook-2.0.0/cubicweb_addressbook/migration/1.2.1_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-08-02 13:01:19.000000 cubicweb-addressbook-2.0.0/cubicweb_addressbook/migration/1.2.4_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-08-02 13:01:19.000000 cubicweb-addressbook-2.0.0/cubicweb_addressbook/migration/1.5.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-02 13:01:19.000000 cubicweb-addressbook-2.0.0/cubicweb_addressbook/migration/1.6.2_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       42 2023-08-02 13:01:19.000000 cubicweb-addressbook-2.0.0/cubicweb_addressbook/migration/1.6.3_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       65 2023-08-02 13:01:19.000000 cubicweb-addressbook-2.0.0/cubicweb_addressbook/migration/postcreate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 13:01:55.340126 cubicweb-addressbook-2.0.0/cubicweb_addressbook/schema/
+-rw-rw-rw-   0 root         (0) root         (0)      824 2023-08-02 13:01:19.000000 cubicweb-addressbook-2.0.0/cubicweb_addressbook/schema/_regproc.postgres.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1492 2023-08-02 13:01:19.000000 cubicweb-addressbook-2.0.0/cubicweb_addressbook/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     2888 2023-08-02 13:01:19.000000 cubicweb-addressbook-2.0.0/cubicweb_addressbook/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 13:01:55.332126 cubicweb-addressbook-2.0.0/cubicweb_addressbook.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      664 2023-08-02 13:01:55.000000 cubicweb-addressbook-2.0.0/cubicweb_addressbook.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-08-02 13:01:55.000000 cubicweb-addressbook-2.0.0/cubicweb_addressbook.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 13:01:55.000000 cubicweb-addressbook-2.0.0/cubicweb_addressbook.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-08-02 13:01:55.000000 cubicweb-addressbook-2.0.0/cubicweb_addressbook.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 13:01:55.000000 cubicweb-addressbook-2.0.0/cubicweb_addressbook.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       83 2023-08-02 13:01:55.000000 cubicweb-addressbook-2.0.0/cubicweb_addressbook.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-02 13:01:55.000000 cubicweb-addressbook-2.0.0/cubicweb_addressbook.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-08-02 13:01:19.000000 cubicweb-addressbook-2.0.0/dev-requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-02 13:01:55.340126 cubicweb-addressbook-2.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2620 2023-08-02 13:01:19.000000 cubicweb-addressbook-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 13:01:55.340126 cubicweb-addressbook-2.0.0/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 13:01:55.340126 cubicweb-addressbook-2.0.0/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-08-02 13:01:19.000000 cubicweb-addressbook-2.0.0/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-08-02 13:01:19.000000 cubicweb-addressbook-2.0.0/test/test_addressbook.py
+-rw-rw-rw-   0 root         (0) root         (0)     1113 2023-08-02 13:01:19.000000 cubicweb-addressbook-2.0.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cubicweb-addressbook-1.9.1/schema.py` & `cubicweb-addressbook-2.0.0/cubicweb_addressbook/schema.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,45 @@
 from yams.buildobjs import EntityType, String, Float
 from yams.constraints import IntervalBoundConstraint
 
-_ = unicode
+from cubicweb import _
+
 
 class PhoneNumber(EntityType):
     number = String(fulltextindexed=True, required=True, maxsize=64)
-    type = String(required=True, internationalizable=True,
-                  vocabulary=((_('mobile'), _('home'), _('office'),
-                               _('fax'), _('secretariat'))),
-                  default=u'mobile')
+    type = String(
+        required=True,
+        internationalizable=True,
+        vocabulary=((_("mobile"), _("home"), _("office"), _("fax"), _("secretariat"))),
+        default="mobile",
+    )
+
 
 class PostalAddress(EntityType):
-    street  = String(fulltextindexed=True, required=True, maxsize=256)
-    street2  = String(fulltextindexed=True, maxsize=256)
+    street = String(fulltextindexed=True, required=True, maxsize=256)
+    street2 = String(fulltextindexed=True, maxsize=256)
     postalcode = String(fulltextindexed=True, required=True, maxsize=256)
-    city    = String(fulltextindexed=True, required=True, maxsize=256,
-                     internationalizable=True) # see static-message.pot
-    country = String(fulltextindexed=True, maxsize=256,
-                     internationalizable=True) # see static-message.pot
-    state   = String(fulltextindexed=True, maxsize=256)
-    latitude = Float(constraints=[IntervalBoundConstraint(-90, 90)],
-                     description=_('latitude in degree'))
-    longitude = Float(constraints=[IntervalBoundConstraint(-180, 180)],
-                     description=_('longitude in degree'))
+    city = String(
+        fulltextindexed=True, required=True, maxsize=256, internationalizable=True
+    )  # see static-message.pot
+    country = String(
+        fulltextindexed=True, maxsize=256, internationalizable=True
+    )  # see static-message.pot
+    state = String(fulltextindexed=True, maxsize=256)
+    latitude = Float(
+        constraints=[IntervalBoundConstraint(-90, 90)],
+        description=_("latitude in degree"),
+    )
+    longitude = Float(
+        constraints=[IntervalBoundConstraint(-180, 180)],
+        description=_("longitude in degree"),
+    )
+
 
 class IMAddress(EntityType):
-    im_account  = String(fulltextindexed=True, required=True, maxsize=64)
-    type = String(required=True, internationalizable=True,
-                  vocabulary=('jabber', 'icq', 'msn'),
-                  default=u'jabber')
+    im_account = String(fulltextindexed=True, required=True, maxsize=64)
+    type = String(
+        required=True,
+        internationalizable=True,
+        vocabulary=("jabber", "icq", "msn"),
+        default="jabber",
+    )
```

### Comparing `cubicweb-addressbook-1.9.1/views.py` & `cubicweb-addressbook-2.0.0/cubicweb_addressbook/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,72 +4,74 @@
 :copyright: 2003-2010 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 :contact: http://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 __docformat__ = "restructuredtext en"
 
 from logilab.mtconverter import xml_escape
 
-from cubicweb.view import EntityView
+from cubicweb_web.view import EntityView
 from cubicweb.predicates import is_instance
-from cubicweb.web.views import baseviews, uicfg
+from cubicweb_web.views import baseviews, uicfg
 
-uicfg.indexview_etype_section['PhoneNumber'] = 'subobject'
-uicfg.indexview_etype_section['PostalAddress'] = 'subobject'
-uicfg.indexview_etype_section['IMAddress'] = 'subobject'
+uicfg.indexview_etype_section["PhoneNumber"] = "subobject"
+uicfg.indexview_etype_section["PostalAddress"] = "subobject"
+uicfg.indexview_etype_section["IMAddress"] = "subobject"
+
+uicfg.autoform_section.tag_attribute(("PostalAddress", "latitude"), "main", "hidden")
+uicfg.autoform_section.tag_attribute(("PostalAddress", "longitude"), "main", "hidden")
 
-uicfg.autoform_section.tag_attribute(('PostalAddress', 'latitude'), 'main', 'hidden')
-uicfg.autoform_section.tag_attribute(('PostalAddress', 'longitude'), 'main', 'hidden')
 
 class PhoneNumberInContextView(baseviews.InContextView):
-    __select__ = is_instance('PhoneNumber')
+    __select__ = is_instance("PhoneNumber")
 
     def cell_call(self, row, col=0):
         self.w(xml_escape(self.cw_rset.get_entity(row, col).dc_title()))
 
+
 class PhoneNumberListItemView(baseviews.ListItemView):
-    __select__ = is_instance('PhoneNumber')
+    __select__ = is_instance("PhoneNumber")
 
     def cell_call(self, row, col=0, vid=None):
         entity = self.cw_rset.get_entity(row, col)
-        self.w(u'<div class="tel"><span class="type">%s</span> %s</div>'
-               % (xml_escape(entity.type),
-                  xml_escape(entity.number)))
+        self.w(
+            '<div class="tel"><span class="type">%s</span> %s</div>'
+            % (xml_escape(entity.type), xml_escape(entity.number))
+        )
+
 
 class PhoneNumberSipView(EntityView):
-    __regid__ = u'sip'
-    __select__ = is_instance('PhoneNumber')
+    __regid__ = "sip"
+    __select__ = is_instance("PhoneNumber")
 
     def cell_call(self, row, col, contexteid=None):
         entity = self.cw_rset.get_entity(row, col)
-        self.w(u'<div class="phonenumber">')
+        self.w('<div class="phonenumber">')
         number = xml_escape(entity.number)
-        self.w(u'<a href="sip:%s">%s</a>' % (number.replace(" ", ""), number))
-        self.w(u'</div>')
+        self.w(f"<a href=\"sip:{number.replace(' ', '')}\">{number}</a>")
+        self.w("</div>")
 
 
 class PostalAddressInContextView(baseviews.InContextView):
-    __select__ = is_instance('PostalAddress')
+    __select__ = is_instance("PostalAddress")
 
     def cell_call(self, row, col, contexteid=None):
         entity = self.cw_rset.get_entity(row, col)
-        self.w(u'<div class="adr">')
-        if entity.street: # may be set optional by client cubes
-            self.w(u'<div class="street-address">%s' %
-                   xml_escape(entity.street))
+        self.w('<div class="adr">')
+        if entity.street:  # may be set optional by client cubes
+            self.w(f'<div class="street-address">{xml_escape(entity.street)}')
             if entity.street2:
-                self.w(u'<br/>')
-                self.w(xml_escape(entity.street2)) # FIXME div-class
-            self.w(u'</div>')
+                self.w("<br/>")
+                self.w(xml_escape(entity.street2))  # FIXME div-class
+            self.w("</div>")
         if entity.postalcode:
-            self.w(u'<span class="postal-code">%s</span> - '
-                   % xml_escape(entity.postalcode))
+            self.w(
+                f'<span class="postal-code">{xml_escape(entity.postalcode)}</span> - '
+            )
         if entity.city:
-            self.w(u'<span class="locality">%s</span>'
-                   % xml_escape(entity.city))
+            self.w(f'<span class="locality">{xml_escape(entity.city)}</span>')
         if entity.state:
-            self.w(u'<br/>')
-            self.w(u'<span class="region">%s</span>' % xml_escape(entity.state))
+            self.w("<br/>")
+            self.w(f'<span class="region">{xml_escape(entity.state)}</span>')
         if entity.country:
-            self.w(u'<br/>')
-            self.w(u'<span class="country-name">%s</span>'
-                   % xml_escape(entity.country))
-        self.w(u'</div>\n')
+            self.w("<br/>")
+            self.w(f'<span class="country-name">{xml_escape(entity.country)}</span>')
+        self.w("</div>\n")
```

### Comparing `cubicweb-addressbook-1.9.1/hooks.py` & `cubicweb-addressbook-2.0.0/cubicweb_addressbook/hooks.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,35 +2,40 @@
 
 :organization: Logilab
 :copyright: 2001-2011 LOGILAB S.A. (Paris, FRANCE), license is LGPL v2.
 :contact: http://www.logilab.fr/ -- mailto:contact@logilab.fr
 :license: GNU Lesser General Public License, v2.1 - http://www.gnu.org/licenses
 """
 
-__docformat__ = 'restructuredtext en'
+__docformat__ = "restructuredtext en"
 
-from cubes.geocoding import geocoding
 
 from cubicweb.predicates import is_instance
 from cubicweb.server.hook import Hook
 
+from cubicweb_geocoding import geocoding
+
+
 class AutoSetLatLng(Hook):
-    __regid__ = 'auto_lat_lng_hook'
-    __select__ = is_instance('PostalAddress')
-    events = ('before_add_entity', 'before_update_entity')
+    __regid__ = "auto_lat_lng_hook"
+    __select__ = is_instance("PostalAddress")
+    events = ("before_add_entity", "before_update_entity")
 
     def __call__(self):
-        gmapkey = self._cw.vreg.config.get('gmap-key')
+        gmapkey = self._cw.vreg.config.get("gmap-key")
         if not gmapkey:
             return
-        geoattrs = set(('street', 'street2', 'postalcode', 'city', 'country'))
+        geoattrs = {"street", "street2", "postalcode", "city", "country"}
         changed_attrs = set(self.entity.cw_edited)
-        if (geoattrs & changed_attrs
-            and not self.entity.cw_attr_cache.get('latitude')
-            and not self.entity.cw_attr_cache.get('longitude')):
+        if (
+            geoattrs & changed_attrs
+            and not self.entity.cw_attr_cache.get("latitude")
+            and not self.entity.cw_attr_cache.get("longitude")
+        ):
             try:
                 latlng = geocoding.get_latlng(self.entity.dc_long_title(), gmapkey)
             except geocoding.UnknownAddress:
-                self._cw.warning('unable to get latitude / longitude for %s',
-                                self.entity.eid)
+                self._cw.warning(
+                    "unable to get latitude / longitude for %s", self.entity.eid
+                )
             else:
                 self.entity.cw_edited.update(latlng)
```

### Comparing `cubicweb-addressbook-1.9.1/schema/_regproc.postgres.sql` & `cubicweb-addressbook-2.0.0/cubicweb_addressbook/schema/_regproc.postgres.sql`

 * *Files identical despite different names*

### Comparing `cubicweb-addressbook-1.9.1/__init__.py` & `cubicweb-addressbook-2.0.0/cubicweb_addressbook/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 """cubicweb-addressbook"""
 
 from cubicweb import ETYPE_NAME_MAP
 from rql.utils import register_function, FunctionDescr
 
-ETYPE_NAME_MAP['Phonenumber'] = 'PhoneNumber'
-ETYPE_NAME_MAP['Postaladdress'] = 'PostalAddress'
+ETYPE_NAME_MAP["Phonenumber"] = "PhoneNumber"
+ETYPE_NAME_MAP["Postaladdress"] = "PostalAddress"
+
 
 class phonetype_sort_value(FunctionDescr):
-    supported_backends = ('postgres', 'sqlite',)
-    rtype = 'Int'
+    supported_backends = (
+        "postgres",
+        "sqlite",
+    )
+    rtype = "Int"
+
 
 try:
     register_function(phonetype_sort_value)
 except AssertionError:
     pass
 
 
 try:
     from cubicweb.server import SQL_CONNECT_HOOKS
-except ImportError: # no server installation
+except ImportError:  # no server installation
     pass
 else:
 
     def init_sqlite_connexion(cnx):
         def phonetype_sort_value(text):
-            return {"mobile":2, "home":1, "office":4,
-                    "fax":0, "secretariat":3}[text]
+            return {"mobile": 2, "home": 1, "office": 4, "fax": 0, "secretariat": 3}[
+                text
+            ]
+
         cnx.create_function("PHONETYPE_SORT_VALUE", 1, phonetype_sort_value)
 
-    sqlite_hooks = SQL_CONNECT_HOOKS.setdefault('sqlite', [])
+    sqlite_hooks = SQL_CONNECT_HOOKS.setdefault("sqlite", [])
     sqlite_hooks.append(init_sqlite_connexion)
```

### Comparing `cubicweb-addressbook-1.9.1/entities.py` & `cubicweb-addressbook-2.0.0/cubicweb_addressbook/entities.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,43 +5,47 @@
 :contact: http://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 __docformat__ = "restructuredtext en"
 
 from cubicweb.entities import AnyEntity, fetch_config
 from cubicweb.predicates import is_instance
 
-from cubes.geocoding.views import IGeocodableAdapter
+from cubicweb_geocoding.views import IGeocodableAdapter
+
 
 class PhoneNumber(AnyEntity):
-    __regid__ = 'PhoneNumber'
-    fetch_attrs = fetch_config(['number', 'type'])[0]
+    __regid__ = "PhoneNumber"
+    fetch_attrs = fetch_config(["number", "type"])[0]
 
     @classmethod
-    def cw_fetch_order(cls, attr, var):
-        if attr == 'type':
-            return 'phonetype_sort_value(%s) DESC' % var
+    def cw_fetch_order(cls, select, attr, var):
+        if attr == "type":
+            return f"phonetype_sort_value({var}) DESC"
         return None
 
     def dc_title(self):
-        return u'%s (%s)' % (self.number, self._cw._(self.type))
+        return f"{self.number} ({self._cw._(self.type)})"
 
 
 class PostalAddress(AnyEntity):
-    __regid__ = 'PostalAddress'
-    fetch_attrs, cw_fetch_order = fetch_config(['street', 'street2', 'postalcode',
-                                             'city', 'country'])
+    __regid__ = "PostalAddress"
+    fetch_attrs, cw_fetch_order = fetch_config(
+        ["street", "street2", "postalcode", "city", "country"]
+    )
+
     def dc_long_title(self):
         lines = []
         if self.street:
             lines.append(self.street)
         if self.street2:
             lines.append(self.street2)
         if self.postalcode:
             lines.append(self.postalcode)
         if self.city:
             lines.append(self.city)
         if self.country:
             lines.append(self.country)
-        return u' '.join(lines)
+        return " ".join(lines)
+
 
 class PostalAddressIGeocodableAdapter(IGeocodableAdapter):
-    __select__ = is_instance('PostalAddress')
+    __select__ = is_instance("PostalAddress")
```

### Comparing `cubicweb-addressbook-1.9.1/i18n/es.po` & `cubicweb-addressbook-2.0.0/cubicweb_addressbook/i18n/es.po`

 * *Files identical despite different names*

### Comparing `cubicweb-addressbook-1.9.1/i18n/fr.po` & `cubicweb-addressbook-2.0.0/cubicweb_addressbook/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `cubicweb-addressbook-1.9.1/i18n/en.po` & `cubicweb-addressbook-2.0.0/cubicweb_addressbook/i18n/en.po`

 * *Files identical despite different names*

