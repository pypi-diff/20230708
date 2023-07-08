# Comparing `tmp/cwt-2.3.2.tar.gz` & `tmp/cwt-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cwt-2.3.2.tar", max compression
+gzip compressed data, was "cwt-2.4.0.tar", max compression
```

## Comparing `cwt-2.3.2.tar` & `cwt-2.4.0.tar`

### file list

```diff
@@ -1,130 +1,130 @@
--rw-r--r--   0        0        0    25375 2023-07-03 10:51:40.937580 cwt-2.3.2/CHANGES.rst
--rw-r--r--   0        0        0     1077 2023-07-03 10:51:40.937580 cwt-2.3.2/LICENSE
--rw-r--r--   0        0        0    52625 2023-07-03 10:51:40.937580 cwt-2.3.2/README.md
--rw-r--r--   0        0        0     1316 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/algs/__init__.py
--rw-r--r--   0        0        0     1381 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/algs/asymmetric.py
--rw-r--r--   0        0        0    12774 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/algs/ec2.py
--rw-r--r--   0        0        0    11923 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/algs/okp.py
--rw-r--r--   0        0        0      858 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/algs/raw.py
--rw-r--r--   0        0        0     5585 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/algs/rsa.py
--rw-r--r--   0        0        0    13279 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/algs/symmetric.py
--rw-r--r--   0        0        0      496 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/cbor_processor.py
--rw-r--r--   0        0        0     8994 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/claims.py
--rw-r--r--   0        0        0    11070 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/const.py
--rw-r--r--   0        0        0    33546 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/cose.py
--rw-r--r--   0        0        0    12038 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/cose_key.py
--rw-r--r--   0        0        0     9682 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/cose_key_interface.py
--rw-r--r--   0        0        0    10667 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/cose_message.py
--rw-r--r--   0        0        0    17714 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/cwt.py
--rw-r--r--   0        0        0     2595 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/encrypted_cose_key.py
--rw-r--r--   0        0        0      190 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/enums.py
--rw-r--r--   0        0        0      455 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/helpers/__init__.py
--rw-r--r--   0        0        0     2017 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/helpers/hcert.py
--rw-r--r--   0        0        0        0 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/py.typed
--rw-r--r--   0        0        0     5750 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/recipient.py
--rw-r--r--   0        0        0        0 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/recipient_algs/__init__.py
--rw-r--r--   0        0        0     2068 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/recipient_algs/aes_key_wrap.py
--rw-r--r--   0        0        0      471 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/recipient_algs/direct.py
--rw-r--r--   0        0        0     3542 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/recipient_algs/direct_hkdf.py
--rw-r--r--   0        0        0      789 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/recipient_algs/direct_key.py
--rw-r--r--   0        0        0     4374 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/recipient_algs/ecdh_aes_key_wrap.py
--rw-r--r--   0        0        0     4417 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/recipient_algs/ecdh_direct_hkdf.py
--rw-r--r--   0        0        0     2652 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/recipient_algs/hpke.py
--rw-r--r--   0        0        0     8500 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/recipient_interface.py
--rw-r--r--   0        0        0     2712 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/recipients.py
--rw-r--r--   0        0        0     5892 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/signer.py
--rw-r--r--   0        0        0    11661 2023-07-03 10:51:40.937580 cwt-2.3.2/cwt/utils.py
--rw-r--r--   0        0        0      634 2023-07-03 10:51:40.937580 cwt-2.3.2/docs/Makefile
--rw-r--r--   0        0        0    18577 2023-07-03 10:51:40.937580 cwt-2.3.2/docs/algorithms.rst
--rw-r--r--   0        0        0      373 2023-07-03 10:51:40.937580 cwt-2.3.2/docs/api.rst
--rw-r--r--   0        0        0       28 2023-07-03 10:51:40.937580 cwt-2.3.2/docs/changes.rst
--rw-r--r--   0        0        0     5646 2023-07-03 10:51:40.937580 cwt-2.3.2/docs/claims.rst
--rw-r--r--   0        0        0     3365 2023-07-03 10:51:40.937580 cwt-2.3.2/docs/conf.py
--rw-r--r--   0        0        0     1637 2023-07-03 10:51:40.937580 cwt-2.3.2/docs/index.rst
--rw-r--r--   0        0        0      112 2023-07-03 10:51:40.937580 cwt-2.3.2/docs/installation.rst
--rw-r--r--   0        0        0    91992 2023-07-03 10:51:40.937580 cwt-2.3.2/poetry.lock
--rw-r--r--   0        0        0     1093 2023-07-03 10:51:40.945580 cwt-2.3.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-03 10:51:40.945580 cwt-2.3.2/samples/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 10:51:40.945580 cwt-2.3.2/samples/eudcc/__init__.py
--rw-r--r--   0        0        0     4765 2023-07-03 10:51:40.945580 cwt-2.3.2/samples/eudcc/swedish_verifier.py
--rw-r--r--   0        0        0     5065 2023-07-03 10:51:40.945580 cwt-2.3.2/samples/eudcc/verifier.py
--rw-r--r--   0        0        0        0 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/__init__.py
--rw-r--r--   0        0        0     1338 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/cacert.pem
--rw-r--r--   0        0        0     1350 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/cacert_2.pem
--rw-r--r--   0        0        0     1854 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/cakey.pem
--rw-r--r--   0        0        0     2401 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/cert_es256.json
--rw-r--r--   0        0        0      956 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/cert_es256.pem
--rw-r--r--   0        0        0     1128 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/cert_es256_2.json
--rw-r--r--   0        0        0      655 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/hcert_testdata_cert_at.pem
--rw-r--r--   0        0        0      437 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/hs256.json
--rw-r--r--   0        0        0      437 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/hs384.json
--rw-r--r--   0        0        0      437 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/hs512.json
--rw-r--r--   0        0        0      241 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/private_key_cert_es256.pem
--rw-r--r--   0        0        0      198 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/private_key_ed25519.json
--rw-r--r--   0        0        0      119 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/private_key_ed25519.pem
--rw-r--r--   0        0        0      260 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/private_key_ed448.json
--rw-r--r--   0        0        0      156 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/private_key_ed448.pem
--rw-r--r--   0        0        0      249 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/private_key_es256.json
--rw-r--r--   0        0        0      227 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/private_key_es256.pem
--rw-r--r--   0        0        0      257 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/private_key_es256k.json
--rw-r--r--   0        0        0      223 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/private_key_es256k.pem
--rw-r--r--   0        0        0      312 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/private_key_es384.json
--rw-r--r--   0        0        0      288 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/private_key_es384.pem
--rw-r--r--   0        0        0      384 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/private_key_es512.json
--rw-r--r--   0        0        0      365 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/private_key_es512.pem
--rw-r--r--   0        0        0     1732 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/private_key_rsa.json
--rw-r--r--   0        0        0     1704 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/private_key_rsa.pem
--rw-r--r--   0        0        0      207 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/private_key_x25519.json
--rw-r--r--   0        0        0      119 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/private_key_x25519.pem
--rw-r--r--   0        0        0      267 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/private_key_x448.json
--rw-r--r--   0        0        0      152 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/private_key_x448.pem
--rw-r--r--   0        0        0      162 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/public_key_ed25519.json
--rw-r--r--   0        0        0      113 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/public_key_ed25519.pem
--rw-r--r--   0        0        0      191 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/public_key_ed448.json
--rw-r--r--   0        0        0      146 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/public_key_ed448.pem
--rw-r--r--   0        0        0      213 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/public_key_es256.json
--rw-r--r--   0        0        0      178 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/public_key_es256.pem
--rw-r--r--   0        0        0      222 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/public_key_es256k.json
--rw-r--r--   0        0        0      174 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/public_key_es256k.pem
--rw-r--r--   0        0        0      255 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/public_key_es384.json
--rw-r--r--   0        0        0      215 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/public_key_es384.pem
--rw-r--r--   0        0        0      303 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/public_key_es512.json
--rw-r--r--   0        0        0      268 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/public_key_es512.pem
--rw-r--r--   0        0        0      454 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/public_key_rsa.json
--rw-r--r--   0        0        0      451 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/public_key_rsa.pem
--rw-r--r--   0        0        0      151 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/public_key_x25519.json
--rw-r--r--   0        0        0      113 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/public_key_x25519.pem
--rw-r--r--   0        0        0      179 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/public_key_x448.json
--rw-r--r--   0        0        0      146 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/keys/public_key_x448.pem
--rw-r--r--   0        0        0     1515 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/test_algs_aes_key_wrap.py
--rw-r--r--   0        0        0    36684 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/test_algs_ec2.py
--rw-r--r--   0        0        0    27545 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/test_algs_okp.py
--rw-r--r--   0        0        0     1294 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/test_algs_raw.py
--rw-r--r--   0        0        0    10106 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/test_algs_rsa.py
--rw-r--r--   0        0        0    22602 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/test_algs_symmetric.py
--rw-r--r--   0        0        0     5804 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/test_claims.py
--rw-r--r--   0        0        0    49481 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/test_cose.py
--rw-r--r--   0        0        0     8940 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/test_cose_hpke.py
--rw-r--r--   0        0        0    26496 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/test_cose_key.py
--rw-r--r--   0        0        0    18424 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/test_cose_message.py
--rw-r--r--   0        0        0    27850 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/test_cose_sample.py
--rw-r--r--   0        0        0    38331 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/test_cose_sample_with_encode.py
--rw-r--r--   0        0        0    24699 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/test_cose_wg_examples.py
--rw-r--r--   0        0        0    23829 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/test_cwt.py
--rw-r--r--   0        0        0    43886 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/test_cwt_sample.py
--rw-r--r--   0        0        0     1205 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/test_encrypted_cose_key.py
--rw-r--r--   0        0        0     6791 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/test_helpers_hcert.py
--rw-r--r--   0        0        0     4909 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/test_key.py
--rw-r--r--   0        0        0    28160 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/test_recipient.py
--rw-r--r--   0        0        0     5552 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/test_recipient_algs_aes_key_wrap.py
--rw-r--r--   0        0        0    15162 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/test_recipient_algs_direct.py
--rw-r--r--   0        0        0    10464 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/test_recipient_algs_ecdh_aes_key_wrap.py
--rw-r--r--   0        0        0    17884 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/test_recipient_algs_ecdh_direct_hkdf.py
--rw-r--r--   0        0        0     1953 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/test_recipient_algs_hpke.py
--rw-r--r--   0        0        0     8237 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/test_signer.py
--rw-r--r--   0        0        0     4792 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/test_utils.py
--rw-r--r--   0        0        0      265 2023-07-03 10:51:40.945580 cwt-2.3.2/tests/utils.py
--rw-r--r--   0        0        0     1100 2023-07-03 10:51:40.945580 cwt-2.3.2/tox.ini
--rw-r--r--   0        0        0    53716 1970-01-01 00:00:00.000000 cwt-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0    26000 2023-07-08 07:57:45.418772 cwt-2.4.0/CHANGES.rst
+-rw-r--r--   0        0        0     1077 2023-07-08 07:57:45.418772 cwt-2.4.0/LICENSE
+-rw-r--r--   0        0        0    55381 2023-07-08 07:57:45.418772 cwt-2.4.0/README.md
+-rw-r--r--   0        0        0     1359 2023-07-08 07:57:45.418772 cwt-2.4.0/cwt/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 07:57:45.418772 cwt-2.4.0/cwt/algs/__init__.py
+-rw-r--r--   0        0        0     1381 2023-07-08 07:57:45.418772 cwt-2.4.0/cwt/algs/asymmetric.py
+-rw-r--r--   0        0        0    12774 2023-07-08 07:57:45.422772 cwt-2.4.0/cwt/algs/ec2.py
+-rw-r--r--   0        0        0    11923 2023-07-08 07:57:45.422772 cwt-2.4.0/cwt/algs/okp.py
+-rw-r--r--   0        0        0      858 2023-07-08 07:57:45.422772 cwt-2.4.0/cwt/algs/raw.py
+-rw-r--r--   0        0        0     5585 2023-07-08 07:57:45.422772 cwt-2.4.0/cwt/algs/rsa.py
+-rw-r--r--   0        0        0    13279 2023-07-08 07:57:45.422772 cwt-2.4.0/cwt/algs/symmetric.py
+-rw-r--r--   0        0        0      496 2023-07-08 07:57:45.422772 cwt-2.4.0/cwt/cbor_processor.py
+-rw-r--r--   0        0        0     8994 2023-07-08 07:57:45.422772 cwt-2.4.0/cwt/claims.py
+-rw-r--r--   0        0        0    11085 2023-07-08 07:57:45.422772 cwt-2.4.0/cwt/const.py
+-rw-r--r--   0        0        0    35047 2023-07-08 07:57:45.422772 cwt-2.4.0/cwt/cose.py
+-rw-r--r--   0        0        0    12038 2023-07-08 07:57:45.422772 cwt-2.4.0/cwt/cose_key.py
+-rw-r--r--   0        0        0     9682 2023-07-08 07:57:45.422772 cwt-2.4.0/cwt/cose_key_interface.py
+-rw-r--r--   0        0        0    10682 2023-07-08 07:57:45.422772 cwt-2.4.0/cwt/cose_message.py
+-rw-r--r--   0        0        0    18090 2023-07-08 07:57:45.422772 cwt-2.4.0/cwt/cwt.py
+-rw-r--r--   0        0        0     2595 2023-07-08 07:57:45.422772 cwt-2.4.0/cwt/encrypted_cose_key.py
+-rw-r--r--   0        0        0      966 2023-07-08 07:57:45.422772 cwt-2.4.0/cwt/enums.py
+-rw-r--r--   0        0        0      455 2023-07-08 07:57:45.422772 cwt-2.4.0/cwt/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-08 07:57:45.422772 cwt-2.4.0/cwt/helpers/__init__.py
+-rw-r--r--   0        0        0     2017 2023-07-08 07:57:45.422772 cwt-2.4.0/cwt/helpers/hcert.py
+-rw-r--r--   0        0        0        0 2023-07-08 07:57:45.422772 cwt-2.4.0/cwt/py.typed
+-rw-r--r--   0        0        0     5750 2023-07-08 07:57:45.422772 cwt-2.4.0/cwt/recipient.py
+-rw-r--r--   0        0        0        0 2023-07-08 07:57:45.422772 cwt-2.4.0/cwt/recipient_algs/__init__.py
+-rw-r--r--   0        0        0     2068 2023-07-08 07:57:45.422772 cwt-2.4.0/cwt/recipient_algs/aes_key_wrap.py
+-rw-r--r--   0        0        0      471 2023-07-08 07:57:45.422772 cwt-2.4.0/cwt/recipient_algs/direct.py
+-rw-r--r--   0        0        0     3542 2023-07-08 07:57:45.422772 cwt-2.4.0/cwt/recipient_algs/direct_hkdf.py
+-rw-r--r--   0        0        0      789 2023-07-08 07:57:45.422772 cwt-2.4.0/cwt/recipient_algs/direct_key.py
+-rw-r--r--   0        0        0     4374 2023-07-08 07:57:45.422772 cwt-2.4.0/cwt/recipient_algs/ecdh_aes_key_wrap.py
+-rw-r--r--   0        0        0     4417 2023-07-08 07:57:45.422772 cwt-2.4.0/cwt/recipient_algs/ecdh_direct_hkdf.py
+-rw-r--r--   0        0        0     2652 2023-07-08 07:57:45.422772 cwt-2.4.0/cwt/recipient_algs/hpke.py
+-rw-r--r--   0        0        0     8500 2023-07-08 07:57:45.422772 cwt-2.4.0/cwt/recipient_interface.py
+-rw-r--r--   0        0        0     2712 2023-07-08 07:57:45.422772 cwt-2.4.0/cwt/recipients.py
+-rw-r--r--   0        0        0     5892 2023-07-08 07:57:45.422772 cwt-2.4.0/cwt/signer.py
+-rw-r--r--   0        0        0    11661 2023-07-08 07:57:45.422772 cwt-2.4.0/cwt/utils.py
+-rw-r--r--   0        0        0      634 2023-07-08 07:57:45.422772 cwt-2.4.0/docs/Makefile
+-rw-r--r--   0        0        0    18577 2023-07-08 07:57:45.422772 cwt-2.4.0/docs/algorithms.rst
+-rw-r--r--   0        0        0      373 2023-07-08 07:57:45.422772 cwt-2.4.0/docs/api.rst
+-rw-r--r--   0        0        0       28 2023-07-08 07:57:45.422772 cwt-2.4.0/docs/changes.rst
+-rw-r--r--   0        0        0     5646 2023-07-08 07:57:45.422772 cwt-2.4.0/docs/claims.rst
+-rw-r--r--   0        0        0     3365 2023-07-08 07:57:45.422772 cwt-2.4.0/docs/conf.py
+-rw-r--r--   0        0        0     1637 2023-07-08 07:57:45.422772 cwt-2.4.0/docs/index.rst
+-rw-r--r--   0        0        0      112 2023-07-08 07:57:45.422772 cwt-2.4.0/docs/installation.rst
+-rw-r--r--   0        0        0    90700 2023-07-08 07:57:45.422772 cwt-2.4.0/poetry.lock
+-rw-r--r--   0        0        0     1093 2023-07-08 07:57:45.422772 cwt-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-08 07:57:45.422772 cwt-2.4.0/samples/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 07:57:45.422772 cwt-2.4.0/samples/eudcc/__init__.py
+-rw-r--r--   0        0        0     4765 2023-07-08 07:57:45.422772 cwt-2.4.0/samples/eudcc/swedish_verifier.py
+-rw-r--r--   0        0        0     5065 2023-07-08 07:57:45.422772 cwt-2.4.0/samples/eudcc/verifier.py
+-rw-r--r--   0        0        0        0 2023-07-08 07:57:45.422772 cwt-2.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     1338 2023-07-08 07:57:45.422772 cwt-2.4.0/tests/keys/cacert.pem
+-rw-r--r--   0        0        0     1350 2023-07-08 07:57:45.422772 cwt-2.4.0/tests/keys/cacert_2.pem
+-rw-r--r--   0        0        0     1854 2023-07-08 07:57:45.422772 cwt-2.4.0/tests/keys/cakey.pem
+-rw-r--r--   0        0        0     2401 2023-07-08 07:57:45.422772 cwt-2.4.0/tests/keys/cert_es256.json
+-rw-r--r--   0        0        0      956 2023-07-08 07:57:45.422772 cwt-2.4.0/tests/keys/cert_es256.pem
+-rw-r--r--   0        0        0     1128 2023-07-08 07:57:45.422772 cwt-2.4.0/tests/keys/cert_es256_2.json
+-rw-r--r--   0        0        0      655 2023-07-08 07:57:45.422772 cwt-2.4.0/tests/keys/hcert_testdata_cert_at.pem
+-rw-r--r--   0        0        0      437 2023-07-08 07:57:45.422772 cwt-2.4.0/tests/keys/hs256.json
+-rw-r--r--   0        0        0      437 2023-07-08 07:57:45.422772 cwt-2.4.0/tests/keys/hs384.json
+-rw-r--r--   0        0        0      437 2023-07-08 07:57:45.422772 cwt-2.4.0/tests/keys/hs512.json
+-rw-r--r--   0        0        0      241 2023-07-08 07:57:45.422772 cwt-2.4.0/tests/keys/private_key_cert_es256.pem
+-rw-r--r--   0        0        0      198 2023-07-08 07:57:45.422772 cwt-2.4.0/tests/keys/private_key_ed25519.json
+-rw-r--r--   0        0        0      119 2023-07-08 07:57:45.422772 cwt-2.4.0/tests/keys/private_key_ed25519.pem
+-rw-r--r--   0        0        0      260 2023-07-08 07:57:45.422772 cwt-2.4.0/tests/keys/private_key_ed448.json
+-rw-r--r--   0        0        0      156 2023-07-08 07:57:45.422772 cwt-2.4.0/tests/keys/private_key_ed448.pem
+-rw-r--r--   0        0        0      249 2023-07-08 07:57:45.422772 cwt-2.4.0/tests/keys/private_key_es256.json
+-rw-r--r--   0        0        0      227 2023-07-08 07:57:45.422772 cwt-2.4.0/tests/keys/private_key_es256.pem
+-rw-r--r--   0        0        0      257 2023-07-08 07:57:45.422772 cwt-2.4.0/tests/keys/private_key_es256k.json
+-rw-r--r--   0        0        0      223 2023-07-08 07:57:45.422772 cwt-2.4.0/tests/keys/private_key_es256k.pem
+-rw-r--r--   0        0        0      312 2023-07-08 07:57:45.422772 cwt-2.4.0/tests/keys/private_key_es384.json
+-rw-r--r--   0        0        0      288 2023-07-08 07:57:45.422772 cwt-2.4.0/tests/keys/private_key_es384.pem
+-rw-r--r--   0        0        0      384 2023-07-08 07:57:45.422772 cwt-2.4.0/tests/keys/private_key_es512.json
+-rw-r--r--   0        0        0      365 2023-07-08 07:57:45.422772 cwt-2.4.0/tests/keys/private_key_es512.pem
+-rw-r--r--   0        0        0     1732 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/keys/private_key_rsa.json
+-rw-r--r--   0        0        0     1704 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/keys/private_key_rsa.pem
+-rw-r--r--   0        0        0      207 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/keys/private_key_x25519.json
+-rw-r--r--   0        0        0      119 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/keys/private_key_x25519.pem
+-rw-r--r--   0        0        0      267 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/keys/private_key_x448.json
+-rw-r--r--   0        0        0      152 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/keys/private_key_x448.pem
+-rw-r--r--   0        0        0      162 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/keys/public_key_ed25519.json
+-rw-r--r--   0        0        0      113 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/keys/public_key_ed25519.pem
+-rw-r--r--   0        0        0      191 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/keys/public_key_ed448.json
+-rw-r--r--   0        0        0      146 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/keys/public_key_ed448.pem
+-rw-r--r--   0        0        0      213 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/keys/public_key_es256.json
+-rw-r--r--   0        0        0      178 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/keys/public_key_es256.pem
+-rw-r--r--   0        0        0      222 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/keys/public_key_es256k.json
+-rw-r--r--   0        0        0      174 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/keys/public_key_es256k.pem
+-rw-r--r--   0        0        0      255 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/keys/public_key_es384.json
+-rw-r--r--   0        0        0      215 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/keys/public_key_es384.pem
+-rw-r--r--   0        0        0      303 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/keys/public_key_es512.json
+-rw-r--r--   0        0        0      268 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/keys/public_key_es512.pem
+-rw-r--r--   0        0        0      454 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/keys/public_key_rsa.json
+-rw-r--r--   0        0        0      451 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/keys/public_key_rsa.pem
+-rw-r--r--   0        0        0      151 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/keys/public_key_x25519.json
+-rw-r--r--   0        0        0      113 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/keys/public_key_x25519.pem
+-rw-r--r--   0        0        0      179 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/keys/public_key_x448.json
+-rw-r--r--   0        0        0      146 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/keys/public_key_x448.pem
+-rw-r--r--   0        0        0     1515 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/test_algs_aes_key_wrap.py
+-rw-r--r--   0        0        0    36684 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/test_algs_ec2.py
+-rw-r--r--   0        0        0    27545 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/test_algs_okp.py
+-rw-r--r--   0        0        0     1294 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/test_algs_raw.py
+-rw-r--r--   0        0        0    10106 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/test_algs_rsa.py
+-rw-r--r--   0        0        0    22602 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/test_algs_symmetric.py
+-rw-r--r--   0        0        0     5804 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/test_claims.py
+-rw-r--r--   0        0        0    49481 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/test_cose.py
+-rw-r--r--   0        0        0     8940 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/test_cose_hpke.py
+-rw-r--r--   0        0        0    26496 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/test_cose_key.py
+-rw-r--r--   0        0        0    18452 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/test_cose_message.py
+-rw-r--r--   0        0        0    28409 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/test_cose_sample.py
+-rw-r--r--   0        0        0    38331 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/test_cose_sample_with_encode.py
+-rw-r--r--   0        0        0    24699 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/test_cose_wg_examples.py
+-rw-r--r--   0        0        0    25416 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/test_cwt.py
+-rw-r--r--   0        0        0    46254 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/test_cwt_sample.py
+-rw-r--r--   0        0        0     1205 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/test_encrypted_cose_key.py
+-rw-r--r--   0        0        0     6791 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/test_helpers_hcert.py
+-rw-r--r--   0        0        0     4909 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/test_key.py
+-rw-r--r--   0        0        0    28160 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/test_recipient.py
+-rw-r--r--   0        0        0     5552 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/test_recipient_algs_aes_key_wrap.py
+-rw-r--r--   0        0        0    15162 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/test_recipient_algs_direct.py
+-rw-r--r--   0        0        0    10464 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/test_recipient_algs_ecdh_aes_key_wrap.py
+-rw-r--r--   0        0        0    17884 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/test_recipient_algs_ecdh_direct_hkdf.py
+-rw-r--r--   0        0        0     1953 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/test_recipient_algs_hpke.py
+-rw-r--r--   0        0        0     8237 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/test_signer.py
+-rw-r--r--   0        0        0     4792 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/test_utils.py
+-rw-r--r--   0        0        0      265 2023-07-08 07:57:45.426772 cwt-2.4.0/tests/utils.py
+-rw-r--r--   0        0        0     1100 2023-07-08 07:57:45.426772 cwt-2.4.0/tox.ini
+-rw-r--r--   0        0        0    56472 1970-01-01 00:00:00.000000 cwt-2.4.0/PKG-INFO
```

### Comparing `cwt-2.3.2/CHANGES.rst` & `cwt-2.4.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,26 @@
 Changes
 =======
 
 Unreleased
 ----------
 
