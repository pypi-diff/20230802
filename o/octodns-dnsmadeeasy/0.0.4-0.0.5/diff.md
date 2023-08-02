# Comparing `tmp/octodns-dnsmadeeasy-0.0.4.tar.gz` & `tmp/octodns-dnsmadeeasy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octodns-dnsmadeeasy-0.0.4.tar", last modified: Mon Jul  3 17:10:45 2023, max compression
+gzip compressed data, was "octodns-dnsmadeeasy-0.0.5.tar", last modified: Wed Aug  2 17:18:27 2023, max compression
```

## Comparing `octodns-dnsmadeeasy-0.0.4.tar` & `octodns-dnsmadeeasy-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 yzguy      (501) staff       (20)        0 2023-07-03 17:10:45.333033 octodns-dnsmadeeasy-0.0.4/
--rw-r--r--   0 yzguy      (501) staff       (20)     2331 2023-07-03 17:10:45.332912 octodns-dnsmadeeasy-0.0.4/PKG-INFO
--rw-r--r--   0 yzguy      (501) staff       (20)     1992 2023-07-03 17:05:24.000000 octodns-dnsmadeeasy-0.0.4/README.md
-drwxr-xr-x   0 yzguy      (501) staff       (20)        0 2023-07-03 17:10:45.331988 octodns-dnsmadeeasy-0.0.4/octodns_dnsmadeeasy/
--rw-r--r--   0 yzguy      (501) staff       (20)    15380 2023-07-03 17:10:07.000000 octodns-dnsmadeeasy-0.0.4/octodns_dnsmadeeasy/__init__.py
-drwxr-xr-x   0 yzguy      (501) staff       (20)        0 2023-07-03 17:10:45.332541 octodns-dnsmadeeasy-0.0.4/octodns_dnsmadeeasy.egg-info/
--rw-r--r--   0 yzguy      (501) staff       (20)     2331 2023-07-03 17:10:45.000000 octodns-dnsmadeeasy-0.0.4/octodns_dnsmadeeasy.egg-info/PKG-INFO
--rw-r--r--   0 yzguy      (501) staff       (20)      322 2023-07-03 17:10:45.000000 octodns-dnsmadeeasy-0.0.4/octodns_dnsmadeeasy.egg-info/SOURCES.txt
--rw-r--r--   0 yzguy      (501) staff       (20)        1 2023-07-03 17:10:45.000000 octodns-dnsmadeeasy-0.0.4/octodns_dnsmadeeasy.egg-info/dependency_links.txt
--rw-r--r--   0 yzguy      (501) staff       (20)      246 2023-07-03 17:10:45.000000 octodns-dnsmadeeasy-0.0.4/octodns_dnsmadeeasy.egg-info/requires.txt
--rw-r--r--   0 yzguy      (501) staff       (20)       20 2023-07-03 17:10:45.000000 octodns-dnsmadeeasy-0.0.4/octodns_dnsmadeeasy.egg-info/top_level.txt
--rw-r--r--   0 yzguy      (501) staff       (20)      312 2023-06-22 18:01:26.000000 octodns-dnsmadeeasy-0.0.4/pyproject.toml
--rw-r--r--   0 yzguy      (501) staff       (20)       38 2023-07-03 17:10:45.333068 octodns-dnsmadeeasy-0.0.4/setup.cfg
--rw-r--r--   0 yzguy      (501) staff       (20)     2090 2023-07-03 17:05:24.000000 octodns-dnsmadeeasy-0.0.4/setup.py
-drwxr-xr-x   0 yzguy      (501) staff       (20)        0 2023-07-03 17:10:45.332660 octodns-dnsmadeeasy-0.0.4/tests/
--rw-r--r--   0 yzguy      (501) staff       (20)    22023 2023-07-03 17:05:24.000000 octodns-dnsmadeeasy-0.0.4/tests/test_octodns_provider_dnsmadeeasy.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-02 17:18:27.694449 octodns-dnsmadeeasy-0.0.5/
+-rw-r--r--   0 ross       (501) staff       (20)     2330 2023-08-02 17:18:27.694060 octodns-dnsmadeeasy-0.0.5/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)     1991 2023-08-02 17:17:58.000000 octodns-dnsmadeeasy-0.0.5/README.md
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-02 17:18:27.691029 octodns-dnsmadeeasy-0.0.5/octodns_dnsmadeeasy/
+-rw-r--r--   0 ross       (501) staff       (20)    16008 2023-08-02 17:17:58.000000 octodns-dnsmadeeasy-0.0.5/octodns_dnsmadeeasy/__init__.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-02 17:18:27.693107 octodns-dnsmadeeasy-0.0.5/octodns_dnsmadeeasy.egg-info/
+-rw-r--r--   0 ross       (501) staff       (20)     2330 2023-08-02 17:18:27.000000 octodns-dnsmadeeasy-0.0.5/octodns_dnsmadeeasy.egg-info/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)      322 2023-08-02 17:18:27.000000 octodns-dnsmadeeasy-0.0.5/octodns_dnsmadeeasy.egg-info/SOURCES.txt
+-rw-r--r--   0 ross       (501) staff       (20)        1 2023-08-02 17:18:27.000000 octodns-dnsmadeeasy-0.0.5/octodns_dnsmadeeasy.egg-info/dependency_links.txt
+-rw-r--r--   0 ross       (501) staff       (20)      246 2023-08-02 17:18:27.000000 octodns-dnsmadeeasy-0.0.5/octodns_dnsmadeeasy.egg-info/requires.txt
+-rw-r--r--   0 ross       (501) staff       (20)       20 2023-08-02 17:18:27.000000 octodns-dnsmadeeasy-0.0.5/octodns_dnsmadeeasy.egg-info/top_level.txt
+-rw-r--r--   0 ross       (501) staff       (20)      312 2023-02-04 19:18:43.000000 octodns-dnsmadeeasy-0.0.5/pyproject.toml
+-rw-r--r--   0 ross       (501) staff       (20)       38 2023-08-02 17:18:27.694591 octodns-dnsmadeeasy-0.0.5/setup.cfg
+-rw-r--r--   0 ross       (501) staff       (20)     2090 2023-06-28 23:41:28.000000 octodns-dnsmadeeasy-0.0.5/setup.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-02 17:18:27.693601 octodns-dnsmadeeasy-0.0.5/tests/
+-rw-r--r--   0 ross       (501) staff       (20)    23542 2023-08-02 17:17:58.000000 octodns-dnsmadeeasy-0.0.5/tests/test_octodns_provider_dnsmadeeasy.py
```

### Comparing `octodns-dnsmadeeasy-0.0.4/PKG-INFO` & `octodns-dnsmadeeasy-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octodns-dnsmadeeasy
-Version: 0.0.4
+Version: 0.0.5
 Summary:  DNS Made Easy provider for octoDNS
 Home-page: https://github.com/octodns/octodns-dnsmadeeasy
 Author: Ross McFarland
 Author-email: rwmcfa1@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -27,16 +27,16 @@
 
 Pinning specific versions or SHAs is recommended to avoid unplanned upgrades.
 
 ##### Versions
 
 ```
 # Start with the latest versions and don't just copy what's here
-octodns==0.9.14
-octodns-dnsmadeeasy==0.0.1
+octodns==1.0.0
+octodns-dnsmadeeasy==0.0.4
 ```
 
 ##### SHAs
 
 ```
 # Start with the latest/specific versions and don't just copy what's here
 -e git+https://git@github.com/octodns/octodns.git@9da19749e28f68407a1c246dfdf65663cdc1c422#egg=octodns
```

