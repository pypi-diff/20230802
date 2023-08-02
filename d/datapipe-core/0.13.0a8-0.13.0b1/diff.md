# Comparing `tmp/datapipe_core-0.13.0a8.tar.gz` & `tmp/datapipe_core-0.13.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datapipe_core-0.13.0a8.tar", max compression
+gzip compressed data, was "datapipe_core-0.13.0b1.tar", max compression
```

## Comparing `datapipe_core-0.13.0a8.tar` & `datapipe_core-0.13.0b1.tar`

### file list

```diff
@@ -1,26 +1,29 @@
--rw-r--r--   0        0        0     1514 2022-12-26 14:30:45.008686 datapipe_core-0.13.0a8/LICENSE
--rw-r--r--   0        0        0      779 2023-07-30 16:02:08.285417 datapipe_core-0.13.0a8/README.md
--rw-r--r--   0        0        0        0 2023-05-29 09:25:17.932322 datapipe_core-0.13.0a8/datapipe/__init__.py
--rw-r--r--   0        0        0    16161 2023-07-31 17:04:18.495884 datapipe_core-0.13.0a8/datapipe/cli.py
--rw-r--r--   0        0        0     9520 2023-07-30 17:16:08.720825 datapipe_core-0.13.0a8/datapipe/compute.py
--rw-r--r--   0        0        0    37565 2023-07-31 17:04:18.495884 datapipe_core-0.13.0a8/datapipe/core_steps.py
--rw-r--r--   0        0        0     6780 2023-07-30 16:03:27.685421 datapipe_core-0.13.0a8/datapipe/datatable.py
--rw-r--r--   0        0        0     4649 2023-07-31 17:04:18.495884 datapipe_core-0.13.0a8/datapipe/event_logger.py
--rw-r--r--   0        0        0     1628 2023-07-30 17:16:08.720825 datapipe_core-0.13.0a8/datapipe/executor/__init__.py
--rw-r--r--   0        0        0     2183 2023-07-30 17:16:08.720825 datapipe_core-0.13.0a8/datapipe/executor/ray.py
--rw-r--r--   0        0        0     4236 2023-07-30 17:16:08.720825 datapipe_core-0.13.0a8/datapipe/lints.py
--rw-r--r--   0        0        0    22222 2023-07-30 17:16:08.720825 datapipe_core-0.13.0a8/datapipe/metastore.py
--rw-r--r--   0        0        0        0 2023-07-31 17:04:18.495884 datapipe_core-0.13.0a8/datapipe/migrations/__init__.py
--rw-r--r--   0        0        0     3071 2023-07-31 17:04:18.495884 datapipe_core-0.13.0a8/datapipe/migrations/v013.py
--rw-r--r--   0        0        0      969 2023-07-30 16:08:00.215417 datapipe_core-0.13.0a8/datapipe/run_config.py
--rw-r--r--   0        0        0        0 2022-12-26 14:30:45.008686 datapipe_core-0.13.0a8/datapipe/store/__init__.py
--rw-r--r--   0        0        0     8435 2023-07-30 16:02:08.295417 datapipe_core-0.13.0a8/datapipe/store/database.py
--rw-r--r--   0        0        0    18238 2023-07-30 16:02:08.295417 datapipe_core-0.13.0a8/datapipe/store/filedir.py
--rw-r--r--   0        0        0     3595 2023-07-30 16:02:08.295417 datapipe_core-0.13.0a8/datapipe/store/milvus.py
--rw-r--r--   0        0        0     1337 2023-07-30 16:02:08.295417 datapipe_core-0.13.0a8/datapipe/store/pandas.py
--rw-r--r--   0        0        0     8674 2023-07-30 16:02:08.295417 datapipe_core-0.13.0a8/datapipe/store/qdrant.py
--rw-r--r--   0        0        0     3209 2023-07-30 16:02:08.295417 datapipe_core-0.13.0a8/datapipe/store/redis.py
--rw-r--r--   0        0        0     3877 2023-03-18 21:02:58.537544 datapipe_core-0.13.0a8/datapipe/store/table_store.py
--rw-r--r--   0        0        0     9945 2023-07-30 16:08:03.355417 datapipe_core-0.13.0a8/datapipe/types.py
--rw-r--r--   0        0        0     2145 2023-07-31 17:04:18.495884 datapipe_core-0.13.0a8/pyproject.toml
--rw-r--r--   0        0        0     3008 1970-01-01 00:00:00.000000 datapipe_core-0.13.0a8/PKG-INFO
+-rw-r--r--   0        0        0     1514 2022-12-26 14:30:45.008686 datapipe_core-0.13.0b1/LICENSE
+-rw-r--r--   0        0        0      779 2023-07-30 16:02:08.285417 datapipe_core-0.13.0b1/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 09:25:17.932322 datapipe_core-0.13.0b1/datapipe/__init__.py
+-rw-r--r--   0        0        0    16171 2023-08-02 18:09:28.809171 datapipe_core-0.13.0b1/datapipe/cli.py
+-rw-r--r--   0        0        0     9435 2023-08-02 18:09:28.809171 datapipe_core-0.13.0b1/datapipe/compute.py
+-rw-r--r--   0        0        0    23521 2023-08-02 18:09:28.809171 datapipe_core-0.13.0b1/datapipe/datatable.py
+-rw-r--r--   0        0        0     4649 2023-07-31 17:04:18.495884 datapipe_core-0.13.0b1/datapipe/event_logger.py
+-rw-r--r--   0        0        0     1628 2023-07-30 17:16:08.720825 datapipe_core-0.13.0b1/datapipe/executor/__init__.py
+-rw-r--r--   0        0        0     2183 2023-07-30 17:16:08.720825 datapipe_core-0.13.0b1/datapipe/executor/ray.py
+-rw-r--r--   0        0        0     4236 2023-07-30 17:16:08.720825 datapipe_core-0.13.0b1/datapipe/lints.py
+-rw-r--r--   0        0        0        0 2023-07-31 17:04:18.495884 datapipe_core-0.13.0b1/datapipe/migrations/__init__.py
+-rw-r--r--   0        0        0     3081 2023-08-02 18:09:28.809171 datapipe_core-0.13.0b1/datapipe/migrations/v013.py
+-rw-r--r--   0        0        0      969 2023-08-01 20:24:08.421185 datapipe_core-0.13.0b1/datapipe/run_config.py
+-rw-r--r--   0        0        0        0 2023-08-02 18:09:28.809171 datapipe_core-0.13.0b1/datapipe/step/__init__.py
+-rw-r--r--   0        0        0     3667 2023-08-02 18:09:28.809171 datapipe_core-0.13.0b1/datapipe/step/batch_generate.py
+-rw-r--r--   0        0        0    34123 2023-08-02 18:09:28.809171 datapipe_core-0.13.0b1/datapipe/step/batch_transform.py
+-rw-r--r--   0        0        0     3680 2023-08-02 18:09:28.809171 datapipe_core-0.13.0b1/datapipe/step/datatable_transform.py
+-rw-r--r--   0        0        0     2532 2023-08-02 18:09:28.809171 datapipe_core-0.13.0b1/datapipe/step/update_external_table.py
+-rw-r--r--   0        0        0        0 2022-12-26 14:30:45.008686 datapipe_core-0.13.0b1/datapipe/store/__init__.py
+-rw-r--r--   0        0        0     8435 2023-07-30 16:02:08.295417 datapipe_core-0.13.0b1/datapipe/store/database.py
+-rw-r--r--   0        0        0    18254 2023-08-02 18:09:28.809171 datapipe_core-0.13.0b1/datapipe/store/filedir.py
+-rw-r--r--   0        0        0     3595 2023-07-30 16:02:08.295417 datapipe_core-0.13.0b1/datapipe/store/milvus.py
+-rw-r--r--   0        0        0     1337 2023-07-30 16:02:08.295417 datapipe_core-0.13.0b1/datapipe/store/pandas.py
+-rw-r--r--   0        0        0     8674 2023-07-30 16:02:08.295417 datapipe_core-0.13.0b1/datapipe/store/qdrant.py
+-rw-r--r--   0        0        0     3209 2023-07-30 16:02:08.295417 datapipe_core-0.13.0b1/datapipe/store/redis.py
+-rw-r--r--   0        0        0     3877 2023-03-18 21:02:58.537544 datapipe_core-0.13.0b1/datapipe/store/table_store.py
+-rw-r--r--   0        0        0    10104 2023-08-02 18:09:28.809171 datapipe_core-0.13.0b1/datapipe/types.py
+-rw-r--r--   0        0        0     2144 2023-08-02 18:09:28.809171 datapipe_core-0.13.0b1/pyproject.toml
+-rw-r--r--   0        0        0     3008 1970-01-01 00:00:00.000000 datapipe_core-0.13.0b1/PKG-INFO
```

### Comparing `datapipe_core-0.13.0a8/LICENSE` & `datapipe_core-0.13.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a8/README.md` & `datapipe_core-0.13.0b1/README.md`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a8/datapipe/cli.py` & `datapipe_core-0.13.0b1/datapipe/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 from opentelemetry.sdk.resources import SERVICE_NAME, Resource
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor, ConsoleSpanExporter
 from rich import print as rprint
 from tqdm_loggable.auto import tqdm
 
 from datapipe.compute import ComputeStep, DatapipeApp, run_steps, run_steps_changelist
-from datapipe.core_steps import BaseBatchTransformStep
 from datapipe.executor import Executor, SingleThreadExecutor
 from datapipe.migrations import v013 as migrations_v013
+from datapipe.step.batch_transform import BaseBatchTransformStep
 from datapipe.types import IndexDF, Labels
 
 tracer = trace.get_tracer("datapipe_app")
 
 rich.reconfigure(highlight=False)
```

