# Comparing `tmp/catenae_stopover-3.219.1-py3-none-any.whl.zip` & `tmp/catenae_stopover-3.2308.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 9392 bytes, number of entries: 12
--rw-r--r--  2.0 unx     2086 b- defN 21-Sep-23 09:21 catenae/__init__.py
--rw-r--r--  2.0 unx    18479 b- defN 21-Sep-23 07:38 catenae/catenae.py
--rw-r--r--  2.0 unx      390 b- defN 21-Sep-21 23:05 catenae/errors.py
--rw-r--r--  2.0 unx      614 b- defN 21-Sep-21 23:05 catenae/health.py
--rw-r--r--  2.0 unx      721 b- defN 21-Sep-22 09:40 catenae/logger.py
--rw-r--r--  2.0 unx     1995 b- defN 21-Sep-21 23:05 catenae/queue.py
--rw-r--r--  2.0 unx     1860 b- defN 21-Sep-21 23:05 catenae/threading.py
--rw-r--r--  2.0 unx      959 b- defN 21-Sep-22 09:42 catenae/utils.py
--rw-r--r--  2.0 unx      835 b- defN 21-Sep-23 09:22 catenae_stopover-3.219.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Sep-23 09:22 catenae_stopover-3.219.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 21-Sep-23 09:22 catenae_stopover-3.219.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      933 b- defN 21-Sep-23 09:22 catenae_stopover-3.219.1.dist-info/RECORD
-12 files, 28972 bytes uncompressed, 7834 bytes compressed:  73.0%
+Zip file size: 9340 bytes, number of entries: 12
+-rw-r--r--  2.0 unx     2088 b- defN 23-Aug-02 17:07 catenae/__init__.py
+-rw-r--r--  2.0 unx    18068 b- defN 23-Aug-02 17:46 catenae/catenae.py
+-rw-r--r--  2.0 unx      390 b- defN 23-Aug-02 17:07 catenae/errors.py
+-rw-r--r--  2.0 unx      636 b- defN 23-Aug-02 17:00 catenae/health.py
+-rw-r--r--  2.0 unx      568 b- defN 23-Aug-02 17:19 catenae/logger.py
+-rw-r--r--  2.0 unx     2096 b- defN 23-Aug-02 17:02 catenae/queue.py
+-rw-r--r--  2.0 unx     2027 b- defN 23-Aug-02 17:08 catenae/threading.py
+-rw-r--r--  2.0 unx     1060 b- defN 23-Aug-02 17:06 catenae/utils.py
+-rw-r--r--  2.0 unx      824 b- defN 23-Aug-02 17:52 catenae_stopover-3.2308.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-02 17:52 catenae_stopover-3.2308.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Aug-02 17:52 catenae_stopover-3.2308.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      938 b- defN 23-Aug-02 17:52 catenae_stopover-3.2308.0.dist-info/RECORD
+12 files, 28795 bytes uncompressed, 7774 bytes compressed:  73.0%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: catenae/threading.py
 Comment: 
 
 Filename: catenae/utils.py
 Comment: 
 
-Filename: catenae_stopover-3.219.1.dist-info/METADATA
+Filename: catenae_stopover-3.2308.0.dist-info/METADATA
 Comment: 
 
-Filename: catenae_stopover-3.219.1.dist-info/WHEEL
+Filename: catenae_stopover-3.2308.0.dist-info/WHEEL
 Comment: 
 
-Filename: catenae_stopover-3.219.1.dist-info/top_level.txt
+Filename: catenae_stopover-3.2308.0.dist-info/top_level.txt
 Comment: 
 
-Filename: catenae_stopover-3.219.1.dist-info/RECORD
+Filename: catenae_stopover-3.2308.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## catenae/__init__.py