### Comparing `octodns-dnsmadeeasy-0.0.4/README.md` & `octodns-dnsmadeeasy-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
 Pinning specific versions or SHAs is recommended to avoid unplanned upgrades.
 
 ##### Versions
 
 ```
 # Start with the latest versions and don't just copy what's here
-octodns==0.9.14
-octodns-dnsmadeeasy==0.0.1
+octodns==1.0.0
+octodns-dnsmadeeasy==0.0.4
 ```
 
 ##### SHAs
 
 ```
 # Start with the latest/specific versions and don't just copy what's here
 -e git+https://git@github.com/octodns/octodns.git@9da19749e28f68407a1c246dfdf65663cdc1c422#egg=octodns
```

### Comparing `octodns-dnsmadeeasy-0.0.4/octodns_dnsmadeeasy/__init__.py` & `octodns-dnsmadeeasy-0.0.5/octodns_dnsmadeeasy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 #
 #
 #
 
 import hashlib
 import hmac
 import logging
+import re
 from collections import defaultdict
 from time import gmtime, sleep, strftime
 
 from requests import Session
 
 from octodns import __VERSION__ as octodns_version
 from octodns.provider import ProviderException
 from octodns.provider.base import BaseProvider
 from octodns.record import Record
 
-__VERSION__ = '0.0.4'
+__VERSION__ = '0.0.5'
 
 
 class DnsMadeEasyClientException(ProviderException):
     pass
 
 
 class DnsMadeEasyClientBadRequest(DnsMadeEasyClientException):
