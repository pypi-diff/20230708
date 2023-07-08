# Comparing `tmp/pyTasker-0.6.1.tar.gz` & `tmp/pyTasker-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyTasker-0.6.1.tar", last modified: Sun Jul 10 15:58:12 2022, max compression
+gzip compressed data, was "pyTasker-0.6.2.tar", last modified: Sat Jul  8 17:41:26 2023, max compression
```

## Comparing `pyTasker-0.6.1.tar` & `pyTasker-0.6.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2022-07-10 15:58:12.232014 pyTasker-0.6.1/
--rw-rw-rw-   0        0        0      304 2022-07-10 15:44:12.000000 pyTasker-0.6.1/.gitignore
--rw-rw-rw-   0        0        0     1115 2022-03-07 21:04:39.000000 pyTasker-0.6.1/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0      733 2022-03-07 21:04:39.000000 pyTasker-0.6.1/CHANGELOG.md
--rw-rw-rw-   0        0        0    35746 2022-02-03 21:25:58.000000 pyTasker-0.6.1/LICENSE
--rw-rw-rw-   0        0        0     7532 2022-07-10 15:58:12.233016 pyTasker-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     6460 2022-04-25 12:50:19.000000 pyTasker-0.6.1/README.md
-drwxrwxrwx   0        0        0        0 2022-07-10 15:58:12.208015 pyTasker-0.6.1/Tasker/
--rw-rw-rw-   0        0        0      569 2022-07-10 15:44:14.000000 pyTasker-0.6.1/Tasker/__init__.py
--rw-rw-rw-   0        0        0     3088 2022-07-10 15:21:35.000000 pyTasker-0.6.1/Tasker/__main__.py
--rw-rw-rw-   0        0        0       23 2022-07-10 15:56:27.000000 pyTasker-0.6.1/Tasker/__version__.py
--rw-rw-rw-   0        0        0     3393 2022-07-10 15:45:31.000000 pyTasker-0.6.1/Tasker/cli.py
--rw-rw-rw-   0        0        0     2712 2022-07-10 12:16:33.000000 pyTasker-0.6.1/Tasker/common.py
--rw-rw-rw-   0        0        0     2578 2022-03-07 21:04:39.000000 pyTasker-0.6.1/Tasker/inspector.py
--rw-rw-rw-   0        0        0    15270 2022-07-10 12:01:07.000000 pyTasker-0.6.1/Tasker/operations.py
--rw-rw-rw-   0        0        0    22627 2022-07-10 15:22:54.000000 pyTasker-0.6.1/Tasker/parser.py
--rw-rw-rw-   0        0        0     1315 2022-03-07 21:04:39.000000 pyTasker-0.6.1/Tasker/parser_test.py
--rw-rw-rw-   0        0        0    17710 2022-07-10 15:36:25.000000 pyTasker-0.6.1/Tasker/templater.py
--rw-rw-rw-   0        0        0     6966 2022-07-10 12:35:40.000000 pyTasker-0.6.1/Tasker/types.py
-drwxrwxrwx   0        0        0        0 2022-07-10 15:58:12.229015 pyTasker-0.6.1/pyTasker.egg-info/
--rw-rw-rw-   0        0        0     7532 2022-07-10 15:58:11.000000 pyTasker-0.6.1/pyTasker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      568 2022-07-10 15:58:12.000000 pyTasker-0.6.1/pyTasker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-10 15:58:11.000000 pyTasker-0.6.1/pyTasker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2022-07-10 15:58:11.000000 pyTasker-0.6.1/pyTasker.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       58 2022-07-10 15:58:11.000000 pyTasker-0.6.1/pyTasker.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-07-10 15:58:11.000000 pyTasker-0.6.1/pyTasker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      268 2022-03-07 21:04:39.000000 pyTasker-0.6.1/pyproject.toml
--rw-rw-rw-   0        0        0      113 2022-04-23 19:46:13.000000 pyTasker-0.6.1/requirements.txt
--rw-rw-rw-   0        0        0      186 2022-07-10 15:58:12.234015 pyTasker-0.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1787 2022-07-10 15:56:27.000000 pyTasker-0.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-10 15:58:12.231015 pyTasker-0.6.1/static/
--rw-rw-rw-   0        0        0   424108 2022-02-03 21:25:58.000000 pyTasker-0.6.1/static/Copy PDFs then zip.png
--rw-rw-rw-   0        0        0   136520 2022-02-03 21:25:58.000000 pyTasker-0.6.1/static/Copy PDFs.png
+drwxrwxrwx   0        0        0        0 2023-07-08 17:41:26.703878 pyTasker-0.6.2/
+-rw-rw-rw-   0        0        0      305 2023-07-08 17:38:54.000000 pyTasker-0.6.2/.gitignore
+-rw-rw-rw-   0        0        0     1115 2022-03-07 21:04:39.000000 pyTasker-0.6.2/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0      733 2022-03-07 21:04:39.000000 pyTasker-0.6.2/CHANGELOG.md
+-rw-rw-rw-   0        0        0    35746 2022-02-03 21:25:58.000000 pyTasker-0.6.2/LICENSE
+-rw-rw-rw-   0        0        0     7532 2023-07-08 17:41:26.704880 pyTasker-0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6460 2023-07-08 17:38:54.000000 pyTasker-0.6.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 17:41:26.687873 pyTasker-0.6.2/Tasker/
+-rw-rw-rw-   0        0        0      569 2023-07-08 17:38:54.000000 pyTasker-0.6.2/Tasker/__init__.py
+-rw-rw-rw-   0        0        0     3109 2023-07-08 17:38:54.000000 pyTasker-0.6.2/Tasker/__main__.py
+-rw-rw-rw-   0        0        0       23 2023-07-08 17:40:40.000000 pyTasker-0.6.2/Tasker/__version__.py
+-rw-rw-rw-   0        0        0     3554 2023-07-08 17:38:54.000000 pyTasker-0.6.2/Tasker/cli.py
+-rw-rw-rw-   0        0        0     2712 2023-07-08 17:38:54.000000 pyTasker-0.6.2/Tasker/common.py
+-rw-rw-rw-   0        0        0     2578 2022-03-07 21:04:39.000000 pyTasker-0.6.2/Tasker/inspector.py
+-rw-rw-rw-   0        0        0    15270 2023-07-08 17:38:54.000000 pyTasker-0.6.2/Tasker/operations.py
+-rw-rw-rw-   0        0        0    27172 2023-07-08 17:38:54.000000 pyTasker-0.6.2/Tasker/parser.py
+-rw-rw-rw-   0        0        0     1315 2022-03-07 21:04:39.000000 pyTasker-0.6.2/Tasker/parser_test.py
+-rw-rw-rw-   0        0        0    17710 2023-07-08 17:38:54.000000 pyTasker-0.6.2/Tasker/templater.py
+-rw-rw-rw-   0        0        0     6966 2023-07-08 17:38:54.000000 pyTasker-0.6.2/Tasker/types.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:41:26.698878 pyTasker-0.6.2/pyTasker.egg-info/
+-rw-rw-rw-   0        0        0     7532 2023-07-08 17:41:26.000000 pyTasker-0.6.2/pyTasker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      568 2023-07-08 17:41:26.000000 pyTasker-0.6.2/pyTasker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 17:41:26.000000 pyTasker-0.6.2/pyTasker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-08 17:41:26.000000 pyTasker-0.6.2/pyTasker.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       58 2023-07-08 17:41:26.000000 pyTasker-0.6.2/pyTasker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-08 17:41:26.000000 pyTasker-0.6.2/pyTasker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      268 2022-03-07 21:04:39.000000 pyTasker-0.6.2/pyproject.toml
+-rw-rw-rw-   0        0        0      113 2023-07-08 17:38:54.000000 pyTasker-0.6.2/requirements.txt
+-rw-rw-rw-   0        0        0      191 2023-07-08 17:41:26.705876 pyTasker-0.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     1787 2023-07-08 17:40:40.000000 pyTasker-0.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:41:26.702882 pyTasker-0.6.2/static/
+-rw-rw-rw-   0        0        0   424108 2022-02-03 21:25:58.000000 pyTasker-0.6.2/static/Copy PDFs then zip.png
+-rw-rw-rw-   0        0        0   136520 2022-02-03 21:25:58.000000 pyTasker-0.6.2/static/Copy PDFs.png
```

### Comparing `pyTasker-0.6.1/.pre-commit-config.yaml` & `pyTasker-0.6.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.1/CHANGELOG.md` & `pyTasker-0.6.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.1/LICENSE` & `pyTasker-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.1/PKG-INFO` & `pyTasker-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTasker
-Version: 0.6.1
+Version: 0.6.2
 Summary: Run pipelines on your own computer for better automation
 Home-page: https://github.com/carlossilva2/pyTasker
 Author: Carlos Silva
 Author-email: carlos.miguel.silva@protonmail.com
 License: GPLv3
 Project-URL: Source, https://github.com/carlossilva2/pyTasker
 Project-URL: Documentation, https://cmsilva.gitbook.io/pytasker/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyTasker Version: 0.6.1 Summary: Run pipelines on