```diff
@@ -10,9 +10,10 @@
     '        ◼◼◼             ◼◼◼◼            ◼◼           ◼◼◼           ◼◼◼◼      ◼◼◼          ◼◼◼◼             ◼◼◼         \n'  # noqa: E501
     '      ◼◼◼             ◼◼◼  ◼◼◼          ◼◼         ◼◼◼             ◼◼◼◼◼     ◼◼◼        ◼◼◼  ◼◼◼         ◼◼◼           \n'  # noqa: E501
     '    ◼◼◼              ◼◼◼    ◼◼◼         ◼◼       ◼◼◼               ◼◼◼ ◼◼◼   ◼◼◼       ◼◼◼    ◼◼◼      ◼◼◼             \n'  # noqa: E501
     '  ◼◼◼               ◼◼◼      ◼◼◼        ◼◼     ◼◼◼◼◼◼◼◼◼◼◼◼◼◼◼◼◼◼  ◼◼◼  ◼◼◼  ◼◼◼      ◼◼◼      ◼◼◼   ◼◼◼◼◼◼◼◼◼◼◼◼◼◼◼◼◼◼\n'  # noqa: E501
     '    ◼◼◼            ◼◼◼        ◼◼◼       ◼◼       ◼◼◼               ◼◼◼    ◼◼ ◼◼◼     ◼◼◼        ◼◼◼    ◼◼◼             \n'  # noqa: E501
     '      ◼◼◼         ◼◼◼          ◼◼◼      ◼◼         ◼◼◼             ◼◼◼     ◼◼◼◼◼    ◼◼◼          ◼◼◼     ◼◼◼           \n'  # noqa: E501
     '        ◼◼◼      ◼◼◼            ◼◼◼     ◼◼           ◼◼◼           ◼◼◼      ◼◼◼◼   ◼◼◼            ◼◼◼      ◼◼◼         \n'  # noqa: E501
-    '          ◼◼◼   ◼◼◼              ◼◼◼    ◼◼             ◼◼◼         ◼◼◼       ◼◼◼  ◼◼◼              ◼◼◼       ◼◼◼       \n')  # noqa: E501
-__version__ = '3.219.1'
+    '          ◼◼◼   ◼◼◼              ◼◼◼    ◼◼             ◼◼◼         ◼◼◼       ◼◼◼  ◼◼◼              ◼◼◼       ◼◼◼       \n'  # noqa: E501
+)
+__version__ = '3.2308.0'
```

## catenae/catenae.py

