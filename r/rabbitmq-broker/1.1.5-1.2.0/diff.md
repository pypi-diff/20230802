# Comparing `tmp/rabbitmq_broker-1.1.5-py3-none-any.whl.zip` & `tmp/rabbitmq_broker-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,33 @@
-Zip file size: 17031 bytes, number of entries: 24
--rw-r--r--  2.0 unx       22 b- defN 23-Jul-27 11:28 rmq_broker/__init__.py
--rw-r--r--  2.0 unx     1080 b- defN 23-May-31 15:11 rmq_broker/schemas.py
--rw-r--r--  2.0 unx      532 b- defN 23-Jul-27 10:36 rmq_broker/settings.py
--rw-r--r--  2.0 unx      257 b- defN 23-Jun-06 15:36 rmq_broker/utils.py
+Zip file size: 21856 bytes, number of entries: 31
+-rw-r--r--  2.0 unx       22 b- defN 23-Aug-02 12:37 rmq_broker/__init__.py
+-rw-r--r--  2.0 unx     5249 b- defN 23-Aug-02 12:37 rmq_broker/models.py
+-rw-r--r--  2.0 unx      528 b- defN 23-Aug-02 12:37 rmq_broker/schemas.py
+-rw-r--r--  2.0 unx      555 b- defN 23-Aug-02 12:37 rmq_broker/settings.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-26 07:16 rmq_broker/async_chains/__init__.py
--rw-r--r--  2.0 unx     9326 b- defN 23-Jul-27 10:36 rmq_broker/async_chains/base.py
+-rw-r--r--  2.0 unx     8889 b- defN 23-Aug-02 12:37 rmq_broker/async_chains/base.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-26 07:16 rmq_broker/chains/__init__.py
--rw-r--r--  2.0 unx     4333 b- defN 23-Jun-06 15:36 rmq_broker/chains/base.py
+-rw-r--r--  2.0 unx     4326 b- defN 23-Aug-02 12:37 rmq_broker/chains/base.py
 -rw-r--r--  2.0 unx       37 b- defN 23-Jun-06 15:36 rmq_broker/documentation/__init__.py
--rw-r--r--  2.0 unx     3577 b- defN 23-Jul-27 10:36 rmq_broker/documentation/base.py
+-rw-r--r--  2.0 unx     3699 b- defN 23-Aug-02 12:37 rmq_broker/documentation/base.py
 -rw-r--r--  2.0 unx    10645 b- defN 23-Jun-06 15:36 rmq_broker/documentation/models.py
 -rw-r--r--  2.0 unx      136 b- defN 23-Jun-06 15:36 rmq_broker/documentation/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 15:36 rmq_broker/documentation/mixins/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 15:36 rmq_broker/documentation/mixins/pydantic/__init__.py
 -rw-r--r--  2.0 unx     1278 b- defN 23-Jun-06 15:36 rmq_broker/documentation/mixins/pydantic/chains.py
 -rw-r--r--  2.0 unx     1307 b- defN 23-Jun-06 15:36 rmq_broker/documentation/mixins/pydantic/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-26 07:16 rmq_broker/queues/__init__.py
--rw-r--r--  2.0 unx     1107 b- defN 23-May-26 07:16 rmq_broker/queues/base.py
--rw-r--r--  2.0 unx     1765 b- defN 23-May-26 07:16 rmq_broker/queues/rabbitmq.py
--rw-r--r--  2.0 unx     1074 b- defN 23-Jul-27 11:28 rabbitmq_broker-1.1.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     4405 b- defN 23-Jul-27 11:28 rabbitmq_broker-1.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-27 11:28 rabbitmq_broker-1.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jul-27 11:28 rabbitmq_broker-1.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2104 b- defN 23-Jul-27 11:28 rabbitmq_broker-1.1.5.dist-info/RECORD
-24 files, 43088 bytes uncompressed, 13555 bytes compressed:  68.5%
+-rw-r--r--  2.0 unx     1083 b- defN 23-Aug-02 12:37 rmq_broker/queues/base.py
+-rw-r--r--  2.0 unx     2426 b- defN 23-Aug-02 12:37 rmq_broker/queues/rabbitmq.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-02 12:37 rmq_broker/services/__init__.py
+-rw-r--r--  2.0 unx     3137 b- defN 23-Aug-02 12:37 rmq_broker/services/base.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-02 12:37 rmq_broker/tests/__init__.py
+-rw-r--r--  2.0 unx      908 b- defN 23-Aug-02 12:37 rmq_broker/tests/factories.py
+-rw-r--r--  2.0 unx     2655 b- defN 23-Aug-02 12:37 rmq_broker/tests/test_models.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-02 12:37 rmq_broker/utils/__init__.py
+-rw-r--r--  2.0 unx      257 b- defN 23-Aug-02 12:37 rmq_broker/utils/singleton.py
+-rw-r--r--  2.0 unx     1074 b- defN 23-Aug-02 12:37 rabbitmq_broker-1.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4373 b- defN 23-Aug-02 12:37 rabbitmq_broker-1.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-02 12:37 rabbitmq_broker-1.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Aug-02 12:37 rabbitmq_broker-1.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2696 b- defN 23-Aug-02 12:37 rabbitmq_broker-1.2.0.dist-info/RECORD
+31 files, 55383 bytes uncompressed, 17440 bytes compressed:  68.5%
```

## zipnote {}

```diff
@@ -1,17 +1,17 @@
 Filename: rmq_broker/__init__.py
 Comment: 
 
