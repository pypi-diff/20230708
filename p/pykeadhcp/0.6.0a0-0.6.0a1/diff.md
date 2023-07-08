# Comparing `tmp/pykeadhcp-0.6.0a0.tar.gz` & `tmp/pykeadhcp-0.6.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykeadhcp-0.6.0a0.tar", max compression
+gzip compressed data, was "pykeadhcp-0.6.0a1.tar", max compression
```

## Comparing `pykeadhcp-0.6.0a0.tar` & `pykeadhcp-0.6.0a1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0    11356 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/LICENSE
--rw-r--r--   0        0        0     8001 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/README.md
--rw-r--r--   0        0        0       30 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/__init__.py
--rw-r--r--   0        0        0      174 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/daemons/__init__.py
--rw-r--r--   0        0        0     4508 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/daemons/ctrlagent.py
--rw-r--r--   0        0        0     4526 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/daemons/ddns.py
--rw-r--r--   0        0        0    46982 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/daemons/dhcp4.py
--rw-r--r--   0        0        0    22336 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/daemons/dhcp6.py
--rw-r--r--   0        0        0     3865 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/exceptions.py
--rw-r--r--   0        0        0    10415 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/kea.py
--rw-r--r--   0        0        0        0 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/ctrlagent/__init__.py
--rw-r--r--   0        0        0      457 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/ctrlagent/config.py
--rw-r--r--   0        0        0        0 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp4/__init__.py
--rw-r--r--   0        0        0      331 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp4/client_class.py
--rw-r--r--   0        0        0      798 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp4/config.py
--rw-r--r--   0        0        0      212 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp4/lease.py
--rw-r--r--   0        0        0      303 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp4/reservation.py
--rw-r--r--   0        0        0      453 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp4/shared_network.py
--rw-r--r--   0        0        0      684 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp4/subnet.py
--rw-r--r--   0        0        0        0 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp6/__init__.py
--rw-r--r--   0        0        0      253 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp6/client_class.py
--rw-r--r--   0        0        0      922 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp6/config.py
--rw-r--r--   0        0        0      346 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp6/lease.py
--rw-r--r--   0        0        0      438 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp6/pd_pool.py
--rw-r--r--   0        0        0      212 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp6/reservation.py
--rw-r--r--   0        0        0      296 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp6/server_id.py
--rw-r--r--   0        0        0      380 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp6/shared_network.py
--rw-r--r--   0        0        0      501 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp6/subnet.py
--rw-r--r--   0        0        0     1638 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/enums.py
--rw-r--r--   0        0        0      169 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/__init__.py
--rw-r--r--   0        0        0      181 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/api_response.py
--rw-r--r--   0        0        0      477 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/authentication.py
--rw-r--r--   0        0        0      435 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/base.py
--rw-r--r--   0        0        0      415 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/client_class.py
--rw-r--r--   0        0        0     1394 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/config.py
--rw-r--r--   0        0        0      396 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/control_socket.py
--rw-r--r--   0        0        0     2458 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/daemon.py
--rw-r--r--   0        0        0      734 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/database.py
--rw-r--r--   0        0        0      399 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/dhcp_common.py
--rw-r--r--   0        0        0      873 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/dhcp_ddns.py
--rw-r--r--   0        0        0      158 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/dhcp_queue_control.py
--rw-r--r--   0        0        0      183 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/hook.py
--rw-r--r--   0        0        0      403 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/lease.py
--rw-r--r--   0        0        0      558 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/logger.py
--rw-r--r--   0        0        0      181 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/multi_threading.py
--rw-r--r--   0        0        0      259 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/option_data.py
--rw-r--r--   0        0        0      294 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/option_def.py
--rw-r--r--   0        0        0      306 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/pool.py
--rw-r--r--   0        0        0      141 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/relay.py
--rw-r--r--   0        0        0      302 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/remote_map.py
--rw-r--r--   0        0        0      217 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/remote_server.py
--rw-r--r--   0        0        0      436 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/reservation.py
--rw-r--r--   0        0        0      112 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/sanity_check.py
--rw-r--r--   0        0        0      175 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/shared_network.py
--rw-r--r--   0        0        0      249 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/sockets.py
--rw-r--r--   0        0        0      477 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/status.py
--rw-r--r--   0        0        0      390 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/subnet.py
--rw-r--r--   0        0        0      152 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/parsers/__init__.py
--rw-r--r--   0        0        0      508 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/parsers/ctrlagent.py
--rw-r--r--   0        0        0        0 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/parsers/ddns.py
--rw-r--r--   0        0        0    17838 2023-07-08 01:36:06.870582 pykeadhcp-0.6.0a0/pykeadhcp/parsers/dhcp4.py
--rw-r--r--   0        0        0    20361 2023-07-08 01:36:06.870582 pykeadhcp-0.6.0a0/pykeadhcp/parsers/dhcp6.py
--rw-r--r--   0        0        0     3436 2023-07-08 01:36:06.870582 pykeadhcp-0.6.0a0/pykeadhcp/parsers/exceptions.py
--rw-r--r--   0        0        0      825 2023-07-08 01:36:06.870582 pykeadhcp-0.6.0a0/pykeadhcp/parsers/generic.py
--rw-r--r--   0        0        0      449 2023-07-08 01:36:06.870582 pykeadhcp-0.6.0a0/pyproject.toml
--rw-r--r--   0        0        0     8608 1970-01-01 00:00:00.000000 pykeadhcp-0.6.0a0/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-07-08 15:09:04.227639 pykeadhcp-0.6.0a1/LICENSE
+-rw-r--r--   0        0        0     8001 2023-07-08 15:09:04.227639 pykeadhcp-0.6.0a1/README.md
+-rw-r--r--   0        0        0       30 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/__init__.py
+-rw-r--r--   0        0        0      174 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/daemons/__init__.py
+-rw-r--r--   0        0        0     4508 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/daemons/ctrlagent.py
+-rw-r--r--   0        0        0     4526 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/daemons/ddns.py
+-rw-r--r--   0        0        0    70245 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/daemons/dhcp4.py
+-rw-r--r--   0        0        0    69516 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/daemons/dhcp6.py
+-rw-r--r--   0        0        0     4068 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/exceptions.py
+-rw-r--r--   0        0        0    10415 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/kea.py
+-rw-r--r--   0        0        0        0 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/ctrlagent/__init__.py
+-rw-r--r--   0        0        0      457 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/ctrlagent/config.py
+-rw-r--r--   0        0        0        0 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/dhcp4/__init__.py
+-rw-r--r--   0        0        0      331 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/dhcp4/client_class.py
+-rw-r--r--   0        0        0      798 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/dhcp4/config.py
+-rw-r--r--   0        0        0      212 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/dhcp4/lease.py
+-rw-r--r--   0        0        0      303 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/dhcp4/reservation.py
+-rw-r--r--   0        0        0      453 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/dhcp4/shared_network.py
+-rw-r--r--   0        0        0      684 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/dhcp4/subnet.py
+-rw-r--r--   0        0        0        0 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/dhcp6/__init__.py
+-rw-r--r--   0        0        0      253 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/dhcp6/client_class.py
+-rw-r--r--   0        0        0      922 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/dhcp6/config.py
+-rw-r--r--   0        0        0      346 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/dhcp6/lease.py
+-rw-r--r--   0        0        0      438 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/dhcp6/pd_pool.py
+-rw-r--r--   0        0        0      212 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/dhcp6/reservation.py
+-rw-r--r--   0        0        0      296 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/dhcp6/server_id.py
+-rw-r--r--   0        0        0      380 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/dhcp6/shared_network.py
+-rw-r--r--   0        0        0      501 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/dhcp6/subnet.py
+-rw-r--r--   0        0        0     1638 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/enums.py
+-rw-r--r--   0        0        0      169 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/generic/__init__.py
+-rw-r--r--   0        0        0      181 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/generic/api_response.py
+-rw-r--r--   0        0        0      477 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/generic/authentication.py
+-rw-r--r--   0        0        0      435 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/generic/base.py
+-rw-r--r--   0        0        0      415 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/generic/client_class.py
+-rw-r--r--   0        0        0     1394 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/generic/config.py
+-rw-r--r--   0        0        0      396 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/generic/control_socket.py
+-rw-r--r--   0        0        0     2458 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/generic/daemon.py
+-rw-r--r--   0        0        0      734 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/generic/database.py
+-rw-r--r--   0        0        0      399 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/generic/dhcp_common.py
+-rw-r--r--   0        0        0      873 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/generic/dhcp_ddns.py
+-rw-r--r--   0        0        0      158 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/generic/dhcp_queue_control.py
+-rw-r--r--   0        0        0      183 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/generic/hook.py
+-rw-r--r--   0        0        0      403 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/generic/lease.py
+-rw-r--r--   0        0        0      558 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/generic/logger.py
+-rw-r--r--   0        0        0      181 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/generic/multi_threading.py
+-rw-r--r--   0        0        0      259 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/generic/option_data.py
+-rw-r--r--   0        0        0      294 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/generic/option_def.py
+-rw-r--r--   0        0        0      306 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/generic/pool.py
+-rw-r--r--   0        0        0      141 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/generic/relay.py
+-rw-r--r--   0        0        0      302 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/generic/remote_map.py
+-rw-r--r--   0        0        0      217 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/generic/remote_server.py
+-rw-r--r--   0        0        0      436 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/generic/reservation.py
+-rw-r--r--   0        0        0      112 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/generic/sanity_check.py
+-rw-r--r--   0        0        0      175 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/generic/shared_network.py
+-rw-r--r--   0        0        0      249 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/generic/sockets.py
+-rw-r--r--   0        0        0      477 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/generic/status.py
+-rw-r--r--   0        0        0      390 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/models/generic/subnet.py
+-rw-r--r--   0        0        0      152 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/parsers/__init__.py
+-rw-r--r--   0        0        0      508 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/parsers/ctrlagent.py
+-rw-r--r--   0        0        0        0 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/parsers/ddns.py
+-rw-r--r--   0        0        0    17838 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/parsers/dhcp4.py
+-rw-r--r--   0        0        0    20361 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/parsers/dhcp6.py
+-rw-r--r--   0        0        0     3436 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/parsers/exceptions.py
+-rw-r--r--   0        0        0      825 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pykeadhcp/parsers/generic.py
+-rw-r--r--   0        0        0      449 2023-07-08 15:09:04.231640 pykeadhcp-0.6.0a1/pyproject.toml
+-rw-r--r--   0        0        0     8608 1970-01-01 00:00:00.000000 pykeadhcp-0.6.0a1/PKG-INFO
```

### Comparing `pykeadhcp-0.6.0a0/LICENSE` & `pykeadhcp-0.6.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.6.0a0/README.md` & `pykeadhcp-0.6.0a1/README.md`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.6.0a0/pykeadhcp/daemons/ctrlagent.py` & `pykeadhcp-0.6.0a1/pykeadhcp/daemons/ctrlagent.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.6.0a0/pykeadhcp/daemons/ddns.py` & `pykeadhcp-0.6.0a1/pykeadhcp/daemons/ddns.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.6.0a0/pykeadhcp/daemons/dhcp4.py` & `pykeadhcp-0.6.0a1/pykeadhcp/daemons/dhcp4.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 from typing import TYPE_CHECKING, List, Dict
 
 if TYPE_CHECKING:
     from pykeadhcp import Kea
 
 from pykeadhcp.models.generic import KeaResponse, StatusGet
 from pykeadhcp.models.generic.remote_server import RemoteServer
+from pykeadhcp.models.generic.option_def import OptionDef
+from pykeadhcp.models.generic.option_data import OptionData
 from pykeadhcp.models.dhcp4.shared_network import SharedNetwork4
 from pykeadhcp.models.dhcp4.subnet import Subnet4
 from pykeadhcp.models.dhcp4.lease import Lease4, Lease4Page
 from pykeadhcp.models.dhcp4.reservation import Reservation4
+from pykeadhcp.models.dhcp4.client_class import ClientClass4
 from pykeadhcp.models.enums import HostReservationIdentifierEnum
 from pykeadhcp.exceptions import (
     KeaException,
     KeaSharedNetworkNotFoundException,
     KeaSubnetNotFoundException,
     KeaLeaseNotFoundException,
     KeaRemoteServerNotFoundException,
     KeaConfigBackendNotConfiguredException,
     KeaUnknownHostReservationTypeException,
     KeaReservationNotFoundException,
+    KeaClientClassNotFoundException,
 )
 
 
 class Dhcp4:
     def __init__(self, api: "Kea"):
         self.service = "dhcp4"
         self.api = api
@@ -58,14 +62,108 @@
         """Returns list of compilation options that this particular binary was built with
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#ref-build-report
         """
         return self.api.send_command(command="build-report", service=self.service)
 
+    def class_add(self, client_class: ClientClass4) -> KeaResponse:
+        """Adds a new class to the existing server configuration
+
+        Args:
+            client_class:       ClientClass4 Object
+
+        Kea API Reference:
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#class-add
+        """
+        return self.api.send_command_with_arguments(
+            command="class-add",
+            service=self.service,
+            arguments={
+                "client-classes": [
+                    client_class.dict(
+                        exclude_none=True, exclude_unset=True, by_alias=True
+                    )
+                ]
+            },
+            required_hook="class_cmds",
+        )
+
+    def class_del(self, name: str) -> KeaResponse:
+        """Removes a client class from the server configuration
+
+        Args:
+            name:   Name of Class
+
+        Kea API Reference:
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#class-del
+        """
+        return self.api.send_command_with_arguments(
+            command="class-del",
+            service=self.service,
+            arguments={"name": name},
+            required_hook="class_cmds",
+        )
+
+    def class_get(self, name: str) -> ClientClass4:
+        """Returns detailed information about an existing client class
+
+        Args:
+            name:   Name of Class
+
+        Kea API Reference:
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#class-get
+        """
+        data = self.api.send_command_with_arguments(
+            command="class-get",
+            service=self.service,
+            arguments={"name": name},
+            required_hook="class_cmds",
+        )
+
+        if data.result == 3:
+            raise KeaClientClassNotFoundException(client_class=name)
+
+        if not data.arguments.get("client-classes"):
+            return None
+
+        client_class = data.arguments["client-classes"][0]
+        return ClientClass4.parse_obj(client_class)
+
+    def class_list(self) -> List[ClientClass4]:
+        """Retrieves a list of all client classes from server configuration
+
+        Kea API Reference:
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#class-list
+        """
+        data = self.api.send_command(
+            command="class-list", service=self.service, required_hook="class_cmds"
+        )
+
+        client_classes = data.arguments.get("client-classes")
+        return [ClientClass4.parse_obj(client_class) for client_class in client_classes]
+
+    def class_update(self, client_class: ClientClass4) -> KeaResponse:
+        """Updates an existing client class in the server configuration
+
+        Kea API Reference:
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#class-update
+        """
+        return self.api.send_command_with_arguments(
+            command="class-update",
+            service=self.service,
+            arguments={
+                "client-classes": [
+                    client_class.dict(
+                        exclude_none=True, exclude_unset=True, by_alias=True
+                    )
+                ]
+            },
+        )
+
     def config_backend_pull(self) -> KeaResponse:
         """Forces an immediate update of the servers using the configuration database
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#config-backend-pull
         """
         data = self.api.send_command(
@@ -555,14 +653,555 @@
         return self.api.send_command_with_arguments(
             command="network4-subnet-del",
             service=self.service,
             arguments={"name": name, "id": subnet_id},
             required_hook="subnet_cmds",
         )
 
+    def remote_class4_del(self, name: str, remote_map: dict = {}) -> KeaResponse:
+        """Deletes a DHCPv4 client class from the configuration database
+
+        Args:
+            name:       Name of the client class
+            remote_map: (remote_type, remote_host or remote_port) to select a specific remote database
+
+        Kea API Reference:
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#remote-class4-del
+        """
+        return self.api.send_command_remote(
+            command="remote-class4-del",
+            service=self.service,
+            arguments={"client-classes": [{"name": name}]},
+            remote_map=remote_map,
+        )
+
+    def remote_class4_get(self, name: str, remote_map: dict = {}) -> ClientClass4:
+        """Gets a DHCPv4 client class from the configuration database
+
+        Args:
+            name:       Name of the client class
+            remote_map: (remote_type, remote_host or remote_port) to select a specific remote database
+
+        Kea API Reference:
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#remote-class4-get
+        """
+        data = self.api.send_command_remote(
+            command="remote-class4-get",
+            service=self.service,
+            arguments={"client-classes": [{"name": name}]},
+            remote_map=remote_map,
+        )
+
+        if data.result == 3:
+            raise KeaClientClassNotFoundException(client_class=name)
+
+        if not data.arguments.get("client-classes"):
+            return None
+
+        client_class = data.arguments["client-classes"][0]
+        return ClientClass4.parse_obj(client_class)
+
+    def remote_class4_get_all(
+        self, server_tags: List[str] = ["all"], remote_map: dict = {}
+    ) -> ClientClass4:
+        """Gets all DHCPv4 client classes from the configuration database
+
+        Args:
+            server_tags:    List of Server Tags
+            remote_map:     (remote_type, remote_host or remote_port) to select a specific remote database
+
+        Kea API Reference:
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#remote-class4-get-all
+        """
+        data = self.api.send_command_remote(
+            command="remote-class4-get-all",
+            service=self.service,
+            arguments={"server-tags": server_tags},
+            remote_map=remote_map,
+        )
+
+        client_classes = data.arguments.get("client-classes")
+        return [ClientClass4.parse_obj(client_class) for client_class in client_classes]
+
+    def remote_class4_set(
+        self,
+        client_class: ClientClass4,
+        server_tags: List[str] = ["all"],
+        follow_class_name: str = None,
+        remote_map: dict = {},
+    ) -> KeaResponse:
+        """Creates/Replaces a DHCPv4 Client Class in the configuration database
+
+        Args:
+            client_class:       ClientClass4 Object
+            follow_class_name:  Places client class after existing class in the hierarchy
+            remote_map:         (remote_type, remote_host or remote_port) to select a specific remote database
+
+        Kea API Reference:
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#remote-class4-set
+        """
+        data = client_class.dict(exclude_none=True, exclude_unset=True, by_alias=True)
+        if follow_class_name:
+            data["follow-class-name"] = follow_class_name
+
+        return self.api.send_command_remote(
+            command="remote-class4-set",
+            service=self.service,
+            arguments={"client-classes": [data], "server-tags": server_tags},
+            remote_map=remote_map,
+        )
+
+    def remote_global_parameter4_del(
+        self, parameter: str, server_tag: str, remote_map: dict = {}
+    ) -> KeaResponse:
+        """Deletes a global DHCPv4 parameter from the configuration database
+
+        Args:
+            parameter:      Parameter to delete
+            server_tag:     Single Server Tag
+            remote_map:     (remote_type, remote_host or remote_port) to select a specific remote database
+
+        Kea API Reference:
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#remote-global-parameter4-del
+        """
+        return self.api.send_command_remote(
+            command="remote-global-parameter4-del",
+            service=self.service,
+            arguments={"parameters": [parameter], "server-tags": [server_tag]},
+            remote_map=remote_map,
+        )
+
+    def remote_global_parameter4_get(
+        self, parameter: str, server_tag: str, remote_map: dict = {}
+    ) -> KeaResponse:
+        """Get a specific global parameter from the configuration database
+
+        Args:
+            parameter:      Parameter to delete
+            server_tag:     Single Server Tag
+            remote_map:     (remote_type, remote_host or remote_port) to select a specific remote database
+
+        Kea API Reference:
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#remote-global-parameter4-get
+        """
+        return self.api.send_command_remote(
+            command="remote-global-parameter4-get",
+            service=self.service,
+            arguments={"parameters": [parameter], "server-tags": [server_tag]},
+            remote_map=remote_map,
+        )
+
+    def remote_global_parameter4_get_all(
+        self, server_tag: str, remote_map: dict = {}
+    ) -> KeaResponse:
+        """Gets all global parameter from the configuration database
+
+        Args:
+            server_tag:     Single Server Tag
+            remote_map:     (remote_type, remote_host or remote_port) to select a specific remote database
+
+        Kea API Reference:
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#remote-global-parameter4-get-all
+        """
+        return self.api.send_command_remote(
+            command="remote-global-parameter4-get-all",
+            service=self.service,
+            arguments={"server-tags": [server_tag]},
+            remote_map=remote_map,
+        )
+
+    def remote_global_parameter4_set(
+        self, parameters: dict, server_tag: str, remote_map: dict = {}
+    ) -> KeaResponse:
+        """Creates/Updates one or more global parameters in the configuration database
+
+        Args:
+            parameters:     Dictionary of parameters (key) and their config (values)
+            server_tag:     Single Server Tag
+            remote_map:     (remote_type, remote_host or remote_port) to select a specific remote database
+
+        Kea API Reference:
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#remote-global-parameter4-set
+        """
+        return self.api.send_command_remote(
+            command="remote-global-parameter4-set",
+            service=self.service,
+            arguments={"parameters": parameters, "server-tags": [server_tag]},
+            remote_map=remote_map,
+        )
+
+    def remote_option_def4_del(
+        self,
+        option_code: int,
+        option_space: str,
+        server_tag: str,
+        remote_map: dict = {},
+    ) -> KeaResponse:
+        """Delete a DHCPv4 option defined in the configuration database
+
+        Args:
+            option_code:    Option Code
+            option_space:   Option Space
+            server_tag:     Single Server Tag
+            remote_map:     (remote_type, remote_host or remote_port) to select a specific remote database
+
+        Kea API Reference:
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#remote-option-def4-del
+        """
+        return self.api.send_command_remote(
+            command="remote-option-def4-del",
+            service=self.service,
+            arguments={
+                "option-defs": [{"code": option_code, "space": option_space}],
+                "server-tags": [server_tag],
+            },
+            remote_map=remote_map,
+        )
+
+    def remote_option_def4_get(
+        self,
+        option_code: int,
+        option_space: str,
+        server_tag: str,
+        remote_map: dict = {},
+    ) -> KeaResponse:
+        """Delete a DHCPv4 option defined in the configuration database
+
+        Args:
+            option_code:    Option Code
+            option_space:   Option Space
+            server_tag:     Single Server Tag
+            remote_map:     (remote_type, remote_host or remote_port) to select a specific remote database
+
+        Kea API Reference:
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#remote-option-def4-get
+        """
+        return self.api.send_command_remote(
+            command="remote-option-def4-get",
+            service=self.service,
+            arguments={
+                "option-defs": [{"code": option_code, "space": option_space}],
+                "server-tags": [server_tag],
+            },
+            remote_map=remote_map,
+        )
+
+    def remote_option_def4_get_all(self, server_tag: str, remote_map: dict = {}):
+        """Fetches all Dhcpv4 option defs from the configuration database
+
+        Args:
+            server_tag:     Single Server Tag
+            remote_map:     (remote_type, remote_host or remote_port) to select a specific remote database
+
+        Kea API Reference:
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#remote-option-def4-get-all
+        """
+        return self.api.send_command_remote(
+            command="remote-option-def4-get-all",
+            service=self.service,
+            arguments={"server-tags": [server_tag]},
+            remote_map=remote_map,
+        )
+
+    def remote_option_def4_set(
+        self,
+        option_def: OptionDef,
+        server_tag: str,
+        remote_map: dict = {},
+    ) -> KeaResponse:
+        """Creates/Delete a DHCPv4 option defined in the configuration database
+
+        Args:
+            option_def:     OptionDef Object
+            server_tag:     Single Server Tag
+            remote_map:     (remote_type, remote_host or remote_port) to select a specific remote database
+
+        Kea API Reference:
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#remote-option-def4-set
+        """
+        return self.api.send_command_remote(
+            command="remote-option-def4-set",
+            service=self.service,
+            arguments={
+                "option-defs": [
+                    option_def.dict(
+                        exclude_none=True, exclude_unset=True, by_alias=True
+                    )
+                ],
+                "server-tags": [server_tag],
+            },
+            remote_map=remote_map,
+        )
+
+    def remote_option4_global_del(
+        self,
+        option_code: int,
+        option_space: str,
+        server_tag: str,
+        remote_map: dict = {},
+    ) -> KeaResponse:
+        """Delete a DHCPv4 global option defined in the configuration database
+
+        Args:
+            option_code:    Option Code
+            option_space:   Option Space
+            server_tag:     Single Server Tag
+            remote_map:     (remote_type, remote_host or remote_port) to select a specific remote database
+
+        Kea API Reference:
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#remote-option4-global-del
+        """
+        return self.api.send_command_remote(
+            command="remote-option4-global-del",
+            service=self.service,
+            arguments={
+                "options": [{"code": option_code, "space": option_space}],
+                "server-tags": [server_tag],
+            },
+            remote_map=remote_map,
+        )
+
+    def remote_option4_global_get(
+        self,
+        option_code: int,
+        option_space: str,
+        server_tag: str,
+        remote_map: dict = {},
+    ) -> KeaResponse:
+        """Gets a DHCPv4 global option defined in the configuration database
+
+        Args:
+            option_code:    Option Code
+            option_space:   Option Space
+            server_tag:     Single Server Tag
+            remote_map:     (remote_type, remote_host or remote_port) to select a specific remote database
+
+        Kea API Reference:
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#remote-option4-global-get
+        """
+        return self.api.send_command_remote(
+            command="remote-option4-global-get",
+            service=self.service,
+            arguments={
+                "options": [{"code": option_code, "space": option_space}],
+                "server-tags": [server_tag],
+            },
+            remote_map=remote_map,
+        )
+
+    def remote_option4_global_get_all(
+        self,
+        server_tag: str,
+        remote_map: dict = {},
+    ) -> KeaResponse:
+        """Gets all DHCPv4 global option defined in the configuration database
+
+        Args:
+            server_tag:     Single Server Tag
+            remote_map:     (remote_type, remote_host or remote_port) to select a specific remote database
+
+        Kea API Reference:
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#remote-option4-global-get-all
+        """
+        return self.api.send_command_remote(
+            command="remote-option4-global-get-all",
+            service=self.service,
+            arguments={
+                "server-tags": [server_tag],
+            },
+            remote_map=remote_map,
+        )
+
+    def remote_option4_global_set(
+        self,
+        option_data: OptionData,
+        server_tag: str,
+        remote_map: dict = {},
+    ) -> KeaResponse:
+        """Creates/Replaces a DHCPv4 option defined in the configuration database
+
+        Args:
+            option_data:    OptionData Object
+            server_tag:     Single Server Tag
+            remote_map:     (remote_type, remote_host or remote_port) to select a specific remote database
+
+        Kea API Reference:
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#remote-option4-global-set
+        """
+        return self.api.send_command_remote(
+            command="remote-option4-global-set",
+            service=self.service,
+            arguments={
+                "options": [
+                    option_data.dict(
+                        exclude_none=True, exclude_unset=True, by_alias=True
+                    )
+                ],
+                "server-tags": [server_tag],
+            },
+            remote_map=remote_map,
+        )
+
+    def remote_option4_network_del(
+        self,
+        shared_network: str,
+        option_code: int,
+        option_space: str,
+        remote_map: dict = {},
+    ) -> KeaResponse:
+        """Delete a DHCPv4 option from a shared network in the configuration database
+
+        Args:
+            shared_network:     Name of shared network
+            option_code:        Option Code
+            option_space:       Option Space
+            remote_map:     (remote_type, remote_host or remote_port) to select a specific remote database
+
+        Kea API Reference:
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#remote-option4-network-del
+        """
+        return self.api.send_command_remote(
+            command="remote-option4-network-del",
+            service=self.service,
+            arguments={
+                "shared-networks": [{"name": shared_network}],
+                "options": [{"code": option_code, "space": option_space}],
+            },
+            remote_map=remote_map,
+        )
+
+    def remote_option4_network_set(
+        self,
+        shared_network: str,
+        option_data: OptionData,
+        remote_map: dict = {},
+    ) -> KeaResponse:
+        """Delete a DHCPv4 option from a shared network in the configuration database
+
+        Args:
+            shared_network:     Name of shared network
+            option_data:        OptionData Object
+            remote_map:     (remote_type, remote_host or remote_port) to select a specific remote database
+
+        Kea API Reference:
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#remote-option4-network-set
+        """
+        return self.api.send_command_remote(
+            command="remote-option4-network-set",
+            service=self.service,
+            arguments={
+                "shared-networks": [{"name": shared_network}],
+                "options": [
+                    option_data.dict(
+                        exclude_none=True, exclude_unset=True, by_alias=True
+                    )
+                ],
+            },
+            remote_map=remote_map,
+        )
+
+    def remote_option4_pool_del(
+        self, pool: str, option_code: int, option_space: str, remote_map: dict = {}
+    ) -> KeaResponse:
+        """Deletes a DHCPv4 option from an address pool in the configuration database
+
+        Args:
+            pool:           Pool Range
+            option_code:    Option Code
+            option_space:   Option Space
+            remote_map:     (remote_type, remote_host or remote_port) to select a specific remote database
+
+        Kea API Reference:
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#remote-option4-pool-del
+        """
+        return self.api.send_command_remote(
+            command="remote-option4-pool-del",
+            service=self.service,
+            arguments={
+                "pools": [{"pool": pool}],
+                "options": [{"code": option_code, "space": option_space}],
+            },
+            remote_map=remote_map,
+        )
+
+    def remote_option4_pool_set(
+        self, pool: str, option_data: OptionData, remote_map: dict = {}
+    ) -> KeaResponse:
+        """Creates/Replaces a DHCPv4 option in an address pool in the configuration database
+
+        Args:
+            pool:           Pool Range
+            option_data:    OptionData Object
+            remote_map:     (remote_type, remote_host or remote_port) to select a specific remote database
+
+        Kea API Reference:
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#remote-option4-pool-set
+        """
+        return self.api.send_command_remote(
+            command="remote-option4-pool-set",
+            service=self.service,
+            arguments={
+                "pools": [{"pool": pool}],
+                "options": [
+                    option_data.dict(
+                        exclude_none=True, exclude_unset=True, by_alias=True
+                    )
+                ],
+            },
+            remote_map=remote_map,
+        )
+
+    def remote_option4_subnet_del(
+        self, subnet_id: int, option_code: int, option_space: str, remote_map: dict = {}
+    ) -> KeaResponse:
+        """Deletes a DHCPv4 option from a subnet in the configuration database
+
+        Args:
+            subnet_id:      Subnet ID
+            option_code:    Option Code
+            option_space:   Option Space
+            remote_map:     (remote_type, remote_host or remote_port) to select a specific remote database
+
+        Kea API Reference:
+            https://kea.readthedocs.io/en/kea-2.2.0/api.html#remote-option4-subnet-del
+        """
+        return self.api.send_command_remote(
+            command="remote-option4-subnet-del",
+            service=self.service,
+            arguments={
+                "subnets": [{"id": subnet_id}],
+                "options": [{"code": option_code, "space": option_space}],
+            },
+            remote_map=remote_map,
+        )
+
+    def remote_option4_subnet_set(
+        self, subnet_id: int, option_data: OptionData, remote_map: dict = {}
+    ) -> KeaResponse:
+        """Creates/Replaces a DHCPv4 option in a subnet in the configuration database
+
+        Args:
+            subnet_id:      Subnet ID
+            option_data:    OptionData Object
+            remote_map:     (remote_type, remote_host or remote_port) to select a specific remote database
+        """
+        return self.api.send_command_remote(
+            command="remote-option4-subnet-set",
+            service=self.service,
+            arguments={
+                "subnets": [{"id": subnet_id}],
+                "options": [
+                    option_data.dict(
+                        exclude_none=True, exclude_unset=True, by_alias=True
+                    )
+                ],
+            },
+            remote_map=remote_map,
+        )
+
     def remote_network4_del(
         self, name: str, keep_subnets: bool = True, remote_map: dict = {}
     ) -> KeaResponse:
         """Deletes an existing Shared Network from the configuration database
 
         Args:
             name:           Name of shared network
```