+Version 2.4.0
+-------------
+
+Released 2023-07-08
+
+- Fix and update examples in README. `#405 <https://github.com/dajiaji/python-cwt/pull/405>`__
+- Add enum CWTClaims. `#404 <https://github.com/dajiaji/python-cwt/pull/404>`__
+- Rename COSEType to COSETypes. `#403 <https://github.com/dajiaji/python-cwt/pull/403>`__
+- Add enum COSEHeaders. `#401 <https://github.com/dajiaji/python-cwt/pull/401>`__
+- Add experimental support for CWT claims in COSE headers. `#400 <https://github.com/dajiaji/python-cwt/pull/400>`__
+- Update dev dependencies.
+    - Bump tox to 4.6.4. `#398 <https://github.com/dajiaji/python-cwt/pull/398>`__
+
 Version 2.3.2
 -------------
 
 Released 2023-07-03
 
 - Update the base python version on CI/CD. `#396 <https://github.com/dajiaji/python-cwt/pull/396>`__
 - Drop support for Python 3.7. `#391 <https://github.com/dajiaji/python-cwt/pull/391>`__
```

### Comparing `cwt-2.3.2/LICENSE` & `cwt-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/README.md` & `cwt-2.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 Python CWT is a CBOR Web Token (CWT) and CBOR Object Signing and Encryption (COSE)
 implementation compliant with:
 - [RFC9052: CBOR Object Signing and Encryption (COSE): Structures and Process](https://www.rfc-editor.org/rfc/rfc9052.html)
 - [RFC9053: CBOR Object Signing and Encryption (COSE): Initial Algorithms](https://www.rfc-editor.org/rfc/rfc9053.html)
 - [RFC9338: CBOR Object Signing and Encryption (COSE): Countersignatures](https://www.rfc-editor.org/rfc/rfc9338.html) - experimental
 - [RFC8392: CWT (CBOR Web Token)](https://tools.ietf.org/html/rfc8392)
 - [draft-04: Use of HPKE with COSE](https://www.ietf.org/archive/id/draft-ietf-cose-hpke-04.html) - experimental
+- [draft-05: CWT Claims in COSE Headers](https://www.ietf.org/archive/id/draft-ietf-cose-cwt-claims-in-headers-05.html) - experimental
 - and related various specifications. See [Referenced Specifications](#referenced-specifications).
 
 It is designed to make users who already know about [JWS](https://tools.ietf.org/html/rfc7515)/[JWE](https://tools.ietf.org/html/rfc7516)/[JWT](https://tools.ietf.org/html/rfc7519)
 be able to use it in ease. Little knowledge of [CBOR](https://tools.ietf.org/html/rfc7049)/[COSE](https://tools.ietf.org/html/rfc8152)/[CWT](https://tools.ietf.org/html/rfc8392)
 is required to use it.
 
 You can install Python CWT with pip:
@@ -44,30 +45,44 @@
     protected={"alg": "HS256"},
     unprotected={"kid": "01"},
 )
 
 # The recipient side:
 recipient = COSE.new()
 assert b"Hello world!" == recipient.decode(encoded, mac_key)
+
+## You can get decoded protected/unprotected headers with the payload as follows:
+# protected, unprotected, payload = recipient.decode_with_headers(encoded, mac_key)
+# assert b"Hello world!" == payload
 ```
 
 **CWT API**
 
 ```py
 import cwt
-from cwt import COSEKey
+from cwt import COSEKey, CWTClaims
 
 mac_key = COSEKey.generate_symmetric_key(alg="HS256", kid="01")
 
 # The sender side:
-token = encode({1: "coaps://as.example", 2: "dajiaji", 7: b"123"}, mac_key)
+token = encode({
+    CWTClaims.ISS: "coaps://as.example",
+    CWTClaims.SUB: "dajiaji",
+    CWTClaims.CTI: b"123"}, mac_key)
 
 # The recipient side:
 decoded = decode(token, mac_key)
-# decoded == {1: 'coaps://as.example', 2: 'dajiaji', 7: b'123', 4: 1620088759, 5: 1620085159, 6: 1620085159}
+# decoded == {
+#     CWTClaims.ISS: 'coaps://as.example',
+#     CWTClaims.SUB: 'dajiaji',
+#     CWTClaims.CTI: b'123',
+#     CWTClaims.EXP: 1620088759,
+#     CWTClaims.NBF: 1620085159,
+#     CWTClaims.IAT: 1620085159
+# }
 ```
 
 Various usage examples are shown in this README.
 
 See [Documentation](https://python-cwt.readthedocs.io/en/stable/) for details of the APIs.
 
 ## Index
@@ -106,14 +121,15 @@
 - [CWT Usage Examples](#cwt-usage-examples)
     - [MACed CWT](#maced-cwt)
     - [Signed CWT](#signed-cwt)
     - [Encrypted CWT](#encrypted-cwt)
     - [Nested CWT](#nested-cwt)
     - [CWT with User Settings (e.g., expires\_in)](#cwt-with-user-settings)
     - [CWT with User-Defined Claims](#cwt-with-user-defined-claims)
+    - [CWT with CWT claims in COSE headers](#cwt-cwt-claims-in-cose-headers)
     - [CWT with PoP Key](#cwt-with-pop-key)
     - [CWT with Private CA](#cwt-with-private-ca)
     - [CWT for EUDCC (EU Digital COVID Certificate)](#cwt-for-eudcc-eu-digital-covid-certificate)
 - [API Reference](#api-reference)
 - [Supported CWT Claims](#supported-cwt-claims)
 - [Supported COSE Algorithms](#supported-cose-algorithms)
 - [Referenced Specifications](#referenced-specifications)
@@ -160,25 +176,25 @@
 ```
 
 Following two samples are other ways of writing the above example.
 
 CBOR object can be used for `protected` and `unprotected` header parameters as follows:
 
 ```py
-from cwt import COSE, COSEKey
+from cwt import COSE, COSEHeaders, COSEKey
 
 mac_key = COSEKey.generate_symmetric_key(alg="HS256", kid="01")
 
 # The sender side:
 sender = COSE.new()
 encoded = sender.encode(
     b"Hello world!",
     mac_key,
-    protected={1: 5},
-    unprotected={4: b"01"},
+    protected={COSEHeaders.ALG: 5},
+    unprotected={COSEHeaders.KID: b"01"},
 )
 
 # The recipient side:
 recipient = COSE.new()
 assert b"Hello world!" == recipient.decode(encoded, mac_key)
 ```
 
@@ -487,46 +503,46 @@
 #### COSE-HPKE (MAC)
 
 **Experimental Implementation. DO NOT USE for production.**
 
 Create a COSE-HPKE MAC message, verify and decode it as follows:
 
 ```py
-from cwt import COSE, COSEKey, Recipient
+from cwt import COSE, COSEHeaders, COSEKey, Recipient
 
 # The sender side:
 mac_key = COSEKey.generate_symmetric_key(alg="HS256")
 rpk = COSEKey.from_jwk(
     {
         "kty": "EC",
         "kid": "01",
         "crv": "P-256",
         "x": "usWxHK2PmfnHKwXPS54m0kTcGJ90UiglWiGahtagnv8",
         "y": "IBOL-C3BttVivg-lSreASjpkttcsz-1rb7btKLv8EX4",
     }
 )
 r = Recipient.new(
     protected={
-        1: -1,  # alg: "HPKE"
+        COSEHeaders.ALG: -1,  # alg: "HPKE"
     },
     unprotected={
-        4: b"01",  # kid: "01"
-        -4: [  # HPKE sender information
+        COSEHeaders.KID: b"01",  # kid: "01"
+        COSEHeaders.HPKE_SENDER_INFO: [  # HPKE sender information
             0x0010,  # kem: DHKEM(P-256, HKDF-SHA256)
             0x0001,  # kdf: HKDF-SHA256
             0x0001,  # aead: AES-128-GCM
         ],
     },
     recipient_key=rpk,
 )
 sender = COSE.new()
 encoded = sender.encode(
     b"This is the content.",
     mac_key,
-    protected={1: 5},  # alg: HS256
+    protected={COSEHeaders.ALG: 5},  # alg: HS256
     recipients=[r],
 )
 
 # The recipient side:
 rsk = COSEKey.from_jwk(
     {
         "kty": "EC",
@@ -551,15 +567,15 @@
 from cwt import COSE, COSEKey
 
 enc_key = COSEKey.generate_symmetric_key(alg="ChaCha20/Poly1305", kid="01")
 
 # The sender side:
 nonce = enc_key.generate_nonce()
 sender = COSE.new(alg_auto_inclusion=True, kid_auto_inclusion=True)
-encoded = sender.encode(b"Hello world!", enc_key, unprotected={5: nonce})
+encoded = sender.encode(b"Hello world!", enc_key, unprotected={COSEHeaders.IV: nonce})
 
 # The recipient side:
 recipient = COSE.new()
 assert b"Hello world!" == recipient.decode(encoded, enc_key)
 ```
 
 The following sample is another way of writing the above:
@@ -594,15 +610,15 @@
 from cwt import COSE, COSEKey, COSEMessage
 
 enc_key = COSEKey.generate_symmetric_key(alg="ChaCha20/Poly1305", kid="01")
 
 # The sender side:
 nonce = enc_key.generate_nonce()
 sender = COSE.new(alg_auto_inclusion=True, kid_auto_inclusion=True)
-encoded = sender.encode(b"Hello world!", enc_key, unprotected={5: nonce})
+encoded = sender.encode(b"Hello world!", enc_key, unprotected={COSEHeaders.IV: nonce})
 
 # The notary side:
 notary = Signer.from_jwk(
     {
         "kid": "01",
         "kty": "OKP",
         "crv": "Ed25519",
@@ -637,15 +653,15 @@
 #### COSE-HPKE (Encrypt0)
 
 **Experimental Implementation. DO NOT USE for production.**
 
 Create a COSE-HPKE Encrypt0 message and decrypt it as follows:
 
 ```py
-from cwt import COSE, COSEKey
+from cwt import COSE, COSEHeaders, COSEKey
 
 # The sender side:
 rpk = COSEKey.from_jwk(
     {
         "kty": "EC",
         "kid": "01",
         "crv": "P-256",
@@ -655,19 +671,19 @@
 )
 
 sender = COSE.new()
 encoded = sender.encode(
     b"This is the content.",
     rpk,
     protected={
-        1: -1,  # alg: "HPKE"
+        COSEHeaders.ALG: -1,  # alg: "HPKE"
     },
     unprotected={
-        4: b"01",  # kid: "01"
-        -4: [  # HPKE sender information
+        COSEHeaders.KID: b"01",  # kid: "01"
+        COSEHeaders.HPKE_SENDER_INFO: [  # HPKE sender information
             0x0010,  # kem: DHKEM(P-256, HKDF-SHA256)
             0x0001,  # kdf: HKDF-SHA256
             0x0001,  # aead: AES-128-GCM
         ],
     },
 )
 
@@ -691,31 +707,31 @@
 #### Direct Key Distribution for encryption
 
 The direct key distribution shares a MAC key between the sender and the recipient that is used directly.
 The follwing example shows the simplest way to make a COSE MAC message, verify and decode it with the direct
 key distribution method.
 
 ```py
-from cwt import COSE, COSEKey, Recipient
+from cwt import COSE, COSEHeaders, COSEKey, Recipient
 
 enc_key = COSEKey.generate_symmetric_key(alg="ChaCha20/Poly1305", kid="01")
 
 # The sender side:
 nonce = enc_key.generate_nonce()
 r = Recipient.new(unprotected={"alg": "direct"})
-# r = Recipient.new(unprotected={1: -6}) # is also acceptable.
+# r = Recipient.new(unprotected={COSEHeaders.ALG: -6}) # is also acceptable.
 
 sender = COSE.new()
 encoded = sender.encode(
     b"Hello world!",
     enc_key,
     protected={"alg": "ChaCha20/Poly1305"},
-    # protected={1: 24},  # is also acceptable.
+    # protected={COSEHeaders.ALG: 24},  # is also acceptable.
     unprotected={"kid": enc_key.kid, "iv": nonce},
-    # unprotected={4: enc_key.kid, 5: nonce},  # is also acceptable.
+    # unprotected={COSEHeaders.KID: enc_key.kid, COSEHeaders.IV: nonce},  # is also acceptable.
     recipients=[r],
 )
 
 # The recipient side:
 recipient = COSE.new()
 assert b"Hello world!" == recipient.decode(encoded, enc_key)
 ```
@@ -859,15 +875,15 @@
   recipient_key=r_pub_key,
   context={"alg": "A128GCM"},
 )
 sender = COSE.new(alg_auto_inclusion=True)
 encoded = sender.encode(
     b"Hello world!",
     key=enc_key,
-    unprotected={5: nonce},
+    unprotected={COSEHeaders.IV: nonce},
     recipients=[r],
 )
 
 # The recipient side:
 recipient = COSE.new()
 r_priv_key = COSEKey.from_jwk(
     {
@@ -945,47 +961,47 @@
 #### COSE-HPKE (Encrypt)
 
 **Experimental Implementation. DO NOT USE for production.**
 
 Create a COSE-HPKE Encrypt message and decrypt it as follows:
 
 ```py
-from cwt import COSE, COSEKey, Recipient
+from cwt import COSE, COSEHeaders, COSEKey, Recipient
 
 # The sender side:
 enc_key = COSEKey.generate_symmetric_key(alg="A128GCM")
 rpk = COSEKey.from_jwk(
     {
         "kty": "EC",
         "kid": "01",
         "crv": "P-256",
         "x": "usWxHK2PmfnHKwXPS54m0kTcGJ90UiglWiGahtagnv8",
         "y": "IBOL-C3BttVivg-lSreASjpkttcsz-1rb7btKLv8EX4",
     }
 )
 r = Recipient.new(
     protected={
-        1: -1,  # alg: "HPKE"
+        COSEHeaders.ALG: -1,  # alg: "HPKE"
     },
     unprotected={
-        4: b"01",  # kid: "01"
-        -4: [  # HPKE sender information
+        COSEHeaders.KID: b"01",  # kid: "01"
+        COSEHeaders.HPKE_SENDER_INFO: [  # HPKE sender information
             0x0010,  # kem: DHKEM(P-256, HKDF-SHA256)
             0x0001,  # kdf: HKDF-SHA256
             0x0001,  # aead: AES-128-GCM
         ],
     },
     recipient_key=rpk,
 )
 sender = COSE.new()
 encoded = sender.encode(
     b"This is the content.",
     enc_key,
     protected={
-        1: 1,  # alg: "A128GCM"
+        COSEHeaders.ALG: 1,  # alg: "A128GCM"
     },
     recipients=[r],
 )
 
 # The recipient side:
 rsk = COSEKey.from_jwk(
     {
@@ -1223,16 +1239,16 @@
 
 ```py
 import cwt
 from cwt import Claims, COSEKey
 
 try:
     key = COSEKey.generate_symmetric_key(alg="HS256", kid="01")
-    token = {"iss": "coaps://as.example", "sub": "dajiaji", "cti": "123"}, key)
-    decoded = decode(token, key)
+    token = cwt.encode({"iss": "coaps://as.example", "sub": "dajiaji", "cti": "123"}, key)
+    decoded = cwt.decode(token, key)
 
     # If you want to treat the result like a JWT;
     readable = Claims.new(decoded)
     assert readable.iss == 'coaps://as.example'
     assert readable.sub == 'dajiaji'
     assert readable.cti == '123'
     # readable.exp == 1620088759
@@ -1249,19 +1265,19 @@
     print(err)
 ```
 
 A raw CWT structure (Dict[int, Any]) can also be used as follows:
 
 ```py
 import cwt
-from cwt import COSEKey
+from cwt import COSEKey, CWTClaims
 
 key = COSEKey.generate_symmetric_key(alg="HS256", kid="01")
-token = cwt.encode({1: "coaps://as.example", 2: "dajiaji", 7: b"123"}, key)
-decoded = decode(token, key)
+token = cwt.encode({CWTClaims.ISS: "coaps://as.example", CWTClaims.SUB: "dajiaji", CWTClaims.CTI: b"123"}, key)
+decoded = cwt.decode(token, key)
 ```
 
 MAC algorithms other than `HS256` are listed in
 [Supported COSE Algorithms](https://python-cwt.readthedocs.io/en/stable/algorithms.html).
 
 ### Signed CWT
 
@@ -1277,22 +1293,22 @@
 ```py
 import cwt
 from cwt import COSEKey
 
 # The sender side:
 with open("./private_key.pem") as key_file:
     private_key = COSEKey.from_pem(key_file.read(), kid="01")
-token = encode(
+token = cwt.encode(
     {"iss": "coaps://as.example", "sub": "dajiaji", "cti": "123"}, private_key
 )
 
 # The recipient side:
 with open("./public_key.pem") as key_file:
     public_key = COSEKey.from_pem(key_file.read(), kid="01")
-decoded = decode(token, public_key)
+decoded = cwt.decode(token, public_key)
 ```
 
 JWKs can also be used instead of the PEM-formatted keys as follows:
 
 ```py
 import cwt
 from cwt import COSEKey
@@ -1303,43 +1319,43 @@
     "kty": "OKP",
     "key_ops": ["sign"],
     "alg": "EdDSA",
     "crv": "Ed25519",
     "x": "2E6dX83gqD_D0eAmqnaHe1TC1xuld6iAKXfw2OVATr0",
     "d": "L8JS08VsFZoZxGa9JvzYmCWOwg7zaKcei3KZmYsj7dc",
 })
-token =
+token = cwt.encode(
     {"iss": "coaps://as.example", "sub": "dajiaji", "cti": "123"}, private_key
 )
 
 # The recipient side:
 public_key = COSEKey.from_jwk({
     "kid": "01",
     "kty": "OKP",
     "key_ops": ["verify"],
     "crv": "Ed25519",
     "x": "2E6dX83gqD_D0eAmqnaHe1TC1xuld6iAKXfw2OVATr0",
 })
-decoded = decode(token, public_key)
+decoded = cwt.decode(token, public_key)
 ```
 
 Signing algorithms other than `Ed25519` are listed in
 [Supported COSE Algorithms](https://python-cwt.readthedocs.io/en/stable/algorithms.html).
 
 ### Encrypted CWT
 
 Create an encrypted CWT with `ChaCha20/Poly1305` and decrypt it as follows:
 
 ```py
 import cwt
 from cwt import COSEKey
 
 enc_key = COSEKey.generate_symmetric_key(alg="ChaCha20/Poly1305", kid="01")
-token = {"iss": "coaps://as.example", "sub": "dajiaji", "cti": "123"}, enc_key)
-decoded = decode(token, enc_key)
+token = cwt.encode({"iss": "coaps://as.example", "sub": "dajiaji", "cti": "123"}, enc_key)
+decoded = cwt.decode(token, enc_key)
 ```
 
 Encryption algorithms other than `ChaCha20/Poly1305` are listed in
 [Supported COSE Algorithms](https://python-cwt.readthedocs.io/en/stable/algorithms.html).
 
 ### Nested CWT
 
@@ -1351,25 +1367,25 @@
 
 # A shared encryption key.
 enc_key = COSEKey.generate_symmetric_key(alg="ChaCha20/Poly1305", kid="enc-01")
 
 # Creates a CWT with ES256 signing.
 with open("./private_key.pem") as key_file:
     private_key = COSEKey.from_pem(key_file.read(), kid="sig-01")
-token =
+token = cwt.encode(
     {"iss": "coaps://as.example", "sub": "dajiaji", "cti": "123"}, private_key
 )
 
 # Encrypts the signed CWT.
-nested = token, enc_key)
+nested = cwt.encode(token, enc_key)
 
 # Decrypts and verifies the nested CWT.
 with open("./public_key.pem") as key_file:
     public_key = COSEKey.from_pem(key_file.read(), kid="sig-01")
-decoded = decode(nested, [enc_key, public_key])
+decoded = cwt.decode(nested, [enc_key, public_key])
 ```
 
 ### CWT with User Settings
 
 The `cwt` in `cwt.encode()` and `cwt.decode()` above is a global `CWT` class instance created
 with default settings in advance. The default settings are as follows:
 - `expires_in`: `3600` seconds. This is the default lifetime in seconds of CWTs.
@@ -1378,48 +1394,48 @@
 If you want to change the settings, you can create your own `CWT` class instance as follows:
 
 ```py
 from cwt import COSEKey, CWT
 
 key = COSEKey.generate_symmetric_key(alg="HS256", kid="01")
 mycwt = CWT.new(expires_in=3600*24, leeway=10)
-token = my{"iss": "coaps://as.example", "sub": "dajiaji", "cti": "123"}, key)
-decoded = mydecode(token, key)
+token = mycwt.encode({"iss": "coaps://as.example", "sub": "dajiaji", "cti": "123"}, key)
+decoded = mycwt.decode(token, key)
 ```
 
 ### CWT with User-Defined Claims
 
 You can use your own claims as follows:
 
 Note that such user-defined claim's key should be less than -65536.
 
 ```py
 import cwt
-from cwt import COSEKey
+from cwt import COSEKey, CWTClaims
 
 # The sender side:
 with open("./private_key.pem") as key_file:
     private_key = COSEKey.from_pem(key_file.read(), kid="01")
-token =
+token = cwt.encode(
     {
-        1: "coaps://as.example",  # iss
-        2: "dajiaji",  # sub
-        7: b"123",  # cti
+        CWTClaims.ISS: "coaps://as.example",  # iss
+        CWTClaims.SUB: "dajiaji",  # sub
+        CWTClaims.CTI: b"123",  # cti
         -70001: "foo",
         -70002: ["bar"],
         -70003: {"baz": "qux"},
         -70004: 123,
     },
     private_key,
 )
 
 # The recipient side:
 with open("./public_key.pem") as key_file:
     public_key = COSEKey.from_pem(key_file.read(), kid="01")
-raw = decode(token, public_key)
+raw = cwt.decode(token, public_key)
 assert raw[-70001] == "foo"
 assert raw[-70002][0] == "bar"
 assert raw[-70003]["baz"] == "qux"
 assert raw[-70004] == 123
 
 readable = Claims.new(raw)
 assert readable.get(-70001) == "foo"
@@ -1441,15 +1457,15 @@
     "ext_1": -70001,
     "ext_2": -70002,
     "ext_3": -70003,
     "ext_4": -70004,
 }
 
 set_private_claim_names(my_claim_names)
-token =
+token = cwt.encode(
     {
         "iss": "coaps://as.example",
         "sub": "dajiaji",
         "cti": b"123",
         "ext_1": "foo",
         "ext_2": ["bar"],
         "ext_3": {"baz": "qux"},
@@ -1457,26 +1473,65 @@
     },
     private_key,
 )
 
 with open("./public_key.pem") as key_file:
     public_key = COSEKey.from_pem(key_file.read(), kid="01")
 
-raw = decode(token, public_key)
+raw = cwt.decode(token, public_key)
 readable = Claims.new(
     raw,
     private_claims_names=my_claim_names,
 )
 assert readable.get("ext_1") == "foo"
 assert readable.get("ext_2")[0] == "bar"
 assert readable.get("ext_3")["baz"] == "qux"
 assert readable.get("ext_4") == 123
 ```
 
 
+### CWT with CWT claims in COSE headers
+
+Python CWT supports [CWT Claims in COSE Headers](https://www.ietf.org/archive/id/draft-ietf-cose-cwt-claims-in-headers-05.html)  experimentally.
+
+If a CWT message has a CWT Claims header parameter in its protected header, `cwt.decode()` checks whether the values of the claims included in that parameter match the values of the corresponding claims in the payload. If they do not match, `VerifyError` is raised.
+
+```py
+from cwt import COSE, COSEHeaders, COSEKey, CWT, CWTClaims
+
+enc_key = COSEKey.from_symmetric_key(alg="A128GCM", kid="01")
+
+# The sender side:
+sender = COSE.new(alg_auto_inclusion=True, kid_auto_inclusion=True)
+payload = cbor2.dumps(
+    {
+        CWTClaims.ISS: "coap://as.example.com",
+        CWTClaims.SUB: "erikw",
+        CWTClaims.AUD: "coap://light.example.com",
+        CWTClaims.EXP: now() + 3600,
+        CWTClaims.NBF: now(),
+        CWTClaims.IAT: now(),
+        CWTClaims.CTI: bytes.fromhex("0b71"),
+    },
+)
+protected = {
+    COSEHeaders.CWT_CLAIMS: {  # 13
+        CWTClaims.ISS: "coap://as.example.com",
+    }
+}
+token = sender.encode(payload, enc_key, protected)
+
+# The recipient side:
+recipient = CWT.new()
+# `decode()` checks the validity of the CWT claims header parameter.
+decoded = recipient.decode(token, enc_key)
+assert decoded[CWTClaims.ISS] == "coap://as.example.com"
+assert decoded[CWTClaims.SUB] == "erikw"
+```
+
 ### CWT with PoP Key
 
 Python CWT supports [Proof-of-Possession Key Semantics for CBOR Web Tokens (CWTs)](https://tools.ietf.org/html/rfc8747).
 A CWT can include a PoP key as follows:
 
 On the issuer side:
 
@@ -1485,15 +1540,15 @@
 from cwt import COSEKey
 
 # Prepares a signing key for CWT in advance.
 with open("./private_key_of_issuer.pem") as key_file:
     private_key = COSEKey.from_pem(key_file.read(), kid="issuer-01")
 
 # Sets the PoP key to a CWT for the presenter.
-token =
+token = cwt.encode(
     {
         "iss": "coaps://as.example",
         "sub": "dajiaji",
         "cti": "123",
         "cnf": {
             "jwk": {  # Provided by the CWT presenter.
                 "kty": "OKP",
@@ -1537,15 +1592,15 @@
 from cwt import Claims, COSEKey
 
 # Prepares the public key of the issuer in advance.
 with open("./public_key_of_issuer.pem") as key_file:
     public_key = COSEKey.from_pem(key_file.read(), kid="issuer-01")
 
 # Verifies and decodes the CWT received from the presenter.
-raw = decode(token, public_key)
+raw = cwt.decode(token, public_key)
 decoded = Claims.new(raw)
 
 # Extracts the PoP key from the CWT.
 extracted_pop_key = COSEKey.new(decoded.cnf)  # = raw[8][1]
 
 # Then, verifies the message sent by the presenter
 # with the signature which is also sent by the presenter as follows:
@@ -1565,15 +1620,15 @@
 import cwt
 from cwt import Claims, COSEKey
 
 # The sernder side:
 with open("./private_key_of_cert.pem")) as f:
     private_key = COSEKey.from_pem(f.read(), kid="01")
 
-token =
+token = cwt.encode(
     {"iss": "coaps://as.example", "sub": "dajiaji", "cti": "123"}, private_key
 )
 
 # The recipient side:
 public_key = COSEKey.from_jwk(
     {
         "kty": "EC",
@@ -1616,15 +1671,15 @@
 # An EUDCC (EU Digital COVID Certificate) quoted from:
 # https://github.com/eu-digital-green-certificates/dgc-testdata/blob/main/AT/2DCode/raw/1.json
 eudcc = bytes.fromhex(
     "d2844da20448d919375fc1e7b6b20126a0590133a4041a61817ca0061a60942ea001624154390103a101a4617681aa62646e01626d616d4f52472d3130303033303231356276706a313131393334393030376264746a323032312d30322d313862636f624154626369783155524e3a555643493a30313a41543a31303830373834334639344145453045453530393346424332353442443831332342626d706c45552f312f32302f31353238626973781b4d696e6973747279206f66204865616c74682c20417573747269616273640262746769383430353339303036636e616da463666e74754d5553544552465241553c474f455353494e47455262666e754d7573746572667261752d47c3b6c39f696e67657263676e74684741425249454c4562676e684761627269656c656376657265312e302e3063646f626a313939382d30322d323658405812fce67cb84c3911d78e3f61f890d0c80eb9675806aebed66aa2d0d0c91d1fc98d7bcb80bf00e181806a9502e11b071325901bd0d2c1b6438747b8cc50f521"
 )
 
 public_key = load_pem_hcert_dsc(dsc)
-decoded = decode(eudcc, keys=[public_key])
+decoded = cwt.decode(eudcc, keys=[public_key])
 claims = Claims.new(decoded)
 # claims.hcert[1] ==
 # {
 #     'v': [
 #         {
 #             'dn': 1,
 #             'ma': 'ORG-100030215',
@@ -1670,14 +1725,15 @@
 - [RFC9338: CBOR Object Signing and Encryption (COSE): Countersignatures](https://www.rfc-editor.org/rfc/rfc9338.html) - experimental
 - [RFC8812: COSE and JOSE Registrations for Web Authentication (WebAuthn) Algorithms](https://tools.ietf.org/html/rfc8812)
 - [RFC8747: Proof-of-Possession Key Semantics for CBOR Web Tokens (CWTs)](https://tools.ietf.org/html/rfc8747)
 - [RFC8392: CWT (CBOR Web Token)](https://tools.ietf.org/html/rfc8392)
 - [RFC8230: Using RSA Algorithms with COSE Messages](https://tools.ietf.org/html/rfc8230)
 - [RFC8152: CBOR Object Signing and Encryption (COSE)](https://tools.ietf.org/html/rfc8152)
 - [draft-04: Use of HPKE with COSE](https://www.ietf.org/archive/id/draft-ietf-cose-hpke-04.html) - experimental
+- [draft-05: CWT Claims in COSE Headers](https://www.ietf.org/archive/id/draft-ietf-cose-cwt-claims-in-headers-05.html) - experimental
 - [Electronic Health Certificate Specification](https://github.com/ehn-dcc-development/hcert-spec/blob/main/hcert_spec.md)
 - [Technical Specifications for Digital Green Certificates Volume 1](https://ec.europa.eu/health/sites/default/files/ehealth/docs/digital-green-certificates_v1_en.pdf)
 
 ## Tests
 
 You can run tests from the project root after cloning with:
```

### Comparing `cwt-2.3.2/cwt/__init__.py` & `cwt-2.4.0/cwt/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,21 +8,21 @@
     encode,
     encode_and_encrypt,
     encode_and_mac,
     encode_and_sign,
     set_private_claim_names,
 )
 from .encrypted_cose_key import EncryptedCOSEKey
-from .enums import COSEType
+from .enums import COSEHeaders, COSETypes, CWTClaims
 from .exceptions import CWTError, DecodeError, EncodeError, VerifyError
 from .helpers.hcert import load_pem_hcert_dsc
 from .recipient import Recipient
 from .signer import Signer
 
-__version__ = "2.3.2"
+__version__ = "2.4.0"
 __title__ = "cwt"
 __description__ = "A Python implementation of CWT/COSE"
 __url__ = "https://python-cwt.readthedocs.io"
 __uri__ = __url__
 __doc__ = __description__ + " <" + __uri__ + ">"
 __author__ = "Ajitomi Daisuke"
 __email__ = "ajitomi@gmail.com"
@@ -33,19 +33,20 @@
     "encode_and_mac",
     "encode_and_sign",
     "encode_and_encrypt",
     "decode",
     "set_private_claim_names",
     "CWT",
     "COSE",
-    "COSEHeaders",
     "COSEKey",
     "COSEMessage",
     "COSESignature",
-    "COSEType",
+    "COSETypes",
+    "COSEHeaders",
+    "CWTClaims",
     "EncryptedCOSEKey",
     "HPKECipherSuite",
     "Claims",
     "Recipient",
     "Signer",
     "load_pem_hcert_dsc",
     "CWTError",
```

### Comparing `cwt-2.3.2/cwt/algs/asymmetric.py` & `cwt-2.4.0/cwt/algs/asymmetric.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/cwt/algs/ec2.py` & `cwt-2.4.0/cwt/algs/ec2.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/cwt/algs/okp.py` & `cwt-2.4.0/cwt/algs/okp.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/cwt/algs/raw.py` & `cwt-2.4.0/cwt/algs/raw.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/cwt/algs/rsa.py` & `cwt-2.4.0/cwt/algs/rsa.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/cwt/algs/symmetric.py` & `cwt-2.4.0/cwt/algs/symmetric.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/cwt/claims.py` & `cwt-2.4.0/cwt/claims.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/cwt/const.py` & `cwt-2.4.0/cwt/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from .enums import COSEType
+from .enums import COSETypes
 
 COSE_TAG_TO_TYPE = {
-    16: COSEType.ENCRYPT0,
-    96: COSEType.ENCRYPT,
-    17: COSEType.MAC0,
-    97: COSEType.MAC,
-    18: COSEType.SIGN1,
-    98: COSEType.SIGN,
-    19: COSEType.COUNTERSIGNATURE,
+    16: COSETypes.ENCRYPT0,
+    96: COSETypes.ENCRYPT,
+    17: COSETypes.MAC0,
+    97: COSETypes.MAC,
+    18: COSETypes.SIGN1,
+    98: COSETypes.SIGN,
+    19: COSETypes.COUNTERSIGNATURE,
 }
 
 COSE_TYPE_TO_TAG = {
-    COSEType.ENCRYPT0: 16,
-    COSEType.ENCRYPT: 96,
-    COSEType.MAC0: 17,
-    COSEType.MAC: 97,
-    COSEType.SIGN1: 18,
-    COSEType.SIGN: 98,
-    COSEType.COUNTERSIGNATURE: 19,
+    COSETypes.ENCRYPT0: 16,
+    COSETypes.ENCRYPT: 96,
+    COSETypes.MAC0: 17,
+    COSETypes.MAC: 97,
+    COSETypes.SIGN1: 18,
+    COSETypes.SIGN: 98,
+    COSETypes.COUNTERSIGNATURE: 19,
 }
 
 # Registered CWT Claims
 CWT_CLAIM_NAMES = {
     "hcert": -260,  # map
     "EUPHNonce": -259,  # bstr
     "EATMAROEPrefix": -258,  # bstr
```

### Comparing `cwt-2.3.2/cwt/cose.py` & `cwt-2.4.0/cwt/cose.py`

 * *Files 3% similar despite different names*

```diff
@@ -288,15 +288,15 @@
         self,
         data: Union[bytes, CBORTag],
         keys: Union[COSEKeyInterface, List[COSEKeyInterface]],
         context: Optional[Union[Dict[str, Any], List[Any]]] = None,
         external_aad: bytes = b"",
     ) -> bytes:
         """
-        Verifies and decodes COSE data.
+        Verifies and decodes COSE data, and returns only payload.
 
         Args:
             data (Union[bytes, CBORTag]): A byte string or cbor2.CBORTag of an
                 encoded data.
             keys (Union[COSEKeyInterface, List[COSEKeyInterface]]): COSE key(s)
                 to verify and decrypt the encoded data.
             context (Optional[Union[Dict[str, Any], List[Any]]]): A context information
@@ -306,14 +306,43 @@
         Returns:
             bytes: A byte string of decoded payload.
         Raises:
             ValueError: Invalid arguments.
             DecodeError: Failed to decode data.
             VerifyError: Failed to verify data.
         """
+        _, _, res = self.decode_with_headers(data, keys, context, external_aad)
+        return res
+
+    def decode_with_headers(
+        self,
+        data: Union[bytes, CBORTag],
+        keys: Union[COSEKeyInterface, List[COSEKeyInterface]],
+        context: Optional[Union[Dict[str, Any], List[Any]]] = None,
+        external_aad: bytes = b"",
+    ) -> Tuple[Dict[int, Any], Dict[int, Any], bytes]:
+        """
+        Verifies and decodes COSE data, and returns protected headers, unprotected headers and payload.
+
+        Args:
+            data (Union[bytes, CBORTag]): A byte string or cbor2.CBORTag of an
+                encoded data.
+            keys (Union[COSEKeyInterface, List[COSEKeyInterface]]): COSE key(s)
+                to verify and decrypt the encoded data.
+            context (Optional[Union[Dict[str, Any], List[Any]]]): A context information
+                structure for key deriviation functions.
+            external_aad(bytes): External additional authenticated data supplied by
+                application.
+        Returns:
+            Tuple[Dict[int, Any], Dict[int, Any], bytes]: A dictionary data of decoded protected headers, and a dictionary data of unprotected headers, and a byte string of decoded payload.
+        Raises:
+            ValueError: Invalid arguments.
+            DecodeError: Failed to decode data.
+            VerifyError: Failed to verify data.
+        """
         if isinstance(data, bytes):
             data = self._loads(data)
         if not isinstance(data, CBORTag):
             raise ValueError("Invalid COSE format.")
 
         if not isinstance(keys, list):
             if not isinstance(keys, COSEKeyInterface):
@@ -367,86 +396,86 @@
                         continue
                     try:
                         if not isinstance(p, bytes) and alg == -1:  # HPKE
                             hpke = HPKE(p, u, data.value[2])
                             res = hpke.decode(k, aad)
                             if not isinstance(res, bytes):
                                 raise TypeError("Internal type error.")
-                            return res
-                        return k.decrypt(data.value[2], nonce, aad)
+                            return p, u, res
+                        return p, u, k.decrypt(data.value[2], nonce, aad)
                     except Exception as e:
                         err = e
                 raise err
             for _, k in enumerate(keys):
                 try:
-                    return k.decrypt(data.value[2], nonce, aad)
+                    return p, u, k.decrypt(data.value[2], nonce, aad)
                 except Exception as e:
                     err = e
             raise err
 
         # Encrypt
         if data.tag == 96:
             rs = Recipients.from_list(data.value[3], self._verify_kid, context)
             nonce = u.get(5, b"")
             enc_key = rs.derive_key(keys, alg, external_aad, "Enc_Recipient")
             aad = self._dumps(["Encrypt", data.value[0], external_aad])
-            return enc_key.decrypt(data.value[2], nonce, aad)
+            return p, u, enc_key.decrypt(data.value[2], nonce, aad)
 
         # MAC0
         if data.tag == 17:
             kid = self._get_kid(p, u)
             msg = self._dumps(["MAC0", data.value[0], external_aad, data.value[2]])
             if kid:
                 for _, k in enumerate(keys):
                     if k.kid != kid:
                         continue
                     try:
                         k.verify(msg, data.value[3])
-                        return data.value[2]
+                        return p, u, data.value[2]
                     except Exception as e:
                         err = e
                 raise err
             for _, k in enumerate(keys):
                 try:
                     k.verify(msg, data.value[3])
-                    return data.value[2]
+                    return p, u, data.value[2]
                 except Exception as e:
                     err = e
             raise err
 
         # MAC
         if data.tag == 97:
             to_be_maced = self._dumps(["MAC", data.value[0], external_aad, data.value[2]])
             rs = Recipients.from_list(data.value[4], self._verify_kid, context)
             mac_auth_key = rs.derive_key(keys, alg, external_aad, "Mac_Recipient")
             mac_auth_key.verify(to_be_maced, data.value[3])
-            return data.value[2]
+            return p, u, data.value[2]
 
         # Signature1
         if data.tag == 18:
             kid = self._get_kid(p, u)
             to_be_signed = self._dumps(["Signature1", data.value[0], external_aad, data.value[2]])
             if kid:
                 for _, k in enumerate(keys):
                     if k.kid != kid:
                         continue
                     try:
                         if self._ca_certs:
                             k.validate_certificate(self._ca_certs)
                         k.verify(to_be_signed, data.value[3])
-                        return data.value[2]
+                        return p, u, data.value[2]
                     except Exception as e:
                         err = e
                 raise err
             for _, k in enumerate(keys):
                 try:
                     if self._ca_certs:
                         k.validate_certificate(self._ca_certs)
                     k.verify(to_be_signed, data.value[3])
-                    return data.value[2]
+                    return p, u, data.value[2]
                 except Exception as e:
                     err = e
             raise err
 
         # Signature
         # if data.tag == 98:
         sigs = data.value[3]
@@ -472,15 +501,15 @@
                                 data.value[0],
                                 sig[0],
                                 external_aad,
                                 data.value[2],
                             ]
                         )
                         k.verify(to_be_signed, sig[2])
-                        return data.value[2]
+                        return p, u, data.value[2]
                     except Exception as e:
                         err = e
                 continue
             for _, k in enumerate(keys):
                 try:
                     to_be_signed = self._dumps(
                         [
@@ -488,15 +517,15 @@
                             data.value[0],
                             sig[0],
                             external_aad,
                             data.value[2],
                         ]
                     )
                     k.verify(to_be_signed, sig[2])
-                    return data.value[2]
+                    return p, u, data.value[2]
                 except Exception as e:
                     err = e
         raise err
 
     def _encode_headers(
         self,
         key: Optional[COSEKeyInterface],
```

### Comparing `cwt-2.3.2/cwt/cose_key.py` & `cwt-2.4.0/cwt/cose_key.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/cwt/cose_key_interface.py` & `cwt-2.4.0/cwt/cose_key_interface.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/cwt/cose_message.py` & `cwt-2.4.0/cwt/cose_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from typing import Any, Dict, List, Optional, TypeVar
 
 from cbor2 import CBORTag, loads
 
 from .cbor_processor import CBORProcessor
 from .const import COSE_TAG_TO_TYPE, COSE_TYPE_TO_TAG
 from .cose_key_interface import COSEKeyInterface
-from .enums import COSEType
+from .enums import COSETypes
 from .signer import Signer
 
 Self = TypeVar("Self", bound="COSEMessage")
 
 
 class COSEMessage(CBORProcessor):
     """
     The COSE message.
     """
 
-    def __init__(self, type: COSEType, msg: List[Any]):
+    def __init__(self, type: COSETypes, msg: List[Any]):
         """
         Constructor.
 
         Args:
             type (List[Any]): A type of the COSE message.
             msg (List[Any]): A COSE message as a CBOR array.
         """
@@ -30,98 +30,98 @@
         self._protected = msg[0]
         self._unprotected = msg[1]
         self._payload = msg[2]
         self._otther_fields: List[bytes] = []
         self._recipients: List[List[Any]] = []
         self._signatures: List[List[Any]] = []
 
-        if self._type == COSEType.ENCRYPT0:
+        if self._type == COSETypes.ENCRYPT0:
             if len(self._msg) != 3:
                 raise ValueError("Invalid COSE_Encrypt0 message.")
 
-        elif self._type == COSEType.ENCRYPT:
+        elif self._type == COSETypes.ENCRYPT:
             if len(self._msg) != 4:
                 raise ValueError("Invalid COSE_Encrypt message.")
             if not isinstance(self._msg[3], list):
                 raise ValueError("The COSE recipients should be array.")
             for recipient in self._msg[3]:
                 self._validate_cose_message(recipient)
             self._recipients = self._msg[3]
 
-        elif self._type == COSEType.MAC0:
+        elif self._type == COSETypes.MAC0:
             if len(self._msg) != 4:
                 raise ValueError("Invalid COSE_Mac0 message.")
             if not isinstance(self._msg[3], bytes):
                 raise ValueError("tag should be bytes.")
             self._otther_fields = [self._msg[3]]  # tag
 
-        elif self._type == COSEType.MAC:
+        elif self._type == COSETypes.MAC:
             if len(self._msg) != 5:
                 raise ValueError("Invalid COSE_Mac message.")
             if not isinstance(self._msg[3], bytes):
                 raise ValueError("The tag value should be bytes.")
             self._otther_fields = [self._msg[3]]  # tag
             if not isinstance(self._msg[4], list):
                 raise ValueError("The COSE recipients should be array.")
             for recipient in self._msg[4]:
                 self._validate_cose_message(recipient)
             self._recipients = self._msg[4]
 
-        elif self._type == COSEType.SIGN1:
+        elif self._type == COSETypes.SIGN1:
             if len(self._msg) != 4:
                 raise ValueError("Invalid COSE_Sign1 message.")
             if not isinstance(self._msg[3], bytes):
                 raise ValueError("The COSE signature should be bytes.")
             self._otther_fields = [self._msg[3]]
 
-        elif self._type == COSEType.SIGN:
+        elif self._type == COSETypes.SIGN:
             if len(self._msg) != 4:
                 raise ValueError("Invalid COSE_Sign message.")
             if not isinstance(self._msg[3], list):
                 raise ValueError("The COSE signatures should be array.")
             for signature in self._msg[3]:
                 self._validate_cose_message(signature)
             self._signatures = self._msg[3]
 
-        elif self._type == COSEType.COUNTERSIGNATURE:
+        elif self._type == COSETypes.COUNTERSIGNATURE:
             if len(self._msg) != 3:
                 raise ValueError("Invalid COSE_Countersignature.")
 
-        elif self._type == COSEType.SIGNATURE:
+        elif self._type == COSETypes.SIGNATURE:
             if len(self._msg) != 3:
                 raise ValueError("Invalid COSE_Signature.")
 
-        elif self._type == COSEType.RECIPIENT:
+        elif self._type == COSETypes.RECIPIENT:
             if len(self._msg) != 3:
                 raise ValueError("Invalid COSE_Recipient.")
 
         else:
-            raise ValueError(f"Invalid COSEType({type}) for COSE message.")
+            raise ValueError(f"Invalid COSETypes({type}) for COSE message.")
         return
 
     @classmethod
     def loads(cls, msg: bytes):
         tagged = loads(msg)
         if not isinstance(tagged, CBORTag):
             raise ValueError("Invalid COSE format.")
         type = COSE_TAG_TO_TYPE.get(tagged.tag, None)
         if type is None:
             raise ValueError(f"Unknown CBOR tag for COSE message: {tagged.tag}.")
         return cls(type, tagged.value)
 
     @classmethod
     def from_cose_signature(cls, signature: List[Any]):
-        return cls(COSEType.SIGNATURE, signature)
+        return cls(COSETypes.SIGNATURE, signature)
 
     @classmethod
     def from_cose_recipient(cls, recipient: List[Any]):
-        return cls(COSEType.RECIPIENT, recipient)
+        return cls(COSETypes.RECIPIENT, recipient)
 
     @property
-    def type(self) -> COSEType:
+    def type(self) -> COSETypes:
         """
         The identifier of the key type.
         """
         return self._type
 
     @property
     def protected(self) -> Dict[int, Any]:
```

### Comparing `cwt-2.3.2/cwt/cwt.py` & `cwt-2.4.0/cwt/cwt.py`

 * *Files 2% similar despite different names*

```diff
@@ -333,19 +333,20 @@
             DecodeError: Failed to decode the CWT.
             VerifyError: Failed to verify the CWT.
         """
         cwt: Union[bytes, CBORTag, Dict[int, Any]] = self._loads(data)
         if isinstance(cwt, CBORTag) and cwt.tag == CWT.CBOR_TAG:
             cwt = cwt.value
         keys = [keys] if isinstance(keys, COSEKeyInterface) else keys
+        p: Dict[int, Any] = {}
         while isinstance(cwt, CBORTag):
-            cwt = self._cose.decode(cwt, keys)
+            p, u, cwt = self._cose.decode_with_headers(cwt, keys)
             cwt = self._loads(cwt)
         if not no_verify:
-            self._verify(cwt)
+            self._verify(cwt, p)
         return cwt
 
     def set_private_claim_names(self, claim_names: Dict[str, int]):
         """
         Sets private claim definitions. The definitions will be used in
         :func:`encode <cwt.CWT.encode>` when it is called with JSON-based claims.
 
@@ -394,15 +395,15 @@
                 raise ValueError("A bytes-formatted claims needs CBOR(COSE) Tag.")
             if nested.tag not in [16, 96, 17, 97, 18, 98]:
                 raise ValueError(f"Unsupported or unknown CBOR tag({nested.tag}).")
             return
         Claims.validate(claims)
         return
 
-    def _verify(self, claims: Union[Dict[int, Any], bytes]):
+    def _verify(self, claims: Union[Dict[int, Any], bytes], protected: Dict[int, Any] = {}):
         if not isinstance(claims, dict):
             raise DecodeError("Failed to decode.")
 
         now = timegm(datetime.now(tz=timezone.utc).utctimetuple())
         if 4 in claims:  # exp
             if isinstance(claims[4], int) or isinstance(claims[4], float):
                 if claims[4] < (now - self._leeway):
@@ -412,14 +413,19 @@
 
         if 5 in claims:  # nbf
             if isinstance(claims[5], int) or isinstance(claims[5], float):
                 if claims[5] > (now + self._leeway):
                     raise VerifyError("The token is not yet valid.")
             else:
                 raise ValueError("nbf should be int or float.")
+
+        if 13 in protected:  # CWT claims in protected headers
+            for k, v in protected[13].items():
+                if k in claims and claims[k] != v:
+                    raise VerifyError(f"The CWT claim({k}) value in protected header does not match the values in the payload.")
         return
 
     def _set_default_value(self, claims: Union[Dict[int, Any], bytes]):
         if isinstance(claims, bytes):
             return
         now = timegm(datetime.now(tz=timezone.utc).utctimetuple())
         if 4 not in claims:
```

### Comparing `cwt-2.3.2/cwt/encrypted_cose_key.py` & `cwt-2.4.0/cwt/encrypted_cose_key.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/cwt/helpers/hcert.py` & `cwt-2.4.0/cwt/helpers/hcert.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/cwt/recipient.py` & `cwt-2.4.0/cwt/recipient.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/cwt/recipient_algs/aes_key_wrap.py` & `cwt-2.4.0/cwt/recipient_algs/aes_key_wrap.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/cwt/recipient_algs/direct_hkdf.py` & `cwt-2.4.0/cwt/recipient_algs/direct_hkdf.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/cwt/recipient_algs/direct_key.py` & `cwt-2.4.0/cwt/recipient_algs/direct_key.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/cwt/recipient_algs/ecdh_aes_key_wrap.py` & `cwt-2.4.0/cwt/recipient_algs/ecdh_aes_key_wrap.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/cwt/recipient_algs/ecdh_direct_hkdf.py` & `cwt-2.4.0/cwt/recipient_algs/ecdh_direct_hkdf.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/cwt/recipient_algs/hpke.py` & `cwt-2.4.0/cwt/recipient_algs/hpke.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/cwt/recipient_interface.py` & `cwt-2.4.0/cwt/recipient_interface.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/cwt/recipients.py` & `cwt-2.4.0/cwt/recipients.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/cwt/signer.py` & `cwt-2.4.0/cwt/signer.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/cwt/utils.py` & `cwt-2.4.0/cwt/utils.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/docs/Makefile` & `cwt-2.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/docs/algorithms.rst` & `cwt-2.4.0/docs/algorithms.rst`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/docs/claims.rst` & `cwt-2.4.0/docs/claims.rst`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/docs/conf.py` & `cwt-2.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/docs/index.rst` & `cwt-2.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/poetry.lock` & `cwt-2.4.0/poetry.lock`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,49 @@
-# This file is automatically @generated by Poetry 1.4.1 and should not be changed by hand.
+# This file is automatically @generated by Poetry 1.5.1 and should not be changed by hand.
 
 [[package]]
 name = "alabaster"
 version = "0.7.13"
 description = "A configurable sidebar-enabled Sphinx theme"
-category = "main"
 optional = true
 python-versions = ">=3.6"
 files = [
     {file = "alabaster-0.7.13-py3-none-any.whl", hash = "sha256:1ee19aca801bbabb5ba3f5f258e4422dfa86f82f3e9cefb0859b283cdd7f62a3"},
     {file = "alabaster-0.7.13.tar.gz", hash = "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"},
 ]
 
 [[package]]
 name = "asn1crypto"
 version = "1.5.1"
 description = "Fast ASN.1 parser and serializer with definitions for private keys, public keys, certificates, CRL, OCSP, CMS, PKCS#3, PKCS#7, PKCS#8, PKCS#12, PKCS#5, X.509 and TSP"
-category = "main"
 optional = false
 python-versions = "*"
 files = [
     {file = "asn1crypto-1.5.1-py2.py3-none-any.whl", hash = "sha256:db4e40728b728508912cbb3d44f19ce188f218e9eba635821bb4b68564f8fd67"},
     {file = "asn1crypto-1.5.1.tar.gz", hash = "sha256:13ae38502be632115abf8a24cbe5f4da52e3b5231990aff31123c805306ccb9c"},
 ]
 
 [[package]]
 name = "babel"
 version = "2.12.1"
 description = "Internationalization utilities"
-category = "main"
 optional = true
 python-versions = ">=3.7"
 files = [
     {file = "Babel-2.12.1-py3-none-any.whl", hash = "sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610"},
     {file = "Babel-2.12.1.tar.gz", hash = "sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455"},
 ]
 
 [package.dependencies]
 pytz = {version = ">=2015.7", markers = "python_version < \"3.9\""}
 
 [[package]]
 name = "beautifulsoup4"
 version = "4.12.2"
 description = "Screen-scraping library"
-category = "main"
 optional = true
 python-versions = ">=3.6.0"
 files = [
     {file = "beautifulsoup4-4.12.2-py3-none-any.whl", hash = "sha256:bd2520ca0d9d7d12694a53d44ac482d181b4ec1888909b035a3dbf40d0f57d4a"},
     {file = "beautifulsoup4-4.12.2.tar.gz", hash = "sha256:492bbc69dca35d12daac71c4db1bfff0c876c00ef4a2ffacce226d4638eb72da"},
 ]
 
@@ -58,27 +54,25 @@
 html5lib = ["html5lib"]
 lxml = ["lxml"]
 
 [[package]]
 name = "cachetools"
 version = "5.3.1"
 description = "Extensible memoizing collections and decorators"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "cachetools-5.3.1-py3-none-any.whl", hash = "sha256:95ef631eeaea14ba2e36f06437f36463aac3a096799e876ee55e5cdccb102590"},
     {file = "cachetools-5.3.1.tar.gz", hash = "sha256:dce83f2d9b4e1f732a8cd44af8e8fab2dbe46201467fc98b3ef8f269092bf62b"},
 ]
 
 [[package]]
 name = "cbor2"
 version = "5.4.6"
 description = "CBOR (de)serializer with extensive tag support"
-category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "cbor2-5.4.6-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:309fffbb7f561d67f02095d4b9657b73c9220558701c997e9bfcfbca2696e927"},
     {file = "cbor2-5.4.6-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:ff95b33e5482313a74648ca3620c9328e9f30ecfa034df040b828e476597d352"},
     {file = "cbor2-5.4.6-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:db9eb582fce972f0fa429d8159b7891ff8deccb7affc4995090afc61ce0d328a"},
     {file = "cbor2-5.4.6-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:3950be57a1698086cf26d8710b4e5a637b65133c5b1f9eec23967d4089d8cfed"},
@@ -120,27 +114,25 @@
 doc = ["sphinx-autodoc-typehints (>=1.2.0)", "sphinx-rtd-theme"]
 test = ["pytest", "pytest-cov"]
 
 [[package]]
 name = "certifi"
 version = "2023.5.7"
 description = "Python package for providing Mozilla's CA Bundle."
-category = "main"
 optional = true
 python-versions = ">=3.6"
 files = [
     {file = "certifi-2023.5.7-py3-none-any.whl", hash = "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"},
     {file = "certifi-2023.5.7.tar.gz", hash = "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7"},
 ]
 
 [[package]]
 name = "certvalidator"
 version = "0.11.1"
 description = "Validates X.509 certificates and paths"
-category = "main"
 optional = false
 python-versions = "*"
 files = [
     {file = "certvalidator-0.11.1-py2.py3-none-any.whl", hash = "sha256:77520b269f516d4fb0902998d5bd0eb3727fe153b659aa1cb828dcf12ea6b8de"},
     {file = "certvalidator-0.11.1.tar.gz", hash = "sha256:922d141c94393ab285ca34338e18dd4093e3ae330b1f278e96c837cb62cffaad"},
 ]
 
@@ -148,15 +140,14 @@
 asn1crypto = ">=0.18.1"
 oscrypto = ">=0.16.1"
 
 [[package]]
 name = "cffi"
 version = "1.15.1"
 description = "Foreign Function Interface for Python calling C code."
-category = "main"
 optional = false
 python-versions = "*"
 files = [
     {file = "cffi-1.15.1-cp27-cp27m-macosx_10_9_x86_64.whl", hash = "sha256:a66d3508133af6e8548451b25058d5812812ec3798c886bf38ed24a98216fab2"},
     {file = "cffi-1.15.1-cp27-cp27m-manylinux1_i686.whl", hash = "sha256:470c103ae716238bbe698d67ad020e1db9d9dba34fa5a899b5e21577e6d52ed2"},
     {file = "cffi-1.15.1-cp27-cp27m-manylinux1_x86_64.whl", hash = "sha256:9ad5db27f9cabae298d151c85cf2bad1d359a1b9c686a275df03385758e2f914"},
     {file = "cffi-1.15.1-cp27-cp27m-win32.whl", hash = "sha256:b3bbeb01c2b273cca1e1e0c5df57f12dce9a4dd331b4fa1635b8bec26350bde3"},
@@ -225,39 +216,36 @@
 [package.dependencies]
 pycparser = "*"
 
 [[package]]
 name = "cfgv"
 version = "3.3.1"
 description = "Validate configuration and produce human readable error messages."
-category = "dev"
 optional = false
 python-versions = ">=3.6.1"
 files = [
     {file = "cfgv-3.3.1-py2.py3-none-any.whl", hash = "sha256:c6a0883f3917a037485059700b9e75da2464e6c27051014ad85ba6aaa5884426"},
     {file = "cfgv-3.3.1.tar.gz", hash = "sha256:f5a830efb9ce7a445376bb66ec94c638a9787422f96264c98edc6bdeed8ab736"},
 ]
 
 [[package]]
 name = "chardet"
 version = "5.1.0"
 description = "Universal encoding detector for Python 3"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "chardet-5.1.0-py3-none-any.whl", hash = "sha256:362777fb014af596ad31334fde1e8c327dfdb076e1960d1694662d46a6917ab9"},
     {file = "chardet-5.1.0.tar.gz", hash = "sha256:0d62712b956bc154f85fb0a266e2a3c5913c2967e00348701b32411d6def31e5"},
 ]
 
 [[package]]
 name = "charset-normalizer"
 version = "3.1.0"
 description = "The Real First Universal Charset Detector. Open, modern and actively maintained alternative to Chardet."
-category = "main"
 optional = true
 python-versions = ">=3.7.0"
 files = [
     {file = "charset-normalizer-3.1.0.tar.gz", hash = "sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5"},
     {file = "charset_normalizer-3.1.0-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b"},
     {file = "charset_normalizer-3.1.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60"},
     {file = "charset_normalizer-3.1.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1"},
@@ -334,27 +322,25 @@
     {file = "charset_normalizer-3.1.0-py3-none-any.whl", hash = "sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d"},
 ]
 
 [[package]]
 name = "colorama"
 version = "0.4.6"
 description = "Cross-platform colored terminal text."
-category = "main"
 optional = false
 python-versions = "!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,!=3.6.*,>=2.7"
 files = [
     {file = "colorama-0.4.6-py2.py3-none-any.whl", hash = "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"},
     {file = "colorama-0.4.6.tar.gz", hash = "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44"},
 ]
 
 [[package]]
 name = "coverage"
 version = "7.2.7"
 description = "Code coverage measurement for Python"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "coverage-7.2.7-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:d39b5b4f2a66ccae8b7263ac3c8170994b65266797fb96cbbfd3fb5b23921db8"},
     {file = "coverage-7.2.7-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:6d040ef7c9859bb11dfeb056ff5b3872436e3b5e401817d87a31e1750b9ae2fb"},
     {file = "coverage-7.2.7-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ba90a9563ba44a72fda2e85302c3abc71c5589cea608ca16c22b9804262aaeb6"},
     {file = "coverage-7.2.7-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:e7d9405291c6928619403db1d10bd07888888ec1abcbd9748fdaa971d7d661b2"},
@@ -422,15 +408,14 @@
 [package.extras]
 toml = ["tomli"]
 
 [[package]]
 name = "cryptography"
 version = "41.0.1"
 description = "cryptography is a package which provides cryptographic recipes and primitives to Python developers."
-category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "cryptography-41.0.1-cp37-abi3-macosx_10_12_universal2.whl", hash = "sha256:f73bff05db2a3e5974a6fd248af2566134d8981fd7ab012e5dd4ddb1d9a70699"},
     {file = "cryptography-41.0.1-cp37-abi3-macosx_10_12_x86_64.whl", hash = "sha256:1a5472d40c8f8e91ff7a3d8ac6dfa363d8e3138b961529c996f3e2df0c7a411a"},
     {file = "cryptography-41.0.1-cp37-abi3-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:7fa01527046ca5facdf973eef2535a27fec4cb651e4daec4d043ef63f6ecd4ca"},
     {file = "cryptography-41.0.1-cp37-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b46e37db3cc267b4dea1f56da7346c9727e1209aa98487179ee8ebed09d21e43"},
@@ -464,54 +449,50 @@
 test = ["pretend", "pytest (>=6.2.0)", "pytest-benchmark", "pytest-cov", "pytest-xdist"]
 test-randomorder = ["pytest-randomly"]
 
 [[package]]
 name = "distlib"
 version = "0.3.6"
 description = "Distribution utilities"
-category = "dev"
 optional = false
 python-versions = "*"
 files = [
     {file = "distlib-0.3.6-py2.py3-none-any.whl", hash = "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"},
     {file = "distlib-0.3.6.tar.gz", hash = "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46"},
 ]
 
 [[package]]
 name = "docutils"
 version = "0.18.1"
 description = "Docutils -- Python Documentation Utilities"
-category = "main"
 optional = true
 python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*"
 files = [
     {file = "docutils-0.18.1-py2.py3-none-any.whl", hash = "sha256:23010f129180089fbcd3bc08cfefccb3b890b0050e1ca00c867036e9d161b98c"},
     {file = "docutils-0.18.1.tar.gz", hash = "sha256:679987caf361a7539d76e584cbeddc311e3aee937877c87346f31debc63e9d06"},
 ]
 
 [[package]]
 name = "exceptiongroup"
 version = "1.1.1"
 description = "Backport of PEP 654 (exception groups)"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "exceptiongroup-1.1.1-py3-none-any.whl", hash = "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e"},
     {file = "exceptiongroup-1.1.1.tar.gz", hash = "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"},
 ]
 
 [package.extras]
 test = ["pytest (>=6)"]
 
 [[package]]
 name = "filelock"
 version = "3.12.2"
 description = "A platform independent file lock."
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "filelock-3.12.2-py3-none-any.whl", hash = "sha256:cbb791cdea2a72f23da6ac5b5269ab0a0d161e9ef0100e653b69049a7706d1ec"},
     {file = "filelock-3.12.2.tar.gz", hash = "sha256:002740518d8aa59a26b0c76e10fb8c6e15eae825d34b6fdf670333fd7b938d81"},
 ]
 
@@ -519,15 +500,14 @@
 docs = ["furo (>=2023.5.20)", "sphinx (>=7.0.1)", "sphinx-autodoc-typehints (>=1.23,!=1.23.4)"]
 testing = ["covdefaults (>=2.3)", "coverage (>=7.2.7)", "diff-cover (>=7.5)", "pytest (>=7.3.1)", "pytest-cov (>=4.1)", "pytest-mock (>=3.10)", "pytest-timeout (>=2.1)"]
 
 [[package]]
 name = "furo"
 version = "2023.5.20"
 description = "A clean customisable Sphinx documentation theme."
-category = "main"
 optional = true
 python-versions = ">=3.7"
 files = [
     {file = "furo-2023.5.20-py3-none-any.whl", hash = "sha256:594a8436ddfe0c071f3a9e9a209c314a219d8341f3f1af33fdf7c69544fab9e6"},
     {file = "furo-2023.5.20.tar.gz", hash = "sha256:40e09fa17c6f4b22419d122e933089226dcdb59747b5b6c79363089827dea16f"},
 ]
 
@@ -537,54 +517,50 @@
 sphinx = ">=6.0,<8.0"
 sphinx-basic-ng = "*"
 
 [[package]]
 name = "identify"
 version = "2.5.24"
 description = "File identification library for Python"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "identify-2.5.24-py2.py3-none-any.whl", hash = "sha256:986dbfb38b1140e763e413e6feb44cd731faf72d1909543178aa79b0e258265d"},
     {file = "identify-2.5.24.tar.gz", hash = "sha256:0aac67d5b4812498056d28a9a512a483f5085cc28640b02b258a59dac34301d4"},
 ]
 
 [package.extras]
 license = ["ukkonen"]
 
 [[package]]
 name = "idna"
 version = "3.4"
 description = "Internationalized Domain Names in Applications (IDNA)"
-category = "main"
 optional = true
 python-versions = ">=3.5"
 files = [
     {file = "idna-3.4-py3-none-any.whl", hash = "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"},
     {file = "idna-3.4.tar.gz", hash = "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4"},
 ]
 
 [[package]]
 name = "imagesize"
 version = "1.4.1"
 description = "Getting image size from png/jpeg/jpeg2000/gif file"
-category = "main"
 optional = true
 python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
 files = [
     {file = "imagesize-1.4.1-py2.py3-none-any.whl", hash = "sha256:0d8d18d08f840c19d0ee7ca1fd82490fdc3729b7ac93f49870406ddde8ef8d8b"},
     {file = "imagesize-1.4.1.tar.gz", hash = "sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a"},
 ]
 
 [[package]]
 name = "importlib-metadata"
 version = "6.7.0"
 description = "Read metadata from Python packages"
-category = "main"
 optional = true
 python-versions = ">=3.7"
 files = [
     {file = "importlib_metadata-6.7.0-py3-none-any.whl", hash = "sha256:cb52082e659e97afc5dac71e79de97d8681de3aa07ff18578330904a9d18e5b5"},
     {file = "importlib_metadata-6.7.0.tar.gz", hash = "sha256:1aaf550d4f73e5d6783e7acb77aec43d49da8017410afae93822cc9cca98c4d4"},
 ]
 
@@ -596,27 +572,25 @@
 perf = ["ipython"]
 testing = ["flufl.flake8", "importlib-resources (>=1.3)", "packaging", "pyfakefs", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-mypy (>=0.9.1)", "pytest-perf (>=0.9.2)", "pytest-ruff"]
 
 [[package]]
 name = "iniconfig"
 version = "2.0.0"
 description = "brain-dead simple config-ini parsing"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "iniconfig-2.0.0-py3-none-any.whl", hash = "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"},
     {file = "iniconfig-2.0.0.tar.gz", hash = "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3"},
 ]
 
 [[package]]
 name = "jinja2"
 version = "3.1.2"
 description = "A very fast and expressive template engine."
-category = "main"
 optional = true
 python-versions = ">=3.7"
 files = [
     {file = "Jinja2-3.1.2-py3-none-any.whl", hash = "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"},
     {file = "Jinja2-3.1.2.tar.gz", hash = "sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852"},
 ]
 
@@ -626,15 +600,14 @@
 [package.extras]
 i18n = ["Babel (>=2.7)"]
 
 [[package]]
 name = "markupsafe"
 version = "2.1.3"
 description = "Safely add untrusted strings to HTML/XML markup."
-category = "main"
 optional = true
 python-versions = ">=3.7"
 files = [
     {file = "MarkupSafe-2.1.3-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa"},
     {file = "MarkupSafe-2.1.3-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57"},
     {file = "MarkupSafe-2.1.3-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f"},
     {file = "MarkupSafe-2.1.3-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52"},
@@ -686,57 +659,53 @@
     {file = "MarkupSafe-2.1.3.tar.gz", hash = "sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad"},
 ]
 
 [[package]]
 name = "nodeenv"
 version = "1.8.0"
 description = "Node.js virtual environment builder"
-category = "dev"
 optional = false
 python-versions = ">=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,!=3.6.*"
 files = [
     {file = "nodeenv-1.8.0-py2.py3-none-any.whl", hash = "sha256:df865724bb3c3adc86b3876fa209771517b0cfe596beff01a92700e0e8be4cec"},
     {file = "nodeenv-1.8.0.tar.gz", hash = "sha256:d51e0c37e64fbf47d017feac3145cdbb58836d7eee8c6f6d3b6880c5456227d2"},
 ]
 
 [package.dependencies]
 setuptools = "*"
 
 [[package]]
 name = "oscrypto"
 version = "1.3.0"
 description = "TLS (SSL) sockets, key generation, encryption, decryption, signing, verification and KDFs using the OS crypto libraries. Does not require a compiler, and relies on the OS for patching. Works on Windows, OS X and Linux/BSD."
-category = "main"
 optional = false
 python-versions = "*"
 files = [
     {file = "oscrypto-1.3.0-py2.py3-none-any.whl", hash = "sha256:2b2f1d2d42ec152ca90ccb5682f3e051fb55986e1b170ebde472b133713e7085"},
     {file = "oscrypto-1.3.0.tar.gz", hash = "sha256:6f5fef59cb5b3708321db7cca56aed8ad7e662853351e7991fcf60ec606d47a4"},
 ]
 
 [package.dependencies]
 asn1crypto = ">=1.5.1"
 
 [[package]]
 name = "packaging"
 version = "23.1"
 description = "Core utilities for Python packages"
-category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "packaging-23.1-py3-none-any.whl", hash = "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61"},
     {file = "packaging-23.1.tar.gz", hash = "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"},
 ]
 
 [[package]]
 name = "platformdirs"
 version = "3.8.0"
 description = "A small Python package for determining appropriate platform-specific dirs, e.g. a \"user data dir\"."
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "platformdirs-3.8.0-py3-none-any.whl", hash = "sha256:ca9ed98ce73076ba72e092b23d3c93ea6c4e186b3f1c3dad6edd98ff6ffcca2e"},
     {file = "platformdirs-3.8.0.tar.gz", hash = "sha256:b0cabcb11063d21a0b261d557acb0a9d2126350e63b70cdf7db6347baea456dc"},
 ]
 
@@ -744,15 +713,14 @@
 docs = ["furo (>=2023.5.20)", "proselint (>=0.13)", "sphinx (>=7.0.1)", "sphinx-autodoc-typehints (>=1.23,!=1.23.4)"]
 test = ["appdirs (==1.4.4)", "covdefaults (>=2.3)", "pytest (>=7.3.1)", "pytest-cov (>=4.1)", "pytest-mock (>=3.10)"]
 
 [[package]]
 name = "pluggy"
 version = "1.2.0"
 description = "plugin and hook calling mechanisms for python"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "pluggy-1.2.0-py3-none-any.whl", hash = "sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849"},
     {file = "pluggy-1.2.0.tar.gz", hash = "sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3"},
 ]
 
@@ -760,15 +728,14 @@
 dev = ["pre-commit", "tox"]
 testing = ["pytest", "pytest-benchmark"]
 
 [[package]]
 name = "pre-commit"
 version = "3.3.3"
 description = "A framework for managing and maintaining multi-language pre-commit hooks."
-category = "dev"
 optional = false
 python-versions = ">=3.8"
 files = [
     {file = "pre_commit-3.3.3-py2.py3-none-any.whl", hash = "sha256:10badb65d6a38caff29703362271d7dca483d01da88f9d7e05d0b97171c136cb"},
     {file = "pre_commit-3.3.3.tar.gz", hash = "sha256:a2256f489cd913d575c145132ae196fe335da32d91a8294b7afe6622335dd023"},
 ]
 
@@ -779,42 +746,39 @@
 pyyaml = ">=5.1"
 virtualenv = ">=20.10.0"
 
 [[package]]
 name = "pycparser"
 version = "2.21"
 description = "C parser in Python"
-category = "main"
 optional = false
 python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
 files = [
     {file = "pycparser-2.21-py2.py3-none-any.whl", hash = "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9"},
     {file = "pycparser-2.21.tar.gz", hash = "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"},
 ]
 
 [[package]]
 name = "pygments"
 version = "2.15.1"
 description = "Pygments is a syntax highlighting package written in Python."
-category = "main"
 optional = true
 python-versions = ">=3.7"
 files = [
     {file = "Pygments-2.15.1-py3-none-any.whl", hash = "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"},
     {file = "Pygments-2.15.1.tar.gz", hash = "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c"},
 ]
 
 [package.extras]
 plugins = ["importlib-metadata"]
 
 [[package]]
 name = "pyhpke"
 version = "0.4.2"
 description = "A Python implementation of HPKE."
-category = "main"
 optional = false
 python-versions = ">=3.8,<4.0"
 files = [
     {file = "pyhpke-0.4.2-py3-none-any.whl", hash = "sha256:a2019c98fb31c6b45df1a55999e5bdeca7a87119f811ff7b3dd62892dfd569f7"},
     {file = "pyhpke-0.4.2.tar.gz", hash = "sha256:9a0ed17dbf5225ae31e7e5d105e64dbdb642cec73a1c28a94378f7f89f7bf378"},
 ]
 
@@ -824,15 +788,14 @@
 [package.extras]
 docs = ["Sphinx[docs] (>=4.3.2,<6.0.0)", "sphinx-autodoc-typehints[docs] (==1.21.0)", "sphinx-rtd-theme[docs] (>=1.0.0,<2.0.0)"]
 
 [[package]]
 name = "pyproject-api"
 version = "1.5.2"
 description = "API to interact with the python pyproject.toml based projects"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "pyproject_api-1.5.2-py3-none-any.whl", hash = "sha256:9cffcbfb64190f207444d7579d315f3278f2c04ba46d685fad93197b5326d348"},
     {file = "pyproject_api-1.5.2.tar.gz", hash = "sha256:999f58fa3c92b23ebd31a6bad5d1f87d456744d75e05391be7f5c729015d3d91"},
 ]
 
@@ -844,15 +807,14 @@
 docs = ["furo (>=2023.5.20)", "sphinx (>=7.0.1)", "sphinx-autodoc-typehints (>=1.23,!=1.23.4)"]
 testing = ["covdefaults (>=2.3)", "importlib-metadata (>=6.6)", "pytest (>=7.3.1)", "pytest-cov (>=4.1)", "pytest-mock (>=3.10)", "setuptools (>=67.8)", "wheel (>=0.40)"]
 
 [[package]]
 name = "pytest"
 version = "7.4.0"
 description = "pytest: simple powerful testing with Python"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "pytest-7.4.0-py3-none-any.whl", hash = "sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32"},
     {file = "pytest-7.4.0.tar.gz", hash = "sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a"},
 ]
 
@@ -867,15 +829,14 @@
 [package.extras]
 testing = ["argcomplete", "attrs (>=19.2.0)", "hypothesis (>=3.56)", "mock", "nose", "pygments (>=2.7.2)", "requests", "setuptools", "xmlschema"]
 
 [[package]]
 name = "pytest-cov"
 version = "4.1.0"
 description = "Pytest plugin for measuring coverage."
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "pytest-cov-4.1.0.tar.gz", hash = "sha256:3904b13dfbfec47f003b8e77fd5b589cd11904a21ddf1ab38a64f204d6a10ef6"},
     {file = "pytest_cov-4.1.0-py3-none-any.whl", hash = "sha256:6ba70b9e97e69fcc3fb45bfeab2d0a138fb65c4d0d6a41ef33983ad114be8c3a"},
 ]
 
@@ -886,27 +847,25 @@
 [package.extras]
 testing = ["fields", "hunter", "process-tests", "pytest-xdist", "six", "virtualenv"]
 
 [[package]]
 name = "pytz"
 version = "2023.3"
 description = "World timezone definitions, modern and historical"
-category = "main"
 optional = true
 python-versions = "*"
 files = [
     {file = "pytz-2023.3-py2.py3-none-any.whl", hash = "sha256:a151b3abb88eda1d4e34a9814df37de2a80e301e68ba0fd856fb9b46bfbbbffb"},
     {file = "pytz-2023.3.tar.gz", hash = "sha256:1d8ce29db189191fb55338ee6d0387d82ab59f3d00eac103412d64e0ebd0c588"},
 ]
 
 [[package]]
 name = "pyyaml"
 version = "6.0"
 description = "YAML parser and emitter for Python"
-category = "dev"
 optional = false
 python-versions = ">=3.6"
 files = [
     {file = "PyYAML-6.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:d4db7c7aef085872ef65a8fd7d6d09a14ae91f691dec3e87ee5ee0539d516f53"},
     {file = "PyYAML-6.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:9df7ed3b3d2e0ecfe09e14741b857df43adb5a3ddadc919a2d94fbdf78fea53c"},
     {file = "PyYAML-6.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:77f396e6ef4c73fdc33a9157446466f1cff553d979bd00ecb64385760c6babdc"},
     {file = "PyYAML-6.0-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:a80a78046a72361de73f8f395f1f1e49f956c6be882eed58505a15f3e430962b"},
@@ -948,15 +907,14 @@
     {file = "PyYAML-6.0.tar.gz", hash = "sha256:68fb519c14306fec9720a2a5b45bc9f0c8d1b9c72adf45c37baedfcd949c35a2"},
 ]
 
 [[package]]
 name = "requests"
 version = "2.31.0"
 description = "Python HTTP for Humans."
-category = "main"
 optional = true
 python-versions = ">=3.7"
 files = [
     {file = "requests-2.31.0-py3-none-any.whl", hash = "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f"},
     {file = "requests-2.31.0.tar.gz", hash = "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"},
 ]
 
@@ -970,15 +928,14 @@
 socks = ["PySocks (>=1.5.6,!=1.5.7)"]
 use-chardet-on-py3 = ["chardet (>=3.0.2,<6)"]
 
 [[package]]
 name = "setuptools"
 version = "68.0.0"
 description = "Easily download, build, install, upgrade, and uninstall Python packages"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "setuptools-68.0.0-py3-none-any.whl", hash = "sha256:11e52c67415a381d10d6b462ced9cfb97066179f0e871399e006c4ab101fc85f"},
     {file = "setuptools-68.0.0.tar.gz", hash = "sha256:baf1fdb41c6da4cd2eae722e135500da913332ab3f2f5c7d33af9b492acb5235"},
 ]
 
@@ -987,39 +944,36 @@
 testing = ["build[virtualenv]", "filelock (>=3.4.0)", "flake8-2020", "ini2toml[lite] (>=0.9)", "jaraco.envs (>=2.2)", "jaraco.path (>=3.2.0)", "pip (>=19.1)", "pip-run (>=8.8)", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-mypy (>=0.9.1)", "pytest-perf", "pytest-ruff", "pytest-timeout", "pytest-xdist", "tomli-w (>=1.0.0)", "virtualenv (>=13.0.0)", "wheel"]
 testing-integration = ["build[virtualenv]", "filelock (>=3.4.0)", "jaraco.envs (>=2.2)", "jaraco.path (>=3.2.0)", "pytest", "pytest-enabler", "pytest-xdist", "tomli", "virtualenv (>=13.0.0)", "wheel"]
 
 [[package]]
 name = "snowballstemmer"
 version = "2.2.0"
 description = "This package provides 29 stemmers for 28 languages generated from Snowball algorithms."
-category = "main"
 optional = true
 python-versions = "*"
 files = [
     {file = "snowballstemmer-2.2.0-py2.py3-none-any.whl", hash = "sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a"},
     {file = "snowballstemmer-2.2.0.tar.gz", hash = "sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1"},
 ]
 
 [[package]]
 name = "soupsieve"
 version = "2.4.1"
 description = "A modern CSS selector implementation for Beautiful Soup."
-category = "main"
 optional = true
 python-versions = ">=3.7"
 files = [
     {file = "soupsieve-2.4.1-py3-none-any.whl", hash = "sha256:1c1bfee6819544a3447586c889157365a27e10d88cde3ad3da0cf0ddf646feb8"},
     {file = "soupsieve-2.4.1.tar.gz", hash = "sha256:89d12b2d5dfcd2c9e8c22326da9d9aa9cb3dfab0a83a024f05704076ee8d35ea"},
 ]
 
 [[package]]
 name = "sphinx"
 version = "6.2.1"
 description = "Python documentation generator"
-category = "main"
 optional = true
 python-versions = ">=3.8"
 files = [
     {file = "Sphinx-6.2.1.tar.gz", hash = "sha256:6d56a34697bb749ffa0152feafc4b19836c755d90a7c59b72bc7dfd371b9cc6b"},
     {file = "sphinx-6.2.1-py3-none-any.whl", hash = "sha256:97787ff1fa3256a3eef9eda523a63dbf299f7b47e053cfcf684a1c2a8380c912"},
 ]
 
@@ -1048,15 +1002,14 @@
 lint = ["docutils-stubs", "flake8 (>=3.5.0)", "flake8-simplify", "isort", "mypy (>=0.990)", "ruff", "sphinx-lint", "types-requests"]
 test = ["cython", "filelock", "html5lib", "pytest (>=4.6)"]
 
 [[package]]
 name = "sphinx-autodoc-typehints"
 version = "1.22"
 description = "Type hints (PEP 484) support for the Sphinx autodoc extension"
-category = "main"
 optional = true
 python-versions = ">=3.7"
 files = [
     {file = "sphinx_autodoc_typehints-1.22-py3-none-any.whl", hash = "sha256:ef4a8b9d52de66065aa7d3adfabf5a436feb8a2eff07c2ddc31625d8807f2b69"},
     {file = "sphinx_autodoc_typehints-1.22.tar.gz", hash = "sha256:71fca2d5eee9b034204e4c686ab20b4d8f5eb9409396216bcae6c87c38e18ea6"},
 ]
 
@@ -1072,39 +1025,33 @@
 testing = ["covdefaults (>=2.2.2)", "coverage (>=7.0.5)", "diff-cover (>=7.3)", "nptyping (>=2.4.1)", "pytest (>=7.2.1)", "pytest-cov (>=4)", "sphobjinv (>=2.3.1)", "typing-extensions (>=4.4)"]
 type-comment = ["typed-ast (>=1.5.4)"]
 
 [[package]]
 name = "sphinx-autodoc-typehints"
 version = "1.23.0"
 description = "Type hints (PEP 484) support for the Sphinx autodoc extension"
-category = "main"
 optional = true
 python-versions = ">=3.7"
 files = [
     {file = "sphinx_autodoc_typehints-1.23.0-py3-none-any.whl", hash = "sha256:ac099057e66b09e51b698058ba7dd76e57e1fe696cd91b54e121d3dad188f91d"},
     {file = "sphinx_autodoc_typehints-1.23.0.tar.gz", hash = "sha256:5d44e2996633cdada499b6d27a496ddf9dbc95dd1f0f09f7b37940249e61f6e9"},
 ]
 
 [package.dependencies]
-furo = {version = ">=2022.12.7", optional = true, markers = "extra == \"docs\""}
-sphinx = [
-    {version = ">=5.3"},
-    {version = ">=6.1.3", optional = true, markers = "extra == \"docs\""},
-]
+sphinx = ">=5.3"
 
 [package.extras]
 docs = ["furo (>=2022.12.7)", "sphinx (>=6.1.3)", "sphinx-autodoc-typehints (>=1.23.4)"]
 testing = ["covdefaults (>=2.2.2)", "coverage (>=7.2.2)", "diff-cover (>=7.5)", "nptyping (>=2.5)", "pytest (>=7.2.2)", "pytest-cov (>=4)", "sphobjinv (>=2.3.1)", "typing-extensions (>=4.5)"]
 type-comment = ["typed-ast (>=1.5.4)"]
 
 [[package]]
 name = "sphinx-basic-ng"
 version = "1.0.0b1"
 description = "A modern skeleton for Sphinx themes."
-category = "main"
 optional = true
 python-versions = ">=3.7"
 files = [
     {file = "sphinx_basic_ng-1.0.0b1-py3-none-any.whl", hash = "sha256:ade597a3029c7865b24ad0eda88318766bcc2f9f4cef60df7e28126fde94db2a"},
     {file = "sphinx_basic_ng-1.0.0b1.tar.gz", hash = "sha256:89374bd3ccd9452a301786781e28c8718e99960f2d4f411845ea75fc7bb5a9b0"},
 ]
 
@@ -1114,15 +1061,14 @@
 [package.extras]
 docs = ["furo", "ipython", "myst-parser", "sphinx-copybutton", "sphinx-inline-tabs"]
 
 [[package]]
 name = "sphinx-rtd-theme"
 version = "1.2.2"
 description = "Read the Docs theme for Sphinx"
-category = "main"
 optional = true
 python-versions = "!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,>=2.7"
 files = [
     {file = "sphinx_rtd_theme-1.2.2-py2.py3-none-any.whl", hash = "sha256:6a7e7d8af34eb8fc57d52a09c6b6b9c46ff44aea5951bc831eeb9245378f3689"},
     {file = "sphinx_rtd_theme-1.2.2.tar.gz", hash = "sha256:01c5c5a72e2d025bd23d1f06c59a4831b06e6ce6c01fdd5ebfe9986c0a880fc7"},
 ]
 
@@ -1134,15 +1080,14 @@
 [package.extras]
 dev = ["bump2version", "sphinxcontrib-httpdomain", "transifex-client", "wheel"]
 
 [[package]]
 name = "sphinxcontrib-applehelp"
 version = "1.0.4"
 description = "sphinxcontrib-applehelp is a Sphinx extension which outputs Apple help books"
-category = "main"
 optional = true
 python-versions = ">=3.8"
 files = [
     {file = "sphinxcontrib-applehelp-1.0.4.tar.gz", hash = "sha256:828f867945bbe39817c210a1abfd1bc4895c8b73fcaade56d45357a348a07d7e"},
     {file = "sphinxcontrib_applehelp-1.0.4-py3-none-any.whl", hash = "sha256:29d341f67fb0f6f586b23ad80e072c8e6ad0b48417db2bde114a4c9746feb228"},
 ]
 
@@ -1150,15 +1095,14 @@
 lint = ["docutils-stubs", "flake8", "mypy"]
 test = ["pytest"]
 
 [[package]]
 name = "sphinxcontrib-devhelp"
 version = "1.0.2"
 description = "sphinxcontrib-devhelp is a sphinx extension which outputs Devhelp document."
-category = "main"
 optional = true
 python-versions = ">=3.5"
 files = [
     {file = "sphinxcontrib-devhelp-1.0.2.tar.gz", hash = "sha256:ff7f1afa7b9642e7060379360a67e9c41e8f3121f2ce9164266f61b9f4b338e4"},
     {file = "sphinxcontrib_devhelp-1.0.2-py2.py3-none-any.whl", hash = "sha256:8165223f9a335cc1af7ffe1ed31d2871f325254c0423bc0c4c7cd1c1e4734a2e"},
 ]
 
@@ -1166,15 +1110,14 @@
 lint = ["docutils-stubs", "flake8", "mypy"]
 test = ["pytest"]
 
 [[package]]
 name = "sphinxcontrib-htmlhelp"
 version = "2.0.1"
 description = "sphinxcontrib-htmlhelp is a sphinx extension which renders HTML help files"
-category = "main"
 optional = true
 python-versions = ">=3.8"
 files = [
     {file = "sphinxcontrib-htmlhelp-2.0.1.tar.gz", hash = "sha256:0cbdd302815330058422b98a113195c9249825d681e18f11e8b1f78a2f11efff"},
     {file = "sphinxcontrib_htmlhelp-2.0.1-py3-none-any.whl", hash = "sha256:c38cb46dccf316c79de6e5515e1770414b797162b23cd3d06e67020e1d2a6903"},
 ]
 
@@ -1182,45 +1125,42 @@
 lint = ["docutils-stubs", "flake8", "mypy"]
 test = ["html5lib", "pytest"]
 
 [[package]]
 name = "sphinxcontrib-jquery"
 version = "4.1"
 description = "Extension to include jQuery on newer Sphinx releases"
-category = "main"
 optional = true
 python-versions = ">=2.7"
 files = [
     {file = "sphinxcontrib-jquery-4.1.tar.gz", hash = "sha256:1620739f04e36a2c779f1a131a2dfd49b2fd07351bf1968ced074365933abc7a"},
     {file = "sphinxcontrib_jquery-4.1-py2.py3-none-any.whl", hash = "sha256:f936030d7d0147dd026a4f2b5a57343d233f1fc7b363f68b3d4f1cb0993878ae"},
 ]
 
 [package.dependencies]
 Sphinx = ">=1.8"
 
 [[package]]
 name = "sphinxcontrib-jsmath"
 version = "1.0.1"
 description = "A sphinx extension which renders display math in HTML via JavaScript"
-category = "main"
 optional = true
 python-versions = ">=3.5"
 files = [
     {file = "sphinxcontrib-jsmath-1.0.1.tar.gz", hash = "sha256:a9925e4a4587247ed2191a22df5f6970656cb8ca2bd6284309578f2153e0c4b8"},
     {file = "sphinxcontrib_jsmath-1.0.1-py2.py3-none-any.whl", hash = "sha256:2ec2eaebfb78f3f2078e73666b1415417a116cc848b72e5172e596c871103178"},
 ]
 
 [package.extras]
 test = ["flake8", "mypy", "pytest"]
 
 [[package]]
 name = "sphinxcontrib-qthelp"
 version = "1.0.3"
 description = "sphinxcontrib-qthelp is a sphinx extension which outputs QtHelp document."
-category = "main"
 optional = true
 python-versions = ">=3.5"
 files = [
     {file = "sphinxcontrib-qthelp-1.0.3.tar.gz", hash = "sha256:4c33767ee058b70dba89a6fc5c1892c0d57a54be67ddd3e7875a18d14cba5a72"},
     {file = "sphinxcontrib_qthelp-1.0.3-py2.py3-none-any.whl", hash = "sha256:bd9fc24bcb748a8d51fd4ecaade681350aa63009a347a8c14e637895444dfab6"},
 ]
 
@@ -1228,15 +1168,14 @@
 lint = ["docutils-stubs", "flake8", "mypy"]
 test = ["pytest"]
 
 [[package]]
 name = "sphinxcontrib-serializinghtml"
 version = "1.1.5"
 description = "sphinxcontrib-serializinghtml is a sphinx extension which outputs \"serialized\" HTML files (json and pickle)."
-category = "main"
 optional = true
 python-versions = ">=3.5"
 files = [
     {file = "sphinxcontrib-serializinghtml-1.1.5.tar.gz", hash = "sha256:aa5f6de5dfdf809ef505c4895e51ef5c9eac17d0f287933eb49ec495280b6952"},
     {file = "sphinxcontrib_serializinghtml-1.1.5-py2.py3-none-any.whl", hash = "sha256:352a9a00ae864471d3a7ead8d7d79f5fc0b57e8b3f95e9867eb9eb28999b92fd"},
 ]
 
@@ -1244,15 +1183,14 @@
 lint = ["docutils-stubs", "flake8", "mypy"]
 test = ["pytest"]
 
 [[package]]
 name = "sphinxcontrib-websupport"
 version = "1.2.4"
 description = "Sphinx API for Web Apps"
-category = "main"
 optional = true
 python-versions = ">=3.5"
 files = [
     {file = "sphinxcontrib-websupport-1.2.4.tar.gz", hash = "sha256:4edf0223a0685a7c485ae5a156b6f529ba1ee481a1417817935b20bde1956232"},
     {file = "sphinxcontrib_websupport-1.2.4-py2.py3-none-any.whl", hash = "sha256:6fc9287dfc823fe9aa432463edd6cea47fa9ebbf488d7f289b322ffcfca075c7"},
 ]
 
@@ -1263,55 +1201,52 @@
 lint = ["flake8"]
 test = ["Sphinx", "pytest", "sqlalchemy", "whoosh"]
 
 [[package]]
 name = "tomli"
 version = "2.0.1"
 description = "A lil' TOML parser"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "tomli-2.0.1-py3-none-any.whl", hash = "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc"},
     {file = "tomli-2.0.1.tar.gz", hash = "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"},
 ]
 
 [[package]]
 name = "tox"
-version = "4.6.3"
+version = "4.6.4"
 description = "tox is a generic virtualenv management and test command line tool"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "tox-4.6.3-py3-none-any.whl", hash = "sha256:2946a0bb38924c3a9f9575c7fb4ca1f4c11a7c69c61592f176778892155cb50c"},
-    {file = "tox-4.6.3.tar.gz", hash = "sha256:9e2c5091a117d03b583c57c4c40aecd068099c17d40520e7b165e85c19334534"},
+    {file = "tox-4.6.4-py3-none-any.whl", hash = "sha256:1b8f8ae08d6a5475cad9d508236c51ea060620126fd7c3c513d0f5c7f29cc776"},
+    {file = "tox-4.6.4.tar.gz", hash = "sha256:5e2ad8845764706170d3dcaac171704513cc8a725655219acb62fe4380bdadda"},
 ]
 
 [package.dependencies]
 cachetools = ">=5.3.1"
 chardet = ">=5.1"
 colorama = ">=0.4.6"
 filelock = ">=3.12.2"
 packaging = ">=23.1"
-platformdirs = ">=3.5.3"
-pluggy = ">=1"
+platformdirs = ">=3.8"
+pluggy = ">=1.2"
 pyproject-api = ">=1.5.2"
 tomli = {version = ">=2.0.1", markers = "python_version < \"3.11\""}
 virtualenv = ">=20.23.1"
 
 [package.extras]
-docs = ["furo (>=2023.5.20)", "sphinx (>=7.0.1)", "sphinx-argparse-cli (>=1.11.1)", "sphinx-autodoc-typehints (>=1.23.2,!=1.23.4)", "sphinx-copybutton (>=0.5.2)", "sphinx-inline-tabs (>=2023.4.21)", "sphinxcontrib-towncrier (>=0.2.1a0)", "towncrier (>=23.6)"]
-testing = ["build[virtualenv] (>=0.10)", "covdefaults (>=2.3)", "detect-test-pollution (>=1.1.1)", "devpi-process (>=0.3.1)", "diff-cover (>=7.6)", "distlib (>=0.3.6)", "flaky (>=3.7)", "hatch-vcs (>=0.3)", "hatchling (>=1.17.1)", "psutil (>=5.9.5)", "pytest (>=7.3.2)", "pytest-cov (>=4.1)", "pytest-mock (>=3.11.1)", "pytest-xdist (>=3.3.1)", "re-assert (>=1.1)", "time-machine (>=2.10)", "wheel (>=0.40)"]
+docs = ["furo (>=2023.5.20)", "sphinx (>=7.0.1)", "sphinx-argparse-cli (>=1.11.1)", "sphinx-autodoc-typehints (>=1.23.3,!=1.23.4)", "sphinx-copybutton (>=0.5.2)", "sphinx-inline-tabs (>=2023.4.21)", "sphinxcontrib-towncrier (>=0.2.1a0)", "towncrier (>=23.6)"]
+testing = ["build[virtualenv] (>=0.10)", "covdefaults (>=2.3)", "detect-test-pollution (>=1.1.1)", "devpi-process (>=0.3.1)", "diff-cover (>=7.6)", "distlib (>=0.3.6)", "flaky (>=3.7)", "hatch-vcs (>=0.3)", "hatchling (>=1.17.1)", "psutil (>=5.9.5)", "pytest (>=7.4)", "pytest-cov (>=4.1)", "pytest-mock (>=3.11.1)", "pytest-xdist (>=3.3.1)", "re-assert (>=1.1)", "time-machine (>=2.10)", "wheel (>=0.40)"]
 
 [[package]]
 name = "urllib3"
 version = "2.0.3"
 description = "HTTP library with thread-safe connection pooling, file post, and more."
-category = "main"
 optional = true
 python-versions = ">=3.7"
 files = [
     {file = "urllib3-2.0.3-py3-none-any.whl", hash = "sha256:48e7fafa40319d358848e1bc6809b208340fafe2096f1725d05d67443d0483d1"},
     {file = "urllib3-2.0.3.tar.gz", hash = "sha256:bee28b5e56addb8226c96f7f13ac28cb4c301dd5ea8a6ca179c0b9835e032825"},
 ]
 
@@ -1321,15 +1256,14 @@
 socks = ["pysocks (>=1.5.6,!=1.5.7,<2.0)"]
 zstd = ["zstandard (>=0.18.0)"]
 
 [[package]]
 name = "virtualenv"
 version = "20.23.1"
 description = "Virtual Python Environment builder"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "virtualenv-20.23.1-py3-none-any.whl", hash = "sha256:34da10f14fea9be20e0fd7f04aba9732f84e593dac291b757ce42e3368a39419"},
     {file = "virtualenv-20.23.1.tar.gz", hash = "sha256:8ff19a38c1021c742148edc4f81cb43d7f8c6816d2ede2ab72af5b84c749ade1"},
 ]
 
@@ -1342,15 +1276,14 @@
 docs = ["furo (>=2023.5.20)", "proselint (>=0.13)", "sphinx (>=7.0.1)", "sphinx-argparse (>=0.4)", "sphinxcontrib-towncrier (>=0.2.1a0)", "towncrier (>=23.6)"]
 test = ["covdefaults (>=2.3)", "coverage (>=7.2.7)", "coverage-enable-subprocess (>=1)", "flaky (>=3.7)", "packaging (>=23.1)", "pytest (>=7.3.1)", "pytest-env (>=0.8.1)", "pytest-freezer (>=0.4.6)", "pytest-mock (>=3.10)", "pytest-randomly (>=3.12)", "pytest-timeout (>=2.1)", "setuptools (>=67.8)", "time-machine (>=2.9)"]
 
 [[package]]
 name = "zipp"
 version = "3.15.0"
 description = "Backport of pathlib-compatible object wrapper for zip files"
-category = "main"
 optional = true
 python-versions = ">=3.7"
 files = [
     {file = "zipp-3.15.0-py3-none-any.whl", hash = "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"},
     {file = "zipp-3.15.0.tar.gz", hash = "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b"},
 ]
 
@@ -1360,8 +1293,8 @@
 
 [extras]
 docs = ["Sphinx", "sphinx-autodoc-typehints", "sphinx-rtd-theme"]
 
 [metadata]
 lock-version = "2.0"
 python-versions = "^3.8"
-content-hash = "c2288f1bcc927ab7b80513ac6d75e76aa00adad0b172fd49bd89e86736579732"
+content-hash = "e0a4dee0cf52d5e1880205c220be36d3b86303a115055fd65bd4687d7999de71"
```

### Comparing `cwt-2.3.2/pyproject.toml` & `cwt-2.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cwt"
-version = "2.3.2"
+version = "2.4.0"
 description = "A Python implementation of CWT/COSE."
 authors = ["Ajitomi Daisuke <dajiaji@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dajiaji/python-cwt"
 
 include = [
@@ -41,12 +41,12 @@
   "sphinx-autodoc-typehints",
   "sphinx-rtd-theme",
 ]
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.4"
 pytest-cov = "^4.1.0"
-tox = "^4.6.3"
+tox = "^4.6.4"
 pre-commit = "^3.3.3"
 
 [tool.mypy]
 ignore_missing_imports = true
```

### Comparing `cwt-2.3.2/samples/eudcc/swedish_verifier.py` & `cwt-2.4.0/samples/eudcc/swedish_verifier.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/samples/eudcc/verifier.py` & `cwt-2.4.0/samples/eudcc/verifier.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/tests/keys/cacert.pem` & `cwt-2.4.0/tests/keys/cacert.pem`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/tests/keys/cacert_2.pem` & `cwt-2.4.0/tests/keys/cacert_2.pem`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/tests/keys/cakey.pem` & `cwt-2.4.0/tests/keys/cakey.pem`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/tests/keys/cert_es256.json` & `cwt-2.4.0/tests/keys/cert_es256.json`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/tests/keys/cert_es256.pem` & `cwt-2.4.0/tests/keys/cert_es256.pem`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/tests/keys/cert_es256_2.json` & `cwt-2.4.0/tests/keys/cert_es256_2.json`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/tests/keys/hcert_testdata_cert_at.pem` & `cwt-2.4.0/tests/keys/hcert_testdata_cert_at.pem`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/tests/keys/private_key_rsa.json` & `cwt-2.4.0/tests/keys/private_key_rsa.json`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/tests/keys/private_key_rsa.pem` & `cwt-2.4.0/tests/keys/private_key_rsa.pem`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/tests/test_algs_aes_key_wrap.py` & `cwt-2.4.0/tests/test_algs_aes_key_wrap.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/tests/test_algs_ec2.py` & `cwt-2.4.0/tests/test_algs_ec2.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/tests/test_algs_okp.py` & `cwt-2.4.0/tests/test_algs_okp.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/tests/test_algs_raw.py` & `cwt-2.4.0/tests/test_algs_raw.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/tests/test_algs_rsa.py` & `cwt-2.4.0/tests/test_algs_rsa.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/tests/test_algs_symmetric.py` & `cwt-2.4.0/tests/test_algs_symmetric.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/tests/test_claims.py` & `cwt-2.4.0/tests/test_claims.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/tests/test_cose.py` & `cwt-2.4.0/tests/test_cose.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/tests/test_cose_hpke.py` & `cwt-2.4.0/tests/test_cose_hpke.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/tests/test_cose_key.py` & `cwt-2.4.0/tests/test_cose_key.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/tests/test_cose_message.py` & `cwt-2.4.0/tests/test_cose_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 """
 Tests for COSEMessage.
 """
 
 import cbor2
 import pytest
 
-from cwt import COSE, COSEKey, COSEMessage, COSEType, Recipient, Signer, VerifyError
+from cwt import COSE, COSEKey, COSEMessage, COSETypes, Recipient, Signer, VerifyError
 
 
 class TestCOSEMessage:
     """
     Tests for COSEMessage.
     """
 
     def test_cose_message_constructor_with_mac0(self):
         mac_key = COSEKey.generate_symmetric_key(alg="HS256", kid="01")
         sender = COSE.new(alg_auto_inclusion=True, kid_auto_inclusion=True)
         encoded = sender.encode(b"Hello world!", mac_key)
         sig = COSEMessage.loads(encoded)
-        assert sig.type == COSEType.MAC0
+        assert sig.type == COSETypes.MAC0
         assert sig.payload == b"Hello world!"
         assert sig.signatures == []
         assert sig.recipients == []
         assert len(sig.other_fields) == 1
 
     def test_cose_message_mac0_countersignature(self):
         mac_key = COSEKey.generate_symmetric_key(alg="HS256", kid="01")
@@ -299,40 +299,40 @@
         countersignature = COSEMessage.from_cose_signature(sig)
         assert countersignature.protected[1] == -8  # alg: "EdDSA"
         assert countersignature.unprotected[4] == b"01"  # kid: b"01"
 
     @pytest.mark.parametrize(
         "type, msg, err_msg",
         [
-            (COSEType.MAC0, [], "Invalid COSE message."),
-            (COSEType.MAC0, [{}, {}, b""], "The protected headers should be bytes."),
-            (COSEType.MAC0, [b"", b"", b""], "The unprotected headers should be Dict[int, Any]."),
-            (COSEType.MAC0, [b"", {}, {}], "The payload should be bytes."),
-            (COSEType.MAC0, [b"", {11: {}}, b""], "The countersignature should be array."),
-            (COSEType.MAC0, [b"", {11: []}, b""], "Invalid countersignature."),
-            (COSEType.MAC0, [b"", {11: [b""]}, b""], "Invalid COSE message."),
-            (COSEType.MAC0, [b"", {11: [""]}, b""], "Invalid countersignature."),
-            (COSEType.MAC0, [b"", {}, b""], "Invalid COSE_Mac0 message."),
-            (COSEType.MAC0, [b"", {}, b"", {}], "tag should be bytes."),
-            (COSEType.ENCRYPT0, [b"", {}, b"", {}], "Invalid COSE_Encrypt0 message."),
-            (COSEType.ENCRYPT, [b"", {}, b""], "Invalid COSE_Encrypt message."),
-            (COSEType.ENCRYPT, [b"", {}, b"", {}], "The COSE recipients should be array."),
-            (COSEType.MAC, [b"", {}, b"", {}], "Invalid COSE_Mac message."),
-            (COSEType.MAC, [b"", {}, b"", {}, {}], "The tag value should be bytes."),
-            (COSEType.MAC, [b"", {}, b"", b"", {}], "The COSE recipients should be array."),
-            (COSEType.MAC, [b"", {}, b"", b"", [[]]], "Invalid COSE message."),
-            (COSEType.SIGN1, [b"", {}, b""], "Invalid COSE_Sign1 message."),
-            (COSEType.SIGN1, [b"", {}, b"", {}], "The COSE signature should be bytes."),
-            (COSEType.SIGN, [b"", {}, b""], "Invalid COSE_Sign message."),
-            (COSEType.SIGN, [b"", {}, b"", {}], "The COSE signatures should be array."),
-            (COSEType.SIGN, [b"", {}, b"", [[]]], "Invalid COSE message."),
-            (COSEType.COUNTERSIGNATURE, [b"", {}, b"", {}], "Invalid COSE_Countersignature."),
-            (COSEType.SIGNATURE, [b"", {}, b"", {}], "Invalid COSE_Signature."),
-            (COSEType.RECIPIENT, [b"", {}, b"", {}], "Invalid COSE_Recipient."),
-            (-1, [b"", {}, b""], "Invalid COSEType(-1) for COSE message."),
+            (COSETypes.MAC0, [], "Invalid COSE message."),
+            (COSETypes.MAC0, [{}, {}, b""], "The protected headers should be bytes."),
+            (COSETypes.MAC0, [b"", b"", b""], "The unprotected headers should be Dict[int, Any]."),
+            (COSETypes.MAC0, [b"", {}, {}], "The payload should be bytes."),
+            (COSETypes.MAC0, [b"", {11: {}}, b""], "The countersignature should be array."),
+            (COSETypes.MAC0, [b"", {11: []}, b""], "Invalid countersignature."),
+            (COSETypes.MAC0, [b"", {11: [b""]}, b""], "Invalid COSE message."),
+            (COSETypes.MAC0, [b"", {11: [""]}, b""], "Invalid countersignature."),
+            (COSETypes.MAC0, [b"", {}, b""], "Invalid COSE_Mac0 message."),
+            (COSETypes.MAC0, [b"", {}, b"", {}], "tag should be bytes."),
+            (COSETypes.ENCRYPT0, [b"", {}, b"", {}], "Invalid COSE_Encrypt0 message."),
+            (COSETypes.ENCRYPT, [b"", {}, b""], "Invalid COSE_Encrypt message."),
+            (COSETypes.ENCRYPT, [b"", {}, b"", {}], "The COSE recipients should be array."),
+            (COSETypes.MAC, [b"", {}, b"", {}], "Invalid COSE_Mac message."),
+            (COSETypes.MAC, [b"", {}, b"", {}, {}], "The tag value should be bytes."),
+            (COSETypes.MAC, [b"", {}, b"", b"", {}], "The COSE recipients should be array."),
+            (COSETypes.MAC, [b"", {}, b"", b"", [[]]], "Invalid COSE message."),
+            (COSETypes.SIGN1, [b"", {}, b""], "Invalid COSE_Sign1 message."),
+            (COSETypes.SIGN1, [b"", {}, b"", {}], "The COSE signature should be bytes."),
+            (COSETypes.SIGN, [b"", {}, b""], "Invalid COSE_Sign message."),
+            (COSETypes.SIGN, [b"", {}, b"", {}], "The COSE signatures should be array."),
+            (COSETypes.SIGN, [b"", {}, b"", [[]]], "Invalid COSE message."),
+            (COSETypes.COUNTERSIGNATURE, [b"", {}, b"", {}], "Invalid COSE_Countersignature."),
+            (COSETypes.SIGNATURE, [b"", {}, b"", {}], "Invalid COSE_Signature."),
+            (COSETypes.RECIPIENT, [b"", {}, b"", {}], "Invalid COSE_Recipient."),
+            (-1, [b"", {}, b""], "Invalid COSETypes(-1) for COSE message."),
         ],
     )
     def test_cose_message_constructor_with_invalid_args(self, type, msg, err_msg):
         with pytest.raises(ValueError) as err:
             COSEMessage(type, msg)
             pytest.fail("COSEMessage() should not fail.")
         assert err_msg in str(err.value)
```

### Comparing `cwt-2.3.2/tests/test_cose_sample.py` & `cwt-2.4.0/tests/test_cose_sample.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from secrets import token_bytes
 
 import pytest
 
-from cwt import COSE, COSEKey, Recipient, Signer
+from cwt import COSE, COSEHeaders, COSEKey, Recipient, Signer
 
 
 class TestCOSESample:
     """
     Tests for samples on COSE Usage Examples.
     """
 
@@ -30,16 +30,16 @@
             unprotected={"kid": "01"},
         )
         assert b"Hello world!" == recipient.decode(encoded2, mac_key)
 
         encoded3 = sender.encode_and_mac(
             b"Hello world!",
             mac_key,
-            protected={1: 5},
-            unprotected={4: b"01"},
+            protected={COSEHeaders.ALG: 5},
+            unprotected={COSEHeaders.KID: b"01"},
         )
         assert b"Hello world!" == recipient.decode(encoded3, mac_key)
 
         assert encoded == encoded2 == encoded3
 
     def test_cose_usage_examples_cose_mac_direct(self):
         mac_key = COSEKey.generate_symmetric_key(alg="HS512", kid="01")
@@ -67,20 +67,20 @@
             mac_key,
             protected={"alg": "HS512"},
             unprotected={"kid": mac_key.kid},
             recipients=[r2],
         )
         assert b"Hello world!" == recipient.decode(encoded2, mac_key)
 
-        r3 = Recipient.new(unprotected={1: -6})
+        r3 = Recipient.new(unprotected={COSEHeaders.ALG: -6})
         encoded3 = sender.encode_and_mac(
             b"Hello world!",
             mac_key,
-            protected={1: 7},
-            unprotected={4: mac_key.kid},
+            protected={COSEHeaders.ALG: 7},
+            unprotected={COSEHeaders.KID: mac_key.kid},
             recipients=[r3],
         )
         assert b"Hello world!" == recipient.decode(encoded3, mac_key)
 
         assert encoded == encoded2 == encoded3
 
     def test_cose_usage_examples_cose_mac_direct_hkdf_sha_256(self):
@@ -282,16 +282,16 @@
             unprotected={"kid": "01", "iv": nonce},
         )
         assert b"Hello world!" == recipient.decode(encoded2, enc_key)
 
         encoded3 = sender.encode_and_encrypt(
             b"Hello world!",
             enc_key,
-            protected={1: 24},
-            unprotected={4: b"01", 5: nonce},
+            protected={COSEHeaders.ALG: 24},
+            unprotected={COSEHeaders.KID: b"01", COSEHeaders.IV: nonce},
         )
         assert b"Hello world!" == recipient.decode(encoded3, enc_key)
 
         # assert encoded == encoded2 == encoded3
 
     def test_cose_usage_examples_cose_encrypt0_hpke(self):
         # The sender side:
@@ -307,19 +307,19 @@
         )
 
         sender = COSE.new()
         encoded = sender.encode_and_encrypt(
             b"This is the content.",
             rpk,
             protected={
-                1: -1,  # alg: "HPKE"
+                COSEHeaders.ALG: -1,  # alg: "HPKE"
             },
             unprotected={
-                4: b"01",  # kid: "01"
-                -4: [  # HPKE sender information
+                COSEHeaders.KID: b"01",  # kid: "01"
+                COSEHeaders.HPKE_SENDER_INFO: [  # HPKE sender information
                     0x0010,  # kem: DHKEM(P-256, HKDF-SHA256)
                     0x0001,  # kdf: HKDF-SHA256
                     0x0001,  # aead: AES-128-GCM
                 ],
             },
         )
 
@@ -357,20 +357,20 @@
         )
 
         # The recipient side:
         recipient = COSE.new()
         assert b"Hello world!" == recipient.decode(encoded, enc_key)
 
         # variation
-        r = Recipient.new(unprotected={1: -6})
+        r = Recipient.new(unprotected={COSEHeaders.ALG: -6})
         encoded2 = sender.encode_and_encrypt(
             b"Hello world!",
             enc_key,
-            protected={1: 24},  # ChaCha20/Poly1305
-            unprotected={4: enc_key.kid, 5: nonce},
+            protected={COSEHeaders.ALG: 24},  # ChaCha20/Poly1305
+            unprotected={COSEHeaders.KID: enc_key.kid, COSEHeaders.IV: nonce},
             recipients=[r],
         )
         assert b"Hello world!" == recipient.decode(encoded2, enc_key)
 
         assert encoded == encoded2
 
     def test_cose_usage_examples_cose_encrypt_hpke(self):
@@ -383,19 +383,19 @@
                 "crv": "P-256",
                 "x": "usWxHK2PmfnHKwXPS54m0kTcGJ90UiglWiGahtagnv8",
                 "y": "IBOL-C3BttVivg-lSreASjpkttcsz-1rb7btKLv8EX4",
             }
         )
         r = Recipient.new(
             protected={
-                1: -1,  # alg: "HPKE"
+                COSEHeaders.ALG: -1,  # alg: "HPKE"
             },
             unprotected={
-                4: b"01",  # kid: "01"
-                -4: [  # HPKE sender information
+                COSEHeaders.KID: b"01",  # kid: "01"
+                COSEHeaders.HPKE_SENDER_INFO: [  # HPKE sender information
                     0x0010,  # kem: DHKEM(P-256, HKDF-SHA256)
                     0x0001,  # kdf: HKDF-SHA256
                     0x0001,  # aead: AES-128-GCM
                 ],
             },
             recipient_key=rpk,
         )
@@ -432,36 +432,36 @@
                 "crv": "P-256",
                 "x": "usWxHK2PmfnHKwXPS54m0kTcGJ90UiglWiGahtagnv8",
                 "y": "IBOL-C3BttVivg-lSreASjpkttcsz-1rb7btKLv8EX4",
             }
         )
         r = Recipient.new(
             protected={
-                1: -1,  # alg: "HPKE"
+                COSEHeaders.ALG: -1,  # alg: "HPKE"
             },
             unprotected={
-                4: b"01",  # kid: "01"
-                -4: [  # HPKE sender information
+                COSEHeaders.KID: b"01",  # kid: "01"
+                COSEHeaders.HPKE_SENDER_INFO: [  # HPKE sender information
                     0x0010,  # kem: DHKEM(P-256, HKDF-SHA256)
                     0x0001,  # kdf: HKDF-SHA256
                     0x0001,  # aead: AES-128-GCM
                 ],
             },
             recipient_key=rpk,
         )
         sender = COSE.new()
         with pytest.raises(ValueError) as err:
             sender.encode_and_encrypt(
                 b"This is the content.",
                 protected={
-                    1: -1,  # alg: "HPKE"
+                    COSEHeaders.ALG: -1,  # alg: "HPKE"
                 },
                 unprotected={
-                    4: b"xx",  # kid: "xx"
-                    -4: [  # HPKE sender information
+                    COSEHeaders.KID: b"xx",  # kid: "xx"
+                    COSEHeaders.HPKE_SENDER_INFO: [  # HPKE sender information
                         0x0010,  # kem: DHKEM(P-256, HKDF-SHA256)
                         0x0001,  # kdf: HKDF-SHA256
                         0x0001,  # aead: AES-128-GCM
                     ],
                 },
                 recipients=[r],
             )
@@ -478,36 +478,36 @@
                 "crv": "P-256",
                 "x": "usWxHK2PmfnHKwXPS54m0kTcGJ90UiglWiGahtagnv8",
                 "y": "IBOL-C3BttVivg-lSreASjpkttcsz-1rb7btKLv8EX4",
             }
         )
         r = Recipient.new(
             protected={
-                1: -1,  # alg: "HPKE"
+                COSEHeaders.ALG: -1,  # alg: "HPKE"
             },
             unprotected={
-                4: b"01",  # kid: "01"
-                -4: [  # HPKE sender information
+                COSEHeaders.KID: b"01",  # kid: "01"
+                COSEHeaders.HPKE_SENDER_INFO: [  # HPKE sender information
                     0x0010,  # kem: DHKEM(P-256, HKDF-SHA256)
                     0x0001,  # kdf: HKDF-SHA256
                     0x0001,  # aead: AES-128-GCM
                 ],
             },
             recipient_key=rpk,
         )
         sender = COSE.new()
         with pytest.raises(ValueError) as err:
             sender.encode_and_encrypt(
                 b"This is the content.",
                 protected={
-                    1: -1,  # alg: "HPKE"
+                    COSEHeaders.ALG: -1,  # alg: "HPKE"
                 },
                 unprotected={
-                    4: b"xx",  # kid: "xx"
-                    -4: [  # HPKE sender information
+                    COSEHeaders.KID: b"xx",  # kid: "xx"
+                    COSEHeaders.HPKE_SENDER_INFO: [  # HPKE sender information
                         0x0010,  # kem: DHKEM(P-256, HKDF-SHA256)
                         0x0001,  # kdf: HKDF-SHA256
                         0x0001,  # aead: AES-128-GCM
                     ],
                 },
                 recipients=[r],
             )
@@ -687,16 +687,16 @@
             unprotected={"kid": "01"},
         )
         assert b"Hello world!" == recipient.decode(encoded2, pub_key)
 
         encoded3 = sender.encode_and_sign(
             b"Hello world!",
             priv_key,
-            protected={1: -7},
-            unprotected={4: b"01"},
+            protected={COSEHeaders.ALG: -7},
+            unprotected={COSEHeaders.KID: b"01"},
         )
         assert b"Hello world!" == recipient.decode(encoded3, pub_key)
 
     def test_cose_usage_examples_cose_encrypt_ecdh_aes_key_wrap(self):
         enc_key = COSEKey.generate_symmetric_key(alg="A128GCM")
 
         # The sender side:
@@ -790,12 +790,12 @@
                     "kid": "01",
                     "crv": "P-256",
                     "x": "usWxHK2PmfnHKwXPS54m0kTcGJ90UiglWiGahtagnv8",
                     "y": "IBOL-C3BttVivg-lSreASjpkttcsz-1rb7btKLv8EX4",
                     "d": "V8kgd2ZBRuh2dgyVINBUqpPDr7BOMGcF22CQMIUHtNM",
                 }
             ),
-            protected={1: -7},
-            unprotected={4: b"01"},
+            protected={COSEHeaders.ALG: -7},
+            unprotected={COSEHeaders.KID: b"01"},
         )
         encoded3 = sender.encode_and_sign(b"Hello world!", signers=[signer])
         assert b"Hello world!" == recipient.decode(encoded3, pub_key)
```

### Comparing `cwt-2.3.2/tests/test_cose_sample_with_encode.py` & `cwt-2.4.0/tests/test_cose_sample_with_encode.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/tests/test_cose_wg_examples.py` & `cwt-2.4.0/tests/test_cose_wg_examples.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/tests/test_cwt.py` & `cwt-2.4.0/tests/test_cwt.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 """
 Tests for CWT.
 """
 from secrets import token_bytes
 
 import cbor2
 import pytest
-from cbor2 import CBORTag
+from cbor2 import CBORTag, dumps
 
-from cwt import CWT, Claims, COSEKey, DecodeError, Recipient, VerifyError
+from cwt import COSE, CWT, Claims, COSEKey, DecodeError, Recipient, VerifyError
 from cwt.cose_key_interface import COSEKeyInterface
 from cwt.signer import Signer
 
 from .utils import key_path, now
 
 
 @pytest.fixture(scope="session", autouse=True)
@@ -601,7 +601,41 @@
         ],
     )
     def test_cwt__verify_with_invalid_args(self, ctx, invalid, msg):
         with pytest.raises(ValueError) as err:
             ctx._verify(invalid)
             pytest.fail("_verify should fail.")
         assert msg in str(err.value)
+
+    def test_cwt_decode_with_cwt_claims_in_headers(self, ctx):
+        cose = COSE.new(alg_auto_inclusion=True, kid_auto_inclusion=True)
+        payload = dumps({1: "https://as.example", 2: "someone"})
+        protected = {13: {1: "https://as.example"}}
+        mac_key = COSEKey.from_symmetric_key(alg="HS256", kid="01")
+        cwt = cose.encode_and_mac(payload, mac_key, protected)
+        decoded = ctx.decode(cwt, mac_key)
+        assert 1 in decoded and decoded[1] == "https://as.example"
+        assert 2 in decoded and decoded[2] == "someone"
+
+    @pytest.mark.parametrize(
+        "invalid, msg",
+        [
+            (
+                {1: "https://asx.example", 2: "someone"},
+                "The CWT claim(1) value in protected header does not match the values in the payload.",
+            ),
+            (
+                {1: "https://as.example", 2: "someonex"},
+                "The CWT claim(2) value in protected header does not match the values in the payload.",
+            ),
+        ],
+    )
+    def test_cwt_decode_with_invalid_cwt_claims_in_headers(self, ctx, invalid, msg):
+        cose = COSE.new(alg_auto_inclusion=True, kid_auto_inclusion=True)
+        payload = dumps({1: "https://as.example", 2: "someone"})
+        protected = {13: invalid}
+        mac_key = COSEKey.from_symmetric_key(alg="HS256", kid="01")
+        cwt = cose.encode_and_mac(payload, mac_key, protected)
+        with pytest.raises(VerifyError) as err:
+            ctx.decode(cwt, mac_key)
+            pytest.fail("verify should fail.")
+        assert msg in str(err.value)
```

### Comparing `cwt-2.3.2/tests/test_cwt_sample.py` & `cwt-2.4.0/tests/test_cwt_sample.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 import pytest
 
 import cwt
 from cwt import (
     COSE,
     CWT,
     Claims,
+    COSEHeaders,
     COSEKey,
+    CWTClaims,
     EncryptedCOSEKey,
     VerifyError,
     load_pem_hcert_dsc,
 )
 
 from .utils import key_path, now
 
@@ -132,21 +134,23 @@
         key = COSEKey.from_symmetric_key(alg="HMAC 256/256", kid="01")
         token = cwt.encode(b'{"iss":"coaps://as.example","sub":"dajiaji","cti":"123"}', key)
         decoded = cwt.decode(token, key)
         assert 1 in decoded and decoded[1] == "coaps://as.example"
 
     def test_sample_readme_maced_cwt_old(self):
         key = COSEKey.from_symmetric_key("mysecretpassword", alg="HS256", kid="01")
-        encoded = cwt.encode_and_mac({1: "coaps://as.example", 2: "dajiaji", 7: b"123"}, key)
+        encoded = cwt.encode_and_mac(
+            {CWTClaims.ISS: "coaps://as.example", CWTClaims.SUB: "dajiaji", CWTClaims.CTI: b"123"}, key
+        )
         decoded = cwt.decode(encoded, key)
         assert 1 in decoded and decoded[1] == "coaps://as.example"
 
     def test_sample_readme_maced_cwt(self):
         key = COSEKey.from_symmetric_key(alg="HMAC 256/256", kid="01")
-        token = cwt.encode({1: "coaps://as.example", 2: "dajiaji", 7: b"123"}, key)
+        token = cwt.encode({CWTClaims.ISS: "coaps://as.example", CWTClaims.SUB: "dajiaji", CWTClaims.CTI: b"123"}, key)
         decoded = cwt.decode(token, key)
         assert 1 in decoded and decoded[1] == "coaps://as.example"
 
     def test_sample_readme_signed_cwt_es256_old(self):
         with open(key_path("private_key_es256.pem")) as key_file:
             private_key = COSEKey.from_pem(key_file.read(), kid="01")
         with open(key_path("public_key_es256.pem")) as key_file:
@@ -551,17 +555,17 @@
     def test_sample_readme_cwt_with_pop_cose_key(self):
         with open(key_path("private_key_ed25519.pem")) as key_file:
             private_key = COSEKey.from_pem(key_file.read(), kid="issuer-01")
         with open(key_path("public_key_es256.pem")) as key_file:
             pop_key = COSEKey.from_pem(key_file.read())
         token = cwt.encode(
             {
-                1: "coaps://as.example",  # iss
-                2: "dajiaji",  # sub
-                7: b"123",  # cti
+                CWTClaims.ISS: "coaps://as.example",  # iss
+                CWTClaims.SUB: "dajiaji",  # sub
+                CWTClaims.CTI: b"123",  # cti
                 8: {  # cnf
                     1: pop_key.to_dict(),
                 },
             },
             private_key,
         )
 
@@ -584,17 +588,17 @@
         )
         pop_key = COSEKey.from_symmetric_key(
             "a-client-secret-of-cwt-presenter",
             alg="HMAC 256/256",
         )
         token = cwt.encode(
             {
-                1: "coaps://as.example",  # iss
-                2: "dajiaji",  # sub
-                7: b"123",  # cti
+                CWTClaims.ISS: "coaps://as.example",  # iss
+                CWTClaims.SUB: "dajiaji",  # sub
+                CWTClaims.CTI: b"123",  # cti
                 8: {  # cnf
                     2: EncryptedCOSEKey.from_cose_key(pop_key, enc_key),
                 },
             },
             private_key,
         )
 
