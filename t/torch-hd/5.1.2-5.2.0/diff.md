# Comparing `tmp/torch-hd-5.1.2.tar.gz` & `tmp/torch-hd-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch-hd-5.1.2.tar", last modified: Wed Apr 26 05:09:51 2023, max compression
+gzip compressed data, was "torch-hd-5.2.0.tar", last modified: Fri Jul  7 22:49:30 2023, max compression
```

## Comparing `torch-hd-5.1.2.tar` & `torch-hd-5.2.0.tar`

### file list

```diff
@@ -1,181 +1,181 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:09:51.913807 torch-hd-5.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-26 05:09:39.000000 torch-hd-5.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-04-26 05:09:51.913807 torch-hd-5.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-04-26 05:09:39.000000 torch-hd-5.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 05:09:51.913807 torch-hd-5.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-26 05:09:39.000000 torch-hd-5.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:09:51.893807 torch-hd-5.1.2/torch_hd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-04-26 05:09:51.000000 torch-hd-5.1.2/torch_hd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-04-26 05:09:51.000000 torch-hd-5.1.2/torch_hd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 05:09:51.000000 torch-hd-5.1.2/torch_hd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-26 05:09:51.000000 torch-hd-5.1.2/torch_hd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 05:09:51.000000 torch-hd-5.1.2/torch_hd.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:09:51.893807 torch-hd-5.1.2/torchhd/
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:09:51.909807 torch-hd-5.1.2/torchhd/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)    11149 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/abalone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/acute_inflammation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/acute_nephritis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/adult.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/airfoil_self_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/annealing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/arrhythmia.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/audiology_std.py
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/balance_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/balloons.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/bank.py
--rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/beijing_air_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/blood.py
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/breast_cancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/breast_cancer_wisc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/breast_cancer_wisc_diag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/breast_cancer_wisc_prog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/breast_tissue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/car.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/cardiotocography_10clases.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/cardiotocography_3clases.py
--rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/ccpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/chess_krvk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/chess_krvkp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/congressional_voting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/conn_bench_sonar_mines_rocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/conn_bench_vowel_deterding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/connect_4.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/contrac.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/credit_approval.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/cylinder_bands.py
--rw-r--r--   0 runner    (1001) docker     (123)    20384 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/dermatology.py
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/echocardiogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/ecoli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/emg_hand_gestures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/energy_y1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/energy_y2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/european_languages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/fertility.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/glass.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/haberman_survival.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/hayes_roth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/heart_cleveland.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/heart_hungarian.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/heart_switzerland.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/heart_va.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/hepatitis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/hill_valley.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/horse_colic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/ilpd_indian_liver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/image_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/ionosphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/iris.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/isolet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/led_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/lenses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/letter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/libras.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/low_res_spect.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/lung_cancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/lymphography.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/magic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/mammographic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/miniboone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/molec_biol_promoter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/molec_biol_splice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/monks_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/monks_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/monks_3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/mushroom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/musk_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/musk_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/nursery.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/oocytes_merluccius_nucleus_4d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/oocytes_merluccius_states_2f.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/oocytes_trisopterus_nucleus_2f.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/oocytes_trisopterus_states_5b.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/optical.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/ozone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/page_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/pamap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/parkinsons.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/pendigits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/pima.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/pittsburg_bridges_material.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/pittsburg_bridges_rel_l.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/pittsburg_bridges_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/pittsburg_bridges_t_or_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/pittsburg_bridges_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/planning.py
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/plant_margin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/plant_shape.py
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/plant_texture.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/post_operative.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/primary_tumor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/ringnorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/seeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/semeion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/soybean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/spambase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/spect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/spectf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/statlog_australian_credit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/statlog_german_credit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/statlog_heart.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/statlog_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/statlog_landsat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/statlog_shuttle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/statlog_vehicle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/steel_plates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/synthetic_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/teaching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/thyroid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/tic_tac_toe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/titanic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/trains.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/twonorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/ucihar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/vertebral_column_2clases.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/vertebral_column_3clases.py
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/wall_following.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/waveform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/waveform_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/wine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/wine_quality_red.py
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/wine_quality_white.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/yeast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/datasets/zoo.py
--rw-r--r--   0 runner    (1001) docker     (123)    38939 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)    59891 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    13714 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    38319 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:09:51.913807 torch-hd-5.1.2/torchhd/tensors/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/tensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/tensors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17175 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/tensors/bsc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17047 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/tensors/fhrr.py
--rw-r--r--   0 runner    (1001) docker     (123)    15142 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/tensors/hrr.py
--rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/tensors/map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:09:51.889807 torch-hd-5.1.2/torchhd/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:09:51.913807 torch-hd-5.1.2/torchhd/tests/basis_hv/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/tests/basis_hv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/tests/basis_hv/test_base_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/tests/basis_hv/test_circular_hv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/tests/basis_hv/test_empty_hv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/tests/basis_hv/test_identity_hv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/tests/basis_hv/test_level_hv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/tests/basis_hv/test_random_hv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:09:51.913807 torch-hd-5.1.2/torchhd/tests/structures/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/tests/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/tests/structures/test_distinct_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/tests/structures/test_fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/tests/structures/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/tests/structures/test_hashtable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/tests/structures/test_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/tests/structures/test_multiset.py
--rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/tests/structures/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/tests/structures/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-26 05:09:39.000000 torch-hd-5.1.2/torchhd/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:49:30.546485 torch-hd-5.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-07 22:49:20.000000 torch-hd-5.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-07-07 22:49:30.546485 torch-hd-5.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-07 22:49:20.000000 torch-hd-5.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 22:49:30.546485 torch-hd-5.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-07 22:49:20.000000 torch-hd-5.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:49:30.526485 torch-hd-5.2.0/torch_hd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-07-07 22:49:30.000000 torch-hd-5.2.0/torch_hd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-07-07 22:49:30.000000 torch-hd-5.2.0/torch_hd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 22:49:30.000000 torch-hd-5.2.0/torch_hd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-07 22:49:30.000000 torch-hd-5.2.0/torch_hd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 22:49:30.000000 torch-hd-5.2.0/torch_hd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:49:30.530485 torch-hd-5.2.0/torchhd/
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:49:30.546485 torch-hd-5.2.0/torchhd/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)    11149 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/abalone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/acute_inflammation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/acute_nephritis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/adult.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/airfoil_self_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/annealing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/arrhythmia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/audiology_std.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/balance_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/balloons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/bank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/beijing_air_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/blood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/breast_cancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/breast_cancer_wisc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/breast_cancer_wisc_diag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/breast_cancer_wisc_prog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/breast_tissue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/car.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/cardiotocography_10clases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/cardiotocography_3clases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/ccpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/chess_krvk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/chess_krvkp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/congressional_voting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/conn_bench_sonar_mines_rocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/conn_bench_vowel_deterding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/connect_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/contrac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/credit_approval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/cylinder_bands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20384 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/dermatology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/echocardiogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/ecoli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/emg_hand_gestures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/energy_y1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/energy_y2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/european_languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/fertility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/glass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/haberman_survival.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/hayes_roth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/heart_cleveland.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/heart_hungarian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/heart_switzerland.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/heart_va.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/hepatitis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/hill_valley.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/horse_colic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/ilpd_indian_liver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/image_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/ionosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/iris.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/isolet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/led_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/lenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/letter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/libras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/low_res_spect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/lung_cancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/lymphography.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/mammographic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/miniboone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/molec_biol_promoter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/molec_biol_splice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/monks_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/monks_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/monks_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/mushroom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/musk_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/musk_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/nursery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/oocytes_merluccius_nucleus_4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/oocytes_merluccius_states_2f.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/oocytes_trisopterus_nucleus_2f.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/oocytes_trisopterus_states_5b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/optical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/ozone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/page_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/pamap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/parkinsons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/pendigits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/pima.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/pittsburg_bridges_material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/pittsburg_bridges_rel_l.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/pittsburg_bridges_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/pittsburg_bridges_t_or_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/pittsburg_bridges_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/planning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/plant_margin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/plant_shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/plant_texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/post_operative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/primary_tumor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/ringnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/seeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/semeion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/soybean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/spambase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/spect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/spectf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/statlog_australian_credit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/statlog_german_credit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/statlog_heart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/statlog_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/statlog_landsat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/statlog_shuttle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/statlog_vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/steel_plates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/synthetic_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/teaching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/thyroid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/tic_tac_toe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/titanic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/trains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/twonorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/ucihar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/vertebral_column_2clases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/vertebral_column_3clases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/wall_following.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/waveform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/waveform_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/wine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/wine_quality_red.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/wine_quality_white.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/yeast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/zoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48690 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59891 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13714 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38319 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:49:30.546485 torch-hd-5.2.0/torchhd/tensors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tensors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17175 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tensors/bsc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17047 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tensors/fhrr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15142 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tensors/hrr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tensors/map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:49:30.526485 torch-hd-5.2.0/torchhd/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:49:30.546485 torch-hd-5.2.0/torchhd/tests/basis_hv/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tests/basis_hv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tests/basis_hv/test_base_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tests/basis_hv/test_circular_hv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tests/basis_hv/test_empty_hv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tests/basis_hv/test_identity_hv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tests/basis_hv/test_level_hv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tests/basis_hv/test_random_hv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:49:30.546485 torch-hd-5.2.0/torchhd/tests/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tests/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tests/structures/test_distinct_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tests/structures/test_fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tests/structures/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tests/structures/test_hashtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tests/structures/test_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tests/structures/test_multiset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tests/structures/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tests/structures/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/version.py
```

### Comparing `torch-hd-5.1.2/LICENSE` & `torch-hd-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/PKG-INFO` & `torch-hd-5.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-hd
-Version: 5.1.2
+Version: 5.2.0
 Summary: Torchhd is a Python library for Hyperdimensional Computing and Vector Symbolic Architectures
 Home-page: https://github.com/hyperdimensional-computing/torchhd
 License: MIT
 Project-URL: Source, https://github.com/hyperdimensional-computing/torchhd
 Project-URL: Documentation, https://torchhd.readthedocs.io
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torch-hd Version: 5.1.2 Summary: Torchhd is a
+Metadata-Version: 2.1 Name: torch-hd Version: 5.2.0 Summary: Torchhd is a
 Python library for Hyperdimensional Computing and Vector Symbolic Architectures
 Home-page: https://github.com/hyperdimensional-computing/torchhd License: MIT
 Project-URL: Source, https://github.com/hyperdimensional-computing/torchhd
 Project-URL: Documentation, https://torchhd.readthedocs.io Requires-Python:
 >=3.6, <4 Description-Content-Type: text/markdown License-File: LICENSE
   [GitHub_license] [pypi_version] [conda_version] [tests_status][PRs Welcome]
                                 [Torchhd_logo]
