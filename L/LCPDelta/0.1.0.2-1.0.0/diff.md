# Comparing `tmp/LCPDelta-0.1.0.2.tar.gz` & `tmp/LCPDelta-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LCPDelta-0.1.0.2.tar", last modified: Wed Jul 26 14:00:34 2023, max compression
+gzip compressed data, was "LCPDelta-1.0.0.tar", last modified: Wed Aug  2 11:05:08 2023, max compression
```

## Comparing `LCPDelta-0.1.0.2.tar` & `LCPDelta-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 14:00:34.651956 LCPDelta-0.1.0.2/
--rw-rw-rw-   0        0        0     1091 2023-06-16 15:59:44.000000 LCPDelta-0.1.0.2/LICENSE
--rw-rw-rw-   0        0        0      563 2023-07-26 14:00:34.650955 LCPDelta-0.1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       85 2023-06-16 15:59:46.000000 LCPDelta-0.1.0.2/README.md
--rw-rw-rw-   0        0        0      632 2023-07-26 14:00:10.000000 LCPDelta-0.1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-26 14:00:34.651956 LCPDelta-0.1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-26 14:00:34.578435 LCPDelta-0.1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-26 14:00:34.618969 LCPDelta-0.1.0.2/src/LCPDelta/
--rw-rw-rw-   0        0        0    34999 2023-07-26 11:08:30.000000 LCPDelta-0.1.0.2/src/LCPDelta/Enact.py
--rw-rw-rw-   0        0        0        0 2023-06-20 13:20:32.000000 LCPDelta-0.1.0.2/src/LCPDelta/FlexTrack.py
--rw-rw-rw-   0        0        0      314 2023-07-25 16:29:17.000000 LCPDelta-0.1.0.2/src/LCPDelta/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 14:00:34.648955 LCPDelta-0.1.0.2/src/LCPDelta.egg-info/
--rw-rw-rw-   0        0        0      563 2023-07-26 14:00:34.000000 LCPDelta-0.1.0.2/src/LCPDelta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-07-26 14:00:34.000000 LCPDelta-0.1.0.2/src/LCPDelta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 14:00:34.000000 LCPDelta-0.1.0.2/src/LCPDelta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-07-26 14:00:34.000000 LCPDelta-0.1.0.2/src/LCPDelta.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-26 14:00:34.000000 LCPDelta-0.1.0.2/src/LCPDelta.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 11:05:08.151450 LCPDelta-1.0.0/
+-rw-rw-rw-   0        0        0     1091 2023-06-16 15:59:44.000000 LCPDelta-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     2055 2023-08-02 11:05:08.149504 LCPDelta-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1566 2023-08-02 10:56:22.000000 LCPDelta-1.0.0/README.md
+-rw-rw-rw-   0        0        0      646 2023-08-02 11:04:43.000000 LCPDelta-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-02 11:05:08.152452 LCPDelta-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-02 11:05:08.026455 LCPDelta-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-08-02 11:05:08.053459 LCPDelta-1.0.0/src/LCPDelta/
+drwxrwxrwx   0        0        0        0 2023-08-02 11:05:08.146511 LCPDelta-1.0.0/src/LCPDelta/Enact/
+-rw-rw-rw-   0        0        0    29435 2023-08-02 10:47:49.000000 LCPDelta-1.0.0/src/LCPDelta/Enact/APIHelper.py
+-rw-rw-rw-   0        0        0     3688 2023-08-02 10:13:35.000000 LCPDelta-1.0.0/src/LCPDelta/Enact/CredentialsHolder.py
+-rw-rw-rw-   0        0        0     4019 2023-08-02 10:47:38.000000 LCPDelta-1.0.0/src/LCPDelta/Enact/DPSHelper.py
+-rw-rw-rw-   0        0        0      118 2023-08-02 10:21:02.000000 LCPDelta-1.0.0/src/LCPDelta/Enact/__init__.py
+-rw-rw-rw-   0        0        0      275 2023-08-02 10:27:03.000000 LCPDelta-1.0.0/src/LCPDelta/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 11:05:08.091458 LCPDelta-1.0.0/src/LCPDelta.egg-info/
+-rw-rw-rw-   0        0        0     2055 2023-08-02 11:05:08.000000 LCPDelta-1.0.0/src/LCPDelta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-08-02 11:05:08.000000 LCPDelta-1.0.0/src/LCPDelta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 11:05:08.000000 LCPDelta-1.0.0/src/LCPDelta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-08-02 11:05:08.000000 LCPDelta-1.0.0/src/LCPDelta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-02 11:05:08.000000 LCPDelta-1.0.0/src/LCPDelta.egg-info/top_level.txt
```

### Comparing `LCPDelta-0.1.0.2/LICENSE` & `LCPDelta-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `LCPDelta-0.1.0.2/pyproject.toml` & `LCPDelta-1.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "LCPDelta"
-version = "0.1.0.2"
+version = "1.0.0"
 authors = [
   { name="Sushanth Kolluru", email="enact.helpdesk@lcp.uk.com" },
 ]
-description = "LCPDelta test package"
+description = "LCPDelta Python Package"
 readme = "README.md"
 requires-python = ">=3.7"
-keywords = ["LCPDelta", "Enact", "Flextrack"]
+keywords = ["LCPDelta", "Enact", "Flextrack", "Storetrack"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "requests",
```

