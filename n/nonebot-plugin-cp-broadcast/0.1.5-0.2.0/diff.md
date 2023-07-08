# Comparing `tmp/nonebot_plugin_cp_broadcast-0.1.5.tar.gz` & `tmp/nonebot_plugin_cp_broadcast-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_cp_broadcast-0.1.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_cp_broadcast-0.2.0.tar", max compression
```

## Comparing `nonebot_plugin_cp_broadcast-0.1.5.tar` & `nonebot_plugin_cp_broadcast-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,9 @@
--rw-r--r--   0        0        0     1064 2023-07-07 08:54:45.194905 nonebot_plugin_cp_broadcast-0.1.5/LICENSE
--rw-r--r--   0        0        0     3852 2023-07-07 08:54:45.194905 nonebot_plugin_cp_broadcast-0.1.5/README.md
--rw-r--r--   0        0        0    13953 2023-07-07 08:54:45.194905 nonebot_plugin_cp_broadcast-0.1.5/nonebot_plugin_cp_broadcast/__init__.py
--rw-r--r--   0        0        0      332 2023-07-07 08:54:45.194905 nonebot_plugin_cp_broadcast-0.1.5/nonebot_plugin_cp_broadcast/config.py
--rw-r--r--   0        0        0      590 2023-07-07 08:54:45.194905 nonebot_plugin_cp_broadcast-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     4618 1970-01-01 00:00:00.000000 nonebot_plugin_cp_broadcast-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-08 04:01:16.961115 nonebot_plugin_cp_broadcast-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4494 2023-07-08 04:01:16.961115 nonebot_plugin_cp_broadcast-0.2.0/README.md
+-rw-r--r--   0        0        0     7431 2023-07-08 04:01:16.965115 nonebot_plugin_cp_broadcast-0.2.0/nonebot_plugin_cp_broadcast/__init__.py
+-rw-r--r--   0        0        0     2503 2023-07-08 04:01:16.965115 nonebot_plugin_cp_broadcast-0.2.0/nonebot_plugin_cp_broadcast/atcoder.py
+-rw-r--r--   0        0        0     1946 2023-07-08 04:01:16.965115 nonebot_plugin_cp_broadcast-0.2.0/nonebot_plugin_cp_broadcast/codeforces.py
+-rw-r--r--   0        0        0      432 2023-07-08 04:01:16.965115 nonebot_plugin_cp_broadcast-0.2.0/nonebot_plugin_cp_broadcast/config.py
+-rw-r--r--   0        0        0     2416 2023-07-08 04:01:16.965115 nonebot_plugin_cp_broadcast-0.2.0/nonebot_plugin_cp_broadcast/nowcoder.py
+-rw-r--r--   0        0        0      766 2023-07-08 04:01:16.965115 nonebot_plugin_cp_broadcast-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5444 1970-01-01 00:00:00.000000 nonebot_plugin_cp_broadcast-0.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_cp_broadcast-0.1.5/LICENSE` & `nonebot_plugin_cp_broadcast-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-0.1.5/README.md` & `nonebot_plugin_cp_broadcast-0.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -21,14 +21,26 @@
 
 </div>
 
 ## 📖 介绍
 
 对于每一个 ACMer 来说，参加编程竞赛是必不可少的，这个插件实现了 Codeforces、牛客竞赛、AtCoder 这三个主流的编程竞赛平台的比赛查询和播报。
 
+除了简单的指令外，它支持每天定时发送三种比赛的信息。
+
+查询的结果会存到列表里，以减少网站爬取的次数。
+
+由于 AtCoder 网站没提供比赛信息的 API，因此是直接对网页进行爬取的，代码中是爬取两个比赛，你可以自己修改得更多。
+
+为什么取 cp-broadcast 这个英文名呢？因为竞赛性编程的英文是：Competitive Programming，直接拿来做名字感觉太长了，因此我把它写成了缩写，broadcast 是播报的意思，因此就用 cp-broadcast 来当名字了。
+
+这是本蒟蒻的第一个上传至 pypi 的 nonebot2 项目，可能有很多不完善的地方，欢迎大家来提 issue 和 pull requests。 
+
+有任何问题可联系QQ：3411907440。
+
 ## 💿 安装
 
 <details>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
     nb plugin install nonebot-plugin-cp-broadcast
