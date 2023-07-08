# Comparing `tmp/pykeadhcp-0.5.1.tar.gz` & `tmp/pykeadhcp-0.6.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykeadhcp-0.5.1.tar", max compression
+gzip compressed data, was "pykeadhcp-0.6.0a0.tar", max compression
```

## Comparing `pykeadhcp-0.5.1.tar` & `pykeadhcp-0.6.0a0.tar`

### file list

```diff
@@ -1,65 +1,67 @@
--rw-r--r--   0        0        0    11356 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/LICENSE
--rw-r--r--   0        0        0     7331 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/README.md
--rw-r--r--   0        0        0       30 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/__init__.py
--rw-r--r--   0        0        0      174 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/daemons/__init__.py
--rw-r--r--   0        0        0     4508 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/daemons/ctrlagent.py
--rw-r--r--   0        0        0     4526 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/daemons/ddns.py
--rw-r--r--   0        0        0    26078 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/daemons/dhcp4.py
--rw-r--r--   0        0        0    22336 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/daemons/dhcp6.py
--rw-r--r--   0        0        0     2718 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/exceptions.py
--rw-r--r--   0        0        0     8243 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/kea.py
--rw-r--r--   0        0        0        0 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/ctrlagent/__init__.py
--rw-r--r--   0        0        0      457 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/ctrlagent/config.py
--rw-r--r--   0        0        0        0 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/dhcp4/__init__.py
--rw-r--r--   0        0        0      331 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/dhcp4/client_class.py
--rw-r--r--   0        0        0      798 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/dhcp4/config.py
--rw-r--r--   0        0        0      212 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/dhcp4/lease.py
--rw-r--r--   0        0        0      303 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/dhcp4/reservation.py
--rw-r--r--   0        0        0      453 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/dhcp4/shared_network.py
--rw-r--r--   0        0        0      684 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/dhcp4/subnet.py
--rw-r--r--   0        0        0        0 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/dhcp6/__init__.py
--rw-r--r--   0        0        0      253 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/dhcp6/client_class.py
--rw-r--r--   0        0        0      922 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/dhcp6/config.py
--rw-r--r--   0        0        0      346 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/dhcp6/lease.py
--rw-r--r--   0        0        0      438 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/dhcp6/pd_pool.py
--rw-r--r--   0        0        0      212 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/dhcp6/reservation.py
--rw-r--r--   0        0        0      296 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/dhcp6/server_id.py
--rw-r--r--   0        0        0      380 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/dhcp6/shared_network.py
--rw-r--r--   0        0        0      501 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/dhcp6/subnet.py
--rw-r--r--   0        0        0     1550 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/enums.py
--rw-r--r--   0        0        0      169 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/__init__.py
--rw-r--r--   0        0        0      181 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/api_response.py
--rw-r--r--   0        0        0      477 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/authentication.py
--rw-r--r--   0        0        0      435 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/base.py
--rw-r--r--   0        0        0      415 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/client_class.py
--rw-r--r--   0        0        0     1394 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/config.py
--rw-r--r--   0        0        0      396 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/control_socket.py
--rw-r--r--   0        0        0     2458 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/daemon.py
--rw-r--r--   0        0        0      734 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/database.py
--rw-r--r--   0        0        0      399 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/dhcp_common.py
--rw-r--r--   0        0        0      873 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/dhcp_ddns.py
--rw-r--r--   0        0        0      158 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/dhcp_queue_control.py
--rw-r--r--   0        0        0      183 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/hook.py
--rw-r--r--   0        0        0      403 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/lease.py
--rw-r--r--   0        0        0      538 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/logger.py
--rw-r--r--   0        0        0      181 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/multi_threading.py
--rw-r--r--   0        0        0      259 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/option_data.py
--rw-r--r--   0        0        0      294 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/option_def.py
--rw-r--r--   0        0        0      306 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/pool.py
--rw-r--r--   0        0        0      141 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/relay.py
--rw-r--r--   0        0        0      379 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/reservation.py
--rw-r--r--   0        0        0      112 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/sanity_check.py
--rw-r--r--   0        0        0      175 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/shared_network.py
--rw-r--r--   0        0        0      249 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/sockets.py
--rw-r--r--   0        0        0      477 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/status.py
--rw-r--r--   0        0        0      390 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/subnet.py
--rw-r--r--   0        0        0      152 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/parsers/__init__.py
--rw-r--r--   0        0        0      508 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/parsers/ctrlagent.py
--rw-r--r--   0        0        0        0 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/parsers/ddns.py
--rw-r--r--   0        0        0    17838 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/parsers/dhcp4.py
--rw-r--r--   0        0        0    20361 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/parsers/dhcp6.py
--rw-r--r--   0        0        0     3436 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/parsers/exceptions.py
--rw-r--r--   0        0        0      825 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/parsers/generic.py
--rw-r--r--   0        0        0      447 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     7936 1970-01-01 00:00:00.000000 pykeadhcp-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/LICENSE
+-rw-r--r--   0        0        0     8001 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/README.md
+-rw-r--r--   0        0        0       30 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/__init__.py
+-rw-r--r--   0        0        0      174 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/daemons/__init__.py
+-rw-r--r--   0        0        0     4508 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/daemons/ctrlagent.py
+-rw-r--r--   0        0        0     4526 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/daemons/ddns.py
+-rw-r--r--   0        0        0    46982 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/daemons/dhcp4.py
+-rw-r--r--   0        0        0    22336 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/daemons/dhcp6.py
+-rw-r--r--   0        0        0     3865 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/exceptions.py
+-rw-r--r--   0        0        0    10415 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/kea.py
+-rw-r--r--   0        0        0        0 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/ctrlagent/__init__.py
+-rw-r--r--   0        0        0      457 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/ctrlagent/config.py
+-rw-r--r--   0        0        0        0 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp4/__init__.py
+-rw-r--r--   0        0        0      331 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp4/client_class.py
+-rw-r--r--   0        0        0      798 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp4/config.py
+-rw-r--r--   0        0        0      212 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp4/lease.py
+-rw-r--r--   0        0        0      303 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp4/reservation.py
+-rw-r--r--   0        0        0      453 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp4/shared_network.py
+-rw-r--r--   0        0        0      684 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp4/subnet.py
+-rw-r--r--   0        0        0        0 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp6/__init__.py
+-rw-r--r--   0        0        0      253 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp6/client_class.py
+-rw-r--r--   0        0        0      922 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp6/config.py
+-rw-r--r--   0        0        0      346 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp6/lease.py
+-rw-r--r--   0        0        0      438 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp6/pd_pool.py
+-rw-r--r--   0        0        0      212 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp6/reservation.py
+-rw-r--r--   0        0        0      296 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp6/server_id.py
+-rw-r--r--   0        0        0      380 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp6/shared_network.py
+-rw-r--r--   0        0        0      501 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp6/subnet.py
+-rw-r--r--   0        0        0     1638 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/enums.py
+-rw-r--r--   0        0        0      169 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/__init__.py
+-rw-r--r--   0        0        0      181 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/api_response.py
+-rw-r--r--   0        0        0      477 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/authentication.py
+-rw-r--r--   0        0        0      435 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/base.py
+-rw-r--r--   0        0        0      415 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/client_class.py
+-rw-r--r--   0        0        0     1394 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/config.py
+-rw-r--r--   0        0        0      396 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/control_socket.py
+-rw-r--r--   0        0        0     2458 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/daemon.py
+-rw-r--r--   0        0        0      734 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/database.py
+-rw-r--r--   0        0        0      399 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/dhcp_common.py
+-rw-r--r--   0        0        0      873 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/dhcp_ddns.py
+-rw-r--r--   0        0        0      158 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/dhcp_queue_control.py
+-rw-r--r--   0        0        0      183 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/hook.py
+-rw-r--r--   0        0        0      403 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/lease.py
+-rw-r--r--   0        0        0      558 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/logger.py
+-rw-r--r--   0        0        0      181 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/multi_threading.py
+-rw-r--r--   0        0        0      259 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/option_data.py
+-rw-r--r--   0        0        0      294 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/option_def.py
+-rw-r--r--   0        0        0      306 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/pool.py
+-rw-r--r--   0        0        0      141 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/relay.py
+-rw-r--r--   0        0        0      302 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/remote_map.py
+-rw-r--r--   0        0        0      217 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/remote_server.py
+-rw-r--r--   0        0        0      436 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/reservation.py
+-rw-r--r--   0        0        0      112 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/sanity_check.py
+-rw-r--r--   0        0        0      175 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/shared_network.py
+-rw-r--r--   0        0        0      249 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/sockets.py
+-rw-r--r--   0        0        0      477 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/status.py
+-rw-r--r--   0        0        0      390 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/models/generic/subnet.py
+-rw-r--r--   0        0        0      152 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/parsers/__init__.py
+-rw-r--r--   0        0        0      508 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/parsers/ctrlagent.py
+-rw-r--r--   0        0        0        0 2023-07-08 01:36:06.866582 pykeadhcp-0.6.0a0/pykeadhcp/parsers/ddns.py
+-rw-r--r--   0        0        0    17838 2023-07-08 01:36:06.870582 pykeadhcp-0.6.0a0/pykeadhcp/parsers/dhcp4.py
+-rw-r--r--   0        0        0    20361 2023-07-08 01:36:06.870582 pykeadhcp-0.6.0a0/pykeadhcp/parsers/dhcp6.py
+-rw-r--r--   0        0        0     3436 2023-07-08 01:36:06.870582 pykeadhcp-0.6.0a0/pykeadhcp/parsers/exceptions.py
+-rw-r--r--   0        0        0      825 2023-07-08 01:36:06.870582 pykeadhcp-0.6.0a0/pykeadhcp/parsers/generic.py
+-rw-r--r--   0        0        0      449 2023-07-08 01:36:06.870582 pykeadhcp-0.6.0a0/pyproject.toml
+-rw-r--r--   0        0        0     8608 1970-01-01 00:00:00.000000 pykeadhcp-0.6.0a0/PKG-INFO
```

### Comparing `pykeadhcp-0.5.1/LICENSE` & `pykeadhcp-0.6.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.5.1/README.md` & `pykeadhcp-0.6.0a0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -123,14 +123,32 @@
 
 ```
 server.dhcp4.refresh_cached_config()
 ```
 
 For API calls that don't amend the configuration (eg. lease4-add, lease6-add, config-get, etc....), there is no need to refresh the relevant daemon configuration. Maybe I will add a feature in the future to allow the user to specify if they want the cached_config to be automatically refreshed when a function is called that requires a refresh but for now its manual.
 