### Comparing `LCPDelta-0.1.0.2/src/LCPDelta/Enact.py` & `LCPDelta-1.0.0/src/LCPDelta/Enact/APIHelper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,112 +1,17 @@
 from LCPDelta import requests
 from LCPDelta import json
 from LCPDelta import date, datetime, time 
-from LCPDelta import HubConnectionBuilder
-from LCPDelta import threading
-from LCPDelta import pytime
-from LCPDelta import partial
 from LCPDelta import calendar
-
-class CredentialsHolder:
-    
-    MAX_RETRIES = 3
-    
-    def __init__(self, username, public_api_key):
-        self.username = username
-        self.public_api_key = public_api_key
-        self.bearer_token = self.get_bearer_token(username, public_api_key)
-        
-    def get_bearer_token(self, enact_username, public_api_key):
-        
-        """Get the bearer token for authentication.
-
-        This method sends a request to obtain a bearer token for authentication
-        using the Enact API. It takes an Enact username and public API key as 
-        input parameters.
-
-        Args:
-            enact_username (str): The username for Enact authentication.
-            public_api_key (str): The public API key for Enact authentication.
-
-        Returns:
-            str: The bearer token obtained from the Enact API.
-        """
-        
-        headers = {'Content-Type': 'application/json', 'cache-control': 'no-cache'}
-        data = {
-            "Username": enact_username,
-            "ApiKey": public_api_key
-        }
-        response = requests.post('https://enactapifd.lcp.uk.com/auth/token', headers=headers, data=json.dumps(data))
-        
-        if response.status_code == 401 or response.status_code == 500:
-            response = self.retry_request(headers, data)
-        
-        bearer_token = response.text
-        return bearer_token
-    
-    def retry_request(self, headers, data):
-        """Retry the request to obtain a valid bearer token.
-
-        This method retries the request to obtain a valid bearer token for
-        authentication. It takes the request headers and data as input parameters.
-
-        Args:
-            headers (dict): The headers for the request.
-            data (dict): The data to be sent with the request.
-
-        Raises:
-            Exception: If a valid bearer token cannot be obtained after
-                    multiple attempts.
-
-        Returns:
-            Response: The response object containing the bearer token.
-        """
-        retry_count = 0
-        while retry_count < self.MAX_RETRIES:
-            response = requests.post('https://enactapifd.lcp.uk.com/auth/token', headers=headers, data=json.dumps(data))
-            if response.status_code != 401 and response.status_code != 500:
-                    # Successful response, no need to retry
-                break   
-            retry_count += 1
-                
-        if retry_count == self.MAX_RETRIES:
-            raise Exception("Failed to obtain a valid bearer token after multiple attempts.")
-        
-        return response
-    
-    def get_remaining_token_count(self):
-        """Get the remaining token count for API calls.
-
-        This method sends a request to obtain the remaining token count
-        for API calls. It retrieves the count based on the Enact username
-        and public API key associated with the instance.
-
-        Returns:
-            str: The remaining token count for API calls.
-        """
-        headers = {'Content-Type': 'application/json', 'cache-control': 'no-cache'}
-        data = {
-            "Username": self.enact_username,
-            "ApiKey": self.public_api_key
-        }
-        response = requests.post('https://enactapifd.lcp.uk.com/auth/usage', headers=headers, data=json.dumps(data))
-        
-        if response.status_code == 401 or response.status_code == 500:
-            response = self.retry_request(headers, data)
-            
-        remaining_calls = response.text    
-        print(f"You have {remaining_calls} API calls remaining") 
-        return remaining_calls
-        
+from .CredentialsHolder import CredentialsHolder 
+      
 class APIHelper:
     
     def __init__(self, username, public_api_key, timezone_id =  "UTC"): 
