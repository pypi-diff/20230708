# Comparing `tmp/cert_utils-0.1.3.tar.gz` & `tmp/cert_utils-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cert_utils-0.1.3.tar", last modified: Wed Jul  5 18:34:11 2023, max compression
+gzip compressed data, was "cert_utils-0.1.4.tar", last modified: Fri Jul  7 22:41:46 2023, max compression
```

## Comparing `cert_utils-0.1.3.tar` & `cert_utils-0.1.4.tar`

### file list

```diff
@@ -1,188 +1,188 @@
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:11.244939 cert_utils-0.1.3/
--rw-r--r--   0 jvanasco   (501) admin       (80)      559 2023-07-05 18:33:55.000000 cert_utils-0.1.3/CHANGES.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)    12231 2023-06-23 17:24:49.000000 cert_utils-0.1.3/LICENSE.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)      191 2023-06-23 17:24:49.000000 cert_utils-0.1.3/MANIFEST.in
--rw-r--r--   0 jvanasco   (501) admin       (80)     4951 2023-07-05 18:34:11.245333 cert_utils-0.1.3/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)     4121 2023-06-23 17:24:49.000000 cert_utils-0.1.3/README.md
--rw-r--r--   0 jvanasco   (501) admin       (80)       39 2023-06-23 17:24:49.000000 cert_utils-0.1.3/pyproject.toml
--rw-r--r--   0 jvanasco   (501) admin       (80)      403 2023-07-05 18:34:11.248645 cert_utils-0.1.3/setup.cfg
--rw-r--r--   0 jvanasco   (501) admin       (80)     2801 2023-06-23 17:24:49.000000 cert_utils-0.1.3/setup.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:10.758927 cert_utils-0.1.3/src/
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:10.805271 cert_utils-0.1.3/src/cert_utils/
--rw-r--r--   0 jvanasco   (501) admin       (80)      145 2023-07-05 18:33:55.000000 cert_utils-0.1.3/src/cert_utils/__init__.py
--rw-r--r--   0 jvanasco   (501) admin       (80)   131802 2023-07-05 18:33:55.000000 cert_utils-0.1.3/src/cert_utils/core.py
--rw-r--r--   0 jvanasco   (501) admin       (80)      441 2023-06-23 18:06:28.000000 cert_utils-0.1.3/src/cert_utils/errors.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:10.869991 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/
--rw-r--r--   0 jvanasco   (501) admin       (80)     1680 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/fakeleintermediatex1.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1797 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/fakelerootx1.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1696 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/isrg-root-ocsp-x1.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1955 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/isrg-root-x1-cross-signed.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1578 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/isrg-root-x2-cross-signed.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)      790 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/isrg-root-x2.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1939 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/isrgrootx1.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1391 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/isrgrootx1.pkix
--rw-r--r--   0 jvanasco   (501) admin       (80)     1021 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-e1.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1021 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-e2.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1586 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-r3-cross-signed.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1826 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-r3.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1586 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-r4-cross-signed.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1826 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-r4.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-x1-cross-signed.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-x2-cross-signed.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1647 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-x3-cross-signed.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1647 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-x4-cross-signed.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     2013 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/letsencryptauthorityx1.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     2013 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/letsencryptauthorityx2.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1984 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/letsencryptauthorityx3.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1984 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/letsencryptauthorityx4.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)      893 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/trustid-x3-root.p7c
--rw-r--r--   0 jvanasco   (501) admin       (80)     1199 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/trustid-x3-root.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)    16333 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/letsencrypt_info.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     1597 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/model.py
--rw-r--r--   0 jvanasco   (501) admin       (80)        0 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/py.typed
--rw-r--r--   0 jvanasco   (501) admin       (80)     3441 2023-06-23 17:24:49.000000 cert_utils-0.1.3/src/cert_utils/utils.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:10.814577 cert_utils-0.1.3/src/cert_utils.egg-info/
--rw-r--r--   0 jvanasco   (501) admin       (80)     4951 2023-07-05 18:34:10.000000 cert_utils-0.1.3/src/cert_utils.egg-info/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)     7615 2023-07-05 18:34:10.000000 cert_utils-0.1.3/src/cert_utils.egg-info/SOURCES.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2023-07-05 18:34:10.000000 cert_utils-0.1.3/src/cert_utils.egg-info/dependency_links.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2023-06-23 18:06:35.000000 cert_utils-0.1.3/src/cert_utils.egg-info/not-zip-safe
--rw-r--r--   0 jvanasco   (501) admin       (80)      200 2023-07-05 18:34:10.000000 cert_utils-0.1.3/src/cert_utils.egg-info/requires.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)       11 2023-07-05 18:34:10.000000 cert_utils-0.1.3/src/cert_utils.egg-info/top_level.txt
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:10.880580 cert_utils-0.1.3/tests/
--rw-r--r--   0 jvanasco   (501) admin       (80)        0 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/__init__.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     7702 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/_utils.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:10.884175 cert_utils-0.1.3/tests/test_data/
--rw-r--r--   0 jvanasco   (501) admin       (80)     3303 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/__README__.txt
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:10.761690 cert_utils-0.1.3/tests/test_data/alternate_chains/
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:10.894009 cert_utils-0.1.3/tests/test_data/alternate_chains/1/
--rw-r--r--   0 jvanasco   (501) admin       (80)       48 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/alternate_chains/1/__README__.txt
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:10.763553 cert_utils-0.1.3/tests/test_data/alternate_chains/1/alternate_chains/
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:10.905522 cert_utils-0.1.3/tests/test_data/alternate_chains/1/alternate_chains/1/
--rw-r--r--   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/alternate_chains/1/alternate_chains/1/chain.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     2779 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/alternate_chains/1/alternate_chains/1/fullchain.pem
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:10.909542 cert_utils-0.1.3/tests/test_data/alternate_chains/1/alternate_chains/2/
--rw-r--r--   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/alternate_chains/1/alternate_chains/2/chain.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     2779 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/alternate_chains/1/alternate_chains/2/fullchain.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1570 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/alternate_chains/1/cert.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/alternate_chains/1/chain.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     2779 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/alternate_chains/1/fullchain.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     3272 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/alternate_chains/1/privkey.pem
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:10.947474 cert_utils-0.1.3/tests/test_data/key_technology-ec/
--rw-r--r--   0 jvanasco   (501) admin       (80)      288 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-ec/ec384-1-key.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)      452 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-ec/ec384-1.csr
--rw-r--r--   0 jvanasco   (501) admin       (80)      288 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-ec/ec384-2-key.pem
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:11.044438 cert_utils-0.1.3/tests/test_data/key_technology-rsa/
--rw-r--r--   0 jvanasco   (501) admin       (80)     1679 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-1.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1679 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-2.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1679 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-3.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-4.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1679 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-5.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-account_daily.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-account_weekly.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-global_daily.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1671 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-global_weekly.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1679 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-single_certificate.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/acme_account_1.key
--rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/acme_account_2.key
--rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/acme_account_3.key
--rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/acme_account_4.key
--rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/acme_account_5.key
--rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/private_1.key
--rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/private_2.key
--rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/private_3.key
--rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/private_4.key
--rw-r--r--   0 jvanasco   (501) admin       (80)     3247 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/private_5.key
--rw-r--r--   0 jvanasco   (501) admin       (80)      664 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_1-server.crt
--rw-r--r--   0 jvanasco   (501) admin       (80)      558 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_1-server.csr
--rw-r--r--   0 jvanasco   (501) admin       (80)      891 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_1-server.key
--rw-r--r--   0 jvanasco   (501) admin       (80)      664 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_2-server.crt
--rw-r--r--   0 jvanasco   (501) admin       (80)      558 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_2-server.csr
--rw-r--r--   0 jvanasco   (501) admin       (80)      887 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_2-server.key
--rw-r--r--   0 jvanasco   (501) admin       (80)      664 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_3-server.crt
--rw-r--r--   0 jvanasco   (501) admin       (80)      558 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_3-server.csr
--rw-r--r--   0 jvanasco   (501) admin       (80)      887 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_3-server.key
--rw-r--r--   0 jvanasco   (501) admin       (80)      664 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_4-server.crt
--rw-r--r--   0 jvanasco   (501) admin       (80)      558 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_4-server.csr
--rw-r--r--   0 jvanasco   (501) admin       (80)      887 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_4-server.key
--rw-r--r--   0 jvanasco   (501) admin       (80)      664 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_5-server.crt
--rw-r--r--   0 jvanasco   (501) admin       (80)      558 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_5-server.csr
--rw-r--r--   0 jvanasco   (501) admin       (80)      887 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_5-server.key
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:11.045961 cert_utils-0.1.3/tests/test_data/long_chains/
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:11.078399 cert_utils-0.1.3/tests/test_data/long_chains/TestA/
--rw-r--r--   0 jvanasco   (501) admin       (80)      573 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/long_chains/TestA/__README__.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)       76 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/long_chains/TestA/_data.json
--rw-r--r--   0 jvanasco   (501) admin       (80)     2683 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/long_chains/TestA/_demo.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     1574 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/long_chains/TestA/cert.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     3665 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/long_chains/TestA/chain_0.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     3664 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/long_chains/TestA/chain_0_bad.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     3665 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/long_chains/TestA/chain_1.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     3665 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/long_chains/TestA/chain_2.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1151 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/long_chains/TestA/root_0.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1151 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/long_chains/TestA/root_1.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1151 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/long_chains/TestA/root_2.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)       46 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/long_chains/__README__.txt
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:11.131146 cert_utils-0.1.3/tests/test_data/pebble-certs/
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/cert1.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/cert2.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/cert3.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/cert4.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/cert5.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/cert6.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/chain1.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/chain2.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/chain3.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/chain4.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/chain5.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/chain6.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/fullchain1.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/fullchain2.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/fullchain3.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/fullchain4.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/fullchain5.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/fullchain6.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/privkey1.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/privkey2.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/privkey3.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/privkey4.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/privkey5.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     3247 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/pebble-certs/privkey6.pem
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:10.774002 cert_utils-0.1.3/tests/test_data/unit_tests/
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:11.135444 cert_utils-0.1.3/tests/test_data/unit_tests/_support/
--rw-r--r--   0 jvanasco   (501) admin       (80)     3247 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/_support/account.key
--rw-r--r--   0 jvanasco   (501) admin       (80)      913 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/_support/info.txt
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:11.143628 cert_utils-0.1.3/tests/test_data/unit_tests/account_001/
--rw-r--r--   0 jvanasco   (501) admin       (80)      212 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/account_001/info.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)       70 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/account_001/meta.json
--rw-r--r--   0 jvanasco   (501) admin       (80)     1632 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/account_001/private_key.json
--rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/account_001/private_key.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)       86 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/account_001/regr.json
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:11.163585 cert_utils-0.1.3/tests/test_data/unit_tests/cert_001/
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1635 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_001/cert.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_001/chain.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1674 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_001/csr.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     2844 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_001/fullchain.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)      387 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_001/info.txt
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_001/privkey.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1516 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_001/test.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:11.172372 cert_utils-0.1.3/tests/test_data/unit_tests/cert_002/
--rw-r--r--   0 jvanasco   (501) admin       (80)      538 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_002/csr.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)      889 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_002/info.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)      887 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_002/privkey.pem
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:11.179525 cert_utils-0.1.3/tests/test_data/unit_tests/cert_003/
--rw-r--r--   0 jvanasco   (501) admin       (80)     1042 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_003/cert.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)      566 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_003/csr.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     2250 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_003/fullchain.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)      569 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_003/info.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)      891 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_003/privkey.pem
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:11.197273 cert_utils-0.1.3/tests/test_data/unit_tests/cert_004/
--rw-r--r--   0 jvanasco   (501) admin       (80)     1111 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_004/cert.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)      631 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_004/csr.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     2319 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_004/fullchain.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)      751 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_004/info.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)      887 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_004/privkey.pem
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-05 18:34:11.243036 cert_utils-0.1.3/tests/test_data/unit_tests/cert_005/
--rw-r--r--   0 jvanasco   (501) admin       (80)      643 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_005/csr.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1146 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_005/info.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)      887 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_data/unit_tests/cert_005/privkey.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)    73620 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tests/test_unit.py
--rw-r--r--   0 jvanasco   (501) admin       (80)      149 2023-06-23 17:24:49.000000 cert_utils-0.1.3/tox.ini
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-07 22:41:46.080349 cert_utils-0.1.4/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      602 2023-07-07 22:41:26.000000 cert_utils-0.1.4/CHANGES.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)    12231 2023-06-23 17:24:49.000000 cert_utils-0.1.4/LICENSE.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      191 2023-06-23 17:24:49.000000 cert_utils-0.1.4/MANIFEST.in
+-rw-r--r--   0 jvanasco   (501) admin       (80)     4971 2023-07-07 22:41:46.080773 cert_utils-0.1.4/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)     4121 2023-06-23 17:24:49.000000 cert_utils-0.1.4/README.md
+-rw-r--r--   0 jvanasco   (501) admin       (80)       39 2023-06-23 17:24:49.000000 cert_utils-0.1.4/pyproject.toml
+-rw-r--r--   0 jvanasco   (501) admin       (80)      403 2023-07-07 22:41:46.083341 cert_utils-0.1.4/setup.cfg
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2801 2023-06-23 17:24:49.000000 cert_utils-0.1.4/setup.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-07 22:41:45.624615 cert_utils-0.1.4/src/
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-07 22:41:45.654064 cert_utils-0.1.4/src/cert_utils/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      145 2023-07-07 22:41:26.000000 cert_utils-0.1.4/src/cert_utils/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)   131792 2023-07-07 22:41:26.000000 cert_utils-0.1.4/src/cert_utils/core.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)      441 2023-06-23 18:06:28.000000 cert_utils-0.1.4/src/cert_utils/errors.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-07 22:41:45.724042 cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1680 2023-06-23 17:24:49.000000 cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/fakeleintermediatex1.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1797 2023-06-23 17:24:49.000000 cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/fakelerootx1.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1696 2023-06-23 17:24:49.000000 cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/isrg-root-ocsp-x1.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1955 2023-06-23 17:24:49.000000 cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/isrg-root-x1-cross-signed.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1578 2023-06-23 17:24:49.000000 cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/isrg-root-x2-cross-signed.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)      790 2023-06-23 17:24:49.000000 cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/isrg-root-x2.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1939 2023-06-23 17:24:49.000000 cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/isrgrootx1.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1391 2023-06-23 17:24:49.000000 cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/isrgrootx1.pkix
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1021 2023-06-23 17:24:49.000000 cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/lets-encrypt-e1.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1021 2023-06-23 17:24:49.000000 cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/lets-encrypt-e2.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1586 2023-06-23 17:24:49.000000 cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/lets-encrypt-r3-cross-signed.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1826 2023-06-23 17:24:49.000000 cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/lets-encrypt-r3.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1586 2023-06-23 17:24:49.000000 cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/lets-encrypt-r4-cross-signed.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1826 2023-06-23 17:24:49.000000 cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/lets-encrypt-r4.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2023-06-23 17:24:49.000000 cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/lets-encrypt-x1-cross-signed.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2023-06-23 17:24:49.000000 cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/lets-encrypt-x2-cross-signed.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1647 2023-06-23 17:24:49.000000 cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/lets-encrypt-x3-cross-signed.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1647 2023-06-23 17:24:49.000000 cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/lets-encrypt-x4-cross-signed.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2013 2023-06-23 17:24:49.000000 cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/letsencryptauthorityx1.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2013 2023-06-23 17:24:49.000000 cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/letsencryptauthorityx2.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1984 2023-06-23 17:24:49.000000 cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/letsencryptauthorityx3.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1984 2023-06-23 17:24:49.000000 cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/letsencryptauthorityx4.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)      893 2023-06-23 17:24:49.000000 cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/trustid-x3-root.p7c
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1199 2023-06-23 17:24:49.000000 cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/trustid-x3-root.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)    16333 2023-06-23 17:24:49.000000 cert_utils-0.1.4/src/cert_utils/letsencrypt_info.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1597 2023-06-23 17:24:49.000000 cert_utils-0.1.4/src/cert_utils/model.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)        0 2023-06-23 17:24:49.000000 cert_utils-0.1.4/src/cert_utils/py.typed
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3477 2023-07-07 22:41:26.000000 cert_utils-0.1.4/src/cert_utils/utils.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-07 22:41:45.670673 cert_utils-0.1.4/src/cert_utils.egg-info/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     4971 2023-07-07 22:41:44.000000 cert_utils-0.1.4/src/cert_utils.egg-info/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)     7615 2023-07-07 22:41:45.000000 cert_utils-0.1.4/src/cert_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2023-07-07 22:41:44.000000 cert_utils-0.1.4/src/cert_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2023-06-23 18:06:35.000000 cert_utils-0.1.4/src/cert_utils.egg-info/not-zip-safe
+-rw-r--r--   0 jvanasco   (501) admin       (80)      200 2023-07-07 22:41:45.000000 cert_utils-0.1.4/src/cert_utils.egg-info/requires.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)       11 2023-07-07 22:41:45.000000 cert_utils-0.1.4/src/cert_utils.egg-info/top_level.txt
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-07 22:41:45.727686 cert_utils-0.1.4/tests/
+-rw-r--r--   0 jvanasco   (501) admin       (80)        0 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     7702 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/_utils.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-07 22:41:45.730154 cert_utils-0.1.4/tests/test_data/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3303 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/__README__.txt
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-07 22:41:45.626658 cert_utils-0.1.4/tests/test_data/alternate_chains/
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-07 22:41:45.736519 cert_utils-0.1.4/tests/test_data/alternate_chains/1/
+-rw-r--r--   0 jvanasco   (501) admin       (80)       48 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/alternate_chains/1/__README__.txt
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-07 22:41:45.628088 cert_utils-0.1.4/tests/test_data/alternate_chains/1/alternate_chains/
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-07 22:41:45.739255 cert_utils-0.1.4/tests/test_data/alternate_chains/1/alternate_chains/1/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/alternate_chains/1/alternate_chains/1/chain.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2779 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/alternate_chains/1/alternate_chains/1/fullchain.pem
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-07 22:41:45.742483 cert_utils-0.1.4/tests/test_data/alternate_chains/1/alternate_chains/2/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/alternate_chains/1/alternate_chains/2/chain.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2779 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/alternate_chains/1/alternate_chains/2/fullchain.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1570 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/alternate_chains/1/cert.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/alternate_chains/1/chain.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2779 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/alternate_chains/1/fullchain.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3272 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/alternate_chains/1/privkey.pem
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-07 22:41:45.746103 cert_utils-0.1.4/tests/test_data/key_technology-ec/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      288 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-ec/ec384-1-key.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)      452 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-ec/ec384-1.csr
+-rw-r--r--   0 jvanasco   (501) admin       (80)      288 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-ec/ec384-2-key.pem
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-07 22:41:45.882983 cert_utils-0.1.4/tests/test_data/key_technology-rsa/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1679 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/AcmeAccountKey-1.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1679 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/AcmeAccountKey-2.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1679 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/AcmeAccountKey-3.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/AcmeAccountKey-4.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1679 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/AcmeAccountKey-5.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-account_daily.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-account_weekly.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-global_daily.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1671 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-global_weekly.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1679 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-single_certificate.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/acme_account_1.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/acme_account_2.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/acme_account_3.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/acme_account_4.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/acme_account_5.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/private_1.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/private_2.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/private_3.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/private_4.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3247 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/private_5.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)      664 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/selfsigned_1-server.crt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      558 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/selfsigned_1-server.csr
+-rw-r--r--   0 jvanasco   (501) admin       (80)      891 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/selfsigned_1-server.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)      664 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/selfsigned_2-server.crt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      558 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/selfsigned_2-server.csr
+-rw-r--r--   0 jvanasco   (501) admin       (80)      887 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/selfsigned_2-server.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)      664 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/selfsigned_3-server.crt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      558 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/selfsigned_3-server.csr
+-rw-r--r--   0 jvanasco   (501) admin       (80)      887 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/selfsigned_3-server.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)      664 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/selfsigned_4-server.crt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      558 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/selfsigned_4-server.csr
+-rw-r--r--   0 jvanasco   (501) admin       (80)      887 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/selfsigned_4-server.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)      664 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/selfsigned_5-server.crt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      558 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/selfsigned_5-server.csr
+-rw-r--r--   0 jvanasco   (501) admin       (80)      887 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/key_technology-rsa/selfsigned_5-server.key
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-07 22:41:45.885357 cert_utils-0.1.4/tests/test_data/long_chains/
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-07 22:41:45.926597 cert_utils-0.1.4/tests/test_data/long_chains/TestA/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      573 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/long_chains/TestA/__README__.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)       76 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/long_chains/TestA/_data.json
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2683 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/long_chains/TestA/_demo.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1574 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/long_chains/TestA/cert.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3665 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/long_chains/TestA/chain_0.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3664 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/long_chains/TestA/chain_0_bad.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3665 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/long_chains/TestA/chain_1.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3665 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/long_chains/TestA/chain_2.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1151 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/long_chains/TestA/root_0.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1151 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/long_chains/TestA/root_1.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1151 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/long_chains/TestA/root_2.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)       46 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/long_chains/__README__.txt
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-07 22:41:45.983725 cert_utils-0.1.4/tests/test_data/pebble-certs/
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/pebble-certs/cert1.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/pebble-certs/cert2.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/pebble-certs/cert3.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/pebble-certs/cert4.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/pebble-certs/cert5.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/pebble-certs/cert6.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/pebble-certs/chain1.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/pebble-certs/chain2.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/pebble-certs/chain3.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/pebble-certs/chain4.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/pebble-certs/chain5.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/pebble-certs/chain6.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/pebble-certs/fullchain1.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/pebble-certs/fullchain2.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/pebble-certs/fullchain3.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/pebble-certs/fullchain4.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/pebble-certs/fullchain5.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/pebble-certs/fullchain6.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/pebble-certs/privkey1.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/pebble-certs/privkey2.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/pebble-certs/privkey3.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/pebble-certs/privkey4.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/pebble-certs/privkey5.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     3247 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/pebble-certs/privkey6.pem
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-07 22:41:45.634766 cert_utils-0.1.4/tests/test_data/unit_tests/
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-07 22:41:45.987690 cert_utils-0.1.4/tests/test_data/unit_tests/_support/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3247 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/unit_tests/_support/account.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)      913 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/unit_tests/_support/info.txt
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-07 22:41:45.996236 cert_utils-0.1.4/tests/test_data/unit_tests/account_001/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      212 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/unit_tests/account_001/info.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)       70 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/unit_tests/account_001/meta.json
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1632 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/unit_tests/account_001/private_key.json
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/unit_tests/account_001/private_key.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)       86 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/unit_tests/account_001/regr.json
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-07 22:41:46.022753 cert_utils-0.1.4/tests/test_data/unit_tests/cert_001/
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1635 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/unit_tests/cert_001/cert.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/unit_tests/cert_001/chain.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1674 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/unit_tests/cert_001/csr.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     2844 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/unit_tests/cert_001/fullchain.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)      387 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/unit_tests/cert_001/info.txt
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/unit_tests/cert_001/privkey.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1516 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/unit_tests/cert_001/test.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-07 22:41:46.027084 cert_utils-0.1.4/tests/test_data/unit_tests/cert_002/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      538 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/unit_tests/cert_002/csr.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)      889 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/unit_tests/cert_002/info.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      887 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/unit_tests/cert_002/privkey.pem
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-07 22:41:46.036868 cert_utils-0.1.4/tests/test_data/unit_tests/cert_003/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1042 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/unit_tests/cert_003/cert.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)      566 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/unit_tests/cert_003/csr.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2250 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/unit_tests/cert_003/fullchain.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)      569 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/unit_tests/cert_003/info.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      891 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/unit_tests/cert_003/privkey.pem
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-07 22:41:46.048582 cert_utils-0.1.4/tests/test_data/unit_tests/cert_004/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1111 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/unit_tests/cert_004/cert.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)      631 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/unit_tests/cert_004/csr.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2319 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/unit_tests/cert_004/fullchain.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)      751 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/unit_tests/cert_004/info.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      887 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/unit_tests/cert_004/privkey.pem
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-07 22:41:46.074885 cert_utils-0.1.4/tests/test_data/unit_tests/cert_005/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      643 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/unit_tests/cert_005/csr.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1146 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/unit_tests/cert_005/info.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      887 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_data/unit_tests/cert_005/privkey.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)    73620 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tests/test_unit.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)      149 2023-06-23 17:24:49.000000 cert_utils-0.1.4/tox.ini
```

### Comparing `cert_utils-0.1.3/LICENSE.txt` & `cert_utils-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/PKG-INFO` & `cert_utils-0.1.4/src/cert_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
-Name: cert_utils
-Version: 0.1.3
+Name: cert-utils
+Version: 0.1.4
 Summary: TLS/SSL Certiicate Utilities
 Home-page: https://github.com/aptise/cert_utils
 Author: Jonathan Vanasco
 Author-email: jonathan@findmeon.com
 License: MIT
 Keywords: web
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -128,7 +129,9 @@
 Python and OpenSSL installations.  Earlier versions of the library
 (within peter_sslers) supported both Python2.7 and Python3, as it was common to
 encounter a machine that did not have Python3 installed.  Although it is still
 common to find these machines, Python2.7 was dropped to take advantage of
 typing.  Depending on the version of OpenSSL installed on a system,
 **cert_utils** will invoke the binary or regex the output to bridge support
 through a unified interface.
