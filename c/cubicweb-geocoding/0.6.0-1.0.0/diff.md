# Comparing `tmp/cubicweb-geocoding-0.6.0.tar.gz` & `tmp/cubicweb-geocoding-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-geocoding-0.6.0.tar", last modified: Thu Nov 24 01:41:13 2022, max compression
+gzip compressed data, was "cubicweb-geocoding-1.0.0.tar", last modified: Wed Aug  2 12:41:23 2023, max compression
```

## Comparing `cubicweb-geocoding-0.6.0.tar` & `cubicweb-geocoding-1.0.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 01:41:13.321990 cubicweb-geocoding-0.6.0/
--rw-rw-rw-   0 root         (0) root         (0)      273 2022-11-24 01:40:58.000000 cubicweb-geocoding-0.6.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      563 2022-11-24 01:41:13.321990 cubicweb-geocoding-0.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      105 2022-11-24 01:40:58.000000 cubicweb-geocoding-0.6.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 01:41:13.321990 cubicweb-geocoding-0.6.0/cubicweb_geocoding/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-24 01:40:58.000000 cubicweb-geocoding-0.6.0/cubicweb_geocoding/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      667 2022-11-24 01:40:58.000000 cubicweb-geocoding-0.6.0/cubicweb_geocoding/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 01:41:13.321990 cubicweb-geocoding-0.6.0/cubicweb_geocoding/data/
--rw-rw-rw-   0 root         (0) root         (0)     3333 2022-11-24 01:40:58.000000 cubicweb-geocoding-0.6.0/cubicweb_geocoding/data/cubicweb.gmap.js
--rw-rw-rw-   0 root         (0) root         (0)     2845 2022-11-24 01:40:58.000000 cubicweb-geocoding-0.6.0/cubicweb_geocoding/data/gmap.utility.labeledmarker.js
--rw-rw-rw-   0 root         (0) root         (0)      869 2022-11-24 01:40:58.000000 cubicweb-geocoding-0.6.0/cubicweb_geocoding/data/gmap_blue_marker.png
--rw-rw-rw-   0 root         (0) root         (0)     2769 2022-11-24 01:40:58.000000 cubicweb-geocoding-0.6.0/cubicweb_geocoding/geocoding.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 01:41:13.321990 cubicweb-geocoding-0.6.0/cubicweb_geocoding/i18n/
--rw-rw-rw-   0 root         (0) root         (0)      203 2022-11-24 01:40:58.000000 cubicweb-geocoding-0.6.0/cubicweb_geocoding/i18n/en.po
--rw-rw-rw-   0 root         (0) root         (0)      203 2022-11-24 01:40:58.000000 cubicweb-geocoding-0.6.0/cubicweb_geocoding/i18n/es.po
--rw-rw-rw-   0 root         (0) root         (0)      203 2022-11-24 01:40:58.000000 cubicweb-geocoding-0.6.0/cubicweb_geocoding/i18n/fr.po
--rw-rw-rw-   0 root         (0) root         (0)      202 2022-11-24 01:40:58.000000 cubicweb-geocoding-0.6.0/cubicweb_geocoding/site_cubicweb.py
--rw-rw-rw-   0 root         (0) root         (0)     4926 2022-11-24 01:40:58.000000 cubicweb-geocoding-0.6.0/cubicweb_geocoding/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 01:41:13.321990 cubicweb-geocoding-0.6.0/cubicweb_geocoding.egg-info/
--rw-r--r--   0 root         (0) root         (0)      563 2022-11-24 01:41:12.000000 cubicweb-geocoding-0.6.0/cubicweb_geocoding.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2022-11-24 01:41:13.000000 cubicweb-geocoding-0.6.0/cubicweb_geocoding.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-24 01:41:12.000000 cubicweb-geocoding-0.6.0/cubicweb_geocoding.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2022-11-24 01:41:12.000000 cubicweb-geocoding-0.6.0/cubicweb_geocoding.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-24 01:41:12.000000 cubicweb-geocoding-0.6.0/cubicweb_geocoding.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       25 2022-11-24 01:41:13.000000 cubicweb-geocoding-0.6.0/cubicweb_geocoding.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2022-11-24 01:41:13.000000 cubicweb-geocoding-0.6.0/cubicweb_geocoding.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-24 01:41:13.321990 cubicweb-geocoding-0.6.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2640 2022-11-24 01:40:58.000000 cubicweb-geocoding-0.6.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 01:41:13.321990 cubicweb-geocoding-0.6.0/test/
--rw-rw-rw-   0 root         (0) root         (0)     1705 2022-11-24 01:40:58.000000 cubicweb-geocoding-0.6.0/test/test_geocoding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 12:41:23.479435 cubicweb-geocoding-1.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      273 2023-08-02 12:40:54.000000 cubicweb-geocoding-1.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      543 2023-08-02 12:41:23.479435 cubicweb-geocoding-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-08-02 12:40:54.000000 cubicweb-geocoding-1.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 12:41:23.435434 cubicweb-geocoding-1.0.0/cubicweb_geocoding/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2023-08-02 12:40:54.000000 cubicweb-geocoding-1.0.0/cubicweb_geocoding/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      711 2023-08-02 12:40:54.000000 cubicweb-geocoding-1.0.0/cubicweb_geocoding/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 12:41:23.463435 cubicweb-geocoding-1.0.0/cubicweb_geocoding/data/
+-rw-rw-rw-   0 root         (0) root         (0)     3333 2023-08-02 12:40:54.000000 cubicweb-geocoding-1.0.0/cubicweb_geocoding/data/cubicweb.gmap.js
+-rw-rw-rw-   0 root         (0) root         (0)     2845 2023-08-02 12:40:54.000000 cubicweb-geocoding-1.0.0/cubicweb_geocoding/data/gmap.utility.labeledmarker.js
+-rw-rw-rw-   0 root         (0) root         (0)      869 2023-08-02 12:40:54.000000 cubicweb-geocoding-1.0.0/cubicweb_geocoding/data/gmap_blue_marker.png
+-rw-rw-rw-   0 root         (0) root         (0)     2789 2023-08-02 12:40:54.000000 cubicweb-geocoding-1.0.0/cubicweb_geocoding/geocoding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 12:41:23.463435 cubicweb-geocoding-1.0.0/cubicweb_geocoding/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-08-02 12:40:54.000000 cubicweb-geocoding-1.0.0/cubicweb_geocoding/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-08-02 12:40:54.000000 cubicweb-geocoding-1.0.0/cubicweb_geocoding/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-08-02 12:40:54.000000 cubicweb-geocoding-1.0.0/cubicweb_geocoding/i18n/fr.po
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-08-02 12:40:54.000000 cubicweb-geocoding-1.0.0/cubicweb_geocoding/site_cubicweb.py
+-rw-rw-rw-   0 root         (0) root         (0)     4909 2023-08-02 12:40:54.000000 cubicweb-geocoding-1.0.0/cubicweb_geocoding/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 12:41:23.447435 cubicweb-geocoding-1.0.0/cubicweb_geocoding.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      543 2023-08-02 12:41:23.000000 cubicweb-geocoding-1.0.0/cubicweb_geocoding.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-08-02 12:41:23.000000 cubicweb-geocoding-1.0.0/cubicweb_geocoding.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 12:41:23.000000 cubicweb-geocoding-1.0.0/cubicweb_geocoding.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-08-02 12:41:23.000000 cubicweb-geocoding-1.0.0/cubicweb_geocoding.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 12:41:23.000000 cubicweb-geocoding-1.0.0/cubicweb_geocoding.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       50 2023-08-02 12:41:23.000000 cubicweb-geocoding-1.0.0/cubicweb_geocoding.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-08-02 12:41:23.000000 cubicweb-geocoding-1.0.0/cubicweb_geocoding.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-02 12:41:23.479435 cubicweb-geocoding-1.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2608 2023-08-02 12:40:54.000000 cubicweb-geocoding-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 12:41:23.463435 cubicweb-geocoding-1.0.0/test/
+-rw-rw-rw-   0 root         (0) root         (0)     1706 2023-08-02 12:40:54.000000 cubicweb-geocoding-1.0.0/test/test_geocoding.py
```

### Comparing `cubicweb-geocoding-0.6.0/PKG-INFO` & `cubicweb-geocoding-1.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: cubicweb-geocoding
-Version: 0.6.0
+Version: 1.0.0
 Summary: geocoding views such as google maps
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-geocoding
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
 
 This is the geocoding cube.
 
 https://forge.extranet.logilab.fr/cubicweb/cubes/geocoding