```

### Comparing `torch-hd-5.1.2/README.md` & `torch-hd-5.2.0/README.md`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/setup.py` & `torch-hd-5.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torch_hd.egg-info/PKG-INFO` & `torch-hd-5.2.0/torch_hd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-hd
-Version: 5.1.2
+Version: 5.2.0
 Summary: Torchhd is a Python library for Hyperdimensional Computing and Vector Symbolic Architectures
 Home-page: https://github.com/hyperdimensional-computing/torchhd
 License: MIT
 Project-URL: Source, https://github.com/hyperdimensional-computing/torchhd
 Project-URL: Documentation, https://torchhd.readthedocs.io
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torch-hd Version: 5.1.2 Summary: Torchhd is a
+Metadata-Version: 2.1 Name: torch-hd Version: 5.2.0 Summary: Torchhd is a
 Python library for Hyperdimensional Computing and Vector Symbolic Architectures
 Home-page: https://github.com/hyperdimensional-computing/torchhd License: MIT
 Project-URL: Source, https://github.com/hyperdimensional-computing/torchhd
 Project-URL: Documentation, https://torchhd.readthedocs.io Requires-Python:
 >=3.6, <4 Description-Content-Type: text/markdown License-File: LICENSE
   [GitHub_license] [pypi_version] [conda_version] [tests_status][PRs Welcome]
                                 [Torchhd_logo]
```