+
+
```

### Comparing `cert_utils-0.1.3/README.md` & `cert_utils-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/setup.py` & `cert_utils-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/src/cert_utils/core.py` & `cert_utils-0.1.4/src/cert_utils/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -3626,19 +3626,19 @@
 
 
 class AccountKeyData(object):
     """
     An object encapsulating Account Key data
     """
 
-    key_pem = None
-    key_pem_filepath = None  # if used
-    jwk = None
-    thumbprint = None
-    alg = None
+    key_pem: str
+    key_pem_filepath: Optional[str]
+    jwk: Dict
+    thumbprint: str
+    alg: str
 
     def __init__(
         self,
         key_pem: str,
         key_pem_filepath: Optional[str] = None,
     ):
         """
```

### Comparing `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/fakeleintermediatex1.pem` & `cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/fakeleintermediatex1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/fakelerootx1.pem` & `cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/fakelerootx1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/isrg-root-ocsp-x1.pem` & `cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/isrg-root-ocsp-x1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/isrg-root-x1-cross-signed.pem` & `cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/isrg-root-x1-cross-signed.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/isrg-root-x2-cross-signed.pem` & `cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/isrg-root-x2-cross-signed.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/isrg-root-x2.pem` & `cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/isrg-root-x2.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/isrgrootx1.pem` & `cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/isrgrootx1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/isrgrootx1.pkix` & `cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/isrgrootx1.pkix`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-e1.pem` & `cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/lets-encrypt-e1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-e2.pem` & `cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/lets-encrypt-e2.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-r3-cross-signed.pem` & `cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/lets-encrypt-r3-cross-signed.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-r3.pem` & `cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/lets-encrypt-r3.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-r4-cross-signed.pem` & `cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/lets-encrypt-r4-cross-signed.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-r4.pem` & `cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/lets-encrypt-r4.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-x1-cross-signed.pem` & `cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/lets-encrypt-x1-cross-signed.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-x2-cross-signed.pem` & `cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/lets-encrypt-x2-cross-signed.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-x3-cross-signed.pem` & `cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/lets-encrypt-x3-cross-signed.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/lets-encrypt-x4-cross-signed.pem` & `cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/lets-encrypt-x4-cross-signed.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/letsencryptauthorityx1.pem` & `cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/letsencryptauthorityx1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/letsencryptauthorityx2.pem` & `cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/letsencryptauthorityx2.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/letsencryptauthorityx3.pem` & `cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/letsencryptauthorityx3.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/letsencryptauthorityx4.pem` & `cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/letsencryptauthorityx4.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/trustid-x3-root.p7c` & `cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/trustid-x3-root.p7c`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/src/cert_utils/letsencrypt-certs/trustid-x3-root.pem` & `cert_utils-0.1.4/src/cert_utils/letsencrypt-certs/trustid-x3-root.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/src/cert_utils/letsencrypt_info.py` & `cert_utils-0.1.4/src/cert_utils/letsencrypt_info.py`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/src/cert_utils/model.py` & `cert_utils-0.1.4/src/cert_utils/model.py`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/src/cert_utils/utils.py` & `cert_utils-0.1.4/src/cert_utils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 # stdlib
 import binascii
 import hashlib
 import re
 from typing import List
+from typing import Iterable
 from typing import Union
 
 # ==============================================================================
 
 
 # technically we could end in a dot (\.?)
 RE_domain = re.compile(
     r"""^(?:[A-Z0-9](?:[A-Z0-9-]{0,61}[A-Z0-9])?\.)+(?:[A-Z]{2,6}|[A-Z0-9-]{2,}(?<!-))$""",
     re.I,
 )
 
 # ------------------------------------------------------------------------------
 
 
-def validate_domains(domain_names: List[str]) -> bool:
+def validate_domains(domain_names: Iterable[str]) -> bool:
     """
     Ensures each items of the iterable `domain_names` matches a regular expression.
 
     :param domain_names: (required) An iterable list of strings
     """
     for d in domain_names:
         if not RE_domain.match(d):
             raise ValueError("invalid domain: `%s`", d)
     return True
 
 
-def domains_from_list(domain_names: List[str]) -> List[str]:
+def domains_from_list(domain_names: Iterable[str]) -> List[str]:
     """
     Turns a list of strings into a standardized list of domain names.
 
     Will raise `ValueError("invalid domain")` if non-conforming elements are encountered.
 
     This invokes `validate_domains`, which uses a simple regex to validate each domain in the list.