-
-
```

### Comparing `cubicweb-geocoding-0.6.0/cubicweb_geocoding/data/cubicweb.gmap.js` & `cubicweb-geocoding-1.0.0/cubicweb_geocoding/data/cubicweb.gmap.js`

 * *Files identical despite different names*

### Comparing `cubicweb-geocoding-0.6.0/cubicweb_geocoding/data/gmap.utility.labeledmarker.js` & `cubicweb-geocoding-1.0.0/cubicweb_geocoding/data/gmap.utility.labeledmarker.js`

 * *Files identical despite different names*

### Comparing `cubicweb-geocoding-0.6.0/cubicweb_geocoding/data/gmap_blue_marker.png` & `cubicweb-geocoding-1.0.0/cubicweb_geocoding/data/gmap_blue_marker.png`

 * *Files identical despite different names*

### Comparing `cubicweb-geocoding-0.6.0/cubicweb_geocoding/geocoding.py` & `cubicweb-geocoding-1.0.0/cubicweb_geocoding/geocoding.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import print_function
-
 """geocoding module using google maps service
 
 Typical KML structure:
 <kml xmlns="http://earth.google.com/kml/2.0">
   <Response>
     <name>1600 amphitheatre mountain view ca</name>
     <Status>
@@ -42,49 +40,57 @@
 </kml>
 """
 
 import urllib
 
 from lxml import etree
 