-Filename: rmq_broker/schemas.py
+Filename: rmq_broker/models.py
 Comment: 
 
-Filename: rmq_broker/settings.py
+Filename: rmq_broker/schemas.py
 Comment: 
 
-Filename: rmq_broker/utils.py
+Filename: rmq_broker/settings.py
 Comment: 
 
 Filename: rmq_broker/async_chains/__init__.py
 Comment: 
 
 Filename: rmq_broker/async_chains/base.py
 Comment: 
@@ -51,23 +51,44 @@
 
 Filename: rmq_broker/queues/base.py
 Comment: 
 
 Filename: rmq_broker/queues/rabbitmq.py
 Comment: 
 
-Filename: rabbitmq_broker-1.1.5.dist-info/LICENSE
+Filename: rmq_broker/services/__init__.py
+Comment: 
+
+Filename: rmq_broker/services/base.py
+Comment: 
+
+Filename: rmq_broker/tests/__init__.py
+Comment: 
+
+Filename: rmq_broker/tests/factories.py
+Comment: 
+
+Filename: rmq_broker/tests/test_models.py
+Comment: 
+
+Filename: rmq_broker/utils/__init__.py
+Comment: 
+
+Filename: rmq_broker/utils/singleton.py
+Comment: 
+
+Filename: rabbitmq_broker-1.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: rabbitmq_broker-1.1.5.dist-info/METADATA
+Filename: rabbitmq_broker-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: rabbitmq_broker-1.1.5.dist-info/WHEEL
+Filename: rabbitmq_broker-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: rabbitmq_broker-1.1.5.dist-info/top_level.txt
+Filename: rabbitmq_broker-1.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: rabbitmq_broker-1.1.5.dist-info/RECORD
+Filename: rabbitmq_broker-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rmq_broker/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.1.5"
+__version__ = "1.2.0"
```

## rmq_broker/schemas.py

```diff
@@ -1,59 +1,29 @@
 from typing import TypedDict
+from uuid import UUID
 
-from schema import Optional, Or, Schema
 from typing_extensions import NotRequired
 
 
-class MessageHeader(TypedDict):
+class BrokerMessageHeader(TypedDict):
     dst: str
     src: str
 
 
-class MessageStatus(TypedDict):
+class BrokerMessageStatus(TypedDict):
     code: int
     message: str
 
 
 class BrokerMessage(TypedDict):
     request_type: str
-    request_id: str
-    header: MessageHeader
+    request_id: UUID
+    header: BrokerMessageHeader
     body: dict
 
 
-class IncomingMessage(BrokerMessage):
-    status: NotRequired[MessageStatus]
+class UnprocessedBrokerMessage(BrokerMessage):
+    status: NotRequired[BrokerMessageStatus]
 
 
-class OutgoingMessage(BrokerMessage):
-    status: MessageStatus
-
-
-PreMessage = Schema(
-    {
-        "request_type": str,
-        "request_id": str,
-        "header": {"src": str, "dst": str},
-        "body": object,
-        Optional("status"): dict,
-    }
-)
-
-
-PostMessage = Schema(
-    {
-        "request_type": str,
-        "request_id": str,
-        "header": {"src": str, "dst": str},
-        "body": object,
-        "status": {"message": str, "code": Or(int, str)},
-    }
-)
-
-MessageTemplate = {
-    "request_type": "",
-    "request_id": "",
-    "header": {"src": "", "dst": ""},
-    "body": {},
-    "status": {"message": "", "code": ""},
-}
+class ProcessedBrokerMessage(BrokerMessage):
+    status: BrokerMessageStatus
```

## rmq_broker/settings.py

```diff
@@ -1,14 +1,20 @@
 import importlib
 
 import environ
 
 env = environ.Env()
 default_path = env("MICROSERVICE_SETTINGS", default="settings")