### Comparing `datapipe_core-0.13.0a8/datapipe/compute.py` & `datapipe_core-0.13.0b1/datapipe/compute.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import hashlib
 import logging
-import time
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Dict, Iterable, List, Optional, Tuple
 
 from opentelemetry import trace
-from tqdm_loggable.auto import tqdm
 
 from datapipe.datatable import DataStore, DataTable
-from datapipe.executor import Executor, ExecutorConfig, SingleThreadExecutor
+from datapipe.executor import Executor, ExecutorConfig
 from datapipe.run_config import RunConfig
 from datapipe.store.table_store import TableStore
-from datapipe.types import ChangeList, DataDF, IndexDF, Labels, TransformResult
+from datapipe.types import ChangeList, IndexDF, Labels
 
 logger = logging.getLogger("datapipe.compute")
 tracer = trace.get_tracer("datapipe.compute")
 
 
 @dataclass
 class Table:
@@ -259,15 +257,15 @@
     ds: DataStore,
     steps: List[ComputeStep],
     changelist: ChangeList,
     run_config: Optional[RunConfig] = None,
     executor: Optional[Executor] = None,
 ) -> None:
     # FIXME extract Batch* steps to separate module
-    from datapipe.core_steps import BaseBatchTransformStep
+    from datapipe.step.batch_transform import BaseBatchTransformStep
 
     current_changes = changelist
     next_changes = ChangeList()
     iteration = 0
 
     with tracer.start_as_current_span("Start pipeline for changelist"):
         while not current_changes.empty() and iteration < 100:
