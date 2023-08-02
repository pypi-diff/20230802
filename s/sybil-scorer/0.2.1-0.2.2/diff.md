# Comparing `tmp/sybil-scorer-0.2.1.tar.gz` & `tmp/sybil-scorer-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sybil-scorer-0.2.1.tar", last modified: Sun Jul  9 20:37:18 2023, max compression
+gzip compressed data, was "sybil-scorer-0.2.2.tar", last modified: Wed Aug  2 15:48:16 2023, max compression
```

## Comparing `sybil-scorer-0.2.1.tar` & `sybil-scorer-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 20:37:18.475887 sybil-scorer-0.2.1/
--rw-rw-rw-   0        0        0     1084 2023-01-29 12:58:09.000000 sybil-scorer-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     9689 2023-07-09 20:37:18.475887 sybil-scorer-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     7755 2023-05-05 09:28:10.000000 sybil-scorer-0.2.1/README.md
--rw-rw-rw-   0        0        0     1142 2023-07-09 20:36:13.000000 sybil-scorer-0.2.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-09 20:37:18.393647 sybil-scorer-0.2.1/sbscorer/
-drwxrwxrwx   0        0        0        0 2023-07-09 20:37:18.415215 sybil-scorer-0.2.1/sbscorer/sbdata/
--rw-rw-rw-   0        0        0    24311 2023-07-08 21:12:35.000000 sybil-scorer-0.2.1/sbscorer/sbdata/FlipsideApi.py
--rw-rw-rw-   0        0        0        0 2023-01-17 19:51:41.000000 sybil-scorer-0.2.1/sbscorer/sbdata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 20:37:18.436217 sybil-scorer-0.2.1/sbscorer/sblegos/
--rw-rw-rw-   0        0        0    30118 2023-07-08 20:54:57.000000 sybil-scorer-0.2.1/sbscorer/sblegos/TransactionAnalyser.py
--rw-rw-rw-   0        0        0     9373 2023-06-09 19:15:54.000000 sybil-scorer-0.2.1/sbscorer/sblegos/TransactionAnalyserTest.py
--rw-rw-rw-   0        0        0        0 2023-01-21 08:46:58.000000 sybil-scorer-0.2.1/sbscorer/sblegos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 20:37:18.446552 sybil-scorer-0.2.1/sbscorer/sbutils/
--rw-rw-rw-   0        0        0     5318 2023-01-30 19:57:35.000000 sybil-scorer-0.2.1/sbscorer/sbutils/LoadData.py
--rw-rw-rw-   0        0        0        0 2023-01-17 19:51:41.000000 sybil-scorer-0.2.1/sbscorer/sbutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 20:37:18.473887 sybil-scorer-0.2.1/sbscorer/sybil_scorer.egg-info/
--rw-rw-rw-   0        0        0     9689 2023-07-09 20:37:18.000000 sybil-scorer-0.2.1/sbscorer/sybil_scorer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      496 2023-07-09 20:37:18.000000 sybil-scorer-0.2.1/sbscorer/sybil_scorer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 20:37:18.000000 sybil-scorer-0.2.1/sbscorer/sybil_scorer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      150 2023-07-09 20:37:18.000000 sybil-scorer-0.2.1/sbscorer/sybil_scorer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-07-09 20:37:18.000000 sybil-scorer-0.2.1/sbscorer/sybil_scorer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      748 2023-07-09 20:37:18.477886 sybil-scorer-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-02 15:48:16.027459 sybil-scorer-0.2.2/
+-rw-rw-rw-   0        0        0     1084 2023-01-29 12:58:09.000000 sybil-scorer-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     7800 2023-08-02 15:48:16.027459 sybil-scorer-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5918 2023-08-02 15:47:13.000000 sybil-scorer-0.2.2/README.md
+-rw-rw-rw-   0        0        0     1170 2023-08-02 15:12:40.000000 sybil-scorer-0.2.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-08-02 15:48:15.987835 sybil-scorer-0.2.2/sbscorer/
+drwxrwxrwx   0        0        0        0 2023-08-02 15:48:15.994325 sybil-scorer-0.2.2/sbscorer/sbdata/
+-rw-rw-rw-   0        0        0    24342 2023-07-10 06:10:34.000000 sybil-scorer-0.2.2/sbscorer/sbdata/FlipsideApi.py
+-rw-rw-rw-   0        0        0        0 2023-01-17 19:51:41.000000 sybil-scorer-0.2.2/sbscorer/sbdata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 15:48:15.994325 sybil-scorer-0.2.2/sbscorer/sblegos/
+-rw-rw-rw-   0        0        0    29815 2023-07-10 06:10:34.000000 sybil-scorer-0.2.2/sbscorer/sblegos/TransactionAnalyser.py
+-rw-rw-rw-   0        0        0     9373 2023-06-09 19:15:54.000000 sybil-scorer-0.2.2/sbscorer/sblegos/TransactionAnalyserTest.py
+-rw-rw-rw-   0        0        0        0 2023-01-21 08:46:58.000000 sybil-scorer-0.2.2/sbscorer/sblegos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 15:48:16.002356 sybil-scorer-0.2.2/sbscorer/sbutils/
+-rw-rw-rw-   0        0        0     5318 2023-01-30 19:57:35.000000 sybil-scorer-0.2.2/sbscorer/sbutils/LoadData.py
+-rw-rw-rw-   0        0        0        0 2023-01-17 19:51:41.000000 sybil-scorer-0.2.2/sbscorer/sbutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 15:48:16.027459 sybil-scorer-0.2.2/sbscorer/sybil_scorer.egg-info/
+-rw-rw-rw-   0        0        0     7800 2023-08-02 15:48:15.000000 sybil-scorer-0.2.2/sbscorer/sybil_scorer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      486 2023-08-02 15:48:15.000000 sybil-scorer-0.2.2/sbscorer/sybil_scorer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 15:48:15.000000 sybil-scorer-0.2.2/sbscorer/sybil_scorer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      150 2023-08-02 15:48:15.000000 sybil-scorer-0.2.2/sbscorer/sybil_scorer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-08-02 15:48:15.000000 sybil-scorer-0.2.2/sbscorer/sybil_scorer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 15:48:16.027459 sybil-scorer-0.2.2/setup.cfg
```

### Comparing `sybil-scorer-0.2.1/LICENSE` & `sybil-scorer-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sybil-scorer-0.2.1/sbscorer/sbdata/FlipsideApi.py` & `sybil-scorer-0.2.2/sbscorer/sbdata/FlipsideApi.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         # return up to 100,000 results per GET request on the query id
         self.PAGE_SIZE = page_size
         # timeout in minutes
         self.TIMEOUT_MINUTES = timeout_minutes
         # return results of page 1
         self.PAGE_NUMBER = page_number
         # max address to query.
