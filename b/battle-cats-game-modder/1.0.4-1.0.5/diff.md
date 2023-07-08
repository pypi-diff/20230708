# Comparing `tmp/battle-cats-game-modder-1.0.4.tar.gz` & `tmp/battle-cats-game-modder-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "battle-cats-game-modder-1.0.4.tar", last modified: Tue May 24 07:27:54 2022, max compression
+gzip compressed data, was "battle-cats-game-modder-1.0.5.tar", last modified: Sat Jul  8 17:59:57 2023, max compression
```

## Comparing `battle-cats-game-modder-1.0.4.tar` & `battle-cats-game-modder-1.0.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2022-05-24 07:27:54.796713 battle-cats-game-modder-1.0.4/
--rw-rw-rw-   0        0        0     1092 2022-04-24 14:40:07.000000 battle-cats-game-modder-1.0.4/LICENSE
--rw-rw-rw-   0        0        0       41 2022-04-24 14:40:31.000000 battle-cats-game-modder-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     6504 2022-05-24 07:27:54.796212 battle-cats-game-modder-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     6039 2022-05-24 07:25:44.000000 battle-cats-game-modder-1.0.4/README.md
--rw-rw-rw-   0        0        0       86 2022-04-19 07:56:57.000000 battle-cats-game-modder-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-05-24 07:27:54.797213 battle-cats-game-modder-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      981 2022-05-20 17:49:11.000000 battle-cats-game-modder-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2022-05-24 07:27:54.752175 battle-cats-game-modder-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2022-05-24 07:27:54.764686 battle-cats-game-modder-1.0.4/src/BCGM_Python/
--rw-rw-rw-   0        0        0        0 2022-04-24 14:42:22.000000 battle-cats-game-modder-1.0.4/src/BCGM_Python/__init__.py
--rw-rw-rw-   0        0        0      309 2022-04-24 15:18:00.000000 battle-cats-game-modder-1.0.4/src/BCGM_Python/__main__.py
-drwxrwxrwx   0        0        0        0 2022-05-24 07:27:54.767187 battle-cats-game-modder-1.0.4/src/BCGM_Python/encrypt_decrypt/
--rw-rw-rw-   0        0        0        0 2022-04-24 14:44:24.000000 battle-cats-game-modder-1.0.4/src/BCGM_Python/encrypt_decrypt/__init__.py
--rw-rw-rw-   0        0        0     3560 2022-04-18 10:01:01.000000 battle-cats-game-modder-1.0.4/src/BCGM_Python/encrypt_decrypt/decrypt_pack.py
--rw-rw-rw-   0        0        0     3945 2022-04-24 14:50:38.000000 battle-cats-game-modder-1.0.4/src/BCGM_Python/encrypt_decrypt/encrypt_pack.py
--rw-rw-rw-   0        0        0     3093 2022-04-24 14:48:45.000000 battle-cats-game-modder-1.0.4/src/BCGM_Python/feature_handler.py
-drwxrwxrwx   0        0        0        0 2022-05-24 07:27:54.771191 battle-cats-game-modder-1.0.4/src/BCGM_Python/file_mods/
--rw-rw-rw-   0        0        0        0 2022-04-24 14:48:55.000000 battle-cats-game-modder-1.0.4/src/BCGM_Python/file_mods/__init__.py
--rw-rw-rw-   0        0        0     3001 2022-04-24 14:49:20.000000 battle-cats-game-modder-1.0.4/src/BCGM_Python/file_mods/enemy_mod.py
--rw-rw-rw-   0        0        0     3570 2022-05-20 17:47:29.000000 battle-cats-game-modder-1.0.4/src/BCGM_Python/file_mods/stage_mod.py
--rw-rw-rw-   0        0        0     4007 2022-04-24 14:49:06.000000 battle-cats-game-modder-1.0.4/src/BCGM_Python/file_mods/unit_mod.py
-drwxrwxrwx   0        0        0        0 2022-05-24 07:27:54.772192 battle-cats-game-modder-1.0.4/src/BCGM_Python/files/
--rw-rw-rw-   0        0        0        5 2022-05-24 07:26:30.000000 battle-cats-game-modder-1.0.4/src/BCGM_Python/files/version.txt
--rw-rw-rw-   0        0        0    10082 2022-05-24 07:25:44.000000 battle-cats-game-modder-1.0.4/src/BCGM_Python/helper.py
-drwxrwxrwx   0        0        0        0 2022-05-24 07:27:54.779199 battle-cats-game-modder-1.0.4/src/BCGM_Python/libnative/
--rw-rw-rw-   0        0        0        0 2022-04-24 14:46:25.000000 battle-cats-game-modder-1.0.4/src/BCGM_Python/libnative/__init__.py
--rw-rw-rw-   0        0        0     3754 2022-05-20 17:44:31.000000 battle-cats-game-modder-1.0.4/src/BCGM_Python/libnative/find_order.py
--rw-rw-rw-   0        0        0     2084 2022-04-24 14:46:41.000000 battle-cats-game-modder-1.0.4/src/BCGM_Python/libnative/write_libnative_md5.py
-drwxrwxrwx   0        0        0        0 2022-05-24 07:27:54.795212 battle-cats-game-modder-1.0.4/src/battle_cats_game_modder.egg-info/
--rw-rw-rw-   0        0        0     6504 2022-05-24 07:27:54.000000 battle-cats-game-modder-1.0.4/src/battle_cats_game_modder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      879 2022-05-24 07:27:54.000000 battle-cats-game-modder-1.0.4/src/battle_cats_game_modder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-24 07:27:54.000000 battle-cats-game-modder-1.0.4/src/battle_cats_game_modder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2022-05-24 07:27:54.000000 battle-cats-game-modder-1.0.4/src/battle_cats_game_modder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-05-24 07:27:54.000000 battle-cats-game-modder-1.0.4/src/battle_cats_game_modder.egg-info/top_level.txt
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-07-08 17:59:57.379961 battle-cats-game-modder-1.0.5/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     1071 2023-07-08 17:58:22.000000 battle-cats-game-modder-1.0.5/LICENSE
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       41 2023-07-08 17:58:22.000000 battle-cats-game-modder-1.0.5/MANIFEST.in
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3919 2023-07-08 17:59:57.379961 battle-cats-game-modder-1.0.5/PKG-INFO
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3467 2023-07-08 17:58:22.000000 battle-cats-game-modder-1.0.5/README.md
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       84 2023-07-08 17:58:22.000000 battle-cats-game-modder-1.0.5/pyproject.toml
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       38 2023-07-08 17:59:57.379961 battle-cats-game-modder-1.0.5/setup.cfg
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      960 2023-07-08 17:58:42.000000 battle-cats-game-modder-1.0.5/setup.py
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-07-08 17:59:57.376628 battle-cats-game-modder-1.0.5/src/
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-07-08 17:59:57.379961 battle-cats-game-modder-1.0.5/src/BCGM_Python/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-07-08 17:58:22.000000 battle-cats-game-modder-1.0.5/src/BCGM_Python/__init__.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      293 2023-07-08 17:58:22.000000 battle-cats-game-modder-1.0.5/src/BCGM_Python/__main__.py
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-07-08 17:59:57.379961 battle-cats-game-modder-1.0.5/src/BCGM_Python/encrypt_decrypt/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-07-08 17:58:22.000000 battle-cats-game-modder-1.0.5/src/BCGM_Python/encrypt_decrypt/__init__.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3462 2023-07-08 17:58:22.000000 battle-cats-game-modder-1.0.5/src/BCGM_Python/encrypt_decrypt/decrypt_pack.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3843 2023-07-08 17:58:22.000000 battle-cats-game-modder-1.0.5/src/BCGM_Python/encrypt_decrypt/encrypt_pack.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3023 2023-07-08 17:58:22.000000 battle-cats-game-modder-1.0.5/src/BCGM_Python/feature_handler.py
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-07-08 17:59:57.379961 battle-cats-game-modder-1.0.5/src/BCGM_Python/file_mods/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-07-08 17:58:22.000000 battle-cats-game-modder-1.0.5/src/BCGM_Python/file_mods/__init__.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2956 2023-07-08 17:58:22.000000 battle-cats-game-modder-1.0.5/src/BCGM_Python/file_mods/enemy_mod.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3469 2023-07-08 17:58:22.000000 battle-cats-game-modder-1.0.5/src/BCGM_Python/file_mods/stage_mod.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3933 2023-07-08 17:58:22.000000 battle-cats-game-modder-1.0.5/src/BCGM_Python/file_mods/unit_mod.py
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-07-08 17:59:57.379961 battle-cats-game-modder-1.0.5/src/BCGM_Python/files/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)        5 2023-07-08 17:59:35.000000 battle-cats-game-modder-1.0.5/src/BCGM_Python/files/version.txt
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)    10082 2023-07-08 17:58:22.000000 battle-cats-game-modder-1.0.5/src/BCGM_Python/helper.py
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-07-08 17:59:57.379961 battle-cats-game-modder-1.0.5/src/BCGM_Python/libnative/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-07-08 17:58:22.000000 battle-cats-game-modder-1.0.5/src/BCGM_Python/libnative/__init__.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3627 2023-07-08 17:58:22.000000 battle-cats-game-modder-1.0.5/src/BCGM_Python/libnative/find_order.py
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     2030 2023-07-08 17:58:22.000000 battle-cats-game-modder-1.0.5/src/BCGM_Python/libnative/write_libnative_md5.py
+drwxr-xr-x   0 fieryhenry  (1000) fieryhenry  (1000)        0 2023-07-08 17:59:57.379961 battle-cats-game-modder-1.0.5/src/battle_cats_game_modder.egg-info/
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)     3919 2023-07-08 17:59:57.000000 battle-cats-game-modder-1.0.5/src/battle_cats_game_modder.egg-info/PKG-INFO
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)      879 2023-07-08 17:59:57.000000 battle-cats-game-modder-1.0.5/src/battle_cats_game_modder.egg-info/SOURCES.txt
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)        1 2023-07-08 17:59:57.000000 battle-cats-game-modder-1.0.5/src/battle_cats_game_modder.egg-info/dependency_links.txt
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       56 2023-07-08 17:59:57.000000 battle-cats-game-modder-1.0.5/src/battle_cats_game_modder.egg-info/requires.txt
+-rw-r--r--   0 fieryhenry  (1000) fieryhenry  (1000)       12 2023-07-08 17:59:57.000000 battle-cats-game-modder-1.0.5/src/battle_cats_game_modder.egg-info/top_level.txt
```

### Comparing `battle-cats-game-modder-1.0.4/LICENSE` & `battle-cats-game-modder-1.0.5/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) [2022] [fieryhenry]
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) [2022] [fieryhenry]
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `battle-cats-game-modder-1.0.4/setup.py` & `battle-cats-game-modder-1.0.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-import setuptools
-
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
-
-with open("src/BCGM_Python/files/version.txt", "r", encoding="utf-8") as fh:
-    version = fh.read()
-
-setuptools.setup(
-    name="battle-cats-game-modder",
-    version=version,
-    author="fieryhenry",
-    description="A battle cats tool for modifying, encrypting, and decrypting game files",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/fieryhenry/BCGM-Python",
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    package_dir={"" : "src"},
-    packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.6",
-    install_requires=[
-        "colored", "tk", "alive-progress", "pycryptodomex", "requests"
-    ],
-    include_package_data=True
+import setuptools
+
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
+with open("src/BCGM_Python/files/version.txt", "r", encoding="utf-8") as fh:
+    version = fh.read()
+
+setuptools.setup(
+    name="battle-cats-game-modder",
+    version=version,
+    author="fieryhenry",
+    description="A battle cats tool for modifying, encrypting, and decrypting game files",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/fieryhenry/BCGM-Python",
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    package_dir={"" : "src"},
+    packages=setuptools.find_packages(where="src"),
+    python_requires=">=3.6",
+    install_requires=[
+        "colored==1.4.4", "tk", "alive-progress", "pycryptodomex", "requests"
+    ],
+    include_package_data=True
 )
```

