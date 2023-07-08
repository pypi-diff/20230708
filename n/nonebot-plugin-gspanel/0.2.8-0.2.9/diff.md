# Comparing `tmp/nonebot_plugin_gspanel-0.2.8.tar.gz` & `tmp/nonebot_plugin_gspanel-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_gspanel-0.2.8.tar", max compression
+gzip compressed data, was "nonebot_plugin_gspanel-0.2.9.tar", max compression
```

## Comparing `nonebot_plugin_gspanel-0.2.8.tar` & `nonebot_plugin_gspanel-0.2.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1086 2022-11-27 11:19:21.255038 nonebot_plugin_gspanel-0.2.8/LICENSE
--rw-r--r--   0        0        0     8213 2022-11-27 11:19:21.255038 nonebot_plugin_gspanel-0.2.8/README.md
--rw-r--r--   0        0        0     3687 2022-11-27 11:19:21.311039 nonebot_plugin_gspanel-0.2.8/nonebot_plugin_gspanel/__init__.py
--rw-r--r--   0        0        0    13933 2022-11-27 11:19:21.311039 nonebot_plugin_gspanel-0.2.8/nonebot_plugin_gspanel/__utils__.py
--rw-r--r--   0        0        0    29437 2022-11-27 11:19:21.311039 nonebot_plugin_gspanel-0.2.8/nonebot_plugin_gspanel/data_convert.py
--rw-r--r--   0        0        0    13306 2022-11-27 11:19:21.311039 nonebot_plugin_gspanel-0.2.8/nonebot_plugin_gspanel/data_source.py
--rw-r--r--   0        0        0     4146 2022-11-27 11:19:21.311039 nonebot_plugin_gspanel-0.2.8/nonebot_plugin_gspanel/data_updater.py
--rw-r--r--   0        0        0      737 2022-11-27 11:19:21.311039 nonebot_plugin_gspanel-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     9040 1970-01-01 00:00:00.000000 nonebot_plugin_gspanel-0.2.8/setup.py
--rw-r--r--   0        0        0     9039 1970-01-01 00:00:00.000000 nonebot_plugin_gspanel-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1086 2022-12-16 12:02:19.165911 nonebot_plugin_gspanel-0.2.9/LICENSE
+-rw-r--r--   0        0        0     8549 2022-12-16 12:02:19.165911 nonebot_plugin_gspanel-0.2.9/README.md
+-rw-r--r--   0        0        0     3687 2022-12-16 12:02:19.217911 nonebot_plugin_gspanel-0.2.9/nonebot_plugin_gspanel/__init__.py
+-rw-r--r--   0        0        0    13933 2022-12-16 12:02:19.217911 nonebot_plugin_gspanel-0.2.9/nonebot_plugin_gspanel/__utils__.py
+-rw-r--r--   0        0        0    29437 2022-12-16 12:02:19.217911 nonebot_plugin_gspanel-0.2.9/nonebot_plugin_gspanel/data_convert.py
+-rw-r--r--   0        0        0    13372 2022-12-16 12:02:19.217911 nonebot_plugin_gspanel-0.2.9/nonebot_plugin_gspanel/data_source.py
+-rw-r--r--   0        0        0     4146 2022-12-16 12:02:19.217911 nonebot_plugin_gspanel-0.2.9/nonebot_plugin_gspanel/data_updater.py
+-rw-r--r--   0        0        0      737 2022-12-16 12:02:19.217911 nonebot_plugin_gspanel-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     9376 1970-01-01 00:00:00.000000 nonebot_plugin_gspanel-0.2.9/setup.py
+-rw-r--r--   0        0        0     9364 1970-01-01 00:00:00.000000 nonebot_plugin_gspanel-0.2.9/PKG-INFO
```

### Comparing `nonebot_plugin_gspanel-0.2.8/LICENSE` & `nonebot_plugin_gspanel-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gspanel-0.2.8/README.md` & `nonebot_plugin_gspanel-0.2.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,22 +33,33 @@
 python3 -m nb_cli plugin install nonebot-plugin-gspanel
 
 # 或从 PyPI 安装
 python3 -m pip install nonebot-plugin-gspanel
 ```
 
 
-> **[@realhuhu/py-plugin](https://github.com/realhuhu/py-plugin) 插件用户须知**
+> **[@realhuhu/py-plugin](https://github.com/realhuhu/py-plugin) 插件用户安装方法**
 > 
-> Yunzai 用户安装 py-plugin 插件后可以兼容运行本插件！安装步骤如下：
+> Yunzai 用户安装 py-plugin 插件后可以兼容运行此插件！安装步骤如下：
 > 
 > 1. 仔细阅读 [README.md](https://github.com/realhuhu/py-plugin#21-%E5%AE%89%E8%A3%85) 配置 Yunzai Bot 的 Python 运行环境
-> 2. 向 Yunzai Bot 发送 QQ 消息 `#py下载插件nonebot-plugin-gspanel` 安装本插件
+> 2. 向 Yunzai Bot 发送 QQ 消息 `#py下载插件nonebot-plugin-gspanel` 安装此插件
 > 3. [建议] 将下方使用须知第 4 条中交待的所有环境变量写入 py-plugin 的配置文件 config.yaml 中（注意格式）
