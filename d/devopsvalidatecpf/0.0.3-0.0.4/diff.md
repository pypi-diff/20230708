# Comparing `tmp/devopsvalidatecpf-0.0.3.tar.gz` & `tmp/devopsvalidatecpf-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devopsvalidatecpf-0.0.3.tar", last modified: Sun Jul  2 21:16:17 2023, max compression
+gzip compressed data, was "devopsvalidatecpf-0.0.4.tar", last modified: Sat Jul  8 21:10:15 2023, max compression
```

## Comparing `devopsvalidatecpf-0.0.3.tar` & `devopsvalidatecpf-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:16:17.119365 devopsvalidatecpf-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-02 21:16:17.119365 devopsvalidatecpf-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-02 21:16:07.000000 devopsvalidatecpf-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-02 21:16:07.000000 devopsvalidatecpf-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-02 21:16:07.000000 devopsvalidatecpf-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 21:16:17.119365 devopsvalidatecpf-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:16:17.119365 devopsvalidatecpf-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:16:17.119365 devopsvalidatecpf-0.0.3/src/devopsvalidatecpf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-02 21:16:17.000000 devopsvalidatecpf-0.0.3/src/devopsvalidatecpf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-02 21:16:17.000000 devopsvalidatecpf-0.0.3/src/devopsvalidatecpf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 21:16:17.000000 devopsvalidatecpf-0.0.3/src/devopsvalidatecpf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-02 21:16:17.000000 devopsvalidatecpf-0.0.3/src/devopsvalidatecpf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-02 21:16:17.000000 devopsvalidatecpf-0.0.3/src/devopsvalidatecpf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:16:17.119365 devopsvalidatecpf-0.0.3/src/validate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 21:16:07.000000 devopsvalidatecpf-0.0.3/src/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-02 21:16:07.000000 devopsvalidatecpf-0.0.3/src/validate/validate_cpf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:16:17.119365 devopsvalidatecpf-0.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-02 21:16:07.000000 devopsvalidatecpf-0.0.3/test/test_validate_cpf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:10:15.062702 devopsvalidatecpf-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-08 21:10:15.062702 devopsvalidatecpf-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-08 21:10:03.000000 devopsvalidatecpf-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-08 21:10:03.000000 devopsvalidatecpf-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-08 21:10:03.000000 devopsvalidatecpf-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 21:10:15.062702 devopsvalidatecpf-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:10:15.058702 devopsvalidatecpf-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:10:15.062702 devopsvalidatecpf-0.0.4/src/devopsvalidatecpf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-08 21:10:15.000000 devopsvalidatecpf-0.0.4/src/devopsvalidatecpf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-08 21:10:15.000000 devopsvalidatecpf-0.0.4/src/devopsvalidatecpf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 21:10:15.000000 devopsvalidatecpf-0.0.4/src/devopsvalidatecpf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-08 21:10:15.000000 devopsvalidatecpf-0.0.4/src/devopsvalidatecpf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-08 21:10:15.000000 devopsvalidatecpf-0.0.4/src/devopsvalidatecpf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:10:15.062702 devopsvalidatecpf-0.0.4/src/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 21:10:03.000000 devopsvalidatecpf-0.0.4/src/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-08 21:10:03.000000 devopsvalidatecpf-0.0.4/src/validate/validate_cpf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:10:15.062702 devopsvalidatecpf-0.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-08 21:10:03.000000 devopsvalidatecpf-0.0.4/test/test_validate_cpf.py
```

### Comparing `devopsvalidatecpf-0.0.3/PKG-INFO` & `devopsvalidatecpf-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devopsvalidatecpf
-Version: 0.0.3
+Version: 0.0.4
 Summary: DevOps course CPF validation package
 Author-email: Ezequiel Lima <ezequiel_lima@hotmail.com>
 Project-URL: Homepage, https://github.com/ezequielcdelima/projeto-final-puc-devops
 Project-URL: Bug Tracker, https://github.com/ezequielcdelima/projeto-final-puc-devops/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `devopsvalidatecpf-0.0.3/pyproject.toml` & `devopsvalidatecpf-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "devopsvalidatecpf"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Ezequiel Lima", email="ezequiel_lima@hotmail.com" },
 ]
 description = "DevOps course CPF validation package"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `devopsvalidatecpf-0.0.3/src/devopsvalidatecpf.egg-info/PKG-INFO` & `devopsvalidatecpf-0.0.4/src/devopsvalidatecpf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devopsvalidatecpf
-Version: 0.0.3
+Version: 0.0.4
 Summary: DevOps course CPF validation package
 Author-email: Ezequiel Lima <ezequiel_lima@hotmail.com>
 Project-URL: Homepage, https://github.com/ezequielcdelima/projeto-final-puc-devops
 Project-URL: Bug Tracker, https://github.com/ezequielcdelima/projeto-final-puc-devops/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `devopsvalidatecpf-0.0.3/src/validate/validate_cpf.py` & `devopsvalidatecpf-0.0.4/src/validate/validate_cpf.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 import re
 
 
 def validar_cpf(cpf):
+    """
+    Checks if the CPF informed by is a valid or invalid CPF.
+
+    :param string: CPF
+    :return dict: CPF numbering and true if valid CPF or false if invalid CPF.
+    """
+
     cpf = re.sub(u'[^0-9]', '', cpf)
 
     if len(cpf) != 11 or not cpf.isdigit():
         return {'cpf': cpf, 'valido': False}
 
     # Verifica o primeiro dígito verificador
     soma = sum(int(cpf[i]) * (10 - i) for i in range(9))
```

