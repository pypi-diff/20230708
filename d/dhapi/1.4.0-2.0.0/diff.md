# Comparing `tmp/dhapi-1.4.0.tar.gz` & `tmp/dhapi-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhapi-1.4.0.tar", last modified: Mon May 15 00:50:10 2023, max compression
+gzip compressed data, was "dhapi-2.0.0.tar", last modified: Sat Jul  8 07:18:28 2023, max compression
```

## Comparing `dhapi-1.4.0.tar` & `dhapi-2.0.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-15 00:50:10.086488 dhapi-1.4.0/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11356 2023-05-15 00:45:36.000000 dhapi-1.4.0/LICENSE.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2615 2023-05-15 00:50:10.086488 dhapi-1.4.0/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1960 2023-05-15 00:45:36.000000 dhapi-1.4.0/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       51 2023-05-15 00:45:36.000000 dhapi-1.4.0/pyproject.toml
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-15 00:50:10.086488 dhapi-1.4.0/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1271 2023-05-15 00:45:36.000000 dhapi-1.4.0/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-15 00:50:10.078488 dhapi-1.4.0/src/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-15 00:50:10.082488 dhapi-1.4.0/src/dhapi/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-15 00:46:17.000000 dhapi-1.4.0/src/dhapi/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-15 00:50:10.082488 dhapi-1.4.0/src/dhapi/client/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-15 00:46:17.000000 dhapi-1.4.0/src/dhapi/client/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4804 2023-05-15 00:45:36.000000 dhapi-1.4.0/src/dhapi/client/lottery_client.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-15 00:50:10.082488 dhapi-1.4.0/src/dhapi/configuration/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-15 00:46:17.000000 dhapi-1.4.0/src/dhapi/configuration/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      862 2023-05-15 00:45:36.000000 dhapi-1.4.0/src/dhapi/configuration/logger.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-15 00:50:10.082488 dhapi-1.4.0/src/dhapi/domain_object/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-15 00:46:17.000000 dhapi-1.4.0/src/dhapi/domain_object/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3954 2023-05-15 00:45:36.000000 dhapi-1.4.0/src/dhapi/domain_object/lotto645_buy_request.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      120 2023-05-15 00:45:36.000000 dhapi-1.4.0/src/dhapi/main.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-15 00:50:10.086488 dhapi-1.4.0/src/dhapi/purchase/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-15 00:46:17.000000 dhapi-1.4.0/src/dhapi/purchase/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2231 2023-05-15 00:45:36.000000 dhapi-1.4.0/src/dhapi/purchase/lotto645_controller.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-15 00:50:10.086488 dhapi-1.4.0/src/dhapi/router/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-15 00:46:17.000000 dhapi-1.4.0/src/dhapi/router/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4616 2023-05-15 00:45:36.000000 dhapi-1.4.0/src/dhapi/router/arg_parser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      518 2023-05-15 00:45:36.000000 dhapi-1.4.0/src/dhapi/router/router.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      953 2023-05-15 00:45:36.000000 dhapi-1.4.0/src/dhapi/router/version_checker.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-15 00:50:10.086488 dhapi-1.4.0/src/dhapi/user_info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-15 00:46:17.000000 dhapi-1.4.0/src/dhapi/user_info/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      202 2023-05-15 00:45:36.000000 dhapi-1.4.0/src/dhapi/user_info/user_info_controller.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-15 00:50:10.082488 dhapi-1.4.0/src/dhapi.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2615 2023-05-15 00:50:10.000000 dhapi-1.4.0/src/dhapi.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      775 2023-05-15 00:50:10.000000 dhapi-1.4.0/src/dhapi.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-15 00:50:10.000000 dhapi-1.4.0/src/dhapi.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       42 2023-05-15 00:50:10.000000 dhapi-1.4.0/src/dhapi.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       72 2023-05-15 00:50:10.000000 dhapi-1.4.0/src/dhapi.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        6 2023-05-15 00:50:10.000000 dhapi-1.4.0/src/dhapi.egg-info/top_level.txt
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-07-08 07:18:28.889818 dhapi-2.0.0/
+-rw-r--r--   0 roeniss    (501) staff       (20)    11356 2023-05-14 08:41:15.000000 dhapi-2.0.0/LICENSE.txt
+-rw-r--r--   0 roeniss    (501) staff       (20)     2983 2023-07-08 07:18:28.889706 dhapi-2.0.0/PKG-INFO
+-rw-r--r--   0 roeniss    (501) staff       (20)     2328 2023-07-08 06:48:18.000000 dhapi-2.0.0/README.md
+-rw-r--r--   0 roeniss    (501) staff       (20)       51 2023-05-14 08:41:15.000000 dhapi-2.0.0/pyproject.toml
+-rw-r--r--   0 roeniss    (501) staff       (20)       38 2023-07-08 07:18:28.889854 dhapi-2.0.0/setup.cfg
+-rw-r--r--   0 roeniss    (501) staff       (20)     1271 2023-05-14 08:41:15.000000 dhapi-2.0.0/setup.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-07-08 07:18:28.884989 dhapi-2.0.0/src/
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-07-08 07:18:28.887284 dhapi-2.0.0/src/dhapi/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-05-14 08:41:15.000000 dhapi-2.0.0/src/dhapi/__init__.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-07-08 07:18:28.888159 dhapi-2.0.0/src/dhapi/client/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-05-14 08:41:15.000000 dhapi-2.0.0/src/dhapi/client/__init__.py
+-rw-r--r--   0 roeniss    (501) staff       (20)     4980 2023-07-08 07:11:45.000000 dhapi-2.0.0/src/dhapi/client/lottery_client.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-07-08 07:18:28.888409 dhapi-2.0.0/src/dhapi/configuration/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-05-14 08:41:15.000000 dhapi-2.0.0/src/dhapi/configuration/__init__.py
+-rw-r--r--   0 roeniss    (501) staff       (20)      862 2023-05-14 08:41:15.000000 dhapi-2.0.0/src/dhapi/configuration/logger.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-07-08 07:18:28.888616 dhapi-2.0.0/src/dhapi/domain_object/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-05-14 08:41:15.000000 dhapi-2.0.0/src/dhapi/domain_object/__init__.py
+-rw-r--r--   0 roeniss    (501) staff       (20)     3960 2023-07-08 07:12:17.000000 dhapi-2.0.0/src/dhapi/domain_object/lotto645_buy_request.py
+-rw-r--r--   0 roeniss    (501) staff       (20)      120 2023-05-14 08:41:15.000000 dhapi-2.0.0/src/dhapi/main.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-07-08 07:18:28.888821 dhapi-2.0.0/src/dhapi/purchase/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-05-14 08:41:15.000000 dhapi-2.0.0/src/dhapi/purchase/__init__.py
+-rw-r--r--   0 roeniss    (501) staff       (20)     2231 2023-05-21 06:21:51.000000 dhapi-2.0.0/src/dhapi/purchase/lotto645_controller.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-07-08 07:18:28.889320 dhapi-2.0.0/src/dhapi/router/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-05-14 08:41:15.000000 dhapi-2.0.0/src/dhapi/router/__init__.py
+-rw-r--r--   0 roeniss    (501) staff       (20)     4467 2023-07-08 07:13:59.000000 dhapi-2.0.0/src/dhapi/router/arg_parser.py
+-rw-r--r--   0 roeniss    (501) staff       (20)      518 2023-05-14 08:41:15.000000 dhapi-2.0.0/src/dhapi/router/router.py
+-rw-r--r--   0 roeniss    (501) staff       (20)      953 2023-05-14 08:41:15.000000 dhapi-2.0.0/src/dhapi/router/version_checker.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-07-08 07:18:28.889548 dhapi-2.0.0/src/dhapi/user_info/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-05-14 08:41:15.000000 dhapi-2.0.0/src/dhapi/user_info/__init__.py
+-rw-r--r--   0 roeniss    (501) staff       (20)      202 2023-05-14 08:41:15.000000 dhapi-2.0.0/src/dhapi/user_info/user_info_controller.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-07-08 07:18:28.887938 dhapi-2.0.0/src/dhapi.egg-info/
+-rw-r--r--   0 roeniss    (501) staff       (20)     2983 2023-07-08 07:18:28.000000 dhapi-2.0.0/src/dhapi.egg-info/PKG-INFO
+-rw-r--r--   0 roeniss    (501) staff       (20)      775 2023-07-08 07:18:28.000000 dhapi-2.0.0/src/dhapi.egg-info/SOURCES.txt
+-rw-r--r--   0 roeniss    (501) staff       (20)        1 2023-07-08 07:18:28.000000 dhapi-2.0.0/src/dhapi.egg-info/dependency_links.txt
+-rw-r--r--   0 roeniss    (501) staff       (20)       42 2023-07-08 07:18:28.000000 dhapi-2.0.0/src/dhapi.egg-info/entry_points.txt
+-rw-r--r--   0 roeniss    (501) staff       (20)      101 2023-07-08 07:18:28.000000 dhapi-2.0.0/src/dhapi.egg-info/requires.txt
+-rw-r--r--   0 roeniss    (501) staff       (20)        6 2023-07-08 07:18:28.000000 dhapi-2.0.0/src/dhapi.egg-info/top_level.txt
```

### Comparing `dhapi-1.4.0/LICENSE.txt` & `dhapi-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dhapi-1.4.0/PKG-INFO` & `dhapi-2.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhapi
-Version: 1.4.0
+Version: 2.0.0
 Summary: 동행복권 비공식 API
 Home-page: https://github.com/roeniss/dhlottery-api
 Author: Roeniss Moon
 Author-email: roeniss2@gmail.com
 Project-URL: Bug Reports, https://github.com/roeniss/dhlottery-api/issues
 Project-URL: Source, https://github.com/roeniss/dhlottery-api/
 Keywords: donghaeng,lottery,lotto645,api,korean