### Comparing `battle-cats-game-modder-1.0.4/src/BCGM_Python/encrypt_decrypt/decrypt_pack.py` & `battle-cats-game-modder-1.0.5/src/BCGM_Python/encrypt_decrypt/decrypt_pack.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-import helper
-import os
-from Cryptodome.Cipher import AES
-from alive_progress import alive_bar 
-
-output_path = "game_files"
-lists_paths = "decrypted_lists"
-
-def unpack_list(ls_file):
-    data = helper.open_file_b(ls_file)
-    key = helper.md5_str("pack")
-    cipher = AES.new(key, AES.MODE_ECB)
-    decrypted_data = cipher.decrypt(data)
-    return decrypted_data
-
-def decrypt_pack(chunk_data, jp, pk_name):
-    aes_mode = AES.MODE_CBC
-    if jp:
-        key = bytes.fromhex("d754868de89d717fa9e7b06da45ae9e3")
-        iv = bytes.fromhex("40b2131a9f388ad4e5002a98118f6128")
-    else:
-        key = bytes.fromhex("0ad39e4aeaf55aa717feb1825edef521")
-        iv = bytes.fromhex("d1d7e708091941d90cdf8aa5f30bb0c2")
-    
-    if "server" in pk_name.lower():
-        key = helper.md5_str("battlecats")
-        iv = None
-        aes_mode = AES.MODE_ECB
-    if iv:
-        cipher = AES.new(key, aes_mode, iv)
-    else:
-        cipher = AES.new(key, aes_mode)
-    decrypted_data = cipher.decrypt(chunk_data)
-    return decrypted_data
-
-
-def unpack_pack(pk_file_path, ls_data, jp, base_path):
-    list_data = ls_data.decode("utf-8")
-    split_data = helper.parse_csv_file(None, list_data.split("\n"), 3)
-
-    pack_data = helper.open_file_b(pk_file_path)
-
-    with alive_bar(len(split_data)) as bar:
-        for i in range(len(split_data)):
-            file = split_data[i]
-            
-            name = file[0]
-            start_offset = int(file[1])
-            length = int(file[2])
-
-            pk_chunk = pack_data[start_offset:start_offset+length]
-            base_name = os.path.basename(pk_file_path)
-            if "imagedatalocal" in base_name.lower():
-                pk_chunk_decrypted = pk_chunk
-            else:
-                pk_chunk_decrypted = decrypt_pack(pk_chunk, jp, base_name)
-            helper.write_file_b(os.path.join(base_path, name), pk_chunk_decrypted)
-            bar()
-
-def decrypt():
-    jp = helper.coloured_text("Are you using game version &jp& 10.8 and up? (y/n):", is_input=True)
-    jp = helper.validate_bool(jp)
-    
-    pack_paths = helper.select_files("Select .pack files", [(".pack files", "*.pack")], False)
-    if not pack_paths:
-        helper.coloured_text("Please select .pack files", base=helper.red)
-        return
-    helper.check_and_create_dir(output_path)
-    
-    file_groups = find_lists(pack_paths)
-
-
-    for i in range(len(file_groups)):
-        file_group = file_groups[i]
-
-        ls_base_name = os.path.basename(file_group["list"])
-        pk_base_name = os.path.basename(file_group["pack"])
-
-        name = pk_base_name.rstrip(".pack")
-        path = os.path.join(output_path, name)
-
-        helper.check_and_create_dir(path)
-        helper.check_and_create_dir(lists_paths)
-
-        ls_data = unpack_list(file_group["list"])
-        helper.write_file_b(os.path.join(lists_paths, ls_base_name), ls_data)
-
-        helper.coloured_text(f"\n&{i+1}&\t\t{name}\t{i+1} / {len(file_groups)}", base=helper.green, new=helper.white)
-        unpack_pack(file_group["pack"], ls_data, jp, path)
-    helper.coloured_text(f"\nSuccessfully decrypted all .pack files to: &{output_path}&", base=helper.green, new=helper.white)
-def find_lists(pack_paths):
-    files = []
-    for pack_path in pack_paths:
-        directory = os.path.dirname(pack_path)
-        ls_path = os.path.join(directory, pack_path.rstrip(".pack") + ".list")
-        group = {"pack" : pack_path, "list" : ls_path}
-        files.append(group)
-    return files
+import helper
+import os
+from Cryptodome.Cipher import AES
+from alive_progress import alive_bar 
+
+output_path = "game_files"
+lists_paths = "decrypted_lists"
+
+def unpack_list(ls_file):
+    data = helper.open_file_b(ls_file)
+    key = helper.md5_str("pack")
+    cipher = AES.new(key, AES.MODE_ECB)
+    decrypted_data = cipher.decrypt(data)
+    return decrypted_data
+
+def decrypt_pack(chunk_data, jp, pk_name):
+    aes_mode = AES.MODE_CBC
+    if jp:
+        key = bytes.fromhex("d754868de89d717fa9e7b06da45ae9e3")
+        iv = bytes.fromhex("40b2131a9f388ad4e5002a98118f6128")
+    else:
+        key = bytes.fromhex("0ad39e4aeaf55aa717feb1825edef521")
+        iv = bytes.fromhex("d1d7e708091941d90cdf8aa5f30bb0c2")
+    
+    if "server" in pk_name.lower():
+        key = helper.md5_str("battlecats")
+        iv = None
+        aes_mode = AES.MODE_ECB
+    if iv:
+        cipher = AES.new(key, aes_mode, iv)
+    else:
+        cipher = AES.new(key, aes_mode)
+    decrypted_data = cipher.decrypt(chunk_data)
+    return decrypted_data
+
+
+def unpack_pack(pk_file_path, ls_data, jp, base_path):
+    list_data = ls_data.decode("utf-8")
+    split_data = helper.parse_csv_file(None, list_data.split("\n"), 3)
+
+    pack_data = helper.open_file_b(pk_file_path)
+
+    with alive_bar(len(split_data)) as bar:
+        for i in range(len(split_data)):
+            file = split_data[i]
+            
+            name = file[0]
+            start_offset = int(file[1])
+            length = int(file[2])
+
+            pk_chunk = pack_data[start_offset:start_offset+length]
+            base_name = os.path.basename(pk_file_path)
+            if "imagedatalocal" in base_name.lower():
+                pk_chunk_decrypted = pk_chunk
+            else:
+                pk_chunk_decrypted = decrypt_pack(pk_chunk, jp, base_name)
+            helper.write_file_b(os.path.join(base_path, name), pk_chunk_decrypted)
+            bar()
+
+def decrypt():
+    jp = helper.coloured_text("Are you using game version &jp& 10.8 and up? (y/n):", is_input=True)
+    jp = helper.validate_bool(jp)
+    
+    pack_paths = helper.select_files("Select .pack files", [(".pack files", "*.pack")], False)
+    if not pack_paths:
+        helper.coloured_text("Please select .pack files", base=helper.red)
+        return
+    helper.check_and_create_dir(output_path)
+    
+    file_groups = find_lists(pack_paths)
+
+
+    for i in range(len(file_groups)):
+        file_group = file_groups[i]
+
+        ls_base_name = os.path.basename(file_group["list"])
+        pk_base_name = os.path.basename(file_group["pack"])
+
+        name = pk_base_name.rstrip(".pack")
+        path = os.path.join(output_path, name)
+
+        helper.check_and_create_dir(path)
+        helper.check_and_create_dir(lists_paths)
+
+        ls_data = unpack_list(file_group["list"])
+        helper.write_file_b(os.path.join(lists_paths, ls_base_name), ls_data)
+
+        helper.coloured_text(f"\n&{i+1}&\t\t{name}\t{i+1} / {len(file_groups)}", base=helper.green, new=helper.white)
+        unpack_pack(file_group["pack"], ls_data, jp, path)
+    helper.coloured_text(f"\nSuccessfully decrypted all .pack files to: &{output_path}&", base=helper.green, new=helper.white)
+def find_lists(pack_paths):
+    files = []
+    for pack_path in pack_paths:
+        directory = os.path.dirname(pack_path)
+        ls_path = os.path.join(directory, pack_path.rstrip(".pack") + ".list")
+        group = {"pack" : pack_path, "list" : ls_path}
+        files.append(group)
+    return files
```

### Comparing `battle-cats-game-modder-1.0.4/src/BCGM_Python/encrypt_decrypt/encrypt_pack.py` & `battle-cats-game-modder-1.0.5/src/BCGM_Python/encrypt_decrypt/encrypt_pack.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-from alive_progress import alive_bar
-import helper
-import os
-from libnative import write_libnative_md5
-import glob
-from Cryptodome.Cipher import AES
-
-initial_dir = "game_files"
-output_path = "encrypted_files"
-
-def create_list(game_files_dir):
-    #return open("decrypted_lists/DataLocal.list", "r").read()
-    list_of_files = glob.glob(game_files_dir + '/*')
-    files_with_size = [(file_path, os.stat(file_path).st_size) 
-                    for file_path in list_of_files ]
-    files = files_with_size
-    list_file = f"{len(files_with_size)}\n"
-    address = 0
-    for i in range(len(files_with_size)):
-        file = files_with_size[i]
-        if file[1] % 16 != 0:
-            extra = helper.add_extra_bytes(file[0], extra=True)
-            file = (file[0], file[1] + extra)
-            files[i] = file
-        
-        list_file += f"{os.path.basename(file[0])},{address},{file[1]}\n"
-        address += file[1]
-    return list_file
-
-def create_pack(game_files_dir, ls_data, jp, pk_name):
-    split_data = helper.parse_csv_file(None, ls_data.split("\n"), 3)
-    pack_data = [0] * (int(split_data[-1][1]) + int(split_data[-1][2]))
-    with alive_bar(len(split_data)) as bar:
-        for i in range(len(split_data)):
-            file = split_data[i]
-
-            name = file[0]
-            start_offset = int(file[1])
-
-            file_data = helper.open_file_b(os.path.join(game_files_dir, name))
-            if "imagedatalocal" in pk_name.lower():
-                encrypted_data = file_data
-            else:
-                encrypted_data = encrypt_file(file_data, jp, pk_name)
-            encrypted_data = list(encrypted_data)
-            pack_data = helper.insert_list(pack_data, encrypted_data, start_offset)
-            bar()
-    return pack_data
-
-def encrypt_file(file_data, jp, pk_name):
-    aes_mode = AES.MODE_CBC
-    if jp:
-        key = bytes.fromhex("d754868de89d717fa9e7b06da45ae9e3")
-        iv = bytes.fromhex("40b2131a9f388ad4e5002a98118f6128")
-    else:
-        key = bytes.fromhex("0ad39e4aeaf55aa717feb1825edef521")
-        iv = bytes.fromhex("d1d7e708091941d90cdf8aa5f30bb0c2")
-    
-    if "server" in pk_name.lower():
-        key = helper.md5_str("battlecats")
-        iv = None
-        aes_mode = AES.MODE_ECB
-    if iv:
-        cipher = AES.new(key, aes_mode, iv)
-    else:
-        cipher = AES.new(key, aes_mode)
-    encrypted_data = cipher.encrypt(file_data)
-    return encrypted_data
-
-def encrypt_list(list_data):
-    key = helper.md5_str("pack")
-    cipher = AES.new(key, AES.MODE_ECB)
-    encrypted_data = cipher.encrypt(list_data)
-    return encrypted_data
-def encrypt():
-    jp = helper.coloured_text("Are you using game version &jp& 10.8 and up? (y/n):", is_input=True)
-    jp = helper.validate_bool(jp)
-
-    name = input("Enter the name of the file to be outputed e.g DataLocal, ImageDataLocal etc:")
-    
-    game_files_dir = helper.select_dir("Select a folder of game files", initial_dir)
-    if not game_files_dir:
-        helper.coloured_text("Please select a folder of game files", base=helper.red)
-        return
-    
-    helper.check_and_create_dir(output_path)
-    list_data = create_list(game_files_dir)
-    list_data_full = helper.add_extra_bytes(None, False, list_data.encode("utf-8"))
-
-    encrypted_data_list = encrypt_list(list_data_full)
-    ls_output = os.path.join(output_path, name + ".list")
-    helper.write_file_b(ls_output, encrypted_data_list)
-    
-    pack_data = create_pack(game_files_dir, list_data, jp, name)
-    pk_output = os.path.join(output_path, name + ".pack")
-    helper.write_file_b(pk_output, bytes(pack_data))
-    print(f"Successfully created .pack and .list files to: {output_path}")
-
-    lib = helper.validate_bool(input("Do you want to patch your libnative-lib.so file now?(y/n):"))
-    if lib:
-        write_libnative_md5.write_libnative([ls_output, pk_output])
-
+from alive_progress import alive_bar
+import helper
+import os
+from libnative import write_libnative_md5
+import glob
+from Cryptodome.Cipher import AES
+
+initial_dir = "game_files"
+output_path = "encrypted_files"
+
+def create_list(game_files_dir):
+    #return open("decrypted_lists/DataLocal.list", "r").read()
+    list_of_files = glob.glob(game_files_dir + '/*')
+    files_with_size = [(file_path, os.stat(file_path).st_size) 
+                    for file_path in list_of_files ]
+    files = files_with_size
+    list_file = f"{len(files_with_size)}\n"
+    address = 0
+    for i in range(len(files_with_size)):
+        file = files_with_size[i]
+        if file[1] % 16 != 0:
+            extra = helper.add_extra_bytes(file[0], extra=True)
+            file = (file[0], file[1] + extra)
+            files[i] = file
+        
+        list_file += f"{os.path.basename(file[0])},{address},{file[1]}\n"
+        address += file[1]
+    return list_file
+
+def create_pack(game_files_dir, ls_data, jp, pk_name):
+    split_data = helper.parse_csv_file(None, ls_data.split("\n"), 3)
+    pack_data = [0] * (int(split_data[-1][1]) + int(split_data[-1][2]))
+    with alive_bar(len(split_data)) as bar:
+        for i in range(len(split_data)):
+            file = split_data[i]
+
+            name = file[0]
+            start_offset = int(file[1])
+
+            file_data = helper.open_file_b(os.path.join(game_files_dir, name))
+            if "imagedatalocal" in pk_name.lower():
+                encrypted_data = file_data
+            else:
+                encrypted_data = encrypt_file(file_data, jp, pk_name)
+            encrypted_data = list(encrypted_data)
+            pack_data = helper.insert_list(pack_data, encrypted_data, start_offset)
+            bar()
+    return pack_data
+
+def encrypt_file(file_data, jp, pk_name):
+    aes_mode = AES.MODE_CBC
+    if jp:
+        key = bytes.fromhex("d754868de89d717fa9e7b06da45ae9e3")
+        iv = bytes.fromhex("40b2131a9f388ad4e5002a98118f6128")
+    else:
+        key = bytes.fromhex("0ad39e4aeaf55aa717feb1825edef521")
+        iv = bytes.fromhex("d1d7e708091941d90cdf8aa5f30bb0c2")
+    
+    if "server" in pk_name.lower():
+        key = helper.md5_str("battlecats")
+        iv = None
+        aes_mode = AES.MODE_ECB
+    if iv:
+        cipher = AES.new(key, aes_mode, iv)
+    else:
+        cipher = AES.new(key, aes_mode)
+    encrypted_data = cipher.encrypt(file_data)
+    return encrypted_data
+
+def encrypt_list(list_data):
+    key = helper.md5_str("pack")
+    cipher = AES.new(key, AES.MODE_ECB)
+    encrypted_data = cipher.encrypt(list_data)
+    return encrypted_data
+def encrypt():
+    jp = helper.coloured_text("Are you using game version &jp& 10.8 and up? (y/n):", is_input=True)
+    jp = helper.validate_bool(jp)
+
+    name = input("Enter the name of the file to be outputed e.g DataLocal, ImageDataLocal etc:")
+    
+    game_files_dir = helper.select_dir("Select a folder of game files", initial_dir)
+    if not game_files_dir:
+        helper.coloured_text("Please select a folder of game files", base=helper.red)
+        return
+    
+    helper.check_and_create_dir(output_path)
+    list_data = create_list(game_files_dir)
+    list_data_full = helper.add_extra_bytes(None, False, list_data.encode("utf-8"))
+
+    encrypted_data_list = encrypt_list(list_data_full)
+    ls_output = os.path.join(output_path, name + ".list")
+    helper.write_file_b(ls_output, encrypted_data_list)
+    
+    pack_data = create_pack(game_files_dir, list_data, jp, name)
+    pk_output = os.path.join(output_path, name + ".pack")
+    helper.write_file_b(pk_output, bytes(pack_data))
+    print(f"Successfully created .pack and .list files to: {output_path}")
+
+    lib = helper.validate_bool(input("Do you want to patch your libnative-lib.so file now?(y/n):"))
+    if lib:
+        write_libnative_md5.write_libnative([ls_output, pk_output])
+
```

### Comparing `battle-cats-game-modder-1.0.4/src/BCGM_Python/feature_handler.py` & `battle-cats-game-modder-1.0.5/src/BCGM_Python/feature_handler.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-import BCGM_Python.helper as helper
-from encrypt_decrypt import decrypt_pack, encrypt_pack
-from libnative import write_libnative_md5
-from file_mods import unit_mod, enemy_mod, stage_mod
-features = {
-    "Pack File Encrypting / Decrypting" : {
-        "Decrypt .pack files" : decrypt_pack.decrypt,
-        "Encrypt game files to .pack file" : encrypt_pack.encrypt
-    },
-    "Set md5 hashes in libnative-lib.so file" : write_libnative_md5.write_libnative,
-    "Game File Modding" : {
-        "Edit unit*.csv files (cat stats)" : unit_mod.edit_unit,
-        "Edit t_unit.csv file (enemy stats)" : enemy_mod.edit_enemy,
-        "Edit stage*.csv files (stage data)" : stage_mod.edit_stage,
-    },
-}
-def display_features():
-    helper.create_list(list(features))
-
-def search_dict(dictionary, item, results=[]):
-    for k, v in dictionary.items():
-        if type(v) == dict:
-            search_dict(v, item, results)
-        else:
-            if item.lower() in k.lower().replace(" ", ""):
-                results.append({"Name": k, "Function": v})
-    return results
-
-def show_options(user_input, feature_dict):
-    result_input = helper.validate_int(user_input)
-    to_search = user_input
-
-    if result_input != None:
-        if result_input > len(list(feature_dict)):
-            print(f"Please enter a number between 1 and {len(list(feature_dict))}")
-            return
-        name = list(feature_dict)[result_input-1]
-        result_data = feature_dict[name]
-        results = []
-        if type(result_data) != dict:
-            return result_data()
-        for result in result_data:
-            results.append(
-                {"Name": result, "Function": feature_dict[name][result]})
-    else:
-        to_search = to_search.replace(" ", "")
-        results = search_dict(feature_dict, to_search, [])
-    if len(results) == 1:
-        return results[0]["Function"]()
-    else:
-        options = []
-        for i in range(len(results)):
-            options.append(results[i]["Name"])
-        if not options:
-            print(f"Error a feature with name: {user_input} doesn't exist")
-            return
-        helper.create_list(options)
-        user_input = input("Enter an option:\n")
-        index = helper.validate_int(user_input)
-        if index != None:
-            if index > len(results):
-                print(f"Please enter a number between 1 and {len(results)}")
-                return
-            if type(results[index-1]["Function"]) == dict:
-                return show_options(user_input, feature_dict[name])
-            return results[index-1]["Function"]()
-def menu():
-    display_features()
-    user_input = input(
-        "What do you want to do (some options contain other features within them)\nYou can enter a number to run a feature or a word to search for that feature (e.g entering decrypt will run the Decrypt .pack files feature, and entering csv will show you all the features that edit csv files)\nYou can press enter to see all of the features:\n")
+import BCGM_Python.helper as helper
+from encrypt_decrypt import decrypt_pack, encrypt_pack
+from libnative import write_libnative_md5
+from file_mods import unit_mod, enemy_mod, stage_mod
+features = {
+    "Pack File Encrypting / Decrypting" : {
+        "Decrypt .pack files" : decrypt_pack.decrypt,
+        "Encrypt game files to .pack file" : encrypt_pack.encrypt
+    },
+    "Set md5 hashes in libnative-lib.so file" : write_libnative_md5.write_libnative,
+    "Game File Modding" : {
+        "Edit unit*.csv files (cat stats)" : unit_mod.edit_unit,
+        "Edit t_unit.csv file (enemy stats)" : enemy_mod.edit_enemy,
+        "Edit stage*.csv files (stage data)" : stage_mod.edit_stage,
+    },
+}
+def display_features():
+    helper.create_list(list(features))
+
+def search_dict(dictionary, item, results=[]):
+    for k, v in dictionary.items():
+        if type(v) == dict:
+            search_dict(v, item, results)
+        else:
+            if item.lower() in k.lower().replace(" ", ""):
+                results.append({"Name": k, "Function": v})
+    return results
+
+def show_options(user_input, feature_dict):
+    result_input = helper.validate_int(user_input)
+    to_search = user_input
+
+    if result_input != None:
+        if result_input > len(list(feature_dict)):
+            print(f"Please enter a number between 1 and {len(list(feature_dict))}")
+            return
+        name = list(feature_dict)[result_input-1]
+        result_data = feature_dict[name]
+        results = []
+        if type(result_data) != dict:
+            return result_data()
+        for result in result_data:
+            results.append(
+                {"Name": result, "Function": feature_dict[name][result]})
+    else:
+        to_search = to_search.replace(" ", "")
+        results = search_dict(feature_dict, to_search, [])
+    if len(results) == 1:
+        return results[0]["Function"]()
+    else:
+        options = []
+        for i in range(len(results)):
+            options.append(results[i]["Name"])
+        if not options:
+            print(f"Error a feature with name: {user_input} doesn't exist")
+            return
+        helper.create_list(options)
+        user_input = input("Enter an option:\n")
+        index = helper.validate_int(user_input)
+        if index != None:
+            if index > len(results):
+                print(f"Please enter a number between 1 and {len(results)}")
+                return
+            if type(results[index-1]["Function"]) == dict:
+                return show_options(user_input, feature_dict[name])
+            return results[index-1]["Function"]()
+def menu():
+    display_features()
+    user_input = input(
+        "What do you want to do (some options contain other features within them)\nYou can enter a number to run a feature or a word to search for that feature (e.g entering decrypt will run the Decrypt .pack files feature, and entering csv will show you all the features that edit csv files)\nYou can press enter to see all of the features:\n")
     show_options(user_input, features)