-        """Your one-stop shop for all API calls on Enact. Enter your credentials and use the methods below to get data from Enact.
+        """ Enter your credentials and use the methods below to get data from Enact.
 
         Args:
             username (str): Enact Username. Please contact the Enact team if you are unsure about what your username or public api key are.
             public_api_key (str): Public API Key provided by Enact. Please contact the Enact team if you are unsure about what your username or public api key are.
             timezone_id (str, optional): Choose what timezone you want data to be returned in. Find the timezone string options on the Enact Query Builder page. Defaults to "GMT Standard Time".
         """
         self.enact_credentials = CredentialsHolder(username, public_api_key)
@@ -122,29 +27,41 @@
         return converted_date
     
     def post_request(self, endpoint, request_details):
         headers = {'Authorization': 'Bearer ' + self.enact_credentials.bearer_token, 
                    'Content-Type': 'application/json',
                    'cache-control': 'no-cache'}
         
-        response = requests.post(endpoint, data=json.dumps(request_details), headers = headers)
+        response_raw = requests.post(endpoint, data=json.dumps(request_details), headers = headers)
         
-        if response.status_code != 200:
-            response = self.handle_error_and_get_response(endpoint, request_details, headers, response)
+        if response_raw.status_code != 200:
+            response_raw = self.handle_error_and_get_response(endpoint, request_details, headers, response)
+            
+        response = json.loads(response_raw.text)
+        
+        if 'Messages' in response:
+            self.raise_exception_for_enact_error(response)
         return response
 
     def handle_error_and_get_updated_response(self, endpoint, request_details, headers, response):
         # check if bearer token has expired and if it has create a new one
         if response.status_code == 401 and 'WWW-Authenticate' in response.headers:
             response = self.handle_authorisation_error(endpoint, request_details, headers)
             
         if response.status_code == 400:
             banana = 1; 
         return response
 
+    def raise_exception_for_enact_error(self, response):
+        error_messages = response['Messages']
+        for error_message in error_messages:
+            if 'ErrorCode' in error_message and error_message['ErrorCode']:
+                # An error code is present, so raise an exception with the error message
+                raise Exception(f"ErrorCode: {error_message['ErrorCode']}. {error_message['Message']}")
+        
     def handle_authorisation_error(self, endpoint, request_details, headers):
         retry_count = 0
         while retry_count < self.enact_credentials.MAX_RETRIES:
             self.enact_credentials.get_bearer_token(self.enact_credentials.username, self.enact_credentials.public_api_key)
             headers['Authorization'] = 'Bearer ' + self.enact_credentials.bearer_token
 
                 # Retry the POST request with the new bearer token
@@ -160,16 +77,15 @@
             raise Exception("Failed to obtain a valid bearer token after multiple attempts.")
         return response
     
     # Series:
     def get_series_data(self, series_id, date_from = date.today(), date_to = date.today(), option_id = None, half_hourly_average = False, country_id = "Gb"):
         """Get series data for a specific series ID.
 
-        This method retrieves the series data for a specific series ID from the Enact API.
-        It allows specifying the date range, option ID, half-hourly average, and country ID.
+        This method retrieves the series data for a specific series ID from the Enact API. It allows specifying the date range, option ID, half-hourly average, and country ID.
 
         Args:
             series_id (str): This is the Enact ID for the requested series, as defined in the query generator on the 'General' tab.
             date_from (datetime.date, optional): This is the start of the date-range being requested. Defaults to today's date.
             date_to (datetime.date, optional): This is the end of the date-range being requested. If a single day is wanted, then this will be the same as the From value. 
                                                Defaults to today's date.
             option_id (str, optional): If the selected Series has options, then this is the Enact ID for the requested Option, as defined in the query generator on the 'General' tab.