-paths = [default_path, "config.settings.base", "app.settings", "settings", "application.settings"]
+paths = [
+    default_path,
+    "config.settings.base",
+    "app.settings",
+    "settings",
+    "application.settings",
+]
 settings = ""
 
 
 for path in paths:
     try:
         settings = importlib.import_module(path)
     except ModuleNotFoundError:
```

## rmq_broker/async_chains/base.py

```diff
@@ -1,22 +1,20 @@
 import logging
 from abc import ABC, abstractmethod
 
-from schema import Schema, SchemaError
+from pydantic.error_wrappers import ValidationError
 from starlette import status
 
+from rmq_broker.models import ErrorMessage, ProcessedMessage, UnprocessedMessage
 from rmq_broker.schemas import (
-    IncomingMessage,
-    MessageHeader,
-    MessageTemplate,
-    OutgoingMessage,
-    PostMessage,
-    PreMessage,
+    BrokerMessageHeader,
+    ProcessedBrokerMessage,
+    UnprocessedBrokerMessage,
 )
-from rmq_broker.utils import Singleton
+from rmq_broker.utils.singleton import Singleton
 
 logger = logging.getLogger(__name__)
 
 
 class AbstractChain(ABC):
     """Интерфейс классов обработчиков.
 
@@ -41,61 +39,61 @@
         """
         self.chains[chain.request_type.lower()] = chain
         logger.debug(
             f"{self.__class__.__name__}.add(): {chain.__name__} added to chains."
         )
 
     @abstractmethod
-    async def handle(self, data: IncomingMessage) -> OutgoingMessage:
+    async def handle(self, data: UnprocessedBrokerMessage) -> ProcessedBrokerMessage:
         """
         Вызывает метод handle() у следующего обработчика в цепочке.
 
         Args:
             data (dict): Словарь с запросом.
 
         Returns:
             None: если следующий обработчик не определен.
             Обработанный запрос: если следующий обработчик определен.
         """
         ...
 
     @abstractmethod
-    def get_response_header(self, data: IncomingMessage) -> MessageHeader:
+    def get_response_header(
+        self, data: UnprocessedBrokerMessage
+    ) -> BrokerMessageHeader:
         """
         Изменяет заголовок запроса.
 
         Args:
             data (dict): Словарь с запросом.
         """
         ...  # pragma: no cover
 
     @abstractmethod
-    async def get_response_body(self, data: IncomingMessage) -> OutgoingMessage:
+    async def get_response_body(
+        self, data: UnprocessedBrokerMessage
+    ) -> ProcessedBrokerMessage:
         """
         Изменяет тело запроса.
 
         Args:
             data (dict): Словарь с запросом.
 
         Returns:
             Cловарь c ответом.
         """
         ...  # pragma: no cover
 
-    @abstractmethod
-    def validate(self, data: IncomingMessage) -> None:
-        ...  # pragma: no cover
-
     def form_response(
         self,
-        data: IncomingMessage,
+        data: UnprocessedBrokerMessage,
         body: dict = None,
         code: int = status.HTTP_200_OK,
         message: str = "",
-    ) -> OutgoingMessage:
+    ) -> ProcessedBrokerMessage:
         body = {} if body is None else body
         data.update({"body": body})
         data.update({"status": {"message": str(message), "code": code}})
         logger.debug(
             f"{self.__class__.__name__}.form_response(): Formed response {data=}"
         )
         return data
@@ -120,15 +118,15 @@
     """
 
     request_type: str = ""
     include_in_schema: bool = True
     deprecated: bool = False
     actual: str = ""
 
-    async def handle(self, data: IncomingMessage) -> OutgoingMessage:
+    async def handle(self, data: UnprocessedBrokerMessage) -> ProcessedBrokerMessage:
         """
         Обрабатывает запрос, пропуская его через методы обработки
         заголовка и тела запроса.
 
         Args:
             data (dict): Словарь с запросом.
 