```

### Comparing `battle-cats-game-modder-1.0.4/src/BCGM_Python/file_mods/enemy_mod.py` & `battle-cats-game-modder-1.0.5/src/BCGM_Python/file_mods/enemy_mod.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-import helper
-from file_mods import unit_mod
-
-values = [
-    "HP", "Knockback amount", "Movement Speed", "Attack Power", "Time between attacks", "Attack range", "Money Drop",
-    "?", "Width", "?", "Red flag", "Area attack flag", "Foreswing", "Floating flag", "Black flag", "Metal Flag", "Traitless Flag",
-    "Angel Flag", "Alien Flag", "Zombie Flag", "Knock back chance", "Freeze chance", "Freeze duration", "Slow Chance",
-    "Slow Duration", "Crit Chance", "Base Destroyer Flag", "Wave Chance", "Wave Level", "Weaken Chance", "Weaken Duration",
-    "Weaken %", "Strengthen Activation health", "Strengthen Multiplier", "Survive Lethal Chance", "Long distance start", "Long distance range",
-    "Wave Immunity", "?", "Knockback immunity", "Freeze immunity", "Slow immunity", "Weaken immunity", "Burrow count",
-    "Burrow distance", "Revive count", "Revive time", "Percentage of health after revive", "Witch Flag", "Is enemy base flag", "loop?",
-    "?", "Self-Destruct Flag (2=self-destruct)", "?", "Soul when dead", "Second attack damage", "Third attack damage", "Second attack start frame",
-    "Third attack start frame", "Use ability on first hit flag", "Second attack flag", "Third attack flag", "?",
-    "Some flag for gudetama", "Barrier HP", "Warp Chance", "Warp Duration", "Warp min range", "Warp max range",
-    "Starred Alien Flag (2-4 = god)", "Some flag for doge sun and the winds", "Eva angel flag", "Relic flag", "Curse Chance",
-    "Cuse Duration", "Savage Blow Chance", "Savage Blow Multiplier", "Invincibility Chance", "Invincibility Duration",
-    "Toxic Chance", "Toxic Percentage health", "Surge Chance", "Surge Min range", "Surge max range", "Surge Level",
-    "Some flag for doge sun, wind enemies and doron", "Mini wave toggle", "Shield HP", "Percentage HP healed when knockbacked",
-    "Surge Chance when killed", "Surge min range when killed", "Surge max range when killed", "Surge Level when killed",
-    "Aku flag", "Baron Trait Flag"
-]
-
-
-def edit_enemy():
-    csv_path = helper.select_files("Select t_unit.csv file", [(
-        "Enemy stats", "t_unit.csv")], default=unit_mod.get_initial_dir())
-    if not csv_path:
-        print("Please select an enemy data file")
-        return
-    csv_file_data = helper.parse_csv_file(
-        csv_path, min_length=3, black_list=["//", "\n"])
-
-    ids = helper.get_range_input(helper.coloured_text(
-        "Enter enemy ids (Look up enemy release order battle cats to find ids)(You can enter &all& to get all, a range e.g &1&-&50&, or ids separate by spaces e.g &5 4 7&):", is_input=True), len(csv_file_data))
-
-    for id in ids:
-        enemy_data = csv_file_data[id]
-
-        helper.coloured_text(f"Enemy unit &{id}& is selected")
-        enemy_data = helper.edit_array_user(
-            values, enemy_data, "Stats", "value", extra_values=enemy_data)
-        csv_file_data[id] = enemy_data
-
-    helper.write_csv_file(csv_path, csv_file_data)
-    print("Successfully edited csv file")
+import helper
+from file_mods import unit_mod
+
+values = [
+    "HP", "Knockback amount", "Movement Speed", "Attack Power", "Time between attacks", "Attack range", "Money Drop",
+    "?", "Width", "?", "Red flag", "Area attack flag", "Foreswing", "Floating flag", "Black flag", "Metal Flag", "Traitless Flag",
+    "Angel Flag", "Alien Flag", "Zombie Flag", "Knock back chance", "Freeze chance", "Freeze duration", "Slow Chance",
+    "Slow Duration", "Crit Chance", "Base Destroyer Flag", "Wave Chance", "Wave Level", "Weaken Chance", "Weaken Duration",
+    "Weaken %", "Strengthen Activation health", "Strengthen Multiplier", "Survive Lethal Chance", "Long distance start", "Long distance range",
+    "Wave Immunity", "?", "Knockback immunity", "Freeze immunity", "Slow immunity", "Weaken immunity", "Burrow count",
+    "Burrow distance", "Revive count", "Revive time", "Percentage of health after revive", "Witch Flag", "Is enemy base flag", "loop?",
+    "?", "Self-Destruct Flag (2=self-destruct)", "?", "Soul when dead", "Second attack damage", "Third attack damage", "Second attack start frame",
+    "Third attack start frame", "Use ability on first hit flag", "Second attack flag", "Third attack flag", "?",
+    "Some flag for gudetama", "Barrier HP", "Warp Chance", "Warp Duration", "Warp min range", "Warp max range",
+    "Starred Alien Flag (2-4 = god)", "Some flag for doge sun and the winds", "Eva angel flag", "Relic flag", "Curse Chance",
+    "Cuse Duration", "Savage Blow Chance", "Savage Blow Multiplier", "Invincibility Chance", "Invincibility Duration",
+    "Toxic Chance", "Toxic Percentage health", "Surge Chance", "Surge Min range", "Surge max range", "Surge Level",
+    "Some flag for doge sun, wind enemies and doron", "Mini wave toggle", "Shield HP", "Percentage HP healed when knockbacked",
+    "Surge Chance when killed", "Surge min range when killed", "Surge max range when killed", "Surge Level when killed",
+    "Aku flag", "Baron Trait Flag"
+]
+
+
+def edit_enemy():
+    csv_path = helper.select_files("Select t_unit.csv file", [(
+        "Enemy stats", "t_unit.csv")], default=unit_mod.get_initial_dir())
+    if not csv_path:
+        print("Please select an enemy data file")
+        return
+    csv_file_data = helper.parse_csv_file(
+        csv_path, min_length=3, black_list=["//", "\n"])
+
+    ids = helper.get_range_input(helper.coloured_text(
+        "Enter enemy ids (Look up enemy release order battle cats to find ids)(You can enter &all& to get all, a range e.g &1&-&50&, or ids separate by spaces e.g &5 4 7&):", is_input=True), len(csv_file_data))
+
+    for id in ids:
+        enemy_data = csv_file_data[id]
+
+        helper.coloured_text(f"Enemy unit &{id}& is selected")
+        enemy_data = helper.edit_array_user(
+            values, enemy_data, "Stats", "value", extra_values=enemy_data)
+        csv_file_data[id] = enemy_data
+
+    helper.write_csv_file(csv_path, csv_file_data)
+    print("Successfully edited csv file")
```

### Comparing `battle-cats-game-modder-1.0.4/src/BCGM_Python/file_mods/stage_mod.py` & `battle-cats-game-modder-1.0.5/src/BCGM_Python/file_mods/stage_mod.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-import os
-import helper
-from file_mods import unit_mod
-
-stage_infos = [
-    "Stage Width",
-    "Base health",
-    "Minimum spawn frame",
-    "Maximum spawn frame",
-    "Background type",
-    "Maximum enemies",
-]
-
-enemy_infos = [
-    "Enemy ID",
-    "Amount to spawn in total",
-    "First spawn frame",
-    "Time between spawns in frames min",
-    "Time between spawns in frames max",
-    "Spawn when base health has reached %",
-    "Front z-layer",
-    "Back z-layer",
-    "Boss flag",
-    "Strength multiplier",
-]
-
-
-def edit_stage():
-    df_path = os.path.abspath(unit_mod.get_initial_dir())
-    csv_path = helper.select_files("Select *stage.csv files", [("stage data files", "stage*.csv")], default=df_path)
-    if not csv_path:
-        print("Please select a stage data file")
-        return
-
-    csv_file_data = helper.parse_csv_file(
-        csv_path, min_length=3, black_list=["//", "\n"])
-
-    stage_id = None
-
-    if len(csv_file_data[0]) < 9:
-        stage_id = helper.ls_to_str(csv_file_data[0])
-        csv_file_data = csv_file_data[1:]
-
-    csv_file_data[-1] = csv_file_data[-1][:-1]
-
-    stage_data = helper.int_ls_to_str_ls(csv_file_data[0])
-    enemy_slot_data = []
-
-    for i in range(1, len(csv_file_data)):
-        enemy_data = helper.int_ls_to_str_ls(csv_file_data[i])
-        enemy_slot_data.append(enemy_data)
-
-    options = ["Edit basic stage data", "Edit enemy slots"]
-    if stage_id != None:
-        options.append("Edit stage id")
-    helper.create_list(options)
-    option = helper.validate_int(input("What do you want to do?:"))
-    if option == None:
-        print("Please enter a valid number")
-        return
-    if option == 1:
-        stage_data = helper.edit_array_user(
-            stage_infos, stage_data, "Basic Stage Stats", "value", extra_values=stage_data, all_at_once=False)
-    elif option == 2:
-        enemy_ids = []
-        for i in range(len(enemy_slot_data)):
-            slot = enemy_slot_data[i]
-            if slot[0] != 0:
-                enemy_ids.append(f"Enemy id {slot[0]}")
-
-        helper.coloured_text(
-            "Enter an enemy slot id (to add new slots just enter a number larger than the highest displayed slot id):")
-        ids = helper.selection_list(enemy_ids, "edit", all_at_once=False)
-        for id in ids:
-            id = helper.validate_int(id)
-            if id == None:
-                print("Please enter a valid number")
-                return
-            if id > len(enemy_slot_data):
-                enemy_slot_data.append([0, 0, 0, 0, 0, 0, 0, 9, 0, 100])
-                id = len(enemy_slot_data)
-            id -= 1
-            enemy_infos_trimmed = enemy_infos
-            if len(enemy_slot_data[id]) < len(enemy_infos):
-                enemy_infos_trimmed = enemy_infos[:-1]
-            helper.coloured_text(f"Slot: &{id+1}& is currently selected")
-            enemy_slot_data[id] = helper.edit_array_user(
-                enemy_infos_trimmed, enemy_slot_data[id], "Enemy Slots", "value", extra_values=enemy_slot_data[id])
-    elif option == 3 and stage_id != None:
-        stage_id = helper.coloured_text(
-            f"Current stage id: &{stage_id}&\nWhat do you want to set the stage id to?:", is_input=True)
-
-    new_csv_data = []
-
-    if stage_id != None:
-        new_csv_data.append(helper.str_to_ls(stage_id))
-    new_csv_data.append(stage_data)
-    new_csv_data += enemy_slot_data
-
-    helper.write_csv_file(csv_path, new_csv_data)
-    print("Successfully modified csv file")
+import os
+import helper
+from file_mods import unit_mod
+
+stage_infos = [
+    "Stage Width",
+    "Base health",
+    "Minimum spawn frame",
+    "Maximum spawn frame",
+    "Background type",
+    "Maximum enemies",
+]
+
+enemy_infos = [
+    "Enemy ID",
+    "Amount to spawn in total",
+    "First spawn frame",
+    "Time between spawns in frames min",
+    "Time between spawns in frames max",
+    "Spawn when base health has reached %",
+    "Front z-layer",
+    "Back z-layer",
+    "Boss flag",
+    "Strength multiplier",
+]
+
+
+def edit_stage():
+    df_path = os.path.abspath(unit_mod.get_initial_dir())
+    csv_path = helper.select_files("Select *stage.csv files", [("stage data files", "stage*.csv")], default=df_path)
+    if not csv_path:
+        print("Please select a stage data file")
+        return
+
+    csv_file_data = helper.parse_csv_file(
+        csv_path, min_length=3, black_list=["//", "\n"])
+
+    stage_id = None
+
+    if len(csv_file_data[0]) < 9:
+        stage_id = helper.ls_to_str(csv_file_data[0])
+        csv_file_data = csv_file_data[1:]
+
+    csv_file_data[-1] = csv_file_data[-1][:-1]
+
+    stage_data = helper.int_ls_to_str_ls(csv_file_data[0])
+    enemy_slot_data = []
+
+    for i in range(1, len(csv_file_data)):
+        enemy_data = helper.int_ls_to_str_ls(csv_file_data[i])
+        enemy_slot_data.append(enemy_data)
+
+    options = ["Edit basic stage data", "Edit enemy slots"]
+    if stage_id != None:
+        options.append("Edit stage id")
+    helper.create_list(options)
+    option = helper.validate_int(input("What do you want to do?:"))
+    if option == None:
+        print("Please enter a valid number")
+        return
+    if option == 1:
+        stage_data = helper.edit_array_user(
+            stage_infos, stage_data, "Basic Stage Stats", "value", extra_values=stage_data, all_at_once=False)
+    elif option == 2:
+        enemy_ids = []
+        for i in range(len(enemy_slot_data)):
+            slot = enemy_slot_data[i]
+            if slot[0] != 0:
+                enemy_ids.append(f"Enemy id {slot[0]}")
+
+        helper.coloured_text(
+            "Enter an enemy slot id (to add new slots just enter a number larger than the highest displayed slot id):")
+        ids = helper.selection_list(enemy_ids, "edit", all_at_once=False)
+        for id in ids:
+            id = helper.validate_int(id)
+            if id == None:
+                print("Please enter a valid number")
+                return
+            if id > len(enemy_slot_data):
+                enemy_slot_data.append([0, 0, 0, 0, 0, 0, 0, 9, 0, 100])
+                id = len(enemy_slot_data)
+            id -= 1
+            enemy_infos_trimmed = enemy_infos
+            if len(enemy_slot_data[id]) < len(enemy_infos):
+                enemy_infos_trimmed = enemy_infos[:-1]
+            helper.coloured_text(f"Slot: &{id+1}& is currently selected")
+            enemy_slot_data[id] = helper.edit_array_user(
+                enemy_infos_trimmed, enemy_slot_data[id], "Enemy Slots", "value", extra_values=enemy_slot_data[id])
+    elif option == 3 and stage_id != None:
+        stage_id = helper.coloured_text(
+            f"Current stage id: &{stage_id}&\nWhat do you want to set the stage id to?:", is_input=True)
+
+    new_csv_data = []
+
+    if stage_id != None:
+        new_csv_data.append(helper.str_to_ls(stage_id))
+    new_csv_data.append(stage_data)
+    new_csv_data += enemy_slot_data
+
+    helper.write_csv_file(csv_path, new_csv_data)
+    print("Successfully modified csv file")
```

### Comparing `battle-cats-game-modder-1.0.4/src/BCGM_Python/file_mods/unit_mod.py` & `battle-cats-game-modder-1.0.5/src/BCGM_Python/file_mods/unit_mod.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-import helper
-from encrypt_decrypt import decrypt_pack
-import os
-
-
-def get_initial_dir():
-    test_path = os.path.join(decrypt_pack.output_path, "DataLocal")
-    if os.path.exists(test_path):
-        return test_path
-    else:
-        return decrypt_pack.output_path
-
-
-values = [
-    "HP", "Knockback amount", "Movement Speed", "Attack Power", "Time between attacks", "Attack Range", "Base cost", "Recharge time",
-    "Hit box position", "Hit box size", "Red effective flag", "Always zero", "Area attack flag", "Attack animation", "Min z layer",
-    "Max z layer", "Floating effective flag", "Black effective flag", "Metal effective flag", "White effective flag", "Angel effective flag", "Alien effective flag",
-    "Zombie effective flag", "Strong against flag", "Knockback chance", "Freeze chance", "Freeze duration", "Slow chance", "Slow duration",
-    "Resistant flag", "Triple damage flag", "Critical chance", "Attack only flag", "Extra money from enemies flag", "Base destroyer flag", "Wave chance",
-    "Wave attack level", "Weaken chance", "Weaken duration", "Weaken to (decrease attack to percentage left)", "HP remain strength",
-    "Boost strength multiplier", "Survive chance", "If unit is metal flag", "Long range start", "Long range append", "Immune to wave flag", "Block wave flag",
-    "Resist knockbacks flag", "Resist freeze flag", "Resist slow flag", "Resist weaken flag", "Zombie killer flag", "Witch killer flag", "Witch effective flag", "Not effected by boss wave flag",
-    "Frames before automatically dying -1 to never die automatically", "Always -1", "Death after attack flag", "Second attack power", "Third attack power", "Second attack animation", "Third attack animation", "Use ability on first hit flag",
-    "Second attack flag", "Third attack flag", "Spawn animation, -1, 0", "Soul animation -1, 0, 1, 2, 3, 5, 6, 7", "Unike spawn animation", "Gudetama soul animation",
-    "Barrier break chance", "Warp Chance", "Warp Duration", "Min warp distance", "Max warp Distance", "Warp blocker flag", "Eva Angel Effective",
-    "Eva angel killer flag", "Relic effective flag", "Immune to curse flag", "Insanely tough flag", "Insane damage flag", "Savage blow chance", "Savage blow level", "Dodge attack chance",
-    "Dodge attack duration", "Surge attack chance", "Surge attack min range", "Surge attack max range", "Surge attack level", "Toxic immunity flag", "Surge immunity flag", "Curse chance", "Curse duration", "Unkown", "Aku shield break chance",
-    "Aku effective flag", "Colossus Slayer"
-]
-
-
-def edit_unit():
-    csv_path = helper.select_files(
-        "Select a unit*.csv file", [("Unit csv files", "unit*.csv")], default=get_initial_dir())
-    if not csv_path:
-        print("Please select a unit data file")
-        return
-    csv_file_data = helper.parse_csv_file(
-        csv_path, min_length=3, black_list=["//", "\n"])
-
-    forms = ["First Form", "Second Form", "Third Form"]
-
-    choices = helper.selection_list(forms, "edit")
-    for choice in choices:
-
-        form_id = helper.validate_int(choice)
-
-        if not form_id or form_id > len(forms):
-            print("Please enter a valid number")
-            continue
-        form_id -= 1
-        form_data = csv_file_data[form_id]
-        form_data = extend_length(form_data, values)
-
-        helper.coloured_text(f"The cat's &{forms[form_id]}& is selected")
-        form_data = helper.edit_array_user(
-            values, form_data, "Stats", "value", extra_values=form_data)
-
-        csv_file_data[form_id] = form_data
-
-    helper.write_csv_file(csv_path, csv_file_data)
-    print("Successfully edited csv file")
-
-
-def extend_length(short_ls, long_ls):
-    extra = len(long_ls) - len(short_ls)
-    if extra > 0:
-        short_ls += ([0] * extra)
-        # values that are required so that the unit works properly
-        short_ls[55] = -1
-        short_ls[57] = -1
-        short_ls[63] = 1
-        short_ls[66] = -1
-    return short_ls
+import helper
+from encrypt_decrypt import decrypt_pack
+import os
+
+
+def get_initial_dir():
+    test_path = os.path.join(decrypt_pack.output_path, "DataLocal")
+    if os.path.exists(test_path):
+        return test_path
+    else:
+        return decrypt_pack.output_path
+
+
+values = [
+    "HP", "Knockback amount", "Movement Speed", "Attack Power", "Time between attacks", "Attack Range", "Base cost", "Recharge time",
+    "Hit box position", "Hit box size", "Red effective flag", "Always zero", "Area attack flag", "Attack animation", "Min z layer",
+    "Max z layer", "Floating effective flag", "Black effective flag", "Metal effective flag", "White effective flag", "Angel effective flag", "Alien effective flag",
+    "Zombie effective flag", "Strong against flag", "Knockback chance", "Freeze chance", "Freeze duration", "Slow chance", "Slow duration",
+    "Resistant flag", "Triple damage flag", "Critical chance", "Attack only flag", "Extra money from enemies flag", "Base destroyer flag", "Wave chance",
+    "Wave attack level", "Weaken chance", "Weaken duration", "Weaken to (decrease attack to percentage left)", "HP remain strength",
+    "Boost strength multiplier", "Survive chance", "If unit is metal flag", "Long range start", "Long range append", "Immune to wave flag", "Block wave flag",
+    "Resist knockbacks flag", "Resist freeze flag", "Resist slow flag", "Resist weaken flag", "Zombie killer flag", "Witch killer flag", "Witch effective flag", "Not effected by boss wave flag",
+    "Frames before automatically dying -1 to never die automatically", "Always -1", "Death after attack flag", "Second attack power", "Third attack power", "Second attack animation", "Third attack animation", "Use ability on first hit flag",
+    "Second attack flag", "Third attack flag", "Spawn animation, -1, 0", "Soul animation -1, 0, 1, 2, 3, 5, 6, 7", "Unike spawn animation", "Gudetama soul animation",
+    "Barrier break chance", "Warp Chance", "Warp Duration", "Min warp distance", "Max warp Distance", "Warp blocker flag", "Eva Angel Effective",
+    "Eva angel killer flag", "Relic effective flag", "Immune to curse flag", "Insanely tough flag", "Insane damage flag", "Savage blow chance", "Savage blow level", "Dodge attack chance",
+    "Dodge attack duration", "Surge attack chance", "Surge attack min range", "Surge attack max range", "Surge attack level", "Toxic immunity flag", "Surge immunity flag", "Curse chance", "Curse duration", "Unkown", "Aku shield break chance",
+    "Aku effective flag", "Colossus Slayer"
+]
+
+
+def edit_unit():
+    csv_path = helper.select_files(
+        "Select a unit*.csv file", [("Unit csv files", "unit*.csv")], default=get_initial_dir())
+    if not csv_path:
+        print("Please select a unit data file")
+        return
+    csv_file_data = helper.parse_csv_file(
+        csv_path, min_length=3, black_list=["//", "\n"])
+
+    forms = ["First Form", "Second Form", "Third Form"]
+
+    choices = helper.selection_list(forms, "edit")
+    for choice in choices:
+
+        form_id = helper.validate_int(choice)
+
+        if not form_id or form_id > len(forms):
+            print("Please enter a valid number")
+            continue
+        form_id -= 1
+        form_data = csv_file_data[form_id]
+        form_data = extend_length(form_data, values)
+
+        helper.coloured_text(f"The cat's &{forms[form_id]}& is selected")
+        form_data = helper.edit_array_user(
+            values, form_data, "Stats", "value", extra_values=form_data)
+
+        csv_file_data[form_id] = form_data
+
+    helper.write_csv_file(csv_path, csv_file_data)
+    print("Successfully edited csv file")
+
+
+def extend_length(short_ls, long_ls):
+    extra = len(long_ls) - len(short_ls)
+    if extra > 0:
+        short_ls += ([0] * extra)
+        # values that are required so that the unit works properly
+        short_ls[55] = -1
+        short_ls[57] = -1
+        short_ls[63] = 1
+        short_ls[66] = -1
+    return short_ls
```

### Comparing `battle-cats-game-modder-1.0.4/src/BCGM_Python/helper.py` & `battle-cats-game-modder-1.0.5/src/BCGM_Python/helper.py`

 * *Files identical despite different names*

### Comparing `battle-cats-game-modder-1.0.4/src/BCGM_Python/libnative/find_order.py` & `battle-cats-game-modder-1.0.5/src/BCGM_Python/libnative/find_order.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-import json
-import math
-
-def search_pos(path):
-    f = open(path, "rb").read()
-    index = f.find(b"DataLocal.list")
-    index_2 = f.find(b"ImageDataLocal.list")
-    if index == -1:
-        print("Error, position couldn't be found")
-        return
-    if index_2 < index:
-        index = index_2
-    start_index = index
-    end_index = index
-    temp_index = index
-
-    limit = 1000
-
-    for i in range(limit):
-        index = f.find(b".pack", index+5)
-        if index == -1:
-            end_index = temp_index + 5
-            break
-        temp_index = index
-    
-    valid_bytes = [b"\x00", b"0", b"1", b"2", b"3", b"4", b"5", b"6", b"7", b"8", b"9", b"a", b"b", b"c", b"d", b"e", b"f"]
-    index = end_index
-    position = index
-    for i in range(limit*33):
-        position = index + i
-        byte = bytes([f[position]])
-
-        if byte not in valid_bytes:
-            break
-
-    file_names = readcstrs(start_index, end_index, f)
-    hashes = readcstrs(end_index+1, position, f)
-    file_names = filter_names(file_names)
-    if "DataLocal.pack" not in file_names:
-        file_names.insert(0, "DataLocal.list")
-        file_names.insert(1, "DataLocal.pack")
-    return {"names" : file_names, "hashes" : hashes}
-
-def filter_names(names):
-    duplicates = ["NumberLocal", "UnitLocal"]
-
-    new_ls = names.copy()
-    for name in names:
-        name_split = name.split("_")
-        if len(name_split) == 2:
-            if name_split[0] in duplicates:
-                new_ls.remove(name)
-    return new_ls
-
-
-def readcstrs(start_address, end_address, data):
-    str = ""
-    strings = []
-    for i in range(start_address, end_address):
-        item = bytes([data[i]])
-
-        if item == b"\x00":
-            strings.append(str)
-            str = ""
-        else:
-            str += item.decode("utf-8")
-    return strings
-
-def generate_order(names, hashes, base_hash, base_name, skip=5, length=4):
-    data = {}
-    for i in range(length):
-        name_index = base_name + i*14
-        hash_index = base_hash + i*7
-
-        for j in range(6, -1, -1):
-            if i == length-1 and j < skip: break
-            name = names[name_index-(j*2)]
-            hash = hashes[hash_index-j]
-
-            data[name] = hash
-    return data
-
-def format(dict):
-    return json.dumps(dict, indent=4)
-
-def find_server_versions(names):
-    for name in names:
-        if "Server" in name:
-            return names.index(name)
-    return -1
-
-def get_length(length):
-    total_loops = math.ceil(length / 7)
-    skip = (total_loops*7) - length
-    return {"length" : total_loops, "skip" : skip}
-
-def server_lists_lengths(names):
-    version = ""
-    counter = 0
-    for name in names:
-        if "Server" in name and ".list" in name:
-            data = name.split("_")
-            if len(data) == 4:
-                if not version:
-                    version = name.split("_")[3][:2]
-                if version and version == name.split("_")[3][:2]:
-                    counter += 1
-            else:
-                counter += 1
-    
-    return get_length(counter)
-
-def find_order(path):
-    data = search_pos(path)
-    if not data:
-        return
-    names = data["names"]
-    hashes = data["hashes"]
-
-    hash_table = {}
-    hash_table.update(generate_order(names, hashes, 6, 12))
-    hash_table.update(generate_order(names, hashes, 33, 13))
-
-    server_version_index = find_server_versions(names)
-    lengths = server_lists_lengths(names)
-    hash_table.update(generate_order(names, hashes, server_version_index+6, server_version_index+12, lengths["skip"], lengths["length"]))
-
+import json
+import math
+
+def search_pos(path):
+    f = open(path, "rb").read()
+    index = f.find(b"DataLocal.list")
+    index_2 = f.find(b"ImageDataLocal.list")
+    if index == -1:
+        print("Error, position couldn't be found")
+        return
+    if index_2 < index:
+        index = index_2
+    start_index = index
+    end_index = index
+    temp_index = index
+
+    limit = 1000
+
+    for i in range(limit):
+        index = f.find(b".pack", index+5)
+        if index == -1:
+            end_index = temp_index + 5
+            break
+        temp_index = index
+    
+    valid_bytes = [b"\x00", b"0", b"1", b"2", b"3", b"4", b"5", b"6", b"7", b"8", b"9", b"a", b"b", b"c", b"d", b"e", b"f"]
+    index = end_index
+    position = index
+    for i in range(limit*33):
+        position = index + i
+        byte = bytes([f[position]])
+
+        if byte not in valid_bytes:
+            break
+
+    file_names = readcstrs(start_index, end_index, f)
+    hashes = readcstrs(end_index+1, position, f)
+    file_names = filter_names(file_names)
+    if "DataLocal.pack" not in file_names:
+        file_names.insert(0, "DataLocal.list")
+        file_names.insert(1, "DataLocal.pack")
+    return {"names" : file_names, "hashes" : hashes}
+
+def filter_names(names):
+    duplicates = ["NumberLocal", "UnitLocal"]
+
+    new_ls = names.copy()
+    for name in names:
+        name_split = name.split("_")
+        if len(name_split) == 2:
+            if name_split[0] in duplicates:
+                new_ls.remove(name)
+    return new_ls
+
+
+def readcstrs(start_address, end_address, data):
+    str = ""
+    strings = []
+    for i in range(start_address, end_address):
+        item = bytes([data[i]])
+
+        if item == b"\x00":
+            strings.append(str)
+            str = ""
+        else:
+            str += item.decode("utf-8")
+    return strings
+
+def generate_order(names, hashes, base_hash, base_name, skip=5, length=4):
+    data = {}
+    for i in range(length):
+        name_index = base_name + i*14
+        hash_index = base_hash + i*7
+
+        for j in range(6, -1, -1):
+            if i == length-1 and j < skip: break
+            name = names[name_index-(j*2)]
+            hash = hashes[hash_index-j]
+
+            data[name] = hash
+    return data
+
+def format(dict):
+    return json.dumps(dict, indent=4)
+
+def find_server_versions(names):
+    for name in names:
+        if "Server" in name:
+            return names.index(name)
+    return -1
+
+def get_length(length):
+    total_loops = math.ceil(length / 7)
+    skip = (total_loops*7) - length
+    return {"length" : total_loops, "skip" : skip}
+
+def server_lists_lengths(names):
+    version = ""
+    counter = 0
+    for name in names:
+        if "Server" in name and ".list" in name:
+            data = name.split("_")
+            if len(data) == 4:
+                if not version:
+                    version = name.split("_")[3][:2]
+                if version and version == name.split("_")[3][:2]:
+                    counter += 1
+            else:
+                counter += 1
+    
+    return get_length(counter)
+
+def find_order(path):
+    data = search_pos(path)
+    if not data:
+        return
+    names = data["names"]
+    hashes = data["hashes"]
+
+    hash_table = {}
+    hash_table.update(generate_order(names, hashes, 6, 12))
+    hash_table.update(generate_order(names, hashes, 33, 13))
+
+    server_version_index = find_server_versions(names)
+    lengths = server_lists_lengths(names)
+    hash_table.update(generate_order(names, hashes, server_version_index+6, server_version_index+12, lengths["skip"], lengths["length"]))
+
     return {"hash_table" : hash_table, "hash_list" : hashes}
