# Comparing `tmp/impose-cli-0.0.41.tar.gz` & `tmp/impose-cli-0.1.41rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impose-cli-0.0.41.tar", last modified: Tue May  9 07:23:08 2023, max compression
+gzip compressed data, was "impose-cli-0.1.41rc0.tar", last modified: Sat Jul  8 14:28:30 2023, max compression
```

## Comparing `impose-cli-0.0.41.tar` & `impose-cli-0.1.41rc0.tar`

### file list

```diff
@@ -1,18 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:23:08.171020 impose-cli-0.0.41/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-09 07:22:48.000000 impose-cli-0.0.41/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-09 07:23:08.171020 impose-cli-0.0.41/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-09 07:22:48.000000 impose-cli-0.0.41/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:23:08.171020 impose-cli-0.0.41/impose_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-09 07:22:48.000000 impose-cli-0.0.41/impose_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-09 07:22:48.000000 impose-cli-0.0.41/impose_cli/impose_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:23:08.171020 impose-cli-0.0.41/impose_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-09 07:23:07.000000 impose-cli-0.0.41/impose_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-09 07:23:08.000000 impose-cli-0.0.41/impose_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 07:23:07.000000 impose-cli-0.0.41/impose_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-09 07:23:07.000000 impose-cli-0.0.41/impose_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-09 07:23:07.000000 impose-cli-0.0.41/impose_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 07:23:08.171020 impose-cli-0.0.41/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-09 07:22:48.000000 impose-cli-0.0.41/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:23:08.171020 impose-cli-0.0.41/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:22:48.000000 impose-cli-0.0.41/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-09 07:22:48.000000 impose-cli-0.0.41/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:28:30.783914 impose-cli-0.1.41rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-08 14:28:08.000000 impose-cli-0.1.41rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-08 14:28:30.779914 impose-cli-0.1.41rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-08 14:28:08.000000 impose-cli-0.1.41rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:28:30.779914 impose-cli-0.1.41rc0/impose_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 14:28:08.000000 impose-cli-0.1.41rc0/impose_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-07-08 14:28:08.000000 impose-cli-0.1.41rc0/impose_cli/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-08 14:28:08.000000 impose-cli-0.1.41rc0/impose_cli/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 14:28:08.000000 impose-cli-0.1.41rc0/impose_cli/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-08 14:28:08.000000 impose-cli-0.1.41rc0/impose_cli/impose_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-07-08 14:28:08.000000 impose-cli-0.1.41rc0/impose_cli/impose_cli_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-08 14:28:08.000000 impose-cli-0.1.41rc0/impose_cli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:28:30.779914 impose-cli-0.1.41rc0/impose_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-08 14:28:30.000000 impose-cli-0.1.41rc0/impose_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-08 14:28:30.000000 impose-cli-0.1.41rc0/impose_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 14:28:30.000000 impose-cli-0.1.41rc0/impose_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-08 14:28:30.000000 impose-cli-0.1.41rc0/impose_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-08 14:28:30.000000 impose-cli-0.1.41rc0/impose_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 14:28:30.783914 impose-cli-0.1.41rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-08 14:28:08.000000 impose-cli-0.1.41rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:28:30.779914 impose-cli-0.1.41rc0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 14:28:08.000000 impose-cli-0.1.41rc0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-08 14:28:08.000000 impose-cli-0.1.41rc0/tests/test.py
```

### Comparing `impose-cli-0.0.41/LICENSE` & `impose-cli-0.1.41rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `impose-cli-0.0.41/impose_cli/impose_cli.py` & `impose-cli-0.1.41rc0/impose_cli/impose_cli_2.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,98 +3,100 @@
 from importlib.util import spec_from_file_location, module_from_spec
 from inspect import getframeinfo, currentframe
 from inspect import Parameter, signature as sig
 from os import listdir
 from os.path import exists, join, dirname, abspath
 
 
-def impose(func):
-    return func
+# def impose(func):
+#     return func
 
 
 def expose(func: click.Group):
     func()
 
 
-def impose_cli(execute: bool = True, target: [str, None] = None) -> None:
-    """
-    If target is a directory, then each file will be a group and all functions will be a command
-    If medium is a file, then there will be no group and all functions will be a command
-    :param target:
-    :return:
-    """
-
-    class ImposeFunctionVisitor(ast.NodeVisitor):
-        def __init__(self):
-            self.imposed_functions = []
-
-        def visit_FunctionDef(self, node):
-            if hasattr(node, 'decorator_list'):
-                for decorator in node.decorator_list:
-                    if isinstance(decorator, ast.Name) and decorator.id == 'impose':
-                        self.imposed_functions.append(node.name)
-
-    def find_imposed_functions(filename):
-        with open(filename, 'r') as file:
-            file_contents = file.read()
-        module = ast.parse(file_contents)
-        visitor = ImposeFunctionVisitor()
-        visitor.visit(module)
-        return visitor.imposed_functions
-
+def impose_cli(target: [str, None] = None, return_before_executing: bool = False):
+    # """
+    # If target is a directory, then each file will be a group and all functions will be a command
+    # If medium is a file, then there will be no group and all functions will be a command
+    # :param return_before_executing: Allows you to return the Click group without executing it.
+    # :param target: Allows you to run the commands on a directory.
+    # :return:
+    # """
+    #
+    # class ImposeFunctionVisitor(ast.NodeVisitor):
+    #     def __init__(self):
+    #         self.imposed_functions = []
+    #
+    #     def visit_FunctionDef(self, node):
+    #         if hasattr(node, 'decorator_list'):
+    #             for decorator in node.decorator_list:
+    #                 if isinstance(decorator, ast.Name) and decorator.id == 'impose':
+    #                     self.imposed_functions.append(node.name)
+    #
+    # def find_imposed_functions(filename):
+    #     with open(filename, 'r') as file:
+    #         file_contents = file.read()
+    #     module = ast.parse(file_contents)
+    #     visitor = ImposeFunctionVisitor()
+    #     visitor.visit(module)
+    #     return visitor.imposed_functions
+    #
     def find_files(origin, target):
         if target is None:
             return [origin]
 
         else:
             directory = join(dirname(origin), target)
             if not exists(directory):
                 raise FileNotFoundError(f"There is no directory {directory}.")
 
             dirs = [x for x in listdir(directory) if x.endswith('.py')]
             return [abspath(join(directory, f)) for f in dirs]
+    #
 
     def load_module_from_file(file_path, module_name):
         spec = spec_from_file_location(module_name, file_path)
         module = module_from_spec(spec)
         spec.loader.exec_module(module)
         return module
-
-    def analyze_functions(module, function):
-        signature = sig(getattr(module, function))
-        parameters = signature.parameters
-        args_with_defaults = [[p.name, p.default, p.annotation if p.annotation.__name__ != '_empty' else None] for p in
-                              parameters.values() if p.default != Parameter.empty]
-        args_without_defaults = [[p.name, p.annotation if p.annotation.__name__ != '_empty' else None] for p in
-                                 parameters.values() if p.default == Parameter.empty and p.default is not None]
-        return args_without_defaults, args_with_defaults
-
-    def create_dynamic_group(group_name, command_list):
-        dynamic_group = click.Group(name=group_name)
-
-        for cmd in command_list:
-            dynamic_command = click.Command(name=cmd['name'].replace('_', '-'), callback=cmd['callback'])
-
-            for arg in cmd['arguments']:
-                arg_name = arg[0].replace('_', '-')
-                if arg[1] is not None:
-                    dynamic_command.params.append(click.Argument((arg_name,), type=arg[1]))
-                else:
-                    dynamic_command.params.append(click.Argument((arg_name,)))
-
-            for opt in cmd['options']:
-                opt_name = opt[0].replace('_', '-')
-                if opt[2] is not None:
-                    dynamic_command.params.append(click.Option((f"--{opt_name}",), default=opt[1], type=opt[2]))
-                else:
-                    dynamic_command.params.append(click.Option((f"--{opt_name}",), default=opt[2]))
-
-            dynamic_group.add_command(dynamic_command)
-
-        return dynamic_group
+    #
+    # def analyze_functions(module, function):
+    #     signature = sig(getattr(module, function))
+    #     parameters = signature.parameters
+    #     args_with_defaults = [[p.name, p.default, p.annotation if p.annotation.__name__ != '_empty' else None] for p in
+    #                           parameters.values() if p.default != Parameter.empty]
+    #     args_without_defaults = [[p.name, p.annotation if p.annotation.__name__ != '_empty' else None] for p in
+    #                              parameters.values() if p.default == Parameter.empty and p.default is not None]
+    #     return args_without_defaults, args_with_defaults
+    #
+    # def create_dynamic_group(group_name, command_list):
+    #     dynamic_group = click.Group(name=group_name)
+    #
+    #     for cdmd in command_list:
+    #         dynamic_command = click.Command(name=cmd['name'].replace('_', '-'), callback=cmd['callback'])
+    #
+    #         for arg in cmd['arguments']:
+    #             arg_name = arg[0].replace('_', '-')
+    #             if arg[1] is not None:
+    #                 dynamic_command.params.append(click.Argument((arg_name,), type=arg[1]))
+    #             else:
+    #                 dynamic_command.params.append(click.Argument((arg_name,)))
+    #
+    #         for opt in cmd['options']:
+    #             opt_name = opt[0].replace('_', '-')
+    #             if opt[2] is not None:
+    #                 dynamic_command.params.append(click.Option((f"--{opt_name}",), default=opt[1], type=opt[2]))
+    #             else:
+    #                 dynamic_command.params.append(click.Option((f"--{opt_name}",), default=opt[2]))
+    #
+    #         dynamic_group.add_command(dynamic_command)
+    #
+    #     return dynamic_group
 
     origin_files = find_files(getframeinfo(currentframe().f_back)[0], target)
 
     meta = {}
     for origin_file in origin_files:
         module_name = origin_file.split('/')[-1].replace('.py', '')
         meta[module_name] = []
@@ -104,20 +106,21 @@
             args, opts = analyze_functions(module, function)
             meta[module_name].append({
                 "name": function,
                 "arguments": args,
                 "options": opts,
                 "callback": getattr(module, function)
             })
+    return None
 
-    if target is not None:
-        main_group = create_dynamic_group('cli', [])
-        keys = meta.keys()
-        for key in keys:
-            main_group.add_command(create_dynamic_group(key, meta[key]))
-    else:
-        main_group = create_dynamic_group('cli', meta[list(meta.keys())[0]])
-
-    if execute:
-        main_group()
-    else:
-        return main_group
+    # if target is not None:
+    #     main_group = create_dynamic_group('cli', [])
+    #     keys = meta.keys()
+    #     for key in keys:
+    #         main_group.add_command(create_dynamic_group(key, meta[key]))
+    # else:
+    #     main_group = create_dynamic_group('cli', meta[list(meta.keys())[0]])
+    #
+    # if return_before_executing:
+    #     return main_group
+    # else:
+    #     main_group()
```

