# Comparing `tmp/dan-build-0.2.6.tar.gz` & `tmp/dan-build-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dan-build-0.2.6.tar", last modified: Fri Jul  7 07:20:39 2023, max compression
+gzip compressed data, was "dan-build-0.2.7.tar", last modified: Sat Jul  8 08:52:25 2023, max compression
```

## Comparing `dan-build-0.2.6.tar` & `dan-build-0.2.7.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.300667 dan-build-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-07 07:20:29.000000 dan-build-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-07 07:20:39.300667 dan-build-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-07-07 07:20:29.000000 dan-build-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.284666 dan-build-0.2.6/completion/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.284666 dan-build-0.2.6/completion/bash/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-07 07:20:29.000000 dan-build-0.2.6/completion/bash/dan-io.sh
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-07 07:20:29.000000 dan-build-0.2.6/completion/bash/dan.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.284666 dan-build-0.2.6/completion/zsh/
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-07 07:20:29.000000 dan-build-0.2.6/completion/zsh/dan-io.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-07 07:20:29.000000 dan-build-0.2.6/completion/zsh/dan.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.288666 dan-build-0.2.6/dan/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.288666 dan-build-0.2.6/dan/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cli/click.py
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cli/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    13800 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cli/vscode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.288666 dan-build-0.2.6/dan/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cmake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cmake/configure_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cmake/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.288666 dan-build-0.2.6/dan/conan/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/conan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/conan/requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.292667 dan-build-0.2.6/dan/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/aiofiles.py
--rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/detect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/find.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/include.py
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/makefile.py
--rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/osinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/pathlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/pm.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    19673 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/core/win.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.296667 dan-build-0.2.6/dan/cxx/
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cxx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cxx/compile_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.296667 dan-build-0.2.6/dan/cxx/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cxx/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cxx/data/detect.cmd
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cxx/data/empty.c
--rw-r--r--   0 runner    (1001) docker     (123)    24754 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cxx/detect.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cxx/msvc_toolchain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.296667 dan-build-0.2.6/dan/cxx/support/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cxx/support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cxx/support/qt.py
--rw-r--r--   0 runner    (1001) docker     (123)    19357 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cxx/targets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cxx/toolchain.py
--rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/cxx/unix_toolchain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.296667 dan-build-0.2.6/dan/io/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10987 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/io/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/io/repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    18574 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/make.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.296667 dan-build-0.2.6/dan/pkgconfig/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/pkgconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/pkgconfig/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.296667 dan-build-0.2.6/dan/pkgconfig/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/pkgconfig/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/pkgconfig/templates/pkg.pc.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.296667 dan-build-0.2.6/dan/src/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/src/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/src/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/src/tar.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-07 07:20:29.000000 dan-build-0.2.6/dan/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.300667 dan-build-0.2.6/dan_build.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-07 07:20:39.000000 dan-build-0.2.6/dan_build.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-07 07:20:39.000000 dan-build-0.2.6/dan_build.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 07:20:39.000000 dan-build-0.2.6/dan_build.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-07 07:20:39.000000 dan-build-0.2.6/dan_build.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-07 07:20:39.000000 dan-build-0.2.6/dan_build.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-07 07:20:39.000000 dan-build-0.2.6/dan_build.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-07 07:20:29.000000 dan-build-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 07:20:39.300667 dan-build-0.2.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:39.300667 dan-build-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-07 07:20:29.000000 dan-build-0.2.6/tests/test_cxx_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-07 07:20:29.000000 dan-build-0.2.6/tests/test_cxx_libraries.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-07-07 07:20:29.000000 dan-build-0.2.6/tests/test_cxx_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-07 07:20:29.000000 dan-build-0.2.6/tests/test_cxx_src_catch2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-07 07:20:29.000000 dan-build-0.2.6/tests/test_python_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:25.611678 dan-build-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-08 08:52:16.000000 dan-build-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-08 08:52:25.611678 dan-build-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-07-08 08:52:16.000000 dan-build-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:25.575678 dan-build-0.2.7/completion/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:25.583678 dan-build-0.2.7/completion/bash/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-08 08:52:16.000000 dan-build-0.2.7/completion/bash/dan-io.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-08 08:52:16.000000 dan-build-0.2.7/completion/bash/dan.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:25.583678 dan-build-0.2.7/completion/zsh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-08 08:52:16.000000 dan-build-0.2.7/completion/zsh/dan-io.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-08 08:52:16.000000 dan-build-0.2.7/completion/zsh/dan.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:25.583678 dan-build-0.2.7/dan/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:25.587678 dan-build-0.2.7/dan/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/cli/click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/cli/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13800 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/cli/vscode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:25.587678 dan-build-0.2.7/dan/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/cmake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/cmake/configure_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/cmake/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:25.587678 dan-build-0.2.7/dan/conan/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/conan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/conan/requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:25.599678 dan-build-0.2.7/dan/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/core/aiofiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/core/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/core/detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/core/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/core/find.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/core/functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/core/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/core/include.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/core/makefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/core/osinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/core/pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/core/pm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/core/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/core/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/core/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20079 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/core/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/core/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/core/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/core/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/core/win.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:25.599678 dan-build-0.2.7/dan/cxx/
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/cxx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/cxx/compile_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:25.603678 dan-build-0.2.7/dan/cxx/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/cxx/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/cxx/data/detect.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/cxx/data/empty.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24754 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/cxx/detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/cxx/msvc_toolchain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:25.603678 dan-build-0.2.7/dan/cxx/support/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/cxx/support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/cxx/support/qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19638 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/cxx/targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/cxx/toolchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/cxx/unix_toolchain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:25.603678 dan-build-0.2.7/dan/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10987 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/io/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/io/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18574 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/make.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:25.603678 dan-build-0.2.7/dan/pkgconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/pkgconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12805 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/pkgconfig/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:25.603678 dan-build-0.2.7/dan/pkgconfig/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/pkgconfig/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/pkgconfig/templates/pkg.pc.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:25.607678 dan-build-0.2.7/dan/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/src/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/src/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/src/tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-08 08:52:16.000000 dan-build-0.2.7/dan/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:25.607678 dan-build-0.2.7/dan_build.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-08 08:52:25.000000 dan-build-0.2.7/dan_build.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-08 08:52:25.000000 dan-build-0.2.7/dan_build.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 08:52:25.000000 dan-build-0.2.7/dan_build.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-08 08:52:25.000000 dan-build-0.2.7/dan_build.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-08 08:52:25.000000 dan-build-0.2.7/dan_build.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-08 08:52:25.000000 dan-build-0.2.7/dan_build.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-08 08:52:16.000000 dan-build-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 08:52:25.611678 dan-build-0.2.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:52:25.611678 dan-build-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-08 08:52:16.000000 dan-build-0.2.7/tests/test_cxx_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-08 08:52:16.000000 dan-build-0.2.7/tests/test_cxx_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-07-08 08:52:16.000000 dan-build-0.2.7/tests/test_cxx_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-08 08:52:16.000000 dan-build-0.2.7/tests/test_cxx_src_catch2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-08 08:52:16.000000 dan-build-0.2.7/tests/test_python_errors.py
```

### Comparing `dan-build-0.2.6/LICENSE` & `dan-build-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/PKG-INFO` & `dan-build-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dan-build
-Version: 0.2.6
+Version: 0.2.7
 Summary: Python-based build system.
 Author-email: Garcia Sylvain <garcia.6l20@gmail.com>, garcia.6l20@gmail.com
 License: MIT License
         
         Copyright (c) 2023 Sylvain Garcia
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dan-build-0.2.6/README.md` & `dan-build-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/completion/bash/dan-io.sh` & `dan-build-0.2.7/completion/bash/dan-io.sh`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/completion/bash/dan.sh` & `dan-build-0.2.7/completion/bash/dan.sh`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/completion/zsh/dan-io.sh` & `dan-build-0.2.7/completion/zsh/dan-io.sh`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/completion/zsh/dan.sh` & `dan-build-0.2.7/completion/zsh/dan.sh`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/cli/click.py` & `dan-build-0.2.7/dan/cli/click.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/cli/io.py` & `dan-build-0.2.7/dan/cli/io.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/cli/main.py` & `dan-build-0.2.7/dan/cli/main.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/cli/vscode.py` & `dan-build-0.2.7/dan/cli/vscode.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/cmake/configure_file.py` & `dan-build-0.2.7/dan/cmake/configure_file.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/cmake/project.py` & `dan-build-0.2.7/dan/cmake/project.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/conan/requirements.py` & `dan-build-0.2.7/dan/conan/requirements.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/core/aiofiles.py` & `dan-build-0.2.7/dan/core/aiofiles.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/core/asyncio.py` & `dan-build-0.2.7/dan/core/asyncio.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/core/cache.py` & `dan-build-0.2.7/dan/core/cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,18 @@
         self.__serializer = json if not binary else pickle
         if self.name in self.__caches:
             other = Cache.get(self.name)
             if other.path == self.path:
                 raise RuntimeError(f'Cache {self.name} already created, use Cache.instance')
             else:
                 raise RuntimeError(f'Cache {self.name} is not unique, use cache_name to distinguish {other.path} from {self.path}')
