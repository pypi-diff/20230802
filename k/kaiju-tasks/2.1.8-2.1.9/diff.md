# Comparing `tmp/kaiju_tasks-2.1.8-py3-none-any.whl.zip` & `tmp/kaiju_tasks-2.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 19012 bytes, number of entries: 12
--rw-r--r--  2.0 unx      151 b- defN 23-Jul-27 19:57 kaiju_tasks/__init__.py
--rw-r--r--  2.0 unx     6119 b- defN 23-Jul-27 19:57 kaiju_tasks/gui.py
--rw-r--r--  2.0 unx    40431 b- defN 23-Jul-27 19:57 kaiju_tasks/services.py
--rw-r--r--  2.0 unx     6161 b- defN 23-Jul-27 19:57 kaiju_tasks/types.py
--rw-r--r--  2.0 unx       42 b- defN 23-Jul-27 19:57 kaiju_tasks/tests/__init__.py
--rw-r--r--  2.0 unx     2272 b- defN 23-Jul-27 19:57 kaiju_tasks/tests/fixtures.py
--rw-r--r--  2.0 unx    15554 b- defN 23-Jul-27 19:57 kaiju_tasks/tests/test_tasks.py
--rw-rw-rw-  2.0 unx      610 b- defN 23-Jul-27 19:57 kaiju_tasks-2.1.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     3212 b- defN 23-Jul-27 19:57 kaiju_tasks-2.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-27 19:57 kaiju_tasks-2.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jul-27 19:57 kaiju_tasks-2.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      976 b- defN 23-Jul-27 19:57 kaiju_tasks-2.1.8.dist-info/RECORD
-12 files, 75632 bytes uncompressed, 17374 bytes compressed:  77.0%
+Zip file size: 19185 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      151 b- defN 23-Aug-02 19:50 kaiju_tasks/__init__.py
+-rw-r--r--  2.0 unx     6119 b- defN 23-Aug-02 19:50 kaiju_tasks/gui.py
+-rw-r--r--  2.0 unx    42158 b- defN 23-Aug-02 19:50 kaiju_tasks/services.py
+-rw-r--r--  2.0 unx     6220 b- defN 23-Aug-02 19:50 kaiju_tasks/types.py
+-rw-r--r--  2.0 unx       42 b- defN 23-Aug-02 19:50 kaiju_tasks/tests/__init__.py
+-rw-r--r--  2.0 unx     2272 b- defN 23-Aug-02 19:50 kaiju_tasks/tests/fixtures.py
+-rw-r--r--  2.0 unx    15615 b- defN 23-Aug-02 19:50 kaiju_tasks/tests/test_tasks.py
+-rw-rw-rw-  2.0 unx      610 b- defN 23-Aug-02 19:51 kaiju_tasks-2.1.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3212 b- defN 23-Aug-02 19:51 kaiju_tasks-2.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-02 19:51 kaiju_tasks-2.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Aug-02 19:51 kaiju_tasks-2.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      976 b- defN 23-Aug-02 19:51 kaiju_tasks-2.1.9.dist-info/RECORD
+12 files, 77479 bytes uncompressed, 17547 bytes compressed:  77.4%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: kaiju_tasks/tests/fixtures.py
 Comment: 
 
 Filename: kaiju_tasks/tests/test_tasks.py
 Comment: 
 
-Filename: kaiju_tasks-2.1.8.dist-info/LICENSE
+Filename: kaiju_tasks-2.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: kaiju_tasks-2.1.8.dist-info/METADATA
+Filename: kaiju_tasks-2.1.9.dist-info/METADATA
 Comment: 
 
-Filename: kaiju_tasks-2.1.8.dist-info/WHEEL
+Filename: kaiju_tasks-2.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: kaiju_tasks-2.1.8.dist-info/top_level.txt
+Filename: kaiju_tasks-2.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: kaiju_tasks-2.1.8.dist-info/RECORD
+Filename: kaiju_tasks-2.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kaiju_tasks/__init__.py

```diff
@@ -1,7 +1,7 @@
 from .types import *
 from .services import *
 from .gui import *
 
-__version__ = '2.1.8'
+__version__ = '2.1.9'
 __python_version__ = '3.11'
 __author__ = 'antonnidhoggr@me.com'
```

