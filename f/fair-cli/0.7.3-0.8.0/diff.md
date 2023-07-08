# Comparing `tmp/fair_cli-0.7.3.tar.gz` & `tmp/fair_cli-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fair_cli-0.7.3.tar", max compression
+gzip compressed data, was "fair_cli-0.8.0.tar", max compression
```

## Comparing `fair_cli-0.7.3.tar` & `fair_cli-0.8.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1855 2023-06-21 19:13:33.324048 fair_cli-0.7.3/CHANGELOG.md
--rw-r--r--   0        0        0     1358 2023-06-22 21:33:37.591898 fair_cli-0.7.3/CITATION.cff
--rw-r--r--   0        0        0     1314 2023-06-12 13:03:22.463351 fair_cli-0.7.3/LICENSE
--rw-r--r--   0        0        0    11363 2023-06-21 19:13:33.324484 fair_cli-0.7.3/README.md
--rw-r--r--   0        0        0     1976 2023-06-12 13:03:22.464552 fair_cli-0.7.3/fair/__init__.py
--rw-r--r--   0        0        0    21491 2023-06-22 21:28:17.110682 fair_cli-0.7.3/fair/cli.py
--rw-r--r--   0        0        0     9190 2023-06-21 19:13:33.326523 fair_cli-0.7.3/fair/common.py
--rw-r--r--   0        0        0    28212 2023-06-21 19:13:33.326880 fair_cli-0.7.3/fair/configuration/__init__.py
--rw-r--r--   0        0        0     3311 2023-06-21 19:13:33.326964 fair_cli-0.7.3/fair/configuration/validation.py
--rw-r--r--   0        0        0     5358 2023-06-21 19:13:33.327099 fair_cli-0.7.3/fair/exceptions.py
--rw-r--r--   0        0        0    10127 2023-06-21 19:13:33.327168 fair_cli-0.7.3/fair/files.txt
--rw-r--r--   0        0        0     4619 2023-06-21 19:13:33.327283 fair_cli-0.7.3/fair/history.py
--rw-r--r--   0        0        0     3958 2023-06-21 19:13:33.327397 fair_cli-0.7.3/fair/identifiers.py
--rw-r--r--   0        0        0     3010 2023-06-21 19:13:33.327463 fair_cli-0.7.3/fair/logging.py
--rw-r--r--   0        0        0     8206 2023-06-21 19:13:33.327581 fair_cli-0.7.3/fair/register.py
--rw-r--r--   0        0        0      161 2023-06-21 19:13:33.327663 fair_cli-0.7.3/fair/registry/__init__.py
--rw-r--r--   0        0        0     1249 2023-06-12 13:03:22.465501 fair_cli-0.7.3/fair/registry/file_formats.json
--rw-r--r--   0        0        0      120 2023-06-12 13:03:22.465547 fair_cli-0.7.3/fair/registry/file_types.py
--rw-r--r--   0        0        0    17292 2023-06-22 15:55:58.649339 fair_cli-0.7.3/fair/registry/requests.py
--rw-r--r--   0        0        0    14756 2023-06-21 19:13:33.328007 fair_cli-0.7.3/fair/registry/server.py
--rw-r--r--   0        0        0    23733 2023-06-22 15:55:58.649688 fair_cli-0.7.3/fair/registry/storage.py
--rw-r--r--   0        0        0    38515 2023-06-22 15:55:58.650104 fair_cli-0.7.3/fair/registry/sync.py
--rw-r--r--   0        0        0     4752 2023-06-21 19:13:33.329007 fair_cli-0.7.3/fair/registry/versioning.py
--rw-r--r--   0        0        0     2302 2023-06-21 19:13:33.329217 fair_cli-0.7.3/fair/run.py
--rw-r--r--   0        0        0    49608 2023-06-21 19:13:33.329700 fair_cli-0.7.3/fair/session.py
--rw-r--r--   0        0        0    16133 2023-06-21 19:13:33.329852 fair_cli-0.7.3/fair/staging.py
--rw-r--r--   0        0        0      490 2023-06-12 13:03:22.466460 fair_cli-0.7.3/fair/templates/__init__.py
--rw-r--r--   0        0        0      296 2023-06-12 13:03:22.466514 fair_cli-0.7.3/fair/templates/config.jinja
--rw-r--r--   0        0        0      136 2023-06-12 13:03:22.466556 fair_cli-0.7.3/fair/templates/hist.jinja
--rw-r--r--   0        0        0     3181 2023-06-21 19:13:33.329963 fair_cli-0.7.3/fair/testing.py
--rw-r--r--   0        0        0    53662 2023-06-22 16:29:13.604131 fair_cli-0.7.3/fair/user_config/__init__.py
--rw-r--r--   0        0        0     4830 2023-06-21 19:13:33.330469 fair_cli-0.7.3/fair/user_config/globbing.py
--rw-r--r--   0        0        0     9187 2023-06-21 19:13:33.330549 fair_cli-0.7.3/fair/user_config/validation.py
--rw-r--r--   0        0        0     5087 2023-06-21 19:13:33.330678 fair_cli-0.7.3/fair/utilities.py
--rw-r--r--   0        0        0     1465 2023-06-21 19:13:33.330742 fair_cli-0.7.3/fair/virtualenv.py
--rw-r--r--   0        0        0     2563 2023-06-22 21:33:27.711998 fair_cli-0.7.3/pyproject.toml
--rw-r--r--   0        0        0    13296 1970-01-01 00:00:00.000000 fair_cli-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1855 2023-06-21 19:13:33.324048 fair_cli-0.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1358 2023-07-08 08:05:57.894695 fair_cli-0.8.0/CITATION.cff
+-rw-r--r--   0        0        0     1314 2023-06-12 13:03:22.463351 fair_cli-0.8.0/LICENSE
+-rw-r--r--   0        0        0    11363 2023-06-21 19:13:33.324484 fair_cli-0.8.0/README.md
+-rw-r--r--   0        0        0     1976 2023-06-12 13:03:22.464552 fair_cli-0.8.0/fair/__init__.py
+-rw-r--r--   0        0        0    21694 2023-07-08 08:05:57.895050 fair_cli-0.8.0/fair/cli.py
+-rw-r--r--   0        0        0     9375 2023-07-08 08:05:57.895206 fair_cli-0.8.0/fair/common.py
+-rw-r--r--   0        0        0    30313 2023-07-08 08:05:57.895622 fair_cli-0.8.0/fair/configuration/__init__.py
+-rw-r--r--   0        0        0     3450 2023-07-08 08:05:57.895747 fair_cli-0.8.0/fair/configuration/validation.py
+-rw-r--r--   0        0        0     5358 2023-06-21 19:13:33.327099 fair_cli-0.8.0/fair/exceptions.py
+-rw-r--r--   0        0        0    10127 2023-06-21 19:13:33.327168 fair_cli-0.8.0/fair/files.txt
+-rw-r--r--   0        0        0     4719 2023-07-08 08:05:57.895862 fair_cli-0.8.0/fair/history.py
+-rw-r--r--   0        0        0     6030 2023-07-08 08:05:57.896046 fair_cli-0.8.0/fair/identifiers.py
+-rw-r--r--   0        0        0     3010 2023-06-21 19:13:33.327463 fair_cli-0.8.0/fair/logging.py
+-rw-r--r--   0        0        0     8866 2023-07-08 08:05:57.896249 fair_cli-0.8.0/fair/register.py
+-rw-r--r--   0        0        0      161 2023-06-21 19:13:33.327663 fair_cli-0.8.0/fair/registry/__init__.py
+-rw-r--r--   0        0        0     1249 2023-06-12 13:03:22.465501 fair_cli-0.8.0/fair/registry/file_formats.json
+-rw-r--r--   0        0        0      120 2023-06-12 13:03:22.465547 fair_cli-0.8.0/fair/registry/file_types.py
+-rw-r--r--   0        0        0    17475 2023-07-08 08:05:57.896859 fair_cli-0.8.0/fair/registry/requests.py
+-rw-r--r--   0        0        0    14996 2023-07-08 08:05:57.897060 fair_cli-0.8.0/fair/registry/server.py
+-rw-r--r--   0        0        0    23951 2023-07-08 08:05:57.897376 fair_cli-0.8.0/fair/registry/storage.py
+-rw-r--r--   0        0        0    40869 2023-07-08 08:05:57.897703 fair_cli-0.8.0/fair/registry/sync.py
+-rw-r--r--   0        0        0     4752 2023-06-21 19:13:33.329007 fair_cli-0.8.0/fair/registry/versioning.py
+-rw-r--r--   0        0        0     2302 2023-06-21 19:13:33.329217 fair_cli-0.8.0/fair/run.py
+-rw-r--r--   0        0        0    51582 2023-07-08 08:05:57.898192 fair_cli-0.8.0/fair/session.py
+-rw-r--r--   0        0        0    16133 2023-06-21 19:13:33.329852 fair_cli-0.8.0/fair/staging.py
+-rw-r--r--   0        0        0      490 2023-06-12 13:03:22.466460 fair_cli-0.8.0/fair/templates/__init__.py
+-rw-r--r--   0        0        0      296 2023-06-12 13:03:22.466514 fair_cli-0.8.0/fair/templates/config.jinja
+-rw-r--r--   0        0        0      136 2023-06-12 13:03:22.466556 fair_cli-0.8.0/fair/templates/hist.jinja
+-rw-r--r--   0        0        0     3220 2023-07-08 08:05:57.898323 fair_cli-0.8.0/fair/testing.py
+-rw-r--r--   0        0        0    54095 2023-07-08 08:05:57.898883 fair_cli-0.8.0/fair/user_config/__init__.py
+-rw-r--r--   0        0        0     4830 2023-06-21 19:13:33.330469 fair_cli-0.8.0/fair/user_config/globbing.py
+-rw-r--r--   0        0        0     9187 2023-06-21 19:13:33.330549 fair_cli-0.8.0/fair/user_config/validation.py
+-rw-r--r--   0        0        0     5087 2023-06-21 19:13:33.330678 fair_cli-0.8.0/fair/utilities.py
+-rw-r--r--   0        0        0     1465 2023-06-21 19:13:33.330742 fair_cli-0.8.0/fair/virtualenv.py
+-rw-r--r--   0        0        0     2496 2023-07-08 08:05:57.900281 fair_cli-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    13295 1970-01-01 00:00:00.000000 fair_cli-0.8.0/PKG-INFO
```

### Comparing `fair_cli-0.7.3/CHANGELOG.md` & `fair_cli-0.8.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.3/CITATION.cff` & `fair_cli-0.8.0/CITATION.cff`

 * *Files 10% similar despite different names*

```diff
@@ -32,8 +32,8 @@
 - FAIR
 - Data Management
 - Provenance
 license: BSD-2-Clause
 message: If you use this software, please cite it using these metadata.
 repository-code: https://github.com/FAIRDataPipeline/FAIR-CLI/
 title: "The FAIR Data Pipeline command line tool"
