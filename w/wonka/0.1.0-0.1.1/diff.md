# Comparing `tmp/wonka-0.1.0.tar.gz` & `tmp/wonka-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wonka-0.1.0.tar", last modified: Mon Jul  3 18:13:05 2023, max compression
+gzip compressed data, was "wonka-0.1.1.tar", last modified: Sat Jul  8 16:03:59 2023, max compression
```

## Comparing `wonka-0.1.0.tar` & `wonka-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rwxr-xr-x   0        0        0    10247 2023-05-28 01:33:59.551260 wonka-0.1.0/LICENSE
--rwxr-xr-x   0        0        0    19947 2023-07-03 17:04:30.327899 wonka-0.1.0/README.md
--rwxr-xr-x   0        0        0     2273 2023-07-03 18:13:05.756037 wonka-0.1.0/pyproject.toml
--rwxr-xr-x   0        0        0     1218 2023-05-29 08:49:55.725143 wonka-0.1.0/src/wonka/__init__.py
--rwxr-xr-x   0        0        0     6095 2023-06-02 23:03:35.347076 wonka-0.1.0/src/wonka/base.py
--rwxr-xr-x   0        0        0     4665 2023-07-01 02:33:15.223761 wonka-0.1.0/src/wonka/configuration.py
--rwxr-xr-x   0        0        0     7620 2023-06-02 22:43:14.108389 wonka-0.1.0/src/wonka/dispatchers.py
--rwxr-xr-x   0        0        0     2919 2023-05-18 18:18:49.728755 wonka-0.1.0/src/wonka/managers.py
--rwxr-xr-x   0        0        0     4959 2023-05-18 18:18:49.746900 wonka-0.1.0/src/wonka/producers.py
--rwxr-xr-x   0        0        0     2052 2023-05-18 18:18:49.761809 wonka-0.1.0/src/wonka/prototypers.py
--rwxr-xr-x   0        0        0     5568 2023-05-18 18:18:49.777692 wonka-0.1.0/src/wonka/registries.py
--rwxr-xr-x   0        0        0     4352 2023-05-18 18:18:49.792545 wonka-0.1.0/src/wonka/shared.py
--rwxr-xr-x   0        0        0     3393 2023-05-18 18:18:49.805357 wonka-0.1.0/src/wonka/storage.py
--rwxr-xr-x   0        0        0      156 2023-07-02 23:46:14.912442 wonka-0.1.0/tests/__init__.py
--rwxr-xr-x   0        0        0      157 2023-07-03 17:49:46.252104 wonka-0.1.0/tests/conftest.py
--rwxr-xr-x   0        0        0     2278 2023-07-03 12:24:25.357007 wonka-0.1.0/tests/test_dispatchers.py
--rwxr-xr-x   0        0        0     1885 2023-07-02 23:44:18.089377 wonka-0.1.0/tests/test_managers.py
--rwxr-xr-x   0        0        0     2465 2023-07-02 23:44:39.655684 wonka-0.1.0/tests/test_producers.py
--rwxr-xr-x   0        0        0     1426 2023-07-02 23:44:56.592550 wonka-0.1.0/tests/test_prototypers.py
--rwxr-xr-x   0        0        0     1991 2023-07-02 23:45:16.845749 wonka-0.1.0/tests/test_registries.py
--rwxr-xr-x   0        0        0     2133 2023-07-02 23:45:33.383975 wonka-0.1.0/tests/test_storage.py
--rw-r--r--   0        0        0    21135 1970-01-01 00:00:00.000000 wonka-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0    10247 2023-05-28 01:33:59.551260 wonka-0.1.1/LICENSE
+-rwxr-xr-x   0        0        0    20089 2023-07-08 01:00:42.113134 wonka-0.1.1/README.md
+-rwxr-xr-x   0        0        0     2686 2023-07-08 16:03:59.106012 wonka-0.1.1/pyproject.toml
+-rwxr-xr-x   0        0        0     1112 2023-07-08 16:02:59.264633 wonka-0.1.1/src/wonka/__init__.py
+-rwxr-xr-x   0        0        0     5733 2023-07-07 05:42:43.924198 wonka-0.1.1/src/wonka/base.py
+-rwxr-xr-x   0        0        0     3979 2023-07-08 15:56:06.770545 wonka-0.1.1/src/wonka/configuration.py
+-rwxr-xr-x   0        0        0     6922 2023-07-08 15:57:25.850437 wonka-0.1.1/src/wonka/dispatchers.py
+-rwxr-xr-x   0        0        0     2203 2023-07-08 15:57:53.426396 wonka-0.1.1/src/wonka/managers.py
+-rwxr-xr-x   0        0        0     4239 2023-07-08 15:58:28.141472 wonka-0.1.1/src/wonka/producers.py
+-rwxr-xr-x   0        0        0     1368 2023-07-08 15:59:01.660110 wonka-0.1.1/src/wonka/prototypers.py
+-rwxr-xr-x   0        0        0     4859 2023-07-08 15:59:32.864526 wonka-0.1.1/src/wonka/registries.py
+-rwxr-xr-x   0        0        0     3607 2023-07-08 16:00:09.156611 wonka-0.1.1/src/wonka/shared.py
+-rwxr-xr-x   0        0        0     2701 2023-07-08 16:00:45.744688 wonka-0.1.1/src/wonka/storage.py
+-rwxr-xr-x   0        0        0      156 2023-07-02 23:46:14.912442 wonka-0.1.1/tests/__init__.py
+-rwxr-xr-x   0        0        0      157 2023-07-03 17:49:46.252104 wonka-0.1.1/tests/conftest.py
+-rwxr-xr-x   0        0        0     1570 2023-07-08 15:48:31.058762 wonka-0.1.1/tests/test_dispatchers.py
+-rwxr-xr-x   0        0        0     1143 2023-07-08 15:48:10.108826 wonka-0.1.1/tests/test_managers.py
+-rwxr-xr-x   0        0        0     1702 2023-07-08 15:50:50.658426 wonka-0.1.1/tests/test_producers.py
+-rwxr-xr-x   0        0        0      713 2023-07-08 15:52:59.857176 wonka-0.1.1/tests/test_prototypers.py
+-rwxr-xr-x   0        0        0     1280 2023-07-08 15:53:30.455489 wonka-0.1.1/tests/test_registries.py
+-rwxr-xr-x   0        0        0     1425 2023-07-08 15:54:13.786424 wonka-0.1.1/tests/test_storage.py
+-rw-r--r--   0        0        0    21277 1970-01-01 00:00:00.000000 wonka-0.1.1/PKG-INFO
```

### Comparing `wonka-0.1.0/LICENSE` & `wonka-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wonka-0.1.0/README.md` & `wonka-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # wonka
 
 <p align="center">
