# Comparing `tmp/openapi_server_test-1.0.25.tar.gz` & `tmp/openapi_server_test-1.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapi_server_test-1.0.25.tar", last modified: Fri Jul  7 22:57:19 2023, max compression
+gzip compressed data, was "openapi_server_test-1.0.27.tar", last modified: Fri Jul  7 23:24:54 2023, max compression
```

## Comparing `openapi_server_test-1.0.25.tar` & `openapi_server_test-1.0.27.tar`

### file list

```diff
@@ -1,174 +1,85 @@
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 22:57:19.171676 openapi_server_test-1.0.25/
--rw-r--r--   0 jialening   (501) staff       (20)       83 2023-07-06 21:38:37.000000 openapi_server_test-1.0.25/MANIFEST.in
--rw-r--r--   0 jialening   (501) staff       (20)      201 2023-07-07 22:57:19.171252 openapi_server_test-1.0.25/PKG-INFO
--rw-r--r--   0 jialening   (501) staff       (20)      902 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/README.md
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 22:57:19.084725 openapi_server_test-1.0.25/app/
--rwxr-xr-x   0 jialening   (501) staff       (20)   117665 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/__init__.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 22:57:19.086406 openapi_server_test-1.0.25/app/alarm/
--rw-r--r--   0 jialening   (501) staff       (20)       49 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/alarm/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)     1781 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/alarm/endpoints.py
--rw-r--r--   0 jialening   (501) staff       (20)     1519 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/alarm/transports.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 22:57:19.086760 openapi_server_test-1.0.25/app/app_service/
--rw-r--r--   0 jialening   (501) staff       (20)       43 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/app_service/__init__.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 22:57:19.087909 openapi_server_test-1.0.25/app/app_service/app/
--rw-r--r--   0 jialening   (501) staff       (20)       49 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/app_service/app/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)     1757 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/app_service/app/endpoints.py
--rw-r--r--   0 jialening   (501) staff       (20)     1650 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/app_service/app/transports.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 22:57:19.089246 openapi_server_test-1.0.25/app/app_service/app_service/
--rw-r--r--   0 jialening   (501) staff       (20)       49 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/app_service/app_service/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)     1853 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/app_service/app_service/endpoints.py
--rw-r--r--   0 jialening   (501) staff       (20)     2612 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/app_service/app_service/transports.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 22:57:19.090948 openapi_server_test-1.0.25/app/authdns_zone/
--rw-r--r--   0 jialening   (501) staff       (20)       49 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/authdns_zone/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)     1877 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/authdns_zone/endpoints.py
--rw-r--r--   0 jialening   (501) staff       (20)     1582 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/authdns_zone/transports.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 22:57:19.091402 openapi_server_test-1.0.25/app/cdn/
--rw-r--r--   0 jialening   (501) staff       (20)      118 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/cdn/__init__.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 22:57:19.092383 openapi_server_test-1.0.25/app/cdn/ingress_host/
--rw-r--r--   0 jialening   (501) staff       (20)       49 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/cdn/ingress_host/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)     1913 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/cdn/ingress_host/endpoints.py
--rw-r--r--   0 jialening   (501) staff       (20)     2793 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/cdn/ingress_host/transports.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 22:57:19.093694 openapi_server_test-1.0.25/app/cdn/origin/
--rw-r--r--   0 jialening   (501) staff       (20)       49 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/cdn/origin/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)     1841 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/cdn/origin/endpoints.py
--rw-r--r--   0 jialening   (501) staff       (20)     2118 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/cdn/origin/transports.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 22:57:19.095320 openapi_server_test-1.0.25/app/cdn/policy/
--rw-r--r--   0 jialening   (501) staff       (20)       49 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/cdn/policy/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)     1843 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/cdn/policy/endpoints.py
--rw-r--r--   0 jialening   (501) staff       (20)     1817 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/cdn/policy/transports.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 22:57:19.097164 openapi_server_test-1.0.25/app/cdn/service/
--rw-r--r--   0 jialening   (501) staff       (20)       49 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/cdn/service/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)     1855 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/cdn/service/endpoints.py
--rw-r--r--   0 jialening   (501) staff       (20)     2277 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/cdn/service/transports.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 22:57:19.098949 openapi_server_test-1.0.25/app/cdn/service_group/
--rw-r--r--   0 jialening   (501) staff       (20)       49 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/cdn/service_group/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)     1926 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/cdn/service_group/endpoints.py
--rw-r--r--   0 jialening   (501) staff       (20)     1719 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/cdn/service_group/transports.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 22:57:19.101535 openapi_server_test-1.0.25/app/common/
--rw-r--r--   0 jialening   (501) staff       (20)       91 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/common/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)      310 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/common/consts.py
--rw-r--r--   0 jialening   (501) staff       (20)     5163 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/common/endpoints.py
--rw-r--r--   0 jialening   (501) staff       (20)     1637 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/common/errors.py
--rw-r--r--   0 jialening   (501) staff       (20)     4192 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/common/transports.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 22:57:19.103323 openapi_server_test-1.0.25/app/dns_app_service/
--rw-r--r--   0 jialening   (501) staff       (20)       49 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/dns_app_service/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)     1178 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/dns_app_service/endpoints.py
--rw-r--r--   0 jialening   (501) staff       (20)      843 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/dns_app_service/transports.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 22:57:19.103857 openapi_server_test-1.0.25/app/gts/
--rw-r--r--   0 jialening   (501) staff       (20)      128 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/gts/__init__.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 22:57:19.105833 openapi_server_test-1.0.25/app/gts/policy/
--rw-r--r--   0 jialening   (501) staff       (20)       49 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/gts/policy/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)     4179 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/gts/policy/endpoints.py
--rw-r--r--   0 jialening   (501) staff       (20)     4839 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/gts/policy/transports.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 22:57:19.114278 openapi_server_test-1.0.25/app/gts/region/
--rw-r--r--   0 jialening   (501) staff       (20)       49 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/gts/region/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)     1793 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/gts/region/endpoints.py
--rw-r--r--   0 jialening   (501) staff       (20)     1519 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/gts/region/transports.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 22:57:19.116302 openapi_server_test-1.0.25/app/gts/region_map/
--rw-r--r--   0 jialening   (501) staff       (20)       49 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/gts/region_map/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)     1841 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/gts/region_map/endpoints.py
--rw-r--r--   0 jialening   (501) staff       (20)     1516 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/gts/region_map/transports.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 22:57:19.117914 openapi_server_test-1.0.25/app/gts/ruleset/
--rw-r--r--   0 jialening   (501) staff       (20)       49 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/gts/ruleset/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)     1853 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/gts/ruleset/endpoints.py
--rw-r--r--   0 jialening   (501) staff       (20)     1522 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/gts/ruleset/transports.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 22:57:19.119322 openapi_server_test-1.0.25/app/gts/view/
--rw-r--r--   0 jialening   (501) staff       (20)       49 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/gts/view/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)     1817 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/gts/view/endpoints.py
--rw-r--r--   0 jialening   (501) staff       (20)     1551 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/gts/view/transports.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 22:57:19.120721 openapi_server_test-1.0.25/app/gts/zones/
--rw-r--r--   0 jialening   (501) staff       (20)       49 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/gts/zones/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)     1901 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/gts/zones/endpoints.py
--rw-r--r--   0 jialening   (501) staff       (20)     1599 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/gts/zones/transports.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 22:57:19.122559 openapi_server_test-1.0.25/app/health_monitors/
--rw-r--r--   0 jialening   (501) staff       (20)       49 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/health_monitors/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)     1889 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/health_monitors/endpoints.py
--rw-r--r--   0 jialening   (501) staff       (20)     1603 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/health_monitors/transports.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 22:57:19.124610 openapi_server_test-1.0.25/app/service_group/
--rw-r--r--   0 jialening   (501) staff       (20)       49 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/service_group/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)     1877 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/service_group/endpoints.py
--rw-r--r--   0 jialening   (501) staff       (20)     1925 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/app/service_group/transports.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 22:57:19.126435 openapi_server_test-1.0.25/dingman/
--rw-r--r--   0 jialening   (501) staff       (20)     1786 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/dingman/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)     4027 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/dingman/cli_pb2.py
--rw-r--r--   0 jialening   (501) staff       (20)     1257 2023-06-15 21:30:55.000000 openapi_server_test-1.0.25/dingman/cli_pb2_grpc.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 22:57:19.129344 openapi_server_test-1.0.25/openapi_server/
--rw-r--r--   0 jialening   (501) staff       (20)        0 2023-07-07 22:56:58.000000 openapi_server_test-1.0.25/openapi_server/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)      393 2023-07-07 22:56:58.000000 openapi_server_test-1.0.25/openapi_server/__main__.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 22:57:19.130827 openapi_server_test-1.0.25/openapi_server/controllers/
--rw-r--r--   0 jialening   (501) staff       (20)        0 2023-07-07 22:56:58.000000 openapi_server_test-1.0.25/openapi_server/controllers/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)     5687 2023-07-07 22:56:58.000000 openapi_server_test-1.0.25/openapi_server/controllers/deploy_resources_controller.py
--rw-r--r--   0 jialening   (501) staff       (20)      552 2023-07-07 22:56:58.000000 openapi_server_test-1.0.25/openapi_server/controllers/security_controller_.py
--rw-r--r--   0 jialening   (501) staff       (20)      608 2023-07-07 22:56:58.000000 openapi_server_test-1.0.25/openapi_server/encoder.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 22:57:19.162426 openapi_server_test-1.0.25/openapi_server/models/
--rw-r--r--   0 jialening   (501) staff       (20)     3610 2023-07-07 22:56:58.000000 openapi_server_test-1.0.25/openapi_server/models/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)     3753 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/affinity.py
--rw-r--r--   0 jialening   (501) staff       (20)     1913 2023-07-07 22:56:58.000000 openapi_server_test-1.0.25/openapi_server/models/base_model_.py
--rw-r--r--   0 jialening   (501) staff       (20)     4907 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/config.py
--rw-r--r--   0 jialening   (501) staff       (20)     2503 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/config_templates_inner.py
--rw-r--r--   0 jialening   (501) staff       (20)    16535 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/container.py
--rw-r--r--   0 jialening   (501) staff       (20)     2639 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/container_life_cycle.py
--rw-r--r--   0 jialening   (501) staff       (20)     3654 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/container_port.py
--rw-r--r--   0 jialening   (501) staff       (20)     3936 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/container_sec_context.py
--rw-r--r--   0 jialening   (501) staff       (20)     2568 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/container_sec_context_capabilities.py
--rw-r--r--   0 jialening   (501) staff       (20)    10247 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/deploy_platform_resource.py
--rw-r--r--   0 jialening   (501) staff       (20)     7015 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/deploy_resources.py
--rw-r--r--   0 jialening   (501) staff       (20)     3963 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/dingman_error.py
--rw-r--r--   0 jialening   (501) staff       (20)     2425 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/dingman_response.py
--rw-r--r--   0 jialening   (501) staff       (20)    10477 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/endpoint.py
--rw-r--r--   0 jialening   (501) staff       (20)     3192 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/env_from_source.py
--rw-r--r--   0 jialening   (501) staff       (20)     2961 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/env_var.py
--rw-r--r--   0 jialening   (501) staff       (20)     1827 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/env_var_source.py
--rw-r--r--   0 jialening   (501) staff       (20)     4682 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/http_get.py
--rw-r--r--   0 jialening   (501) staff       (20)     4413 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/http_ingress_path.py
--rw-r--r--   0 jialening   (501) staff       (20)     5643 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/ingress.py
--rw-r--r--   0 jialening   (501) staff       (20)     1821 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/ingress_backend.py
--rw-r--r--   0 jialening   (501) staff       (20)     2446 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/ingress_backend_service.py
--rw-r--r--   0 jialening   (501) staff       (20)     3082 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/ingress_rule.py
--rw-r--r--   0 jialening   (501) staff       (20)     3211 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/ingress_tls.py
--rw-r--r--   0 jialening   (501) staff       (20)     3561 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/life_cycle_handler.py
--rw-r--r--   0 jialening   (501) staff       (20)     4613 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/node_affinity.py
--rw-r--r--   0 jialening   (501) staff       (20)     2047 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/node_selector.py
--rw-r--r--   0 jialening   (501) staff       (20)     3199 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/node_selector_term.py
--rw-r--r--   0 jialening   (501) staff       (20)     2827 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/object_field_selector.py
--rw-r--r--   0 jialening   (501) staff       (20)     9740 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/persistent_volume_claim.py
--rw-r--r--   0 jialening   (501) staff       (20)     4948 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/pod.py
--rw-r--r--   0 jialening   (501) staff       (20)     4649 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/pod_affinity.py
--rw-r--r--   0 jialening   (501) staff       (20)     3664 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/pod_affinity_term.py
--rw-r--r--   0 jialening   (501) staff       (20)     4713 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/pod_anti_affinity.py
--rw-r--r--   0 jialening   (501) staff       (20)     2623 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/preferred_scheduling_term.py
--rw-r--r--   0 jialening   (501) staff       (20)     7480 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/probe.py
--rw-r--r--   0 jialening   (501) staff       (20)     3598 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/ref_volume_source.py
--rw-r--r--   0 jialening   (501) staff       (20)     6245 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/relabel_config.py
--rw-r--r--   0 jialening   (501) staff       (20)     2787 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/resource_requirements.py
--rw-r--r--   0 jialening   (501) staff       (20)     8819 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/service.py
--rw-r--r--   0 jialening   (501) staff       (20)     7583 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/service_monitor.py
--rw-r--r--   0 jialening   (501) staff       (20)     3055 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/service_monitor_namespace_selector.py
--rw-r--r--   0 jialening   (501) staff       (20)     5386 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/service_port.py
--rw-r--r--   0 jialening   (501) staff       (20)     2413 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/tcp_socket.py
--rw-r--r--   0 jialening   (501) staff       (20)     3521 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/update_strategy.py
--rw-r--r--   0 jialening   (501) staff       (20)     4965 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/update_strategy_rolling_update_config.py
--rw-r--r--   0 jialening   (501) staff       (20)     6189 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/volume.py
--rw-r--r--   0 jialening   (501) staff       (20)     3553 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/volume_device.py
--rw-r--r--   0 jialening   (501) staff       (20)     2767 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/volume_empty_dir.py
--rw-r--r--   0 jialening   (501) staff       (20)     2585 2023-07-07 22:56:57.000000 openapi_server_test-1.0.25/openapi_server/models/volume_host_path.py
--rw-r--r--   0 jialening   (501) staff       (20)     4139 2023-07-07 22:56:58.000000 openapi_server_test-1.0.25/openapi_server/models/volume_mount.py
--rw-r--r--   0 jialening   (501) staff       (20)     2938 2023-07-07 22:56:58.000000 openapi_server_test-1.0.25/openapi_server/models/volume_persistent_volume_claim.py
--rw-r--r--   0 jialening   (501) staff       (20)     2769 2023-07-07 22:56:58.000000 openapi_server_test-1.0.25/openapi_server/models/weighted_pod_affinity_term.py
--rw-r--r--   0 jialening   (501) staff       (20)    10344 2023-07-07 22:56:58.000000 openapi_server_test-1.0.25/openapi_server/models/workload.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 22:57:19.163528 openapi_server_test-1.0.25/openapi_server/openapi/
--rw-r--r--   0 jialening   (501) staff       (20)   164349 2023-07-07 22:56:58.000000 openapi_server_test-1.0.25/openapi_server/openapi/openapi.yaml
--rw-r--r--   0 jialening   (501) staff       (20)        7 2023-07-07 22:56:59.000000 openapi_server_test-1.0.25/openapi_server/openapi_version
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 22:57:19.167180 openapi_server_test-1.0.25/openapi_server/test/
--rw-r--r--   0 jialening   (501) staff       (20)      437 2023-07-07 22:56:58.000000 openapi_server_test-1.0.25/openapi_server/test/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)   120299 2023-07-07 22:56:58.000000 openapi_server_test-1.0.25/openapi_server/test/test_deploy_resources_controller.py
--rw-r--r--   0 jialening   (501) staff       (20)      809 2023-07-07 22:56:58.000000 openapi_server_test-1.0.25/openapi_server/typing_utils.py
--rw-r--r--   0 jialening   (501) staff       (20)     3533 2023-07-07 22:56:58.000000 openapi_server_test-1.0.25/openapi_server/util.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 22:57:19.170740 openapi_server_test-1.0.25/openapi_server_test.egg-info/
--rw-r--r--   0 jialening   (501) staff       (20)      201 2023-07-07 22:57:19.000000 openapi_server_test-1.0.25/openapi_server_test.egg-info/PKG-INFO
--rw-r--r--   0 jialening   (501) staff       (20)     4869 2023-07-07 22:57:19.000000 openapi_server_test-1.0.25/openapi_server_test.egg-info/SOURCES.txt
--rw-r--r--   0 jialening   (501) staff       (20)        1 2023-07-07 22:57:19.000000 openapi_server_test-1.0.25/openapi_server_test.egg-info/dependency_links.txt
--rw-r--r--   0 jialening   (501) staff       (20)        6 2023-07-07 22:57:19.000000 openapi_server_test-1.0.25/openapi_server_test.egg-info/requires.txt
--rw-r--r--   0 jialening   (501) staff       (20)       69 2023-07-07 22:57:19.000000 openapi_server_test-1.0.25/openapi_server_test.egg-info/top_level.txt
--rw-r--r--   0 jialening   (501) staff       (20)       38 2023-07-07 22:57:19.171832 openapi_server_test-1.0.25/setup.cfg
--rw-r--r--   0 jialening   (501) staff       (20)     1332 2023-07-07 22:56:23.000000 openapi_server_test-1.0.25/setup.py
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 23:24:54.747277 openapi_server_test-1.0.27/
+-rw-r--r--   0 jialening   (501) staff       (20)      100 2023-07-07 23:24:18.000000 openapi_server_test-1.0.27/MANIFEST.in
+-rw-r--r--   0 jialening   (501) staff       (20)      201 2023-07-07 23:24:54.746691 openapi_server_test-1.0.27/PKG-INFO
+-rw-r--r--   0 jialening   (501) staff       (20)      902 2023-06-15 21:30:55.000000 openapi_server_test-1.0.27/README.md
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 23:24:54.705828 openapi_server_test-1.0.27/openapi_server/
+-rw-r--r--   0 jialening   (501) staff       (20)        0 2023-07-07 23:24:46.000000 openapi_server_test-1.0.27/openapi_server/__init__.py
+-rw-r--r--   0 jialening   (501) staff       (20)      393 2023-07-07 23:24:46.000000 openapi_server_test-1.0.27/openapi_server/__main__.py
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 23:24:54.707278 openapi_server_test-1.0.27/openapi_server/controllers/
+-rw-r--r--   0 jialening   (501) staff       (20)        0 2023-07-07 23:24:46.000000 openapi_server_test-1.0.27/openapi_server/controllers/__init__.py
+-rw-r--r--   0 jialening   (501) staff       (20)     5687 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/controllers/deploy_resources_controller.py
+-rw-r--r--   0 jialening   (501) staff       (20)      552 2023-07-07 23:24:46.000000 openapi_server_test-1.0.27/openapi_server/controllers/security_controller_.py
+-rw-r--r--   0 jialening   (501) staff       (20)      608 2023-07-07 23:24:46.000000 openapi_server_test-1.0.27/openapi_server/encoder.py
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 23:24:54.737557 openapi_server_test-1.0.27/openapi_server/models/
+-rw-r--r--   0 jialening   (501) staff       (20)     3610 2023-07-07 23:24:46.000000 openapi_server_test-1.0.27/openapi_server/models/__init__.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3753 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/affinity.py
+-rw-r--r--   0 jialening   (501) staff       (20)     1913 2023-07-07 23:24:46.000000 openapi_server_test-1.0.27/openapi_server/models/base_model_.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4907 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/config.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2503 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/config_templates_inner.py
+-rw-r--r--   0 jialening   (501) staff       (20)    16535 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/container.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2639 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/container_life_cycle.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3654 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/container_port.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3936 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/container_sec_context.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2568 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/container_sec_context_capabilities.py
+-rw-r--r--   0 jialening   (501) staff       (20)    10247 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/deploy_platform_resource.py
+-rw-r--r--   0 jialening   (501) staff       (20)     7015 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/deploy_resources.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3963 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/dingman_error.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2425 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/dingman_response.py
+-rw-r--r--   0 jialening   (501) staff       (20)    10477 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/endpoint.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3192 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/env_from_source.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2961 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/env_var.py
+-rw-r--r--   0 jialening   (501) staff       (20)     1827 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/env_var_source.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4682 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/http_get.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4413 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/http_ingress_path.py
+-rw-r--r--   0 jialening   (501) staff       (20)     5643 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/ingress.py
+-rw-r--r--   0 jialening   (501) staff       (20)     1821 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/ingress_backend.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2446 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/ingress_backend_service.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3082 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/ingress_rule.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3211 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/ingress_tls.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3561 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/life_cycle_handler.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4613 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/node_affinity.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2047 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/node_selector.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3199 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/node_selector_term.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2827 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/object_field_selector.py
+-rw-r--r--   0 jialening   (501) staff       (20)     9740 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/persistent_volume_claim.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4948 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/pod.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4649 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/pod_affinity.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3664 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/pod_affinity_term.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4713 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/pod_anti_affinity.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2623 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/preferred_scheduling_term.py
+-rw-r--r--   0 jialening   (501) staff       (20)     7480 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/probe.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3598 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/ref_volume_source.py
+-rw-r--r--   0 jialening   (501) staff       (20)     6245 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/relabel_config.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2787 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/resource_requirements.py
+-rw-r--r--   0 jialening   (501) staff       (20)     8819 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/service.py
+-rw-r--r--   0 jialening   (501) staff       (20)     7583 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/service_monitor.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3055 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/service_monitor_namespace_selector.py
+-rw-r--r--   0 jialening   (501) staff       (20)     5386 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/service_port.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2413 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/tcp_socket.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3521 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/update_strategy.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4965 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/update_strategy_rolling_update_config.py
+-rw-r--r--   0 jialening   (501) staff       (20)     6189 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/volume.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3553 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/volume_device.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2767 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/volume_empty_dir.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2585 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/volume_host_path.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4139 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/volume_mount.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2938 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/volume_persistent_volume_claim.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2769 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/weighted_pod_affinity_term.py
+-rw-r--r--   0 jialening   (501) staff       (20)    10344 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/models/workload.py
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 23:24:54.737914 openapi_server_test-1.0.27/openapi_server/openapi/
+-rw-r--r--   0 jialening   (501) staff       (20)   164349 2023-07-07 23:24:46.000000 openapi_server_test-1.0.27/openapi_server/openapi/openapi.yaml
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 23:24:54.743945 openapi_server_test-1.0.27/openapi_server/openapi_server_test.egg-info/
+-rw-r--r--   0 jialening   (501) staff       (20)      201 2023-07-07 23:24:54.000000 openapi_server_test-1.0.27/openapi_server/openapi_server_test.egg-info/PKG-INFO
+-rw-r--r--   0 jialening   (501) staff       (20)     3049 2023-07-07 23:24:54.000000 openapi_server_test-1.0.27/openapi_server/openapi_server_test.egg-info/SOURCES.txt
+-rw-r--r--   0 jialening   (501) staff       (20)        1 2023-07-07 23:24:54.000000 openapi_server_test-1.0.27/openapi_server/openapi_server_test.egg-info/dependency_links.txt
+-rw-r--r--   0 jialening   (501) staff       (20)        6 2023-07-07 23:24:54.000000 openapi_server_test-1.0.27/openapi_server/openapi_server_test.egg-info/requires.txt
+-rw-r--r--   0 jialening   (501) staff       (20)       76 2023-07-07 23:24:54.000000 openapi_server_test-1.0.27/openapi_server/openapi_server_test.egg-info/top_level.txt
+-rw-r--r--   0 jialening   (501) staff       (20)        7 2023-07-07 23:24:46.000000 openapi_server_test-1.0.27/openapi_server/openapi_version
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-07 23:24:54.745437 openapi_server_test-1.0.27/openapi_server/test/
+-rw-r--r--   0 jialening   (501) staff       (20)      437 2023-07-07 23:24:46.000000 openapi_server_test-1.0.27/openapi_server/test/__init__.py
+-rw-r--r--   0 jialening   (501) staff       (20)   120299 2023-07-07 23:24:45.000000 openapi_server_test-1.0.27/openapi_server/test/test_deploy_resources_controller.py
+-rw-r--r--   0 jialening   (501) staff       (20)      809 2023-07-07 23:24:46.000000 openapi_server_test-1.0.27/openapi_server/typing_utils.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3533 2023-07-07 23:24:46.000000 openapi_server_test-1.0.27/openapi_server/util.py
+-rw-r--r--   0 jialening   (501) staff       (20)       38 2023-07-07 23:24:54.747488 openapi_server_test-1.0.27/setup.cfg
+-rw-r--r--   0 jialening   (501) staff       (20)     1252 2023-07-07 23:22:59.000000 openapi_server_test-1.0.27/setup.py
+-rw-r--r--   0 jialening   (501) staff       (20)        0 2023-07-07 23:24:06.000000 openapi_server_test-1.0.27/test.py
```

### Comparing `openapi_server_test-1.0.25/README.md` & `openapi_server_test-1.0.27/README.md`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/controllers/deploy_resources_controller.py` & `openapi_server_test-1.0.27/openapi_server/controllers/deploy_resources_controller.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/controllers/security_controller_.py` & `openapi_server_test-1.0.27/openapi_server/controllers/security_controller_.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/encoder.py` & `openapi_server_test-1.0.27/openapi_server/encoder.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/__init__.py` & `openapi_server_test-1.0.27/openapi_server/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/affinity.py` & `openapi_server_test-1.0.27/openapi_server/models/affinity.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/base_model_.py` & `openapi_server_test-1.0.27/openapi_server/models/base_model_.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/config.py` & `openapi_server_test-1.0.27/openapi_server/models/config.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/config_templates_inner.py` & `openapi_server_test-1.0.27/openapi_server/models/config_templates_inner.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/container.py` & `openapi_server_test-1.0.27/openapi_server/models/container.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/container_life_cycle.py` & `openapi_server_test-1.0.27/openapi_server/models/container_life_cycle.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/container_port.py` & `openapi_server_test-1.0.27/openapi_server/models/container_port.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/container_sec_context.py` & `openapi_server_test-1.0.27/openapi_server/models/container_sec_context.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/container_sec_context_capabilities.py` & `openapi_server_test-1.0.27/openapi_server/models/container_sec_context_capabilities.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/deploy_platform_resource.py` & `openapi_server_test-1.0.27/openapi_server/models/deploy_platform_resource.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/deploy_resources.py` & `openapi_server_test-1.0.27/openapi_server/models/deploy_resources.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/dingman_error.py` & `openapi_server_test-1.0.27/openapi_server/models/dingman_error.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/dingman_response.py` & `openapi_server_test-1.0.27/openapi_server/models/dingman_response.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/endpoint.py` & `openapi_server_test-1.0.27/openapi_server/models/endpoint.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/env_from_source.py` & `openapi_server_test-1.0.27/openapi_server/models/env_from_source.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/env_var.py` & `openapi_server_test-1.0.27/openapi_server/models/env_var.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/env_var_source.py` & `openapi_server_test-1.0.27/openapi_server/models/env_var_source.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/http_get.py` & `openapi_server_test-1.0.27/openapi_server/models/http_get.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/http_ingress_path.py` & `openapi_server_test-1.0.27/openapi_server/models/http_ingress_path.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/ingress.py` & `openapi_server_test-1.0.27/openapi_server/models/ingress.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/ingress_backend.py` & `openapi_server_test-1.0.27/openapi_server/models/ingress_backend.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/ingress_backend_service.py` & `openapi_server_test-1.0.27/openapi_server/models/ingress_backend_service.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/ingress_rule.py` & `openapi_server_test-1.0.27/openapi_server/models/ingress_rule.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/ingress_tls.py` & `openapi_server_test-1.0.27/openapi_server/models/ingress_tls.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/life_cycle_handler.py` & `openapi_server_test-1.0.27/openapi_server/models/life_cycle_handler.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/node_affinity.py` & `openapi_server_test-1.0.27/openapi_server/models/node_affinity.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/node_selector.py` & `openapi_server_test-1.0.27/openapi_server/models/node_selector.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/node_selector_term.py` & `openapi_server_test-1.0.27/openapi_server/models/node_selector_term.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/object_field_selector.py` & `openapi_server_test-1.0.27/openapi_server/models/object_field_selector.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/persistent_volume_claim.py` & `openapi_server_test-1.0.27/openapi_server/models/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/pod.py` & `openapi_server_test-1.0.27/openapi_server/models/pod.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/pod_affinity.py` & `openapi_server_test-1.0.27/openapi_server/models/pod_affinity.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/pod_affinity_term.py` & `openapi_server_test-1.0.27/openapi_server/models/pod_affinity_term.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/pod_anti_affinity.py` & `openapi_server_test-1.0.27/openapi_server/models/pod_anti_affinity.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/preferred_scheduling_term.py` & `openapi_server_test-1.0.27/openapi_server/models/preferred_scheduling_term.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/probe.py` & `openapi_server_test-1.0.27/openapi_server/models/probe.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/ref_volume_source.py` & `openapi_server_test-1.0.27/openapi_server/models/ref_volume_source.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/relabel_config.py` & `openapi_server_test-1.0.27/openapi_server/models/relabel_config.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/resource_requirements.py` & `openapi_server_test-1.0.27/openapi_server/models/resource_requirements.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/service.py` & `openapi_server_test-1.0.27/openapi_server/models/service.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/service_monitor.py` & `openapi_server_test-1.0.27/openapi_server/models/service_monitor.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/service_monitor_namespace_selector.py` & `openapi_server_test-1.0.27/openapi_server/models/service_monitor_namespace_selector.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/service_port.py` & `openapi_server_test-1.0.27/openapi_server/models/service_port.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/tcp_socket.py` & `openapi_server_test-1.0.27/openapi_server/models/tcp_socket.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/update_strategy.py` & `openapi_server_test-1.0.27/openapi_server/models/update_strategy.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/update_strategy_rolling_update_config.py` & `openapi_server_test-1.0.27/openapi_server/models/update_strategy_rolling_update_config.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/volume.py` & `openapi_server_test-1.0.27/openapi_server/models/volume.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/volume_device.py` & `openapi_server_test-1.0.27/openapi_server/models/volume_device.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/volume_empty_dir.py` & `openapi_server_test-1.0.27/openapi_server/models/volume_empty_dir.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/volume_host_path.py` & `openapi_server_test-1.0.27/openapi_server/models/volume_host_path.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/volume_mount.py` & `openapi_server_test-1.0.27/openapi_server/models/volume_mount.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/volume_persistent_volume_claim.py` & `openapi_server_test-1.0.27/openapi_server/models/volume_persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/weighted_pod_affinity_term.py` & `openapi_server_test-1.0.27/openapi_server/models/weighted_pod_affinity_term.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/models/workload.py` & `openapi_server_test-1.0.27/openapi_server/models/workload.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/openapi/openapi.yaml` & `openapi_server_test-1.0.27/openapi_server/openapi/openapi.yaml`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/test/test_deploy_resources_controller.py` & `openapi_server_test-1.0.27/openapi_server/test/test_deploy_resources_controller.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/typing_utils.py` & `openapi_server_test-1.0.27/openapi_server/typing_utils.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/openapi_server/util.py` & `openapi_server_test-1.0.27/openapi_server/util.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.25/setup.py` & `openapi_server_test-1.0.27/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,16 +35,16 @@
     version=api_version,
     author="BD Data Sys IE CDN",
     description="CDN DMS Open API",
     url="https://code.byted.org/savanna/dingman_api_server",
     # package_data={
     #     "": ["openapi_version"],
     # },
-    # packages=setuptools.find_packages(where="openapi_server"),
-    packages=['openapi_server/test', 'openapi_server/models', 'openapi_server/controllers'],
-    # package_dir={"":"openapi_server"},
-    include_package_data=True,
+    # packages=setuptools.find_packages(),
+    # packages=['openapi_server'],
+    package_dir={"":"openapi_server"},
+    # include_package_data=True,
     python_requires=">=3.7",
     install_requires = [
         "flask"
     ],
 )
```

