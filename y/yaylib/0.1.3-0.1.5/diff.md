# Comparing `tmp/yaylib-0.1.3.tar.gz` & `tmp/yaylib-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaylib-0.1.3.tar", last modified: Sun Jun 25 08:32:04 2023, max compression
+gzip compressed data, was "yaylib-0.1.5.tar", last modified: Sat Jul  8 15:02:44 2023, max compression
```

## Comparing `yaylib-0.1.3.tar` & `yaylib-0.1.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 08:32:04.006271 yaylib-0.1.3/
--rw-rw-rw-   0        0        0     1088 2023-06-23 06:06:02.000000 yaylib-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     8215 2023-06-25 08:32:04.005228 yaylib-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     7358 2023-06-23 12:05:23.000000 yaylib-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-25 08:32:04.006271 yaylib-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1506 2023-06-25 08:29:29.000000 yaylib-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-25 08:32:03.970299 yaylib-0.1.3/tests/
--rw-rw-rw-   0        0        0      229 2023-06-23 06:06:02.000000 yaylib-0.1.3/tests/test_call.py
--rw-rw-rw-   0        0        0      829 2023-06-23 06:06:02.000000 yaylib-0.1.3/tests/test_cassandra.py
--rw-rw-rw-   0        0        0      229 2023-06-23 06:06:02.000000 yaylib-0.1.3/tests/test_chat.py
--rw-rw-rw-   0        0        0      231 2023-06-23 06:06:02.000000 yaylib-0.1.3/tests/test_group.py
--rw-rw-rw-   0        0        0      229 2023-06-23 06:06:02.000000 yaylib-0.1.3/tests/test_misc.py
--rw-rw-rw-   0        0        0     2552 2023-06-23 06:06:02.000000 yaylib-0.1.3/tests/test_post.py
--rw-rw-rw-   0        0        0      922 2023-06-23 06:06:02.000000 yaylib-0.1.3/tests/test_review.py
--rw-rw-rw-   0        0        0      233 2023-06-23 06:06:02.000000 yaylib-0.1.3/tests/test_thread.py
--rw-rw-rw-   0        0        0      229 2023-06-23 06:06:02.000000 yaylib-0.1.3/tests/test_user.py
-drwxrwxrwx   0        0        0        0 2023-06-25 08:32:03.977375 yaylib-0.1.3/yaylib/
--rw-rw-rw-   0        0        0      263 2023-06-23 06:06:02.000000 yaylib-0.1.3/yaylib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 08:32:04.004222 yaylib-0.1.3/yaylib/api/
--rw-rw-rw-   0        0        0      356 2023-05-31 13:14:39.000000 yaylib-0.1.3/yaylib/api/__init__.py
--rw-rw-rw-   0        0        0     6814 2023-06-23 06:06:02.000000 yaylib-0.1.3/yaylib/api/api.py
--rw-rw-rw-   0        0        0     7402 2023-06-23 06:06:02.000000 yaylib-0.1.3/yaylib/api/call.py
--rw-rw-rw-   0        0        0     1393 2023-06-23 06:06:02.000000 yaylib-0.1.3/yaylib/api/cassandra.py
--rw-rw-rw-   0        0        0    12827 2023-06-23 06:06:02.000000 yaylib-0.1.3/yaylib/api/chat.py
--rw-rw-rw-   0        0        0    19559 2023-06-23 06:06:02.000000 yaylib-0.1.3/yaylib/api/group.py
--rw-rw-rw-   0        0        0     4772 2023-06-23 06:06:02.000000 yaylib-0.1.3/yaylib/api/login.py
--rw-rw-rw-   0        0        0     5831 2023-06-23 06:06:02.000000 yaylib-0.1.3/yaylib/api/misc.py
--rw-rw-rw-   0        0        0    29363 2023-06-23 06:06:02.000000 yaylib-0.1.3/yaylib/api/post.py
--rw-rw-rw-   0        0        0     3492 2023-06-23 06:06:02.000000 yaylib-0.1.3/yaylib/api/review.py
--rw-rw-rw-   0        0        0     4082 2023-06-23 06:06:02.000000 yaylib-0.1.3/yaylib/api/thread.py
--rw-rw-rw-   0        0        0    21385 2023-06-23 12:05:23.000000 yaylib-0.1.3/yaylib/api/user.py
--rw-rw-rw-   0        0        0    76772 2023-06-23 12:05:23.000000 yaylib-0.1.3/yaylib/client.py
--rw-rw-rw-   0        0        0    17844 2023-06-25 08:32:00.000000 yaylib-0.1.3/yaylib/config.py
--rw-rw-rw-   0        0        0      373 2023-05-23 09:12:41.000000 yaylib-0.1.3/yaylib/errors.py
--rw-rw-rw-   0        0        0    50892 2023-06-23 06:06:02.000000 yaylib-0.1.3/yaylib/models.py
--rw-rw-rw-   0        0        0    31265 2023-06-23 06:06:02.000000 yaylib-0.1.3/yaylib/responses.py
--rw-rw-rw-   0        0        0     1079 2023-06-23 06:06:02.000000 yaylib-0.1.3/yaylib/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-25 08:32:03.990981 yaylib-0.1.3/yaylib.egg-info/
--rw-rw-rw-   0        0        0     8215 2023-06-25 08:32:03.000000 yaylib-0.1.3/yaylib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      721 2023-06-25 08:32:03.000000 yaylib-0.1.3/yaylib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 08:32:03.000000 yaylib-0.1.3/yaylib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-06-25 08:32:03.000000 yaylib-0.1.3/yaylib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-25 08:32:03.000000 yaylib-0.1.3/yaylib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 15:02:44.273987 yaylib-0.1.5/
+-rw-rw-rw-   0        0        0     1088 2023-07-08 04:33:49.000000 yaylib-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     8205 2023-07-08 15:02:44.273987 yaylib-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     7341 2023-07-08 15:02:21.000000 yaylib-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 15:02:44.273987 yaylib-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1552 2023-07-08 14:37:25.000000 yaylib-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 15:02:44.227270 yaylib-0.1.5/tests/
+-rw-rw-rw-   0        0        0      227 2023-07-08 14:37:25.000000 yaylib-0.1.5/tests/test_call.py
+-rw-rw-rw-   0        0        0      827 2023-07-08 14:37:25.000000 yaylib-0.1.5/tests/test_cassandra.py
+-rw-rw-rw-   0        0        0      227 2023-07-08 14:37:25.000000 yaylib-0.1.5/tests/test_chat.py
+-rw-rw-rw-   0        0        0      229 2023-07-08 14:37:25.000000 yaylib-0.1.5/tests/test_group.py
+-rw-rw-rw-   0        0        0      227 2023-07-08 14:37:25.000000 yaylib-0.1.5/tests/test_misc.py
+-rw-rw-rw-   0        0        0     2615 2023-07-08 14:37:25.000000 yaylib-0.1.5/tests/test_post.py
+-rw-rw-rw-   0        0        0      920 2023-07-08 14:37:25.000000 yaylib-0.1.5/tests/test_review.py
+-rw-rw-rw-   0        0        0      231 2023-07-08 14:37:25.000000 yaylib-0.1.5/tests/test_thread.py
+-rw-rw-rw-   0        0        0      227 2023-07-08 14:37:25.000000 yaylib-0.1.5/tests/test_user.py
+drwxrwxrwx   0        0        0        0 2023-07-08 15:02:44.234213 yaylib-0.1.5/yaylib/
+-rw-rw-rw-   0        0        0      288 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 15:02:44.272982 yaylib-0.1.5/yaylib/api/
+-rw-rw-rw-   0        0        0      466 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/api/__init__.py
+-rw-rw-rw-   0        0        0     8312 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/api/api.py
+-rw-rw-rw-   0        0        0     6242 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/api/call.py
+-rw-rw-rw-   0        0        0     1391 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/api/cassandra.py
+-rw-rw-rw-   0        0        0    11309 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/api/chat.py
+-rw-rw-rw-   0        0        0    19089 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/api/group.py
+-rw-rw-rw-   0        0        0     8042 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/api/login.py
+-rw-rw-rw-   0        0        0     5067 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/api/misc.py
+-rw-rw-rw-   0        0        0    28876 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/api/post.py
+-rw-rw-rw-   0        0        0     2847 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/api/review.py
+-rw-rw-rw-   0        0        0     4074 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/api/thread.py
+-rw-rw-rw-   0        0        0    17806 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/api/user.py
+-rw-rw-rw-   0        0        0    67557 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/client.py
+-rw-rw-rw-   0        0        0    18106 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/config.py
+-rw-rw-rw-   0        0        0      373 2023-07-08 10:04:28.000000 yaylib-0.1.5/yaylib/errors.py
+-rw-rw-rw-   0        0        0    52228 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/models.py
+-rw-rw-rw-   0        0        0    31004 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/responses.py
+-rw-rw-rw-   0        0        0     1428 2023-07-08 14:37:25.000000 yaylib-0.1.5/yaylib/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-08 15:02:44.260244 yaylib-0.1.5/yaylib.egg-info/
+-rw-rw-rw-   0        0        0     8205 2023-07-08 15:02:44.000000 yaylib-0.1.5/yaylib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      721 2023-07-08 15:02:44.000000 yaylib-0.1.5/yaylib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 15:02:44.000000 yaylib-0.1.5/yaylib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-08 15:02:44.000000 yaylib-0.1.5/yaylib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-08 15:02:44.000000 yaylib-0.1.5/yaylib.egg-info/top_level.txt
```

### Comparing `yaylib-0.1.3/LICENSE` & `yaylib-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yaylib-0.1.3/PKG-INFO` & `yaylib-0.1.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: yaylib
-Version: 0.1.3
+Version: 0.1.5
 Summary: This Python package provides an easy-to-use interface for accessing data from Yay! (https://yay.space/). With this API Client, you can retrieve user profiles, posts, comments, and other content from Yay!, as well as perform common tasks like liking and commenting on posts.
 Home-page: https://github.com/qvco/yaylib
 Download-URL: https://github.com/qvco/yaylib
 Author: Qvco, Konn
 Author-email: nikola.desuga@gmail.com
 Maintainer: Qvco, Konn
 Maintainer-email: nikola.desuga@gmail.com
 License: MIT
-Keywords: yay,yaylib,api,bot,library,wrapper,ボット,ライブラリ
+Keywords: yay,yaylib,api,bot,client,library,wrapper,ボット,ライブラリ
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div><a id="readme-top"></a></div>
@@ -21,27 +21,24 @@
     <img src="https://img.shields.io/github/stars/qvco/yaylib?style=for-the-badge&logo=appveyor&color=blue" />
     <img src="https://img.shields.io/github/forks/qvco/yaylib?style=for-the-badge&logo=appveyor&color=blue" />
     <img src="https://img.shields.io/github/issues/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational" />
     <img src="https://img.shields.io/github/issues-pr/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational" />
 </div>
 <br />
 <p align="center">
-<!--     <a href="https://github.com/othneildrew/Best-README-Template">
-        <img src="https://github.com/qvco/yaylib/assets/77382767/6e72ec90-b8e9-40bf-a7ad-34fb2ccea0f9" alt="Logo" height="300px">
-    </a> -->
     <a href="https://github.com/othneildrew/Best-README-Template">
-        <img src="https://github.com/qvco/yaylib/assets/77382767/5265b956-55b7-466c-8cdb-cf0f3abed946" alt="Logo" height="300px">
+        <img src="https://github.com/qvco/yaylib/assets/77382767/45c45b21-d812-4cad-8f27-315ffef53201" alt="Logo" height="300px">
     </a>
     <h3 align="center">yaylib</h3>
     <p align="center">
-        「<strong>yaylib</strong>」は同世代でつながるチャットアプリ、Yay!（イェイ）の API クライアントです。<br />
-        このライブラリを使用することで、あらゆる操作の自動化や、ボットの開発が可能です。
+        「<strong>yaylib</strong>」は同世代でつながるチャットアプリ、Yay!（イェイ）の API ラッパーです。<br />
+        あらゆる操作の自動化や、ボットの開発が可能です。
         <br />
         <br />
-        <a href="https://github.com/qvco/yaylib/blob/main/docs/README.md">
+        <a href="https://github.com/qvco/yaylib/blob/master/docs/README.md">
             <strong>詳しい機能の詳細や使い方はこちらから »</strong>
         </a>
         <br />
         <br />
         <a href="https://github.com/qvco/yaylib/issues">Report Bug</a>
         ·
         <a href="https://github.com/qvco/yaylib/issues">Request Feature</a>
@@ -65,26 +62,26 @@
   </ol>
 </details>
 
 <!-- Buy me a coffee -->
 
 ## Buy me a coffee
 
-もしこのライブラリが気に入っていただけたら、<a href="https://github.com/qvco/yaylib/">ぜひスターをお願いします</a> ⭐️  
+このライブラリが気に入っていただけたら、<a href="https://github.com/qvco/yaylib/">スターをお願いします</a> ⭐️  
 また、Buy Me a Coffee からご支援いただけますと幸いです。
 
 <a href="https://www.buymeacoffee.com/qvco" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: auto !important;width: auto !important;" ></a>
 
 <!-- インストール -->
 
 ## インストール
 
 **※ Python 3.11 かそれ以上のバージョンが必要です。**
 
-ライブラリをインストールするには、以下のコマンドを実行します:
+「yaylib」をインストールするには、以下のコマンドを実行します:
 
 ```bash
 pip install yaylib
 ```
 
 開発バージョンをインストールするには、以下の手順を実行します:
 
@@ -94,90 +91,97 @@
 cd yaylib
 
 pip install -r requirements.txt
 
 pip install -e .
 ```
 
-「yaylib」の始め方については、[こちら](https://github.com/qvco/yaylib/blob/main/docs/TUTORIAL.md) を確認してください。
+「yaylib」の始め方については、[こちら](https://github.com/qvco/yaylib/blob/master/docs/TUTORIAL.md) を確認してください。
 
 <!-- 使用例 -->
 
 ## 使用例
 
-メールアドレスとパスワードを用いてログイン後、新しく投稿を作成するコードです。
+メールアドレスとパスワードを使用してログインしたあと、タイムラインをキーワードで検索して「いいね」するコードです。
 
 ```python
 import yaylib
 
-api = yaylib.Client()
 
+api = yaylib.Client()
 api.login(email="メールアドレス", password="パスワード")
 
-api.create_post(text="初めての投稿！", color=2)
+timeline = api.get_timeline_by_keyword(
+    keyword="プログラミング",
+    number=15
+)
+
+for post in timeline.posts:
+    response = api.like_post(post.id)
+    print(post.id, response.data) # 実行結果を出力
 ```
 
-より詳しい使用例については、[こちら](https://github.com/qvco/yaylib/blob/main/examples) を参照してください。
+より詳しい使用例については、[こちら](https://github.com/qvco/yaylib/blob/master/examples) を参照してください。
 
 <p align="right">(<a href="#readme-top">トップに戻る</a>)</p>
 
 <!-- yaylib で誕生したボットの一覧 -->
 
 ## yaylib で誕生したロボットたち
 
-yaylib を用いて開発したロボットがある場合は、ぜひ教えてください！
+「yaylib」を用いて開発したロボットがある場合は、ぜひ教えてください！
 
 <table align="center">
     <thead>
         <tr>
             <th><a href="https://yay.space/user/5855987">MindReader AI</a></th>
-            <th><a href="https://yay.space/user/0">Funktion</a></th>
-            <th><a href="https://yay.space/user/0">香ばしいボット</a></th>
+            <th><a href="https://yay.space/user/7293290">香ばしいボット</a></th>
+            <th><a href="https://yay.space/user/7406336">GIGAZINE</a></th>
         </tr>
     </thead>
     <tbody>
         <tr>
             <td align="center">
-                <img src="https://github.com/qvco/yaylib/assets/77382767/472febe4-4c5f-490c-8417-de0d5dbbbc72" width="200px">
+                <img src="https://github.com/qvco/yaylib/assets/77382767/cc41ce3c-0e11-4ec5-be99-ff7090a95667" width="200px">
                 <br />
                 <p>開発者: <a href="https://yay.space/user/35152">毛の可能性</a></p>
             </td>
             <td align="center">
-                <img src="https://github.com/qvco/yaylib/assets/77382767/ff207016-21bf-4e76-b0e0-f70ebc4a121f" width="200px">
+                <img src="https://github.com/qvco/yaylib/assets/77382767/cbffdc25-7873-4242-b065-e6a686bade54" width="200px">
                 <br />
-                <p>開発者: <a href="https://yay.space/user/0">ぺゅー</a></p>
+                <p>開発者: <a href="https://yay.space/user/93923">めんぶれ天然水。</a></p>
             </td>
             <td align="center">
-                <img src="https://github.com/qvco/yaylib/assets/77382767/2324e518-b2c8-43cd-95e5-90ee2383aec1" width="200px">
+                <img src="https://github.com/qvco/yaylib/assets/77382767/65fcb885-4fbe-4170-9378-6f8d9af61ff8" width="200px">
                 <br />
-                <p>開発者: <a href="https://yay.space/user/0">めんぶれ天然水。</a></p>
+                <p>開発者: <a href="https://yay.space/user/1298298">ぺゅー</a></p>
             </td>
         </tr>
     </tbody>
 </table>
 
 <!-- 共同開発について -->
 
 ## 共同開発について
 
-私たちと一緒に開発することに興味を持っていただけているなら大歓迎です。
+私たちと開発することに興味を持っていただけているなら、ぜひ参加してください！
 
 - <a href="https://github.com/qvco/yaylib/pulls">プルリクエストを送信する</a>
 - <a href="mailto:nikola.desuga@gmail.com">nikola.desuga@gmail.com</a> にメールを送信する
 - <a href="https://discord.gg/MEuBfNtqRN">Discord サーバーに参加する</a>
 
-のいずれかの方法でコンタクトしてください。詳しくは[こちら](https://github.com/qvco/yaylib/blob/main/CONTRIBUTING.md)から！
+のいずれかの方法でコンタクトしてください。詳しくは[こちらから](https://github.com/qvco/yaylib/blob/master/CONTRIBUTING.md)！
 
 <!-- 免責事項 -->
 
 ## 免責事項
 
 yaylib は、API の公式なサポートやメンテナンスを提供するものではありません。このクライアントを使用する場合、利用者は**リスクや責任を自己負担**できるものとします。このクライアントによって提供される情報やデータの正確性、信頼性、完全性、適時性について、いかなる保証も行いません。また、このクライアントの使用によって生じた損害や不利益について、一切の責任を負いかねます。利用者は自己の責任において、このクライアントを使用し、API にアクセスするものとします。なお、この免責事項は予告なく変更される場合があります。
 
 <!-- 利用許諾 -->
 
 ## 利用許諾
 
-フルライセンスは [こちら](https://github.com/qvco/yaylib/blob/main/LICENSE) からご確認いただけます。  
+フルライセンスは [こちら](https://github.com/qvco/yaylib/blob/master/LICENSE) からご確認いただけます。  
 このプロジェクトは、 **【MIT ライセンス】** の条件の下でライセンスされています。
 
 <p align="right">(<a href="#readme-top">トップに戻る</a>)</p>
```

#### html2text {}

```diff
@@ -1,78 +1,80 @@
-Metadata-Version: 2.1 Name: yaylib Version: 0.1.3 Summary: This Python package
+Metadata-Version: 2.1 Name: yaylib Version: 0.1.5 Summary: This Python package
 provides an easy-to-use interface for accessing data from Yay! (https://
 yay.space/). With this API Client, you can retrieve user profiles, posts,
 comments, and other content from Yay!, as well as perform common tasks like
 liking and commenting on posts. Home-page: https://github.com/qvco/yaylib
 Download-URL: https://github.com/qvco/yaylib Author: Qvco, Konn Author-email:
 nikola.desuga@gmail.com Maintainer: Qvco, Konn Maintainer-email:
 nikola.desuga@gmail.com License: MIT Keywords:
-yay,yaylib,api,bot,library,wrapper,ããã,ã©ã¤ãã©ãª Classifier:
+yay,yaylib,api,bot,client,library,wrapper,ããã,ã©ã¤ãã©ãª Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.11 Description-
 Content-Type: text/markdown License-File: LICENSE
         [https://img.shields.io/github/stars/qvco/yaylib?style=for-the-
   badge&logo=appveyor&color=blue] [https://img.shields.io/github/forks/qvco/
  yaylib?style=for-the-badge&logo=appveyor&color=blue] [https://img.shields.io/
                    github/issues/qvco/yaylib?style=for-the-
 badge&logo=appveyor&color=informational] [https://img.shields.io/github/issues-
      pr/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational]
 
-                                     [Logo]
+                                    [Logo]
                                **** yaylib ****
 ãyaylibãã¯åä¸ä»£ã§ã¤ãªãããã£ããã¢ããªãYay!ï¼ã¤ã§ã¤ï¼ã®
-                        API ã¯ã©ã¤ã¢ã³ãã§ãã
-ãã®ã©ã¤ãã©ãªãä½¿ç¨ãããã¨ã§ãããããæä½ã®èªååãããããã®éçºãå¯è½ã§ãã
-
+                           API ã©ããã¼ã§ãã
+   ããããæä½ã®èªååãããããã®éçºãå¯è½ã§ãã
 
           è©³ããæ©è½ã®è©³ç´°ãä½¿ãæ¹ã¯ãã¡ããã_Â»
 
                Report_Bug Â· Request_Feature Â· Join_the_discord
   Table of Contents
    1. Buy_me_a_coffee
    2. ã¤ã³ã¹ãã¼ã«
    3. ä½¿ç¨ä¾
    4. yaylib_ã§èªçããã­ããããã¡
    5. å±åéçºã«ã¤ãã¦
    6. åè²¬äºé 
    7. å©ç¨è¨±è«¾
   ## Buy me a coffee
-ãããã®ã©ã¤ãã©ãªãæ°ã«å¥ã£ã¦ããã ãããããã²ã¹ã¿ã¼ããé¡ããã¾ã
+ãã®ã©ã¤ãã©ãªãæ°ã«å¥ã£ã¦ããã ããããã¹ã¿ã¼ããé¡ããã¾ã
 â­ï¸ ã¾ããBuy Me a Coffee
 ãããæ¯æ´ããã ãã¾ãã¨å¹¸ãã§ãã [Buy_Me_A_Coffee]  ##
 ã¤ã³ã¹ãã¼ã« **â» Python 3.11
 ãããä»¥ä¸ã®ãã¼ã¸ã§ã³ãå¿è¦ã§ãã**
-ã©ã¤ãã©ãªãã¤ã³ã¹ãã¼ã«ããã«ã¯ãä»¥ä¸ã®ã³ãã³ããå®è¡ãã¾ã:
+ãyaylibããã¤ã³ã¹ãã¼ã«ããã«ã¯ãä»¥ä¸ã®ã³ãã³ããå®è¡ãã¾ã:
 ```bash pip install yaylib ```
 éçºãã¼ã¸ã§ã³ãã¤ã³ã¹ãã¼ã«ããã«ã¯ãä»¥ä¸ã®æé ãå®è¡ãã¾ã:
 ```bash git clone https://github.com/qvco/yaylib cd yaylib pip install -
 r requirements.txt pip install -e . ```
 ãyaylibãã®å§ãæ¹ã«ã¤ãã¦ã¯ã[ãã¡ã](https://github.com/qvco/
-yaylib/blob/main/docs/TUTORIAL.md) ãç¢ºèªãã¦ãã ããã  ## ä½¿ç¨ä¾
-ã¡ã¼ã«ã¢ãã¬ã¹ã¨ãã¹ã¯ã¼ããç¨ãã¦ã­ã°ã¤ã³å¾ãæ°ããæç¨¿ãä½æããã³ã¼ãã§ãã
+yaylib/blob/master/docs/TUTORIAL.md) ãç¢ºèªãã¦ãã ããã  ##
+ä½¿ç¨ä¾
+ã¡ã¼ã«ã¢ãã¬ã¹ã¨ãã¹ã¯ã¼ããä½¿ç¨ãã¦ã­ã°ã¤ã³ãããã¨ãã¿ã¤ã ã©ã¤ã³ãã­ã¼ã¯ã¼ãã§æ¤ç´¢ãã¦ãããã­ãããã³ã¼ãã§ãã
 ```python import yaylib api = yaylib.Client() api.login
-(email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã") api.create_post
-(text="åãã¦ã®æç¨¿ï¼", color=2) ```
+(email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã") timeline =
+api.get_timeline_by_keyword( keyword="ãã­ã°ã©ãã³ã°", number=15 ) for
+post in timeline.posts: response = api.like_post(post.id) print(post.id,
+response.data) # å®è¡çµæãåºå ```
 ããè©³ããä½¿ç¨ä¾ã«ã¤ãã¦ã¯ã[ãã¡ã](https://github.com/qvco/
-yaylib/blob/main/examples) ãåç§ãã¦ãã ããã
+yaylib/blob/master/examples) ãåç§ãã¦ãã ããã
                                                            (ãããã«æ»ã)
- ## yaylib ã§èªçããã­ããããã¡ yaylib
-ãç¨ãã¦éçºããã­ããããããå ´åã¯ããã²æãã¦ãã ããï¼
-MindReader_AI                                      Funktion                               é¦ã°ããããã
- [https://github.com/qvco/yaylib/assets/77382767/     [https://github.com/qvco/yaylib/    [https://github.com/qvco/yaylib/assets/77382767/2324e518-b2c8-43cd-
-      472febe4-4c5f-490c-8417-de0d5dbbbc72]         assets/77382767/ff207016-21bf-4e76-                           95e5-90ee2383aec1]
-            éçºè: æ¯ã®å¯�         b0e0-f70ebc4a121f]                            éçºè: ããã¶ãå¤©ç¶æ°´ã
-                                                            éçºè: ãºãã¼
+ ## yaylib ã§èªçããã­ããããã¡
+ãyaylibããç¨ãã¦éçºããã­ããããããå ´åã¯ããã²æãã¦ãã ããï¼
+MindReader_AI                                      é¦ã°ããããã                           GIGAZINE
+ [https://github.com/qvco/yaylib/assets/77382767/  [https://github.com/qvco/yaylib/assets/77382767/cbffdc25-7873-4242-     [https://github.com/qvco/yaylib/
+      cc41ce3c-0e11-4ec5-be99-ff7090a95667]                                b065-e6a686bade54]                            assets/77382767/65fcb885-4fbe-4170-
+            éçºè: æ¯ã®å¯�                éçºè: ããã¶ãå¤©ç�         9378-6f8d9af61ff8]
+                                                                                                                                 éçºè: ãºãã¼
  ## å±åéçºã«ã¤ãã¦
-ç§ãã¡ã¨ä¸ç·ã«éçºãããã¨ã«èå³ãæã£ã¦ããã ãã¦ãããªãå¤§æ­è¿ã§ãã
+ç§ãã¡ã¨éçºãããã¨ã«èå³ãæã£ã¦ããã ãã¦ãããªãããã²åå ãã¦ãã ããï¼
 - ãã«ãªã¯ã¨ã¹ããéä¿¡ãã - nikola.desuga@gmail.com
 ã«ã¡ã¼ã«ãéä¿¡ãã - Discord_ãµã¼ãã¼ã«åå ãã
 ã®ããããã®æ¹æ³ã§ã³ã³ã¿ã¯ããã¦ãã ãããè©³ããã¯
-[ãã¡ã](https://github.com/qvco/yaylib/blob/main/CONTRIBUTING.md)ããï¼
-## åè²¬äºé  yaylib ã¯ãAPI
+[ãã¡ããã](https://github.com/qvco/yaylib/blob/master/
+CONTRIBUTING.md)ï¼  ## åè²¬äºé  yaylib ã¯ãAPI
 ã®å¬å¼ãªãµãã¼ããã¡ã³ããã³ã¹ãæä¾ãããã®ã§ã¯ããã¾ããããã®ã¯ã©ã¤ã¢ã³ããä½¿ç¨ããå ´åãå©ç¨èã¯**ãªã¹ã¯ãè²¬ä»»ãèªå·±è² æ**ã§ãããã®ã¨ãã¾ãããã®ã¯ã©ã¤ã¢ã³ãã«ãã£ã¦æä¾ãããæå ±ããã¼ã¿ã®æ­£ç¢ºæ§ãä¿¡é ¼æ§ãå®å¨æ§ãé©ææ§ã«ã¤ãã¦ããããªãä¿è¨¼ãè¡ãã¾ãããã¾ãããã®ã¯ã©ã¤ã¢ã³ãã®ä½¿ç¨ã«ãã£ã¦çããæå®³ãä¸å©çã«ã¤ãã¦ãä¸åã®è²¬ä»»ãè² ããã­ã¾ããå©ç¨èã¯èªå·±ã®è²¬ä»»ã«ããã¦ããã®ã¯ã©ã¤ã¢ã³ããä½¿ç¨ããAPI
 ã«ã¢ã¯ã»ã¹ãããã®ã¨ãã¾ãããªãããã®åè²¬äºé ã¯äºåãªãå¤æ´ãããå ´åãããã¾ãã
 ## å©ç¨è¨±è«¾ ãã«ã©ã¤ã»ã³ã¹ã¯ [ãã¡ã](https://github.com/qvco/
-yaylib/blob/main/LICENSE) ãããç¢ºèªããã ãã¾ãã
+yaylib/blob/master/LICENSE) ãããç¢ºèªããã ãã¾ãã
 ãã®ãã­ã¸ã§ã¯ãã¯ã **ãMIT ã©ã¤ã»ã³ã¹ã**
 ã®æ¡ä»¶ã®ä¸ã§ã©ã¤ã»ã³ã¹ããã¦ãã¾ãã
                                                            (ãããã«æ»ã)
```

### Comparing `yaylib-0.1.3/README.md` & `yaylib-0.1.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,27 +3,24 @@
     <img src="https://img.shields.io/github/stars/qvco/yaylib?style=for-the-badge&logo=appveyor&color=blue" />
     <img src="https://img.shields.io/github/forks/qvco/yaylib?style=for-the-badge&logo=appveyor&color=blue" />
     <img src="https://img.shields.io/github/issues/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational" />
     <img src="https://img.shields.io/github/issues-pr/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational" />
 </div>
 <br />
 <p align="center">
-<!--     <a href="https://github.com/othneildrew/Best-README-Template">
-        <img src="https://github.com/qvco/yaylib/assets/77382767/6e72ec90-b8e9-40bf-a7ad-34fb2ccea0f9" alt="Logo" height="300px">
-    </a> -->
     <a href="https://github.com/othneildrew/Best-README-Template">
-        <img src="https://github.com/qvco/yaylib/assets/77382767/5265b956-55b7-466c-8cdb-cf0f3abed946" alt="Logo" height="300px">
+        <img src="https://github.com/qvco/yaylib/assets/77382767/45c45b21-d812-4cad-8f27-315ffef53201" alt="Logo" height="300px">
     </a>
     <h3 align="center">yaylib</h3>
     <p align="center">
-        「<strong>yaylib</strong>」は同世代でつながるチャットアプリ、Yay!（イェイ）の API クライアントです。<br />
-        このライブラリを使用することで、あらゆる操作の自動化や、ボットの開発が可能です。
+        「<strong>yaylib</strong>」は同世代でつながるチャットアプリ、Yay!（イェイ）の API ラッパーです。<br />
+        あらゆる操作の自動化や、ボットの開発が可能です。
         <br />
         <br />
-        <a href="https://github.com/qvco/yaylib/blob/main/docs/README.md">
+        <a href="https://github.com/qvco/yaylib/blob/master/docs/README.md">
             <strong>詳しい機能の詳細や使い方はこちらから »</strong>
         </a>
         <br />
         <br />
         <a href="https://github.com/qvco/yaylib/issues">Report Bug</a>
         ·
         <a href="https://github.com/qvco/yaylib/issues">Request Feature</a>
@@ -47,26 +44,26 @@
   </ol>
 </details>
 
 <!-- Buy me a coffee -->
 
 ## Buy me a coffee
 
-もしこのライブラリが気に入っていただけたら、<a href="https://github.com/qvco/yaylib/">ぜひスターをお願いします</a> ⭐️  
+このライブラリが気に入っていただけたら、<a href="https://github.com/qvco/yaylib/">スターをお願いします</a> ⭐️  
 また、Buy Me a Coffee からご支援いただけますと幸いです。
 
 <a href="https://www.buymeacoffee.com/qvco" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: auto !important;width: auto !important;" ></a>
 
 <!-- インストール -->
 
 ## インストール
 
 **※ Python 3.11 かそれ以上のバージョンが必要です。**
 
-ライブラリをインストールするには、以下のコマンドを実行します:
+「yaylib」をインストールするには、以下のコマンドを実行します:
 
 ```bash
 pip install yaylib
 ```
 
 開発バージョンをインストールするには、以下の手順を実行します:
 
@@ -76,90 +73,97 @@
 cd yaylib
 
 pip install -r requirements.txt
 
 pip install -e .
 ```
 
-「yaylib」の始め方については、[こちら](https://github.com/qvco/yaylib/blob/main/docs/TUTORIAL.md) を確認してください。
+「yaylib」の始め方については、[こちら](https://github.com/qvco/yaylib/blob/master/docs/TUTORIAL.md) を確認してください。
 
 <!-- 使用例 -->
 
 ## 使用例
 
-メールアドレスとパスワードを用いてログイン後、新しく投稿を作成するコードです。
+メールアドレスとパスワードを使用してログインしたあと、タイムラインをキーワードで検索して「いいね」するコードです。
 
 ```python
 import yaylib
 
-api = yaylib.Client()
 
+api = yaylib.Client()
 api.login(email="メールアドレス", password="パスワード")
 
-api.create_post(text="初めての投稿！", color=2)
+timeline = api.get_timeline_by_keyword(
+    keyword="プログラミング",
+    number=15
+)
+
+for post in timeline.posts:
+    response = api.like_post(post.id)
+    print(post.id, response.data) # 実行結果を出力
 ```
 
-より詳しい使用例については、[こちら](https://github.com/qvco/yaylib/blob/main/examples) を参照してください。
+より詳しい使用例については、[こちら](https://github.com/qvco/yaylib/blob/master/examples) を参照してください。
 
 <p align="right">(<a href="#readme-top">トップに戻る</a>)</p>
 
 <!-- yaylib で誕生したボットの一覧 -->
 
 ## yaylib で誕生したロボットたち
 
-yaylib を用いて開発したロボットがある場合は、ぜひ教えてください！
+「yaylib」を用いて開発したロボットがある場合は、ぜひ教えてください！
 
 <table align="center">
     <thead>
         <tr>
             <th><a href="https://yay.space/user/5855987">MindReader AI</a></th>
-            <th><a href="https://yay.space/user/0">Funktion</a></th>
-            <th><a href="https://yay.space/user/0">香ばしいボット</a></th>
+            <th><a href="https://yay.space/user/7293290">香ばしいボット</a></th>
+            <th><a href="https://yay.space/user/7406336">GIGAZINE</a></th>
         </tr>
     </thead>
     <tbody>
         <tr>
             <td align="center">
-                <img src="https://github.com/qvco/yaylib/assets/77382767/472febe4-4c5f-490c-8417-de0d5dbbbc72" width="200px">
+                <img src="https://github.com/qvco/yaylib/assets/77382767/cc41ce3c-0e11-4ec5-be99-ff7090a95667" width="200px">
                 <br />
                 <p>開発者: <a href="https://yay.space/user/35152">毛の可能性</a></p>
             </td>
             <td align="center">
-                <img src="https://github.com/qvco/yaylib/assets/77382767/ff207016-21bf-4e76-b0e0-f70ebc4a121f" width="200px">
+                <img src="https://github.com/qvco/yaylib/assets/77382767/cbffdc25-7873-4242-b065-e6a686bade54" width="200px">
                 <br />
-                <p>開発者: <a href="https://yay.space/user/0">ぺゅー</a></p>
+                <p>開発者: <a href="https://yay.space/user/93923">めんぶれ天然水。</a></p>
             </td>
             <td align="center">
-                <img src="https://github.com/qvco/yaylib/assets/77382767/2324e518-b2c8-43cd-95e5-90ee2383aec1" width="200px">
+                <img src="https://github.com/qvco/yaylib/assets/77382767/65fcb885-4fbe-4170-9378-6f8d9af61ff8" width="200px">
                 <br />
-                <p>開発者: <a href="https://yay.space/user/0">めんぶれ天然水。</a></p>
+                <p>開発者: <a href="https://yay.space/user/1298298">ぺゅー</a></p>
             </td>
         </tr>
     </tbody>
 </table>
 
 <!-- 共同開発について -->
 
 ## 共同開発について
 
-私たちと一緒に開発することに興味を持っていただけているなら大歓迎です。
+私たちと開発することに興味を持っていただけているなら、ぜひ参加してください！
 
 - <a href="https://github.com/qvco/yaylib/pulls">プルリクエストを送信する</a>
 - <a href="mailto:nikola.desuga@gmail.com">nikola.desuga@gmail.com</a> にメールを送信する
 - <a href="https://discord.gg/MEuBfNtqRN">Discord サーバーに参加する</a>
 
-のいずれかの方法でコンタクトしてください。詳しくは[こちら](https://github.com/qvco/yaylib/blob/main/CONTRIBUTING.md)から！
+のいずれかの方法でコンタクトしてください。詳しくは[こちらから](https://github.com/qvco/yaylib/blob/master/CONTRIBUTING.md)！
 
 <!-- 免責事項 -->
 
 ## 免責事項
 
 yaylib は、API の公式なサポートやメンテナンスを提供するものではありません。このクライアントを使用する場合、利用者は**リスクや責任を自己負担**できるものとします。このクライアントによって提供される情報やデータの正確性、信頼性、完全性、適時性について、いかなる保証も行いません。また、このクライアントの使用によって生じた損害や不利益について、一切の責任を負いかねます。利用者は自己の責任において、このクライアントを使用し、API にアクセスするものとします。なお、この免責事項は予告なく変更される場合があります。
 
 <!-- 利用許諾 -->
 
 ## 利用許諾
 
-フルライセンスは [こちら](https://github.com/qvco/yaylib/blob/main/LICENSE) からご確認いただけます。  
+フルライセンスは [こちら](https://github.com/qvco/yaylib/blob/master/LICENSE) からご確認いただけます。  
 このプロジェクトは、 **【MIT ライセンス】** の条件の下でライセンスされています。
 
 <p align="right">(<a href="#readme-top">トップに戻る</a>)</p>
```

#### html2text {}

```diff
@@ -1,66 +1,68 @@
         [https://img.shields.io/github/stars/qvco/yaylib?style=for-the-
   badge&logo=appveyor&color=blue] [https://img.shields.io/github/forks/qvco/
  yaylib?style=for-the-badge&logo=appveyor&color=blue] [https://img.shields.io/
                    github/issues/qvco/yaylib?style=for-the-
 badge&logo=appveyor&color=informational] [https://img.shields.io/github/issues-
      pr/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational]
 
-                                     [Logo]
+                                    [Logo]
                                **** yaylib ****
 ãyaylibãã¯åä¸ä»£ã§ã¤ãªãããã£ããã¢ããªãYay!ï¼ã¤ã§ã¤ï¼ã®
-                        API ã¯ã©ã¤ã¢ã³ãã§ãã
-ãã®ã©ã¤ãã©ãªãä½¿ç¨ãããã¨ã§ãããããæä½ã®èªååãããããã®éçºãå¯è½ã§ãã
-
+                           API ã©ããã¼ã§ãã
+   ããããæä½ã®èªååãããããã®éçºãå¯è½ã§ãã
 
           è©³ããæ©è½ã®è©³ç´°ãä½¿ãæ¹ã¯ãã¡ããã_Â»
 
                Report_Bug Â· Request_Feature Â· Join_the_discord
   Table of Contents
    1. Buy_me_a_coffee
    2. ã¤ã³ã¹ãã¼ã«
    3. ä½¿ç¨ä¾
    4. yaylib_ã§èªçããã­ããããã¡
    5. å±åéçºã«ã¤ãã¦
    6. åè²¬äºé 
    7. å©ç¨è¨±è«¾
   ## Buy me a coffee
-ãããã®ã©ã¤ãã©ãªãæ°ã«å¥ã£ã¦ããã ãããããã²ã¹ã¿ã¼ããé¡ããã¾ã
+ãã®ã©ã¤ãã©ãªãæ°ã«å¥ã£ã¦ããã ããããã¹ã¿ã¼ããé¡ããã¾ã
 â­ï¸ ã¾ããBuy Me a Coffee
 ãããæ¯æ´ããã ãã¾ãã¨å¹¸ãã§ãã [Buy_Me_A_Coffee]  ##
 ã¤ã³ã¹ãã¼ã« **â» Python 3.11
 ãããä»¥ä¸ã®ãã¼ã¸ã§ã³ãå¿è¦ã§ãã**
-ã©ã¤ãã©ãªãã¤ã³ã¹ãã¼ã«ããã«ã¯ãä»¥ä¸ã®ã³ãã³ããå®è¡ãã¾ã:
+ãyaylibããã¤ã³ã¹ãã¼ã«ããã«ã¯ãä»¥ä¸ã®ã³ãã³ããå®è¡ãã¾ã:
 ```bash pip install yaylib ```
 éçºãã¼ã¸ã§ã³ãã¤ã³ã¹ãã¼ã«ããã«ã¯ãä»¥ä¸ã®æé ãå®è¡ãã¾ã:
 ```bash git clone https://github.com/qvco/yaylib cd yaylib pip install -
 r requirements.txt pip install -e . ```
 ãyaylibãã®å§ãæ¹ã«ã¤ãã¦ã¯ã[ãã¡ã](https://github.com/qvco/
-yaylib/blob/main/docs/TUTORIAL.md) ãç¢ºèªãã¦ãã ããã  ## ä½¿ç¨ä¾
-ã¡ã¼ã«ã¢ãã¬ã¹ã¨ãã¹ã¯ã¼ããç¨ãã¦ã­ã°ã¤ã³å¾ãæ°ããæç¨¿ãä½æããã³ã¼ãã§ãã
+yaylib/blob/master/docs/TUTORIAL.md) ãç¢ºèªãã¦ãã ããã  ##
+ä½¿ç¨ä¾
+ã¡ã¼ã«ã¢ãã¬ã¹ã¨ãã¹ã¯ã¼ããä½¿ç¨ãã¦ã­ã°ã¤ã³ãããã¨ãã¿ã¤ã ã©ã¤ã³ãã­ã¼ã¯ã¼ãã§æ¤ç´¢ãã¦ãããã­ãããã³ã¼ãã§ãã
 ```python import yaylib api = yaylib.Client() api.login
-(email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã") api.create_post
-(text="åãã¦ã®æç¨¿ï¼", color=2) ```
+(email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã") timeline =
+api.get_timeline_by_keyword( keyword="ãã­ã°ã©ãã³ã°", number=15 ) for
+post in timeline.posts: response = api.like_post(post.id) print(post.id,
+response.data) # å®è¡çµæãåºå ```
 ããè©³ããä½¿ç¨ä¾ã«ã¤ãã¦ã¯ã[ãã¡ã](https://github.com/qvco/
-yaylib/blob/main/examples) ãåç§ãã¦ãã ããã
+yaylib/blob/master/examples) ãåç§ãã¦ãã ããã
                                                            (ãããã«æ»ã)
- ## yaylib ã§èªçããã­ããããã¡ yaylib
-ãç¨ãã¦éçºããã­ããããããå ´åã¯ããã²æãã¦ãã ããï¼
-MindReader_AI                                      Funktion                               é¦ã°ããããã
- [https://github.com/qvco/yaylib/assets/77382767/     [https://github.com/qvco/yaylib/    [https://github.com/qvco/yaylib/assets/77382767/2324e518-b2c8-43cd-
-      472febe4-4c5f-490c-8417-de0d5dbbbc72]         assets/77382767/ff207016-21bf-4e76-                           95e5-90ee2383aec1]
-            éçºè: æ¯ã®å¯�         b0e0-f70ebc4a121f]                            éçºè: ããã¶ãå¤©ç¶æ°´ã
-                                                            éçºè: ãºãã¼
+ ## yaylib ã§èªçããã­ããããã¡
+ãyaylibããç¨ãã¦éçºããã­ããããããå ´åã¯ããã²æãã¦ãã ããï¼
+MindReader_AI                                      é¦ã°ããããã                           GIGAZINE
+ [https://github.com/qvco/yaylib/assets/77382767/  [https://github.com/qvco/yaylib/assets/77382767/cbffdc25-7873-4242-     [https://github.com/qvco/yaylib/
+      cc41ce3c-0e11-4ec5-be99-ff7090a95667]                                b065-e6a686bade54]                            assets/77382767/65fcb885-4fbe-4170-
+            éçºè: æ¯ã®å¯�                éçºè: ããã¶ãå¤©ç�         9378-6f8d9af61ff8]
+                                                                                                                                 éçºè: ãºãã¼
  ## å±åéçºã«ã¤ãã¦
-ç§ãã¡ã¨ä¸ç·ã«éçºãããã¨ã«èå³ãæã£ã¦ããã ãã¦ãããªãå¤§æ­è¿ã§ãã
+ç§ãã¡ã¨éçºãããã¨ã«èå³ãæã£ã¦ããã ãã¦ãããªãããã²åå ãã¦ãã ããï¼
 - ãã«ãªã¯ã¨ã¹ããéä¿¡ãã - nikola.desuga@gmail.com
 ã«ã¡ã¼ã«ãéä¿¡ãã - Discord_ãµã¼ãã¼ã«åå ãã
 ã®ããããã®æ¹æ³ã§ã³ã³ã¿ã¯ããã¦ãã ãããè©³ããã¯
-[ãã¡ã](https://github.com/qvco/yaylib/blob/main/CONTRIBUTING.md)ããï¼
-## åè²¬äºé  yaylib ã¯ãAPI
+[ãã¡ããã](https://github.com/qvco/yaylib/blob/master/
+CONTRIBUTING.md)ï¼  ## åè²¬äºé  yaylib ã¯ãAPI
 ã®å¬å¼ãªãµãã¼ããã¡ã³ããã³ã¹ãæä¾ãããã®ã§ã¯ããã¾ããããã®ã¯ã©ã¤ã¢ã³ããä½¿ç¨ããå ´åãå©ç¨èã¯**ãªã¹ã¯ãè²¬ä»»ãèªå·±è² æ**ã§ãããã®ã¨ãã¾ãããã®ã¯ã©ã¤ã¢ã³ãã«ãã£ã¦æä¾ãããæå ±ããã¼ã¿ã®æ­£ç¢ºæ§ãä¿¡é ¼æ§ãå®å¨æ§ãé©ææ§ã«ã¤ãã¦ããããªãä¿è¨¼ãè¡ãã¾ãããã¾ãããã®ã¯ã©ã¤ã¢ã³ãã®ä½¿ç¨ã«ãã£ã¦çããæå®³ãä¸å©çã«ã¤ãã¦ãä¸åã®è²¬ä»»ãè² ããã­ã¾ããå©ç¨èã¯èªå·±ã®è²¬ä»»ã«ããã¦ããã®ã¯ã©ã¤ã¢ã³ããä½¿ç¨ããAPI
 ã«ã¢ã¯ã»ã¹ãããã®ã¨ãã¾ãããªãããã®åè²¬äºé ã¯äºåãªãå¤æ´ãããå ´åãããã¾ãã
 ## å©ç¨è¨±è«¾ ãã«ã©ã¤ã»ã³ã¹ã¯ [ãã¡ã](https://github.com/qvco/
-yaylib/blob/main/LICENSE) ãããç¢ºèªããã ãã¾ãã
+yaylib/blob/master/LICENSE) ãããç¢ºèªããã ãã¾ãã
 ãã®ãã­ã¸ã§ã¯ãã¯ã **ãMIT ã©ã¤ã»ã³ã¹ã**
 ã®æ¡ä»¶ã®ä¸ã§ã©ã¤ã»ã³ã¹ããã¦ãã¾ãã
                                                            (ãããã«æ»ã)
```

### Comparing `yaylib-0.1.3/setup.py` & `yaylib-0.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,23 +10,25 @@
 url = "https://github.com/qvco/yaylib"
 
 keywords = [
     "yay",
     "yaylib",
     "api",
     "bot",
+    "client",
     "library",
     "wrapper",
     "ボット",
-    "ライブラリ"
+    "ライブラリ",
 ]
 
 install_requires = [
     "httpx>=0.17.1",
-    "Pillow>=9.3.0"
+    "Pillow>=9.3.0",
+    "cryptography>=41.0.1",
 ]
 
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.11",
 ]
```

### Comparing `yaylib-0.1.3/tests/test_cassandra.py` & `yaylib-0.1.5/tests/test_cassandra.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,14 @@
     user_id,
     opponent_id,
     YaylibTestCase,
 )
 
 
 class YaylibCassandraTests(YaylibTestCase):
-
     path = "./cassandra/"
 
     @tape.use_cassette(path + "test_get_user_activities.yaml")
     def test_get_user_activities(self):
         number = 1
         self.api.get_user_activities(number=number)
 
@@ -25,9 +24,9 @@
     # @tape.use_cassette(path + "test_received_notification.yaml")
     # def test_received_notification(self):
     #     pid = ""
     #     type = ""
     #     self.api.received_notification(pid, type)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `yaylib-0.1.3/tests/test_post.py` & `yaylib-0.1.5/tests/test_post.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,38 +5,46 @@
     user_id,
     opponent_id,
     YaylibTestCase,
 )
 
 
 class YaylibPostTests(YaylibTestCase):
-
     path = "./post/"
 
     @tape.use_cassette(path + "posts.yaml")
     def test_posts(self):
         text = "testing"
         font_size = 2
         color = 3
         number = 1
 
         # create post
         post_id = self.api.create_post(
-            text, font_size, color,
+            text,
+            font_size,
+            color,
         ).id
         self.api.get_post(post_id=post_id)
 
         # create reply
         conversation_id = self.api.create_post(
-            text, font_size, color, in_reply_to=post_id,
+            text,
+            font_size,
+            color,
+            in_reply_to=post_id,
         ).conversation_id
         self.api.get_conversation(conversation_id, number=number)
         self.api.get_conversation_root_posts(conversation_id)
         self.api.create_repost(
-            post_id, text, font_size, color, in_reply_to=post_id,
+            post_id,
+            text,
+            font_size,
+            color,
+            in_reply_to=post_id,
         )
         self.api.get_post_reposts(post_id=post_id, number=number)
 
     @tape.use_cassette(path + "timeline.yaml")
     def test_timeline(self):
         number = 1
         user_id = 93
@@ -50,32 +58,28 @@
         self.api.get_timeline(number=number, noreply_mode=True)
         self.api.get_timeline_by_keyword(keyword=keyword, number=number)
         self.api.get_timeline_by_hashtag(hashtag=hashtag, number=number)
         self.api.get_timeline_calls(number=number)
         self.api.get_timeline_calls(number=number, group_id=group_id)
         self.api.get_group_timeline(group_id=group_id, number=number)
         self.api.get_group_timeline_by_keyword(
-            group_id=group_id,
-            keyword=keyword,
-            number=number
+            group_id=group_id, keyword=keyword, number=number
         )
         self.api.get_following_timeline(number=number)
         self.api.get_following_call_timeline(number=number)
         self.api.get_recommended_posts(
-            number=number,
-            experiment_num=experiment_num,
-            variant_num=variant_num
+            number=number, experiment_num=experiment_num, variant_num=variant_num
         )
         self.api.get_user_timeline(user_id=user_id, number=number)
         self.api.get_my_posts(number=number)
 
     @tape.use_cassette(path + "bookmarks.yaml")
     def test_bookmarks(self):
         post_id = 371574235
 
         self.api.add_bookmark(user_id, post_id)
         self.api.get_bookmark(user_id)
         self.api.remove_bookmark(user_id, post_id)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `yaylib-0.1.3/tests/test_review.py` & `yaylib-0.1.5/tests/test_review.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
     user_id,
     opponent_id,
     YaylibTestCase,
 )
 
 
 class YaylibReviewTests(YaylibTestCase):
-
     path = "./review/"
 
     @tape.use_cassette(path + "reviews.yaml")
     def test_bookmarks(self):
         comment = "testing"
         number = 1
 
@@ -30,9 +29,9 @@
             self.api.unpin_review(review_id)
 
         reviews = self.api.get_my_reviews(number=number).reviews
         review_id = reviews[0].id
         self.api.delete_reviews([review_id])
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `yaylib-0.1.3/yaylib/api/api.py` & `yaylib-0.1.5/yaylib/api/api.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,162 +3,204 @@
 import logging
 
 from json import JSONDecodeError
 from typing import Optional, Dict, Any
 
 import httpx
 
+from .login import *
+
 from ..config import *
 from ..errors import *
-from ..responses import LoginUserResponse
+from ..responses import *
 from ..utils import *
 
 
 current_path = os.path.abspath(os.getcwd())
 
 
 class API:
-
     def __init__(
-            self,
-            access_token: str = None,
-            refresh_token: str = None,
-            proxy: str = None,
-            max_retries=3,
-            backoff_factor=1.0,
-            timeout=30,
-            lang="ja",
-            base_path=current_path,
-            loglevel_stream=logging.INFO,
-            host=Configs.YAY_PRODUCTION_HOST,
+        self,
+        access_token: str = None,
+        proxy: str = None,
+        max_retries=3,
+        backoff_factor=1.0,
+        timeout=30,
+        err_lang="ja",
+        base_path=current_path + "/config/",
+        loglevel_stream=logging.INFO,
+        host=Configs.YAY_PRODUCTION_HOST,
     ):
         self.yaylib_version = Configs.YAYLIB_VERSION
         self.api_version = Configs.YAY_API_VERSION
         self.api_key = Configs.YAY_API_KEY
-
-        self.login_data = LoginUserResponse({
-            "access_token": access_token,
-            "refresh_token": refresh_token,
-        })
+        self.secret_key = None
 
         self.proxy = {}
         if proxy is not None:
             self.proxy["https"] = proxy
 
         self.max_retries = max_retries
         self.retry_statuses = [500, 502, 503, 504]
         self.backoff_factor = backoff_factor
         self.timeout = timeout
-        self.lang = lang
+        self.err_lang = err_lang
         self.base_path = base_path
         self.host = "https://" + host
 
         self.generate_all_uuids()
         self.session = httpx.Client(proxies=self.proxy, timeout=self.timeout)
         self.session.headers.update(Configs.REQUEST_HEADERS)
         self.session.headers.update({"X-Device-Uuid": self.device_uuid})
         if access_token:
-            self.session.headers.setdefault(
-                "Authorization", f"Bearer {access_token}"
-            )
+            self.session.headers.setdefault("Authorization", f"Bearer {access_token}")
+
+        self.logger = logging.getLogger("yaylib version: " + self.yaylib_version)
+
+        if not os.path.exists(base_path):
+            os.makedirs(base_path)
 
-        self.logger = logging.getLogger(
-            "yaylib version: " + self.yaylib_version
-        )
         ch = logging.StreamHandler()
         ch.setLevel(loglevel_stream)
-        ch.setFormatter(logging.Formatter(
-            "%(asctime)s - %(levelname)s - %(message)s"
-        ))
+        ch.setFormatter(logging.Formatter("%(asctime)s - %(levelname)s - %(message)s"))
 
         handler_existed = False
         for handler in self.logger.handlers:
             if isinstance(handler, logging.StreamHandler):
                 handler_existed = True
                 break
         if not handler_existed:
             self.logger.addHandler(ch)
         self.logger.setLevel(logging.DEBUG)
 
         self.logger.info("yaylib version: " + self.yaylib_version + " started")
 
-    def request(self, method, endpoint, params=None, payload=None, user_auth=True, headers=None):
+    def request(
+        self, method, endpoint, params=None, payload=None, user_auth=True, headers=None
+    ):
+        headers = headers or self.session.headers
 
-        if headers is None:
-            headers = self.session.headers
         if not user_auth:
-            headers["Authorization"] = None
+            del headers["Authorization"]
 
         response = None
         backoff_duration = 0
+        auth_retry_count = 0
+        max_auth_retries = 2
 
         for i in range(self.max_retries):
             time.sleep(backoff_duration)
-            try:
 
-                self.logger.debug(
-                    "Making API request:\n\n"
-                    f"{method}: {endpoint}\n\n"
-                    f"Parameters: {params}\n\n"
-                    f"Headers: {headers}\n\n"
-                    f"Body: {payload}\n"
-                )
-                response = self.session.request(
-                    method, endpoint, params=params, json=payload, headers=headers
-                )
-                self.logger.debug(
-                    "Received API response:\n\n"
-                    f"Status Code: {response.status_code}\n\n"
-                    f"Headers: {response.headers}\n\n"
-                    f"Response: {response.text}\n"
-                )
+            self.logger.debug(
+                "Making API request:\n\n"
+                f"{method}: {endpoint}\n\n"
+                f"Parameters: {params}\n\n"
+                f"Headers: {headers}\n\n"
+                f"Body: {payload}\n"
+            )
+
+            response = self.session.request(
+                method, endpoint, params=params, json=payload, headers=headers
+            )
 
-                if response.status_code not in self.retry_statuses:
-                    break
+            if response.status_code == 401:
+                if "/api/v1/oauth/token" in endpoint:
+                    os.remove(self.base_path + "credentials.json")
+                    message = "Refresh token expired. Try logging in again."
+                    raise AuthenticationError(message)
+
+                auth_retry_count += 1
+                self.logger.debug("Access token expired. Refreshing tokens...")
+
+                if auth_retry_count < max_auth_retries:
+                    credentials = load_credentials(self)
+
+                    if credentials is not None:
+                        refresh_token = credentials["refresh_token"]
+                        response = get_token(
+                            self,
+                            grant_type="refresh_token",
+                            refresh_token=refresh_token,
+                        )
+                        save_credentials(
+                            self,
+                            response.access_token,
+                            response.refresh_token,
+                            response.user_id,
+                        )
+                        self.session.headers[
+                            "Authorization"
+                        ] = f"Bearer {response.access_token}"
+                        continue
+
+                else:
+                    os.remove(self.base_path + "credentials.json")
+                    message = (
+                        "Maximum authentication retries exceeded. Try logging in again."
+                    )
+                    raise AuthenticationError(message)
 
-            except httpx.HTTPError:
-                pass
+            if response.status_code not in self.retry_statuses:
+                break
 
             if response is not None:
                 self.logger.error(
-                    f"Request failed with status code {response.status_code}. Retrying...")
+                    f"Request failed with status code {response.status_code}. Retrying...",
+                    exc_info=True,
+                )
             else:
                 self.logger.error("Request failed. Retrying...")
-            backoff_duration = self.backoff_factor * (2 ** i)
+
+            backoff_duration = self.backoff_factor * (2**i)
+
+        if response is None:
+            return None
+
+        self.logger.debug(
+            "Received API response:\n\n"
+            f"Status Code: {response.status_code}\n\n"
+            f"Headers: {response.headers}\n\n"
+            f"Response: {response.text}\n"
+        )
 
         try:
             json_response = response.json()
         except JSONDecodeError:
             return response.text
 
         return self._handle_response(response, json_response)
 
     def _make_request(
-            self, method: str, endpoint: str, params: dict = None,
-            payload: dict = None, data_type=None, user_auth=True, headers=None
+        self,
+        method: str,
+        endpoint: str,
+        params: dict = None,
+        payload: dict = None,
+        data_type=None,
+        user_auth=True,
+        headers=None,
     ):
-        response = self.request(
-            method, endpoint, params, payload, user_auth, headers
-        )
+        response = self.request(method, endpoint, params, payload, user_auth, headers)
         if data_type:
             return self._construct_response(response, data_type)
         return response
 
     def _construct_response(self, data, data_type):
         if data_type is not None:
             if isinstance(data, list):
                 data = [data_type(result) for result in data]
             elif data is not None:
                 data = data_type(data)
         return data
 
     def _check_authorization(self) -> None:
         if self.session.headers.get("Authorization") is None:
-            raise AuthenticationError(
-                "Authorization is not present in the header.")
+            message = "Authorization is not present in the header."
+            raise AuthenticationError(message)
 
     def _handle_response(self, response, json_response):
         translated_response = self.translate_error_message(json_response)
         if response.status_code == 400:
             raise BadRequestError(translated_response)
         if response.status_code == 401:
             raise AuthenticationError(translated_response)
@@ -171,15 +213,15 @@
         if response.status_code == 500:
             raise YayServerError(translated_response)
         if response.status_code and not 200 <= response.status_code < 300:
             raise HTTPError(translated_response)
         return json_response
 
     def translate_error_message(self, response):
-        if self.lang == "ja":
+        if self.err_lang == "ja":
             try:
                 error_code = response.get("error_code", None)
                 if error_code is not None:
                     error_type = ErrorType(error_code)
                     if error_type.name in ErrorMessage.__members__:
                         error_message = ErrorMessage[error_type.name].value
                         response["message"] = error_message
```

### Comparing `yaylib-0.1.3/yaylib/api/call.py` & `yaylib-0.1.5/yaylib/api/call.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,88 +9,98 @@
 
 
 def bump_call(self, call_id: int, participant_limit: int = None):
     params = {}
     if participant_limit:
         params["participant_limit"] = participant_limit
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.CALLS_V1}/{call_id}/bump",
-        params=params
+        "POST", endpoint=f"{Endpoints.CALLS_V1}/{call_id}/bump", params=params
     )
     self.logger.info("Call bumped.")
     return response
 
 
 def get_user_active_call(self, user_id: int) -> Post:
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.POSTS_V1}/active_call",
-        params={"user_id": user_id}, data_type=PostResponse
+        "GET",
+        endpoint=f"{Endpoints.POSTS_V1}/active_call",
+        params={"user_id": user_id},
+        data_type=PostResponse,
     ).post
 
 
 def get_bgms(self) -> List[Bgm]:
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.CALLS_V1}/bgm",
-        data_type=BgmsResponse
+        "GET", endpoint=f"{Endpoints.CALLS_V1}/bgm", data_type=BgmsResponse
     ).bgm
 
 
 def get_call(self, call_id: int) -> ConferenceCall:
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.CALLS_V1}/conferences/{call_id}",
-        data_type=ConferenceCallResponse
+        "GET",
+        endpoint=f"{Endpoints.CALLS_V1}/conferences/{call_id}",
+        data_type=ConferenceCallResponse,
     ).conference_call
 
 
-def get_call_invitable_users(self, call_id: int, from_timestamp: int = None) -> UsersByTimestampResponse:
+def get_call_invitable_users(
+    self, call_id: int, from_timestamp: int = None
+) -> UsersByTimestampResponse:
     # @Nullable @Query("user[nickname]")
     params = {}
     if from_timestamp:
         params["from_timestamp"] = from_timestamp
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.CALLS_V1}/{call_id}/users/invitable",
-        params=params, data_type=UsersByTimestampResponse
+        "GET",
+        endpoint=f"{Endpoints.CALLS_V1}/{call_id}/users/invitable",
+        params=params,
+        data_type=UsersByTimestampResponse,
     )
 
 
 def get_call_status(self, opponent_id: int) -> CallStatusResponse:
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.CALLS_V1}/phone_status/{opponent_id}",
-        data_type=CallStatusResponse
+        "GET",
+        endpoint=f"{Endpoints.CALLS_V1}/phone_status/{opponent_id}",
+        data_type=CallStatusResponse,
     )
 
 
 def get_games(self, **params) -> GamesResponse:
     """
 
     Parameters
     ----------
         - number: int - (optional)
         - ids: List[int] - (optional)
         - from_id: int - (optional)
 
     """
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.GAMES_V1}/apps",
-        params=params, data_type=GamesResponse
+        "GET",
+        endpoint=f"{Endpoints.GAMES_V1}/apps",
+        params=params,
+        data_type=GamesResponse,
     )
 
 
 def get_genres(self, **params) -> GenresResponse:
     """
 
     Parameters
     ----------
         - number: int - (optional)
         - from: int - (optional)
 
     """
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.GENRES_V1}",
-        params=params, data_type=GenresResponse
+        "GET",
+        endpoint=f"{Endpoints.GENRES_V1}",
+        params=params,
+        data_type=GenresResponse,
     )
 
 
 def get_group_calls(self, **params) -> PostsResponse:
     """
 
     Parameters
@@ -98,16 +108,18 @@
         - number: int - (optional)
         - group_category_id: int - (optional)
         - from_timestamp: int - (optional)
         - scope: str - (optional)
 
     """
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.POSTS_V1}/group_calls",
-        params=params, data_type=PostsResponse
+        "GET",
+        endpoint=f"{Endpoints.POSTS_V1}/group_calls",
+        params=params,
+        data_type=PostsResponse,
     )
 
 
 def invite_to_call_bulk(self, call_id: int, group_id: int = None):
     """
 
     Parameters
@@ -116,16 +128,15 @@
         - group_id: int - (optional)
 
     """
     params = {}
     if group_id:
         params["group_id"] = group_id
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.CALLS_V1}/{call_id}/bulk_invite",
-        params=params
+        "POST", endpoint=f"{Endpoints.CALLS_V1}/{call_id}/bulk_invite", params=params
     )
     self.logger.info("Invited your online followings to the call.")
     return response
 
 
 def invite_users_to_call(self, call_id: int, user_ids: List[int]):
     """
@@ -133,136 +144,88 @@
     Parameters
     ----------
         - call_id: int - (required)
         - user_ids: List[int] - (required)
 
     """
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.CALLS_V1}/conference_calls/{call_id}/invite",
-        payload={
-            "call_id": call_id,
-            "user_ids[]": user_ids
-        }
+        "POST",
+        endpoint=f"{Endpoints.CALLS_V1}/conference_calls/{call_id}/invite",
+        payload={"call_id": call_id, "user_ids[]": user_ids},
     )
     self.logger.info("Invited users to call.")
     return response
 
 
-def invite_users_to_chat_call(
-        self,
-        chat_room_id: int,
-        room_id: int,
-        room_url: str
-):
+def invite_users_to_chat_call(self, chat_room_id: int, room_id: int, room_url: str):
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.CALLS_V2}/invite",
+        "POST",
+        endpoint=f"{Endpoints.CALLS_V2}/invite",
         payload={
             "chat_room_id": chat_room_id,
             "room_id": room_id,
-            "room_url": room_url
-        }
+            "room_url": room_url,
+        },
     )
     self.logger.info("Invited users to chat call.")
     return response
 
 
 def kick_and_ban_from_call(self, call_id: int, user_id: int):
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.CALLS_V1}/conference_calls/{call_id}/kick",
-        payload={"user_id": user_id}
+        "POST",
+        endpoint=f"{Endpoints.CALLS_V1}/conference_calls/{call_id}/kick",
+        payload={"user_id": user_id},
     )
     self.logger.info("User has been banned from the call.")
     return response
 
 
-def notify_anonymous_user_leave_agora_channel(self, conference_id: int, agora_uid: str):
-    response = self._make_request(
-        "POST", endpoint=f"{Endpoints.ANONYMOUS_CALLS_V1}/leave_agora_channel",
-        payload={"conference_id": conference_id, "agora_uid": agora_uid}
-    )
-    self.logger.info("Notified anonymous user left the call.")
-    return response
-
-
-def notify_user_leave_agora_channel(self, conference_id: int, user_id: int):
-    response = self._make_request(
-        "POST", endpoint=f"{Endpoints.CALLS_V1}/leave_agora_channel",
-        payload={"conference_id": conference_id, "user_id": user_id}
-    )
-    self.logger.info(f"Notified user '{user_id}' left the call.")
-    return response
-
-
-def send_call_screenshot(
-        self,
-        screenshot_filename: str,
-        conference_id: int
-):
-    response = self._make_request(
-        "PUT", endpoint=f"{Endpoints.CALLS_V1}/screenshot",
-        payload={
-            "conference_id": conference_id,
-            "screenshot_filename": screenshot_filename
-        }
-    )
-    self.logger.info("Call screenshot sent.")
-    return response
-
-
 def set_call(
-        self,
-        call_id: int,
-        joinable_by: str,
-        game_title: str = None,
-        category_id: str = None
+    self,
+    call_id: int,
+    joinable_by: str,
+    game_title: str = None,
+    category_id: str = None,
 ):
     response = self._make_request(
-        "PUT", endpoint=f"{Endpoints.CALLS_V1}/{call_id}",
+        "PUT",
+        endpoint=f"{Endpoints.CALLS_V1}/{call_id}",
         payload={
             "joinable_by": joinable_by,
             "game_title": game_title,
             "category_id": category_id,
-        }
+        },
     )
     self.logger.info("Started a call")
     return response
 
 
-def set_user_role(
-        self,
-        call_id: int,
-        user_id: int,
-        role: str
-):
+def set_user_role(self, call_id: int, user_id: int, role: str):
     response = self._make_request(
-        "PUT", endpoint=f"{Endpoints.CALLS_V1}/{call_id}/users/{user_id}",
-        payload={"role": role}
+        "PUT",
+        endpoint=f"{Endpoints.CALLS_V1}/{call_id}/users/{user_id}",
+        payload={"role": role},
     )
     self.logger.info(f"User '{user_id}' has been given a role.")
     return response
 
 
-def start_call(
-        self,
-        conference_id: int,
-        call_sid: str
-) -> ConferenceCall:
+def start_call(self, conference_id: int, call_sid: str = None) -> ConferenceCall:
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.CALLS_V1}/start_conference_call",
+        "POST",
+        endpoint=f"{Endpoints.CALLS_V1}/start_conference_call",
         payload={"conference_id": conference_id, "call_sid": call_sid},
-        data_type=ConferenceCallResponse
+        data_type=ConferenceCallResponse,
     ).conference_call
     self.logger.info("Joined the call.")
     return response
 
 
-def stop_call(
-        self,
-        conference_id: int,
-        call_sid: str
-):
+def stop_call(self, conference_id: int, call_sid: str = None):
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.CALLS_V1}/leave_conference_call",
-        payload={"conference_id": conference_id, "call_sid": call_sid}
+        "POST",
+        endpoint=f"{Endpoints.CALLS_V1}/leave_conference_call",
+        payload={"conference_id": conference_id, "call_sid": call_sid},
     )
     self.logger.info("Left the call.")
     return response
```

### Comparing `yaylib-0.1.3/yaylib/api/cassandra.py` & `yaylib-0.1.5/yaylib/api/cassandra.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,39 +13,40 @@
         - important: bool - (required)
         - from_timestamp: int - (optional)
         - number: int - (optional)
 
     """
     self._check_authorization()
     return self._make_request(
-        "GET", endpoint=f"https://{Configs.YAY_STAGING_HOST_2}/api/user_activities",
-        params=params, data_type=ActivitiesResponse
+        "GET",
+        endpoint=f"https://{Configs.YAY_STAGING_HOST_2}/api/user_activities",
+        params=params,
+        data_type=ActivitiesResponse,
     )
 
 
 def get_user_merged_activities(self, **params) -> ActivitiesResponse:
     """
     Parameters
     ----------
 
         - from_timestamp: int - (optional)
         - number: int - (optional)
 
     """
     self._check_authorization()
     return self._make_request(
-        "GET", endpoint=f"https://{Configs.YAY_STAGING_HOST_2}/api/v2/user_activities",
-        params=params, data_type=ActivitiesResponse
+        "GET",
+        endpoint=f"https://{Configs.YAY_STAGING_HOST_2}/api/v2/user_activities",
+        params=params,
+        data_type=ActivitiesResponse,
     )
 
 
 def received_notification(self, pid: str, type: str, opened_at: int = None):
     # TODO: opened_atはnullalbeか確認する
     self._check_authorization()
     return self._make_request(
-        "POST", endpoint=f"{self.host}/api/received_push_notifications",
-        payload={
-            "pid": pid,
-            "type": type,
-            "opened_at": opened_at
-        }
+        "POST",
+        endpoint=f"{self.host}/api/received_push_notifications",
+        payload={"pid": pid, "type": type, "opened_at": opened_at},
     )
```

### Comparing `yaylib-0.1.3/yaylib/api/chat.py` & `yaylib-0.1.5/yaylib/api/chat.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,125 +7,131 @@
 from ..responses import *
 from ..utils import *
 
 
 def accept_chat_request(self, chat_room_ids: List[int]):
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V1}/accept_chat_request",
-        payload={"chat_room_ids[]": chat_room_ids}
+        "POST",
+        endpoint=f"{Endpoints.CHAT_ROOMS_V1}/accept_chat_request",
+        payload={"chat_room_ids[]": chat_room_ids},
     )
     self.logger.info("Accepted chat requests")
     return response
 
 
 def check_unread_status(self, from_time: int) -> UnreadStatusResponse:
     self._check_authorization()
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.CHAT_ROOMS_V1}/unread_status",
+        "GET",
+        endpoint=f"{Endpoints.CHAT_ROOMS_V1}/unread_status",
         params={"from_time": from_time},
-        data_type=UnreadStatusResponse
+        data_type=UnreadStatusResponse,
     )
 
 
 def create_group_chat(
-        self,
-        name: str,
-        with_user_ids: List[int],
-        icon_filename: str = None,
-        background_filename: str = None
+    self,
+    name: str,
+    with_user_ids: List[int],
+    icon_filename: str = None,
+    background_filename: str = None,
 ) -> CreateChatRoomResponse:
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V3}/new",
+        "POST",
+        endpoint=f"{Endpoints.CHAT_ROOMS_V3}/new",
         payload={
             "name": name,
             "with_user_ids[]": with_user_ids,
             "icon_filename": icon_filename,
             "background_filename": background_filename,
         },
-        data_type=CreateChatRoomResponse
+        data_type=CreateChatRoomResponse,
     )
     self.logger.info(f"Group chat '{name}' has been created.")
     return response
 
 
 def create_private_chat(
-        self,
-        with_user_id: int,
-        matching_id: int = None,
-        hima_chat: bool = False
+    self, with_user_id: int, matching_id: int = None, hima_chat: bool = False
 ) -> CreateChatRoomResponse:
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V1}/new",
+        "POST",
+        endpoint=f"{Endpoints.CHAT_ROOMS_V1}/new",
         payload={
             "with_user_id": with_user_id,
             "matching_id": matching_id,
             "hima_chat": hima_chat,
         },
-        data_type=CreateChatRoomResponse
+        data_type=CreateChatRoomResponse,
     )
     self.logger.info(f"Created a private chatroom with '{with_user_id}'.")
     return response
 
 
 def delete_background(self, room_id: int):
     self._check_authorization()
     response = self._make_request(
-        "DELETE", endpoint=f"{Endpoints.CHAT_ROOMS_V2}/{room_id}/background",
+        "DELETE",
+        endpoint=f"{Endpoints.CHAT_ROOMS_V2}/{room_id}/background",
     )
     self.logger.info("Background image of the chatroom has been deleted.")
     return response
 
 
 def delete_message(self, room_id: int, message_id: int):
     self._check_authorization()
     response = self._make_request(
-        "DELETE", endpoint=f"{Endpoints.CHAT_ROOMS_V1}/{room_id}/messages/{message_id}/delete",
+        "DELETE",
+        endpoint=f"{Endpoints.CHAT_ROOMS_V1}/{room_id}/messages/{message_id}/delete",
     )
     self.logger.info("Message has been deleted.")
     return response
 
 
 def edit_chat_room(
-        self,
-        chat_room_id: int,
-        name: str,
-        icon_filename: str = None,
-        background_filename: str = None
+    self,
+    chat_room_id: int,
+    name: str,
+    icon_filename: str = None,
+    background_filename: str = None,
 ):
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V1}/{chat_room_id}/edit",
+        "POST",
+        endpoint=f"{Endpoints.CHAT_ROOMS_V1}/{chat_room_id}/edit",
         payload={
             "name": name,
             "icon_filename": icon_filename,
             "background_filename": background_filename,
-        }
+        },
     )
     self.logger.info("Chatroom has been updated.")
     return response
 
 
 def get_chatable_users(
-        self,
-        # @Body @Nullable SearchUsersRequest searchUsersRequest
-        from_follow_id: int = None,
-        from_timestamp: int = None,
-        order_by: str = None
+    self,
+    # @Body @Nullable SearchUsersRequest searchUsersRequest
+    from_follow_id: int = None,
+    from_timestamp: int = None,
+    order_by: str = None,
 ) -> FollowUsersResponse:
     self._check_authorization()
     return self._make_request(
-        "POST", endpoint=f"{Endpoints.USERS_V1}/followings/chatable",
+        "POST",
+        endpoint=f"{Endpoints.USERS_V1}/followings/chatable",
         payload={
             "from_follow_id": from_follow_id,
             "from_timestamp": from_timestamp,
             "order_by": order_by,
-        }, data_type=FollowUsersResponse
+        },
+        data_type=FollowUsersResponse,
     )
 
 
 def get_gifs_data(self) -> List[GifImageCategory]:
     self._check_authorization()
     return self._make_request(
         "GET", endpoint=f"{Endpoints.HIDDEN_V1}/chats", data_type=GifsDataResponse
@@ -140,112 +146,116 @@
 
         - from_timestamp: int - (optional)
         - number: int - (optional)
 
     """
     self._check_authorization()
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.HIDDEN_V1}/chats",
-        params=params, data_type=ChatRoomsResponse
+        "GET",
+        endpoint=f"{Endpoints.HIDDEN_V1}/chats",
+        params=params,
+        data_type=ChatRoomsResponse,
     )
 
 
 def get_main_chat_rooms(self, from_timestamp: int = None) -> ChatRoomsResponse:
     self._check_authorization()
     params = {}
     if from_timestamp:
         params["from_timestamp"] = from_timestamp
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.CHAT_ROOMS_V1}/main_list",
-        params=params, data_type=ChatRoomsResponse
+        "GET",
+        endpoint=f"{Endpoints.CHAT_ROOMS_V1}/main_list",
+        params=params,
+        data_type=ChatRoomsResponse,
     )
 
 
 def get_messages(self, chat_room_id: int, **params) -> List[Message]:
     """
 
     Parameters:
     ---------------
         - from_message_id: int - (optional)
         - to_message_id: int - (optional)
 
     """
     self._check_authorization()
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.CHAT_ROOMS_V2}/{chat_room_id}/messages",
-        params=params, data_type=MessagesResponse
+        "GET",
+        endpoint=f"{Endpoints.CHAT_ROOMS_V2}/{chat_room_id}/messages",
+        params=params,
+        data_type=MessagesResponse,
     ).messages
 
 
-# def get_chat_room_notification_settings(self, room_id: int) -> Settings:
-#     self._check_authorization()
-#     return self._make_request(
-#         "GET", endpoint=f"{Endpoints.NOTIFICATION_SETTINGS_V2}/chat_rooms/{room_id}",
-#         data_type=AdditionalSettingsResponse
-#     ).settings
-
-
 def get_request_chat_rooms(self, from_timestamp: int = None) -> ChatRoomsResponse:
     self._check_authorization()
     params = {}
     if from_timestamp:
         params["from_timestamp"] = from_timestamp
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.CHAT_ROOMS_V1}/request_list",
-        params=params, data_type=ChatRoomsResponse
+        "GET",
+        endpoint=f"{Endpoints.CHAT_ROOMS_V1}/request_list",
+        params=params,
+        data_type=ChatRoomsResponse,
     )
 
 
 def get_chat_room(self, chat_room_id: int) -> ChatRoom:
     self._check_authorization()
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.CHAT_ROOMS_V2}/{chat_room_id}",
-        data_type=ChatRoomResponse
+        "GET",
+        endpoint=f"{Endpoints.CHAT_ROOMS_V2}/{chat_room_id}",
+        data_type=ChatRoomResponse,
     ).chat
 
 
 def get_sticker_packs(self) -> List[StickerPack]:
     return self._make_request(
-        "GET", endpoint=Endpoints.STICKER_PACKS_V2,
-        data_type=StickerPacksResponse
+        "GET", endpoint=Endpoints.STICKER_PACKS_V2, data_type=StickerPacksResponse
     ).sticker_packs
 
 
 def get_total_chat_requests(self) -> int:
     self._check_authorization()
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.CHAT_ROOMS_V1}/total_chat_request",
-        data_type=TotalChatRequestResponse
+        "GET",
+        endpoint=f"{Endpoints.CHAT_ROOMS_V1}/total_chat_request",
+        data_type=TotalChatRequestResponse,
     ).total
 
 
 def hide_chat(self, chat_room_id: int):
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.HIDDEN_V1}/chats",
+        "POST",
+        endpoint=f"{Endpoints.HIDDEN_V1}/chats",
         payload={"chat_room_id": chat_room_id},
     )
     self.logger.info(f"Chatroom '{chat_room_id}' has been hidden.")
     return response
 
 
 def invite_to_chat(self, chat_room_id: int, user_ids: List[int]):
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V2}/{chat_room_id}/invite",
+        "POST",
+        endpoint=f"{Endpoints.CHAT_ROOMS_V2}/{chat_room_id}/invite",
         payload={"with_user_ids[]": user_ids},
     )
     self.logger.info("Invited users to the chatroom.")
     return response
 
 
 def kick_users_from_chat(self, chat_room_id: int, user_ids: List[int]):
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V2}/{chat_room_id}/kick",
+        "POST",
+        endpoint=f"{Endpoints.CHAT_ROOMS_V2}/{chat_room_id}/kick",
         payload={"with_user_ids[]": user_ids},
     )
     self.logger.info(f"Users have been kicked from the chatroom.")
     return response
 
 
 def pin_chat(self, room_id: int):
@@ -253,89 +263,63 @@
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V1}/{room_id}/pinned"
     )
     self.logger.info("Pinned the chatroom.")
     return response
 
 
-def read_attachment(
-        self,
-        room_id: int,
-        attachment_msg_ids: List[int]
-):
-    # TODO: check if this works
-    self._check_authorization()
-    response = self._make_request(
-        "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V1}/{room_id}/attachments_read",
-        payload={
-            "attachment_msg_ids[]": attachment_msg_ids
-        }
-    )
-    self.logger.info("Attachment has been read.")
-    return response
-
-
 def read_message(self, chat_room_id: int, message_id: int):
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V2}/{chat_room_id}/messages/{message_id}/read",
+        "POST",
+        endpoint=f"{Endpoints.CHAT_ROOMS_V2}/{chat_room_id}/messages/{message_id}/read",
     )
     self.logger.info("Message has been read.")
     return response
 
 
-def read_video_message(
-        self,
-        room_id: int,
-        video_msg_ids: List[int]
-):
-    self._check_authorization()
-    response = self._make_request(
-        "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V1}/{room_id}/videos_read",
-        payload={"video_msg_ids": video_msg_ids},
-    )
-    self.logger.info("Video message has been read.")
-    return response
-
-
 def refresh_chat_rooms(self, from_time: int = None) -> ChatRoomsResponse:
     self._check_authorization()
     params = {}
     if from_time:
         params["from_time"] = from_time
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.CHAT_ROOMS_V2}/update",
-        params=params, data_type=ChatRoomsResponse
+        "GET",
+        endpoint=f"{Endpoints.CHAT_ROOMS_V2}/update",
+        params=params,
+        data_type=ChatRoomsResponse,
     )
 
 
 def remove_chat_rooms(self, chat_room_ids: List[int]):
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V2}/mass_destroy",
+        "POST",
+        endpoint=f"{Endpoints.CHAT_ROOMS_V2}/mass_destroy",
         payload={"chat_room_ids[]": chat_room_ids},
     )
     self.logger.info(f"Chatrooms have been removed.")
     return response
 
 
 def report_chat_room(
-        self,
-        chat_room_id: int,
-        opponent_id: int,
-        category_id: int,
-        reason: str = None,
-        screenshot_filename: str = None,
-        screenshot_2_filename: str = None,
-        screenshot_3_filename: str = None,
-        screenshot_4_filename: str = None
+    self,
+    chat_room_id: int,
+    opponent_id: int,
+    category_id: int,
+    reason: str = None,
+    screenshot_filename: str = None,
+    screenshot_2_filename: str = None,
+    screenshot_3_filename: str = None,
+    screenshot_4_filename: str = None,
 ):
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V3}/{chat_room_id}/report",
+        "POST",
+        endpoint=f"{Endpoints.CHAT_ROOMS_V3}/{chat_room_id}/report",
         payload={
             "chat_room_id": chat_room_id,
             "opponent_id": opponent_id,
             "category_id": category_id,
             "reason": reason,
             "screenshot_filename": screenshot_filename,
             "screenshot_2_filename": screenshot_2_filename,
@@ -343,67 +327,52 @@
             "screenshot_4_filename": screenshot_4_filename,
         },
     )
     self.logger.info(f"Chatroom '{chat_room_id}' has been reported.")
     return response
 
 
-def send_media_screenshot_notification(self, room_id: int):
-    self._check_authorization()
-    response = self._make_request(
-        "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V1}/{room_id}/screen_captured"
-    )
-    self.logger.info("Media screenshot notification has been sent.")
-    return response
-
-
 def send_message(
-        self,
-        chat_room_id: int,
-        message_type: str,
-        call_type: str = None,
-        text: str = None,
-        font_size: int = None,
-        gif_image_id: int = None,
-        attachment_file_name: str = None,
-        sticker_pack_id: int = None,
-        video_file_name: str = None
+    self,
+    chat_room_id: int,
+    message_type: str,
+    call_type: str = None,
+    text: str = None,
+    font_size: int = None,
+    gif_image_id: int = None,
+    attachment_file_name: str = None,
+    sticker_pack_id: int = None,
+    video_file_name: str = None,
 ) -> MessageResponse:
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V3}/{chat_room_id}/messages/new",
+        "POST",
+        endpoint=f"{Endpoints.CHAT_ROOMS_V3}/{chat_room_id}/messages/new",
         payload={
             "chat_room_id": chat_room_id,
             "message_type": message_type,
             "call_type": call_type,
             "text": text,
             "font_size": font_size,
             "gif_image_id": gif_image_id,
             "attachment_file_name": attachment_file_name,
             "sticker_pack_id": sticker_pack_id,
             "video_file_name": video_file_name,
-        }, data_type=MessageResponse
+        },
+        data_type=MessageResponse,
     )
     self.logger.info("Your message has been sent.")
     return response
 
 
-def set_notification_settings(
-        self,
-        chat_room_id: int,
-        notification_chat: int
-) -> Settings:
-    # NotificationSettingResponse
-    pass
-
-
 def unhide_chat(self, chat_room_ids: int):
     self._check_authorization()
     response = self._make_request(
-        "DELETE", endpoint=f"{Endpoints.HIDDEN_V1}/chats",
+        "DELETE",
+        endpoint=f"{Endpoints.HIDDEN_V1}/chats",
         params={"chat_room_ids[]": chat_room_ids},
     )
     self.logger.info("Unhid the chatrooms")
     return response
 
 
 def unpin_chat(self, chat_room_id: int):
```

### Comparing `yaylib-0.1.3/yaylib/api/group.py` & `yaylib-0.1.5/yaylib/api/group.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,18 +32,24 @@
         "POST", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/accept/{user_id}"
     )
     self.logger.info("Accepted the group join request.")
     return response
 
 
 def add_related_groups(self, group_id: int, related_group_id: List[int]):
+    """
+
+    関連サークルを追加する
+
+    """
     self._check_authorization()
     response = self._make_request(
-        "PUT", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/related",
-        params={"related_group_id[]": related_group_id}
+        "PUT",
+        endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/related",
+        params={"related_group_id[]": related_group_id},
     )
     self.logger.info("Group has been added to the related groups")
     return response
 
 
 def ban_group_user(self, group_id: int, user_id: int):
     self._check_authorization()
@@ -56,45 +62,48 @@
 
 def check_unread_status(self, from_time: int = None) -> UnreadStatusResponse:
     self._check_authorization()
     params = {}
     if from_time:
         params["from_time"] = from_time
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.GROUPS_V1}/unread_status",
-        params=params, data_type=UnreadStatusResponse
+        "GET",
+        endpoint=f"{Endpoints.GROUPS_V1}/unread_status",
+        params=params,
+        data_type=UnreadStatusResponse,
     )
 
 
 def create_group(
-        self,
-        topic: str,
-        description: str = None,
-        secret: bool = None,
-        hide_reported_posts: bool = None,
-        hide_conference_call: bool = None,
-        is_private: bool = None,
-        only_verified_age: bool = None,
-        only_mobile_verified: bool = None,
-        call_timeline_display: bool = None,
-        allow_ownership_transfer: bool = None,
-        allow_thread_creation_by: str = None,
-        gender: int = None,
-        generation_groups_limit: int = None,
-        group_category_id: int = None,
-        cover_image_filename: str = None,
-        sub_category_id: str = None,
-        hide_from_game_eight: bool = None,
-        allow_members_to_post_media: bool = None,
-        allow_members_to_post_url: bool = None,
-        guidelines: str = None,
+    self,
+    topic: str,
+    description: str = None,
+    secret: bool = None,
+    hide_reported_posts: bool = None,
+    hide_conference_call: bool = None,
+    is_private: bool = None,
+    only_verified_age: bool = None,
+    only_mobile_verified: bool = None,
+    call_timeline_display: bool = None,
+    allow_ownership_transfer: bool = None,
+    allow_thread_creation_by: str = None,
+    gender: int = None,
+    generation_groups_limit: int = None,
+    group_category_id: int = None,
+    cover_image_filename: str = None,
+    sub_category_id: str = None,
+    hide_from_game_eight: bool = None,
+    allow_members_to_post_media: bool = None,
+    allow_members_to_post_url: bool = None,
+    guidelines: str = None,
 ) -> CreateGroupResponse:
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.GROUPS_V3}/new",
+        "POST",
+        endpoint=f"{Endpoints.GROUPS_V3}/new",
         payload={
             "topic": topic,
             "description": description,
             "secret": secret,
             "hide_reported_posts": hide_reported_posts,
             "hide_conference_call": hide_conference_call,
             "is_private": is_private,
@@ -107,33 +116,32 @@
             "generation_groups_limit": generation_groups_limit,
             "group_category_id": group_category_id,
             "cover_image_filename": cover_image_filename,
             "uuid": self.uuid,
             "api_key": self.api_key,
             "timestamp": int(datetime.now().timestamp()),
             "signed_info": signed_info_calculating(
-                self.api_key, self.device_uuid,
-                int(datetime.now().timestamp())
+                self.api_key, self.device_uuid, int(datetime.now().timestamp())
             ),
             "sub_category_id": sub_category_id,
             "hide_from_game_eight": hide_from_game_eight,
             "allow_members_to_post_image_and_video": allow_members_to_post_media,
             "allow_members_to_post_url": allow_members_to_post_url,
             "guidelines": guidelines,
-        }, data_type=CreateGroupResponse
+        },
+        data_type=CreateGroupResponse,
     )
     self.logger.info("Group has been created.")
     return response
 
 
 def create_pin_group(self, group_id: int):
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.PINNED_V1}/groups",
-        payload={"id": group_id}
+        "POST", endpoint=f"{Endpoints.PINNED_V1}/groups", payload={"id": group_id}
     )
     self.logger.info("Pinned the group.")
     return response
 
 
 def decline_moderator_offer(self, group_id: int):
     self._check_authorization()
@@ -173,98 +181,99 @@
 
 def get_banned_group_members(self, group_id: int, page: int = None) -> UsersResponse:
     self._check_authorization()
     params = {}
     if page:
         params["page"] = page
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/ban_list",
-        params=params
+        "GET", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/ban_list", params=params
     )
 
 
 def get_group_categories(self, **params) -> GroupCategoriesResponse:
     """
 
     Parameters:
     ----------
 
         - page: int - (optional)
         - number: int - (optional)
 
     """
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.GROUPS_V1}/categories",
-        params=params, data_type=GroupCategoriesResponse
+        "GET",
+        endpoint=f"{Endpoints.GROUPS_V1}/categories",
+        params=params,
+        data_type=GroupCategoriesResponse,
     )
 
 
 def get_create_group_quota(self) -> CreateGroupQuota:
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.GROUPS_V1}/created_quota",
-        data_type=CreateGroupQuota
+        "GET",
+        endpoint=f"{Endpoints.GROUPS_V1}/created_quota",
+        data_type=CreateGroupQuota,
     ).create
 
 
 def get_group(self, group_id: int) -> GroupResponse:
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}",
-        data_type=GroupResponse
+        "GET", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}", data_type=GroupResponse
     )
 
 
-def get_group_notification_settings(self, group_id: int) -> GroupNotificationSettingsResponse:
-    pass
-
-
 def get_groups(self, **params) -> GroupsResponse:
     """
 
     Parameters:
     ----------
 
         - group_category_id: int = None
         - keyword: str = None
         - from_timestamp: int = None
         - sub_category_id: int = None
 
     """
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.GROUPS_V2}",
-        params=params, data_type=GroupsResponse
+        "GET",
+        endpoint=f"{Endpoints.GROUPS_V2}",
+        params=params,
+        data_type=GroupsResponse,
     )
 
 
 def get_invitable_users(self, group_id: int, **params) -> UsersByTimestampResponse:
     """
 
     Parameters:
     ----------
 
         - from_timestamp: int - (optional)
         - user[nickname]: str - (optional)
 
     """
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/users/invitable",
-        params=params, data_type=UsersByTimestampResponse
+        "GET",
+        endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/users/invitable",
+        params=params,
+        data_type=UsersByTimestampResponse,
     )
 
 
 def get_joined_statuses(self, ids: List[int]) -> dict:
     self._check_authorization()
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.GROUPS_V1}/joined_statuses",
-        params={"ids[]": ids}
+        "GET", endpoint=f"{Endpoints.GROUPS_V1}/joined_statuses", params={"ids[]": ids}
     )
 
 
 def get_group_member(self, group_id: int, user_id: int) -> GroupUserResponse:
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/members/{user_id}",
+        "GET",
+        endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/members/{user_id}",
     )
 
 
 def get_group_members(self, group_id: int, **params) -> GroupUsersResponse:
     """
 
     Parameters:
@@ -276,27 +285,31 @@
         - from_id: int - (optional)
         - from_timestamp: int - (optional)
         - order_by: str - (optional)
         - followed_by_me: bool - (optional)
 
     """
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.GROUPS_V2}/{group_id}/members",
-        params=params, data_type=GroupUsersResponse
+        "GET",
+        endpoint=f"{Endpoints.GROUPS_V2}/{group_id}/members",
+        params=params,
+        data_type=GroupUsersResponse,
     )
 
 
 def get_my_groups(self, from_timestamp: None) -> GroupsResponse:
     self._check_authorization()
     params = {}
     if from_timestamp:
         params["from_timestamp"] = from_timestamp
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.GROUPS_V2}/mine",
-        params=params, data_type=GroupsResponse
+        "GET",
+        endpoint=f"{Endpoints.GROUPS_V2}/mine",
+        params=params,
+        data_type=GroupsResponse,
     )
 
 
 def get_relatable_groups(self, group_id: int, **params) -> GroupsRelatedResponse:
     """
 
     Parameters:
@@ -304,16 +317,18 @@
 
         - group_id: int - (required)
         - keyword: str - (optional)
         - from: str - (optional)
 
     """
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/relatable",
-        params=params, data_type=GroupsRelatedResponse
+        "GET",
+        endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/relatable",
+        params=params,
+        data_type=GroupsRelatedResponse,
     )
 
 
 def get_related_groups(self, group_id: int, **params) -> GroupsRelatedResponse:
     """
 
     Parameters:
@@ -321,229 +336,238 @@
 
         - group_id: int - (required)
         - keyword: str - (optional)
         - from: str - (optional)
 
     """
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/related",
-        params=params, data_type=GroupsRelatedResponse
+        "GET",
+        endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/related",
+        params=params,
+        data_type=GroupsRelatedResponse,
     )
 
 
 def get_user_groups(self, **params) -> GroupsResponse:
     """
 
     Parameters:
     ----------
 
         - user_id: int - (required)
         - page: int - (optional)
 
     """
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.GROUPS_V1}/user_group_list",
-        params=params, data_type=GroupsResponse
+        "GET",
+        endpoint=f"{Endpoints.GROUPS_V1}/user_group_list",
+        params=params,
+        data_type=GroupsResponse,
     )
 
 
 def invite_users_to_group(self, group_id: int, user_ids: List[int]):
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/invite",
-        payload={"user_ids[]": user_ids}
+        "POST",
+        endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/invite",
+        payload={"user_ids[]": user_ids},
     )
     self.logger.info("Invited users to the group.")
     return response
 
 
 def join_group(self, group_id: int):
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/join",
+        "POST",
+        endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/join",
     )
     self.logger.info("You are now one of the members of the group.")
     return response
 
 
 def leave_group(self, group_id: int):
     self._check_authorization()
     response = self._make_request(
-        "DELETE", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/leave",
+        "DELETE",
+        endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/leave",
     )
     self.logger.info("Left the group.")
     return response
 
 
 def post_gruop_social_shared(self, group_id: int, sns_name: str):
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.GROUPS_V2}/{group_id}/social_shared",
-        params={"sns_name": sns_name}
+        "POST",
+        endpoint=f"{Endpoints.GROUPS_V2}/{group_id}/social_shared",
+        params={"sns_name": sns_name},
     )
     self.logger.info("Group social shared has been posted.")
     return response
 
 
 def remove_group_cover(self, group_id: int):
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/remove_cover",
+        "POST",
+        endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/remove_cover",
     )
     self.logger.info("Group cover image has been removed.")
     return response
 
 
 def remove_moderator(self, group_id: int, user_id: int):
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/fire/{user_id}",
+        "POST",
+        endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/fire/{user_id}",
     )
     self.logger.info(f"Group moderator '{user_id}' has been removed.")
     return response
 
 
 def remove_related_groups(self, group_id: int, related_group_ids: List[int]):
     self._check_authorization()
     response = self._make_request(
-        "DELETE", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/related",
-        params={"related_group_id[]": related_group_ids}
+        "DELETE",
+        endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/related",
+        params={"related_group_id[]": related_group_ids},
     )
     self.logger.info("Related groups have been removed.")
     return response
 
 
 def report_group(
-        self,
-        group_id: int,
-        category_id: int,
-        reason: str = None,
-        opponent_id: int = None,
-        screenshot_filename: str = None,
-        screenshot_2_filename: str = None,
-        screenshot_3_filename: str = None,
-        screenshot_4_filename: str = None,
+    self,
+    group_id: int,
+    category_id: int,
+    reason: str = None,
+    opponent_id: int = None,
+    screenshot_filename: str = None,
+    screenshot_2_filename: str = None,
+    screenshot_3_filename: str = None,
+    screenshot_4_filename: str = None,
 ):
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.GROUPS_V3}/{group_id}/report",
+        "POST",
+        endpoint=f"{Endpoints.GROUPS_V3}/{group_id}/report",
         payload={
             "category_id": category_id,
             "reason": reason,
             "opponent_id": opponent_id,
             "screenshot_filename": screenshot_filename,
             "screenshot_2_filename": screenshot_2_filename,
             "screenshot_3_filename": screenshot_3_filename,
-            "screenshot_4_filename": screenshot_4_filename
-        }
+            "screenshot_4_filename": screenshot_4_filename,
+        },
     )
     self.logger.info("Group has been reported.")
     return response
 
 
 def send_moderator_offers(self, group_id: int, user_ids: List[int]):
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.GROUPS_V3}/{group_id}/deputize/mass",
+        "POST",
+        endpoint=f"{Endpoints.GROUPS_V3}/{group_id}/deputize/mass",
         payload={
-            "user_ids[]": user_ids, "uuid": self.uuid,
-            "api_key": self.api_key, "timestamp": int(datetime.now().timestamp()),
+            "user_ids[]": user_ids,
+            "uuid": self.uuid,
+            "api_key": self.api_key,
+            "timestamp": int(datetime.now().timestamp()),
             "signed_info": signed_info_calculating(
-                self.api_key, self.device_uuid,
-                int(datetime.now().timestamp())
+                self.api_key, self.device_uuid, int(datetime.now().timestamp())
             ),
-        }
+        },
     )
     self.logger.info("Offered users to become a group moderator.")
     return response
 
 
 def send_ownership_offer(self, group_id: int, user_id: int):
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.GROUPS_V3}/{group_id}/transfer",
+        "POST",
+        endpoint=f"{Endpoints.GROUPS_V3}/{group_id}/transfer",
         payload={
-            "user_id": user_id, "uuid": self.uuid,
-            "api_key": self.api_key, "timestamp": int(datetime.now().timestamp()),
+            "user_id": user_id,
+            "uuid": self.uuid,
+            "api_key": self.api_key,
+            "timestamp": int(datetime.now().timestamp()),
             "signed_info": signed_info_calculating(
-                self.api_key, self.device_uuid,
-                int(datetime.now().timestamp())
+                self.api_key, self.device_uuid, int(datetime.now().timestamp())
             ),
-        }
+        },
     )
     self.logger.info("Offered user to become a group owner.")
     return response
 
 
-def set_group_notification_settings(
-        self,
-        group_id: int,
-        notification_group_post: int = None,
-        notification_group_join: int = None,
-        notification_group_request: int = None,
-        notification_group_message_tag_all: int = None,
-) -> AdditionalSettingsResponse:
-    pass
-
-
 def set_group_title(self, group_id: int, title: str):
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/set_title",
-        payload={"title": title}
+        "POST",
+        endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/set_title",
+        payload={"title": title},
     )
     self.logger.info("Group tittle has been set.")
     return response
 
 
 def take_over_group_ownership(self, group_id: int):
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/take_over",
+        "POST",
+        endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/take_over",
     )
     self.logger.info(f"Took over the group ownership of {group_id}")
     return response
 
 
 def unban_group_member(self, group_id: int, user_id: int):
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/unban/{user_id}",
+        "POST",
+        endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/unban/{user_id}",
     )
     self.logger.info("User has been banned from the group.")
     return response
 
 
 def update_group(
-        self,
-        group_id: int,
-        topic: str,
-        description: str = None,
-        secret: bool = None,
-        hide_reported_posts: bool = None,
-        hide_conference_call: bool = None,
-        is_private: bool = None,
-        only_verified_age: bool = None,
-        only_mobile_verified: bool = None,
-        call_timeline_display: bool = None,
-        allow_ownership_transfer: bool = None,
-        allow_thread_creation_by: str = None,
-        gender: int = None,
-        generation_groups_limit: int = None,
-        group_category_id: int = None,
-        cover_image_filename: str = None,
-        sub_category_id: str = None,
-        hide_from_game_eight: bool = None,
-        allow_members_to_post_media: bool = None,
-        allow_members_to_post_url: bool = None,
-        guidelines: str = None,
+    self,
+    group_id: int,
+    topic: str,
+    description: str = None,
+    secret: bool = None,
+    hide_reported_posts: bool = None,
+    hide_conference_call: bool = None,
+    is_private: bool = None,
+    only_verified_age: bool = None,
+    only_mobile_verified: bool = None,
+    call_timeline_display: bool = None,
+    allow_ownership_transfer: bool = None,
+    allow_thread_creation_by: str = None,
+    gender: int = None,
+    generation_groups_limit: int = None,
+    group_category_id: int = None,
+    cover_image_filename: str = None,
+    sub_category_id: str = None,
+    hide_from_game_eight: bool = None,
+    allow_members_to_post_media: bool = None,
+    allow_members_to_post_url: bool = None,
+    guidelines: str = None,
 ) -> GroupResponse:
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.GROUPS_V3}/{group_id}/update",
+        "POST",
+        endpoint=f"{Endpoints.GROUPS_V3}/{group_id}/update",
         payload={
             "topic": topic,
             "description": description,
             "secret": secret,
             "hide_reported_posts": hide_reported_posts,
             "hide_conference_call": hide_conference_call,
             "is_private": is_private,
@@ -557,45 +581,39 @@
             "group_category_id": group_category_id,
             "cover_image_filename": cover_image_filename,
             "sub_category_id": sub_category_id,
             "uuid": self.uuid,
             "api_key": self.api_key,
             "timestamp": int(datetime.now().timestamp()),
             "signed_info": signed_info_calculating(
-                self.api_key, self.device_uuid,
-                int(datetime.now().timestamp())
+                self.api_key, self.device_uuid, int(datetime.now().timestamp())
             ),
             "hide_from_game_eight": hide_from_game_eight,
             "allow_members_to_post_image_and_video": allow_members_to_post_media,
             "allow_members_to_post_url": allow_members_to_post_url,
             "guidelines": guidelines,
-        }, data_type=GroupResponse
+        },
+        data_type=GroupResponse,
     )
     self.logger.info("Group details have been updated.")
     return response
 
 
-def visit_group(self, group_id: int):
-    response = self._make_request(
-        "POST", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/visit",
-    )
-    self.logger.info("Visited the group.")
-    return response
-
-
 def withdraw_moderator_offer(self, group_id: int, user_id: int):
     self._check_authorization()
     response = self._make_request(
-        "PUT", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/deputize/{user_id}/withdraw",
+        "PUT",
+        endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/deputize/{user_id}/withdraw",
     )
     self.logger.info("Group moderator offer has been withdrawn")
     return response
 
 
 def withdraw_ownership_offer(self, group_id: int, user_id: int):
     self._check_authorization()
     response = self._make_request(
-        "PUT", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/transfer/withdraw",
-        payload={"user_id": user_id}
+        "PUT",
+        endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/transfer/withdraw",
+        payload={"user_id": user_id},
     )
     self.logger.info("Group ownership offer has been withdrawn")
     return response
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `yaylib-0.1.3/yaylib/api/misc.py` & `yaylib-0.1.5/yaylib/api/misc.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,126 +27,100 @@
     ----------
 
         - resource_type: str - (Required)
         - resource_id: int - (Required)
 
     """
     response = self._make_request(
-        "GET", endpoint=f"{Endpoints.SNS_THUMBNAIL_V1}/generate",
-        params=params
+        "GET", endpoint=f"{Endpoints.SNS_THUMBNAIL_V1}/generate", params=params
     )
     self.logger.info("SNS thumbnail generated.")
     return response
 
 
 def get_email_grant_token(self, code: int, email: str) -> EmailGrantTokenResponse:
     return self._make_request(
-        "POST", endpoint=f"{Endpoints.GET_EMAIL_GRANT_TOKEN}",
+        "POST",
+        endpoint=f"{Endpoints.GET_EMAIL_GRANT_TOKEN}",
         payload={"code": code, "email": email},
-        data_type=EmailGrantTokenResponse
+        data_type=EmailGrantTokenResponse,
     ).email_grant_token
 
 
-def get_email_verification_presigned_url(self, email: str, locale: str, intent: str = None) -> str:
+def get_email_verification_presigned_url(
+    self, email: str, locale: str, intent: str = None
+) -> str:
     return self._make_request(
-        "POST", endpoint=f"{Endpoints.EMAIL_VERIFICATION_URL_V1}",
+        "POST",
+        endpoint=f"{Endpoints.EMAIL_VERIFICATION_URL_V1}",
         payload={
             "device_uuid": self.device_uuid,
             "email": email,
             "locale": locale,
-            "intent": intent
-        }, data_type=EmailVerificationPresignedUrlResponse
+            "intent": intent,
+        },
+        data_type=EmailVerificationPresignedUrlResponse,
     ).url
 
 
 def get_file_upload_presigned_urls(self, file_names: List[str]) -> List[PresignedUrl]:
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.BUCKETS_V1}/presigned_urls",
-        params={"file_names[]": file_names}, data_type=PresignedUrlsResponse
+        "GET",
+        endpoint=f"{Endpoints.BUCKETS_V1}/presigned_urls",
+        params={"file_names[]": file_names},
+        data_type=PresignedUrlsResponse,
     ).presigned_urls
 
 
-def get_id_checker_presigned_url(
-        self,
-        model: str,
-        action: str,
-        **params
-) -> str:
+def get_id_checker_presigned_url(self, model: str, action: str, **params) -> str:
     # TODO: @QueryMap @NotNull Map<String, String> map
     """
     Meow..
     """
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.ID_CHECK_V1}/{model}/{action}",
-        params=params, data_type=IdCheckerPresignedUrlResponse
+        "GET",
+        endpoint=f"{Endpoints.ID_CHECK_V1}/{model}/{action}",
+        params=params,
+        data_type=IdCheckerPresignedUrlResponse,
     ).presigned_url
 
 
 def get_old_file_upload_presigned_url(self, video_file_name: str) -> str:
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V1}/presigned_url",
-        params={"video_file_name": video_file_name}, data_type=PresignedUrlResponse
+        "GET",
+        endpoint=f"{Endpoints.USERS_V1}/presigned_url",
+        params={"video_file_name": video_file_name},
+        data_type=PresignedUrlResponse,
     ).presigned_url
 
 
-def get_policy_agreements(self) -> PolicyAgreementsResponse:
-    return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V1}/policy_agreements",
-        data_type=PolicyAgreementsResponse
-    )
-
-
-def get_promotions(self, **params) -> List[Promotion]:
-    """
-
-    Parameters:
-    ----------
-
-        - page: int - (Optional)
-        - number: int - (Optional)
-
-    """
-    return self._make_request(
-        "GET", endpoint=f"{Endpoints.PROMOTIONS_V1}",
-        params=params, data_type=PromotionsResponse
-    ).promotions
-
-
-def get_vip_game_reward_url(self, device_type: str) -> str:
-    # TODO: device_type
-    return self._make_request(
-        "GET", endpoint=f"{Endpoints.SKYFALL_V1}/url",
-        params={"device_type": device_type}, data_type=VipGameRewardUrlResponse
-    ).url
-
-
-def get_web_socket_token(self) -> str:
+def get_web_socket_token(self, headers: dict = None) -> str:
     self._check_authorization()
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V1}/ws_token",
-        data_type=WebSocketTokenResponse
+        "GET",
+        endpoint=f"{Endpoints.USERS_V1}/ws_token",
+        data_type=WebSocketTokenResponse,
+        headers=headers,
     ).token
 
 
 def verify_device(
-        self,
-        app_version: str,
-        device_uuid: str,
-        platform: str,
-        verification_string: str
+    self, app_version: str, device_uuid: str, platform: str, verification_string: str
 ) -> VerifyDeviceResponse:
     # TODO: check platform, verification_string
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.GENUINE_DEVICES_V1}/verify",
+        "POST",
+        endpoint=f"{Endpoints.GENUINE_DEVICES_V1}/verify",
         payload={
             "app_version": app_version,
             "device_uuid": device_uuid,
             "platform": platform,
             "verification_string": verification_string,
-        }, data_type=VerifyDeviceResponse
+        },
+        data_type=VerifyDeviceResponse,
     )
     self.logger.info("Device has been verified.")
     return response
 
 
 def upload_image(self, image_type: str, image_path: str) -> str:
     """
@@ -172,17 +146,15 @@
         width, height = image.size
 
     base_url = f"{image_type}/{date.year}/{date.month}/{date.day}"
     mid_url = f"{filename}_{timestamp}_0_size_"
     original_url = f"{base_url}/{mid_url}{width}x{height}{ext}"
     thumb_url = f"{base_url}/thumb_{mid_url}{width}x{height}{ext}"
 
-    presigned_urls = get_file_upload_presigned_urls(
-        self, [original_url, thumb_url]
-    )
+    presigned_urls = get_file_upload_presigned_urls(self, [original_url, thumb_url])
 
     with open(image_path, "rb") as f:
         response = httpx.put(presigned_urls[0].url, data=f.read())
         self._handle_response(response)
 
     with open(image_path, "rb") as f:
         response = httpx.put(presigned_urls[1].url, data=f.read())
```

### Comparing `yaylib-0.1.3/yaylib/api/post.py` & `yaylib-0.1.5/yaylib/api/post.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,131 +8,139 @@
 from ..responses import *
 from ..utils import *
 
 
 def add_bookmark(self, user_id: int, post_id: int) -> BookmarkPostResponse:
     self._check_authorization()
     response = self._make_request(
-        "PUT", endpoint=f"{Endpoints.USERS_V1}/{user_id}/bookmarks/{post_id}",
-        data_type=BookmarkPostResponse
+        "PUT",
+        endpoint=f"{Endpoints.USERS_V1}/{user_id}/bookmarks/{post_id}",
+        data_type=BookmarkPostResponse,
     )
     self.logger.info("Post has been added to the bookmarks.")
     return response
 
 
 def add_group_highlight_post(self, group_id: int, post_id: int):
+    """
+
+    投稿をグループのまとめに追加します
+
+    """
     self._check_authorization()
     response = self._make_request(
-        "PUT", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/highlights/{post_id}",
+        "PUT",
+        endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/highlights/{post_id}",
     )
     self.logger.info("Post has been added to the group highlight.")
     return response
 
 
 def create_call_post(
-        self,
-        text: str = None,
-        font_size: int = None,
-        color: int = None,
-        group_id: int = None,
-        call_type: str = None,
-        category_id: int = None,
-        game_title: str = None,
-        joinable_by: str = None,
-        message_tags: str = "[]",
-        attachment_filename: str = None,
-        attachment_2_filename: str = None,
-        attachment_3_filename: str = None,
-        attachment_4_filename: str = None,
-        attachment_5_filename: str = None,
-        attachment_6_filename: str = None,
-        attachment_7_filename: str = None,
-        attachment_8_filename: str = None,
-        attachment_9_filename: str = None,
+    self,
+    text: str = None,
+    font_size: int = None,
+    color: int = None,
+    group_id: int = None,
+    call_type: str = None,
+    category_id: int = None,
+    game_title: str = None,
+    joinable_by: str = None,
+    message_tags: str = "[]",
+    attachment_filename: str = None,
+    attachment_2_filename: str = None,
+    attachment_3_filename: str = None,
+    attachment_4_filename: str = None,
+    attachment_5_filename: str = None,
+    attachment_6_filename: str = None,
+    attachment_7_filename: str = None,
+    attachment_8_filename: str = None,
+    attachment_9_filename: str = None,
 ) -> ConferenceCall:
     self._check_authorization()
 
     if text is not None:
         if "@:start:" in text and ":end:" in text:
             text, message_tags = parse_mention_format(self, text)
 
     timestamp = int(datetime.now().timestamp())
 
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.POSTS_V2}/new_conference_call",
+        "POST",
+        endpoint=f"{Endpoints.POSTS_V2}/new_conference_call",
         payload={
             "text": text,
             "font_size": font_size,
             "color": color,
             "group_id": group_id,
             "call_type": call_type,
             "uuid": self.uuid,
             "api_key": self.api_key,
             "timestamp": timestamp,
-            "signed_info": signed_info_calculating(
-                self.device_uuid, timestamp
-            ),
+            "signed_info": signed_info_calculating(self.device_uuid, timestamp),
             "category_id": category_id,
             "game_title": game_title,
             "joinable_by": joinable_by,
             "message_tags": message_tags,
             "attachment_filename": attachment_filename,
             "attachment_2_filename": attachment_2_filename,
             "attachment_3_filename": attachment_3_filename,
             "attachment_4_filename": attachment_4_filename,
             "attachment_5_filename": attachment_5_filename,
             "attachment_6_filename": attachment_6_filename,
             "attachment_7_filename": attachment_7_filename,
             "attachment_8_filename": attachment_8_filename,
             "attachment_9_filename": attachment_9_filename,
-        }, data_type=CreatePostResponse
+        },
+        data_type=CreatePostResponse,
     ).conference_call
     self.logger.info("Call post has been created.")
     return response
 
 
 def create_group_pin_post(self, post_id: int, group_id: int):
     self._check_authorization()
     response = self._make_request(
-        "PUT", endpoint=f"{Endpoints.POSTS_V2}/group_pinned_post",
-        payload={"post_id": post_id, "group_id": group_id}
+        "PUT",
+        endpoint=f"{Endpoints.POSTS_V2}/group_pinned_post",
+        payload={"post_id": post_id, "group_id": group_id},
     )
     self.logger.info("Pinned the post in the group.")
     return response
 
 
 def create_pin_post(self, post_id: int):
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.PINNED_V1}/posts",
-        payload={"id": post_id}
+        "POST", endpoint=f"{Endpoints.PINNED_V1}/posts", payload={"id": post_id}
     )
     self.logger.info("Pinned post.")
     return response
 
 
 def mention(self, user_id: int) -> str:
     if not (isinstance(user_id, int) or str(user_id).isdigit()):
         raise ValueError(
-            "The value of 'user_id' must be an integer or a string containing only digits.")
+            "The value of 'user_id' must be an integer or a string containing only digits."
+        )
     return "@:start:" + str(user_id) + ":end:"
 
 
 def convert_mention_format(self, text) -> tuple:
     # Do NOT write this function in client.py
     formatted_text = ""
     user_ids = []
     segments = text.split("@:start:")
 
     for i, segment in enumerate(segments):
         if i == 0:
             formatted_text += segment
             continue
         user_id, text = segment.split(":end:")
-        username = self.get_user(user_id).nickname
+        username = self.get_user_without_leaving_footprint(user_id).user.nickname
         formatted_text += "@" + username + " " + text
         user_ids.append(user_id)
 
     return formatted_text, user_ids
 
 
 def parse_mention_format(self, text) -> tuple:
@@ -146,67 +154,80 @@
     for user_id in user_ids:
         start = text.find("@", offset)
         if start == -1:
             break
         end = text.find(" ", start)
         if end == -1:
             end = len(text)
-        username = text[start+1:end]
-        message_tags.append({
-            "type": "user",
-            "user_id": int(user_id),
-            "offset": start,
-            "length": len(username)+1
-        })
+        username = text[start + 1 : end]
+        message_tags.append(
+            {
+                "type": "user",
+                "user_id": int(user_id),
+                "offset": start,
+                "length": len(username) + 1,
+            }
+        )
         offset = end
 
     return text, json.dumps(message_tags)
 
 
 def create_post(
-        self,
-        text: str = None,
-        font_size: int = 0,
-        color: int = 0,
-        in_reply_to: int = None,
-        group_id: int = None,
-        mention_ids: List[int] = None,
-        choices: List[str] = None,
-        shared_url: str = None,
-        message_tags: str = "[]",
-        attachment_filename: str = None,
-        attachment_2_filename: str = None,
-        attachment_3_filename: str = None,
-        attachment_4_filename: str = None,
-        attachment_5_filename: str = None,
-        attachment_6_filename: str = None,
-        attachment_7_filename: str = None,
-        attachment_8_filename: str = None,
-        attachment_9_filename: str = None,
-        video_file_name: str = None,
+    self,
+    text: str = None,
+    font_size: int = 0,
+    color: int = 0,
+    in_reply_to: int = None,
+    group_id: int = None,
+    mention_ids: List[int] = None,
+    choices: List[str] = None,
+    shared_url: str = None,
+    message_tags: str = "[]",
+    attachment_filename: str = None,
+    attachment_2_filename: str = None,
+    attachment_3_filename: str = None,
+    attachment_4_filename: str = None,
+    attachment_5_filename: str = None,
+    attachment_6_filename: str = None,
+    attachment_7_filename: str = None,
+    attachment_8_filename: str = None,
+    attachment_9_filename: str = None,
+    video_file_name: str = None,
 ) -> Post:
     self._check_authorization()
     headers = self.session.headers
     headers["X-Jwt"] = self.get_web_socket_token()
 
     if text is not None:
         if "@:start:" in text and ":end:" in text:
             text, message_tags = parse_mention_format(self, text)
 
-    post_type = "survey" if choices else "shareable_url" if shared_url else "video" if video_file_name else "image" if attachment_filename else "text"
+    post_type = (
+        "survey"
+        if choices
+        else "shareable_url"
+        if shared_url
+        else "video"
+        if video_file_name
+        else "image"
+        if attachment_filename
+        else "text"
+    )
 
     if shared_url is not None:
         try:
             shared_url = self.get_url_metadata(url=shared_url).data
         except ForbiddenError:
             self.logger.error("Unable to get the URL metadata")
             shared_url = None
 
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.POSTS_V3}/new",
+        "POST",
+        endpoint=f"{Endpoints.POSTS_V3}/new",
         payload={
             "text": text,
             "font_size": font_size,
             "color": color,
             "in_reply_to": in_reply_to,
             "group_id": group_id,
             "post_type": post_type,
@@ -220,62 +241,75 @@
             "attachment_4_filename": attachment_4_filename,
             "attachment_5_filename": attachment_5_filename,
             "attachment_6_filename": attachment_6_filename,
             "attachment_7_filename": attachment_7_filename,
             "attachment_8_filename": attachment_8_filename,
             "attachment_9_filename": attachment_9_filename,
             "video_file_name": video_file_name,
-        }, data_type=Post, headers=headers
+        },
+        data_type=Post,
+        headers=headers,
     )
     self.logger.info("Post has been created.")
     return response
 
 
 def create_repost(
-        self,
-        post_id: int,
-        text: str = None,
-        font_size: int = None,
-        color: int = None,
-        in_reply_to: int = None,
-        group_id: int = None,
-        mention_ids: List[int] = None,
-        choices: List[str] = None,
-        shared_url: Dict[str, Union[str, int]] = None,
-        message_tags: str = "[]",
-        attachment_filename: str = None,
-        attachment_2_filename: str = None,
-        attachment_3_filename: str = None,
-        attachment_4_filename: str = None,
-        attachment_5_filename: str = None,
-        attachment_6_filename: str = None,
-        attachment_7_filename: str = None,
-        attachment_8_filename: str = None,
-        attachment_9_filename: str = None,
-        video_file_name: str = None,
+    self,
+    post_id: int,
+    text: str = None,
+    font_size: int = None,
+    color: int = None,
+    in_reply_to: int = None,
+    group_id: int = None,
+    mention_ids: List[int] = None,
+    choices: List[str] = None,
+    shared_url: Dict[str, Union[str, int]] = None,
+    message_tags: str = "[]",
+    attachment_filename: str = None,
+    attachment_2_filename: str = None,
+    attachment_3_filename: str = None,
+    attachment_4_filename: str = None,
+    attachment_5_filename: str = None,
+    attachment_6_filename: str = None,
+    attachment_7_filename: str = None,
+    attachment_8_filename: str = None,
+    attachment_9_filename: str = None,
+    video_file_name: str = None,
 ) -> Post:
     self._check_authorization()
     headers = self.session.headers
     headers["X-Jwt"] = self.get_web_socket_token()
 
     if text is not None:
         if "@:start:" in text and ":end:" in text:
             text, message_tags = parse_mention_format(self, text)
 
-    post_type = "survey" if choices else "shareable_url" if shared_url else "video" if video_file_name else "image" if attachment_filename else "text"
+    post_type = (
+        "survey"
+        if choices
+        else "shareable_url"
+        if shared_url
+        else "video"
+        if video_file_name
+        else "image"
+        if attachment_filename
+        else "text"
+    )
 
     if shared_url is not None:
         try:
             shared_url = self.get_url_metadata(url=shared_url).data
         except ForbiddenError:
             self.logger.error("Unable to get the URL metadata")
             shared_url = None
 
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.POSTS_V3}/repost",
+        "POST",
+        endpoint=f"{Endpoints.POSTS_V3}/repost",
         payload={
             "post_id": post_id,
             "text": text,
             "font_size": font_size,
             "color": color,
             "in_reply_to": in_reply_to,
             "group_id": group_id,
@@ -290,94 +324,107 @@
             "attachment_4_filename": attachment_4_filename,
             "attachment_5_filename": attachment_5_filename,
             "attachment_6_filename": attachment_6_filename,
             "attachment_7_filename": attachment_7_filename,
             "attachment_8_filename": attachment_8_filename,
             "attachment_9_filename": attachment_9_filename,
             "video_file_name": video_file_name,
-        }, data_type=CreatePostResponse, headers=headers
+        },
+        data_type=CreatePostResponse,
+        headers=headers,
     ).post
     self.logger.info("Repost has been created.")
     return response
 
 
 def create_share_post(
-        self,
-        shareable_type: str,
-        shareable_id: int,
-        text: str = None,
-        font_size: int = None,
-        color: int = None,
-        group_id: int = None,
+    self,
+    shareable_type: str,
+    shareable_id: int,
+    text: str = None,
+    font_size: int = None,
+    color: int = None,
+    group_id: int = None,
 ) -> Post:
     self._check_authorization()
     timestamp = int(datetime.now().timestamp())
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.POSTS_V2}/new_share_post",
+        "POST",
+        endpoint=f"{Endpoints.POSTS_V2}/new_share_post",
         payload={
             "shareable_type": shareable_type,
             "shareable_id": shareable_id,
             "text": text,
             "font_size": font_size,
             "color": color,
             "group_id": group_id,
             "uuid": self.uuid,
             "api_key": self.api_key,
             "timestamp": timestamp,
-            "signed_info": signed_info_calculating(
-                self.device_uuid, timestamp
-            ),
-        }, data_type=Post
+            "signed_info": signed_info_calculating(self.device_uuid, timestamp),
+        },
+        data_type=Post,
     )
     self.logger.info("Share post has been created.")
     return response
 
 
 def create_thread_post(
-        self,
-        post_id: int,
-        text: str = None,
-        font_size: int = None,
-        color: int = None,
-        in_reply_to: int = None,
-        group_id: int = None,
-        mention_ids: List[int] = None,
-        choices: List[str] = None,
-        shared_url: Dict[str, Union[str, int]] = None,
-        message_tags: str = "[]",
-        attachment_filename: str = None,
-        attachment_2_filename: str = None,
-        attachment_3_filename: str = None,
-        attachment_4_filename: str = None,
-        attachment_5_filename: str = None,
-        attachment_6_filename: str = None,
-        attachment_7_filename: str = None,
-        attachment_8_filename: str = None,
-        attachment_9_filename: str = None,
-        video_file_name: str = None,
+    self,
+    post_id: int,
+    text: str = None,
+    font_size: int = None,
+    color: int = None,
+    in_reply_to: int = None,
+    group_id: int = None,
+    mention_ids: List[int] = None,
+    choices: List[str] = None,
+    shared_url: Dict[str, Union[str, int]] = None,
+    message_tags: str = "[]",
+    attachment_filename: str = None,
+    attachment_2_filename: str = None,
+    attachment_3_filename: str = None,
+    attachment_4_filename: str = None,
+    attachment_5_filename: str = None,
+    attachment_6_filename: str = None,
+    attachment_7_filename: str = None,
+    attachment_8_filename: str = None,
+    attachment_9_filename: str = None,
+    video_file_name: str = None,
 ) -> Post:
     self._check_authorization()
     headers = self.session.headers
     headers["X-Jwt"] = self.get_web_socket_token()
 
     if text is not None:
         if "@:start:" in text and ":end:" in text:
             text, message_tags = parse_mention_format(self, text)
 
-    post_type = "survey" if choices else "shareable_url" if shared_url else "video" if video_file_name else "image" if attachment_filename else "text"
+    post_type = (
+        "survey"
+        if choices
+        else "shareable_url"
+        if shared_url
+        else "video"
+        if video_file_name
+        else "image"
+        if attachment_filename
+        else "text"
+    )
 
     if shared_url is not None:
         try:
             shared_url = self.get_url_metadata(url=shared_url).data
         except ForbiddenError:
             self.logger.error("Unable to get the URL metadata")
             shared_url = None
 
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.THREADS_V1}/{post_id}/posts",
+        "POST",
+        endpoint=f"{Endpoints.THREADS_V1}/{post_id}/posts",
         payload={
             "id": post_id,
             "text": text,
             "font_size": font_size,
             "color": color,
             "in_reply_to": in_reply_to,
             "group_id": group_id,
@@ -392,37 +439,41 @@
             "attachment_4_filename": attachment_4_filename,
             "attachment_5_filename": attachment_5_filename,
             "attachment_6_filename": attachment_6_filename,
             "attachment_7_filename": attachment_7_filename,
             "attachment_8_filename": attachment_8_filename,
             "attachment_9_filename": attachment_9_filename,
             "video_file_name": video_file_name,
-        }, data_type=Post, headers=headers
+        },
+        data_type=Post,
+        headers=headers,
     )
     self.logger.info("Thread post has been created.")
     return response
 
 
 def delete_all_post(self):
     self._check_authorization()
     try:
         response = self._make_request(
-            "POST", endpoint=f"{Endpoints.POSTS_V1}/delete_all_post",
+            "POST",
+            endpoint=f"{Endpoints.POSTS_V1}/delete_all_post",
         )
         self.logger.info("Post deletion request has been sent.")
         return response
     except NotFoundError:
         self.logger.info("Post not found. Skipping...")
 
 
 def delete_group_pin_post(self, group_id: int):
     self._check_authorization()
     response = self._make_request(
-        "DELETE", endpoint=f"{Endpoints.POSTS_V2}/group_pinned_post",
-        payload={"group_id": group_id}
+        "DELETE",
+        endpoint=f"{Endpoints.POSTS_V2}/group_pinned_post",
+        payload={"group_id": group_id},
     )
     self.logger.info("Unpinned post in the group.")
     return response
 
 
 def delete_pin_post(self, post_id: int):
     self._check_authorization()
@@ -435,16 +486,18 @@
 
 def get_bookmark(self, user_id: int, from_str: str = None) -> PostsResponse:
     self._check_authorization()
     params = {}
     if from_str:
         params = {"from": from_str}
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V1}/{user_id}/bookmarks",
-        params=params, data_type=PostsResponse
+        "GET",
+        endpoint=f"{Endpoints.USERS_V1}/{user_id}/bookmarks",
+        params=params,
+        data_type=PostsResponse,
     )
 
 
 def get_timeline_calls(self, **params) -> PostsResponse:
     """
 
     Parameters:
@@ -458,16 +511,18 @@
         - include_circle_call: bool = None
         - cross_generation: bool = None
         - exclude_recent_gomimushi: bool = None
         - shared_interest_categories: bool = None
 
     """
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.POSTS_V2}/call_timeline",
-        params=params, data_type=PostsResponse
+        "GET",
+        endpoint=f"{Endpoints.POSTS_V2}/call_timeline",
+        params=params,
+        data_type=PostsResponse,
     )
 
 
 def get_conversation(self, conversation_id: int, **params) -> PostsResponse:
     """
 
     Parameters:
@@ -478,23 +533,27 @@
         - thread_id: int = None
         - from_post_id: int = None
         - number: int = 50
         - reverse: bool = True
 
     """
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.CONVERSATIONS_V2}/{conversation_id}",
-        params=params, data_type=PostsResponse
+        "GET",
+        endpoint=f"{Endpoints.CONVERSATIONS_V2}/{conversation_id}",
+        params=params,
+        data_type=PostsResponse,
     )
 
 
 def get_conversation_root_posts(self, post_ids: List[int]) -> PostsResponse:
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.CONVERSATIONS_V2}/root_posts",
-        params={"ids[]": post_ids}, data_type=PostsResponse
+        "GET",
+        endpoint=f"{Endpoints.CONVERSATIONS_V2}/root_posts",
+        params={"ids[]": post_ids},
+        data_type=PostsResponse,
     )
 
 
 def get_following_call_timeline(self, **params) -> PostsResponse:
     """
 
     Parameters:
@@ -506,16 +565,18 @@
         - call_type: str = None
         - include_circle_call: bool = None
         - exclude_recent_gomimushi: bool = None
 
     """
     self._check_authorization()
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.POSTS_V2}/call_followers_timeline",
-        params=params, data_type=PostsResponse
+        "GET",
+        endpoint=f"{Endpoints.POSTS_V2}/call_followers_timeline",
+        params=params,
+        data_type=PostsResponse,
     )
 
 
 def get_following_timeline(self, **params) -> PostsResponse:
     """
 
     Parameters:
@@ -528,53 +589,63 @@
         - mxn: int = None
         - reduce_selfie: bool = None
         - custom_generation_range: bool = None
 
     """
     self._check_authorization()
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.POSTS_V2}/following_timeline",
-        params=params, data_type=PostsResponse
+        "GET",
+        endpoint=f"{Endpoints.POSTS_V2}/following_timeline",
+        params=params,
+        data_type=PostsResponse,
     )
 
 
 def get_group_highlight_posts(self, group_id: int, **params) -> PostsResponse:
     """
 
+    グループのまとめ投稿を取得します
+
     Parameters:
     ----------
 
         - group_id: int
         - from_post: int = None
         - number: int = None
 
     """
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/highlights",
-        params=params, data_type=PostsResponse
+        "GET",
+        endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/highlights",
+        params=params,
+        data_type=PostsResponse,
     )
 
 
-def get_group_timeline_by_keyword(self, group_id: int, keyword: str, **params) -> PostsResponse:
+def get_group_timeline_by_keyword(
+    self, group_id: int, keyword: str, **params
+) -> PostsResponse:
     """
 
     Parameters:
     ----------
 
         - group_id: int
         - keyword: str
         - from_post_id: int = None
         - number: int = None
         - only_thread_posts: bool = False
 
     """
     params["keyword"] = keyword
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.GROUPS_V2}/{group_id}/posts/search",
-        params=params, data_type=PostsResponse
+        "GET",
+        endpoint=f"{Endpoints.GROUPS_V2}/{group_id}/posts/search",
+        params=params,
+        data_type=PostsResponse,
     )
 
 
 def get_group_timeline(self, group_id: int, **params) -> PostsResponse:
     """
 
     Parameters:
@@ -586,16 +657,18 @@
         - post_type: str
         - number: int
         - only_root: bool
 
     """
     params["group_id"] = group_id
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.POSTS_V2}/group_timeline",
-        params=params, data_type=PostsResponse
+        "GET",
+        endpoint=f"{Endpoints.POSTS_V2}/group_timeline",
+        params=params,
+        data_type=PostsResponse,
     )
 
 
 def get_timeline_by_hashtag(self, hashtag: str, **params) -> PostsResponse:
     """
 
     Parameters:
@@ -603,16 +676,18 @@
 
         - hashtag: str - (required)
         - from_post_id: int - (optional)
         - number: int - (optional)
 
     """
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.POSTS_V2}/tags/{hashtag}",
-        params=params, data_type=PostsResponse
+        "GET",
+        endpoint=f"{Endpoints.POSTS_V2}/tags/{hashtag}",
+        params=params,
+        data_type=PostsResponse,
     )
 
 
 def get_my_posts(self, **params) -> PostsResponse:
     """
 
     Parameters:
@@ -621,40 +696,42 @@
         - from_post_id: int - (optional)
         - number: int - (optional)
         - include_group_post: bool - (optional)
 
     """
     self._check_authorization()
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.POSTS_V2}/mine",
-        params=params, data_type=PostsResponse
+        "GET",
+        endpoint=f"{Endpoints.POSTS_V2}/mine",
+        params=params,
+        data_type=PostsResponse,
     )
 
 
 def get_post(self, post_id: int) -> Post:
-    # @Header("Cache-Control") @Nullable String str);
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.POSTS_V2}/{post_id}",
-        data_type=PostResponse
+        "GET", endpoint=f"{Endpoints.POSTS_V2}/{post_id}", data_type=PostResponse
     ).post
 
 
 def get_post_likers(self, post_id: int, **params) -> PostLikersResponse:
     """
 
     Parameters:
     ---------------
 
         - from_id: int - (optional)
         - number: int - (optional)
 
     """
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.POSTS_V1}/{post_id}/likers",
-        params=params, data_type=PostLikersResponse
+        "GET",
+        endpoint=f"{Endpoints.POSTS_V1}/{post_id}/likers",
+        params=params,
+        data_type=PostLikersResponse,
     )
 
 
 def get_post_reposts(self, post_id: int, **params: int) -> PostsResponse:
     """
 
     Parameters:
@@ -662,33 +739,38 @@
 
         - post_id: int - (required)
         - from_post_id: int - (optional)
         - number: int - (optional)
 
     """
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.POSTS_V2}/{post_id}/reposts",
-        params=params, data_type=PostsResponse
+        "GET",
+        endpoint=f"{Endpoints.POSTS_V2}/{post_id}/reposts",
+        params=params,
+        data_type=PostsResponse,
     )
 
 
 def get_posts(self, post_ids: List[int]) -> PostsResponse:
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.POSTS_V2}/multiple",
-        params={"post_ids[]": post_ids}, data_type=PostsResponse
+        "GET",
+        endpoint=f"{Endpoints.POSTS_V2}/multiple",
+        params={"post_ids[]": post_ids},
+        data_type=PostsResponse,
     )
 
 
 def get_recommended_post_tags(
-        self, tag: str = None, save_recent_search: bool = False
+    self, tag: str = None, save_recent_search: bool = False
 ) -> PostTagsResponse:
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.POSTS_V1}/recommended_tag",
+        "GET",
+        endpoint=f"{Endpoints.POSTS_V1}/recommended_tag",
         payload={"tag": tag, "save_recent_search": save_recent_search},
-        data_type=PostTagsResponse
+        data_type=PostTagsResponse,
     )
 
 
 def get_recommended_posts(self, **params) -> PostsResponse:
     """
 
     Parameters:
@@ -696,16 +778,18 @@
 
         - experiment_num: int - (Required)
         - variant_num: int - (Required)
         - number: int - (Optional)
 
     """
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.POSTS_V2}/recommended_timeline",
-        params=params, data_type=PostsResponse
+        "GET",
+        endpoint=f"{Endpoints.POSTS_V2}/recommended_timeline",
+        params=params,
+        data_type=PostsResponse,
     )
 
 
 def get_timeline_by_keyword(self, keyword: str = None, **params) -> PostsResponse:
     """
 
     Parameters:
@@ -714,16 +798,18 @@
         - keyword: str
         - from_post_id: int
         - number: int
 
     """
     params["keyword"] = keyword
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.POSTS_V2}/search",
-        params=params, data_type=PostsResponse
+        "GET",
+        endpoint=f"{Endpoints.POSTS_V2}/search",
+        params=params,
+        data_type=PostsResponse,
     )
 
 
 def get_timeline(self, **params: int | str | bool) -> PostsResponse:
     # - from: str - (optional)
     """
 
@@ -744,23 +830,24 @@
 
     """
     endpoint = f"{Endpoints.POSTS_V2}/timeline"
     if "noreply_mode" in params and params["noreply_mode"] is True:
         self._check_authorization()
         endpoint = f"{Endpoints.POSTS_V2}/noreply_timeline"
     return self._make_request(
-        "GET", endpoint=endpoint,
-        params=params, data_type=PostsResponse
+        "GET", endpoint=endpoint, params=params, data_type=PostsResponse
     )
 
 
 def get_url_metadata(self, url: str) -> SharedUrl:
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.POSTS_V2}/url_metadata",
-        params={"url": url}, data_type=SharedUrl
+        "GET",
+        endpoint=f"{Endpoints.POSTS_V2}/url_metadata",
+        params={"url": url},
+        data_type=SharedUrl,
     )
 
 
 def get_user_timeline(self, user_id: int, **params) -> PostsResponse:
     """
 
     Parameters:
@@ -769,165 +856,146 @@
         - from_post_id: int - (optional)
         - number: int - (optional)
         - post_type: str - (optional)
 
     """
     params["user_id"] = user_id
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.POSTS_V2}/user_timeline",
-        params=params, data_type=PostsResponse
+        "GET",
+        endpoint=f"{Endpoints.POSTS_V2}/user_timeline",
+        params=params,
+        data_type=PostsResponse,
     )
 
 
 def like_posts(self, post_ids: List[int]) -> LikePostsResponse:
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.POSTS_V2}/like",
-        payload={"post_ids": post_ids}, data_type=LikePostsResponse
+        "POST",
+        endpoint=f"{Endpoints.POSTS_V2}/like",
+        payload={"post_ids": post_ids},
+        data_type=LikePostsResponse,
     )
     self.logger.info("Posts have been liked.")
     return response
 
 
 def remove_bookmark(self, user_id: int, post_id: int):
     self._check_authorization()
     response = self._make_request(
-        "DELETE", endpoint=f"{Endpoints.USERS_V1}/{user_id}/bookmarks/{post_id}",
+        "DELETE",
+        endpoint=f"{Endpoints.USERS_V1}/{user_id}/bookmarks/{post_id}",
     )
     self.logger.info("Bookmark has been removed.")
     return response
 
 
 def remove_group_highlight_post(self, group_id: int, post_id: int):
     self._check_authorization()
     response = self._make_request(
-        "DELETE", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/highlights/{post_id}",
+        "DELETE",
+        endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/highlights/{post_id}",
     )
     self.logger.info("Group hightlight post removed.")
     return response
 
 
 def remove_posts(self, post_ids: List[int]):
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.POSTS_V2}/mass_destroy",
-        payload={"posts_ids": post_ids}
+        "POST",
+        endpoint=f"{Endpoints.POSTS_V2}/mass_destroy",
+        payload={"posts_ids": post_ids},
     )
     self.logger.info("Posts have been removed.")
     return response
 
 
 def report_post(
-        self,
-        post_id: int,
-        opponent_id: int,
-        category_id: int,
-        reason: str = None,
-        screenshot_filename: str = None,
-        screenshot_2_filename: str = None,
-        screenshot_3_filename: str = None,
-        screenshot_4_filename: str = None
+    self,
+    post_id: int,
+    opponent_id: int,
+    category_id: int,
+    reason: str = None,
+    screenshot_filename: str = None,
+    screenshot_2_filename: str = None,
+    screenshot_3_filename: str = None,
+    screenshot_4_filename: str = None,
 ):
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.POSTS_V3}/{post_id}/report",
+        "POST",
+        endpoint=f"{Endpoints.POSTS_V3}/{post_id}/report",
         payload={
             "opponent_id": opponent_id,
             "category_id": category_id,
             "reason": reason,
             "screenshot_filename": screenshot_filename,
             "screenshot_2_filename": screenshot_2_filename,
             "screenshot_3_filename": screenshot_3_filename,
             "screenshot_4_filename": screenshot_4_filename,
-        }
+        },
     )
     self.logger.info("Post has been reported.")
     return response
 
 
 def unlike_post(self, post_id: int):
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.POSTS_V1}/{post_id}/unlike",
+        "POST",
+        endpoint=f"{Endpoints.POSTS_V1}/{post_id}/unlike",
     )
     self.logger.info("Post has been unliked.")
     return response
 
 
 def update_post(
-        self,
-        post_id: int,
-        text: str = None,
-        font_size: int = None,
-        color: int = None,
-        message_tags: str = "[]",
+    self,
+    post_id: int,
+    text: str = None,
+    font_size: int = None,
+    color: int = None,
+    message_tags: str = "[]",
 ) -> Post:
     self._check_authorization()
 
     if "@:start:" in text and ":end:" in text:
         text, message_tags = parse_mention_format(self, text)
 
     timestamp = int(datetime.now().timestamp())
 
     response = self._make_request(
-        "PUT", endpoint=f"{Endpoints.POSTS_V3}/{post_id}",
+        "PUT",
+        endpoint=f"{Endpoints.POSTS_V3}/{post_id}",
         payload={
             "text": text,
             "font_size": font_size,
             "color": color,
             "message_tags": str(message_tags),
             "api_key": self.api_key,
             "timestamp": timestamp,
-            "signed_info": signed_info_calculating(
-                self.device_uuid, timestamp
-            ),
-        }
+            "signed_info": signed_info_calculating(self.device_uuid, timestamp),
+        },
     )
     self.logger.info("Post has been updated.")
     return response
 
 
-def update_recommendation_feedback(
-        self, post_id: int, feedback_result: str, *,
-        experiment_num: int, variant_num: int,
-):
-    self._check_authorization()
-    response = self._make_request(
-        "POST", endpoint=f"{Endpoints.POSTS_V2}/{post_id}/recommendation_feedback",
-        payload={
-            "feedback_result": feedback_result,
-            "experiment_num": experiment_num,
-            "variant_num": variant_num
-        }
-    )
-    self.logger.info("Recommendation feedback has been updated.")
-    return response
-
-
-def validate_post(self, text: str, *, group_id: int = None, thread_id: int = None) -> ValidationPostResponse:
-    self._check_authorization()
-    response = self._make_request(
-        "POST", endpoint=f"{Endpoints.POSTS_V1}/validate",
-        payload={
-            "text": text, "group_id": group_id, "thread_id": thread_id
-        }, data_type=ValidationPostResponse
-    )
-    self.logger.info("Post has been validated.")
-    return response
-
-
 def view_video(self, video_id: int):
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.POSTS_V1}/videos/{video_id}/view"
     )
     self.logger.info("Viewed the video.")
     return response
 
 
 def vote_survey(self, survey_id: int, choice_id: int) -> Survey:
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.SURVEYS_V2}/{survey_id}/vote",
-        payload={"choice_id": choice_id}, data_type=ValidationPostResponse
+        "POST",
+        endpoint=f"{Endpoints.SURVEYS_V2}/{survey_id}/vote",
+        payload={"choice_id": choice_id},
+        data_type=ValidationPostResponse,
     ).survey
     self.logger.info("Voted.")
     return response
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `yaylib-0.1.3/yaylib/api/thread.py` & `yaylib-0.1.5/yaylib/api/thread.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,138 +7,140 @@
 from ..responses import *
 from ..utils import *
 
 
 def add_post_to_thread(self, post_id: int, thread_id: int) -> ThreadInfo:
     self._check_authorization()
     response = self._make_request(
-        "PUT", endpoint=f"{Endpoints.POSTS_V3}/{post_id}/move_to_thread/{thread_id}",
-        data_type=ThreadInfo
+        "PUT",
+        endpoint=f"{Endpoints.POSTS_V3}/{post_id}/move_to_thread/{thread_id}",
+        data_type=ThreadInfo,
     )
     self.logger.info(f"Post '{post_id}' added to the thread '{thread_id}'.")
     return response
 
 
 def convert_post_to_thread(
-        self,
-        post_id: int,
-        title: str = None,
-        thread_icon_filename: str = None
+    self, post_id: int, title: str = None, thread_icon_filename: str = None
 ) -> ThreadInfo:
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.POSTS_V3}/{post_id}/move_to_thread",
-        payload={
-            "title": title,
-            "thread_icon_filename": thread_icon_filename
-        }, data_type=ThreadInfo
+        "POST",
+        endpoint=f"{Endpoints.POSTS_V3}/{post_id}/move_to_thread",
+        payload={"title": title, "thread_icon_filename": thread_icon_filename},
+        data_type=ThreadInfo,
     )
     self.logger.info("Post has been converted to a thread.")
     return response
 
 
 def create_thread(
-        self,
-        group_id: int,
-        title: str,
-        thread_icon_filename: str
+    self, group_id: int, title: str, thread_icon_filename: str
 ) -> ThreadInfo:
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.THREADS_V1}",
+        "POST",
+        endpoint=f"{Endpoints.THREADS_V1}",
         payload={
             "group_id": group_id,
             "title": title,
             "thread_icon_filename": thread_icon_filename,
-        }, data_type=ThreadInfo
+        },
+        data_type=ThreadInfo,
     )
     self.logger.info("A new thread has been created.")
     return response
 
 
-def get_group_thread_list(self, group_id: int, from_str: str = None, **params) -> GroupThreadListResponse:
+def get_group_thread_list(
+    self, group_id: int, from_str: str = None, **params
+) -> GroupThreadListResponse:
     """
 
     Parameters:
     ----------
 
         - group_id: int
         - from_str: str = None
         - join_status: str = None
 
     """
     params["group_id"] = group_id
     if from_str:
         params["from"] = from_str
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.THREADS_V1}",
-        params=params, data_type=GroupThreadListResponse
+        "GET",
+        endpoint=f"{Endpoints.THREADS_V1}",
+        params=params,
+        data_type=GroupThreadListResponse,
     )
 
 
 def get_thread_joined_statuses(self, ids: List[int]) -> dict:
     self._check_authorization()
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.THREADS_V1}/joined_statuses",
-        params={"ids[]": ids}
+        "GET", endpoint=f"{Endpoints.THREADS_V1}/joined_statuses", params={"ids[]": ids}
     )
 
 
-def get_thread_posts(self, thread_id: int, from_str: str = None, **params) -> PostsResponse:
+def get_thread_posts(
+    self, thread_id: int, from_str: str = None, **params
+) -> PostsResponse:
     """
 
     Parameters:
     ----------
 
         - post_type: str
         - number: int = None
         - from_str: str = None
 
     """
     if from_str:
         params["from"] = from_str
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.THREADS_V1}/{thread_id}/posts",
-        params=params, data_type=PostsResponse
+        "GET",
+        endpoint=f"{Endpoints.THREADS_V1}/{thread_id}/posts",
+        params=params,
+        data_type=PostsResponse,
     )
 
 
 def join_thread(self, thread_id: int, user_id: int):
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.THREADS_V1}/{thread_id}/members/{user_id}",
+        "POST",
+        endpoint=f"{Endpoints.THREADS_V1}/{thread_id}/members/{user_id}",
     )
     self.logger.info(f"Joined the thread '{thread_id}'.")
     return response
 
 
 def leave_thread(self, thread_id: int, user_id: int):
     self._check_authorization()
     response = self._make_request(
-        "DELETE", endpoint=f"{Endpoints.THREADS_V1}/{thread_id}/members/{user_id}",
+        "DELETE",
+        endpoint=f"{Endpoints.THREADS_V1}/{thread_id}/members/{user_id}",
     )
     self.logger.info("Left the thread.")
     return response
 
 
 def remove_thread(self, thread_id: int):
     self._check_authorization()
     response = self._make_request(
-        "DELETE", endpoint=f"{Endpoints.THREADS_V1}/{thread_id}",
+        "DELETE",
+        endpoint=f"{Endpoints.THREADS_V1}/{thread_id}",
     )
     self.logger.info(f"Thread '{thread_id}' has been removed.")
     return response
 
 
-def update_thread(
-        self,
-        thread_id: int,
-        title: str,
-        thread_icon_filename: str
-):
+def update_thread(self, thread_id: int, title: str, thread_icon_filename: str):
     self._check_authorization()
     response = self._make_request(
-        "PUT", endpoint=f"{Endpoints.THREADS_V1}/{thread_id}",
-        payload={"title": title, "thread_icon_filename": thread_icon_filename}
+        "PUT",
+        endpoint=f"{Endpoints.THREADS_V1}/{thread_id}",
+        payload={"title": title, "thread_icon_filename": thread_icon_filename},
     )
     self.logger.info(f"Thread '{thread_id}' has been updated.")
     return response
```

### Comparing `yaylib-0.1.3/yaylib/api/user.py` & `yaylib-0.1.5/yaylib/api/user.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,23 +4,14 @@
 from ..config import *
 from ..errors import *
 from ..models import *
 from ..responses import *
 from ..utils import *
 
 
-def delete_contact_friends(self):
-    self._check_authorization()
-    response = self._make_request(
-        "DELETE", endpoint=f"{Endpoints.USERS_V1}/contact_friends"
-    )
-    self.logger.info("Contact friends have been deleted.")
-    return response
-
-
 def delete_footprint(self, user_id: int, footprint_id: int):
     self._check_authorization()
     response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.USERS_V2}/{user_id}/footprints/{footprint_id}"
     )
     self.logger.info("Footprint has been deleted.")
     return response
@@ -29,23 +20,22 @@
 def destroy_user(self):
     self._check_authorization()
     answer = input("Are you sure you want to delete your account? Y/N")
     if answer.lower() != "y":
         return
     timestamp = int(datetime.now().timestamp())
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.USERS_V2}/destroy",
+        "POST",
+        endpoint=f"{Endpoints.USERS_V2}/destroy",
         payload={
             "uuid": self.uuid,
             "api_key": self.api_key,
             "timestamp": timestamp,
-            "signed_info": signed_info_calculating(
-                self.device_uuid, timestamp
-            ),
-        }
+            "signed_info": signed_info_calculating(self.device_uuid, timestamp),
+        },
     )
     self.logger.info("User has been deleted.")
     return response
 
 
 def follow_user(self, user_id: int):
     self._check_authorization()
@@ -55,16 +45,15 @@
     self.logger.info("Followed the user '{user_id}'.")
     return response
 
 
 def follow_users(self, user_ids: List[int]):
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.USERS_V2}/follow",
-        params={"user_ids[]": user_ids}
+        "POST", endpoint=f"{Endpoints.USERS_V2}/follow", params={"user_ids[]": user_ids}
     )
     self.logger.info("Followed multiple users.")
     return response
 
 
 def get_active_followings(self, **params) -> ActiveFollowingsResponse:
     """
@@ -74,90 +63,73 @@
 
         - only_online: bool
         - from_loggedin_at: int = None
 
     """
     self._check_authorization()
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V1}/active_followings",
-        params=params, data_type=ActiveFollowingsResponse
+        "GET",
+        endpoint=f"{Endpoints.USERS_V1}/active_followings",
+        params=params,
+        data_type=ActiveFollowingsResponse,
     )
 
 
-def get_additional_settings(self) -> Settings:
-    # AdditionalSettingsResponse
-    pass
-
-
-def get_app_review_status(self) -> AppReviewStatusResponse:
-    self._check_authorization()
-    return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V1}/{self.url_uuid}/app_review_status",
-        payload={"uuid": self.uuid}, data_type=AppReviewStatusResponse
-    )
-
-
-def get_contact_status(self, mobile_numbers: List[str]) -> ContactStatusResponse:
-    self._check_authorization()
-    return self._make_request(
-        "POST", endpoint=f"{Endpoints.USERS_V1}/contact_status",
-        payload={"mobile_numbers[]": mobile_numbers}, data_type=ContactStatusResponse
-    )
-
-
-def get_default_settings(self) -> TimelineSettings:
-    # DefaultSettingsResponse
-    pass
-
-
 def get_follow_recommendations(self, **params) -> FollowRecommendationsResponse:
     """
 
     Parameters:
     ----------
 
         - from_timestamp: int = None,
         - number: int = None,
         - sources: List[str] = None
 
     """
     self._check_authorization()
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.FRIENDS_V1}",
-        params=params, data_type=ActiveFollowingsResponse
+        "GET",
+        endpoint=f"{Endpoints.FRIENDS_V1}",
+        params=params,
+        data_type=FollowRecommendationsResponse,
     )
 
 
 def get_follow_request(self, from_timestamp: int = None) -> UsersByTimestampResponse:
     params = {}
     if from_timestamp:
         params["from_timestamp"] = from_timestamp
     self._check_authorization()
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V2}/follow_requests",
-        params=params, data_type=UsersByTimestampResponse
+        "GET",
+        endpoint=f"{Endpoints.USERS_V2}/follow_requests",
+        params=params,
+        data_type=UsersByTimestampResponse,
     )
 
 
 def get_follow_request_count(self) -> int:
     self._check_authorization()
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V2}/follow_requests_count",
-        data_type=FollowRequestCountResponse
+        "GET",
+        endpoint=f"{Endpoints.USERS_V2}/follow_requests_count",
+        data_type=FollowRequestCountResponse,
     ).users_count
 
 
 def get_following_users_born(self, birthdate: int = None) -> UsersResponse:
     params = {}
     if birthdate:
         params["birthdate"] = birthdate
     self._check_authorization()
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V1}/following_born_today",
-        params=params, data_type=UsersResponse
+        "GET",
+        endpoint=f"{Endpoints.USERS_V1}/following_born_today",
+        params=params,
+        data_type=UsersResponse,
     )
 
 
 def get_footprints(self, **params) -> List[Footprint]:
     """
 
     Parameters:
@@ -166,24 +138,25 @@
         - from_id: int = None
         - number: int = None
         - mode: str = None
 
     """
     self._check_authorization()
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V2}/footprints",
-        params=params, data_type=FootprintsResponse
+        "GET",
+        endpoint=f"{Endpoints.USERS_V2}/footprints",
+        params=params,
+        data_type=FootprintsResponse,
     ).footprints
 
 
 def get_fresh_user(self, user_id: int) -> UserResponse:
     self._check_authorization()
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V2}/fresh/{user_id}",
-        data_type=UserResponse
+        "GET", endpoint=f"{Endpoints.USERS_V2}/fresh/{user_id}", data_type=UserResponse
     )
 
 
 def get_hima_users(self, **params) -> List[UserWrapper]:
     """
 
     Parameters:
@@ -191,59 +164,60 @@
 
         - from_hima_id: int = None
         - number: int = None
 
     """
     self._check_authorization()
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V2}/hima_users",
-        params=params, data_type=HimaUsersResponse
+        "GET",
+        endpoint=f"{Endpoints.USERS_V2}/hima_users",
+        params=params,
+        data_type=HimaUsersResponse,
     ).hima_users
 
 
-def get_initial_recommended_users_to_follow(self, **params) -> UsersResponse:
+def get_user_ranking(self, mode: str) -> RankingUsersResponse:
     """
 
-    Parameters:
-    ----------
+    ユーザーのランキングを取得します
 
-        - en: int - (Optional)
-        - vn: int - (Optional)
+    Examples:
+    --------
 
-    """
-    self._check_authorization()
-    return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V1}/initial_follow_recommended",
-        params=params, data_type=UsersResponse
-    )
+    >>> ルーキーを取得する場合:
 
+    >>> api.get_user_ranking(mode="one_month")
 
-def get_recommended_users_to_follow_for_profile(self, user_id: int, **params) -> UsersResponse:
-    """
+    ---
 
-    Parameters:
-    ----------
+    >>> ミドルを取得する場合:
 
-        - user_id: int - (Required)
-        - number: int - (Optional)
-        - page: int - (Optional)
+    >>> api.get_user_ranking(mode="six_months")
+
+    ---
+
+    >>> 殿堂入りを取得する場合:
+
+    >>> api.get_user_ranking(mode="all_time")
 
     """
-    self._check_authorization()
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V1}/{user_id}/follow_recommended",
-        params=params, data_type=UsersResponse
+        "GET",
+        endpoint=f"{Endpoints.WEB_V1}/users/ranking",
+        params={"mode": mode},
+        data_type=RankingUsersResponse,
     )
 
 
 def get_refresh_counter_requests(self) -> RefreshCounterRequestsResponse:
     self._check_authorization()
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V1}/reset_counters",
-        data_type=RefreshCounterRequestsResponse
+        "GET",
+        endpoint=f"{Endpoints.USERS_V1}/reset_counters",
+        data_type=RefreshCounterRequestsResponse,
     )
 
 
 def get_social_shared_users(self, **params) -> SocialShareUsersResponse:
     """
 
     Parameters:
@@ -252,46 +226,41 @@
         - sns_name: str - (Required)
         - number: int - (Optional)
         - from_id: int - (Optional)
 
     """
     self._check_authorization()
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V2}/social_shared_users",
-        params=params, data_type=SocialShareUsersResponse
+        "GET",
+        endpoint=f"{Endpoints.USERS_V2}/social_shared_users",
+        params=params,
+        data_type=SocialShareUsersResponse,
     )
 
 
 def get_timestamp(self) -> UserTimestampResponse:
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V2}/timestamp",
-        data_type=UserTimestampResponse
+        "GET",
+        endpoint=f"{Endpoints.USERS_V2}/timestamp",
+        data_type=UserTimestampResponse,
     )
 
 
 def get_user(self, user_id: int) -> User:
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V2}/{user_id}",
-        data_type=UserResponse
+        "GET", endpoint=f"{Endpoints.USERS_V2}/{user_id}", data_type=UserResponse
     ).user
 
 
-def get_user_custom_definitions(self) -> UserCustomDefinitionsResponse:
-    self._check_authorization()
-    return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V1}/custom_definitions",
-        data_type=UserCustomDefinitionsResponse
-    )
-
-
 def get_user_email(self, user_id: int) -> str:
     self._check_authorization()
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V2}/fresh/{user_id}",
-        data_type=UserEmailResponse
+        "GET",
+        endpoint=f"{Endpoints.USERS_V2}/fresh/{user_id}",
+        data_type=UserEmailResponse,
     ).email
 
 
 def get_user_followers(self, user_id: int, **params) -> FollowUsersResponse:
     """
 
     Parameters:
@@ -300,16 +269,18 @@
         - user_id: int - (required)
         - from_follow_id: int - (optional)
         - followed_by_me: int - (optional)
         - number: int - (optional)
 
     """
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V2}/{user_id}/followers",
-        params=params, data_type=FollowUsersResponse
+        "GET",
+        endpoint=f"{Endpoints.USERS_V2}/{user_id}/followers",
+        params=params,
+        data_type=FollowUsersResponse,
     )
 
 
 def get_user_followings(self, user_id: int, **params) -> FollowUsersResponse:
     # @Body @Nullable SearchUsersRequest searchUsersRequest
     """
 
@@ -321,97 +292,69 @@
         - from_timestamp: int = None
         - order_by: str = None
         - number: int - (optional)
 
     """
     self._check_authorization()
     return self._make_request(
-        "POST", endpoint=f"{Endpoints.USERS_V2}/{user_id}/list_followings",
-        params=params, data_type=FollowUsersResponse
+        "POST",
+        endpoint=f"{Endpoints.USERS_V2}/{user_id}/list_followings",
+        params=params,
+        data_type=FollowUsersResponse,
     )
 
 
 def get_user_from_qr(self, qr: str) -> UserResponse:
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V1}/qr_codes/{qr}",
-        data_type=UserResponse
+        "GET", endpoint=f"{Endpoints.USERS_V1}/qr_codes/{qr}", data_type=UserResponse
     )
 
 
-def get_user_interests(self):
-    # @NotNull Continuation<? super UserInterestsResponse> continuation
-    pass
-
-
 def get_user_without_leaving_footprint(self, user_id: int) -> UserResponse:
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V2}/info/{user_id}",
-        data_type=UserResponse
+        "GET", endpoint=f"{Endpoints.USERS_V2}/info/{user_id}", data_type=UserResponse
     )
 
 
 def get_users(self, user_ids: List[int]) -> UsersResponse:
     headers = self.session.headers
     headers["X-Jwt"] = self.get_web_socket_token()
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V1}/list_id",
-        params={"user_ids[]": user_ids}, data_type=UsersResponse,
-        headers=headers
+        "GET",
+        endpoint=f"{Endpoints.USERS_V1}/list_id",
+        params={"user_ids[]": user_ids},
+        data_type=UsersResponse,
+        headers=headers,
     )
 
 
-def get_users_from_uuid(self, uuid: str) -> UsersResponse:
-    # TODO: what it does?
-    return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V2}/list_uuid/",
-        params={"uuid": uuid}, data_type=UsersResponse
-    )
-
-
-def post_social_shared(self, sns_name: str):
-    response = self._make_request(
-        "POST", endpoint=f"{Endpoints.USERS_V2}/social_shared",
-        params={"sns_name": sns_name}
-    )
-    self.logger.info("Posted social shared post.")
-    return response
-
-
-def record_app_review_status(self):
-    response = self._make_request(
-        "POST", endpoint=f"{Endpoints.USERS_V1}/{self.url_uuid}/app_review_status",
-        params={"uuid": self.uuid}
-    )
-    self.logger.info("App review status recored.")
-    return response
-
-
 def reduce_kenta_penalty(self, user_id: int):
     self._check_authorization()
     timestamp = int(datetime.now().timestamp())
     response = self._make_request(
-        "POST", endpoint=f"{self.host}api/v3/users/{user_id}/reduce_penalty",
+        "POST",
+        endpoint=f"{self.host}api/v3/users/{user_id}/reduce_penalty",
         payload={
             "uuid": self.uuid,
             "api_key": self.api_key,
             "timestamp": timestamp,
-            "signed_info": signed_info_calculating(
-                self.device_uuid, timestamp
-            ),
-            "signed_version": signed_version_calculating()
-        }, data_type=CreatePostResponse
+            "signed_info": signed_info_calculating(self.device_uuid, timestamp),
+            "signed_version": signed_version_calculating(),
+        },
+        data_type=CreatePostResponse,
     )
     self.logger.info("Penalty has been reduced.")
     return response
 
 
 def refresh_counter(self, counter: str):
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.USERS_V1}/reset_counters",
-        payload={"counter": counter}
+        "POST",
+        endpoint=f"{Endpoints.USERS_V1}/reset_counters",
+        payload={"counter": counter},
     )
     self.logger.info("Requested counter refresh.")
     return response
 
 
 def remove_user_avatar(self):
     response = self._make_request(
@@ -426,47 +369,49 @@
         "POST", endpoint=f"{Endpoints.USERS_V2}/remove_cover_image"
     )
     self.logger.info("Profile cover image has been removed.")
     return response
 
 
 def report_user(
-        self,
-        user_id: int,
-        category_id: int,
-        reason: str = None,
-        screenshot_filename: str = None,
-        screenshot_2_filename: str = None,
-        screenshot_3_filename: str = None,
-        screenshot_4_filename: str = None
+    self,
+    user_id: int,
+    category_id: int,
+    reason: str = None,
+    screenshot_filename: str = None,
+    screenshot_2_filename: str = None,
+    screenshot_3_filename: str = None,
+    screenshot_4_filename: str = None,
 ):
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.USERS_V3}/{user_id}/report",
+        "POST",
+        endpoint=f"{Endpoints.USERS_V3}/{user_id}/report",
         payload={
             "category_id": category_id,
             "reason": reason,
             "screenshot_filename": screenshot_filename,
             "screenshot_2_filename": screenshot_2_filename,
             "screenshot_3_filename": screenshot_3_filename,
             "screenshot_4_filename": screenshot_4_filename,
-        }
+        },
     )
     self.logger.info(f"Reported the user '{user_id}'")
     return response
 
 
 def reset_password(self, email: str, email_grant_token: str, password: str):
     response = self._make_request(
-        "PUT", endpoint=f"{Endpoints.USERS_V1}/reset_password",
+        "PUT",
+        endpoint=f"{Endpoints.USERS_V1}/reset_password",
         payload={
             "email": email,
             "email_grant_token": email_grant_token,
             "password": password,
-        }
+        },
     )
     self.logger.info("Reset the password.")
     return response
 
 
 def search_lobi_users(self, **params) -> UsersResponse:
     """
@@ -476,16 +421,18 @@
 
         - nickname: str = None
         - number: int = None
         - from_str: str = None
 
     """
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.LOBI_FRIENDS_V1}",
-        params=params, data_type=UsersResponse
+        "GET",
+        endpoint=f"{Endpoints.LOBI_FRIENDS_V1}",
+        params=params,
+        data_type=UsersResponse,
     )
 
 
 def search_users(self, **params) -> UsersResponse:
     """
 
     Parameters:
@@ -500,202 +447,165 @@
         - not_recent_gomimushi: bool = None
         - recently_created: bool = None
         - same_prefecture: bool = None
         - save_recent_search: bool = None
 
     """
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V1}/search",
-        params=params, data_type=UsersResponse,
+        "GET",
+        endpoint=f"{Endpoints.USERS_V1}/search",
+        params=params,
+        data_type=UsersResponse,
     )
 
 
-def set_additional_setting_enabled(self, mode: str, on: int = None):
-    response = self._make_request(
-        "POST", endpoint=f"{Endpoints.USERS_V1}/additonal_notification_setting",
-        payload={"mode": mode, "on": on}
-    )
-    self.logger.info("Additional settings have been enabled.")
-    return response
-
-
 def set_follow_permission_enabled(self, nickname: str, is_private: bool = None):
     timestamp = int(datetime.now().timestamp())
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.USERS_V2}/edit",
+        "POST",
+        endpoint=f"{Endpoints.USERS_V2}/edit",
         payload={
             "nickname": nickname,
             "is_private": is_private,
             "uuid": self.uuid,
             "api_key": self.api_key,
             "timestamp": timestamp,
-            "signed_info": signed_info_calculating(
-                self.device_uuid, timestamp
-            ),
-            "signed_version": signed_version_calculating()
-        }
+            "signed_info": signed_info_calculating(self.device_uuid, timestamp),
+            "signed_version": signed_version_calculating(),
+        },
     )
     self.logger.info("Follow permission has been enabled.")
     return response
 
 
 def set_setting_follow_recommendation_enabled(self, on: bool):
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.USERS_V1}/visible_on_sns_friend_recommendation_setting",
-        params={"on": on}
+        params={"on": on},
     )
     self.logger.info("Follow recommendation has been enabled.")
     return response
 
 
 def take_action_follow_request(self, target_id: int, action: str):
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.USERS_V2}/{target_id}/follow_request",
-        payload={"action": action}
+        "POST",
+        endpoint=f"{Endpoints.USERS_V2}/{target_id}/follow_request",
+        payload={"action": action},
     )
     self.logger.info("Took action follow request.")
     return response
 
 
 def turn_on_hima(self):
     self._check_authorization()
     response = self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V1}/hima",
+        "GET",
+        endpoint=f"{Endpoints.USERS_V1}/hima",
     )
     self.logger.info("Turned on 'hima now'.")
     return response
 
 
 def unfollow_user(self, user_id: int):
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.USERS_V2}/{user_id}/unfollow",
+        "POST",
+        endpoint=f"{Endpoints.USERS_V2}/{user_id}/unfollow",
     )
     self.logger.info(f"Unfollowed the user '{user_id}'")
     return response
 
 
-def update_invite_contact_status(self, mobile_number: str):
-    self._check_authorization()
-    response = self._make_request(
-        "POST", endpoint=f"{Endpoints.USERS_V1}/invite_contact",
-        params={"mobile_number": mobile_number}
-    )
-    self.logger.info("Invite contact status updated.")
-    return response
-
-
 def update_language(self, language: str):
     timestamp = int(datetime.now().timestamp())
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.USERS_V1}/language",
+        "POST",
+        endpoint=f"{Endpoints.USERS_V1}/language",
         payload={
             "uuid": self.uuid,
             "api_key": self.api_key,
             "timestamp": timestamp,
-            "signed_info": signed_info_calculating(
-                self.device_uuid, timestamp),
+            "signed_info": signed_info_calculating(self.device_uuid, timestamp),
             "language": language,
-        }
+        },
     )
     self.logger.info("Language has been updated.")
     return response
 
 
 def update_user(
-        self,
-        nickname: str,
-        biography: str = None,
-        prefecture: str = None,
-        gender: int = None,
-        country_code: str = None,
-        profile_icon_filename: str = None,
-        cover_image_filename: str = None,
-        username: str = None,
+    self,
+    nickname: str,
+    biography: str = None,
+    prefecture: str = None,
+    gender: int = None,
+    country_code: str = None,
+    profile_icon_filename: str = None,
+    cover_image_filename: str = None,
+    username: str = None,
 ):
     self._check_authorization()
     timestamp = int(datetime.now().timestamp())
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.USERS_V3}/edit",
+        "POST",
+        endpoint=f"{Endpoints.USERS_V3}/edit",
         payload={
             "nickname": nickname,
             "biography": biography,
             "prefecture": prefecture,
             "gender": gender,
             "country_code": country_code,
             "profile_icon_filename": profile_icon_filename,
             "cover_image_filename": cover_image_filename,
             "username": username,
             "uuid": self.uuid,
             "api_key": self.api_key,
             "timestamp": timestamp,
-            "signed_info": signed_info_calculating(
-                self.device_uuid, timestamp
-            ),
-        }
+            "signed_info": signed_info_calculating(self.device_uuid, timestamp),
+        },
     )
     self.logger.info("User profile has been updated.")
     return response
 
 
-def update_user_interests(
-        self,
-        # @Body @NotNull CommonIdsRequest commonIdsRequest,
-        # @NotNull Continuation<? super Unit> continuation
-):
-    pass
-
-
-def upload_contacts_friends(
-        self,
-        # @Body @Nullable UploadContactsRequest uploadContactsRequest
-):
-    pass
-
-
-def upload_twitter_friend_ids(self, twitter_friend_ids: List[str]):
-    self._check_authorization()
-    response = self._make_request(
-        "POST", endpoint=f"{Endpoints.USERS_V1}/twitter_friends",
-        payload={"twitter_friend_ids[]": twitter_friend_ids}
-    )
-    self.logger.info("Uploaded Twitter friend ids.")
-    return response
-
-
 # BlockApi
 
 
 def block_user(self, user_id: int):
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.USERS_V1}/{user_id}/block",
+        "POST",
+        endpoint=f"{Endpoints.USERS_V1}/{user_id}/block",
     )
     self.logger.info(f"Blocked the user '{user_id}'")
     return response
 
 
 def get_blocked_user_ids(self) -> BlockedUserIdsResponse:
     self._check_authorization()
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V1}/block_ids",
-        data_type=BlockedUserIdsResponse
+        "GET",
+        endpoint=f"{Endpoints.USERS_V1}/block_ids",
+        data_type=BlockedUserIdsResponse,
     )
 
 
 def get_blocked_users(self, from_id: int = None) -> BlockedUsersResponse:
     # @Body @NotNull SearchUsersRequest searchUsersRequest
     self._check_authorization()
     params = {}
     if from_id:
         params["from_id"] = from_id
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.USERS_V2}/blocked",
-        params=params, data_type=BlockedUsersResponse
+        "GET",
+        endpoint=f"{Endpoints.USERS_V2}/blocked",
+        params=params,
+        data_type=BlockedUsersResponse,
     )
 
 
 def unblock_user(self, user_id: int):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V2}/{user_id}/unblock"
@@ -715,30 +625,32 @@
 
         - from: str = None
         - number: int = None
 
     """
     self._check_authorization()
     return self._make_request(
-        "GET", endpoint=f"{Endpoints.HIDDEN_V1}/users",
-        params=params, data_type=HiddenResponse
+        "GET",
+        endpoint=f"{Endpoints.HIDDEN_V1}/users",
+        params=params,
+        data_type=HiddenResponse,
     )
 
 
 def hide_user(self, user_id: int):
     self._check_authorization()
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.HIDDEN_V1}/users",
-        payload={"user_id": user_id}
+        "POST", endpoint=f"{Endpoints.HIDDEN_V1}/users", payload={"user_id": user_id}
     )
     self.logger.info(f"User '{user_id}' is hidden")
     return response
 
 
 def unhide_users(self, user_ids: List[int]):
     self._check_authorization()
     response = self._make_request(
-        "DELETE", endpoint=f"{Endpoints.HIDDEN_V1}/users",
-        params={"user_ids[]": user_ids}
+        "DELETE",
+        endpoint=f"{Endpoints.HIDDEN_V1}/users",
+        params={"user_ids[]": user_ids},
     )
     self.logger.info("Unhid users")
     return response
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `yaylib-0.1.3/yaylib/client.py` & `yaylib-0.1.5/yaylib/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,20 +36,19 @@
 
         >>> api = yaylib.Client()
         >>> timeline = api.get_timeline(number=30)
 
     #### Parameters
 
         - access_token: str - (optional)
-        - refresh_token: str - (optional)
         - proxy: str - (optional)
         - max_retries: int - (optional)
         - backoff_factor: float - (optional)
         - timeout: int - (optional)
-        - lang: str - (optional)
+        - err_lang: str - (optional)
         - base_path: str - (optional)
         - loglevel_stream: int - (optional)
         - host: str - (optional)
 
     <https://github.com/qvco/yaylib>
 
     ---
@@ -58,17 +57,14 @@
 
     Copyright (c) 2023 Qvco, Konn
 
     """
 
     # -CALL
 
-    def bump_call(self, call_id: int, participant_limit: int = None) -> dict:
-        return bump_call(self, call_id, participant_limit)
-
     def get_user_active_call(self, user_id: int) -> Post:
         """
 
         ユーザーが参加中の通話を取得します
 
         """
         return get_user_active_call(self, user_id)
@@ -85,22 +81,24 @@
         """
 
         通話の詳細を取得します
 
         """
         return get_call(self, call_id)
 
-    def get_call_invitable_users(self, call_id: int, from_timestamp: int = None) -> UsersByTimestampResponse:
+    def get_call_invitable_users(
+        self, call_id: int, from_timestamp: int = None
+    ) -> UsersByTimestampResponse:
         # @Nullable @Query("user[nickname]")
         """
 
         通話に招待可能なユーザーを取得します
 
         """
-        return UsersByTimestampResponse(self, call_id, from_timestamp)
+        return get_call_invitable_users(self, call_id, from_timestamp)
 
     def get_call_status(self, opponent_id: int) -> CallStatusResponse:
         """
 
         通話の状態を取得します
 
         """
@@ -119,15 +117,15 @@
 
         """
         return get_games(self, **params)
 
     def get_genres(self, **params) -> GenresResponse:
         """
 
-        ジャンルを取得します
+        通話のジャンルを取得します
 
         Parameters
         ----------
             - number: int - (optional)
             - from: int - (optional)
 
         """
@@ -144,15 +142,17 @@
             - group_category_id: int - (optional)
             - from_timestamp: int - (optional)
             - scope: str - (optional)
 
         """
         return get_group_calls(self, **params)
 
-    def invite_online_followings_to_call(self, call_id: int, group_id: int = None) -> dict:
+    def invite_online_followings_to_call(
+        self, call_id: int, group_id: int = None
+    ) -> dict:
         """
 
         オンラインの友達をまとめて通話に招待します
 
         Parameters
         ----------
             - call_id: int - (required)
@@ -171,18 +171,15 @@
             - call_id: int - (required)
             - user_ids: List[int] - (required)
 
         """
         return invite_users_to_call(self, call_id, user_ids)
 
     def invite_users_to_chat_call(
-            self,
-            chat_room_id: int,
-            room_id: int,
-            room_url: str
+        self, chat_room_id: int, room_id: int, room_url: str
     ) -> dict:
         """
 
         チャット通話にユーザーを招待します
 
         Parameters
         ----------
@@ -190,130 +187,83 @@
             - chat_room_id: int - (required)
             - room_id: int - (required)
             - room_url: int - (required)
 
         """
         return invite_users_to_chat_call(self, chat_room_id, room_id, room_url)
 
-    def kick_and_ban_from_call(self, call_id: int, user_id: int) -> dict:
+    def kick_user_from_call(self, call_id: int, user_id: int) -> dict:
         """
 
         ユーザーを通話からキックします
 
         Parameters
         ----------
 
             - call_id: int - (required)
             - user_id: int - (required)
 
         """
         return kick_and_ban_from_call(self, call_id, user_id)
 
-    def notify_anonymous_user_leave_agora_channel(
-            self,
-            conference_id: int,
-            agora_uid: str
-    ) -> dict:
-        """
-
-        匿名ユーザーが通話から退出したことを通知します
-
-        """
-        return notify_anonymous_user_leave_agora_channel(
-            self, conference_id, agora_uid
-        )
-
-    def notify_user_leave_agora_channel(self, conference_id: int, user_id: int) -> dict:
-        """
-
-        ユーザーが通話から退出したことを通知します
-
-        """
-        return notify_user_leave_agora_channel(self, conference_id, user_id)
-
-    def send_call_screenshot(
-            self,
-            screenshot_filename: str,
-            conference_id: int
-    ) -> dict:
-        """
-
-        通話のスクリーンショットを送信します
-
-        """
-        return send_call_screenshot(self, screenshot_filename, conference_id)
-
     def set_call(
-            self,
-            call_id: int,
-            joinable_by: str,
-            game_title: str = None,
-            category_id: str = None
+        self,
+        call_id: int,
+        joinable_by: str,
+        game_title: str = None,
+        category_id: str = None,
     ) -> dict:
         """
 
         通話を開始します
 
         """
         return set_call(self, call_id, joinable_by, game_title, category_id)
 
-    def set_user_role(
-            self,
-            call_id: int,
-            user_id: int,
-            role: str
-    ) -> dict:
+    def set_user_role(self, call_id: int, user_id: int, role: str) -> dict:
         """
 
         通話に参加中ののユーザーに役職を与えます
 
         """
         return set_user_role(self, call_id, user_id, role)
 
-    def start_call(
-            self,
-            conference_id: int,
-            call_sid: str
-    ) -> ConferenceCall:
+    def join_call(self, conference_id: int, call_sid: str = None) -> ConferenceCall:
         """
 
         通話に参加します
 
         """
         return start_call(self, conference_id, call_sid)
 
-    def stop_call(
-            self,
-            conference_id: int,
-            call_sid: str
-    ) -> dict:
+    def leave_call(self, conference_id: int, call_sid: str = None) -> dict:
         """
 
         通話から退出します
 
         """
         return stop_call(self, conference_id, call_sid)
 
     # -CASSANDRA
 
-    def get_user_activities(self, **params) -> ActivitiesResponse:
+    def get_activities(self, **params) -> ActivitiesResponse:
         """
 
         通知を取得します
 
         Parameters
         ----------
             - important: bool - (required)
             - from_timestamp: int - (optional)
             - number: int - (optional)
 
         """
         return get_user_activities(self, **params)
 
-    def get_user_merged_activities(self, **params) -> ActivitiesResponse:
+    def get_merged_activities(self, **params) -> ActivitiesResponse:
         """
 
         全種類の通知を取得します
 
         Parameters
         ----------
 
@@ -346,19 +296,19 @@
 
         チャットの未読ステータスを確認します
 
         """
         return check_unread_status(self, from_time)
 
     def create_group_chat(
-            self,
-            name: str,
-            with_user_ids: List[int],
-            icon_filename: str = None,
-            background_filename: str = None
+        self,
+        name: str,
+        with_user_ids: List[int],
+        icon_filename: str = None,
+        background_filename: str = None,
     ) -> CreateChatRoomResponse:
         """
 
         グループチャットを作成します
 
         Parameters
         ----------
@@ -366,45 +316,33 @@
             - name: str - (required)
             - with_user_ids: List[int] - (required)
             - icon_filename: str - (optional)
             - background_filename: str - (optional)
 
         """
         return create_group_chat(
-            self,
-            name,
-            with_user_ids,
-            icon_filename,
-            background_filename
+            self, name, with_user_ids, icon_filename, background_filename
         )
 
     def create_private_chat(
-            self,
-            with_user_id: int,
-            matching_id: int = None,
-            hima_chat: bool = False
+        self, with_user_id: int, matching_id: int = None, hima_chat: bool = False
     ) -> CreateChatRoomResponse:
         """
 
         個人チャットを作成します
 
         Parameters
         ----------
 
             - with_user_id: int - (required)
             - matching_id: str - (optional)
             - hima_chat: bool - (optional)
 
         """
-        return create_private_chat(
-            self,
-            with_user_id,
-            matching_id,
-            hima_chat
-        )
+        return create_private_chat(self, with_user_id, matching_id, hima_chat)
 
     def delete_background(self, room_id: int) -> dict:
         """
 
         チャットの背景画像を削除します
 
         Parameters
@@ -426,38 +364,34 @@
             - room_id: int - (required)
             - message_id: int - (required)
 
         """
         return delete_message(self, room_id, message_id)
 
     def edit_chat_room(
-            self,
-            chat_room_id: int,
-            name: str,
-            icon_filename: str = None,
-            background_filename: str = None
+        self,
+        chat_room_id: int,
+        name: str,
+        icon_filename: str = None,
+        background_filename: str = None,
     ) -> dict:
         """
 
         チャットルームを編集します
 
         """
         return edit_chat_room(
-            self,
-            chat_room_id,
-            name,
-            icon_filename,
-            background_filename
+            self, chat_room_id, name, icon_filename, background_filename
         )
 
     def get_chatable_users(
-            self,
-            from_follow_id: int = None,
-            from_timestamp: int = None,
-            order_by: str = None
+        self,
+        from_follow_id: int = None,
+        from_timestamp: int = None,
+        order_by: str = None,
     ) -> FollowUsersResponse:
         """
 
         チャット可能なユーザーを取得します
 
         """
         return get_chatable_users(from_follow_id, from_timestamp, order_by)
@@ -501,17 +435,14 @@
         ---------------
             - from_message_id: int - (optional)
             - to_message_id: int - (optional)
 
         """
         return get_messages(self, chat_room_id, **params)
 
-    # def get_notification_settings(self, chat_room_id: int) -> Settings:
-    #     return get_notification_settings(self, chat_room_id)
-
     def get_request_chat_rooms(self, from_timestamp: int = None) -> ChatRoomsResponse:
         """
 
         チャットリクエストを取得します
 
         """
         return get_request_chat_rooms(self, from_timestamp)
@@ -528,15 +459,15 @@
         """
 
         スタンプを取得します
 
         """
         return get_sticker_packs(self)
 
-    def get_total_chat_requests(self) -> int:
+    def get_chat_requests_count(self) -> int:
         """
 
         チャットリクエストの数を取得します
 
         """
         return get_total_chat_requests(self)
 
@@ -568,47 +499,22 @@
         """
 
         チャットルームをピン止めします
 
         """
         return pin_chat(self, room_id)
 
-    # def read_attachment(
-    #         self,
-    #         room_id: int,
-    #         attachment_msg_ids: List[int]
-    # ) -> dict:
-    #     """
-
-    #     アタッチメントを既読にします
-
-    #     """
-    #     # TODO: check if this works
-    #     return read_attachment(self, room_id, attachment_msg_ids)
-
     def read_message(self, chat_room_id: int, message_id: int) -> dict:
         """
 
         メッセージを既読にします
 
         """
         return read_message(self, chat_room_id, message_id)
 
-    # def read_video_message(
-    #         self,
-    #         room_id: int,
-    #         video_msg_ids: List[int]
-    # ) -> dict:
-    #     """
-
-    #     動画のメッセージを既読にします
-
-    #     """
-    #     return read_video_message(self, room_id, video_msg_ids)
-
     def refresh_chat_rooms(self, from_time: int = None) -> ChatRoomsResponse:
         """
 
         チャットルームを更新します
 
         """
         return refresh_chat_rooms(self, from_time)
@@ -626,15 +532,15 @@
         chat_room_id: int,
         opponent_id: int,
         category_id: int,
         reason: str = None,
         screenshot_filename: str = None,
         screenshot_2_filename: str = None,
         screenshot_3_filename: str = None,
-        screenshot_4_filename: str = None
+        screenshot_4_filename: str = None,
     ) -> dict:
         """
 
         チャットルームを通報します
 
         """
         return report_chat_room(
@@ -642,36 +548,28 @@
             chat_room_id,
             opponent_id,
             category_id,
             reason,
             screenshot_filename,
             screenshot_2_filename,
             screenshot_3_filename,
-            screenshot_4_filename
+            screenshot_4_filename,
         )
 
-    def send_media_screenshot_notification(self, room_id: int) -> dict:
-        """
-
-        スクリーンショットを通知します
-
-        """
-        return send_media_screenshot_notification(self, room_id)
-
     def send_message(
-            self,
-            chat_room_id: int,
-            message_type: str,
-            call_type: str = None,
-            text: str = None,
-            font_size: int = None,
-            gif_image_id: int = None,
-            attachment_file_name: str = None,
-            sticker_pack_id: int = None,
-            video_file_name: str = None
+        self,
+        chat_room_id: int,
+        message_type: str,
+        call_type: str = None,
+        text: str = None,
+        font_size: int = None,
+        gif_image_id: int = None,
+        attachment_file_name: str = None,
+        sticker_pack_id: int = None,
+        video_file_name: str = None,
     ) -> MessageResponse:
         """
 
         チャットルームにメッセージを送信します
 
         """
         return send_message(
@@ -680,24 +578,17 @@
             message_type,
             call_type,
             text,
             font_size,
             gif_image_id,
             attachment_file_name,
             sticker_pack_id,
-            video_file_name
+            video_file_name,
         )
 
-    # def set_notification_settings(
-    #     self,
-    #     chat_room_id: int,
-    #     notification_chat: int
-    # ) -> Settings:
-    #     return set_notification_settings(self)
-
     def unhide_chat(self, chat_room_ids: int) -> dict:
         """
 
         チャットの非表示を解除します
 
         """
         return unhide_chat(self, chat_room_ids)
@@ -757,35 +648,35 @@
 
         サークルの未読ステータスを取得します
 
         """
         return check_unread_status(self, from_time)
 
     def create_group(
-            self,
-            topic: str,
-            description: str = None,
-            secret: bool = None,
-            hide_reported_posts: bool = None,
-            hide_conference_call: bool = None,
-            is_private: bool = None,
-            only_verified_age: bool = None,
-            only_mobile_verified: bool = None,
-            call_timeline_display: bool = None,
-            allow_ownership_transfer: bool = None,
-            allow_thread_creation_by: str = None,
-            gender: int = None,
-            generation_groups_limit: int = None,
-            group_category_id: int = None,
-            cover_image_filename: str = None,
-            sub_category_id: str = None,
-            hide_from_game_eight: bool = None,
-            allow_members_to_post_media: bool = None,
-            allow_members_to_post_url: bool = None,
-            guidelines: str = None,
+        self,
+        topic: str,
+        description: str = None,
+        secret: bool = None,
+        hide_reported_posts: bool = None,
+        hide_conference_call: bool = None,
+        is_private: bool = None,
+        only_verified_age: bool = None,
+        only_mobile_verified: bool = None,
+        call_timeline_display: bool = None,
+        allow_ownership_transfer: bool = None,
+        allow_thread_creation_by: str = None,
+        gender: int = None,
+        generation_groups_limit: int = None,
+        group_category_id: int = None,
+        cover_image_filename: str = None,
+        sub_category_id: str = None,
+        hide_from_game_eight: bool = None,
+        allow_members_to_post_media: bool = None,
+        allow_members_to_post_url: bool = None,
+        guidelines: str = None,
     ) -> CreateGroupResponse:
         """
 
         サークルを作成します
 
         """
         return create_group(
@@ -797,28 +688,29 @@
             hide_conference_call,
             is_private,
             only_verified_age,
             only_mobile_verified,
             call_timeline_display,
             allow_ownership_transfer,
             allow_thread_creation_by,
-            gender, generation_groups_limit,
+            gender,
+            generation_groups_limit,
             group_category_id,
             cover_image_filename,
             sub_category_id,
             hide_from_game_eight,
             allow_members_to_post_media,
             allow_members_to_post_url,
-            guidelines
+            guidelines,
         )
 
-    def create_pin_group(self, group_id: int) -> dict:
+    def pin_group(self, group_id: int) -> dict:
         """
 
-        サークルの投稿をピンします
+        サークルをピンします
 
         """
         return create_pin_group(self, group_id)
 
     def decline_moderator_offer(self, group_id: int) -> dict:
         """
 
@@ -839,23 +731,25 @@
         """
 
         サークル参加リクエストを断ります
 
         """
         return decline_ownership_offer(self, group_id, user_id)
 
-    def delete_pin_group(self, group_id: int) -> dict:
+    def unpin_group(self, group_id: int) -> dict:
         """
 
-        サークルのピン投稿を解除します
+        サークルのピン止めを解除します
 
         """
         return delete_pin_group(self, group_id)
 
-    def get_banned_group_members(self, group_id: int, page: int = None) -> UsersResponse:
+    def get_banned_group_members(
+        self, group_id: int, page: int = None
+    ) -> UsersResponse:
         """
 
         追放されたサークルメンバーを取得します
 
         """
         return get_banned_group_members(self, group_id, page)
 
@@ -885,17 +779,14 @@
         """
 
         サークルの詳細を取得します
 
         """
         return get_group(self, group_id)
 
-    # def get_group_notification_settings(self, group_id: int) -> GroupNotificationSettingsResponse:
-    #     return get_group_notification_settings(self, group_id)
-
     def get_groups(self, **params) -> GroupsResponse:
         """
 
         複数のサークルの詳細を取得します
 
         Parameters
         ----------
@@ -919,14 +810,19 @@
             - from_timestamp: int - (optional)
             - user[nickname]: str - (optional)
 
         """
         return get_invitable_users(self, group_id, **params)
 
     def get_joined_statuses(self, ids: List[int]) -> dict:
+        """
+
+        サークルの参加ステータスを取得します
+
+        """
         return get_joined_statuses(self, ids)
 
     def get_group_member(self, group_id: int, user_id: int) -> GroupUserResponse:
         """
 
         特定のサークルメンバーの情報を取得します
 
@@ -1048,32 +944,34 @@
         """
 
         サークルの副管理人を削除します
 
         """
         return remove_moderator(self, group_id, user_id)
 
-    def remove_related_groups(self, group_id: int, related_group_ids: List[int]) -> dict:
+    def remove_related_groups(
+        self, group_id: int, related_group_ids: List[int]
+    ) -> dict:
         """
 
         関連のあるサークルを削除します
 
         """
         return remove_related_groups(self, group_id, related_group_ids)
 
     def report_group(
-            self,
-            group_id: int,
-            category_id: int,
-            reason: str = None,
-            opponent_id: int = None,
-            screenshot_filename: str = None,
-            screenshot_2_filename: str = None,
-            screenshot_3_filename: str = None,
-            screenshot_4_filename: str = None,
+        self,
+        group_id: int,
+        category_id: int,
+        reason: str = None,
+        opponent_id: int = None,
+        screenshot_filename: str = None,
+        screenshot_2_filename: str = None,
+        screenshot_3_filename: str = None,
+        screenshot_4_filename: str = None,
     ) -> dict:
         """
 
         サークルを通報します
 
         """
         return report_group(
@@ -1081,15 +979,15 @@
             group_id,
             category_id,
             reason,
             opponent_id,
             screenshot_filename,
             screenshot_2_filename,
             screenshot_3_filename,
-            screenshot_4_filename
+            screenshot_4_filename,
         )
 
     def send_moderator_offers(self, group_id: int, user_ids: List[int]) -> dict:
         """
 
         複数人にサークル副管理人のオファーを送信します
 
@@ -1100,24 +998,14 @@
         """
 
         サークル管理人権限のオファーを送信します
 
         """
         return send_ownership_offer(self, group_id, user_id)
 
-    # def set_group_notification_settings(
-    #         self,
-    #         group_id: int,
-    #         notification_group_post: int = None,
-    #         notification_group_join: int = None,
-    #         notification_group_request: int = None,
-    #         notification_group_message_tag_all: int = None,
-    # ) -> AdditionalSettingsResponse:
-    #     return set_group_notification_settings(self)
-
     def set_group_title(self, group_id: int, title: str) -> dict:
         """
 
         サークルのタイトルを設定します
 
         """
         return set_group_title(self, group_id, title)
@@ -1135,36 +1023,36 @@
 
         特定のサークルメンバーの追放を解除します
 
         """
         return unban_group_member(self, group_id, user_id)
 
     def update_group(
-            self,
-            group_id: int,
-            topic: str,
-            description: str = None,
-            secret: bool = None,
-            hide_reported_posts: bool = None,
-            hide_conference_call: bool = None,
-            is_private: bool = None,
-            only_verified_age: bool = None,
-            only_mobile_verified: bool = None,
-            call_timeline_display: bool = None,
-            allow_ownership_transfer: bool = None,
-            allow_thread_creation_by: str = None,
-            gender: int = None,
-            generation_groups_limit: int = None,
-            group_category_id: int = None,
-            cover_image_filename: str = None,
-            sub_category_id: str = None,
-            hide_from_game_eight: bool = None,
-            allow_members_to_post_media: bool = None,
-            allow_members_to_post_url: bool = None,
-            guidelines: str = None,
+        self,
+        group_id: int,
+        topic: str,
+        description: str = None,
+        secret: bool = None,
+        hide_reported_posts: bool = None,
+        hide_conference_call: bool = None,
+        is_private: bool = None,
+        only_verified_age: bool = None,
+        only_mobile_verified: bool = None,
+        call_timeline_display: bool = None,
+        allow_ownership_transfer: bool = None,
+        allow_thread_creation_by: str = None,
+        gender: int = None,
+        generation_groups_limit: int = None,
+        group_category_id: int = None,
+        cover_image_filename: str = None,
+        sub_category_id: str = None,
+        hide_from_game_eight: bool = None,
+        allow_members_to_post_media: bool = None,
+        allow_members_to_post_url: bool = None,
+        guidelines: str = None,
     ) -> GroupResponse:
         """
 
         サークルを編集します
 
         """
         return update_group(
@@ -1187,22 +1075,14 @@
             sub_category_id,
             hide_from_game_eight,
             allow_members_to_post_media,
             allow_members_to_post_url,
             guidelines,
         )
 
-    def visit_group(self, group_id: int) -> dict:
-        """
-
-        サークルを訪問します
-
-        """
-        return visit_group(self, group_id)
-
     def withdraw_moderator_offer(self, group_id: int, user_id: int) -> dict:
         """
 
         サークル副管理人のオファーを取り消します
 
         """
         return withdraw_moderator_offer(self, group_id, user_id)
@@ -1213,90 +1093,64 @@
         サークル管理人のオファーを取り消します
 
         """
         return withdraw_ownership_offer(self, group_id, user_id)
 
     # -LOGIN
 
-    def change_email(
-            self,
-            email: str,
-            password: str,
-            email_grant_token: str = None
-    ) -> LoginUpdateResponse:
+    def is_valid_token(self, access_token: str):
         """
 
-        メールアドレスを変更します
+        アクセストークンが有効か検証します
 
         """
-        return change_email(self, email, password, email_grant_token)
+        return is_valid_token(self, access_token)
 
     def change_password(
-            self,
-            current_password: str,
-            new_password: str
+        self, current_password: str, new_password: str
     ) -> LoginUpdateResponse:
         """
 
         パスワードを変更します
 
         """
         return change_password(self, current_password, new_password)
 
-    # def connect_account_with_sns(self) -> dict:
-    #     return connect_account_with_sns(self)
-
-    # def disconnect_account_with_sns(self) -> dict:
-    #     return disconnect_account_with_sns(self)
-
     def get_token(
-            self,
-            grant_type: str,
-            refresh_token: str = None,
-            email: str = None,
-            password: str = None
+        self,
+        grant_type: str,
+        refresh_token: str = None,
+        email: str = None,
+        password: str = None,
     ) -> TokenResponse:
         """
 
-        アクセストークンを再発行します
+        トークンを再発行します
 
         """
-        return get_token(
-            self,
-            grant_type,
-            refresh_token,
-            email,
-            password
-        )
+        return get_token(self, grant_type, refresh_token, email, password)
 
-    def login(self, email: str, password: str) -> LoginUserResponse:
+    def login(
+        self, email: str, password: str, secret_key: str = None
+    ) -> LoginUserResponse:
         """
 
         メールアドレスでログインします
 
         """
-        return login(self, email, password)
-
-    # def login_with_sns(self) -> dict:
-    #     return login_with_sns(self)
+        return login_with_email(self, email, password, secret_key)
 
     def logout(self) -> dict:
         """
 
         ログアウトします
 
         """
         return logout(self)
 
-    # def migrate_token(self) -> dict:
-    #     return migrate_token(self)
-
-    # def register_device_token(self) -> dict:
-    #     return register_device_token(self)
-
     def resend_confirm_email(self) -> dict:
         """
 
         確認メールを再送信します
 
         """
         return resend_confirm_email(self)
@@ -1314,19 +1168,19 @@
 
         トークンを無効化します
 
         """
         return revoke_tokens(self)
 
     def save_account_with_email(
-            self,
-            email: str,
-            password: str = None,
-            current_password: str = None,
-            email_grant_token: str = None
+        self,
+        email: str,
+        password: str = None,
+        current_password: str = None,
+        email_grant_token: str = None,
     ) -> LoginUpdateResponse:
         """
 
         メールアドレスでアカウントを保存します
 
         """
         return save_account_with_email(
@@ -1335,46 +1189,35 @@
             password,
             current_password,
             email_grant_token,
         )
 
     # -MISC
 
-    # def accept_policy_agreement(self, type: str) -> dict:
-    #     return accept_policy_agreement(self, type)
-
-    # def generate_sns_thumbnail(self, **params) -> dict:
-    #     """
-
-    #     Parameters
-    #     ----------
-
-    #         - resource_type: str - (Required)
-    #         - resource_id: int - (Required)
-
-    #     """
-    #     return generate_sns_thumbnail(self, **params)
-
     def get_email_grant_token(self, code: int, email: str) -> str:
         """
 
-        email_grant_token を取得します
+        email_grant_tokenを取得します
 
         """
         return get_email_grant_token(self, code, email)
 
-    def get_email_verification_presigned_url(self, email: str, locale: str, intent: str = None) -> str:
+    def get_email_verification_presigned_url(
+        self, email: str, locale: str, intent: str = None
+    ) -> str:
         """
 
         メールアドレス確認用の署名付きURLを取得します
 
         """
         return get_email_verification_presigned_url(self, email, locale, intent)
 
-    def get_file_upload_presigned_urls(self, file_names: List[str]) -> List[PresignedUrl]:
+    def get_file_upload_presigned_urls(
+        self, file_names: List[str]
+    ) -> List[PresignedUrl]:
         """
 
         ファイルアップロード用の署名付きURLを取得します
 
         """
         return get_file_upload_presigned_urls(self, file_names)
 
@@ -1390,62 +1233,21 @@
         """
 
         動画ファイルアップロード用の署名付きURLを取得します
 
         """
         return get_old_file_upload_presigned_url(self, video_file_name)
 
-    def get_policy_agreements(self) -> PolicyAgreementsResponse:
-        return get_policy_agreements(self)
-
-    # def get_promotions(self, **params) -> List[Promotion]:
-    #     """
-
-    #     プロモーションを取得します
-
-    #     Parameters
-    #     ----------
-
-    #         - page: int - (Optional)
-    #         - number: int - (Optional)
-
-    #     """
-    #     return get_promotions(self, **params)
-
-    # def get_vip_game_reward_url(self, device_type: str) -> str:
-    #     return get_vip_game_reward_url(self, device_type)
-
-    def get_web_socket_token(self) -> str:
+    def get_web_socket_token(self, headers: dict = None) -> str:
         """
 
-        Web Socket Token を取得します
+        Web Socket Tokenを取得します
 
         """
-        return get_web_socket_token(self)
-
-    # def verify_device(
-    #         self,
-    #         app_version: str,
-    #         device_uuid: str,
-    #         platform: str,
-    #         verification_string: str
-    # ) -> VerifyDeviceResponse:
-    #     """
-
-    #     デバイスを検証します
-
-    #     """
-    #     # TODO: check platform, verification_string
-    #     return verify_device(
-    #         self,
-    #         app_version,
-    #         device_uuid,
-    #         platform,
-    #         verification_string
-    #     )
+        return get_web_socket_token(self, headers)
 
     def upload_image(self, image_type: str, image_path: str) -> str:
         """
 
         画像をアップロードしてattachment_filenameを返します。
 
         Parameteres
@@ -1465,39 +1267,39 @@
 
         """
         return add_bookmark(self, user_id, post_id)
 
     def add_group_highlight_post(self, group_id: int, post_id: int) -> dict:
         """
 
-        投稿をグループハイライトに追加します
+        投稿をグループのまとめに追加します
 
         """
         return add_group_highlight_post(self, group_id, post_id)
 
     def create_call_post(
-            self,
-            text: str = None,
-            font_size: int = None,
-            color: int = None,
-            group_id: int = None,
-            call_type: str = None,
-            category_id: int = None,
-            game_title: str = None,
-            joinable_by: str = None,
-            message_tags: str = "[]",
-            attachment_filename: str = None,
-            attachment_2_filename: str = None,
-            attachment_3_filename: str = None,
-            attachment_4_filename: str = None,
-            attachment_5_filename: str = None,
-            attachment_6_filename: str = None,
-            attachment_7_filename: str = None,
-            attachment_8_filename: str = None,
-            attachment_9_filename: str = None,
+        self,
+        text: str = None,
+        font_size: int = None,
+        color: int = None,
+        group_id: int = None,
+        call_type: str = None,
+        category_id: int = None,
+        game_title: str = None,
+        joinable_by: str = None,
+        message_tags: str = "[]",
+        attachment_filename: str = None,
+        attachment_2_filename: str = None,
+        attachment_3_filename: str = None,
+        attachment_4_filename: str = None,
+        attachment_5_filename: str = None,
+        attachment_6_filename: str = None,
+        attachment_7_filename: str = None,
+        attachment_8_filename: str = None,
+        attachment_9_filename: str = None,
     ) -> ConferenceCall:
         """
 
         通話の投稿を作成します
 
         """
         return create_call_post(
@@ -1515,15 +1317,15 @@
             attachment_2_filename,
             attachment_3_filename,
             attachment_4_filename,
             attachment_5_filename,
             attachment_6_filename,
             attachment_7_filename,
             attachment_8_filename,
-            attachment_9_filename
+            attachment_9_filename,
         )
 
     def pin_group_post(self, post_id: int, group_id: int) -> dict:
         """
 
         グループの投稿をピンします
 
@@ -1543,34 +1345,34 @@
 
         メンション用文字列を返します
 
         """
         return mention(self, user_id)
 
     def create_post(
-            self,
-            text: str = None,
-            font_size: int = 0,
-            color: int = 0,
-            in_reply_to: int = None,
-            group_id: int = None,
-            mention_ids: List[int] = None,
-            choices: List[str] = None,
-            shared_url: str = None,
-            message_tags: str = "[]",
-            attachment_filename: str = None,
-            attachment_2_filename: str = None,
-            attachment_3_filename: str = None,
-            attachment_4_filename: str = None,
-            attachment_5_filename: str = None,
-            attachment_6_filename: str = None,
-            attachment_7_filename: str = None,
-            attachment_8_filename: str = None,
-            attachment_9_filename: str = None,
-            video_file_name: str = None,
+        self,
+        text: str = None,
+        font_size: int = 0,
+        color: int = 0,
+        in_reply_to: int = None,
+        group_id: int = None,
+        mention_ids: List[int] = None,
+        choices: List[str] = None,
+        shared_url: str = None,
+        message_tags: str = "[]",
+        attachment_filename: str = None,
+        attachment_2_filename: str = None,
+        attachment_3_filename: str = None,
+        attachment_4_filename: str = None,
+        attachment_5_filename: str = None,
+        attachment_6_filename: str = None,
+        attachment_7_filename: str = None,
+        attachment_8_filename: str = None,
+        attachment_9_filename: str = None,
+        video_file_name: str = None,
     ) -> Post:
         """
 
         投稿を作成します
 
         """
         return create_post(
@@ -1589,39 +1391,39 @@
             attachment_3_filename,
             attachment_4_filename,
             attachment_5_filename,
             attachment_6_filename,
             attachment_7_filename,
             attachment_8_filename,
             attachment_9_filename,
-            video_file_name
+            video_file_name,
         )
 
     def create_repost(
-            self,
-            post_id: int,
-            text: str = None,
-            font_size: int = None,
-            color: int = None,
-            in_reply_to: int = None,
-            group_id: int = None,
-            mention_ids: List[int] = None,
-            choices: List[str] = None,
-            shared_url: Dict[str, Union[str, int]] = None,
-            message_tags: str = "[]",
-            attachment_filename: str = None,
-            attachment_2_filename: str = None,
-            attachment_3_filename: str = None,
-            attachment_4_filename: str = None,
-            attachment_5_filename: str = None,
-            attachment_6_filename: str = None,
-            attachment_7_filename: str = None,
-            attachment_8_filename: str = None,
-            attachment_9_filename: str = None,
-            video_file_name: str = None,
+        self,
+        post_id: int,
+        text: str = None,
+        font_size: int = None,
+        color: int = None,
+        in_reply_to: int = None,
+        group_id: int = None,
+        mention_ids: List[int] = None,
+        choices: List[str] = None,
+        shared_url: Dict[str, Union[str, int]] = None,
+        message_tags: str = "[]",
+        attachment_filename: str = None,
+        attachment_2_filename: str = None,
+        attachment_3_filename: str = None,
+        attachment_4_filename: str = None,
+        attachment_5_filename: str = None,
+        attachment_6_filename: str = None,
+        attachment_7_filename: str = None,
+        attachment_8_filename: str = None,
+        attachment_9_filename: str = None,
+        video_file_name: str = None,
     ) -> Post:
         """
 
         投稿を(´∀｀∩)↑age↑します
 
         """
         return create_repost(
@@ -1645,59 +1447,53 @@
             attachment_7_filename,
             attachment_8_filename,
             attachment_9_filename,
             video_file_name,
         )
 
     def create_share_post(
-            self,
-            shareable_type: str,
-            shareable_id: int,
-            text: str = None,
-            font_size: int = None,
-            color: int = None,
-            group_id: int = None,
+        self,
+        shareable_type: str,
+        shareable_id: int,
+        text: str = None,
+        font_size: int = None,
+        color: int = None,
+        group_id: int = None,
     ) -> Post:
         """
 
         シェア投稿を作成します
 
         """
         return create_share_post(
-            self,
-            shareable_type,
-            shareable_id,
-            text,
-            font_size,
-            color,
-            group_id
+            self, shareable_type, shareable_id, text, font_size, color, group_id
         )
 
     def create_thread_post(
-            self,
-            post_id: int,
-            text: str = None,
-            font_size: int = None,
-            color: int = None,
-            in_reply_to: int = None,
-            group_id: int = None,
-            mention_ids: List[int] = None,
-            choices: List[str] = None,
-            shared_url: Dict[str, Union[str, int]] = None,
-            message_tags: str = "[]",
-            attachment_filename: str = None,
-            attachment_2_filename: str = None,
-            attachment_3_filename: str = None,
-            attachment_4_filename: str = None,
-            attachment_5_filename: str = None,
-            attachment_6_filename: str = None,
-            attachment_7_filename: str = None,
-            attachment_8_filename: str = None,
-            attachment_9_filename: str = None,
-            video_file_name: str = None,
+        self,
+        post_id: int,
+        text: str = None,
+        font_size: int = None,
+        color: int = None,
+        in_reply_to: int = None,
+        group_id: int = None,
+        mention_ids: List[int] = None,
+        choices: List[str] = None,
+        shared_url: Dict[str, Union[str, int]] = None,
+        message_tags: str = "[]",
+        attachment_filename: str = None,
+        attachment_2_filename: str = None,
+        attachment_3_filename: str = None,
+        attachment_4_filename: str = None,
+        attachment_5_filename: str = None,
+        attachment_6_filename: str = None,
+        attachment_7_filename: str = None,
+        attachment_8_filename: str = None,
+        attachment_9_filename: str = None,
+        video_file_name: str = None,
     ) -> Post:
         """
 
         スレッドの投稿を作成します
 
         """
         return create_thread_post(
@@ -1723,15 +1519,15 @@
             attachment_9_filename,
             video_file_name,
         )
 
     def delete_all_post(self) -> dict:
         """
 
-        すべての投稿を削除します
+        すべての自分の投稿を削除します
 
         """
         return delete_all_post(self)
 
     def unpin_group_post(self, group_id: int) -> dict:
         """
 
@@ -1776,15 +1572,15 @@
 
         """
         return get_timeline_calls(self, **params)
 
     def get_conversation(self, conversation_id: int, **params) -> PostsResponse:
         """
 
-        会話を取得します
+        リプライを含める投稿の会話を取得します
 
         Parameters
         ----------
 
             - conversation_id: int
             - group_id: int = None
             - thread_id: int = None
@@ -1851,15 +1647,17 @@
             - group_id: int
             - from_post: int = None
             - number: int = None
 
         """
         return get_group_highlight_posts(self, group_id, **params)
 
-    def get_group_timeline_by_keyword(self, group_id: int, keyword: str, **params) -> PostsResponse:
+    def get_group_timeline_by_keyword(
+        self, group_id: int, keyword: str, **params
+    ) -> PostsResponse:
         """
 
         グループの投稿をキーワードで検索します
 
         Parameters
         ----------
 
@@ -2053,14 +1851,16 @@
         return get_user_timeline(self, user_id, **params)
 
     def like_posts(self, post_ids: List[int]) -> LikePostsResponse:
         """
 
         投稿にいいねします
 
+        ※ 一度にいいねできる投稿数は最大25個
+
         """
         return like_posts(self, post_ids)
 
     def remove_bookmark(self, user_id: int, post_id: int) -> dict:
         """
 
         ブックマークを削除します
@@ -2081,23 +1881,23 @@
 
         複数の投稿を削除します
 
         """
         return remove_posts(self, post_ids)
 
     def report_post(
-            self,
-            post_id: int,
-            opponent_id: int,
-            category_id: int,
-            reason: str = None,
-            screenshot_filename: str = None,
-            screenshot_2_filename: str = None,
-            screenshot_3_filename: str = None,
-            screenshot_4_filename: str = None
+        self,
+        post_id: int,
+        opponent_id: int,
+        category_id: int,
+        reason: str = None,
+        screenshot_filename: str = None,
+        screenshot_2_filename: str = None,
+        screenshot_3_filename: str = None,
+        screenshot_4_filename: str = None,
     ) -> dict:
         """
 
         投稿を通報します
 
         """
         return report_post(
@@ -2105,62 +1905,39 @@
             post_id,
             opponent_id,
             category_id,
             reason,
             screenshot_filename,
             screenshot_2_filename,
             screenshot_3_filename,
-            screenshot_4_filename
+            screenshot_4_filename,
         )
 
     def unlike_post(self, post_id: int) -> dict:
         """
 
         投稿のいいねを解除します
 
         """
         return unlike_post(self, post_id)
 
     def update_post(
-            self,
-            post_id: int,
-            text: str = None,
-            font_size: int = None,
-            color: int = None,
-            message_tags: str = "[]",
+        self,
+        post_id: int,
+        text: str = None,
+        font_size: int = None,
+        color: int = None,
+        message_tags: str = "[]",
     ) -> Post:
         """
 
         投稿を編集します
 
         """
-        return update_post(
-            self, post_id, text, font_size, color, message_tags
-        )
-
-    # def update_recommendation_feedback(
-    #     self, post_id: int, feedback_result: str,
-    #     experiment_num: int, variant_num: int,
-    # ) -> dict:
-    #     """
-
-    #     おすすめのフィードバックを更新します
-
-    #     """
-    #     return update_recommendation_feedback(
-    #         self, post_id, feedback_result, experiment_num, variant_num
-    #     )
-
-    def validate_post(self, text: str, *, group_id: int = None, thread_id: int = None) -> ValidationPostResponse:
-        """
-
-        与えられたテキストが有効な投稿であるかどうかを検証します
-
-        """
-        return validate_post(self, text, group_id, thread_id)
+        return update_post(self, post_id, text, font_size, color, message_tags)
 
     def view_video(self, video_id: int) -> dict:
         """
 
         動画を視聴します
 
         """
@@ -2213,15 +1990,15 @@
 
         """
         return get_my_reviews(self, **params)
 
     def get_reviews(self, user_id: int, **params) -> ReviewsResponse:
         """
 
-        受け取ったレターを取得します
+        ユーザーが受け取ったレターを取得します
 
         Parameters
         ----------
 
             - user_id: int (required)
             - from_id: int = (optional)
             - number: int = (optional)
@@ -2236,15 +2013,15 @@
 
         """
         return pin_review(self, review_id)
 
     def unpin_review(self, review_id: int) -> dict:
         """
 
-        レターのピンを解除します
+        レターのピン止めを解除します
 
         """
         return unpin_review(self, review_id)
 
     # -THREAD
 
     def add_post_to_thread(self, post_id: int, thread_id: int) -> ThreadInfo:
@@ -2252,50 +2029,36 @@
 
         投稿をスレッドに追加します
 
         """
         return add_post_to_thread(self, post_id, thread_id)
 
     def convert_post_to_thread(
-            self,
-            post_id: int,
-            title: str = None,
-            thread_icon_filename: str = None
+        self, post_id: int, title: str = None, thread_icon_filename: str = None
     ) -> ThreadInfo:
         """
 
         投稿をスレッドに変換します
 
         """
-        return convert_post_to_thread(
-            self,
-            post_id,
-            title,
-            thread_icon_filename
-        )
+        return convert_post_to_thread(self, post_id, title, thread_icon_filename)
 
     def create_thread(
-            self,
-            group_id: int,
-            title: str,
-            thread_icon_filename: str
+        self, group_id: int, title: str, thread_icon_filename: str
     ) -> ThreadInfo:
         """
 
         スレッドを作成します
 
         """
-        return create_thread(
-            self,
-            group_id,
-            title,
-            thread_icon_filename
-        )
+        return create_thread(self, group_id, title, thread_icon_filename)
 
-    def get_group_thread_list(self, group_id: int, from_str: str = None, **params) -> GroupThreadListResponse:
+    def get_group_thread_list(
+        self, group_id: int, from_str: str = None, **params
+    ) -> GroupThreadListResponse:
         """
 
         グループのスレッド一覧を取得します
 
         Parameters
         ----------
 
@@ -2310,15 +2073,17 @@
         """
 
         スレッド参加ステータスを取得します
 
         """
         return get_thread_joined_statuses(self, ids)
 
-    def get_thread_posts(self, thread_id: int, from_str: str = None, **params) -> PostsResponse:
+    def get_thread_posts(
+        self, thread_id: int, from_str: str = None, **params
+    ) -> PostsResponse:
         """
 
         スレッドの投稿を取得します
 
         Parameters
         ----------
 
@@ -2350,41 +2115,25 @@
 
         スレッドを削除します
 
         """
         return remove_thread(self, thread_id)
 
     def update_thread(
-            self,
-            thread_id: int,
-            title: str,
-            thread_icon_filename: str
+        self, thread_id: int, title: str, thread_icon_filename: str
     ) -> dict:
         """
 
         スレッドを編集します
 
         """
-        return update_thread(
-            self,
-            thread_id,
-            title,
-            thread_icon_filename
-        )
+        return update_thread(self, thread_id, title, thread_icon_filename)
 
     # -USER
 
-    # def delete_contact_friends(self) -> dict:
-    #     """
-
-    #     連絡先の友人を削除します
-
-    #     """
-    #     return delete_contact_friends(self)
-
     def delete_footprint(self, user_id: int, footprint_id: int) -> dict:
         """
 
         足跡を削除します
 
         """
         return delete_footprint(self, user_id, footprint_id)
@@ -2423,26 +2172,14 @@
 
             - only_online: bool
             - from_loggedin_at: int = None
 
         """
         return get_active_followings(self, **params)
 
-    # def get_additional_settings(self) -> Settings:
-    #     return get_additional_settings(self)
-
-    # def get_app_review_status(self) -> AppReviewStatusResponse:
-    #     return get_app_review_status(self)
-
-    # def get_contact_status(self, mobile_numbers: List[str]) -> ContactStatusResponse:
-    #     return get_contact_status(self, mobile_numbers)
-
-    # def get_default_settings(self) -> TimelineSettings:
-    #     return get_default_settings(self)
-
     def get_follow_recommendations(self, **params) -> FollowRecommendationsResponse:
         """
 
         フォローするのにおすすめのユーザーを取得します
 
         Parameters
         ----------
@@ -2450,15 +2187,17 @@
             - from_timestamp: int = None,
             - number: int = None,
             - sources: List[str] = None
 
         """
         return get_follow_recommendations(self, **params)
 
-    def get_follow_request(self, from_timestamp: int = None) -> UsersByTimestampResponse:
+    def get_follow_request(
+        self, from_timestamp: int = None
+    ) -> UsersByTimestampResponse:
         """
 
         フォローリクエストを取得します
 
         """
         return get_follow_request(self, from_timestamp)
 
@@ -2490,61 +2229,75 @@
             - number: int = None
             - mode: str = None
 
         """
         return get_footprints(self, **params)
 
     def get_fresh_user(self, user_id: int) -> UserResponse:
+        """
+
+        認証情報などを含んだユーザー情報を取得します
+
+        """
         return get_fresh_user(self, user_id)
 
     def get_hima_users(self, **params) -> List[UserWrapper]:
         """
 
-        暇なユーザーを取得する
+        暇なユーザーを取得します
 
         Parameters
         ----------
 
             - from_hima_id: int = None
             - number: int = None
 
         """
         return get_hima_users(self, **params)
 
-    # def get_initial_recommended_users_to_follow(self, **params) -> UsersResponse:
-    #     return get_initial_recommended_users_to_follow(self, **params)
+    def get_user_ranking(self, mode: str) -> RankingUsersResponse:
+        """
+
+        ユーザーのフォロワーランキングを取得します
+
+        Examples:
+        --------
+
+        >>> ルーキーを取得する場合:
+
+        >>> api.get_user_ranking(mode="one_month")
+
+        ---
+
+        >>> ミドルを取得する場合:
+
+        >>> api.get_user_ranking(mode="six_months")
+
+        ---
+
+        >>> 殿堂入りを取得する場合:
 
-    # def get_recommended_users_to_follow_for_profile(
-    #         self, user_id: int, **params
-    # ) -> UsersResponse:
-    #     """
-
-    #     Parameters
-    #     ----------
-
-    #         - user_id: int - (Required)
-    #         - number: int - (Optional)
-    #         - page: int - (Optional)
-
-    #     """
-    #     return get_recommended_users_to_follow_for_profile(
-    #         self, user_id, **params
-    #     )
+        >>> api.get_user_ranking(mode="all_time")
+
+        """
+        return get_user_ranking(self, mode)
 
     def get_refresh_counter_requests(self) -> RefreshCounterRequestsResponse:
         """
 
         カウンター更新のリクエストを取得します
 
         """
         return get_refresh_counter_requests(self)
 
     def get_social_shared_users(self, **params) -> SocialShareUsersResponse:
         """
 
+        SNS共有をしたユーザーを取得します
+
         Parameters
         ----------
 
             - sns_name: str - (Required)
             - number: int - (Optional)
             - from_id: int - (Optional)
 
@@ -2563,17 +2316,14 @@
         """
 
         ユーザーの情報を取得します
 
         """
         return get_user(self, user_id)
 
-    # def get_user_custom_definitions(self) -> UserCustomDefinitionsResponse:
-    #     return get_user_custom_definitions(self)
-
     def get_user_email(self, user_id: int) -> str:
         """
 
         ユーザーのメールアドレスを取得します
 
         """
         return get_user_email(self, user_id)
@@ -2613,45 +2363,30 @@
         """
 
         QRコードからユーザーを取得します
 
         """
         return get_user_from_qr(self, qr)
 
-    # def get_user_interests(self) -> dict:
-    #     return get_user_interests(self)
-
     def get_user_without_leaving_footprint(self, user_id: int) -> UserResponse:
         """
-        ユーザーの情報を取得します
+
+        足跡をつけずにユーザーの情報を取得します
+
         """
         return get_user_without_leaving_footprint(self, user_id)
 
     def get_users(self, user_ids: List[int]) -> UsersResponse:
         """
 
         複数のユーザーの情報を取得します
 
         """
         return get_users(self, user_ids)
 
-    # def get_users_from_uuid(self, uuid: str) -> UsersResponse:
-    #     """
-
-    #     UUIDからユーザーを取得します
-
-    #     """
-    #     return get_users_from_uuid(self, uuid)
-
-    def post_social_shared(self, sns_name: str) -> dict:
-        return post_social_shared(self, sns_name)
-
-    # def record_app_review_status(self) -> dict:
-    #     return record_app_review_status(self)
-
     def reduce_kenta_penalty(self, user_id: int) -> dict:
         """
 
         ペナルティーを緩和します
 
         """
         return reduce_kenta_penalty(self, user_id)
@@ -2677,37 +2412,37 @@
 
         ユーザーのカバー画像を削除します
 
         """
         return remove_user_cover(self)
 
     def report_user(
-            self,
-            user_id: int,
-            category_id: int,
-            reason: str = None,
-            screenshot_filename: str = None,
-            screenshot_2_filename: str = None,
-            screenshot_3_filename: str = None,
-            screenshot_4_filename: str = None
+        self,
+        user_id: int,
+        category_id: int,
+        reason: str = None,
+        screenshot_filename: str = None,
+        screenshot_2_filename: str = None,
+        screenshot_3_filename: str = None,
+        screenshot_4_filename: str = None,
     ) -> dict:
         """
 
         ユーザーを通報します
 
         """
         return report_user(
             self,
             user_id,
             category_id,
             reason,
             screenshot_filename,
             screenshot_2_filename,
             screenshot_3_filename,
-            screenshot_4_filename
+            screenshot_4_filename,
         )
 
     def reset_password(self, email: str, email_grant_token: str, password: str) -> dict:
         """
 
         パスワードをリセットします
 
@@ -2723,15 +2458,15 @@
         ----------
 
             - nickname: str = None
             - number: int = None
             - from_str: str = None
 
         """
-        return search_lobi_users(self ** params)
+        return search_lobi_users(self**params)
 
     def search_users(self, **params) -> UsersResponse:
         """
 
         ユーザーを検索します
 
         Parameters
@@ -2747,24 +2482,23 @@
             - recently_created: bool = None
             - same_prefecture: bool = None
             - save_recent_search: bool = None
 
         """
         return search_users(self, **params)
 
-    # def set_additional_setting_enabled(self, mode: str, on: int = None) -> dict:
-    #     return set_additional_setting_enabled(self, mode, on)
-
     def set_follow_permission_enabled(
-            self, nickname: str, is_private: bool = None
+        self, nickname: str, is_private: bool = None
     ) -> dict:
-        return set_follow_permission_enabled(self, nickname, is_private)
+        """
 
-    # def set_setting_follow_recommendation_enabled(self, on: bool) -> dict:
-    #     return set_setting_follow_recommendation_enabled(self, on)
+        フォローを許可制に設定します
+
+        """
+        return set_follow_permission_enabled(self, nickname, is_private)
 
     def take_action_follow_request(self, target_id: int, action: str) -> dict:
         return take_action_follow_request(self, target_id, action)
 
     def turn_on_hima(self) -> dict:
         """
 
@@ -2777,60 +2511,42 @@
         """
 
         ユーザーをアンフォローします
 
         """
         return unfollow_user(self, user_id)
 
-    # def update_invite_contact_status(self, mobile_number: str) -> dict:
-    #     return update_invite_contact_status(self, mobile_number)
-
-    def update_language(self, language: str) -> dict:
-        """
-
-        言語を更新します
-
-        """
-        return update_language(self, language)
-
     def update_user(
-            self,
-            nickname: str,
-            biography: str = None,
-            prefecture: str = None,
-            gender: int = None,
-            country_code: str = None,
-            profile_icon_filename: str = None,
-            cover_image_filename: str = None,
-            username: str = None,
+        self,
+        nickname: str,
+        biography: str = None,
+        prefecture: str = None,
+        gender: int = None,
+        country_code: str = None,
+        profile_icon_filename: str = None,
+        cover_image_filename: str = None,
+        username: str = None,
     ) -> dict:
         """
 
         プロフィールを更新します
 
         """
         return update_user(
-            self, nickname, biography, prefecture, gender, country_code,
-            profile_icon_filename, cover_image_filename, username
+            self,
+            nickname,
+            biography,
+            prefecture,
+            gender,
+            country_code,
+            profile_icon_filename,
+            cover_image_filename,
+            username,
         )
 
-    # def update_user_interests(self) -> dict:
-    #     return update_user_interests(self)
-
-    # def upload_contacts_friends(self) -> dict:
-    #     return upload_contacts_friends(self)
-
-    # def upload_twitter_friend_ids(self, twitter_friend_ids: List[str]) -> dict:
-    #     """
-
-    #     TwitterのフレンドのIDをアップロードします
-
-    #     """
-    #     return upload_twitter_friend_ids(self, twitter_friend_ids)
-
     def block_user(self, user_id: int) -> dict:
         """
 
         ユーザーをブロックします
 
         """
         return block_user(self, user_id)
```

### Comparing `yaylib-0.1.3/yaylib/config.py` & `yaylib-0.1.5/yaylib/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from enum import Enum
 
 
 class Configs:
-
-    YAYLIB_VERSION = "0.1.3"
+    YAYLIB_VERSION = "0.1.5"
     YAY_API_VERSION = "3.16"
     YAY_VERSION_NAME = "3.16.1"
     YAY_API_VERSION_KEY = "e83a1d2588918c2061280427c88e6f56"
     YAY_API_KEY = "ccd59ee269c01511ba763467045c115779fcae3050238a252f1bd1a4b65cfec6"
     YAY_SHARED_KEY = "yayZ1"
     YAY_STORE_KEY = "yayZ1payment"
     ID_CARD_CHECK_SECRET_KEY = "4aa6d1c301a97154bc1098c2"
@@ -24,20 +23,19 @@
         "Host": YAY_PRODUCTION_HOST,
         "X-App-Version": YAY_API_VERSION,
         "User-Agent": USER_AGENT,
         "X-Device-Info": f"yay {YAY_VERSION_NAME} {USER_AGENT}",
         "X-Device-Uuid": "",
         "X-Connection-Type": "wifi",
         "Accept-Language": "ja",
-        "Content-Type": "application/json;charset=UTF-8"
+        "Content-Type": "application/json;charset=UTF-8",
     }
 
 
 class Endpoints:
-
     # api v1 endpoints
     USERS_V1 = Configs.YAY_API_URL + "/v1/users"
     PAYMENTS_V1 = Configs.YAY_API_URL + "/v1/payments"
     THREADS_V1 = Configs.YAY_API_URL + "/v1/threads"
     PINNED_V1 = Configs.YAY_API_URL + "/v1/pinned"
     POSTS_V1 = Configs.YAY_API_URL + "/v1/posts"
     CONVERSATIONS_V1 = Configs.YAY_API_URL + "/v1/conversations"
@@ -56,14 +54,15 @@
     EMAIL_VERIFICATION_URL_V1 = Configs.YAY_API_URL + "/v1/email_verification_urls"
     BUCKETS_V1 = Configs.YAY_API_URL + "/v1/buckets"
     ID_CHECK_V1 = Configs.YAY_API_URL + "/v1/id_check"
     PROMOTIONS_V1 = Configs.YAY_API_URL + "/v1/promotions"
     SKYFALL_V1 = Configs.YAY_API_URL + "/v1/skyfall"
     GENUINE_DEVICES_V1 = Configs.YAY_API_URL + "/v1/genuine_devices"
     LOBI_FRIENDS_V1 = Configs.YAY_API_URL + "/v1/lobi_friends"
+    WEB_V1 = Configs.YAY_API_URL + "/v1/web"
 
     # api v2 endpoints
     USERS_V2 = Configs.YAY_API_URL + "/v2/users"
     PAYMENTS_V2 = Configs.YAY_API_URL + "/v2/payments"
     THREADS_V2 = Configs.YAY_API_URL + "/v2/threads"
     PINNED_V2 = Configs.YAY_API_URL + "/v2/pinned"
     POSTS_V2 = Configs.YAY_API_URL + "/v2/posts"
@@ -83,14 +82,15 @@
     EMAIL_VERIFICATION_URL_V2 = Configs.YAY_API_URL + "/v2/email_verification_urls"
     BUCKETS_V2 = Configs.YAY_API_URL + "/v2/buckets"
     ID_CHECK_V2 = Configs.YAY_API_URL + "/v2/id_check"
     PROMOTIONS_V2 = Configs.YAY_API_URL + "/v2/promotions"
     SKYFALL_V2 = Configs.YAY_API_URL + "/v2/skyfall"
     GENUINE_DEVICES_V2 = Configs.YAY_API_URL + "/v2/genuine_devices"
     LOBI_FRIENDS_V2 = Configs.YAY_API_URL + "/v2/lobi_friends"
+    WEB_V2 = Configs.YAY_API_URL + "/v2/web"
 
     # api v3 endpoints
     USERS_V3 = Configs.YAY_API_URL + "/v3/users"
     PAYMENTS_V3 = Configs.YAY_API_URL + "/v3/payments"
     THREADS_V3 = Configs.YAY_API_URL + "/v3/threads"
     PINNED_V3 = Configs.YAY_API_URL + "/v3/pinned"
     POSTS_V3 = Configs.YAY_API_URL + "/v3/posts"
@@ -110,22 +110,25 @@
     EMAIL_VERIFICATION_URL_V3 = Configs.YAY_API_URL + "/v3/email_verification_urls"
     BUCKETS_V3 = Configs.YAY_API_URL + "/v3/buckets"
     ID_CHECK_V3 = Configs.YAY_API_URL + "/v3/id_check"
     PROMOTIONS_V3 = Configs.YAY_API_URL + "/v3/promotions"
     SKYFALL_V3 = Configs.YAY_API_URL + "/v3/skyfall"
     GENUINE_DEVICES_V3 = Configs.YAY_API_URL + "/v3/genuine_devices"
     LOBI_FRIENDS_V3 = Configs.YAY_API_URL + "/v3/lobi_friends"
+    WEB_V3 = Configs.YAY_API_URL + "/v3/web"
 
     # misc
-    GET_EMAIL_GRANT_TOKEN = "https://" + Configs.ID_CARD_CHECK_HOST_PRODUCTION + \
-        "/apis/v1/apps/yay/email_grant_tokens"
+    GET_EMAIL_GRANT_TOKEN = (
+        "https://"
+        + Configs.ID_CARD_CHECK_HOST_PRODUCTION
+        + "/apis/v1/apps/yay/email_grant_tokens"
+    )
 
 
 class ErrorType(Enum):
-
     Unknown = "unknown"
     InvalidParameter = -1
     RegisteredUser = -2
     AccessTokenExpired = -3
     ScreenNameAlreadyBeenTaken = -4
     UserNotFound = -5
     PostNotFound = -6
@@ -215,18 +218,18 @@
     PasswordTooLong = -408
     PasswordNotAllowed = -409
     CommonPassword = -410
     UnableToMovePostToThread = -412
     UnableToPostUrl = -413
     UnableToSetCall = -977
     PhoneNumberBanned = -1000
+    TooManyRequests = -5302
 
 
 class ErrorMessage(Enum):
-
     Unknown = "原因不明"
     # InvalidParameter = "引数が不正です"
     RegisteredUser = "このアカウントはすでに登録されています"
     AccessTokenExpired = "アクセストークンの有効期限切れ"
     ScreenNameAlreadyBeenTaken = "このIDはすでに使われています"
     UserNotFound = "ユーザーが見つかりません"
     PostNotFound = "投稿が見つかりません"
@@ -280,15 +283,17 @@
     SnsShareRewardAlreadyBeenClaimed = "SNS共有の特典は既に取得済みです"
     QuotaLimitExceeded = "この機能の上限回数に達しました。1時間ほど時間を置いて再度お試しください。"
     ChatNeedAgeVerified = "チャット送信に年齢確認が必要です"
     OnlyAgeVerifiedUserCanJoinGroup = "このサークルに参加するには年齢確認をする必要があります"
     RequirePhoneVerificationToChat = "チャットをするには電話番号認証が必要です"
     NotPostOwner = "編集は投稿の作成者のみ可能です"
     GroupGenerationNotMatched = "特定の年齢層のみ参加が許可されているサークルです"
-    PhoneNumberCheckVerificationCodeSubmitQuotaExceeded = "認証コードの送信回数が上限を越えました。1時間ほど時間をおいて再度お試しください"
+    PhoneNumberCheckVerificationCodeSubmitQuotaExceeded = (
+        "認証コードの送信回数が上限を越えました。1時間ほど時間をおいて再度お試しください"
+    )
     PhoneNumberCheckVerificationCodeRequestQuotaExceeded = "チャットをするには電話番号認証が必要です"
     GroupOfferHasBeenAccepted = "サークルの招待は承諾されています"
     GroupOfferHasBeenWithdrawn = "サークルの招待は拒否されています"
     IpBanned = "IPがBanされました"
     NotConnectedToTwitter = "Twitterに接続されていません"
     PrivateUserTimeline = "フォロワーにのみ投稿を公開しています"
     CounterRefreshLimitExceeded = "カウンター更新の回数制限に達しました"
@@ -316,7 +321,8 @@
     PasswordTooLong = "パスワードが長すぎます"
     PasswordNotAllowed = "他のパスワードを使用してください。無効な文字列が含まれています"
     CommonPassword = "他のパスワードを使用してください。文字列や数字、または記号などの組み合わせをお試しください"
     UnableToMovePostToThread = "投稿をスレッドに移動できません"
     UnableToPostUrl = "URLを投稿できません"
     UnableToSetCall = "通話を開始できませんでした"
     PhoneNumberBanned = "電話番号がBanされています"
+    TooManyRequests = "リクエストが多すぎます"
```

### Comparing `yaylib-0.1.3/yaylib/models.py` & `yaylib-0.1.5/yaylib/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 from .utils import parse_datetime
 
 
 class Activity:
-
     __slots__ = (
-        "data", "id", "created_at", "created_at_parsed", "type", "user", "from_post",
-        "to_post", "group", "followers", "from_post_ids", "vip_reward",
+        "data",
+        "id",
+        "created_at",
+        "created_at_parsed",
+        "type",
+        "user",
+        "from_post",
+        "to_post",
+        "group",
+        "followers",
+        "from_post_ids",
+        "vip_reward",
         "is_bulk_invitation",
     )
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.created_at = data.get("created_at")
@@ -30,57 +39,52 @@
 
         self.group = data.get("group")
         if self.group is not None:
             self.group = Group(self.group)
 
         self.followers = data.get("followers")
         if self.followers is not None:
-            self.followers = [
-                User(follower) for follower in self.followers
-            ]
+            self.followers = [User(follower) for follower in self.followers]
 
         self.from_post_ids = data.get("from_post_ids")
         self.vip_reward = data.get("vip_reward")
         self.is_bulk_invitation = data.get("is_bulk_invitation")
 
     def __repr__(self):
         return f"Activity(data={self.data})"
 
 
 class BanWord:
-
     __slots__ = ("data", "id", "type", "word")
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.type = data.get("type")
         self.word = data.get("word")
 
     def __repr__(self):
         return f"BanWord(data={self.data})"
 
 
 class Bgm:
-
     __slots__ = ("data", "id", "title", "music_url", "order")
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.title = data.get("title")
         self.music_url = data.get("music_url")
         self.order = data.get("order")
 
     def __repr__(self):
         return f"Bgm(data={self.data})"
 
 
 class CallGiftHistory:
-
     __slots__ = ("data", "gifts_count", "sent_at", "sent_at_parsed", "sender")
 
     def __init__(self, data):
         self.data = data
 
         self.gifts_count = data.get("gifts_count")
         if self.gifts_count is not None:
@@ -96,32 +100,40 @@
             self.sender = User(self.sender)
 
     def __repr__(self):
         return f"CallGiftHistory(data={self.data})"
 
 
 class ChatRoom:
-
     __slots__ = (
-        "data", "id", "unread_count", "updated_at", "updated_at_parsed", "members",
-        "background", "last_message", "name", "is_group", "owner", "is_request", "user_setting"
+        "data",
+        "id",
+        "unread_count",
+        "updated_at",
+        "updated_at_parsed",
+        "members",
+        "background",
+        "last_message",
+        "name",
+        "is_group",
+        "owner",
+        "is_request",
+        "user_setting",
     )
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.unread_count = data.get("unread_count")
         self.updated_at = data.get("updated_at")
         self.updated_at_parsed = parse_datetime(data.get("updated_at"))
 
         self.members = data.get("members")
         if self.members is not None:
-            self.members = [
-                User(member) for member in self.members
-            ]
+            self.members = [User(member) for member in self.members]
 
         self.background = data.get("background")
 
         self.last_message = data.get("last_message")
         if self.last_message is not None:
             self.last_message = Message(self.last_message)
 
@@ -139,111 +151,116 @@
         #     self.user_setting = UserSetting(self.user_setting)
 
     def __repr__(self):
         return f"ChatRoom(data={self.data})"
 
 
 class ChatRoomDraft:
-
     __slots__ = ("data", "id", "text")
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.text = data.get("text")
 
     def __repr__(self):
         return f"ChatRoomDraft(data={self.data})"
 
 
 class Choice:
-
     __slots__ = ("data", "id", "label", "votes_count")
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.label = data.get("label")
         self.votes_count = data.get("votes_count")
 
     def __repr__(self):
         return f"Choice(data={self.data})"
 
 
 class CoinAmount:
-
     __slots__ = ("data", "paid", "free", "total")
 
     def __init__(self, data):
         self.data = data
         self.paid = data.get("paid")
         self.free = data.get("free")
         self.total = data.get("total")
 
     def __repr__(self):
         return f"CoinAmount(data={self.data})"
 
 
 class CoinExpiration:
-
     __slots__ = ("data", "expired_at", "amount")
 
     def __init__(self, data):
         self.data = data
         self.expired_at = data.get("expired_at")
         self.amount = data.get("amount")
 
     def __repr__(self):
         return f"CoinExpiration(data={self.data})"
 
 
 class CoinProduct:
-
     __slots__ = ("data", "id", "purchasable", "amount")
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.purchasable = data.get("purchasable")
         self.amount = data.get("amount")
 
     def __repr__(self):
         return f"CoinProduct(data={self.data})"
 
 
 class CoinProductQuota:
-
     __slots__ = ("data", "bought", "limit")
 
     def __init__(self, data):
         self.data = data
         self.bought = data.get("bought")
         self.limit = data.get("limit")
 
     def __repr__(self):
         return f"CoinProductQuota(data={self.data})"
 
 
 class ConferenceCall:
-
     __slots__ = (
-        "data", "id", "post_id", "group_id", "is_active",
-        "anonymous_call_users_count", "agora_channel", "agora_token", "call_type",
-        "joinable_by", "game", "genre", "duration_seconds", "max_participants",
-        "conference_call_users", "bump_params", "conference_call_users_role"
+        "data",
+        "id",
+        "post_id",
+        "group_id",
+        "is_active",
+        "anonymous_call_users_count",
+        "agora_channel",
+        "agora_token",
+        "call_type",
+        "joinable_by",
+        "game",
+        "genre",
+        "duration_seconds",
+        "max_participants",
+        "conference_call_users",
+        "bump_params",
+        "conference_call_users_role",
     )
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.post_id = data.get("post_id")
         self.group_id = data.get("group_id")
         self.is_active = data.get("is_active")
-        self.anonymous_call_users_count = data.get(
-            "anonymous_call_users_count")
+        self.anonymous_call_users_count = data.get("anonymous_call_users_count")
         self.agora_channel = data.get("agora_channel")
         self.agora_token = data.get("agora_token")
         self.call_type = data.get("call_type")
         self.joinable_by = data.get("joinable_by")
 
         self.game = data.get("game")
         if self.game is not None:
@@ -255,106 +272,103 @@
 
         self.duration_seconds = data.get("duration_seconds")
         self.max_participants = data.get("max_participants")
 
         self.conference_call_users = data.get("conference_call_users")
         if self.conference_call_users is not None:
             self.conference_call_users = [
-                User(conference_call_user) for conference_call_user in self.conference_call_users
+                User(conference_call_user)
+                for conference_call_user in self.conference_call_users
             ]
 
         self.bump_params = data.get("bump_params")
         # if self.bump_params is not None:
         #     self.bump_params = BumpParams(self.bump_params)
 
         self.conference_call_users_role = data.get("conference_call_usersRole")
         if self.conference_call_users_role is not None:
             self.conference_call_users_role = [
-                ConferenceCallUserRole(conference_call_user_role) for conference_call_user_role in self.conference_call_users_role
+                ConferenceCallUserRole(conference_call_user_role)
+                for conference_call_user_role in self.conference_call_users_role
             ]
 
     def __repr__(self):
         return f"ConferenceCall(data={self.data})"
 
 
 class ConferenceCallUserRole:
-
     __slots__ = ("data", "id", "role")
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.role = data.get("role")
 
     def __repr__(self):
         return f"ConferenceCallUserRole(data={self.data})"
 
 
 class ContactStatus:
-
     __slots__ = ("data", "status", "user_id")
 
     def __init__(self, data):
         self.data = data
         self.status = data.get("status")
         self.user_id = data.get("user_id")
 
     def __repr__(self):
         return f"ContactStatus(data={self.data})"
 
 
 class CreateGroupQuota:
-
     __slots__ = ("data", "used_quota", "remaining_quota")
 
     def __init__(self, data):
         self.data = data
         self.used_quota = data.get("used_quota")
         self.remaining_quota = data.get("remaining_quota")
 
     def __repr__(self):
         return f"CreateGroupQuota(data={self.data})"
 
 
 class TimelineSettings:
-
     __slots__ = (
-        "data", "hide_hot_post", "hide_reply_public_timeline",
-        "hide_reply_following_timeline", "faves_filter"
+        "data",
+        "hide_hot_post",
+        "hide_reply_public_timeline",
+        "hide_reply_following_timeline",
+        "faves_filter",
     )
 
     def __init__(self, data):
         self.data = data
         self.hide_hot_post = data.get("hide_hot_post")
-        self.hide_reply_public_timeline = data.get(
-            "hide_reply_public_timeline")
-        self.hide_reply_following_timeline = data.get(
-            "hide_reply_following_timeline")
+        self.hide_reply_public_timeline = data.get("hide_reply_public_timeline")
+        self.hide_reply_following_timeline = data.get("hide_reply_following_timeline")
         self.faves_filter = data.get("faves_filter")
 
     def __repr__(self):
         return f"TimelineSettings(data={self.data})"
 
 
 class Error:
-
     __slots__ = ("data", "throwable", "type", "action")
 
     def __init__(self, data):
         self.data = data
         self.throwable = data.get("throwable")
         self.type = data.get("type")
         self.action = data.get("action")
 
     def __repr__(self):
         return f"Error(data={self.data})"
 
 
 class Footprint:
-
     __slots__ = ("data", "user", "visited_at", "visited_at_parsed", "id")
 
     def __init__(self, data):
         self.data = data
 
         self.user = data.get("user")
         if self.user is not None:
@@ -365,15 +379,14 @@
         self.id = data.get("id")
 
     def __repr__(self):
         return f"Footprint(data={self.data})"
 
 
 class Game:
-
     __slots__ = ("data", "id", "type", "title", "icon_url", "platform_details")
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.type = data.get("type")
         self.title = data.get("title")
@@ -384,65 +397,59 @@
             self.platform_details = PlatformDetails(self.platform_details)
 
     def __repr__(self):
         return f"Game(data={self.data})"
 
 
 class Genre:
-
     __slots__ = ("data", "id", "type", "title", "icon_url")
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.type = data.get("type")
         self.title = data.get("title")
         self.icon_url = data.get("icon_url")
 
     def __repr__(self):
         return f"Genre(data={self.data})"
 
 
 class GifImage:
-
     __slots__ = ("data", "id", "url", "width", "height")
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.url = data.get("url")
         self.width = data.get("width")
         self.height = data.get("height")
 
     def __repr__(self):
         return f"GifImage(data={self.data})"
 
 
 class GifImageCategory:
-
     __slots__ = ("data", "id", "name", "language", "gifs")
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.name = data.get("name")
         self.language = data.get("language")
 
         self.gifs = data.get("gifs")
         if self.gifs is not None:
-            self.gifs = [
-                GifImage(gif) for gif in self.gifs
-            ]
+            self.gifs = [GifImage(gif) for gif in self.gifs]
 
     def __repr__(self):
         return f"GifImageCategory(data={self.data})"
 
 
 class Gift:
-
     __slots__ = ("data", "id", "title", "icon", "iconThumbnail", "price")
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.type = data.get("title")
         self.title = data.get("icon")
@@ -450,80 +457,108 @@
         self.icon_url = data.get("price")
 
     def __repr__(self):
         return f"Gift(data={self.data})"
 
 
 class GiftCount:
-
     __slots__ = ("data", "id", "quantity")
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.quantity = data.get("quantity")
 
     def __repr__(self):
         return f"GiftCount(data={self.data})"
 
 
 class GiftHistory:
-
     __slots__ = ("data", "transaction_at_seconds", "user", "gifts")
 
     def __init__(self, data):
         self.data = data
         self.transaction_at_seconds = data.get("transaction_at_seconds")
 
         self.user = data.get("user")
         if self.user is not None:
             self.user = User(self.user)
 
         self.gifts = data.get("gifts")
         if self.gifts is not None:
-            self.gifts = [
-                ReceivedGift(gift) for gift in self.gifts
-            ]
+            self.gifts = [ReceivedGift(gift) for gift in self.gifts]
 
     def __repr__(self):
         return f"GiftHistory(data={self.data})"
 
 
 class GiftingAbility:
-
     __slots__ = ("data", "user_id", "enabled", "can_send", "can_receive")
 
     def __init__(self, data):
         self.data = data
         self.user_id = data.get("user_id")
         self.enabled = data.get("enabled")
         self.can_send = data.get("can_send")
         self.can_receive = data.get("can_receive")
 
     def __repr__(self):
         return f"GiftingAbility(data={self.data})"
 
 
 class Group:
-
     __slots__ = (
-        "data", "id", "topic", "description", "user_id", "groups_users_count",
-        "posts_count", "threads_count", "highlighted_count", "views_count",
-        "related_count", "secret", "gender", "hide_reported_posts",
-        "hide_conference_call", "is_private", "only_verified_age",
-        "only_mobile_verified", "call_timeline_display", "updated_at", "updated_at_parsed",
-        "cover_image", "cover_image_thumbnail", "generation_groups_limit",
-        "owner", "is_joined", "is_pending", "group_category_id",
-        "unread_counts", "moderator_ids", "seizable", "seizable_before",
-        "pending_count", "pending_transfer_id", "pending_deputize_ids",
-        "safe_mode", "is_related", "allow_ownership_transfer",
-        "sub_category_id", "title", "allow_thread_creation_by",
-        "hide_from_game_eight", "walkthrough_requested",
-        "unread_threads_count", "allow_members_to_post_image_and_video",
-        "allow_members_to_post_url", "guidelines", "invited_to_join"
+        "data",
+        "id",
+        "topic",
+        "description",
+        "user_id",
+        "groups_users_count",
+        "posts_count",
+        "threads_count",
+        "highlighted_count",
+        "views_count",
+        "related_count",
+        "secret",
+        "gender",
+        "hide_reported_posts",
+        "hide_conference_call",
+        "is_private",
+        "only_verified_age",
+        "only_mobile_verified",
+        "call_timeline_display",
+        "updated_at",
+        "updated_at_parsed",
+        "cover_image",
+        "cover_image_thumbnail",
+        "generation_groups_limit",
+        "owner",
+        "is_joined",
+        "is_pending",
+        "group_category_id",
+        "unread_counts",
+        "moderator_ids",
+        "seizable",
+        "seizable_before",
+        "pending_count",
+        "pending_transfer_id",
+        "pending_deputize_ids",
+        "safe_mode",
+        "is_related",
+        "allow_ownership_transfer",
+        "sub_category_id",
+        "title",
+        "allow_thread_creation_by",
+        "hide_from_game_eight",
+        "walkthrough_requested",
+        "unread_threads_count",
+        "allow_members_to_post_image_and_video",
+        "allow_members_to_post_url",
+        "guidelines",
+        "invited_to_join",
     )
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.topic = data.get("topic")
         self.description = data.get("description")
@@ -568,40 +603,39 @@
         self.sub_category_id = data.get("sub_category_id")
         self.title = data.get("title")
         self.allow_thread_creation_by = data.get("allow_thread_creation_by")
         self.hide_from_game_eight = data.get("hide_from_game_eight")
         self.walkthrough_requested = data.get("walkthrough_requested")
         self.unread_threads_count = data.get("unread_threads_count")
         self.allow_members_to_post_image_and_video = data.get(
-            "allow_members_to_post_image_and_video")
+            "allow_members_to_post_image_and_video"
+        )
         self.allow_members_to_post_url = data.get("allow_members_to_post_url")
         self.guidelines = data.get("guidelines")
         self.invited_to_join = data.get("invited_to_join")
 
     def __repr__(self):
         return f"Group(data={self.data})"
 
 
 class GroupCategory:
-
     __slots__ = ("data", "id", "name", "icon", "rank")
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.name = data.get("name")
         self.icon = data.get("icon")
         self.rank = data.get("rank")
 
     def __repr__(self):
         return f"GroupCategory(data={self.data})"
 
 
 class GroupGiftHistory:
-
     __slots__ = ("data", "gifts_count", "received_date", "user")
 
     def __init__(self, data):
         self.data = data
 
         self.gifts_count = data.get("gifts_count")
         if self.gifts_count is not None:
@@ -616,17 +650,21 @@
             self.user = User(self.user)
 
     def __repr__(self):
         return f"GroupGiftHistory(data={self.data})"
 
 
 class GroupUser:
-
     __slots__ = (
-        "data", "user", "is_moderator", "pending_transfer", "pending_deputize", "title"
+        "data",
+        "user",
+        "is_moderator",
+        "pending_transfer",
+        "pending_deputize",
+        "title",
     )
 
     def __init__(self, data):
         self.data = data
 
         self.user = data.get("user")
         if self.user is not None:
@@ -638,44 +676,41 @@
         self.title = data.get("title")
 
     def __repr__(self):
         return f"GroupUser(data={self.data})"
 
 
 class HiddenRecommendedPost:
-
     __slots__ = ("data", "post")
 
     def __init__(self, data):
         self.data = data
         self.post = data.get("post")
         if self.post is not None:
             self.post = Post(self.post)
 
     def __repr__(self):
         return f"HiddenRecommendedPost(data={self.data})"
 
 
 class Interest:
-
     __slots__ = ("data", "id", "name", "icon", "selected")
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.name = data.get("name")
         self.icon = data.get("icon")
         self.selected = data.get("selected")
 
     def __repr__(self):
         return f"Interest(data={self.data})"
 
 
 class Message:
-
     __slots__ = ("data", "id", "user_id", "type", "text", "conference_call")
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.user_id = data.get("user_id")
         self.type = data.get("type")
@@ -686,86 +721,123 @@
             self.conference_call = ConferenceCall(self.conference_call)
 
     def __repr__(self):
         return f"Message(data={self.data})"
 
 
 class MessageTag:
-
     __slots__ = ("data", "user_id", "offset", "length", "type")
 
     def __init__(self, data):
         self.data = data
         self.user_id = data.get("user_id")
         self.offset = data.get("offset")
         self.length = data.get("length")
         self.type = data.get("type")
 
     def __repr__(self):
         return f"MessageTag(data={self.data})"
 
 
 class MuteKeyword:
-
     __slots__ = ("data", "id", "word", "context")
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.word = data.get("word")
         self.context = data.get("context")
 
     def __repr__(self):
         return f"MuteKeyword(data={self.data})"
 
 
 class PlatformDetails:
-
     __slots__ = ("data", "package_id", "affiliate_url")
 
     def __init__(self, data):
         self.data = data
         self.package_id = data.get("package_id")
         self.affiliate_url = data.get("affiliate_url")
 
     def __repr__(self):
         return f"PlatformDetails(data={self.data})"
 
 
 class PopularWord:
-
     __slots__ = ("data", "id", "word", "type")
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.word = data.get("word")
         self.type = data.get("type")
 
     def __repr__(self):
         return f"PopularWord(data={self.data})"
 
 
 class Post:
-
     __slots__ = (
-        "data", "id", "text", "post_type", "group_id", "font_size", "color",
-        "likes_count", "created_at", "updated_at", "updated_at_parsed", "edited_at",
-        "edited_at_parsed", "liked", "tag", "reposts_count", "reposted",
-        "repostable", "reported_count", "conversation_id", "in_reply_to",
-        "in_reply_to_post", "in_reply_to_post_count", "user", "mentions",
-        "group", "conference_call", "attachment", "attachment_thumbnail",
-        "attachment_2", "attachment_2_thumbnail", "attachment_3",
-        "attachment_3_thumbnail", "attachment_4", "attachment_4_thumbnail",
-        "attachment_5", "attachment_5_thumbnail", "attachment_6",
-        "attachment_6_thumbnail", "attachment_7", "attachment_7_thumbnail",
-        "attachment_8", "attachment_8_thumbnail", "attachment_9",
-        "attachment_9_thumbnail", "shareable", "shared_url", "survey", "videos",
-        "gifts_count", "shared_thread", "thread_id", "thread", "highlighted",
-        "message_tags", "is_fail_to_send"
+        "data",
+        "id",
+        "text",
+        "post_type",
+        "group_id",
+        "font_size",
+        "color",
+        "likes_count",
+        "created_at",
+        "updated_at",
+        "updated_at_parsed",
+        "edited_at",
+        "edited_at_parsed",
+        "liked",
+        "tag",
+        "reposts_count",
+        "reposted",
+        "repostable",
+        "reported_count",
+        "conversation_id",
+        "in_reply_to",
+        "in_reply_to_post",
+        "in_reply_to_post_count",
+        "user",
+        "mentions",
+        "group",
+        "conference_call",
+        "attachment",
+        "attachment_thumbnail",
+        "attachment_2",
+        "attachment_2_thumbnail",
+        "attachment_3",
+        "attachment_3_thumbnail",
+        "attachment_4",
+        "attachment_4_thumbnail",
+        "attachment_5",
+        "attachment_5_thumbnail",
+        "attachment_6",
+        "attachment_6_thumbnail",
+        "attachment_7",
+        "attachment_7_thumbnail",
+        "attachment_8",
+        "attachment_8_thumbnail",
+        "attachment_9",
+        "attachment_9_thumbnail",
+        "shareable",
+        "shared_url",
+        "survey",
+        "videos",
+        "gifts_count",
+        "shared_thread",
+        "thread_id",
+        "thread",
+        "highlighted",
+        "message_tags",
+        "is_fail_to_send",
     )
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.text = data.get("text")
         self.post_type = data.get("post_type")
@@ -791,17 +863,15 @@
 
         self.user = data.get("user")
         if self.user is not None:
             self.user = User(self.user)
 
         self.mentions = data.get("mentions")
         if self.mentions is not None:
-            self.mentions = [
-                User(mention) for mention in self.mentions
-            ]
+            self.mentions = [User(mention) for mention in self.mentions]
 
         self.group = data.get("group")
         if self.group is not None:
             self.group = Group(self.group)
 
         self.conference_call = data.get("conference_call")
         if self.conference_call is not None:
@@ -833,17 +903,15 @@
 
         self.survey = data.get("survey")
         if self.survey is not None:
             self.survey = Survey(self.survey)
 
         self.videos = data.get("videos")
         if self.videos is not None:
-            self.videos = [
-                Video(video) for video in self.videos
-            ]
+            self.videos = [Video(video) for video in self.videos]
 
         self.gifts_count = data.get("gifts_count")
         if self.gifts_count is not None:
             self.gifts_count = [
                 GiftCount(gifts_count) for gifts_count in self.gifts_count
             ]
 
@@ -853,17 +921,15 @@
                 ThreadInfo(shared_thread) for shared_thread in self.shared_thread
             ]
 
         self.thread_id = data.get("thread_id")
 
         self.thread = data.get("thread")
         if self.thread is not None:
-            self.thread = [
-                ThreadInfo(thread) for thread in self.thread
-            ]
+            self.thread = [ThreadInfo(thread) for thread in self.thread]
 
         self.highlighted = data.get("highlighted")
 
         self.message_tags = data.get("message_tags")
         if self.message_tags is not None:
             self.message_tags = [
                 MessageTag(message_tag) for message_tag in self.message_tags
@@ -872,15 +938,14 @@
         self.is_fail_to_send = data.get("is_fail_to_send")
 
     def __repr__(self):
         return f"Post(data={self.data})"
 
 
 class PostGift:
-
     __slots__ = ("data", "count", "gift")
 
     def __init__(self, data):
         self.data = data
         self.count = data.get("count")
 
         self.gift = data.get("gift")
@@ -888,42 +953,39 @@
             self.gift = Gift(self.gift)
 
     def __repr__(self):
         return f"PostGift(data={self.data})"
 
 
 class PostTag:
-
     __slots__ = ("data", "id", "tag", "post_hashtags_count")
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.tag = data.get("tag")
         self.post_hashtags_count = data.get("post_hashtags_count")
 
     def __repr__(self):
         return f"PostTag(data={self.data})"
 
 
 class PresignedUrl:
-
     __slots__ = ("data", "filename", "url")
 
     def __init__(self, data):
         self.data = data
         self.filename = data.get("filename")
         self.url = data.get("url")
 
     def __repr__(self):
         return f"PresignedUrl(data={self.data})"
 
 
 class Promotion:
-
     __slots__ = ("data", "id", "title", "image_url", "promotion_url", "order")
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.title = data.get("title")
         self.image_url = data.get("image_url")
@@ -931,41 +993,36 @@
         self.order = data.get("order")
 
     def __repr__(self):
         return f"Promotion(data={self.data})"
 
 
 class ReceivedGift:
-
-    __slots__ = ("data", "gift", "received_count",
-                 "senders", "total_senders_count")
+    __slots__ = ("data", "gift", "received_count", "senders", "total_senders_count")
 
     def __init__(self, data):
         self.data = data
 
         self.gift = data.get("gift")
         if self.gift is not None:
             self.gift = Gift(self.gift)
 
         self.received_count = data.get("received_count")
 
         self.senders = data.get("senders")
         if self.senders is not None:
-            self.senders = [
-                User(sender) for sender in self.senders
-            ]
+            self.senders = [User(sender) for sender in self.senders]
 
         self.total_senders_count = data.get("total_senders_count")
 
     def __repr__(self):
         return f"ReceivedGift(data={self.data})"
 
 
 class RecentSearch:
-
     __slots__ = ("data", "id", "type", "user", "hashtag", "keyword")
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.type = data.get("type")
 
@@ -980,32 +1037,37 @@
         self.keyword = data.get("keyword")
 
     def __repr__(self):
         return f"RecentSearch(data={self.data})"
 
 
 class RefreshCounterRequest:
-
     __slots__ = ("data", "counter", "status", "last_requested_at")
 
     def __init__(self, data):
         self.data = data
         self.counter = data.get("counter")
         self.status = data.get("status")
         self.last_requested_at = data.get("last_requested_at")
 
     def __repr__(self):
         return f"RefreshCounterRequest(data={self.data})"
 
 
 class Review:
-
     __slots__ = (
-        "data", "id", "comment", "reported_count", "user", "reviewer",
-        "created_at", "created_at_parsed", "mutual_review",
+        "data",
+        "id",
+        "comment",
+        "reported_count",
+        "user",
+        "reviewer",
+        "created_at",
+        "created_at_parsed",
+        "mutual_review",
     )
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.comment = data.get("comment")
         self.reported_count = data.get("reported_count")
@@ -1020,170 +1082,193 @@
         self.mutual_review = data.get("mutual_review")
 
     def __repr__(self):
         return f"Review(data={self.data})"
 
 
 class SearchCriteria:
-
-    __slots__ = (
-        "data", "nickname", "username", "biography", "prefecture", "gender"
-    )
+    __slots__ = ("data", "nickname", "username", "biography", "prefecture", "gender")
 
     def __init__(self, data):
         self.data = data
         self.nickname = data.get("nickname")
         self.username = data.get("username")
         self.biography = data.get("biography")
         self.prefecture = data.get("prefecture")
         self.gender = data.get("gender")
 
     def __repr__(self):
         return f"SearchCriteria(data={self.data})"
 
 
 class Setting:
-
     __slots__ = (
-        "data", "notification_group_request", "notification_group_join",
-        "notification_group_post", "notification_group_message_tag_all"
+        "data",
+        "notification_group_request",
+        "notification_group_join",
+        "notification_group_post",
+        "notification_group_message_tag_all",
     )
 
     def __init__(self, data):
         self.data = data
-        self.notification_group_request = data.get(
-            "notification_group_request")
+        self.notification_group_request = data.get("notification_group_request")
         self.notification_group_join = data.get("notification_group_join")
         self.notification_group_post = data.get("notification_group_post")
         self.notification_group_message_tag_all = data.get(
-            "notification_group_message_tag_all")
+            "notification_group_message_tag_all"
+        )
 
     def __repr__(self):
         return f"Setting(data={self.data})"
 
 
 class Settings:
-
     __slots__ = (
-        "data", "notification_like", "notification_reply",
-        "notification_repost", "notification_follow", "notification_chat",
-        "notification_chat_delete", "notification_follow_request",
-        "notification_message_tag", "notification_follow_accept",
-        "notification_group_request", "notification_group_accept",
-        "notification_group_join", "notification_group_post",
-        "notification_group_invite", "notification_group_message_tag_all",
-        "notification_profile_screenshot", "notification_following_birthdate_on",
+        "data",
+        "notification_like",
+        "notification_reply",
+        "notification_repost",
+        "notification_follow",
+        "notification_chat",
+        "notification_chat_delete",
+        "notification_follow_request",
+        "notification_message_tag",
+        "notification_follow_accept",
+        "notification_group_request",
+        "notification_group_accept",
+        "notification_group_join",
+        "notification_group_post",
+        "notification_group_invite",
+        "notification_group_message_tag_all",
+        "notification_profile_screenshot",
+        "notification_following_birthdate_on",
         "notification_follower_create_group",
         "notification_follower_conference_call",
-        "notification_group_conference_call", "notification_review",
-        "notification_call_invite", "notification_bulk_call_invite",
-        "notification_group_moderator", "notification_daily_summary",
-        "notification_footprint", "notification_latest_news",
-        "notification_popular_post", "notification_following_post_after_break",
-        "notification_hima_now", "notification_birthday_to_followers",
-        "notification_twitter_friend", "notification_contact_friend",
-        "notification_security_warning", "notification_followings_in_call",
-        "hide_active_call", "privacy_mode", "private_post", "private_user_timeline",
-        "vip_invisible_footprint_mode", "allow_reposts", "invisible_on_user_search",
-        "age_restricted_on_review", "hide_online_status",
-        "following_restricted_on_review", "visible_on_sns_friend_recommendation",
-        "following_only_call_invite", "following_only_group_invite",
-        "caution_user_chat", "hide_vip", "hide_on_invitable", "hide_hot_post",
-        "no_reply_public_timeline", "no_reply_following_timeline",
-        "no_reply_group_timeline"
+        "notification_group_conference_call",
+        "notification_review",
+        "notification_call_invite",
+        "notification_bulk_call_invite",
+        "notification_group_moderator",
+        "notification_daily_summary",
+        "notification_footprint",
+        "notification_latest_news",
+        "notification_popular_post",
+        "notification_following_post_after_break",
+        "notification_hima_now",
+        "notification_birthday_to_followers",
+        "notification_twitter_friend",
+        "notification_contact_friend",
+        "notification_security_warning",
+        "notification_followings_in_call",
+        "hide_active_call",
+        "privacy_mode",
+        "private_post",
+        "private_user_timeline",
+        "vip_invisible_footprint_mode",
+        "allow_reposts",
+        "invisible_on_user_search",
+        "age_restricted_on_review",
+        "hide_online_status",
+        "following_restricted_on_review",
+        "visible_on_sns_friend_recommendation",
+        "following_only_call_invite",
+        "following_only_group_invite",
+        "caution_user_chat",
+        "hide_vip",
+        "hide_on_invitable",
+        "hide_hot_post",
+        "no_reply_public_timeline",
+        "no_reply_following_timeline",
+        "no_reply_group_timeline",
     )
 
     def __init__(self, data):
         self.data = data
         self.notification_like = data.get("notification_like")
         self.notification_reply = data.get("notification_reply")
         self.notification_repost = data.get("notification_repost")
         self.notification_follow = data.get("notification_follow")
         self.notification_chat = data.get("notification_chat")
         self.notification_chat_delete = data.get("notification_chat_delete")
-        self.notification_follow_request = data.get(
-            "notification_follow_request")
+        self.notification_follow_request = data.get("notification_follow_request")
         self.notification_message_tag = data.get("notification_message_tag")
-        self.notification_follow_accept = data.get(
-            "notification_follow_accept")
-        self.notification_group_request = data.get(
-            "notification_group_request")
+        self.notification_follow_accept = data.get("notification_follow_accept")
+        self.notification_group_request = data.get("notification_group_request")
         self.notification_group_accept = data.get("notification_group_accept")
         self.notification_group_join = data.get("notification_group_join")
         self.notification_group_post = data.get("notification_group_post")
         self.notification_group_invite = data.get("notification_group_invite")
         self.notification_group_message_tag_all = data.get(
-            "notification_group_message_tag_all")
+            "notification_group_message_tag_all"
+        )
         self.notification_profile_screenshot = data.get(
-            "notification_profile_screenshot")
+            "notification_profile_screenshot"
+        )
         self.notification_following_birthdate_on = data.get(
-            "notification_following_birthdate_on")
+            "notification_following_birthdate_on"
+        )
         self.notification_follower_create_group = data.get(
-            "notification_follower_create_group")
+            "notification_follower_create_group"
+        )
         self.notification_follower_conference_call = data.get(
-            "notification_follower_conference_call")
+            "notification_follower_conference_call"
+        )
         self.notification_group_conference_call = data.get(
-            "notification_group_conference_call")
+            "notification_group_conference_call"
+        )
         self.notification_review = data.get("notification_review")
         self.notification_call_invite = data.get("notification_call_invite")
-        self.notification_bulk_call_invite = data.get(
-            "notification_bulk_call_invite")
-        self.notification_group_moderator = data.get(
-            "notification_group_moderator")
-        self.notification_daily_summary = data.get(
-            "notification_daily_summary")
+        self.notification_bulk_call_invite = data.get("notification_bulk_call_invite")
+        self.notification_group_moderator = data.get("notification_group_moderator")
+        self.notification_daily_summary = data.get("notification_daily_summary")
         self.notification_footprint = data.get("notification_footprint")
         self.notification_latest_news = data.get("notification_latest_news")
         self.notification_popular_post = data.get("notification_popular_post")
         self.notification_following_post_after_break = data.get(
-            "notification_following_post_after_break")
+            "notification_following_post_after_break"
+        )
         self.notification_hima_now = data.get("notification_hima_now")
         self.notification_birthday_to_followers = data.get(
-            "notification_birthday_to_followers")
-        self.notification_twitter_friend = data.get(
-            "notification_twitter_friend")
-        self.notification_contact_friend = data.get(
-            "notification_contact_friend")
-        self.notification_security_warning = data.get(
-            "notification_security_warning")
+            "notification_birthday_to_followers"
+        )
+        self.notification_twitter_friend = data.get("notification_twitter_friend")
+        self.notification_contact_friend = data.get("notification_contact_friend")
+        self.notification_security_warning = data.get("notification_security_warning")
         self.notification_followings_in_call = data.get(
-            "notification_followings_in_call")
+            "notification_followings_in_call"
+        )
         self.hide_active_call = data.get("hide_active_call")
         self.privacy_mode = data.get("privacy_mode")
         self.private_post = data.get("private_post")
         self.private_user_timeline = data.get("private_user_timeline")
-        self.vip_invisible_footprint_mode = data.get(
-            "vip_invisible_footprint_mode")
+        self.vip_invisible_footprint_mode = data.get("vip_invisible_footprint_mode")
         self.allow_reposts = data.get("allow_reposts")
         self.invisible_on_user_search = data.get("invisible_on_user_search")
         self.age_restricted_on_review = data.get("age_restricted_on_review")
         self.hide_online_status = data.get("hide_online_status")
-        self.following_restricted_on_review = data.get(
-            "following_restricted_on_review")
+        self.following_restricted_on_review = data.get("following_restricted_on_review")
         self.visible_on_sns_friend_recommendation = data.get(
-            "visible_on_sns_friend_recommendation")
-        self.following_only_call_invite = data.get(
-            "following_only_call_invite")
-        self.following_only_group_invite = data.get(
-            "following_only_group_invite")
+            "visible_on_sns_friend_recommendation"
+        )
+        self.following_only_call_invite = data.get("following_only_call_invite")
+        self.following_only_group_invite = data.get("following_only_group_invite")
         self.caution_user_chat = data.get("caution_user_chat")
         self.hide_vip = data.get("hide_vip")
         self.hide_on_invitable = data.get("hide_on_invitable")
         self.hide_hot_post = data.get("hide_hot_post")
         self.no_reply_public_timeline = data.get("no_reply_public_timeline")
-        self.no_reply_following_timeline = data.get(
-            "no_reply_following_timeline")
+        self.no_reply_following_timeline = data.get("no_reply_following_timeline")
         self.no_reply_group_timeline = data.get("no_reply_group_timeline")
 
     def __repr__(self):
         return f"Settings(data={self.data})"
 
 
 class Shareable:
-
     __slots__ = ("data", "post", "group", "thread")
 
     def __init__(self, data):
         self.data = data
 
         self.post = data.get("post")
         if self.post is not None:
@@ -1198,32 +1283,36 @@
             self.thread = ThreadInfo(self.thread)
 
     def __repr__(self):
         return f"Shareable(data={self.data})"
 
 
 class SharedUrl:
-
     __slots__ = ("data", "url", "title", "description", "image_url")
 
     def __init__(self, data):
         self.data = data
         self.url = data.get("url")
         self.title = data.get("title")
         self.description = data.get("description")
         self.image_url = data.get("image_url")
 
     def __repr__(self):
         return f"SharedUrl(data={self.data})"
 
 
 class SnsInfo:
-
     __slots__ = (
-        "data", "type", "uid", "nickname", "biography", "profile_image", "gender"
+        "data",
+        "type",
+        "uid",
+        "nickname",
+        "biography",
+        "profile_image",
+        "gender",
     )
 
     def __init__(self, data):
         self.data = data
         self.type = data.get("type")
         self.uid = data.get("uid")
         self.nickname = data.get("nickname")
@@ -1232,18 +1321,15 @@
         self.gender = data.get("gender")
 
     def __repr__(self):
         return f"SnsInfo(data={self.data})"
 
 
 class Sticker:
-
-    __slots__ = (
-        "data", "id", "sticker_pack_id", "width", "height", "url", "extension"
-    )
+    __slots__ = ("data", "id", "sticker_pack_id", "width", "height", "url", "extension")
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.sticker_pack_id = data.get("sticker_pack_id")
         self.width = data.get("width")
         self.height = data.get("height")
@@ -1251,65 +1337,67 @@
         self.extension = data.get("extension")
 
     def __repr__(self):
         return f"Sticker(data={self.data})"
 
 
 class StickerPack:
-
-    __slots__ = (
-        "data", "id", "name", "description", "cover", "stickers", "order"
-    )
+    __slots__ = ("data", "id", "name", "description", "cover", "stickers", "order")
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.name = data.get("name")
         self.description = data.get("description")
         self.cover = data.get("cover")
 
         self.stickers = data.get("stickers")
         if self.stickers is not None:
-            self.stickers = [
-                Sticker(sticker) for sticker in self.stickers
-            ]
+            self.stickers = [Sticker(sticker) for sticker in self.stickers]
 
         self.order = data.get("order")
 
     def __repr__(self):
         return f"StickerPack(data={self.data})"
 
 
 class Survey:
-
     __slots__ = ("data", "id", "votes_count", "choices", "voted")
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.votes_count = data.get("votes_count")
 
         self.choices = data.get("choices")
         if self.choices is not None:
-            self.choices = [
-                Choice(choice) for choice in self.choices
-            ]
+            self.choices = [Choice(choice) for choice in self.choices]
 
         self.voted = data.get("voted")
 
     def __repr__(self):
         return f"Survey(data={self.data})"
 
 
 class ThreadInfo:
-
     __slots__ = (
-        "data", "id", "title", "owner", "last_post", "unread_count", "posts_count",
-        "created_at", "created_at_parsed", "updated_at", "updated_at_parsed",
-        "thread_icon", "is_joined", "new_updates"
+        "data",
+        "id",
+        "title",
+        "owner",
+        "last_post",
+        "unread_count",
+        "posts_count",
+        "created_at",
+        "created_at_parsed",
+        "updated_at",
+        "updated_at_parsed",
+        "thread_icon",
+        "is_joined",
+        "new_updates",
     )
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.title = data.get("title")
 
@@ -1332,43 +1420,74 @@
         self.new_updates = data.get("new_updates")
 
     def __repr__(self):
         return f"ThreadInfo(data={self.data})"
 
 
 class User:
-
     # TODO: last_logged_in_at, created_at, updated_time_millis 確かめる
 
     __slots__ = (
-        "data", "id", "nickname", "prefecture", "biography", "gender", "generation",
-        "last_logged_in_at", "last_logged_in_at_parsed", "created_at",
-        "created_at_parsed", "badge", "followers_count", "followings_count",
-        "posts_count", "groups_users_count", "reviews_count", "login_streak_count",
-        "profile_icon", "profile_icon_thumbnail", "cover_image",
-        "cover_image_thumbnail", "is_private", "is_vip", "is_vip_hidden",
-        "is_chat_request_on", "mobile_number", "is_age_verified", "is_new_user",
-        "online_status", "country_code", "is_recently_banned", "is_dangerous_user",
-        "is_trusted_different_generation", "is_selected_interests", "group_user",
-        "restricted_review_by", "is_following", "is_followed_by",
-        "is_follow_pending", "is_hidden", "connected_by", "contact_phones",
-        "updated_time_millis", "updated_time_millis_parsed"
+        "data",
+        "id",
+        "nickname",
+        "prefecture",
+        "biography",
+        "gender",
+        "generation",
+        "last_logged_in_at",
+        "last_logged_in_at_parsed",
+        "created_at",
+        "created_at_parsed",
+        "badge",
+        "followers_count",
+        "followings_count",
+        "posts_count",
+        "groups_users_count",
+        "reviews_count",
+        "login_streak_count",
+        "profile_icon",
+        "profile_icon_thumbnail",
+        "cover_image",
+        "cover_image_thumbnail",
+        "is_private",
+        "is_vip",
+        "is_vip_hidden",
+        "is_chat_request_on",
+        "mobile_number",
+        "is_age_verified",
+        "is_new_user",
+        "online_status",
+        "country_code",
+        "is_recently_banned",
+        "is_dangerous_user",
+        "is_trusted_different_generation",
+        "is_selected_interests",
+        "group_user",
+        "restricted_review_by",
+        "is_following",
+        "is_followed_by",
+        "is_follow_pending",
+        "is_hidden",
+        "connected_by",
+        "contact_phones",
+        "updated_time_millis",
+        "updated_time_millis_parsed",
     )
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.nickname = data.get("nickname")
         self.prefecture = data.get("prefecture")
         self.biography = data.get("biography")
         self.gender = data.get("gender")
         self.generation = data.get("generation")
         self.last_logged_in_at = data.get("last_logged_in_at")
-        self.last_logged_in_at_parsed = parse_datetime(
-            data.get("last_logged_in_at"))
+        self.last_logged_in_at_parsed = parse_datetime(data.get("last_logged_in_at"))
         self.created_at = data.get("created_at")
         self.created_at_parsed = parse_datetime(data.get("created_at"))
         self.badge = data.get("title")
         self.followers_count = data.get("followers_count")
         self.followings_count = data.get("followings_count")
         self.posts_count = data.get("posts_count")
         self.groups_users_count = data.get("groups_users_count")
@@ -1386,15 +1505,16 @@
         self.is_age_verified = data.get("age_verified")
         self.is_new_user = data.get("new_user")
         self.online_status = data.get("online_status")
         self.country_code = data.get("country_code")
         self.is_recently_banned = data.get("recently_kenta")
         self.is_dangerous_user = data.get("dangerous_user")
         self.is_trusted_different_generation = data.get(
-            "from_different_generation_and_trusted")
+            "from_different_generation_and_trusted"
+        )
         self.is_selected_interests = data.get("interests_selected")
 
         self.group_user = data.get("group_user")
         if self.group_user is not None:
             self.group_user = GroupUser(self.group_user)
 
         self.restricted_review_by = data.get("restricted_review_by")
@@ -1402,24 +1522,23 @@
         self.is_followed_by = data.get("followed_by")
         self.is_follow_pending = data.get("follow_pending")
         self.is_hidden = data.get("hidden")
         self.connected_by = data.get("connected_by")
         self.contact_phones = data.get("contact_phones")
         self.updated_time_millis = data.get("updated_time_millis")
         self.updated_time_millis_parsed = parse_datetime(
-            data.get("updated_time_millis"))
+            data.get("updated_time_millis")
+        )
 
     def __repr__(self):
         return f"User(data={self.data})"
 
 
 class UserAuth:
-
-    __slots__ = ("data", "user_id", "access_token",
-                 "refresh_token", "expires_in")
+    __slots__ = ("data", "user_id", "access_token", "refresh_token", "expires_in")
 
     def __init__(self, data):
         self.data = data
         self.user_id = data.get("user_id")
         self.access_token = data.get("access_token")
         self.refresh_token = data.get("refresh_token")
         self.expires_in = data.get("expires_in")
@@ -1429,15 +1548,14 @@
             self.user = User(self.user)
 
     def __repr__(self):
         return f"UserWrapper(data={self.data})"
 
 
 class UserWrapper:
-
     __slots__ = ("data", "id", "user")
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
 
         self.user = data.get("user")
@@ -1445,18 +1563,25 @@
             self.user = User(self.user)
 
     def __repr__(self):
         return f"UserWrapper(data={self.data})"
 
 
 class Video:
-
     __slots__ = (
-        "data", "id", "completed", "width", "height", "bitrate",
-        "views_count", "video_url", "thumbnail_url", "thumbnail_big_url"
+        "data",
+        "id",
+        "completed",
+        "width",
+        "height",
+        "bitrate",
+        "views_count",
+        "video_url",
+        "thumbnail_url",
+        "thumbnail_big_url",
     )
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.completed = data.get("completed")
         self.width = data.get("width")
@@ -1468,28 +1593,26 @@
         self.thumbnail_big_url = data.get("thumbnail_big_url")
 
     def __repr__(self):
         return f"Video(data={self.data})"
 
 
 class Walkthrough:
-
     __slots__ = ("data", "title", "url")
 
     def __init__(self, data):
         self.data = data
         self.title = data.get("title")
         self.url = data.get("url")
 
     def __repr__(self):
         return f"Walkthrough(data={self.data})"
 
 
 class WalletTransaction:
-
     __slots__ = ("data", "id", "created_at", "description", "amount", "coins")
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.created_at = data.get("created_at")
         self.created_at_parsed = parse_datetime(data.get("created_at"))
```

### Comparing `yaylib-0.1.3/yaylib/responses.py` & `yaylib-0.1.5/yaylib/responses.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,271 +1,243 @@
 from .models import *
 
 
 class ActiveFollowingsResponse:
-
     __slots__ = ("data", "last_loggedin_at", "users")
 
     def __init__(self, data):
         self.data = data
         self.last_loggedin_at = data.get("last_loggedin_at")
 
         self.users = data.get("users")
         if self.users is not None:
-            self.users = [
-                User(user) for user in self.users
-            ]
+            self.users = [User(user) for user in self.users]
 
     def __repr__(self):
         return f"ActiveFollowingsResponse(data={self.data})"
 
 
 class ActivitiesResponse:
-
-    __slots__ = ("data", "activities", "last_timestamp",
-                 "parsed_last_timestamp")
+    __slots__ = ("data", "activities", "last_timestamp", "parsed_last_timestamp")
 
     def __init__(self, data):
         self.data = data
 
         self.activities = data.get("activities")
         if self.activities is not None:
-            self.activities = [
-                Activity(activity) for activity in self.activities
-            ]
+            self.activities = [Activity(activity) for activity in self.activities]
 
         self.last_timestamp = data.get("last_timestamp")
         self.parsed_last_timestamp = parse_datetime(data.get("last_timestamp"))
 
     def __repr__(self):
         return f"ActivitiesResponse(data={self.data})"
 
 
 class AdditionalSettingsResponse:
-
     __slots__ = ("data", "settings")
 
     def __init__(self, data):
         self.data = data
 
         self.settings = data.get("settings")
         if self.settings is not None:
             self.settings = Settings(self.settings)
 
     def __repr__(self):
         return f"AdditionalSettingsResponse(data={self.data})"
 
 
 class AppReviewStatusResponse:
-
     __slots__ = ("data", "is_app_reviewed")
 
     def __init__(self, data):
         self.data = data
         self.is_app_reviewed = data.get("is_app_reviewed")
 
     def __repr__(self):
         return f"AppReviewStatusResponse(data={self.data})"
 
 
 class BgmsResponse:
-
     __slots__ = ("data", "bgm")
 
     def __init__(self, data):
         self.data = data
 
         self.bgm = data.get("bgm")
         if self.bgm is not None:
-            self.bgm = [
-                Bgm(bgm) for bgm in self.bgm
-            ]
+            self.bgm = [Bgm(bgm) for bgm in self.bgm]
 
     def __repr__(self):
         return f"BgmsResponse(data={self.data})"
 
 
 class BlockedUserIdsResponse:
-
     __slots__ = ("data", "block_ids")
 
     def __init__(self, data):
         self.data = data
 
         self.block_ids = data.get("block_ids")
 
     def __repr__(self):
         return f"BlockedUserIdsResponse(data={self.data})"
 
 
 class BlockedUsersResponse:
-
     __slots__ = ("data", "blocked_count", "last_id", "users")
 
     def __init__(self, data):
         self.data = data
         self.blocked_count = data.get("blocked_count")
         self.last_id = data.get("last_id")
 
         self.users = data.get("users")
         if self.users is not None:
-            self.users = [
-                User(user) for user in self.users
-            ]
+            self.users = [User(user) for user in self.users]
 
     def __repr__(self):
         return f"BlockedUsersResponse(data={self.data})"
 
 
 class BookmarkPostResponse:
-
     __slots__ = ("data", "is_bookmarked")
 
     def __init__(self, data):
         self.data = data
         self.is_bookmarked = data.get("is_bookmarked")
 
     def __repr__(self):
         return f"BookmarkPostResponse(data={self.data})"
 
 
 class CallStatusResponse:
-
     __slots__ = ("data", "phone_status", "video_status", "room_url")
 
     def __init__(self, data):
         self.data = data
         self.phone_status = data.get("phone_status")
         self.video_status = data.get("video_status")
         self.room_url = data.get("room_url")
 
     def __repr__(self):
         return f"CallStatusResponse(data={self.data})"
 
 
 class ChatRoomResponse:
-
     __slots__ = ("data", "chat")
 
     def __init__(self, data):
         self.data = data
 
         self.chat = data.get("chat")
         if self.chat is not None:
             self.chat = ChatRoom(self.chat)
 
     def __repr__(self):
         return f"ChatRoomResponse(data={self.data})"
 
 
 class ChatRoomsResponse:
-
     __slots__ = ("data", "pinned_chat_rooms", "chat_rooms", "next_page_value")
 
     def __init__(self, data):
         self.data = data
 
         self.pinned_chat_rooms = data.get("pinned_chat_rooms")
         if self.pinned_chat_rooms is not None:
             self.pinned_chat_rooms = [
-                ChatRoom(pinned_chat_room) for pinned_chat_room in self.pinned_chat_rooms
+                ChatRoom(pinned_chat_room)
+                for pinned_chat_room in self.pinned_chat_rooms
             ]
 
         self.chat_rooms = data.get("chat_rooms")
         if self.chat_rooms is not None:
-            self.chat_rooms = [
-                ChatRoom(chat_room) for chat_room in self.chat_rooms
-            ]
+            self.chat_rooms = [ChatRoom(chat_room) for chat_room in self.chat_rooms]
 
         self.next_page_value = data.get("next_page_value")
 
     def __repr__(self):
         return f"ChatRoomsResponse(data={self.data})"
 
 
 class TotalChatRequestResponse:
-
     __slots__ = ("data", "total")
 
     def __init__(self, data):
         self.data = data
         self.chat = data.get("total")
 
     def __repr__(self):
         return f"TotalChatRequestResponse(data={self.data})"
 
 
 class ConferenceCallResponse:
-
     __slots__ = ("data", "conference_call")
 
     def __init__(self, data):
         self.data = data
 
         self.conference_call = data.get("conference_call")
         if self.conference_call is not None:
             self.conference_call = ConferenceCall(self.conference_call)
 
     def __repr__(self):
         return f"ConferenceCallResponse(data={self.data})"
 
 
 class ContactStatusResponse:
-
     __slots__ = ("data", "contacts")
 
     def __init__(self, data):
         self.data = data
         self.contacts = data.get("contacts")
 
     def __repr__(self):
         return f"ContactStatusResponse(data={self.data})"
 
 
 class CreateGroupResponse:
-
     __slots__ = ("data", "group_id")
 
     def __init__(self, data):
         self.data = data
         self.group_id = data.get("group_id")
 
     def __repr__(self):
         return f"CreateGroupResponse(data={self.data})"
 
 
 class CreateQuotaResponse:
-
     __slots__ = ("data", "create")
 
     def __init__(self, data):
         self.data = data
 
         self.create = data.get("create")
         if self.create is not None:
             self.create = CreateGroupQuota(self.create)
 
     def __repr__(self):
         return f"CreateQuotaResponse(data={self.data})"
 
 
 class CreateChatRoomResponse:
-
     __slots__ = ("data", "room_id")
 
     def __init__(self, data):
         self.data = data
         self.room_id = data.get("room_id")
 
     def __repr__(self):
         return f"CreateChatRoomResponse(data={self.data})"
 
 
 class CreatePostResponse:
-
     __slots__ = ("data", "conference_call", "post")
 
     def __init__(self, data):
         self.data = data
 
         self.conference_call = data.get("conference_call")
         if self.conference_call is not None:
@@ -276,66 +248,61 @@
             self.post = Post(self.post)
 
     def __repr__(self):
         return f"CreatePostResponse(data={self.data})"
 
 
 class CreateUserResponse:
-
     __slots__ = ("data", "id", "access_token", "refresh_token", "expires_in")
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.access_token = data.get("access_token")
         self.refresh_token = data.get("refresh_token")
         self.expires_in = data.get("expires_in")
 
     def __repr__(self):
         return f"CreateUserResponse(data={self.data})"
 
 
 class EmailGrantTokenResponse:
-
     __slots__ = ("data", "email_grant_token")
 
     def __init__(self, data):
         self.data = data
         self.email_grant_token = data.get("email_grant_token")
 
     def __repr__(self):
         return f"EmailGrantTokenResponse(data={self.data})"
 
 
 class EmailVerificationPresignedUrlResponse:
-
     __slots__ = ("data", "url")
 
     def __init__(self, data):
         self.data = data
         self.url = data.get("url")
 
     def __repr__(self):
         return f"EmailVerificationPresignedUrlResponse(data={self.data})"
 
 
 class PresignedUrlResponse:
-
     __slots__ = ("data", "presigned_url")
 
     def __init__(self, data):
         self.data = data
         self.presigned_url = data.get("presigned_url")
 
     def __repr__(self):
         return f"PresignedUrlResponse(data={self.data})"
 
 
 class PresignedUrlsResponse:
-
     __slots__ = ("data", "presigned_urls")
 
     def __init__(self, data):
         self.data = data
 
         self.presigned_urls = data.get("presigned_urls")
         if self.presigned_urls is not None:
@@ -344,164 +311,145 @@
             ]
 
     def __repr__(self):
         return f"PresignedUrlsResponse(data={self.data})"
 
 
 class IdCheckerPresignedUrlResponse:
-
     __slots__ = ("data", "presigned_url")
 
     def __init__(self, data):
         self.data = data
         self.presigned_url = data.get("presigned_url")
 
     def __repr__(self):
         return f"IdCheckerPresignedUrlResponse(data={self.data})"
 
 
 class DefaultSettingsResponse:
-
     __slots__ = ("data", "timeline_settings")
 
     def __init__(self, data):
         self.data = data
 
         self.timeline_settings = data.get("timeline_settings")
         if self.timeline_settings is not None:
             self.timeline_settings = TimelineSettings(self.timeline_settings)
 
     def __repr__(self):
         return f"DefaultSettingsResponse(data={self.data})"
 
 
 class FollowRecommendationsResponse:
-
     __slots__ = ("data", "total", "users", "next")
 
     def __init__(self, data):
         self.data = data
         self.total = data.get("total")
 
         self.users = data.get("users")
         if self.users is not None:
-            self.users = [
-                User(user) for user in self.users
-            ]
+            self.users = [User(user) for user in self.users]
 
         self.next = data.get("next")
 
     def __repr__(self):
         return f"FollowRecommendationsResponse(data={self.data})"
 
 
 class FollowRequestCountResponse:
-
     __slots__ = ("data", "users_count")
 
     def __init__(self, data):
         self.data = data
         self.users_count = data.get("users_count")
 
     def __repr__(self):
         return f"FollowRequestCountResponse(data={self.data})"
 
 
 class FollowUsersResponse:
-
     __slots__ = ("data", "last_follow_id", "users")
 
     def __init__(self, data):
         self.data = data
         self.last_follow_id = data.get("last_follow_id")
 
         self.users = data.get("users")
         if self.users is not None:
-            self.users = [
-                User(user) for user in self.users
-            ]
+            self.users = [User(user) for user in self.users]
 
     def __repr__(self):
         return f"FollowUsersResponse(data={self.data})"
 
 
 class FootprintsResponse:
-
     __slots__ = ("data", "footprints")
 
     def __init__(self, data):
         self.data = data
 
         self.footprints = data.get("footprints")
         if self.footprints is not None:
-            self.footprints = [
-                Footprint(footprint) for footprint in self.footprints
-            ]
+            self.footprints = [Footprint(footprint) for footprint in self.footprints]
 
     def __repr__(self):
         return f"FootprintsResponse(data={self.data})"
 
 
 class GamesResponse:
-
     __slots__ = ("data", "games", "from_id")
 
     def __init__(self, data):
         self.data = data
 
         self.games = data.get("games")
         if self.games is not None:
-            self.games = [
-                Game(game) for game in self.games
-            ]
+            self.games = [Game(game) for game in self.games]
 
         self.from_id = data.get("from_id")
 
     def __repr__(self):
         return f"GamesResponse(data={self.data})"
 
 
 class GenresResponse:
-
     __slots__ = ("data", "genres", "next_page_value")
 
     def __init__(self, data):
         self.data = data
 
         self.genres = data.get("genres")
         if self.genres is not None:
-            self.genres = [
-                Genre(genre) for genre in self.genres
-            ]
+            self.genres = [Genre(genre) for genre in self.genres]
 
         self.next_page_value = data.get("next_page_value")
 
     def __repr__(self):
         return f"GenresResponse(data={self.data})"
 
 
 class GroupCategoriesResponse:
-
     __slots__ = ("data", "group_categories")
 
     def __init__(self, data):
         self.data = data
 
         self.group_categories = data.get("group_categories")
         if self.group_categories is not None:
             self.group_categories = [
-                GroupCategory(group_categorie) for group_categorie in self.group_categories
+                GroupCategory(group_categorie)
+                for group_categorie in self.group_categories
             ]
 
     def __repr__(self):
         return f"GroupCategoriesResponse(data={self.data})"
 
 
 class GroupGiftHistoryResponse:
-
     __slots__ = ("data", "gift_history", "next_page_value")
 
     def __init__(self, data):
         self.data = data
 
         self.gift_history = data.get("gift_history")
         if self.gift_history is not None:
@@ -512,121 +460,108 @@
         self.next_page_value = data.get("next_page_value")
 
     def __repr__(self):
         return f"GroupGiftHistoryResponse(data={self.data})"
 
 
 class GroupNotificationSettingsResponse:
-
     __slots__ = ("data", "setting")
 
     def __init__(self, data):
         self.data = data
 
         self.setting = data.get("setting")
         if self.setting is not None:
             self.setting = Setting(self.setting)
 
     def __repr__(self):
         return f"GroupNotificationSettingsResponse(data={self.data})"
 
 
 class GroupResponse:
-
     __slots__ = ("data", "group")
 
     def __init__(self, data):
         self.data = data
 
         self.group = data.get("group")
         if self.group is not None:
             self.group = Setting(self.group)
 
     def __repr__(self):
         return f"GroupResponse(data={self.data})"
 
 
 class GroupsRelatedResponse:
-
     __slots__ = ("data", "groups", "next_page_value")
 
     def __init__(self, data):
         self.data = data
 
         self.groups = data.get("groups")
         if self.groups is not None:
-            self.groups = [
-                Group(group) for group in self.groups
-            ]
+            self.groups = [Group(group) for group in self.groups]
 
         self.next_page_value = data.get("next_page_value")
 
     def __repr__(self):
         return f"GroupsRelatedResponse(data={self.data})"
 
 
 class GroupsResponse:
-
     __slots__ = ("data", "pinned_groups", "groups")
 
     def __init__(self, data):
         self.data = data
 
         self.pinned_groups = data.get("pinned_groups")
         if self.pinned_groups is not None:
             self.pinned_groups = [
                 Group(pinned_group) for pinned_group in self.pinned_groups
             ]
 
         self.groups = data.get("groups")
         if self.groups is not None:
-            self.groups = [
-                Group(group) for group in self.groups
-            ]
+            self.groups = [Group(group) for group in self.groups]
 
     def __repr__(self):
         return f"GroupsResponse(data={self.data})"
 
 
 class GroupThreadListResponse:
-
     __slots__ = ("data", "threads", "next_page_value")
 
     def __init__(self, data):
         self.data = data
 
         self.threads = data.get("threads")
         if self.threads is not None:
-            self.threads = [
-                ThreadInfo(thread) for thread in self.threads
-            ]
+            self.threads = [ThreadInfo(thread) for thread in self.threads]
 
         self.next_page_value = data.get("next_page_value")
 
     def __repr__(self):
         return f"GroupThreadListResponse(data={self.data})"
 
 
 class GroupUserResponse:
-
     __slots__ = ("data", "group_user")
 
     def __init__(self, data):
         self.data = data
 
         self.group_user = data.get("group_user")
         if self.group_user is not None:
             self.group_user = GroupUser(self.group_user)
 
     def __repr__(self):
         return f"GroupUserResponse(data={self.data})"
 
 
 class GroupUsersResponse:
-
     __slots__ = ("data", "group_users")
 
     def __init__(self, data):
         self.data = data
 
         self.group_users = data.get("group_users")
         if self.group_users is not None:
@@ -635,15 +570,14 @@
             ]
 
     def __repr__(self):
         return f"GroupUsersResponse(data={self.data})"
 
 
 class GifsDataResponse:
-
     __slots__ = ("data", "gif_categories")
 
     def __init__(self, data):
         self.data = data
 
         self.gif_categories = data.get("gif_categories")
         if self.gif_categories is not None:
@@ -652,42 +586,41 @@
             ]
 
     def __repr__(self):
         return f"GifsDataResponse(data={self.data})"
 
 
 class HiddenResponse:
-
-    __slots__ = (
-        "data", "hidden_users", "next_page_value", "total_count",
-        "limit"
-    )
+    __slots__ = ("data", "hidden_users", "next_page_value", "total_count", "limit")
 
     def __init__(self, data):
         self.data = data
 
         self.hidden_users = data.get("hidden_users")
         if self.hidden_users is not None:
-            self.hidden_users = [
-                User(hidden_user) for hidden_user in self.hidden_users
-            ]
+            self.hidden_users = [User(hidden_user) for hidden_user in self.hidden_users]
 
         self.next_page_value = data.get("next_page_value")
         self.total_count = data.get("total_count")
         self.limit = data.get("limit")
 
     def __repr__(self):
         return f"HiddenResponse(data={self.data})"
 
 
 class LoginUserResponse:
-
     __slots__ = (
-        "data", "user_id", "username", "is_new", "sns_info",
-        "access_token", "refresh_token", "expires_in"
+        "data",
+        "user_id",
+        "username",
+        "is_new",
+        "sns_info",
+        "access_token",
+        "refresh_token",
+        "expires_in",
     )
 
     def __init__(self, data):
         self.data = data
         self.user_id = data.get("user_id")
         self.username = data.get("username")
         self.is_new = data.get("is_new")
@@ -701,18 +634,21 @@
         self.expires_in = data.get("expires_in")
 
     def __repr__(self):
         return f"LoginUserResponse(data={self.data})"
 
 
 class LoginUpdateResponse:
-
     __slots__ = (
-        "data", "user_id", "username",  "access_token",
-        "refresh_token", "expires_in"
+        "data",
+        "user_id",
+        "username",
+        "access_token",
+        "refresh_token",
+        "expires_in",
     )
 
     def __init__(self, data):
         self.data = data
         self.user_id = data.get("user_id")
         self.username = data.get("username")
         self.access_token = data.get("access_token")
@@ -720,15 +656,14 @@
         self.expires_in = data.get("expires_in")
 
     def __repr__(self):
         return f"LoginUpdateResponse(data={self.data})"
 
 
 class MessageResponse:
-
     __slots__ = ("data", "id", "conference_call")
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
 
         self.conference_call = data.get("conference_call")
@@ -736,220 +671,192 @@
             self.conference_call = ConferenceCall(self.conference_call)
 
     def __repr__(self):
         return f"MessageResponse(data={self.data})"
 
 
 class MessagesResponse:
-
     __slots__ = ("data", "messages")
 
     def __init__(self, data):
         self.data = data
 
         self.messages = data.get("messages")
         if self.messages is not None:
-            self.messages = [
-                Message(message) for message in self.messages
-            ]
+            self.messages = [Message(message) for message in self.messages]
 
     def __repr__(self):
         return f"MessagesResponse(data={self.data})"
 
 
 class PolicyAgreementsResponse:
-
-    __slots__ = ("data", "latest_privacy_policy_agreed",
-                 "latest_terms_of_use_agreed")
+    __slots__ = ("data", "latest_privacy_policy_agreed", "latest_terms_of_use_agreed")
 
     def __init__(self, data):
         self.data = data
-        self.latest_privacy_policy_agreed = data.get(
-            "latest_privacy_policy_agreed")
-        self.latest_terms_of_use_agreed = data.get(
-            "latest_terms_of_use_agreed")
+        self.latest_privacy_policy_agreed = data.get("latest_privacy_policy_agreed")
+        self.latest_terms_of_use_agreed = data.get("latest_terms_of_use_agreed")
 
     def __repr__(self):
         return f"PolicyAgreementsResponse(data={self.data})"
 
 
 class PostResponse:
-
     __slots__ = ("data", "post")
 
     def __init__(self, data):
         self.data = data
 
         self.post = data.get("post")
         if self.post is not None:
             self.post = Post(self.post)
 
     def __repr__(self):
         return f"PostResponse(data={self.data})"
 
 
 class PostsResponse:
-
     __slots__ = ("data", "next_page_value", "posts", "pinned_posts")
 
     def __init__(self, data):
         self.data = data
         self.next_page_value = data.get("next_page_value")
 
         self.posts = data.get("posts")
         if self.posts is not None:
-            self.posts = [
-                Post(post) for post in self.posts
-            ]
+            self.posts = [Post(post) for post in self.posts]
 
         self.pinned_posts = data.get("pinned_posts")
         if self.pinned_posts is not None:
-            self.pinned_posts = [
-                Post(pinned_post) for pinned_post in self.pinned_posts
-            ]
+            self.pinned_posts = [Post(pinned_post) for pinned_post in self.pinned_posts]
 
     def __repr__(self):
         return f"PostsResponse(data={self.data})"
 
 
 class PostLikersResponse:
-
     __slots__ = ("data", "last_id", "users")
 
     def __init__(self, data):
         self.data = data
         self.last_id = data.get("last_id")
 
         self.users = data.get("users")
         if self.users is not None:
-            self.users = [
-                User(user) for user in self.users
-            ]
+            self.users = [User(user) for user in self.users]
 
     def __repr__(self):
         return f"PostLikersResponse(data={self.data})"
 
 
 class PostTagsResponse:
-
     __slots__ = ("data", "tags")
 
     def __init__(self, data):
         self.data = data
 
         self.tags = data.get("tags")
         if self.tags is not None:
-            self.tags = [
-                PostTag(tag) for tag in self.tags
-            ]
+            self.tags = [PostTag(tag) for tag in self.tags]
 
     def __repr__(self):
         return f"PostTagsResponse(data={self.data})"
 
 
 class PromotionsResponse:
-
     __slots__ = ("data", "promotions")
 
     def __init__(self, data):
         self.data = data
 
         self.promotions = data.get("promotions")
         if self.promotions is not None:
-            self.promotions = [
-                Promotion(promotion) for promotion in self.promotions
-            ]
+            self.promotions = [Promotion(promotion) for promotion in self.promotions]
 
     def __repr__(self):
         return f"PromotionsResponse(data={self.data})"
 
 
 class LikePostsResponse:
-
     __slots__ = ("data", "like_ids")
 
     def __init__(self, data):
         self.data = data
         self.like_ids = data.get("like_ids")
 
     def __repr__(self):
         return f"LikePostsResponse(data={self.data})"
 
 
 class ValidationPostResponse:
-
     __slots__ = ("data", "is_allow_to_post")
 
     def __init__(self, data):
         self.data = data
         self.is_allow_to_post = data.get("is_allow_to_post")
 
     def __repr__(self):
         return f"ValidationPostResponse(data={self.data})"
 
 
 class RefreshCounterRequestsResponse:
-
     __slots__ = ("data", "reset_counter_requests")
 
     def __init__(self, data):
         self.data = data
 
         self.reset_counter_requests = data.get("reset_counter_requests")
         if self.reset_counter_requests is not None:
             self.reset_counter_requests = [
-                RefreshCounterRequest(reset_counter_request) for reset_counter_request in self.reset_counter_requests
+                RefreshCounterRequest(reset_counter_request)
+                for reset_counter_request in self.reset_counter_requests
             ]
 
     def __repr__(self):
         return f"RefreshCounterRequestsResponse(data={self.data})"
 
 
 class ReviewsResponse:
-
     __slots__ = ("data", "reviews", "pinned_reviews")
 
     def __init__(self, data):
         self.data = data
 
         self.reviews = data.get("reviews")
         if self.reviews is not None:
-            self.reviews = [
-                Review(review) for review in self.reviews
-            ]
+            self.reviews = [Review(review) for review in self.reviews]
 
         self.pinned_reviews = data.get("pinned_reviews")
         if self.pinned_reviews is not None:
             self.pinned_reviews = [
                 Review(pinned_review) for pinned_review in self.pinned_reviews
             ]
 
     def __repr__(self):
         return f"ReviewsResponse(data={self.data})"
 
 
 class SocialShareUsersResponse:
-
     __slots__ = ("data", "social_shared_users")
 
     def __init__(self, data):
         self.data = data
 
         self.social_shared_users = data.get("social_shared_users")
         if self.social_shared_users is not None:
             self.social_shared_users = [
-                UserWrapper(social_shared_user) for social_shared_user in self.social_shared_users
+                UserWrapper(social_shared_user)
+                for social_shared_user in self.social_shared_users
             ]
 
     def __repr__(self):
         return f"SocialShareUsersResponse(data={self.data})"
 
 
 class StickerPacksResponse:
-
     __slots__ = ("data", "sticker_packs")
 
     def __init__(self, data):
         self.data = data
 
         self.sticker_packs = data.get("sticker_packs")
         if self.sticker_packs is not None:
@@ -958,90 +865,103 @@
             ]
 
     def __repr__(self):
         return f"StickerPacksResponse(data={self.data})"
 
 
 class TokenResponse:
-
     __slots__ = (
-        "data", "id", "created_at", "access_token", "refresh_token", "expires_in"
+        "data",
+        "user_id",
+        "created_at",
+        "access_token",
+        "refresh_token",
+        "expires_in",
     )
 
     def __init__(self, data):
         self.data = data
-        self.id = data.get("id")
+        self.user_id = data.get("id")
         self.created_at = data.get("created_at")
         self.access_token = data.get("access_token")
         self.refresh_token = data.get("refresh_token")
         self.expires_in = data.get("expires_in")
 
     def __repr__(self):
         return f"TokenResponse(data={self.data})"
 
 
 class VerifyDeviceResponse:
-
     __slots__ = ("data", "verified", "verified_at")
 
     def __init__(self, data):
         self.data = data
         self.verified = data.get("verified")
         self.verified_at = data.get("verified_at")
 
     def __repr__(self):
         return f"VerifyDeviceResponse(data={self.data})"
 
 
 class VipGameRewardUrlResponse:
-
     __slots__ = ("data", "url")
 
     def __init__(self, data):
         self.data = data
         self.url = data.get("url")
 
     def __repr__(self):
         return f"VipGameRewardUrlResponse(data={self.data})"
 
 
 class VoteSurveyResponse:
-
     __slots__ = ("data", "survey")
 
     def __init__(self, data):
         self.data = data
 
         self.survey = data.get("survey")
         if self.survey is not None:
             self.survey = Survey(self.survey)
 
     def __repr__(self):
         return f"VoteSurveyResponse(data={self.data})"
 
 
 class UnreadStatusResponse:
-
     __slots__ = ("data", "is_unread")
 
     def __init__(self, data):
         self.data = data
         self.is_unread = data.get("is_unread")
 
     def __repr__(self):
         return f"UnreadStatusResponse(data={self.data})"
 
 
 class UserResponse:
-
     __slots__ = (
-        "data", "user", "masked_email", "twitter_id", "is_line_connected",
-        "is_facebook_connected", "is_lobi_connected", "is_push_notification_on",
-        "is_call_on", "is_video_on", "is_group_call_on", "is_group_video_on", "vip_until",
-        "is_email_confirmed", "blocking_limit", "uuid", "birthdate", "gifting_ability"
+        "data",
+        "user",
+        "masked_email",
+        "twitter_id",
+        "is_line_connected",
+        "is_facebook_connected",
+        "is_lobi_connected",
+        "is_push_notification_on",
+        "is_call_on",
+        "is_video_on",
+        "is_group_call_on",
+        "is_group_video_on",
+        "vip_until",
+        "is_email_confirmed",
+        "blocking_limit",
+        "uuid",
+        "birthdate",
+        "gifting_ability",
     )
 
     def __init__(self, data):
         self.data = data
 
         self.user = data.get("user")
         if self.user is not None:
@@ -1068,37 +988,52 @@
             self.gifting_ability = GiftingAbility(self.gifting_ability)
 
     def __repr__(self):
         return f"UserResponse(data={self.data})"
 
 
 class UsersResponse:
-
     __slots__ = ("data", "users", "next_page_value")
 
     def __init__(self, data):
         self.data = data
 
         self.users = data.get("users")
         if self.users is not None:
-            self.users = [
-                User(user) for user in self.users
-            ]
+            self.users = [User(user) for user in self.users]
 
         self.next_page_value = data.get("next_page_value")
 
     def __repr__(self):
         return f"UsersResponse(data={self.data})"
 
 
-class UserCustomDefinitionsResponse:
+class RankingUsersResponse:
+    __slots__ = ("data", "users")
 
+    def __init__(self, data):
+        self.data = data
+
+        self.users = data.get("users")
+        if self.users is not None:
+            self.users = [User(user) for user in self.users]
+
+    def __repr__(self):
+        return f"RankingUsersResponse(data={self.data})"
+
+
+class UserCustomDefinitionsResponse:
     __slots__ = (
-        "age", "followers_count", "followings_count", "created_at",
-        "last_loggedin_at", "status", "reported_count"
+        "age",
+        "followers_count",
+        "followings_count",
+        "created_at",
+        "last_loggedin_at",
+        "status",
+        "reported_count",
     )
 
     def __init__(self, data):
         self.data = data
         self.age = data.get("age")
         self.followers_count = data.get("followers_count")
         self.followings_count = data.get("followings_count")
@@ -1108,76 +1043,67 @@
         self.reported_count = data.get("reported_count")
 
     def __repr__(self):
         return f"UserCustomDefinitionsResponse(data={self.data})"
 
 
 class UserEmailResponse:
-
-    __slots__ = ("email")
+    __slots__ = "email"
 
     def __init__(self, data):
         self.data = data
         self.email = data.get("email")
 
     def __repr__(self):
         return f"UserEmailResponse(data={self.data})"
 
 
 class HimaUsersResponse:
-
     __slots__ = ("data", "hima_users")
 
     def __init__(self, data):
         self.data = data
 
         self.hima_users = data.get("hima_users")
         if self.hima_users is not None:
-            self.hima_users = [
-                UserWrapper(hima_user) for hima_user in self.hima_users
-            ]
+            self.hima_users = [UserWrapper(hima_user) for hima_user in self.hima_users]
 
     def __repr__(self):
         return f"HimaUsersResponse(data={self.data})"
 
 
 class UsersByTimestampResponse:
-
     __slots__ = ("data", "last_timestamp", "users")
 
     def __init__(self, data):
         self.data = data
         self.last_timestamp = data.get("last_timestamp")
 
         self.users = data.get("users")
         if self.users is not None:
-            self.users = [
-                User(user) for user in self.users
-            ]
+            self.users = [User(user) for user in self.users]
 
     def __repr__(self):
         return f"UsersByTimestampResponse(data={self.data})"
 
 
 class UserTimestampResponse:
-
     __slots__ = ("data", "time", "ip_address", "country")
 
     def __init__(self, data):
         self.data = data
         self.time = data.get("time")
         self.ip_address = data.get("ip_address")
         self.country = data.get("country")
 
     def __repr__(self):
         return f"UserTimestampResponse(data={self.data})"
 
 
 class WebSocketTokenResponse:
-
     __slots__ = ("data", "token")
 
     def __init__(self, data):
         self.data = data
         self.token = data.get("token")
 
     def __repr__(self):
```

### Comparing `yaylib-0.1.3/yaylib/utils.py` & `yaylib-0.1.5/yaylib/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,14 +3,33 @@
 import base64
 import uuid
 
 from datetime import datetime
 from .config import Configs
 
 
+class colors:
+    HEADER = "\033[95m"
+    OKBLUE = "\033[94m"
+    OKCYAN = "\033[96m"
+    OKGREEN = "\033[92m"
+    WARNING = "\033[93m"
+    FAIL = "\033[91m"
+    RESET = "\033[0m"
+    BOLD = "\033[1m"
+    UNDERLINE = "\033[4m"
+
+
+def console_print(*args):
+    print("\n")
+    for arg in args:
+        print(arg)
+    print("\n")
+
+
 def generate_uuid() -> tuple:
     generated_uuid = str(uuid.uuid4())
     url_uuid = generated_uuid.replace("-", "")
     return generated_uuid, url_uuid
 
 
 def parse_datetime(timestamp: int) -> str:
@@ -20,19 +39,19 @@
 
 
 def signed_info_calculating(uuid: str, timestamp: int, shared_key: bool = False) -> str:
     """
     Pass the device_uuid when shared_key is False.
     """
     shared_key = Configs.YAY_SHARED_KEY if shared_key is True else ""
-    return hashlib.md5((
-        Configs.YAY_API_KEY + uuid + str(timestamp) + shared_key
-    ).encode()).hexdigest()
+    return hashlib.md5(
+        (Configs.YAY_API_KEY + uuid + str(timestamp) + shared_key).encode()
+    ).hexdigest()
 
 
 def signed_version_calculating() -> str:
     hash_object = hmac.new(
         Configs.YAY_API_VERSION_KEY.encode(),
         "yay_android/{}".format(Configs.YAY_API_VERSION).encode(),
-        hashlib.sha256
+        hashlib.sha256,
     )
     return base64.b64encode(hash_object.digest()).decode("utf-8")
```

### Comparing `yaylib-0.1.3/yaylib.egg-info/PKG-INFO` & `yaylib-0.1.5/yaylib.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: yaylib
-Version: 0.1.3
+Version: 0.1.5
 Summary: This Python package provides an easy-to-use interface for accessing data from Yay! (https://yay.space/). With this API Client, you can retrieve user profiles, posts, comments, and other content from Yay!, as well as perform common tasks like liking and commenting on posts.
 Home-page: https://github.com/qvco/yaylib
 Download-URL: https://github.com/qvco/yaylib
 Author: Qvco, Konn
 Author-email: nikola.desuga@gmail.com
 Maintainer: Qvco, Konn
 Maintainer-email: nikola.desuga@gmail.com
 License: MIT
-Keywords: yay,yaylib,api,bot,library,wrapper,ボット,ライブラリ
+Keywords: yay,yaylib,api,bot,client,library,wrapper,ボット,ライブラリ
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div><a id="readme-top"></a></div>
@@ -21,27 +21,24 @@
     <img src="https://img.shields.io/github/stars/qvco/yaylib?style=for-the-badge&logo=appveyor&color=blue" />
     <img src="https://img.shields.io/github/forks/qvco/yaylib?style=for-the-badge&logo=appveyor&color=blue" />
     <img src="https://img.shields.io/github/issues/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational" />
     <img src="https://img.shields.io/github/issues-pr/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational" />
 </div>
 <br />
 <p align="center">
-<!--     <a href="https://github.com/othneildrew/Best-README-Template">
-        <img src="https://github.com/qvco/yaylib/assets/77382767/6e72ec90-b8e9-40bf-a7ad-34fb2ccea0f9" alt="Logo" height="300px">
-    </a> -->
     <a href="https://github.com/othneildrew/Best-README-Template">
-        <img src="https://github.com/qvco/yaylib/assets/77382767/5265b956-55b7-466c-8cdb-cf0f3abed946" alt="Logo" height="300px">
+        <img src="https://github.com/qvco/yaylib/assets/77382767/45c45b21-d812-4cad-8f27-315ffef53201" alt="Logo" height="300px">
     </a>
     <h3 align="center">yaylib</h3>
     <p align="center">
-        「<strong>yaylib</strong>」は同世代でつながるチャットアプリ、Yay!（イェイ）の API クライアントです。<br />
-        このライブラリを使用することで、あらゆる操作の自動化や、ボットの開発が可能です。
+        「<strong>yaylib</strong>」は同世代でつながるチャットアプリ、Yay!（イェイ）の API ラッパーです。<br />
+        あらゆる操作の自動化や、ボットの開発が可能です。
         <br />
         <br />
-        <a href="https://github.com/qvco/yaylib/blob/main/docs/README.md">
+        <a href="https://github.com/qvco/yaylib/blob/master/docs/README.md">
             <strong>詳しい機能の詳細や使い方はこちらから »</strong>
         </a>
         <br />
         <br />
         <a href="https://github.com/qvco/yaylib/issues">Report Bug</a>
         ·
         <a href="https://github.com/qvco/yaylib/issues">Request Feature</a>
@@ -65,26 +62,26 @@
   </ol>
 </details>
 
 <!-- Buy me a coffee -->
 
 ## Buy me a coffee
 
-もしこのライブラリが気に入っていただけたら、<a href="https://github.com/qvco/yaylib/">ぜひスターをお願いします</a> ⭐️  
+このライブラリが気に入っていただけたら、<a href="https://github.com/qvco/yaylib/">スターをお願いします</a> ⭐️  
 また、Buy Me a Coffee からご支援いただけますと幸いです。
 
 <a href="https://www.buymeacoffee.com/qvco" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: auto !important;width: auto !important;" ></a>
 
 <!-- インストール -->
 
 ## インストール
 
 **※ Python 3.11 かそれ以上のバージョンが必要です。**
 
-ライブラリをインストールするには、以下のコマンドを実行します:
+「yaylib」をインストールするには、以下のコマンドを実行します:
 
 ```bash
 pip install yaylib
 ```
 
 開発バージョンをインストールするには、以下の手順を実行します:
 
@@ -94,90 +91,97 @@
 cd yaylib
 
 pip install -r requirements.txt
 
 pip install -e .
 ```
 
-「yaylib」の始め方については、[こちら](https://github.com/qvco/yaylib/blob/main/docs/TUTORIAL.md) を確認してください。
+「yaylib」の始め方については、[こちら](https://github.com/qvco/yaylib/blob/master/docs/TUTORIAL.md) を確認してください。
 
 <!-- 使用例 -->
 
 ## 使用例
 
-メールアドレスとパスワードを用いてログイン後、新しく投稿を作成するコードです。
+メールアドレスとパスワードを使用してログインしたあと、タイムラインをキーワードで検索して「いいね」するコードです。
 
 ```python
 import yaylib
 
-api = yaylib.Client()
 
+api = yaylib.Client()
 api.login(email="メールアドレス", password="パスワード")
 
-api.create_post(text="初めての投稿！", color=2)
+timeline = api.get_timeline_by_keyword(
+    keyword="プログラミング",
+    number=15
+)
+
+for post in timeline.posts:
+    response = api.like_post(post.id)
+    print(post.id, response.data) # 実行結果を出力
 ```
 
-より詳しい使用例については、[こちら](https://github.com/qvco/yaylib/blob/main/examples) を参照してください。
+より詳しい使用例については、[こちら](https://github.com/qvco/yaylib/blob/master/examples) を参照してください。
 
 <p align="right">(<a href="#readme-top">トップに戻る</a>)</p>
 
 <!-- yaylib で誕生したボットの一覧 -->
 
 ## yaylib で誕生したロボットたち
 
-yaylib を用いて開発したロボットがある場合は、ぜひ教えてください！
+「yaylib」を用いて開発したロボットがある場合は、ぜひ教えてください！
 
 <table align="center">
     <thead>
         <tr>
             <th><a href="https://yay.space/user/5855987">MindReader AI</a></th>
-            <th><a href="https://yay.space/user/0">Funktion</a></th>
-            <th><a href="https://yay.space/user/0">香ばしいボット</a></th>
+            <th><a href="https://yay.space/user/7293290">香ばしいボット</a></th>
+            <th><a href="https://yay.space/user/7406336">GIGAZINE</a></th>
         </tr>
     </thead>
     <tbody>
         <tr>
             <td align="center">
-                <img src="https://github.com/qvco/yaylib/assets/77382767/472febe4-4c5f-490c-8417-de0d5dbbbc72" width="200px">
+                <img src="https://github.com/qvco/yaylib/assets/77382767/cc41ce3c-0e11-4ec5-be99-ff7090a95667" width="200px">
                 <br />
                 <p>開発者: <a href="https://yay.space/user/35152">毛の可能性</a></p>
             </td>
             <td align="center">
-                <img src="https://github.com/qvco/yaylib/assets/77382767/ff207016-21bf-4e76-b0e0-f70ebc4a121f" width="200px">
+                <img src="https://github.com/qvco/yaylib/assets/77382767/cbffdc25-7873-4242-b065-e6a686bade54" width="200px">
                 <br />
-                <p>開発者: <a href="https://yay.space/user/0">ぺゅー</a></p>
+                <p>開発者: <a href="https://yay.space/user/93923">めんぶれ天然水。</a></p>
             </td>
             <td align="center">
-                <img src="https://github.com/qvco/yaylib/assets/77382767/2324e518-b2c8-43cd-95e5-90ee2383aec1" width="200px">
+                <img src="https://github.com/qvco/yaylib/assets/77382767/65fcb885-4fbe-4170-9378-6f8d9af61ff8" width="200px">
                 <br />
-                <p>開発者: <a href="https://yay.space/user/0">めんぶれ天然水。</a></p>
+                <p>開発者: <a href="https://yay.space/user/1298298">ぺゅー</a></p>
             </td>
         </tr>
     </tbody>
 </table>
 
 <!-- 共同開発について -->
 
 ## 共同開発について
 
-私たちと一緒に開発することに興味を持っていただけているなら大歓迎です。
+私たちと開発することに興味を持っていただけているなら、ぜひ参加してください！
 
 - <a href="https://github.com/qvco/yaylib/pulls">プルリクエストを送信する</a>
 - <a href="mailto:nikola.desuga@gmail.com">nikola.desuga@gmail.com</a> にメールを送信する
 - <a href="https://discord.gg/MEuBfNtqRN">Discord サーバーに参加する</a>
 
-のいずれかの方法でコンタクトしてください。詳しくは[こちら](https://github.com/qvco/yaylib/blob/main/CONTRIBUTING.md)から！
+のいずれかの方法でコンタクトしてください。詳しくは[こちらから](https://github.com/qvco/yaylib/blob/master/CONTRIBUTING.md)！
 
 <!-- 免責事項 -->
 
 ## 免責事項
 
 yaylib は、API の公式なサポートやメンテナンスを提供するものではありません。このクライアントを使用する場合、利用者は**リスクや責任を自己負担**できるものとします。このクライアントによって提供される情報やデータの正確性、信頼性、完全性、適時性について、いかなる保証も行いません。また、このクライアントの使用によって生じた損害や不利益について、一切の責任を負いかねます。利用者は自己の責任において、このクライアントを使用し、API にアクセスするものとします。なお、この免責事項は予告なく変更される場合があります。
 
 <!-- 利用許諾 -->
 
 ## 利用許諾
 
-フルライセンスは [こちら](https://github.com/qvco/yaylib/blob/main/LICENSE) からご確認いただけます。  
+フルライセンスは [こちら](https://github.com/qvco/yaylib/blob/master/LICENSE) からご確認いただけます。  
 このプロジェクトは、 **【MIT ライセンス】** の条件の下でライセンスされています。
 
 <p align="right">(<a href="#readme-top">トップに戻る</a>)</p>
```

#### html2text {}

```diff
@@ -1,78 +1,80 @@
-Metadata-Version: 2.1 Name: yaylib Version: 0.1.3 Summary: This Python package
+Metadata-Version: 2.1 Name: yaylib Version: 0.1.5 Summary: This Python package
 provides an easy-to-use interface for accessing data from Yay! (https://
 yay.space/). With this API Client, you can retrieve user profiles, posts,
 comments, and other content from Yay!, as well as perform common tasks like
 liking and commenting on posts. Home-page: https://github.com/qvco/yaylib
 Download-URL: https://github.com/qvco/yaylib Author: Qvco, Konn Author-email:
 nikola.desuga@gmail.com Maintainer: Qvco, Konn Maintainer-email:
 nikola.desuga@gmail.com License: MIT Keywords:
-yay,yaylib,api,bot,library,wrapper,ããã,ã©ã¤ãã©ãª Classifier:
+yay,yaylib,api,bot,client,library,wrapper,ããã,ã©ã¤ãã©ãª Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.11 Description-
 Content-Type: text/markdown License-File: LICENSE
         [https://img.shields.io/github/stars/qvco/yaylib?style=for-the-
   badge&logo=appveyor&color=blue] [https://img.shields.io/github/forks/qvco/
  yaylib?style=for-the-badge&logo=appveyor&color=blue] [https://img.shields.io/
                    github/issues/qvco/yaylib?style=for-the-
 badge&logo=appveyor&color=informational] [https://img.shields.io/github/issues-
      pr/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational]
 
-                                     [Logo]
+                                    [Logo]
                                **** yaylib ****
 ãyaylibãã¯åä¸ä»£ã§ã¤ãªãããã£ããã¢ããªãYay!ï¼ã¤ã§ã¤ï¼ã®
-                        API ã¯ã©ã¤ã¢ã³ãã§ãã
-ãã®ã©ã¤ãã©ãªãä½¿ç¨ãããã¨ã§ãããããæä½ã®èªååãããããã®éçºãå¯è½ã§ãã
-
+                           API ã©ããã¼ã§ãã
+   ããããæä½ã®èªååãããããã®éçºãå¯è½ã§ãã
 
           è©³ããæ©è½ã®è©³ç´°ãä½¿ãæ¹ã¯ãã¡ããã_Â»
 
                Report_Bug Â· Request_Feature Â· Join_the_discord
   Table of Contents
    1. Buy_me_a_coffee
    2. ã¤ã³ã¹ãã¼ã«
    3. ä½¿ç¨ä¾
    4. yaylib_ã§èªçããã­ããããã¡
    5. å±åéçºã«ã¤ãã¦
    6. åè²¬äºé 
    7. å©ç¨è¨±è«¾
   ## Buy me a coffee
-ãããã®ã©ã¤ãã©ãªãæ°ã«å¥ã£ã¦ããã ãããããã²ã¹ã¿ã¼ããé¡ããã¾ã
+ãã®ã©ã¤ãã©ãªãæ°ã«å¥ã£ã¦ããã ããããã¹ã¿ã¼ããé¡ããã¾ã
 â­ï¸ ã¾ããBuy Me a Coffee
 ãããæ¯æ´ããã ãã¾ãã¨å¹¸ãã§ãã [Buy_Me_A_Coffee]  ##
 ã¤ã³ã¹ãã¼ã« **â» Python 3.11
 ãããä»¥ä¸ã®ãã¼ã¸ã§ã³ãå¿è¦ã§ãã**
-ã©ã¤ãã©ãªãã¤ã³ã¹ãã¼ã«ããã«ã¯ãä»¥ä¸ã®ã³ãã³ããå®è¡ãã¾ã:
+ãyaylibããã¤ã³ã¹ãã¼ã«ããã«ã¯ãä»¥ä¸ã®ã³ãã³ããå®è¡ãã¾ã:
 ```bash pip install yaylib ```
 éçºãã¼ã¸ã§ã³ãã¤ã³ã¹ãã¼ã«ããã«ã¯ãä»¥ä¸ã®æé ãå®è¡ãã¾ã:
 ```bash git clone https://github.com/qvco/yaylib cd yaylib pip install -
 r requirements.txt pip install -e . ```
 ãyaylibãã®å§ãæ¹ã«ã¤ãã¦ã¯ã[ãã¡ã](https://github.com/qvco/
-yaylib/blob/main/docs/TUTORIAL.md) ãç¢ºèªãã¦ãã ããã  ## ä½¿ç¨ä¾
-ã¡ã¼ã«ã¢ãã¬ã¹ã¨ãã¹ã¯ã¼ããç¨ãã¦ã­ã°ã¤ã³å¾ãæ°ããæç¨¿ãä½æããã³ã¼ãã§ãã
+yaylib/blob/master/docs/TUTORIAL.md) ãç¢ºèªãã¦ãã ããã  ##
+ä½¿ç¨ä¾
+ã¡ã¼ã«ã¢ãã¬ã¹ã¨ãã¹ã¯ã¼ããä½¿ç¨ãã¦ã­ã°ã¤ã³ãããã¨ãã¿ã¤ã ã©ã¤ã³ãã­ã¼ã¯ã¼ãã§æ¤ç´¢ãã¦ãããã­ãããã³ã¼ãã§ãã
 ```python import yaylib api = yaylib.Client() api.login
-(email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã") api.create_post
-(text="åãã¦ã®æç¨¿ï¼", color=2) ```
+(email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã") timeline =
+api.get_timeline_by_keyword( keyword="ãã­ã°ã©ãã³ã°", number=15 ) for
+post in timeline.posts: response = api.like_post(post.id) print(post.id,
+response.data) # å®è¡çµæãåºå ```
 ããè©³ããä½¿ç¨ä¾ã«ã¤ãã¦ã¯ã[ãã¡ã](https://github.com/qvco/
-yaylib/blob/main/examples) ãåç§ãã¦ãã ããã
+yaylib/blob/master/examples) ãåç§ãã¦ãã ããã
                                                            (ãããã«æ»ã)
- ## yaylib ã§èªçããã­ããããã¡ yaylib
-ãç¨ãã¦éçºããã­ããããããå ´åã¯ããã²æãã¦ãã ããï¼
-MindReader_AI                                      Funktion                               é¦ã°ããããã
- [https://github.com/qvco/yaylib/assets/77382767/     [https://github.com/qvco/yaylib/    [https://github.com/qvco/yaylib/assets/77382767/2324e518-b2c8-43cd-
-      472febe4-4c5f-490c-8417-de0d5dbbbc72]         assets/77382767/ff207016-21bf-4e76-                           95e5-90ee2383aec1]
-            éçºè: æ¯ã®å¯�         b0e0-f70ebc4a121f]                            éçºè: ããã¶ãå¤©ç¶æ°´ã
-                                                            éçºè: ãºãã¼
+ ## yaylib ã§èªçããã­ããããã¡
+ãyaylibããç¨ãã¦éçºããã­ããããããå ´åã¯ããã²æãã¦ãã ããï¼
+MindReader_AI                                      é¦ã°ããããã                           GIGAZINE
+ [https://github.com/qvco/yaylib/assets/77382767/  [https://github.com/qvco/yaylib/assets/77382767/cbffdc25-7873-4242-     [https://github.com/qvco/yaylib/
+      cc41ce3c-0e11-4ec5-be99-ff7090a95667]                                b065-e6a686bade54]                            assets/77382767/65fcb885-4fbe-4170-
+            éçºè: æ¯ã®å¯�                éçºè: ããã¶ãå¤©ç�         9378-6f8d9af61ff8]
+                                                                                                                                 éçºè: ãºãã¼
  ## å±åéçºã«ã¤ãã¦
-ç§ãã¡ã¨ä¸ç·ã«éçºãããã¨ã«èå³ãæã£ã¦ããã ãã¦ãããªãå¤§æ­è¿ã§ãã
+ç§ãã¡ã¨éçºãããã¨ã«èå³ãæã£ã¦ããã ãã¦ãããªãããã²åå ãã¦ãã ããï¼
 - ãã«ãªã¯ã¨ã¹ããéä¿¡ãã - nikola.desuga@gmail.com
 ã«ã¡ã¼ã«ãéä¿¡ãã - Discord_ãµã¼ãã¼ã«åå ãã
 ã®ããããã®æ¹æ³ã§ã³ã³ã¿ã¯ããã¦ãã ãããè©³ããã¯
-[ãã¡ã](https://github.com/qvco/yaylib/blob/main/CONTRIBUTING.md)ããï¼
-## åè²¬äºé  yaylib ã¯ãAPI
+[ãã¡ããã](https://github.com/qvco/yaylib/blob/master/
+CONTRIBUTING.md)ï¼  ## åè²¬äºé  yaylib ã¯ãAPI
 ã®å¬å¼ãªãµãã¼ããã¡ã³ããã³ã¹ãæä¾ãããã®ã§ã¯ããã¾ããããã®ã¯ã©ã¤ã¢ã³ããä½¿ç¨ããå ´åãå©ç¨èã¯**ãªã¹ã¯ãè²¬ä»»ãèªå·±è² æ**ã§ãããã®ã¨ãã¾ãããã®ã¯ã©ã¤ã¢ã³ãã«ãã£ã¦æä¾ãããæå ±ããã¼ã¿ã®æ­£ç¢ºæ§ãä¿¡é ¼æ§ãå®å¨æ§ãé©ææ§ã«ã¤ãã¦ããããªãä¿è¨¼ãè¡ãã¾ãããã¾ãããã®ã¯ã©ã¤ã¢ã³ãã®ä½¿ç¨ã«ãã£ã¦çããæå®³ãä¸å©çã«ã¤ãã¦ãä¸åã®è²¬ä»»ãè² ããã­ã¾ããå©ç¨èã¯èªå·±ã®è²¬ä»»ã«ããã¦ããã®ã¯ã©ã¤ã¢ã³ããä½¿ç¨ããAPI
 ã«ã¢ã¯ã»ã¹ãããã®ã¨ãã¾ãããªãããã®åè²¬äºé ã¯äºåãªãå¤æ´ãããå ´åãããã¾ãã
 ## å©ç¨è¨±è«¾ ãã«ã©ã¤ã»ã³ã¹ã¯ [ãã¡ã](https://github.com/qvco/
-yaylib/blob/main/LICENSE) ãããç¢ºèªããã ãã¾ãã
+yaylib/blob/master/LICENSE) ãããç¢ºèªããã ãã¾ãã
 ãã®ãã­ã¸ã§ã¯ãã¯ã **ãMIT ã©ã¤ã»ã³ã¹ã**
 ã®æ¡ä»¶ã®ä¸ã§ã©ã¤ã»ã³ã¹ããã¦ãã¾ãã
                                                            (ãããã«æ»ã)
```

### Comparing `yaylib-0.1.3/yaylib.egg-info/SOURCES.txt` & `yaylib-0.1.5/yaylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

