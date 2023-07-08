# Comparing `tmp/lichenggong-0.2.3.4.tar.gz` & `tmp/lichenggong-0.3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lichenggong-0.2.3.4.tar", last modified: Fri Sep 23 13:49:30 2022, max compression
+gzip compressed data, was "lichenggong-0.3.0.0.tar", last modified: Sat Jul  8 10:16:40 2023, max compression
```

## Comparing `lichenggong-0.2.3.4.tar` & `lichenggong-0.3.0.0.tar`

### file list

```diff
@@ -1,22 +1,8 @@
-drwxrwxrwx   0        0        0        0 2022-09-23 13:49:30.233404 lichenggong-0.2.3.4/
--rw-rw-rw-   0        0        0     1091 2022-09-02 00:32:24.000000 lichenggong-0.2.3.4/LICENSE
--rw-rw-rw-   0        0        0     1242 2022-09-23 13:49:30.200403 lichenggong-0.2.3.4/PKG-INFO
--rw-rw-rw-   0        0        0      833 2022-09-23 13:49:21.000000 lichenggong-0.2.3.4/README.md
-drwxrwxrwx   0        0        0        0 2022-09-23 13:49:30.168404 lichenggong-0.2.3.4/lichenggong/
-drwxrwxrwx   0        0        0        0 2022-09-23 13:49:30.198407 lichenggong-0.2.3.4/lichenggong/System/
--rw-rw-rw-   0        0        0        6 2022-09-18 09:10:01.000000 lichenggong-0.2.3.4/lichenggong/System/Password_for_Boss.txt
--rw-rw-rw-   0        0        0        1 2022-09-18 02:20:17.000000 lichenggong-0.2.3.4/lichenggong/System/lauguage.txt
--rw-rw-rw-   0        0        0        0 2022-09-10 11:16:06.000000 lichenggong-0.2.3.4/lichenggong/System/pi.txt
--rw-rw-rw-   0        0        0        5 2022-09-18 01:49:37.000000 lichenggong-0.2.3.4/lichenggong/System/upgrade.txt
--rw-rw-rw-   0        0        0        7 2022-09-23 13:43:34.000000 lichenggong-0.2.3.4/lichenggong/System/version.txt
--rw-rw-rw-   0        0        0     3473 2022-09-14 11:15:35.000000 lichenggong-0.2.3.4/lichenggong/System/windows蓝瓶钙圣经.txt
--rw-rw-rw-   0        0        0      198 2022-09-13 00:48:06.000000 lichenggong-0.2.3.4/lichenggong/__init__.py
--rw-rw-rw-   0        0        0    65334 2022-09-23 13:45:58.000000 lichenggong-0.2.3.4/lichenggong/__lidao__.py
--rw-rw-rw-   0        0        0       33 2022-09-23 13:22:16.000000 lichenggong-0.2.3.4/lichenggong/__test__.py
-drwxrwxrwx   0        0        0        0 2022-09-23 13:49:30.179405 lichenggong-0.2.3.4/lichenggong.egg-info/
--rw-rw-rw-   0        0        0     1242 2022-09-23 13:49:29.000000 lichenggong-0.2.3.4/lichenggong.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      446 2022-09-23 13:49:29.000000 lichenggong-0.2.3.4/lichenggong.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-23 13:49:29.000000 lichenggong-0.2.3.4/lichenggong.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2022-09-23 13:49:29.000000 lichenggong-0.2.3.4/lichenggong.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-09-23 13:49:30.234404 lichenggong-0.2.3.4/setup.cfg
--rw-rw-rw-   0        0        0      858 2022-09-23 13:46:42.000000 lichenggong-0.2.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 10:16:40.708974 lichenggong-0.3.0.0/
+-rw-rw-rw-   0        0        0      935 2023-07-08 10:16:40.693346 lichenggong-0.3.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-08 10:16:40.693346 lichenggong-0.3.0.0/lichenggong.egg-info/
+-rw-rw-rw-   0        0        0      935 2023-07-08 10:16:40.000000 lichenggong-0.3.0.0/lichenggong.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      139 2023-07-08 10:16:40.000000 lichenggong-0.3.0.0/lichenggong.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 10:16:40.000000 lichenggong-0.3.0.0/lichenggong.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 10:16:40.000000 lichenggong-0.3.0.0/lichenggong.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 10:16:40.708974 lichenggong-0.3.0.0/setup.cfg
```

