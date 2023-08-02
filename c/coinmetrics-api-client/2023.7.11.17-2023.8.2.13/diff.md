# Comparing `tmp/coinmetrics_api_client-2023.7.11.17.tar.gz` & `tmp/coinmetrics_api_client-2023.8.2.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coinmetrics_api_client-2023.7.11.17.tar", max compression
+gzip compressed data, was "coinmetrics_api_client-2023.8.2.13.tar", max compression
```

## Comparing `coinmetrics_api_client-2023.7.11.17.tar` & `coinmetrics_api_client-2023.8.2.13.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0     1088 2023-07-11 17:15:41.002508 coinmetrics_api_client-2023.7.11.17/LICENSE
--rw-r--r--   0        0        0    20461 2023-07-11 17:15:41.002508 coinmetrics_api_client-2023.7.11.17/README.md
--rw-r--r--   0        0        0       29 2023-07-11 17:23:23.700383 coinmetrics_api_client-2023.7.11.17/coinmetrics/__init__.py
--rw-r--r--   0        0        0    21023 2023-07-11 17:15:41.002508 coinmetrics_api_client-2023.7.11.17/coinmetrics/_catalogs.py
--rw-r--r--   0        0        0     9947 2023-07-11 17:15:41.002508 coinmetrics_api_client-2023.7.11.17/coinmetrics/_data_collection.py
--rw-r--r--   0        0        0     2328 2023-07-11 17:15:41.002508 coinmetrics_api_client-2023.7.11.17/coinmetrics/_exceptions.py
--rw-r--r--   0        0        0     1286 2023-07-11 17:15:41.002508 coinmetrics_api_client-2023.7.11.17/coinmetrics/_models.py
--rw-r--r--   0        0        0      699 2023-07-11 17:15:41.002508 coinmetrics_api_client-2023.7.11.17/coinmetrics/_typing.py
--rw-r--r--   0        0        0     3951 2023-07-11 17:15:41.002508 coinmetrics_api_client-2023.7.11.17/coinmetrics/_utils.py
--rw-r--r--   0        0        0   233688 2023-07-11 17:15:41.002508 coinmetrics_api_client-2023.7.11.17/coinmetrics/api_client.py
--rw-r--r--   0        0        0        0 2023-07-11 20:05:55.696998 coinmetrics_api_client-2023.7.11.17/coinmetrics/build.py
--rw-r--r--   0        0        0      148 2023-07-11 17:15:41.006507 coinmetrics_api_client-2023.7.11.17/coinmetrics/constants.py
--rw-r--r--   0        0        0    20520 2023-07-11 17:15:41.006507 coinmetrics_api_client-2023.7.11.17/coinmetrics/data_exporter.py
--rw-r--r--   0        0        0     8669 2023-07-11 17:15:41.006507 coinmetrics_api_client-2023.7.11.17/coinmetrics/typer_cli.py
--rw-r--r--   0        0        0     1237 2023-07-11 17:23:23.700383 coinmetrics_api_client-2023.7.11.17/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-11 20:05:55.700998 coinmetrics_api_client-2023.7.11.17/test/__init__.py
--rw-r--r--   0        0        0     1640 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/data/catalog_asset_pair_candles.csv
--rw-r--r--   0        0        0      412 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/data/catalog_asset_pairs.csv
--rw-r--r--   0        0        0     2097 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/data/catalog_assets_markets.csv
--rw-r--r--   0        0        0      605 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/data/catalog_assets_metrics.csv
--rw-r--r--   0        0        0      436 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/data/catalog_exchange_assets.csv
--rw-r--r--   0        0        0     3595 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/data/catalog_exchanges_markets.csv
--rw-r--r--   0        0        0      822 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/data/catalog_exchanges_metrics.csv
--rw-r--r--   0        0        0      556 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/data/catalog_indexes.csv
--rw-r--r--   0        0        0      223 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/data/catalog_institutions.csv
--rw-r--r--   0        0        0      178 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/data/catalog_market_orderbooks.csv
--rw-r--r--   0        0        0      254 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/data/catalog_market_quotes.csv
--rw-r--r--   0        0        0      297 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/data/catalog_market_trades.csv
--rw-r--r--   0        0        0      582 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/data/catalog_markets.csv
--rw-r--r--   0        0        0     2557 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/data/catalog_metrics.csv
--rw-r--r--   0        0        0    28630 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/test_api_client.py
--rw-r--r--   0        0        0    10311 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/test_api_methods.py
--rw-r--r--   0        0        0     2910 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/test_as_list.py
--rw-r--r--   0        0        0     1788 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/test_blockchain_methods.py
--rw-r--r--   0        0        0     2273 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/test_custom_exceptions.py
--rw-r--r--   0        0        0    13462 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/test_data_exporter.py
--rw-r--r--   0        0        0     1015 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/test_debugging.py
--rw-r--r--   0        0        0     2142 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/test_models.py
--rw-r--r--   0        0        0     1193 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/test_rate_limits.py
--rw-r--r--   0        0        0    15850 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/test_to_dataframe.py
--rw-r--r--   0        0        0     5829 2023-07-11 17:15:41.046508 coinmetrics_api_client-2023.7.11.17/test/test_websocket_methods.py
--rw-r--r--   0        0        0    21650 1970-01-01 00:00:00.000000 coinmetrics_api_client-2023.7.11.17/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-07-31 14:00:54.331639 coinmetrics_api_client-2023.8.2.13/LICENSE
+-rw-r--r--   0        0        0    20461 2023-07-31 14:00:54.331639 coinmetrics_api_client-2023.8.2.13/README.md
+-rw-r--r--   0        0        0       28 2023-08-02 13:48:41.943844 coinmetrics_api_client-2023.8.2.13/coinmetrics/__init__.py
+-rw-r--r--   0        0        0    21024 2023-08-01 00:42:44.766831 coinmetrics_api_client-2023.8.2.13/coinmetrics/_catalogs.py
+-rw-r--r--   0        0        0    10454 2023-08-01 00:42:44.766831 coinmetrics_api_client-2023.8.2.13/coinmetrics/_data_collection.py
+-rw-r--r--   0        0        0     2328 2023-07-31 14:00:54.331639 coinmetrics_api_client-2023.8.2.13/coinmetrics/_exceptions.py
+-rw-r--r--   0        0        0     1286 2023-07-31 14:00:54.331639 coinmetrics_api_client-2023.8.2.13/coinmetrics/_models.py
+-rw-r--r--   0        0        0      679 2023-08-01 00:42:44.766831 coinmetrics_api_client-2023.8.2.13/coinmetrics/_typing.py
+-rw-r--r--   0        0        0     3951 2023-07-31 14:00:54.331639 coinmetrics_api_client-2023.8.2.13/coinmetrics/_utils.py
+-rw-r--r--   0        0        0   291412 2023-08-01 00:42:44.770831 coinmetrics_api_client-2023.8.2.13/coinmetrics/api_client.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:56:11.010387 coinmetrics_api_client-2023.8.2.13/coinmetrics/build.py
+-rw-r--r--   0        0        0      148 2023-07-31 14:00:54.331639 coinmetrics_api_client-2023.8.2.13/coinmetrics/constants.py
+-rw-r--r--   0        0        0    20520 2023-07-31 14:00:54.331639 coinmetrics_api_client-2023.8.2.13/coinmetrics/data_exporter.py
+-rw-r--r--   0        0        0     8669 2023-07-31 14:00:54.331639 coinmetrics_api_client-2023.8.2.13/coinmetrics/typer_cli.py
+-rw-r--r--   0        0        0     1234 2023-08-02 13:48:41.955844 coinmetrics_api_client-2023.8.2.13/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-02 13:56:11.010387 coinmetrics_api_client-2023.8.2.13/test/__init__.py
+-rw-r--r--   0        0        0     1640 2023-07-31 14:00:54.375640 coinmetrics_api_client-2023.8.2.13/test/data/catalog_asset_pair_candles.csv
+-rw-r--r--   0        0        0      412 2023-07-31 14:00:54.375640 coinmetrics_api_client-2023.8.2.13/test/data/catalog_asset_pairs.csv
+-rw-r--r--   0        0        0     2097 2023-07-31 14:00:54.375640 coinmetrics_api_client-2023.8.2.13/test/data/catalog_assets_markets.csv
+-rw-r--r--   0        0        0      605 2023-07-31 14:00:54.375640 coinmetrics_api_client-2023.8.2.13/test/data/catalog_assets_metrics.csv
+-rw-r--r--   0        0        0      436 2023-07-31 14:00:54.375640 coinmetrics_api_client-2023.8.2.13/test/data/catalog_exchange_assets.csv
+-rw-r--r--   0        0        0     3595 2023-07-31 14:00:54.375640 coinmetrics_api_client-2023.8.2.13/test/data/catalog_exchanges_markets.csv
+-rw-r--r--   0        0        0      822 2023-07-31 14:00:54.375640 coinmetrics_api_client-2023.8.2.13/test/data/catalog_exchanges_metrics.csv
+-rw-r--r--   0        0        0      556 2023-07-31 14:00:54.375640 coinmetrics_api_client-2023.8.2.13/test/data/catalog_indexes.csv
+-rw-r--r--   0        0        0      223 2023-07-31 14:00:54.375640 coinmetrics_api_client-2023.8.2.13/test/data/catalog_institutions.csv
+-rw-r--r--   0        0        0      178 2023-07-31 14:00:54.375640 coinmetrics_api_client-2023.8.2.13/test/data/catalog_market_orderbooks.csv
+-rw-r--r--   0        0        0      254 2023-07-31 14:00:54.375640 coinmetrics_api_client-2023.8.2.13/test/data/catalog_market_quotes.csv
+-rw-r--r--   0        0        0      297 2023-07-31 14:00:54.375640 coinmetrics_api_client-2023.8.2.13/test/data/catalog_market_trades.csv
+-rw-r--r--   0        0        0      582 2023-07-31 14:00:54.375640 coinmetrics_api_client-2023.8.2.13/test/data/catalog_markets.csv
+-rw-r--r--   0        0        0     2557 2023-07-31 14:00:54.375640 coinmetrics_api_client-2023.8.2.13/test/data/catalog_metrics.csv
+-rw-r--r--   0        0        0    28646 2023-08-01 00:42:44.770831 coinmetrics_api_client-2023.8.2.13/test/test_api_client.py
+-rw-r--r--   0        0        0    10311 2023-07-31 14:00:54.375640 coinmetrics_api_client-2023.8.2.13/test/test_api_methods.py
+-rw-r--r--   0        0        0     2910 2023-07-31 14:00:54.375640 coinmetrics_api_client-2023.8.2.13/test/test_as_list.py
+-rw-r--r--   0        0        0     1788 2023-07-31 14:00:54.375640 coinmetrics_api_client-2023.8.2.13/test/test_blockchain_methods.py
+-rw-r--r--   0        0        0    10642 2023-08-01 00:42:44.770831 coinmetrics_api_client-2023.8.2.13/test/test_catalogs_v2.py
+-rw-r--r--   0        0        0     2273 2023-07-31 14:00:54.375640 coinmetrics_api_client-2023.8.2.13/test/test_custom_exceptions.py
+-rw-r--r--   0        0        0    13462 2023-07-31 14:00:54.375640 coinmetrics_api_client-2023.8.2.13/test/test_data_exporter.py
+-rw-r--r--   0        0        0     1015 2023-07-31 14:00:54.375640 coinmetrics_api_client-2023.8.2.13/test/test_debugging.py
+-rw-r--r--   0        0        0     2142 2023-07-31 14:00:54.375640 coinmetrics_api_client-2023.8.2.13/test/test_models.py
+-rw-r--r--   0        0        0     1193 2023-07-31 14:00:54.375640 coinmetrics_api_client-2023.8.2.13/test/test_rate_limits.py
+-rw-r--r--   0        0        0    15834 2023-07-31 23:08:06.733876 coinmetrics_api_client-2023.8.2.13/test/test_to_dataframe.py
+-rw-r--r--   0        0        0     5829 2023-07-31 14:00:54.375640 coinmetrics_api_client-2023.8.2.13/test/test_websocket_methods.py
+-rw-r--r--   0        0        0    21649 1970-01-01 00:00:00.000000 coinmetrics_api_client-2023.8.2.13/PKG-INFO
```

### Comparing `coinmetrics_api_client-2023.7.11.17/LICENSE` & `coinmetrics_api_client-2023.8.2.13/LICENSE`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.7.11.17/README.md` & `coinmetrics_api_client-2023.8.2.13/README.md`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.7.11.17/coinmetrics/_catalogs.py` & `coinmetrics_api_client-2023.8.2.13/coinmetrics/_catalogs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
+import datetime
+
 from dateutil.parser import isoparse
 from typing import Iterable
 from coinmetrics._typing import DataFrameType, List, Any, Optional
 from logging import getLogger
 
 logger = getLogger("cm_client")
 
 try:
-    import pandas as pd  # type: ignore
+    import pandas as pd
 except ImportError:
-    pd = None
     logger.warning(
         "Pandas export is unavailable. Install pandas to unlock dataframe functions."
     )
 
 
-def _convert_utc(x: Any) -> DataFrameType:
+def _convert_utc(x: Any) -> Optional[datetime.datetime]:
     try:
         return isoparse(x)
     except TypeError:
         return None
 
 
 def _expand_df(key: str, iterable: Iterable[Any]) -> List[Any]:
```

### Comparing `coinmetrics_api_client-2023.7.11.17/coinmetrics/_data_collection.py` & `coinmetrics_api_client-2023.8.2.13/coinmetrics/_data_collection.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,45 @@
+import requests
 from copy import deepcopy
 from gzip import GzipFile
 from io import BytesIO
 from logging import getLogger
 from time import sleep
-from typing import Any, Dict, Iterable, Iterator, List, Optional, cast, Type
+from datetime import datetime
+from typing import Any, Dict, Iterable, Iterator, List, Optional, cast, Type, Callable, Union
 from dateutil.parser import isoparse
-
-import requests
-
 from coinmetrics._typing import (
     DataRetrievalFuncType,
     DataReturnType,
     FilePathOrBuffer,
     UrlParamTypes,
     DataFrameType,
 )
 from coinmetrics._utils import get_file_path_or_buffer
 from coinmetrics._models import AssetChainsData, CoinMetricsAPIModel, TransactionTrackerData
+from importlib import import_module
+orjson_found = True
 try:
+    json = import_module("orjson")
+except ModuleNotFoundError:
+    orjson_found = False
+
+if not orjson_found:
+    import json
+else:
     import orjson as json
-except ImportError:
-    import json  # type: ignore
+
+isoparse_typed: Callable[[Union[str, bytes]], datetime] = isoparse
 
 
 logger = getLogger("cm_client_data_collection")
 
 try:
-    import pandas as pd  # type: ignore
+    import pandas as pd
 except ImportError:
-    pd = None
     logger.info(
         "Pandas export is unavailable. Install pandas to unlock dataframe functions."
     )
 
 
 class CsvExportError(Exception):
     pass
@@ -245,27 +252,29 @@
                         .decode()
                         .strip()
                         .split(",")
                     )
                     datetime_cols = [
                         c for c in columns if c.endswith("_time") or c == "time"
                     ]