-> 4. [建议] 将环境变量 `gspanel_alias` 定义为 `面板` 以外的关键词，避免此插件的功能与 Yunzai 相关功能同时触发
+> 4. [建议] 将环境变量 `gspanel_alias` 定义为 `面板` 以外的触发词，避免此插件与 Yunzai 相关功能同时触发
+> 
+> py-plugin 的配置文件 config.yaml 中 **务必手动添加** 此插件的一些配置：
+> 
+> ```yaml
+> gspanel_alias:
+>   - 想要的面板触发词
+>   - 支持多个触发词
+> gspanel_scale: 1.0
+> resources_dir: /path/to/data  # Windows 要将反斜杠替换为 /
+> resources_mirror: https://enka.network/ui/
+> ```
 
 
 ## 使用须知
 
 
  - 插件的圣遗物评分计算规则、卡片样式均来自 [@yoimiya-kokomi/miao-plugin](https://github.com/yoimiya-kokomi/miao-plugin)。插件移植时对 **评分规则** 主要做了以下修改：
```

#### html2text {}

```diff
@@ -6,24 +6,29 @@
 images.githubusercontent.com/22407052/201661930-f9ecdfe0-e278-4641-a012-
 cf090da6b6c7.PNG) | ![å¦®é²](https://user-images.githubusercontent.com/
 22407052/201667744-decfdf25-c889-4a65-bbe0-94e194fe8d82.PNG) | |:--:|:--:|:--:
 | ## å®è£æ¹æ³ å¦æä½ æ­£å¨ä½¿ç¨ 2.0.0.beta1 ä»¥ä¸çæ¬
 NoneBotï¼æ¨èä½¿ç¨ä»¥ä¸å½ä»¤å®è£ï¼ ```bash # ä» nb_cli å®è£ python3
 -m nb_cli plugin install nonebot-plugin-gspanel # æä» PyPI å®è£ python3 -
 m pip install nonebot-plugin-gspanel ``` > **[@realhuhu/py-plugin](https://
-github.com/realhuhu/py-plugin) æä»¶ç¨æ·é¡»ç¥** > > Yunzai ç¨æ·å®è£ py-
-plugin æä»¶åå¯ä»¥å¼å®¹è¿è¡æ¬æä»¶ï¼å®è£æ­¥éª¤å¦ä¸ï¼ > > 1.
+github.com/realhuhu/py-plugin) æä»¶ç¨æ·å®è£æ¹æ³** > > Yunzai
+ç¨æ·å®è£ py-plugin
+æä»¶åå¯ä»¥å¼å®¹è¿è¡æ­¤æä»¶ï¼å®è£æ­¥éª¤å¦ä¸ï¼ > > 1.
 ä»ç»éè¯» [README.md](https://github.com/realhuhu/py-plugin#21-
 %E5%AE%89%E8%A3%85) éç½® Yunzai Bot ç Python è¿è¡ç¯å¢ > 2. å Yunzai
-Bot åé QQ æ¶æ¯ `#pyä¸è½½æä»¶nonebot-plugin-gspanel` å®è£æ¬æä»¶ >
+Bot åé QQ æ¶æ¯ `#pyä¸è½½æä»¶nonebot-plugin-gspanel` å®è£æ­¤æä»¶ >
 3. [å»ºè®®] å°ä¸æ¹ä½¿ç¨é¡»ç¥ç¬¬ 4 æ¡ä¸­äº¤å¾çææç¯å¢åéåå¥
 py-plugin çéç½®æä»¶ config.yaml ä¸­ï¼æ³¨ææ ¼å¼ï¼ > 4. [å»ºè®®]
 å°ç¯å¢åé `gspanel_alias` å®ä¹ä¸º `é¢æ¿`
-ä»¥å¤çå³é®è¯ï¼é¿åæ­¤æä»¶çåè½ä¸ Yunzai
-ç¸å³åè½åæ¶è§¦å ## ä½¿ç¨é¡»ç¥ -
+ä»¥å¤çè§¦åè¯ï¼é¿åæ­¤æä»¶ä¸ Yunzai ç¸å³åè½åæ¶è§¦å > > py-
+plugin çéç½®æä»¶ config.yaml ä¸­ **å¡å¿æå¨æ·»å **
+æ­¤æä»¶çä¸äºéç½®ï¼ > > ```yaml > gspanel_alias: > -
+æ³è¦çé¢æ¿è§¦åè¯ > - æ¯æå¤ä¸ªè§¦åè¯ > gspanel_scale: 1.0 >
+resources_dir: /path/to/data # Windows è¦å°åææ æ¿æ¢ä¸º / >
+resources_mirror: https://enka.network/ui/ > ``` ## ä½¿ç¨é¡»ç¥ -
 æä»¶çå£éç©è¯åè®¡ç®è§åãå¡çæ ·å¼åæ¥èª [@yoimiya-kokomi/
 miao-plugin](https://github.com/yoimiya-kokomi/miao-
 plugin)ãæä»¶ç§»æ¤æ¶å¯¹ **è¯åè§å** ä¸»è¦åäºä»¥ä¸ä¿®æ¹ï¼ +
 ä»¥è§è²çå½å¼ãæ»å»åãé²å¾¡åçå®éåºç¡å¼è¿è¡è¯æ¡å¾åè®¡ç®ï¼å¯¼è´åºå®å¼ççå½å¼ãæ»å»åãé²å¾¡åè¯æ¡è¯åç¸è¾åçæå°å¹åº¦æ³¢å¨
 +
 äºé¢æ¿æ°æ®åºåå±ç¤ºå£éç©è¯åä½¿ç¨çè¯æ¡æéè§åï¼æä»¶å°æªèªå®ä¹è¯æ¡æéè§åçè§è²ä½¿ç¨é»è®¤è§åï¼æ»å»å
 `75`ãæ´å»ç `100`ãæ´å»ä¼¤å®³ `100`ï¼ +
```

### Comparing `nonebot_plugin_gspanel-0.2.8/nonebot_plugin_gspanel/__init__.py` & `nonebot_plugin_gspanel-0.2.9/nonebot_plugin_gspanel/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gspanel-0.2.8/nonebot_plugin_gspanel/__utils__.py` & `nonebot_plugin_gspanel-0.2.9/nonebot_plugin_gspanel/__utils__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gspanel-0.2.8/nonebot_plugin_gspanel/data_convert.py` & `nonebot_plugin_gspanel-0.2.9/nonebot_plugin_gspanel/data_convert.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gspanel-0.2.8/nonebot_plugin_gspanel/data_source.py` & `nonebot_plugin_gspanel-0.2.9/nonebot_plugin_gspanel/data_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,22 @@
 import json
 from copy import deepcopy
 from time import time
 from traceback import format_exc
 from typing import Dict, List, Literal, Union
 
 from httpx import AsyncClient, HTTPError