-        # It is not recommended to go above 10000 it already takes a long time and it depends on the network
+        # It is not recommended to go above 10000 it already takes a long time, and it depends on the network
         # You will probably have to run more queries because either the query times out or the max rows is reached
         # At 100 tx per address the 1 million rows is reached if you use max_address=10000
         # At 1000 tx per address the 1 million rows is reached if you use max_address=1000
         # on ethereum 1000 or 2000 should be fine but on polygon it is better to use 500
         self.MAX_ADDRESS = max_address
         # TTL for the query id in minutes
         self.TTL_MINUTES = ttl
@@ -586,15 +586,15 @@
                     {string_limit};
                     """
         return sql
 
     def get_cross_chain_info_sql_query(self, array_address, info_type="label", limit=0):
         """
         Get the sql query to extract the cross chain labels or tags for the array of addresses.
-        WARNING you should not provide to much addresses in the array_address parameter because the query may time out.
+        WARNING you should not provide too many addresses in the array_address parameter because the query may time out.
         Parameters
         ----------
         array_address : array
             The array of addresses to extract
         info_type : str
             The type of info to extract. It can be "label" or "tag"
         limit : int
@@ -609,14 +609,15 @@
         str_list_add = self.get_string_address(array_address)
         if info_type == "label":
             table_name = "crosschain.address_labels"
         elif info_type == "tag":
             table_name = "crosschain.address_tags"
         else:
             Exception("Invalid info type")
