# Comparing `tmp/timeturner-0.3.0a0.tar.gz` & `tmp/timeturner-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeturner-0.3.0a0.tar", max compression
+gzip compressed data, was "timeturner-0.3.1.tar", max compression
```

## Comparing `timeturner-0.3.0a0.tar` & `timeturner-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1055 2023-03-09 18:33:41.398880 timeturner-0.3.0a0/LICENSE
--rw-r--r--   0        0        0     6099 2023-04-20 17:44:07.808207 timeturner-0.3.0a0/README.md
--rw-r--r--   0        0        0     1163 2023-04-27 12:01:12.321609 timeturner-0.3.0a0/pyproject.toml
--rw-r--r--   0        0        0       47 2023-04-27 12:02:37.218708 timeturner-0.3.0a0/timeturner/__init__.py
--rw-r--r--   0        0        0    12422 2023-04-16 18:53:08.962749 timeturner-0.3.0a0/timeturner/db.py
--rw-r--r--   0        0        0      674 2023-04-16 19:13:02.245927 timeturner-0.3.0a0/timeturner/helper.py
--rw-r--r--   0        0        0     3015 2023-04-14 14:18:26.695772 timeturner-0.3.0a0/timeturner/loader.py
--rw-r--r--   0        0        0     2534 2023-04-20 15:54:26.254760 timeturner-0.3.0a0/timeturner/models.py
--rw-r--r--   0        0        0     8708 2023-04-20 15:54:38.728125 timeturner-0.3.0a0/timeturner/parser.py
--rw-r--r--   0        0        0     3048 2023-04-20 15:55:29.878254 timeturner-0.3.0a0/timeturner/rich_output.py
--rw-r--r--   0        0        0     2614 2023-04-20 19:55:13.187167 timeturner-0.3.0a0/timeturner/run.py
--rw-r--r--   0        0        0     5890 2023-04-20 19:51:16.822890 timeturner-0.3.0a0/timeturner/settings.py
--rw-r--r--   0        0        0    16051 2023-04-20 19:54:37.770360 timeturner-0.3.0a0/timeturner/timeturner.py
--rw-r--r--   0        0        0     2773 2023-03-26 14:00:20.572942 timeturner-0.3.0a0/timeturner/tools/boltons_iterutils.py
--rw-r--r--   0        0        0     7132 1970-01-01 00:00:00.000000 timeturner-0.3.0a0/setup.py
--rw-r--r--   0        0        0     6607 1970-01-01 00:00:00.000000 timeturner-0.3.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-03-09 18:33:41.398880 timeturner-0.3.1/LICENSE
+-rw-r--r--   0        0        0     6162 2023-08-02 07:24:57.271895 timeturner-0.3.1/README.md
+-rw-r--r--   0        0        0     1161 2023-08-02 07:27:34.759133 timeturner-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-08-02 07:27:21.665750 timeturner-0.3.1/timeturner/__init__.py
+-rw-r--r--   0        0        0    12587 2023-08-02 07:24:57.271895 timeturner-0.3.1/timeturner/db.py
+-rw-r--r--   0        0        0      709 2023-04-27 12:45:43.590878 timeturner-0.3.1/timeturner/helper.py
+-rw-r--r--   0        0        0     3015 2023-04-14 14:18:26.695772 timeturner-0.3.1/timeturner/loader.py
+-rw-r--r--   0        0        0     2554 2023-04-27 12:58:23.861346 timeturner-0.3.1/timeturner/models.py
+-rw-r--r--   0        0        0     8708 2023-08-02 07:26:33.535570 timeturner-0.3.1/timeturner/parser.py
+-rw-r--r--   0        0        0     3137 2023-04-27 14:43:47.972879 timeturner-0.3.1/timeturner/rich_output.py
+-rw-r--r--   0        0        0     2614 2023-04-20 19:55:13.187167 timeturner-0.3.1/timeturner/run.py
+-rw-r--r--   0        0        0     7206 2023-04-27 16:47:25.646001 timeturner-0.3.1/timeturner/settings.py
+-rw-r--r--   0        0        0    17984 2023-08-02 07:24:57.271895 timeturner-0.3.1/timeturner/timeturner.py
+-rw-r--r--   0        0        0     2773 2023-03-26 14:00:20.572942 timeturner-0.3.1/timeturner/tools/boltons_iterutils.py
+-rw-r--r--   0        0        0     6668 1970-01-01 00:00:00.000000 timeturner-0.3.1/PKG-INFO
```

### Comparing `timeturner-0.3.0a0/LICENSE` & `timeturner-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `timeturner-0.3.0a0/README.md` & `timeturner-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,15 @@
   - [ ] split up multiday activities
   - [ ] summaries full day tags differently
   - [x] holidays should not count as work time
     - [x] it should also not count as missing work time
   - [ ] group by year, month, week, daysplit up multiday activities
   - [ ] add option to show only open activities
   - [ ] add tests
+  - [ ] MM-DD or YYYY-MM-DD should only show show a single day
 
 - [ ] import holidays
 
 - [ ] export
   - [ ] probably like list --format jsonl
 
 - [ ] undo (revert the last change)
```

