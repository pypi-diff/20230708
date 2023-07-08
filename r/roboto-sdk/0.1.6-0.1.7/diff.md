# Comparing `tmp/roboto_sdk-0.1.6.tar.gz` & `tmp/roboto_sdk-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roboto_sdk-0.1.6.tar", max compression
+gzip compressed data, was "roboto_sdk-0.1.7.tar", max compression
```

## Comparing `roboto_sdk-0.1.6.tar` & `roboto_sdk-0.1.7.tar`

### file list

```diff
@@ -1,169 +1,169 @@
--rw-r--r--   0        0        0       22 2023-07-07 04:18:57.189444 roboto_sdk-0.1.6/README.md
--rw-r--r--   0        0        0      948 2023-07-07 04:20:43.065351 roboto_sdk-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       62 2023-07-07 04:18:57.193444 roboto_sdk-0.1.6/src/roboto_sdk/__init__.py
--rw-r--r--   0        0        0       48 2023-07-07 04:18:57.193444 roboto_sdk-0.1.6/src/roboto_sdk/auth/__init__.py
--rw-r--r--   0        0        0      322 2023-07-07 04:20:01.901387 roboto_sdk-0.1.6/src/roboto_sdk/auth/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3811 2023-07-07 04:20:01.901387 roboto_sdk-0.1.6/src/roboto_sdk/auth/__pycache__/pat.cpython-310.pyc
--rw-r--r--   0        0        0     4037 2023-07-07 04:18:57.193444 roboto_sdk-0.1.6/src/roboto_sdk/auth/pat.py
--rw-r--r--   0        0        0      132 2023-07-07 04:18:57.197444 roboto_sdk-0.1.6/src/roboto_sdk/cli/__init__.py
--rw-r--r--   0        0        0      111 2023-07-07 04:18:57.197444 roboto_sdk-0.1.6/src/roboto_sdk/cli/actions/__init__.py
--rw-r--r--   0        0        0      791 2023-07-07 04:18:57.197444 roboto_sdk-0.1.6/src/roboto_sdk/cli/actions/commands.py
--rw-r--r--   0        0        0     4678 2023-07-07 04:18:57.197444 roboto_sdk-0.1.6/src/roboto_sdk/cli/actions/create.py
--rw-r--r--   0        0        0     1437 2023-07-07 04:18:57.197444 roboto_sdk-0.1.6/src/roboto_sdk/cli/actions/docker_login.py
--rw-r--r--   0        0        0     3187 2023-07-07 04:18:57.197444 roboto_sdk-0.1.6/src/roboto_sdk/cli/actions/invoke.py
--rw-r--r--   0        0        0     1174 2023-07-07 04:18:57.197444 roboto_sdk-0.1.6/src/roboto_sdk/cli/actions/list_invocations.py
--rw-r--r--   0        0        0     1827 2023-07-07 04:18:57.197444 roboto_sdk-0.1.6/src/roboto_sdk/cli/actions/search.py
--rw-r--r--   0        0        0     6397 2023-07-07 04:18:57.197444 roboto_sdk-0.1.6/src/roboto_sdk/cli/actions/shared.py
--rw-r--r--   0        0        0      960 2023-07-07 04:18:57.197444 roboto_sdk-0.1.6/src/roboto_sdk/cli/actions/show.py
--rw-r--r--   0        0        0     4945 2023-07-07 04:18:57.197444 roboto_sdk-0.1.6/src/roboto_sdk/cli/actions/update.py
--rw-r--r--   0        0        0      334 2023-07-07 04:18:57.201444 roboto_sdk-0.1.6/src/roboto_sdk/cli/command/__init__.py
--rw-r--r--   0        0        0     1471 2023-07-07 04:18:57.201444 roboto_sdk-0.1.6/src/roboto_sdk/cli/command/args.py
--rw-r--r--   0        0        0     2286 2023-07-07 04:18:57.201444 roboto_sdk-0.1.6/src/roboto_sdk/cli/command/model.py
--rw-r--r--   0        0        0      891 2023-07-07 04:18:57.201444 roboto_sdk-0.1.6/src/roboto_sdk/cli/context.py
--rw-r--r--   0        0        0      110 2023-07-07 04:18:57.201444 roboto_sdk-0.1.6/src/roboto_sdk/cli/datasets/__init__.py
--rw-r--r--   0        0        0     6741 2023-07-07 04:18:57.201444 roboto_sdk-0.1.6/src/roboto_sdk/cli/datasets/commands.py
--rw-r--r--   0        0        0     4025 2023-07-07 04:18:57.201444 roboto_sdk-0.1.6/src/roboto_sdk/cli/entry.py
--rw-r--r--   0        0        0      108 2023-07-07 04:18:57.205444 roboto_sdk-0.1.6/src/roboto_sdk/cli/help/__init__.py
--rw-r--r--   0        0        0      167 2023-07-07 04:18:57.205444 roboto_sdk-0.1.6/src/roboto_sdk/cli/help/args.py
--rw-r--r--   0        0        0      322 2023-07-07 04:18:57.205444 roboto_sdk-0.1.6/src/roboto_sdk/cli/invocations/__init__.py
--rw-r--r--   0        0        0     1967 2023-07-07 04:18:57.205444 roboto_sdk-0.1.6/src/roboto_sdk/cli/invocations/status.py
--rw-r--r--   0        0        0      110 2023-07-07 04:18:57.205444 roboto_sdk-0.1.6/src/roboto_sdk/cli/orgs/__init__.py
--rw-r--r--   0        0        0     8083 2023-07-07 04:18:57.205444 roboto_sdk-0.1.6/src/roboto_sdk/cli/orgs/commands.py
--rw-r--r--   0        0        0      110 2023-07-07 04:18:57.209444 roboto_sdk-0.1.6/src/roboto_sdk/cli/tokens/__init__.py
--rw-r--r--   0        0        0     3291 2023-07-07 04:18:57.209444 roboto_sdk-0.1.6/src/roboto_sdk/cli/tokens/commands.py
--rw-r--r--   0        0        0      110 2023-07-07 04:18:57.209444 roboto_sdk-0.1.6/src/roboto_sdk/cli/triggers/__init__.py
--rw-r--r--   0        0        0     2876 2023-07-07 04:18:57.209444 roboto_sdk-0.1.6/src/roboto_sdk/cli/triggers/commands.py
--rw-r--r--   0        0        0      110 2023-07-07 04:18:57.213444 roboto_sdk-0.1.6/src/roboto_sdk/cli/users/__init__.py
--rw-r--r--   0        0        0      733 2023-07-07 04:18:57.213444 roboto_sdk-0.1.6/src/roboto_sdk/cli/users/commands.py
--rw-r--r--   0        0        0      120 2023-07-07 04:18:57.213444 roboto_sdk-0.1.6/src/roboto_sdk/domain/__init__.py
--rw-r--r--   0        0        0      398 2023-07-07 04:20:01.541387 roboto_sdk-0.1.6/src/roboto_sdk/domain/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1849 2023-07-07 04:20:01.541387 roboto_sdk-0.1.6/src/roboto_sdk/domain/__pycache__/http_delegates.cpython-310.pyc
--rw-r--r--   0        0        0     1877 2023-07-07 04:18:57.213444 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__init__.py
--rw-r--r--   0        0        0     1682 2023-07-07 04:20:01.937387 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     7230 2023-07-07 04:20:01.937387 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/action.cpython-310.pyc
--rw-r--r--   0        0        0     3263 2023-07-07 04:20:01.941387 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/action_container_resources.cpython-310.pyc
--rw-r--r--   0        0        0     3263 2023-07-07 04:20:01.945387 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/action_delegate.cpython-310.pyc
--rw-r--r--   0        0        0     5468 2023-07-07 04:20:01.957387 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/action_http_delegate.cpython-310.pyc
--rw-r--r--   0        0        0     1583 2023-07-07 04:20:01.957387 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/action_http_resources.cpython-310.pyc
--rw-r--r--   0        0        0     1336 2023-07-07 04:20:01.945387 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/action_record.cpython-310.pyc
--rw-r--r--   0        0        0      636 2023-07-07 04:20:01.961387 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/error.cpython-310.pyc
--rw-r--r--   0        0        0     5231 2023-07-07 04:20:01.949386 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/invocation.cpython-310.pyc
--rw-r--r--   0        0        0     2517 2023-07-07 04:20:01.949386 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/invocation_delegate.cpython-310.pyc
--rw-r--r--   0        0        0     4924 2023-07-07 04:20:01.961387 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/invocation_http_delegate.cpython-310.pyc
--rw-r--r--   0        0        0     1484 2023-07-07 04:20:01.961387 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/invocation_http_resources.cpython-310.pyc
--rw-r--r--   0        0        0     2519 2023-07-07 04:20:01.949386 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/invocation_record.cpython-310.pyc
--rw-r--r--   0        0        0     8680 2023-07-07 04:18:57.213444 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/action.py
--rw-r--r--   0        0        0     2685 2023-07-07 04:18:57.213444 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/action_container_resources.py
--rw-r--r--   0        0        0     2875 2023-07-07 04:18:57.213444 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/action_delegate.py
--rw-r--r--   0        0        0     5629 2023-07-07 04:18:57.213444 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/action_http_delegate.py
--rw-r--r--   0        0        0      860 2023-07-07 04:18:57.213444 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/action_http_resources.py
--rw-r--r--   0        0        0      988 2023-07-07 04:18:57.213444 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/action_record.py
--rw-r--r--   0        0        0      106 2023-07-07 04:18:57.213444 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/error.py
--rw-r--r--   0        0        0     4836 2023-07-07 04:18:57.213444 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/invocation.py
--rw-r--r--   0        0        0     1939 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/invocation_delegate.py
--rw-r--r--   0        0        0     5108 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/invocation_http_delegate.py
--rw-r--r--   0        0        0      752 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/invocation_http_resources.py
--rw-r--r--   0        0        0     1839 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/invocation_record.py
--rw-r--r--   0        0        0      546 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/__init__.py
--rw-r--r--   0        0        0      735 2023-07-07 04:20:01.965386 roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     7622 2023-07-07 04:20:01.965386 roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/__pycache__/dataset.cpython-310.pyc
--rw-r--r--   0        0        0     3184 2023-07-07 04:20:01.973386 roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/__pycache__/delegate.cpython-310.pyc
--rw-r--r--   0        0        0     5064 2023-07-07 04:20:01.981387 roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/__pycache__/http_delegate.cpython-310.pyc
--rw-r--r--   0        0        0      867 2023-07-07 04:20:01.981387 roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/__pycache__/http_resources.cpython-310.pyc
--rw-r--r--   0        0        0     1263 2023-07-07 04:20:01.977387 roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/__pycache__/record.cpython-310.pyc
--rw-r--r--   0        0        0    10221 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/dataset.py
--rw-r--r--   0        0        0     2215 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/delegate.py
--rw-r--r--   0        0        0     4911 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/http_delegate.py
--rw-r--r--   0        0        0      340 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/http_resources.py
--rw-r--r--   0        0        0      867 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/record.py
--rw-r--r--   0        0        0      436 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/files/__init__.py
--rw-r--r--   0        0        0      712 2023-07-07 04:20:01.969386 roboto_sdk-0.1.6/src/roboto_sdk/domain/files/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1916 2023-07-07 04:20:01.969386 roboto_sdk-0.1.6/src/roboto_sdk/domain/files/__pycache__/delegate.cpython-310.pyc
--rw-r--r--   0        0        0     1536 2023-07-07 04:20:01.973386 roboto_sdk-0.1.6/src/roboto_sdk/domain/files/__pycache__/file.cpython-310.pyc
--rw-r--r--   0        0        0     2835 2023-07-07 04:20:01.973386 roboto_sdk-0.1.6/src/roboto_sdk/domain/files/__pycache__/http_delegate.cpython-310.pyc
--rw-r--r--   0        0        0      723 2023-07-07 04:20:01.973386 roboto_sdk-0.1.6/src/roboto_sdk/domain/files/__pycache__/http_resources.cpython-310.pyc
--rw-r--r--   0        0        0      696 2023-07-07 04:20:01.969386 roboto_sdk-0.1.6/src/roboto_sdk/domain/files/__pycache__/record.cpython-310.pyc
--rw-r--r--   0        0        0     3232 2023-07-07 04:20:01.973386 roboto_sdk-0.1.6/src/roboto_sdk/domain/files/__pycache__/s3_delegate.cpython-310.pyc
--rw-r--r--   0        0        0     1181 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/files/delegate.py
--rw-r--r--   0        0        0      802 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/files/file.py
--rw-r--r--   0        0        0     2166 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/files/http_delegate.py
--rw-r--r--   0        0        0      168 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/files/http_resources.py
--rw-r--r--   0        0        0      382 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/files/record.py
--rw-r--r--   0        0        0     2358 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/files/s3_delegate.py
--rw-r--r--   0        0        0     1974 2023-07-07 04:18:57.217444 roboto_sdk-0.1.6/src/roboto_sdk/domain/http_delegates.py
--rw-r--r--   0        0        0      852 2023-07-07 04:18:57.221444 roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/__init__.py
--rw-r--r--   0        0        0      976 2023-07-07 04:20:01.981387 roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3586 2023-07-07 04:20:01.981387 roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/__pycache__/delegate.cpython-310.pyc
--rw-r--r--   0        0        0     6907 2023-07-07 04:20:01.989386 roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/__pycache__/http_delegate.cpython-310.pyc
--rw-r--r--   0        0        0     1378 2023-07-07 04:20:01.989386 roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/__pycache__/http_resources.cpython-310.pyc
--rw-r--r--   0        0        0     4106 2023-07-07 04:20:01.993386 roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/__pycache__/org.cpython-310.pyc
--rw-r--r--   0        0        0     2331 2023-07-07 04:20:01.993386 roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/__pycache__/org_invite.cpython-310.pyc
--rw-r--r--   0        0        0     2671 2023-07-07 04:20:01.993386 roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/__pycache__/org_role.cpython-310.pyc
--rw-r--r--   0        0        0     1709 2023-07-07 04:20:01.981387 roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/__pycache__/record.cpython-310.pyc
--rw-r--r--   0        0        0     2856 2023-07-07 04:18:57.221444 roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/delegate.py
--rw-r--r--   0        0        0     6889 2023-07-07 04:18:57.221444 roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/http_delegate.py
--rw-r--r--   0        0        0      540 2023-07-07 04:18:57.221444 roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/http_resources.py
--rw-r--r--   0        0        0     3344 2023-07-07 04:18:57.221444 roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/org.py
--rw-r--r--   0        0        0     1768 2023-07-07 04:18:57.221444 roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/org_invite.py
--rw-r--r--   0        0        0     1751 2023-07-07 04:18:57.221444 roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/org_role.py
--rw-r--r--   0        0        0      726 2023-07-07 04:18:57.221444 roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/record.py
--rw-r--r--   0        0        0      387 2023-07-07 04:18:57.221444 roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/__init__.py
--rw-r--r--   0        0        0      640 2023-07-07 04:20:01.993386 roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1616 2023-07-07 04:20:01.993386 roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/__pycache__/delegate.cpython-310.pyc
--rw-r--r--   0        0        0     2697 2023-07-07 04:20:01.997387 roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/__pycache__/http_delegate.cpython-310.pyc
--rw-r--r--   0        0        0      685 2023-07-07 04:20:01.997387 roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/__pycache__/http_resources.cpython-310.pyc
--rw-r--r--   0        0        0     1003 2023-07-07 04:20:01.993386 roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/__pycache__/record.cpython-310.pyc
--rw-r--r--   0        0        0     2528 2023-07-07 04:20:01.997387 roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/__pycache__/token.cpython-310.pyc
--rw-r--r--   0        0        0      888 2023-07-07 04:18:57.221444 roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/delegate.py
--rw-r--r--   0        0        0     2038 2023-07-07 04:18:57.221444 roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/http_delegate.py
--rw-r--r--   0        0        0      216 2023-07-07 04:18:57.221444 roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/http_resources.py
--rw-r--r--   0        0        0      455 2023-07-07 04:18:57.221444 roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/record.py
--rw-r--r--   0        0        0     1826 2023-07-07 04:18:57.221444 roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/token.py
--rw-r--r--   0        0        0      391 2023-07-07 04:18:57.225444 roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/__init__.py
--rw-r--r--   0        0        0      642 2023-07-07 04:20:02.001387 roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2758 2023-07-07 04:20:02.001387 roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/__pycache__/http_delegate.cpython-310.pyc
--rw-r--r--   0        0        0      657 2023-07-07 04:20:02.001387 roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/__pycache__/http_resources.cpython-310.pyc
--rw-r--r--   0        0        0     2392 2023-07-07 04:20:02.005386 roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/__pycache__/trigger.cpython-310.pyc
--rw-r--r--   0        0        0     1488 2023-07-07 04:20:02.001387 roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/__pycache__/trigger_delegate.cpython-310.pyc
--rw-r--r--   0        0        0      617 2023-07-07 04:20:02.001387 roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/__pycache__/trigger_record.cpython-310.pyc
--rw-r--r--   0        0        0     2280 2023-07-07 04:18:57.225444 roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/http_delegate.py
--rw-r--r--   0        0        0      205 2023-07-07 04:18:57.225444 roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/http_resources.py
--rw-r--r--   0        0        0     2685 2023-07-07 04:18:57.225444 roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/trigger.py
--rw-r--r--   0        0        0      882 2023-07-07 04:18:57.225444 roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/trigger_delegate.py
--rw-r--r--   0        0        0      249 2023-07-07 04:18:57.225444 roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/trigger_record.py
--rw-r--r--   0        0        0      262 2023-07-07 04:18:57.225444 roboto_sdk-0.1.6/src/roboto_sdk/domain/users/__init__.py
--rw-r--r--   0        0        0      554 2023-07-07 04:20:01.981387 roboto_sdk-0.1.6/src/roboto_sdk/domain/users/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1617 2023-07-07 04:20:01.985386 roboto_sdk-0.1.6/src/roboto_sdk/domain/users/__pycache__/http_delegate.cpython-310.pyc
--rw-r--r--   0        0        0     2213 2023-07-07 04:20:01.985386 roboto_sdk-0.1.6/src/roboto_sdk/domain/users/__pycache__/user.cpython-310.pyc
--rw-r--r--   0        0        0     1172 2023-07-07 04:20:01.985386 roboto_sdk-0.1.6/src/roboto_sdk/domain/users/__pycache__/user_delegate.cpython-310.pyc
--rw-r--r--   0        0        0      723 2023-07-07 04:20:01.985386 roboto_sdk-0.1.6/src/roboto_sdk/domain/users/__pycache__/user_record.cpython-310.pyc
--rw-r--r--   0        0        0     1051 2023-07-07 04:18:57.225444 roboto_sdk-0.1.6/src/roboto_sdk/domain/users/http_delegate.py
--rw-r--r--   0        0        0     1408 2023-07-07 04:18:57.225444 roboto_sdk-0.1.6/src/roboto_sdk/domain/users/user.py
--rw-r--r--   0        0        0      485 2023-07-07 04:18:57.225444 roboto_sdk-0.1.6/src/roboto_sdk/domain/users/user_delegate.py
--rw-r--r--   0        0        0      257 2023-07-07 04:18:57.225444 roboto_sdk-0.1.6/src/roboto_sdk/domain/users/user_record.py
--rw-r--r--   0        0        0      285 2023-07-07 04:18:57.229444 roboto_sdk-0.1.6/src/roboto_sdk/exceptions/__init__.py
--rw-r--r--   0        0        0      506 2023-07-07 04:20:01.957387 roboto_sdk-0.1.6/src/roboto_sdk/exceptions/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2105 2023-07-07 04:20:01.957387 roboto_sdk-0.1.6/src/roboto_sdk/exceptions/__pycache__/domain.cpython-310.pyc
--rw-r--r--   0        0        0     1266 2023-07-07 04:18:57.229444 roboto_sdk-0.1.6/src/roboto_sdk/exceptions/domain.py
--rw-r--r--   0        0        0      782 2023-07-07 04:18:57.229444 roboto_sdk-0.1.6/src/roboto_sdk/http/__init__.py
--rw-r--r--   0        0        0      902 2023-07-07 04:20:01.541387 roboto_sdk-0.1.6/src/roboto_sdk/http/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      500 2023-07-07 04:20:01.545387 roboto_sdk-0.1.6/src/roboto_sdk/http/__pycache__/constants.cpython-310.pyc
--rw-r--r--   0        0        0      688 2023-07-07 04:20:01.545387 roboto_sdk-0.1.6/src/roboto_sdk/http/__pycache__/headers.cpython-310.pyc
--rw-r--r--   0        0        0     9636 2023-07-07 04:20:01.545387 roboto_sdk-0.1.6/src/roboto_sdk/http/__pycache__/http_client.cpython-310.pyc
--rw-r--r--   0        0        0     3963 2023-07-07 04:20:01.585387 roboto_sdk-0.1.6/src/roboto_sdk/http/__pycache__/request_decorators.cpython-310.pyc
--rw-r--r--   0        0        0     1666 2023-07-07 04:20:01.937387 roboto_sdk-0.1.6/src/roboto_sdk/http/__pycache__/testing_util.cpython-310.pyc
--rw-r--r--   0        0        0      216 2023-07-07 04:18:57.229444 roboto_sdk-0.1.6/src/roboto_sdk/http/constants.py
--rw-r--r--   0        0        0      443 2023-07-07 04:18:57.229444 roboto_sdk-0.1.6/src/roboto_sdk/http/headers.py
--rw-r--r--   0        0        0     9060 2023-07-07 04:18:57.229444 roboto_sdk-0.1.6/src/roboto_sdk/http/http_client.py
--rw-r--r--   0        0        0     3161 2023-07-07 04:18:57.229444 roboto_sdk-0.1.6/src/roboto_sdk/http/request_decorators.py
--rw-r--r--   0        0        0     1004 2023-07-07 04:18:57.229444 roboto_sdk-0.1.6/src/roboto_sdk/http/testing_util.py
--rw-r--r--   0        0        0      158 2023-07-07 04:18:57.229444 roboto_sdk-0.1.6/src/roboto_sdk/logging.py
--rw-r--r--   0        0        0      224 2023-07-07 04:18:57.229444 roboto_sdk-0.1.6/src/roboto_sdk/pagination.py
--rw-r--r--   0        0        0      168 2023-07-07 04:18:57.233444 roboto_sdk-0.1.6/src/roboto_sdk/profile/__init__.py
--rw-r--r--   0        0        0      428 2023-07-07 04:20:01.933386 roboto_sdk-0.1.6/src/roboto_sdk/profile/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2991 2023-07-07 04:20:01.933386 roboto_sdk-0.1.6/src/roboto_sdk/profile/__pycache__/profile.cpython-310.pyc
--rw-r--r--   0        0        0     2977 2023-07-07 04:18:57.233444 roboto_sdk-0.1.6/src/roboto_sdk/profile/profile.py
--rw-r--r--   0        0        0        0 2023-07-07 04:18:57.233444 roboto_sdk-0.1.6/src/roboto_sdk/py.typed
--rw-r--r--   0        0        0     1250 2023-07-07 04:18:57.233444 roboto_sdk-0.1.6/src/roboto_sdk/serde.py
--rw-r--r--   0        0        0      112 2023-07-07 04:18:57.233444 roboto_sdk-0.1.6/src/roboto_sdk/time.py
--rw-r--r--   0        0        0      691 1970-01-01 00:00:00.000000 roboto_sdk-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-07-08 17:50:26.458340 roboto_sdk-0.1.7/README.md
+-rw-r--r--   0        0        0      948 2023-07-08 17:52:13.290404 roboto_sdk-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-07-08 17:50:26.462340 roboto_sdk-0.1.7/src/roboto_sdk/__init__.py
+-rw-r--r--   0        0        0       48 2023-07-08 17:50:26.462340 roboto_sdk-0.1.7/src/roboto_sdk/auth/__init__.py
+-rw-r--r--   0        0        0      322 2023-07-08 17:51:37.026384 roboto_sdk-0.1.7/src/roboto_sdk/auth/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3811 2023-07-08 17:51:37.030384 roboto_sdk-0.1.7/src/roboto_sdk/auth/__pycache__/pat.cpython-310.pyc
+-rw-r--r--   0        0        0     4037 2023-07-08 17:50:26.462340 roboto_sdk-0.1.7/src/roboto_sdk/auth/pat.py
+-rw-r--r--   0        0        0      132 2023-07-08 17:50:26.466340 roboto_sdk-0.1.7/src/roboto_sdk/cli/__init__.py
+-rw-r--r--   0        0        0      111 2023-07-08 17:50:26.470340 roboto_sdk-0.1.7/src/roboto_sdk/cli/actions/__init__.py
+-rw-r--r--   0        0        0      791 2023-07-08 17:50:26.470340 roboto_sdk-0.1.7/src/roboto_sdk/cli/actions/commands.py
+-rw-r--r--   0        0        0     4678 2023-07-08 17:50:26.470340 roboto_sdk-0.1.7/src/roboto_sdk/cli/actions/create.py
+-rw-r--r--   0        0        0     1437 2023-07-08 17:50:26.470340 roboto_sdk-0.1.7/src/roboto_sdk/cli/actions/docker_login.py
+-rw-r--r--   0        0        0     3187 2023-07-08 17:50:26.470340 roboto_sdk-0.1.7/src/roboto_sdk/cli/actions/invoke.py
+-rw-r--r--   0        0        0     1174 2023-07-08 17:50:26.470340 roboto_sdk-0.1.7/src/roboto_sdk/cli/actions/list_invocations.py
+-rw-r--r--   0        0        0     1827 2023-07-08 17:50:26.470340 roboto_sdk-0.1.7/src/roboto_sdk/cli/actions/search.py
+-rw-r--r--   0        0        0     6397 2023-07-08 17:50:26.470340 roboto_sdk-0.1.7/src/roboto_sdk/cli/actions/shared.py
+-rw-r--r--   0        0        0      960 2023-07-08 17:50:26.470340 roboto_sdk-0.1.7/src/roboto_sdk/cli/actions/show.py
+-rw-r--r--   0        0        0     4945 2023-07-08 17:50:26.470340 roboto_sdk-0.1.7/src/roboto_sdk/cli/actions/update.py
+-rw-r--r--   0        0        0      334 2023-07-08 17:50:26.470340 roboto_sdk-0.1.7/src/roboto_sdk/cli/command/__init__.py
+-rw-r--r--   0        0        0     1471 2023-07-08 17:50:26.470340 roboto_sdk-0.1.7/src/roboto_sdk/cli/command/args.py
+-rw-r--r--   0        0        0     2286 2023-07-08 17:50:26.470340 roboto_sdk-0.1.7/src/roboto_sdk/cli/command/model.py
+-rw-r--r--   0        0        0      955 2023-07-08 17:50:26.470340 roboto_sdk-0.1.7/src/roboto_sdk/cli/context.py
+-rw-r--r--   0        0        0      110 2023-07-08 17:50:26.474340 roboto_sdk-0.1.7/src/roboto_sdk/cli/datasets/__init__.py
+-rw-r--r--   0        0        0     6741 2023-07-08 17:50:26.474340 roboto_sdk-0.1.7/src/roboto_sdk/cli/datasets/commands.py
+-rw-r--r--   0        0        0     4124 2023-07-08 17:50:26.474340 roboto_sdk-0.1.7/src/roboto_sdk/cli/entry.py
+-rw-r--r--   0        0        0      108 2023-07-08 17:50:26.474340 roboto_sdk-0.1.7/src/roboto_sdk/cli/help/__init__.py
+-rw-r--r--   0        0        0      167 2023-07-08 17:50:26.474340 roboto_sdk-0.1.7/src/roboto_sdk/cli/help/args.py
+-rw-r--r--   0        0        0      322 2023-07-08 17:50:26.478340 roboto_sdk-0.1.7/src/roboto_sdk/cli/invocations/__init__.py
+-rw-r--r--   0        0        0     1967 2023-07-08 17:50:26.478340 roboto_sdk-0.1.7/src/roboto_sdk/cli/invocations/status.py
+-rw-r--r--   0        0        0      110 2023-07-08 17:50:26.478340 roboto_sdk-0.1.7/src/roboto_sdk/cli/orgs/__init__.py
+-rw-r--r--   0        0        0     8263 2023-07-08 17:50:26.478340 roboto_sdk-0.1.7/src/roboto_sdk/cli/orgs/commands.py
+-rw-r--r--   0        0        0      110 2023-07-08 17:50:26.482340 roboto_sdk-0.1.7/src/roboto_sdk/cli/tokens/__init__.py
+-rw-r--r--   0        0        0     3271 2023-07-08 17:50:26.482340 roboto_sdk-0.1.7/src/roboto_sdk/cli/tokens/commands.py
+-rw-r--r--   0        0        0      110 2023-07-08 17:50:26.482340 roboto_sdk-0.1.7/src/roboto_sdk/cli/triggers/__init__.py
+-rw-r--r--   0        0        0     2876 2023-07-08 17:50:26.482340 roboto_sdk-0.1.7/src/roboto_sdk/cli/triggers/commands.py
+-rw-r--r--   0        0        0      110 2023-07-08 17:50:26.486340 roboto_sdk-0.1.7/src/roboto_sdk/cli/users/__init__.py
+-rw-r--r--   0        0        0     3154 2023-07-08 17:50:26.486340 roboto_sdk-0.1.7/src/roboto_sdk/cli/users/commands.py
+-rw-r--r--   0        0        0      120 2023-07-08 17:50:26.486340 roboto_sdk-0.1.7/src/roboto_sdk/domain/__init__.py
+-rw-r--r--   0        0        0      398 2023-07-08 17:51:36.662384 roboto_sdk-0.1.7/src/roboto_sdk/domain/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1849 2023-07-08 17:51:36.666384 roboto_sdk-0.1.7/src/roboto_sdk/domain/__pycache__/http_delegates.cpython-310.pyc
+-rw-r--r--   0        0        0     1877 2023-07-08 17:50:26.490340 roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/__init__.py
+-rw-r--r--   0        0        0     1682 2023-07-08 17:51:37.066384 roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     7230 2023-07-08 17:51:37.066384 roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/__pycache__/action.cpython-310.pyc
+-rw-r--r--   0        0        0     3263 2023-07-08 17:51:37.066384 roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/__pycache__/action_container_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     3263 2023-07-08 17:51:37.070384 roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/__pycache__/action_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     5466 2023-07-08 17:51:37.082384 roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/__pycache__/action_http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     1583 2023-07-08 17:51:37.082384 roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/__pycache__/action_http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     1336 2023-07-08 17:51:37.074384 roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/__pycache__/action_record.cpython-310.pyc
+-rw-r--r--   0        0        0      636 2023-07-08 17:51:37.086384 roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/__pycache__/error.cpython-310.pyc
+-rw-r--r--   0        0        0     5231 2023-07-08 17:51:37.074384 roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/__pycache__/invocation.cpython-310.pyc
+-rw-r--r--   0        0        0     2517 2023-07-08 17:51:37.078384 roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/__pycache__/invocation_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     4922 2023-07-08 17:51:37.086384 roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/__pycache__/invocation_http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     1484 2023-07-08 17:51:37.086384 roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/__pycache__/invocation_http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     2519 2023-07-08 17:51:37.078384 roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/__pycache__/invocation_record.cpython-310.pyc
+-rw-r--r--   0        0        0     8680 2023-07-08 17:50:26.490340 roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/action.py
+-rw-r--r--   0        0        0     2685 2023-07-08 17:50:26.490340 roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/action_container_resources.py
+-rw-r--r--   0        0        0     2875 2023-07-08 17:50:26.490340 roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/action_delegate.py
+-rw-r--r--   0        0        0     5627 2023-07-08 17:50:26.490340 roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/action_http_delegate.py
+-rw-r--r--   0        0        0      860 2023-07-08 17:50:26.490340 roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/action_http_resources.py
+-rw-r--r--   0        0        0      988 2023-07-08 17:50:26.490340 roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/action_record.py
+-rw-r--r--   0        0        0      106 2023-07-08 17:50:26.490340 roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/error.py
+-rw-r--r--   0        0        0     4836 2023-07-08 17:50:26.490340 roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/invocation.py
+-rw-r--r--   0        0        0     1939 2023-07-08 17:50:26.490340 roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/invocation_delegate.py
+-rw-r--r--   0        0        0     5106 2023-07-08 17:50:26.490340 roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/invocation_http_delegate.py
+-rw-r--r--   0        0        0      752 2023-07-08 17:50:26.490340 roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/invocation_http_resources.py
+-rw-r--r--   0        0        0     1839 2023-07-08 17:50:26.490340 roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/invocation_record.py
+-rw-r--r--   0        0        0      546 2023-07-08 17:50:26.490340 roboto_sdk-0.1.7/src/roboto_sdk/domain/datasets/__init__.py
+-rw-r--r--   0        0        0      735 2023-07-08 17:51:37.090384 roboto_sdk-0.1.7/src/roboto_sdk/domain/datasets/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     7770 2023-07-08 17:51:37.090384 roboto_sdk-0.1.7/src/roboto_sdk/domain/datasets/__pycache__/dataset.cpython-310.pyc
+-rw-r--r--   0        0        0     3184 2023-07-08 17:51:37.102384 roboto_sdk-0.1.7/src/roboto_sdk/domain/datasets/__pycache__/delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     5064 2023-07-08 17:51:37.106384 roboto_sdk-0.1.7/src/roboto_sdk/domain/datasets/__pycache__/http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0      867 2023-07-08 17:51:37.106384 roboto_sdk-0.1.7/src/roboto_sdk/domain/datasets/__pycache__/http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     1263 2023-07-08 17:51:37.102384 roboto_sdk-0.1.7/src/roboto_sdk/domain/datasets/__pycache__/record.cpython-310.pyc
+-rw-r--r--   0        0        0    10309 2023-07-08 17:50:26.490340 roboto_sdk-0.1.7/src/roboto_sdk/domain/datasets/dataset.py
+-rw-r--r--   0        0        0     2215 2023-07-08 17:50:26.490340 roboto_sdk-0.1.7/src/roboto_sdk/domain/datasets/delegate.py
+-rw-r--r--   0        0        0     4911 2023-07-08 17:50:26.490340 roboto_sdk-0.1.7/src/roboto_sdk/domain/datasets/http_delegate.py
+-rw-r--r--   0        0        0      340 2023-07-08 17:50:26.490340 roboto_sdk-0.1.7/src/roboto_sdk/domain/datasets/http_resources.py
+-rw-r--r--   0        0        0      867 2023-07-08 17:50:26.490340 roboto_sdk-0.1.7/src/roboto_sdk/domain/datasets/record.py
+-rw-r--r--   0        0        0      436 2023-07-08 17:50:26.494340 roboto_sdk-0.1.7/src/roboto_sdk/domain/files/__init__.py
+-rw-r--r--   0        0        0      712 2023-07-08 17:51:37.098384 roboto_sdk-0.1.7/src/roboto_sdk/domain/files/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1916 2023-07-08 17:51:37.098384 roboto_sdk-0.1.7/src/roboto_sdk/domain/files/__pycache__/delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     1536 2023-07-08 17:51:37.098384 roboto_sdk-0.1.7/src/roboto_sdk/domain/files/__pycache__/file.cpython-310.pyc
+-rw-r--r--   0        0        0     2835 2023-07-08 17:51:37.098384 roboto_sdk-0.1.7/src/roboto_sdk/domain/files/__pycache__/http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0      723 2023-07-08 17:51:37.102384 roboto_sdk-0.1.7/src/roboto_sdk/domain/files/__pycache__/http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0      696 2023-07-08 17:51:37.098384 roboto_sdk-0.1.7/src/roboto_sdk/domain/files/__pycache__/record.cpython-310.pyc
+-rw-r--r--   0        0        0     3232 2023-07-08 17:51:37.102384 roboto_sdk-0.1.7/src/roboto_sdk/domain/files/__pycache__/s3_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     1181 2023-07-08 17:50:26.494340 roboto_sdk-0.1.7/src/roboto_sdk/domain/files/delegate.py
+-rw-r--r--   0        0        0      802 2023-07-08 17:50:26.494340 roboto_sdk-0.1.7/src/roboto_sdk/domain/files/file.py
+-rw-r--r--   0        0        0     2166 2023-07-08 17:50:26.494340 roboto_sdk-0.1.7/src/roboto_sdk/domain/files/http_delegate.py
+-rw-r--r--   0        0        0      168 2023-07-08 17:50:26.494340 roboto_sdk-0.1.7/src/roboto_sdk/domain/files/http_resources.py
+-rw-r--r--   0        0        0      382 2023-07-08 17:50:26.494340 roboto_sdk-0.1.7/src/roboto_sdk/domain/files/record.py
+-rw-r--r--   0        0        0     2358 2023-07-08 17:50:26.494340 roboto_sdk-0.1.7/src/roboto_sdk/domain/files/s3_delegate.py
+-rw-r--r--   0        0        0     1974 2023-07-08 17:50:26.494340 roboto_sdk-0.1.7/src/roboto_sdk/domain/http_delegates.py
+-rw-r--r--   0        0        0      852 2023-07-08 17:50:26.494340 roboto_sdk-0.1.7/src/roboto_sdk/domain/orgs/__init__.py
+-rw-r--r--   0        0        0      976 2023-07-08 17:51:37.110384 roboto_sdk-0.1.7/src/roboto_sdk/domain/orgs/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3767 2023-07-08 17:51:37.110384 roboto_sdk-0.1.7/src/roboto_sdk/domain/orgs/__pycache__/delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     7346 2023-07-08 17:51:37.118384 roboto_sdk-0.1.7/src/roboto_sdk/domain/orgs/__pycache__/http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     1378 2023-07-08 17:51:37.118384 roboto_sdk-0.1.7/src/roboto_sdk/domain/orgs/__pycache__/http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     4106 2023-07-08 17:51:37.118384 roboto_sdk-0.1.7/src/roboto_sdk/domain/orgs/__pycache__/org.cpython-310.pyc
+-rw-r--r--   0        0        0     2736 2023-07-08 17:51:37.122384 roboto_sdk-0.1.7/src/roboto_sdk/domain/orgs/__pycache__/org_invite.cpython-310.pyc
+-rw-r--r--   0        0        0     2671 2023-07-08 17:51:37.122384 roboto_sdk-0.1.7/src/roboto_sdk/domain/orgs/__pycache__/org_role.cpython-310.pyc
+-rw-r--r--   0        0        0     1709 2023-07-08 17:51:37.110384 roboto_sdk-0.1.7/src/roboto_sdk/domain/orgs/__pycache__/record.cpython-310.pyc
+-rw-r--r--   0        0        0     3042 2023-07-08 17:50:26.494340 roboto_sdk-0.1.7/src/roboto_sdk/domain/orgs/delegate.py
+-rw-r--r--   0        0        0     7541 2023-07-08 17:50:26.494340 roboto_sdk-0.1.7/src/roboto_sdk/domain/orgs/http_delegate.py
+-rw-r--r--   0        0        0      540 2023-07-08 17:50:26.494340 roboto_sdk-0.1.7/src/roboto_sdk/domain/orgs/http_resources.py
+-rw-r--r--   0        0        0     3344 2023-07-08 17:50:26.494340 roboto_sdk-0.1.7/src/roboto_sdk/domain/orgs/org.py
+-rw-r--r--   0        0        0     2051 2023-07-08 17:50:26.494340 roboto_sdk-0.1.7/src/roboto_sdk/domain/orgs/org_invite.py
+-rw-r--r--   0        0        0     1751 2023-07-08 17:50:26.494340 roboto_sdk-0.1.7/src/roboto_sdk/domain/orgs/org_role.py
+-rw-r--r--   0        0        0      726 2023-07-08 17:50:26.494340 roboto_sdk-0.1.7/src/roboto_sdk/domain/orgs/record.py
+-rw-r--r--   0        0        0      387 2023-07-08 17:50:26.498340 roboto_sdk-0.1.7/src/roboto_sdk/domain/tokens/__init__.py
+-rw-r--r--   0        0        0      640 2023-07-08 17:51:37.122384 roboto_sdk-0.1.7/src/roboto_sdk/domain/tokens/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1637 2023-07-08 17:51:37.122384 roboto_sdk-0.1.7/src/roboto_sdk/domain/tokens/__pycache__/delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     2980 2023-07-08 17:51:37.126384 roboto_sdk-0.1.7/src/roboto_sdk/domain/tokens/__pycache__/http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0      685 2023-07-08 17:51:37.126384 roboto_sdk-0.1.7/src/roboto_sdk/domain/tokens/__pycache__/http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     1003 2023-07-08 17:51:37.122384 roboto_sdk-0.1.7/src/roboto_sdk/domain/tokens/__pycache__/record.cpython-310.pyc
+-rw-r--r--   0        0        0     2760 2023-07-08 17:51:37.126384 roboto_sdk-0.1.7/src/roboto_sdk/domain/tokens/__pycache__/token.cpython-310.pyc
+-rw-r--r--   0        0        0      909 2023-07-08 17:50:26.498340 roboto_sdk-0.1.7/src/roboto_sdk/domain/tokens/delegate.py
+-rw-r--r--   0        0        0     2254 2023-07-08 17:50:26.498340 roboto_sdk-0.1.7/src/roboto_sdk/domain/tokens/http_delegate.py
+-rw-r--r--   0        0        0      216 2023-07-08 17:50:26.498340 roboto_sdk-0.1.7/src/roboto_sdk/domain/tokens/http_resources.py
+-rw-r--r--   0        0        0      455 2023-07-08 17:50:26.498340 roboto_sdk-0.1.7/src/roboto_sdk/domain/tokens/record.py
+-rw-r--r--   0        0        0     2047 2023-07-08 17:50:26.498340 roboto_sdk-0.1.7/src/roboto_sdk/domain/tokens/token.py
+-rw-r--r--   0        0        0      391 2023-07-08 17:50:26.498340 roboto_sdk-0.1.7/src/roboto_sdk/domain/triggers/__init__.py
+-rw-r--r--   0        0        0      642 2023-07-08 17:51:37.126384 roboto_sdk-0.1.7/src/roboto_sdk/domain/triggers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2758 2023-07-08 17:51:37.126384 roboto_sdk-0.1.7/src/roboto_sdk/domain/triggers/__pycache__/http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0      657 2023-07-08 17:51:37.126384 roboto_sdk-0.1.7/src/roboto_sdk/domain/triggers/__pycache__/http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     2392 2023-07-08 17:51:37.130385 roboto_sdk-0.1.7/src/roboto_sdk/domain/triggers/__pycache__/trigger.cpython-310.pyc
+-rw-r--r--   0        0        0     1488 2023-07-08 17:51:37.130385 roboto_sdk-0.1.7/src/roboto_sdk/domain/triggers/__pycache__/trigger_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0      617 2023-07-08 17:51:37.130385 roboto_sdk-0.1.7/src/roboto_sdk/domain/triggers/__pycache__/trigger_record.cpython-310.pyc
+-rw-r--r--   0        0        0     2280 2023-07-08 17:50:26.498340 roboto_sdk-0.1.7/src/roboto_sdk/domain/triggers/http_delegate.py
+-rw-r--r--   0        0        0      205 2023-07-08 17:50:26.498340 roboto_sdk-0.1.7/src/roboto_sdk/domain/triggers/http_resources.py
+-rw-r--r--   0        0        0     2685 2023-07-08 17:50:26.498340 roboto_sdk-0.1.7/src/roboto_sdk/domain/triggers/trigger.py
+-rw-r--r--   0        0        0      882 2023-07-08 17:50:26.498340 roboto_sdk-0.1.7/src/roboto_sdk/domain/triggers/trigger_delegate.py
+-rw-r--r--   0        0        0      249 2023-07-08 17:50:26.498340 roboto_sdk-0.1.7/src/roboto_sdk/domain/triggers/trigger_record.py
+-rw-r--r--   0        0        0      262 2023-07-08 17:50:26.502340 roboto_sdk-0.1.7/src/roboto_sdk/domain/users/__init__.py
+-rw-r--r--   0        0        0      554 2023-07-08 17:51:37.110384 roboto_sdk-0.1.7/src/roboto_sdk/domain/users/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1769 2023-07-08 17:51:37.110384 roboto_sdk-0.1.7/src/roboto_sdk/domain/users/__pycache__/http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     2253 2023-07-08 17:51:37.114385 roboto_sdk-0.1.7/src/roboto_sdk/domain/users/__pycache__/user.cpython-310.pyc
+-rw-r--r--   0        0        0     1181 2023-07-08 17:51:37.110384 roboto_sdk-0.1.7/src/roboto_sdk/domain/users/__pycache__/user_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0      723 2023-07-08 17:51:37.110384 roboto_sdk-0.1.7/src/roboto_sdk/domain/users/__pycache__/user_record.cpython-310.pyc
+-rw-r--r--   0        0        0     1121 2023-07-08 17:50:26.502340 roboto_sdk-0.1.7/src/roboto_sdk/domain/users/http_delegate.py
+-rw-r--r--   0        0        0     1463 2023-07-08 17:50:26.502340 roboto_sdk-0.1.7/src/roboto_sdk/domain/users/user.py
+-rw-r--r--   0        0        0      499 2023-07-08 17:50:26.502340 roboto_sdk-0.1.7/src/roboto_sdk/domain/users/user_delegate.py
+-rw-r--r--   0        0        0      257 2023-07-08 17:50:26.502340 roboto_sdk-0.1.7/src/roboto_sdk/domain/users/user_record.py
+-rw-r--r--   0        0        0      285 2023-07-08 17:50:26.502340 roboto_sdk-0.1.7/src/roboto_sdk/exceptions/__init__.py
+-rw-r--r--   0        0        0      506 2023-07-08 17:51:37.082384 roboto_sdk-0.1.7/src/roboto_sdk/exceptions/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2401 2023-07-08 17:51:37.082384 roboto_sdk-0.1.7/src/roboto_sdk/exceptions/__pycache__/domain.cpython-310.pyc
+-rw-r--r--   0        0        0     1568 2023-07-08 17:50:26.502340 roboto_sdk-0.1.7/src/roboto_sdk/exceptions/domain.py
+-rw-r--r--   0        0        0      782 2023-07-08 17:50:26.506340 roboto_sdk-0.1.7/src/roboto_sdk/http/__init__.py
+-rw-r--r--   0        0        0      902 2023-07-08 17:51:36.666384 roboto_sdk-0.1.7/src/roboto_sdk/http/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      500 2023-07-08 17:51:36.666384 roboto_sdk-0.1.7/src/roboto_sdk/http/__pycache__/constants.cpython-310.pyc
+-rw-r--r--   0        0        0      785 2023-07-08 17:51:36.666384 roboto_sdk-0.1.7/src/roboto_sdk/http/__pycache__/headers.cpython-310.pyc
+-rw-r--r--   0        0        0     9636 2023-07-08 17:51:36.666384 roboto_sdk-0.1.7/src/roboto_sdk/http/__pycache__/http_client.cpython-310.pyc
+-rw-r--r--   0        0        0     3963 2023-07-08 17:51:36.706384 roboto_sdk-0.1.7/src/roboto_sdk/http/__pycache__/request_decorators.cpython-310.pyc
+-rw-r--r--   0        0        0     1666 2023-07-08 17:51:37.066384 roboto_sdk-0.1.7/src/roboto_sdk/http/__pycache__/testing_util.cpython-310.pyc
+-rw-r--r--   0        0        0      216 2023-07-08 17:50:26.506340 roboto_sdk-0.1.7/src/roboto_sdk/http/constants.py
+-rw-r--r--   0        0        0      588 2023-07-08 17:50:26.506340 roboto_sdk-0.1.7/src/roboto_sdk/http/headers.py
+-rw-r--r--   0        0        0     9060 2023-07-08 17:50:26.506340 roboto_sdk-0.1.7/src/roboto_sdk/http/http_client.py
+-rw-r--r--   0        0        0     3161 2023-07-08 17:50:26.506340 roboto_sdk-0.1.7/src/roboto_sdk/http/request_decorators.py
+-rw-r--r--   0        0        0     1004 2023-07-08 17:50:26.506340 roboto_sdk-0.1.7/src/roboto_sdk/http/testing_util.py
+-rw-r--r--   0        0        0      158 2023-07-08 17:50:26.506340 roboto_sdk-0.1.7/src/roboto_sdk/logging.py
+-rw-r--r--   0        0        0      224 2023-07-08 17:50:26.506340 roboto_sdk-0.1.7/src/roboto_sdk/pagination.py
+-rw-r--r--   0        0        0      168 2023-07-08 17:50:26.506340 roboto_sdk-0.1.7/src/roboto_sdk/profile/__init__.py
+-rw-r--r--   0        0        0      428 2023-07-08 17:51:37.062384 roboto_sdk-0.1.7/src/roboto_sdk/profile/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2991 2023-07-08 17:51:37.062384 roboto_sdk-0.1.7/src/roboto_sdk/profile/__pycache__/profile.cpython-310.pyc
+-rw-r--r--   0        0        0     2977 2023-07-08 17:50:26.506340 roboto_sdk-0.1.7/src/roboto_sdk/profile/profile.py
+-rw-r--r--   0        0        0        0 2023-07-08 17:50:26.506340 roboto_sdk-0.1.7/src/roboto_sdk/py.typed
+-rw-r--r--   0        0        0     1250 2023-07-08 17:50:26.506340 roboto_sdk-0.1.7/src/roboto_sdk/serde.py
+-rw-r--r--   0        0        0      112 2023-07-08 17:50:26.506340 roboto_sdk-0.1.7/src/roboto_sdk/time.py
+-rw-r--r--   0        0        0      691 1970-01-01 00:00:00.000000 roboto_sdk-0.1.7/PKG-INFO
```

### Comparing `roboto_sdk-0.1.6/pyproject.toml` & `roboto_sdk-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires-python = ">=3.10"
 # Ignore this version attribute, it is here to satisfy setuptools.
 # The actual version is set by Poetry in the [tool.poetry] section.
 version = "0.0.0"
 
 [tool.poetry]
 name = "roboto_sdk"
-version = "0.1.6"
+version = "0.1.7"
 description = "Tools for interacting with roboto.ai"
 license = "MIT"
 readme = "README.md"
 authors = ["Roboto <admin@roboto.ai>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/auth/__pycache__/pat.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/auth/__pycache__/pat.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 4037 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 c50f 0000  o.......1..d....
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 c50f 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 6400  d.l.m.Z.m.Z...d.
 00000050: 6401 6c05 5a05 6400 6401 6c06 5a06 6403  d.l.Z.d.d.l.Z.d.
 00000060: 6404 6c07 6d08 5a08 0100 6403 6405 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6508 8300 5a0b 6401 5a0c  m.Z...e...Z.d.Z.
@@ -26,16 +26,16 @@
 00000190: 0000 4000 0000 730c 0000 0065 005a 0164  ..@...s....e.Z.d
 000001a0: 005a 0264 0153 0029 02da 1652 656a 6563  .Z.d.S.)...Rejec
 000001b0: 7465 6454 6f6b 656e 4578 6365 7074 696f  tedTokenExceptio
 000001c0: 6e4e 2903 da08 5f5f 6e61 6d65 5f5f da0a  nN)...__name__..
 000001d0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
 000001e0: 616c 6e61 6d65 5f5f a900 720b 0000 0072  alname__..r....r
 000001f0: 0b00 0000 fae0 2f63 6f64 6562 7569 6c64  ....../codebuild
-00000200: 2f6f 7574 7075 742f 7372 6331 3638 3931  /output/src16891
-00000210: 3535 3339 392f 7372 632f 636f 6465 7374  55399/src/codest
+00000200: 2f6f 7574 7075 742f 7372 6333 3537 3831  /output/src35781
+00000210: 3132 3139 312f 7372 632f 636f 6465 7374  12191/src/codest
 00000220: 6172 2d63 6f6e 6e65 6374 696f 6e73 2e75  ar-connections.u
 00000230: 732d 7765 7374 2d32 2e61 6d61 7a6f 6e61  s-west-2.amazona
 00000240: 7773 2e63 6f6d 2f67 6974 2d68 7474 702f  ws.com/git-http/
 00000250: 3036 3631 3935 3131 3233 3835 2f75 732d  066195112385/us-
 00000260: 7765 7374 2d32 2f65 3635 3032 6138 302d  west-2/e6502a80-
 00000270: 6262 3465 2d34 6662 652d 3837 3263 2d35  bb4e-4fbe-872c-5
 00000280: 6434 3263 3139 3336 3939 642f 726f 626f  d42c193699d/robo
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/auth/pat.py` & `roboto_sdk-0.1.7/src/roboto_sdk/auth/pat.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/cli/actions/commands.py` & `roboto_sdk-0.1.7/src/roboto_sdk/cli/actions/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/cli/actions/create.py` & `roboto_sdk-0.1.7/src/roboto_sdk/cli/actions/create.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/cli/actions/docker_login.py` & `roboto_sdk-0.1.7/src/roboto_sdk/cli/actions/docker_login.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/cli/actions/invoke.py` & `roboto_sdk-0.1.7/src/roboto_sdk/cli/actions/invoke.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/cli/actions/list_invocations.py` & `roboto_sdk-0.1.7/src/roboto_sdk/cli/actions/list_invocations.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/cli/actions/search.py` & `roboto_sdk-0.1.7/src/roboto_sdk/cli/actions/search.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/cli/actions/shared.py` & `roboto_sdk-0.1.7/src/roboto_sdk/cli/actions/shared.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/cli/actions/show.py` & `roboto_sdk-0.1.7/src/roboto_sdk/cli/actions/show.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/cli/actions/update.py` & `roboto_sdk-0.1.7/src/roboto_sdk/cli/actions/update.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/cli/command/args.py` & `roboto_sdk-0.1.7/src/roboto_sdk/cli/command/args.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/cli/command/model.py` & `roboto_sdk-0.1.7/src/roboto_sdk/cli/command/model.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/cli/datasets/commands.py` & `roboto_sdk-0.1.7/src/roboto_sdk/cli/datasets/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/cli/entry.py` & `roboto_sdk-0.1.7/src/roboto_sdk/cli/entry.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     ActionHttpDelegate,
     InvocationHttpDelegate,
 )
 from ..domain.datasets import DatasetHttpDelegate
 from ..domain.orgs import OrgHttpDelegate
 from ..domain.tokens import TokenHttpDelegate
 from ..domain.triggers import TriggerHttpDelegate
+from ..domain.users import UserHttpDelegate
 from ..http import (
     HttpClient,
     LocalAuthDecorator,
     PATAuthDecorator,
 )
 from ..profile import RobotoProfile
 from .actions import (
@@ -86,14 +87,15 @@
         http_client=http, roboto_service_base_url=profile_entry.default_endpoint
     )
     context.invocations = InvocationHttpDelegate(
         http_client=http, roboto_service_base_url=profile_entry.default_endpoint
     )
     context.orgs = OrgHttpDelegate(http_client=http)
     context.triggers = TriggerHttpDelegate(http_client=http)
+    context.users = UserHttpDelegate(http_client=http)
     context.http = http
     context.tokens = TokenHttpDelegate(http_client=http)
 
 
 def entry():
     parser = argparse.ArgumentParser(
         prog="roboto",
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/cli/invocations/status.py` & `roboto_sdk-0.1.7/src/roboto_sdk/cli/invocations/status.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/cli/orgs/commands.py` & `roboto_sdk-0.1.7/src/roboto_sdk/cli/orgs/commands.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,64 +44,63 @@
         "--bind-email-domain",
         action="store_true",
         help="Automatically add new users with your email domain to this org",
     )
 
 
 def delete(args, context: CLIContext, parser: argparse.ArgumentParser):
+    if not args.ignore_prompt:
+        sys.stdout.write("Are you absolutely sure you want to delete your org? [y/n]: ")
+
+        choice = input().lower()
+        if choice not in ["y", "yes"]:
+            return
+
     Org.from_id(org_id=args.org, org_delegate=context.orgs).delete()
     sys.stdout.write("Successfully deleted!\n")
 
 
 def delete_setup_parser(parser):
     parser.add_argument(
         "--org",
         type=str,
         required=True,
         help="The org_id for the org you're about to delete.",
     )
 
+    parser.add_argument(
+        "--ignore-prompt",
+        action="store_true",
+        help="Ignore the prompt which asks you to confirm that you'd like to delete your org.",
+    )
+
 
-def get(args, context: CLIContext, parser: argparse.ArgumentParser):
+def show(args, context: CLIContext, parser: argparse.ArgumentParser):
     record = Org.from_id(org_id=args.org, org_delegate=context.orgs)
     sys.stdout.write(json.dumps(record.to_dict()) + "\n")
 
 
-def get_setup_parser(parser):
+def show_setup_parser(parser):
     parser.add_argument(
         "--org",
         type=str,
-        required=True,
         help="The org_id for the org you want to see.",
     )
 
 
-def list_orgs(args, context: CLIContext, parser: argparse.ArgumentParser):
-    records = Org.for_user(user_id=None, org_delegate=context.orgs)
-    for record in records:
-        sys.stdout.write(json.dumps(record.to_dict()) + "\n")
-
-
-def list_roles(args, context: CLIContext, parser: argparse.ArgumentParser):
-    records = OrgRole.for_user(user_id=None, org_delegate=context.orgs)
-    for record in records:
-        sys.stdout.write(json.dumps(record.to_dict()) + "\n")
-
-
 def list_org_members(args, context: CLIContext, parser: argparse.ArgumentParser):
     records = OrgRole.for_org(org_id=args.org, org_delegate=context.orgs)
     for record in records:
         sys.stdout.write(json.dumps(record.to_dict()) + "\n")
 
 
 def list_org_members_setup_parser(parser):
     parser.add_argument(
         "--org",
         type=str,
-        required=True,
         help="The org_id for the org you want to see.",
     )
 
 
 def remove_user(args, context: CLIContext, parser: argparse.ArgumentParser):
     org = Org.from_id(org_id=args.org, org_delegate=context.orgs)
     org.remove_user(user_id=args.user)
@@ -138,20 +137,33 @@
         "--user",
         type=str,
         required=True,
         help="The user_id of the user to invite.",
     )
     parser.add_argument(
         "--org",
-        type=str,
         help="The org_id of the org to invite a user to. "
         + "Required only if the caller is a member of more than one org.",
     )
 
 
+def list_invites(args, context: CLIContext, parser: argparse.ArgumentParser):
+    invites = OrgInvite.for_org(org_id=args.org, org_delegate=context.orgs)
+    for invite in invites:
+        sys.stdout.write(json.dumps(invite.to_dict()) + "\n")
+
+
+def list_invites_setup_parser(parser):
+    parser.add_argument(
+        "--org",
+        help="The org_id of the org to view invites for. "
+        + "Required only if the caller is a member of more than one org.",
+    )
+
+
 def add_role(args, context: CLIContext, parser: argparse.ArgumentParser):
     Org.from_id(org_id=args.org, org_delegate=context.orgs).add_role_for_user(
         user_id=args.user, role_name=args.role
     )
     sys.stdout.write("Added!\n")
 
 
@@ -217,39 +229,24 @@
     name="delete",
     logic=delete,
     setup_parser=delete_setup_parser,
     command_kwargs={"help": "Deletes an existing organization"},
 )
 
 
-get_command = RobotoCommand(
-    name="get",
-    logic=get,
-    setup_parser=get_setup_parser,
+show_command = RobotoCommand(
+    name="show",
+    logic=show,
+    setup_parser=show_setup_parser,
     command_kwargs={"help": "Gets metadata for a single organization"},
 )
 
 
-list_orgs_command = RobotoCommand(
-    name="list-orgs",
-    logic=list_orgs,
-    command_kwargs={"help": "Lists the orgs that you're a member of"},
-)
-
-
-list_roles_command = RobotoCommand(
-    name="list-roles",
-    logic=list_roles,
-    command_kwargs={
-        "help": "Lists the roles that you have in orgs that you're a member of"
-    },
-)
-
 list_org_members_command = RobotoCommand(
-    name="list-org-members",
+    name="members",
     logic=list_org_members,
     setup_parser=list_org_members_setup_parser,
     command_kwargs={"help": "Lists the members of an organization"},
 )
 
 remove_user_command = RobotoCommand(
     name="remove-user",
@@ -261,14 +258,21 @@
 invite_command = RobotoCommand(
     name="invite-user",
     logic=invite_user,
     setup_parser=invite_user_setup_parser,
     command_kwargs={"help": "Invites a user to join an org."},
 )
 
+list_invites_command = RobotoCommand(
+    name="list-invites",
+    logic=list_invites,
+    setup_parser=list_invites_setup_parser,
+    command_kwargs={"help": "Lists the current pending invites for a specified org"},
+)
+
 add_role_command = RobotoCommand(
     name="add-role",
     logic=add_role,
     setup_parser=add_role_setup_parser,
     command_kwargs={"help": "Promotes a user to a more permissive org access level."},
 )
 
@@ -279,21 +283,20 @@
     command_kwargs={"help": "Demotes a user to a less permissive org access level."},
 )
 
 commands = [
     add_role_command,
     create_command,
     delete_command,
-    get_command,
     invite_command,
+    list_invites_command,
     list_org_members_command,
-    list_orgs_command,
-    list_roles_command,
     remove_role_command,
     remove_user_command,
+    show_command,
 ]
 
 command_set = RobotoCommandSet(
     name="orgs",
     help="Commands for interacting with orgs.",
     commands=commands,
 )
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/cli/tokens/commands.py` & `roboto_sdk-0.1.7/src/roboto_sdk/cli/tokens/commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,28 +9,26 @@
     RobotoCommand,
     RobotoCommandSet,
 )
 from ..context import CLIContext
 
 
 def create(args, context: CLIContext, parser: argparse.ArgumentParser):
-    print(args)
     token = Token.create(
         user_id=None,
         expiry_days=args.expiry_days,
         name=args.name,
         description=args.description,
         token_delegate=context.tokens,
     )
-    sys.stdout.write(json.dumps(token.to_dict()) + "\n")
 
     creds_example_json = json.dumps({"username": "<your email>", "token": token.secret})
 
     sys.stderr.write(
-        "\nThis secret will only be available to you once, so store it somewhere safe!\n"
+        "This secret will only be available to you once, so store it somewhere safe!\n"
         + "To use this personal access token, create a file at ~/.roboto/credentials.json, and populate it with "
         + f"{creds_example_json}.\n"
     )
 
 
 def create_setup_parser(parser):
     parser.add_argument(
@@ -54,39 +52,39 @@
         help="The number of days this token will be valid for.",
     )
 
 
 def list(args, context: CLIContext, parser: argparse.ArgumentParser):
     tokens = Token.for_user(user_id=None, token_delegate=context.tokens)
     for token in tokens:
-        sys.stdout.write(json.dumps(token.to_dict()) + "\n")
+        sys.stdout.write(json.dumps(token.to_dict(exclude_none=True)) + "\n")
 
 
-def get(args, context: CLIContext, parser: argparse.ArgumentParser):
-    token = Token.from_id(token_id=args.token_id, token_delegate=context.tokens)
-    sys.stdout.write(json.dumps(token.to_dict()) + "\n")
+def show(args, context: CLIContext, parser: argparse.ArgumentParser):
+    token = Token.from_id(token_id=args.id, token_delegate=context.tokens)
+    sys.stdout.write(json.dumps(token.to_dict(exclude_none=True)) + "\n")
 
 
-def get_setup_parser(parser):
+def show_setup_parser(parser):
     parser.add_argument(
-        "--token-id",
+        "--id",
         type=str,
         required=True,
         help="The token_id for a token to look up.",
     )
 
 
 def delete(args, context: CLIContext, parser: argparse.ArgumentParser):
-    Token.from_id(token_id=args.token_id, token_delegate=context.tokens).delete()
-    sys.stdout.write("Successfully deleted!\n")
+    Token.from_id(token_id=args.id, token_delegate=context.tokens).delete()
+    sys.stdout.write(f"Successfully deleted token '{args.id}'!\n")
 
 
 def delete_setup_parser(parser):
     parser.add_argument(
-        "--token-id",
+        "--id",
         type=str,
         required=True,
         help="The token_id for a token to delete.",
     )
 
 
 create_command = RobotoCommand(
@@ -99,28 +97,33 @@
 
 list_command = RobotoCommand(
     name="list",
     logic=list,
     command_kwargs={"help": "Creates a temporary access token."},
 )
 
-get_command = RobotoCommand(
-    name="get",
-    logic=get,
-    setup_parser=get_setup_parser,
+show_command = RobotoCommand(
+    name="show",
+    logic=show,
+    setup_parser=show_setup_parser,
     command_kwargs={"help": "Gets a token by unique token_id."},
 )
 
 delete_command = RobotoCommand(
     name="delete",
     logic=delete,
     setup_parser=delete_setup_parser,
     command_kwargs={"help": "Deletes a token by unique token_id."},
 )
 
-commands = [create_command, get_command, delete_command, list_command]
+commands = [
+    create_command,
+    delete_command,
+    list_command,
+    show_command,
+]
 
 command_set = RobotoCommandSet(
     name="tokens",
     help="Commands for generating and parsing access tokens.",
     commands=commands,
 )
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/cli/triggers/commands.py` & `roboto_sdk-0.1.7/src/roboto_sdk/cli/triggers/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/__pycache__/http_delegates.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/__pycache__/http_delegates.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 1974 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 b607 0000  o.......1..d....
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 b607 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6402 6403 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6402 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6405 6406 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6405 6407 6c09 6d0a 5a0a 0100 6405  ..d.d.l.m.Z...d.
 00000070: 6408 6c0b 6d0c 5a0c 0100 6405 6409 6c0d  d.l.m.Z...d.d.l.
@@ -66,16 +66,16 @@
 00000410: 0a00 0000 720b 0000 0072 0c00 0000 720d  ....r....r....r.
 00000420: 0000 0072 0f00 0000 290c 7218 0000 0072  ...r....).r....r
 00000430: 1900 0000 da05 656e 7472 795a 0461 7574  ......entryZ.aut
 00000440: 68da 0468 7474 7072 1000 0000 7211 0000  h..httpr....r...
 00000450: 0072 1200 0000 7213 0000 0072 1400 0000  .r....r....r....
 00000460: 7215 0000 0072 1600 0000 a900 721e 0000  r....r......r...
 00000470: 00fa ed2f 636f 6465 6275 696c 642f 6f75  .../codebuild/ou
-00000480: 7470 7574 2f73 7263 3136 3839 3135 3533  tput/src16891553
-00000490: 3939 2f73 7263 2f63 6f64 6573 7461 722d  99/src/codestar-
+00000480: 7470 7574 2f73 7263 3335 3738 3131 3231  tput/src35781121
+00000490: 3931 2f73 7263 2f63 6f64 6573 7461 722d  91/src/codestar-
 000004a0: 636f 6e6e 6563 7469 6f6e 732e 7573 2d77  connections.us-w
 000004b0: 6573 742d 322e 616d 617a 6f6e 6177 732e  est-2.amazonaws.
 000004c0: 636f 6d2f 6769 742d 6874 7470 2f30 3636  com/git-http/066
 000004d0: 3139 3531 3132 3338 352f 7573 2d77 6573  195112385/us-wes
 000004e0: 742d 322f 6536 3530 3261 3830 2d62 6234  t-2/e6502a80-bb4
 000004f0: 652d 3466 6265 2d38 3732 632d 3564 3432  e-4fbe-872c-5d42
 00000500: 6331 3933 3639 3964 2f72 6f62 6f74 6f2d  c193699d/roboto-
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__init__.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/__init__.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 1877 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 5507 0000  o.......1..dU...
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 5507 0000  o..........dU...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 d800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 0100 6400 6403 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 6d0a 5a0a 0100 6400 6404 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6405 6c0d 6d0e 5a0e 6d0f 5a0f  ..d.d.l.m.Z.m.Z.
@@ -82,16 +82,16 @@
 00000510: 5f72 6573 6f75 7263 6573 7214 0000 0072  _resourcesr....r
 00000520: 1500 0000 7216 0000 005a 1169 6e76 6f63  ....r....Z.invoc
 00000530: 6174 696f 6e5f 7265 636f 7264 7217 0000  ation_recordr...
 00000540: 0072 1800 0000 7219 0000 0072 1a00 0000  .r....r....r....
 00000550: 721b 0000 0072 1c00 0000 721d 0000 00da  r....r....r.....
 00000560: 075f 5f61 6c6c 5f5f a900 7221 0000 0072  .__all__..r!...r
 00000570: 2100 0000 faef 2f63 6f64 6562 7569 6c64  !...../codebuild
-00000580: 2f6f 7574 7075 742f 7372 6331 3638 3931  /output/src16891
-00000590: 3535 3339 392f 7372 632f 636f 6465 7374  55399/src/codest
+00000580: 2f6f 7574 7075 742f 7372 6333 3537 3831  /output/src35781
+00000590: 3132 3139 312f 7372 632f 636f 6465 7374  12191/src/codest
 000005a0: 6172 2d63 6f6e 6e65 6374 696f 6e73 2e75  ar-connections.u
 000005b0: 732d 7765 7374 2d32 2e61 6d61 7a6f 6e61  s-west-2.amazona
 000005c0: 7773 2e63 6f6d 2f67 6974 2d68 7474 702f  ws.com/git-http/
 000005d0: 3036 3631 3935 3131 3233 3835 2f75 732d  066195112385/us-
 000005e0: 7765 7374 2d32 2f65 3635 3032 6138 302d  west-2/e6502a80-
 000005f0: 6262 3465 2d34 6662 652d 3837 3263 2d35  bb4e-4fbe-872c-5
 00000600: 6434 3263 3139 3336 3939 642f 726f 626f  d42c193699d/robo
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/action.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/__pycache__/action.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 8680 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 e821 0000  o.......1..d.!..
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 e821 0000  o..........d.!..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 9600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 6d05 5a05 0100 6403  d.l.m.Z.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6405 6406 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 0100 6405  m.Z.m.Z.m.Z...d.
 00000070: 6407 6c0c 6d0d 5a0d 6d0e 5a0e 0100 6405  d.l.m.Z.m.Z...d.
@@ -65,45 +65,45 @@
 00000400: 6411 650d 650c 650e 6602 1900 6602 6439  d.e.e.e.f...f.d9
 00000410: 643a 8404 5a27 0905 0905 0905 6442 643b  d:..Z'......dBd;
 00000420: 650d 650c 650e 6602 1900 643c 6509 650f  e.e.e.f...d<e.e.
 00000430: 6528 1900 1900 640a 6509 650c 1900 643d  e(....d.e.e...d=
 00000440: 6509 650c 1900 6411 6405 660a 643e 643f  e.e...d.d.f.d>d?
 00000450: 8405 5a29 6405 5300 2943 da06 4163 7469  ..Z)d.S.)C..Acti
 00000460: 6f6e 3e07 0000 00da 066f 7267 5f69 645a  on>......org_idZ
-00000470: 0a63 7265 6174 6564 5f61 74da 0375 7269  .created_at..uri
-00000480: da0a 6372 6561 7465 645f 6279 5a0b 6d6f  ..created_byZ.mo
-00000490: 6469 6669 6564 5f62 79da 086d 6f64 6966  dified_by..modif
-000004a0: 6965 64da 046e 616d 65da 185f 4163 7469  ied..name.._Acti
+00000470: 0b6d 6f64 6966 6965 645f 6279 da03 7572  .modified_by..ur
+00000480: 695a 0a63 7265 6174 6564 5f61 74da 046e  iZ.created_at..n
+00000490: 616d 65da 086d 6f64 6966 6965 64da 0a63  ame..modified..c
+000004a0: 7265 6174 6564 5f62 79da 185f 4163 7469  reated_by.._Acti
 000004b0: 6f6e 5f5f 6163 7469 6f6e 5f64 656c 6567  on__action_deleg
 000004c0: 6174 65da 1c5f 4163 7469 6f6e 5f5f 696e  ate.._Action__in
 000004d0: 766f 6361 7469 6f6e 5f64 656c 6567 6174  vocation_delegat
 000004e0: 65da 0f5f 4163 7469 6f6e 5f5f 7265 636f  e.._Action__reco
 000004f0: 7264 4eda 235f 4163 7469 6f6e 5f5f 7465  rdN.#_Action__te
 00000500: 6d70 5f63 6f6e 7461 696e 6572 5f63 7265  mp_container_cre
-00000510: 6465 6e74 6961 6c73 7216 0000 00da 0f61  dentialsr......a
+00000510: 6465 6e74 6961 6c73 7214 0000 00da 0f61  dentialsr......a
 00000520: 6374 696f 6e5f 6465 6c65 6761 7465 da13  ction_delegate..
 00000530: 696e 766f 6361 7469 6f6e 5f64 656c 6567  invocation_deleg
 00000540: 6174 6572 1200 0000 da0b 6465 7363 7269  ater......descri
 00000550: 7074 696f 6eda 086d 6574 6164 6174 61da  ption..metadata.
-00000560: 0474 6167 7372 1400 0000 da14 636f 6d70  .tagsr......comp
+00000560: 0474 6167 7372 1600 0000 da14 636f 6d70  .tagsr......comp
 00000570: 7574 655f 7265 7175 6972 656d 656e 7473  ute_requirements
 00000580: da14 636f 6e74 6169 6e65 725f 7061 7261  ..container_para
 00000590: 6d65 7465 7273 da06 7265 7475 726e 630b  meters..returnc.
 000005a0: 0000 0000 0000 0000 0000 000c 0000 000a  ................
 000005b0: 0000 0043 0000 0073 2400 0000 7c02 a000  ...C...s$...|...
 000005c0: 7c01 7c04 7c08 7c05 7c06 7c07 7c09 7c0a  |.|.|.|.|.|.|.|.
 000005d0: a108 7d0b 7c00 7c0b 7c02 7c03 8303 5300  ..}.|.|.|.|...S.
 000005e0: a901 4e29 015a 0d63 7265 6174 655f 6163  ..N).Z.create_ac
-000005f0: 7469 6f6e 290c da03 636c 7372 1600 0000  tion)...clsr....
+000005f0: 7469 6f6e 290c da03 636c 7372 1400 0000  tion)...clsr....
 00000600: 721b 0000 0072 1c00 0000 7212 0000 0072  r....r....r....r
-00000610: 1d00 0000 721e 0000 0072 1f00 0000 7214  ....r....r....r.
+00000610: 1d00 0000 721e 0000 0072 1f00 0000 7216  ....r....r....r.
 00000620: 0000 0072 2000 0000 7221 0000 00da 0672  ...r ...r!.....r
 00000630: 6563 6f72 64a9 0072 2600 0000 faed 2f63  ecord..r&...../c
 00000640: 6f64 6562 7569 6c64 2f6f 7574 7075 742f  odebuild/output/
-00000650: 7372 6331 3638 3931 3535 3339 392f 7372  src1689155399/sr
+00000650: 7372 6333 3537 3831 3132 3139 312f 7372  src3578112191/sr
 00000660: 632f 636f 6465 7374 6172 2d63 6f6e 6e65  c/codestar-conne
 00000670: 6374 696f 6e73 2e75 732d 7765 7374 2d32  ctions.us-west-2
 00000680: 2e61 6d61 7a6f 6e61 7773 2e63 6f6d 2f67  .amazonaws.com/g
 00000690: 6974 2d68 7474 702f 3036 3631 3935 3131  it-http/06619511
 000006a0: 3233 3835 2f75 732d 7765 7374 2d32 2f65  2385/us-west-2/e
 000006b0: 3635 3032 6138 302d 6262 3465 2d34 6662  6502a80-bb4e-4fb
 000006c0: 652d 3837 3263 2d35 6434 3263 3139 3336  e-872c-5d42c1936
@@ -118,15 +118,15 @@
 00000750: 0c0a 7a0d 4163 7469 6f6e 2e63 7265 6174  ..z.Action.creat
 00000760: 6563 0500 0000 0000 0000 0000 0000 0600  ec..............
 00000770: 0000 0400 0000 4300 0000 7318 0000 007c  ......C...s....|
 00000780: 02a0 007c 017c 04a1 027d 057c 007c 057c  ...|.|...}.|.|.|
 00000790: 027c 0383 0353 0072 2300 0000 2901 5a19  .|...S.r#...).Z.
 000007a0: 6765 745f 6163 7469 6f6e 5f62 795f 7072  get_action_by_pr
 000007b0: 696d 6172 795f 6b65 7929 0672 2400 0000  imary_key).r$...
-000007c0: 7216 0000 0072 1b00 0000 721c 0000 0072  r....r....r....r
+000007c0: 7214 0000 0072 1b00 0000 721c 0000 0072  r....r....r....r
 000007d0: 1200 0000 7225 0000 0072 2600 0000 7226  ....r%...r&...r&
 000007e0: 0000 0072 2700 0000 da09 6672 6f6d 5f6e  ...r'.....from_n
 000007f0: 616d 6544 0000 0073 0400 0000 0c08 0c01  ameD...s........
 00000800: 7a10 4163 7469 6f6e 2e66 726f 6d5f 6e61  z.Action.from_na
 00000810: 6d65 da07 6669 6c74 6572 7329 0372 1100  me..filters).r..
 00000820: 0000 4e4e 6305 0000 0000 0000 0000 0000  ..NNc...........
 00000830: 000c 0000 0006 0000 0063 0000 0073 a200  .........c...s..
@@ -195,17 +195,17 @@
 00000c20: 0029 0272 1900 0000 7215 0000 0072 3a00  .).r....r....r:.
 00000c30: 0000 7226 0000 0072 2600 0000 7227 0000  ..r&...r&...r'..
 00000c40: 00da 0d6c 6173 745f 6d6f 6469 6669 6564  ...last_modified
 00000c50: 8000 0000 723b 0000 007a 1441 6374 696f  ....r;...z.Actio
 00000c60: 6e2e 6c61 7374 5f6d 6f64 6966 6965 6463  n.last_modifiedc
 00000c70: 0100 0000 0000 0000 0000 0000 0100 0000  ................
 00000c80: 0100 0000 4300 0000 7239 0000 0072 2300  ....C...r9...r#.
-00000c90: 0000 2902 7219 0000 0072 1600 0000 723a  ..).r....r....r:
+00000c90: 0000 2902 7219 0000 0072 1400 0000 723a  ..).r....r....r:
 00000ca0: 0000 0072 2600 0000 7226 0000 0072 2700  ...r&...r&...r'.
-00000cb0: 0000 7216 0000 0084 0000 0072 3b00 0000  ..r........r;...
+00000cb0: 0000 7214 0000 0084 0000 0072 3b00 0000  ..r........r;...
 00000cc0: 7a0b 4163 7469 6f6e 2e6e 616d 6563 0100  z.Action.namec..
 00000cd0: 0000 0000 0000 0000 0000 0100 0000 0100  ................
 00000ce0: 0000 4300 0000 7239 0000 0072 2300 0000  ..C...r9...r#...
 00000cf0: 2902 7219 0000 0072 1200 0000 723a 0000  ).r....r....r:..
 00000d00: 0072 2600 0000 7226 0000 0072 2700 0000  .r&...r&...r'...
 00000d10: 7212 0000 0088 0000 0072 3b00 0000 7a0d  r........r;...z.
 00000d20: 4163 7469 6f6e 2e6f 7267 5f69 6463 0100  Action.org_idc..
@@ -406,15 +406,15 @@
 00001950: 736d 6574 686f 64da 0373 7472 724e 0000  smethod..strrN..
 00001960: 0072 0200 0000 da04 6c69 7374 7207 0000  .r......listr...
 00001970: 0072 0900 0000 7228 0000 0072 2900 0000  .r....r(...r)...
 00001980: da0b 636f 6c6c 6563 7469 6f6e 73da 0361  ..collections..a
 00001990: 6263 da09 4765 6e65 7261 746f 7272 3600  bc..Generatorr6.
 000019a0: 0000 7238 0000 00da 0870 726f 7065 7274  ..r8.....propert
 000019b0: 7972 2000 0000 7221 0000 00da 0864 6174  yr ...r!.....dat
-000019c0: 6574 696d 6572 3c00 0000 7216 0000 0072  etimer<...r....r
+000019c0: 6574 696d 6572 3c00 0000 7214 0000 0072  etimer<...r....r
 000019d0: 1200 0000 7213 0000 0072 4000 0000 720f  ....r....r@...r.
 000019e0: 0000 0072 1000 0000 720d 0000 0072 4f00  ...r....r....rO.
 000019f0: 0000 7252 0000 0072 5400 0000 720b 0000  ..rR...rT...r...
 00001a00: 0072 4c00 0000 7226 0000 0072 2600 0000  .rL...r&...r&...
 00001a10: 7226 0000 0072 2700 0000 7211 0000 001a  r&...r'...r.....
 00001a20: 0000 0073 0e01 0000 0a00 0801 080a 0801  ...s............
 00001a30: 0801 1001 0202 0206 0201 0201 0201 0201  ................
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/action_container_resources.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/__pycache__/action_container_resources.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 2685 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 7d0a 0000  o.......1..d}...
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 7d0a 0000  o..........d}...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a03 6400 6401 6c04 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c05 5a05 6402 6403 6c06 6d07 5a07  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6402 6404 6c08 6d09 5a09 0100 4700  ..d.d.l.m.Z...G.
 00000070: 6405 6406 8400 6406 6503 6a0a 8303 5a0b  d.d...d.e.j...Z.
@@ -20,15 +20,15 @@
 00000130: 6570 6f73 6974 6f72 7950 7572 706f 7365  epositoryPurpose
 00000140: da08 6578 6563 7574 6f72 4e29 04da 085f  ..executorN)..._
 00000150: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
 00000160: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
 00000170: 5fda 0845 7865 6375 746f 72a9 0072 0c00  _..Executor..r..
 00000180: 0000 720c 0000 00e1 0101 0000 2f63 6f64  ..r........./cod
 00000190: 6562 7569 6c64 2f6f 7574 7075 742f 7372  ebuild/output/sr
-000001a0: 6331 3638 3931 3535 3339 392f 7372 632f  c1689155399/src/
+000001a0: 6333 3537 3831 3132 3139 312f 7372 632f  c3578112191/src/
 000001b0: 636f 6465 7374 6172 2d63 6f6e 6e65 6374  codestar-connect
 000001c0: 696f 6e73 2e75 732d 7765 7374 2d32 2e61  ions.us-west-2.a
 000001d0: 6d61 7a6f 6e61 7773 2e63 6f6d 2f67 6974  mazonaws.com/git
 000001e0: 2d68 7474 702f 3036 3631 3935 3131 3233  -http/0661951123
 000001f0: 3835 2f75 732d 7765 7374 2d32 2f65 3635  85/us-west-2/e65
 00000200: 3032 6138 302d 6262 3465 2d34 6662 652d  02a80-bb4e-4fbe-
 00000210: 3837 3263 2d35 6434 3263 3139 3336 3939  872c-5d42c193699
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/action_delegate.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/__pycache__/action_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 2875 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 3b0b 0000  o.......1..d;...
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 3b0b 0000  o..........d;...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7800 0000 6400  .....@...sx...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6401 6c05  m.Z.m.Z...d.d.l.
 00000050: 5a05 6403 6404 6c06 6d07 5a07 0100 6405  Z.d.d.l.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  d.l.m.Z.m.Z.m.Z.
 00000070: 0100 6405 6407 6c0c 6d0d 5a0d 0100 4700  ..d.d.l.m.Z...G.
@@ -50,16 +50,16 @@
 00000310: 7061 7261 746f 724e 2908 da08 5f5f 6e61  paratorN)...__na
 00000320: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
 00000330: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
 00000340: 5f5f 646f 635f 5fda 0373 7472 da0f 5f5f  __doc__..str..__
 00000350: 616e 6e6f 7461 7469 6f6e 735f 5f72 0200  annotations__r..
 00000360: 0000 7203 0000 00a9 0072 1800 0000 7218  ..r......r....r.
 00000370: 0000 00fa f62f 636f 6465 6275 696c 642f  ...../codebuild/
-00000380: 6f75 7470 7574 2f73 7263 3136 3839 3135  output/src168915
-00000390: 3533 3939 2f73 7263 2f63 6f64 6573 7461  5399/src/codesta
+00000380: 6f75 7470 7574 2f73 7263 3335 3738 3131  output/src357811
+00000390: 3231 3931 2f73 7263 2f63 6f64 6573 7461  2191/src/codesta
 000003a0: 722d 636f 6e6e 6563 7469 6f6e 732e 7573  r-connections.us
 000003b0: 2d77 6573 742d 322e 616d 617a 6f6e 6177  -west-2.amazonaw
 000003c0: 732e 636f 6d2f 6769 742d 6874 7470 2f30  s.com/git-http/0
 000003d0: 3636 3139 3531 3132 3338 352f 7573 2d77  66195112385/us-w
 000003e0: 6573 742d 322f 6536 3530 3261 3830 2d62  est-2/e6502a80-b
 000003f0: 6234 652d 3466 6265 2d38 3732 632d 3564  b4e-4fbe-872c-5d
 00000400: 3432 6331 3933 3639 3964 2f72 6f62 6f74  42c193699d/robot
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/action_http_delegate.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/__pycache__/action_http_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 5629 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 fd15 0000  o.......1..d....
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 fb15 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 ce00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 6403  d.l.m.Z.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6403 6405 6c00  d.l.m.Z...d.d.l.
 00000060: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000070: 0100 6403 6406 6c0b 6d0c 5a0c 0100 6403  ..d.d.l.m.Z...d.
@@ -85,16 +85,16 @@
 00000540: 0300 0000 731a 0000 0074 0083 00a0 01a1  ....s....t......
 00000550: 0001 007c 027c 005f 027c 017c 005f 0364  ...|.|._.|.|._.d
 00000560: 0053 00a9 014e 2904 da05 7375 7065 72da  .S...N)...super.
 00000570: 085f 5f69 6e69 745f 5f72 1800 0000 7219  .__init__r....r.
 00000580: 0000 0029 03da 0473 656c 6672 1a00 0000  ...)...selfr....
 00000590: 721b 0000 00a9 01da 095f 5f63 6c61 7373  r........__class
 000005a0: 5f5f a900 fafb 2f63 6f64 6562 7569 6c64  __..../codebuild
-000005b0: 2f6f 7574 7075 742f 7372 6331 3638 3931  /output/src16891
-000005c0: 3535 3339 392f 7372 632f 636f 6465 7374  55399/src/codest
+000005b0: 2f6f 7574 7075 742f 7372 6333 3537 3831  /output/src35781
+000005c0: 3132 3139 312f 7372 632f 636f 6465 7374  12191/src/codest
 000005d0: 6172 2d63 6f6e 6e65 6374 696f 6e73 2e75  ar-connections.u
 000005e0: 732d 7765 7374 2d32 2e61 6d61 7a6f 6e61  s-west-2.amazona
 000005f0: 7773 2e63 6f6d 2f67 6974 2d68 7474 702f  ws.com/git-http/
 00000600: 3036 3631 3935 3131 3233 3835 2f75 732d  066195112385/us-
 00000610: 7765 7374 2d32 2f65 3635 3032 6138 302d  west-2/e6502a80-
 00000620: 6262 3465 2d34 6662 652d 3837 3263 2d35  bb4e-4fbe-872c-5
 00000630: 6434 3263 3139 3336 3939 642f 726f 626f  d42c193699d/robo
@@ -274,69 +274,69 @@
 00001110: 6405 8d01 a101 5700 5300 0400 740a 7949  d.....W.S...t.yI
 00001120: 0100 7d09 0100 7a0e 7c09 6a0b 740c 6a0d  ..}...z.|.j.t.j.
 00001130: 6a0e 6b02 7244 740f 7c09 6a10 8301 6400  j.k.rDt.|.j...d.
 00001140: 8202 8200 6400 7d09 7e09 7701 7700 2906  ....d.}.~.w.w.).
 00001150: 4e72 3b00 0000 2902 7253 0000 0072 5400  Nr;...).rS...rT.
 00001160: 0000 7230 0000 0072 3100 0000 7232 0000  ..r0...r1...r2..
 00001170: 0029 1172 1900 0000 7228 0000 0072 1400  .).r....r(...r..
-00001180: 0000 7218 0000 00da 0570 6174 6368 da04  ..r......patch..
-00001190: 6469 6374 7227 0000 0072 1500 0000 7235  dictr'...r....r5
-000011a0: 0000 0072 3600 0000 7208 0000 00da 0673  ...r6...r......s
-000011b0: 7461 7475 73da 0468 7474 70da 0a48 5454  tatus..http..HTT
-000011c0: 5053 7461 7475 73da 0843 4f4e 464c 4943  PStatus..CONFLIC
-000011d0: 5472 1600 0000 da03 6d73 6729 0a72 2000  Tr......msg).r .
-000011e0: 0000 7241 0000 0072 5300 0000 7254 0000  ..rA...rS...rT..
-000011f0: 0072 2500 0000 7255 0000 0072 3700 0000  .r%...rU...r7...
-00001200: da07 7061 796c 6f61 6472 3e00 0000 723f  ..payloadr>...r?
-00001210: 0000 0072 2300 0000 7223 0000 0072 2400  ...r#...r#...r$.
-00001220: 0000 da06 7570 6461 7465 9100 0000 7320  ....update....s 
-00001230: 0000 0012 0802 0102 010e 0106 fe02 0406  ................
-00001240: 0112 0106 ff16 030e 010e 010c 0102 0108  ................
-00001250: 8002 fd7a 1941 6374 696f 6e48 7474 7044  ...z.ActionHttpD
-00001260: 656c 6567 6174 652e 7570 6461 7465 2902  elegate.update).
-00001270: 4e4e 2907 4e4e 4e4e 4e4e 4e72 1d00 0000  NN).NNNNNNNr....
-00001280: 291a da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-00001290: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-000012a0: 6e61 6d65 5f5f da07 5f5f 646f 635f 5f72  name__..__doc__r
-000012b0: 0900 0000 da0f 5f5f 616e 6e6f 7461 7469  ......__annotati
-000012c0: 6f6e 735f 5fda 0373 7472 721f 0000 0072  ons__..strr....r
-000012d0: 0300 0000 7257 0000 0072 2700 0000 7202  ....rW...r'...r.
-000012e0: 0000 00da 046c 6973 7472 0e00 0000 7210  .....listr....r.
-000012f0: 0000 0072 1500 0000 723a 0000 0072 4000  ...r....r:...r@.
-00001300: 0000 7247 0000 0072 0f00 0000 7248 0000  ..rG...r....rH..
-00001310: 0072 0b00 0000 7252 0000 0072 1200 0000  .r....rR...r....
-00001320: 725e 0000 00da 0d5f 5f63 6c61 7373 6365  r^.....__classce
-00001330: 6c6c 5f5f 7223 0000 0072 2300 0000 7221  ll__r#...r#...r!
-00001340: 0000 0072 2400 0000 7217 0000 0024 0000  ...r$...r....$..
-00001350: 0073 ba00 0000 0a00 0401 0804 0801 1a02  .s..............
-00001360: 0206 04ff 0601 02ff 0601 02ff 0a02 0afe  ................
-00001370: 020d 0201 0201 0201 0201 0201 0201 04f7  ................
-00001380: 0202 02fe 0603 02fd 0604 02fc 0605 02fb  ................
-00001390: 0e06 02fa 0a07 02f9 0608 02f8 0609 02f7  ................
-000013a0: 020a 0af6 021c 04ff 0201 02ff 0601 02ff  ................
-000013b0: 0202 0afe 020f 04fb 0202 02fe 0203 02fd  ................
-000013c0: 0204 02fc 0605 02fb 0206 0afa 0215 04fd  ................
-000013d0: 0202 02fe 0603 02fd 0204 0afc 020c 0201  ................
-000013e0: 04fc 0a02 02fe 0603 02fd 0e04 02fc 0605  ................
-000013f0: 0afb 021b 0201 04fa 0202 02fe 0a03 02fd  ................
-00001400: 0a04 02fc 0605 02fb 0606 02fa 0207 12f9  ................
-00001410: 7217 0000 0029 2172 5900 0000 724f 0000  r....)!rY...rO..
-00001420: 00da 0674 7970 696e 6772 0200 0000 7203  ...typingr....r.
-00001430: 0000 00da 0a65 7863 6570 7469 6f6e 7372  .....exceptionsr
-00001440: 0500 0000 7206 0000 0072 0700 0000 7208  ....r....r....r.
-00001450: 0000 0072 0900 0000 da07 6c6f 6767 696e  ...r......loggin
-00001460: 6772 0a00 0000 da0a 7061 6769 6e61 7469  gr......paginati
-00001470: 6f6e 720b 0000 00da 0573 6572 6465 720c  onr......serder.
-00001480: 0000 00da 1a61 6374 696f 6e5f 636f 6e74  .....action_cont
-00001490: 6169 6e65 725f 7265 736f 7572 6365 7372  ainer_resourcesr
-000014a0: 0e00 0000 720f 0000 0072 1000 0000 da0f  ....r....r......
-000014b0: 6163 7469 6f6e 5f64 656c 6567 6174 6572  action_delegater
-000014c0: 1100 0000 7212 0000 00da 1561 6374 696f  ....r......actio
-000014d0: 6e5f 6874 7470 5f72 6573 6f75 7263 6573  n_http_resources
-000014e0: 7213 0000 0072 1400 0000 da0d 6163 7469  r....r......acti
-000014f0: 6f6e 5f72 6563 6f72 6472 1500 0000 da05  on_recordr......
-00001500: 6572 726f 7272 1600 0000 da06 6c6f 6767  errorr......logg
-00001510: 6572 7217 0000 0072 2300 0000 7223 0000  err....r#...r#..
-00001520: 0072 2300 0000 7224 0000 00da 083c 6d6f  .r#...r$.....<mo
-00001530: 6475 6c65 3e01 0000 0073 1e00 0000 0800  dule>....s......
-00001540: 0801 1001 0c02 1801 0c06 0c01 0c01 1401  ................
-00001550: 1005 1004 0c04 0c01 0604 1403            ............
+00001180: 0000 7218 0000 0072 4600 0000 da04 6469  ..r....rF.....di
+00001190: 6374 7227 0000 0072 1500 0000 7235 0000  ctr'...r....r5..
+000011a0: 0072 3600 0000 7208 0000 00da 0673 7461  .r6...r......sta
+000011b0: 7475 73da 0468 7474 70da 0a48 5454 5053  tus..http..HTTPS
+000011c0: 7461 7475 73da 0843 4f4e 464c 4943 5472  tatus..CONFLICTr
+000011d0: 1600 0000 da03 6d73 6729 0a72 2000 0000  ......msg).r ...
+000011e0: 7241 0000 0072 5300 0000 7254 0000 0072  rA...rS...rT...r
+000011f0: 2500 0000 7255 0000 0072 3700 0000 da07  %...rU...r7.....
+00001200: 7061 796c 6f61 6472 3e00 0000 723f 0000  payloadr>...r?..
+00001210: 0072 2300 0000 7223 0000 0072 2400 0000  .r#...r#...r$...
+00001220: da06 7570 6461 7465 9100 0000 7320 0000  ..update....s ..
+00001230: 0012 0802 0102 010e 0106 fe02 0406 0112  ................
+00001240: 0106 ff16 030e 010e 010c 0102 0108 8002  ................
+00001250: fd7a 1941 6374 696f 6e48 7474 7044 656c  .z.ActionHttpDel
+00001260: 6567 6174 652e 7570 6461 7465 2902 4e4e  egate.update).NN
+00001270: 2907 4e4e 4e4e 4e4e 4e72 1d00 0000 291a  ).NNNNNNNr....).
+00001280: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00001290: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+000012a0: 6d65 5f5f da07 5f5f 646f 635f 5f72 0900  me__..__doc__r..
+000012b0: 0000 da0f 5f5f 616e 6e6f 7461 7469 6f6e  ....__annotation
+000012c0: 735f 5fda 0373 7472 721f 0000 0072 0300  s__..strr....r..
+000012d0: 0000 7256 0000 0072 2700 0000 7202 0000  ..rV...r'...r...
+000012e0: 00da 046c 6973 7472 0e00 0000 7210 0000  ...listr....r...
+000012f0: 0072 1500 0000 723a 0000 0072 4000 0000  .r....r:...r@...
+00001300: 7247 0000 0072 0f00 0000 7248 0000 0072  rG...r....rH...r
+00001310: 0b00 0000 7252 0000 0072 1200 0000 725d  ....rR...r....r]
+00001320: 0000 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
+00001330: 5f5f 7223 0000 0072 2300 0000 7221 0000  __r#...r#...r!..
+00001340: 0072 2400 0000 7217 0000 0024 0000 0073  .r$...r....$...s
+00001350: ba00 0000 0a00 0401 0804 0801 1a02 0206  ................
+00001360: 04ff 0601 02ff 0601 02ff 0a02 0afe 020d  ................
+00001370: 0201 0201 0201 0201 0201 0201 04f7 0202  ................
+00001380: 02fe 0603 02fd 0604 02fc 0605 02fb 0e06  ................
+00001390: 02fa 0a07 02f9 0608 02f8 0609 02f7 020a  ................
+000013a0: 0af6 021c 04ff 0201 02ff 0601 02ff 0202  ................
+000013b0: 0afe 020f 04fb 0202 02fe 0203 02fd 0204  ................
+000013c0: 02fc 0605 02fb 0206 0afa 0215 04fd 0202  ................
+000013d0: 02fe 0603 02fd 0204 0afc 020c 0201 04fc  ................
+000013e0: 0a02 02fe 0603 02fd 0e04 02fc 0605 0afb  ................
+000013f0: 021b 0201 04fa 0202 02fe 0a03 02fd 0a04  ................
+00001400: 02fc 0605 02fb 0606 02fa 0207 12f9 7217  ..............r.
+00001410: 0000 0029 2172 5800 0000 724f 0000 00da  ...)!rX...rO....
+00001420: 0674 7970 696e 6772 0200 0000 7203 0000  .typingr....r...
+00001430: 00da 0a65 7863 6570 7469 6f6e 7372 0500  ...exceptionsr..
+00001440: 0000 7206 0000 0072 0700 0000 7208 0000  ..r....r....r...
+00001450: 0072 0900 0000 da07 6c6f 6767 696e 6772  .r......loggingr
+00001460: 0a00 0000 da0a 7061 6769 6e61 7469 6f6e  ......pagination
+00001470: 720b 0000 00da 0573 6572 6465 720c 0000  r......serder...
+00001480: 00da 1a61 6374 696f 6e5f 636f 6e74 6169  ...action_contai
+00001490: 6e65 725f 7265 736f 7572 6365 7372 0e00  ner_resourcesr..
+000014a0: 0000 720f 0000 0072 1000 0000 da0f 6163  ..r....r......ac
+000014b0: 7469 6f6e 5f64 656c 6567 6174 6572 1100  tion_delegater..
+000014c0: 0000 7212 0000 00da 1561 6374 696f 6e5f  ..r......action_
+000014d0: 6874 7470 5f72 6573 6f75 7263 6573 7213  http_resourcesr.
+000014e0: 0000 0072 1400 0000 da0d 6163 7469 6f6e  ...r......action
+000014f0: 5f72 6563 6f72 6472 1500 0000 da05 6572  _recordr......er
+00001500: 726f 7272 1600 0000 da06 6c6f 6767 6572  rorr......logger
+00001510: 7217 0000 0072 2300 0000 7223 0000 0072  r....r#...r#...r
+00001520: 2300 0000 7224 0000 00da 083c 6d6f 6475  #...r$.....<modu
+00001530: 6c65 3e01 0000 0073 1e00 0000 0800 0801  le>....s........
+00001540: 1001 0c02 1801 0c06 0c01 0c01 1401 1005  ................
+00001550: 1004 0c04 0c01 0604 1403                 ..........
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/action_http_resources.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/__pycache__/action_http_resources.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 860 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 5c03 0000  o.......1..d\...
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 5c03 0000  o..........d\...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a03 6403 6404 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000050: 6d06 5a06 0100 6403 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 4700 6406 6407 8400 6407 6503 6a09  ..G.d.d...d.e.j.
 00000070: 8303 5a0a 4700 6408 6409 8400 6409 6503  ..Z.G.d.d...d.e.
@@ -37,16 +37,16 @@
 00000240: 5f5f 616e 6e6f 7461 7469 6f6e 735f 5f72  __annotations__r
 00000250: 0a00 0000 7203 0000 00da 0870 7964 616e  ....r......pydan
 00000260: 7469 63da 0546 6965 6c64 da04 6469 6374  tic..Field..dict
 00000270: 720c 0000 0072 0200 0000 da04 6c69 7374  r....r......list
 00000280: 720d 0000 0072 0e00 0000 7205 0000 0072  r....r....r....r
 00000290: 0f00 0000 7206 0000 00a9 0072 1900 0000  ....r......r....
 000002a0: 7219 0000 00fa fc2f 636f 6465 6275 696c  r....../codebuil
-000002b0: 642f 6f75 7470 7574 2f73 7263 3136 3839  d/output/src1689
-000002c0: 3135 3533 3939 2f73 7263 2f63 6f64 6573  155399/src/codes
+000002b0: 642f 6f75 7470 7574 2f73 7263 3335 3738  d/output/src3578
+000002c0: 3131 3231 3931 2f73 7263 2f63 6f64 6573  112191/src/codes
 000002d0: 7461 722d 636f 6e6e 6563 7469 6f6e 732e  tar-connections.
 000002e0: 7573 2d77 6573 742d 322e 616d 617a 6f6e  us-west-2.amazon
 000002f0: 6177 732e 636f 6d2f 6769 742d 6874 7470  aws.com/git-http
 00000300: 2f30 3636 3139 3531 3132 3338 352f 7573  /066195112385/us
 00000310: 2d77 6573 742d 322f 6536 3530 3261 3830  -west-2/e6502a80
 00000320: 2d62 6234 652d 3466 6265 2d38 3732 632d  -bb4e-4fbe-872c-
 00000330: 3564 3432 6331 3933 3639 3964 2f72 6f62  5d42c193699d/rob
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/action_record.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/__pycache__/action_record.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 988 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 dc03 0000  o.......1..d....
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 dc03 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6400 6401 6c04 5a04 6403  m.Z...d.d.l.Z.d.
 00000050: 6404 6c05 6d06 5a06 6d07 5a07 0100 4700  d.l.m.Z.m.Z...G.
 00000060: 6405 6406 8400 6406 6504 6a08 8303 5a09  d.d...d.e.j...Z.
 00000070: 6401 5300 2907 e900 0000 004e 2902 da03  d.S.)......N)...
@@ -51,16 +51,16 @@
 00000320: 696f 6e73 5f5f da03 7374 72da 0870 7964  ions__..str..pyd
 00000330: 616e 7469 63da 0546 6965 6c64 7205 0000  antic..Fieldr...
 00000340: 0072 0f00 0000 7206 0000 0072 1000 0000  .r....r....r....
 00000350: 7211 0000 0072 0300 0000 7212 0000 00da  r....r....r.....
 00000360: 0464 6963 7472 0200 0000 7213 0000 00da  .dictr....r.....
 00000370: 046c 6973 7472 1400 0000 a900 7220 0000  .listr......r ..
 00000380: 0072 2000 0000 faf4 2f63 6f64 6562 7569  .r ...../codebui
-00000390: 6c64 2f6f 7574 7075 742f 7372 6331 3638  ld/output/src168
-000003a0: 3931 3535 3339 392f 7372 632f 636f 6465  9155399/src/code
+00000390: 6c64 2f6f 7574 7075 742f 7372 6333 3537  ld/output/src357
+000003a0: 3831 3132 3139 312f 7372 632f 636f 6465  8112191/src/code
 000003b0: 7374 6172 2d63 6f6e 6e65 6374 696f 6e73  star-connections
 000003c0: 2e75 732d 7765 7374 2d32 2e61 6d61 7a6f  .us-west-2.amazo
 000003d0: 6e61 7773 2e63 6f6d 2f67 6974 2d68 7474  naws.com/git-htt
 000003e0: 702f 3036 3631 3935 3131 3233 3835 2f75  p/066195112385/u
 000003f0: 732d 7765 7374 2d32 2f65 3635 3032 6138  s-west-2/e6502a8
 00000400: 302d 6262 3465 2d34 6662 652d 3837 3263  0-bb4e-4fbe-872c
 00000410: 2d35 6434 3263 3139 3336 3939 642f 726f  -5d42c193699d/ro
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/error.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/__pycache__/error.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 106 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 6a00 0000  o.......1..dj...
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 6a00 0000  o..........dj...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2400 0000 4700  .....@...s$...G.
 00000030: 6400 6401 8400 6401 6500 8303 5a01 4700  d.d...d.e...Z.G.
 00000040: 6402 6403 8400 6403 6500 8303 5a02 6404  d.d...d.e...Z.d.
 00000050: 5300 2905 6300 0000 0000 0000 0000 0000  S.).c...........
 00000060: 0000 0000 0001 0000 0040 0000 00f3 0c00  .........@......
 00000070: 0000 6500 5a01 6400 5a02 6401 5300 2902  ..e.Z.d.Z.d.S.).
 00000080: da21 4163 7469 6f6e 5570 6461 7465 436f  .!ActionUpdateCo
 00000090: 6e64 6974 696f 6e43 6865 636b 4661 696c  nditionCheckFail
 000000a0: 7572 654e a903 da08 5f5f 6e61 6d65 5f5f  ureN....__name__
 000000b0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
 000000c0: 7175 616c 6e61 6d65 5f5f a900 7207 0000  qualname__..r...
 000000d0: 0072 0700 0000 faec 2f63 6f64 6562 7569  .r....../codebui
-000000e0: 6c64 2f6f 7574 7075 742f 7372 6331 3638  ld/output/src168
-000000f0: 3931 3535 3339 392f 7372 632f 636f 6465  9155399/src/code
+000000e0: 6c64 2f6f 7574 7075 742f 7372 6333 3537  ld/output/src357
+000000f0: 3831 3132 3139 312f 7372 632f 636f 6465  8112191/src/code
 00000100: 7374 6172 2d63 6f6e 6e65 6374 696f 6e73  star-connections
 00000110: 2e75 732d 7765 7374 2d32 2e61 6d61 7a6f  .us-west-2.amazo
 00000120: 6e61 7773 2e63 6f6d 2f67 6974 2d68 7474  naws.com/git-htt
 00000130: 702f 3036 3631 3935 3131 3233 3835 2f75  p/066195112385/u
 00000140: 732d 7765 7374 2d32 2f65 3635 3032 6138  s-west-2/e6502a8
 00000150: 302d 6262 3465 2d34 6662 652d 3837 3263  0-bb4e-4fbe-872c
 00000160: 2d35 6434 3263 3139 3336 3939 642f 726f  -5d42c193699d/ro
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/invocation.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/__pycache__/invocation.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 4836 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 e412 0000  o.......1..d....
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 e412 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6a00 0000 6400  .....@...sj...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 6d04 5a04 0100 6403 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 0100 6405 6406 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6405 6407 6c0a 6d0b 5a0b 0100 6405  ..d.d.l.m.Z...d.
 00000070: 6408 6c0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  d.l.m.Z.m.Z.m.Z.
@@ -60,15 +60,15 @@
 000003b0: 0000 0400 0000 4300 0000 7316 0000 007c  ......C...s....|
 000003c0: 02a0 007c 017c 03a1 027d 047c 007c 047c  ...|.|...}.|.|.|
 000003d0: 0283 0253 00a9 014e 2901 5a09 6765 745f  ...S...N).Z.get_
 000003e0: 6279 5f69 6429 05da 0363 6c73 7211 0000  by_id)...clsr...
 000003f0: 0072 1200 0000 7213 0000 00da 0672 6563  .r....r......rec
 00000400: 6f72 64a9 0072 1800 0000 faf1 2f63 6f64  ord..r....../cod
 00000410: 6562 7569 6c64 2f6f 7574 7075 742f 7372  ebuild/output/sr
-00000420: 6331 3638 3931 3535 3339 392f 7372 632f  c1689155399/src/
+00000420: 6333 3537 3831 3132 3139 312f 7372 632f  c3578112191/src/
 00000430: 636f 6465 7374 6172 2d63 6f6e 6e65 6374  codestar-connect
 00000440: 696f 6e73 2e75 732d 7765 7374 2d32 2e61  ions.us-west-2.a
 00000450: 6d61 7a6f 6e61 7773 2e63 6f6d 2f67 6974  mazonaws.com/git
 00000460: 2d68 7474 702f 3036 3631 3935 3131 3233  -http/0661951123
 00000470: 3835 2f75 732d 7765 7374 2d32 2f65 3635  85/us-west-2/e65
 00000480: 3032 6138 302d 6262 3465 2d34 6662 652d  02a80-bb4e-4fbe-
 00000490: 3837 3263 2d35 6434 3263 3139 3336 3939  872c-5d42c193699
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/invocation_delegate.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/__pycache__/invocation_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 1939 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 9307 0000  o.......1..d....
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 9307 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6403 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6405 6406 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6405 6407 6c09 6d0a 5a0a 0100 6405  ..d.d.l.m.Z...d.
 00000070: 6408 6c0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  d.l.m.Z.m.Z.m.Z.
@@ -55,16 +55,16 @@
 00000360: 6174 696f 6eda 1163 7265 6174 655f 696e  ation..create_in
 00000370: 766f 6361 7469 6f6e a901 da13 4e6f 7449  vocation....NotI
 00000380: 6d70 6c65 6d65 6e74 6564 4572 726f 7229  mplementedError)
 00000390: 09da 0473 656c 6672 0f00 0000 7210 0000  ...selfr....r...
 000003a0: 0072 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
 000003b0: 7214 0000 0072 1500 0000 7216 0000 00a9  r....r....r.....
 000003c0: 0072 1d00 0000 fafa 2f63 6f64 6562 7569  .r....../codebui
-000003d0: 6c64 2f6f 7574 7075 742f 7372 6331 3638  ld/output/src168
-000003e0: 3931 3535 3339 392f 7372 632f 636f 6465  9155399/src/code
+000003d0: 6c64 2f6f 7574 7075 742f 7372 6333 3537  ld/output/src357
+000003e0: 3831 3132 3139 312f 7372 632f 636f 6465  8112191/src/code
 000003f0: 7374 6172 2d63 6f6e 6e65 6374 696f 6e73  star-connections
 00000400: 2e75 732d 7765 7374 2d32 2e61 6d61 7a6f  .us-west-2.amazo
 00000410: 6e61 7773 2e63 6f6d 2f67 6974 2d68 7474  naws.com/git-htt
 00000420: 702f 3036 3631 3935 3131 3233 3835 2f75  p/066195112385/u
 00000430: 732d 7765 7374 2d32 2f65 3635 3032 6138  s-west-2/e6502a8
 00000440: 302d 6262 3465 2d34 6662 652d 3837 3263  0-bb4e-4fbe-872c
 00000450: 2d35 6434 3263 3139 3336 3939 642f 726f  -5d42c193699d/ro
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/invocation_http_delegate.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/__pycache__/invocation_http_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 5108 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 f413 0000  o.......1..d....
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 f213 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 ba00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6403 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 0100 6403 6405 6c08  m.Z.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6403 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6403 6407 6c0c 6d0d 5a0d 0100 6408  ..d.d.l.m.Z...d.
@@ -76,16 +76,16 @@
 000004b0: 0000 0073 1a00 0000 7400 8300 a001 a100  ...s....t.......
 000004c0: 0100 7c02 7c00 5f02 7c01 7c00 5f03 6400  ..|.|._.|.|._.d.
 000004d0: 5300 a901 4e29 04da 0573 7570 6572 da08  S...N)...super..
 000004e0: 5f5f 696e 6974 5f5f 7217 0000 0072 1800  __init__r....r..
 000004f0: 0000 2903 da04 7365 6c66 7219 0000 0072  ..)...selfr....r
 00000500: 1a00 0000 a901 da09 5f5f 636c 6173 735f  ........__class_
 00000510: 5fa9 00fa ff2f 636f 6465 6275 696c 642f  _..../codebuild/
-00000520: 6f75 7470 7574 2f73 7263 3136 3839 3135  output/src168915
-00000530: 3533 3939 2f73 7263 2f63 6f64 6573 7461  5399/src/codesta
+00000520: 6f75 7470 7574 2f73 7263 3335 3738 3131  output/src357811
+00000530: 3231 3931 2f73 7263 2f63 6f64 6573 7461  2191/src/codesta
 00000540: 722d 636f 6e6e 6563 7469 6f6e 732e 7573  r-connections.us
 00000550: 2d77 6573 742d 322e 616d 617a 6f6e 6177  -west-2.amazonaw
 00000560: 732e 636f 6d2f 6769 742d 6874 7470 2f30  s.com/git-http/0
 00000570: 3636 3139 3531 3132 3338 352f 7573 2d77  66195112385/us-w
 00000580: 6573 742d 322f 6536 3530 3261 3830 2d62  est-2/e6502a80-b
 00000590: 6234 652d 3466 6265 2d38 3732 632d 3564  b4e-4fbe-872c-5d
 000005a0: 3432 6331 3933 3639 3964 2f72 6f62 6f74  42c193699d/robot
@@ -183,126 +183,126 @@
 00000b60: 7c00 6a03 6a04 7c04 7405 7c05 6404 6405  |.j.j.|.t.|.d.d.
 00000b70: 8d02 7c00 a006 7c01 6a07 a101 6406 8d03  ..|...|.j...d...
 00000b80: 7d06 7408 a009 7c06 6a0a 6407 6701 6408  }.t...|.j.d.g.d.
 00000b90: 8d01 a101 5300 2909 4e72 3f00 0000 7a05  ....S.).Nr?...z.
 00000ba0: 2f6c 6f67 7329 0272 4300 0000 7244 0000  /logs).rC...rD..
 00000bb0: 0054 722f 0000 0072 3100 0000 7232 0000  .Tr/...r1...r2..
 00000bc0: 0072 3300 0000 290b 7218 0000 0072 3e00  .r3...).r....r>.
-00000bd0: 0000 7211 0000 0072 1700 0000 da05 7061  ..r....r......pa
-00000be0: 7463 6872 0a00 0000 7226 0000 0072 2400  tchr....r&...r$.
-00000bf0: 0000 7213 0000 0072 3800 0000 7239 0000  ..r....r8...r9..
-00000c00: 0029 0772 1f00 0000 7242 0000 0072 4300  .).r....rB...rC.
-00000c10: 0000 7244 0000 0072 3a00 0000 723b 0000  ..rD...r:...r;..
-00000c20: 0072 3c00 0000 7222 0000 0072 2200 0000  .r<...r"...r"...
-00000c30: 7223 0000 00da 1173 6574 5f6c 6f67 735f  r#.....set_logs_
-00000c40: 6c6f 6361 7469 6f6e 6100 0000 7310 0000  locationa...s...
-00000c50: 0014 030c 0106 0102 010a 010a 0106 fd14  ................
-00000c60: 057a 2849 6e76 6f63 6174 696f 6e48 7474  .z(InvocationHtt
-00000c70: 7044 656c 6567 6174 652e 7365 745f 6c6f  pDelegate.set_lo
-00000c80: 6773 5f6c 6f63 6174 696f 6eda 0673 7461  gs_location..sta
-00000c90: 7475 73da 0664 6574 6169 6c63 0400 0000  tus..detailc....
-00000ca0: 0000 0000 0000 0000 0600 0000 0600 0000  ................
-00000cb0: 4300 0000 734a 0000 007c 006a 009b 0064  C...sJ...|.j...d
-00000cc0: 017c 016a 019b 0064 029d 047d 047c 006a  .|.j...d...}.|.j
-00000cd0: 026a 037c 047c 026a 047c 0364 039c 027c  .j.|.|.j.|.d...|
-00000ce0: 00a0 057c 016a 06a1 0164 048d 037d 0574  ...|.j...d...}.t
-00000cf0: 07a0 087c 056a 0964 0567 0164 068d 01a1  ...|.j.d.g.d....
-00000d00: 0153 0029 074e 723f 0000 007a 072f 7374  .S.).Nr?...z./st
-00000d10: 6174 7573 2902 7247 0000 0072 4800 0000  atus).rG...rH...
-00000d20: 7231 0000 0072 3200 0000 7233 0000 0029  r1...r2...r3...)
-00000d30: 0a72 1800 0000 723e 0000 0072 1700 0000  .r....r>...r....
-00000d40: 7236 0000 00da 0576 616c 7565 7226 0000  r6.....valuer&..
-00000d50: 0072 2400 0000 7213 0000 0072 3800 0000  .r$...r....r8...
-00000d60: 7239 0000 0029 0672 1f00 0000 7242 0000  r9...).r....rB..
-00000d70: 0072 4700 0000 7248 0000 0072 3a00 0000  .rG...rH...r:...
-00000d80: 723c 0000 0072 2200 0000 7222 0000 0072  r<...r"...r"...r
-00000d90: 2300 0000 da18 7570 6461 7465 5f69 6e76  #.....update_inv
-00000da0: 6f63 6174 696f 6e5f 7374 6174 7573 6d00  ocation_statusm.
-00000db0: 0000 730e 0000 0014 0606 0102 010a 010a  ..s.............
-00000dc0: 0106 fd14 057a 2f49 6e76 6f63 6174 696f  .....z/Invocatio
-00000dd0: 6e48 7474 7044 656c 6567 6174 652e 7570  nHttpDelegate.up
-00000de0: 6461 7465 5f69 6e76 6f63 6174 696f 6e5f  date_invocation_
-00000df0: 7374 6174 7573 da07 6669 6c74 6572 73da  status..filters.
-00000e00: 0a70 6167 655f 746f 6b65 6e63 0400 0000  .page_tokenc....
-00000e10: 0000 0000 0000 0000 0800 0000 0600 0000  ................
-00000e20: 4300 0000 736c 0000 007c 0372 067c 037c  C...sl...|.r.|.|
-00000e30: 0164 013c 0074 00a0 0174 00a0 027c 01a1  .d.<.t...t...|..
-00000e40: 01a1 017d 047c 006a 039b 0064 029d 027d  ...}.|.j...d...}
-00000e50: 057c 006a 046a 057c 057c 047c 00a0 067c  .|.j.j.|.|.|...|
-00000e60: 02a1 0164 038d 037d 067c 066a 0764 0467  ...d...}.|.j.d.g
-00000e70: 0164 058d 017d 0774 0864 0664 0784 007c  .d...}.t.d.d...|
-00000e80: 0764 0819 0044 0083 017c 0764 0919 0064  .d...D...|.d...d
-00000e90: 0a8d 0253 0029 0b4e 724c 0000 007a 1d2f  ...S.).NrL...z./
-00000ea0: 7631 2f61 6374 696f 6e73 2f69 6e76 6f63  v1/actions/invoc
-00000eb0: 6174 696f 6e73 2f71 7565 7279 7231 0000  ations/queryr1..
-00000ec0: 0072 3200 0000 7233 0000 0063 0100 0000  .r2...r3...c....
-00000ed0: 0000 0000 0000 0000 0200 0000 0500 0000  ................
-00000ee0: 5300 0000 7316 0000 0067 007c 005d 077d  S...s....g.|.].}
-00000ef0: 0174 00a0 017c 01a1 0191 0271 0253 0072  .t...|.....q.S.r
-00000f00: 2200 0000 2902 7213 0000 0072 3800 0000  "...).r....r8...
-00000f10: 2902 da02 2e30 da07 6461 7461 7365 7472  )....0..datasetr
-00000f20: 2200 0000 7222 0000 0072 2300 0000 da0a  "...r"...r#.....
-00000f30: 3c6c 6973 7463 6f6d 703e 8b00 0000 7306  <listcomp>....s.
-00000f40: 0000 0006 000a 0106 ff7a 3c49 6e76 6f63  .........z<Invoc
-00000f50: 6174 696f 6e48 7474 7044 656c 6567 6174  ationHttpDelegat
-00000f60: 652e 7175 6572 795f 696e 766f 6361 7469  e.query_invocati
-00000f70: 6f6e 732e 3c6c 6f63 616c 733e 2e3c 6c69  ons.<locals>.<li
-00000f80: 7374 636f 6d70 3eda 0569 7465 6d73 da0a  stcomp>..items..
-00000f90: 6e65 7874 5f74 6f6b 656e 2902 7250 0000  next_token).rP..
-00000fa0: 0072 5100 0000 2909 da04 6a73 6f6e da05  .rQ...)...json..
-00000fb0: 6c6f 6164 73da 0564 756d 7073 7218 0000  loads..dumpsr...
-00000fc0: 0072 1700 0000 7236 0000 0072 2600 0000  .r....r6...r&...
-00000fd0: 7239 0000 0072 0900 0000 2908 721f 0000  r9...r....).r...
-00000fe0: 0072 4b00 0000 7224 0000 0072 4c00 0000  .rK...r$...rL...
-00000ff0: da0c 7361 6665 5f66 696c 7465 7273 723a  ..safe_filtersr:
-00001000: 0000 00da 0372 6573 da0c 756e 6d61 7273  .....res..unmars
-00001010: 6861 6c6c 6564 7222 0000 0072 2200 0000  halledr"...r"...
-00001020: 7223 0000 00da 1171 7565 7279 5f69 6e76  r#.....query_inv
-00001030: 6f63 6174 696f 6e73 7b00 0000 731c 0000  ocations{...s...
-00001040: 0004 0608 0110 020c 0106 010c 0106 ff0e  ................
-00001050: 0302 0106 0106 0104 ff06 0306 fc7a 2849  .............z(I
-00001060: 6e76 6f63 6174 696f 6e48 7474 7044 656c  nvocationHttpDel
-00001070: 6567 6174 652e 7175 6572 795f 696e 766f  egate.query_invo
-00001080: 6361 7469 6f6e 7329 024e 4e72 1c00 0000  cations).NNr....
-00001090: 291b da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-000010a0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-000010b0: 6e61 6d65 5f5f da07 5f5f 646f 635f 5f72  name__..__doc__r
-000010c0: 0700 0000 da0f 5f5f 616e 6e6f 7461 7469  ......__annotati
-000010d0: 6f6e 735f 5fda 0373 7472 721e 0000 0072  ons__..strr....r
-000010e0: 0300 0000 da04 6469 6374 7226 0000 0072  ......dictr&...r
-000010f0: 0e00 0000 da04 6c69 7374 720c 0000 0072  ......listr....r
-00001100: 0d00 0000 7212 0000 0072 1400 0000 7213  ....r....r....r.
-00001110: 0000 0072 3d00 0000 7241 0000 0072 4600  ...r=...rA...rF.
-00001120: 0000 7215 0000 0072 4a00 0000 7202 0000  ..r....rJ...r...
-00001130: 0072 0900 0000 7258 0000 00da 0d5f 5f63  .r....rX.....__c
-00001140: 6c61 7373 6365 6c6c 5f5f 7222 0000 0072  lasscell__r"...r
-00001150: 2200 0000 7220 0000 0072 2300 0000 7216  "...r ...r#...r.
-00001160: 0000 0022 0000 0073 8e00 0000 0a00 0401  ..."...s........
-00001170: 0804 0801 1a02 0206 04ff 0601 02ff 0601  ................
-00001180: 02ff 0a02 0afe 0213 04f7 0202 02fe 0603  ................
-00001190: 02fd 0204 02fc 0205 02fb 0206 02fa 0207  ................
-000011a0: 02f9 0208 02f8 0609 02f7 020a 0af6 0222  ..............."
-000011b0: 04ff 0201 02ff 0601 02ff 0202 0afe 0207  ................
-000011c0: 0201 02ff 0201 02ff 0201 02ff 0202 0afe  ................
-000011d0: 0210 04fc 0202 02fe 0203 02fd 0604 02fc  ................
-000011e0: 0205 0afb 0211 0201 04fc 0a02 02fe 0603  ................
-000011f0: 02fd 0e04 02fc 0605 12fb 7216 0000 0029  ..........r....)
-00001200: 1f72 5200 0000 da06 7479 7069 6e67 7202  .rR.....typingr.
-00001210: 0000 0072 0300 0000 da04 6874 7470 7205  ...r......httpr.
-00001220: 0000 0072 0600 0000 7207 0000 00da 076c  ...r....r......l
-00001230: 6f67 6769 6e67 7208 0000 00da 0a70 6167  oggingr......pag
-00001240: 696e 6174 696f 6e72 0900 0000 da05 7365  inationr......se
-00001250: 7264 6572 0a00 0000 da1a 6163 7469 6f6e  rder......action
-00001260: 5f63 6f6e 7461 696e 6572 5f72 6573 6f75  _container_resou
-00001270: 7263 6573 720c 0000 0072 0d00 0000 7227  rcesr....r....r'
-00001280: 0000 0072 0e00 0000 da13 696e 766f 6361  ...r......invoca
-00001290: 7469 6f6e 5f64 656c 6567 6174 6572 0f00  tion_delegater..
-000012a0: 0000 da19 696e 766f 6361 7469 6f6e 5f68  ....invocation_h
-000012b0: 7474 705f 7265 736f 7572 6365 7372 1000  ttp_resourcesr..
-000012c0: 0000 7211 0000 00da 1169 6e76 6f63 6174  ..r......invocat
-000012d0: 696f 6e5f 7265 636f 7264 7212 0000 0072  ion_recordr....r
-000012e0: 1300 0000 7214 0000 0072 1500 0000 da06  ....r....r......
-000012f0: 6c6f 6767 6572 7216 0000 0072 2200 0000  loggerr....r"...
-00001300: 7222 0000 0072 2200 0000 7223 0000 00da  r"...r"...r#....
-00001310: 083c 6d6f 6475 6c65 3e01 0000 0073 1a00  .<module>....s..
-00001320: 0000 0800 1001 1402 0c05 0c01 0c01 1001  ................
-00001330: 0c04 0c01 1003 1804 0607 1403            ............
+00000bd0: 0000 7211 0000 0072 1700 0000 da03 7075  ..r....r......pu
+00000be0: 7472 0a00 0000 7226 0000 0072 2400 0000  tr....r&...r$...
+00000bf0: 7213 0000 0072 3800 0000 7239 0000 0029  r....r8...r9...)
+00000c00: 0772 1f00 0000 7242 0000 0072 4300 0000  .r....rB...rC...
+00000c10: 7244 0000 0072 3a00 0000 723b 0000 0072  rD...r:...r;...r
+00000c20: 3c00 0000 7222 0000 0072 2200 0000 7223  <...r"...r"...r#
+00000c30: 0000 00da 1173 6574 5f6c 6f67 735f 6c6f  .....set_logs_lo
+00000c40: 6361 7469 6f6e 6100 0000 7310 0000 0014  cationa...s.....
+00000c50: 030c 0106 0102 010a 010a 0106 fd14 057a  ...............z
+00000c60: 2849 6e76 6f63 6174 696f 6e48 7474 7044  (InvocationHttpD
+00000c70: 656c 6567 6174 652e 7365 745f 6c6f 6773  elegate.set_logs
+00000c80: 5f6c 6f63 6174 696f 6eda 0673 7461 7475  _location..statu
+00000c90: 73da 0664 6574 6169 6c63 0400 0000 0000  s..detailc......
+00000ca0: 0000 0000 0000 0600 0000 0600 0000 4300  ..............C.
+00000cb0: 0000 734a 0000 007c 006a 009b 0064 017c  ..sJ...|.j...d.|
+00000cc0: 016a 019b 0064 029d 047d 047c 006a 026a  .j...d...}.|.j.j
+00000cd0: 037c 047c 026a 047c 0364 039c 027c 00a0  .|.|.j.|.d...|..
+00000ce0: 057c 016a 06a1 0164 048d 037d 0574 07a0  .|.j...d...}.t..
+00000cf0: 087c 056a 0964 0567 0164 068d 01a1 0153  .|.j.d.g.d.....S
+00000d00: 0029 074e 723f 0000 007a 072f 7374 6174  .).Nr?...z./stat
+00000d10: 7573 2902 7247 0000 0072 4800 0000 7231  us).rG...rH...r1
+00000d20: 0000 0072 3200 0000 7233 0000 0029 0a72  ...r2...r3...).r
+00000d30: 1800 0000 723e 0000 0072 1700 0000 7236  ....r>...r....r6
+00000d40: 0000 00da 0576 616c 7565 7226 0000 0072  .....valuer&...r
+00000d50: 2400 0000 7213 0000 0072 3800 0000 7239  $...r....r8...r9
+00000d60: 0000 0029 0672 1f00 0000 7242 0000 0072  ...).r....rB...r
+00000d70: 4700 0000 7248 0000 0072 3a00 0000 723c  G...rH...r:...r<
+00000d80: 0000 0072 2200 0000 7222 0000 0072 2300  ...r"...r"...r#.
+00000d90: 0000 da18 7570 6461 7465 5f69 6e76 6f63  ....update_invoc
+00000da0: 6174 696f 6e5f 7374 6174 7573 6d00 0000  ation_statusm...
+00000db0: 730e 0000 0014 0606 0102 010a 010a 0106  s...............
+00000dc0: fd14 057a 2f49 6e76 6f63 6174 696f 6e48  ...z/InvocationH
+00000dd0: 7474 7044 656c 6567 6174 652e 7570 6461  ttpDelegate.upda
+00000de0: 7465 5f69 6e76 6f63 6174 696f 6e5f 7374  te_invocation_st
+00000df0: 6174 7573 da07 6669 6c74 6572 73da 0a70  atus..filters..p
+00000e00: 6167 655f 746f 6b65 6e63 0400 0000 0000  age_tokenc......
+00000e10: 0000 0000 0000 0800 0000 0600 0000 4300  ..............C.
+00000e20: 0000 736c 0000 007c 0372 067c 037c 0164  ..sl...|.r.|.|.d
+00000e30: 013c 0074 00a0 0174 00a0 027c 01a1 01a1  .<.t...t...|....
+00000e40: 017d 047c 006a 039b 0064 029d 027d 057c  .}.|.j...d...}.|
+00000e50: 006a 046a 057c 057c 047c 00a0 067c 02a1  .j.j.|.|.|...|..
+00000e60: 0164 038d 037d 067c 066a 0764 0467 0164  .d...}.|.j.d.g.d
+00000e70: 058d 017d 0774 0864 0664 0784 007c 0764  ...}.t.d.d...|.d
+00000e80: 0819 0044 0083 017c 0764 0919 0064 0a8d  ...D...|.d...d..
+00000e90: 0253 0029 0b4e 724c 0000 007a 1d2f 7631  .S.).NrL...z./v1
+00000ea0: 2f61 6374 696f 6e73 2f69 6e76 6f63 6174  /actions/invocat
+00000eb0: 696f 6e73 2f71 7565 7279 7231 0000 0072  ions/queryr1...r
+00000ec0: 3200 0000 7233 0000 0063 0100 0000 0000  2...r3...c......
+00000ed0: 0000 0000 0000 0200 0000 0500 0000 5300  ..............S.
+00000ee0: 0000 7316 0000 0067 007c 005d 077d 0174  ..s....g.|.].}.t
+00000ef0: 00a0 017c 01a1 0191 0271 0253 0072 2200  ...|.....q.S.r".
+00000f00: 0000 2902 7213 0000 0072 3800 0000 2902  ..).r....r8...).
+00000f10: da02 2e30 da07 6461 7461 7365 7472 2200  ...0..datasetr".
+00000f20: 0000 7222 0000 0072 2300 0000 da0a 3c6c  ..r"...r#.....<l
+00000f30: 6973 7463 6f6d 703e 8b00 0000 7306 0000  istcomp>....s...
+00000f40: 0006 000a 0106 ff7a 3c49 6e76 6f63 6174  .......z<Invocat
+00000f50: 696f 6e48 7474 7044 656c 6567 6174 652e  ionHttpDelegate.
+00000f60: 7175 6572 795f 696e 766f 6361 7469 6f6e  query_invocation
+00000f70: 732e 3c6c 6f63 616c 733e 2e3c 6c69 7374  s.<locals>.<list
+00000f80: 636f 6d70 3eda 0569 7465 6d73 da0a 6e65  comp>..items..ne
+00000f90: 7874 5f74 6f6b 656e 2902 7250 0000 0072  xt_token).rP...r
+00000fa0: 5100 0000 2909 da04 6a73 6f6e da05 6c6f  Q...)...json..lo
+00000fb0: 6164 73da 0564 756d 7073 7218 0000 0072  ads..dumpsr....r
+00000fc0: 1700 0000 7236 0000 0072 2600 0000 7239  ....r6...r&...r9
+00000fd0: 0000 0072 0900 0000 2908 721f 0000 0072  ...r....).r....r
+00000fe0: 4b00 0000 7224 0000 0072 4c00 0000 da0c  K...r$...rL.....
+00000ff0: 7361 6665 5f66 696c 7465 7273 723a 0000  safe_filtersr:..
+00001000: 00da 0372 6573 da0c 756e 6d61 7273 6861  ...res..unmarsha
+00001010: 6c6c 6564 7222 0000 0072 2200 0000 7223  lledr"...r"...r#
+00001020: 0000 00da 1171 7565 7279 5f69 6e76 6f63  .....query_invoc
+00001030: 6174 696f 6e73 7b00 0000 731c 0000 0004  ations{...s.....
+00001040: 0608 0110 020c 0106 010c 0106 ff0e 0302  ................
+00001050: 0106 0106 0104 ff06 0306 fc7a 2849 6e76  ...........z(Inv
+00001060: 6f63 6174 696f 6e48 7474 7044 656c 6567  ocationHttpDeleg
+00001070: 6174 652e 7175 6572 795f 696e 766f 6361  ate.query_invoca
+00001080: 7469 6f6e 7329 024e 4e72 1c00 0000 291b  tions).NNr....).
+00001090: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+000010a0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+000010b0: 6d65 5f5f da07 5f5f 646f 635f 5f72 0700  me__..__doc__r..
+000010c0: 0000 da0f 5f5f 616e 6e6f 7461 7469 6f6e  ....__annotation
+000010d0: 735f 5fda 0373 7472 721e 0000 0072 0300  s__..strr....r..
+000010e0: 0000 da04 6469 6374 7226 0000 0072 0e00  ....dictr&...r..
+000010f0: 0000 da04 6c69 7374 720c 0000 0072 0d00  ....listr....r..
+00001100: 0000 7212 0000 0072 1400 0000 7213 0000  ..r....r....r...
+00001110: 0072 3d00 0000 7241 0000 0072 4600 0000  .r=...rA...rF...
+00001120: 7215 0000 0072 4a00 0000 7202 0000 0072  r....rJ...r....r
+00001130: 0900 0000 7258 0000 00da 0d5f 5f63 6c61  ....rX.....__cla
+00001140: 7373 6365 6c6c 5f5f 7222 0000 0072 2200  sscell__r"...r".
+00001150: 0000 7220 0000 0072 2300 0000 7216 0000  ..r ...r#...r...
+00001160: 0022 0000 0073 8e00 0000 0a00 0401 0804  ."...s..........
+00001170: 0801 1a02 0206 04ff 0601 02ff 0601 02ff  ................
+00001180: 0a02 0afe 0213 04f7 0202 02fe 0603 02fd  ................
+00001190: 0204 02fc 0205 02fb 0206 02fa 0207 02f9  ................
+000011a0: 0208 02f8 0609 02f7 020a 0af6 0222 04ff  ............."..
+000011b0: 0201 02ff 0601 02ff 0202 0afe 0207 0201  ................
+000011c0: 02ff 0201 02ff 0201 02ff 0202 0afe 0210  ................
+000011d0: 04fc 0202 02fe 0203 02fd 0604 02fc 0205  ................
+000011e0: 0afb 0211 0201 04fc 0a02 02fe 0603 02fd  ................
+000011f0: 0e04 02fc 0605 12fb 7216 0000 0029 1f72  ........r....).r
+00001200: 5200 0000 da06 7479 7069 6e67 7202 0000  R.....typingr...
+00001210: 0072 0300 0000 da04 6874 7470 7205 0000  .r......httpr...
+00001220: 0072 0600 0000 7207 0000 00da 076c 6f67  .r....r......log
+00001230: 6769 6e67 7208 0000 00da 0a70 6167 696e  gingr......pagin
+00001240: 6174 696f 6e72 0900 0000 da05 7365 7264  ationr......serd
+00001250: 6572 0a00 0000 da1a 6163 7469 6f6e 5f63  er......action_c
+00001260: 6f6e 7461 696e 6572 5f72 6573 6f75 7263  ontainer_resourc
+00001270: 6573 720c 0000 0072 0d00 0000 7227 0000  esr....r....r'..
+00001280: 0072 0e00 0000 da13 696e 766f 6361 7469  .r......invocati
+00001290: 6f6e 5f64 656c 6567 6174 6572 0f00 0000  on_delegater....
+000012a0: da19 696e 766f 6361 7469 6f6e 5f68 7474  ..invocation_htt
+000012b0: 705f 7265 736f 7572 6365 7372 1000 0000  p_resourcesr....
+000012c0: 7211 0000 00da 1169 6e76 6f63 6174 696f  r......invocatio
+000012d0: 6e5f 7265 636f 7264 7212 0000 0072 1300  n_recordr....r..
+000012e0: 0000 7214 0000 0072 1500 0000 da06 6c6f  ..r....r......lo
+000012f0: 6767 6572 7216 0000 0072 2200 0000 7222  ggerr....r"...r"
+00001300: 0000 0072 2200 0000 7223 0000 00da 083c  ...r"...r#.....<
+00001310: 6d6f 6475 6c65 3e01 0000 0073 1a00 0000  module>....s....
+00001320: 0800 1001 1402 0c05 0c01 0c01 1001 0c04  ................
+00001330: 0c01 1003 1804 0607 1403                 ..........
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/invocation_http_resources.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/__pycache__/invocation_http_resources.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 752 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 f002 0000  o.......1..d....
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 f002 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7200 0000 6400  .....@...sr...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6403 6404 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
 00000050: 0100 6403 6405 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 6d09 5a09 0100 4700 6406 6407 8400 6407  m.Z...G.d.d...d.
 00000070: 6502 6a0a 8303 5a0b 4700 6408 6409 8400  e.j...Z.G.d.d...
@@ -37,15 +37,15 @@
 00000240: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
 00000250: 6e61 6d65 5f5f da04 6c69 7374 da03 7374  name__..list..st
 00000260: 72da 0f5f 5f61 6e6e 6f74 6174 696f 6e73  r..__annotations
 00000270: 5f5f 7204 0000 0072 0500 0000 7206 0000  __r....r....r...
 00000280: 0072 0700 0000 7202 0000 00a9 0072 1700  .r....r......r..
 00000290: 0000 7217 0000 00e1 0001 0000 2f63 6f64  ..r........./cod
 000002a0: 6562 7569 6c64 2f6f 7574 7075 742f 7372  ebuild/output/sr
-000002b0: 6331 3638 3931 3535 3339 392f 7372 632f  c1689155399/src/
+000002b0: 6333 3537 3831 3132 3139 312f 7372 632f  c3578112191/src/
 000002c0: 636f 6465 7374 6172 2d63 6f6e 6e65 6374  codestar-connect
 000002d0: 696f 6e73 2e75 732d 7765 7374 2d32 2e61  ions.us-west-2.a
 000002e0: 6d61 7a6f 6e61 7773 2e63 6f6d 2f67 6974  mazonaws.com/git
 000002f0: 2d68 7474 702f 3036 3631 3935 3131 3233  -http/0661951123
 00000300: 3835 2f75 732d 7765 7374 2d32 2f65 3635  85/us-west-2/e65
 00000310: 3032 6138 302d 6262 3465 2d34 6662 652d  02a80-bb4e-4fbe-
 00000320: 3837 3263 2d35 6434 3263 3139 3336 3939  872c-5d42c193699
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/__pycache__/invocation_record.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/__pycache__/invocation_record.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 1839 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 2f07 0000  o.......1..d/...
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 2f07 0000  o..........d/...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6401 6c04  d.l.m.Z...d.d.l.
 00000050: 5a04 6403 6404 6c05 6d06 5a06 6d07 5a07  Z.d.d.l.m.Z.m.Z.
 00000060: 0100 4700 6405 6406 8400 6406 6501 6a08  ..G.d.d...d.e.j.
 00000070: 8303 5a09 4700 6407 6408 8400 6408 6504  ..Z.G.d.d...d.e.
@@ -26,15 +26,15 @@
 00000190: 6374 696f 6e27 7320 496e 7075 7442 696e  ction's InputBin
 000001a0: 6469 6e67 da07 4461 7461 7365 744e 2905  ding..DatasetN).
 000001b0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
 000001c0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
 000001d0: 6d65 5f5f da07 5f5f 646f 635f 5f72 0800  me__..__doc__r..
 000001e0: 0000 a900 720d 0000 0072 0d00 0000 faf8  ....r....r......
 000001f0: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
-00000200: 742f 7372 6331 3638 3931 3535 3339 392f  t/src1689155399/
+00000200: 742f 7372 6333 3537 3831 3132 3139 312f  t/src3578112191/
 00000210: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
 00000220: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
 00000230: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
 00000240: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
 00000250: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
 00000260: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
 00000270: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/action.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/action.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/action_container_resources.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/action_container_resources.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/action_delegate.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/action_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/action_http_delegate.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/action_http_delegate.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
     ) -> ActionRecord:
         url = f"{self.__roboto_service_base_url}/v1/actions/{record.name}"
         payload = UpdateActionRequest(
             updates=updates,
             conditions=conditions if conditions is not None else [],
         )
         try:
-            res = self.__http_client.patch(
+            res = self.__http_client.put(
                 url, data=payload.dict(), headers=self.headers(org_id, updated_by)
             )
             return ActionRecord.parse_obj(res.from_json(json_path=["data"]))
         except ClientError as exc:
             if exc.status == http.HTTPStatus.CONFLICT:
                 raise ActionUpdateConditionCheckFailure(exc.msg) from None
             raise
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/action_http_resources.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/action_http_resources.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/action_record.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/action_record.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/invocation.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/invocation.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/invocation_delegate.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/invocation_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/invocation_http_delegate.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/invocation_http_delegate.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         return InvocationRecord.parse_obj(response.from_json(json_path=["data"]))
 
     def set_logs_location(
         self, record: InvocationRecord, bucket: str, prefix: str
     ) -> InvocationRecord:
         url = f"{self.__roboto_service_base_url}/v1/actions/invocations/{record.invocation_id}/logs"
         request_body = SetLogsLocationRequest(bucket=bucket, prefix=prefix)
-        response = self.__http_client.patch(
+        response = self.__http_client.put(
             url,
             data=pydantic_jsonable_dict(request_body, exclude_none=True),
             headers=self.headers(record.org_id),
         )
         return InvocationRecord.parse_obj(response.from_json(json_path=["data"]))
 
     def update_invocation_status(
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/invocation_http_resources.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/invocation_http_resources.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/actions/invocation_record.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/actions/invocation_record.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/__init__.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/__pycache__/__init__.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/datasets/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 546 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 2202 0000  o.......1..d"...
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 2202 0000  o..........d"...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6406 5a0e 6407  m.Z.m.Z...d.Z.d.
@@ -24,15 +24,15 @@
 00000170: 0400 0000 7205 0000 005a 0d68 7474 705f  ....r....Z.http_
 00000180: 6465 6c65 6761 7465 7206 0000 005a 0e68  delegater....Z.h
 00000190: 7474 705f 7265 736f 7572 6365 7372 0700  ttp_resourcesr..
 000001a0: 0000 da06 7265 636f 7264 7208 0000 0072  ....recordr....r
 000001b0: 0900 0000 720a 0000 00da 075f 5f61 6c6c  ....r......__all
 000001c0: 5f5f a900 720e 0000 0072 0e00 0000 faf0  __..r....r......
 000001d0: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
-000001e0: 742f 7372 6331 3638 3931 3535 3339 392f  t/src1689155399/
+000001e0: 742f 7372 6333 3537 3831 3132 3139 312f  t/src3578112191/
 000001f0: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
 00000200: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
 00000210: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
 00000220: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
 00000230: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
 00000240: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
 00000250: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/__pycache__/dataset.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/datasets/__pycache__/dataset.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 10221 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 ed27 0000  o.......1..d.'..
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 4528 0000  o..........dE(..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 8600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 6d05 5a05 0100 6400  d.l.m.Z.m.Z...d.
 00000050: 6401 6c06 5a06 6403 6404 6c07 6d08 5a08  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6405 6406 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6407 6408 6c0e  m.Z.m.Z...d.d.l.
@@ -19,459 +19,468 @@
 00000120: e901 0000 0029 04da 0a41 6363 6573 734d  .....)...AccessM
 00000130: 6f64 65da 0b43 7265 6465 6e74 6961 6c73  ode..Credentials
 00000140: da0f 4461 7461 7365 7444 656c 6567 6174  ..DatasetDelegat
 00000150: 65da 0f53 746f 7261 6765 4c6f 6361 7469  e..StorageLocati
 00000160: 6f6e 2902 da0d 4164 6d69 6e69 7374 7261  on)...Administra
 00000170: 746f 72da 0d44 6174 6173 6574 5265 636f  tor..DatasetReco
 00000180: 7264 6300 0000 0000 0000 0000 0000 0000  rdc.............
-00000190: 0000 0014 0000 0040 0000 0073 1602 0000  .......@...s....
+00000190: 0000 0014 0000 0040 0000 0073 2802 0000  .......@...s(...
 000001a0: 6500 5a01 6400 5a02 5500 6503 6504 6401  e.Z.d.Z.U.e.e.d.
 000001b0: 3c00 6505 6504 6402 3c00 6403 5a06 6507  <.e.e.d.<.d.Z.e.
 000001c0: 6508 1900 6504 6404 3c00 6403 5a09 6507  e...e.d.<.d.Z.e.
 000001d0: 650a 1900 6504 6405 3c00 650b 650c 6a0d  e...e.d.<.e.e.j.
 000001e0: 650e 6a0f 6403 6403 6403 6403 6403 6607  e.j.d.d.d.d.d.f.
 000001f0: 6406 6503 6407 650c 6408 650e 6409 6507  d.e.d.e.d.e.d.e.
 00000200: 6510 1900 640a 6507 6510 1900 640b 6507  e...d.e.e...d.e.
 00000210: 6511 6510 6512 6602 1900 1900 640c 6507  e.e.e.f.....d.e.
 00000220: 6513 6510 1900 1900 640d 6507 6508 1900  e.e.....d.e.e...
 00000230: 640e 6400 6612 640f 6410 8405 8301 5a14  d.d.f.d.d.....Z.
-00000240: 650b 0903 0903 6430 6411 6510 6406 6503  e.....d0d.e.d.e.
+00000240: 650b 0903 0903 6432 6411 6510 6406 6503  e.....d2d.e.d.e.
 00000250: 6409 6507 6510 1900 640d 6507 6508 1900  d.e.e...d.e.e...
 00000260: 640e 6400 660a 6412 6413 8405 8301 5a15  d.d.f.d.d.....Z.
-00000270: 650b 0903 0903 6430 6414 6511 6510 6512  e.....d0d.e.e.e.
+00000270: 650b 0903 0903 6432 6414 6511 6510 6512  e.....d2d.e.e.e.
 00000280: 6602 1900 6406 6503 640d 6507 6508 1900  f...d.e.d.e.e...
 00000290: 6409 6507 6510 1900 640e 6516 6a17 6a18  d.e.e...d.e.j.j.
 000002a0: 6415 1900 660a 6416 6417 8405 8301 5a19  d...f.d.d.....Z.
-000002b0: 0903 6431 6418 6505 6419 6503 640d 6507  ..d1d.e.d.e.d.e.
+000002b0: 0903 6433 6418 6505 6419 6503 640d 6507  ..d3d.e.d.e.d.e.
 000002c0: 6508 1900 640e 6403 6608 641a 641b 8405  e...d.d.f.d.d...
-000002d0: 5a1a 0903 0903 6430 641c 651b 6a1c 641d  Z.....d0d.e.j.d.
-000002e0: 6507 6513 6510 1900 1900 641e 6507 6513  e.e.e.....d.e.e.
-000002f0: 6510 1900 1900 640e 6403 6608 641f 6420  e.....d.d.f.d.d 
-00000300: 8405 5a1d 651e 6a1f 6403 6602 6421 651e  ..Z.e.j.d.f.d!e.
-00000310: 6422 6507 6510 1900 640e 650a 6606 6423  d"e.e...d.e.f.d#
-00000320: 6424 8405 5a20 0903 0903 6430 641d 6507  d$..Z ....d0d.e.
-00000330: 6513 6510 1900 1900 641e 6507 6513 6510  e.e.....d.e.e.e.
-00000340: 1900 1900 640e 6516 6a17 6a18 6521 6403  ....d.e.j.j.e!d.
-00000350: 6403 6603 1900 6606 6425 6426 8405 5a22  d.f...f.d%d&..Z"
-00000360: 640e 6511 6510 6512 6602 1900 6602 6427  d.e.e.e.f...f.d'
-00000370: 6428 8404 5a23 0903 6431 6429 651b 6a1c  d(..Z#..d1d)e.j.
-00000380: 641e 6507 6513 6510 1900 1900 640e 6403  d.e.e.e.....d.d.
-00000390: 6606 642a 642b 8405 5a24 642c 651b 6a1c  f.d*d+..Z$d,e.j.
-000003a0: 642d 6510 640e 6403 6606 642e 642f 8404  d-e.d.d.f.d.d/..
-000003b0: 5a25 6403 5300 2932 da07 4461 7461 7365  Z%d.S.)2..Datase
-000003c0: 74da 125f 4461 7461 7365 745f 5f64 656c  t.._Dataset__del
-000003d0: 6567 6174 65da 105f 4461 7461 7365 745f  egate.._Dataset_
-000003e0: 5f72 6563 6f72 644e da18 5f44 6174 6173  _recordN.._Datas
-000003f0: 6574 5f5f 6669 6c65 735f 6465 6c65 6761  et__files_delega
-00000400: 7465 da1a 5f44 6174 6173 6574 5f5f 7465  te.._Dataset__te
-00000410: 6d70 5f63 7265 6465 6e74 6961 6c73 da10  mp_credentials..
-00000420: 6461 7461 7365 745f 6465 6c65 6761 7465  dataset_delegate
-00000430: da0d 6164 6d69 6e69 7374 7261 746f 72da  ..administrator.
-00000440: 1073 746f 7261 6765 5f6c 6f63 6174 696f  .storage_locatio
-00000450: 6eda 066f 7267 5f69 64da 0a63 7265 6174  n..org_id..creat
-00000460: 6564 5f62 79da 086d 6574 6164 6174 61da  ed_by..metadata.
-00000470: 0474 6167 73da 0e66 696c 6573 5f64 656c  .tags..files_del
-00000480: 6567 6174 65da 0672 6574 7572 6e63 0900  egate..returnc..
-00000490: 0000 0000 0000 0000 0000 0a00 0000 0800  ................
-000004a0: 0000 4300 0000 7320 0000 007c 01a0 007c  ..C...s ...|...|
-000004b0: 027c 067c 037c 077c 047c 05a1 067d 097c  .|.|.|.|.|...}.|
-000004c0: 007c 097c 017c 0883 0353 00a9 014e 2901  .|.|.|...S...N).
-000004d0: 5a0e 6372 6561 7465 5f64 6174 6173 6574  Z.create_dataset
-000004e0: 290a da03 636c 7372 1700 0000 7218 0000  )...clsr....r...
-000004f0: 0072 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
-00000500: 721c 0000 0072 1d00 0000 721e 0000 00da  r....r....r.....
-00000510: 0672 6563 6f72 64a9 0072 2300 0000 faef  .record..r#.....
-00000520: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
-00000530: 742f 7372 6331 3638 3931 3535 3339 392f  t/src1689155399/
-00000540: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
-00000550: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
-00000560: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
-00000570: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
-00000580: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
-00000590: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
-000005a0: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
-000005b0: 3336 3939 642f 726f 626f 746f 2d61 692f  3699d/roboto-ai/
-000005c0: 726f 626f 746f 2d68 6f73 7465 642d 6170  roboto-hosted-ap
-000005d0: 702f 7061 636b 6167 6573 2f72 6f62 6f74  p/packages/robot
-000005e0: 6f5f 7364 6b2f 7372 632f 726f 626f 746f  o_sdk/src/roboto
-000005f0: 5f73 646b 2f64 6f6d 6169 6e2f 6461 7461  _sdk/domain/data
-00000600: 7365 7473 2f64 6174 6173 6574 2e70 79da  sets/dataset.py.
-00000610: 0663 7265 6174 651d 0000 0073 0800 0000  .create....s....
-00000620: 040c 0c01 04ff 0c03 7a0e 4461 7461 7365  ........z.Datase
-00000630: 742e 6372 6561 7465 da0a 6461 7461 7365  t.create..datase
-00000640: 745f 6964 6305 0000 0000 0000 0000 0000  t_idc...........
-00000650: 0006 0000 0004 0000 0043 0000 0073 1800  .........C...s..
-00000660: 0000 7c02 a000 7c01 7c03 a102 7d05 7c00  ..|...|.|...}.|.
-00000670: 7c05 7c02 7c04 8303 5300 7220 0000 0029  |.|.|...S.r ...)
-00000680: 015a 1a67 6574 5f64 6174 6173 6574 5f62  .Z.get_dataset_b
-00000690: 795f 7072 696d 6172 795f 6b65 7929 0672  y_primary_key).r
-000006a0: 2100 0000 7226 0000 0072 1700 0000 721a  !...r&...r....r.
-000006b0: 0000 0072 1e00 0000 7222 0000 0072 2300  ...r....r"...r#.
-000006c0: 0000 7223 0000 0072 2400 0000 da07 6672  ..r#...r$.....fr
-000006d0: 6f6d 5f69 642e 0000 0073 0400 0000 0c08  om_id....s......
-000006e0: 0c01 7a0f 4461 7461 7365 742e 6672 6f6d  ..z.Dataset.from
-000006f0: 5f69 64da 0766 696c 7465 7273 2903 7212  _id..filters).r.
-00000700: 0000 004e 4e63 0500 0000 0000 0000 0000  ...NNc..........
-00000710: 0000 0c00 0000 0600 0000 6300 0000 73a2  ..........c...s.
-00000720: 0000 0081 0074 0074 016a 02a0 03a1 0083  .....t.t.j......
-00000730: 017d 0574 007c 01a0 03a1 0083 017d 067c  .}.t.|.......}.|
-00000740: 067c 0518 007d 077c 0772 2c74 047c 0783  .|...}.|.r,t.|..
-00000750: 0164 016b 047d 087c 0872 1e64 026e 0164  .d.k.}.|.r.d.n.d
-00000760: 037d 0974 057c 079b 0064 047c 099b 0064  .}.t.|...d.|...d
-00000770: 057c 059b 009d 0583 0182 017c 026a 067c  .|.........|.j.|
-00000780: 017c 0464 068d 027d 0a09 007c 0a6a 0744  .|.d...}...|.j.D
-00000790: 005d 097d 0b7c 007c 0b7c 027c 0383 0356  .].}.|.|.|.|...V
-000007a0: 0001 0071 377c 0a6a 0872 4e7c 026a 067c  ...q7|.j.rN|.j.|
-000007b0: 017c 047c 0a6a 0864 088d 037d 0a6e 0264  .|.|.j.d...}.n.d
-000007c0: 0053 0071 3429 094e 720b 0000 007a 2361  .S.q4).Nr....z#a
-000007d0: 7265 206e 6f74 206b 6e6f 776e 2061 7474  re not known att
-000007e0: 7269 6275 7465 7320 6f66 2044 6174 6173  ributes of Datas
-000007f0: 6574 7a23 6973 206e 6f74 2061 206b 6e6f  etz#is not a kno
-00000800: 776e 2061 7474 7269 6275 7465 206f 6620  wn attribute of 
-00000810: 4461 7461 7365 74da 0120 7a14 2e20 4b6e  Dataset.. z.. Kn
-00000820: 6f77 6e20 6174 7472 6962 7574 6573 3a20  own attributes: 
-00000830: 2901 721a 0000 0054 2902 721a 0000 00da  ).r....T).r.....
-00000840: 0a70 6167 655f 746f 6b65 6e29 09da 0373  .page_token)...s
-00000850: 6574 7211 0000 00da 0a5f 5f66 6965 6c64  etr......__field
-00000860: 735f 5fda 046b 6579 73da 036c 656e da0a  s__..keys..len..
-00000870: 5661 6c75 6545 7272 6f72 5a0e 7175 6572  ValueErrorZ.quer
-00000880: 795f 6461 7461 7365 7473 da05 6974 656d  y_datasets..item
-00000890: 73da 0a6e 6578 745f 746f 6b65 6e29 0c72  s..next_token).r
-000008a0: 2100 0000 7228 0000 0072 1700 0000 721e  !...r(...r....r.
-000008b0: 0000 0072 1a00 0000 da0a 6b6e 6f77 6e5f  ...r......known_
-000008c0: 6b65 7973 da0b 6163 7475 616c 5f6b 6579  keys..actual_key
-000008d0: 73da 0c75 6e6b 6e6f 776e 5f6b 6579 73da  s..unknown_keys.
-000008e0: 0670 6c75 7261 6cda 036d 7367 da11 7061  .plural..msg..pa
-000008f0: 6769 6e61 7465 645f 7265 7375 6c74 7372  ginated_resultsr
-00000900: 2200 0000 7223 0000 0072 2300 0000 7224  "...r#...r#...r$
-00000910: 0000 00da 0571 7565 7279 3900 0000 732a  .....query9...s*
-00000920: 0000 0002 800e 080c 0108 0104 010c 0102  ................
-00000930: 0306 ff02 0202 fd18 050e 0202 010a 0110  ................
-00000940: 0106 0104 0108 0108 ff04 0402 f87a 0d44  .............z.D
-00000950: 6174 6173 6574 2e71 7565 7279 7222 0000  ataset.queryr"..
-00000960: 00da 0864 656c 6567 6174 6563 0400 0000  ...delegatec....
-00000970: 0000 0000 0000 0000 0400 0000 0200 0000  ................
-00000980: 4300 0000 7316 0000 007c 027c 005f 007c  C...s....|.|._.|
-00000990: 037c 005f 017c 017c 005f 0264 0053 0072  .|._.|.|._.d.S.r
-000009a0: 2000 0000 2903 7213 0000 0072 1500 0000   ...).r....r....
-000009b0: 7214 0000 0029 04da 0473 656c 6672 2200  r....)...selfr".
-000009c0: 0000 7239 0000 0072 1e00 0000 7223 0000  ..r9...r....r#..
-000009d0: 0072 2300 0000 7224 0000 00da 085f 5f69  .r#...r$.....__i
-000009e0: 6e69 745f 5f58 0000 0073 0600 0000 0606  nit__X...s......
-000009f0: 0601 0a01 7a10 4461 7461 7365 742e 5f5f  ....z.Dataset.__
-00000a00: 696e 6974 5f5f da08 6f75 745f 7061 7468  init__..out_path
-00000a10: da10 696e 636c 7564 655f 7061 7474 6572  ..include_patter
-00000a20: 6e73 da10 6578 636c 7564 655f 7061 7474  ns..exclude_patt
-00000a30: 6572 6e73 6304 0000 0000 0000 0000 0000  ernsc...........
-00000a40: 0008 0000 0005 0000 0043 0000 0073 9000  .........C...s..
-00000a50: 0000 7c00 6a00 6a01 7402 6a03 6b03 730e  ..|.j.j.t.j.k.s.
-00000a60: 7c00 6a00 6a04 7405 6a06 6b03 7212 7407  |.j.j.t.j.k.r.t.
-00000a70: 6401 8301 8201 7c01 a008 a100 731c 7c01  d.....|.....s.|.
-00000a80: 6a09 6402 6403 8d01 0100 7c00 a00a 740b  j.d.d.....|...t.
-00000a90: 6a0c a101 7d04 7c00 6a0d 6404 7501 722a  j...}.|.j.d.u.r*
-00000aa0: 7c00 6a0d 6e06 740e 7c04 6a0f 7c04 6405  |.j.n.t.|.j.|.d.
-00000ab0: 8d02 7d05 7c00 a010 7c02 7c03 a102 4400  ..}.|...|.|...D.
-00000ac0: 5d0e 7d06 7c01 7c06 6a11 1b00 7d07 7c05  ].}.|.|.j...}.|.
-00000ad0: a012 7c06 6a13 7c07 a102 0100 7137 6404  ..|.j.|.....q7d.
-00000ae0: 5300 2906 613f 0200 000a 2020 2020 2020  S.).a?....      
-00000af0: 2020 446f 776e 6c6f 6164 2066 696c 6573    Download files
-00000b00: 2061 7373 6f63 6961 7465 6420 7769 7468   associated with
-00000b10: 2074 6869 7320 6461 7461 7365 7420 746f   this dataset to
-00000b20: 2074 6865 2067 6976 656e 2064 6972 6563   the given direc
-00000b30: 746f 7279 2e0a 2020 2020 2020 2020 4966  tory..        If
-00000b40: 2060 6f75 745f 7061 7468 6020 646f 6573   `out_path` does
-00000b50: 206e 6f74 2065 7869 7374 2c20 6974 2077   not exist, it w
-00000b60: 696c 6c20 6265 2063 7265 6174 6564 2e0a  ill be created..
-00000b70: 0a20 2020 2020 2020 2060 696e 636c 7564  .        `includ
-00000b80: 655f 7061 7474 6572 6e73 6020 616e 6420  e_patterns` and 
-00000b90: 6065 7863 6c75 6465 5f70 6174 7465 726e  `exclude_pattern
-00000ba0: 7360 2061 7265 206c 6973 7473 206f 6620  s` are lists of 
-00000bb0: 6769 7469 676e 6f72 652d 7374 796c 6520  gitignore-style 
-00000bc0: 7061 7474 6572 6e73 2e0a 2020 2020 2020  patterns..      
-00000bd0: 2020 5365 6520 6874 7470 733a 2f2f 6769    See https://gi
-00000be0: 742d 7363 6d2e 636f 6d2f 646f 6373 2f67  t-scm.com/docs/g
-00000bf0: 6974 6967 6e6f 7265 2e0a 0a20 2020 2020  itignore...     
-00000c00: 2020 2045 7861 6d70 6c65 3a0a 2020 2020     Example:.    
-00000c10: 2020 2020 6060 600a 2020 2020 2020 2020      ```.        
-00000c20: 6461 7461 7365 7420 3d20 6461 7461 7365  dataset = datase
-00000c30: 7473 2e44 6174 6173 6574 2e62 795f 6964  ts.Dataset.by_id
-00000c40: 2822 3c64 6174 6173 6574 5f69 643e 222c  ("<dataset_id>",
-00000c50: 2064 6174 6173 6574 5f64 656c 6567 6174   dataset_delegat
-00000c60: 6529 0a20 2020 2020 2020 2064 6174 6173  e).        datas
-00000c70: 6574 2e64 6f77 6e6c 6f61 645f 6669 6c65  et.download_file
-00000c80: 7328 0a20 2020 2020 2020 2020 2020 2070  s(.            p
-00000c90: 6174 686c 6962 2e50 6174 6828 222f 746d  athlib.Path("/tm
-00000ca0: 702f 746d 702e 6e56 3167 6457 3557 4856  p/tmp.nV1gdW5WHV
-00000cb0: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
-00000cc0: 696e 636c 7564 655f 7061 7474 6572 6e73  include_patterns
-00000cd0: 3d5b 222a 2a2f 2a2e 6734 225d 2c0a 2020  =["**/*.g4"],.  
-00000ce0: 2020 2020 2020 2020 2020 6578 636c 7564            exclud
-00000cf0: 655f 7061 7474 6572 6e73 3d5b 222a 2a2f  e_patterns=["**/
-00000d00: 7465 7374 2f2a 2a22 5d0a 2020 2020 2020  test/**"].      
-00000d10: 2020 290a 2020 2020 2020 2020 6060 600a    ).        ```.
-00000d20: 2020 2020 2020 2020 fa48 4f6e 6c79 2053          .HOnly S
-00000d30: 332d 6261 636b 6564 2073 746f 7261 6765  3-backed storage
-00000d40: 2061 646d 696e 6973 7465 7265 6420 6279   administered by
-00000d50: 2052 6f62 6f74 6f20 6973 2073 7570 706f   Roboto is suppo
-00000d60: 7274 6564 2061 7420 7468 6973 2074 696d  rted at this tim
-00000d70: 652e 5429 01da 0770 6172 656e 7473 4ea9  e.T)...parentsN.
-00000d80: 02da 0b62 7563 6b65 745f 6e61 6d65 da0b  ...bucket_name..
-00000d90: 6372 6564 656e 7469 616c 7329 1472 1400  credentials).r..
-00000da0: 0000 7219 0000 0072 0f00 0000 da02 5333  ..r....r......S3
-00000db0: 7218 0000 0072 1000 0000 da06 526f 626f  r....r......Robo
-00000dc0: 746f da13 4e6f 7449 6d70 6c65 6d65 6e74  to..NotImplement
-00000dd0: 6564 4572 726f 72da 0669 735f 6469 72da  edError..is_dir.
-00000de0: 056d 6b64 6972 da19 6765 745f 7465 6d70  .mkdir..get_temp
-00000df0: 6f72 6172 795f 6372 6564 656e 7469 616c  orary_credential
-00000e00: 7372 0c00 0000 da08 5265 6164 4f6e 6c79  sr......ReadOnly
-00000e10: 7215 0000 0072 0900 0000 da06 6275 636b  r....r......buck
-00000e20: 6574 da0a 6c69 7374 5f66 696c 6573 da0d  et..list_files..
-00000e30: 7265 6c61 7469 7665 5f70 6174 68da 0d64  relative_path..d
-00000e40: 6f77 6e6c 6f61 645f 6669 6c65 da03 6b65  ownload_file..ke
-00000e50: 7929 0872 3a00 0000 723c 0000 0072 3d00  y).r:...r<...r=.
-00000e60: 0000 723e 0000 0072 4300 0000 721e 0000  ..r>...rC...r...
-00000e70: 00da 0466 696c 655a 0a6c 6f63 616c 5f70  ...fileZ.local_p
-00000e80: 6174 6872 2300 0000 7223 0000 0072 2400  athr#...r#...r$.
-00000e90: 0000 da0e 646f 776e 6c6f 6164 5f66 696c  ....download_fil
-00000ea0: 6573 6200 0000 7326 0000 000e 180e 0102  esb...s&........
-00000eb0: 0202 0104 ff08 040c 010c 020a 0306 ff02  ................
-00000ec0: 0204 0102 0104 fe02 fd10 080a 0110 0104  ................
-00000ed0: fe7a 1644 6174 6173 6574 2e64 6f77 6e6c  .z.Dataset.downl
-00000ee0: 6f61 645f 6669 6c65 73da 046d 6f64 65da  oad_files..mode.
-00000ef0: 0663 616c 6c65 7263 0300 0000 0000 0000  .callerc........
-00000f00: 0000 0000 0300 0000 0500 0000 4300 0000  ............C...
-00000f10: 732e 0000 007c 006a 0064 0075 0073 0a7c  s....|.j.d.u.s.|
-00000f20: 006a 00a0 01a1 0072 147c 006a 02a0 037c  .j.....r.|.j...|
-00000f30: 006a 047c 017c 02a1 037c 005f 007c 006a  .j.|.|...|._.|.j
-00000f40: 0053 0072 2000 0000 2905 7216 0000 00da  .S.r ...).r.....
-00000f50: 0a69 735f 6578 7069 7265 6472 1300 0000  .is_expiredr....
-00000f60: 7249 0000 0072 1400 0000 2903 723a 0000  rI...r....).r:..
-00000f70: 0072 5200 0000 7253 0000 0072 2300 0000  .rR...rS...r#...
-00000f80: 7223 0000 0072 2400 0000 7249 0000 0091  r#...r$...rI....
-00000f90: 0000 0073 0a00 0000 1405 0601 0801 06ff  ...s............
-00000fa0: 0603 7a21 4461 7461 7365 742e 6765 745f  ..z!Dataset.get_
-00000fb0: 7465 6d70 6f72 6172 795f 6372 6564 656e  temporary_creden
-00000fc0: 7469 616c 7363 0300 0000 0000 0000 0000  tialsc..........
-00000fd0: 0000 0800 0000 0500 0000 6300 0000 73ba  ..........c...s.
-00000fe0: 0000 0081 0064 017d 037c 0164 0175 0172  .....d.}.|.d.u.r
-00000ff0: 1074 006a 01a0 0274 006a 036a 047c 01a1  .t.j...t.j.j.|..
-00001000: 027d 0364 017d 047c 0264 0175 0172 1c74  .}.d.}.|.d.u.r.t
-00001010: 006a 05a0 027c 02a1 017d 047c 006a 06a0  .j...|...}.|.j..
-00001020: 077c 006a 086a 097c 006a 086a 0aa1 027d  .|.j.j.|.j.j...}
-00001030: 0509 007c 056a 0b44 005d 1d7d 0674 0c7c  ...|.j.D.].}.t.|
-00001040: 0683 017d 077c 0372 3b7c 03a0 0d7c 076a  ...}.|.r;|...|.j
-00001050: 0ea1 0173 3b09 0071 2b7c 0472 457c 04a0  ...s;..q+|.rE|..
-00001060: 0d7c 076a 0ea1 0172 4509 0071 2b7c 0756  .|.j...rE..q+|.V
-00001070: 0001 0071 2b7c 056a 0f72 5a7c 006a 06a0  ...q+|.j.rZ|.j..
-00001080: 077c 006a 086a 097c 006a 086a 0a7c 056a  .|.j.j.|.j.j.|.j
-00001090: 0fa1 037d 056e 0264 0153 0071 2829 027a  ...}.n.d.S.q().z
-000010a0: 920a 2020 2020 2020 2020 6069 6e63 6c75  ..        `inclu
-000010b0: 6465 5f70 6174 7465 726e 7360 2061 6e64  de_patterns` and
-000010c0: 2060 6578 636c 7564 655f 7061 7474 6572   `exclude_patter
-000010d0: 6e73 6020 6172 6520 6c69 7374 7320 6f66  ns` are lists of
-000010e0: 2067 6974 6967 6e6f 7265 2d73 7479 6c65   gitignore-style
-000010f0: 2070 6174 7465 726e 732e 0a20 2020 2020   patterns..     
-00001100: 2020 2053 6565 2068 7474 7073 3a2f 2f67     See https://g
-00001110: 6974 2d73 636d 2e63 6f6d 2f64 6f63 732f  it-scm.com/docs/
-00001120: 6769 7469 676e 6f72 652e 0a20 2020 2020  gitignore..     
-00001130: 2020 204e 2910 da08 7061 7468 7370 6563     N)...pathspec
-00001140: 5a08 5061 7468 5370 6563 da0a 6672 6f6d  Z.PathSpec..from
-00001150: 5f6c 696e 6573 da08 7061 7474 6572 6e73  _lines..patterns
-00001160: 5a13 4769 7457 696c 644d 6174 6368 5061  Z.GitWildMatchPa
-00001170: 7474 6572 6eda 0d47 6974 4967 6e6f 7265  ttern..GitIgnore
-00001180: 5370 6563 7213 0000 0072 4c00 0000 7214  Specr....rL...r.
-00001190: 0000 0072 2600 0000 721a 0000 0072 3000  ...r&...r....r0.
-000011a0: 0000 7207 0000 00da 0a6d 6174 6368 5f66  ..r......match_f
-000011b0: 696c 6572 4d00 0000 7231 0000 0029 0872  ilerM...r1...).r
-000011c0: 3a00 0000 723d 0000 0072 3e00 0000 5a14  :...r=...r>...Z.
-000011d0: 696e 636c 7564 655f 7061 7474 6572 6e5f  include_pattern_
-000011e0: 7370 6563 5a14 6578 636c 7564 655f 7061  specZ.exclude_pa
-000011f0: 7474 6572 6e5f 7370 6563 7237 0000 0072  ttern_specr7...r
-00001200: 2200 0000 7250 0000 0072 2300 0000 7223  "...rP...r#...r#
-00001210: 0000 0072 2400 0000 724c 0000 009c 0000  ...r$...rL......
-00001220: 0073 4400 0000 0280 0409 0801 0601 0801  .sD.............
-00001230: 04ff 0404 0801 0c01 0602 0c01 04ff 0203  ................
-00001240: 0a01 0801 0801 0401 04ff 0203 0201 0801  ................
-00001250: 0401 04ff 0203 0201 0801 0601 0601 0601  ................
-00001260: 0601 0401 06fd 0406 02eb 7a12 4461 7461  ..........z.Data
-00001270: 7365 742e 6c69 7374 5f66 696c 6573 6301  set.list_filesc.
-00001280: 0000 0000 0000 0000 0000 0001 0000 0002  ................
-00001290: 0000 0043 0000 0073 0a00 0000 7400 7c00  ...C...s....t.|.
-000012a0: 6a01 8301 5300 7220 0000 0029 0272 0500  j...S.r ...).r..
-000012b0: 0000 7214 0000 0029 0172 3a00 0000 7223  ..r....).r:...r#
-000012c0: 0000 0072 2300 0000 7224 0000 00da 0774  ...r#...r$.....t
-000012d0: 6f5f 6469 6374 c900 0000 7302 0000 000a  o_dict....s.....
-000012e0: 017a 0f44 6174 6173 6574 2e74 6f5f 6469  .z.Dataset.to_di
-000012f0: 6374 da0e 6469 7265 6374 6f72 795f 7061  ct..directory_pa
-00001300: 7468 6303 0000 0000 0000 0000 0000 0003  thc.............
-00001310: 0000 0006 0000 0003 0000 0073 5c00 0000  ...........s\...
-00001320: 7c01 a000 a100 730b 7401 7c01 9b00 6401  |.....s.t.|...d.
-00001330: 9d02 8301 8201 6402 8901 7c02 6402 7501  ......d...|.d.u.
-00001340: 7217 7402 6a03 a004 7c02 a101 8901 6403  r.t.j...|.....d.
-00001350: 7405 6a06 6404 7407 6405 6402 6606 8700  t.j.d.t.d.d.f...
-00001360: 8701 8702 6603 6406 6407 840c 8900 8800  ....f.d.d.......
-00001370: 7c01 6408 8302 0100 6402 5300 2909 6122  |.d.....d.S.).a"
-00001380: 0200 000a 2020 2020 2020 2020 5570 6c6f  ....        Uplo
-00001390: 6164 2065 7665 7279 7468 696e 672c 2072  ad everything, r
-000013a0: 6563 7572 7369 7665 6c79 2c20 696e 2064  ecursively, in d
-000013b0: 6972 6563 746f 7279 2c20 6967 6e6f 7269  irectory, ignori
-000013c0: 6e67 2066 696c 6573 2074 6861 7420 6d61  ng files that ma
-000013d0: 7463 6820 616e 7920 6f66 2074 6865 2069  tch any of the i
-000013e0: 676e 6f72 6520 7061 7474 6572 6e73 2e0a  gnore patterns..
-000013f0: 0a20 2020 2020 2020 2060 6578 636c 7564  .        `exclud
-00001400: 655f 7061 7474 6572 6e73 6020 6973 2061  e_patterns` is a
-00001410: 206c 6973 7420 6f66 2067 6974 6967 6e6f   list of gitigno
-00001420: 7265 2d73 7479 6c65 2070 6174 7465 726e  re-style pattern
-00001430: 732e 0a20 2020 2020 2020 2053 6565 2068  s..        See h
-00001440: 7474 7073 3a2f 2f67 6974 2d73 636d 2e63  ttps://git-scm.c
-00001450: 6f6d 2f64 6f63 732f 6769 7469 676e 6f72  om/docs/gitignor
-00001460: 6523 5f70 6174 7465 726e 5f66 6f72 6d61  e#_pattern_forma
-00001470: 742e 0a0a 2020 2020 2020 2020 4578 616d  t...        Exam
-00001480: 706c 653a 0a20 2020 2020 2020 2060 6060  ple:.        ```
-00001490: 0a20 2020 2020 2020 2064 6174 6173 6574  .        dataset
-000014a0: 2e75 706c 6f61 645f 6469 7265 6374 6f72  .upload_director
-000014b0: 7928 0a20 2020 2020 2020 2020 2020 2070  y(.            p
-000014c0: 6174 686c 6962 2e50 6174 6828 222f 7061  athlib.Path("/pa
-000014d0: 7468 2f74 6f2f 6469 7265 6374 6f72 7922  th/to/directory"
-000014e0: 292c 0a20 2020 2020 2020 2020 2020 2065  ),.            e
-000014f0: 7863 6c75 6465 5f70 6174 7465 726e 733d  xclude_patterns=
-00001500: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
-00001510: 2020 225f 5f70 7963 6163 6865 5f5f 2f22    "__pycache__/"
-00001520: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001530: 2020 222a 2e70 7963 222c 0a20 2020 2020    "*.pyc",.     
-00001540: 2020 2020 2020 2020 2020 2022 6e6f 6465             "node
-00001550: 5f6d 6f64 756c 6573 2f22 2c0a 2020 2020  _modules/",.    
-00001560: 2020 2020 2020 2020 2020 2020 222a 2a2f              "**/
-00001570: 2a2e 6c6f 6722 2c0a 2020 2020 2020 2020  *.log",.        
-00001580: 2020 2020 5d2c 0a20 2020 2020 2020 2029      ],.        )
-00001590: 0a20 2020 2020 2020 2060 6060 0a20 2020  .        ```.   
-000015a0: 2020 2020 207a 1320 6973 206e 6f74 2061       z. is not a
-000015b0: 2064 6972 6563 746f 7279 4e72 5b00 0000   directoryNr[...
-000015c0: da0a 6b65 795f 7072 6566 6978 721f 0000  ..key_prefixr...
-000015d0: 0063 0200 0000 0000 0000 0000 0000 0300  .c..............
-000015e0: 0000 0700 0000 1300 0000 735e 0000 007c  ..........s^...|
-000015f0: 00a0 00a1 0044 005d 287d 027c 02a0 01a1  .....D.](}.|....
-00001600: 0072 1688 007c 027c 019b 0064 017c 026a  .r...|.|...d.|.j
-00001610: 029b 009d 0383 0201 0071 0488 0164 0075  .........q...d.u
-00001620: 0172 2088 01a0 037c 02a1 0172 2071 0488  .r ....|...r q..
-00001630: 02a0 047c 027c 019b 0064 017c 026a 029b  ...|.|...d.|.j..
-00001640: 009d 03a1 0201 0071 0464 0053 0029 024e  .......q.d.S.).N
-00001650: fa01 2f29 05da 0769 7465 7264 6972 7247  ../)...iterdirrG
-00001660: 0000 00da 046e 616d 6572 5900 0000 da0b  .....namerY.....
-00001670: 7570 6c6f 6164 5f66 696c 6529 0372 5b00  upload_file).r[.
-00001680: 0000 725c 0000 00da 0470 6174 68a9 03da  ..r\.....path...
-00001690: 115f 7570 6c6f 6164 5f64 6972 6563 746f  ._upload_directo
-000016a0: 7279 5a0c 6578 636c 7564 655f 7370 6563  ryZ.exclude_spec
-000016b0: 723a 0000 0072 2300 0000 7224 0000 0072  r:...r#...r$...r
-000016c0: 6300 0000 ed00 0000 730e 0000 000c 0108  c.......s.......
-000016d0: 0118 0112 0202 011a 0104 fa7a 3344 6174  ...........z3Dat
-000016e0: 6173 6574 2e75 706c 6f61 645f 6469 7265  aset.upload_dire
-000016f0: 6374 6f72 792e 3c6c 6f63 616c 733e 2e5f  ctory.<locals>._
-00001700: 7570 6c6f 6164 5f64 6972 6563 746f 7279  upload_directory
-00001710: da00 2908 7247 0000 0072 2f00 0000 7255  ..).rG...r/...rU
-00001720: 0000 0072 5800 0000 7256 0000 00da 0770  ...rX...rV.....p
-00001730: 6174 686c 6962 da04 5061 7468 da03 7374  athlib..Path..st
-00001740: 7229 0372 3a00 0000 725b 0000 0072 3e00  r).r:...r[...r>.
-00001750: 0000 7223 0000 0072 6200 0000 7224 0000  ..r#...rb...r$..
-00001760: 00da 1075 706c 6f61 645f 6469 7265 6374  ...upload_direct
-00001770: 6f72 79cc 0000 0073 1200 0000 0818 0e01  ory....s........
-00001780: 0402 0801 0601 0201 04ff 2004 0e09 7a18  .......... ...z.
-00001790: 4461 7461 7365 742e 7570 6c6f 6164 5f64  Dataset.upload_d
-000017a0: 6972 6563 746f 7279 da0f 6c6f 6361 6c5f  irectory..local_
-000017b0: 6669 6c65 5f70 6174 6872 4f00 0000 6303  file_pathrO...c.
-000017c0: 0000 0000 0000 0000 0000 0005 0000 0009  ................
-000017d0: 0000 0043 0000 0073 aa00 0000 7c01 a000  ...C...s....|...
-000017e0: a100 730b 7401 7c01 9b00 6401 9d02 8301  ..s.t.|...d.....
-000017f0: 8201 7c00 6a02 6a03 7404 6a05 6b03 7319  ..|.j.j.t.j.k.s.
-00001800: 7c00 6a02 6a06 7407 6a08 6b03 721d 7409  |.j.j.t.j.k.r.t.
-00001810: 6402 8301 8201 7c00 a00a 740b 6a0c a101  d.....|...t.j...
-00001820: 7d03 7c00 6a0d 6403 7501 722b 7c00 6a0d  }.|.j.d.u.r+|.j.
-00001830: 6e06 740e 7c03 6a0f 7c03 6404 8d02 7d04  n.t.|.j.|.d...}.
-00001840: 7c03 6a10 9b00 6405 7c02 a011 6405 a101  |.j...d.|...d...
-00001850: 9b00 9d03 7d02 7c04 6a12 7c01 7c02 7413  ....}.|.j.|.|.t.
-00001860: 6a14 7c00 6a02 6a15 7413 6a16 7c00 6a02  j.|.j.j.t.j.|.j.
-00001870: 6a17 7413 6a18 7c03 6a10 6903 6406 8d03  j.t.j.|.j.i.d...
-00001880: 0100 6403 5300 2907 611c 0100 000a 2020  ..d.S.).a.....  
-00001890: 2020 2020 2020 5570 6c6f 6164 7320 6120        Uploads a 
-000018a0: 6669 6c65 2074 6f20 7468 6520 6461 7461  file to the data
-000018b0: 7365 7427 7320 7374 6f72 6167 6520 6c6f  set's storage lo
-000018c0: 6361 7469 6f6e 2e0a 0a20 2020 2020 2020  cation...       
-000018d0: 203a 7061 7261 6d20 6669 6c65 5f70 6174   :param file_pat
-000018e0: 683a 2054 6865 2070 6174 6820 746f 2074  h: The path to t
-000018f0: 6865 2066 696c 6520 746f 2075 706c 6f61  he file to uploa
-00001900: 642e 0a20 2020 2020 2020 203a 7061 7261  d..        :para
-00001910: 6d20 6b65 793a 2054 6865 206b 6579 2074  m key: The key t
-00001920: 6f20 7573 6520 666f 7220 7468 6520 6669  o use for the fi
-00001930: 6c65 2069 6e20 7468 6520 6461 7461 7365  le in the datase
-00001940: 7427 7320 7374 6f72 6167 6520 6c6f 6361  t's storage loca
-00001950: 7469 6f6e 2e0a 2020 2020 2020 2020 2020  tion..          
-00001960: 2020 2020 2020 2020 2020 4974 2077 696c            It wil
-00001970: 6c20 6265 2070 7265 6669 7865 6420 7769  l be prefixed wi
-00001980: 7468 2074 6865 2064 6174 6173 6574 2773  th the dataset's
-00001990: 2073 746f 7261 6765 2070 7265 6669 782e   storage prefix.
-000019a0: 0a20 2020 2020 2020 207a 0e20 6973 206e  .        z. is n
-000019b0: 6f74 2061 2066 696c 6572 3f00 0000 4e72  ot a filer?...Nr
-000019c0: 4100 0000 725d 0000 0029 0172 1d00 0000  A...r]...).r....
-000019d0: 2919 da07 6973 5f66 696c 6572 2f00 0000  )...is_filer/...
-000019e0: 7214 0000 0072 1900 0000 720f 0000 0072  r....r....r....r
-000019f0: 4400 0000 7218 0000 0072 1000 0000 7245  D...r....r....rE
-00001a00: 0000 0072 4600 0000 7249 0000 0072 0c00  ...rF...rI...r..
-00001a10: 0000 5a09 5265 6164 5772 6974 6572 1500  ..Z.ReadWriter..
-00001a20: 0000 7209 0000 0072 4b00 0000 5a0f 7265  ..r....rK...Z.re
-00001a30: 7175 6972 6564 5f70 7265 6669 78da 066c  quired_prefix..l
-00001a40: 7374 7269 7072 6000 0000 720a 0000 005a  stripr`...r....Z
-00001a50: 0944 6174 6173 6574 4964 7226 0000 00da  .DatasetIdr&....
-00001a60: 054f 7267 4964 721a 0000 005a 0c43 6f6d  .OrgIdr....Z.Com
-00001a70: 6d6f 6e50 7265 6669 7829 0572 3a00 0000  monPrefix).r:...
-00001a80: 7269 0000 0072 4f00 0000 7243 0000 0072  ri...rO...rC...r
-00001a90: 1e00 0000 7223 0000 0072 2300 0000 7224  ....r#...r#...r$
-00001aa0: 0000 0072 6000 0000 f800 0000 7330 0000  ...r`.......s0..
-00001ab0: 0008 0c0e 010e 030e 0102 0202 0104 ff0c  ................
-00001ac0: 040a 0306 ff02 0204 0102 0104 fe02 fd16  ................
-00001ad0: 0804 0102 0102 010a 020a 0108 0102 fd0a  ................
-00001ae0: fd7a 1344 6174 6173 6574 2e75 706c 6f61  .z.Dataset.uploa
-00001af0: 645f 6669 6c65 2902 4e4e 7220 0000 0029  d_file).NNr ...)
-00001b00: 26da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  &..__name__..__m
-00001b10: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00001b20: 616d 655f 5f72 0e00 0000 da0f 5f5f 616e  ame__r......__an
-00001b30: 6e6f 7461 7469 6f6e 735f 5f72 1100 0000  notations__r....
-00001b40: 7215 0000 0072 0300 0000 7208 0000 0072  r....r....r....r
-00001b50: 1600 0000 720d 0000 00da 0b63 6c61 7373  ....r......class
-00001b60: 6d65 7468 6f64 7210 0000 0072 4500 0000  methodr....rE...
-00001b70: 720f 0000 0072 4400 0000 7267 0000 00da  r....rD...rg....
-00001b80: 0464 6963 7472 0200 0000 da04 6c69 7374  .dictr......list
-00001b90: 7225 0000 0072 2700 0000 da0b 636f 6c6c  r%...r'.....coll
-00001ba0: 6563 7469 6f6e 73da 0361 6263 da09 4765  ections..abc..Ge
-00001bb0: 6e65 7261 746f 7272 3800 0000 723b 0000  neratorr8...r;..
-00001bc0: 0072 6500 0000 7266 0000 0072 5100 0000  .re...rf...rQ...
-00001bd0: 720c 0000 0072 4a00 0000 7249 0000 0072  r....rJ...rI...r
-00001be0: 0700 0000 724c 0000 0072 5a00 0000 7268  ....rL...rZ...rh
-00001bf0: 0000 0072 6000 0000 7223 0000 0072 2300  ...r`...r#...r#.
-00001c00: 0000 7223 0000 0072 2400 0000 7212 0000  ..r#...r$...r...
-00001c10: 0017 0000 0073 e600 0000 0a00 0801 0801  .....s..........
-00001c20: 1001 1001 0202 0404 0401 0201 0201 0201  ................
-00001c30: 0201 0201 04f7 0202 02fe 0203 02fd 0204  ................
-00001c40: 02fc 0605 02fb 0606 02fa 0e07 02f9 0a08  ................
-00001c50: 02f8 0609 02f7 020a 0cf6 0210 0205 0201  ................
-00001c60: 04fb 0202 02fe 0203 02fd 0604 02fc 0605  ................
-00001c70: 02fb 0206 0cfa 020a 0205 0201 04fb 0a02  ................
-00001c80: 02fe 0203 02fd 0604 02fc 0605 02fb 0a06  ................
-00001c90: 0cfa 0222 04fc 0202 02fe 0203 02fd 0604  ..."............
-00001ca0: 02fc 0205 0afb 020d 0201 04fc 0402 02fe  ................
-00001cb0: 0a03 02fd 0a04 02fc 0205 0afb 0431 0201  .............1..
-00001cc0: 04fd 0202 02fe 0603 02fd 0204 0afc 020d  ................
-00001cd0: 0201 04fd 0a02 02fe 0a03 02fd 1004 0afc  ................
-00001ce0: 162d 0206 04fd 0402 02fe 0a03 02fd 0204  .-..............
-00001cf0: 0afc 022c 0402 02fe 0203 02fd 0204 0efc  ...,............
-00001d00: 7212 0000 0029 17da 0f63 6f6c 6c65 6374  r....)...collect
-00001d10: 696f 6e73 2e61 6263 7274 0000 0072 6500  ions.abcrt...re.
-00001d20: 0000 da06 7479 7069 6e67 7202 0000 0072  ....typingr....r
-00001d30: 0300 0000 7255 0000 00da 0573 6572 6465  ....rU.....serde
-00001d40: 7205 0000 00da 0566 696c 6573 7207 0000  r......filesr...
-00001d50: 0072 0800 0000 7209 0000 0072 0a00 0000  .r....r....r....
-00001d60: 7239 0000 0072 0c00 0000 720d 0000 0072  r9...r....r....r
-00001d70: 0e00 0000 720f 0000 0072 2200 0000 7210  ....r....r"...r.
-00001d80: 0000 0072 1100 0000 7212 0000 0072 2300  ...r....r....r#.
-00001d90: 0000 7223 0000 0072 2300 0000 7224 0000  ..r#...r#...r$..
-00001da0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00001db0: 1200 0000 0800 0801 1001 0802 0c02 1801  ................
-00001dc0: 1806 1006 1203                           ......
+000002d0: 5a1a 651b 640e 6510 6602 641c 641d 8404  Z.e.d.e.f.d.d...
+000002e0: 8301 5a1c 0903 0903 6432 641e 651d 6a1e  ..Z.....d2d.e.j.
+000002f0: 641f 6507 6513 6510 1900 1900 6420 6507  d.e.e.e.....d e.
+00000300: 6513 6510 1900 1900 640e 6403 6608 6421  e.e.....d.d.f.d!
+00000310: 6422 8405 5a1f 6520 6a21 6403 6602 6423  d"..Z.e j!d.f.d#
+00000320: 6520 6424 6507 6510 1900 640e 650a 6606  e d$e.e...d.e.f.
+00000330: 6425 6426 8405 5a22 0903 0903 6432 641f  d%d&..Z"....d2d.
+00000340: 6507 6513 6510 1900 1900 6420 6507 6513  e.e.e.....d e.e.
+00000350: 6510 1900 1900 640e 6516 6a17 6a18 6523  e.....d.e.j.j.e#
+00000360: 6403 6403 6603 1900 6606 6427 6428 8405  d.d.f...f.d'd(..
+00000370: 5a24 640e 6511 6510 6512 6602 1900 6602  Z$d.e.e.e.f...f.
+00000380: 6429 642a 8404 5a25 0903 6433 642b 651d  d)d*..Z%..d3d+e.
+00000390: 6a1e 6420 6507 6513 6510 1900 1900 640e  j.d e.e.e.....d.
+000003a0: 6403 6606 642c 642d 8405 5a26 642e 651d  d.f.d,d-..Z&d.e.
+000003b0: 6a1e 642f 6510 640e 6403 6606 6430 6431  j.d/e.d.d.f.d0d1
+000003c0: 8404 5a27 6403 5300 2934 da07 4461 7461  ..Z'd.S.)4..Data
+000003d0: 7365 74da 125f 4461 7461 7365 745f 5f64  set.._Dataset__d
+000003e0: 656c 6567 6174 65da 105f 4461 7461 7365  elegate.._Datase
+000003f0: 745f 5f72 6563 6f72 644e da18 5f44 6174  t__recordN.._Dat
+00000400: 6173 6574 5f5f 6669 6c65 735f 6465 6c65  aset__files_dele
+00000410: 6761 7465 da1a 5f44 6174 6173 6574 5f5f  gate.._Dataset__
+00000420: 7465 6d70 5f63 7265 6465 6e74 6961 6c73  temp_credentials
+00000430: da10 6461 7461 7365 745f 6465 6c65 6761  ..dataset_delega
+00000440: 7465 da0d 6164 6d69 6e69 7374 7261 746f  te..administrato
+00000450: 72da 1073 746f 7261 6765 5f6c 6f63 6174  r..storage_locat
+00000460: 696f 6eda 066f 7267 5f69 64da 0a63 7265  ion..org_id..cre
+00000470: 6174 6564 5f62 79da 086d 6574 6164 6174  ated_by..metadat
+00000480: 61da 0474 6167 73da 0e66 696c 6573 5f64  a..tags..files_d
+00000490: 656c 6567 6174 65da 0672 6574 7572 6e63  elegate..returnc
+000004a0: 0900 0000 0000 0000 0000 0000 0a00 0000  ................
+000004b0: 0800 0000 4300 0000 7320 0000 007c 01a0  ....C...s ...|..
+000004c0: 007c 027c 067c 037c 077c 047c 05a1 067d  .|.|.|.|.|.|...}
+000004d0: 097c 007c 097c 017c 0883 0353 00a9 014e  .|.|.|.|...S...N
+000004e0: 2901 5a0e 6372 6561 7465 5f64 6174 6173  ).Z.create_datas
+000004f0: 6574 290a da03 636c 7372 1700 0000 7218  et)...clsr....r.
+00000500: 0000 0072 1900 0000 721a 0000 0072 1b00  ...r....r....r..
+00000510: 0000 721c 0000 0072 1d00 0000 721e 0000  ..r....r....r...
+00000520: 00da 0672 6563 6f72 64a9 0072 2300 0000  ...record..r#...
+00000530: faef 2f63 6f64 6562 7569 6c64 2f6f 7574  ../codebuild/out
+00000540: 7075 742f 7372 6333 3537 3831 3132 3139  put/src357811219
+00000550: 312f 7372 632f 636f 6465 7374 6172 2d63  1/src/codestar-c
+00000560: 6f6e 6e65 6374 696f 6e73 2e75 732d 7765  onnections.us-we
+00000570: 7374 2d32 2e61 6d61 7a6f 6e61 7773 2e63  st-2.amazonaws.c
+00000580: 6f6d 2f67 6974 2d68 7474 702f 3036 3631  om/git-http/0661
+00000590: 3935 3131 3233 3835 2f75 732d 7765 7374  95112385/us-west
+000005a0: 2d32 2f65 3635 3032 6138 302d 6262 3465  -2/e6502a80-bb4e
+000005b0: 2d34 6662 652d 3837 3263 2d35 6434 3263  -4fbe-872c-5d42c
+000005c0: 3139 3336 3939 642f 726f 626f 746f 2d61  193699d/roboto-a
+000005d0: 692f 726f 626f 746f 2d68 6f73 7465 642d  i/roboto-hosted-
+000005e0: 6170 702f 7061 636b 6167 6573 2f72 6f62  app/packages/rob
+000005f0: 6f74 6f5f 7364 6b2f 7372 632f 726f 626f  oto_sdk/src/robo
+00000600: 746f 5f73 646b 2f64 6f6d 6169 6e2f 6461  to_sdk/domain/da
+00000610: 7461 7365 7473 2f64 6174 6173 6574 2e70  tasets/dataset.p
+00000620: 79da 0663 7265 6174 651d 0000 0073 0800  y..create....s..
+00000630: 0000 040c 0c01 04ff 0c03 7a0e 4461 7461  ..........z.Data
+00000640: 7365 742e 6372 6561 7465 da0a 6461 7461  set.create..data
+00000650: 7365 745f 6964 6305 0000 0000 0000 0000  set_idc.........
+00000660: 0000 0006 0000 0004 0000 0043 0000 0073  ...........C...s
+00000670: 1800 0000 7c02 a000 7c01 7c03 a102 7d05  ....|...|.|...}.
+00000680: 7c00 7c05 7c02 7c04 8303 5300 7220 0000  |.|.|.|...S.r ..
+00000690: 0029 015a 1a67 6574 5f64 6174 6173 6574  .).Z.get_dataset
+000006a0: 5f62 795f 7072 696d 6172 795f 6b65 7929  _by_primary_key)
+000006b0: 0672 2100 0000 7226 0000 0072 1700 0000  .r!...r&...r....
+000006c0: 721a 0000 0072 1e00 0000 7222 0000 0072  r....r....r"...r
+000006d0: 2300 0000 7223 0000 0072 2400 0000 da07  #...r#...r$.....
+000006e0: 6672 6f6d 5f69 642e 0000 0073 0400 0000  from_id....s....
+000006f0: 0c08 0c01 7a0f 4461 7461 7365 742e 6672  ....z.Dataset.fr
+00000700: 6f6d 5f69 64da 0766 696c 7465 7273 2903  om_id..filters).
+00000710: 7212 0000 004e 4e63 0500 0000 0000 0000  r....NNc........
+00000720: 0000 0000 0c00 0000 0600 0000 6300 0000  ............c...
+00000730: 73a2 0000 0081 0074 0074 016a 02a0 03a1  s......t.t.j....
+00000740: 0083 017d 0574 007c 01a0 03a1 0083 017d  ...}.t.|.......}
+00000750: 067c 067c 0518 007d 077c 0772 2c74 047c  .|.|...}.|.r,t.|
+00000760: 0783 0164 016b 047d 087c 0872 1e64 026e  ...d.k.}.|.r.d.n
+00000770: 0164 037d 0974 057c 079b 0064 047c 099b  .d.}.t.|...d.|..
+00000780: 0064 057c 059b 009d 0583 0182 017c 026a  .d.|.........|.j
+00000790: 067c 017c 0464 068d 027d 0a09 007c 0a6a  .|.|.d...}...|.j
+000007a0: 0744 005d 097d 0b7c 007c 0b7c 027c 0383  .D.].}.|.|.|.|..
+000007b0: 0356 0001 0071 377c 0a6a 0872 4e7c 026a  .V...q7|.j.rN|.j
+000007c0: 067c 017c 047c 0a6a 0864 088d 037d 0a6e  .|.|.|.j.d...}.n
+000007d0: 0264 0053 0071 3429 094e 720b 0000 007a  .d.S.q4).Nr....z
+000007e0: 2361 7265 206e 6f74 206b 6e6f 776e 2061  #are not known a
+000007f0: 7474 7269 6275 7465 7320 6f66 2044 6174  ttributes of Dat
+00000800: 6173 6574 7a23 6973 206e 6f74 2061 206b  asetz#is not a k
+00000810: 6e6f 776e 2061 7474 7269 6275 7465 206f  nown attribute o
+00000820: 6620 4461 7461 7365 74da 0120 7a14 2e20  f Dataset.. z.. 
+00000830: 4b6e 6f77 6e20 6174 7472 6962 7574 6573  Known attributes
+00000840: 3a20 2901 721a 0000 0054 2902 721a 0000  : ).r....T).r...
+00000850: 00da 0a70 6167 655f 746f 6b65 6e29 09da  ...page_token)..
+00000860: 0373 6574 7211 0000 00da 0a5f 5f66 6965  .setr......__fie
+00000870: 6c64 735f 5fda 046b 6579 73da 036c 656e  lds__..keys..len
+00000880: da0a 5661 6c75 6545 7272 6f72 5a0e 7175  ..ValueErrorZ.qu
+00000890: 6572 795f 6461 7461 7365 7473 da05 6974  ery_datasets..it
+000008a0: 656d 73da 0a6e 6578 745f 746f 6b65 6e29  ems..next_token)
+000008b0: 0c72 2100 0000 7228 0000 0072 1700 0000  .r!...r(...r....
+000008c0: 721e 0000 0072 1a00 0000 da0a 6b6e 6f77  r....r......know
+000008d0: 6e5f 6b65 7973 da0b 6163 7475 616c 5f6b  n_keys..actual_k
+000008e0: 6579 73da 0c75 6e6b 6e6f 776e 5f6b 6579  eys..unknown_key
+000008f0: 73da 0670 6c75 7261 6cda 036d 7367 da11  s..plural..msg..
+00000900: 7061 6769 6e61 7465 645f 7265 7375 6c74  paginated_result
+00000910: 7372 2200 0000 7223 0000 0072 2300 0000  sr"...r#...r#...
+00000920: 7224 0000 00da 0571 7565 7279 3900 0000  r$.....query9...
+00000930: 732a 0000 0002 800e 080c 0108 0104 010c  s*..............
+00000940: 0102 0306 ff02 0202 fd18 050e 0202 010a  ................
+00000950: 0110 0106 0104 0108 0108 ff04 0402 f87a  ...............z
+00000960: 0d44 6174 6173 6574 2e71 7565 7279 7222  .Dataset.queryr"
+00000970: 0000 00da 0864 656c 6567 6174 6563 0400  .....delegatec..
+00000980: 0000 0000 0000 0000 0000 0400 0000 0200  ................
+00000990: 0000 4300 0000 7316 0000 007c 027c 005f  ..C...s....|.|._
+000009a0: 007c 037c 005f 017c 017c 005f 0264 0053  .|.|._.|.|._.d.S
+000009b0: 0072 2000 0000 2903 7213 0000 0072 1500  .r ...).r....r..
+000009c0: 0000 7214 0000 0029 04da 0473 656c 6672  ..r....)...selfr
+000009d0: 2200 0000 7239 0000 0072 1e00 0000 7223  "...r9...r....r#
+000009e0: 0000 0072 2300 0000 7224 0000 00da 085f  ...r#...r$....._
+000009f0: 5f69 6e69 745f 5f58 0000 0073 0600 0000  _init__X...s....
+00000a00: 0606 0601 0a01 7a10 4461 7461 7365 742e  ......z.Dataset.
+00000a10: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
+00000a20: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
+00000a30: 0073 0800 0000 7c00 6a00 6a01 5300 7220  .s....|.j.j.S.r 
+00000a40: 0000 0029 0272 1400 0000 7226 0000 00a9  ...).r....r&....
+00000a50: 0172 3a00 0000 7223 0000 0072 2300 0000  .r:...r#...r#...
+00000a60: 7224 0000 0072 2600 0000 6200 0000 7302  r$...r&...b...s.
+00000a70: 0000 0008 027a 1244 6174 6173 6574 2e64  .....z.Dataset.d
+00000a80: 6174 6173 6574 5f69 64da 086f 7574 5f70  ataset_id..out_p
+00000a90: 6174 68da 1069 6e63 6c75 6465 5f70 6174  ath..include_pat
+00000aa0: 7465 726e 73da 1065 7863 6c75 6465 5f70  terns..exclude_p
+00000ab0: 6174 7465 726e 7363 0400 0000 0000 0000  atternsc........
+00000ac0: 0000 0000 0800 0000 0500 0000 4300 0000  ............C...
+00000ad0: 7390 0000 007c 006a 006a 0174 026a 036b  s....|.j.j.t.j.k
+00000ae0: 0373 0e7c 006a 006a 0474 056a 066b 0372  .s.|.j.j.t.j.k.r
+00000af0: 1274 0764 0183 0182 017c 01a0 08a1 0073  .t.d.....|.....s
+00000b00: 1c7c 016a 0964 0264 038d 0101 007c 00a0  .|.j.d.d.....|..
+00000b10: 0a74 0b6a 0ca1 017d 047c 006a 0d64 0475  .t.j...}.|.j.d.u
+00000b20: 0172 2a7c 006a 0d6e 0674 0e7c 046a 0f7c  .r*|.j.n.t.|.j.|
+00000b30: 0464 058d 027d 057c 00a0 107c 027c 03a1  .d...}.|...|.|..
+00000b40: 0244 005d 0e7d 067c 017c 066a 111b 007d  .D.].}.|.|.j...}
+00000b50: 077c 05a0 127c 066a 137c 07a1 0201 0071  .|...|.j.|.....q
+00000b60: 3764 0453 0029 0661 3f02 0000 0a20 2020  7d.S.).a?....   
+00000b70: 2020 2020 2044 6f77 6e6c 6f61 6420 6669       Download fi
+00000b80: 6c65 7320 6173 736f 6369 6174 6564 2077  les associated w
+00000b90: 6974 6820 7468 6973 2064 6174 6173 6574  ith this dataset
+00000ba0: 2074 6f20 7468 6520 6769 7665 6e20 6469   to the given di
+00000bb0: 7265 6374 6f72 792e 0a20 2020 2020 2020  rectory..       
+00000bc0: 2049 6620 606f 7574 5f70 6174 6860 2064   If `out_path` d
+00000bd0: 6f65 7320 6e6f 7420 6578 6973 742c 2069  oes not exist, i
+00000be0: 7420 7769 6c6c 2062 6520 6372 6561 7465  t will be create
+00000bf0: 642e 0a0a 2020 2020 2020 2020 6069 6e63  d...        `inc
+00000c00: 6c75 6465 5f70 6174 7465 726e 7360 2061  lude_patterns` a
+00000c10: 6e64 2060 6578 636c 7564 655f 7061 7474  nd `exclude_patt
+00000c20: 6572 6e73 6020 6172 6520 6c69 7374 7320  erns` are lists 
+00000c30: 6f66 2067 6974 6967 6e6f 7265 2d73 7479  of gitignore-sty
+00000c40: 6c65 2070 6174 7465 726e 732e 0a20 2020  le patterns..   
+00000c50: 2020 2020 2053 6565 2068 7474 7073 3a2f       See https:/
+00000c60: 2f67 6974 2d73 636d 2e63 6f6d 2f64 6f63  /git-scm.com/doc
+00000c70: 732f 6769 7469 676e 6f72 652e 0a0a 2020  s/gitignore...  
+00000c80: 2020 2020 2020 4578 616d 706c 653a 0a20        Example:. 
+00000c90: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
+00000ca0: 2020 2064 6174 6173 6574 203d 2064 6174     dataset = dat
+00000cb0: 6173 6574 732e 4461 7461 7365 742e 6279  asets.Dataset.by
+00000cc0: 5f69 6428 223c 6461 7461 7365 745f 6964  _id("<dataset_id
+00000cd0: 3e22 2c20 6461 7461 7365 745f 6465 6c65  >", dataset_dele
+00000ce0: 6761 7465 290a 2020 2020 2020 2020 6461  gate).        da
+00000cf0: 7461 7365 742e 646f 776e 6c6f 6164 5f66  taset.download_f
+00000d00: 696c 6573 280a 2020 2020 2020 2020 2020  iles(.          
+00000d10: 2020 7061 7468 6c69 622e 5061 7468 2822    pathlib.Path("
+00000d20: 2f74 6d70 2f74 6d70 2e6e 5631 6764 5735  /tmp/tmp.nV1gdW5
+00000d30: 5748 5622 292c 0a20 2020 2020 2020 2020  WHV"),.         
+00000d40: 2020 2069 6e63 6c75 6465 5f70 6174 7465     include_patte
+00000d50: 726e 733d 5b22 2a2a 2f2a 2e67 3422 5d2c  rns=["**/*.g4"],
+00000d60: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
+00000d70: 6c75 6465 5f70 6174 7465 726e 733d 5b22  lude_patterns=["
+00000d80: 2a2a 2f74 6573 742f 2a2a 225d 0a20 2020  **/test/**"].   
+00000d90: 2020 2020 2029 0a20 2020 2020 2020 2060       ).        `
+00000da0: 6060 0a20 2020 2020 2020 20fa 484f 6e6c  ``.        .HOnl
+00000db0: 7920 5333 2d62 6163 6b65 6420 7374 6f72  y S3-backed stor
+00000dc0: 6167 6520 6164 6d69 6e69 7374 6572 6564  age administered
+00000dd0: 2062 7920 526f 626f 746f 2069 7320 7375   by Roboto is su
+00000de0: 7070 6f72 7465 6420 6174 2074 6869 7320  pported at this 
+00000df0: 7469 6d65 2e54 2901 da07 7061 7265 6e74  time.T)...parent
+00000e00: 734e a902 da0b 6275 636b 6574 5f6e 616d  sN....bucket_nam
+00000e10: 65da 0b63 7265 6465 6e74 6961 6c73 2914  e..credentials).
+00000e20: 7214 0000 0072 1900 0000 720f 0000 00da  r....r....r.....
+00000e30: 0253 3372 1800 0000 7210 0000 00da 0652  .S3r....r......R
+00000e40: 6f62 6f74 6fda 134e 6f74 496d 706c 656d  oboto..NotImplem
+00000e50: 656e 7465 6445 7272 6f72 da06 6973 5f64  entedError..is_d
+00000e60: 6972 da05 6d6b 6469 72da 1967 6574 5f74  ir..mkdir..get_t
+00000e70: 656d 706f 7261 7279 5f63 7265 6465 6e74  emporary_credent
+00000e80: 6961 6c73 720c 0000 00da 0852 6561 644f  ialsr......ReadO
+00000e90: 6e6c 7972 1500 0000 7209 0000 00da 0662  nlyr....r......b
+00000ea0: 7563 6b65 74da 0a6c 6973 745f 6669 6c65  ucket..list_file
+00000eb0: 73da 0d72 656c 6174 6976 655f 7061 7468  s..relative_path
+00000ec0: da0d 646f 776e 6c6f 6164 5f66 696c 65da  ..download_file.
+00000ed0: 036b 6579 2908 723a 0000 0072 3d00 0000  .key).r:...r=...
+00000ee0: 723e 0000 0072 3f00 0000 7244 0000 0072  r>...r?...rD...r
+00000ef0: 1e00 0000 da04 6669 6c65 5a0a 6c6f 6361  ......fileZ.loca
+00000f00: 6c5f 7061 7468 7223 0000 0072 2300 0000  l_pathr#...r#...
+00000f10: 7224 0000 00da 0e64 6f77 6e6c 6f61 645f  r$.....download_
+00000f20: 6669 6c65 7366 0000 0073 2600 0000 0e18  filesf...s&.....
+00000f30: 0e01 0202 0201 04ff 0804 0c01 0c02 0a03  ................
+00000f40: 06ff 0202 0401 0201 04fe 02fd 1008 0a01  ................
+00000f50: 1001 04fe 7a16 4461 7461 7365 742e 646f  ....z.Dataset.do
+00000f60: 776e 6c6f 6164 5f66 696c 6573 da04 6d6f  wnload_files..mo
+00000f70: 6465 da06 6361 6c6c 6572 6303 0000 0000  de..callerc.....
+00000f80: 0000 0000 0000 0003 0000 0005 0000 0043  ...............C
+00000f90: 0000 0073 2e00 0000 7c00 6a00 6400 7500  ...s....|.j.d.u.
+00000fa0: 730a 7c00 6a00 a001 a100 7214 7c00 6a02  s.|.j.....r.|.j.
+00000fb0: a003 7c00 6a04 7c01 7c02 a103 7c00 5f00  ..|.j.|.|...|._.
+00000fc0: 7c00 6a00 5300 7220 0000 0029 0572 1600  |.j.S.r ...).r..
+00000fd0: 0000 da0a 6973 5f65 7870 6972 6564 7213  ....is_expiredr.
+00000fe0: 0000 0072 4a00 0000 7214 0000 0029 0372  ...rJ...r....).r
+00000ff0: 3a00 0000 7253 0000 0072 5400 0000 7223  :...rS...rT...r#
+00001000: 0000 0072 2300 0000 7224 0000 0072 4a00  ...r#...r$...rJ.
+00001010: 0000 9500 0000 730a 0000 0014 0506 0108  ......s.........
+00001020: 0106 ff06 037a 2144 6174 6173 6574 2e67  .....z!Dataset.g
+00001030: 6574 5f74 656d 706f 7261 7279 5f63 7265  et_temporary_cre
+00001040: 6465 6e74 6961 6c73 6303 0000 0000 0000  dentialsc.......
+00001050: 0000 0000 0008 0000 0005 0000 0063 0000  .............c..
+00001060: 0073 ba00 0000 8100 6401 7d03 7c01 6401  .s......d.}.|.d.
+00001070: 7501 7210 7400 6a01 a002 7400 6a03 6a04  u.r.t.j...t.j.j.
+00001080: 7c01 a102 7d03 6401 7d04 7c02 6401 7501  |...}.d.}.|.d.u.
+00001090: 721c 7400 6a05 a002 7c02 a101 7d04 7c00  r.t.j...|...}.|.
+000010a0: 6a06 a007 7c00 6a08 6a09 7c00 6a08 6a0a  j...|.j.j.|.j.j.
+000010b0: a102 7d05 0900 7c05 6a0b 4400 5d1d 7d06  ..}...|.j.D.].}.
+000010c0: 740c 7c06 8301 7d07 7c03 723b 7c03 a00d  t.|...}.|.r;|...
+000010d0: 7c07 6a0e a101 733b 0900 712b 7c04 7245  |.j...s;..q+|.rE
+000010e0: 7c04 a00d 7c07 6a0e a101 7245 0900 712b  |...|.j...rE..q+
+000010f0: 7c07 5600 0100 712b 7c05 6a0f 725a 7c00  |.V...q+|.j.rZ|.
+00001100: 6a06 a007 7c00 6a08 6a09 7c00 6a08 6a0a  j...|.j.j.|.j.j.
+00001110: 7c05 6a0f a103 7d05 6e02 6401 5300 7128  |.j...}.n.d.S.q(
+00001120: 2902 7a92 0a20 2020 2020 2020 2060 696e  ).z..        `in
+00001130: 636c 7564 655f 7061 7474 6572 6e73 6020  clude_patterns` 
+00001140: 616e 6420 6065 7863 6c75 6465 5f70 6174  and `exclude_pat
+00001150: 7465 726e 7360 2061 7265 206c 6973 7473  terns` are lists
+00001160: 206f 6620 6769 7469 676e 6f72 652d 7374   of gitignore-st
+00001170: 796c 6520 7061 7474 6572 6e73 2e0a 2020  yle patterns..  
+00001180: 2020 2020 2020 5365 6520 6874 7470 733a        See https:
+00001190: 2f2f 6769 742d 7363 6d2e 636f 6d2f 646f  //git-scm.com/do
+000011a0: 6373 2f67 6974 6967 6e6f 7265 2e0a 2020  cs/gitignore..  
+000011b0: 2020 2020 2020 4e29 10da 0870 6174 6873        N)...paths
+000011c0: 7065 635a 0850 6174 6853 7065 63da 0a66  pecZ.PathSpec..f
+000011d0: 726f 6d5f 6c69 6e65 73da 0870 6174 7465  rom_lines..patte
+000011e0: 726e 735a 1347 6974 5769 6c64 4d61 7463  rnsZ.GitWildMatc
+000011f0: 6850 6174 7465 726e da0d 4769 7449 676e  hPattern..GitIgn
+00001200: 6f72 6553 7065 6372 1300 0000 724d 0000  oreSpecr....rM..
+00001210: 0072 1400 0000 7226 0000 0072 1a00 0000  .r....r&...r....
+00001220: 7230 0000 0072 0700 0000 da0a 6d61 7463  r0...r......matc
+00001230: 685f 6669 6c65 724e 0000 0072 3100 0000  h_filerN...r1...
+00001240: 2908 723a 0000 0072 3e00 0000 723f 0000  ).r:...r>...r?..
+00001250: 005a 1469 6e63 6c75 6465 5f70 6174 7465  .Z.include_patte
+00001260: 726e 5f73 7065 635a 1465 7863 6c75 6465  rn_specZ.exclude
+00001270: 5f70 6174 7465 726e 5f73 7065 6372 3700  _pattern_specr7.
+00001280: 0000 7222 0000 0072 5100 0000 7223 0000  ..r"...rQ...r#..
+00001290: 0072 2300 0000 7224 0000 0072 4d00 0000  .r#...r$...rM...
+000012a0: a000 0000 7344 0000 0002 8004 0908 0106  ....sD..........
+000012b0: 0108 0104 ff04 0408 010c 0106 020c 0104  ................
+000012c0: ff02 030a 0108 0108 0104 0104 ff02 0302  ................
+000012d0: 0108 0104 0104 ff02 0302 0108 0106 0106  ................
+000012e0: 0106 0106 0104 0106 fd04 0602 eb7a 1244  .............z.D
+000012f0: 6174 6173 6574 2e6c 6973 745f 6669 6c65  ataset.list_file
+00001300: 7363 0100 0000 0000 0000 0000 0000 0100  sc..............
+00001310: 0000 0200 0000 4300 0000 730a 0000 0074  ......C...s....t
+00001320: 007c 006a 0183 0153 0072 2000 0000 2902  .|.j...S.r ...).
+00001330: 7205 0000 0072 1400 0000 723c 0000 0072  r....r....r<...r
+00001340: 2300 0000 7223 0000 0072 2400 0000 da07  #...r#...r$.....
+00001350: 746f 5f64 6963 74cd 0000 0073 0200 0000  to_dict....s....
+00001360: 0a01 7a0f 4461 7461 7365 742e 746f 5f64  ..z.Dataset.to_d
+00001370: 6963 74da 0e64 6972 6563 746f 7279 5f70  ict..directory_p
+00001380: 6174 6863 0300 0000 0000 0000 0000 0000  athc............
+00001390: 0300 0000 0600 0000 0300 0000 735c 0000  ............s\..
+000013a0: 007c 01a0 00a1 0073 0b74 017c 019b 0064  .|.....s.t.|...d
+000013b0: 019d 0283 0182 0164 0289 017c 0264 0275  .......d...|.d.u
+000013c0: 0172 1774 026a 03a0 047c 02a1 0189 0164  .r.t.j...|.....d
+000013d0: 0374 056a 0664 0474 0764 0564 0266 0687  .t.j.d.t.d.d.f..
+000013e0: 0087 0187 0266 0364 0664 0784 0c89 0088  .....f.d.d......
+000013f0: 007c 0164 0883 0201 0064 0253 0029 0961  .|.d.....d.S.).a
+00001400: 2202 0000 0a20 2020 2020 2020 2055 706c  "....        Upl
+00001410: 6f61 6420 6576 6572 7974 6869 6e67 2c20  oad everything, 
+00001420: 7265 6375 7273 6976 656c 792c 2069 6e20  recursively, in 
+00001430: 6469 7265 6374 6f72 792c 2069 676e 6f72  directory, ignor
+00001440: 696e 6720 6669 6c65 7320 7468 6174 206d  ing files that m
+00001450: 6174 6368 2061 6e79 206f 6620 7468 6520  atch any of the 
+00001460: 6967 6e6f 7265 2070 6174 7465 726e 732e  ignore patterns.
+00001470: 0a0a 2020 2020 2020 2020 6065 7863 6c75  ..        `exclu
+00001480: 6465 5f70 6174 7465 726e 7360 2069 7320  de_patterns` is 
+00001490: 6120 6c69 7374 206f 6620 6769 7469 676e  a list of gitign
+000014a0: 6f72 652d 7374 796c 6520 7061 7474 6572  ore-style patter
+000014b0: 6e73 2e0a 2020 2020 2020 2020 5365 6520  ns..        See 
+000014c0: 6874 7470 733a 2f2f 6769 742d 7363 6d2e  https://git-scm.
+000014d0: 636f 6d2f 646f 6373 2f67 6974 6967 6e6f  com/docs/gitigno
+000014e0: 7265 235f 7061 7474 6572 6e5f 666f 726d  re#_pattern_form
+000014f0: 6174 2e0a 0a20 2020 2020 2020 2045 7861  at...        Exa
+00001500: 6d70 6c65 3a0a 2020 2020 2020 2020 6060  mple:.        ``
+00001510: 600a 2020 2020 2020 2020 6461 7461 7365  `.        datase
+00001520: 742e 7570 6c6f 6164 5f64 6972 6563 746f  t.upload_directo
+00001530: 7279 280a 2020 2020 2020 2020 2020 2020  ry(.            
+00001540: 7061 7468 6c69 622e 5061 7468 2822 2f70  pathlib.Path("/p
+00001550: 6174 682f 746f 2f64 6972 6563 746f 7279  ath/to/directory
+00001560: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
+00001570: 6578 636c 7564 655f 7061 7474 6572 6e73  exclude_patterns
+00001580: 3d5b 0a20 2020 2020 2020 2020 2020 2020  =[.             
+00001590: 2020 2022 5f5f 7079 6361 6368 655f 5f2f     "__pycache__/
+000015a0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000015b0: 2020 2022 2a2e 7079 6322 2c0a 2020 2020     "*.pyc",.    
+000015c0: 2020 2020 2020 2020 2020 2020 226e 6f64              "nod
+000015d0: 655f 6d6f 6475 6c65 732f 222c 0a20 2020  e_modules/",.   
+000015e0: 2020 2020 2020 2020 2020 2020 2022 2a2a               "**
+000015f0: 2f2a 2e6c 6f67 222c 0a20 2020 2020 2020  /*.log",.       
+00001600: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
+00001610: 290a 2020 2020 2020 2020 6060 600a 2020  ).        ```.  
+00001620: 2020 2020 2020 7a13 2069 7320 6e6f 7420        z. is not 
+00001630: 6120 6469 7265 6374 6f72 794e 725c 0000  a directoryNr\..
+00001640: 00da 0a6b 6579 5f70 7265 6669 7872 1f00  ...key_prefixr..
+00001650: 0000 6302 0000 0000 0000 0000 0000 0003  ..c.............
+00001660: 0000 0007 0000 0013 0000 0073 5e00 0000  ...........s^...
+00001670: 7c00 a000 a100 4400 5d28 7d02 7c02 a001  |.....D.](}.|...
+00001680: a100 7216 8800 7c02 7c01 9b00 6401 7c02  ..r...|.|...d.|.
+00001690: 6a02 9b00 9d03 8302 0100 7104 8801 6400  j.........q...d.
+000016a0: 7501 7220 8801 a003 7c02 a101 7220 7104  u.r ....|...r q.
+000016b0: 8802 a004 7c02 7c01 9b00 6401 7c02 6a02  ....|.|...d.|.j.
+000016c0: 9b00 9d03 a102 0100 7104 6400 5300 2902  ........q.d.S.).
+000016d0: 4efa 012f 2905 da07 6974 6572 6469 7272  N../)...iterdirr
+000016e0: 4800 0000 da04 6e61 6d65 725a 0000 00da  H.....namerZ....
+000016f0: 0b75 706c 6f61 645f 6669 6c65 2903 725c  .upload_file).r\
+00001700: 0000 0072 5d00 0000 da04 7061 7468 a903  ...r].....path..
+00001710: da11 5f75 706c 6f61 645f 6469 7265 6374  .._upload_direct
+00001720: 6f72 795a 0c65 7863 6c75 6465 5f73 7065  oryZ.exclude_spe
+00001730: 6372 3a00 0000 7223 0000 0072 2400 0000  cr:...r#...r$...
+00001740: 7264 0000 00f1 0000 0073 0e00 0000 0c01  rd.......s......
+00001750: 0801 1801 1202 0201 1a01 04fa 7a33 4461  ............z3Da
+00001760: 7461 7365 742e 7570 6c6f 6164 5f64 6972  taset.upload_dir
+00001770: 6563 746f 7279 2e3c 6c6f 6361 6c73 3e2e  ectory.<locals>.
+00001780: 5f75 706c 6f61 645f 6469 7265 6374 6f72  _upload_director
+00001790: 79da 0029 0872 4800 0000 722f 0000 0072  y..).rH...r/...r
+000017a0: 5600 0000 7259 0000 0072 5700 0000 da07  V...rY...rW.....
+000017b0: 7061 7468 6c69 62da 0450 6174 68da 0373  pathlib..Path..s
+000017c0: 7472 2903 723a 0000 0072 5c00 0000 723f  tr).r:...r\...r?
+000017d0: 0000 0072 2300 0000 7263 0000 0072 2400  ...r#...rc...r$.
+000017e0: 0000 da10 7570 6c6f 6164 5f64 6972 6563  ....upload_direc
+000017f0: 746f 7279 d000 0000 7312 0000 0008 180e  tory....s.......
+00001800: 0104 0208 0106 0102 0104 ff20 040e 097a  ........... ...z
+00001810: 1844 6174 6173 6574 2e75 706c 6f61 645f  .Dataset.upload_
+00001820: 6469 7265 6374 6f72 79da 0f6c 6f63 616c  directory..local
+00001830: 5f66 696c 655f 7061 7468 7250 0000 0063  _file_pathrP...c
+00001840: 0300 0000 0000 0000 0000 0000 0500 0000  ................
+00001850: 0900 0000 4300 0000 73aa 0000 007c 01a0  ....C...s....|..
+00001860: 00a1 0073 0b74 017c 019b 0064 019d 0283  ...s.t.|...d....
+00001870: 0182 017c 006a 026a 0374 046a 056b 0373  ...|.j.j.t.j.k.s
+00001880: 197c 006a 026a 0674 076a 086b 0372 1d74  .|.j.j.t.j.k.r.t
+00001890: 0964 0283 0182 017c 00a0 0a74 0b6a 0ca1  .d.....|...t.j..
+000018a0: 017d 037c 006a 0d64 0375 0172 2b7c 006a  .}.|.j.d.u.r+|.j
+000018b0: 0d6e 0674 0e7c 036a 0f7c 0364 048d 027d  .n.t.|.j.|.d...}
+000018c0: 047c 036a 109b 0064 057c 02a0 1164 05a1  .|.j...d.|...d..
+000018d0: 019b 009d 037d 027c 046a 127c 017c 0274  .....}.|.j.|.|.t
+000018e0: 136a 147c 006a 026a 1574 136a 167c 006a  .j.|.j.j.t.j.|.j
+000018f0: 026a 1774 136a 187c 036a 1069 0364 068d  .j.t.j.|.j.i.d..
+00001900: 0301 0064 0353 0029 0761 1c01 0000 0a20  ...d.S.).a..... 
+00001910: 2020 2020 2020 2055 706c 6f61 6473 2061         Uploads a
+00001920: 2066 696c 6520 746f 2074 6865 2064 6174   file to the dat
+00001930: 6173 6574 2773 2073 746f 7261 6765 206c  aset's storage l
+00001940: 6f63 6174 696f 6e2e 0a0a 2020 2020 2020  ocation...      
+00001950: 2020 3a70 6172 616d 2066 696c 655f 7061    :param file_pa
+00001960: 7468 3a20 5468 6520 7061 7468 2074 6f20  th: The path to 
+00001970: 7468 6520 6669 6c65 2074 6f20 7570 6c6f  the file to uplo
+00001980: 6164 2e0a 2020 2020 2020 2020 3a70 6172  ad..        :par
+00001990: 616d 206b 6579 3a20 5468 6520 6b65 7920  am key: The key 
+000019a0: 746f 2075 7365 2066 6f72 2074 6865 2066  to use for the f
+000019b0: 696c 6520 696e 2074 6865 2064 6174 6173  ile in the datas
+000019c0: 6574 2773 2073 746f 7261 6765 206c 6f63  et's storage loc
+000019d0: 6174 696f 6e2e 0a20 2020 2020 2020 2020  ation..         
+000019e0: 2020 2020 2020 2020 2020 2049 7420 7769             It wi
+000019f0: 6c6c 2062 6520 7072 6566 6978 6564 2077  ll be prefixed w
+00001a00: 6974 6820 7468 6520 6461 7461 7365 7427  ith the dataset'
+00001a10: 7320 7374 6f72 6167 6520 7072 6566 6978  s storage prefix
+00001a20: 2e0a 2020 2020 2020 2020 7a0e 2069 7320  ..        z. is 
+00001a30: 6e6f 7420 6120 6669 6c65 7240 0000 004e  not a filer@...N
+00001a40: 7242 0000 0072 5e00 0000 2901 721d 0000  rB...r^...).r...
+00001a50: 0029 19da 0769 735f 6669 6c65 722f 0000  .)...is_filer/..
+00001a60: 0072 1400 0000 7219 0000 0072 0f00 0000  .r....r....r....
+00001a70: 7245 0000 0072 1800 0000 7210 0000 0072  rE...r....r....r
+00001a80: 4600 0000 7247 0000 0072 4a00 0000 720c  F...rG...rJ...r.
+00001a90: 0000 005a 0952 6561 6457 7269 7465 7215  ...Z.ReadWriter.
+00001aa0: 0000 0072 0900 0000 724c 0000 005a 0f72  ...r....rL...Z.r
+00001ab0: 6571 7569 7265 645f 7072 6566 6978 da06  equired_prefix..
+00001ac0: 6c73 7472 6970 7261 0000 0072 0a00 0000  lstripra...r....
+00001ad0: 5a09 4461 7461 7365 7449 6472 2600 0000  Z.DatasetIdr&...
+00001ae0: da05 4f72 6749 6472 1a00 0000 5a0c 436f  ..OrgIdr....Z.Co
+00001af0: 6d6d 6f6e 5072 6566 6978 2905 723a 0000  mmonPrefix).r:..
+00001b00: 0072 6a00 0000 7250 0000 0072 4400 0000  .rj...rP...rD...
+00001b10: 721e 0000 0072 2300 0000 7223 0000 0072  r....r#...r#...r
+00001b20: 2400 0000 7261 0000 00fc 0000 0073 3000  $...ra.......s0.
+00001b30: 0000 080c 0e01 0e03 0e01 0202 0201 04ff  ................
+00001b40: 0c04 0a03 06ff 0202 0401 0201 04fe 02fd  ................
+00001b50: 1608 0401 0201 0201 0a02 0a01 0801 02fd  ................
+00001b60: 0afd 7a13 4461 7461 7365 742e 7570 6c6f  ..z.Dataset.uplo
+00001b70: 6164 5f66 696c 6529 024e 4e72 2000 0000  ad_file).NNr ...
+00001b80: 2928 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )(..__name__..__
+00001b90: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00001ba0: 6e61 6d65 5f5f 720e 0000 00da 0f5f 5f61  name__r......__a
+00001bb0: 6e6e 6f74 6174 696f 6e73 5f5f 7211 0000  nnotations__r...
+00001bc0: 0072 1500 0000 7203 0000 0072 0800 0000  .r....r....r....
+00001bd0: 7216 0000 0072 0d00 0000 da0b 636c 6173  r....r......clas
+00001be0: 736d 6574 686f 6472 1000 0000 7246 0000  smethodr....rF..
+00001bf0: 0072 0f00 0000 7245 0000 0072 6800 0000  .r....rE...rh...
+00001c00: da04 6469 6374 7202 0000 00da 046c 6973  ..dictr......lis
+00001c10: 7472 2500 0000 7227 0000 00da 0b63 6f6c  tr%...r'.....col
+00001c20: 6c65 6374 696f 6e73 da03 6162 63da 0947  lections..abc..G
+00001c30: 656e 6572 6174 6f72 7238 0000 0072 3b00  eneratorr8...r;.
+00001c40: 0000 da08 7072 6f70 6572 7479 7226 0000  ....propertyr&..
+00001c50: 0072 6600 0000 7267 0000 0072 5200 0000  .rf...rg...rR...
+00001c60: 720c 0000 0072 4b00 0000 724a 0000 0072  r....rK...rJ...r
+00001c70: 0700 0000 724d 0000 0072 5b00 0000 7269  ....rM...r[...ri
+00001c80: 0000 0072 6100 0000 7223 0000 0072 2300  ...ra...r#...r#.
+00001c90: 0000 7223 0000 0072 2400 0000 7212 0000  ..r#...r$...r...
+00001ca0: 0017 0000 0073 ea00 0000 0a00 0801 0801  .....s..........
+00001cb0: 1001 1001 0202 0404 0401 0201 0201 0201  ................
+00001cc0: 0201 0201 04f7 0202 02fe 0203 02fd 0204  ................
+00001cd0: 02fc 0605 02fb 0606 02fa 0e07 02f9 0a08  ................
+00001ce0: 02f8 0609 02f7 020a 0cf6 0210 0205 0201  ................
+00001cf0: 04fb 0202 02fe 0203 02fd 0604 02fc 0605  ................
+00001d00: 02fb 0206 0cfa 020a 0205 0201 04fb 0a02  ................
+00001d10: 02fe 0203 02fd 0604 02fc 0605 02fb 0a06  ................
+00001d20: 0cfa 0222 04fc 0202 02fe 0203 02fd 0604  ..."............
+00001d30: 02fc 0205 0afb 020a 1001 0206 0201 04fc  ................
+00001d40: 0402 02fe 0a03 02fd 0a04 02fc 0205 0afb  ................
+00001d50: 0431 0201 04fd 0202 02fe 0603 02fd 0204  .1..............
+00001d60: 0afc 020d 0201 04fd 0a02 02fe 0a03 02fd  ................
+00001d70: 1004 0afc 162d 0206 04fd 0402 02fe 0a03  .....-..........
+00001d80: 02fd 0204 0afc 022c 0402 02fe 0203 02fd  .......,........
+00001d90: 0204 0efc 7212 0000 0029 17da 0f63 6f6c  ....r....)...col
+00001da0: 6c65 6374 696f 6e73 2e61 6263 7275 0000  lections.abcru..
+00001db0: 0072 6600 0000 da06 7479 7069 6e67 7202  .rf.....typingr.
+00001dc0: 0000 0072 0300 0000 7256 0000 00da 0573  ...r....rV.....s
+00001dd0: 6572 6465 7205 0000 00da 0566 696c 6573  erder......files
+00001de0: 7207 0000 0072 0800 0000 7209 0000 0072  r....r....r....r
+00001df0: 0a00 0000 7239 0000 0072 0c00 0000 720d  ....r9...r....r.
+00001e00: 0000 0072 0e00 0000 720f 0000 0072 2200  ...r....r....r".
+00001e10: 0000 7210 0000 0072 1100 0000 7212 0000  ..r....r....r...
+00001e20: 0072 2300 0000 7223 0000 0072 2300 0000  .r#...r#...r#...
+00001e30: 7224 0000 00da 083c 6d6f 6475 6c65 3e01  r$.....<module>.
+00001e40: 0000 0073 1200 0000 0800 0801 1001 0802  ...s............
+00001e50: 0c02 1801 1806 1006 1203                 ..........
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/__pycache__/delegate.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/datasets/__pycache__/delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 2215 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 a708 0000  o.......1..d....
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 a708 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 ae00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 6d05 5a05 0100 6400 6401 6c06 5a06 6403  m.Z...d.d.l.Z.d.
 00000060: 6404 6c07 6d08 5a08 0100 6403 6405 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6403 6406 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
@@ -28,15 +28,15 @@
 000001b0: 6365 7373 4d6f 6465 da08 5265 6164 4f6e  cessMode..ReadOn
 000001c0: 6c79 da09 5265 6164 5772 6974 654e 2905  ly..ReadWriteN).
 000001d0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
 000001e0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
 000001f0: 6d65 5f5f 7210 0000 0072 1100 0000 a900  me__r....r......
 00000200: 7215 0000 0072 1500 0000 faf0 2f63 6f64  r....r....../cod
 00000210: 6562 7569 6c64 2f6f 7574 7075 742f 7372  ebuild/output/sr
-00000220: 6331 3638 3931 3535 3339 392f 7372 632f  c1689155399/src/
+00000220: 6333 3537 3831 3132 3139 312f 7372 632f  c3578112191/src/
 00000230: 636f 6465 7374 6172 2d63 6f6e 6e65 6374  codestar-connect
 00000240: 696f 6e73 2e75 732d 7765 7374 2d32 2e61  ions.us-west-2.a
 00000250: 6d61 7a6f 6e61 7773 2e63 6f6d 2f67 6974  mazonaws.com/git
 00000260: 2d68 7474 702f 3036 3631 3935 3131 3233  -http/0661951123
 00000270: 3835 2f75 732d 7765 7374 2d32 2f65 3635  85/us-west-2/e65
 00000280: 3032 6138 302d 6262 3465 2d34 6662 652d  02a80-bb4e-4fbe-
 00000290: 3837 3263 2d35 6434 3263 3139 3336 3939  872c-5d42c193699
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/__pycache__/http_delegate.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/datasets/__pycache__/http_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 4911 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 2f13 0000  o.......1..d/...
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 2f13 0000  o..........d/...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6400 6401 6c04 5a05 6403  m.Z...d.d.l.Z.d.
 00000050: 6404 6c06 6d07 5a07 6d08 5a08 6d09 5a09  d.l.m.Z.m.Z.m.Z.
 00000060: 0100 6403 6405 6c0a 6d0b 5a0b 0100 6403  ..d.d.l.m.Z...d.
 00000070: 6406 6c0c 6d0d 5a0d 0100 6407 6408 6c0e  d.l.m.Z...d.d.l.
@@ -66,16 +66,16 @@
 00000410: 0000 0300 0000 731a 0000 0074 0083 00a0  ......s....t....
 00000420: 01a1 0001 007c 027c 005f 027c 017c 005f  .....|.|._.|.|._
 00000430: 0364 0053 00a9 014e 2904 da05 7375 7065  .d.S...N)...supe
 00000440: 72da 085f 5f69 6e69 745f 5f72 1500 0000  r..__init__r....
 00000450: 7216 0000 0029 03da 0473 656c 6672 1700  r....)...selfr..
 00000460: 0000 7218 0000 00a9 01da 095f 5f63 6c61  ..r........__cla
 00000470: 7373 5f5f a900 faf5 2f63 6f64 6562 7569  ss__..../codebui
-00000480: 6c64 2f6f 7574 7075 742f 7372 6331 3638  ld/output/src168
-00000490: 3931 3535 3339 392f 7372 632f 636f 6465  9155399/src/code
+00000480: 6c64 2f6f 7574 7075 742f 7372 6333 3537  ld/output/src357
+00000490: 3831 3132 3139 312f 7372 632f 636f 6465  8112191/src/code
 000004a0: 7374 6172 2d63 6f6e 6e65 6374 696f 6e73  star-connections
 000004b0: 2e75 732d 7765 7374 2d32 2e61 6d61 7a6f  .us-west-2.amazo
 000004c0: 6e61 7773 2e63 6f6d 2f67 6974 2d68 7474  naws.com/git-htt
 000004d0: 702f 3036 3631 3935 3131 3233 3835 2f75  p/066195112385/u
 000004e0: 732d 7765 7374 2d32 2f65 3635 3032 6138  s-west-2/e6502a8
 000004f0: 302d 6262 3465 2d34 6662 652d 3837 3263  0-bb4e-4fbe-872c
 00000500: 2d35 6434 3263 3139 3336 3939 642f 726f  -5d42c193699d/ro
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/__pycache__/http_resources.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/datasets/__pycache__/http_resources.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 340 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 5401 0000  o.......1..dT...
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 5401 0000  o..........dT...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6403 6404 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
 00000050: 0100 4700 6405 6406 8400 6406 6502 6a06  ..G.d.d...d.e.j.
 00000060: 8303 5a07 6402 5300 2907 e900 0000 0029  ..Z.d.S.)......)
 00000070: 01da 0341 6e79 4ee9 0100 0000 2902 da0d  ...AnyN.....)...
@@ -26,15 +26,15 @@
 00000190: 5f72 0400 0000 da0f 5f5f 616e 6e6f 7461  _r......__annota
 000001a0: 7469 6f6e 735f 5f72 0500 0000 da08 7079  tions__r......py
 000001b0: 6461 6e74 6963 da05 4669 656c 64da 0464  dantic..Field..d
 000001c0: 6963 7472 0a00 0000 da03 7374 7272 0200  ictr......strr..
 000001d0: 0000 da04 6c69 7374 720b 0000 00a9 0072  ....listr......r
 000001e0: 1500 0000 7215 0000 00fa f62f 636f 6465  ....r....../code
 000001f0: 6275 696c 642f 6f75 7470 7574 2f73 7263  build/output/src
-00000200: 3136 3839 3135 3533 3939 2f73 7263 2f63  1689155399/src/c
+00000200: 3335 3738 3131 3231 3931 2f73 7263 2f63  3578112191/src/c
 00000210: 6f64 6573 7461 722d 636f 6e6e 6563 7469  odestar-connecti
 00000220: 6f6e 732e 7573 2d77 6573 742d 322e 616d  ons.us-west-2.am
 00000230: 617a 6f6e 6177 732e 636f 6d2f 6769 742d  azonaws.com/git-
 00000240: 6874 7470 2f30 3636 3139 3531 3132 3338  http/06619511238
 00000250: 352f 7573 2d77 6573 742d 322f 6536 3530  5/us-west-2/e650
 00000260: 3261 3830 2d62 6234 652d 3466 6265 2d38  2a80-bb4e-4fbe-8
 00000270: 3732 632d 3564 3432 6331 3933 3639 3964  72c-5d42c193699d
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/__pycache__/record.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/datasets/__pycache__/record.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 867 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 6303 0000  o.......1..dc...
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 6303 0000  o..........dc...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6401 6c04  d.l.m.Z...d.d.l.
 00000050: 5a04 4700 6403 6404 8400 6404 6505 6501  Z.G.d.d...d.e.e.
 00000060: 6a06 8304 5a07 4700 6405 6406 8400 6406  j...Z.G.d.d...d.
 00000070: 6505 6501 6a06 8304 5a08 4700 6407 6408  e.e.j...Z.G.d.d.
@@ -13,15 +13,15 @@
 000000c0: 0164 005a 0264 015a 0364 0253 0029 03da  .d.Z.d.Z.d.S.)..
 000000d0: 0d41 646d 696e 6973 7472 6174 6f72 da06  .Administrator..
 000000e0: 526f 626f 746f 4e29 04da 085f 5f6e 616d  RobotoN)...__nam
 000000f0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
 00000100: 0c5f 5f71 7561 6c6e 616d 655f 5f72 0500  .__qualname__r..
 00000110: 0000 a900 7209 0000 0072 0900 0000 faee  ....r....r......
 00000120: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
-00000130: 742f 7372 6331 3638 3931 3535 3339 392f  t/src1689155399/
+00000130: 742f 7372 6333 3537 3831 3132 3139 312f  t/src3578112191/
 00000140: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
 00000150: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
 00000160: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
 00000170: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
 00000180: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
 00000190: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
 000001a0: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/dataset.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/datasets/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,14 +91,18 @@
         delegate: DatasetDelegate,
         files_delegate: Optional[FileDelegate] = None,
     ) -> None:
         self.__delegate = delegate
         self.__files_delegate = files_delegate
         self.__record = record
 
+    @property
+    def dataset_id(self) -> str:
+        return self.__record.dataset_id
+
     def download_files(
         self,
         out_path: pathlib.Path,
         include_patterns: Optional[list[str]] = None,
         exclude_patterns: Optional[list[str]] = None,
     ) -> None:
         """
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/delegate.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/datasets/delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/http_delegate.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/datasets/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/datasets/record.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/datasets/record.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/files/__pycache__/__init__.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/files/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 436 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 b401 0000  o.......1..d....
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 b401 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6406 6c0c 6d0d 5a0d 0100 6407  ..d.d.l.m.Z...d.
@@ -22,16 +22,16 @@
 00000150: 6572 0400 0000 da0d 6874 7470 5f64 656c  er......http_del
 00000160: 6567 6174 6572 0500 0000 da0e 6874 7470  egater......http
 00000170: 5f72 6573 6f75 7263 6573 7206 0000 0072  _resourcesr....r
 00000180: 0700 0000 da06 7265 636f 7264 7208 0000  ......recordr...
 00000190: 005a 0b73 335f 6465 6c65 6761 7465 7209  .Z.s3_delegater.
 000001a0: 0000 00da 075f 5f61 6c6c 5f5f a900 7210  .....__all__..r.
 000001b0: 0000 0072 1000 0000 faed 2f63 6f64 6562  ...r....../codeb
-000001c0: 7569 6c64 2f6f 7574 7075 742f 7372 6331  uild/output/src1
-000001d0: 3638 3931 3535 3339 392f 7372 632f 636f  689155399/src/co
+000001c0: 7569 6c64 2f6f 7574 7075 742f 7372 6333  uild/output/src3
+000001d0: 3537 3831 3132 3139 312f 7372 632f 636f  578112191/src/co
 000001e0: 6465 7374 6172 2d63 6f6e 6e65 6374 696f  destar-connectio
 000001f0: 6e73 2e75 732d 7765 7374 2d32 2e61 6d61  ns.us-west-2.ama
 00000200: 7a6f 6e61 7773 2e63 6f6d 2f67 6974 2d68  zonaws.com/git-h
 00000210: 7474 702f 3036 3631 3935 3131 3233 3835  ttp/066195112385
 00000220: 2f75 732d 7765 7374 2d32 2f65 3635 3032  /us-west-2/e6502
 00000230: 6138 302d 6262 3465 2d34 6662 652d 3837  a80-bb4e-4fbe-87
 00000240: 3263 2d35 6434 3263 3139 3336 3939 642f  2c-5d42c193699d/
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/files/__pycache__/delegate.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/files/__pycache__/delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 1181 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 9d04 0000  o.......1..d....
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 9d04 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6403 6404 6c05 6d06 5a06 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6405 6406 8400 6406 6501 6a07 8303 5a08  d.d...d.e.j...Z.
 00000070: 4700 6407 6408 8400 6408 6500 6a09 8303  G.d.d...d.e.j...
@@ -17,16 +17,16 @@
 00000100: 6964 5a0d 636f 6d6d 6f6e 5f70 7265 6669  idZ.common_prefi
 00000110: 784e 2906 da08 5f5f 6e61 6d65 5f5f da0a  xN)...__name__..
 00000120: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
 00000130: 616c 6e61 6d65 5f5f da09 4461 7461 7365  alname__..Datase
 00000140: 7449 64da 054f 7267 4964 da0c 436f 6d6d  tId..OrgId..Comm
 00000150: 6f6e 5072 6566 6978 a900 720e 0000 0072  onPrefix..r....r
 00000160: 0e00 0000 faed 2f63 6f64 6562 7569 6c64  ....../codebuild
-00000170: 2f6f 7574 7075 742f 7372 6331 3638 3931  /output/src16891
-00000180: 3535 3339 392f 7372 632f 636f 6465 7374  55399/src/codest
+00000170: 2f6f 7574 7075 742f 7372 6333 3537 3831  /output/src35781
+00000180: 3132 3139 312f 7372 632f 636f 6465 7374  12191/src/codest
 00000190: 6172 2d63 6f6e 6e65 6374 696f 6e73 2e75  ar-connections.u
 000001a0: 732d 7765 7374 2d32 2e61 6d61 7a6f 6e61  s-west-2.amazona
 000001b0: 7773 2e63 6f6d 2f67 6974 2d68 7474 702f  ws.com/git-http/
 000001c0: 3036 3631 3935 3131 3233 3835 2f75 732d  066195112385/us-
 000001d0: 7765 7374 2d32 2f65 3635 3032 6138 302d  west-2/e6502a80-
 000001e0: 6262 3465 2d34 6662 652d 3837 3263 2d35  bb4e-4fbe-872c-5
 000001f0: 6434 3263 3139 3336 3939 642f 726f 626f  d42c193699d/robo
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/files/__pycache__/file.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/files/__pycache__/file.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 802 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 2203 0000  o.......1..d"...
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 2203 0000  o..........d"...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a03 6403 6404 6c04 6d05 5a05 0100 4700  Z.d.d.l.m.Z...G.
 00000050: 6405 6406 8400 6406 8302 5a06 6402 5300  d.d...d...Z.d.S.
 00000060: 2907 e900 0000 0029 01da 084f 7074 696f  )......)...Optio
 00000070: 6e61 6c4e e901 0000 0029 01da 0a46 696c  nalN.....)...Fil
@@ -21,15 +21,15 @@
 00000140: 4669 6c65 5f5f 7061 7273 6564 5f75 7269  File__parsed_uri
 00000150: da06 7265 636f 7264 6302 0000 0000 0000  ..recordc.......
 00000160: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
 00000170: 0073 0a00 0000 7c01 7c00 5f00 6400 5300  .s....|.|._.d.S.
 00000180: a901 4e29 0172 0600 0000 2902 da04 7365  ..N).r....)...se
 00000190: 6c66 7208 0000 00a9 0072 0b00 0000 fae9  lfr......r......
 000001a0: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
-000001b0: 742f 7372 6331 3638 3931 3535 3339 392f  t/src1689155399/
+000001b0: 742f 7372 6333 3537 3831 3132 3139 312f  t/src3578112191/
 000001c0: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
 000001d0: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
 000001e0: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
 000001f0: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
 00000200: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
 00000210: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
 00000220: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/files/__pycache__/http_delegate.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/files/__pycache__/http_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 2166 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 7608 0000  o.......1..dv...
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 7608 0000  o..........dv...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6c00 0000 6400  .....@...sl...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6403 6404 6c03 6d04 5a04 0100 6403  ..d.d.l.m.Z...d.
 00000050: 6405 6c05 6d06 5a06 0100 6406 6407 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 0100 6406 6408 6c0a  m.Z.m.Z...d.d.l.
 00000070: 6d0b 5a0b 6d0c 5a0c 0100 6406 6409 6c0d  m.Z.m.Z...d.d.l.
@@ -56,15 +56,15 @@
 00000370: 0000 0074 0083 00a0 01a1 0001 007c 027c  ...t.........|.|
 00000380: 005f 027c 017c 005f 0364 0053 00a9 014e  ._.|.|._.d.S...N
 00000390: 2904 da05 7375 7065 72da 085f 5f69 6e69  )...super..__ini
 000003a0: 745f 5f72 0d00 0000 720e 0000 0029 03da  t__r....r....)..
 000003b0: 0473 656c 6672 0f00 0000 7210 0000 00a9  .selfr....r.....
 000003c0: 01da 095f 5f63 6c61 7373 5f5f a900 faf2  ...__class__....
 000003d0: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
-000003e0: 742f 7372 6331 3638 3931 3535 3339 392f  t/src1689155399/
+000003e0: 742f 7372 6333 3537 3831 3132 3139 312f  t/src3578112191/
 000003f0: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
 00000400: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
 00000410: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
 00000420: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
 00000430: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
 00000440: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
 00000450: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/files/__pycache__/http_resources.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/files/__pycache__/http_resources.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 168 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 a800 0000  o.......1..d....
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 a800 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3000 0000 6400  .....@...s0...d.
 00000030: 6401 6c00 5a00 4700 6402 6403 8400 6403  d.l.Z.G.d.d...d.
 00000040: 6500 6a01 8303 5a02 4700 6404 6405 8400  e.j...Z.G.d.d...
 00000050: 6405 6500 6a01 8303 5a03 6401 5300 2906  d.e.j...Z.d.S.).
 00000060: e900 0000 004e 6300 0000 0000 0000 0000  .....Nc.........
 00000070: 0000 0000 0000 0003 0000 0040 0000 00f3  ...........@....
@@ -12,15 +12,15 @@
 000000b0: 5265 7175 6573 74da 0662 7563 6b65 74da  Request..bucket.
 000000c0: 036b 6579 4ea9 05da 085f 5f6e 616d 655f  .keyN....__name_
 000000d0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
 000000e0: 5f71 7561 6c6e 616d 655f 5fda 0373 7472  _qualname__..str
 000000f0: da0f 5f5f 616e 6e6f 7461 7469 6f6e 735f  ..__annotations_
 00000100: 5fa9 0072 0c00 0000 720c 0000 00fa f32f  _..r....r....../
 00000110: 636f 6465 6275 696c 642f 6f75 7470 7574  codebuild/output
-00000120: 2f73 7263 3136 3839 3135 3533 3939 2f73  /src1689155399/s
+00000120: 2f73 7263 3335 3738 3131 3231 3931 2f73  /src3578112191/s
 00000130: 7263 2f63 6f64 6573 7461 722d 636f 6e6e  rc/codestar-conn
 00000140: 6563 7469 6f6e 732e 7573 2d77 6573 742d  ections.us-west-
 00000150: 322e 616d 617a 6f6e 6177 732e 636f 6d2f  2.amazonaws.com/
 00000160: 6769 742d 6874 7470 2f30 3636 3139 3531  git-http/0661951
 00000170: 3132 3338 352f 7573 2d77 6573 742d 322f  12385/us-west-2/
 00000180: 6536 3530 3261 3830 2d62 6234 652d 3466  e6502a80-bb4e-4f
 00000190: 6265 2d38 3732 632d 3564 3432 6331 3933  be-872c-5d42c193
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/files/__pycache__/record.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/files/__pycache__/record.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 382 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 7e01 0000  o.......1..d~...
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 7e01 0000  o..........d~...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 4700  d.l.Z.d.d.l.Z.G.
 00000040: 6402 6403 8400 6403 6501 6a02 8303 5a03  d.d...d.e.j...Z.
 00000050: 6401 5300 2904 e900 0000 004e 6300 0000  d.S.)......Nc...
 00000060: 0000 0000 0000 0000 0000 0000 0003 0000  ................
 00000070: 0040 0000 0073 4000 0000 6500 5a01 6400  .@...s@...e.Z.d.
@@ -17,15 +17,15 @@
 00000100: 0375 7269 4e29 07da 085f 5f6e 616d 655f  .uriN)...__name_
 00000110: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
 00000120: 5f71 7561 6c6e 616d 655f 5fda 0373 7472  _qualname__..str
 00000130: da0f 5f5f 616e 6e6f 7461 7469 6f6e 735f  ..__annotations_
 00000140: 5fda 0864 6174 6574 696d 65da 0369 6e74  _..datetime..int
 00000150: a900 720f 0000 0072 0f00 0000 faeb 2f63  ..r....r....../c
 00000160: 6f64 6562 7569 6c64 2f6f 7574 7075 742f  odebuild/output/
-00000170: 7372 6331 3638 3931 3535 3339 392f 7372  src1689155399/sr
+00000170: 7372 6333 3537 3831 3132 3139 312f 7372  src3578112191/sr
 00000180: 632f 636f 6465 7374 6172 2d63 6f6e 6e65  c/codestar-conne
 00000190: 6374 696f 6e73 2e75 732d 7765 7374 2d32  ctions.us-west-2
 000001a0: 2e61 6d61 7a6f 6e61 7773 2e63 6f6d 2f67  .amazonaws.com/g
 000001b0: 6974 2d68 7474 702f 3036 3631 3935 3131  it-http/06619511
 000001c0: 3233 3835 2f75 732d 7765 7374 2d32 2f65  2385/us-west-2/e
 000001d0: 3635 3032 6138 302d 6262 3465 2d34 6662  6502a80-bb4e-4fb
 000001e0: 652d 3837 3263 2d35 6434 3263 3139 3336  e-872c-5d42c1936
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/files/__pycache__/s3_delegate.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/files/__pycache__/s3_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 2358 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 3609 0000  o.......1..d6...
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 3609 0000  o..........d6...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6c00 0000 6400  .....@...sl...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6401 6c05  m.Z.m.Z...d.d.l.
 00000050: 5a06 6400 6401 6c07 5a07 6403 6404 6c08  Z.d.d.l.Z.d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6403 6405 6c0b  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 4700 6406 6407 8400 6407  m.Z...G.d.d...d.
@@ -22,16 +22,16 @@
 00000150: 6563 7265 745f 6163 6365 7373 5f6b 6579  ecret_access_key
 00000160: da0d 7365 7373 696f 6e5f 746f 6b65 6e4e  ..session_tokenN
 00000170: 2905 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
 00000180: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
 00000190: 6e61 6d65 5f5f da03 7374 72da 0f5f 5f61  name__..str..__a
 000001a0: 6e6e 6f74 6174 696f 6e73 5f5f a900 7212  nnotations__..r.
 000001b0: 0000 0072 1200 0000 faf0 2f63 6f64 6562  ...r....../codeb
-000001c0: 7569 6c64 2f6f 7574 7075 742f 7372 6331  uild/output/src1
-000001d0: 3638 3931 3535 3339 392f 7372 632f 636f  689155399/src/co
+000001c0: 7569 6c64 2f6f 7574 7075 742f 7372 6333  uild/output/src3
+000001d0: 3537 3831 3132 3139 312f 7372 632f 636f  578112191/src/co
 000001e0: 6465 7374 6172 2d63 6f6e 6e65 6374 696f  destar-connectio
 000001f0: 6e73 2e75 732d 7765 7374 2d32 2e61 6d61  ns.us-west-2.ama
 00000200: 7a6f 6e61 7773 2e63 6f6d 2f67 6974 2d68  zonaws.com/git-h
 00000210: 7474 702f 3036 3631 3935 3131 3233 3835  ttp/066195112385
 00000220: 2f75 732d 7765 7374 2d32 2f65 3635 3032  /us-west-2/e6502
 00000230: 6138 302d 6262 3465 2d34 6662 652d 3837  a80-bb4e-4fbe-87
 00000240: 3263 2d35 6434 3263 3139 3336 3939 642f  2c-5d42c193699d/
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/files/delegate.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/files/delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/files/file.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/files/file.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/files/http_delegate.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/files/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/files/s3_delegate.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/files/s3_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/http_delegates.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/http_delegates.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/__init__.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/orgs/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/__pycache__/__init__.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/orgs/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 852 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 5403 0000  o.......1..dT...
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 5403 0000  o..........dT...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 8400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6400 6404 6c0a 6d0b 5a0b 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6405 6c0c 6d0d 5a0d 0100 6400 6406 6c0e  d.l.m.Z...d.d.l.
@@ -39,15 +39,15 @@
 00000260: 0900 0000 5a0a 6f72 675f 696e 7669 7465  ....Z.org_invite
 00000270: 720a 0000 005a 086f 7267 5f72 6f6c 6572  r....Z.org_roler
 00000280: 0b00 0000 da06 7265 636f 7264 720c 0000  ......recordr...
 00000290: 0072 0d00 0000 720e 0000 0072 0f00 0000  .r....r....r....
 000002a0: 7210 0000 0072 1100 0000 da07 5f5f 616c  r....r......__al
 000002b0: 6c5f 5fa9 0072 1800 0000 7218 0000 00fa  l__..r....r.....
 000002c0: ec2f 636f 6465 6275 696c 642f 6f75 7470  ./codebuild/outp
-000002d0: 7574 2f73 7263 3136 3839 3135 3533 3939  ut/src1689155399
+000002d0: 7574 2f73 7263 3335 3738 3131 3231 3931  ut/src3578112191
 000002e0: 2f73 7263 2f63 6f64 6573 7461 722d 636f  /src/codestar-co
 000002f0: 6e6e 6563 7469 6f6e 732e 7573 2d77 6573  nnections.us-wes
 00000300: 742d 322e 616d 617a 6f6e 6177 732e 636f  t-2.amazonaws.co
 00000310: 6d2f 6769 742d 6874 7470 2f30 3636 3139  m/git-http/06619
 00000320: 3531 3132 3338 352f 7573 2d77 6573 742d  5112385/us-west-
 00000330: 322f 6536 3530 3261 3830 2d62 6234 652d  2/e6502a80-bb4e-
 00000340: 3466 6265 2d38 3732 632d 3564 3432 6331  4fbe-872c-5d42c1
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/__pycache__/delegate.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/orgs/__pycache__/delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 2856 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,225 +1,236 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 280b 0000  o.......1..d(...
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 e20b 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6403 6404 6c03 6d04 5a04 6d05 5a05  ..d.d.l.m.Z.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 4700  m.Z.m.Z.m.Z...G.
 00000060: 6405 6406 8400 6406 6500 6a09 8303 5a0a  d.d...d.e.j...Z.
 00000070: 6401 5300 2907 e900 0000 004e 2901 da08  d.S.)......N)...
 00000080: 4f70 7469 6f6e 616c e901 0000 0029 05da  Optional.....)..
 00000090: 0f4f 7267 496e 7669 7465 5265 636f 7264  .OrgInviteRecord
 000000a0: da09 4f72 6752 6563 6f72 64da 0b4f 7267  ..OrgRecord..Org
 000000b0: 526f 6c65 4e61 6d65 da0d 4f72 6752 6f6c  RoleName..OrgRol
 000000c0: 6552 6563 6f72 64da 074f 7267 5479 7065  eRecord..OrgType
 000000d0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-000000e0: 000c 0000 0040 0000 0073 f601 0000 6500  .....@...s....e.
-000000f0: 5a01 6400 5a02 6503 6a04 0901 642d 6402  Z.d.Z.e.j...d-d.
+000000e0: 000c 0000 0040 0000 0073 1a02 0000 6500  .....@...s....e.
+000000f0: 5a01 6400 5a02 6503 6a04 0901 642f 6402  Z.d.Z.e.j...d/d.
 00000100: 6505 6506 1900 6403 6506 6404 6507 6405  e.e...d.e.d.e.d.
 00000110: 6508 6406 6509 660a 6407 6408 8405 8301  e.d.e.f.d.d.....
 00000120: 5a0a 6503 6a04 6409 6505 6506 1900 6406  Z.e.j.d.e.e...d.
 00000130: 650b 6509 1900 6604 640a 640b 8404 8301  e.e...f.d.d.....
 00000140: 5a0c 6503 6a04 6409 6505 6506 1900 6406  Z.e.j.d.e.e...d.
 00000150: 650b 650d 1900 6604 640c 640d 8404 8301  e.e...f.d.d.....
 00000160: 5a0e 6503 6a04 640e 6505 6506 1900 6406  Z.e.j.d.e.e...d.
 00000170: 650b 650d 1900 6604 640f 6410 8404 8301  e.e...f.d.d.....
-00000180: 5a0f 6503 6a04 0911 642e 6409 6505 6506  Z.e.j...d.d.e.e.
+00000180: 5a0f 6503 6a04 0911 6430 6409 6505 6506  Z.e.j...d0d.e.e.
 00000190: 1900 640e 6505 6506 1900 6406 650d 6606  ..d.e.e...d.e.f.
 000001a0: 6412 6413 8405 8301 5a10 6503 6a04 0911  d.d.....Z.e.j...
-000001b0: 642f 6409 6506 6414 6511 640e 6505 6506  d/d.e.d.e.d.e.e.
+000001b0: 6431 6409 6506 6414 6511 640e 6505 6506  d1d.e.d.e.d.e.e.
 000001c0: 1900 6606 6415 6416 8405 8301 5a12 6503  ..f.d.d.....Z.e.
-000001d0: 6a04 0911 642f 6409 6506 6414 6511 640e  j...d/d.e.d.e.d.
+000001d0: 6a04 0911 6431 6409 6506 6414 6511 640e  j...d1d.e.d.e.d.
 000001e0: 6505 6506 1900 6606 6417 6418 8405 8301  e.e...f.d.d.....
-000001f0: 5a13 6503 6a04 642f 6409 6506 640e 6505  Z.e.j.d/d.e.d.e.
+000001f0: 5a13 6503 6a04 6431 6409 6506 640e 6505  Z.e.j.d1d.e.d.e.
 00000200: 6506 1900 6406 6411 6606 6419 641a 8405  e...d.d.f.d.d...
 00000210: 8301 5a14 6503 6a04 640e 6506 6406 6509  ..Z.e.j.d.e.d.e.
 00000220: 6604 641b 641c 8404 8301 5a15 6503 6a04  f.d.d.....Z.e.j.
 00000230: 640e 6506 6602 641d 641e 8404 8301 5a16  d.e.f.d.d.....Z.
 00000240: 6503 6a04 640e 6506 641f 6506 6604 6420  e.j.d.e.d.e.f.d 
-00000250: 6421 8404 8301 5a17 6503 6a04 0911 642f  d!....Z.e.j...d/
+00000250: 6421 8404 8301 5a17 6503 6a04 0911 6431  d!....Z.e.j...d1
 00000260: 6422 6506 640e 6506 6423 6505 6506 1900  d"e.d.e.d#e.e...
 00000270: 6406 6518 6608 6424 6425 8405 8301 5a19  d.e.f.d$d%....Z.
-00000280: 6503 6a04 642f 6426 6506 6409 6505 6506  e.j.d/d&e.d.e.e.
-00000290: 1900 6604 6427 6428 8405 8301 5a1a 6503  ..f.d'd(....Z.e.
-000002a0: 6a04 642f 6426 6506 6409 6505 6506 1900  j.d/d&e.d.e.e...
-000002b0: 6604 6429 642a 8405 8301 5a1b 6503 6a04  f.d)d*....Z.e.j.
-000002c0: 0911 642f 6426 6506 6409 6505 6506 1900  ..d/d&e.d.e.e...
-000002d0: 6406 6518 6606 642b 642c 8405 8301 5a1c  d.e.f.d+d,....Z.
-000002e0: 6411 5300 2930 da0b 4f72 6744 656c 6567  d.S.)0..OrgDeleg
-000002f0: 6174 6546 da0f 6372 6561 746f 725f 7573  ateF..creator_us
-00000300: 6572 5f69 64da 046e 616d 65da 086f 7267  er_id..name..org
-00000310: 5f74 7970 65da 1162 696e 645f 656d 6169  _type..bind_emai
-00000320: 6c5f 646f 6d61 696e da06 7265 7475 726e  l_domain..return
-00000330: 6305 0000 0000 0000 0000 0000 0005 0000  c...............
-00000340: 0002 0000 0043 0000 00f3 0800 0000 7400  .....C........t.
-00000350: 6401 8301 8201 2902 4eda 0a63 7265 6174  d.....).N..creat
-00000360: 655f 6f72 67a9 01da 134e 6f74 496d 706c  e_org....NotImpl
-00000370: 656d 656e 7465 6445 7272 6f72 2905 da04  ementedError)...
-00000380: 7365 6c66 720a 0000 0072 0b00 0000 720c  selfr....r....r.
-00000390: 0000 0072 0d00 0000 a900 7214 0000 00fa  ...r......r.....
-000003a0: ec2f 636f 6465 6275 696c 642f 6f75 7470  ./codebuild/outp
-000003b0: 7574 2f73 7263 3136 3839 3135 3533 3939  ut/src1689155399
-000003c0: 2f73 7263 2f63 6f64 6573 7461 722d 636f  /src/codestar-co
-000003d0: 6e6e 6563 7469 6f6e 732e 7573 2d77 6573  nnections.us-wes
-000003e0: 742d 322e 616d 617a 6f6e 6177 732e 636f  t-2.amazonaws.co
-000003f0: 6d2f 6769 742d 6874 7470 2f30 3636 3139  m/git-http/06619
-00000400: 3531 3132 3338 352f 7573 2d77 6573 742d  5112385/us-west-
-00000410: 322f 6536 3530 3261 3830 2d62 6234 652d  2/e6502a80-bb4e-
-00000420: 3466 6265 2d38 3732 632d 3564 3432 6331  4fbe-872c-5d42c1
-00000430: 3933 3639 3964 2f72 6f62 6f74 6f2d 6169  93699d/roboto-ai
-00000440: 2f72 6f62 6f74 6f2d 686f 7374 6564 2d61  /roboto-hosted-a
-00000450: 7070 2f70 6163 6b61 6765 732f 726f 626f  pp/packages/robo
-00000460: 746f 5f73 646b 2f73 7263 2f72 6f62 6f74  to_sdk/src/robot
-00000470: 6f5f 7364 6b2f 646f 6d61 696e 2f6f 7267  o_sdk/domain/org
-00000480: 732f 6465 6c65 6761 7465 2e70 7972 1000  s/delegate.pyr..
-00000490: 0000 1000 0000 7302 0000 0008 087a 164f  ......s......z.O
-000004a0: 7267 4465 6c65 6761 7465 2e63 7265 6174  rgDelegate.creat
-000004b0: 655f 6f72 67da 0775 7365 725f 6964 6302  e_org..user_idc.
-000004c0: 0000 0000 0000 0000 0000 0002 0000 0002  ................
-000004d0: 0000 0043 0000 0072 0f00 0000 2902 4eda  ...C...r....).N.
-000004e0: 0d6f 7267 735f 666f 725f 7573 6572 7211  .orgs_for_userr.
-000004f0: 0000 00a9 0272 1300 0000 7216 0000 0072  .....r....r....r
-00000500: 1400 0000 7214 0000 0072 1500 0000 7217  ....r....r....r.
-00000510: 0000 001a 0000 00f3 0200 0000 0802 7a19  ..............z.
-00000520: 4f72 6744 656c 6567 6174 652e 6f72 6773  OrgDelegate.orgs
-00000530: 5f66 6f72 5f75 7365 7263 0200 0000 0000  _for_userc......
-00000540: 0000 0000 0000 0200 0000 0200 0000 4300  ..............C.
-00000550: 0000 720f 0000 0029 024e da12 6f72 675f  ..r....).N..org_
-00000560: 726f 6c65 735f 666f 725f 7573 6572 7211  roles_for_userr.
-00000570: 0000 0072 1800 0000 7214 0000 0072 1400  ...r....r....r..
-00000580: 0000 7215 0000 0072 1a00 0000 1e00 0000  ..r....r........
-00000590: 7219 0000 007a 1e4f 7267 4465 6c65 6761  r....z.OrgDelega
-000005a0: 7465 2e6f 7267 5f72 6f6c 6573 5f66 6f72  te.org_roles_for
-000005b0: 5f75 7365 72da 066f 7267 5f69 6463 0200  _user..org_idc..
-000005c0: 0000 0000 0000 0000 0000 0200 0000 0200  ................
-000005d0: 0000 4300 0000 720f 0000 0029 024e da11  ..C...r....).N..
-000005e0: 6f72 675f 726f 6c65 735f 666f 725f 6f72  org_roles_for_or
-000005f0: 6772 1100 0000 a902 7213 0000 0072 1b00  gr......r....r..
-00000600: 0000 7214 0000 0072 1400 0000 7215 0000  ..r....r....r...
-00000610: 0072 1c00 0000 2200 0000 7219 0000 007a  .r...."...r....z
-00000620: 1d4f 7267 4465 6c65 6761 7465 2e6f 7267  .OrgDelegate.org
-00000630: 5f72 6f6c 6573 5f66 6f72 5f6f 7267 4e63  _roles_for_orgNc
-00000640: 0300 0000 0000 0000 0000 0000 0300 0000  ................
-00000650: 0200 0000 4300 0000 720f 0000 0029 024e  ....C...r....).N
-00000660: da18 6f72 675f 726f 6c65 5f66 6f72 5f75  ..org_role_for_u
-00000670: 7365 725f 696e 5f6f 7267 7211 0000 00a9  ser_in_orgr.....
-00000680: 0372 1300 0000 7216 0000 0072 1b00 0000  .r....r....r....
-00000690: 7214 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
-000006a0: 1e00 0000 2600 0000 f302 0000 0008 047a  ....&..........z
-000006b0: 244f 7267 4465 6c65 6761 7465 2e6f 7267  $OrgDelegate.org
-000006c0: 5f72 6f6c 655f 666f 725f 7573 6572 5f69  _role_for_user_i
-000006d0: 6e5f 6f72 67da 0972 6f6c 655f 6e61 6d65  n_org..role_name
-000006e0: 6304 0000 0000 0000 0000 0000 0004 0000  c...............
-000006f0: 0002 0000 0043 0000 0072 0f00 0000 2902  .....C...r....).
-00000700: 4eda 1161 6464 5f72 6f6c 655f 666f 725f  N..add_role_for_
-00000710: 7573 6572 7211 0000 00a9 0472 1300 0000  userr......r....
-00000720: 7216 0000 0072 2100 0000 721b 0000 0072  r....r!...r....r
-00000730: 1400 0000 7214 0000 0072 1500 0000 7222  ....r....r....r"
-00000740: 0000 002c 0000 0072 2000 0000 7a1d 4f72  ...,...r ...z.Or
-00000750: 6744 656c 6567 6174 652e 6164 645f 726f  gDelegate.add_ro
-00000760: 6c65 5f66 6f72 5f75 7365 7263 0400 0000  le_for_userc....
-00000770: 0000 0000 0000 0000 0400 0000 0200 0000  ................
-00000780: 4300 0000 720f 0000 0029 024e 5a14 7265  C...r....).NZ.re
-00000790: 6d6f 7665 5f72 6f6c 655f 666f 725f 7573  move_role_for_us
-000007a0: 6572 7211 0000 0072 2300 0000 7214 0000  err....r#...r...
-000007b0: 0072 1400 0000 7215 0000 00da 1572 656d  .r....r......rem
-000007c0: 6f76 655f 726f 6c65 5f66 726f 6d5f 7573  ove_role_from_us
-000007d0: 6572 3200 0000 7220 0000 007a 214f 7267  er2...r ...z!Org
-000007e0: 4465 6c65 6761 7465 2e72 656d 6f76 655f  Delegate.remove_
-000007f0: 726f 6c65 5f66 726f 6d5f 7573 6572 6303  role_from_userc.
-00000800: 0000 0000 0000 0000 0000 0003 0000 0002  ................
-00000810: 0000 0043 0000 0072 0f00 0000 2902 4eda  ...C...r....).N.
-00000820: 1472 656d 6f76 655f 7573 6572 5f66 726f  .remove_user_fro
-00000830: 6d5f 6f72 6772 1100 0000 721f 0000 0072  m_orgr....r....r
-00000840: 1400 0000 7214 0000 0072 1500 0000 7225  ....r....r....r%
-00000850: 0000 0038 0000 0072 1900 0000 7a20 4f72  ...8...r....z Or
-00000860: 6744 656c 6567 6174 652e 7265 6d6f 7665  gDelegate.remove
-00000870: 5f75 7365 725f 6672 6f6d 5f6f 7267 6302  _user_from_orgc.
-00000880: 0000 0000 0000 0000 0000 0002 0000 0002  ................
-00000890: 0000 0043 0000 0072 0f00 0000 2902 4eda  ...C...r....).N.
-000008a0: 0d67 6574 5f6f 7267 5f62 795f 6964 7211  .get_org_by_idr.
-000008b0: 0000 0072 1d00 0000 7214 0000 0072 1400  ...r....r....r..
-000008c0: 0000 7215 0000 0072 2600 0000 3c00 0000  ..r....r&...<...
-000008d0: 7219 0000 007a 194f 7267 4465 6c65 6761  r....z.OrgDelega
-000008e0: 7465 2e67 6574 5f6f 7267 5f62 795f 6964  te.get_org_by_id
-000008f0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00000900: 0002 0000 0043 0000 0072 0f00 0000 2902  .....C...r....).
-00000910: 4eda 0a64 656c 6574 655f 6f72 6772 1100  N..delete_orgr..
-00000920: 0000 721d 0000 0072 1400 0000 7214 0000  ..r....r....r...
-00000930: 0072 1500 0000 7227 0000 0040 0000 0072  .r....r'...@...r
-00000940: 1900 0000 7a16 4f72 6744 656c 6567 6174  ....z.OrgDelegat
-00000950: 652e 6465 6c65 7465 5f6f 7267 da0c 656d  e.delete_org..em
-00000960: 6169 6c5f 646f 6d61 696e 6303 0000 0000  ail_domainc.....
-00000970: 0000 0000 0000 0003 0000 0002 0000 0043  ...............C
-00000980: 0000 0072 0f00 0000 2902 4e72 0d00 0000  ...r....).Nr....
-00000990: 7211 0000 0029 0372 1300 0000 721b 0000  r....).r....r...
-000009a0: 0072 2800 0000 7214 0000 0072 1400 0000  .r(...r....r....
-000009b0: 7215 0000 0072 0d00 0000 4400 0000 7219  r....r....D...r.
-000009c0: 0000 007a 1d4f 7267 4465 6c65 6761 7465  ...z.OrgDelegate
-000009d0: 2e62 696e 645f 656d 6169 6c5f 646f 6d61  .bind_email_doma
-000009e0: 696e da0f 696e 7669 7465 645f 7573 6572  in..invited_user
-000009f0: 5f69 64da 1069 6e76 6974 696e 675f 7573  _id..inviting_us
-00000a00: 6572 5f69 6463 0400 0000 0000 0000 0000  er_idc..........
-00000a10: 0000 0400 0000 0200 0000 4300 0000 720f  ..........C...r.
-00000a20: 0000 0029 024e da12 696e 7669 7465 5f75  ...).N..invite_u
-00000a30: 7365 725f 746f 5f6f 7267 7211 0000 0029  ser_to_orgr....)
-00000a40: 0472 1300 0000 7229 0000 0072 1b00 0000  .r....r)...r....
-00000a50: 722a 0000 0072 1400 0000 7214 0000 0072  r*...r....r....r
-00000a60: 1500 0000 722b 0000 0048 0000 0072 2000  ....r+...H...r .
-00000a70: 0000 7a1e 4f72 6744 656c 6567 6174 652e  ..z.OrgDelegate.
-00000a80: 696e 7669 7465 5f75 7365 725f 746f 5f6f  invite_user_to_o
-00000a90: 7267 da09 696e 7669 7465 5f69 6463 0300  rg..invite_idc..
-00000aa0: 0000 0000 0000 0000 0000 0300 0000 0200  ................
-00000ab0: 0000 4300 0000 720f 0000 00a9 024e da11  ..C...r......N..
-00000ac0: 6163 6365 7074 5f6f 7267 5f69 6e76 6974  accept_org_invit
-00000ad0: 6572 1100 0000 a903 7213 0000 0072 2c00  er......r....r,.
-00000ae0: 0000 7216 0000 0072 1400 0000 7214 0000  ..r....r....r...
-00000af0: 0072 1500 0000 722e 0000 004e 0000 0072  .r....r....N...r
-00000b00: 1900 0000 7a1d 4f72 6744 656c 6567 6174  ....z.OrgDelegat
-00000b10: 652e 6163 6365 7074 5f6f 7267 5f69 6e76  e.accept_org_inv
-00000b20: 6974 6563 0300 0000 0000 0000 0000 0000  itec............
-00000b30: 0300 0000 0200 0000 4300 0000 720f 0000  ........C...r...
-00000b40: 0072 2d00 0000 7211 0000 0072 2f00 0000  .r-...r....r/...
-00000b50: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
-00000b60: 1264 6563 6c69 6e65 5f6f 7267 5f69 6e76  .decline_org_inv
-00000b70: 6974 6552 0000 0072 1900 0000 7a1e 4f72  iteR...r....z.Or
-00000b80: 6744 656c 6567 6174 652e 6465 636c 696e  gDelegate.declin
-00000b90: 655f 6f72 675f 696e 7669 7465 6303 0000  e_org_invitec...
-00000ba0: 0000 0000 0000 0000 0003 0000 0002 0000  ................
-00000bb0: 0043 0000 0072 0f00 0000 2902 4eda 0e67  .C...r....).N..g
-00000bc0: 6574 5f6f 7267 5f69 6e76 6974 6572 1100  et_org_inviter..
-00000bd0: 0000 722f 0000 0072 1400 0000 7214 0000  ..r/...r....r...
-00000be0: 0072 1500 0000 7231 0000 0056 0000 0072  .r....r1...V...r
-00000bf0: 2000 0000 7a1a 4f72 6744 656c 6567 6174   ...z.OrgDelegat
-00000c00: 652e 6765 745f 6f72 675f 696e 7669 7465  e.get_org_invite
-00000c10: 2901 4629 024e 4e29 014e 291d da08 5f5f  ).F).NN).N)...__
-00000c20: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00000c30: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00000c40: da03 6162 63da 0e61 6273 7472 6163 746d  ..abc..abstractm
-00000c50: 6574 686f 6472 0200 0000 da03 7374 7272  ethodr......strr
-00000c60: 0800 0000 da04 626f 6f6c 7205 0000 0072  ......boolr....r
-00000c70: 1000 0000 da04 6c69 7374 7217 0000 0072  ......listr....r
-00000c80: 0700 0000 721a 0000 0072 1c00 0000 721e  ....r....r....r.
-00000c90: 0000 0072 0600 0000 7222 0000 0072 2400  ...r....r"...r$.
-00000ca0: 0000 7225 0000 0072 2600 0000 7227 0000  ..r%...r&...r'..
-00000cb0: 0072 0d00 0000 7204 0000 0072 2b00 0000  .r....r....r+...
-00000cc0: 722e 0000 0072 3000 0000 7231 0000 0072  r....r0...r1...r
-00000cd0: 1400 0000 7214 0000 0072 1400 0000 7215  ....r....r....r.
-00000ce0: 0000 0072 0900 0000 0f00 0000 739e 0000  ...r........s...
-00000cf0: 0008 0004 0102 0604 fb06 0202 fe02 0302  ................
-00000d00: fd02 0402 fc02 0502 fb02 060c fa04 091c  ................
-00000d10: 0104 031c 0104 031c 0104 0302 0204 ff06  ................
-00000d20: 0102 ff06 0102 ff02 020c fe04 0502 0204  ................
-00000d30: ff02 0102 ff02 0102 ff06 010c ff04 0502  ................
-00000d40: 0204 ff02 0102 ff02 0102 ff06 010c ff04  ................
-00000d50: 051e 0104 0314 0104 0310 0104 0314 0104  ................
-00000d60: 0302 0204 ff02 0102 ff02 0102 ff06 0102  ................
-00000d70: ff02 020c fe04 051a 0104 031a 0104 0302  ................
-00000d80: 0204 ff02 0102 ff06 0102 ff02 0210 fe72  ...............r
-00000d90: 0900 0000 290b 7235 0000 00da 0674 7970  ....).r5.....typ
-00000da0: 696e 6772 0200 0000 da06 7265 636f 7264  ingr......record
-00000db0: 7204 0000 0072 0500 0000 7206 0000 0072  r....r....r....r
-00000dc0: 0700 0000 7208 0000 00da 0341 4243 7209  ....r......ABCr.
-00000dd0: 0000 0072 1400 0000 7214 0000 0072 1400  ...r....r....r..
-00000de0: 0000 7215 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000df0: 3e01 0000 0073 0800 0000 0802 0c01 1c02  >....s..........
-00000e00: 1609                                     ..
+00000280: 6503 6a04 0911 6431 640e 6505 6506 1900  e.j...d1d.e.e...
+00000290: 6406 650b 6518 1900 6604 6426 6427 8405  d.e.e...f.d&d'..
+000002a0: 8301 5a1a 6503 6a04 6431 6428 6506 6409  ..Z.e.j.d1d(e.d.
+000002b0: 6505 6506 1900 6604 6429 642a 8405 8301  e.e...f.d)d*....
+000002c0: 5a1b 6503 6a04 6431 6428 6506 6409 6505  Z.e.j.d1d(e.d.e.
+000002d0: 6506 1900 6604 642b 642c 8405 8301 5a1c  e...f.d+d,....Z.
+000002e0: 6503 6a04 0911 6431 6428 6506 6409 6505  e.j...d1d(e.d.e.
+000002f0: 6506 1900 6406 6518 6606 642d 642e 8405  e...d.e.f.d-d...
+00000300: 8301 5a1d 6411 5300 2932 da0b 4f72 6744  ..Z.d.S.)2..OrgD
+00000310: 656c 6567 6174 6546 da0f 6372 6561 746f  elegateF..creato
+00000320: 725f 7573 6572 5f69 64da 046e 616d 65da  r_user_id..name.
+00000330: 086f 7267 5f74 7970 65da 1162 696e 645f  .org_type..bind_
+00000340: 656d 6169 6c5f 646f 6d61 696e da06 7265  email_domain..re
+00000350: 7475 726e 6305 0000 0000 0000 0000 0000  turnc...........
+00000360: 0005 0000 0002 0000 0043 0000 00f3 0800  .........C......
+00000370: 0000 7400 6401 8301 8201 2902 4eda 0a63  ..t.d.....).N..c
+00000380: 7265 6174 655f 6f72 67a9 01da 134e 6f74  reate_org....Not
+00000390: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
+000003a0: 2905 da04 7365 6c66 720a 0000 0072 0b00  )...selfr....r..
+000003b0: 0000 720c 0000 0072 0d00 0000 a900 7214  ..r....r......r.
+000003c0: 0000 00fa ec2f 636f 6465 6275 696c 642f  ...../codebuild/
+000003d0: 6f75 7470 7574 2f73 7263 3335 3738 3131  output/src357811
+000003e0: 3231 3931 2f73 7263 2f63 6f64 6573 7461  2191/src/codesta
+000003f0: 722d 636f 6e6e 6563 7469 6f6e 732e 7573  r-connections.us
+00000400: 2d77 6573 742d 322e 616d 617a 6f6e 6177  -west-2.amazonaw
+00000410: 732e 636f 6d2f 6769 742d 6874 7470 2f30  s.com/git-http/0
+00000420: 3636 3139 3531 3132 3338 352f 7573 2d77  66195112385/us-w
+00000430: 6573 742d 322f 6536 3530 3261 3830 2d62  est-2/e6502a80-b
+00000440: 6234 652d 3466 6265 2d38 3732 632d 3564  b4e-4fbe-872c-5d
+00000450: 3432 6331 3933 3639 3964 2f72 6f62 6f74  42c193699d/robot
+00000460: 6f2d 6169 2f72 6f62 6f74 6f2d 686f 7374  o-ai/roboto-host
+00000470: 6564 2d61 7070 2f70 6163 6b61 6765 732f  ed-app/packages/
+00000480: 726f 626f 746f 5f73 646b 2f73 7263 2f72  roboto_sdk/src/r
+00000490: 6f62 6f74 6f5f 7364 6b2f 646f 6d61 696e  oboto_sdk/domain
+000004a0: 2f6f 7267 732f 6465 6c65 6761 7465 2e70  /orgs/delegate.p
+000004b0: 7972 1000 0000 1000 0000 7302 0000 0008  yr........s.....
+000004c0: 087a 164f 7267 4465 6c65 6761 7465 2e63  .z.OrgDelegate.c
+000004d0: 7265 6174 655f 6f72 67da 0775 7365 725f  reate_org..user_
+000004e0: 6964 6302 0000 0000 0000 0000 0000 0002  idc.............
+000004f0: 0000 0002 0000 0043 0000 0072 0f00 0000  .......C...r....
+00000500: 2902 4eda 0d6f 7267 735f 666f 725f 7573  ).N..orgs_for_us
+00000510: 6572 7211 0000 00a9 0272 1300 0000 7216  err......r....r.
+00000520: 0000 0072 1400 0000 7214 0000 0072 1500  ...r....r....r..
+00000530: 0000 7217 0000 001a 0000 00f3 0200 0000  ..r.............
+00000540: 0802 7a19 4f72 6744 656c 6567 6174 652e  ..z.OrgDelegate.
+00000550: 6f72 6773 5f66 6f72 5f75 7365 7263 0200  orgs_for_userc..
+00000560: 0000 0000 0000 0000 0000 0200 0000 0200  ................
+00000570: 0000 4300 0000 720f 0000 0029 024e da12  ..C...r....).N..
+00000580: 6f72 675f 726f 6c65 735f 666f 725f 7573  org_roles_for_us
+00000590: 6572 7211 0000 0072 1800 0000 7214 0000  err....r....r...
+000005a0: 0072 1400 0000 7215 0000 0072 1a00 0000  .r....r....r....
+000005b0: 1e00 0000 7219 0000 007a 1e4f 7267 4465  ....r....z.OrgDe
+000005c0: 6c65 6761 7465 2e6f 7267 5f72 6f6c 6573  legate.org_roles
+000005d0: 5f66 6f72 5f75 7365 72da 066f 7267 5f69  _for_user..org_i
+000005e0: 6463 0200 0000 0000 0000 0000 0000 0200  dc..............
+000005f0: 0000 0200 0000 4300 0000 720f 0000 0029  ......C...r....)
+00000600: 024e da11 6f72 675f 726f 6c65 735f 666f  .N..org_roles_fo
+00000610: 725f 6f72 6772 1100 0000 a902 7213 0000  r_orgr......r...
+00000620: 0072 1b00 0000 7214 0000 0072 1400 0000  .r....r....r....
+00000630: 7215 0000 0072 1c00 0000 2200 0000 7219  r....r...."...r.
+00000640: 0000 007a 1d4f 7267 4465 6c65 6761 7465  ...z.OrgDelegate
+00000650: 2e6f 7267 5f72 6f6c 6573 5f66 6f72 5f6f  .org_roles_for_o
+00000660: 7267 4e63 0300 0000 0000 0000 0000 0000  rgNc............
+00000670: 0300 0000 0200 0000 4300 0000 720f 0000  ........C...r...
+00000680: 0029 024e da18 6f72 675f 726f 6c65 5f66  .).N..org_role_f
+00000690: 6f72 5f75 7365 725f 696e 5f6f 7267 7211  or_user_in_orgr.
+000006a0: 0000 00a9 0372 1300 0000 7216 0000 0072  .....r....r....r
+000006b0: 1b00 0000 7214 0000 0072 1400 0000 7215  ....r....r....r.
+000006c0: 0000 0072 1e00 0000 2600 0000 f302 0000  ...r....&.......
+000006d0: 0008 047a 244f 7267 4465 6c65 6761 7465  ...z$OrgDelegate
+000006e0: 2e6f 7267 5f72 6f6c 655f 666f 725f 7573  .org_role_for_us
+000006f0: 6572 5f69 6e5f 6f72 67da 0972 6f6c 655f  er_in_org..role_
+00000700: 6e61 6d65 6304 0000 0000 0000 0000 0000  namec...........
+00000710: 0004 0000 0002 0000 0043 0000 0072 0f00  .........C...r..
+00000720: 0000 2902 4eda 1161 6464 5f72 6f6c 655f  ..).N..add_role_
+00000730: 666f 725f 7573 6572 7211 0000 00a9 0472  for_userr......r
+00000740: 1300 0000 7216 0000 0072 2100 0000 721b  ....r....r!...r.
+00000750: 0000 0072 1400 0000 7214 0000 0072 1500  ...r....r....r..
+00000760: 0000 7222 0000 002c 0000 0072 2000 0000  ..r"...,...r ...
+00000770: 7a1d 4f72 6744 656c 6567 6174 652e 6164  z.OrgDelegate.ad
+00000780: 645f 726f 6c65 5f66 6f72 5f75 7365 7263  d_role_for_userc
+00000790: 0400 0000 0000 0000 0000 0000 0400 0000  ................
+000007a0: 0200 0000 4300 0000 720f 0000 0029 024e  ....C...r....).N
+000007b0: 5a14 7265 6d6f 7665 5f72 6f6c 655f 666f  Z.remove_role_fo
+000007c0: 725f 7573 6572 7211 0000 0072 2300 0000  r_userr....r#...
+000007d0: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
+000007e0: 1572 656d 6f76 655f 726f 6c65 5f66 726f  .remove_role_fro
+000007f0: 6d5f 7573 6572 3200 0000 7220 0000 007a  m_user2...r ...z
+00000800: 214f 7267 4465 6c65 6761 7465 2e72 656d  !OrgDelegate.rem
+00000810: 6f76 655f 726f 6c65 5f66 726f 6d5f 7573  ove_role_from_us
+00000820: 6572 6303 0000 0000 0000 0000 0000 0003  erc.............
+00000830: 0000 0002 0000 0043 0000 0072 0f00 0000  .......C...r....
+00000840: 2902 4eda 1472 656d 6f76 655f 7573 6572  ).N..remove_user
+00000850: 5f66 726f 6d5f 6f72 6772 1100 0000 721f  _from_orgr....r.
+00000860: 0000 0072 1400 0000 7214 0000 0072 1500  ...r....r....r..
+00000870: 0000 7225 0000 0038 0000 0072 1900 0000  ..r%...8...r....
+00000880: 7a20 4f72 6744 656c 6567 6174 652e 7265  z OrgDelegate.re
+00000890: 6d6f 7665 5f75 7365 725f 6672 6f6d 5f6f  move_user_from_o
+000008a0: 7267 6302 0000 0000 0000 0000 0000 0002  rgc.............
+000008b0: 0000 0002 0000 0043 0000 0072 0f00 0000  .......C...r....
+000008c0: 2902 4eda 0d67 6574 5f6f 7267 5f62 795f  ).N..get_org_by_
+000008d0: 6964 7211 0000 0072 1d00 0000 7214 0000  idr....r....r...
+000008e0: 0072 1400 0000 7215 0000 0072 2600 0000  .r....r....r&...
+000008f0: 3c00 0000 7219 0000 007a 194f 7267 4465  <...r....z.OrgDe
+00000900: 6c65 6761 7465 2e67 6574 5f6f 7267 5f62  legate.get_org_b
+00000910: 795f 6964 6302 0000 0000 0000 0000 0000  y_idc...........
+00000920: 0002 0000 0002 0000 0043 0000 0072 0f00  .........C...r..
+00000930: 0000 2902 4eda 0a64 656c 6574 655f 6f72  ..).N..delete_or
+00000940: 6772 1100 0000 721d 0000 0072 1400 0000  gr....r....r....
+00000950: 7214 0000 0072 1500 0000 7227 0000 0040  r....r....r'...@
+00000960: 0000 0072 1900 0000 7a16 4f72 6744 656c  ...r....z.OrgDel
+00000970: 6567 6174 652e 6465 6c65 7465 5f6f 7267  egate.delete_org
+00000980: da0c 656d 6169 6c5f 646f 6d61 696e 6303  ..email_domainc.
+00000990: 0000 0000 0000 0000 0000 0003 0000 0002  ................
+000009a0: 0000 0043 0000 0072 0f00 0000 2902 4e72  ...C...r....).Nr
+000009b0: 0d00 0000 7211 0000 0029 0372 1300 0000  ....r....).r....
+000009c0: 721b 0000 0072 2800 0000 7214 0000 0072  r....r(...r....r
+000009d0: 1400 0000 7215 0000 0072 0d00 0000 4400  ....r....r....D.
+000009e0: 0000 7219 0000 007a 1d4f 7267 4465 6c65  ..r....z.OrgDele
+000009f0: 6761 7465 2e62 696e 645f 656d 6169 6c5f  gate.bind_email_
+00000a00: 646f 6d61 696e da0f 696e 7669 7465 645f  domain..invited_
+00000a10: 7573 6572 5f69 64da 1069 6e76 6974 696e  user_id..invitin
+00000a20: 675f 7573 6572 5f69 6463 0400 0000 0000  g_user_idc......
+00000a30: 0000 0000 0000 0400 0000 0200 0000 4300  ..............C.
+00000a40: 0000 720f 0000 0029 024e da12 696e 7669  ..r....).N..invi
+00000a50: 7465 5f75 7365 725f 746f 5f6f 7267 7211  te_user_to_orgr.
+00000a60: 0000 0029 0472 1300 0000 7229 0000 0072  ...).r....r)...r
+00000a70: 1b00 0000 722a 0000 0072 1400 0000 7214  ....r*...r....r.
+00000a80: 0000 0072 1500 0000 722b 0000 0048 0000  ...r....r+...H..
+00000a90: 0072 2000 0000 7a1e 4f72 6744 656c 6567  .r ...z.OrgDeleg
+00000aa0: 6174 652e 696e 7669 7465 5f75 7365 725f  ate.invite_user_
+00000ab0: 746f 5f6f 7267 6302 0000 0000 0000 0000  to_orgc.........
+00000ac0: 0000 0002 0000 0002 0000 0043 0000 0072  ...........C...r
+00000ad0: 0f00 0000 2902 4eda 1367 6574 5f69 6e76  ....).N..get_inv
+00000ae0: 6974 6573 5f66 6f72 5f6f 7267 7211 0000  ites_for_orgr...
+00000af0: 0072 1d00 0000 7214 0000 0072 1400 0000  .r....r....r....
+00000b00: 7215 0000 0072 2c00 0000 4e00 0000 7220  r....r,...N...r 
+00000b10: 0000 007a 1f4f 7267 4465 6c65 6761 7465  ...z.OrgDelegate
+00000b20: 2e67 6574 5f69 6e76 6974 6573 5f66 6f72  .get_invites_for
+00000b30: 5f6f 7267 da09 696e 7669 7465 5f69 6463  _org..invite_idc
+00000b40: 0300 0000 0000 0000 0000 0000 0300 0000  ................
+00000b50: 0200 0000 4300 0000 720f 0000 00a9 024e  ....C...r......N
+00000b60: da11 6163 6365 7074 5f6f 7267 5f69 6e76  ..accept_org_inv
+00000b70: 6974 6572 1100 0000 a903 7213 0000 0072  iter......r....r
+00000b80: 2d00 0000 7216 0000 0072 1400 0000 7214  -...r....r....r.
+00000b90: 0000 0072 1500 0000 722f 0000 0054 0000  ...r....r/...T..
+00000ba0: 0072 1900 0000 7a1d 4f72 6744 656c 6567  .r....z.OrgDeleg
+00000bb0: 6174 652e 6163 6365 7074 5f6f 7267 5f69  ate.accept_org_i
+00000bc0: 6e76 6974 6563 0300 0000 0000 0000 0000  nvitec..........
+00000bd0: 0000 0300 0000 0200 0000 4300 0000 720f  ..........C...r.
+00000be0: 0000 0072 2e00 0000 7211 0000 0072 3000  ...r....r....r0.
+00000bf0: 0000 7214 0000 0072 1400 0000 7215 0000  ..r....r....r...
+00000c00: 00da 1264 6563 6c69 6e65 5f6f 7267 5f69  ...decline_org_i
+00000c10: 6e76 6974 6558 0000 0072 1900 0000 7a1e  nviteX...r....z.
+00000c20: 4f72 6744 656c 6567 6174 652e 6465 636c  OrgDelegate.decl
+00000c30: 696e 655f 6f72 675f 696e 7669 7465 6303  ine_org_invitec.
+00000c40: 0000 0000 0000 0000 0000 0003 0000 0002  ................
+00000c50: 0000 0043 0000 0072 0f00 0000 2902 4eda  ...C...r....).N.
+00000c60: 0e67 6574 5f6f 7267 5f69 6e76 6974 6572  .get_org_inviter
+00000c70: 1100 0000 7230 0000 0072 1400 0000 7214  ....r0...r....r.
+00000c80: 0000 0072 1500 0000 7232 0000 005c 0000  ...r....r2...\..
+00000c90: 0072 2000 0000 7a1a 4f72 6744 656c 6567  .r ...z.OrgDeleg
+00000ca0: 6174 652e 6765 745f 6f72 675f 696e 7669  ate.get_org_invi
+00000cb0: 7465 2901 4629 024e 4e29 014e 291e da08  te).F).NN).N)...
+00000cc0: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+00000cd0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+00000ce0: 5f5f da03 6162 63da 0e61 6273 7472 6163  __..abc..abstrac
+00000cf0: 746d 6574 686f 6472 0200 0000 da03 7374  tmethodr......st
+00000d00: 7272 0800 0000 da04 626f 6f6c 7205 0000  rr......boolr...
+00000d10: 0072 1000 0000 da04 6c69 7374 7217 0000  .r......listr...
+00000d20: 0072 0700 0000 721a 0000 0072 1c00 0000  .r....r....r....
+00000d30: 721e 0000 0072 0600 0000 7222 0000 0072  r....r....r"...r
+00000d40: 2400 0000 7225 0000 0072 2600 0000 7227  $...r%...r&...r'
+00000d50: 0000 0072 0d00 0000 7204 0000 0072 2b00  ...r....r....r+.
+00000d60: 0000 722c 0000 0072 2f00 0000 7231 0000  ..r,...r/...r1..
+00000d70: 0072 3200 0000 7214 0000 0072 1400 0000  .r2...r....r....
+00000d80: 7214 0000 0072 1500 0000 7209 0000 000f  r....r....r.....
+00000d90: 0000 0073 ac00 0000 0800 0401 0206 04fb  ...s............
+00000da0: 0602 02fe 0203 02fd 0204 02fc 0205 02fb  ................
+00000db0: 0206 0cfa 0409 1c01 0403 1c01 0403 1c01  ................
+00000dc0: 0403 0202 04ff 0601 02ff 0601 02ff 0202  ................
+00000dd0: 0cfe 0405 0202 04ff 0201 02ff 0201 02ff  ................
+00000de0: 0601 0cff 0405 0202 04ff 0201 02ff 0201  ................
+00000df0: 02ff 0601 0cff 0405 1e01 0403 1401 0403  ................
+00000e00: 1001 0403 1401 0403 0202 04ff 0201 02ff  ................
+00000e10: 0201 02ff 0601 02ff 0202 0cfe 0405 0202  ................
+00000e20: 04ff 0601 02ff 0602 0cfe 0405 1a01 0403  ................
+00000e30: 1a01 0403 0202 04ff 0201 02ff 0601 02ff  ................
+00000e40: 0202 10fe 7209 0000 0029 0b72 3600 0000  ....r....).r6...
+00000e50: da06 7479 7069 6e67 7202 0000 00da 0672  ..typingr......r
+00000e60: 6563 6f72 6472 0400 0000 7205 0000 0072  ecordr....r....r
+00000e70: 0600 0000 7207 0000 0072 0800 0000 da03  ....r....r......
+00000e80: 4142 4372 0900 0000 7214 0000 0072 1400  ABCr....r....r..
+00000e90: 0000 7214 0000 0072 1500 0000 da08 3c6d  ..r....r......<m
+00000ea0: 6f64 756c 653e 0100 0000 7308 0000 0008  odule>....s.....
+00000eb0: 020c 011c 0216 09                        .......
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/__pycache__/http_delegate.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/orgs/__pycache__/http_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 6889 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 e91a 0000  o.......1..d....
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 751d 0000  o..........du...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8c00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6402 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 0100 6402 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6406 6407 6c09 6d0a 5a0a 0100 6406  ..d.d.l.m.Z...d.
 00000070: 6408 6c0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  d.l.m.Z.m.Z.m.Z.
@@ -27,406 +27,434 @@
 000001a0: 656d 6f76 6555 7365 7246 726f 6d4f 7267  emoveUserFromOrg
 000001b0: 5265 7175 6573 7429 05da 0f4f 7267 496e  Request)...OrgIn
 000001c0: 7669 7465 5265 636f 7264 da09 4f72 6752  viteRecord..OrgR
 000001d0: 6563 6f72 64da 0b4f 7267 526f 6c65 4e61  ecord..OrgRoleNa
 000001e0: 6d65 da0d 4f72 6752 6f6c 6552 6563 6f72  me..OrgRoleRecor
 000001f0: 64da 074f 7267 5479 7065 6300 0000 0000  d..OrgTypec.....
 00000200: 0000 0000 0000 0000 0000 000b 0000 0000  ................
-00000210: 0000 0073 c001 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+00000210: 0000 0073 de01 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
 00000220: 5500 6503 6504 6401 3c00 6402 6503 6602  U.e.e.d.<.d.e.f.
-00000230: 8700 6601 6403 6404 840c 5a05 0905 6431  ..f.d.d...Z...d1
+00000230: 8700 6601 6403 6404 840c 5a05 0905 6433  ..f.d.d...Z...d3
 00000240: 6406 6506 6507 1900 6407 6507 6408 6508  d.e.e...d.e.d.e.
 00000250: 6409 6509 640a 650a 660a 640b 640c 8405  d.e.d.e.f.d.d...
 00000260: 5a0b 640d 6506 6507 1900 640a 650c 650a  Z.d.e.e...d.e.e.
 00000270: 1900 6604 640e 640f 8404 5a0d 640d 6506  ..f.d.d...Z.d.e.
 00000280: 6507 1900 640a 650c 650e 1900 6604 6410  e...d.e.e...f.d.
-00000290: 6411 8404 5a0f 0912 6432 640d 6507 6413  d...Z...d2d.e.d.
+00000290: 6411 8404 5a0f 0912 6434 640d 6507 6413  d...Z...d4d.e.d.
 000002a0: 6510 6414 6506 6507 1900 6606 6415 6416  e.d.e.e...f.d.d.
-000002b0: 8405 5a11 0912 6432 640d 6507 6413 6510  ..Z...d2d.e.d.e.
+000002b0: 8405 5a11 0912 6434 640d 6507 6413 6510  ..Z...d4d.e.d.e.
 000002c0: 6414 6506 6507 1900 6606 6417 6418 8405  d.e.e...f.d.d...
 000002d0: 5a12 6414 6506 6507 1900 640a 650c 650e  Z.d.e.e...d.e.e.
-000002e0: 1900 6604 6419 641a 8404 5a13 6432 640d  ..f.d.d...Z.d2d.
+000002e0: 1900 6604 6419 641a 8404 5a13 6434 640d  ..f.d.d...Z.d4d.
 000002f0: 6507 6414 6506 6507 1900 640a 6412 6606  e.d.e.e...d.d.f.
 00000300: 641b 641c 8405 5a14 6414 6507 640a 650a  d.d...Z.d.e.d.e.
 00000310: 6604 641d 641e 8404 5a15 6414 6507 640a  f.d.d...Z.d.e.d.
 00000320: 6412 6604 641f 6420 8404 5a16 6414 6507  d.f.d.d ..Z.d.e.
 00000330: 6421 6507 6604 6422 6423 8404 5a17 0912  d!e.f.d"d#..Z...
-00000340: 6432 6424 6507 6414 6507 6425 6506 6507  d2d$e.d.e.d%e.e.
+00000340: 6434 6424 6507 6414 6507 6425 6506 6507  d4d$e.d.e.d%e.e.
 00000350: 1900 640a 6518 6608 6426 6427 8405 5a19  ..d.e.f.d&d'..Z.
-00000360: 6432 6428 6507 640d 6506 6507 1900 6604  d2d(e.d.e.e...f.
-00000370: 6429 642a 8405 5a1a 6432 6428 6507 640d  d)d*..Z.d2d(e.d.
+00000360: 6434 6428 6507 640d 6506 6507 1900 6604  d4d(e.d.e.e...f.
+00000370: 6429 642a 8405 5a1a 6434 6428 6507 640d  d)d*..Z.d4d(e.d.
 00000380: 6506 6507 1900 6604 642b 642c 8405 5a1b  e.e...f.d+d,..Z.
-00000390: 0912 6432 6428 6507 640d 6506 6507 1900  ..d2d(e.d.e.e...
+00000390: 0912 6434 6428 6507 640d 6506 6507 1900  ..d4d(e.d.e.e...
 000003a0: 640a 6518 6606 642d 642e 8405 5a1c 0912  d.e.f.d-d...Z...
-000003b0: 6433 640d 6506 6507 1900 6414 6506 6507  d3d.e.e...d.e.e.
-000003c0: 1900 640a 650e 6606 642f 6430 8405 5a1d  ..d.e.f.d/d0..Z.
-000003d0: 8700 0400 5a1e 5300 2934 da0f 4f72 6748  ....Z.S.)4..OrgH
-000003e0: 7474 7044 656c 6567 6174 65da 1d5f 4f72  ttpDelegate.._Or
-000003f0: 6748 7474 7044 656c 6567 6174 655f 5f68  gHttpDelegate__h
-00000400: 7474 705f 636c 6965 6e74 da0b 6874 7470  ttp_client..http
-00000410: 5f63 6c69 656e 7463 0200 0000 0000 0000  _clientc........
-00000420: 0000 0000 0200 0000 0200 0000 0300 0000  ................
-00000430: 7314 0000 0074 0083 00a0 01a1 0001 007c  s....t.........|
-00000440: 017c 005f 0264 0053 00a9 014e 2903 da05  .|._.d.S...N)...
-00000450: 7375 7065 72da 085f 5f69 6e69 745f 5f72  super..__init__r
-00000460: 1500 0000 2902 da04 7365 6c66 7216 0000  ....)...selfr...
-00000470: 00a9 01da 095f 5f63 6c61 7373 5f5f a900  .....__class__..
-00000480: faf1 2f63 6f64 6562 7569 6c64 2f6f 7574  ../codebuild/out
-00000490: 7075 742f 7372 6331 3638 3931 3535 3339  put/src168915539
-000004a0: 392f 7372 632f 636f 6465 7374 6172 2d63  9/src/codestar-c
-000004b0: 6f6e 6e65 6374 696f 6e73 2e75 732d 7765  onnections.us-we
-000004c0: 7374 2d32 2e61 6d61 7a6f 6e61 7773 2e63  st-2.amazonaws.c
-000004d0: 6f6d 2f67 6974 2d68 7474 702f 3036 3631  om/git-http/0661
-000004e0: 3935 3131 3233 3835 2f75 732d 7765 7374  95112385/us-west
-000004f0: 2d32 2f65 3635 3032 6138 302d 6262 3465  -2/e6502a80-bb4e
-00000500: 2d34 6662 652d 3837 3263 2d35 6434 3263  -4fbe-872c-5d42c
-00000510: 3139 3336 3939 642f 726f 626f 746f 2d61  193699d/roboto-a
-00000520: 692f 726f 626f 746f 2d68 6f73 7465 642d  i/roboto-hosted-
-00000530: 6170 702f 7061 636b 6167 6573 2f72 6f62  app/packages/rob
-00000540: 6f74 6f5f 7364 6b2f 7372 632f 726f 626f  oto_sdk/src/robo
-00000550: 746f 5f73 646b 2f64 6f6d 6169 6e2f 6f72  to_sdk/domain/or
-00000560: 6773 2f68 7474 705f 6465 6c65 6761 7465  gs/http_delegate
-00000570: 2e70 7972 1900 0000 1f00 0000 7304 0000  .pyr........s...
-00000580: 000a 010a 017a 184f 7267 4874 7470 4465  .....z.OrgHttpDe
-00000590: 6c65 6761 7465 2e5f 5f69 6e69 745f 5f46  legate.__init__F
-000005a0: da0f 6372 6561 746f 725f 7573 6572 5f69  ..creator_user_i
-000005b0: 64da 046e 616d 65da 086f 7267 5f74 7970  d..name..org_typ
-000005c0: 65da 1162 696e 645f 656d 6169 6c5f 646f  e..bind_email_do
-000005d0: 6d61 696e da06 7265 7475 726e 6305 0000  main..returnc...
-000005e0: 0000 0000 0000 0000 0009 0000 0008 0000  ................
-000005f0: 0043 0000 0073 7c00 0000 7c00 6a00 a001  .C...s|...|.j...
-00000600: 6401 a101 7d05 7402 7c01 6402 8d01 7d06  d...}.t.|.d...}.
-00000610: 6403 7c06 6404 3c00 7403 7c02 7c03 7c04  d.|.d.<.t.|.|.|.
-00000620: 6405 8d03 7d07 7404 8300 8f13 0100 7c00  d...}.t.......|.
-00000630: 6a00 6a05 7c05 7c06 7406 7c07 8301 6406  j.j.|.|.t.|...d.
-00000640: 8d03 7d08 5700 6400 0400 0400 8303 0100  ..}.W.d.........
-00000650: 6e08 3100 732f 7701 0100 0100 0100 5900  n.1.s/w.......Y.
-00000660: 0100 7407 a008 7c08 6a09 6407 6701 6408  ..t...|.j.d.g.d.
-00000670: 8d01 a101 5300 2909 4efa 0776 312f 6f72  ....S.).N..v1/or
-00000680: 6773 a901 da07 7573 6572 5f69 647a 1061  gs....user_idz.a
-00000690: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e7a  pplication/jsonz
-000006a0: 0c43 6f6e 7465 6e74 2d54 7970 6529 0372  .Content-Type).r
-000006b0: 2000 0000 7221 0000 0072 2200 0000 a903   ...r!...r".....
-000006c0: da03 7572 6cda 0768 6561 6465 7273 da04  ..url..headers..
-000006d0: 6461 7461 722a 0000 00a9 01da 096a 736f  datar*.......jso
-000006e0: 6e5f 7061 7468 290a 7215 0000 0072 2800  n_path).r....r(.
-000006f0: 0000 7206 0000 0072 0b00 0000 7204 0000  ..r....r....r...
-00000700: 00da 0470 6f73 7472 0700 0000 7210 0000  ...postr....r...
-00000710: 00da 0970 6172 7365 5f6f 626a da09 6672  ...parse_obj..fr
-00000720: 6f6d 5f6a 736f 6e29 0972 1a00 0000 721f  om_json).r....r.
-00000730: 0000 0072 2000 0000 7221 0000 0072 2200  ...r ...r!...r".
-00000740: 0000 7228 0000 0072 2900 0000 da0c 7265  ..r(...r).....re
-00000750: 7175 6573 745f 626f 6479 da08 7265 7370  quest_body..resp
-00000760: 6f6e 7365 721d 0000 0072 1d00 0000 721e  onser....r....r.
-00000770: 0000 00da 0a63 7265 6174 655f 6f72 6723  .....create_org#
-00000780: 0000 0073 1800 0000 0c07 0a01 0801 0202  ...s............
-00000790: 0601 06ff 0804 0601 0a01 08ff 1cff 1405  ................
-000007a0: 7a1a 4f72 6748 7474 7044 656c 6567 6174  z.OrgHttpDelegat
-000007b0: 652e 6372 6561 7465 5f6f 7267 7226 0000  e.create_orgr&..
-000007c0: 0063 0200 0000 0000 0000 0000 0000 0400  .c..............
-000007d0: 0000 0800 0000 4300 0000 7358 0000 007c  ......C...sX...|
-000007e0: 006a 00a0 0164 01a1 017d 0274 0283 008f  .j...d...}.t....
-000007f0: 0f01 007c 006a 006a 037c 0264 028d 017d  ...|.j.j.|.d...}
-00000800: 0357 0064 0004 0004 0083 0301 006e 0831  .W.d.........n.1
-00000810: 0073 1b77 0101 0001 0001 0059 0001 0064  .s.w.......Y...d
-00000820: 0364 0484 007c 036a 0464 0567 0164 068d  .d...|.j.d.g.d..
-00000830: 0144 0083 0153 0029 074e 7a0c 7631 2f6f  .D...S.).Nz.v1/o
-00000840: 7267 732f 6c69 7374 a901 7228 0000 0063  rgs/list..r(...c
-00000850: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000860: 0500 0000 5300 0000 f316 0000 0067 007c  ....S........g.|
-00000870: 005d 077d 0174 00a0 017c 01a1 0191 0271  .].}.t...|.....q
-00000880: 0253 0072 1d00 0000 2902 7210 0000 0072  .S.r....).r....r
-00000890: 2e00 0000 a902 da02 2e30 da06 7265 636f  .........0..reco
-000008a0: 7264 721d 0000 0072 1d00 0000 721e 0000  rdr....r....r...
-000008b0: 00da 0a3c 6c69 7374 636f 6d70 3e3f 0000  ...<listcomp>?..
-000008c0: 00f3 0800 0000 0600 0202 08ff 06ff 7a31  ..............z1
-000008d0: 4f72 6748 7474 7044 656c 6567 6174 652e  OrgHttpDelegate.
-000008e0: 6f72 6773 5f66 6f72 5f75 7365 722e 3c6c  orgs_for_user.<l
-000008f0: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-00000900: 3e72 2a00 0000 722b 0000 0029 0572 1500  >r*...r+...).r..
-00000910: 0000 7228 0000 0072 0400 0000 da03 6765  ..r(...r......ge
-00000920: 7472 2f00 0000 2904 721a 0000 0072 2600  tr/...).r....r&.
-00000930: 0000 7228 0000 0072 3100 0000 721d 0000  ..r(...r1...r...
-00000940: 0072 1d00 0000 721e 0000 00da 0d6f 7267  .r....r......org
-00000950: 735f 666f 725f 7573 6572 3900 0000 730e  s_for_user9...s.
-00000960: 0000 000c 0108 0210 011c ff06 030c 0206  ................
-00000970: fe7a 1d4f 7267 4874 7470 4465 6c65 6761  .z.OrgHttpDelega
-00000980: 7465 2e6f 7267 735f 666f 725f 7573 6572  te.orgs_for_user
-00000990: 6302 0000 0000 0000 0000 0000 0005 0000  c...............
-000009a0: 0008 0000 0043 0000 00f3 6400 0000 7c00  .....C....d...|.
-000009b0: 6a00 a001 6401 a101 7d02 7402 7c01 6402  j...d...}.t.|.d.
-000009c0: 8d01 7d03 7403 8300 8f10 0100 7c00 6a00  ..}.t.......|.j.
-000009d0: 6a04 7c02 7c03 6403 8d02 7d04 5700 6400  j.|.|.d...}.W.d.
-000009e0: 0400 0400 8303 0100 6e08 3100 7321 7701  ........n.1.s!w.
-000009f0: 0100 0100 0100 5900 0100 6404 6405 8400  ......Y...d.d...
-00000a00: 7c04 6a05 6406 6701 6407 8d01 4400 8301  |.j.d.g.d...D...
-00000a10: 5300 2908 4efa 1276 312f 6f72 6773 2f72  S.).N..v1/orgs/r
-00000a20: 6f6c 6573 2f75 7365 7272 2500 0000 a902  oles/userr%.....
-00000a30: 7228 0000 0072 2900 0000 6301 0000 0000  r(...r)...c.....
-00000a40: 0000 0000 0000 0002 0000 0005 0000 0053  ...............S
-00000a50: 0000 0072 3400 0000 721d 0000 00a9 0272  ...r4...r......r
-00000a60: 1200 0000 722e 0000 0072 3500 0000 721d  ....r....r5...r.
-00000a70: 0000 0072 1d00 0000 721e 0000 0072 3800  ...r....r....r8.
-00000a80: 0000 4c00 0000 7239 0000 007a 364f 7267  ..L...r9...z6Org
-00000a90: 4874 7470 4465 6c65 6761 7465 2e6f 7267  HttpDelegate.org
-00000aa0: 5f72 6f6c 6573 5f66 6f72 5f75 7365 722e  _roles_for_user.
-00000ab0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-00000ac0: 6d70 3e72 2a00 0000 722b 0000 00a9 0672  mp>r*...r+.....r
-00000ad0: 1500 0000 7228 0000 0072 0600 0000 7204  ....r(...r....r.
-00000ae0: 0000 0072 3a00 0000 722f 0000 0029 0572  ...r:...r/...).r
-00000af0: 1a00 0000 7226 0000 0072 2800 0000 7229  ....r&...r(...r)
-00000b00: 0000 0072 3100 0000 721d 0000 0072 1d00  ...r1...r....r..
-00000b10: 0000 721e 0000 00da 126f 7267 5f72 6f6c  ..r......org_rol
-00000b20: 6573 5f66 6f72 5f75 7365 7244 0000 00f3  es_for_userD....
-00000b30: 1000 0000 0c01 0a02 0802 1201 1cff 0603  ................
-00000b40: 0c02 06fe 7a22 4f72 6748 7474 7044 656c  ....z"OrgHttpDel
-00000b50: 6567 6174 652e 6f72 675f 726f 6c65 735f  egate.org_roles_
-00000b60: 666f 725f 7573 6572 4eda 0972 6f6c 655f  for_userN..role_
-00000b70: 6e61 6d65 da06 6f72 675f 6964 6304 0000  name..org_idc...
-00000b80: 0000 0000 0000 0000 0007 0000 0008 0000  ................
-00000b90: 0043 0000 00f3 6400 0000 7c00 6a00 a001  .C....d...|.j...
-00000ba0: 6401 a101 7d04 7402 7c03 6402 8d01 7d05  d...}.t.|.d...}.
-00000bb0: 7403 7c01 7c02 6403 8d02 7d06 7404 8300  t.|.|.d...}.t...
-00000bc0: 8f14 0100 7c00 6a00 6a05 7c04 7c05 7406  ....|.j.j.|.|.t.
-00000bd0: 7c06 8301 6404 8d03 0100 5700 6400 0400  |...d.....W.d...
-00000be0: 0400 8303 0100 6400 5300 3100 732b 7701  ......d.S.1.s+w.
-00000bf0: 0100 0100 0100 5900 0100 6400 5300 a905  ......Y...d.S...
-00000c00: 4e72 3d00 0000 a901 7244 0000 0029 0272  Nr=.....rD...).r
-00000c10: 2600 0000 7243 0000 0072 2700 0000 2907  &...rC...r'...).
-00000c20: 7215 0000 0072 2800 0000 7206 0000 0072  r....r(...r....r
-00000c30: 0d00 0000 7204 0000 00da 0370 7574 7207  ....r......putr.
-00000c40: 0000 00a9 0772 1a00 0000 7226 0000 0072  .....r....r&...r
-00000c50: 4300 0000 7244 0000 0072 2800 0000 7229  C...rD...r(...r)
-00000c60: 0000 0072 3000 0000 721d 0000 0072 1d00  ...r0...r....r..
-00000c70: 0000 721e 0000 00da 1161 6464 5f72 6f6c  ..r......add_rol
-00000c80: 655f 666f 725f 7573 6572 5100 0000 f310  e_for_userQ.....
-00000c90: 0000 000c 030a 010c 0108 0206 010a 0108  ................
-00000ca0: ff22 ff7a 214f 7267 4874 7470 4465 6c65  .".z!OrgHttpDele
-00000cb0: 6761 7465 2e61 6464 5f72 6f6c 655f 666f  gate.add_role_fo
-00000cc0: 725f 7573 6572 6304 0000 0000 0000 0000  r_userc.........
-00000cd0: 0000 0007 0000 0008 0000 0043 0000 0072  ...........C...r
-00000ce0: 4500 0000 7246 0000 0029 0772 1500 0000  E...rF...).r....
-00000cf0: 7228 0000 0072 0600 0000 720d 0000 0072  r(...r....r....r
-00000d00: 0400 0000 da06 6465 6c65 7465 7207 0000  ......deleter...
-00000d10: 0072 4900 0000 721d 0000 0072 1d00 0000  .rI...r....r....
-00000d20: 721e 0000 00da 1572 656d 6f76 655f 726f  r......remove_ro
-00000d30: 6c65 5f66 726f 6d5f 7573 6572 5d00 0000  le_from_user]...
-00000d40: 724b 0000 007a 254f 7267 4874 7470 4465  rK...z%OrgHttpDe
-00000d50: 6c65 6761 7465 2e72 656d 6f76 655f 726f  legate.remove_ro
-00000d60: 6c65 5f66 726f 6d5f 7573 6572 6302 0000  le_from_userc...
-00000d70: 0000 0000 0000 0000 0005 0000 0008 0000  ................
-00000d80: 0043 0000 0072 3c00 0000 2908 4e7a 0d76  .C...r<...).Nz.v
-00000d90: 312f 6f72 6773 2f72 6f6c 6573 7247 0000  1/orgs/rolesrG..
-00000da0: 0072 3e00 0000 6301 0000 0000 0000 0000  .r>...c.........
-00000db0: 0000 0002 0000 0005 0000 0053 0000 0072  ...........S...r
-00000dc0: 3400 0000 721d 0000 0072 3f00 0000 7235  4...r....r?...r5
-00000dd0: 0000 0072 1d00 0000 721d 0000 0072 1e00  ...r....r....r..
-00000de0: 0000 7238 0000 0071 0000 0072 3900 0000  ..r8...q...r9...
-00000df0: 7a35 4f72 6748 7474 7044 656c 6567 6174  z5OrgHttpDelegat
-00000e00: 652e 6f72 675f 726f 6c65 735f 666f 725f  e.org_roles_for_
-00000e10: 6f72 672e 3c6c 6f63 616c 733e 2e3c 6c69  org.<locals>.<li
-00000e20: 7374 636f 6d70 3e72 2a00 0000 722b 0000  stcomp>r*...r+..
-00000e30: 0072 4000 0000 a905 721a 0000 0072 4400  .r@.....r....rD.
-00000e40: 0000 7228 0000 0072 2900 0000 7231 0000  ..r(...r)...r1..
-00000e50: 0072 1d00 0000 721d 0000 0072 1e00 0000  .r....r....r....
-00000e60: da11 6f72 675f 726f 6c65 735f 666f 725f  ..org_roles_for_
-00000e70: 6f72 6769 0000 0072 4200 0000 7a21 4f72  orgi...rB...z!Or
-00000e80: 6748 7474 7044 656c 6567 6174 652e 6f72  gHttpDelegate.or
-00000e90: 675f 726f 6c65 735f 666f 725f 6f72 6763  g_roles_for_orgc
-00000ea0: 0300 0000 0000 0000 0000 0000 0600 0000  ................
-00000eb0: 0800 0000 4300 0000 7362 0000 007c 006a  ....C...sb...|.j
-00000ec0: 00a0 0164 01a1 017d 0374 027c 0264 028d  ...d...}.t.|.d..
-00000ed0: 017d 0474 037c 0164 038d 017d 0574 0483  .}.t.|.d...}.t..
-00000ee0: 008f 1401 007c 006a 006a 057c 037c 0474  .....|.j.j.|.|.t
-00000ef0: 067c 0583 0164 048d 0301 0057 0064 0004  .|...d.....W.d..
-00000f00: 0004 0083 0301 0064 0053 0031 0073 2a77  .......d.S.1.s*w
-00000f10: 0101 0001 0001 0059 0001 0064 0053 0029  .......Y...d.S.)
-00000f20: 054e 7a0d 7631 2f6f 7267 732f 7573 6572  .Nz.v1/orgs/user
-00000f30: 7372 4700 0000 7225 0000 0072 2700 0000  srG...r%...r'...
-00000f40: 2907 7215 0000 0072 2800 0000 7206 0000  ).r....r(...r...
-00000f50: 0072 0e00 0000 7204 0000 0072 4c00 0000  .r....r....rL...
-00000f60: 7207 0000 0029 0672 1a00 0000 7226 0000  r....).r....r&..
-00000f70: 0072 4400 0000 7228 0000 0072 2900 0000  .rD...r(...r)...
-00000f80: 7230 0000 0072 1d00 0000 721d 0000 0072  r0...r....r....r
-00000f90: 1e00 0000 da14 7265 6d6f 7665 5f75 7365  ......remove_use
-00000fa0: 725f 6672 6f6d 5f6f 7267 7600 0000 7310  r_from_orgv...s.
-00000fb0: 0000 000c 010a 020a 0208 0206 010a 0108  ................
-00000fc0: ff22 ff7a 244f 7267 4874 7470 4465 6c65  .".z$OrgHttpDele
-00000fd0: 6761 7465 2e72 656d 6f76 655f 7573 6572  gate.remove_user
-00000fe0: 5f66 726f 6d5f 6f72 6763 0200 0000 0000  _from_orgc......
-00000ff0: 0000 0000 0000 0500 0000 0800 0000 4300  ..............C.
-00001000: 0000 7360 0000 007c 006a 00a0 0164 01a1  ..s`...|.j...d..
-00001010: 017d 0274 027c 0164 028d 017d 0374 0383  .}.t.|.d...}.t..
-00001020: 008f 1001 007c 006a 006a 047c 027c 0364  .....|.j.j.|.|.d
-00001030: 038d 027d 0457 0064 0004 0004 0083 0301  ...}.W.d........
-00001040: 006e 0831 0073 2177 0101 0001 0001 0059  .n.1.s!w.......Y
-00001050: 0001 0074 05a0 067c 046a 0764 0467 0164  ...t...|.j.d.g.d
-00001060: 058d 01a1 0153 0029 064e 7224 0000 0072  .....S.).Nr$...r
-00001070: 4700 0000 723e 0000 0072 2a00 0000 722b  G...r>...r*...r+
-00001080: 0000 0029 0872 1500 0000 7228 0000 0072  ...).r....r(...r
-00001090: 0600 0000 7204 0000 0072 3a00 0000 7210  ....r....r:...r.
-000010a0: 0000 0072 2e00 0000 722f 0000 0072 4e00  ...r....r/...rN.
-000010b0: 0000 721d 0000 0072 1d00 0000 721e 0000  ..r....r....r...
-000010c0: 00da 0d67 6574 5f6f 7267 5f62 795f 6964  ...get_org_by_id
-000010d0: 8200 0000 730c 0000 000c 010a 0108 0212  ....s...........
-000010e0: 011c ff14 037a 1d4f 7267 4874 7470 4465  .....z.OrgHttpDe
-000010f0: 6c65 6761 7465 2e67 6574 5f6f 7267 5f62  legate.get_org_b
-00001100: 795f 6964 6302 0000 0000 0000 0000 0000  y_idc...........
-00001110: 0004 0000 0008 0000 0043 0000 0073 5200  .........C...sR.
-00001120: 0000 7c00 6a00 a001 6401 a101 7d02 7402  ..|.j...d...}.t.
-00001130: 7c01 6402 8d01 7d03 7403 8300 8f11 0100  |.d...}.t.......
-00001140: 7c00 6a00 6a04 7c02 7c03 6403 8d02 0100  |.j.j.|.|.d.....
-00001150: 5700 6400 0400 0400 8303 0100 6400 5300  W.d.........d.S.
-00001160: 3100 7322 7701 0100 0100 0100 5900 0100  1.s"w.......Y...
-00001170: 6400 5300 2904 4e72 2400 0000 7247 0000  d.S.).Nr$...rG..
-00001180: 0072 3e00 0000 2905 7215 0000 0072 2800  .r>...).r....r(.
-00001190: 0000 7206 0000 0072 0400 0000 724c 0000  ..r....r....rL..
-000011a0: 0029 0472 1a00 0000 7244 0000 0072 2800  .).r....rD...r(.
-000011b0: 0000 7229 0000 0072 1d00 0000 721d 0000  ..r)...r....r...
-000011c0: 0072 1e00 0000 da0a 6465 6c65 7465 5f6f  .r......delete_o
-000011d0: 7267 8b00 0000 730a 0000 000c 010a 0108  rg....s.........
-000011e0: 0212 0122 ff7a 1a4f 7267 4874 7470 4465  ...".z.OrgHttpDe
-000011f0: 6c65 6761 7465 2e64 656c 6574 655f 6f72  legate.delete_or
-00001200: 67da 0c65 6d61 696c 5f64 6f6d 6169 6e63  g..email_domainc
-00001210: 0300 0000 0000 0000 0000 0000 0600 0000  ................
-00001220: 0800 0000 4300 0000 7362 0000 007c 006a  ....C...sb...|.j
-00001230: 00a0 0164 01a1 017d 0374 027c 0164 028d  ...d...}.t.|.d..
-00001240: 017d 0474 037c 0264 038d 017d 0574 0483  .}.t.|.d...}.t..
-00001250: 008f 1401 007c 006a 006a 057c 037c 0474  .....|.j.j.|.|.t
-00001260: 067c 0583 0164 048d 0301 0057 0064 0004  .|...d.....W.d..
-00001270: 0004 0083 0301 0064 0053 0031 0073 2a77  .......d.S.1.s*w
-00001280: 0101 0001 0001 0059 0001 0064 0053 0029  .......Y...d.S.)
-00001290: 054e 7a12 7631 2f6f 7267 732f 7375 6264  .Nz.v1/orgs/subd
-000012a0: 6f6d 6169 6e73 7247 0000 0029 0172 5300  omainsrG...).rS.
-000012b0: 0000 7227 0000 0029 0772 1500 0000 7228  ..r'...).r....r(
-000012c0: 0000 0072 0600 0000 720a 0000 0072 0400  ...r....r....r..
-000012d0: 0000 7248 0000 0072 0700 0000 2906 721a  ..rH...r....).r.
-000012e0: 0000 0072 4400 0000 7253 0000 0072 2800  ...rD...rS...r(.
-000012f0: 0000 7229 0000 0072 3000 0000 721d 0000  ..r)...r0...r...
-00001300: 0072 1d00 0000 721e 0000 0072 2200 0000  .r....r....r"...
-00001310: 9200 0000 7310 0000 000c 010a 010a 0108  ....s...........
-00001320: 0206 010a 0108 ff22 ff7a 214f 7267 4874  .......".z!OrgHt
-00001330: 7470 4465 6c65 6761 7465 2e62 696e 645f  tpDelegate.bind_
-00001340: 656d 6169 6c5f 646f 6d61 696e da0f 696e  email_domain..in
-00001350: 7669 7465 645f 7573 6572 5f69 64da 1069  vited_user_id..i
-00001360: 6e76 6974 696e 675f 7573 6572 5f69 6463  nviting_user_idc
-00001370: 0400 0000 0000 0000 0000 0000 0800 0000  ................
-00001380: 0800 0000 4300 0000 7370 0000 007c 006a  ....C...sp...|.j
-00001390: 00a0 0164 01a1 017d 0474 027c 0264 028d  ...d...}.t.|.d..
-000013a0: 017d 0574 037c 0164 038d 017d 0674 0483  .}.t.|.d...}.t..
-000013b0: 008f 1301 007c 006a 006a 057c 047c 0574  .....|.j.j.|.|.t
-000013c0: 067c 0683 0164 048d 037d 0757 0064 0004  .|...d...}.W.d..
-000013d0: 0004 0083 0301 006e 0831 0073 2977 0101  .......n.1.s)w..
-000013e0: 0001 0001 0059 0001 0074 07a0 087c 076a  .....Y...t...|.j
-000013f0: 0964 0567 0164 068d 01a1 0153 0029 074e  .d.g.d.....S.).N
-00001400: 7a0f 7631 2f6f 7267 732f 696e 7669 7465  z.v1/orgs/invite
-00001410: 7372 4700 0000 2901 7254 0000 0072 2700  srG...).rT...r'.
-00001420: 0000 722a 0000 0072 2b00 0000 290a 7215  ..r*...r+...).r.
-00001430: 0000 0072 2800 0000 7206 0000 0072 0c00  ...r(...r....r..
-00001440: 0000 7204 0000 0072 2d00 0000 7207 0000  ..r....r-...r...
-00001450: 0072 0f00 0000 722e 0000 0072 2f00 0000  .r....r....r/...
-00001460: 2908 721a 0000 0072 5400 0000 7244 0000  ).r....rT...rD..
-00001470: 0072 5500 0000 7228 0000 0072 2900 0000  .rU...r(...r)...
-00001480: 7230 0000 0072 3100 0000 721d 0000 0072  r0...r1...r....r
-00001490: 1d00 0000 721e 0000 00da 1269 6e76 6974  ....r......invit
-000014a0: 655f 7573 6572 5f74 6f5f 6f72 679c 0000  e_user_to_org...
-000014b0: 0073 1200 0000 0c03 0a01 0a01 0802 0601  .s..............
-000014c0: 0a01 08ff 1cff 1405 7a22 4f72 6748 7474  ........z"OrgHtt
-000014d0: 7044 656c 6567 6174 652e 696e 7669 7465  pDelegate.invite
-000014e0: 5f75 7365 725f 746f 5f6f 7267 da09 696e  _user_to_org..in
-000014f0: 7669 7465 5f69 6463 0300 0000 0000 0000  vite_idc........
-00001500: 0000 0000 0400 0000 0800 0000 4300 0000  ............C...
-00001510: f34c 0000 007c 006a 00a0 0164 017c 019b  .L...|.j...d.|..
-00001520: 009d 02a1 017d 0374 0283 008f 1001 007c  .....}.t.......|
-00001530: 006a 006a 037c 0364 028d 0101 0057 0064  .j.j.|.d.....W.d
-00001540: 0004 0004 0083 0301 0064 0053 0031 0073  .........d.S.1.s
-00001550: 1f77 0101 0001 0001 0059 0001 0064 0053  .w.......Y...d.S
-00001560: 0029 034e 7a17 7631 2f6f 7267 732f 696e  .).Nz.v1/orgs/in
-00001570: 7669 7465 732f 6163 6365 7074 2f72 3300  vites/accept/r3.
-00001580: 0000 a904 7215 0000 0072 2800 0000 7204  ....r....r(...r.
-00001590: 0000 0072 2d00 0000 a904 721a 0000 0072  ...r-.....r....r
-000015a0: 5700 0000 7226 0000 0072 2800 0000 721d  W...r&...r(...r.
-000015b0: 0000 0072 1d00 0000 721e 0000 00da 1161  ...r....r......a
-000015c0: 6363 6570 745f 6f72 675f 696e 7669 7465  ccept_org_invite
-000015d0: aa00 0000 f308 0000 0012 0108 0210 0122  ..............."
-000015e0: ff7a 214f 7267 4874 7470 4465 6c65 6761  .z!OrgHttpDelega
-000015f0: 7465 2e61 6363 6570 745f 6f72 675f 696e  te.accept_org_in
-00001600: 7669 7465 6303 0000 0000 0000 0000 0000  vitec...........
-00001610: 0004 0000 0008 0000 0043 0000 0072 5800  .........C...rX.
-00001620: 0000 2903 4e7a 1876 312f 6f72 6773 2f69  ..).Nz.v1/orgs/i
-00001630: 6e76 6974 6573 2f64 6563 6c69 6e65 2f72  nvites/decline/r
-00001640: 3300 0000 7259 0000 0072 5a00 0000 721d  3...rY...rZ...r.
-00001650: 0000 0072 1d00 0000 721e 0000 00da 1264  ...r....r......d
-00001660: 6563 6c69 6e65 5f6f 7267 5f69 6e76 6974  ecline_org_invit
-00001670: 65b0 0000 0072 5c00 0000 7a22 4f72 6748  e....r\...z"OrgH
-00001680: 7474 7044 656c 6567 6174 652e 6465 636c  ttpDelegate.decl
-00001690: 696e 655f 6f72 675f 696e 7669 7465 6303  ine_org_invitec.
-000016a0: 0000 0000 0000 0000 0000 0005 0000 0008  ................
-000016b0: 0000 0043 0000 0073 5a00 0000 7c00 6a00  ...C...sZ...|.j.
-000016c0: a001 6401 7c01 9b00 9d02 a101 7d03 7402  ..d.|.......}.t.
-000016d0: 8300 8f0f 0100 7c00 6a00 6a03 7c03 6402  ......|.j.j.|.d.
-000016e0: 8d01 7d04 5700 6400 0400 0400 8303 0100  ..}.W.d.........
-000016f0: 6e08 3100 731e 7701 0100 0100 0100 5900  n.1.s.w.......Y.
-00001700: 0100 7404 a005 7c04 6a06 6403 6701 6404  ..t...|.j.d.g.d.
-00001710: 8d01 a101 5300 2905 4e7a 1376 312f 6f72  ....S.).Nz.v1/or
-00001720: 6773 2f69 6e76 6974 6573 2f69 642f 7233  gs/invites/id/r3
-00001730: 0000 0072 2a00 0000 722b 0000 0029 0772  ...r*...r+...).r
-00001740: 1500 0000 7228 0000 0072 0400 0000 723a  ....r(...r....r:
-00001750: 0000 0072 0f00 0000 722e 0000 0072 2f00  ...r....r....r/.
-00001760: 0000 2905 721a 0000 0072 5700 0000 7226  ..).r....rW...r&
-00001770: 0000 0072 2800 0000 7231 0000 0072 1d00  ...r(...r1...r..
-00001780: 0000 721d 0000 0072 1e00 0000 da0e 6765  ..r....r......ge
-00001790: 745f 6f72 675f 696e 7669 7465 b600 0000  t_org_invite....
-000017a0: 730a 0000 0012 0308 0210 011c ff14 027a  s..............z
-000017b0: 1e4f 7267 4874 7470 4465 6c65 6761 7465  .OrgHttpDelegate
-000017c0: 2e67 6574 5f6f 7267 5f69 6e76 6974 6563  .get_org_invitec
-000017d0: 0300 0000 0000 0000 0000 0000 0300 0000  ................
-000017e0: 0200 0000 4300 0000 7308 0000 0074 0064  ....C...s....t.d
-000017f0: 0183 0182 0129 024e 7a2b 4e6f 2048 5454  .....).Nz+No HTT
-00001800: 5020 656e 6470 6f69 6e74 2065 7869 7374  P endpoint exist
-00001810: 7320 666f 7220 7468 6973 206f 7065 7261  s for this opera
-00001820: 7469 6f6e 2129 01da 134e 6f74 496d 706c  tion!)...NotImpl
-00001830: 656d 656e 7465 6445 7272 6f72 2903 721a  ementedError).r.
-00001840: 0000 0072 2600 0000 7244 0000 0072 1d00  ...r&...rD...r..
-00001850: 0000 721d 0000 0072 1e00 0000 da18 6f72  ..r....r......or
-00001860: 675f 726f 6c65 5f66 6f72 5f75 7365 725f  g_role_for_user_
-00001870: 696e 5f6f 7267 bf00 0000 7302 0000 0008  in_org....s.....
-00001880: 037a 284f 7267 4874 7470 4465 6c65 6761  .z(OrgHttpDelega
-00001890: 7465 2e6f 7267 5f72 6f6c 655f 666f 725f  te.org_role_for_
-000018a0: 7573 6572 5f69 6e5f 6f72 6729 0146 7217  user_in_org).Fr.
-000018b0: 0000 0029 024e 4e29 1fda 085f 5f6e 616d  ...).NN)...__nam
-000018c0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-000018d0: 0c5f 5f71 7561 6c6e 616d 655f 5f72 0500  .__qualname__r..
-000018e0: 0000 da0f 5f5f 616e 6e6f 7461 7469 6f6e  ....__annotation
-000018f0: 735f 5f72 1900 0000 7202 0000 00da 0373  s__r....r......s
-00001900: 7472 7213 0000 00da 0462 6f6f 6c72 1000  trr......boolr..
-00001910: 0000 7232 0000 00da 046c 6973 7472 3b00  ..r2.....listr;.
-00001920: 0000 7212 0000 0072 4100 0000 7211 0000  ..r....rA...r...
-00001930: 0072 4a00 0000 724d 0000 0072 4f00 0000  .rJ...rM...rO...
-00001940: 7250 0000 0072 5100 0000 7252 0000 0072  rP...rQ...rR...r
-00001950: 2200 0000 720f 0000 0072 5600 0000 725b  "...r....rV...r[
-00001960: 0000 0072 5d00 0000 725e 0000 0072 6000  ...r]...r^...r`.
-00001970: 0000 da0d 5f5f 636c 6173 7363 656c 6c5f  ....__classcell_
-00001980: 5f72 1d00 0000 721d 0000 0072 1b00 0000  _r....r....r....
-00001990: 721e 0000 0072 1400 0000 1c00 0000 7384  r....r........s.
-000019a0: 0000 000a 0008 0112 0202 0904 fb06 0202  ................
-000019b0: fe02 0302 fd02 0402 fc02 0502 fb02 060a  ................
-000019c0: fa1a 161a 0b02 0e04 ff02 0102 ff02 0102  ................
-000019d0: ff06 010a ff02 0d04 ff02 0102 ff02 0102  ................
-000019e0: ff06 010a ff1a 0c1c 0d12 0c12 0912 0702  ................
-000019f0: 0b04 ff02 0102 ff02 0102 ff06 0102 ff02  ................
-00001a00: 020a fe18 0e18 0602 0704 ff02 0102 ff06  ................
-00001a10: 0102 ff02 020a fe02 0a04 ff06 0102 ff06  ................
-00001a20: 0102 ff02 0212 fe72 1400 0000 4e29 18da  .......r....N)..
-00001a30: 0674 7970 696e 6772 0200 0000 da0a 6578  .typingr......ex
-00001a40: 6365 7074 696f 6e73 7204 0000 00da 0468  ceptionsr......h
-00001a50: 7474 7072 0500 0000 7206 0000 00da 0573  ttpr....r......s
-00001a60: 6572 6465 7207 0000 00da 0864 656c 6567  erder......deleg
-00001a70: 6174 6572 0900 0000 da0e 6874 7470 5f72  ater......http_r
-00001a80: 6573 6f75 7263 6573 720a 0000 0072 0b00  esourcesr....r..
-00001a90: 0000 720c 0000 0072 0d00 0000 720e 0000  ..r....r....r...
-00001aa0: 0072 3700 0000 720f 0000 0072 1000 0000  .r7...r....r....
-00001ab0: 7211 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
-00001ac0: 1400 0000 721d 0000 0072 1d00 0000 721d  ....r....r....r.
-00001ad0: 0000 0072 1e00 0000 da08 3c6d 6f64 756c  ...r......<modul
-00001ae0: 653e 0100 0000 7310 0000 000c 020c 0210  e>....s.........
-00001af0: 010c 040c 011c 011c 0714 09              ...........
+000003b0: 6434 6414 6506 6507 1900 640a 650c 6518  d4d.e.e...d.e.e.
+000003c0: 1900 6604 642f 6430 8405 5a1d 0912 6435  ..f.d/d0..Z...d5
+000003d0: 640d 6506 6507 1900 6414 6506 6507 1900  d.e.e...d.e.e...
+000003e0: 640a 650e 6606 6431 6432 8405 5a1e 8700  d.e.f.d1d2..Z...
+000003f0: 0400 5a1f 5300 2936 da0f 4f72 6748 7474  ..Z.S.)6..OrgHtt
+00000400: 7044 656c 6567 6174 65da 1d5f 4f72 6748  pDelegate.._OrgH
+00000410: 7474 7044 656c 6567 6174 655f 5f68 7474  ttpDelegate__htt
+00000420: 705f 636c 6965 6e74 da0b 6874 7470 5f63  p_client..http_c
+00000430: 6c69 656e 7463 0200 0000 0000 0000 0000  lientc..........
+00000440: 0000 0200 0000 0200 0000 0300 0000 7314  ..............s.
+00000450: 0000 0074 0083 00a0 01a1 0001 007c 017c  ...t.........|.|
+00000460: 005f 0264 0053 00a9 014e 2903 da05 7375  ._.d.S...N)...su
+00000470: 7065 72da 085f 5f69 6e69 745f 5f72 1500  per..__init__r..
+00000480: 0000 2902 da04 7365 6c66 7216 0000 00a9  ..)...selfr.....
+00000490: 01da 095f 5f63 6c61 7373 5f5f a900 faf1  ...__class__....
+000004a0: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
+000004b0: 742f 7372 6333 3537 3831 3132 3139 312f  t/src3578112191/
+000004c0: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
+000004d0: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
+000004e0: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
+000004f0: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
+00000500: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
+00000510: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
+00000520: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
+00000530: 3336 3939 642f 726f 626f 746f 2d61 692f  3699d/roboto-ai/
+00000540: 726f 626f 746f 2d68 6f73 7465 642d 6170  roboto-hosted-ap
+00000550: 702f 7061 636b 6167 6573 2f72 6f62 6f74  p/packages/robot
+00000560: 6f5f 7364 6b2f 7372 632f 726f 626f 746f  o_sdk/src/roboto
+00000570: 5f73 646b 2f64 6f6d 6169 6e2f 6f72 6773  _sdk/domain/orgs
+00000580: 2f68 7474 705f 6465 6c65 6761 7465 2e70  /http_delegate.p
+00000590: 7972 1900 0000 1f00 0000 7304 0000 000a  yr........s.....
+000005a0: 010a 017a 184f 7267 4874 7470 4465 6c65  ...z.OrgHttpDele
+000005b0: 6761 7465 2e5f 5f69 6e69 745f 5f46 da0f  gate.__init__F..
+000005c0: 6372 6561 746f 725f 7573 6572 5f69 64da  creator_user_id.
+000005d0: 046e 616d 65da 086f 7267 5f74 7970 65da  .name..org_type.
+000005e0: 1162 696e 645f 656d 6169 6c5f 646f 6d61  .bind_email_doma
+000005f0: 696e da06 7265 7475 726e 6305 0000 0000  in..returnc.....
+00000600: 0000 0000 0000 0009 0000 0008 0000 0043  ...............C
+00000610: 0000 0073 7c00 0000 7c00 6a00 a001 6401  ...s|...|.j...d.
+00000620: a101 7d05 7402 7c01 6402 8d01 7d06 6403  ..}.t.|.d...}.d.
+00000630: 7c06 6404 3c00 7403 7c02 7c03 7c04 6405  |.d.<.t.|.|.|.d.
+00000640: 8d03 7d07 7404 8300 8f13 0100 7c00 6a00  ..}.t.......|.j.
+00000650: 6a05 7c05 7c06 7406 7c07 8301 6406 8d03  j.|.|.t.|...d...
+00000660: 7d08 5700 6400 0400 0400 8303 0100 6e08  }.W.d.........n.
+00000670: 3100 732f 7701 0100 0100 0100 5900 0100  1.s/w.......Y...
+00000680: 7407 a008 7c08 6a09 6407 6701 6408 8d01  t...|.j.d.g.d...
+00000690: a101 5300 2909 4efa 0776 312f 6f72 6773  ..S.).N..v1/orgs
+000006a0: a901 da07 7573 6572 5f69 647a 1061 7070  ....user_idz.app
+000006b0: 6c69 6361 7469 6f6e 2f6a 736f 6e7a 0c43  lication/jsonz.C
+000006c0: 6f6e 7465 6e74 2d54 7970 6529 0372 2000  ontent-Type).r .
+000006d0: 0000 7221 0000 0072 2200 0000 a903 da03  ..r!...r".......
+000006e0: 7572 6cda 0768 6561 6465 7273 da04 6461  url..headers..da
+000006f0: 7461 722a 0000 00a9 01da 096a 736f 6e5f  tar*.......json_
+00000700: 7061 7468 290a 7215 0000 0072 2800 0000  path).r....r(...
+00000710: 7206 0000 0072 0b00 0000 7204 0000 00da  r....r....r.....
+00000720: 0470 6f73 7472 0700 0000 7210 0000 00da  .postr....r.....
+00000730: 0970 6172 7365 5f6f 626a da09 6672 6f6d  .parse_obj..from
+00000740: 5f6a 736f 6e29 0972 1a00 0000 721f 0000  _json).r....r...
+00000750: 0072 2000 0000 7221 0000 0072 2200 0000  .r ...r!...r"...
+00000760: 7228 0000 0072 2900 0000 da0c 7265 7175  r(...r).....requ
+00000770: 6573 745f 626f 6479 da08 7265 7370 6f6e  est_body..respon
+00000780: 7365 721d 0000 0072 1d00 0000 721e 0000  ser....r....r...
+00000790: 00da 0a63 7265 6174 655f 6f72 6723 0000  ...create_org#..
+000007a0: 0073 1800 0000 0c07 0a01 0801 0202 0601  .s..............
+000007b0: 06ff 0804 0601 0a01 08ff 1cff 1405 7a1a  ..............z.
+000007c0: 4f72 6748 7474 7044 656c 6567 6174 652e  OrgHttpDelegate.
+000007d0: 6372 6561 7465 5f6f 7267 7226 0000 0063  create_orgr&...c
+000007e0: 0200 0000 0000 0000 0000 0000 0400 0000  ................
+000007f0: 0800 0000 4300 0000 7358 0000 007c 006a  ....C...sX...|.j
+00000800: 00a0 0164 01a1 017d 0274 0283 008f 0f01  ...d...}.t......
+00000810: 007c 006a 006a 037c 0264 028d 017d 0357  .|.j.j.|.d...}.W
+00000820: 0064 0004 0004 0083 0301 006e 0831 0073  .d.........n.1.s
+00000830: 1b77 0101 0001 0001 0059 0001 0064 0364  .w.......Y...d.d
+00000840: 0484 007c 036a 0464 0567 0164 068d 0144  ...|.j.d.g.d...D
+00000850: 0083 0153 0029 074e 7a0d 7631 2f75 7365  ...S.).Nz.v1/use
+00000860: 7273 2f6f 7267 73a9 0172 2800 0000 6301  rs/orgs..r(...c.
+00000870: 0000 0000 0000 0000 0000 0002 0000 0005  ................
+00000880: 0000 0053 0000 00f3 1600 0000 6700 7c00  ...S........g.|.
+00000890: 5d07 7d01 7400 a001 7c01 a101 9102 7102  ].}.t...|.....q.
+000008a0: 5300 721d 0000 0029 0272 1000 0000 722e  S.r....).r....r.
+000008b0: 0000 00a9 02da 022e 30da 0672 6563 6f72  ........0..recor
+000008c0: 6472 1d00 0000 721d 0000 0072 1e00 0000  dr....r....r....
+000008d0: da0a 3c6c 6973 7463 6f6d 703e 3f00 0000  ..<listcomp>?...
+000008e0: f308 0000 0006 0002 0208 ff06 ff7a 314f  .............z1O
+000008f0: 7267 4874 7470 4465 6c65 6761 7465 2e6f  rgHttpDelegate.o
+00000900: 7267 735f 666f 725f 7573 6572 2e3c 6c6f  rgs_for_user.<lo
+00000910: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+00000920: 722a 0000 0072 2b00 0000 2905 7215 0000  r*...r+...).r...
+00000930: 0072 2800 0000 7204 0000 00da 0367 6574  .r(...r......get
+00000940: 722f 0000 0029 0472 1a00 0000 7226 0000  r/...).r....r&..
+00000950: 0072 2800 0000 7231 0000 0072 1d00 0000  .r(...r1...r....
+00000960: 721d 0000 0072 1e00 0000 da0d 6f72 6773  r....r......orgs
+00000970: 5f66 6f72 5f75 7365 7239 0000 0073 0e00  _for_user9...s..
+00000980: 0000 0c01 0802 1001 1cff 0603 0c02 06fe  ................
+00000990: 7a1d 4f72 6748 7474 7044 656c 6567 6174  z.OrgHttpDelegat
+000009a0: 652e 6f72 6773 5f66 6f72 5f75 7365 7263  e.orgs_for_userc
+000009b0: 0200 0000 0000 0000 0000 0000 0500 0000  ................
+000009c0: 0800 0000 4300 0000 f364 0000 007c 006a  ....C....d...|.j
+000009d0: 00a0 0164 01a1 017d 0274 027c 0164 028d  ...d...}.t.|.d..
+000009e0: 017d 0374 0383 008f 1001 007c 006a 006a  .}.t.......|.j.j
+000009f0: 047c 027c 0364 038d 027d 0457 0064 0004  .|.|.d...}.W.d..
+00000a00: 0004 0083 0301 006e 0831 0073 2177 0101  .......n.1.s!w..
+00000a10: 0001 0001 0059 0001 0064 0464 0584 007c  .....Y...d.d...|
+00000a20: 046a 0564 0667 0164 078d 0144 0083 0153  .j.d.g.d...D...S
+00000a30: 0029 084e 7a0e 7631 2f75 7365 7273 2f72  .).Nz.v1/users/r
+00000a40: 6f6c 6573 7225 0000 00a9 0272 2800 0000  olesr%.....r(...
+00000a50: 7229 0000 0063 0100 0000 0000 0000 0000  r)...c..........
+00000a60: 0000 0200 0000 0500 0000 5300 0000 7234  ..........S...r4
+00000a70: 0000 0072 1d00 0000 a902 7212 0000 0072  ...r......r....r
+00000a80: 2e00 0000 7235 0000 0072 1d00 0000 721d  ....r5...r....r.
+00000a90: 0000 0072 1e00 0000 7238 0000 004c 0000  ...r....r8...L..
+00000aa0: 0072 3900 0000 7a36 4f72 6748 7474 7044  .r9...z6OrgHttpD
+00000ab0: 656c 6567 6174 652e 6f72 675f 726f 6c65  elegate.org_role
+00000ac0: 735f 666f 725f 7573 6572 2e3c 6c6f 6361  s_for_user.<loca
+00000ad0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 722a  ls>.<listcomp>r*
+00000ae0: 0000 0072 2b00 0000 a906 7215 0000 0072  ...r+.....r....r
+00000af0: 2800 0000 7206 0000 0072 0400 0000 723a  (...r....r....r:
+00000b00: 0000 0072 2f00 0000 2905 721a 0000 0072  ...r/...).r....r
+00000b10: 2600 0000 7228 0000 0072 2900 0000 7231  &...r(...r)...r1
+00000b20: 0000 0072 1d00 0000 721d 0000 0072 1e00  ...r....r....r..
+00000b30: 0000 da12 6f72 675f 726f 6c65 735f 666f  ....org_roles_fo
+00000b40: 725f 7573 6572 4400 0000 f310 0000 000c  r_userD.........
+00000b50: 010a 0208 0212 011c ff06 030c 0206 fe7a  ...............z
+00000b60: 224f 7267 4874 7470 4465 6c65 6761 7465  "OrgHttpDelegate
+00000b70: 2e6f 7267 5f72 6f6c 6573 5f66 6f72 5f75  .org_roles_for_u
+00000b80: 7365 724e da09 726f 6c65 5f6e 616d 65da  serN..role_name.
+00000b90: 066f 7267 5f69 6463 0400 0000 0000 0000  .org_idc........
+00000ba0: 0000 0000 0700 0000 0800 0000 4300 0000  ............C...
+00000bb0: f364 0000 007c 006a 00a0 0164 01a1 017d  .d...|.j...d...}
+00000bc0: 0474 027c 0364 028d 017d 0574 037c 017c  .t.|.d...}.t.|.|
+00000bd0: 0264 038d 027d 0674 0483 008f 1401 007c  .d...}.t.......|
+00000be0: 006a 006a 057c 047c 0574 067c 0683 0164  .j.j.|.|.t.|...d
+00000bf0: 048d 0301 0057 0064 0004 0004 0083 0301  .....W.d........
+00000c00: 0064 0053 0031 0073 2b77 0101 0001 0001  .d.S.1.s+w......
+00000c10: 0059 0001 0064 0053 00a9 054e fa0d 7631  .Y...d.S...N..v1
+00000c20: 2f6f 7267 732f 726f 6c65 73a9 0172 4300  /orgs/roles..rC.
+00000c30: 0000 2902 7226 0000 0072 4200 0000 7227  ..).r&...rB...r'
+00000c40: 0000 0029 0772 1500 0000 7228 0000 0072  ...).r....r(...r
+00000c50: 0600 0000 720d 0000 0072 0400 0000 da03  ....r....r......
+00000c60: 7075 7472 0700 0000 a907 721a 0000 0072  putr......r....r
+00000c70: 2600 0000 7242 0000 0072 4300 0000 7228  &...rB...rC...r(
+00000c80: 0000 0072 2900 0000 7230 0000 0072 1d00  ...r)...r0...r..
+00000c90: 0000 721d 0000 0072 1e00 0000 da11 6164  ..r....r......ad
+00000ca0: 645f 726f 6c65 5f66 6f72 5f75 7365 7251  d_role_for_userQ
+00000cb0: 0000 00f3 1000 0000 0c03 0a01 0c01 0802  ................
+00000cc0: 0601 0a01 08ff 22ff 7a21 4f72 6748 7474  ......".z!OrgHtt
+00000cd0: 7044 656c 6567 6174 652e 6164 645f 726f  pDelegate.add_ro
+00000ce0: 6c65 5f66 6f72 5f75 7365 7263 0400 0000  le_for_userc....
+00000cf0: 0000 0000 0000 0000 0700 0000 0800 0000  ................
+00000d00: 4300 0000 7244 0000 0072 4500 0000 2907  C...rD...rE...).
+00000d10: 7215 0000 0072 2800 0000 7206 0000 0072  r....r(...r....r
+00000d20: 0d00 0000 7204 0000 00da 0664 656c 6574  ....r......delet
+00000d30: 6572 0700 0000 7249 0000 0072 1d00 0000  er....rI...r....
+00000d40: 721d 0000 0072 1e00 0000 da15 7265 6d6f  r....r......remo
+00000d50: 7665 5f72 6f6c 655f 6672 6f6d 5f75 7365  ve_role_from_use
+00000d60: 725d 0000 0072 4b00 0000 7a25 4f72 6748  r]...rK...z%OrgH
+00000d70: 7474 7044 656c 6567 6174 652e 7265 6d6f  ttpDelegate.remo
+00000d80: 7665 5f72 6f6c 655f 6672 6f6d 5f75 7365  ve_role_from_use
+00000d90: 7263 0200 0000 0000 0000 0000 0000 0500  rc..............
+00000da0: 0000 0800 0000 4300 0000 723c 0000 0029  ......C...r<...)
+00000db0: 084e 7246 0000 0072 4700 0000 723d 0000  .NrF...rG...r=..
+00000dc0: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
+00000dd0: 0000 0500 0000 5300 0000 7234 0000 0072  ......S...r4...r
+00000de0: 1d00 0000 723e 0000 0072 3500 0000 721d  ....r>...r5...r.
+00000df0: 0000 0072 1d00 0000 721e 0000 0072 3800  ...r....r....r8.
+00000e00: 0000 7100 0000 7239 0000 007a 354f 7267  ..q...r9...z5Org
+00000e10: 4874 7470 4465 6c65 6761 7465 2e6f 7267  HttpDelegate.org
+00000e20: 5f72 6f6c 6573 5f66 6f72 5f6f 7267 2e3c  _roles_for_org.<
+00000e30: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00000e40: 703e 722a 0000 0072 2b00 0000 723f 0000  p>r*...r+...r?..
+00000e50: 00a9 0572 1a00 0000 7243 0000 0072 2800  ...r....rC...r(.
+00000e60: 0000 7229 0000 0072 3100 0000 721d 0000  ..r)...r1...r...
+00000e70: 0072 1d00 0000 721e 0000 00da 116f 7267  .r....r......org
+00000e80: 5f72 6f6c 6573 5f66 6f72 5f6f 7267 6900  _roles_for_orgi.
+00000e90: 0000 7241 0000 007a 214f 7267 4874 7470  ..rA...z!OrgHttp
+00000ea0: 4465 6c65 6761 7465 2e6f 7267 5f72 6f6c  Delegate.org_rol
+00000eb0: 6573 5f66 6f72 5f6f 7267 6303 0000 0000  es_for_orgc.....
+00000ec0: 0000 0000 0000 0006 0000 0008 0000 0043  ...............C
+00000ed0: 0000 0073 6200 0000 7c00 6a00 a001 6401  ...sb...|.j...d.
+00000ee0: a101 7d03 7402 7c02 6402 8d01 7d04 7403  ..}.t.|.d...}.t.
+00000ef0: 7c01 6403 8d01 7d05 7404 8300 8f14 0100  |.d...}.t.......
+00000f00: 7c00 6a00 6a05 7c03 7c04 7406 7c05 8301  |.j.j.|.|.t.|...
+00000f10: 6404 8d03 0100 5700 6400 0400 0400 8303  d.....W.d.......
+00000f20: 0100 6400 5300 3100 732a 7701 0100 0100  ..d.S.1.s*w.....
+00000f30: 0100 5900 0100 6400 5300 2905 4e7a 0d76  ..Y...d.S.).Nz.v
+00000f40: 312f 6f72 6773 2f75 7365 7273 7247 0000  1/orgs/usersrG..
+00000f50: 0072 2500 0000 7227 0000 0029 0772 1500  .r%...r'...).r..
+00000f60: 0000 7228 0000 0072 0600 0000 720e 0000  ..r(...r....r...
+00000f70: 0072 0400 0000 724c 0000 0072 0700 0000  .r....rL...r....
+00000f80: 2906 721a 0000 0072 2600 0000 7243 0000  ).r....r&...rC..
+00000f90: 0072 2800 0000 7229 0000 0072 3000 0000  .r(...r)...r0...
+00000fa0: 721d 0000 0072 1d00 0000 721e 0000 00da  r....r....r.....
+00000fb0: 1472 656d 6f76 655f 7573 6572 5f66 726f  .remove_user_fro
+00000fc0: 6d5f 6f72 6776 0000 0073 1000 0000 0c01  m_orgv...s......
+00000fd0: 0a02 0a02 0802 0601 0a01 08ff 22ff 7a24  ............".z$
+00000fe0: 4f72 6748 7474 7044 656c 6567 6174 652e  OrgHttpDelegate.
+00000ff0: 7265 6d6f 7665 5f75 7365 725f 6672 6f6d  remove_user_from
+00001000: 5f6f 7267 6302 0000 0000 0000 0000 0000  _orgc...........
+00001010: 0005 0000 0008 0000 0043 0000 0073 6000  .........C...s`.
+00001020: 0000 7c00 6a00 a001 6401 a101 7d02 7402  ..|.j...d...}.t.
+00001030: 7c01 6402 8d01 7d03 7403 8300 8f10 0100  |.d...}.t.......
+00001040: 7c00 6a00 6a04 7c02 7c03 6403 8d02 7d04  |.j.j.|.|.d...}.
+00001050: 5700 6400 0400 0400 8303 0100 6e08 3100  W.d.........n.1.
+00001060: 7321 7701 0100 0100 0100 5900 0100 7405  s!w.......Y...t.
+00001070: a006 7c04 6a07 6404 6701 6405 8d01 a101  ..|.j.d.g.d.....
+00001080: 5300 2906 4e72 2400 0000 7247 0000 0072  S.).Nr$...rG...r
+00001090: 3d00 0000 722a 0000 0072 2b00 0000 2908  =...r*...r+...).
+000010a0: 7215 0000 0072 2800 0000 7206 0000 0072  r....r(...r....r
+000010b0: 0400 0000 723a 0000 0072 1000 0000 722e  ....r:...r....r.
+000010c0: 0000 0072 2f00 0000 724e 0000 0072 1d00  ...r/...rN...r..
+000010d0: 0000 721d 0000 0072 1e00 0000 da0d 6765  ..r....r......ge
+000010e0: 745f 6f72 675f 6279 5f69 6482 0000 0073  t_org_by_id....s
+000010f0: 0c00 0000 0c01 0a01 0802 1201 1cff 1403  ................
+00001100: 7a1d 4f72 6748 7474 7044 656c 6567 6174  z.OrgHttpDelegat
+00001110: 652e 6765 745f 6f72 675f 6279 5f69 6463  e.get_org_by_idc
+00001120: 0200 0000 0000 0000 0000 0000 0400 0000  ................
+00001130: 0800 0000 4300 0000 7352 0000 007c 006a  ....C...sR...|.j
+00001140: 00a0 0164 01a1 017d 0274 027c 0164 028d  ...d...}.t.|.d..
+00001150: 017d 0374 0383 008f 1101 007c 006a 006a  .}.t.......|.j.j
+00001160: 047c 027c 0364 038d 0201 0057 0064 0004  .|.|.d.....W.d..
+00001170: 0004 0083 0301 0064 0053 0031 0073 2277  .......d.S.1.s"w
+00001180: 0101 0001 0001 0059 0001 0064 0053 0029  .......Y...d.S.)
+00001190: 044e 7224 0000 0072 4700 0000 723d 0000  .Nr$...rG...r=..
+000011a0: 0029 0572 1500 0000 7228 0000 0072 0600  .).r....r(...r..
+000011b0: 0000 7204 0000 0072 4c00 0000 2904 721a  ..r....rL...).r.
+000011c0: 0000 0072 4300 0000 7228 0000 0072 2900  ...rC...r(...r).
+000011d0: 0000 721d 0000 0072 1d00 0000 721e 0000  ..r....r....r...
+000011e0: 00da 0a64 656c 6574 655f 6f72 678b 0000  ...delete_org...
+000011f0: 0073 0a00 0000 0c01 0a01 0802 1201 22ff  .s............".
+00001200: 7a1a 4f72 6748 7474 7044 656c 6567 6174  z.OrgHttpDelegat
+00001210: 652e 6465 6c65 7465 5f6f 7267 da0c 656d  e.delete_org..em
+00001220: 6169 6c5f 646f 6d61 696e 6303 0000 0000  ail_domainc.....
+00001230: 0000 0000 0000 0006 0000 0008 0000 0043  ...............C
+00001240: 0000 0073 6200 0000 7c00 6a00 a001 6401  ...sb...|.j...d.
+00001250: a101 7d03 7402 7c01 6402 8d01 7d04 7403  ..}.t.|.d...}.t.
+00001260: 7c02 6403 8d01 7d05 7404 8300 8f14 0100  |.d...}.t.......
+00001270: 7c00 6a00 6a05 7c03 7c04 7406 7c05 8301  |.j.j.|.|.t.|...
+00001280: 6404 8d03 0100 5700 6400 0400 0400 8303  d.....W.d.......
+00001290: 0100 6400 5300 3100 732a 7701 0100 0100  ..d.S.1.s*w.....
+000012a0: 0100 5900 0100 6400 5300 2905 4e7a 1276  ..Y...d.S.).Nz.v
+000012b0: 312f 6f72 6773 2f73 7562 646f 6d61 696e  1/orgs/subdomain
+000012c0: 7372 4700 0000 2901 7253 0000 0072 2700  srG...).rS...r'.
+000012d0: 0000 2907 7215 0000 0072 2800 0000 7206  ..).r....r(...r.
+000012e0: 0000 0072 0a00 0000 7204 0000 0072 4800  ...r....r....rH.
+000012f0: 0000 7207 0000 0029 0672 1a00 0000 7243  ..r....).r....rC
+00001300: 0000 0072 5300 0000 7228 0000 0072 2900  ...rS...r(...r).
+00001310: 0000 7230 0000 0072 1d00 0000 721d 0000  ..r0...r....r...
+00001320: 0072 1e00 0000 7222 0000 0092 0000 0073  .r....r".......s
+00001330: 1000 0000 0c01 0a01 0a01 0802 0601 0a01  ................
+00001340: 08ff 22ff 7a21 4f72 6748 7474 7044 656c  ..".z!OrgHttpDel
+00001350: 6567 6174 652e 6269 6e64 5f65 6d61 696c  egate.bind_email
+00001360: 5f64 6f6d 6169 6eda 0f69 6e76 6974 6564  _domain..invited
+00001370: 5f75 7365 725f 6964 da10 696e 7669 7469  _user_id..inviti
+00001380: 6e67 5f75 7365 725f 6964 6304 0000 0000  ng_user_idc.....
+00001390: 0000 0000 0000 0008 0000 0008 0000 0043  ...............C
+000013a0: 0000 0073 7000 0000 7c00 6a00 a001 6401  ...sp...|.j...d.
+000013b0: a101 7d04 7402 7c02 6402 8d01 7d05 7403  ..}.t.|.d...}.t.
+000013c0: 7c01 6403 8d01 7d06 7404 8300 8f13 0100  |.d...}.t.......
+000013d0: 7c00 6a00 6a05 7c04 7c05 7406 7c06 8301  |.j.j.|.|.t.|...
+000013e0: 6404 8d03 7d07 5700 6400 0400 0400 8303  d...}.W.d.......
+000013f0: 0100 6e08 3100 7329 7701 0100 0100 0100  ..n.1.s)w.......
+00001400: 5900 0100 7407 a008 7c07 6a09 6405 6701  Y...t...|.j.d.g.
+00001410: 6406 8d01 a101 5300 2907 4efa 0f76 312f  d.....S.).N..v1/
+00001420: 6f72 6773 2f69 6e76 6974 6573 7247 0000  orgs/invitesrG..
+00001430: 0029 0172 5400 0000 7227 0000 0072 2a00  .).rT...r'...r*.
+00001440: 0000 722b 0000 0029 0a72 1500 0000 7228  ..r+...).r....r(
+00001450: 0000 0072 0600 0000 720c 0000 0072 0400  ...r....r....r..
+00001460: 0000 722d 0000 0072 0700 0000 720f 0000  ..r-...r....r...
+00001470: 0072 2e00 0000 722f 0000 0029 0872 1a00  .r....r/...).r..
+00001480: 0000 7254 0000 0072 4300 0000 7255 0000  ..rT...rC...rU..
+00001490: 0072 2800 0000 7229 0000 0072 3000 0000  .r(...r)...r0...
+000014a0: 7231 0000 0072 1d00 0000 721d 0000 0072  r1...r....r....r
+000014b0: 1e00 0000 da12 696e 7669 7465 5f75 7365  ......invite_use
+000014c0: 725f 746f 5f6f 7267 9c00 0000 7312 0000  r_to_org....s...
+000014d0: 000c 030a 010a 0108 0206 010a 0108 ff1c  ................
+000014e0: ff14 057a 224f 7267 4874 7470 4465 6c65  ...z"OrgHttpDele
+000014f0: 6761 7465 2e69 6e76 6974 655f 7573 6572  gate.invite_user
+00001500: 5f74 6f5f 6f72 67da 0969 6e76 6974 655f  _to_org..invite_
+00001510: 6964 6303 0000 0000 0000 0000 0000 0004  idc.............
+00001520: 0000 0008 0000 0043 0000 00f3 4e00 0000  .......C....N...
+00001530: 7c00 6a00 a001 6401 7c01 9b00 6402 9d03  |.j...d.|...d...
+00001540: a101 7d03 7402 8300 8f10 0100 7c00 6a00  ..}.t.......|.j.
+00001550: 6a03 7c03 6403 8d01 0100 5700 6400 0400  j.|.d.....W.d...
+00001560: 0400 8303 0100 6400 5300 3100 7320 7701  ......d.S.1.s w.
+00001570: 0100 0100 0100 5900 0100 6400 5300 2904  ......Y...d.S.).
+00001580: 4efa 1076 312f 6f72 6773 2f69 6e76 6974  N..v1/orgs/invit
+00001590: 6573 2f7a 072f 6163 6365 7074 7233 0000  es/z./acceptr3..
+000015a0: 00a9 0472 1500 0000 7228 0000 0072 0400  ...r....r(...r..
+000015b0: 0000 722d 0000 00a9 0472 1a00 0000 7258  ..r-.....r....rX
+000015c0: 0000 0072 2600 0000 7228 0000 0072 1d00  ...r&...r(...r..
+000015d0: 0000 721d 0000 0072 1e00 0000 da11 6163  ..r....r......ac
+000015e0: 6365 7074 5f6f 7267 5f69 6e76 6974 65aa  cept_org_invite.
+000015f0: 0000 00f3 0800 0000 1401 0802 1001 22ff  ..............".
+00001600: 7a21 4f72 6748 7474 7044 656c 6567 6174  z!OrgHttpDelegat
+00001610: 652e 6163 6365 7074 5f6f 7267 5f69 6e76  e.accept_org_inv
+00001620: 6974 6563 0300 0000 0000 0000 0000 0000  itec............
+00001630: 0400 0000 0800 0000 4300 0000 7259 0000  ........C...rY..
+00001640: 0029 044e 725a 0000 007a 082f 6465 636c  .).NrZ...z./decl
+00001650: 696e 6572 3300 0000 725b 0000 0072 5c00  iner3...r[...r\.
+00001660: 0000 721d 0000 0072 1d00 0000 721e 0000  ..r....r....r...
+00001670: 00da 1264 6563 6c69 6e65 5f6f 7267 5f69  ...decline_org_i
+00001680: 6e76 6974 65b0 0000 0072 5e00 0000 7a22  nvite....r^...z"
+00001690: 4f72 6748 7474 7044 656c 6567 6174 652e  OrgHttpDelegate.
+000016a0: 6465 636c 696e 655f 6f72 675f 696e 7669  decline_org_invi
+000016b0: 7465 6303 0000 0000 0000 0000 0000 0005  tec.............
+000016c0: 0000 0008 0000 0043 0000 0073 5a00 0000  .......C...sZ...
+000016d0: 7c00 6a00 a001 6401 7c01 9b00 9d02 a101  |.j...d.|.......
+000016e0: 7d03 7402 8300 8f0f 0100 7c00 6a00 6a03  }.t.......|.j.j.
+000016f0: 7c03 6402 8d01 7d04 5700 6400 0400 0400  |.d...}.W.d.....
+00001700: 8303 0100 6e08 3100 731e 7701 0100 0100  ....n.1.s.w.....
+00001710: 0100 5900 0100 7404 a005 7c04 6a06 6403  ..Y...t...|.j.d.
+00001720: 6701 6404 8d01 a101 5300 2905 4e72 5a00  g.d.....S.).NrZ.
+00001730: 0000 7233 0000 0072 2a00 0000 722b 0000  ..r3...r*...r+..
+00001740: 0029 0772 1500 0000 7228 0000 0072 0400  .).r....r(...r..
+00001750: 0000 723a 0000 0072 0f00 0000 722e 0000  ..r:...r....r...
+00001760: 0072 2f00 0000 2905 721a 0000 0072 5800  .r/...).r....rX.
+00001770: 0000 7226 0000 0072 2800 0000 7231 0000  ..r&...r(...r1..
+00001780: 0072 1d00 0000 721d 0000 0072 1e00 0000  .r....r....r....
+00001790: da0e 6765 745f 6f72 675f 696e 7669 7465  ..get_org_invite
+000017a0: b600 0000 730a 0000 0012 0308 0210 011c  ....s...........
+000017b0: ff14 027a 1e4f 7267 4874 7470 4465 6c65  ...z.OrgHttpDele
+000017c0: 6761 7465 2e67 6574 5f6f 7267 5f69 6e76  gate.get_org_inv
+000017d0: 6974 6563 0200 0000 0000 0000 0000 0000  itec............
+000017e0: 0500 0000 0800 0000 4300 0000 723c 0000  ........C...r<..
+000017f0: 0029 084e 7256 0000 0072 4700 0000 723d  .).NrV...rG...r=
+00001800: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00001810: 0200 0000 0500 0000 5300 0000 7234 0000  ........S...r4..
+00001820: 0072 1d00 0000 2902 720f 0000 0072 2e00  .r....).r....r..
+00001830: 0000 7235 0000 0072 1d00 0000 721d 0000  ..r5...r....r...
+00001840: 0072 1e00 0000 7238 0000 00c8 0000 0072  .r....r8.......r
+00001850: 3900 0000 7a37 4f72 6748 7474 7044 656c  9...z7OrgHttpDel
+00001860: 6567 6174 652e 6765 745f 696e 7669 7465  egate.get_invite
+00001870: 735f 666f 725f 6f72 672e 3c6c 6f63 616c  s_for_org.<local
+00001880: 733e 2e3c 6c69 7374 636f 6d70 3e72 2a00  s>.<listcomp>r*.
+00001890: 0000 722b 0000 0072 3f00 0000 724e 0000  ..r+...r?...rN..
+000018a0: 0072 1d00 0000 721d 0000 0072 1e00 0000  .r....r....r....
+000018b0: da13 6765 745f 696e 7669 7465 735f 666f  ..get_invites_fo
+000018c0: 725f 6f72 67bf 0000 0073 1000 0000 0c03  r_org....s......
+000018d0: 0a01 0802 1201 1cff 0603 0c02 06fe 7a23  ..............z#
+000018e0: 4f72 6748 7474 7044 656c 6567 6174 652e  OrgHttpDelegate.
+000018f0: 6765 745f 696e 7669 7465 735f 666f 725f  get_invites_for_
+00001900: 6f72 6763 0300 0000 0000 0000 0000 0000  orgc............
+00001910: 0500 0000 0800 0000 4300 0000 7366 0000  ........C...sf..
+00001920: 007c 0164 0075 0173 064a 0082 017c 006a  .|.d.u.s.J...|.j
+00001930: 00a0 0164 017c 019b 009d 02a1 017d 0374  ...d.|.......}.t
+00001940: 0283 008f 0f01 007c 006a 006a 037c 0364  .......|.j.j.|.d
+00001950: 028d 017d 0457 0064 0004 0004 0083 0301  ...}.W.d........
+00001960: 006e 0831 0073 2477 0101 0001 0001 0059  .n.1.s$w.......Y
+00001970: 0001 0074 04a0 057c 046a 0664 0367 0164  ...t...|.j.d.g.d
+00001980: 048d 01a1 0153 0029 054e 7a0e 7631 2f6f  .....S.).Nz.v1/o
+00001990: 7267 732f 726f 6c65 732f 7233 0000 0072  rgs/roles/r3...r
+000019a0: 2a00 0000 722b 0000 0029 0772 1500 0000  *...r+...).r....
+000019b0: 7228 0000 0072 0400 0000 723a 0000 0072  r(...r....r:...r
+000019c0: 1200 0000 722e 0000 0072 2f00 0000 2905  ....r....r/...).
+000019d0: 721a 0000 0072 2600 0000 7243 0000 0072  r....r&...rC...r
+000019e0: 2800 0000 7231 0000 0072 1d00 0000 721d  (...r1...r....r.
+000019f0: 0000 0072 1e00 0000 da18 6f72 675f 726f  ...r......org_ro
+00001a00: 6c65 5f66 6f72 5f75 7365 725f 696e 5f6f  le_for_user_in_o
+00001a10: 7267 cd00 0000 730c 0000 000c 0312 0208  rg....s.........
+00001a20: 0210 011c ff14 027a 284f 7267 4874 7470  .......z(OrgHttp
+00001a30: 4465 6c65 6761 7465 2e6f 7267 5f72 6f6c  Delegate.org_rol
+00001a40: 655f 666f 725f 7573 6572 5f69 6e5f 6f72  e_for_user_in_or
+00001a50: 6729 0146 7217 0000 0029 024e 4e29 20da  g).Fr....).NN) .
+00001a60: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+00001a70: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+00001a80: 655f 5f72 0500 0000 da0f 5f5f 616e 6e6f  e__r......__anno
+00001a90: 7461 7469 6f6e 735f 5f72 1900 0000 7202  tations__r....r.
+00001aa0: 0000 00da 0373 7472 7213 0000 00da 0462  .....strr......b
+00001ab0: 6f6f 6c72 1000 0000 7232 0000 00da 046c  oolr....r2.....l
+00001ac0: 6973 7472 3b00 0000 7212 0000 0072 4000  istr;...r....r@.
+00001ad0: 0000 7211 0000 0072 4a00 0000 724d 0000  ..r....rJ...rM..
+00001ae0: 0072 4f00 0000 7250 0000 0072 5100 0000  .rO...rP...rQ...
+00001af0: 7252 0000 0072 2200 0000 720f 0000 0072  rR...r"...r....r
+00001b00: 5700 0000 725d 0000 0072 5f00 0000 7260  W...r]...r_...r`
+00001b10: 0000 0072 6100 0000 7262 0000 00da 0d5f  ...ra...rb....._
+00001b20: 5f63 6c61 7373 6365 6c6c 5f5f 721d 0000  _classcell__r...
+00001b30: 0072 1d00 0000 721b 0000 0072 1e00 0000  .r....r....r....
+00001b40: 7214 0000 001c 0000 0073 9000 0000 0a00  r........s......
+00001b50: 0801 1202 0209 04fb 0602 02fe 0203 02fd  ................
+00001b60: 0204 02fc 0205 02fb 0206 0afa 1a16 1a0b  ................
+00001b70: 020e 04ff 0201 02ff 0201 02ff 0601 0aff  ................
+00001b80: 020d 04ff 0201 02ff 0201 02ff 0601 0aff  ................
+00001b90: 1a0c 1c0d 120c 1209 1207 020b 04ff 0201  ................
+00001ba0: 02ff 0201 02ff 0601 02ff 0202 0afe 180e  ................
+00001bb0: 1806 0207 04ff 0201 02ff 0601 02ff 0202  ................
+00001bc0: 0afe 020a 04ff 0601 02ff 0602 0afe 020f  ................
+00001bd0: 04ff 0601 02ff 0601 02ff 0202 12fe 7214  ..............r.
+00001be0: 0000 004e 2918 da06 7479 7069 6e67 7202  ...N)...typingr.
+00001bf0: 0000 00da 0a65 7863 6570 7469 6f6e 7372  .....exceptionsr
+00001c00: 0400 0000 da04 6874 7470 7205 0000 0072  ......httpr....r
+00001c10: 0600 0000 da05 7365 7264 6572 0700 0000  ......serder....
+00001c20: da08 6465 6c65 6761 7465 7209 0000 00da  ..delegater.....
+00001c30: 0e68 7474 705f 7265 736f 7572 6365 7372  .http_resourcesr
+00001c40: 0a00 0000 720b 0000 0072 0c00 0000 720d  ....r....r....r.
+00001c50: 0000 0072 0e00 0000 7237 0000 0072 0f00  ...r....r7...r..
+00001c60: 0000 7210 0000 0072 1100 0000 7212 0000  ..r....r....r...
+00001c70: 0072 1300 0000 7214 0000 0072 1d00 0000  .r....r....r....
+00001c80: 721d 0000 0072 1d00 0000 721e 0000 00da  r....r....r.....
+00001c90: 083c 6d6f 6475 6c65 3e01 0000 0073 1000  .<module>....s..
+00001ca0: 0000 0c02 0c02 1001 0c04 0c01 1c01 1c07  ................
+00001cb0: 1409                                     ..
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/__pycache__/http_resources.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/orgs/__pycache__/http_resources.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 540 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 1c02 0000  o.......1..d....
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 1c02 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 6401 6c00 5a00 6402 6403 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 4700 6404 6405 8400 6405  m.Z...G.d.d...d.
 00000050: 6500 6a04 8303 5a05 4700 6406 6407 8400  e.j...Z.G.d.d...
 00000060: 6407 6500 6a04 8303 5a06 4700 6408 6409  d.e.j...Z.G.d.d.
 00000070: 8400 6409 6500 6a04 8303 5a07 4700 640a  ..d.e.j...Z.G.d.
@@ -21,16 +21,16 @@
 00000140: 696c 5f64 6f6d 6169 6e4e 2908 da08 5f5f  il_domainN)...__
 00000150: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
 00000160: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
 00000170: 7204 0000 00da 0f5f 5f61 6e6e 6f74 6174  r......__annotat
 00000180: 696f 6e73 5f5f da03 7374 7272 0800 0000  ions__..strr....
 00000190: da04 626f 6f6c a900 720f 0000 0072 0f00  ..bool..r....r..
 000001a0: 0000 faf2 2f63 6f64 6562 7569 6c64 2f6f  ..../codebuild/o
-000001b0: 7574 7075 742f 7372 6331 3638 3931 3535  utput/src1689155
-000001c0: 3339 392f 7372 632f 636f 6465 7374 6172  399/src/codestar
+000001b0: 7574 7075 742f 7372 6333 3537 3831 3132  utput/src3578112
+000001c0: 3139 312f 7372 632f 636f 6465 7374 6172  191/src/codestar
 000001d0: 2d63 6f6e 6e65 6374 696f 6e73 2e75 732d  -connections.us-
 000001e0: 7765 7374 2d32 2e61 6d61 7a6f 6e61 7773  west-2.amazonaws
 000001f0: 2e63 6f6d 2f67 6974 2d68 7474 702f 3036  .com/git-http/06
 00000200: 3631 3935 3131 3233 3835 2f75 732d 7765  6195112385/us-we
 00000210: 7374 2d32 2f65 3635 3032 6138 302d 6262  st-2/e6502a80-bb
 00000220: 3465 2d34 6662 652d 3837 3263 2d35 6434  4e-4fbe-872c-5d4
 00000230: 3263 3139 3336 3939 642f 726f 626f 746f  2c193699d/roboto
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/__pycache__/org.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/orgs/__pycache__/org.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 3344 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 100d 0000  o.......1..d....
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 100d 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6402  d.l.m.Z.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6404 6405 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6404 6406 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 0100 4700 6407 6408  m.Z.m.Z...G.d.d.
 00000070: 8400 6408 8302 5a0b 6409 5300 290a e900  ..d...Z.d.S.)...
@@ -45,16 +45,16 @@
 000002c0: 0029 034e 2904 7212 0000 0072 0e00 0000  .).N).r....r....
 000002d0: 720f 0000 0072 1100 0000 a902 da06 7265  r....r........re
 000002e0: 636f 7264 7210 0000 0029 01da 0a63 7265  cordr....)...cre
 000002f0: 6174 655f 6f72 6729 07da 0363 6c73 720e  ate_org)...clsr.
 00000300: 0000 0072 0f00 0000 7210 0000 0072 1100  ...r....r....r..
 00000310: 0000 7212 0000 0072 1400 0000 a900 7217  ..r....r......r.
 00000320: 0000 00fa e72f 636f 6465 6275 696c 642f  ...../codebuild/
-00000330: 6f75 7470 7574 2f73 7263 3136 3839 3135  output/src168915
-00000340: 3533 3939 2f73 7263 2f63 6f64 6573 7461  5399/src/codesta
+00000330: 6f75 7470 7574 2f73 7263 3335 3738 3131  output/src357811
+00000340: 3231 3931 2f73 7263 2f63 6f64 6573 7461  2191/src/codesta
 00000350: 722d 636f 6e6e 6563 7469 6f6e 732e 7573  r-connections.us
 00000360: 2d77 6573 742d 322e 616d 617a 6f6e 6177  -west-2.amazonaw
 00000370: 732e 636f 6d2f 6769 742d 6874 7470 2f30  s.com/git-http/0
 00000380: 3636 3139 3531 3132 3338 352f 7573 2d77  66195112385/us-w
 00000390: 6573 742d 322f 6536 3530 3261 3830 2d62  est-2/e6502a80-b
 000003a0: 6234 652d 3466 6265 2d38 3732 632d 3564  b4e-4fbe-872c-5d
 000003b0: 3432 6331 3933 3639 3964 2f72 6f62 6f74  42c193699d/robot
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/__pycache__/org_invite.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/orgs/__pycache__/org_invite.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 1768 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 23% similar despite different names*

```diff
@@ -1,146 +1,171 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 e806 0000  o.......1..d....
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 0308 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6402  d.l.m.Z.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6404 6405 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6404 6406 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6404 6407 6c09 6d0a 5a0a 0100 4700  ..d.d.l.m.Z...G.
 00000070: 6408 6409 8400 6409 8302 5a0b 640a 5300  d.d...d...Z.d.S.
 00000080: 290b e900 0000 0029 02da 0341 6e79 da08  )......)...Any..
 00000090: 4f70 7469 6f6e 616c e903 0000 0029 01da  Optional.....)..
 000000a0: 1670 7964 616e 7469 635f 6a73 6f6e 6162  .pydantic_jsonab
 000000b0: 6c65 5f64 6963 74e9 0100 0000 2901 da0b  le_dict.....)...
 000000c0: 4f72 6744 656c 6567 6174 6529 01da 034f  OrgDelegate)...O
 000000d0: 7267 2901 da0f 4f72 6749 6e76 6974 6552  rg)...OrgInviteR
 000000e0: 6563 6f72 6463 0000 0000 0000 0000 0000  ecordc..........
-000000f0: 0000 0000 0000 0c00 0000 4000 0000 73d0  ..........@...s.
+000000f0: 0000 0000 0000 0c00 0000 4000 0000 73f6  ..........@...s.
 00000100: 0000 0065 005a 0164 005a 0255 0065 0365  ...e.Z.d.Z.U.e.e
 00000110: 0464 013c 0065 0565 0464 023c 0065 0665  .d.<.e.e.d.<.e.e
-00000120: 0464 033c 0065 0709 0464 1b64 0565 0864  .d.<.e...d.d.e.d
+00000120: 0464 033c 0065 0709 0464 1d64 0565 0864  .d.<.e...d.d.e.d
 00000130: 0665 0864 0765 0364 0865 0965 0819 0064  .e.d.e.d.e.e...d
 00000140: 0964 0066 0a64 0a64 0b84 0583 015a 0a65  .d.f.d.d.....Z.e
-00000150: 0709 0464 1b64 0c65 0864 0765 0364 0d65  ...d.d.e.d.e.d.e
+00000150: 0709 0464 1d64 0c65 0864 0765 0364 0d65  ...d.d.e.d.e.d.e
 00000160: 0965 0819 0066 0664 0e64 0f84 0583 015a  .e...f.d.d.....Z
-00000170: 0b64 0d65 0965 0819 0066 0264 1064 1184  .d.e.e...f.d.d..
-00000180: 045a 0c64 0d65 0965 0819 0066 0264 1264  .Z.d.e.e...f.d.d
-00000190: 1384 045a 0d65 0e64 0965 0866 0264 1464  ...Z.e.d.e.f.d.d
-000001a0: 1584 0483 015a 0f64 1665 0664 0765 0366  .....Z.d.e.d.e.f
-000001b0: 0464 1764 1884 045a 1064 0965 1165 0865  .d.d...Z.d.e.e.e
-000001c0: 1266 0219 0066 0264 1964 1a84 045a 1364  .f...f.d.d...Z.d
-000001d0: 0453 0029 1cda 094f 7267 496e 7669 7465  .S.)...OrgInvite
-000001e0: da18 5f4f 7267 496e 7669 7465 5f5f 6f72  .._OrgInvite__or
-000001f0: 675f 6465 6c65 6761 7465 da0f 5f4f 7267  g_delegate.._Org
-00000200: 496e 7669 7465 5f5f 6f72 67da 125f 4f72  Invite__org.._Or
-00000210: 6749 6e76 6974 655f 5f72 6563 6f72 644e  gInvite__recordN
-00000220: da0f 696e 7669 7465 645f 7573 6572 5f69  ..invited_user_i
-00000230: 64da 066f 7267 5f69 64da 0c6f 7267 5f64  d..org_id..org_d
-00000240: 656c 6567 6174 65da 1069 6e76 6974 696e  elegate..invitin
-00000250: 675f 7573 6572 5f69 64da 0672 6574 7572  g_user_id..retur
-00000260: 6e63 0500 0000 0000 0000 0000 0000 0600  nc..............
-00000270: 0000 0500 0000 4300 0000 731c 0000 007c  ......C...s....|
-00000280: 036a 007c 017c 047c 0264 018d 037d 057c  .j.|.|.|.d...}.|
-00000290: 007c 057c 0364 028d 0253 0029 034e 2903  .|.|.d...S.).N).
-000002a0: 720e 0000 0072 1100 0000 720f 0000 00a9  r....r....r.....
-000002b0: 02da 0672 6563 6f72 6472 1000 0000 2901  ...recordr....).
-000002c0: da12 696e 7669 7465 5f75 7365 725f 746f  ..invite_user_to
-000002d0: 5f6f 7267 2906 da03 636c 7372 0e00 0000  _org)...clsr....
-000002e0: 720f 0000 0072 1000 0000 7211 0000 0072  r....r....r....r
-000002f0: 1400 0000 a900 7217 0000 00fa ee2f 636f  ......r....../co
-00000300: 6465 6275 696c 642f 6f75 7470 7574 2f73  debuild/output/s
-00000310: 7263 3136 3839 3135 3533 3939 2f73 7263  rc1689155399/src
-00000320: 2f63 6f64 6573 7461 722d 636f 6e6e 6563  /codestar-connec
-00000330: 7469 6f6e 732e 7573 2d77 6573 742d 322e  tions.us-west-2.
-00000340: 616d 617a 6f6e 6177 732e 636f 6d2f 6769  amazonaws.com/gi
-00000350: 742d 6874 7470 2f30 3636 3139 3531 3132  t-http/066195112
-00000360: 3338 352f 7573 2d77 6573 742d 322f 6536  385/us-west-2/e6
-00000370: 3530 3261 3830 2d62 6234 652d 3466 6265  502a80-bb4e-4fbe
-00000380: 2d38 3732 632d 3564 3432 6331 3933 3639  -872c-5d42c19369
-00000390: 3964 2f72 6f62 6f74 6f2d 6169 2f72 6f62  9d/roboto-ai/rob
-000003a0: 6f74 6f2d 686f 7374 6564 2d61 7070 2f70  oto-hosted-app/p
-000003b0: 6163 6b61 6765 732f 726f 626f 746f 5f73  ackages/roboto_s
-000003c0: 646b 2f73 7263 2f72 6f62 6f74 6f5f 7364  dk/src/roboto_sd
-000003d0: 6b2f 646f 6d61 696e 2f6f 7267 732f 6f72  k/domain/orgs/or
-000003e0: 675f 696e 7669 7465 2e70 79da 0663 7265  g_invite.py..cre
-000003f0: 6174 6510 0000 0073 0c00 0000 0408 0201  ate....s........
-00000400: 0201 0201 06fd 0c05 7a10 4f72 6749 6e76  ........z.OrgInv
-00000410: 6974 652e 6372 6561 7465 da09 696e 7669  ite.create..invi
-00000420: 7465 5f69 64da 0775 7365 725f 6964 6304  te_id..user_idc.
-00000430: 0000 0000 0000 0000 0000 0005 0000 0004  ................
-00000440: 0000 0043 0000 0073 1a00 0000 7c02 6a00  ...C...s....|.j.
-00000450: 7c01 7c03 6401 8d02 7d04 7c00 7c04 7c02  |.|.d...}.|.|.|.
-00000460: 6402 8d02 5300 2903 4ea9 0272 1a00 0000  d...S.).N..r....
-00000470: 721b 0000 0072 1300 0000 2901 da0e 6765  r....r....)...ge
-00000480: 745f 6f72 675f 696e 7669 7465 2905 7216  t_org_invite).r.
-00000490: 0000 0072 1a00 0000 7210 0000 0072 1b00  ...r....r....r..
-000004a0: 0000 7214 0000 0072 1700 0000 7217 0000  ..r....r....r...
-000004b0: 0072 1800 0000 da07 6672 6f6d 5f69 641f  .r......from_id.
-000004c0: 0000 0073 0400 0000 0e04 0c01 7a11 4f72  ...s........z.Or
-000004d0: 6749 6e76 6974 652e 6672 6f6d 5f69 6463  gInvite.from_idc
-000004e0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-000004f0: 0400 0000 4300 0000 f318 0000 007c 006a  ....C........|.j
-00000500: 006a 017c 006a 026a 037c 0164 018d 0201  .j.|.j.j.|.d....
-00000510: 0064 0053 00a9 024e 721c 0000 0029 0472  .d.S...Nr....).r
-00000520: 0b00 0000 da11 6163 6365 7074 5f6f 7267  ......accept_org
-00000530: 5f69 6e76 6974 6572 0d00 0000 721a 0000  _inviter....r...
-00000540: 00a9 02da 0473 656c 6672 1b00 0000 7217  .....selfr....r.
-00000550: 0000 0072 1700 0000 7218 0000 00da 0661  ...r....r......a
-00000560: 6363 6570 7426 0000 00f3 0600 0000 0601  ccept&..........
-00000570: 0801 0aff 7a10 4f72 6749 6e76 6974 652e  ....z.OrgInvite.
-00000580: 6163 6365 7074 6302 0000 0000 0000 0000  acceptc.........
-00000590: 0000 0002 0000 0004 0000 0043 0000 0072  ...........C...r
-000005a0: 1f00 0000 7220 0000 0029 0472 0b00 0000  ....r ...).r....
-000005b0: da12 6465 636c 696e 655f 6f72 675f 696e  ..decline_org_in
-000005c0: 7669 7465 720d 0000 0072 1a00 0000 7222  viter....r....r"
-000005d0: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
-000005e0: 0000 da07 6465 636c 696e 652b 0000 0072  ....decline+...r
-000005f0: 2500 0000 7a11 4f72 6749 6e76 6974 652e  %...z.OrgInvite.
-00000600: 6465 636c 696e 6563 0100 0000 0000 0000  declinec........
-00000610: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
-00000620: 7308 0000 007c 006a 006a 0153 00a9 014e  s....|.j.j.S...N
-00000630: 2902 720d 0000 0072 1a00 0000 a901 7223  ).r....r......r#
-00000640: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
-00000650: 0000 721a 0000 0030 0000 0073 0200 0000  ..r....0...s....
-00000660: 0802 7a13 4f72 6749 6e76 6974 652e 696e  ..z.OrgInvite.in
-00000670: 7669 7465 5f69 6472 1400 0000 6303 0000  vite_idr....c...
-00000680: 0000 0000 0000 0000 0003 0000 0004 0000  ................
-00000690: 0043 0000 0073 2000 0000 7c01 7c00 5f00  .C...s ...|.|._.
-000006a0: 7c02 7c00 5f01 7402 7c01 6a03 7c02 6401  |.|._.t.|.j.|.d.
-000006b0: 8d02 7c00 5f04 6400 5300 2902 4e72 1300  ..|._.d.S.).Nr..
-000006c0: 0000 2905 720d 0000 0072 0b00 0000 7208  ..).r....r....r.
-000006d0: 0000 00da 036f 7267 720c 0000 0029 0372  .....orgr....).r
-000006e0: 2300 0000 7214 0000 0072 1000 0000 7217  #...r....r....r.
-000006f0: 0000 0072 1700 0000 7218 0000 00da 085f  ...r....r......_
-00000700: 5f69 6e69 745f 5f34 0000 0073 0600 0000  _init__4...s....
-00000710: 0601 0601 1401 7a12 4f72 6749 6e76 6974  ......z.OrgInvit
-00000720: 652e 5f5f 696e 6974 5f5f 6301 0000 0000  e.__init__c.....
-00000730: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-00000740: 0000 0073 0a00 0000 7400 7c00 6a01 8301  ...s....t.|.j...
-00000750: 5300 7228 0000 0029 0272 0500 0000 720d  S.r(...).r....r.
-00000760: 0000 0072 2900 0000 7217 0000 0072 1700  ...r)...r....r..
-00000770: 0000 7218 0000 00da 0774 6f5f 6469 6374  ..r......to_dict
-00000780: 3900 0000 7302 0000 000a 017a 114f 7267  9...s......z.Org
-00000790: 496e 7669 7465 2e74 6f5f 6469 6374 7228  Invite.to_dictr(
-000007a0: 0000 0029 14da 085f 5f6e 616d 655f 5fda  ...)...__name__.
-000007b0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-000007c0: 7561 6c6e 616d 655f 5f72 0700 0000 da0f  ualname__r......
-000007d0: 5f5f 616e 6e6f 7461 7469 6f6e 735f 5f72  __annotations__r
-000007e0: 0800 0000 7209 0000 00da 0b63 6c61 7373  ....r......class
-000007f0: 6d65 7468 6f64 da03 7374 7272 0300 0000  method..strr....
-00000800: 7219 0000 0072 1e00 0000 7224 0000 0072  r....r....r$...r
-00000810: 2700 0000 da08 7072 6f70 6572 7479 721a  '.....propertyr.
-00000820: 0000 0072 2b00 0000 da04 6469 6374 7202  ...r+.....dictr.
-00000830: 0000 0072 2c00 0000 7217 0000 0072 1700  ...r,...r....r..
-00000840: 0000 7217 0000 0072 1800 0000 720a 0000  ..r....r....r...
-00000850: 000b 0000 0073 4000 0000 0a00 0801 0801  .....s@.........
-00000860: 0801 0202 0206 04fb 0202 02fe 0203 02fd  ................
-00000870: 0204 02fc 0605 02fb 0206 0cfa 020e 0202  ................
-00000880: 04ff 0201 02ff 0201 02ff 0601 0cff 1206  ................
-00000890: 1205 0205 1001 1203 1a05 720a 0000 004e  ..........r....N
-000008a0: 290c da06 7479 7069 6e67 7202 0000 0072  )...typingr....r
-000008b0: 0300 0000 da05 7365 7264 6572 0500 0000  ......serder....
-000008c0: da08 6465 6c65 6761 7465 7207 0000 0072  ..delegater....r
-000008d0: 2a00 0000 7208 0000 0072 1400 0000 7209  *...r....r....r.
-000008e0: 0000 0072 0a00 0000 7217 0000 0072 1700  ...r....r....r..
-000008f0: 0000 7217 0000 0072 1800 0000 da08 3c6d  ..r....r......<m
-00000900: 6f64 756c 653e 0100 0000 730c 0000 0010  odule>....s.....
-00000910: 020c 020c 010c 010c 0112 03              ...........
+00000170: 0b65 0709 0464 1d64 0765 0364 0665 0965  .e...d.d.e.d.e.e
+00000180: 0819 0064 0965 0c64 0019 0066 0664 1064  ...d.e.d...f.d.d
+00000190: 1184 0583 015a 0d64 0d65 0965 0819 0066  .....Z.d.e.e...f
+000001a0: 0264 1264 1384 045a 0e64 0d65 0965 0819  .d.d...Z.d.e.e..
+000001b0: 0066 0264 1464 1584 045a 0f65 1064 0965  .f.d.d...Z.e.d.e
+000001c0: 0866 0264 1664 1784 0483 015a 1164 1865  .f.d.d.....Z.d.e
+000001d0: 0664 0765 0366 0464 1964 1a84 045a 1264  .d.e.f.d.d...Z.d
+000001e0: 0965 1365 0865 1466 0219 0066 0264 1b64  .e.e.e.f...f.d.d
+000001f0: 1c84 045a 1564 0453 0029 1eda 094f 7267  ...Z.d.S.)...Org
+00000200: 496e 7669 7465 da18 5f4f 7267 496e 7669  Invite.._OrgInvi
+00000210: 7465 5f5f 6f72 675f 6465 6c65 6761 7465  te__org_delegate
+00000220: da0f 5f4f 7267 496e 7669 7465 5f5f 6f72  .._OrgInvite__or
+00000230: 67da 125f 4f72 6749 6e76 6974 655f 5f72  g.._OrgInvite__r
+00000240: 6563 6f72 644e da0f 696e 7669 7465 645f  ecordN..invited_
+00000250: 7573 6572 5f69 64da 066f 7267 5f69 64da  user_id..org_id.
+00000260: 0c6f 7267 5f64 656c 6567 6174 65da 1069  .org_delegate..i
+00000270: 6e76 6974 696e 675f 7573 6572 5f69 64da  nviting_user_id.
+00000280: 0672 6574 7572 6e63 0500 0000 0000 0000  .returnc........
+00000290: 0000 0000 0600 0000 0500 0000 4300 0000  ............C...
+000002a0: 731c 0000 007c 036a 007c 017c 047c 0264  s....|.j.|.|.|.d
+000002b0: 018d 037d 057c 007c 057c 0364 028d 0253  ...}.|.|.|.d...S
+000002c0: 0029 034e 2903 720e 0000 0072 1100 0000  .).N).r....r....
+000002d0: 720f 0000 00a9 02da 0672 6563 6f72 6472  r........recordr
+000002e0: 1000 0000 2901 da12 696e 7669 7465 5f75  ....)...invite_u
+000002f0: 7365 725f 746f 5f6f 7267 2906 da03 636c  ser_to_org)...cl
+00000300: 7372 0e00 0000 720f 0000 0072 1000 0000  sr....r....r....
+00000310: 7211 0000 0072 1400 0000 a900 7217 0000  r....r......r...
+00000320: 00fa ee2f 636f 6465 6275 696c 642f 6f75  .../codebuild/ou
+00000330: 7470 7574 2f73 7263 3335 3738 3131 3231  tput/src35781121
+00000340: 3931 2f73 7263 2f63 6f64 6573 7461 722d  91/src/codestar-
+00000350: 636f 6e6e 6563 7469 6f6e 732e 7573 2d77  connections.us-w
+00000360: 6573 742d 322e 616d 617a 6f6e 6177 732e  est-2.amazonaws.
+00000370: 636f 6d2f 6769 742d 6874 7470 2f30 3636  com/git-http/066
+00000380: 3139 3531 3132 3338 352f 7573 2d77 6573  195112385/us-wes
+00000390: 742d 322f 6536 3530 3261 3830 2d62 6234  t-2/e6502a80-bb4
+000003a0: 652d 3466 6265 2d38 3732 632d 3564 3432  e-4fbe-872c-5d42
+000003b0: 6331 3933 3639 3964 2f72 6f62 6f74 6f2d  c193699d/roboto-
+000003c0: 6169 2f72 6f62 6f74 6f2d 686f 7374 6564  ai/roboto-hosted
+000003d0: 2d61 7070 2f70 6163 6b61 6765 732f 726f  -app/packages/ro
+000003e0: 626f 746f 5f73 646b 2f73 7263 2f72 6f62  boto_sdk/src/rob
+000003f0: 6f74 6f5f 7364 6b2f 646f 6d61 696e 2f6f  oto_sdk/domain/o
+00000400: 7267 732f 6f72 675f 696e 7669 7465 2e70  rgs/org_invite.p
+00000410: 79da 0663 7265 6174 6510 0000 0073 0c00  y..create....s..
+00000420: 0000 0408 0201 0201 0201 06fd 0c05 7a10  ..............z.
+00000430: 4f72 6749 6e76 6974 652e 6372 6561 7465  OrgInvite.create
+00000440: da09 696e 7669 7465 5f69 64da 0775 7365  ..invite_id..use
+00000450: 725f 6964 6304 0000 0000 0000 0000 0000  r_idc...........
+00000460: 0005 0000 0004 0000 0043 0000 0073 1a00  .........C...s..
+00000470: 0000 7c02 6a00 7c01 7c03 6401 8d02 7d04  ..|.j.|.|.d...}.
+00000480: 7c00 7c04 7c02 6402 8d02 5300 2903 4ea9  |.|.|.d...S.).N.
+00000490: 0272 1a00 0000 721b 0000 0072 1300 0000  .r....r....r....
+000004a0: 2901 da0e 6765 745f 6f72 675f 696e 7669  )...get_org_invi
+000004b0: 7465 2905 7216 0000 0072 1a00 0000 7210  te).r....r....r.
+000004c0: 0000 0072 1b00 0000 7214 0000 0072 1700  ...r....r....r..
+000004d0: 0000 7217 0000 0072 1800 0000 da07 6672  ..r....r......fr
+000004e0: 6f6d 5f69 641f 0000 0073 0400 0000 0e04  om_id....s......
+000004f0: 0c01 7a11 4f72 6749 6e76 6974 652e 6672  ..z.OrgInvite.fr
+00000500: 6f6d 5f69 6463 0300 0000 0000 0000 0000  om_idc..........
+00000510: 0000 0400 0000 0300 0000 0300 0000 7320  ..............s 
+00000520: 0000 0088 016a 007c 0264 018d 017d 0387  .....j.|.d...}..
+00000530: 0087 0166 0264 0264 0384 087c 0344 0083  ...f.d.d...|.D..
+00000540: 0153 0029 044e 2901 720f 0000 0063 0100  .S.).N).r....c..
+00000550: 0000 0000 0000 0000 0000 0200 0000 0600  ................
+00000560: 0000 1300 0000 7318 0000 0067 007c 005d  ......s....g.|.]
+00000570: 087d 0188 007c 0188 0164 008d 0291 0271  .}...|...d.....q
+00000580: 0253 0029 0172 1300 0000 7217 0000 0029  .S.).r....r....)
+00000590: 02da 022e 3072 1400 0000 a902 7216 0000  ....0r......r...
+000005a0: 0072 1000 0000 7217 0000 0072 1800 0000  .r....r....r....
+000005b0: da0a 3c6c 6973 7463 6f6d 703e 2b00 0000  ..<listcomp>+...
+000005c0: 7302 0000 0018 007a 254f 7267 496e 7669  s......z%OrgInvi
+000005d0: 7465 2e66 6f72 5f6f 7267 2e3c 6c6f 6361  te.for_org.<loca
+000005e0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 2901  ls>.<listcomp>).
+000005f0: da13 6765 745f 696e 7669 7465 735f 666f  ..get_invites_fo
+00000600: 725f 6f72 6729 0472 1600 0000 7210 0000  r_org).r....r...
+00000610: 0072 0f00 0000 da07 7265 636f 7264 7372  .r......recordsr
+00000620: 1700 0000 7220 0000 0072 1800 0000 da07  ....r ...r......
+00000630: 666f 725f 6f72 6726 0000 0073 0400 0000  for_org&...s....
+00000640: 0c04 1401 7a11 4f72 6749 6e76 6974 652e  ....z.OrgInvite.
+00000650: 666f 725f 6f72 6763 0200 0000 0000 0000  for_orgc........
+00000660: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
+00000670: f318 0000 007c 006a 006a 017c 006a 026a  .....|.j.j.|.j.j
+00000680: 037c 0164 018d 0201 0064 0053 00a9 024e  .|.d.....d.S...N
+00000690: 721c 0000 0029 0472 0b00 0000 da11 6163  r....).r......ac
+000006a0: 6365 7074 5f6f 7267 5f69 6e76 6974 6572  cept_org_inviter
+000006b0: 0d00 0000 721a 0000 00a9 02da 0473 656c  ....r........sel
+000006c0: 6672 1b00 0000 7217 0000 0072 1700 0000  fr....r....r....
+000006d0: 7218 0000 00da 0661 6363 6570 742d 0000  r......accept-..
+000006e0: 00f3 0600 0000 0601 0801 0aff 7a10 4f72  ............z.Or
+000006f0: 6749 6e76 6974 652e 6163 6365 7074 6302  gInvite.acceptc.
+00000700: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00000710: 0000 0043 0000 0072 2500 0000 7226 0000  ...C...r%...r&..
+00000720: 0029 0472 0b00 0000 da12 6465 636c 696e  .).r......declin
+00000730: 655f 6f72 675f 696e 7669 7465 720d 0000  e_org_inviter...
+00000740: 0072 1a00 0000 7228 0000 0072 1700 0000  .r....r(...r....
+00000750: 7217 0000 0072 1800 0000 da07 6465 636c  r....r......decl
+00000760: 696e 6532 0000 0072 2b00 0000 7a11 4f72  ine2...r+...z.Or
+00000770: 6749 6e76 6974 652e 6465 636c 696e 6563  gInvite.declinec
+00000780: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000790: 0100 0000 4300 0000 7308 0000 007c 006a  ....C...s....|.j
+000007a0: 006a 0153 00a9 014e 2902 720d 0000 0072  .j.S...N).r....r
+000007b0: 1a00 0000 a901 7229 0000 0072 1700 0000  ......r)...r....
+000007c0: 7217 0000 0072 1800 0000 721a 0000 0037  r....r....r....7
+000007d0: 0000 0073 0200 0000 0802 7a13 4f72 6749  ...s......z.OrgI
+000007e0: 6e76 6974 652e 696e 7669 7465 5f69 6472  nvite.invite_idr
+000007f0: 1400 0000 6303 0000 0000 0000 0000 0000  ....c...........
+00000800: 0003 0000 0004 0000 0043 0000 0073 2000  .........C...s .
+00000810: 0000 7c01 7c00 5f00 7c02 7c00 5f01 7402  ..|.|._.|.|._.t.
+00000820: 7c01 6a03 7c02 6401 8d02 7c00 5f04 6400  |.j.|.d...|._.d.
+00000830: 5300 2902 4e72 1300 0000 2905 720d 0000  S.).Nr....).r...
+00000840: 0072 0b00 0000 7208 0000 00da 036f 7267  .r....r......org
+00000850: 720c 0000 0029 0372 2900 0000 7214 0000  r....).r)...r...
+00000860: 0072 1000 0000 7217 0000 0072 1700 0000  .r....r....r....
+00000870: 7218 0000 00da 085f 5f69 6e69 745f 5f3b  r......__init__;
+00000880: 0000 0073 0600 0000 0601 0601 1401 7a12  ...s..........z.
+00000890: 4f72 6749 6e76 6974 652e 5f5f 696e 6974  OrgInvite.__init
+000008a0: 5f5f 6301 0000 0000 0000 0000 0000 0001  __c.............
+000008b0: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
+000008c0: 7400 7c00 6a01 8301 5300 722e 0000 0029  t.|.j...S.r....)
+000008d0: 0272 0500 0000 720d 0000 0072 2f00 0000  .r....r....r/...
+000008e0: 7217 0000 0072 1700 0000 7218 0000 00da  r....r....r.....
+000008f0: 0774 6f5f 6469 6374 4000 0000 7302 0000  .to_dict@...s...
+00000900: 000a 017a 114f 7267 496e 7669 7465 2e74  ...z.OrgInvite.t
+00000910: 6f5f 6469 6374 722e 0000 0029 16da 085f  o_dictr....)..._
+00000920: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+00000930: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+00000940: 5f72 0700 0000 da0f 5f5f 616e 6e6f 7461  _r......__annota
+00000950: 7469 6f6e 735f 5f72 0800 0000 7209 0000  tions__r....r...
+00000960: 00da 0b63 6c61 7373 6d65 7468 6f64 da03  ...classmethod..
+00000970: 7374 7272 0300 0000 7219 0000 0072 1e00  strr....r....r..
+00000980: 0000 da04 6c69 7374 7224 0000 0072 2a00  ....listr$...r*.
+00000990: 0000 722d 0000 00da 0870 726f 7065 7274  ..r-.....propert
+000009a0: 7972 1a00 0000 7231 0000 00da 0464 6963  yr....r1.....dic
+000009b0: 7472 0200 0000 7232 0000 0072 1700 0000  tr....r2...r....
+000009c0: 7217 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
+000009d0: 0a00 0000 0b00 0000 7352 0000 000a 0008  ........sR......
+000009e0: 0108 0108 0102 0202 0604 fb02 0202 fe02  ................
+000009f0: 0302 fd02 0402 fc06 0502 fb02 060c fa02  ................
+00000a00: 0e02 0204 ff02 0102 ff02 0102 ff06 010c  ................
+00000a10: ff02 0602 0204 ff02 0102 ff06 0102 ff06  ................
+00000a20: 020c fe12 0612 0502 0510 0112 031a 0572  ...............r
+00000a30: 0a00 0000 4e29 0cda 0674 7970 696e 6772  ....N)...typingr
+00000a40: 0200 0000 7203 0000 00da 0573 6572 6465  ....r......serde
+00000a50: 7205 0000 00da 0864 656c 6567 6174 6572  r......delegater
+00000a60: 0700 0000 7230 0000 0072 0800 0000 7214  ....r0...r....r.
+00000a70: 0000 0072 0900 0000 720a 0000 0072 1700  ...r....r....r..
+00000a80: 0000 7217 0000 0072 1700 0000 7218 0000  ..r....r....r...
+00000a90: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00000aa0: 0c00 0000 1002 0c02 0c01 0c01 0c01 1203  ................
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/__pycache__/org_role.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/orgs/__pycache__/org_role.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 1751 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 d706 0000  o.......1..d....
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 d706 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6402  d.l.m.Z.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6404 6405 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6404 6406 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6404 6407 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 0100 4700 6408 6409 8400 6409 8302 5a0c  ..G.d.d...d...Z.
@@ -44,16 +44,16 @@
 000002b0: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
 000002c0: 0000 0600 0000 1300 0000 f318 0000 0067  ...............g
 000002d0: 007c 005d 087d 0188 007c 0188 0164 008d  .|.].}...|...d..
 000002e0: 0291 0271 0253 00a9 01a9 02da 0672 6563  ...q.S.......rec
 000002f0: 6f72 6472 1000 0000 a900 a902 da02 2e30  ordr...........0
 00000300: 7216 0000 00a9 02da 0363 6c73 7210 0000  r........clsr...
 00000310: 0072 1700 0000 faec 2f63 6f64 6562 7569  .r....../codebui
-00000320: 6c64 2f6f 7574 7075 742f 7372 6331 3638  ld/output/src168
-00000330: 3931 3535 3339 392f 7372 632f 636f 6465  9155399/src/code
+00000320: 6c64 2f6f 7574 7075 742f 7372 6333 3537  ld/output/src357
+00000330: 3831 3132 3139 312f 7372 632f 636f 6465  8112191/src/code
 00000340: 7374 6172 2d63 6f6e 6e65 6374 696f 6e73  star-connections
 00000350: 2e75 732d 7765 7374 2d32 2e61 6d61 7a6f  .us-west-2.amazo
 00000360: 6e61 7773 2e63 6f6d 2f67 6974 2d68 7474  naws.com/git-htt
 00000370: 702f 3036 3631 3935 3131 3233 3835 2f75  p/066195112385/u
 00000380: 732d 7765 7374 2d32 2f65 3635 3032 6138  s-west-2/e6502a8
 00000390: 302d 6262 3465 2d34 6662 652d 3837 3263  0-bb4e-4fbe-872c
 000003a0: 2d35 6434 3263 3139 3336 3939 642f 726f  -5d42c193699d/ro
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/__pycache__/record.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/orgs/__pycache__/record.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 726 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 d602 0000  o.......1..d....
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 d602 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 9200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 6c02 6d03 5a03 0100 4700 6404 6405  d.l.m.Z...G.d.d.
 00000050: 8400 6405 6504 6500 6a05 8304 5a06 4700  ..d.e.e.j...Z.G.
 00000060: 6406 6407 8400 6407 6504 6500 6a05 8304  d.d...d.e.e.j...
 00000070: 5a07 4700 6408 6409 8400 6409 6501 6a08  Z.G.d.d...d.e.j.
@@ -17,16 +17,16 @@
 00000100: 0264 015a 0364 025a 0464 0353 0029 04da  .d.Z.d.Z.d.S.)..
 00000110: 074f 7267 5479 7065 da0a 696e 6469 7669  .OrgType..indivi
 00000120: 6475 616c da04 7465 616d 4e29 05da 085f  dual..teamN)..._
 00000130: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
 00000140: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
 00000150: 5f72 0600 0000 7207 0000 00a9 0072 0b00  _r....r......r..
 00000160: 0000 720b 0000 00fa ea2f 636f 6465 6275  ..r....../codebu
-00000170: 696c 642f 6f75 7470 7574 2f73 7263 3136  ild/output/src16
-00000180: 3839 3135 3533 3939 2f73 7263 2f63 6f64  89155399/src/cod
+00000170: 696c 642f 6f75 7470 7574 2f73 7263 3335  ild/output/src35
+00000180: 3738 3131 3231 3931 2f73 7263 2f63 6f64  78112191/src/cod
 00000190: 6573 7461 722d 636f 6e6e 6563 7469 6f6e  estar-connection
 000001a0: 732e 7573 2d77 6573 742d 322e 616d 617a  s.us-west-2.amaz
 000001b0: 6f6e 6177 732e 636f 6d2f 6769 742d 6874  onaws.com/git-ht
 000001c0: 7470 2f30 3636 3139 3531 3132 3338 352f  tp/066195112385/
 000001d0: 7573 2d77 6573 742d 322f 6536 3530 3261  us-west-2/e6502a
 000001e0: 3830 2d62 6234 652d 3466 6265 2d38 3732  80-bb4e-4fbe-872
 000001f0: 632d 3564 3432 6331 3933 3639 3964 2f72  c-5d42c193699d/r
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/delegate.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/orgs/delegate.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,14 +72,20 @@
     @abc.abstractmethod
     def invite_user_to_org(
         self, invited_user_id: str, org_id: str, inviting_user_id: Optional[str] = None
     ) -> OrgInviteRecord:
         raise NotImplementedError("invite_user_to_org")
 
     @abc.abstractmethod
+    def get_invites_for_org(
+        self, org_id: Optional[str] = None
+    ) -> list[OrgInviteRecord]:
+        raise NotImplementedError("get_invites_for_org")
+
+    @abc.abstractmethod
     def accept_org_invite(self, invite_id: str, user_id: Optional[str] = None):
         raise NotImplementedError("accept_org_invite")
 
     @abc.abstractmethod
     def decline_org_invite(self, invite_id: str, user_id: Optional[str] = None):
         raise NotImplementedError("accept_org_invite")
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/http_delegate.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/orgs/http_delegate.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,53 +51,53 @@
             response = self.__http_client.post(
                 url=url, headers=headers, data=pydantic_jsonable_dict(request_body)
             )
 
         return OrgRecord.parse_obj(response.from_json(json_path=["data"]))
 
     def orgs_for_user(self, user_id: Optional[str]) -> list[OrgRecord]:
-        url = self.__http_client.url("v1/orgs/list")
+        url = self.__http_client.url("v1/users/orgs")
 
         with RobotoHttpExceptionParse():
             response = self.__http_client.get(url=url)
 
         return [
             OrgRecord.parse_obj(record)
             for record in response.from_json(json_path=["data"])
         ]
 
     def org_roles_for_user(self, user_id: Optional[str]) -> list[OrgRoleRecord]:
-        url = self.__http_client.url("v1/orgs/roles/user")
+        url = self.__http_client.url("v1/users/roles")
 
         headers = headers_for_org_and_user(user_id=user_id)
 
         with RobotoHttpExceptionParse():
             response = self.__http_client.get(url=url, headers=headers)
 
         return [
             OrgRoleRecord.parse_obj(record)
             for record in response.from_json(json_path=["data"])
         ]
 
     def add_role_for_user(
         self, user_id: str, role_name: OrgRoleName, org_id: Optional[str] = None
     ):
-        url = self.__http_client.url("v1/orgs/roles/user")
+        url = self.__http_client.url("v1/orgs/roles")
         headers = headers_for_org_and_user(org_id=org_id)
         request_body = ModifyRoleForUserRequest(user_id=user_id, role_name=role_name)
 
         with RobotoHttpExceptionParse():
             self.__http_client.put(
                 url=url, headers=headers, data=pydantic_jsonable_dict(request_body)
             )
 
     def remove_role_from_user(
         self, user_id: str, role_name: OrgRoleName, org_id: Optional[str] = None
     ):
-        url = self.__http_client.url("v1/orgs/roles/user")
+        url = self.__http_client.url("v1/orgs/roles")
         headers = headers_for_org_and_user(org_id=org_id)
         request_body = ModifyRoleForUserRequest(user_id=user_id, role_name=role_name)
 
         with RobotoHttpExceptionParse():
             self.__http_client.delete(
                 url=url, headers=headers, data=pydantic_jsonable_dict(request_body)
             )
@@ -164,31 +164,51 @@
             response = self.__http_client.post(
                 url=url, headers=headers, data=pydantic_jsonable_dict(request_body)
             )
 
         return OrgInviteRecord.parse_obj(response.from_json(json_path=["data"]))
 
     def accept_org_invite(self, invite_id: str, user_id: Optional[str] = None):
-        url = self.__http_client.url(f"v1/orgs/invites/accept/{invite_id}")
+        url = self.__http_client.url(f"v1/orgs/invites/{invite_id}/accept")
 
         with RobotoHttpExceptionParse():
             self.__http_client.post(url=url)
 
     def decline_org_invite(self, invite_id: str, user_id: Optional[str] = None):
-        url = self.__http_client.url(f"v1/orgs/invites/decline/{invite_id}")
+        url = self.__http_client.url(f"v1/orgs/invites/{invite_id}/decline")
 
         with RobotoHttpExceptionParse():
             self.__http_client.post(url=url)
 
     def get_org_invite(
         self, invite_id: str, user_id: Optional[str] = None
     ) -> OrgInviteRecord:
-        url = self.__http_client.url(f"v1/orgs/invites/id/{invite_id}")
+        url = self.__http_client.url(f"v1/orgs/invites/{invite_id}")
 
         with RobotoHttpExceptionParse():
             response = self.__http_client.get(url=url)
         return OrgInviteRecord.parse_obj(response.from_json(json_path=["data"]))
 
+    def get_invites_for_org(
+        self, org_id: Optional[str] = None
+    ) -> list[OrgInviteRecord]:
+        url = self.__http_client.url("v1/orgs/invites")
+        headers = headers_for_org_and_user(org_id=org_id)
+
+        with RobotoHttpExceptionParse():
+            response = self.__http_client.get(url=url, headers=headers)
+
+        return [
+            OrgInviteRecord.parse_obj(record)
+            for record in response.from_json(json_path=["data"])
+        ]
+
     def org_role_for_user_in_org(
         self, user_id: Optional[str] = None, org_id: Optional[str] = None
     ) -> OrgRoleRecord:
-        raise NotImplementedError("No HTTP endpoint exists for this operation!")
+        assert user_id is not None
+
+        url = self.__http_client.url(f"v1/orgs/roles/{user_id}")
+
+        with RobotoHttpExceptionParse():
+            response = self.__http_client.get(url=url)
+        return OrgRoleRecord.parse_obj(response.from_json(json_path=["data"]))
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/http_resources.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/orgs/http_resources.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/org.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/orgs/org.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/org_invite.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/orgs/org_invite.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,14 +31,21 @@
     @classmethod
     def from_id(
         cls, invite_id: str, org_delegate: OrgDelegate, user_id: Optional[str] = None
     ):
         record = org_delegate.get_org_invite(invite_id=invite_id, user_id=user_id)
         return cls(record=record, org_delegate=org_delegate)
 
+    @classmethod
+    def for_org(
+        cls, org_delegate: OrgDelegate, org_id: Optional[str] = None
+    ) -> list["OrgInvite"]:
+        records = org_delegate.get_invites_for_org(org_id=org_id)
+        return [cls(record=record, org_delegate=org_delegate) for record in records]
+
     def accept(self, user_id: Optional[str]):
         self.__org_delegate.accept_org_invite(
             invite_id=self.__record.invite_id, user_id=user_id
         )
 
     def decline(self, user_id: Optional[str]):
         self.__org_delegate.decline_org_invite(
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/org_role.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/orgs/org_role.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/orgs/record.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/orgs/record.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/__pycache__/__init__.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/tokens/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 387 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 8301 0000  o.......1..d....
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 8301 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6700  ..d.d.l.m.Z...g.
 00000070: 6406 a201 5a0b 6407 5300 2908 e901 0000  d...Z.d.S.).....
@@ -18,16 +18,16 @@
 00000110: 7202 0000 00da 0d68 7474 705f 6465 6c65  r......http_dele
 00000120: 6761 7465 7203 0000 00da 0e68 7474 705f  gater......http_
 00000130: 7265 736f 7572 6365 7372 0400 0000 da06  resourcesr......
 00000140: 7265 636f 7264 7205 0000 0072 0600 0000  recordr....r....
 00000150: da05 746f 6b65 6e72 0700 0000 da07 5f5f  ..tokenr......__
 00000160: 616c 6c5f 5fa9 0072 0e00 0000 720e 0000  all__..r....r...
 00000170: 00fa ee2f 636f 6465 6275 696c 642f 6f75  .../codebuild/ou
-00000180: 7470 7574 2f73 7263 3136 3839 3135 3533  tput/src16891553
-00000190: 3939 2f73 7263 2f63 6f64 6573 7461 722d  99/src/codestar-
+00000180: 7470 7574 2f73 7263 3335 3738 3131 3231  tput/src35781121
+00000190: 3931 2f73 7263 2f63 6f64 6573 7461 722d  91/src/codestar-
 000001a0: 636f 6e6e 6563 7469 6f6e 732e 7573 2d77  connections.us-w
 000001b0: 6573 742d 322e 616d 617a 6f6e 6177 732e  est-2.amazonaws.
 000001c0: 636f 6d2f 6769 742d 6874 7470 2f30 3636  com/git-http/066
 000001d0: 3139 3531 3132 3338 352f 7573 2d77 6573  195112385/us-wes
 000001e0: 742d 322f 6536 3530 3261 3830 2d62 6234  t-2/e6502a80-bb4
 000001f0: 652d 3466 6265 2d38 3732 632d 3564 3432  e-4fbe-872c-5d42
 00000200: 6331 3933 3639 3964 2f72 6f62 6f74 6f2d  c193699d/roboto-
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/__pycache__/delegate.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/tokens/__pycache__/delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 888 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,101 +1,103 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 7803 0000  o.......1..dx...
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 8d03 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6403 6404 6c03 6d04 5a04 0100 4700  ..d.d.l.m.Z...G.
 00000050: 6405 6406 8400 6406 6500 6a05 8303 5a06  d.d...d.e.j...Z.
 00000060: 6401 5300 2907 e900 0000 004e 2901 da08  d.S.)......N)...
 00000070: 4f70 7469 6f6e 616c e901 0000 0029 01da  Optional.....)..
 00000080: 0b54 6f6b 656e 5265 636f 7264 6300 0000  .TokenRecordc...
-00000090: 0000 0000 0000 0000 0000 0000 000b 0000  ................
-000000a0: 0000 0000 0073 9800 0000 6500 5a01 6400  .....s....e.Z.d.
+00000090: 0000 0000 0000 0000 0000 0000 000c 0000  ................
+000000a0: 0000 0000 0073 a000 0000 6500 5a01 6400  .....s....e.Z.d.
 000000b0: 5a02 8700 6601 6401 6402 8408 5a03 6504  Z...f.d.d...Z.e.
-000000c0: 6a05 6403 6506 6507 1900 6404 6508 6509  j.d.e.e...d.e.e.
-000000d0: 1900 6604 6405 6406 8404 8301 5a0a 6504  ..f.d.d.....Z.e.
-000000e0: 6a05 6403 6506 6507 1900 6407 650b 6408  j.d.e.e...d.e.d.
-000000f0: 6507 6409 6506 6507 1900 6404 6509 660a  e.d.e.e...d.e.f.
-00000100: 640a 640b 8404 8301 5a0c 6504 6a05 640c  d.d.....Z.e.j.d.
-00000110: 6507 6404 640d 6604 640e 640f 8404 8301  e.d.d.f.d.d.....
-00000120: 5a0d 6504 6a05 640c 6507 6404 6509 6604  Z.e.j.d.e.d.e.f.
-00000130: 6410 6411 8404 8301 5a0e 8700 0400 5a0f  d.d.....Z.....Z.
-00000140: 5300 2912 da0d 546f 6b65 6e44 656c 6567  S.)...TokenDeleg
-00000150: 6174 6563 0100 0000 0000 0000 0000 0000  atec............
-00000160: 0100 0000 0200 0000 0300 0000 730e 0000  ............s...
-00000170: 0074 0083 00a0 01a1 0001 0064 0053 0029  .t.........d.S.)
-00000180: 014e 2902 da05 7375 7065 72da 085f 5f69  .N)...super..__i
-00000190: 6e69 745f 5f29 01da 0473 656c 66a9 01da  nit__)...self...
-000001a0: 095f 5f63 6c61 7373 5f5f a900 faee 2f63  .__class__..../c
-000001b0: 6f64 6562 7569 6c64 2f6f 7574 7075 742f  odebuild/output/
-000001c0: 7372 6331 3638 3931 3535 3339 392f 7372  src1689155399/sr
-000001d0: 632f 636f 6465 7374 6172 2d63 6f6e 6e65  c/codestar-conne
-000001e0: 6374 696f 6e73 2e75 732d 7765 7374 2d32  ctions.us-west-2
-000001f0: 2e61 6d61 7a6f 6e61 7773 2e63 6f6d 2f67  .amazonaws.com/g
-00000200: 6974 2d68 7474 702f 3036 3631 3935 3131  it-http/06619511
-00000210: 3233 3835 2f75 732d 7765 7374 2d32 2f65  2385/us-west-2/e
-00000220: 3635 3032 6138 302d 6262 3465 2d34 6662  6502a80-bb4e-4fb
-00000230: 652d 3837 3263 2d35 6434 3263 3139 3336  e-872c-5d42c1936
-00000240: 3939 642f 726f 626f 746f 2d61 692f 726f  99d/roboto-ai/ro
-00000250: 626f 746f 2d68 6f73 7465 642d 6170 702f  boto-hosted-app/
-00000260: 7061 636b 6167 6573 2f72 6f62 6f74 6f5f  packages/roboto_
-00000270: 7364 6b2f 7372 632f 726f 626f 746f 5f73  sdk/src/roboto_s
-00000280: 646b 2f64 6f6d 6169 6e2f 746f 6b65 6e73  dk/domain/tokens
-00000290: 2f64 656c 6567 6174 652e 7079 7207 0000  /delegate.pyr...
-000002a0: 0009 0000 0073 0200 0000 0e01 7a16 546f  .....s......z.To
-000002b0: 6b65 6e44 656c 6567 6174 652e 5f5f 696e  kenDelegate.__in
-000002c0: 6974 5f5f da07 7573 6572 5f69 64da 0672  it__..user_id..r
-000002d0: 6574 7572 6e63 0200 0000 0000 0000 0000  eturnc..........
-000002e0: 0000 0200 0000 0200 0000 4300 0000 f308  ..........C.....
-000002f0: 0000 0074 0064 0183 0182 0129 024e da13  ...t.d.....).N..
-00000300: 6765 745f 746f 6b65 6e73 5f66 6f72 5f75  get_tokens_for_u
-00000310: 7365 72a9 01da 134e 6f74 496d 706c 656d  ser....NotImplem
-00000320: 656e 7465 6445 7272 6f72 2902 7208 0000  entedError).r...
-00000330: 0072 0d00 0000 720b 0000 0072 0b00 0000  .r....r....r....
-00000340: 720c 0000 0072 1000 0000 0c00 0000 f302  r....r..........
-00000350: 0000 0008 027a 2154 6f6b 656e 4465 6c65  .....z!TokenDele
-00000360: 6761 7465 2e67 6574 5f74 6f6b 656e 735f  gate.get_tokens_
-00000370: 666f 725f 7573 6572 da0b 6578 7069 7279  for_user..expiry
-00000380: 5f64 6179 73da 046e 616d 65da 0b64 6573  _days..name..des
-00000390: 6372 6970 7469 6f6e 6305 0000 0000 0000  criptionc.......
-000003a0: 0000 0000 0005 0000 0002 0000 0043 0000  .............C..
-000003b0: 0072 0f00 0000 2902 4eda 0c63 7265 6174  .r....).N..creat
-000003c0: 655f 746f 6b65 6e72 1100 0000 2905 7208  e_tokenr....).r.
-000003d0: 0000 0072 0d00 0000 7214 0000 0072 1500  ...r....r....r..
-000003e0: 0000 7216 0000 0072 0b00 0000 720b 0000  ..r....r....r...
-000003f0: 0072 0c00 0000 7217 0000 0010 0000 0073  .r....r........s
-00000400: 0200 0000 0808 7a1a 546f 6b65 6e44 656c  ......z.TokenDel
-00000410: 6567 6174 652e 6372 6561 7465 5f74 6f6b  egate.create_tok
-00000420: 656e da08 746f 6b65 6e5f 6964 4e63 0200  en..token_idNc..
-00000430: 0000 0000 0000 0000 0000 0200 0000 0200  ................
-00000440: 0000 4300 0000 720f 0000 0029 024e da0c  ..C...r....).N..
-00000450: 6465 6c65 7465 5f74 6f6b 656e 7211 0000  delete_tokenr...
-00000460: 00a9 0272 0800 0000 7218 0000 0072 0b00  ...r....r....r..
-00000470: 0000 720b 0000 0072 0c00 0000 7219 0000  ..r....r....r...
-00000480: 001a 0000 0072 1300 0000 7a1a 546f 6b65  .....r....z.Toke
-00000490: 6e44 656c 6567 6174 652e 6465 6c65 7465  nDelegate.delete
-000004a0: 5f74 6f6b 656e 6302 0000 0000 0000 0000  _tokenc.........
-000004b0: 0000 0002 0000 0002 0000 0043 0000 0072  ...........C...r
-000004c0: 0f00 0000 2902 4eda 1567 6574 5f74 6f6b  ....).N..get_tok
-000004d0: 656e 5f62 795f 746f 6b65 6e5f 6964 7211  en_by_token_idr.
-000004e0: 0000 0072 1a00 0000 720b 0000 0072 0b00  ...r....r....r..
-000004f0: 0000 720c 0000 0072 1b00 0000 1e00 0000  ..r....r........
-00000500: 7213 0000 007a 2354 6f6b 656e 4465 6c65  r....z#TokenDele
-00000510: 6761 7465 2e67 6574 5f74 6f6b 656e 5f62  gate.get_token_b
-00000520: 795f 746f 6b65 6e5f 6964 2910 da08 5f5f  y_token_id)...__
-00000530: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00000540: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00000550: 7207 0000 00da 0361 6263 da0e 6162 7374  r......abc..abst
-00000560: 7261 6374 6d65 7468 6f64 7202 0000 00da  ractmethodr.....
-00000570: 0373 7472 da04 6c69 7374 7204 0000 0072  .str..listr....r
-00000580: 1000 0000 da03 696e 7472 1700 0000 7219  ......intr....r.
-00000590: 0000 0072 1b00 0000 da0d 5f5f 636c 6173  ...r......__clas
-000005a0: 7363 656c 6c5f 5f72 0b00 0000 720b 0000  scell__r....r...
-000005b0: 0072 0900 0000 720c 0000 0072 0500 0000  .r....r....r....
-000005c0: 0800 0000 7328 0000 0008 000c 0104 031c  ....s(..........
-000005d0: 0104 0302 0106 0202 fe02 0302 fd02 0402  ................
-000005e0: fc06 0502 fb02 060c fa04 0914 0104 031c  ................
-000005f0: 0172 0500 0000 2907 721f 0000 00da 0674  .r....).r......t
-00000600: 7970 696e 6772 0200 0000 da06 7265 636f  ypingr......reco
-00000610: 7264 7204 0000 00da 0341 4243 7205 0000  rdr......ABCr...
-00000620: 0072 0b00 0000 720b 0000 0072 0b00 0000  .r....r....r....
-00000630: 720c 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00000640: 0000 0073 0800 0000 0801 0c01 0c02 1603  ...s............
+000000c0: 6a05 6412 6404 6506 6507 1900 6405 6508  j.d.d.e.e...d.e.
+000000d0: 6509 1900 6604 6406 6407 8405 8301 5a0a  e...f.d.d.....Z.
+000000e0: 6504 6a05 0903 0903 6413 6408 650b 6409  e.j.....d.d.e.d.
+000000f0: 6507 6404 6506 6507 1900 640a 6506 6507  e.d.e.e...d.e.e.
+00000100: 1900 6405 6509 660a 640b 640c 8405 8301  ..d.e.f.d.d.....
+00000110: 5a0c 6504 6a05 640d 6507 6405 6403 6604  Z.e.j.d.e.d.d.f.
+00000120: 640e 640f 8404 8301 5a0d 6504 6a05 640d  d.d.....Z.e.j.d.
+00000130: 6507 6405 6509 6604 6410 6411 8404 8301  e.d.e.f.d.d.....
+00000140: 5a0e 8700 0400 5a0f 5300 2914 da0d 546f  Z.....Z.S.)...To
+00000150: 6b65 6e44 656c 6567 6174 6563 0100 0000  kenDelegatec....
+00000160: 0000 0000 0000 0000 0100 0000 0200 0000  ................
+00000170: 0300 0000 730e 0000 0074 0083 00a0 01a1  ....s....t......
+00000180: 0001 0064 0053 00a9 014e 2902 da05 7375  ...d.S...N)...su
+00000190: 7065 72da 085f 5f69 6e69 745f 5f29 01da  per..__init__)..
+000001a0: 0473 656c 66a9 01da 095f 5f63 6c61 7373  .self....__class
+000001b0: 5f5f a900 faee 2f63 6f64 6562 7569 6c64  __..../codebuild
+000001c0: 2f6f 7574 7075 742f 7372 6333 3537 3831  /output/src35781
+000001d0: 3132 3139 312f 7372 632f 636f 6465 7374  12191/src/codest
+000001e0: 6172 2d63 6f6e 6e65 6374 696f 6e73 2e75  ar-connections.u
+000001f0: 732d 7765 7374 2d32 2e61 6d61 7a6f 6e61  s-west-2.amazona
+00000200: 7773 2e63 6f6d 2f67 6974 2d68 7474 702f  ws.com/git-http/
+00000210: 3036 3631 3935 3131 3233 3835 2f75 732d  066195112385/us-
+00000220: 7765 7374 2d32 2f65 3635 3032 6138 302d  west-2/e6502a80-
+00000230: 6262 3465 2d34 6662 652d 3837 3263 2d35  bb4e-4fbe-872c-5
+00000240: 6434 3263 3139 3336 3939 642f 726f 626f  d42c193699d/robo
+00000250: 746f 2d61 692f 726f 626f 746f 2d68 6f73  to-ai/roboto-hos
+00000260: 7465 642d 6170 702f 7061 636b 6167 6573  ted-app/packages
+00000270: 2f72 6f62 6f74 6f5f 7364 6b2f 7372 632f  /roboto_sdk/src/
+00000280: 726f 626f 746f 5f73 646b 2f64 6f6d 6169  roboto_sdk/domai
+00000290: 6e2f 746f 6b65 6e73 2f64 656c 6567 6174  n/tokens/delegat
+000002a0: 652e 7079 7208 0000 0009 0000 0073 0200  e.pyr........s..
+000002b0: 0000 0e01 7a16 546f 6b65 6e44 656c 6567  ....z.TokenDeleg
+000002c0: 6174 652e 5f5f 696e 6974 5f5f 4eda 0775  ate.__init__N..u
+000002d0: 7365 725f 6964 da06 7265 7475 726e 6302  ser_id..returnc.
+000002e0: 0000 0000 0000 0000 0000 0002 0000 0002  ................
+000002f0: 0000 0043 0000 00f3 0800 0000 7400 6401  ...C........t.d.
+00000300: 8301 8201 2902 4eda 1367 6574 5f74 6f6b  ....).N..get_tok
+00000310: 656e 735f 666f 725f 7573 6572 a901 da13  ens_for_user....
+00000320: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
+00000330: 726f 7229 0272 0900 0000 720e 0000 0072  ror).r....r....r
+00000340: 0c00 0000 720c 0000 0072 0d00 0000 7211  ....r....r....r.
+00000350: 0000 000c 0000 00f3 0200 0000 0802 7a21  ..............z!
+00000360: 546f 6b65 6e44 656c 6567 6174 652e 6765  TokenDelegate.ge
+00000370: 745f 746f 6b65 6e73 5f66 6f72 5f75 7365  t_tokens_for_use
+00000380: 72da 0b65 7870 6972 795f 6461 7973 da04  r..expiry_days..
+00000390: 6e61 6d65 da0b 6465 7363 7269 7074 696f  name..descriptio
+000003a0: 6e63 0500 0000 0000 0000 0000 0000 0500  nc..............
+000003b0: 0000 0200 0000 4300 0000 7210 0000 0029  ......C...r....)
+000003c0: 024e da0c 6372 6561 7465 5f74 6f6b 656e  .N..create_token
+000003d0: 7212 0000 0029 0572 0900 0000 7215 0000  r....).r....r...
+000003e0: 0072 1600 0000 720e 0000 0072 1700 0000  .r....r....r....
+000003f0: 720c 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
+00000400: 1800 0000 1000 0000 7302 0000 0008 087a  ........s......z
+00000410: 1a54 6f6b 656e 4465 6c65 6761 7465 2e63  .TokenDelegate.c
+00000420: 7265 6174 655f 746f 6b65 6eda 0874 6f6b  reate_token..tok
+00000430: 656e 5f69 6463 0200 0000 0000 0000 0000  en_idc..........
+00000440: 0000 0200 0000 0200 0000 4300 0000 7210  ..........C...r.
+00000450: 0000 0029 024e da0c 6465 6c65 7465 5f74  ...).N..delete_t
+00000460: 6f6b 656e 7212 0000 00a9 0272 0900 0000  okenr......r....
+00000470: 7219 0000 0072 0c00 0000 720c 0000 0072  r....r....r....r
+00000480: 0d00 0000 721a 0000 001a 0000 0072 1400  ....r........r..
+00000490: 0000 7a1a 546f 6b65 6e44 656c 6567 6174  ..z.TokenDelegat
+000004a0: 652e 6465 6c65 7465 5f74 6f6b 656e 6302  e.delete_tokenc.
+000004b0: 0000 0000 0000 0000 0000 0002 0000 0002  ................
+000004c0: 0000 0043 0000 0072 1000 0000 2902 4eda  ...C...r....).N.
+000004d0: 1567 6574 5f74 6f6b 656e 5f62 795f 746f  .get_token_by_to
+000004e0: 6b65 6e5f 6964 7212 0000 0072 1b00 0000  ken_idr....r....
+000004f0: 720c 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
+00000500: 1c00 0000 1e00 0000 7214 0000 007a 2354  ........r....z#T
+00000510: 6f6b 656e 4465 6c65 6761 7465 2e67 6574  okenDelegate.get
+00000520: 5f74 6f6b 656e 5f62 795f 746f 6b65 6e5f  _token_by_token_
+00000530: 6964 7206 0000 0029 024e 4e29 10da 085f  idr....).NN)..._
+00000540: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+00000550: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+00000560: 5f72 0800 0000 da03 6162 63da 0e61 6273  _r......abc..abs
+00000570: 7472 6163 746d 6574 686f 6472 0200 0000  tractmethodr....
+00000580: da03 7374 72da 046c 6973 7472 0400 0000  ..str..listr....
+00000590: 7211 0000 00da 0369 6e74 7218 0000 0072  r......intr....r
+000005a0: 1a00 0000 721c 0000 00da 0d5f 5f63 6c61  ....r......__cla
+000005b0: 7373 6365 6c6c 5f5f 720c 0000 0072 0c00  sscell__r....r..
+000005c0: 0000 720a 0000 0072 0d00 0000 7205 0000  ..r....r....r...
+000005d0: 0008 0000 0073 2c00 0000 0800 0c01 0403  .....s,.........
+000005e0: 1e01 0403 0205 0201 04fb 0202 02fe 0203  ................
+000005f0: 02fd 0604 02fc 0605 02fb 0206 0cfa 0409  ................
+00000600: 1401 0403 1c01 7205 0000 0029 0772 2000  ......r....).r .
+00000610: 0000 da06 7479 7069 6e67 7202 0000 00da  ....typingr.....
+00000620: 0672 6563 6f72 6472 0400 0000 da03 4142  .recordr......AB
+00000630: 4372 0500 0000 720c 0000 0072 0c00 0000  Cr....r....r....
+00000640: 720c 0000 0072 0d00 0000 da08 3c6d 6f64  r....r......<mod
+00000650: 756c 653e 0100 0000 7308 0000 0008 010c  ule>....s.......
+00000660: 010c 0216 03                             .....
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/__pycache__/http_delegate.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/triggers/__pycache__/http_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 2038 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,169 +1,173 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 f607 0000  o.......1..d....
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 e808 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
-00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 6d04 5a04 0100 6402 6404 6c05  m.Z.m.Z...d.d.l.
-00000050: 6d06 5a06 0100 6405 6406 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
-00000060: 0100 6405 6407 6c09 6d0a 5a0a 0100 6405  ..d.d.l.m.Z...d.
-00000070: 6408 6c0b 6d0c 5a0c 0100 4700 6409 640a  d.l.m.Z...G.d.d.
-00000080: 8400 640a 6508 8303 5a0d 640b 5300 290c  ..d.e...Z.d.S.).
-00000090: e900 0000 0029 01da 084f 7074 696f 6e61  .....)...Optiona
-000000a0: 6ce9 0300 0000 2902 da14 5553 4552 5f4f  l.....)...USER_O
-000000b0: 5645 5252 4944 455f 4845 4144 4552 da0a  VERRIDE_HEADER..
-000000c0: 4874 7470 436c 6965 6e74 2901 da16 7079  HttpClient)...py
-000000d0: 6461 6e74 6963 5f6a 736f 6e61 626c 655f  dantic_jsonable_
-000000e0: 6469 6374 e901 0000 0029 01da 0d54 6f6b  dict.....)...Tok
-000000f0: 656e 4465 6c65 6761 7465 2901 da12 4372  enDelegate)...Cr
-00000100: 6561 7465 546f 6b65 6e52 6571 7565 7374  eateTokenRequest
-00000110: 2901 da0b 546f 6b65 6e52 6563 6f72 6463  )...TokenRecordc
-00000120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000130: 0a00 0000 0000 0000 7390 0000 0065 005a  ........s....e.Z
-00000140: 0164 005a 0255 0065 0365 0464 013c 0064  .d.Z.U.e.e.d.<.d
-00000150: 0265 0366 0287 0066 0164 0364 0484 0c5a  .e.f...f.d.d...Z
-00000160: 0564 0565 0665 0719 0064 0665 0865 0919  .d.e.e...d.e.e..
-00000170: 0066 0464 0764 0884 045a 0a64 0565 0665  .f.d.d...Z.d.e.e
-00000180: 0719 0064 0965 0b64 0a65 0764 0b65 0665  ...d.e.d.e.d.e.e
-00000190: 0719 0064 0665 0966 0a64 0c64 0d84 045a  ...d.e.f.d.d...Z
-000001a0: 0c64 0e65 0764 0664 0f66 0464 1064 1184  .d.e.d.d.f.d.d..
-000001b0: 045a 0d64 0e65 0764 0665 0966 0464 1264  .Z.d.e.d.e.f.d.d
-000001c0: 1384 045a 0e87 0004 005a 0f53 0029 14da  ...Z.....Z.S.)..
-000001d0: 1154 6f6b 656e 4874 7470 4465 6c65 6761  .TokenHttpDelega
-000001e0: 7465 da1f 5f54 6f6b 656e 4874 7470 4465  te.._TokenHttpDe
-000001f0: 6c65 6761 7465 5f5f 6874 7470 5f63 6c69  legate__http_cli
-00000200: 656e 74da 0b68 7474 705f 636c 6965 6e74  ent..http_client
-00000210: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00000220: 0002 0000 0003 0000 0073 1400 0000 7400  .........s....t.
-00000230: 8300 a001 a100 0100 7c01 7c00 5f02 6400  ........|.|._.d.
-00000240: 5300 2901 4e29 03da 0573 7570 6572 da08  S.).N)...super..
-00000250: 5f5f 696e 6974 5f5f 720c 0000 0029 02da  __init__r....)..
-00000260: 0473 656c 6672 0d00 0000 a901 da09 5f5f  .selfr........__
-00000270: 636c 6173 735f 5fa9 00fa f32f 636f 6465  class__..../code
-00000280: 6275 696c 642f 6f75 7470 7574 2f73 7263  build/output/src
-00000290: 3136 3839 3135 3533 3939 2f73 7263 2f63  1689155399/src/c
-000002a0: 6f64 6573 7461 722d 636f 6e6e 6563 7469  odestar-connecti
-000002b0: 6f6e 732e 7573 2d77 6573 742d 322e 616d  ons.us-west-2.am
-000002c0: 617a 6f6e 6177 732e 636f 6d2f 6769 742d  azonaws.com/git-
-000002d0: 6874 7470 2f30 3636 3139 3531 3132 3338  http/06619511238
-000002e0: 352f 7573 2d77 6573 742d 322f 6536 3530  5/us-west-2/e650
-000002f0: 3261 3830 2d62 6234 652d 3466 6265 2d38  2a80-bb4e-4fbe-8
-00000300: 3732 632d 3564 3432 6331 3933 3639 3964  72c-5d42c193699d
-00000310: 2f72 6f62 6f74 6f2d 6169 2f72 6f62 6f74  /roboto-ai/robot
-00000320: 6f2d 686f 7374 6564 2d61 7070 2f70 6163  o-hosted-app/pac
-00000330: 6b61 6765 732f 726f 626f 746f 5f73 646b  kages/roboto_sdk
-00000340: 2f73 7263 2f72 6f62 6f74 6f5f 7364 6b2f  /src/roboto_sdk/
-00000350: 646f 6d61 696e 2f74 6f6b 656e 732f 6874  domain/tokens/ht
-00000360: 7470 5f64 656c 6567 6174 652e 7079 720f  tp_delegate.pyr.
-00000370: 0000 0012 0000 0073 0400 0000 0a01 0a01  .......s........
-00000380: 7a1a 546f 6b65 6e48 7474 7044 656c 6567  z.TokenHttpDeleg
-00000390: 6174 652e 5f5f 696e 6974 5f5f da07 7573  ate.__init__..us
-000003a0: 6572 5f69 64da 0672 6574 7572 6e63 0200  er_id..returnc..
-000003b0: 0000 0000 0000 0000 0000 0600 0000 0400  ................
-000003c0: 0000 4300 0000 734c 0000 007c 006a 00a0  ..C...sL...|.j..
-000003d0: 0164 01a1 017d 0269 007d 037c 0164 0075  .d...}.i.}.|.d.u
-000003e0: 0172 107c 017c 0374 023c 007c 006a 006a  .r.|.|.t.<.|.j.j
-000003f0: 037c 027c 0364 028d 027d 047c 046a 0464  .|.|.d...}.|.j.d
-00000400: 0367 0164 048d 017d 0564 0564 0684 007c  .g.d...}.d.d...|
-00000410: 0544 0083 0153 0029 074e fa09 7631 2f74  .D...S.).N..v1/t
-00000420: 6f6b 656e 7329 02da 0375 726c da07 6865  okens)...url..he
-00000430: 6164 6572 73da 0464 6174 61a9 01da 096a  aders..data....j
-00000440: 736f 6e5f 7061 7468 6301 0000 0000 0000  son_pathc.......
-00000450: 0000 0000 0002 0000 0005 0000 0053 0000  .............S..
-00000460: 0073 1600 0000 6700 7c00 5d07 7d01 7400  .s....g.|.].}.t.
-00000470: a001 7c01 a101 9102 7102 5300 7213 0000  ..|.....q.S.r...
-00000480: 0029 0272 0a00 0000 da09 7061 7273 655f  .).r......parse_
-00000490: 6f62 6a29 02da 022e 30da 0672 6563 6f72  obj)....0..recor
-000004a0: 6472 1300 0000 7213 0000 0072 1400 0000  dr....r....r....
-000004b0: da0a 3c6c 6973 7463 6f6d 703e 1e00 0000  ..<listcomp>....
-000004c0: 7302 0000 0016 007a 3954 6f6b 656e 4874  s......z9TokenHt
-000004d0: 7470 4465 6c65 6761 7465 2e67 6574 5f74  tpDelegate.get_t
-000004e0: 6f6b 656e 735f 666f 725f 7573 6572 2e3c  okens_for_user.<
-000004f0: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
-00000500: 703e 2905 720c 0000 0072 1800 0000 7204  p>).r....r....r.
-00000510: 0000 00da 0367 6574 da09 6672 6f6d 5f6a  .....get..from_j
-00000520: 736f 6e29 0672 1000 0000 7215 0000 0072  son).r....r....r
-00000530: 1800 0000 7219 0000 00da 0872 6573 706f  ....r......respo
-00000540: 6e73 65da 0c75 6e6d 6172 7368 616c 6c65  nse..unmarshalle
-00000550: 6472 1300 0000 7213 0000 0072 1400 0000  dr....r....r....
-00000560: da13 6765 745f 746f 6b65 6e73 5f66 6f72  ..get_tokens_for
-00000570: 5f75 7365 7216 0000 0073 0e00 0000 0c01  _user....s......
-00000580: 0401 0801 0801 1002 0e01 0e01 7a25 546f  ............z%To
-00000590: 6b65 6e48 7474 7044 656c 6567 6174 652e  kenHttpDelegate.
-000005a0: 6765 745f 746f 6b65 6e73 5f66 6f72 5f75  get_tokens_for_u
-000005b0: 7365 72da 0b65 7870 6972 795f 6461 7973  ser..expiry_days
-000005c0: da04 6e61 6d65 da0b 6465 7363 7269 7074  ..name..descript
-000005d0: 696f 6e63 0500 0000 0000 0000 0000 0000  ionc............
-000005e0: 0900 0000 0500 0000 4300 0000 735c 0000  ........C...s\..
-000005f0: 007c 006a 00a0 0164 01a1 017d 0564 0264  .|.j...d...}.d.d
-00000600: 0369 017d 067c 0164 0075 0172 127c 017c  .i.}.|.d.u.r.|.|
-00000610: 0674 023c 0074 037c 027c 037c 0464 048d  .t.<.t.|.|.|.d..
-00000620: 037d 077c 006a 006a 047c 057c 0674 057c  .}.|.j.j.|.|.t.|
-00000630: 0783 0164 058d 037d 0874 06a0 077c 086a  ...d...}.t...|.j
-00000640: 0864 0667 0164 078d 01a1 0153 0029 084e  .d.g.d.....S.).N
-00000650: 7217 0000 007a 0c43 6f6e 7465 6e74 2d54  r....z.Content-T
-00000660: 7970 657a 1061 7070 6c69 6361 7469 6f6e  ypez.application
-00000670: 2f6a 736f 6e29 0372 2600 0000 7227 0000  /json).r&...r'..
-00000680: 0072 2800 0000 2903 7218 0000 0072 1900  .r(...).r....r..
-00000690: 0000 721a 0000 0072 1a00 0000 721b 0000  ..r....r....r...
-000006a0: 0029 0972 0c00 0000 7218 0000 0072 0400  .).r....r....r..
-000006b0: 0000 7209 0000 00da 0470 6f73 7472 0600  ..r......postr..
-000006c0: 0000 720a 0000 0072 1d00 0000 7222 0000  ..r....r....r"..
-000006d0: 0029 0972 1000 0000 7215 0000 0072 2600  .).r....r....r&.
-000006e0: 0000 7227 0000 0072 2800 0000 7218 0000  ..r'...r(...r...
-000006f0: 0072 1900 0000 721a 0000 0072 2300 0000  .r....r....r#...
-00000700: 7213 0000 0072 1300 0000 7214 0000 00da  r....r....r.....
-00000710: 0c63 7265 6174 655f 746f 6b65 6e20 0000  .create_token ..
-00000720: 0073 1600 0000 0c07 0801 0801 0801 0202  .s..............
-00000730: 0601 06ff 0604 0a01 06ff 1403 7a1e 546f  ............z.To
-00000740: 6b65 6e48 7474 7044 656c 6567 6174 652e  kenHttpDelegate.
-00000750: 6372 6561 7465 5f74 6f6b 656e da08 746f  create_token..to
-00000760: 6b65 6e5f 6964 4e63 0200 0000 0000 0000  ken_idNc........
-00000770: 0000 0000 0300 0000 0400 0000 4300 0000  ............C...
-00000780: 7324 0000 007c 006a 00a0 0164 017c 019b  s$...|.j...d.|..
-00000790: 009d 02a1 017d 027c 006a 006a 027c 0264  .....}.|.j.j.|.d
-000007a0: 028d 0101 0064 0053 0029 034e fa0d 7631  .....d.S.).N..v1
-000007b0: 2f74 6f6b 656e 732f 6964 2fa9 0172 1800  /tokens/id/..r..
-000007c0: 0000 2903 720c 0000 0072 1800 0000 da06  ..).r....r......
-000007d0: 6465 6c65 7465 2903 7210 0000 0072 2b00  delete).r....r+.
-000007e0: 0000 7218 0000 0072 1300 0000 7213 0000  ..r....r....r...
-000007f0: 0072 1400 0000 da0c 6465 6c65 7465 5f74  .r......delete_t
-00000800: 6f6b 656e 3500 0000 7304 0000 0012 0112  oken5...s.......
-00000810: 017a 1e54 6f6b 656e 4874 7470 4465 6c65  .z.TokenHttpDele
-00000820: 6761 7465 2e64 656c 6574 655f 746f 6b65  gate.delete_toke
-00000830: 6e63 0200 0000 0000 0000 0000 0000 0400  nc..............
-00000840: 0000 0500 0000 4300 0000 7334 0000 007c  ......C...s4...|
-00000850: 006a 00a0 0164 017c 019b 009d 02a1 017d  .j...d.|.......}
-00000860: 027c 006a 006a 027c 0264 028d 017d 0374  .|.j.j.|.d...}.t
-00000870: 03a0 047c 036a 0564 0367 0164 048d 01a1  ...|.j.d.g.d....
-00000880: 0153 0029 054e 722c 0000 0072 2d00 0000  .S.).Nr,...r-...
-00000890: 721a 0000 0072 1b00 0000 2906 720c 0000  r....r....).r...
-000008a0: 0072 1800 0000 7221 0000 0072 0a00 0000  .r....r!...r....
-000008b0: 721d 0000 0072 2200 0000 2904 7210 0000  r....r"...).r...
-000008c0: 0072 2b00 0000 7218 0000 0072 2300 0000  .r+...r....r#...
-000008d0: 7213 0000 0072 1300 0000 7214 0000 00da  r....r....r.....
-000008e0: 1567 6574 5f74 6f6b 656e 5f62 795f 746f  .get_token_by_to
-000008f0: 6b65 6e5f 6964 3900 0000 7306 0000 0012  ken_id9...s.....
-00000900: 010e 0114 017a 2754 6f6b 656e 4874 7470  .....z'TokenHttp
-00000910: 4465 6c65 6761 7465 2e67 6574 5f74 6f6b  Delegate.get_tok
-00000920: 656e 5f62 795f 746f 6b65 6e5f 6964 2910  en_by_token_id).
-00000930: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00000940: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00000950: 6d65 5f5f 7205 0000 00da 0f5f 5f61 6e6e  me__r......__ann
-00000960: 6f74 6174 696f 6e73 5f5f 720f 0000 0072  otations__r....r
-00000970: 0200 0000 da03 7374 72da 046c 6973 7472  ......str..listr
-00000980: 0a00 0000 7225 0000 00da 0369 6e74 722a  ....r%.....intr*
-00000990: 0000 0072 2f00 0000 7230 0000 00da 0d5f  ...r/...r0....._
-000009a0: 5f63 6c61 7373 6365 6c6c 5f5f 7213 0000  _classcell__r...
-000009b0: 0072 1300 0000 7211 0000 0072 1400 0000  .r....r....r....
-000009c0: 720b 0000 000f 0000 0073 2200 0000 0a00  r........s".....
-000009d0: 0801 1202 1a04 020a 0602 02fe 0203 02fd  ................
-000009e0: 0204 02fc 0605 02fb 0206 0afa 1215 1a04  ................
-000009f0: 720b 0000 004e 290e da06 7479 7069 6e67  r....N)...typing
-00000a00: 7202 0000 00da 0468 7474 7072 0400 0000  r......httpr....
-00000a10: 7205 0000 00da 0573 6572 6465 7206 0000  r......serder...
-00000a20: 00da 0864 656c 6567 6174 6572 0800 0000  ...delegater....
-00000a30: da0e 6874 7470 5f72 6573 6f75 7263 6573  ..http_resources
-00000a40: 7209 0000 0072 1f00 0000 720a 0000 0072  r....r....r....r
-00000a50: 0b00 0000 7213 0000 0072 1300 0000 7213  ....r....r....r.
-00000a60: 0000 0072 1400 0000 da08 3c6d 6f64 756c  ...r......<modul
-00000a70: 653e 0100 0000 730e 0000 000c 0210 020c  e>....s.........
-00000a80: 040c 010c 010c 0114 03                   .........
+00000020: 0004 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
+00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6402  d.l.m.Z.m.Z...d.
+00000040: 6403 6c03 6d04 5a04 6d05 5a05 0100 6402  d.l.m.Z.m.Z...d.
+00000050: 6404 6c06 6d07 5a07 0100 6402 6405 6c08  d.l.m.Z...d.d.l.
+00000060: 6d09 5a09 0100 6406 6407 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
+00000070: 0100 6406 6408 6c0c 6d0d 5a0d 0100 6406  ..d.d.l.m.Z...d.
+00000080: 6409 6c0e 6d0f 5a0f 0100 4700 640a 640b  d.l.m.Z...G.d.d.
+00000090: 8400 640b 650d 8303 5a10 640c 5300 290d  ..d.e...Z.d.S.).
+000000a0: e900 0000 0029 02da 0341 6e79 da08 4f70  .....)...Any..Op
+000000b0: 7469 6f6e 616c e903 0000 0029 02da 134f  tional.....)...O
+000000c0: 5247 5f4f 5645 5252 4944 455f 4845 4144  RG_OVERRIDE_HEAD
+000000d0: 4552 da0a 4874 7470 436c 6965 6e74 2901  ER..HttpClient).
+000000e0: da0d 5061 6769 6e61 7465 644c 6973 7429  ..PaginatedList)
+000000f0: 01da 1670 7964 616e 7469 635f 6a73 6f6e  ...pydantic_json
+00000100: 6162 6c65 5f64 6963 74e9 0100 0000 2901  able_dict.....).
+00000110: da14 4372 6561 7465 5472 6967 6765 7252  ..CreateTriggerR
+00000120: 6571 7565 7374 2901 da0f 5472 6967 6765  equest)...Trigge
+00000130: 7244 656c 6567 6174 6529 01da 0d54 7269  rDelegate)...Tri
+00000140: 6767 6572 5265 636f 7264 6300 0000 0000  ggerRecordc.....
+00000150: 0000 0000 0000 0000 0000 000a 0000 0000  ................
+00000160: 0000 0073 a200 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+00000170: 5500 6503 6504 6401 3c00 6402 6503 6602  U.e.e.d.<.d.e.f.
+00000180: 8700 6601 6403 6404 840c 5a05 6405 6506  ..f.d.d...Z.d.e.
+00000190: 6406 6507 6506 1900 6407 6506 6408 6508  d.e.e...d.e.d.e.
+000001a0: 6608 6409 640a 8404 5a09 6405 6506 6406  f.d.d...Z.d.e.d.
+000001b0: 6507 6506 1900 6408 6508 6606 640b 640c  e.e...d.e.f.d.d.
+000001c0: 8404 5a0a 090d 6412 640e 6507 650b 6506  ..Z...d.d.e.e.e.
+000001d0: 650c 6602 1900 1900 6406 6507 6506 1900  e.f.....d.e.e...
+000001e0: 640f 6507 650b 6506 6506 6602 1900 1900  d.e.e.e.e.f.....
+000001f0: 6408 650d 6508 1900 6608 6410 6411 8405  d.e.e...f.d.d...
+00000200: 5a0e 8700 0400 5a0f 5300 2913 da13 5472  Z.....Z.S.)...Tr
+00000210: 6967 6765 7248 7474 7044 656c 6567 6174  iggerHttpDelegat
+00000220: 65da 215f 5472 6967 6765 7248 7474 7044  e.!_TriggerHttpD
+00000230: 656c 6567 6174 655f 5f68 7474 705f 636c  elegate__http_cl
+00000240: 6965 6e74 da0b 6874 7470 5f63 6c69 656e  ient..http_clien
+00000250: 7463 0200 0000 0000 0000 0000 0000 0200  tc..............
+00000260: 0000 0200 0000 0300 0000 7314 0000 0074  ..........s....t
+00000270: 0083 00a0 01a1 0001 007c 017c 005f 0264  .........|.|._.d
+00000280: 0053 00a9 014e 2903 da05 7375 7065 72da  .S...N)...super.
+00000290: 085f 5f69 6e69 745f 5f72 0e00 0000 2902  .__init__r....).
+000002a0: da04 7365 6c66 720f 0000 00a9 01da 095f  ..selfr........_
+000002b0: 5f63 6c61 7373 5f5f a900 faf5 2f63 6f64  _class__..../cod
+000002c0: 6562 7569 6c64 2f6f 7574 7075 742f 7372  ebuild/output/sr
+000002d0: 6333 3537 3831 3132 3139 312f 7372 632f  c3578112191/src/
+000002e0: 636f 6465 7374 6172 2d63 6f6e 6e65 6374  codestar-connect
+000002f0: 696f 6e73 2e75 732d 7765 7374 2d32 2e61  ions.us-west-2.a
+00000300: 6d61 7a6f 6e61 7773 2e63 6f6d 2f67 6974  mazonaws.com/git
+00000310: 2d68 7474 702f 3036 3631 3935 3131 3233  -http/0661951123
+00000320: 3835 2f75 732d 7765 7374 2d32 2f65 3635  85/us-west-2/e65
+00000330: 3032 6138 302d 6262 3465 2d34 6662 652d  02a80-bb4e-4fbe-
+00000340: 3837 3263 2d35 6434 3263 3139 3336 3939  872c-5d42c193699
+00000350: 642f 726f 626f 746f 2d61 692f 726f 626f  d/roboto-ai/robo
+00000360: 746f 2d68 6f73 7465 642d 6170 702f 7061  to-hosted-app/pa
+00000370: 636b 6167 6573 2f72 6f62 6f74 6f5f 7364  ckages/roboto_sd
+00000380: 6b2f 7372 632f 726f 626f 746f 5f73 646b  k/src/roboto_sdk
+00000390: 2f64 6f6d 6169 6e2f 7472 6967 6765 7273  /domain/triggers
+000003a0: 2f68 7474 705f 6465 6c65 6761 7465 2e70  /http_delegate.p
+000003b0: 7972 1200 0000 1300 0000 7304 0000 000a  yr........s.....
+000003c0: 010a 017a 1c54 7269 6767 6572 4874 7470  ...z.TriggerHttp
+000003d0: 4465 6c65 6761 7465 2e5f 5f69 6e69 745f  Delegate.__init_
+000003e0: 5fda 046e 616d 65da 066f 7267 5f69 64da  _..name..org_id.
+000003f0: 0b61 6374 696f 6e5f 6e61 6d65 da06 7265  .action_name..re
+00000400: 7475 726e 6304 0000 0000 0000 0000 0000  turnc...........
+00000410: 0008 0000 0005 0000 0043 0000 0073 5a00  .........C...sZ.
+00000420: 0000 7c00 6a00 a001 6401 a101 7d04 6402  ..|.j...d...}.d.
+00000430: 6403 6901 7d05 7c02 6400 7501 7212 7c02  d.i.}.|.d.u.r.|.
+00000440: 7c05 7402 3c00 7403 7c01 7c03 6404 8d02  |.t.<.t.|.|.d...
+00000450: 7d06 7c00 6a00 6a04 7c04 7405 7c06 8301  }.|.j.j.|.t.|...
+00000460: 7c05 6405 8d03 7d07 7406 a007 7c07 6a08  |.d...}.t...|.j.
+00000470: 6406 6701 6407 8d01 a101 5300 2908 4efa  d.g.d.....S.).N.
+00000480: 0b76 312f 7472 6967 6765 7273 7a0c 436f  .v1/triggersz.Co
+00000490: 6e74 656e 742d 5479 7065 7a10 6170 706c  ntent-Typez.appl
+000004a0: 6963 6174 696f 6e2f 6a73 6f6e 2902 7218  ication/json).r.
+000004b0: 0000 0072 1a00 0000 2902 da04 6461 7461  ...r....)...data
+000004c0: da07 6865 6164 6572 7372 1d00 0000 a901  ..headersr......
+000004d0: da09 6a73 6f6e 5f70 6174 6829 0972 0e00  ..json_path).r..
+000004e0: 0000 da03 7572 6c72 0500 0000 720a 0000  ....urlr....r...
+000004f0: 00da 0470 6f73 7472 0800 0000 720c 0000  ...postr....r...
+00000500: 00da 0970 6172 7365 5f6f 626a da09 6672  ...parse_obj..fr
+00000510: 6f6d 5f6a 736f 6e29 0872 1300 0000 7218  om_json).r....r.
+00000520: 0000 0072 1900 0000 721a 0000 0072 2100  ...r....r....r!.
+00000530: 0000 721e 0000 00da 0c72 6571 7565 7374  ..r......request
+00000540: 5f62 6f64 79da 0872 6573 706f 6e73 6572  _body..responser
+00000550: 1600 0000 7216 0000 0072 1700 0000 da0e  ....r....r......
+00000560: 6372 6561 7465 5f74 7269 6767 6572 1700  create_trigger..
+00000570: 0000 7312 0000 000c 0308 0108 0108 010c  ..s.............
+00000580: 0206 020a 0106 ff14 037a 2254 7269 6767  .........z"Trigg
+00000590: 6572 4874 7470 4465 6c65 6761 7465 2e63  erHttpDelegate.c
+000005a0: 7265 6174 655f 7472 6967 6765 7263 0300  reate_triggerc..
+000005b0: 0000 0000 0000 0000 0000 0600 0000 0500  ................
+000005c0: 0000 4300 0000 734a 0000 007c 006a 00a0  ..C...sJ...|.j..
+000005d0: 0164 017c 019b 009d 02a1 017d 0369 007d  .d.|.......}.i.}
+000005e0: 047c 0264 0075 0172 137c 027c 0474 023c  .|.d.u.r.|.|.t.<
+000005f0: 007c 006a 006a 037c 037c 0464 028d 027d  .|.j.j.|.|.d...}
+00000600: 0574 04a0 057c 056a 0664 0367 0164 048d  .t...|.j.d.g.d..
+00000610: 01a1 0153 0029 054e 7a0c 7631 2f74 7269  ...S.).Nz.v1/tri
+00000620: 6767 6572 732f a901 721e 0000 0072 1d00  ggers/..r....r..
+00000630: 0000 721f 0000 0029 0772 0e00 0000 7221  ..r....).r....r!
+00000640: 0000 0072 0500 0000 da03 6765 7472 0c00  ...r......getr..
+00000650: 0000 7223 0000 0072 2400 0000 2906 7213  ..r#...r$...).r.
+00000660: 0000 0072 1800 0000 7219 0000 0072 2100  ...r....r....r!.
+00000670: 0000 721e 0000 0072 2600 0000 7216 0000  ..r....r&...r...
+00000680: 0072 1600 0000 7217 0000 00da 1a67 6574  .r....r......get
+00000690: 5f74 7269 6767 6572 5f62 795f 7072 696d  _trigger_by_prim
+000006a0: 6172 795f 6b65 7926 0000 0073 0c00 0000  ary_key&...s....
+000006b0: 1203 0401 0801 0801 1001 1401 7a2e 5472  ............z.Tr
+000006c0: 6967 6765 7248 7474 7044 656c 6567 6174  iggerHttpDelegat
+000006d0: 652e 6765 745f 7472 6967 6765 725f 6279  e.get_trigger_by
+000006e0: 5f70 7269 6d61 7279 5f6b 6579 4eda 0766  _primary_keyN..f
+000006f0: 696c 7465 7273 da0a 7061 6765 5f74 6f6b  ilters..page_tok
+00000700: 656e 6304 0000 0000 0000 0000 0000 0008  enc.............
+00000710: 0000 0006 0000 0043 0000 0073 6000 0000  .......C...s`...
+00000720: 7c00 6a00 a001 6401 a101 7d04 6900 7d05  |.j...d...}.i.}.
+00000730: 7c02 6400 7501 7210 7402 7c02 6901 7d05  |.d.u.r.t.|.i.}.
+00000740: 7c00 6a00 6a03 7c04 7c05 6402 8d02 7d06  |.j.j.|.|.d...}.
+00000750: 7c06 6a04 6403 6701 6404 8d01 7d07 7405  |.j.d.g.d...}.t.
+00000760: 6405 6406 8400 7c07 6407 1900 4400 8301  d.d...|.d...D...
+00000770: 7c07 a003 6408 6400 a102 6409 8d02 5300  |...d.d...d...S.
+00000780: 290a 4e72 1c00 0000 7228 0000 0072 1d00  ).Nr....r(...r..
+00000790: 0000 721f 0000 0063 0100 0000 0000 0000  ..r....c........
+000007a0: 0000 0000 0200 0000 0500 0000 5300 0000  ............S...
+000007b0: 7316 0000 0067 007c 005d 077d 0174 00a0  s....g.|.].}.t..
+000007c0: 017c 01a1 0191 0271 0253 0072 1600 0000  .|.....q.S.r....
+000007d0: 2902 720c 0000 0072 2300 0000 2902 da02  ).r....r#...)...
+000007e0: 2e30 da07 7472 6967 6765 7272 1600 0000  .0..triggerr....
+000007f0: 7216 0000 0072 1700 0000 da0a 3c6c 6973  r....r......<lis
+00000800: 7463 6f6d 703e 3f00 0000 7306 0000 0006  tcomp>?...s.....
+00000810: 000a 0106 ff7a 3654 7269 6767 6572 4874  .....z6TriggerHt
+00000820: 7470 4465 6c65 6761 7465 2e71 7565 7279  tpDelegate.query
+00000830: 5f74 7269 6767 6572 732e 3c6c 6f63 616c  _triggers.<local
+00000840: 733e 2e3c 6c69 7374 636f 6d70 3eda 0569  s>.<listcomp>..i
+00000850: 7465 6d73 da0a 6e65 7874 5f74 6f6b 656e  tems..next_token
+00000860: 2902 7230 0000 0072 3100 0000 2906 720e  ).r0...r1...).r.
+00000870: 0000 0072 2100 0000 7205 0000 0072 2900  ...r!...r....r).
+00000880: 0000 7224 0000 0072 0700 0000 2908 7213  ..r$...r....).r.
+00000890: 0000 0072 2b00 0000 7219 0000 0072 2c00  ...r+...r....r,.
+000008a0: 0000 7221 0000 0072 1e00 0000 7226 0000  ..r!...r....r&..
+000008b0: 00da 0c75 6e6d 6172 7368 616c 6c65 6472  ...unmarshalledr
+000008c0: 1600 0000 7216 0000 0072 1700 0000 da0e  ....r....r......
+000008d0: 7175 6572 795f 7472 6967 6765 7273 3000  query_triggers0.
+000008e0: 0000 7318 0000 000c 0604 0208 0108 0110  ..s.............
+000008f0: 020e 0102 0106 0106 0104 ff0a 0306 fc7a  ...............z
+00000900: 2254 7269 6767 6572 4874 7470 4465 6c65  "TriggerHttpDele
+00000910: 6761 7465 2e71 7565 7279 5f74 7269 6767  gate.query_trigg
+00000920: 6572 7372 1000 0000 2910 da08 5f5f 6e61  ersr....)...__na
+00000930: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000940: da0c 5f5f 7175 616c 6e61 6d65 5f5f 7206  ..__qualname__r.
+00000950: 0000 00da 0f5f 5f61 6e6e 6f74 6174 696f  .....__annotatio
+00000960: 6e73 5f5f 7212 0000 00da 0373 7472 7203  ns__r......strr.
+00000970: 0000 0072 0c00 0000 7227 0000 0072 2a00  ...r....r'...r*.
+00000980: 0000 da04 6469 6374 7202 0000 0072 0700  ....dictr....r..
+00000990: 0000 7233 0000 00da 0d5f 5f63 6c61 7373  ..r3.....__class
+000009a0: 6365 6c6c 5f5f 7216 0000 0072 1600 0000  cell__r....r....
+000009b0: 7214 0000 0072 1700 0000 720d 0000 0010  r....r....r.....
+000009c0: 0000 0073 3a00 0000 0a00 0801 1202 0204  ...s:...........
+000009d0: 0201 02ff 0601 02ff 0201 02ff 0202 0afe  ................
+000009e0: 020f 0201 02ff 0601 02ff 0202 0afe 020e  ................
+000009f0: 04fc 0e02 02fe 0603 02fd 0e04 02fc 0605  ................
+00000a00: 12fb 720d 0000 004e 2911 da06 7479 7069  ..r....N)...typi
+00000a10: 6e67 7202 0000 0072 0300 0000 da04 6874  ngr....r......ht
+00000a20: 7470 7205 0000 0072 0600 0000 da0a 7061  tpr....r......pa
+00000a30: 6769 6e61 7469 6f6e 7207 0000 00da 0573  ginationr......s
+00000a40: 6572 6465 7208 0000 00da 0e68 7474 705f  erder......http_
+00000a50: 7265 736f 7572 6365 7372 0a00 0000 da10  resourcesr......
+00000a60: 7472 6967 6765 725f 6465 6c65 6761 7465  trigger_delegate
+00000a70: 720b 0000 00da 0e74 7269 6767 6572 5f72  r......trigger_r
+00000a80: 6563 6f72 6472 0c00 0000 720d 0000 0072  ecordr....r....r
+00000a90: 1600 0000 7216 0000 0072 1600 0000 7217  ....r....r....r.
+00000aa0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000ab0: 0073 1000 0000 1002 1002 0c04 0c01 0c01  .s..............
+00000ac0: 0c01 0c01 1403                           ......
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/__pycache__/http_resources.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/tokens/__pycache__/http_resources.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 216 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 d800 0000  o.......1..d....
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 d800 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2a00 0000 6400  .....@...s*...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 4700 6403 6404 8400 6404 6502 6a03  Z.G.d.d...d.e.j.
 00000050: 8303 5a04 6402 5300 2905 e900 0000 0029  ..Z.d.S.)......)
 00000060: 01da 084f 7074 696f 6e61 6c4e 6300 0000  ...OptionalNc...
 00000070: 0000 0000 0000 0000 0000 0000 0003 0000  ................
@@ -15,16 +15,16 @@
 000000e0: 654e da0b 6465 7363 7269 7074 696f 6e29  eN..description)
 000000f0: 08da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
 00000100: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
 00000110: 616d 655f 5fda 0369 6e74 da0f 5f5f 616e  ame__..int..__an
 00000120: 6e6f 7461 7469 6f6e 735f 5fda 0373 7472  notations__..str
 00000130: 7206 0000 0072 0200 0000 a900 720d 0000  r....r......r...
 00000140: 0072 0d00 0000 faf4 2f63 6f64 6562 7569  .r....../codebui
-00000150: 6c64 2f6f 7574 7075 742f 7372 6331 3638  ld/output/src168
-00000160: 3931 3535 3339 392f 7372 632f 636f 6465  9155399/src/code
+00000150: 6c64 2f6f 7574 7075 742f 7372 6333 3537  ld/output/src357
+00000160: 3831 3132 3139 312f 7372 632f 636f 6465  8112191/src/code
 00000170: 7374 6172 2d63 6f6e 6e65 6374 696f 6e73  star-connections
 00000180: 2e75 732d 7765 7374 2d32 2e61 6d61 7a6f  .us-west-2.amazo
 00000190: 6e61 7773 2e63 6f6d 2f67 6974 2d68 7474  naws.com/git-htt
 000001a0: 702f 3036 3631 3935 3131 3233 3835 2f75  p/066195112385/u
 000001b0: 732d 7765 7374 2d32 2f65 3635 3032 6138  s-west-2/e6502a8
 000001c0: 302d 6262 3465 2d34 6662 652d 3837 3263  0-bb4e-4fbe-872c
 000001d0: 2d35 6434 3263 3139 3336 3939 642f 726f  -5d42c193699d/ro
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/__pycache__/record.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/tokens/__pycache__/record.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 455 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 c701 0000  o.......1..d....
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 c701 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 4700 6403 6404  ..d.d.l.Z.G.d.d.
 00000050: 8400 6404 6503 6a04 8303 5a05 4700 6405  ..d.e.j...Z.G.d.
 00000060: 6406 8400 6406 6503 6a04 8303 5a06 6401  d...d.e.j...Z.d.
 00000070: 5300 2907 e900 0000 004e 2901 da08 4f70  S.)......N)...Op
@@ -20,16 +20,16 @@
 00000130: 2909 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
 00000140: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
 00000150: 6e61 6d65 5f5f da03 7374 72da 0f5f 5f61  name__..str..__a
 00000160: 6e6e 6f74 6174 696f 6e73 5f5f 7206 0000  nnotations__r...
 00000170: 0072 0200 0000 da08 6461 7465 7469 6d65  .r......datetime
 00000180: 7208 0000 00a9 0072 0f00 0000 720f 0000  r......r....r...
 00000190: 00fa ec2f 636f 6465 6275 696c 642f 6f75  .../codebuild/ou
-000001a0: 7470 7574 2f73 7263 3136 3839 3135 3533  tput/src16891553
-000001b0: 3939 2f73 7263 2f63 6f64 6573 7461 722d  99/src/codestar-
+000001a0: 7470 7574 2f73 7263 3335 3738 3131 3231  tput/src35781121
+000001b0: 3931 2f73 7263 2f63 6f64 6573 7461 722d  91/src/codestar-
 000001c0: 636f 6e6e 6563 7469 6f6e 732e 7573 2d77  connections.us-w
 000001d0: 6573 742d 322e 616d 617a 6f6e 6177 732e  est-2.amazonaws.
 000001e0: 636f 6d2f 6769 742d 6874 7470 2f30 3636  com/git-http/066
 000001f0: 3139 3531 3132 3338 352f 7573 2d77 6573  195112385/us-wes
 00000200: 742d 322f 6536 3530 3261 3830 2d62 6234  t-2/e6502a80-bb4
 00000210: 652d 3466 6265 2d38 3732 632d 3564 3432  e-4fbe-872c-5d42
 00000220: 6331 3933 3639 3964 2f72 6f62 6f74 6f2d  c193699d/roboto-
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/__pycache__/token.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/tokens/__pycache__/token.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 1826 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,158 +1,173 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 2207 0000  o.......1..d"...
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 ff07 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6402  d.l.m.Z.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6404 6405 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6404 6406 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 4700 6407 6408 8400 6408 8302 5a09  ..G.d.d...d...Z.
 00000070: 6409 5300 290a e900 0000 0029 02da 0341  d.S.)......)...A
 00000080: 6e79 da08 4f70 7469 6f6e 616c e903 0000  ny..Optional....
 00000090: 0029 01da 1670 7964 616e 7469 635f 6a73  .)...pydantic_js
 000000a0: 6f6e 6162 6c65 5f64 6963 74e9 0100 0000  onable_dict.....
 000000b0: 2901 da0d 546f 6b65 6e44 656c 6567 6174  )...TokenDelegat
 000000c0: 6529 01da 0b54 6f6b 656e 5265 636f 7264  e)...TokenRecord
 000000d0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-000000e0: 000b 0000 0040 0000 0073 e000 0000 6500  .....@...s....e.
+000000e0: 000d 0000 0040 0000 0073 0601 0000 6500  .....@...s....e.
 000000f0: 5a01 6400 5a02 5500 6503 6504 6401 3c00  Z.d.Z.U.e.e.d.<.
 00000100: 6505 6504 6402 3c00 6506 6403 6507 6404  e.e.d.<.e.d.e.d.
 00000110: 6505 6405 6400 6606 6406 6407 8404 8301  e.d.d.f.d.d.....
-00000120: 5a08 6506 6408 6509 6507 1900 6404 6505  Z.e.d.e.e...d.e.
-00000130: 6405 650a 6400 1900 6606 6409 640a 8404  d.e.d...f.d.d...
-00000140: 8301 5a0b 6506 6408 6509 6507 1900 640b  ..Z.e.d.e.e...d.
-00000150: 650c 640c 6507 640d 6509 6507 1900 6404  e.d.e.d.e.e...d.
-00000160: 6505 660a 640e 640f 8404 8301 5a0d 6410  e.f.d.d.....Z.d.
-00000170: 6411 8400 5a0e 6412 6503 6404 6505 6604  d...Z.d.e.d.e.f.
-00000180: 6413 6414 8404 5a0f 6405 6510 6507 6511  d.d...Z.d.e.e.e.
-00000190: 6602 1900 6602 6415 6416 8404 5a12 6513  f...f.d.d...Z.e.
-000001a0: 6405 6509 6507 1900 6602 6417 6418 8404  d.e.e...f.d.d...
-000001b0: 8301 5a14 6513 6405 6509 6507 1900 6602  ..Z.e.d.e.e...f.
-000001c0: 6419 641a 8404 8301 5a15 641b 5300 291c  d.d.....Z.d.S.).
-000001d0: da05 546f 6b65 6eda 0e5f 546f 6b65 6e5f  ..Token.._Token_
-000001e0: 5f72 6563 6f72 64da 165f 546f 6b65 6e5f  _record.._Token_
-000001f0: 5f74 6f6b 656e 5f64 656c 6567 6174 65da  _token_delegate.
-00000200: 0874 6f6b 656e 5f69 64da 0e74 6f6b 656e  .token_id..token
-00000210: 5f64 656c 6567 6174 65da 0672 6574 7572  _delegate..retur
-00000220: 6e63 0300 0000 0000 0000 0000 0000 0400  nc..............
-00000230: 0000 0400 0000 4300 0000 7318 0000 007c  ......C...s....|
-00000240: 026a 007c 0164 018d 017d 037c 007c 037c  .j.|.d...}.|.|.|
-00000250: 0264 028d 0253 0029 034e a901 720c 0000  .d...S.).N..r...
-00000260: 00a9 02da 0672 6563 6f72 6472 0d00 0000  .....recordr....
-00000270: 2901 da15 6765 745f 746f 6b65 6e5f 6279  )...get_token_by
-00000280: 5f74 6f6b 656e 5f69 6429 04da 0363 6c73  _token_id)...cls
-00000290: 720c 0000 0072 0d00 0000 7211 0000 00a9  r....r....r.....
-000002a0: 0072 1400 0000 faeb 2f63 6f64 6562 7569  .r....../codebui
-000002b0: 6c64 2f6f 7574 7075 742f 7372 6331 3638  ld/output/src168
-000002c0: 3931 3535 3339 392f 7372 632f 636f 6465  9155399/src/code
-000002d0: 7374 6172 2d63 6f6e 6e65 6374 696f 6e73  star-connections
-000002e0: 2e75 732d 7765 7374 2d32 2e61 6d61 7a6f  .us-west-2.amazo
-000002f0: 6e61 7773 2e63 6f6d 2f67 6974 2d68 7474  naws.com/git-htt
-00000300: 702f 3036 3631 3935 3131 3233 3835 2f75  p/066195112385/u
-00000310: 732d 7765 7374 2d32 2f65 3635 3032 6138  s-west-2/e6502a8
-00000320: 302d 6262 3465 2d34 6662 652d 3837 3263  0-bb4e-4fbe-872c
-00000330: 2d35 6434 3263 3139 3336 3939 642f 726f  -5d42c193699d/ro
-00000340: 626f 746f 2d61 692f 726f 626f 746f 2d68  boto-ai/roboto-h
-00000350: 6f73 7465 642d 6170 702f 7061 636b 6167  osted-app/packag
-00000360: 6573 2f72 6f62 6f74 6f5f 7364 6b2f 7372  es/roboto_sdk/sr
-00000370: 632f 726f 626f 746f 5f73 646b 2f64 6f6d  c/roboto_sdk/dom
-00000380: 6169 6e2f 746f 6b65 6e73 2f74 6f6b 656e  ain/tokens/token
-00000390: 2e70 79da 0766 726f 6d5f 6964 0e00 0000  .py..from_id....
-000003a0: 7304 0000 000c 020c 017a 0d54 6f6b 656e  s........z.Token
-000003b0: 2e66 726f 6d5f 6964 da07 7573 6572 5f69  .from_id..user_i
-000003c0: 6463 0300 0000 0000 0000 0000 0000 0400  dc..............
-000003d0: 0000 0300 0000 0300 0000 7320 0000 0088  ..........s ....
-000003e0: 016a 007c 0164 018d 017d 0387 0087 0166  .j.|.d...}.....f
-000003f0: 0264 0264 0384 087c 0344 0083 0153 0029  .d.d...|.D...S.)
-00000400: 044e 2901 7217 0000 0063 0100 0000 0000  .N).r....c......
-00000410: 0000 0000 0000 0200 0000 0600 0000 1300  ................
-00000420: 0000 7318 0000 0067 007c 005d 087d 0188  ..s....g.|.].}..
-00000430: 007c 0188 0164 008d 0291 0271 0253 0029  .|...d.....q.S.)
-00000440: 0172 1000 0000 7214 0000 0029 02da 022e  .r....r....)....
-00000450: 3072 1100 0000 a902 7213 0000 0072 0d00  0r......r....r..
-00000460: 0000 7214 0000 0072 1500 0000 da0a 3c6c  ..r....r......<l
-00000470: 6973 7463 6f6d 703e 1800 0000 7302 0000  istcomp>....s...
-00000480: 0018 007a 2254 6f6b 656e 2e66 6f72 5f75  ...z"Token.for_u
-00000490: 7365 722e 3c6c 6f63 616c 733e 2e3c 6c69  ser.<locals>.<li
-000004a0: 7374 636f 6d70 3e29 01da 1367 6574 5f74  stcomp>)...get_t
-000004b0: 6f6b 656e 735f 666f 725f 7573 6572 2904  okens_for_user).
-000004c0: 7213 0000 0072 1700 0000 720d 0000 00da  r....r....r.....
-000004d0: 0772 6563 6f72 6473 7214 0000 0072 1900  .recordsr....r..
-000004e0: 0000 7215 0000 00da 0866 6f72 5f75 7365  ..r......for_use
-000004f0: 7213 0000 0073 0400 0000 0c04 1401 7a0e  r....s........z.
-00000500: 546f 6b65 6e2e 666f 725f 7573 6572 da0b  Token.for_user..
-00000510: 6578 7069 7279 5f64 6179 73da 046e 616d  expiry_days..nam
-00000520: 65da 0b64 6573 6372 6970 7469 6f6e 6306  e..descriptionc.
-00000530: 0000 0000 0000 0000 0000 0007 0000 0006  ................
-00000540: 0000 0043 0000 0073 1e00 0000 7c05 6a00  ...C...s....|.j.
-00000550: 7c01 7c02 7c03 7c04 6401 8d04 7d06 7c00  |.|.|.|.d...}.|.
-00000560: 7c06 7c05 6402 8d02 5300 2903 4e29 0472  |.|.d...S.).N).r
-00000570: 1700 0000 721e 0000 0072 1f00 0000 7220  ....r....r....r 
-00000580: 0000 0072 1000 0000 2901 da0c 6372 6561  ...r....)...crea
-00000590: 7465 5f74 6f6b 656e 2907 7213 0000 0072  te_token).r....r
-000005a0: 1700 0000 721e 0000 0072 1f00 0000 7220  ....r....r....r 
-000005b0: 0000 0072 0d00 0000 7211 0000 0072 1400  ...r....r....r..
-000005c0: 0000 7214 0000 0072 1500 0000 da06 6372  ..r....r......cr
-000005d0: 6561 7465 1a00 0000 7308 0000 0004 0908  eate....s.......
-000005e0: 0106 ff0c 037a 0c54 6f6b 656e 2e63 7265  .....z.Token.cre
-000005f0: 6174 6563 0100 0000 0000 0000 0000 0000  atec............
-00000600: 0100 0000 0300 0000 4300 0000 7324 0000  ........C...s$..
-00000610: 007c 006a 006a 0164 0075 0173 084a 0082  .|.j.j.d.u.s.J..
-00000620: 017c 006a 026a 037c 006a 006a 016a 0464  .|.j.j.|.j.j.j.d
-00000630: 018d 0153 0029 024e 720f 0000 0029 0572  ...S.).Nr....).r
-00000640: 0a00 0000 da07 636f 6e74 6578 7472 0b00  ......contextr..
-00000650: 0000 da0c 6465 6c65 7465 5f74 6f6b 656e  ....delete_token
-00000660: 720c 0000 00a9 01da 0473 656c 6672 1400  r........selfr..
-00000670: 0000 7214 0000 0072 1500 0000 da06 6465  ..r....r......de
-00000680: 6c65 7465 2800 0000 7308 0000 0010 0106  lete(...s.......
-00000690: 0108 0106 ff7a 0c54 6f6b 656e 2e64 656c  .....z.Token.del
-000006a0: 6574 6572 1100 0000 6303 0000 0000 0000  eter....c.......
-000006b0: 0000 0000 0003 0000 0002 0000 0043 0000  .............C..
-000006c0: 0073 1000 0000 7c01 7c00 5f00 7c02 7c00  .s....|.|._.|.|.
-000006d0: 5f01 6400 5300 a901 4e29 0272 0a00 0000  _.d.S...N).r....
-000006e0: 720b 0000 0029 0372 2600 0000 7211 0000  r....).r&...r...
-000006f0: 0072 0d00 0000 7214 0000 0072 1400 0000  .r....r....r....
-00000700: 7215 0000 00da 085f 5f69 6e69 745f 5f2e  r......__init__.
-00000710: 0000 0073 0400 0000 0601 0a01 7a0e 546f  ...s........z.To
-00000720: 6b65 6e2e 5f5f 696e 6974 5f5f 6301 0000  ken.__init__c...
-00000730: 0000 0000 0000 0000 0001 0000 0002 0000  ................
-00000740: 0043 0000 0073 0a00 0000 7400 7c00 6a01  .C...s....t.|.j.
-00000750: 8301 5300 7228 0000 0029 0272 0500 0000  ..S.r(...).r....
-00000760: 720a 0000 0072 2500 0000 7214 0000 0072  r....r%...r....r
-00000770: 1400 0000 7215 0000 00da 0774 6f5f 6469  ....r......to_di
-00000780: 6374 3200 0000 7302 0000 000a 017a 0d54  ct2...s......z.T
-00000790: 6f6b 656e 2e74 6f5f 6469 6374 6301 0000  oken.to_dictc...
-000007a0: 0000 0000 0000 0000 0001 0000 0001 0000  ................
-000007b0: 0043 0000 00f3 0800 0000 7c00 6a00 6a01  .C........|.j.j.
-000007c0: 5300 7228 0000 0029 0272 0a00 0000 da06  S.r(...).r......
-000007d0: 7365 6372 6574 7225 0000 0072 1400 0000  secretr%...r....
-000007e0: 7214 0000 0072 1500 0000 722c 0000 0035  r....r....r,...5
-000007f0: 0000 00f3 0200 0000 0802 7a0c 546f 6b65  ..........z.Toke
-00000800: 6e2e 7365 6372 6574 6301 0000 0000 0000  n.secretc.......
-00000810: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
-00000820: 0072 2b00 0000 7228 0000 0029 0272 0a00  .r+...r(...).r..
-00000830: 0000 7217 0000 0072 2500 0000 7214 0000  ..r....r%...r...
-00000840: 0072 1400 0000 7215 0000 0072 1700 0000  .r....r....r....
-00000850: 3900 0000 722d 0000 007a 0d54 6f6b 656e  9...r-...z.Token
-00000860: 2e75 7365 725f 6964 4e29 16da 085f 5f6e  .user_idN)...__n
-00000870: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00000880: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
-00000890: 0800 0000 da0f 5f5f 616e 6e6f 7461 7469  ......__annotati
-000008a0: 6f6e 735f 5f72 0700 0000 da0b 636c 6173  ons__r......clas
-000008b0: 736d 6574 686f 64da 0373 7472 7216 0000  smethod..strr...
-000008c0: 0072 0300 0000 da04 6c69 7374 721d 0000  .r......listr...
-000008d0: 00da 0369 6e74 7222 0000 0072 2700 0000  ...intr"...r'...
-000008e0: 7229 0000 00da 0464 6963 7472 0200 0000  r).....dictr....
-000008f0: 722a 0000 00da 0870 726f 7065 7274 7972  r*.....propertyr
-00000900: 2c00 0000 7217 0000 0072 1400 0000 7214  ,...r....r....r.
-00000910: 0000 0072 1400 0000 7215 0000 0072 0900  ...r....r....r..
-00000920: 0000 0a00 0000 7340 0000 000a 0008 0108  ......s@........
-00000930: 0102 0218 0102 0402 0106 0102 ff02 0102  ................
-00000940: ff06 020c fe02 0602 0106 0202 fe02 0302  ................
-00000950: fd02 0402 fc06 0502 fb02 060c fa08 0d12  ................
-00000960: 0616 0402 0314 0102 0318 0172 0900 0000  ...........r....
-00000970: 4e29 0ada 0674 7970 696e 6772 0200 0000  N)...typingr....
-00000980: 7203 0000 00da 0573 6572 6465 7205 0000  r......serder...
-00000990: 00da 0864 656c 6567 6174 6572 0700 0000  ...delegater....
-000009a0: 7211 0000 0072 0800 0000 7209 0000 0072  r....r....r....r
-000009b0: 1400 0000 7214 0000 0072 1400 0000 7215  ....r....r....r.
-000009c0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-000009d0: 0073 0a00 0000 1002 0c02 0c01 0c01 1203  .s..............
+00000120: 5a08 6506 0908 6420 6404 6505 6409 6509  Z.e...d d.e.d.e.
+00000130: 6507 1900 6405 650a 6400 1900 6606 640a  e...d.e.d...f.d.
+00000140: 640b 8405 8301 5a0b 6506 0908 0908 6421  d.....Z.e.....d!
+00000150: 640c 650c 640d 6507 6404 6505 6409 6509  d.e.d.e.d.e.d.e.
+00000160: 6507 1900 640e 6509 6507 1900 660a 640f  e...d.e.e...f.d.
+00000170: 6410 8405 8301 5a0d 6411 6412 8400 5a0e  d.....Z.d.d...Z.
+00000180: 6413 6503 6404 6505 6604 6414 6415 8404  d.e.d.e.f.d.d...
+00000190: 5a0f 6422 6417 6510 6405 6511 6507 6512  Z.d"d.e.d.e.e.e.
+000001a0: 6602 1900 6604 6418 6419 8405 5a13 6514  f...f.d.d...Z.e.
+000001b0: 6405 6509 6507 1900 6602 641a 641b 8404  d.e.e...f.d.d...
+000001c0: 8301 5a15 6514 6405 6509 6507 1900 6602  ..Z.e.d.e.e...f.
+000001d0: 641c 641d 8404 8301 5a16 6514 6405 6509  d.d.....Z.e.d.e.
+000001e0: 6507 1900 6602 641e 641f 8404 8301 5a17  e...f.d.d.....Z.
+000001f0: 6408 5300 2923 da05 546f 6b65 6eda 0e5f  d.S.)#..Token.._
+00000200: 546f 6b65 6e5f 5f72 6563 6f72 64da 165f  Token__record.._
+00000210: 546f 6b65 6e5f 5f74 6f6b 656e 5f64 656c  Token__token_del
+00000220: 6567 6174 65da 0874 6f6b 656e 5f69 64da  egate..token_id.
+00000230: 0e74 6f6b 656e 5f64 656c 6567 6174 65da  .token_delegate.
+00000240: 0672 6574 7572 6e63 0300 0000 0000 0000  .returnc........
+00000250: 0000 0000 0400 0000 0400 0000 4300 0000  ............C...
+00000260: 7318 0000 007c 026a 007c 0164 018d 017d  s....|.j.|.d...}
+00000270: 037c 007c 037c 0264 028d 0253 0029 034e  .|.|.|.d...S.).N
+00000280: a901 720c 0000 00a9 02da 0672 6563 6f72  ..r........recor
+00000290: 6472 0d00 0000 2901 da15 6765 745f 746f  dr....)...get_to
+000002a0: 6b65 6e5f 6279 5f74 6f6b 656e 5f69 6429  ken_by_token_id)
+000002b0: 04da 0363 6c73 720c 0000 0072 0d00 0000  ...clsr....r....
+000002c0: 7211 0000 00a9 0072 1400 0000 faeb 2f63  r......r....../c
+000002d0: 6f64 6562 7569 6c64 2f6f 7574 7075 742f  odebuild/output/
+000002e0: 7372 6333 3537 3831 3132 3139 312f 7372  src3578112191/sr
+000002f0: 632f 636f 6465 7374 6172 2d63 6f6e 6e65  c/codestar-conne
+00000300: 6374 696f 6e73 2e75 732d 7765 7374 2d32  ctions.us-west-2
+00000310: 2e61 6d61 7a6f 6e61 7773 2e63 6f6d 2f67  .amazonaws.com/g
+00000320: 6974 2d68 7474 702f 3036 3631 3935 3131  it-http/06619511
+00000330: 3233 3835 2f75 732d 7765 7374 2d32 2f65  2385/us-west-2/e
+00000340: 3635 3032 6138 302d 6262 3465 2d34 6662  6502a80-bb4e-4fb
+00000350: 652d 3837 3263 2d35 6434 3263 3139 3336  e-872c-5d42c1936
+00000360: 3939 642f 726f 626f 746f 2d61 692f 726f  99d/roboto-ai/ro
+00000370: 626f 746f 2d68 6f73 7465 642d 6170 702f  boto-hosted-app/
+00000380: 7061 636b 6167 6573 2f72 6f62 6f74 6f5f  packages/roboto_
+00000390: 7364 6b2f 7372 632f 726f 626f 746f 5f73  sdk/src/roboto_s
+000003a0: 646b 2f64 6f6d 6169 6e2f 746f 6b65 6e73  dk/domain/tokens
+000003b0: 2f74 6f6b 656e 2e70 79da 0766 726f 6d5f  /token.py..from_
+000003c0: 6964 0e00 0000 7304 0000 000c 020c 017a  id....s........z
+000003d0: 0d54 6f6b 656e 2e66 726f 6d5f 6964 4eda  .Token.from_idN.
+000003e0: 0775 7365 725f 6964 6303 0000 0000 0000  .user_idc.......
+000003f0: 0000 0000 0004 0000 0003 0000 0003 0000  ................
+00000400: 0073 2000 0000 8801 6a00 7c02 6401 8d01  .s .....j.|.d...
+00000410: 7d03 8700 8701 6602 6402 6403 8408 7c03  }.....f.d.d...|.
+00000420: 4400 8301 5300 2904 4e29 0172 1700 0000  D...S.).N).r....
+00000430: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00000440: 0006 0000 0013 0000 0073 1800 0000 6700  .........s....g.
+00000450: 7c00 5d08 7d01 8800 7c01 8801 6400 8d02  |.].}...|...d...
+00000460: 9102 7102 5300 2901 7210 0000 0072 1400  ..q.S.).r....r..
+00000470: 0000 2902 da02 2e30 7211 0000 00a9 0272  ..)....0r......r
+00000480: 1300 0000 720d 0000 0072 1400 0000 7215  ....r....r....r.
+00000490: 0000 00da 0a3c 6c69 7374 636f 6d70 3e18  .....<listcomp>.
+000004a0: 0000 0073 0200 0000 1800 7a22 546f 6b65  ...s......z"Toke
+000004b0: 6e2e 666f 725f 7573 6572 2e3c 6c6f 6361  n.for_user.<loca
+000004c0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 2901  ls>.<listcomp>).
+000004d0: da13 6765 745f 746f 6b65 6e73 5f66 6f72  ..get_tokens_for
+000004e0: 5f75 7365 7229 0472 1300 0000 720d 0000  _user).r....r...
+000004f0: 0072 1700 0000 da07 7265 636f 7264 7372  .r......recordsr
+00000500: 1400 0000 7219 0000 0072 1500 0000 da08  ....r....r......
+00000510: 666f 725f 7573 6572 1300 0000 7304 0000  for_user....s...
+00000520: 000c 0414 017a 0e54 6f6b 656e 2e66 6f72  .....z.Token.for
+00000530: 5f75 7365 72da 0b65 7870 6972 795f 6461  _user..expiry_da
+00000540: 7973 da04 6e61 6d65 da0b 6465 7363 7269  ys..name..descri
+00000550: 7074 696f 6e63 0600 0000 0000 0000 0000  ptionc..........
+00000560: 0000 0700 0000 0600 0000 4300 0000 731e  ..........C...s.
+00000570: 0000 007c 036a 007c 047c 017c 027c 0564  ...|.j.|.|.|.|.d
+00000580: 018d 047d 067c 007c 067c 0364 028d 0253  ...}.|.|.|.d...S
+00000590: 0029 034e 2904 7217 0000 0072 1e00 0000  .).N).r....r....
+000005a0: 721f 0000 0072 2000 0000 7210 0000 0029  r....r ...r....)
+000005b0: 01da 0c63 7265 6174 655f 746f 6b65 6e29  ...create_token)
+000005c0: 0772 1300 0000 721e 0000 0072 1f00 0000  .r....r....r....
+000005d0: 720d 0000 0072 1700 0000 7220 0000 0072  r....r....r ...r
+000005e0: 1100 0000 7214 0000 0072 1400 0000 7215  ....r....r....r.
+000005f0: 0000 00da 0663 7265 6174 651a 0000 0073  .....create....s
+00000600: 0800 0000 0409 0801 06ff 0c03 7a0c 546f  ............z.To
+00000610: 6b65 6e2e 6372 6561 7465 6301 0000 0000  ken.createc.....
+00000620: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
+00000630: 0000 0073 2400 0000 7c00 6a00 6a01 6400  ...s$...|.j.j.d.
+00000640: 7501 7308 4a00 8201 7c00 6a02 6a03 7c00  u.s.J...|.j.j.|.
+00000650: 6a00 6a01 6a04 6401 8d01 5300 2902 4e72  j.j.j.d...S.).Nr
+00000660: 0f00 0000 2905 720a 0000 00da 0763 6f6e  ....).r......con
+00000670: 7465 7874 720b 0000 00da 0c64 656c 6574  textr......delet
+00000680: 655f 746f 6b65 6e72 0c00 0000 a901 da04  e_tokenr........
+00000690: 7365 6c66 7214 0000 0072 1400 0000 7215  selfr....r....r.
+000006a0: 0000 00da 0664 656c 6574 6528 0000 0073  .....delete(...s
+000006b0: 0800 0000 1001 0601 0801 06ff 7a0c 546f  ............z.To
+000006c0: 6b65 6e2e 6465 6c65 7465 7211 0000 0063  ken.deleter....c
+000006d0: 0300 0000 0000 0000 0000 0000 0300 0000  ................
+000006e0: 0200 0000 4300 0000 7310 0000 007c 017c  ....C...s....|.|
+000006f0: 005f 007c 027c 005f 0164 0053 00a9 014e  ._.|.|._.d.S...N
+00000700: 2902 720a 0000 0072 0b00 0000 2903 7226  ).r....r....).r&
+00000710: 0000 0072 1100 0000 720d 0000 0072 1400  ...r....r....r..
+00000720: 0000 7214 0000 0072 1500 0000 da08 5f5f  ..r....r......__
+00000730: 696e 6974 5f5f 2e00 0000 7304 0000 0006  init__....s.....
+00000740: 010a 017a 0e54 6f6b 656e 2e5f 5f69 6e69  ...z.Token.__ini
+00000750: 745f 5f46 da0c 6578 636c 7564 655f 6e6f  t__F..exclude_no
+00000760: 6e65 6302 0000 0000 0000 0000 0000 0002  nec.............
+00000770: 0000 0004 0000 0043 0000 0073 0e00 0000  .......C...s....
+00000780: 7400 7c00 6a01 7c01 6401 8d02 5300 2902  t.|.j.|.d...S.).
+00000790: 4e29 0172 2a00 0000 2902 7205 0000 0072  N).r*...).r....r
+000007a0: 0a00 0000 2902 7226 0000 0072 2a00 0000  ....).r&...r*...
+000007b0: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
+000007c0: 0774 6f5f 6469 6374 3200 0000 7302 0000  .to_dict2...s...
+000007d0: 000e 017a 0d54 6f6b 656e 2e74 6f5f 6469  ...z.Token.to_di
+000007e0: 6374 6301 0000 0000 0000 0000 0000 0001  ctc.............
+000007f0: 0000 0001 0000 0043 0000 00f3 0800 0000  .......C........
+00000800: 7c00 6a00 6a01 5300 7228 0000 0029 0272  |.j.j.S.r(...).r
+00000810: 0a00 0000 da06 7365 6372 6574 7225 0000  ......secretr%..
+00000820: 0072 1400 0000 7214 0000 0072 1500 0000  .r....r....r....
+00000830: 722d 0000 0035 0000 00f3 0200 0000 0802  r-...5..........
+00000840: 7a0c 546f 6b65 6e2e 7365 6372 6574 6301  z.Token.secretc.
+00000850: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+00000860: 0000 0043 0000 0072 2c00 0000 7228 0000  ...C...r,...r(..
+00000870: 0029 0272 0a00 0000 7217 0000 0072 2500  .).r....r....r%.
+00000880: 0000 7214 0000 0072 1400 0000 7215 0000  ..r....r....r...
+00000890: 0072 1700 0000 3900 0000 722e 0000 007a  .r....9...r....z
+000008a0: 0d54 6f6b 656e 2e75 7365 725f 6964 6301  .Token.user_idc.
+000008b0: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+000008c0: 0000 0043 0000 0073 1a00 0000 7c00 6a00  ...C...s....|.j.
+000008d0: 6a01 6400 7500 7208 6400 5300 7c00 6a00  j.d.u.r.d.S.|.j.
+000008e0: 6a01 6a02 5300 7228 0000 0029 0372 0a00  j.j.S.r(...).r..
+000008f0: 0000 7223 0000 0072 0c00 0000 7225 0000  ..r#...r....r%..
+00000900: 0072 1400 0000 7214 0000 0072 1500 0000  .r....r....r....
+00000910: 720c 0000 003d 0000 0073 0200 0000 1a02  r....=...s......
+00000920: 7a0e 546f 6b65 6e2e 746f 6b65 6e5f 6964  z.Token.token_id
+00000930: 7228 0000 0029 024e 4e29 0146 2918 da08  r(...).NN).F)...
+00000940: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+00000950: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+00000960: 5f5f 7208 0000 00da 0f5f 5f61 6e6e 6f74  __r......__annot
+00000970: 6174 696f 6e73 5f5f 7207 0000 00da 0b63  ations__r......c
+00000980: 6c61 7373 6d65 7468 6f64 da03 7374 7272  lassmethod..strr
+00000990: 1600 0000 7203 0000 00da 046c 6973 7472  ....r......listr
+000009a0: 1d00 0000 da03 696e 7472 2200 0000 7227  ......intr"...r'
+000009b0: 0000 0072 2900 0000 da04 626f 6f6c da04  ...r).....bool..
+000009c0: 6469 6374 7202 0000 0072 2b00 0000 da08  dictr....r+.....
+000009d0: 7072 6f70 6572 7479 722d 0000 0072 1700  propertyr-...r..
+000009e0: 0000 720c 0000 0072 1400 0000 7214 0000  ..r....r....r...
+000009f0: 0072 1400 0000 7215 0000 0072 0900 0000  .r....r....r....
+00000a00: 0a00 0000 734a 0000 000a 0008 0108 0102  ....sJ..........
+00000a10: 0218 0102 0402 0204 ff02 0102 ff06 0102  ................
+00000a20: ff06 020c fe02 0602 0602 0104 fa02 0202  ................
+00000a30: fe02 0302 fd02 0402 fc06 0502 fb06 060c  ................
+00000a40: fa08 0d12 061c 0402 0314 0102 0314 0102  ................
+00000a50: 0318 0172 0900 0000 4e29 0ada 0674 7970  ...r....N)...typ
+00000a60: 696e 6772 0200 0000 7203 0000 00da 0573  ingr....r......s
+00000a70: 6572 6465 7205 0000 00da 0864 656c 6567  erder......deleg
+00000a80: 6174 6572 0700 0000 7211 0000 0072 0800  ater....r....r..
+00000a90: 0000 7209 0000 0072 1400 0000 7214 0000  ..r....r....r...
+00000aa0: 0072 1400 0000 7215 0000 00da 083c 6d6f  .r....r......<mo
+00000ab0: 6475 6c65 3e01 0000 0073 0a00 0000 1002  dule>....s......
+00000ac0: 0c02 0c01 0c01 1203                      ........
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/delegate.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/tokens/delegate.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 
 
 class TokenDelegate(abc.ABC):
     def __init__(self):
         super().__init__()
 
     @abc.abstractmethod
-    def get_tokens_for_user(self, user_id: Optional[str]) -> list[TokenRecord]:
+    def get_tokens_for_user(self, user_id: Optional[str] = None) -> list[TokenRecord]:
         raise NotImplementedError("get_tokens_for_user")
 
     @abc.abstractmethod
     def create_token(
         self,
-        user_id: Optional[str],
         expiry_days: int,
         name: str,
-        description: Optional[str],
+        user_id: Optional[str] = None,
+        description: Optional[str] = None,
     ) -> TokenRecord:
         raise NotImplementedError("create_token")
 
     @abc.abstractmethod
     def delete_token(self, token_id: str) -> None:
         raise NotImplementedError("delete_token")
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/http_delegate.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/tokens/http_delegate.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,66 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 
 from typing import Optional
 
+from ...exceptions import RobotoHttpExceptionParse
 from ...http import (
-    USER_OVERRIDE_HEADER,
     HttpClient,
+    headers_for_org_and_user,
 )
 from ...serde import pydantic_jsonable_dict
 from .delegate import TokenDelegate
 from .http_resources import CreateTokenRequest
 from .record import TokenRecord
 
 
 class TokenHttpDelegate(TokenDelegate):
     __http_client: HttpClient
 
     def __init__(self, http_client: HttpClient):
         super().__init__()
         self.__http_client = http_client
 
-    def get_tokens_for_user(self, user_id: Optional[str]) -> list[TokenRecord]:
+    def get_tokens_for_user(self, user_id: Optional[str] = None) -> list[TokenRecord]:
         url = self.__http_client.url("v1/tokens")
-        headers = {}
-        if user_id is not None:
-            headers[USER_OVERRIDE_HEADER] = user_id
+        headers = headers_for_org_and_user(user_id=user_id)
+
+        with RobotoHttpExceptionParse():
+            response = self.__http_client.get(url=url, headers=headers)
 
-        response = self.__http_client.get(url=url, headers=headers)
         unmarshalled = response.from_json(json_path=["data"])
         return [TokenRecord.parse_obj(record) for record in unmarshalled]
 
     def create_token(
         self,
-        user_id: Optional[str],
         expiry_days: int,
         name: str,
-        description: Optional[str],
+        user_id: Optional[str] = None,
+        description: Optional[str] = None,
     ) -> TokenRecord:
         url = self.__http_client.url("v1/tokens")
-        headers = {"Content-Type": "application/json"}
-        if user_id is not None:
-            headers[USER_OVERRIDE_HEADER] = user_id
+        headers = headers_for_org_and_user(
+            user_id=user_id, additional_headers={"Content-Type": "application/json"}
+        )
 
         data = CreateTokenRequest(
             expiry_days=expiry_days, name=name, description=description
         )
 
-        response = self.__http_client.post(
-            url=url, headers=headers, data=pydantic_jsonable_dict(data)
-        )
+        with RobotoHttpExceptionParse():
+            response = self.__http_client.post(
+                url=url, headers=headers, data=pydantic_jsonable_dict(data)
+            )
         return TokenRecord.parse_obj(response.from_json(json_path=["data"]))
 
     def delete_token(self, token_id: str) -> None:
-        url = self.__http_client.url(f"v1/tokens/id/{token_id}")
-        self.__http_client.delete(url=url)
+        url = self.__http_client.url(f"v1/tokens/{token_id}")
+
+        with RobotoHttpExceptionParse():
+            self.__http_client.delete(url=url)
 
     def get_token_by_token_id(self, token_id: str) -> TokenRecord:
-        url = self.__http_client.url(f"v1/tokens/id/{token_id}")
-        response = self.__http_client.get(url=url)
+        url = self.__http_client.url(f"v1/tokens/{token_id}")
+
+        with RobotoHttpExceptionParse():
+            response = self.__http_client.get(url=url)
         return TokenRecord.parse_obj(response.from_json(json_path=["data"]))
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/tokens/token.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/tokens/token.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,27 +14,27 @@
     @classmethod
     def from_id(cls, token_id: str, token_delegate: TokenDelegate) -> "Token":
         record = token_delegate.get_token_by_token_id(token_id=token_id)
         return cls(record=record, token_delegate=token_delegate)
 
     @classmethod
     def for_user(
-        cls, user_id: Optional[str], token_delegate: TokenDelegate
+        cls, token_delegate: TokenDelegate, user_id: Optional[str] = None
     ) -> list["Token"]:
         records = token_delegate.get_tokens_for_user(user_id=user_id)
         return [cls(record=record, token_delegate=token_delegate) for record in records]
 
     @classmethod
     def create(
         cls,
-        user_id: Optional[str],
         expiry_days: int,
         name: str,
-        description: Optional[str],
         token_delegate: TokenDelegate,
+        user_id: Optional[str] = None,
+        description: Optional[str] = None,
     ):
         record = token_delegate.create_token(
             user_id=user_id, expiry_days=expiry_days, name=name, description=description
         )
         return cls(record=record, token_delegate=token_delegate)
 
     def delete(self):
@@ -43,17 +43,21 @@
             token_id=self.__record.context.token_id
         )
 
     def __init__(self, record: TokenRecord, token_delegate: TokenDelegate):
         self.__record = record
         self.__token_delegate = token_delegate
 
-    def to_dict(self) -> dict[str, Any]:
-        return pydantic_jsonable_dict(self.__record)
+    def to_dict(self, exclude_none: bool = False) -> dict[str, Any]:
+        return pydantic_jsonable_dict(self.__record, exclude_none=exclude_none)
 
     @property
     def secret(self) -> Optional[str]:
         return self.__record.secret
 
     @property
     def user_id(self) -> Optional[str]:
         return self.__record.user_id
+
+    @property
+    def token_id(self) -> Optional[str]:
+        return None if self.__record.context is None else self.__record.context.token_id
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/__pycache__/__init__.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/triggers/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 391 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 8701 0000  o.......1..d....
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 8701 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 0100 6700 6406 a201  d.l.m.Z...g.d...
 00000070: 5a0a 6407 5300 2908 e901 0000 0029 01da  Z.d.S.)......)..
@@ -18,16 +18,16 @@
 00000110: 7474 705f 7265 736f 7572 6365 7372 0300  ttp_resourcesr..
 00000120: 0000 5a07 7472 6967 6765 7272 0400 0000  ..Z.triggerr....
 00000130: 5a10 7472 6967 6765 725f 6465 6c65 6761  Z.trigger_delega
 00000140: 7465 7205 0000 005a 0e74 7269 6767 6572  ter....Z.trigger
 00000150: 5f72 6563 6f72 6472 0600 0000 da07 5f5f  _recordr......__
 00000160: 616c 6c5f 5fa9 0072 0a00 0000 720a 0000  all__..r....r...
 00000170: 00fa f02f 636f 6465 6275 696c 642f 6f75  .../codebuild/ou
-00000180: 7470 7574 2f73 7263 3136 3839 3135 3533  tput/src16891553
-00000190: 3939 2f73 7263 2f63 6f64 6573 7461 722d  99/src/codestar-
+00000180: 7470 7574 2f73 7263 3335 3738 3131 3231  tput/src35781121
+00000190: 3931 2f73 7263 2f63 6f64 6573 7461 722d  91/src/codestar-
 000001a0: 636f 6e6e 6563 7469 6f6e 732e 7573 2d77  connections.us-w
 000001b0: 6573 742d 322e 616d 617a 6f6e 6177 732e  est-2.amazonaws.
 000001c0: 636f 6d2f 6769 742d 6874 7470 2f30 3636  com/git-http/066
 000001d0: 3139 3531 3132 3338 352f 7573 2d77 6573  195112385/us-wes
 000001e0: 742d 322f 6536 3530 3261 3830 2d62 6234  t-2/e6502a80-bb4
 000001f0: 652d 3466 6265 2d38 3732 632d 3564 3432  e-4fbe-872c-5d42
 00000200: 6331 3933 3639 3964 2f72 6f62 6f74 6f2d  c193699d/roboto-
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/__pycache__/http_resources.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/triggers/__pycache__/http_resources.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 205 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 cd00 0000  o.......1..d....
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 cd00 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 1e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 4700 6402 6403 8400 6403  d.l.Z.G.d.d...d.
 00000040: 6500 6a01 8303 5a02 6401 5300 2904 e900  e.j...Z.d.S.)...
 00000050: 0000 004e 6300 0000 0000 0000 0000 0000  ...Nc...........
 00000060: 0000 0000 0003 0000 0040 0000 0073 2a00  .........@...s*.
 00000070: 0000 6500 5a01 6400 5a02 5500 6503 6a04  ..e.Z.d.Z.U.e.j.
@@ -15,15 +15,15 @@
 000000e0: 2908 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
 000000f0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
 00000100: 6e61 6d65 5f5f da08 7079 6461 6e74 6963  name__..pydantic
 00000110: da05 4669 656c 6472 0400 0000 da03 7374  ..Fieldr......st
 00000120: 72da 0f5f 5f61 6e6e 6f74 6174 696f 6e73  r..__annotations
 00000130: 5f5f a900 720d 0000 0072 0d00 0000 faf6  __..r....r......
 00000140: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
-00000150: 742f 7372 6331 3638 3931 3535 3339 392f  t/src1689155399/
+00000150: 742f 7372 6333 3537 3831 3132 3139 312f  t/src3578112191/
 00000160: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
 00000170: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
 00000180: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
 00000190: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
 000001a0: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
 000001b0: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
 000001c0: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/__pycache__/trigger.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/triggers/__pycache__/trigger.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 2685 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 7d0a 0000  o.......1..d}...
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 7d0a 0000  o..........d}...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5a00 0000 6400  .....@...sZ...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 6d04 5a04 0100 6403 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 0100 6403 6405 6c07 6d08 5a08 0100 6406  ..d.d.l.m.Z...d.
 00000060: 6407 6c09 6d0a 5a0a 0100 6406 6408 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 4700 6409 640a 8400 640a  m.Z...G.d.d...d.
@@ -46,16 +46,16 @@
 000002d0: 720e 0000 0072 0f00 0000 7210 0000 00a9  r....r....r.....
 000002e0: 03da 0672 6563 6f72 6472 1100 0000 7212  ...recordr....r.
 000002f0: 0000 0029 01da 0e63 7265 6174 655f 7472  ...)...create_tr
 00000300: 6967 6765 7229 07da 0363 6c73 720e 0000  igger)...clsr...
 00000310: 0072 0f00 0000 7210 0000 0072 1100 0000  .r....r....r....
 00000320: 7212 0000 0072 1500 0000 a900 7218 0000  r....r......r...
 00000330: 00fa ef2f 636f 6465 6275 696c 642f 6f75  .../codebuild/ou
-00000340: 7470 7574 2f73 7263 3136 3839 3135 3533  tput/src16891553
-00000350: 3939 2f73 7263 2f63 6f64 6573 7461 722d  99/src/codestar-
+00000340: 7470 7574 2f73 7263 3335 3738 3131 3231  tput/src35781121
+00000350: 3931 2f73 7263 2f63 6f64 6573 7461 722d  91/src/codestar-
 00000360: 636f 6e6e 6563 7469 6f6e 732e 7573 2d77  connections.us-w
 00000370: 6573 742d 322e 616d 617a 6f6e 6177 732e  est-2.amazonaws.
 00000380: 636f 6d2f 6769 742d 6874 7470 2f30 3636  com/git-http/066
 00000390: 3139 3531 3132 3338 352f 7573 2d77 6573  195112385/us-wes
 000003a0: 742d 322f 6536 3530 3261 3830 2d62 6234  t-2/e6502a80-bb4
 000003b0: 652d 3466 6265 2d38 3732 632d 3564 3432  e-4fbe-872c-5d42
 000003c0: 6331 3933 3639 3964 2f72 6f62 6f74 6f2d  c193699d/roboto-
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/__pycache__/trigger_delegate.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/triggers/__pycache__/trigger_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 882 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 7203 0000  o.......1..dr...
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 7203 0000  o..........dr...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6403 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6405 6406 6c06 6d07 5a07 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6407 6408 8400 6408 6500 6a08 8303 5a09  d.d...d.e.j...Z.
 00000070: 6401 5300 2909 e900 0000 004e 2902 da03  d.S.)......N)...
@@ -28,15 +28,15 @@
 000001b0: 0000 0200 0000 4300 0000 f308 0000 0074  ......C........t
 000001c0: 0064 0183 0182 0129 024e da0e 6372 6561  .d.....).N..crea
 000001d0: 7465 5f74 7269 6767 6572 a901 da13 4e6f  te_trigger....No
 000001e0: 7449 6d70 6c65 6d65 6e74 6564 4572 726f  tImplementedErro
 000001f0: 7229 04da 0473 656c 6672 0900 0000 720a  r)...selfr....r.
 00000200: 0000 0072 0b00 0000 a900 7212 0000 00fa  ...r......r.....
 00000210: f82f 636f 6465 6275 696c 642f 6f75 7470  ./codebuild/outp
-00000220: 7574 2f73 7263 3136 3839 3135 3533 3939  ut/src1689155399
+00000220: 7574 2f73 7263 3335 3738 3131 3231 3931  ut/src3578112191
 00000230: 2f73 7263 2f63 6f64 6573 7461 722d 636f  /src/codestar-co
 00000240: 6e6e 6563 7469 6f6e 732e 7573 2d77 6573  nnections.us-wes
 00000250: 742d 322e 616d 617a 6f6e 6177 732e 636f  t-2.amazonaws.co
 00000260: 6d2f 6769 742d 6874 7470 2f30 3636 3139  m/git-http/06619
 00000270: 3531 3132 3338 352f 7573 2d77 6573 742d  5112385/us-west-
 00000280: 322f 6536 3530 3261 3830 2d62 6234 652d  2/e6502a80-bb4e-
 00000290: 3466 6265 2d38 3732 632d 3564 3432 6331  4fbe-872c-5d42c1
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/__pycache__/trigger_record.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/triggers/__pycache__/trigger_record.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 249 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 f900 0000  o.......1..d....
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 f900 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 1e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 4700 6402 6403 8400 6403  d.l.Z.G.d.d...d.
 00000040: 6500 6a01 8303 5a02 6401 5300 2904 e900  e.j...Z.d.S.)...
 00000050: 0000 004e 6300 0000 0000 0000 0000 0000  ...Nc...........
 00000060: 0000 0000 0003 0000 0040 0000 0073 2600  .........@...s&.
 00000070: 0000 6500 5a01 6400 5a02 5500 6503 6504  ..e.Z.d.Z.U.e.e.
@@ -12,15 +12,15 @@
 000000b0: 066f 7267 5f69 64da 0b61 6374 696f 6e5f  .org_id..action_
 000000c0: 6e61 6d65 4e29 05da 085f 5f6e 616d 655f  nameN)...__name_
 000000d0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
 000000e0: 5f71 7561 6c6e 616d 655f 5fda 0373 7472  _qualname__..str
 000000f0: da0f 5f5f 616e 6e6f 7461 7469 6f6e 735f  ..__annotations_
 00000100: 5fa9 0072 0b00 0000 720b 0000 00fa f62f  _..r....r....../
 00000110: 636f 6465 6275 696c 642f 6f75 7470 7574  codebuild/output
-00000120: 2f73 7263 3136 3839 3135 3533 3939 2f73  /src1689155399/s
+00000120: 2f73 7263 3335 3738 3131 3231 3931 2f73  /src3578112191/s
 00000130: 7263 2f63 6f64 6573 7461 722d 636f 6e6e  rc/codestar-conn
 00000140: 6563 7469 6f6e 732e 7573 2d77 6573 742d  ections.us-west-
 00000150: 322e 616d 617a 6f6e 6177 732e 636f 6d2f  2.amazonaws.com/
 00000160: 6769 742d 6874 7470 2f30 3636 3139 3531  git-http/0661951
 00000170: 3132 3338 352f 7573 2d77 6573 742d 322f  12385/us-west-2/
 00000180: 6536 3530 3261 3830 2d62 6234 652d 3466  e6502a80-bb4e-4f
 00000190: 6265 2d38 3732 632d 3564 3432 6331 3933  be-872c-5d42c193
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/http_delegate.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/triggers/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/trigger.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/triggers/trigger.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/triggers/trigger_delegate.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/triggers/trigger_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/users/__pycache__/__init__.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/users/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 262 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 0601 0000  o.......1..d....
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 0601 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6700  ..d.d.l.m.Z...g.
 00000060: 6405 a201 5a08 6406 5300 2907 e901 0000  d...Z.d.S.).....
 00000070: 0029 01da 1055 7365 7248 7474 7044 656c  .)...UserHttpDel
@@ -13,15 +13,15 @@
 000000c0: 004e 2909 da0d 6874 7470 5f64 656c 6567  .N)...http_deleg
 000000d0: 6174 6572 0200 0000 da04 7573 6572 7203  ater......userr.
 000000e0: 0000 005a 0d75 7365 725f 6465 6c65 6761  ...Z.user_delega
 000000f0: 7465 7204 0000 005a 0b75 7365 725f 7265  ter....Z.user_re
 00000100: 636f 7264 7205 0000 00da 075f 5f61 6c6c  cordr......__all
 00000110: 5f5f a900 7209 0000 0072 0900 0000 faed  __..r....r......
 00000120: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
-00000130: 742f 7372 6331 3638 3931 3535 3339 392f  t/src1689155399/
+00000130: 742f 7372 6333 3537 3831 3132 3139 312f  t/src3578112191/
 00000140: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
 00000150: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
 00000160: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
 00000170: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
 00000180: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
 00000190: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
 000001a0: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/users/__pycache__/user.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/users/__pycache__/user.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 1408 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,139 +1,141 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 8005 0000  o.......1..d....
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 b705 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6402  d.l.m.Z.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6404 6405 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6404 6406 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 4700 6407 6408 8400 6408 8302 5a09  ..G.d.d...d...Z.
 00000070: 6409 5300 290a e900 0000 0029 02da 0341  d.S.)......)...A
 00000080: 6e79 da08 4f70 7469 6f6e 616c e903 0000  ny..Optional....
 00000090: 0029 01da 1670 7964 616e 7469 635f 6a73  .)...pydantic_js
 000000a0: 6f6e 6162 6c65 5f64 6963 74e9 0100 0000  onable_dict.....
 000000b0: 2901 da0c 5573 6572 4465 6c65 6761 7465  )...UserDelegate
 000000c0: 2901 da0a 5573 6572 5265 636f 7264 6300  )...UserRecordc.
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0007  ................
-000000e0: 0000 0040 0000 0073 ce00 0000 6500 5a01  ...@...s....e.Z.
+000000e0: 0000 0040 0000 0073 d400 0000 6500 5a01  ...@...s....e.Z.
 000000f0: 6400 5a02 5500 6503 6504 6401 3c00 6505  d.Z.U.e.e.d.<.e.
-00000100: 6504 6402 3c00 6506 641a 6404 6505 6405  e.d.<.e.d.d.e.d.
+00000100: 6504 6402 3c00 6506 641c 6404 6505 6405  e.d.<.e.d.d.e.d.
 00000110: 6507 6508 1900 6604 6406 6407 8405 8301  e.e...f.d.d.....
 00000120: 5a09 6408 6503 6404 6505 6604 6409 640a  Z.d.e.d.e.f.d.d.
-00000130: 8404 5a0a 640b 650b 6508 650c 6602 1900  ..Z.d.e.e.e.f...
-00000140: 6602 640c 640d 8404 5a0d 641b 640e 640f  f.d.d...Z.d.d.d.
-00000150: 8404 5a0e 650f 640b 6508 6602 6410 6411  ..Z.e.d.e.f.d.d.
-00000160: 8404 8301 5a10 650f 640b 6508 6602 6412  ....Z.e.d.e.f.d.
-00000170: 6413 8404 8301 5a11 650f 640b 6512 6602  d.....Z.e.d.e.f.
-00000180: 6414 6415 8404 8301 5a13 650f 640b 6507  d.d.....Z.e.d.e.
-00000190: 6508 1900 6602 6416 6417 8404 8301 5a14  e...f.d.d.....Z.
-000001a0: 650f 640b 6507 6508 1900 6602 6418 6419  e.d.e.e...f.d.d.
-000001b0: 8404 8301 5a15 6403 5300 291c da04 5573  ....Z.d.S.)...Us
-000001c0: 6572 da0d 5f55 7365 725f 5f72 6563 6f72  er.._User__recor
-000001d0: 64da 145f 5573 6572 5f5f 7573 6572 5f64  d.._User__user_d
-000001e0: 656c 6567 6174 654e da0d 7573 6572 5f64  elegateN..user_d
-000001f0: 656c 6567 6174 65da 0775 7365 725f 6964  elegate..user_id
-00000200: 6303 0000 0000 0000 0000 0000 0004 0000  c...............
-00000210: 0004 0000 0043 0000 0073 1800 0000 7c01  .....C...s....|.
-00000220: 6a00 7c02 6401 8d01 7d03 7c00 7c03 7c01  j.|.d...}.|.|.|.
-00000230: 6402 8d02 5300 2903 4ea9 0172 0d00 0000  d...S.).N..r....
-00000240: 2902 da06 7265 636f 7264 720c 0000 0029  )...recordr....)
-00000250: 01da 0e67 6574 5f75 7365 725f 6279 5f69  ...get_user_by_i
-00000260: 6429 04da 0363 6c73 720c 0000 0072 0d00  d)...clsr....r..
-00000270: 0000 720f 0000 00a9 0072 1200 0000 fae9  ..r......r......
-00000280: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
-00000290: 742f 7372 6331 3638 3931 3535 3339 392f  t/src1689155399/
-000002a0: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
-000002b0: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
-000002c0: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
-000002d0: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
-000002e0: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
-000002f0: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
-00000300: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
-00000310: 3336 3939 642f 726f 626f 746f 2d61 692f  3699d/roboto-ai/
-00000320: 726f 626f 746f 2d68 6f73 7465 642d 6170  roboto-hosted-ap
-00000330: 702f 7061 636b 6167 6573 2f72 6f62 6f74  p/packages/robot
-00000340: 6f5f 7364 6b2f 7372 632f 726f 626f 746f  o_sdk/src/roboto
-00000350: 5f73 646b 2f64 6f6d 6169 6e2f 7573 6572  _sdk/domain/user
-00000360: 732f 7573 6572 2e70 79da 0766 726f 6d5f  s/user.py..from_
-00000370: 6964 0e00 0000 7304 0000 000c 020c 017a  id....s........z
-00000380: 0c55 7365 722e 6672 6f6d 5f69 6472 0f00  .User.from_idr..
-00000390: 0000 6303 0000 0000 0000 0000 0000 0003  ..c.............
-000003a0: 0000 0002 0000 0043 0000 0073 1000 0000  .......C...s....
-000003b0: 7c01 7c00 5f00 7c02 7c00 5f01 6400 5300  |.|._.|.|._.d.S.
-000003c0: a901 4e29 0272 0a00 0000 720b 0000 0029  ..N).r....r....)
-000003d0: 03da 0473 656c 6672 0f00 0000 720c 0000  ...selfr....r...
-000003e0: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
-000003f0: da08 5f5f 696e 6974 5f5f 1300 0000 7304  ..__init__....s.
-00000400: 0000 0006 010a 017a 0d55 7365 722e 5f5f  .......z.User.__
-00000410: 696e 6974 5f5f da06 7265 7475 726e 6301  init__..returnc.
-00000420: 0000 0000 0000 0000 0000 0001 0000 0002  ................
-00000430: 0000 0043 0000 0073 0a00 0000 7400 7c00  ...C...s....t.|.
-00000440: 6a01 8301 5300 7215 0000 0029 0272 0500  j...S.r....).r..
-00000450: 0000 720a 0000 00a9 0172 1600 0000 7212  ..r......r....r.
-00000460: 0000 0072 1200 0000 7213 0000 00da 0774  ...r....r......t
-00000470: 6f5f 6469 6374 1700 0000 7302 0000 000a  o_dict....s.....
-00000480: 017a 0c55 7365 722e 746f 5f64 6963 7463  .z.User.to_dictc
-00000490: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000004a0: 0300 0000 4300 0000 7312 0000 007c 006a  ....C...s....|.j
-000004b0: 006a 017c 006a 026a 0364 018d 0153 0029  .j.|.j.j.d...S.)
-000004c0: 024e 720e 0000 0029 0472 0b00 0000 da0b  .Nr....).r......
-000004d0: 6465 6c65 7465 5f75 7365 7272 0a00 0000  delete_userr....
-000004e0: 720d 0000 0072 1900 0000 7212 0000 0072  r....r....r....r
-000004f0: 1200 0000 7213 0000 00da 0664 656c 6574  ....r......delet
-00000500: 651a 0000 0073 0200 0000 1201 7a0b 5573  e....s......z.Us
-00000510: 6572 2e64 656c 6574 6563 0100 0000 0000  er.deletec......
-00000520: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
-00000530: 0000 f308 0000 007c 006a 006a 0153 0072  .......|.j.j.S.r
-00000540: 1500 0000 a902 720a 0000 0072 0d00 0000  ......r....r....
-00000550: 7219 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
-00000560: 1300 0000 720d 0000 001d 0000 00f3 0200  ....r...........
-00000570: 0000 0802 7a0c 5573 6572 2e75 7365 725f  ....z.User.user_
-00000580: 6964 6301 0000 0000 0000 0000 0000 0001  idc.............
-00000590: 0000 0001 0000 0043 0000 0072 1d00 0000  .......C...r....
-000005a0: 7215 0000 0072 1e00 0000 7219 0000 0072  r....r....r....r
-000005b0: 1200 0000 7212 0000 0072 1300 0000 da08  ....r....r......
-000005c0: 7573 6572 6e61 6d65 2100 0000 721f 0000  username!...r...
-000005d0: 007a 0d55 7365 722e 7573 6572 6e61 6d65  .z.User.username
-000005e0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-000005f0: 0002 0000 0043 0000 0073 1800 0000 7c00  .....C...s....|.
-00000600: 6a00 6a01 6400 7501 720a 7c00 6a00 6a01  j.j.d.u.r.|.j.j.
-00000610: 5300 6401 5300 2902 4e46 2902 720a 0000  S.d.S.).NF).r...
-00000620: 00da 0e69 735f 7379 7374 656d 5f75 7365  ...is_system_use
-00000630: 7272 1900 0000 7212 0000 0072 1200 0000  rr....r....r....
-00000640: 7213 0000 0072 2100 0000 2500 0000 730a  r....r!...%...s.
-00000650: 0000 000c 0406 ff02 ff02 0302 fd7a 1355  .............z.U
-00000660: 7365 722e 6973 5f73 7973 7465 6d5f 7573  ser.is_system_us
-00000670: 6572 6301 0000 0000 0000 0000 0000 0001  erc.............
-00000680: 0000 0001 0000 0043 0000 0072 1d00 0000  .......C...r....
-00000690: 7215 0000 0029 0272 0a00 0000 da04 6e61  r....).r......na
-000006a0: 6d65 7219 0000 0072 1200 0000 7212 0000  mer....r....r...
-000006b0: 0072 1300 0000 7222 0000 002d 0000 0072  .r....r"...-...r
-000006c0: 1f00 0000 7a09 5573 6572 2e6e 616d 6563  ....z.User.namec
-000006d0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000006e0: 0100 0000 4300 0000 721d 0000 0072 1500  ....C...r....r..
-000006f0: 0000 2902 720a 0000 00da 0b70 6963 7475  ..).r......pictu
-00000700: 7265 5f75 726c 7219 0000 0072 1200 0000  re_urlr....r....
-00000710: 7212 0000 0072 1300 0000 7223 0000 0031  r....r....r#...1
-00000720: 0000 0072 1f00 0000 7a10 5573 6572 2e70  ...r....z.User.p
-00000730: 6963 7475 7265 5f75 726c 7215 0000 0029  icture_urlr....)
-00000740: 0272 1800 0000 4e29 16da 085f 5f6e 616d  .r....N)...__nam
-00000750: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00000760: 0c5f 5f71 7561 6c6e 616d 655f 5f72 0800  .__qualname__r..
-00000770: 0000 da0f 5f5f 616e 6e6f 7461 7469 6f6e  ....__annotation
-00000780: 735f 5f72 0700 0000 da0b 636c 6173 736d  s__r......classm
-00000790: 6574 686f 6472 0300 0000 da03 7374 7272  ethodr......strr
-000007a0: 1400 0000 7217 0000 00da 0464 6963 7472  ....r......dictr
-000007b0: 0200 0000 721a 0000 0072 1c00 0000 da08  ....r....r......
-000007c0: 7072 6f70 6572 7479 720d 0000 0072 2000  propertyr....r .
-000007d0: 0000 da04 626f 6f6c 7221 0000 0072 2200  ....boolr!...r".
-000007e0: 0000 7223 0000 0072 1200 0000 7212 0000  ..r#...r....r...
-000007f0: 0072 1200 0000 7213 0000 0072 0900 0000  .r....r....r....
-00000800: 0a00 0000 7324 0000 000a 0008 0108 0102  ....s$..........
-00000810: 021a 0112 0416 040a 0302 0310 0102 0310  ................
-00000820: 0102 0310 0102 0714 0102 0318 0172 0900  .............r..
-00000830: 0000 4e29 0ada 0674 7970 696e 6772 0200  ..N)...typingr..
-00000840: 0000 7203 0000 00da 0573 6572 6465 7205  ..r......serder.
-00000850: 0000 0072 0c00 0000 7207 0000 00da 0b75  ...r....r......u
-00000860: 7365 725f 7265 636f 7264 7208 0000 0072  ser_recordr....r
-00000870: 0900 0000 7212 0000 0072 1200 0000 7212  ....r....r....r.
-00000880: 0000 0072 1300 0000 da08 3c6d 6f64 756c  ...r......<modul
-00000890: 653e 0100 0000 730a 0000 0010 020c 020c  e>....s.........
-000008a0: 010c 0112 03                             .....
+00000130: 8404 5a0a 641d 640c 650b 640d 650c 6508  ..Z.d.d.e.d.e.e.
+00000140: 650d 6602 1900 6604 640e 640f 8405 5a0e  e.f...f.d.d...Z.
+00000150: 641e 6410 6411 8404 5a0f 6510 640d 6508  d.d.d...Z.e.d.e.
+00000160: 6602 6412 6413 8404 8301 5a11 6510 640d  f.d.d.....Z.e.d.
+00000170: 6508 6602 6414 6415 8404 8301 5a12 6510  e.f.d.d.....Z.e.
+00000180: 640d 650b 6602 6416 6417 8404 8301 5a13  d.e.f.d.d.....Z.
+00000190: 6510 640d 6507 6508 1900 6602 6418 6419  e.d.e.e...f.d.d.
+000001a0: 8404 8301 5a14 6510 640d 6507 6508 1900  ....Z.e.d.e.e...
+000001b0: 6602 641a 641b 8404 8301 5a15 6403 5300  f.d.d.....Z.d.S.
+000001c0: 291f da04 5573 6572 da0d 5f55 7365 725f  )...User.._User_
+000001d0: 5f72 6563 6f72 64da 145f 5573 6572 5f5f  _record.._User__
+000001e0: 7573 6572 5f64 656c 6567 6174 654e da0d  user_delegateN..
+000001f0: 7573 6572 5f64 656c 6567 6174 65da 0775  user_delegate..u
+00000200: 7365 725f 6964 6303 0000 0000 0000 0000  ser_idc.........
+00000210: 0000 0004 0000 0004 0000 0043 0000 0073  ...........C...s
+00000220: 1800 0000 7c01 6a00 7c02 6401 8d01 7d03  ....|.j.|.d...}.
+00000230: 7c00 7c03 7c01 6402 8d02 5300 2903 4ea9  |.|.|.d...S.).N.
+00000240: 0172 0d00 0000 2902 da06 7265 636f 7264  .r....)...record
+00000250: 720c 0000 0029 01da 0e67 6574 5f75 7365  r....)...get_use
+00000260: 725f 6279 5f69 6429 04da 0363 6c73 720c  r_by_id)...clsr.
+00000270: 0000 0072 0d00 0000 720f 0000 00a9 0072  ...r....r......r
+00000280: 1200 0000 fae9 2f63 6f64 6562 7569 6c64  ....../codebuild
+00000290: 2f6f 7574 7075 742f 7372 6333 3537 3831  /output/src35781
+000002a0: 3132 3139 312f 7372 632f 636f 6465 7374  12191/src/codest
+000002b0: 6172 2d63 6f6e 6e65 6374 696f 6e73 2e75  ar-connections.u
+000002c0: 732d 7765 7374 2d32 2e61 6d61 7a6f 6e61  s-west-2.amazona
+000002d0: 7773 2e63 6f6d 2f67 6974 2d68 7474 702f  ws.com/git-http/
+000002e0: 3036 3631 3935 3131 3233 3835 2f75 732d  066195112385/us-
+000002f0: 7765 7374 2d32 2f65 3635 3032 6138 302d  west-2/e6502a80-
+00000300: 6262 3465 2d34 6662 652d 3837 3263 2d35  bb4e-4fbe-872c-5
+00000310: 6434 3263 3139 3336 3939 642f 726f 626f  d42c193699d/robo
+00000320: 746f 2d61 692f 726f 626f 746f 2d68 6f73  to-ai/roboto-hos
+00000330: 7465 642d 6170 702f 7061 636b 6167 6573  ted-app/packages
+00000340: 2f72 6f62 6f74 6f5f 7364 6b2f 7372 632f  /roboto_sdk/src/
+00000350: 726f 626f 746f 5f73 646b 2f64 6f6d 6169  roboto_sdk/domai
+00000360: 6e2f 7573 6572 732f 7573 6572 2e70 79da  n/users/user.py.
+00000370: 0766 726f 6d5f 6964 0e00 0000 7304 0000  .from_id....s...
+00000380: 000c 020c 017a 0c55 7365 722e 6672 6f6d  .....z.User.from
+00000390: 5f69 6472 0f00 0000 6303 0000 0000 0000  _idr....c.......
+000003a0: 0000 0000 0003 0000 0002 0000 0043 0000  .............C..
+000003b0: 0073 1000 0000 7c01 7c00 5f00 7c02 7c00  .s....|.|._.|.|.
+000003c0: 5f01 6400 5300 a901 4e29 0272 0a00 0000  _.d.S...N).r....
+000003d0: 720b 0000 0029 03da 0473 656c 6672 0f00  r....)...selfr..
+000003e0: 0000 720c 0000 0072 1200 0000 7212 0000  ..r....r....r...
+000003f0: 0072 1300 0000 da08 5f5f 696e 6974 5f5f  .r......__init__
+00000400: 1300 0000 7304 0000 0006 010a 017a 0d55  ....s........z.U
+00000410: 7365 722e 5f5f 696e 6974 5f5f 46da 0c65  ser.__init__F..e
+00000420: 7863 6c75 6465 5f6e 6f6e 65da 0672 6574  xclude_none..ret
+00000430: 7572 6e63 0200 0000 0000 0000 0000 0000  urnc............
+00000440: 0200 0000 0400 0000 4300 0000 730e 0000  ........C...s...
+00000450: 0074 007c 006a 017c 0164 018d 0253 0029  .t.|.j.|.d...S.)
+00000460: 024e 2901 7218 0000 0029 0272 0500 0000  .N).r....).r....
+00000470: 720a 0000 0029 0272 1600 0000 7218 0000  r....).r....r...
+00000480: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
+00000490: da07 746f 5f64 6963 7417 0000 0073 0200  ..to_dict....s..
+000004a0: 0000 0e01 7a0c 5573 6572 2e74 6f5f 6469  ....z.User.to_di
+000004b0: 6374 6301 0000 0000 0000 0000 0000 0001  ctc.............
+000004c0: 0000 0003 0000 0043 0000 0073 1200 0000  .......C...s....
+000004d0: 7c00 6a00 6a01 7c00 6a02 6a03 6401 8d01  |.j.j.|.j.j.d...
+000004e0: 5300 2902 4e72 0e00 0000 2904 720b 0000  S.).Nr....).r...
+000004f0: 00da 0b64 656c 6574 655f 7573 6572 720a  ...delete_userr.
+00000500: 0000 0072 0d00 0000 a901 7216 0000 0072  ...r......r....r
+00000510: 1200 0000 7212 0000 0072 1300 0000 da06  ....r....r......
+00000520: 6465 6c65 7465 1a00 0000 7302 0000 0012  delete....s.....
+00000530: 017a 0b55 7365 722e 6465 6c65 7465 6301  .z.User.deletec.
+00000540: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+00000550: 0000 0043 0000 00f3 0800 0000 7c00 6a00  ...C........|.j.
+00000560: 6a01 5300 7215 0000 00a9 0272 0a00 0000  j.S.r......r....
+00000570: 720d 0000 0072 1c00 0000 7212 0000 0072  r....r....r....r
+00000580: 1200 0000 7213 0000 0072 0d00 0000 1d00  ....r....r......
+00000590: 0000 f302 0000 0008 027a 0c55 7365 722e  .........z.User.
+000005a0: 7573 6572 5f69 6463 0100 0000 0000 0000  user_idc........
+000005b0: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
+000005c0: 721e 0000 0072 1500 0000 721f 0000 0072  r....r....r....r
+000005d0: 1c00 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
+000005e0: 0000 00da 0875 7365 726e 616d 6521 0000  .....username!..
+000005f0: 0072 2000 0000 7a0d 5573 6572 2e75 7365  .r ...z.User.use
+00000600: 726e 616d 6563 0100 0000 0000 0000 0000  rnamec..........
+00000610: 0000 0100 0000 0200 0000 4300 0000 7318  ..........C...s.
+00000620: 0000 007c 006a 006a 0164 0075 0172 0a7c  ...|.j.j.d.u.r.|
+00000630: 006a 006a 0153 0064 0153 0029 024e 4629  .j.j.S.d.S.).NF)
+00000640: 0272 0a00 0000 da0e 6973 5f73 7973 7465  .r......is_syste
+00000650: 6d5f 7573 6572 721c 0000 0072 1200 0000  m_userr....r....
+00000660: 7212 0000 0072 1300 0000 7222 0000 0025  r....r....r"...%
+00000670: 0000 0073 0a00 0000 0c04 06ff 02ff 0203  ...s............
+00000680: 02fd 7a13 5573 6572 2e69 735f 7379 7374  ..z.User.is_syst
+00000690: 656d 5f75 7365 7263 0100 0000 0000 0000  em_userc........
+000006a0: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
+000006b0: 721e 0000 0072 1500 0000 2902 720a 0000  r....r....).r...
+000006c0: 00da 046e 616d 6572 1c00 0000 7212 0000  ...namer....r...
+000006d0: 0072 1200 0000 7213 0000 0072 2300 0000  .r....r....r#...
+000006e0: 2d00 0000 7220 0000 007a 0955 7365 722e  -...r ...z.User.
+000006f0: 6e61 6d65 6301 0000 0000 0000 0000 0000  namec...........
+00000700: 0001 0000 0001 0000 0043 0000 0072 1e00  .........C...r..
+00000710: 0000 7215 0000 0029 0272 0a00 0000 da0b  ..r....).r......
+00000720: 7069 6374 7572 655f 7572 6c72 1c00 0000  picture_urlr....
+00000730: 7212 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
+00000740: 2400 0000 3100 0000 7220 0000 007a 1055  $...1...r ...z.U
+00000750: 7365 722e 7069 6374 7572 655f 7572 6c72  ser.picture_urlr
+00000760: 1500 0000 2901 4629 0272 1900 0000 4e29  ....).F).r....N)
+00000770: 16da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+00000780: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00000790: 616d 655f 5f72 0800 0000 da0f 5f5f 616e  ame__r......__an
+000007a0: 6e6f 7461 7469 6f6e 735f 5f72 0700 0000  notations__r....
+000007b0: da0b 636c 6173 736d 6574 686f 6472 0300  ..classmethodr..
+000007c0: 0000 da03 7374 7272 1400 0000 7217 0000  ....strr....r...
+000007d0: 00da 0462 6f6f 6cda 0464 6963 7472 0200  ...bool..dictr..
+000007e0: 0000 721a 0000 0072 1d00 0000 da08 7072  ..r....r......pr
+000007f0: 6f70 6572 7479 720d 0000 0072 2100 0000  opertyr....r!...
+00000800: 7222 0000 0072 2300 0000 7224 0000 0072  r"...r#...r$...r
+00000810: 1200 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
+00000820: 0000 0072 0900 0000 0a00 0000 7324 0000  ...r........s$..
+00000830: 000a 0008 0108 0102 021a 0112 041c 040a  ................
+00000840: 0302 0310 0102 0310 0102 0310 0102 0714  ................
+00000850: 0102 0318 0172 0900 0000 4e29 0ada 0674  .....r....N)...t
+00000860: 7970 696e 6772 0200 0000 7203 0000 00da  ypingr....r.....
+00000870: 0573 6572 6465 7205 0000 0072 0c00 0000  .serder....r....
+00000880: 7207 0000 00da 0b75 7365 725f 7265 636f  r......user_reco
+00000890: 7264 7208 0000 0072 0900 0000 7212 0000  rdr....r....r...
+000008a0: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
+000008b0: da08 3c6d 6f64 756c 653e 0100 0000 730a  ..<module>....s.
+000008c0: 0000 0010 020c 020c 010c 0112 03         .............
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/users/__pycache__/user_delegate.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/users/__pycache__/user_delegate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 485 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 e501 0000  o.......1..d....
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 f301 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6403 6404 6c03 6d04 5a04 0100 4700  ..d.d.l.m.Z...G.
 00000050: 6405 6406 8400 6406 6500 6a05 8303 5a06  d.d...d.e.j...Z.
 00000060: 6401 5300 2907 e900 0000 004e 2901 da08  d.S.)......N)...
 00000070: 4f70 7469 6f6e 616c e901 0000 0029 01da  Optional.....)..
 00000080: 0a55 7365 7252 6563 6f72 6463 0000 0000  .UserRecordc....
-00000090: 0000 0000 0000 0000 0000 0000 0500 0000  ................
-000000a0: 0000 0000 7354 0000 0065 005a 0164 005a  ....sT...e.Z.d.Z
+00000090: 0000 0000 0000 0000 0000 0000 0600 0000  ................
+000000a0: 0000 0000 7358 0000 0065 005a 0164 005a  ....sX...e.Z.d.Z
 000000b0: 0287 0066 0164 0164 0284 085a 0365 046a  ...f.d.d...Z.e.j
-000000c0: 0564 0365 0665 0719 0064 0465 0866 0464  .d.e.e...d.e.f.d
-000000d0: 0564 0684 0483 015a 0965 046a 0564 0365  .d.....Z.e.j.d.e
-000000e0: 0665 0719 0064 0464 0766 0464 0864 0984  .e...d.d.f.d.d..
-000000f0: 0483 015a 0a87 0004 005a 0b53 0029 0ada  ...Z.....Z.S.)..
-00000100: 0c55 7365 7244 656c 6567 6174 6563 0100  .UserDelegatec..
-00000110: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-00000120: 0000 0300 0000 730e 0000 0074 0083 00a0  ......s....t....
-00000130: 01a1 0001 0064 0053 0029 014e 2902 da05  .....d.S.).N)...
-00000140: 7375 7065 72da 085f 5f69 6e69 745f 5f29  super..__init__)
-00000150: 01da 0473 656c 66a9 01da 095f 5f63 6c61  ...self....__cla
-00000160: 7373 5f5f a900 faf2 2f63 6f64 6562 7569  ss__..../codebui
-00000170: 6c64 2f6f 7574 7075 742f 7372 6331 3638  ld/output/src168
-00000180: 3931 3535 3339 392f 7372 632f 636f 6465  9155399/src/code
-00000190: 7374 6172 2d63 6f6e 6e65 6374 696f 6e73  star-connections
-000001a0: 2e75 732d 7765 7374 2d32 2e61 6d61 7a6f  .us-west-2.amazo
-000001b0: 6e61 7773 2e63 6f6d 2f67 6974 2d68 7474  naws.com/git-htt
-000001c0: 702f 3036 3631 3935 3131 3233 3835 2f75  p/066195112385/u
-000001d0: 732d 7765 7374 2d32 2f65 3635 3032 6138  s-west-2/e6502a8
-000001e0: 302d 6262 3465 2d34 6662 652d 3837 3263  0-bb4e-4fbe-872c
-000001f0: 2d35 6434 3263 3139 3336 3939 642f 726f  -5d42c193699d/ro
-00000200: 626f 746f 2d61 692f 726f 626f 746f 2d68  boto-ai/roboto-h
-00000210: 6f73 7465 642d 6170 702f 7061 636b 6167  osted-app/packag
-00000220: 6573 2f72 6f62 6f74 6f5f 7364 6b2f 7372  es/roboto_sdk/sr
-00000230: 632f 726f 626f 746f 5f73 646b 2f64 6f6d  c/roboto_sdk/dom
-00000240: 6169 6e2f 7573 6572 732f 7573 6572 5f64  ain/users/user_d
-00000250: 656c 6567 6174 652e 7079 7207 0000 000a  elegate.pyr.....
-00000260: 0000 0073 0200 0000 0e01 7a15 5573 6572  ...s......z.User
-00000270: 4465 6c65 6761 7465 2e5f 5f69 6e69 745f  Delegate.__init_
-00000280: 5fda 0775 7365 725f 6964 da06 7265 7475  _..user_id..retu
-00000290: 726e 6302 0000 0000 0000 0000 0000 0002  rnc.............
-000002a0: 0000 0002 0000 0043 0000 00f3 0800 0000  .......C........
-000002b0: 7400 6401 8301 8201 2902 4eda 0e67 6574  t.d.....).N..get
-000002c0: 5f75 7365 725f 6279 5f69 64a9 01da 134e  _user_by_id....N
-000002d0: 6f74 496d 706c 656d 656e 7465 6445 7272  otImplementedErr
-000002e0: 6f72 a902 7208 0000 0072 0d00 0000 720b  or..r....r....r.
-000002f0: 0000 0072 0b00 0000 720c 0000 0072 1000  ...r....r....r..
-00000300: 0000 0d00 0000 f302 0000 0008 027a 1b55  .............z.U
-00000310: 7365 7244 656c 6567 6174 652e 6765 745f  serDelegate.get_
-00000320: 7573 6572 5f62 795f 6964 4e63 0200 0000  user_by_idNc....
-00000330: 0000 0000 0000 0000 0200 0000 0200 0000  ................
-00000340: 4300 0000 720f 0000 0029 024e da0b 6465  C...r....).N..de
-00000350: 6c65 7465 5f75 7365 7272 1100 0000 7213  lete_userr....r.
-00000360: 0000 0072 0b00 0000 720b 0000 0072 0c00  ...r....r....r..
-00000370: 0000 7215 0000 0011 0000 0072 1400 0000  ..r........r....
-00000380: 7a18 5573 6572 4465 6c65 6761 7465 2e64  z.UserDelegate.d
-00000390: 656c 6574 655f 7573 6572 290c da08 5f5f  elete_user)...__
-000003a0: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-000003b0: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-000003c0: 7207 0000 00da 0361 6263 da0e 6162 7374  r......abc..abst
-000003d0: 7261 6374 6d65 7468 6f64 7202 0000 00da  ractmethodr.....
-000003e0: 0373 7472 7204 0000 0072 1000 0000 7215  .strr....r....r.
-000003f0: 0000 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
-00000400: 5f5f 720b 0000 0072 0b00 0000 7209 0000  __r....r....r...
-00000410: 0072 0c00 0000 7205 0000 0009 0000 0073  .r....r........s
-00000420: 0c00 0000 0800 0c01 0403 1801 0403 2001  .............. .
-00000430: 7205 0000 0029 0772 1900 0000 da06 7479  r....).r......ty
-00000440: 7069 6e67 7202 0000 00da 0b75 7365 725f  pingr......user_
-00000450: 7265 636f 7264 7204 0000 00da 0341 4243  recordr......ABC
-00000460: 7205 0000 0072 0b00 0000 720b 0000 0072  r....r....r....r
-00000470: 0b00 0000 720c 0000 00da 083c 6d6f 6475  ....r......<modu
-00000480: 6c65 3e01 0000 0073 0800 0000 0802 0c01  le>....s........
-00000490: 0c02 1603                                ....
+000000c0: 0564 0a64 0465 0665 0719 0064 0565 0866  .d.d.e.e...d.e.f
+000000d0: 0464 0664 0784 0583 015a 0965 046a 0564  .d.d.....Z.e.j.d
+000000e0: 0a64 0465 0665 0719 0064 0564 0366 0464  .d.e.e...d.d.f.d
+000000f0: 0864 0984 0583 015a 0a87 0004 005a 0b53  .d.....Z.....Z.S
+00000100: 0029 0bda 0c55 7365 7244 656c 6567 6174  .)...UserDelegat
+00000110: 6563 0100 0000 0000 0000 0000 0000 0100  ec..............
+00000120: 0000 0200 0000 0300 0000 730e 0000 0074  ..........s....t
+00000130: 0083 00a0 01a1 0001 0064 0053 00a9 014e  .........d.S...N
+00000140: 2902 da05 7375 7065 72da 085f 5f69 6e69  )...super..__ini
+00000150: 745f 5f29 01da 0473 656c 66a9 01da 095f  t__)...self...._
+00000160: 5f63 6c61 7373 5f5f a900 faf2 2f63 6f64  _class__..../cod
+00000170: 6562 7569 6c64 2f6f 7574 7075 742f 7372  ebuild/output/sr
+00000180: 6333 3537 3831 3132 3139 312f 7372 632f  c3578112191/src/
+00000190: 636f 6465 7374 6172 2d63 6f6e 6e65 6374  codestar-connect
+000001a0: 696f 6e73 2e75 732d 7765 7374 2d32 2e61  ions.us-west-2.a
+000001b0: 6d61 7a6f 6e61 7773 2e63 6f6d 2f67 6974  mazonaws.com/git
+000001c0: 2d68 7474 702f 3036 3631 3935 3131 3233  -http/0661951123
+000001d0: 3835 2f75 732d 7765 7374 2d32 2f65 3635  85/us-west-2/e65
+000001e0: 3032 6138 302d 6262 3465 2d34 6662 652d  02a80-bb4e-4fbe-
+000001f0: 3837 3263 2d35 6434 3263 3139 3336 3939  872c-5d42c193699
+00000200: 642f 726f 626f 746f 2d61 692f 726f 626f  d/roboto-ai/robo
+00000210: 746f 2d68 6f73 7465 642d 6170 702f 7061  to-hosted-app/pa
+00000220: 636b 6167 6573 2f72 6f62 6f74 6f5f 7364  ckages/roboto_sd
+00000230: 6b2f 7372 632f 726f 626f 746f 5f73 646b  k/src/roboto_sdk
+00000240: 2f64 6f6d 6169 6e2f 7573 6572 732f 7573  /domain/users/us
+00000250: 6572 5f64 656c 6567 6174 652e 7079 7208  er_delegate.pyr.
+00000260: 0000 000a 0000 0073 0200 0000 0e01 7a15  .......s......z.
+00000270: 5573 6572 4465 6c65 6761 7465 2e5f 5f69  UserDelegate.__i
+00000280: 6e69 745f 5f4e da07 7573 6572 5f69 64da  nit__N..user_id.
+00000290: 0672 6574 7572 6e63 0200 0000 0000 0000  .returnc........
+000002a0: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
+000002b0: f308 0000 0074 0064 0183 0182 0129 024e  .....t.d.....).N
+000002c0: da0e 6765 745f 7573 6572 5f62 795f 6964  ..get_user_by_id
+000002d0: a901 da13 4e6f 7449 6d70 6c65 6d65 6e74  ....NotImplement
+000002e0: 6564 4572 726f 72a9 0272 0900 0000 720e  edError..r....r.
+000002f0: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
+00000300: 0000 7211 0000 000d 0000 00f3 0200 0000  ..r.............
+00000310: 0802 7a1b 5573 6572 4465 6c65 6761 7465  ..z.UserDelegate
+00000320: 2e67 6574 5f75 7365 725f 6279 5f69 6463  .get_user_by_idc
+00000330: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00000340: 0200 0000 4300 0000 7210 0000 0029 024e  ....C...r....).N
+00000350: da0b 6465 6c65 7465 5f75 7365 7272 1200  ..delete_userr..
+00000360: 0000 7214 0000 0072 0c00 0000 720c 0000  ..r....r....r...
+00000370: 0072 0d00 0000 7216 0000 0011 0000 0072  .r....r........r
+00000380: 1500 0000 7a18 5573 6572 4465 6c65 6761  ....z.UserDelega
+00000390: 7465 2e64 656c 6574 655f 7573 6572 7206  te.delete_userr.
+000003a0: 0000 0029 0cda 085f 5f6e 616d 655f 5fda  ...)...__name__.
+000003b0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+000003c0: 7561 6c6e 616d 655f 5f72 0800 0000 da03  ualname__r......
+000003d0: 6162 63da 0e61 6273 7472 6163 746d 6574  abc..abstractmet
+000003e0: 686f 6472 0200 0000 da03 7374 7272 0400  hodr......strr..
+000003f0: 0000 7211 0000 0072 1600 0000 da0d 5f5f  ..r....r......__
+00000400: 636c 6173 7363 656c 6c5f 5f72 0c00 0000  classcell__r....
+00000410: 720c 0000 0072 0a00 0000 720d 0000 0072  r....r....r....r
+00000420: 0500 0000 0900 0000 730c 0000 0008 000c  ........s.......
+00000430: 0104 031a 0104 0322 0172 0500 0000 2907  .......".r....).
+00000440: 721a 0000 00da 0674 7970 696e 6772 0200  r......typingr..
+00000450: 0000 da0b 7573 6572 5f72 6563 6f72 6472  ....user_recordr
+00000460: 0400 0000 da03 4142 4372 0500 0000 720c  ......ABCr....r.
+00000470: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
+00000480: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00000490: 7308 0000 0008 020c 010c 0216 03         s............
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/users/__pycache__/user_record.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/users/__pycache__/user_record.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 257 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 0101 0000  o.......1..d....
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 0101 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2a00 0000 6400  .....@...s*...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 4700 6403 6404 8400 6404 6502 6a03  Z.G.d.d...d.e.j.
 00000050: 8303 5a04 6402 5300 2905 e900 0000 0029  ..Z.d.S.)......)
 00000060: 01da 084f 7074 696f 6e61 6c4e 6300 0000  ...OptionalNc...
 00000070: 0000 0000 0000 0000 0000 0000 0003 0000  ................
@@ -18,15 +18,15 @@
 00000110: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
 00000120: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
 00000130: 5f5f da03 7374 72da 0f5f 5f61 6e6e 6f74  __..str..__annot
 00000140: 6174 696f 6e73 5f5f 7205 0000 0072 0200  ations__r....r..
 00000150: 0000 da04 626f 6f6c 7206 0000 0072 0700  ....boolr....r..
 00000160: 0000 a900 720e 0000 0072 0e00 0000 faf0  ....r....r......
 00000170: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
-00000180: 742f 7372 6331 3638 3931 3535 3339 392f  t/src1689155399/
+00000180: 742f 7372 6333 3537 3831 3132 3139 312f  t/src3578112191/
 00000190: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
 000001a0: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
 000001b0: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
 000001c0: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
 000001d0: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
 000001e0: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
 000001f0: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/domain/users/user.py` & `roboto_sdk-0.1.7/src/roboto_sdk/domain/users/user.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,16 +16,16 @@
         record = user_delegate.get_user_by_id(user_id=user_id)
         return cls(record=record, user_delegate=user_delegate)
 
     def __init__(self, record: UserRecord, user_delegate: UserDelegate):
         self.__record = record
         self.__user_delegate = user_delegate
 
-    def to_dict(self) -> dict[str, Any]:
-        return pydantic_jsonable_dict(self.__record)
+    def to_dict(self, exclude_none: bool = False) -> dict[str, Any]:
+        return pydantic_jsonable_dict(self.__record, exclude_none=exclude_none)
 
     def delete(self) -> None:
         return self.__user_delegate.delete_user(user_id=self.__record.user_id)
 
     @property
     def user_id(self) -> str:
         return self.__record.user_id
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/exceptions/__pycache__/domain.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/exceptions/__pycache__/domain.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 1266 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,132 +1,151 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 f204 0000  o.......1..d....
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 2006 0000  o..........d ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
+00000020: 0004 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6502 8303 5a03 4700 6404 6405  ..d.e...Z.G.d.d.
 00000050: 8400 6405 6504 8303 5a05 4700 6406 6407  ..d.e...Z.G.d.d.
 00000060: 8400 6407 6503 8303 5a06 4700 6408 6409  ..d.e...Z.G.d.d.
 00000070: 8400 6409 6503 8303 5a07 4700 640a 640b  ..d.e...Z.G.d.d.
-00000080: 8400 640b 6503 8303 5a08 640c 5300 290d  ..d.e...Z.d.S.).
-00000090: e902 0000 0029 01da 0b43 6c69 656e 7445  .....)...ClientE
-000000a0: 7272 6f72 6300 0000 0000 0000 0000 0000  rrorc...........
-000000b0: 0000 0000 0004 0000 0040 0000 0073 2200  .........@...s".
-000000c0: 0000 6500 5a01 6400 5a02 6401 5a03 6504  ..e.Z.d.Z.d.Z.e.
-000000d0: 6402 6505 6602 6403 6404 8404 8301 5a06  d.e.f.d.d.....Z.
-000000e0: 6405 5300 2906 da15 526f 626f 746f 446f  d.S.)...RobotoDo
-000000f0: 6d61 696e 4578 6365 7074 696f 6e7a 440a  mainExceptionzD.
-00000100: 2020 2020 4578 7065 6374 6564 2065 7863      Expected exc
-00000110: 6570 7469 6f6e 7320 6672 6f6d 2074 6865  eptions from the
-00000120: 2052 6f62 6f74 6f20 646f 6d61 696e 2065   Roboto domain e
-00000130: 6e74 6974 7920 6f62 6a65 6374 732e 0a20  ntity objects.. 
-00000140: 2020 20da 0565 7272 6f72 6301 0000 0000     ..errorc.....
-00000150: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-00000160: 0000 0073 4000 0000 7c00 6a00 6401 6b02  ...s@...|.j.d.k.
-00000170: 720a 7401 7c00 6a02 8301 5300 7c00 6a00  r.t.|.j...S.|.j.
-00000180: 6402 7600 7214 7403 7c00 6a02 8301 5300  d.v.r.t.|.j...S.
-00000190: 7c00 6a00 6403 6b02 721e 7404 7c00 6a02  |.j.d.k.r.t.|.j.
-000001a0: 8301 5300 7c00 8201 2904 4e69 9001 0000  ..S.|...).Ni....
-000001b0: 2902 6991 0100 0069 9301 0000 6994 0100  ).i....i....i...
-000001c0: 0029 05da 0673 7461 7475 73da 1d52 6f62  .)...status..Rob
-000001d0: 6f74 6f49 6e76 616c 6964 5265 7175 6573  otoInvalidReques
-000001e0: 7445 7863 6570 7469 6f6e da03 6d73 67da  tException..msg.
-000001f0: 1b52 6f62 6f74 6f55 6e61 7574 686f 7269  .RobotoUnauthori
-00000200: 7a65 6445 7863 6570 7469 6f6e da17 526f  zedException..Ro
-00000210: 626f 746f 4e6f 7446 6f75 6e64 4578 6365  botoNotFoundExce
-00000220: 7074 696f 6ea9 0172 0400 0000 a900 720b  ption..r......r.
-00000230: 0000 00fa e92f 636f 6465 6275 696c 642f  ...../codebuild/
-00000240: 6f75 7470 7574 2f73 7263 3136 3839 3135  output/src168915
-00000250: 3533 3939 2f73 7263 2f63 6f64 6573 7461  5399/src/codesta
-00000260: 722d 636f 6e6e 6563 7469 6f6e 732e 7573  r-connections.us
-00000270: 2d77 6573 742d 322e 616d 617a 6f6e 6177  -west-2.amazonaw
-00000280: 732e 636f 6d2f 6769 742d 6874 7470 2f30  s.com/git-http/0
-00000290: 3636 3139 3531 3132 3338 352f 7573 2d77  66195112385/us-w
-000002a0: 6573 742d 322f 6536 3530 3261 3830 2d62  est-2/e6502a80-b
-000002b0: 6234 652d 3466 6265 2d38 3732 632d 3564  b4e-4fbe-872c-5d
-000002c0: 3432 6331 3933 3639 3964 2f72 6f62 6f74  42c193699d/robot
-000002d0: 6f2d 6169 2f72 6f62 6f74 6f2d 686f 7374  o-ai/roboto-host
-000002e0: 6564 2d61 7070 2f70 6163 6b61 6765 732f  ed-app/packages/
-000002f0: 726f 626f 746f 5f73 646b 2f73 7263 2f72  roboto_sdk/src/r
-00000300: 6f62 6f74 6f5f 7364 6b2f 6578 6365 7074  oboto_sdk/except
-00000310: 696f 6e73 2f64 6f6d 6169 6e2e 7079 da11  ions/domain.py..
-00000320: 6672 6f6d 5f63 6c69 656e 745f 6572 726f  from_client_erro
-00000330: 720b 0000 0073 0e00 0000 0a02 0a01 0a01  r....s..........
-00000340: 0a01 0a01 0a01 0401 7a27 526f 626f 746f  ........z'Roboto
-00000350: 446f 6d61 696e 4578 6365 7074 696f 6e2e  DomainException.
-00000360: 6672 6f6d 5f63 6c69 656e 745f 6572 726f  from_client_erro
-00000370: 724e 2907 da08 5f5f 6e61 6d65 5f5f da0a  rN)...__name__..
-00000380: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-00000390: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
-000003a0: 5fda 0c73 7461 7469 636d 6574 686f 6472  _..staticmethodr
-000003b0: 0200 0000 720d 0000 0072 0b00 0000 720b  ....r....r....r.
-000003c0: 0000 0072 0b00 0000 720c 0000 0072 0300  ...r....r....r..
-000003d0: 0000 0600 0000 7308 0000 0008 0004 0102  ......s.........
-000003e0: 0414 0172 0300 0000 6300 0000 0000 0000  ...r....c.......
-000003f0: 0000 0000 0000 0000 0002 0000 0040 0000  .............@..
-00000400: 0073 1c00 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
-00000410: 6402 8400 5a03 6403 6404 8400 5a04 6405  d...Z.d.d...Z.d.
-00000420: 5300 2906 da18 526f 626f 746f 4874 7470  S.)...RobotoHttp
-00000430: 4578 6365 7074 696f 6e50 6172 7365 6301  ExceptionParsec.
-00000440: 0000 0000 0000 0000 0000 0001 0000 0001  ................
-00000450: 0000 0043 0000 0073 0400 0000 7c00 5300  ...C...s....|.S.
-00000460: 2901 4e72 0b00 0000 2901 da04 7365 6c66  ).Nr....)...self
-00000470: 720b 0000 0072 0b00 0000 720c 0000 00da  r....r....r.....
-00000480: 095f 5f65 6e74 6572 5f5f 1700 0000 7302  .__enter__....s.
-00000490: 0000 0004 017a 2252 6f62 6f74 6f48 7474  .....z"RobotoHtt
-000004a0: 7045 7863 6570 7469 6f6e 5061 7273 652e  pExceptionParse.
-000004b0: 5f5f 656e 7465 725f 5f63 0400 0000 0000  __enter__c......
-000004c0: 0000 0000 0000 0400 0000 0300 0000 4300  ..............C.
-000004d0: 0000 7318 0000 007c 0174 0075 0072 0a74  ..s....|.t.u.r.t
-000004e0: 016a 027c 0264 018d 0182 0164 0053 0029  .j.|.d.....d.S.)
-000004f0: 024e 720a 0000 0029 0372 0200 0000 7203  .Nr....).r....r.
-00000500: 0000 0072 0d00 0000 2904 7214 0000 00da  ...r....).r.....
-00000510: 0e65 7863 6570 7469 6f6e 5f74 7970 65da  .exception_type.
-00000520: 0965 7863 6570 7469 6f6e da09 7472 6163  .exception..trac
-00000530: 6562 6163 6b72 0b00 0000 720b 0000 0072  ebackr....r....r
-00000540: 0c00 0000 da08 5f5f 6578 6974 5f5f 1a00  ......__exit__..
-00000550: 0000 7306 0000 0008 010c 0104 ff7a 2152  ..s..........z!R
-00000560: 6f62 6f74 6f48 7474 7045 7863 6570 7469  obotoHttpExcepti
-00000570: 6f6e 5061 7273 652e 5f5f 6578 6974 5f5f  onParse.__exit__
-00000580: 4e29 0572 0e00 0000 720f 0000 0072 1000  N).r....r....r..
-00000590: 0000 7215 0000 0072 1900 0000 720b 0000  ..r....r....r...
-000005a0: 0072 0b00 0000 720b 0000 0072 0c00 0000  .r....r....r....
-000005b0: 7213 0000 0016 0000 0073 0600 0000 0800  r........s......
-000005c0: 0801 0c03 7213 0000 0063 0000 0000 0000  ....r....c......
-000005d0: 0000 0000 0000 0000 0000 0100 0000 4000  ..............@.
-000005e0: 0000 f310 0000 0065 005a 0164 005a 0264  .......e.Z.d.Z.d
-000005f0: 015a 0364 0253 0029 0372 0800 0000 7a6a  .Z.d.S.).r....zj
-00000600: 0a20 2020 2054 6872 6f77 6e20 7768 656e  .    Thrown when
-00000610: 2061 2075 7365 7220 6973 2061 7474 656d   a user is attem
-00000620: 7074 696e 6720 746f 2061 6363 6573 7320  pting to access 
-00000630: 6120 7265 736f 7572 6365 2074 6861 7420  a resource that 
-00000640: 7468 6579 2064 6f20 6e6f 7420 6861 7665  they do not have
-00000650: 2070 6572 6d69 7373 696f 6e20 746f 2061   permission to a
-00000660: 6363 6573 730a 2020 2020 4ea9 0472 0e00  ccess.    N..r..
-00000670: 0000 720f 0000 0072 1000 0000 7211 0000  ..r....r....r...
-00000680: 0072 0b00 0000 720b 0000 0072 0b00 0000  .r....r....r....
-00000690: 720c 0000 0072 0800 0000 1f00 0000 f304  r....r..........
-000006a0: 0000 0008 0008 0172 0800 0000 6300 0000  .......r....c...
-000006b0: 0000 0000 0000 0000 0000 0000 0001 0000  ................
-000006c0: 0040 0000 0072 1a00 0000 2903 7209 0000  .@...r....).r...
-000006d0: 007a 380a 2020 2020 5468 726f 7720 7768  .z8.    Throw wh
-000006e0: 656e 2061 2072 6571 7565 7374 6564 2072  en a requested r
-000006f0: 6573 6f75 7263 6520 646f 6573 206e 6f74  esource does not
-00000700: 2065 7869 7374 0a20 2020 204e 721b 0000   exist.    Nr...
-00000710: 0072 0b00 0000 720b 0000 0072 0b00 0000  .r....r....r....
-00000720: 720c 0000 0072 0900 0000 2500 0000 721c  r....r....%...r.
-00000730: 0000 0072 0900 0000 6300 0000 0000 0000  ...r....c.......
-00000740: 0000 0000 0000 0000 0001 0000 0040 0000  .............@..
-00000750: 0072 1a00 0000 2903 7206 0000 007a 400a  .r....).r....z@.
-00000760: 2020 2020 5468 726f 776e 2077 6865 6e20      Thrown when 
-00000770: 7265 7175 6573 7420 7061 7261 6d65 7465  request paramete
-00000780: 7273 2061 7265 2069 6e20 736f 6d65 2077  rs are in some w
-00000790: 6179 2069 6e76 616c 6964 0a20 2020 204e  ay invalid.    N
-000007a0: 721b 0000 0072 0b00 0000 720b 0000 0072  r....r....r....r
-000007b0: 0b00 0000 720c 0000 0072 0600 0000 2b00  ....r....r....+.
-000007c0: 0000 721c 0000 0072 0600 0000 4e29 09da  ..r....r....N)..
-000007d0: 0468 7474 7072 0200 0000 da09 4578 6365  .httpr......Exce
-000007e0: 7074 696f 6e72 0300 0000 da06 6f62 6a65  ptionr......obje
-000007f0: 6374 7213 0000 0072 0800 0000 7209 0000  ctr....r....r...
-00000800: 0072 0600 0000 720b 0000 0072 0b00 0000  .r....r....r....
-00000810: 720b 0000 0072 0c00 0000 da08 3c6d 6f64  r....r......<mod
-00000820: 756c 653e 0100 0000 730c 0000 000c 0210  ule>....s.......
-00000830: 0310 1010 0910 0614 06                   .........
+00000080: 8400 640b 6503 8303 5a08 4700 640c 640d  ..d.e...Z.G.d.d.
+00000090: 8400 640d 6503 8303 5a09 640e 5300 290f  ..d.e...Z.d.S.).
+000000a0: e902 0000 0029 01da 0948 7474 7045 7272  .....)...HttpErr
+000000b0: 6f72 6300 0000 0000 0000 0000 0000 0000  orc.............
+000000c0: 0000 0004 0000 0040 0000 0073 2200 0000  .......@...s"...
+000000d0: 6500 5a01 6400 5a02 6401 5a03 6504 6402  e.Z.d.Z.d.Z.e.d.
+000000e0: 6505 6602 6403 6404 8404 8301 5a06 6405  e.f.d.d.....Z.d.
+000000f0: 5300 2906 da15 526f 626f 746f 446f 6d61  S.)...RobotoDoma
+00000100: 696e 4578 6365 7074 696f 6e7a 440a 2020  inExceptionzD.  
+00000110: 2020 4578 7065 6374 6564 2065 7863 6570    Expected excep
+00000120: 7469 6f6e 7320 6672 6f6d 2074 6865 2052  tions from the R
+00000130: 6f62 6f74 6f20 646f 6d61 696e 2065 6e74  oboto domain ent
+00000140: 6974 7920 6f62 6a65 6374 732e 0a20 2020  ity objects..   
+00000150: 20da 0565 7272 6f72 6301 0000 0000 0000   ..errorc.......
+00000160: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
+00000170: 0073 7a00 0000 7c00 6a00 6400 7500 720a  .sz...|.j.d.u.r.
+00000180: 7401 7c00 6a02 8301 8201 7c00 6a00 6401  t.|.j.....|.j.d.
+00000190: 6b02 7214 7403 7c00 6a02 8301 5300 7c00  k.r.t.|.j...S.|.
+000001a0: 6a00 6402 7600 721e 7404 7c00 6a02 8301  j.d.v.r.t.|.j...
+000001b0: 5300 7c00 6a00 6403 6b02 7228 7405 7c00  S.|.j.d.k.r(t.|.
+000001c0: 6a02 8301 5300 6404 7c00 6a00 0400 0300  j...S.d.|.j.....
+000001d0: 6b01 7233 6405 6b00 723b 6e03 0100 7c00  k.r3d.k.r;n...|.
+000001e0: 8201 7406 7c00 6a02 8301 5300 7c00 8201  ..t.|.j...S.|...
+000001f0: 2906 4e69 9001 0000 2902 6991 0100 0069  ).Ni....).i....i
+00000200: 9301 0000 6994 0100 0069 f401 0000 6958  ....i....i....iX
+00000210: 0200 0029 07da 0673 7461 7475 7372 0300  ...)...statusr..
+00000220: 0000 da03 6d73 67da 1d52 6f62 6f74 6f49  ....msg..RobotoI
+00000230: 6e76 616c 6964 5265 7175 6573 7445 7863  nvalidRequestExc
+00000240: 6570 7469 6f6e da1b 526f 626f 746f 556e  eption..RobotoUn
+00000250: 6175 7468 6f72 697a 6564 4578 6365 7074  authorizedExcept
+00000260: 696f 6eda 1752 6f62 6f74 6f4e 6f74 466f  ion..RobotoNotFo
+00000270: 756e 6445 7863 6570 7469 6f6e da12 526f  undException..Ro
+00000280: 626f 746f 5365 7276 6963 6545 7272 6f72  botoServiceError
+00000290: a901 7204 0000 00a9 0072 0c00 0000 fae9  ..r......r......
+000002a0: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
+000002b0: 742f 7372 6333 3537 3831 3132 3139 312f  t/src3578112191/
+000002c0: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
+000002d0: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
+000002e0: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
+000002f0: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
+00000300: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
+00000310: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
+00000320: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
+00000330: 3336 3939 642f 726f 626f 746f 2d61 692f  3699d/roboto-ai/
+00000340: 726f 626f 746f 2d68 6f73 7465 642d 6170  roboto-hosted-ap
+00000350: 702f 7061 636b 6167 6573 2f72 6f62 6f74  p/packages/robot
+00000360: 6f5f 7364 6b2f 7372 632f 726f 626f 746f  o_sdk/src/roboto
+00000370: 5f73 646b 2f65 7863 6570 7469 6f6e 732f  _sdk/exceptions/
+00000380: 646f 6d61 696e 2e70 79da 1166 726f 6d5f  domain.py..from_
+00000390: 636c 6965 6e74 5f65 7272 6f72 0b00 0000  client_error....
+000003a0: 7318 0000 000a 020a 010a 010a 010a 010a  s...............
+000003b0: 010a 010a 0118 0104 020a ff04 017a 2752  .............z'R
+000003c0: 6f62 6f74 6f44 6f6d 6169 6e45 7863 6570  obotoDomainExcep
+000003d0: 7469 6f6e 2e66 726f 6d5f 636c 6965 6e74  tion.from_client
+000003e0: 5f65 7272 6f72 4e29 07da 085f 5f6e 616d  _errorN)...__nam
+000003f0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+00000400: 0c5f 5f71 7561 6c6e 616d 655f 5fda 075f  .__qualname__.._
+00000410: 5f64 6f63 5f5f da0c 7374 6174 6963 6d65  _doc__..staticme
+00000420: 7468 6f64 7202 0000 0072 0e00 0000 720c  thodr....r....r.
+00000430: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
+00000440: 0000 7203 0000 0006 0000 0073 0800 0000  ..r........s....
+00000450: 0800 0401 0204 1401 7203 0000 0063 0000  ........r....c..
+00000460: 0000 0000 0000 0000 0000 0000 0000 0200  ................
+00000470: 0000 4000 0000 731c 0000 0065 005a 0164  ..@...s....e.Z.d
+00000480: 005a 0264 0164 0284 005a 0364 0364 0484  .Z.d.d...Z.d.d..
+00000490: 005a 0464 0553 0029 06da 1852 6f62 6f74  .Z.d.S.)...Robot
+000004a0: 6f48 7474 7045 7863 6570 7469 6f6e 5061  oHttpExceptionPa
+000004b0: 7273 6563 0100 0000 0000 0000 0000 0000  rsec............
+000004c0: 0100 0000 0100 0000 4300 0000 7304 0000  ........C...s...
+000004d0: 007c 0053 0029 014e 720c 0000 0029 01da  .|.S.).Nr....)..
+000004e0: 0473 656c 6672 0c00 0000 720c 0000 0072  .selfr....r....r
+000004f0: 0d00 0000 da09 5f5f 656e 7465 725f 5f1b  ......__enter__.
+00000500: 0000 0073 0200 0000 0401 7a22 526f 626f  ...s......z"Robo
+00000510: 746f 4874 7470 4578 6365 7074 696f 6e50  toHttpExceptionP
+00000520: 6172 7365 2e5f 5f65 6e74 6572 5f5f 6304  arse.__enter__c.
+00000530: 0000 0000 0000 0000 0000 0004 0000 0003  ................
+00000540: 0000 0043 0000 0073 1e00 0000 7400 7401  ...C...s....t.t.
+00000550: 7c02 8301 7402 8302 720d 7403 6a04 7c02  |...t...r.t.j.|.
+00000560: 6401 8d01 8201 6400 5300 2902 4e72 0b00  d.....d.S.).Nr..
+00000570: 0000 2905 da0a 6973 7375 6263 6c61 7373  ..)...issubclass
+00000580: da04 7479 7065 7202 0000 0072 0300 0000  ..typer....r....
+00000590: 720e 0000 0029 0472 1500 0000 da0e 6578  r....).r......ex
+000005a0: 6365 7074 696f 6e5f 7479 7065 da09 6578  ception_type..ex
+000005b0: 6365 7074 696f 6eda 0974 7261 6365 6261  ception..traceba
+000005c0: 636b 720c 0000 0072 0c00 0000 720d 0000  ckr....r....r...
+000005d0: 00da 085f 5f65 7869 745f 5f1e 0000 0073  ...__exit__....s
+000005e0: 0600 0000 0e01 0c01 04ff 7a21 526f 626f  ..........z!Robo
+000005f0: 746f 4874 7470 4578 6365 7074 696f 6e50  toHttpExceptionP
+00000600: 6172 7365 2e5f 5f65 7869 745f 5f4e 2905  arse.__exit__N).
+00000610: 720f 0000 0072 1000 0000 7211 0000 0072  r....r....r....r
+00000620: 1600 0000 721c 0000 0072 0c00 0000 720c  ....r....r....r.
+00000630: 0000 0072 0c00 0000 720d 0000 0072 1400  ...r....r....r..
+00000640: 0000 1a00 0000 7306 0000 0008 0008 010c  ......s.........
+00000650: 0372 1400 0000 6300 0000 0000 0000 0000  .r....c.........
+00000660: 0000 0000 0000 0001 0000 0040 0000 00f3  ...........@....
+00000670: 1000 0000 6500 5a01 6400 5a02 6401 5a03  ....e.Z.d.Z.d.Z.
+00000680: 6402 5300 2903 7208 0000 007a 6a0a 2020  d.S.).r....zj.  
+00000690: 2020 5468 726f 776e 2077 6865 6e20 6120    Thrown when a 
+000006a0: 7573 6572 2069 7320 6174 7465 6d70 7469  user is attempti
+000006b0: 6e67 2074 6f20 6163 6365 7373 2061 2072  ng to access a r
+000006c0: 6573 6f75 7263 6520 7468 6174 2074 6865  esource that the
+000006d0: 7920 646f 206e 6f74 2068 6176 6520 7065  y do not have pe
+000006e0: 726d 6973 7369 6f6e 2074 6f20 6163 6365  rmission to acce
+000006f0: 7373 0a20 2020 204e a904 720f 0000 0072  ss.    N..r....r
+00000700: 1000 0000 7211 0000 0072 1200 0000 720c  ....r....r....r.
+00000710: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
+00000720: 0000 7208 0000 0023 0000 00f3 0400 0000  ..r....#........
+00000730: 0800 0801 7208 0000 0063 0000 0000 0000  ....r....c......
+00000740: 0000 0000 0000 0000 0000 0100 0000 4000  ..............@.
+00000750: 0000 721d 0000 0029 0372 0900 0000 7a38  ..r....).r....z8
+00000760: 0a20 2020 2054 6872 6f77 2077 6865 6e20  .    Throw when 
+00000770: 6120 7265 7175 6573 7465 6420 7265 736f  a requested reso
+00000780: 7572 6365 2064 6f65 7320 6e6f 7420 6578  urce does not ex
+00000790: 6973 740a 2020 2020 4e72 1e00 0000 720c  ist.    Nr....r.
+000007a0: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
+000007b0: 0000 7209 0000 0029 0000 0072 1f00 0000  ..r....)...r....
+000007c0: 7209 0000 0063 0000 0000 0000 0000 0000  r....c..........
+000007d0: 0000 0000 0000 0100 0000 4000 0000 721d  ..........@...r.
+000007e0: 0000 0029 0372 0700 0000 7a40 0a20 2020  ...).r....z@.   
+000007f0: 2054 6872 6f77 6e20 7768 656e 2072 6571   Thrown when req
+00000800: 7565 7374 2070 6172 616d 6574 6572 7320  uest parameters 
+00000810: 6172 6520 696e 2073 6f6d 6520 7761 7920  are in some way 
+00000820: 696e 7661 6c69 640a 2020 2020 4e72 1e00  invalid.    Nr..
+00000830: 0000 720c 0000 0072 0c00 0000 720c 0000  ..r....r....r...
+00000840: 0072 0d00 0000 7207 0000 002f 0000 0072  .r....r..../...r
+00000850: 1f00 0000 7207 0000 0063 0000 0000 0000  ....r....c......
+00000860: 0000 0000 0000 0000 0000 0100 0000 4000  ..............@.
+00000870: 0000 721d 0000 0029 0372 0a00 0000 7a40  ..r....).r....z@
+00000880: 0a20 2020 2054 6872 6f77 6e20 7768 656e  .    Thrown when
+00000890: 2052 6f62 6f74 6f20 5365 7276 6963 6520   Roboto Service 
+000008a0: 6661 696c 6564 2069 6e20 616e 2075 6e65  failed in an une
+000008b0: 7870 6563 7465 6420 7761 790a 2020 2020  xpected way.    
+000008c0: 4e72 1e00 0000 720c 0000 0072 0c00 0000  Nr....r....r....
+000008d0: 720c 0000 0072 0d00 0000 720a 0000 0035  r....r....r....5
+000008e0: 0000 0072 1f00 0000 720a 0000 004e 290a  ...r....r....N).
+000008f0: da04 6874 7470 7202 0000 00da 0945 7863  ..httpr......Exc
+00000900: 6570 7469 6f6e 7203 0000 00da 066f 626a  eptionr......obj
+00000910: 6563 7472 1400 0000 7208 0000 0072 0900  ectr....r....r..
+00000920: 0000 7207 0000 0072 0a00 0000 720c 0000  ..r....r....r...
+00000930: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+00000940: da08 3c6d 6f64 756c 653e 0100 0000 730e  ..<module>....s.
+00000950: 0000 000c 0210 0310 1410 0910 0610 0614  ................
+00000960: 06                                       .
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/exceptions/domain.py` & `roboto_sdk-0.1.7/src/roboto_sdk/exceptions/domain.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 
-from ..http import ClientError
+from ..http import HttpError
 
 
 class RobotoDomainException(Exception):
     """
     Expected exceptions from the Roboto domain entity objects.
     """
 
     @staticmethod
-    def from_client_error(error: ClientError):
+    def from_client_error(error: HttpError):
+        if error.status is None:
+            raise RobotoDomainException(error.msg)
         if error.status == 400:
             return RobotoInvalidRequestException(error.msg)
         if error.status in (401, 403):
             return RobotoUnauthorizedException(error.msg)
         if error.status == 404:
             return RobotoNotFoundException(error.msg)
+        if 500 <= error.status < 600:
+            return RobotoServiceError(error.msg)
         raise error
 
 
 class RobotoHttpExceptionParse(object):
     def __enter__(self):
         return self
 
     def __exit__(self, exception_type, exception, traceback):
-        if exception_type is ClientError:
+        if issubclass(type(exception), HttpError):
             raise RobotoDomainException.from_client_error(error=exception)
 
 
 class RobotoUnauthorizedException(RobotoDomainException):
     """
     Thrown when a user is attempting to access a resource that they do not have permission to access
     """
@@ -40,7 +44,13 @@
     """
 
 
 class RobotoInvalidRequestException(RobotoDomainException):
     """
     Thrown when request parameters are in some way invalid
     """
+
+
+class RobotoServiceError(RobotoDomainException):
+    """
+    Thrown when Roboto Service failed in an unexpected way
+    """
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/http/__init__.py` & `roboto_sdk-0.1.7/src/roboto_sdk/http/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/http/__pycache__/__init__.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/http/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 782 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 0e03 0000  o.......1..d....
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 0e03 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6400 6402 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6403 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
 00000060: 6d0a 5a0a 6d0b 5a0b 0100 6400 6404 6c0c  m.Z.m.Z...d.d.l.
 00000070: 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f 0100 6400  m.Z.m.Z.m.Z...d.
@@ -35,16 +35,16 @@
 00000220: 7472 0700 0000 7208 0000 0072 0900 0000  tr....r....r....
 00000230: 720a 0000 005a 1272 6571 7565 7374 5f64  r....Z.request_d
 00000240: 6563 6f72 6174 6f72 7372 0b00 0000 720c  ecoratorsr....r.
 00000250: 0000 0072 0d00 0000 5a0c 7465 7374 696e  ...r....Z.testin
 00000260: 675f 7574 696c 720e 0000 00da 075f 5f61  g_utilr......__a
 00000270: 6c6c 5f5f a900 7213 0000 0072 1300 0000  ll__..r....r....
 00000280: fae5 2f63 6f64 6562 7569 6c64 2f6f 7574  ../codebuild/out
-00000290: 7075 742f 7372 6331 3638 3931 3535 3339  put/src168915539
-000002a0: 392f 7372 632f 636f 6465 7374 6172 2d63  9/src/codestar-c
+00000290: 7075 742f 7372 6333 3537 3831 3132 3139  put/src357811219
+000002a0: 312f 7372 632f 636f 6465 7374 6172 2d63  1/src/codestar-c
 000002b0: 6f6e 6e65 6374 696f 6e73 2e75 732d 7765  onnections.us-we
 000002c0: 7374 2d32 2e61 6d61 7a6f 6e61 7773 2e63  st-2.amazonaws.c
 000002d0: 6f6d 2f67 6974 2d68 7474 702f 3036 3631  om/git-http/0661
 000002e0: 3935 3131 3233 3835 2f75 732d 7765 7374  95112385/us-west
 000002f0: 2d32 2f65 3635 3032 6138 302d 6262 3465  -2/e6502a80-bb4e
 00000300: 2d34 6662 652d 3837 3263 2d35 6434 3263  -4fbe-872c-5d42c
 00000310: 3139 3336 3939 642f 726f 626f 746f 2d61  193699d/roboto-a
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/http/__pycache__/http_client.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/http/__pycache__/http_client.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 9060 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 6423 0000  o.......1..dd#..
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 6423 0000  o..........dd#..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3801 0000 6400  .....@...s8...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6401 6c06 5a07 6400 6401 6c08 5a07 6400  d.l.Z.d.d.l.Z.d.
 00000070: 6401 6c09 5a07 6400 6401 6c0a 5a07 6400  d.l.Z.d.d.l.Z.d.
@@ -42,15 +42,15 @@
 00000290: 0463 6f64 655a 1154 4f4f 5f4d 414e 595f  .codeZ.TOO_MANY_
 000002a0: 5245 5155 4553 5453 5a13 5345 5256 4943  REQUESTSZ.SERVIC
 000002b0: 455f 554e 4156 4149 4c41 424c 45da 0a56  E_UNAVAILABLE..V
 000002c0: 616c 7565 4572 726f 72da 0855 524c 4572  alueError..URLEr
 000002d0: 726f 72da 0373 7472 da06 7265 6173 6f6e  ror..str..reason
 000002e0: 2901 7205 0000 00a9 0072 1300 0000 fae8  ).r......r......
 000002f0: 2f63 6f64 6562 7569 6c64 2f6f 7574 7075  /codebuild/outpu
-00000300: 742f 7372 6331 3638 3931 3535 3339 392f  t/src1689155399/
+00000300: 742f 7372 6333 3537 3831 3132 3139 312f  t/src3578112191/
 00000310: 7372 632f 636f 6465 7374 6172 2d63 6f6e  src/codestar-con
 00000320: 6e65 6374 696f 6e73 2e75 732d 7765 7374  nections.us-west
 00000330: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
 00000340: 2f67 6974 2d68 7474 702f 3036 3631 3935  /git-http/066195
 00000350: 3131 3233 3835 2f75 732d 7765 7374 2d32  112385/us-west-2
 00000360: 2f65 3635 3032 6138 302d 6262 3465 2d34  /e6502a80-bb4e-4
 00000370: 6662 652d 3837 3263 2d35 6434 3263 3139  fbe-872c-5d42c19
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/http/__pycache__/request_decorators.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/http/__pycache__/request_decorators.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 3161 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 590c 0000  o.......1..dY...
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 590c 0000  o..........dY...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 6400 6403 6c04  ..d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6406  ..d.d.l.m.Z...d.
 00000070: 6407 6c0a 6d0b 5a0b 0100 6406 6408 6c0c  d.l.m.Z...d.d.l.
@@ -33,16 +33,16 @@
 00000200: 7574 6844 6563 6f72 6174 6f72 5f5f 7573  uthDecorator__us
 00000210: 6572 5f69 64da 0775 7365 725f 6964 6302  er_id..user_idc.
 00000220: 0000 0000 0000 0000 0000 0002 0000 0002  ................
 00000230: 0000 0043 0000 00f3 0a00 0000 7c01 7c00  ...C........|.|.
 00000240: 5f00 6400 5300 a901 4e29 0172 0e00 0000  _.d.S...N).r....
 00000250: 2902 da04 7365 6c66 720f 0000 00a9 0072  )...selfr......r
 00000260: 1300 0000 faef 2f63 6f64 6562 7569 6c64  ....../codebuild
-00000270: 2f6f 7574 7075 742f 7372 6331 3638 3931  /output/src16891
-00000280: 3535 3339 392f 7372 632f 636f 6465 7374  55399/src/codest
+00000270: 2f6f 7574 7075 742f 7372 6333 3537 3831  /output/src35781
+00000280: 3132 3139 312f 7372 632f 636f 6465 7374  12191/src/codest
 00000290: 6172 2d63 6f6e 6e65 6374 696f 6e73 2e75  ar-connections.u
 000002a0: 732d 7765 7374 2d32 2e61 6d61 7a6f 6e61  s-west-2.amazona
 000002b0: 7773 2e63 6f6d 2f67 6974 2d68 7474 702f  ws.com/git-http/
 000002c0: 3036 3631 3935 3131 3233 3835 2f75 732d  066195112385/us-
 000002d0: 7765 7374 2d32 2f65 3635 3032 6138 302d  west-2/e6502a80-
 000002e0: 6262 3465 2d34 6662 652d 3837 3263 2d35  bb4e-4fbe-872c-5
 000002f0: 6434 3263 3139 3336 3939 642f 726f 626f  d42c193699d/robo
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/http/__pycache__/testing_util.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/http/__pycache__/testing_util.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 1004 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 ec03 0000  o.......1..d....
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 ec03 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a03 6400 6401 6c04 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c05 5a05 6402 6403 6c06 6d07 5a07  d.l.Z.d.d.l.m.Z.
 00000060: 0100 4700 6404 6405 8400 6405 8302 5a08  ..G.d.d...d...Z.
 00000070: 6401 5300 2906 e900 0000 004e e901 0000  d.S.)......N....
@@ -36,16 +36,16 @@
 00000230: 5f00 7c04 7007 7401 8300 7c00 5f02 7c02  _.|.p.t...|._.|.
 00000240: 7c00 5f03 7c01 7c00 5f04 6400 5300 a901  |._.|.|._.d.S...
 00000250: 4e29 0572 0700 0000 da04 6469 6374 7205  N).r......dictr.
 00000260: 0000 0072 0600 0000 7208 0000 0029 05da  ...r....r....)..
 00000270: 0473 656c 6672 0a00 0000 720b 0000 0072  .selfr....r....r
 00000280: 0c00 0000 720d 0000 00a9 0072 1200 0000  ....r......r....
 00000290: fae9 2f63 6f64 6562 7569 6c64 2f6f 7574  ../codebuild/out
-000002a0: 7075 742f 7372 6331 3638 3931 3535 3339  put/src168915539
-000002b0: 392f 7372 632f 636f 6465 7374 6172 2d63  9/src/codestar-c
+000002a0: 7075 742f 7372 6333 3537 3831 3132 3139  put/src357811219
+000002b0: 312f 7372 632f 636f 6465 7374 6172 2d63  1/src/codestar-c
 000002c0: 6f6e 6e65 6374 696f 6e73 2e75 732d 7765  onnections.us-we
 000002d0: 7374 2d32 2e61 6d61 7a6f 6e61 7773 2e63  st-2.amazonaws.c
 000002e0: 6f6d 2f67 6974 2d68 7474 702f 3036 3631  om/git-http/0661
 000002f0: 3935 3131 3233 3835 2f75 732d 7765 7374  95112385/us-west
 00000300: 2d32 2f65 3635 3032 6138 302d 6262 3465  -2/e6502a80-bb4e
 00000310: 2d34 6662 652d 3837 3263 2d35 6434 3263  -4fbe-872c-5d42c
 00000320: 3139 3336 3939 642f 726f 626f 746f 2d61  193699d/roboto-a
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/http/http_client.py` & `roboto_sdk-0.1.7/src/roboto_sdk/http/http_client.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/http/request_decorators.py` & `roboto_sdk-0.1.7/src/roboto_sdk/http/request_decorators.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/http/testing_util.py` & `roboto_sdk-0.1.7/src/roboto_sdk/http/testing_util.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/profile/__pycache__/profile.cpython-310.pyc` & `roboto_sdk-0.1.7/src/roboto_sdk/profile/__pycache__/profile.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul  7 04:18:57 2023 UTC, .py size: 2977 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3192 a764 a10b 0000  o.......1..d....
+00000000: 6f0d 0d0a 0000 0000 e2a1 a964 a10b 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 b400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c04 6d05 5a05 6d06 5a06 0100 6400  d.l.m.Z.m.Z...d.
 00000060: 6401 6c07 5a07 6403 6404 6c08 6d09 5a09  d.l.Z.d.d.l.m.Z.
 00000070: 0100 6509 8300 5a0a 6405 5a0b 6406 5a0c  ..e...Z.d.Z.d.Z.
@@ -35,16 +35,16 @@
 00000220: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
 00000230: 5f5f da03 7374 72da 0f5f 5f61 6e6e 6f74  __..str..__annot
 00000240: 6174 696f 6e73 5f5f da0d 5052 4f44 5f45  ations__..PROD_E
 00000250: 4e44 504f 494e 5472 0a00 0000 da18 5052  NDPOINTr......PR
 00000260: 4f44 5f55 5345 525f 504f 4f4c 5f43 4c49  OD_USER_POOL_CLI
 00000270: 454e 545f 4944 720b 0000 00a9 0072 1300  ENT_IDr......r..
 00000280: 0000 7213 0000 00fa e72f 636f 6465 6275  ..r....../codebu
-00000290: 696c 642f 6f75 7470 7574 2f73 7263 3136  ild/output/src16
-000002a0: 3839 3135 3533 3939 2f73 7263 2f63 6f64  89155399/src/cod
+00000290: 696c 642f 6f75 7470 7574 2f73 7263 3335  ild/output/src35
+000002a0: 3738 3131 3231 3931 2f73 7263 2f63 6f64  78112191/src/cod
 000002b0: 6573 7461 722d 636f 6e6e 6563 7469 6f6e  estar-connection
 000002c0: 732e 7573 2d77 6573 742d 322e 616d 617a  s.us-west-2.amaz
 000002d0: 6f6e 6177 732e 636f 6d2f 6769 742d 6874  onaws.com/git-ht
 000002e0: 7470 2f30 3636 3139 3531 3132 3338 352f  tp/066195112385/
 000002f0: 7573 2d77 6573 742d 322f 6536 3530 3261  us-west-2/e6502a
 00000300: 3830 2d62 6234 652d 3466 6265 2d38 3732  80-bb4e-4fbe-872
 00000310: 632d 3564 3432 6331 3933 3639 3964 2f72  c-5d42c193699d/r
```

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/profile/profile.py` & `roboto_sdk-0.1.7/src/roboto_sdk/profile/profile.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/src/roboto_sdk/serde.py` & `roboto_sdk-0.1.7/src/roboto_sdk/serde.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.6/PKG-INFO` & `roboto_sdk-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboto-sdk
-Version: 0.1.6
+Version: 0.1.7
 Summary: Tools for interacting with roboto.ai
 License: MIT
 Author: Roboto
 Author-email: admin@roboto.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