-                    df = pd.read_csv(
-                        f,
-                        parse_dates=datetime_cols,
-                        dtype=dtype_mapper,
-                        date_parser=isoparse,
+                    buffer: BytesIO = f
+                    cols: List[str] = datetime_cols
+                    dtype_map: Optional[Dict[str, Any]] = dtype_mapper
+                    df: pd.DataFrame = pd.read_csv(
+                        buffer,
+                        parse_dates=cols,
+                        dtype=dtype_map,
                     )
                     if dtype_mapper is None:
                         df = df.convert_dtypes()
                     if header is not None:
                         assert len(df.columns) == len(
                             header
                         ), "header length does not match output values"
-                        df.columns = header
+                        df.columns = pd.Index(header)
                     return df
             else:
                 if dtype_mapper is None:
                     return pd.DataFrame(self)
                 else:
                     return pd.DataFrame(self).astype(dtype=dtype_mapper)
 
@@ -285,7 +294,13 @@
             df['reorg'] = df['reorg'].apply(lambda reorg: True if reorg == "true" else False)
         return df
 
 
 class TransactionTrackerDataCollection(DataCollection):
 
     API_RETURN_MODEL = TransactionTrackerData
+
+
+class CatalogV2DataCollection(DataCollection):
+    """
+    This class will be used to implement functionality specific to catalog-v2 endpoints.
+    """
```

### Comparing `coinmetrics_api_client-2023.7.11.17/coinmetrics/_exceptions.py` & `coinmetrics_api_client-2023.8.2.13/coinmetrics/_exceptions.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.7.11.17/coinmetrics/_models.py` & `coinmetrics_api_client-2023.8.2.13/coinmetrics/_models.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.7.11.17/coinmetrics/_typing.py` & `coinmetrics_api_client-2023.8.2.13/coinmetrics/_typing.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from datetime import date, datetime
 from pathlib import Path
 from typing import Any, Callable, Dict, IO, List, Tuple, Union, Optional
 from coinmetrics.constants import PagingFrom
+pandas_found = True
 
 try:
-    import pandas as pd  # type: ignore
+    import pandas as pd
 
-    DataFrameType = pd.core.frame.DataFrame
+    DataFrameType = pd.DataFrame
 except ImportError:
-    pd = None
-    DataFrameType = Any
+    pandas_found = False
 
 FilePathOrBuffer = Union[str, Path, IO[str], IO[bytes], None]
 DataReturnType = Dict[str, Union[str, Dict[str, str], List[Dict[str, Any]]]]
 DataRetrievalFuncType = Callable[[str, Dict[str, Any]], DataReturnType]
 UrlParamTypes = Union[
     str, List[str], Tuple[str], PagingFrom, int, datetime, date, bool, None
 ]
```

### Comparing `coinmetrics_api_client-2023.7.11.17/coinmetrics/_utils.py` & `coinmetrics_api_client-2023.8.2.13/coinmetrics/_utils.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.7.11.17/coinmetrics/api_client.py` & `coinmetrics_api_client-2023.8.2.13/coinmetrics/api_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,32 +4,25 @@
 from datetime import date, datetime
 from logging import getLogger
 from typing import Any, Dict, List, Optional, Union, cast
 from urllib.parse import urlencode
 
 import requests
 from requests import HTTPError, Response
-import websocket  # type: ignore
+import websocket
 
 from coinmetrics._utils import retry, transform_url_params_values_to_str
 from coinmetrics import __version__ as version
 from coinmetrics._exceptions import CoinMetricsClientQueryParamsException
-
-try:
-    import ujson as json
-except ImportError:
-    # fall back to std json package
-    import json  # type: ignore
-
 from coinmetrics._typing import (
     DataReturnType,
     MessageHandlerType,
 )
 from coinmetrics.constants import PagingFrom, Backfill
-from coinmetrics._data_collection import DataCollection, AssetChainsDataCollection, TransactionTrackerDataCollection
+from coinmetrics._data_collection import DataCollection, AssetChainsDataCollection, TransactionTrackerDataCollection, CatalogV2DataCollection
 from coinmetrics._catalogs import (
     CatalogAssetsData,
     CatalogAssetAlertsData,
     CatalogAssetPairsData,
     CatalogAssetPairCandlesData,
     CatalogExchangeAssetsData,
     CatalogExchangesData,
@@ -48,23 +41,26 @@
     CatalogMempoolFeeratesData,
     CatalogMiningPoolTipsData,
     CatalogTransactionTrackerData,
     CatalogMarketContractPrices,
     CatalogMarketImpliedVolatility
 )
 
-logger = getLogger("cm_client")
-
+from importlib import import_module
+ujson_found = True
 try:
-    import pandas as pd  # type: ignore
-except ImportError:
-    pd = None
-    logger.warning(
-        "Pandas export is unavailable. Install pandas to unlock dataframe functions."
-    )
+    json = import_module('ujson')
+except ModuleNotFoundError:
+    ujson_found = False
+
+if not ujson_found:
+    import json
+else:
+    import ujson as json
+logger = getLogger("cm_client")
 
 
 class CmStream:
     def __init__(self, ws_url: str):
         self.ws_url = ws_url
 
     def run(
@@ -1723,14 +1719,70 @@
             "asset": asset,
             "symbol": symbol,
             "format": format,
             "limit": limit,
         }
         return CatalogMarketContractPrices(self._get_data("catalog-all/market-contract-prices", params)['data'])
 
+    def catalog_full_contract_prices_v2(
+            self,
+            markets: Optional[Union[str, List[str]]] = None,
+            exchange: Optional[str] = None,
+            market_type: Optional[str] = None,
+            base: Optional[str] = None,
+            quote: Optional[str] = None,
+            asset: Optional[str] = None,
+            symbol: Optional[str] = None,
+            format: Optional[str] = None,
+            page_size: Optional[int] = None,
+            paging_from: Optional[str] = None,
+            next_page_token: Optional[str] = None,
+    ) -> CatalogV2DataCollection:
+        """
+        :param markets: Comma separated list of markets. By default all markets are returned.
+        :type markets: Optional[Union[str, List[str]]]
+        :param exchange: Unique name of an exchange.
+        :type exchange: Optional[str]
+        :param market_type: Type of markets.
+        :type market_type: Optional[str]
+        :param base: Base asset of markets.
+        :type base: Optional[str]
+        :param quote: Quote asset of markets.
+        :type quote: Optional[str]
+        :param asset: Any asset of markets.
+        :type asset: Optional[str]
+        :param symbol: Symbol of derivative markets, full instrument name.
+        :type symbol: Optional[str]
+        :param format: Format of the response. Supported values are `json`, `json_stream`.
+        :type format: Optional[str]
+        :param page_size: Number of items per single page of results.
+        :type page_size: Optional[int]
+        :param paging_from: Where does the first page start, at the start of the interval or at the end.
+        :type paging_from: Optional[str]
+        :param next_page_token: Token for receiving the results from the next page of a query. Should not be used directly. To iterate through pages just use `next_page_url` response field.
+        :type next_page_token: Optional[str]
+
+        :return: List of contract prices statistics.
+        :rtype: CatalogV2DataCollection
+        """
+        params: Dict[str, Any] = {
+            "markets": markets,
+            "exchange": exchange,
+            "type": market_type,
+            "base": base,
+            "quote": quote,
+            "asset": asset,
+            "symbol": symbol,
+            "format": format,
+            "page_size": page_size,
+            "paging_from": paging_from,
+            "next_page_token": next_page_token,
+        }
+        return CatalogV2DataCollection(self._get_data, "/catalog-all-v2/market-contract-prices", params)
+
     def catalog_full_market_implied_volatility(
             self,
             markets: Optional[Union[str, List[str]]] = None,
             exchange: Optional[str] = None,
             type: Optional[str] = None,
             base: Optional[str] = None,
             quote: Optional[str] = None,
@@ -1900,14 +1952,1246 @@
             "asset": asset,
             "symbol": symbol,
         }
         return CatalogMarketTradesData(
             self._get_data("catalog-all/market-liquidations", params)["data"]
         )
 
+    def catalog_market_trades_v2(
+            self,
+            markets: Optional[Union[str, List[str]]] = None,
+            exchange: Optional[str] = None,
+            market_type: Optional[str] = None,
+            base: Optional[str] = None,
+            quote: Optional[str] = None,
+            asset: Optional[str] = None,
+            symbol: Optional[str] = None,
+            format: Optional[str] = None,
+            page_size: Optional[int] = None,
+            paging_from: Optional[str] = None,
+            next_page_token: Optional[str] = None,
+    ) -> CatalogV2DataCollection:
+        """
+        :param markets: Comma separated list of markets. By default all markets are returned.
+        :type markets: Optional[Union[str, List[str]]]
+        :param exchange: Unique name of an exchange.
+        :type exchange: Optional[str]
+        :param market_type: Type of markets.
+        :type market_type: Optional[str]
+        :param base: Base asset of markets.
+        :type base: Optional[str]
+        :param quote: Quote asset of markets.
+        :type quote: Optional[str]
+        :param asset: Any asset of markets.
+        :type asset: Optional[str]
+        :param symbol: Symbol of derivative markets, full instrument name.
+        :type symbol: Optional[str]
+        :param format: Format of the response. Supported values are `json`, `json_stream`.
+        :type format: Optional[str]
+        :param page_size: Number of items per single page of results.
+        :type page_size: Optional[int]
+        :param paging_from: Where does the first page start, at the start of the interval or at the end.
+        :type paging_from: Optional[str]
+        :param next_page_token: Token for receiving the results from the next page of a query. Should not be used directly. To iterate through pages just use `next_page_url` response field.
+        :type next_page_token: Optional[str]
+
+        :return: List of market trades statistics.
+        :rtype: CatalogV2DataCollection
+        """
+        params: Dict[str, Any] = {
+            "markets": markets,
+            "exchange": exchange,
+            "type": market_type,
+            "base": base,
+            "quote": quote,
+            "asset": asset,
+            "symbol": symbol,
+            "format": format,
+            "page_size": page_size,
+            "paging_from": paging_from,
+            "next_page_token": next_page_token,
+        }
+        return CatalogV2DataCollection(self._get_data, "/catalog-v2/market-trades", params)
+
+    def catalog_market_candles_v2(
+            self,
+            markets: Optional[Union[str, List[str]]] = None,
+            exchange: Optional[str] = None,
+            market_type: Optional[str] = None,
+            base: Optional[str] = None,
+            quote: Optional[str] = None,
+            asset: Optional[str] = None,
+            symbol: Optional[str] = None,
+            format: Optional[str] = None,
+            page_size: Optional[int] = None,
+            paging_from: Optional[str] = None,
+            next_page_token: Optional[str] = None,
+    ) -> CatalogV2DataCollection:
+        """
+        :param markets: Comma separated list of markets. By default all markets are returned.
+        :type markets: Optional[Union[str, List[str]]]
+        :param exchange: Unique name of an exchange.
+        :type exchange: Optional[str]
+        :param market_type: Type of markets.
+        :type market_type: Optional[str]
+        :param base: Base asset of markets.
+        :type base: Optional[str]
+        :param quote: Quote asset of markets.
+        :type quote: Optional[str]
+        :param asset: Any asset of markets.
+        :type asset: Optional[str]
+        :param symbol: Symbol of derivative markets, full instrument name.
+        :type symbol: Optional[str]
+        :param format: Format of the response. Supported values are `json`, `json_stream`.
+        :type format: Optional[str]
+        :param page_size: Number of items per single page of results.
+        :type page_size: Optional[int]
+        :param paging_from: Where does the first page start, at the start of the interval or at the end.
+        :type paging_from: Optional[str]
+        :param next_page_token: Token for receiving the results from the next page of a query. Should not be used directly. To iterate through pages just use `next_page_url` response field.
+        :type next_page_token: Optional[str]
+
+        :return: List of market candles statistics.
+        :rtype: CatalogV2DataCollection
+        """
+        params: Dict[str, Any] = {
+            "markets": markets,
+            "exchange": exchange,
+            "type": market_type,
+            "base": base,
+            "quote": quote,
+            "asset": asset,
+            "symbol": symbol,
+            "format": format,
+            "page_size": page_size,
+            "paging_from": paging_from,
+            "next_page_token": next_page_token,
+        }
+        return CatalogV2DataCollection(self._get_data, "/catalog-v2/market-candles", params)
+
+    def catalog_market_orderbooks_v2(
+            self,
+            markets: Optional[Union[str, List[str]]] = None,
+            exchange: Optional[str] = None,
+            market_type: Optional[str] = None,
+            base: Optional[str] = None,
+            quote: Optional[str] = None,
+            asset: Optional[str] = None,
+            symbol: Optional[str] = None,
+            format: Optional[str] = None,
+            page_size: Optional[int] = None,
+            paging_from: Optional[str] = None,
+            next_page_token: Optional[str] = None,
+    ) -> CatalogV2DataCollection:
+        """
+        :param markets: Comma separated list of markets. By default all markets are returned.
+        :type markets: Optional[Union[str, List[str]]]
+        :param exchange: Unique name of an exchange.
+        :type exchange: Optional[str]
+        :param market_type: Type of markets.
+        :type market_type: Optional[str]
+        :param base: Base asset of markets.
+        :type base: Optional[str]
+        :param quote: Quote asset of markets.
+        :type quote: Optional[str]
+        :param asset: Any asset of markets.
+        :type asset: Optional[str]
+        :param symbol: Symbol of derivative markets, full instrument name.
+        :type symbol: Optional[str]
+        :param format: Format of the response. Supported values are `json`, `json_stream`.
+        :type format: Optional[str]
+        :param page_size: Number of items per single page of results.
+        :type page_size: Optional[int]
+        :param paging_from: Where does the first page start, at the start of the interval or at the end.
+        :type paging_from: Optional[str]
+        :param next_page_token: Token for receiving the results from the next page of a query. Should not be used directly. To iterate through pages just use `next_page_url` response field.
+        :type next_page_token: Optional[str]
+
+        :return: List of market orderbooks statistics.
+        :rtype: CatalogV2DataCollection
+        """
+        params: Dict[str, Any] = {
+            "markets": markets,
+            "exchange": exchange,
+            "type": market_type,
+            "base": base,
+            "quote": quote,
+            "asset": asset,
+            "symbol": symbol,
+            "format": format,
+            "page_size": page_size,
+            "paging_from": paging_from,
+            "next_page_token": next_page_token,
+        }
+        return CatalogV2DataCollection(self._get_data, "/catalog-v2/market-orderbooks", params)
+
+    def catalog_market_quotes_v2(
+            self,
+            markets: Optional[Union[str, List[str]]] = None,
+            exchange: Optional[str] = None,
+            market_type: Optional[str] = None,
+            base: Optional[str] = None,
+            quote: Optional[str] = None,
+            asset: Optional[str] = None,
+            symbol: Optional[str] = None,
+            format: Optional[str] = None,
+            page_size: Optional[int] = None,
+            paging_from: Optional[str] = None,
+            next_page_token: Optional[str] = None,
+    ) -> CatalogV2DataCollection:
+        """
+        :param markets: Comma separated list of markets. By default all markets are returned.
+        :type markets: Optional[Union[str, List[str]]]
+        :param exchange: Unique name of an exchange.
+        :type exchange: Optional[str]
+        :param market_type: Type of markets.
+        :type market_type: Optional[str]
+        :param base: Base asset of markets.
+        :type base: Optional[str]
+        :param quote: Quote asset of markets.
+        :type quote: Optional[str]
+        :param asset: Any asset of markets.
+        :type asset: Optional[str]
+        :param symbol: Symbol of derivative markets, full instrument name.
+        :type symbol: Optional[str]
+        :param format: Format of the response. Supported values are `json`, `json_stream`.
+        :type format: Optional[str]
+        :param page_size: Number of items per single page of results.
+        :type page_size: Optional[int]
+        :param paging_from: Where does the first page start, at the start of the interval or at the end.
+        :type paging_from: Optional[str]
+        :param next_page_token: Token for receiving the results from the next page of a query. Should not be used directly. To iterate through pages just use `next_page_url` response field.
+        :type next_page_token: Optional[str]
+
+        :return: List of market quotes statistics.
+        :rtype: CatalogV2DataCollection
+        """
+        params: Dict[str, Any] = {
+            "markets": markets,
+            "exchange": exchange,
+            "type": market_type,
+            "base": base,
+            "quote": quote,
+            "asset": asset,
+            "symbol": symbol,
+            "format": format,
+            "page_size": page_size,
+            "paging_from": paging_from,
+            "next_page_token": next_page_token,
+        }
+        return CatalogV2DataCollection(self._get_data, "/catalog-v2/market-quotes", params)
+
+    def catalog_market_funding_rates_v2(
+            self,
+            markets: Optional[Union[str, List[str]]] = None,
+            exchange: Optional[str] = None,
+            market_type: Optional[str] = None,
+            base: Optional[str] = None,
+            quote: Optional[str] = None,
+            asset: Optional[str] = None,
+            symbol: Optional[str] = None,
+            format: Optional[str] = None,
+            page_size: Optional[int] = None,
+            paging_from: Optional[str] = None,
+            next_page_token: Optional[str] = None,
+    ) -> CatalogV2DataCollection:
+        """
+        :param markets: Comma separated list of markets. By default all markets are returned.
+        :type markets: Optional[Union[str, List[str]]]
+        :param exchange: Unique name of an exchange.
+        :type exchange: Optional[str]
+        :param market_type: Type of markets.
+        :type market_type: Optional[str]
+        :param base: Base asset of markets.
+        :type base: Optional[str]
+        :param quote: Quote asset of markets.
+        :type quote: Optional[str]
+        :param asset: Any asset of markets.
+        :type asset: Optional[str]
+        :param symbol: Symbol of derivative markets, full instrument name.
+        :type symbol: Optional[str]
+        :param format: Format of the response. Supported values are `json`, `json_stream`.
+        :type format: Optional[str]
+        :param page_size: Number of items per single page of results.
+        :type page_size: Optional[int]
+        :param paging_from: Where does the first page start, at the start of the interval or at the end.
+        :type paging_from: Optional[str]
+        :param next_page_token: Token for receiving the results from the next page of a query. Should not be used directly. To iterate through pages just use `next_page_url` response field.
+        :type next_page_token: Optional[str]
+
+        :return: List of market funding rates statistics.
+        :rtype: CatalogV2DataCollection
+        """
+        params: Dict[str, Any] = {
+            "markets": markets,
+            "exchange": exchange,
+            "type": market_type,
+            "base": base,
+            "quote": quote,
+            "asset": asset,
+            "symbol": symbol,
+            "format": format,
+            "page_size": page_size,
+            "paging_from": paging_from,
+            "next_page_token": next_page_token,
+        }
+        return CatalogV2DataCollection(self._get_data, "/catalog-v2/market-funding-rates", params)
+
+    def catalog_market_contract_prices_v2(
+            self,
+            markets: Optional[Union[str, List[str]]] = None,
+            exchange: Optional[str] = None,
+            market_type: Optional[str] = None,
+            base: Optional[str] = None,
+            quote: Optional[str] = None,
+            asset: Optional[str] = None,
+            symbol: Optional[str] = None,
+            format: Optional[str] = None,
+            page_size: Optional[int] = None,
+            paging_from: Optional[str] = None,
+            next_page_token: Optional[str] = None,
+    ) -> CatalogV2DataCollection:
+        """
+        :param markets: Comma separated list of markets. By default all markets are returned.
+        :type markets: Optional[Union[str, List[str]]]
+        :param exchange: Unique name of an exchange.
+        :type exchange: Optional[str]
+        :param market_type: Type of markets.
+        :type market_type: Optional[str]
+        :param base: Base asset of markets.
+        :type base: Optional[str]
+        :param quote: Quote asset of markets.
+        :type quote: Optional[str]
+        :param asset: Any asset of markets.
+        :type asset: Optional[str]
+        :param symbol: Symbol of derivative markets, full instrument name.
+        :type symbol: Optional[str]
+        :param format: Format of the response. Supported values are `json`, `json_stream`.
+        :type format: Optional[str]
+        :param page_size: Number of items per single page of results.
+        :type page_size: Optional[int]
+        :param paging_from: Where does the first page start, at the start of the interval or at the end.
+        :type paging_from: Optional[str]
+        :param next_page_token: Token for receiving the results from the next page of a query. Should not be used directly. To iterate through pages just use `next_page_url` response field.
+        :type next_page_token: Optional[str]
+
+        :return: List of contract prices statistics.
+        :rtype: CatalogV2DataCollection
+        """
+        params: Dict[str, Any] = {
+            "markets": markets,
+            "exchange": exchange,
+            "type": market_type,
+            "base": base,
+            "quote": quote,
+            "asset": asset,
+            "symbol": symbol,
+            "format": format,
+            "page_size": page_size,
+            "paging_from": paging_from,
+            "next_page_token": next_page_token,
+        }
+        return CatalogV2DataCollection(self._get_data, "/catalog-v2/market-contract-prices", params)
+
+    def catalog_market_implied_volatility_v2(
+            self,
+            markets: Optional[Union[str, List[str]]] = None,
+            exchange: Optional[str] = None,
+            market_type: Optional[str] = None,
+            base: Optional[str] = None,
+            quote: Optional[str] = None,
+            asset: Optional[str] = None,
+            symbol: Optional[str] = None,
+            format: Optional[str] = None,
+            page_size: Optional[int] = None,
+            paging_from: Optional[str] = None,
+            next_page_token: Optional[str] = None,
+    ) -> CatalogV2DataCollection:
+        """
+        :param markets: Comma separated list of markets. By default all markets are returned.
+        :type markets: Optional[Union[str, List[str]]]
+        :param exchange: Unique name of an exchange.
+        :type exchange: Optional[str]
+        :param market_type: Type of markets.
+        :type market_type: Optional[str]
+        :param base: Base asset of markets.
+        :type base: Optional[str]
+        :param quote: Quote asset of markets.
+        :type quote: Optional[str]
+        :param asset: Any asset of markets.
+        :type asset: Optional[str]
+        :param symbol: Symbol of derivative markets, full instrument name.
+        :type symbol: Optional[str]
+        :param format: Format of the response. Supported values are `json`, `json_stream`.
+        :type format: Optional[str]
+        :param page_size: Number of items per single page of results.
+        :type page_size: Optional[int]
+        :param paging_from: Where does the first page start, at the start of the interval or at the end.
+        :type paging_from: Optional[str]
+        :param next_page_token: Token for receiving the results from the next page of a query. Should not be used directly. To iterate through pages just use `next_page_url` response field.
+        :type next_page_token: Optional[str]
+
+        :return: List of implied volatility statistics.
+        :rtype: CatalogV2DataCollection
+        """
+        params: Dict[str, Any] = {
+            "markets": markets,
+            "exchange": exchange,
+            "type": market_type,
+            "base": base,
+            "quote": quote,
+            "asset": asset,
+            "symbol": symbol,
+            "format": format,
+            "page_size": page_size,
+            "paging_from": paging_from,
+            "next_page_token": next_page_token,
+        }
+        return CatalogV2DataCollection(self._get_data, "/catalog-v2/market-implied-volatility", params)
+
+    def catalog_market_greeks_v2(
+            self,
+            markets: Optional[Union[str, List[str]]] = None,
+            exchange: Optional[str] = None,
+            market_type: Optional[str] = None,
+            base: Optional[str] = None,
+            quote: Optional[str] = None,
+            asset: Optional[str] = None,
+            symbol: Optional[str] = None,
+            format: Optional[str] = None,
+            page_size: Optional[int] = None,
+            paging_from: Optional[str] = None,
+            next_page_token: Optional[str] = None,
+    ) -> CatalogV2DataCollection:
+        """
+        :param markets: Comma separated list of markets. By default all markets are returned.
+        :type markets: Optional[Union[str, List[str]]]
+        :param exchange: Unique name of an exchange.
+        :type exchange: Optional[str]
+        :param market_type: Type of markets.
+        :type market_type: Optional[str]
+        :param base: Base asset of markets.
+        :type base: Optional[str]
+        :param quote: Quote asset of markets.
+        :type quote: Optional[str]
+        :param asset: Any asset of markets.
+        :type asset: Optional[str]
+        :param symbol: Symbol of derivative markets, full instrument name.
+        :type symbol: Optional[str]
+        :param format: Format of the response. Supported values are `json`, `json_stream`.
+        :type format: Optional[str]
+        :param page_size: Number of items per single page of results.
+        :type page_size: Optional[int]
+        :param paging_from: Where does the first page start, at the start of the interval or at the end.
+        :type paging_from: Optional[str]
+        :param next_page_token: Token for receiving the results from the next page of a query. Should not be used directly. To iterate through pages just use `next_page_url` response field.
+        :type next_page_token: Optional[str]
+
+        :return: List of greeks statistics.
+        :rtype: CatalogV2DataCollection
+        """
+        params: Dict[str, Any] = {
+            "markets": markets,
+            "exchange": exchange,
+            "type": market_type,
+            "base": base,
+            "quote": quote,
+            "asset": asset,
+            "symbol": symbol,
+            "format": format,
+            "page_size": page_size,
+            "paging_from": paging_from,
+            "next_page_token": next_page_token,
+        }
+        return CatalogV2DataCollection(self._get_data, "/catalog-v2/market-greeks", params)
+
+    def catalog_market_open_interest_v2(
+            self,
+            markets: Optional[Union[str, List[str]]] = None,
+            exchange: Optional[str] = None,
+            market_type: Optional[str] = None,
+            base: Optional[str] = None,
+            quote: Optional[str] = None,
+            asset: Optional[str] = None,
+            symbol: Optional[str] = None,
+            format: Optional[str] = None,
+            page_size: Optional[int] = None,
+            paging_from: Optional[str] = None,
+            next_page_token: Optional[str] = None,
+    ) -> CatalogV2DataCollection:
+        """
+        :param markets: Comma separated list of markets. By default all markets are returned.
+        :type markets: Optional[Union[str, List[str]]]
+        :param exchange: Unique name of an exchange.
+        :type exchange: Optional[str]
+        :param market_type: Type of markets.
+        :type market_type: Optional[str]
+        :param base: Base asset of markets.
+        :type base: Optional[str]
+        :param quote: Quote asset of markets.
+        :type quote: Optional[str]
+        :param asset: Any asset of markets.
+        :type asset: Optional[str]
+        :param symbol: Symbol of derivative markets, full instrument name.
+        :type symbol: Optional[str]
+        :param format: Format of the response. Supported values are `json`, `json_stream`.
+        :type format: Optional[str]
+        :param page_size: Number of items per single page of results.
+        :type page_size: Optional[int]
+        :param paging_from: Where does the first page start, at the start of the interval or at the end.
+        :type paging_from: Optional[str]
+        :param next_page_token: Token for receiving the results from the next page of a query. Should not be used directly. To iterate through pages just use `next_page_url` response field.
+        :type next_page_token: Optional[str]
+
+        :return: List of market open interest statistics.
+        :rtype: CatalogV2DataCollection
+        """
+        params: Dict[str, Any] = {
+            "markets": markets,
+            "exchange": exchange,
+            "type": market_type,
+            "base": base,
+            "quote": quote,
+            "asset": asset,
+            "symbol": symbol,
+            "format": format,
+            "page_size": page_size,
+            "paging_from": paging_from,
+            "next_page_token": next_page_token,
+        }
+        return CatalogV2DataCollection(self._get_data, "/catalog-v2/market-openinterest", params)
+
+    def catalog_market_liquidations_v2(
+            self,
+            markets: Optional[Union[str, List[str]]] = None,
+            exchange: Optional[str] = None,
+            market_type: Optional[str] = None,
+            base: Optional[str] = None,
+            quote: Optional[str] = None,
+            asset: Optional[str] = None,
+            symbol: Optional[str] = None,
+            format: Optional[str] = None,
+            page_size: Optional[int] = None,
+            paging_from: Optional[str] = None,
+            next_page_token: Optional[str] = None,
+    ) -> CatalogV2DataCollection:
+        """
+        :param markets: Comma separated list of markets. By default all markets are returned.
+        :type markets: Optional[Union[str, List[str]]]
+        :param exchange: Unique name of an exchange.
+        :type exchange: Optional[str]
+        :param market_type: Type of markets.
+        :type market_type: Optional[str]
+        :param base: Base asset of markets.
+        :type base: Optional[str]
+        :param quote: Quote asset of markets.
+        :type quote: Optional[str]
+        :param asset: Any asset of markets.
+        :type asset: Optional[str]
+        :param symbol: Symbol of derivative markets, full instrument name.
+        :type symbol: Optional[str]
+        :param format: Format of the response. Supported values are `json`, `json_stream`.
+        :type format: Optional[str]
+        :param page_size: Number of items per single page of results.
+        :type page_size: Optional[int]
+        :param paging_from: Where does the first page start, at the start of the interval or at the end.
+        :type paging_from: Optional[str]
+        :param next_page_token: Token for receiving the results from the next page of a query. Should not be used directly. To iterate through pages just use `next_page_url` response field.
+        :type next_page_token: Optional[str]
+
+        :return: List of market liquidations statistics.
+        :rtype: CatalogV2DataCollection
+        """
+        params: Dict[str, Any] = {
+            "markets": markets,
+            "exchange": exchange,
+            "type": market_type,
+            "base": base,
+            "quote": quote,
+            "asset": asset,
+            "symbol": symbol,
+            "format": format,
+            "page_size": page_size,
+            "paging_from": paging_from,
+            "next_page_token": next_page_token,
+        }
+        return CatalogV2DataCollection(self._get_data, "/catalog-v2/market-liquidations", params)
+
+    def catalog_market_metrics_v2(
+            self,
+            markets: Optional[Union[str, List[str]]] = None,
+            exchange: Optional[str] = None,
+            market_type: Optional[str] = None,
+            base: Optional[str] = None,
+            quote: Optional[str] = None,
+            asset: Optional[str] = None,
+            symbol: Optional[str] = None,
+            format: Optional[str] = None,
+            page_size: Optional[int] = None,
+            paging_from: Optional[str] = None,
+            next_page_token: Optional[str] = None,
+    ) -> CatalogV2DataCollection:
+        """
+        :param markets: Comma separated list of markets. By default all markets are returned.
+        :type markets: Optional[Union[str, List[str]]]
+        :param exchange: Unique name of an exchange.
+        :type exchange: Optional[str]
+        :param market_type: Type of markets.
+        :type market_type: Optional[str]
+        :param base: Base asset of markets.
+        :type base: Optional[str]
+        :param quote: Quote asset of markets.
+        :type quote: Optional[str]
+        :param asset: Any asset of markets.
+        :type asset: Optional[str]
+        :param symbol: Symbol of derivative markets, full instrument name.
+        :type symbol: Optional[str]
+        :param format: Format of the response. Supported values are `json`, `json_stream`.
+        :type format: Optional[str]
+        :param page_size: Number of items per single page of results.
+        :type page_size: Optional[int]
+        :param paging_from: Where does the first page start, at the start of the interval or at the end.
+        :type paging_from: Optional[str]
+        :param next_page_token: Token for receiving the results from the next page of a query. Should not be used directly. To iterate through pages just use `next_page_url` response field.
+        :type next_page_token: Optional[str]
+
+        :return: List of market metrics statistics.
+        :rtype: CatalogV2DataCollection
+        """
+        params: Dict[str, Any] = {
+            "markets": markets,
+            "exchange": exchange,
+            "type": market_type,
+            "base": base,
+            "quote": quote,
+            "asset": asset,
+            "symbol": symbol,
+            "format": format,
+            "page_size": page_size,
+            "paging_from": paging_from,
+            "next_page_token": next_page_token,
+        }
+        return CatalogV2DataCollection(self._get_data, "/catalog-v2/market-metrics", params)
+
+    def catalog_full_market_trades_v2(
+            self,
+            markets: Optional[Union[str, List[str]]] = None,
+            exchange: Optional[str] = None,
+            market_type: Optional[str] = None,
+            base: Optional[str] = None,
+            quote: Optional[str] = None,
+            asset: Optional[str] = None,
+            symbol: Optional[str] = None,
+            format: Optional[str] = None,
+            page_size: Optional[int] = None,
+            paging_from: Optional[str] = None,
+            next_page_token: Optional[str] = None,
+    ) -> CatalogV2DataCollection:
+        """
+        :param markets: Comma separated list of markets. By default all markets are returned.
+        :type markets: Optional[Union[str, List[str]]]
+        :param exchange: Unique name of an exchange.
+        :type exchange: Optional[str]
+        :param market_type: Type of markets.
+        :type market_type: Optional[str]
+        :param base: Base asset of markets.
+        :type base: Optional[str]
+        :param quote: Quote asset of markets.
+        :type quote: Optional[str]
+        :param asset: Any asset of markets.
+        :type asset: Optional[str]
+        :param symbol: Symbol of derivative markets, full instrument name.
+        :type symbol: Optional[str]
+        :param format: Format of the response. Supported values are `json`, `json_stream`.
+        :type format: Optional[str]
+        :param page_size: Number of items per single page of results.
+        :type page_size: Optional[int]
+        :param paging_from: Where does the first page start, at the start of the interval or at the end.
+        :type paging_from: Optional[str]
+        :param next_page_token: Token for receiving the results from the next page of a query. Should not be used directly. To iterate through pages just use `next_page_url` response field.
+        :type next_page_token: Optional[str]
+
+        :return: List of market trades statistics.
+        :rtype: CatalogV2DataCollection
+        """
+        params: Dict[str, Any] = {
+            "markets": markets,
+            "exchange": exchange,
+            "type": market_type,
+            "base": base,
+            "quote": quote,
+            "asset": asset,
+            "symbol": symbol,
+            "format": format,
+            "page_size": page_size,
+            "paging_from": paging_from,
+            "next_page_token": next_page_token,
+        }
+        return CatalogV2DataCollection(self._get_data, "/catalog-all-v2/market-trades", params)
+
+    def catalog_full_market_candles_v2(
+            self,
+            markets: Optional[Union[str, List[str]]] = None,
+            exchange: Optional[str] = None,
+            market_type: Optional[str] = None,
+            base: Optional[str] = None,
+            quote: Optional[str] = None,
+            asset: Optional[str] = None,
+            symbol: Optional[str] = None,
+            format: Optional[str] = None,
+            page_size: Optional[int] = None,
+            paging_from: Optional[str] = None,
+            next_page_token: Optional[str] = None,
+    ) -> CatalogV2DataCollection:
+        """
+        :param markets: Comma separated list of markets. By default all markets are returned.
+        :type markets: Optional[Union[str, List[str]]]
+        :param exchange: Unique name of an exchange.
+        :type exchange: Optional[str]
+        :param market_type: Type of markets.
+        :type market_type: Optional[str]
+        :param base: Base asset of markets.
+        :type base: Optional[str]
+        :param quote: Quote asset of markets.
+        :type quote: Optional[str]
+        :param asset: Any asset of markets.
+        :type asset: Optional[str]
+        :param symbol: Symbol of derivative markets, full instrument name.
+        :type symbol: Optional[str]
+        :param format: Format of the response. Supported values are `json`, `json_stream`.
+        :type format: Optional[str]
+        :param page_size: Number of items per single page of results.
+        :type page_size: Optional[int]
+        :param paging_from: Where does the first page start, at the start of the interval or at the end.
+        :type paging_from: Optional[str]
+        :param next_page_token: Token for receiving the results from the next page of a query. Should not be used directly. To iterate through pages just use `next_page_url` response field.
+        :type next_page_token: Optional[str]
+
+        :return: List of market candles statistics.
+        :rtype: CatalogV2DataCollection
+        """
+        params: Dict[str, Any] = {
+            "markets": markets,
+            "exchange": exchange,
+            "type": market_type,
+            "base": base,
+            "quote": quote,
+            "asset": asset,
+            "symbol": symbol,
+            "format": format,
+            "page_size": page_size,
+            "paging_from": paging_from,
+            "next_page_token": next_page_token,
+        }
+        return CatalogV2DataCollection(self._get_data, "/catalog-all-v2/market-candles", params)
+
+    def catalog_full_market_orderbooks_v2(
+            self,
+            markets: Optional[Union[str, List[str]]] = None,
+            exchange: Optional[str] = None,
+            market_type: Optional[str] = None,
+            base: Optional[str] = None,
+            quote: Optional[str] = None,
+            asset: Optional[str] = None,
+            symbol: Optional[str] = None,
+            format: Optional[str] = None,
+            page_size: Optional[int] = None,
+            paging_from: Optional[str] = None,
+            next_page_token: Optional[str] = None,
+    ) -> CatalogV2DataCollection:
+        """
+        :param markets: Comma separated list of markets. By default all markets are returned.
+        :type markets: Optional[Union[str, List[str]]]
+        :param exchange: Unique name of an exchange.
+        :type exchange: Optional[str]
+        :param market_type: Type of markets.
+        :type market_type: Optional[str]
+        :param base: Base asset of markets.
+        :type base: Optional[str]
+        :param quote: Quote asset of markets.
+        :type quote: Optional[str]
+        :param asset: Any asset of markets.
+        :type asset: Optional[str]
+        :param symbol: Symbol of derivative markets, full instrument name.
+        :type symbol: Optional[str]
+        :param format: Format of the response. Supported values are `json`, `json_stream`.
+        :type format: Optional[str]
+        :param page_size: Number of items per single page of results.
+        :type page_size: Optional[int]
+        :param paging_from: Where does the first page start, at the start of the interval or at the end.
+        :type paging_from: Optional[str]
+        :param next_page_token: Token for receiving the results from the next page of a query. Should not be used directly. To iterate through pages just use `next_page_url` response field.
+        :type next_page_token: Optional[str]
+
+        :return: List of market orderbooks statistics.
+        :rtype: CatalogV2DataCollection
+        """
+        params: Dict[str, Any] = {
+            "markets": markets,
+            "exchange": exchange,
+            "type": market_type,
+            "base": base,
+            "quote": quote,
+            "asset": asset,
+            "symbol": symbol,
+            "format": format,
+            "page_size": page_size,
+            "paging_from": paging_from,
+            "next_page_token": next_page_token,
+        }
+        return CatalogV2DataCollection(self._get_data, "/catalog-all-v2/market-orderbooks", params)
+
+    def catalog_full_market_quotes_v2(
+            self,
+            markets: Optional[Union[str, List[str]]] = None,
+            exchange: Optional[str] = None,
+            market_type: Optional[str] = None,
+            base: Optional[str] = None,
+            quote: Optional[str] = None,
+            asset: Optional[str] = None,
+            symbol: Optional[str] = None,
+            format: Optional[str] = None,
+            page_size: Optional[int] = None,
+            paging_from: Optional[str] = None,
+            next_page_token: Optional[str] = None,
+    ) -> CatalogV2DataCollection:
+        """
+        :param markets: Comma separated list of markets. By default all markets are returned.
+        :type markets: Optional[Union[str, List[str]]]
+        :param exchange: Unique name of an exchange.
+        :type exchange: Optional[str]
+        :param market_type: Type of markets.
+        :type market_type: Optional[str]
+        :param base: Base asset of markets.
+        :type base: Optional[str]
+        :param quote: Quote asset of markets.
+        :type quote: Optional[str]
+        :param asset: Any asset of markets.
+        :type asset: Optional[str]
+        :param symbol: Symbol of derivative markets, full instrument name.
+        :type symbol: Optional[str]
+        :param format: Format of the response. Supported values are `json`, `json_stream`.
+        :type format: Optional[str]
+        :param page_size: Number of items per single page of results.
+        :type page_size: Optional[int]
+        :param paging_from: Where does the first page start, at the start of the interval or at the end.
+        :type paging_from: Optional[str]
+        :param next_page_token: Token for receiving the results from the next page of a query. Should not be used directly. To iterate through pages just use `next_page_url` response field.
+        :type next_page_token: Optional[str]
+
+        :return: List of market quotes statistics.
+        :rtype: CatalogV2DataCollection
+        """
+        params: Dict[str, Any] = {
+            "markets": markets,
+            "exchange": exchange,
+            "type": market_type,
+            "base": base,
+            "quote": quote,
+            "asset": asset,
+            "symbol": symbol,
+            "format": format,
+            "page_size": page_size,
+            "paging_from": paging_from,
+            "next_page_token": next_page_token,
+        }
+        return CatalogV2DataCollection(self._get_data, "/catalog-all-v2/market-quotes", params)
+
+    def catalog_full_market_funding_rates_v2(
+            self,
+            markets: Optional[Union[str, List[str]]] = None,
+            exchange: Optional[str] = None,
+            market_type: Optional[str] = None,
+            base: Optional[str] = None,
+            quote: Optional[str] = None,
+            asset: Optional[str] = None,
+            symbol: Optional[str] = None,
+            format: Optional[str] = None,
+            page_size: Optional[int] = None,
+            paging_from: Optional[str] = None,
+            next_page_token: Optional[str] = None,
+    ) -> CatalogV2DataCollection:
+        """
+        :param markets: Comma separated list of markets. By default all markets are returned.
+        :type markets: Optional[Union[str, List[str]]]
+        :param exchange: Unique name of an exchange.
+        :type exchange: Optional[str]
+        :param market_type: Type of markets.
+        :type market_type: Optional[str]
+        :param base: Base asset of markets.
+        :type base: Optional[str]
+        :param quote: Quote asset of markets.
+        :type quote: Optional[str]
+        :param asset: Any asset of markets.
+        :type asset: Optional[str]
+        :param symbol: Symbol of derivative markets, full instrument name.
+        :type symbol: Optional[str]
+        :param format: Format of the response. Supported values are `json`, `json_stream`.
+        :type format: Optional[str]
+        :param page_size: Number of items per single page of results.
+        :type page_size: Optional[int]
+        :param paging_from: Where does the first page start, at the start of the interval or at the end.
+        :type paging_from: Optional[str]
+        :param next_page_token: Token for receiving the results from the next page of a query. Should not be used directly. To iterate through pages just use `next_page_url` response field.
+        :type next_page_token: Optional[str]
+
+        :return: List of market funding rates statistics.
+        :rtype: CatalogV2DataCollection
+        """
+        params: Dict[str, Any] = {
+            "markets": markets,
+            "exchange": exchange,
+            "type": market_type,
+            "base": base,
+            "quote": quote,
+            "asset": asset,
+            "symbol": symbol,
+            "format": format,
+            "page_size": page_size,
+            "paging_from": paging_from,
+            "next_page_token": next_page_token,
+        }
+        return CatalogV2DataCollection(self._get_data, "/catalog-all-v2/market-funding-rates", params)
+
+    def catalog_full_market_contract_prices_v2(
+            self,
+            markets: Optional[Union[str, List[str]]] = None,
+            exchange: Optional[str] = None,
+            market_type: Optional[str] = None,
+            base: Optional[str] = None,
+            quote: Optional[str] = None,
+            asset: Optional[str] = None,
+            symbol: Optional[str] = None,
+            format: Optional[str] = None,
+            page_size: Optional[int] = None,
+            paging_from: Optional[str] = None,
+            next_page_token: Optional[str] = None,
+    ) -> CatalogV2DataCollection:
+        """
+        :param markets: Comma separated list of markets. By default all markets are returned.
+        :type markets: Optional[Union[str, List[str]]]
+        :param exchange: Unique name of an exchange.
+        :type exchange: Optional[str]
+        :param market_type: Type of markets.
+        :type market_type: Optional[str]
+        :param base: Base asset of markets.
+        :type base: Optional[str]
+        :param quote: Quote asset of markets.
+        :type quote: Optional[str]
+        :param asset: Any asset of markets.
+        :type asset: Optional[str]
+        :param symbol: Symbol of derivative markets, full instrument name.
+        :type symbol: Optional[str]
+        :param format: Format of the response. Supported values are `json`, `json_stream`.
+        :type format: Optional[str]
+        :param page_size: Number of items per single page of results.
+        :type page_size: Optional[int]
+        :param paging_from: Where does the first page start, at the start of the interval or at the end.
+        :type paging_from: Optional[str]
+        :param next_page_token: Token for receiving the results from the next page of a query. Should not be used directly. To iterate through pages just use `next_page_url` response field.
+        :type next_page_token: Optional[str]
+
+        :return: List of contract prices statistics.
+        :rtype: CatalogV2DataCollection
+        """
+        params: Dict[str, Any] = {
+            "markets": markets,
+            "exchange": exchange,
+            "type": market_type,
+            "base": base,
+            "quote": quote,
+            "asset": asset,
+            "symbol": symbol,
+            "format": format,
+            "page_size": page_size,
+            "paging_from": paging_from,
+            "next_page_token": next_page_token,
+        }
+        return CatalogV2DataCollection(self._get_data, "/catalog-all-v2/market-contract-prices", params)
+
+    def catalog_full_market_implied_volatility_v2(
+            self,
+            markets: Optional[Union[str, List[str]]] = None,
+            exchange: Optional[str] = None,
+            market_type: Optional[str] = None,
+            base: Optional[str] = None,
+            quote: Optional[str] = None,
+            asset: Optional[str] = None,
+            symbol: Optional[str] = None,
+            format: Optional[str] = None,
+            page_size: Optional[int] = None,
+            paging_from: Optional[str] = None,
+            next_page_token: Optional[str] = None,
+    ) -> CatalogV2DataCollection:
+        """
+        :param markets: Comma separated list of markets. By default all markets are returned.
+        :type markets: Optional[Union[str, List[str]]]
+        :param exchange: Unique name of an exchange.
+        :type exchange: Optional[str]
+        :param market_type: Type of markets.
+        :type market_type: Optional[str]
+        :param base: Base asset of markets.
+        :type base: Optional[str]
+        :param quote: Quote asset of markets.
+        :type quote: Optional[str]
+        :param asset: Any asset of markets.
+        :type asset: Optional[str]
+        :param symbol: Symbol of derivative markets, full instrument name.
+        :type symbol: Optional[str]
+        :param format: Format of the response. Supported values are `json`, `json_stream`.
+        :type format: Optional[str]
+        :param page_size: Number of items per single page of results.
+        :type page_size: Optional[int]
+        :param paging_from: Where does the first page start, at the start of the interval or at the end.
+        :type paging_from: Optional[str]
+        :param next_page_token: Token for receiving the results from the next page of a query. Should not be used directly. To iterate through pages just use `next_page_url` response field.
+        :type next_page_token: Optional[str]
+
+        :return: List of implied volatility statistics.
+        :rtype: CatalogV2DataCollection
+        """
+        params: Dict[str, Any] = {
+            "markets": markets,
+            "exchange": exchange,
+            "type": market_type,
+            "base": base,
+            "quote": quote,
+            "asset": asset,
+            "symbol": symbol,
+            "format": format,
+            "page_size": page_size,
+            "paging_from": paging_from,
+            "next_page_token": next_page_token,
+        }
+        return CatalogV2DataCollection(self._get_data, "/catalog-all-v2/market-implied-volatility", params)
+
+    def catalog_full_market_greeks_v2(
+            self,
+            markets: Optional[Union[str, List[str]]] = None,
+            exchange: Optional[str] = None,
+            market_type: Optional[str] = None,
+            base: Optional[str] = None,
+            quote: Optional[str] = None,
+            asset: Optional[str] = None,
+            symbol: Optional[str] = None,
+            format: Optional[str] = None,
+            page_size: Optional[int] = None,
+            paging_from: Optional[str] = None,
+            next_page_token: Optional[str] = None,
+    ) -> CatalogV2DataCollection:
+        """
+        :param markets: Comma separated list of markets. By default all markets are returned.
+        :type markets: Optional[Union[str, List[str]]]
+        :param exchange: Unique name of an exchange.
+        :type exchange: Optional[str]
+        :param market_type: Type of markets.
+        :type market_type: Optional[str]
+        :param base: Base asset of markets.
+        :type base: Optional[str]
+        :param quote: Quote asset of markets.
+        :type quote: Optional[str]
+        :param asset: Any asset of markets.
+        :type asset: Optional[str]
+        :param symbol: Symbol of derivative markets, full instrument name.
+        :type symbol: Optional[str]
+        :param format: Format of the response. Supported values are `json`, `json_stream`.
+        :type format: Optional[str]
+        :param page_size: Number of items per single page of results.
+        :type page_size: Optional[int]
+        :param paging_from: Where does the first page start, at the start of the interval or at the end.
+        :type paging_from: Optional[str]
+        :param next_page_token: Token for receiving the results from the next page of a query. Should not be used directly. To iterate through pages just use `next_page_url` response field.
+        :type next_page_token: Optional[str]
+
+        :return: List of greeks statistics.
+        :rtype: CatalogV2DataCollection
+        """
+        params: Dict[str, Any] = {
+            "markets": markets,
+            "exchange": exchange,
+            "type": market_type,
+            "base": base,
+            "quote": quote,
+            "asset": asset,
+            "symbol": symbol,
+            "format": format,
+            "page_size": page_size,
+            "paging_from": paging_from,
+            "next_page_token": next_page_token,
+        }
+        return CatalogV2DataCollection(self._get_data, "/catalog-all-v2/market-greeks", params)
+
+    def catalog_full_market_open_interest_v2(
+            self,
+            markets: Optional[Union[str, List[str]]] = None,
+            exchange: Optional[str] = None,
+            market_type: Optional[str] = None,
+            base: Optional[str] = None,
+            quote: Optional[str] = None,
+            asset: Optional[str] = None,
+            symbol: Optional[str] = None,
+            format: Optional[str] = None,
+            page_size: Optional[int] = None,
+            paging_from: Optional[str] = None,
+            next_page_token: Optional[str] = None,
+    ) -> CatalogV2DataCollection:
+        """
+        :param markets: Comma separated list of markets. By default all markets are returned.
+        :type markets: Optional[Union[str, List[str]]]
+        :param exchange: Unique name of an exchange.
+        :type exchange: Optional[str]
+        :param market_type: Type of markets.
+        :type market_type: Optional[str]
+        :param base: Base asset of markets.
+        :type base: Optional[str]
+        :param quote: Quote asset of markets.
+        :type quote: Optional[str]
+        :param asset: Any asset of markets.
+        :type asset: Optional[str]
+        :param symbol: Symbol of derivative markets, full instrument name.
+        :type symbol: Optional[str]
+        :param format: Format of the response. Supported values are `json`, `json_stream`.
+        :type format: Optional[str]
+        :param page_size: Number of items per single page of results.
+        :type page_size: Optional[int]
+        :param paging_from: Where does the first page start, at the start of the interval or at the end.
+        :type paging_from: Optional[str]
+        :param next_page_token: Token for receiving the results from the next page of a query. Should not be used directly. To iterate through pages just use `next_page_url` response field.
+        :type next_page_token: Optional[str]
+
+        :return: List of market open interest statistics.
+        :rtype: CatalogV2DataCollection
+        """
+        params: Dict[str, Any] = {
+            "markets": markets,
+            "exchange": exchange,
+            "type": market_type,
+            "base": base,
+            "quote": quote,
+            "asset": asset,
+            "symbol": symbol,
+            "format": format,
+            "page_size": page_size,
+            "paging_from": paging_from,
+            "next_page_token": next_page_token,
+        }
+        return CatalogV2DataCollection(self._get_data, "/catalog-all-v2/market-openinterest", params)
+
+    def catalog_full_market_liquidations_v2(
+            self,
+            markets: Optional[Union[str, List[str]]] = None,
+            exchange: Optional[str] = None,
+            market_type: Optional[str] = None,
+            base: Optional[str] = None,
+            quote: Optional[str] = None,
+            asset: Optional[str] = None,
+            symbol: Optional[str] = None,
+            format: Optional[str] = None,
+            page_size: Optional[int] = None,
+            paging_from: Optional[str] = None,
+            next_page_token: Optional[str] = None,
+    ) -> CatalogV2DataCollection:
+        """
+        :param markets: Comma separated list of markets. By default all markets are returned.
+        :type markets: Optional[Union[str, List[str]]]
+        :param exchange: Unique name of an exchange.
+        :type exchange: Optional[str]
+        :param market_type: Type of markets.
+        :type market_type: Optional[str]
+        :param base: Base asset of markets.
+        :type base: Optional[str]
+        :param quote: Quote asset of markets.
+        :type quote: Optional[str]
+        :param asset: Any asset of markets.
+        :type asset: Optional[str]
+        :param symbol: Symbol of derivative markets, full instrument name.
+        :type symbol: Optional[str]
+        :param format: Format of the response. Supported values are `json`, `json_stream`.
+        :type format: Optional[str]
+        :param page_size: Number of items per single page of results.
+        :type page_size: Optional[int]
+        :param paging_from: Where does the first page start, at the start of the interval or at the end.
+        :type paging_from: Optional[str]
+        :param next_page_token: Token for receiving the results from the next page of a query. Should not be used directly. To iterate through pages just use `next_page_url` response field.
+        :type next_page_token: Optional[str]
+
+        :return: List of market liquidations statistics.
+        :rtype: CatalogV2DataCollection
+        """
+        params: Dict[str, Any] = {
+            "markets": markets,
+            "exchange": exchange,
+            "type": market_type,
+            "base": base,
+            "quote": quote,
+            "asset": asset,
+            "symbol": symbol,
+            "format": format,
+            "page_size": page_size,
+            "paging_from": paging_from,
+            "next_page_token": next_page_token,
+        }
+        return CatalogV2DataCollection(self._get_data, "/catalog-all-v2/market-liquidations", params)
+
+    def catalog_full_market_metrics_v2(
+            self,
+            markets: Optional[Union[str, List[str]]] = None,
+            exchange: Optional[str] = None,
+            market_type: Optional[str] = None,
+            base: Optional[str] = None,
+            quote: Optional[str] = None,
+            asset: Optional[str] = None,
+            symbol: Optional[str] = None,
+            format: Optional[str] = None,
+            page_size: Optional[int] = None,
+            paging_from: Optional[str] = None,
+            next_page_token: Optional[str] = None,
+    ) -> CatalogV2DataCollection:
+        """
+        :param markets: Comma separated list of markets. By default all markets are returned.
+        :type markets: Optional[Union[str, List[str]]]
+        :param exchange: Unique name of an exchange.
+        :type exchange: Optional[str]
+        :param market_type: Type of markets.
+        :type market_type: Optional[str]
+        :param base: Base asset of markets.
+        :type base: Optional[str]
+        :param quote: Quote asset of markets.
+        :type quote: Optional[str]
+        :param asset: Any asset of markets.
+        :type asset: Optional[str]
+        :param symbol: Symbol of derivative markets, full instrument name.
+        :type symbol: Optional[str]
+        :param format: Format of the response. Supported values are `json`, `json_stream`.
+        :type format: Optional[str]
+        :param page_size: Number of items per single page of results.
+        :type page_size: Optional[int]
+        :param paging_from: Where does the first page start, at the start of the interval or at the end.
+        :type paging_from: Optional[str]
+        :param next_page_token: Token for receiving the results from the next page of a query. Should not be used directly. To iterate through pages just use `next_page_url` response field.
+        :type next_page_token: Optional[str]
+
+        :return: List of market metrics statistics.
+        :rtype: CatalogV2DataCollection
+        """
+        params: Dict[str, Any] = {
+            "markets": markets,
+            "exchange": exchange,
+            "type": market_type,
+            "base": base,
+            "quote": quote,
+            "asset": asset,
+            "symbol": symbol,
+            "format": format,
+            "page_size": page_size,
+            "paging_from": paging_from,
+            "next_page_token": next_page_token,
+        }
+        return CatalogV2DataCollection(self._get_data, "/catalog-all-v2/market-metrics", params)
+
     def get_asset_alerts(
         self,
         assets: Union[List[str], str],
         alerts: Union[List[str], str],
         page_size: Optional[int] = None,
         paging_from: Optional[Union[PagingFrom, str]] = "start",
         start_time: Optional[Union[datetime, date, str]] = None,
```

### Comparing `coinmetrics_api_client-2023.7.11.17/coinmetrics/data_exporter.py` & `coinmetrics_api_client-2023.8.2.13/coinmetrics/data_exporter.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.7.11.17/coinmetrics/typer_cli.py` & `coinmetrics_api_client-2023.8.2.13/coinmetrics/typer_cli.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.7.11.17/pyproject.toml` & `coinmetrics_api_client-2023.8.2.13/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "coinmetrics-api-client"
-version = "2023.7.11.17"
+version = "2023.8.2.13"
 description = "Python client for Coin Metrics API v4."
 authors = ["Coin Metrics <info@coinmetrics.io>", "Oleksandr Buchkovskyi <oleksandr@coinmetrics.io>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://coinmetrics.github.io/api-client-python/site/index.html"
 repository = "https://github.com/coinmetrics/api-client-python"
 packages = [{include = "coinmetrics"}]
@@ -23,15 +23,15 @@
 
 [tool.poetry.dev-dependencies]
 mypy = "^1.1.1"
 flake8 = "^3.8.3"
 black = "^23.1"
 mkdocs = "^1.3.1"
 mkdocs-material = "^9.1.3"
-pydoc-markdown = "^4.6.4"
+pydoc-markdown = "^4.8"
 
 pytest-mock = "^3.2.0"
 
 [tool.poetry.scripts]
 coinmetrics = 'coinmetrics.typer_cli:main'
 
 [build-system]
```

### Comparing `coinmetrics_api_client-2023.7.11.17/test/data/catalog_asset_pair_candles.csv` & `coinmetrics_api_client-2023.8.2.13/test/data/catalog_asset_pair_candles.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.7.11.17/test/data/catalog_assets_markets.csv` & `coinmetrics_api_client-2023.8.2.13/test/data/catalog_assets_markets.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.7.11.17/test/data/catalog_assets_metrics.csv` & `coinmetrics_api_client-2023.8.2.13/test/data/catalog_assets_metrics.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.7.11.17/test/data/catalog_exchanges_markets.csv` & `coinmetrics_api_client-2023.8.2.13/test/data/catalog_exchanges_markets.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.7.11.17/test/data/catalog_exchanges_metrics.csv` & `coinmetrics_api_client-2023.8.2.13/test/data/catalog_exchanges_metrics.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.7.11.17/test/data/catalog_indexes.csv` & `coinmetrics_api_client-2023.8.2.13/test/data/catalog_indexes.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.7.11.17/test/data/catalog_markets.csv` & `coinmetrics_api_client-2023.8.2.13/test/data/catalog_markets.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.7.11.17/test/data/catalog_metrics.csv` & `coinmetrics_api_client-2023.8.2.13/test/data/catalog_metrics.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.7.11.17/test/test_api_client.py` & `coinmetrics_api_client-2023.8.2.13/test/test_api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+import logging
 import os
-from typing import Any
+from typing import Any, Type
 from unittest.mock import Mock
 
 from coinmetrics.api_client import CoinMetricsClient, requests
 from coinmetrics._catalogs import (
     CatalogAssetsData,
     CatalogAssetAlertsData,
     CatalogAssetPairsData,
@@ -17,25 +18,23 @@
     CatalogMarketTradesData,
 )
 from coinmetrics._data_collection import DataCollection
 from coinmetrics._typing import (
     DataRetrievalFuncType,
     UrlParamTypes,
     Dict,
-    DataReturnType,
-    DataFrameType,
+    DataReturnType
 )
 
 try:
-    import pandas as pd  # type: ignore
+    import pandas as pd
 
-    DataFrameType = pd.core.frame.DataFrame
+    DataFrameType: Type[pd.core.frame.DataFrame] = pd.core.frame.DataFrame
 except ImportError:
-    pd = None
-    DataFrameType = Any
+    logging.info("Pandas not imported")
 
 catalog_assets_test_data = [
     {
         "asset": "btc",
         "full_name": "Bitcoin",
         "metrics": [
             {
@@ -615,25 +614,25 @@
     test_data_retrieval_function: DataRetrievalFuncType = lambda x, y: test_data_dict
 
     test_data_collection: DataCollection = DataCollection(
         data_retrieval_function=test_data_retrieval_function,
         endpoint="",
         url_params=test_param_dict,
     )
-    test_df: DataFrameType = test_data_collection.to_dataframe()
+    test_df: pd.DataFrame = test_data_collection.to_dataframe()
     assert test_df.shape == (2, 2)
     assert list(test_param_dict.keys()) == list(test_df.columns)
     assert (test_df["asset"] == "btc").all()
 
     test_data_collection_header = DataCollection(
         data_retrieval_function=test_data_retrieval_function,
         endpoint="",
         url_params=test_param_dict,
     )
-    test_df_header: DataFrameType = test_data_collection_header.to_dataframe(
+    test_df_header: pd.DataFrame = test_data_collection_header.to_dataframe(
         header=test_header
     )
     assert list(test_df_header.columns) == test_header
 
 
 def test_catalog_assets_dataframe() -> None:
     data = CatalogAssetsData(catalog_assets_test_data)
```

### Comparing `coinmetrics_api_client-2023.7.11.17/test/test_api_methods.py` & `coinmetrics_api_client-2023.8.2.13/test/test_api_methods.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.7.11.17/test/test_as_list.py` & `coinmetrics_api_client-2023.8.2.13/test/test_as_list.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.7.11.17/test/test_blockchain_methods.py` & `coinmetrics_api_client-2023.8.2.13/test/test_blockchain_methods.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.7.11.17/test/test_custom_exceptions.py` & `coinmetrics_api_client-2023.8.2.13/test/test_custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.7.11.17/test/test_data_exporter.py` & `coinmetrics_api_client-2023.8.2.13/test/test_data_exporter.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.7.11.17/test/test_debugging.py` & `coinmetrics_api_client-2023.8.2.13/test/test_debugging.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.7.11.17/test/test_models.py` & `coinmetrics_api_client-2023.8.2.13/test/test_models.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.7.11.17/test/test_rate_limits.py` & `coinmetrics_api_client-2023.8.2.13/test/test_rate_limits.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.7.11.17/test/test_to_dataframe.py` & `coinmetrics_api_client-2023.8.2.13/test/test_to_dataframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import pandas as pd  # type: ignore
+import pandas as pd
 import pytest
 from coinmetrics.api_client import CoinMetricsClient
 import os
 import numpy as np
 
 CM_API_KEY = os.environ.get("CM_API_KEY")
 client = CoinMetricsClient(str(CM_API_KEY))
```

### Comparing `coinmetrics_api_client-2023.7.11.17/test/test_websocket_methods.py` & `coinmetrics_api_client-2023.8.2.13/test/test_websocket_methods.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.7.11.17/PKG-INFO` & `coinmetrics_api_client-2023.8.2.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinmetrics-api-client
-Version: 2023.7.11.17
+Version: 2023.8.2.13
 Summary: Python client for Coin Metrics API v4.
 Home-page: https://coinmetrics.github.io/api-client-python/site/index.html
 License: MIT
 Keywords: coin metrics,coin,metrics,crypto,bitcoin,network-data,market-data,api,handy
 Author: Coin Metrics
 Author-email: info@coinmetrics.io
 Requires-Python: >=3.7.1,<4.0.0
```

