# Comparing `tmp/github-secret-syncer-0.0.6.tar.gz` & `tmp/github-secret-syncer-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github-secret-syncer-0.0.6.tar", last modified: Mon Jul  3 08:33:42 2023, max compression
+gzip compressed data, was "github-secret-syncer-0.0.7.tar", last modified: Sat Jul  8 09:45:18 2023, max compression
```

## Comparing `github-secret-syncer-0.0.6.tar` & `github-secret-syncer-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-03 08:33:42.112405 github-secret-syncer-0.0.6/
--rw-r--r--   0 j3ymac     (501) staff       (20)     1066 2023-06-30 17:47:40.000000 github-secret-syncer-0.0.6/LICENSE
--rw-r--r--   0 j3ymac     (501) staff       (20)     1223 2023-07-03 08:33:42.112264 github-secret-syncer-0.0.6/PKG-INFO
--rw-r--r--   0 j3ymac     (501) staff       (20)      741 2023-07-01 07:55:17.000000 github-secret-syncer-0.0.6/README.md
-drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-03 08:33:42.111489 github-secret-syncer-0.0.6/github_secret_syncer/
--rw-r--r--   0 j3ymac     (501) staff       (20)     4623 2023-06-30 18:17:38.000000 github-secret-syncer-0.0.6/github_secret_syncer/__init__.py
-drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-03 08:33:42.112046 github-secret-syncer-0.0.6/github_secret_syncer.egg-info/
--rw-r--r--   0 j3ymac     (501) staff       (20)     1223 2023-07-03 08:33:42.000000 github-secret-syncer-0.0.6/github_secret_syncer.egg-info/PKG-INFO
--rw-r--r--   0 j3ymac     (501) staff       (20)      235 2023-07-03 08:33:42.000000 github-secret-syncer-0.0.6/github_secret_syncer.egg-info/SOURCES.txt
--rw-r--r--   0 j3ymac     (501) staff       (20)        1 2023-07-03 08:33:42.000000 github-secret-syncer-0.0.6/github_secret_syncer.egg-info/dependency_links.txt
--rw-r--r--   0 j3ymac     (501) staff       (20)       21 2023-07-03 08:33:42.000000 github-secret-syncer-0.0.6/github_secret_syncer.egg-info/top_level.txt
--rw-r--r--   0 j3ymac     (501) staff       (20)       38 2023-07-03 08:33:42.112454 github-secret-syncer-0.0.6/setup.cfg
--rw-r--r--   0 j3ymac     (501) staff       (20)      733 2023-07-01 07:55:22.000000 github-secret-syncer-0.0.6/setup.py
+drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-08 09:45:18.874470 github-secret-syncer-0.0.7/
+-rw-r--r--   0 j3ymac     (501) staff       (20)     1066 2023-06-30 17:47:40.000000 github-secret-syncer-0.0.7/LICENSE
+-rw-r--r--   0 j3ymac     (501) staff       (20)     1216 2023-07-08 09:45:18.874256 github-secret-syncer-0.0.7/PKG-INFO
+-rw-r--r--   0 j3ymac     (501) staff       (20)      734 2023-07-08 09:44:30.000000 github-secret-syncer-0.0.7/README.md
+drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-08 09:45:18.873089 github-secret-syncer-0.0.7/github_secret_syncer/
+-rw-r--r--   0 j3ymac     (501) staff       (20)     4525 2023-07-08 09:29:14.000000 github-secret-syncer-0.0.7/github_secret_syncer/__init__.py
+drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-08 09:45:18.873702 github-secret-syncer-0.0.7/github_secret_syncer.egg-info/
+-rw-r--r--   0 j3ymac     (501) staff       (20)     1216 2023-07-08 09:45:18.000000 github-secret-syncer-0.0.7/github_secret_syncer.egg-info/PKG-INFO
+-rw-r--r--   0 j3ymac     (501) staff       (20)      235 2023-07-08 09:45:18.000000 github-secret-syncer-0.0.7/github_secret_syncer.egg-info/SOURCES.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)        1 2023-07-08 09:45:18.000000 github-secret-syncer-0.0.7/github_secret_syncer.egg-info/dependency_links.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)       21 2023-07-08 09:45:18.000000 github-secret-syncer-0.0.7/github_secret_syncer.egg-info/top_level.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)       38 2023-07-08 09:45:18.874526 github-secret-syncer-0.0.7/setup.cfg
+-rw-r--r--   0 j3ymac     (501) staff       (20)      733 2023-07-08 09:44:16.000000 github-secret-syncer-0.0.7/setup.py
```

### Comparing `github-secret-syncer-0.0.6/LICENSE` & `github-secret-syncer-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `github-secret-syncer-0.0.6/PKG-INFO` & `github-secret-syncer-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github-secret-syncer
-Version: 0.0.6
+Version: 0.0.7
 Summary: Github Secret Syncer.
 Home-page: https://github.com/thejimmylin/github-secret-syncer
 Author: thejimmylin
 Author-email: b00502013@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -37,15 +37,15 @@
 
 base_dir = Path(__file__).parent
 
 github_secret_syncer.sync_secrets(
     dotenv_path=base_dir / ".env",
     owner="your_github_username",
     repo="your_github_repo_name",
-    github_pat="your_github_personal_access_token",
+    pat="your_github_personal_access_token",
 )
 ```
 
 You will get some output like this:
 
 ![Screenshot](https://raw.githubusercontent.com/thejimmylin/github-secret-syncer/master/docs/quickstart.png)
```

### Comparing `github-secret-syncer-0.0.6/README.md` & `github-secret-syncer-0.0.7/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -21,14 +21,14 @@
 
 base_dir = Path(__file__).parent
 
 github_secret_syncer.sync_secrets(
     dotenv_path=base_dir / ".env",
     owner="your_github_username",
     repo="your_github_repo_name",
-    github_pat="your_github_personal_access_token",
+    pat="your_github_personal_access_token",
 )
 ```
 
 You will get some output like this:
 
 ![Screenshot](https://raw.githubusercontent.com/thejimmylin/github-secret-syncer/master/docs/quickstart.png)
```

### Comparing `github-secret-syncer-0.0.6/github_secret_syncer/__init__.py` & `github-secret-syncer-0.0.7/github_secret_syncer/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,33 +27,33 @@
 
 
 class GithubSecretManager:
     """Manage Github Secrets"""
 
     _public_key: PublicKey | None
 
-    def __init__(self, owner: str, repo: str, github_pat: str, github_api_version: str = "2022-11-28"):
+    def __init__(self, owner: str, repo: str, pat: str, api_version: str = "2022-11-28"):
         self.owner = owner
         self.repo = repo
-        self.github_pat = github_pat
-        self.github_api_version = github_api_version
+        self.pat = pat
+        self.api_version = api_version
         self._public_key = None
 
     @property
     def public_key(self) -> PublicKey:
         if self._public_key is None:
             self._public_key = self._get_public_key()
         return self._public_key
 
     @property
     def headers(self) -> dict[str, str]:
         return {
             "Accept": "application/vnd.github+json",
-            "Authorization": f"Bearer {self.github_pat}",
-            "X-GitHub-Api-Version": f"{self.github_api_version}",
+            "Authorization": f"Bearer {self.pat}",
+            "X-GitHub-Api-Version": f"{self.api_version}",
         }
 
     def _get_public_key(self) -> PublicKey:
         url = f"https://api.github.com/repos/{self.owner}/{self.repo}/actions/secrets/public-key"
         response = requests.get(url, headers=self.headers)
         public_key = response.json()
         return public_key
@@ -86,37 +86,37 @@
             raise ValueError(f"Failed to delete secret: `{response = }`, `{response.json() = }`")
 
 
 def sync_secrets(
     dotenv_path: Path,
     owner: str,
     repo: str,
-    github_pat: str,
+    pat: str,
     delete_missing: bool = True,
-    github_api_version: str = "2022-11-28",
+    api_version: str = "2022-11-28",
 ) -> None:
     """Sync secrets from dotenv to Github Actions
 
     This function can be seen as an example of how to use GithubSecretManager.
     Feel free to copy and modify it to fit your needs.
     """
-    secret_manager = GithubSecretManager(owner, repo, github_pat, github_api_version)
-    github_secrets = secret_manager.list_repo_secrets()
+    secret_manager = GithubSecretManager(owner, repo, pat, api_version)
+    secrets = secret_manager.list_repo_secrets()
     _dotenv_secrets = dotenv.dotenv_values(dotenv_path)
 
     # Ignore secrets like `foo` (without `=`)
     # This will not ignore secrets like `bar=` (it's value will be `""`)
     dotenv_secrets: dict[str, str] = {}
     for secret_name, secret_value in _dotenv_secrets.items():
         if secret_value is not None:
             dotenv_secrets[secret_name] = secret_value
 
     if delete_missing:
         # Delete secrets that are in Github but not in dotenv
-        for secret in github_secrets["secrets"]:
+        for secret in secrets["secrets"]:
             if secret["name"] not in dotenv_secrets:
                 logger.info(f"Deleting secret `{secret['name']}` from Github")
                 secret_manager.delete_repo_secret(secret["name"])
 
     # Put secrets that are in dotenv
     for secret_name, secret_value in dotenv_secrets.items():
         logger.info(f"Putting secret `{secret_name}` to Github")
```

### Comparing `github-secret-syncer-0.0.6/github_secret_syncer.egg-info/PKG-INFO` & `github-secret-syncer-0.0.7/github_secret_syncer.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github-secret-syncer
-Version: 0.0.6
+Version: 0.0.7
 Summary: Github Secret Syncer.
 Home-page: https://github.com/thejimmylin/github-secret-syncer
 Author: thejimmylin
 Author-email: b00502013@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -37,15 +37,15 @@
 
 base_dir = Path(__file__).parent
 
 github_secret_syncer.sync_secrets(
     dotenv_path=base_dir / ".env",
     owner="your_github_username",
     repo="your_github_repo_name",
-    github_pat="your_github_personal_access_token",
+    pat="your_github_personal_access_token",
 )
 ```
 
 You will get some output like this:
 
 ![Screenshot](https://raw.githubusercontent.com/thejimmylin/github-secret-syncer/master/docs/quickstart.png)
```

### Comparing `github-secret-syncer-0.0.6/setup.py` & `github-secret-syncer-0.0.7/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 base_dir = Path(__file__).parent.resolve()
 long_description = (base_dir / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="github-secret-syncer",
-    version="0.0.6",
+    version="0.0.7",
     author="thejimmylin",
     author_email="b00502013@gmail.com",
     description="Github Secret Syncer.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/thejimmylin/github-secret-syncer",
     packages=setuptools.find_packages(),
```

