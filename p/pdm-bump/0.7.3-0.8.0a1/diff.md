# Comparing `tmp/pdm_bump-0.7.3.tar.gz` & `tmp/pdm_bump-0.8.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_bump-0.7.3.tar", last modified: Tue Jul 18 19:38:01 2023, max compression
+gzip compressed data, was "pdm_bump-0.8.0a1.tar", last modified: Wed Aug  2 13:23:20 2023, max compression
```

## Comparing `pdm_bump-0.7.3.tar` & `pdm_bump-0.8.0a1.tar`

### file list

```diff
@@ -1,28 +1,31 @@
--rw-r--r--   0        0        0     1092 2023-07-18 19:37:07.256097 pdm_bump-0.7.3/LICENSE
--rw-r--r--   0        0        0     2397 2023-07-18 19:37:07.256097 pdm_bump-0.7.3/README.md
--rw-r--r--   0        0        0     6003 2023-07-18 19:38:01.051993 pdm_bump-0.7.3/pyproject.toml
--rw-r--r--   0        0        0      869 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/__init__.py
--rw-r--r--   0        0        0      531 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/actions/__init__.py
--rw-r--r--   0        0        0     8508 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/actions/base.py
--rw-r--r--   0        0        0     1954 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/actions/explicit.py
--rw-r--r--   0        0        0     9966 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/actions/increment.py
--rw-r--r--   0        0        0     8897 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/actions/preview.py
--rw-r--r--   0        0        0     1558 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/actions/vcs.py
--rw-r--r--   0        0        0     1378 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/cli.py
--rw-r--r--   0        0        0      259 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/core/__init__.py
--rw-r--r--   0        0        0     9461 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/core/config.py
--rw-r--r--   0        0        0     7404 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/core/logging.py
--rw-r--r--   0        0        0     7593 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/core/version.py
--rw-r--r--   0        0        0     6596 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/dynamic.py
--rw-r--r--   0        0        0     6668 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/plugin.py
--rw-r--r--   0        0        0        0 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/py.typed
--rw-r--r--   0        0        0     2402 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/source.py
--rw-r--r--   0        0        0      699 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/vcs/__init__.py
--rw-r--r--   0        0        0     9907 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/vcs/core.py
--rw-r--r--   0        0        0     1103 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/vcs/git.py
--rw-r--r--   0        0        0     7356 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/vcs/gitcli.py
--rw-r--r--   0        0        0     4906 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/vcs/mixins.py
--rw-r--r--   0        0        0    25464 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/tests/action_test.py
--rw-r--r--   0        0        0     3743 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/tests/plugin_test.py
--rw-r--r--   0        0        0    24207 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/tests/version_test.py
--rw-r--r--   0        0        0     3062 1970-01-01 00:00:00.000000 pdm_bump-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-08-02 13:22:21.690005 pdm_bump-0.8.0a1/LICENSE
+-rw-r--r--   0        0        0     5318 2023-08-02 13:22:21.690005 pdm_bump-0.8.0a1/README.md
+-rw-r--r--   0        0        0     6005 2023-08-02 13:23:20.566916 pdm_bump-0.8.0a1/pyproject.toml
+-rw-r--r--   0        0        0      869 2023-08-02 13:22:21.690005 pdm_bump-0.8.0a1/src/pdm_bump/__init__.py
+-rw-r--r--   0        0        0      544 2023-08-02 13:22:21.690005 pdm_bump-0.8.0a1/src/pdm_bump/actions/__init__.py
+-rw-r--r--   0        0        0     8616 2023-08-02 13:22:21.690005 pdm_bump-0.8.0a1/src/pdm_bump/actions/base.py
+-rw-r--r--   0        0        0     1954 2023-08-02 13:22:21.690005 pdm_bump-0.8.0a1/src/pdm_bump/actions/explicit.py
+-rw-r--r--   0        0        0    10702 2023-08-02 13:22:21.690005 pdm_bump-0.8.0a1/src/pdm_bump/actions/increment.py
+-rw-r--r--   0        0        0     5088 2023-08-02 13:22:21.690005 pdm_bump-0.8.0a1/src/pdm_bump/actions/poetry_like.py
+-rw-r--r--   0        0        0     8897 2023-08-02 13:22:21.690005 pdm_bump-0.8.0a1/src/pdm_bump/actions/preview.py
+-rw-r--r--   0        0        0     4761 2023-08-02 13:22:21.690005 pdm_bump-0.8.0a1/src/pdm_bump/actions/vcs.py
+-rw-r--r--   0        0        0     8959 2023-08-02 13:22:21.690005 pdm_bump-0.8.0a1/src/pdm_bump/actions/version_providers.py
+-rw-r--r--   0        0        0     1378 2023-08-02 13:22:21.690005 pdm_bump-0.8.0a1/src/pdm_bump/cli.py
+-rw-r--r--   0        0        0      259 2023-08-02 13:22:21.690005 pdm_bump-0.8.0a1/src/pdm_bump/core/__init__.py
+-rw-r--r--   0        0        0     9461 2023-08-02 13:22:21.690005 pdm_bump-0.8.0a1/src/pdm_bump/core/config.py
+-rw-r--r--   0        0        0     7667 2023-08-02 13:22:21.690005 pdm_bump-0.8.0a1/src/pdm_bump/core/logging.py
+-rw-r--r--   0        0        0     7842 2023-08-02 13:22:21.690005 pdm_bump-0.8.0a1/src/pdm_bump/core/version.py
+-rw-r--r--   0        0        0     6596 2023-08-02 13:22:21.690005 pdm_bump-0.8.0a1/src/pdm_bump/dynamic.py
+-rw-r--r--   0        0        0     6668 2023-08-02 13:22:21.694005 pdm_bump-0.8.0a1/src/pdm_bump/plugin.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:22:21.694005 pdm_bump-0.8.0a1/src/pdm_bump/py.typed
+-rw-r--r--   0        0        0     2402 2023-08-02 13:22:21.694005 pdm_bump-0.8.0a1/src/pdm_bump/source.py
+-rw-r--r--   0        0        0      920 2023-08-02 13:22:21.694005 pdm_bump-0.8.0a1/src/pdm_bump/vcs/__init__.py
+-rw-r--r--   0        0        0    10170 2023-08-02 13:22:21.694005 pdm_bump-0.8.0a1/src/pdm_bump/vcs/core.py
+-rw-r--r--   0        0        0     1103 2023-08-02 13:22:21.694005 pdm_bump-0.8.0a1/src/pdm_bump/vcs/git.py
+-rw-r--r--   0        0        0     8645 2023-08-02 13:22:21.694005 pdm_bump-0.8.0a1/src/pdm_bump/vcs/gitcli.py
+-rw-r--r--   0        0        0     6318 2023-08-02 13:22:21.694005 pdm_bump-0.8.0a1/src/pdm_bump/vcs/history.py
+-rw-r--r--   0        0        0     4906 2023-08-02 13:22:21.694005 pdm_bump-0.8.0a1/src/pdm_bump/vcs/mixins.py
+-rw-r--r--   0        0        0    33814 2023-08-02 13:22:21.694005 pdm_bump-0.8.0a1/tests/action_test.py
+-rw-r--r--   0        0        0     3867 2023-08-02 13:22:21.694005 pdm_bump-0.8.0a1/tests/plugin_test.py
+-rw-r--r--   0        0        0    24207 2023-08-02 13:22:21.694005 pdm_bump-0.8.0a1/tests/version_test.py
+-rw-r--r--   0        0        0     5985 1970-01-01 00:00:00.000000 pdm_bump-0.8.0a1/PKG-INFO
```

### Comparing `pdm_bump-0.7.3/LICENSE` & `pdm_bump-0.8.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.3/pyproject.toml` & `pdm_bump-0.8.0a1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pdm-bump"
-version = "0.7.3"
+version = "0.8.0a1"
 readme = "README.md"
 description = "A plugin for PDM providing the ability to modify the version according to PEP440"
 authors = [
     { name = "Carsten Igel", email = "cig@bite-that-bit.de" },
 ]
 dependencies = [
     "pdm>=2.00",
```

### Comparing `pdm_bump-0.7.3/src/pdm_bump/__init__.py` & `pdm_bump-0.8.0a1/src/pdm_bump/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.3/src/pdm_bump/actions/__init__.py` & `pdm_bump-0.8.0a1/src/pdm_bump/actions/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # This file is published using the MIT license.
 # Refer to LICENSE for more information
 #
 """"""
 
 # Justification: load module for decoupling
-from . import explicit, increment, preview, vcs  # noqa: F401
+from . import explicit, increment, poetry_like, preview, vcs  # noqa: F401
 from .base import ActionBase, VersionConsumer, VersionModifier, actions
 
 __all__ = [
     "actions",
     "ActionBase",
     "VersionConsumer",
     "VersionModifier",
```

### Comparing `pdm_bump-0.7.3/src/pdm_bump/actions/base.py` & `pdm_bump-0.8.0a1/src/pdm_bump/actions/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,14 +247,17 @@
     @classmethod
     def get_allowed_arguments(cls) -> set[str]:
         """"""
         return set(["persister"]).union(
             VersionConsumer.get_allowed_arguments()
         )
 
+    def __str__(self) -> str:
+        return self.__class__.__name__.replace(VersionModifier.__name__, "")
+
 
 class ActionRegistry:
     """"""
 
     def __init__(self) -> None:
         self.__items: dict[str, type[ActionBase]] = {}
```

### Comparing `pdm_bump-0.7.3/src/pdm_bump/actions/explicit.py` & `pdm_bump-0.8.0a1/src/pdm_bump/actions/explicit.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.3/src/pdm_bump/actions/increment.py` & `pdm_bump-0.8.0a1/src/pdm_bump/actions/increment.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,23 +323,41 @@
     name: str = "dev"
     description: str = "Increment the local development part"
 
     @traced_function
     def create_new_version(self) -> Version:
         """"""
         dev_version: NonNegativeInteger = 1
+        micro_version = self.current_version.micro
         if self.current_version.dev is not None:
             _, dev_version = self.current_version.dev
             logger.debug("Incrementing development version part by one")
             dev_version = dev_version + 1
+        else:
+            logger.debug(
+                "Incrementing micro version as it is no dev version yet"
+            )
+            micro_version = micro_version + 1
 
         constructional_args: dict[str, Any] = dataclass_to_dict(
             self.current_version
         )
         constructional_args["dev"] = ("dev", dev_version)
+        constructional_args["release_tuple"] = (
+            self.current_version.major,
+            self.current_version.minor,
+            micro_version,
+        )
+
+        if (
+            self.current_version.is_post_release
+            and not self.current_version.is_development_version
+        ):
+            logger.debug("Resetting post version to zero")
+            constructional_args["post"] = None
 
         next_version: Version = Version(**constructional_args)
         self._report_new_version(next_version)
 
         return next_version
 
 
@@ -360,12 +378,14 @@
             logger.debug("Incrementing post version part by one")
             post_version = post_version + 1
 
         constructional_args: dict[str, Any] = dataclass_to_dict(
             self.current_version
         )
         constructional_args["post"] = ("post", post_version)
+        if self.current_version.is_development_version:
+            constructional_args["dev"] = None
 
         next_version: Version = Version(**constructional_args)
         self._report_new_version(next_version)
 
         return next_version
```

### Comparing `pdm_bump-0.7.3/src/pdm_bump/actions/preview.py` & `pdm_bump-0.8.0a1/src/pdm_bump/actions/preview.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.3/src/pdm_bump/cli.py` & `pdm_bump-0.8.0a1/src/pdm_bump/cli.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.3/src/pdm_bump/core/config.py` & `pdm_bump-0.8.0a1/src/pdm_bump/core/config.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.3/src/pdm_bump/core/logging.py` & `pdm_bump-0.8.0a1/src/pdm_bump/core/logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # This file is published using the MIT license.
 # Refer to LICENSE for more information
 #
 """"""
 
 
 from collections.abc import Mapping
+from contextlib import contextmanager
 from logging import (
     CRITICAL,
     DEBUG,
     ERROR,
     INFO,
     NOTSET,
     WARN,
@@ -337,7 +338,19 @@
             return fun(*args, **kwargs)
         finally:
             logger.trace(
                 "%s: Exiting function", fun.__qualname__ or fun.__name__
             )
 
     return tracing_function
+
+
+@contextmanager
+def silenced(log: Logger):
+    """"""
+    log_level: int = log.level
+    try:
+        if log_level > DEBUG:
+            log.setLevel(CRITICAL + 20)
+        yield
+    finally:
+        log.setLevel(log_level)
```

### Comparing `pdm_bump-0.7.3/src/pdm_bump/core/version.py` & `pdm_bump-0.8.0a1/src/pdm_bump/core/version.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,14 +129,24 @@
 
     @property
     def is_release_candidate(self) -> bool:
         """"""
         rc_part: Final[tuple[str, ...]] = ("c", "rc")
         return self.preview is not None and self.__compare_preview(rc_part)
 
+    @property
+    def is_final(self) -> bool:
+        """"""
+        return (
+            not self.preview
+            and not self.is_local_version
+            and not self.is_post_release
+            and not self.is_development_version
+        )
+
     def __compare_preview(self, valid_parts: tuple[str, ...]) -> bool:
         if self.preview is not None:
             pre: tuple[str, int] = cast(tuple[str, int], self.preview)
             return pre[0] in valid_parts
         return False
 
     def __eq__(self, other: Any) -> bool:
```

### Comparing `pdm_bump-0.7.3/src/pdm_bump/dynamic.py` & `pdm_bump-0.8.0a1/src/pdm_bump/dynamic.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.3/src/pdm_bump/plugin.py` & `pdm_bump-0.8.0a1/src/pdm_bump/plugin.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.3/src/pdm_bump/source.py` & `pdm_bump-0.8.0a1/src/pdm_bump/source.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.3/src/pdm_bump/vcs/core.py` & `pdm_bump-0.8.0a1/src/pdm_bump/vcs/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 from abc import ABC, abstractmethod
 from collections.abc import Iterator
 from pathlib import Path
 from typing import AnyStr, Callable, Final, NamedTuple, Optional, Union, cast
 
 from ..core.version import Pep440VersionFormatter, Version
+from .history import History
 
 _Pathlike = Union[Path, AnyStr]
 
 
 class _PathLikeConverter(ABC):
     """"""
 
@@ -143,14 +144,19 @@
         raise NotImplementedError()
 
     @abstractmethod
     def get_changes_not_checked_in(self) -> int:
         """"""
         raise NotImplementedError()
 
+    @abstractmethod
+    def get_history(self, since_last_tag: bool = True) -> History:
+        """"""
+        raise NotImplementedError()
+
 
 class VcsProviderAggregator:
     """"""
 
     def __init__(self, vcs_provider: VcsProvider, **kwargs) -> None:
         self.__vcs_provider: VcsProvider = vcs_provider
 
@@ -475,12 +481,15 @@
         return 0
 
     def get_changes_not_checked_in(self) -> int:
         """"""
         # Cannot be provided
         return 0
 
+    def get_history(self, since_last_tag: bool = True) -> History:
+        return History([])
+
 
 class VcsProviderError(Exception):
     """"""
 
     pass
```

### Comparing `pdm_bump-0.7.3/src/pdm_bump/vcs/git.py` & `pdm_bump-0.8.0a1/src/pdm_bump/vcs/git.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.3/src/pdm_bump/vcs/gitcli.py` & `pdm_bump-0.8.0a1/src/pdm_bump/vcs/gitcli.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 
 from functools import cached_property
 from pathlib import Path
 from subprocess import CalledProcessError
 from typing import Optional, cast
 
 from ..core.logging import logger
-from ..core.version import Version
+from ..core.version import Pep440VersionFormatter, Version
 from .core import VcsProvider, VcsProviderError, vcs_provider
 from .git import GitCommonVcsProviderFactory
+from .history import Commit, History
 from .mixins import CliRunnerMixin
 
 
 class GitCliVcsProvider(VcsProvider, CliRunnerMixin):
     """"""
 
     __GIT_EXECUTABLE_NAME = "git"
@@ -220,14 +221,50 @@
             return len(lines)
         except CalledProcessError as cpe:
             raise VcsProviderError(
                 f"Failed to receive number of changes that are not committed."
                 f" Reason: {cpe.stderr}"
             ) from cpe
 
+    def get_history(self, since_last_tag: bool = True) -> History:
+        """"""
+        commit_history: str = ""
+        if since_last_tag:
+            last_tag: Optional[Version] = self.get_most_recent_tag()
+            if last_tag is not None:
+                last_tag_name: str = (
+                    f"v{Pep440VersionFormatter().format(last_tag)}"
+                )
+                commit_history = f"{last_tag_name}..HEAD"
+
+        try:
+            _, output, _ = self.run(
+                self.git_executable_path,
+                ("log", commit_history, "--format=%s"),
+                raise_on_exit=True,
+                cwd=self.current_path,
+            )
+            logger.debug(
+                "The following commits have been received for %s:\n%s",
+                commit_history,
+                output,
+            )
+            commit_texts: list[str] = output.split("\n")
+
+            commits: list[Commit] = [
+                Commit(t) for t in commit_texts if t.strip() != ""
+            ]
+
+            return History(commits)
+
+        except CalledProcessError as cpe:
+            raise VcsProviderError(
+                f"Failed to receive commit history. Reason: {cpe.stderr}"
+            ) from cpe
+
 
 @vcs_provider("git-cli")
 class GitCliVcsProviderFactory(GitCommonVcsProviderFactory):
     """"""
 
     def _create_provider(self, path: Path) -> VcsProvider:
         """
```

### Comparing `pdm_bump-0.7.3/src/pdm_bump/vcs/mixins.py` & `pdm_bump-0.8.0a1/src/pdm_bump/vcs/mixins.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.3/tests/action_test.py` & `pdm_bump-0.8.0a1/tests/action_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,14 +26,20 @@
 )
 from pdm_bump.actions.preview import (
     PreviewMismatchError,
     AlphaIncrementingVersionModifier,
     BetaIncrementingVersionModifier,
     ReleaseCandidateIncrementingVersionModifier,
 )
+from pdm_bump.actions.poetry_like import (
+    PoetryLikePreReleaseVersionModifier,
+    PoetryLikePreMajorVersionModifier,
+    PoetryLikePreMinorVersionModifier,
+    PoetryLikePrePatchVersionModifier,
+)
 
 from pdm_bump.core.version import Version
 
 import pytest
 
 parametrize = pytest.mark.parametrize
 assert_raises = pytest.raises
@@ -184,15 +190,15 @@
     (
         "Increment minor parts without removing pre-parts and alpha pre-parts",
         "1.0.0a1",
         "1.1.0a1",
         lambda v: MinorIncrementingVersionModifier(v, _unit_test_persister, False),
     ),
     (
-        "Increment minor parts without removing pre-parts and beta pre-parts",
+        "Increment minor parVersionModifierts without removing pre-parts and beta pre-parts",
         "1.0.0b1",
         "1.1.0b1",
         lambda v: MinorIncrementingVersionModifier(v, _unit_test_persister, False),
     ),
     (
         "Increment minor parts without removing pre-parts and rc pre-parts",
         "1.0.0rc1",
@@ -645,61 +651,295 @@
     ),
     (
         "Remove non-final parts",
         "1.2.3-b4-post6-dev8+local9",
         "1.2.3",
         lambda v: FinalizingVersionModifier(v, _unit_test_persister),
     ),
-]  # TODO Test Dev and Post Incrementing modifier
+    (
+        "Increment development part of existing development version",
+        "1.2.3-dev1",
+        "1.2.3-dev2",
+        lambda v: DevelopmentVersionIncrementingVersionModifier(v, _unit_test_persister),
+    ),
+    (
+        "Increment development part of non-existing development version",
+        "1.2.3",
+        "1.2.4-dev1",
+        lambda v: DevelopmentVersionIncrementingVersionModifier(v, _unit_test_persister),
+    ),
+    (
+        "Increment development part of existing post and non-existing development version",
+        "1.2.3-post6",
+        "1.2.4-dev1",
+        lambda v: DevelopmentVersionIncrementingVersionModifier(v, _unit_test_persister),
+    ),
+    (
+        "Increment development part of existing post and existing development version",
+        "1.2.3-post6-dev1",
+        "1.2.3-post6-dev2",
+        lambda v: DevelopmentVersionIncrementingVersionModifier(v, _unit_test_persister),
+    ),
+    (
+        "Increment development part of existing post and existing development version with local revision",
+        "1.2.3-post6-dev1+local9",
+        "1.2.3-post6-dev2+local9",
+        lambda v: DevelopmentVersionIncrementingVersionModifier(v, _unit_test_persister),
+    ),
+    (
+        "Increment development part of existing development version with local revision",
+        "1.2.3-dev1+local9",
+        "1.2.3-dev2+local9",
+        lambda v: DevelopmentVersionIncrementingVersionModifier(v, _unit_test_persister),
+    ),
+    (
+        "Increment development part of existing post and non-existing development version with local revision",
+        "1.2.3-post1+local9",
+        "1.2.4-dev1+local9",
+        lambda v: DevelopmentVersionIncrementingVersionModifier(v, _unit_test_persister),
+    ),
+    (
+        "Increment post part of a non-existing post part",
+        "1.2.3",
+        "1.2.3-post1",
+        lambda v: PostVersionIncrementingVersionModifier(v, _unit_test_persister),
+    ),
+    (
+        "Increment post part of an existing post part",
+        "1.2.3-post1",
+        "1.2.3-post2",
+        lambda v: PostVersionIncrementingVersionModifier(v, _unit_test_persister),
+    ),
+    (
+        "Increment post part of a non-existing post part, but dev exists",
+        "1.2.3-dev3",
+        "1.2.3-post1",
+        lambda v: PostVersionIncrementingVersionModifier(v, _unit_test_persister),
+    ),
+    (
+        "Increment post part of an existing post part, but dev exists",
+        "1.2.3-post1-dev3",
+        "1.2.3-post2",
+        lambda v: PostVersionIncrementingVersionModifier(v, _unit_test_persister),
+    ),
+    (
+        "Increment post part of a non-existing post part, but local exists",
+        "1.2.3+local1",
+        "1.2.3-post1+local1",
+        lambda v: PostVersionIncrementingVersionModifier(v, _unit_test_persister),
+    ),
+    (
+        "Increment post part of a non-existing post part, but dev and local exist",
+        "1.2.3-dev1+local1",
+        "1.2.3-post1+local1",
+        lambda v: PostVersionIncrementingVersionModifier(v, _unit_test_persister),
+    ),
+    (
+        "Run premajor from poetry version commands (demo from https://python-poetry.org/docs/cli/#version)",
+        "1.0.2",
+        "2.0.0a0",
+        lambda v: PoetryLikePreMajorVersionModifier(v, _unit_test_persister),
+    ),
+    (
+        "Run preminor from poetry version commands (demo from https://python-poetry.org/docs/cli/#version)",
+        "1.0.2",
+        "1.1.0a0",
+        lambda v: PoetryLikePreMinorVersionModifier(v, _unit_test_persister),
+    ),
+    (
+        "Run prepatch from poetry version commands (demo from https://python-poetry.org/docs/cli/#version)",
+        "1.0.2",
+        "1.0.3a0",
+        lambda v: PoetryLikePrePatchVersionModifier(v, _unit_test_persister),
+    ),
+    (
+        "Run prerelease from poetry version commands (demo from https://python-poetry.org/docs/cli/#version)",
+        "1.0.2",
+        "1.0.3a0",
+        lambda v: PoetryLikePreReleaseVersionModifier(v, _unit_test_persister),
+    ),
+    (
+        "Run prerelease from poetry version commands (demo from https://python-poetry.org/docs/cli/#version)",
+        "1.0.3a0",
+        "1.0.3a1",
+        lambda v: PoetryLikePreReleaseVersionModifier(v, _unit_test_persister),
+    ),
+    (
+        "Run prerelease from poetry version commands (demo from https://python-poetry.org/docs/cli/#version)",
+        "1.0.3b0",
+        "1.0.3b1",
+        lambda v: PoetryLikePreReleaseVersionModifier(v, _unit_test_persister),
+    ),
+    (
+        "Run prerelease from poetry version commands (demo from https://python-poetry.org/docs/cli/#version)",
+        "1.0.3rc0",
+        "1.0.3rc1",
+        lambda v: PoetryLikePreReleaseVersionModifier(v, _unit_test_persister),
+    ),
+]
 _CREATE_NEXT_VERSION_ERROR_PARAMS: list[
     tuple[str, str, Callable[[Version], VersionModifier]]
 ] = [
     (
         "Increment alpha version if beta is present",
         "1.2.3b1",
         lambda v: AlphaIncrementingVersionModifier(v, _unit_test_persister, False),
+        PreviewMismatchError,
     ),
     (
         "Increment alpha version if beta is present",
         "1.2.3b1",
         lambda v: AlphaIncrementingVersionModifier(v, _unit_test_persister, True),
+        PreviewMismatchError,
     ),
     (
         "Increment alpha version if rc is present",
         "1.2.3rc1",
         lambda v: AlphaIncrementingVersionModifier(v, _unit_test_persister, False),
+        PreviewMismatchError,
     ),
     (
         "Increment alpha version if rc is present",
         "1.2.3rc1",
         lambda v: AlphaIncrementingVersionModifier(v, _unit_test_persister, True),
+        PreviewMismatchError,
     ),
     (
         "Increment beta version if rc is present",
         "1.2.3rc1",
         lambda v: BetaIncrementingVersionModifier(v, _unit_test_persister, False),
+        PreviewMismatchError,
     ),
     (
         "Increment beta version if rc is present",
         "1.2.3rc1",
         lambda v: BetaIncrementingVersionModifier(v, _unit_test_persister, True),
+        PreviewMismatchError,
+    ),
+    (
+        "Pre-Major if version is dev version",
+        "1.2.3-dev1",
+        lambda v: PoetryLikePreMajorVersionModifier(v, _unit_test_persister),
+        ValueError,
+    ),
+    (
+        "Pre-Major if version is local version",
+        "1.2.3+local17",
+        lambda v: PoetryLikePreMajorVersionModifier(v, _unit_test_persister),
+        ValueError,
+    ),
+    (
+        "Pre-Major if version is post version",
+        "1.2.3-post12",
+        lambda v: PoetryLikePreMajorVersionModifier(v, _unit_test_persister),
+        ValueError,
+    ),
+    (
+        "Pre-Major if version is alpha version",
+        "1.2.3a23",
+        lambda v: PoetryLikePreMajorVersionModifier(v, _unit_test_persister),
+        ValueError,
+    ),
+    (
+        "Pre-Major if version is beta version",
+        "1.2.3b23",
+        lambda v: PoetryLikePreMajorVersionModifier(v, _unit_test_persister),
+        ValueError,
+    ),
+    (
+        "Pre-Major if version is release candidate",
+        "1.2.3rc23",
+        lambda v: PoetryLikePreMajorVersionModifier(v, _unit_test_persister),
+        ValueError,
+    ),
+    (
+        "Pre-Minor if version is dev version",
+        "1.2.3-dev1",
+        lambda v: PoetryLikePreMinorVersionModifier(v, _unit_test_persister),
+        ValueError,
+    ),
+    (
+        "Pre-Minor if version is local version",
+        "1.2.3+local17",
+        lambda v: PoetryLikePreMinorVersionModifier(v, _unit_test_persister),
+        ValueError,
+    ),
+    (
+        "Pre-Minor if version is post version",
+        "1.2.3-post12",
+        lambda v: PoetryLikePreMinorVersionModifier(v, _unit_test_persister),
+        ValueError,
+    ),
+    (
+        "Pre-Minor if version is alpha version",
+        "1.2.3a23",
+        lambda v: PoetryLikePreMinorVersionModifier(v, _unit_test_persister),
+        ValueError,
+    ),
+    (
+        "Pre-Minor if version is beta version",
+        "1.2.3b23",
+        lambda v: PoetryLikePreMinorVersionModifier(v, _unit_test_persister),
+        ValueError,
+    ),
+    (
+        "Pre-Minor if version is release candidate",
+        "1.2.3rc23",
+        lambda v: PoetryLikePreMinorVersionModifier(v, _unit_test_persister),
+        ValueError,
+    ),
+    (
+        "Pre-Patch if version is dev version",
+        "1.2.3-dev1",
+        lambda v: PoetryLikePrePatchVersionModifier(v, _unit_test_persister),
+        ValueError,
+    ),
+    (
+        "Pre-Patch if version is local version",
+        "1.2.3+local17",
+        lambda v: PoetryLikePrePatchVersionModifier(v, _unit_test_persister),
+        ValueError,
+    ),
+    (
+        "Pre-Patch if version is post version",
+        "1.2.3-post12",
+        lambda v: PoetryLikePrePatchVersionModifier(v, _unit_test_persister),
+        ValueError,
+    ),
+    (
+        "Pre-Patch if version is alpha version",
+        "1.2.3a23",
+        lambda v: PoetryLikePrePatchVersionModifier(v, _unit_test_persister),
+        ValueError,
+    ),
+    (
+        "Pre-Patch if version is beta version",
+        "1.2.3b23",
+        lambda v: PoetryLikePrePatchVersionModifier(v, _unit_test_persister),
+        ValueError,
+    ),
+    (
+        "Pre-Patch if version is release candidate",
+        "1.2.3rc23",
+        lambda v: PoetryLikePrePatchVersionModifier(v, _unit_test_persister),
+        ValueError,
     ),
 ]
 
 @parametrize(",".join(["message", "current_version_str", "expected_version_str", "factory"]), _CREATE_NEXT_VERSION_PARAMS)
 def test_create_next_version_success(message, current_version_str, expected_version_str, factory) -> None:
     current: Version = Version.from_string(current_version_str)
     expected: Version = Version.from_string(expected_version_str)
 
     command: VersionModifier = factory(current)
 
     modified: Version = command.create_new_version()
     assert modified == expected
 
-@parametrize(",".join(["message", "current_version_str", "factory"]), _CREATE_NEXT_VERSION_ERROR_PARAMS)
-def test_create_next_version_fail(message, current_version_str, factory) -> None:
+@parametrize(",".join(["message", "current_version_str", "factory", "exception_type"]), _CREATE_NEXT_VERSION_ERROR_PARAMS)
+def test_create_next_version_fail(message, current_version_str, factory, exception_type) -> None:
     current: Version = Version.from_string(current_version_str)
 
     command: VersionModifier = factory(current)
 
-    with assert_raises(PreviewMismatchError):
+    with assert_raises(exception_type):
         _ = command.create_new_version()
```

### Comparing `pdm_bump-0.7.3/tests/plugin_test.py` & `pdm_bump-0.8.0a1/tests/plugin_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,14 +70,18 @@
     ("minor", "minor"),
     ("micro", "micro"),
     ("patch", "patch"),
     ("pre-release", "pre-release"),
     ("no-pre-release", "no-pre-release"),
     ("post", "post"),
     ("dev", "dev"),
+    ("prerelease", "prerelease"),
+    ("premajor", "premajor"),
+    ("preminor", "preminor"),
+    ("prepatch", "prepatch"),
 ]
 SUB_TEST_PARAMS_PRE_SUCCESS: Iterable[tuple[str, str]] = [
     ("alpha", "alpha"),
     ("beta", "beta"),
     ("c", "c"),
     ("rc", "rc"),
 ]
```

### Comparing `pdm_bump-0.7.3/tests/version_test.py` & `pdm_bump-0.8.0a1/tests/version_test.py`

 * *Files identical despite different names*