+            table_name = ""
         if limit != 0:
             string_limit = f"LIMIT {limit}"
         else:
             string_limit = ""
 
         sql = f"""
                 SELECT *
```

### Comparing `sybil-scorer-0.2.1/sbscorer/sblegos/TransactionAnalyser.py` & `sybil-scorer-0.2.2/sbscorer/sblegos/TransactionAnalyser.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,31 +241,33 @@
             Set the details_first_incoming_transaction attribute of the class
 
         """
         df_filtered = self.df_transactions[self.df_transactions['EOA'] == self.df_transactions['to_address']]
         df_gb = df_filtered.sort_values('block_timestamp', ascending=True).groupby('EOA').first()
         cols = ['from_address', 'gas_limit', 'gas_used', 'eth_value', 'block_timestamp']
         df_gb_first = df_gb.loc[:, cols].reset_index()
-        self.details_first_incoming_transaction = df_gb_first.rename(columns=dict(from_address='first_in_tx_from',
-                                                                                  gas_limit='first_in_tx_gas_limit',
-                                                                                  gas_used='first_in_tx_gas_used',
-                                                                                  eth_value='first_in_tx_eth_value',
-                                                                                  block_timestamp='first_in_tx_timestamp'))
+        self.details_first_incoming_transaction = df_gb_first.rename(
+            columns=dict(from_address='first_in_tx_from',
+                         gas_limit='first_in_tx_gas_limit',
+                         gas_used='first_in_tx_gas_used',
+                         eth_value='first_in_tx_eth_value',
+                         block_timestamp='first_in_tx_timestamp'))
 
     def set_details_first_outgoing_transaction(self):
 
         df_filtered = self.df_transactions[self.df_transactions['EOA'] == self.df_transactions['from_address']]
         df_gb = df_filtered.sort_values('block_timestamp', ascending=True).groupby('EOA').first()
         cols = ['to_address', 'gas_limit', 'gas_used', 'eth_value', 'block_timestamp']
         df_gb_first = df_gb.loc[:, cols].reset_index()
-        self.details_first_outgoing_transaction = df_gb_first.rename(columns=dict(from_address='first_out_tx_from',
-                                                                                  gas_limit='first_out_tx_gas_limit',
-                                                                                  gas_used='first_out_tx_gas_used',
-                                                                                  eth_value='first_out_tx_eth_value',
-                                                                                  block_timestamp='first_out_tx_timestamp'))
+        self.details_first_outgoing_transaction = df_gb_first.rename(
+            columns=dict(from_address='first_out_tx_from',
+                         gas_limit='first_out_tx_gas_limit',
+                         gas_used='first_out_tx_gas_used',
+                         eth_value='first_out_tx_eth_value',
+                         block_timestamp='first_out_tx_timestamp'))
 
     def has_less_than_n_transactions(self, address, n=5):
         """
         Return a boolean whether the address has less than n transactions
         Parameters
         ----------
         address : str
@@ -416,64 +418,65 @@
         address : str
             The address to check
         algo_type : str
             The type of algorithm to use. Default is "address_only" which only use the address to compare.
             options are: address_only, address_and_value
         minimum_sim_tx : int
             The number of transactions to use to compare. Default is 5.
-        char_tolerance : int
-            The number of character to skip when using the longest common substring algorithm. Default is 0.
-            1 may be a good choice when algo_type is "address_and_value".
+        # char_tolerance : int
+        #     The number of character to skip when using the longest common substring algorithm. Default is 0.
+        #     1 may be a good choice when algo_type is "address_and_value".
 
         Returns
         -------
         has_similar_behavior : bool
             True if the address has similar behavior as another address
         score_similar_behavior : float
             The similarity score of the address
         list_similar_address : map
             The map of address and their similarity score
 
         """
 