@@ -70,27 +82,26 @@
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | cp_broadcast_list | 否 | [ ] | 开启早晨自动播报今日比赛的群聊，填 QQ 群号，注意以字符串形式填入 |
 | cp_broadcast_botname | 否 | "bot" | 填入你 bot 的名字，在 `help` 指令下会使用到你的 bot 的名字 |
-| cp_broadcast_time | 否 | {"hour":"7", "minute":"20"} | 每日在群聊播报比赛信息的时间，默认是早上 7 点 20，你可以在配置文件中按默认值格式修改成你想要的时间，注意需要安装 `nonebot_plugin_apscheduler` 插件以实现定时效果。 |
-| cp_broadcast_updatetime | 否 | {"hour":"0", "minute":"0"} | 每天自动更新比赛数据的时间，默认是 0 点 0 分，你可以在配置文件中按默认值格式修改成你想要的时间，注意需要安装 `nonebot_plugin_apscheduler` 插件以实现定时效果。 |
+| cp_broadcast_time | 否 | {"hour":"7", "minute":"20"} | 每日在群聊播报比赛信息的时间，默认是早上 7 点 20，你可以在配置文件中按默认值格式修改成你想要的时间 |
+| cp_broadcast_updatetime | 否 | {"hour":"0", "minute":"0"} | 每天自动更新比赛数据的时间，默认是 0 点 0 分，你可以在配置文件中按默认值格式修改成你想要的时间 |
+
+该插件依赖 [nonebot_plugin_apscheduler](https://github.com/nonebot/plugin-apscheduler) 实现定时发送功能，如果你是通过下载项目源码安装插件的话，请注意安装好依赖。
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | `cf` | 群员 | 否 | 群聊 | 发送最近三场 Codeforces 比赛的信息 |
 | `牛客` or `nc` | 群员 | 否 | 群聊 | 发送最近三场牛客比赛的信息 |
-| atc | 群员 | 否 | 群聊 | 发送最近两场 AtCoder 比赛的信息 |
-| today | 群员 | 否 | 群聊 | 发送今天的比赛信息 |
-| next | 群员 | 否 | 群聊 | 发送今天后的部分比赛信息 |
-| help | 群员 | 否 | 群聊 | 发送帮助信息 |
-| update | 群员 | 否 | 群聊 | 手动更新比赛信息 |
+| `atc` | 群员 | 否 | 群聊 | 发送最近两场 AtCoder 比赛的信息 |
+| `today` | 群员 | 否 | 群聊 | 发送今天的比赛信息 |
+| `next` | 群员 | 否 | 群聊 | 发送今天后的部分比赛信息 |
+| `help` | 群员 | 是 | 群聊 | 发送帮助信息 |
+| `update` | 群员 | 否 | 群聊 | 手动更新比赛信息 |
 ### 效果图
 <img src="./docs/preview.webp" style="zoom:30%;" />
 
-这是本蒟蒻的第一个上传至 pypi 的 nonebot 项目，可能有很多不完善的地方，欢迎大家来 pull requests。 
-
-有任何问题可联系QQ：3411907440
```

#### html2text {}

```diff
@@ -1,16 +1,27 @@
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # nonebot-plugin-cp-broadcast _â¨ ä¸ä¸ª Codeforcesãçå®¢ç«èµãAtCoder
 å¹³å°çç¼ç¨ç«èµæ¥è¯¢æä»¶ï¼ACMerå¿å¤ â¨_ [license] [pypi] [python]
 ## ð ä»ç» å¯¹äºæ¯ä¸ä¸ª ACMer
 æ¥è¯´ï¼åå ç¼ç¨ç«èµæ¯å¿ä¸å¯å°çï¼è¿ä¸ªæä»¶å®ç°äº
 Codeforcesãçå®¢ç«èµãAtCoder
-è¿ä¸ä¸ªä¸»æµçç¼ç¨ç«èµå¹³å°çæ¯èµæ¥è¯¢åæ­æ¥ã ## ð¿ å®è£
-ä½¿ç¨ nb-cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
+è¿ä¸ä¸ªä¸»æµçç¼ç¨ç«èµå¹³å°çæ¯èµæ¥è¯¢åæ­æ¥ã
+é¤äºç®åçæä»¤å¤ï¼å®æ¯ææ¯å¤©å®æ¶åéä¸ç§æ¯èµçä¿¡æ¯ã
+æ¥è¯¢çç»æä¼å­å°åè¡¨éï¼ä»¥åå°ç½ç«ç¬åçæ¬¡æ°ã ç±äº
+AtCoder ç½ç«æ²¡æä¾æ¯èµä¿¡æ¯ç
+APIï¼å æ­¤æ¯ç´æ¥å¯¹ç½é¡µè¿è¡ç¬åçï¼ä»£ç ä¸­æ¯ç¬åä¸¤ä¸ªæ¯èµï¼ä½ å¯ä»¥èªå·±ä¿®æ¹å¾æ´å¤ã
+ä¸ºä»ä¹å cp-broadcast
+è¿ä¸ªè±æåå¢ï¼å ä¸ºç«èµæ§ç¼ç¨çè±ææ¯ï¼Competitive
+Programmingï¼ç´æ¥æ¿æ¥ååå­æè§å¤ªé¿äºï¼å æ­¤ææå®åæäºç¼©åï¼broadcast
+æ¯æ­æ¥çææï¼å æ­¤å°±ç¨ cp-broadcast æ¥å½åå­äºã
+è¿æ¯æ¬èè»çç¬¬ä¸ä¸ªä¸ä¼ è³ pypi ç nonebot2
+é¡¹ç®ï¼å¯è½æå¾å¤ä¸å®åçå°æ¹ï¼æ¬¢è¿å¤§å®¶æ¥æ issue å pull
+requestsã æä»»ä½é®é¢å¯èç³»QQï¼3411907440ã ## ð¿ å®è£  ä½¿ç¨
+nb-cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-cp-broadcast
 ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-cp-broadcast   pdm pdm add nonebot-plugin-cp-
 broadcast   poetry poetry add nonebot-plugin-cp-broadcast   conda conda install
 nonebot-plugin-cp-broadcast  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
@@ -18,25 +29,23 @@
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
 é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | cp_broadcast_list | å¦ |
 [ ] | å¼å¯æ©æ¨èªå¨æ­æ¥ä»æ¥æ¯èµçç¾¤èï¼å¡« QQ
 ç¾¤å·ï¼æ³¨æä»¥å­ç¬¦ä¸²å½¢å¼å¡«å¥ | | cp_broadcast_botname | å¦ | "bot"
 | å¡«å¥ä½  bot çåå­ï¼å¨ `help` æä»¤ä¸ä¼ä½¿ç¨å°ä½ ç bot
 çåå­ | | cp_broadcast_time | å¦ | {"hour":"7", "minute":"20"} |
 æ¯æ¥å¨ç¾¤èæ­æ¥æ¯èµä¿¡æ¯çæ¶é´ï¼é»è®¤æ¯æ©ä¸ 7 ç¹
-20ï¼ä½ å¯ä»¥å¨éç½®æä»¶ä¸­æé»è®¤å¼æ ¼å¼ä¿®æ¹æä½ æ³è¦çæ¶é´ï¼æ³¨æéè¦å®è£
-`nonebot_plugin_apscheduler` æä»¶ä»¥å®ç°å®æ¶ææã | |
-cp_broadcast_updatetime | å¦ | {"hour":"0", "minute":"0"} |
+20ï¼ä½ å¯ä»¥å¨éç½®æä»¶ä¸­æé»è®¤å¼æ ¼å¼ä¿®æ¹æä½ æ³è¦çæ¶é´ |
+| cp_broadcast_updatetime | å¦ | {"hour":"0", "minute":"0"} |
 æ¯å¤©èªå¨æ´æ°æ¯èµæ°æ®çæ¶é´ï¼é»è®¤æ¯ 0 ç¹ 0
-åï¼ä½ å¯ä»¥å¨éç½®æä»¶ä¸­æé»è®¤å¼æ ¼å¼ä¿®æ¹æä½ æ³è¦çæ¶é´ï¼æ³¨æéè¦å®è£
-`nonebot_plugin_apscheduler` æä»¶ä»¥å®ç°å®æ¶ææã | ## ð ä½¿ç¨
-### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:
-----:|:----:|:----:| | `cf` | ç¾¤å | å¦ | ç¾¤è | åéæè¿ä¸åº
-Codeforces æ¯èµçä¿¡æ¯ | | `çå®¢` or `nc` | ç¾¤å | å¦ | ç¾¤è |
-åéæè¿ä¸åºçå®¢æ¯èµçä¿¡æ¯ | | atc | ç¾¤å | å¦ | ç¾¤è |
-åéæè¿ä¸¤åº AtCoder æ¯èµçä¿¡æ¯ | | today | ç¾¤å | å¦ | ç¾¤è |
-åéä»å¤©çæ¯èµä¿¡æ¯ | | next | ç¾¤å | å¦ | ç¾¤è |
-åéä»å¤©åçé¨åæ¯èµä¿¡æ¯ | | help | ç¾¤å | å¦ | ç¾¤è |
-åéå¸®å©ä¿¡æ¯ | | update | ç¾¤å | å¦ | ç¾¤è |
+åï¼ä½ å¯ä»¥å¨éç½®æä»¶ä¸­æé»è®¤å¼æ ¼å¼ä¿®æ¹æä½ æ³è¦çæ¶é´
+| è¯¥æä»¶ä¾èµ [nonebot_plugin_apscheduler](https://github.com/nonebot/
+plugin-apscheduler)
+å®ç°å®æ¶åéåè½ï¼å¦æä½ æ¯éè¿ä¸è½½é¡¹ç®æºç å®è£æä»¶çè¯ï¼è¯·æ³¨æå®è£å¥½ä¾èµã
+## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:
+-----:|:----:|:----:|:----:|:----:| | `cf` | ç¾¤å | å¦ | ç¾¤è |
+åéæè¿ä¸åº Codeforces æ¯èµçä¿¡æ¯ | | `çå®¢` or `nc` | ç¾¤å |
+å¦ | ç¾¤è | åéæè¿ä¸åºçå®¢æ¯èµçä¿¡æ¯ | | `atc` | ç¾¤å | å¦
+| ç¾¤è | åéæè¿ä¸¤åº AtCoder æ¯èµçä¿¡æ¯ | | `today` | ç¾¤å |
+å¦ | ç¾¤è | åéä»å¤©çæ¯èµä¿¡æ¯ | | `next` | ç¾¤å | å¦ | ç¾¤è |
+åéä»å¤©åçé¨åæ¯èµä¿¡æ¯ | | `help` | ç¾¤å | æ¯ | ç¾¤è |
+åéå¸®å©ä¿¡æ¯ | | `update` | ç¾¤å | å¦ | ç¾¤è |
 æå¨æ´æ°æ¯èµä¿¡æ¯ | ### ææå¾ [./docs/preview.webp]
-è¿æ¯æ¬èè»çç¬¬ä¸ä¸ªä¸ä¼ è³ pypi ç nonebot
-é¡¹ç®ï¼å¯è½æå¾å¤ä¸å®åçå°æ¹ï¼æ¬¢è¿å¤§å®¶æ¥ pull requestsã
-æä»»ä½é®é¢å¯èç³»QQï¼3411907440
```

### Comparing `nonebot_plugin_cp_broadcast-0.1.5/PKG-INFO` & `nonebot_plugin_cp_broadcast-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cp-broadcast
-Version: 0.1.5
-Summary: A nonebot plugin package
+Version: 0.2.0
+Summary: Codeforces、牛客、AtCoder平台比赛查询，ACMer 必备
+Home-page: https://github.com/HuParry/nonebot-plugin-cp-broadcast
 License: MIT
 Author: HuParry
 Author-email: huparry@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -13,14 +14,15 @@
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: fake-useragent (>=1.1.3,<2.0.0)
 Requires-Dist: httpx (>=0.20.0,<1.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.2,<3.0.0)
 Requires-Dist: nonebot-plugin-apscheduler (>=0.3.0,<0.4.0)
 Requires-Dist: nonebot2[fastapi] (>=2.0.0,<3.0.0)
+Project-URL: Repository, https://github.com/HuParry/nonebot-plugin-cp-broadcast
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
@@ -42,14 +44,26 @@
 
 </div>
 
 ## 📖 介绍
 
 对于每一个 ACMer 来说，参加编程竞赛是必不可少的，这个插件实现了 Codeforces、牛客竞赛、AtCoder 这三个主流的编程竞赛平台的比赛查询和播报。
 
+除了简单的指令外，它支持每天定时发送三种比赛的信息。
+
+查询的结果会存到列表里，以减少网站爬取的次数。
+
+由于 AtCoder 网站没提供比赛信息的 API，因此是直接对网页进行爬取的，代码中是爬取两个比赛，你可以自己修改得更多。
+
+为什么取 cp-broadcast 这个英文名呢？因为竞赛性编程的英文是：Competitive Programming，直接拿来做名字感觉太长了，因此我把它写成了缩写，broadcast 是播报的意思，因此就用 cp-broadcast 来当名字了。
+
+这是本蒟蒻的第一个上传至 pypi 的 nonebot2 项目，可能有很多不完善的地方，欢迎大家来提 issue 和 pull requests。 
+
+有任何问题可联系QQ：3411907440。
+
 ## 💿 安装
 
 <details>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
     nb plugin install nonebot-plugin-cp-broadcast
@@ -91,28 +105,27 @@
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | cp_broadcast_list | 否 | [ ] | 开启早晨自动播报今日比赛的群聊，填 QQ 群号，注意以字符串形式填入 |
 | cp_broadcast_botname | 否 | "bot" | 填入你 bot 的名字，在 `help` 指令下会使用到你的 bot 的名字 |
-| cp_broadcast_time | 否 | {"hour":"7", "minute":"20"} | 每日在群聊播报比赛信息的时间，默认是早上 7 点 20，你可以在配置文件中按默认值格式修改成你想要的时间，注意需要安装 `nonebot_plugin_apscheduler` 插件以实现定时效果。 |
-| cp_broadcast_updatetime | 否 | {"hour":"0", "minute":"0"} | 每天自动更新比赛数据的时间，默认是 0 点 0 分，你可以在配置文件中按默认值格式修改成你想要的时间，注意需要安装 `nonebot_plugin_apscheduler` 插件以实现定时效果。 |
+| cp_broadcast_time | 否 | {"hour":"7", "minute":"20"} | 每日在群聊播报比赛信息的时间，默认是早上 7 点 20，你可以在配置文件中按默认值格式修改成你想要的时间 |
+| cp_broadcast_updatetime | 否 | {"hour":"0", "minute":"0"} | 每天自动更新比赛数据的时间，默认是 0 点 0 分，你可以在配置文件中按默认值格式修改成你想要的时间 |
+
+该插件依赖 [nonebot_plugin_apscheduler](https://github.com/nonebot/plugin-apscheduler) 实现定时发送功能，如果你是通过下载项目源码安装插件的话，请注意安装好依赖。
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | `cf` | 群员 | 否 | 群聊 | 发送最近三场 Codeforces 比赛的信息 |
 | `牛客` or `nc` | 群员 | 否 | 群聊 | 发送最近三场牛客比赛的信息 |
-| atc | 群员 | 否 | 群聊 | 发送最近两场 AtCoder 比赛的信息 |
-| today | 群员 | 否 | 群聊 | 发送今天的比赛信息 |
-| next | 群员 | 否 | 群聊 | 发送今天后的部分比赛信息 |
-| help | 群员 | 否 | 群聊 | 发送帮助信息 |
-| update | 群员 | 否 | 群聊 | 手动更新比赛信息 |
+| `atc` | 群员 | 否 | 群聊 | 发送最近两场 AtCoder 比赛的信息 |
+| `today` | 群员 | 否 | 群聊 | 发送今天的比赛信息 |
+| `next` | 群员 | 否 | 群聊 | 发送今天后的部分比赛信息 |
+| `help` | 群员 | 是 | 群聊 | 发送帮助信息 |
+| `update` | 群员 | 否 | 群聊 | 手动更新比赛信息 |
 ### 效果图
 <img src="./docs/preview.webp" style="zoom:30%;" />
 
-这是本蒟蒻的第一个上传至 pypi 的 nonebot 项目，可能有很多不完善的地方，欢迎大家来 pull requests。 
-
-有任何问题可联系QQ：3411907440
```

#### html2text {}

```diff
@@ -1,27 +1,40 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-cp-broadcast Version: 0.1.5 Summary:
-A nonebot plugin package License: MIT Author: HuParry Author-email:
-huparry@outlook.com Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
-Approved :: MIT License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: asyncio (>=3.4.3,<4.0.0) Requires-
-Dist: bs4 (>=0.0.1,<0.0.2) Requires-Dist: fake-useragent (>=1.1.3,<2.0.0)
-Requires-Dist: httpx (>=0.20.0,<1.0.0) Requires-Dist: nonebot-adapter-onebot
-(>=2.2.2,<3.0.0) Requires-Dist: nonebot-plugin-apscheduler (>=0.3.0,<0.4.0)
-Requires-Dist: nonebot2[fastapi] (>=2.0.0,<3.0.0) Description-Content-Type:
-text/markdown
+Metadata-Version: 2.1 Name: nonebot-plugin-cp-broadcast Version: 0.2.0 Summary:
+Codeforcesãçå®¢ãAtCoderå¹³å°æ¯èµæ¥è¯¢ï¼ACMer å¿å¤ Home-page:
+https://github.com/HuParry/nonebot-plugin-cp-broadcast License: MIT Author:
+HuParry Author-email: huparry@outlook.com Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: asyncio
+(>=3.4.3,<4.0.0) Requires-Dist: bs4 (>=0.0.1,<0.0.2) Requires-Dist: fake-
+useragent (>=1.1.3,<2.0.0) Requires-Dist: httpx (>=0.20.0,<1.0.0) Requires-
+Dist: nonebot-adapter-onebot (>=2.2.2,<3.0.0) Requires-Dist: nonebot-plugin-
+apscheduler (>=0.3.0,<0.4.0) Requires-Dist: nonebot2[fastapi] (>=2.0.0,<3.0.0)
+Project-URL: Repository, https://github.com/HuParry/nonebot-plugin-cp-broadcast
+Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # nonebot-plugin-cp-broadcast _â¨ ä¸ä¸ª Codeforcesãçå®¢ç«èµãAtCoder
 å¹³å°çç¼ç¨ç«èµæ¥è¯¢æä»¶ï¼ACMerå¿å¤ â¨_ [license] [pypi] [python]
 ## ð ä»ç» å¯¹äºæ¯ä¸ä¸ª ACMer
 æ¥è¯´ï¼åå ç¼ç¨ç«èµæ¯å¿ä¸å¯å°çï¼è¿ä¸ªæä»¶å®ç°äº
 Codeforcesãçå®¢ç«èµãAtCoder
-è¿ä¸ä¸ªä¸»æµçç¼ç¨ç«èµå¹³å°çæ¯èµæ¥è¯¢åæ­æ¥ã ## ð¿ å®è£
-ä½¿ç¨ nb-cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
+è¿ä¸ä¸ªä¸»æµçç¼ç¨ç«èµå¹³å°çæ¯èµæ¥è¯¢åæ­æ¥ã
+é¤äºç®åçæä»¤å¤ï¼å®æ¯ææ¯å¤©å®æ¶åéä¸ç§æ¯èµçä¿¡æ¯ã
+æ¥è¯¢çç»æä¼å­å°åè¡¨éï¼ä»¥åå°ç½ç«ç¬åçæ¬¡æ°ã ç±äº
+AtCoder ç½ç«æ²¡æä¾æ¯èµä¿¡æ¯ç
+APIï¼å æ­¤æ¯ç´æ¥å¯¹ç½é¡µè¿è¡ç¬åçï¼ä»£ç ä¸­æ¯ç¬åä¸¤ä¸ªæ¯èµï¼ä½ å¯ä»¥èªå·±ä¿®æ¹å¾æ´å¤ã
+ä¸ºä»ä¹å cp-broadcast
+è¿ä¸ªè±æåå¢ï¼å ä¸ºç«èµæ§ç¼ç¨çè±ææ¯ï¼Competitive
+Programmingï¼ç´æ¥æ¿æ¥ååå­æè§å¤ªé¿äºï¼å æ­¤ææå®åæäºç¼©åï¼broadcast
+æ¯æ­æ¥çææï¼å æ­¤å°±ç¨ cp-broadcast æ¥å½åå­äºã
+è¿æ¯æ¬èè»çç¬¬ä¸ä¸ªä¸ä¼ è³ pypi ç nonebot2
+é¡¹ç®ï¼å¯è½æå¾å¤ä¸å®åçå°æ¹ï¼æ¬¢è¿å¤§å®¶æ¥æ issue å pull
+requestsã æä»»ä½é®é¢å¯èç³»QQï¼3411907440ã ## ð¿ å®è£  ä½¿ç¨
+nb-cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-cp-broadcast
 ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-cp-broadcast   pdm pdm add nonebot-plugin-cp-
 broadcast   poetry poetry add nonebot-plugin-cp-broadcast   conda conda install
 nonebot-plugin-cp-broadcast  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
@@ -29,25 +42,23 @@
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
 é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | cp_broadcast_list | å¦ |
 [ ] | å¼å¯æ©æ¨èªå¨æ­æ¥ä»æ¥æ¯èµçç¾¤èï¼å¡« QQ
 ç¾¤å·ï¼æ³¨æä»¥å­ç¬¦ä¸²å½¢å¼å¡«å¥ | | cp_broadcast_botname | å¦ | "bot"
 | å¡«å¥ä½  bot çåå­ï¼å¨ `help` æä»¤ä¸ä¼ä½¿ç¨å°ä½ ç bot
 çåå­ | | cp_broadcast_time | å¦ | {"hour":"7", "minute":"20"} |
 æ¯æ¥å¨ç¾¤èæ­æ¥æ¯èµä¿¡æ¯çæ¶é´ï¼é»è®¤æ¯æ©ä¸ 7 ç¹
-20ï¼ä½ å¯ä»¥å¨éç½®æä»¶ä¸­æé»è®¤å¼æ ¼å¼ä¿®æ¹æä½ æ³è¦çæ¶é´ï¼æ³¨æéè¦å®è£
-`nonebot_plugin_apscheduler` æä»¶ä»¥å®ç°å®æ¶ææã | |
-cp_broadcast_updatetime | å¦ | {"hour":"0", "minute":"0"} |
+20ï¼ä½ å¯ä»¥å¨éç½®æä»¶ä¸­æé»è®¤å¼æ ¼å¼ä¿®æ¹æä½ æ³è¦çæ¶é´ |
+| cp_broadcast_updatetime | å¦ | {"hour":"0", "minute":"0"} |
 æ¯å¤©èªå¨æ´æ°æ¯èµæ°æ®çæ¶é´ï¼é»è®¤æ¯ 0 ç¹ 0
-åï¼ä½ å¯ä»¥å¨éç½®æä»¶ä¸­æé»è®¤å¼æ ¼å¼ä¿®æ¹æä½ æ³è¦çæ¶é´ï¼æ³¨æéè¦å®è£
-`nonebot_plugin_apscheduler` æä»¶ä»¥å®ç°å®æ¶ææã | ## ð ä½¿ç¨
-### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:
-----:|:----:|:----:| | `cf` | ç¾¤å | å¦ | ç¾¤è | åéæè¿ä¸åº
-Codeforces æ¯èµçä¿¡æ¯ | | `çå®¢` or `nc` | ç¾¤å | å¦ | ç¾¤è |
-åéæè¿ä¸åºçå®¢æ¯èµçä¿¡æ¯ | | atc | ç¾¤å | å¦ | ç¾¤è |
-åéæè¿ä¸¤åº AtCoder æ¯èµçä¿¡æ¯ | | today | ç¾¤å | å¦ | ç¾¤è |
-åéä»å¤©çæ¯èµä¿¡æ¯ | | next | ç¾¤å | å¦ | ç¾¤è |
-åéä»å¤©åçé¨åæ¯èµä¿¡æ¯ | | help | ç¾¤å | å¦ | ç¾¤è |
-åéå¸®å©ä¿¡æ¯ | | update | ç¾¤å | å¦ | ç¾¤è |
+åï¼ä½ å¯ä»¥å¨éç½®æä»¶ä¸­æé»è®¤å¼æ ¼å¼ä¿®æ¹æä½ æ³è¦çæ¶é´
+| è¯¥æä»¶ä¾èµ [nonebot_plugin_apscheduler](https://github.com/nonebot/
+plugin-apscheduler)
+å®ç°å®æ¶åéåè½ï¼å¦æä½ æ¯éè¿ä¸è½½é¡¹ç®æºç å®è£æä»¶çè¯ï¼è¯·æ³¨æå®è£å¥½ä¾èµã
+## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:
+-----:|:----:|:----:|:----:|:----:| | `cf` | ç¾¤å | å¦ | ç¾¤è |
+åéæè¿ä¸åº Codeforces æ¯èµçä¿¡æ¯ | | `çå®¢` or `nc` | ç¾¤å |
+å¦ | ç¾¤è | åéæè¿ä¸åºçå®¢æ¯èµçä¿¡æ¯ | | `atc` | ç¾¤å | å¦
+| ç¾¤è | åéæè¿ä¸¤åº AtCoder æ¯èµçä¿¡æ¯ | | `today` | ç¾¤å |
+å¦ | ç¾¤è | åéä»å¤©çæ¯èµä¿¡æ¯ | | `next` | ç¾¤å | å¦ | ç¾¤è |
+åéä»å¤©åçé¨åæ¯èµä¿¡æ¯ | | `help` | ç¾¤å | æ¯ | ç¾¤è |
+åéå¸®å©ä¿¡æ¯ | | `update` | ç¾¤å | å¦ | ç¾¤è |
 æå¨æ´æ°æ¯èµä¿¡æ¯ | ### ææå¾ [./docs/preview.webp]
-è¿æ¯æ¬èè»çç¬¬ä¸ä¸ªä¸ä¼ è³ pypi ç nonebot
-é¡¹ç®ï¼å¯è½æå¾å¤ä¸å®åçå°æ¹ï¼æ¬¢è¿å¤§å®¶æ¥ pull requestsã
-æä»»ä½é®é¢å¯èç³»QQï¼3411907440
```