@@ -609,17 +613,17 @@
         assert extracted.key == b"a-client-secret-of-cwt-presenter"
 
     def test_sample_readme_cwt_with_pop_kid(self):
         with open(key_path("private_key_ed25519.pem")) as key_file:
             private_key = COSEKey.from_pem(key_file.read(), kid="01")
         token = cwt.encode(
             {
-                1: "coaps://as.example",  # iss
-                2: "dajiaji",  # sub
-                7: b"123",  # cti
+                CWTClaims.ISS: "coaps://as.example",  # iss
+                CWTClaims.SUB: "dajiaji",  # sub
+                CWTClaims.CTI: b"123",  # cti
                 8: {  # cnf
                     3: b"pop-key-id-of-cwt-presenter",
                 },
             },
             private_key,
         )
 
@@ -630,17 +634,17 @@
         assert 3 in decoded[8] and decoded[8][3] == b"pop-key-id-of-cwt-presenter"
 
     def test_sample_readme_cwt_with_user_defined_claims(self):
         with open(key_path("private_key_ed25519.pem")) as key_file:
             private_key = COSEKey.from_pem(key_file.read(), kid="01")
         token = cwt.encode(
             {
-                1: "coaps://as.example",  # iss
-                2: "dajiaji",  # sub
-                7: b"123",  # cti
+                CWTClaims.ISS: "coaps://as.example",  # iss
+                CWTClaims.SUB: "dajiaji",  # sub
+                CWTClaims.CTI: b"123",  # cti
                 -70001: "foo",
                 -70002: ["bar"],
                 -70003: {"baz": "qux"},
                 -70004: 123,
             },
             private_key,
         )