### Comparing `torch-hd-5.1.2/torch_hd.egg-info/SOURCES.txt` & `torch-hd-5.2.0/torch_hd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/__init__.py` & `torch-hd-5.2.0/torchhd/__init__.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/__init__.py` & `torch-hd-5.2.0/torchhd/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/abalone.py` & `torch-hd-5.2.0/torchhd/datasets/abalone.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/acute_inflammation.py` & `torch-hd-5.2.0/torchhd/datasets/acute_inflammation.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/acute_nephritis.py` & `torch-hd-5.2.0/torchhd/datasets/acute_nephritis.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/adult.py` & `torch-hd-5.2.0/torchhd/datasets/adult.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/airfoil_self_noise.py` & `torch-hd-5.2.0/torchhd/datasets/airfoil_self_noise.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/annealing.py` & `torch-hd-5.2.0/torchhd/datasets/annealing.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/arrhythmia.py` & `torch-hd-5.2.0/torchhd/datasets/arrhythmia.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/audiology_std.py` & `torch-hd-5.2.0/torchhd/datasets/audiology_std.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/balance_scale.py` & `torch-hd-5.2.0/torchhd/datasets/balance_scale.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/balloons.py` & `torch-hd-5.2.0/torchhd/datasets/balloons.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/bank.py` & `torch-hd-5.2.0/torchhd/datasets/bank.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/beijing_air_quality.py` & `torch-hd-5.2.0/torchhd/datasets/beijing_air_quality.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/blood.py` & `torch-hd-5.2.0/torchhd/datasets/blood.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/breast_cancer.py` & `torch-hd-5.2.0/torchhd/datasets/breast_cancer.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/breast_cancer_wisc.py` & `torch-hd-5.2.0/torchhd/datasets/breast_cancer_wisc.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/breast_cancer_wisc_diag.py` & `torch-hd-5.2.0/torchhd/datasets/breast_cancer_wisc_diag.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/breast_cancer_wisc_prog.py` & `torch-hd-5.2.0/torchhd/datasets/breast_cancer_wisc_prog.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/breast_tissue.py` & `torch-hd-5.2.0/torchhd/datasets/breast_tissue.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/car.py` & `torch-hd-5.2.0/torchhd/datasets/car.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/cardiotocography_10clases.py` & `torch-hd-5.2.0/torchhd/datasets/cardiotocography_10clases.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/cardiotocography_3clases.py` & `torch-hd-5.2.0/torchhd/datasets/cardiotocography_3clases.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/ccpp.py` & `torch-hd-5.2.0/torchhd/datasets/ccpp.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/chess_krvk.py` & `torch-hd-5.2.0/torchhd/datasets/chess_krvk.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/chess_krvkp.py` & `torch-hd-5.2.0/torchhd/datasets/chess_krvkp.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/congressional_voting.py` & `torch-hd-5.2.0/torchhd/datasets/congressional_voting.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/conn_bench_sonar_mines_rocks.py` & `torch-hd-5.2.0/torchhd/datasets/conn_bench_sonar_mines_rocks.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/conn_bench_vowel_deterding.py` & `torch-hd-5.2.0/torchhd/datasets/conn_bench_vowel_deterding.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/connect_4.py` & `torch-hd-5.2.0/torchhd/datasets/connect_4.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/contrac.py` & `torch-hd-5.2.0/torchhd/datasets/contrac.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/credit_approval.py` & `torch-hd-5.2.0/torchhd/datasets/credit_approval.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/cylinder_bands.py` & `torch-hd-5.2.0/torchhd/datasets/cylinder_bands.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/dataset.py` & `torch-hd-5.2.0/torchhd/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/dermatology.py` & `torch-hd-5.2.0/torchhd/datasets/dermatology.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/echocardiogram.py` & `torch-hd-5.2.0/torchhd/datasets/echocardiogram.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/ecoli.py` & `torch-hd-5.2.0/torchhd/datasets/ecoli.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/emg_hand_gestures.py` & `torch-hd-5.2.0/torchhd/datasets/emg_hand_gestures.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/energy_y1.py` & `torch-hd-5.2.0/torchhd/datasets/energy_y1.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/energy_y2.py` & `torch-hd-5.2.0/torchhd/datasets/energy_y2.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/european_languages.py` & `torch-hd-5.2.0/torchhd/datasets/european_languages.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/fertility.py` & `torch-hd-5.2.0/torchhd/datasets/fertility.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/flags.py` & `torch-hd-5.2.0/torchhd/datasets/flags.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/glass.py` & `torch-hd-5.2.0/torchhd/datasets/glass.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/haberman_survival.py` & `torch-hd-5.2.0/torchhd/datasets/haberman_survival.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/hayes_roth.py` & `torch-hd-5.2.0/torchhd/datasets/hayes_roth.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/heart_cleveland.py` & `torch-hd-5.2.0/torchhd/datasets/heart_cleveland.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/heart_hungarian.py` & `torch-hd-5.2.0/torchhd/datasets/heart_hungarian.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/heart_switzerland.py` & `torch-hd-5.2.0/torchhd/datasets/heart_switzerland.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/heart_va.py` & `torch-hd-5.2.0/torchhd/datasets/heart_va.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/hepatitis.py` & `torch-hd-5.2.0/torchhd/datasets/hepatitis.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/hill_valley.py` & `torch-hd-5.2.0/torchhd/datasets/hill_valley.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/horse_colic.py` & `torch-hd-5.2.0/torchhd/datasets/horse_colic.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/ilpd_indian_liver.py` & `torch-hd-5.2.0/torchhd/datasets/ilpd_indian_liver.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/image_segmentation.py` & `torch-hd-5.2.0/torchhd/datasets/image_segmentation.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/ionosphere.py` & `torch-hd-5.2.0/torchhd/datasets/ionosphere.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/iris.py` & `torch-hd-5.2.0/torchhd/datasets/iris.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/isolet.py` & `torch-hd-5.2.0/torchhd/datasets/isolet.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/led_display.py` & `torch-hd-5.2.0/torchhd/datasets/led_display.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/lenses.py` & `torch-hd-5.2.0/torchhd/datasets/lenses.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/letter.py` & `torch-hd-5.2.0/torchhd/datasets/letter.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/libras.py` & `torch-hd-5.2.0/torchhd/datasets/libras.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/low_res_spect.py` & `torch-hd-5.2.0/torchhd/datasets/low_res_spect.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/lung_cancer.py` & `torch-hd-5.2.0/torchhd/datasets/lung_cancer.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/lymphography.py` & `torch-hd-5.2.0/torchhd/datasets/lymphography.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/magic.py` & `torch-hd-5.2.0/torchhd/datasets/magic.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/mammographic.py` & `torch-hd-5.2.0/torchhd/datasets/mammographic.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/miniboone.py` & `torch-hd-5.2.0/torchhd/datasets/miniboone.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/molec_biol_promoter.py` & `torch-hd-5.2.0/torchhd/datasets/molec_biol_promoter.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/molec_biol_splice.py` & `torch-hd-5.2.0/torchhd/datasets/molec_biol_splice.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/monks_1.py` & `torch-hd-5.2.0/torchhd/datasets/monks_1.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/monks_2.py` & `torch-hd-5.2.0/torchhd/datasets/monks_2.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/monks_3.py` & `torch-hd-5.2.0/torchhd/datasets/monks_3.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/mushroom.py` & `torch-hd-5.2.0/torchhd/datasets/mushroom.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/musk_1.py` & `torch-hd-5.2.0/torchhd/datasets/musk_1.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/musk_2.py` & `torch-hd-5.2.0/torchhd/datasets/musk_2.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/nursery.py` & `torch-hd-5.2.0/torchhd/datasets/nursery.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/oocytes_merluccius_nucleus_4d.py` & `torch-hd-5.2.0/torchhd/datasets/oocytes_merluccius_nucleus_4d.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/oocytes_merluccius_states_2f.py` & `torch-hd-5.2.0/torchhd/datasets/oocytes_merluccius_states_2f.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/oocytes_trisopterus_nucleus_2f.py` & `torch-hd-5.2.0/torchhd/datasets/oocytes_trisopterus_nucleus_2f.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/oocytes_trisopterus_states_5b.py` & `torch-hd-5.2.0/torchhd/datasets/oocytes_trisopterus_states_5b.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/optical.py` & `torch-hd-5.2.0/torchhd/datasets/optical.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/ozone.py` & `torch-hd-5.2.0/torchhd/datasets/ozone.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/page_blocks.py` & `torch-hd-5.2.0/torchhd/datasets/page_blocks.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/pamap.py` & `torch-hd-5.2.0/torchhd/datasets/pamap.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/parkinsons.py` & `torch-hd-5.2.0/torchhd/datasets/parkinsons.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/pendigits.py` & `torch-hd-5.2.0/torchhd/datasets/pendigits.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/pima.py` & `torch-hd-5.2.0/torchhd/datasets/pima.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/pittsburg_bridges_material.py` & `torch-hd-5.2.0/torchhd/datasets/pittsburg_bridges_material.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/pittsburg_bridges_rel_l.py` & `torch-hd-5.2.0/torchhd/datasets/pittsburg_bridges_rel_l.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/pittsburg_bridges_span.py` & `torch-hd-5.2.0/torchhd/datasets/pittsburg_bridges_span.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/pittsburg_bridges_t_or_d.py` & `torch-hd-5.2.0/torchhd/datasets/pittsburg_bridges_t_or_d.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/pittsburg_bridges_type.py` & `torch-hd-5.2.0/torchhd/datasets/pittsburg_bridges_type.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/planning.py` & `torch-hd-5.2.0/torchhd/datasets/planning.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/plant_margin.py` & `torch-hd-5.2.0/torchhd/datasets/plant_margin.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/plant_shape.py` & `torch-hd-5.2.0/torchhd/datasets/plant_shape.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/plant_texture.py` & `torch-hd-5.2.0/torchhd/datasets/plant_texture.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/post_operative.py` & `torch-hd-5.2.0/torchhd/datasets/post_operative.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/primary_tumor.py` & `torch-hd-5.2.0/torchhd/datasets/primary_tumor.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/ringnorm.py` & `torch-hd-5.2.0/torchhd/datasets/ringnorm.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/seeds.py` & `torch-hd-5.2.0/torchhd/datasets/seeds.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/semeion.py` & `torch-hd-5.2.0/torchhd/datasets/semeion.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/soybean.py` & `torch-hd-5.2.0/torchhd/datasets/soybean.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/spambase.py` & `torch-hd-5.2.0/torchhd/datasets/spambase.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/spect.py` & `torch-hd-5.2.0/torchhd/datasets/spect.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/spectf.py` & `torch-hd-5.2.0/torchhd/datasets/spectf.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/statlog_australian_credit.py` & `torch-hd-5.2.0/torchhd/datasets/statlog_australian_credit.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/statlog_german_credit.py` & `torch-hd-5.2.0/torchhd/datasets/statlog_german_credit.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/statlog_heart.py` & `torch-hd-5.2.0/torchhd/datasets/statlog_heart.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/statlog_image.py` & `torch-hd-5.2.0/torchhd/datasets/statlog_image.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/statlog_landsat.py` & `torch-hd-5.2.0/torchhd/datasets/statlog_landsat.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/statlog_shuttle.py` & `torch-hd-5.2.0/torchhd/datasets/statlog_shuttle.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/statlog_vehicle.py` & `torch-hd-5.2.0/torchhd/datasets/statlog_vehicle.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/steel_plates.py` & `torch-hd-5.2.0/torchhd/datasets/steel_plates.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/synthetic_control.py` & `torch-hd-5.2.0/torchhd/datasets/synthetic_control.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/teaching.py` & `torch-hd-5.2.0/torchhd/datasets/teaching.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/thyroid.py` & `torch-hd-5.2.0/torchhd/datasets/thyroid.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/tic_tac_toe.py` & `torch-hd-5.2.0/torchhd/datasets/tic_tac_toe.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/titanic.py` & `torch-hd-5.2.0/torchhd/datasets/titanic.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/trains.py` & `torch-hd-5.2.0/torchhd/datasets/trains.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/twonorm.py` & `torch-hd-5.2.0/torchhd/datasets/twonorm.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/ucihar.py` & `torch-hd-5.2.0/torchhd/datasets/ucihar.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/utils.py` & `torch-hd-5.2.0/torchhd/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/vertebral_column_2clases.py` & `torch-hd-5.2.0/torchhd/datasets/vertebral_column_2clases.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/vertebral_column_3clases.py` & `torch-hd-5.2.0/torchhd/datasets/vertebral_column_3clases.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/wall_following.py` & `torch-hd-5.2.0/torchhd/datasets/wall_following.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/waveform.py` & `torch-hd-5.2.0/torchhd/datasets/waveform.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/waveform_noise.py` & `torch-hd-5.2.0/torchhd/datasets/waveform_noise.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/wine.py` & `torch-hd-5.2.0/torchhd/datasets/wine.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/wine_quality_red.py` & `torch-hd-5.2.0/torchhd/datasets/wine_quality_red.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/wine_quality_white.py` & `torch-hd-5.2.0/torchhd/datasets/wine_quality_white.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/yeast.py` & `torch-hd-5.2.0/torchhd/datasets/yeast.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/datasets/zoo.py` & `torch-hd-5.2.0/torchhd/datasets/zoo.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/embeddings.py` & `torch-hd-5.2.0/torchhd/embeddings.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,36 +18,40 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 import math
-from typing import Type, Union, Optional
+from typing import Type, Union, Optional, Literal, Callable
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch import Tensor
 from torch.nn.parameter import Parameter
 
 import torchhd.functional as functional
 from torchhd.tensors.base import VSATensor
 from torchhd.tensors.map import MAPTensor