```diff
@@ -68,28 +68,30 @@
         'no_messages_sleep_interval': .5,
         'intervals': {
             'loop_check_stop': 1,
             'loop_check_start': 1
         }
     }
 
-    def __init__(self,
-                 endpoint: str = None,
-                 endpoints: List = None,
-                 input_stream: str = None,
-                 input_streams: List = None,
-                 default_output_stream: str = None,
-                 receiver_group: str = None,
-                 rpc_enabled: bool = None,
-                 rpc_by_uid: bool = None,
-                 enable_health: bool = None,
-                 health_port: int = None,
-                 log_level: str = None,
-                 progress_without_commit: bool = None,
-                 **ignored_kwargs):
+    def __init__(
+        self,
+        endpoint: str = None,
+        endpoints: List = None,
+        input_stream: str = None,
+        input_streams: List = None,
+        default_output_stream: str = None,
+        receiver_group: str = None,
+        rpc_enabled: bool = None,
+        rpc_by_uid: bool = None,
+        enable_health: bool = None,
+        health_port: int = None,
+        log_level: str = None,
+        progress_without_commit: bool = None,
+        **ignored_kwargs,
+    ):
         self.logger = Logger(self, level=log_level)
 
         if endpoint is not None:
             endpoints = [endpoint]
         if not endpoints:
             endpoints = []
 
@@ -98,41 +100,49 @@
         if not input_streams:
             input_streams = []
 
         self._uncommitted_messages = []
 
         self._config = dict(Link.DEFAULT_CONFIG)
         self._set_uid()
-        self._config.update({
-            'endpoints': endpoints,
-            'input_streams': input_streams,
-            'default_output_stream': default_output_stream,
-            'receiver_group': (receiver_group if receiver_group
-                            else self.__class__.__name__),
-            'rpc_enabled': True if rpc_enabled else False,
-            'enable_health': False if enable_health is False else True,
-            'health_port': health_port if health_port else 2094,
-            'rpc_topics': [f'catenae_rpc_{self.__class__.__name__.lower()}',
-                            'catenae_rpc_broadcast'],
-            'progress_without_commit': (True if progress_without_commit
-                                        else False),
-        })
+        self._config.update(
+            {
+                'endpoints': endpoints,
+                'input_streams': input_streams,
+                'default_output_stream': default_output_stream,
+                'receiver_group': (
+                    receiver_group
+                    if receiver_group else self.__class__.__name__
+                ),
+                'rpc_enabled': True if rpc_enabled else False,
+                'enable_health': False if enable_health is False else True,
+                'health_port': health_port if health_port else 2094,
+                'rpc_topics': [
+                    f'catenae_rpc_{self.__class__.__name__.lower()}',
+                    'catenae_rpc_broadcast'
+                ],
+                'progress_without_commit': (
+                    True if progress_without_commit else False
+                ),
+            }
+        )
         if rpc_by_uid:
             self._config['rpc_topics'].append(f'catenae_rpc_{self.uid}')
 
         self._load_args()
 
         if ignored_kwargs:
             self.logger.log(
-                f'the following kwargs were ignored: {ignored_kwargs}')
+                f'the following kwargs were ignored: {ignored_kwargs}'
+            )
 
         if self._config['endpoints']:
             self.stopover = stopover.Stopover(
                 endpoint=self._config['endpoints'][0],
-                uid=self._config['uid']
+                uid=self._config['uid'],
             )
         else:
             self.stopover = None
 
         self._threads = []
         self._locks = {
             'threads': Lock(),
@@ -150,72 +160,83 @@
     @property
     def args(self):
         return list(self._args)
 
     def _load_args(self):
         parser = argparse.ArgumentParser()
 
-        parser.add_argument('-e',
-                            '--endpoint',
-                            '--endpoints',
-                            action='store',
-                            dest='endpoint',
-                            help='Message broker endpoint. \
-                            E.g., http://localhost:5704',
-                            required=False)
-
-        parser.add_argument('-i',
-                            '--input',
-                            action='store',
-                            dest='input_streams',
-                            help='Input streams. Several streams '
-                            + 'can be specified separated by commas',
-                            required=False)
-
-        parser.add_argument('-o',
-                            '--default-output',
-                            action='store',
-                            dest='default_output_stream',
-                            help='Default output stream.',
-                            required=False)
-
-        parser.add_argument('-g',
-                            '--receiver-group',
-                            action='store',
-                            dest='receiver_group',
-                            help='Receiver group.',
-                            required=False)
-
-        parser.add_argument('-u',
-                            '--uid',
-                            action='store',
-                            dest='uid',
-                            help='Link\'s Unique ID.',
-                            required=False)
-
-        parser.add_argument('-r',
-                            '--rpc',
-                            action='store_true',
-                            dest='rpc_enabled',
-                            help='Enable RPC.',
-                            required=False)
+        parser.add_argument(
+            '-e',
+            '--endpoint',
+            '--endpoints',
+            action='store',
+            dest='endpoint',
+            help='Message broker endpoint. E.g., http://localhost:5704',
+            required=False,
+        )
+
+        parser.add_argument(
+            '-i',
+            '--input',
+            action='store',
+            dest='input_streams',
+            help='Input streams. Several streams '
+            + 'can be specified separated by commas',
+            required=False,
+        )
+
+        parser.add_argument(
+            '-o',
+            '--default-output',
+            action='store',
+            dest='default_output_stream',
+            help='Default output stream.',
+            required=False,
+        )
+
+        parser.add_argument(
+            '-g',
+            '--receiver-group',
+            action='store',
+            dest='receiver_group',
+            help='Receiver group.',
+            required=False,
+        )
+
+        parser.add_argument(
+            '-u',
+            '--uid',
+            action='store',
+            dest='uid',
+            help='Link\'s Unique ID.',
+            required=False,
+        )
+
+        parser.add_argument(
+            '-r',
+            '--rpc',
+            action='store_true',
+            dest='rpc_enabled',
+            help='Enable RPC.',
+            required=False,
+        )
 
         parsed_args = parser.parse_known_args()
         link_args = parsed_args[0]
         self._args = parsed_args[1]
 
         if link_args.endpoint:
             self._config['endpoints'] = link_args.endpoint.split(',')
 
         if link_args.input_streams:
             self._config['input_streams'] = link_args.input_streams.split(',')
 
         if link_args.default_output_stream:
-            self._config[
-                'default_output_stream'] = link_args.default_output_stream
+            self._config['default_output_stream'
+                         ] = link_args.default_output_stream
 
         if link_args.receiver_group:
             self._config['receiver_group'] = link_args.receiver_group
 
         if link_args.uid:
             self._config['uid'] = link_args.uid
 
@@ -229,30 +250,33 @@
     @property
     def config(self):
         return dict(self._config)
 
     def setup(self):
         pass
 
-    def start(self,
-              startup_text: str = None,
-              setup_kwargs: Dict = None,
-              embedded: bool = False,
-              **_):
+    def start(
+        self,
+        startup_text: str = None,
+        setup_kwargs: Dict = None,
+        embedded: bool = False,
+        **_,
+    ):
         with self._locks['start_stop']:
             if self._started:
                 return
 
         if not startup_text:
-            self.logger.log(catenae.text_logo)
+            print(catenae.text_logo)
         self.logger.log(f'catenae  v{catenae.__version__}')
         self.logger.log(f'stopover v{stopover.__version__}')
 
         self.logger.log(
-            f'configuration:\n{utils.dump_dict_pretty(self._config)}')
+            f'configuration:\n{utils.dump_dict_pretty(self._config)}'
+        )
 
         if startup_text:
             self.logger.log(startup_text)
 
         with self._locks['start_stop']:
             self._started = True
 
@@ -270,31 +294,33 @@
             if hasattr(self, 'transform'):
                 self._threads.append(self.loop(self._transform))
 
             self._threads.append(
                 self.loop(
                     self.stopover.knock,
                     kwargs={'receiver_group': self.config['receiver_group']},
-                    interval=5))
+                    interval=5
+                )
+            )
 
         if self.config['enable_health']:
             health_server = HealthCheck(self.config['health_port'])
             self.launch_thread(health_server.start)
 
         if not embedded:
             self._setup_signals_handler()
             for thread in self._threads:
                 thread.join()
 
     def stop(self):
         pass
 
     def send(self, message, stream: str = None):
-        stream = self.config[
-            'default_output_stream'] if stream is None else stream
+        stream = self.config['default_output_stream'
+                             ] if stream is None else stream
         if stream is None:
             raise ValueError('stream not provided')
         self.stopover.put(message, stream)
 
     def launch_thread(
         self,
         target,
@@ -322,17 +348,17 @@
         loop_task_kwargs = {
             'target': target,
             'args': args,
             'kwargs': kwargs,
             'interval': interval,
             'wait': wait,
         }
-        thread = self.launch_thread(self._loop_task,
-                                    kwargs=loop_task_kwargs,
-                                    safe_stop=safe_stop)
+        thread = self.launch_thread(
+            self._loop_task, kwargs=loop_task_kwargs, safe_stop=safe_stop
+        )
         return thread
 
     def rpc_notify(
         self,
         method=None,
         args=None,
         kwargs=None,
@@ -353,15 +379,15 @@
         call = {
             'method': method,
             'context': {
                 'group': self.config['receiver_group'],
                 'uid': self.uid
             },
             'args': args,
-            'kwargs': kwargs
+            'kwargs': kwargs,
         }
 
         self.send(call, topic)
 
     def suicide(self, message=None, exception=False):
         with self._locks['start_stop']:
             if self._stopped:
@@ -408,35 +434,37 @@
         no_messages = True
         for input_stream in self.config['input_streams']:
             message = None
             try:
                 message = self.stopover.get(
                     input_stream,
                     self.config['receiver_group'],
-                    progress_without_commit=self.config[
-                        'progress_without_commit'],
+                    progress_without_commit=self.
+                    config['progress_without_commit'],
                 )
             except Exception:
                 pass
 
             if not message:
                 continue
             no_messages = False
 
             if self.config['progress_without_commit']:
                 self._uncommitted_messages.append(message)
 
             result = self.transform(message)
-            output = result.value if isinstance(result,
-                                                stopover.Response) else result
+            output = result.value if isinstance(
+                result, stopover.Response
+            ) else result
 
             if output:
                 if self.config['default_output_stream']:
-                    self.stopover.put(output,
-                                      self.config['default_output_stream'])
+                    self.stopover.put(
+                        output, self.config['default_output_stream']
+                    )
                 else:
                     raise ValueError('default stream is missing')
 
             if not self.config['progress_without_commit']:
                 self.stopover.commit(message, self.config['receiver_group'])
 
         if no_messages:
@@ -489,31 +517,26 @@
 
         try:
             context = call['context']
             args = [context] + call['args']
             kwargs = call['kwargs']
             self.logger.log(
                 f"RPC invocation from {context['uid']} ({context['group']})",
-                level='debug')
+                level='debug'
+            )
             with self._locks['rpc_lock']:
                 getattr(self, call['method'])(*args, **kwargs)
 
         except Exception:
-            self.logger.log(f'error when invoking {method} remotely',
-                            level='exception')
+            self.logger.log(
+                f'error when invoking {method} remotely', level='exception'
+            )
 
     @suicide_on_error
-    def _loop_task(
-        self,
-        target,
-        args,
-        kwargs,
-        interval,
-        wait
-    ):
+    def _loop_task(self, target, args, kwargs, interval, wait):
         if wait:
             time.sleep(interval)
 
         if args is None:
             args = []
 
         if not isinstance(args, list):
@@ -525,15 +548,16 @@
         while not current_thread().will_stop:
             start_timestamp = utils.get_timestamp()
 
             target(*args, **kwargs)
 
             while not current_thread().will_stop:
                 continue_sleeping = (
-                    utils.get_timestamp() - start_timestamp) < interval
+                    utils.get_timestamp() - start_timestamp
+                ) < interval
                 if not continue_sleeping:
                     break
                 time.sleep(self.config['intervals']['loop_check_stop'])
 
     def _setup_signals_handler(self):
         for signal_name in ['SIGINT', 'SIGTERM', 'SIGQUIT']:
             signal.signal(getattr(signal, signal_name), self._signal_handler)
```

