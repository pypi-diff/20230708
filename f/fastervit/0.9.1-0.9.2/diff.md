# Comparing `tmp/fastervit-0.9.1.tar.gz` & `tmp/fastervit-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/ali/Desktop/Gitlab_repos/FasterViT_pip_test/dist/.tmp-zaj7smev/fastervit-0.9.1.tar", last modified: Wed Jul  5 05:28:12 2023, max compression
+gzip compressed data, was "/home/ali/Desktop/Gitlab_repos/FasterViT_pip_test/dist/.tmp-rbstb00d/fastervit-0.9.2.tar", last modified: Fri Jul  7 22:30:07 2023, max compression
```

## Comparing `fastervit-0.9.1.tar` & `fastervit-0.9.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-05 05:28:12.000000 fastervit-0.9.1/
--rw-rw-r--   0 ali       (1000) ali       (1000)     4146 2023-07-05 05:27:14.000000 fastervit-0.9.1/LICENSE
--rw-rw-r--   0 ali       (1000) ali       (1000)       45 2023-07-05 05:27:14.000000 fastervit-0.9.1/MANIFEST.in
--rw-rw-r--   0 ali       (1000) ali       (1000)    11887 2023-07-05 05:28:12.000000 fastervit-0.9.1/PKG-INFO
--rw-rw-r--   0 ali       (1000) ali       (1000)    10937 2023-07-05 05:27:14.000000 fastervit-0.9.1/README.md
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-05 05:28:12.000000 fastervit-0.9.1/fastervit/
--rw-rw-r--   0 ali       (1000) ali       (1000)       41 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/__init__.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-05 05:28:12.000000 fastervit-0.9.1/fastervit/assets/
--rw-rw-r--   0 ali       (1000) ali       (1000)   100537 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/assets/hierarchial_attn.png
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-05 05:28:12.000000 fastervit-0.9.1/fastervit/models/
--rw-rw-r--   0 ali       (1000) ali       (1000)       96 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/models/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    48432 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/models/faster_vit.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    50190 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/models/faster_vit_any_res.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     7844 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/models/registry.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-05 05:28:12.000000 fastervit-0.9.1/fastervit/scheduler/
--rw-rw-r--   0 ali       (1000) ali       (1000)      291 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/scheduler/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     4161 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/scheduler/cosine_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     2098 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/scheduler/multistep_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     3457 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/scheduler/plateau_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     4003 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/scheduler/poly_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     5095 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/scheduler/scheduler.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     3907 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/scheduler/scheduler_factory.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     1902 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/scheduler/step_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     3936 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/scheduler/tanh_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      734 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/tensorboard.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    49422 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/train.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-05 05:28:12.000000 fastervit-0.9.1/fastervit/utils/
--rw-rw-r--   0 ali       (1000) ali       (1000)        0 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/utils/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    19251 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/utils/datasets.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    16145 2023-07-05 05:27:14.000000 fastervit-0.9.1/fastervit/validate.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-05 05:28:12.000000 fastervit-0.9.1/fastervit.egg-info/
--rw-rw-r--   0 ali       (1000) ali       (1000)    11887 2023-07-05 05:28:12.000000 fastervit-0.9.1/fastervit.egg-info/PKG-INFO
--rw-rw-r--   0 ali       (1000) ali       (1000)      824 2023-07-05 05:28:12.000000 fastervit-0.9.1/fastervit.egg-info/SOURCES.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)        1 2023-07-05 05:28:12.000000 fastervit-0.9.1/fastervit.egg-info/dependency_links.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)       32 2023-07-05 05:28:12.000000 fastervit-0.9.1/fastervit.egg-info/requires.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)       10 2023-07-05 05:28:12.000000 fastervit-0.9.1/fastervit.egg-info/top_level.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)      126 2023-07-05 05:28:12.000000 fastervit-0.9.1/setup.cfg
--rw-rw-r--   0 ali       (1000) ali       (1000)     1549 2023-07-05 05:27:14.000000 fastervit-0.9.1/setup.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-07 22:30:07.000000 fastervit-0.9.2/
+-rw-rw-r--   0 ali       (1000) ali       (1000)     4146 2023-07-07 22:05:20.000000 fastervit-0.9.2/LICENSE
+-rw-rw-r--   0 ali       (1000) ali       (1000)       45 2023-07-07 22:05:20.000000 fastervit-0.9.2/MANIFEST.in
+-rw-rw-r--   0 ali       (1000) ali       (1000)    10232 2023-07-07 22:30:07.000000 fastervit-0.9.2/PKG-INFO
+-rw-rw-r--   0 ali       (1000) ali       (1000)     9282 2023-07-07 22:29:03.000000 fastervit-0.9.2/README.md
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-07 22:30:07.000000 fastervit-0.9.2/fastervit/
+-rw-rw-r--   0 ali       (1000) ali       (1000)       41 2023-07-07 22:05:20.000000 fastervit-0.9.2/fastervit/__init__.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-07 22:30:07.000000 fastervit-0.9.2/fastervit/assets/
+-rw-rw-r--   0 ali       (1000) ali       (1000)   100537 2023-07-07 22:05:20.000000 fastervit-0.9.2/fastervit/assets/hierarchial_attn.png
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-07 22:30:07.000000 fastervit-0.9.2/fastervit/models/
+-rw-rw-r--   0 ali       (1000) ali       (1000)       96 2023-07-07 22:05:20.000000 fastervit-0.9.2/fastervit/models/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    49072 2023-07-07 22:14:53.000000 fastervit-0.9.2/fastervit/models/faster_vit.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    50830 2023-07-07 22:20:22.000000 fastervit-0.9.2/fastervit/models/faster_vit_any_res.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     7844 2023-07-07 22:05:20.000000 fastervit-0.9.2/fastervit/models/registry.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-07 22:30:07.000000 fastervit-0.9.2/fastervit/scheduler/
+-rw-rw-r--   0 ali       (1000) ali       (1000)      291 2023-07-07 22:05:20.000000 fastervit-0.9.2/fastervit/scheduler/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     4161 2023-07-07 22:05:20.000000 fastervit-0.9.2/fastervit/scheduler/cosine_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     2098 2023-07-07 22:05:20.000000 fastervit-0.9.2/fastervit/scheduler/multistep_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     3457 2023-07-07 22:05:20.000000 fastervit-0.9.2/fastervit/scheduler/plateau_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     4003 2023-07-07 22:05:20.000000 fastervit-0.9.2/fastervit/scheduler/poly_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     5095 2023-07-07 22:05:20.000000 fastervit-0.9.2/fastervit/scheduler/scheduler.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     3907 2023-07-07 22:05:20.000000 fastervit-0.9.2/fastervit/scheduler/scheduler_factory.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1902 2023-07-07 22:05:20.000000 fastervit-0.9.2/fastervit/scheduler/step_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     3936 2023-07-07 22:05:20.000000 fastervit-0.9.2/fastervit/scheduler/tanh_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      734 2023-07-07 22:05:20.000000 fastervit-0.9.2/fastervit/tensorboard.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    49422 2023-07-07 22:05:20.000000 fastervit-0.9.2/fastervit/train.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-07 22:30:07.000000 fastervit-0.9.2/fastervit/utils/
+-rw-rw-r--   0 ali       (1000) ali       (1000)        0 2023-07-07 22:05:20.000000 fastervit-0.9.2/fastervit/utils/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    19251 2023-07-07 22:05:20.000000 fastervit-0.9.2/fastervit/utils/datasets.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    16159 2023-07-07 22:17:54.000000 fastervit-0.9.2/fastervit/validate.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-07 22:30:07.000000 fastervit-0.9.2/fastervit.egg-info/
+-rw-rw-r--   0 ali       (1000) ali       (1000)    10232 2023-07-07 22:30:07.000000 fastervit-0.9.2/fastervit.egg-info/PKG-INFO
+-rw-rw-r--   0 ali       (1000) ali       (1000)      824 2023-07-07 22:30:07.000000 fastervit-0.9.2/fastervit.egg-info/SOURCES.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)        1 2023-07-07 22:30:07.000000 fastervit-0.9.2/fastervit.egg-info/dependency_links.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)       32 2023-07-07 22:30:07.000000 fastervit-0.9.2/fastervit.egg-info/requires.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)       10 2023-07-07 22:30:07.000000 fastervit-0.9.2/fastervit.egg-info/top_level.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)      126 2023-07-07 22:30:07.000000 fastervit-0.9.2/setup.cfg
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1549 2023-07-07 22:29:54.000000 fastervit-0.9.2/setup.py
```

### Comparing `fastervit-0.9.1/LICENSE` & `fastervit-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.1/PKG-INFO` & `fastervit-0.9.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6661 7374  : 2.1.Name: fast
 00000020: 6572 7669 740a 5665 7273 696f 6e3a 2030  ervit.Version: 0
-00000030: 2e39 2e31 0a53 756d 6d61 7279 3a20 4661  .9.1.Summary: Fa
+00000030: 2e39 2e32 0a53 756d 6d61 7279 3a20 4661  .9.2.Summary: Fa
 00000040: 7374 6572 5669 543a 2046 6173 7420 5669  sterViT: Fast Vi
 00000050: 7369 6f6e 2054 7261 6e73 666f 726d 6572  sion Transformer
 00000060: 7320 7769 7468 2048 6965 7261 7263 6869  s with Hierarchi
 00000070: 6361 6c20 4174 7465 6e74 696f 6e0a 486f  cal Attention.Ho
 00000080: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
 00000090: 2f67 6974 6875 622e 636f 6d2f 4e56 6c61  /github.com/NVla
 000000a0: 6273 2f46 6173 7465 7256 6954 0a41 7574  bs/FasterViT.Aut
@@ -118,626 +118,523 @@
 00000750: 2f67 6974 6875 622e 636f 6d2f 4e56 6c61  /github.com/NVla
 00000760: 6273 2f46 6173 7465 7256 6954 2f61 7373  bs/FasterViT/ass
 00000770: 6574 732f 3236 3830 3633 3934 2f32 3533  ets/26806394/253
 00000780: 6431 6132 652d 6235 6635 2d34 6139 622d  d1a2e-b5f5-4a9b-
 00000790: 6133 3632 2d36 6364 6431 3662 6663 6363  a362-6cdd16bfccc
 000007a0: 3122 2077 6964 7468 3d36 3225 2068 6569  1" width=62% hei
 000007b0: 6768 743d 3632 2520 0a63 6c61 7373 3d22  ght=62% .class="
