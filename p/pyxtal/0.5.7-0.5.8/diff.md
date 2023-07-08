# Comparing `tmp/pyxtal-0.5.7.tar.gz` & `tmp/pyxtal-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/qiangzhu/Desktop/github/PyXtal/dist/.tmp-hw7pnauu/pyxtal-0.5.7.tar", last modified: Tue Jun 20 14:43:17 2023, max compression
+gzip compressed data, was "/Users/qiangzhu/Desktop/github/PyXtal/dist/.tmp-26n5y_i3/pyxtal-0.5.8.tar", last modified: Sat Jul  8 02:39:13 2023, max compression
```

## Comparing `pyxtal-0.5.7.tar` & `pyxtal-0.5.8.tar`

### file list

```diff
@@ -1,156 +1,157 @@
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-20 14:43:17.000000 pyxtal-0.5.7/
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1084 2022-06-13 19:36:20.000000 pyxtal-0.5.7/LICENSE.txt
--rwxr-xr-x   0 qiangzhu   (501) staff       (20)       82 2022-06-15 16:30:37.000000 pyxtal-0.5.7/MANIFEST.in
--rw-r--r--   0 qiangzhu   (501) staff       (20)     5203 2023-06-20 14:43:17.000000 pyxtal-0.5.7/PKG-INFO
--rw-r--r--   0 qiangzhu   (501) staff       (20)     4692 2022-07-27 22:43:15.000000 pyxtal-0.5.7/README.md
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-20 14:43:17.000000 pyxtal-0.5.7/pyxtal/
--rw-r--r--   0 qiangzhu   (501) staff       (20)    31648 2022-08-14 23:14:59.000000 pyxtal-0.5.7/pyxtal/XRD.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)   101275 2023-06-14 20:14:43.000000 pyxtal-0.5.7/pyxtal/__init__.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)     5985 2022-06-21 15:19:36.000000 pyxtal-0.5.7/pyxtal/block_crystal.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1784 2022-06-23 22:59:32.000000 pyxtal-0.5.7/pyxtal/constants.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    13810 2022-06-21 13:41:23.000000 pyxtal-0.5.7/pyxtal/crystal.py
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-20 14:43:17.000000 pyxtal-0.5.7/pyxtal/database/
--rw-r--r--   0 qiangzhu   (501) staff       (20)    22281 2022-06-17 19:11:39.000000 pyxtal-0.5.7/pyxtal/database/HM_Full.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)        0 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/__init__.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)     6824 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/atomic_scattering_params.json
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2120 2022-08-11 19:04:42.000000 pyxtal-0.5.7/pyxtal/database/bonds.json
--rw-------   0 qiangzhu   (501) staff       (20)     2950 2022-01-27 19:42:36.000000 pyxtal-0.5.7/pyxtal/database/bug.json
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-20 14:43:17.000000 pyxtal-0.5.7/pyxtal/database/cifs/
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2051 2021-12-27 22:37:10.000000 pyxtal-0.5.7/pyxtal/database/cifs/0-G62.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1921 2021-11-09 00:08:43.000000 pyxtal-0.5.7/pyxtal/database/cifs/1-G59.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      367 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/191.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2043 2021-12-27 00:51:46.000000 pyxtal-0.5.7/pyxtal/database/cifs/2-G71.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2373 2021-12-27 00:21:38.000000 pyxtal-0.5.7/pyxtal/database/cifs/3-G139.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     5688 2021-11-09 00:08:43.000000 pyxtal-0.5.7/pyxtal/database/cifs/4-G225.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2940 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/ACBNZA01.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     9863 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/AXOSOW01.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1184 2022-04-27 19:27:52.000000 pyxtal-0.5.7/pyxtal/database/cifs/Al2SiO5_mp-4753_symmetrized.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1009 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/BTO-Amm2.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1323 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/BTO.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1534 2022-04-28 13:54:25.000000 pyxtal-0.5.7/pyxtal/database/cifs/CuAu_mp-582681_symmetrized.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     4636 2022-06-17 15:45:22.000000 pyxtal-0.5.7/pyxtal/database/cifs/FAU.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     3542 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/database/cifs/Fd3.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     6258 2022-06-17 19:14:34.000000 pyxtal-0.5.7/pyxtal/database/cifs/Fd3.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)     4992 2021-12-29 18:59:05.000000 pyxtal-0.5.7/pyxtal/database/cifs/Fd3m.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     9559 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/GUMMUW.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      885 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/GeF2.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2946 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/HAHCOI.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      221 2022-06-17 19:31:24.000000 pyxtal-0.5.7/pyxtal/database/cifs/I41amd.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1836 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/database/cifs/I4_132.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)    10505 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/JAPWIH.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)   441469 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/LAGNAL.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     7132 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/LUFHAW.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2001 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/LiCs.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)    12413 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/MERQIM.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1238 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/MPWO.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     4577 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/NaCl.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1416 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/NaSb3F10.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1180 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/NbO2.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1696 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/NiS-Cm.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1134 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/database/cifs/P3_112.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1498 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/database/cifs/P4_332.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      226 2022-06-17 19:18:01.000000 pyxtal-0.5.7/pyxtal/database/cifs/P4nmm.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1205 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/database/cifs/P6_422.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     6482 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/PAHYON01.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1184 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/PPO.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1086 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/PVO.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1222 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/database/cifs/Pm3.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      230 2022-06-17 19:19:37.000000 pyxtal-0.5.7/pyxtal/database/cifs/Pmmn.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)      286 2022-06-17 19:13:51.000000 pyxtal-0.5.7/pyxtal/database/cifs/Pn3.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)      286 2022-06-17 19:13:21.000000 pyxtal-0.5.7/pyxtal/database/cifs/Pn3m.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1605 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/database/cifs/R-3.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1933 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/database/cifs/R-3c.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      986 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/database/cifs/R32.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     3542 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/TMPPIO03.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)    13289 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/WEXBOS.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)   177150 2022-06-17 20:12:44.000000 pyxtal-0.5.7/pyxtal/database/cifs/YICMOP.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2546 2022-07-27 19:22:51.000000 pyxtal-0.5.7/pyxtal/database/cifs/anthracene.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2703 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/aspirin-c.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)    12951 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/aspirin.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1509 2022-07-27 00:49:00.000000 pyxtal-0.5.7/pyxtal/database/cifs/benzene.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      733 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/bug.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)    17895 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/coumarin.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2260 2022-01-18 15:40:54.000000 pyxtal-0.5.7/pyxtal/database/cifs/dist_6_0.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2260 2022-01-18 15:40:53.000000 pyxtal-0.5.7/pyxtal/database/cifs/dist_6_1.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     7884 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/gdh.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1964 2022-08-22 20:08:21.000000 pyxtal-0.5.7/pyxtal/database/cifs/ht_KNbBO.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     5997 2022-08-22 18:10:54.000000 pyxtal-0.5.7/pyxtal/database/cifs/ht_cristobalite.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1251 2022-08-22 18:21:32.000000 pyxtal-0.5.7/pyxtal/database/cifs/ht_quartz.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1864 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/ice.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2869 2022-08-22 20:08:21.000000 pyxtal-0.5.7/pyxtal/database/cifs/lt_KNbBO.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      931 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/lt_cristobalite.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      866 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/lt_quartz.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1541 2022-07-27 00:49:34.000000 pyxtal-0.5.7/pyxtal/database/cifs/naphthalene.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)   317844 2021-11-23 20:29:41.000000 pyxtal-0.5.7/pyxtal/database/cifs/resorcinol.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)      473 2022-01-21 16:08:56.000000 pyxtal-0.5.7/pyxtal/database/cifs/sim-0.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)      488 2022-01-21 16:08:55.000000 pyxtal-0.5.7/pyxtal/database/cifs/sim-1.vasp
--rw-r--r--   0 qiangzhu   (501) staff       (20)     4786 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/cifs/xxvi.cif
--rw-r--r--   0 qiangzhu   (501) staff       (20)  1103778 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/clusters.json
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2617 2022-06-23 00:39:04.000000 pyxtal-0.5.7/pyxtal/database/collection.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    19164 2022-06-14 14:22:59.000000 pyxtal-0.5.7/pyxtal/database/element.py
--rw-r--r--   0 qiangzhu   (501) staff       (20) 10480157 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/k_subgroup.json
--rw-r--r--   0 qiangzhu   (501) staff       (20)    20717 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/layer.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)    25842 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/layer_generators.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)    58872 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/layer_symmetry.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)    90734 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/molecules.json
--rw-r--r--   0 qiangzhu   (501) staff       (20)   130892 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/point.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)   146327 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/point_generators.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)   301944 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/point_symmetry.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)    18501 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/rod.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)    21935 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/rod_generators.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)    44320 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/rod_symmetry.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)     5478 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/symbols.json
--rw-r--r--   0 qiangzhu   (501) staff       (20)  1245398 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/t_subgroup.json
--rw-r--r--   0 qiangzhu   (501) staff       (20)   259897 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/wyckoff_generators.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)   251719 2021-08-17 15:48:08.000000 pyxtal-0.5.7/pyxtal/database/wyckoff_list.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)   117892 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/database/wyckoff_sets.json
--rw-r--r--   0 qiangzhu   (501) staff       (20)   627207 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/database/wyckoff_symmetry.csv
--rw-r--r--   0 qiangzhu   (501) staff       (20)     8405 2023-06-13 10:12:21.000000 pyxtal-0.5.7/pyxtal/db.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    18767 2023-01-09 17:49:14.000000 pyxtal-0.5.7/pyxtal/descriptor.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    42770 2023-04-04 17:06:21.000000 pyxtal-0.5.7/pyxtal/elasticity.py
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-20 14:43:17.000000 pyxtal-0.5.7/pyxtal/interface/
--rw-r--r--   0 qiangzhu   (501) staff       (20)    13515 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/interface/LJ.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)        0 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/interface/__init__.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    27549 2023-01-11 02:44:28.000000 pyxtal-0.5.7/pyxtal/interface/dftb.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    12441 2023-06-20 14:35:57.000000 pyxtal-0.5.7/pyxtal/interface/gulp.py
--rwxr-xr-x   0 qiangzhu   (501) staff       (20)    19477 2022-01-06 13:19:42.000000 pyxtal-0.5.7/pyxtal/interface/lammpslib.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)     8403 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/interface/vasp.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    31490 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/interface/vasprun.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    23034 2022-09-24 05:16:49.000000 pyxtal-0.5.7/pyxtal/io.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    67422 2023-06-12 20:57:05.000000 pyxtal-0.5.7/pyxtal/lattice.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    17952 2022-09-15 04:47:12.000000 pyxtal-0.5.7/pyxtal/molecular_crystal.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    63216 2022-11-18 06:08:23.000000 pyxtal-0.5.7/pyxtal/molecule.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)     2758 2022-08-09 01:18:08.000000 pyxtal-0.5.7/pyxtal/msg.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    30344 2022-08-15 15:30:42.000000 pyxtal-0.5.7/pyxtal/operations.py
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-20 14:43:17.000000 pyxtal-0.5.7/pyxtal/optimize/
--rw-r--r--   0 qiangzhu   (501) staff       (20)        0 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/optimize/__init__.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)     5636 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/optimize/fire.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    12084 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/optimize/fire2.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    14967 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/optimize/myscipy_optimize.py
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-20 14:43:17.000000 pyxtal-0.5.7/pyxtal/potentials/
--rw-r--r--   0 qiangzhu   (501) staff       (20)  1820580 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/potentials/CuAg.eam.alloy
--rw-r--r--   0 qiangzhu   (501) staff       (20)     1652 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/potentials/LJ_cluster.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)      837 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/potentials/Si.tersoff
--rw-r--r--   0 qiangzhu   (501) staff       (20)     3991 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/potentials/SiCGe.tersoff
--rwxr-xr-x   0 qiangzhu   (501) staff       (20)       26 2021-08-17 15:48:09.000000 pyxtal-0.5.7/pyxtal/potentials/__init__.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    16972 2023-06-12 20:43:44.000000 pyxtal-0.5.7/pyxtal/representation.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    46380 2023-06-05 08:59:34.000000 pyxtal-0.5.7/pyxtal/supergroup.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)   130450 2023-06-15 07:38:47.000000 pyxtal-0.5.7/pyxtal/symmetry.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    42484 2023-06-12 09:31:13.000000 pyxtal-0.5.7/pyxtal/test_all.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    11061 2022-06-20 18:26:47.000000 pyxtal-0.5.7/pyxtal/tolerance.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    17439 2023-06-15 07:58:40.000000 pyxtal-0.5.7/pyxtal/util.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)       22 2023-06-20 14:38:04.000000 pyxtal-0.5.7/pyxtal/version.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    13329 2022-09-09 18:39:24.000000 pyxtal-0.5.7/pyxtal/viz.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    39382 2023-06-09 13:57:18.000000 pyxtal-0.5.7/pyxtal/wyckoff_site.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)    21212 2023-06-05 08:57:39.000000 pyxtal-0.5.7/pyxtal/wyckoff_split.py
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-20 14:43:17.000000 pyxtal-0.5.7/pyxtal.egg-info/
--rw-r--r--   0 qiangzhu   (501) staff       (20)     5203 2023-06-20 14:43:17.000000 pyxtal-0.5.7/pyxtal.egg-info/PKG-INFO
--rw-r--r--   0 qiangzhu   (501) staff       (20)     4217 2023-06-20 14:43:17.000000 pyxtal-0.5.7/pyxtal.egg-info/SOURCES.txt
--rw-r--r--   0 qiangzhu   (501) staff       (20)        1 2023-06-20 14:43:17.000000 pyxtal-0.5.7/pyxtal.egg-info/dependency_links.txt
--rw-r--r--   0 qiangzhu   (501) staff       (20)      158 2023-06-20 14:43:17.000000 pyxtal-0.5.7/pyxtal.egg-info/requires.txt
--rw-r--r--   0 qiangzhu   (501) staff       (20)        7 2023-06-20 14:43:17.000000 pyxtal-0.5.7/pyxtal.egg-info/top_level.txt
-drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-06-20 14:43:17.000000 pyxtal-0.5.7/scripts/
--rwxr-xr-x   0 qiangzhu   (501) staff       (20)     3973 2021-08-17 15:48:09.000000 pyxtal-0.5.7/scripts/pyxtal_main.py
--rwxr-xr-x   0 qiangzhu   (501) staff       (20)      960 2021-08-17 15:48:09.000000 pyxtal-0.5.7/scripts/pyxtal_symmetry.py
--rw-r--r--   0 qiangzhu   (501) staff       (20)      125 2023-06-20 14:43:17.000000 pyxtal-0.5.7/setup.cfg
--rwxr-xr-x   0 qiangzhu   (501) staff       (20)     1796 2023-06-09 17:27:30.000000 pyxtal-0.5.7/setup.py
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-07-08 02:39:13.000000 pyxtal-0.5.8/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1084 2022-06-13 19:36:20.000000 pyxtal-0.5.8/LICENSE.txt
+-rwxr-xr-x   0 qiangzhu   (501) staff       (20)       83 2023-07-08 00:55:55.000000 pyxtal-0.5.8/MANIFEST.in
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     5203 2023-07-08 02:39:13.000000 pyxtal-0.5.8/PKG-INFO
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     4692 2022-07-27 22:43:15.000000 pyxtal-0.5.8/README.md
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-07-08 02:39:13.000000 pyxtal-0.5.8/pyxtal/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    31648 2022-08-14 23:14:59.000000 pyxtal-0.5.8/pyxtal/XRD.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   105417 2023-07-08 02:10:23.000000 pyxtal-0.5.8/pyxtal/__init__.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     5985 2022-06-21 15:19:36.000000 pyxtal-0.5.8/pyxtal/block_crystal.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1784 2022-06-23 22:59:32.000000 pyxtal-0.5.8/pyxtal/constants.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    13810 2022-06-21 13:41:23.000000 pyxtal-0.5.8/pyxtal/crystal.py
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-07-08 02:39:13.000000 pyxtal-0.5.8/pyxtal/database/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    22281 2022-06-17 19:11:39.000000 pyxtal-0.5.8/pyxtal/database/HM_Full.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)        0 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/__init__.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     6824 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/atomic_scattering_params.json
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2120 2022-08-11 19:04:42.000000 pyxtal-0.5.8/pyxtal/database/bonds.json
+-rw-------   0 qiangzhu   (501) staff       (20)     2950 2022-01-27 19:42:36.000000 pyxtal-0.5.8/pyxtal/database/bug.json
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-07-08 02:39:13.000000 pyxtal-0.5.8/pyxtal/database/cifs/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2051 2021-12-27 22:37:10.000000 pyxtal-0.5.8/pyxtal/database/cifs/0-G62.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1921 2021-11-09 00:08:43.000000 pyxtal-0.5.8/pyxtal/database/cifs/1-G59.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      367 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/191.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2043 2021-12-27 00:51:46.000000 pyxtal-0.5.8/pyxtal/database/cifs/2-G71.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2373 2021-12-27 00:21:38.000000 pyxtal-0.5.8/pyxtal/database/cifs/3-G139.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     5688 2021-11-09 00:08:43.000000 pyxtal-0.5.8/pyxtal/database/cifs/4-G225.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2940 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/ACBNZA01.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     9863 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/AXOSOW01.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1184 2022-04-27 19:27:52.000000 pyxtal-0.5.8/pyxtal/database/cifs/Al2SiO5_mp-4753_symmetrized.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1009 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/BTO-Amm2.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1323 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/BTO.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1534 2022-04-28 13:54:25.000000 pyxtal-0.5.8/pyxtal/database/cifs/CuAu_mp-582681_symmetrized.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     4636 2022-06-17 15:45:22.000000 pyxtal-0.5.8/pyxtal/database/cifs/FAU.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     3542 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/database/cifs/Fd3.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     6258 2022-06-17 19:14:34.000000 pyxtal-0.5.8/pyxtal/database/cifs/Fd3.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     4992 2021-12-29 18:59:05.000000 pyxtal-0.5.8/pyxtal/database/cifs/Fd3m.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     9559 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/GUMMUW.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      885 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/GeF2.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2946 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/HAHCOI.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      221 2022-06-17 19:31:24.000000 pyxtal-0.5.8/pyxtal/database/cifs/I41amd.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1836 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/database/cifs/I4_132.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    10505 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/JAPWIH.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   441469 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/LAGNAL.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     7132 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/LUFHAW.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2001 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/LiCs.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    12413 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/MERQIM.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1238 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/MPWO.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     4577 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/NaCl.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1416 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/NaSb3F10.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1180 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/NbO2.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1696 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/NiS-Cm.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1134 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/database/cifs/P3_112.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1498 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/database/cifs/P4_332.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      226 2022-06-17 19:18:01.000000 pyxtal-0.5.8/pyxtal/database/cifs/P4nmm.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1205 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/database/cifs/P6_422.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     6482 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/PAHYON01.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1184 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/PPO.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1086 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/PVO.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1222 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/database/cifs/Pm3.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      230 2022-06-17 19:19:37.000000 pyxtal-0.5.8/pyxtal/database/cifs/Pmmn.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      286 2022-06-17 19:13:51.000000 pyxtal-0.5.8/pyxtal/database/cifs/Pn3.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      286 2022-06-17 19:13:21.000000 pyxtal-0.5.8/pyxtal/database/cifs/Pn3m.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1605 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/database/cifs/R-3.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1933 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/database/cifs/R-3c.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      986 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/database/cifs/R32.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     3542 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/TMPPIO03.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    13289 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/WEXBOS.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   177150 2022-06-17 20:12:44.000000 pyxtal-0.5.8/pyxtal/database/cifs/YICMOP.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)        0 2023-07-08 02:10:33.000000 pyxtal-0.5.8/pyxtal/database/cifs/__init__.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2546 2022-07-27 19:22:51.000000 pyxtal-0.5.8/pyxtal/database/cifs/anthracene.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2703 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/aspirin-c.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    12951 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/aspirin.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1509 2022-07-27 00:49:00.000000 pyxtal-0.5.8/pyxtal/database/cifs/benzene.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      733 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/bug.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    17895 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/coumarin.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2260 2022-01-18 15:40:54.000000 pyxtal-0.5.8/pyxtal/database/cifs/dist_6_0.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2260 2022-01-18 15:40:53.000000 pyxtal-0.5.8/pyxtal/database/cifs/dist_6_1.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     7884 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/gdh.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1964 2022-08-22 20:08:21.000000 pyxtal-0.5.8/pyxtal/database/cifs/ht_KNbBO.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     5997 2022-08-22 18:10:54.000000 pyxtal-0.5.8/pyxtal/database/cifs/ht_cristobalite.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1251 2022-08-22 18:21:32.000000 pyxtal-0.5.8/pyxtal/database/cifs/ht_quartz.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1864 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/ice.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2869 2022-08-22 20:08:21.000000 pyxtal-0.5.8/pyxtal/database/cifs/lt_KNbBO.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      931 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/lt_cristobalite.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      866 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/lt_quartz.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1541 2022-07-27 00:49:34.000000 pyxtal-0.5.8/pyxtal/database/cifs/naphthalene.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   317844 2021-11-23 20:29:41.000000 pyxtal-0.5.8/pyxtal/database/cifs/resorcinol.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      473 2022-01-21 16:08:56.000000 pyxtal-0.5.8/pyxtal/database/cifs/sim-0.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      488 2022-01-21 16:08:55.000000 pyxtal-0.5.8/pyxtal/database/cifs/sim-1.vasp
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     4786 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/cifs/xxvi.cif
+-rw-r--r--   0 qiangzhu   (501) staff       (20)  1103778 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/clusters.json
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2617 2022-06-23 00:39:04.000000 pyxtal-0.5.8/pyxtal/database/collection.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    19164 2022-06-14 14:22:59.000000 pyxtal-0.5.8/pyxtal/database/element.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20) 10480157 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/k_subgroup.json
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    20717 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/layer.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    25842 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/layer_generators.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    58872 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/layer_symmetry.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    90734 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/molecules.json
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   130892 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/point.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   146327 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/point_generators.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   301944 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/point_symmetry.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    18501 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/rod.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    21935 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/rod_generators.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    44320 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/rod_symmetry.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     5478 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/symbols.json
+-rw-r--r--   0 qiangzhu   (501) staff       (20)  1245398 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/t_subgroup.json
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   259897 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/wyckoff_generators.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   251719 2021-08-17 15:48:08.000000 pyxtal-0.5.8/pyxtal/database/wyckoff_list.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   117892 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/database/wyckoff_sets.json
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   627207 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/database/wyckoff_symmetry.csv
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     8405 2023-06-28 06:05:35.000000 pyxtal-0.5.8/pyxtal/db.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    18843 2023-07-08 02:00:23.000000 pyxtal-0.5.8/pyxtal/descriptor.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    42770 2023-04-04 17:06:21.000000 pyxtal-0.5.8/pyxtal/elasticity.py
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-07-08 02:39:13.000000 pyxtal-0.5.8/pyxtal/interface/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    13515 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/interface/LJ.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)        0 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/interface/__init__.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    27602 2023-07-01 12:59:09.000000 pyxtal-0.5.8/pyxtal/interface/dftb.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    14489 2023-06-23 09:35:50.000000 pyxtal-0.5.8/pyxtal/interface/gulp.py
+-rwxr-xr-x   0 qiangzhu   (501) staff       (20)    19477 2022-01-06 13:19:42.000000 pyxtal-0.5.8/pyxtal/interface/lammpslib.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     8403 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/interface/vasp.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    31490 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/interface/vasprun.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    23034 2022-09-24 05:16:49.000000 pyxtal-0.5.8/pyxtal/io.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    67553 2023-06-22 22:47:40.000000 pyxtal-0.5.8/pyxtal/lattice.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    18090 2023-07-08 01:32:18.000000 pyxtal-0.5.8/pyxtal/molecular_crystal.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    63216 2022-11-18 06:08:23.000000 pyxtal-0.5.8/pyxtal/molecule.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     2758 2022-08-09 01:18:08.000000 pyxtal-0.5.8/pyxtal/msg.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    30344 2023-06-23 21:31:46.000000 pyxtal-0.5.8/pyxtal/operations.py
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-07-08 02:39:13.000000 pyxtal-0.5.8/pyxtal/optimize/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)        0 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/optimize/__init__.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     5636 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/optimize/fire.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    12084 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/optimize/fire2.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    14967 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/optimize/myscipy_optimize.py
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-07-08 02:39:13.000000 pyxtal-0.5.8/pyxtal/potentials/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)  1820580 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/potentials/CuAg.eam.alloy
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     1652 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/potentials/LJ_cluster.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      837 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/potentials/Si.tersoff
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     3991 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/potentials/SiCGe.tersoff
+-rwxr-xr-x   0 qiangzhu   (501) staff       (20)       26 2021-08-17 15:48:09.000000 pyxtal-0.5.8/pyxtal/potentials/__init__.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    16972 2023-06-23 22:45:29.000000 pyxtal-0.5.8/pyxtal/representation.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    46380 2023-06-05 08:59:34.000000 pyxtal-0.5.8/pyxtal/supergroup.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)   130447 2023-06-24 19:46:55.000000 pyxtal-0.5.8/pyxtal/symmetry.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    43692 2023-07-08 02:00:44.000000 pyxtal-0.5.8/pyxtal/test_all.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    11061 2023-07-08 00:51:34.000000 pyxtal-0.5.8/pyxtal/tolerance.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    17663 2023-06-25 10:12:42.000000 pyxtal-0.5.8/pyxtal/util.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)       22 2023-07-08 00:52:50.000000 pyxtal-0.5.8/pyxtal/version.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    13329 2022-09-09 18:39:24.000000 pyxtal-0.5.8/pyxtal/viz.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    40631 2023-07-08 01:50:50.000000 pyxtal-0.5.8/pyxtal/wyckoff_site.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)    21212 2023-06-05 08:57:39.000000 pyxtal-0.5.8/pyxtal/wyckoff_split.py
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-07-08 02:39:13.000000 pyxtal-0.5.8/pyxtal.egg-info/
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     5203 2023-07-08 02:39:13.000000 pyxtal-0.5.8/pyxtal.egg-info/PKG-INFO
+-rw-r--r--   0 qiangzhu   (501) staff       (20)     4250 2023-07-08 02:39:13.000000 pyxtal-0.5.8/pyxtal.egg-info/SOURCES.txt
+-rw-r--r--   0 qiangzhu   (501) staff       (20)        1 2023-07-08 02:39:13.000000 pyxtal-0.5.8/pyxtal.egg-info/dependency_links.txt
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      160 2023-07-08 02:39:13.000000 pyxtal-0.5.8/pyxtal.egg-info/requires.txt
+-rw-r--r--   0 qiangzhu   (501) staff       (20)        7 2023-07-08 02:39:13.000000 pyxtal-0.5.8/pyxtal.egg-info/top_level.txt
+drwxr-xr-x   0 qiangzhu   (501) staff       (20)        0 2023-07-08 02:39:13.000000 pyxtal-0.5.8/scripts/
+-rwxr-xr-x   0 qiangzhu   (501) staff       (20)     4296 2023-06-27 08:23:49.000000 pyxtal-0.5.8/scripts/pyxtal_main.py
+-rwxr-xr-x   0 qiangzhu   (501) staff       (20)      960 2021-08-17 15:48:09.000000 pyxtal-0.5.8/scripts/pyxtal_symmetry.py
+-rw-r--r--   0 qiangzhu   (501) staff       (20)      125 2023-07-08 02:39:13.000000 pyxtal-0.5.8/setup.cfg
+-rwxr-xr-x   0 qiangzhu   (501) staff       (20)     1798 2023-07-08 00:50:33.000000 pyxtal-0.5.8/setup.py
```

### Comparing `pyxtal-0.5.7/LICENSE.txt` & `pyxtal-0.5.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/PKG-INFO` & `pyxtal-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxtal
-Version: 0.5.7
+Version: 0.5.8
 Summary: Python code for generation of crystal structures based on symmetry constraints.
 Home-page: https://github.com/qzhu2017/PyXtal
 Author: Scott Fredericks, Qiang Zhu
 Author-email: qiang.zhu@unlv.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyxtal-0.5.7/README.md` & `pyxtal-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/XRD.py` & `pyxtal-0.5.8/pyxtal/XRD.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/__init__.py` & `pyxtal-0.5.8/pyxtal/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 from pyxtal.lattice import Lattice
 from pyxtal.tolerance import Tol_matrix
 from pyxtal.representation import representation, representation_atom
 from pyxtal.io import read_cif, write_cif, structure_from_ext
 from pyxtal.constants import letters
 from pyxtal.viz import display_molecular, display_atomic, display_cluster
 from pyxtal.constants import letters