@@ -732,38 +736,38 @@
         assert 6 in decoded and decoded[6] == 1443944944
         assert 7 in decoded and decoded[7] == bytes.fromhex("0b71")
 
     def test_sample_rfc8392_a3_with_encoding_old(self):
         key = COSEKey.from_bytes(bytes.fromhex(SAMPLE_COSE_KEY_RFC8392_A2_3))
         encoded = cwt.encode_and_sign(
             {
-                1: "coap://as.example.com",
-                2: "erikw",
-                3: "coap://light.example.com",
-                4: 1444064944,
-                5: 1443944944,
-                6: 1443944944,
-                7: bytes.fromhex("0b71"),
+                CWTClaims.ISS: "coap://as.example.com",
+                CWTClaims.SUB: "erikw",
+                CWTClaims.AUD: "coap://light.example.com",
+                CWTClaims.EXP: 1444064944,
+                CWTClaims.NBF: 1443944944,
+                CWTClaims.IAT: 1443944944,
+                CWTClaims.CTI: bytes.fromhex("0b71"),
             },
             key=key,
         )
         decoded = cwt.decode(encoded, keys=key, no_verify=True)
         assert 1 in decoded and decoded[1] == "coap://as.example.com"
 
     def test_sample_rfc8392_a3_with_encoding(self):
         key = COSEKey.from_bytes(bytes.fromhex(SAMPLE_COSE_KEY_RFC8392_A2_3))
         token = cwt.encode(
             {
-                1: "coap://as.example.com",
-                2: "erikw",
-                3: "coap://light.example.com",
-                4: 1444064944,
-                5: 1443944944,
-                6: 1443944944,
-                7: bytes.fromhex("0b71"),
+                CWTClaims.ISS: "coap://as.example.com",
+                CWTClaims.SUB: "erikw",
+                CWTClaims.AUD: "coap://light.example.com",
+                CWTClaims.EXP: 1444064944,
+                CWTClaims.NBF: 1443944944,
+                CWTClaims.IAT: 1443944944,
+                CWTClaims.CTI: bytes.fromhex("0b71"),
             },
             key,
         )
         decoded = cwt.decode(token, keys=key, no_verify=True)
         assert 1 in decoded and decoded[1] == "coap://as.example.com"
 
     def test_sample_rfc8392_a4_old(self):