+
         assert not self.name in self.__caches, 'a cache should be unique'
+        self.__caches[self.name] = self
+
         if self.path.exists():
             with open(self.path, 'rb') as f:
                 if dataclasses.is_dataclass(self.dataclass):
                     self.__data = self.dataclass.from_json(f.read())
                 else:
                     self.__data = self.__serializer.load(f)
                 if not isinstance(self.__data, self.dataclass):
@@ -42,15 +45,14 @@
                 self.__modification_date = self.path.modification_time
         else:
             self.__data = self.dataclass(*args, **kwargs)
             self.__modification_date = 0.0
         
         self.__initial_state = self._dump()
         self.__dirty = False
-        self.__caches[self.name] = self
     
     @classmethod
     def instance(cls, path: Path|str, *args, cache_name:str = None, **kwargs):
         cache_name = cache_name or path.stem
         if cache_name in cls.__caches:
             return cls.__caches[cache_name]
         return cls(path, *args, cache_name=cache_name, **kwargs)
```

### Comparing `dan-build-0.2.6/dan/core/diagnostics.py` & `dan-build-0.2.7/dan/core/diagnostics.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/core/find.py` & `dan-build-0.2.7/dan/core/find.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/core/functools.py` & `dan-build-0.2.7/dan/core/functools.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/core/generator.py` & `dan-build-0.2.7/dan/core/generator.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/core/include.py` & `dan-build-0.2.7/dan/core/include.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/core/makefile.py` & `dan-build-0.2.7/dan/core/makefile.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     @property
     def fullname(self):
         return f'{self.parent.fullname}.{self.name}' if self.parent else self.name
 
     @property
     def cache(self) -> Cache:
         if not self.__cache:
