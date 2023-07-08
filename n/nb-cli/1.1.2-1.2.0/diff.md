# Comparing `tmp/nb-cli-1.1.2.tar.gz` & `tmp/nb-cli-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb-cli-1.1.2.tar", last modified: Sun Apr 16 04:19:51 2023, max compression
+gzip compressed data, was "nb-cli-1.2.0.tar", last modified: Sat Jul  8 16:00:00 2023, max compression
```

## Comparing `nb-cli-1.1.2.tar` & `nb-cli-1.2.0.tar`

### file list

```diff
@@ -1,74 +1,77 @@
--rw-r--r--   0        0        0     1065 2023-04-16 04:19:22.485298 nb-cli-1.1.2/LICENSE
--rw-r--r--   0        0        0     3350 2023-04-16 04:19:22.485298 nb-cli-1.1.2/README.md
--rw-r--r--   0        0        0      246 2023-04-16 04:19:22.485298 nb-cli-1.1.2/build.py
--rw-r--r--   0        0        0      795 2023-04-16 04:19:22.485298 nb-cli-1.1.2/nb_cli/__init__.py
--rw-r--r--   0        0        0      202 2023-04-16 04:19:22.485298 nb-cli-1.1.2/nb_cli/__main__.py
--rw-r--r--   0        0        0     3305 2023-04-16 04:19:22.485298 nb-cli-1.1.2/nb_cli/cli/__init__.py
--rw-r--r--   0        0        0      257 2023-04-16 04:19:22.485298 nb-cli-1.1.2/nb_cli/cli/commands/__init__.py
--rw-r--r--   0        0        0     6866 2023-04-16 04:19:22.485298 nb-cli-1.1.2/nb_cli/cli/commands/adapter.py
--rw-r--r--   0        0        0     4243 2023-04-16 04:19:22.485298 nb-cli-1.1.2/nb_cli/cli/commands/driver.py
--rw-r--r--   0        0        0     7195 2023-04-16 04:19:22.485298 nb-cli-1.1.2/nb_cli/cli/commands/plugin.py
--rw-r--r--   0        0        0    10063 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/cli/commands/project.py
--rw-r--r--   0        0        0     3409 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/cli/commands/self.py
--rw-r--r--   0        0        0     5459 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/cli/customize.py
--rw-r--r--   0        0        0     1966 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/cli/utils.py
--rw-r--r--   0        0        0      429 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/config/__init__.py
--rw-r--r--   0        0        0      661 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/config/model.py
--rw-r--r--   0        0        0     6153 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/config/parser.py
--rw-r--r--   0        0        0      347 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/consts.py
--rw-r--r--   0        0        0      373 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/exceptions.py
--rw-r--r--   0        0        0     2965 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/handlers/__init__.py
--rw-r--r--   0        0        0      865 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/handlers/adapter.py
--rw-r--r--   0        0        0      374 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/handlers/driver.py
--rw-r--r--   0        0        0     5756 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/handlers/meta.py
--rw-r--r--   0        0        0     3198 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/handlers/pip.py
--rw-r--r--   0        0        0     1557 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/handlers/plugin.py
--rw-r--r--   0        0        0     2990 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/handlers/process.py
--rw-r--r--   0        0        0     2665 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/handlers/project.py
--rw-r--r--   0        0        0     5718 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/handlers/reloader.py
--rw-r--r--   0        0        0     2063 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/handlers/script.py
--rw-r--r--   0        0        0     1860 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/handlers/signal.py
--rw-r--r--   0        0        0     3720 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/handlers/store.py
--rw-r--r--   0        0        0      734 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/handlers/venv.py
--rw-r--r--   0        0        0     1193 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/i18n.py
--rw-r--r--   0        0        0     8829 2023-04-16 04:19:49.185418 nb-cli-1.1.2/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.mo
--rw-r--r--   0        0        0    13703 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.po
--rw-r--r--   0        0        0      635 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/log/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/py.typed
--rw-r--r--   0        0        0      143 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/adapter/cookiecutter.json
--rw-r--r--   0        0        0      120 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/__init__.{{cookiecutter.py}}
--rw-r--r--   0        0        0      847 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/adapter.{{cookiecutter.py}}
--rw-r--r--   0        0        0      354 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/bot.{{cookiecutter.py}}
--rw-r--r--   0        0        0      203 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/config.{{cookiecutter.py}}
--rw-r--r--   0        0        0      688 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/event.{{cookiecutter.py}}
--rw-r--r--   0        0        0      676 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/message.{{cookiecutter.py}}
--rw-r--r--   0        0        0      164 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/plugin/cookiecutter.json
--rw-r--r--   0        0        0      315 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/plugin/hooks/post_gen_project.py
--rw-r--r--   0        0        0      385 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/__init__.{{cookiecutter.py}}
--rw-r--r--   0        0        0      114 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/config.{{cookiecutter.py}}
--rw-r--r--   0        0        0        0 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/plugins/.gitkeep
--rw-r--r--   0        0        0      259 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/project/bootstrap/cookiecutter.json
--rw-r--r--   0        0        0      132 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/.env.prod
--rw-r--r--   0        0        0      235 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/README.md
--rw-r--r--   0        0        0      611 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/pyproject.toml
--rw-r--r--   0        0        0      452 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/project/simple/cookiecutter.json
--rw-r--r--   0        0        0      307 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/project/simple/hooks/post_gen_project.py
--rw-r--r--   0        0        0      148 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env
--rw-r--r--   0        0        0       16 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env.dev
--rw-r--r--   0        0        0        0 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env.prod
--rw-r--r--   0        0        0     2087 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.gitignore
--rw-r--r--   0        0        0      331 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/README.md
--rw-r--r--   0        0        0      657 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/{{cookiecutter.custom.source_dir}}/plugins/.gitkeep
--rw-r--r--   0        0        0      232 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/scripts/meta/_package_version.py.jinja
--rw-r--r--   0        0        0      110 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/scripts/meta/nonebot_version.py.jinja
--rw-r--r--   0        0        0      105 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/scripts/meta/pip_version.py.jinja
--rw-r--r--   0        0        0      142 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/scripts/meta/python_version.py.jinja
--rw-r--r--   0        0        0      181 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/scripts/plugin/list_builtin_plugin.py.jinja
--rw-r--r--   0        0        0     1091 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/scripts/project/_prepare.py.jinja
--rw-r--r--   0        0        0      151 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/scripts/project/run_project.py.jinja
--rw-r--r--   0        0        0      222 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/scripts/script/_entrypoint.py.jinja
--rw-r--r--   0        0        0      158 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/scripts/script/list_scripts.py.jinja
--rw-r--r--   0        0        0      333 2023-04-16 04:19:22.489298 nb-cli-1.1.2/nb_cli/template/scripts/script/run_script.py.jinja
--rw-r--r--   0        0        0     2770 2023-04-16 04:19:22.489298 nb-cli-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     3994 1970-01-01 00:00:00.000000 nb-cli-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-08 15:59:26.355390 nb-cli-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3347 2023-07-08 15:59:26.355390 nb-cli-1.2.0/README.md
+-rw-r--r--   0        0        0      246 2023-07-08 15:59:26.355390 nb-cli-1.2.0/build.py
+-rw-r--r--   0        0        0      795 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/__init__.py
+-rw-r--r--   0        0        0      202 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/__main__.py
+-rw-r--r--   0        0        0     3305 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/cli/__init__.py
+-rw-r--r--   0        0        0      257 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/cli/commands/__init__.py
+-rw-r--r--   0        0        0     6866 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/cli/commands/adapter.py
+-rw-r--r--   0        0        0     4243 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/cli/commands/driver.py
+-rw-r--r--   0        0        0     7195 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/cli/commands/plugin.py
+-rw-r--r--   0        0        0    10538 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/cli/commands/project.py
+-rw-r--r--   0        0        0     3409 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/cli/commands/self.py
+-rw-r--r--   0        0        0     5459 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/cli/customize.py
+-rw-r--r--   0        0        0     1966 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/cli/utils.py
+-rw-r--r--   0        0        0      429 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/config/__init__.py
+-rw-r--r--   0        0        0      661 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/config/model.py
+-rw-r--r--   0        0        0     6220 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/config/parser.py
+-rw-r--r--   0        0        0      347 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/consts.py
+-rw-r--r--   0        0        0      472 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/exceptions.py
+-rw-r--r--   0        0        0      214 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/extensions.py
+-rw-r--r--   0        0        0     3030 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/handlers/__init__.py
+-rw-r--r--   0        0        0      865 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/handlers/adapter.py
+-rw-r--r--   0        0        0      374 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/handlers/driver.py
+-rw-r--r--   0        0        0     6766 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/handlers/meta.py
+-rw-r--r--   0        0        0     3198 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/handlers/pip.py
+-rw-r--r--   0        0        0     1557 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/handlers/plugin.py
+-rw-r--r--   0        0        0     2990 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/handlers/process.py
+-rw-r--r--   0        0        0     2665 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/handlers/project.py
+-rw-r--r--   0        0        0     5718 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/handlers/reloader.py
+-rw-r--r--   0        0        0     2150 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/handlers/script.py
+-rw-r--r--   0        0        0     1860 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/handlers/signal.py
+-rw-r--r--   0        0        0     4082 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/handlers/store.py
+-rw-r--r--   0        0        0      734 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/handlers/venv.py
+-rw-r--r--   0        0        0     1193 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/i18n.py
+-rw-r--r--   0        0        0     8966 2023-07-08 15:59:57.571354 nb-cli-1.2.0/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.mo
+-rw-r--r--   0        0        0    13886 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.po
+-rw-r--r--   0        0        0      635 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/log/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/py.typed
+-rw-r--r--   0        0        0      143 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/adapter/cookiecutter.json
+-rw-r--r--   0        0        0      120 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/__init__.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      847 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/adapter.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      354 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/bot.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      203 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/config.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      688 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/event.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      676 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/message.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      164 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/plugin/cookiecutter.json
+-rw-r--r--   0        0        0      315 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/plugin/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      365 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/__init__.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      114 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/config.{{cookiecutter.py}}
+-rw-r--r--   0        0        0        0 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/plugins/.gitkeep
+-rw-r--r--   0        0        0      318 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/project/bootstrap/cookiecutter.json
+-rw-r--r--   0        0        0      236 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/project/bootstrap/hooks/pre_gen_project.py
+-rw-r--r--   0        0        0      141 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/.env.prod
+-rw-r--r--   0        0        0      232 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/README.md
+-rw-r--r--   0        0        0      620 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/pyproject.toml
+-rw-r--r--   0        0        0      501 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/project/simple/cookiecutter.json
+-rw-r--r--   0        0        0      307 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/project/simple/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      236 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/project/simple/hooks/pre_gen_project.py
+-rw-r--r--   0        0        0      157 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env
+-rw-r--r--   0        0        0       16 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env.dev
+-rw-r--r--   0        0        0        0 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env.prod
+-rw-r--r--   0        0        0     2087 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.gitignore
+-rw-r--r--   0        0        0      328 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/README.md
+-rw-r--r--   0        0        0      666 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/{{cookiecutter.custom.source_dir}}/plugins/.gitkeep
+-rw-r--r--   0        0        0      232 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/scripts/meta/_package_version.py.jinja
+-rw-r--r--   0        0        0      110 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/scripts/meta/nonebot_version.py.jinja
+-rw-r--r--   0        0        0      105 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/scripts/meta/pip_version.py.jinja
+-rw-r--r--   0        0        0      142 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/scripts/meta/python_version.py.jinja
+-rw-r--r--   0        0        0      181 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/scripts/plugin/list_builtin_plugin.py.jinja
+-rw-r--r--   0        0        0     1091 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/scripts/project/_prepare.py.jinja
+-rw-r--r--   0        0        0      151 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/scripts/project/run_project.py.jinja
+-rw-r--r--   0        0        0      222 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/scripts/script/_entrypoint.py.jinja
+-rw-r--r--   0        0        0      158 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/scripts/script/list_scripts.py.jinja
+-rw-r--r--   0        0        0      333 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/scripts/script/run_script.py.jinja
+-rw-r--r--   0        0        0     2732 2023-07-08 15:59:26.359390 nb-cli-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3991 1970-01-01 00:00:00.000000 nb-cli-1.2.0/PKG-INFO
```

### Comparing `nb-cli-1.1.2/LICENSE` & `nb-cli-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.2/README.md` & `nb-cli-1.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 </p>
 
 <p align="center">
   <a href="https://cli.nonebot.dev/">文档</a>
   ·
   <a href="https://cli.nonebot.dev/docs/guide/installation">安装</a>
   ·