## kaiju_tasks/services.py

```diff
@@ -67,14 +67,15 @@
         sa.Column('stage', sa_pg.INTEGER, nullable=False),
         sa.Column('stages', sa_pg.INTEGER, nullable=False),
         sa.Column('created', sa_pg.TIMESTAMP(timezone=True), nullable=False),
         sa.Column('queued_at', sa_pg.INTEGER, nullable=True),
         sa.Column('exec_deadline', sa_pg.INTEGER, nullable=True),
         sa.Column('wait_deadline', sa_pg.INTEGER, nullable=True),
         sa.Column('next_run', sa_pg.INTEGER, nullable=True),
+        sa.Column('status_change', sa_pg.INTEGER, nullable=True),
         sa.Column('user_id', sa_pg.UUID(as_uuid=True), nullable=True),
         sa.Column('executor_id', sa_pg.UUID(as_uuid=True), nullable=True),
         sa.Column('job_id', sa_pg.TEXT, nullable=True),
         sa.Column('retries', sa_pg.INTEGER, nullable=False),
         sa.Column('exit_code', sa_pg.INTEGER, nullable=True),
         sa.Column('error', sa_pg.JSONB, nullable=True),
     )
@@ -172,14 +173,15 @@
                 'executor_id': None,
                 'job_id': get_short_uid(),
                 'exit_code': None,
                 'error': None,
                 'retries': 0,
                 'exec_deadline': None,
                 'wait_deadline': None,
+                'status_change': int(time()),
                 'stage': 0,
                 'result': [],
             },
             columns=['id'],
         )
         return bool(restarted)
 
@@ -193,14 +195,15 @@
         """
         updated = await self.m_update(
             id=[id],
             data={
                 'status': TaskStatus.SUSPENDED.value,
                 'result': self.table.c.result + [data],
                 'stage': self.table.c.stage + 1,
+                'status_change': int(time()),
                 'executor_id': None,
             },
             conditions={'status': TaskStatus.WAITING.value},
             columns=['id'],
         )
         return bool(updated)
 
@@ -394,104 +397,121 @@
 
     async def suspend_executor(self, executor_id: UUID) -> None:
         """Suspend an executor and its tasks.
 
         Usually an exiting executor calls this method to tell the manager it's no longer available.
         """
         self.logger.info('Suspending executor', executor_id=executor_id)
+        t = int(time())
         sql = (
             self.table.update()
             .where(sa.and_(self.table.c.status == TaskStatus.EXECUTED.value, self.table.c.executor_id == executor_id))
-            .values({'status': TaskStatus.SUSPENDED.value, 'executor_id': None})
+            .values({'status': TaskStatus.SUSPENDED.value, 'executor_id': None, 'status_change': t})
         )
         await self._db.execute(sql)
         await self._redis.hdel(self.executor_map_key, [str(executor_id)])
 
-    async def execute_stage(self, task_id: str, executor_id: UUID, stage: int) -> None:
+    async def execute_stage(self, task_id: str, executor_id: UUID, stage: int, timestamp: int) -> None:
         """Accept an executor report on stage execution."""
         self.logger.info('Stage executed', task_id=task_id, stage=stage, executor_id=executor_id)
         sql = (
             self.table.update()
-            .where(sa.and_(self.table.c.id == task_id, self.table.c.status == TaskStatus.QUEUED.value))
+            .where(
+                sa.and_(
+                    self.table.c.id == task_id,
+                    self.table.c.status == TaskStatus.QUEUED.value,
+                    self.table.c.status_change <= timestamp,
+                )
+            )
             .values(
                 {
                     'status': TaskStatus.EXECUTED.value,
-                    # 'stage': stage,
+                    'stage': stage,
                     'executor_id': executor_id,
+                    'status_change': timestamp,
                 }
             )
         )
         await self._db.execute(sql)
         await self.ping(executor_id)
 
-    async def wait_for_timer(self, task_id: str, executor_id: UUID, stage: int, deadline: int) -> None:
+    async def wait_for_timer(self, task_id: str, executor_id: UUID, stage: int, deadline: int, timestamp: int) -> None:
         """Require a task to wait for a message to continue."""
         sql = (
             self.table.update()
             .where(
-                sa.and_(
-                    self.table.c.id == task_id,
-                    self.table.c.status == TaskStatus.EXECUTED.value,
-                    self.table.c.executor_id == executor_id,
+                sa.or_(
+                    sa.and_(self.table.c.id == task_id, self.table.c.executor_id == executor_id),
+                    sa.and_(
+                        self.table.c.id == task_id,
+                        self.table.c.executor_id.is_(None),
+                        self.table.c.status == TaskStatus.QUEUED.value,
+                    ),
                 )
             )
             .values(
-                {'status': TaskStatus.WAITING.value, 'stage': stage, 'executor_id': None, 'wait_deadline': deadline}
+                {
+                    'status': TaskStatus.WAITING.value,
+                    'stage': stage,
+                    'executor_id': None,
+                    'wait_deadline': deadline,
+                    'status_change': timestamp,
+                }
             )
         )
         await self._db.execute(sql)
 
-    async def wait_for_message(self, task_id: str, executor_id: UUID, stage: int) -> None:
+    async def wait_for_message(self, task_id: str, executor_id: UUID, stage: int, timestamp: int) -> None:
         """Require a task to wait for a message to continue."""
         sql = (
             self.table.update()
             .where(
-                sa.and_(
-                    self.table.c.id == task_id,
-                    self.table.c.status == TaskStatus.EXECUTED.value,
-                    self.table.c.executor_id == executor_id,
+                sa.or_(
+                    sa.and_(self.table.c.id == task_id, self.table.c.executor_id == executor_id),
+                    sa.and_(
+                        self.table.c.id == task_id,
+                        self.table.c.executor_id.is_(None),
+                        self.table.c.status == TaskStatus.QUEUED.value,
+                    ),
                 )
             )
-            .values({'status': TaskStatus.WAITING.value, 'stage': stage, 'executor_id': None})
+            .values(
+                {'status': TaskStatus.WAITING.value, 'stage': stage, 'executor_id': None, 'status_change': timestamp}
+            )
         )
         await self._db.execute(sql)
 
     async def write_stage(
-        self, task_id: str, executor_id: UUID, stage: int, stages: int, result: Any, error: bool
+        self, task_id: str, executor_id: UUID, stage: int, stages: int, result: Any, error: bool, timestamp: int
     ) -> None:
         """Write stage result to the task table.
 
         This method will also change task status depending on which stage has been executed. The task my become
         'FINISHED' or 'FAILED'.
         """
         sql = self.table.update().where(
             sa.or_(
-                sa.and_(
-                    self.table.c.id == task_id,
-                    self.table.c.executor_id == executor_id,
-                    self.table.c.stage == stage,
-                    self.table.c.status == TaskStatus.EXECUTED.value,
-                ),
+                sa.and_(self.table.c.id == task_id, self.table.c.executor_id == executor_id),
                 sa.and_(
                     self.table.c.id == task_id,
                     self.table.c.executor_id.is_(None),
-                    self.table.c.stage == stage,
                     self.table.c.status == TaskStatus.QUEUED.value,
                 ),
             )
         )
         columns = [self.table.c.job_id, self.table.c.result, self.table.c.notify, self.table.c.user_id]
         if error:
             sql = sql.values(
                 {
                     'status': TaskStatus.FAILED.value,
                     'error': result,
                     'exit_code': self.ExitCode.EXECUTION_ERROR.value,
                     'executor_id': None,
                     'next_run': None,
+                    'status_change': timestamp,
                 }
             ).returning(*columns)
             task = await self._db.execute(sql)
             task = task.first()
             if task:
                 self.logger.error('Stage failed', stage=stage, task_id=task_id, executor_id=executor_id, error=result)
                 if task.notify:
@@ -512,14 +532,15 @@
             sql = sql.values(
                 {
                     'status': TaskStatus.FINISHED.value,
                     'result': self.table.c.result + [result],
                     'exit_code': self.ExitCode.SUCCESS.value,
                     'executor_id': None,
                     'next_run': None,
+                    'status_change': timestamp,
                 }
             ).returning(*columns)
             task = await self._db.execute(sql)
             task = task.first()
             if task:
                 self.logger.info('Task finished', stage=stage, task_id=task_id, executor_id=executor_id)
                 if task.next_task:
@@ -547,17 +568,15 @@
                         job_id=task['job_id'],
                         status=TaskStatus.FINISHED.value,
                         result=task['result'],
                         exit_code=self.ExitCode.SUCCESS.value,
                     )
                     await self._notifications.create(notification, columns=[])
         else:
-            sql = sql.values(
-                {'status': TaskStatus.EXECUTED.value, 'result': self.table.c.result + [result], 'stage': stage + 1}
-            )
+            sql = sql.values({'result': self.table.c.result + [result], 'stage': stage + 1}).returning(self.table.c.id)
             task = await self._db.execute(sql)
             task = task.first()
             if task:
                 self.logger.info('Stage finished', stage=stage, task_id=task_id, executor_id=executor_id)
 
     async def _queue_tasks(self):
         """Iterate over the tasks table."""
@@ -567,23 +586,24 @@
         await self._queue_timers()
         await self._queue_suspended_and_idle()
         await self._queue_failed()
 
     async def _expell_dead_executors(self):
         """Check if some executors are not responding and abort their tasks."""
         dead_executors = await self._list_dead_executors()
+        t = int(time())
         if dead_executors:
             sql = (
                 self.table.update()
                 .where(
                     sa.and_(
                         self.table.c.executor_id.in_(dead_executors), self.table.c.status == TaskStatus.EXECUTED.value
                     )
                 )
-                .values({'status': TaskStatus.SUSPENDED.value, 'executor_id': None})
+                .values({'status': TaskStatus.SUSPENDED.value, 'executor_id': None, 'status_change': t})
             )
             self.logger.info('Suspending dead executors', executor_id=dead_executors)
             await self._db.execute(sql)
             await self._redis.hdel(self.executor_map_key, dead_executors)
 
     async def _list_dead_executors(self) -> List[str]:
         """List executors with expired lifetime."""
@@ -591,14 +611,15 @@
         t = time()
         dt = Limit.PING_INTERVAL.value * 4
         dead_executors = [key.decode('utf-8') for key, t0 in executors.items() if t - int(t0.decode('utf-8')) > dt]
         return dead_executors
 
     async def _queue_timers(self):
         """Queue tasks waiting for timers."""
+        t = int(time())
         sql = (
             self.table.update()
             .where(
                 sa.and_(
                     self.table.c.wait_deadline < int(time()),
                     self.table.c.status == TaskStatus.WAITING.value,
                     self.table.c.enabled.is_(True),
@@ -607,21 +628,23 @@
             .values(
                 {
                     'status': TaskStatus.SUSPENDED.value,
                     'result': self.table.c.result + [None],
                     'stage': self.table.c.stage + 1,
                     'wait_deadline': None,
                     'executor_id': None,
+                    'status_change': t,
                 }
             )
         )
         await self._db.execute(sql)
 
     async def _queue_suspended_and_idle(self):
         """Queue all suspended tasks."""
+        t = int(time())
         sql = (
             self.table.update()
             .where(
                 sa.or_(
                     sa.and_(
                         self.table.c.next_run < int(time()),
                         self.table.c.status == TaskStatus.IDLE.value,
@@ -638,14 +661,20 @@
                 {
                     'status': TaskStatus.QUEUED.value,
                     'queued_at': int(time()),
                     'exec_deadline': int(time()) + self.table.c.max_exec_timeout,
                     'wait_deadline': None,
                     'exit_code': None,
                     'error': None,
+                    'status_change': t,
+                    'result': sa.text(
+                        f"CASE WHEN {self.table.c.status.name} = '{TaskStatus.SUSPENDED.value}'"
+                        f' THEN {self.table.c.result.name}'
+                        " ELSE '[]' END"
+                    ),  # CURRENT or FIRST
                 }
             )
             .returning(
                 self.table.c.id,
                 self.table.c.commands,
                 self.table.c.kws,
                 self.table.c.stage,
@@ -659,14 +688,15 @@
             queued_tasks = await conn.execute(sql)
             queued_tasks = [r._asdict() for r in queued_tasks.all()]  # noqa
             await self._send_tasks(queued_tasks)
             await conn.commit()
 
     async def _abort_timed_out_tasks(self):
         """Abort all queued tasks reached their timeout."""
+        t = int(time())
         sql = (
             self.table.update()
             .where(
                 sa.and_(
                     self.table.c.queued_at < int(time()) - Limit.MIN_T.value - self.table.c.max_exec_timeout,
                     self.table.c.status.in_(
                         [TaskStatus.QUEUED.value, TaskStatus.EXECUTED.value, TaskStatus.WAITING.value]
@@ -676,22 +706,25 @@
             )
             .values(
                 {
                     'status': TaskStatus.FAILED.value,
                     'error': None,
                     'exit_code': self.ExitCode.ABORTED.value,
                     'next_run': None,
+                    'executor_id': None,
+                    'status_change': t,
                 }
             )
             .returning(self.table.c.id)
         )
         await self._db.execute(sql)
 
     async def _queue_failed(self):
         """Queue all failed tasks with available retries."""
+        t = int(time())
         sql = (
             self.table.update()
             .where(
                 sa.and_(
                     self.table.c.queued_at > int(time()) - self._suspended_lifetime * 3600,
                     self.table.c.status == TaskStatus.FAILED.value,
                     self.table.c.max_retries > self.table.c.retries,
@@ -708,14 +741,15 @@
                         f"CASE WHEN {self.table.c.restart_policy.name} = '{RestartPolicy.CURRENT.value}'"
                         f' THEN {self.table.c.stage.name}'
                         ' ELSE 0 END'
                     ),  # CURRENT or FIRST
                     'executor_id': None,
                     'retries': self.table.c.retries + 1,
                     'exit_code': None,
+                    'status_change': t,
                 }
             )
             .returning(
                 self.table.c.id,
                 self.table.c.commands,
                 self.table.c.kws,
                 self.table.c.stage,
@@ -730,14 +764,15 @@
             queued_tasks = [r._asdict() for r in queued_tasks.all()]  # noqa
             await self._send_tasks(queued_tasks)
             await conn.commit()
 
     async def _restart_cron_tasks(self):
         """Reset all finished cron tasks to IDLE."""
         t = datetime.now(timezone.utc)
+        _t = int(time())
         sql = (
             self.table.update()
             .where(
                 sa.and_(
                     self.table.c.cron.isnot(None),
                     self.table.c.enabled.is_(True),
                     sa.or_(
@@ -748,19 +783,20 @@
                         ),
                     ),
                 )
             )
             .values(
                 {
                     'status': TaskStatus.IDLE.value,
-                    'result': [],
                     'stage': 0,
                     'executor_id': None,
                     'retries': 0,
-                    'wait_deadline': None
+                    'wait_deadline': None,
+                    'status_change': _t,
+                    # 'result': [],
                     # 'exit_code': None,
                     # 'error': None,
                 }
             )
             .returning(self.table.c.id, self.table.c.cron)
         )
         async with self._db.begin() as conn:
@@ -959,36 +995,47 @@
             retries=5,
             retry_timeout=1,
             logger=self.logger,
         )
 
     async def _wait_for_timer(self, data: ExecutorTask, stage: int, timer: int) -> None:
         """Wait for a timer."""
-        params = {'task_id': data['id'], 'executor_id': self.app.id, 'stage': stage, 'deadline': int(time()) + timer}
+        t = int(time())
+        params = {
+            'task_id': data['id'],
+            'executor_id': self.app.id,
+            'stage': stage,
+            'deadline': t + timer,
+            'timestamp': t,
+        }
         await self._call_manager('wait_for_timer', params, data['job_id'])
 
     async def _wait_for_message(self, data: ExecutorTask, stage: int) -> None:
         """Wait until the task receives a callback message."""
-        params = {'task_id': data['id'], 'executor_id': self.app.id, 'stage': stage}
+        t = int(time())
+        params = {'task_id': data['id'], 'executor_id': self.app.id, 'stage': stage, 'timestamp': t}
         await self._call_manager('wait_for_message', params, data['job_id'])
 
     async def _alert_on_stage_execution(self, data: ExecutorTask, stage: int) -> None:
         """Alert the manager on task execution."""
-        params = {'task_id': data['id'], 'executor_id': self.app.id, 'stage': stage}
+        t = int(time())
+        params = {'task_id': data['id'], 'executor_id': self.app.id, 'stage': stage, 'timestamp': t}
         await self._call_manager('execute_stage', params, data['job_id'])
 
     async def _write_stage_result(self, data: ExecutorTask, stage: int, error: bool, result) -> None:
         """Send task stage results to the manager."""
+        t = int(time())
         params = {
             'task_id': data['id'],
             'executor_id': self.app.id,
             'stage': stage,
             'stages': data['stages'],
             'result': result,
             'error': error,
+            'timestamp': t,
         }
         await self._call_manager('write_stage', params, data['job_id'])
 
     async def _send_ping(self) -> None:
         """Send a health report message to the manager."""
         if not self._closing:
             await self._call_manager('ping', {'executor_id': self.app.id}, None)
```