-version: 0.7.3
+version: 0.8.0
```

### Comparing `fair_cli-0.7.3/LICENSE` & `fair_cli-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.3/README.md` & `fair_cli-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.3/fair/__init__.py` & `fair_cli-0.8.0/fair/__init__.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.3/fair/cli.py` & `fair_cli-0.8.0/fair/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,29 +101,30 @@
             os.getcwd(), debug=debug, server_mode=fdp_svr.SwitchMode.CLI
         ) as fair_session:
             fair_session.status_data_products()
             fair_session.status_code_runs()
     except fdp_exc.FAIRCLIException as e:
         e.err_print()
         if e.level.lower() == "error":
-            if e.level.lower() == "error":
-                sys.exit(e.exit_code)
+            sys.exit(e.exit_code)
 
 @cli.group(invoke_without_command=True)
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 @click.option("--remote", help="Show Remote Code Runs", default= "")
 @click.pass_context
 def list(ctx, debug, remote) -> None:
     """Commands to list data_product(s) and code_run(s)"""
     if ctx.obj is None:
         ctx.obj = {}
     ctx.obj['DEBUG'] = debug
     ctx.obj['REMOTE'] = remote
-    ctx.invoke(data_products)
-    ctx.invoke(code_runs)
+    _current_args = " ".join(sys.argv)
+    if not ("data-products" in _current_args or "code-runs" in _current_args):
+        ctx.invoke(data_products)
+        ctx.invoke(code_runs)
 
 @list.command()
 @click.pass_context
 def data_products(ctx) -> None:
     debug = ctx.obj['DEBUG']
     remote = ctx.obj['REMOTE']
     try:
@@ -157,15 +158,15 @@
 def create(debug, output: str) -> None:
     """Generate a new FAIR repository user YAML config file"""
     output = (
         output[0]
         if output
         else os.path.join(os.getcwd(), fdp_com.USER_CONFIG_FILE)
     )
-    click.echo(f"Generating new user configuration file" f" '{output}'")
+    click.echo(f"Generating new user configuration file '{output}'")
     with fdp_session.FAIR(os.getcwd(), debug=debug) as fair_session:
         fair_session.make_starter_config(output)
 
 
 @cli.command()
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 def reset(debug: bool) -> None:
@@ -523,14 +524,15 @@
     default=False,
 )
 def run(
     config: str, script: str, debug: bool, ci: bool, dirty: bool, local: bool
 ):
     """Initialises a job with the option to specify a bash command"""
     # Allow no config to be specified, if that is the case use default local