+Metadata-Version: 2.1 Name: pyTasker Version: 0.6.2 Summary: Run pipelines on
 your own computer for better automation Home-page: https://github.com/
 carlossilva2/pyTasker Author: Carlos Silva Author-email:
 carlos.miguel.silva@protonmail.com License: GPLv3 Project-URL: Source, https://
 github.com/carlossilva2/pyTasker Project-URL: Documentation, https://
 cmsilva.gitbook.io/pytasker/ Platform: UNKNOWN Classifier: Development Status
 :: 4 - Beta Classifier: Environment :: Console Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: GNU General Public License v3
```

### Comparing `pyTasker-0.6.1/README.md` & `pyTasker-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.1/Tasker/__init__.py` & `pyTasker-0.6.2/Tasker/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.1/Tasker/__main__.py` & `pyTasker-0.6.2/Tasker/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             )
         else:
             logger.error("Path and Name flags are required when creating Aliases")
     elif args.action == "install":
         if args.Extension is None:
             logger.error("Missing Extension flag `-e`. Check Help for command syntax")
             sys.exit(1)
-        Parser.install_remote_extension(args.Extension, logger)
+        Parser.install_remote_extension(args.Extension, logger, upgrade=args.Update)
     elif args.action == "uninstall":
         if args.Extension is None:
             logger.error("Missing Extension flag `-e`. Check Help for command syntax")
             sys.exit(1)
         Parser.uninstall_extension(args.Extension, logger)
     elif args.action == "remote-search" or args.action == "remote-list":
         if args.action == "remote-search":