@@ -182,14 +183,20 @@
             'NS',
             'PTR',
             'SPF',
             'SRV',
             'TXT',
         )
     )
+    # Regex to replace any pair of double quotes that aren't escaped with a backslash. Used as a delimiter in long TXT
+    # records.
+    #
+    #  Will match: Alpha""Bravo
+    #  Will not match: Alpha\""Bravo
+    TXT_RECORD_VALUE_DELIMITER_PATTERN = re.compile(r'(?<!\\)\"\"')
 
     def __init__(
         self,
         id,
         api_key,
         secret_key,
         sandbox=False,
@@ -232,15 +239,21 @@
                     'tag': record['caaType'],
                     'value': record['value'][1:-1],
                 }
             )
         return {'ttl': records[0]['ttl'], 'type': _type, 'values': values}
 
     def _data_for_TXT(self, _type, records):
-        values = [value['value'].replace(';', '\\;') for value in records]
+        # Long TXT records in DNS Mady Easy have their value split into 255 character chunks, delimited by "".
+        values = [
+            self.TXT_RECORD_VALUE_DELIMITER_PATTERN.sub(
+                '', value['value'].replace(';', '\\;')
+            )
+            for value in records
+        ]
         return {'ttl': records[0]['ttl'], 'type': _type, 'values': values}
 
     _data_for_SPF = _data_for_TXT
 
     def _data_for_MX(self, _type, records):
         values = []
         for record in records:
@@ -388,18 +401,20 @@
                 'priority': value.priority,
                 'ttl': record.ttl,
                 'type': record._type,
                 'weight': value.weight,
             }
 
     def _params_for_TXT(self, record):
+        # DNSMadeEasy doesn't need chunking, it accepts the record and will chunk it itself
         # DNSMadeEasy does not want values escaped
-        for value in record.chunked_values:
+        for value in record.values:
+            value = value.replace('\\;', ';')
             yield {
-                'value': value.replace('\\;', ';'),
+                'value': f'"{value}"',
                 'name': record.name,
                 'ttl': record.ttl,
                 'type': record._type,
             }
 
     _params_for_SPF = _params_for_TXT
```

### Comparing `octodns-dnsmadeeasy-0.0.4/octodns_dnsmadeeasy.egg-info/PKG-INFO` & `octodns-dnsmadeeasy-0.0.5/octodns_dnsmadeeasy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octodns-dnsmadeeasy
-Version: 0.0.4
+Version: 0.0.5
 Summary:  DNS Made Easy provider for octoDNS
 Home-page: https://github.com/octodns/octodns-dnsmadeeasy
 Author: Ross McFarland
 Author-email: rwmcfa1@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -27,16 +27,16 @@
 
 Pinning specific versions or SHAs is recommended to avoid unplanned upgrades.
 
 ##### Versions
 
 ```
 # Start with the latest versions and don't just copy what's here
-octodns==0.9.14
-octodns-dnsmadeeasy==0.0.1
+octodns==1.0.0
+octodns-dnsmadeeasy==0.0.4
 ```
 
 ##### SHAs
 
 ```
 # Start with the latest/specific versions and don't just copy what's here
 -e git+https://git@github.com/octodns/octodns.git@9da19749e28f68407a1c246dfdf65663cdc1c422#egg=octodns
```