+    click.echo("Running run please wait")
     config = config[0] if config else fdp_com.local_user_config(os.getcwd())
     try:
         with fdp_session.FAIR(
             os.getcwd(),
             config,
             debug=debug,
             server_mode=fdp_svr.SwitchMode.CLI,
@@ -632,14 +634,15 @@
 @click.option(
     "--dirty/--clean",
     help="Allow running with uncommitted changes",
     default=False,
 )
 def push(remote: str, debug: bool, dirty: bool):
     """Push data between the local and remote registry"""
+    click.echo("Running push please wait")
     remote = remote[0] if remote else "origin"
     try:
         with fdp_session.FAIR(
             os.getcwd(),
             debug=debug,
             server_mode=fdp_svr.SwitchMode.CLI,
             allow_dirty=dirty,
@@ -675,14 +678,15 @@
 @click.option(
     "--local/--no-local",
     help="init without a remote registry - useful for closed systems",
     default=False,
 )
 def pull(config: str, debug: bool, local: bool):
     """Update local registry from remotes and sources"""
+    click.echo("Running pull please wait")
     config = config[0] if config else fdp_com.local_user_config(os.getcwd())
     try:
         with fdp_session.FAIR(
             os.getcwd(),
             config,
             server_mode=fdp_svr.SwitchMode.CLI,
             debug=debug,
```

### Comparing `fair_cli-0.7.3/fair/common.py` & `fair_cli-0.8.0/fair/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,8 +292,15 @@
     return _repository.git.rev_parse("--show-toplevel").strip()
 
 def set_file_permissions(path: str):
     for root, dirs, files in os.walk(path, topdown=False):
         for dir in [os.path.join(root,d) for d in dirs]:
             os.chmod(dir, stat.S_IRWXU | stat.S_IRWXG | stat.S_IRWXO)
         for file in [os.path.join(root, f) for f in files]:
-            os.chmod(file, stat.S_IRWXU | stat.S_IRWXG | stat.S_IRWXO)
+            os.chmod(file, stat.S_IRWXU | stat.S_IRWXG | stat.S_IRWXO)
+
+def remove_readonly(fn, path, excinfo):
+    try:
+        os.chmod(path, stat.S_IWRITE)
+        fn(path)
+    except Exception as exc:
+        print("Skipped:", path, "because:\n", exc)
```

### Comparing `fair_cli-0.7.3/fair/configuration/__init__.py` & `fair_cli-0.8.0/fair/configuration/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,15 +258,15 @@
         raise fdp_exc.CLIConfigurationError(
             "Expected key 'git:remote_repo' in local CLI configuration"
         ) from e
 
 
 def get_remote_token(
     repo_dir: str, remote: str = "origin", local: bool = False
-) -> str:
+) -> typing.Optional[str]:
     _local_config = read_local_fdpconfig(repo_dir)
     if remote not in _local_config["registries"]:
         raise fdp_exc.CLIConfigurationError(
             f"Cannot find remote registry '{remote}' in local CLI configuration"
         )
     if "token" not in _local_config["registries"][remote]:
         raise fdp_exc.CLIConfigurationError(
@@ -374,14 +374,30 @@
         _uri = _local_conf["user"]["uri"]
     except KeyError:
         _uri = None
     if not _uri or _uri == "None":
         raise fdp_exc.CLIConfigurationError("No user URI identifier defined.")
     return _uri
 
+def get_current_user_github(repo_loc: str) -> str:
+    """Retrieves the URI identifier for the current user
+
+    Returns
+    -------
+    str
+        github username
+    """
+    _local_conf = read_local_fdpconfig(repo_loc)
+    try:
+        _github = _local_conf["user"]["github"]
+    except KeyError:
+        _github = None
+    if not _github or _github == "None":
+        raise fdp_exc.CLIConfigurationError("No user GitHub username defined.")
+    return _github
 
 def check_registry_exists(registry: str = None) -> typing.Optional[str]:
     """Checks if fair registry is set up on users machine
 
     Returns
     -------
     str
@@ -432,18 +448,18 @@
     if not _port:
         raise fdp_exc.InternalError(
             "Failed to determine port number from local registry URL"
         )
     return _port
 
 
-def update_local_port() -> str:
+def update_local_port(registry_dir: str = None) -> str:
     """Updates the local port in the global configuration from the session port file"""
-    _current_port = fdp_com.registry_session_port()
-    _current_address = fdp_com.registry_session_address()
+    _current_port = fdp_com.registry_session_port(registry_dir)
+    _current_address = fdp_com.registry_session_address(registry_dir)
 
     _new_url = f'http://{_current_address}:{_current_port}/api/'
 
     if os.path.exists(fdp_com.global_fdpconfig()) and read_global_fdpconfig():
         _glob_conf = read_global_fdpconfig()
         _glob_conf["registries"]["local"]["uri"] = _new_url
         with open(fdp_com.global_fdpconfig(), "w") as out_f:
@@ -470,15 +486,15 @@
     _user_info = fdp_id.check_orcid(user_orcid.strip())
 
     while not _user_info:
         click.echo("Invalid ORCID given.")
         user_orcid = click.prompt("ORCID")
         _user_info = fdp_id.check_orcid(user_orcid.strip())
 
-    _user_info["orcid"] = user_orcid
+    _user_info["orcid"] = user_orcid.strip()
 
     click.echo(
         f"Found entry: {_user_info['given_names']} {_user_info['family_name']}"
     )
 
     _def_ospace = "".join(_user_info["given_names"]).lower()
 
@@ -505,15 +521,15 @@
     _user_info = fdp_id.check_ror(user_ror.strip())
 
     while not _user_info:
         click.echo("Invalid ROR ID given.")
         user_ror = click.prompt("ROR ID")
         _user_info = fdp_id.check_ror(user_ror.strip())
 
-    _user_info["ror"] = user_ror
+    _user_info["ror"] = user_ror.strip()
 
     click.echo(f"Found entry: {_user_info['family_name']} ")
 
     _def_ospace = _user_info["family_name"].lower().replace(" ", "_")
 
     return _user_info, _def_ospace
 
@@ -536,22 +552,38 @@
     _user_info = fdp_id.check_grid(user_grid.strip())
 
     while not _user_info:
         click.echo("Invalid GRID ID given.")
         user_grid = click.prompt("GRID ID")
         _user_info = fdp_id.check_grid(user_grid.strip())
 
-    _user_info["grid"] = user_grid
+    _user_info["grid"] = user_grid.strip()
 
     click.echo(f"Found entry: {_user_info['family_name']} ")
 
     _def_ospace = _user_info["family_name"].lower().replace(" ", "_")
 
     return _user_info, _def_ospace
 
+def _handle_github(user_github: str) -> typing.Tuple[typing.Dict, str]:
+
+    _user_info = fdp_id.check_github(user_github.strip())
+
+    while not _user_info:
+        time.sleep(3)
+        click.echo(f"Invalid GitHub Username '{user_github}' given.")
+        user_github = click.prompt("GitHub Username")
+        _user_info = fdp_id.check_github(user_github.strip())
+
+    _def_ospace = _user_info["github"].lower()
+    
+    click.echo(f"Found entry: {_user_info['github']} ")
+    return _user_info, _def_ospace
+
+
 
 def _handle_uuid() -> typing.Tuple[typing.Dict, str]:
     """Obtain metadata for user where no ID provided
 
     Returns
     -------
     user_info : typing.Dict
@@ -571,25 +603,32 @@
         _def_ospace += _full_name
         _user_info["given_names"] = _full_name
         _user_info["family_name"] = None
 
     return _user_info, _def_ospace
 
 
-def _get_user_info_and_namespaces() -> typing.Dict[str, typing.Dict]:
-    _user_email = click.prompt("Email")
+def _get_user_info_and_namespaces(local: bool = False) -> typing.Dict[str, typing.Dict]:
+    _user_email = click.prompt("Email (optional)", default = "")
 
     _invalid_input = True
 
     while _invalid_input:
         _id_type = click.prompt(
-            "User ID system (ORCID/ROR/GRID/None)", default="None"
+            "User ID system (GITHUB/ORCID/ROR/GRID/None)", default="GITHUB"
         )
-
-        if _id_type.upper() == "ORCID":
+        if _id_type.upper() == "GITHUB":
+            _user_github = click.prompt("GitHub Username")
+            _user_info, _def_ospace = _handle_github(_user_github)
+            if not _user_info["name"]:
+                _user_info["given_names"] = click.prompt("Given Names")
+                _user_info["family_name"] = click.prompt("Family Name")
+                _user_info["name"] = " ".join([_user_info["given_names"], _user_info["family_name"]])
+            _invalid_input = False
+        elif _id_type.upper() == "ORCID":
             _user_orcid = click.prompt("ORCID")
             _user_info, _def_ospace = _handle_orcid(_user_orcid)
             _invalid_input = False
         elif _id_type.upper() == "ROR":
             _user_ror = click.prompt("ROR ID")
             _user_info, _def_ospace = _handle_ror(_user_ror)
             _invalid_input = False
@@ -599,22 +638,33 @@
             _invalid_input = False
         elif _id_type.upper() == "NONE":
             _user_info, _def_ospace = _handle_uuid()
             _user_uuid = str(uuid.uuid4())
             _user_info["uuid"] = _user_uuid
             _invalid_input = False
 
-    _user_info["email"] = _user_email
-
     _def_ospace = _def_ospace.lower().replace(" ", "").strip()
     _def_ospace = click.prompt("Default output namespace", default=_def_ospace)
     _def_ispace = click.prompt("Default input namespace", default=_def_ospace)
 
     _namespaces = {"input": _def_ispace, "output": _def_ospace}
 
+    if not "github" in _user_info:
+        if local:
+            _user_info["github"] = "FAIRDataPipeline"
+        else:
+            _user_github = click.prompt("GitHub Username")
+            _user_github_info = _handle_github(_user_github)[0]
+            _user_info["github"] = _user_github_info["github"]
+
+    if not _user_email:
+        _user_info["email"] = f'{_user_info["github"]}@users.noreply.github.com'
+    else:
+        _user_info["email"] = _user_email
+
     return {"user": _user_info, "namespaces": _namespaces}
 
 
 def global_config_query(
     registry: str = None, local: bool = False
 ) -> typing.Dict[str, typing.Any]:
     """Ask user question set for creating global FAIR config"""
@@ -664,43 +714,45 @@
         _remote_url = click.prompt("Remote API URL", default=_default_rem)
 
         _rem_data_store = click.prompt(
             "Remote Data Storage Root",
             default=_remote_url.replace("/api/", "/data/"),
         )
 
-        _rem_key_file = click.prompt(
-            "Remote API Token File",
-        )
-        _rem_key_file = os.path.expandvars(_rem_key_file)
-
-        while (
-            not os.path.exists(_rem_key_file)
-            or not open(_rem_key_file).read().strip()
-        ):
-            click.echo(
-                f"Token file '{_rem_key_file}' does not exist or is empty, "
-                "please provide a valid token file."
+        _rem_key_valid = False
+        while not _rem_key_valid:
+            _rem_key = click.prompt(
+                f"Remote API Token",
             )
-            _rem_key_file = click.prompt("Remote API Token File")
-            _rem_key_file = os.path.expandvars(_rem_key_file)
+            if len(_rem_key) == 40:
+                _rem_key_valid = True
+            else:
+                click.echo("Remote token should be 40 characters long")
+
+        _rem_key_file = os.path.join(fdp_com.global_config_dir(), "remotetoken.txt")
+
+        with open(_rem_key_file, 'w') as f:
+            f.write(_rem_key)
+
+        if not os.path.exists(_rem_key_file):
+            raise fdp_exc.CLIConfigurationError(f'Token could not be written to {_rem_key_file}')
 
     if not fdp_serv.check_server_running():
         if _ := click.confirm(
             "Local registry is offline, would you like to start it?",
             default=False,
         ):
             fdp_serv.launch_server(registry_dir=registry)
 
             # Keep server running by creating user run cache file
             _cache_addr = os.path.join(fdp_com.session_cache_dir(), "user.run")
             pathlib.Path(_cache_addr).touch()
 
         else:
-            click.echo("Temporarily launching server to retrieve API token.")
+            click.echo("Temporarily launching local registry to retrieve API token.")
             fdp_serv.launch_server(registry_dir=registry)
             fdp_serv.stop_server(registry_dir=registry, local_uri=_local_uri)
             try:
                 fdp_req.local_token(registry_dir=registry)
             except fdp_exc.FileNotFoundError as e:
                 raise fdp_exc.RegistryError(
                     "Failed to retrieve local API token from registry."
@@ -709,15 +761,15 @@
     _loc_data_store = click.prompt(
         "Default Data Store",
         default=os.path.join(fdp_com.USER_FAIR_DIR, f"data{os.path.sep}"),
     )
     if _loc_data_store[-1] != os.path.sep:
         _loc_data_store += os.path.sep
 
-    _glob_conf_dict = _get_user_info_and_namespaces()
+    _glob_conf_dict = _get_user_info_and_namespaces(local)
     _glob_conf_dict["registries"] = {
         "local": {
             "uri": _local_uri,
             "directory": os.path.abspath(registry),
             "data_store": _loc_data_store,
             "token": os.path.join(os.path.abspath(registry), "token"),
         },
```

### Comparing `fair_cli-0.7.3/fair/configuration/validation.py` & `fair_cli-0.8.0/fair/configuration/validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,17 @@
     )
     uuid: typing.Optional[pydantic.UUID4] = pydantic.Field(
         None, title="user UUID", description="The users UUID if applicable"
     )
     name: typing.Optional[str] = pydantic.Field(
         None, title="Full Name", description="Full name for the user"
     )
+    github: typing.Optional[str] = pydantic.Field(
+        None, title="GitHub Username", description="GitHub Username for the user"
+    )
 
     class Config:
         extra = "forbid"
 
 
 class LocalCLIConfig(pydantic.BaseModel):
     git: Git
```

### Comparing `fair_cli-0.7.3/fair/exceptions.py` & `fair_cli-0.8.0/fair/exceptions.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.3/fair/files.txt` & `fair_cli-0.8.0/fair/files.txt`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.3/fair/history.py` & `fair_cli-0.8.0/fair/history.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 """
 import glob
 import os
 
 import click
 import rich
 
+from pathlib import Path
+
 import fair.common as fdp_com
 import fair.exceptions as fdp_exc
 import fair.run as fdp_run
 import fair.templates as fdp_tpl
 
 
 def history_directory(repo_loc: str) -> str:
@@ -57,16 +59,18 @@
         SHA identifier for the job
 
     Returns
     -------
     str
         log file location for the given job
     """
+    _job_dir  = Path(f"{fdp_com.default_jobs_dir()}")
+
     _sorted_time_dirs = sorted(
-        glob.glob(os.path.join(fdp_com.default_jobs_dir(), "*")), reverse=True
+        glob.glob(os.path.join(_job_dir, "*")), reverse=True
     )
 
     _log_files = [
         os.path.join(
             history_directory(repo_loc), f"job_{os.path.basename(i)}.log"
         )
         for i in _sorted_time_dirs
@@ -103,16 +107,18 @@
     ----------
     repo_loc : str
         FAIR-CLI repository path
     length : int, optional
         max number of entries to display, by default 10
     """
 
+    _job_dir  = Path(f"{fdp_com.default_jobs_dir()}")
+
     _sorted_time_dirs = sorted(
-        glob.glob(os.path.join(fdp_com.default_jobs_dir(), "*")), reverse=True
+        glob.glob(os.path.join(_job_dir, "*")), reverse=True
     )
 
     _log_files = [
         os.path.join(
             history_directory(repo_loc), f"job_{os.path.basename(i)}.log"
         )
         for i in _sorted_time_dirs
```

### Comparing `fair_cli-0.7.3/fair/identifiers.py` & `fair_cli-0.8.0/fair/identifiers.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,23 +20,30 @@
 
 import time
 import typing
 import urllib.parse
 
 import requests
 import requests.exceptions
+import logging
+from urllib3.exceptions import InsecureRequestWarning
+from fake_useragent import UserAgent
+
+logger = logging.getLogger("FAIRDataPipeline.Identifiers")
 
 ID_URIS = {
     "orcid": "https://orcid.org/",
     "ror": "https://ror.org/",
+    "github" : "https://github.com/"
 }
 
 QUERY_URLS = {
     "orcid": "https://pub.orcid.org/v3.0/",
     "ror": "https://api.ror.org/organizations?query=",
+    "github": "https://api.github.com/users/"
 }
 
 
 def check_orcid(orcid: str) -> typing.Dict:
     """Checks if valid ORCID using ORCID public api
 
     Parameters
@@ -45,22 +52,24 @@
         ORCID to be checked
 
     Returns
     -------
     typing.Dict
         metadata from the given ID
     """
-
+    orcid = orcid.replace(ID_URIS["orcid"], "")
     _header = {"Accept": "application/json"}
     _url = urllib.parse.urljoin(QUERY_URLS["orcid"], orcid)
-    _response = requests.get(_url, headers=_header)
+    requests.packages.urllib3.disable_warnings(category=InsecureRequestWarning)
+    _response = requests.get(_url, headers=_header, verify = False, allow_redirects = True)
 
     _result_dict: typing.Dict[str, typing.Any] = {}
 
     if _response.status_code != 200:
+        logger.debug(f"{_url} Responded with {_response.status_code}")
         return _result_dict
 
     _names = _response.json()["person"]["name"]
     _given = _names["given-names"]["value"]
     _family = _names["family-name"]["value"]
     _name = f"{_given} {_family}"
 
@@ -68,29 +77,64 @@
     _result_dict["family_name"] = _family
     _result_dict["given_names"] = _given
     _result_dict["orcid"] = orcid
     _result_dict["uri"] = f'{ID_URIS["orcid"]}{orcid}'
 
     return _result_dict
 
+def check_github(github: str) -> typing.Dict:
+    """Checks if valid ORCID using ORCID public api
+
+    Parameters
+    ----------
+    github : str
+        github username to be checked
+
+    Returns
+    -------
+    typing.Dict
+        metadata from the given ID
+    """
+    _header = {"Accept": "application/json"}
+    _url = urllib.parse.urljoin(QUERY_URLS["github"], github)
+    requests.packages.urllib3.disable_warnings(category=InsecureRequestWarning)
+    _response = requests.get(_url, headers=_header, verify = False, allow_redirects = True)
+
+    _result_dict: typing.Dict[str, typing.Any] = {}
+
+    if _response.status_code != 200:
+        logger.debug(f"{_url} Responded with {_response.status_code}")
+        return _result_dict
+
+    _login = _response.json()["login"]
+    _name = _response.json()["name"]
+    if _name:
+        _result_dict["family_name"] = _name.split()[-1]
+        _result_dict["given_names"] = " ".join(_name.split()[:-1])
+        
+    _result_dict["name"] = _name    
+    _result_dict["github"] = _login
+    _result_dict["uri"] = f'{ID_URIS["github"]}{_login}'
+
+    return _result_dict
+
 
 def check_ror(ror: str) -> typing.Dict:
     """Checks if valid ROR using ROR public api
 
     Parameters
     ----------
     ror : str
         ROR to be checked
 
     Returns
     -------
     typing.Dict
         metadata from the given ID
     """
-
     _result_dict = _check_generic_ror(ror)
     if _result_dict:
         _result_dict["ror"] = ror
 
     return _result_dict
 
 
@@ -120,21 +164,21 @@
         ROR to be checked
 
     Returns
     -------
     typing.Dict
         metadata from the given ID
     """
-
     _url = f"{QUERY_URLS['ror']}{id}"
     _response = requests.get(_url)
 
     _result_dict: typing.Dict[str, typing.Any] = {}
 
     if _response.status_code != 200:
+        logger.debug(f"{_url} Responded with {_response.status_code}")
         return _result_dict
 
     if _response.json()["number_of_results"] == 0:
         return _result_dict
 
     _id = _response.json()["items"][0]["id"]
     _name = _response.json()["items"][0]["name"]
@@ -160,22 +204,29 @@
 
     Returns
     -------
     bool
         if valid identifier
     """
     _n_attempts = 0
+    fake_agent = False
 
     while _n_attempts < retries:
         try:
-            requests.get(identifier).raise_for_status()
+            requests.packages.urllib3.disable_warnings(category=InsecureRequestWarning)
+            headers = {}
+            if fake_agent:
+                headers = {'User-Agent':str(UserAgent().chrome)} 
+            requests.get(identifier, verify = False, allow_redirects = True, headers = headers).raise_for_status()
             return True
         except (
             requests.exceptions.MissingSchema,
             requests.exceptions.HTTPError,
             requests.exceptions.ConnectionError,
-        ):
+        ) as e:
             _n_attempts += 1
-            time.sleep(1)
+            time.sleep(3)
+            fake_agent = True
+            logger.warning(f"Error identifier: '{identifier}' caused '{e}'")
             continue
 
     return False
```

### Comparing `fair_cli-0.7.3/fair/logging.py` & `fair_cli-0.8.0/fair/logging.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.3/fair/register.py` & `fair_cli-0.8.0/fair/register.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,26 +84,41 @@
         Dict containing working config
 
     Returns
     -------
     typing.List[str]
         list of registered object URLs
     """
-    _expected_keys = [
+    _expected_keys_external_object = [
         "root",
         "path",
         "file_type",
         "primary",
         "version",
         "public",
     ]
 
+    _expected_keys_data_product = [
+        "root",
+        "path",
+        "file_type",
+        "version",
+        "public"
+    ]
+
     _stored_objects: typing.List[str] = []
 
     for entry in user_config_register:
+        logger.debug(f"entry {entry}")
+
+        if "external_object" in entry:
+            _expected_keys = _expected_keys_external_object
+        else:
+            _expected_keys = _expected_keys_data_product
+
         for key in _expected_keys:
             if key not in entry and key not in entry["use"]:
                 raise fdp_exc.UserConfigError(
                     f"Expected key '{key}' in 'register' item"
                 )
 
         _identifier: str = entry["identifier"] if "identifier" in entry else ""
@@ -162,26 +177,30 @@
             _name = entry["use"]["data_product"]
             _obj_type = "data_product"
             _search_data = {"name": _name}
 
         _search_data["version"] = entry["use"]["version"]
         _namespace = entry["use"]["namespace"]
 
-        if not _identifier and not _unique_name:
-            raise fdp_exc.UserConfigError(
-                "Expected either 'unique_name' or 'identifier' in 'register' item"
-            )
-
-        elif _identifier and _unique_name:
-            raise fdp_exc.UserConfigError(
-                "Only one unique identifier may be provided (doi/unique_name)"
-            )
+        if _external_object:
+            if not _identifier and not _unique_name:
+                raise fdp_exc.UserConfigError(
+                    "Expected either 'unique_name' or 'identifier' in 'register' item"
+                )
 
+            elif _identifier and _unique_name:
+                raise fdp_exc.UserConfigError(
+                    "Only one unique identifier may be provided (doi/unique_name)"
+                )
+        # Set Remove to True by default so the tempory file gets deleted
+        _remove = True
         if "cache" in entry:
             _temp_data_file = entry["cache"]
+            # Don't delete the tempory file if it's from a cache
+            _remove = False
         else:
             _local_parsed = urllib.parse.urlparse(local_uri)
             _local_url = f"{_local_parsed.scheme}://{_local_parsed.netloc}"
             _temp_data_file = fdp_sync.download_from_registry(
                 _local_url, root=entry["root"], path=entry["path"]
             )
 
@@ -203,15 +222,16 @@
         # Hash matched version already present
         if _is_present == "hash_match":
             logger.debug(
                 "Skipping item '%s' as a hash matched entry is already"
                 " present with this name, deleting temporary data file",
                 _name,
             )
-            os.remove(_temp_data_file)
+            if _remove:
+                os.remove(_temp_data_file)
             continue
 
         # Item found but not hash matched retrieve a version number
         elif _is_present != "absent":
             _results = _is_present
             _user_version = fdp_ver.get_correct_version(
                 results_list=_results,
@@ -235,15 +255,16 @@
             _local_dir, f"{_user_version}.{entry['file_type']}"
         )
         # Copy the temporary file into the data store
         # then remove temporary file to save space
         logger.debug("Saving data file to '%s'", _local_file)
         shutil.copy(_temp_data_file, _local_file)
 
-        os.remove(_temp_data_file)
+        if _remove:
+            os.remove(_temp_data_file)
 
         if "public" in entry:
             _public = entry["public"]
 
         data = copy.deepcopy(entry)
 
         data["namespace_name"] = entry["use"]["namespace"]
```

### Comparing `fair_cli-0.7.3/fair/registry/file_formats.json` & `fair_cli-0.8.0/fair/registry/file_formats.json`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.3/fair/registry/requests.py` & `fair_cli-0.8.0/fair/registry/requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,17 @@
 import fair.common as fdp_com
 import fair.exceptions as fdp_exc
 import fair.utilities as fdp_util
 
 import ssl
 from requests.adapters import HTTPAdapter
 from urllib3.poolmanager import PoolManager
+from urllib3.exceptions import InsecureRequestWarning
+
+from fake_useragent import UserAgent
 
 logger = logging.getLogger("FAIRDataPipeline.Requests")
 
 
 def split_api_url(
     request_url: str, splitter: str = "api"
 ) -> typing.Tuple[str]:
@@ -524,35 +527,34 @@
     str
         path of downloaded temporary file
     """
     # Save the data to a temporary file so we can calculate the hash
     _file = tempfile.NamedTemporaryFile(delete=False)
     _fname = _file.name
 
-    # Copy File if local (Windows fix)
-    if "file://" in url and platform.system() == "Windows":
+    # Copy File if local
+    if "file://" in url:
         _local_fname = url.replace("file://", "")
         try:
             shutil.copy2(_local_fname, _fname)
         except Exception as e:
             raise fdp_exc.FAIRCLIException(
                 f"Failed to download file '{url}'"
                 f" due to connection error: {traceback.format_exc()}"
             ) from e
-
     else:
         try:
-            with urllib.request.urlopen(url) as response, open(
-                _fname, "wb"
-            ) as out_file:
-                shutil.copyfileobj(response, out_file)
-        except urllib.error.URLError as e:
+            requests.packages.urllib3.disable_warnings(category=InsecureRequestWarning)
+            headers = {'User-Agent':str(UserAgent().chrome)}
+            response = requests.get(url, allow_redirects = True, verify = False, headers = headers)
+            open(_fname, 'wb').write(response.content)
+        except Exception as e:
             raise fdp_exc.FAIRCLIException(
                 f"Failed to download file '{url}'"
-                f" due to connection error: {e.reason}"
+                f" due to connection error: {traceback.format_exc()}"
             ) from e
 
     return _fname
 
 
 def get_dependency_listing(uri: str, token: str, read_only: bool = False) -> typing.Dict:
     """Get complete listing of all objects and their registry based dependencies
@@ -567,15 +569,15 @@
     Returns
     -------
     typing.Dict
         dictionary of object types and their registry based dependencies
     """
     try:
         _registry_objs = url_get(uri, token)
-    except:
+    except Exception:
         return {[]}
 
     _rtn =  {
         obj: filter_object_dependencies(
             uri,
             obj,
             token,
```

### Comparing `fair_cli-0.7.3/fair/registry/server.py` & `fair_cli-0.8.0/fair/registry/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         raise fdp_exc.RegistryError(
             f"Failed to find local registry executable '{_server_start_script}',"
             " is the FAIR data pipeline properly installed on this system?"
         )
 
     _cmd = [_server_start_script, "-p", f"{port}", "-a", f"{address}"]
 
-    os.environ["FAIR_ALLOWED_HOSTS"] = address if not "FAIR_ALLOWED_HOSTS" in os.environ else os.environ["FAIR_ALLOWED_HOSTS"] + f",{address}"
+    os.environ["FAIR_ALLOWED_HOSTS"] = address if "FAIR_ALLOWED_HOSTS" not in os.environ else os.environ["FAIR_ALLOWED_HOSTS"] + f",{address}"
 
     logger.debug("Launching server with command '%s'", " ".join(_cmd))
 
     _start = subprocess.Popen(
         _cmd,
         stdout=subprocess.PIPE,
         stderr=subprocess.STDOUT,
@@ -137,15 +137,15 @@
 
     if verbose and platform.system() != "Windows":
         for c in iter(lambda: _start.stdout.read(1), b""):
             sys.stdout.buffer.write(c)
 
     _start.wait()
 
-    local_uri = fdp_conf.update_local_port()
+    local_uri = fdp_conf.update_local_port(registry_dir)
 
     if not check_server_running(local_uri):
         raise fdp_exc.RegistryError(
             "Failed to start local registry, no response from server"
         )
 
 
@@ -189,18 +189,18 @@
 
     if not os.path.exists(_server_stop_script):
         raise fdp_exc.RegistryError(
             f"Failed to find local registry executable '{_server_stop_script}',"
             " is the FAIR data pipeline properly installed on this system?"
         )
 
-    logger.debug("Stopping local registry server.")
+    logger.debug(f"Stopping local registry server with '{_server_stop_script}'.")
 
     _stop = subprocess.Popen(
-        _server_stop_script,
+        [_server_stop_script, ""],
         stdout=subprocess.PIPE,
         stderr=subprocess.STDOUT,
         shell=False,
     )
 
     if verbose:
         for c in iter(lambda: _stop.stdout.read(1), b""):
@@ -324,15 +324,15 @@
         with open(fdp_com.global_fdpconfig(), "w") as out_conf:
             yaml.dump(fdp_util.expand_dict(_glob_conf), out_conf)
 
     if force:
         logger.debug("Removing existing installation at '%s'", install_dir)
         if platform.system() == "Windows":
             fdp_com.set_file_permissions(install_dir)
-        shutil.rmtree(install_dir, ignore_errors=True)
+        shutil.rmtree(install_dir, onerror=fdp_com.remove_readonly)
 
     logger.debug("Creating directories for installation if they do not exist")
 
     os.makedirs(os.path.dirname(install_dir), exist_ok=True)
 
     _repo = git.Repo.clone_from(repository, install_dir)
 
@@ -419,32 +419,32 @@
     ):
         logger.debug(
             "Uninstalling registry, removing '%s'", fdp_com.registry_home()
         )
         # On windows file permisions need to be set prior to removing the directory
         if platform.system() == "Windows":
             fdp_com.set_file_permissions(fdp_com.registry_home())
-        shutil.rmtree(fdp_com.registry_home())
+        shutil.rmtree(fdp_com.registry_home(), onerror=fdp_com.remove_readonly)
     elif os.path.exists(fdp_com.DEFAULT_REGISTRY_LOCATION):
         logger.debug(
             "Uninstalling registry, removing '%s'",
             fdp_com.DEFAULT_REGISTRY_LOCATION,
         )
         # On windows file permisions need to be set prior to removing the directory
         if platform.system() == "Windows":
             fdp_com.set_file_permissions(fdp_com.DEFAULT_REGISTRY_LOCATION)
-        shutil.rmtree(fdp_com.DEFAULT_REGISTRY_LOCATION)
+        shutil.rmtree(fdp_com.DEFAULT_REGISTRY_LOCATION, onerror=fdp_com.remove_readonly)
     else:
         raise fdp_exc.RegistryError(
             "Cannot uninstall registry, no local installation identified"
         )
 
 
 def update_registry_post_setup(
-    repo_dir: str, global_setup: bool = False
+    repo_dir: str, global_setup: bool = False, registry_dir: str = None
 ) -> None:
     """Add user namespace and file types after CLI setup
 
     Parameters
     ----------
     repo_dir : str
         current FAIR repository location
@@ -454,43 +454,43 @@
     logger = logging.getLogger("FAIRDataPipeline.Server")
 
     logger.debug("Updating registry from latest setup")
 
     _is_running = check_server_running(fdp_conf.get_local_uri())
 
     if not _is_running:
-        launch_server()
+        launch_server(registry_dir = registry_dir)
 
     if global_setup:
         logger.debug("Populating file types")
         fdp_store.populate_file_type(
-            fdp_conf.get_local_uri(), fdp_req.local_token()
+            fdp_conf.get_local_uri(), fdp_req.local_token(registry_dir)
         )
 
     logger.debug("Adding 'author' and 'UserAuthor' entries if not present")
     # Add author and UserAuthor
     _author_url = fdp_store.store_user(
-        repo_dir, fdp_conf.get_local_uri(), fdp_req.local_token()
+        repo_dir, fdp_conf.get_local_uri(), fdp_req.local_token(registry_dir)
     )
 
     try:
         _admin_url = fdp_req.get(
             fdp_conf.get_local_uri(),
             "users",
-            fdp_req.local_token(),
+            fdp_req.local_token(registry_dir),
             params={"username": "admin"},
         )[0]["url"]
     except (KeyError, IndexError) as e:
         raise fdp_exc.RegistryError(
             "Failed to retrieve 'admin' user from registry database"
         ) from e
 
     fdp_req.post_else_get(
         fdp_conf.get_local_uri(),
         "user_author",
-        fdp_req.local_token(),
+        fdp_req.local_token(registry_dir),
         data={"user": _admin_url, "author": _author_url},
     )
 
     # Only stop the server if it was not running initially
     if not _is_running:
-        stop_server()
+        stop_server(registry_dir)
```

### Comparing `fair_cli-0.7.3/fair/registry/storage.py` & `fair_cli-0.8.0/fair/registry/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,14 +132,19 @@
     try:
         _id = fdp_conf.get_current_user_uri(repo_dir)
     except fdp_exc.CLIConfigurationError:
         _uuid = fdp_conf.get_current_user_uuid(repo_dir)
 
     return store_author(uri, token, name, _id, _uuid)
 
+def store_user_author(uri:str, token:str, user_uri:str, author_uri:str)-> str:
+    _data = {"user": user_uri, "author": author_uri}
+
+    return fdp_req.post_else_get(uri, "user_author", token, _data, _data)
+
 
 def populate_file_type(uri: str, token: str) -> typing.List[typing.Dict]:
     """Populates file_type table with common file file_types
 
     Parameters
     ----------
     uri: str
@@ -473,15 +478,15 @@
     is_public: bool,
 ) -> str:
     _hash = calculate_file_hash(local_file)
 
     _storage_loc_data = {
         "path": relative_path,
         "storage_root": root_store_url,
-        "public": is_public,
+        "public": str(is_public).lower(),
         "hash": _hash,
     }
 
     _search_data = {"hash": _hash}
 
     return fdp_req.post_else_get(
         registry_uri,
@@ -576,15 +581,15 @@
             registry_uri, "object", registry_token, data=_object_data
         )["url"]
     except fdp_exc.RegistryAPICallError as e:
         if e.error_code != 409:
             raise e
         else:
             raise fdp_exc.RegistryAPICallError(
-                f"Cannot post object" f"'{_desc}', duplicate already exists",
+                f"Cannot post object '{_desc}', duplicate already exists",
                 error_code=409,
             ) from e
 
     except KeyError as e:
         raise fdp_exc.InternalError(
             f"Expected key 'url' in local registry API response"
             f" for post object '{_desc}'"
```

### Comparing `fair_cli-0.7.3/fair/registry/sync.py` & `fair_cli-0.8.0/fair/registry/sync.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
     def _dependency_of(url_list: collections.deque, item: str, _dependency_list:dict):
         if item in url_list:
             return
         url_list.appendleft(item)
         try:
             _results = fdp_req.url_get(item, token)
-        except:
+        except Exception:
             _results = {}
         _type = fdp_req.get_obj_type_from_url(item, token)
         for req, val in _results.items():
             if req in _dependency_list[_type] and val:
                 if isinstance(val, list):
                     for url in val:
                         _dependency_of(url_list, url, _dependency_list)
@@ -120,38 +120,38 @@
     logger.debug(
         "Found %s namespace%s on remote",
         len(_remote_namespaces),
         "s" if len(_remote_namespaces) != 1 else "",
     )
 
     if not _remote_namespaces:
-        return
+        return []
 
     _writable_fields = fdp_req.get_writable_fields(
         local_uri, "namespace", local_token
     )
 
     for namespace in _remote_namespaces:
         _writable_data = {
             k: v for k, v in namespace.items() if k in _writable_fields
         }
         logger.debug("Writable local object data: %s", _writable_data)
         fdp_req.post_else_get(
             local_uri, "namespace", local_token, _writable_data
         )
 
-
 def sync_dependency_chain(
     object_url: str,
     dest_uri: str,
     origin_uri: str,
     dest_token: str,
     origin_token: str,
     local_data_store: str = None,
     public: bool = False,
+    remote_author_url = None
 ) -> typing.Dict[str, str]:
     """Push an object and all of its dependencies to the remote registry
 
     In order to push an object, firstly any dependencies which are also
     registry items must be pushed first.
 
     Parameters
@@ -221,15 +221,16 @@
             origin_token=origin_token,
             dest_uri=dest_uri,
             dest_token=dest_token,
             object_url=object_url,
             new_urls=_new_urls,
             writable_data=_writable_data,
             local_data_store = local_data_store,
-            public = public
+            public = public,
+            remote_author_url = remote_author_url
         )
 
         if not fdp_util.is_api_url(dest_uri, _new_url):
             raise fdp_exc.InternalError(
                 f"Expected new URL '{_new_url}' to be compatible with destination URI '{dest_uri}'"
             )
 
@@ -244,15 +245,16 @@
     origin_token: str,
     dest_uri: str,
     dest_token: str,
     object_url: str,
     new_urls: typing.Dict,
     writable_data: typing.Dict,
     local_data_store = None,
-    public = False
+    public = False,
+    remote_author_url = None
 ) -> typing.Tuple[typing.Dict, typing.List]:
     """Internal Function to return a resgistry entry from the remote registry given an origin entry URL
     If the entry does not exist it will be created
 
     Args:
         origin_uri (str): Url of the origin registry
         origin_token (str): Token of the origin registry
@@ -322,32 +324,84 @@
             return _remote_storage_root_url
         if "path" in _new_obj_data:
             _new_obj_data["path"] = _filters["path"] = _new_obj_data["hash"]
         if "storage_root" in _new_obj_data:
             _new_obj_data["storage_root"] = _remote_storage_root_url
             _filters["storage_root"] = fdp_req.get_obj_id_from_url(_remote_storage_root_url)
 
+    if remote_author_url and _obj_type == "object":
+        _new_obj_data["authors"] = _filters["authors"] = [remote_author_url]
+
     return fdp_req.post_else_get(
         dest_uri,
         _obj_type,
         data=_new_obj_data,
         token=dest_token,
         params=_filters,
     )
 
+def sync_author(
+    origin_uri: str,
+    dest_uri: str,
+    dest_token: str,
+    origin_token: str,
+    identifier: str
+) -> None:
+    current_author = fdp_req.get(
+        origin_uri,
+        "author",
+        origin_token,
+        params= {"identifier": identifier}
+    )
+    if not current_author:
+        raise fdp_exc.RegistryError(f"No author matching {name}, on local registry", "Have you run fair init?")
+    current_author_url = current_author[0]['url']
+    new_urls = sync_dependency_chain(
+        current_author_url,
+        dest_uri,
+        origin_uri,
+        dest_token,
+        origin_token
+        )
+    if not new_urls:
+        raise fdp_exc.RegistryError(f"Auther {name}, could not be pushed to {dest_uri}")
+    new_author_url = new_urls[current_author_url]
+    if not new_author_url:
+        raise fdp_exc.RegistryError(f"Auther {name}, was not be pushed to {dest_uri}")
+    return new_author_url
+
+def sync_user_author(
+    origin_uri: str,
+    dest_uri: str,
+    dest_token: str,
+    origin_token: str,
+    author_url: str,
+    github: str
+) -> None:
+    current_user = fdp_req.get(
+        dest_uri,
+        "users",
+        dest_token,
+        params= {"username": github}
+    )
+    if not current_user:
+        raise fdp_exc.RegistryError(f"No user matching {github}, on remote registry", "Does your GitHub username match the remote registry GitHub user?")
+    current_user_url = current_user[0]['url']
+    fdp_store.store_user_author(dest_uri, dest_token, current_user_url, author_url)
 
 def sync_data_products(
     origin_uri: str,
     dest_uri: str,
     dest_token: str,
     origin_token: str,
     remote_label: str,
     data_products: typing.List[str],
     local_data_store: str = None,
     force: bool = False,
+    remote_author_url = None
 ) -> None:
     """Transfer data products from one registry to another
 
     Parameters
     ----------
     origin_uri : str
         origin data registry URL
@@ -436,15 +490,16 @@
         sync_dependency_chain(
             object_url=result["url"],
             dest_uri=dest_uri,
             origin_uri=origin_uri,
             dest_token=dest_token,
             origin_token=origin_token,
             local_data_store=local_data_store,
-            public=_is_public
+            public=_is_public,
+            remote_author_url = remote_author_url
         )
         # If local_data_store assume we're syncing from remote to local
         if local_data_store:
             logger.debug("Retrieving files from remote registry data storage")
             fetch_data_product(origin_token, local_data_store, result[0])
         # Else going from local to remote
         else:
@@ -458,27 +513,27 @@
                         "code_run",
                         origin_token,
                         params= {"inputs": fdp_req.get_obj_id_from_url(origin_component_url)}
                     )
                 for origin_input_code_run in origin_input_code_runs:
                     dest_component_url = get_dest_component_url(origin_component_url, dest_uri, dest_token, origin_token)
                     dest_inputs = [dest_component_url]
-                    dest_inputs += get_dest_inputs(origin_input_code_run["inputs"], origin_uri, dest_uri, dest_token, origin_token, remote_label)
-                    sync_code_run(origin_uri, dest_uri, dest_token, origin_token, origin_input_code_run["uuid"], inputs= dest_inputs)
+                    dest_inputs += get_dest_inputs(origin_input_code_run["inputs"], origin_uri, dest_uri, dest_token, origin_token, remote_label, remote_author_url)
+                    sync_code_run(origin_uri, dest_uri, dest_token, origin_token, origin_input_code_run["uuid"], inputs= dest_inputs, remote_author_url = remote_author_url)
                 
                 origin_output_code_runs = fdp_req.get(
                         origin_uri,
                         "code_run",
                         origin_token,
                         params= {"outputs": fdp_req.get_obj_id_from_url(origin_component_url)}
                     )
                 for origin_output_code_run in origin_output_code_runs:
                     dest_component_url = get_dest_component_url(origin_component_url, dest_uri, dest_token, origin_token)
-                    dest_inputs = get_dest_inputs(origin_output_code_run["inputs"], origin_uri, dest_uri, dest_token, origin_token, remote_label, force)
-                    sync_code_run(origin_uri, dest_uri, dest_token, origin_token, origin_output_code_run["uuid"], inputs= dest_inputs, outputs= [dest_component_url])
+                    dest_inputs = get_dest_inputs(origin_output_code_run["inputs"], origin_uri, dest_uri, dest_token, origin_token, remote_label, force, remote_author_url)
+                    sync_code_run(origin_uri, dest_uri, dest_token, origin_token, origin_output_code_run["uuid"], inputs= dest_inputs, outputs= [dest_component_url], remote_author_url = remote_author_url)
                     
 def get_dest_component_url(
     origin_component_url: str,
     dest_uri: str,
     dest_token:str,
     origin_token:str) -> str:
     """Get the destination component url for the given origin component url
@@ -517,14 +572,15 @@
     dest_uri: str,
     dest_token: str,
     origin_token: str,
     remote_label: str,
     code_runs: typing.List[str],
     local_data_store: str = None,
     force: bool = False,
+    remote_author_url = None
 ) -> None:
     """Transfer data code_run(s) from one registry to another
 
     Parameters
     ----------
     origin_uri : str
         origin data registry URL
@@ -585,15 +641,16 @@
         sync_data_products(origin_uri,
             dest_uri,
             dest_token, 
             origin_token, 
             remote_label, 
             _origin_data_products_formatted, 
             local_data_store,
-            force)
+            force,
+            remote_author_url)
 
         # Iterate through formatted objects and get their new values from the remote registry
         for _origin_data_product_formatted in _origin_data_products_formatted:
             namespace, name, version = re.split("[:@]", _origin_data_product_formatted)
             # Get the destination namespace
             _dest_namespace = fdp_req.get(dest_uri, "namespace", dest_token, params={"name": namespace})
             if not _dest_namespace:
@@ -613,15 +670,15 @@
                 )
             _dest_object = fdp_req.url_get(_dest_data_product[0]["object"], dest_token)
             if _origin_data_product_formatted in _inputs_data_products:
                 _dest_inputs += _dest_object["components"]
             if _origin_data_product_formatted in _outputs_data_products:
                 _dest_outputs += _dest_object["components"]
         logger.debug(f'attempting to sync coderun {code_run_uuid} with inputs {_dest_inputs} and outputs {_dest_outputs}')
-        sync_code_run(origin_uri, dest_uri, dest_token, origin_token, code_run_uuid, _dest_inputs, _dest_outputs)
+        sync_code_run(origin_uri, dest_uri, dest_token, origin_token, code_run_uuid, _dest_inputs, _dest_outputs, remote_author_url = remote_author_url)
 
 # Internal function to return the (remote) object associated with a code_run field containing and object url
 def get_dest_object_url(
     origin_object_url: str,
     dest_uri: str,
     dest_token: str,
     origin_token: str)->str:
@@ -659,15 +716,16 @@
 def sync_code_run(
     origin_uri: str,
     dest_uri: str,
     dest_token: str,
     origin_token: str,
     code_run_uuid: str,
     inputs = [],
-    outputs = []) -> typing.Dict:
+    outputs = [],
+    remote_author_url = None) -> typing.Dict:
     """_summary_
 
     Args:
         origin_uri (str): Origin registry URL
         dest_uri (str): Destination registry URL
         dest_token (str): Destingation token
         origin_token (str): Origin token
@@ -706,38 +764,41 @@
         # Get and sync model config
         sync_dependency_chain(
         object_url=code_run["model_config"],
         dest_uri=dest_uri,
         origin_uri=origin_uri,
         dest_token=dest_token,
         origin_token=origin_token,
-        public= True
+        public= True,
+        remote_author_url = remote_author_url
         )
         _dest_code_run_model_config = get_dest_object_url(code_run["model_config"], dest_uri, dest_token, origin_token)
         upload_object(origin_uri, dest_uri, dest_token, origin_token, code_run["model_config"])
         # If theres a code_repo sync it
         _dest_code_run_code_repo = None
         if code_run["code_repo"]:
             sync_dependency_chain(
             object_url=code_run["code_repo"],
             dest_uri=dest_uri,
             origin_uri=origin_uri,
             dest_token=dest_token,
             origin_token=origin_token,
-            public= True
+            public= True,
+            remote_author_url = remote_author_url
             )
             _dest_code_run_code_repo = get_dest_object_url(code_run["code_repo"],  dest_uri, dest_token, origin_token)
         # Sync Submision Script
         sync_dependency_chain(
         object_url=code_run["submission_script"],
         dest_uri=dest_uri,
         origin_uri=origin_uri,
         dest_token=dest_token,
         origin_token=origin_token,
-        public= True
+        public= True,
+        remote_author_url = remote_author_url
         )
         _dest_code_run_submission_script = get_dest_object_url(code_run["submission_script"], dest_uri, dest_token, origin_token)
         upload_object(origin_uri, dest_uri, dest_token, origin_token, code_run["submission_script"])
 
         # If the code run is not in the remote registry post the coderun
         dest_code_run = fdp_req.post(dest_uri,
             "code_run",
@@ -824,15 +885,16 @@
 
 def get_dest_inputs(origin_inputs: typing.List, 
     origin_uri: str,
     dest_uri: str,
     dest_token: str,
     origin_token: str,
     remote_label: str,
-    force: bool = False) -> list:
+    force: bool = False,
+    remote_author_url = None) -> list:
     """Returns a list of input component urls on the destination registry
      from a given list of input component urls from the origin registry
      assumes the destination componets already exists in the remote registry
 
     Args:
         origin_inputs (typing.List): list of object_component urls from the origin registry
         origin_uri (str): Origin registry URL
@@ -845,28 +907,29 @@
     Returns:
         list: A list of destination input component URLS
     """
     dest_inputs = []
     for origin_input in origin_inputs:
         component_data_products = get_data_products_from_component(origin_input, origin_token)
         if component_data_products:
-            sync_data_products(origin_uri, dest_uri, dest_token, origin_token, remote_label, format_data_product_list(component_data_products, origin_token), force= force)
+            sync_data_products(origin_uri, dest_uri, dest_token, origin_token, remote_label, format_data_product_list(component_data_products, origin_token), force= force, remote_author_url = remote_author_url)
             for data_product_url in component_data_products:
                 origin_data_product_object_url = fdp_req.url_get(data_product_url, origin_token)["object"]
                 dest_object_url = get_dest_object_url(origin_data_product_object_url, dest_uri, dest_token, origin_token)
                 dest_object = fdp_req.url_get(dest_object_url, dest_token)
                 dest_inputs += (dest_object["components"])                             
         else:
             sync_dependency_chain(
                 object_url=origin_input,
                 dest_uri=dest_uri,
                 origin_uri=origin_uri,
                 dest_token=dest_token,
                 origin_token=origin_token,
-                public= is_component_public(origin_input, origin_token)
+                public= is_component_public(origin_input, origin_token),
+                remote_author_url = remote_author_url
                 )
             dest_inputs.append(get_dest_component_url(origin_input, dest_uri, dest_token, origin_token))
     return dest_inputs
 
 def fetch_data_product(
     remote_token: str, local_data_store: str, data_product: typing.Dict
 ) -> None:
@@ -1015,11 +1078,11 @@
     _object_storage_location = fdp_req.url_get(_object["storage_location"], origin_token)
     _object_storage_location_root = fdp_req.url_get(_object_storage_location["storage_root"], origin_token)
     _file_loc = download_from_registry(origin_uri, _object_storage_location_root["root"], _object_storage_location["path"])
     try:
         fdp_store.upload_remote_file(_file_loc, dest_uri, dest_token)
         logger.debug(f"File {_file_loc} Uploaded Successfully")
         return True
-    except Exception as e:
+    except Exception:
         logger.warning(f'File upload error: {_object["description"]} was not uploaded to remote registry please upload the file manually')
         logger.debug(f'{traceback.format_exc()}')
         return False
```

### Comparing `fair_cli-0.7.3/fair/registry/versioning.py` & `fair_cli-0.8.0/fair/registry/versioning.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.3/fair/run.py` & `fair_cli-0.8.0/fair/run.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.3/fair/session.py` & `fair_cli-0.8.0/fair/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -207,40 +207,40 @@
             fdp_com.find_fair_root(self._session_loc), fdp_com.FAIR_FOLDER
         )
         if os.path.exists(_root_dir):
             if verbose:
                 click.echo(f"Removing directory '{_root_dir}'")
             if platform.system() == "Windows":
                 fdp_com.set_file_permissions(_root_dir)
-            shutil.rmtree(_root_dir)
+            shutil.rmtree(_root_dir, onerror=fdp_com.remove_readonly)
         if clear_all:
             try:
                 if fdp_serv.check_server_running():
                     fdp_serv.stop_server()
             except (fdp_exc.FileNotFoundError, fdp_exc.CLIConfigurationError):
                 click.echo(
                     "Warning: Unable to check if server is running, "
                     "you may need to manually terminate the Django process"
                 )
             if verbose and os.path.exists(fdp_com.USER_FAIR_DIR):
                 click.echo(f"Removing directory '{fdp_com.USER_FAIR_DIR}'")
             if platform.system() == "Windows":
                 fdp_com.set_file_permissions(fdp_com.USER_FAIR_DIR)
-            shutil.rmtree(fdp_com.USER_FAIR_DIR)
+            shutil.rmtree(fdp_com.USER_FAIR_DIR, onerror=fdp_com.remove_readonly)
             return
         if clear_data:
             try:
                 if verbose and os.path.exists(fdp_com.default_data_dir()):
                     click.echo(
                         f"Removing directory '{fdp_com.default_data_dir()}'"
                     )
                 if os.path.exists(fdp_com.default_data_dir()):
                     if platform.system() == "Windows":
                         fdp_com.set_file_permissions(fdp_com.default_data_dir())
-                    shutil.rmtree(fdp_com.default_data_dir())
+                    shutil.rmtree(fdp_com.default_data_dir(), onerror=fdp_com.remove_readonly)
             except FileNotFoundError as e:
                 raise fdp_exc.FileNotFoundError(
                     "Cannot remove local data store, a global CLI configuration "
                     "is required to identify its location"
                 ) from e
 
         if global_cfg:
@@ -248,15 +248,15 @@
                 click.echo(
                     f"Removing directory '{fdp_com.global_config_dir()}'"
                 )
             _global_dirs = fdp_com.global_config_dir()
             if os.path.exists(_global_dirs):
                 if platform.system() == "Windows":
                         fdp_com.set_file_permissions(_global_dirs)
-                shutil.rmtree(_global_dirs)
+                shutil.rmtree(_global_dirs, onerror=fdp_com.remove_readonly)
 
     def _setup_server(self, port: int, address: str) -> None:
         """Start or stop the server if required"""
         self._logger.debug(
             f"Running server setup for run mode {self._run_mode}"
         )
         if self._run_mode == fdp_serv.SwitchMode.CLI:
@@ -356,15 +356,15 @@
 
         self._session_config.close_log()
 
     def registry_status(self):
         if fdp_serv.check_server_running():
             click.echo(f'Server running at: {fdp_conf.get_local_uri()}')
         else:
-            click.echo(f'Server is not running')
+            click.echo('Server is not running')
 
     def push(self, remote: str = "origin"):
         self._pre_job_setup(remote)
         self._session_config.prepare(
             fdp_com.CMD_MODE.PUSH, allow_dirty=self._allow_dirty
         )
         _staged_data_products = self._stager.get_item_list(
@@ -377,34 +377,57 @@
 
         if not _staged_data_products:
             click.echo("No Staged Data Products to Push.")
 
         if not _staged_code_runs:
             click.echo("No Staged Code Runs to Push.")
 
+        remote_author_url = fdp_sync.sync_author(
+            origin_uri=fdp_conf.get_local_uri(),
+            dest_uri=fdp_conf.get_remote_uri(self._session_loc, remote),
+            dest_token=fdp_conf.get_remote_token(
+                self._session_loc, remote, local=self._local
+            ),
+            origin_token=fdp_req.local_token(),
+            identifier= fdp_conf.get_current_user_uri(self._session_loc)
+        )
+
+        fdp_sync.sync_user_author(
+            origin_uri=fdp_conf.get_local_uri(),
+            dest_uri=fdp_conf.get_remote_uri(self._session_loc, remote),
+            dest_token=fdp_conf.get_remote_token(
+                self._session_loc, remote, local=self._local
+            ),
+            origin_token=fdp_req.local_token(),
+            author_url = remote_author_url,
+            github = fdp_conf.get_current_user_github(self._session_loc)
+        )
+
         fdp_sync.sync_code_runs(
             origin_uri=fdp_conf.get_local_uri(),
             dest_uri=fdp_conf.get_remote_uri(self._session_loc, remote),
             dest_token=fdp_conf.get_remote_token(
                 self._session_loc, remote, local=self._local
             ),
             origin_token=fdp_req.local_token(),
             remote_label=remote,
             code_runs=_staged_code_runs,
+            remote_author_url = remote_author_url
         )
 
         fdp_sync.sync_data_products(
             origin_uri=fdp_conf.get_local_uri(),
             dest_uri=fdp_conf.get_remote_uri(self._session_loc, remote),
             dest_token=fdp_conf.get_remote_token(
                 self._session_loc, remote, local=self._local
             ),
             origin_token=fdp_req.local_token(),
             remote_label=remote,
             data_products=_staged_data_products,
+            remote_author_url = remote_author_url
         )
 
         self._session_config.write_log_lines(
             [f"Pushing code_run(s) to remote '{remote}':"]
             + [f"\t- {code_run}" for code_run in _staged_code_runs]
         )
 
@@ -893,15 +916,15 @@
                 _remote_code_run = fdp_req.get(
                     fdp_conf.get_remote_uri(self._session_loc, label),
                     "code_run",
                     fdp_conf.get_remote_token(self._session_loc, label, local=self._local),
                     params={"uuid": uuid})
                 if _remote_code_run:
                     return _remote_code_run[0]["description"]
-        except Exception as e:
+        except Exception:
             pass
         return "Unknown"
 
     def show_code_runs(
         self, code_runs: typing.List[str], title: str, style="green"
     ) -> None:
         console = Console()
@@ -939,15 +962,15 @@
                     fdp_conf.get_remote_uri(self._session_loc, remote),
                     "code_run",
                     fdp_conf.get_remote_token(self._session_loc, remote, local=self._local),
                     )
                 if _remote_code_runs:
                     for _remote_code_run in _remote_code_runs:
                         _code_run_uuids.append(_remote_code_run["uuid"])
-            except Exception as e:
+            except Exception:
                 self._logger.warning("Could not Fetch from a remote registry")
                 self._logger.debug(f'{traceback.format_exc()}')
         _code_run_uuids = list(set(_code_run_uuids))
         return self.show_code_runs(_code_run_uuids, _title)
 
     def show_all_data_products(self, remote: str = None):
         _title = "Local Data Products"
@@ -965,15 +988,15 @@
                     "data_product",
                     fdp_conf.get_remote_token(self._session_loc, remote, local=self._local),
                     )
                 if _remote_data_products:
                     for remote_data_product in _remote_data_products:
                         _namespace_name = fdp_req.url_get(remote_data_product["namespace"], fdp_conf.get_remote_token(self._session_loc, remote, local=self._local))["name"]
                         _data_products.append(f'{_namespace_name}:{remote_data_product["name"]}@v{remote_data_product["version"]}')
-            except Exception as e:
+            except Exception:
                 self._logger.warning("Could not Fetch from a remote registry")
                 self._logger.debug(f'{traceback.format_exc()}')
         _data_products = list(set(_data_products))
         return self.show_data_products(_data_products, _title)
 
     def status_jobs(self, verbose: bool = False) -> None:
         """Get the staging status of jobs"""
@@ -1080,15 +1103,15 @@
 
     # noqa: C901
     def initialise(
         self,
         using: typing.Dict = None,
         registry: str = None,
         export_as: str = None,
-        local: bool = False,
+        local: bool = False
     ) -> None:
         """Initialise an fair repository within the current location
 
         Parameters
         ----------
         using : str
             load from an existing global CLI configuration file
@@ -1096,87 +1119,97 @@
         _fair_dir = os.path.abspath(
             os.path.join(self._session_loc, fdp_com.FAIR_FOLDER)
         )
 
         _first_time = not os.path.exists(fdp_com.global_fdpconfig())
 
         if self._testing:
+            if os.path.exists(_fair_dir):
+                if platform.system() == "Windows":
+                    fdp_com.set_file_permissions(_fair_dir)
+                shutil.rmtree(_fair_dir, onerror=fdp_com.remove_readonly)
             using = fdp_test.create_configurations(
                 registry,
                 fdp_com.find_git_root(os.getcwd()),
                 os.getcwd(),
-                os.path.join(os.getcwd(), "data_store"),
+                os.path.join(os.getcwd(), ".fair"),
             )
 
-        if os.path.exists(_fair_dir):
+        if os.path.exists(_fair_dir) and not self._testing:
             if export_as:
                 self._export_cli_configuration(export_as)
                 return
-            click.echo("FAIR repository is already initialised.")
-            return
+            else:
+                click.echo("FAIR repository is already initialised.")
+                return
 
-        if _existing := fdp_com.find_fair_root(self._session_loc):
+        if _existing := fdp_com.find_fair_root(self._session_loc) and not self._testing:
             click.echo(
                 "A FAIR repository was initialised for this location at"
                 f" '{_existing}'"
             )
             _confirm = click.confirm("Do you want to continue?", default=False)
             if not _confirm:
                 click.echo("Aborted intialisation.")
                 return
 
         if not using:
             click.echo(
                 "Initialising FAIR repository, setup will now ask for basic info (leave blank for default value):\n"
             )
 
-        if not os.path.exists(_fair_dir):
-            os.mkdir(_fair_dir)
+        if not os.path.exists(_fair_dir) or self._testing:
+            os.makedirs(_fair_dir, exist_ok=True)
             os.makedirs(fdp_com.session_cache_dir(), exist_ok=True)
             if using:
                 self._validate_and_load_cli_config(using)
             self._stager.initialise()
 
         if not os.path.exists(fdp_com.global_fdpconfig()):
             try:
+                click.echo("Setup will now ask you questions regarding the global configuration")
                 self._global_config = fdp_conf.global_config_query(
                     registry, local
                 )
             except (fdp_exc.CLIConfigurationError, click.Abort) as e:
                 self._clean_reset(_fair_dir, e)
             try:
+                click.echo("Setup will now ask you questions regarding this repo configuration")
                 self._local_config = fdp_conf.local_config_query(
                     self._global_config,
                     first_time_setup=_first_time,
                     local=local,
                 )
             except (fdp_exc.CLIConfigurationError, click.Abort) as e:
                 self._clean_reset(_fair_dir, e, True)
         elif not using:
             try:
+                click.echo("Setup will now ask you questions regarding this repo configuration")
                 self._local_config = fdp_conf.local_config_query(
                     self._global_config, local=local
                 )
             except (fdp_exc.CLIConfigurationError, click.Abort) as e:
                 self._clean_reset(_fair_dir, e, True)
         if not using:
             with open(fdp_com.local_fdpconfig(self._session_loc), "w") as f:
                 yaml.dump(self._local_config, f)
             with open(fdp_com.global_fdpconfig(), "w") as f:
                 yaml.dump(self._global_config, f)
         else:
+            click.echo("Setup will now ask you questions regarding the global configuration")
             self._global_config = fdp_conf.read_global_fdpconfig()
+            click.echo("Setup will now ask you questions regarding this repo configuration")
             self._local_config = fdp_conf.read_local_fdpconfig(
                 self._session_loc
             )
 
         if export_as:
             self._export_cli_configuration(export_as)
 
-        fdp_serv.update_registry_post_setup(self._session_loc, _first_time)
+        fdp_serv.update_registry_post_setup(self._session_loc, _first_time, registry)
         try:
             fdp_clivalid.LocalCLIConfig(**self._local_config)
         except pydantic.ValidationError as e:
             self._logger.debug(f"Local CLI validator returned: {e.json()}")
             self._clean_reset(_fair_dir, local_only=True)
             raise fdp_exc.InternalError(
                 "Initialisation failed, validation of local CLI config file did not pass"
@@ -1199,20 +1232,20 @@
 
     def _clean_reset(
         self, _fair_dir, e: Exception = None, local_only: bool = False
     ):
         if not local_only:
             if platform.system() == "Windows":
                 fdp_com.set_file_permissions(fdp_com.session_cache_dir())
-                fdp_com.set_file_permissions(fdp_com.fdp_com.global_config_dir())
-            shutil.rmtree(fdp_com.session_cache_dir(), ignore_errors=True)
-            shutil.rmtree(fdp_com.global_config_dir(), ignore_errors=True)
+                fdp_com.set_file_permissions(fdp_com.global_config_dir())
+            shutil.rmtree(fdp_com.session_cache_dir(), onerror=fdp_com.remove_readonly)
+            shutil.rmtree(fdp_com.global_config_dir(), onerror=fdp_com.remove_readonly)
         if platform.system() == "Windows":
             fdp_com.set_file_permissions(_fair_dir)
-        shutil.rmtree(_fair_dir)
+        shutil.rmtree(_fair_dir, onerror=fdp_com.remove_readonly)
         if e:
             raise e
 
     def close_session(self) -> None:
         """Upon exiting, dump all configurations to file"""
         if not os.path.exists(
             os.path.join(self._session_loc, fdp_com.FAIR_FOLDER)
@@ -1267,26 +1300,26 @@
                     "in CLI configuration"
                 )
             if name == "local" and "directory" not in reg:
                 raise fdp_exc.CLIConfigurationError(
                     "Expected key 'directory' for local registry in CLI configuration"
                 )
 
-        _user_keys = ["email", "family_name", "given_names", "orcid", "uuid"]
+        _user_keys = ["email", "family_name", "given_names", "uuid", "github"]
 
         for key in _user_keys:
             if key not in cli_config["user"]:
                 self.purge(verbose=False)
                 raise fdp_exc.CLIConfigurationError(
                     f"Expected key 'user:{key}' in CLI configuration file"
                 )
 
-        if not cli_config["user"]["orcid"] and not cli_config["user"]["uuid"]:
+        if not cli_config["user"]["github"] and not cli_config["user"]["uuid"]:
             raise fdp_exc.CLIConfigurationError(
-                "At least one of 'user:orcid' and 'user:uuid' must be provided "
+                "At least one of 'user:github' and 'user:uuid' must be provided "
                 " in CLI configuration"
             )
 
         for key in ["local_repo", "remote"]:
             if key not in cli_config["git"]:
                 self.purge(verbose=False)
                 raise fdp_exc.CLIConfigurationError(
```

### Comparing `fair_cli-0.7.3/fair/staging.py` & `fair_cli-0.8.0/fair/staging.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.3/fair/testing.py` & `fair_cli-0.8.0/fair/testing.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 def create_configurations(
     registry_dir: str,
     local_git_dir: typing.Optional[str] = None,
     remote_reg_dir: typing.Optional[str] = None,
     testing_dir: str = tempfile.mkdtemp(),
-    tokenless: bool = False,
+    tokenless: bool = False
 ) -> typing.Dict:
     """
     Setup CLI for testing
 
     Running without a token limits the functionality, this should only be used
     when testing without need to access a local registry.
 
@@ -76,16 +76,17 @@
             },
         },
         "user": {
             "email": "test@noreply.com",
             "family_name": "Test",
             "given_names": "Interface",
             "orcid": "000-0000-0000-0000",
-            "uri": f'{fdp_id.ID_URIS["orcid"]}000-0000-0000-0000',
+            "uri": f'{fdp_id.ID_URIS["github"]}FAIRDataPipeline',
             "uuid": "2ddb2358-84bf-43ff-b2aa-3ac7dc3b49f1",
+            "github": "FAIRDataPipeline"
         },
         "git": {
             "local_repo": local_git_dir,
             "remote": "origin",
             "remote_repo": "git@notagit.com/user/project.git",
         },
     }