```

### Comparing `pyTasker-0.6.1/Tasker/cli.py` & `pyTasker-0.6.2/Tasker/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,14 +107,20 @@
     )
     options.add_argument(
         "-no",
         "--No-Output",
         action="store_true",
         help="Disables normal logging, only shows Warnings and Errors.",
     )
+    options.add_argument(
+        "-u",
+        "--Update",
+        action="store_true",
+        help="Indicates that Extension should be updated.",
+    )
     args = parser.parse_args()
     if args.No_Warning:
         env["-No-Warning"] = "1"
     if args.No_Rollback:
         env["-No-Rollback"] = "1"
     if args.No_Output:
         logger.setLevel(logging.WARNING)
```

### Comparing `pyTasker-0.6.1/Tasker/common.py` & `pyTasker-0.6.2/Tasker/common.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.1/Tasker/inspector.py` & `pyTasker-0.6.2/Tasker/inspector.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.1/Tasker/operations.py` & `pyTasker-0.6.2/Tasker/operations.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.1/Tasker/parser.py` & `pyTasker-0.6.2/Tasker/parser.py`

 * *Files 11% similar despite different names*

```diff
@@ -411,14 +411,20 @@
         Parser.do_config()
         return [
             _.replace(".tasker.json", "")
             for _ in os.listdir(f"{Path.expanduser('~')}/.tasker/Tasks")
         ]
 
     @staticmethod
+    def get_task_descriptor(task: str) -> Task:
+        return json.load(
+            open(f"{Path.expanduser('~')}/.tasker/Tasks/{task}.tasker.json", "r")
+        )
+
+    @staticmethod
     def create_new_task(file_name: str, name: str, description: str) -> InstructionSet:
         Parser.do_config()
         i: InstructionSet = InstructionSet(name=name, description=description, tasks=[])
         with open(
             f"{Path.expanduser('~')}/.tasker/Tasks/{file_name}.tasker.json", "w"
         ) as instruction_set:
             json.dump(i, instruction_set, indent=4)
@@ -444,14 +450,15 @@
                 ex.close()
             j: Settings = json.load(open(f"{root}/.tasker/config.json"))
             j["extensions"].append(
                 {
                     "name": name,
                     "file": f_name,
                     "path": f"{root}/.tasker/Templates/{f_name}",
+                    "version": 0,
                 }
             )
             json.dump(j, open(f"{root}/.tasker/config.json", "w"), indent=4)
             template.close()
 
     @staticmethod
     def add_alias(alias: Alias, logger: Logger) -> None:
@@ -462,56 +469,164 @@
             if alias["name"] == _alias["name"]:
                 logger.error("An Alias with that name already exists")
                 sys.exit(1)
         settings["alias"].append(alias)
         json.dump(settings, open(f"{root}/.tasker/config.json", "w"), indent=4)
 
     @staticmethod