## catenae/health.py

```diff
@@ -9,15 +9,17 @@
     def log_message(self, *_):
         pass
 
 
 class HealthCheck:
     def __init__(self, port):
         self.server = WSGIServer(
-            ('0.0.0.0', port), NoLoggingWSGIRequestHandler)
+            ('0.0.0.0', port),
+            NoLoggingWSGIRequestHandler,
+        )
         api = falcon.App()
         api.add_route('/health', self)
         self.server.set_app(api)
 
     def on_get(self, _, response):
         response.media = {'status': 'available'}
```

## catenae/logger.py

```diff
@@ -1,25 +1,23 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-import logging
+from binnakle import Binnakle
 
 
 class Logger:
     def __init__(self, instance, level=None):
-        if level is None:
-            level = 'info'
+        self.level = level.lower() if level else 'info'
         self.instance = instance
-        logging.basicConfig(
-            format='%(asctime)-15s [%(levelname)s] %(message)s',
-            datefmt='%Y-%m-%d %H:%M:%S')
-        logging.getLogger().setLevel(getattr(
-            logging,
-            level.upper(),
-            logging.INFO)
-        )
+        self._logger = Binnakle()
 
-    def log(self, message='', level='info'):
-        if message:
-            message = (f'{self.instance.__class__.__name__}/{self.instance.uid}'
-                       f' → {message}')
-        getattr(logging, level.lower(), 'INFO')(message)
+    def log(
+        self,
+        message='',
+        level=None,
+    ):
+        level = level.lower() if level else self.level
+        getattr(self._logger, level.lower())(
+            message,
+            instance=self.instance.uid,
+            microservice=self.instance.__class__.__name__,
+        )
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## catenae/queue.py

```diff
@@ -18,24 +18,33 @@
         pass
 
     def get(self):
         pass
 
 
 class ThreadingQueue(CustomQueue):