-URL = 'http://maps.google.com/maps/geo?sensor=false&output=kml&q=%s&key=%s'
+URL = "http://maps.google.com/maps/geo?sensor=false&output=kml&q=%s&key=%s"
 
 NAMESPACES = {
-    'kml': "http://earth.google.com/kml/2.0",
+    "kml": "http://earth.google.com/kml/2.0",
 }
 
 
 def xpath(node, path):
     return node.xpath(path, namespaces=NAMESPACES)
 
 
 class UnknownAddress(Exception):
     """raise if an error occurs during geocoding process"""
 
 
 def extract_info(response):
     try:
-        code = int(xpath(response, 'kml:Response/kml:Status/kml:code/text()')[0])
+        code = int(xpath(response, "kml:Response/kml:Status/kml:code/text()")[0])
     except (IndexError, ValueError):
-        raise UnknownAddress('unable to read status code')
+        raise UnknownAddress("unable to read status code")
     if code != 200:
-        raise UnknownAddress('unable to find address info')
-    coords = xpath(response, 'kml:Response/kml:Placemark/kml:Point/kml:coordinates/text()')[0]
-    lng, lat, _ = [float(info) for info in coords.split(',')]
+        raise UnknownAddress("unable to find address info")
+    coords = xpath(
+        response, "kml:Response/kml:Placemark/kml:Point/kml:coordinates/text()"
+    )[0]
+    lng, lat, _ = (float(info) for info in coords.split(","))
     # XXX return city name / postalcode as returned by google ?
-    return {'latitude': lat, 'longitude': lng}
+    return {"latitude": lat, "longitude": lng}
 
 
 def get_latlng(address, gmapkey):
     try:
-        kml = urllib.urlopen(URL % (urllib.quote(address.encode('utf-8')), gmapkey)).read()
+        kml = urllib.urlopen(
+            URL % (urllib.quote(address.encode("utf-8")), gmapkey)
+        ).read()
         tree = etree.fromstring(kml)
         return extract_info(tree)
     except UnknownAddress:
         raise
     except Exception as exc:
-        raise UnknownAddress('%r (%s)' % (address, exc))
+        raise UnknownAddress(f"{address!r} ({exc})")
 
 
-if __name__ == '__main__':
-    print(get_latlng(u'10 rue Louis Vicat 75015 Paris',
-                     'ABQIAAAAAZKTE_iGKkEkfmJ-abtesRTwM0brOpm-All5BF6PoaKBxRWWERT7VGewoYPPmZ1Upon0H9cweSYQ0A'))
+if __name__ == "__main__":
+    print(
+        get_latlng(
+            "10 rue Louis Vicat 75015 Paris",
+            "ABQIAAAAAZKTE_iGKkEkfmJ-abtesRTwM0brOpm-All5BF6PoaKBxRWWERT7VGewoYPPmZ1Upon0H9cweSYQ0A",
+        )
+    )
```

### Comparing `cubicweb-geocoding-0.6.0/cubicweb_geocoding/views.py` & `cubicweb-geocoding-1.0.0/cubicweb_geocoding/views.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 from cubicweb.entity import EntityAdapter
 from cubicweb.predicates import adaptable
 from cubicweb.utils import json_dumps
 
 
 class IGeocodableAdapter(EntityAdapter):
     """interface required by geocoding views such as gmap-view"""