## kaiju_tasks/types.py

```diff
@@ -150,14 +150,15 @@
     result: list  #: task execution result, a list of stage returns
     stage: int  #: current stage being executed (or about to execute)
     stages: int  #: total number of stages
     queued_at: Optional[int]  #: UNIX time last queued
     exec_deadline: Optional[int]  #: UNIX time deadline
     wait_deadline: Optional[int]  #: UNIX time deadline for a timer command (see `Timer`)
     next_run: Optional[int]  #: UNIX time for next run
+    status_change: Optional[int]  #: last change of status
     user_id: Optional[UUID]  #: user created the task
     executor_id: Optional[UUID]  #: which executor has this task
     job_id: Optional[str]  #: updated for each new run
     retries: int  #: current number of retries
     created: datetime  #: when task record was added to the table
     exit_code: Optional[int]  #: exit (error) code similar to UNIX codes
     error: Optional[dict]  #: error.repr() if there's an error
```

## kaiju_tasks/tests/test_tasks.py

```diff
@@ -252,15 +252,15 @@
             (
                 {'status': TaskStatus.FAILED.value, 'cron': '* * * * 5', 'queued_at': int(time())},
                 {'status': TaskStatus.IDLE.value},
             ),
             ({'status': TaskStatus.FINISHED.value}, {'status': TaskStatus.FINISHED.value}),
             (
                 {'status': TaskStatus.FINISHED.value, 'cron': '* * * * 5', 'stage': 1, 'retries': 3, 'result': [1, 2]},
-                {'status': TaskStatus.IDLE.value, 'stage': 0, 'retries': 0, 'result': []},
+                {'status': TaskStatus.IDLE.value, 'stage': 0, 'retries': 0, 'result': [1, 2]},
             ),
             (
                 {'status': TaskStatus.WAITING.value, 'queued_at': int(time()), 'wait_deadline': int(time()) - 1},
                 {'status': TaskStatus.QUEUED.value},
             ),
             (
                 {'status': TaskStatus.WAITING.value, 'queued_at': int(time())},
@@ -305,16 +305,17 @@
         task = await task_service.create({'commands': [{'method': 'do'}], 'notify': True}, columns=['id', 'job_id'])
         await asyncio.sleep(1)
         await _service._queue_tasks()
         task = await task_service.get(task['id'])
         assert task['status'] == TaskStatus.QUEUED.value
         executor_id = uuid4()
         result = str(uuid4())
-        await _service.execute_stage(task['id'], executor_id, 0)
-        await _service.write_stage(task['id'], executor_id, 0, 1, result, False)
+        t = int(time())
+        await _service.execute_stage(task['id'], executor_id, 0, t)
+        await _service.write_stage(task['id'], executor_id, 0, 1, result, False, t)
         notifications = await notification_service.list(conditions={'job_id': task['job_id']})
         notifications = notifications['data']
         assert notifications
         notification = notifications[0]
         task = await task_service.get(task['id'])
         assert task['exit_code'] == 0
         assert task['error'] is None
@@ -326,15 +327,16 @@
         next_task = await task_service.create({'commands': [{'method': 'do'}]})
         task = await task_service.create({'commands': [{'method': 'do'}], 'next_task': next_task['id']}, columns='*')
         await task_service.update(next_task['id'], {'status': TaskStatus.FINISHED.value, 'next_run': time() + 10000})
         executor_id = uuid4()
         await task_service.update(
             task['id'], {'status': TaskStatus.EXECUTED.value, 'executor_id': executor_id, 'stage': 0}
         )
-        await _service.write_stage(task['id'], executor_id, 0, 1, 'result', False)
+        t = int(time())
+        await _service.write_stage(task['id'], executor_id, 0, 1, 'result', False, t)
         next_task = await task_service.get(next_task['id'])
         assert next_task['status'] == TaskStatus.IDLE.value
         assert next_task['next_run'] <= time()
 
     async def test_executor_management(self, _service, task_service):
         task_service._validator = lambda o: o
         new_executor = uuid4()
```

