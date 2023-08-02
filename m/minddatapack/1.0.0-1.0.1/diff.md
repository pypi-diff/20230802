# Comparing `tmp/minddatapack-1.0.0.tar.gz` & `tmp/minddatapack-1.0.1.tar.gz`

## Comparing `minddatapack-1.0.0.tar` & `minddatapack-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 minddatapack-1.0.0/minddatapack/__init__.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 minddatapack-1.0.0/minddatapack/arweaveconnector.py
--rw-r--r--   0        0        0    11327 2020-02-02 00:00:00.000000 minddatapack-1.0.0/minddatapack/localfileconnector.py
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 minddatapack-1.0.0/minddatapack/mindlakeconnector.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 minddatapack-1.0.0/minddatapack/utils.py
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 minddatapack-1.0.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 minddatapack-1.0.0/LICENSE
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 minddatapack-1.0.0/README.md
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 minddatapack-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 minddatapack-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 minddatapack-1.0.1/minddatapack/__init__.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 minddatapack-1.0.1/minddatapack/arweaveconnector.py
+-rw-r--r--   0        0        0     3766 2020-02-02 00:00:00.000000 minddatapack-1.0.1/minddatapack/ipfsconnector.py
+-rw-r--r--   0        0        0    11414 2020-02-02 00:00:00.000000 minddatapack-1.0.1/minddatapack/localfileconnector.py
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 minddatapack-1.0.1/minddatapack/mindlakeconnector.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 minddatapack-1.0.1/minddatapack/utils.py
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 minddatapack-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 minddatapack-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 minddatapack-1.0.1/README.md
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 minddatapack-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 minddatapack-1.0.1/PKG-INFO
```

### Comparing `minddatapack-1.0.0/minddatapack/__init__.py` & `minddatapack-1.0.1/minddatapack/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 name = "minddatapack"
 
 import mindlakesdk
 from mindlakesdk.utils import ResultType, DataType
 from web3 import Web3
+import importlib.metadata
 import minddatapack.arweaveconnector
 import minddatapack.mindlakeconnector
 import minddatapack.localfileconnector
+import minddatapack.ipfsconnector
 from minddatapack.utils import Column
 
 class DataPack:
     DataType = DataType
     Column = Column
 
     def __init__(self, walletPrivateKey: str):
         self.existData = False
         self.__columns = None
         self.data = None
         self.columnName = None
         self.fileName = None
-        self.filePath = None
         self.primaryKey = None
+        self.version = importlib.metadata.version('minddatapack')
         self.__walletPrivateKey = walletPrivateKey
         web3 = Web3(Web3.HTTPProvider(mindlakesdk.settings.WEB3API))
         self.__walletAccount = web3.eth.account.from_key(walletPrivateKey)
 
     def loadFromMindByQuery(self, sqlStatement: str, mindLake: mindlakesdk.MindLake) -> ResultType:
         result, self.__columns = minddatapack.mindlakeconnector.loadFromMindByQuery(self, sqlStatement, mindLake)
         return result
@@ -43,7 +45,13 @@
         return minddatapack.localfileconnector.loadFromCSVFileByDefineColumn(self, csvFilePath, columns)
 
     def saveToArweave(self, fileName: str, tokenName: str, arWalletFile: str = None):
         return minddatapack.arweaveconnector.saveToArweave(self, fileName, tokenName, arWalletFile, self.__walletPrivateKey)
 
     def loadFromArweave(self, id: str, arGateway: str = 'https://arseed.web3infra.dev/'):
         return minddatapack.arweaveconnector.loadFromArweave(self, id, arGateway)
+
+    def saveToIPFS(self, fileName: str, apiEndpoint: str = 'http://localhost:5001', apiKey: str = None, apiSecret: str = None):
+        return minddatapack.ipfsconnector.saveToIPFS(self, fileName, apiEndpoint, apiKey, apiSecret)
+
+    def loadFromIPFS(self, ipfsCID: str, apiEndpoint: str = 'http://localhost:5001', apiKey: str = None, apiSecret: str = None):
+        return minddatapack.ipfsconnector.loadFromIPFS(self, ipfsCID, apiEndpoint, apiKey, apiSecret)
```

### Comparing `minddatapack-1.0.0/minddatapack/arweaveconnector.py` & `minddatapack-1.0.1/minddatapack/arweaveconnector.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import os
 import logging
 import requests
+from datetime import datetime
 from mindlakesdk.utils import ResultType
 import minddatapack.utils
 
 def saveToArweave(dataPack, fileName: str, tokenName: str, arWalletFile: str, ethWalletPrivateKey: str):
     result = dataPack.saveToLocalFile(fileName)
     if not result:
         return result
