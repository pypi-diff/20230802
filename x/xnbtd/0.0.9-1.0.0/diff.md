# Comparing `tmp/xnbtd-0.0.9.tar.gz` & `tmp/xnbtd-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xnbtd-0.0.9.tar", max compression
+gzip compressed data, was "xnbtd-1.0.0.tar", max compression
```

## Comparing `xnbtd-0.0.9.tar` & `xnbtd-1.0.0.tar`

### file list

```diff
@@ -1,41 +1,43 @@
--rwxr-xr-x   0        0        0    35149 2023-07-17 12:58:10.128808 xnbtd-0.0.9/LICENSE
--rwxr-xr-x   0        0        0     1537 2023-07-17 13:41:38.389506 xnbtd-0.0.9/README.md
--rwxr-xr-x   0        0        0     3622 2023-07-21 21:55:24.583110 xnbtd-0.0.9/pyproject.toml
--rwxr-xr-x   0        0        0      222 2023-07-21 21:52:15.409174 xnbtd-0.0.9/xnbtd/__init__.py
--rwxr-xr-x   0        0        0      281 2023-07-20 13:58:05.853446 xnbtd-0.0.9/xnbtd/admin.py
--rwxr-xr-x   0        0        0      288 2023-07-21 21:49:55.059033 xnbtd-0.0.9/xnbtd/apps.py
--rwxr-xr-x   0        0        0      167 2023-07-17 13:12:55.756710 xnbtd-0.0.9/xnbtd/asgi.py
--rwxr-xr-x   0        0        0      610 2023-07-21 21:03:24.000000 xnbtd-0.0.9/xnbtd/locale/fr/LC_MESSAGES/django.mo
--rwxr-xr-x   0        0        0     1080 2023-07-21 21:02:51.383951 xnbtd-0.0.9/xnbtd/locale/fr/LC_MESSAGES/django.po
--rwxr-xr-x   0        0        0      794 2023-07-21 21:52:56.078123 xnbtd-0.0.9/xnbtd/migrations/0001_initial.py
--rwxr-xr-x   0        0        0        0 2023-07-21 21:39:32.426120 xnbtd-0.0.9/xnbtd/migrations/__init__.py
--rwxr-xr-x   0        0        0        0 2023-07-18 14:26:39.334718 xnbtd-0.0.9/xnbtd/plannings/__init__.py
--rwxr-xr-x   0        0        0      389 2023-07-17 14:30:12.899432 xnbtd-0.0.9/xnbtd/plannings/admin.py
--rwxr-xr-x   0        0        0      262 2023-07-17 17:19:57.751481 xnbtd-0.0.9/xnbtd/plannings/apps.py
--rwxr-xr-x   0        0        0      581 2023-07-21 21:03:24.000000 xnbtd-0.0.9/xnbtd/plannings/locale/fr/LC_MESSAGES/django.mo
--rwxr-xr-x   0        0        0      953 2023-07-21 21:02:51.303633 xnbtd-0.0.9/xnbtd/plannings/locale/fr/LC_MESSAGES/django.po
--rwxr-xr-x   0        0        0      914 2023-07-21 21:35:35.367721 xnbtd-0.0.9/xnbtd/plannings/migrations/0001_initial.py
--rwxr-xr-x   0        0        0        0 2023-07-20 11:49:50.131931 xnbtd-0.0.9/xnbtd/plannings/migrations/__init__.py
--rwxr-xr-x   0        0        0      421 2023-07-17 14:12:11.523365 xnbtd-0.0.9/xnbtd/plannings/models.py
--rwxr-xr-x   0        0        0      584 2023-07-17 17:06:06.530198 xnbtd-0.0.9/xnbtd/publish.py
--rwxr-xr-x   0        0        0        0 2023-07-17 12:58:01.655818 xnbtd-0.0.9/xnbtd/settings/__init__.py
--rwxr-xr-x   0        0        0     5841 2023-07-21 20:58:24.764238 xnbtd-0.0.9/xnbtd/settings/base.py
--rwxr-xr-x   0        0        0     1554 2023-07-17 13:22:20.009794 xnbtd-0.0.9/xnbtd/settings/local.py
--rwxr-xr-x   0        0        0      157 2023-07-17 15:13:41.392423 xnbtd-0.0.9/xnbtd/settings/prod.py
--rwxr-xr-x   0        0        0      220 2023-07-17 13:22:25.149688 xnbtd-0.0.9/xnbtd/settings/test.py
--rwxr-xr-x   0        0        0     1391 2023-07-21 21:31:26.839640 xnbtd-0.0.9/xnbtd/templates/xnbtd/admin/change_list.html
--rwxr-xr-x   0        0        0     1656 2023-07-20 12:50:03.246479 xnbtd-0.0.9/xnbtd/templates/xnbtd/admin/index.html
--rwxr-xr-x   0        0        0      849 2023-07-19 05:10:22.167337 xnbtd-0.0.9/xnbtd/templatetags/events.py
--rwxr-xr-x   0        0        0     1383 2023-07-21 21:53:11.656492 xnbtd-0.0.9/xnbtd/templatetags/tours.py
--rwxr-xr-x   0        0        0        0 2023-07-18 14:26:50.555819 xnbtd-0.0.9/xnbtd/tours/__init__.py
--rwxr-xr-x   0        0        0    10206 2023-07-21 21:53:23.129533 xnbtd-0.0.9/xnbtd/tours/admin.py
--rwxr-xr-x   0        0        0      250 2023-07-17 17:18:19.849741 xnbtd-0.0.9/xnbtd/tours/apps.py
--rwxr-xr-x   0        0        0      401 2023-07-17 14:19:16.195276 xnbtd-0.0.9/xnbtd/tours/forms.py
--rwxr-xr-x   0        0        0     4392 2023-07-21 21:03:25.000000 xnbtd-0.0.9/xnbtd/tours/locale/fr/LC_MESSAGES/django.mo
--rwxr-xr-x   0        0        0     7986 2023-07-21 21:02:51.223602 xnbtd-0.0.9/xnbtd/tours/locale/fr/LC_MESSAGES/django.po
--rwxr-xr-x   0        0        0     8264 2023-07-21 21:35:35.397000 xnbtd-0.0.9/xnbtd/tours/migrations/0001_initial.py
--rwxr-xr-x   0        0        0        0 2023-07-20 11:49:44.075539 xnbtd-0.0.9/xnbtd/tours/migrations/__init__.py
--rwxr-xr-x   0        0        0     7296 2023-07-21 21:53:41.456419 xnbtd-0.0.9/xnbtd/tours/models.py
--rwxr-xr-x   0        0        0      120 2023-07-21 08:12:20.934692 xnbtd-0.0.9/xnbtd/urls.py
--rwxr-xr-x   0        0        0      167 2023-07-17 13:21:04.199785 xnbtd-0.0.9/xnbtd/wsgi.py
--rw-r--r--   0        0        0     2467 1970-01-01 00:00:00.000000 xnbtd-0.0.9/PKG-INFO
+-rwxr-xr-x   0        0        0    35149 2023-07-17 12:58:10.128808 xnbtd-1.0.0/LICENSE
+-rwxr-xr-x   0        0        0     1537 2023-07-17 13:41:38.389506 xnbtd-1.0.0/README.md
+-rwxr-xr-x   0        0        0     3622 2023-08-02 17:52:14.796219 xnbtd-1.0.0/pyproject.toml
+-rwxr-xr-x   0        0        0      222 2023-07-21 21:52:15.409174 xnbtd-1.0.0/xnbtd/__init__.py
+-rwxr-xr-x   0        0        0      281 2023-07-24 18:46:24.620500 xnbtd-1.0.0/xnbtd/admin.py
+-rwxr-xr-x   0        0        0      288 2023-07-21 21:49:55.059033 xnbtd-1.0.0/xnbtd/apps.py
+-rwxr-xr-x   0        0        0      167 2023-07-17 13:12:55.756710 xnbtd-1.0.0/xnbtd/asgi.py
+-rwxr-xr-x   0        0        0      610 2023-08-02 17:47:49.000000 xnbtd-1.0.0/xnbtd/locale/fr/LC_MESSAGES/django.mo
+-rwxr-xr-x   0        0        0     1080 2023-08-02 17:47:22.504710 xnbtd-1.0.0/xnbtd/locale/fr/LC_MESSAGES/django.po
+-rwxr-xr-x   0        0        0        0 2023-07-18 14:26:39.334718 xnbtd-1.0.0/xnbtd/plannings/__init__.py
+-rwxr-xr-x   0        0        0      389 2023-07-17 14:30:12.899432 xnbtd-1.0.0/xnbtd/plannings/admin.py
+-rwxr-xr-x   0        0        0      262 2023-07-17 17:19:57.751481 xnbtd-1.0.0/xnbtd/plannings/apps.py
+-rwxr-xr-x   0        0        0      581 2023-08-02 17:47:50.000000 xnbtd-1.0.0/xnbtd/plannings/locale/fr/LC_MESSAGES/django.mo
+-rwxr-xr-x   0        0        0      953 2023-08-02 17:47:22.441722 xnbtd-1.0.0/xnbtd/plannings/locale/fr/LC_MESSAGES/django.po
+-rwxr-xr-x   0        0        0      914 2023-07-21 21:35:35.367721 xnbtd-1.0.0/xnbtd/plannings/migrations/0001_initial.py
+-rwxr-xr-x   0        0        0        0 2023-07-20 11:49:50.131931 xnbtd-1.0.0/xnbtd/plannings/migrations/__init__.py
+-rwxr-xr-x   0        0        0      421 2023-07-17 14:12:11.523365 xnbtd-1.0.0/xnbtd/plannings/models.py
+-rwxr-xr-x   0        0        0      584 2023-07-17 17:06:06.530198 xnbtd-1.0.0/xnbtd/publish.py
+-rwxr-xr-x   0        0        0        0 2023-07-17 12:58:01.655818 xnbtd-1.0.0/xnbtd/settings/__init__.py
+-rwxr-xr-x   0        0        0     5841 2023-07-21 20:58:24.764238 xnbtd-1.0.0/xnbtd/settings/base.py
+-rwxr-xr-x   0        0        0     1554 2023-07-17 13:22:20.009794 xnbtd-1.0.0/xnbtd/settings/local.py
+-rwxr-xr-x   0        0        0      157 2023-07-17 15:13:41.392423 xnbtd-1.0.0/xnbtd/settings/prod.py
+-rwxr-xr-x   0        0        0      220 2023-07-17 13:22:25.149688 xnbtd-1.0.0/xnbtd/settings/test.py
+-rwxr-xr-x   0        0        0     1391 2023-07-21 21:31:26.839640 xnbtd-1.0.0/xnbtd/templates/xnbtd/admin/change_list.html
+-rwxr-xr-x   0        0        0     1656 2023-07-20 12:50:03.246479 xnbtd-1.0.0/xnbtd/templates/xnbtd/admin/index.html
+-rwxr-xr-x   0        0        0      849 2023-07-19 05:10:22.167337 xnbtd-1.0.0/xnbtd/templatetags/events.py
+-rwxr-xr-x   0        0        0     1499 2023-07-24 16:48:20.567679 xnbtd-1.0.0/xnbtd/templatetags/tours.py
+-rwxr-xr-x   0        0        0        0 2023-07-18 14:26:50.555819 xnbtd-1.0.0/xnbtd/tours/__init__.py
+-rwxr-xr-x   0        0        0    16856 2023-08-02 17:39:30.074888 xnbtd-1.0.0/xnbtd/tours/admin.py
+-rwxr-xr-x   0        0        0      250 2023-07-17 17:18:19.849741 xnbtd-1.0.0/xnbtd/tours/apps.py
+-rwxr-xr-x   0        0        0      401 2023-07-17 14:19:16.195276 xnbtd-1.0.0/xnbtd/tours/forms.py
+-rwxr-xr-x   0        0        0     4732 2023-08-02 17:47:50.000000 xnbtd-1.0.0/xnbtd/tours/locale/fr/LC_MESSAGES/django.mo
+-rwxr-xr-x   0        0        0     8447 2023-08-02 17:48:31.196994 xnbtd-1.0.0/xnbtd/tours/locale/fr/LC_MESSAGES/django.po
+-rwxr-xr-x   0        0        0     8264 2023-07-21 21:35:35.397000 xnbtd-1.0.0/xnbtd/tours/migrations/0001_initial.py
+-rwxr-xr-x   0        0        0     1912 2023-07-24 15:47:49.294370 xnbtd-1.0.0/xnbtd/tours/migrations/0002_chronopostpickup_and_more.py
+-rwxr-xr-x   0        0        0     2282 2023-07-24 16:10:57.506588 xnbtd-1.0.0/xnbtd/tours/migrations/0003_chronopostdelivery_linked_user_and_more.py
+-rwxr-xr-x   0        0        0      826 2023-07-24 19:00:42.569177 xnbtd-1.0.0/xnbtd/tours/migrations/0004_alter_chronopostdelivery_options_and_more.py
+-rwxr-xr-x   0        0        0     1121 2023-08-02 17:41:02.878443 xnbtd-1.0.0/xnbtd/tours/migrations/0005_alter_chronopostdelivery_options_and_more.py
+-rwxr-xr-x   0        0        0        0 2023-07-20 11:49:44.075539 xnbtd-1.0.0/xnbtd/tours/migrations/__init__.py
+-rwxr-xr-x   0        0        0     4777 2023-08-02 17:39:56.090739 xnbtd-1.0.0/xnbtd/tours/models.py
+-rwxr-xr-x   0        0        0      120 2023-07-21 08:12:20.934692 xnbtd-1.0.0/xnbtd/urls.py
+-rwxr-xr-x   0        0        0      167 2023-07-17 13:21:04.199785 xnbtd-1.0.0/xnbtd/wsgi.py
+-rw-r--r--   0        0        0     2467 1970-01-01 00:00:00.000000 xnbtd-1.0.0/PKG-INFO
```

### Comparing `xnbtd-0.0.9/LICENSE` & `xnbtd-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.9/README.md` & `xnbtd-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.9/pyproject.toml` & `xnbtd-1.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xnbtd"
-version = "0.0.9"
+version = "1.0.0"
 description = "xNBTD est une application de gestion pour entreprise de livraison. Elle facilite la gestion des tournées et des plannings."
 authors = [
     "André Théo LAURET <andrelauret@eclipse-technology.eu>",
 ]
 maintainers = [
     "André Théo LAURET <andrelauret@eclipse-technology.eu>",
 ]
