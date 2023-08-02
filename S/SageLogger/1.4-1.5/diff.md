# Comparing `tmp/SageLogger-1.4.tar.gz` & `tmp/SageLogger-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SageLogger-1.4.tar", last modified: Sun Jul 23 12:41:12 2023, max compression
+gzip compressed data, was "SageLogger-1.5.tar", last modified: Wed Aug  2 08:57:26 2023, max compression
```

## Comparing `SageLogger-1.4.tar` & `SageLogger-1.5.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 12:41:11.097313 SageLogger-1.4/
--rw-rw-rw-   0        0        0    13846 2023-07-23 12:41:11.096313 SageLogger-1.4/PKG-INFO
--rw-rw-rw-   0        0        0    13254 2023-07-23 12:39:38.000000 SageLogger-1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-23 12:41:08.920719 SageLogger-1.4/SageLogger/
--rw-rw-rw-   0        0        0    13884 2023-07-23 12:09:10.000000 SageLogger-1.4/SageLogger/Logger.py
--rw-rw-rw-   0        0        0     1093 2023-07-23 12:11:42.000000 SageLogger-1.4/SageLogger/SageException.py
--rw-rw-rw-   0        0        0     3143 2023-07-23 12:31:15.000000 SageLogger-1.4/SageLogger/SageFactory.py
--rw-rw-rw-   0        0        0       15 2023-07-22 20:32:47.000000 SageLogger-1.4/SageLogger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-23 12:41:10.923952 SageLogger-1.4/SageLogger.egg-info/
--rw-rw-rw-   0        0        0    13846 2023-07-23 12:41:08.000000 SageLogger-1.4/SageLogger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2023-07-23 12:41:08.000000 SageLogger-1.4/SageLogger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 12:41:08.000000 SageLogger-1.4/SageLogger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-07-23 12:41:08.000000 SageLogger-1.4/SageLogger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-23 12:41:08.000000 SageLogger-1.4/SageLogger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      659 2023-07-23 12:40:48.000000 SageLogger-1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-23 12:41:11.097313 SageLogger-1.4/setup.cfg
--rw-rw-rw-   0        0        0     1067 2023-07-23 12:40:53.000000 SageLogger-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:57:26.013739 SageLogger-1.5/
+-rw-rw-rw-   0        0        0    12915 2023-08-02 08:57:26.013739 SageLogger-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0    12205 2023-08-02 08:54:53.000000 SageLogger-1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 08:57:25.983862 SageLogger-1.5/SageLogger/
+-rw-rw-rw-   0        0        0    13645 2023-08-02 08:53:19.000000 SageLogger-1.5/SageLogger/Logger.py
+-rw-rw-rw-   0        0        0     1062 2023-08-02 08:48:59.000000 SageLogger-1.5/SageLogger/SageException.py
+-rw-rw-rw-   0        0        0     3060 2023-08-02 08:48:59.000000 SageLogger-1.5/SageLogger/SageFactory.py
+-rw-rw-rw-   0        0        0       15 2023-08-02 08:48:59.000000 SageLogger-1.5/SageLogger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:57:25.987674 SageLogger-1.5/SageLogger.egg-info/
+-rw-rw-rw-   0        0        0    12915 2023-08-02 08:57:25.000000 SageLogger-1.5/SageLogger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-08-02 08:57:25.000000 SageLogger-1.5/SageLogger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 08:57:25.000000 SageLogger-1.5/SageLogger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-08-02 08:57:25.000000 SageLogger-1.5/SageLogger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-02 08:57:25.000000 SageLogger-1.5/SageLogger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 08:57:26.013739 SageLogger-1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1030 2023-08-02 08:55:39.000000 SageLogger-1.5/setup.py
```

### Comparing `SageLogger-1.4/PKG-INFO` & `SageLogger-1.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,288 +1,269 @@
-Metadata-Version: 2.1
-Name: SageLogger
-Version: 1.4
-Summary: Yet another python logger, or is it like any other?
-Home-page: https://github.com/PanSageYT/SageLogger
-Author: PanSageYT
-Author-email: PanSageYT <pansage@hugedick.fyi>
-Project-URL: Homepage, https://github.com/PanSageYT/SageLogger
-Project-URL: Bug Tracker, https://github.com/PanSageYT/SageLogger/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
-# SageLogger: Python Logger Package
-
-SageLogger is a versatile Python logger package that allows you to create loggers with both remote and local capabilities. The core module, "SageFactory.py," facilitates the creation of loggers with options for SageRemoteLogger (remote) and SageLogger (local). When using SageLogger, you have the flexibility to choose from 7 predefined log types for local logging: DEFAULT, POSITIVE, ONHOLD, NEGATIVE, FROZEN, INFORMATION, and MILD_EXCEPTION. Additionally, you can easily create custom log types to suit your specific needs using the `SageLogger.DynamicType` class.
-
-## Features
-
-### Local Logging Options
-SageLogger offers 7 built-in log types for local logging:
-
-1. DEFAULT: The default log type.
-2. POSITIVE: For positive events and actions.
-3. ONHOLD: To indicate events that are on hold or waiting for further action.
-4. NEGATIVE: For negative events or errors.
-5. FROZEN: To represent frozen states or events.
-6. INFORMATION: For general information logging.
-7. MILD_EXCEPTION: To log minor exceptions or errors.
-8. DEBUG: To troubleshoot some things. (disabled by default)
-
-### Custom Local Log Types
-Apart from the predefined log types, you can create custom log types using the `SageLogger.DynamicType.fromChar` method or the `SageLogger.DynamicType.fromColoredChar` method for colored logs.
-
-### Remote Logging
-SageLogger enables remote logging capabilities through the SageRemoteLogger class. You can load custom APIs for remote logging, and it also provides built-in support for Discord webhook integration.
-
-## Example Code
-
-To create a local logger with SageLogger, you can use the following code:
-
-```python
-from SageLogger import SageFactory, Logger
-import colorama
-
-sagelogs = SageFactory.create("tester", True)
-
-sagelogs.log("Checking all types")
-
-for x in sagelogs.Type.__iter__():
-    sagelogs.log("Hello World! It's " + x.name, type=x)
-
-sagelogs.log("It's dynamic!", type=sagelogs.DynamicType.fromChar(sagelogs, "XD"))
-
-sagelogs.log("Doing the test again but with changed borders")
-
-sagelogs.customization.set_border_style(colorama.Fore.GREEN, "()")
-
-for x in sagelogs.Type.__iter__():
-    sagelogs.log("Hello World! It's " + x.name, type=x)
-
-sagelogs.log("It's dynamic!", type=sagelogs.DynamicType.fromColoredChar(sagelogs, colorama.Fore.LIGHTYELLOW_EX, "X"))
-
-sagelogs.log("I'm ID 21", type=sagelogs.DynamicType.fromColoredChar(sagelogs, colorama.Fore.LIGHTYELLOW_EX, "N"), id=20)
-
-sagelogs.log("I have time", type=sagelogs.DynamicType.fromColoredChar(sagelogs, colorama.Fore.LIGHTYELLOW_EX, "N"), date=True)
-sagelogs.log("I have date", type=sagelogs.DynamicType.fromColoredChar(sagelogs, colorama.Fore.LIGHTYELLOW_EX, "N"), time=True)
-sagelogs.log("I have time and date", type=sagelogs.DynamicType.fromColoredChar(sagelogs, colorama.Fore.LIGHTYELLOW_EX, "N"), time=True, date=True)
-sagelogs.log("I have time and date", type=sagelogs.DynamicType.fromColoredChar(sagelogs, colorama.Fore.LIGHTYELLOW_EX, "N"), time=True, date=True, timecolor=colorama.Fore.YELLOW, datecolor=colorama.Fore.RED)
-
-sageremotelog = SageFactory.create_discord_webhook_remote("<webhook>", savetofile=True)
-
-sagelogs.log("Sent to discord", type=sagelogs.Type.INFORMATION)
-sageremotelog.log("I sent to discord!")
-```
-
-IntelliSense should show you around!
-
-### Big issue:
-In log files it writes color codes.
-
-### Version naming:
-First number: Which major release
-Second number: Which minor release
-Third number: Which revision
-No third number indicates that there was no revisions/the version will stay as it is.
-If you catch a release that contains the third number, then you should remove and upgrade to the 2 number release - the 3 number are considered obsolete.
-
-### Changelogs:
-v1.0 - Initial version
-v1.1 - Skipped as of a fail in version naming :(
-v1.2 - Skipped as of a fail in version naming :(
-v1.3 - Logger arrays in SageFactory and getLoggerByName(name), 3 more loggers (1 secret shh). More functions of enabling, changed class name from SageLogger.Logger.SageLogger to SageLogger.Logger.SageConsoleLogger
-v1.4 - Forced release because I forgot to change sample code from README.md
-
-# 
-#  ____       _       ____  U _____ u  _       U  ___ u   ____     ____  U _____ u   ____          ____      U  ___ u   ____  ____     
-# / __"| uU  /"\\  uU /"___|u\\| ___"|/ |"|       \\/"_ \\/U /"___|uU /"___|u\\| ___"|/U |  _"\\ u      |  _"\\      \\/"_ \\/U /"___|/ __"| u  
-#<\\___ \\/  \\/ _ \\/ \\| |  _ / |  _|" U | | u     | | | |\\| |  _ /\\| |  _ / |  _|"   \\| |_) |/     /| | | |     | | | |\\| | u <\\___ \\/   
-# u___) |  / ___ \\  | |_| |  | |___  \\| |/__.-,_| |_| | | |_| |  | |_| |  | |___    |  _ <       U| |_| |\\.-,_| |_| | | |/__ u___) |   
-# |____/>>/_/   \\_\\  \\____|  |_____|  |_____|\\_)-\\___/   \\____|   \\____|  |_____|   |_| \\_\\       |____/ u \\_)-\\___/   \\____||____/>>  
-#  )(  (__)\\\\    >>  _)(|_   <<   >>  //  \\\\      \\\\     _)(|_    _)(|_   <<   >>   //   \\\\_       |||_         \\\\    _// \\\\  )(  (__) 
-# (__)    (__)  (__)(__)__) (__) (__)(_")("_)    (__)   (__)__)  (__)__) (__) (__) (__)  (__)     (__)_)       (__)  (__)(__)(__)      
-#
-
-# SageFactory.py
-
-`SageFactory.py` is a Python module that provides logging functionalities through the `Logger` module.
-
-## Functions
-
-### getLoggerByName(name: str) -> Logger
-- Description: Returns a logger object by name.
-- Parameters:
-  - `name` (str): The name of the logger to retrieve.
-- Returns:
-  - (Logger): The logger object if found, otherwise `None`.
-
-### create(name: str = "", savetofile: bool = False, logfile: str = "log") -> Logger
-- Description: Creates a console logger and adds it to the list of loggers.
-- Parameters:
-  - `name` (str, optional): The name of the logger. Default is an empty string.
-  - `savetofile` (bool, optional): Whether to save logs to a file. Default is `False`.
-  - `logfile` (str, optional): The filename to save logs. Default is "log".
-- Returns:
-  - (Logger): The created console logger.
-
-### create_remote(method, url, headers, body, name: str = "", savetofile: bool = False, logfile: str = "log") -> Logger
-- Description: Creates a remote logger and adds it to the list of loggers.
-- Parameters:
-  - `method`: The HTTP method to use for the remote logger.
-  - `url`: The URL to send logs to.
-  - `headers`: The headers to be included in the request.
-  - `body`: The log payload.
-  - `name` (str, optional): The name of the logger. Default is an empty string.
-  - `savetofile` (bool, optional): Whether to save logs to a file. Default is `False`.
-  - `logfile` (str, optional): The filename to save logs. Default is "log".
-- Returns:
-  - (Logger): The created remote logger.
-
-### create_discord_webhook_remote(url, name: str = "", savetofile: bool = False, logfile: str = "log") -> Logger
-- Description: Creates a Discord webhook logger and adds it to the list of loggers.
-- Parameters:
-  - `url`: The Discord webhook URL to send logs to.
-  - `name` (str, optional): The name of the logger. Default is an empty string.
-  - `savetofile` (bool, optional): Whether to save logs to a file. Default is `False`.
-  - `logfile` (str, optional): The filename to save logs. Default is "log".
-- Returns:
-  - (Logger): The created Discord webhook logger.
-
-### create_temporary() -> Logger
-- Description: Creates a temporary logger and adds it to the list of loggers.
-- Returns:
-  - (Logger): The created temporary logger.
-
-## Usage
-
-Example usage:
-```python
-from SageFactory import create
-
-# Create a console logger with name "MyLogger" and save logs to file "mylog.txt"
-console_logger = create(name="MyLogger", savetofile=True, logfile="mylog.txt")
-
-# Create a remote logger with custom HTTP method, URL, headers, and log payload
-remote_logger = create_remote(method="POST", url="https://example.com/log", headers={"Authorization": "Bearer XXX"}, body={"message": "Log message"})
-
-# Create a Discord webhook logger with the webhook URL
-discord_logger = create_discord_webhook_remote(url="https://discord.com/api/webhooks/XXX")
-
-# Create a temporary logger with default settings
-temporary_logger = create_temporary()
-```
-
-# SageException.py
-
-`SageException.py` is a Python module that defines custom exception classes used in the SageFactory module.
-
-## Custom Exception Classes
-
-### NoLogPlaceholder
-- Description: This exception is raised when there is an attempt to use a log placeholder that has not been defined.
-
-## NotDiscordWebhook
-- Description: This exception is raised when there is an attempt to use a non-Discord webhook logger in a Discord webhook context.
-
-## UhOhSomeoneTooCurious
-- Description: This exception is raised when a user is being too curious or attempting unauthorized actions.
-
-This file should be used to catch errors.
-
-# Logger.py
-
-`Logger.py` is a Python module that provides logging functionalities through custom logger classes.
-
-## Classes
-
-### SageConsoleLogger
-- Description: Provides console logging capabilities.
-- Methods:
-  - `is_enabled_type(type)`: Checks if the given log type is enabled.
-  - `log(message, type = Type.DEFAULT.value, color = colorama.Fore.RESET, id = -2137, date = False, time = False, datecolor = colorama.Fore.RESET, timecolor = colorama.Fore.RESET, showname = True, ending = "\n")`: Logs a message with the specified log type and customization options.
-  - `ask(message, type = Type.DEFAULT.value, color = colorama.Fore.RESET, answercolor = colorama.Fore.RESET, id = -2137, date = False, time = False, datecolor = colorama.Fore.RESET, timecolor = colorama.Fore.RESET)`: Asks a question with the specified log type and customization options.
-
-### SageRemoteLogger (Based on SageConsoleLogger)
-- Description: Provides remote logging capabilities using HTTP requests.
-- Methods:
-  - `log(message, print_on_console = False, ending = "\n")`: Logs a message and sends it remotely using an HTTP request.
-
-### SageDiscordWebhookLogger
-- Description: Creates a Discord webhook logger using SageRemoteLogger.
-- Methods:
-  - `create(url, name = "", savetofile = False, logfile = "log")`: Creates a Discord webhook logger.
-
-### SageConsoleLogger.customization
-- Description: Customizes log message appearance.
-- Methods:
-  - `set_border_style(border_colorama, borders)`: Sets the border style for log messages.
-  - `setup_custom_border(cos)`: Sets up a custom border for the log message.
-
-### SageConsoleLogger.Type
-- Description: Enumerates different log types with customizations.
-- Properties: `DEFAULT`, `POSITIVE`, `ONHOLD`, `NEGATIVE`, `FROZEN`, `INFORMATION`, `MILD_EXCEPTION`, `DEBUG`, `AMONGUS`, `SAGE_LOGGER_DEBUG`
-- Methods:
-  - `toggle_type(type)`: Toggles the given log type on/off.
-  - `enable_type(type)`: Enables the given log type.
-  - `disable_type(type)`: Disables the given log type.
-
-### SageConsoleLogger.Type.XYZ (PartType)
-- Description: Defines a part of a log type with customization options.
-- Properties: `name`, `Id`, `customization`, `value`, `enabled`, `lockedup`
-
-### DynamicType
-- Description: Represents dynamic log types.
-- Methods:
-  - `fromChar(logger, char)`: Creates a dynamic log type from a character.
-  - `fromColoredChar(logger, color, char)`: Creates a dynamic log type from a colored character.
-  - `custom(prefix)`: Creates a custom dynamic log type.
-
-## Usage
-
-Example usage (SageConsoleLogger):
-```python
-from Logger import SageConsoleLogger
-
-# Create a console logger with name "MyLogger" and save logs to file "mylog.txt"
-console_logger = SageConsoleLogger(name="MyLogger", savetofile=True, logfile="mylog.txt")
-
-# Log a message with the default log type
-console_logger.log("This is a log message.")
-
-# Enable the "POSITIVE" log type and log a message with that type
-console_logger.enable_type(SageConsoleLogger.Type.POSITIVE)
-console_logger.log("This is a positive message.", type=SageConsoleLogger.Type.POSITIVE.value, color=colorama.Fore.GREEN)
-
-# Disable the "DEFAULT" log type and log a message with that type
-console_logger.disable_type(SageConsoleLogger.Type.DEFAULT)
-console_logger.log("This message will not be displayed.", type=SageConsoleLogger.Type.DEFAULT.value)
-```
-
-Example usage (SageRemoteLogger):
-```python
-from Logger import SageRemoteLogger
-
-# Create a remote logger with custom HTTP method, URL, headers, and log payload
-remote_logger = SageRemoteLogger("POST", "https://example.com/log", {"Authorization": "Bearer XXX"}, {"message": "Log message"})
-
-# Log a message and send it remotely
-remote_logger.log("This is a remote log message.")
-```
-
-Example usage (SageDiscordWebhookLogger):
-```python
-from Logger import SageDiscordWebhookLogger
-
-# Create a Discord webhook logger with the webhook URL
-discord_logger = SageDiscordWebhookLogger.create(url="https://discord.com/api/webhooks/XXX")
-
-# Log a message and send it to the Discord webhook
-discord_logger.log("This is a log message sent via Discord webhook.")
-```
-
-## Note
-
-Make sure to import the necessary modules (colorama, datetime, requests, etc.) before using the logger classes.
-For Logger.py the docs in the file aren't available.
+# SageLogger: Python Logger Package
+
+SageLogger is a versatile Python logger package that allows you to create loggers with both remote and local capabilities. The core module, "SageFactory.py," facilitates the creation of loggers with options for SageRemoteLogger (remote) and SageLogger (local). When using SageLogger, you have the flexibility to choose from 7 predefined log types for local logging: DEFAULT, POSITIVE, ONHOLD, NEGATIVE, FROZEN, INFORMATION, and MILD_EXCEPTION. Additionally, you can easily create custom log types to suit your specific needs using the `SageLogger.DynamicType` class.
+
+## Features
+
+### Local Logging Options
+SageLogger offers 9 built-in log types for local logging:
+
+1. DEFAULT: The default log type.
+2. POSITIVE: For positive events and actions.
+3. ONHOLD: To indicate events that are on hold or waiting for further action.
+4. NEGATIVE: For negative events or errors.
+5. FROZEN: To represent frozen states or events.
+6. INFORMATION: For general information logging.
+7. MILD_EXCEPTION: To log minor exceptions or errors.
+8. DEBUG: To troubleshoot some things. (disabled by default)
+9. .................................... (shh secret)
+
+### Custom Local Log Types
+Apart from the predefined log types, you can create custom log types using the `SageLogger.DynamicType.fromChar` method or the `SageLogger.DynamicType.fromColoredChar` method for colored logs.
+
+### Remote Logging
+SageLogger enables remote logging capabilities through the SageRemoteLogger class. You can load custom APIs for remote logging, and it also provides built-in support for Discord webhook integration.
+
+## Example Code
+
+To create a local logger with SageLogger, you can use the following code:
+
+```python
+from SageLogger import SageFactory, Logger
+import colorama
+
+sagelogs = SageFactory.create("tester", True)
+
+sagelogs.log("Checking all types")
+
+for x in sagelogs.Type.__iter__():
+    sagelogs.log("Hello World! It's " + x.name, type=x)
+
+sagelogs.log("It's dynamic!", type=sagelogs.DynamicType.fromChar(sagelogs, "XD"))
+
+sagelogs.log("Doing the test again but with changed borders")
+
+sagelogs.customization.set_border_style(colorama.Fore.GREEN, "()")
+
+for x in sagelogs.Type.__iter__():
+    sagelogs.log("Hello World! It's " + x.name, type=x)
+
+sagelogs.log("It's dynamic!", type=sagelogs.DynamicType.fromColoredChar(sagelogs, colorama.Fore.LIGHTYELLOW_EX, "X"))
+
+sagelogs.log("I'm ID 21", type=sagelogs.DynamicType.fromColoredChar(sagelogs, colorama.Fore.LIGHTYELLOW_EX, "N"), id=20)
+
+sagelogs.log("I have time", type=sagelogs.DynamicType.fromColoredChar(sagelogs, colorama.Fore.LIGHTYELLOW_EX, "N"), date=True)
+sagelogs.log("I have date", type=sagelogs.DynamicType.fromColoredChar(sagelogs, colorama.Fore.LIGHTYELLOW_EX, "N"), time=True)
+sagelogs.log("I have time and date", type=sagelogs.DynamicType.fromColoredChar(sagelogs, colorama.Fore.LIGHTYELLOW_EX, "N"), time=True, date=True)
+sagelogs.log("I have time and date", type=sagelogs.DynamicType.fromColoredChar(sagelogs, colorama.Fore.LIGHTYELLOW_EX, "N"), time=True, date=True, timecolor=colorama.Fore.YELLOW, datecolor=colorama.Fore.RED)
+
+sageremotelog = SageFactory.create_discord_webhook_remote("<webhook>", savetofile=True)
+
+sagelogs.log("Sent to discord", type=sagelogs.Type.INFORMATION)
+sageremotelog.log("I sent to discord!")
+```
+
+IntelliSense should show you around!
+
+### Big issue:
+In log files it writes color codes.
+
+### Version naming:
+First number: Which major release
+Second number: Which minor release
+Third number: Which revision
+No third number indicates that there was no revisions/the version will stay as it is.
+If you catch a release that contains the third number, then you should remove and upgrade to the 2 number release - the 3 number are considered obsolete.
+
+### Changelogs:
+v1.0 - Initial version
+v1.1 - Skipped as of a fail in version naming :(
+v1.2 - Skipped as of a fail in version naming :(
+v1.3 - Logger arrays in SageFactory and getLoggerByName(name), 3 more loggers (1 secret shh). More functions of enabling, changed class name from SageLogger.Logger.SageLogger to SageLogger.Logger.SageConsoleLogger
+v1.4 - Forced release because I forgot to change sample code from README.md
+v1.5 - Fixed logger.ask() method so it returns String object (which is the users answer)
+
+# -------------------------
+# SageLogger Documentation:
+# -------------------------
+#
+# SageFactory.py
+
+`SageFactory.py` is a Python module that provides logging functionalities through the `Logger` module.
+
+## Functions
+
+### getLoggerByName(name: str) -> Logger
+- Description: Returns a logger object by name.
+- Parameters:
+  - `name` (str): The name of the logger to retrieve.
+- Returns:
+  - (Logger): The logger object if found, otherwise `None`.
+
+### create(name: str = "", savetofile: bool = False, logfile: str = "log") -> Logger
+- Description: Creates a console logger and adds it to the list of loggers.
+- Parameters:
+  - `name` (str, optional): The name of the logger. Default is an empty string.
+  - `savetofile` (bool, optional): Whether to save logs to a file. Default is `False`.
+  - `logfile` (str, optional): The filename to save logs. Default is "log".
+- Returns:
+  - (Logger): The created console logger.
+
+### create_remote(method, url, headers, body, name: str = "", savetofile: bool = False, logfile: str = "log") -> Logger
+- Description: Creates a remote logger and adds it to the list of loggers.
+- Parameters:
+  - `method`: The HTTP method to use for the remote logger.
+  - `url`: The URL to send logs to.
+  - `headers`: The headers to be included in the request.
+  - `body`: The log payload.
+  - `name` (str, optional): The name of the logger. Default is an empty string.
+  - `savetofile` (bool, optional): Whether to save logs to a file. Default is `False`.
+  - `logfile` (str, optional): The filename to save logs. Default is "log".
+- Returns:
+  - (Logger): The created remote logger.
+
+### create_discord_webhook_remote(url, name: str = "", savetofile: bool = False, logfile: str = "log") -> Logger
+- Description: Creates a Discord webhook logger and adds it to the list of loggers.
+- Parameters:
+  - `url`: The Discord webhook URL to send logs to.
+  - `name` (str, optional): The name of the logger. Default is an empty string.
+  - `savetofile` (bool, optional): Whether to save logs to a file. Default is `False`.
+  - `logfile` (str, optional): The filename to save logs. Default is "log".
+- Returns:
+  - (Logger): The created Discord webhook logger.
+
+### create_temporary() -> Logger
+- Description: Creates a temporary logger and adds it to the list of loggers.
+- Returns:
+  - (Logger): The created temporary logger.
+
+## Usage
+
+Example usage:
+```python
+from SageFactory import create
+
+# Create a console logger with name "MyLogger" and save logs to file "mylog.txt"
+console_logger = create(name="MyLogger", savetofile=True, logfile="mylog.txt")
+
+# Create a remote logger with custom HTTP method, URL, headers, and log payload
+remote_logger = create_remote(method="POST", url="https://example.com/log", headers={"Authorization": "Bearer XXX"}, body={"message": "Log message"})
+
+# Create a Discord webhook logger with the webhook URL
+discord_logger = create_discord_webhook_remote(url="https://discord.com/api/webhooks/XXX")
+
+# Create a temporary logger with default settings
+temporary_logger = create_temporary()
+```
+
+# SageException.py
+
+`SageException.py` is a Python module that defines custom exception classes used in the SageFactory module.
+
+## Custom Exception Classes
+
+### NoLogPlaceholder
+- Description: This exception is raised when there is an attempt to use a log placeholder that has not been defined.
+
+## NotDiscordWebhook
+- Description: This exception is raised when there is an attempt to use a non-Discord webhook logger in a Discord webhook context.
+
+## UhOhSomeoneTooCurious
+- Description: This exception is raised when a user is being too curious or attempting unauthorized actions.
+
+This file should be used to catch errors.
+
+# Logger.py
+
+`Logger.py` is a Python module that provides logging functionalities through custom logger classes.
+
+## Classes
+
+### SageConsoleLogger
+- Description: Provides console logging capabilities.
+- Methods:
+  - `is_enabled_type(type)`: Checks if the given log type is enabled.
+  - `log(message, type = Type.DEFAULT.value, color = colorama.Fore.RESET, id = -2137, date = False, time = False, datecolor = colorama.Fore.RESET, timecolor = colorama.Fore.RESET, showname = True, ending = "\n")`: Logs a message with the specified log type and customization options.
+  - `ask(message, type = Type.DEFAULT.value, color = colorama.Fore.RESET, answercolor = colorama.Fore.RESET, id = -2137, date = False, time = False, datecolor = colorama.Fore.RESET, timecolor = colorama.Fore.RESET)`: Asks a question with the specified log type and customization options.
+
+### SageRemoteLogger (Based on SageConsoleLogger)
+- Description: Provides remote logging capabilities using HTTP requests.
+- Methods:
+  - `log(message, print_on_console = False, ending = "\n")`: Logs a message and sends it remotely using an HTTP request.
+
+### SageDiscordWebhookLogger
+- Description: Creates a Discord webhook logger using SageRemoteLogger.
+- Methods:
+  - `create(url, name = "", savetofile = False, logfile = "log")`: Creates a Discord webhook logger.
+
+### SageConsoleLogger.customization
+- Description: Customizes log message appearance.
+- Methods:
+  - `set_border_style(border_colorama, borders)`: Sets the border style for log messages.
+  - `setup_custom_border(cos)`: Sets up a custom border for the log message.
+
+### SageConsoleLogger.Type
+- Description: Enumerates different log types with customizations.
+- Properties: `DEFAULT`, `POSITIVE`, `ONHOLD`, `NEGATIVE`, `FROZEN`, `INFORMATION`, `MILD_EXCEPTION`, `DEBUG`, `AMONGUS`, `SAGE_LOGGER_DEBUG`
+- Methods:
+  - `toggle_type(type)`: Toggles the given log type on/off.
+  - `enable_type(type)`: Enables the given log type.
+  - `disable_type(type)`: Disables the given log type.
+
+### SageConsoleLogger.Type.XYZ (PartType)
+- Description: Defines a part of a log type with customization options.
+- Properties: `name`, `Id`, `customization`, `value`, `enabled`, `lockedup`
+
+### DynamicType
+- Description: Represents dynamic log types.
+- Methods:
+  - `fromChar(logger, char)`: Creates a dynamic log type from a character.
+  - `fromColoredChar(logger, color, char)`: Creates a dynamic log type from a colored character.
+  - `custom(prefix)`: Creates a custom dynamic log type.
+
+## Usage
+
+Example usage (SageConsoleLogger):
+```python
+from Logger import SageConsoleLogger
+
+# Create a console logger with name "MyLogger" and save logs to file "mylog.txt"
+console_logger = SageConsoleLogger(name="MyLogger", savetofile=True, logfile="mylog.txt")
+
+# Log a message with the default log type
+console_logger.log("This is a log message.")
+
+# Enable the "POSITIVE" log type and log a message with that type
+console_logger.enable_type(SageConsoleLogger.Type.POSITIVE)
+console_logger.log("This is a positive message.", type=SageConsoleLogger.Type.POSITIVE.value, color=colorama.Fore.GREEN)
+
+# Disable the "DEFAULT" log type and log a message with that type
+console_logger.disable_type(SageConsoleLogger.Type.DEFAULT)
+console_logger.log("This message will not be displayed.", type=SageConsoleLogger.Type.DEFAULT.value)
+```
+
+Example usage (SageRemoteLogger):
+```python
+from Logger import SageRemoteLogger
+
+# Create a remote logger with custom HTTP method, URL, headers, and log payload
+remote_logger = SageRemoteLogger("POST", "https://example.com/log", {"Authorization": "Bearer XXX"}, {"message": "Log message"})
+
+# Log a message and send it remotely
+remote_logger.log("This is a remote log message.")
+```
+
+Example usage (SageDiscordWebhookLogger):
+```python
+from Logger import SageDiscordWebhookLogger
+
+# Create a Discord webhook logger with the webhook URL
+discord_logger = SageDiscordWebhookLogger.create(url="https://discord.com/api/webhooks/XXX")
+
+# Log a message and send it to the Discord webhook
+discord_logger.log("This is a log message sent via Discord webhook.")
+```
+
+## Note
+
+Make sure to import the necessary modules (colorama, datetime, requests, etc.) before using the logger classes.
+For Logger.py the docs in the file aren't available.
```

### Comparing `SageLogger-1.4/README.md` & `SageLogger-1.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,38 @@
+Metadata-Version: 2.1
+Name: SageLogger
+Version: 1.5
+Summary: Yet another python logger, or is it like any other?
+Home-page: https://github.com/PanSageYT/SageLogger
+Author: PanSageYT
+Author-email: pansage@hugedick.fyi
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 # SageLogger: Python Logger Package
 
 SageLogger is a versatile Python logger package that allows you to create loggers with both remote and local capabilities. The core module, "SageFactory.py," facilitates the creation of loggers with options for SageRemoteLogger (remote) and SageLogger (local). When using SageLogger, you have the flexibility to choose from 7 predefined log types for local logging: DEFAULT, POSITIVE, ONHOLD, NEGATIVE, FROZEN, INFORMATION, and MILD_EXCEPTION. Additionally, you can easily create custom log types to suit your specific needs using the `SageLogger.DynamicType` class.
 
 ## Features
 
 ### Local Logging Options
-SageLogger offers 7 built-in log types for local logging:
+SageLogger offers 9 built-in log types for local logging:
 
 1. DEFAULT: The default log type.
 2. POSITIVE: For positive events and actions.
 3. ONHOLD: To indicate events that are on hold or waiting for further action.
 4. NEGATIVE: For negative events or errors.
 5. FROZEN: To represent frozen states or events.
 6. INFORMATION: For general information logging.
 7. MILD_EXCEPTION: To log minor exceptions or errors.
 8. DEBUG: To troubleshoot some things. (disabled by default)
+9. .................................... (shh secret)
 
 ### Custom Local Log Types
 Apart from the predefined log types, you can create custom log types using the `SageLogger.DynamicType.fromChar` method or the `SageLogger.DynamicType.fromColoredChar` method for colored logs.
 
 ### Remote Logging
 SageLogger enables remote logging capabilities through the SageRemoteLogger class. You can load custom APIs for remote logging, and it also provides built-in support for Discord webhook integration.
 
@@ -75,25 +89,20 @@
 
 ### Changelogs:
 v1.0 - Initial version
 v1.1 - Skipped as of a fail in version naming :(
 v1.2 - Skipped as of a fail in version naming :(
 v1.3 - Logger arrays in SageFactory and getLoggerByName(name), 3 more loggers (1 secret shh). More functions of enabling, changed class name from SageLogger.Logger.SageLogger to SageLogger.Logger.SageConsoleLogger
 v1.4 - Forced release because I forgot to change sample code from README.md
+v1.5 - Fixed logger.ask() method so it returns String object (which is the users answer)
 
-# 
-#  ____       _       ____  U _____ u  _       U  ___ u   ____     ____  U _____ u   ____          ____      U  ___ u   ____  ____     
-# / __"| uU  /"\\  uU /"___|u\\| ___"|/ |"|       \\/"_ \\/U /"___|uU /"___|u\\| ___"|/U |  _"\\ u      |  _"\\      \\/"_ \\/U /"___|/ __"| u  
-#<\\___ \\/  \\/ _ \\/ \\| |  _ / |  _|" U | | u     | | | |\\| |  _ /\\| |  _ / |  _|"   \\| |_) |/     /| | | |     | | | |\\| | u <\\___ \\/   
-# u___) |  / ___ \\  | |_| |  | |___  \\| |/__.-,_| |_| | | |_| |  | |_| |  | |___    |  _ <       U| |_| |\\.-,_| |_| | | |/__ u___) |   
-# |____/>>/_/   \\_\\  \\____|  |_____|  |_____|\\_)-\\___/   \\____|   \\____|  |_____|   |_| \\_\\       |____/ u \\_)-\\___/   \\____||____/>>  
-#  )(  (__)\\\\    >>  _)(|_   <<   >>  //  \\\\      \\\\     _)(|_    _)(|_   <<   >>   //   \\\\_       |||_         \\\\    _// \\\\  )(  (__) 
-# (__)    (__)  (__)(__)__) (__) (__)(_")("_)    (__)   (__)__)  (__)__) (__) (__) (__)  (__)     (__)_)       (__)  (__)(__)(__)      
+# -------------------------
+# SageLogger Documentation:
+# -------------------------
 #
-
 # SageFactory.py
 
 `SageFactory.py` is a Python module that provides logging functionalities through the `Logger` module.
 
 ## Functions
 
 ### getLoggerByName(name: str) -> Logger
@@ -266,8 +275,8 @@
 # Log a message and send it to the Discord webhook
 discord_logger.log("This is a log message sent via Discord webhook.")
 ```
 
 ## Note
 
 Make sure to import the necessary modules (colorama, datetime, requests, etc.) before using the logger classes.
-For Logger.py the docs in the file aren't available.
+For Logger.py the docs in the file aren't available.
```

### Comparing `SageLogger-1.4/SageLogger/Logger.py` & `SageLogger-1.5/SageLogger/Logger.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,266 +1,267 @@
-import colorama
-import datetime
-import requests
-from typing import Union
-from enum import Enum
-import os
-from . import SageException, SageFactory
-
-thislogger = None
-
-class DynamicType:
-    @staticmethod
-    def fromChar(logger, char) -> tuple[int, str, bool]:
-        #if len(char) != 1:
-            #MildError.throw(logger, "sagelogs.errors.TooLongChars", "Char in DynamicType is only allowed to have one character! If you need more characters, use \"custom\" method")
-        return (-1, logger.customization.setup_custom_border(char[0]), True)
-    
-    @staticmethod
-    def fromColoredChar(logger, color, char) -> tuple[int, str, bool]:
-        #if len(char) != 1:
-            #MildError.throw(logger, "sagelogs.errors.TooLongChars", "Char in DynamicType is only allowed to have one character! If you need more characters, use \"custom\" method")
-        return (-1, logger.customization.setup_custom_border(color + char[0]), True)
-    
-    @staticmethod
-    def custom(prefix) -> tuple[int, str]:
-        return (-1, prefix)
-
-class xxPartType:
-    name : str = ""
-    Id : int = 0
-    customization : str = ""
-    value : tuple[int, str, bool] = (-2, "", False)
-    enabled = False
-    lockedup = False
-    def __init__(self, name, Id, customization, enabled, lockedup : bool = False) -> None:
-        self.name = name
-        self.Id = Id
-        self.customization = customization
-        self.value = (self.Id, self.customization, self.enabled)
-        self.enabled = enabled
-        self.lockedup = lockedup
-
-class xxType:
-    DEFAULT : xxPartType = xxPartType("DEFAULT", -2, "", True)
-    POSITIVE : xxPartType = xxPartType("POSITIVE", -2, "", True)
-    ONHOLD : xxPartType = xxPartType("ONHOLD", -2, "", True)
-    NEGATIVE : xxPartType = xxPartType("NEGATIVE", -2, "", True)
-    FROZEN : xxPartType = xxPartType("FROZEN", -2, "", True)
-    INFORMATION : xxPartType = xxPartType("INFORMATION", -2, "", True)
-    MILD_EXCEPTION : xxPartType = xxPartType("MILD_EXCEPTION", -2, "", True)
-    DEBUG : xxPartType = xxPartType("DEBUG", -2, "", False)
-    AMONGUS : xxPartType = xxPartType("AMONGUS", -2, "", True)
-    SAGE_LOGGER_DEBUG : xxPartType = xxPartType("SAGE_LOGGER_DEBUG", -2, "", True)
-    def refresh(self, customization):
-        self.DEFAULT = xxPartType("DEFAULT", 0, "", self.DEFAULT.enabled)
-        self.POSITIVE = xxPartType("POSITIVE", 1, customization.setup_custom_border(colorama.Fore.GREEN + "+"), self.POSITIVE.enabled)
-        self.ONHOLD = xxPartType("ONHOLD", 2, customization.setup_custom_border(colorama.Fore.YELLOW + "/"), self.ONHOLD.enabled)
-        self.NEGATIVE = xxPartType("NEGATIVE", 3, customization.setup_custom_border(colorama.Fore.RED + "-"), self.NEGATIVE.enabled)
-        self.FROZEN = xxPartType("FROZEN", 4, customization.setup_custom_border(colorama.Fore.LIGHTBLUE_EX + "#"), self.FROZEN.enabled)
-        self.INFORMATION = xxPartType("INFORMATION", 5, customization.setup_custom_border(colorama.Fore.CYAN + "i"), self.INFORMATION.enabled)
-        self.MILD_EXCEPTION = xxPartType("MILD_EXCEPTION", 6, customization.setup_custom_border(colorama.Fore.LIGHTRED_EX + "X"), self.MILD_EXCEPTION.enabled)
-        self.DEBUG = xxPartType("DEBUG", 7, customization.setup_custom_border(colorama.Fore.LIGHTMAGENTA_EX + "*"), self.DEBUG.enabled)
-        self.AMONGUS = xxPartType("AMONGUS", 8, customization.setup_custom_border(colorama.Fore.RED + "ඞ"), self.AMONGUS.enabled)
-        self.SAGE_LOGGER_DEBUG = xxPartType("SAGE_LOGGER_DEBUG", 9, customization.setup_custom_border(colorama.Fore.LIGHTGREEN_EX + "S" + colorama.Fore.GREEN + "L" + colorama.Fore.LIGHTMAGENTA_EX + "D"), self.SAGE_LOGGER_DEBUG.enabled and not self.SAGE_LOGGER_DEBUG.lockedup)
-    
-    def loggers_in_array(self):
-        return [self.DEFAULT, self.POSITIVE, self.ONHOLD, self.NEGATIVE, self.FROZEN, self.INFORMATION, self.MILD_EXCEPTION, self.DEBUG, self.AMONGUS, self.SAGE_LOGGER_DEBUG]
-    
-    def __iter__(self):
-        return self.loggers_in_array()
-    
-    def is_enabled_type(self, type):
-        return self.loggers_in_array()[type.Id].enabled
-    
-    def toggle_type(self, type):
-        if (type.lockedup):
-            yield SageException.UhOhSomeoneTooCurious()
-        self.loggers_in_array()[type.Id].enabled = not self.loggers_in_array()[type.Id].enabled
-        
-    def enable_type(self, type):
-        if (self.loggers_in_array()[type.Id].lockedup):
-            yield SageException.UhOhSomeoneTooCurious()
-        self.loggers_in_array()[type.Id].enabled = True
-        
-    def disable_type(self, type):
-        self.loggers_in_array()[type.Id].enabled = False
-        
-    def unlock_type_not_recommended_please_leave_it_alone_it_will_spam(self, type):
-        customization = xxCustomization(None)
-        customization.bordcol = colorama.Back.RED + colorama.Fore.WHITE
-        SageFactory.create(name="SageLoggerImportant").log("Unlocked, it isn't recommended, remember. This message cannot be turned off." + colorama.Back.RESET, type=xxPartType("IMPORTANT_HARD_CODED", 1, customization.setup_custom_border(colorama.Fore.LIGHTRED_EX + "!"), True))
-        self.loggers_in_array()[type.Id].lockedup = False
-class MildError:
-    @staticmethod
-    def throw(logger, name, args):
-        logger.log(f"Mild {name} - {args}, you don't need to catch it, but you may fix it ;)", type=SageConsoleLogger.Type.MILD_EXCEPTION)
-        
-class xxCustomization:
-    bordcol = colorama.Fore.LIGHTBLACK_EX
-    borders = "[]"
-    logger = None
-    
-    def __init__(self, logger):
-        self.logger = logger
-
-    def set_border_style(self, border_colorama, borders):
-        self.bordcol = border_colorama
-        if len(borders) != 2:
-            MildError.throw(self.logger, "sagelogs.errors.TooLongChars", "Too much characters in border styling (max 2)")
-        self.borders = borders
-        self.logger.Type.refresh(self) # type: ignore
-
-    def setup_custom_border(self, cos):
-        return self.bordcol + self.borders[0] + colorama.Fore.RESET + cos + self.bordcol + self.borders[1] + " "
-    
-class SageConsoleLogger:
-    customization : xxCustomization = None # type: ignore
-    DynamicType = DynamicType()
-    
-    name = ""
-    logfile = ""
-    savetofile = True
-    Type = xxType()
-    def __init__(self, name : str = "", savetofile : bool = False, logfile : str = "log"):
-        global thislogger
-        if thislogger == None:
-            thislogger = self
-        self.customization = xxCustomization(logger=thislogger)
-        self.Type.refresh(customization=self.customization)
-        self.name = name
-        self.logfile = logfile
-        self.savetofile = savetofile
-        if savetofile:
-            with open(self.name + "." + self.logfile, "a") as wr:
-                wr.write(("-" * 16) + " " + datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S") + " " + ("-" * 16) + "\n")
-                wr.close()
-    
-    def log(self, message : str, type : Union[tuple[int, str, bool], xxPartType] = Type.DEFAULT.value, color = colorama.Fore.RESET, id : int = -2137, date : bool = False, time : bool = False, datecolor : str = colorama.Fore.RESET, timecolor : str = colorama.Fore.RESET, showname : bool = True, ending : str = "\n"):
-        typefinish = None
-        if(isinstance(type, xxPartType)):
-            typefinish = (type.Id, type.customization, type.enabled)
-        else:
-            typefinish = type
-        if not typefinish[2]:
-            return
-        t = ""
-        if date or time:
-            t = self.customization.setup_custom_border(datetime.datetime.now().strftime((datecolor + "%d/%m/%Y" if date else "") + colorama.Fore.RESET + (", " if date and time else "") + (timecolor + "%H:%M:%S" if time else "")))
-        x = t + (self.customization.setup_custom_border(str(id)) if id != -2137 else "") + typefinish[1] + color + message
-        c = (self.customization.setup_custom_border(self.name) + " " if showname else "")
-        x = c + x
-        print(x, end=ending)
-        if self.savetofile:
-            with open(self.name + "." + self.logfile, "a") as wr:
-                wr.write(x.replace("ඞ", "AMONGUS") + ending)
-                wr.close()
-                
-    def ask(self, message : str, type : Union[tuple[int, str, bool], xxPartType] = Type.DEFAULT.value, color = colorama.Fore.RESET, answercolor = colorama.Fore.RESET, id : int = -2137, date : bool = False, time : bool = False, datecolor : str = colorama.Fore.RESET, timecolor : str = colorama.Fore.RESET):
-        typefinish = None
-        if(isinstance(type, xxPartType)):
-            typefinish = (type.Id, type.customization, type.enabled)
-        else:
-            typefinish = type
-        t = ""
-        if date or time:
-            t = self.customization.setup_custom_border(datetime.datetime.now().strftime((datecolor + "%d/%m/%Y" if date else "") + (", " if date and time else "") + (timecolor + "%H:%M:%S" if time else "")))
-        x = t + (self.customization.setup_custom_border(str(id)) if id != -2137 else "") + typefinish[1] + color + message + answercolor
-        ans = input(x)
-        if self.savetofile:
-            with open(self.name + "." + self.logfile, "a") as wr:
-                wr.write(x.replace("ඞ", "AMONGUS") + ">" + ans + "\n")
-                wr.close()
-
-class RemoteWhereLog(Enum):
-    NOWHERE = 0
-    HEADERS = 1
-    BODY = 2
-
-class SageRemoteLogger(SageConsoleLogger):
-    @staticmethod
-    def search_for_placeholder(headers, body) -> RemoteWhereLog:
-        for h in headers.keys():
-            if len(headers[h].split("%LOG%")) != 1:
-                return RemoteWhereLog.HEADERS
-        for h in body.keys():
-            if len(body[h].split("%LOG%")) != 1:
-                return RemoteWhereLog.BODY
-        return RemoteWhereLog.NOWHERE
-    
-    @staticmethod
-    def replace_placeholder(message, whoami, rwl, headers, body):
-        if rwl == RemoteWhereLog.HEADERS and whoami == RemoteWhereLog.HEADERS:
-            for h in headers.keys():
-                if len(headers[h].split("%LOG%")) != 1:
-                    headers[h] = headers[h].replace("%LOG%", message)
-            return headers
-        elif rwl == RemoteWhereLog.HEADERS and whoami == RemoteWhereLog.BODY:
-            return body
-        if rwl == RemoteWhereLog.BODY and whoami == RemoteWhereLog.BODY:
-            for h in body.keys():
-                if len(body[h].split("%LOG%")) != 1:
-                    body[h] = body[h].replace("%LOG%", message)
-            return body
-        elif rwl == RemoteWhereLog.BODY and whoami == RemoteWhereLog.HEADERS:
-            return headers
-    
-    method = ""
-    url = ""
-    headers = {}
-    body = {}
-    remote = RemoteWhereLog.NOWHERE
-    
-    name = ""
-    logfile = ""
-    savetofile = ""
-    def __init__(self, method, url, headers, body, name: str = "", savetofile: bool = False, logfile: str = "log"):
-        SageFactory.errorlogger.log("Initializing remote logger...", type=SageConsoleLogger.Type.SAGE_LOGGER_DEBUG)
-        global thislogger
-        if thislogger is None:
-            thislogger = self
-        self.name = "remote" + ("-" if name != "" else "") + name
-        self.logfile = logfile
-        self.savetofile = savetofile
-        self.url = url
-        self.method = method
-        self.headers = headers
-        self.body = body
-        SageFactory.errorlogger.log("Searching for placeholder %LOG%", type=SageConsoleLogger.Type.SAGE_LOGGER_DEBUG)
-        self.remote = SageRemoteLogger.search_for_placeholder(headers, body)
-        if self.remote == RemoteWhereLog.NOWHERE:
-            raise SageException.NoLogPlaceholder("Remember to somewhere put %LOG%, maybe in the body?")
-
-        if savetofile:
-            with open(self.name + "." + self.logfile, "a") as wr:
-                wr.write(("-" * 16) + " " + datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S") + " " + ("-" * 16) + "\n")
-                wr.close()
-    
-    def log(self, message : str, print_on_console : bool = False, ending : str = "\n"):
-        if print_on_console:
-            print(message, end=ending)
-        
-        a = requests.request(self.method, self.url, json=SageRemoteLogger.replace_placeholder(message, RemoteWhereLog.BODY, self.remote, self.headers, self.body), headers=SageRemoteLogger.replace_placeholder(message, RemoteWhereLog.HEADERS, self.remote, self.headers, self.body))
-        SageFactory.errorlogger.log(a.text + " - " + str(a.status_code), type=SageConsoleLogger.Type.SAGE_LOGGER_DEBUG)
-        if self.savetofile:
-            with open(self.name + "." + self.logfile, "a") as wr:
-                wr.write("(" + str(a.status_code) + ") " + message + ending)
-                wr.write(a.text + ending)
-                wr.close()
-                
-    def ask(self, its_unsupported_sadly):
-        i = its_unsupported_sadly
-        return i
-    
-class SageDiscordWebhookLogger:
-    @staticmethod
-    def create(url, name : str = "", savetofile : bool = False, logfile : str = "log") -> SageRemoteLogger:
-        if len(url.split("discord.com")) >= 2 and len(url.split("webhook")) >= 2:
-            esc = "\\"
-            return SageRemoteLogger("POST", url, {"Content-Type": "application/json"},
-                                    {
-                                        "content": "%LOG%",
-                                        "username": f"Sage Logger - {os.getcwd().split(esc)[-1]}"
-                                    }, name, savetofile, logfile)
-        else:
-            MildError.throw(SageFactory.create_temporary(), "NotDiscordWebhook", "This url isn't a discord webhook, maybe try SageFactory.create_remote method")
+import colorama
+import datetime
+import requests
+from typing import Union
+from enum import Enum
+import os
+from . import SageException, SageFactory
+
+thislogger = None
+
+class DynamicType:
+    @staticmethod
+    def fromChar(logger, char) -> tuple[int, str, bool]:
+        #if len(char) != 1:
+            #MildError.throw(logger, "sagelogs.errors.TooLongChars", "Char in DynamicType is only allowed to have one character! If you need more characters, use \"custom\" method")
+        return (-1, logger.customization.setup_custom_border(char[0]), True)
+    
+    @staticmethod
+    def fromColoredChar(logger, color, char) -> tuple[int, str, bool]:
+        #if len(char) != 1:
+            #MildError.throw(logger, "sagelogs.errors.TooLongChars", "Char in DynamicType is only allowed to have one character! If you need more characters, use \"custom\" method")
+        return (-1, logger.customization.setup_custom_border(color + char[0]), True)
+    
+    @staticmethod
+    def custom(prefix) -> tuple[int, str]:
+        return (-1, prefix)
+
+class xxPartType:
+    name : str = ""
+    Id : int = 0
+    customization : str = ""
+    value : tuple[int, str, bool] = (-2, "", False)
+    enabled = False
+    lockedup = False
+    def __init__(self, name, Id, customization, enabled, lockedup : bool = False) -> None:
+        self.name = name
+        self.Id = Id
+        self.customization = customization
+        self.value = (self.Id, self.customization, self.enabled)
+        self.enabled = enabled
+        self.lockedup = lockedup
+
+class xxType:
+    DEFAULT : xxPartType = xxPartType("DEFAULT", -2, "", True)
+    POSITIVE : xxPartType = xxPartType("POSITIVE", -2, "", True)
+    ONHOLD : xxPartType = xxPartType("ONHOLD", -2, "", True)
+    NEGATIVE : xxPartType = xxPartType("NEGATIVE", -2, "", True)
+    FROZEN : xxPartType = xxPartType("FROZEN", -2, "", True)
+    INFORMATION : xxPartType = xxPartType("INFORMATION", -2, "", True)
+    MILD_EXCEPTION : xxPartType = xxPartType("MILD_EXCEPTION", -2, "", True)
+    DEBUG : xxPartType = xxPartType("DEBUG", -2, "", False)
+    AMONGUS : xxPartType = xxPartType("AMONGUS", -2, "", True)
+    SAGE_LOGGER_DEBUG : xxPartType = xxPartType("SAGE_LOGGER_DEBUG", -2, "", True)
+    def refresh(self, customization):
+        self.DEFAULT = xxPartType("DEFAULT", 0, "", self.DEFAULT.enabled)
+        self.POSITIVE = xxPartType("POSITIVE", 1, customization.setup_custom_border(colorama.Fore.GREEN + "+"), self.POSITIVE.enabled)
+        self.ONHOLD = xxPartType("ONHOLD", 2, customization.setup_custom_border(colorama.Fore.YELLOW + "/"), self.ONHOLD.enabled)
+        self.NEGATIVE = xxPartType("NEGATIVE", 3, customization.setup_custom_border(colorama.Fore.RED + "-"), self.NEGATIVE.enabled)
+        self.FROZEN = xxPartType("FROZEN", 4, customization.setup_custom_border(colorama.Fore.LIGHTBLUE_EX + "#"), self.FROZEN.enabled)
+        self.INFORMATION = xxPartType("INFORMATION", 5, customization.setup_custom_border(colorama.Fore.CYAN + "i"), self.INFORMATION.enabled)
+        self.MILD_EXCEPTION = xxPartType("MILD_EXCEPTION", 6, customization.setup_custom_border(colorama.Fore.LIGHTRED_EX + "X"), self.MILD_EXCEPTION.enabled)
+        self.DEBUG = xxPartType("DEBUG", 7, customization.setup_custom_border(colorama.Fore.LIGHTMAGENTA_EX + "*"), self.DEBUG.enabled)
+        self.AMONGUS = xxPartType("AMONGUS", 8, customization.setup_custom_border(colorama.Fore.RED + "ඞ"), self.AMONGUS.enabled)
+        self.SAGE_LOGGER_DEBUG = xxPartType("SAGE_LOGGER_DEBUG", 9, customization.setup_custom_border(colorama.Fore.LIGHTGREEN_EX + "S" + colorama.Fore.GREEN + "L" + colorama.Fore.LIGHTMAGENTA_EX + "D"), self.SAGE_LOGGER_DEBUG.enabled and not self.SAGE_LOGGER_DEBUG.lockedup)
+    
+    def loggers_in_array(self):
+        return [self.DEFAULT, self.POSITIVE, self.ONHOLD, self.NEGATIVE, self.FROZEN, self.INFORMATION, self.MILD_EXCEPTION, self.DEBUG, self.AMONGUS, self.SAGE_LOGGER_DEBUG]
+    
+    def __iter__(self):
+        return self.loggers_in_array()
+    
+    def is_enabled_type(self, type):
+        return self.loggers_in_array()[type.Id].enabled
+    
+    def toggle_type(self, type):
+        if (type.lockedup):
+            yield SageException.UhOhSomeoneTooCurious()
+        self.loggers_in_array()[type.Id].enabled = not self.loggers_in_array()[type.Id].enabled
+        
+    def enable_type(self, type):
+        if (self.loggers_in_array()[type.Id].lockedup):
+            yield SageException.UhOhSomeoneTooCurious()
+        self.loggers_in_array()[type.Id].enabled = True
+        
+    def disable_type(self, type):
+        self.loggers_in_array()[type.Id].enabled = False
+        
+    def unlock_type_not_recommended_please_leave_it_alone_it_will_spam(self, type):
+        customization = xxCustomization(None)
+        customization.bordcol = colorama.Back.RED + colorama.Fore.WHITE
+        SageFactory.create(name="SageLoggerImportant").log("Unlocked, it isn't recommended, remember. This message cannot be turned off." + colorama.Back.RESET, type=xxPartType("IMPORTANT_HARD_CODED", 1, customization.setup_custom_border(colorama.Fore.LIGHTRED_EX + "!"), True))
+        self.loggers_in_array()[type.Id].lockedup = False
+class MildError:
+    @staticmethod
+    def throw(logger, name, args):
+        logger.log(f"Mild {name} - {args}, you don't need to catch it, but you may fix it ;)", type=SageConsoleLogger.Type.MILD_EXCEPTION)
+        
+class xxCustomization:
+    bordcol = colorama.Fore.LIGHTBLACK_EX
+    borders = "[]"
+    logger = None
+    
+    def __init__(self, logger):
+        self.logger = logger
+
+    def set_border_style(self, border_colorama, borders):
+        self.bordcol = border_colorama
+        if len(borders) != 2:
+            MildError.throw(self.logger, "sagelogs.errors.TooLongChars", "Too much characters in border styling (max 2)")
+        self.borders = borders
+        self.logger.Type.refresh(self) # type: ignore
+
+    def setup_custom_border(self, cos):
+        return self.bordcol + self.borders[0] + colorama.Fore.RESET + cos + self.bordcol + self.borders[1] + " "
+    
+class SageConsoleLogger:
+    customization : xxCustomization = None # type: ignore
+    DynamicType = DynamicType()
+    
+    name = ""
+    logfile = ""
+    savetofile = True
+    Type = xxType()
+    def __init__(self, name : str = "", savetofile : bool = False, logfile : str = "log"):
+        global thislogger
+        if thislogger == None:
+            thislogger = self
+        self.customization = xxCustomization(logger=thislogger)
+        self.Type.refresh(customization=self.customization)
+        self.name = name
+        self.logfile = logfile
+        self.savetofile = savetofile
+        if savetofile:
+            with open(self.name + "." + self.logfile, "a") as wr:
+                wr.write(("-" * 16) + " " + datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S") + " " + ("-" * 16) + "\n")
+                wr.close()
+    
+    def log(self, message : str, type : Union[tuple[int, str, bool], xxPartType] = Type.DEFAULT.value, color = colorama.Fore.RESET, id : int = -2137, date : bool = False, time : bool = False, datecolor : str = colorama.Fore.RESET, timecolor : str = colorama.Fore.RESET, showname : bool = True, ending : str = "\n"):
+        typefinish = None
+        if(isinstance(type, xxPartType)):
+            typefinish = (type.Id, type.customization, type.enabled)
+        else:
+            typefinish = type
+        if not typefinish[2]:
+            return
+        t = ""
+        if date or time:
+            t = self.customization.setup_custom_border(datetime.datetime.now().strftime((datecolor + "%d/%m/%Y" if date else "") + colorama.Fore.RESET + (", " if date and time else "") + (timecolor + "%H:%M:%S" if time else "")))
+        x = t + (self.customization.setup_custom_border(str(id)) if id != -2137 else "") + typefinish[1] + color + message
+        c = (self.customization.setup_custom_border(self.name) + " " if showname else "")
+        x = c + x
+        print(x, end=ending)
+        if self.savetofile:
+            with open(self.name + "." + self.logfile, "a") as wr:
+                wr.write(x.replace("ඞ", "AMONGUS") + ending)
+                wr.close()
+                
+    def ask(self, message : str, type : Union[tuple[int, str, bool], xxPartType] = Type.DEFAULT.value, color = colorama.Fore.RESET, answercolor = colorama.Fore.RESET, id : int = -2137, date : bool = False, time : bool = False, datecolor : str = colorama.Fore.RESET, timecolor : str = colorama.Fore.RESET) -> str:
+        typefinish = None
+        if(isinstance(type, xxPartType)):
+            typefinish = (type.Id, type.customization, type.enabled)
+        else:
+            typefinish = type
+        t = ""
+        if date or time:
+            t = self.customization.setup_custom_border(datetime.datetime.now().strftime((datecolor + "%d/%m/%Y" if date else "") + (", " if date and time else "") + (timecolor + "%H:%M:%S" if time else "")))
+        x = t + (self.customization.setup_custom_border(str(id)) if id != -2137 else "") + typefinish[1] + color + message + answercolor
+        ans = input(x)
+        if self.savetofile:
+            with open(self.name + "." + self.logfile, "a") as wr:
+                wr.write(x.replace("ඞ", "AMONGUS") + ">" + ans + "\n")
+                wr.close()
+        return ans
+
+class RemoteWhereLog(Enum):
+    NOWHERE = 0
+    HEADERS = 1
+    BODY = 2
+
+class SageRemoteLogger(SageConsoleLogger):
+    @staticmethod
+    def search_for_placeholder(headers, body) -> RemoteWhereLog:
+        for h in headers.keys():
+            if len(headers[h].split("%LOG%")) != 1:
+                return RemoteWhereLog.HEADERS
+        for h in body.keys():
+            if len(body[h].split("%LOG%")) != 1:
+                return RemoteWhereLog.BODY
+        return RemoteWhereLog.NOWHERE
+    
+    @staticmethod
+    def replace_placeholder(message, whoami, rwl, headers, body):
+        if rwl == RemoteWhereLog.HEADERS and whoami == RemoteWhereLog.HEADERS:
+            for h in headers.keys():
+                if len(headers[h].split("%LOG%")) != 1:
+                    headers[h] = headers[h].replace("%LOG%", message)
+            return headers
+        elif rwl == RemoteWhereLog.HEADERS and whoami == RemoteWhereLog.BODY:
+            return body
+        if rwl == RemoteWhereLog.BODY and whoami == RemoteWhereLog.BODY:
+            for h in body.keys():
+                if len(body[h].split("%LOG%")) != 1:
+                    body[h] = body[h].replace("%LOG%", message)
+            return body
+        elif rwl == RemoteWhereLog.BODY and whoami == RemoteWhereLog.HEADERS:
+            return headers
+    
+    method = ""
+    url = ""
+    headers = {}
+    body = {}
+    remote = RemoteWhereLog.NOWHERE
+    
+    name = ""
+    logfile = ""
+    savetofile = ""
+    def __init__(self, method, url, headers, body, name: str = "", savetofile: bool = False, logfile: str = "log"):
+        SageFactory.errorlogger.log("Initializing remote logger...", type=SageConsoleLogger.Type.SAGE_LOGGER_DEBUG)
+        global thislogger
+        if thislogger is None:
+            thislogger = self
+        self.name = "remote" + ("-" if name != "" else "") + name
+        self.logfile = logfile
+        self.savetofile = savetofile
+        self.url = url
+        self.method = method
+        self.headers = headers
+        self.body = body
+        SageFactory.errorlogger.log("Searching for placeholder %LOG%", type=SageConsoleLogger.Type.SAGE_LOGGER_DEBUG)
+        self.remote = SageRemoteLogger.search_for_placeholder(headers, body)
+        if self.remote == RemoteWhereLog.NOWHERE:
+            raise SageException.NoLogPlaceholder("Remember to somewhere put %LOG%, maybe in the body?")
+
+        if savetofile:
+            with open(self.name + "." + self.logfile, "a") as wr:
+                wr.write(("-" * 16) + " " + datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S") + " " + ("-" * 16) + "\n")
+                wr.close()
+    
+    def log(self, message : str, print_on_console : bool = False, ending : str = "\n"):
+        if print_on_console:
+            print(message, end=ending)
+        
+        a = requests.request(self.method, self.url, json=SageRemoteLogger.replace_placeholder(message, RemoteWhereLog.BODY, self.remote, self.headers, self.body), headers=SageRemoteLogger.replace_placeholder(message, RemoteWhereLog.HEADERS, self.remote, self.headers, self.body))
+        SageFactory.errorlogger.log(a.text + " - " + str(a.status_code), type=SageConsoleLogger.Type.SAGE_LOGGER_DEBUG)
+        if self.savetofile:
+            with open(self.name + "." + self.logfile, "a") as wr:
+                wr.write("(" + str(a.status_code) + ") " + message + ending)
+                wr.write(a.text + ending)
+                wr.close()
+                
+    def ask(self, its_unsupported_sadly):
+        i = its_unsupported_sadly
+        return i
+    
+class SageDiscordWebhookLogger:
+    @staticmethod
+    def create(url, name : str = "", savetofile : bool = False, logfile : str = "log") -> SageRemoteLogger:
+        if len(url.split("discord.com")) >= 2 and len(url.split("webhook")) >= 2:
+            esc = "\\"
+            return SageRemoteLogger("POST", url, {"Content-Type": "application/json"},
+                                    {
+                                        "content": "%LOG%",
+                                        "username": f"Sage Logger - {os.getcwd().split(esc)[-1]}"
+                                    }, name, savetofile, logfile)
+        else:
+            MildError.throw(SageFactory.create_temporary(), "NotDiscordWebhook", "This url isn't a discord webhook, maybe try SageFactory.create_remote method")
             return SageRemoteLogger("", "", {"log":"%LOG%"}, {})
```

### Comparing `SageLogger-1.4/SageLogger/SageFactory.py` & `SageLogger-1.5/SageLogger/SageFactory.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-from . import Logger
-from typing import Union
-
-loggers = []
-
-def getLoggerByName(name: str) -> Union[Logger.SageConsoleLogger, Logger.SageRemoteLogger]:
-    """
-    Returns a logger object by name.
-    :param name: The name of the logger to retrieve.
-    :type name: str
-    :return: The logger object if found, otherwise None.
-    :rtype: Logger
-    """
-    for l in loggers:
-        if l.name == name:
-            return l
-        
-    return Logger.SageConsoleLogger(name="NotFoundLogger", savetofile=False, logfile="log")
-
-def create(name: str = "", savetofile: bool = False, logfile: str = "log"):
-    """
-    Creates a console logger and adds it to the list of loggers.
-    :param name: The name of the logger. Default is an empty string.
-    :type name: str
-    :param savetofile: Whether to save logs to a file. Default is False.
-    :type savetofile: bool
-    :param logfile: The filename to save logs. Default is "log".
-    :type logfile: str
-    :return: The created console logger.
-    :rtype: Logger
-    """
-    l = Logger.SageConsoleLogger(name, savetofile, logfile)
-    loggers.append(l)
-    return l
-
-def create_remote(method, url, headers, body, name: str = "", savetofile: bool = False, logfile: str = "log"):
-    """
-    Creates a remote logger and adds it to the list of loggers.
-    :param method: The HTTP method to use for the remote logger.
-    :param url: The URL to send logs to.
-    :param headers: The headers to be included in the request.
-    :param body: The log payload.
-    :param name: The name of the logger. Default is an empty string.
-    :type name: str
-    :param savetofile: Whether to save logs to a file. Default is False.
-    :type savetofile: bool
-    :param logfile: The filename to save logs. Default is "log".
-    :type logfile: str
-    :return: The created remote logger.
-    :rtype: Logger
-    """
-    l = Logger.SageRemoteLogger(method, url, headers, body, name, savetofile, logfile)
-    loggers.append(l)
-    return l
-
-def create_discord_webhook_remote(url, name: str = "", savetofile: bool = False, logfile: str = "log"):
-    """
-    Creates a Discord webhook logger and adds it to the list of loggers.
-    :param url: The Discord webhook URL to send logs to.
-    :param name: The name of the logger. Default is an empty string.
-    :type name: str
-    :param savetofile: Whether to save logs to a file. Default is False.
-    :type savetofile: bool
-    :param logfile: The filename to save logs. Default is "log".
-    :type logfile: str
-    :return: The created Discord webhook logger.
-    :rtype: Logger
-    """
-    l = Logger.SageDiscordWebhookLogger.create(url, name, savetofile, logfile)
-    loggers.append(l)
-    return l
-
-def create_temporary():
-    """
-    Creates a temporary logger and adds it to the list of loggers.
-    :return: The created temporary logger.
-    :rtype: Logger
-    """
-    l = create(name="temporary", savetofile=False)
-    loggers.append(l)
-    return l
-
-# A pre-created console logger named "Errors" that doesn't save logs to a file.
+from . import Logger
+from typing import Union
+
+loggers = []
+
+def getLoggerByName(name: str) -> Union[Logger.SageConsoleLogger, Logger.SageRemoteLogger]:
+    """
+    Returns a logger object by name.
+    :param name: The name of the logger to retrieve.
+    :type name: str
+    :return: The logger object if found, otherwise None.
+    :rtype: Logger
+    """
+    for l in loggers:
+        if l.name == name:
+            return l
+        
+    return Logger.SageConsoleLogger(name="NotFoundLogger", savetofile=False, logfile="log")
+
+def create(name: str = "", savetofile: bool = False, logfile: str = "log"):
+    """
+    Creates a console logger and adds it to the list of loggers.
+    :param name: The name of the logger. Default is an empty string.
+    :type name: str
+    :param savetofile: Whether to save logs to a file. Default is False.
+    :type savetofile: bool
+    :param logfile: The filename to save logs. Default is "log".
+    :type logfile: str
+    :return: The created console logger.
+    :rtype: Logger
+    """
+    l = Logger.SageConsoleLogger(name, savetofile, logfile)
+    loggers.append(l)
+    return l
+
+def create_remote(method, url, headers, body, name: str = "", savetofile: bool = False, logfile: str = "log"):
+    """
+    Creates a remote logger and adds it to the list of loggers.
+    :param method: The HTTP method to use for the remote logger.
+    :param url: The URL to send logs to.
+    :param headers: The headers to be included in the request.
+    :param body: The log payload.
+    :param name: The name of the logger. Default is an empty string.
+    :type name: str
+    :param savetofile: Whether to save logs to a file. Default is False.
+    :type savetofile: bool
+    :param logfile: The filename to save logs. Default is "log".
+    :type logfile: str
+    :return: The created remote logger.
+    :rtype: Logger
+    """
+    l = Logger.SageRemoteLogger(method, url, headers, body, name, savetofile, logfile)
+    loggers.append(l)
+    return l
+
+def create_discord_webhook_remote(url, name: str = "", savetofile: bool = False, logfile: str = "log"):
+    """
+    Creates a Discord webhook logger and adds it to the list of loggers.
+    :param url: The Discord webhook URL to send logs to.
+    :param name: The name of the logger. Default is an empty string.
+    :type name: str
+    :param savetofile: Whether to save logs to a file. Default is False.
+    :type savetofile: bool
+    :param logfile: The filename to save logs. Default is "log".
+    :type logfile: str
+    :return: The created Discord webhook logger.
+    :rtype: Logger
+    """
+    l = Logger.SageDiscordWebhookLogger.create(url, name, savetofile, logfile)
+    loggers.append(l)
+    return l
+
+def create_temporary():
+    """
+    Creates a temporary logger and adds it to the list of loggers.
+    :return: The created temporary logger.
+    :rtype: Logger
+    """
+    l = create(name="temporary", savetofile=False)
+    loggers.append(l)
+    return l
+
+# A pre-created console logger named "Errors" that doesn't save logs to a file.
 errorlogger = create("Errors", False, "log")
```

### Comparing `SageLogger-1.4/SageLogger.egg-info/PKG-INFO` & `SageLogger-1.5/SageLogger.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 Metadata-Version: 2.1
 Name: SageLogger
-Version: 1.4
+Version: 1.5
 Summary: Yet another python logger, or is it like any other?
 Home-page: https://github.com/PanSageYT/SageLogger
 Author: PanSageYT
-Author-email: PanSageYT <pansage@hugedick.fyi>
-Project-URL: Homepage, https://github.com/PanSageYT/SageLogger
-Project-URL: Bug Tracker, https://github.com/PanSageYT/SageLogger/issues
+Author-email: pansage@hugedick.fyi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # SageLogger: Python Logger Package
 
 SageLogger is a versatile Python logger package that allows you to create loggers with both remote and local capabilities. The core module, "SageFactory.py," facilitates the creation of loggers with options for SageRemoteLogger (remote) and SageLogger (local). When using SageLogger, you have the flexibility to choose from 7 predefined log types for local logging: DEFAULT, POSITIVE, ONHOLD, NEGATIVE, FROZEN, INFORMATION, and MILD_EXCEPTION. Additionally, you can easily create custom log types to suit your specific needs using the `SageLogger.DynamicType` class.
 
 ## Features
 
 ### Local Logging Options
-SageLogger offers 7 built-in log types for local logging:
+SageLogger offers 9 built-in log types for local logging:
 
 1. DEFAULT: The default log type.
 2. POSITIVE: For positive events and actions.
 3. ONHOLD: To indicate events that are on hold or waiting for further action.
 4. NEGATIVE: For negative events or errors.
 5. FROZEN: To represent frozen states or events.
 6. INFORMATION: For general information logging.
 7. MILD_EXCEPTION: To log minor exceptions or errors.
 8. DEBUG: To troubleshoot some things. (disabled by default)
+9. .................................... (shh secret)
 
 ### Custom Local Log Types
 Apart from the predefined log types, you can create custom log types using the `SageLogger.DynamicType.fromChar` method or the `SageLogger.DynamicType.fromColoredChar` method for colored logs.
 
 ### Remote Logging
 SageLogger enables remote logging capabilities through the SageRemoteLogger class. You can load custom APIs for remote logging, and it also provides built-in support for Discord webhook integration.
 
@@ -90,25 +89,20 @@
 
 ### Changelogs:
 v1.0 - Initial version
 v1.1 - Skipped as of a fail in version naming :(
 v1.2 - Skipped as of a fail in version naming :(
 v1.3 - Logger arrays in SageFactory and getLoggerByName(name), 3 more loggers (1 secret shh). More functions of enabling, changed class name from SageLogger.Logger.SageLogger to SageLogger.Logger.SageConsoleLogger
 v1.4 - Forced release because I forgot to change sample code from README.md
+v1.5 - Fixed logger.ask() method so it returns String object (which is the users answer)
 
-# 
-#  ____       _       ____  U _____ u  _       U  ___ u   ____     ____  U _____ u   ____          ____      U  ___ u   ____  ____     
-# / __"| uU  /"\\  uU /"___|u\\| ___"|/ |"|       \\/"_ \\/U /"___|uU /"___|u\\| ___"|/U |  _"\\ u      |  _"\\      \\/"_ \\/U /"___|/ __"| u  
-#<\\___ \\/  \\/ _ \\/ \\| |  _ / |  _|" U | | u     | | | |\\| |  _ /\\| |  _ / |  _|"   \\| |_) |/     /| | | |     | | | |\\| | u <\\___ \\/   
-# u___) |  / ___ \\  | |_| |  | |___  \\| |/__.-,_| |_| | | |_| |  | |_| |  | |___    |  _ <       U| |_| |\\.-,_| |_| | | |/__ u___) |   
-# |____/>>/_/   \\_\\  \\____|  |_____|  |_____|\\_)-\\___/   \\____|   \\____|  |_____|   |_| \\_\\       |____/ u \\_)-\\___/   \\____||____/>>  
-#  )(  (__)\\\\    >>  _)(|_   <<   >>  //  \\\\      \\\\     _)(|_    _)(|_   <<   >>   //   \\\\_       |||_         \\\\    _// \\\\  )(  (__) 
-# (__)    (__)  (__)(__)__) (__) (__)(_")("_)    (__)   (__)__)  (__)__) (__) (__) (__)  (__)     (__)_)       (__)  (__)(__)(__)      
+# -------------------------
+# SageLogger Documentation:
+# -------------------------
 #
-
 # SageFactory.py
 
 `SageFactory.py` is a Python module that provides logging functionalities through the `Logger` module.
 
 ## Functions
 
 ### getLoggerByName(name: str) -> Logger
```