@@ -773,21 +777,21 @@
                 1: 4,  # Symmetric
                 2: bytes.fromhex("53796d6d6574726963323536"),
                 3: 4,  # HMAC256/64
             }
         )
         encoded = cwt.encode_and_mac(
             {
-                1: "coap://as.example.com",
-                2: "erikw",
-                3: "coap://light.example.com",
-                4: 1444064944,
-                5: 1443944944,
-                6: 1443944944,
-                7: bytes.fromhex("0b71"),
+                CWTClaims.ISS: "coap://as.example.com",
+                CWTClaims.SUB: "erikw",
+                CWTClaims.AUD: "coap://light.example.com",
+                CWTClaims.EXP: 1444064944,
+                CWTClaims.NBF: 1443944944,
+                CWTClaims.IAT: 1443944944,
+                CWTClaims.CTI: bytes.fromhex("0b71"),
             },
             key=key,
             tagged=True,
         )
         assert encoded == bytes.fromhex(SAMPLE_CWT_RFC8392_A4)
         decoded = cwt.decode(encoded, keys=key, no_verify=True)
         assert 1 in decoded and decoded[1] == "coap://as.example.com"
@@ -799,100 +803,100 @@
                 1: 4,  # Symmetric
                 2: bytes.fromhex("53796d6d6574726963323536"),
                 3: 4,  # HMAC256/64
             }
         )
         token = cwt.encode(
             {
-                1: "coap://as.example.com",
-                2: "erikw",
-                3: "coap://light.example.com",
-                4: 1444064944,
-                5: 1443944944,
-                6: 1443944944,
-                7: bytes.fromhex("0b71"),
+                CWTClaims.ISS: "coap://as.example.com",
+                CWTClaims.SUB: "erikw",
+                CWTClaims.AUD: "coap://light.example.com",
+                CWTClaims.EXP: 1444064944,
+                CWTClaims.NBF: 1443944944,
+                CWTClaims.IAT: 1443944944,
+                CWTClaims.CTI: bytes.fromhex("0b71"),
             },
             key,
             tagged=True,
         )
         assert token == bytes.fromhex(SAMPLE_CWT_RFC8392_A4)
         decoded = cwt.decode(token, keys=key, no_verify=True)
         assert 1 in decoded and decoded[1] == "coap://as.example.com"
 
     def test_sample_rfc8392_a5_old(self):
         key = COSEKey.from_bytes(bytes.fromhex(SAMPLE_COSE_KEY_RFC8392_A2_1))
         nonce = bytes.fromhex("99a0d7846e762c49ffe8a63e0b")
         encoded = cwt.encode_and_encrypt(
             {
-                1: "coap://as.example.com",
-                2: "erikw",
-                3: "coap://light.example.com",
-                4: 1444064944,
-                5: 1443944944,
-                6: 1443944944,
-                7: bytes.fromhex("0b71"),
+                CWTClaims.ISS: "coap://as.example.com",
+                CWTClaims.SUB: "erikw",
+                CWTClaims.AUD: "coap://light.example.com",
+                CWTClaims.EXP: 1444064944,
+                CWTClaims.NBF: 1443944944,
+                CWTClaims.IAT: 1443944944,
+                CWTClaims.CTI: bytes.fromhex("0b71"),
             },
             key=key,
             nonce=nonce,
         )
         # assert encoded == bytes.fromhex(SAMPLE_CWT_RFC8392_A5)
         ctx = COSE.new()
         token2 = ctx.encode_and_encrypt(
             cbor2.dumps(
                 {
-                    1: "coap://as.example.com",
-                    2: "erikw",
-                    3: "coap://light.example.com",
-                    4: 1444064944,
-                    5: 1443944944,
-                    6: 1443944944,
-                    7: bytes.fromhex("0b71"),
+                    CWTClaims.ISS: "coap://as.example.com",
+                    CWTClaims.SUB: "erikw",
+                    CWTClaims.AUD: "coap://light.example.com",
+                    CWTClaims.EXP: 1444064944,
+                    CWTClaims.NBF: 1443944944,
+                    CWTClaims.IAT: 1443944944,
+                    CWTClaims.CTI: bytes.fromhex("0b71"),
                 }
             ),
             key,
             protected={1: key.alg},
-            unprotected={4: key.kid, 5: nonce},
+            unprotected={COSEHeaders.KID: key.kid, COSEHeaders.IV: nonce},
         )
         assert token2 == bytes.fromhex(SAMPLE_CWT_RFC8392_A5)
         decoded = cwt.decode(encoded, keys=key, no_verify=True)
         assert 1 in decoded and decoded[1] == "coap://as.example.com"
 
     def test_sample_rfc8392_a5(self):
         key = COSEKey.from_bytes(bytes.fromhex(SAMPLE_COSE_KEY_RFC8392_A2_1))
         nonce = bytes.fromhex("99a0d7846e762c49ffe8a63e0b")
         token = cwt.encode(
             {
-                1: "coap://as.example.com",
-                2: "erikw",
-                3: "coap://light.example.com",
-                4: 1444064944,
-                5: 1443944944,
-                6: 1443944944,
-                7: bytes.fromhex("0b71"),
+                CWTClaims.ISS: "coap://as.example.com",
+                CWTClaims.SUB: "erikw",
+                CWTClaims.AUD: "coap://light.example.com",
+                CWTClaims.EXP: 1444064944,
+                CWTClaims.NBF: 1443944944,
+                CWTClaims.IAT: 1443944944,
+                CWTClaims.CTI: bytes.fromhex("0b71"),
             },
             key=key,
             nonce=nonce,
         )
         # assert token == bytes.fromhex(SAMPLE_CWT_RFC8392_A5)
         ctx = COSE.new()
         token2 = ctx.encode_and_encrypt(
             cbor2.dumps(
                 {
-                    1: "coap://as.example.com",
-                    2: "erikw",
-                    3: "coap://light.example.com",
-                    4: 1444064944,
-                    5: 1443944944,
-                    6: 1443944944,
-                    7: bytes.fromhex("0b71"),
+                    CWTClaims.ISS: "coap://as.example.com",
+                    CWTClaims.SUB: "erikw",
+                    CWTClaims.AUD: "coap://light.example.com",
+                    CWTClaims.EXP: 1444064944,
+                    CWTClaims.NBF: 1443944944,
+                    CWTClaims.IAT: 1443944944,
+                    CWTClaims.CTI: bytes.fromhex("0b71"),
                 }
             ),
             key,
             protected={1: key.alg},
-            unprotected={4: key.kid, 5: nonce},
+            unprotected={COSEHeaders.KID: key.kid, COSEHeaders.IV: nonce},
         )
         assert token2 == bytes.fromhex(SAMPLE_CWT_RFC8392_A5)
         decoded = cwt.decode(token, keys=key, no_verify=True)
         assert 1 in decoded and decoded[1] == "coap://as.example.com"
 
     def test_sample_rfc8392_a6(self):
         sig_key = COSEKey.from_bytes(bytes.fromhex(SAMPLE_COSE_KEY_RFC8392_A2_3))