```

### Comparing `fair_cli-0.7.3/fair/user_config/__init__.py` & `fair_cli-0.8.0/fair/user_config/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,14 +328,22 @@
         Checks namespace listed in 'namespace_name' if given, if there is a
         match the entry is removed and replaced with a 'use:namespace' entry
         """
         _new_register_block: typing.List[typing.Dict] = []
         for register_entry in register_block:
             _new_entry = register_entry.copy()
             if "namespace_name" not in register_entry:
+                if not "use" in register_entry:
+                    _new_entry["use"] = {}
+                else:
+                    if "namespace" in register_entry["use"]:
+                        _new_entry["use"]["namespace"] = register_entry["use"]["namespace"]
+                    else:
+                        _new_entry["use"]["namespace"] = self.default_input_namespace
+                _new_register_block.append(_new_entry)
                 continue
             if (
                 register_entry["namespace_name"]
                 not in self._parsed["namespace"]
             ):
                 self._logger.error(
                     "'%s' not in available namespaces:\n\t-%s",
```

### Comparing `fair_cli-0.7.3/fair/user_config/globbing.py` & `fair_cli-0.8.0/fair/user_config/globbing.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.3/fair/user_config/validation.py` & `fair_cli-0.8.0/fair/user_config/validation.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.3/fair/utilities.py` & `fair_cli-0.8.0/fair/utilities.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.3/fair/virtualenv.py` & `fair_cli-0.8.0/fair/virtualenv.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.3/pyproject.toml` & `fair_cli-0.8.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   "Environment :: Console",
   "Operating System :: POSIX :: Linux",
   "Operating System :: MacOS",
   "Operating System :: OS Independent",
 ]
 description = "Synchronization interface for the SCRC FAIR Data Pipeline registry"
 name = "fair-cli"
-version = "0.7.3"
+version = "0.8.0"
 
 homepage = "https://www.fairdatapipeline.org/"
 
 repository = "https://github.com/FAIRDataPipeline/FAIR-CLI"
 
 documentation = "https://www.fairdatapipeline.org/docs/interface/fdp/"
 
@@ -60,46 +60,45 @@
 python = "^3.8.0,<4.0"
 requests = "^2.23.0"
 rich = ">=10.2.3,<12.0.0"
 semver = "^2.13.0"
 simplejson = "^3.17.5"
 toml = "^0.10.2"
 validators = "^0.18.2"
-netCDF4 = "^1.5.8"
+fake-useragent = "^1"
 
 [tool.poetry.dev-dependencies]
-bandit = "^1.7.2"
-black = "^22.1"
-coverage = "^6.3"
+bandit = "*"
+black = "*"
+coverage = "7.2.*"
 deepdiff = "^5.5.0"
-flake8 = "^3.9.2"
+flake8 = "*"
 isort = "^5.10.1"
-loremipsum = "^1.0.5"
 mypy = "^0.931"
 poetry = "^1.1.12"
-pre-commit = "^2.16.0"
+pre-commit = "^2.17.0"
 pycodestyle = "^2.7.0"
 pydocstyle = "^6.0.0"
 pylama = "^7.7.1"
-pytest = "^7.0.0"
-pytest-cov = "^4.0.0"
-pytest-dependency = "^0.5.1"
-pytest-mock = "^3.7.0"
-pytest-virtualenv = "^1.7.0"
-requests-mock = "^1.9.3"
+pytest = "*"
+pytest-cov = "*"
+pytest-dependency = "*"
+pytest-mock = "*"
+pytest-virtualenv = "*"
+requests-mock = "*"
 boto3 = "^1.24"
 moto = "^4.0.3"
 Flask = "^2.2.2"
 Flask-Cors = "^3.0.10"
 
 [tool.poetry.scripts]
 fair = 'fair.cli:cli'
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry>=1.0.0"]
 
 [tool.poetry.urls]
 "Issue Tracker" = "https://github.com/FAIRDataPipeline/FAIR-CLI/issues"
 
 [tool.poetry.extras]
 all = ["moto"]
```

### Comparing `fair_cli-0.7.3/PKG-INFO` & `fair_cli-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fair-cli
-Version: 0.7.3
+Version: 0.8.0
 Summary: Synchronization interface for the SCRC FAIR Data Pipeline registry
 Home-page: https://www.fairdatapipeline.org/
 License: BSD-2-Clause
 Keywords: FAIR Data Pipeline,FAIR,Data Management,Provenance
 Author: Richard Reeve
 Author-email: richard.reeve@glasgow.ac.uk
 Requires-Python: >=3.8.0,<4.0.0
@@ -25,15 +25,15 @@
 Classifier: Topic :: Scientific/Engineering
 Provides-Extra: all
 Requires-Dist: GitPython (>=3.1.18,<4.0.0)
 Requires-Dist: Jinja2 (>=3.0.1,<4.0.0)
 Requires-Dist: PyYAML (>=5.4.1,<7.0.0)
 Requires-Dist: click (>=8.0.0,<9.0.0)
 Requires-Dist: email-validator (>=1.1.3,<2.0.0)
-Requires-Dist: netCDF4 (>=1.5.8,<2.0.0)
+Requires-Dist: fake-useragent (>=1,<2)
 Requires-Dist: pre-commit (>=2.15.0,<3.0.0)
 Requires-Dist: pydantic[email] (>=1.9.0,<2.0.0)
 Requires-Dist: requests (>=2.23.0,<3.0.0)
 Requires-Dist: rich (>=10.2.3,<12.0.0)
 Requires-Dist: semver (>=2.13.0,<3.0.0)
 Requires-Dist: simplejson (>=3.17.5,<4.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
```