@@ -201,17 +117,16 @@
         response = self.post_request(endpoint, request_details)
         
         return response
     
     def get_series_info(self, series_id, country_id = None):
         """Get information about a specific series.
 
-        This method retrieves information about a specific series based on the given series ID.
-        Optional country ID can be provided to filter the series information.
-
+        This method retrieves information about a specific series based on the given series ID. Optional country ID can be provided to filter the series information.
+        
         Args:
             series_id (str): This is the Enact ID for the requested series, as defined in the query generator on the 'General' tab.
             country_id (str, optional): The country ID to filter the series information. Defaults to None. If this is not provided, then details will be displayed for the first country available for this series.
         """
         endpoint = 'https://enactapifd.lcp.uk.com/EnactAPI/Series/Info'
         request_details = {
             "SeriesId": series_id
@@ -365,15 +280,15 @@
     def get_bm_data_by_search(self, date, option = "all", search_string = None, includeAcceptedTimes = False):
         """Get BM data based for a specific date and search criteria.
 
         Args:
             date (datetime.date): The date for which to retrieve the BM data.
             option (str): This allows you to select whether you want to search for BOA data for plants, fuels or just return everything. Can be set to "plant", "fuel", "all"
             search_string (str): The search string to match against the BM data. If Option is "plant", this allows you to search for all BOA actions from plants with BMU ID containing "CARR" (e.g. all Carrington units).
-                                  If option is "fuel", this allows you to search for all BOA actions from plants with fuel type "Coal". If Option is "all", this must not be sent to work.        
+                                If option is "fuel", this allows you to search for all BOA actions from plants with fuel type "Coal". If Option is "all", this must not be sent to work.        
             includeAcceptedTimes (bool): Determine whether the returned object includes a column for accepted times in the response object
         Returns:
             Response: The response object containing the BM data.
         """
         endpoint = 'https://enactapifd.lcp.uk.com/EnactAPI/BOA/Data'
         
         date = self.convert_date_time_to_right_format(date)
@@ -683,65 +598,8 @@
         date = self.convert_date_time_to_right_format(date)
         
         request_details = {
             "Date" : date,
         }
         
         response = self.post_request(endpoint, request_details)
-        return response
-
-class DPSHelper:
-    def __init__(self, username, public_api_key): 
-        self.enact_credentials = CredentialsHolder(username, public_api_key)
-        access_token_factory = partial(self.fetch_bearer_token)
-        self.hub_connection = HubConnectionBuilder().with_url("https://enact-signalrhub.azurewebsites.net/dataHub",
-            options={
-                "access_token_factory" : access_token_factory
-                }
-            ).with_automatic_reconnect({
-                "type": "raw",
-                "keep_alive_interval": 10,
-                "reconnect_interval": 5,
-                "max_attempts": 5
-            }).build()
-        
-        self.hub_connection.on_open(lambda: print("connection opened and handshake received ready to send messages"))
-        self.hub_connection.on_close(lambda: print("connection closed"))
-        
-        success = self.hub_connection.start()
-        pytime.sleep(5)
-        
-        if not success:
-            raise ValueError("connection failed")        
-    def fetch_bearer_token (self):
-        return self.enact_credentials.bearer_token
-              
-    def add_subscription(self, request_object, handle_data):
-        pytime.sleep(3)
-        enact_push_response = self.hub_connection.send("JoinEnactPush", request_object, lambda m: self.callback_received(m.result, handle_data))
-        if not enact_push_response:
-            banana = 1
-    
-    def callback_received(self, m, handle_data):
-        self.hub_connection.on(m['data']['pushName'], handle_data)
-    
-    def terminate_hub_connection(self): 
-        self.hub_connection.stop()
-        
-    def subscribe_to_epex_trade_updates(self, handle_data_method):
-        enact_request_object_epex = [{ "Type" : "EPEX", "Group" : "Trades"}]
-        self.add_subscription(enact_request_object_epex, handle_data_method)
-
-    def subscribe_to_series_updates(self, handle_data_method, series_id, option_id = None, country_id = "Gb"):
-        
-        request_details = {
-            "SeriesId" : series_id,
-            "CountryId" : country_id
-        }
-        
-        if option_id is not None:
-            request_details["OptionId"] = option_id
-        
-        enact_request_object_series = [ request_details ]
-        self.add_subscription(enact_request_object_series, handle_data_method)    
-
-        
+        return response
```