-  <a href="https://v2.nonebot.dev/">NoneBot 文档</a>
+  <a href="https://nonebot.dev/">NoneBot 文档</a>
 </p>
 
 ## 功能
 
 - 创建新的 Nonebot 项目
 - 启动 Nonebot
 - 管理插件
```

### Comparing `nb-cli-1.1.2/nb_cli/__init__.py` & `nb-cli-1.2.0/nb_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.2/nb_cli/cli/__init__.py` & `nb-cli-1.2.0/nb_cli/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.2/nb_cli/cli/commands/adapter.py` & `nb-cli-1.2.0/nb_cli/cli/commands/adapter.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.2/nb_cli/cli/commands/driver.py` & `nb-cli-1.2.0/nb_cli/cli/commands/driver.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.2/nb_cli/cli/commands/plugin.py` & `nb-cli-1.2.0/nb_cli/cli/commands/plugin.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.2/nb_cli/cli/commands/project.py` & `nb-cli-1.2.0/nb_cli/cli/commands/project.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 import sys
+import json
 from pathlib import Path
 from logging import Logger
 from functools import partial
 from dataclasses import field, dataclass
 from typing import Any, Dict, List, Optional
 
 import click
@@ -90,15 +91,17 @@
             index
             for index, driver in enumerate(all_drivers)
             if driver.name in DEFAULT_DRIVER
         ],
         validator=bool,
         error_message=_("Chosen drivers is not valid!"),
     ).prompt_async(style=CLI_DEFAULT_STYLE)