-            self.__cache = Cache(
+            self.__cache = Cache.instance(
                 self.build_path / f'{self.name}.cache', cache_name=self.fullname, binary=True)
         return self.__cache
     
     @property
     def parents(self):
         parent = self.parent
         while parent is not None:
```

### Comparing `dan-build-0.2.6/dan/core/osinfo.py` & `dan-build-0.2.7/dan/core/osinfo.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/core/pathlib.py` & `dan-build-0.2.7/dan/core/pathlib.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/core/pm.py` & `dan-build-0.2.7/dan/core/pm.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/core/register.py` & `dan-build-0.2.7/dan/core/register.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/core/requirements.py` & `dan-build-0.2.7/dan/core/requirements.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,17 +49,28 @@
         if len(args) == 2:
             name = args[0]
             self.version_spec = args[1]
         else:
             name, self.version_spec = VersionSpec.parse(args[0])
         super().__init__(name)
         self.target : 'Target' = None
+        self.pn = name
         self.package, self.name, self.repository = parse_package(name)
         self.__skipped = list()
 
+    def __getstate__(self) -> object:
+        return {
+            'pn': self.pn,
+            'version_spec': self.version_spec,
+        }
+    
+    def __setstate__(self, data):
+        self.__init__(data['pn'], data['version_spec'])
+
+
     def is_compatible(self, t: 'Target'):
         if self.version_spec is not None:
             version_ok = self.version_spec.is_compatible(t.version)
         else:
             version_ok = True
         return version_ok
```

### Comparing `dan-build-0.2.6/dan/core/runners.py` & `dan-build-0.2.7/dan/core/runners.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/core/settings.py` & `dan-build-0.2.7/dan/core/settings.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/core/target.py` & `dan-build-0.2.7/dan/core/target.py`

 * *Files 2% similar despite different names*

```diff
@@ -344,14 +344,21 @@
         self.preload_dependencies = Dependencies(
             self, self.preload_dependencies)
 
         super().__init__(self.fullname)
 
         self._output: Path = None
         self._build_path = None
+        
+        if inspect.isclass(self.source_path) and issubclass(self.source_path, Target):
+            # delayed resolution
+            def _get_source_path(TargetClass, self):
+                return self.get_dependency(TargetClass).output
+            self.preload_dependencies.add(self.source_path)
+            type(self).source_path = property(functools.partial(_get_source_path, self.source_path))
 
         if type(self).output != Target.output:
             # hack class-defined output
             #   transform it to classproperty for build_path resolution
             output = self.output
             type(self).output = utils.classproperty(lambda: self.build_path / output)
```

### Comparing `dan-build-0.2.6/dan/core/test.py` & `dan-build-0.2.7/dan/core/test.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/core/utils.py` & `dan-build-0.2.7/dan/core/utils.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/core/version.py` & `dan-build-0.2.7/dan/core/version.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/core/win.py` & `dan-build-0.2.7/dan/core/win.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/cxx/__init__.py` & `dan-build-0.2.7/dan/cxx/__init__.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/cxx/compile_commands.py` & `dan-build-0.2.7/dan/cxx/compile_commands.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/cxx/detect.py` & `dan-build-0.2.7/dan/cxx/detect.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/cxx/msvc_toolchain.py` & `dan-build-0.2.7/dan/cxx/msvc_toolchain.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/cxx/support/qt.py` & `dan-build-0.2.7/dan/cxx/support/qt.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/cxx/targets.py` & `dan-build-0.2.7/dan/cxx/targets.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,16 +110,18 @@
                  private: list | set = set(),
                  transform_out: t.Callable[[t.Any], t.Any] = None,
                  transform_in: t.Callable[[t.Any], t.Any] = None) -> None:
         self._parent = parent
         self._name = name
         self._transform_out = transform_out or self.__nop_transform
         self._transform_in = transform_in or self.__nop_transform