-from pyxtal.descriptor import spherical_image
 
 # name = "pyxtal"
 
 def print_logo():
     """
     print out the logo and version information
     """
@@ -193,20 +192,21 @@
 
     def __str__(self):
         if self.valid:
             s = "\n------Crystal from {:s}------".format(self.source)
             s += "\nDimension: {}".format(self.dim)
             s += "\nComposition: {}".format(self.formula)
             #if not self.standard_setting:
-            if self.molecular:
-                symbol = self.mol_sites[0].wp.get_hm_symbol()
+            if self.dim < 3:
+                symbol = self.group.symbol
             else:
-                symbol = self.atom_sites[0].wp.get_hm_symbol()
-            #else:
-            #    symbol = self.group.symbol
+                if self.molecular:
+                    symbol = self.mol_sites[0].wp.get_hm_symbol()
+                else:
+                    symbol = self.atom_sites[0].wp.get_hm_symbol()
             s += "\nGroup: {} ({})".format(symbol, self.group.number)
             s += "\n{}".format(self.lattice)
             s += "\nWyckoff sites:"
             if self.molecular:
                 for wyc in self.mol_sites:
                     s += "\n\t{}".format(wyc)
             else:
@@ -1548,24 +1548,32 @@
         if self.molecular:
             pmg = self.to_pymatgen()
             self.from_seed(pmg, molecules=self.molecules, standard=True)
 
     def resort_species(self, species):
         """
         resort the atomic species
+
+        Args:
+            species: list of elements, e.g. ['Si', 'O']
         """