-    context.variables["drivers"] = [d.data.dict() for d in drivers]
+    context.variables["drivers"] = json.dumps(
+        {d.data.project_link: d.data.dict() for d in drivers}
+    )
     context.packages.extend(
         [d.data.project_link for d in drivers if d.data.project_link]
     )
 
     confirm = False
     adapters = []
     while not confirm:
@@ -114,15 +117,17 @@
             if adapters
             else await ConfirmPrompt(
                 _("You haven't chosen any adapter! Please confirm."),
                 default_choice=False,
             ).prompt_async(style=CLI_DEFAULT_STYLE)
         )
 
-    context.variables["adapters"] = [a.data.dict() for a in adapters]
+    context.variables["adapters"] = json.dumps(
+        {a.data.project_link: a.data.dict() for a in adapters}
+    )
     context.packages.extend([a.data.project_link for a in adapters])
 
     return context
 
 
 async def prompt_simple_context(context: ProjectContext) -> ProjectContext:
     dir_name = (
@@ -236,39 +241,48 @@
         proc = await call_pip_install(
             ["nonebot2", *context.packages],
             pip_args,
             python_path=config_manager.python_path,
         )
         await proc.wait()
 
-        builtin_plugins = await list_builtin_plugins(
-            python_path=config_manager.python_path
-        )
-        try:
-            loaded_builtin_plugins = [
-                c.data
-                for c in await CheckboxPrompt(
-                    _("Which builtin plugin(s) would you like to use?"),
-                    [Choice(p, p) for p in builtin_plugins],
-                ).prompt_async(style=CLI_DEFAULT_STYLE)
-            ]
-        except CancelledError:
-            ctx.exit()
-
-        try:
-            for plugin in loaded_builtin_plugins:
-                config_manager.add_builtin_plugin(plugin)
-        except Exception as e:
+        if proc.returncode == 0:
+            builtin_plugins = await list_builtin_plugins(
+                python_path=config_manager.python_path
+            )
+            try:
+                loaded_builtin_plugins = [
+                    c.data
+                    for c in await CheckboxPrompt(
+                        _("Which builtin plugin(s) would you like to use?"),
+                        [Choice(p, p) for p in builtin_plugins],
+                    ).prompt_async(style=CLI_DEFAULT_STYLE)
+                ]
+            except CancelledError:
+                ctx.exit()
+
+            try:
+                for plugin in loaded_builtin_plugins:
+                    config_manager.add_builtin_plugin(plugin)
+            except Exception as e:
+                click.secho(
+                    _(
+                        "Failed to add builtin plugins {builtin_plugins} to config: {e}"
+                    ).format(builtin_plugin=loaded_builtin_plugins, e=e),
+                    fg="red",
+                )
+                ctx.exit()
+        else:
             click.secho(
                 _(
-                    "Failed to add builtin plugins {builtin_plugins} to config: {e}"
-                ).format(builtin_plugin=loaded_builtin_plugins, e=e),
+                    "Failed to install dependencies! "
+                    "You should install the dependencies manually."
+                ),
                 fg="red",
             )