```

### Comparing `xnbtd-0.0.9/xnbtd/locale/fr/LC_MESSAGES/django.mo` & `xnbtd-1.0.0/xnbtd/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.9/xnbtd/locale/fr/LC_MESSAGES/django.po` & `xnbtd-1.0.0/xnbtd/locale/fr/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-21 08:27+0000\n"
+"POT-Creation-Date: 2023-07-24 15:32+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
-#: xnbtd/templates/xnbtd/admin/change_list.html:8
+#: xnbtd/templates/xnbtd/admin/change_list.html:7
 msgid "Statistic"
 msgstr "Statistique"
 
-#: xnbtd/templates/xnbtd/admin/change_list.html:12
+#: xnbtd/templates/xnbtd/admin/change_list.html:14
 msgid "Filter"
 msgstr "Filtre"
 
-#: xnbtd/templates/xnbtd/admin/change_list.html:18
+#: xnbtd/templates/xnbtd/admin/change_list.html:20
 msgid "Hide counts"
 msgstr "Cacher"
 
-#: xnbtd/templates/xnbtd/admin/change_list.html:20
+#: xnbtd/templates/xnbtd/admin/change_list.html:22
 msgid "Show counts"
 msgstr "Afficher"
 
-#: xnbtd/templates/xnbtd/admin/change_list.html:26
+#: xnbtd/templates/xnbtd/admin/change_list.html:28
 msgid "Clear all filters"
 msgstr "Effacer tous les filtres"