-        self._public = list(public)
-        self._private = list(private)
+        self._public = list()
+        self._private = list()
+        self.add(*public, public=True)
+        self.add(*private, public=False)
 
     @staticmethod
     def __nop_transform(x):
         return x
 
     @property
     def private(self) -> list:
@@ -284,19 +286,23 @@
     def _init_sources(self):
         if callable(self.sources):
             self.sources = list(self.sources())
         if not isinstance(self.sources, Iterable):
             assert callable(
                 self.sources), f'{self.name} sources parameter should be an iterable or a callable returning an iterable'
         sources = list()
+        if self.source_path != self.makefile.source_path:
+            self.sources = [self.source_path / source for source in self.sources]
         source_root = Path(os.path.commonprefix(self.sources))
         for source in self.sources:
             source = Path(source)
             if source.is_absolute():
                 root = source_root
+                if root.is_file():
+                    root = root.parent
             else:
                 root = self.source_path
             sources.append(source)
             self.objs.append(
                 CXXObject(Path(source), self, root=root))
         self.sources = sources
```

### Comparing `dan-build-0.2.6/dan/cxx/toolchain.py` & `dan-build-0.2.7/dan/cxx/toolchain.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/cxx/unix_toolchain.py` & `dan-build-0.2.7/dan/cxx/unix_toolchain.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/io/package.py` & `dan-build-0.2.7/dan/io/package.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/io/repositories.py` & `dan-build-0.2.7/dan/io/repositories.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/jinja.py` & `dan-build-0.2.7/dan/jinja.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/logging.py` & `dan-build-0.2.7/dan/logging.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/make.py` & `dan-build-0.2.7/dan/make.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/pkgconfig/package.py` & `dan-build-0.2.7/dan/pkgconfig/package.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from copy import deepcopy
 import jinja2
 from dan.core import aiofiles, asyncio
 from dan.core.pathlib import Path
 import re
 import importlib.util
 
+from dan.core.cache import Cache
 from dan.core.find import find_file, find_files, library_paths_lookup
 from dan.core.pm import re_match
 from dan.core.requirements import RequiredPackage, parse_requirement
 from dan.core.runners import cmdline2list
 from dan.core.settings import InstallMode, InstallSettings
 from dan.core.utils import unique
 from dan.core.version import Version, VersionSpec