-            ctx.exit()
 
     click.secho(_("Done!"), fg="green")
     click.secho(
         _(
             "Add following packages to your project using dependency manager like poetry or pdm:"
         ),
         fg="green",
```

### Comparing `nb-cli-1.1.2/nb_cli/cli/commands/self.py` & `nb-cli-1.2.0/nb_cli/cli/commands/self.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.2/nb_cli/cli/customize.py` & `nb-cli-1.2.0/nb_cli/cli/customize.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.2/nb_cli/cli/utils.py` & `nb-cli-1.2.0/nb_cli/cli/utils.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.2/nb_cli/config/model.py` & `nb-cli-1.2.0/nb_cli/config/model.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.2/nb_cli/config/parser.py` & `nb-cli-1.2.0/nb_cli/config/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import tomlkit
 from tomlkit.toml_document import TOMLDocument
 
 from nb_cli import _
 from nb_cli.log import SUCCESS
 from nb_cli.consts import WINDOWS
+from nb_cli.exceptions import ProjectNotFoundError
 
 from .model import SimpleInfo, NoneBotConfig
 
 CONFIG_FILE = "pyproject.toml"
 CONFIG_FILE_ENCODING = "utf-8"
 
 
@@ -40,15 +41,15 @@
 
     @staticmethod
     def _locate_project_root(cwd: Optional[Path] = None) -> Path:
         cwd = (cwd or Path.cwd()).resolve()
         for dir in (cwd,) + tuple(cwd.parents):
             if dir.joinpath(CONFIG_FILE).is_file():
                 return dir
-        raise RuntimeError(
+        raise ProjectNotFoundError(
             _(
                 "Cannot find project root directory! {config_file} file not exists."
             ).format(config_file=CONFIG_FILE)
         )
 
     @property
     def project_root(self) -> Path:
@@ -72,15 +73,15 @@
     @property
     def python_path(self) -> Optional[str]:
         if python := (self._python_path or self._global_python_path):
             return python
         elif self.use_venv:
             try:
                 cwd = self.project_root.resolve()
-            except RuntimeError:
+            except ProjectNotFoundError:
                 cwd = Path.cwd().resolve()
 
             if cwd in self._path_venv_cache:
                 return self._path_venv_cache[cwd]
 
             if venv_python := self._detact_virtual_env(cwd):
                 self._path_venv_cache[cwd] = venv_python
```

### Comparing `nb-cli-1.1.2/nb_cli/handlers/__init__.py` & `nb-cli-1.2.0/nb_cli/handlers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from .meta import requires_python as requires_python
 from .meta import get_project_root as get_project_root
 from .meta import requires_nonebot as requires_nonebot
 from .meta import get_default_python as get_default_python
 from .meta import get_nonebot_config as get_nonebot_config
 from .meta import get_python_version as get_python_version
 from .meta import get_nonebot_version as get_nonebot_version
+from .meta import requires_project_root as requires_project_root
 
 # isort: split
 
 # package
 from .store import load_module_data as load_module_data
 from .store import format_package_results as format_package_results
```

### Comparing `nb-cli-1.1.2/nb_cli/handlers/adapter.py` & `nb-cli-1.2.0/nb_cli/handlers/adapter.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.2/nb_cli/handlers/meta.py` & `nb-cli-1.2.0/nb_cli/handlers/meta.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,25 +3,24 @@
 from pathlib import Path
 from functools import wraps
 from typing_extensions import ParamSpec
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
-    Union,
     TypeVar,
     Callable,
     Optional,
     Coroutine,
     cast,
 )
 
 from nb_cli import _, cache
 from nb_cli.consts import WINDOWS, REQUIRES_PYTHON
-from nb_cli.config import GLOBAL_CONFIG, NoneBotConfig
+from nb_cli.config import GLOBAL_CONFIG, ConfigManager, NoneBotConfig
 from nb_cli.exceptions import (
     PipNotInstalledError,
     PythonInterpreterError,
     NoneBotNotInstalledError,
 )
 
 from . import templates
@@ -45,16 +44,28 @@
     return figlet_format("NoneBot", font="basic").strip()
 
 
 def get_nonebot_config() -> NoneBotConfig:
     return GLOBAL_CONFIG.get_nonebot_config()
 
 
-def get_project_root() -> Path:
-    return GLOBAL_CONFIG.project_root
+def get_project_root(cwd: Optional[Path] = None) -> Path:
+    config = ConfigManager(working_dir=cwd) if cwd is not None else GLOBAL_CONFIG
+    return config.project_root
+
+
+def requires_project_root(
+    func: Callable[P, Coroutine[Any, Any, R]]
+) -> Callable[P, Coroutine[Any, Any, R]]:
+    @wraps(func)
+    async def wrapper(*args: P.args, **kwargs: P.kwargs) -> R:
+        get_project_root(cast(Optional[Path], kwargs.get("cwd")))
+        return await func(*args, **kwargs)
+
+    return wrapper
 
 
 if TYPE_CHECKING:
 
     async def _get_env_python() -> str:
         ...
 
@@ -78,32 +89,37 @@
                     continue
         raise PythonInterpreterError(
             _("Cannot find a valid Python interpreter.")
             + (f" stdout={stdout!r}" if stdout else "")
         )
 
 
-async def get_default_python() -> str:
-    if GLOBAL_CONFIG.python_path is not None:
-        return GLOBAL_CONFIG.python_path
+async def get_default_python(cwd: Optional[Path] = None) -> str:
+    config = ConfigManager(working_dir=cwd) if cwd is not None else GLOBAL_CONFIG
+    if config.python_path is not None:
+        return config.python_path
 
     return await _get_env_python()
 
 
 if TYPE_CHECKING:
 
-    async def get_python_version(python_path: Optional[str] = None) -> Dict[str, int]:
+    async def get_python_version(
+        python_path: Optional[str] = None, cwd: Optional[Path] = None
+    ) -> Dict[str, int]:
         ...
 
 else:
 
     @cache(ttl=None)
-    async def get_python_version(python_path: Optional[str] = None) -> Dict[str, int]:
+    async def get_python_version(
+        python_path: Optional[str] = None, cwd: Optional[Path] = None
+    ) -> Dict[str, int]:
         if python_path is None:
-            python_path = await get_default_python()
+            python_path = await get_default_python(cwd)
 
         t = templates.get_template("meta/python_version.py.jinja")
         proc = await create_process(
             python_path,
             "-W",
             "ignore",
             "-c",
@@ -116,15 +132,16 @@
 
 def requires_python(
     func: Callable[P, Coroutine[Any, Any, R]]
 ) -> Callable[P, Coroutine[Any, Any, R]]:
     @wraps(func)
     async def wrapper(*args: P.args, **kwargs: P.kwargs) -> R:
         version = await get_python_version(
-            cast(Union[str, None], kwargs.get("python_path"))
+            cast(Optional[str], kwargs.get("python_path")),
+            cast(Optional[Path], kwargs.get("cwd")),
         )
         if (version["major"], version["minor"]) >= REQUIRES_PYTHON:
             return await func(*args, **kwargs)
 
         raise PythonInterpreterError(
             _("Python {major}.{minor} is not supported.").format(
                 major=version["major"], minor=version["minor"]
@@ -132,23 +149,27 @@
         )
 
     return wrapper
 
 
 if TYPE_CHECKING:
 
-    async def get_nonebot_version(python_path: Optional[str] = None) -> str:
+    async def get_nonebot_version(
+        python_path: Optional[str] = None, cwd: Optional[Path] = None
+    ) -> str:
         ...
 
 else:
 
     @cache(ttl=None)
-    async def get_nonebot_version(python_path: Optional[str] = None) -> str:
+    async def get_nonebot_version(
+        python_path: Optional[str] = None, cwd: Optional[Path] = None
+    ) -> str:
         if python_path is None:
-            python_path = await get_default_python()
+            python_path = await get_default_python(cwd)
 
         t = templates.get_template("meta/nonebot_version.py.jinja")
         proc = await create_process(
             python_path,
             "-W",
             "ignore",
             "-c",
@@ -159,35 +180,43 @@
         return json.loads(stdout.strip())
 
 
 def requires_nonebot(
     func: Callable[P, Coroutine[Any, Any, R]]
 ) -> Callable[P, Coroutine[Any, Any, R]]:
     @wraps(func)
+    @requires_project_root
     @requires_python
     async def wrapper(*args: P.args, **kwargs: P.kwargs) -> R:
-        if await get_nonebot_version(cast(Union[str, None], kwargs.get("python_path"))):
+        if await get_nonebot_version(
+            cast(Optional[str], kwargs.get("python_path")),
+            cast(Optional[Path], kwargs.get("cwd")),
+        ):
             return await func(*args, **kwargs)
 
         raise NoneBotNotInstalledError(_("NoneBot is not installed."))
 
     return wrapper
 
 
 if TYPE_CHECKING:
 
-    async def get_pip_version(python_path: Optional[str] = None) -> str:
+    async def get_pip_version(
+        python_path: Optional[str] = None, cwd: Optional[Path] = None
+    ) -> str:
         ...
 
 else:
 
     @cache(ttl=None)
-    async def get_pip_version(python_path: Optional[str] = None) -> str:
+    async def get_pip_version(
+        python_path: Optional[str] = None, cwd: Optional[Path] = None
+    ) -> str:
         if python_path is None:
-            python_path = await get_default_python()
+            python_path = await get_default_python(cwd)
 
         t = templates.get_template("meta/pip_version.py.jinja")
         proc = await create_process(
             python_path,
             "-W",
             "ignore",
             "-c",
@@ -200,13 +229,16 @@
 
 def requires_pip(
     func: Callable[P, Coroutine[Any, Any, R]]
 ) -> Callable[P, Coroutine[Any, Any, R]]:
     @wraps(func)
     @requires_python
     async def wrapper(*args: P.args, **kwargs: P.kwargs) -> R:
-        if await get_pip_version(cast(Union[str, None], kwargs.get("python_path"))):
+        if await get_pip_version(
+            cast(Optional[str], kwargs.get("python_path")),
+            cast(Optional[Path], kwargs.get("cwd")),
+        ):
             return await func(*args, **kwargs)
 
         raise PipNotInstalledError(_("pip is not installed."))
 
     return wrapper
```

### Comparing `nb-cli-1.1.2/nb_cli/handlers/pip.py` & `nb-cli-1.2.0/nb_cli/handlers/pip.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.2/nb_cli/handlers/plugin.py` & `nb-cli-1.2.0/nb_cli/handlers/plugin.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.2/nb_cli/handlers/process.py` & `nb-cli-1.2.0/nb_cli/handlers/process.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.2/nb_cli/handlers/project.py` & `nb-cli-1.2.0/nb_cli/handlers/project.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.2/nb_cli/handlers/reloader.py` & `nb-cli-1.2.0/nb_cli/handlers/reloader.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.2/nb_cli/handlers/script.py` & `nb-cli-1.2.0/nb_cli/handlers/script.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,21 +9,25 @@
 from .process import create_process
 from .meta import (
     requires_python,
     get_project_root,
     requires_nonebot,
     get_default_python,
     get_nonebot_config,
+    requires_project_root,
 )
 
 
+@requires_project_root
 @requires_python
-async def list_scripts(*, python_path: Optional[str] = None) -> List[str]:
+async def list_scripts(
+    *, python_path: Optional[str] = None, cwd: Optional[Path] = None
+) -> List[str]:
     if python_path is None:
-        python_path = await get_default_python()
+        python_path = await get_default_python(cwd)
 
     t = templates.get_template("script/list_scripts.py.jinja")
     proc = await create_process(
         python_path,
         "-W",
         "ignore",
         "-c",
```

### Comparing `nb-cli-1.1.2/nb_cli/handlers/signal.py` & `nb-cli-1.2.0/nb_cli/handlers/signal.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.2/nb_cli/handlers/store.py` & `nb-cli-1.2.0/nb_cli/handlers/store.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import shutil
-from asyncio import as_completed
+from asyncio import create_task, as_completed
 from typing import TYPE_CHECKING, List, Union, Literal, TypeVar, Optional, overload
 
 import httpx
 from wcwidth import wcswidth
 
 from nb_cli import _, cache
 from nb_cli.exceptions import ModuleLoadFailed
@@ -47,29 +47,35 @@
             raise ValueError(
                 _("Invalid module type: {module_type}").format(module_type=module_type)
             )
         module_name: str = getattr(module_class.__config__, "module_name")
 
         exceptions: List[Exception] = []
         urls = [
-            f"https://v2.nonebot.dev/{module_name}.json",
-            f"https://raw.fastgit.org/nonebot/nonebot2/master/website/static/{module_name}.json",
-            f"https://cdn.jsdelivr.net/gh/nonebot/nonebot2/website/static/{module_name}.json",
+            f"https://registry.nonebot.dev/{module_name}.json",
+            f"https://cdn.jsdelivr.net/gh/nonebot/registry@results/{module_name}.json",
+            f"https://cdn.staticaly.com/gh/nonebot/registry@results/{module_name}.json",
+            f"https://jsd.cdn.zzko.cn/gh/nonebot/registry@results/{module_name}.json",
+            f"https://ghproxy.com/https://raw.githubusercontent.com/nonebot/registry/results/{module_name}.json",
         ]
 
         async def _request(url: str) -> httpx.Response:
             async with httpx.AsyncClient() as client:
                 return await client.get(url)
 
-        tasks = [_request(url) for url in urls]
+        tasks = [create_task(_request(url)) for url in urls]
         for future in as_completed(tasks):
             try:
                 resp = await future
                 items = resp.json()
-                return [module_class.parse_obj(item) for item in items]  # type: ignore
+                result = [module_class.parse_obj(item) for item in items]
+                for task in tasks:
+                    if not task.done():
+                        task.cancel()
+                return result  # type: ignore
             except Exception as e:
                 exceptions.append(e)
 
         raise ModuleLoadFailed(
             _("Failed to get {module_type} list.").format(module_type=module_type),
             exceptions,
         )
```

### Comparing `nb-cli-1.1.2/nb_cli/handlers/venv.py` & `nb-cli-1.2.0/nb_cli/handlers/venv.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.2/nb_cli/i18n.py` & `nb-cli-1.2.0/nb_cli/i18n.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.2/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.mo` & `nb-cli-1.2.0/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: nb-cli 1.0.0\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-04-12 05:58+0000\n"
+"POT-Creation-Date: 2023-07-08 15:40+0000\n"
 "PO-Revision-Date: 2023-01-11 08:56+0000\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh_Hans_CN\n"
 "Language-Team: zh_Hans_CN <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -92,14 +92,18 @@
 
 msgid "Failed to add plugin {plugin.name} to config: {e}"
 msgstr "添加插件 {plugin.name} 到配置文件失败: {e}"
 
 msgid "Failed to get {module_type} list."
 msgstr "获取 {module_type} 列表失败."
 
+msgid ""
+"Failed to install dependencies! You should install the dependencies manually."
+msgstr "安装依赖失败! 请手动安装依赖."
+
 msgid "Failed to remove adapter {adapter.name} from config: {e}"
 msgstr "从配置文件移除适配器 {adapter.name} 失败: {e}"
 
 msgid "Failed to remove plugin {plugin.name} from config: {e}"
 msgstr "从配置文件中移除插件 {plugin.name} 失败: {e}"
 
 msgid "Files to ignore for changes."
```

### Comparing `nb-cli-1.1.2/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.po` & `nb-cli-1.2.0/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the nb-cli project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: nb-cli 1.0.0\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-04-12 05:58+0000\n"
+"POT-Creation-Date: 2023-07-08 15:40+0000\n"
 "PO-Revision-Date: 2023-01-11 08:56+0000\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh_Hans_CN\n"
 "Language-Team: zh_Hans_CN <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -237,141 +237,147 @@
 msgid "Plugin name:"
 msgstr "插件名称:"
 
 #: nb_cli/cli/commands/plugin.py:193
 msgid "Use nested plugin?"
 msgstr "使用嵌套插件?"
 
-#: nb_cli/cli/commands/plugin.py:210 nb_cli/cli/commands/project.py:136
+#: nb_cli/cli/commands/plugin.py:210 nb_cli/cli/commands/project.py:141
 msgid "Where to store the plugin?"
 msgstr "请输入插件存储位置:"
 
-#: nb_cli/cli/commands/project.py:44
+#: nb_cli/cli/commands/project.py:45
 msgid "bootstrap (for beginner or user)"
 msgstr "bootstrap (初学者或用户)"
 
-#: nb_cli/cli/commands/project.py:45
+#: nb_cli/cli/commands/project.py:46
 msgid "simple (for plugin developer)"
 msgstr "simple (插件开发者)"
 
-#: nb_cli/cli/commands/project.py:73
+#: nb_cli/cli/commands/project.py:74
 msgid "Loading adapters..."
 msgstr "正在加载适配器..."
 
-#: nb_cli/cli/commands/project.py:75
+#: nb_cli/cli/commands/project.py:76
 msgid "Loading drivers..."
 msgstr "正在加载驱动器..."
 
-#: nb_cli/cli/commands/project.py:80
+#: nb_cli/cli/commands/project.py:81
 msgid "Project Name:"
 msgstr "项目名称:"
 
-#: nb_cli/cli/commands/project.py:82
+#: nb_cli/cli/commands/project.py:83
 msgid "Invalid project name!"
 msgstr "无效的项目名称!"
 
-#: nb_cli/cli/commands/project.py:87
+#: nb_cli/cli/commands/project.py:88
 msgid "Which driver(s) would you like to use?"
 msgstr "要使用哪些驱动器?"
 
-#: nb_cli/cli/commands/project.py:95
+#: nb_cli/cli/commands/project.py:96
 msgid "Chosen drivers is not valid!"
 msgstr "选择的驱动器不合法!"
 
-#: nb_cli/cli/commands/project.py:106
+#: nb_cli/cli/commands/project.py:109
 msgid "Which adapter(s) would you like to use?"
 msgstr "要使用哪些适配器?"
 
-#: nb_cli/cli/commands/project.py:116
+#: nb_cli/cli/commands/project.py:119
 msgid "You haven't chosen any adapter! Please confirm."
 msgstr "你没有选择任何适配器! 请确认."
 
-#: nb_cli/cli/commands/project.py:132
+#: nb_cli/cli/commands/project.py:137
 msgid "1) In a \"{dir_name}\" folder"
 msgstr "1) 在 \"{dir_name}\" 文件夹中"
 
-#: nb_cli/cli/commands/project.py:133
+#: nb_cli/cli/commands/project.py:138
 msgid "2) In a \"src\" folder"
 msgstr "2) 在 \"src\" 文件夹中"
 
-#: nb_cli/cli/commands/project.py:153
+#: nb_cli/cli/commands/project.py:158
 msgid "Create a NoneBot project."
 msgstr "创建一个 NoneBot 项目."
 
-#: nb_cli/cli/commands/project.py:161
+#: nb_cli/cli/commands/project.py:166
 msgid "The project template to use."
 msgstr "使用的项目模板."
 
-#: nb_cli/cli/commands/project.py:166
+#: nb_cli/cli/commands/project.py:171
 msgid "The python interpreter virtualenv is installed into."
 msgstr "虚拟环境使用的 Python 解释器."
 
-#: nb_cli/cli/commands/project.py:183
+#: nb_cli/cli/commands/project.py:188
 msgid "Select a template to use:"
 msgstr "选择一个要使用的模板:"
 
-#: nb_cli/cli/commands/project.py:205
+#: nb_cli/cli/commands/project.py:210
 msgid "Install dependencies now?"
 msgstr "立即安装依赖?"
 
-#: nb_cli/cli/commands/project.py:218
+#: nb_cli/cli/commands/project.py:223
 msgid "Create virtual environment?"
 msgstr "创建虚拟环境?"
 
-#: nb_cli/cli/commands/project.py:225
+#: nb_cli/cli/commands/project.py:230
 msgid "Creating virtual environment in {venv_dir} ..."
 msgstr "在 {venv_dir} 中创建虚拟环境..."
 
-#: nb_cli/cli/commands/project.py:250
+#: nb_cli/cli/commands/project.py:256
 msgid "Which builtin plugin(s) would you like to use?"
 msgstr "要使用哪些内置插件?"
 
-#: nb_cli/cli/commands/project.py:262
+#: nb_cli/cli/commands/project.py:268
 msgid "Failed to add builtin plugins {builtin_plugins} to config: {e}"
 msgstr "添加内置插件 {builtin_plugins} 到配置文件失败: {e}"
 
-#: nb_cli/cli/commands/project.py:269
+#: nb_cli/cli/commands/project.py:276
+msgid ""
+"Failed to install dependencies! You should install the dependencies "
+"manually."
+msgstr "安装依赖失败! 请手动安装依赖."
+
+#: nb_cli/cli/commands/project.py:283
 msgid "Done!"
 msgstr "完成!"
 
-#: nb_cli/cli/commands/project.py:271
+#: nb_cli/cli/commands/project.py:285
 msgid ""
 "Add following packages to your project using dependency manager like "
 "poetry or pdm:"
 msgstr "使用 poetry 或 pdm 等依赖管理工具添加以下包:"
 
-#: nb_cli/cli/commands/project.py:277
+#: nb_cli/cli/commands/project.py:291
 msgid "Run the following command to start your bot:"
 msgstr "运行以下命令来启动你的机器人:"
 
-#: nb_cli/cli/commands/project.py:282
+#: nb_cli/cli/commands/project.py:296
 msgid "Generate entry file of your bot."
 msgstr "生成机器人的入口文件."
 
-#: nb_cli/cli/commands/project.py:288
+#: nb_cli/cli/commands/project.py:302
 msgid "The file script saved to."
 msgstr "脚本文件保存路径."
 
-#: nb_cli/cli/commands/project.py:297
+#: nb_cli/cli/commands/project.py:311
 msgid "Run the bot in current folder."
 msgstr "在当前文件夹中运行机器人."
 
-#: nb_cli/cli/commands/project.py:304
+#: nb_cli/cli/commands/project.py:318
 msgid "Exist entry file of your bot."
 msgstr "存在的机器人入口文件."
 
-#: nb_cli/cli/commands/project.py:311
+#: nb_cli/cli/commands/project.py:325
 msgid "Reload the bot when file changed."
 msgstr "当文件发生变化时重新加载机器人."
 
-#: nb_cli/cli/commands/project.py:317
+#: nb_cli/cli/commands/project.py:331
 msgid "Files to watch for changes."
 msgstr "要监视变化的文件."
 
-#: nb_cli/cli/commands/project.py:323
+#: nb_cli/cli/commands/project.py:337
 msgid "Files to ignore for changes."
 msgstr "要忽略变化的文件."
 
 #: nb_cli/cli/commands/self.py:18
 msgid "Manage NB CLI."
 msgstr "管理 NB CLI."
 
@@ -395,35 +401,35 @@
 msgid "Package name you want to uninstall?"
 msgstr "要卸载的包名?"
 
 #: nb_cli/cli/commands/self.py:110
 msgid "List installed packages in cli venv."
 msgstr "列出 cli 虚拟环境中已安装的包."
 
-#: nb_cli/config/parser.py:48
+#: nb_cli/config/parser.py:49
 msgid "Cannot find project root directory! {config_file} file not exists."
 msgstr "无法找到项目根目录! {config_file} 文件不存在."
 
-#: nb_cli/config/parser.py:90
+#: nb_cli/config/parser.py:91
 msgid "Using python: {python_path}"
 msgstr "使用 Python: {python_path}"
 
-#: nb_cli/handlers/meta.py:80
+#: nb_cli/handlers/meta.py:91
 msgid "Cannot find a valid Python interpreter."
 msgstr "无法找到可用的 Python 解释器."
 
-#: nb_cli/handlers/meta.py:129
+#: nb_cli/handlers/meta.py:146
 msgid "Python {major}.{minor} is not supported."
 msgstr "Python {major}.{minor} 不受支持."
 
-#: nb_cli/handlers/meta.py:171
+#: nb_cli/handlers/meta.py:196
 msgid "NoneBot is not installed."
 msgstr "NoneBot 未安装."
 
-#: nb_cli/handlers/meta.py:210
+#: nb_cli/handlers/meta.py:242
 msgid "pip is not installed."
 msgstr "pip 未安装."
 
 #: nb_cli/handlers/reloader.py:120
 msgid "Watchfiles detected changes in {paths}. Reloading..."
 msgstr "Watchfiles 在 {paths} 中发现变化. 正在重新加载..."
 
@@ -443,10 +449,10 @@
 msgid "Stopped reloader."
 msgstr "停止重载监视"
 
 #: nb_cli/handlers/store.py:48
 msgid "Invalid module type: {module_type}"
 msgstr "无效的模块类型: {module_type}"
 
-#: nb_cli/handlers/store.py:73
+#: nb_cli/handlers/store.py:79
 msgid "Failed to get {module_type} list."
 msgstr "获取 {module_type} 列表失败."
```

### Comparing `nb-cli-1.1.2/nb_cli/log/__init__.py` & `nb-cli-1.2.0/nb_cli/log/__init__.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.2/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/adapter.{{cookiecutter.py}}` & `nb-cli-1.2.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/adapter.{{cookiecutter.py}}`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.2/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/event.{{cookiecutter.py}}` & `nb-cli-1.2.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/event.{{cookiecutter.py}}`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.2/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/message.{{cookiecutter.py}}` & `nb-cli-1.2.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/message.{{cookiecutter.py}}`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.2/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/pyproject.toml` & `nb-cli-1.2.0/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 version = "0.1.0"
 description = "{{ cookiecutter.computed.project_desc }}"
 readme = "README.md"
 requires-python = ">=3.8, <4.0"
 
 [tool.nonebot]
 {% set adapters = [] -%}
-{% for adapter in cookiecutter.nonebot.adapters -%}
+{% for adapter in cookiecutter.nonebot.adapters.values() -%}
 {% set name = adapter.name -%}
 {% set module_name = adapter.module_name -%}
 {% set adapter_str = '{ name = "%s", module_name = "%s" }'|format(name, module_name) -%}
 {% set _ = adapters.append(adapter_str) -%}
 {%- endfor -%}
 adapters = [
     {{ adapters|join(",\n")|indent(4) }}
```

### Comparing `nb-cli-1.1.2/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.gitignore` & `nb-cli-1.2.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.2/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/pyproject.toml` & `nb-cli-1.2.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 version = "0.1.0"
 description = "{{ cookiecutter.computed.project_desc }}"
 readme = "README.md"
 requires-python = ">=3.8, <4.0"
 
 [tool.nonebot]
 {% set adapters = [] -%}
-{% for adapter in cookiecutter.nonebot.adapters -%}
+{% for adapter in cookiecutter.nonebot.adapters.values() -%}
 {% set name = adapter.name -%}
 {% set module_name = adapter.module_name -%}
 {% set adapter_str = '{ name = "%s", module_name = "%s" }'|format(name, module_name) -%}
 {% set _ = adapters.append(adapter_str) -%}
 {%- endfor -%}
 adapters = [
     {{ adapters|join(",\n")|indent(4) }}
```

### Comparing `nb-cli-1.1.2/nb_cli/template/scripts/project/_prepare.py.jinja` & `nb-cli-1.2.0/nb_cli/template/scripts/project/_prepare.py.jinja`

 * *Files identical despite different names*

### Comparing `nb-cli-1.1.2/pyproject.toml` & `nb-cli-1.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nb-cli"
-version = "1.1.2"
+version = "1.2.0"
 description = "CLI for nonebot2"
 authors = [
     { name = "yanyongyu", email = "yyy@nonebot.dev" },
 ]
 readme = "README.md"
 keywords = [
     "bot",
@@ -29,15 +29,15 @@
     "httpx ~=0.18",
     "jinja2 ~=3.0",
     "cashews ~=6.0",
     "wcwidth ~=0.2",
     "tomlkit ~=0.10",
     "pydantic ~=1.9",
     "watchfiles ~=0.16",
-    "cookiecutter ~=2.1",
+    "cookiecutter ~=2.2",
     "virtualenv ~=20.17.1",
     "typing-extensions ~=4.4",
     "noneprompt >=0.1.9, <1.0.0",
     "pyfiglet >=0.8.post1, <1.0.0",
     "importlib-metadata >=4.6; python_version < '3.10'",
 ]
 
@@ -59,15 +59,15 @@
     "isort ~=5.10",
     "black >=22.3.0",
     "nonemoji ~=0.1",
     "pre-commit ~=3.1",
     "importlib-metadata",
 ]
 docs = [
-    "nb-autodoc @ git+https://github.com/nonebot/nb-autodoc.git",
+    "nb-autodoc >=1.0.0a5",
 ]
 
 [tool.pdm.scripts]
 extract = "pybabel extract -o messages.pot --project nb-cli --version 1.0.0 nb_cli/"
 _init = "pybabel init -D nb-cli -i messages.pot -d nb_cli/locale/ -l {args}"
 _update = "pybabel update -D nb-cli -i messages.pot -d nb_cli/locale/"
 compile = "pybabel compile -D nb-cli -d nb_cli/locale/"
```

### Comparing `nb-cli-1.1.2/PKG-INFO` & `nb-cli-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-cli
-Version: 1.1.2
+Version: 1.2.0
 Summary: CLI for nonebot2
 License: MIT
 Keywords: bot,qq,nonebot,bot,qq,nonebot
 Author-email: yanyongyu <yyy@nonebot.dev>
 Requires-Python: >=3.8, <4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Robot Framework
@@ -59,15 +59,15 @@
 </p>
 
 <p align="center">
   <a href="https://cli.nonebot.dev/">文档</a>
   ·
   <a href="https://cli.nonebot.dev/docs/guide/installation">安装</a>
   ·
-  <a href="https://v2.nonebot.dev/">NoneBot 文档</a>
+  <a href="https://nonebot.dev/">NoneBot 文档</a>
 </p>
 
 ## 功能
 
 - 创建新的 Nonebot 项目
 - 启动 Nonebot
 - 管理插件
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_vpkajojb_/tmpkzlr0hy9_TarContainer/0/73", line 148, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_vpkajojb_/tmpkzlr0hy9_TarContainer/0/73", line 148, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nb-cli Version: 1.1.2 Summary: CLI for nonebot2
+Metadata-Version: 2.1 Name: nb-cli Version: 1.2.0 Summary: CLI for nonebot2
 License: MIT Keywords: bot,qq,nonebot,bot,qq,nonebot Author-email: yanyongyu
 nonebot.dev> Requires-Python: >=3.8, <4.0 Classifier: Development Status :: 5 -
 Production/Stable Classifier: Framework :: Robot Framework Classifier:
 Framework :: Robot Framework :: Library Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Project-URL: homepage, https://
 cli.nonebot.dev/ Project-URL: repository, https://github.com/nonebot/nb-cli
```