-000007c0: 6365 6e74 6572 223e 0a3c 2f70 3e0a 0a57  center">.</p>..W
-000007d0: 6520 696e 7472 6f64 7563 6520 6120 6e65  e introduce a ne
-000007e0: 7720 7365 6c66 2d61 7474 656e 7469 6f6e  w self-attention
-000007f0: 206d 6563 6861 6e69 736d 2c20 6465 6e6f   mechanism, deno
-00000800: 7465 6420 6173 2048 6965 7261 7263 6869  ted as Hierarchi
-00000810: 6361 6c0a 4174 7465 6e74 696f 6e20 2848  cal.Attention (H
-00000820: 4154 292c 2074 6861 7420 6361 7074 7572  AT), that captur
-00000830: 6573 2062 6f74 6820 7368 6f72 7420 616e  es both short an
-00000840: 6420 6c6f 6e67 2d72 616e 6765 2069 6e66  d long-range inf
-00000850: 6f72 6d61 7469 6f6e 2062 7920 6c65 6172  ormation by lear
-00000860: 6e69 6e67 0a63 726f 7373 2d77 696e 646f  ning.cross-windo
-00000870: 7720 6361 7272 6965 7220 746f 6b65 6e73  w carrier tokens
-00000880: 2e0a 0a21 5b74 6561 7365 725d 282e 2f66  ...![teaser](./f
-00000890: 6173 7465 7276 6974 2f61 7373 6574 732f  astervit/assets/
-000008a0: 6869 6572 6172 6368 6961 6c5f 6174 746e  hierarchial_attn
-000008b0: 2e70 6e67 290a 0a23 2320 5175 6963 6b20  .png)..## Quick 
-000008c0: 5374 6172 740a 0a57 6520 6361 6e20 696d  Start..We can im
-000008d0: 706f 7274 2070 7265 2d74 7261 696e 6564  port pre-trained
-000008e0: 2046 6173 7465 7256 6954 206d 6f64 656c   FasterViT model
-000008f0: 7320 7769 7468 202a 2a31 206c 696e 6520  s with **1 line 
-00000900: 6f66 2063 6f64 652a 2a2e 2046 6972 7374  of code**. First
-00000910: 2c20 4661 7374 6572 5669 5420 6361 6e20  , FasterViT can 
-00000920: 6265 2073 696d 706c 7920 696e 7374 616c  be simply instal
-00000930: 6c65 6420 6279 3a0a 0a60 6060 6261 7368  led by:..```bash
-00000940: 0a70 6970 2069 6e73 7461 6c6c 2066 6173  .pip install fas
-00000950: 7465 7276 6974 0a60 6060 0a0a 4120 7072  tervit.```..A pr
-00000960: 6574 7261 696e 6564 2046 6173 7465 7256  etrained FasterV
-00000970: 6954 206d 6f64 656c 2077 6974 6820 6465  iT model with de
-00000980: 6661 756c 7420 6879 7065 722d 7061 7261  fault hyper-para
-00000990: 6d65 7465 7273 2063 616e 2062 6520 6372  meters can be cr
-000009a0: 6561 7465 6420 6173 2069 6e20 7468 6520  eated as in the 
-000009b0: 666f 6c6c 6f77 696e 673a 0a0a 6060 6070  following:..```p
-000009c0: 7974 686f 6e0a 3e3e 3e20 6672 6f6d 2066  ython.>>> from f
-000009d0: 6173 7465 7276 6974 2069 6d70 6f72 7420  astervit import 
-000009e0: 6372 6561 7465 5f6d 6f64 656c 0a0a 2320  create_model..# 
-000009f0: 4465 6669 6e65 2066 6173 7465 7276 6974  Define fastervit
-00000a00: 2d30 206d 6f64 656c 2077 6974 6820 3232  -0 model with 22
-00000a10: 3420 7820 3232 3420 7265 736f 6c75 7469  4 x 224 resoluti
-00000a20: 6f6e 0a0a 3e3e 3e20 6d6f 6465 6c20 3d20  on..>>> model = 
-00000a30: 6372 6561 7465 5f6d 6f64 656c 2827 6661  create_model('fa
-00000a40: 7374 6572 5f76 6974 5f30 5f32 3234 272c  ster_vit_0_224',
-00000a50: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-00000a60: 2020 2020 2020 2020 2020 2020 7072 6574              pret
-00000a70: 7261 696e 6564 3d54 7275 652c 0a20 2020  rained=True,.   
-00000a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a90: 2020 2020 2020 206d 6f64 656c 5f70 6174         model_pat
-00000aa0: 683d 222f 746d 702f 6661 7374 6572 5f76  h="/tmp/faster_v
-00000ab0: 6974 5f30 2e70 7468 2e74 6172 2229 0a60  it_0.pth.tar").`
-00000ac0: 6060 0a0a 5765 2063 616e 2061 646a 7573  ``..We can adjus
-00000ad0: 7420 7768 6572 6520 746f 2064 6f77 6e6c  t where to downl
-00000ae0: 6f61 6420 7468 6520 6162 6f76 6520 4661  oad the above Fa
-00000af0: 7374 6572 5669 542d 3020 6d6f 6465 6c20  sterViT-0 model 
-00000b00: 6279 2070 6173 7369 6e67 2060 6d6f 6465  by passing `mode
-00000b10: 6c5f 7061 7468 602e 0a0a 5765 2063 616e  l_path`...We can
-00000b20: 2061 6c73 6f20 7369 6d70 6c79 2074 6573   also simply tes
-00000b30: 7420 7468 6520 6d6f 6465 6c20 6279 2070  t the model by p
-00000b40: 6173 7369 6e67 2061 2064 756d 6d79 2069  assing a dummy i
-00000b50: 6e70 7574 2069 6d61 6765 2e20 5468 6520  nput image. The 
-00000b60: 6f75 7470 7574 2069 7320 7468 6520 6c6f  output is the lo
-00000b70: 6769 7473 3a0a 0a60 6060 7079 7468 6f6e  gits:..```python
-00000b80: 0a3e 3e3e 2069 6d70 6f72 7420 746f 7263  .>>> import torc
-00000b90: 680a 0a3e 3e3e 2069 6d61 6765 203d 2074  h..>>> image = t
-00000ba0: 6f72 6368 2e72 616e 6428 312c 2033 2c20  orch.rand(1, 3, 
-00000bb0: 3232 342c 2032 3234 290a 3e3e 3e20 6f75  224, 224).>>> ou
-00000bc0: 7470 7574 203d 206d 6f64 656c 2869 6d61  tput = model(ima
-00000bd0: 6765 2920 2320 746f 7263 682e 5369 7a65  ge) # torch.Size
-00000be0: 285b 312c 2031 3030 305d 290a 6060 600a  ([1, 1000]).```.
-00000bf0: 0a57 6520 6361 6e20 616c 736f 2075 7365  .We can also use
-00000c00: 2074 6865 2061 6e79 2d72 6573 6f6c 7574   the any-resolut
-00000c10: 696f 6e20 4661 7374 6572 5669 5420 6d6f  ion FasterViT mo
-00000c20: 6465 6c20 746f 2061 6363 6f6d 6d6f 6461  del to accommoda
-00000c30: 7465 2061 7262 6974 7261 7279 2069 6d61  te arbitrary ima
-00000c40: 6765 2072 6573 6f6c 7574 696f 6e73 2e20  ge resolutions. 
-00000c50: 496e 2074 6865 2066 6f6c 6c6f 7769 6e67  In the following
-00000c60: 2c20 7765 2064 6566 696e 6520 616e 2061  , we define an a
-00000c70: 6e79 2d72 6573 6f6c 7574 696f 6e20 4661  ny-resolution Fa
-00000c80: 7374 6572 5669 542d 300a 6d6f 6465 6c20  sterViT-0.model 
-00000c90: 7769 7468 2069 6e70 7574 2072 6573 6f6c  with input resol
-00000ca0: 7574 696f 6e20 6f66 2035 3736 2078 2039  ution of 576 x 9
-00000cb0: 3630 2c20 7769 6e64 6f77 2073 697a 6573  60, window sizes
-00000cc0: 206f 6620 3132 2061 6e64 2036 2069 6e20   of 12 and 6 in 
-00000cd0: 3372 6420 616e 6420 3474 6820 7374 6167  3rd and 4th stag
-00000ce0: 6573 2c20 6361 7272 6965 7220 746f 6b65  es, carrier toke
-00000cf0: 6e20 7369 7a65 206f 6620 3220 616e 6420  n size of 2 and 
-00000d00: 656d 6265 6464 696e 6720 6469 6d65 6e73  embedding dimens
-00000d10: 696f 6e20 6f66 0a31 3238 3a0a 0a60 6060  ion of.128:..```
-00000d20: 7079 7468 6f6e 0a3e 3e3e 2066 726f 6d20  python.>>> from 
-00000d30: 6661 7374 6572 7669 7420 696d 706f 7274  fastervit import
-00000d40: 2063 7265 6174 655f 6d6f 6465 6c0a 0a23   create_model..#
-00000d50: 2044 6566 696e 6520 616e 792d 7265 736f   Define any-reso
-00000d60: 6c75 7469 6f6e 2046 6173 7465 7256 6954  lution FasterViT
-00000d70: 2d30 206d 6f64 656c 2077 6974 6820 3537  -0 model with 57
-00000d80: 3620 7820 3936 3020 7265 736f 6c75 7469  6 x 960 resoluti
-00000d90: 6f6e 0a3e 3e3e 206d 6f64 656c 203d 2063  on.>>> model = c
-00000da0: 7265 6174 655f 6d6f 6465 6c28 2766 6173  reate_model('fas
-00000db0: 7465 725f 7669 745f 305f 616e 795f 7265  ter_vit_0_any_re
-00000dc0: 7327 2c20 0a20 2020 2020 2020 2020 2020  s', .           
-00000dd0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00000de0: 6573 6f6c 7574 696f 6e3d 5b35 3736 2c20  esolution=[576, 
-00000df0: 3936 305d 2c0a 2020 2020 2020 2020 2020  960],.          
-00000e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e10: 7769 6e64 6f77 5f73 697a 653d 5b37 2c20  window_size=[7, 
-00000e20: 372c 2031 322c 2036 5d2c 0a20 2020 2020  7, 12, 6],.     
-00000e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e40: 2020 2020 2063 745f 7369 7a65 3d32 2c0a       ct_size=2,.
-00000e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e60: 2020 2020 2020 2020 2020 6469 6d3d 3634            dim=64
-00000e70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00000e80: 2020 2020 2020 2020 2020 2020 7072 6574              pret
-00000e90: 7261 696e 6564 3d54 7275 6529 0a60 6060  rained=True).```
-00000ea0: 0a4e 6f74 6520 7468 6174 2074 6865 2061  .Note that the a
-00000eb0: 626f 7665 206d 6f64 656c 2069 7320 696e  bove model is in
-00000ec0: 7469 6c69 617a 6564 2066 726f 6d20 7468  tiliazed from th
-00000ed0: 6520 6f72 6967 696e 616c 2049 6d61 6765  e original Image
-00000ee0: 4e65 7420 7072 652d 7472 6169 6e65 6420  Net pre-trained 
-00000ef0: 4661 7374 6572 5669 5420 7769 7468 206f  FasterViT with o
-00000f00: 7269 6769 6e61 6c20 7265 736f 6c75 7469  riginal resoluti
-00000f10: 6f6e 206f 6620 3232 3420 7820 3232 342e  on of 224 x 224.
-00000f20: 2041 7320 6120 7265 7375 6c74 2c20 6d69   As a result, mi
-00000f30: 7373 696e 6720 6b65 7973 2061 6e64 206d  ssing keys and m
-00000f40: 6973 2d6d 6174 6368 6573 2063 6f75 6c64  is-matches could
-00000f50: 2062 6520 6578 7065 6374 6564 2073 696e   be expected sin
-00000f60: 6365 2077 6520 6172 6520 6164 6469 676e  ce we are addign
-00000f70: 206e 6577 206c 6179 6572 7320 2865 2e67   new layers (e.g
-00000f80: 2e20 6164 6469 7469 6f6e 206f 6620 6e65  . addition of ne
-00000f90: 7720 6361 7272 6965 7220 746f 6b65 6e73  w carrier tokens
-00000fa0: 2c20 6574 632e 2920 0a0a 5765 2063 616e  , etc.) ..We can
-00000fb0: 2073 696d 706c 7920 7465 7374 2074 6865   simply test the
-00000fc0: 206d 6f64 656c 2062 7920 7061 7373 696e   model by passin
-00000fd0: 6720 6120 6475 6d6d 7920 696e 7075 7420  g a dummy input 
-00000fe0: 696d 6167 652e 2054 6865 206f 7574 7075  image. The outpu
-00000ff0: 7420 6973 2074 6865 206c 6f67 6974 733a  t is the logits:
-00001000: 0a0a 6060 6070 7974 686f 6e0a 3e3e 3e20  ..```python.>>> 
-00001010: 696d 706f 7274 2074 6f72 6368 0a0a 3e3e  import torch..>>
-00001020: 3e20 696d 6167 6520 3d20 746f 7263 682e  > image = torch.
-00001030: 7261 6e64 2831 2c20 332c 2035 3736 2c20  rand(1, 3, 576, 
-00001040: 3936 3029 0a3e 3e3e 206f 7574 7075 7420  960).>>> output 
-00001050: 3d20 6d6f 6465 6c28 696d 6167 6529 2023  = model(image) #
-00001060: 2074 6f72 6368 2e53 697a 6528 5b31 2c20   torch.Size([1, 
-00001070: 3130 3030 5d29 0a60 6060 0a0a 2323 20f0  1000]).```..## .
-00001080: 9f92 a520 4e65 7773 20f0 9f92 a50a 0a2d  ... News ......-
-00001090: 202a 2a5b 3037 2e30 342e 3230 3233 5d2a   **[07.04.2023]*
-000010a0: 2a20 f09f 94a5 f09f 94a5 2049 6d61 6765  * ........ Image
-000010b0: 4e65 7420 7072 6574 7261 696e 6564 2046  Net pretrained F
-000010c0: 6173 7465 7256 6954 206d 6f64 656c 7320  asterViT models 
-000010d0: 6361 6e20 6e6f 7720 6265 2069 6d70 6f72  can now be impor
-000010e0: 7465 6420 7769 7468 202a 2a31 206c 696e  ted with **1 lin
-000010f0: 6520 6f66 2063 6f64 652a 2a2e 2050 6c65  e of code**. Ple
-00001100: 6173 6520 696e 7374 616c 6c20 7468 6520  ase install the 
-00001110: 6c61 7465 7374 2046 6173 7465 7256 6954  latest FasterViT
-00001120: 2070 6970 2070 6163 6b61 6765 2074 6f20   pip package to 
-00001130: 7573 6520 7468 6973 2066 756e 6374 696f  use this functio
-00001140: 6e61 6c69 7479 2028 616c 736f 2073 7570  nality (also sup
-00001150: 706f 7274 7320 416e 792d 7265 736f 6c75  ports Any-resolu
-00001160: 7469 6f6e 2046 6173 7465 7256 6954 206d  tion FasterViT m
-00001170: 6f64 656c 7329 2e0a 2d20 2a2a 5b30 362e  odels)..- **[06.
-00001180: 3330 2e32 3032 335d 2a2a 20f0 9f94 a520  30.2023]** .... 
-00001190: 5765 2068 6176 6520 6675 7274 6865 7220  We have further 
-000011a0: 696d 7072 6f76 6564 2074 6865 205b 5465  improved the [Te
-000011b0: 6e73 6f72 5254 5d28 6874 7470 733a 2f2f  nsorRT](https://
-000011c0: 6465 7665 6c6f 7065 722e 6e76 6964 6961  developer.nvidia
-000011d0: 2e63 6f6d 2f74 656e 736f 7272 742d 6765  .com/tensorrt-ge
-000011e0: 7474 696e 672d 7374 6172 7465 6429 2074  tting-started) t
-000011f0: 6872 6f75 6768 7075 7420 6f66 2046 6173  hroughput of Fas
-00001200: 7465 7256 6954 206d 6f64 656c 7320 6279  terViT models by
-00001210: 2031 302d 3135 2520 6f6e 2061 7665 7261   10-15% on avera
-00001220: 6765 2061 6372 6f73 7320 6469 6666 6572  ge across differ
-00001230: 656e 7420 6d6f 6465 6c73 2e20 200a 2d20  ent models.  .- 
-00001240: 2a2a 5b30 362e 3239 2e32 3032 335d 2a2a  **[06.29.2023]**
-00001250: 2041 6e79 2d72 6573 6f6c 7574 696f 6e20   Any-resolution 
-00001260: 4661 7374 6572 5669 5420 6d6f 6465 6c20  FasterViT model 
-00001270: 6361 6e20 6e6f 7720 6265 2069 6e74 6974  can now be intit
-00001280: 6961 6c69 7a65 6420 6672 6f6d 2070 7265  ialized from pre
-00001290: 2d74 7261 696e 6564 2049 6d61 6765 4e65  -trained ImageNe
-000012a0: 7420 7265 736f 6c75 7469 6f6e 2028 3232  t resolution (22
-000012b0: 3420 7820 3234 3429 206d 6f64 656c 732e  4 x 244) models.
-000012c0: 0a2d 202a 2a5b 3036 2e31 382e 3230 3233  .- **[06.18.2023
-000012d0: 5d2a 2a20 5765 2068 6176 6520 7265 6c65  ]** We have rele
-000012e0: 6173 6564 2074 6865 2046 6173 7465 7256  ased the FasterV
-000012f0: 6954 205b 7069 7020 7061 636b 6167 655d  iT [pip package]
-00001300: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
-00001310: 672f 7072 6f6a 6563 742f 6661 7374 6572  g/project/faster
-00001320: 7669 742f 2920 210a 2d20 2a2a 5b30 362e  vit/) !.- **[06.
-00001330: 3137 2e32 3032 335d 2a2a 20f0 9f94 a520  17.2023]** .... 
-00001340: 5b41 6e79 2d72 6573 6f6c 7574 696f 6e20  [Any-resolution 
-00001350: 4661 7374 6572 5669 545d 282e 2f66 6173  FasterViT](./fas
-00001360: 7465 7276 6974 2f6d 6f64 656c 732f 6661  tervit/models/fa
-00001370: 7374 6572 5f76 6974 5f61 6e79 5f72 6573  ster_vit_any_res
-00001380: 2e70 7929 2020 6d6f 6465 6c20 6973 206e  .py)  model is n
-00001390: 6f77 2061 7661 696c 6162 6c65 2021 2074  ow available ! t
-000013a0: 6865 206d 6f64 656c 2063 616e 2062 6520  he model can be 
-000013b0: 7573 6564 2066 6f72 2076 6172 6965 7479  used for variety
-000013c0: 206f 6620 6170 706c 6963 6174 696f 6e73   of applications
-000013d0: 2073 7563 6820 6173 2064 6574 6563 7469   such as detecti
-000013e0: 6f6e 2061 6e64 2073 6567 6d65 6e74 6174  on and segmentat
-000013f0: 696f 6e20 6f72 2068 6967 682d 7265 736f  ion or high-reso
-00001400: 6c75 7469 6f6e 2066 696e 652d 7475 6e69  lution fine-tuni
-00001410: 6e67 2077 6974 6820 6172 6269 7472 6172  ng with arbitrar
-00001420: 7920 696e 7075 7420 696d 6167 6520 7265  y input image re
-00001430: 736f 6c75 7469 6f6e 732e 0a2d 202a 2a5b  solutions..- **[
-00001440: 3036 2e30 392e 3230 3233 5d2a 2a20 f09f  06.09.2023]** ..
-00001450: 94a5 f09f 94a5 2057 6520 6861 7665 2072  ...... We have r
-00001460: 656c 6561 7365 6420 736f 7572 6365 2063  eleased source c
-00001470: 6f64 6520 616e 6420 496d 6167 654e 6574  ode and ImageNet
-00001480: 2d31 4b20 4661 7374 6572 5669 542d 6d6f  -1K FasterViT-mo
-00001490: 6465 6c73 2021 0a0a 0a23 2320 4361 7461  dels !...## Cata
-000014a0: 6c6f 670a 2d20 5b78 5d20 496d 6167 654e  log.- [x] ImageN
-000014b0: 6574 2d31 4b20 7472 6169 6e69 6e67 2063  et-1K training c
-000014c0: 6f64 650a 2d20 5b78 5d20 496d 6167 654e  ode.- [x] ImageN
-000014d0: 6574 2d31 4b20 7072 652d 7472 6169 6e65  et-1K pre-traine
-000014e0: 6420 6d6f 6465 6c73 0a2d 205b 785d 2041  d models.- [x] A
-000014f0: 6e79 2d72 6573 6f6c 7574 696f 6e20 4661  ny-resolution Fa
-00001500: 7374 6572 5669 540a 2d20 5b78 5d20 4661  sterViT.- [x] Fa
-00001510: 7374 6572 5669 5420 7069 702d 7061 636b  sterViT pip-pack
-00001520: 6167 6520 7265 6c65 6173 650a 2d20 5b78  age release.- [x
-00001530: 5d20 4164 6420 6361 7061 626c 6974 7920  ] Add capablity 
-00001540: 746f 2069 6e69 7469 616c 697a 6520 616e  to initialize an
-00001550: 792d 7265 736f 6c75 7469 6f6e 2046 6173  y-resolution Fas
-00001560: 7465 7256 6954 2066 726f 6d20 496d 6167  terViT from Imag
-00001570: 654e 6574 2d70 7265 7472 6169 6e65 6420  eNet-pretrained 
-00001580: 7765 6967 6874 732e 200a 2d20 5b20 5d20  weights. .- [ ] 
-00001590: 496d 6167 654e 6574 2d32 314b 2070 7265  ImageNet-21K pre
-000015a0: 2d74 7261 696e 6564 206d 6f64 656c 730a  -trained models.
-000015b0: 2d20 5b20 5d20 4465 7465 6374 696f 6e20  - [ ] Detection 
-000015c0: 636f 6465 2028 4449 4e4f 2920 2b20 6d6f  code (DINO) + mo
-000015d0: 6465 6c73 0a2d 205b 205d 2053 6567 6d65  dels.- [ ] Segme
-000015e0: 6e74 6174 696f 6e20 636f 6465 202b 206d  ntation code + m
-000015f0: 6f64 656c 730a 0a2d 2d2d 200a 0a23 2320  odels..--- ..## 
-00001600: 5265 7375 6c74 7320 2b20 5072 6574 7261  Results + Pretra
-00001610: 696e 6564 204d 6f64 656c 730a 0a23 2323  ined Models..###
-00001620: 2049 6d61 6765 4e65 742d 314b 0a2a 2a46   ImageNet-1K.**F
-00001630: 6173 7465 7256 6954 2049 6d61 6765 4e65  asterViT ImageNe
-00001640: 742d 314b 2050 7265 7472 6169 6e65 6420  t-1K Pretrained 
-00001650: 4d6f 6465 6c73 2a2a 0a0a 3c74 6162 6c65  Models**..<table
-00001660: 3e0a 2020 3c74 723e 0a20 2020 203c 7468  >.  <tr>.    <th
-00001670: 3e4e 616d 653c 2f74 683e 0a20 2020 203c  >Name</th>.    <
-00001680: 7468 3e41 6363 4031 2825 293c 2f74 683e  th>Acc@1(%)</th>
-00001690: 0a20 2020 203c 7468 3e41 6363 4035 2825  .    <th>Acc@5(%
-000016a0: 293c 2f74 683e 0a20 2020 203c 7468 3e54  )</th>.    <th>T
-000016b0: 6872 6f75 6768 7075 7428 496d 672f 5365  hroughput(Img/Se
-000016c0: 6329 3c2f 7468 3e0a 2020 2020 3c74 683e  c)</th>.    <th>
-000016d0: 5265 736f 6c75 7469 6f6e 3c2f 7468 3e0a  Resolution</th>.
-000016e0: 2020 2020 3c74 683e 2350 6172 616d 7328      <th>#Params(
-000016f0: 4d29 3c2f 7468 3e0a 2020 2020 3c74 683e  M)</th>.    <th>
-00001700: 464c 4f50 7328 4729 3c2f 7468 3e0a 2020  FLOPs(G)</th>.  
-00001710: 2020 3c74 683e 446f 776e 6c6f 6164 3c2f    <th>Download</
-00001720: 7468 3e0a 2020 3c2f 7472 3e0a 0a3c 7472  th>.  </tr>..<tr
-00001730: 3e0a 2020 2020 3c74 643e 4661 7374 6572  >.    <td>Faster
-00001740: 5669 542d 303c 2f74 643e 0a20 2020 203c  ViT-0</td>.    <
-00001750: 7464 3e38 322e 313c 2f74 643e 0a20 2020  td>82.1</td>.   
-00001760: 203c 7464 3e39 352e 393c 2f74 643e 0a20   <td>95.9</td>. 
-00001770: 2020 203c 7464 3e35 3830 323c 2f74 643e     <td>5802</td>
-00001780: 0a20 2020 203c 7464 3e32 3234 7832 3234  .    <td>224x224
-00001790: 3c2f 7464 3e0a 2020 2020 3c74 643e 3331  </td>.    <td>31
-000017a0: 2e34 3c2f 7464 3e0a 2020 2020 3c74 643e  .4</td>.    <td>
-000017b0: 332e 333c 2f74 643e 0a20 2020 203c 7464  3.3</td>.    <td
-000017c0: 3e3c 6120 6872 6566 3d22 6874 7470 733a  ><a href="https:
-000017d0: 2f2f 6472 6976 652e 676f 6f67 6c65 2e63  //drive.google.c
-000017e0: 6f6d 2f75 633f 6578 706f 7274 3d64 6f77  om/uc?export=dow
-000017f0: 6e6c 6f61 6426 6964 3d31 7477 4932 4c46  nload&id=1twI2LF
-00001800: 4a73 3339 3159 726a 384d 5234 5569 3950  Js391Yrj8MR4Ui9P
-00001810: 6672 7657 716a 4531 6942 223e 6d6f 6465  frvWqjE1iB">mode
-00001820: 6c3c 2f61 3e3c 2f74 643e 0a3c 2f74 723e  l</a></td>.</tr>
-00001830: 0a0a 3c74 723e 0a20 2020 203c 7464 3e46  ..<tr>.    <td>F
-00001840: 6173 7465 7256 6954 2d31 3c2f 7464 3e0a  asterViT-1</td>.
-00001850: 2020 2020 3c74 643e 3833 2e32 3c2f 7464      <td>83.2</td
-00001860: 3e0a 2020 2020 3c74 643e 3936 2e35 3c2f  >.    <td>96.5</
-00001870: 7464 3e0a 2020 2020 3c74 643e 3431 3838  td>.    <td>4188
-00001880: 3c2f 7464 3e0a 2020 2020 3c74 643e 3232  </td>.    <td>22
-00001890: 3478 3232 343c 2f74 643e 0a20 2020 203c  4x224</td>.    <
-000018a0: 7464 3e35 332e 343c 2f74 643e 0a20 2020  td>53.4</td>.   
-000018b0: 203c 7464 3e35 2e33 3c2f 7464 3e0a 2020   <td>5.3</td>.  
-000018c0: 2020 3c74 643e 3c61 2068 7265 663d 2268    <td><a href="h
-000018d0: 7474 7073 3a2f 2f64 7269 7665 2e67 6f6f  ttps://drive.goo
-000018e0: 676c 652e 636f 6d2f 7563 3f65 7870 6f72  gle.com/uc?expor
-000018f0: 743d 646f 776e 6c6f 6164 2669 643d 3172  t=download&id=1r
-00001900: 3757 3130 6e35 2d62 4674 4d33 737a 3462  7W10n5-bFtM3sz4b
-00001910: 6d61 4c72 6f77 4e32 6759 506b 4c47 5422  maLrowN2gYPkLGT"
-00001920: 3e6d 6f64 656c 3c2f 613e 3c2f 7464 3e0a  >model</a></td>.
-00001930: 3c2f 7472 3e0a 0a3c 7472 3e0a 2020 2020  </tr>..<tr>.    
-00001940: 3c74 643e 4661 7374 6572 5669 542d 323c  <td>FasterViT-2<
-00001950: 2f74 643e 0a20 2020 203c 7464 3e38 342e  /td>.    <td>84.
-00001960: 323c 2f74 643e 0a20 2020 203c 7464 3e39  2</td>.    <td>9
-00001970: 362e 383c 2f74 643e 0a20 2020 203c 7464  6.8</td>.    <td
-00001980: 3e33 3136 313c 2f74 643e 0a20 2020 203c  >3161</td>.    <
-00001990: 7464 3e32 3234 7832 3234 3c2f 7464 3e0a  td>224x224</td>.
-000019a0: 2020 2020 3c74 643e 3735 2e39 3c2f 7464      <td>75.9</td
-000019b0: 3e0a 2020 2020 3c74 643e 382e 373c 2f74  >.    <td>8.7</t
-000019c0: 643e 0a20 2020 203c 7464 3e3c 6120 6872  d>.    <td><a hr
-000019d0: 6566 3d22 6874 7470 733a 2f2f 6472 6976  ef="https://driv
-000019e0: 652e 676f 6f67 6c65 2e63 6f6d 2f75 633f  e.google.com/uc?
-000019f0: 6578 706f 7274 3d64 6f77 6e6c 6f61 6426  export=download&
-00001a00: 6964 3d31 6e5f 6136 7330 7067 6930 6a56  id=1n_a6s0pgi0jV
-00001a10: 5a4f 476d 4465 6932 7658 4855 3545 3652  ZOGmDei2vXHU5E6R
-00001a20: 4835 7755 223e 6d6f 6465 6c3c 2f61 3e3c  H5wU">model</a><
-00001a30: 2f74 643e 0a3c 2f74 723e 0a0a 3c74 723e  /td>.</tr>..<tr>
-00001a40: 0a20 2020 203c 7464 3e46 6173 7465 7256  .    <td>FasterV
-00001a50: 6954 2d33 3c2f 7464 3e0a 2020 2020 3c74  iT-3</td>.    <t
-00001a60: 643e 3834 2e39 3c2f 7464 3e0a 2020 2020  d>84.9</td>.    
-00001a70: 3c74 643e 3937 2e32 3c2f 7464 3e0a 2020  <td>97.2</td>.  
-00001a80: 2020 3c74 643e 3137 3830 3c2f 7464 3e0a    <td>1780</td>.
-00001a90: 2020 2020 3c74 643e 3232 3478 3232 343c      <td>224x224<
-00001aa0: 2f74 643e 0a20 2020 203c 7464 3e31 3539  /td>.    <td>159
-00001ab0: 2e35 3c2f 7464 3e0a 2020 2020 3c74 643e  .5</td>.    <td>
-00001ac0: 3138 2e32 3c2f 7464 3e0a 2020 2020 3c74  18.2</td>.    <t
-00001ad0: 643e 3c61 2068 7265 663d 2268 7474 7073  d><a href="https
-00001ae0: 3a2f 2f64 7269 7665 2e67 6f6f 676c 652e  ://drive.google.
-00001af0: 636f 6d2f 7563 3f65 7870 6f72 743d 646f  com/uc?export=do
-00001b00: 776e 6c6f 6164 2669 643d 3174 7657 456c  wnload&id=1tvWEl
-00001b10: 5a39 3153 6961 3253 7358 5958 464d 4e59  Z91Sia2SsXYXFMNY
-00001b20: 5177 6669 7043 7874 4937 5822 3e6d 6f64  QwfipCxtI7X">mod
-00001b30: 656c 3c2f 613e 3c2f 7464 3e0a 3c2f 7472  el</a></td>.</tr
-00001b40: 3e0a 0a3c 7472 3e0a 2020 2020 3c74 643e  >..<tr>.    <td>
-00001b50: 4661 7374 6572 5669 542d 343c 2f74 643e  FasterViT-4</td>
-00001b60: 0a20 2020 203c 7464 3e38 352e 343c 2f74  .    <td>85.4</t
-00001b70: 643e 0a20 2020 203c 7464 3e39 372e 333c  d>.    <td>97.3<
-00001b80: 2f74 643e 0a20 2020 203c 7464 3e38 3439  /td>.    <td>849
-00001b90: 3c2f 7464 3e0a 2020 2020 3c74 643e 3232  </td>.    <td>22
-00001ba0: 3478 3232 343c 2f74 643e 0a20 2020 203c  4x224</td>.    <
-00001bb0: 7464 3e34 3234 2e36 3c2f 7464 3e0a 2020  td>424.6</td>.  
-00001bc0: 2020 3c74 643e 3336 2e36 3c2f 7464 3e0a    <td>36.6</td>.
-00001bd0: 2020 2020 3c74 643e 3c61 2068 7265 663d      <td><a href=
-00001be0: 2268 7474 7073 3a2f 2f64 7269 7665 2e67  "https://drive.g
-00001bf0: 6f6f 676c 652e 636f 6d2f 7563 3f65 7870  oogle.com/uc?exp
-00001c00: 6f72 743d 646f 776e 6c6f 6164 2669 643d  ort=download&id=
-00001c10: 3167 5968 5841 3332 512d 5f39 4335 4458  1gYhXA32Q-_9C5DX
-00001c20: 656c 3137 6176 565f 5a4c 6f61 4877 6467  el17avV_ZLoaHwdg
-00001c30: 7a22 3e6d 6f64 656c 3c2f 613e 3c2f 7464  z">model</a></td
-00001c40: 3e0a 3c2f 7472 3e0a 0a3c 7472 3e0a 2020  >.</tr>..<tr>.  
-00001c50: 2020 3c74 643e 4661 7374 6572 5669 542d    <td>FasterViT-
-00001c60: 353c 2f74 643e 0a20 2020 203c 7464 3e38  5</td>.    <td>8
-00001c70: 352e 363c 2f74 643e 0a20 2020 203c 7464  5.6</td>.    <td
-00001c80: 3e39 372e 343c 2f74 643e 0a20 2020 203c  >97.4</td>.    <
-00001c90: 7464 3e34 3439 3c2f 7464 3e0a 2020 2020  td>449</td>.    
-00001ca0: 3c74 643e 3232 3478 3232 343c 2f74 643e  <td>224x224</td>
-00001cb0: 0a20 2020 203c 7464 3e39 3735 2e35 3c2f  .    <td>975.5</
-00001cc0: 7464 3e0a 2020 2020 3c74 643e 3131 332e  td>.    <td>113.
-00001cd0: 303c 2f74 643e 0a20 2020 203c 7464 3e3c  0</td>.    <td><
-00001ce0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00001cf0: 6472 6976 652e 676f 6f67 6c65 2e63 6f6d  drive.google.com
-00001d00: 2f75 633f 6578 706f 7274 3d64 6f77 6e6c  /uc?export=downl
-00001d10: 6f61 6426 6964 3d31 6d71 7061 6937 5869  oad&id=1mqpai7Xi
-00001d20: 484c 725f 6e31 746a 786a 7a54 3871 3336  HLr_n1tjxjzT8q36
-00001d30: 3978 5443 715f 7a2d 223e 6d6f 6465 6c3c  9xTCq_z-">model<
-00001d40: 2f61 3e3c 2f74 643e 0a3c 2f74 723e 0a0a  /a></td>.</tr>..
-00001d50: 3c74 723e 0a20 2020 203c 7464 3e46 6173  <tr>.    <td>Fas
-00001d60: 7465 7256 6954 2d36 3c2f 7464 3e0a 2020  terViT-6</td>.  
-00001d70: 2020 3c74 643e 3835 2e38 3c2f 7464 3e0a    <td>85.8</td>.
-00001d80: 2020 2020 3c74 643e 3937 2e34 3c2f 7464      <td>97.4</td
-00001d90: 3e0a 2020 2020 3c74 643e 3335 323c 2f74  >.    <td>352</t
-00001da0: 643e 0a20 2020 203c 7464 3e32 3234 7832  d>.    <td>224x2
-00001db0: 3234 3c2f 7464 3e0a 2020 2020 3c74 643e  24</td>.    <td>
-00001dc0: 3133 3630 2e30 3c2f 7464 3e0a 2020 2020  1360.0</td>.    
-00001dd0: 3c74 643e 3134 322e 303c 2f74 643e 0a20  <td>142.0</td>. 
-00001de0: 2020 203c 7464 3e3c 6120 6872 6566 3d22     <td><a href="
-00001df0: 6874 7470 733a 2f2f 6472 6976 652e 676f  https://drive.go
-00001e00: 6f67 6c65 2e63 6f6d 2f75 633f 6578 706f  ogle.com/uc?expo
-00001e10: 7274 3d64 6f77 6e6c 6f61 6426 6964 3d31  rt=download&id=1
-00001e20: 326a 7461 7652 3251 786d 4d7a 634b 7750  2jtavR2QxmMzcKwP
-00001e30: 7a57 6537 6b77 2d6f 7933 3449 5969 3539  zWe7kw-oy34IYi59
-00001e40: 223e 6d6f 6465 6c3c 2f61 3e3c 2f74 643e  ">model</a></td>
-00001e50: 0a3c 2f74 723e 0a0a 3c2f 7461 626c 653e  .</tr>..</table>
-00001e60: 0a0a 0a23 2323 2052 6f62 7573 746e 6573  ...### Robustnes
-00001e70: 7320 2849 6d61 6765 4e65 742d 4120 2d20  s (ImageNet-A - 
-00001e80: 496d 6167 654e 6574 2d52 202d 2049 6d61  ImageNet-R - Ima
-00001e90: 6765 4e65 742d 5632 290a 0a41 6c6c 206d  geNet-V2)..All m
-00001ea0: 6f64 656c 7320 7573 6520 6063 726f 705f  odels use `crop_
-00001eb0: 7063 743d 302e 3837 3560 2e20 5265 7375  pct=0.875`. Resu
-00001ec0: 6c74 7320 6172 6520 6f62 7461 696e 6564  lts are obtained
-00001ed0: 2062 7920 7275 6e6e 696e 6720 696e 6665   by running infe
-00001ee0: 7265 6e63 6520 6f6e 2049 6d61 6765 4e65  rence on ImageNe
-00001ef0: 742d 314b 2070 7265 7472 6169 6e65 6420  t-1K pretrained 
-00001f00: 6d6f 6465 6c73 2077 6974 686f 7574 2066  models without f
-00001f10: 696e 6574 756e 696e 672e 0a3c 7461 626c  inetuning..<tabl
-00001f20: 653e 0a20 203c 7472 3e0a 2020 2020 3c74  e>.  <tr>.    <t
-00001f30: 683e 4e61 6d65 3c2f 7468 3e0a 2020 2020  h>Name</th>.    
-00001f40: 3c74 683e 412d 4163 6340 3128 2529 3c2f  <th>A-Acc@1(%)</
-00001f50: 7468 3e0a 2020 2020 3c74 683e 412d 4163  th>.    <th>A-Ac
-00001f60: 6340 3528 2529 3c2f 7468 3e0a 2020 2020  c@5(%)</th>.    
-00001f70: 3c74 683e 522d 4163 6340 3128 2529 3c2f  <th>R-Acc@1(%)</
-00001f80: 7468 3e0a 2020 2020 3c74 683e 522d 4163  th>.    <th>R-Ac
-00001f90: 6340 3528 2529 3c2f 7468 3e0a 2020 2020  c@5(%)</th>.    
-00001fa0: 3c74 683e 5632 2d41 6363 4031 2825 293c  <th>V2-Acc@1(%)<
-00001fb0: 2f74 683e 0a20 2020 203c 7468 3e56 322d  /th>.    <th>V2-
-00001fc0: 4163 6340 3528 2529 3c2f 7468 3e0a 2020  Acc@5(%)</th>.  
-00001fd0: 3c2f 7472 3e0a 0a3c 7472 3e0a 2020 2020  </tr>..<tr>.    
-00001fe0: 3c74 643e 4661 7374 6572 5669 542d 303c  <td>FasterViT-0<
-00001ff0: 2f74 643e 0a20 2020 203c 7464 3e32 332e  /td>.    <td>23.
-00002000: 393c 2f74 643e 0a20 2020 203c 7464 3e35  9</td>.    <td>5
-00002010: 372e 363c 2f74 643e 0a20 2020 203c 7464  7.6</td>.    <td
-00002020: 3e34 352e 393c 2f74 643e 0a20 2020 203c  >45.9</td>.    <
-00002030: 7464 3e36 302e 343c 2f74 643e 0a20 2020  td>60.4</td>.   
-00002040: 203c 7464 3e37 302e 393c 2f74 643e 0a20   <td>70.9</td>. 
-00002050: 2020 203c 7464 3e39 302e 303c 2f74 643e     <td>90.0</td>
-00002060: 0a3c 2f74 723e 0a0a 3c74 723e 0a20 2020  .</tr>..<tr>.   
-00002070: 203c 7464 3e46 6173 7465 7256 6954 2d31   <td>FasterViT-1
-00002080: 3c2f 7464 3e0a 2020 2020 3c74 643e 3331  </td>.    <td>31
-00002090: 2e32 3c2f 7464 3e0a 2020 2020 3c74 643e  .2</td>.    <td>
-000020a0: 3633 2e33 3c2f 7464 3e0a 2020 2020 3c74  63.3</td>.    <t
-000020b0: 643e 3437 2e35 3c2f 7464 3e0a 2020 2020  d>47.5</td>.    
-000020c0: 3c74 643e 3631 2e39 3c2f 7464 3e0a 2020  <td>61.9</td>.  
-000020d0: 2020 3c74 643e 3732 2e36 3c2f 7464 3e0a    <td>72.6</td>.
-000020e0: 2020 2020 3c74 643e 3931 2e30 3c2f 7464      <td>91.0</td
-000020f0: 3e0a 3c2f 7472 3e0a 0a3c 7472 3e0a 2020  >.</tr>..<tr>.  
-00002100: 2020 3c74 643e 4661 7374 6572 5669 542d    <td>FasterViT-
-00002110: 323c 2f74 643e 0a20 2020 203c 7464 3e33  2</td>.    <td>3
-00002120: 382e 323c 2f74 643e 0a20 2020 203c 7464  8.2</td>.    <td
-00002130: 3e36 382e 393c 2f74 643e 0a20 2020 203c  >68.9</td>.    <
-00002140: 7464 3e34 392e 363c 2f74 643e 0a20 2020  td>49.6</td>.   
-00002150: 203c 7464 3e36 332e 343c 2f74 643e 0a20   <td>63.4</td>. 
-00002160: 2020 203c 7464 3e37 332e 373c 2f74 643e     <td>73.7</td>
-00002170: 0a20 2020 203c 7464 3e39 312e 363c 2f74  .    <td>91.6</t
-00002180: 643e 0a3c 2f74 723e 0a0a 3c74 723e 0a20  d>.</tr>..<tr>. 
-00002190: 2020 203c 7464 3e46 6173 7465 7256 6954     <td>FasterViT
-000021a0: 2d33 3c2f 7464 3e0a 2020 2020 3c74 643e  -3</td>.    <td>
-000021b0: 3434 2e32 3c2f 7464 3e0a 2020 2020 3c74  44.2</td>.    <t
-000021c0: 643e 3733 2e30 3c2f 7464 3e0a 2020 2020  d>73.0</td>.    
-000021d0: 3c74 643e 3531 2e39 3c2f 7464 3e0a 2020  <td>51.9</td>.  
-000021e0: 2020 3c74 643e 3635 2e36 3c2f 7464 3e0a    <td>65.6</td>.
-000021f0: 2020 2020 3c74 643e 3735 2e30 3c2f 7464      <td>75.0</td
-00002200: 3e0a 2020 2020 3c74 643e 3932 2e32 3c2f  >.    <td>92.2</
-00002210: 7464 3e0a 3c2f 7472 3e0a 0a3c 7472 3e0a  td>.</tr>..<tr>.
-00002220: 2020 2020 3c74 643e 4661 7374 6572 5669      <td>FasterVi
-00002230: 542d 343c 2f74 643e 0a20 2020 203c 7464  T-4</td>.    <td
-00002240: 3e34 392e 303c 2f74 643e 0a20 2020 203c  >49.0</td>.    <
-00002250: 7464 3e37 352e 343c 2f74 643e 0a20 2020  td>75.4</td>.   
-00002260: 203c 7464 3e35 362e 303c 2f74 643e 0a20   <td>56.0</td>. 
-00002270: 2020 203c 7464 3e36 392e 363c 2f74 643e     <td>69.6</td>
-00002280: 0a20 2020 203c 7464 3e37 352e 373c 2f74  .    <td>75.7</t
-00002290: 643e 0a20 2020 203c 7464 3e39 322e 373c  d>.    <td>92.7<
-000022a0: 2f74 643e 0a3c 2f74 723e 0a0a 3c74 723e  /td>.</tr>..<tr>
-000022b0: 0a20 2020 203c 7464 3e46 6173 7465 7256  .    <td>FasterV
-000022c0: 6954 2d35 3c2f 7464 3e0a 2020 2020 3c74  iT-5</td>.    <t
-000022d0: 643e 3532 2e37 3c2f 7464 3e0a 2020 2020  d>52.7</td>.    
-000022e0: 3c74 643e 3737 2e36 3c2f 7464 3e0a 2020  <td>77.6</td>.  
-000022f0: 2020 3c74 643e 3536 2e39 3c2f 7464 3e0a    <td>56.9</td>.
-00002300: 2020 2020 3c74 643e 3730 2e30 3c2f 7464      <td>70.0</td
-00002310: 3e0a 2020 2020 3c74 643e 3736 2e30 3c2f  >.    <td>76.0</
-00002320: 7464 3e0a 2020 2020 3c74 643e 3933 2e30  td>.    <td>93.0
-00002330: 3c2f 7464 3e0a 3c2f 7472 3e0a 0a3c 7472  </td>.</tr>..<tr
-00002340: 3e0a 2020 2020 3c74 643e 4661 7374 6572  >.    <td>Faster
-00002350: 5669 542d 363c 2f74 643e 0a20 2020 203c  ViT-6</td>.    <
-00002360: 7464 3e35 332e 373c 2f74 643e 0a20 2020  td>53.7</td>.   
-00002370: 203c 7464 3e37 382e 343c 2f74 643e 0a20   <td>78.4</td>. 
-00002380: 2020 203c 7464 3e35 372e 313c 2f74 643e     <td>57.1</td>
-00002390: 0a20 2020 203c 7464 3e37 302e 313c 2f74  .    <td>70.1</t
-000023a0: 643e 0a20 2020 203c 7464 3e37 362e 313c  d>.    <td>76.1<
-000023b0: 2f74 643e 0a20 2020 203c 7464 3e39 332e  /td>.    <td>93.
-000023c0: 303c 2f74 643e 0a3c 2f74 723e 0a0a 3c2f  0</td>.</tr>..</
-000023d0: 7461 626c 653e 0a0a 412c 2052 2061 6e64  table>..A, R and
-000023e0: 2056 3220 6465 6e6f 7465 2049 6d61 6765   V2 denote Image
-000023f0: 4e65 742d 412c 2049 6d61 6765 4e65 742d  Net-A, ImageNet-
-00002400: 5220 616e 6420 496d 6167 654e 6574 2d56  R and ImageNet-V
-00002410: 3220 7265 7370 6563 7469 7665 6c79 2e20  2 respectively. 
-00002420: 0a23 2320 5472 6169 6e69 6e67 0a0a 506c  .## Training..Pl
-00002430: 6561 7365 2073 6565 205b 5452 4149 4e49  ease see [TRAINI
-00002440: 4e47 2e6d 645d 2854 5241 494e 494e 472e  NG.md](TRAINING.
-00002450: 6d64 2920 666f 7220 6465 7461 696c 6564  md) for detailed
-00002460: 2074 7261 696e 696e 6720 696e 7374 7275   training instru
-00002470: 6374 696f 6e73 206f 6620 616c 6c20 6d6f  ctions of all mo
-00002480: 6465 6c73 2e20 0a0a 2323 2045 7661 6c75  dels. ..## Evalu
-00002490: 6174 696f 6e0a 0a54 6865 2046 6173 7465  ation..The Faste
-000024a0: 7256 6954 206d 6f64 656c 7320 6361 6e20  rViT models can 
-000024b0: 6265 2065 7661 6c75 6174 6564 206f 6e20  be evaluated on 
-000024c0: 496d 6167 654e 6574 2d31 4b20 7661 6c69  ImageNet-1K vali
-000024d0: 6461 7469 6f6e 2073 6574 2075 7369 6e67  dation set using
-000024e0: 2074 6865 2066 6f6c 6c6f 7769 6e67 3a20   the following: 
-000024f0: 0a0a 6060 600a 7079 7468 6f6e 2076 616c  ..```.python val
-00002500: 6964 6174 652e 7079 205c 0a2d 2d6d 6f64  idate.py \.--mod
-00002510: 656c 203c 6d6f 6465 6c2d 6e61 6d65 3e0a  el <model-name>.
-00002520: 2d2d 6368 6563 6b70 6f69 6e74 203c 6368  --checkpoint <ch
-00002530: 6563 6b70 6f69 6e74 2d70 6174 683e 0a2d  eckpoint-path>.-
-00002540: 2d64 6174 615f 6469 7220 3c69 6d61 6765  -data_dir <image
-00002550: 6e65 742d 7061 7468 3e0a 2d2d 6261 7463  net-path>.--batc
-00002560: 682d 7369 7a65 203c 6261 7463 682d 7369  h-size <batch-si
-00002570: 7a65 2d70 6572 2d67 7075 0a60 6060 200a  ze-per-gpu.``` .
-00002580: 0a48 6572 6520 602d 2d6d 6f64 656c 6020  .Here `--model` 
-00002590: 6973 2074 6865 2046 6173 7465 7256 6954  is the FasterViT
-000025a0: 2076 6172 6961 6e74 2028 652e 672e 2060   variant (e.g. `
-000025b0: 6661 7374 6572 5f76 6974 5f30 5f32 3234  faster_vit_0_224
-000025c0: 5f31 6b60 292c 2060 2d2d 6368 6563 6b70  _1k`), `--checkp
-000025d0: 6f69 6e74 6020 6973 2074 6865 2070 6174  oint` is the pat
-000025e0: 6820 746f 2070 7265 7472 6169 6e65 6420  h to pretrained 
-000025f0: 6d6f 6465 6c20 7765 6967 6874 732c 2060  model weights, `
-00002600: 2d2d 6461 7461 5f64 6972 6020 6973 2074  --data_dir` is t
-00002610: 6865 2070 6174 6820 746f 2049 6d61 6765  he path to Image
-00002620: 4e65 742d 314b 2076 616c 6964 6174 696f  Net-1K validatio
-00002630: 6e20 7365 7420 616e 6420 602d 2d62 6174  n set and `--bat
-00002640: 6368 2d73 697a 6560 2069 7320 7468 6520  ch-size` is the 
-00002650: 6e75 6d62 6572 206f 6620 6261 7463 6820  number of batch 
-00002660: 7369 7a65 2e20 5765 2061 6c73 6f20 7072  size. We also pr
-00002670: 6f76 6964 6520 6120 7361 6d70 6c65 2073  ovide a sample s
-00002680: 6372 6970 7420 5b68 6572 655d 282e 2f66  cript [here](./f
-00002690: 6173 7465 7276 6974 2f76 616c 6964 6174  astervit/validat
-000026a0: 652e 7368 292e 200a 0a23 2320 4f4e 4e58  e.sh). ..## ONNX
-000026b0: 2043 6f6e 7665 7273 696f 6e0a 0a57 6520   Conversion..We 
-000026c0: 7072 6f76 6964 6520 4f4e 4e58 2063 6f6e  provide ONNX con
-000026d0: 7665 7273 696f 6e20 7363 7269 7074 2074  version script t
-000026e0: 6f20 656e 6162 6c65 2064 796e 616d 6963  o enable dynamic
-000026f0: 2062 6174 6368 2073 697a 6520 696e 6665   batch size infe
-00002700: 7265 6e63 652e 2046 6f72 2069 6e73 7461  rence. For insta
-00002710: 6e63 652c 2074 6f20 6765 6e65 7261 7465  nce, to generate
-00002720: 204f 4e4e 5820 6d6f 6465 6c20 666f 7220   ONNX model for 
-00002730: 6066 6173 7465 725f 7669 745f 305f 616e  `faster_vit_0_an
-00002740: 795f 7265 7360 2077 6974 6820 7265 736f  y_res` with reso
-00002750: 6c75 7469 6f6e 2035 3736 2078 2039 3630  lution 576 x 960
-00002760: 2061 6e64 204f 4e4e 5820 6f70 7365 7420   and ONNX opset 
-00002770: 6e75 6d62 6572 2031 372c 2074 6865 2066  number 17, the f
-00002780: 6f6c 6c6f 7769 6e67 2063 616e 2062 6520  ollowing can be 
-00002790: 7573 6564 2e20 0a0a 6060 6062 6173 6820  used. ..```bash 
-000027a0: 0a70 7974 686f 6e20 6f6e 6e78 5f63 6f6e  .python onnx_con
-000027b0: 7665 7274 202d 2d6d 6f64 656c 2d6e 616d  vert --model-nam
-000027c0: 6520 6661 7374 6572 5f76 6974 5f30 5f61  e faster_vit_0_a
-000027d0: 6e79 5f72 6573 202d 2d72 6573 6f6c 7574  ny_res --resolut
-000027e0: 696f 6e2d 6820 3537 3620 2d2d 7265 736f  ion-h 576 --reso
-000027f0: 6c75 7469 6f6e 2d77 2039 3630 202d 2d6f  lution-w 960 --o
-00002800: 6e6e 782d 6f70 7365 7420 3137 0a0a 6060  nnx-opset 17..``
-00002810: 600a 0a0a 2323 2049 6e73 7461 6c6c 6174  `...## Installat
-00002820: 696f 6e0a 0a54 6865 2064 6570 656e 6465  ion..The depende
-00002830: 6e63 6965 7320 6361 6e20 6265 2069 6e73  ncies can be ins
-00002840: 7461 6c6c 6564 2062 7920 7275 6e6e 696e  talled by runnin
-00002850: 673a 0a0a 6060 6062 6173 680a 7069 7020  g:..```bash.pip 
-00002860: 696e 7374 616c 6c20 2d72 2072 6571 7569  install -r requi
-00002870: 7265 6d65 6e74 732e 7478 740a 6060 600a  rements.txt.```.
-00002880: 0a23 2320 5374 6172 2048 6973 746f 7279  .## Star History
-00002890: 0a0a 5b21 5b53 7461 7220 4869 7374 6f72  ..[![Star Histor
-000028a0: 7920 4368 6172 745d 2868 7474 7073 3a2f  y Chart](https:/
-000028b0: 2f61 7069 2e73 7461 722d 6869 7374 6f72  /api.star-histor
-000028c0: 792e 636f 6d2f 7376 673f 7265 706f 733d  y.com/svg?repos=
-000028d0: 4e56 6c61 6273 2f46 6173 7465 7256 6954  NVlabs/FasterViT
-000028e0: 2674 7970 653d 4461 7465 295d 2868 7474  &type=Date)](htt
-000028f0: 7073 3a2f 2f73 7461 722d 6869 7374 6f72  ps://star-histor
-00002900: 792e 636f 6d2f 234e 566c 6162 732f 4661  y.com/#NVlabs/Fa
-00002910: 7374 6572 5669 5426 4461 7465 290a 0a0a  sterViT&Date)...
-00002920: 2323 2054 6869 7264 2d70 6172 7479 2045  ## Third-party E
-00002930: 7874 656e 7469 6f6e 730a 5765 2061 6c77  xtentions.We alw
-00002940: 6179 7320 7765 6c63 6f6d 6520 7468 6972  ays welcome thir
-00002950: 642d 7061 7274 7920 6578 7465 6e74 696f  d-party extentio
-00002960: 6e73 2f69 6d70 6c65 6d65 6e74 6174 696f  ns/implementatio
-00002970: 6e73 2061 6e64 2075 7361 6765 2066 6f72  ns and usage for
-00002980: 206f 7468 6572 2070 7572 706f 7365 732e   other purposes.
-00002990: 2049 6620 796f 7520 776f 756c 6420 6c69   If you would li
-000029a0: 6b65 2079 6f75 7220 776f 726b 2074 6f20  ke your work to 
-000029b0: 6265 206c 6973 7465 6420 696e 2074 6869  be listed in thi
-000029c0: 7320 7265 706f 7369 746f 7279 2c20 706c  s repository, pl
-000029d0: 6561 7365 2072 6169 7365 2061 6e64 2069  ease raise and i
-000029e0: 7373 7565 2061 6e64 2070 726f 7669 6465  ssue and provide
-000029f0: 2075 7320 7769 7468 2064 6574 6169 6c65   us with detaile
-00002a00: 6420 696e 666f 726d 6174 696f 6e2e 2020  d information.  
-00002a10: 0a0a 2323 2043 6974 6174 696f 6e0a 0a50  ..## Citation..P
-00002a20: 6c65 6173 6520 636f 6e73 6964 6572 2063  lease consider c
-00002a30: 6974 696e 6720 4661 7374 6572 5669 5420  iting FasterViT 
-00002a40: 6966 2074 6869 7320 7265 706f 7369 746f  if this reposito
-00002a50: 7279 2069 7320 7573 6566 756c 2066 6f72  ry is useful for
-00002a60: 2079 6f75 7220 776f 726b 2e20 0a0a 6060   your work. ..``
-00002a70: 600a 4061 7274 6963 6c65 7b68 6174 616d  `.@article{hatam
-00002a80: 697a 6164 6568 3230 3233 6661 7374 6572  izadeh2023faster
-00002a90: 7669 742c 0a20 2074 6974 6c65 3d7b 4661  vit,.  title={Fa
-00002aa0: 7374 6572 5669 543a 2046 6173 7420 5669  sterViT: Fast Vi
-00002ab0: 7369 6f6e 2054 7261 6e73 666f 726d 6572  sion Transformer
-00002ac0: 7320 7769 7468 2048 6965 7261 7263 6869  s with Hierarchi
-00002ad0: 6361 6c20 4174 7465 6e74 696f 6e7d 2c0a  cal Attention},.
-00002ae0: 2020 6175 7468 6f72 3d7b 4861 7461 6d69    author={Hatami
-00002af0: 7a61 6465 682c 2041 6c69 2061 6e64 2048  zadeh, Ali and H
-00002b00: 6569 6e72 6963 682c 2047 7265 6720 616e  einrich, Greg an
-00002b10: 6420 5969 6e2c 2048 6f6e 6778 7520 616e  d Yin, Hongxu an
-00002b20: 6420 5461 6f2c 2041 6e64 7265 7720 616e  d Tao, Andrew an
-00002b30: 6420 416c 7661 7265 7a2c 204a 6f73 6520  d Alvarez, Jose 
-00002b40: 4d20 616e 6420 4b61 7574 7a2c 204a 616e  M and Kautz, Jan
-00002b50: 2061 6e64 204d 6f6c 6368 616e 6f76 2c20   and Molchanov, 
-00002b60: 5061 766c 6f7d 2c0a 2020 6a6f 7572 6e61  Pavlo},.  journa
-00002b70: 6c3d 7b61 7258 6976 2070 7265 7072 696e  l={arXiv preprin
-00002b80: 7420 6172 5869 763a 3233 3036 2e30 3631  t arXiv:2306.061
-00002b90: 3839 7d2c 0a20 2079 6561 723d 7b32 3032  89},.  year={202
-00002ba0: 337d 0a7d 0a60 6060 0a0a 0a23 2320 4c69  3}.}.```...## Li
-00002bb0: 6365 6e73 6573 0a0a 436f 7079 7269 6768  censes..Copyrigh
-00002bc0: 7420 c2a9 2032 3032 332c 204e 5649 4449  t .. 2023, NVIDI
-00002bd0: 4120 436f 7270 6f72 6174 696f 6e2e 2041  A Corporation. A
-00002be0: 6c6c 2072 6967 6874 7320 7265 7365 7276  ll rights reserv
-00002bf0: 6564 2e0a 0a54 6869 7320 776f 726b 2069  ed...This work i
-00002c00: 7320 6d61 6465 2061 7661 696c 6162 6c65  s made available
-00002c10: 2075 6e64 6572 2074 6865 204e 5649 4449   under the NVIDI
-00002c20: 4120 536f 7572 6365 2043 6f64 6520 4c69  A Source Code Li
-00002c30: 6365 6e73 652d 4e43 2e20 436c 6963 6b20  cense-NC. Click 
-00002c40: 5b68 6572 655d 284c 4943 454e 5345 2920  [here](LICENSE) 
-00002c50: 746f 2076 6965 7720 6120 636f 7079 206f  to view a copy o
-00002c60: 6620 7468 6973 206c 6963 656e 7365 2e0a  f this license..
-00002c70: 0a46 6f72 206c 6963 656e 7365 2069 6e66  .For license inf
-00002c80: 6f72 6d61 7469 6f6e 2072 6567 6172 6469  ormation regardi
-00002c90: 6e67 2074 6865 2074 696d 6d20 7265 706f  ng the timm repo
-00002ca0: 7369 746f 7279 2c20 706c 6561 7365 2072  sitory, please r
-00002cb0: 6566 6572 2074 6f20 6974 7320 5b72 6570  efer to its [rep
-00002cc0: 6f73 6974 6f72 795d 2868 7474 7073 3a2f  ository](https:/
-00002cd0: 2f67 6974 6875 622e 636f 6d2f 7277 6967  /github.com/rwig
-00002ce0: 6874 6d61 6e2f 7079 746f 7263 682d 696d  htman/pytorch-im
-00002cf0: 6167 652d 6d6f 6465 6c73 292e 0a0a 466f  age-models)...Fo
-00002d00: 7220 6c69 6365 6e73 6520 696e 666f 726d  r license inform
-00002d10: 6174 696f 6e20 7265 6761 7264 696e 6720  ation regarding 
-00002d20: 7468 6520 496d 6167 654e 6574 2064 6174  the ImageNet dat
-00002d30: 6173 6574 2c20 706c 6561 7365 2073 6565  aset, please see
-00002d40: 2074 6865 205b 496d 6167 654e 6574 206f   the [ImageNet o
-00002d50: 6666 6963 6961 6c20 7765 6273 6974 655d  fficial website]
-00002d60: 2868 7474 7073 3a2f 2f77 7777 2e69 6d61  (https://www.ima
-00002d70: 6765 2d6e 6574 2e6f 7267 2f29 2e20 0a0a  ge-net.org/). ..
-00002d80: 2323 2041 636b 6e6f 776c 6564 6765 6d65  ## Acknowledgeme
-00002d90: 6e74 0a54 6869 7320 7265 706f 7369 746f  nt.This reposito
-00002da0: 7279 2069 7320 6275 696c 7420 6f6e 2074  ry is built on t
-00002db0: 6f70 206f 6620 7468 6520 5b74 696d 6d5d  op of the [timm]
-00002dc0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00002dd0: 636f 6d2f 6875 6767 696e 6766 6163 652f  com/huggingface/
-00002de0: 7079 746f 7263 682d 696d 6167 652d 6d6f  pytorch-image-mo
-00002df0: 6465 6c73 2920 7265 706f 7369 746f 7279  dels) repository
-00002e00: 2e20 5765 2074 6861 6e6b 205b 526f 7373  . We thank [Ross
-00002e10: 2057 7269 6768 746d 616e 5d28 6874 7470   Wrightman](http
-00002e20: 733a 2f2f 7277 6967 6874 6d61 6e2e 636f  s://rwightman.co
-00002e30: 6d2f 2920 666f 7220 6372 6561 7469 6e67  m/) for creating
-00002e40: 2061 6e64 206d 6169 6e74 6169 6e69 6e67   and maintaining
-00002e50: 2074 6869 7320 6869 6768 2d71 7561 6c69   this high-quali
-00002e60: 7479 206c 6962 7261 7279 2e20 200a 0a    ty library.  ..
+000007c0: 6365 6e74 6572 223e 0a3c 2f70 3e0a 0a0a  center">.</p>...
+000007d0: 2323 2051 7569 636b 2053 7461 7274 0a0a  ## Quick Start..
+000007e0: 5765 2063 616e 2069 6d70 6f72 7420 7072  We can import pr
+000007f0: 652d 7472 6169 6e65 6420 4661 7374 6572  e-trained Faster
+00000800: 5669 5420 6d6f 6465 6c73 2077 6974 6820  ViT models with 
+00000810: 2a2a 3120 6c69 6e65 206f 6620 636f 6465  **1 line of code
+00000820: 2a2a 2e20 4669 7273 742c 2046 6173 7465  **. First, Faste
+00000830: 7256 6954 2063 616e 2062 6520 7369 6d70  rViT can be simp
+00000840: 6c79 2069 6e73 7461 6c6c 6564 2062 793a  ly installed by:
+00000850: 0a0a 6060 6062 6173 680a 7069 7020 696e  ..```bash.pip in
+00000860: 7374 616c 6c20 6661 7374 6572 7669 740a  stall fastervit.
+00000870: 6060 600a 0a41 2070 7265 7472 6169 6e65  ```..A pretraine
+00000880: 6420 4661 7374 6572 5669 5420 6d6f 6465  d FasterViT mode
+00000890: 6c20 7769 7468 2064 6566 6175 6c74 2068  l with default h
+000008a0: 7970 6572 2d70 6172 616d 6574 6572 7320  yper-parameters 
+000008b0: 6361 6e20 6265 2063 7265 6174 6564 2061  can be created a
+000008c0: 7320 696e 2074 6865 2066 6f6c 6c6f 7769  s in the followi
+000008d0: 6e67 3a0a 0a60 6060 7079 7468 6f6e 0a3e  ng:..```python.>
+000008e0: 3e3e 2066 726f 6d20 6661 7374 6572 7669  >> from fastervi
+000008f0: 7420 696d 706f 7274 2063 7265 6174 655f  t import create_
+00000900: 6d6f 6465 6c0a 0a23 2044 6566 696e 6520  model..# Define 
+00000910: 6661 7374 6572 7669 742d 3020 6d6f 6465  fastervit-0 mode
+00000920: 6c20 7769 7468 2032 3234 2078 2032 3234  l with 224 x 224
+00000930: 2072 6573 6f6c 7574 696f 6e0a 0a3e 3e3e   resolution..>>>
+00000940: 206d 6f64 656c 203d 2063 7265 6174 655f   model = create_
+00000950: 6d6f 6465 6c28 2766 6173 7465 725f 7669  model('faster_vi
+00000960: 745f 305f 3232 3427 2c20 0a20 2020 2020  t_0_224', .     
+00000970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000980: 2020 2020 2070 7265 7472 6169 6e65 643d       pretrained=
+00000990: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+000009a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009b0: 6d6f 6465 6c5f 7061 7468 3d22 2f74 6d70  model_path="/tmp
+000009c0: 2f66 6173 7465 725f 7669 745f 302e 7074  /faster_vit_0.pt
+000009d0: 682e 7461 7222 290a 6060 600a 0a60 6d6f  h.tar").```..`mo
+000009e0: 6465 6c5f 7061 7468 6020 6973 2075 7365  del_path` is use
+000009f0: 6420 746f 2073 6574 2074 6865 2064 6972  d to set the dir
+00000a00: 6563 746f 7279 2074 6f20 646f 776e 6c6f  ectory to downlo
+00000a10: 6164 2074 6865 206d 6f64 656c 2e0a 0a57  ad the model...W
+00000a20: 6520 6361 6e20 616c 736f 2073 696d 706c  e can also simpl
+00000a30: 7920 7465 7374 2074 6865 206d 6f64 656c  y test the model
+00000a40: 2062 7920 7061 7373 696e 6720 6120 6475   by passing a du
+00000a50: 6d6d 7920 696e 7075 7420 696d 6167 652e  mmy input image.
+00000a60: 2054 6865 206f 7574 7075 7420 6973 2074   The output is t
+00000a70: 6865 206c 6f67 6974 733a 0a0a 6060 6070  he logits:..```p
+00000a80: 7974 686f 6e0a 3e3e 3e20 696d 706f 7274  ython.>>> import
+00000a90: 2074 6f72 6368 0a0a 3e3e 3e20 696d 6167   torch..>>> imag
+00000aa0: 6520 3d20 746f 7263 682e 7261 6e64 2831  e = torch.rand(1
+00000ab0: 2c20 332c 2032 3234 2c20 3232 3429 0a3e  , 3, 224, 224).>
+00000ac0: 3e3e 206f 7574 7075 7420 3d20 6d6f 6465  >> output = mode
+00000ad0: 6c28 696d 6167 6529 2023 2074 6f72 6368  l(image) # torch
+00000ae0: 2e53 697a 6528 5b31 2c20 3130 3030 5d29  .Size([1, 1000])
+00000af0: 0a60 6060 0a0a 5765 2063 616e 2061 6c73  .```..We can als
+00000b00: 6f20 7573 6520 7468 6520 616e 792d 7265  o use the any-re
+00000b10: 736f 6c75 7469 6f6e 2046 6173 7465 7256  solution FasterV
+00000b20: 6954 206d 6f64 656c 2074 6f20 6163 636f  iT model to acco
+00000b30: 6d6d 6f64 6174 6520 6172 6269 7472 6172  mmodate arbitrar
+00000b40: 7920 696d 6167 6520 7265 736f 6c75 7469  y image resoluti
+00000b50: 6f6e 732e 2049 6e20 7468 6520 666f 6c6c  ons. In the foll
+00000b60: 6f77 696e 672c 2077 6520 6465 6669 6e65  owing, we define
+00000b70: 2061 6e20 616e 792d 7265 736f 6c75 7469   an any-resoluti
+00000b80: 6f6e 2046 6173 7465 7256 6954 2d30 0a6d  on FasterViT-0.m
+00000b90: 6f64 656c 2077 6974 6820 696e 7075 7420  odel with input 
+00000ba0: 7265 736f 6c75 7469 6f6e 206f 6620 3537  resolution of 57
+00000bb0: 3620 7820 3936 302c 2077 696e 646f 7720  6 x 960, window 
+00000bc0: 7369 7a65 7320 6f66 2031 3220 616e 6420  sizes of 12 and 
+00000bd0: 3620 696e 2033 7264 2061 6e64 2034 7468  6 in 3rd and 4th
+00000be0: 2073 7461 6765 732c 2063 6172 7269 6572   stages, carrier
+00000bf0: 2074 6f6b 656e 2073 697a 6520 6f66 2032   token size of 2
+00000c00: 2061 6e64 2065 6d62 6564 6469 6e67 2064   and embedding d
+00000c10: 696d 656e 7369 6f6e 206f 660a 3634 3a0a  imension of.64:.
+00000c20: 0a60 6060 7079 7468 6f6e 0a3e 3e3e 2066  .```python.>>> f
+00000c30: 726f 6d20 6661 7374 6572 7669 7420 696d  rom fastervit im
+00000c40: 706f 7274 2063 7265 6174 655f 6d6f 6465  port create_mode
+00000c50: 6c0a 0a23 2044 6566 696e 6520 616e 792d  l..# Define any-
+00000c60: 7265 736f 6c75 7469 6f6e 2046 6173 7465  resolution Faste
+00000c70: 7256 6954 2d30 206d 6f64 656c 2077 6974  rViT-0 model wit
+00000c80: 6820 3537 3620 7820 3936 3020 7265 736f  h 576 x 960 reso
+00000c90: 6c75 7469 6f6e 0a3e 3e3e 206d 6f64 656c  lution.>>> model
+00000ca0: 203d 2063 7265 6174 655f 6d6f 6465 6c28   = create_model(
+00000cb0: 2766 6173 7465 725f 7669 745f 305f 616e  'faster_vit_0_an
+00000cc0: 795f 7265 7327 2c20 0a20 2020 2020 2020  y_res', .       
+00000cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ce0: 2020 2072 6573 6f6c 7574 696f 6e3d 5b35     resolution=[5
+00000cf0: 3736 2c20 3936 305d 2c0a 2020 2020 2020  76, 960],.      
+00000d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d10: 2020 2020 7769 6e64 6f77 5f73 697a 653d      window_size=
+00000d20: 5b37 2c20 372c 2031 322c 2036 5d2c 0a20  [7, 7, 12, 6],. 
+00000d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d40: 2020 2020 2020 2020 2063 745f 7369 7a65           ct_size
+00000d50: 3d32 2c0a 2020 2020 2020 2020 2020 2020  =2,.            
+00000d60: 2020 2020 2020 2020 2020 2020 2020 6469                di
+00000d70: 6d3d 3634 2c0a 2020 2020 2020 2020 2020  m=64,.          
+00000d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d90: 7072 6574 7261 696e 6564 3d54 7275 6529  pretrained=True)
+00000da0: 0a60 6060 0a4e 6f74 6520 7468 6174 2074  .```.Note that t
+00000db0: 6865 2061 626f 7665 206d 6f64 656c 2069  he above model i
+00000dc0: 7320 696e 7469 6c69 617a 6564 2066 726f  s intiliazed fro
+00000dd0: 6d20 7468 6520 6f72 6967 696e 616c 2049  m the original I
+00000de0: 6d61 6765 4e65 7420 7072 652d 7472 6169  mageNet pre-trai
+00000df0: 6e65 6420 4661 7374 6572 5669 5420 7769  ned FasterViT wi
+00000e00: 7468 206f 7269 6769 6e61 6c20 7265 736f  th original reso
+00000e10: 6c75 7469 6f6e 206f 6620 3232 3420 7820  lution of 224 x 
+00000e20: 3232 342e 2041 7320 6120 7265 7375 6c74  224. As a result
+00000e30: 2c20 6d69 7373 696e 6720 6b65 7973 2061  , missing keys a
+00000e40: 6e64 206d 6973 2d6d 6174 6368 6573 2063  nd mis-matches c
+00000e50: 6f75 6c64 2062 6520 6578 7065 6374 6564  ould be expected
+00000e60: 2073 696e 6365 2077 6520 6172 6520 6164   since we are ad
+00000e70: 6469 676e 206e 6577 206c 6179 6572 7320  dign new layers 
+00000e80: 2865 2e67 2e20 6164 6469 7469 6f6e 206f  (e.g. addition o
+00000e90: 6620 6e65 7720 6361 7272 6965 7220 746f  f new carrier to
+00000ea0: 6b65 6e73 2c20 6574 632e 2920 0a0a 5765  kens, etc.) ..We
+00000eb0: 2063 616e 2073 696d 706c 7920 7465 7374   can simply test
+00000ec0: 2074 6865 206d 6f64 656c 2062 7920 7061   the model by pa
+00000ed0: 7373 696e 6720 6120 6475 6d6d 7920 696e  ssing a dummy in
+00000ee0: 7075 7420 696d 6167 652e 2054 6865 206f  put image. The o
+00000ef0: 7574 7075 7420 6973 2074 6865 206c 6f67  utput is the log
+00000f00: 6974 733a 0a0a 6060 6070 7974 686f 6e0a  its:..```python.
+00000f10: 3e3e 3e20 696d 706f 7274 2074 6f72 6368  >>> import torch
+00000f20: 0a0a 3e3e 3e20 696d 6167 6520 3d20 746f  ..>>> image = to
+00000f30: 7263 682e 7261 6e64 2831 2c20 332c 2035  rch.rand(1, 3, 5
+00000f40: 3736 2c20 3936 3029 0a3e 3e3e 206f 7574  76, 960).>>> out
+00000f50: 7075 7420 3d20 6d6f 6465 6c28 696d 6167  put = model(imag
+00000f60: 6529 2023 2074 6f72 6368 2e53 697a 6528  e) # torch.Size(
+00000f70: 5b31 2c20 3130 3030 5d29 0a60 6060 0a0a  [1, 1000]).```..
+00000f80: 2d2d 2d20 0a0a 2323 2052 6573 756c 7473  --- ..## Results
+00000f90: 202b 2050 7265 7472 6169 6e65 6420 4d6f   + Pretrained Mo
+00000fa0: 6465 6c73 0a0a 2323 2320 496d 6167 654e  dels..### ImageN
+00000fb0: 6574 2d31 4b0a 2a2a 4661 7374 6572 5669  et-1K.**FasterVi
+00000fc0: 5420 496d 6167 654e 6574 2d31 4b20 5072  T ImageNet-1K Pr
+00000fd0: 6574 7261 696e 6564 204d 6f64 656c 732a  etrained Models*
+00000fe0: 2a0a 0a3c 7461 626c 653e 0a20 203c 7472  *..<table>.  <tr
+00000ff0: 3e0a 2020 2020 3c74 683e 4e61 6d65 3c2f  >.    <th>Name</
+00001000: 7468 3e0a 2020 2020 3c74 683e 4163 6340  th>.    <th>Acc@
+00001010: 3128 2529 3c2f 7468 3e0a 2020 2020 3c74  1(%)</th>.    <t
+00001020: 683e 4163 6340 3528 2529 3c2f 7468 3e0a  h>Acc@5(%)</th>.
+00001030: 2020 2020 3c74 683e 5468 726f 7567 6870      <th>Throughp
+00001040: 7574 2849 6d67 2f53 6563 293c 2f74 683e  ut(Img/Sec)</th>
+00001050: 0a20 2020 203c 7468 3e52 6573 6f6c 7574  .    <th>Resolut
+00001060: 696f 6e3c 2f74 683e 0a20 2020 203c 7468  ion</th>.    <th
+00001070: 3e23 5061 7261 6d73 284d 293c 2f74 683e  >#Params(M)</th>
+00001080: 0a20 2020 203c 7468 3e46 4c4f 5073 2847  .    <th>FLOPs(G
+00001090: 293c 2f74 683e 0a20 2020 203c 7468 3e44  )</th>.    <th>D
+000010a0: 6f77 6e6c 6f61 643c 2f74 683e 0a20 203c  ownload</th>.  <
+000010b0: 2f74 723e 0a0a 3c74 723e 0a20 2020 203c  /tr>..<tr>.    <
+000010c0: 7464 3e46 6173 7465 7256 6954 2d30 3c2f  td>FasterViT-0</
+000010d0: 7464 3e0a 2020 2020 3c74 643e 3832 2e31  td>.    <td>82.1
+000010e0: 3c2f 7464 3e0a 2020 2020 3c74 643e 3935  </td>.    <td>95
+000010f0: 2e39 3c2f 7464 3e0a 2020 2020 3c74 643e  .9</td>.    <td>
+00001100: 3538 3032 3c2f 7464 3e0a 2020 2020 3c74  5802</td>.    <t
+00001110: 643e 3232 3478 3232 343c 2f74 643e 0a20  d>224x224</td>. 
+00001120: 2020 203c 7464 3e33 312e 343c 2f74 643e     <td>31.4</td>
+00001130: 0a20 2020 203c 7464 3e33 2e33 3c2f 7464  .    <td>3.3</td
+00001140: 3e0a 2020 2020 3c74 643e 3c61 2068 7265  >.    <td><a hre
+00001150: 663d 2268 7474 7073 3a2f 2f64 7269 7665  f="https://drive
+00001160: 2e67 6f6f 676c 652e 636f 6d2f 7563 3f65  .google.com/uc?e
+00001170: 7870 6f72 743d 646f 776e 6c6f 6164 2669  xport=download&i
+00001180: 643d 3174 7749 324c 464a 7333 3931 5972  d=1twI2LFJs391Yr
+00001190: 6a38 4d52 3455 6939 5066 7276 5771 6a45  j8MR4Ui9PfrvWqjE
+000011a0: 3169 4222 3e6d 6f64 656c 3c2f 613e 3c2f  1iB">model</a></
+000011b0: 7464 3e0a 3c2f 7472 3e0a 0a3c 7472 3e0a  td>.</tr>..<tr>.
+000011c0: 2020 2020 3c74 643e 4661 7374 6572 5669      <td>FasterVi
+000011d0: 542d 313c 2f74 643e 0a20 2020 203c 7464  T-1</td>.    <td
+000011e0: 3e38 332e 323c 2f74 643e 0a20 2020 203c  >83.2</td>.    <
+000011f0: 7464 3e39 362e 353c 2f74 643e 0a20 2020  td>96.5</td>.   
+00001200: 203c 7464 3e34 3138 383c 2f74 643e 0a20   <td>4188</td>. 
+00001210: 2020 203c 7464 3e32 3234 7832 3234 3c2f     <td>224x224</
+00001220: 7464 3e0a 2020 2020 3c74 643e 3533 2e34  td>.    <td>53.4
+00001230: 3c2f 7464 3e0a 2020 2020 3c74 643e 352e  </td>.    <td>5.
+00001240: 333c 2f74 643e 0a20 2020 203c 7464 3e3c  3</td>.    <td><
+00001250: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00001260: 6472 6976 652e 676f 6f67 6c65 2e63 6f6d  drive.google.com
+00001270: 2f75 633f 6578 706f 7274 3d64 6f77 6e6c  /uc?export=downl
+00001280: 6f61 6426 6964 3d31 7237 5731 306e 352d  oad&id=1r7W10n5-
+00001290: 6246 744d 3373 7a34 626d 614c 726f 774e  bFtM3sz4bmaLrowN
+000012a0: 3267 5950 6b4c 4754 223e 6d6f 6465 6c3c  2gYPkLGT">model<
+000012b0: 2f61 3e3c 2f74 643e 0a3c 2f74 723e 0a0a  /a></td>.</tr>..
+000012c0: 3c74 723e 0a20 2020 203c 7464 3e46 6173  <tr>.    <td>Fas
+000012d0: 7465 7256 6954 2d32 3c2f 7464 3e0a 2020  terViT-2</td>.  
+000012e0: 2020 3c74 643e 3834 2e32 3c2f 7464 3e0a    <td>84.2</td>.
+000012f0: 2020 2020 3c74 643e 3936 2e38 3c2f 7464      <td>96.8</td
+00001300: 3e0a 2020 2020 3c74 643e 3331 3631 3c2f  >.    <td>3161</
+00001310: 7464 3e0a 2020 2020 3c74 643e 3232 3478  td>.    <td>224x
+00001320: 3232 343c 2f74 643e 0a20 2020 203c 7464  224</td>.    <td
+00001330: 3e37 352e 393c 2f74 643e 0a20 2020 203c  >75.9</td>.    <
+00001340: 7464 3e38 2e37 3c2f 7464 3e0a 2020 2020  td>8.7</td>.    
+00001350: 3c74 643e 3c61 2068 7265 663d 2268 7474  <td><a href="htt
+00001360: 7073 3a2f 2f64 7269 7665 2e67 6f6f 676c  ps://drive.googl
+00001370: 652e 636f 6d2f 7563 3f65 7870 6f72 743d  e.com/uc?export=
+00001380: 646f 776e 6c6f 6164 2669 643d 316e 5f61  download&id=1n_a
+00001390: 3673 3070 6769 306a 565a 4f47 6d44 6569  6s0pgi0jVZOGmDei
+000013a0: 3276 5848 5535 4536 5248 3577 5522 3e6d  2vXHU5E6RH5wU">m
+000013b0: 6f64 656c 3c2f 613e 3c2f 7464 3e0a 3c2f  odel</a></td>.</
+000013c0: 7472 3e0a 0a3c 7472 3e0a 2020 2020 3c74  tr>..<tr>.    <t
+000013d0: 643e 4661 7374 6572 5669 542d 333c 2f74  d>FasterViT-3</t
+000013e0: 643e 0a20 2020 203c 7464 3e38 342e 393c  d>.    <td>84.9<
+000013f0: 2f74 643e 0a20 2020 203c 7464 3e39 372e  /td>.    <td>97.
+00001400: 323c 2f74 643e 0a20 2020 203c 7464 3e31  2</td>.    <td>1
+00001410: 3738 303c 2f74 643e 0a20 2020 203c 7464  780</td>.    <td
+00001420: 3e32 3234 7832 3234 3c2f 7464 3e0a 2020  >224x224</td>.  
+00001430: 2020 3c74 643e 3135 392e 353c 2f74 643e    <td>159.5</td>
+00001440: 0a20 2020 203c 7464 3e31 382e 323c 2f74  .    <td>18.2</t
+00001450: 643e 0a20 2020 203c 7464 3e3c 6120 6872  d>.    <td><a hr
+00001460: 6566 3d22 6874 7470 733a 2f2f 6472 6976  ef="https://driv
+00001470: 652e 676f 6f67 6c65 2e63 6f6d 2f75 633f  e.google.com/uc?
+00001480: 6578 706f 7274 3d64 6f77 6e6c 6f61 6426  export=download&
+00001490: 6964 3d31 7476 5745 6c5a 3931 5369 6132  id=1tvWElZ91Sia2
+000014a0: 5373 5859 5846 4d4e 5951 7766 6970 4378  SsXYXFMNYQwfipCx
+000014b0: 7449 3758 223e 6d6f 6465 6c3c 2f61 3e3c  tI7X">model</a><
+000014c0: 2f74 643e 0a3c 2f74 723e 0a0a 3c74 723e  /td>.</tr>..<tr>
+000014d0: 0a20 2020 203c 7464 3e46 6173 7465 7256  .    <td>FasterV
+000014e0: 6954 2d34 3c2f 7464 3e0a 2020 2020 3c74  iT-4</td>.    <t
+000014f0: 643e 3835 2e34 3c2f 7464 3e0a 2020 2020  d>85.4</td>.    
+00001500: 3c74 643e 3937 2e33 3c2f 7464 3e0a 2020  <td>97.3</td>.  
+00001510: 2020 3c74 643e 3834 393c 2f74 643e 0a20    <td>849</td>. 
+00001520: 2020 203c 7464 3e32 3234 7832 3234 3c2f     <td>224x224</
+00001530: 7464 3e0a 2020 2020 3c74 643e 3432 342e  td>.    <td>424.
+00001540: 363c 2f74 643e 0a20 2020 203c 7464 3e33  6</td>.    <td>3
+00001550: 362e 363c 2f74 643e 0a20 2020 203c 7464  6.6</td>.    <td
+00001560: 3e3c 6120 6872 6566 3d22 6874 7470 733a  ><a href="https:
+00001570: 2f2f 6472 6976 652e 676f 6f67 6c65 2e63  //drive.google.c
+00001580: 6f6d 2f75 633f 6578 706f 7274 3d64 6f77  om/uc?export=dow
+00001590: 6e6c 6f61 6426 6964 3d31 6759 6858 4133  nload&id=1gYhXA3
+000015a0: 3251 2d5f 3943 3544 5865 6c31 3761 7656  2Q-_9C5DXel17avV
+000015b0: 5f5a 4c6f 6148 7764 677a 223e 6d6f 6465  _ZLoaHwdgz">mode
+000015c0: 6c3c 2f61 3e3c 2f74 643e 0a3c 2f74 723e  l</a></td>.</tr>
+000015d0: 0a0a 3c74 723e 0a20 2020 203c 7464 3e46  ..<tr>.    <td>F
+000015e0: 6173 7465 7256 6954 2d35 3c2f 7464 3e0a  asterViT-5</td>.
+000015f0: 2020 2020 3c74 643e 3835 2e36 3c2f 7464      <td>85.6</td
+00001600: 3e0a 2020 2020 3c74 643e 3937 2e34 3c2f  >.    <td>97.4</
+00001610: 7464 3e0a 2020 2020 3c74 643e 3434 393c  td>.    <td>449<
+00001620: 2f74 643e 0a20 2020 203c 7464 3e32 3234  /td>.    <td>224
+00001630: 7832 3234 3c2f 7464 3e0a 2020 2020 3c74  x224</td>.    <t
+00001640: 643e 3937 352e 353c 2f74 643e 0a20 2020  d>975.5</td>.   
+00001650: 203c 7464 3e31 3133 2e30 3c2f 7464 3e0a   <td>113.0</td>.
+00001660: 2020 2020 3c74 643e 3c61 2068 7265 663d      <td><a href=
+00001670: 2268 7474 7073 3a2f 2f64 7269 7665 2e67  "https://drive.g
+00001680: 6f6f 676c 652e 636f 6d2f 7563 3f65 7870  oogle.com/uc?exp
+00001690: 6f72 743d 646f 776e 6c6f 6164 2669 643d  ort=download&id=
+000016a0: 316d 7170 6169 3758 6948 4c72 5f6e 3174  1mqpai7XiHLr_n1t
+000016b0: 6a78 6a7a 5438 7133 3639 7854 4371 5f7a  jxjzT8q369xTCq_z
+000016c0: 2d22 3e6d 6f64 656c 3c2f 613e 3c2f 7464  -">model</a></td
+000016d0: 3e0a 3c2f 7472 3e0a 0a3c 7472 3e0a 2020  >.</tr>..<tr>.  
+000016e0: 2020 3c74 643e 4661 7374 6572 5669 542d    <td>FasterViT-
+000016f0: 363c 2f74 643e 0a20 2020 203c 7464 3e38  6</td>.    <td>8
+00001700: 352e 383c 2f74 643e 0a20 2020 203c 7464  5.8</td>.    <td
+00001710: 3e39 372e 343c 2f74 643e 0a20 2020 203c  >97.4</td>.    <
+00001720: 7464 3e33 3532 3c2f 7464 3e0a 2020 2020  td>352</td>.    
+00001730: 3c74 643e 3232 3478 3232 343c 2f74 643e  <td>224x224</td>
+00001740: 0a20 2020 203c 7464 3e31 3336 302e 303c  .    <td>1360.0<
+00001750: 2f74 643e 0a20 2020 203c 7464 3e31 3432  /td>.    <td>142
+00001760: 2e30 3c2f 7464 3e0a 2020 2020 3c74 643e  .0</td>.    <td>
+00001770: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00001780: 2f64 7269 7665 2e67 6f6f 676c 652e 636f  /drive.google.co
+00001790: 6d2f 7563 3f65 7870 6f72 743d 646f 776e  m/uc?export=down
+000017a0: 6c6f 6164 2669 643d 3132 6a74 6176 5232  load&id=12jtavR2
+000017b0: 5178 6d4d 7a63 4b77 507a 5765 376b 772d  QxmMzcKwPzWe7kw-
+000017c0: 6f79 3334 4959 6935 3922 3e6d 6f64 656c  oy34IYi59">model
+000017d0: 3c2f 613e 3c2f 7464 3e0a 3c2f 7472 3e0a  </a></td>.</tr>.
+000017e0: 0a3c 2f74 6162 6c65 3e0a 0a0a 2323 2320  .</table>...### 
+000017f0: 526f 6275 7374 6e65 7373 2028 496d 6167  Robustness (Imag
+00001800: 654e 6574 2d41 202d 2049 6d61 6765 4e65  eNet-A - ImageNe
+00001810: 742d 5220 2d20 496d 6167 654e 6574 2d56  t-R - ImageNet-V
+00001820: 3229 0a0a 416c 6c20 6d6f 6465 6c73 2075  2)..All models u
+00001830: 7365 2060 6372 6f70 5f70 6374 3d30 2e38  se `crop_pct=0.8
+00001840: 3735 602e 2052 6573 756c 7473 2061 7265  75`. Results are
+00001850: 206f 6274 6169 6e65 6420 6279 2072 756e   obtained by run
+00001860: 6e69 6e67 2069 6e66 6572 656e 6365 206f  ning inference o
+00001870: 6e20 496d 6167 654e 6574 2d31 4b20 7072  n ImageNet-1K pr
+00001880: 6574 7261 696e 6564 206d 6f64 656c 7320  etrained models 
+00001890: 7769 7468 6f75 7420 6669 6e65 7475 6e69  without finetuni
+000018a0: 6e67 2e0a 3c74 6162 6c65 3e0a 2020 3c74  ng..<table>.  <t
+000018b0: 723e 0a20 2020 203c 7468 3e4e 616d 653c  r>.    <th>Name<
+000018c0: 2f74 683e 0a20 2020 203c 7468 3e41 2d41  /th>.    <th>A-A
+000018d0: 6363 4031 2825 293c 2f74 683e 0a20 2020  cc@1(%)</th>.   
+000018e0: 203c 7468 3e41 2d41 6363 4035 2825 293c   <th>A-Acc@5(%)<
+000018f0: 2f74 683e 0a20 2020 203c 7468 3e52 2d41  /th>.    <th>R-A
+00001900: 6363 4031 2825 293c 2f74 683e 0a20 2020  cc@1(%)</th>.   
+00001910: 203c 7468 3e52 2d41 6363 4035 2825 293c   <th>R-Acc@5(%)<
+00001920: 2f74 683e 0a20 2020 203c 7468 3e56 322d  /th>.    <th>V2-
+00001930: 4163 6340 3128 2529 3c2f 7468 3e0a 2020  Acc@1(%)</th>.  
+00001940: 2020 3c74 683e 5632 2d41 6363 4035 2825    <th>V2-Acc@5(%
+00001950: 293c 2f74 683e 0a20 203c 2f74 723e 0a0a  )</th>.  </tr>..
+00001960: 3c74 723e 0a20 2020 203c 7464 3e46 6173  <tr>.    <td>Fas
+00001970: 7465 7256 6954 2d30 3c2f 7464 3e0a 2020  terViT-0</td>.  
+00001980: 2020 3c74 643e 3233 2e39 3c2f 7464 3e0a    <td>23.9</td>.
+00001990: 2020 2020 3c74 643e 3537 2e36 3c2f 7464      <td>57.6</td
+000019a0: 3e0a 2020 2020 3c74 643e 3435 2e39 3c2f  >.    <td>45.9</
+000019b0: 7464 3e0a 2020 2020 3c74 643e 3630 2e34  td>.    <td>60.4
+000019c0: 3c2f 7464 3e0a 2020 2020 3c74 643e 3730  </td>.    <td>70
+000019d0: 2e39 3c2f 7464 3e0a 2020 2020 3c74 643e  .9</td>.    <td>
+000019e0: 3930 2e30 3c2f 7464 3e0a 3c2f 7472 3e0a  90.0</td>.</tr>.
+000019f0: 0a3c 7472 3e0a 2020 2020 3c74 643e 4661  .<tr>.    <td>Fa
+00001a00: 7374 6572 5669 542d 313c 2f74 643e 0a20  sterViT-1</td>. 
+00001a10: 2020 203c 7464 3e33 312e 323c 2f74 643e     <td>31.2</td>
+00001a20: 0a20 2020 203c 7464 3e36 332e 333c 2f74  .    <td>63.3</t
+00001a30: 643e 0a20 2020 203c 7464 3e34 372e 353c  d>.    <td>47.5<
+00001a40: 2f74 643e 0a20 2020 203c 7464 3e36 312e  /td>.    <td>61.
+00001a50: 393c 2f74 643e 0a20 2020 203c 7464 3e37  9</td>.    <td>7
+00001a60: 322e 363c 2f74 643e 0a20 2020 203c 7464  2.6</td>.    <td
+00001a70: 3e39 312e 303c 2f74 643e 0a3c 2f74 723e  >91.0</td>.</tr>
+00001a80: 0a0a 3c74 723e 0a20 2020 203c 7464 3e46  ..<tr>.    <td>F
+00001a90: 6173 7465 7256 6954 2d32 3c2f 7464 3e0a  asterViT-2</td>.
+00001aa0: 2020 2020 3c74 643e 3338 2e32 3c2f 7464      <td>38.2</td
+00001ab0: 3e0a 2020 2020 3c74 643e 3638 2e39 3c2f  >.    <td>68.9</
+00001ac0: 7464 3e0a 2020 2020 3c74 643e 3439 2e36  td>.    <td>49.6
+00001ad0: 3c2f 7464 3e0a 2020 2020 3c74 643e 3633  </td>.    <td>63
+00001ae0: 2e34 3c2f 7464 3e0a 2020 2020 3c74 643e  .4</td>.    <td>
+00001af0: 3733 2e37 3c2f 7464 3e0a 2020 2020 3c74  73.7</td>.    <t
+00001b00: 643e 3931 2e36 3c2f 7464 3e0a 3c2f 7472  d>91.6</td>.</tr
+00001b10: 3e0a 0a3c 7472 3e0a 2020 2020 3c74 643e  >..<tr>.    <td>
+00001b20: 4661 7374 6572 5669 542d 333c 2f74 643e  FasterViT-3</td>
+00001b30: 0a20 2020 203c 7464 3e34 342e 323c 2f74  .    <td>44.2</t
+00001b40: 643e 0a20 2020 203c 7464 3e37 332e 303c  d>.    <td>73.0<
+00001b50: 2f74 643e 0a20 2020 203c 7464 3e35 312e  /td>.    <td>51.
+00001b60: 393c 2f74 643e 0a20 2020 203c 7464 3e36  9</td>.    <td>6
+00001b70: 352e 363c 2f74 643e 0a20 2020 203c 7464  5.6</td>.    <td
+00001b80: 3e37 352e 303c 2f74 643e 0a20 2020 203c  >75.0</td>.    <
+00001b90: 7464 3e39 322e 323c 2f74 643e 0a3c 2f74  td>92.2</td>.</t
+00001ba0: 723e 0a0a 3c74 723e 0a20 2020 203c 7464  r>..<tr>.    <td
+00001bb0: 3e46 6173 7465 7256 6954 2d34 3c2f 7464  >FasterViT-4</td
+00001bc0: 3e0a 2020 2020 3c74 643e 3439 2e30 3c2f  >.    <td>49.0</
+00001bd0: 7464 3e0a 2020 2020 3c74 643e 3735 2e34  td>.    <td>75.4
+00001be0: 3c2f 7464 3e0a 2020 2020 3c74 643e 3536  </td>.    <td>56
+00001bf0: 2e30 3c2f 7464 3e0a 2020 2020 3c74 643e  .0</td>.    <td>
+00001c00: 3639 2e36 3c2f 7464 3e0a 2020 2020 3c74  69.6</td>.    <t
+00001c10: 643e 3735 2e37 3c2f 7464 3e0a 2020 2020  d>75.7</td>.    
+00001c20: 3c74 643e 3932 2e37 3c2f 7464 3e0a 3c2f  <td>92.7</td>.</
+00001c30: 7472 3e0a 0a3c 7472 3e0a 2020 2020 3c74  tr>..<tr>.    <t
+00001c40: 643e 4661 7374 6572 5669 542d 353c 2f74  d>FasterViT-5</t
+00001c50: 643e 0a20 2020 203c 7464 3e35 322e 373c  d>.    <td>52.7<
+00001c60: 2f74 643e 0a20 2020 203c 7464 3e37 372e  /td>.    <td>77.
+00001c70: 363c 2f74 643e 0a20 2020 203c 7464 3e35  6</td>.    <td>5
+00001c80: 362e 393c 2f74 643e 0a20 2020 203c 7464  6.9</td>.    <td
+00001c90: 3e37 302e 303c 2f74 643e 0a20 2020 203c  >70.0</td>.    <
+00001ca0: 7464 3e37 362e 303c 2f74 643e 0a20 2020  td>76.0</td>.   
+00001cb0: 203c 7464 3e39 332e 303c 2f74 643e 0a3c   <td>93.0</td>.<
+00001cc0: 2f74 723e 0a0a 3c74 723e 0a20 2020 203c  /tr>..<tr>.    <
+00001cd0: 7464 3e46 6173 7465 7256 6954 2d36 3c2f  td>FasterViT-6</
+00001ce0: 7464 3e0a 2020 2020 3c74 643e 3533 2e37  td>.    <td>53.7
+00001cf0: 3c2f 7464 3e0a 2020 2020 3c74 643e 3738  </td>.    <td>78
+00001d00: 2e34 3c2f 7464 3e0a 2020 2020 3c74 643e  .4</td>.    <td>
+00001d10: 3537 2e31 3c2f 7464 3e0a 2020 2020 3c74  57.1</td>.    <t
+00001d20: 643e 3730 2e31 3c2f 7464 3e0a 2020 2020  d>70.1</td>.    
+00001d30: 3c74 643e 3736 2e31 3c2f 7464 3e0a 2020  <td>76.1</td>.  
+00001d40: 2020 3c74 643e 3933 2e30 3c2f 7464 3e0a    <td>93.0</td>.
+00001d50: 3c2f 7472 3e0a 0a3c 2f74 6162 6c65 3e0a  </tr>..</table>.
+00001d60: 0a41 2c20 5220 616e 6420 5632 2064 656e  .A, R and V2 den
+00001d70: 6f74 6520 496d 6167 654e 6574 2d41 2c20  ote ImageNet-A, 
+00001d80: 496d 6167 654e 6574 2d52 2061 6e64 2049  ImageNet-R and I
+00001d90: 6d61 6765 4e65 742d 5632 2072 6573 7065  mageNet-V2 respe
+00001da0: 6374 6976 656c 792e 200a 2323 2054 7261  ctively. .## Tra
+00001db0: 696e 696e 670a 0a50 6c65 6173 6520 7365  ining..Please se
+00001dc0: 6520 5b54 5241 494e 494e 472e 6d64 5d28  e [TRAINING.md](
+00001dd0: 5452 4149 4e49 4e47 2e6d 6429 2066 6f72  TRAINING.md) for
+00001de0: 2064 6574 6169 6c65 6420 7472 6169 6e69   detailed traini
+00001df0: 6e67 2069 6e73 7472 7563 7469 6f6e 7320  ng instructions 
+00001e00: 6f66 2061 6c6c 206d 6f64 656c 732e 200a  of all models. .
+00001e10: 0a23 2320 4576 616c 7561 7469 6f6e 0a0a  .## Evaluation..
+00001e20: 5468 6520 4661 7374 6572 5669 5420 6d6f  The FasterViT mo
+00001e30: 6465 6c73 2063 616e 2062 6520 6576 616c  dels can be eval
+00001e40: 7561 7465 6420 6f6e 2049 6d61 6765 4e65  uated on ImageNe
+00001e50: 742d 314b 2076 616c 6964 6174 696f 6e20  t-1K validation 
+00001e60: 7365 7420 7573 696e 6720 7468 6520 666f  set using the fo
+00001e70: 6c6c 6f77 696e 673a 200a 0a60 6060 0a70  llowing: ..```.p
+00001e80: 7974 686f 6e20 7661 6c69 6461 7465 2e70  ython validate.p
+00001e90: 7920 5c0a 2d2d 6d6f 6465 6c20 3c6d 6f64  y \.--model <mod
+00001ea0: 656c 2d6e 616d 653e 0a2d 2d63 6865 636b  el-name>.--check
+00001eb0: 706f 696e 7420 3c63 6865 636b 706f 696e  point <checkpoin
+00001ec0: 742d 7061 7468 3e0a 2d2d 6461 7461 5f64  t-path>.--data_d
+00001ed0: 6972 203c 696d 6167 656e 6574 2d70 6174  ir <imagenet-pat
+00001ee0: 683e 0a2d 2d62 6174 6368 2d73 697a 6520  h>.--batch-size 
+00001ef0: 3c62 6174 6368 2d73 697a 652d 7065 722d  <batch-size-per-
+00001f00: 6770 750a 6060 6020 0a0a 4865 7265 2060  gpu.``` ..Here `
+00001f10: 2d2d 6d6f 6465 6c60 2069 7320 7468 6520  --model` is the 
+00001f20: 4661 7374 6572 5669 5420 7661 7269 616e  FasterViT varian
+00001f30: 7420 2865 2e67 2e20 6066 6173 7465 725f  t (e.g. `faster_
+00001f40: 7669 745f 305f 3232 345f 316b 6029 2c20  vit_0_224_1k`), 
+00001f50: 602d 2d63 6865 636b 706f 696e 7460 2069  `--checkpoint` i
+00001f60: 7320 7468 6520 7061 7468 2074 6f20 7072  s the path to pr
+00001f70: 6574 7261 696e 6564 206d 6f64 656c 2077  etrained model w
+00001f80: 6569 6768 7473 2c20 602d 2d64 6174 615f  eights, `--data_
+00001f90: 6469 7260 2069 7320 7468 6520 7061 7468  dir` is the path
+00001fa0: 2074 6f20 496d 6167 654e 6574 2d31 4b20   to ImageNet-1K 
+00001fb0: 7661 6c69 6461 7469 6f6e 2073 6574 2061  validation set a
+00001fc0: 6e64 2060 2d2d 6261 7463 682d 7369 7a65  nd `--batch-size
+00001fd0: 6020 6973 2074 6865 206e 756d 6265 7220  ` is the number 
+00001fe0: 6f66 2062 6174 6368 2073 697a 652e 2057  of batch size. W
+00001ff0: 6520 616c 736f 2070 726f 7669 6465 2061  e also provide a
+00002000: 2073 616d 706c 6520 7363 7269 7074 205b   sample script [
+00002010: 6865 7265 5d28 2e2f 6661 7374 6572 7669  here](./fastervi
+00002020: 742f 7661 6c69 6461 7465 2e73 6829 2e20  t/validate.sh). 
+00002030: 0a0a 2323 204f 4e4e 5820 436f 6e76 6572  ..## ONNX Conver
+00002040: 7369 6f6e 0a0a 5765 2070 726f 7669 6465  sion..We provide
+00002050: 204f 4e4e 5820 636f 6e76 6572 7369 6f6e   ONNX conversion
+00002060: 2073 6372 6970 7420 746f 2065 6e61 626c   script to enabl
+00002070: 6520 6479 6e61 6d69 6320 6261 7463 6820  e dynamic batch 
+00002080: 7369 7a65 2069 6e66 6572 656e 6365 2e20  size inference. 
+00002090: 466f 7220 696e 7374 616e 6365 2c20 746f  For instance, to
+000020a0: 2067 656e 6572 6174 6520 4f4e 4e58 206d   generate ONNX m
+000020b0: 6f64 656c 2066 6f72 2060 6661 7374 6572  odel for `faster
+000020c0: 5f76 6974 5f30 5f61 6e79 5f72 6573 6020  _vit_0_any_res` 
+000020d0: 7769 7468 2072 6573 6f6c 7574 696f 6e20  with resolution 
+000020e0: 3537 3620 7820 3936 3020 616e 6420 4f4e  576 x 960 and ON
+000020f0: 4e58 206f 7073 6574 206e 756d 6265 7220  NX opset number 
+00002100: 3137 2c20 7468 6520 666f 6c6c 6f77 696e  17, the followin
+00002110: 6720 6361 6e20 6265 2075 7365 642e 200a  g can be used. .
+00002120: 0a60 6060 6261 7368 200a 7079 7468 6f6e  .```bash .python
+00002130: 206f 6e6e 785f 636f 6e76 6572 7420 2d2d   onnx_convert --
+00002140: 6d6f 6465 6c2d 6e61 6d65 2066 6173 7465  model-name faste
+00002150: 725f 7669 745f 305f 616e 795f 7265 7320  r_vit_0_any_res 
+00002160: 2d2d 7265 736f 6c75 7469 6f6e 2d68 2035  --resolution-h 5
+00002170: 3736 202d 2d72 6573 6f6c 7574 696f 6e2d  76 --resolution-
+00002180: 7720 3936 3020 2d2d 6f6e 6e78 2d6f 7073  w 960 --onnx-ops
+00002190: 6574 2031 370a 0a60 6060 0a0a 0a23 2320  et 17..```...## 
+000021a0: 496e 7374 616c 6c61 7469 6f6e 0a0a 5468  Installation..Th
+000021b0: 6520 6465 7065 6e64 656e 6369 6573 2063  e dependencies c
+000021c0: 616e 2062 6520 696e 7374 616c 6c65 6420  an be installed 
+000021d0: 6279 2072 756e 6e69 6e67 3a0a 0a60 6060  by running:..```
+000021e0: 6261 7368 0a70 6970 2069 6e73 7461 6c6c  bash.pip install
+000021f0: 202d 7220 7265 7175 6972 656d 656e 7473   -r requirements
+00002200: 2e74 7874 0a60 6060 0a0a 2323 2053 7461  .txt.```..## Sta
+00002210: 7220 4869 7374 6f72 790a 0a5b 215b 5374  r History..[![St
+00002220: 6172 2048 6973 746f 7279 2043 6861 7274  ar History Chart
+00002230: 5d28 6874 7470 733a 2f2f 6170 692e 7374  ](https://api.st
+00002240: 6172 2d68 6973 746f 7279 2e63 6f6d 2f73  ar-history.com/s
+00002250: 7667 3f72 6570 6f73 3d4e 566c 6162 732f  vg?repos=NVlabs/
+00002260: 4661 7374 6572 5669 5426 7479 7065 3d44  FasterViT&type=D
+00002270: 6174 6529 5d28 6874 7470 733a 2f2f 7374  ate)](https://st
+00002280: 6172 2d68 6973 746f 7279 2e63 6f6d 2f23  ar-history.com/#
+00002290: 4e56 6c61 6273 2f46 6173 7465 7256 6954  NVlabs/FasterViT
+000022a0: 2644 6174 6529 0a0a 0a23 2320 5468 6972  &Date)...## Thir
+000022b0: 642d 7061 7274 7920 4578 7465 6e74 696f  d-party Extentio
+000022c0: 6e73 0a57 6520 616c 7761 7973 2077 656c  ns.We always wel
+000022d0: 636f 6d65 2074 6869 7264 2d70 6172 7479  come third-party
+000022e0: 2065 7874 656e 7469 6f6e 732f 696d 706c   extentions/impl
+000022f0: 656d 656e 7461 7469 6f6e 7320 616e 6420  ementations and 
+00002300: 7573 6167 6520 666f 7220 6f74 6865 7220  usage for other 
+00002310: 7075 7270 6f73 6573 2e20 4966 2079 6f75  purposes. If you
+00002320: 2077 6f75 6c64 206c 696b 6520 796f 7572   would like your
+00002330: 2077 6f72 6b20 746f 2062 6520 6c69 7374   work to be list
+00002340: 6564 2069 6e20 7468 6973 2072 6570 6f73  ed in this repos
+00002350: 6974 6f72 792c 2070 6c65 6173 6520 7261  itory, please ra
+00002360: 6973 6520 616e 6420 6973 7375 6520 616e  ise and issue an
+00002370: 6420 7072 6f76 6964 6520 7573 2077 6974  d provide us wit
+00002380: 6820 6465 7461 696c 6564 2069 6e66 6f72  h detailed infor
+00002390: 6d61 7469 6f6e 2e20 200a 0a23 2320 4369  mation.  ..## Ci
+000023a0: 7461 7469 6f6e 0a0a 506c 6561 7365 2063  tation..Please c
+000023b0: 6f6e 7369 6465 7220 6369 7469 6e67 2046  onsider citing F
+000023c0: 6173 7465 7256 6954 2069 6620 7468 6973  asterViT if this
+000023d0: 2072 6570 6f73 6974 6f72 7920 6973 2075   repository is u
+000023e0: 7365 6675 6c20 666f 7220 796f 7572 2077  seful for your w
+000023f0: 6f72 6b2e 200a 0a60 6060 0a40 6172 7469  ork. ..```.@arti
+00002400: 636c 657b 6861 7461 6d69 7a61 6465 6832  cle{hatamizadeh2
+00002410: 3032 3366 6173 7465 7276 6974 2c0a 2020  023fastervit,.  
+00002420: 7469 746c 653d 7b46 6173 7465 7256 6954  title={FasterViT
+00002430: 3a20 4661 7374 2056 6973 696f 6e20 5472  : Fast Vision Tr
+00002440: 616e 7366 6f72 6d65 7273 2077 6974 6820  ansformers with 
+00002450: 4869 6572 6172 6368 6963 616c 2041 7474  Hierarchical Att
+00002460: 656e 7469 6f6e 7d2c 0a20 2061 7574 686f  ention},.  autho
+00002470: 723d 7b48 6174 616d 697a 6164 6568 2c20  r={Hatamizadeh, 
+00002480: 416c 6920 616e 6420 4865 696e 7269 6368  Ali and Heinrich
+00002490: 2c20 4772 6567 2061 6e64 2059 696e 2c20  , Greg and Yin, 
+000024a0: 486f 6e67 7875 2061 6e64 2054 616f 2c20  Hongxu and Tao, 
+000024b0: 416e 6472 6577 2061 6e64 2041 6c76 6172  Andrew and Alvar
+000024c0: 657a 2c20 4a6f 7365 204d 2061 6e64 204b  ez, Jose M and K
+000024d0: 6175 747a 2c20 4a61 6e20 616e 6420 4d6f  autz, Jan and Mo
+000024e0: 6c63 6861 6e6f 762c 2050 6176 6c6f 7d2c  lchanov, Pavlo},
+000024f0: 0a20 206a 6f75 726e 616c 3d7b 6172 5869  .  journal={arXi
+00002500: 7620 7072 6570 7269 6e74 2061 7258 6976  v preprint arXiv
+00002510: 3a32 3330 362e 3036 3138 397d 2c0a 2020  :2306.06189},.  
+00002520: 7965 6172 3d7b 3230 3233 7d0a 7d0a 6060  year={2023}.}.``
+00002530: 600a 0a0a 2323 204c 6963 656e 7365 730a  `...## Licenses.
+00002540: 0a43 6f70 7972 6967 6874 20c2 a920 3230  .Copyright .. 20
+00002550: 3233 2c20 4e56 4944 4941 2043 6f72 706f  23, NVIDIA Corpo
+00002560: 7261 7469 6f6e 2e20 416c 6c20 7269 6768  ration. All righ
+00002570: 7473 2072 6573 6572 7665 642e 0a0a 5468  ts reserved...Th
+00002580: 6973 2077 6f72 6b20 6973 206d 6164 6520  is work is made 
+00002590: 6176 6169 6c61 626c 6520 756e 6465 7220  available under 
+000025a0: 7468 6520 4e56 4944 4941 2053 6f75 7263  the NVIDIA Sourc
+000025b0: 6520 436f 6465 204c 6963 656e 7365 2d4e  e Code License-N
+000025c0: 432e 2043 6c69 636b 205b 6865 7265 5d28  C. Click [here](
+000025d0: 4c49 4345 4e53 4529 2074 6f20 7669 6577  LICENSE) to view
+000025e0: 2061 2063 6f70 7920 6f66 2074 6869 7320   a copy of this 
+000025f0: 6c69 6365 6e73 652e 0a0a 466f 7220 6c69  license...For li
+00002600: 6365 6e73 6520 696e 666f 726d 6174 696f  cense informatio
+00002610: 6e20 7265 6761 7264 696e 6720 7468 6520  n regarding the 
+00002620: 7469 6d6d 2072 6570 6f73 6974 6f72 792c  timm repository,
+00002630: 2070 6c65 6173 6520 7265 6665 7220 746f   please refer to
+00002640: 2069 7473 205b 7265 706f 7369 746f 7279   its [repository
+00002650: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00002660: 2e63 6f6d 2f72 7769 6768 746d 616e 2f70  .com/rwightman/p
+00002670: 7974 6f72 6368 2d69 6d61 6765 2d6d 6f64  ytorch-image-mod
+00002680: 656c 7329 2e0a 0a46 6f72 206c 6963 656e  els)...For licen
+00002690: 7365 2069 6e66 6f72 6d61 7469 6f6e 2072  se information r
+000026a0: 6567 6172 6469 6e67 2074 6865 2049 6d61  egarding the Ima
+000026b0: 6765 4e65 7420 6461 7461 7365 742c 2070  geNet dataset, p
+000026c0: 6c65 6173 6520 7365 6520 7468 6520 5b49  lease see the [I
+000026d0: 6d61 6765 4e65 7420 6f66 6669 6369 616c  mageNet official
+000026e0: 2077 6562 7369 7465 5d28 6874 7470 733a   website](https:
+000026f0: 2f2f 7777 772e 696d 6167 652d 6e65 742e  //www.image-net.
+00002700: 6f72 672f 292e 200a 0a23 2320 4163 6b6e  org/). ..## Ackn
+00002710: 6f77 6c65 6467 656d 656e 740a 5468 6973  owledgement.This
+00002720: 2072 6570 6f73 6974 6f72 7920 6973 2062   repository is b
+00002730: 7569 6c74 206f 6e20 746f 7020 6f66 2074  uilt on top of t
+00002740: 6865 205b 7469 6d6d 5d28 6874 7470 733a  he [timm](https:
+00002750: 2f2f 6769 7468 7562 2e63 6f6d 2f68 7567  //github.com/hug
+00002760: 6769 6e67 6661 6365 2f70 7974 6f72 6368  gingface/pytorch
+00002770: 2d69 6d61 6765 2d6d 6f64 656c 7329 2072  -image-models) r
+00002780: 6570 6f73 6974 6f72 792e 2057 6520 7468  epository. We th
+00002790: 616e 6b20 5b52 6f73 7320 5772 6967 6874  ank [Ross Wright
+000027a0: 6d61 6e5d 2868 7474 7073 3a2f 2f72 7769  man](https://rwi
+000027b0: 6768 746d 616e 2e63 6f6d 2f29 2066 6f72  ghtman.com/) for
+000027c0: 2063 7265 6174 696e 6720 616e 6420 6d61   creating and ma
+000027d0: 696e 7461 696e 696e 6720 7468 6973 2068  intaining this h
+000027e0: 6967 682d 7175 616c 6974 7920 6c69 6272  igh-quality libr
+000027f0: 6172 792e 2020 0a0a                      ary.  ..
```

### Comparing `fastervit-0.9.1/README.md` & `fastervit-0.9.2/fastervit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,684 +1,640 @@
-00000000: 2320 4661 7374 6572 5669 543a 2046 6173  # FasterViT: Fas
-00000010: 7420 5669 7369 6f6e 2054 7261 6e73 666f  t Vision Transfo
-00000020: 726d 6572 7320 7769 7468 2048 6965 7261  rmers with Hiera
-00000030: 7263 6869 6361 6c20 4174 7465 6e74 696f  rchical Attentio
-00000040: 6e0a 0a4f 6666 6963 6961 6c20 5079 546f  n..Official PyTo
-00000050: 7263 6820 696d 706c 656d 656e 7461 7469  rch implementati
-00000060: 6f6e 206f 6620 5b2a 2a46 6173 7465 7256  on of [**FasterV
-00000070: 6954 3a20 4661 7374 2056 6973 696f 6e20  iT: Fast Vision 
-00000080: 5472 616e 7366 6f72 6d65 7273 2077 6974  Transformers wit
-00000090: 6820 4869 6572 6172 6368 6963 616c 2041  h Hierarchical A
-000000a0: 7474 656e 7469 6f6e 2a2a 5d28 6874 7470  ttention**](http
-000000b0: 733a 2f2f 6172 7869 762e 6f72 672f 6162  s://arxiv.org/ab
-000000c0: 732f 3233 3036 2e30 3631 3839 292e 0a0a  s/2306.06189)...
-000000d0: 5b41 6c69 2048 6174 616d 697a 6164 6568  [Ali Hatamizadeh
-000000e0: 5d28 6874 7470 733a 2f2f 7265 7365 6172  ](https://resear
-000000f0: 6368 2e6e 7669 6469 612e 636f 6d2f 7065  ch.nvidia.com/pe
-00000100: 7273 6f6e 2f61 6c69 2d68 6174 616d 697a  rson/ali-hatamiz
-00000110: 6164 6568 292c 0a5b 4772 6567 2048 6569  adeh),.[Greg Hei
-00000120: 6e72 6963 685d 2868 7474 7073 3a2f 2f64  nrich](https://d
-00000130: 6576 656c 6f70 6572 2e6e 7669 6469 612e  eveloper.nvidia.
-00000140: 636f 6d2f 626c 6f67 2f61 7574 686f 722f  com/blog/author/
-00000150: 6768 6569 6e72 6963 682f 292c 0a5b 486f  gheinrich/),.[Ho
-00000160: 6e67 7875 2028 4461 6e6e 7929 2059 696e  ngxu (Danny) Yin
-00000170: 5d28 6874 7470 733a 2f2f 7363 686f 6c61  ](https://schola
-00000180: 722e 7072 696e 6365 746f 6e2e 6564 752f  r.princeton.edu/
-00000190: 686f 6e67 7875 292c 0a5b 416e 6472 6577  hongxu),.[Andrew
-000001a0: 2054 616f 5d28 6874 7470 733a 2f2f 6465   Tao](https://de
-000001b0: 7665 6c6f 7065 722e 6e76 6964 6961 2e63  veloper.nvidia.c
-000001c0: 6f6d 2f62 6c6f 672f 6175 7468 6f72 2f61  om/blog/author/a
-000001d0: 7461 6f2f 292c 0a5b 4a6f 7365 204d 2e20  tao/),.[Jose M. 
-000001e0: 416c 7661 7265 7a5d 2868 7474 7073 3a2f  Alvarez](https:/
-000001f0: 2f61 6c76 6172 657a 6c6f 7065 7a6a 6f73  /alvarezlopezjos
-00000200: 656d 2e67 6974 6875 622e 696f 2f29 2c0a  em.github.io/),.
-00000210: 5b4a 616e 204b 6175 747a 5d28 6874 7470  [Jan Kautz](http
-00000220: 733a 2f2f 6a61 6e6b 6175 747a 2e63 6f6d  s://jankautz.com
-00000230: 2f29 2c20 0a5b 5061 766c 6f20 4d6f 6c63  /), .[Pavlo Molc
-00000240: 6861 6e6f 765d 2868 7474 7073 3a2f 2f77  hanov](https://w
-00000250: 7777 2e70 6d6f 6c63 6861 6e6f 762e 636f  ww.pmolchanov.co
-00000260: 6d2f 292e 0a0a 466f 7220 6275 7369 6e65  m/)...For busine
-00000270: 7373 2069 6e71 7569 7269 6573 2c20 706c  ss inquiries, pl
-00000280: 6561 7365 2076 6973 6974 206f 7572 2077  ease visit our w
-00000290: 6562 7369 7465 2061 6e64 2073 7562 6d69  ebsite and submi
-000002a0: 7420 7468 6520 666f 726d 3a20 5b4e 5649  t the form: [NVI
-000002b0: 4449 4120 5265 7365 6172 6368 204c 6963  DIA Research Lic
-000002c0: 656e 7369 6e67 5d28 6874 7470 733a 2f2f  ensing](https://
-000002d0: 7777 772e 6e76 6964 6961 2e63 6f6d 2f65  www.nvidia.com/e
-000002e0: 6e2d 7573 2f72 6573 6561 7263 682f 696e  n-us/research/in
-000002f0: 7175 6972 6965 732f 290a 0a0a 2d2d 2d20  quiries/)...--- 
-00000300: 0a0a 4661 7374 6572 5669 5420 6163 6869  ..FasterViT achi
-00000310: 6576 6573 2061 206e 6577 2053 4f54 4120  eves a new SOTA 
-00000320: 5061 7265 746f 2d66 726f 6e74 2069 6e0a  Pareto-front in.
-00000330: 7465 726d 7320 6f66 2061 6363 7572 6163  terms of accurac
-00000340: 7920 7673 2e20 696d 6167 6520 7468 726f  y vs. image thro
-00000350: 7567 6870 7574 2077 6974 686f 7574 2065  ughput without e
-00000360: 7874 7261 2074 7261 696e 696e 6720 6461  xtra training da
-00000370: 7461 2021 0a0a 3c70 2061 6c69 676e 3d22  ta !..<p align="
-00000380: 6365 6e74 6572 223e 0a3c 696d 6720 7372  center">.<img sr
-00000390: 633d 2268 7474 7073 3a2f 2f67 6974 6875  c="https://githu
-000003a0: 622e 636f 6d2f 4e56 6c61 6273 2f46 6173  b.com/NVlabs/Fas
-000003b0: 7465 7256 6954 2f61 7373 6574 732f 3236  terViT/assets/26
-000003c0: 3830 3633 3934 2f32 3533 6431 6132 652d  806394/253d1a2e-
-000003d0: 6235 6635 2d34 6139 622d 6133 3632 2d36  b5f5-4a9b-a362-6
-000003e0: 6364 6431 3662 6663 6363 3122 2077 6964  cdd16bfccc1" wid
-000003f0: 7468 3d36 3225 2068 6569 6768 743d 3632  th=62% height=62
-00000400: 2520 0a63 6c61 7373 3d22 6365 6e74 6572  % .class="center
-00000410: 223e 0a3c 2f70 3e0a 0a57 6520 696e 7472  ">.</p>..We intr
-00000420: 6f64 7563 6520 6120 6e65 7720 7365 6c66  oduce a new self
-00000430: 2d61 7474 656e 7469 6f6e 206d 6563 6861  -attention mecha
-00000440: 6e69 736d 2c20 6465 6e6f 7465 6420 6173  nism, denoted as
-00000450: 2048 6965 7261 7263 6869 6361 6c0a 4174   Hierarchical.At
-00000460: 7465 6e74 696f 6e20 2848 4154 292c 2074  tention (HAT), t
-00000470: 6861 7420 6361 7074 7572 6573 2062 6f74  hat captures bot
-00000480: 6820 7368 6f72 7420 616e 6420 6c6f 6e67  h short and long
-00000490: 2d72 616e 6765 2069 6e66 6f72 6d61 7469  -range informati
-000004a0: 6f6e 2062 7920 6c65 6172 6e69 6e67 0a63  on by learning.c
-000004b0: 726f 7373 2d77 696e 646f 7720 6361 7272  ross-window carr
-000004c0: 6965 7220 746f 6b65 6e73 2e0a 0a21 5b74  ier tokens...![t
-000004d0: 6561 7365 725d 282e 2f66 6173 7465 7276  easer](./fasterv
-000004e0: 6974 2f61 7373 6574 732f 6869 6572 6172  it/assets/hierar
-000004f0: 6368 6961 6c5f 6174 746e 2e70 6e67 290a  chial_attn.png).
-00000500: 0a23 2320 5175 6963 6b20 5374 6172 740a  .## Quick Start.
-00000510: 0a57 6520 6361 6e20 696d 706f 7274 2070  .We can import p
-00000520: 7265 2d74 7261 696e 6564 2046 6173 7465  re-trained Faste
-00000530: 7256 6954 206d 6f64 656c 7320 7769 7468  rViT models with
-00000540: 202a 2a31 206c 696e 6520 6f66 2063 6f64   **1 line of cod
-00000550: 652a 2a2e 2046 6972 7374 2c20 4661 7374  e**. First, Fast
-00000560: 6572 5669 5420 6361 6e20 6265 2073 696d  erViT can be sim
-00000570: 706c 7920 696e 7374 616c 6c65 6420 6279  ply installed by
-00000580: 3a0a 0a60 6060 6261 7368 0a70 6970 2069  :..```bash.pip i
-00000590: 6e73 7461 6c6c 2066 6173 7465 7276 6974  nstall fastervit
-000005a0: 0a60 6060 0a0a 4120 7072 6574 7261 696e  .```..A pretrain
-000005b0: 6564 2046 6173 7465 7256 6954 206d 6f64  ed FasterViT mod
-000005c0: 656c 2077 6974 6820 6465 6661 756c 7420  el with default 
-000005d0: 6879 7065 722d 7061 7261 6d65 7465 7273  hyper-parameters
-000005e0: 2063 616e 2062 6520 6372 6561 7465 6420   can be created 
-000005f0: 6173 2069 6e20 7468 6520 666f 6c6c 6f77  as in the follow
-00000600: 696e 673a 0a0a 6060 6070 7974 686f 6e0a  ing:..```python.
-00000610: 3e3e 3e20 6672 6f6d 2066 6173 7465 7276  >>> from fasterv
-00000620: 6974 2069 6d70 6f72 7420 6372 6561 7465  it import create
-00000630: 5f6d 6f64 656c 0a0a 2320 4465 6669 6e65  _model..# Define
-00000640: 2066 6173 7465 7276 6974 2d30 206d 6f64   fastervit-0 mod
-00000650: 656c 2077 6974 6820 3232 3420 7820 3232  el with 224 x 22
-00000660: 3420 7265 736f 6c75 7469 6f6e 0a0a 3e3e  4 resolution..>>
-00000670: 3e20 6d6f 6465 6c20 3d20 6372 6561 7465  > model = create
-00000680: 5f6d 6f64 656c 2827 6661 7374 6572 5f76  _model('faster_v
-00000690: 6974 5f30 5f32 3234 272c 200a 2020 2020  it_0_224', .    
-000006a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000006b0: 2020 2020 2020 7072 6574 7261 696e 6564        pretrained
-000006c0: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
-000006d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000006e0: 206d 6f64 656c 5f70 6174 683d 222f 746d   model_path="/tm
-000006f0: 702f 6661 7374 6572 5f76 6974 5f30 2e70  p/faster_vit_0.p
-00000700: 7468 2e74 6172 2229 0a60 6060 0a0a 5765  th.tar").```..We
-00000710: 2063 616e 2061 646a 7573 7420 7768 6572   can adjust wher
-00000720: 6520 746f 2064 6f77 6e6c 6f61 6420 7468  e to download th
-00000730: 6520 6162 6f76 6520 4661 7374 6572 5669  e above FasterVi
-00000740: 542d 3020 6d6f 6465 6c20 6279 2070 6173  T-0 model by pas
-00000750: 7369 6e67 2060 6d6f 6465 6c5f 7061 7468  sing `model_path
-00000760: 602e 0a0a 5765 2063 616e 2061 6c73 6f20  `...We can also 
-00000770: 7369 6d70 6c79 2074 6573 7420 7468 6520  simply test the 
-00000780: 6d6f 6465 6c20 6279 2070 6173 7369 6e67  model by passing
-00000790: 2061 2064 756d 6d79 2069 6e70 7574 2069   a dummy input i
-000007a0: 6d61 6765 2e20 5468 6520 6f75 7470 7574  mage. The output
-000007b0: 2069 7320 7468 6520 6c6f 6769 7473 3a0a   is the logits:.
-000007c0: 0a60 6060 7079 7468 6f6e 0a3e 3e3e 2069  .```python.>>> i
-000007d0: 6d70 6f72 7420 746f 7263 680a 0a3e 3e3e  mport torch..>>>
-000007e0: 2069 6d61 6765 203d 2074 6f72 6368 2e72   image = torch.r
-000007f0: 616e 6428 312c 2033 2c20 3232 342c 2032  and(1, 3, 224, 2
-00000800: 3234 290a 3e3e 3e20 6f75 7470 7574 203d  24).>>> output =
-00000810: 206d 6f64 656c 2869 6d61 6765 2920 2320   model(image) # 
-00000820: 746f 7263 682e 5369 7a65 285b 312c 2031  torch.Size([1, 1
-00000830: 3030 305d 290a 6060 600a 0a57 6520 6361  000]).```..We ca
-00000840: 6e20 616c 736f 2075 7365 2074 6865 2061  n also use the a
-00000850: 6e79 2d72 6573 6f6c 7574 696f 6e20 4661  ny-resolution Fa
-00000860: 7374 6572 5669 5420 6d6f 6465 6c20 746f  sterViT model to
-00000870: 2061 6363 6f6d 6d6f 6461 7465 2061 7262   accommodate arb
-00000880: 6974 7261 7279 2069 6d61 6765 2072 6573  itrary image res
-00000890: 6f6c 7574 696f 6e73 2e20 496e 2074 6865  olutions. In the
-000008a0: 2066 6f6c 6c6f 7769 6e67 2c20 7765 2064   following, we d
-000008b0: 6566 696e 6520 616e 2061 6e79 2d72 6573  efine an any-res
-000008c0: 6f6c 7574 696f 6e20 4661 7374 6572 5669  olution FasterVi
-000008d0: 542d 300a 6d6f 6465 6c20 7769 7468 2069  T-0.model with i
-000008e0: 6e70 7574 2072 6573 6f6c 7574 696f 6e20  nput resolution 
-000008f0: 6f66 2035 3736 2078 2039 3630 2c20 7769  of 576 x 960, wi
-00000900: 6e64 6f77 2073 697a 6573 206f 6620 3132  ndow sizes of 12
-00000910: 2061 6e64 2036 2069 6e20 3372 6420 616e   and 6 in 3rd an
-00000920: 6420 3474 6820 7374 6167 6573 2c20 6361  d 4th stages, ca
-00000930: 7272 6965 7220 746f 6b65 6e20 7369 7a65  rrier token size
-00000940: 206f 6620 3220 616e 6420 656d 6265 6464   of 2 and embedd
-00000950: 696e 6720 6469 6d65 6e73 696f 6e20 6f66  ing dimension of
-00000960: 0a31 3238 3a0a 0a60 6060 7079 7468 6f6e  .128:..```python
-00000970: 0a3e 3e3e 2066 726f 6d20 6661 7374 6572  .>>> from faster
-00000980: 7669 7420 696d 706f 7274 2063 7265 6174  vit import creat
-00000990: 655f 6d6f 6465 6c0a 0a23 2044 6566 696e  e_model..# Defin
-000009a0: 6520 616e 792d 7265 736f 6c75 7469 6f6e  e any-resolution
-000009b0: 2046 6173 7465 7256 6954 2d30 206d 6f64   FasterViT-0 mod
-000009c0: 656c 2077 6974 6820 3537 3620 7820 3936  el with 576 x 96
-000009d0: 3020 7265 736f 6c75 7469 6f6e 0a3e 3e3e  0 resolution.>>>
-000009e0: 206d 6f64 656c 203d 2063 7265 6174 655f   model = create_
-000009f0: 6d6f 6465 6c28 2766 6173 7465 725f 7669  model('faster_vi
-00000a00: 745f 305f 616e 795f 7265 7327 2c20 0a20  t_0_any_res', . 
-00000a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a20: 2020 2020 2020 2020 2072 6573 6f6c 7574           resolut
-00000a30: 696f 6e3d 5b35 3736 2c20 3936 305d 2c0a  ion=[576, 960],.
-00000a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a50: 2020 2020 2020 2020 2020 7769 6e64 6f77            window
-00000a60: 5f73 697a 653d 5b37 2c20 372c 2031 322c  _size=[7, 7, 12,
-00000a70: 2036 5d2c 0a20 2020 2020 2020 2020 2020   6],.           
-00000a80: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00000a90: 745f 7369 7a65 3d32 2c0a 2020 2020 2020  t_size=2,.      
-00000aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ab0: 2020 2020 6469 6d3d 3634 2c0a 2020 2020      dim=64,.    
-00000ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ad0: 2020 2020 2020 7072 6574 7261 696e 6564        pretrained
-00000ae0: 3d54 7275 6529 0a60 6060 0a4e 6f74 6520  =True).```.Note 
-00000af0: 7468 6174 2074 6865 2061 626f 7665 206d  that the above m
-00000b00: 6f64 656c 2069 7320 696e 7469 6c69 617a  odel is intiliaz
-00000b10: 6564 2066 726f 6d20 7468 6520 6f72 6967  ed from the orig
-00000b20: 696e 616c 2049 6d61 6765 4e65 7420 7072  inal ImageNet pr
-00000b30: 652d 7472 6169 6e65 6420 4661 7374 6572  e-trained Faster
-00000b40: 5669 5420 7769 7468 206f 7269 6769 6e61  ViT with origina
-00000b50: 6c20 7265 736f 6c75 7469 6f6e 206f 6620  l resolution of 
-00000b60: 3232 3420 7820 3232 342e 2041 7320 6120  224 x 224. As a 
-00000b70: 7265 7375 6c74 2c20 6d69 7373 696e 6720  result, missing 
-00000b80: 6b65 7973 2061 6e64 206d 6973 2d6d 6174  keys and mis-mat
-00000b90: 6368 6573 2063 6f75 6c64 2062 6520 6578  ches could be ex
-00000ba0: 7065 6374 6564 2073 696e 6365 2077 6520  pected since we 
-00000bb0: 6172 6520 6164 6469 676e 206e 6577 206c  are addign new l
-00000bc0: 6179 6572 7320 2865 2e67 2e20 6164 6469  ayers (e.g. addi
-00000bd0: 7469 6f6e 206f 6620 6e65 7720 6361 7272  tion of new carr
-00000be0: 6965 7220 746f 6b65 6e73 2c20 6574 632e  ier tokens, etc.
-00000bf0: 2920 0a0a 5765 2063 616e 2073 696d 706c  ) ..We can simpl
-00000c00: 7920 7465 7374 2074 6865 206d 6f64 656c  y test the model
-00000c10: 2062 7920 7061 7373 696e 6720 6120 6475   by passing a du
-00000c20: 6d6d 7920 696e 7075 7420 696d 6167 652e  mmy input image.
-00000c30: 2054 6865 206f 7574 7075 7420 6973 2074   The output is t
-00000c40: 6865 206c 6f67 6974 733a 0a0a 6060 6070  he logits:..```p
-00000c50: 7974 686f 6e0a 3e3e 3e20 696d 706f 7274  ython.>>> import
-00000c60: 2074 6f72 6368 0a0a 3e3e 3e20 696d 6167   torch..>>> imag
-00000c70: 6520 3d20 746f 7263 682e 7261 6e64 2831  e = torch.rand(1
-00000c80: 2c20 332c 2035 3736 2c20 3936 3029 0a3e  , 3, 576, 960).>
-00000c90: 3e3e 206f 7574 7075 7420 3d20 6d6f 6465  >> output = mode
-00000ca0: 6c28 696d 6167 6529 2023 2074 6f72 6368  l(image) # torch
-00000cb0: 2e53 697a 6528 5b31 2c20 3130 3030 5d29  .Size([1, 1000])
-00000cc0: 0a60 6060 0a0a 2323 20f0 9f92 a520 4e65  .```..## .... Ne
-00000cd0: 7773 20f0 9f92 a50a 0a2d 202a 2a5b 3037  ws ......- **[07
-00000ce0: 2e30 342e 3230 3233 5d2a 2a20 f09f 94a5  .04.2023]** ....
-00000cf0: f09f 94a5 2049 6d61 6765 4e65 7420 7072  .... ImageNet pr
-00000d00: 6574 7261 696e 6564 2046 6173 7465 7256  etrained FasterV
-00000d10: 6954 206d 6f64 656c 7320 6361 6e20 6e6f  iT models can no
-00000d20: 7720 6265 2069 6d70 6f72 7465 6420 7769  w be imported wi
-00000d30: 7468 202a 2a31 206c 696e 6520 6f66 2063  th **1 line of c
-00000d40: 6f64 652a 2a2e 2050 6c65 6173 6520 696e  ode**. Please in
-00000d50: 7374 616c 6c20 7468 6520 6c61 7465 7374  stall the latest
-00000d60: 2046 6173 7465 7256 6954 2070 6970 2070   FasterViT pip p
-00000d70: 6163 6b61 6765 2074 6f20 7573 6520 7468  ackage to use th
-00000d80: 6973 2066 756e 6374 696f 6e61 6c69 7479  is functionality
-00000d90: 2028 616c 736f 2073 7570 706f 7274 7320   (also supports 
-00000da0: 416e 792d 7265 736f 6c75 7469 6f6e 2046  Any-resolution F
-00000db0: 6173 7465 7256 6954 206d 6f64 656c 7329  asterViT models)
-00000dc0: 2e0a 2d20 2a2a 5b30 362e 3330 2e32 3032  ..- **[06.30.202
-00000dd0: 335d 2a2a 20f0 9f94 a520 5765 2068 6176  3]** .... We hav
-00000de0: 6520 6675 7274 6865 7220 696d 7072 6f76  e further improv
-00000df0: 6564 2074 6865 205b 5465 6e73 6f72 5254  ed the [TensorRT
-00000e00: 5d28 6874 7470 733a 2f2f 6465 7665 6c6f  ](https://develo
-00000e10: 7065 722e 6e76 6964 6961 2e63 6f6d 2f74  per.nvidia.com/t
-00000e20: 656e 736f 7272 742d 6765 7474 696e 672d  ensorrt-getting-
-00000e30: 7374 6172 7465 6429 2074 6872 6f75 6768  started) through
-00000e40: 7075 7420 6f66 2046 6173 7465 7256 6954  put of FasterViT
-00000e50: 206d 6f64 656c 7320 6279 2031 302d 3135   models by 10-15
-00000e60: 2520 6f6e 2061 7665 7261 6765 2061 6372  % on average acr
-00000e70: 6f73 7320 6469 6666 6572 656e 7420 6d6f  oss different mo
-00000e80: 6465 6c73 2e20 200a 2d20 2a2a 5b30 362e  dels.  .- **[06.
-00000e90: 3239 2e32 3032 335d 2a2a 2041 6e79 2d72  29.2023]** Any-r
-00000ea0: 6573 6f6c 7574 696f 6e20 4661 7374 6572  esolution Faster
-00000eb0: 5669 5420 6d6f 6465 6c20 6361 6e20 6e6f  ViT model can no
-00000ec0: 7720 6265 2069 6e74 6974 6961 6c69 7a65  w be intitialize
-00000ed0: 6420 6672 6f6d 2070 7265 2d74 7261 696e  d from pre-train
-00000ee0: 6564 2049 6d61 6765 4e65 7420 7265 736f  ed ImageNet reso
-00000ef0: 6c75 7469 6f6e 2028 3232 3420 7820 3234  lution (224 x 24
-00000f00: 3429 206d 6f64 656c 732e 0a2d 202a 2a5b  4) models..- **[
-00000f10: 3036 2e31 382e 3230 3233 5d2a 2a20 5765  06.18.2023]** We
-00000f20: 2068 6176 6520 7265 6c65 6173 6564 2074   have released t
-00000f30: 6865 2046 6173 7465 7256 6954 205b 7069  he FasterViT [pi
-00000f40: 7020 7061 636b 6167 655d 2868 7474 7073  p package](https
-00000f50: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
-00000f60: 6563 742f 6661 7374 6572 7669 742f 2920  ect/fastervit/) 
-00000f70: 210a 2d20 2a2a 5b30 362e 3137 2e32 3032  !.- **[06.17.202
-00000f80: 335d 2a2a 20f0 9f94 a520 5b41 6e79 2d72  3]** .... [Any-r
-00000f90: 6573 6f6c 7574 696f 6e20 4661 7374 6572  esolution Faster
-00000fa0: 5669 545d 282e 2f66 6173 7465 7276 6974  ViT](./fastervit
-00000fb0: 2f6d 6f64 656c 732f 6661 7374 6572 5f76  /models/faster_v
-00000fc0: 6974 5f61 6e79 5f72 6573 2e70 7929 2020  it_any_res.py)  
-00000fd0: 6d6f 6465 6c20 6973 206e 6f77 2061 7661  model is now ava
-00000fe0: 696c 6162 6c65 2021 2074 6865 206d 6f64  ilable ! the mod
-00000ff0: 656c 2063 616e 2062 6520 7573 6564 2066  el can be used f
-00001000: 6f72 2076 6172 6965 7479 206f 6620 6170  or variety of ap
-00001010: 706c 6963 6174 696f 6e73 2073 7563 6820  plications such 
-00001020: 6173 2064 6574 6563 7469 6f6e 2061 6e64  as detection and
-00001030: 2073 6567 6d65 6e74 6174 696f 6e20 6f72   segmentation or
-00001040: 2068 6967 682d 7265 736f 6c75 7469 6f6e   high-resolution
-00001050: 2066 696e 652d 7475 6e69 6e67 2077 6974   fine-tuning wit
-00001060: 6820 6172 6269 7472 6172 7920 696e 7075  h arbitrary inpu
-00001070: 7420 696d 6167 6520 7265 736f 6c75 7469  t image resoluti
-00001080: 6f6e 732e 0a2d 202a 2a5b 3036 2e30 392e  ons..- **[06.09.
-00001090: 3230 3233 5d2a 2a20 f09f 94a5 f09f 94a5  2023]** ........
-000010a0: 2057 6520 6861 7665 2072 656c 6561 7365   We have release
-000010b0: 6420 736f 7572 6365 2063 6f64 6520 616e  d source code an
-000010c0: 6420 496d 6167 654e 6574 2d31 4b20 4661  d ImageNet-1K Fa
-000010d0: 7374 6572 5669 542d 6d6f 6465 6c73 2021  sterViT-models !
-000010e0: 0a0a 0a23 2320 4361 7461 6c6f 670a 2d20  ...## Catalog.- 
-000010f0: 5b78 5d20 496d 6167 654e 6574 2d31 4b20  [x] ImageNet-1K 
-00001100: 7472 6169 6e69 6e67 2063 6f64 650a 2d20  training code.- 
-00001110: 5b78 5d20 496d 6167 654e 6574 2d31 4b20  [x] ImageNet-1K 
-00001120: 7072 652d 7472 6169 6e65 6420 6d6f 6465  pre-trained mode
-00001130: 6c73 0a2d 205b 785d 2041 6e79 2d72 6573  ls.- [x] Any-res
-00001140: 6f6c 7574 696f 6e20 4661 7374 6572 5669  olution FasterVi
-00001150: 540a 2d20 5b78 5d20 4661 7374 6572 5669  T.- [x] FasterVi
-00001160: 5420 7069 702d 7061 636b 6167 6520 7265  T pip-package re
-00001170: 6c65 6173 650a 2d20 5b78 5d20 4164 6420  lease.- [x] Add 
-00001180: 6361 7061 626c 6974 7920 746f 2069 6e69  capablity to ini
-00001190: 7469 616c 697a 6520 616e 792d 7265 736f  tialize any-reso
-000011a0: 6c75 7469 6f6e 2046 6173 7465 7256 6954  lution FasterViT
-000011b0: 2066 726f 6d20 496d 6167 654e 6574 2d70   from ImageNet-p
-000011c0: 7265 7472 6169 6e65 6420 7765 6967 6874  retrained weight
-000011d0: 732e 200a 2d20 5b20 5d20 496d 6167 654e  s. .- [ ] ImageN
-000011e0: 6574 2d32 314b 2070 7265 2d74 7261 696e  et-21K pre-train
-000011f0: 6564 206d 6f64 656c 730a 2d20 5b20 5d20  ed models.- [ ] 
-00001200: 4465 7465 6374 696f 6e20 636f 6465 2028  Detection code (
-00001210: 4449 4e4f 2920 2b20 6d6f 6465 6c73 0a2d  DINO) + models.-
-00001220: 205b 205d 2053 6567 6d65 6e74 6174 696f   [ ] Segmentatio
-00001230: 6e20 636f 6465 202b 206d 6f64 656c 730a  n code + models.
-00001240: 0a2d 2d2d 200a 0a23 2320 5265 7375 6c74  .--- ..## Result
-00001250: 7320 2b20 5072 6574 7261 696e 6564 204d  s + Pretrained M
-00001260: 6f64 656c 730a 0a23 2323 2049 6d61 6765  odels..### Image
-00001270: 4e65 742d 314b 0a2a 2a46 6173 7465 7256  Net-1K.**FasterV
-00001280: 6954 2049 6d61 6765 4e65 742d 314b 2050  iT ImageNet-1K P
-00001290: 7265 7472 6169 6e65 6420 4d6f 6465 6c73  retrained Models
-000012a0: 2a2a 0a0a 3c74 6162 6c65 3e0a 2020 3c74  **..<table>.  <t
-000012b0: 723e 0a20 2020 203c 7468 3e4e 616d 653c  r>.    <th>Name<
-000012c0: 2f74 683e 0a20 2020 203c 7468 3e41 6363  /th>.    <th>Acc
-000012d0: 4031 2825 293c 2f74 683e 0a20 2020 203c  @1(%)</th>.    <
-000012e0: 7468 3e41 6363 4035 2825 293c 2f74 683e  th>Acc@5(%)</th>
-000012f0: 0a20 2020 203c 7468 3e54 6872 6f75 6768  .    <th>Through
-00001300: 7075 7428 496d 672f 5365 6329 3c2f 7468  put(Img/Sec)</th
-00001310: 3e0a 2020 2020 3c74 683e 5265 736f 6c75  >.    <th>Resolu
-00001320: 7469 6f6e 3c2f 7468 3e0a 2020 2020 3c74  tion</th>.    <t
-00001330: 683e 2350 6172 616d 7328 4d29 3c2f 7468  h>#Params(M)</th
-00001340: 3e0a 2020 2020 3c74 683e 464c 4f50 7328  >.    <th>FLOPs(
-00001350: 4729 3c2f 7468 3e0a 2020 2020 3c74 683e  G)</th>.    <th>
-00001360: 446f 776e 6c6f 6164 3c2f 7468 3e0a 2020  Download</th>.  
-00001370: 3c2f 7472 3e0a 0a3c 7472 3e0a 2020 2020  </tr>..<tr>.    
-00001380: 3c74 643e 4661 7374 6572 5669 542d 303c  <td>FasterViT-0<
-00001390: 2f74 643e 0a20 2020 203c 7464 3e38 322e  /td>.    <td>82.
-000013a0: 313c 2f74 643e 0a20 2020 203c 7464 3e39  1</td>.    <td>9
-000013b0: 352e 393c 2f74 643e 0a20 2020 203c 7464  5.9</td>.    <td
-000013c0: 3e35 3830 323c 2f74 643e 0a20 2020 203c  >5802</td>.    <
-000013d0: 7464 3e32 3234 7832 3234 3c2f 7464 3e0a  td>224x224</td>.
-000013e0: 2020 2020 3c74 643e 3331 2e34 3c2f 7464      <td>31.4</td
-000013f0: 3e0a 2020 2020 3c74 643e 332e 333c 2f74  >.    <td>3.3</t
-00001400: 643e 0a20 2020 203c 7464 3e3c 6120 6872  d>.    <td><a hr
-00001410: 6566 3d22 6874 7470 733a 2f2f 6472 6976  ef="https://driv
-00001420: 652e 676f 6f67 6c65 2e63 6f6d 2f75 633f  e.google.com/uc?
-00001430: 6578 706f 7274 3d64 6f77 6e6c 6f61 6426  export=download&
-00001440: 6964 3d31 7477 4932 4c46 4a73 3339 3159  id=1twI2LFJs391Y
-00001450: 726a 384d 5234 5569 3950 6672 7657 716a  rj8MR4Ui9PfrvWqj
-00001460: 4531 6942 223e 6d6f 6465 6c3c 2f61 3e3c  E1iB">model</a><
-00001470: 2f74 643e 0a3c 2f74 723e 0a0a 3c74 723e  /td>.</tr>..<tr>
-00001480: 0a20 2020 203c 7464 3e46 6173 7465 7256  .    <td>FasterV
-00001490: 6954 2d31 3c2f 7464 3e0a 2020 2020 3c74  iT-1</td>.    <t
-000014a0: 643e 3833 2e32 3c2f 7464 3e0a 2020 2020  d>83.2</td>.    
-000014b0: 3c74 643e 3936 2e35 3c2f 7464 3e0a 2020  <td>96.5</td>.  
-000014c0: 2020 3c74 643e 3431 3838 3c2f 7464 3e0a    <td>4188</td>.
-000014d0: 2020 2020 3c74 643e 3232 3478 3232 343c      <td>224x224<
-000014e0: 2f74 643e 0a20 2020 203c 7464 3e35 332e  /td>.    <td>53.
-000014f0: 343c 2f74 643e 0a20 2020 203c 7464 3e35  4</td>.    <td>5
-00001500: 2e33 3c2f 7464 3e0a 2020 2020 3c74 643e  .3</td>.    <td>
-00001510: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00001520: 2f64 7269 7665 2e67 6f6f 676c 652e 636f  /drive.google.co
-00001530: 6d2f 7563 3f65 7870 6f72 743d 646f 776e  m/uc?export=down
-00001540: 6c6f 6164 2669 643d 3172 3757 3130 6e35  load&id=1r7W10n5
-00001550: 2d62 4674 4d33 737a 3462 6d61 4c72 6f77  -bFtM3sz4bmaLrow
-00001560: 4e32 6759 506b 4c47 5422 3e6d 6f64 656c  N2gYPkLGT">model
-00001570: 3c2f 613e 3c2f 7464 3e0a 3c2f 7472 3e0a  </a></td>.</tr>.
-00001580: 0a3c 7472 3e0a 2020 2020 3c74 643e 4661  .<tr>.    <td>Fa
-00001590: 7374 6572 5669 542d 323c 2f74 643e 0a20  sterViT-2</td>. 
-000015a0: 2020 203c 7464 3e38 342e 323c 2f74 643e     <td>84.2</td>
-000015b0: 0a20 2020 203c 7464 3e39 362e 383c 2f74  .    <td>96.8</t
-000015c0: 643e 0a20 2020 203c 7464 3e33 3136 313c  d>.    <td>3161<
-000015d0: 2f74 643e 0a20 2020 203c 7464 3e32 3234  /td>.    <td>224
-000015e0: 7832 3234 3c2f 7464 3e0a 2020 2020 3c74  x224</td>.    <t
-000015f0: 643e 3735 2e39 3c2f 7464 3e0a 2020 2020  d>75.9</td>.    
-00001600: 3c74 643e 382e 373c 2f74 643e 0a20 2020  <td>8.7</td>.   
-00001610: 203c 7464 3e3c 6120 6872 6566 3d22 6874   <td><a href="ht
-00001620: 7470 733a 2f2f 6472 6976 652e 676f 6f67  tps://drive.goog
-00001630: 6c65 2e63 6f6d 2f75 633f 6578 706f 7274  le.com/uc?export
-00001640: 3d64 6f77 6e6c 6f61 6426 6964 3d31 6e5f  =download&id=1n_
-00001650: 6136 7330 7067 6930 6a56 5a4f 476d 4465  a6s0pgi0jVZOGmDe
-00001660: 6932 7658 4855 3545 3652 4835 7755 223e  i2vXHU5E6RH5wU">
-00001670: 6d6f 6465 6c3c 2f61 3e3c 2f74 643e 0a3c  model</a></td>.<
-00001680: 2f74 723e 0a0a 3c74 723e 0a20 2020 203c  /tr>..<tr>.    <
-00001690: 7464 3e46 6173 7465 7256 6954 2d33 3c2f  td>FasterViT-3</
-000016a0: 7464 3e0a 2020 2020 3c74 643e 3834 2e39  td>.    <td>84.9
-000016b0: 3c2f 7464 3e0a 2020 2020 3c74 643e 3937  </td>.    <td>97
-000016c0: 2e32 3c2f 7464 3e0a 2020 2020 3c74 643e  .2</td>.    <td>
-000016d0: 3137 3830 3c2f 7464 3e0a 2020 2020 3c74  1780</td>.    <t
-000016e0: 643e 3232 3478 3232 343c 2f74 643e 0a20  d>224x224</td>. 
-000016f0: 2020 203c 7464 3e31 3539 2e35 3c2f 7464     <td>159.5</td
-00001700: 3e0a 2020 2020 3c74 643e 3138 2e32 3c2f  >.    <td>18.2</
-00001710: 7464 3e0a 2020 2020 3c74 643e 3c61 2068  td>.    <td><a h
-00001720: 7265 663d 2268 7474 7073 3a2f 2f64 7269  ref="https://dri
-00001730: 7665 2e67 6f6f 676c 652e 636f 6d2f 7563  ve.google.com/uc
-00001740: 3f65 7870 6f72 743d 646f 776e 6c6f 6164  ?export=download
-00001750: 2669 643d 3174 7657 456c 5a39 3153 6961  &id=1tvWElZ91Sia
-00001760: 3253 7358 5958 464d 4e59 5177 6669 7043  2SsXYXFMNYQwfipC
-00001770: 7874 4937 5822 3e6d 6f64 656c 3c2f 613e  xtI7X">model</a>
-00001780: 3c2f 7464 3e0a 3c2f 7472 3e0a 0a3c 7472  </td>.</tr>..<tr
-00001790: 3e0a 2020 2020 3c74 643e 4661 7374 6572  >.    <td>Faster
-000017a0: 5669 542d 343c 2f74 643e 0a20 2020 203c  ViT-4</td>.    <
-000017b0: 7464 3e38 352e 343c 2f74 643e 0a20 2020  td>85.4</td>.   
-000017c0: 203c 7464 3e39 372e 333c 2f74 643e 0a20   <td>97.3</td>. 
-000017d0: 2020 203c 7464 3e38 3439 3c2f 7464 3e0a     <td>849</td>.
-000017e0: 2020 2020 3c74 643e 3232 3478 3232 343c      <td>224x224<
-000017f0: 2f74 643e 0a20 2020 203c 7464 3e34 3234  /td>.    <td>424
-00001800: 2e36 3c2f 7464 3e0a 2020 2020 3c74 643e  .6</td>.    <td>
-00001810: 3336 2e36 3c2f 7464 3e0a 2020 2020 3c74  36.6</td>.    <t
-00001820: 643e 3c61 2068 7265 663d 2268 7474 7073  d><a href="https
-00001830: 3a2f 2f64 7269 7665 2e67 6f6f 676c 652e  ://drive.google.
-00001840: 636f 6d2f 7563 3f65 7870 6f72 743d 646f  com/uc?export=do
-00001850: 776e 6c6f 6164 2669 643d 3167 5968 5841  wnload&id=1gYhXA
-00001860: 3332 512d 5f39 4335 4458 656c 3137 6176  32Q-_9C5DXel17av
-00001870: 565f 5a4c 6f61 4877 6467 7a22 3e6d 6f64  V_ZLoaHwdgz">mod
-00001880: 656c 3c2f 613e 3c2f 7464 3e0a 3c2f 7472  el</a></td>.</tr
-00001890: 3e0a 0a3c 7472 3e0a 2020 2020 3c74 643e  >..<tr>.    <td>
-000018a0: 4661 7374 6572 5669 542d 353c 2f74 643e  FasterViT-5</td>
-000018b0: 0a20 2020 203c 7464 3e38 352e 363c 2f74  .    <td>85.6</t
-000018c0: 643e 0a20 2020 203c 7464 3e39 372e 343c  d>.    <td>97.4<
-000018d0: 2f74 643e 0a20 2020 203c 7464 3e34 3439  /td>.    <td>449
-000018e0: 3c2f 7464 3e0a 2020 2020 3c74 643e 3232  </td>.    <td>22
-000018f0: 3478 3232 343c 2f74 643e 0a20 2020 203c  4x224</td>.    <
-00001900: 7464 3e39 3735 2e35 3c2f 7464 3e0a 2020  td>975.5</td>.  
-00001910: 2020 3c74 643e 3131 332e 303c 2f74 643e    <td>113.0</td>
-00001920: 0a20 2020 203c 7464 3e3c 6120 6872 6566  .    <td><a href
-00001930: 3d22 6874 7470 733a 2f2f 6472 6976 652e  ="https://drive.
-00001940: 676f 6f67 6c65 2e63 6f6d 2f75 633f 6578  google.com/uc?ex
-00001950: 706f 7274 3d64 6f77 6e6c 6f61 6426 6964  port=download&id
-00001960: 3d31 6d71 7061 6937 5869 484c 725f 6e31  =1mqpai7XiHLr_n1
-00001970: 746a 786a 7a54 3871 3336 3978 5443 715f  tjxjzT8q369xTCq_
-00001980: 7a2d 223e 6d6f 6465 6c3c 2f61 3e3c 2f74  z-">model</a></t
-00001990: 643e 0a3c 2f74 723e 0a0a 3c74 723e 0a20  d>.</tr>..<tr>. 
-000019a0: 2020 203c 7464 3e46 6173 7465 7256 6954     <td>FasterViT
-000019b0: 2d36 3c2f 7464 3e0a 2020 2020 3c74 643e  -6</td>.    <td>
-000019c0: 3835 2e38 3c2f 7464 3e0a 2020 2020 3c74  85.8</td>.    <t
-000019d0: 643e 3937 2e34 3c2f 7464 3e0a 2020 2020  d>97.4</td>.    
-000019e0: 3c74 643e 3335 323c 2f74 643e 0a20 2020  <td>352</td>.   
-000019f0: 203c 7464 3e32 3234 7832 3234 3c2f 7464   <td>224x224</td
-00001a00: 3e0a 2020 2020 3c74 643e 3133 3630 2e30  >.    <td>1360.0
-00001a10: 3c2f 7464 3e0a 2020 2020 3c74 643e 3134  </td>.    <td>14
-00001a20: 322e 303c 2f74 643e 0a20 2020 203c 7464  2.0</td>.    <td
-00001a30: 3e3c 6120 6872 6566 3d22 6874 7470 733a  ><a href="https:
-00001a40: 2f2f 6472 6976 652e 676f 6f67 6c65 2e63  //drive.google.c
-00001a50: 6f6d 2f75 633f 6578 706f 7274 3d64 6f77  om/uc?export=dow
-00001a60: 6e6c 6f61 6426 6964 3d31 326a 7461 7652  nload&id=12jtavR
-00001a70: 3251 786d 4d7a 634b 7750 7a57 6537 6b77  2QxmMzcKwPzWe7kw
-00001a80: 2d6f 7933 3449 5969 3539 223e 6d6f 6465  -oy34IYi59">mode
-00001a90: 6c3c 2f61 3e3c 2f74 643e 0a3c 2f74 723e  l</a></td>.</tr>
-00001aa0: 0a0a 3c2f 7461 626c 653e 0a0a 0a23 2323  ..</table>...###
-00001ab0: 2052 6f62 7573 746e 6573 7320 2849 6d61   Robustness (Ima
-00001ac0: 6765 4e65 742d 4120 2d20 496d 6167 654e  geNet-A - ImageN
-00001ad0: 6574 2d52 202d 2049 6d61 6765 4e65 742d  et-R - ImageNet-
-00001ae0: 5632 290a 0a41 6c6c 206d 6f64 656c 7320  V2)..All models 
-00001af0: 7573 6520 6063 726f 705f 7063 743d 302e  use `crop_pct=0.
-00001b00: 3837 3560 2e20 5265 7375 6c74 7320 6172  875`. Results ar
-00001b10: 6520 6f62 7461 696e 6564 2062 7920 7275  e obtained by ru
-00001b20: 6e6e 696e 6720 696e 6665 7265 6e63 6520  nning inference 
-00001b30: 6f6e 2049 6d61 6765 4e65 742d 314b 2070  on ImageNet-1K p
-00001b40: 7265 7472 6169 6e65 6420 6d6f 6465 6c73  retrained models
-00001b50: 2077 6974 686f 7574 2066 696e 6574 756e   without finetun
-00001b60: 696e 672e 0a3c 7461 626c 653e 0a20 203c  ing..<table>.  <
-00001b70: 7472 3e0a 2020 2020 3c74 683e 4e61 6d65  tr>.    <th>Name
-00001b80: 3c2f 7468 3e0a 2020 2020 3c74 683e 412d  </th>.    <th>A-
-00001b90: 4163 6340 3128 2529 3c2f 7468 3e0a 2020  Acc@1(%)</th>.  
-00001ba0: 2020 3c74 683e 412d 4163 6340 3528 2529    <th>A-Acc@5(%)
-00001bb0: 3c2f 7468 3e0a 2020 2020 3c74 683e 522d  </th>.    <th>R-
-00001bc0: 4163 6340 3128 2529 3c2f 7468 3e0a 2020  Acc@1(%)</th>.  
-00001bd0: 2020 3c74 683e 522d 4163 6340 3528 2529    <th>R-Acc@5(%)
-00001be0: 3c2f 7468 3e0a 2020 2020 3c74 683e 5632  </th>.    <th>V2
-00001bf0: 2d41 6363 4031 2825 293c 2f74 683e 0a20  -Acc@1(%)</th>. 
-00001c00: 2020 203c 7468 3e56 322d 4163 6340 3528     <th>V2-Acc@5(
-00001c10: 2529 3c2f 7468 3e0a 2020 3c2f 7472 3e0a  %)</th>.  </tr>.
-00001c20: 0a3c 7472 3e0a 2020 2020 3c74 643e 4661  .<tr>.    <td>Fa
-00001c30: 7374 6572 5669 542d 303c 2f74 643e 0a20  sterViT-0</td>. 
-00001c40: 2020 203c 7464 3e32 332e 393c 2f74 643e     <td>23.9</td>
-00001c50: 0a20 2020 203c 7464 3e35 372e 363c 2f74  .    <td>57.6</t
-00001c60: 643e 0a20 2020 203c 7464 3e34 352e 393c  d>.    <td>45.9<
-00001c70: 2f74 643e 0a20 2020 203c 7464 3e36 302e  /td>.    <td>60.
-00001c80: 343c 2f74 643e 0a20 2020 203c 7464 3e37  4</td>.    <td>7
-00001c90: 302e 393c 2f74 643e 0a20 2020 203c 7464  0.9</td>.    <td
-00001ca0: 3e39 302e 303c 2f74 643e 0a3c 2f74 723e  >90.0</td>.</tr>
-00001cb0: 0a0a 3c74 723e 0a20 2020 203c 7464 3e46  ..<tr>.    <td>F
-00001cc0: 6173 7465 7256 6954 2d31 3c2f 7464 3e0a  asterViT-1</td>.
-00001cd0: 2020 2020 3c74 643e 3331 2e32 3c2f 7464      <td>31.2</td
-00001ce0: 3e0a 2020 2020 3c74 643e 3633 2e33 3c2f  >.    <td>63.3</
-00001cf0: 7464 3e0a 2020 2020 3c74 643e 3437 2e35  td>.    <td>47.5
-00001d00: 3c2f 7464 3e0a 2020 2020 3c74 643e 3631  </td>.    <td>61
-00001d10: 2e39 3c2f 7464 3e0a 2020 2020 3c74 643e  .9</td>.    <td>
-00001d20: 3732 2e36 3c2f 7464 3e0a 2020 2020 3c74  72.6</td>.    <t
-00001d30: 643e 3931 2e30 3c2f 7464 3e0a 3c2f 7472  d>91.0</td>.</tr
-00001d40: 3e0a 0a3c 7472 3e0a 2020 2020 3c74 643e  >..<tr>.    <td>
-00001d50: 4661 7374 6572 5669 542d 323c 2f74 643e  FasterViT-2</td>
-00001d60: 0a20 2020 203c 7464 3e33 382e 323c 2f74  .    <td>38.2</t
-00001d70: 643e 0a20 2020 203c 7464 3e36 382e 393c  d>.    <td>68.9<
-00001d80: 2f74 643e 0a20 2020 203c 7464 3e34 392e  /td>.    <td>49.
-00001d90: 363c 2f74 643e 0a20 2020 203c 7464 3e36  6</td>.    <td>6
-00001da0: 332e 343c 2f74 643e 0a20 2020 203c 7464  3.4</td>.    <td
-00001db0: 3e37 332e 373c 2f74 643e 0a20 2020 203c  >73.7</td>.    <
-00001dc0: 7464 3e39 312e 363c 2f74 643e 0a3c 2f74  td>91.6</td>.</t
-00001dd0: 723e 0a0a 3c74 723e 0a20 2020 203c 7464  r>..<tr>.    <td
-00001de0: 3e46 6173 7465 7256 6954 2d33 3c2f 7464  >FasterViT-3</td
-00001df0: 3e0a 2020 2020 3c74 643e 3434 2e32 3c2f  >.    <td>44.2</
-00001e00: 7464 3e0a 2020 2020 3c74 643e 3733 2e30  td>.    <td>73.0
-00001e10: 3c2f 7464 3e0a 2020 2020 3c74 643e 3531  </td>.    <td>51
-00001e20: 2e39 3c2f 7464 3e0a 2020 2020 3c74 643e  .9</td>.    <td>
-00001e30: 3635 2e36 3c2f 7464 3e0a 2020 2020 3c74  65.6</td>.    <t
-00001e40: 643e 3735 2e30 3c2f 7464 3e0a 2020 2020  d>75.0</td>.    
-00001e50: 3c74 643e 3932 2e32 3c2f 7464 3e0a 3c2f  <td>92.2</td>.</
-00001e60: 7472 3e0a 0a3c 7472 3e0a 2020 2020 3c74  tr>..<tr>.    <t
-00001e70: 643e 4661 7374 6572 5669 542d 343c 2f74  d>FasterViT-4</t
-00001e80: 643e 0a20 2020 203c 7464 3e34 392e 303c  d>.    <td>49.0<
-00001e90: 2f74 643e 0a20 2020 203c 7464 3e37 352e  /td>.    <td>75.
-00001ea0: 343c 2f74 643e 0a20 2020 203c 7464 3e35  4</td>.    <td>5
-00001eb0: 362e 303c 2f74 643e 0a20 2020 203c 7464  6.0</td>.    <td
-00001ec0: 3e36 392e 363c 2f74 643e 0a20 2020 203c  >69.6</td>.    <
-00001ed0: 7464 3e37 352e 373c 2f74 643e 0a20 2020  td>75.7</td>.   
-00001ee0: 203c 7464 3e39 322e 373c 2f74 643e 0a3c   <td>92.7</td>.<
-00001ef0: 2f74 723e 0a0a 3c74 723e 0a20 2020 203c  /tr>..<tr>.    <
-00001f00: 7464 3e46 6173 7465 7256 6954 2d35 3c2f  td>FasterViT-5</
-00001f10: 7464 3e0a 2020 2020 3c74 643e 3532 2e37  td>.    <td>52.7
-00001f20: 3c2f 7464 3e0a 2020 2020 3c74 643e 3737  </td>.    <td>77
-00001f30: 2e36 3c2f 7464 3e0a 2020 2020 3c74 643e  .6</td>.    <td>
-00001f40: 3536 2e39 3c2f 7464 3e0a 2020 2020 3c74  56.9</td>.    <t
-00001f50: 643e 3730 2e30 3c2f 7464 3e0a 2020 2020  d>70.0</td>.    
-00001f60: 3c74 643e 3736 2e30 3c2f 7464 3e0a 2020  <td>76.0</td>.  
-00001f70: 2020 3c74 643e 3933 2e30 3c2f 7464 3e0a    <td>93.0</td>.
-00001f80: 3c2f 7472 3e0a 0a3c 7472 3e0a 2020 2020  </tr>..<tr>.    
-00001f90: 3c74 643e 4661 7374 6572 5669 542d 363c  <td>FasterViT-6<
-00001fa0: 2f74 643e 0a20 2020 203c 7464 3e35 332e  /td>.    <td>53.
-00001fb0: 373c 2f74 643e 0a20 2020 203c 7464 3e37  7</td>.    <td>7
-00001fc0: 382e 343c 2f74 643e 0a20 2020 203c 7464  8.4</td>.    <td
-00001fd0: 3e35 372e 313c 2f74 643e 0a20 2020 203c  >57.1</td>.    <
-00001fe0: 7464 3e37 302e 313c 2f74 643e 0a20 2020  td>70.1</td>.   
-00001ff0: 203c 7464 3e37 362e 313c 2f74 643e 0a20   <td>76.1</td>. 
-00002000: 2020 203c 7464 3e39 332e 303c 2f74 643e     <td>93.0</td>
-00002010: 0a3c 2f74 723e 0a0a 3c2f 7461 626c 653e  .</tr>..</table>
-00002020: 0a0a 412c 2052 2061 6e64 2056 3220 6465  ..A, R and V2 de
-00002030: 6e6f 7465 2049 6d61 6765 4e65 742d 412c  note ImageNet-A,
-00002040: 2049 6d61 6765 4e65 742d 5220 616e 6420   ImageNet-R and 
-00002050: 496d 6167 654e 6574 2d56 3220 7265 7370  ImageNet-V2 resp
-00002060: 6563 7469 7665 6c79 2e20 0a23 2320 5472  ectively. .## Tr
-00002070: 6169 6e69 6e67 0a0a 506c 6561 7365 2073  aining..Please s
-00002080: 6565 205b 5452 4149 4e49 4e47 2e6d 645d  ee [TRAINING.md]
-00002090: 2854 5241 494e 494e 472e 6d64 2920 666f  (TRAINING.md) fo
-000020a0: 7220 6465 7461 696c 6564 2074 7261 696e  r detailed train
-000020b0: 696e 6720 696e 7374 7275 6374 696f 6e73  ing instructions
-000020c0: 206f 6620 616c 6c20 6d6f 6465 6c73 2e20   of all models. 
-000020d0: 0a0a 2323 2045 7661 6c75 6174 696f 6e0a  ..## Evaluation.
-000020e0: 0a54 6865 2046 6173 7465 7256 6954 206d  .The FasterViT m
-000020f0: 6f64 656c 7320 6361 6e20 6265 2065 7661  odels can be eva
-00002100: 6c75 6174 6564 206f 6e20 496d 6167 654e  luated on ImageN
-00002110: 6574 2d31 4b20 7661 6c69 6461 7469 6f6e  et-1K validation
-00002120: 2073 6574 2075 7369 6e67 2074 6865 2066   set using the f
-00002130: 6f6c 6c6f 7769 6e67 3a20 0a0a 6060 600a  ollowing: ..```.
-00002140: 7079 7468 6f6e 2076 616c 6964 6174 652e  python validate.
-00002150: 7079 205c 0a2d 2d6d 6f64 656c 203c 6d6f  py \.--model <mo
-00002160: 6465 6c2d 6e61 6d65 3e0a 2d2d 6368 6563  del-name>.--chec
-00002170: 6b70 6f69 6e74 203c 6368 6563 6b70 6f69  kpoint <checkpoi
-00002180: 6e74 2d70 6174 683e 0a2d 2d64 6174 615f  nt-path>.--data_
-00002190: 6469 7220 3c69 6d61 6765 6e65 742d 7061  dir <imagenet-pa
-000021a0: 7468 3e0a 2d2d 6261 7463 682d 7369 7a65  th>.--batch-size
-000021b0: 203c 6261 7463 682d 7369 7a65 2d70 6572   <batch-size-per
-000021c0: 2d67 7075 0a60 6060 200a 0a48 6572 6520  -gpu.``` ..Here 
-000021d0: 602d 2d6d 6f64 656c 6020 6973 2074 6865  `--model` is the
-000021e0: 2046 6173 7465 7256 6954 2076 6172 6961   FasterViT varia
-000021f0: 6e74 2028 652e 672e 2060 6661 7374 6572  nt (e.g. `faster
-00002200: 5f76 6974 5f30 5f32 3234 5f31 6b60 292c  _vit_0_224_1k`),
-00002210: 2060 2d2d 6368 6563 6b70 6f69 6e74 6020   `--checkpoint` 
-00002220: 6973 2074 6865 2070 6174 6820 746f 2070  is the path to p
-00002230: 7265 7472 6169 6e65 6420 6d6f 6465 6c20  retrained model 
-00002240: 7765 6967 6874 732c 2060 2d2d 6461 7461  weights, `--data
-00002250: 5f64 6972 6020 6973 2074 6865 2070 6174  _dir` is the pat
-00002260: 6820 746f 2049 6d61 6765 4e65 742d 314b  h to ImageNet-1K
-00002270: 2076 616c 6964 6174 696f 6e20 7365 7420   validation set 
-00002280: 616e 6420 602d 2d62 6174 6368 2d73 697a  and `--batch-siz
-00002290: 6560 2069 7320 7468 6520 6e75 6d62 6572  e` is the number
-000022a0: 206f 6620 6261 7463 6820 7369 7a65 2e20   of batch size. 
-000022b0: 5765 2061 6c73 6f20 7072 6f76 6964 6520  We also provide 
-000022c0: 6120 7361 6d70 6c65 2073 6372 6970 7420  a sample script 
-000022d0: 5b68 6572 655d 282e 2f66 6173 7465 7276  [here](./fasterv
-000022e0: 6974 2f76 616c 6964 6174 652e 7368 292e  it/validate.sh).
-000022f0: 200a 0a23 2320 4f4e 4e58 2043 6f6e 7665   ..## ONNX Conve
-00002300: 7273 696f 6e0a 0a57 6520 7072 6f76 6964  rsion..We provid
-00002310: 6520 4f4e 4e58 2063 6f6e 7665 7273 696f  e ONNX conversio
-00002320: 6e20 7363 7269 7074 2074 6f20 656e 6162  n script to enab
-00002330: 6c65 2064 796e 616d 6963 2062 6174 6368  le dynamic batch
-00002340: 2073 697a 6520 696e 6665 7265 6e63 652e   size inference.
-00002350: 2046 6f72 2069 6e73 7461 6e63 652c 2074   For instance, t
-00002360: 6f20 6765 6e65 7261 7465 204f 4e4e 5820  o generate ONNX 
-00002370: 6d6f 6465 6c20 666f 7220 6066 6173 7465  model for `faste
-00002380: 725f 7669 745f 305f 616e 795f 7265 7360  r_vit_0_any_res`
-00002390: 2077 6974 6820 7265 736f 6c75 7469 6f6e   with resolution
-000023a0: 2035 3736 2078 2039 3630 2061 6e64 204f   576 x 960 and O
-000023b0: 4e4e 5820 6f70 7365 7420 6e75 6d62 6572  NNX opset number
-000023c0: 2031 372c 2074 6865 2066 6f6c 6c6f 7769   17, the followi
-000023d0: 6e67 2063 616e 2062 6520 7573 6564 2e20  ng can be used. 
-000023e0: 0a0a 6060 6062 6173 6820 0a70 7974 686f  ..```bash .pytho
-000023f0: 6e20 6f6e 6e78 5f63 6f6e 7665 7274 202d  n onnx_convert -
-00002400: 2d6d 6f64 656c 2d6e 616d 6520 6661 7374  -model-name fast
-00002410: 6572 5f76 6974 5f30 5f61 6e79 5f72 6573  er_vit_0_any_res
-00002420: 202d 2d72 6573 6f6c 7574 696f 6e2d 6820   --resolution-h 
-00002430: 3537 3620 2d2d 7265 736f 6c75 7469 6f6e  576 --resolution
-00002440: 2d77 2039 3630 202d 2d6f 6e6e 782d 6f70  -w 960 --onnx-op
-00002450: 7365 7420 3137 0a0a 6060 600a 0a0a 2323  set 17..```...##
-00002460: 2049 6e73 7461 6c6c 6174 696f 6e0a 0a54   Installation..T
-00002470: 6865 2064 6570 656e 6465 6e63 6965 7320  he dependencies 
-00002480: 6361 6e20 6265 2069 6e73 7461 6c6c 6564  can be installed
-00002490: 2062 7920 7275 6e6e 696e 673a 0a0a 6060   by running:..``
-000024a0: 6062 6173 680a 7069 7020 696e 7374 616c  `bash.pip instal
-000024b0: 6c20 2d72 2072 6571 7569 7265 6d65 6e74  l -r requirement
-000024c0: 732e 7478 740a 6060 600a 0a23 2320 5374  s.txt.```..## St
-000024d0: 6172 2048 6973 746f 7279 0a0a 5b21 5b53  ar History..[![S
-000024e0: 7461 7220 4869 7374 6f72 7920 4368 6172  tar History Char
-000024f0: 745d 2868 7474 7073 3a2f 2f61 7069 2e73  t](https://api.s
-00002500: 7461 722d 6869 7374 6f72 792e 636f 6d2f  tar-history.com/
-00002510: 7376 673f 7265 706f 733d 4e56 6c61 6273  svg?repos=NVlabs
-00002520: 2f46 6173 7465 7256 6954 2674 7970 653d  /FasterViT&type=
-00002530: 4461 7465 295d 2868 7474 7073 3a2f 2f73  Date)](https://s
-00002540: 7461 722d 6869 7374 6f72 792e 636f 6d2f  tar-history.com/
-00002550: 234e 566c 6162 732f 4661 7374 6572 5669  #NVlabs/FasterVi
-00002560: 5426 4461 7465 290a 0a0a 2323 2054 6869  T&Date)...## Thi
-00002570: 7264 2d70 6172 7479 2045 7874 656e 7469  rd-party Extenti
-00002580: 6f6e 730a 5765 2061 6c77 6179 7320 7765  ons.We always we
-00002590: 6c63 6f6d 6520 7468 6972 642d 7061 7274  lcome third-part
-000025a0: 7920 6578 7465 6e74 696f 6e73 2f69 6d70  y extentions/imp
-000025b0: 6c65 6d65 6e74 6174 696f 6e73 2061 6e64  lementations and
-000025c0: 2075 7361 6765 2066 6f72 206f 7468 6572   usage for other
-000025d0: 2070 7572 706f 7365 732e 2049 6620 796f   purposes. If yo
-000025e0: 7520 776f 756c 6420 6c69 6b65 2079 6f75  u would like you
-000025f0: 7220 776f 726b 2074 6f20 6265 206c 6973  r work to be lis
-00002600: 7465 6420 696e 2074 6869 7320 7265 706f  ted in this repo
-00002610: 7369 746f 7279 2c20 706c 6561 7365 2072  sitory, please r
-00002620: 6169 7365 2061 6e64 2069 7373 7565 2061  aise and issue a
-00002630: 6e64 2070 726f 7669 6465 2075 7320 7769  nd provide us wi
-00002640: 7468 2064 6574 6169 6c65 6420 696e 666f  th detailed info
-00002650: 726d 6174 696f 6e2e 2020 0a0a 2323 2043  rmation.  ..## C
-00002660: 6974 6174 696f 6e0a 0a50 6c65 6173 6520  itation..Please 
-00002670: 636f 6e73 6964 6572 2063 6974 696e 6720  consider citing 
-00002680: 4661 7374 6572 5669 5420 6966 2074 6869  FasterViT if thi
-00002690: 7320 7265 706f 7369 746f 7279 2069 7320  s repository is 
-000026a0: 7573 6566 756c 2066 6f72 2079 6f75 7220  useful for your 
-000026b0: 776f 726b 2e20 0a0a 6060 600a 4061 7274  work. ..```.@art
-000026c0: 6963 6c65 7b68 6174 616d 697a 6164 6568  icle{hatamizadeh
-000026d0: 3230 3233 6661 7374 6572 7669 742c 0a20  2023fastervit,. 
-000026e0: 2074 6974 6c65 3d7b 4661 7374 6572 5669   title={FasterVi
-000026f0: 543a 2046 6173 7420 5669 7369 6f6e 2054  T: Fast Vision T
-00002700: 7261 6e73 666f 726d 6572 7320 7769 7468  ransformers with
-00002710: 2048 6965 7261 7263 6869 6361 6c20 4174   Hierarchical At
-00002720: 7465 6e74 696f 6e7d 2c0a 2020 6175 7468  tention},.  auth
-00002730: 6f72 3d7b 4861 7461 6d69 7a61 6465 682c  or={Hatamizadeh,
-00002740: 2041 6c69 2061 6e64 2048 6569 6e72 6963   Ali and Heinric
-00002750: 682c 2047 7265 6720 616e 6420 5969 6e2c  h, Greg and Yin,
-00002760: 2048 6f6e 6778 7520 616e 6420 5461 6f2c   Hongxu and Tao,
-00002770: 2041 6e64 7265 7720 616e 6420 416c 7661   Andrew and Alva
-00002780: 7265 7a2c 204a 6f73 6520 4d20 616e 6420  rez, Jose M and 
-00002790: 4b61 7574 7a2c 204a 616e 2061 6e64 204d  Kautz, Jan and M
-000027a0: 6f6c 6368 616e 6f76 2c20 5061 766c 6f7d  olchanov, Pavlo}
-000027b0: 2c0a 2020 6a6f 7572 6e61 6c3d 7b61 7258  ,.  journal={arX
-000027c0: 6976 2070 7265 7072 696e 7420 6172 5869  iv preprint arXi
-000027d0: 763a 3233 3036 2e30 3631 3839 7d2c 0a20  v:2306.06189},. 
-000027e0: 2079 6561 723d 7b32 3032 337d 0a7d 0a60   year={2023}.}.`
-000027f0: 6060 0a0a 0a23 2320 4c69 6365 6e73 6573  ``...## Licenses
-00002800: 0a0a 436f 7079 7269 6768 7420 c2a9 2032  ..Copyright .. 2
-00002810: 3032 332c 204e 5649 4449 4120 436f 7270  023, NVIDIA Corp
-00002820: 6f72 6174 696f 6e2e 2041 6c6c 2072 6967  oration. All rig
-00002830: 6874 7320 7265 7365 7276 6564 2e0a 0a54  hts reserved...T
-00002840: 6869 7320 776f 726b 2069 7320 6d61 6465  his work is made
-00002850: 2061 7661 696c 6162 6c65 2075 6e64 6572   available under
-00002860: 2074 6865 204e 5649 4449 4120 536f 7572   the NVIDIA Sour
-00002870: 6365 2043 6f64 6520 4c69 6365 6e73 652d  ce Code License-
-00002880: 4e43 2e20 436c 6963 6b20 5b68 6572 655d  NC. Click [here]
-00002890: 284c 4943 454e 5345 2920 746f 2076 6965  (LICENSE) to vie
-000028a0: 7720 6120 636f 7079 206f 6620 7468 6973  w a copy of this
-000028b0: 206c 6963 656e 7365 2e0a 0a46 6f72 206c   license...For l
-000028c0: 6963 656e 7365 2069 6e66 6f72 6d61 7469  icense informati
-000028d0: 6f6e 2072 6567 6172 6469 6e67 2074 6865  on regarding the
-000028e0: 2074 696d 6d20 7265 706f 7369 746f 7279   timm repository
-000028f0: 2c20 706c 6561 7365 2072 6566 6572 2074  , please refer t
-00002900: 6f20 6974 7320 5b72 6570 6f73 6974 6f72  o its [repositor
-00002910: 795d 2868 7474 7073 3a2f 2f67 6974 6875  y](https://githu
-00002920: 622e 636f 6d2f 7277 6967 6874 6d61 6e2f  b.com/rwightman/
-00002930: 7079 746f 7263 682d 696d 6167 652d 6d6f  pytorch-image-mo
-00002940: 6465 6c73 292e 0a0a 466f 7220 6c69 6365  dels)...For lice
-00002950: 6e73 6520 696e 666f 726d 6174 696f 6e20  nse information 
-00002960: 7265 6761 7264 696e 6720 7468 6520 496d  regarding the Im
-00002970: 6167 654e 6574 2064 6174 6173 6574 2c20  ageNet dataset, 
-00002980: 706c 6561 7365 2073 6565 2074 6865 205b  please see the [
-00002990: 496d 6167 654e 6574 206f 6666 6963 6961  ImageNet officia
-000029a0: 6c20 7765 6273 6974 655d 2868 7474 7073  l website](https
-000029b0: 3a2f 2f77 7777 2e69 6d61 6765 2d6e 6574  ://www.image-net
-000029c0: 2e6f 7267 2f29 2e20 0a0a 2323 2041 636b  .org/). ..## Ack
-000029d0: 6e6f 776c 6564 6765 6d65 6e74 0a54 6869  nowledgement.Thi
-000029e0: 7320 7265 706f 7369 746f 7279 2069 7320  s repository is 
-000029f0: 6275 696c 7420 6f6e 2074 6f70 206f 6620  built on top of 
-00002a00: 7468 6520 5b74 696d 6d5d 2868 7474 7073  the [timm](https
-00002a10: 3a2f 2f67 6974 6875 622e 636f 6d2f 6875  ://github.com/hu
-00002a20: 6767 696e 6766 6163 652f 7079 746f 7263  ggingface/pytorc
-00002a30: 682d 696d 6167 652d 6d6f 6465 6c73 2920  h-image-models) 
-00002a40: 7265 706f 7369 746f 7279 2e20 5765 2074  repository. We t
-00002a50: 6861 6e6b 205b 526f 7373 2057 7269 6768  hank [Ross Wrigh
-00002a60: 746d 616e 5d28 6874 7470 733a 2f2f 7277  tman](https://rw
-00002a70: 6967 6874 6d61 6e2e 636f 6d2f 2920 666f  ightman.com/) fo
-00002a80: 7220 6372 6561 7469 6e67 2061 6e64 206d  r creating and m
-00002a90: 6169 6e74 6169 6e69 6e67 2074 6869 7320  aintaining this 
-00002aa0: 6869 6768 2d71 7561 6c69 7479 206c 6962  high-quality lib
-00002ab0: 7261 7279 2e20 200a 0a                   rary.  ..
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6661 7374  : 2.1.Name: fast
+00000020: 6572 7669 740a 5665 7273 696f 6e3a 2030  ervit.Version: 0
+00000030: 2e39 2e32 0a53 756d 6d61 7279 3a20 4661  .9.2.Summary: Fa
+00000040: 7374 6572 5669 543a 2046 6173 7420 5669  sterViT: Fast Vi
+00000050: 7369 6f6e 2054 7261 6e73 666f 726d 6572  sion Transformer
+00000060: 7320 7769 7468 2048 6965 7261 7263 6869  s with Hierarchi
+00000070: 6361 6c20 4174 7465 6e74 696f 6e0a 486f  cal Attention.Ho
+00000080: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
+00000090: 2f67 6974 6875 622e 636f 6d2f 4e56 6c61  /github.com/NVla
+000000a0: 6273 2f46 6173 7465 7256 6954 0a41 7574  bs/FasterViT.Aut
+000000b0: 686f 723a 2041 6c69 2048 6174 616d 697a  hor: Ali Hatamiz
+000000c0: 6164 6568 0a41 7574 686f 722d 656d 6169  adeh.Author-emai
+000000d0: 6c3a 2061 6861 7461 6d69 7a31 3233 4067  l: ahatamiz123@g
+000000e0: 6d61 696c 2e63 6f6d 0a4c 6963 656e 7365  mail.com.License
+000000f0: 3a20 4e56 4944 4941 2053 6f75 7263 6520  : NVIDIA Source 
+00000100: 436f 6465 204c 6963 656e 7365 2d4e 430a  Code License-NC.
+00000110: 4b65 7977 6f72 6473 3a20 7079 746f 7263  Keywords: pytorc
+00000120: 6820 7072 6574 7261 696e 6564 206d 6f64  h pretrained mod
+00000130: 656c 7320 6566 6669 6369 656e 746e 6574  els efficientnet
+00000140: 206d 6f62 696c 656e 6574 7633 206d 6e61   mobilenetv3 mna
+00000150: 736e 6574 2072 6573 6e65 7420 7669 7369  snet resnet visi
+00000160: 6f6e 2074 7261 6e73 666f 726d 6572 2076  on transformer v
+00000170: 6974 0a43 6c61 7373 6966 6965 723a 2050  it.Classifier: P
+00000180: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000190: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000001a0: 2033 2e37 0a43 6c61 7373 6966 6965 723a   3.7.Classifier:
+000001b0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+000001c0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+000001d0: 3a3a 2033 2e38 0a43 6c61 7373 6966 6965  :: 3.8.Classifie
+000001e0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+000001f0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000200: 6e20 3a3a 2033 2e39 0a43 6c61 7373 6966  n :: 3.9.Classif
+00000210: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00000220: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000230: 686f 6e20 3a3a 2033 2e31 300a 436c 6173  hon :: 3.10.Clas
+00000240: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+00000250: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000260: 5079 7468 6f6e 203a 3a20 332e 3131 0a43  Python :: 3.11.C
+00000270: 6c61 7373 6966 6965 723a 2054 6f70 6963  lassifier: Topic
+00000280: 203a 3a20 5363 6965 6e74 6966 6963 2f45   :: Scientific/E
+00000290: 6e67 696e 6565 7269 6e67 203a 3a20 4172  ngineering :: Ar
+000002a0: 7469 6669 6369 616c 2049 6e74 656c 6c69  tificial Intelli
+000002b0: 6765 6e63 650a 436c 6173 7369 6669 6572  gence.Classifier
+000002c0: 3a20 546f 7069 6320 3a3a 2053 6f66 7477  : Topic :: Softw
+000002d0: 6172 6520 4465 7665 6c6f 706d 656e 740a  are Development.
+000002e0: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
+000002f0: 6320 3a3a 2053 6f66 7477 6172 6520 4465  c :: Software De
+00000300: 7665 6c6f 706d 656e 7420 3a3a 204c 6962  velopment :: Lib
+00000310: 7261 7269 6573 0a43 6c61 7373 6966 6965  raries.Classifie
+00000320: 723a 2054 6f70 6963 203a 3a20 536f 6674  r: Topic :: Soft
+00000330: 7761 7265 2044 6576 656c 6f70 6d65 6e74  ware Development
+00000340: 203a 3a20 4c69 6272 6172 6965 7320 3a3a   :: Libraries ::
+00000350: 2050 7974 686f 6e20 4d6f 6475 6c65 730a   Python Modules.
+00000360: 5265 7175 6972 6573 2d50 7974 686f 6e3a  Requires-Python:
+00000370: 203e 3d33 2e37 0a44 6573 6372 6970 7469   >=3.7.Descripti
+00000380: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
+00000390: 2074 6578 742f 6d61 726b 646f 776e 0a4c   text/markdown.L
+000003a0: 6963 656e 7365 2d46 696c 653a 204c 4943  icense-File: LIC
+000003b0: 454e 5345 0a0a 2320 4661 7374 6572 5669  ENSE..# FasterVi
+000003c0: 543a 2046 6173 7420 5669 7369 6f6e 2054  T: Fast Vision T
+000003d0: 7261 6e73 666f 726d 6572 7320 7769 7468  ransformers with
+000003e0: 2048 6965 7261 7263 6869 6361 6c20 4174   Hierarchical At
+000003f0: 7465 6e74 696f 6e0a 0a4f 6666 6963 6961  tention..Officia
+00000400: 6c20 5079 546f 7263 6820 696d 706c 656d  l PyTorch implem
+00000410: 656e 7461 7469 6f6e 206f 6620 5b2a 2a46  entation of [**F
+00000420: 6173 7465 7256 6954 3a20 4661 7374 2056  asterViT: Fast V
+00000430: 6973 696f 6e20 5472 616e 7366 6f72 6d65  ision Transforme
+00000440: 7273 2077 6974 6820 4869 6572 6172 6368  rs with Hierarch
+00000450: 6963 616c 2041 7474 656e 7469 6f6e 2a2a  ical Attention**
+00000460: 5d28 6874 7470 733a 2f2f 6172 7869 762e  ](https://arxiv.
+00000470: 6f72 672f 6162 732f 3233 3036 2e30 3631  org/abs/2306.061
+00000480: 3839 292e 0a0a 5b41 6c69 2048 6174 616d  89)...[Ali Hatam
+00000490: 697a 6164 6568 5d28 6874 7470 733a 2f2f  izadeh](https://
+000004a0: 7265 7365 6172 6368 2e6e 7669 6469 612e  research.nvidia.
+000004b0: 636f 6d2f 7065 7273 6f6e 2f61 6c69 2d68  com/person/ali-h
+000004c0: 6174 616d 697a 6164 6568 292c 0a5b 4772  atamizadeh),.[Gr
+000004d0: 6567 2048 6569 6e72 6963 685d 2868 7474  eg Heinrich](htt
+000004e0: 7073 3a2f 2f64 6576 656c 6f70 6572 2e6e  ps://developer.n
+000004f0: 7669 6469 612e 636f 6d2f 626c 6f67 2f61  vidia.com/blog/a
+00000500: 7574 686f 722f 6768 6569 6e72 6963 682f  uthor/gheinrich/
+00000510: 292c 0a5b 486f 6e67 7875 2028 4461 6e6e  ),.[Hongxu (Dann
+00000520: 7929 2059 696e 5d28 6874 7470 733a 2f2f  y) Yin](https://
+00000530: 7363 686f 6c61 722e 7072 696e 6365 746f  scholar.princeto
+00000540: 6e2e 6564 752f 686f 6e67 7875 292c 0a5b  n.edu/hongxu),.[
+00000550: 416e 6472 6577 2054 616f 5d28 6874 7470  Andrew Tao](http
+00000560: 733a 2f2f 6465 7665 6c6f 7065 722e 6e76  s://developer.nv
+00000570: 6964 6961 2e63 6f6d 2f62 6c6f 672f 6175  idia.com/blog/au
+00000580: 7468 6f72 2f61 7461 6f2f 292c 0a5b 4a6f  thor/atao/),.[Jo
+00000590: 7365 204d 2e20 416c 7661 7265 7a5d 2868  se M. Alvarez](h
+000005a0: 7474 7073 3a2f 2f61 6c76 6172 657a 6c6f  ttps://alvarezlo
+000005b0: 7065 7a6a 6f73 656d 2e67 6974 6875 622e  pezjosem.github.
+000005c0: 696f 2f29 2c0a 5b4a 616e 204b 6175 747a  io/),.[Jan Kautz
+000005d0: 5d28 6874 7470 733a 2f2f 6a61 6e6b 6175  ](https://jankau
+000005e0: 747a 2e63 6f6d 2f29 2c20 0a5b 5061 766c  tz.com/), .[Pavl
+000005f0: 6f20 4d6f 6c63 6861 6e6f 765d 2868 7474  o Molchanov](htt
+00000600: 7073 3a2f 2f77 7777 2e70 6d6f 6c63 6861  ps://www.pmolcha
+00000610: 6e6f 762e 636f 6d2f 292e 0a0a 466f 7220  nov.com/)...For 
+00000620: 6275 7369 6e65 7373 2069 6e71 7569 7269  business inquiri
+00000630: 6573 2c20 706c 6561 7365 2076 6973 6974  es, please visit
+00000640: 206f 7572 2077 6562 7369 7465 2061 6e64   our website and
+00000650: 2073 7562 6d69 7420 7468 6520 666f 726d   submit the form
+00000660: 3a20 5b4e 5649 4449 4120 5265 7365 6172  : [NVIDIA Resear
+00000670: 6368 204c 6963 656e 7369 6e67 5d28 6874  ch Licensing](ht
+00000680: 7470 733a 2f2f 7777 772e 6e76 6964 6961  tps://www.nvidia
+00000690: 2e63 6f6d 2f65 6e2d 7573 2f72 6573 6561  .com/en-us/resea
+000006a0: 7263 682f 696e 7175 6972 6965 732f 290a  rch/inquiries/).
+000006b0: 0a0a 2d2d 2d20 0a0a 4661 7374 6572 5669  ..--- ..FasterVi
+000006c0: 5420 6163 6869 6576 6573 2061 206e 6577  T achieves a new
+000006d0: 2053 4f54 4120 5061 7265 746f 2d66 726f   SOTA Pareto-fro
+000006e0: 6e74 2069 6e0a 7465 726d 7320 6f66 2061  nt in.terms of a
+000006f0: 6363 7572 6163 7920 7673 2e20 696d 6167  ccuracy vs. imag
+00000700: 6520 7468 726f 7567 6870 7574 2077 6974  e throughput wit
+00000710: 686f 7574 2065 7874 7261 2074 7261 696e  hout extra train
+00000720: 696e 6720 6461 7461 2021 0a0a 3c70 2061  ing data !..<p a
+00000730: 6c69 676e 3d22 6365 6e74 6572 223e 0a3c  lign="center">.<
+00000740: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00000750: 2f67 6974 6875 622e 636f 6d2f 4e56 6c61  /github.com/NVla
+00000760: 6273 2f46 6173 7465 7256 6954 2f61 7373  bs/FasterViT/ass
+00000770: 6574 732f 3236 3830 3633 3934 2f32 3533  ets/26806394/253
+00000780: 6431 6132 652d 6235 6635 2d34 6139 622d  d1a2e-b5f5-4a9b-
+00000790: 6133 3632 2d36 6364 6431 3662 6663 6363  a362-6cdd16bfccc
+000007a0: 3122 2077 6964 7468 3d36 3225 2068 6569  1" width=62% hei
+000007b0: 6768 743d 3632 2520 0a63 6c61 7373 3d22  ght=62% .class="
+000007c0: 6365 6e74 6572 223e 0a3c 2f70 3e0a 0a0a  center">.</p>...
+000007d0: 2323 2051 7569 636b 2053 7461 7274 0a0a  ## Quick Start..
+000007e0: 5765 2063 616e 2069 6d70 6f72 7420 7072  We can import pr
+000007f0: 652d 7472 6169 6e65 6420 4661 7374 6572  e-trained Faster
+00000800: 5669 5420 6d6f 6465 6c73 2077 6974 6820  ViT models with 
+00000810: 2a2a 3120 6c69 6e65 206f 6620 636f 6465  **1 line of code
+00000820: 2a2a 2e20 4669 7273 742c 2046 6173 7465  **. First, Faste
+00000830: 7256 6954 2063 616e 2062 6520 7369 6d70  rViT can be simp
+00000840: 6c79 2069 6e73 7461 6c6c 6564 2062 793a  ly installed by:
+00000850: 0a0a 6060 6062 6173 680a 7069 7020 696e  ..```bash.pip in
+00000860: 7374 616c 6c20 6661 7374 6572 7669 740a  stall fastervit.
+00000870: 6060 600a 0a41 2070 7265 7472 6169 6e65  ```..A pretraine
+00000880: 6420 4661 7374 6572 5669 5420 6d6f 6465  d FasterViT mode
+00000890: 6c20 7769 7468 2064 6566 6175 6c74 2068  l with default h
+000008a0: 7970 6572 2d70 6172 616d 6574 6572 7320  yper-parameters 
+000008b0: 6361 6e20 6265 2063 7265 6174 6564 2061  can be created a
+000008c0: 7320 696e 2074 6865 2066 6f6c 6c6f 7769  s in the followi
+000008d0: 6e67 3a0a 0a60 6060 7079 7468 6f6e 0a3e  ng:..```python.>
+000008e0: 3e3e 2066 726f 6d20 6661 7374 6572 7669  >> from fastervi
+000008f0: 7420 696d 706f 7274 2063 7265 6174 655f  t import create_
+00000900: 6d6f 6465 6c0a 0a23 2044 6566 696e 6520  model..# Define 
+00000910: 6661 7374 6572 7669 742d 3020 6d6f 6465  fastervit-0 mode
+00000920: 6c20 7769 7468 2032 3234 2078 2032 3234  l with 224 x 224
+00000930: 2072 6573 6f6c 7574 696f 6e0a 0a3e 3e3e   resolution..>>>
+00000940: 206d 6f64 656c 203d 2063 7265 6174 655f   model = create_
+00000950: 6d6f 6465 6c28 2766 6173 7465 725f 7669  model('faster_vi
+00000960: 745f 305f 3232 3427 2c20 0a20 2020 2020  t_0_224', .     
+00000970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000980: 2020 2020 2070 7265 7472 6169 6e65 643d       pretrained=
+00000990: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+000009a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009b0: 6d6f 6465 6c5f 7061 7468 3d22 2f74 6d70  model_path="/tmp
+000009c0: 2f66 6173 7465 725f 7669 745f 302e 7074  /faster_vit_0.pt
+000009d0: 682e 7461 7222 290a 6060 600a 0a60 6d6f  h.tar").```..`mo
+000009e0: 6465 6c5f 7061 7468 6020 6973 2075 7365  del_path` is use
+000009f0: 6420 746f 2073 6574 2074 6865 2064 6972  d to set the dir
+00000a00: 6563 746f 7279 2074 6f20 646f 776e 6c6f  ectory to downlo
+00000a10: 6164 2074 6865 206d 6f64 656c 2e0a 0a57  ad the model...W
+00000a20: 6520 6361 6e20 616c 736f 2073 696d 706c  e can also simpl
+00000a30: 7920 7465 7374 2074 6865 206d 6f64 656c  y test the model
+00000a40: 2062 7920 7061 7373 696e 6720 6120 6475   by passing a du
+00000a50: 6d6d 7920 696e 7075 7420 696d 6167 652e  mmy input image.
+00000a60: 2054 6865 206f 7574 7075 7420 6973 2074   The output is t
+00000a70: 6865 206c 6f67 6974 733a 0a0a 6060 6070  he logits:..```p
+00000a80: 7974 686f 6e0a 3e3e 3e20 696d 706f 7274  ython.>>> import
+00000a90: 2074 6f72 6368 0a0a 3e3e 3e20 696d 6167   torch..>>> imag
+00000aa0: 6520 3d20 746f 7263 682e 7261 6e64 2831  e = torch.rand(1
+00000ab0: 2c20 332c 2032 3234 2c20 3232 3429 0a3e  , 3, 224, 224).>
+00000ac0: 3e3e 206f 7574 7075 7420 3d20 6d6f 6465  >> output = mode
+00000ad0: 6c28 696d 6167 6529 2023 2074 6f72 6368  l(image) # torch
+00000ae0: 2e53 697a 6528 5b31 2c20 3130 3030 5d29  .Size([1, 1000])
+00000af0: 0a60 6060 0a0a 5765 2063 616e 2061 6c73  .```..We can als
+00000b00: 6f20 7573 6520 7468 6520 616e 792d 7265  o use the any-re
+00000b10: 736f 6c75 7469 6f6e 2046 6173 7465 7256  solution FasterV
+00000b20: 6954 206d 6f64 656c 2074 6f20 6163 636f  iT model to acco
+00000b30: 6d6d 6f64 6174 6520 6172 6269 7472 6172  mmodate arbitrar
+00000b40: 7920 696d 6167 6520 7265 736f 6c75 7469  y image resoluti
+00000b50: 6f6e 732e 2049 6e20 7468 6520 666f 6c6c  ons. In the foll
+00000b60: 6f77 696e 672c 2077 6520 6465 6669 6e65  owing, we define
+00000b70: 2061 6e20 616e 792d 7265 736f 6c75 7469   an any-resoluti
+00000b80: 6f6e 2046 6173 7465 7256 6954 2d30 0a6d  on FasterViT-0.m
+00000b90: 6f64 656c 2077 6974 6820 696e 7075 7420  odel with input 
+00000ba0: 7265 736f 6c75 7469 6f6e 206f 6620 3537  resolution of 57
+00000bb0: 3620 7820 3936 302c 2077 696e 646f 7720  6 x 960, window 
+00000bc0: 7369 7a65 7320 6f66 2031 3220 616e 6420  sizes of 12 and 
+00000bd0: 3620 696e 2033 7264 2061 6e64 2034 7468  6 in 3rd and 4th
+00000be0: 2073 7461 6765 732c 2063 6172 7269 6572   stages, carrier
+00000bf0: 2074 6f6b 656e 2073 697a 6520 6f66 2032   token size of 2
+00000c00: 2061 6e64 2065 6d62 6564 6469 6e67 2064   and embedding d
+00000c10: 696d 656e 7369 6f6e 206f 660a 3634 3a0a  imension of.64:.
+00000c20: 0a60 6060 7079 7468 6f6e 0a3e 3e3e 2066  .```python.>>> f
+00000c30: 726f 6d20 6661 7374 6572 7669 7420 696d  rom fastervit im
+00000c40: 706f 7274 2063 7265 6174 655f 6d6f 6465  port create_mode
+00000c50: 6c0a 0a23 2044 6566 696e 6520 616e 792d  l..# Define any-
+00000c60: 7265 736f 6c75 7469 6f6e 2046 6173 7465  resolution Faste
+00000c70: 7256 6954 2d30 206d 6f64 656c 2077 6974  rViT-0 model wit
+00000c80: 6820 3537 3620 7820 3936 3020 7265 736f  h 576 x 960 reso
+00000c90: 6c75 7469 6f6e 0a3e 3e3e 206d 6f64 656c  lution.>>> model
+00000ca0: 203d 2063 7265 6174 655f 6d6f 6465 6c28   = create_model(
+00000cb0: 2766 6173 7465 725f 7669 745f 305f 616e  'faster_vit_0_an
+00000cc0: 795f 7265 7327 2c20 0a20 2020 2020 2020  y_res', .       
+00000cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ce0: 2020 2072 6573 6f6c 7574 696f 6e3d 5b35     resolution=[5
+00000cf0: 3736 2c20 3936 305d 2c0a 2020 2020 2020  76, 960],.      
+00000d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d10: 2020 2020 7769 6e64 6f77 5f73 697a 653d      window_size=
+00000d20: 5b37 2c20 372c 2031 322c 2036 5d2c 0a20  [7, 7, 12, 6],. 
+00000d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d40: 2020 2020 2020 2020 2063 745f 7369 7a65           ct_size
+00000d50: 3d32 2c0a 2020 2020 2020 2020 2020 2020  =2,.            
+00000d60: 2020 2020 2020 2020 2020 2020 2020 6469                di
+00000d70: 6d3d 3634 2c0a 2020 2020 2020 2020 2020  m=64,.          
+00000d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d90: 7072 6574 7261 696e 6564 3d54 7275 6529  pretrained=True)
+00000da0: 0a60 6060 0a4e 6f74 6520 7468 6174 2074  .```.Note that t
+00000db0: 6865 2061 626f 7665 206d 6f64 656c 2069  he above model i
+00000dc0: 7320 696e 7469 6c69 617a 6564 2066 726f  s intiliazed fro
+00000dd0: 6d20 7468 6520 6f72 6967 696e 616c 2049  m the original I
+00000de0: 6d61 6765 4e65 7420 7072 652d 7472 6169  mageNet pre-trai
+00000df0: 6e65 6420 4661 7374 6572 5669 5420 7769  ned FasterViT wi
+00000e00: 7468 206f 7269 6769 6e61 6c20 7265 736f  th original reso
+00000e10: 6c75 7469 6f6e 206f 6620 3232 3420 7820  lution of 224 x 
+00000e20: 3232 342e 2041 7320 6120 7265 7375 6c74  224. As a result
+00000e30: 2c20 6d69 7373 696e 6720 6b65 7973 2061  , missing keys a
+00000e40: 6e64 206d 6973 2d6d 6174 6368 6573 2063  nd mis-matches c
+00000e50: 6f75 6c64 2062 6520 6578 7065 6374 6564  ould be expected
+00000e60: 2073 696e 6365 2077 6520 6172 6520 6164   since we are ad
+00000e70: 6469 676e 206e 6577 206c 6179 6572 7320  dign new layers 
+00000e80: 2865 2e67 2e20 6164 6469 7469 6f6e 206f  (e.g. addition o
+00000e90: 6620 6e65 7720 6361 7272 6965 7220 746f  f new carrier to
+00000ea0: 6b65 6e73 2c20 6574 632e 2920 0a0a 5765  kens, etc.) ..We
+00000eb0: 2063 616e 2073 696d 706c 7920 7465 7374   can simply test
+00000ec0: 2074 6865 206d 6f64 656c 2062 7920 7061   the model by pa
+00000ed0: 7373 696e 6720 6120 6475 6d6d 7920 696e  ssing a dummy in
+00000ee0: 7075 7420 696d 6167 652e 2054 6865 206f  put image. The o
+00000ef0: 7574 7075 7420 6973 2074 6865 206c 6f67  utput is the log
+00000f00: 6974 733a 0a0a 6060 6070 7974 686f 6e0a  its:..```python.
+00000f10: 3e3e 3e20 696d 706f 7274 2074 6f72 6368  >>> import torch
+00000f20: 0a0a 3e3e 3e20 696d 6167 6520 3d20 746f  ..>>> image = to
+00000f30: 7263 682e 7261 6e64 2831 2c20 332c 2035  rch.rand(1, 3, 5
+00000f40: 3736 2c20 3936 3029 0a3e 3e3e 206f 7574  76, 960).>>> out
+00000f50: 7075 7420 3d20 6d6f 6465 6c28 696d 6167  put = model(imag
+00000f60: 6529 2023 2074 6f72 6368 2e53 697a 6528  e) # torch.Size(
+00000f70: 5b31 2c20 3130 3030 5d29 0a60 6060 0a0a  [1, 1000]).```..
+00000f80: 2d2d 2d20 0a0a 2323 2052 6573 756c 7473  --- ..## Results
+00000f90: 202b 2050 7265 7472 6169 6e65 6420 4d6f   + Pretrained Mo
+00000fa0: 6465 6c73 0a0a 2323 2320 496d 6167 654e  dels..### ImageN
+00000fb0: 6574 2d31 4b0a 2a2a 4661 7374 6572 5669  et-1K.**FasterVi
+00000fc0: 5420 496d 6167 654e 6574 2d31 4b20 5072  T ImageNet-1K Pr
+00000fd0: 6574 7261 696e 6564 204d 6f64 656c 732a  etrained Models*
+00000fe0: 2a0a 0a3c 7461 626c 653e 0a20 203c 7472  *..<table>.  <tr
+00000ff0: 3e0a 2020 2020 3c74 683e 4e61 6d65 3c2f  >.    <th>Name</
+00001000: 7468 3e0a 2020 2020 3c74 683e 4163 6340  th>.    <th>Acc@
+00001010: 3128 2529 3c2f 7468 3e0a 2020 2020 3c74  1(%)</th>.    <t
+00001020: 683e 4163 6340 3528 2529 3c2f 7468 3e0a  h>Acc@5(%)</th>.
+00001030: 2020 2020 3c74 683e 5468 726f 7567 6870      <th>Throughp
+00001040: 7574 2849 6d67 2f53 6563 293c 2f74 683e  ut(Img/Sec)</th>
+00001050: 0a20 2020 203c 7468 3e52 6573 6f6c 7574  .    <th>Resolut
+00001060: 696f 6e3c 2f74 683e 0a20 2020 203c 7468  ion</th>.    <th
+00001070: 3e23 5061 7261 6d73 284d 293c 2f74 683e  >#Params(M)</th>
+00001080: 0a20 2020 203c 7468 3e46 4c4f 5073 2847  .    <th>FLOPs(G
+00001090: 293c 2f74 683e 0a20 2020 203c 7468 3e44  )</th>.    <th>D
+000010a0: 6f77 6e6c 6f61 643c 2f74 683e 0a20 203c  ownload</th>.  <
+000010b0: 2f74 723e 0a0a 3c74 723e 0a20 2020 203c  /tr>..<tr>.    <
+000010c0: 7464 3e46 6173 7465 7256 6954 2d30 3c2f  td>FasterViT-0</
+000010d0: 7464 3e0a 2020 2020 3c74 643e 3832 2e31  td>.    <td>82.1
+000010e0: 3c2f 7464 3e0a 2020 2020 3c74 643e 3935  </td>.    <td>95
+000010f0: 2e39 3c2f 7464 3e0a 2020 2020 3c74 643e  .9</td>.    <td>
+00001100: 3538 3032 3c2f 7464 3e0a 2020 2020 3c74  5802</td>.    <t
+00001110: 643e 3232 3478 3232 343c 2f74 643e 0a20  d>224x224</td>. 
+00001120: 2020 203c 7464 3e33 312e 343c 2f74 643e     <td>31.4</td>
+00001130: 0a20 2020 203c 7464 3e33 2e33 3c2f 7464  .    <td>3.3</td
+00001140: 3e0a 2020 2020 3c74 643e 3c61 2068 7265  >.    <td><a hre
+00001150: 663d 2268 7474 7073 3a2f 2f64 7269 7665  f="https://drive
+00001160: 2e67 6f6f 676c 652e 636f 6d2f 7563 3f65  .google.com/uc?e
+00001170: 7870 6f72 743d 646f 776e 6c6f 6164 2669  xport=download&i
+00001180: 643d 3174 7749 324c 464a 7333 3931 5972  d=1twI2LFJs391Yr
+00001190: 6a38 4d52 3455 6939 5066 7276 5771 6a45  j8MR4Ui9PfrvWqjE
+000011a0: 3169 4222 3e6d 6f64 656c 3c2f 613e 3c2f  1iB">model</a></
+000011b0: 7464 3e0a 3c2f 7472 3e0a 0a3c 7472 3e0a  td>.</tr>..<tr>.
+000011c0: 2020 2020 3c74 643e 4661 7374 6572 5669      <td>FasterVi
+000011d0: 542d 313c 2f74 643e 0a20 2020 203c 7464  T-1</td>.    <td
+000011e0: 3e38 332e 323c 2f74 643e 0a20 2020 203c  >83.2</td>.    <
+000011f0: 7464 3e39 362e 353c 2f74 643e 0a20 2020  td>96.5</td>.   
+00001200: 203c 7464 3e34 3138 383c 2f74 643e 0a20   <td>4188</td>. 
+00001210: 2020 203c 7464 3e32 3234 7832 3234 3c2f     <td>224x224</
+00001220: 7464 3e0a 2020 2020 3c74 643e 3533 2e34  td>.    <td>53.4
+00001230: 3c2f 7464 3e0a 2020 2020 3c74 643e 352e  </td>.    <td>5.
+00001240: 333c 2f74 643e 0a20 2020 203c 7464 3e3c  3</td>.    <td><
+00001250: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00001260: 6472 6976 652e 676f 6f67 6c65 2e63 6f6d  drive.google.com
+00001270: 2f75 633f 6578 706f 7274 3d64 6f77 6e6c  /uc?export=downl
+00001280: 6f61 6426 6964 3d31 7237 5731 306e 352d  oad&id=1r7W10n5-
+00001290: 6246 744d 3373 7a34 626d 614c 726f 774e  bFtM3sz4bmaLrowN
+000012a0: 3267 5950 6b4c 4754 223e 6d6f 6465 6c3c  2gYPkLGT">model<
+000012b0: 2f61 3e3c 2f74 643e 0a3c 2f74 723e 0a0a  /a></td>.</tr>..
+000012c0: 3c74 723e 0a20 2020 203c 7464 3e46 6173  <tr>.    <td>Fas
+000012d0: 7465 7256 6954 2d32 3c2f 7464 3e0a 2020  terViT-2</td>.  
+000012e0: 2020 3c74 643e 3834 2e32 3c2f 7464 3e0a    <td>84.2</td>.
+000012f0: 2020 2020 3c74 643e 3936 2e38 3c2f 7464      <td>96.8</td
+00001300: 3e0a 2020 2020 3c74 643e 3331 3631 3c2f  >.    <td>3161</
+00001310: 7464 3e0a 2020 2020 3c74 643e 3232 3478  td>.    <td>224x
+00001320: 3232 343c 2f74 643e 0a20 2020 203c 7464  224</td>.    <td
+00001330: 3e37 352e 393c 2f74 643e 0a20 2020 203c  >75.9</td>.    <
+00001340: 7464 3e38 2e37 3c2f 7464 3e0a 2020 2020  td>8.7</td>.    
+00001350: 3c74 643e 3c61 2068 7265 663d 2268 7474  <td><a href="htt
+00001360: 7073 3a2f 2f64 7269 7665 2e67 6f6f 676c  ps://drive.googl
+00001370: 652e 636f 6d2f 7563 3f65 7870 6f72 743d  e.com/uc?export=
+00001380: 646f 776e 6c6f 6164 2669 643d 316e 5f61  download&id=1n_a
+00001390: 3673 3070 6769 306a 565a 4f47 6d44 6569  6s0pgi0jVZOGmDei
+000013a0: 3276 5848 5535 4536 5248 3577 5522 3e6d  2vXHU5E6RH5wU">m
+000013b0: 6f64 656c 3c2f 613e 3c2f 7464 3e0a 3c2f  odel</a></td>.</
+000013c0: 7472 3e0a 0a3c 7472 3e0a 2020 2020 3c74  tr>..<tr>.    <t
+000013d0: 643e 4661 7374 6572 5669 542d 333c 2f74  d>FasterViT-3</t
+000013e0: 643e 0a20 2020 203c 7464 3e38 342e 393c  d>.    <td>84.9<
+000013f0: 2f74 643e 0a20 2020 203c 7464 3e39 372e  /td>.    <td>97.
+00001400: 323c 2f74 643e 0a20 2020 203c 7464 3e31  2</td>.    <td>1
+00001410: 3738 303c 2f74 643e 0a20 2020 203c 7464  780</td>.    <td
+00001420: 3e32 3234 7832 3234 3c2f 7464 3e0a 2020  >224x224</td>.  
+00001430: 2020 3c74 643e 3135 392e 353c 2f74 643e    <td>159.5</td>
+00001440: 0a20 2020 203c 7464 3e31 382e 323c 2f74  .    <td>18.2</t
+00001450: 643e 0a20 2020 203c 7464 3e3c 6120 6872  d>.    <td><a hr
+00001460: 6566 3d22 6874 7470 733a 2f2f 6472 6976  ef="https://driv
+00001470: 652e 676f 6f67 6c65 2e63 6f6d 2f75 633f  e.google.com/uc?
+00001480: 6578 706f 7274 3d64 6f77 6e6c 6f61 6426  export=download&
+00001490: 6964 3d31 7476 5745 6c5a 3931 5369 6132  id=1tvWElZ91Sia2
+000014a0: 5373 5859 5846 4d4e 5951 7766 6970 4378  SsXYXFMNYQwfipCx
+000014b0: 7449 3758 223e 6d6f 6465 6c3c 2f61 3e3c  tI7X">model</a><
+000014c0: 2f74 643e 0a3c 2f74 723e 0a0a 3c74 723e  /td>.</tr>..<tr>
+000014d0: 0a20 2020 203c 7464 3e46 6173 7465 7256  .    <td>FasterV
+000014e0: 6954 2d34 3c2f 7464 3e0a 2020 2020 3c74  iT-4</td>.    <t
+000014f0: 643e 3835 2e34 3c2f 7464 3e0a 2020 2020  d>85.4</td>.    
+00001500: 3c74 643e 3937 2e33 3c2f 7464 3e0a 2020  <td>97.3</td>.  
+00001510: 2020 3c74 643e 3834 393c 2f74 643e 0a20    <td>849</td>. 
+00001520: 2020 203c 7464 3e32 3234 7832 3234 3c2f     <td>224x224</
+00001530: 7464 3e0a 2020 2020 3c74 643e 3432 342e  td>.    <td>424.
+00001540: 363c 2f74 643e 0a20 2020 203c 7464 3e33  6</td>.    <td>3
+00001550: 362e 363c 2f74 643e 0a20 2020 203c 7464  6.6</td>.    <td
+00001560: 3e3c 6120 6872 6566 3d22 6874 7470 733a  ><a href="https:
+00001570: 2f2f 6472 6976 652e 676f 6f67 6c65 2e63  //drive.google.c
+00001580: 6f6d 2f75 633f 6578 706f 7274 3d64 6f77  om/uc?export=dow
+00001590: 6e6c 6f61 6426 6964 3d31 6759 6858 4133  nload&id=1gYhXA3
+000015a0: 3251 2d5f 3943 3544 5865 6c31 3761 7656  2Q-_9C5DXel17avV
+000015b0: 5f5a 4c6f 6148 7764 677a 223e 6d6f 6465  _ZLoaHwdgz">mode
+000015c0: 6c3c 2f61 3e3c 2f74 643e 0a3c 2f74 723e  l</a></td>.</tr>
+000015d0: 0a0a 3c74 723e 0a20 2020 203c 7464 3e46  ..<tr>.    <td>F
+000015e0: 6173 7465 7256 6954 2d35 3c2f 7464 3e0a  asterViT-5</td>.
+000015f0: 2020 2020 3c74 643e 3835 2e36 3c2f 7464      <td>85.6</td
+00001600: 3e0a 2020 2020 3c74 643e 3937 2e34 3c2f  >.    <td>97.4</
+00001610: 7464 3e0a 2020 2020 3c74 643e 3434 393c  td>.    <td>449<
+00001620: 2f74 643e 0a20 2020 203c 7464 3e32 3234  /td>.    <td>224
+00001630: 7832 3234 3c2f 7464 3e0a 2020 2020 3c74  x224</td>.    <t
+00001640: 643e 3937 352e 353c 2f74 643e 0a20 2020  d>975.5</td>.   
+00001650: 203c 7464 3e31 3133 2e30 3c2f 7464 3e0a   <td>113.0</td>.
+00001660: 2020 2020 3c74 643e 3c61 2068 7265 663d      <td><a href=
+00001670: 2268 7474 7073 3a2f 2f64 7269 7665 2e67  "https://drive.g
+00001680: 6f6f 676c 652e 636f 6d2f 7563 3f65 7870  oogle.com/uc?exp
+00001690: 6f72 743d 646f 776e 6c6f 6164 2669 643d  ort=download&id=
+000016a0: 316d 7170 6169 3758 6948 4c72 5f6e 3174  1mqpai7XiHLr_n1t
+000016b0: 6a78 6a7a 5438 7133 3639 7854 4371 5f7a  jxjzT8q369xTCq_z
+000016c0: 2d22 3e6d 6f64 656c 3c2f 613e 3c2f 7464  -">model</a></td
+000016d0: 3e0a 3c2f 7472 3e0a 0a3c 7472 3e0a 2020  >.</tr>..<tr>.  
+000016e0: 2020 3c74 643e 4661 7374 6572 5669 542d    <td>FasterViT-
+000016f0: 363c 2f74 643e 0a20 2020 203c 7464 3e38  6</td>.    <td>8
+00001700: 352e 383c 2f74 643e 0a20 2020 203c 7464  5.8</td>.    <td
+00001710: 3e39 372e 343c 2f74 643e 0a20 2020 203c  >97.4</td>.    <
+00001720: 7464 3e33 3532 3c2f 7464 3e0a 2020 2020  td>352</td>.    
+00001730: 3c74 643e 3232 3478 3232 343c 2f74 643e  <td>224x224</td>
+00001740: 0a20 2020 203c 7464 3e31 3336 302e 303c  .    <td>1360.0<
+00001750: 2f74 643e 0a20 2020 203c 7464 3e31 3432  /td>.    <td>142
+00001760: 2e30 3c2f 7464 3e0a 2020 2020 3c74 643e  .0</td>.    <td>
+00001770: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00001780: 2f64 7269 7665 2e67 6f6f 676c 652e 636f  /drive.google.co
+00001790: 6d2f 7563 3f65 7870 6f72 743d 646f 776e  m/uc?export=down
+000017a0: 6c6f 6164 2669 643d 3132 6a74 6176 5232  load&id=12jtavR2
+000017b0: 5178 6d4d 7a63 4b77 507a 5765 376b 772d  QxmMzcKwPzWe7kw-
+000017c0: 6f79 3334 4959 6935 3922 3e6d 6f64 656c  oy34IYi59">model
+000017d0: 3c2f 613e 3c2f 7464 3e0a 3c2f 7472 3e0a  </a></td>.</tr>.
+000017e0: 0a3c 2f74 6162 6c65 3e0a 0a0a 2323 2320  .</table>...### 
+000017f0: 526f 6275 7374 6e65 7373 2028 496d 6167  Robustness (Imag
+00001800: 654e 6574 2d41 202d 2049 6d61 6765 4e65  eNet-A - ImageNe
+00001810: 742d 5220 2d20 496d 6167 654e 6574 2d56  t-R - ImageNet-V
+00001820: 3229 0a0a 416c 6c20 6d6f 6465 6c73 2075  2)..All models u
+00001830: 7365 2060 6372 6f70 5f70 6374 3d30 2e38  se `crop_pct=0.8
+00001840: 3735 602e 2052 6573 756c 7473 2061 7265  75`. Results are
+00001850: 206f 6274 6169 6e65 6420 6279 2072 756e   obtained by run
+00001860: 6e69 6e67 2069 6e66 6572 656e 6365 206f  ning inference o
+00001870: 6e20 496d 6167 654e 6574 2d31 4b20 7072  n ImageNet-1K pr
+00001880: 6574 7261 696e 6564 206d 6f64 656c 7320  etrained models 
+00001890: 7769 7468 6f75 7420 6669 6e65 7475 6e69  without finetuni
+000018a0: 6e67 2e0a 3c74 6162 6c65 3e0a 2020 3c74  ng..<table>.  <t
+000018b0: 723e 0a20 2020 203c 7468 3e4e 616d 653c  r>.    <th>Name<
+000018c0: 2f74 683e 0a20 2020 203c 7468 3e41 2d41  /th>.    <th>A-A
+000018d0: 6363 4031 2825 293c 2f74 683e 0a20 2020  cc@1(%)</th>.   
+000018e0: 203c 7468 3e41 2d41 6363 4035 2825 293c   <th>A-Acc@5(%)<
+000018f0: 2f74 683e 0a20 2020 203c 7468 3e52 2d41  /th>.    <th>R-A
+00001900: 6363 4031 2825 293c 2f74 683e 0a20 2020  cc@1(%)</th>.   
+00001910: 203c 7468 3e52 2d41 6363 4035 2825 293c   <th>R-Acc@5(%)<
+00001920: 2f74 683e 0a20 2020 203c 7468 3e56 322d  /th>.    <th>V2-
+00001930: 4163 6340 3128 2529 3c2f 7468 3e0a 2020  Acc@1(%)</th>.  
+00001940: 2020 3c74 683e 5632 2d41 6363 4035 2825    <th>V2-Acc@5(%
+00001950: 293c 2f74 683e 0a20 203c 2f74 723e 0a0a  )</th>.  </tr>..
+00001960: 3c74 723e 0a20 2020 203c 7464 3e46 6173  <tr>.    <td>Fas
+00001970: 7465 7256 6954 2d30 3c2f 7464 3e0a 2020  terViT-0</td>.  
+00001980: 2020 3c74 643e 3233 2e39 3c2f 7464 3e0a    <td>23.9</td>.
+00001990: 2020 2020 3c74 643e 3537 2e36 3c2f 7464      <td>57.6</td
+000019a0: 3e0a 2020 2020 3c74 643e 3435 2e39 3c2f  >.    <td>45.9</
+000019b0: 7464 3e0a 2020 2020 3c74 643e 3630 2e34  td>.    <td>60.4
+000019c0: 3c2f 7464 3e0a 2020 2020 3c74 643e 3730  </td>.    <td>70
+000019d0: 2e39 3c2f 7464 3e0a 2020 2020 3c74 643e  .9</td>.    <td>
+000019e0: 3930 2e30 3c2f 7464 3e0a 3c2f 7472 3e0a  90.0</td>.</tr>.
+000019f0: 0a3c 7472 3e0a 2020 2020 3c74 643e 4661  .<tr>.    <td>Fa
+00001a00: 7374 6572 5669 542d 313c 2f74 643e 0a20  sterViT-1</td>. 
+00001a10: 2020 203c 7464 3e33 312e 323c 2f74 643e     <td>31.2</td>
+00001a20: 0a20 2020 203c 7464 3e36 332e 333c 2f74  .    <td>63.3</t
+00001a30: 643e 0a20 2020 203c 7464 3e34 372e 353c  d>.    <td>47.5<
+00001a40: 2f74 643e 0a20 2020 203c 7464 3e36 312e  /td>.    <td>61.
+00001a50: 393c 2f74 643e 0a20 2020 203c 7464 3e37  9</td>.    <td>7
+00001a60: 322e 363c 2f74 643e 0a20 2020 203c 7464  2.6</td>.    <td
+00001a70: 3e39 312e 303c 2f74 643e 0a3c 2f74 723e  >91.0</td>.</tr>
+00001a80: 0a0a 3c74 723e 0a20 2020 203c 7464 3e46  ..<tr>.    <td>F
+00001a90: 6173 7465 7256 6954 2d32 3c2f 7464 3e0a  asterViT-2</td>.
+00001aa0: 2020 2020 3c74 643e 3338 2e32 3c2f 7464      <td>38.2</td
+00001ab0: 3e0a 2020 2020 3c74 643e 3638 2e39 3c2f  >.    <td>68.9</
+00001ac0: 7464 3e0a 2020 2020 3c74 643e 3439 2e36  td>.    <td>49.6
+00001ad0: 3c2f 7464 3e0a 2020 2020 3c74 643e 3633  </td>.    <td>63
+00001ae0: 2e34 3c2f 7464 3e0a 2020 2020 3c74 643e  .4</td>.    <td>
+00001af0: 3733 2e37 3c2f 7464 3e0a 2020 2020 3c74  73.7</td>.    <t
+00001b00: 643e 3931 2e36 3c2f 7464 3e0a 3c2f 7472  d>91.6</td>.</tr
+00001b10: 3e0a 0a3c 7472 3e0a 2020 2020 3c74 643e  >..<tr>.    <td>
+00001b20: 4661 7374 6572 5669 542d 333c 2f74 643e  FasterViT-3</td>
+00001b30: 0a20 2020 203c 7464 3e34 342e 323c 2f74  .    <td>44.2</t
+00001b40: 643e 0a20 2020 203c 7464 3e37 332e 303c  d>.    <td>73.0<
+00001b50: 2f74 643e 0a20 2020 203c 7464 3e35 312e  /td>.    <td>51.
+00001b60: 393c 2f74 643e 0a20 2020 203c 7464 3e36  9</td>.    <td>6
+00001b70: 352e 363c 2f74 643e 0a20 2020 203c 7464  5.6</td>.    <td
+00001b80: 3e37 352e 303c 2f74 643e 0a20 2020 203c  >75.0</td>.    <
+00001b90: 7464 3e39 322e 323c 2f74 643e 0a3c 2f74  td>92.2</td>.</t
+00001ba0: 723e 0a0a 3c74 723e 0a20 2020 203c 7464  r>..<tr>.    <td
+00001bb0: 3e46 6173 7465 7256 6954 2d34 3c2f 7464  >FasterViT-4</td
+00001bc0: 3e0a 2020 2020 3c74 643e 3439 2e30 3c2f  >.    <td>49.0</
+00001bd0: 7464 3e0a 2020 2020 3c74 643e 3735 2e34  td>.    <td>75.4
+00001be0: 3c2f 7464 3e0a 2020 2020 3c74 643e 3536  </td>.    <td>56
+00001bf0: 2e30 3c2f 7464 3e0a 2020 2020 3c74 643e  .0</td>.    <td>
+00001c00: 3639 2e36 3c2f 7464 3e0a 2020 2020 3c74  69.6</td>.    <t
+00001c10: 643e 3735 2e37 3c2f 7464 3e0a 2020 2020  d>75.7</td>.    
+00001c20: 3c74 643e 3932 2e37 3c2f 7464 3e0a 3c2f  <td>92.7</td>.</
+00001c30: 7472 3e0a 0a3c 7472 3e0a 2020 2020 3c74  tr>..<tr>.    <t
+00001c40: 643e 4661 7374 6572 5669 542d 353c 2f74  d>FasterViT-5</t
+00001c50: 643e 0a20 2020 203c 7464 3e35 322e 373c  d>.    <td>52.7<
+00001c60: 2f74 643e 0a20 2020 203c 7464 3e37 372e  /td>.    <td>77.
+00001c70: 363c 2f74 643e 0a20 2020 203c 7464 3e35  6</td>.    <td>5
+00001c80: 362e 393c 2f74 643e 0a20 2020 203c 7464  6.9</td>.    <td
+00001c90: 3e37 302e 303c 2f74 643e 0a20 2020 203c  >70.0</td>.    <
+00001ca0: 7464 3e37 362e 303c 2f74 643e 0a20 2020  td>76.0</td>.   
+00001cb0: 203c 7464 3e39 332e 303c 2f74 643e 0a3c   <td>93.0</td>.<
+00001cc0: 2f74 723e 0a0a 3c74 723e 0a20 2020 203c  /tr>..<tr>.    <
+00001cd0: 7464 3e46 6173 7465 7256 6954 2d36 3c2f  td>FasterViT-6</
+00001ce0: 7464 3e0a 2020 2020 3c74 643e 3533 2e37  td>.    <td>53.7
+00001cf0: 3c2f 7464 3e0a 2020 2020 3c74 643e 3738  </td>.    <td>78
+00001d00: 2e34 3c2f 7464 3e0a 2020 2020 3c74 643e  .4</td>.    <td>
+00001d10: 3537 2e31 3c2f 7464 3e0a 2020 2020 3c74  57.1</td>.    <t
+00001d20: 643e 3730 2e31 3c2f 7464 3e0a 2020 2020  d>70.1</td>.    
+00001d30: 3c74 643e 3736 2e31 3c2f 7464 3e0a 2020  <td>76.1</td>.  
+00001d40: 2020 3c74 643e 3933 2e30 3c2f 7464 3e0a    <td>93.0</td>.
+00001d50: 3c2f 7472 3e0a 0a3c 2f74 6162 6c65 3e0a  </tr>..</table>.
+00001d60: 0a41 2c20 5220 616e 6420 5632 2064 656e  .A, R and V2 den
+00001d70: 6f74 6520 496d 6167 654e 6574 2d41 2c20  ote ImageNet-A, 
+00001d80: 496d 6167 654e 6574 2d52 2061 6e64 2049  ImageNet-R and I
+00001d90: 6d61 6765 4e65 742d 5632 2072 6573 7065  mageNet-V2 respe
+00001da0: 6374 6976 656c 792e 200a 2323 2054 7261  ctively. .## Tra
+00001db0: 696e 696e 670a 0a50 6c65 6173 6520 7365  ining..Please se
+00001dc0: 6520 5b54 5241 494e 494e 472e 6d64 5d28  e [TRAINING.md](
+00001dd0: 5452 4149 4e49 4e47 2e6d 6429 2066 6f72  TRAINING.md) for
+00001de0: 2064 6574 6169 6c65 6420 7472 6169 6e69   detailed traini
+00001df0: 6e67 2069 6e73 7472 7563 7469 6f6e 7320  ng instructions 
+00001e00: 6f66 2061 6c6c 206d 6f64 656c 732e 200a  of all models. .
+00001e10: 0a23 2320 4576 616c 7561 7469 6f6e 0a0a  .## Evaluation..
+00001e20: 5468 6520 4661 7374 6572 5669 5420 6d6f  The FasterViT mo
+00001e30: 6465 6c73 2063 616e 2062 6520 6576 616c  dels can be eval
+00001e40: 7561 7465 6420 6f6e 2049 6d61 6765 4e65  uated on ImageNe
+00001e50: 742d 314b 2076 616c 6964 6174 696f 6e20  t-1K validation 
+00001e60: 7365 7420 7573 696e 6720 7468 6520 666f  set using the fo
+00001e70: 6c6c 6f77 696e 673a 200a 0a60 6060 0a70  llowing: ..```.p
+00001e80: 7974 686f 6e20 7661 6c69 6461 7465 2e70  ython validate.p
+00001e90: 7920 5c0a 2d2d 6d6f 6465 6c20 3c6d 6f64  y \.--model <mod
+00001ea0: 656c 2d6e 616d 653e 0a2d 2d63 6865 636b  el-name>.--check
+00001eb0: 706f 696e 7420 3c63 6865 636b 706f 696e  point <checkpoin
+00001ec0: 742d 7061 7468 3e0a 2d2d 6461 7461 5f64  t-path>.--data_d
+00001ed0: 6972 203c 696d 6167 656e 6574 2d70 6174  ir <imagenet-pat
+00001ee0: 683e 0a2d 2d62 6174 6368 2d73 697a 6520  h>.--batch-size 
+00001ef0: 3c62 6174 6368 2d73 697a 652d 7065 722d  <batch-size-per-
+00001f00: 6770 750a 6060 6020 0a0a 4865 7265 2060  gpu.``` ..Here `
+00001f10: 2d2d 6d6f 6465 6c60 2069 7320 7468 6520  --model` is the 
+00001f20: 4661 7374 6572 5669 5420 7661 7269 616e  FasterViT varian
+00001f30: 7420 2865 2e67 2e20 6066 6173 7465 725f  t (e.g. `faster_
+00001f40: 7669 745f 305f 3232 345f 316b 6029 2c20  vit_0_224_1k`), 
+00001f50: 602d 2d63 6865 636b 706f 696e 7460 2069  `--checkpoint` i
+00001f60: 7320 7468 6520 7061 7468 2074 6f20 7072  s the path to pr
+00001f70: 6574 7261 696e 6564 206d 6f64 656c 2077  etrained model w
+00001f80: 6569 6768 7473 2c20 602d 2d64 6174 615f  eights, `--data_
+00001f90: 6469 7260 2069 7320 7468 6520 7061 7468  dir` is the path
+00001fa0: 2074 6f20 496d 6167 654e 6574 2d31 4b20   to ImageNet-1K 
+00001fb0: 7661 6c69 6461 7469 6f6e 2073 6574 2061  validation set a
+00001fc0: 6e64 2060 2d2d 6261 7463 682d 7369 7a65  nd `--batch-size
+00001fd0: 6020 6973 2074 6865 206e 756d 6265 7220  ` is the number 
+00001fe0: 6f66 2062 6174 6368 2073 697a 652e 2057  of batch size. W
+00001ff0: 6520 616c 736f 2070 726f 7669 6465 2061  e also provide a
+00002000: 2073 616d 706c 6520 7363 7269 7074 205b   sample script [
+00002010: 6865 7265 5d28 2e2f 6661 7374 6572 7669  here](./fastervi
+00002020: 742f 7661 6c69 6461 7465 2e73 6829 2e20  t/validate.sh). 
+00002030: 0a0a 2323 204f 4e4e 5820 436f 6e76 6572  ..## ONNX Conver
+00002040: 7369 6f6e 0a0a 5765 2070 726f 7669 6465  sion..We provide
+00002050: 204f 4e4e 5820 636f 6e76 6572 7369 6f6e   ONNX conversion
+00002060: 2073 6372 6970 7420 746f 2065 6e61 626c   script to enabl
+00002070: 6520 6479 6e61 6d69 6320 6261 7463 6820  e dynamic batch 
+00002080: 7369 7a65 2069 6e66 6572 656e 6365 2e20  size inference. 
+00002090: 466f 7220 696e 7374 616e 6365 2c20 746f  For instance, to
+000020a0: 2067 656e 6572 6174 6520 4f4e 4e58 206d   generate ONNX m
+000020b0: 6f64 656c 2066 6f72 2060 6661 7374 6572  odel for `faster
+000020c0: 5f76 6974 5f30 5f61 6e79 5f72 6573 6020  _vit_0_any_res` 
+000020d0: 7769 7468 2072 6573 6f6c 7574 696f 6e20  with resolution 
+000020e0: 3537 3620 7820 3936 3020 616e 6420 4f4e  576 x 960 and ON
+000020f0: 4e58 206f 7073 6574 206e 756d 6265 7220  NX opset number 
+00002100: 3137 2c20 7468 6520 666f 6c6c 6f77 696e  17, the followin
+00002110: 6720 6361 6e20 6265 2075 7365 642e 200a  g can be used. .
+00002120: 0a60 6060 6261 7368 200a 7079 7468 6f6e  .```bash .python
+00002130: 206f 6e6e 785f 636f 6e76 6572 7420 2d2d   onnx_convert --
+00002140: 6d6f 6465 6c2d 6e61 6d65 2066 6173 7465  model-name faste
+00002150: 725f 7669 745f 305f 616e 795f 7265 7320  r_vit_0_any_res 
+00002160: 2d2d 7265 736f 6c75 7469 6f6e 2d68 2035  --resolution-h 5
+00002170: 3736 202d 2d72 6573 6f6c 7574 696f 6e2d  76 --resolution-
+00002180: 7720 3936 3020 2d2d 6f6e 6e78 2d6f 7073  w 960 --onnx-ops
+00002190: 6574 2031 370a 0a60 6060 0a0a 0a23 2320  et 17..```...## 
+000021a0: 496e 7374 616c 6c61 7469 6f6e 0a0a 5468  Installation..Th
+000021b0: 6520 6465 7065 6e64 656e 6369 6573 2063  e dependencies c
+000021c0: 616e 2062 6520 696e 7374 616c 6c65 6420  an be installed 
+000021d0: 6279 2072 756e 6e69 6e67 3a0a 0a60 6060  by running:..```
+000021e0: 6261 7368 0a70 6970 2069 6e73 7461 6c6c  bash.pip install
+000021f0: 202d 7220 7265 7175 6972 656d 656e 7473   -r requirements
+00002200: 2e74 7874 0a60 6060 0a0a 2323 2053 7461  .txt.```..## Sta
+00002210: 7220 4869 7374 6f72 790a 0a5b 215b 5374  r History..[![St
+00002220: 6172 2048 6973 746f 7279 2043 6861 7274  ar History Chart
+00002230: 5d28 6874 7470 733a 2f2f 6170 692e 7374  ](https://api.st
+00002240: 6172 2d68 6973 746f 7279 2e63 6f6d 2f73  ar-history.com/s
+00002250: 7667 3f72 6570 6f73 3d4e 566c 6162 732f  vg?repos=NVlabs/
+00002260: 4661 7374 6572 5669 5426 7479 7065 3d44  FasterViT&type=D
+00002270: 6174 6529 5d28 6874 7470 733a 2f2f 7374  ate)](https://st
+00002280: 6172 2d68 6973 746f 7279 2e63 6f6d 2f23  ar-history.com/#
+00002290: 4e56 6c61 6273 2f46 6173 7465 7256 6954  NVlabs/FasterViT
+000022a0: 2644 6174 6529 0a0a 0a23 2320 5468 6972  &Date)...## Thir
+000022b0: 642d 7061 7274 7920 4578 7465 6e74 696f  d-party Extentio
+000022c0: 6e73 0a57 6520 616c 7761 7973 2077 656c  ns.We always wel
+000022d0: 636f 6d65 2074 6869 7264 2d70 6172 7479  come third-party
+000022e0: 2065 7874 656e 7469 6f6e 732f 696d 706c   extentions/impl
+000022f0: 656d 656e 7461 7469 6f6e 7320 616e 6420  ementations and 
+00002300: 7573 6167 6520 666f 7220 6f74 6865 7220  usage for other 
+00002310: 7075 7270 6f73 6573 2e20 4966 2079 6f75  purposes. If you
+00002320: 2077 6f75 6c64 206c 696b 6520 796f 7572   would like your
+00002330: 2077 6f72 6b20 746f 2062 6520 6c69 7374   work to be list
+00002340: 6564 2069 6e20 7468 6973 2072 6570 6f73  ed in this repos
+00002350: 6974 6f72 792c 2070 6c65 6173 6520 7261  itory, please ra
+00002360: 6973 6520 616e 6420 6973 7375 6520 616e  ise and issue an
+00002370: 6420 7072 6f76 6964 6520 7573 2077 6974  d provide us wit
+00002380: 6820 6465 7461 696c 6564 2069 6e66 6f72  h detailed infor
+00002390: 6d61 7469 6f6e 2e20 200a 0a23 2320 4369  mation.  ..## Ci
+000023a0: 7461 7469 6f6e 0a0a 506c 6561 7365 2063  tation..Please c
+000023b0: 6f6e 7369 6465 7220 6369 7469 6e67 2046  onsider citing F
+000023c0: 6173 7465 7256 6954 2069 6620 7468 6973  asterViT if this
+000023d0: 2072 6570 6f73 6974 6f72 7920 6973 2075   repository is u
+000023e0: 7365 6675 6c20 666f 7220 796f 7572 2077  seful for your w
+000023f0: 6f72 6b2e 200a 0a60 6060 0a40 6172 7469  ork. ..```.@arti
+00002400: 636c 657b 6861 7461 6d69 7a61 6465 6832  cle{hatamizadeh2
+00002410: 3032 3366 6173 7465 7276 6974 2c0a 2020  023fastervit,.  
+00002420: 7469 746c 653d 7b46 6173 7465 7256 6954  title={FasterViT
+00002430: 3a20 4661 7374 2056 6973 696f 6e20 5472  : Fast Vision Tr
+00002440: 616e 7366 6f72 6d65 7273 2077 6974 6820  ansformers with 
+00002450: 4869 6572 6172 6368 6963 616c 2041 7474  Hierarchical Att
+00002460: 656e 7469 6f6e 7d2c 0a20 2061 7574 686f  ention},.  autho
+00002470: 723d 7b48 6174 616d 697a 6164 6568 2c20  r={Hatamizadeh, 
+00002480: 416c 6920 616e 6420 4865 696e 7269 6368  Ali and Heinrich
+00002490: 2c20 4772 6567 2061 6e64 2059 696e 2c20  , Greg and Yin, 
+000024a0: 486f 6e67 7875 2061 6e64 2054 616f 2c20  Hongxu and Tao, 
+000024b0: 416e 6472 6577 2061 6e64 2041 6c76 6172  Andrew and Alvar
+000024c0: 657a 2c20 4a6f 7365 204d 2061 6e64 204b  ez, Jose M and K
+000024d0: 6175 747a 2c20 4a61 6e20 616e 6420 4d6f  autz, Jan and Mo
+000024e0: 6c63 6861 6e6f 762c 2050 6176 6c6f 7d2c  lchanov, Pavlo},
+000024f0: 0a20 206a 6f75 726e 616c 3d7b 6172 5869  .  journal={arXi
+00002500: 7620 7072 6570 7269 6e74 2061 7258 6976  v preprint arXiv
+00002510: 3a32 3330 362e 3036 3138 397d 2c0a 2020  :2306.06189},.  
+00002520: 7965 6172 3d7b 3230 3233 7d0a 7d0a 6060  year={2023}.}.``
+00002530: 600a 0a0a 2323 204c 6963 656e 7365 730a  `...## Licenses.
+00002540: 0a43 6f70 7972 6967 6874 20c2 a920 3230  .Copyright .. 20
+00002550: 3233 2c20 4e56 4944 4941 2043 6f72 706f  23, NVIDIA Corpo
+00002560: 7261 7469 6f6e 2e20 416c 6c20 7269 6768  ration. All righ
+00002570: 7473 2072 6573 6572 7665 642e 0a0a 5468  ts reserved...Th
+00002580: 6973 2077 6f72 6b20 6973 206d 6164 6520  is work is made 
+00002590: 6176 6169 6c61 626c 6520 756e 6465 7220  available under 
+000025a0: 7468 6520 4e56 4944 4941 2053 6f75 7263  the NVIDIA Sourc
+000025b0: 6520 436f 6465 204c 6963 656e 7365 2d4e  e Code License-N
+000025c0: 432e 2043 6c69 636b 205b 6865 7265 5d28  C. Click [here](
+000025d0: 4c49 4345 4e53 4529 2074 6f20 7669 6577  LICENSE) to view
+000025e0: 2061 2063 6f70 7920 6f66 2074 6869 7320   a copy of this 
+000025f0: 6c69 6365 6e73 652e 0a0a 466f 7220 6c69  license...For li
+00002600: 6365 6e73 6520 696e 666f 726d 6174 696f  cense informatio
+00002610: 6e20 7265 6761 7264 696e 6720 7468 6520  n regarding the 
+00002620: 7469 6d6d 2072 6570 6f73 6974 6f72 792c  timm repository,
+00002630: 2070 6c65 6173 6520 7265 6665 7220 746f   please refer to
+00002640: 2069 7473 205b 7265 706f 7369 746f 7279   its [repository
+00002650: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00002660: 2e63 6f6d 2f72 7769 6768 746d 616e 2f70  .com/rwightman/p
+00002670: 7974 6f72 6368 2d69 6d61 6765 2d6d 6f64  ytorch-image-mod
+00002680: 656c 7329 2e0a 0a46 6f72 206c 6963 656e  els)...For licen
+00002690: 7365 2069 6e66 6f72 6d61 7469 6f6e 2072  se information r
+000026a0: 6567 6172 6469 6e67 2074 6865 2049 6d61  egarding the Ima
+000026b0: 6765 4e65 7420 6461 7461 7365 742c 2070  geNet dataset, p
+000026c0: 6c65 6173 6520 7365 6520 7468 6520 5b49  lease see the [I
+000026d0: 6d61 6765 4e65 7420 6f66 6669 6369 616c  mageNet official
+000026e0: 2077 6562 7369 7465 5d28 6874 7470 733a   website](https:
+000026f0: 2f2f 7777 772e 696d 6167 652d 6e65 742e  //www.image-net.
+00002700: 6f72 672f 292e 200a 0a23 2320 4163 6b6e  org/). ..## Ackn
+00002710: 6f77 6c65 6467 656d 656e 740a 5468 6973  owledgement.This
+00002720: 2072 6570 6f73 6974 6f72 7920 6973 2062   repository is b
+00002730: 7569 6c74 206f 6e20 746f 7020 6f66 2074  uilt on top of t
+00002740: 6865 205b 7469 6d6d 5d28 6874 7470 733a  he [timm](https:
+00002750: 2f2f 6769 7468 7562 2e63 6f6d 2f68 7567  //github.com/hug
+00002760: 6769 6e67 6661 6365 2f70 7974 6f72 6368  gingface/pytorch
+00002770: 2d69 6d61 6765 2d6d 6f64 656c 7329 2072  -image-models) r
+00002780: 6570 6f73 6974 6f72 792e 2057 6520 7468  epository. We th
+00002790: 616e 6b20 5b52 6f73 7320 5772 6967 6874  ank [Ross Wright
+000027a0: 6d61 6e5d 2868 7474 7073 3a2f 2f72 7769  man](https://rwi
+000027b0: 6768 746d 616e 2e63 6f6d 2f29 2066 6f72  ghtman.com/) for
+000027c0: 2063 7265 6174 696e 6720 616e 6420 6d61   creating and ma
+000027d0: 696e 7461 696e 696e 6720 7468 6973 2068  intaining this h
+000027e0: 6967 682d 7175 616c 6974 7920 6c69 6272  igh-quality libr
+000027f0: 6172 792e 2020 0a0a                      ary.  ..
```

### Comparing `fastervit-0.9.1/fastervit/assets/hierarchial_attn.png` & `fastervit-0.9.2/fastervit/assets/hierarchial_attn.png`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.1/fastervit/models/faster_vit.py` & `fastervit-0.9.2/fastervit/models/faster_vit.py`

 * *Files 1% similar despite different names*