```

### Comparing `datapipe_core-0.13.0a8/datapipe/core_steps.py` & `datapipe_core-0.13.0b1/datapipe/step/batch_transform.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,74 +6,66 @@
 import time
 from dataclasses import dataclass
 from typing import (
     Any,
     Callable,
     Dict,
     Iterable,
-    Iterator,
     List,
     Literal,
     Optional,
     Protocol,
     Tuple,
     Union,
     cast,
 )
 
 import pandas as pd
 from opentelemetry import trace
 from sqlalchemy import (
+    Boolean,
+    Column,
+    Float,
+    Integer,
+    String,
+    Table,
     alias,
     and_,
     asc,
     column,
     desc,
     func,
     literal,
     or_,
     select,
     tuple_,
+    update,
 )
+from sqlalchemy.sql.expression import select
 from tqdm_loggable.auto import tqdm
 
 from datapipe.compute import Catalog, ComputeStep, PipelineStep
-from datapipe.datatable import DataStore, DataTable
+from datapipe.datatable import DataStore, DataTable, MetaTable
 from datapipe.executor import Executor, ExecutorConfig, SingleThreadExecutor
-from datapipe.metastore import MetaTable, TransformMetaTable
 from datapipe.run_config import LabelDict, RunConfig
-from datapipe.store.database import sql_apply_runconfig_filter
+from datapipe.store.database import DBConn, sql_apply_runconfig_filter
 from datapipe.types import (
     ChangeList,
     DataDF,
+    DataSchema,
     IndexDF,
     Labels,
     MetaSchema,
     TransformResult,
     data_to_index,
     get_tables_that_have_different_intersections,
 )
 
-logger = logging.getLogger("datapipe.core_steps")
-tracer = trace.get_tracer("datapipe.core_steps")
-
-
-class DatatableTransformFunc(Protocol):
-    __name__: str
-
-    def __call__(
-        self,
-        ds: DataStore,
-        input_dts: List[DataTable],
-        output_dts: List[DataTable],
-        run_config: Optional[RunConfig],
-        # Возможно, лучше передавать как переменную, а не  **
-        **kwargs,
-    ) -> None:
-        ...
+logger = logging.getLogger("datapipe.step.batch_transform")
+tracer = trace.get_tracer("datapipe.step.batch_transform")
 
 
 # TODO подумать, может быть мы хотим дать возможность возвращать итератор TransformResult
 class DatatableBatchTransformFunc(Protocol):
     __name__: str
 
     def __call__(
@@ -83,106 +75,185 @@
         input_dts: List[DataTable],
         run_config: Optional[RunConfig] = None,
         kwargs: Optional[Dict[str, Any]] = None,
     ) -> TransformResult:
         ...
 
 
-# TODO подумать, может быть мы хотим дать возможность возвращать итератор TransformResult
 BatchTransformFunc = Callable[..., TransformResult]
 
-BatchGenerateFunc = Callable[..., Iterator[TransformResult]]
-
-
-@dataclass
-class DatatableTransform(PipelineStep):
-    func: DatatableTransformFunc
-    inputs: List[str]
-    outputs: List[str]
-    check_for_changes: bool = True
-    kwargs: Optional[Dict[str, Any]] = None
-    labels: Optional[Labels] = None
 
-    def build_compute(self, ds: DataStore, catalog: Catalog) -> List["ComputeStep"]:
-        return [
-            DatatableTransformStep(
-                name=self.func.__name__,
-                input_dts=[catalog.get_datatable(ds, i) for i in self.inputs],
-                output_dts=[catalog.get_datatable(ds, i) for i in self.outputs],
-                func=self.func,
-                kwargs=self.kwargs,
-                check_for_changes=self.check_for_changes,
-                labels=self.labels,
-            )
-        ]
+TRANSFORM_META_SCHEMA: DataSchema = [
+    Column("process_ts", Float),  # Время последней успешной обработки
+    Column("is_success", Boolean),  # Успешно ли обработана строка
+    Column("priority", Integer),  # Приоритет обработки (чем больше, тем выше)
+    Column("error", String),  # Текст ошибки
+]
 
 
-class DatatableTransformStep(ComputeStep):
+class TransformMetaTable:
     def __init__(
         self,
+        dbconn: DBConn,
         name: str,
-        input_dts: List[DataTable],
-        output_dts: List[DataTable],
-        func: DatatableTransformFunc,
-        kwargs: Optional[Dict] = None,
-        check_for_changes: bool = True,
-        labels: Optional[Labels] = None,
+        primary_schema: DataSchema,
+        create_table: bool = False,
     ) -> None:
-        ComputeStep.__init__(self, name, input_dts, output_dts, labels)
+        self.dbconn = dbconn
+        self.name = name
+        self.primary_schema = primary_schema
+        self.primary_keys = [i.name for i in primary_schema]
+
+        self.sql_schema = [i.copy() for i in primary_schema + TRANSFORM_META_SCHEMA]  # type: ignore
+
+        self.sql_table = Table(
+            name,
+            dbconn.sqla_metadata,
+            *self.sql_schema,
+        )
 
-        self.func = func
-        self.kwargs = kwargs or {}
-        self.check_for_changes = check_for_changes
+        if create_table:
+            self.sql_table.create(self.dbconn.con, checkfirst=True)
 
