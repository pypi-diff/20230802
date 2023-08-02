# Comparing `tmp/SRTrain-2.0.7.tar.gz` & `tmp/SRTrain-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SRTrain-2.0.7.tar", last modified: Wed Apr  5 00:18:16 2023, max compression
+gzip compressed data, was "SRTrain-2.0.8.tar", last modified: Wed Aug  2 12:41:25 2023, max compression
```

## Comparing `SRTrain-2.0.7.tar` & `SRTrain-2.0.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 00:18:16.760538 SRTrain-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-05 00:18:05.000000 SRTrain-2.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-05 00:18:16.760538 SRTrain-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-05 00:18:05.000000 SRTrain-2.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 00:18:16.756538 SRTrain-2.0.7/SRT/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-05 00:18:05.000000 SRTrain-2.0.7/SRT/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 00:18:16.756538 SRTrain-2.0.7/SRT/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 00:18:05.000000 SRTrain-2.0.7/SRT/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-04-05 00:18:05.000000 SRTrain-2.0.7/SRT/cli/reserve.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-05 00:18:05.000000 SRTrain-2.0.7/SRT/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-05 00:18:05.000000 SRTrain-2.0.7/SRT/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-05 00:18:05.000000 SRTrain-2.0.7/SRT/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-04-05 00:18:05.000000 SRTrain-2.0.7/SRT/passenger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-05 00:18:05.000000 SRTrain-2.0.7/SRT/reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-05 00:18:05.000000 SRTrain-2.0.7/SRT/response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-05 00:18:05.000000 SRTrain-2.0.7/SRT/seat_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    15670 2023-04-05 00:18:05.000000 SRTrain-2.0.7/SRT/srt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 00:18:16.756538 SRTrain-2.0.7/SRT/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 00:18:05.000000 SRTrain-2.0.7/SRT/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-05 00:18:05.000000 SRTrain-2.0.7/SRT/tests/test_srt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-05 00:18:05.000000 SRTrain-2.0.7/SRT/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 00:18:16.760538 SRTrain-2.0.7/SRTrain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-05 00:18:16.000000 SRTrain-2.0.7/SRTrain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-05 00:18:16.000000 SRTrain-2.0.7/SRTrain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 00:18:16.000000 SRTrain-2.0.7/SRTrain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-05 00:18:16.000000 SRTrain-2.0.7/SRTrain.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 00:18:16.000000 SRTrain-2.0.7/SRTrain.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-05 00:18:16.000000 SRTrain-2.0.7/SRTrain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-05 00:18:16.000000 SRTrain-2.0.7/SRTrain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-05 00:18:05.000000 SRTrain-2.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-05 00:18:16.760538 SRTrain-2.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:41:25.852184 SRTrain-2.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-02 12:41:12.000000 SRTrain-2.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-08-02 12:41:25.852184 SRTrain-2.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-08-02 12:41:12.000000 SRTrain-2.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:41:25.852184 SRTrain-2.0.8/SRT/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-02 12:41:12.000000 SRTrain-2.0.8/SRT/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:41:25.852184 SRTrain-2.0.8/SRT/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:41:12.000000 SRTrain-2.0.8/SRT/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-08-02 12:41:12.000000 SRTrain-2.0.8/SRT/cli/reserve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-08-02 12:41:12.000000 SRTrain-2.0.8/SRT/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-08-02 12:41:12.000000 SRTrain-2.0.8/SRT/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-02 12:41:12.000000 SRTrain-2.0.8/SRT/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-08-02 12:41:12.000000 SRTrain-2.0.8/SRT/passenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-08-02 12:41:12.000000 SRTrain-2.0.8/SRT/reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-08-02 12:41:12.000000 SRTrain-2.0.8/SRT/response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-02 12:41:12.000000 SRTrain-2.0.8/SRT/seat_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15134 2023-08-02 12:41:12.000000 SRTrain-2.0.8/SRT/srt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:41:25.852184 SRTrain-2.0.8/SRT/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:41:12.000000 SRTrain-2.0.8/SRT/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-08-02 12:41:12.000000 SRTrain-2.0.8/SRT/tests/test_srt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-08-02 12:41:12.000000 SRTrain-2.0.8/SRT/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:41:25.852184 SRTrain-2.0.8/SRTrain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-08-02 12:41:25.000000 SRTrain-2.0.8/SRTrain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-02 12:41:25.000000 SRTrain-2.0.8/SRTrain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 12:41:25.000000 SRTrain-2.0.8/SRTrain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-02 12:41:25.000000 SRTrain-2.0.8/SRTrain.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 12:41:25.000000 SRTrain-2.0.8/SRTrain.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-02 12:41:25.000000 SRTrain-2.0.8/SRTrain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-02 12:41:25.000000 SRTrain-2.0.8/SRTrain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-02 12:41:12.000000 SRTrain-2.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-08-02 12:41:25.856184 SRTrain-2.0.8/setup.cfg
```

### Comparing `SRTrain-2.0.7/LICENSE` & `SRTrain-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `SRTrain-2.0.7/PKG-INFO` & `SRTrain-2.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: SRTrain
-Version: 2.0.7
+Version: 2.0.8
 Summary: SRT(Super Rapid Train) wrapper for python
 Home-page: https://github.com/ryanking13/SRT
 Author: ryanking13
 Author-email: def6488@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/ryanking13/SRT/issues
 Project-URL: Changelog, https://github.com/ryanking13/SRT/blob/master/CHANGELOG.md
 Keywords: one,two
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SRT
 
-![github actions badge](https://github.com/ryanking13/SRT/workflows/Python%20package/badge.svg)
+![github actions badge](https://github.com/ryanking13/SRT/workflows/Test/badge.svg)
 [![Downloads](https://pepy.tech/badge/srtrain)](https://pepy.tech/project/srtrain)
 [![Downloads](https://pepy.tech/badge/srtrain/month)](https://pepy.tech/project/srtrain)
 [![Documentation Status](https://readthedocs.org/projects/srtrain/badge/?version=latest)](https://srtrain.readthedocs.io/en/latest/?badge=latest)
 
 
 SRT(Super Rapid Train) application python wrapper
```