@@ -49,34 +49,58 @@
 
 [동행복권](https://dhlottery.co.kr/) 사이트를 터미널에서 이용할 수 있게 랩핑한 API입니다.
 
 Python 3.8 이상에서 설치해야 최신버전이 작동합니다.
 
 ## 구현된 기능
 
--   [로또 6/45](https://dhlottery.co.kr/gameInfo.do?method=gameMethod&wiselog=H_B_1_1)
-    -   자동 구매 1 ~ 5장
+- [로또 6/45](https://dhlottery.co.kr/gameInfo.do?method=gameMethod&wiselog=H_B_1_1)
+  - 자동 구매 1 ~ 5장
 
 ## 사용법
 
-### 사전준비: 계정 정보 세팅
+### 계정 정보 세팅
 
-`~/.dhapi_profile` 파일에 아이디와 패스워드를 입력하면 자동으로 로그인합니다. (`-p` 인자를 이용해 경로를 임의로 지정할 수도 있습니다)
+`~/.dhapi/credentials` 파일에 username, password를 입력하면 자동으로 로그인합니다.
+profile을 여러개 설정할 수 있습니다.
 
-    ```sh
-    echo $USER_ID > ~/.dhapi_profile # 첫째 줄은 아이디
-    echo $USER_PW >> ~/.dhapi_profile # 둘째 줄은 비밀번호 (미리 복잡한 난수로 변경하시길 권장합니다)
-    ```
+```sh
+DHAPI_USERNAME=asdf
+DHAPI_PASSWORD=****
+
+mkdir -p ~/.dhapi
+cd ~/.dhapi
+
+echo "[default]" > credentials
+echo username = $DHAPI_USERNAME >> credentials # username
+echo password = $DHAPI_PASSWORD >> credentials # password (미리 복잡한 난수로 변경하시길 권장합니다)
+```
+```sh
+DHAPI_USERNAME=qwer
+DHAPI_PASSWORD=5678
+
+cd ~/.dhapi
+
+echo "" >> credentials
+echo "[qwer]" >> credentials
+echo username = $DHAPI_USERNAME >> credentials
+echo password = $DHAPI_PASSWORD >> credentials
+```
 
 > `-u $USER_ID` 파라미터를 이용하면 명령어 실행 중 비밀번호를 입력받는 방법도 있지만, 권장하지 않습니다.
 
-### 설치 밎 사용법:
+### 설치 밎 사용법
 
 ```sh
+pip install --upgrade pip # pip 가 최신 버전이 아니면 dhapi 구버전이 깔리는 경우가 있습니다
 pip install dhapi
+
 dhapi -h
-dhapi buy_lotto645 -q # 프로필 파일을 이용해 계정 정보 입력 & 자동모드로 5장 구매
+
+# 자동모드로 5장 구매
+dhapi buy_lotto645 -q # profile: default
+dhapi buy_lotto645 -q -p qwer # profile: qwer
 ```
 
 ## 기여하기
 
 기여는 대환영입니다! [CONTRIBUTING.md](/docs/CONTRIBUTING.md) 파일을 참고해주세요.
```

### Comparing `dhapi-1.4.0/README.md` & `dhapi-2.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -31,34 +31,58 @@
 
 [동행복권](https://dhlottery.co.kr/) 사이트를 터미널에서 이용할 수 있게 랩핑한 API입니다.
 
 Python 3.8 이상에서 설치해야 최신버전이 작동합니다.
 
 ## 구현된 기능
 
--   [로또 6/45](https://dhlottery.co.kr/gameInfo.do?method=gameMethod&wiselog=H_B_1_1)
-    -   자동 구매 1 ~ 5장
+- [로또 6/45](https://dhlottery.co.kr/gameInfo.do?method=gameMethod&wiselog=H_B_1_1)
+  - 자동 구매 1 ~ 5장
 
 ## 사용법
 
-### 사전준비: 계정 정보 세팅
+### 계정 정보 세팅
 
-`~/.dhapi_profile` 파일에 아이디와 패스워드를 입력하면 자동으로 로그인합니다. (`-p` 인자를 이용해 경로를 임의로 지정할 수도 있습니다)
+`~/.dhapi/credentials` 파일에 username, password를 입력하면 자동으로 로그인합니다.
+profile을 여러개 설정할 수 있습니다.
 
-    ```sh
-    echo $USER_ID > ~/.dhapi_profile # 첫째 줄은 아이디
-    echo $USER_PW >> ~/.dhapi_profile # 둘째 줄은 비밀번호 (미리 복잡한 난수로 변경하시길 권장합니다)
-    ```
+```sh
+DHAPI_USERNAME=asdf
+DHAPI_PASSWORD=****
+
+mkdir -p ~/.dhapi
+cd ~/.dhapi
+
+echo "[default]" > credentials
+echo username = $DHAPI_USERNAME >> credentials # username
+echo password = $DHAPI_PASSWORD >> credentials # password (미리 복잡한 난수로 변경하시길 권장합니다)
+```
+```sh
+DHAPI_USERNAME=qwer
+DHAPI_PASSWORD=5678
+
+cd ~/.dhapi
+
+echo "" >> credentials
+echo "[qwer]" >> credentials
+echo username = $DHAPI_USERNAME >> credentials
+echo password = $DHAPI_PASSWORD >> credentials
+```
 
 > `-u $USER_ID` 파라미터를 이용하면 명령어 실행 중 비밀번호를 입력받는 방법도 있지만, 권장하지 않습니다.
 
-### 설치 밎 사용법:
+### 설치 밎 사용법
 
 ```sh
+pip install --upgrade pip # pip 가 최신 버전이 아니면 dhapi 구버전이 깔리는 경우가 있습니다
 pip install dhapi
+
 dhapi -h
-dhapi buy_lotto645 -q # 프로필 파일을 이용해 계정 정보 입력 & 자동모드로 5장 구매
+
+# 자동모드로 5장 구매
+dhapi buy_lotto645 -q # profile: default
+dhapi buy_lotto645 -q -p qwer # profile: qwer
 ```
 
 ## 기여하기
 
 기여는 대환영입니다! [CONTRIBUTING.md](/docs/CONTRIBUTING.md) 파일을 참고해주세요.
```

### Comparing `dhapi-1.4.0/setup.py` & `dhapi-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `dhapi-1.4.0/src/dhapi/client/lottery_client.py` & `dhapi-2.0.0/src/dhapi/client/lottery_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,32 +12,34 @@
 class LotteryClient:
     _default_session_url = "https://dhlottery.co.kr/gameResult.do?method=byWin&wiselog=H_C_1_1"
     _system_under_check_url = "https://dhlottery.co.kr/index_check.html"
     _main_url = "https://dhlottery.co.kr/common.do?method=main"
     _login_request_url = "https://www.dhlottery.co.kr/userSsl.do?method=login"
     _buy_lotto645_url = "https://ol.dhlottery.co.kr/olotto/game/execBuy.do"
     _round_info_url = "https://www.dhlottery.co.kr/common.do?method=main"
+    _ready_socket = "https://ol.dhlottery.co.kr/olotto/game/egovUserReadySocket.json"
 
     def __init__(self):
         self._headers = {
             "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.77 Safari/537.36",
             "Connection": "keep-alive",
             "Cache-Control": "max-age=0",
             "sec-ch-ua": '" Not;A Brand";v="99", "Google Chrome";v="91", "Chromium";v="91"',
             "sec-ch-ua-mobile": "?0",
             "Upgrade-Insecure-Requests": "1",
             "Origin": "https://dhlottery.co.kr",
-            "Content-Type": "application/x-www-form-urlencoded",
+            "Content-Type": "application/x-www-form-urlencoded; charset=UTF-8",
             "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9",
-            "Referer": "https://dhlottery.co.kr/",
+            "Referer": "https://dhlottery.co.kr",
             "Sec-Fetch-Site": "same-site",
             "Sec-Fetch-Mode": "navigate",
             "Sec-Fetch-User": "?1",
             "Sec-Fetch-Dest": "document",
             "Accept-Language": "ko,en-US;q=0.9,en;q=0.8,ko-KR;q=0.7",
+            "X-Requested-With": "XMLHttpRequest",
         }
         self._set_default_session()
 
     # 로그인을 시도하면 새로운 JSESSIONID 값이 내려오는데,
     #  이 값으로 갱신하면 로그인이 풀리는 듯하여 헤더를 갱신하지 않음
     def _set_default_session(self):
         resp = requests.get(LotteryClient._default_session_url, timeout=10)
@@ -81,25 +83,30 @@
         """
         :param first 첫 번째 복권 게임을 의미한다. 다음 두 가지 형태 중 하나를 가진다.
          - 일반 숫자 5개와 보너스 숫자를 포함하는 list ([1, 2, 3, 4, 5, 6]) (각각 1~45)
          - 자동 또는 반자동을 의미하는 str ("AUTO", "SEMI_AUTO")
          위 내용은 second, third, fourth, fifth 파라미터에도 적용된다.
         """
 
+        res = requests.post(url=self._ready_socket, headers=self._headers, timeout=5)
+        direct = json.loads(res.text)["ready_ip"]
+
+        logger.debug(f"direct: {direct}")
+
+        data = {
+            "round": str(self._get_round()),
+            "direct": direct,
+            "nBuyAmount": str(1000 * req.get_game_count()),
+            "param": req.create_dhlottery_request_param(),
+            "gameCnt": req.get_game_count(),
+        }
+        logger.debug(f"data: {data}")
         resp = requests.post(
             self._buy_lotto645_url,
             headers=self._headers,
-            data={
-                "round": str(self._get_round()),
-                "direct": "172.17.20.52",  # TODO: test if this can be omitted
-                "nBuyAmount": str(1000 * req.get_game_count()),
-                "param": req.create_dhlottery_request_param(),
-                "gameCnt": req.get_game_count(),
-                # "ROUND_DRAW_DATE": "2021/06/01", # succeed after commented
-                # "WAMT_PAY_TLMT_END_DT": "2022/06/01", # succeed after commented
-            },
+            data=data,
             timeout=10,
         )
 
-        resp.encoding = "utf-8"
+        logger.debug(f"resp.text: {resp.text}")
 
         return json.loads(resp.text)
```

### Comparing `dhapi-1.4.0/src/dhapi/configuration/logger.py` & `dhapi-2.0.0/src/dhapi/configuration/logger.py`

 * *Files identical despite different names*

### Comparing `dhapi-1.4.0/src/dhapi/domain_object/lotto645_buy_request.py` & `dhapi-2.0.0/src/dhapi/domain_object/lotto645_buy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
         raise RuntimeError("지원하지 않는 게임 타입입니다.")
 
     def _get_gen_type(self, game_type):
         if not isinstance(game_type, Lotto645GameType):
             raise RuntimeError("지원하지 않는 게임 타입입니다.")
 
-        return str(game_type)
+        return str(game_type.value)
 
     def _encode_game(self, slot, game):
         game_type = self._get_game_type(game)
         # fmt: off
         return {
             "genType": self._get_gen_type(game_type),
             "arrGameChoiceNum": ",".join(map(str, game)) if game_type != Lotto645GameType.AUTO else None,
```

### Comparing `dhapi-1.4.0/src/dhapi/purchase/lotto645_controller.py` & `dhapi-2.0.0/src/dhapi/purchase/lotto645_controller.py`

 * *Files identical despite different names*

### Comparing `dhapi-1.4.0/src/dhapi/router/arg_parser.py` & `dhapi-2.0.0/src/dhapi/router/arg_parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
-import pathlib
 import getpass
-import os
 import sys
 
+from seunggabi_core_python.util import config_util
+
 from dhapi.router.version_checker import get_versions
 from dhapi.domain_object.lotto645_buy_request import Lotto645BuyRequest
 
 
 class HelpOnErrorParser(argparse.ArgumentParser):
     def error(self, message):
         sys.stderr.write(f"🚨 입력 파라미터 에러 발생: {message}\n")
@@ -68,29 +68,26 @@
 옵션을 아예 입력하지 않으면 '자동으로 5장 구매'를 수행합니다.""",
         )
         buy_lotto645.add_argument(
             "-p",
             "--profile",
             required=False,
             nargs=1,
-            default="~/.dhapi_profile",
-            help="프로필 파일 절대경로입니다. (default: ~/.dhapi_profile; 포맷은 README.md 참고)",
+            default=["default"],
+            help="https://github.com/roeniss/dhlottery-api#계정 정보 세팅",
         )
         buy_lotto645.add_argument("-d", "--debug", action="store_true", help="로그 출력 레벨을 debug로 세팅합니다.")  # "store_true" means "set default to False"
         self._args = parser.parse_args()
 
-        if not self._args.username is None:
+        if self._args.username:
             self._args.password = getpass.getpass("비밀번호를 입력하세요: ")
         else:
-            profile_path = pathlib.Path(self._args.profile).expanduser()
-            if not (os.path.exists(profile_path) and os.path.isfile(profile_path)):
-                _exit(f"{self._args.profile} 파일이 존재하지 않습니다")
-
-            with open(profile_path, encoding="utf-8") as f:
-                self._args.username, self._args.password = f.read().splitlines()
+            credentials = config_util.get(group="dhapi", context="credentials", profile=self._args.profile[0])
+            self._args.username = credentials["username"]
+            self._args.password = credentials["password"]
 
         if self.is_buylotto645():
             self.normalize_games_for_lotto645()
 
     def get_is_debug(self):
         return self._args.debug
 
@@ -104,15 +101,15 @@
         return self._args.quiet
 
     def is_buylotto645(self):
         return self._args.command == "buy_lotto645"
 
     def normalize_games_for_lotto645(self):
         if self._args.games is None:
-            self._args.games = [None for _ in range(5)]
+            self._args.games = [None for _ in range(Lotto645BuyRequest.MAX_GAME_COUNT)]
 
         req_bucket = []
         for game in self._args.games:
             req_bucket.append([] if game is None else [*map(int, game.split(","))])
 
         self._args.games = req_bucket
```

### Comparing `dhapi-1.4.0/src/dhapi/router/router.py` & `dhapi-2.0.0/src/dhapi/router/router.py`

 * *Files identical despite different names*

### Comparing `dhapi-1.4.0/src/dhapi/router/version_checker.py` & `dhapi-2.0.0/src/dhapi/router/version_checker.py`

 * *Files identical despite different names*

### Comparing `dhapi-1.4.0/src/dhapi.egg-info/PKG-INFO` & `dhapi-2.0.0/src/dhapi.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhapi
-Version: 1.4.0
+Version: 2.0.0
 Summary: 동행복권 비공식 API
 Home-page: https://github.com/roeniss/dhlottery-api
 Author: Roeniss Moon
 Author-email: roeniss2@gmail.com
 Project-URL: Bug Reports, https://github.com/roeniss/dhlottery-api/issues
 Project-URL: Source, https://github.com/roeniss/dhlottery-api/
 Keywords: donghaeng,lottery,lotto645,api,korean
@@ -49,34 +49,58 @@
 
 [동행복권](https://dhlottery.co.kr/) 사이트를 터미널에서 이용할 수 있게 랩핑한 API입니다.
 
 Python 3.8 이상에서 설치해야 최신버전이 작동합니다.
 
 ## 구현된 기능
 
--   [로또 6/45](https://dhlottery.co.kr/gameInfo.do?method=gameMethod&wiselog=H_B_1_1)
-    -   자동 구매 1 ~ 5장
+- [로또 6/45](https://dhlottery.co.kr/gameInfo.do?method=gameMethod&wiselog=H_B_1_1)
+  - 자동 구매 1 ~ 5장
 
 ## 사용법
 
-### 사전준비: 계정 정보 세팅
+### 계정 정보 세팅
 
-`~/.dhapi_profile` 파일에 아이디와 패스워드를 입력하면 자동으로 로그인합니다. (`-p` 인자를 이용해 경로를 임의로 지정할 수도 있습니다)
+`~/.dhapi/credentials` 파일에 username, password를 입력하면 자동으로 로그인합니다.
+profile을 여러개 설정할 수 있습니다.
 
-    ```sh
-    echo $USER_ID > ~/.dhapi_profile # 첫째 줄은 아이디
-    echo $USER_PW >> ~/.dhapi_profile # 둘째 줄은 비밀번호 (미리 복잡한 난수로 변경하시길 권장합니다)
-    ```
+```sh
+DHAPI_USERNAME=asdf
+DHAPI_PASSWORD=****
+
+mkdir -p ~/.dhapi
+cd ~/.dhapi
+
+echo "[default]" > credentials
+echo username = $DHAPI_USERNAME >> credentials # username
+echo password = $DHAPI_PASSWORD >> credentials # password (미리 복잡한 난수로 변경하시길 권장합니다)
+```
+```sh
+DHAPI_USERNAME=qwer
+DHAPI_PASSWORD=5678
+
+cd ~/.dhapi
+
+echo "" >> credentials
+echo "[qwer]" >> credentials
+echo username = $DHAPI_USERNAME >> credentials
+echo password = $DHAPI_PASSWORD >> credentials
+```
 
 > `-u $USER_ID` 파라미터를 이용하면 명령어 실행 중 비밀번호를 입력받는 방법도 있지만, 권장하지 않습니다.
 
-### 설치 밎 사용법:
+### 설치 밎 사용법
 
 ```sh
+pip install --upgrade pip # pip 가 최신 버전이 아니면 dhapi 구버전이 깔리는 경우가 있습니다
 pip install dhapi
+
 dhapi -h
-dhapi buy_lotto645 -q # 프로필 파일을 이용해 계정 정보 입력 & 자동모드로 5장 구매
+
+# 자동모드로 5장 구매
+dhapi buy_lotto645 -q # profile: default
+dhapi buy_lotto645 -q -p qwer # profile: qwer
 ```
 
 ## 기여하기
 
 기여는 대환영입니다! [CONTRIBUTING.md](/docs/CONTRIBUTING.md) 파일을 참고해주세요.
```

### Comparing `dhapi-1.4.0/src/dhapi.egg-info/SOURCES.txt` & `dhapi-2.0.0/src/dhapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