-<img src="./docs/assets/top_hat.png" alt="wonka top hat logo" style="width:250px;"/>
+<img src="./docs/img/top_hat.png" alt="wonka top hat logo" style="width:250px;"/>
 </p>
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/wonka.svg?style=for-the-badge&logo=PyPI)](https://pypi.org/project/wonka/)
 [![Documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=for-the-badge&logo=github)](https://WithPrecedent.github.io/wonka)
-[![GitHub Actions](https://img.shields.io/github/actions/workflow/status/WithPrecedent/wonka/actions?style=for-the-badge&logo=githubactions&logoColor=white)](https://img.shields.io/github/actions/)
 ![Code Coverage](https://img.shields.io/codecov/c/github/WithPrecedent/wonka?style=for-the-badge&logo=codecov&logoColor=white)
 [![PDM Managed](https://img.shields.io/badge/pdm-managed-blueviolet?style=for-the-badge)](https://pdm.fming.dev)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg?style=for-the-badge&logo=apache)](https://opensource.org/licenses/Apache-2.0)
+<!-- ![GitHub Actions](https://img.shields.io/github/actions/workflow/status/WithPrecedent/wonka/actions?style=for-the-badge&logo=githubactions&logoColor=white) -->
 
 ## What is wonka?
 
 `wonka`[^1] is an extensible library that enables simple implementation of class and object constructors in Python. Out-of-the-box, `wonka` includes various creational design patterns, from registry factories to prototypers to composite builder workflows. It is also easy to add custom factories,[^2] while taking advantage of `wonka`'s convenient mixin classes and helper functions. This readme file offers a basic outline of how `wonka` works. If you would prefer to jump right into the full documentation, go [here](https://WithPrecedent.github.io/wonka).
 
 ## Why use wonka?
 
@@ -115,15 +115,15 @@
 class Settings(wonka.Sourcerer):
     
     contents: MutableMapping[Hashable, Any] = dataclasses.field(
         default_factory = dict)
     defaults: Optional[MutableMapping[Hashable, Any]] = dataclasses.field(
         default_factory = dict)
     infer_types: Optional[bool] = True
-    sources: ClassVar[MutableMapping[Type[Any], str]] = {
+    sources: ClassVar[MutableMapping[type[Any], str]] = {
         MutableMapping, 'dictionary',
         pathlib.Path, 'path',
         str, 'path'}
 
     @classmethod
     def from_dictionary(cls, item: MutableMapping[Hashable, Any]) -> Settings:
         """Creates a Settings instance from a dict-like object."""      
@@ -165,20 +165,20 @@
 
 * Registries - factories that build classes or objects from explicit or implicit registries.
 * Dispatchers - factories that call appropriate creation methods or functions based on the type or content of data passed.
 * Prototypers - factories that clone exsting classes or objects.
 
 All `wonka` factory classes have a `create` class method which is used to construct new items. The only required parameter for `create` is `item`, which contains the data for building products. Other parameters are optional, but may be used for greater functionality, particularly in regard to `Producer` mixins, discussed below.
 
-These are the registry factory classes:
+These are the registry factory classes. Keys for any registry-style factory follow the naming convention of the global setting `_KEY_NAMER` (defaults to snakecase) which may be changed with `set_keyer`. These are the registration-style classes:
 
 * `Registrar`: a factory that creates items from data stored in the `registry` class attribute (which may be any dict-like object).
-* `Subclasser`: mixin that acts like a `Registrar`, but without the `registry` attribute. Instead, the class creates a dictionary facade at runtime by drawing data from the `__subclasses__` attribute of every class. Keys for 'registry' follow the naming convenction of the global setting `_KEY_NAMER` (defaults to snakecase) which may be changed with `set_keyer`.
+* `Subclasser`: mixin that acts like a `Registrar`, but without the `registry` attribute. Instead, the class creates a dictionary facade at runtime by drawing data from the `__subclasses__` attribute of every class.
 
-The second type of factory is a dispatch type. These factories will call creation class methods of subclasses that follow the naming convention of `_METHOD_NAMER` (`f'from_{snakecase(substring))}'` by default) which may be changed with `set_method_namer`. These are the dispatcher factories:
+The second type of factory is dispatch. These factories will call creation class methods of subclasses that follow the naming convention of `_METHOD_NAMER` (`f'from_{snakecase(substring))}'` by default) which may be changed with `set_method_namer`. These are the dispatcher factories:
 
 * `Sourcerer`: calls the appropriate creation class method based on the type of the first passed argument. The keys of `sources` are types which the `item` argument may either be instances of subclasses of those types to trigger the dispatching to the appropriate creation method.
 * `Delegate`: similar to `Sourcerer`, but it does not have a `sources` attribute. Instead, it uses the string name of the type of the `item` argument. This is far less forgiving than the process used by `Sourcerer` and should only be used if you are absolutely sure that the string names of the `item` arguments will always correspond with a creation method in the `Delegate`.
 
 The final type of factory, the prototypers, clone existing classes or objects. Out of the box, `wonka` includes just one prototyper:
 
 * `Scribe`: creates a [deep copy](https://docs.python.org/3/library/copy.html) of an existing object or class. If mixed in with certain `Producer` subcclasses, it can add, modify, or delete existing attributes of the cloned object in its copy.
@@ -219,22 +219,22 @@
 
 In addition to the core classes described above, `wonka` includes other convenience classes and functions, each of which is outlined below.
 
 The library includes `Manufacturer`, a dictionary of factories, if you want all of your project factories in one location and runtime addition and subtraction of factories.
 
 `wonka` also includes convenience functions for changing global settings that set naming conventions for registry keys and creation method names. Those methods and settings are:
 
-* 'set_compatibility_rule' sets whether `wonka` runs a validation check to see if a prospective factory is either a subclass of `Factory` or a subclass instance of `Manager`. If True, strict inheritance will be enforced. If False, no check will be performed and any incompatibility will only be discovered when the constructor's `create` method is called. The value for this setting is stored in `_STRICT_COMPATIBILITY` and defaults to True.
+* `set_compatibility_rule` sets whether `wonka` runs a validation check to see if a prospective factory is either a subclass of `Factory` or a subclass instance of `Manager`. If True, strict inheritance will be enforced. If False, no check will be performed and any incompatibility will only be discovered when the constructor's `create` method is called. The value for this setting is stored in `_STRICT_COMPATIBILITY` and defaults to True.
 * `set_keyer` may be used to change the global value of `_KEY_NAMER`, which controls the naming convention for registry dictionary keys in `wonka`. This is particularly important for `Subclasser`, which automatically creates keys based on a class' `__subclasses__` attribute. By default, `_KEY_NAMER' infers a snakecase name of any passed value.
 * `set_method_namer` may be used to change the global value of the `_METHOD_NAMER`, which controls the naming convention for creation method names used in dispatcher factories. By default `_METHOD_NAMER` uses a prefix of 'from_' followed by the snakecase name of the type of the passed `item` argument. So, as the example above indicates, a class method named `from_path` is used for creating a `Settings` instance from a file path.
 * `set_overwrite_rule` sets whether existing attributes are overwritten when parameters are passed to a factory `create` method. This situation only arises with a registry-based factory stores at least some instances (instead of just classes). In such a situation, if the value is set to True, the passed parameters will be injected and overwrite any existing values. If False, no existing values will be overwritten, even if a parameter with the same attribute name is passed. The value for this setting is stored in `_OVERWRITE` and defaults to True.
 
 ## Contributing
 
-Contributors are always welcome and should find `wonka` easy to work with. The project is highly documented so that users and developers can make `wonka` work with their projects. It is designed for Python coders at all levels. Even beginners should be able to follow the readable code and internal documentation to understand how it works.
+Contributors are always welcome and should find `wonka` easy to work with. The project is highly documented so that users and developers can make `wonka` work with their projects. It is designed for Python coders at all levels. Even beginners should be able to follow the readable code and internal documentation to understand how it works. If you wish to contribute, please read the [Contribution Guide](./CONTRIBUTING.md) and [Code of Conduct](./CODE_OF_CONDUCT.md).
 
 Notably, `wonka` is 100% compatible with my other project framework libraries, of which it was originally a part. This is why you should feel confident in the continued development and maintenance of the library - it is essential part of my overall work. I have decided to make it available as a separate library for those that just want to use its implementation without the other components of my project framework ecosystem. So, for example, any of the many registry types of [ashford](https://github.com/WithPrecedent/ashford) can be used with a `Registrar` in `wonka`. Further, for project workflow pipelining, where dynamic factories are essential, the `wonka` classes are interwoven and can be extended in the [chrisjen](https://github.com/WithPrecedent/chrisjen) and [amos](https://github.com/WithPrecedent/amos) packages. Also, for those using configuration option files, `wonka` is supported by the [bobbie](https://github.com/WithPrecedent/bobbie) project settings library. So, I, and any other maintainers, will do my best to promptly integrate any contributions.
 
 ## Similar Projects
 
 If `wonka` does not fit your needs, you might find one of these other packages helpful. None of them does the same things that `wonka` does (which is why I created this library), but they might fit your particular project needs better.
```

### Comparing `wonka-0.1.0/pyproject.toml` & `wonka-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "wonka"
 description = "Extensible, lightweight, accessible constructors"
 authors = [
     { name = "Corey Rayburn Yung", email = "coreyrayburnyung@gmail.com" },
 ]
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -49,57 +49,70 @@
 
 [tool.pdm]
 plugins = [
     "pdm-multirun",
 ]
 
 [tool.pdm.build]
-package-dir = "src/wonka"
+package-dir = "src"
 editable-backend = "editables"
 
 [tool.pdm.dev-dependencies]
 duty = [
-    "duty>=0.10",
+    "duty >= 0.10",
 ]
 ci-quality = [
     "wonka[duty, docs, quality, typing, security]",
 ]
 ci-tests = [
     "wonka[duty, tests]",
 ]
 docs = [
-    "black>=23.1",
-    "markdown-callouts>=0.2",
-    "markdown-exec>=0.5",
-    "mkdocs>=1.3",
-    "mkdocs-coverage>=0.2",
-    "mkdocs-gen-files>=0.3",
-    "mkdocs-git-committers-plugin-2>=1.1",
-    "mkdocs-literate-nav>=0.4",
-    "mkdocs-material>=7.3",
-    "mkdocs-minify-plugin>=0.6.4",
-    "mkdocstrings[python]>=0.18",
-    "toml>=0.10",
+    "black >= 23.1",
+    "markdown-callouts >= 0.2",
+    "markdown-exec >= 0.5",
+    "mkdocs >= 1.3",
+    "mkdocs-coverage >= 0.2",
+    "mkdocs-gen-files >= 0.3",
+    "mkdocs-git-committers-plugin-2 >= 1.1",
+    "mkdocs-literate-nav >= 0.4",
+    "mkdocs-material >= 7.3",
+    "mkdocs-minify-plugin >= 0.6.4",
+    "mkdocstrings[python] >= 0.18",
+    "toml >= 0.10",
 ]
 maintain = [
-    "black>=23.1",
-    "blacken-docs>=1.13",
-    "git-changelog>=1.0",
+    "black >= 23.1",
+    "blacken-docs >= 1.13",
+    "git-changelog >= 1.0",
+    "toml >= 0.10",
+    "yapf >= 0.40.1",
 ]
 quality = [
-    "ruff>=0.0.246",
+    "ruff >= 0.0.246",
 ]
 tests = [
-    "pytest>=6.2",
-    "pytest-cov>=3.0",
-    "pytest-randomly>=3.10",
-    "pytest-xdist>=2.4",
+    "pytest >= 6.2",
+    "pytest-cov >= 3.0",
+    "pytest-randomly >= 3.10",
+    "pytest-xdist >= 2.4",
 ]
 typing = [
-    "mypy>=0.910",
-    "types-markdown>=3.3",
-    "types-pyyaml>=6.0",
-    "types-toml>=0.10",
+    "mypy >= 0.910",
+    "types-markdown >= 3.3",
+    "types-pyyaml >= 6.0",
+    "types-toml >= 0.10",
 ]
 security = [
-    "safety>=2",
+    "safety >= 2",
 ]
+
+[tool.yapf]
+based_on_style = "google"
+column_limit = 80
+spaces_before_comment = 4
+split_before_logical_operator = true
+ALIGN_CLOSING_BRACKET_WITH_VISUAL_INDENT = false
+BLANK_LINE_BEFORE_CLASS_DOCSTRING = false
+BLANK_LINE_BEFORE_MODULE_DOCSTRING = false
+COALESCE_BRACKETS = true
+SPACES_AROUND_DEFAULT_OR_NAMED_ASSIGN = false
```

### Comparing `wonka-0.1.0/src/wonka/__init__.py` & `wonka-0.1.1/src/wonka/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-# wonka: runtime class and object creation, made simple
-# Corey Rayburn Yung <coreyrayburnyung@gmail.com>
-# Copyright 2023, Corey Rayburn Yung
-# License: Apache-2.0
-    
-# ToDo:
-#     Increase test coverage
-    
+""" 
+An extensible library that enables simple implementation of class and object 
+constructors. 
+"""
+   
 from __future__ import annotations
 
-__version__ = '0.1.0'
+__version__ = '0.1.1'
 
 __author__ = 'Corey Rayburn Yung'
 
 __all__: list[str] = [
     'Assembler',
     'Classer',
     'Delegate',
```

### Comparing `wonka-0.1.0/src/wonka/base.py` & `wonka-0.1.1/src/wonka/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,31 @@
+"""
+Base classes for wonka factories.
 
-# base: base classes for wonka factories
-# Corey Rayburn Yung <coreyrayburnyung@gmail.com>
-# Copyright 2023, Corey Rayburn Yung
-# License: Apache-2.0
-
-# Contents:
-#     Factory (abc.ABC): interface for basic wonka creation classes. A 'create' 
-#         class method is required for subclasses.
-#     Manager (Iterable, abc.ABC): iterable interface for complex construction 
-#         managers. A 'manage' instance method is required for subclasses. For
-#         compatibility as a wonka constructor, a 'create' property is included
-#         which automatically calls the 'manage' method with all args and kwargs.
-#     Producer (abc.ABC): mixin interface for classes that alter created items 
-#         before returning them. A 'produce' class method is required for 
-#         subclasses.
-#     Constructor (TypeAlias): type alias for a wonka.compatible constructor type.
-#         By default, it includes a Factory subclass, a Factory subclass instance,
-#         and a Manager subclass instance.
-
-# To Do:
-
-""" 
-The module containing the core base classes for `wonka`. 
+Contents:
+    Factory (abc.ABC): interface for basic wonka creation classes. A 'create' 
+        class method is required for subclasses.
+    Manager (Iterable, abc.ABC): iterable interface for complex construction 
+        managers. A 'manage' instance method is required for subclasses. For
+        compatibility as a wonka constructor, a 'create' property is included
+        which automatically calls the 'manage' method with all args and kwargs.
+    Producer (abc.ABC): mixin interface for classes that alter created items 
+        before returning them. A 'produce' class method is required for 
+        subclasses.
+    Constructor (TypeAlias): type alias for a wonka-compatible constructor type.
+        By default, it includes a Factory subclass, a Factory subclass instance,
+        and a Manager subclass instance.
 
 """
+
 from __future__ import annotations
 import abc
 from collections.abc import Hashable, Iterable, MutableMapping
 import dataclasses
-from typing import Any, Optional, Type, TypeAlias
-
-import camina
+from typing import Any, Optional, TypeAlias
 
 
 @dataclasses.dataclass
 class Factory(abc.ABC):
     """Base for wonka constructors.
     
     A wonka Factory can be subclassed into any constructer design (not just 
@@ -59,48 +50,46 @@
 
     @classmethod
     @abc.abstractmethod
     def create(cls, item: Any, *args: Any, **kwargs: Any) -> Any:
         """Returns a created or modified item.
         
         Args:
-            item (Any): data for creation of an item or an item to be modified.     
+            item: data for creation of an item or an item to be modified.     
                          
         Returns:
             Any: created or modified item.
                 
         """
-        pass
 
 
 @dataclasses.dataclass
 class Manager(Iterable, abc.ABC):
     """Base for manageing complex class or object construction.
     
     Args:
-        contents (Iterable): an iterable containing Factory subclasses or
+        contents: an iterable containing Factory subclasses or
             Manager subclass instances.
                           
     """
     contents: Iterable
     
     """ Required Subclass Methods """
     
     @abc.abstractmethod
     def manage(self, item: Any, *args: Any, **kwargs: Any) -> Any:
         """Manages construction and/or modification based on 'item'.
         
         Args:
-            item (Any): item to be passed to factories in 'contents'.
+            item: item to be passed to factories in 'contents'.
                          
         Returns:
             Any: constructed item.
                 
         """
-        pass
 
     """ Properties """
 
     @property
     def create(self, *args, **kwargs) -> Any:
         """Calls 'manage' method with args and kwargs.
         
@@ -152,21 +141,18 @@
     def produce(
         cls,
         item: Any,
         parameters: Optional[MutableMapping[Hashable, Any]] = None) -> Any:
         """Modifies 'item' and possibly incorporates 'parameters'.
         
         Args:
-            item (Any): item to be modified. 
-            parameters: Optional[MutableMapping[Hashable, Any]]: keyword 
-                arguments to pass or add to a created instance. Defaults to 
-                None.       
+            item: item to be modified. 
+            parameters: keyword arguments to pass or add to a created instance. 
+                Defaults to None.       
                          
         Returns:
             Any: modified item.
                 
         """
-        pass
 
 
-Constructor: TypeAlias = Factory | Type[Factory] | Manager
-  
+Constructor: TypeAlias = Factory | type[Factory] | Manager
```

### Comparing `wonka-0.1.0/src/wonka/configuration.py` & `wonka-0.1.1/src/wonka/configuration.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,27 @@
-"""
-configuration: wonka settings and convenience functions for changing settings
-Corey Rayburn Yung <coreyrayburnyung@gmail.com>
-Copyright 2023, Corey Rayburn Yung
-License: Apache-2.0
-
-    Licensed under the Apache License, Version 2.0 (the "License");
-    you may not use this file except in compliance with the License.
-    You may obtain a copy of the License at
-
-        http://www.apache.org/licenses/LICENSE-2.0
-
-    Unless required by applicable law or agreed to in writing, software
-    distributed under the License is distributed on an "AS IS" BASIS,
-    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-    See the License for the specific language governing permissions and
-    limitations under the License.
+""" wonka settings and convenience functions for changing those settings.
 
 Contents:
     set_compatibility_rule: sets the global attribute compatibility rule.
     set_keyer: sets the global default function used to name dict keys.
     set_method_namer: sets the global default function used to name factory 
         creation methods.
     set_overwrite_rule: sets the global attribute overwrite rule.
     set_verbose_rule: sets the global attribute message verbosity rule.
         
-ToDo:
-
-
 """
 from __future__ import annotations
 from collections.abc import Callable
-from typing import Any, Type
+from typing import Any
 
 import camina
 
 
-_KEY_NAMER: Callable[[object | Type[Any]], str] = camina.namify
-_METHOD_NAMER: Callable[[object | Type[Any]], str] = (lambda x: f'from_{x}')
+_KEY_NAMER: Callable[[object | type[Any]], str] = camina.namify
+_METHOD_NAMER: Callable[[object | type[Any]], str] = (lambda x: f'from_{x}')
 _OVERWRITE: bool = True
 _STRICT_COMPATIBILITY: bool = True
 _VERBOSE: bool = False
 
 
 def set_compatibility_rule(compatibility: bool) -> None:
     """Sets the global attribute compatibility rule.
@@ -54,35 +35,35 @@
         
     """
     if isinstance(compatibility, bool):
         globals()._STRICT_COMPATIBILITY = compatibility
     else:
         raise TypeError('compatibility argument must be boolean')   
 
-def set_keyer(keyer: Callable[[object | Type[Any]], str]) -> None:
+def set_keyer(keyer: Callable[[object | type[Any]], str]) -> None:
     """Sets the global default function used to name dict keys.
 
     Args:
-        keyer (Callable[[object | Type[Any]], str]): function that returns a 
+        keyer (Callable[[object | type[Any]], str]): function that returns a 
             str name of any item passed.
 
     Raises:
         TypeError: if 'keyer' is not callable.
         
     """
     if isinstance(keyer, Callable):
         globals()._KEY_NAMER = keyer
     else:
         raise TypeError('keyer argument must be a callable')
 
-def set_method_namer(namer: Callable[[object | Type[Any]], str]) -> None:
+def set_method_namer(namer: Callable[[object | type[Any]], str]) -> None:
     """Sets the global default function used to name factory creation methods.
 
     Args:
-        namer (Callable[[object | Type[Any]], str]): function that returns a 
+        namer (Callable[[object | type[Any]], str]): function that returns a 
             str name of any item passed.
 
     Raises:
         TypeError: if 'keyer' is not callable.
         
     """
     if isinstance(namer, Callable):
```

### Comparing `wonka-0.1.0/src/wonka/dispatchers.py` & `wonka-0.1.1/src/wonka/dispatchers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,24 @@
-"""
-dispatchers: factory classes that call other construction methods or functions
-Corey Rayburn Yung <coreyrayburnyung@gmail.com>
-Copyright 2023, Corey Rayburn Yung
-License: Apache-2.0
-
-    Licensed under the Apache License, Version 2.0 (the "License");
-    you may not use this file except in compliance with the License.
-    You may obtain a copy of the License at
-
-        http://www.apache.org/licenses/LICENSE-2.0
-
-    Unless required by applicable law or agreed to in writing, software
-    distributed under the License is distributed on an "AS IS" BASIS,
-    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-    See the License for the specific language governing permissions and
-    limitations under the License.
+""" Dispatchers: factory classes that call other constructors.
 
 Contents: 
     Delegate (base.Factory): builds classes and/or instances using methods 
         that follow a naming convention and the str names of the types of the
         first argument passed to the 'create' class method.  
     Sourcerer (base.Factory): builds classes and/or instances using methods 
         that follow a naming convention (set at 'configuration._METHOD_NAMER') 
         and a dict of types stored in the 'sources' class attribute.
           
-ToDo:
-
-
 """
 from __future__ import annotations
 import abc
 from collections.abc import Hashable, MutableMapping
 import dataclasses
 import inspect
-from typing import Any, Callable, ClassVar, Optional, Type
+from typing import Any, Callable, ClassVar, Optional
 
 from . import base
 from . import configuration
 from . import shared
 
                     
 @dataclasses.dataclass
@@ -97,21 +78,21 @@
     The name for a Sourcerer is spelled the way it is instead of "Sorcerer" 
     because the 'sources' attribute is used. This is inspired by the Divinity:
     Original Sin games where the magic users are called "Sourcerers" because
     they may manipulate the magical energy known as "source". 
     https://divinity.fandom.com/wiki/Sourcerer
     
     Attributes:
-        sources (ClassVar[MutableMapping[Type[Any], str]]): dict with keys that
+        sources (ClassVar[MutableMapping[type[Any], str]]): dict with keys that
             are types and values are substrings of the names of methods to call
             when the key type is passed to the 'create' method. Defaults to an
             empty dict.
     
     """
-    sources: ClassVar[MutableMapping[Type[Any], str]] = dict()
+    sources: ClassVar[MutableMapping[type[Any], str]] = dict()
     
     """ Class Methods """
 
     @classmethod
     def create(
         cls,
         item: Any,
@@ -144,39 +125,39 @@
                     **kwargs)
                 return shared.finalize(item = item, parameters = parameters)
         raise KeyError(f'{item} does not match any recognized types')
 
 
 def _get_creation_method_name(
     source: Any,
-    method_namer: Optional[Callable[[object | Type[Any]], str]] = None) -> str:
+    method_namer: Optional[Callable[[object | type[Any]], str]] = None) -> str:
     """Returns the creation method name for factories that call other methods.
 
     Args:
         source (Any): source data for creating a method name.
-        method_namer (Optional[Callable[[object | Type[Any]], str]], optional): 
+        method_namer (Optional[Callable[[object | type[Any]], str]], optional): 
             callable to create the creation method name. Defaults to None. If it 
             is None, the global namer stored in configuration._METHOD_NAMER will 
             be used.
 
     Returns:
         str: name of the creation method to use.
         
     """
     if not isinstance(source, str):
         source = configuration._KEY_NAMER(source)
     namer = method_namer or configuration._METHOD_NAMER
     return namer(source)
 
-def _is_kind(item: Any, kind: Type[Any]) -> bool:
+def _is_kind(item: Any, kind: type[Any]) -> bool:
     """Returns if 'item' is an instance or subclass of 'kind'.
 
     Args:
         item (Any): item to evalute.
-        kind (Type[Any]): type to compare 'item' to.
+        kind (type[Any]): type to compare 'item' to.
 
     Returns:
         bool: whether 'item' is an instance or subclass of 'kind'.
         
     """
     return (
         isinstance(item, kind)
```

### Comparing `wonka-0.1.0/src/wonka/managers.py` & `wonka-0.1.1/src/wonka/managers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,18 @@
-"""
-managers: manager classes for iterable constructors
-Corey Rayburn Yung <coreyrayburnyung@gmail.com>
-Copyright 2023, Corey Rayburn Yung
-License: Apache-2.0
-
-    Licensed under the Apache License, Version 2.0 (the "License");
-    you may not use this file except in compliance with the License.
-    You may obtain a copy of the License at
-
-        http://www.apache.org/licenses/LICENSE-2.0
-
-    Unless required by applicable law or agreed to in writing, software
-    distributed under the License is distributed on an "AS IS" BASIS,
-    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-    See the License for the specific language governing permissions and
-    limitations under the License.
+""" Manager classes for iterable constructors. 
 
 Contents:  
     Assembler (camina.Listing, base.Manager): iterable that stores a list of
         constructors that build an item like an assembly line.
                
-ToDo:
-
-
 """
 from __future__ import annotations
-from collections.abc import Hashable, MutableSequence, Sequence
+from collections.abc import MutableSequence, Sequence
 import dataclasses
-from typing import Any, ClassVar, Optional, Type
+from typing import Any
 
 import camina
 
 from . import base
 from . import shared
```

### Comparing `wonka-0.1.0/src/wonka/producers.py` & `wonka-0.1.1/src/wonka/producers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,24 @@
-"""
-producers: mixins for created objection modification
-Corey Rayburn Yung <coreyrayburnyung@gmail.com>
-Copyright 2023, Corey Rayburn Yung
-License: Apache-2.0
-
-    Licensed under the Apache License, Version 2.0 (the "License");
-    you may not use this file except in compliance with the License.
-    You may obtain a copy of the License at
-
-        http://www.apache.org/licenses/LICENSE-2.0
-
-    Unless required by applicable law or agreed to in writing, software
-    distributed under the License is distributed on an "AS IS" BASIS,
-    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-    See the License for the specific language governing permissions and
-    limitations under the License.
+""" Mixins for created object modification.
 
 Contents:  
     Classer (base.Producer, abc.ABC): Producer with an 'produce' method that 
         always returns a class.
     Flexer (base.Producer, abc.ABC): Producer that conditions return value of 
         the 'produce' method based on whether 'parameters' are passed.
     Instancer (base.Producer, abc.ABC): Producer with an 'produce' method that 
         always returns an instance.   
-                   
-ToDo:
-
 
 """
 from __future__ import annotations
 import abc
 from collections.abc import Hashable, MutableMapping
 import dataclasses
 import inspect
-from typing import Any, ClassVar, Optional, Type
+from typing import Any, Optional
 
 from . import base
 from . import shared
 
 
 @dataclasses.dataclass
 class Classer(base.Producer, abc.ABC):
```

### Comparing `wonka-0.1.0/src/wonka/registries.py` & `wonka-0.1.1/src/wonka/registries.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,23 @@
-"""
-registries: factory classes that utilize explicit or implicit registries
-Corey Rayburn Yung <coreyrayburnyung@gmail.com>
-Copyright 2023, Corey Rayburn Yung
-License: Apache-2.0
-
-    Licensed under the Apache License, Version 2.0 (the "License");
-    you may not use this file except in compliance with the License.
-    You may obtain a copy of the License at
-
-        http://www.apache.org/licenses/LICENSE-2.0
-
-    Unless required by applicable law or agreed to in writing, software
-    distributed under the License is distributed on an "AS IS" BASIS,
-    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-    See the License for the specific language governing permissions and
-    limitations under the License.
+"""Factory classes that utilize explicit or implicit registries.
 
 Contents:  
     Registrar (base.Factory): builds classes and/or instances from a registry 
         stored in the 'registry' class attribute.
     Subclasser (base.Factory, abc.ABC): builds classes and/or instances from the 
         '__subclasses__' method and a dynamically created registry based upon 
         it. 
-                   
-ToDo:
-
 
 """
 from __future__ import annotations
 import abc
 from collections.abc import Hashable, MutableMapping
 import copy
 import dataclasses
-from typing import Any, ClassVar, Optional, Type
+from typing import Any, ClassVar, Optional
 
 from . import base
 from . import configuration
 from . import shared
 
           
 @dataclasses.dataclass
@@ -143,19 +124,19 @@
         
     """
     try:
         return copy.deepcopy(registry[item])
     except KeyError as e:
         raise KeyError(f'{item} was not found in the registry') from e
 
-def _get_all_subclasses(item: Type[Any]) -> list[Type[Any]]:
+def _get_all_subclasses(item: type[Any]) -> list[type[Any]]:
     """Returns a list of all subclasses of 'items', including indirect ones.
 
     Args:
-        item (Type[Any]): class for which to find subclasses.
+        item (type[Any]): class for which to find subclasses.
 
     Returns:
-        list[Type[Any]]: list of all subclasses of 'item'
+        list[type[Any]]: list of all subclasses of 'item'
         
     """
     return list(set(item.__subclasses__()).union(
         [s for c in item.__subclasses__() for s in _get_all_subclasses(c)]))
```

### Comparing `wonka-0.1.0/tests/test_registries.py` & `wonka-0.1.1/tests/test_managers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,13 @@
-"""
-test_registries: tests wonka registry factories
-Corey Rayburn Yung <coreyrayburnyung@gmail.com>
-Copyright 2023, Corey Rayburn Yung
-License: Apache-2.0
-
-    Licensed under the Apache License, Version 2.0 (the "License");
-    you may not use this file except in compliance with the License.
-    You may obtain a copy of the License at
-
-        http://www.apache.org/licenses/LICENSE-2.0
-
-    Unless required by applicable law or agreed to in writing, software
-    distributed under the License is distributed on an "AS IS" BASIS,
-    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-    See the License for the specific language governing permissions and
-    limitations under the License.
+""" Tests wonka construction managers."""
 
-ToDo:
-   
-    
-"""
 from __future__ import annotations
 import dataclasses
 from typing import Any, ClassVar
 
-import pytest
-
 import wonka
 
 
 @dataclasses.dataclass
 class Options(wonka.Subclasser):
     pass
 
@@ -54,28 +32,24 @@
 class Registration_Desk(wonka.Registrar):
     
     registry: ClassVar[dict[str, Any]] = {
         'configuration': Configuration, 
         'setup': Setup}
 
 
-def test_registrar():
+def test_assembler():
+    assembly_line = wonka.Assembler()
+    
     dictionary = {'verbose': True, 'processors': 8}
     config = Registration_Desk.create(
         'configuration', 
         parameters = {'contents': dictionary})
-    assert config.contents['processors'] == 8
-    assert isinstance(config, Configuration)
-    return
-
-def test_subclasser():
-    dictionary = {'verbose': True, 'processors': 8}
+    other_dictionary = {'ghost': 'town'}
     setup = Options.create(
         'configuration', 
-        parameters = {'contents': dictionary})
-    assert setup.contents['processors'] == 8
-    assert isinstance(setup, Configuration)
+        parameters = {'contents': other_dictionary})
+    assembly_line.add(config)
+    assembly_line.add(setup)
     return
 
 if __name__ == '__main__':
-    test_registrar()
-    test_subclasser()
+    test_assembler()
```

### Comparing `wonka-0.1.0/PKG-INFO` & `wonka-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wonka
-Version: 0.1.0
+Version: 0.1.1
 Summary: Extensible, lightweight, accessible constructors
 Keywords: factory construction constructor design pattern
 Author-Email: Corey Rayburn Yung <coreyrayburnyung@gmail.com>
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
@@ -25,23 +25,23 @@
 Requires-Dist: camina
 Requires-Dist: miller
 Description-Content-Type: text/markdown
 
 # wonka
 
 <p align="center">
-<img src="./docs/assets/top_hat.png" alt="wonka top hat logo" style="width:250px;"/>
+<img src="./docs/img/top_hat.png" alt="wonka top hat logo" style="width:250px;"/>
 </p>
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/wonka.svg?style=for-the-badge&logo=PyPI)](https://pypi.org/project/wonka/)
 [![Documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=for-the-badge&logo=github)](https://WithPrecedent.github.io/wonka)
-[![GitHub Actions](https://img.shields.io/github/actions/workflow/status/WithPrecedent/wonka/actions?style=for-the-badge&logo=githubactions&logoColor=white)](https://img.shields.io/github/actions/)
 ![Code Coverage](https://img.shields.io/codecov/c/github/WithPrecedent/wonka?style=for-the-badge&logo=codecov&logoColor=white)
 [![PDM Managed](https://img.shields.io/badge/pdm-managed-blueviolet?style=for-the-badge)](https://pdm.fming.dev)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg?style=for-the-badge&logo=apache)](https://opensource.org/licenses/Apache-2.0)
+<!-- ![GitHub Actions](https://img.shields.io/github/actions/workflow/status/WithPrecedent/wonka/actions?style=for-the-badge&logo=githubactions&logoColor=white) -->
 
 ## What is wonka?
 
 `wonka`[^1] is an extensible library that enables simple implementation of class and object constructors in Python. Out-of-the-box, `wonka` includes various creational design patterns, from registry factories to prototypers to composite builder workflows. It is also easy to add custom factories,[^2] while taking advantage of `wonka`'s convenient mixin classes and helper functions. This readme file offers a basic outline of how `wonka` works. If you would prefer to jump right into the full documentation, go [here](https://WithPrecedent.github.io/wonka).
 
 ## Why use wonka?
 
@@ -143,15 +143,15 @@
 class Settings(wonka.Sourcerer):
     
     contents: MutableMapping[Hashable, Any] = dataclasses.field(
         default_factory = dict)
     defaults: Optional[MutableMapping[Hashable, Any]] = dataclasses.field(
         default_factory = dict)
     infer_types: Optional[bool] = True
-    sources: ClassVar[MutableMapping[Type[Any], str]] = {
+    sources: ClassVar[MutableMapping[type[Any], str]] = {
         MutableMapping, 'dictionary',
         pathlib.Path, 'path',
         str, 'path'}
 
     @classmethod
     def from_dictionary(cls, item: MutableMapping[Hashable, Any]) -> Settings:
         """Creates a Settings instance from a dict-like object."""      
@@ -193,20 +193,20 @@
 
 * Registries - factories that build classes or objects from explicit or implicit registries.
 * Dispatchers - factories that call appropriate creation methods or functions based on the type or content of data passed.
 * Prototypers - factories that clone exsting classes or objects.
 
 All `wonka` factory classes have a `create` class method which is used to construct new items. The only required parameter for `create` is `item`, which contains the data for building products. Other parameters are optional, but may be used for greater functionality, particularly in regard to `Producer` mixins, discussed below.
 
-These are the registry factory classes:
+These are the registry factory classes. Keys for any registry-style factory follow the naming convention of the global setting `_KEY_NAMER` (defaults to snakecase) which may be changed with `set_keyer`. These are the registration-style classes:
 
 * `Registrar`: a factory that creates items from data stored in the `registry` class attribute (which may be any dict-like object).
-* `Subclasser`: mixin that acts like a `Registrar`, but without the `registry` attribute. Instead, the class creates a dictionary facade at runtime by drawing data from the `__subclasses__` attribute of every class. Keys for 'registry' follow the naming convenction of the global setting `_KEY_NAMER` (defaults to snakecase) which may be changed with `set_keyer`.
+* `Subclasser`: mixin that acts like a `Registrar`, but without the `registry` attribute. Instead, the class creates a dictionary facade at runtime by drawing data from the `__subclasses__` attribute of every class.
 
-The second type of factory is a dispatch type. These factories will call creation class methods of subclasses that follow the naming convention of `_METHOD_NAMER` (`f'from_{snakecase(substring))}'` by default) which may be changed with `set_method_namer`. These are the dispatcher factories:
+The second type of factory is dispatch. These factories will call creation class methods of subclasses that follow the naming convention of `_METHOD_NAMER` (`f'from_{snakecase(substring))}'` by default) which may be changed with `set_method_namer`. These are the dispatcher factories:
 
 * `Sourcerer`: calls the appropriate creation class method based on the type of the first passed argument. The keys of `sources` are types which the `item` argument may either be instances of subclasses of those types to trigger the dispatching to the appropriate creation method.
 * `Delegate`: similar to `Sourcerer`, but it does not have a `sources` attribute. Instead, it uses the string name of the type of the `item` argument. This is far less forgiving than the process used by `Sourcerer` and should only be used if you are absolutely sure that the string names of the `item` arguments will always correspond with a creation method in the `Delegate`.
 
 The final type of factory, the prototypers, clone existing classes or objects. Out of the box, `wonka` includes just one prototyper:
 
 * `Scribe`: creates a [deep copy](https://docs.python.org/3/library/copy.html) of an existing object or class. If mixed in with certain `Producer` subcclasses, it can add, modify, or delete existing attributes of the cloned object in its copy.
@@ -247,22 +247,22 @@
 
 In addition to the core classes described above, `wonka` includes other convenience classes and functions, each of which is outlined below.
 
 The library includes `Manufacturer`, a dictionary of factories, if you want all of your project factories in one location and runtime addition and subtraction of factories.
 
 `wonka` also includes convenience functions for changing global settings that set naming conventions for registry keys and creation method names. Those methods and settings are:
 
-* 'set_compatibility_rule' sets whether `wonka` runs a validation check to see if a prospective factory is either a subclass of `Factory` or a subclass instance of `Manager`. If True, strict inheritance will be enforced. If False, no check will be performed and any incompatibility will only be discovered when the constructor's `create` method is called. The value for this setting is stored in `_STRICT_COMPATIBILITY` and defaults to True.
+* `set_compatibility_rule` sets whether `wonka` runs a validation check to see if a prospective factory is either a subclass of `Factory` or a subclass instance of `Manager`. If True, strict inheritance will be enforced. If False, no check will be performed and any incompatibility will only be discovered when the constructor's `create` method is called. The value for this setting is stored in `_STRICT_COMPATIBILITY` and defaults to True.
 * `set_keyer` may be used to change the global value of `_KEY_NAMER`, which controls the naming convention for registry dictionary keys in `wonka`. This is particularly important for `Subclasser`, which automatically creates keys based on a class' `__subclasses__` attribute. By default, `_KEY_NAMER' infers a snakecase name of any passed value.
 * `set_method_namer` may be used to change the global value of the `_METHOD_NAMER`, which controls the naming convention for creation method names used in dispatcher factories. By default `_METHOD_NAMER` uses a prefix of 'from_' followed by the snakecase name of the type of the passed `item` argument. So, as the example above indicates, a class method named `from_path` is used for creating a `Settings` instance from a file path.
 * `set_overwrite_rule` sets whether existing attributes are overwritten when parameters are passed to a factory `create` method. This situation only arises with a registry-based factory stores at least some instances (instead of just classes). In such a situation, if the value is set to True, the passed parameters will be injected and overwrite any existing values. If False, no existing values will be overwritten, even if a parameter with the same attribute name is passed. The value for this setting is stored in `_OVERWRITE` and defaults to True.
 
 ## Contributing
 
-Contributors are always welcome and should find `wonka` easy to work with. The project is highly documented so that users and developers can make `wonka` work with their projects. It is designed for Python coders at all levels. Even beginners should be able to follow the readable code and internal documentation to understand how it works.
+Contributors are always welcome and should find `wonka` easy to work with. The project is highly documented so that users and developers can make `wonka` work with their projects. It is designed for Python coders at all levels. Even beginners should be able to follow the readable code and internal documentation to understand how it works. If you wish to contribute, please read the [Contribution Guide](./CONTRIBUTING.md) and [Code of Conduct](./CODE_OF_CONDUCT.md).
 
 Notably, `wonka` is 100% compatible with my other project framework libraries, of which it was originally a part. This is why you should feel confident in the continued development and maintenance of the library - it is essential part of my overall work. I have decided to make it available as a separate library for those that just want to use its implementation without the other components of my project framework ecosystem. So, for example, any of the many registry types of [ashford](https://github.com/WithPrecedent/ashford) can be used with a `Registrar` in `wonka`. Further, for project workflow pipelining, where dynamic factories are essential, the `wonka` classes are interwoven and can be extended in the [chrisjen](https://github.com/WithPrecedent/chrisjen) and [amos](https://github.com/WithPrecedent/amos) packages. Also, for those using configuration option files, `wonka` is supported by the [bobbie](https://github.com/WithPrecedent/bobbie) project settings library. So, I, and any other maintainers, will do my best to promptly integrate any contributions.
 
 ## Similar Projects
 
 If `wonka` does not fit your needs, you might find one of these other packages helpful. None of them does the same things that `wonka` does (which is why I created this library), but they might fit your particular project needs better.
```