### Comparing `SRTrain-2.0.7/README.md` & `SRTrain-2.0.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # SRT
 
-![github actions badge](https://github.com/ryanking13/SRT/workflows/Python%20package/badge.svg)
+![github actions badge](https://github.com/ryanking13/SRT/workflows/Test/badge.svg)
 [![Downloads](https://pepy.tech/badge/srtrain)](https://pepy.tech/project/srtrain)
 [![Downloads](https://pepy.tech/badge/srtrain/month)](https://pepy.tech/project/srtrain)
 [![Documentation Status](https://readthedocs.org/projects/srtrain/badge/?version=latest)](https://srtrain.readthedocs.io/en/latest/?badge=latest)
 
 
 SRT(Super Rapid Train) application python wrapper
```

### Comparing `SRTrain-2.0.7/SRT/cli/reserve.py` & `SRTrain-2.0.8/SRT/cli/reserve.py`

 * *Files identical despite different names*

### Comparing `SRTrain-2.0.7/SRT/constants.py` & `SRTrain-2.0.8/SRT/constants.py`

 * *Files identical despite different names*

### Comparing `SRTrain-2.0.7/SRT/errors.py` & `SRTrain-2.0.8/SRT/errors.py`

 * *Files identical despite different names*

### Comparing `SRTrain-2.0.7/SRT/passenger.py` & `SRTrain-2.0.8/SRT/passenger.py`

 * *Files identical despite different names*

### Comparing `SRTrain-2.0.7/SRT/reservation.py` & `SRTrain-2.0.8/SRT/reservation.py`

 * *Files identical despite different names*

### Comparing `SRTrain-2.0.7/SRT/response_data.py` & `SRTrain-2.0.8/SRT/response_data.py`

 * *Files identical despite different names*

### Comparing `SRTrain-2.0.7/SRT/srt.py` & `SRTrain-2.0.8/SRT/srt.py`

 * *Files 17% similar despite different names*

```diff
@@ -53,32 +53,34 @@
         verbose (bool): 디버깅용 로그 출력 여부
 
     >>> srt = SRT("1234567890", YOUR_PASSWORD) # with membership number
     >>> srt = SRT("def6488@gmail.com", YOUR_PASSWORD) # with email
     >>> srt = SRT("010-1234-xxxx", YOUR_PASSWORD) # with phone number
     """
 
-    def __init__(self, srt_id, srt_pw, auto_login=True, verbose=False):
+    def __init__(
+        self, srt_id: str, srt_pw: str, auto_login: bool = True, verbose: bool = False
+    ) -> None:
         self._session = requests.session()
         self._session.headers.update(DEFAULT_HEADERS)
 
-        self.srt_id = srt_id
-        self.srt_pw = srt_pw
-        self.verbose = verbose
+        self.srt_id: str = srt_id
+        self.srt_pw: str = srt_pw
+        self.verbose: bool = verbose
 
-        self.is_login = False
+        self.is_login: bool = False
 
         if auto_login:
             self.login(srt_id, srt_pw)
 
-    def _log(self, msg):
+    def _log(self, msg: str) -> None:
         if self.verbose:
             print("[*] " + msg)
 
-    def login(self, srt_id=None, srt_pw=None):
+    def login(self, srt_id: str | None = None, srt_pw: str | None = None):
         """SRT 서버에 로그인합니다.
 
         일반적인 경우에는 인스턴스가 생성될 때에 자동으로 로그인 되므로,
         이 함수를 직접 호출할 필요가 없습니다.
 
         Args:
             srt_id (str, optional): SRT 계정 아이디
@@ -93,26 +95,30 @@
             self.srt_id = srt_id
 
         if srt_pw is None:
             srt_pw = self.srt_pw
         else:
             self.srt_pw = srt_pw
 
-        LOGIN_TYPES = {"MEMBERSHIP_ID": "1", "EMAIL": "2", "PHONE_NUMBER": "3"}
+        LOGIN_TYPES: dict[str, str] = {
+            "MEMBERSHIP_ID": "1",
+            "EMAIL": "2",
+            "PHONE_NUMBER": "3",
+        }
 
         if EMAIL_REGEX.match(srt_id):
             login_type = LOGIN_TYPES["EMAIL"]
         elif PHONE_NUMBER_REGEX.match(srt_id):
             login_type = LOGIN_TYPES["PHONE_NUMBER"]
             srt_id = re.sub("-", "", srt_id)  # hyphen is not sent
         else:
             login_type = LOGIN_TYPES["MEMBERSHIP_ID"]
 
         url = SRT_LOGIN
-        data = {
+        data: dict[str, str] = {
             "auto": "Y",
             "check": "Y",
             "page": "menu",
             "deviceKey": "-",
             "customerYn": "",
             "login_referer": SRT_MAIN,
             "srchDvCd": login_type,
@@ -127,72 +133,55 @@
             raise SRTLoginError(r.json()["MSG"])
 
         if "비밀번호 오류" in r.text:
             self.is_login = False
             raise SRTLoginError(r.json()["MSG"])
 
         self.is_login = True
-        return True
-        # parser = SRTResponseData(r.text)
 
-        # if parser.success():
-        #     status, result, _, __ = parser.get_all()
-        #     self.kr_session_id = status.get("KR_JSESSIONID")
-        #     self.sr_session_id = status.get("SR_JSESSIONID")
-        #     self.user_name = result.get("CUST_NM")
-        #     self.user_membership_number = result.get("MB_CRD_NO")
-        #     self.user_phone_number = result.get("MBL_PHONE")
-        #     self.user_type = result.get("CUST_MG_SRT_NM")  # 개인고객 or ...
-        #     self.user_level = result.get("CUST_DTL_SRT_NM")  # 일반회원 or ...
-        #     self.user_sex = result.get("SEX_DV_NM")
-        #     self._session.cookies.update({"gs_loginCrdNo": result.get("MB_CRD_NO")})
-
-        #     self._log(parser.message())
-        #     self.is_login = True
-        #     return True
-
-        # else:
-        #     self.is_login = False
-        #     raise SRTResponseError(parser.message())
+        return True
 
-    def logout(self):
+    def logout(self) -> bool:
         """SRT 서버에서 로그아웃합니다."""
 
         if not self.is_login:
-            return
+            return True
 
         url = SRT_LOGOUT
 
         r = self._session.post(url=url)
 
         if not r.ok:
             raise SRTResponseError(r.text)
 
         return True
 
     def search_train(
-        self, dep, arr, date=None, time=None, time_limit=None, available_only=True
-    ):
+        self,
+        dep: str,
+        arr: str,
+        date: str | None = None,
+        time: str | None = None,
+        time_limit: str | None = None,
+        available_only: bool = True,
+    ) -> list[SRTTrain]:
         """주어진 출발지에서 도착지로 향하는 SRT 열차를 검색합니다.
 
         Args:
             dep (str): 출발역
             arr (str): 도착역
             date (str, optional): 출발 날짜 (yyyyMMdd) (default: 당일)
             time (str, optional): 출발 시각 (hhmmss) (default: 0시 0분 0초)
             time_limit (str, optional): 출발 시각 조회 한도 (hhmmss)
             available_only (bool, optional): 매진되지 않은 열차만 검색합니다 (default: True)
 
         Returns:
             list[:class:`SRTTrain`]: 열차 리스트
         """
 
-        if not self.is_login:
-            raise SRTNotLoggedInError()
-
         if dep not in STATION_CODE:
             raise ValueError(f'Station "{dep}" not exists')
         if arr not in STATION_CODE:
             raise ValueError(f'Station "{arr}" not exists')
 
         dep_code = STATION_CODE[dep]
         arr_code = STATION_CODE[arr]
@@ -259,19 +248,19 @@
         if time_limit:
             trains = list(filter(lambda t: t.dep_time <= time_limit, trains))
 
         return trains
 
     def reserve(
         self,
-        train,
-        passengers=None,
-        special_seat=SeatType.GENERAL_FIRST,
-        window_seat=None,
-    ):
+        train: SRTTrain,
+        passengers: list[Passenger] | None = None,
+        special_seat: SeatType = SeatType.GENERAL_FIRST,
+        window_seat: bool | None = None,
+    ) -> SRTReservation:
         """열차를 예약합니다.
 
         >>> trains = srt.search_train("수서", "부산", "210101", "000000")
         >>> srt.reserve(trains[0])
 
         Args:
             train (:class:`SRTrain`): 예약할 열차
@@ -350,19 +339,19 @@
         reservation_result = parser.get_all()["reservListMap"][0]
 
         # find corresponding ticket and return it
         tickets = self.get_reservations()
         for ticket in tickets:
             if ticket.reservation_number == reservation_result["pnrNo"]:
                 return ticket
+
         # if ticket not found, it's an error
-        else:
-            SRTError("Ticket not found: check reservation status")
+        raise SRTError("Ticket not found: check reservation status")
 
-    def get_reservations(self, paid_only: bool = False):
+    def get_reservations(self, paid_only: bool = False) -> list[SRTReservation]:
         """전체 예약 정보를 얻습니다.
 
         Args:
             paid_only (bool): 결제된 예약 내역만 가져올지 여부
 
         Returns:
             list[:class:`SRTReservation`]: 예약 리스트
@@ -389,15 +378,15 @@
                 continue
             ticket = self.ticket_info(train["pnrNo"])
             reservation = SRTReservation(train, pay, ticket)
             reservations.append(reservation)
 
         return reservations
 
-    def ticket_info(self, reservation):
+    def ticket_info(self, reservation: SRTReservation | int) -> list[SRTTicket]:
         """예약에 포함된 티켓 정보를 반환합니다.
 
         >>> reservations = srt.get_reservations()
         >>> reservations
         # [[SRT] 09월 30일, 수서~부산(15:30~18:06) 130700원(3석), 구입기한 09월 19일 19:11]
         >>> reservations[0].tickets
         # [18호차 9C (일반실) 어른/청소년 [52300원(600원 할인)],
@@ -425,15 +414,15 @@
         if not parser.success():
             raise SRTResponseError(parser.message())
 
         tickets = [SRTTicket(ticket) for ticket in parser.get_all()["trainListMap"]]
 
         return tickets
 
-    def cancel(self, reservation):
+    def cancel(self, reservation: SRTReservation | int) -> bool:
         """예약을 취소합니다.
 
         >>> reservation = srt.reserve(train)
         >>> srt.cancel(reservation)
         >>> reservations = srt.get_reservations()
         >>> srt.cancel(reservations[0])
```

### Comparing `SRTrain-2.0.7/SRT/tests/test_srt.py` & `SRTrain-2.0.8/SRT/tests/test_srt.py`

 * *Files identical despite different names*

### Comparing `SRTrain-2.0.7/SRT/train.py` & `SRTrain-2.0.8/SRT/train.py`

 * *Files identical despite different names*

### Comparing `SRTrain-2.0.7/SRTrain.egg-info/PKG-INFO` & `SRTrain-2.0.8/SRTrain.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: SRTrain
-Version: 2.0.7
+Version: 2.0.8
 Summary: SRT(Super Rapid Train) wrapper for python
 Home-page: https://github.com/ryanking13/SRT
 Author: ryanking13
 Author-email: def6488@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/ryanking13/SRT/issues
 Project-URL: Changelog, https://github.com/ryanking13/SRT/blob/master/CHANGELOG.md
 Keywords: one,two
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SRT
 
-![github actions badge](https://github.com/ryanking13/SRT/workflows/Python%20package/badge.svg)
+![github actions badge](https://github.com/ryanking13/SRT/workflows/Test/badge.svg)
 [![Downloads](https://pepy.tech/badge/srtrain)](https://pepy.tech/project/srtrain)
 [![Downloads](https://pepy.tech/badge/srtrain/month)](https://pepy.tech/project/srtrain)
 [![Documentation Status](https://readthedocs.org/projects/srtrain/badge/?version=latest)](https://srtrain.readthedocs.io/en/latest/?badge=latest)
 
 
 SRT(Super Rapid Train) application python wrapper
```

### Comparing `SRTrain-2.0.7/pyproject.toml` & `SRTrain-2.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SRTrain-2.0.7/setup.cfg` & `SRTrain-2.0.8/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -12,27 +12,26 @@
 license_file = LICENSE
 platform = any
 classifiers = 
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Software Development :: Libraries :: Python Modules
 project_urls = 
 	Bug Tracker = https://github.com/ryanking13/SRT/issues
 	Changelog = https://github.com/ryanking13/SRT/blob/master/CHANGELOG.md
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
-python_requires = >= 3.8
+python_requires = >= 3.10
 install_requires = 
 	requests
 	PyInquirer
 
 [bdist_wheel]
 universal = true
```