```

### Comparing `cert_utils-0.1.3/src/cert_utils.egg-info/PKG-INFO` & `cert_utils-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
-Name: cert-utils
-Version: 0.1.3
+Name: cert_utils
+Version: 0.1.4
 Summary: TLS/SSL Certiicate Utilities
 Home-page: https://github.com/aptise/cert_utils
 Author: Jonathan Vanasco
 Author-email: jonathan@findmeon.com
 License: MIT
 Keywords: web
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -128,7 +129,9 @@
 Python and OpenSSL installations.  Earlier versions of the library
 (within peter_sslers) supported both Python2.7 and Python3, as it was common to
 encounter a machine that did not have Python3 installed.  Although it is still
 common to find these machines, Python2.7 was dropped to take advantage of
 typing.  Depending on the version of OpenSSL installed on a system,
 **cert_utils** will invoke the binary or regex the output to bridge support
 through a unified interface.
+
+
```

### Comparing `cert_utils-0.1.3/src/cert_utils.egg-info/SOURCES.txt` & `cert_utils-0.1.4/src/cert_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/_utils.py` & `cert_utils-0.1.4/tests/_utils.py`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/__README__.txt` & `cert_utils-0.1.4/tests/test_data/__README__.txt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/alternate_chains/1/alternate_chains/1/chain.pem` & `cert_utils-0.1.4/tests/test_data/alternate_chains/1/alternate_chains/1/chain.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/alternate_chains/1/alternate_chains/1/fullchain.pem` & `cert_utils-0.1.4/tests/test_data/alternate_chains/1/alternate_chains/1/fullchain.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/alternate_chains/1/alternate_chains/2/chain.pem` & `cert_utils-0.1.4/tests/test_data/alternate_chains/1/alternate_chains/2/chain.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/alternate_chains/1/alternate_chains/2/fullchain.pem` & `cert_utils-0.1.4/tests/test_data/alternate_chains/1/alternate_chains/2/fullchain.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/alternate_chains/1/cert.pem` & `cert_utils-0.1.4/tests/test_data/alternate_chains/1/cert.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/alternate_chains/1/chain.pem` & `cert_utils-0.1.4/tests/test_data/alternate_chains/1/chain.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/alternate_chains/1/fullchain.pem` & `cert_utils-0.1.4/tests/test_data/alternate_chains/1/fullchain.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/alternate_chains/1/privkey.pem` & `cert_utils-0.1.4/tests/test_data/alternate_chains/1/privkey.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-1.pem` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/AcmeAccountKey-1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-2.pem` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/AcmeAccountKey-2.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-3.pem` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/AcmeAccountKey-3.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-4.pem` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/AcmeAccountKey-4.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-5.pem` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/AcmeAccountKey-5.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-account_daily.pem` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-account_daily.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-account_weekly.pem` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-account_weekly.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-global_daily.pem` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-global_daily.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-global_weekly.pem` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-global_weekly.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-single_certificate.pem` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-single_certificate.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/acme_account_1.key` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/acme_account_1.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/acme_account_2.key` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/acme_account_2.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/acme_account_3.key` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/acme_account_3.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/acme_account_4.key` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/acme_account_4.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/acme_account_5.key` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/acme_account_5.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/private_1.key` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/private_1.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/private_2.key` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/private_2.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/private_3.key` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/private_3.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/private_4.key` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/private_4.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/private_5.key` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/private_5.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_1-server.crt` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/selfsigned_1-server.crt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_1-server.csr` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/selfsigned_1-server.csr`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_1-server.key` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/selfsigned_1-server.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_2-server.crt` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/selfsigned_2-server.crt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_2-server.csr` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/selfsigned_2-server.csr`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_2-server.key` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/selfsigned_2-server.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_3-server.crt` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/selfsigned_3-server.crt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_3-server.csr` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/selfsigned_3-server.csr`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_3-server.key` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/selfsigned_3-server.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_4-server.crt` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/selfsigned_4-server.crt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_4-server.csr` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/selfsigned_4-server.csr`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_4-server.key` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/selfsigned_4-server.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_5-server.crt` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/selfsigned_5-server.crt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_5-server.csr` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/selfsigned_5-server.csr`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/key_technology-rsa/selfsigned_5-server.key` & `cert_utils-0.1.4/tests/test_data/key_technology-rsa/selfsigned_5-server.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/long_chains/TestA/__README__.txt` & `cert_utils-0.1.4/tests/test_data/long_chains/TestA/__README__.txt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/long_chains/TestA/_demo.py` & `cert_utils-0.1.4/tests/test_data/long_chains/TestA/_demo.py`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/long_chains/TestA/cert.pem` & `cert_utils-0.1.4/tests/test_data/long_chains/TestA/cert.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/long_chains/TestA/chain_0.pem` & `cert_utils-0.1.4/tests/test_data/long_chains/TestA/chain_0.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/long_chains/TestA/chain_0_bad.pem` & `cert_utils-0.1.4/tests/test_data/long_chains/TestA/chain_0_bad.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/long_chains/TestA/chain_1.pem` & `cert_utils-0.1.4/tests/test_data/long_chains/TestA/chain_1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/long_chains/TestA/chain_2.pem` & `cert_utils-0.1.4/tests/test_data/long_chains/TestA/chain_2.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/long_chains/TestA/root_0.pem` & `cert_utils-0.1.4/tests/test_data/long_chains/TestA/root_0.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/long_chains/TestA/root_1.pem` & `cert_utils-0.1.4/tests/test_data/long_chains/TestA/root_1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/long_chains/TestA/root_2.pem` & `cert_utils-0.1.4/tests/test_data/long_chains/TestA/root_2.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/pebble-certs/cert1.pem` & `cert_utils-0.1.4/tests/test_data/pebble-certs/cert1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/pebble-certs/cert2.pem` & `cert_utils-0.1.4/tests/test_data/pebble-certs/cert2.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/pebble-certs/cert3.pem` & `cert_utils-0.1.4/tests/test_data/pebble-certs/cert3.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/pebble-certs/cert4.pem` & `cert_utils-0.1.4/tests/test_data/pebble-certs/cert4.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/pebble-certs/cert5.pem` & `cert_utils-0.1.4/tests/test_data/pebble-certs/cert5.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/pebble-certs/cert6.pem` & `cert_utils-0.1.4/tests/test_data/pebble-certs/cert6.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/pebble-certs/chain1.pem` & `cert_utils-0.1.4/tests/test_data/pebble-certs/chain1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/pebble-certs/chain2.pem` & `cert_utils-0.1.4/tests/test_data/pebble-certs/chain2.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/pebble-certs/chain3.pem` & `cert_utils-0.1.4/tests/test_data/pebble-certs/chain3.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/pebble-certs/chain4.pem` & `cert_utils-0.1.4/tests/test_data/pebble-certs/chain4.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/pebble-certs/chain5.pem` & `cert_utils-0.1.4/tests/test_data/pebble-certs/chain5.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/pebble-certs/chain6.pem` & `cert_utils-0.1.4/tests/test_data/pebble-certs/chain6.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/pebble-certs/fullchain1.pem` & `cert_utils-0.1.4/tests/test_data/pebble-certs/fullchain1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/pebble-certs/fullchain2.pem` & `cert_utils-0.1.4/tests/test_data/pebble-certs/fullchain2.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/pebble-certs/fullchain3.pem` & `cert_utils-0.1.4/tests/test_data/pebble-certs/fullchain3.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/pebble-certs/fullchain4.pem` & `cert_utils-0.1.4/tests/test_data/pebble-certs/fullchain4.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/pebble-certs/fullchain5.pem` & `cert_utils-0.1.4/tests/test_data/pebble-certs/fullchain5.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/pebble-certs/fullchain6.pem` & `cert_utils-0.1.4/tests/test_data/pebble-certs/fullchain6.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/pebble-certs/privkey1.pem` & `cert_utils-0.1.4/tests/test_data/pebble-certs/privkey1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/pebble-certs/privkey2.pem` & `cert_utils-0.1.4/tests/test_data/pebble-certs/privkey2.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/pebble-certs/privkey3.pem` & `cert_utils-0.1.4/tests/test_data/pebble-certs/privkey3.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/pebble-certs/privkey4.pem` & `cert_utils-0.1.4/tests/test_data/pebble-certs/privkey4.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/pebble-certs/privkey5.pem` & `cert_utils-0.1.4/tests/test_data/pebble-certs/privkey5.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/pebble-certs/privkey6.pem` & `cert_utils-0.1.4/tests/test_data/pebble-certs/privkey6.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/unit_tests/_support/account.key` & `cert_utils-0.1.4/tests/test_data/unit_tests/_support/account.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/unit_tests/_support/info.txt` & `cert_utils-0.1.4/tests/test_data/unit_tests/_support/info.txt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/unit_tests/account_001/private_key.json` & `cert_utils-0.1.4/tests/test_data/unit_tests/account_001/private_key.json`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/unit_tests/account_001/private_key.pem` & `cert_utils-0.1.4/tests/test_data/unit_tests/account_001/private_key.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/unit_tests/cert_001/cert.pem` & `cert_utils-0.1.4/tests/test_data/unit_tests/cert_001/cert.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/unit_tests/cert_001/chain.pem` & `cert_utils-0.1.4/tests/test_data/unit_tests/cert_001/chain.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/unit_tests/cert_001/csr.pem` & `cert_utils-0.1.4/tests/test_data/unit_tests/cert_001/csr.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/unit_tests/cert_001/fullchain.pem` & `cert_utils-0.1.4/tests/test_data/unit_tests/cert_001/fullchain.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/unit_tests/cert_001/privkey.pem` & `cert_utils-0.1.4/tests/test_data/unit_tests/cert_001/privkey.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/unit_tests/cert_001/test.py` & `cert_utils-0.1.4/tests/test_data/unit_tests/cert_001/test.py`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/unit_tests/cert_002/csr.pem` & `cert_utils-0.1.4/tests/test_data/unit_tests/cert_002/csr.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/unit_tests/cert_002/info.txt` & `cert_utils-0.1.4/tests/test_data/unit_tests/cert_002/info.txt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/unit_tests/cert_002/privkey.pem` & `cert_utils-0.1.4/tests/test_data/unit_tests/cert_002/privkey.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/unit_tests/cert_003/cert.pem` & `cert_utils-0.1.4/tests/test_data/unit_tests/cert_003/cert.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/unit_tests/cert_003/csr.pem` & `cert_utils-0.1.4/tests/test_data/unit_tests/cert_003/csr.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/unit_tests/cert_003/fullchain.pem` & `cert_utils-0.1.4/tests/test_data/unit_tests/cert_003/fullchain.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/unit_tests/cert_003/info.txt` & `cert_utils-0.1.4/tests/test_data/unit_tests/cert_003/info.txt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/unit_tests/cert_003/privkey.pem` & `cert_utils-0.1.4/tests/test_data/unit_tests/cert_003/privkey.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/unit_tests/cert_004/cert.pem` & `cert_utils-0.1.4/tests/test_data/unit_tests/cert_004/cert.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/unit_tests/cert_004/csr.pem` & `cert_utils-0.1.4/tests/test_data/unit_tests/cert_004/csr.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/unit_tests/cert_004/fullchain.pem` & `cert_utils-0.1.4/tests/test_data/unit_tests/cert_004/fullchain.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/unit_tests/cert_004/info.txt` & `cert_utils-0.1.4/tests/test_data/unit_tests/cert_004/info.txt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/unit_tests/cert_004/privkey.pem` & `cert_utils-0.1.4/tests/test_data/unit_tests/cert_004/privkey.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/unit_tests/cert_005/csr.pem` & `cert_utils-0.1.4/tests/test_data/unit_tests/cert_005/csr.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/unit_tests/cert_005/info.txt` & `cert_utils-0.1.4/tests/test_data/unit_tests/cert_005/info.txt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_data/unit_tests/cert_005/privkey.pem` & `cert_utils-0.1.4/tests/test_data/unit_tests/cert_005/privkey.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.3/tests/test_unit.py` & `cert_utils-0.1.4/tests/test_unit.py`

 * *Files identical despite different names*