@@ -901,50 +905,81 @@
         decoded = cwt.decode(encrypted, keys=[enc_key, sig_key], no_verify=True)
         assert 1 in decoded and decoded[1] == "coap://as.example.com"
 
     def test_sample_rfc8392_a6_with_encoding_old(self):
         sig_key = COSEKey.from_bytes(bytes.fromhex(SAMPLE_COSE_KEY_RFC8392_A2_3))
         signed = cwt.encode_and_sign(
             {
-                1: "coap://as.example.com",
-                2: "erikw",
-                3: "coap://light.example.com",
-                4: 1444064944,
-                5: 1443944944,
-                6: 1443944944,
-                7: bytes.fromhex("0b71"),
+                CWTClaims.ISS: "coap://as.example.com",
+                CWTClaims.SUB: "erikw",
+                CWTClaims.AUD: "coap://light.example.com",
+                CWTClaims.EXP: 1444064944,
+                CWTClaims.NBF: 1443944944,
+                CWTClaims.IAT: 1443944944,
+                CWTClaims.CTI: bytes.fromhex("0b71"),
             },
             key=sig_key,
         )
         enc_key = COSEKey.from_bytes(bytes.fromhex(SAMPLE_COSE_KEY_RFC8392_A2_1))
         nonce = bytes.fromhex("4a0694c0e69ee6b5956655c7b2")
         encrypted = cwt.encode_and_encrypt(signed, key=enc_key, nonce=nonce)
         decoded = cwt.decode(encrypted, keys=[enc_key, sig_key], no_verify=True)
         assert 1 in decoded and decoded[1] == "coap://as.example.com"
 
     def test_sample_rfc8392_a6_with_encoding(self):
         sig_key = COSEKey.from_bytes(bytes.fromhex(SAMPLE_COSE_KEY_RFC8392_A2_3))
         signed = cwt.encode(
             {
-                1: "coap://as.example.com",
-                2: "erikw",
-                3: "coap://light.example.com",
-                4: 1444064944,
-                5: 1443944944,
-                6: 1443944944,
-                7: bytes.fromhex("0b71"),
+                CWTClaims.ISS: "coap://as.example.com",
+                CWTClaims.SUB: "erikw",
+                CWTClaims.AUD: "coap://light.example.com",
+                CWTClaims.EXP: 1444064944,
+                CWTClaims.NBF: 1443944944,
+                CWTClaims.IAT: 1443944944,
+                CWTClaims.CTI: bytes.fromhex("0b71"),
             },
             key=sig_key,
         )
         enc_key = COSEKey.from_bytes(bytes.fromhex(SAMPLE_COSE_KEY_RFC8392_A2_1))
         nonce = bytes.fromhex("4a0694c0e69ee6b5956655c7b2")
         encrypted = cwt.encode(signed, key=enc_key, nonce=nonce)
         decoded = cwt.decode(encrypted, keys=[enc_key, sig_key], no_verify=True)
         assert 1 in decoded and decoded[1] == "coap://as.example.com"
 