-    def __init__(self, size=0, circular=False):
+    def __init__(
+        self,
+        size=0,
+        circular=False,
+    ):
         super().__init__(size, circular)
         self._queue = list()
         self._lock = threading.Lock()
 
     def _truncate(self):
         if self._size > 0 and len(self._queue) > self._size:
             self._queue.pop(0)
 
-    def put(self, item, block=True, timeout=None):
+    def put(
+        self,
+        item,
+        block=True,
+        timeout=None,
+    ):
         if self._circular:
             self._lock.acquire()
             self._queue.append(item)
             self._truncate()
             self._lock.release()
             return
 
@@ -47,15 +56,19 @@
                 self._lock.release()
                 return
             self._lock.release()
             if not block:
                 raise EmptyError
             time.sleep(ThreadingQueue.BLOCKING_SECONDS)
 
-    def get(self, block=True, timeout=None):
+    def get(
+        self,
+        block=True,
+        timeout=None,
+    ):
         if timeout is not None:
             block = False
 
         start_timestamp = get_timestamp()
         while timeout is None or get_timestamp() - start_timestamp < timeout:
             self._lock.acquire()
             if len(self._queue) > 0:
```

## catenae/threading.py

```diff
@@ -7,15 +7,20 @@
 
 
 def should_stop():
     return threading.current_thread().will_stop
 
 
 class Thread(threading.Thread):