```diff
@@ -847,15 +847,15 @@
                  qkv_bias=True,
                  qk_scale=None,
                  drop_rate=0.,
                  attn_drop_rate=0.,
                  layer_scale=None,
                  layer_scale_conv=None,
                  layer_norm_last=False,
-                 hat=None,
+                 hat=[False, False, True, False],
                  do_propagation=False,
                  **kwargs):
         """
         Args:
             dim: feature size dimension.
             in_dim: inner-plane feature size dimension.
             depths: layer depth.
@@ -960,23 +960,25 @@
     ct_size = kwargs.pop("ct_size", 2)
     dim = kwargs.pop("dim", 64)
     in_dim = kwargs.pop("in_dim", 64)
     mlp_ratio = kwargs.pop("mlp_ratio", 4)
     resolution = kwargs.pop("resolution", 224)
     drop_path_rate = kwargs.pop("drop_path_rate", 0.2)
     model_path = kwargs.pop("model_path", "/tmp/faster_vit_0.pth.tar")
+    hat = kwargs.pop("hat", [False, False, True, False])
     model = FasterViT(depths=depths,
                       num_heads=num_heads,
                       window_size=window_size,
                       ct_size=ct_size,
                       dim=dim,
                       in_dim=in_dim,
                       mlp_ratio=mlp_ratio,
                       resolution=resolution,
                       drop_path_rate=drop_path_rate,
+                      hat=hat,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_0_224']
     if pretrained:
         if not Path(model_path).is_file():
             url = model.default_cfg['url']
             torch.hub.download_url_to_file(url=url, dst=model_path)
         model._load_state_dict(model_path)
@@ -992,23 +994,25 @@
     ct_size = kwargs.pop("ct_size", 2)
     dim = kwargs.pop("dim", 80)
     in_dim = kwargs.pop("in_dim", 32)
     mlp_ratio = kwargs.pop("mlp_ratio", 4)
     resolution = kwargs.pop("resolution", 224)
     drop_path_rate = kwargs.pop("drop_path_rate", 0.2)
     model_path = kwargs.pop("model_path", "/tmp/faster_vit_1.pth.tar")
+    hat = kwargs.pop("hat", [False, False, True, False])
     model = FasterViT(depths=depths,
                       num_heads=num_heads,
                       window_size=window_size,
                       ct_size=ct_size,
                       dim=dim,
                       in_dim=in_dim,
                       mlp_ratio=mlp_ratio,
                       resolution=resolution,
                       drop_path_rate=drop_path_rate,
+                      hat=hat,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_1_224']
     if pretrained:
         if not Path(model_path).is_file():
             url = model.default_cfg['url']
             torch.hub.download_url_to_file(url=url, dst=model_path)
         model._load_state_dict(model_path)
@@ -1024,23 +1028,25 @@
     ct_size = kwargs.pop("ct_size", 2)
     dim = kwargs.pop("dim", 96)
     in_dim = kwargs.pop("in_dim", 64)
     mlp_ratio = kwargs.pop("mlp_ratio", 4)
     resolution = kwargs.pop("resolution", 224)
     drop_path_rate = kwargs.pop("drop_path_rate", 0.2)
     model_path = kwargs.pop("model_path", "/tmp/faster_vit_2.pth.tar")
+    hat = kwargs.pop("hat", [False, False, True, False])
     model = FasterViT(depths=depths,
                       num_heads=num_heads,
                       window_size=window_size,
                       ct_size=ct_size,
                       dim=dim,
                       in_dim=in_dim,
                       mlp_ratio=mlp_ratio,
                       resolution=resolution,
                       drop_path_rate=drop_path_rate,
+                      hat=hat,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_2_224']
     if pretrained:
         if not Path(model_path).is_file():
             url = model.default_cfg['url']
             torch.hub.download_url_to_file(url=url, dst=model_path)
         model._load_state_dict(model_path)
@@ -1057,63 +1063,67 @@
     dim = kwargs.pop("dim", 128)
     in_dim = kwargs.pop("in_dim", 64)
     mlp_ratio = kwargs.pop("mlp_ratio", 4)
     resolution = kwargs.pop("resolution", 224)
     drop_path_rate = kwargs.pop("drop_path_rate", 0.3)
     layer_scale = kwargs.pop("layer_scale", 1e-5)
     model_path = kwargs.pop("model_path", "/tmp/faster_vit_3.pth.tar")
+    hat = kwargs.pop("hat", [False, False, True, False])
     model = FasterViT(depths=depths,
                       num_heads=num_heads,
                       window_size=window_size,
                       ct_size=ct_size,
                       dim=dim,
                       in_dim=in_dim,
                       mlp_ratio=mlp_ratio,
                       resolution=resolution,
                       drop_path_rate=drop_path_rate,
                       layer_scale=layer_scale,
                       layer_scale_conv=None,
                       do_propagation=True,
+                      hat=hat,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_3_224']
     if pretrained:
         if not Path(model_path).is_file():
             url = model.default_cfg['url']
             torch.hub.download_url_to_file(url=url, dst=model_path)
         model._load_state_dict(model_path)
     return model
 
 
 @register_pip_model
 @register_model
 def faster_vit_4_224(pretrained=False, **kwargs):
     depths = kwargs.pop("depths", [3, 3, 12, 5])
-    num_heads = kwargs.pop("num_heads", [2, 4, 8, 16])
+    num_heads = kwargs.pop("num_heads", [4, 8, 16, 32])
     window_size = kwargs.pop("window_size", [7, 7, 7, 7])
     ct_size = kwargs.pop("ct_size", 2)
     dim = kwargs.pop("dim", 196)
     in_dim = kwargs.pop("in_dim", 64)
     mlp_ratio = kwargs.pop("mlp_ratio", 4)
     resolution = kwargs.pop("resolution", 224)
     drop_path_rate = kwargs.pop("drop_path_rate", 0.3)
     layer_scale = kwargs.pop("layer_scale", 1e-5)
     model_path = kwargs.pop("model_path", "/tmp/faster_vit_4.pth.tar")
+    hat = kwargs.pop("hat", [False, False, True, False])
     model = FasterViT(depths=depths,
                       num_heads=num_heads,
                       window_size=window_size,
                       ct_size=ct_size,
                       dim=dim,
                       in_dim=in_dim,
                       mlp_ratio=mlp_ratio,
                       resolution=resolution,
                       drop_path_rate=drop_path_rate,
                       layer_scale=layer_scale,
                       layer_scale_conv=None,
                       layer_norm_last=False,
                       do_propagation=True,
+                      hat=hat,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_4_224']
     if pretrained:
         if not Path(model_path).is_file():
             url = model.default_cfg['url']
             torch.hub.download_url_to_file(url=url, dst=model_path)
         model._load_state_dict(model_path)
@@ -1130,27 +1140,29 @@
     dim = kwargs.pop("dim", 320)
     in_dim = kwargs.pop("in_dim", 64)
     mlp_ratio = kwargs.pop("mlp_ratio", 4)
     resolution = kwargs.pop("resolution", 224)
     drop_path_rate = kwargs.pop("drop_path_rate", 0.3)
     layer_scale = kwargs.pop("layer_scale", 1e-5)
     model_path = kwargs.pop("model_path", "/tmp/faster_vit_5.pth.tar")
+    hat = kwargs.pop("hat", [False, False, True, False])
     model = FasterViT(depths=depths,
                       num_heads=num_heads,
                       window_size=window_size,
                       ct_size=ct_size,
                       dim=dim,
                       in_dim=in_dim,
                       mlp_ratio=mlp_ratio,
                       resolution=resolution,
                       drop_path_rate=drop_path_rate,
                       layer_scale=layer_scale,
                       layer_scale_conv=None,
                       layer_norm_last=False,
                       do_propagation=True,
+                      hat=hat,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_5_224']
     if pretrained:
         if not Path(model_path).is_file():
             url = model.default_cfg['url']
             torch.hub.download_url_to_file(url=url, dst=model_path)
         model._load_state_dict(model_path)
@@ -1167,27 +1179,29 @@
     dim = kwargs.pop("dim", 320)
     in_dim = kwargs.pop("in_dim", 64)
     mlp_ratio = kwargs.pop("mlp_ratio", 4)
     resolution = kwargs.pop("resolution", 224)
     drop_path_rate = kwargs.pop("drop_path_rate", 0.5)
     layer_scale = kwargs.pop("layer_scale", 1e-5)
     model_path = kwargs.pop("model_path", "/tmp/faster_vit_6.pth.tar")
+    hat = kwargs.pop("hat", [False, False, True, False])
     model = FasterViT(depths=depths,
                       num_heads=num_heads,
                       window_size=window_size,
                       ct_size=ct_size,
                       dim=dim,
                       in_dim=in_dim,
                       mlp_ratio=mlp_ratio,
                       resolution=resolution,
                       drop_path_rate=drop_path_rate,
                       layer_scale=layer_scale,
                       layer_scale_conv=None,
                       layer_norm_last=False,
                       do_propagation=True,
+                      hat=hat,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_6_224']
     if pretrained:
         if not Path(model_path).is_file():
             url = model.default_cfg['url']
             torch.hub.download_url_to_file(url=url, dst=model_path)
         model._load_state_dict(model_path)
```