-    def install_remote_extension(extension: str, logger: Logger) -> bool:
+    def install_remote_extension(
+        extension: str, logger: Logger, upgrade: bool = False
+    ) -> bool:
+        def install(context: dict, extension: str, logger: Logger) -> bool:
+            # Check if extension is allowed on Current OS
+            os = platform.system()
+            if (
+                context[extension]["platform"] != os
+                and context[extension]["platform"] != "*"
+            ):
+                logger.error(f"Extension cannot be installed in '{os}'")
+                return False
+            # Check for extension dependencies
+            existing_modules = pip_freeze()
+            for dep in context[extension]["dependencies"]:
+                if dep not in existing_modules:
+                    pip(dep)
+            # Retrieve Template
+            template = get(context[extension]["extension"]).text
+            # Install Extension locally
+            _n = md5(f"{time()}_{extension}".encode("UTF-8")).hexdigest()[:10]
+            f_name = f"extension_{_n}.py"
+            with open(f"{root}/.tasker/Templates/{f_name}", "w") as ex:
+                ex.write(template)
+                ex.close()
+            j["extensions"].append(
+                {
+                    "name": extension,
+                    "description": context[extension]["description"],
+                    "file": f_name,
+                    "path": f"{root}/.tasker/Templates/{f_name}",
+                    "version": context[extension]["version"],
+                }
+            )
+            json.dump(j, open(f"{root}/.tasker/config.json", "w"), indent=4)
+            return True
+
         Parser.do_config()
         root = Path.expanduser("~")
         # Remove DEBUG WARNINGS
         getLogger("requests").setLevel(WARNING)
         getLogger("urllib3").setLevel(WARNING)
+        j: Settings = json.load(open(f"{root}/.tasker/config.json"))
+        index = None
+        for i, ex in enumerate(j["extensions"]):
+            if ex["name"] == extension:
+                index = i
+                break
+        # Check if extension is already installed
+        if (
+            index != None
+            and extension in [_["name"] for _ in j["extensions"]]
+            and upgrade is False
+        ):
+            logger.error("Extension already installed")
+            return False
         # Get Context file
         context = get(
             "https://raw.githubusercontent.com/carlossilva2/pyTasker-actions/main/context.json"
         ).json()
         # Check if extension exists on remote
         if extension not in context.keys():
             logger.error("Extension does not exist. Check spelling")
             return False
-        # Check if extension is allowed on Current OS
-        os = platform.system()
-        if context[extension]["platform"] != os and context[extension]["platform"] != "*":
-            logger.error(f"Extension cannot be installed in '{os}'")
-            return False
-        # Check for extension dependencies
-        existing_modules = pip_freeze()
-        for dep in context[extension]["dependencies"]:
-            if dep not in existing_modules:
-                pip(dep)
-        # Retrieve Template
-        template = get(context[extension]["extension"]).text
-        # Install Extension locally
-        _n = md5(f"{time()}_{extension}".encode("UTF-8")).hexdigest()[:10]
-        f_name = f"extension_{_n}.py"
-        with open(f"{root}/.tasker/Templates/{f_name}", "w") as ex:
-            ex.write(template)
-            ex.close()
+        # Check for update
+        if (
+            index != None
+            and j["extensions"][index]["version"] == context[extension]["version"]
+            and upgrade
+        ):
+            logger.debug("Already up to date")
+            return True
+        if (
+            index != None
+            and j["extensions"][index]["version"] < context[extension]["version"]
+            and upgrade
+        ):
+            logger.debug(f"Updating '{extension}'....")
+            Parser.uninstall_extension(extension, logger)
+            return install(context, extension, logger)
+        else:
+            return install(context, extension, logger)
+
+    @staticmethod
+    def install_local_extension(descriptor: dict, logger: Logger, upgrade: bool = False):
+        def install(context: dict, logger: Logger) -> bool:
+            # Check if extension is allowed on Current OS
+            os = platform.system()
+            if context["platform"] != os and context["platform"] != "*":
+                logger.error(f"Extension cannot be installed in '{os}'")
+                return False
+            # Check for extension dependencies
+            existing_modules = pip_freeze()
+            for dep in context["dependencies"]:
+                if dep not in existing_modules:
+                    pip(dep)
+            # Retrieve Template
+            template = context["extension"]
+            # Install Extension locally
+            _n = md5(f"{time()}_{context['name']}".encode("UTF-8")).hexdigest()[:10]
+            f_name = f"extension_{_n}.py"
+            with open(f"{root}/.tasker/Templates/{f_name}", "w") as ex:
+                ex.write(template)
+                ex.close()
+            j["extensions"].append(
+                {
+                    "name": context["name"],
+                    "file": f_name,
+                    "description": context["description"],
+                    "path": f"{root}/.tasker/Templates/{f_name}",
+                    "version": context["version"],
+                }
+            )
+            json.dump(j, open(f"{root}/.tasker/config.json", "w"), indent=4)
+            return True
+
+        Parser.do_config()
+        root = Path.expanduser("~")
         j: Settings = json.load(open(f"{root}/.tasker/config.json"))