-        sp1 = deepcopy(species).sort()
-        sp2 = deepcopy(self.species).sort()
+        sp1 = deepcopy(species); sp1.sort()
+        sp2 = deepcopy(self.species); sp2.sort()
         if sp1 == sp2:
             self.species = species
             self.resort()
-            #self._get_formula()
-            #print("=========Sort", species, self.species)
         else:
-            raise ValueError("the species are inconsistent", species, self.sepecies)
+            ids = []
+            for specie in species:
+                for j, site in enumerate(self.atom_sites):
+                    if site.specie == specie and j not in ids:
+                        ids.append(j)
+            self.atom_sites = [self.atom_sites[j] for j in ids]
+            self.species = species
+            self._get_formula()
 
     def resort(self):
         """
         A short cut to resort the sites by self.molecules or self.species
         """
         ids = []
         if self.molecular:
@@ -1688,56 +1696,75 @@
 
     def get_density(self):
         """
         Compute density
         """
         return self.to_pymatgen().density
 
-    def has_special_site(self):
+    def has_special_site(self, species=None):
         """
-        Check if the molecular crystal has a special site
+        Check if the crystal has a special site
         """
         special = False
-        for msite in self.mol_sites:
-            if msite.wp.index > 0:
+        if species is None: species = self.species
+
+        if self.molecular:
+            sites = self.mol_sites
+        else:
+            sites = self.atom_sites
+
+        for msite in sites:
+            if msite.specie in species and msite.wp.index > 0:
                 special = True
                 break
         return special
 