### Comparing `pykeadhcp-0.6.0a0/pykeadhcp/exceptions.py` & `pykeadhcp-0.6.0a1/pykeadhcp/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,7 +103,13 @@
         super().__init__(self.message)
 
 
 class KeaReservationNotFoundException(KeaException):
     def __init__(self, reservation_data: str):
         self.message = f"Reservation '{reservation_data}' not found"
         super().__init__(self.message)
+
+
+class KeaClientClassNotFoundException(KeaException):
+    def __init__(self, client_class: str):
+        self.message = f"Client Class '{client_class}' not found"
+        super().__init__(self.message)
```

### Comparing `pykeadhcp-0.6.0a0/pykeadhcp/kea.py` & `pykeadhcp-0.6.0a1/pykeadhcp/kea.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp4/config.py` & `pykeadhcp-0.6.0a1/pykeadhcp/models/dhcp4/config.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp4/subnet.py` & `pykeadhcp-0.6.0a1/pykeadhcp/models/dhcp4/subnet.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp6/config.py` & `pykeadhcp-0.6.0a1/pykeadhcp/models/dhcp6/config.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.6.0a0/pykeadhcp/models/enums.py` & `pykeadhcp-0.6.0a1/pykeadhcp/models/enums.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.6.0a0/pykeadhcp/models/generic/config.py` & `pykeadhcp-0.6.0a1/pykeadhcp/models/generic/config.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.6.0a0/pykeadhcp/models/generic/daemon.py` & `pykeadhcp-0.6.0a1/pykeadhcp/models/generic/daemon.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.6.0a0/pykeadhcp/models/generic/database.py` & `pykeadhcp-0.6.0a1/pykeadhcp/models/generic/database.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.6.0a0/pykeadhcp/models/generic/dhcp_ddns.py` & `pykeadhcp-0.6.0a1/pykeadhcp/models/generic/dhcp_ddns.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.6.0a0/pykeadhcp/models/generic/logger.py` & `pykeadhcp-0.6.0a1/pykeadhcp/models/generic/logger.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.6.0a0/pykeadhcp/parsers/dhcp4.py` & `pykeadhcp-0.6.0a1/pykeadhcp/parsers/dhcp4.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.6.0a0/pykeadhcp/parsers/dhcp6.py` & `pykeadhcp-0.6.0a1/pykeadhcp/parsers/dhcp6.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.6.0a0/pykeadhcp/parsers/exceptions.py` & `pykeadhcp-0.6.0a1/pykeadhcp/parsers/exceptions.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.6.0a0/pykeadhcp/parsers/generic.py` & `pykeadhcp-0.6.0a1/pykeadhcp/parsers/generic.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.6.0a0/PKG-INFO` & `pykeadhcp-0.6.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykeadhcp
-Version: 0.6.0a0
+Version: 0.6.0a1
 Summary: Wrapper around requests module to query ISC Kea DHCP API Daemons (ctrlagent, dhcp4, dhcp6, ddns)
 License: Apache 2.0
 Author: Brandon Spendlove
 Author-email: brandon-spendlove@hotmail.co.uk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