-from nonebot_plugin_htmlrender import template_to_pic
 
+from nonebot import require
 from nonebot.log import logger
 
-from .__utils__ import LOCAL_DIR, TPL_VERSION, SCALE_FACTOR, download
+require("nonebot_plugin_htmlrender")
+from nonebot_plugin_htmlrender import template_to_pic
+
+from .__utils__ import LOCAL_DIR, SCALE_FACTOR, TPL_VERSION, download
 from .data_convert import (
     simplDamageRes,
     simplFightProp,
     simplTeamDamageRes,
     transFromEnka,
     transToTeyvat,
 )
```

### Comparing `nonebot_plugin_gspanel-0.2.8/nonebot_plugin_gspanel/data_updater.py` & `nonebot_plugin_gspanel-0.2.9/nonebot_plugin_gspanel/data_updater.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gspanel-0.2.8/pyproject.toml` & `nonebot_plugin_gspanel-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-gspanel"
-version = "0.2.8"
+version = "0.2.9"
 description = "Genshin player cards plugin for NoneBot2"
 authors = ["monsterxcn <monsterxcn@gmail.com>"]
 documentation = "https://github.com/monsterxcn/nonebot-plugin-gspanel#readme"
 license = "MIT"
 homepage = "https://github.com/monsterxcn/nonebot-plugin-gspanel"
 readme = "README.md"
 keywords = ["nonebot", "nonebot2", "genshin", "panel", "card"]
```

### Comparing `nonebot_plugin_gspanel-0.2.8/setup.py` & `nonebot_plugin_gspanel-0.2.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,17 @@
  'nonebot-adapter-onebot>=2.0.0b1',
  'nonebot-plugin-htmlrender>=0.2.0.1',
  'nonebot2>=2.0.0b3',
  'playwright>=1.25.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-gspanel',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'Genshin player cards plugin for NoneBot2',