@@ -137,57 +135,54 @@
             и конкретного экземпляра обработчика совпадают.
 
             Метод handle() у родительского класса: если типы запроса переданного сообщения
             и конкретного экземпляра обработчика отличаются.
         """
         logger.info(f"{self.__class__.__name__}.get_response_body(): data={data}")
         try:
-            self.validate(data, PreMessage)
-        except SchemaError as e:
-            logger.error(f"{self.__class__.__name__}.handle(): SchemaError: {e}")
-            return self.form_response(
-                MessageTemplate, {}, status.HTTP_400_BAD_REQUEST, e
-            )
-        response = {}
-        if self.request_type == data["request_type"]:
-            response["request_id"] = data["request_id"]
-            response["request_type"] = data["request_type"]
+            UnprocessedMessage(**data)
+        except ValidationError as error:
+            logger.error(f"{self.__class__.__name__}.handle(): {error}")
+            return ErrorMessage().generate(message=str(error))
+        if self.request_type.lower() == data["request_type"].lower():
+            response = ProcessedMessage().generate()
             try:
                 response.update(await self.get_response_body(data))
                 logger.debug(
                     f"{self.__class__.__name__}.handle(): After body update {response=}"
                 )
-            except Exception as e:
-                return self.form_response(
-                    MessageTemplate, {}, status.HTTP_400_BAD_REQUEST, e
-                )
+            except Exception as exc:
+                return ErrorMessage().generate(message=str(exc))
             response.update(self.get_response_header(data))
             logger.debug(
                 f"{self.__class__.__name__}.handle(): After header update {response=}"
             )
+            # These field must stay the same.
+            response["request_id"] = data["request_id"]
+            response["request_type"] = data["request_type"]
+            logger.debug(
+                f"{self.__class__.__name__}.handle(): Before sending {response=}"
+            )
             try:
-                self.validate(response, PostMessage)
+                ProcessedMessage(**response)
                 return response
-            except SchemaError as e:
-                logger.error(f"{self.__class__.__name__}.handle(): SchemaError: {e}")
-                return self.form_response(
-                    MessageTemplate, {}, status.HTTP_400_BAD_REQUEST, e
+            except ValidationError as error:
+                logger.error(
+                    f"{self.__class__.__name__}.handle(): ValidationError: {error}"
                 )
+                return ErrorMessage().generate(message=str(error))
         else:
             logger.error(
                 f"{self.__class__.__name__}.handle(): Unknown request_type='{data['request_type']}'"
             )
-            return self.form_response(
-                MessageTemplate,
-                {},
-                status.HTTP_400_BAD_REQUEST,
-                "Can't handle this request type",
-            )
+            return ErrorMessage().generate(message="Can't handle this request type")
 
-    def get_response_header(self, data: IncomingMessage) -> MessageHeader:
+    def get_response_header(
+        self, data: UnprocessedBrokerMessage
+    ) -> BrokerMessageHeader:
         """
         Меняет местами получателя('dst') и отправителя('src') запроса.
 
         Args:
             data (dict): Словарь с запросом.
 
         Returns:
@@ -197,52 +192,36 @@
             "header": {"src": data["header"]["dst"], "dst": data["header"]["src"]}
         }
         logger.debug(
             f"{self.__class__.__name__}.get_response_header(): {updated_header=}"
         )
         return updated_header
 
-    def validate(self, message: IncomingMessage, schema: Schema) -> None:
-        """Валидирует сообщение по переданной схеме.
-
-        Raises:
-            SchemaError: Валидация не была пройдена.
-        """
-        schema.validate(message)
-        logger.debug(
-            f"{self.__class__.__name__}.validate(): Successful validation, {message=}"
-        )
-
 
 class ChainManager(BaseChain, Singleton):
     """Единая точка для распределения запросов по обработчикам."""
 
     chains = {}
 
     def __init__(self, parent_chain: BaseChain = BaseChain) -> None:
         """Собирает все обработчики в словарь."""
         if subclasses := parent_chain.__subclasses__():
             for subclass in subclasses:
                 if subclass.request_type:
                     self.add(subclass)
                 self.__init__(subclass)
 
-    async def handle(self, data: IncomingMessage) -> OutgoingMessage:
+    async def handle(self, data: UnprocessedBrokerMessage) -> ProcessedBrokerMessage:
         """Направляет запрос на нужный обработчик."""
         try:
-            self.validate(data, PreMessage)
+            UnprocessedMessage(**data)
             chain = self.chains[data["request_type"].lower()]
             return await chain().handle(data)
-        except SchemaError as e:
-            msg = f"Incoming message validation error: {e}"
-        except KeyError as e:
-            msg = f"Can't handle this request type: {e}"
+        except ValidationError as error:
+            msg = f"Incoming message validation error: {error}"
+        except KeyError as error:
+            msg = f"Can't handle this request type: {error}"
         logger.error(f"{self.__class__.__name__}.handle(): {msg}")
-        return self.form_response(
-            MessageTemplate,
-            {},
-            status.HTTP_400_BAD_REQUEST,
-            msg,
-        )
+        return ErrorMessage().generate(message=msg)
 
     async def get_response_body(self, data):
         pass
```

## rmq_broker/chains/base.py

```diff
@@ -1,31 +1,25 @@
 import logging
 from abc import abstractmethod
 