### Comparing `octodns-dnsmadeeasy-0.0.4/setup.py` & `octodns-dnsmadeeasy-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `octodns-dnsmadeeasy-0.0.4/tests/test_octodns_provider_dnsmadeeasy.py` & `octodns-dnsmadeeasy-0.0.5/tests/test_octodns_provider_dnsmadeeasy.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,22 +99,22 @@
             with open('tests/fixtures/dnsmadeeasy-domains.json') as fh:
                 mock.get(f'{base}/', text=fh.read())
             with open('tests/fixtures/dnsmadeeasy-records.json') as fh:
                 mock.get(f'{base}/123123/records', text=fh.read())
 
                 zone = Zone('unit.tests.', [])
                 provider.populate(zone)
-                self.assertEqual(14, len(zone.records))
+                self.assertEqual(16, len(zone.records))
                 changes = self.expected.changes(zone, provider)
                 self.assertEqual(0, len(changes))
 
         # 2nd populate makes no network calls/all from cache
         again = Zone('unit.tests.', [])
         provider.populate(again)
-        self.assertEqual(14, len(again.records))
+        self.assertEqual(16, len(again.records))
 
         # bust the cache
         del provider._zone_records[zone.name]
 
     def test_populate_empty(self):
         provider = DnsMadeEasyProvider('test', 'api', 'secret')
 
@@ -280,21 +280,35 @@
                             'value': 'foo.bar.com.',
                             'name': 'ptr',
                             'ttl': 300,
                             'type': 'PTR',
                             'gtdLocation': 'DEFAULT',
                         },
                         {
+                            'value': '"This is a TXT record with \\"quotes\\" in it to ensure they are handled correctly"',
+                            'name': 'quotes',
+                            'ttl': 600,
+                            'type': 'TXT',
+                            'gtdLocation': 'DEFAULT',
+                        },
+                        {
                             'value': '"v=spf1 ip4:192.168.0.1/16-all"',
                             'name': 'spf',
                             'ttl': 600,
                             'type': 'SPF',
                             'gtdLocation': 'DEFAULT',
                         },
                         {
+                            'value': '"Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc porttitor, odio eleifend ullamcorper ultricies, lectus lorem iaculis erat, ut porttitor erat orci eget est. Nunc tortor odio, suscipit non maximus in, euismod nec dolor. Nullam quis ultricies orci. Donec malesuada tempor accumsan. Vivamus erat eros, condimentum et urna vitae, aliquam congue quam. Phasellus nibh mauris, congue quis euismod vel, porta sed dui. Fusce massa dui, feugiat dapibus condimentum nec, vulputate eget ex. Sed vitae augue et ex facilisis placerat id sit amet tortor. Morbi pellentesque velit arcu, ut suscipit quam consectetur in. Quisque pulvinar ante sit amet egestas gravida. Etiam accumsan urna et suscipit pulvinar. Fusce ultricies congue sapien non semper. Morbi eleifend molestie blandit. Suspendisse potenti. Fusce vestibulum commodo leo. Nulla cursus turpis sit amet tincidunt bibendum."',
+                            'name': 'split',
+                            'ttl': 600,
+                            'type': 'TXT',
+                            'gtdLocation': 'DEFAULT',
+                        },
+                        {
                             'value': '"Bah bah black sheep"',
                             'name': 'txt',
                             'ttl': 600,
                             'type': 'TXT',
                             'gtdLocation': 'DEFAULT',
                         },
                         {
```