@@ -32,40 +33,37 @@
     finally:
         if os.path.exists(dataFileName):
             os.remove(dataFileName)
         if os.path.exists(metaFileName):
             os.remove(metaFileName)
 
 def loadFromArweave(dataPack, id: str, arGateway: str):
-    metaFileName = None
-    dataFileName = None
+    cacheDataFileName = minddatapack.utils.CACHE_PREFIX + datetime.now().strftime("%Y%m%d%H%M%S%f") + '.csv'
+    cacheMetaFileName = cacheDataFileName + minddatapack.utils.METADATA_EXT
     try:
         if arGateway[-1] != '/':
             arGateway += '/'
         metaUrl = arGateway + 'bundle/tx/' + id
         metaResponse = requests.get(metaUrl)
         if metaResponse and metaResponse.status_code == 200:
             txMeta = json.loads(metaResponse.text)
             metadataJsonStr = txMeta['tags'][1]['value']
-            metadata = json.loads(metadataJsonStr)
-            dataFileName = metadata['FileName']
-            metaFileName = dataFileName + minddatapack.utils.METADATA_EXT
-            with open(metaFileName, 'wb') as file:
+            with open(cacheMetaFileName, 'wb') as file:
                 file.write(metadataJsonStr.encode('utf-8'))
             
             dataUrl = arGateway + id
             dataResponse = requests.get(dataUrl)
             if dataResponse and dataResponse.status_code == 200:
-                with open(dataFileName, 'wb') as file:
+                with open(cacheDataFileName, 'wb') as file:
                     file.write(dataResponse.content)
 
-            return dataPack.loadFromLocalFile(dataFileName)
+            return dataPack.loadFromLocalFile(cacheDataFileName)
         else:
             return ResultType(60001, "Network error", None)
     except Exception as e:
         logging.debug("Exception:", str(e))
         return ResultType(60014, "Fail to connect to Arweave", None)
     finally:
-        if dataFileName and os.path.exists(dataFileName):
-            os.remove(dataFileName)
-        if metaFileName and os.path.exists(metaFileName):
-            os.remove(metaFileName)
+        if os.path.exists(cacheDataFileName):
+            os.remove(cacheDataFileName)
+        if os.path.exists(cacheMetaFileName):
+            os.remove(cacheMetaFileName)
```

### Comparing `minddatapack-1.0.0/minddatapack/localfileconnector.py` & `minddatapack-1.0.1/minddatapack/localfileconnector.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,46 +52,46 @@
 def saveToLocalFile(dataPack, filePath: str, ignoreEncrypt: bool, columns: list, walletAccount):
     if not dataPack.existData:
         return ResultType(60006, 'No data in DataPack')
     dataPack.fileName = os.path.basename(filePath)
     with open(filePath, 'w') as file:
         writer = csv.writer(file)
         writer.writerow(dataPack.columnName)
-        if ignoreEncrypt:
-            for row in dataPack.data:
-                writer.writerow(row)
-        else:
-            for row in dataPack.data:
-                rowEncrypted = []
-                for index, cell in enumerate(row):
-                    if columns[index].encrypt:
-                        encryptResult = __encrypt(cell, columns[index])
-                        if not encryptResult:
-                            return encryptResult
-                        rowEncrypted.append(encryptResult.data)
+        for row in dataPack.data:
+            rowEncoded = []
+            for index, cell in enumerate(row):
+                if not ignoreEncrypt and columns[index].encrypt:
+                    encryptResult = __encrypt(cell, columns[index])
+                    if not encryptResult:
+                        return encryptResult
+                    rowEncoded.append(encryptResult.data)
+                else:
+                    if columns[index].type == DataType.timestamp:
+                        rowEncoded.append(cell.strftime('%Y-%m-%d %H:%M:%S.%f'))
                     else:
-                        rowEncrypted.append(cell)
-                writer.writerow(rowEncrypted)
+                        rowEncoded.append(str(cell))
+            writer.writerow(rowEncoded)
 
     sha256_hash = SHA256.new()
     with open(filePath, 'rb') as file:
         for chunk in iter(lambda: file.read(4096), b''):
             sha256_hash.update(chunk)
     sha256_hash_hex = sha256_hash.hexdigest()
 
-    metadata = __buildMetadata(dataPack.fileName, ignoreEncrypt, sha256_hash_hex, columns, walletAccount)
+    metadata = __buildMetadata(dataPack.fileName, ignoreEncrypt, sha256_hash_hex, columns, walletAccount, dataPack.version)
     with open(filePath+minddatapack.utils.METADATA_EXT, 'w') as file:
         json.dump(metadata, file)
     return ResultType(0, None)
 