-    __regid__ = 'IGeocodable'
+
+    __regid__ = "IGeocodable"
     __abstract__ = True
 
     @property
     def latitude(self):
         """returns the latitude of the entity in degree (-90 < float < +90)"""
         raise NotImplementedError
 
@@ -43,92 +44,99 @@
     def marker_icon(self):
         """returns the icon that should be used as the marker.
 
         an icon is defined by a 4-uple:
 
           (icon._url, icon.size,  icon.iconAnchor, icon.shadow)
         """
-        return (self._cw.uiprops['GMARKER_ICON'], (20, 34), (4, 34), None)
+        return (self._cw.uiprops["GMARKER_ICON"], (20, 34), (4, 34), None)
 
 
 class GeocodingJsonView(EntityView):
-    __regid__ = 'geocoding-json'
-    __select__ = adaptable('IGeocodable')
+    __regid__ = "geocoding-json"
+    __select__ = adaptable("IGeocodable")
 
     binary = True
     templatable = False
-    content_type = 'application/json'
+    content_type = "application/json"
 
     def call(self):
-        zoomlevel = self._cw.form.pop('zoomlevel', None)
+        zoomlevel = self._cw.form.pop("zoomlevel", None)
         extraparams = self._cw.form.copy()
-        extraparams.pop('vid', None)
-        extraparams.pop('rql', None)
+        extraparams.pop("vid", None)
+        extraparams.pop("rql", None)
         markers = []
         for entity in self.cw_rset.entities():
-            igeocodable = entity.cw_adapt_to('IGeocodable')
+            igeocodable = entity.cw_adapt_to("IGeocodable")
             # remove entities that don't define latitude and longitude
             if not (igeocodable.latitude and igeocodable.longitude):
                 continue
-            markers.append(self.build_marker_data(entity, igeocodable,
-                                                  extraparams))
+            markers.append(self.build_marker_data(entity, igeocodable, extraparams))
         if not markers:
             return
         geodata = {
-            'markers': markers,
+            "markers": markers,
         }
         if zoomlevel:
-            geodata['zoomlevel'] = int(zoomlevel)
+            geodata["zoomlevel"] = int(zoomlevel)
         self.w(json_dumps(geodata))
 
     def build_marker_data(self, entity, igeocodable, extraparams):
-        return {'latitude': igeocodable.latitude,
-                'longitude': igeocodable.longitude,
-                'icon': igeocodable.marker_icon(),
-                'title': entity.dc_long_title(),
-                'bubbleUrl': entity.absolute_url(
-                    vid='gmap-bubble', __notemplate=1, **extraparams),
-                }
+        return {
+            "latitude": igeocodable.latitude,
+            "longitude": igeocodable.longitude,
+            "icon": igeocodable.marker_icon(),
+            "title": entity.dc_long_title(),
+            "bubbleUrl": entity.absolute_url(
+                vid="gmap-bubble", __notemplate=1, **extraparams
+            ),
+        }
 
 
 class GoogleMapBubbleView(EntityView):
-    __regid__ = 'gmap-bubble'
-    __select__ = adaptable('IGeocodable')
+    __regid__ = "gmap-bubble"
+    __select__ = adaptable("IGeocodable")
 
     def cell_call(self, row, col):
         entity = self.cw_rset.get_entity(row, col)
-        self.w(u'<div>%s</div>' % entity.view('oneline'))
+        self.w(f"<div>{entity.view('oneline')}</div>")
         # FIXME: we should call something like address-view if available
 
 
 class GoogleMapsView(EntityView):
-    __regid__ = 'gmap-view'
-    __select__ = adaptable('IGeocodable')
+    __regid__ = "gmap-view"
+    __select__ = adaptable("IGeocodable")
 
     paginable = False
 
     def call(self, gmap_key, width=400, height=400, uselabel=True, urlparams=None):
         self._cw.demote_to_html()