-    def __init__(self, target, args=None, kwargs=None):
+    def __init__(
+        self,
+        target,
+        args=None,
+        kwargs=None,
+    ):
         if args is None:
             args = tuple()
         elif isinstance(args, list):
             args = tuple(args)
         elif not isinstance(args, tuple):
             args = tuple([args])
 
@@ -30,25 +35,34 @@
 
     @property
     def will_stop(self):
         return self._will_stop
 
 
 class ThreadPool:
-    def __init__(self, link_instance, num_threads=1):
+    def __init__(
+        self,
+        link_instance,
+        num_threads=1,
+    ):
         self.link_instance = link_instance
         self.tasks_queue = ThreadingQueue()
         self.threads = []
 
         for i in range(num_threads):
             thread = Thread(self._worker_target, i)
             self.threads.append(thread)
             thread.start()
 
-    def submit(self, target, args=None, kwargs=None):
+    def submit(
+        self,
+        target,
+        args=None,
+        kwargs=None,
+    ):
         if args is None:
             args = []
 
         if not isinstance(args, list):
             args = [args]
 
         if kwargs is None:
@@ -56,15 +70,20 @@
 
         self.tasks_queue.put((target, args, kwargs))
 
     def _worker_target(self, index):
         while not self.threads[index].will_stop:
             try:
                 target, args, kwargs = self.tasks_queue.get(
-                    timeout=1, block=False)
+                    timeout=1,
+                    block=False,
+                )
                 target(*args, **kwargs)
+
             except EmptyError:
                 pass
+
             except Exception:
                 self.link_instance.logger.log(
                     'exception during the execution of a task',
-                    level='exception')
+                    level='exception',
+                )
```

## catenae/utils.py

```diff
@@ -16,32 +16,45 @@
     return int(round(time.time() * 1000))
 
 
 def dump_dict_pretty(input_dict):
     return json.dumps(
         input_dict,
         indent=4,
-        ensure_ascii=False
+        ensure_ascii=False,
     )
 
 
 def dump_dict(input_dict):
-    return json.dumps(input_dict, separators=(',', ':'), ensure_ascii=False)
+    return json.dumps(
+        input_dict,
+        separators=(',', ':'),
+        ensure_ascii=False,
+    )
 
 
 def load_dict(str_dict):
-    return json.loads(str_dict, object_pairs_hook=OrderedDict)
+    return json.loads(
+        str_dict,
+        object_pairs_hook=OrderedDict,
+    )
 
 
 def blake2b_256(text: str):
-    return hashlib.blake2b(text.encode('utf-8'), digest_size=32).hexdigest()
+    return hashlib.blake2b(
+        text.encode('utf-8'),
+        digest_size=32,
+    ).hexdigest()
 
 
 def blake2b_512(text: str):
-    return hashlib.blake2b(text.encode('utf-8'), digest_size=64).hexdigest()
+    return hashlib.blake2b(
+        text.encode('utf-8'),
+        digest_size=64,
+    ).hexdigest()
 
 
 def sha3_512(text: str):
     return hashlib.sha3_512(text.encode('utf-8')).hexdigest()
 
 
 def get_uid():
```

## Comparing `catenae_stopover-3.219.1.dist-info/METADATA` & `catenae_stopover-3.2308.0.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
 Name: catenae-stopover
-Version: 3.219.1
+Version: 3.2308.0
 Summary: Catenae 3 – Microservices Framework for Stopover
 Home-page: https://github.com/catenae
 Author: Rodrigo Martínez
 Author-email: dev@brunneis.com
 License: GNU General Public License v3.0
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: stopover (>=1.219.1)
-Requires-Dist: orderedset (~=2.0.3)
+Requires-Dist: stopover (<2.0.0,>=1.214.0)
 Requires-Dist: falcon (<4.0.0,>=3.0.0)
-
-UNKNOWN
+Requires-Dist: binnakle (<2.0.0,>=1.2212.1)
```