```

### Comparing `xnbtd-0.0.9/xnbtd/plannings/locale/fr/LC_MESSAGES/django.mo` & `xnbtd-1.0.0/xnbtd/plannings/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.9/xnbtd/plannings/locale/fr/LC_MESSAGES/django.po` & `xnbtd-1.0.0/xnbtd/plannings/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.9/xnbtd/plannings/migrations/0001_initial.py` & `xnbtd-1.0.0/xnbtd/plannings/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.9/xnbtd/publish.py` & `xnbtd-1.0.0/xnbtd/publish.py`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.9/xnbtd/settings/base.py` & `xnbtd-1.0.0/xnbtd/settings/base.py`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.9/xnbtd/settings/local.py` & `xnbtd-1.0.0/xnbtd/settings/local.py`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.9/xnbtd/templates/xnbtd/admin/change_list.html` & `xnbtd-1.0.0/xnbtd/templates/xnbtd/admin/change_list.html`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.9/xnbtd/templates/xnbtd/admin/index.html` & `xnbtd-1.0.0/xnbtd/templates/xnbtd/admin/index.html`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.9/xnbtd/templatetags/events.py` & `xnbtd-1.0.0/xnbtd/templatetags/events.py`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.9/xnbtd/templatetags/tours.py` & `xnbtd-1.0.0/xnbtd/templatetags/tours.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,30 +13,31 @@
     Calculate the total for a given column in a queryset
 
     Arguments:
         queryset (QuerySet): The queryset that is being used to calculate the total.
         column (str): The column for which the total is being calculated.
 
     Returns:
-        float: The total of the column rounded to two decimal places
+        float or None: The total of the column rounded to two decimal places,
+        or None if the total is None.
     """
     if queryset.exists():
         model_class = queryset.model
         field_type = model_class._meta.get_field(column).get_internal_type()
 
         if field_type in ('IntegerField', 'FloatField'):
             total = queryset.aggregate(total=Sum(column)).get('total')
-            return round(total, 2)
+            return round(total, 2) if total is not None else None
         elif field_type == 'TimeField':
             total_time = timedelta()
 
             for item in queryset:
                 value = getattr(item, column)
                 if value:
                     total_time += timedelta(hours=value.hour, minutes=value.minute,
                                             seconds=value.second)
 
             # Calculate total hours and round to 2 decimal places
             total_hours = total_time.total_seconds() / 3600
-            return round(total_hours, 2)
+            return round(total_hours, 2) if total_hours is not None else None
 
     return None
```

### Comparing `xnbtd-0.0.9/xnbtd/tours/locale/fr/LC_MESSAGES/django.mo` & `xnbtd-1.0.0/xnbtd/tours/locale/fr/LC_MESSAGES/django.mo`

 * *Files 15% similar despite different names*

#### msgunfmt {}

```diff
@@ -14,39 +14,48 @@
 msgid "AVP Relay"
 msgstr "AVP Relais"
 
 msgid "Anomalies"
 msgstr "Anomalies"
 
 msgid "Beginning Hour"
-msgstr "début de la tournée"
+msgstr "début de la journée"
 
 msgid "Breaks"
 msgstr "pauses"
 
 msgid "Charged Packages"
 msgstr "Colis chargé"
 
 msgid "Charged Points"
 msgstr "Points chargés"
 
-msgid "Chronopost"
-msgstr "Chronopost"
+msgid "Chronopost Delivery"
+msgstr "Chronopost - Livraison"
+
+msgid "Chronopost Pickup"
+msgstr "Chronopost - Ramasse"
 
 msgid "Ciblex"
 msgstr "Ciblex"
 
 msgid "Client numbers"
 msgstr "Nombres clients"
 
+msgid "Deliveryman"
+msgstr "livreur"
+
 msgid "EO"
 msgstr "EO"
 
+msgid "ESD"
+msgstr "ESD"
+
 msgid "Ending Hour"
-msgstr "fin de la tournée"
+msgstr "fin de la journée"
 
 msgid "Full KM"
 msgstr "Plein / KM"
 
 msgid "GLS"
 msgstr "GLS"
 
@@ -61,23 +70,29 @@
 
 msgid "Packages Charges"
 msgstr "Colis chargés"
 
 msgid "Packages Delivered"
 msgstr "Colis livrés"
 
+msgid "Picked Points"
+msgstr "Point ramassés"
+
 msgid "Pickup Point"
 msgstr "Point de ramasse"
 
 msgid "Points Charges"
 msgstr "Points chargés"
 
 msgid "Points Delivered"
 msgstr "Points livrés"
 
+msgid "Poste"
+msgstr "Poste"
+
 msgid "Refused"
 msgstr "refuse"
 
 msgid "Relay"
 msgstr "Relais"
 
 msgid "Return Packages"
@@ -85,38 +100,41 @@
 
 msgid "Return Points"
 msgstr "Retour POINTS"
 
 msgid "SHD"
 msgstr "SHD"
 
-msgid "TNT - Fedex"
+msgid "TNT"
 msgstr "TNT - Fedex"
 
 msgid "Total Break Hours"
 msgstr "Total d’heures de pause"
 
 msgid "Total Clients"
 msgstr "Totals clients"
 
 msgid "Total Days"
 msgstr "Total de jours"
 
 msgid "Total Hour"
-msgstr "Durée de la tournée"
+msgstr "Durée de la journée"
 
 msgid "Total Packages Delivered"
 msgstr "Total colis livrés"
 
 msgid "Total Points"
 msgstr "Total points"
 
 msgid "Total Work Hours"
 msgstr "Total d’heures de travail"
 
+msgid "Total of Picked Points"
+msgstr "Total de points ramassés"
+
 msgid "Total of Points"
 msgstr "Total de points"
 
 msgid "Tour Date"
 msgstr "date"
 
 msgid "Tour Name"
@@ -131,15 +149,15 @@
 msgid "avp"
 msgstr "avp"
 
 msgid "avp_relay"
 msgstr "avp relais"
 
 msgid "beginning_hour"
-msgstr "début de la tournée"
+msgstr "début de la journée"
 
 msgid "breaks"
 msgstr "pauses"
 
 msgid "cad"
 msgstr "cad"
 
@@ -151,29 +169,29 @@
 
 msgid "charged_points"
 msgstr "points chargés"
 
 msgid "client_numbers"
 msgstr "nombres clients"
 
-msgid "code"
-msgstr "code"
-
 msgid "date"
 msgstr "date"
 
 msgid "days"
 msgstr "jours"
 
 msgid "ending_hour"
-msgstr "fin de la tournée"
+msgstr "fin de la journée"
 
 msgid "eo"
 msgstr "eo"
 
+msgid "esd"
+msgstr "esd"
+
 msgid "full_km"
 msgstr "plein / km"
 
 msgid "including_ip"
 msgstr "dont ip"
 
 msgid "kilometers"
@@ -202,23 +220,29 @@
 
 msgid "packages_charges"
 msgstr "colis chargés"
 
 msgid "packages_delivered"
 msgstr "colis livrés"
 
+msgid "picked_points"
+msgstr "points ramassés"
+
 msgid "pickup_point"
 msgstr "point de ramasse"
 
 msgid "points_charges"
 msgstr "points chargés"
 
 msgid "points_delivered"
 msgstr "points livrés"
 
+msgid "poste"
+msgstr "poste"
+
 msgid "refused"
 msgstr "refuse"
 
 msgid "regular abductions"
 msgstr "enlèvements réguliers"
 
 msgid "regular_abductions"
@@ -245,15 +269,15 @@
 msgid "synchro"
 msgstr "synchro"
 
 msgid "total clients abductions"
 msgstr "totals clients enlèvements"
 
 msgid "total_hour"
-msgstr "Durée de la tournée"
+msgstr "Durée de la journée"
 
 msgid "total_points"
 msgstr "total points"
 
 msgid "totals clients"
 msgstr "totals client"
```

### Comparing `xnbtd-0.0.9/xnbtd/tours/locale/fr/LC_MESSAGES/django.po` & `xnbtd-1.0.0/xnbtd/tours/locale/fr/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -3,370 +3,398 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-21 21:01+0000\n"
+"POT-Creation-Date: 2023-08-02 17:47+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
-#: xnbtd/tours/admin.py:14 xnbtd/tours/admin.py:41 xnbtd/tours/admin.py:69
-#: xnbtd/tours/admin.py:94
+#: xnbtd/tours/admin.py:14 xnbtd/tours/admin.py:42 xnbtd/tours/admin.py:71
+#: xnbtd/tours/admin.py:97 xnbtd/tours/admin.py:114 xnbtd/tours/models.py:10
+msgid "Deliveryman"
+msgstr "livreur"
+
+#: xnbtd/tours/admin.py:15 xnbtd/tours/admin.py:43 xnbtd/tours/admin.py:72
+#: xnbtd/tours/admin.py:98 xnbtd/tours/admin.py:115
 msgid "name"
 msgstr "nom"
 
-#: xnbtd/tours/admin.py:15 xnbtd/tours/admin.py:42 xnbtd/tours/admin.py:70
-#: xnbtd/tours/admin.py:95
+#: xnbtd/tours/admin.py:16 xnbtd/tours/admin.py:44 xnbtd/tours/admin.py:73
+#: xnbtd/tours/admin.py:99 xnbtd/tours/admin.py:116
 msgid "date"
 msgstr "date"
 
-#: xnbtd/tours/admin.py:16
+#: xnbtd/tours/admin.py:17
 msgid "points_charges"
 msgstr "points chargés"
 
-#: xnbtd/tours/admin.py:18
+#: xnbtd/tours/admin.py:19
 msgid "points_delivered"
 msgstr "points livrés"
 
-#: xnbtd/tours/admin.py:21
+#: xnbtd/tours/admin.py:22
 msgid "packages_charges"
 msgstr "colis chargés"
 
-#: xnbtd/tours/admin.py:24
+#: xnbtd/tours/admin.py:25
 msgid "packages_delivered"
 msgstr "colis livrés"
 
-#: xnbtd/tours/admin.py:26
+#: xnbtd/tours/admin.py:27
 msgid "avp_relay"
 msgstr "avp relais"
 
-#: xnbtd/tours/admin.py:27
+#: xnbtd/tours/admin.py:28
 msgid "shd"
 msgstr "shd"
 
-#: xnbtd/tours/admin.py:28
+#: xnbtd/tours/admin.py:29
 msgid "eo"
 msgstr "eo"
 
-#: xnbtd/tours/admin.py:29
+#: xnbtd/tours/admin.py:30
 msgid "pickup_point"
 msgstr "point de ramasse"
 
-#: xnbtd/tours/admin.py:30 xnbtd/tours/admin.py:58 xnbtd/tours/admin.py:83
-#: xnbtd/tours/admin.py:104 xnbtd/tours/models.py:96
+#: xnbtd/tours/admin.py:31 xnbtd/tours/admin.py:60 xnbtd/tours/admin.py:86
+#: xnbtd/tours/admin.py:103 xnbtd/tours/admin.py:124
 msgid "breaks"
 msgstr "pauses"
 
-#: xnbtd/tours/admin.py:31 xnbtd/tours/admin.py:59 xnbtd/tours/admin.py:84
-#: xnbtd/tours/admin.py:105
+#: xnbtd/tours/admin.py:32 xnbtd/tours/admin.py:61 xnbtd/tours/admin.py:87
+#: xnbtd/tours/admin.py:104 xnbtd/tours/admin.py:125
 msgid "beginning_hour"
-msgstr "début de la tournée"
+msgstr "début de la journée"
 
-#: xnbtd/tours/admin.py:32 xnbtd/tours/admin.py:60 xnbtd/tours/admin.py:85
-#: xnbtd/tours/admin.py:106
+#: xnbtd/tours/admin.py:33 xnbtd/tours/admin.py:62 xnbtd/tours/admin.py:88
+#: xnbtd/tours/admin.py:105 xnbtd/tours/admin.py:126
 msgid "ending_hour"
-msgstr "fin de la tournée"
+msgstr "fin de la journée"
 
-#: xnbtd/tours/admin.py:33 xnbtd/tours/admin.py:61 xnbtd/tours/admin.py:86
-#: xnbtd/tours/admin.py:107
+#: xnbtd/tours/admin.py:34 xnbtd/tours/admin.py:63 xnbtd/tours/admin.py:89
+#: xnbtd/tours/admin.py:106 xnbtd/tours/admin.py:127
 msgid "total_hour"
-msgstr "Durée de la tournée"
+msgstr "Durée de la journée"
 
-#: xnbtd/tours/admin.py:43
+#: xnbtd/tours/admin.py:45
 msgid "client_numbers"
 msgstr "nombres clients"
 
-#: xnbtd/tours/admin.py:44
+#: xnbtd/tours/admin.py:46
 msgid "refused"
 msgstr "refuse"
 
-#: xnbtd/tours/admin.py:45 xnbtd/tours/admin.py:100 xnbtd/tours/models.py:89
-#: xnbtd/tours/models.py:138
+#: xnbtd/tours/admin.py:47 xnbtd/tours/admin.py:120 xnbtd/tours/models.py:85
+#: xnbtd/tours/models.py:102
 msgid "avp"
 msgstr "avp"
 
-#: xnbtd/tours/admin.py:46
+#: xnbtd/tours/admin.py:48
 msgid "cad"
 msgstr "cad"
 
-#: xnbtd/tours/admin.py:47
+#: xnbtd/tours/admin.py:49
 msgid "totals_clients"
 msgstr "totals client"
 
-#: xnbtd/tours/admin.py:49
+#: xnbtd/tours/admin.py:51
 msgid "occasional_abductions"
 msgstr "enlèvements occasionnels"
 
-#: xnbtd/tours/admin.py:52
+#: xnbtd/tours/admin.py:54
 msgid "regular_abductions"
 msgstr "enlèvements réguliers"
 
-#: xnbtd/tours/admin.py:55
+#: xnbtd/tours/admin.py:57
 msgid "totals_clients_abductions"
 msgstr "totals clients enlèvements"
 
-#: xnbtd/tours/admin.py:57
+#: xnbtd/tours/admin.py:59
 msgid "kilometers"
 msgstr "kilomètres"
 
-#: xnbtd/tours/admin.py:72
+#: xnbtd/tours/admin.py:75
 msgid "charged_packages"
 msgstr "colis chargé"
 
-#: xnbtd/tours/admin.py:74
+#: xnbtd/tours/admin.py:77
 msgid "charged_points"
 msgstr "points chargés"
 
-#: xnbtd/tours/admin.py:75
+#: xnbtd/tours/admin.py:78
 msgid "including_ip"
 msgstr "dont ip"
 
-#: xnbtd/tours/admin.py:76
+#: xnbtd/tours/admin.py:79
 msgid "relay"
 msgstr "relais"
 
-#: xnbtd/tours/admin.py:77
+#: xnbtd/tours/admin.py:80
 msgid "return_packages"
 msgstr "retour colis"
 
-#: xnbtd/tours/admin.py:78
+#: xnbtd/tours/admin.py:81
 msgid "return_points"
 msgstr "retour points"
 
-#: xnbtd/tours/admin.py:79
+#: xnbtd/tours/admin.py:82
 msgid "overdue"
 msgstr "hors délais"
 
-#: xnbtd/tours/admin.py:80
+#: xnbtd/tours/admin.py:83
 msgid "anomalies"
 msgstr "anomalies"
 
-#: xnbtd/tours/admin.py:81
+#: xnbtd/tours/admin.py:84
 msgid "total_points"
 msgstr "total points"
 
-#: xnbtd/tours/admin.py:82
+#: xnbtd/tours/admin.py:85
 msgid "full_km"
 msgstr "plein / km"
 
-#: xnbtd/tours/admin.py:96
+#: xnbtd/tours/admin.py:100
+msgid "esd"
+msgstr "esd"
+
+#: xnbtd/tours/admin.py:101
+msgid "picked_points"
+msgstr "points ramassés"
+
+#: xnbtd/tours/admin.py:102
+msgid "poste"
+msgstr "poste"
+
+#: xnbtd/tours/admin.py:117
 msgid "type"
 msgstr "type"
 
-#: xnbtd/tours/admin.py:97
-msgid "code"
-msgstr "code"
-
-#: xnbtd/tours/admin.py:98 xnbtd/tours/models.py:136
+#: xnbtd/tours/admin.py:118 xnbtd/tours/models.py:100
 msgid "nights"
 msgstr "nuits"
 
-#: xnbtd/tours/admin.py:99 xnbtd/tours/models.py:137
+#: xnbtd/tours/admin.py:119 xnbtd/tours/models.py:101
 msgid "days"
 msgstr "jours"
 
-#: xnbtd/tours/admin.py:101
+#: xnbtd/tours/admin.py:121
 msgid "spare_part"
 msgstr "spare part"
 
-#: xnbtd/tours/admin.py:102 xnbtd/tours/models.py:140
+#: xnbtd/tours/admin.py:122 xnbtd/tours/models.py:104
 msgid "synchro"
 msgstr "synchro"
 
-#: xnbtd/tours/admin.py:103
+#: xnbtd/tours/admin.py:123
 msgid "morning_pickup"
 msgstr "ramassages matin"
 
-#: xnbtd/tours/admin.py:136 xnbtd/tours/admin.py:171 xnbtd/tours/admin.py:207
-#: xnbtd/tours/admin.py:241
+#: xnbtd/tours/admin.py:157 xnbtd/tours/admin.py:207 xnbtd/tours/admin.py:258
+#: xnbtd/tours/admin.py:303 xnbtd/tours/admin.py:352
 msgid "Total Work Hours"
 msgstr "Total d’heures de travail"
 
-#: xnbtd/tours/admin.py:137 xnbtd/tours/admin.py:172 xnbtd/tours/admin.py:208
-#: xnbtd/tours/admin.py:242
+#: xnbtd/tours/admin.py:158 xnbtd/tours/admin.py:208 xnbtd/tours/admin.py:259
+#: xnbtd/tours/admin.py:304 xnbtd/tours/admin.py:353
 msgid "Total Break Hours"
 msgstr "Total d’heures de pause"
 
-#: xnbtd/tours/admin.py:138
+#: xnbtd/tours/admin.py:159
 msgid "Total Packages Delivered"
 msgstr "Total colis livrés"
 
-#: xnbtd/tours/admin.py:173
+#: xnbtd/tours/admin.py:209
 msgid "Total Clients"
 msgstr "Totals clients"
 
-#: xnbtd/tours/admin.py:209
+#: xnbtd/tours/admin.py:260
 msgid "Total of Points"
 msgstr "Total de points"
 
-#: xnbtd/tours/admin.py:243
+#: xnbtd/tours/admin.py:305
+msgid "Total of Picked Points"
+msgstr "Total de points ramassés"
+
+#: xnbtd/tours/admin.py:354
 msgid "Total Days"
 msgstr "Total de jours"
 
 #: xnbtd/tours/apps.py:8
 msgid "app_tours_name"
 msgstr "Tournées"
 
-#: xnbtd/tours/models.py:7 xnbtd/tours/models.py:45 xnbtd/tours/models.py:85
-#: xnbtd/tours/models.py:124
+#: xnbtd/tours/models.py:11
 msgid "Tour Name"
 msgstr "numéro de tournée"
 
-#: xnbtd/tours/models.py:8 xnbtd/tours/models.py:46 xnbtd/tours/models.py:86
-#: xnbtd/tours/models.py:135
+#: xnbtd/tours/models.py:12
 msgid "Tour Date"
 msgstr "date"
 
-#: xnbtd/tours/models.py:9
+#: xnbtd/tours/models.py:13
+msgid "Breaks"
+msgstr "pauses"
+
+#: xnbtd/tours/models.py:14
+msgid "Beginning Hour"
+msgstr "début de la journée"
+
+#: xnbtd/tours/models.py:15
+msgid "Ending Hour"
+msgstr "fin de la journée"
+
+#: xnbtd/tours/models.py:16
+msgid "Total Hour"
+msgstr "Durée de la journée"
+
+#: xnbtd/tours/models.py:41
 msgid "Points Charges"
 msgstr "Points chargés"
 
-#: xnbtd/tours/models.py:10
+#: xnbtd/tours/models.py:42
 msgid "Points Delivered"
 msgstr "Points livrés"
 
-#: xnbtd/tours/models.py:11
+#: xnbtd/tours/models.py:43
 msgid "Packages Charges"
 msgstr "Colis chargés"
 
-#: xnbtd/tours/models.py:12
+#: xnbtd/tours/models.py:44
 msgid "Packages Delivered"
 msgstr "Colis livrés"
 
-#: xnbtd/tours/models.py:13
+#: xnbtd/tours/models.py:45
 msgid "AVP Relay"
 msgstr "AVP Relais"
 
-#: xnbtd/tours/models.py:14
+#: xnbtd/tours/models.py:46
 msgid "SHD"
 msgstr "SHD"
 
-#: xnbtd/tours/models.py:15
+#: xnbtd/tours/models.py:47
 msgid "EO"
 msgstr "EO"
 
-#: xnbtd/tours/models.py:16
+#: xnbtd/tours/models.py:48
 msgid "Pickup Point"
 msgstr "Point de ramasse"
 
-#: xnbtd/tours/models.py:17 xnbtd/tours/models.py:57 xnbtd/tours/models.py:142
-msgid "Breaks"
-msgstr "pauses"
-
-#: xnbtd/tours/models.py:19 xnbtd/tours/models.py:59 xnbtd/tours/models.py:98
-#: xnbtd/tours/models.py:144
-msgid "Beginning Hour"
-msgstr "début de la tournée"
-
-#: xnbtd/tours/models.py:20 xnbtd/tours/models.py:60 xnbtd/tours/models.py:99
-#: xnbtd/tours/models.py:145
-msgid "Ending Hour"
-msgstr "fin de la tournée"
-
-#: xnbtd/tours/models.py:21 xnbtd/tours/models.py:61 xnbtd/tours/models.py:100
-#: xnbtd/tours/models.py:146
-msgid "Total Hour"
-msgstr "Durée de la tournée"
-
-#: xnbtd/tours/models.py:40 xnbtd/tours/models.py:41
+#: xnbtd/tours/models.py:51 xnbtd/tours/models.py:52
 msgid "GLS"
 msgstr "GLS"
 
-#: xnbtd/tours/models.py:47
+#: xnbtd/tours/models.py:56
 msgid "Charged Packages"
 msgstr "Colis chargé"
 
-#: xnbtd/tours/models.py:48
+#: xnbtd/tours/models.py:57
 msgid "Charged Points"
 msgstr "Points chargés"
 
-#: xnbtd/tours/models.py:49
+#: xnbtd/tours/models.py:58
 msgid "Including IP"
 msgstr "Dont IP"
 
-#: xnbtd/tours/models.py:50
+#: xnbtd/tours/models.py:59
 msgid "Relay"
 msgstr "Relais"
 
-#: xnbtd/tours/models.py:51
+#: xnbtd/tours/models.py:60
 msgid "Return Packages"
 msgstr "Retour COLIS"
 
-#: xnbtd/tours/models.py:52
+#: xnbtd/tours/models.py:61
 msgid "Return Points"
 msgstr "Retour POINTS"
 
-#: xnbtd/tours/models.py:53
+#: xnbtd/tours/models.py:62
 msgid "Overdue"
 msgstr "HORS DELAIS"
 
-#: xnbtd/tours/models.py:54
+#: xnbtd/tours/models.py:63
 msgid "Anomalies"
 msgstr "Anomalies"
 
-#: xnbtd/tours/models.py:55
+#: xnbtd/tours/models.py:64
 msgid "Total Points"
 msgstr "Total points"
 
-#: xnbtd/tours/models.py:56
+#: xnbtd/tours/models.py:65
 msgid "Full KM"
 msgstr "Plein / KM"
 
-#: xnbtd/tours/models.py:80 xnbtd/tours/models.py:81
-msgid "Chronopost"
-msgstr "Chronopost"
+#: xnbtd/tours/models.py:68 xnbtd/tours/models.py:69
+msgid "Chronopost Delivery"
+msgstr "Chronopost - Livraison"
+
+#: xnbtd/tours/models.py:73
+msgid "ESD"
+msgstr "ESD"
+
+#: xnbtd/tours/models.py:74
+msgid "Picked Points"
+msgstr "Point ramassés"
+
+#: xnbtd/tours/models.py:75
+msgid "Poste"
+msgstr "Poste"
+
+#: xnbtd/tours/models.py:78 xnbtd/tours/models.py:79
+msgid "Chronopost Pickup"
+msgstr "Chronopost - Ramasse"
 
-#: xnbtd/tours/models.py:87
+#: xnbtd/tours/models.py:83
 msgid "Client numbers"
 msgstr "Nombres clients"
 
-#: xnbtd/tours/models.py:88
+#: xnbtd/tours/models.py:84
 msgid "Refused"
 msgstr "refuse"
 
-#: xnbtd/tours/models.py:90
+#: xnbtd/tours/models.py:86
 msgid "cad/return"
 msgstr "cad/retour"
 
-#: xnbtd/tours/models.py:91
+#: xnbtd/tours/models.py:87
 msgid "totals clients"
 msgstr "totals client"
 
-#: xnbtd/tours/models.py:92
+#: xnbtd/tours/models.py:88
 msgid "occasional abductions"
 msgstr "enlèvements occasionnels"
 
-#: xnbtd/tours/models.py:93
+#: xnbtd/tours/models.py:89
 msgid "regular abductions"
 msgstr "enlèvements réguliers"
 
-#: xnbtd/tours/models.py:94
+#: xnbtd/tours/models.py:90
 msgid "total clients abductions"
 msgstr "totals clients enlèvements"
 
-#: xnbtd/tours/models.py:95
+#: xnbtd/tours/models.py:91
 msgid "KM/Full"
 msgstr "KM/Plein"
 
-#: xnbtd/tours/models.py:119 xnbtd/tours/models.py:120
-msgid "TNT - Fedex"
+#: xnbtd/tours/models.py:94 xnbtd/tours/models.py:95
+msgid "TNT"
 msgstr "TNT - Fedex"
 
-#: xnbtd/tours/models.py:139
+#: xnbtd/tours/models.py:103
 msgid "spare part"
 msgstr "spare part"
 
-#: xnbtd/tours/models.py:141
+#: xnbtd/tours/models.py:105
 msgid "morning pickups"
 msgstr "ramassages matin"
 
-#: xnbtd/tours/models.py:165 xnbtd/tours/models.py:166
+#: xnbtd/tours/models.py:108 xnbtd/tours/models.py:109
 msgid "Ciblex"
-msgstr "Ciblex"
+msgstr "Ciblex"
```

### Comparing `xnbtd-0.0.9/xnbtd/tours/migrations/0001_initial.py` & `xnbtd-1.0.0/xnbtd/tours/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `xnbtd-0.0.9/PKG-INFO` & `xnbtd-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xnbtd
-Version: 0.0.9
+Version: 1.0.0
 Summary: xNBTD est une application de gestion pour entreprise de livraison. Elle facilite la gestion des tournées et des plannings.
 Home-page: https://github.com/eldertek/xnbtd
 License: GPL-3.0-or-later
 Author: André Théo LAURET
 Author-email: andrelauret@eclipse-technology.eu
 Maintainer: André Théo LAURET
 Maintainer-email: andrelauret@eclipse-technology.eu
```