@@ -20,41 +21,63 @@
 
 class MissingPackage(RuntimeError):
     def __init__(self, name) -> None:
         super().__init__(f'package {name} not found')
 
 
 def find_pkg_config(name, paths=list()) -> Path:
-    return find_file(fr'.*{name}\.pc$', [*paths, '$PKG_CONFIG_PATH', *library_paths_lookup])
+    return find_file(fr'{re.escape(name)}\.pc$', [*paths, '$PKG_CONFIG_PATH', *library_paths_lookup])
 
 
 def find_pkg_configs(name, paths=list()) -> t.Generator[Path, None, None]:
-    yield from find_files(fr'.*{name}\.pc$', [*paths, '$PKG_CONFIG_PATH', *library_paths_lookup])
+    yield from find_files(fr'{re.escape(name)}\.pc$', [*paths, '$PKG_CONFIG_PATH', *library_paths_lookup])
 
 
 def has_package(name,  paths=list()):
     return find_pkg_config(name,  paths) is not None
 
-
+def parse_package_requires(reqs):
+    result = []
+    reqs = [r for r in re.split(r'[\s,]', reqs) if len(r.strip()) > 0]
+    tmp = []
+    it = iter(reqs)
+    ii = next(it, None)
+    while ii is not None:
+        if any(op in ii for op in ('=', '>', '<')):
+            tmp.append(ii)
+            ii = next(it)
+            tmp.append(ii)
+            result.append(parse_requirement(' '.join(tmp)))
+            tmp = []
+        else:
+            if len(tmp):
+                result.append(parse_requirement(' '.join(tmp)))
+                tmp = [ii]
+            else:
+                tmp.append(ii)
+        ii = next(it, None)
+    if len(tmp):
+        result.append(parse_requirement(' '.join(tmp)))
+    return result
 
 class Data:
     def __init__(self, path) -> None:
         self._path = Path(path)
         self._items = dict()
         with open(self._path) as f:
             lines = [l for l in [l.strip().removesuffix('\n')
                                  for l in f.readlines()] if len(l)]
             for line in lines:
                 m = Data.__split_expr.match(line)
                 if m:
                     k = m.group(1).lower()
                     v = m.group(2)
                     self._items[k] = v
-        self.__requires = None
-        self.__version = None
+        self._requires = None
+        self._version = None
 
     __split_expr = re.compile(r'(.+?)[:=](.+)')
 
     def get(self, name: str, default=None):
         if not name in self._items:
             return default
         value = self._items[name]
@@ -65,85 +88,120 @@
                     var = m.group(1)
                     value = value.replace(
                         f'${{{var}}}', self.get(var))
                 else:
                     break
         return value
     
+    def __getstate__(self):
+        return {
+            'path': self._path,
+            'items': self._items,
+            'requires': self._requires,
+            'version': self._version,
+        }
+    
+    def __setstate__(self, data):
+        self._path = data['path']
+        self._items = data['items']
+        self._requires = data['requires']
+        self._version = data['version']
+
     @property
     def path(self) -> Path:
         return self._path
     
     @property
     def requires(self) -> list[RequiredPackage]:
-        if self.__requires is None:
-            self.__requires = list()
+        if self._requires is None:
+            self._requires = list()
             reqs = self.get('requires')
             if reqs is not None:
-                reqs = reqs.strip()
-                # conan generates invalid requires clause
-                # it should be 'comma separated values but it is not'
-                #  eg.: 'boost-headers boost-_cmake'
-                if any([c in reqs for c in ',=']):
-                    # the right way
-                    for req in reqs.split(','):
-                        req = parse_requirement(req)
-                        self.__requires.append(req)
-                else:
-                    # conan's way
-                    for req in reqs.split(' '):
-                        req = parse_requirement(req)
-                        self.__requires.append(req)
-        return self.__requires
+                self._requires = parse_package_requires(reqs)
+        return self._requires
     
     @property
     def version(self) -> Version:
-        if self.__version is None:
+        if self._version is None:
             v = self.get('version')
             if v:
-                self.__version = Version(v)
-        return self.__version
+                self._version = Version(v)
+        return self._version
 
 
 class Package(CXXTarget, internal=True):
     all: dict[str, 'Package'] = dict()
 
     default = False
 