### Comparing `fastervit-0.9.1/fastervit/models/faster_vit_any_res.py` & `fastervit-0.9.2/fastervit/models/faster_vit_any_res.py`

 * *Files 2% similar despite different names*

```diff
@@ -862,26 +862,26 @@
                  dim,
                  in_dim,
                  depths,
                  window_size,
                  ct_size,
                  mlp_ratio,
                  num_heads,
-                 resolution=[224,224],
+                 resolution=[224, 224],
                  drop_path_rate=0.2,
                  in_chans=3,
                  num_classes=1000,
                  qkv_bias=True,
                  qk_scale=None,
                  drop_rate=0.,
                  attn_drop_rate=0.,
                  layer_scale=None,
                  layer_scale_conv=None,
                  layer_norm_last=False,
-                 hat=None,
+                 hat=[False, False, True, False],
                  do_propagation=False,
                  **kwargs):
         """
         Args:
             dim: feature size dimension.
             in_dim: inner-plane feature size dimension.
             depths: layer depth.
@@ -989,23 +989,25 @@
     ct_size = kwargs.pop("ct_size", 2)
     dim = kwargs.pop("dim", 64)
     in_dim = kwargs.pop("in_dim", 64)
     mlp_ratio = kwargs.pop("mlp_ratio", 4)
     resolution = kwargs.pop("resolution", [576, 960])
     drop_path_rate = kwargs.pop("drop_path_rate", 0.2)
     model_path = kwargs.pop("model_path", "/tmp/faster_vit_0.pth.tar")
+    hat = kwargs.pop("hat", [False, False, True, False])
     model = FasterViT(depths=depths,
                       num_heads=num_heads,
                       window_size=window_size,
                       ct_size=ct_size,
                       dim=dim,
                       in_dim=in_dim,
                       mlp_ratio=mlp_ratio,
                       resolution=resolution,
                       drop_path_rate=drop_path_rate,
+                      hat=hat,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_0_any_res']
     if pretrained:
         if not Path(model_path).is_file():
             url = model.default_cfg['url']
             torch.hub.download_url_to_file(url=url, dst=model_path)
         model._load_state_dict(model_path)
@@ -1021,23 +1023,25 @@
     ct_size = kwargs.pop("ct_size", 2)
     dim = kwargs.pop("dim", 80)
     in_dim = kwargs.pop("in_dim", 32)
     mlp_ratio = kwargs.pop("mlp_ratio", 4)
     resolution = kwargs.pop("resolution", [576, 960])
     drop_path_rate = kwargs.pop("drop_path_rate", 0.2)
     model_path = kwargs.pop("model_path", "/tmp/faster_vit_1.pth.tar")
+    hat = kwargs.pop("hat", [False, False, True, False])
     model = FasterViT(depths=depths,
                       num_heads=num_heads,
                       window_size=window_size,
                       ct_size=ct_size,
                       dim=dim,
                       in_dim=in_dim,
                       mlp_ratio=mlp_ratio,
                       resolution=resolution,
                       drop_path_rate=drop_path_rate,
+                      hat=hat,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_1_any_res']
     if pretrained:
         if not Path(model_path).is_file():
             url = model.default_cfg['url']
             torch.hub.download_url_to_file(url=url, dst=model_path)
         model._load_state_dict(model_path)
@@ -1053,23 +1057,25 @@
     ct_size = kwargs.pop("ct_size", 2)
     dim = kwargs.pop("dim", 96)
     in_dim = kwargs.pop("in_dim", 64)
     mlp_ratio = kwargs.pop("mlp_ratio", 4)
     resolution = kwargs.pop("resolution", [541, 960])
     drop_path_rate = kwargs.pop("drop_path_rate", 0.2)
     model_path = kwargs.pop("model_path", "/tmp/faster_vit_2.pth.tar")
+    hat = kwargs.pop("hat", [False, False, True, False])
     model = FasterViT(depths=depths,
                       num_heads=num_heads,
                       window_size=window_size,
                       ct_size=ct_size,
                       dim=dim,
                       in_dim=in_dim,
                       mlp_ratio=mlp_ratio,
                       resolution=resolution,
                       drop_path_rate=drop_path_rate,
+                      hat=hat
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_2_any_res']
     if pretrained:
         if not Path(model_path).is_file():
             url = model.default_cfg['url']
             torch.hub.download_url_to_file(url=url, dst=model_path)
         model._load_state_dict(model_path)
@@ -1086,63 +1092,67 @@
     dim = kwargs.pop("dim", 128)
     in_dim = kwargs.pop("in_dim", 64)
     mlp_ratio = kwargs.pop("mlp_ratio", 4)
     resolution = kwargs.pop("resolution", [576, 960])
     drop_path_rate = kwargs.pop("drop_path_rate", 0.3)
     layer_scale = kwargs.pop("layer_scale", 1e-5)
     model_path = kwargs.pop("model_path", "/tmp/faster_vit_3.pth.tar")
+    hat = kwargs.pop("hat", [False, False, True, False])
     model = FasterViT(depths=depths,
                       num_heads=num_heads,
                       window_size=window_size,
                       ct_size=ct_size,
                       dim=dim,
                       in_dim=in_dim,
                       mlp_ratio=mlp_ratio,
                       resolution=resolution,
                       drop_path_rate=drop_path_rate,
                       layer_scale=layer_scale,
                       layer_scale_conv=None,
                       do_propagation=True,
+                      hat=hat,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_3_any_res']
     if pretrained:
         if not Path(model_path).is_file():
             url = model.default_cfg['url']
             torch.hub.download_url_to_file(url=url, dst=model_path)
         model._load_state_dict(model_path)
     return model
 
 
 @register_pip_model
 @register_model
 def faster_vit_4_any_res(pretrained=False, **kwargs):
     depths = kwargs.pop("depths", [3, 3, 12, 5])
-    num_heads = kwargs.pop("num_heads", [2, 4, 8, 16])
+    num_heads = kwargs.pop("num_heads", [4, 8, 16, 32])
     window_size = kwargs.pop("window_size", [7, 7, 7, 7])
     ct_size = kwargs.pop("ct_size", 2)
     dim = kwargs.pop("dim", 196)
     in_dim = kwargs.pop("in_dim", 64)
     mlp_ratio = kwargs.pop("mlp_ratio", 4)
     resolution = kwargs.pop("resolution", [576, 960])
     drop_path_rate = kwargs.pop("drop_path_rate", 0.3)
     layer_scale = kwargs.pop("layer_scale", 1e-5)
     model_path = kwargs.pop("model_path", "/tmp/faster_vit_4.pth.tar")
+    hat = kwargs.pop("hat", [False, False, True, False])
     model = FasterViT(depths=depths,
                       num_heads=num_heads,
                       window_size=window_size,
                       ct_size=ct_size,
                       dim=dim,
                       in_dim=in_dim,
                       mlp_ratio=mlp_ratio,
                       resolution=resolution,
                       drop_path_rate=drop_path_rate,
                       layer_scale=layer_scale,
                       layer_scale_conv=None,
                       layer_norm_last=False,
                       do_propagation=True,
+                      hat=hat,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_4_any_res']
     if pretrained:
         if not Path(model_path).is_file():
             url = model.default_cfg['url']
             torch.hub.download_url_to_file(url=url, dst=model_path)
         model._load_state_dict(model_path)
@@ -1159,27 +1169,29 @@
     dim = kwargs.pop("dim", 320)
     in_dim = kwargs.pop("in_dim", 64)
     mlp_ratio = kwargs.pop("mlp_ratio", 4)
     resolution = kwargs.pop("resolution", [576, 960])
     drop_path_rate = kwargs.pop("drop_path_rate", 0.3)
     layer_scale = kwargs.pop("layer_scale", 1e-5)
     model_path = kwargs.pop("model_path", "/tmp/faster_vit_5.pth.tar")
+    hat = kwargs.pop("hat", [False, False, True, False])
     model = FasterViT(depths=depths,
                       num_heads=num_heads,
                       window_size=window_size,
                       ct_size=ct_size,
                       dim=dim,
                       in_dim=in_dim,
                       mlp_ratio=mlp_ratio,
                       resolution=resolution,
                       drop_path_rate=drop_path_rate,
                       layer_scale=layer_scale,
                       layer_scale_conv=None,
                       layer_norm_last=False,
                       do_propagation=True,
+                      hat=hat,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_5_any_res']
     if pretrained:
         if not Path(model_path).is_file():
             url = model.default_cfg['url']
             torch.hub.download_url_to_file(url=url, dst=model_path)
         model._load_state_dict(model_path)
@@ -1196,27 +1208,29 @@
     dim = kwargs.pop("dim", 320)
     in_dim = kwargs.pop("in_dim", 64)
     mlp_ratio = kwargs.pop("mlp_ratio", 4)
     resolution = kwargs.pop("resolution", [576, 960])
     drop_path_rate = kwargs.pop("drop_path_rate", 0.5)
     layer_scale = kwargs.pop("layer_scale", 1e-5)
     model_path = kwargs.pop("model_path", "/tmp/faster_vit_6.pth.tar")
+    hat = kwargs.pop("hat", [False, False, True, False])
     model = FasterViT(depths=depths,
                       num_heads=num_heads,
                       window_size=window_size,
                       ct_size=ct_size,
                       dim=dim,
                       in_dim=in_dim,
                       mlp_ratio=mlp_ratio,
                       resolution=resolution,
                       drop_path_rate=drop_path_rate,
                       layer_scale=layer_scale,
                       layer_scale_conv=None,
                       layer_norm_last=False,
                       do_propagation=True,
+                      hat=hat,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_6_any_res']
     if pretrained:
         if not Path(model_path).is_file():
             url = model.default_cfg['url']
             torch.hub.download_url_to_file(url=url, dst=model_path)
         model._load_state_dict(model_path)
```