+## Configuration Backend (cb_cmds hook)
+
+Majority if not all `remote-` commands which interact with the configuration backend implement the `remote_map` variable which allows you to specify the database instance you want to [interact with as per documentation here](https://kea.readthedocs.io/en/kea-2.2.0/arm/hooks.html#command-structure). It accepts the following variables inside the dictionary:
+
+```
+{
+    "type": "<mysql | postgresql>",
+    "host": "<ip address>",
+    "port": <port>
+}
+
+For example:
+
+kea_server.dhcp4.remote_subnet4_set(subnet=subnet, server_tags=["all"], remote_map={"type": "mysql"})
+
+Note that the remote_map is optional and not mandatory.
+```
+
 ## Parsers
 
 Majority of the useful API functionality requires a subscription for the premium hooks to use API commands like `subnet4-add` or `network6-add` as an example. This is typically the recommended way to interact with Kea as there is some additional validation that the API will perform and potentially prevent misconfiguration of your daemons (Dhcp4, Dhcp6, Control Agent, DDNS) that pykeadhcp may not correctly implement.
 
 However with the use of `config-test` and `config-set` API commands which are supported for all daemons in the free version of ISC Kea DHCP, you can utilize the various parsers implemented in pykeadhcp which provides similar functionality to create, read, update and delete various resources like subnets, shared networks, reservations etc... The parsers attempt to parse a local configuration (eg. server.dhcp4.cached_config) and should be used with the 2 API commands `config-test` and `config-set`. The problem with `config-set` is that it will restart the daemon on the server unlike the specific commands to directly interact with the configuration.
 
 Before continuing, these parsers are manually crafted and can break at anytime when ISC release an update that changes the behaviour of the configuration model. Therefore you should use parsers at your own risk.
```

### Comparing `pykeadhcp-0.5.1/pykeadhcp/daemons/ctrlagent.py` & `pykeadhcp-0.6.0a0/pykeadhcp/daemons/ctrlagent.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.5.1/pykeadhcp/daemons/ddns.py` & `pykeadhcp-0.6.0a0/pykeadhcp/daemons/ddns.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.5.1/pykeadhcp/daemons/dhcp6.py` & `pykeadhcp-0.6.0a0/pykeadhcp/daemons/dhcp6.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.5.1/pykeadhcp/exceptions.py` & `pykeadhcp-0.6.0a0/pykeadhcp/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -63,15 +63,47 @@
     def __init__(self, name: str):
         self.message = f"Shared Network '{name}' not found"
         super().__init__(self.message)
 
 
 class KeaSubnetNotFoundException(KeaException):
     def __init__(self, subnet_id: int):
-        self.message = f"Subnet with id '{subnet_id}' not found"
+        self.message = f"Subnet '{subnet_id}' not found"
         super().__init__(self.message)
 
 
 class KeaLeaseNotFoundException(KeaException):
     def __init__(self, lease: str):
         self.message = f"Lease '{lease}' not found"
         super().__init__(self.message)
+
+
+class KeaInvalidRemoteMapException(KeaException):
+    def __init__(self, detailed_error: str):
+        self.message = f"Remote map for cm_cmd remote API call is not correctly formatted. Detailed Error: {detailed_error}"
+        super().__init__(self.message)
+
+
+class KeaRemoteServerNotFoundException(KeaException):
+    def __init__(self, server_tag: str):
+        self.message = f"Server with server_tag '{server_tag}' not found"
+        super().__init__(self.message)
+
+
+class KeaConfigBackendNotConfiguredException(KeaException):
+    def __init__(self):
+        self.message = "Kea API reports that there is no configuration backends"
+        super().__init__(self.message)
+
+
+class KeaUnknownHostReservationTypeException(KeaException):
+    def __init__(self, reservation_type: str):
+        self.message = (
+            f"Reservation type '{reservation_type}' is not a valid reservation type"
+        )
+        super().__init__(self.message)
+
+
+class KeaReservationNotFoundException(KeaException):
+    def __init__(self, reservation_data: str):
+        self.message = f"Reservation '{reservation_data}' not found"
+        super().__init__(self.message)
```

### Comparing `pykeadhcp-0.5.1/pykeadhcp/kea.py` & `pykeadhcp-0.6.0a0/pykeadhcp/kea.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import requests
 from requests.auth import HTTPBasicAuth
 from requests.exceptions import HTTPError
 from pathlib import Path
 from typing import List, Union
+from pydantic import ValidationError
 
 from pykeadhcp.daemons import CtrlAgent, Ddns, Dhcp4, Dhcp6
 from pykeadhcp.models.generic import KeaResponse
 from pykeadhcp.models.generic.hook import Hook
+from pykeadhcp.models.generic.remote_map import RemoteMap
 from pykeadhcp.exceptions import (
     KeaGenericException,
     KeaCommandNotSupportedException,
     KeaObjectNotFoundException,
     KeaServerConflictException,
     KeaUnauthorizedAccessException,
     KeaHookLibraryNotConfiguredException,
+    KeaInvalidRemoteMapException,
 )
 
 
 class Kea:
     """Basic wrapper around requests module for interacting with the
     Kea Management API for the various daemons supported.
 
@@ -198,14 +201,61 @@
 
         command_results = self.post(
             endpoint="/",
             body={
                 "command": command,
                 "service": [service] if service else [],
                 "arguments": arguments,
+            },
+        )
+        return command_results
+
+    def send_command_remote(
+        self, command: str, service: str, arguments: dict = {}, remote_map: dict = {}
+    ):
+        """Sends a command to the specific API daemon with provided arguments and remote map settings
+
+        This command should only be used with the cb_cmds hook.
+
+        Args:
+            command:        Supported command by the daemons API
+            service:        Service to send request to
+            arguments:      Argument parameters to pass to the command/service
+            required_hook:  Precheck if hook library is enabled
+            remote_map:     (remote_type, remote_host or remote_port) to select a specific remote database
+        """
+        if service and service.lower() not in self.services:
+            raise TypeError(
+                f"Service {service} is not a supported service. The supported services are {self.services}"
+            )
+
+        # All remote commands require cb_cmds hook to be loaded
+        if not self.is_hook_enabled("cb_cmds", self.hook_library[service]):
+            raise KeaHookLibraryNotConfiguredException(service, "cb_cmds")
+
+        # Build remote payload if user wants to select a specific database instance as per API documentation
+        # https://kea.readthedocs.io/en/kea-2.2.0/arm/hooks.html#command-structure
+        if remote_map:
+            try:
+                remote_map_parsed = RemoteMap.parse_obj(remote_map)
+            except ValidationError as err:
+                raise KeaInvalidRemoteMapException(str(err))
+            except Exception as err:
+                raise KeaInvalidRemoteMapException(f"Generic Exception caught: {err}")
+
+            arguments["remote"] = remote_map_parsed.dict(
+                exclude_unset=True, exclude_none=True
+            )
+
+        command_results = self.post(
+            endpoint="/",
+            body={
+                "command": command,
+                "service": [service] if service else [],
+                "arguments": arguments,
             },
         )
         return command_results
 
     def get_next_available_subnet_id(self, subnet_ids: List[int]) -> int:
         """Returns the next available subnet-id based on a given list of
         existing subnet-ids
```

### Comparing `pykeadhcp-0.5.1/pykeadhcp/models/dhcp4/config.py` & `pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp4/config.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.5.1/pykeadhcp/models/dhcp4/subnet.py` & `pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp4/subnet.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.5.1/pykeadhcp/models/dhcp6/config.py` & `pykeadhcp-0.6.0a0/pykeadhcp/models/dhcp6/config.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.5.1/pykeadhcp/models/enums.py` & `pykeadhcp-0.6.0a0/pykeadhcp/models/enums.py`

 * *Files 9% similar despite different names*

```diff
@@ -77,7 +77,12 @@
     llt = "LLT"
     en = "EN"
     ll = "LL"
 
 
 class AuthenticationTypeEnum(str, Enum):
     basic = "basic"
+
+
+class RemoteMapTypeEnum(str, Enum):
+    mysql = "mysql"
+    postgresql = "postgresql"
```

### Comparing `pykeadhcp-0.5.1/pykeadhcp/models/generic/config.py` & `pykeadhcp-0.6.0a0/pykeadhcp/models/generic/config.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.5.1/pykeadhcp/models/generic/daemon.py` & `pykeadhcp-0.6.0a0/pykeadhcp/models/generic/daemon.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.5.1/pykeadhcp/models/generic/database.py` & `pykeadhcp-0.6.0a0/pykeadhcp/models/generic/database.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.5.1/pykeadhcp/models/generic/dhcp_ddns.py` & `pykeadhcp-0.6.0a0/pykeadhcp/models/generic/dhcp_ddns.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.5.1/pykeadhcp/models/generic/logger.py` & `pykeadhcp-0.6.0a0/pykeadhcp/models/generic/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from pykeadhcp.models.generic.base import KeaBaseModel, KeaModel
 from pykeadhcp.models.enums import LoggerLevelEnum
 
 
 class Output(KeaBaseModel):
     output: str
     flush: bool
-    maxsize: int
-    maxver: int
+    maxsize: Optional[int]
+    maxver: Optional[int]
     pattern: Optional[str]
 
 
 class Logger(KeaModel):
     name: str
     output_options: Optional[List[Output]] = []
     debuglevel: conint(ge=0, le=100)
```

### Comparing `pykeadhcp-0.5.1/pykeadhcp/parsers/dhcp4.py` & `pykeadhcp-0.6.0a0/pykeadhcp/parsers/dhcp4.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.5.1/pykeadhcp/parsers/dhcp6.py` & `pykeadhcp-0.6.0a0/pykeadhcp/parsers/dhcp6.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.5.1/pykeadhcp/parsers/exceptions.py` & `pykeadhcp-0.6.0a0/pykeadhcp/parsers/exceptions.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.5.1/pykeadhcp/parsers/generic.py` & `pykeadhcp-0.6.0a0/pykeadhcp/parsers/generic.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.5.1/PKG-INFO` & `pykeadhcp-0.6.0a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykeadhcp
-Version: 0.5.1
+Version: 0.6.0a0
 Summary: Wrapper around requests module to query ISC Kea DHCP API Daemons (ctrlagent, dhcp4, dhcp6, ddns)
 License: Apache 2.0
 Author: Brandon Spendlove
 Author-email: brandon-spendlove@hotmail.co.uk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -139,14 +139,32 @@
 
 ```
 server.dhcp4.refresh_cached_config()
 ```
 
 For API calls that don't amend the configuration (eg. lease4-add, lease6-add, config-get, etc....), there is no need to refresh the relevant daemon configuration. Maybe I will add a feature in the future to allow the user to specify if they want the cached_config to be automatically refreshed when a function is called that requires a refresh but for now its manual.
 
+## Configuration Backend (cb_cmds hook)
+
+Majority if not all `remote-` commands which interact with the configuration backend implement the `remote_map` variable which allows you to specify the database instance you want to [interact with as per documentation here](https://kea.readthedocs.io/en/kea-2.2.0/arm/hooks.html#command-structure). It accepts the following variables inside the dictionary:
+
+```
+{
+    "type": "<mysql | postgresql>",
+    "host": "<ip address>",
+    "port": <port>
+}
+
+For example:
+
+kea_server.dhcp4.remote_subnet4_set(subnet=subnet, server_tags=["all"], remote_map={"type": "mysql"})
+
+Note that the remote_map is optional and not mandatory.
+```
+
 ## Parsers
 
 Majority of the useful API functionality requires a subscription for the premium hooks to use API commands like `subnet4-add` or `network6-add` as an example. This is typically the recommended way to interact with Kea as there is some additional validation that the API will perform and potentially prevent misconfiguration of your daemons (Dhcp4, Dhcp6, Control Agent, DDNS) that pykeadhcp may not correctly implement.
 
 However with the use of `config-test` and `config-set` API commands which are supported for all daemons in the free version of ISC Kea DHCP, you can utilize the various parsers implemented in pykeadhcp which provides similar functionality to create, read, update and delete various resources like subnets, shared networks, reservations etc... The parsers attempt to parse a local configuration (eg. server.dhcp4.cached_config) and should be used with the 2 API commands `config-test` and `config-set`. The problem with `config-set` is that it will restart the daemon on the server unlike the specific commands to directly interact with the configuration.
 
 Before continuing, these parsers are manually crafted and can break at anytime when ISC release an update that changes the behaviour of the configuration model. Therefore you should use parsers at your own risk.
```