-    def to_subgroup(self, path=None):
+    def to_subgroup(self, path=None, t_only=True,iterate=False, species=None):
         """
         Transform a crystal with speical sites to subgroup
         represenatation with general sites
+
+        Args:
+            Path: list of path to get the general sites
+            iterate (bool): whether or not do it iteratively
         """
         if not self.standard_setting:
             self.optimize_lattice(standard=True)
+        if species is None: species = self.species
 
         # Compute the path is needed
         if path is None:
             if self.molecular:
                 sites = self.mol_sites
             else:
                 sites = self.atom_sites
 
-            max_index = max([site.wp.index for site in sites])
+            max_index = max([site.wp.index for site in sites if site.specie in species])
+            #print([site.wp.index for site in sites])
             if self.molecular:
-                path = self.group.short_path_to_general_wp(max_index, True)
+                path = self.group.short_path_to_general_wp(max_index, t_only)
             else:
-                path = self.group.short_path_to_general_wp(max_index)
+                path = self.group.short_path_to_general_wp(max_index, t_only)
+            #print(max_index, path)
 
         if path is not None:
             gtypes, ids = [], []
             for p in path:
                 gtypes.append(p[0])
                 ids.append(p[1])
             sub = self.subgroup_by_path(gtypes, ids, eps=0)
             sub.optimize_lattice()
             sub.source = "subgroup"
         else:
             sub = self.copy()
+
+        if iterate:
+            if sub.has_special_site(): 
+                sub = sub.to_subgroup()
+
         return sub
 
     def show(self, **kwargs):
         """
         display the crystal structure
         """
         if self.molecular:
@@ -2437,14 +2464,16 @@
 
         Args:
             model: either 'molecule' or 'contacts'
 
         Returns:
             the sph class
         """
+        from pyxtal.descriptor import spherical_image
+
         sph = spherical_image(self, **kwargs)
         return sph
 
     def get_neighboring_dists(self, site_id=0, factor=1.5, max_d=5.0):
         """
         For molecular crystals, get the neighboring molecules for a given WP
 
@@ -2522,24 +2551,118 @@
             molecules.append(Molecule(specie0, neigh))
 
         return display_cluster(molecules, self.lattice.matrix, engs, cmap, **kwargs)
 
     def substitute(self, dicts):
         """
         A quick function to apply substitution
-        For molecule only
 
         Args:
             dicts: e.g., {"F": "Cl"}
         """
         pmg = self.to_pymatgen()
         pmg.replace_species(dicts)
-        for e1e in dicts.keys():
-            smi = [m.smile.replace(ele, dicts[ele]) + '.smi' for m in self.molecules]
-        self.from_seed(pmg, smi)
+        if self.molecular:
+            for e1e in dicts.keys():
+                smi = [m.smile.replace(ele, dicts[ele]) + '.smi' for m in self.molecules]
+            self.from_seed(pmg, smi)
+        else:
+            self.from_seed(pmg)
+
+    def remove_species(self, species):
+        """
+        To remove the atom_sites by specie name
+        Args:
+            dicts: e.g., ["O"]
+        """
+        numIons = []
+        new_species = []
+        sites = []
+        count = 0
+        for site in self.atom_sites:
+            sp = site.specie
+            if sp not in species:
+                num = site.wp.multiplicity 
+                sites.append(site)
+                if sp in new_species:
+                    id = new_species.index(sp)
+                    numIons[id] += num
+                else:
+                    new_species.append(sp)
+                    numIons.append(num)
+            count += num
+        struc = self.copy()
+        struc.atom_sites = sites
+        struc.numIons = numIons
+        struc.species = new_species
+        struc.resort()
+        return struc
+
+
+    def substitute_linear(self, dicts):
+        """
+        This is mainly designed for substitution between single atom and the linear block
+        e.g., we want to make Zn(CN)2 from SiO2
+        Args:
+            dicts: e.g., {"Si": ["Zn"], "O": ["C","N"]}
+        """
+        from ase.neighborlist import neighbor_list
+
+        if not hasattr(self, 'cutoff'):
+            self.set_cutoff()
+            cutoff = self.cutoff
+
+        atoms = self.to_ase(resort=False)
+        (id1, id2, shifts) = neighbor_list('ijS', atoms, cutoff)
+
+        self.lattice = self.lattice.scale(1.5)
+        matrix = self.lattice.matrix
+        numIons = []
+        species = []
+        sites = []
+        count = 0
+        for site in self.atom_sites:
+            sp = site.specie
+            if sp in dicts.keys():
+                if len(dicts[sp]) == 1:
+                    e = dicts[sp][0]
+                    sites.append(site.substitute_with_single(e))
+                    if e in species:
+                        id = species.index(e)
+                        numIons[id] += site.wp.multiplicity
+                    else:
+                        species.append(e)
+                        numIons.append(site.wp.multiplicity)
+                else:
+                    eles = dicts[sp]
+                    ids = id2[id1==count] # index of ids
+                    neighbors = atoms.positions[ids] + shifts[id1==count].dot(atoms.cell)
+                    direction = neighbors[1] - neighbors[0]
+                    direction /= np.linalg.norm(direction)
+                    s1, s2 = site.substitute_with_linear(eles, direction, matrix)
+                    for e in eles:
+                        if e in species:
+                            id = species.index(e)
+                            numIons[id] += site.wp.multiplicity
+                        else:
+                            species.append(e)
+                            numIons.append(site.wp.multiplicity)
+                    sites.append(s1)
+                    sites.append(s2)
+            else:
+                sites.append(site)
+            count += site.wp.multiplicity
+
+        struc = self.copy()
+        struc.atom_sites = sites
+        struc.numIons = numIons
+        struc.species = species
+        struc.resort()
+        return struc
+
 
     def remove_water(self):
         """
         Remove water from hydrates
         """
         molecules = []
         numMols = []