-        self._cw.add_js('http://maps.google.com/maps?sensor=false&file=api&v=2&key=%s'
-                        % gmap_key, localfile=False)
-        self._cw.add_js(('cubicweb.widgets.js', 'cubicweb.gmap.js', 'gmap.utility.labeledmarker.js'))
+        self._cw.add_js(
+            f"http://maps.google.com/maps?sensor=false&file=api&v=2&key={gmap_key}",
+            localfile=False,
+        )
+        self._cw.add_js(
+            ("cubicweb.widgets.js", "cubicweb.gmap.js", "gmap.utility.labeledmarker.js")
+        )
         rql = self.cw_rset.printable_rql()
         if urlparams is None:
-            loadurl = self._cw.build_url(rql=rql, vid='geocoding-json')
+            loadurl = self._cw.build_url(rql=rql, vid="geocoding-json")
         else:
-            loadurl = self._cw.build_url(rql=rql, vid='geocoding-json', **urlparams)
-        self.w(u'<div style="width: %spx; height: %spx;" class="widget gmap" '
-               u'cubicweb:wdgtype="GMapWidget" cubicweb:loadtype="auto" '
-               u'cubicweb:loadurl="%s" cubicweb:uselabel="%s"> </div>'
-               % (width, height, loadurl, uselabel))
+            loadurl = self._cw.build_url(rql=rql, vid="geocoding-json", **urlparams)
+        self.w(
+            '<div style="width: %spx; height: %spx;" class="widget gmap" '
+            'cubicweb:wdgtype="GMapWidget" cubicweb:loadtype="auto" '
+            'cubicweb:loadurl="%s" cubicweb:uselabel="%s"> </div>'
+            % (width, height, loadurl, uselabel)
+        )
 
 
 class GoogeMapsLegend(EntityView):
-    __regid__ = 'gmap-legend'
+    __regid__ = "gmap-legend"
 
     def call(self):
-        self.w(u'<ol>')
+        self.w("<ol>")
         for rowidx in range(len(self.cw_rset)):
-            self.w(u'<li>')
-            self.wview('listitem', self.cw_rset, row=rowidx, col=0)
-            self.w(u'</li>')
-        self.w(u'</ol>')
+            self.w("<li>")
+            self.wview("listitem", self.cw_rset, row=rowidx, col=0)
+            self.w("</li>")
+        self.w("</ol>")
```

### Comparing `cubicweb-geocoding-0.6.0/cubicweb_geocoding.egg-info/PKG-INFO` & `cubicweb-geocoding-1.0.0/cubicweb_geocoding.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: cubicweb-geocoding
-Version: 0.6.0
+Version: 1.0.0
 Summary: geocoding views such as google maps
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-geocoding
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
 
 This is the geocoding cube.
 
 https://forge.extranet.logilab.fr/cubicweb/cubes/geocoding
-
-
```

### Comparing `cubicweb-geocoding-0.6.0/cubicweb_geocoding.egg-info/SOURCES.txt` & `cubicweb-geocoding-1.0.0/cubicweb_geocoding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-geocoding-0.6.0/setup.py` & `cubicweb-geocoding-1.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,56 +27,55 @@
 from setuptools import find_packages, setup
 
 
 here = dirname(__file__)
 
 # load metadata from the __pkginfo__.py file so there is no risk of conflict
 # see https://packaging.python.org/en/latest/single_source_version.html
-pkginfo = join(here, 'cubicweb_geocoding', '__pkginfo__.py')
+pkginfo = join(here, "cubicweb_geocoding", "__pkginfo__.py")
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
-            'geocoding=cubicweb_geocoding',
+        "cubicweb.cubes": [
+            "geocoding=cubicweb_geocoding",
         ],
     },
     zip_safe=False,
 )
```

### Comparing `cubicweb-geocoding-0.6.0/test/test_geocoding.py` & `cubicweb-geocoding-1.0.0/test/test_geocoding.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,13 +38,14 @@
 """
 
 from cubicweb.devtools import testlib
 
 
 class DefaultTC(testlib.CubicWebTC):
     def test_something(self):
-        self.skipTest('this cube has no test')
+        self.skipTest("this cube has no test")
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     import unittest
+
     unittest.main()
```