+    def test_sample_cwt_with_cwt_claims_in_headers(self):
+        # The sender side:
+        sender = COSE.new(alg_auto_inclusion=True, kid_auto_inclusion=True)
+        payload = cbor2.dumps(
+            {
+                CWTClaims.ISS: "coap://as.example.com",
+                CWTClaims.SUB: "erikw",
+                CWTClaims.AUD: "coap://light.example.com",
+                CWTClaims.EXP: now() + 3600,
+                CWTClaims.NBF: now(),
+                CWTClaims.IAT: now(),
+                CWTClaims.CTI: bytes.fromhex("0b71"),
+            },
+        )
+        protected = {
+            COSEHeaders.CWT_CLAIMS: {  # 13
+                CWTClaims.ISS: "coap://as.example.com",
+            }
+        }
+        enc_key = COSEKey.from_symmetric_key(alg="A128GCM", kid="01")
+        token = sender.encode(payload, enc_key, protected)
+
+        # print(token.hex())
+
+        # The recipient side:
+        recipient = CWT.new()
+        # `decode()` checks the validity of the CWT claims header parameter.
+        decoded = recipient.decode(token, enc_key)
+        assert 1 in decoded and decoded[CWTClaims.ISS] == "coap://as.example.com"
+        assert 2 in decoded and decoded[CWTClaims.SUB] == "erikw"
+
     def test_sample_hcert_testdata_AT_2DCode_raw_1(self):
         # A DSC(Document Signing Certificate) issued by a CSCA (Certificate Signing Certificate Authority).
         dsc = "-----BEGIN CERTIFICATE-----\nMIIBvTCCAWOgAwIBAgIKAXk8i88OleLsuTAKBggqhkjOPQQDAjA2MRYwFAYDVQQDDA1BVCBER0MgQ1NDQSAxMQswCQYDVQQGEwJBVDEPMA0GA1UECgwGQk1TR1BLMB4XDTIxMDUwNTEyNDEwNloXDTIzMDUwNTEyNDEwNlowPTERMA8GA1UEAwwIQVQgRFNDIDExCzAJBgNVBAYTAkFUMQ8wDQYDVQQKDAZCTVNHUEsxCjAIBgNVBAUTATEwWTATBgcqhkjOPQIBBggqhkjOPQMBBwNCAASt1Vz1rRuW1HqObUE9MDe7RzIk1gq4XW5GTyHuHTj5cFEn2Rge37+hINfCZZcozpwQKdyaporPUP1TE7UWl0F3o1IwUDAOBgNVHQ8BAf8EBAMCB4AwHQYDVR0OBBYEFO49y1ISb6cvXshLcp8UUp9VoGLQMB8GA1UdIwQYMBaAFP7JKEOflGEvef2iMdtopsetwGGeMAoGCCqGSM49BAMCA0gAMEUCIQDG2opotWG8tJXN84ZZqT6wUBz9KF8D+z9NukYvnUEQ3QIgdBLFSTSiDt0UJaDF6St2bkUQuVHW6fQbONd731/M4nc=\n-----END CERTIFICATE-----"
 
         # An EUDCC (EU Digital COVID Certificate)
         eudcc = bytes.fromhex(
             "d2844da20448d919375fc1e7b6b20126a0590133a4041a61817ca0061a60942ea001624154390103a101a4617681aa62646e01626d616d4f52472d3130303033303231356276706a313131393334393030376264746a323032312d30322d313862636f624154626369783155524e3a555643493a30313a41543a31303830373834334639344145453045453530393346424332353442443831332342626d706c45552f312f32302f31353238626973781b4d696e6973747279206f66204865616c74682c20417573747269616273640262746769383430353339303036636e616da463666e74754d5553544552465241553c474f455353494e47455262666e754d7573746572667261752d47c3b6c39f696e67657263676e74684741425249454c4562676e684761627269656c656376657265312e302e3063646f626a313939382d30322d323658405812fce67cb84c3911d78e3f61f890d0c80eb9675806aebed66aa2d0d0c91d1fc98d7bcb80bf00e181806a9502e11b071325901bd0d2c1b6438747b8cc50f521"
```

### Comparing `cwt-2.3.2/tests/test_encrypted_cose_key.py` & `cwt-2.4.0/tests/test_encrypted_cose_key.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/tests/test_helpers_hcert.py` & `cwt-2.4.0/tests/test_helpers_hcert.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/tests/test_key.py` & `cwt-2.4.0/tests/test_key.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/tests/test_recipient.py` & `cwt-2.4.0/tests/test_recipient.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/tests/test_recipient_algs_aes_key_wrap.py` & `cwt-2.4.0/tests/test_recipient_algs_aes_key_wrap.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/tests/test_recipient_algs_direct.py` & `cwt-2.4.0/tests/test_recipient_algs_direct.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/tests/test_recipient_algs_ecdh_aes_key_wrap.py` & `cwt-2.4.0/tests/test_recipient_algs_ecdh_aes_key_wrap.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/tests/test_recipient_algs_ecdh_direct_hkdf.py` & `cwt-2.4.0/tests/test_recipient_algs_ecdh_direct_hkdf.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/tests/test_recipient_algs_hpke.py` & `cwt-2.4.0/tests/test_recipient_algs_hpke.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/tests/test_signer.py` & `cwt-2.4.0/tests/test_signer.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/tests/test_utils.py` & `cwt-2.4.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/tox.ini` & `cwt-2.4.0/tox.ini`

 * *Files identical despite different names*

### Comparing `cwt-2.3.2/PKG-INFO` & `cwt-2.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwt
-Version: 2.3.2
+Version: 2.4.0
 Summary: A Python implementation of CWT/COSE.
 Home-page: https://github.com/dajiaji/python-cwt
 License: MIT
 Author: Ajitomi Daisuke
 Author-email: dajiaji@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -37,14 +37,15 @@
 Python CWT is a CBOR Web Token (CWT) and CBOR Object Signing and Encryption (COSE)
 implementation compliant with:
 - [RFC9052: CBOR Object Signing and Encryption (COSE): Structures and Process](https://www.rfc-editor.org/rfc/rfc9052.html)
 - [RFC9053: CBOR Object Signing and Encryption (COSE): Initial Algorithms](https://www.rfc-editor.org/rfc/rfc9053.html)
 - [RFC9338: CBOR Object Signing and Encryption (COSE): Countersignatures](https://www.rfc-editor.org/rfc/rfc9338.html) - experimental
 - [RFC8392: CWT (CBOR Web Token)](https://tools.ietf.org/html/rfc8392)
 - [draft-04: Use of HPKE with COSE](https://www.ietf.org/archive/id/draft-ietf-cose-hpke-04.html) - experimental
+- [draft-05: CWT Claims in COSE Headers](https://www.ietf.org/archive/id/draft-ietf-cose-cwt-claims-in-headers-05.html) - experimental
 - and related various specifications. See [Referenced Specifications](#referenced-specifications).
 
 It is designed to make users who already know about [JWS](https://tools.ietf.org/html/rfc7515)/[JWE](https://tools.ietf.org/html/rfc7516)/[JWT](https://tools.ietf.org/html/rfc7519)
 be able to use it in ease. Little knowledge of [CBOR](https://tools.ietf.org/html/rfc7049)/[COSE](https://tools.ietf.org/html/rfc8152)/[CWT](https://tools.ietf.org/html/rfc8392)
 is required to use it.
 
 You can install Python CWT with pip:
@@ -71,30 +72,44 @@
     protected={"alg": "HS256"},
     unprotected={"kid": "01"},
 )
 
 # The recipient side:
 recipient = COSE.new()
 assert b"Hello world!" == recipient.decode(encoded, mac_key)
+
+## You can get decoded protected/unprotected headers with the payload as follows:
+# protected, unprotected, payload = recipient.decode_with_headers(encoded, mac_key)
+# assert b"Hello world!" == payload
 ```
 
 **CWT API**
 
 ```py
 import cwt
-from cwt import COSEKey
+from cwt import COSEKey, CWTClaims
 
 mac_key = COSEKey.generate_symmetric_key(alg="HS256", kid="01")
 
 # The sender side:
-token = encode({1: "coaps://as.example", 2: "dajiaji", 7: b"123"}, mac_key)
+token = encode({
+    CWTClaims.ISS: "coaps://as.example",
+    CWTClaims.SUB: "dajiaji",
+    CWTClaims.CTI: b"123"}, mac_key)
 
 # The recipient side:
 decoded = decode(token, mac_key)
-# decoded == {1: 'coaps://as.example', 2: 'dajiaji', 7: b'123', 4: 1620088759, 5: 1620085159, 6: 1620085159}
+# decoded == {
+#     CWTClaims.ISS: 'coaps://as.example',
+#     CWTClaims.SUB: 'dajiaji',
+#     CWTClaims.CTI: b'123',
+#     CWTClaims.EXP: 1620088759,
+#     CWTClaims.NBF: 1620085159,
+#     CWTClaims.IAT: 1620085159
+# }
 ```
 
 Various usage examples are shown in this README.
 
 See [Documentation](https://python-cwt.readthedocs.io/en/stable/) for details of the APIs.
 
 ## Index
@@ -133,14 +148,15 @@
 - [CWT Usage Examples](#cwt-usage-examples)
     - [MACed CWT](#maced-cwt)
     - [Signed CWT](#signed-cwt)
     - [Encrypted CWT](#encrypted-cwt)
     - [Nested CWT](#nested-cwt)
     - [CWT with User Settings (e.g., expires\_in)](#cwt-with-user-settings)
     - [CWT with User-Defined Claims](#cwt-with-user-defined-claims)
+    - [CWT with CWT claims in COSE headers](#cwt-cwt-claims-in-cose-headers)
     - [CWT with PoP Key](#cwt-with-pop-key)
     - [CWT with Private CA](#cwt-with-private-ca)
     - [CWT for EUDCC (EU Digital COVID Certificate)](#cwt-for-eudcc-eu-digital-covid-certificate)
 - [API Reference](#api-reference)
 - [Supported CWT Claims](#supported-cwt-claims)
 - [Supported COSE Algorithms](#supported-cose-algorithms)
 - [Referenced Specifications](#referenced-specifications)
@@ -187,25 +203,25 @@
 ```
 
 Following two samples are other ways of writing the above example.
 
 CBOR object can be used for `protected` and `unprotected` header parameters as follows:
 
 ```py
-from cwt import COSE, COSEKey
+from cwt import COSE, COSEHeaders, COSEKey
 
 mac_key = COSEKey.generate_symmetric_key(alg="HS256", kid="01")
 
 # The sender side:
 sender = COSE.new()
 encoded = sender.encode(
     b"Hello world!",
     mac_key,
-    protected={1: 5},
-    unprotected={4: b"01"},
+    protected={COSEHeaders.ALG: 5},
+    unprotected={COSEHeaders.KID: b"01"},
 )
 
 # The recipient side:
 recipient = COSE.new()
 assert b"Hello world!" == recipient.decode(encoded, mac_key)
 ```
 
@@ -514,46 +530,46 @@
 #### COSE-HPKE (MAC)
 
 **Experimental Implementation. DO NOT USE for production.**
 
 Create a COSE-HPKE MAC message, verify and decode it as follows:
 
 ```py
-from cwt import COSE, COSEKey, Recipient
+from cwt import COSE, COSEHeaders, COSEKey, Recipient
 
 # The sender side:
 mac_key = COSEKey.generate_symmetric_key(alg="HS256")
 rpk = COSEKey.from_jwk(
     {
         "kty": "EC",
         "kid": "01",
         "crv": "P-256",
         "x": "usWxHK2PmfnHKwXPS54m0kTcGJ90UiglWiGahtagnv8",
         "y": "IBOL-C3BttVivg-lSreASjpkttcsz-1rb7btKLv8EX4",
     }
 )
 r = Recipient.new(
     protected={
-        1: -1,  # alg: "HPKE"
+        COSEHeaders.ALG: -1,  # alg: "HPKE"
     },
     unprotected={
-        4: b"01",  # kid: "01"
-        -4: [  # HPKE sender information
+        COSEHeaders.KID: b"01",  # kid: "01"
+        COSEHeaders.HPKE_SENDER_INFO: [  # HPKE sender information
             0x0010,  # kem: DHKEM(P-256, HKDF-SHA256)
             0x0001,  # kdf: HKDF-SHA256
             0x0001,  # aead: AES-128-GCM
         ],
     },
     recipient_key=rpk,
 )
 sender = COSE.new()
 encoded = sender.encode(
     b"This is the content.",
     mac_key,
-    protected={1: 5},  # alg: HS256
+    protected={COSEHeaders.ALG: 5},  # alg: HS256
     recipients=[r],
 )
 
 # The recipient side:
 rsk = COSEKey.from_jwk(
     {
         "kty": "EC",
@@ -578,15 +594,15 @@
 from cwt import COSE, COSEKey
 
 enc_key = COSEKey.generate_symmetric_key(alg="ChaCha20/Poly1305", kid="01")
 
 # The sender side:
 nonce = enc_key.generate_nonce()
 sender = COSE.new(alg_auto_inclusion=True, kid_auto_inclusion=True)
-encoded = sender.encode(b"Hello world!", enc_key, unprotected={5: nonce})
+encoded = sender.encode(b"Hello world!", enc_key, unprotected={COSEHeaders.IV: nonce})
 
 # The recipient side:
 recipient = COSE.new()
 assert b"Hello world!" == recipient.decode(encoded, enc_key)
 ```
 
 The following sample is another way of writing the above:
@@ -621,15 +637,15 @@
 from cwt import COSE, COSEKey, COSEMessage
 
 enc_key = COSEKey.generate_symmetric_key(alg="ChaCha20/Poly1305", kid="01")
 
 # The sender side:
 nonce = enc_key.generate_nonce()
 sender = COSE.new(alg_auto_inclusion=True, kid_auto_inclusion=True)
-encoded = sender.encode(b"Hello world!", enc_key, unprotected={5: nonce})
+encoded = sender.encode(b"Hello world!", enc_key, unprotected={COSEHeaders.IV: nonce})
 
 # The notary side:
 notary = Signer.from_jwk(
     {
         "kid": "01",
         "kty": "OKP",
         "crv": "Ed25519",
@@ -664,15 +680,15 @@
 #### COSE-HPKE (Encrypt0)
 
 **Experimental Implementation. DO NOT USE for production.**
 
 Create a COSE-HPKE Encrypt0 message and decrypt it as follows:
 
 ```py
-from cwt import COSE, COSEKey
+from cwt import COSE, COSEHeaders, COSEKey
 
 # The sender side:
 rpk = COSEKey.from_jwk(
     {
         "kty": "EC",
         "kid": "01",
         "crv": "P-256",
@@ -682,19 +698,19 @@
 )
 
 sender = COSE.new()
 encoded = sender.encode(
     b"This is the content.",
     rpk,
     protected={
-        1: -1,  # alg: "HPKE"
+        COSEHeaders.ALG: -1,  # alg: "HPKE"
     },
     unprotected={
-        4: b"01",  # kid: "01"
-        -4: [  # HPKE sender information
+        COSEHeaders.KID: b"01",  # kid: "01"
+        COSEHeaders.HPKE_SENDER_INFO: [  # HPKE sender information
             0x0010,  # kem: DHKEM(P-256, HKDF-SHA256)
             0x0001,  # kdf: HKDF-SHA256
             0x0001,  # aead: AES-128-GCM
         ],
     },
 )
 
@@ -718,31 +734,31 @@
 #### Direct Key Distribution for encryption
 
 The direct key distribution shares a MAC key between the sender and the recipient that is used directly.
 The follwing example shows the simplest way to make a COSE MAC message, verify and decode it with the direct
 key distribution method.
 
 ```py
-from cwt import COSE, COSEKey, Recipient
+from cwt import COSE, COSEHeaders, COSEKey, Recipient
 
 enc_key = COSEKey.generate_symmetric_key(alg="ChaCha20/Poly1305", kid="01")
 
 # The sender side:
 nonce = enc_key.generate_nonce()
 r = Recipient.new(unprotected={"alg": "direct"})
-# r = Recipient.new(unprotected={1: -6}) # is also acceptable.
+# r = Recipient.new(unprotected={COSEHeaders.ALG: -6}) # is also acceptable.
 
 sender = COSE.new()
 encoded = sender.encode(
     b"Hello world!",
     enc_key,
     protected={"alg": "ChaCha20/Poly1305"},
-    # protected={1: 24},  # is also acceptable.
+    # protected={COSEHeaders.ALG: 24},  # is also acceptable.
     unprotected={"kid": enc_key.kid, "iv": nonce},
-    # unprotected={4: enc_key.kid, 5: nonce},  # is also acceptable.
+    # unprotected={COSEHeaders.KID: enc_key.kid, COSEHeaders.IV: nonce},  # is also acceptable.
     recipients=[r],
 )
 
 # The recipient side:
 recipient = COSE.new()
 assert b"Hello world!" == recipient.decode(encoded, enc_key)
 ```
@@ -886,15 +902,15 @@
   recipient_key=r_pub_key,
   context={"alg": "A128GCM"},
 )
 sender = COSE.new(alg_auto_inclusion=True)
 encoded = sender.encode(
     b"Hello world!",
     key=enc_key,
-    unprotected={5: nonce},
+    unprotected={COSEHeaders.IV: nonce},
     recipients=[r],
 )
 
 # The recipient side:
 recipient = COSE.new()
 r_priv_key = COSEKey.from_jwk(
     {
@@ -972,47 +988,47 @@
 #### COSE-HPKE (Encrypt)
 
 **Experimental Implementation. DO NOT USE for production.**
 
 Create a COSE-HPKE Encrypt message and decrypt it as follows:
 
 ```py
-from cwt import COSE, COSEKey, Recipient
+from cwt import COSE, COSEHeaders, COSEKey, Recipient
 
 # The sender side:
 enc_key = COSEKey.generate_symmetric_key(alg="A128GCM")
 rpk = COSEKey.from_jwk(
     {
         "kty": "EC",
         "kid": "01",
         "crv": "P-256",
         "x": "usWxHK2PmfnHKwXPS54m0kTcGJ90UiglWiGahtagnv8",
         "y": "IBOL-C3BttVivg-lSreASjpkttcsz-1rb7btKLv8EX4",
     }
 )
 r = Recipient.new(
     protected={
-        1: -1,  # alg: "HPKE"
+        COSEHeaders.ALG: -1,  # alg: "HPKE"
     },
     unprotected={
-        4: b"01",  # kid: "01"
-        -4: [  # HPKE sender information
+        COSEHeaders.KID: b"01",  # kid: "01"
+        COSEHeaders.HPKE_SENDER_INFO: [  # HPKE sender information
             0x0010,  # kem: DHKEM(P-256, HKDF-SHA256)
             0x0001,  # kdf: HKDF-SHA256
             0x0001,  # aead: AES-128-GCM
         ],
     },
     recipient_key=rpk,
 )
 sender = COSE.new()
 encoded = sender.encode(
     b"This is the content.",
     enc_key,
     protected={
-        1: 1,  # alg: "A128GCM"
+        COSEHeaders.ALG: 1,  # alg: "A128GCM"
     },
     recipients=[r],
 )
 
 # The recipient side:
 rsk = COSEKey.from_jwk(
     {
@@ -1250,16 +1266,16 @@
 
 ```py
 import cwt
 from cwt import Claims, COSEKey
 
 try:
     key = COSEKey.generate_symmetric_key(alg="HS256", kid="01")
-    token = {"iss": "coaps://as.example", "sub": "dajiaji", "cti": "123"}, key)
-    decoded = decode(token, key)
+    token = cwt.encode({"iss": "coaps://as.example", "sub": "dajiaji", "cti": "123"}, key)
+    decoded = cwt.decode(token, key)
 
     # If you want to treat the result like a JWT;
     readable = Claims.new(decoded)
     assert readable.iss == 'coaps://as.example'
     assert readable.sub == 'dajiaji'
     assert readable.cti == '123'
     # readable.exp == 1620088759
@@ -1276,19 +1292,19 @@
     print(err)
 ```
 
 A raw CWT structure (Dict[int, Any]) can also be used as follows:
 
 ```py
 import cwt
-from cwt import COSEKey
+from cwt import COSEKey, CWTClaims
 
 key = COSEKey.generate_symmetric_key(alg="HS256", kid="01")
-token = cwt.encode({1: "coaps://as.example", 2: "dajiaji", 7: b"123"}, key)
-decoded = decode(token, key)
+token = cwt.encode({CWTClaims.ISS: "coaps://as.example", CWTClaims.SUB: "dajiaji", CWTClaims.CTI: b"123"}, key)
+decoded = cwt.decode(token, key)
 ```
 
 MAC algorithms other than `HS256` are listed in
 [Supported COSE Algorithms](https://python-cwt.readthedocs.io/en/stable/algorithms.html).
 
 ### Signed CWT
 
@@ -1304,22 +1320,22 @@
 ```py
 import cwt
 from cwt import COSEKey
 
 # The sender side:
 with open("./private_key.pem") as key_file:
     private_key = COSEKey.from_pem(key_file.read(), kid="01")
-token = encode(
+token = cwt.encode(
     {"iss": "coaps://as.example", "sub": "dajiaji", "cti": "123"}, private_key
 )
 
 # The recipient side:
 with open("./public_key.pem") as key_file:
     public_key = COSEKey.from_pem(key_file.read(), kid="01")
-decoded = decode(token, public_key)
+decoded = cwt.decode(token, public_key)
 ```
 
 JWKs can also be used instead of the PEM-formatted keys as follows:
 
 ```py
 import cwt
 from cwt import COSEKey
@@ -1330,43 +1346,43 @@
     "kty": "OKP",
     "key_ops": ["sign"],
     "alg": "EdDSA",
     "crv": "Ed25519",
     "x": "2E6dX83gqD_D0eAmqnaHe1TC1xuld6iAKXfw2OVATr0",
     "d": "L8JS08VsFZoZxGa9JvzYmCWOwg7zaKcei3KZmYsj7dc",
 })
-token =
+token = cwt.encode(
     {"iss": "coaps://as.example", "sub": "dajiaji", "cti": "123"}, private_key
 )
 
 # The recipient side:
 public_key = COSEKey.from_jwk({
     "kid": "01",
     "kty": "OKP",
     "key_ops": ["verify"],
     "crv": "Ed25519",
     "x": "2E6dX83gqD_D0eAmqnaHe1TC1xuld6iAKXfw2OVATr0",
 })
-decoded = decode(token, public_key)
+decoded = cwt.decode(token, public_key)
 ```
 
 Signing algorithms other than `Ed25519` are listed in
 [Supported COSE Algorithms](https://python-cwt.readthedocs.io/en/stable/algorithms.html).
 
 ### Encrypted CWT
 
 Create an encrypted CWT with `ChaCha20/Poly1305` and decrypt it as follows:
 
 ```py
 import cwt
 from cwt import COSEKey
 
 enc_key = COSEKey.generate_symmetric_key(alg="ChaCha20/Poly1305", kid="01")
-token = {"iss": "coaps://as.example", "sub": "dajiaji", "cti": "123"}, enc_key)
-decoded = decode(token, enc_key)
+token = cwt.encode({"iss": "coaps://as.example", "sub": "dajiaji", "cti": "123"}, enc_key)
+decoded = cwt.decode(token, enc_key)
 ```
 
 Encryption algorithms other than `ChaCha20/Poly1305` are listed in
 [Supported COSE Algorithms](https://python-cwt.readthedocs.io/en/stable/algorithms.html).
 
 ### Nested CWT
 
@@ -1378,25 +1394,25 @@
 
 # A shared encryption key.
 enc_key = COSEKey.generate_symmetric_key(alg="ChaCha20/Poly1305", kid="enc-01")
 
 # Creates a CWT with ES256 signing.
 with open("./private_key.pem") as key_file:
     private_key = COSEKey.from_pem(key_file.read(), kid="sig-01")
-token =
+token = cwt.encode(
     {"iss": "coaps://as.example", "sub": "dajiaji", "cti": "123"}, private_key
 )
 
 # Encrypts the signed CWT.
-nested = token, enc_key)
+nested = cwt.encode(token, enc_key)
 
 # Decrypts and verifies the nested CWT.
 with open("./public_key.pem") as key_file:
     public_key = COSEKey.from_pem(key_file.read(), kid="sig-01")
-decoded = decode(nested, [enc_key, public_key])
+decoded = cwt.decode(nested, [enc_key, public_key])
 ```
 
 ### CWT with User Settings
 
 The `cwt` in `cwt.encode()` and `cwt.decode()` above is a global `CWT` class instance created
 with default settings in advance. The default settings are as follows:
 - `expires_in`: `3600` seconds. This is the default lifetime in seconds of CWTs.
@@ -1405,48 +1421,48 @@
 If you want to change the settings, you can create your own `CWT` class instance as follows:
 
 ```py
 from cwt import COSEKey, CWT
 
 key = COSEKey.generate_symmetric_key(alg="HS256", kid="01")
 mycwt = CWT.new(expires_in=3600*24, leeway=10)
-token = my{"iss": "coaps://as.example", "sub": "dajiaji", "cti": "123"}, key)
-decoded = mydecode(token, key)
+token = mycwt.encode({"iss": "coaps://as.example", "sub": "dajiaji", "cti": "123"}, key)
+decoded = mycwt.decode(token, key)
 ```
 
 ### CWT with User-Defined Claims
 
 You can use your own claims as follows:
 
 Note that such user-defined claim's key should be less than -65536.
 
 ```py
 import cwt
-from cwt import COSEKey
+from cwt import COSEKey, CWTClaims
 
 # The sender side:
 with open("./private_key.pem") as key_file:
     private_key = COSEKey.from_pem(key_file.read(), kid="01")
-token =
+token = cwt.encode(
     {
-        1: "coaps://as.example",  # iss
-        2: "dajiaji",  # sub
-        7: b"123",  # cti
+        CWTClaims.ISS: "coaps://as.example",  # iss
+        CWTClaims.SUB: "dajiaji",  # sub
+        CWTClaims.CTI: b"123",  # cti
         -70001: "foo",
         -70002: ["bar"],
         -70003: {"baz": "qux"},
         -70004: 123,
     },
     private_key,
 )
 
 # The recipient side:
 with open("./public_key.pem") as key_file:
     public_key = COSEKey.from_pem(key_file.read(), kid="01")
-raw = decode(token, public_key)
+raw = cwt.decode(token, public_key)
 assert raw[-70001] == "foo"
 assert raw[-70002][0] == "bar"
 assert raw[-70003]["baz"] == "qux"
 assert raw[-70004] == 123
 
 readable = Claims.new(raw)
 assert readable.get(-70001) == "foo"
@@ -1468,15 +1484,15 @@
     "ext_1": -70001,
     "ext_2": -70002,
     "ext_3": -70003,
     "ext_4": -70004,
 }
 
 set_private_claim_names(my_claim_names)
-token =
+token = cwt.encode(
     {
         "iss": "coaps://as.example",
         "sub": "dajiaji",
         "cti": b"123",
         "ext_1": "foo",
         "ext_2": ["bar"],
         "ext_3": {"baz": "qux"},
@@ -1484,26 +1500,65 @@
     },
     private_key,
 )
 
 with open("./public_key.pem") as key_file:
     public_key = COSEKey.from_pem(key_file.read(), kid="01")
 
-raw = decode(token, public_key)
+raw = cwt.decode(token, public_key)
 readable = Claims.new(
     raw,
     private_claims_names=my_claim_names,
 )
 assert readable.get("ext_1") == "foo"
 assert readable.get("ext_2")[0] == "bar"
 assert readable.get("ext_3")["baz"] == "qux"
 assert readable.get("ext_4") == 123
 ```
 
 
+### CWT with CWT claims in COSE headers
+
+Python CWT supports [CWT Claims in COSE Headers](https://www.ietf.org/archive/id/draft-ietf-cose-cwt-claims-in-headers-05.html)  experimentally.
+
+If a CWT message has a CWT Claims header parameter in its protected header, `cwt.decode()` checks whether the values of the claims included in that parameter match the values of the corresponding claims in the payload. If they do not match, `VerifyError` is raised.
+
+```py
+from cwt import COSE, COSEHeaders, COSEKey, CWT, CWTClaims
+
+enc_key = COSEKey.from_symmetric_key(alg="A128GCM", kid="01")
+
+# The sender side:
+sender = COSE.new(alg_auto_inclusion=True, kid_auto_inclusion=True)
+payload = cbor2.dumps(
+    {
+        CWTClaims.ISS: "coap://as.example.com",
+        CWTClaims.SUB: "erikw",
+        CWTClaims.AUD: "coap://light.example.com",
+        CWTClaims.EXP: now() + 3600,
+        CWTClaims.NBF: now(),
+        CWTClaims.IAT: now(),
+        CWTClaims.CTI: bytes.fromhex("0b71"),
+    },
+)
+protected = {
+    COSEHeaders.CWT_CLAIMS: {  # 13
+        CWTClaims.ISS: "coap://as.example.com",
+    }
+}
+token = sender.encode(payload, enc_key, protected)
+
+# The recipient side:
+recipient = CWT.new()
+# `decode()` checks the validity of the CWT claims header parameter.
+decoded = recipient.decode(token, enc_key)
+assert decoded[CWTClaims.ISS] == "coap://as.example.com"
+assert decoded[CWTClaims.SUB] == "erikw"
+```
+
 ### CWT with PoP Key
 
 Python CWT supports [Proof-of-Possession Key Semantics for CBOR Web Tokens (CWTs)](https://tools.ietf.org/html/rfc8747).
 A CWT can include a PoP key as follows:
 
 On the issuer side:
 
@@ -1512,15 +1567,15 @@
 from cwt import COSEKey
 
 # Prepares a signing key for CWT in advance.
 with open("./private_key_of_issuer.pem") as key_file:
     private_key = COSEKey.from_pem(key_file.read(), kid="issuer-01")
 
 # Sets the PoP key to a CWT for the presenter.
-token =
+token = cwt.encode(
     {
         "iss": "coaps://as.example",
         "sub": "dajiaji",
         "cti": "123",
         "cnf": {
             "jwk": {  # Provided by the CWT presenter.
                 "kty": "OKP",
@@ -1564,15 +1619,15 @@
 from cwt import Claims, COSEKey
 
 # Prepares the public key of the issuer in advance.
 with open("./public_key_of_issuer.pem") as key_file:
     public_key = COSEKey.from_pem(key_file.read(), kid="issuer-01")
 
 # Verifies and decodes the CWT received from the presenter.
-raw = decode(token, public_key)
+raw = cwt.decode(token, public_key)
 decoded = Claims.new(raw)
 
 # Extracts the PoP key from the CWT.
 extracted_pop_key = COSEKey.new(decoded.cnf)  # = raw[8][1]
 
 # Then, verifies the message sent by the presenter
 # with the signature which is also sent by the presenter as follows:
@@ -1592,15 +1647,15 @@
 import cwt
 from cwt import Claims, COSEKey
 
 # The sernder side:
 with open("./private_key_of_cert.pem")) as f:
     private_key = COSEKey.from_pem(f.read(), kid="01")
 
-token =
+token = cwt.encode(
     {"iss": "coaps://as.example", "sub": "dajiaji", "cti": "123"}, private_key
 )
 
 # The recipient side:
 public_key = COSEKey.from_jwk(
     {
         "kty": "EC",
@@ -1643,15 +1698,15 @@
 # An EUDCC (EU Digital COVID Certificate) quoted from:
 # https://github.com/eu-digital-green-certificates/dgc-testdata/blob/main/AT/2DCode/raw/1.json
 eudcc = bytes.fromhex(
     "d2844da20448d919375fc1e7b6b20126a0590133a4041a61817ca0061a60942ea001624154390103a101a4617681aa62646e01626d616d4f52472d3130303033303231356276706a313131393334393030376264746a323032312d30322d313862636f624154626369783155524e3a555643493a30313a41543a31303830373834334639344145453045453530393346424332353442443831332342626d706c45552f312f32302f31353238626973781b4d696e6973747279206f66204865616c74682c20417573747269616273640262746769383430353339303036636e616da463666e74754d5553544552465241553c474f455353494e47455262666e754d7573746572667261752d47c3b6c39f696e67657263676e74684741425249454c4562676e684761627269656c656376657265312e302e3063646f626a313939382d30322d323658405812fce67cb84c3911d78e3f61f890d0c80eb9675806aebed66aa2d0d0c91d1fc98d7bcb80bf00e181806a9502e11b071325901bd0d2c1b6438747b8cc50f521"
 )
 
 public_key = load_pem_hcert_dsc(dsc)
-decoded = decode(eudcc, keys=[public_key])
+decoded = cwt.decode(eudcc, keys=[public_key])
 claims = Claims.new(decoded)
 # claims.hcert[1] ==
 # {
 #     'v': [
 #         {
 #             'dn': 1,
 #             'ma': 'ORG-100030215',
@@ -1697,14 +1752,15 @@
 - [RFC9338: CBOR Object Signing and Encryption (COSE): Countersignatures](https://www.rfc-editor.org/rfc/rfc9338.html) - experimental
 - [RFC8812: COSE and JOSE Registrations for Web Authentication (WebAuthn) Algorithms](https://tools.ietf.org/html/rfc8812)
 - [RFC8747: Proof-of-Possession Key Semantics for CBOR Web Tokens (CWTs)](https://tools.ietf.org/html/rfc8747)
 - [RFC8392: CWT (CBOR Web Token)](https://tools.ietf.org/html/rfc8392)
 - [RFC8230: Using RSA Algorithms with COSE Messages](https://tools.ietf.org/html/rfc8230)
 - [RFC8152: CBOR Object Signing and Encryption (COSE)](https://tools.ietf.org/html/rfc8152)
 - [draft-04: Use of HPKE with COSE](https://www.ietf.org/archive/id/draft-ietf-cose-hpke-04.html) - experimental
+- [draft-05: CWT Claims in COSE Headers](https://www.ietf.org/archive/id/draft-ietf-cose-cwt-claims-in-headers-05.html) - experimental
 - [Electronic Health Certificate Specification](https://github.com/ehn-dcc-development/hcert-spec/blob/main/hcert_spec.md)
 - [Technical Specifications for Digital Green Certificates Volume 1](https://ec.europa.eu/health/sites/default/files/ehealth/docs/digital-green-certificates_v1_en.pdf)
 
 ## Tests
 
 You can run tests from the project root after cloning with:
```