```

### Comparing `pyxtal-0.5.7/pyxtal/block_crystal.py` & `pyxtal-0.5.8/pyxtal/block_crystal.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/constants.py` & `pyxtal-0.5.8/pyxtal/constants.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/crystal.py` & `pyxtal-0.5.8/pyxtal/crystal.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/HM_Full.csv` & `pyxtal-0.5.8/pyxtal/database/HM_Full.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/atomic_scattering_params.json` & `pyxtal-0.5.8/pyxtal/database/atomic_scattering_params.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/bonds.json` & `pyxtal-0.5.8/pyxtal/database/bonds.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/bug.json` & `pyxtal-0.5.8/pyxtal/database/bug.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/0-G62.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/0-G62.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/1-G59.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/1-G59.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/2-G71.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/2-G71.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/3-G139.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/3-G139.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/4-G225.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/4-G225.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/ACBNZA01.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/ACBNZA01.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/AXOSOW01.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/AXOSOW01.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/Al2SiO5_mp-4753_symmetrized.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/Al2SiO5_mp-4753_symmetrized.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/BTO-Amm2.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/BTO-Amm2.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/BTO.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/BTO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/CuAu_mp-582681_symmetrized.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/CuAu_mp-582681_symmetrized.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/FAU.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/FAU.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/Fd3.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/Fd3.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/Fd3.vasp` & `pyxtal-0.5.8/pyxtal/database/cifs/Fd3.vasp`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/Fd3m.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/Fd3m.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/GUMMUW.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/GUMMUW.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/GeF2.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/GeF2.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/HAHCOI.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/HAHCOI.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/I4_132.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/I4_132.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/JAPWIH.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/JAPWIH.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/LAGNAL.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/LAGNAL.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/LUFHAW.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/LUFHAW.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/LiCs.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/LiCs.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/MERQIM.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/MERQIM.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/MPWO.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/MPWO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/NaCl.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/NaCl.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/NaSb3F10.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/NaSb3F10.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/NbO2.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/NbO2.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/NiS-Cm.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/NiS-Cm.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/P3_112.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/P3_112.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/P4_332.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/P4_332.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/P6_422.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/P6_422.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/PAHYON01.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/PAHYON01.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/PPO.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/PPO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/PVO.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/PVO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/Pm3.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/Pm3.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/R-3.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/R-3.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/R-3c.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/R-3c.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/R32.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/R32.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/TMPPIO03.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/TMPPIO03.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/WEXBOS.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/WEXBOS.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/YICMOP.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/YICMOP.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/anthracene.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/anthracene.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/aspirin-c.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/aspirin-c.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/aspirin.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/aspirin.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/benzene.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/benzene.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/bug.vasp` & `pyxtal-0.5.8/pyxtal/database/cifs/bug.vasp`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/coumarin.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/coumarin.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/dist_6_0.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/dist_6_0.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/dist_6_1.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/dist_6_1.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/gdh.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/gdh.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/ht_KNbBO.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/ht_KNbBO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/ht_cristobalite.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/ht_cristobalite.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/ht_quartz.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/ht_quartz.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/ice.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/ice.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/lt_KNbBO.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/lt_KNbBO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/lt_cristobalite.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/lt_cristobalite.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/lt_quartz.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/lt_quartz.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/naphthalene.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/naphthalene.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/resorcinol.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/resorcinol.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/cifs/xxvi.cif` & `pyxtal-0.5.8/pyxtal/database/cifs/xxvi.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/clusters.json` & `pyxtal-0.5.8/pyxtal/database/clusters.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/collection.py` & `pyxtal-0.5.8/pyxtal/database/collection.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/element.py` & `pyxtal-0.5.8/pyxtal/database/element.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/k_subgroup.json` & `pyxtal-0.5.8/pyxtal/database/k_subgroup.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/layer.csv` & `pyxtal-0.5.8/pyxtal/database/layer.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/layer_generators.csv` & `pyxtal-0.5.8/pyxtal/database/layer_generators.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/layer_symmetry.csv` & `pyxtal-0.5.8/pyxtal/database/layer_symmetry.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/molecules.json` & `pyxtal-0.5.8/pyxtal/database/molecules.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/point.csv` & `pyxtal-0.5.8/pyxtal/database/point.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/point_generators.csv` & `pyxtal-0.5.8/pyxtal/database/point_generators.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/point_symmetry.csv` & `pyxtal-0.5.8/pyxtal/database/point_symmetry.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/rod.csv` & `pyxtal-0.5.8/pyxtal/database/rod.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/rod_generators.csv` & `pyxtal-0.5.8/pyxtal/database/rod_generators.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/rod_symmetry.csv` & `pyxtal-0.5.8/pyxtal/database/rod_symmetry.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/symbols.json` & `pyxtal-0.5.8/pyxtal/database/symbols.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/t_subgroup.json` & `pyxtal-0.5.8/pyxtal/database/t_subgroup.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/wyckoff_generators.csv` & `pyxtal-0.5.8/pyxtal/database/wyckoff_generators.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/wyckoff_list.csv` & `pyxtal-0.5.8/pyxtal/database/wyckoff_list.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/wyckoff_sets.json` & `pyxtal-0.5.8/pyxtal/database/wyckoff_sets.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/database/wyckoff_symmetry.csv` & `pyxtal-0.5.8/pyxtal/database/wyckoff_symmetry.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/db.py` & `pyxtal-0.5.8/pyxtal/db.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/descriptor.py` & `pyxtal-0.5.8/pyxtal/descriptor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 Module for crystal packing descriptor from energy decomposition
 """
 import numpy as np
-import pyshtools as pysh
 from scipy.stats import qmc
 from scipy.spatial.transform import Rotation
 from scipy.optimize import minimize
 from scipy.special import sph_harm
 
 def _qlm(dists, l=4):
     '''
@@ -228,19 +227,21 @@
             Coefficients of the spherican harmonic
 
         chi2: float
             The residual sum of squares misfit for an overdetermined inversion.
     """
     thetas, phis, vals = pts[:,0], pts[:,1], pts[:,2]
     phis = np.degrees(phis)
+    # shift from (0, 180) to (-90, 90)
     thetas = np.degrees(thetas)
+    thetas -= 90
 
     # if thetas is within [0, 180]
-    if abs(thetas.min()) < 1e-3: thetas -= 90
-    #print('check thetas', thetas.min())
+    #print('check thetas', thetas.min(), thetas.max())
+    #if abs(thetas.min()) < 1e-3: thetas -= 90
     cilm, chi2 = SHExpandLSQ(vals, thetas, phis, l_max, norm=norm, csphase=csphase)
 
     return cilm, chi2
 
 def get_alignment(pts, degrees=True):
     """
     Here we define the equator is the plane with three most important neighbors.
@@ -280,14 +281,16 @@
         xtal: pyxtal structure
         model: 'molecule' or 'contact'
         max_d: maximum intermolecular distances
         lmax: maximum bandwidth for spherical harmonic expansion
         sigma: Gaussian width to project into the unit sphere
         N: number of grid points on the unit sphere
     """
+    import pyshtools as pysh
+
     def __init__(self, xtal, model='molecule', max_d=10, 
         factor=2.2, lmax=13, sigma=0.1, N=10000):
 
         for i in range(len(xtal.mol_sites)):
             try:
                 numbers = xtal.mol_sites[i].molecule.mol.atomic_numbers
                 if numbers.count(7)>0 or numbers.count(8)>0:
```

### Comparing `pyxtal-0.5.7/pyxtal/elasticity.py` & `pyxtal-0.5.8/pyxtal/elasticity.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/interface/LJ.py` & `pyxtal-0.5.8/pyxtal/interface/LJ.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/interface/dftb.py` & `pyxtal-0.5.8/pyxtal/interface/dftb.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
     #pbc
     #print(calc_type, kwargs)
     return kwargs
 
 
 def DFTB_relax(struc, skf_dir, opt_cell=False, step=500, \
                fmax=0.1, kresol=0.10, folder='tmp', disp='D3', \
-               mask=None, symmetrize=True, logfile=None):
+               mask=None, symmetrize=True, logfile=None, use_omp=False):
     """
     DFTB optimizer based on ASE
 
     Args:
         struc: ase atoms object
         mode: [`single`, `relax`, `vc_relax`] (str)
         step: optimization steps (int)
@@ -170,15 +170,15 @@
     if not os.path.exists(folder):
         os.makedirs(folder)
     cwd = os.getcwd()
     os.chdir(folder)
 
     kpts = Kgrid(struc, kresol)
     atom_types = set(struc.get_chemical_symbols())
-    kwargs = make_Hamiltonian(skf_dir, atom_types, disp, kpts)
+    kwargs = make_Hamiltonian(skf_dir, atom_types, disp, kpts, use_omp=use_omp)
 
     calc = Dftb(label='test',
                 atoms=struc,
                 kpts=kpts,
                 **kwargs,
                 )
     struc.set_calculator(calc)
@@ -195,14 +195,15 @@
     try:
         dyn.run(fmax=fmax, steps=step)
         os.remove('dftb_pin.hsd')
         os.remove('geo_end.gen')
         os.remove('charges.bin')
     except:
         print("Problem in DFTB calculation")
+        struc = None
     os.chdir(cwd)
     return struc
 
 def DFTB_SCF(struc, skf_dir, kresol=0.10, folder='tmp', disp=None, filename=None):
     """
     DFTB SCF to get band structure