+        str_transactions_target = None
         # Transform all transactions into a 1D string
         if algo_type == "address_only":
             if self.dict_add_string_tx is None:
                 self.set_dict_add_string_transactions(algo_type)
             str_transactions_target = self.dict_add_string_tx.get(address)
         elif algo_type == "address_and_value":
             if self.dict_add_value_string_tx is None:
                 self.set_dict_add_string_transactions(algo_type)
             # Get all the transactions of the address in a 1D array
             str_transactions_target = self.dict_add_value_string_tx.get(address)
         else:
             Exception("algo_type not supported")
 
         shape_target = self.get_address_transactions(address).shape[0]
-        min_shape = max(1, shape_target / 4)
+        min_shape = max(1, int(shape_target / 4))
         max_shape = max(shape_target, shape_target * 3)
 
         list_lcs = []
         for add in self.array_address:
             if add != address:
                 shape_other = self.get_address_transactions(add).shape[0]
-                if min_shape < shape_other < max_shape:  # Heuristic to avoid comparing addresses with too different shapes
+                if min_shape < shape_other < max_shape:  # Heuristic prevent comparing addresses with different shapes
                     if algo_type == "address_only":
                         str_transactions_other = self.dict_add_string_tx.get(add)
                     else:
                         str_transactions_other = self.dict_add_value_string_tx.get(add)
                     lcs = self.longest_common_sub_string_pylcs(str_transactions_target, str_transactions_other)
                     list_lcs.append(lcs)
                 else:
                     list_lcs.append(0)
             else:
                 list_lcs.append(0)
 
         if minimum_sim_tx == -1:
-            mask = np.array(list_lcs) > max(3, min(10, shape_target / 4))
+            mask = np.array(list_lcs) > max(3, min(10, int(shape_target / 4)))
         else:
             mask = np.array(list_lcs) > minimum_sim_tx
         df_similar_address = pd.DataFrame(self.array_address[mask], columns=['address'])
         df_similar_address['lcs'] = np.array(list_lcs)[mask]
         len_tx = len(str_transactions_target) / 2  # Divide by 2 because we have from_address and to_address
         df_similar_address['score'] = df_similar_address.loc[:, 'lcs'].apply(
             lambda x: min(x / len_tx, 1))
@@ -509,23 +512,25 @@
                 array_transactions = df_address_transactions.loc[:, ['from_address', 'to_address']].dropna() \
                     .apply(lambda x: x.str[:8]) \
                     .replace(address[:8], 'x') \
                     .agg('-'.join, axis=1) \
                     .values
             except Exception as e:
                 array_transactions = []
+                print(e)
         elif algo_type == "address_and_value":
             try:
                 array_transactions = df_address_transactions.loc[:, ['from_address', 'value', 'to_address']].dropna() \
                     .apply(lambda x: x.str[:8]) \
                     .replace(address, 'x') \
                     .agg('-'.join, axis=1) \
                     .values
             except Exception as e:
                 array_transactions = []
+                print(e)
         else:
             raise ValueError("algo_type must be either address_only or address_and_value")
         return array_transactions
 
     def get_address_transactions(self, address):
         """
         Get transactions of an address from the self.df_transaction df using the group by
@@ -540,14 +545,15 @@
             The data frame with the transactions of the address
 
         """
         try:
             df = self.gb_EOA_sorted.get_group(address)
         except Exception as e:
             df = pd.DataFrame()
+            print(e)
         return df
 
     def get_address_transactions_add(self, df, address):
         """
         Get transactions of an address from a dataframe df
         Parameters
         ----------
```

### Comparing `sybil-scorer-0.2.1/sbscorer/sblegos/TransactionAnalyserTest.py` & `sybil-scorer-0.2.2/sbscorer/sblegos/TransactionAnalyserTest.py`

 * *Files identical despite different names*

### Comparing `sybil-scorer-0.2.1/sbscorer/sbutils/LoadData.py` & `sybil-scorer-0.2.2/sbscorer/sbutils/LoadData.py`

 * *Files identical despite different names*

