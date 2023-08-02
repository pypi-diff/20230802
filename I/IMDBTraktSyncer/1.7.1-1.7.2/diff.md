# Comparing `tmp/IMDBTraktSyncer-1.7.1.tar.gz` & `tmp/IMDBTraktSyncer-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDBTraktSyncer-1.7.1.tar", last modified: Sat Jul 29 12:04:50 2023, max compression
+gzip compressed data, was "IMDBTraktSyncer-1.7.2.tar", last modified: Wed Aug  2 07:07:56 2023, max compression
```

## Comparing `IMDBTraktSyncer-1.7.1.tar` & `IMDBTraktSyncer-1.7.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 12:04:50.103719 IMDBTraktSyncer-1.7.1/
-drwxrwxrwx   0        0        0        0 2023-07-29 12:04:50.069297 IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/
--rw-rw-rw-   0        0        0    41112 2023-07-29 12:00:01.000000 IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/IMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     4624 2023-06-19 09:47:47.000000 IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     4317 2023-06-19 09:47:23.000000 IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     6946 2023-06-27 06:49:08.000000 IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     1669 2023-06-25 00:09:11.000000 IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/errorLogger.py
--rw-rw-rw-   0        0        0    11362 2023-07-29 10:06:33.000000 IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/imdbData.py
--rw-rw-rw-   0        0        0    10572 2023-07-29 08:41:16.000000 IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0    12192 2023-06-19 15:47:42.000000 IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-07-29 12:04:50.100708 IMDBTraktSyncer-1.7.1/IMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0    12719 2023-07-29 12:04:49.000000 IMDBTraktSyncer-1.7.1/IMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      549 2023-07-29 12:04:49.000000 IMDBTraktSyncer-1.7.1/IMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 12:04:49.000000 IMDBTraktSyncer-1.7.1/IMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-07-29 12:04:49.000000 IMDBTraktSyncer-1.7.1/IMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-07-29 12:04:49.000000 IMDBTraktSyncer-1.7.1/IMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-29 12:04:49.000000 IMDBTraktSyncer-1.7.1/IMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.7.1/LICENSE
--rw-rw-rw-   0        0        0    12719 2023-07-29 12:04:50.102708 IMDBTraktSyncer-1.7.1/PKG-INFO
--rw-rw-rw-   0        0        0    11972 2023-07-29 10:46:05.000000 IMDBTraktSyncer-1.7.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-29 12:04:50.103719 IMDBTraktSyncer-1.7.1/setup.cfg
--rw-rw-rw-   0        0        0     1377 2023-07-29 12:04:16.000000 IMDBTraktSyncer-1.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:07:56.036050 IMDBTraktSyncer-1.7.2/
+drwxrwxrwx   0        0        0        0 2023-08-02 07:07:56.003039 IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    41616 2023-08-02 07:06:39.000000 IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/IMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     4624 2023-07-31 01:18:20.000000 IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     4317 2023-07-31 01:18:20.000000 IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     6946 2023-08-02 06:46:34.000000 IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     1669 2023-07-31 01:18:20.000000 IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/errorLogger.py
+-rw-rw-rw-   0        0        0    11546 2023-08-02 05:50:14.000000 IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/imdbData.py
+-rw-rw-rw-   0        0        0    10572 2023-07-31 01:18:20.000000 IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0    12192 2023-07-31 01:18:20.000000 IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:07:56.033041 IMDBTraktSyncer-1.7.2/IMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0    12719 2023-08-02 07:07:55.000000 IMDBTraktSyncer-1.7.2/IMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      549 2023-08-02 07:07:55.000000 IMDBTraktSyncer-1.7.2/IMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 07:07:55.000000 IMDBTraktSyncer-1.7.2/IMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-08-02 07:07:55.000000 IMDBTraktSyncer-1.7.2/IMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-08-02 07:07:55.000000 IMDBTraktSyncer-1.7.2/IMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-08-02 07:07:55.000000 IMDBTraktSyncer-1.7.2/IMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.7.2/LICENSE
+-rw-rw-rw-   0        0        0    12719 2023-08-02 07:07:56.035040 IMDBTraktSyncer-1.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0    11972 2023-08-02 07:07:19.000000 IMDBTraktSyncer-1.7.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-02 07:07:56.036050 IMDBTraktSyncer-1.7.2/setup.cfg
+-rw-rw-rw-   0        0        0     1377 2023-08-02 07:00:53.000000 IMDBTraktSyncer-1.7.2/setup.py
```

### Comparing `IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/IMDBTraktSyncer.py` & `IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/IMDBTraktSyncer.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,21 +227,24 @@
                         })
                     elif media_type == 'episode':
                         data['episodes'].append({
                             "ids": {
                                 "imdb": imdb_id
                             }
                         })