```

### Comparing `pyxtal-0.5.7/pyxtal/interface/gulp.py` & `pyxtal-0.5.8/pyxtal/interface/gulp.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     steps (int): relaxation steps
     symm (bool): whether or not impose the symmetry
     """
 
     def __init__(self, struc, label="_", path='tmp', ff='reax', \
                  pstress=None, opt='conp', steps=1000, exe='gulp',\
                  input='gulp.in', output='gulp.log', dump=None,
-                 symmetry=False):
+                 symmetry=False, labels=None):
 
         if isinstance(struc, pyxtal):
             self.pyxtal = struc
             self.species = struc.species
             struc = struc.to_ase(resort=False)
         else:
             self.pyxtal = None
@@ -37,18 +37,19 @@
             self.lattice = Lattice.from_matrix(struc.cell)
             self.frac_coords = struc.get_scaled_positions()
             self.sites = struc.get_chemical_symbols()
             self.species = None
         else:
             raise NotImplementedError("only support ASE atoms object")
         
-        self.symmetry = symmetry
+        self.symmetry = symmetry#; print(self.pyxtal.lattice.ltype)
         self.structure = struc
         self.pstress= pstress
         self.label = label
+        self.labels = labels
         self.ff = ff
         self.opt = opt
         self.exe = exe
         self.steps = steps
         self.folder = path  
         if not os.path.exists(self.folder):
             os.makedirs(self.folder)
@@ -61,14 +62,23 @@
         self.stress = None
         self.forces = None
         self.positions = None
         self.optimized = False
         self.cputime = 0
         self.error = False
 
+    def set_catlow(self):
+        """
+        set the atomic label for catlow potentials
+        O_O2- general O2- species
+        O_OH oxygen in hydroxyl group
+        H_OH hydrogen in hydroxyl group
+        """
+        pass
+
     def run(self, clean=True):
         self.write()
         self.execute()
         self.read()
         if clean:
             self.clean()
 
@@ -119,45 +129,71 @@
             f.write('\ncell\n')
             f.write('{:12.6f}{:12.6f}{:12.6f}{:12.6f}{:12.6f}{:12.6f}\n'.format(\
                     a, b, c, alpha, beta, gamma))
             f.write('\nfractional\n')
             
             symbols = []
             if self.symmetry and self.pyxtal is not None:
-                # Use pyxta here
+                # Use pyxtal here
                 for site in self.pyxtal.atom_sites:
                     symbol, coord = site.specie, site.position
                     f.write('{:4s} {:12.6f} {:12.6f} {:12.6f} core \n'.format(symbol, *coord))
+                    if self.ff == 'catlow' and symbol == 'O':
+                        f.write('{:4s} {:12.6f} {:12.6f} {:12.6f} shell \n'.format(symbol, *coord))
+
+
+                # Tested for all space groups
                 f.write('\nspace\n{:d}\n'.format(self.pyxtal.group.number))
+                f.write('\norigin\n0 0 0\n')
             else:
-                # all coordinates
+                # All coordinates
                 for coord, site in zip(self.frac_coords, self.sites):
                     f.write('{:4s} {:12.6f} {:12.6f} {:12.6f} core \n'.format(site, *coord))
             if self.species is not None:
                 species = self.structure.species
             else:
                 species = list(set(self.sites))
 
             f.write('\nSpecies\n')
-            for specie in species:
-                f.write('{:4s} core {:4s}\n'.format(specie, specie))
+            if self.labels is not None:
+                for specie in species:
+                    if specie in self.labels.keys():
+                        sp = self.labels[specie]
+                        f.write('{:4s} core {:s}\n'.format(specie, sp))
+                    else:
+                        f.write('{:4s} core {:4s}\n'.format(specie, specie))
+            else:
+                for specie in species:
+                    if self.ff == 'catlow' and specie == 'O':
+                        f.write('O    core O_O2- core\n')
+                        f.write('O    shell O_O2- shell\n')
+                    else:
+                        f.write('{:4s} core {:4s}\n'.format(specie, specie))
 
             f.write('\nlibrary {:s}\n'.format(self.ff))
             f.write('ewald 10.0\n')
             #f.write('switch rfo gnorm 1.0\n')
             #f.write('switch rfo cycle 0.03\n')
             if self.opt != "single":
                 f.write('maxcycle {:d}\n'.format(self.steps))
             if self.pstress is not None:
                 f.write("pressure {:6.3f}\n".format(self.pstress))
             if self.dump is not None:
                 f.write('output cif {:s}\n'.format(self.dump))
 
 
     def read(self):
+        # for symmetry case
+        lattice_para = None
+        lattice_vector = None
+        if self.pyxtal is not None:
+            ltype = self.pyxtal.lattice.ltype
+        else:
+            ltype = 'triclinic'
+
         with open(self.output, 'r') as f:
             lines = f.readlines()
         try: 
             for i, line in enumerate(lines):
                 if self.symmetry and self.pyxtal.group.symbol[0] != 'P':
                     m = re.match(r'\s*Non-primitive unit cell\s*=\s*(\S+)\s*eV', line)
                 elif self.pstress is None or self.pstress == 0:
@@ -241,40 +277,56 @@
                         xyz = lines[s].split()[3:6]
                         XYZ = [float(x) for x in xyz]
                         positions.append(XYZ)
                         species.append(lines[s].split()[1])
                     #if len(species) != len(self.sites):
                     #    print("Warning", len(species), len(self.sites))
                     self.frac_coords = np.array(positions)
-
                 elif line.find('Final Cartesian lattice vectors') != -1:
                     lattice_vectors = np.zeros((3,3))
                     s = i + 2
                     for j in range(s, s+3):
                         temp=lines[j].split()
                         for k in range(3):
                             lattice_vectors[j-s][k]=float(temp[k])
-                    self.lattice = Lattice.from_matrix(lattice_vectors)
-                    if self.pyxtal is not None:
-                        self.pyxtal.lattice = self.lattice
-            if np.isnan(self.energy):
-                self.error = True
-                self.energy = None
-                print("GULP calculation is wrong, reading------")
+                    lattice_vector = Lattice.from_matrix(lattice_vectors, ltype=ltype)
+
+                elif line.find('Non-primitive lattice parameters') != -1:
+                    s = i + 2
+                    temp = lines[s].split()
+                    a, b, c = float(temp[2]), float(temp[5]), float(temp[8])
+                    temp = lines[s+1].split()
+                    alpha, beta, gamma = float(temp[1]), float(temp[3]), float(temp[5])
+                    lattice_para = Lattice.from_para(a, b, c, alpha, beta, gamma, ltype)
         except:
             self.error = True
             self.energy = None
-            print("GULP calculation is wrong")
+        if lattice_para is not None:
+            self.lattice = lattice_para
+        elif lattice_vector is not None:
+            self.lattice = lattice_vector
+        else:
+            self.error = True
+            self.energy = None
+
+        if self.pyxtal is not None:
+            self.pyxtal.lattice = self.lattice
+
+        if self.energy is None or np.isnan(self.energy):
+            self.error = True
+            self.energy = None
+            print("GULP calculation is wrong, reading------")
 
 def single_optimize(struc, ff, steps=1000, pstress=None, opt="conp", 
                     exe="gulp", path="tmp", label="_", clean=True,
-                    symmetry=False):
+                    symmetry=False, labels=None):
 
     calc = GULP(struc, steps=steps, label=label, path=path, 
-                pstress=pstress, ff=ff, opt=opt, symmetry=symmetry)
+                pstress=pstress, ff=ff, opt=opt, 
+                symmetry=symmetry, labels=labels)
 
     calc.run(clean=clean)
 
     if calc.error:
         print("GULP error in single optimize")
         return None, None, 0, True
     else:
```

### Comparing `pyxtal-0.5.7/pyxtal/interface/lammpslib.py` & `pyxtal-0.5.8/pyxtal/interface/lammpslib.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/interface/vasp.py` & `pyxtal-0.5.8/pyxtal/interface/vasp.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/interface/vasprun.py` & `pyxtal-0.5.8/pyxtal/interface/vasprun.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/io.py` & `pyxtal-0.5.8/pyxtal/io.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/lattice.py` & `pyxtal-0.5.8/pyxtal/lattice.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,14 +168,18 @@
         return deepcopy(self)
 
     def get_lengths(self):
         mat = create_matrix(self.PBC, True)
         mat = np.dot(mat, self.matrix)
         return mat, np.linalg.norm(mat, axis=1)
 
+    def scale(self, factor=1.1):
+        matrix = self.matrix
+        return Lattice.from_matrix(matrix*factor, ltype=self.ltype)
+
     def get_permutation_matrices(self):
         """
         Return the possible permutation matrices that donot violate the symmetry
         """
         if self.ltype in ["monoclinic"]: #permutation between a and c
             return np.array([
                              [[1,0,0],[0,1,0],[0,0,1]], #self
```

### Comparing `pyxtal-0.5.7/pyxtal/molecular_crystal.py` & `pyxtal-0.5.8/pyxtal/molecular_crystal.py`

 * *Files 1% similar despite different names*

```diff
@@ -409,17 +409,20 @@
                     self.thickness < 0.1:
                         pt[-1] = 0.5
 
                     ms0 = self._set_orientation(pyxtal_mol, pt, oris, wp)
                     if ms0 is not None:
                         # Check current WP against existing WP's
                         passed_wp_check = True
-                        for ms1 in mol_sites_tmp + mol_wyks:
+                        #print("Checking", ms0)
+                        for ms1 in mol_wyks + mol_sites_tmp:
                             if not ms0.short_dist_with_wp2(ms1, tm=self.tol_matrix):
                                 passed_wp_check = False
+                            #else:
+                            #    print("passing", ms1)
 
                         if passed_wp_check:
                             if sites_list is not None:
                                 sites_list.pop(0)
 
                             ms0.type = id
                             mol_sites_tmp.append(ms0)
```

### Comparing `pyxtal-0.5.7/pyxtal/molecule.py` & `pyxtal-0.5.8/pyxtal/molecule.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/msg.py` & `pyxtal-0.5.8/pyxtal/msg.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/operations.py` & `pyxtal-0.5.8/pyxtal/operations.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/optimize/fire.py` & `pyxtal-0.5.8/pyxtal/optimize/fire.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/optimize/fire2.py` & `pyxtal-0.5.8/pyxtal/optimize/fire2.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/optimize/myscipy_optimize.py` & `pyxtal-0.5.8/pyxtal/optimize/myscipy_optimize.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/potentials/CuAg.eam.alloy` & `pyxtal-0.5.8/pyxtal/potentials/CuAg.eam.alloy`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/potentials/LJ_cluster.py` & `pyxtal-0.5.8/pyxtal/potentials/LJ_cluster.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/potentials/Si.tersoff` & `pyxtal-0.5.8/pyxtal/potentials/Si.tersoff`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/potentials/SiCGe.tersoff` & `pyxtal-0.5.8/pyxtal/potentials/SiCGe.tersoff`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/representation.py` & `pyxtal-0.5.8/pyxtal/representation.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/supergroup.py` & `pyxtal-0.5.8/pyxtal/supergroup.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/symmetry.py` & `pyxtal-0.5.8/pyxtal/symmetry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1126,15 +1126,15 @@
                             for _index in _indexs],[]))] \
                             for i in range(len_k) if kdict['subgroup'][i]!=tail[2]]
                 for n in next_steps:
                     _potential.append(deepcopy(p)+n)
             potential=deepcopy(_potential)
 
             for p in deepcopy(potential):
-                   #Check there's only one wp.  #Check that the 1 wp is the general position
+                #Check there's only one wp.  #Check that the 1 wp is the general position
                 if (len(set(p[-1][3]))==1) and (p[-1][3][0][-1]==Group(p[-1][2])[0].letter):
                     solutions.append(deepcopy(p)[1:])
                     potential.remove(p)
 
         return solutions
 
     def short_path_to_general_wp(self, index=1, t_only=False):
```

### Comparing `pyxtal-0.5.7/pyxtal/test_all.py` & `pyxtal-0.5.8/pyxtal/test_all.py`

 * *Files 2% similar despite different names*

```diff
@@ -671,14 +671,45 @@
 
         for i in range(3):
             struc = pyxtal(molecular=True)
             struc.from_random(3, 10, [Li, ps4], [6, 2], 1.2, conventional=False)
             if struc.valid:
                 self.assertTrue(len(struc.to_pymatgen()) == 16)
 
+    def test_distance(self):
+        Ag_xyz = """1
+        AgC2N2H
+        Ag         4.30800        8.26300       -0.2200
+        """
+        
+        C2N2H7_xyz = """12
+        AgC2N2H
+        H          5.95800        5.80600       -0.9530
+        N          5.24100        6.16800       -1.1210
+        N          2.23200        6.99000       -0.6820
+        C          4.02900        5.47000       -1.5870
+        C          2.78500        5.61100       -0.6610
+        H          3.69300        5.63500       -2.5830
+        H          4.17400        4.42800       -1.6990
+        H          3.12700        5.50500        0.4260
+        H          2.05000        5.01200       -0.9300
+        H          1.96000        7.20500       -1.3860
+        H          1.59400        6.99200       -0.0710
+        """
+        with open('Ag.xyz', "w") as f:
+            f.write(Ag_xyz)
+        with open('C2N2H7.xyz', "w") as f:
+            f.write(C2N2H7_xyz)
+        
+        for i in range(10):
+            c = pyxtal(molecular=True)
+            c.from_random(3, 9, ['Ag.xyz', 'C2N2H7.xyz'], [12, 12])
+            short_bonds = c.check_short_distances(r=1.1)
+            self.assertTrue(len(short_bonds)==0)
+
     def test_molecular_2d(self):
         # print("test_molecular_2d")
         struc = pyxtal(molecular=True)
         struc.from_random(2, 20, ["H2O"])
         self.assertTrue(struc.valid)
 
     def test_molecular_1d(self):
```

### Comparing `pyxtal-0.5.7/pyxtal/tolerance.py` & `pyxtal-0.5.8/pyxtal/tolerance.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         Args:
             specie1/2: atomic number (int or float), name (str), symbol (str),
                 an Element object, or a pymatgen Specie object
 
         Returns:
             the tolerance between the provided pair of atomic species
         """
