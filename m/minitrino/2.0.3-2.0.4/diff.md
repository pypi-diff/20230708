# Comparing `tmp/minitrino-2.0.3.tar.gz` & `tmp/minitrino-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minitrino-2.0.3.tar", last modified: Fri Apr 28 21:32:16 2023, max compression
+gzip compressed data, was "minitrino-2.0.4.tar", last modified: Sat Jul  8 20:15:09 2023, max compression
```

## Comparing `minitrino-2.0.3.tar` & `minitrino-2.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jlester    (503) staff       (20)        0 2023-04-28 21:32:16.331374 minitrino-2.0.3/
--rw-r--r--   0 jlester    (503) staff       (20)    31768 2023-04-28 21:32:16.331204 minitrino-2.0.3/PKG-INFO
-drwxr-xr-x   0 jlester    (503) staff       (20)        0 2023-04-28 21:32:16.329030 minitrino-2.0.3/minitrino/
--rw-r--r--   0 jlester    (503) staff       (20)        0 2023-01-12 16:45:57.000000 minitrino-2.0.3/minitrino/__init__.py
--rw-r--r--   0 jlester    (503) staff       (20)     1977 2023-01-12 16:45:57.000000 minitrino-2.0.3/minitrino/cli.py
-drwxr-xr-x   0 jlester    (503) staff       (20)        0 2023-04-28 21:32:16.330984 minitrino-2.0.3/minitrino/cmd/
--rw-r--r--   0 jlester    (503) staff       (20)        0 2023-01-12 16:45:57.000000 minitrino-2.0.3/minitrino/cmd/__init__.py
--rw-r--r--   0 jlester    (503) staff       (20)     2368 2023-01-12 16:45:57.000000 minitrino-2.0.3/minitrino/cmd/cmd_config.py
--rw-r--r--   0 jlester    (503) staff       (20)     2194 2023-01-12 16:45:57.000000 minitrino-2.0.3/minitrino/cmd/cmd_down.py
--rw-r--r--   0 jlester    (503) staff       (20)     2971 2023-04-17 15:08:13.000000 minitrino-2.0.3/minitrino/cmd/cmd_lib_install.py
--rw-r--r--   0 jlester    (503) staff       (20)     2291 2023-04-28 18:26:59.000000 minitrino-2.0.3/minitrino/cmd/cmd_modules.py
--rw-r--r--   0 jlester    (503) staff       (20)    26055 2023-04-28 17:43:50.000000 minitrino-2.0.3/minitrino/cmd/cmd_provision.py
--rw-r--r--   0 jlester    (503) staff       (20)     4058 2023-01-12 16:45:57.000000 minitrino-2.0.3/minitrino/cmd/cmd_remove.py
--rw-r--r--   0 jlester    (503) staff       (20)    13142 2023-04-28 16:41:24.000000 minitrino-2.0.3/minitrino/cmd/cmd_snapshot.py
--rw-r--r--   0 jlester    (503) staff       (20)      642 2023-01-12 16:45:57.000000 minitrino-2.0.3/minitrino/cmd/cmd_version.py
--rw-r--r--   0 jlester    (503) staff       (20)    30017 2023-04-28 17:40:12.000000 minitrino-2.0.3/minitrino/components.py
--rw-r--r--   0 jlester    (503) staff       (20)      987 2023-01-12 16:45:57.000000 minitrino-2.0.3/minitrino/errors.py
--rw-r--r--   0 jlester    (503) staff       (20)     1656 2023-04-27 23:02:35.000000 minitrino-2.0.3/minitrino/settings.py
--rw-r--r--   0 jlester    (503) staff       (20)    11306 2023-04-17 15:08:13.000000 minitrino-2.0.3/minitrino/utils.py
-drwxr-xr-x   0 jlester    (503) staff       (20)        0 2023-04-28 21:32:16.329836 minitrino-2.0.3/minitrino.egg-info/
--rw-r--r--   0 jlester    (503) staff       (20)    31768 2023-04-28 21:32:16.000000 minitrino-2.0.3/minitrino.egg-info/PKG-INFO
--rw-r--r--   0 jlester    (503) staff       (20)      592 2023-04-28 21:32:16.000000 minitrino-2.0.3/minitrino.egg-info/SOURCES.txt
--rw-r--r--   0 jlester    (503) staff       (20)        1 2023-04-28 21:32:16.000000 minitrino-2.0.3/minitrino.egg-info/dependency_links.txt
--rw-r--r--   0 jlester    (503) staff       (20)       49 2023-04-28 21:32:16.000000 minitrino-2.0.3/minitrino.egg-info/entry_points.txt
--rw-r--r--   0 jlester    (503) staff       (20)       43 2023-04-28 21:32:16.000000 minitrino-2.0.3/minitrino.egg-info/requires.txt
--rw-r--r--   0 jlester    (503) staff       (20)       10 2023-04-28 21:32:16.000000 minitrino-2.0.3/minitrino.egg-info/top_level.txt
--rw-r--r--   0 jlester    (503) staff       (20)       38 2023-04-28 21:32:16.331430 minitrino-2.0.3/setup.cfg
--rw-r--r--   0 jlester    (503) staff       (20)     1110 2023-04-28 21:30:48.000000 minitrino-2.0.3/setup.py
+drwxr-xr-x   0 jlester    (503) staff       (20)        0 2023-07-08 20:15:09.869463 minitrino-2.0.4/
+-rw-r--r--   0 jlester    (503) staff       (20)    22719 2023-07-08 20:15:09.869234 minitrino-2.0.4/PKG-INFO
+drwxr-xr-x   0 jlester    (503) staff       (20)        0 2023-07-08 20:15:09.864033 minitrino-2.0.4/minitrino/
+-rw-r--r--   0 jlester    (503) staff       (20)        0 2023-01-12 16:45:57.000000 minitrino-2.0.4/minitrino/__init__.py
+-rw-r--r--   0 jlester    (503) staff       (20)     1977 2023-01-12 16:45:57.000000 minitrino-2.0.4/minitrino/cli.py
+drwxr-xr-x   0 jlester    (503) staff       (20)        0 2023-07-08 20:15:09.868618 minitrino-2.0.4/minitrino/cmd/
+-rw-r--r--   0 jlester    (503) staff       (20)        0 2023-01-12 16:45:57.000000 minitrino-2.0.4/minitrino/cmd/__init__.py
+-rw-r--r--   0 jlester    (503) staff       (20)     2302 2023-07-08 08:22:32.000000 minitrino-2.0.4/minitrino/cmd/cmd_config.py
+-rw-r--r--   0 jlester    (503) staff       (20)     2118 2023-07-08 08:17:26.000000 minitrino-2.0.4/minitrino/cmd/cmd_down.py
+-rw-r--r--   0 jlester    (503) staff       (20)     2887 2023-07-08 08:22:55.000000 minitrino-2.0.4/minitrino/cmd/cmd_lib_install.py
+-rw-r--r--   0 jlester    (503) staff       (20)     2294 2023-07-08 08:18:05.000000 minitrino-2.0.4/minitrino/cmd/cmd_modules.py
+-rw-r--r--   0 jlester    (503) staff       (20)    23055 2023-07-08 18:07:18.000000 minitrino-2.0.4/minitrino/cmd/cmd_provision.py
+-rw-r--r--   0 jlester    (503) staff       (20)     3908 2023-07-08 08:21:18.000000 minitrino-2.0.4/minitrino/cmd/cmd_remove.py
+-rw-r--r--   0 jlester    (503) staff       (20)    12933 2023-07-08 18:28:34.000000 minitrino-2.0.4/minitrino/cmd/cmd_snapshot.py
+-rw-r--r--   0 jlester    (503) staff       (20)      645 2023-07-08 08:22:19.000000 minitrino-2.0.4/minitrino/cmd/cmd_version.py
+-rw-r--r--   0 jlester    (503) staff       (20)    29740 2023-07-08 08:38:32.000000 minitrino-2.0.4/minitrino/components.py
+-rw-r--r--   0 jlester    (503) staff       (20)      987 2023-01-12 16:45:57.000000 minitrino-2.0.4/minitrino/errors.py
+-rw-r--r--   0 jlester    (503) staff       (20)     1746 2023-07-08 02:13:25.000000 minitrino-2.0.4/minitrino/settings.py
+-rw-r--r--   0 jlester    (503) staff       (20)    11894 2023-07-08 08:32:25.000000 minitrino-2.0.4/minitrino/utils.py
+drwxr-xr-x   0 jlester    (503) staff       (20)        0 2023-07-08 20:15:09.865391 minitrino-2.0.4/minitrino.egg-info/
+-rw-r--r--   0 jlester    (503) staff       (20)    22719 2023-07-08 20:15:09.000000 minitrino-2.0.4/minitrino.egg-info/PKG-INFO
+-rw-r--r--   0 jlester    (503) staff       (20)      592 2023-07-08 20:15:09.000000 minitrino-2.0.4/minitrino.egg-info/SOURCES.txt
+-rw-r--r--   0 jlester    (503) staff       (20)        1 2023-07-08 20:15:09.000000 minitrino-2.0.4/minitrino.egg-info/dependency_links.txt
+-rw-r--r--   0 jlester    (503) staff       (20)       48 2023-07-08 20:15:09.000000 minitrino-2.0.4/minitrino.egg-info/entry_points.txt
+-rw-r--r--   0 jlester    (503) staff       (20)       43 2023-07-08 20:15:09.000000 minitrino-2.0.4/minitrino.egg-info/requires.txt
+-rw-r--r--   0 jlester    (503) staff       (20)       10 2023-07-08 20:15:09.000000 minitrino-2.0.4/minitrino.egg-info/top_level.txt
+-rw-r--r--   0 jlester    (503) staff       (20)       38 2023-07-08 20:15:09.869516 minitrino-2.0.4/setup.cfg
+-rw-r--r--   0 jlester    (503) staff       (20)     1110 2023-07-08 02:13:25.000000 minitrino-2.0.4/setup.py
```

### Comparing `minitrino-2.0.3/PKG-INFO` & `minitrino-2.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,447 +1,232 @@
 Metadata-Version: 2.1
 Name: minitrino
-Version: 2.0.3
+Version: 2.0.4
 Summary: A command line tool that makes it easy to run modular Trino environments locally.
 Home-page: https://github.com/jefflester/minitrino
 Author: Jeff Lester
 Author-email: jeff.lester.dev@gmail.com
 License: Apache-2.0
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Minitrino
 
 A command line tool that makes it easy to run modular Trino environments