+from torchhd.tensors.fhrr import FHRRTensor
+from torchhd.tensors.hrr import HRRTensor
 from torchhd.types import VSAOptions
 
+
 __all__ = [
     "Empty",
     "Identity",
     "Random",
     "Level",
     "Thermometer",
     "Circular",
     "Projection",
     "Sinusoid",
     "Density",
+    "FractionalPower",
 ]
 
 
 class Empty(nn.Embedding):
     """Embedding wrapper around :func:`~torchhd.empty`.
 
     Class inherits from `Embedding <https://pytorch.org/docs/stable/generated/torch.nn.Embedding.html>`_ and supports the same keyword arguments.
@@ -962,7 +966,198 @@
 
     # Specify the steps needed to perform the encoding
     def forward(self, input: Tensor) -> Tensor:
         # Perform binding of key and value vectors
         output = functional.bind(self.key.weight, self.density_encoding(input))
         # Perform the superposition operation on the bound key-value pairs
         return functional.multibundle(output)
+
+
+class FractionalPower(nn.Module):
+    """Class for fractional power encoding (FPE) method that forms hypervectors for given values, kernel shape, bandwidth, and dimensionality. Implements similarity-preserving hypervectors approximating desired kernel shape as described in `Computing on Functions Using Randomized Vector Representations <https://arxiv.org/abs/2109.03429>`_.
+
+    Args:
+        in_features (int): the dimensionality of the input feature vector.
+        out_features (int): the dimensionality of the hypervectors.
+        distribution (str, optional): hyperparameter defining the shape of the kernel by specifying a particular probability distribution that is used to sample the base hypervector(s).  Default: ``"sinc"``.
+        bandwidth (float, optional): positive hyperparameter defining the width of the similarity kernel. Lower values lead to broader kernels while larger values lead to more narrow kernels. Default: ``1.0``.
+        vsa: (``VSAOptions``, optional): specifies the hypervector type to be instantiated. Default: ``"FHRR"``.
+        dtype (``torch.dtype``, optional): the desired data type of returned tensor. Default: if ``None`` depends on VSATensor.
+        device (``torch.device``, optional):  the desired device of returned tensor. Default: if ``None``, uses the current device for the default tensor type (see torch.set_default_tensor_type()). ``device`` will be the CPU for CPU tensor types and the current CUDA device for CUDA tensor types.
+        requires_grad (bool, optional): If autograd should record operations on the returned tensor. Default: ``False``.
+
+    Examples::
+
+        >>> embed = embeddings.FractionalPower(1, 6, "sinc", 1.0, "FHRR")
+        >>> embed(torch.arange(1, 4, 1.).view(-1, 1))
+        FHRRTensor([[-0.7181-0.6959j, -0.5269+0.8499j, -0.0848+0.9964j,  0.9720-0.2348j,
+              0.6358+0.7718j,  0.4352+0.9003j],
+            [ 0.0314+0.9995j, -0.4447-0.8957j, -0.9856-0.1689j,  0.8897-0.4565j,
+             -0.1915+0.9815j, -0.6212+0.7836j],
+            [ 0.6730-0.7396j,  0.9956+0.0940j,  0.2519-0.9678j,  0.7576-0.6527j,
+             -0.8793+0.4762j, -0.9759-0.2183j]])
+
+    """
+
+    # The collection of distributions for basic predefined kernels
+    predefined_kernels = {
+        "sinc": torch.distributions.Uniform(-math.pi, math.pi),
+        "gaussian": torch.distributions.Normal(0.0, 1.0),
+    }
+
+    def __init__(
+        self,
+        in_features: int,
+        out_features: int,
+        distribution: Union[
+            torch.distributions.Distribution, Literal["sinc", "gaussian"]
+        ] = "sinc",
+        bandwidth: float = 1.0,
+        vsa: Literal["HRR", "FHRR"] = "FHRR",
+        device=None,
+        dtype=None,
+        requires_grad: bool = False,
+    ) -> None:
+        factory_kwargs = {"device": device, "dtype": dtype}
+        super(FractionalPower, self).__init__()
+
+        self.in_features = in_features  # data dimensions
+        self.out_features = out_features  # hypervector dimensions
+        self.bandwidth = bandwidth
+        self.requires_grad = requires_grad
+
+        if vsa not in {"HRR", "FHRR"}:
+            raise ValueError(
+                f"FractionalPower embedding only supports HRR and FHRR but provided: {vsa}"
+            )
+
+        self.vsa_tensor = functional.get_vsa_tensor_class(vsa)
+
+        if dtype not in self.vsa_tensor.supported_dtypes:
+            raise ValueError(f"dtype {dtype} not supported by {vsa}")
+
+        # If the distribution is a string use the presets in predefined_kernels
+        if isinstance(distribution, str):
+            try:
+                self.distribution = self.predefined_kernels[distribution]
+            except KeyError:
+                available_names = ", ".join(list(self.predefined_kernels.keys()))
+                raise ValueError(
+                    f"{distribution} kernel is not supported, use one of: {available_names}, or provide a custom torch distribution."
+                )
+        else:
+            self.distribution = distribution
+
+        # Initialize encoding's parameters
+        self.weight = nn.Parameter(
+            torch.empty(self.out_features, self.in_features, **factory_kwargs),
+            requires_grad,
+        )
+        self.reset_parameters()
+
+    # Sample the angles using the provided distribution
+    def reset_parameters(self) -> None:
+        """Generate the angles for basis hypervector(s) to be used for encoding the data."""
+
+        sample_shape = self.distribution.sample().shape
+
+        # Check HD/VSA model type
+        if self.vsa_tensor == FHRRTensor:
+            # Generate the angles for base hypervector(s) that determines the shape of the FPE kernel
+            # If the distribution is one-dimensional this implies that base hypervectors are independent so it is safe to generate self.in_features * self.out_features independent samples
+            if sample_shape == ():
+                # Draw angles from a uniform  distribution for base hypervector(s). Note that data dimensions here are independent but this does not have to be always the case
+                phases = self.distribution.sample((self.out_features, self.in_features))
+                phases = phases.to(self.weight)
+                self.weight.data.copy_(phases)
+
+            # If base hypervectors are correlated then the dimensionality of the distribution should match that of the data
+            elif sample_shape == (self.in_features,):
+                phases = self.distribution.sample((self.out_features,))
+                phases = phases.to(self.weight)
+                self.weight.data.copy_(phases)
+
+            # Raise error due to the ambiguity of the situation
+            else:
+                raise ValueError(
+                    f"The provided distribution has shape {sample_shape} while the input data expects shape () or ({self.in_features},) so there is a mismatch."
+                )
+
+        elif self.vsa_tensor == HRRTensor:
+            # Fewer angles are needed
+            dimensions_real = int((self.out_features - 1) / 2)
+
+            # Generate the angles for base hypervector(s) that determines the shape of the FPE kernel
+            # If the distribution is one-dimensional this implies that base hypervectors are independent so it is safe to generate self.in_features * self.out_features independent samples
+            if sample_shape == ():
+                # Draw angles from a uniform  distribution for base hypervector(s). Note that data dimensions here are independent but this does not have to be always the case
+                phases = self.distribution.sample((dimensions_real, self.in_features))
+
+            # If base hypervectors are correlated then the dimensionality of the distribution should match that of the data
+            elif sample_shape == (self.in_features,):
+                phases = self.distribution.sample((dimensions_real,))
+
+            # Raise error due to the ambiguity of the situation
+            else:
+                raise ValueError(
+                    f"The provided distribution has shape {sample_shape} while the input data expects shape () or ({self.in_features},) so there is a mismatch."
+                )
+
+            # Make the generated angles negatively symmetric so they look as a spectrum
+            phases = torch.cat(
+                (
+                    phases,
+                    torch.zeros(1, self.in_features),
+                    -torch.flip(phases, dims=[0]),
+                ),
+                dim=0,
+            )
+            if self.out_features % 2 == 0:
+                phases = torch.cat((torch.zeros(1, self.in_features), phases), dim=0)
+
+            phases = phases.to(self.weight)
+            # Set the generated angles to the object's parameters
+            self.weight.data.copy_(phases)
+
+    def basis(self):
+        """Return the values of the base hypervector(s)"""
+
+        # Use the angles in self.weight to obtain the values of the base hypervector(s)
+        if self.vsa_tensor == FHRRTensor:
+            hvs = torch.complex(self.weight.cos(), self.weight.sin()).T
+            hvs = hvs.as_subclass(FHRRTensor)
+
+        elif self.vsa_tensor == HRRTensor:
+            complex_hv = torch.complex(self.weight.cos(), self.weight.sin()).T
+            hvs = torch.real(
+                torch.fft.ifft(torch.fft.ifftshift(complex_hv, dim=1), dim=1)
+            )
+            hvs = hvs.as_subclass(HRRTensor)
+
+        return hvs
+
+    def forward(self, input: Tensor) -> Tensor:
+        """Creates a fractional power encoding (FPE) for given values.
+
+        Args:
+            input (Tensor): values for which FPE hypervectors should be generated. Either a vector or a batch of vectors.
+
+        Shapes:
+            - Input: :math:`(*, f)` where f is the in_features and * is an optional batch dimension.
+            - Output: :math:`(*, d)` where d is the out_features and * is an optional batch dimension.
+
+        """
+
+        # Perform FPE of the desired values using the base hypervector(s)
+        # Simultaneously computes angles for given values and their sum that is equivalent to the binding
+        if self.vsa_tensor == FHRRTensor:
+            phases = F.linear(self.bandwidth * input, self.weight)
+            hv = torch.complex(phases.cos(), phases.sin())
+            hv = hv.as_subclass(FHRRTensor)
+
+        elif self.vsa_tensor == HRRTensor:
+            phases = F.linear(self.bandwidth * input, self.weight)
+            hv = torch.complex(phases.cos(), phases.sin())
+            hv = torch.real(torch.fft.ifft(torch.fft.ifftshift(hv, dim=1), dim=1))
+            hv = hv.as_subclass(HRRTensor)
+
+        return hv
```

### Comparing `torch-hd-5.1.2/torchhd/functional.py` & `torch-hd-5.2.0/torchhd/functional.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/memory.py` & `torch-hd-5.2.0/torchhd/memory.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/models.py` & `torch-hd-5.2.0/torchhd/models.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/structures.py` & `torch-hd-5.2.0/torchhd/structures.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/tensors/__init__.py` & `torch-hd-5.2.0/torchhd/tensors/__init__.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/tensors/base.py` & `torch-hd-5.2.0/torchhd/tensors/base.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/tensors/bsc.py` & `torch-hd-5.2.0/torchhd/tensors/bsc.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/tensors/fhrr.py` & `torch-hd-5.2.0/torchhd/tensors/fhrr.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/tensors/hrr.py` & `torch-hd-5.2.0/torchhd/tensors/hrr.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/tensors/map.py` & `torch-hd-5.2.0/torchhd/tensors/map.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/tests/basis_hv/__init__.py` & `torch-hd-5.2.0/torchhd/tests/basis_hv/__init__.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/tests/basis_hv/test_base_tensor.py` & `torch-hd-5.2.0/torchhd/tests/basis_hv/test_base_tensor.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/tests/basis_hv/test_circular_hv.py` & `torch-hd-5.2.0/torchhd/tests/basis_hv/test_circular_hv.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/tests/basis_hv/test_empty_hv.py` & `torch-hd-5.2.0/torchhd/tests/basis_hv/test_empty_hv.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/tests/basis_hv/test_identity_hv.py` & `torch-hd-5.2.0/torchhd/tests/basis_hv/test_identity_hv.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/tests/basis_hv/test_level_hv.py` & `torch-hd-5.2.0/torchhd/tests/basis_hv/test_level_hv.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/tests/basis_hv/test_random_hv.py` & `torch-hd-5.2.0/torchhd/tests/basis_hv/test_random_hv.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/tests/structures/__init__.py` & `torch-hd-5.2.0/torchhd/tests/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/tests/structures/test_distinct_sequence.py` & `torch-hd-5.2.0/torchhd/tests/structures/test_distinct_sequence.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/tests/structures/test_fsa.py` & `torch-hd-5.2.0/torchhd/tests/structures/test_fsa.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/tests/structures/test_graph.py` & `torch-hd-5.2.0/torchhd/tests/structures/test_graph.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/tests/structures/test_hashtable.py` & `torch-hd-5.2.0/torchhd/tests/structures/test_hashtable.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/tests/structures/test_memory.py` & `torch-hd-5.2.0/torchhd/tests/structures/test_memory.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/tests/structures/test_multiset.py` & `torch-hd-5.2.0/torchhd/tests/structures/test_multiset.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/tests/structures/test_sequence.py` & `torch-hd-5.2.0/torchhd/tests/structures/test_sequence.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/tests/structures/test_tree.py` & `torch-hd-5.2.0/torchhd/tests/structures/test_tree.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/types.py` & `torch-hd-5.2.0/torchhd/types.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/utils.py` & `torch-hd-5.2.0/torchhd/utils.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.1.2/torchhd/version.py` & `torch-hd-5.2.0/torchhd/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
-__version__ = "5.1.2"
+__version__ = "5.2.0"
```