-        if self.prototype == "single_value":
+        if self.prototype == "single value":
             return self.matrix[0][0]
         index1 = Element.number_from_specie(specie1)
         index2 = Element.number_from_specie(specie2)
         if index1 is not None and index2 is not None:
             return self.matrix[index1][index2]
         else:
             return None
```

### Comparing `pyxtal-0.5.7/pyxtal/util.py` & `pyxtal-0.5.8/pyxtal/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -484,15 +484,16 @@
         s1, e1 = id*N_atoms, (id+1)*N_atoms
         s2, e2 = i*N_atoms, (i+1)*N_atoms
         pos1[s2:e2, :] += pos0[s1:e1, :] - shifts[i].dot(atoms.cell[:])
 
     atoms.set_positions(pos1)
     return atoms
 
-def generate_wp_lib(spg_list, composition, max_wp=None, min_wp=None):
+def generate_wp_lib(spg_list, composition, max_wp=None, min_wp=None, 
+                    max_fu=None, min_fu=None, N_max=1000):
     """
     Generate wps according to the composition constraint (e.g., SiO2)
 
     Args;
         - spg_list: list of space group choices
         - composition: chemical compositions [1, 2]
         - max_wp: the number of maximum wp sites
@@ -509,26 +510,31 @@
     if min_wp is None: min_wp = len(composition)
     #print(max_wp, min_wp)
     wps = []
     for sg in spg_list:
         g = Group(sg)
         lat_dof = g.get_lattice_dof()
         # determine the upper and lower limit 
-        min_repeat = max([int(len(g[-1])/min(composition)), 1])
-        max_repeat = max([int(len(g[0])/max(composition)), 1])
-        for i in range(min_repeat, max_repeat+1):
+        if min_fu is None: min_fu = max([int(len(g[-1])/min(composition)), 1])
+        if max_fu is None: max_fu = max([int(len(g[0])/max(composition)), 1])
+        count = 0
+        for i in range(max_fu, min_fu-1, -1):
             letters, _, wp_ids = g.list_wyckoff_combinations(
-                    composition*i, max_wp=max_wp, min_wp=min_wp)
+                    composition*i, max_wp=max_wp, 
+                    min_wp=min_wp, Nmax=100000)
             for j, wp in enumerate(wp_ids):
                 wp_dofs = 0
                 for wp0 in wp:
                     for id in wp0:
                         wp_dofs += g[id].get_dof()
-                #print(sg, wp, letters[i])
+                #print(sg, wp, letters[j])
                 wps.append((sg, wp, lat_dof + wp_dofs))
+            count += len(letters)
+            if count >= N_max:
+                break
     return wps 
  
 
 if __name__ == "__main__":
     from argparse import ArgumentParser
 
     parser = ArgumentParser()
```

### Comparing `pyxtal-0.5.7/pyxtal/viz.py` & `pyxtal-0.5.8/pyxtal/viz.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal/wyckoff_site.py` & `pyxtal-0.5.8/pyxtal/wyckoff_site.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Module for handling Wyckoff sites for both atom and molecule
 """
 
 # Standard Libraries
 import numpy as np
 from scipy.spatial.transform import Rotation as R
 from scipy.spatial.distance import cdist
