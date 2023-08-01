# Comparing `tmp/zutool-0.0.4.tar.gz` & `tmp/zutool-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zutool-0.0.4.tar", max compression
+gzip compressed data, was "zutool-0.0.5.tar", max compression
```

## Comparing `zutool-0.0.4.tar` & `zutool-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0     1049 2023-07-26 18:26:47.272546 zutool-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0     8795 2023-07-26 18:26:47.272546 zutool-0.0.4/README.md
--rw-r--r--   0        0        0     1965 2023-07-26 18:26:47.272546 zutool-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      244 2023-07-26 18:26:47.272546 zutool-0.0.4/zutool/__init__.py
--rw-r--r--   0        0        0     1775 2023-07-26 18:26:47.272546 zutool-0.0.4/zutool/api.py
--rw-r--r--   0        0        0     7149 2023-07-26 18:26:47.272546 zutool-0.0.4/zutool/main.py
--rw-r--r--   0        0        0      410 2023-07-26 18:26:47.272546 zutool-0.0.4/zutool/models/__init__.py
--rw-r--r--   0        0        0     1630 2023-07-26 18:26:47.272546 zutool-0.0.4/zutool/models/enum.py
--rw-r--r--   0        0        0      363 2023-07-26 18:26:47.272546 zutool-0.0.4/zutool/models/error.py
--rw-r--r--   0        0        0     1023 2023-07-26 18:26:47.272546 zutool-0.0.4/zutool/models/get_pain_status.py
--rw-r--r--   0        0        0      657 2023-07-26 18:26:47.272546 zutool-0.0.4/zutool/models/get_weather_point.py
--rw-r--r--   0        0        0     2045 2023-07-26 18:26:47.272546 zutool-0.0.4/zutool/models/get_weather_status.py
--rw-r--r--   0        0        0      131 2023-07-26 18:26:47.272546 zutool-0.0.4/zutool/models/set_weather_point.py
--rw-r--r--   0        0        0        0 2023-07-26 18:26:47.272546 zutool-0.0.4/zutool/py.typed
--rw-r--r--   0        0        0     9723 1970-01-01 00:00:00.000000 zutool-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1049 2023-08-01 22:11:29.574345 zutool-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0    11946 2023-08-01 22:11:29.574345 zutool-0.0.5/README.md
+-rw-r--r--   0        0        0     1965 2023-08-01 22:11:29.574345 zutool-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      282 2023-08-01 22:11:29.574345 zutool-0.0.5/zutool/__init__.py
+-rw-r--r--   0        0        0     2758 2023-08-01 22:11:29.574345 zutool-0.0.5/zutool/api.py
+-rw-r--r--   0        0        0     8767 2023-08-01 22:11:29.574345 zutool-0.0.5/zutool/main.py
+-rw-r--r--   0        0        0      487 2023-08-01 22:11:29.574345 zutool-0.0.5/zutool/models/__init__.py
+-rw-r--r--   0        0        0      458 2023-08-01 22:11:29.574345 zutool-0.0.5/zutool/models/dict.py
+-rw-r--r--   0        0        0     2703 2023-08-01 22:11:29.574345 zutool-0.0.5/zutool/models/enum.py
+-rw-r--r--   0        0        0      363 2023-08-01 22:11:29.574345 zutool-0.0.5/zutool/models/error.py
+-rw-r--r--   0        0        0     2163 2023-08-01 22:11:29.574345 zutool-0.0.5/zutool/models/get_otenki_asp.py
+-rw-r--r--   0        0        0     1023 2023-08-01 22:11:29.574345 zutool-0.0.5/zutool/models/get_pain_status.py
+-rw-r--r--   0        0        0      657 2023-08-01 22:11:29.574345 zutool-0.0.5/zutool/models/get_weather_point.py
+-rw-r--r--   0        0        0     2047 2023-08-01 22:11:29.574345 zutool-0.0.5/zutool/models/get_weather_status.py
+-rw-r--r--   0        0        0      131 2023-08-01 22:11:29.574345 zutool-0.0.5/zutool/models/set_weather_point.py
+-rw-r--r--   0        0        0        0 2023-08-01 22:11:29.574345 zutool-0.0.5/zutool/py.typed
+-rw-r--r--   0        0        0    12874 1970-01-01 00:00:00.000000 zutool-0.0.5/PKG-INFO
```

### Comparing `zutool-0.0.4/LICENSE.txt` & `zutool-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zutool-0.0.4/README.md` & `zutool-0.0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: zutool
+Version: 0.0.5
+Summary: Unofficial zutool (頭痛ール: https://zutool.jp/) API Wrapper
+Home-page: https://github.com/eggplants/zutool
+License: MIT
+Keywords: zutool
+Author: eggplants
+Author-email: w10776e8w@yahoo.co.jp
+Requires-Python: >=3.9,<4
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Dist: pydantic (>=2.0.3,<3.0.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: rich (>=13.4.2,<14.0.0)
+Project-URL: Repository, https://github.com/eggplants/zutool
+Description-Content-Type: text/markdown
+
 # zutool
 
 [![PyPI version](
   <https://badge.fury.io/py/zutool.svg>
   )](
   <https://badge.fury.io/py/zutool>
 ) [![Maintainability](
@@ -16,14 +40,18 @@
   <https://api.codeclimate.com/v1/badges/b999c03e104b0629e426/test_coverage>
   )](
   <https://codeclimate.com/github/eggplants/zutool/test_coverage>
 ) [![Test](
   <https://github.com/eggplants/zutool/actions/workflows/test.yml/badge.svg>
   )](
   <https://github.com/eggplants/zutool/actions/workflows/test.yml>
+) [![Release](
+  <https://github.com/eggplants/zutool/actions/workflows/release.yml/badge.svg>
+  )](
+  <https://github.com/eggplants/zutool/actions/workflows/release.yml>
 )
 
 [![ghcr latest](
   <https://ghcr-badge.deta.dev/eggplants/zutool/latest_tag?trim=major&label=latest>
  ) ![ghcr size](
   <https://ghcr-badge.deta.dev/eggplants/zutool/size>
 )](
@@ -49,29 +77,33 @@
 
 keyword = "東京都"
 z.get_weather_point(keyword)
 
 # see: <https://geoshape.ex.nii.ac.jp/city/code/?13113>
 city_code = "13113" # 東京都渋谷区
 z.get_weather_status(city_code)
+
+city_code = "13101" # 東京都千代田区
+z.get_otenki_asp(city_code)
 ```
 
 ## As CLI
 
 ```shellsession
 $ zutool -h
-usage: zutool [-h] [-j] {pain_status,ps,weather_point,wp,weather_status,ws} ...
+usage: zutool [-h] [-j] {pain_status,ps,weather_point,wp,weather_status,ws,otenki_asp,oa} ...
 
 Get info of zutool <https://zutool.jp/>.
 
 positional arguments:
-  {pain_status,ps,weather_point,wp,weather_status,ws}
+  {pain_status,ps,weather_point,wp,weather_status,ws,otenki_asp,oa}
     pain_status (ps)          get pain status by prefecture
     weather_point (wp)        search weather point
     weather_status (ws)       get pain status by city
+    otenki_asp (oa)           get weather infomations
 
 optional arguments:
   -h, --help                  show this help message and exit
   -j, --json                  print as json (default: False)
 ```
 
 ### `pain_status (ps)`
@@ -161,7 +193,39 @@
 │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │ ☼      │
 │ 34.5℃  │ 35.3℃  │ 35.7℃  │ 35.2℃  │ 33.9℃  │ 32.2℃  │ 30.4℃  │ 28.6℃  │ 27.2℃  │ 26.5℃  │ 26.3℃  │ 26.3℃  │
 │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │
 │ 1015.5 │ 1014.9 │ 1014.3 │ 1013.9 │ 1013.8 │ 1013.8 │ 1014.2 │ 1014.7 │ 1015.4 │ 1016.0 │ 1015.8 │ 1015.9 │
 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │
 └────────┴────────┴────────┴────────┴────────┴────────┴────────┴────────┴────────┴────────┴────────┴────────┘
 ```
+
+### `otenki_asp (oa)`
+
+```shellsession
+$ zutool oa -h
+usage: zutool otenki_asp [-h] [-n N [N ...]] {01101,04101,13101,15103,17201,23106,27128,34101,39201,40133,47201}
+
+positional arguments:
+  {01101,04101,13101,15103,17201,23106,27128,34101,39201,40133,47201}
+                                                  see: <https://geoshape.ex.nii.ac.jp/city/code/> (ex. `13113`)
+
+optional arguments:
+  -h, --help                                      show this help message and exit
+  -n N [N ...]                                    specify day number to show (default: [0, 1, 2, 3, 4, 5, 6])
+```
+
+```shellsession
+$ zutool oa 13101
+                                            <東京|13101>の天気情報
+┏━━━━━━━┳━━━━━━━━━━━━┳━━━━━━━━━━┳━━━━━━━━━━┳━━━━━━━━━━┳━━━━━━━━━━┳━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━┳━━━━━━━━━━┓
+┃ 日付  ┃ 天気       ┃ 降水確率 ┃ 最高気温 ┃ 最低気温 ┃ 最大風速 ┃ 最大風速時風向 ┃ 気圧予報レベル ┃ 最小湿度 ┃
+┡━━━━━━━╇━━━━━━━━━━━━╇━━━━━━━━━━╇━━━━━━━━━━╇━━━━━━━━━━╇━━━━━━━━━━╇━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━╇━━━━━━━━━━┩
+│ 08/02 │ 晴れ       │ 10.0     │ 35.0     │ 26.0     │ 11.2     │ 8.0            │ 2.0            │ 60.5     │
+│ 08/03 │ 晴れ       │ 10.0     │ 36.0     │ 26.0     │ 11.8     │ 8.0            │ 4.0            │ 63.6     │
+│ 08/04 │ 晴れ       │ 0.0      │ 36.0     │ 26.0     │ 10.0     │ 8.0            │ 2.0            │ 59.6     │
+│ 08/05 │ 晴れのち雨 │ 30.0     │ 36.0     │ 27.0     │ 11.8     │ 8.0            │ 1.0            │ 64.3     │
+│ 08/06 │ 雨のち晴れ │ 30.0     │ 36.0     │ 27.0     │ 10.3     │ 8.0            │ 2.0            │ 61.9     │
+│ 08/07 │ 晴れのち雨 │ 50.0     │ 33.0     │ 26.0     │ 7.2      │ 2.0            │ 2.0            │ 63.6     │
+│ 08/08 │ 雨一時晴れ │ 80.0     │ 33.0     │ 26.0     │ 6.2      │ 6.0            │ 1.0            │ 79.5     │
+└───────┴────────────┴──────────┴──────────┴──────────┴──────────┴────────────────┴────────────────┴──────────┘
+```
+
```

### Comparing `zutool-0.0.4/pyproject.toml` & `zutool-0.0.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 description = "Unofficial zutool (頭痛ール: https://zutool.jp/) API Wrapper"
 keywords = ["zutool"]
 name = "zutool"
 packages = [{include = "zutool"}]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/eggplants/zutool"
-version = "0.0.4"
+version = "0.0.5"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
 requests = "^2.28.2"
 pydantic = "^2.0.3"
 rich = "^13.4.2"
```

### Comparing `zutool-0.0.4/zutool/main.py` & `zutool-0.0.5/zutool/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from shutil import get_terminal_size
 from typing import TYPE_CHECKING
 
 from rich.console import Console
 from rich.table import Table
 
 from . import api
+from .models.dict import CONFIRMED_OTENKI_ASP_CITY_CODE_DICT, WEATHER_EMOJI_DICT
 from .models.get_pain_status import _GetPainStatus
 
 if TYPE_CHECKING:
     from .models.get_weather_status import _WeatherStatusByTime
 
 
 class _ZutoolFormatter(argparse.ArgumentDefaultsHelpFormatter, argparse.RawDescriptionHelpFormatter):
@@ -77,55 +78,79 @@
         fields = [weather_point.city_code, weather_point.name]
         if bool(ns.kata):
             fields.append(weather_point.name_kata)
         table.add_row(*fields)
     Console().print(table)
 
 
-def func_weather_status(ns: argparse.Namespace) -> None:
-    def __helper(res: list[_WeatherStatusByTime], n: int, prev_pressure: float, title: str) -> float:
-        table = Table()
-        for i in range(12 * n, 12 * (n + 1)):
-            table.add_column(str(i))
-        weathers, temps, pressures, pressure_levels = [], [], [], []
-        for by_time in res[12 * n : 12 * (n + 1)]:
-            weathers.append({"100": "☼", "200": "☁", "300": "☔", "400": "☃"}[by_time.weather.value])
-            temps.append(f"{by_time.temp}℃")
-            pressure = by_time.pressure
-            pressures.append(
-                f"↗\n{pressure}"
-                if pressure > prev_pressure
-                else f"↘\n{pressure}"
-                if pressure < prev_pressure
-                else f"→\n{pressure}",
-            )
-            pressure_levels.append(by_time.pressure_level.name)
-        table.add_row(*weathers)
-        table.add_row(*temps)
-        table.add_row(*pressures)
-        table.add_row(*pressure_levels)
-
-        if n == 0:
-            table.title = title
-        Console().print(table)
-        return prev_pressure
+def __func_weather_status_helper(res: list[_WeatherStatusByTime], n: int, prev_pressure: float, title: str) -> float:
+    table = Table()
+    for i in range(12 * n, 12 * (n + 1)):
+        table.add_column(str(i))
+    weathers, temps, pressures, pressure_levels = [], [], [], []
+    for by_time in res[12 * n : 12 * (n + 1)]:
+        weathers.append(WEATHER_EMOJI_DICT[int(by_time.weather.value)])
+        temps.append(f"{by_time.temp}℃")
+        pressure = by_time.pressure
+        pressures.append(
+            f"↗\n{pressure}"
+            if pressure > prev_pressure
+            else f"↘\n{pressure}"
+            if pressure < prev_pressure
+            else f"→\n{pressure}",
+        )
+        pressure_levels.append(by_time.pressure_level.name)
+    table.add_row(*weathers)
+    table.add_row(*temps)
+    table.add_row(*pressures)
+    table.add_row(*pressure_levels)
+
+    if n == 0:
+        table.title = title
+    Console().print(table)
+    return prev_pressure
+
 
+def func_weather_status(ns: argparse.Namespace) -> None:
     try:
         res_raw = api.get_weather_status(ns.city_code)
     except ValueError as e:
         print(f"{type(e).__name__}:", e, file=sys.stderr)
         sys.exit(1)
     if bool(ns.json):
         print(res_raw.model_dump_json(indent=4))
         return
     for day_idx, day in enumerate([("yesterday", "today", "tomorrow", "dayaftertomorrow")[i + 1] for i in ns.n]):
         res: list[_WeatherStatusByTime] = getattr(res_raw, day)
         title = f"{res_raw.place_name}の気圧予報\n{res_raw.date_time+timedelta(days=day_idx-1)}"
-        prev_pressure = __helper(res, 0, 0, title)
-        __helper(res, 1, prev_pressure, title)
+        prev_pressure = __func_weather_status_helper(res, 0, 0, title)
+        __func_weather_status_helper(res, 1, prev_pressure, title)
+
+
+def func_otenki_asp(ns: argparse.Namespace) -> None:
+    try:
+        res = api.get_otenki_asp(ns.city_code)
+    except ValueError as e:
+        print(f"{type(e).__name__}:", e, file=sys.stderr)
+        sys.exit(1)
+    if bool(ns.json):
+        print(res.model_dump_json(indent=4))
+        return
+    table = Table(title=f"<{CONFIRMED_OTENKI_ASP_CITY_CODE_DICT[ns.city_code]}|{ns.city_code}>の天気情報")
+    table.add_column("日付")
+    for element in res.elements:
+        table.add_column(element.title.replace("(日別)", ""))
+
+    target_date_times = [date_time for i, date_time in enumerate(res.elements[0].records.keys()) if i in ns.n]
+    for target_date_time in target_date_times:
+        table.add_row(
+            target_date_time.strftime("%m/%d"),
+            *[getattr(v := element.records[target_date_time], "name", str(v)) for element in res.elements],
+        )
+    Console().print(table)
 
 
 def parse(test_args: list[str] | None = None) -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="zutool",
         formatter_class=lambda prog: __get_formatter_class(prog, 30),
         description="Get info of zutool <https://zutool.jp/>.",
@@ -199,14 +224,38 @@
         metavar="N",
         nargs="+",
         help="specify day number to show",
     )
 
     weather_status_parser.set_defaults(func=func_weather_status)
 
+    otenki_asp_parser = subparsers.add_parser(
+        "otenki_asp",
+        aliases=["oa"],
+        formatter_class=lambda prog: __get_formatter_class(prog),
+        help="get weather infomations",
+    )
+    otenki_asp_parser.add_argument(
+        "city_code",
+        choices=CONFIRMED_OTENKI_ASP_CITY_CODE_DICT.keys(),
+        type=str,
+        help="see: <https://geoshape.ex.nii.ac.jp/city/code/> (ex. `13113`)",
+    )
+    otenki_asp_parser.add_argument(
+        "-n",
+        choices=range(7),
+        default=[*range(7)],
+        type=int,
+        metavar="N",
+        nargs="+",
+        help="specify day number to show",
+    )
+
+    otenki_asp_parser.set_defaults(func=func_otenki_asp)
+
     if test_args is not None:
         return parser.parse_args(test_args)
     return parser.parse_args()
 
 
 def main(test_args: list[str] | None = None) -> None:
     args = parse(test_args=test_args)
```

### Comparing `zutool-0.0.4/zutool/models/get_pain_status.py` & `zutool-0.0.5/zutool/models/get_pain_status.py`

 * *Files identical despite different names*

### Comparing `zutool-0.0.4/zutool/models/get_weather_point.py` & `zutool-0.0.5/zutool/models/get_weather_point.py`

 * *Files identical despite different names*

### Comparing `zutool-0.0.4/zutool/models/get_weather_status.py` & `zutool-0.0.5/zutool/models/get_weather_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from datetime import datetime, timedelta, timezone
 
 from pydantic import BaseModel, Field, field_validator
 
 from .enum import AreaEnum, PressureLevelEnum, WeatherEnum
 
-JTC = timezone(timedelta(hours=9))
+_JTC = timezone(timedelta(hours=9))
 
 
 class _WeatherStatusByTime(BaseModel):
     time: int = Field(ge=0, le=24)
     weather: WeatherEnum
     temp: float
     pressure: float
@@ -50,8 +50,8 @@
             return AreaEnum(v)
         except KeyError as e:
             msg = f"Error validating prefectures_id {e}. Valid ones are: {[a.name for a in AreaEnum]}"
             raise ValueError(msg) from e
 
     @field_validator("date_time", mode="before")
     def validate_date_time(cls, v: str) -> datetime:
-        return datetime.strptime(v, "%Y-%m-%d %H").replace(tzinfo=JTC)
+        return datetime.strptime(v, "%Y-%m-%d %H").replace(tzinfo=_JTC)
```

### Comparing `zutool-0.0.4/PKG-INFO` & `zutool-0.0.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: zutool
-Version: 0.0.4
-Summary: Unofficial zutool (頭痛ール: https://zutool.jp/) API Wrapper
-Home-page: https://github.com/eggplants/zutool
-License: MIT
-Keywords: zutool
-Author: eggplants
-Author-email: w10776e8w@yahoo.co.jp
-Requires-Python: >=3.9,<4
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Dist: pydantic (>=2.0.3,<3.0.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
-Requires-Dist: rich (>=13.4.2,<14.0.0)
-Project-URL: Repository, https://github.com/eggplants/zutool
-Description-Content-Type: text/markdown
-
 # zutool
 
 [![PyPI version](
   <https://badge.fury.io/py/zutool.svg>
   )](
   <https://badge.fury.io/py/zutool>
 ) [![Maintainability](
@@ -40,14 +16,18 @@
   <https://api.codeclimate.com/v1/badges/b999c03e104b0629e426/test_coverage>
   )](
   <https://codeclimate.com/github/eggplants/zutool/test_coverage>
 ) [![Test](
   <https://github.com/eggplants/zutool/actions/workflows/test.yml/badge.svg>
   )](
   <https://github.com/eggplants/zutool/actions/workflows/test.yml>
+) [![Release](
+  <https://github.com/eggplants/zutool/actions/workflows/release.yml/badge.svg>
+  )](
+  <https://github.com/eggplants/zutool/actions/workflows/release.yml>
 )
 
 [![ghcr latest](
   <https://ghcr-badge.deta.dev/eggplants/zutool/latest_tag?trim=major&label=latest>
  ) ![ghcr size](
   <https://ghcr-badge.deta.dev/eggplants/zutool/size>
 )](
@@ -73,29 +53,33 @@
 
 keyword = "東京都"
 z.get_weather_point(keyword)
 
 # see: <https://geoshape.ex.nii.ac.jp/city/code/?13113>
 city_code = "13113" # 東京都渋谷区
 z.get_weather_status(city_code)
+
+city_code = "13101" # 東京都千代田区
+z.get_otenki_asp(city_code)
 ```
 
 ## As CLI
 
 ```shellsession
 $ zutool -h
-usage: zutool [-h] [-j] {pain_status,ps,weather_point,wp,weather_status,ws} ...
+usage: zutool [-h] [-j] {pain_status,ps,weather_point,wp,weather_status,ws,otenki_asp,oa} ...
 
 Get info of zutool <https://zutool.jp/>.
 
 positional arguments:
-  {pain_status,ps,weather_point,wp,weather_status,ws}
+  {pain_status,ps,weather_point,wp,weather_status,ws,otenki_asp,oa}
     pain_status (ps)          get pain status by prefecture
     weather_point (wp)        search weather point
     weather_status (ws)       get pain status by city
+    otenki_asp (oa)           get weather infomations
 
 optional arguments:
   -h, --help                  show this help message and exit
   -j, --json                  print as json (default: False)
 ```
 
 ### `pain_status (ps)`
@@ -186,7 +170,37 @@
 │ 34.5℃  │ 35.3℃  │ 35.7℃  │ 35.2℃  │ 33.9℃  │ 32.2℃  │ 30.4℃  │ 28.6℃  │ 27.2℃  │ 26.5℃  │ 26.3℃  │ 26.3℃  │
 │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │ ↗      │
 │ 1015.5 │ 1014.9 │ 1014.3 │ 1013.9 │ 1013.8 │ 1013.8 │ 1014.2 │ 1014.7 │ 1015.4 │ 1016.0 │ 1015.8 │ 1015.9 │
 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │ 通常_0 │
 └────────┴────────┴────────┴────────┴────────┴────────┴────────┴────────┴────────┴────────┴────────┴────────┘
 ```
 
+### `otenki_asp (oa)`
+
+```shellsession
+$ zutool oa -h
+usage: zutool otenki_asp [-h] [-n N [N ...]] {01101,04101,13101,15103,17201,23106,27128,34101,39201,40133,47201}
+
+positional arguments:
+  {01101,04101,13101,15103,17201,23106,27128,34101,39201,40133,47201}
+                                                  see: <https://geoshape.ex.nii.ac.jp/city/code/> (ex. `13113`)
+
+optional arguments:
+  -h, --help                                      show this help message and exit
+  -n N [N ...]                                    specify day number to show (default: [0, 1, 2, 3, 4, 5, 6])
+```
+
+```shellsession
+$ zutool oa 13101
+                                            <東京|13101>の天気情報
+┏━━━━━━━┳━━━━━━━━━━━━┳━━━━━━━━━━┳━━━━━━━━━━┳━━━━━━━━━━┳━━━━━━━━━━┳━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━┳━━━━━━━━━━┓
+┃ 日付  ┃ 天気       ┃ 降水確率 ┃ 最高気温 ┃ 最低気温 ┃ 最大風速 ┃ 最大風速時風向 ┃ 気圧予報レベル ┃ 最小湿度 ┃
+┡━━━━━━━╇━━━━━━━━━━━━╇━━━━━━━━━━╇━━━━━━━━━━╇━━━━━━━━━━╇━━━━━━━━━━╇━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━╇━━━━━━━━━━┩
+│ 08/02 │ 晴れ       │ 10.0     │ 35.0     │ 26.0     │ 11.2     │ 8.0            │ 2.0            │ 60.5     │
+│ 08/03 │ 晴れ       │ 10.0     │ 36.0     │ 26.0     │ 11.8     │ 8.0            │ 4.0            │ 63.6     │
+│ 08/04 │ 晴れ       │ 0.0      │ 36.0     │ 26.0     │ 10.0     │ 8.0            │ 2.0            │ 59.6     │
+│ 08/05 │ 晴れのち雨 │ 30.0     │ 36.0     │ 27.0     │ 11.8     │ 8.0            │ 1.0            │ 64.3     │
+│ 08/06 │ 雨のち晴れ │ 30.0     │ 36.0     │ 27.0     │ 10.3     │ 8.0            │ 2.0            │ 61.9     │
+│ 08/07 │ 晴れのち雨 │ 50.0     │ 33.0     │ 26.0     │ 7.2      │ 2.0            │ 2.0            │ 63.6     │
+│ 08/08 │ 雨一時晴れ │ 80.0     │ 33.0     │ 26.0     │ 6.2      │ 6.0            │ 1.0            │ 79.5     │
+└───────┴────────────┴──────────┴──────────┴──────────┴──────────┴────────────────┴────────────────┴──────────┘
+```
```