-        j["extensions"].append(
-            {
-                "name": extension,
-                "file": f_name,
-                "path": f"{root}/.tasker/Templates/{f_name}",
-            }
-        )
-        json.dump(j, open(f"{root}/.tasker/config.json", "w"), indent=4)
-        return True
+        index = None
+        for i, ex in enumerate(j["extensions"]):
+            if ex["name"] == descriptor["name"]:
+                index = i
+                break
+        # Check if extension is already installed
+        if (
+            index != None
+            and descriptor["name"] in [_["name"] for _ in j["extensions"]]
+            and upgrade is False
+        ):
+            logger.error("Extension already installed")
+            return False
+        # Check for update
+        if (
+            index != None
+            and j["extensions"][index]["version"] == descriptor["version"]
+            and upgrade
+        ):
+            logger.debug("Already up to date")
+            return True
+        if (
+            index != None
+            and j["extensions"][index]["version"] < descriptor["version"]
+            and upgrade
+        ):
+            logger.debug(f"Updating '{descriptor['name']}'....")
+            Parser.uninstall_extension(descriptor["name"], logger)
+            return install(descriptor, logger)
+        else:
+            return install(descriptor, logger)
 
     @staticmethod
     def uninstall_extension(extension: str, logger: Logger) -> None:
         Parser.do_config()
         root = Path.expanduser("~")
         j: Settings = json.load(open(f"{root}/.tasker/config.json"))
         if extension not in [_["name"] for _ in j["extensions"]]:
@@ -551,7 +666,8 @@
         getLogger("urllib3").setLevel(WARNING)
         # Get Context file
         context = get(
             "https://raw.githubusercontent.com/carlossilva2/pyTasker-actions/main/context.json"
         ).json()
         for extension in context.keys():
             logger.debug(f"{extension}=={context[extension]['version']}")
+        return context
```

### Comparing `pyTasker-0.6.1/Tasker/parser_test.py` & `pyTasker-0.6.2/Tasker/parser_test.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.1/Tasker/templater.py` & `pyTasker-0.6.2/Tasker/templater.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.1/Tasker/types.py` & `pyTasker-0.6.2/Tasker/types.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.1/pyTasker.egg-info/PKG-INFO` & `pyTasker-0.6.2/pyTasker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTasker
-Version: 0.6.1
+Version: 0.6.2
 Summary: Run pipelines on your own computer for better automation
 Home-page: https://github.com/carlossilva2/pyTasker
 Author: Carlos Silva
 Author-email: carlos.miguel.silva@protonmail.com
 License: GPLv3
 Project-URL: Source, https://github.com/carlossilva2/pyTasker
 Project-URL: Documentation, https://cmsilva.gitbook.io/pytasker/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyTasker Version: 0.6.1 Summary: Run pipelines on
+Metadata-Version: 2.1 Name: pyTasker Version: 0.6.2 Summary: Run pipelines on
 your own computer for better automation Home-page: https://github.com/
 carlossilva2/pyTasker Author: Carlos Silva Author-email:
 carlos.miguel.silva@protonmail.com License: GPLv3 Project-URL: Source, https://
 github.com/carlossilva2/pyTasker Project-URL: Documentation, https://
 cmsilva.gitbook.io/pytasker/ Platform: UNKNOWN Classifier: Development Status
 :: 4 - Beta Classifier: Environment :: Console Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: GNU General Public License v3
```

### Comparing `pyTasker-0.6.1/pyTasker.egg-info/SOURCES.txt` & `pyTasker-0.6.2/pyTasker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.1/setup.py` & `pyTasker-0.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 setup(
     author="Carlos Silva",
     author_email="carlos.miguel.silva@protonmail.com",
     name="pyTasker",
     description="Run pipelines on your own computer for better automation",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.6.1",
+    version="0.6.2",
     url="https://github.com/carlossilva2/pyTasker",
     packages=find_packages(),
     license="GPLv3",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Developers",
```

### Comparing `pyTasker-0.6.1/static/Copy PDFs then zip.png` & `pyTasker-0.6.2/static/Copy PDFs then zip.png`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.1/static/Copy PDFs.png` & `pyTasker-0.6.2/static/Copy PDFs.png`

 * *Files identical despite different names*