```

### Comparing `battle-cats-game-modder-1.0.4/src/BCGM_Python/libnative/write_libnative_md5.py` & `battle-cats-game-modder-1.0.5/src/BCGM_Python/libnative/write_libnative_md5.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-import hashlib
-import helper
-import binascii
-import os
-from encrypt_decrypt import encrypt_pack
-from libnative import find_order
-
-def write_libnative(file_paths=None):
-    so_path = helper.select_files("Select a libnative-lib.so file", [("libnative-lib.so files", "*.so")])
-    if not so_path:
-        print("Please select an .so file")
-        return
-    if not file_paths:
-        file_paths = helper.select_files("Select modified .pack and .list files", [(".pack and .list files", "*.pack *.list")], False, encrypt_pack.output_path)
-        if not file_paths:
-            print("Please select .pack and .list files")
-            return
-
-    hash_data = find_order.find_order(so_path)
-    hash_list = hash_data["hash_list"]
-
-    start_pos = find_start_pos(so_path, hash_list[0])
-    for file in file_paths:
-        file_name = os.path.basename(file)
-
-        hash_list = hash_data["hash_list"]
-
-        current = hash_data["hash_table"][file_name]
-        index = hash_list.index(current)
-        file_data = helper.open_file_b(file)
-        hash = binascii.hexlify(hashlib.md5(file_data).digest())
-        if index == -1:
-            helper.coloured_text(f"{file_name} doesn't get checked by the game")
-            continue
-
-        pos = start_pos + (index*33)
-        write_hash(so_path, hash, pos)
-        helper.coloured_text(f"Set: &{file_name}& hash to &{hash.decode('utf-8')}&")
-    print("Successfully set hashes")
-    
-    push = helper.validate_bool(input("Do you want to push your modified libnative-lib.so file to the game (y/n)?:"))
-    if push:
-        gv = input("What game version are you using (en, jp, kr, tw)?:")
-        helper.adb_push_lib(gv.lower(), so_path)
-        print("Success")
-
-def find_start_pos(path, first_hash):
-    data = helper.open_file_b(path)
-    start_pos = data.find(first_hash.encode("utf-8"))
-    return start_pos
-
-def write_hash(path, hash, pos):
-    data = list(helper.open_file_b(path))
-    data = bytes(helper.insert_list(data, list(hash), pos))
+import hashlib
+import helper
+import binascii
+import os
+from encrypt_decrypt import encrypt_pack
+from libnative import find_order
+
+def write_libnative(file_paths=None):
+    so_path = helper.select_files("Select a libnative-lib.so file", [("libnative-lib.so files", "*.so")])
+    if not so_path:
+        print("Please select an .so file")
+        return
+    if not file_paths:
+        file_paths = helper.select_files("Select modified .pack and .list files", [(".pack and .list files", "*.pack *.list")], False, encrypt_pack.output_path)
+        if not file_paths:
+            print("Please select .pack and .list files")
+            return
+
+    hash_data = find_order.find_order(so_path)
+    hash_list = hash_data["hash_list"]
+
+    start_pos = find_start_pos(so_path, hash_list[0])
+    for file in file_paths:
+        file_name = os.path.basename(file)
+
+        hash_list = hash_data["hash_list"]
+
+        current = hash_data["hash_table"][file_name]
+        index = hash_list.index(current)
+        file_data = helper.open_file_b(file)
+        hash = binascii.hexlify(hashlib.md5(file_data).digest())
+        if index == -1:
+            helper.coloured_text(f"{file_name} doesn't get checked by the game")
+            continue
+
+        pos = start_pos + (index*33)
+        write_hash(so_path, hash, pos)
+        helper.coloured_text(f"Set: &{file_name}& hash to &{hash.decode('utf-8')}&")
+    print("Successfully set hashes")
+    
+    push = helper.validate_bool(input("Do you want to push your modified libnative-lib.so file to the game (y/n)?:"))
+    if push:
+        gv = input("What game version are you using (en, jp, kr, tw)?:")
+        helper.adb_push_lib(gv.lower(), so_path)
+        print("Success")
+
+def find_start_pos(path, first_hash):
+    data = helper.open_file_b(path)
+    start_pos = data.find(first_hash.encode("utf-8"))
+    return start_pos
+
+def write_hash(path, hash, pos):
+    data = list(helper.open_file_b(path))
+    data = bytes(helper.insert_list(data, list(hash), pos))
     helper.write_file_b(path, data)
```

### Comparing `battle-cats-game-modder-1.0.4/src/battle_cats_game_modder.egg-info/SOURCES.txt` & `battle-cats-game-modder-1.0.5/src/battle_cats_game_modder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