-    def run_full(
+    def insert_rows(
         self,
-        ds: DataStore,
+        idx: IndexDF,
+    ) -> None:
+        """
+        Создает строки в таблице метаданных для указанных индексов. Если строки
+        уже существуют - не делает ничего.
+        """
+
+        idx = cast(IndexDF, idx[self.primary_keys])
+
+        insert_sql = self.dbconn.insert(self.sql_table).values(
+            [
+                {
+                    "process_ts": 0,
+                    "is_success": False,
+                    "priority": 0,
+                    "error": None,
+                    **idx_dict,  # type: ignore
+                }
+                for idx_dict in idx.to_dict(orient="records")
+            ]
+        )
+
+        sql = insert_sql.on_conflict_do_nothing(index_elements=self.primary_keys)
+
+        with self.dbconn.con.begin() as con:
+            con.execute(sql)
+
+    def mark_rows_processed_success(
+        self,
+        idx: IndexDF,
+        process_ts: float,
         run_config: Optional[RunConfig] = None,
-        executor: Optional[Executor] = None,
     ) -> None:
-        logger.info(f"Running: {self.name}")
+        idx = cast(
+            IndexDF, idx[self.primary_keys].drop_duplicates()
+        )  # FIXME: сделать в основном запросе distinct
+
+        insert_sql = self.dbconn.insert(self.sql_table).values(
+            [
+                {
+                    "process_ts": process_ts,
+                    "is_success": True,
+                    "priority": 0,
+                    "error": None,
+                    **idx_dict,  # type: ignore
+                }
+                for idx_dict in idx.to_dict(orient="records")
+            ]
+        )
 
-        # TODO implement "watermark" system for tracking computation status in DatatableTransform
-        #
-        # if len(self.input_dts) > 0 and self.check_for_changes:
-        #     with tracer.start_as_current_span("check for changes"):
-        #         changed_idx_count = ds.get_changed_idx_count(
-        #             inputs=self.input_dts,
-        #             outputs=self.output_dts,
-        #             run_config=run_config,
-        #         )
-
-        #         if changed_idx_count == 0:
-        #             logger.debug(
-        #                 f"Skipping {self.get_name()} execution - nothing to compute"
-        #             )
+        sql = insert_sql.on_conflict_do_update(
+            index_elements=self.primary_keys,
+            set_={
+                "process_ts": process_ts,
+                "is_success": True,
+                "error": None,
+            },
+        )
 
-        #             return
+        # execute
+        with self.dbconn.con.begin() as con:
+            con.execute(sql)
 
-        run_config = RunConfig.add_labels(run_config, {"step_name": self.get_name()})
+    def mark_rows_processed_error(
+        self,
+        idx: IndexDF,
+        process_ts: float,
+        error: str,
+        run_config: Optional[RunConfig] = None,
+    ) -> None:
+        idx = cast(
+            IndexDF, idx[self.primary_keys].drop_duplicates()
+        )  # FIXME: сделать в основном запросе distinct
+
+        insert_sql = self.dbconn.insert(self.sql_table).values(
+            [
+                {
+                    "process_ts": process_ts,
+                    "is_success": False,
+                    "priority": 0,
+                    "error": error,
+                    **idx_dict,  # type: ignore
+                }
+                for idx_dict in idx.to_dict(orient="records")
+            ]
+        )
 
-        with tracer.start_as_current_span(f"Run {self.func}"):
-            try:
-                self.func(
-                    ds=ds,
-                    input_dts=self.input_dts,
-                    output_dts=self.output_dts,
-                    run_config=run_config,
-                    kwargs=self.kwargs,
-                )
-            except Exception as e:
-                logger.error(f"Datatable transform ({self.func}) run failed: {str(e)}")
-                ds.event_logger.log_exception(e, run_config=run_config)
+        sql = insert_sql.on_conflict_do_update(
+            index_elements=self.primary_keys,
+            set_={
+                "process_ts": process_ts,
+                "is_success": False,
+                "error": error,
+            },
+        )
 
+        # execute
+        with self.dbconn.con.begin() as con:
+            con.execute(sql)
 
-def safe_func_name(func: Callable) -> str:
-    raw_name = func.__name__
-    if raw_name == "<lambda>":
-        return "lambda"
-    return raw_name
+    def get_metadata_size(self) -> int:
+        """
+        Получить количество строк метаданных трансформации.
+        """
+
+        sql = select([func.count()]).select_from(self.sql_table)
+        res = self.dbconn.con.execute(sql).fetchone()
+
+        assert res is not None and len(res) == 1
+        return res[0]
+
+    def mark_all_rows_unprocessed(
+        self,
+        run_config: Optional[RunConfig] = None,
+    ) -> None:
+        update_sql = (
+            update(self.sql_table)
+            .values(
+                {
+                    "process_ts": 0,
+                    "is_success": False,
+                    "error": None,
+                }
+            )
+            .where(self.sql_table.c.is_success == True)
+        )
+
+        sql = sql_apply_runconfig_filter(
+            update_sql, self.sql_table, self.primary_keys, run_config
+        )
+
+        # execute
+        with self.dbconn.con.begin() as con:
+            con.execute(sql)
 
 
 class BaseBatchTransformStep(ComputeStep):
     """
     Abstract class for batch transform steps
     """
 
@@ -985,166 +1056,7 @@
         kwargs = {
             **({"ds": ds} if "ds" in self.parameters else {}),
             **({"idx": idx} if "idx" in self.parameters else {}),
             **({"run_config": run_config} if "run_config" in self.parameters else {}),
             **(self.kwargs or {}),
         }
         return self.func(*input_dfs, **kwargs)
-
-
-def do_batch_generate(
-    func: BatchGenerateFunc,
-    ds: DataStore,
-    output_dts: List[DataTable],
-    run_config: Optional[RunConfig] = None,
-    kwargs: Optional[Dict] = None,
-) -> None:
-    import inspect
-
-    import pandas as pd
-
-    """
-    Создание новой таблицы из результатов запуска `proc_func`.
-    Функция может быть как обычной, так и генерирующейся
-    """
-
-    now = time.time()
-    empty_generator = True
-    parameters = inspect.signature(func).parameters
-    kwargs = {
-        **({"ds": ds} if "ds" in parameters else {}),
-        **(kwargs or {}),
-    }
-
-    assert inspect.isgeneratorfunction(
-        func
-    ), "Starting v0.8.0 proc_func should be a generator"
-
-    with tracer.start_as_current_span("init generator"):
-        try:
-            iterable = func(**kwargs or {})
-        except Exception as e:
-            # mypy bug: https://github.com/python/mypy/issues/10976
-            logger.exception(f"Generating failed ({func.__name__}): {str(e)}")  # type: ignore
-            ds.event_logger.log_exception(e, run_config=run_config)
-
-            raise e
-
-    while True:
-        with tracer.start_as_current_span("get next batch"):
-            try:
-                chunk_dfs = next(iterable)
-
-                if isinstance(chunk_dfs, pd.DataFrame):
-                    chunk_dfs = (chunk_dfs,)
-            except StopIteration:
-                break
-            except Exception as e:
-                logger.exception(f"Generating failed ({func}): {str(e)}")
-                ds.event_logger.log_exception(e, run_config=run_config)
-
-                # raise e
-                return
-
-        empty_generator = False
-
-        with tracer.start_as_current_span("store results"):
-            for k, dt_k in enumerate(output_dts):
-                dt_k.store_chunk(chunk_dfs[k], run_config=run_config)
-
-    with tracer.start_as_current_span("delete stale rows"):
-        for k, dt_k in enumerate(output_dts):
-            dt_k.delete_stale_by_process_ts(now, run_config=run_config)
-
-
-@dataclass
-class BatchGenerate(PipelineStep):
-    func: BatchGenerateFunc
-    outputs: List[str]
-    kwargs: Optional[Dict] = None
-    labels: Optional[Labels] = None
-
-    def build_compute(self, ds: DataStore, catalog: Catalog) -> List[ComputeStep]:
-        return [
-            DatatableTransformStep(
-                name=self.func.__name__,
-                func=cast(
-                    DatatableTransformFunc,
-                    lambda ds, input_dts, output_dts, run_config, kwargs: do_batch_generate(
-                        func=self.func,
-                        ds=ds,
-                        output_dts=output_dts,
-                        run_config=run_config,
-                        kwargs=kwargs,
-                    ),
-                ),
-                input_dts=[],
-                output_dts=[catalog.get_datatable(ds, name) for name in self.outputs],
-                check_for_changes=False,
-                kwargs=self.kwargs,
-                labels=self.labels,
-            )
-        ]
-
-
-def update_external_table(
-    ds: DataStore, table: DataTable, run_config: Optional[RunConfig] = None
-) -> None:
-    now = time.time()
-
-    for ps_df in tqdm(
-        table.table_store.read_rows_meta_pseudo_df(run_config=run_config)
-    ):
-        (
-            new_df,
-            changed_df,
-            new_meta_df,
-            changed_meta_df,
-        ) = table.meta_table.get_changes_for_store_chunk(ps_df, now=now)
-
-        # TODO switch to iterative store_chunk and table.sync_meta_by_process_ts
-
-        table.meta_table.insert_meta_for_store_chunk(new_meta_df)
-        table.meta_table.update_meta_for_store_chunk(changed_meta_df)
-
-    for stale_idx in table.meta_table.get_stale_idx(now, run_config=run_config):
-        logger.debug(f"Deleting {len(stale_idx.index)} rows from {table.name} data")
-        table.event_logger.log_state(
-            table.name,
-            added_count=0,
-            updated_count=0,
-            deleted_count=len(stale_idx),
-            processed_count=len(stale_idx),
-            run_config=run_config,
-        )
-
-        table.meta_table.mark_rows_deleted(stale_idx, now=now)
-
-
-class UpdateExternalTable(PipelineStep):
-    def __init__(
-        self,
-        output: str,
-        labels: Optional[Labels] = None,
-    ) -> None:
-        self.output_table_name = output
-        self.labels = labels
-
-    def build_compute(self, ds: DataStore, catalog: Catalog) -> List[ComputeStep]:
-        def transform_func(
-            ds: DataStore,
-            input_dts: List[DataTable],
-            output_dts: List[DataTable],
-            run_config: Optional[RunConfig],
-            **kwargs,
-        ):
-            return update_external_table(ds, output_dts[0], run_config)
-
-        return [
-            DatatableTransformStep(
-                name=f"update_{self.output_table_name}",
-                func=cast(DatatableTransformFunc, transform_func),
-                input_dts=[],
-                output_dts=[catalog.get_datatable(ds, self.output_table_name)],
-                labels=self.labels,
-            )
-        ]
```

### Comparing `datapipe_core-0.13.0a8/datapipe/event_logger.py` & `datapipe_core-0.13.0b1/datapipe/event_logger.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a8/datapipe/executor/__init__.py` & `datapipe_core-0.13.0b1/datapipe/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a8/datapipe/executor/ray.py` & `datapipe_core-0.13.0b1/datapipe/executor/ray.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a8/datapipe/lints.py` & `datapipe_core-0.13.0b1/datapipe/lints.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a8/datapipe/metastore.py` & `datapipe_core-0.13.0b1/datapipe/datatable.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 import copy
 import logging
 import math
 import time
 from dataclasses import dataclass
-from typing import Any, Iterator, List, Optional, Tuple, cast
+from typing import Any, Dict, Iterator, List, Optional, Tuple, cast
 
 import pandas as pd
 from cityhash import CityHash32
-from sqlalchemy import Boolean, Column, Float, Integer, String, Table, func, update
-from sqlalchemy.sql.expression import and_, delete, or_, select, text, tuple_
+from opentelemetry import trace
+from sqlalchemy import Column, Float, Integer, Table
+from sqlalchemy.sql.expression import and_, delete, func, or_, select, text, tuple_
 
+from datapipe.event_logger import EventLogger
 from datapipe.run_config import RunConfig
 from datapipe.store.database import (
     DBConn,
     MetaKey,
     sql_apply_idx_filter,
     sql_apply_runconfig_filter,
     sql_schema_to_sqltype,
 )
+from datapipe.store.table_store import TableStore
 from datapipe.types import (
     DataDF,
     DataSchema,
     IndexDF,
     MetadataDF,
     MetaSchema,
     TAnyDF,
     data_to_index,
+    index_difference,
 )
 
-logger = logging.getLogger("datapipe.metastore")
+logger = logging.getLogger("datapipe.datatable")
+tracer = trace.get_tracer("datapipe.datatable")
+
 
 TABLE_META_SCHEMA = [
     Column("hash", Integer),
     Column("create_ts", Float),  # Время создания строки
     Column("update_ts", Float),  # Время последнего изменения
     Column("process_ts", Float),  # Время последней успешной обработки
     Column("delete_ts", Float),  # Время удаления
@@ -481,175 +487,183 @@
         with self.dbconn.con.begin() as con:
             return cast(
                 Iterator[IndexDF],
                 list(pd.read_sql_query(sql, con=con, chunksize=1000)),
             )
 
 
-TRANSFORM_META_SCHEMA = [
-    Column("process_ts", Float),  # Время последней успешной обработки
-    Column("is_success", Boolean),  # Успешно ли обработана строка
-    Column("priority", Integer),  # Приоритет обработки (чем больше, тем выше)
-    Column("error", String),  # Текст ошибки
-]
-
-
-class TransformMetaTable:
+class DataTable:
     def __init__(
         self,
-        dbconn: DBConn,
         name: str,
-        primary_schema: DataSchema,
-        create_table: bool = False,
-    ) -> None:
-        self.dbconn = dbconn
+        meta_dbconn: DBConn,
+        meta_table: MetaTable,
+        table_store: TableStore,
+        event_logger: EventLogger,
+    ):
         self.name = name
-        self.primary_schema = primary_schema
-        self.primary_keys = [i.name for i in primary_schema]
-
-        self.sql_schema = [i.copy() for i in primary_schema + TRANSFORM_META_SCHEMA]  # type: ignore
-
-        self.sql_table = Table(
-            name,
-            dbconn.sqla_metadata,
-            *self.sql_schema,
-        )
+        self.meta_dbconn = meta_dbconn
+        self.meta_table = meta_table
+        self.table_store = table_store
+        self.event_logger = event_logger
+
+        self.primary_schema = meta_table.primary_schema
+        self.primary_keys = meta_table.primary_keys
+
+    def get_metadata(self, idx: Optional[IndexDF] = None) -> MetadataDF:
+        return self.meta_table.get_metadata(idx)
+
+    def get_data(self, idx: Optional[IndexDF] = None) -> DataDF:
+        return self.table_store.read_rows(self.meta_table.get_existing_idx(idx))
+
+    def reset_metadata(self):
+        with self.meta_dbconn.con.begin() as con:
+            con.execute(
+                self.meta_table.sql_table.update().values(process_ts=0, update_ts=0)
+            )
 
-        if create_table:
-            self.sql_table.create(self.dbconn.con, checkfirst=True)
+    def get_size(self) -> int:
+        """
+        Get the number of non-deleted rows in the DataTable
+        """
+        return self.meta_table.get_metadata_size(idx=None, include_deleted=False)
 
-    def insert_rows(
+    def store_chunk(
         self,
-        idx: IndexDF,
-    ) -> None:
+        data_df: DataDF,
+        processed_idx: Optional[IndexDF] = None,
+        now: Optional[float] = None,
+        run_config: Optional[RunConfig] = None,
+    ) -> IndexDF:
         """
-        Создает строки в таблице метаданных для указанных индексов. Если строки
-        уже существуют - не делает ничего.
+        Записать новые данные в таблицу.
+
+        При указанном `processed_idx` удалить те строки, которые находятся
+        внутри `processed_idx`, но отсутствуют в `data_df`.
         """
 
-        idx = cast(IndexDF, idx[self.primary_keys])
+        # In case `processed_idx` is not None, check that it contains any of
+        # relevant columns
+        if processed_idx is not None:
+            relevant_keys = set(self.primary_keys) & set(processed_idx.columns)
+            if not relevant_keys:
+                processed_idx = None
 
-        insert_sql = self.dbconn.insert(self.sql_table).values(
-            [
-                {
-                    "process_ts": 0,
-                    "is_success": False,
-                    "priority": 0,
-                    "error": None,
-                    **idx_dict,  # type: ignore
-                }
-                for idx_dict in idx.to_dict(orient="records")
-            ]
-        )
+        # Check that all index values in `data_df` is unique
+        if data_df.duplicated(self.primary_keys).any():
+            raise ValueError("`data_df` index values should be unique")
 
-        sql = insert_sql.on_conflict_do_nothing(index_elements=self.primary_keys)
+        changes = [IndexDF(pd.DataFrame(columns=self.primary_keys))]
 
-        with self.dbconn.con.begin() as con:
-            con.execute(sql)
+        with tracer.start_as_current_span(f"{self.name} store_chunk"):
+            if not data_df.empty:
+                logger.debug(
+                    f"Inserting chunk {len(data_df.index)} rows into {self.name}"
+                )
 
-    def mark_rows_processed_success(
+                with tracer.start_as_current_span("get_changes_for_store_chunk"):
+                    (
+                        new_df,
+                        changed_df,
+                        new_meta_df,
+                        changed_meta_df,
+                    ) = self.meta_table.get_changes_for_store_chunk(data_df, now)
+
+                # TODO implement transaction meckanism
+                with tracer.start_as_current_span("store data"):
+                    self.table_store.insert_rows(new_df)
+                    self.table_store.update_rows(changed_df)
+
+                with tracer.start_as_current_span("store metadata"):
+                    self.meta_table.insert_meta_for_store_chunk(new_meta_df)
+                    self.meta_table.update_meta_for_store_chunk(changed_meta_df)
+
+                    changes.append(data_to_index(new_df, self.primary_keys))
+                    changes.append(data_to_index(changed_df, self.primary_keys))
+            else:
+                data_df = pd.DataFrame(columns=self.primary_keys)
+
+            with tracer.start_as_current_span("cleanup deleted rows"):
+                data_idx = data_to_index(data_df, self.primary_keys)
+
+                if processed_idx is not None:
+                    existing_idx = self.meta_table.get_existing_idx(processed_idx)
+                    deleted_idx = index_difference(existing_idx, data_idx)
+
+                    self.delete_by_idx(deleted_idx, now=now, run_config=run_config)
+
+                    changes.append(deleted_idx)
+
+        return cast(IndexDF, pd.concat(changes))
+
+    def delete_by_idx(
         self,
         idx: IndexDF,
-        process_ts: float,
+        now: Optional[float] = None,
         run_config: Optional[RunConfig] = None,
     ) -> None:
-        idx = cast(
-            IndexDF, idx[self.primary_keys].drop_duplicates()
-        )  # FIXME: сделать в основном запросе distinct
-
-        insert_sql = self.dbconn.insert(self.sql_table).values(
-            [
-                {
-                    "process_ts": process_ts,
-                    "is_success": True,
-                    "priority": 0,
-                    "error": None,
-                    **idx_dict,  # type: ignore
-                }
-                for idx_dict in idx.to_dict(orient="records")
-            ]
-        )
-
-        sql = insert_sql.on_conflict_do_update(
-            index_elements=self.primary_keys,
-            set_={
-                "process_ts": process_ts,
-                "is_success": True,
-                "error": None,
-            },
-        )
+        if len(idx) > 0:
+            logger.debug(f"Deleting {len(idx.index)} rows from {self.name} data")
 
-        # execute
-        with self.dbconn.con.begin() as con:
-            con.execute(sql)
+            self.table_store.delete_rows(idx)
+            self.meta_table.mark_rows_deleted(idx, now=now)
 
-    def mark_rows_processed_error(
+    def delete_stale_by_process_ts(
         self,
-        idx: IndexDF,
         process_ts: float,
-        error: str,
+        now: Optional[float] = None,
         run_config: Optional[RunConfig] = None,
     ) -> None:
-        idx = cast(
-            IndexDF, idx[self.primary_keys].drop_duplicates()
-        )  # FIXME: сделать в основном запросе distinct
-
-        insert_sql = self.dbconn.insert(self.sql_table).values(
-            [
-                {
-                    "process_ts": process_ts,
-                    "is_success": False,
-                    "priority": 0,
-                    "error": error,
-                    **idx_dict,  # type: ignore
-                }
-                for idx_dict in idx.to_dict(orient="records")
-            ]
-        )
-
-        sql = insert_sql.on_conflict_do_update(
-            index_elements=self.primary_keys,
-            set_={
-                "process_ts": process_ts,
-                "is_success": False,
-                "error": error,
-            },
-        )
+        for deleted_df in self.meta_table.get_stale_idx(
+            process_ts, run_config=run_config
+        ):
+            deleted_idx = data_to_index(deleted_df, self.primary_keys)
 
-        # execute
-        with self.dbconn.con.begin() as con:
-            con.execute(sql)
+            self.delete_by_idx(deleted_idx, now=now, run_config=run_config)
 
-    def get_metadata_size(self) -> int:
-        """
-        Получить количество строк метаданных трансформации.
-        """
 
-        sql = select([func.count()]).select_from(self.sql_table)
-        res = self.dbconn.con.execute(sql).fetchone()
-
-        assert res is not None and len(res) == 1
-        return res[0]
-
-    def mark_all_rows_unprocessed(
+class DataStore:
+    def __init__(
         self,
-        run_config: Optional[RunConfig] = None,
+        meta_dbconn: DBConn,
+        create_meta_table: bool = False,
     ) -> None:
-        update_sql = (
-            update(self.sql_table)
-            .values(
-                {
-                    "process_ts": 0,
-                    "is_success": False,
-                    "error": None,
-                }
-            )
-            .where(self.sql_table.c.is_success == True)
+        self.meta_dbconn = meta_dbconn
+        self.event_logger = EventLogger(
+            self.meta_dbconn, create_table=create_meta_table
         )
+        self.tables: Dict[str, DataTable] = {}
 
-        sql = sql_apply_runconfig_filter(
-            update_sql, self.sql_table, self.primary_keys, run_config
+        self.create_meta_table = create_meta_table
+
+    def create_table(self, name: str, table_store: TableStore) -> DataTable:
+        assert name not in self.tables
+
+        primary_schema = table_store.get_primary_schema()
+        meta_schema = table_store.get_meta_schema()
+
+        res = DataTable(
+            name=name,
+            meta_dbconn=self.meta_dbconn,
+            meta_table=MetaTable(
+                dbconn=self.meta_dbconn,
+                name=name,
+                primary_schema=primary_schema,
+                meta_schema=meta_schema,
+                create_table=self.create_meta_table,
+            ),
+            table_store=table_store,
+            event_logger=self.event_logger,
         )
 
-        # execute
-        with self.dbconn.con.begin() as con:
-            con.execute(sql)
+        self.tables[name] = res
+
+        return res
+
+    def get_or_create_table(self, name: str, table_store: TableStore) -> DataTable:
+        if name in self.tables:
+            return self.tables[name]
+        else:
+            return self.create_table(name, table_store)
+
+    def get_table(self, name: str) -> DataTable:
+        return self.tables[name]
```

### Comparing `datapipe_core-0.13.0a8/datapipe/migrations/v013.py` & `datapipe_core-0.13.0b1/datapipe/migrations/v013.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from rich import print as rprint
 from sqlalchemy import insert, literal
 from sqlalchemy.sql import and_, func, select
 
-from datapipe.core_steps import BaseBatchTransformStep
+from datapipe.step.batch_transform import BaseBatchTransformStep
 
 
 def migrate_transform_tables(app, steps):
     for batch_transform in steps:
         if not isinstance(batch_transform, BaseBatchTransformStep):
             continue
```

### Comparing `datapipe_core-0.13.0a8/datapipe/run_config.py` & `datapipe_core-0.13.0b1/datapipe/run_config.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a8/datapipe/store/database.py` & `datapipe_core-0.13.0b1/datapipe/store/database.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a8/datapipe/store/filedir.py` & `datapipe_core-0.13.0b1/datapipe/store/filedir.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,15 @@
             self.primary_schema = primary_schema
         else:
             self.primary_schema = [
                 Column(attrname, String, primary_key=True)
                 for attrname in self.attrnames
             ]
         self.attrname_to_cls = {
-            column.name: type_to_cls[type(column.type)]
+            column.name: type_to_cls[type(column.type)]  # type: ignore
             for column in self.primary_schema
         }
 
     def get_primary_schema(self) -> DataSchema:
         return self.primary_schema
 
     def get_meta_schema(self) -> MetaSchema:
```

### Comparing `datapipe_core-0.13.0a8/datapipe/store/milvus.py` & `datapipe_core-0.13.0b1/datapipe/store/milvus.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a8/datapipe/store/pandas.py` & `datapipe_core-0.13.0b1/datapipe/store/pandas.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a8/datapipe/store/qdrant.py` & `datapipe_core-0.13.0b1/datapipe/store/qdrant.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a8/datapipe/store/redis.py` & `datapipe_core-0.13.0b1/datapipe/store/redis.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a8/datapipe/store/table_store.py` & `datapipe_core-0.13.0b1/datapipe/store/table_store.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a8/datapipe/types.py` & `datapipe_core-0.13.0b1/datapipe/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations  # NOQA
 
 import itertools
 from dataclasses import dataclass, field
-from typing import Dict, List, NewType, Set, Tuple, TypeVar, Union, cast
+from typing import Callable, Dict, List, NewType, Set, Tuple, TypeVar, Union, cast
 
 import pandas as pd
 from sqlalchemy import Column
 
 DataSchema = List[Column]
 MetaSchema = List[Column]
 
@@ -261,7 +261,14 @@
         if (
             non_empty_sets_intersection is not None
             and len(non_empty_sets_intersection) == 0
         ):
             raise ValueError(f"Table {table_name} has bad intersection with tables.")
 
     return all_equalience_tables
+
+
+def safe_func_name(func: Callable) -> str:
+    raw_name = func.__name__
+    if raw_name == "<lambda>":
+        return "lambda"
+    return raw_name
```

### Comparing `datapipe_core-0.13.0a8/pyproject.toml` & `datapipe_core-0.13.0b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datapipe-core"
-version = "0.13.0-alpha.8"
+version = "0.13.0-beta.1"
 description = "`datapipe` is a realtime incremental ETL library for Python application"
 readme = "README.md"
 repository = "https://github.com/epoch8/datapipe"
 authors = ["Andrey Tatarinov <a@tatarinov.co>"]
 packages = [
     { include = "datapipe" }
 ]
```

### Comparing `datapipe_core-0.13.0a8/PKG-INFO` & `datapipe_core-0.13.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapipe-core
-Version: 0.13.0a8
+Version: 0.13.0b1
 Summary: `datapipe` is a realtime incremental ETL library for Python application
 Home-page: https://github.com/epoch8/datapipe
 Author: Andrey Tatarinov
 Author-email: a@tatarinov.co
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