-def __buildMetadata(fileName: str, ignoreEncrypt: bool, fileHash: str, columns: list, walletAccount) -> dict:
+def __buildMetadata(fileName: str, ignoreEncrypt: bool, fileHash: str, columns: list, walletAccount, version: str) -> dict:
     metadata = {}
     metadata['FileName'] = fileName
     metadata['IgnoreEncrypt'] = ignoreEncrypt
     metadata['FileHash'] = fileHash
+    metadata['Version'] = version
     metadata['Column'] = []
     for column in columns:
         columnMeta = {}
         columnMeta['ColumnName'] = column.columnName
         columnMeta['DataType'] = column.type.name
         columnMeta['Encrypt'] = column.encrypt
         if column.encrypt:
@@ -124,33 +124,33 @@
                 columnMeta = minddatapack.utils.Column(column['ColumnName'], DataType[column['DataType']], column['Encrypt'])
             columns.append(columnMeta)
     with open(filePath, 'r') as file:
         reader = csv.reader(file)
         dataPack.columnName = next(reader)
         dataPack.data = []
         for row in reader:
-            rowDecrypted = []
+            rowDecoded = []
             for index, cell in enumerate(row):
                 if not ignoreEncrypt and columns[index].encrypt:
                     decryptResult = __decrypt(cell, columns[index])
                     if not decryptResult:
                         return decryptResult
-                    rowDecrypted.append(decryptResult.data)
+                    rowDecoded.append(decryptResult.data)
                 else:
                     if columns[index].type == DataType.int4 or columns[index].type == DataType.int8:
-                        rowDecrypted.append(int(cell))
+                        rowDecoded.append(int(cell))
                     elif columns[index].type == DataType.float4 or columns[index].type == DataType.float8:
-                        rowDecrypted.append(float(cell))
+                        rowDecoded.append(float(cell))
                     elif columns[index].type == DataType.decimal:
-                        rowDecrypted.append(Decimal(cell))
+                        rowDecoded.append(Decimal(cell))
                     elif columns[index].type == DataType.timestamp:
-                        rowDecrypted.append(datetime.datetime.strptime(cell, '%Y-%m-%d %H:%M:%S.%f'))
+                        rowDecoded.append(datetime.datetime.strptime(cell, '%Y-%m-%d %H:%M:%S.%f'))
                     else:
-                        rowDecrypted.append(cell)
-            dataPack.data.append(rowDecrypted)
+                        rowDecoded.append(cell)
+            dataPack.data.append(rowDecoded)
         dataPack.existData = True
     return ResultType(0, "Success"), columns
 
 def loadFromCSVFileByDefineColumn(dataPack, csvFilePath: str, columns: list):
     # the whole csv file should be in plain text
     if not os.path.exists(csvFilePath):
         return ResultType(60007, 'CSV File not found')
```

### Comparing `minddatapack-1.0.0/minddatapack/mindlakeconnector.py` & `minddatapack-1.0.1/minddatapack/mindlakeconnector.py`

 * *Files identical despite different names*

### Comparing `minddatapack-1.0.0/minddatapack/utils.py` & `minddatapack-1.0.1/minddatapack/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import mindlakesdk
 from mindlakesdk.utils import ResultType, DataType
 from mindlakesdk.datalake import DataLake
 
 METADATA_EXT = '.meta.json'
+CACHE_PREFIX = 'datapack_cache_'
 
 class Column(DataLake.Column):
     def __init__(self, columnName: str, dataType: DataType, encrypt: bool, dataKey: bytes = None):
         super().__init__(columnName, dataType, encrypt)
         if encrypt:
             if dataKey:
                 self.dataKey = dataKey
```

### Comparing `minddatapack-1.0.0/.gitignore` & `minddatapack-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `minddatapack-1.0.0/LICENSE` & `minddatapack-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `minddatapack-1.0.0/README.md` & `minddatapack-1.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 DataPack, contributed by the Mind Network Team, is to enable data transformation and transportation between Mind Network and storage protocols, like Arweave. It is an adapter that facilitates the smooth conversion of data between plaintext and ciphertext to be stored in Mind Network or Arweave. This module empowers users to retrieve their infrequently processed data, known as "cold data," from Mind Network and store it in local or decentralized storage. When the need arises to perform computing on the encrypted data again, users can effortlessly load it back into Mind Network for processing.
 
 
 ## Getting Started
 
 ### Dependencies
 
-* Python > 3.8
+* Python >= 3.8
 * pip
 * mindlakesdk
 * arseeding
 
 ### Installing
 
 * pip install minddatapack