-locally. Compatible with Starburst versions 370-e and later.
+locally. Compatible with Starburst versions 388-e and later.
 
 [![PyPI
 version](https://badge.fury.io/py/minitrino.svg)](https://badge.fury.io/py/minitrino)
-[![Build
-Status](https://app.travis-ci.com/jefflester/minitrino.svg?branch=master)](https://app.travis-ci.com/jefflester/minitrino)
+![Build
+Status](https://github.com/jefflester/minitrino/actions/workflows/tests.yml/badge.svg)
 [![Trino
 Slack](https://img.shields.io/static/v1?logo=slack&logoColor=959DA5&label=Slack&labelColor=333a41&message=join%20conversation&color=3AC358)](https://trinodb.io/slack.html)
 
 -----
 
-**Latest Stable Release**: 2.0.3
+**Latest Stable Release**: 2.0.4
 
 -----
 
 ## Overview
 
 - [Minitrino](#minitrino)
   - [Overview](#overview)
   - [Requirements](#requirements)
-  - [Installation](#installation)
+  - [Installation and Upgrades](#installation-and-upgrades)
     - [End Users](#end-users)
     - [Developers](#developers)
-  - [CLI](#cli)
-    - [Top-Level CLI Options](#top-level-cli-options)
-    - [Provisioning Environments](#provisioning-environments)
-      - [Environment Variables](#environment-variables)
-      - [Using Licensed Starburst Features](#using-licensed-starburst-features)
-    - [Removing Resources](#removing-resources)
-    - [Shutting Down Environments](#shutting-down-environments)
-    - [Taking Environment Snapshots](#taking-environment-snapshots)
-    - [Manage User Configuration](#manage-user-configuration)
-    - [Install the Library](#install-the-library)
-    - [Display Module Metadata](#display-module-metadata)
-    - [Display Minitrino Versions](#display-minitrino-versions)
-    - [Pointing the CLI to the Minitrino Library](#pointing-the-cli-to-the-minitrino-library)
+    - [Using Colima and Other Docker Contexts](#using-colima-and-other-docker-contexts)
+    - [End User Upgrades](#end-user-upgrades)
+  - [Workflow Examples](#workflow-examples)
+    - [Provision an Environment](#provision-an-environment)
+    - [Modify Files in a Running Container](#modify-files-in-a-running-container)
+    - [Shut Down an Environment](#shut-down-an-environment)
+    - [Remove Minitrino Resources](#remove-minitrino-resources)
+    - [Snapshot a Customized Module](#snapshot-a-customized-module)
   - [Minitrino Configuration File](#minitrino-configuration-file)
     - [\[CLI\] Section](#cli-section)
     - [\[MODULES\] Section](#modules-section)
   - [Project Structure](#project-structure)
     - [Trino Dockerfile](#trino-dockerfile)
-  - [Adding New Modules (Tutorial)](#adding-new-modules-tutorial)
+  - [Add New Modules (Tutorial)](#add-new-modules-tutorial)
     - [Create the Module Directory](#create-the-module-directory)
     - [Add Trino Resources](#add-trino-resources)
     - [Add the Docker Compose YAML](#add-the-docker-compose-yaml)
     - [Add a Metadata File](#add-a-metadata-file)
     - [Add a Readme File](#add-a-readme-file)
     - [Review Progress](#review-progress)
     - [Configure the Docker Compose YAML File](#configure-the-docker-compose-yaml-file)
     - [Important Implementation Details: Paths and Labels](#important-implementation-details-paths-and-labels)
       - [Path References for Volumes and Build Contexts](#path-references-for-volumes-and-build-contexts)
       - [Minitrino Docker Labels](#minitrino-docker-labels)
     - [Test the New Catalog](#test-the-new-catalog)
-    - [Customizing Images](#customizing-images)
     - [Bootstrap Scripts](#bootstrap-scripts)
       - [Installing Shell Packages for Bootstrap Scripts](#installing-shell-packages-for-bootstrap-scripts)
     - [Managing Trino's `config.properties` and `jvm.config` Files](#managing-trinos-configproperties-and-jvmconfig-files)
+      - [Preferable Method: Environment Variables](#preferable-method-environment-variables)
+      - [Secondary Method: Bootstrap Scripts](#secondary-method-bootstrap-scripts)
   - [Troubleshooting](#troubleshooting)
   - [Reporting Bugs and Contributing](#reporting-bugs-and-contributing)
 
 -----
 
 ## Requirements
 
-- Docker 19.03.0+
-- Docker Compose (1.29.0+)
-- Python 3.8+
+- Docker Desktop >= 3.5
+- Python >= 3.8
 - Pip
-- Linux or Mac OS
+- Linux / MacOS
 
 -----
 
-## Installation
+## Installation and Upgrades
 
 ### End Users
 
 Minitrino is available on PyPI and the library is available for public download
-on GitHub. To install the Minitrino CLI, run `pip install minitrino`. To install
-the library, run `minitrino lib_install`.
+on GitHub. To set everything up, run:
 
-### Developers
-
-In the project's root, run `./install.sh` to install the Minitrino CLI. If you
-encounter errors during installation, try running `sudo -H ./install.sh -v`.
-
------
-
-## CLI
-
-Minitrino is built with [Click](https://click.palletsprojects.com/en/7.x/), a
-popular, open-source toolkit used to build Python-based CLIs.
-
-All Minitrino commands/options are documented below. Note that many command
-options can be specified with a shorthand alternative, which is the first letter
-of each option, i.e. `--module` can be `-m`.
-
-### Top-Level CLI Options
-
-You can get help, enable verbose output, and change the runtime library
-directory for any command.
-
-```
-Usage: minitrino [OPTIONS] COMMAND [ARGS]...
-
-Options:
-  -v, --verbose   Enable verbose output.
-  -e, --env TEXT  Add or override environment variables.
-                  
-                  Environment variables are sourced from the Minitrino
-                  library's root 'minitrino.env' file as well as the user 
-                  config file in '~/.minitrino/minitrino.cfg'. Variables 
-                  supplied by this option will override values from either 
-                  of those sources. The variables will also be passed to the
-                  environment of the shell executing commands during the
-                  'provision' command.
-
-  --help          Show this message and exit.
-```
-
-### Provisioning Environments
-
-You can provision an environment via the `provision` command.
-
-```
-Usage: minitrino provision [OPTIONS]
-
-  Provision an environment based on specified modules. All options are
-  optional and can be left empty.
-
-Options:
-  -m, --module TEXT         A specific module to provision.
-  -n, --no-rollback         Do not rollback provisioned resources in the event
-                            of an error.
-
-  -d, --docker-native TEXT  Appends native docker-compose commands to the
-                            generated docker-compose shell command. Run
-                            `docker-compose up --help` to see all available
-                            options.
-                            
-                            Example: minitrino provision --docker-native
-                            --build
-                            
-                            Example: minitrino provision --docker-native '--
-                            remove-orphans --force-recreate'
-
-  --help                    Show this message and exit.
-```
-
-Notes:
-
-- If no options are passed in, the CLI will provision a standalone Trino
-  container.
-- The command cannot currently be used to append additional modules to an active
-  environment. To modify an environment, first shut it down, then re-provision
-  with the needed modules.
-
-Sample `provision` commands:
-
-```bash
-minitrino provision \
-  --module hive \
-  --module elasticsearch \
-  --module ldap \
-  --docker-native '--build --force-recreate'
-
-minitrino provision -m hive -m elasticsearch -m ldap
-
-minitrino --env STARBURST_VER=411-e provision
-```
-
-The `provision` command constructs a Docker Compose command and executes it in
-the host shell. The commands look similar to:
-
-```bash
-ENV_VAR_1=SOMETHING ENV_VAR_2=SOMETHING ENV_VAR_3=${ENV_VAR_3} ... \
-docker-compose -f docker-compose.yml \
-  -f modules/catalog/elasticsearch/elasticsearch.yml \
-  -f modules/catalog/hive/hive.yml \
-  -f modules/security/ldap/ldap.yml \
-  up -d
-```
-
-Using the structure of the Minitrino library, it is able to merge multiple
-Docker Compose files together.
-
-#### Environment Variables
-
-Environment variables passed to Docker containers are sourced through two
-locations. The first is from the `minitrino.env` file in the library root. These
-variables define the versions of the provisioned Docker services. The second is
-from from variables set in the `[MODULES]` section of the `minitrino.cfg` file.
-These variables can contain sensitive information like access credentials, so
-their values are intentionally left out of library files.
-
-Any existing environment variable can be overridden with the top-level `--env`
-option, and any unset variable can be set with it.
-
-#### Using Licensed Starburst Features
-
-If you are using licensed features, you will need to provide a path to a valid
-Starburst license. This can be set via `minitrino config` or provided via the
-`--env` option at command runtime. The variable for this is
-`STARBURST_LIC_PATH`.
-
-Additionally, you need to uncomment the volume mount in the library's root
-`docker-compose.yml` file:
-
-```yaml
-  # Uncomment this to enable the volume mount. The variable should point to a
-  # valid SEP license. 
-  volumes:
-    - "${STARBURST_LIC_PATH}:/etc/starburst/starburstdata.license:ro"
-```
-
-### Removing Resources
-
-You can remove resources with the `remove` command.
-
-```
-Usage: minitrino remove [OPTIONS]
-
-  Remove Minitrino resources.
-
-Options:
-  -i, --images      Remove Minitrino images.
-  -v, --volumes     Remove Minitrino container volumes.
-  -l, --label TEXT  Target specific labels for removal (format: key-value
-                    pair(s)).
-
-  -f, --force       Force the removal of Minitrino resources. Normal Docker
-                    removal restrictions apply.
-
-  --help            Show this message and exit.
-```
-
-Notes:
-
-- Named volumes tied to any *existing* container cannot be forcibly removed,
-  neither by Minitrino nor by the Docker CLI/SDK.
-- Images tied to stopped containers can be forcibly removed, but any image tied
-  to a running container cannot be forcibly removed, neither by Minitrino nor by
-  the Docker CLI.
-- You can find a module's label key by looking at the module's
-  `docker-compose.yml` file in the Minitrino library.
-
-Sample `remove` command:
-
-```bash
-minitrino -v remove \
-  --volumes \
-  --label com.starburst.tests.module.postgres=catalog-postgres \
-  --force
+```sh
+  pip install minitrino
+  minitrino -v lib_install
 ```
 
-This will only remove volumes associated to the Postgres catalog module.
+Using this installation method, the `LIB_PATH` variable will point to
+`~/.minitrino/lib/`.
 
-### Shutting Down Environments
+### Developers
 
-You can shut down an active environment with the `down` command.
+In the project's root directory, run `./install.sh` to install the Minitrino
+CLI. If you encounter errors during installation, try running `sudo -H
+./install.sh -v`.
+
+Using this installation method, the `LIB_PATH` variable will point to
+`${MINITRINO_REPOSITORY_DIRECTORY}/lib/`.
+
+### Using Colima and Other Docker Contexts
+
+For users not operating on the default Docker Desktop context, you can set the
+`DOCKER_HOST` shell environment variable to point to the desired context's
+`.sock` file, e.g.:
 
+```sh
+echo 'export DOCKER_HOST="unix://${HOME}/.colima/default/docker.sock"' >> ~/.bash_profile
 ```
-Usage: minitrino down [OPTIONS]
 
-  Bring down running Minitrino containers. This command follows the
-  behavior of `docker-compose down` where containers are both stopped and
-  removed.
-
-Options:
-  -k, --keep  Does not remove containers; instead, containers will only be
-              stopped.
-
-  --sig-kill  Stop Minitrino containers without a grace period.
-  --help      Show this message and exit.
-```
+### End User Upgrades
 
-Sample `down` command:
+To upgrade the Minitrino CLI, run:
 
-```bash
-minitrino -v down
+```sh
+pip install minitrino --upgrade
 ```
 
-### Taking Environment Snapshots
-
-You can capture snapshots for both active and inactive environments with the
-`snapshot` command.
+Each CLI version has its own respective library. To install the updated library,
+run:
 
+```sh
+minitrino -v lib_install
 ```
-Usage: minitrino snapshot [OPTIONS]
 
-  Create a snapshot of a Minitrino environment. A tarball is placed in the
-  Minitrino `lib/snapshots/` directory.
+**Note**: Installing the new library will overwrite all modules and snapshots in
+the current library. If you have customized modules or snapshot files in
+`lib/snapshots/`, make sure to take a backup of the `~/.minitrino/lib` directory
+prior to running this command in order to persist your local changes.
 
-  To take a snapshot of an active environment, leave the `--module` and
-  option out of the command.
+-----
 
-  To take a snapshot of modules whether they are active or not, specify the
-  modules via the `--module` option.
+## Workflow Examples
 
-Options:
-  -m, --module TEXT     A specific module to snapshot.
-  -n, --name TEXT       Basename of the resulting snapshot tarball file.
-                        Allowed characters: alphanumerics, hyphens, and
-                        underscores.  [required]
+Minitrino is best suited for local Trino development. This project is not
+intended for usage on a large scale, and is intentionally designed to limit the
+deployment to a single coordinator container.
 
-  -d, --directory PATH  Directory to save the resulting snapshot file in.
-                        Defaults to the snapshots directory in the Minitrino
-                        library.
+### Provision an Environment
 
-  -f, --force           Overwrite the file if it already exists.
-  --no-scrub            Do not scrub sensitive data from user config file.
-                        
-                        WARNING: all sensitive information (passwords and
-                        keys) will be kept in the user config file added to
-                        the snapshot. Only use this if you are prepared to
-                        share those secrets with another person.
+Provision the `postgres` module with a specific SEP version:
 
-  --help                Show this message and exit.
+```sh
+minitrino -v -e STARBURST_VER=${VER} provision -m postgres
 ```
 
-Notes:
-
-- Minitrino records the original `provision` command and places it in the
-  snapshot file as `provision-snapshot.sh`; this can be directly executed. This
-  makes it easier for others to reuse the environment and provision it
-  identically.
-
-Sample `snapshot` commands:
+Provision the `iceberg` and `oauth2` modules:
 
-```bash
-# Take a snapshot of an active environment (this will create a tarball 
-# called `snapshot-t2533.tar.gz` in the library's `snapshots/` directory):
-minitrino snapshot --name t-2533
-
-# Take a snapshot of specific modules:
-minitrino snapshot -n super-cool-env -m hive -m elasticsearch -m ldap
+```sh
+minitrino -v provision -m postgres -m oauth2
 ```
 
-### Manage User Configuration
-
-You can manage Minitrino configuration with the `config` command.
+Append the running environment with a third module:
 
+```sh
+minitrino -v provision -m postgres -m oauth2 -m hive
 ```
-Usage: minitrino config [OPTIONS]
-
-  Edit the Minitrino user configuration file.
 
-Options:
-  -r, --reset  Reset the Minitrino user configuration file and create a new
-               config file from a template.
-               
-               WARNING: This will remove your configuration file (if it
-               exists) and replace it with a template.
+All environments expose the Starburst service on `localhost:8080`, meaning you
+can visit the web UI directly, or you can connect external clients, such as
+DBeaver, to the `localhost` service. The `trino` container shell can be directly
+accessed via:
 
-  --help       Show this message and exit.
+```sh
+docker exec -it trino bash 
 ```
 
-### Install the Library
+### Modify Files in a Running Container
 
-You can install the Minitrino library with the `lib_install` command. Note that
-it is best practice to have the library version match the CLI version. You can
-check these versions with `minitrino version`.
+You can modify files inside a running container with this workflow:
 
+```sh
+docker exec -it trino bash 
+echo "io.trino=DEBUG" >> /etc/starburst/log.properties
+exit
+docker restart trino
 ```
-Usage: minitrino lib_install [OPTIONS]
 
-  Install the Minitrino library.
+### Shut Down an Environment
 
-Options:
-  -v, --version TEXT  The version of the library to install.
-  --help              Show this message and exit.
+```sh
+minitrino down
 ```
 
-### Display Module Metadata
+### Remove Minitrino Resources
 
-You can see Minitrino module metadata with the `modules` command.
+To remove all images, run:
 
+```sh
+minitrino remove --images
 ```
-Usage: minitrino modules [OPTIONS]
-
-  Display module metadata.
 
-Options:
-  -m, --module TEXT  A specific module to display metadata for.
-  -j, --json         Print the resulting metadata in JSON form (shows
-                     additional module metadata).
+To remove images from a specific module, run:
 
-  -r, --running      Print metadata for all running modules.
-  --help             Show this message and exit.
+```sh
+minitrino remove --images \
+  --label com.starburst.tests.module.${MODULE}=${MODULE_TYPE}-${MODULE}
 ```
 
-### Display Minitrino Versions
+Where `${MODULE_TYPE}` is one of: `admin`, `catalog`, `security`.
 
-You can display the Minitrino CLI and library versions with the `version`
-command.
+You can also use the `remove` command to remove individual volumes with the
+`--volumes` option.
 
-```
-Usage: minitrino version [OPTIONS]
+### Snapshot a Customized Module
 
-  Display Minitrino CLI and library versions.
+Users designing and customizing their own modules can persist them with the
+`snapshot` command. For example, if a user has modified the `hive` module, they
+can persist their changes by running:
 
-Options:
-  --help  Show this message and exit.
+```sh
+minitrino snapshot --name ${SNAPSHOT_NAME} -m hive
 ```
 
-### Pointing the CLI to the Minitrino Library
-
-The Minitrino CLI should always point to a compatible library with the expected
-structure. The library directory can be set one of four ways, listed below in
-the order of precedence:
-
-1. Passing the `LIB_PATH` variable to the CLI's `--env` option sets the library
-   directory for the current command.
-2. The `minitrino.cfg` file's `LIB_PATH` variable sets the library directory if
-   present.
-3. The path `~/.minitrino/lib/` is used as the default lib path if the
-   `LIB_PATH` var is not found.
-4. As a last resort, Minitrino will check to see if the library exists in
-   relation to the positioning of the `components.py` file and assumes the
-   project is being run out of a cloned repository.
-
-If you not running out of a cloned repository, it is advisable to provide a
-pointer to the library in Minitrino's configuration via the `LIB_PATH` config.
+By default, the snapshot file is placed in
+`${LIB_PATH}/${SNAPSHOT_NAME}.tar.gz`. The snapshot can be saved to a different
+directory by passing the `--directory` option to the `snapshot` command.
 
 -----
 
 ## Minitrino Configuration File
 
 Sticky configuration is set in `~/.minitrino/minitrino.cfg`. The sections in
 this file each serve a separate purpose.
@@ -453,17 +238,17 @@
 - `LIB_PATH`: The filesystem path of the Minitrino library (specifically to the
   `lib/` directory).
 - `TEXT_EDITOR`: The text editor to use with the `config` command, e.g. "vi",
   "nano", etc. Defaults to the shell's default editor.
 
 ### [MODULES] Section
 
-This section has only one default config: `STARBURST_LIC_PATH`. This is required
-if using licensed Starburst Enterprise features. It can point to any valid
-license on your filesystem.
+This section has only one default config: `SEP_LIC_PATH`. This is required if
+using licensed Starburst Enterprise features. It can point to any valid license
+on your filesystem.
 
 This section can also be used to set environment variables passed to containers
 provisioned by Minitrino. Environment variables are only passed to a container
 if the variable is specified in the module's `docker-compose.yml` file.
 
 For example, if your `minitrino.cfg` config file contains this variable:
 
@@ -473,38 +258,36 @@
 
 And your `docker-compose.yml` file contains this:
 
 ```yaml
 services:
   trino:
     environment:
-      DB_PASSWORD: "${DB_PASSWORD}"
+      DB_PASSWORD: ${DB_PASSWORD}
 ```
 
-Then `DB_PASSWORD` is accessible inside of the resulting Trino container in the
-form of a shell environment variable. This functionality can be applied to any
-container as long as the above is followed.
+Then `DB_PASSWORD` is accessible inside of the Trino container as an environment
+variable. This functionality can be applied to any container as long as the
+convention above is followed.
 
 -----
 
 ## Project Structure
 
 The library is built around Docker Compose files and utilizes Docker's ability
 to [extend Compose
 files](https://docs.docker.com/compose/extends/#multiple-compose-files).
 
 The Starburst Trino service is defined in a Compose file at the library root,
 and all other services look up in the directory tree to reference the parent
-Trino service. In Compose files, the fully-qualified path––relative to the
-library's root `docker-compose.yml` file––must be provided for Docker to locate
-resources.
+Trino service.
 
 A simplified library structure:
 
-```
+```sh
 lib
 ├── Dockerfile
 ├── docker-compose.yml
 ├── minitrino.env
 ├── modules
 │   ├── admin
 │   │   └── ...
@@ -521,65 +304,37 @@
 │   ├── resources
 │   └── security
 │       └── ...
 ├── snapshots
 └── version
 ```
 
-And the contents of a `docker-compose.yml` file (`postgres.yml`):
-
-```yaml
-version: "3.8"
-services:
-
-  trino:
-    volumes:
-      - "./modules/catalog/postgres/resources/trino/postgres.properties:/etc/starburst/catalog/postgres.properties"
-
-  postgres:
-    image: "postgres:${POSTGRES_VER}"
-    container_name: "postgres"
-    labels:
-      - "com.starburst.tests=minitrino"
-      - "com.starburst.tests.module.postgres=catalog-postgres"
-    env_file:
-      - "./modules/catalog/postgres/resources/postgres/postgres.env"
-```
-
-Notice that the volume mount is not relative to the
-`lib/modules/catalog/postgres/` directory––it is relative to the parent
-directory which houses the top-level `docker-compose.yml` file. Also, notice the
-labels––these labels will be used to identify Docker resources tied to Minitrino
-modules so that the CLI commands actually work.
-
 ### Trino Dockerfile
 
-Minitrino modifies the Starburst Trino Docker image by adding the Trino CLI to
-the image as well as by providing `sudo` to the `trino` user. This is required
-for certain bootstrap scripts (i.e. using `yum` to install packages in a Trino
-container for a module). This image is compatible with Starburst Trino images
-back to Starburst Trino version `332-e.0`.
+Minitrino modifies Starburst's Docker image by adding the Trino CLI to the image
+as well as by adding `sudo` privileges to the `trino` user. This is required for
+certain bootstrap scripts (i.e. using `microdnf` to install packages in a Trino
+container for a module).
 
 -----
 
-## Adding New Modules (Tutorial)
+## Add New Modules (Tutorial)
 
 Adding new modules is relatively simple, but there are a few important
-guidelines to follow to ensure compatibility with the Minitrino CLI. The design
-rules are the same for both catalogs and security modules. The example below
-demonstrates the process of creating a new catalog module for a Postgres
-service.
+guidelines to follow to ensure compatibility with the Minitrino CLI. Module
+design principals are the same all modules. The example below demonstrates the
+process of creating a new catalog module for a Postgres service.
 
 ### Create the Module Directory
 
 Create the module's directory in the `lib/modules/catalog/` directory:
 
 ```sh
-mkdir lib/modules/catalog/postgres/
-cd lib/modules/catalog/postgres/
+mkdir lib/modules/catalog/my-postgres/
+cd lib/modules/catalog/my-postgres/
 ```
 
 ### Add Trino Resources
 
 All resources for a module go inside of a `resources/` directory within the
 module. Inside this directory, place Trino-specific resources into a `trino/`
 directory, then mount the resources to the Trino service defined in the root
@@ -598,30 +353,32 @@
 connection-user=admin
 connection-password=trinoRocks15
 EOF"
 ```
 
 -----
 
-**Note**: Passwords should always be `trinoRocks15` for consistency throughout
-modules.
+**Note**: Passwords in the default modules tend to be `trinoRocks15`. For
+consistency throughout the library, it is recommended to use this as the
+password of choice for new module development.
 
 -----
 
 ### Add the Docker Compose YAML
 
-In `lib/modules/catalog/postgres/`, add a Docker Compose file:
+In `lib/modules/catalog/my-postgres/`, add a Docker Compose file:
 
 ```sh
-touch postgres.yml
+touch my-postgres.yml
 ```
 
-Notice the naming convention: `postgres.yml`. Giving the same root name of
-"postgres" to both the parent directory `postgres/` and to the Docker Compose
-file `postgres.yml` will allow Minitrino to find our new catalog module.
+Notice the naming convention: `my-postgres.yml`. Giving the same root name of
+"my-postgres" to both the parent directory `my-postgres/` and to the Docker
+Compose file `my-postgres.yml` will allow Minitrino to find the new catalog
+module.
 
 Next, add an environment file for the Postgres service. Non-Trino resources
 should go into their own directory, so create one for postgres:
 
 ```sh
 mkdir resources/postgres/
 ```
@@ -638,88 +395,92 @@
 ```
 
 This file will initialize Postgres with a database `minitrino`, a user `trino`,
 and a password `trinoRocks15`.
 
 ### Add a Metadata File
 
-The `metadata.json` file allows Minitrino to obtain key information for the
-module. It is required for a module to work with the CLI.
+The `metadata.json` file allows Minitrino to obtain key information about the
+module. **It is required for a module to work with the CLI.**
 
-In `lib/modules/catalog/postgres/`, add the `metadata.json` file:
+In `lib/modules/catalog/my-postgres/`, add a `metadata.json` file:
 
 ```sh
 bash -c 'cat << EOF > metadata.json
 {
   "description": "Creates a Postgres catalog using the standard Postgres connector.",
   "incompatibleModules": [],
-  "dependentModules": []
+  "dependentModules": [],
+  "enterprise": false
 }
 EOF'
 ```
 
-The metadata file is presentable to the user via the `modules` command. The
-`incompatibleModules` key restricts certain modules from being provisioned
+- `description`: describes the module.
+- `incompatibleModules`: restricts certain modules from being provisioned
 alongside the given module. The `*` wildcard is a supported convention if the
-module is incompatible with all other modules. Lastly, the `dependentModules`
-key can be used to require other pre-defined modules to provision alongside the
-module containing the `metadata.json` file.
+module is incompatible with all other modules.
+- `dependentModules`: specifies which modules must be provisioned alongside the
+target. Dependent modules will be automatically provisioned with the `provision`
+command.
+- `enterprise`: requires a Starburst license file (`starburstdata.license`).
+
+The metadata file information can be exposed via the `modules` command.
 
 ### Add a Readme File
 
 This step is not required for personal development, but it is required to commit
 a module to the Minitrino repository.
 
-In `lib/modules/catalog/postgres/`, add the `readme.md` file:
+In `lib/modules/catalog/my-postgres/`, add a `readme.md` file:
 
 ```sh
 touch readme.md
 ```
 
 This file should contain an overview of the module.
 
 ### Review Progress
 
-The resulting directory tree should look like this (from the `/modules/catalog/`
-directory):
+The resulting directory tree should look like this (from the
+`lib/modules/catalog/` directory):
 
-```
-postgres
+```sh
+my-postgres
 ├── metadata.json
-├── postgres.yml
+├── my-postgres.yml
 ├── readme.md
 └── resources
     ├── postgres
     │   └── postgres.env
     └── trino
         └── postgres.properties
 ```
 
 ### Configure the Docker Compose YAML File
 
-We will now define the `postgres.yml` Docker Compose file. Set it up as follows,
-and **read the important notes after**:
+We will now define the `my-postgres.yml` Docker Compose file. Set it up as
+follows:
 
 ```yaml
-version: "3.8"
+version: '3.8'
 services:
 
   trino:
     volumes:
-    # Always place Trino files in `/etc/starburst/` as symbolic links can change between versions
-      - "./modules/catalog/postgres/resources/trino/postgres.properties:/etc/starburst/catalog/postgres.properties"
+      - ./modules/catalog/my-postgres/resources/trino/postgres.properties:/etc/starburst/catalog/postgres.properties
 
   postgres:
-    image: "postgres:${POSTGRES_VER}"
-    container_name: "postgres"
-    labels:
-      - "com.starburst.tests=minitrino"
-      - "com.starburst.tests.module.postgres=catalog-postgres"
+    image: postgres:${POSTGRES_VER}
+    container_name: postgres
     env_file:
-      - "./modules/catalog/postgres/resources/postgres/postgres.env"
+      - ./modules/catalog/my-postgres/resources/postgres/postgres.env
+    labels:
+      - com.starburst.tests=minitrino
+      - com.starburst.tests.module.my-postgres=catalog-my-postgres
 
 ```
 
 ### Important Implementation Details: Paths and Labels
 
 We can observe a few things about the Compose file we just defined.
 
@@ -736,104 +497,98 @@
 is how Minitrino constructs these commands.
 
 If this is confusing, you can read more about extending Compose files on the
 [Docker docs](https://docs.docker.com/compose/extends/#multiple-compose-files).
 
 #### Minitrino Docker Labels
 
-Secondly, notice how we applied sets of labels to the Postgres service. These
+Secondly, notice the applied sets of labels to the Postgres service. These
 labels tell the CLI which resources to target when executing commands.
 
 In general, there is no need to apply labels to the Trino service since they are
 already applied in the parent Compose file **unless** the module is an extension
-of the Trino service itself (i.e. the Snowflake modules). Labels should always
-be applied to:
+of the Trino service itself (i.e. the `biac` module). Labels should always be
+applied to:
 
 - Docker services (AKA the resulting container)
-- Named volumes
-- Images built from a Dockerfile
+- Persistent volumes
+- Images built from a Dockerfile (see the main `docker-compose.yml` file for an
+  example)
 
 Labels should be defined in pairs of two. The convention is:
 
 - The standard Minitrino resource label: `com.starburst.tests=minitrino`
 - A module-specific resource label:
-  `com.starburst.tests.module.<module-name>=<module-type>-<module-name>`
-  - For this label, the `module-type` should be either `catalog` or `security`
-  - This applies a unique label to the module, allowing it to be an isolated
-    component when necessary.
+  `com.starburst.tests.module.${MODULE_NAME}=${MODULE_CATEGORY}-${MODULE_NAME}`
+  - For this label, the `module-type` should be one of: `admin`, `catalog`, or
+    `security`
+  - This applies a unique label to the module, allowing it to be isolated when
+    necessary
 
 In Compose files where multiple services are defined, all services should be
-labeled with the same label sets (see `hive.yml` for an example).
+labeled with the same label sets (see the `hive` for an example).
 
 -----
 
 **Note**: A named volume is defined explicitly in the Compose file, and these
 should always have label sets applied to them. Below is an example of the
 Compose file we just created with a named volume.
 
 -----
 
 ```yaml
-version: "3.8"
+version: '3.8'
 services:
 
   trino:
     volumes:
-      - "./modules/catalog/postgres/resources/trino/postgres.properties:/etc/starburst/catalog/postgres.properties"
+      - ./modules/catalog/my-postgres/resources/trino/postgres.properties:/etc/starburst/catalog/postgres.properties
 
   postgres:
-    image: "postgres:${POSTGRES_VER}"
-    container_name: "postgres"
-    labels: # These labels are applied to the service/container
-      - "com.starburst.tests=minitrino"
-      - "com.starburst.tests.module.postgres=catalog-postgres"
+    image: postgres:${POSTGRES_VER}
+    container_name: postgres
     env_file:
-      - "./modules/catalog/postgres/resources/postgres/postgres.env"
+      - ./modules/catalog/my-postgres/resources/postgres/postgres.env
+    labels: # These labels are applied to the service/container
+      - com.starburst.tests=minitrino
+      - com.starburst.tests.module.my-postgres=catalog-my-postgres
 
 volumes:
   postgres-data:
     labels: # These labels are applied to the named volume
-      - "com.starburst.tests=minitrino"
-      - "com.starburst.tests.module.postgres=catalog-postgres"
+      - com.starburst.tests=minitrino
+      - com.starburst.tests.module.my-postgres=catalog-my-postgres
 ```
 
 -----
 
 **Note**: Certain modules will only extend the parent Trino service and do not
-actually define any new services/containers. See the Snowflake catalog modules
-for an example of this. For these modules, the only label requirement is to add
-the module-specific label to the Trino service in the relevant
-`docker-compose.yml` file
+actually define any new services/containers. See the `biac` module for an
+example of this. For these modules, the only label requirement is to add the
+module-specific label to the Trino service in the relevant `docker-compose.yml`
+file.
 
 -----
 
 ### Test the New Catalog
 
 We are all finished up. We can test our new catalog through the Minitrino CLI:
 
 ```sh
-minitrino provision -m postgres
+minitrino provision -m my-postgres
 ```
 
-We can now shell into the `trino` container and run some tests:
+We can now open a shell session in the `trino` container and run some tests:
 
-```
+```sh
 docker exec -it trino bash 
 trino-cli
 trino> show catalogs;
 ```
 
-### Customizing Images
-
-If you need to build an image from a local Dockerfile, you can do so and
-structure the Compose file accordingly. See the library's root
-`docker-compose.yml` file for an example of this. Path references for volumes
-and the image build context will follow the same convention as volume mount
-paths described earlier.
-
 ### Bootstrap Scripts
 
 Minitrino supports container bootstrap scripts. These scripts **do not replace**
 the entrypoint (or default command) for a given container. The script is copied
 from the Minitrino library to the container, executed, and then removed from the
 container. Containers are restarted after each bootstrap script execution, **so
 the bootstrap scripts themselves should not restart the container's service**.
@@ -849,20 +604,20 @@
 container(s) via `minitrino down` and then to re-provision.
 
 To add a bootstrap script, add a `resources/bootstrap/` directory in any given
 module, create a shell script, and then reference the script name in the Compose
 YAML file:
 
 ```yaml
-version: "3.8"
+version: '3.8'
 services:
 
   trino:
     environment:
-      MINITRINO_BOOTSTRAP: "bootstrap.sh"
+      MINITRINO_BOOTSTRAP: bootstrap.sh
 ```
 
 The `elasticsearch` module is a good example of this.
 
 #### Installing Shell Packages for Bootstrap Scripts
 
 If you need to install a shell package for a bootstrap script, it is recommended
@@ -871,60 +626,65 @@
 releases.
 
 To add the necessary package, simply update shell dependencies in
 `lib/dockerfile-resources/configure.sh`.
 
 ### Managing Trino's `config.properties` and `jvm.config` Files
 
-Many modules can change the Trino `config.properties` and `jvm.config` files.
-Because of this, there are two supported ways to modify these files with
-Minitrino.
-
-The first way is by setting the relevant environment variables in your
-`module.yml` Docker Compose file. This will propagate the configs to the Trino
-container when it is provisioned. For example:
+Many modules may change the Trino `config.properties` and `jvm.config` files.
+There are two supported ways to modify these files with within the `trino`
+container.
+
+#### Preferable Method: Environment Variables
+
+Minitrino has special support for two Trino-specific environment variables:
+`CONFIG_PROPERTIES` and `JVM_CONFIG`. Below is an example of setting these
+variables:
 
 ```yaml
 trino:
   environment:
     CONFIG_PROPERTIES: |-
       insights.jdbc.url=jdbc:postgresql://postgresdb:5432/insights
       insights.jdbc.user=admin
       insights.jdbc.password=password
       insights.persistence-enabled=true
     JVM_CONFIG: |-
       -Xlog:gc:/var/log/sep-gc-%t.log:time:filecount=10
 ```
 
-The second way to modify these configuration files is via module [bootstrap
-scripts](#bootstrap-scripts).
+#### Secondary Method: Bootstrap Scripts
+
+The `config.properties` and `jvm.config` files can also be modified directly
+with a Trino [bootstrap script](#bootstrap-scripts).
 
 -----
 
 ## Troubleshooting
 
 - If you experience issues executing a Minitrino command, re-run it with the
-  `-v` option for verbose output. This will often reveal the issue
+  `-v` option for verbose output. This will often reveal the issue's root cause.
 - If you experience an issue with a particular Docker container, consider
   running these commands:
-  - `docker logs <container>`: Print the logs for a given container to the
+  - `docker logs ${CONTAINER_NAME}`: Print the logs for a given container to the
     terminal
   - `docker ps`: Show all running Docker containers and associated statistics
-  - `docker inspect <container>` to see various details about a container
+  - `docker inspect ${CONTAINER_NAME}` to see various details about a container
 - If you experience issues with a library module, check that that module is
   structured correctly according to the [module
-  tutorial](#adding-new-modules-tutorial), and ensure the library and the CLI
+  tutorial](#add-new-modules-tutorial), and ensure the library and the CLI
   versions match
-- Sometimes, a lingering persistent volume can cause problem (i.e. a stale Hive
-  metastore database volume from a previous module), so you can run:
+- Sometimes, a lingering persistent volume can cause problems (i.e. a stale Hive
+  metastore database volume from a previous module deployment), so you can run:
   - `minitrino down`
   - `minitrino -v remove --volumes` to remove **all** existing Minitrino
     volumes. Alternatively, run `minitrino -v remove --volumes --label <your
     label>` to specify a specific module for which to remove volumes. See the
-    [removing resources](#removing-resources) section for more information.
+    [removing resources](#remove-minitrino-resources) section for more
+    information.
 
 If none of these troubleshooting tips help to resolve your issue, [please file a
 GitHub issue](#reporting-bugs-and-contributing) and provide as much information
 as possible.
 
 -----
 
@@ -943,9 +703,7 @@
 1. Fork the repository, then make a PR to merge your changes
 2. If you have been added as a contributor, you can go with the method above or
    you can create a feature branch, then submit a PR for that feature branch
    when it is ready to be merged.
 
 In either case, please provide a comprehensive description of your changes with
 the PR.
-
-
```

### Comparing `minitrino-2.0.3/minitrino/cli.py` & `minitrino-2.0.4/minitrino/cli.py`

 * *Files identical despite different names*

### Comparing `minitrino-2.0.3/minitrino/cmd/cmd_config.py` & `minitrino-2.0.4/minitrino/cmd/cmd_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,35 +30,33 @@
 )
 @utils.exception_handler
 @pass_environment
 def cli(ctx, reset):
     """Config command for Minitrino."""
 
     if not os.path.isdir(ctx.minitrino_user_dir):
-        ctx.logger.log(f"No {ctx.minitrino_user_dir} directory found. Creating...")
+        ctx.logger.info(f"No {ctx.minitrino_user_dir} directory found. Creating...")
         os.mkdir(ctx.minitrino_user_dir)
 
     if os.path.isfile(ctx.config_file) and not reset:
-        ctx.logger.log(
+        ctx.logger.verbose(
             f"Opening existing config file at path: {ctx.config_file}",
-            level=ctx.logger.verbose,
         )
         edit_file()
     elif os.path.isfile(ctx.config_file) and reset:
         response = ctx.logger.prompt_msg(f"Configuration file exists. Overwrite? [Y/N]")
         if utils.validate_yes(response):
             write_template()
             edit_file()
         else:
-            ctx.logger.log(f"Opted out of recreating {ctx.minitrino_user_dir} file.")
+            ctx.logger.info(f"Opted out of recreating {ctx.minitrino_user_dir} file.")
     else:
-        ctx.logger.log(
+        ctx.logger.verbose(
             f"No config file found at path: {ctx.config_file}. "
             f"Creating template config file and opening for edits...",
-            level=ctx.logger.verbose,
         )
         write_template()
         edit_file()
 
 
 @pass_environment
 def write_template(ctx):
```

### Comparing `minitrino-2.0.3/minitrino/cmd/cmd_down.py` & `minitrino-2.0.4/minitrino/cmd/cmd_down.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from minitrino.settings import RESOURCE_LABEL
 
 
 @click.command(
     "down",
     help=(
         """Bring down running Minitrino containers. This command follows the
-        behavior of `docker-compose down` where containers are both stopped and
+        behavior of `docker compose down` where containers are both stopped and
         removed."""
     ),
 )
 @click.option(
     "-k",
     "--keep",
     is_flag=True,
@@ -44,38 +44,37 @@
     utils.check_lib(ctx)
 
     containers = ctx.docker_client.containers.list(
         filters={"label": RESOURCE_LABEL}, all=True
     )
 
     if len(containers) == 0:
-        ctx.logger.log("No containers to bring down.")
+        ctx.logger.info("No containers to bring down.")
         sys.exit(0)
 
     if sig_kill:
         stop_timeout = 1
-        ctx.logger.log(
+        ctx.logger.verbose(
             "Stopping Minitrino containers with sig-kill...",
-            level=ctx.logger.verbose,
         )
     else:
         stop_timeout = 10
 
     # Stop
     for container in containers:
         identifier = utils.generate_identifier(
             {"ID": container.short_id, "Name": container.name}
         )
         if container.status == "running":
             container.stop(timeout=stop_timeout)
-            ctx.logger.log(f"Stopped container: {identifier}", level=ctx.logger.verbose)
+            ctx.logger.verbose(f"Stopped container: {identifier}")
 
     # Remove
     if not keep:
         for container in containers:
             identifier = utils.generate_identifier(
                 {"ID": container.short_id, "Name": container.name}
             )
             container.remove()
-            ctx.logger.log(f"Removed container: {identifier}", level=ctx.logger.verbose)
+            ctx.logger.verbose(f"Removed container: {identifier}")
 
-    ctx.logger.log("Brought down all Minitrino containers.")
+    ctx.logger.info("Brought down all Minitrino containers.")
```

### Comparing `minitrino-2.0.3/minitrino/cmd/cmd_lib_install.py` & `minitrino-2.0.4/minitrino/cmd/cmd_lib_install.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,24 +33,22 @@
     lib_dir = os.path.join(ctx.minitrino_user_dir, "lib")
     if os.path.isdir(lib_dir):
         response = ctx.logger.prompt_msg(
             f"The Minitrino library at {lib_dir} will be overwritten. "
             f"Continue? [Y/N]"
         )
         if utils.validate_yes(response):
-            ctx.logger.log(
-                "Removing existing library directory...", level=ctx.logger.verbose
-            )
+            ctx.logger.verbose("Removing existing library directory...")
             shutil.rmtree(lib_dir)
         else:
-            ctx.logger.log("Opted to skip library installation.")
+            ctx.logger.info("Opted to skip library installation.")
             sys.exit(0)
 
     download_and_extract(version)
-    ctx.logger.log("Library installation complete.")
+    ctx.logger.info("Library installation complete.")
 
 
 @pass_environment
 def download_and_extract(ctx, version=""):
     github_uri = f"https://github.com/jefflester/minitrino/archive/{version}.tar.gz"
     tarball = os.path.join(ctx.minitrino_user_dir, f"{version}.tar.gz")
     file_basename = f"minitrino-{version}"  # filename after unpacking
@@ -62,17 +60,16 @@
         ctx.cmd_executor.execute_commands(cmd)
         if not os.path.isfile(tarball):
             raise err.MinitrinoError(
                 f"Failed to download Minitrino library ({tarball} not found)."
             )
 
         # Unpack tarball and copy lib
-        ctx.logger.log(
+        ctx.logger.verbose(
             f"Unpacking tarball at {tarball} and copying library...",
-            level=ctx.logger.verbose,
         )
         ctx.cmd_executor.execute_commands(
             f"tar -xzvf {tarball} -C {ctx.minitrino_user_dir}",
             f"mv {lib_dir} {ctx.minitrino_user_dir}",
         )
 
         # Check that the library is present
```

### Comparing `minitrino-2.0.3/minitrino/cmd/cmd_modules.py` & `minitrino-2.0.4/minitrino/cmd/cmd_modules.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 @utils.exception_handler
 @pass_environment
 def cli(ctx, modules, json_format, running):
     """Module metadata command for Minitrino."""
 
     utils.check_lib(ctx)
 
-    ctx.logger.log("Printing module metadata...")
+    ctx.logger.info("Printing module metadata...")
 
     if not modules and not running:
         for module, module_dict in ctx.modules.data.items():
             log_info(module, module_dict, json_format)
         return
 
     if running:
@@ -69,20 +69,20 @@
 
 @pass_environment
 def log_info(ctx, module_name="", module_dict={}, json_format=False):
     """Logs module metadata to the user's terminal."""
 
     if json_format:
         module_dict = {module_name: module_dict}
-        ctx.logger.log(json.dumps(module_dict, indent=2))
+        ctx.logger.info(json.dumps(module_dict, indent=2))
     else:
         log_msg = [f"Module: {module_name}\n"]
         keys = ["description", "incompatibleModules", "dependentModules", "enterprise"]
         for key in keys:
             val = module_dict.get(key, None)
             if val is not None:
                 key = list(key)
                 key[0] = key[0].title()
                 key = "".join(key)
                 log_msg.extend(f"{key}: {val}\n")
 
-        ctx.logger.log("".join(log_msg))
+        ctx.logger.info("".join(log_msg))
```

### Comparing `minitrino-2.0.3/minitrino/cmd/cmd_provision.py` & `minitrino-2.0.4/minitrino/cmd/cmd_provision.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 #!usr/bin/env/python3
 # -*- coding: utf-8 -*-
 
 # Instead of using the Docker SDK, this script will form a Docker Compose
-# command string to execute straight through the docker-compose CLI. This is
+# command string to execute straight through the docker compose CLI. This is
 # required because the Docker SDK does not support communication with Compose
 # files, and Minitrino benefits hugely from Docker Compose.
 
 import os
+import re
 import stat
 import hashlib
 import time
 import platform
 import click
 import yaml
 
 from minitrino.cli import pass_environment
 from minitrino import utils
 from minitrino import errors as err
 from minitrino.settings import RESOURCE_LABEL
 from minitrino.settings import ETC_TRINO
 from minitrino.settings import SEP_VOLUME_MOUNT
+from minitrino.settings import SEP_LIC_MOUNT_PATH
+from minitrino.settings import DUMMY_LIC_MOUNT_PATH
 from minitrino.settings import TRINO_CONFIG
 from minitrino.settings import TRINO_JVM_CONFIG
 
 from docker.errors import NotFound
 
 
 @click.command(
@@ -54,41 +57,41 @@
 )
 @click.option(
     "-d",
     "--docker-native",
     default="",
     type=str,
     help=(
-        """Appends native docker-compose commands to the generated
-        docker-compose shell command. Run `docker-compose up --help` to see all
+        """Appends native docker compose commands to the generated
+        docker compose shell command. Run `docker compose up --help` to see all
         available options.
 
         Example: minitrino provision --docker-native --build
 
         Example: minitrino provision --docker-native '--remove-orphans
         --force-recreate'"""
     ),
 )
 @utils.exception_handler
 @pass_environment
 def cli(ctx, modules, no_rollback, docker_native):
-    """Provision command for Minitrino. If the resulting docker-compose command
+    """Provision command for Minitrino. If the resulting docker compose command
     is unsuccessful, the function exits with a non-zero status code."""
 
     utils.check_daemon(ctx.docker_client)
     utils.check_lib(ctx)
     utils.check_starburst_ver(ctx)
-    modules = append_running_modules(modules)
+    modules = list(set(append_running_modules(modules)))
     modules = check_dependent_modules(modules)
     check_compatibility(modules)
-    check_enterprise(modules)
+    compose_env = check_enterprise(modules)
     check_volumes(modules)
 
     if not modules:
-        ctx.logger.log(
+        ctx.logger.info(
             f"No modules specified. Provisioning standalone Trino container..."
         )
     else:
         for module in modules:
             if not ctx.modules.data.get(module, False):
                 raise err.UserError(
                     f"Invalid module: '{module}'. It was not found "
@@ -98,47 +101,45 @@
     try:
         cmd_chunk = chunk(modules)
 
         # Module env variables shared with compose should be from the modules
         # section of environment variables and any extra variables provided by the
         # user that didn't fit into any other section
 
-        compose_env = ctx.env.get_section("MODULES")
         compose_env.update(ctx.env.get_section("EXTRA"))
         if is_apple_m1():
             compose_env.update({"MODULE_PLATFORM": "linux/amd64"})
         compose_cmd = build_command(docker_native, compose_env, cmd_chunk)
 
         ctx.cmd_executor.execute_commands(compose_cmd, environment=compose_env)
         initialize_containers()
 
-        containers_to_restart = execute_bootstraps(modules)
-        containers_to_restart = write_trino_configs(containers_to_restart, modules)
-        check_dup_configs()
-        restart_containers(containers_to_restart)
-        ctx.logger.log(f"Environment provisioning complete.")
+        c_restart = execute_bootstraps(modules)
+        c_restart = write_trino_cfg(c_restart, modules)
+        check_dup_cfgs()
+        restart_containers(c_restart)
+        ctx.logger.info(f"Environment provisioning complete.")
 
     except Exception as e:
-        rollback_provision(no_rollback)
+        rollback(no_rollback)
         utils.handle_exception(e)
 
 
 @pass_environment
 def append_running_modules(ctx, modules=[]):
     """Checks if any modules are already running. If they are, they are appended
     to the provided modules list and the updated list is returned."""
 
-    ctx.logger.log("Checking for running modules...", level=ctx.logger.verbose)
+    ctx.logger.verbose("Checking for running modules...")
     running_modules = ctx.modules.get_running_modules()
 
     if running_modules:
-        ctx.logger.log(
+        ctx.logger.verbose(
             f"Identified the following running modules: {running_modules}. "
             f"Appending the running module list to the list of modules to provision.",
-            level=ctx.logger.verbose,
         )
 
     modules = list(modules)
     modules.extend(running_modules)
     return modules
 
 
@@ -149,17 +150,16 @@
     for module in modules:
         dependent_modules = ctx.modules.data.get(module, {}).get("dependentModules", [])
         if not dependent_modules:
             continue
         for dependent_module in dependent_modules:
             if not dependent_module in modules:
                 modules.append(dependent_module)
-                ctx.logger.log(
+                ctx.logger.verbose(
                     f"Module dependency for module '{module}' will be included: '{dependent_module}'",
-                    level=ctx.logger.verbose,
                 )
     return modules
 
 
 @pass_environment
 def check_compatibility(ctx, modules=[]):
     """Checks if any of the provided modules are mutually exclusive of each
@@ -182,120 +182,127 @@
                     f"running 'minitrino modules -m {module}'",
                 )
 
 
 @pass_environment
 def check_enterprise(ctx, modules=[]):
     """Checks if any of the provided modules are Starburst Enterprise features.
-    If they are, we check that a pointer to an SEP license is provided."""
+    If they are, we check that a pointer to a SEP license is provided."""
 
-    ctx.logger.log(
+    ctx.logger.verbose(
         "Checking for SEP license for enterprise modules...",
-        level=ctx.logger.verbose,
     )
 
+    yaml_path = os.path.join(ctx.minitrino_lib_dir, "docker-compose.yml")
+    with open(yaml_path) as f:
+        yaml_file = yaml.load(f, Loader=yaml.FullLoader)
+    volumes = yaml_file.get("services", {}).get("trino", {}).get("volumes", [])
+
+    if SEP_VOLUME_MOUNT not in volumes:
+        raise err.UserError(
+            f"The required license volume in the library's root docker-compose.yml "
+            f"is either commented out or deleted: {yaml_path}. For reference, "
+            f"the proper volume mount is: '{SEP_VOLUME_MOUNT}'"
+        )
+
+    enterprise_modules = []
     for module in modules:
-        enterprise = ctx.modules.data.get(module, {}).get("enterprise", False)
-        if enterprise:
-            yaml_path = os.path.join(ctx.minitrino_lib_dir, "docker-compose.yml")
-            with open(yaml_path) as f:
-                yaml_file = yaml.load(f, Loader=yaml.FullLoader)
-            volumes = yaml_file.get("services", {}).get("trino", {}).get("volumes", [])
-            if SEP_VOLUME_MOUNT not in volumes:
-                raise err.UserError(
-                    f"Module {module} requires a Starburst license. "
-                    f"The license volume in the library's docker-compose.yml "
-                    f"file must be uncommented at: {yaml_path}."
-                    f"For reference, the proper volume mount is: '{SEP_VOLUME_MOUNT}'"
-                )
-            if not ctx.env.get_var("STARBURST_LIC_PATH", False):
-                raise err.UserError(
-                    f"Module {module} requires a Starburst license. "
-                    f"You must provide a path to a Starburst license via the "
-                    f"STARBURST_LIC_PATH environment variable"
-                )
+        if ctx.modules.data.get(module, {}).get("enterprise", False):
+            enterprise_modules.append(module)
+
+    compose_env = ctx.env.get_section("MODULES")
+
+    if enterprise_modules:
+        if not ctx.env.get_var("SEP_LIC_PATH", False):
+            raise err.UserError(
+                f"Module(s) {enterprise_modules} requires a Starburst license. "
+                f"You must provide a path to a Starburst license via the "
+                f"SEP_LIC_PATH environment variable"
+            )
+        compose_env.update({"SEP_LIC_MOUNT_PATH": SEP_LIC_MOUNT_PATH})
+    elif ctx.env.get_var("SEP_LIC_PATH", False):
+        compose_env.update({"SEP_LIC_MOUNT_PATH": SEP_LIC_MOUNT_PATH})
+    else:
+        compose_env.update({"SEP_LIC_PATH": "./modules/resources/dummy.license"})
+        compose_env.update({"SEP_LIC_MOUNT_PATH": DUMMY_LIC_MOUNT_PATH})
+    return compose_env
 
 
 @pass_environment
 def check_volumes(ctx, modules=[]):
     """Checks if any of the modules have persistent volumes and issues a warning
     to the user if so."""
 
-    ctx.logger.log(
-        "Checking modules for persisent volumes...",
-        level=ctx.logger.verbose,
+    ctx.logger.verbose(
+        "Checking modules for persistent volumes...",
     )
 
     for module in modules:
         if ctx.modules.data.get(module, {}).get("yaml_dict", {}).get("volumes", {}):
-            ctx.logger.log(
+            ctx.logger.warn(
                 f"Module '{module}' has persistent volumes associated with it. "
                 f"To delete these volumes, remember to run `minitrino remove --volumes`.",
-                level=ctx.logger.warn,
             )
 
 
 @pass_environment
 def is_apple_m1(ctx):
     """Checks the host platform to determine if MODULE_PLATFORM needs to
     be set."""
 
-    ctx.logger.log(
+    ctx.logger.verbose(
         "Checking host platform...",
-        level=ctx.logger.verbose,
     )
 
     if "arm64" == os.uname().machine.lower() and platform.processor().lower() == "arm":
-        ctx.logger.log(
+        ctx.logger.verbose(
             f"Host machine running on Apple M1 architecture. "
             f"Images will pull in a best-effort fashion.",
-            level=ctx.logger.verbose,
         )
         return True
     return False
 
 
 @pass_environment
 def chunk(ctx, modules=[]):
-    """Builds docker-compose command chunk for the chosen modules. Returns a
+    """Builds docker compose command chunk for the chosen modules. Returns a
     command chunk string."""
 
     chunk = []
     for module in modules:
         yaml_file = ctx.modules.data.get(module, {}).get("yaml_file", "")
         chunk.extend(f"-f {yaml_file} \\\n")
     return "".join(chunk)
 
 
 @pass_environment
 def build_command(ctx, docker_native="", compose_env={}, chunk=""):
-    """Builds a formatted docker-compose command for shell execution. Returns a
-    docker-compose command string."""
+    """Builds a formatted docker compose command for shell execution. Returns a
+    docker compose command string."""
 
     cmd = []
     compose_env_string = ""
     for k, v in compose_env.items():
         compose_env_string += f'{k.upper()}="{v}" '
 
     cmd.extend(
         [
             compose_env_string,
             "\\\n",
-            "docker-compose -f ",
+            "docker compose -f ",
             os.path.join(ctx.minitrino_lib_dir, "docker-compose.yml"),
             " \\\n",
             chunk,  # Module YAML paths
-            "up -d",
+            "up -d --no-recreate",
         ]
     )
 
     if docker_native:
-        ctx.logger.log(
+        ctx.logger.verbose(
             f"Received native Docker Compose options: '{docker_native}'",
-            level=ctx.logger.verbose,
         )
         cmd.extend([" ", docker_native])
     return "".join(cmd)
 
 
 @pass_environment
 def execute_bootstraps(ctx, modules=[]):
@@ -337,15 +344,15 @@
             containers.append(container_name)
     return containers
 
 
 @pass_environment
 def execute_container_bootstrap(ctx, bootstrap="", container_name="", yaml_file=""):
     """Executes a single bootstrap inside a container. If the
-    `/opt/minitrino/bootstrap_status.txt` file has the same checksum as the
+    `/opt/minitrino/bootstrap-status.txt` file has the same checksum as the
     bootstrap script that is about to be executed, the boostrap script is
     skipped.
 
     Returns `False` if the script is not executed and `True` if it is."""
 
     if any((not bootstrap, not container_name, not yaml_file)):
         raise utils.handle_missing_param(list(locals().keys()))
@@ -362,363 +369,327 @@
     # Add executable permissions to bootstrap
     st = os.stat(bootstrap_file)
     os.chmod(
         bootstrap_file,
         st.st_mode | stat.S_IXUSR | stat.S_IXGRP | stat.S_IXOTH,
     )
 
-    bootstrap_checksum = hashlib.md5(open(bootstrap_file, "rb").read()).hexdigest()
+    checksum = hashlib.md5(open(bootstrap_file, "rb").read()).hexdigest()
     container = ctx.docker_client.containers.get(container_name)
 
     # Check if this script has already been executed
     output = ctx.cmd_executor.execute_commands(
-        "cat /opt/minitrino/bootstrap_status.txt",
-        suppress_output=True,
+        "cat /opt/minitrino/bootstrap-status.txt",
         container=container,
         trigger_error=False,
     )
 
-    if f"{bootstrap_checksum}" in output[0].get("output", ""):
-        ctx.logger.log(
+    if f"{checksum}" in output[0].get("output", ""):
+        ctx.logger.verbose(
             f"Bootstrap already executed in container '{container_name}'. Skipping.",
-            level=ctx.logger.verbose,
         )
         return False
 
-    ctx.logger.log(
+    ctx.logger.verbose(
         f"Executing bootstrap script in container '{container_name}'...",
-        level=ctx.logger.verbose,
     )
 
     ctx.cmd_executor.execute_commands(
         f"docker cp {bootstrap_file} {container_name}:/tmp/"
     )
 
     # Record executed file checksum
     ctx.cmd_executor.execute_commands(
         f"/tmp/{os.path.basename(bootstrap_file)}",
-        f'bash -c "echo {bootstrap_checksum} >> /opt/minitrino/bootstrap_status.txt"',
+        f'bash -c "echo {checksum} >> /opt/minitrino/bootstrap-status.txt"',
         container=container,
     )
 
-    ctx.logger.log(
+    ctx.logger.verbose(
         f"Successfully executed bootstrap script in container '{container_name}'.",
-        level=ctx.logger.verbose,
     )
 
     return True
 
 
+def split_cfg(cfgs=""):
+    cfgs = cfgs.strip().split("\n")
+    for i, cfg in enumerate(cfgs):
+        cfg = re.sub(r"\s*=\s*", "=", cfg)
+        cfgs[i] = cfg.split("=", 1)
+    return cfgs
+
+
 @pass_environment
-def check_dup_configs(ctx):
-    """Checks for duplicate configs in Trino config files (jvm.config and
-    config.properties). This is a safety check for modules that may improperly
-    modify these files.
+def get_current_trino_cfgs(ctx):
+    """Get Trino config.properties and jvm.config files. Return the two sets of
+    configs as lists, e.g.:
 
-    Duplicates will only be registered for JVM config if the configs are
-    identical. For config.properties, duplicates will be registered if there are
-    multiple overlapping property keys."""
-
-    check_files = [TRINO_CONFIG, TRINO_JVM_CONFIG]
-    for check_file in check_files:
-        ctx.logger.log(
-            f"Checking Trino {check_file} for duplicate configs...",
-            level=ctx.logger.verbose,
-        )
-        container = ctx.docker_client.containers.get("trino")
-        output = ctx.cmd_executor.execute_commands(
-            f"cat {ETC_TRINO}/{check_file}",
-            suppress_output=True,
-            container=container,
-        )
+    [['a', 'b'], ['c', 'd'], ['e', 'f']]
+    """
 
-        configs = output[0].get("output", "")
-        if not configs:
-            raise err.MinitrinoError(
-                f"Trino {check_file} file unable to be read from Trino container."
-            )
+    current_cfgs = ctx.cmd_executor.execute_commands(
+        f"cat {ETC_TRINO}/{TRINO_CONFIG}",
+        f"cat {ETC_TRINO}/{TRINO_JVM_CONFIG}",
+        container=ctx.docker_client.containers.get("trino"),
+        suppress_output=True,
+    )
 
-        configs = configs.strip().split("\n")
-        configs.sort()
+    current_trino_cfgs = split_cfg(current_cfgs[0].get("output", ""))
+    current_jvm_cfg = split_cfg(current_cfgs[1].get("output", ""))
 
-        duplicates = []
-        if check_file == TRINO_CONFIG:
-            for i, config in enumerate(configs):
-                if config.startswith("#"):
-                    continue
-                config = utils.parse_key_value_pair(
-                    config, err_type=err.UserError, key_to_upper=False
-                )
-                if config is None:
-                    continue
-                if i + 1 != len(configs):
-                    next_config = utils.parse_key_value_pair(
-                        configs[i + 1], err_type=err.UserError, key_to_upper=False
-                    )
-                    if config[0] == next_config[0]:
-                        duplicates.extend(["=".join(config), "=".join(next_config)])
-                else:
-                    next_config = [""]
-                if config[0] == next_config[0]:
-                    duplicates.extend(["=".join(config), "=".join(next_config)])
-                elif duplicates:
-                    duplicates = set(duplicates)
-                    duplicates_string = "\n".join(duplicates)
-                    ctx.logger.log(
-                        f"Duplicate Trino configuration properties detected in "
-                        f"{check_file} file:\n{duplicates_string}",
-                        level=ctx.logger.warn,
-                    )
-                    duplicates = []
-        else:  # JVM config
-            for i, config in enumerate(configs):
-                config = config.strip()
-                if config.startswith("#") or not config:
-                    continue
-                if i + 1 != len(configs):
-                    next_config = configs[i + 1].strip()
-                else:
-                    next_config = ""
-                if config == next_config:
-                    duplicates.extend([config, next_config])
-                elif duplicates:
-                    duplicates_string = "\n".join(duplicates)
-                    ctx.logger.log(
-                        f"Duplicate Trino configuration properties detected in "
-                        f"{check_file} file:\n{duplicates_string}",
-                        level=ctx.logger.warn,
-                    )
-                    duplicates = []
+    return current_trino_cfgs, current_jvm_cfg
 
 
 @pass_environment
-def write_trino_configs(ctx, containers_to_restart=[], modules=[]):
+def write_trino_cfg(ctx, c_restart=[], modules=[]):
     """Appends Trino config from various modules if specified in the module YAML
     file. The Trino container is added to the restart list if any configs are
     written to files in the container."""
 
-    config_properties = []
-    jvm_config = []
+    def handle_password_authenticators(cfgs):
+        merge = []
+        for i, cfg in enumerate(cfgs):
+            if cfg[0] == "http-server.authentication.type":
+                merge.append(i)
+
+        if not merge:
+            return cfgs
+
+        auth_property = "http-server.authentication.type="
+        for i, cfg in enumerate(merge):
+            if i + 1 == len(merge):
+                auth_property += cfgs[cfg][1].upper()
+            else:
+                auth_property += f"{cfgs[cfg][1].upper()},"
+
+        cfgs = [x for i, x in enumerate(cfgs) if i not in merge]
+        cfgs.append(auth_property.split("="))
+        return cfgs
+
+    trino_container = ctx.docker_client.containers.get("trino")
+
+    if not trino_container:
+        raise err.MinitrinoError(
+            f"Attempting to append Trino configuration in Trino container, "
+            f"but no running Trino container was found."
+        )
+
+    cfgs = []
+    jvm_cfg = []
 
     for module in modules:
         yaml = ctx.modules.data.get(module, {}).get("yaml_dict")
-        conf = (
+        usr_cfgs = (
             yaml.get("services", {})
             .get("trino", {})
             .get("environment", {})
-            .get("CONFIG_PROPERTIES", {})
+            .get("CONFIG_PROPERTIES", [])
         )
-        jvm = (
+        user_jvm_cfg = (
             yaml.get("services", {})
             .get("trino", {})
             .get("environment", {})
-            .get("JVM_CONFIG", {})
+            .get("JVM_CONFIG", [])
         )
 
-        if conf:
-            config_properties.extend(conf.strip().split("\n"))
-        if jvm:
-            jvm_config.extend(jvm.strip().split("\n"))
+        if usr_cfgs:
+            cfgs.extend(split_cfg(usr_cfgs))
+        if user_jvm_cfg:
+            jvm_cfg.extend(split_cfg(user_jvm_cfg))
 
-    if not config_properties and not jvm_config:
-        return containers_to_restart
+    if not cfgs and not jvm_cfg:
+        return c_restart
 
-    ctx.logger.log(
-        "Appending user-defined Trino config to Trino container config...",
-        level=ctx.logger.verbose,
+    cfgs = handle_password_authenticators(cfgs)
+
+    checksum_file = "/opt/minitrino/user-config.txt"
+    checksum_data = bytes(str([cfgs, jvm_cfg]), "utf-8")
+    checksum = hashlib.md5(checksum_data).hexdigest()
+
+    output = ctx.cmd_executor.execute_commands(
+        f"cat {checksum_file}",
+        container=trino_container,
+        trigger_error=False,
     )
 
-    trino_container = ctx.docker_client.containers.get("trino")
-    if not trino_container:
-        raise err.MinitrinoError(
-            f"Attempting to append Trino configuration in Trino container, "
-            f"but no running Trino container was found."
-        )
+    old_checksum = output[0].get("output", "").strip().lower()
+    if not "no such file or directory" in old_checksum:
+        if old_checksum == checksum:
+            ctx.logger.verbose(
+                "User-defined config already added to config files. Skipping...",
+            )
+            return c_restart
 
-    ctx.logger.log(
+    ctx.logger.verbose(
         "Checking Trino server status before updating configs...",
-        level=ctx.logger.verbose,
     )
+
     retry = 0
     while retry <= 30:
         logs = trino_container.logs().decode()
         if "======== SERVER STARTED ========" in logs:
+            ctx.logger.verbose(
+                "Trino server started.",
+            )
             break
         elif trino_container.status != "running":
             raise err.MinitrinoError(
                 f"Trino container stopped running. Inspect the container logs if the "
                 f"container is still available. If the container was rolled back, rerun "
                 f"the command with the '--no-rollback' option, then inspect the logs."
             )
         else:
-            ctx.logger.log(
-                "Trino server has not started. Waiting one second and trying again...",
-                level=ctx.logger.verbose,
+            ctx.logger.verbose(
+                "Waiting for Trino server to start...",
             )
             time.sleep(1)
             retry += 1
 
-    current_configs = ctx.cmd_executor.execute_commands(
-        f"cat {ETC_TRINO}/{TRINO_CONFIG}",
-        f"cat {ETC_TRINO}/{TRINO_JVM_CONFIG}",
-        container=trino_container,
-        suppress_output=True,
-    )
-
-    current_trino_config = current_configs[0].get("output", "").strip().split("\n")
-    current_jvm_config = current_configs[1].get("output", "").strip().split("\n")
+    def append_cfgs(trino_container, usr_cfgs, current_cfgs, filename):
+        """If there is an overlapping config key, replace it with the user
+        config."""
 
-    def append_configs(user_configs, current_configs, filename):
-        # If there is an overlapping config key, replace it with the user
-        # config. If there is not overlapping config key, append it to the
-        # current config list.
-
-        # No additional configs, leave the file in the container alone
-        if not user_configs:
+        if not usr_cfgs:
             return
 
-        if filename == TRINO_CONFIG:
-            for user_config in user_configs:
-                user_config = utils.parse_key_value_pair(
-                    user_config, err_type=err.UserError, key_to_upper=False
-                )
-                if user_config is None:
-                    continue
-                for i, current_config in enumerate(current_configs):
-                    if current_config.startswith("#"):
-                        continue
-                    current_config = utils.parse_key_value_pair(
-                        current_config, err_type=err.UserError, key_to_upper=False
-                    )
-                    if current_config is None:
-                        continue
-                    if user_config[0] == current_config[0]:
-                        current_configs[i] = "=".join(user_config)
-                        break
-                    if (
-                        i + 1 == len(current_configs)
-                        and not "=".join(user_config) in current_configs
-                    ):
-                        current_configs.append("=".join(user_config))
-        else:
-            for user_config in user_configs:
-                user_config = user_config.strip()
-                if not user_config:
-                    continue
-                for i, current_config in enumerate(current_configs):
-                    if current_config.startswith("#"):
-                        continue
-                    current_config = current_config.strip()
-                    if not current_config:
-                        continue
-                    if user_config == current_config:
-                        current_configs[i] = user_config
-                        break
-                    if (
-                        i + 1 == len(current_configs)
-                        and not user_config in current_configs
-                    ):
-                        current_configs.append(user_config)
+        current_cfgs = [
+            cfg
+            for cfg in current_cfgs
+            if not any(cfg[0] == usr_cfg[0] for usr_cfg in usr_cfgs)
+        ]
+
+        current_cfgs.extend(usr_cfgs)
+        current_cfgs = ["=".join(x) for x in current_cfgs]
 
-        ctx.logger.log(
+        ctx.logger.verbose(
             f"Removing existing {filename} file...",
-            level=ctx.logger.verbose,
         )
         ctx.cmd_executor.execute_commands(
             f"rm {ETC_TRINO}/{filename}", container=trino_container
         )
 
-        ctx.logger.log(
+        ctx.logger.verbose(
             f"Writing new config to {filename}...",
-            level=ctx.logger.verbose,
         )
-        for current_config in current_configs:
-            append_config = (
-                f'bash -c "cat <<EOT >> {ETC_TRINO}/{filename}\n{current_config}\nEOT"'
+        for current_cfg in current_cfgs:
+            append_cfg = (
+                f'bash -c "cat <<EOT >> {ETC_TRINO}/{filename}\n{current_cfg}\nEOT"'
             )
             ctx.cmd_executor.execute_commands(
-                append_config, container=trino_container, suppress_output=True
+                append_cfg, container=trino_container, suppress_output=True
             )
 
-    append_configs(config_properties, current_trino_config, TRINO_CONFIG)
-    append_configs(jvm_config, current_jvm_config, TRINO_JVM_CONFIG)
+    ctx.logger.verbose(
+        "Appending user-defined Trino config to Trino container config...",
+    )
+
+    current_trino_cfgs, current_jvm_cfg = get_current_trino_cfgs()
+    append_cfgs(trino_container, cfgs, current_trino_cfgs, TRINO_CONFIG)
+    append_cfgs(trino_container, jvm_cfg, current_jvm_cfg, TRINO_JVM_CONFIG)
+
+    if not "trino" in c_restart:
+        c_restart.append("trino")
 
-    if not "trino" in containers_to_restart:
-        containers_to_restart.append("trino")
+    ctx.logger.verbose("Recording config checksum...")
+    output = ctx.cmd_executor.execute_commands(
+        f'bash -c "echo {checksum} > {checksum_file}"', container=trino_container
+    )
 
-    return containers_to_restart
+    return c_restart
 
 
 @pass_environment
-def restart_containers(ctx, containers_to_restart=[]):
+def check_dup_cfgs(ctx):
+    """Checks for duplicate configs in Trino config files (jvm.config and
+    config.properties). This is a safety check for modules that may improperly
+    modify these files."""
+
+    def log_duplicates(cfgs, filename):
+        ctx.logger.verbose(
+            f"Checking Trino '{filename}' file for duplicate configs...",
+        )
+
+        unique = {}
+        for cfg in cfgs:
+            key = cfg[0]
+            if key in unique:
+                unique[key].append(cfg)
+            else:
+                unique[key] = [cfg]
+
+        duplicates = ["=".join(x) for y in unique.values() for x in y if len(y) > 1]
+
+        if duplicates:
+            ctx.logger.warn(
+                f"Duplicate Trino configuration properties detected in "
+                f"'{filename}' file:\n{str(duplicates)}",
+            )
+
+    current_trino_cfgs, current_jvm_cfg = get_current_trino_cfgs()
+
+    log_duplicates(current_trino_cfgs, TRINO_CONFIG)
+    log_duplicates(current_jvm_cfg, TRINO_JVM_CONFIG)
+
+
+@pass_environment
+def restart_containers(ctx, c_restart=[]):
     """Restarts all the containers in the list."""
 
-    if containers_to_restart == []:
+    if c_restart == []:
         return
 
-    # Remove any duplicates
-    containers_to_restart = list(set(containers_to_restart))
+    c_restart = list(set(c_restart))
 
-    for container in containers_to_restart:
+    for container in c_restart:
         try:
             container = ctx.docker_client.containers.get(container)
-            ctx.logger.log(
-                f"Restarting container '{container.name}'...", level=ctx.logger.verbose
-            )
+            ctx.logger.verbose(f"Restarting container '{container.name}'...")
             container.restart()
         except NotFound:
             raise err.MinitrinoError(
                 f"Attempting to restart container '{container.name}', but the container was not found."
             )
 
 
 @pass_environment
 def initialize_containers(ctx):
-    """Initializes each container with /opt/minitrino/bootstrap_status.txt."""
+    """Initializes each container with /opt/minitrino/ directory."""
 
     containers = ctx.docker_client.containers.list(filters={"label": RESOURCE_LABEL})
     for container in containers:
         output = ctx.cmd_executor.execute_commands(
-            "cat /opt/minitrino/bootstrap_status.txt",
-            suppress_output=True,
+            "mkdir -p /opt/minitrino/",
             container=container,
             trigger_error=False,
         )
-        output_string = output[0].get("output", "").strip()
-        if "no such file or directory" in output_string.lower():
-            ctx.cmd_executor.execute_commands(
-                "mkdir -p /opt/minitrino/",
-                "touch /opt/minitrino/bootstrap_status.txt",
-                container=container,
-            )
-        elif output[0].get("return_code", None) == 0:
+        if output[0].get("return_code", None) in [0, 126]:
             continue
         else:
             raise err.MinitrinoError(
                 f"Command failed.\n"
-                f"Output: {output_string}\n"
+                f"Output: {output[0].get('output', '').strip()}\n"
                 f"Exit code: {output[0].get('return_code', None)}"
             )
 
 
 @pass_environment
-def rollback_provision(ctx, no_rollback):
+def rollback(ctx, no_rollback):
     """Rolls back the provisioning command in the event of an error."""
 
     if no_rollback:
-        ctx.logger.log(
+        ctx.logger.warn(
             f"Errors occurred during environment provisioning and rollback has been disabled. "
             f"Provisioned resources will remain in an unaltered state.",
-            level=ctx.logger.warn,
         )
         return
-    ctx.logger.log(
+
+    ctx.logger.warn(
         f"Rolling back provisioned resources due to "
         f"errors encountered while provisioning the environment.",
-        level=ctx.logger.warn,
     )
 
     containers = ctx.docker_client.containers.list(
         filters={"label": RESOURCE_LABEL}, all=True
     )
 
     for container in containers:
```

### Comparing `minitrino-2.0.3/minitrino/cmd/cmd_remove.py` & `minitrino-2.0.4/minitrino/cmd/cmd_remove.py`

 * *Files 11% similar despite different names*

```diff
@@ -63,23 +63,23 @@
         response = ctx.logger.prompt_msg(
             "You are about to all remove minitrino images and volumes. Continue? [Y/N]"
         )
         if utils.validate_yes(response):
             remove_items(IMAGE, force)
             remove_items(VOLUME, force)
         else:
-            ctx.logger.log(f"Opted to skip resource removal.")
+            ctx.logger.info(f"Opted to skip resource removal.")
             sys.exit(0)
 
     if images:
         remove_items(IMAGE, force, labels)
     if volumes:
         remove_items(VOLUME, force, labels)
 
-    ctx.logger.log(f"Removal complete.")
+    ctx.logger.info(f"Removal complete.")
 
 
 @pass_environment
 def remove_items(ctx, item_type, force, labels=[]):
     """Removes Docker items. If no labels are passed in, all Minitrino
     resources are removed. If label(s) are passed in, the removal is limited to
     the passed in labels."""
@@ -103,42 +103,38 @@
             )
             if force:
                 ctx.docker_client.images.remove(
                     image.short_id, force=True, noprune=False
                 )
             else:
                 ctx.docker_client.images.remove(image.short_id)
-            ctx.logger.log(
+            ctx.logger.verbose(
                 f"{item_type.title()} removed: {identifier}",
-                level=ctx.logger.verbose,
             )
         except APIError as e:
-            ctx.logger.log(
+            ctx.logger.verbose(
                 f"Cannot remove image: {identifier}\n"
                 f"Error from Docker: {e.explanation}",
-                level=ctx.logger.verbose,
             )
 
     volumes = list(set(volumes))
     for volume in volumes:
         try:
             identifier = utils.generate_identifier({"ID": volume.id})
             if force:
                 volume.remove(force=True)
             else:
                 volume.remove()
-            ctx.logger.log(
+            ctx.logger.verbose(
                 f"{item_type.title()} removed: {identifier}",
-                level=ctx.logger.verbose,
             )
         except APIError as e:
-            ctx.logger.log(
+            ctx.logger.verbose(
                 f"Cannot remove volume: {identifier}\n"
                 f"Error from Docker: {e.explanation}",
-                level=ctx.logger.verbose,
             )
 
 
 def try_get_image_tag(image):
     """Tries to get an image tag. If there is no tag, returns an empty string."""
 
     try:
```

### Comparing `minitrino-2.0.3/minitrino/cmd/cmd_snapshot.py` & `minitrino-2.0.4/minitrino/cmd/cmd_snapshot.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,30 +103,29 @@
     if not directory:
         directory = os.path.join(ctx.minitrino_lib_dir, "snapshots")
 
     validate_name(name)
     check_exists(name, directory, force)
 
     if modules:
-        ctx.logger.log(f"Creating snapshot of specified modules...")
+        ctx.logger.info(f"Creating snapshot of specified modules...")
         snapshot_runner(name, no_scrub, False, modules, directory)
     else:
         modules = ctx.modules.get_running_modules()
         if not modules:
-            ctx.logger.log(
+            ctx.logger.verbose(
                 f"No running Minitrino modules to snapshot. Snapshotting "
                 f"Trino resources only.",
-                level=ctx.logger.verbose,
             )
         else:
-            ctx.logger.log(f"Creating snapshot of active environment...")
+            ctx.logger.info(f"Creating snapshot of active environment...")
         snapshot_runner(name, no_scrub, True, modules, directory)
 
     check_complete(name, directory)
-    ctx.logger.log(
+    ctx.logger.info(
         f"Snapshot complete and saved at path: {os.path.join(directory, name)}.tar.gz"
     )
 
 
 @pass_environment
 def validate_name(ctx, name):
     """Validates the chosen filename for correct input."""
@@ -150,38 +149,35 @@
 
     snapshot_file = os.path.abspath(os.path.join(directory, f"{name}.tar.gz"))
     if os.path.isfile(snapshot_file):
         response = ctx.logger.prompt_msg(
             f"Snapshot file {name}.tar.gz already exists. Overwrite? [Y/N]"
         )
         if not utils.validate_yes(response):
-            ctx.logger.log(f"Opted to skip snapshot.")
+            ctx.logger.info(f"Opted to skip snapshot.")
             sys.exit(0)
 
 
 @pass_environment
 def prepare_snapshot_dir(ctx, name, active, no_scrub, modules):
     """Checks if the snapshot temp directory exists. If it does, clears
     files/directories inside of it. If it doesn't, (1) creates it and clones the
     library structure, (2) adds a Bash file that can be executed to spin up the
     environment as it was snapshotted.
 
     Returns the absolute path of the named snapshot directory."""
 
     if os.path.isdir(ctx.snapshot_dir):
-        ctx.logger.log(
+        ctx.logger.verbose(
             "Snapshot temp directory exists. Removing and recreating...",
-            level=ctx.logger.verbose,
         )
         shutil.rmtree(ctx.snapshot_dir)
         os.mkdir(ctx.snapshot_dir)
     else:
-        ctx.logger.log(
-            "Snapshot directory does not exist. Creating...", level=ctx.logger.verbose
-        )
+        ctx.logger.verbose("Snapshot directory does not exist. Creating...")
         os.mkdir(ctx.snapshot_dir)
 
     snapshot_name_dir = clone_lib_dir(name)
     handle_copy_config_file(snapshot_name_dir, no_scrub)
     build_snapshot_command(snapshot_name_dir, modules, active)
 
     return snapshot_name_dir
@@ -220,17 +216,16 @@
 @pass_environment
 def create_snapshot_command_file(ctx, command_string="", snapshot_name_dir=""):
     """Creates an .sh file in the minitrino directory for usage by the snapshot
     command. This way, a similar command used to provision the environment is
     preserved."""
 
     file_dest = os.path.join(snapshot_name_dir, "provision-snapshot.sh")
-    ctx.logger.log(
+    ctx.logger.verbose(
         f"Creating snapshot command to file at path: {file_dest}",
-        level=ctx.logger.verbose,
     )
 
     # Create provisioning command snapshot file from template and make it
     # executable
     try:
         with open(file_dest, "w") as provision_command_file:
             provision_command_file.write(PROVISION_SNAPSHOT_TEMPLATE.lstrip())
@@ -290,30 +285,29 @@
     if no_scrub:
         response = ctx.logger.prompt_msg(
             f"All sensitive information in user config will be added to the snapshot. Continue? [Y/N]"
         )
         if utils.validate_yes(response):
             copy_config_file(snapshot_name_dir, no_scrub)
         else:
-            ctx.logger.log(f"Opted to scrub sensitive user config data.")
+            ctx.logger.info(f"Opted to scrub sensitive user config data.")
             copy_config_file(snapshot_name_dir)
     else:
         copy_config_file(snapshot_name_dir)
 
 
 @pass_environment
 def copy_config_file(ctx, snapshot_name_dir, no_scrub=False):
     """Copies user config file to the named snapshot directory."""
 
     if os.path.isfile(ctx.config_file):
         shutil.copy(ctx.config_file, snapshot_name_dir)
     else:
-        ctx.logger.log(
+        ctx.logger.warn(
             f"No user config file at path: {ctx.config_file}. Will not be added to snapshot.",
-            level=ctx.logger.warn,
         )
         return
 
     if not no_scrub:
         scrub_config_file(snapshot_name_dir)
 
 
@@ -325,17 +319,16 @@
     if os.path.isfile(snapshot_config_file):
         for line in fileinput.input(snapshot_config_file, inplace=True):
             if "=" in line:
                 print(line.replace(line, scrub_line(line)))
             else:
                 print(line.replace(line, line.rstrip()))
     else:
-        ctx.logger.log(
+        ctx.logger.warn(
             f"No user config file at path: {ctx.config_file}. Nothing to scrub.",
-            level=ctx.logger.warn,
         )
 
 
 @pass_environment
 def scrub_line(ctx, line):
     """Scrubs a line from a snapshot config file. Returns the scrubbed line."""
```

### Comparing `minitrino-2.0.3/minitrino/cmd/cmd_version.py` & `minitrino-2.0.4/minitrino/cmd/cmd_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,14 @@
 )
 @utils.exception_handler
 @pass_environment
 def cli(ctx):
     """Version command for Minitrino."""
 
     cli_version = utils.get_cli_ver()
-    ctx.logger.log(f"Minitrino version: {cli_version}")
+    ctx.logger.info(f"Minitrino version: {cli_version}")
 
     try:
         lib_version = utils.get_lib_ver(ctx.minitrino_lib_dir)
-        ctx.logger.log(f"Library version: {lib_version}")
+        ctx.logger.info(f"Library version: {lib_version}")
     except:
-        ctx.logger.log("Library version: NOT INSTALLED")
+        ctx.logger.info("Library version: NOT INSTALLED")
```

### Comparing `minitrino-2.0.3/minitrino/components.py` & `minitrino-2.0.4/minitrino/components.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 from pathlib import Path
 from configparser import ConfigParser
 
 from minitrino import utils
 from minitrino import errors as err
 from minitrino.settings import RESOURCE_LABEL
-from minitrino.settings import MODULE_LABEL_KEY_ROOT
 from minitrino.settings import MODULE_ROOT
 from minitrino.settings import MODULE_ADMIN
 from minitrino.settings import MODULE_SECURITY
 from minitrino.settings import MODULE_CATALOG
 
 
 class Environment:
@@ -125,34 +124,32 @@
         # Instantiate/update interactive attributes
         self.logger = utils.Logger(self.verbose)
         self.env = EnvironmentVariables(self)
 
         # Skip the library-related procedures if the library is not found
         try:
             if self.minitrino_lib_dir:
-                self.logger.log(
+                self.logger.verbose(
                     f"Library path set to: {self.minitrino_lib_dir}",
-                    level=self.logger.verbose,
                 )
 
             # Now that we know where the library is, we can try to parse the env
             # file and obtain all of the modules
             self.env._parse_library_env()
             self.modules = Modules(self)
 
             # Warn the user if the library and CLI vers don't match
             cli_ver = utils.get_cli_ver()
             lib_ver = utils.get_lib_ver(self.minitrino_lib_dir)
             if cli_ver != lib_ver:
-                self.logger.log(
+                self.logger.warn(
                     f"CLI version {cli_ver} and library version {lib_ver} "
                     f"do not match. You can update the Minitrino library "
                     f"version to match the CLI version by running 'minitrino "
                     f"lib_install'.",
-                    level=self.logger.warn,
                 )
         except:
             pass
 
         self.env._log_env_vars()
         self.cmd_executor = CommandExecutor(self)
         self._get_docker_clients()
@@ -172,33 +169,34 @@
     def _get_config_file(self):
         """Returns the correct filepath for the minitrino.cfg file. Adds to
         initialization warnings if the file does not exist, but will return the
         path regardless."""
 
         config_file = os.path.join(self.minitrino_user_dir, "minitrino.cfg")
         if not os.path.isfile(config_file):
-            self.logger.log(
+            self.logger.warn(
                 f"No minitrino.cfg file found at {config_file}. "
                 f"Run 'minitrino config' to reconfigure this file and directory.",
-                level=self.logger.warn,
             )
         return config_file
 
     def _get_docker_clients(self):
         """Gets DockerClient and APIClient objects. Returns a tuple of DockerClient
         and APIClient objects, respectively.
 
         If there is an error fetching the clients, None types will be returned
         for each client. The lack of clients should be caught by check_daemon()
         calls that execute in each command that requires an accessible Docker
         service."""
 
+        docker_url = os.environ.get("DOCKER_HOST", "")
+
         try:
-            docker_client = docker.DockerClient(base_url="")
-            api_client = docker.APIClient(base_url="")
+            docker_client = docker.DockerClient(base_url=docker_url)
+            api_client = docker.APIClient(base_url=docker_url)
             self.docker_client, self.api_client = docker_client, api_client
         except:
             return None, None
 
 
 class EnvironmentVariables:
     """Gathers all Minitrino variables into a single source of truth.
@@ -213,15 +211,15 @@
     ### Public Methods
     - `get_var()`: Gets an environment variable from a specific section and key.
     - `get_section()`: Gets a a section from the environment variable dict.
 
     ### Usage
     ```python
     # ctx object has an instantiated EnvironmentVariables object
-    env_variable = ctx.env.get_var("STARBURST_VER", "370-e")
+    env_variable = ctx.env.get_var("STARBURST_VER", "388-e")
     env_section = ctx.env.get_section("MODULES")
     ```"""
 
     @utils.exception_handler
     def __init__(self, ctx=None):
         if not ctx:
             raise utils.handle_missing_param(list(locals().keys()))
@@ -368,17 +366,16 @@
             for k, v in user_env_dict.items():
                 self.env["EXTRA"][k] = v
 
     def _log_env_vars(self):
         """Logs environment variables."""
 
         if self.env:
-            self._ctx.logger.log(
+            self._ctx.logger.verbose(
                 f"Registered environment variables:\n{json.dumps(self.env, indent=2)}",
-                level=self._ctx.logger.verbose,
             )
 
 
 class Modules:
     """Contains information about all valid Minitrino modules.
 
     ### Parameters
@@ -427,27 +424,28 @@
             if not label_set and container.name != "trino":
                 raise err.UserError(
                     f"Missing Minitrino labels for container '{container.name}'.",
                     f"Check this module's 'docker-compose.yml' file and ensure you are "
                     f"following the documentation on labels.",
                 )
 
+        modules = set(modules)
         for module in modules:
             if not isinstance(self.data.get(module), dict):
                 raise err.UserError(
                     f"Module '{module}' is running, but it is not found "
                     f"in the library. Was it deleted, or are you pointing "
                     f"Minitrino to the wrong location?"
                 )
         return modules
 
     def _load_modules(self):
         """Loads module data during instantiation."""
 
-        self._ctx.logger.log("Loading modules...", level=self._ctx.logger.verbose)
+        self._ctx.logger.verbose("Loading modules...")
 
         modules_dir = os.path.join(self._ctx.minitrino_lib_dir, MODULE_ROOT)
         if not os.path.isdir(modules_dir):
             raise err.MinitrinoError(
                 f"Path is not a directory: {modules_dir}. "
                 f"Are you pointing to a compatible Minitrino library?"
             )
@@ -460,18 +458,17 @@
         ]
 
         for section_dir in sections:
             for _dir in os.listdir(section_dir):
                 module_dir = os.path.join(section_dir, _dir)
 
                 if not os.path.isdir(module_dir):
-                    self._ctx.logger.log(
+                    self._ctx.logger.verbose(
                         f"Skipping file (expected a directory, not a file) "
                         f"at path: {module_dir}",
-                        level=self._ctx.logger.verbose,
                     )
                     continue
 
                 # List inner-module files
                 module_files = os.listdir(module_dir)
 
                 yaml_basename = f"{os.path.basename(module_dir)}.yml"
@@ -502,18 +499,17 @@
                 json_basename = "metadata.json"
                 json_file = os.path.join(module_dir, json_basename)
                 metadata = {}
                 if os.path.isfile(json_file):
                     with open(json_file) as f:
                         metadata = json.load(f)
                 else:
-                    self._ctx.logger.log(
+                    self._ctx.logger.verbose(
                         f"No JSON metadata file for module '{module_name}'. "
                         f"Will not load metadata for module.",
-                        level=self._ctx.logger.verbose,
                     )
                 for k, v in metadata.items():
                     self.data[module_name][k] = v
 
 
 class CommandExecutor:
     """Executes commands in the host shell/host containers with customized
@@ -575,17 +571,16 @@
                 output.append(self._execute_in_shell(command, **kwargs))
 
         return output
 
     def _execute_in_shell(self, command="", **kwargs):
         """Executes a command in the host shell."""
 
-        self._ctx.logger.log(
+        self._ctx.logger.verbose(
             f"Executing command in shell:\n{command}",
-            level=self._ctx.logger.verbose,
         )
 
         process = subprocess.Popen(
             command,
             shell=True,
             env=kwargs.get("environment", {}),
             stdout=subprocess.PIPE,
@@ -596,29 +591,26 @@
         if not kwargs.get("suppress_output", False):
             # Stream the output of the executed command line-by-line.
             # `universal_newlines=True` ensures output is generated as a string,
             # so there is no need to decode bytes. The only cleansing we need to
             # do is to run the string through the `_strip_ansi()` function.
 
             started_stream = False
+            output = ""
             while True:
                 output_line = process.stdout.readline()
                 if output_line == "" and process.poll() is not None:
                     break
                 output_line = self._strip_ansi(output_line)
                 if not started_stream:
-                    self._ctx.logger.log(
-                        "Command Output:", level=self._ctx.logger.verbose
-                    )
+                    self._ctx.logger.verbose("Command Output:")
                     started_stream = True
-                self._ctx.logger.log(
-                    output_line, level=self._ctx.logger.verbose, stream=True
-                )
+                self._ctx.logger.verbose(output_line, stream=True)
+                output += output_line
 
-        output, _ = process.communicate()  # Get full output (stdout + stderr)
         if process.returncode != 0 and kwargs.get("trigger_error", True):
             raise err.MinitrinoError(
                 f"Failed to execute shell command:\n{command}\n"
                 f"Exit code: {process.returncode}"
             )
 
         return {
@@ -635,17 +627,16 @@
         if container is None:
             raise err.MinitrinoError(
                 f"Attempted to execute a command inside of a "
                 f"container, but a container object was not provided."
             )
 
         if not kwargs.get("suppress_output"):
-            self._ctx.logger.log(
+            self._ctx.logger.verbose(
                 f"Executing command in container '{container.name}':\n{command}",
-                level=self._ctx.logger.verbose,
             )
 
         # Create exec handler and execute the command
         exec_handler = self._ctx.api_client.exec_create(
             container.name,
             cmd=command,
             environment=kwargs.get("environment", {}),
@@ -670,35 +661,38 @@
             chunk = self._strip_ansi(chunk.decode())
             output += chunk
             chunk = chunk.split("\n", 1)
             if len(chunk) > 1:  # Indicates newline present
                 full_line += chunk[0]
                 if not kwargs.get("suppress_output", False):
                     if not started_stream:
-                        self._ctx.logger.log(
-                            "Command Output:", level=self._ctx.logger.verbose
-                        )
+                        self._ctx.logger.verbose("Command Output:")
                         started_stream = True
-                    self._ctx.logger.log(
-                        full_line, level=self._ctx.logger.verbose, stream=True
-                    )
+                    self._ctx.logger.verbose(full_line, stream=True)
                     full_line = ""
                 if chunk[1]:
                     full_line = chunk[1]
             else:
                 full_line += chunk[0]
 
         # Catch lingering full line post-loop
         if not kwargs.get("suppress_output", False) and full_line:
-            self._ctx.logger.log(full_line, level=self._ctx.logger.verbose, stream=True)
+            self._ctx.logger.verbose(full_line, stream=True)
 
         # Get the exit code
         return_code = self._ctx.api_client.exec_inspect(exec_handler["Id"]).get(
             "ExitCode"
         )
+        # https://www.gnu.org/software/bash/manual/html_node/Exit-Status.html
+        if return_code == 126:
+            self._ctx.logger.warn(
+                f"The command exited with a 126 code which typically means an "
+                f"executable is not accessible or installed. Does this image have "
+                f"all required dependencies installed?\nCommand: {command}",
+            )
 
         if return_code != 0 and kwargs.get("trigger_error", True):
             raise err.MinitrinoError(
                 f"Failed to execute command in container '{container.name}':\n{command}\n"
                 f"Exit code: {return_code}"
             )
```

### Comparing `minitrino-2.0.3/minitrino/errors.py` & `minitrino-2.0.4/minitrino/errors.py`

 * *Files identical despite different names*

### Comparing `minitrino-2.0.3/minitrino/settings.py` & `minitrino-2.0.4/minitrino/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 LIB = "lib"
 MODULE_ROOT = "modules"
 MODULE_ADMIN = "admin"
 MODULE_CATALOG = "catalog"
 MODULE_SECURITY = "security"
 MODULE_RESOURCES = "resources"
 ETC_TRINO = "/etc/starburst"
-SEP_VOLUME_MOUNT = "${STARBURST_LIC_PATH}:/etc/starburst/starburstdata.license:ro"
+SEP_VOLUME_MOUNT = "${SEP_LIC_PATH}:${SEP_LIC_MOUNT_PATH}"
+SEP_LIC_MOUNT_PATH = "/etc/starburst/starburstdata.license:ro"
+DUMMY_LIC_MOUNT_PATH = "/etc/starburst/dummy.license:ro"
 TRINO_CONFIG = "config.properties"
 TRINO_JVM_CONFIG = "jvm.config"
 LIB_INDEPENDENT_CMDS = ["lib_install"]
 
 # Snapshots
 SNAPSHOT_ROOT_FILES = [
     "docker-compose.yml",
@@ -46,15 +48,15 @@
 # Templates
 CONFIG_TEMPLATE = """
 [CLI]
 LIB_PATH=
 TEXT_EDITOR=
 
 [MODULES]
-STARBURST_LIC_PATH=
+SEP_LIC_PATH=
 """
 
 PROVISION_SNAPSHOT_TEMPLATE = """
 #!/usr/bin/env bash
 
 # ------------------------------------------------------------------------------------
 # Below is the exact command used to provision the snapshotted environment. Run this
```

### Comparing `minitrino-2.0.3/minitrino/utils.py` & `minitrino-2.0.4/minitrino/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,40 +31,45 @@
     ### Public Attributes
     - `info`: Info log level.
     - `warn`: Warn log level.
     - `error`: Error log level.
     - `verbose`: Verbose log level.
 
     ### Public Methods
-    - `log()`: Logs a message to the user's terminal.
+    - `log()`: Logs a message to the user's terminal. Level must be specified,
+      defaults to INFO.
+    - `info()`: Logs an info message
+    - `warn()`: Logs a warning message
+    - `error()`: Logs an error message
+    - `verbose()`: Logs a verbose message
     - `prompt_msg()`: Logs a prompt message and returns the user's input."""
 
     def __init__(self, log_verbose=False):
-        self.info = {"prefix": "[i]  ", "prefix_color": "cyan"}
-        self.warn = {"prefix": "[w]  ", "prefix_color": "yellow"}
-        self.error = {"prefix": "[e]  ", "prefix_color": "red"}
-        self.verbose = {"prefix": "[i]  ", "prefix_color": "cyan", "verbose": True}
+        self.INFO = {"prefix": "[i]  ", "prefix_color": "cyan"}
+        self.WARN = {"prefix": "[w]  ", "prefix_color": "yellow"}
+        self.ERROR = {"prefix": "[e]  ", "prefix_color": "red"}
+        self.VERBOSE = {"prefix": "[i]  ", "prefix_color": "cyan", "verbose": True}
 
         self._log_verbose = log_verbose
 
     def log(self, *args, level=None, stream=False):
         """Logs messages to the user's console. Defaults to 'info' log level.
 
         ### Parameters
         - `*args`: Messages to log.
         - `level`: The level of the log message (info, warn, error, and
           verbose).
         - `stream`: If `True`, the logger will not apply a prefix to each line
           streamed to the console."""
 
         if not level:
-            level = self.info
+            level = self.INFO
 
         # Skip verbose messages unless verbose mode is enabled
-        if not self._log_verbose and level == self.verbose:
+        if not self._log_verbose and level == self.VERBOSE:
             return
 
         for msg in args:
             # Ensure the message can be a string
             try:
                 msg = str(msg)
             except:
@@ -83,14 +88,26 @@
                     msg_prefix = style(
                         level.get("prefix", ""),
                         fg=level.get("prefix_color", ""),
                         bold=True,
                     )
                 echo(f"{msg_prefix}{msg}")
 
+    def info(self, *args, stream=False):
+        self.log(*args, level=self.INFO, stream=stream)
+
+    def warn(self, *args, stream=False):
+        self.log(*args, level=self.WARN, stream=stream)
+
+    def error(self, *args, stream=False):
+        self.log(*args, level=self.ERROR, stream=stream)
+
+    def verbose(self, *args, stream=False):
+        self.log(*args, level=self.VERBOSE, stream=stream)
+
     def prompt_msg(self, msg="", input_type=str):
         """Logs a prompt message and returns the user's input.
 
         ### Parameters
         - `msg`: The prompt message
         - `input_type`: The object type to check the input for"""
 
@@ -100,15 +117,15 @@
         try:
             msg = str(msg)
         except:
             raise err.MinitrinoError(f"A string is required for {self.log.__name__}.")
 
         msg = self._format(msg)
         styled_prefix = style(
-            self.info.get("prefix", ""), fg=self.info.get("prefix_color", ""), bold=True
+            self.INFO.get("prefix", ""), fg=self.INFO.get("prefix_color", ""), bold=True
         )
 
         return prompt(
             f"{styled_prefix}{msg}",
             type=input_type,
         )
 
@@ -161,15 +178,15 @@
     else:
         raise err.MinitrinoError(
             f"Invalid type given to 'e' parameter of {handle_exception.__name__}. "
             f"Expected an Exception type, but got type {type(error).__name__}"
         )
 
     logger = Logger()
-    logger.log(additional_msg, error_msg, level=logger.error)
+    logger.error(additional_msg, error_msg)
     if not skip_traceback:
         echo()  # Force a newline
         echo(f"{traceback.format_exc()}", err=True)
 
     sys.exit(exit_code)
 
 
@@ -241,20 +258,20 @@
 
 def check_starburst_ver(ctx):
     """Checks if a proper Starburst version is provided."""
 
     starburst_ver = ctx.env.get_var("STARBURST_VER", "")
     error_msg = (
         f"Provided Starburst version '{starburst_ver}' is invalid. "
-        f"The provided version must be 370-e or higher."
+        f"The provided version must be 388-e or higher."
     )
 
     try:
         starburst_ver_int = int(starburst_ver[0:3])
-        if starburst_ver_int < 370 or "-e" not in starburst_ver:
+        if starburst_ver_int < 380 or "-e" not in starburst_ver:
             raise err.UserError(error_msg)
     except:
         raise err.UserError(error_msg)
 
 
 def generate_identifier(identifiers=None):
     """Returns an 'object identifier' string used for creating log messages,
@@ -284,15 +301,15 @@
 ):
     """Parses a key-value pair in string form and returns the resulting pair as
     both a 2-element list. If the string cannot be split by "=", a
     MinitrinoError is raised.
 
     ### Parameters
     - `key_value_pair`: A string formatted as a key-value pair, i.e.
-      `"STARBURST_VER=370-e"`.
+      `"STARBURST_VER=388-e"`.
     - `err_type`: The exception to raise if an "=" delimiter is not in the
       key-value pair. Defaults to `MinitrinoError`.
     - `key_to_upper`: If `True`, the key will be forced to uppercase.
 
     ### Return Values
     - A list `[k, v]`, but will return `None` if the stripped input is an empty
       string."""
```

### Comparing `minitrino-2.0.3/minitrino.egg-info/PKG-INFO` & `minitrino-2.0.4/minitrino.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,447 +1,232 @@
 Metadata-Version: 2.1
 Name: minitrino
-Version: 2.0.3
+Version: 2.0.4
 Summary: A command line tool that makes it easy to run modular Trino environments locally.
 Home-page: https://github.com/jefflester/minitrino
 Author: Jeff Lester
 Author-email: jeff.lester.dev@gmail.com
 License: Apache-2.0
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Minitrino
 
 A command line tool that makes it easy to run modular Trino environments
-locally. Compatible with Starburst versions 370-e and later.
+locally. Compatible with Starburst versions 388-e and later.
 
 [![PyPI
 version](https://badge.fury.io/py/minitrino.svg)](https://badge.fury.io/py/minitrino)
-[![Build
-Status](https://app.travis-ci.com/jefflester/minitrino.svg?branch=master)](https://app.travis-ci.com/jefflester/minitrino)
+![Build
+Status](https://github.com/jefflester/minitrino/actions/workflows/tests.yml/badge.svg)
 [![Trino
 Slack](https://img.shields.io/static/v1?logo=slack&logoColor=959DA5&label=Slack&labelColor=333a41&message=join%20conversation&color=3AC358)](https://trinodb.io/slack.html)
 
 -----
 
-**Latest Stable Release**: 2.0.3
+**Latest Stable Release**: 2.0.4
 
 -----
 
 ## Overview
 
 - [Minitrino](#minitrino)
   - [Overview](#overview)
   - [Requirements](#requirements)
-  - [Installation](#installation)
+  - [Installation and Upgrades](#installation-and-upgrades)
     - [End Users](#end-users)
     - [Developers](#developers)
-  - [CLI](#cli)
-    - [Top-Level CLI Options](#top-level-cli-options)
-    - [Provisioning Environments](#provisioning-environments)
-      - [Environment Variables](#environment-variables)
-      - [Using Licensed Starburst Features](#using-licensed-starburst-features)
-    - [Removing Resources](#removing-resources)
-    - [Shutting Down Environments](#shutting-down-environments)
-    - [Taking Environment Snapshots](#taking-environment-snapshots)
-    - [Manage User Configuration](#manage-user-configuration)
-    - [Install the Library](#install-the-library)
-    - [Display Module Metadata](#display-module-metadata)
-    - [Display Minitrino Versions](#display-minitrino-versions)
-    - [Pointing the CLI to the Minitrino Library](#pointing-the-cli-to-the-minitrino-library)
+    - [Using Colima and Other Docker Contexts](#using-colima-and-other-docker-contexts)
+    - [End User Upgrades](#end-user-upgrades)
+  - [Workflow Examples](#workflow-examples)
+    - [Provision an Environment](#provision-an-environment)
+    - [Modify Files in a Running Container](#modify-files-in-a-running-container)
+    - [Shut Down an Environment](#shut-down-an-environment)
+    - [Remove Minitrino Resources](#remove-minitrino-resources)
+    - [Snapshot a Customized Module](#snapshot-a-customized-module)
   - [Minitrino Configuration File](#minitrino-configuration-file)
     - [\[CLI\] Section](#cli-section)
     - [\[MODULES\] Section](#modules-section)
   - [Project Structure](#project-structure)
     - [Trino Dockerfile](#trino-dockerfile)
-  - [Adding New Modules (Tutorial)](#adding-new-modules-tutorial)
+  - [Add New Modules (Tutorial)](#add-new-modules-tutorial)
     - [Create the Module Directory](#create-the-module-directory)
     - [Add Trino Resources](#add-trino-resources)
     - [Add the Docker Compose YAML](#add-the-docker-compose-yaml)
     - [Add a Metadata File](#add-a-metadata-file)
     - [Add a Readme File](#add-a-readme-file)
     - [Review Progress](#review-progress)
     - [Configure the Docker Compose YAML File](#configure-the-docker-compose-yaml-file)
     - [Important Implementation Details: Paths and Labels](#important-implementation-details-paths-and-labels)
       - [Path References for Volumes and Build Contexts](#path-references-for-volumes-and-build-contexts)
       - [Minitrino Docker Labels](#minitrino-docker-labels)
     - [Test the New Catalog](#test-the-new-catalog)
-    - [Customizing Images](#customizing-images)
     - [Bootstrap Scripts](#bootstrap-scripts)
       - [Installing Shell Packages for Bootstrap Scripts](#installing-shell-packages-for-bootstrap-scripts)
     - [Managing Trino's `config.properties` and `jvm.config` Files](#managing-trinos-configproperties-and-jvmconfig-files)
+      - [Preferable Method: Environment Variables](#preferable-method-environment-variables)
+      - [Secondary Method: Bootstrap Scripts](#secondary-method-bootstrap-scripts)
   - [Troubleshooting](#troubleshooting)
   - [Reporting Bugs and Contributing](#reporting-bugs-and-contributing)
 
 -----
 
 ## Requirements
 
-- Docker 19.03.0+
-- Docker Compose (1.29.0+)
-- Python 3.8+
+- Docker Desktop >= 3.5
+- Python >= 3.8
 - Pip
-- Linux or Mac OS
+- Linux / MacOS
 
 -----
 
-## Installation
+## Installation and Upgrades
 
 ### End Users
 
 Minitrino is available on PyPI and the library is available for public download
-on GitHub. To install the Minitrino CLI, run `pip install minitrino`. To install
-the library, run `minitrino lib_install`.
+on GitHub. To set everything up, run:
 
-### Developers
-
-In the project's root, run `./install.sh` to install the Minitrino CLI. If you
-encounter errors during installation, try running `sudo -H ./install.sh -v`.
-
------
-
-## CLI
-
-Minitrino is built with [Click](https://click.palletsprojects.com/en/7.x/), a
-popular, open-source toolkit used to build Python-based CLIs.
-
-All Minitrino commands/options are documented below. Note that many command
-options can be specified with a shorthand alternative, which is the first letter
-of each option, i.e. `--module` can be `-m`.
-
-### Top-Level CLI Options
-
-You can get help, enable verbose output, and change the runtime library
-directory for any command.
-
-```
-Usage: minitrino [OPTIONS] COMMAND [ARGS]...
-
-Options:
-  -v, --verbose   Enable verbose output.
-  -e, --env TEXT  Add or override environment variables.
-                  
-                  Environment variables are sourced from the Minitrino
-                  library's root 'minitrino.env' file as well as the user 
-                  config file in '~/.minitrino/minitrino.cfg'. Variables 
-                  supplied by this option will override values from either 
-                  of those sources. The variables will also be passed to the
-                  environment of the shell executing commands during the
-                  'provision' command.
-
-  --help          Show this message and exit.
-```
-
-### Provisioning Environments
-
-You can provision an environment via the `provision` command.
-
-```
-Usage: minitrino provision [OPTIONS]
-
-  Provision an environment based on specified modules. All options are
-  optional and can be left empty.
-
-Options:
-  -m, --module TEXT         A specific module to provision.
-  -n, --no-rollback         Do not rollback provisioned resources in the event
-                            of an error.
-
-  -d, --docker-native TEXT  Appends native docker-compose commands to the
-                            generated docker-compose shell command. Run
-                            `docker-compose up --help` to see all available
-                            options.
-                            
-                            Example: minitrino provision --docker-native
-                            --build
-                            
-                            Example: minitrino provision --docker-native '--
-                            remove-orphans --force-recreate'
-
-  --help                    Show this message and exit.
-```
-
-Notes:
-
-- If no options are passed in, the CLI will provision a standalone Trino
-  container.
-- The command cannot currently be used to append additional modules to an active
-  environment. To modify an environment, first shut it down, then re-provision
-  with the needed modules.
-
-Sample `provision` commands:
-
-```bash
-minitrino provision \
-  --module hive \
-  --module elasticsearch \
-  --module ldap \
-  --docker-native '--build --force-recreate'
-
-minitrino provision -m hive -m elasticsearch -m ldap
-
-minitrino --env STARBURST_VER=411-e provision
-```
-
-The `provision` command constructs a Docker Compose command and executes it in
-the host shell. The commands look similar to:
-
-```bash
-ENV_VAR_1=SOMETHING ENV_VAR_2=SOMETHING ENV_VAR_3=${ENV_VAR_3} ... \
-docker-compose -f docker-compose.yml \
-  -f modules/catalog/elasticsearch/elasticsearch.yml \
-  -f modules/catalog/hive/hive.yml \
-  -f modules/security/ldap/ldap.yml \
-  up -d
-```
-
-Using the structure of the Minitrino library, it is able to merge multiple
-Docker Compose files together.
-
-#### Environment Variables
-
-Environment variables passed to Docker containers are sourced through two
-locations. The first is from the `minitrino.env` file in the library root. These
-variables define the versions of the provisioned Docker services. The second is
-from from variables set in the `[MODULES]` section of the `minitrino.cfg` file.
-These variables can contain sensitive information like access credentials, so
-their values are intentionally left out of library files.
-
-Any existing environment variable can be overridden with the top-level `--env`
-option, and any unset variable can be set with it.
-
-#### Using Licensed Starburst Features
-
-If you are using licensed features, you will need to provide a path to a valid
-Starburst license. This can be set via `minitrino config` or provided via the
-`--env` option at command runtime. The variable for this is
-`STARBURST_LIC_PATH`.
-
-Additionally, you need to uncomment the volume mount in the library's root
-`docker-compose.yml` file:
-
-```yaml
-  # Uncomment this to enable the volume mount. The variable should point to a
-  # valid SEP license. 
-  volumes:
-    - "${STARBURST_LIC_PATH}:/etc/starburst/starburstdata.license:ro"
-```
-
-### Removing Resources
-
-You can remove resources with the `remove` command.
-
-```
-Usage: minitrino remove [OPTIONS]
-
-  Remove Minitrino resources.
-
-Options:
-  -i, --images      Remove Minitrino images.
-  -v, --volumes     Remove Minitrino container volumes.
-  -l, --label TEXT  Target specific labels for removal (format: key-value
-                    pair(s)).
-
-  -f, --force       Force the removal of Minitrino resources. Normal Docker
-                    removal restrictions apply.
-
-  --help            Show this message and exit.
-```
-
-Notes:
-
-- Named volumes tied to any *existing* container cannot be forcibly removed,
-  neither by Minitrino nor by the Docker CLI/SDK.
-- Images tied to stopped containers can be forcibly removed, but any image tied
-  to a running container cannot be forcibly removed, neither by Minitrino nor by
-  the Docker CLI.
-- You can find a module's label key by looking at the module's
-  `docker-compose.yml` file in the Minitrino library.
-
-Sample `remove` command:
-
-```bash
-minitrino -v remove \
-  --volumes \
-  --label com.starburst.tests.module.postgres=catalog-postgres \
-  --force
+```sh
+  pip install minitrino
+  minitrino -v lib_install
 ```
 
-This will only remove volumes associated to the Postgres catalog module.
+Using this installation method, the `LIB_PATH` variable will point to
+`~/.minitrino/lib/`.
 
-### Shutting Down Environments
+### Developers
 
-You can shut down an active environment with the `down` command.
+In the project's root directory, run `./install.sh` to install the Minitrino
+CLI. If you encounter errors during installation, try running `sudo -H
+./install.sh -v`.
+
+Using this installation method, the `LIB_PATH` variable will point to
+`${MINITRINO_REPOSITORY_DIRECTORY}/lib/`.
+
+### Using Colima and Other Docker Contexts
+
+For users not operating on the default Docker Desktop context, you can set the
+`DOCKER_HOST` shell environment variable to point to the desired context's
+`.sock` file, e.g.:
 
+```sh
+echo 'export DOCKER_HOST="unix://${HOME}/.colima/default/docker.sock"' >> ~/.bash_profile
 ```
-Usage: minitrino down [OPTIONS]
 
-  Bring down running Minitrino containers. This command follows the
-  behavior of `docker-compose down` where containers are both stopped and
-  removed.
-
-Options:
-  -k, --keep  Does not remove containers; instead, containers will only be
-              stopped.
-
-  --sig-kill  Stop Minitrino containers without a grace period.
-  --help      Show this message and exit.
-```
+### End User Upgrades
 
-Sample `down` command:
+To upgrade the Minitrino CLI, run:
 
-```bash
-minitrino -v down
+```sh
+pip install minitrino --upgrade
 ```
 
-### Taking Environment Snapshots
-
-You can capture snapshots for both active and inactive environments with the
-`snapshot` command.
+Each CLI version has its own respective library. To install the updated library,
+run:
 
+```sh
+minitrino -v lib_install
 ```
-Usage: minitrino snapshot [OPTIONS]
 
-  Create a snapshot of a Minitrino environment. A tarball is placed in the
-  Minitrino `lib/snapshots/` directory.
+**Note**: Installing the new library will overwrite all modules and snapshots in
+the current library. If you have customized modules or snapshot files in
+`lib/snapshots/`, make sure to take a backup of the `~/.minitrino/lib` directory
+prior to running this command in order to persist your local changes.
 
-  To take a snapshot of an active environment, leave the `--module` and
-  option out of the command.
+-----
 
-  To take a snapshot of modules whether they are active or not, specify the
-  modules via the `--module` option.
+## Workflow Examples
 
-Options:
-  -m, --module TEXT     A specific module to snapshot.
-  -n, --name TEXT       Basename of the resulting snapshot tarball file.
-                        Allowed characters: alphanumerics, hyphens, and
-                        underscores.  [required]
+Minitrino is best suited for local Trino development. This project is not
+intended for usage on a large scale, and is intentionally designed to limit the
+deployment to a single coordinator container.
 
-  -d, --directory PATH  Directory to save the resulting snapshot file in.
-                        Defaults to the snapshots directory in the Minitrino
-                        library.
+### Provision an Environment
 
-  -f, --force           Overwrite the file if it already exists.
-  --no-scrub            Do not scrub sensitive data from user config file.
-                        
-                        WARNING: all sensitive information (passwords and
-                        keys) will be kept in the user config file added to
-                        the snapshot. Only use this if you are prepared to
-                        share those secrets with another person.
+Provision the `postgres` module with a specific SEP version:
 
-  --help                Show this message and exit.
+```sh
+minitrino -v -e STARBURST_VER=${VER} provision -m postgres
 ```
 
-Notes:
-
-- Minitrino records the original `provision` command and places it in the
-  snapshot file as `provision-snapshot.sh`; this can be directly executed. This
-  makes it easier for others to reuse the environment and provision it
-  identically.
-
-Sample `snapshot` commands:
+Provision the `iceberg` and `oauth2` modules:
 
-```bash
-# Take a snapshot of an active environment (this will create a tarball 
-# called `snapshot-t2533.tar.gz` in the library's `snapshots/` directory):
-minitrino snapshot --name t-2533
-
-# Take a snapshot of specific modules:
-minitrino snapshot -n super-cool-env -m hive -m elasticsearch -m ldap
+```sh
+minitrino -v provision -m postgres -m oauth2
 ```
 
-### Manage User Configuration
-
-You can manage Minitrino configuration with the `config` command.
+Append the running environment with a third module:
 
+```sh
+minitrino -v provision -m postgres -m oauth2 -m hive
 ```
-Usage: minitrino config [OPTIONS]
-
-  Edit the Minitrino user configuration file.
 
-Options:
-  -r, --reset  Reset the Minitrino user configuration file and create a new
-               config file from a template.
-               
-               WARNING: This will remove your configuration file (if it
-               exists) and replace it with a template.
+All environments expose the Starburst service on `localhost:8080`, meaning you
+can visit the web UI directly, or you can connect external clients, such as
+DBeaver, to the `localhost` service. The `trino` container shell can be directly
+accessed via:
 
-  --help       Show this message and exit.
+```sh
+docker exec -it trino bash 
 ```
 
-### Install the Library
+### Modify Files in a Running Container
 
-You can install the Minitrino library with the `lib_install` command. Note that
-it is best practice to have the library version match the CLI version. You can
-check these versions with `minitrino version`.
+You can modify files inside a running container with this workflow:
 
+```sh
+docker exec -it trino bash 
+echo "io.trino=DEBUG" >> /etc/starburst/log.properties
+exit
+docker restart trino
 ```
-Usage: minitrino lib_install [OPTIONS]
 
-  Install the Minitrino library.
+### Shut Down an Environment
 
-Options:
-  -v, --version TEXT  The version of the library to install.
-  --help              Show this message and exit.
+```sh
+minitrino down
 ```
 
-### Display Module Metadata
+### Remove Minitrino Resources
 
-You can see Minitrino module metadata with the `modules` command.
+To remove all images, run:
 
+```sh
+minitrino remove --images
 ```
-Usage: minitrino modules [OPTIONS]
-
-  Display module metadata.
 
-Options:
-  -m, --module TEXT  A specific module to display metadata for.
-  -j, --json         Print the resulting metadata in JSON form (shows
-                     additional module metadata).
+To remove images from a specific module, run:
 
-  -r, --running      Print metadata for all running modules.
-  --help             Show this message and exit.
+```sh
+minitrino remove --images \
+  --label com.starburst.tests.module.${MODULE}=${MODULE_TYPE}-${MODULE}
 ```
 
-### Display Minitrino Versions
+Where `${MODULE_TYPE}` is one of: `admin`, `catalog`, `security`.
 
-You can display the Minitrino CLI and library versions with the `version`
-command.
+You can also use the `remove` command to remove individual volumes with the
+`--volumes` option.
 
-```
-Usage: minitrino version [OPTIONS]
+### Snapshot a Customized Module
 
-  Display Minitrino CLI and library versions.
+Users designing and customizing their own modules can persist them with the
+`snapshot` command. For example, if a user has modified the `hive` module, they
+can persist their changes by running:
 
-Options:
-  --help  Show this message and exit.
+```sh
+minitrino snapshot --name ${SNAPSHOT_NAME} -m hive
 ```
 
-### Pointing the CLI to the Minitrino Library
-
-The Minitrino CLI should always point to a compatible library with the expected
-structure. The library directory can be set one of four ways, listed below in
-the order of precedence:
-
-1. Passing the `LIB_PATH` variable to the CLI's `--env` option sets the library
-   directory for the current command.
-2. The `minitrino.cfg` file's `LIB_PATH` variable sets the library directory if
-   present.
-3. The path `~/.minitrino/lib/` is used as the default lib path if the
-   `LIB_PATH` var is not found.
-4. As a last resort, Minitrino will check to see if the library exists in
-   relation to the positioning of the `components.py` file and assumes the
-   project is being run out of a cloned repository.
-
-If you not running out of a cloned repository, it is advisable to provide a
-pointer to the library in Minitrino's configuration via the `LIB_PATH` config.
+By default, the snapshot file is placed in
+`${LIB_PATH}/${SNAPSHOT_NAME}.tar.gz`. The snapshot can be saved to a different
+directory by passing the `--directory` option to the `snapshot` command.
 
 -----
 
 ## Minitrino Configuration File
 
 Sticky configuration is set in `~/.minitrino/minitrino.cfg`. The sections in
 this file each serve a separate purpose.
@@ -453,17 +238,17 @@
 - `LIB_PATH`: The filesystem path of the Minitrino library (specifically to the
   `lib/` directory).
 - `TEXT_EDITOR`: The text editor to use with the `config` command, e.g. "vi",
   "nano", etc. Defaults to the shell's default editor.
 
 ### [MODULES] Section
 
-This section has only one default config: `STARBURST_LIC_PATH`. This is required
-if using licensed Starburst Enterprise features. It can point to any valid
-license on your filesystem.
+This section has only one default config: `SEP_LIC_PATH`. This is required if
+using licensed Starburst Enterprise features. It can point to any valid license
+on your filesystem.
 
 This section can also be used to set environment variables passed to containers
 provisioned by Minitrino. Environment variables are only passed to a container
 if the variable is specified in the module's `docker-compose.yml` file.
 
 For example, if your `minitrino.cfg` config file contains this variable:
 
@@ -473,38 +258,36 @@
 
 And your `docker-compose.yml` file contains this:
 
 ```yaml
 services:
   trino:
     environment:
-      DB_PASSWORD: "${DB_PASSWORD}"
+      DB_PASSWORD: ${DB_PASSWORD}
 ```
 
-Then `DB_PASSWORD` is accessible inside of the resulting Trino container in the
-form of a shell environment variable. This functionality can be applied to any
-container as long as the above is followed.
+Then `DB_PASSWORD` is accessible inside of the Trino container as an environment
+variable. This functionality can be applied to any container as long as the
+convention above is followed.
 
 -----
 
 ## Project Structure
 
 The library is built around Docker Compose files and utilizes Docker's ability
 to [extend Compose
 files](https://docs.docker.com/compose/extends/#multiple-compose-files).
 
 The Starburst Trino service is defined in a Compose file at the library root,
 and all other services look up in the directory tree to reference the parent
-Trino service. In Compose files, the fully-qualified path––relative to the
-library's root `docker-compose.yml` file––must be provided for Docker to locate
-resources.
+Trino service.
 
 A simplified library structure:
 
-```
+```sh
 lib
 ├── Dockerfile
 ├── docker-compose.yml
 ├── minitrino.env
 ├── modules
 │   ├── admin
 │   │   └── ...
@@ -521,65 +304,37 @@
 │   ├── resources
 │   └── security
 │       └── ...
 ├── snapshots
 └── version
 ```
 
-And the contents of a `docker-compose.yml` file (`postgres.yml`):
-
-```yaml
-version: "3.8"
-services:
-
-  trino:
-    volumes:
-      - "./modules/catalog/postgres/resources/trino/postgres.properties:/etc/starburst/catalog/postgres.properties"
-
-  postgres:
-    image: "postgres:${POSTGRES_VER}"
-    container_name: "postgres"
-    labels:
-      - "com.starburst.tests=minitrino"
-      - "com.starburst.tests.module.postgres=catalog-postgres"
-    env_file:
-      - "./modules/catalog/postgres/resources/postgres/postgres.env"
-```
-
-Notice that the volume mount is not relative to the
-`lib/modules/catalog/postgres/` directory––it is relative to the parent
-directory which houses the top-level `docker-compose.yml` file. Also, notice the
-labels––these labels will be used to identify Docker resources tied to Minitrino
-modules so that the CLI commands actually work.
-
 ### Trino Dockerfile
 
-Minitrino modifies the Starburst Trino Docker image by adding the Trino CLI to
-the image as well as by providing `sudo` to the `trino` user. This is required
-for certain bootstrap scripts (i.e. using `yum` to install packages in a Trino
-container for a module). This image is compatible with Starburst Trino images
-back to Starburst Trino version `332-e.0`.
+Minitrino modifies Starburst's Docker image by adding the Trino CLI to the image
+as well as by adding `sudo` privileges to the `trino` user. This is required for
+certain bootstrap scripts (i.e. using `microdnf` to install packages in a Trino
+container for a module).
 
 -----
 
-## Adding New Modules (Tutorial)
+## Add New Modules (Tutorial)
 
 Adding new modules is relatively simple, but there are a few important
-guidelines to follow to ensure compatibility with the Minitrino CLI. The design
-rules are the same for both catalogs and security modules. The example below
-demonstrates the process of creating a new catalog module for a Postgres
-service.
+guidelines to follow to ensure compatibility with the Minitrino CLI. Module
+design principals are the same all modules. The example below demonstrates the
+process of creating a new catalog module for a Postgres service.
 
 ### Create the Module Directory
 
 Create the module's directory in the `lib/modules/catalog/` directory:
 
 ```sh
-mkdir lib/modules/catalog/postgres/
-cd lib/modules/catalog/postgres/
+mkdir lib/modules/catalog/my-postgres/
+cd lib/modules/catalog/my-postgres/
 ```
 
 ### Add Trino Resources
 
 All resources for a module go inside of a `resources/` directory within the
 module. Inside this directory, place Trino-specific resources into a `trino/`
 directory, then mount the resources to the Trino service defined in the root
@@ -598,30 +353,32 @@
 connection-user=admin
 connection-password=trinoRocks15
 EOF"
 ```
 
 -----
 
-**Note**: Passwords should always be `trinoRocks15` for consistency throughout
-modules.
+**Note**: Passwords in the default modules tend to be `trinoRocks15`. For
+consistency throughout the library, it is recommended to use this as the
+password of choice for new module development.
 
 -----
 
 ### Add the Docker Compose YAML
 
-In `lib/modules/catalog/postgres/`, add a Docker Compose file:
+In `lib/modules/catalog/my-postgres/`, add a Docker Compose file:
 
 ```sh
-touch postgres.yml
+touch my-postgres.yml
 ```
 
-Notice the naming convention: `postgres.yml`. Giving the same root name of
-"postgres" to both the parent directory `postgres/` and to the Docker Compose
-file `postgres.yml` will allow Minitrino to find our new catalog module.
+Notice the naming convention: `my-postgres.yml`. Giving the same root name of
+"my-postgres" to both the parent directory `my-postgres/` and to the Docker
+Compose file `my-postgres.yml` will allow Minitrino to find the new catalog
+module.
 
 Next, add an environment file for the Postgres service. Non-Trino resources
 should go into their own directory, so create one for postgres:
 
 ```sh
 mkdir resources/postgres/
 ```
@@ -638,88 +395,92 @@
 ```
 
 This file will initialize Postgres with a database `minitrino`, a user `trino`,
 and a password `trinoRocks15`.
 
 ### Add a Metadata File
 
-The `metadata.json` file allows Minitrino to obtain key information for the
-module. It is required for a module to work with the CLI.
+The `metadata.json` file allows Minitrino to obtain key information about the
+module. **It is required for a module to work with the CLI.**
 
-In `lib/modules/catalog/postgres/`, add the `metadata.json` file:
+In `lib/modules/catalog/my-postgres/`, add a `metadata.json` file:
 
 ```sh
 bash -c 'cat << EOF > metadata.json
 {
   "description": "Creates a Postgres catalog using the standard Postgres connector.",
   "incompatibleModules": [],
-  "dependentModules": []
+  "dependentModules": [],
+  "enterprise": false
 }
 EOF'
 ```
 
-The metadata file is presentable to the user via the `modules` command. The
-`incompatibleModules` key restricts certain modules from being provisioned
+- `description`: describes the module.
+- `incompatibleModules`: restricts certain modules from being provisioned
 alongside the given module. The `*` wildcard is a supported convention if the
-module is incompatible with all other modules. Lastly, the `dependentModules`
-key can be used to require other pre-defined modules to provision alongside the
-module containing the `metadata.json` file.
+module is incompatible with all other modules.
+- `dependentModules`: specifies which modules must be provisioned alongside the
+target. Dependent modules will be automatically provisioned with the `provision`
+command.
+- `enterprise`: requires a Starburst license file (`starburstdata.license`).
+
+The metadata file information can be exposed via the `modules` command.
 
 ### Add a Readme File
 
 This step is not required for personal development, but it is required to commit
 a module to the Minitrino repository.
 
-In `lib/modules/catalog/postgres/`, add the `readme.md` file:
+In `lib/modules/catalog/my-postgres/`, add a `readme.md` file:
 
 ```sh
 touch readme.md
 ```
 
 This file should contain an overview of the module.
 
 ### Review Progress
 
-The resulting directory tree should look like this (from the `/modules/catalog/`
-directory):
+The resulting directory tree should look like this (from the
+`lib/modules/catalog/` directory):
 
-```
-postgres
+```sh
+my-postgres
 ├── metadata.json
-├── postgres.yml
+├── my-postgres.yml
 ├── readme.md
 └── resources
     ├── postgres
     │   └── postgres.env
     └── trino
         └── postgres.properties
 ```
 
 ### Configure the Docker Compose YAML File
 
-We will now define the `postgres.yml` Docker Compose file. Set it up as follows,
-and **read the important notes after**:
+We will now define the `my-postgres.yml` Docker Compose file. Set it up as
+follows:
 
 ```yaml
-version: "3.8"
+version: '3.8'
 services:
 
   trino:
     volumes:
-    # Always place Trino files in `/etc/starburst/` as symbolic links can change between versions
-      - "./modules/catalog/postgres/resources/trino/postgres.properties:/etc/starburst/catalog/postgres.properties"
+      - ./modules/catalog/my-postgres/resources/trino/postgres.properties:/etc/starburst/catalog/postgres.properties
 
   postgres:
-    image: "postgres:${POSTGRES_VER}"
-    container_name: "postgres"
-    labels:
-      - "com.starburst.tests=minitrino"
-      - "com.starburst.tests.module.postgres=catalog-postgres"
+    image: postgres:${POSTGRES_VER}
+    container_name: postgres
     env_file:
-      - "./modules/catalog/postgres/resources/postgres/postgres.env"
+      - ./modules/catalog/my-postgres/resources/postgres/postgres.env
+    labels:
+      - com.starburst.tests=minitrino
+      - com.starburst.tests.module.my-postgres=catalog-my-postgres
 
 ```
 
 ### Important Implementation Details: Paths and Labels
 
 We can observe a few things about the Compose file we just defined.
 
@@ -736,104 +497,98 @@
 is how Minitrino constructs these commands.
 
 If this is confusing, you can read more about extending Compose files on the
 [Docker docs](https://docs.docker.com/compose/extends/#multiple-compose-files).
 
 #### Minitrino Docker Labels
 
-Secondly, notice how we applied sets of labels to the Postgres service. These
+Secondly, notice the applied sets of labels to the Postgres service. These
 labels tell the CLI which resources to target when executing commands.
 
 In general, there is no need to apply labels to the Trino service since they are
 already applied in the parent Compose file **unless** the module is an extension
-of the Trino service itself (i.e. the Snowflake modules). Labels should always
-be applied to:
+of the Trino service itself (i.e. the `biac` module). Labels should always be
+applied to:
 
 - Docker services (AKA the resulting container)
-- Named volumes
-- Images built from a Dockerfile
+- Persistent volumes
+- Images built from a Dockerfile (see the main `docker-compose.yml` file for an
+  example)
 
 Labels should be defined in pairs of two. The convention is:
 
 - The standard Minitrino resource label: `com.starburst.tests=minitrino`
 - A module-specific resource label:
-  `com.starburst.tests.module.<module-name>=<module-type>-<module-name>`
-  - For this label, the `module-type` should be either `catalog` or `security`
-  - This applies a unique label to the module, allowing it to be an isolated
-    component when necessary.
+  `com.starburst.tests.module.${MODULE_NAME}=${MODULE_CATEGORY}-${MODULE_NAME}`
+  - For this label, the `module-type` should be one of: `admin`, `catalog`, or
+    `security`
+  - This applies a unique label to the module, allowing it to be isolated when
+    necessary
 
 In Compose files where multiple services are defined, all services should be
-labeled with the same label sets (see `hive.yml` for an example).
+labeled with the same label sets (see the `hive` for an example).
 
 -----
 
 **Note**: A named volume is defined explicitly in the Compose file, and these
 should always have label sets applied to them. Below is an example of the
 Compose file we just created with a named volume.
 
 -----
 
 ```yaml
-version: "3.8"
+version: '3.8'
 services:
 
   trino:
     volumes:
-      - "./modules/catalog/postgres/resources/trino/postgres.properties:/etc/starburst/catalog/postgres.properties"
+      - ./modules/catalog/my-postgres/resources/trino/postgres.properties:/etc/starburst/catalog/postgres.properties
 
   postgres:
-    image: "postgres:${POSTGRES_VER}"
-    container_name: "postgres"
-    labels: # These labels are applied to the service/container
-      - "com.starburst.tests=minitrino"
-      - "com.starburst.tests.module.postgres=catalog-postgres"
+    image: postgres:${POSTGRES_VER}
+    container_name: postgres
     env_file:
-      - "./modules/catalog/postgres/resources/postgres/postgres.env"
+      - ./modules/catalog/my-postgres/resources/postgres/postgres.env
+    labels: # These labels are applied to the service/container
+      - com.starburst.tests=minitrino
+      - com.starburst.tests.module.my-postgres=catalog-my-postgres
 
 volumes:
   postgres-data:
     labels: # These labels are applied to the named volume
-      - "com.starburst.tests=minitrino"
-      - "com.starburst.tests.module.postgres=catalog-postgres"
+      - com.starburst.tests=minitrino
+      - com.starburst.tests.module.my-postgres=catalog-my-postgres
 ```
 
 -----
 
 **Note**: Certain modules will only extend the parent Trino service and do not
-actually define any new services/containers. See the Snowflake catalog modules
-for an example of this. For these modules, the only label requirement is to add
-the module-specific label to the Trino service in the relevant
-`docker-compose.yml` file
+actually define any new services/containers. See the `biac` module for an
+example of this. For these modules, the only label requirement is to add the
+module-specific label to the Trino service in the relevant `docker-compose.yml`
+file.
 
 -----
 
 ### Test the New Catalog
 
 We are all finished up. We can test our new catalog through the Minitrino CLI:
 
 ```sh
-minitrino provision -m postgres
+minitrino provision -m my-postgres
 ```
 
-We can now shell into the `trino` container and run some tests:
+We can now open a shell session in the `trino` container and run some tests:
 
-```
+```sh
 docker exec -it trino bash 
 trino-cli
 trino> show catalogs;
 ```
 
-### Customizing Images
-
-If you need to build an image from a local Dockerfile, you can do so and
-structure the Compose file accordingly. See the library's root
-`docker-compose.yml` file for an example of this. Path references for volumes
-and the image build context will follow the same convention as volume mount
-paths described earlier.
-
 ### Bootstrap Scripts
 
 Minitrino supports container bootstrap scripts. These scripts **do not replace**
 the entrypoint (or default command) for a given container. The script is copied
 from the Minitrino library to the container, executed, and then removed from the
 container. Containers are restarted after each bootstrap script execution, **so
 the bootstrap scripts themselves should not restart the container's service**.
@@ -849,20 +604,20 @@
 container(s) via `minitrino down` and then to re-provision.
 
 To add a bootstrap script, add a `resources/bootstrap/` directory in any given
 module, create a shell script, and then reference the script name in the Compose
 YAML file:
 
 ```yaml
-version: "3.8"
+version: '3.8'
 services:
 
   trino:
     environment:
-      MINITRINO_BOOTSTRAP: "bootstrap.sh"
+      MINITRINO_BOOTSTRAP: bootstrap.sh
 ```
 
 The `elasticsearch` module is a good example of this.
 
 #### Installing Shell Packages for Bootstrap Scripts
 
 If you need to install a shell package for a bootstrap script, it is recommended
@@ -871,60 +626,65 @@
 releases.
 
 To add the necessary package, simply update shell dependencies in
 `lib/dockerfile-resources/configure.sh`.
 
 ### Managing Trino's `config.properties` and `jvm.config` Files
 
-Many modules can change the Trino `config.properties` and `jvm.config` files.
-Because of this, there are two supported ways to modify these files with
-Minitrino.
-
-The first way is by setting the relevant environment variables in your
-`module.yml` Docker Compose file. This will propagate the configs to the Trino
-container when it is provisioned. For example:
+Many modules may change the Trino `config.properties` and `jvm.config` files.
+There are two supported ways to modify these files with within the `trino`
+container.
+
+#### Preferable Method: Environment Variables
+
+Minitrino has special support for two Trino-specific environment variables:
+`CONFIG_PROPERTIES` and `JVM_CONFIG`. Below is an example of setting these
+variables:
 
 ```yaml
 trino:
   environment:
     CONFIG_PROPERTIES: |-
       insights.jdbc.url=jdbc:postgresql://postgresdb:5432/insights
       insights.jdbc.user=admin
       insights.jdbc.password=password
       insights.persistence-enabled=true
     JVM_CONFIG: |-
       -Xlog:gc:/var/log/sep-gc-%t.log:time:filecount=10
 ```
 
-The second way to modify these configuration files is via module [bootstrap
-scripts](#bootstrap-scripts).
+#### Secondary Method: Bootstrap Scripts
+
+The `config.properties` and `jvm.config` files can also be modified directly
+with a Trino [bootstrap script](#bootstrap-scripts).
 
 -----
 
 ## Troubleshooting
 
 - If you experience issues executing a Minitrino command, re-run it with the
-  `-v` option for verbose output. This will often reveal the issue
+  `-v` option for verbose output. This will often reveal the issue's root cause.
 - If you experience an issue with a particular Docker container, consider
   running these commands:
-  - `docker logs <container>`: Print the logs for a given container to the
+  - `docker logs ${CONTAINER_NAME}`: Print the logs for a given container to the
     terminal
   - `docker ps`: Show all running Docker containers and associated statistics
-  - `docker inspect <container>` to see various details about a container
+  - `docker inspect ${CONTAINER_NAME}` to see various details about a container
 - If you experience issues with a library module, check that that module is
   structured correctly according to the [module
-  tutorial](#adding-new-modules-tutorial), and ensure the library and the CLI
+  tutorial](#add-new-modules-tutorial), and ensure the library and the CLI
   versions match
-- Sometimes, a lingering persistent volume can cause problem (i.e. a stale Hive
-  metastore database volume from a previous module), so you can run:
+- Sometimes, a lingering persistent volume can cause problems (i.e. a stale Hive
+  metastore database volume from a previous module deployment), so you can run:
   - `minitrino down`
   - `minitrino -v remove --volumes` to remove **all** existing Minitrino
     volumes. Alternatively, run `minitrino -v remove --volumes --label <your
     label>` to specify a specific module for which to remove volumes. See the
-    [removing resources](#removing-resources) section for more information.
+    [removing resources](#remove-minitrino-resources) section for more
+    information.
 
 If none of these troubleshooting tips help to resolve your issue, [please file a
 GitHub issue](#reporting-bugs-and-contributing) and provide as much information
 as possible.
 
 -----
 
@@ -943,9 +703,7 @@
 1. Fork the repository, then make a PR to merge your changes
 2. If you have been added as a contributor, you can go with the method above or
    you can create a feature branch, then submit a PR for that feature branch
    when it is ready to be merged.
 
 In either case, please provide a comprehensive description of your changes with
 the PR.
-
-
```

### Comparing `minitrino-2.0.3/minitrino.egg-info/SOURCES.txt` & `minitrino-2.0.4/minitrino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `minitrino-2.0.3/setup.py` & `minitrino-2.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 HERE = Path(os.path.abspath(__file__)).resolve().parents[1]
 README = (HERE / "readme.md").read_text()
 
 setup(
     name="minitrino",
-    version="2.0.3",
+    version="2.0.4",
     description="A command line tool that makes it easy to run modular Trino environments locally.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/jefflester/minitrino",
     author="Jeff Lester",
     author_email="jeff.lester.dev@gmail.com",
     license="Apache-2.0",
@@ -24,14 +24,14 @@
         "Operating System :: OS Independent",
     ],
     keyword="trino, docker, minitrino",
     python_requires=">=3.8",
     packages=["minitrino", "minitrino.cmd"],
     include_package_data=True,
     install_requires=[
-        "click==8.1.3",
+        "click==8.1.4",
         "colorama",
-        "docker==5.0.0",
+        "docker==6.1.2",
         "PyYAML",
     ],
     entry_points={"console_scripts": ["minitrino=minitrino.cli:cli"]},
 )
```