-from schema import SchemaError
-from starlette import status
+from pydantic.error_wrappers import ValidationError
 
 from rmq_broker.async_chains.base import BaseChain as AsyncBaseChain
 from rmq_broker.async_chains.base import ChainManager as AsyncChainManager
-from rmq_broker.schemas import (
-    IncomingMessage,
-    MessageTemplate,
-    OutgoingMessage,
-    PostMessage,
-    PreMessage,
-)
-from rmq_broker.utils import Singleton
+from rmq_broker.models import ErrorMessage, ProcessedMessage, UnprocessedMessage
+from rmq_broker.schemas import ProcessedBrokerMessage, UnprocessedBrokerMessage
+from rmq_broker.utils.singleton import Singleton
 
 logger = logging.getLogger(__name__)
 
 
 class BaseChain(AsyncBaseChain):
     """Синхронная версия базового класса обработчика."""
 
-    def handle(self, data: IncomingMessage) -> OutgoingMessage:
+    def handle(self, data: UnprocessedBrokerMessage) -> ProcessedBrokerMessage:
         """
         Обрабатывает запрос, пропуская его через методы обработки
         заголовка и тела запроса.
 
         Args:
             data (dict): Словарь с запросом.
 
@@ -34,77 +28,71 @@
             и конкретного экземпляра обработчика совпадают.
 
             Метод handle() у родительского класса: если типы запроса переданного сообщения
             и конкретного экземпляра обработчика отличаются.
         """
         logger.info(f"{self.__class__.__name__}.get_response_body(): data={data}")
         try:
-            self.validate(data, PreMessage)
-        except SchemaError as e:
-            logger.error(f"{self.__class__.__name__}.handle(): SchemaError: {e}")
-            return self.form_response(
-                MessageTemplate, {}, status.HTTP_400_BAD_REQUEST, e
+            UnprocessedMessage(**data)
+        except ValidationError as error:
+            logger.error(
+                f"{self.__class__.__name__}.handle(): ValidationError: {error}"
             )
-        response = {}
+            return ErrorMessage().generate(message=str(error))
         if self.request_type.lower() == data["request_type"].lower():
-            response["request_id"] = data["request_id"]
-            response["request_type"] = data["request_type"]
+            response = ProcessedMessage().generate()
             try:
                 response.update(self.get_response_body(data))
                 logger.debug(
                     f"{self.__class__.__name__}.handle(): After body update {response=}"
                 )
-            except Exception as e:
-                return self.form_response(
-                    MessageTemplate, {}, status.HTTP_400_BAD_REQUEST, e
-                )
+            except Exception as exc:
+                return ErrorMessage().generate(message=str(exc))
             response.update(self.get_response_header(data))
             logger.debug(
                 f"{self.__class__.__name__}.handle(): After header update {response=}"
             )
+            # These field must stay the same.
+            response["request_id"] = data["request_id"]
+            response["request_type"] = data["request_type"]
+            logger.debug(
+                f"{self.__class__.__name__}.handle(): Before sending {response=}"
+            )
             try:
-                self.validate(response, PostMessage)
+                ProcessedMessage(**response)
                 return response
-            except SchemaError as e:
-                logger.error(f"{self.__class__.__name__}.handle(): SchemaError: {e}")
-                return self.form_response(
-                    MessageTemplate, {}, status.HTTP_400_BAD_REQUEST, e
+            except ValidationError as error:
+                logger.error(
+                    f"{self.__class__.__name__}.handle(): ValidationError: {error}"
                 )
+                return ErrorMessage().generate(message=str(error))
         else:
             logger.error(
                 f"{self.__class__.__name__}.handle(): Unknown request_type='{data['request_type']}'"
             )
-            return self.form_response(
-                MessageTemplate,
-                {},
-                status.HTTP_400_BAD_REQUEST,
-                "Can't handle this request type",
-            )
+            return ErrorMessage().generate(message="Can't handle this request type")
 
     @abstractmethod
-    def get_response_body(self, data: IncomingMessage) -> OutgoingMessage:
+    def get_response_body(
+        self, data: UnprocessedBrokerMessage
+    ) -> ProcessedBrokerMessage:
         ...
 
 
 class ChainManager(AsyncChainManager, Singleton):
     """Синхронная версия менеджера распределения запросов."""
 
-    def handle(self, data: IncomingMessage) -> OutgoingMessage:
+    def handle(self, data: UnprocessedBrokerMessage) -> ProcessedBrokerMessage:
         """Направляет запрос на нужный обработчик."""
         try:
-            self.validate(data, PreMessage)
+            UnprocessedMessage(**data)
             chain = self.chains[data["request_type"].lower()]
             return chain().handle(data)
-        except SchemaError as e:
-            msg = f"Incoming message validation error: {e}"
-        except KeyError as e:
-            msg = f"Can't handle this request type: {e}"
+        except ValidationError as error:
+            msg = f"Incoming message validation error: {error}"
+        except KeyError as error:
+            msg = f"Can't handle this request type: {error}"
         logger.error(f"{self.__class__.__name__}: handle(data): {msg}")
-        return self.form_response(
-            MessageTemplate,
-            {},
-            status.HTTP_400_BAD_REQUEST,
-            msg,
-        )
+        return ErrorMessage().generate(message=msg)
 
     def get_response_body(self, data):
         pass
```

## rmq_broker/documentation/base.py

```diff
@@ -1,14 +1,14 @@
 from collections import defaultdict
 from typing import Tuple
 
 from rmq_broker.async_chains.base import BaseChain as AsyncBaseChain
 from rmq_broker.async_chains.base import ChainManager
 from rmq_broker.chains.base import BaseChain
-from rmq_broker.schemas import IncomingMessage, OutgoingMessage
+from rmq_broker.schemas import ProcessedBrokerMessage, UnprocessedBrokerMessage
 from rmq_broker.settings import settings
 
 from . import REF_PREFIX
 from .models import OpenAPI
 from .utils import get_class_dir
 
 
@@ -26,18 +26,18 @@
         operation = {
             "tags": [f"RPC: {get_class_dir(chain)}"],
             "summary": name,
             "description": chain.__class__.__doc__,
             "operationId": chain.request_type,
         }
         if chain.deprecated:
-            operation['deprecated'] = True
+            operation["deprecated"] = True
         if chain.actual:
-            operation['deprecated'] = True
-            operation['summary'] += ". Актуальный - " + chain.actual + "."
+            operation["deprecated"] = True
+            operation["summary"] += ". Актуальный - " + chain.actual + "."
         request_body = {
             "required": required,
         }
         if required:
             model_name = model_name_map.get(chain.body_model)
             request_body["content"] = {
                 "application/json": {"schema": {"$ref": f"{REF_PREFIX}{model_name}"}}
@@ -52,15 +52,19 @@
         self,
         chain_manager: ChainManager,
     ) -> dict:
         output: dict = {
             "openapi": self.openapi_version,
             "info": {"title": self.title, "version": self.version},
         }
-        chains = [chain() for chain in chain_manager.chains.values() if chain.include_in_schema]
+        chains = [
+            chain()
+            for chain in chain_manager.chains.values()
+            if chain.include_in_schema
+        ]
         components: dict = {}
         paths = defaultdict(dict)
 
         typed_requests = [
             chain.body_model for chain in chains if getattr(chain, "body_model", None)
         ]
         model_name_map, definitions = self.process_forms(models=typed_requests)
@@ -77,18 +81,22 @@
         output["paths"] = dict(
             sorted(paths.items(), key=lambda i: i[1]["post"]["tags"][0])
         )
         return OpenAPI(**output).dict(by_alias=True, exclude_none=True)
 
 
 class DocsChain(BaseDocsChain, BaseChain):
-    def get_response_body(self, data: IncomingMessage) -> OutgoingMessage:
+    def get_response_body(
+        self, data: UnprocessedBrokerMessage
+    ) -> ProcessedBrokerMessage:
         if not self.openapi:
             self.openapi = self.make_openapi(chain_manager=ChainManager())
         return self.form_response(data, self.openapi)
 
 
 class AsyncDocsChain(BaseDocsChain, AsyncBaseChain):
-    async def get_response_body(self, data: IncomingMessage) -> OutgoingMessage:
+    async def get_response_body(
+        self, data: UnprocessedBrokerMessage
+    ) -> ProcessedBrokerMessage:
         if not self.openapi:
             self.openapi = self.make_openapi(chain_manager=ChainManager())
         return self.form_response(data, self.openapi)
```

## rmq_broker/queues/base.py

```diff
@@ -13,15 +13,14 @@
         """Создает необходимые атрибуты для подключения к брокеру сообщений."""
         if self.MessageQueue == "":
             raise AttributeError("Broker name has not been set.")
         self.config = settings.CONSUMERS.get(self.MessageQueue)
         self.broker_url = self.config["broker_url"]
         self.connection = None
         self.client_properties = None
-        self.rpc = None
         logger.debug("%s: Initialized" % self.__class__.__name__)
 
     @abstractmethod
     async def __aenter__(self):
         pass
 
     @abstractmethod
```

## rmq_broker/queues/rabbitmq.py

```diff
@@ -1,38 +1,52 @@
 import asyncio
 import logging
 
 import aio_pika
 from aio_pika.patterns import RPC
-from schema import SchemaError
+from pydantic.error_wrappers import ValidationError
 
+from rmq_broker.models import ErrorMessage, ProcessedMessage, UnprocessedMessage
 from rmq_broker.queues.base import AsyncAbstractMessageQueue
-from rmq_broker.schemas import PreMessage
+from rmq_broker.schemas import ProcessedBrokerMessage, UnprocessedBrokerMessage
 
 logger = logging.getLogger(__name__)
 
 
 class AsyncRabbitMessageQueue(AsyncAbstractMessageQueue):
     MessageQueue: str = "rabbitmq"
 
     async def consume(self) -> None:
         logger.info("%s.consume: RPC consumer started" % self.__class__.__name__)
         await asyncio.Future()
 
-    async def post_message(self, data, worker):
+    async def post_message(
+        self, data: UnprocessedBrokerMessage, worker: str
+    ) -> ProcessedBrokerMessage:
         try:
-            PreMessage.validate(data)
-        except SchemaError as e:
+            UnprocessedMessage(**data)
+        except ValidationError as error:
             logger.error(
-                "{}.post_message: Message validation failed!: {}".format(
-                    self.__class__.__name__, e
+                "{}.post_message: UnprocessedMessage validation failed!: {}".format(
+                    self.__class__.__name__, error
                 )
             )
-        else:
-            return await self.rpc.call(worker, kwargs=dict(data=data))
+            return ErrorMessage().generate(message=str(error))
+        response = await self.rpc.call(worker, kwargs=dict(data=data))
+        try:
+            ProcessedMessage(**response)
+        except ValidationError as error:
+            return ErrorMessage().generate(
+                request_id=data["request_id"],
+                request_type=data["request_type"],
+                dst=data["src"],
+                src=data["dst"],
+                message=str(error),
+            )
+        return response
 
     async def register_tasks(self, routing_key: str, worker: callable):
         """Вызывать перед стартом консьюмера."""
         await self.rpc.register(routing_key, worker, auto_delete=True)
 
     async def __aenter__(self):
         """
```

## Comparing `rabbitmq_broker-1.1.5.dist-info/LICENSE` & `rabbitmq_broker-1.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rabbitmq_broker-1.1.5.dist-info/METADATA` & `rabbitmq_broker-1.2.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: rabbitmq-broker
-Version: 1.1.5
+Version: 1.2.0
 Summary: RPC брокер сообщений
 Author-email: Nikita Sysoev <njt55cs@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aio-pika (~=9.0.2)
 Requires-Dist: django-environ (~=0.9.0)
-Requires-Dist: schema (~=0.7.5)
 Requires-Dist: starlette (~=0.25.0)
 
 # RabbitMQ Broker
 [![Python versions](https://img.shields.io/badge/python-%3E=3.9-blue)](https://www.python.org/)
 [![Docker version](https://img.shields.io/badge/Docker-23.0.1-blue)](https://www.docker.com//)
 [![](https://img.shields.io/badge/-FastAPI-green)](https://fastapi.tiangolo.com/)
 [![Black code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
```

## Comparing `rabbitmq_broker-1.1.5.dist-info/RECORD` & `rabbitmq_broker-1.2.0.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,31 @@
-rmq_broker/__init__.py,sha256=KlgaVSJ1AQxCDJZgh4wFk-gpem-k9PfebW8U3hiKJD4,22
-rmq_broker/schemas.py,sha256=1XNpJKdyX34IU1RGnpVpYdH5LgzQfejDT7pAi27_mWg,1080
-rmq_broker/settings.py,sha256=Xe-HSUjcZcQw1DSnchItGFn_E6b4rwuwrHyFo8zFYdg,532
-rmq_broker/utils.py,sha256=en9PcLeHH6ZZ4QWllXmGDcBoUYEHbGhIbpNT1cmfQlA,257
+rmq_broker/__init__.py,sha256=MpAT5hgNoHnTtG1XRD_GV_A7QrHVU6vJjGSw_8qMGA4,22
+rmq_broker/models.py,sha256=IBfK_Q-r1j3jQBLKDv65WXOJvTwpBo3xsBCcZ2EhjAQ,5249
+rmq_broker/schemas.py,sha256=UvM4-nD9KAEEQ1LBGdxzYcQY7IRHKvmYS-DuZJjziho,528
+rmq_broker/settings.py,sha256=mZt6t_qwbGugpPJlZ25o0E7R2umquE3xvCOnm0s8P5Y,555
 rmq_broker/async_chains/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-rmq_broker/async_chains/base.py,sha256=ZaVG1trd2XX1Iku64LfwoFh831ZIBLVVI7xmNdMlTWw,9326
+rmq_broker/async_chains/base.py,sha256=DFWll6AOIh_MNghjSYUg0I9GgTsIo7LeBhLjfUyKESo,8889
 rmq_broker/chains/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-rmq_broker/chains/base.py,sha256=UCCkAcO0QLoZBhnygxxSOsB9nOiRMYGxZAuZ4zdy5Us,4333
+rmq_broker/chains/base.py,sha256=ey00N0qaw6Dxkugj9QzoxCUbZ2lIYlYm5wULDQorKv0,4326
 rmq_broker/documentation/__init__.py,sha256=-JASC9CfKyUXByBfarQKfYyhIMF77gz_UUCH4aiQ7UY,37
-rmq_broker/documentation/base.py,sha256=F78FwbFJpw9rWjWO8i1hDwyC8d66HGiM_nP_S4Dpuyc,3577
+rmq_broker/documentation/base.py,sha256=vKs9jWoMnlG76K8S6OE3e7VPI3M-9NlA47_05lA15PI,3699
 rmq_broker/documentation/models.py,sha256=YA84fcsPVjTwcM7t8pMMBT9MJ4acKc24IOAq71S-OM0,10645
 rmq_broker/documentation/utils.py,sha256=ej76hHKJFAh73xZ2_wDo4aQrpxxhCQqA_7W599fCYGE,136
 rmq_broker/documentation/mixins/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 rmq_broker/documentation/mixins/pydantic/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 rmq_broker/documentation/mixins/pydantic/chains.py,sha256=vZsVZA4WdEp1FisayPvBAaDnvjp0lgtvjT9ZXYHbjbA,1278
 rmq_broker/documentation/mixins/pydantic/utils.py,sha256=3IAa7--LakKyyfcFcsfbOScSppYOyNNrmX42RpY3EsI,1307
 rmq_broker/queues/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-rmq_broker/queues/base.py,sha256=XgUIn04MxoulYjN-v8LVcPKprmiSHy9UmKTzoBfyBug,1107
-rmq_broker/queues/rabbitmq.py,sha256=cujY9KKwld146SEyCHhcXe08cgHxRn3ARIxOfXuIViQ,1765
-rabbitmq_broker-1.1.5.dist-info/LICENSE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
-rabbitmq_broker-1.1.5.dist-info/METADATA,sha256=4Joo4xQeC-iLz4tHYYYh0EMQ75I0rytluncYkmReNe0,4405
-rabbitmq_broker-1.1.5.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-rabbitmq_broker-1.1.5.dist-info/top_level.txt,sha256=gyiGN4_aIuuxH76M_A_yn64Bxy2nj4fFJ1C84g3BPQQ,11
-rabbitmq_broker-1.1.5.dist-info/RECORD,,
+rmq_broker/queues/base.py,sha256=KsNBqvVOzmimov0u5Zwf98IifjR6cupJoDs181nR9Sk,1083
+rmq_broker/queues/rabbitmq.py,sha256=c18--zuSzkF9jNlX1OiB7KIF2238OYT6P78m8RZ2EoE,2426
+rmq_broker/services/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+rmq_broker/services/base.py,sha256=cB6Nq205KHWxoCt12Hug8FPbdLgMzq2bf77Yn73TXxk,3137
+rmq_broker/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+rmq_broker/tests/factories.py,sha256=Y_3pavH3vFsHrb3yStdRZlGs6rK7J0bc8qxyYfsddCs,908
+rmq_broker/tests/test_models.py,sha256=zwT8br7Zc3wEMVd34Cv4kwZW1awLGusHSSj_T6kQ_u0,2655
+rmq_broker/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+rmq_broker/utils/singleton.py,sha256=en9PcLeHH6ZZ4QWllXmGDcBoUYEHbGhIbpNT1cmfQlA,257
+rabbitmq_broker-1.2.0.dist-info/LICENSE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
+rabbitmq_broker-1.2.0.dist-info/METADATA,sha256=Dt0AYeOTmWOJkmpJDedZ8A7gyFegQR5UW3wH0_l2mNU,4373
+rabbitmq_broker-1.2.0.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+rabbitmq_broker-1.2.0.dist-info/top_level.txt,sha256=gyiGN4_aIuuxH76M_A_yn64Bxy2nj4fFJ1C84g3BPQQ,11
+rabbitmq_broker-1.2.0.dist-info/RECORD,,
```