-    'long_description': '<h1 align="center">NoneBot Plugin GsPanel</h1></br>\n\n\n<p align="center">🤖 用于展示原神游戏内角色展柜数据的 NoneBot2 插件</p></br>\n\n\n<p align="center">\n  <a href="https://github.com/monsterxcn/nonebot-plugin-gspanel/actions">\n    <img src="https://img.shields.io/github/workflow/status/monsterxcn/nonebot-plugin-gspanel/Build%20distributions?style=flat-square" alt="actions">\n  </a>\n  <a href="https://raw.githubusercontent.com/monsterxcn/nonebot-plugin-gspanel/master/LICENSE">\n    <img src="https://img.shields.io/github/license/monsterxcn/nonebot-plugin-gspanel?style=flat-square" alt="license">\n  </a>\n  <a href="https://pypi.python.org/pypi/nonebot-plugin-gspanel">\n    <img src="https://img.shields.io/pypi/v/nonebot-plugin-gspanel?style=flat-square" alt="pypi">\n  </a>\n  <img src="https://img.shields.io/badge/python-3.8+-blue?style=flat-square" alt="python"><br />\n</p></br>\n\n\n| ![琴](https://user-images.githubusercontent.com/22407052/201662130-2b3bdcd3-acaa-4b59-9c88-3e50fa1887f3.PNG) | ![刻晴](https://user-images.githubusercontent.com/22407052/201661930-f9ecdfe0-e278-4641-a012-cf090da6b6c7.PNG) | ![妮露](https://user-images.githubusercontent.com/22407052/201667744-decfdf25-c889-4a65-bbe0-94e194fe8d82.PNG) |\n|:--:|:--:|:--:|\n\n\n## 安装方法\n\n\n如果你正在使用 2.0.0.beta1 以上版本 NoneBot，推荐使用以下命令安装：\n\n\n```bash\n# 从 nb_cli 安装\npython3 -m nb_cli plugin install nonebot-plugin-gspanel\n\n# 或从 PyPI 安装\npython3 -m pip install nonebot-plugin-gspanel\n```\n\n\n> **[@realhuhu/py-plugin](https://github.com/realhuhu/py-plugin) 插件用户须知**\n> \n> Yunzai 用户安装 py-plugin 插件后可以兼容运行本插件！安装步骤如下：\n> \n> 1. 仔细阅读 [README.md](https://github.com/realhuhu/py-plugin#21-%E5%AE%89%E8%A3%85) 配置 Yunzai Bot 的 Python 运行环境\n> 2. 向 Yunzai Bot 发送 QQ 消息 `#py下载插件nonebot-plugin-gspanel` 安装本插件\n> 3. [建议] 将下方使用须知第 4 条中交待的所有环境变量写入 py-plugin 的配置文件 config.yaml 中（注意格式）\n> 4. [建议] 将环境变量 `gspanel_alias` 定义为 `面板` 以外的关键词，避免此插件的功能与 Yunzai 相关功能同时触发\n\n\n## 使用须知\n\n\n - 插件的圣遗物评分计算规则、卡片样式均来自 [@yoimiya-kokomi/miao-plugin](https://github.com/yoimiya-kokomi/miao-plugin)。插件移植时对 **评分规则** 主要做了以下修改：\n   \n   + 以角色生命值、攻击力、防御力的实际基础值进行词条得分计算，导致固定值的生命值、攻击力、防御力词条评分相较原版有小幅度波动\n   + 于面板数据区域展示圣遗物评分使用的词条权重规则，插件尚未自定义词条权重规则的角色使用默认规则（攻击力 `75`、暴击率 `100`、暴击伤害 `100`）\n   + 于面板数据区域展示角色最高的伤害加成数据，该属性与角色实际伤害属性不一致时区别显示词条权重规则\n   + 对元素属性异常的空之杯进行评分惩罚，扣除该圣遗物总分的 50%（最大扣除比例）\n   \n - 插件返回「暂时无法访问面板数据接口..」可能的原因有：Bot 与 [Enka.Network](https://enka.network/) 的连接不稳定；[Enka.Network](https://enka.network/) 服务器暂时故障等。\n   \n - 插件首次生成某个角色的面板图片时，会尝试从 [Enka.Network](https://enka.network/) 下载该角色的抽卡大图、命座图片、技能图片、圣遗物及武器图片等素材图片，生成面板图片的时间由 Bot 与 [Enka.Network](https://enka.network/) 的连接质量决定。素材图片下载至本地后将不再从远程下载，生成面板图片的时间将大幅缩短。\n   \n - 一般来说，插件安装完成后无需设置环境变量，只需重启 Bot 即可开始使用。你也可以在 NoneBot2 当前使用的 `.env` 文件中添加下表给出的环境变量，对插件进行更多配置。环境变量修改后需要重启 Bot 才能生效。\n   \n   | 环境变量 | 必需 | 默认 | 说明 |\n   |:-------|:----:|:-----|:----|\n   | `gspanel_alias` | 否 | `["面板"]` | 插件响应词别名，多个别名按 `["面面", "板板"]` 格式填写 |\n   | `gspanel_scale` | 否 | `1.0` | 浏览器缩放比例，此值越大返回图片的分辨率越高 |\n   | `resources_dir` | 否 | `/path/to/bot/data/` | 插件数据缓存目录的父文件夹，包含 `gspanel` 文件夹的上级文件夹路径 |\n   | `resources_mirror` | 否 | `https://enka.network/ui/` | 素材图片下载镜像，需提供 `UI_Talent_S_Nilou_01.png` 形式的图片地址，可选镜像：<br>`http://file.microgg.cn/ui/`（小灰灰）<br>`https://api.ambr.top/assets/UI/`（安柏计划）<br>`https://cdn.monsterx.cn/genshin/`（插件作者） |\n   \n - 插件图片生成采用 [@kexue-z/nonebot-plugin-htmlrender](https://github.com/kexue-z/nonebot-plugin-htmlrender)，若插件自动安装运行 Chromium 所需的额外依赖失败，请参考 [@SK-415/HarukaBot](https://haruka-bot.sk415.icu/faq.html#playwright-%E4%BE%9D%E8%B5%96%E4%B8%8D%E5%85%A8) 给出的以下解决方案：\n   \n   + Ubuntu：`python3 -m playwright install-deps`\n   + CentOS（仅供参考）：`yum install -y atk at-spi2-atk cups-libs libxkbcommon libXcomposite libXdamage libXrandr mesa-libgbm gtk3`\n   + 其他非 Ubuntu 系统：[@microsoft/playwright/issues](https://github.com/microsoft/playwright/issues)\n\n\n## 命令说明\n\n\n### 角色面板\n\n\n插件响应以 `panel` / `面板` 开头的消息，下面仅以 `面板` 为例：\n\n\n*\\*如果定义了环境变量 `gspanel_alias` 则以环境变量定义的命令别名为准，默认情况下该环境变量会使插件响应 `面板` 开头的消息。*\n\n\n - `面板绑定100123456`\n   \n   绑定 UID `100123456` 至发送此指令的 QQ，QQ 已被绑定过则会更新绑定的 UID。\n   \n   Bot 管理员可以通过在此指令后附带 `@某人` 或 `2334556789` 的方式将 UID `100123456` 绑定至指定的 QQ。\n   \n - `面板100123456`\n   \n   查找 UID `100123456` 角色展柜中展示的所有角色（文本）。\n   \n   仅发送 `面板` 时将尝试使用发送此指令的 QQ 绑定的 UID；发送 `面板@某人` 时将尝试使用指定 QQ 绑定的 UID。\n   \n - `面板夜兰100123456` / `面板100123456夜兰`\n   \n   查找 UID `100123456` 的夜兰面板（图片）。\n   \n   仅发送 `面板夜兰` 时将尝试使用发送此指令的 QQ 绑定的 UID；发送 `面板夜兰@某人` 时将尝试使用指定 QQ 绑定的 UID。\n\n\n*\\* 所有指令都可以用空格将关键词分割开来，如果你喜欢的话。*\n\n\n### 队伍伤害\n\n\n插件响应以 `teamdmg` / `队伍伤害` 开头的消息，下面仅以 `队伍伤害` 为例：\n\n\n - `队伍伤害` / `队伍伤害100123456` / `队伍伤害@某人`\n   \n   查找指定 UID 角色展柜中前四个角色组成的队伍伤害。\n   \n   当仅发送 `队伍伤害` 时将尝试使用发送此指令的 QQ 绑定的 UID；附带 9 位数字时尝试使用该 UID；附带 `@某人` 时将尝试使用指定 QQ 绑定的 UID。\n   \n - `队伍伤害雷九万班` / `队伍伤害 雷神 九条 万叶 班尼特` / `队伍伤害雷神 九条 万叶 班尼特@某人`\n   \n   查找雷电将军、九条裟罗、枫原万叶、班尼特组成的队伍伤害。注意角色名之间必须使用空格分开。含有 **旅行者** 的配队暂时无法查询。\n   \n   为此形式的命令指定 UID 方式与上面相同。\n   \n   队伍别名支持可能不全请见谅，如果有十分流行的配队未能支持请提出 issue 耐心等待适配。\n\n\n*\\* 队伍伤害为 **实验性功能**，计算结果可能存在问题。欢迎附带详细日志提交 issue 帮助改进此功能。*\n\n\n## 特别鸣谢\n\n\n[@nonebot/nonebot2](https://github.com/nonebot/nonebot2/) | [@Mrs4s/go-cqhttp](https://github.com/Mrs4s/go-cqhttp) | [@yoimiya-kokomi/miao-plugin](https://github.com/yoimiya-kokomi/miao-plugin) | [Enka.Network](https://enka.network/) | [Miniprogram Teyvat Helper](#)\n',
+    'long_description': '<h1 align="center">NoneBot Plugin GsPanel</h1></br>\n\n\n<p align="center">🤖 用于展示原神游戏内角色展柜数据的 NoneBot2 插件</p></br>\n\n\n<p align="center">\n  <a href="https://github.com/monsterxcn/nonebot-plugin-gspanel/actions">\n    <img src="https://img.shields.io/github/workflow/status/monsterxcn/nonebot-plugin-gspanel/Build%20distributions?style=flat-square" alt="actions">\n  </a>\n  <a href="https://raw.githubusercontent.com/monsterxcn/nonebot-plugin-gspanel/master/LICENSE">\n    <img src="https://img.shields.io/github/license/monsterxcn/nonebot-plugin-gspanel?style=flat-square" alt="license">\n  </a>\n  <a href="https://pypi.python.org/pypi/nonebot-plugin-gspanel">\n    <img src="https://img.shields.io/pypi/v/nonebot-plugin-gspanel?style=flat-square" alt="pypi">\n  </a>\n  <img src="https://img.shields.io/badge/python-3.8+-blue?style=flat-square" alt="python"><br />\n</p></br>\n\n\n| ![琴](https://user-images.githubusercontent.com/22407052/201662130-2b3bdcd3-acaa-4b59-9c88-3e50fa1887f3.PNG) | ![刻晴](https://user-images.githubusercontent.com/22407052/201661930-f9ecdfe0-e278-4641-a012-cf090da6b6c7.PNG) | ![妮露](https://user-images.githubusercontent.com/22407052/201667744-decfdf25-c889-4a65-bbe0-94e194fe8d82.PNG) |\n|:--:|:--:|:--:|\n\n\n## 安装方法\n\n\n如果你正在使用 2.0.0.beta1 以上版本 NoneBot，推荐使用以下命令安装：\n\n\n```bash\n# 从 nb_cli 安装\npython3 -m nb_cli plugin install nonebot-plugin-gspanel\n\n# 或从 PyPI 安装\npython3 -m pip install nonebot-plugin-gspanel\n```\n\n\n> **[@realhuhu/py-plugin](https://github.com/realhuhu/py-plugin) 插件用户安装方法**\n> \n> Yunzai 用户安装 py-plugin 插件后可以兼容运行此插件！安装步骤如下：\n> \n> 1. 仔细阅读 [README.md](https://github.com/realhuhu/py-plugin#21-%E5%AE%89%E8%A3%85) 配置 Yunzai Bot 的 Python 运行环境\n> 2. 向 Yunzai Bot 发送 QQ 消息 `#py下载插件nonebot-plugin-gspanel` 安装此插件\n> 3. [建议] 将下方使用须知第 4 条中交待的所有环境变量写入 py-plugin 的配置文件 config.yaml 中（注意格式）\n> 4. [建议] 将环境变量 `gspanel_alias` 定义为 `面板` 以外的触发词，避免此插件与 Yunzai 相关功能同时触发\n> \n> py-plugin 的配置文件 config.yaml 中 **务必手动添加** 此插件的一些配置：\n> \n> ```yaml\n> gspanel_alias:\n>   - 想要的面板触发词\n>   - 支持多个触发词\n> gspanel_scale: 1.0\n> resources_dir: /path/to/data  # Windows 要将反斜杠替换为 /\n> resources_mirror: https://enka.network/ui/\n> ```\n\n\n## 使用须知\n\n\n - 插件的圣遗物评分计算规则、卡片样式均来自 [@yoimiya-kokomi/miao-plugin](https://github.com/yoimiya-kokomi/miao-plugin)。插件移植时对 **评分规则** 主要做了以下修改：\n   \n   + 以角色生命值、攻击力、防御力的实际基础值进行词条得分计算，导致固定值的生命值、攻击力、防御力词条评分相较原版有小幅度波动\n   + 于面板数据区域展示圣遗物评分使用的词条权重规则，插件尚未自定义词条权重规则的角色使用默认规则（攻击力 `75`、暴击率 `100`、暴击伤害 `100`）\n   + 于面板数据区域展示角色最高的伤害加成数据，该属性与角色实际伤害属性不一致时区别显示词条权重规则\n   + 对元素属性异常的空之杯进行评分惩罚，扣除该圣遗物总分的 50%（最大扣除比例）\n   \n - 插件返回「暂时无法访问面板数据接口..」可能的原因有：Bot 与 [Enka.Network](https://enka.network/) 的连接不稳定；[Enka.Network](https://enka.network/) 服务器暂时故障等。\n   \n - 插件首次生成某个角色的面板图片时，会尝试从 [Enka.Network](https://enka.network/) 下载该角色的抽卡大图、命座图片、技能图片、圣遗物及武器图片等素材图片，生成面板图片的时间由 Bot 与 [Enka.Network](https://enka.network/) 的连接质量决定。素材图片下载至本地后将不再从远程下载，生成面板图片的时间将大幅缩短。\n   \n - 一般来说，插件安装完成后无需设置环境变量，只需重启 Bot 即可开始使用。你也可以在 NoneBot2 当前使用的 `.env` 文件中添加下表给出的环境变量，对插件进行更多配置。环境变量修改后需要重启 Bot 才能生效。\n   \n   | 环境变量 | 必需 | 默认 | 说明 |\n   |:-------|:----:|:-----|:----|\n   | `gspanel_alias` | 否 | `["面板"]` | 插件响应词别名，多个别名按 `["面面", "板板"]` 格式填写 |\n   | `gspanel_scale` | 否 | `1.0` | 浏览器缩放比例，此值越大返回图片的分辨率越高 |\n   | `resources_dir` | 否 | `/path/to/bot/data/` | 插件数据缓存目录的父文件夹，包含 `gspanel` 文件夹的上级文件夹路径 |\n   | `resources_mirror` | 否 | `https://enka.network/ui/` | 素材图片下载镜像，需提供 `UI_Talent_S_Nilou_01.png` 形式的图片地址，可选镜像：<br>`http://file.microgg.cn/ui/`（小灰灰）<br>`https://api.ambr.top/assets/UI/`（安柏计划）<br>`https://cdn.monsterx.cn/genshin/`（插件作者） |\n   \n - 插件图片生成采用 [@kexue-z/nonebot-plugin-htmlrender](https://github.com/kexue-z/nonebot-plugin-htmlrender)，若插件自动安装运行 Chromium 所需的额外依赖失败，请参考 [@SK-415/HarukaBot](https://haruka-bot.sk415.icu/faq.html#playwright-%E4%BE%9D%E8%B5%96%E4%B8%8D%E5%85%A8) 给出的以下解决方案：\n   \n   + Ubuntu：`python3 -m playwright install-deps`\n   + CentOS（仅供参考）：`yum install -y atk at-spi2-atk cups-libs libxkbcommon libXcomposite libXdamage libXrandr mesa-libgbm gtk3`\n   + 其他非 Ubuntu 系统：[@microsoft/playwright/issues](https://github.com/microsoft/playwright/issues)\n\n\n## 命令说明\n\n\n### 角色面板\n\n\n插件响应以 `panel` / `面板` 开头的消息，下面仅以 `面板` 为例：\n\n\n*\\*如果定义了环境变量 `gspanel_alias` 则以环境变量定义的命令别名为准，默认情况下该环境变量会使插件响应 `面板` 开头的消息。*\n\n\n - `面板绑定100123456`\n   \n   绑定 UID `100123456` 至发送此指令的 QQ，QQ 已被绑定过则会更新绑定的 UID。\n   \n   Bot 管理员可以通过在此指令后附带 `@某人` 或 `2334556789` 的方式将 UID `100123456` 绑定至指定的 QQ。\n   \n - `面板100123456`\n   \n   查找 UID `100123456` 角色展柜中展示的所有角色（文本）。\n   \n   仅发送 `面板` 时将尝试使用发送此指令的 QQ 绑定的 UID；发送 `面板@某人` 时将尝试使用指定 QQ 绑定的 UID。\n   \n - `面板夜兰100123456` / `面板100123456夜兰`\n   \n   查找 UID `100123456` 的夜兰面板（图片）。\n   \n   仅发送 `面板夜兰` 时将尝试使用发送此指令的 QQ 绑定的 UID；发送 `面板夜兰@某人` 时将尝试使用指定 QQ 绑定的 UID。\n\n\n*\\* 所有指令都可以用空格将关键词分割开来，如果你喜欢的话。*\n\n\n### 队伍伤害\n\n\n插件响应以 `teamdmg` / `队伍伤害` 开头的消息，下面仅以 `队伍伤害` 为例：\n\n\n - `队伍伤害` / `队伍伤害100123456` / `队伍伤害@某人`\n   \n   查找指定 UID 角色展柜中前四个角色组成的队伍伤害。\n   \n   当仅发送 `队伍伤害` 时将尝试使用发送此指令的 QQ 绑定的 UID；附带 9 位数字时尝试使用该 UID；附带 `@某人` 时将尝试使用指定 QQ 绑定的 UID。\n   \n - `队伍伤害雷九万班` / `队伍伤害 雷神 九条 万叶 班尼特` / `队伍伤害雷神 九条 万叶 班尼特@某人`\n   \n   查找雷电将军、九条裟罗、枫原万叶、班尼特组成的队伍伤害。注意角色名之间必须使用空格分开。含有 **旅行者** 的配队暂时无法查询。\n   \n   为此形式的命令指定 UID 方式与上面相同。\n   \n   队伍别名支持可能不全请见谅，如果有十分流行的配队未能支持请提出 issue 耐心等待适配。\n\n\n*\\* 队伍伤害为 **实验性功能**，计算结果可能存在问题。欢迎附带详细日志提交 issue 帮助改进此功能。*\n\n\n## 特别鸣谢\n\n\n[@nonebot/nonebot2](https://github.com/nonebot/nonebot2/) | [@Mrs4s/go-cqhttp](https://github.com/Mrs4s/go-cqhttp) | [@yoimiya-kokomi/miao-plugin](https://github.com/yoimiya-kokomi/miao-plugin) | [Enka.Network](https://enka.network/) | [Miniprogram Teyvat Helper](#)\n',
     'author': 'monsterxcn',
     'author_email': 'monsterxcn@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/monsterxcn/nonebot-plugin-gspanel',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['nonebot_plugin_gspanel'] package_data = \ {'': ['*']} install_requires = \
 ['httpx>=0.20.0,<1.0.0', 'nonebot-adapter-onebot>=2.0.0b1', 'nonebot-plugin-
 htmlrender>=0.2.0.1', 'nonebot2>=2.0.0b3', 'playwright>=1.25.0'] setup_kwargs =
-{ 'name': 'nonebot-plugin-gspanel', 'version': '0.2.8', 'description': 'Genshin
+{ 'name': 'nonebot-plugin-gspanel', 'version': '0.2.9', 'description': 'Genshin
 player cards plugin for NoneBot2', 'long_description': '
                      ****** NoneBot Plugin GsPanel ******
 \n\n\n
      ð¤ ç¨äºå±ç¤ºåç¥æ¸¸æåè§è²å±ææ°æ®ç NoneBot2 æä»¶
 \n\n\n
           \n \n_[actions]\n\n \n_[license]\n\n \n_[pypi]\n\n [python]
                                       \n
@@ -16,24 +16,28 @@
 cf090da6b6c7.PNG) | ![å¦®é²](https://user-images.githubusercontent.com/
 22407052/201667744-decfdf25-c889-4a65-bbe0-94e194fe8d82.PNG) |\n|:--:|:--:|:--:
 |\n\n\n## å®è£æ¹æ³\n\n\nå¦æä½ æ­£å¨ä½¿ç¨ 2.0.0.beta1 ä»¥ä¸çæ¬
 NoneBotï¼æ¨èä½¿ç¨ä»¥ä¸å½ä»¤å®è£ï¼\n\n\n```bash\n# ä» nb_cli
 å®è£\npython3 -m nb_cli plugin install nonebot-plugin-gspanel\n\n# æä»
 PyPI å®è£\npython3 -m pip install nonebot-plugin-gspanel\n```\n\n\n> **
 [@realhuhu/py-plugin](https://github.com/realhuhu/py-plugin)
-æä»¶ç¨æ·é¡»ç¥**\n> \n> Yunzai ç¨æ·å®è£ py-plugin
-æä»¶åå¯ä»¥å¼å®¹è¿è¡æ¬æä»¶ï¼å®è£æ­¥éª¤å¦ä¸ï¼\n> \n> 1.
+æä»¶ç¨æ·å®è£æ¹æ³**\n> \n> Yunzai ç¨æ·å®è£ py-plugin
+æä»¶åå¯ä»¥å¼å®¹è¿è¡æ­¤æä»¶ï¼å®è£æ­¥éª¤å¦ä¸ï¼\n> \n> 1.
 ä»ç»éè¯» [README.md](https://github.com/realhuhu/py-plugin#21-
 %E5%AE%89%E8%A3%85) éç½® Yunzai Bot ç Python è¿è¡ç¯å¢\n> 2. å Yunzai
-Bot åé QQ æ¶æ¯ `#pyä¸è½½æä»¶nonebot-plugin-gspanel` å®è£æ¬æä»¶\n>
+Bot åé QQ æ¶æ¯ `#pyä¸è½½æä»¶nonebot-plugin-gspanel` å®è£æ­¤æä»¶\n>
 3. [å»ºè®®] å°ä¸æ¹ä½¿ç¨é¡»ç¥ç¬¬ 4 æ¡ä¸­äº¤å¾çææç¯å¢åéåå¥
 py-plugin çéç½®æä»¶ config.yaml ä¸­ï¼æ³¨ææ ¼å¼ï¼\n> 4. [å»ºè®®]
 å°ç¯å¢åé `gspanel_alias` å®ä¹ä¸º `é¢æ¿`
-ä»¥å¤çå³é®è¯ï¼é¿åæ­¤æä»¶çåè½ä¸ Yunzai
-ç¸å³åè½åæ¶è§¦å\n\n\n## ä½¿ç¨é¡»ç¥\n\n\n -
+ä»¥å¤çè§¦åè¯ï¼é¿åæ­¤æä»¶ä¸ Yunzai ç¸å³åè½åæ¶è§¦å\n> \n>
+py-plugin çéç½®æä»¶ config.yaml ä¸­ **å¡å¿æå¨æ·»å **
+æ­¤æä»¶çä¸äºéç½®ï¼\n> \n> ```yaml\n> gspanel_alias:\n> -
+æ³è¦çé¢æ¿è§¦åè¯\n> - æ¯æå¤ä¸ªè§¦åè¯\n> gspanel_scale: 1.0\n>
+resources_dir: /path/to/data # Windows è¦å°åææ æ¿æ¢ä¸º /\n>
+resources_mirror: https://enka.network/ui/\n> ```\n\n\n## ä½¿ç¨é¡»ç¥\n\n\n -
 æä»¶çå£éç©è¯åè®¡ç®è§åãå¡çæ ·å¼åæ¥èª [@yoimiya-kokomi/
 miao-plugin](https://github.com/yoimiya-kokomi/miao-
 plugin)ãæä»¶ç§»æ¤æ¶å¯¹ **è¯åè§å** ä¸»è¦åäºä»¥ä¸ä¿®æ¹ï¼\n \n
 +
 ä»¥è§è²çå½å¼ãæ»å»åãé²å¾¡åçå®éåºç¡å¼è¿è¡è¯æ¡å¾åè®¡ç®ï¼å¯¼è´åºå®å¼ççå½å¼ãæ»å»åãé²å¾¡åè¯æ¡è¯åç¸è¾åçæå°å¹åº¦æ³¢å¨\n
 +
 äºé¢æ¿æ°æ®åºåå±ç¤ºå£éç©è¯åä½¿ç¨çè¯æ¡æéè§åï¼æä»¶å°æªèªå®ä¹è¯æ¡æéè§åçè§è²ä½¿ç¨é»è®¤è§åï¼æ»å»å
```

### Comparing `nonebot_plugin_gspanel-0.2.8/PKG-INFO` & `nonebot_plugin_gspanel-0.2.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-gspanel
-Version: 0.2.8
+Version: 0.2.9
 Summary: Genshin player cards plugin for NoneBot2
 Home-page: https://github.com/monsterxcn/nonebot-plugin-gspanel
 License: MIT
 Keywords: nonebot,nonebot2,genshin,panel,card
 Author: monsterxcn
 Author-email: monsterxcn@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -57,22 +57,33 @@
 python3 -m nb_cli plugin install nonebot-plugin-gspanel
 
 # 或从 PyPI 安装
 python3 -m pip install nonebot-plugin-gspanel
 ```
 
 
-> **[@realhuhu/py-plugin](https://github.com/realhuhu/py-plugin) 插件用户须知**
+> **[@realhuhu/py-plugin](https://github.com/realhuhu/py-plugin) 插件用户安装方法**
 > 
-> Yunzai 用户安装 py-plugin 插件后可以兼容运行本插件！安装步骤如下：
+> Yunzai 用户安装 py-plugin 插件后可以兼容运行此插件！安装步骤如下：
 > 
 > 1. 仔细阅读 [README.md](https://github.com/realhuhu/py-plugin#21-%E5%AE%89%E8%A3%85) 配置 Yunzai Bot 的 Python 运行环境
-> 2. 向 Yunzai Bot 发送 QQ 消息 `#py下载插件nonebot-plugin-gspanel` 安装本插件
+> 2. 向 Yunzai Bot 发送 QQ 消息 `#py下载插件nonebot-plugin-gspanel` 安装此插件
 > 3. [建议] 将下方使用须知第 4 条中交待的所有环境变量写入 py-plugin 的配置文件 config.yaml 中（注意格式）
-> 4. [建议] 将环境变量 `gspanel_alias` 定义为 `面板` 以外的关键词，避免此插件的功能与 Yunzai 相关功能同时触发
+> 4. [建议] 将环境变量 `gspanel_alias` 定义为 `面板` 以外的触发词，避免此插件与 Yunzai 相关功能同时触发
+> 
+> py-plugin 的配置文件 config.yaml 中 **务必手动添加** 此插件的一些配置：
+> 
+> ```yaml
+> gspanel_alias:
+>   - 想要的面板触发词
+>   - 支持多个触发词
+> gspanel_scale: 1.0
+> resources_dir: /path/to/data  # Windows 要将反斜杠替换为 /
+> resources_mirror: https://enka.network/ui/
+> ```
 
 
 ## 使用须知
 
 
  - 插件的圣遗物评分计算规则、卡片样式均来自 [@yoimiya-kokomi/miao-plugin](https://github.com/yoimiya-kokomi/miao-plugin)。插件移植时对 **评分规则** 主要做了以下修改：
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-gspanel Version: 0.2.8 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-gspanel Version: 0.2.9 Summary:
 Genshin player cards plugin for NoneBot2 Home-page: https://github.com/
 monsterxcn/nonebot-plugin-gspanel License: MIT Keywords:
 nonebot,nonebot2,genshin,panel,card Author: monsterxcn Author-email:
 monsterxcn@gmail.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
@@ -20,24 +20,29 @@
 images.githubusercontent.com/22407052/201661930-f9ecdfe0-e278-4641-a012-
 cf090da6b6c7.PNG) | ![å¦®é²](https://user-images.githubusercontent.com/
 22407052/201667744-decfdf25-c889-4a65-bbe0-94e194fe8d82.PNG) | |:--:|:--:|:--:
 | ## å®è£æ¹æ³ å¦æä½ æ­£å¨ä½¿ç¨ 2.0.0.beta1 ä»¥ä¸çæ¬
 NoneBotï¼æ¨èä½¿ç¨ä»¥ä¸å½ä»¤å®è£ï¼ ```bash # ä» nb_cli å®è£ python3
 -m nb_cli plugin install nonebot-plugin-gspanel # æä» PyPI å®è£ python3 -
 m pip install nonebot-plugin-gspanel ``` > **[@realhuhu/py-plugin](https://
-github.com/realhuhu/py-plugin) æä»¶ç¨æ·é¡»ç¥** > > Yunzai ç¨æ·å®è£ py-
-plugin æä»¶åå¯ä»¥å¼å®¹è¿è¡æ¬æä»¶ï¼å®è£æ­¥éª¤å¦ä¸ï¼ > > 1.
+github.com/realhuhu/py-plugin) æä»¶ç¨æ·å®è£æ¹æ³** > > Yunzai
+ç¨æ·å®è£ py-plugin
+æä»¶åå¯ä»¥å¼å®¹è¿è¡æ­¤æä»¶ï¼å®è£æ­¥éª¤å¦ä¸ï¼ > > 1.
 ä»ç»éè¯» [README.md](https://github.com/realhuhu/py-plugin#21-
 %E5%AE%89%E8%A3%85) éç½® Yunzai Bot ç Python è¿è¡ç¯å¢ > 2. å Yunzai
-Bot åé QQ æ¶æ¯ `#pyä¸è½½æä»¶nonebot-plugin-gspanel` å®è£æ¬æä»¶ >
+Bot åé QQ æ¶æ¯ `#pyä¸è½½æä»¶nonebot-plugin-gspanel` å®è£æ­¤æä»¶ >
 3. [å»ºè®®] å°ä¸æ¹ä½¿ç¨é¡»ç¥ç¬¬ 4 æ¡ä¸­äº¤å¾çææç¯å¢åéåå¥
 py-plugin çéç½®æä»¶ config.yaml ä¸­ï¼æ³¨ææ ¼å¼ï¼ > 4. [å»ºè®®]
 å°ç¯å¢åé `gspanel_alias` å®ä¹ä¸º `é¢æ¿`
-ä»¥å¤çå³é®è¯ï¼é¿åæ­¤æä»¶çåè½ä¸ Yunzai
-ç¸å³åè½åæ¶è§¦å ## ä½¿ç¨é¡»ç¥ -
+ä»¥å¤çè§¦åè¯ï¼é¿åæ­¤æä»¶ä¸ Yunzai ç¸å³åè½åæ¶è§¦å > > py-
+plugin çéç½®æä»¶ config.yaml ä¸­ **å¡å¿æå¨æ·»å **
+æ­¤æä»¶çä¸äºéç½®ï¼ > > ```yaml > gspanel_alias: > -
+æ³è¦çé¢æ¿è§¦åè¯ > - æ¯æå¤ä¸ªè§¦åè¯ > gspanel_scale: 1.0 >
+resources_dir: /path/to/data # Windows è¦å°åææ æ¿æ¢ä¸º / >
+resources_mirror: https://enka.network/ui/ > ``` ## ä½¿ç¨é¡»ç¥ -
 æä»¶çå£éç©è¯åè®¡ç®è§åãå¡çæ ·å¼åæ¥èª [@yoimiya-kokomi/
 miao-plugin](https://github.com/yoimiya-kokomi/miao-
 plugin)ãæä»¶ç§»æ¤æ¶å¯¹ **è¯åè§å** ä¸»è¦åäºä»¥ä¸ä¿®æ¹ï¼ +
 ä»¥è§è²çå½å¼ãæ»å»åãé²å¾¡åçå®éåºç¡å¼è¿è¡è¯æ¡å¾åè®¡ç®ï¼å¯¼è´åºå®å¼ççå½å¼ãæ»å»åãé²å¾¡åè¯æ¡è¯åç¸è¾åçæå°å¹åº¦æ³¢å¨
 +
 äºé¢æ¿æ°æ®åºåå±ç¤ºå£éç©è¯åä½¿ç¨çè¯æ¡æéè§åï¼æä»¶å°æªèªå®ä¹è¯æ¡æéè§åçè§è²ä½¿ç¨é»è®¤è§åï¼æ»å»å
 `75`ãæ´å»ç `100`ãæ´å»ä¼¤å®³ `100`ï¼ +
```