@@ -26,21 +26,23 @@
 ```
 from minddatapack import DataPack
 ...
 ```
 
 ### More examples
 * [use case of arweave in jupyter](/examples/use_case_arweave.ipynb)
+* [use case of IPFS in jupyter](/examples/use_case_ipfs.ipynb)
 
 ## code
 ```
 mind-datapack-python
 |-- minddatapack # source code
 |   |-- __init__.py
 |   |-- arweaveconnector.py
+|   |-- ipfsconnector.py
 |   |-- localfileconnector.py
 |   |-- mindlakeconnector.py
 |   └-- utils.py
 |-- examples # use case examples
 |-- README.md
 └--- LICENSE
 
@@ -55,11 +57,13 @@
 * Dennis [@NuIlPtr](https://twitter.com/nuilptr)
 * George [@georgemindnet](https://twitter.com/georgemindnet)
 
 ## Version History
 
 * v1.0
     * Initial Release
+* v1.0.1
+    * Add IPFS support
 
 ## License
 
 This project is licensed under the [MIT] License - see the LICENSE.md file for details
```

### Comparing `minddatapack-1.0.0/pyproject.toml` & `minddatapack-1.0.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "minddatapack"
-version = "v1.0.0"
+version = "v1.0.1"
 authors = [
   { name="Mind Labs", email="biz@mindnetwork.xyz" },
 ]
 description = "A Python SDK to migrate data between Mind Lake and other storages"
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 keywords = ["web3", "encryption", "datalake"]
 dependencies = [
     "mindlakesdk",
     "arseeding"
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/mind-network/mind-lake-sdk-python"
-"Bug Tracker" = "https://github.com/mind-network/mind-lake-sdk-python/issues"
+"Homepage" = "https://github.com/mind-network/mind-datapack-python"
+"Bug Tracker" = "https://github.com/mind-network/mind-datapack-python/issues"
 
 [tool.hatch.build]
 exclude = ["/examples", "/tests", "/tutorial"]
```

### Comparing `minddatapack-1.0.0/PKG-INFO` & `minddatapack-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: minddatapack
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python SDK to migrate data between Mind Lake and other storages
-Project-URL: Homepage, https://github.com/mind-network/mind-lake-sdk-python
-Project-URL: Bug Tracker, https://github.com/mind-network/mind-lake-sdk-python/issues
+Project-URL: Homepage, https://github.com/mind-network/mind-datapack-python
+Project-URL: Bug Tracker, https://github.com/mind-network/mind-datapack-python/issues
 Author-email: Mind Labs <biz@mindnetwork.xyz>
 License-File: LICENSE
 Keywords: datalake,encryption,web3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Requires-Dist: arseeding
 Requires-Dist: mindlakesdk
 Description-Content-Type: text/markdown
 
 # Mind DataPack Python SDK
 
 An Python implementation for Mind DataPack
@@ -26,15 +26,15 @@
 DataPack, contributed by the Mind Network Team, is to enable data transformation and transportation between Mind Network and storage protocols, like Arweave. It is an adapter that facilitates the smooth conversion of data between plaintext and ciphertext to be stored in Mind Network or Arweave. This module empowers users to retrieve their infrequently processed data, known as "cold data," from Mind Network and store it in local or decentralized storage. When the need arises to perform computing on the encrypted data again, users can effortlessly load it back into Mind Network for processing.
 
 
 ## Getting Started
 
 ### Dependencies
 
-* Python > 3.8
+* Python >= 3.8
 * pip
 * mindlakesdk
 * arseeding
 
 ### Installing
 
 * pip install minddatapack
@@ -43,21 +43,23 @@
 ```
 from minddatapack import DataPack
 ...
 ```
 
 ### More examples
 * [use case of arweave in jupyter](/examples/use_case_arweave.ipynb)
+* [use case of IPFS in jupyter](/examples/use_case_ipfs.ipynb)
 
 ## code
 ```
 mind-datapack-python
 |-- minddatapack # source code
 |   |-- __init__.py
 |   |-- arweaveconnector.py
+|   |-- ipfsconnector.py
 |   |-- localfileconnector.py
 |   |-- mindlakeconnector.py
 |   └-- utils.py
 |-- examples # use case examples
 |-- README.md
 └--- LICENSE
 
@@ -72,11 +74,13 @@
 * Dennis [@NuIlPtr](https://twitter.com/nuilptr)
 * George [@georgemindnet](https://twitter.com/georgemindnet)
 
 ## Version History
 
 * v1.0
     * Initial Release
+* v1.0.1
+    * Add IPFS support
 
 ## License
 
 This project is licensed under the [MIT] License - see the LICENSE.md file for details
```