## Comparing `kaiju_tasks-2.1.8.dist-info/LICENSE` & `kaiju_tasks-2.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kaiju_tasks-2.1.8.dist-info/METADATA` & `kaiju_tasks-2.1.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaiju-tasks
-Version: 2.1.8
+Version: 2.1.9
 Summary: Service and user task management
 Home-page: https://gitlab.com/kaiju-python/kaiju-tasks
 Author: antonnidhoggr@me.com
 Author-email: antonnidhoggr@me.com
 License: Apache Software License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `kaiju_tasks-2.1.8.dist-info/RECORD` & `kaiju_tasks-2.1.9.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-kaiju_tasks/__init__.py,sha256=Ih9UnjM7iNyezQ9mouTN-04qF9aIIApPf0uaD3pfrI0,151
+kaiju_tasks/__init__.py,sha256=HFbW1NO8LtdVEw2sAS2H5v1rF_1JBAY5c0_wLm-Xxvc,151
 kaiju_tasks/gui.py,sha256=SwPN_7GQkMDU7VUONXOCk7_tMBoyZTIflb60vxxjmRw,6119
-kaiju_tasks/services.py,sha256=spxIjehmr7-BN8OVF862vfhgrl20d3aE_AsdgoHfKdQ,40431
-kaiju_tasks/types.py,sha256=3JLF6ZsCXPFTcwZISQcwNUbTqJeGIpe24GRNa8i9lpE,6161
+kaiju_tasks/services.py,sha256=0rYpNvL11fgts-my1mteRWNCXLJ0GtZ-YPukLnRGeSY,42158
+kaiju_tasks/types.py,sha256=NeB9dUjO-wLK-GME4dn5kNRn0R3Af01tX1AOiAA2Sw0,6220
 kaiju_tasks/tests/__init__.py,sha256=WlPruePOcaMi5ikqn6GheE1Z-zYcysb9M1dj6SteWGY,42
 kaiju_tasks/tests/fixtures.py,sha256=7hLaDyE3Sjibnt5zZ9YNNJ2586541NRPC4Y3qIQzI2s,2272
-kaiju_tasks/tests/test_tasks.py,sha256=NT4kACEZeYw2OiNA9AwbKOVrfM1JLfnh7KefYUplF3s,15554
-kaiju_tasks-2.1.8.dist-info/LICENSE,sha256=XIlN2qA8UqpBDA-PteoYP4hTU0qBW0G9PRB__khO2zc,610
-kaiju_tasks-2.1.8.dist-info/METADATA,sha256=Fxt3QpHc8NQQjKA2cJ2xaJrR2T9ilIhatf_jXzv_L5Q,3212
-kaiju_tasks-2.1.8.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-kaiju_tasks-2.1.8.dist-info/top_level.txt,sha256=QyLogqOVVajJlalq6RfikGx5VGn_lLeTANJEsfZZlM0,12
-kaiju_tasks-2.1.8.dist-info/RECORD,,
+kaiju_tasks/tests/test_tasks.py,sha256=f5F2o_r0auP2ctC472oJzv_JTDpd51K70z91dz5Gubs,15615
+kaiju_tasks-2.1.9.dist-info/LICENSE,sha256=XIlN2qA8UqpBDA-PteoYP4hTU0qBW0G9PRB__khO2zc,610
+kaiju_tasks-2.1.9.dist-info/METADATA,sha256=6xL9uNwIuuqE1QsahDRITj_3ZdsU26LA6_b7B8Ba-0o,3212
+kaiju_tasks-2.1.9.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+kaiju_tasks-2.1.9.dist-info/top_level.txt,sha256=QyLogqOVVajJlalq6RfikGx5VGn_lLeTANJEsfZZlM0,12
+kaiju_tasks-2.1.9.dist-info/RECORD,,
```