+                    else:
+                        data = None
 
-                    response = EH.make_trakt_request(url, payload=data)
-                    
-                    if response is None:
-                        error_message = f"Failed to add item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) to Trakt Watchlist"
-                        print(f"   - {error_message}")
-                        EL.logger.error(error_message)
+                    if data:
+                        response = EH.make_trakt_request(url, payload=data)
+                        
+                        if response is None:
+                            error_message = f"Failed to add item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) to Trakt Watchlist"
+                            print(f"   - {error_message}")
+                            EL.logger.error(error_message)
 
                 print('Setting Trakt Watchlist Items Complete')
             else:
                 print('No Trakt Watchlist Items To Set')
 
             # Set IMDB Watchlist Items
             if imdb_watchlist_to_set:
@@ -360,22 +363,25 @@
                                 "ids": {
                                     "imdb": item["IMDB_ID"]
                                 },
                                 "rating": item["Rating"]
                             }]
                         }
                         print(f" - Rating episode ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt")
+                    else:
+                        data = None
+                    
+                    if data:
+                        # Make the API call to rate the item
+                        response = EH.make_trakt_request(rate_url, payload=data)
 
-                    # Make the API call to rate the item
-                    response = EH.make_trakt_request(rate_url, payload=data)
-
-                    if response is None:
-                        error_message = f"Failed rating {item['Type']} ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt"
-                        print(f"   - {error_message}")
-                        EL.logger.error(error_message)
+                        if response is None:
+                            error_message = f"Failed rating {item['Type']} ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt"
+                            print(f"   - {error_message}")
+                            EL.logger.error(error_message)
 
                 print('Setting Trakt Ratings Complete')
             else:
                 print('No Trakt Ratings To Set')
 
             # Set IMDB Ratings
             if imdb_ratings_to_set:
@@ -483,21 +489,24 @@
                             }
                         elif media_type == 'episode':
                             data['episode'] = {
                                 "ids": {
                                     "imdb": episode_id
                                 }
                             }
+                        else:
+                            data = None
                         
-                        response = EH.make_trakt_request(url, payload=data)
-                        
-                        if response is None:
-                            error_message = f"Failed to submit comment ({item_count} of {num_items}): {review['Title']} ({review['Year']}) on Trakt"
-                            print(f"   - {error_message}")
-                            EL.logger.error(error_message)
+                        if data:
+                            response = EH.make_trakt_request(url, payload=data)
+                            
+                            if response is None:
+                                error_message = f"Failed to submit comment ({item_count} of {num_items}): {review['Title']} ({review['Year']}) on Trakt"
+                                print(f"   - {error_message}")
+                                EL.logger.error(error_message)
 
                     print('Trakt Reviews Set Successfully')
                 else:
                     print('No Trakt Reviews To Set')
 
                 # Set IMDB Reviews
                 if imdb_reviews_to_set:
@@ -596,22 +605,25 @@
                             "episodes": [{
                                 "ids": {
                                     "trakt": item["TraktID"]
                                 }
                             }]
                         }
                         print(f" - Removing episode ({item_count} of {num_items}): {item['Title']} ({item['Year']}) from Trakt Watchlist")
+                    else:
+                        data = None
 
-                    # Make the API call to remove the item from the watchlist
-                    response = EH.make_trakt_request(remove_url, payload=data)
+                    if data:
+                        # Make the API call to remove the item from the watchlist
+                        response = EH.make_trakt_request(remove_url, payload=data)
 
-                    if response is None:
-                        error_message = f"Failed removing {item['Type']} ({item_count} of {num_items}): {item['Title']} ({item['Year']}) from Trakt Watchlist"
-                        print(f"   - {error_message}")
-                        EL.logger.error(error_message)
+                        if response is None:
+                            error_message = f"Failed removing {item['Type']} ({item_count} of {num_items}): {item['Title']} ({item['Year']}) from Trakt Watchlist"
+                            print(f"   - {error_message}")
+                            EL.logger.error(error_message)
 
                 print('Removing Watched Items From Trakt Watchlist Complete')
             else:
                 print('No Watched Items To Remove From Trakt Watchlist')
 
             # Remove Watched Items IMDB Watchlist
             if imdb_watchlist_items_to_remove:
```

### Comparing `IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/authTrakt.py` & `IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/checkChromedriver.py` & `IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/checkChromedriver.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/errorHandling.py` & `IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/errorHandling.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,24 +28,24 @@
     print("Please submit the error to GitHub with the following information:")
     print("-" * 50)
     print(traceback_info)
     print("-" * 50)
     print(f"Submit the error here: {github_issue_url}")
     print("-" * 50)
 
-def make_trakt_request(url, headers=None, params=None, payload=None, max_retries=3):
+def make_trakt_request(url, headers=None, params=None, payload=None, max_retries=5):
     if headers is None:
         headers = {
             'Content-Type': 'application/json',
             'trakt-api-version': '2',
             'trakt-api-key': VC.trakt_client_id,
             'Authorization': f'Bearer {VC.trakt_access_token}'
         }
 
-    retry_delay = 5  # seconds between retries
+    retry_delay = 1  # seconds between retries
     retry_attempts = 0
 
     while retry_attempts < max_retries:
         response = None
         try:
             if payload is None:
                 if params:
```

### Comparing `IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/errorLogger.py` & `IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/errorLogger.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/imdbData.py` & `IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/imdbData.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,15 +57,15 @@
                     date_added = row[2]
                     # Convert date format
                     date_added = datetime.strptime(date_added, '%Y-%m-%d').strftime('%Y-%m-%dT%H:%M:%S.000Z')
                     if "tvSeries" in row[7] or "tvMiniSeries" in row[7]:
                         media_type = "show"
                     elif "tvEpisode" in row[7]:
                         media_type = "episode"
-                    elif "movie" in row[7]:
+                    elif "movie" in row[7] or "tvSpecial" in row[7] or "tvMovie" in row[7] or "tvShort" in row[7] or "video" in row[7]:
                         media_type = "movie"
                     else:
                         media_type = "unknown"
                     imdb_watchlist.append({'Title': title, 'Year': year, 'IMDB_ID': imdb_id, 'Date_Added': date_added, 'Type': media_type})
         except FileNotFoundError:
             error_message = "Ratings file not found"
             print(f"{error_message}")
@@ -115,15 +115,15 @@
                     date_added = row[2]
                     # Convert date format
                     date_added = datetime.strptime(date_added, '%Y-%m-%d').strftime('%Y-%m-%dT%H:%M:%S.000Z')
                     if "tvSeries" in row[5] or "tvMiniSeries" in row[5]:
                         media_type = "show"
                     elif "tvEpisode" in row[5]:
                         media_type = "episode"
-                    elif "movie" in row[5]:
+                    elif "movie" in row[5] or "tvSpecial" in row[5] or "tvMovie" in row[5] or "tvShort" in row[5] or "video" in row[5]:
                         media_type = "movie"
                     else:
                         media_type = "unknown"
                     imdb_ratings.append({'Title': title, 'Year': year, 'Rating': int(rating), 'IMDB_ID': imdb_id, 'Date_Added': date_added, 'Type': media_type})
         except FileNotFoundError:
             print('Ratings file not found')
```

### Comparing `IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/traktData.py` & `IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/traktData.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.7.1/IMDBTraktSyncer/verifyCredentials.py` & `IMDBTraktSyncer-1.7.2/IMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.7.1/IMDBTraktSyncer.egg-info/PKG-INFO` & `IMDBTraktSyncer-1.7.2/IMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.7.1
+Version: 1.7.2
 Summary: A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
```

### Comparing `IMDBTraktSyncer-1.7.1/IMDBTraktSyncer.egg-info/SOURCES.txt` & `IMDBTraktSyncer-1.7.2/IMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.7.1/LICENSE` & `IMDBTraktSyncer-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.7.1/PKG-INFO` & `IMDBTraktSyncer-1.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.7.1
+Version: 1.7.2
 Summary: A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
```

### Comparing `IMDBTraktSyncer-1.7.1/README.md` & `IMDBTraktSyncer-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.7.1/setup.py` & `IMDBTraktSyncer-1.7.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), 'r', encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.7.1'
+VERSION = '1.7.2'
 DESCRIPTION = 'A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.'
 
 # Setting up
 setup(
     name="IMDBTraktSyncer",
     version=VERSION,
     author="RileyXX",
```