### Comparing `timeturner-0.3.0a0/pyproject.toml` & `timeturner-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "timeturner"
-version = "0.3.0a0"
+version = "0.3.1"
 description = ""
 authors = ["Olaf Gladis <olaf@gladis.org>"]
 readme = "README.md"
 packages = [{ include = "timeturner" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `timeturner-0.3.0a0/timeturner/db.py` & `timeturner-0.3.1/timeturner/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,19 +246,23 @@
                         DELETE FROM tags WHERE tag = ?
                         """,
                         (tag,),
                     )
 
         self.connection.commit()
 
-    def get_latest_segment(self) -> PensiveRow | None:
+    def get_latest_segment(self, filter_closed_segments=False) -> PensiveRow | None:
         cursor = self.connection.cursor()
+        where_clause = ""
+        if filter_closed_segments:
+            where_clause = "WHERE end IS NULL"
         cursor.execute(
             f"""
             SELECT pk, start, end, passive, description FROM {self.table_name}
+            {where_clause}
             ORDER BY start DESC LIMIT 1
             """
         )
 
         row = cursor.fetchone()
         if row is None:
             return None
```

### Comparing `timeturner-0.3.0a0/timeturner/helper.py` & `timeturner-0.3.1/timeturner/helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from pendulum import period
 from pendulum.date import Date
 from pendulum.datetime import DateTime
 
 
 def iter_over_days(start: DateTime, end: DateTime) -> Iterator[Date]:
     end = end.subtract(microseconds=1)
+    if end < start:
+        return
     for dt in period(start.start_of("day"), end.start_of("day")).range("days"):
         yield cast(DateTime, dt).date()
 
 
 def end_of(dt: DateTime, unit: str) -> DateTime:
     """Return the first possible moment of the next unit."""
     return dt.start_of(unit).add(**{f"{unit}s": 1})
```

### Comparing `timeturner-0.3.0a0/timeturner/loader.py` & `timeturner-0.3.1/timeturner/loader.py`

 * *Files identical despite different names*

### Comparing `timeturner-0.3.0a0/timeturner/models.py` & `timeturner-0.3.1/timeturner/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,15 @@
 
 
 class SegmentsByDay(BaseModel):
     day: Date
     weekday: int
     segments: list[PensiveRow]
     summary: DailySummary
+    tags: list[str]
 
 
 class NewSegmentParams(BaseModel):
     start: DateTime
     end: Optional[DateTime]
     tags: list[str]
     description: str = ""
```

### Comparing `timeturner-0.3.0a0/timeturner/parser.py` & `timeturner-0.3.1/timeturner/parser.py`

 * *Files identical despite different names*

### Comparing `timeturner-0.3.0a0/timeturner/rich_output.py` & `timeturner-0.3.1/timeturner/rich_output.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 
     table.add_column("Start", style="dim", width=20)
     table.add_column("End", style="dim", width=6)
     table.add_column("Type", style="dim", width=6)
     table.add_column("Work Time", style="dim", width=8)
     table.add_column("Break Time", style="dim", width=8)
     table.add_column("Over Time", style="dim", width=8)
+    table.add_column("Tags", style="dim", width=20)
 
     total_work = []
     total_break = []
     total_over = []
     w = ["Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun"]
     for segment in segments:
         total_work.append(segment.summary.work_time)
@@ -70,14 +71,15 @@
         table.add_row(
             start_str,
             segment.summary.end.format("HH:mm") if segment.summary.end else "",
             str(segment.summary.day_type.value),
             pretty_duration(segment.summary.work_time),
             pretty_duration(segment.summary.break_time),
             pretty_duration(segment.summary.over_time),
+            ", ".join(segment.tags),
         )
     table.add_row(
         "total:",
         "",
         "",
         pretty_duration(sum(total_work, Duration())),
         pretty_duration(sum(total_break, Duration())),
```

### Comparing `timeturner-0.3.0a0/timeturner/run.py` & `timeturner-0.3.1/timeturner/run.py`

 * *Files identical despite different names*

### Comparing `timeturner-0.3.0a0/timeturner/settings.py` & `timeturner-0.3.1/timeturner/settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from os import environ
 from pathlib import Path
-from typing import Any, Literal
+from typing import Any, Iterable, Literal
 
 import tomlkit
 from pendulum.date import Date
 from pendulum.duration import Duration
 from pydantic import BaseModel, BaseSettings, root_validator
 
 from timeturner import __COMMIT__, __VERSION__
@@ -73,15 +73,15 @@
     name: str
     full_day: bool = False
     work_day: bool = False
     priority: int = 0
     track_work_time: bool = False
     track_work_time_passive: bool = False
     track_break_time: bool = False
-    # track_over_time: bool = False
+    track_over_time: bool = False
     only_cover_work_days: bool = False
 
     @root_validator
     def check_tag_settings(cls, values):
         if values["track_work_time"] and values["track_work_time_passive"]:
             raise ValueError(
                 "track_work_time and track_work_time_passive "
@@ -94,14 +94,23 @@
         if values["track_work_time_passive"] and values["track_break_time"]:
             raise ValueError(
                 "track_work_time_passive and track_break_time "
                 "cannot be set at the same time"
             )
         if values["only_cover_work_days"] and not values["full_day"]:
             raise ValueError("only_cover_work_days can only be set if full_day is set")
+
+        if values["track_over_time"] and not values["track_work_time"]:
+            raise ValueError(
+                "track_over_time can only be set if track_work_time is set"
+            )
+
+        if values["track_work_time"] and values["full_day"]:
+            raise ValueError("track_work_time cannot be set if full_day is set")
+
         return values
 
 
 class ReportSettings(BaseModel):
     output: Literal["json", "rich"] = "rich"
     holiday_tag: str = "holiday"
     passive_travel_tag: str = "travel"
@@ -109,15 +118,15 @@
     # sick_tag: str = "sick"
     # sick_certified_tag: str = "sick-certified"
     worktime_per_weekday: dict[int, DurationSetting] = {
         0: DurationSetting(hours=8),
         1: DurationSetting(hours=8),
         2: DurationSetting(hours=8),
         3: DurationSetting(hours=8),
-        4: DurationSetting(hours=2),
+        4: DurationSetting(hours=8),
         5: DurationSetting(hours=0),
         6: DurationSetting(hours=0),
     }
     reset_default_work_time: bool = True
     tag_settings: dict[str, TagSettings] = {
         "holiday": TagSettings(
             name="holiday",
@@ -142,22 +151,46 @@
         ),
         "travel": TagSettings(
             name="travel",
             track_work_time_passive=True,
         ),
     }
 
-    def is_work_day(self, day: Date):
+    def is_work_day(self, day: Date) -> bool:
         weekday = day.weekday()
         if not self.worktime_per_weekday:
             return 0 <= weekday <= 4
         if weekday in self.worktime_per_weekday:
             return bool(self.worktime_per_weekday[weekday].duration)
         return False
 
+    def has_full_day_tags(self, tags: Iterable[str]) -> bool:
+        for tag in tags:
+            if tag in self.tag_settings and self.tag_settings[tag].full_day:
+                return True
+        return False
+
+    def get_tag(self, tag: str) -> TagSettings:
+        if tag in self.tag_settings:
+            return self.tag_settings[tag]
+        return DefaultTagSettings(
+            name=tag,
+        )
+
+    def get_highest_priority_tag(
+        self, tags: Iterable[str], filter_full_day=False
+    ) -> TagSettings:
+
+        tag_settings = [self.get_tag(tag) for tag in tags]
+        if filter_full_day:
+            tag_settings = [tag for tag in tag_settings if tag.full_day]
+        if tag_settings:
+            return max(tag_settings, key=lambda tag: tag.priority)
+        return DefaultTagSettings()
+
     @root_validator
     def validate_tag_settings(cls, values):
 
         avaliable_tags = set(values["tag_settings"].keys())
         required_tags = {
             values["holiday_tag"],
             values["passive_travel_tag"],
@@ -195,7 +228,16 @@
         ):
             del file_secret_settings
             return (
                 init_settings,
                 env_settings,
                 load_config_file,
             )
+
+
+def DefaultTagSettings(name="no_tag"):
+
+    return TagSettings(
+        name=name,
+        track_work_time=True,
+        track_over_time=True,
+    )
```

### Comparing `timeturner-0.3.0a0/timeturner/timeturner.py` & `timeturner-0.3.1/timeturner/timeturner.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,20 +35,48 @@
     get daily work time
     get daily break time
     get daily overtime
 
     vacation and holiday are not considered work time and produce no overtime
     """
     work_time = Duration()
+    passive_work_time = Duration()
     break_time = Duration()
     start = None
     end = None
     by_tag = {}
     segment = None
+    track_work_time = True
+    tags = set(tag for segment in segments for tag in segment.tags)
+
+    has_full_day_tag = report_settings.has_full_day_tags(tags)
+    if has_full_day_tag:
+        assert len(segments) == 1
+
+    track_work_time = True
+    track_break_time = False
+    track_over_time = True
+    if tags:
+        highest_priority_tag = report_settings.get_highest_priority_tag(
+            tags,
+            filter_full_day=True,
+        )
+        if highest_priority_tag.full_day:
+            track_work_time = highest_priority_tag.track_work_time
+            track_break_time = highest_priority_tag.track_break_time
+            track_over_time = highest_priority_tag.track_over_time
+
     for segment in segments:
+        worktime_is_passive = False
+        for tag in segment.tags:
+            tag_setting = report_settings.get_tag(tag)
+            if tag_setting.track_work_time_passive:
+                worktime_is_passive = True
+                break
+
         if segment.start.date() != day:
             raise ValueError(
                 f"Segment is not on the given day. {day} != {segment.start.date()}"
             )
         if report_settings.holiday_tag in segment.tags:
             return DailySummary(
                 day=day,
@@ -59,15 +87,21 @@
                 start=None,
                 end=None,
                 description="Holiday",
                 by_tag={},
             )
         if start is None:
             start = segment.start.time()
-        work_time += segment.duration
+        if track_work_time:
+            if worktime_is_passive:
+                passive_work_time += segment.duration
+            else:
+                work_time += segment.duration
+        elif track_break_time:
+            break_time += segment.duration
         for tag in segment.tags:
             if tag not in by_tag:
                 by_tag[tag] = Duration()
             by_tag[tag] += segment.duration
 
     if segment and segment.end is not None:
         end = segment.end.time()
@@ -90,18 +124,30 @@
             break_time += missing_break_time
     elif work_time > Duration(hours=4):
         if break_time < Duration(minutes=15):
             missing_break_time = Duration(minutes=15) - break_time
             work_time -= missing_break_time
             break_time += missing_break_time
 
+    # only add passive work time until both add upto 10 hours
+    # everything above is ignored
+    if work_time > Duration(hours=10):
+        # we ignore passive work time
+        pass
+    elif work_time + passive_work_time > Duration(hours=10):
+        work_time = Duration(hours=10)
+    else:
+        work_time = work_time + passive_work_time
+
     required_work_duration = report_settings.worktime_per_weekday[
         day.weekday()
     ].duration
     day_type = DayType.WORK if required_work_duration else DayType.WEEKEND
+    if not track_over_time:
+        required_work_duration = Duration()
 
     return DailySummary(
         day=day,
         day_type=day_type,
         work_time=work_time,
         break_time=break_time,
         over_time=work_time - required_work_duration,
@@ -126,20 +172,20 @@
                 pk=row.pk,
                 start=row.start,
                 end=end_of_day(row.start),
                 tags=row.tags,
                 description=row.description,
                 passive=row.passive,
             )
-            for day in iter_over_days(row.start.add(days=1), row.end):
+            for day in iter_over_days(end_of_day(row.start), row.end):
                 if day == row.end.date():
                     end = row.end
                 else:
-                    end = day.add(days=1).start_of("day")
-                print(f"day: {day.start_of('day')}, end: {end}")
+                    _end = day.add(days=1)
+                    end = DateTime(_end.year, _end.month, _end.day, tzinfo=row.start.tz)
                 yield PensiveRow(
                     pk=row.pk,
                     start=DateTime(day.year, day.month, day.day, tzinfo=row.start.tz),
                     end=end,
                     tags=row.tags,
                     description=row.description,
                     passive=row.passive,
@@ -173,14 +219,22 @@
                 weekday=day.weekday(),
                 segments=segments,
                 summary=get_daily_summary(
                     day,
                     segments,
                     report_settings=report_settings,
                 ),
+                tags=sorted(
+                    set(
+                        tag
+                        for segment in segments
+                        for tag in segment.tags
+                        # if tag not in report_settings.ignore_tags
+                    )
+                ),
             )
         )
     return daily_segments
 
 
 def add(
     time: list[str] | None,
@@ -426,15 +480,15 @@
     *,
     report_settings: ReportSettings,
     db: DatabaseConnection,
 ) -> PensiveRow | None:
     if time is None:
         time = []
     end = single_time_parse(time)
-    last_entry = db.get_latest_segment()
+    last_entry = db.get_latest_segment(filter_closed_segments=True)
 
     if last_entry is None:
         raise ValueError("No entries to stop")
     if last_entry.end is not None:
         raise ValueError(f"Last entry already ended {last_entry.end!r}")
     pk = last_entry.pk
     db.update_segment(pk, end=end)
```

### Comparing `timeturner-0.3.0a0/timeturner/tools/boltons_iterutils.py` & `timeturner-0.3.1/timeturner/tools/boltons_iterutils.py`

 * *Files identical despite different names*

### Comparing `timeturner-0.3.0a0/setup.py` & `timeturner-0.3.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,188 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: timeturner
+Version: 0.3.1
+Summary: 
+Author: Olaf Gladis
+Author-email: olaf@gladis.org
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pendulum (>=2.1.2,<3.0.0)
+Requires-Dist: pydantic (>=1.10.5,<2.0.0)
+Requires-Dist: rich
+Requires-Dist: tomlkit (>=0.11.6,<0.12.0)
+Requires-Dist: typer[all]
+Description-Content-Type: text/markdown
 
-packages = \
-['timeturner', 'timeturner.tools']
+Time Turner
+===========
 
-package_data = \
-{'': ['*']}
+## A Minimalistic Time Tracker.
 
-install_requires = \
-['pendulum>=2.1.2,<3.0.0',
- 'pydantic>=1.10.5,<2.0.0',
- 'rich',
- 'tomlkit>=0.11.6,<0.12.0',
- 'typer[all]']
-
-entry_points = \
-{'console_scripts': ['timeturner = timeturner.run:entrypoint',
-                     'tt = timeturner.run:entrypoint']}
-
-setup_kwargs = {
-    'name': 'timeturner',
-    'version': '0.3.0a0',
-    'description': '',
-    'long_description': 'Time Turner\n===========\n\n## A Minimalistic Time Tracker.\n\nThis is a minimalistic time tracker that allows you to record when you start working, even if it is in the past, stop running activities now, and add activities from the past. It also ensures legal rest periods are included if you forgot to track them.\n\nIn the Harry Potter series, the Time-Turner is a magical device that allows the user to travel back in time. Time Turner is a time tracker that lets you "turn back time" and record activities from the past.\n\n**Warning, this is still an alpha release, the API is not stable yet.**\n\n## Usage\n\n### Starting an Activity\n\nTo start tracking an activity, run the following command:\n\n\n![`timeturner add`](img/add.svg)\n\nThis will record the current time as the start of your activity.\n\nIf you forgot to start tracking an activity yesterday, you can provide the start time with an additional parameter, `-10m` would mean 10 minutest ago. The full list of possible time values can be [seen further down](#examples-for-times)\n\n### Stopping an Activity\n\nTo stop tracking the current activity, run the following command:\n\n\n![`timeturner end`](img/end.svg)\n\n\nThis will record the current time as the end of your activity and calculate the total duration.\n\n### Adding a Past Activity\n\nIf you forgot to track an activity in the past, you can add it with `timeturner add <start_time> - <end_time>`\n\n![`timeturner add -- -1d@9:00 - +8h45m`](img/add_past.svg)\n\n### Adding a public holiday\n\nTo add May 1st as a public holiday, run the following command:\n\n![`timeturner add 05-01 @holiday`](img/add_holiday.svg)\n\n### Adding your vacation\n\nTo add your vacation, run the following command:\n\n![`timeturner add 04-25 - 05-14 @vacation`](img/add_vacation.svg)\n\nAdding your vacation will add a segments that are not part of holidays, it will also split\nweekends and only add working days as vacation.\n\n\n\n\n## Configuration\n\n| Environment Variable       | Default Value                    | Description                                  |\n| -------------------------- | -------------------------------- | -------------------------------------------- |\n| TIMETURNER_CONFIG_HOME     | ~/$XDG_CONFIG_HOME/timeturner    | The directory for configuration files.       |\n| TIMETURNER_CONFIG_FILE     | timeturner.toml                  | The configuration file to use.               |\n| TIMETURNER_DATABASE__HOME  | value of $TIMETURNER_CONFIG_HOME | The directory to store the database file in. |\n| TIMETURNER_DATABASE__FILE  | timeturner.db                    | The database file to use.                    |\n| TIMETURNER_DATABASE__TABLE | pensive                          | The table to use in the database.            |\n\n## Examples\n\n### Examples for times\n\n<start_time> or <end_time> could be one of the following Examples:\n\n| Example         | Description                               |\n| --------------- | ----------------------------------------- |\n|                 | now                                       |\n| 9:00            | 9:00 today                                |\n| -1m             | 1 minute ago                              |\n| -1h             | 1 hour ago                                |\n| -1d             | 1 day ago, you will be asked for the time |\n| -1d@9:00        | 1 day ago 9:00                            |\n| +1m             | 1 minute from now                         |\n| +1h             | 1 hour from now                           |\n| 12 7:00         | 7:00 on the 12th of the current month     |\n| 02-28 9:00      | 9:00 on February 28 of the current year   |\n| 2022-02-28 9:00 | 9:00 on February 28, 2022                 |\n\n\n\n### Automatic Rest Periods\n\nIf you forget to track a rest period, the time tracker will reduce the required rest period before showing it. For periods greater than 4h 15 are reducted, for periods greater than 6:15 additional 30m are reducted.\n\n\n\nTODOs:\n- [ ] Add Configuration\n  - [ ] ignore seconds\n  - [ ] freeze time, to generate useful and pretty images for docs\n  - [ ] automatic rest periods\n  - [ ] default work time\n  - [ ] default work week days\n- [ ] allow full day activities to coexist with other activities\n  - [ ] travel time and holiday could happen\n- [ ] DB migrations\n- [ ] show and generate tui output\n- [ ] Add section about contributions\n- [ ] Add precommit hook to ensure code is formatted\n- [ ] Generate docstrings for DB methods\n- [ ] Remove import command (it contains assumptions that will not be true for everyone)\n  - [ ] Document how to import data from other time trackers\n  - [ ] Add mode to convert hamster output to jsonl file.\n  - [ ] Add mode to import jsonl file\n- [ ] Add logging\n  - [ ] allow different log levels for database and application\n- [ ] add test that the last release version in Changelog is the same as in pyproject.toml and app\n- [ ] README\n  - [ ] auto generate config options\n\n\nTODOS by command:\n\n- [x] add\n\n- [ ] end\n  - [ ] add tests\n\n- [ ] configure\n  - [ ] modify and write configfile\n  - [ ] allow to add aliases for commands\n    - [ ] e.g. new new add alias with setting passive to true\n  - [ ] add test when holiday tag name is changed in settings\n\n- [ ] list\n  - [ ] split up multiday activities\n  - [ ] summaries full day tags differently\n  - [x] holidays should not count as work time\n    - [x] it should also not count as missing work time\n  - [ ] group by year, month, week, daysplit up multiday activities\n  - [ ] add option to show only open activities\n  - [ ] add tests\n\n- [ ] import holidays\n\n- [ ] export\n  - [ ] probably like list --format jsonl\n\n- [ ] undo (revert the last change)\n- [ ] confirm changes that would modify other entries\n\n### Design Goals\n\n- minimalistic, little to type\n- enforce as little as possible\n- be clear\n- be extensible\n  - TODO: support plugins (maybe a later version)\n  - be able to use it programmatically\n  - be able to use it as a library\n\n\n### Open Questions\n\n- [ ] should the get_latest_segment return segments from the future (start_time in the future)?\n\n### Nice to have:\n- [ ] Build a minimal Docker image (maybe)\n- [ ] https://github.com/ines/termynal\n',
-    'author': 'Olaf Gladis',
-    'author_email': 'olaf@gladis.org',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
-}
+This is a minimalistic time tracker that allows you to record when you start working, even if it is in the past, stop running activities now, and add activities from the past. It also ensures legal rest periods are included if you forgot to track them.
 
+In the Harry Potter series, the Time-Turner is a magical device that allows the user to travel back in time. Time Turner is a time tracker that lets you "turn back time" and record activities from the past.
+
+**Warning, this is still an alpha release, the API is not stable yet.**
+
+## Usage
+
+### Starting an Activity
+
+To start tracking an activity, run the following command:
+
+
+![`timeturner add`](img/add.svg)
+
+This will record the current time as the start of your activity.
+
+If you forgot to start tracking an activity yesterday, you can provide the start time with an additional parameter, `-10m` would mean 10 minutest ago. The full list of possible time values can be [seen further down](#examples-for-times)
+
+### Stopping an Activity
+
+To stop tracking the current activity, run the following command:
+
+
+![`timeturner end`](img/end.svg)
+
+
+This will record the current time as the end of your activity and calculate the total duration.
+
+### Adding a Past Activity
+
+If you forgot to track an activity in the past, you can add it with `timeturner add <start_time> - <end_time>`
+
+![`timeturner add -- -1d@9:00 - +8h45m`](img/add_past.svg)
+
+### Adding a public holiday
+
+To add May 1st as a public holiday, run the following command:
+
+![`timeturner add 05-01 @holiday`](img/add_holiday.svg)
+
+### Adding your vacation
+
+To add your vacation, run the following command:
+
+![`timeturner add 04-25 - 05-14 @vacation`](img/add_vacation.svg)
+
+Adding your vacation will add a segments that are not part of holidays, it will also split
+weekends and only add working days as vacation.
+
+
+
+
+## Configuration
+
+| Environment Variable       | Default Value                    | Description                                  |
+| -------------------------- | -------------------------------- | -------------------------------------------- |
+| TIMETURNER_CONFIG_HOME     | ~/$XDG_CONFIG_HOME/timeturner    | The directory for configuration files.       |
+| TIMETURNER_CONFIG_FILE     | timeturner.toml                  | The configuration file to use.               |
+| TIMETURNER_DATABASE__HOME  | value of $TIMETURNER_CONFIG_HOME | The directory to store the database file in. |
+| TIMETURNER_DATABASE__FILE  | timeturner.db                    | The database file to use.                    |
+| TIMETURNER_DATABASE__TABLE | pensive                          | The table to use in the database.            |
+
+## Examples
+
+### Examples for times
+
+<start_time> or <end_time> could be one of the following Examples:
+
+| Example         | Description                               |
+| --------------- | ----------------------------------------- |
+|                 | now                                       |
+| 9:00            | 9:00 today                                |
+| -1m             | 1 minute ago                              |
+| -1h             | 1 hour ago                                |
+| -1d             | 1 day ago, you will be asked for the time |
+| -1d@9:00        | 1 day ago 9:00                            |
+| +1m             | 1 minute from now                         |
+| +1h             | 1 hour from now                           |
+| 12 7:00         | 7:00 on the 12th of the current month     |
+| 02-28 9:00      | 9:00 on February 28 of the current year   |
+| 2022-02-28 9:00 | 9:00 on February 28, 2022                 |
+
+
+
+### Automatic Rest Periods
+
+If you forget to track a rest period, the time tracker will reduce the required rest period before showing it. For periods greater than 4h 15 are reducted, for periods greater than 6:15 additional 30m are reducted.
+
+
+
+TODOs:
+- [ ] Add Configuration
+  - [ ] ignore seconds
+  - [ ] freeze time, to generate useful and pretty images for docs
+  - [ ] automatic rest periods
+  - [ ] default work time
+  - [ ] default work week days
+- [ ] allow full day activities to coexist with other activities
+  - [ ] travel time and holiday could happen
+- [ ] DB migrations
+- [ ] show and generate tui output
+- [ ] Add section about contributions
+- [ ] Add precommit hook to ensure code is formatted
+- [ ] Generate docstrings for DB methods
+- [ ] Remove import command (it contains assumptions that will not be true for everyone)
+  - [ ] Document how to import data from other time trackers
+  - [ ] Add mode to convert hamster output to jsonl file.
+  - [ ] Add mode to import jsonl file
+- [ ] Add logging
+  - [ ] allow different log levels for database and application
+- [ ] add test that the last release version in Changelog is the same as in pyproject.toml and app
+- [ ] README
+  - [ ] auto generate config options
+
+
+TODOS by command:
+
+- [x] add
+
+- [ ] end
+  - [ ] add tests
+
+- [ ] configure
+  - [ ] modify and write configfile
+  - [ ] allow to add aliases for commands
+    - [ ] e.g. new new add alias with setting passive to true
+  - [ ] add test when holiday tag name is changed in settings
+
+- [ ] list
+  - [ ] split up multiday activities
+  - [ ] summaries full day tags differently
+  - [x] holidays should not count as work time
+    - [x] it should also not count as missing work time
+  - [ ] group by year, month, week, daysplit up multiday activities
+  - [ ] add option to show only open activities
+  - [ ] add tests
+  - [ ] MM-DD or YYYY-MM-DD should only show show a single day
+
+- [ ] import holidays
+
+- [ ] export
+  - [ ] probably like list --format jsonl
+
+- [ ] undo (revert the last change)
+- [ ] confirm changes that would modify other entries
+
+### Design Goals
+
+- minimalistic, little to type
+- enforce as little as possible
+- be clear
+- be extensible
+  - TODO: support plugins (maybe a later version)
+  - be able to use it programmatically
+  - be able to use it as a library
+
+
+### Open Questions
+
+- [ ] should the get_latest_segment return segments from the future (start_time in the future)?
+
+### Nice to have:
+- [ ] Build a minimal Docker image (maybe)
+- [ ] https://github.com/ines/termynal
 
-setup(**setup_kwargs)
```