-    def __init__(self, name, search_paths: list[str] = list(), config_path: Path = None, data: Data = None, **kwargs) -> None:
+    def __init__(self, name, search_paths: list[str] = list(), config_path: Path = None, dan_plugin=None, search_plugin=True, data: Data = None, **kwargs) -> None:
         if data is not None:
             self.config_path = data.path
             self.data = data
         else:
             self.config_path = config_path or find_pkg_config(name, search_paths)
             self.data: Data = None
         self.search_paths = search_paths
         if not self.config_path:
             raise MissingPackage(name)
-        self.search_paths.insert(0, self.config_path.parent)
+        if not self.config_path.parent in self.search_paths:
+            self.search_paths.insert(0, self.config_path.parent)
         self.pn = name
         self.all[name] = self
 
         super().__init__(f'{name}-pkgconfig', **kwargs)
 
-        dan_plugin = find_file(rf'{name}\.py', [self.config_path.parent.parent])
-        if dan_plugin is not None:
-            spec = importlib.util.spec_from_file_location(
-                f'{name}_plugin', dan_plugin)
-            module = importlib.util.module_from_spec(spec)
-            setattr(module, 'self', self)
-            spec.loader.exec_module(module)
+        if dan_plugin:
+            self.__dan_plugin = dan_plugin
+        elif search_plugin:
+            self.__dan_plugin = find_file(rf'{name}\.py', [self.config_path.parent.parent])
+        else:
+            self.__dan_plugin = None
+        self.__load_plugin()
         self.__cflags = None
         self.__libs = None
         self.__lib_paths = None
         if not data:
             self.data = Data(self.config_path)
 
 
         self.version = self.data.version
+    
+    def __load_plugin(self):
+        if self.__dan_plugin is not None:
+            spec = importlib.util.spec_from_file_location(
+                f'{self.name}_plugin', self.__dan_plugin)
+            module = importlib.util.module_from_spec(spec)
+            setattr(module, 'self', self)
+            spec.loader.exec_module(module)
+
+
+    def __getstate__(self):
+        return {
+            'pn': self.pn,
+            'search_paths': self.search_paths,
+            'dan_plugin': self.__dan_plugin,
+            'config_path': self.config_path,
+            'data': self.data,
+            '__cflags': self.__cflags,
+            '__libs': self.__libs,
+            '__lib_paths': self.__lib_paths,
+        }
+    
+    def __setstate__(self, data):
+        from dan.core.include import context
+        makefile = context.current.root
+        self.__init__(data['pn'], data['search_paths'], data['config_path'],
+                      data=data['data'],
+                      dan_plugin=data['dan_plugin'],
+                      search_plugin=False,
+                      makefile=makefile)
+        self.__cflags = data['__cflags']
+        self.__libs = data['__libs']
+        self.__lib_paths = data['__lib_paths']
 
     @property
     def modification_time(self):
         return 0.0
 
     @property
     def found(self):
@@ -242,30 +300,45 @@
 
 
 _jinja_env: jinja2.Environment = None
 
 
 def find_package(name, spec: VersionSpec = None, search_paths: list = None, makefile = None):
     
-    if name in Package.all:
-        pkg = Package.all[name]
-        if spec and not spec.is_compatible(pkg.version):
-            raise RuntimeError(f'incompatible package {name} ({pkg.version} {spec})')
-        return pkg
+    pkg = None
+
     if makefile is None:
         from dan.core.include import context
         makefile = context.current
+
+    makefile = makefile.root
+
+    cache: list[Package] = Cache.instance(makefile.build_path / 'pkgconfig.cache', cache_name='pkgconfig', binary=True).data
+    if name in cache:
+        cached_pkg = cache[name]
+        if spec and not spec.is_compatible(cached_pkg.version):
+            raise RuntimeError(f'incompatible package {name} ({cached_pkg.version} {spec})')
+        return cached_pkg
+
     search_paths = search_paths or makefile.pkgs_path
     for config in find_pkg_configs(name, search_paths):
         if spec is not None:
             data = Data(config)
             if spec.is_compatible(data.version):
-                return Package(name, data=data, makefile=makefile)
+                pkg = Package(name, data=data, makefile=makefile)
+                break
+
         else:
-            return Package(name, config_path=config, makefile=makefile)
+            pkg = Package(name, config_path=config, makefile=makefile)
+            break
+    
+    if pkg:
+        cache[name] = pkg
+
+    return pkg
 
 
 def _get_jinja_env():
     global _jinja_env
     if _jinja_env is None:
         _jinja_env = jinja2.Environment(
             loader=jinja2.PackageLoader('dan.pkgconfig'))
```

### Comparing `dan-build-0.2.6/dan/src/git.py` & `dan-build-0.2.7/dan/src/git.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 
 class GitSources(Target, internal=True):
 
     url: str = None
     refspec: str = None
     patches: Iterable = list()
 
-    def __init__(self, *args, url=None, refspec=None, patches=None, dirname='sources', subdirectory=None, **kwargs) -> None:
+    def __init__(self, *args, url=None, refspec=None, patches=None, subdirectory=None, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         if url is not None:
             self.url = url
         if refspec is not None:
             self.refspec = refspec
         if patches is not None:
             self.patches = patches
         self.sha1 = None
-        self.output: Path = dirname
+        self.output = self.name
         self.git_dir: Path = self.output / '.git'
         self.subdirectory = subdirectory
 
     async def __build__(self):
         try:
             self.output.mkdir()            
             await async_run(f'git init -q', logger=self, cwd=self.output)
```

### Comparing `dan-build-0.2.6/dan/src/github.py` & `dan-build-0.2.7/dan/src/github.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/dan/src/tar.py` & `dan-build-0.2.7/dan/src/tar.py`

 * *Files 19% similar despite different names*

```diff
@@ -24,28 +24,32 @@
                         await f.write(chunk)
                         progressbar.update(len(chunk) // 1024)
 
 
 class TarSources(Target, internal=True):
 
     url: str
+    archive_name: str = None
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
-        self.output: Path = 'sources'
+        self.output = str(self.name)
 
     async def __build__(self):
         self.info(f'downloading {self.url}')
-        archive_name = self.url.split("/")[-1]
+        archive_name = self.archive_name or self.url.split("/")[-1]
         await fetch_file(self.url, self.build_path / archive_name)
         self.info(f'extracting {archive_name}')
         if archive_name.endswith('.zip'):
             with zipfile.ZipFile(self.build_path / archive_name) as f:
                 root = os.path.commonprefix(f.namelist())
-                f.extractall(self.output.parent)
+                f.extractall(self.output.with_suffix('.tmp_extract'))
         else:
             with tarfile.open(self.build_path / archive_name) as f:
                 root = os.path.commonprefix(f.getnames())
-                f.extractall(self.output.parent)
-        async with asyncio.TaskGroup() as g:
-            g.create_task(aiofiles.os.rename(self.output.parent / root, self.output))
-            g.create_task(aiofiles.os.remove(self.build_path / archive_name))
+                f.extractall(self.output.with_suffix('.tmp_extract'))
+        
+        await aiofiles.os.rename(self.output.with_suffix('.tmp_extract') / root, self.output)
+        await aiofiles.os.remove(self.build_path / archive_name)
+
+        if len(root) > 0:
+            await aiofiles.rmtree(self.output.with_suffix('.tmp_extract'))
```

### Comparing `dan-build-0.2.6/dan_build.egg-info/PKG-INFO` & `dan-build-0.2.7/dan_build.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dan-build
-Version: 0.2.6
+Version: 0.2.7
 Summary: Python-based build system.
 Author-email: Garcia Sylvain <garcia.6l20@gmail.com>, garcia.6l20@gmail.com
 License: MIT License
         
         Copyright (c) 2023 Sylvain Garcia
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dan-build-0.2.6/dan_build.egg-info/SOURCES.txt` & `dan-build-0.2.7/dan_build.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/pyproject.toml` & `dan-build-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/tests/test_cxx_errors.py` & `dan-build-0.2.7/tests/test_cxx_errors.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/tests/test_cxx_libraries.py` & `dan-build-0.2.7/tests/test_cxx_libraries.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/tests/test_cxx_simple.py` & `dan-build-0.2.7/tests/test_cxx_simple.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/tests/test_cxx_src_catch2.py` & `dan-build-0.2.7/tests/test_cxx_src_catch2.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.2.6/tests/test_python_errors.py` & `dan-build-0.2.7/tests/test_python_errors.py`

 * *Files identical despite different names*

