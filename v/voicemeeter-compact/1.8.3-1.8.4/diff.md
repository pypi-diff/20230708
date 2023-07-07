# Comparing `tmp/voicemeeter_compact-1.8.3.tar.gz` & `tmp/voicemeeter_compact-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicemeeter_compact-1.8.3.tar", max compression
+gzip compressed data, was "voicemeeter_compact-1.8.4.tar", max compression
```

## Comparing `voicemeeter_compact-1.8.3.tar` & `voicemeeter_compact-1.8.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1091 2022-04-11 12:14:57.626259 voicemeeter_compact-1.8.3/LICENSE
--rw-r--r--   0        0        0      730 2023-07-07 02:35:59.201861 voicemeeter_compact-1.8.3/pyproject.toml
--rw-r--r--   0        0        0     6125 2022-09-03 16:03:26.518297 voicemeeter_compact-1.8.3/README.md
--rw-r--r--   0        0        0       51 2022-07-07 14:44:58.582602 voicemeeter_compact-1.8.3/vmcompact/__init__.py
--rw-r--r--   0        0        0     4672 2023-07-01 06:21:50.087433 voicemeeter_compact-1.8.3/vmcompact/app.py
--rw-r--r--   0        0        0     1123 2023-06-24 22:06:19.553026 voicemeeter_compact-1.8.3/vmcompact/banner.py
--rw-r--r--   0        0        0    23309 2023-07-05 22:29:08.031736 voicemeeter_compact-1.8.3/vmcompact/builders.py
--rw-r--r--   0        0        0    10867 2023-07-05 23:06:46.459871 voicemeeter_compact-1.8.3/vmcompact/channels.py
--rw-r--r--   0        0        0     9634 2023-07-05 22:31:26.458658 voicemeeter_compact-1.8.3/vmcompact/config.py
--rw-r--r--   0        0        0     2661 2023-06-29 18:10:03.397989 voicemeeter_compact-1.8.3/vmcompact/configurations.py
--rw-r--r--   0        0        0     2124 2023-06-29 14:29:39.821962 voicemeeter_compact-1.8.3/vmcompact/data.py
--rw-r--r--   0        0        0       86 2023-06-25 11:25:22.327174 voicemeeter_compact-1.8.3/vmcompact/errors.py
--rw-r--r--   0        0        0     8960 2023-06-29 10:16:01.341472 voicemeeter_compact-1.8.3/vmcompact/gainlayer.py
--rw-r--r--   0        0        0   112922 2022-07-01 01:04:51.170192 voicemeeter_compact-1.8.3/vmcompact/img/cat.ico
--rw-r--r--   0        0        0    17812 2023-07-07 02:35:18.760660 voicemeeter_compact-1.8.3/vmcompact/menu.py
--rw-r--r--   0        0        0     3785 2023-06-29 10:52:07.632943 voicemeeter_compact-1.8.3/vmcompact/navigation.py
--rw-r--r--   0        0        0      854 2022-08-02 08:43:15.749028 voicemeeter_compact-1.8.3/vmcompact/subject.py
--rw-r--r--   0        0        0     6909 1970-01-01 00:00:00.000000 voicemeeter_compact-1.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-04-11 12:14:57.626259 voicemeeter_compact-1.8.4/LICENSE
+-rw-r--r--   0        0        0      730 2023-07-07 23:22:00.757305 voicemeeter_compact-1.8.4/pyproject.toml
+-rw-r--r--   0        0        0     6125 2022-09-03 16:03:26.518297 voicemeeter_compact-1.8.4/README.md
+-rw-r--r--   0        0        0       51 2022-07-07 14:44:58.582602 voicemeeter_compact-1.8.4/vmcompact/__init__.py
+-rw-r--r--   0        0        0     4685 2023-07-07 21:33:25.991940 voicemeeter_compact-1.8.4/vmcompact/app.py
+-rw-r--r--   0        0        0     1123 2023-06-24 22:06:19.553026 voicemeeter_compact-1.8.4/vmcompact/banner.py
+-rw-r--r--   0        0        0    23309 2023-07-05 22:29:08.031736 voicemeeter_compact-1.8.4/vmcompact/builders.py
+-rw-r--r--   0        0        0    10867 2023-07-05 23:06:46.459871 voicemeeter_compact-1.8.4/vmcompact/channels.py
+-rw-r--r--   0        0        0     9634 2023-07-05 22:31:26.458658 voicemeeter_compact-1.8.4/vmcompact/config.py
+-rw-r--r--   0        0        0     2835 2023-07-07 21:51:19.065698 voicemeeter_compact-1.8.4/vmcompact/configurations.py
+-rw-r--r--   0        0        0     2124 2023-06-29 14:29:39.821962 voicemeeter_compact-1.8.4/vmcompact/data.py
+-rw-r--r--   0        0        0       86 2023-06-25 11:25:22.327174 voicemeeter_compact-1.8.4/vmcompact/errors.py
+-rw-r--r--   0        0        0     8960 2023-06-29 10:16:01.341472 voicemeeter_compact-1.8.4/vmcompact/gainlayer.py
+-rw-r--r--   0        0        0   112922 2022-07-01 01:04:51.170192 voicemeeter_compact-1.8.4/vmcompact/img/cat.ico
+-rw-r--r--   0        0        0    16815 2023-07-07 17:15:19.541901 voicemeeter_compact-1.8.4/vmcompact/menu.py
+-rw-r--r--   0        0        0     3785 2023-06-29 10:52:07.632943 voicemeeter_compact-1.8.4/vmcompact/navigation.py
+-rw-r--r--   0        0        0      854 2022-08-02 08:43:15.749028 voicemeeter_compact-1.8.4/vmcompact/subject.py
+-rw-r--r--   0        0        0     6909 1970-01-01 00:00:00.000000 voicemeeter_compact-1.8.4/PKG-INFO
```

### Comparing `voicemeeter_compact-1.8.3/LICENSE` & `voicemeeter_compact-1.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.8.3/pyproject.toml` & `voicemeeter_compact-1.8.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "voicemeeter-compact"
-version = "1.8.3"
+version = "1.8.4"
 description = "A Compact Voicemeeter Remote App"
 authors = ["onyx-and-iris <code@onyxandiris.online>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/onyx-and-iris/voicemeeter-compact"
 
 packages = [{ include = "vmcompact" }]
```

### Comparing `voicemeeter_compact-1.8.3/README.md` & `voicemeeter_compact-1.8.4/README.md`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.8.3/vmcompact/app.py` & `voicemeeter_compact-1.8.4/vmcompact/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 
     def stop_drag(self):
         self.drag_id = ""
         _base_values.dragging = False
 
     @cached_property
     def userconfigs(self):
-        self._configs = loader(self.kind.name)
+        self._configs = loader(self.kind.name, self.target)
         return self._configs
 
 
 _apps = {kind.name: App.make(kind) for kind in _kinds_all}
 
 
 def connect(kind_id: str, vmr) -> App:
```

### Comparing `voicemeeter_compact-1.8.3/vmcompact/banner.py` & `voicemeeter_compact-1.8.4/vmcompact/banner.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.8.3/vmcompact/builders.py` & `voicemeeter_compact-1.8.4/vmcompact/builders.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.8.3/vmcompact/channels.py` & `voicemeeter_compact-1.8.4/vmcompact/channels.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.8.3/vmcompact/config.py` & `voicemeeter_compact-1.8.4/vmcompact/config.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.8.3/vmcompact/configurations.py` & `voicemeeter_compact-1.8.4/vmcompact/configurations.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,36 +6,40 @@
 except ModuleNotFoundError:
     import tomli as tomllib
 
 logger = logging.getLogger(__name__)
 
 configuration = {}
 
-configpaths = [
-    Path.cwd() / "configs",
-    Path.home() / ".config" / "vm-compact" / "configs",
-    Path.home() / "Documents" / "Voicemeeter" / "configs",
-]
-for configpath in configpaths:
-    if configpath.is_dir():
-        filepaths = list(configpath.glob("*.toml"))
-        if any(f.stem in ("app", "vban") for f in filepaths):
-            configs = {}
-            for filepath in filepaths:
-                filename = filepath.with_suffix("").stem
-                if filename in ("app", "vban"):
-                    try:
-                        with open(filepath, "rb") as f:
-                            configs[filename] = tomllib.load(f)
-                        logger.info(f"configuration: {filename} loaded into memory")
-                    except tomllib.TOMLDecodeError:
-                        logger.error(f"Invalid TOML config: configs/{filename.stem}")
 
-            configuration |= configs
-            break
+def get_configpath():
+    configpaths = [
+        Path.cwd() / "configs",
+        Path.home() / ".config" / "vm-compact" / "configs",
+        Path.home() / "Documents" / "Voicemeeter" / "configs",
+    ]
+    for configpath in configpaths:
+        if configpath.exists():
+            return configpath
+
+
+if configpath := get_configpath():
+    filepaths = list(configpath.glob("*.toml"))
+    if any(f.stem in ("app", "vban") for f in filepaths):
+        configs = {}
+        for filepath in filepaths:
+            filename = filepath.with_suffix("").stem
+            if filename in ("app", "vban"):
+                try:
+                    with open(filepath, "rb") as f:
+                        configs[filename] = tomllib.load(f)
+                    logger.info(f"configuration: {filename} loaded into memory")
+                except tomllib.TOMLDecodeError:
+                    logger.error(f"Invalid TOML config: configs/{filename.stem}")
+        configuration |= configs
 
 _defaults = {
     "configs": {
         "config": None,
     },
     "theme": {
         "enabled": True,
@@ -71,21 +75,24 @@
 
 
 def get_configuration(key):
     if key in configuration:
         return configuration[key]
 
 
-def loader(kind_id):
-    configs = {}
-    userconfigpath = Path.home() / ".config" / "vm-compact" / "configs" / kind_id
-    if userconfigpath.exists():
-        filepaths = list(userconfigpath.glob("*.toml"))
-        for filepath in filepaths:
-            identifier = filepath.with_suffix("").stem
-            try:
-                with open(filepath, "rb") as f:
-                    configs[identifier] = tomllib.load(f)
-                logger.info(f"loader: {identifier} loaded into memory")
-            except tomllib.TOMLDecodeError:
-                logger.error(f"Invalid TOML config: configs/{filename.stem}")
-    return configs
+def loader(kind_id, target):
+    configs = {"reset": target.configs["reset"]}
+    if configpath := get_configpath():
+        userconfigpath = configpath / kind_id
+        if userconfigpath.exists():
+            filepaths = list(userconfigpath.glob("*.toml"))
+            for filepath in filepaths:
+                identifier = filepath.with_suffix("").stem
+                try:
+                    with open(filepath, "rb") as f:
+                        configs[identifier] = tomllib.load(f)
+                    logger.info(f"loader: {identifier} loaded into memory")
+                except tomllib.TOMLDecodeError:
+                    logger.error(f"Invalid TOML config: configs/{filename.stem}")
+
+    target.configs = configs
+    return target.configs
```

### Comparing `voicemeeter_compact-1.8.3/vmcompact/data.py` & `voicemeeter_compact-1.8.4/vmcompact/data.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.8.3/vmcompact/gainlayer.py` & `voicemeeter_compact-1.8.4/vmcompact/gainlayer.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.8.3/vmcompact/img/cat.ico` & `voicemeeter_compact-1.8.4/vmcompact/img/cat.ico`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.8.3/vmcompact/menu.py` & `voicemeeter_compact-1.8.4/vmcompact/menu.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,32 +81,24 @@
 
         # configs menu
         self.menu_configs = tk.Menu(self, tearoff=0)
         self.add_cascade(menu=self.menu_configs, label="Configs")
         self.menu_configs_load = tk.Menu(self.menu_configs, tearoff=0)
         self.menu_configs.add_cascade(menu=self.menu_configs_load, label="Load config")
         self.config_defaults = {"reset"}
-        if len(self.target.configs) > len(self.config_defaults) and all(
-            key in self.target.configs for key in self.config_defaults
+        if len(self.parent.userconfigs) > len(self.config_defaults) and all(
+            key in self.parent.userconfigs for key in self.config_defaults
         ):
             [
                 self.menu_configs_load.add_command(
                     label=profile, command=partial(self.load_profile, profile)
                 )
-                for profile in self.target.configs.keys()
+                for profile in self.parent.userconfigs.keys()
                 if profile not in self.config_defaults
             ]
-        elif self.parent.userconfigs:
-            [
-                self.menu_configs_load.add_command(
-                    label=name, command=partial(self.load_custom_profile, data)
-                )
-                for name, data in self.parent.userconfigs.items()
-                if name not in self.config_defaults
-            ]
         else:
             self.menu_configs.entryconfig(0, state="disabled")
         self.menu_configs.add_command(
             label="Reset to defaults", command=self.load_defaults
         )
 
         # layout menu
@@ -311,55 +303,36 @@
         ]
         self.logger.info(
             f"Finished loading theme Sunvalley {sv_ttk.get_theme().capitalize()} theme"
         )
 
     def menu_teardown(self, i):
         # remove config load menus
-        removed = []
-        for key in self.target.configs.keys():
-            if key not in self.config_defaults:
-                try:
-                    self.menu_configs_load.delete(key)
-                    removed.append(key)
-                except tk._tkinter.tclError as e:
-                    self.logger.warning(f"{type(e).__name__}: {e}")
-
-        for key in self.parent.userconfigs.keys():
-            if key not in self.config_defaults and key not in removed:
-                try:
-                    self.menu_configs_load.delete(key)
-                except tk._tkinter.tclError as e:
-                    self.logger.warning(f"{type(e).__name__}: {e}")
+        if len(self.parent.userconfigs) > len(self.config_defaults):
+            for profile in self.parent.userconfigs:
+                if profile not in self.config_defaults:
+                    try:
+                        self.menu_configs_load.delete(profile)
+                    except tk._tkinter.tclError as e:
+                        self.logger.warning(f"{type(e).__name__}: {e}")
 
         [
             self.menu_vban.entryconfig(j, state="disabled")
             for j, _ in enumerate(self.menu_vban.winfo_children())
             if j != i
         ]
 
     def menu_setup(self):
-        if len(self.target.configs) > len(self.config_defaults) and all(
-            key in self.target.configs for key in self.config_defaults
-        ):
-            [
-                self.menu_configs_load.add_command(
-                    label=profile, command=partial(self.load_profile, profile)
-                )
-                for profile in self.target.configs.keys()
-                if profile not in self.config_defaults
-            ]
-        elif self.parent.userconfigs:
-            [
-                self.menu_configs_load.add_command(
-                    label=name, command=partial(self.load_custom_profile, data)
-                )
-                for name, data in self.parent.userconfigs.items()
-                if name not in self.config_defaults
-            ]
+        if len(self.parent.userconfigs) > len(self.config_defaults):
+            for profile in self.parent.userconfigs:
+                if profile not in self.config_defaults:
+                    self.menu_configs_load.add_command(
+                        label=profile, command=partial(self.load_profile, profile)
+                    )
+                    self.menu_configs.entryconfig(0, state="normal")
         else:
             self.menu_configs.entryconfig(0, state="disabled")
 
     def toggle_navigation(self, cmd=None):
         if cmd == "show":
             self.logger.debug("show navframe")
             self.parent.nav_frame.grid()
```

### Comparing `voicemeeter_compact-1.8.3/vmcompact/navigation.py` & `voicemeeter_compact-1.8.4/vmcompact/navigation.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.8.3/vmcompact/subject.py` & `voicemeeter_compact-1.8.4/vmcompact/subject.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.8.3/PKG-INFO` & `voicemeeter_compact-1.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicemeeter-compact
-Version: 1.8.3
+Version: 1.8.4
 Summary: A Compact Voicemeeter Remote App
 Home-page: https://github.com/onyx-and-iris/voicemeeter-compact
 License: MIT
 Author: onyx-and-iris
 Author-email: code@onyxandiris.online
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