+from copy import deepcopy
 
 # External Libraries
 from pymatgen.core import Molecule
 
 # PyXtal imports
 from pyxtal.tolerance import Tol_matrix
 from pyxtal.operations import (
@@ -57,14 +58,20 @@
         s += "Site [{:}]".format(self.wp.site_symm.replace(" ",""))
 
         return s
 
     def __repr__(self):
         return str(self)
 
+    def copy(self):
+        """
+        Simply copy the structure
+        """
+        return deepcopy(self)
+
     def save_dict(self):
         dict0 = {"position": self.position,
                  "specie": self.specie,
                  "wp": self.wp.save_dict(),
                 }
         return dict0
 
@@ -261,14 +268,48 @@
             dm = distance_matrix(ws1.coords, ws2.coords, lattice, PBC=ws1.PBC)
             # Check if any distances are less than the tolerance
             if (dm < tol).any():
                 return False
             else:
                 return True
 
+    def substitute_with_single(self, ele):
+        """
+        chemical substitution with another element
+
+        Args:
+            ele (str): e.g. 'Zn'
+        """
+        self.specie = ele
+        return self
+
+    def substitute_with_linear(self, eles, direction, lattice):
+        """
+        chemical substitution with another linear building block, e.g. CN
+
+        Args:
+            eles (str): e.g., ['C', 'N']
+            neighbors: two nearest neiboring atom xyz
+        """
+        bond_length = 1.4
+        #direction = neighbors[1] - neighbors[0]
+        #direction = np.dot(direction, lattice)
+        #direction /= np.linalg.norm(direction)
+
+        # Get the fraction coordinates
+        shift = np.dot(bond_length/2 * direction, np.linalg.inv(lattice))
+        site1 = self.copy()
+        site2 = self.copy()
+        site1.specie = eles[0]
+        site2.specie = eles[1]
+        site1.update(site1.position + shift)
+        site2.update(site2.position - shift)
+        return site1, site2
+        
+
 class mol_site:
     """
     Class for storing molecular Wyckoff positions and orientations within
     the molecular_crystal class. Each mol_site object represenents an
     entire Wyckoff position, not necessarily a single molecule.
     This is the molecular version of Wyckoff_site
 
@@ -457,16 +498,16 @@
                 center_relative -= np.floor(center_relative)
             center_absolute = np.dot(center_relative, self.lattice.matrix)
 
             # Rotate the molecule (Euclidean metric)
             #op2_m = self.wp.generators_m[point_index]
             op2_m = self.wp.get_euclidean_generator(self.lattice.matrix, point_index)
             rot = op2_m.affine_matrix[:3, :3].T
-            #NOTE=====the euclidean_generator has wrong translation vectors,
-            #but we don't care. This needs to be fixed later
+            # NOTE=====the euclidean_generator has wrong translation vectors,
+            # but we don't care. This needs to be fixed later
 
             #if self.diag and self.wp.index > 0:
             #    tau = op2.translation_vector
             #else:
             #    tau = op2_m.translation_vector
             tmp = np.dot(coord0, rot) #+ tau
 
@@ -678,15 +719,15 @@
         else:
             import pickle
             with open('wrong.pkl', "wb") as f:
                 pickle.dump([mol, self.mol], f)
                 mol.to(filename='Wrong.xyz', fmt='xyz')
                 self.mol.to(filename='Ref.xyz', fmt='xyz')
             raise ValueError("molecular connectivity changes! Exit")
-        #todo check if connectivty changed
+        # todo check if connectivty changed
 
     def _create_matrix(self, center=False, ignore=False):
         """
         Used for calculating distances in lattices with periodic boundary
         conditions. When multiplied with a set of points, generates additional
         points in cells adjacent to and diagonal to the original cell
 
@@ -699,15 +740,15 @@
         # QZ: This should be based on the occupation of current molecule
         if hasattr(self, 'ijk_lists'):
             ijk_lists = self.ijk_lists
         else:
             ijk_lists = []
             for id in range(3):
                 if self.PBC[id]:
-                    if not ignore and abc[id] > 20 and self.radius<10:
+                    if not ignore and abc[id] > 25 and self.radius < 10:
                         ijk_lists.append([0])
                     elif abc[id] < 7.0:
                         ijk_lists.append([-3, -2, -1, 0, 1, 2, 3])
                     else:
                         ijk_lists.append([-1, 0, 1])
                 else:
                     ijk_lists.append([0])
@@ -717,15 +758,15 @@
         else:
             matrix = []
         for i in ijk_lists[0]:
             for j in ijk_lists[1]:
                 for k in ijk_lists[2]:
                     if [i, j, k] != [0, 0, 0]:
                         matrix.append([i, j, k])
-        #In case a,b,c are all greater than 20
+        # In case a,b,c are all greater than 20
         if len(matrix) == 0:
             matrix = [[1,0,0]]
         return np.array(matrix, dtype=float)
 
 
     def get_distances(self, coord1, coord2, m2=None, center=True, ignore=False):
         """
@@ -739,23 +780,22 @@
             center: whether or not consider the self image for coord2
 
         Returns:
             distance matrix: [m1*m2*pbc, m1, m2]
             coord2 under PBC: [pbc, m2, 3]
         """
         m1 = len(coord1)
-        if m2 is None:
-            m2 = m1
+        if m2 is None: m2 = m1
         N2 = int(len(coord2)/m2)
 
-        #peridoic images
+        # peridoic images
         m = self._create_matrix(center, ignore) #PBC matrix
         coord2 = np.vstack([coord2 + v for v in m])
 
-        #absolute xyz
+        # absolute xyz
         coord1 = np.dot(coord1, self.lattice.matrix)
         coord2 = np.dot(coord2, self.lattice.matrix)
 
         d = cdist(coord1, coord2)
         d = d.T.reshape([len(m)*N2, m1, m2])
         return d, coord2.reshape([len(m)*N2, m2, 3])
 
@@ -794,23 +834,23 @@
     def get_min_dist(self):
         """
         Compute the minimum interatomic distance within the WP.
 
         Returns:
             minimum distance
         """
-        #Self image
+        # Self image
         ds, _ = self.get_dists_auto()
         min_dist = np.min(ds)
 
         if min_dist < 0.9:
-            #terminate earlier
+            # terminate earlier
             return min_dist
         else:
-            #Other molecules
+            # Other molecules
             if self.wp.multiplicity > 1:
                 ds, _ = self.get_dists_WP()
                 if min_dist > np.min(ds):
                     min_dist = np.min(ds)
             return min_dist
 
     def short_dist(self):
@@ -865,15 +905,17 @@
         else:
             coord1 = c2[:m_length2]
             coord2 = c1
             tols_matrix = wp2.molecule.get_tols_matrix(self.molecule, tm)
             m2 = m_length1
 
         # compute the distance matrix
-        d, _ = self.get_distances(coord1, coord2, m2)
+        d, _ = self.get_distances(coord1-np.floor(coord1), coord2-np.floor(coord2), m2)
+        #print("short dist", len(c1), len(c2), d.min())
+        
         if np.min(d) < np.max(tols_matrix):
             tols = np.min(d, axis=0)
             if (tols < tols_matrix).any():
                 return False
         return True
 
     def get_neighbors_auto(self, factor=1.1, max_d=4.0, ignore_E=True, detail=False, etol=-5e-2):
```

### Comparing `pyxtal-0.5.7/pyxtal/wyckoff_split.py` & `pyxtal-0.5.8/pyxtal/wyckoff_split.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/pyxtal.egg-info/PKG-INFO` & `pyxtal-0.5.8/pyxtal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxtal
-Version: 0.5.7
+Version: 0.5.8
 Summary: Python code for generation of crystal structures based on symmetry constraints.
 Home-page: https://github.com/qzhu2017/PyXtal
 Author: Scott Fredericks, Qiang Zhu
 Author-email: qiang.zhu@unlv.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyxtal-0.5.7/pyxtal.egg-info/SOURCES.txt` & `pyxtal-0.5.8/pyxtal.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -101,14 +101,15 @@
 pyxtal/database/cifs/Pn3m.vasp
 pyxtal/database/cifs/R-3.cif
 pyxtal/database/cifs/R-3c.cif
 pyxtal/database/cifs/R32.cif
 pyxtal/database/cifs/TMPPIO03.cif
 pyxtal/database/cifs/WEXBOS.cif
 pyxtal/database/cifs/YICMOP.cif
+pyxtal/database/cifs/__init__.py
 pyxtal/database/cifs/anthracene.cif
 pyxtal/database/cifs/aspirin-c.cif
 pyxtal/database/cifs/aspirin.cif
 pyxtal/database/cifs/benzene.cif
 pyxtal/database/cifs/bug.vasp
 pyxtal/database/cifs/coumarin.cif
 pyxtal/database/cifs/dist_6_0.cif
```

### Comparing `pyxtal-0.5.7/scripts/pyxtal_main.py` & `pyxtal-0.5.8/scripts/pyxtal_main.py`

 * *Files 15% similar despite different names*

```diff
@@ -87,14 +87,23 @@
         "--molecular",
         dest="molecular",
         action = 'store_true',
         default = False,
         help="molecular? default: False",
     )
 
+    parser.add_argument(
+        "-c",
+        "--conventional",
+        dest="conventional",
+        action = 'store_true',
+        default = False,
+        help="conventional setting? default: False",
+    )
+
     print_logo()
     options = parser.parse_args()
     sg = options.sg
     dimension = options.dimension
     if isinstance(sg, str) and sg.isnumeric():
         sg = int(sg)
     symbol, sg = get_symbol_and_number(sg, dimension)
@@ -115,27 +124,28 @@
         raise ValueError("Volume factor {:.2f} must be greater than 0.".format(factor))
 
     attempts = options.attempts
     outdir = options.outdir
     dimension = options.dimension
     thickness = options.thickness
     molecular = options.molecular
+    conventional = options.conventional
 
     if not os.path.exists(outdir):
         os.mkdir(outdir)
 
     for i in range(attempts):
         numIons0 = np.array(numIons)
-        rand_crystal = pyxtal(molecular=options.molecular)
+        rand_crystal = pyxtal(molecular=molecular)
         if dimension == 3:
-            rand_crystal.from_random(3, sg, system, numIons0, factor)
+            rand_crystal.from_random(3, sg, system, numIons0, factor, conventional=conventional)
         elif dimension == 2:
-            rand_crystal.from_random(2, sg, system, numIons0, factor, thickness)
+            rand_crystal.from_random(2, sg, system, numIons0, factor, thickness, conventional=conventional)
         elif dimension == 1:                                             
-            rand_crystal.from_random(1, sg, system, numIons0, factor, thickness)
+            rand_crystal.from_random(1, sg, system, numIons0, factor, thickness, conventional=conventional)
         if dimension == 0:
             rand_crystal.from_random(0, sg, system, numIons0, factor)
         # Output a cif or xyz file
         if dimension > 0:
             outpath = options.outdir + '/' + str(i) + '.cif'
         else:
             outpath = options.outdir + '/' + str(i) + '.xyz'
```

### Comparing `pyxtal-0.5.7/scripts/pyxtal_symmetry.py` & `pyxtal-0.5.8/scripts/pyxtal_symmetry.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.5.7/setup.py` & `pyxtal-0.5.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,13 +48,13 @@
         "pandas>=0.24.2",
         "networkx>=2.3",
         "py3Dmol>=0.8.0",
         'ase>=3.18.0',  #covered by pymatgen
         'numba>=0.55.2', #now supports numpy 1.22
         'scipy>=1.7.3',
         'importlib_metadata>=1.4',
-        'pyshtools==4.10',
+        'pyshtools>=4.10.3',
         #"openbabel>=3.0.0",
     ],
     python_requires=">=3.7, <=3.11", #add the restriction for now issue #189
     license="MIT",
 )
```