### Comparing `fastervit-0.9.1/fastervit/models/registry.py` & `fastervit-0.9.2/fastervit/models/registry.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.1/fastervit/scheduler/cosine_lr.py` & `fastervit-0.9.2/fastervit/scheduler/cosine_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.1/fastervit/scheduler/multistep_lr.py` & `fastervit-0.9.2/fastervit/scheduler/multistep_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.1/fastervit/scheduler/plateau_lr.py` & `fastervit-0.9.2/fastervit/scheduler/plateau_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.1/fastervit/scheduler/poly_lr.py` & `fastervit-0.9.2/fastervit/scheduler/poly_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.1/fastervit/scheduler/scheduler.py` & `fastervit-0.9.2/fastervit/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.1/fastervit/scheduler/scheduler_factory.py` & `fastervit-0.9.2/fastervit/scheduler/scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.1/fastervit/scheduler/step_lr.py` & `fastervit-0.9.2/fastervit/scheduler/step_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.1/fastervit/scheduler/tanh_lr.py` & `fastervit-0.9.2/fastervit/scheduler/tanh_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.1/fastervit/tensorboard.py` & `fastervit-0.9.2/fastervit/tensorboard.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.1/fastervit/train.py` & `fastervit-0.9.2/fastervit/train.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.1/fastervit/utils/datasets.py` & `fastervit-0.9.2/fastervit/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.1/fastervit/validate.py` & `fastervit-0.9.2/fastervit/validate.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
             print("Quantization aware training is not supported for this model !")
 
     if args.num_classes is None:
         assert hasattr(model, 'num_classes'), 'Model must have `num_classes` attr if not set on cmd line/config.'
         args.num_classes = model.num_classes
 
     if args.checkpoint:
-        load_checkpoint(model, args.checkpoint, args.use_ema)
+        load_checkpoint(model, args.checkpoint, args.use_ema, strict=False)
 
     param_count = sum([m.numel() for m in model.parameters()])
     _logger.info('Model %s created, param count: %d' % (args.model, param_count))
 
     data_config = resolve_data_config(vars(args), model=model, use_test_size=True, verbose=True)
     test_time_pool = False
     if args.test_pool:
```

### Comparing `fastervit-0.9.1/fastervit.egg-info/SOURCES.txt` & `fastervit-0.9.2/fastervit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.1/setup.py` & `fastervit-0.9.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='fastervit',
-    version='0.9.1',
+    version='0.9.2',
     description='FasterViT: Fast Vision Transformers with Hierarchical Attention',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/NVlabs/FasterViT',
     author='Ali Hatamizadeh',
     author_email='ahatamiz123@gmail.com',
     classifiers=[
```

