# Comparing `tmp/nonebot2-2.2.1.tar.gz` & `tmp/nonebot2-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot2-2.2.1.tar", max compression
+gzip compressed data, was "nonebot2-2.3.0.tar", max compression
```

## Comparing `nonebot2-2.2.1.tar` & `nonebot2-2.3.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     1078 2024-02-24 04:38:34.801971 nonebot2-2.2.1/LICENSE
--rw-r--r--   0        0        0    20392 2024-02-24 04:38:34.801971 nonebot2-2.2.1/README.md
--rw-r--r--   0        0        0    12555 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/__init__.py
--rw-r--r--   0        0        0      913 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/adapters/__init__.py
--rw-r--r--   0        0        0    12814 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/compat.py
--rw-r--r--   0        0        0    16332 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/config.py
--rw-r--r--   0        0        0     1863 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/consts.py
--rw-r--r--   0        0        0     6346 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/dependencies/__init__.py
--rw-r--r--   0        0        0     1699 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/dependencies/utils.py
--rw-r--r--   0        0        0     1770 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/drivers/__init__.py
--rw-r--r--   0        0        0     5533 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/drivers/aiohttp.py
--rw-r--r--   0        0        0     9785 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/drivers/fastapi.py
--rw-r--r--   0        0        0     1874 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/drivers/httpx.py
--rw-r--r--   0        0        0     4068 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/drivers/none.py
--rw-r--r--   0        0        0     8550 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/drivers/quart.py
--rw-r--r--   0        0        0     3715 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/drivers/websockets.py
--rw-r--r--   0        0        0     6462 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/exception.py
--rw-r--r--   0        0        0        0 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/internal/__init__.py
--rw-r--r--   0        0        0      253 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/internal/adapter/__init__.py
--rw-r--r--   0        0        0     3947 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/internal/adapter/adapter.py
--rw-r--r--   0        0        0     5166 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/internal/adapter/bot.py
--rw-r--r--   0        0        0     2916 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/internal/adapter/event.py
--rw-r--r--   0        0        0    12502 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/internal/adapter/message.py
--rw-r--r--   0        0        0     7361 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/internal/adapter/template.py
--rw-r--r--   0        0        0     1389 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/internal/driver/__init__.py
--rw-r--r--   0        0        0     1778 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/internal/driver/_lifespan.py
--rw-r--r--   0        0        0     9242 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/internal/driver/abstract.py
--rw-r--r--   0        0        0     1143 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/internal/driver/combine.py
--rw-r--r--   0        0        0    11228 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/internal/driver/model.py
--rw-r--r--   0        0        0      516 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/internal/matcher/__init__.py
--rw-r--r--   0        0        0     2738 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/internal/matcher/manager.py
--rw-r--r--   0        0        0    29037 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/internal/matcher/matcher.py
--rw-r--r--   0        0        0      731 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/internal/matcher/provider.py
--rw-r--r--   0        0        0    17018 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/internal/params.py
--rw-r--r--   0        0        0     5671 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/internal/permission.py
--rw-r--r--   0        0        0     3178 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/internal/rule.py
--rw-r--r--   0        0        0     2501 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/log.py
--rw-r--r--   0        0        0     1057 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/matcher.py
--rw-r--r--   0        0        0    15446 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/message.py
--rw-r--r--   0        0        0     6537 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/params.py
--rw-r--r--   0        0        0     3063 2024-02-24 04:38:34.805971 nonebot2-2.2.1/nonebot/permission.py
--rw-r--r--   0        0        0     5972 2024-02-24 04:38:34.809971 nonebot2-2.2.1/nonebot/plugin/__init__.py
--rw-r--r--   0        0        0     6934 2024-02-24 04:38:34.809971 nonebot2-2.2.1/nonebot/plugin/load.py
--rw-r--r--   0        0        0     8763 2024-02-24 04:38:34.809971 nonebot2-2.2.1/nonebot/plugin/manager.py
--rw-r--r--   0        0        0     2448 2024-02-24 04:38:34.809971 nonebot2-2.2.1/nonebot/plugin/model.py
--rw-r--r--   0        0        0    30975 2024-02-24 04:38:34.809971 nonebot2-2.2.1/nonebot/plugin/on.py
--rw-r--r--   0        0        0    14583 2024-02-24 04:38:34.809971 nonebot2-2.2.1/nonebot/plugin/on.pyi
--rw-r--r--   0        0        0      669 2024-02-24 04:38:34.809971 nonebot2-2.2.1/nonebot/plugins/echo.py
--rw-r--r--   0        0        0     1259 2024-02-24 04:38:34.809971 nonebot2-2.2.1/nonebot/plugins/single_session.py
--rw-r--r--   0        0        0        0 2024-02-24 04:38:34.809971 nonebot2-2.2.1/nonebot/py.typed
--rw-r--r--   0        0        0    23003 2024-02-24 04:38:34.809971 nonebot2-2.2.1/nonebot/rule.py
--rw-r--r--   0        0        0     6889 2024-02-24 04:38:34.809971 nonebot2-2.2.1/nonebot/typing.py
--rw-r--r--   0        0        0     9526 2024-02-24 04:38:34.809971 nonebot2-2.2.1/nonebot/utils.py
--rw-r--r--   0        0        0     3166 2024-02-24 04:38:34.809971 nonebot2-2.2.1/pyproject.toml
--rw-r--r--   0        0        0    22511 1970-01-01 00:00:00.000000 nonebot2-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-05-01 09:02:00.544923 nonebot2-2.3.0/LICENSE
+-rw-r--r--   0        0        0    20697 2024-05-01 09:02:00.544923 nonebot2-2.3.0/README.md
+-rw-r--r--   0        0        0    12601 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/__init__.py
+-rw-r--r--   0        0        0      913 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/adapters/__init__.py
+-rw-r--r--   0        0        0    12802 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/compat.py
+-rw-r--r--   0        0        0    16345 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/config.py
+-rw-r--r--   0        0        0     1863 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/consts.py
+-rw-r--r--   0        0        0     6295 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/dependencies/__init__.py
+-rw-r--r--   0        0        0     1693 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/dependencies/utils.py
+-rw-r--r--   0        0        0     1845 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/drivers/__init__.py
+-rw-r--r--   0        0        0     8202 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/drivers/aiohttp.py
+-rw-r--r--   0        0        0     9770 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/drivers/fastapi.py
+-rw-r--r--   0        0        0     4186 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/drivers/httpx.py
+-rw-r--r--   0        0        0     4113 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/drivers/none.py
+-rw-r--r--   0        0        0     8535 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/drivers/quart.py
+-rw-r--r--   0        0        0     3773 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/drivers/websockets.py
+-rw-r--r--   0        0        0     6462 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/exception.py
+-rw-r--r--   0        0        0        0 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/__init__.py
+-rw-r--r--   0        0        0      253 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/adapter/__init__.py
+-rw-r--r--   0        0        0     3968 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/adapter/adapter.py
+-rw-r--r--   0        0        0     5191 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/adapter/bot.py
+-rw-r--r--   0        0        0     2926 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/adapter/event.py
+-rw-r--r--   0        0        0    12912 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/adapter/message.py
+-rw-r--r--   0        0        0     7495 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/adapter/template.py
+-rw-r--r--   0        0        0     1450 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/driver/__init__.py
+-rw-r--r--   0        0        0     1799 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/driver/_lifespan.py
+-rw-r--r--   0        0        0    10962 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/driver/abstract.py
+-rw-r--r--   0        0        0     1160 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/driver/combine.py
+-rw-r--r--   0        0        0    11376 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/driver/model.py
+-rw-r--r--   0        0        0      516 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/matcher/__init__.py
+-rw-r--r--   0        0        0     2823 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/matcher/manager.py
+-rw-r--r--   0        0        0    29452 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/matcher/matcher.py
+-rw-r--r--   0        0        0      746 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/matcher/provider.py
+-rw-r--r--   0        0        0    17537 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/params.py
+-rw-r--r--   0        0        0     5707 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/permission.py
+-rw-r--r--   0        0        0     3219 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/rule.py
+-rw-r--r--   0        0        0     2636 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/log.py
+-rw-r--r--   0        0        0     1057 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/matcher.py
+-rw-r--r--   0        0        0    15429 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/message.py
+-rw-r--r--   0        0        0     6487 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/params.py
+-rw-r--r--   0        0        0     3063 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/permission.py
+-rw-r--r--   0        0        0     7673 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/plugin/__init__.py
+-rw-r--r--   0        0        0     6905 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/plugin/load.py
+-rw-r--r--   0        0        0     9076 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/plugin/manager.py
+-rw-r--r--   0        0        0     2669 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/plugin/model.py
+-rw-r--r--   0        0        0    30978 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/plugin/on.py
+-rw-r--r--   0        0        0    14583 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/plugin/on.pyi
+-rw-r--r--   0        0        0      669 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/plugins/echo.py
+-rw-r--r--   0        0        0     1262 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/plugins/single_session.py
+-rw-r--r--   0        0        0        0 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/py.typed
+-rw-r--r--   0        0        0    23027 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/rule.py
+-rw-r--r--   0        0        0     6964 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/typing.py
+-rw-r--r--   0        0        0     9444 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/utils.py
+-rw-r--r--   0        0        0     3663 2024-05-01 09:02:00.552923 nonebot2-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0    22766 1970-01-01 00:00:00.000000 nonebot2-2.3.0/PKG-INFO
```

### Comparing `nonebot2-2.2.1/LICENSE` & `nonebot2-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot2-2.2.1/README.md` & `nonebot2-2.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 <p align="center">
   <a href="https://raw.githubusercontent.com/nonebot/nonebot2/master/LICENSE">
     <img src="https://img.shields.io/github/license/nonebot/nonebot2" alt="license">
   </a>
   <a href="https://pypi.python.org/pypi/nonebot2">
     <img src="https://img.shields.io/pypi/v/nonebot2?logo=python&logoColor=edb641" alt="pypi">
   </a>
-  <img src="https://img.shields.io/badge/python-3.8+-blue?logo=python&logoColor=edb641" alt="python">
+  <img src="https://img.shields.io/badge/python-3.9+-blue?logo=python&logoColor=edb641" alt="python">
   <a href="https://github.com/psf/black">
     <img src="https://img.shields.io/badge/code%20style-black-000000.svg?logo=python&logoColor=edb641" alt="black">
   </a>
   <a href="https://github.com/Microsoft/pyright">
     <img src="https://img.shields.io/badge/types-pyright-797952.svg?logo=python&logoColor=edb641" alt="pyright">
   </a>
   <a href="https://github.com/astral-sh/ruff">
@@ -106,34 +106,36 @@
 
 - 异步优先：基于 Python 的异步特性，即使是~~非常~~大量的消息，也能吞吐自如
 - 易于开发：配合 NB-CLI 脚手架，代码编写上手简单，没有过多的冗余代码，可以让开发者专注于业务逻辑
 - 生而可靠：100% 类型注解覆盖，配合编辑器的类型推导功能，能将绝大多数的 Bug 杜绝在编辑器中 ([编辑器支持](https://nonebot.dev/docs/editor-support))
 - 社区丰富：社区用户众多，直接和间接用户超过十万人，每天都有大量的活跃用户 ([社区资源](#社区资源))
 - 海纳百川：一个框架，支持多个聊天软件平台，可自定义通信协议
 
-  |                                                           协议名称                                                           | 状态 |                                   注释                                    |
-  | :--------------------------------------------------------------------------------------------------------------------------: | :--: | :-----------------------------------------------------------------------: |
-  |                   OneBot（[仓库](https://github.com/nonebot/adapter-onebot)，[协议](https://onebot.dev/)）                   |  ✅  | 支持 QQ、TG、微信公众号、KOOK 等[平台](https://onebot.dev/ecosystem.html) |
-  |         Telegram（[仓库](https://github.com/nonebot/adapter-telegram)，[协议](https://core.telegram.org/bots/api)）          |  ✅  |                                                                           |
-  |        飞书（[仓库](https://github.com/nonebot/adapter-feishu)，[协议](https://open.feishu.cn/document/home/index)）         |  ✅  |                                                                           |
-  |             GitHub（[仓库](https://github.com/nonebot/adapter-github)，[协议](https://docs.github.com/en/apps)）             |  ✅  |                          GitHub APP & OAuth APP                           |
-  |                   QQ（[仓库](https://github.com/nonebot/adapter-qq)，[协议](https://bot.q.qq.com/wiki/)）                    |  ✅  |                            QQ 官方接口调整较多                            |
-  |             钉钉（[仓库](https://github.com/nonebot/adapter-ding)，[协议](https://open.dingtalk.com/document/)）             |  🤗  |                        寻找 Maintainer（暂不可用）                        |
-  |                                Console（[仓库](https://github.com/nonebot/adapter-console)）                                 |  ✅  |                                控制台交互                                 |
-  |        Red （[仓库](https://github.com/nonebot/adapter-red)，[协议](https://chrononeko.github.io/QQNTRedProtocol/)）         |  ✅  |                                  QQ 协议                                  |
-  |               Satori（[仓库](https://github.com/nonebot/adapter-satori)，[协议](https://satori.js.org/zh-CN)）               |  ✅  |               支持 Onebot、TG、飞书、微信公众号、Koishi 等                |
-  |      Discord （[仓库](https://github.com/nonebot/adapter-discord)，[协议](https://discord.com/developers/docs/intro)）       |  ✅  |                             Discord Bot 协议                              |
-  |                  DoDo （[仓库](https://github.com/nonebot/adapter-dodo)，[协议](https://open.imdodo.com/)）                  |  ✅  |                               DoDo Bot 协议                               |
-  |        开黑啦（[仓库](https://github.com/Tian-que/nonebot-adapter-kaiheila)，[协议](https://developer.kookapp.cn/)）         |  ↗️  |                                由社区贡献                                 |
-  |    Mirai（[仓库](https://github.com/ieew/nonebot_adapter_mirai2)，[协议](https://docs.mirai.mamoe.net/mirai-api-http/)）     |  ↗️  |                            QQ 协议，由社区贡献                            |
-  |                              Ntchat（[仓库](https://github.com/JustUndertaker/adapter-ntchat)）                              |  ↗️  |                           微信协议，由社区贡献                            |
-  |                         MineCraft（[仓库](https://github.com/17TheWord/nonebot-adapter-minecraft)）                          |  ↗️  |                                由社区贡献                                 |
-  |                             BiliBili Live（[仓库](https://github.com/wwweww/adapter-bilibili)）                              |  ↗️  |                                由社区贡献                                 |
-  |                          Walle-Q（[仓库](https://github.com/onebot-walle/nonebot_adapter_walleq)）                           |  ↗️  |                            QQ 协议，由社区贡献                            |
-  | Villa（[仓库](https://github.com/CMHopeSunshine/nonebot-adapter-villa)，[协议](https://webstatic.mihoyo.com/vila/bot/doc/)） |  ↗️  |                     米游社大别野 Bot 协议，由社区贡献                     |
+  |                                                       协议名称                                                        | 状态 |                                   注释                                    |
+  | :-------------------------------------------------------------------------------------------------------------------: | :--: | :-----------------------------------------------------------------------: |
+  |               OneBot（[仓库](https://github.com/nonebot/adapter-onebot)，[协议](https://onebot.dev/)）                |  ✅  | 支持 QQ、TG、微信公众号、KOOK 等[平台](https://onebot.dev/ecosystem.html) |
+  |      Telegram（[仓库](https://github.com/nonebot/adapter-telegram)，[协议](https://core.telegram.org/bots/api)）      |  ✅  |                                                                           |
+  |     飞书（[仓库](https://github.com/nonebot/adapter-feishu)，[协议](https://open.feishu.cn/document/home/index)）     |  ✅  |                                                                           |
+  |         GitHub（[仓库](https://github.com/nonebot/adapter-github)，[协议](https://docs.github.com/en/apps)）          |  ✅  |                          GitHub APP & OAuth APP                           |
+  |                QQ（[仓库](https://github.com/nonebot/adapter-qq)，[协议](https://bot.q.qq.com/wiki/)）                |  ✅  |                            QQ 官方接口调整较多                            |
+  |                             Console（[仓库](https://github.com/nonebot/adapter-console)）                             |  ✅  |                                控制台交互                                 |
+  |     Red（[仓库](https://github.com/nonebot/adapter-red)，[协议](https://chrononeko.github.io/QQNTRedProtocol/)）      |  ✅  |                                  QQ 协议                                  |
+  |           Satori（[仓库](https://github.com/nonebot/adapter-satori)，[协议](https://satori.js.org/zh-CN)）            |  ✅  |               支持 Onebot、TG、飞书、微信公众号、Koishi 等                |
+  |   Discord（[仓库](https://github.com/nonebot/adapter-discord)，[协议](https://discord.com/developers/docs/intro)）    |  ✅  |                             Discord Bot 协议                              |
+  |               DoDo（[仓库](https://github.com/nonebot/adapter-dodo)，[协议](https://open.imdodo.com/)）               |  ✅  |                               DoDo Bot 协议                               |
+  |        Kritor（[仓库](https://github.com/nonebot/adapter-kritor)，[协议](https://github.com/KarinJS/kritor)）         |  ✅  |                 Kritor (OnebotX) 协议，QQ 机器人接口标准                  |
+  |         钉钉（[仓库](https://github.com/nonebot/adapter-ding)，[协议](https://open.dingtalk.com/document/)）          |  🤗  |                        寻找 Maintainer（暂不可用）                        |
+  |     开黑啦（[仓库](https://github.com/Tian-que/nonebot-adapter-kaiheila)，[协议](https://developer.kookapp.cn/)）     |  ↗️  |                                由社区贡献                                 |
+  | Mirai（[仓库](https://github.com/ieew/nonebot_adapter_mirai2)，[协议](https://docs.mirai.mamoe.net/mirai-api-http/)） |  ↗️  |                            QQ 协议，由社区贡献                            |
+  |                          Ntchat（[仓库](https://github.com/JustUndertaker/adapter-ntchat)）                           |  ↗️  |                           微信协议，由社区贡献                            |
+  |                      MineCraft（[仓库](https://github.com/17TheWord/nonebot-adapter-minecraft)）                      |  ↗️  |                                由社区贡献                                 |
+  |                          BiliBili Live（[仓库](https://github.com/wwweww/adapter-bilibili)）                          |  ↗️  |                                由社区贡献                                 |
+  |                       Walle-Q（[仓库](https://github.com/onebot-walle/nonebot_adapter_walleq)）                       |  ↗️  |                            QQ 协议，由社区贡献                            |
+  |                       Villa（[仓库](https://github.com/CMHopeSunshine/nonebot-adapter-villa)）                        |  ❌  |                     米游社大别野 Bot 协议，官方已下线                     |
+  | Rocket.Chat（[仓库](https://github.com/IUnlimit/nonebot-adapter-rocketchat)，[协议](https://developer.rocket.chat/)） |  ↗️  |                     Rocket.Chat Bot 协议，由社区贡献                      |
 
 - 坚实后盾：支持多种 web 框架，可自定义替换、组合
 
   |                              驱动框架                               |  类型  |
   | :-----------------------------------------------------------------: | :----: |
   |              [FastAPI](https://fastapi.tiangolo.com/)               | 服务端 |
   | [Quart](https://quart.palletsprojects.com/en/latest/)（异步 Flask） | 服务端 |
```

#### html2text {}

```diff
@@ -18,51 +18,55 @@
 ç±»åæ³¨è§£è¦çï¼éåç¼è¾å¨çç±»åæ¨å¯¼åè½ï¼è½å°ç»å¤§å¤æ°ç
 Bug æç»å¨ç¼è¾å¨ä¸­ ([ç¼è¾å¨æ¯æ](https://nonebot.dev/docs/editor-
 support)) -
 ç¤¾åºä¸°å¯ï¼ç¤¾åºç¨æ·ä¼å¤ï¼ç´æ¥åé´æ¥ç¨æ·è¶è¿åä¸äººï¼æ¯å¤©é½æå¤§éçæ´»è·ç¨æ·
 ([ç¤¾åºèµæº](#ç¤¾åºèµæº)) -
 æµ·çº³ç¾å·ï¼ä¸ä¸ªæ¡æ¶ï¼æ¯æå¤ä¸ªèå¤©è½¯ä»¶å¹³å°ï¼å¯èªå®ä¹éä¿¡åè®®
 | åè®®åç§° | ç¶æ | æ³¨é | | :-----------------------------------------
--------------------------------------------------------------------------------
---: | :--: | :-----------------------------------------------------------------
-------: | | OneBotï¼[ä»åº](https://github.com/nonebot/adapter-onebot)ï¼
-[åè®®](https://onebot.dev/)ï¼ | â | æ¯æ
-QQãTGãå¾®ä¿¡å¬ä¼å·ãKOOK ç­[å¹³å°](https://onebot.dev/ecosystem.html)
-| | Telegramï¼[ä»åº](https://github.com/nonebot/adapter-telegram)ï¼[åè®®]
-(https://core.telegram.org/bots/api)ï¼ | â | | | é£ä¹¦ï¼[ä»åº](https://
-github.com/nonebot/adapter-feishu)ï¼[åè®®](https://open.feishu.cn/document/
-home/index)ï¼ | â | | | GitHubï¼[ä»åº](https://github.com/nonebot/
-adapter-github)ï¼[åè®®](https://docs.github.com/en/apps)ï¼ | â | GitHub
-APP & OAuth APP | | QQï¼[ä»åº](https://github.com/nonebot/adapter-qq)ï¼
-[åè®®](https://bot.q.qq.com/wiki/)ï¼ | â | QQ å®æ¹æ¥å£è°æ´è¾å¤ | |
-ééï¼[ä»åº](https://github.com/nonebot/adapter-ding)ï¼[åè®®](https://
-open.dingtalk.com/document/)ï¼ | ð¤ | å¯»æ¾ Maintainerï¼æä¸å¯ç¨ï¼ |
-| Consoleï¼[ä»åº](https://github.com/nonebot/adapter-console)ï¼ | â |
-æ§å¶å°äº¤äº | | Red ï¼[ä»åº](https://github.com/nonebot/adapter-red)ï¼
-[åè®®](https://chrononeko.github.io/QQNTRedProtocol/)ï¼ | â | QQ åè®® |
-| Satoriï¼[ä»åº](https://github.com/nonebot/adapter-satori)ï¼[åè®®]
-(https://satori.js.org/zh-CN)ï¼ | â | æ¯æ
-OnebotãTGãé£ä¹¦ãå¾®ä¿¡å¬ä¼å·ãKoishi ç­ | | Discord ï¼[ä»åº]
+--------------------------------------------------------------------------: | :
+--: | :-----------------------------------------------------------------------:
+| | OneBotï¼[ä»åº](https://github.com/nonebot/adapter-onebot)ï¼[åè®®]
+(https://onebot.dev/)ï¼ | â | æ¯æ QQãTGãå¾®ä¿¡å¬ä¼å·ãKOOK ç­
+[å¹³å°](https://onebot.dev/ecosystem.html) | | Telegramï¼[ä»åº](https://
+github.com/nonebot/adapter-telegram)ï¼[åè®®](https://core.telegram.org/bots/
+api)ï¼ | â | | | é£ä¹¦ï¼[ä»åº](https://github.com/nonebot/adapter-
+feishu)ï¼[åè®®](https://open.feishu.cn/document/home/index)ï¼ | â | | |
+GitHubï¼[ä»åº](https://github.com/nonebot/adapter-github)ï¼[åè®®](https:/
+/docs.github.com/en/apps)ï¼ | â | GitHub APP & OAuth APP | | QQï¼[ä»åº]
+(https://github.com/nonebot/adapter-qq)ï¼[åè®®](https://bot.q.qq.com/wiki/
+)ï¼ | â | QQ å®æ¹æ¥å£è°æ´è¾å¤ | | Consoleï¼[ä»åº](https://
+github.com/nonebot/adapter-console)ï¼ | â | æ§å¶å°äº¤äº | | Redï¼
+[ä»åº](https://github.com/nonebot/adapter-red)ï¼[åè®®](https://
+chrononeko.github.io/QQNTRedProtocol/)ï¼ | â | QQ åè®® | | Satoriï¼
+[ä»åº](https://github.com/nonebot/adapter-satori)ï¼[åè®®](https://
+satori.js.org/zh-CN)ï¼ | â | æ¯æ
+OnebotãTGãé£ä¹¦ãå¾®ä¿¡å¬ä¼å·ãKoishi ç­ | | Discordï¼[ä»åº]
 (https://github.com/nonebot/adapter-discord)ï¼[åè®®](https://discord.com/
-developers/docs/intro)ï¼ | â | Discord Bot åè®® | | DoDo ï¼[ä»åº]
-(https://github.com/nonebot/adapter-dodo)ï¼[åè®®](https://open.imdodo.com/
-)ï¼ | â | DoDo Bot åè®® | | å¼é»å¦ï¼[ä»åº](https://github.com/Tian-
-que/nonebot-adapter-kaiheila)ï¼[åè®®](https://developer.kookapp.cn/)ï¼ |
-âï¸ | ç±ç¤¾åºè´¡ç® | | Miraiï¼[ä»åº](https://github.com/ieew/
-nonebot_adapter_mirai2)ï¼[åè®®](https://docs.mirai.mamoe.net/mirai-api-http/
-)ï¼ | âï¸ | QQ åè®®ï¼ç±ç¤¾åºè´¡ç® | | Ntchatï¼[ä»åº](https://
-github.com/JustUndertaker/adapter-ntchat)ï¼ | âï¸ |
-å¾®ä¿¡åè®®ï¼ç±ç¤¾åºè´¡ç® | | MineCraftï¼[ä»åº](https://github.com/
-17TheWord/nonebot-adapter-minecraft)ï¼ | âï¸ | ç±ç¤¾åºè´¡ç® | | BiliBili
-Liveï¼[ä»åº](https://github.com/wwweww/adapter-bilibili)ï¼ | âï¸ |
-ç±ç¤¾åºè´¡ç® | | Walle-Qï¼[ä»åº](https://github.com/onebot-walle/
-nonebot_adapter_walleq)ï¼ | âï¸ | QQ åè®®ï¼ç±ç¤¾åºè´¡ç® | | Villaï¼
-[ä»åº](https://github.com/CMHopeSunshine/nonebot-adapter-villa)ï¼[åè®®]
-(https://webstatic.mihoyo.com/vila/bot/doc/)ï¼ | âï¸ | ç±³æ¸¸ç¤¾å¤§å«é
-Bot åè®®ï¼ç±ç¤¾åºè´¡ç® | - åå®åç¾ï¼æ¯æå¤ç§ web
+developers/docs/intro)ï¼ | â | Discord Bot åè®® | | DoDoï¼[ä»åº](https:
+//github.com/nonebot/adapter-dodo)ï¼[åè®®](https://open.imdodo.com/)ï¼ |
+â | DoDo Bot åè®® | | Kritorï¼[ä»åº](https://github.com/nonebot/adapter-
+kritor)ï¼[åè®®](https://github.com/KarinJS/kritor)ï¼ | â | Kritor
+(OnebotX) åè®®ï¼QQ æºå¨äººæ¥å£æ å | | ééï¼[ä»åº](https://
+github.com/nonebot/adapter-ding)ï¼[åè®®](https://open.dingtalk.com/document/
+)ï¼ | ð¤ | å¯»æ¾ Maintainerï¼æä¸å¯ç¨ï¼ | | å¼é»å¦ï¼[ä»åº]
+(https://github.com/Tian-que/nonebot-adapter-kaiheila)ï¼[åè®®](https://
+developer.kookapp.cn/)ï¼ | âï¸ | ç±ç¤¾åºè´¡ç® | | Miraiï¼[ä»åº]
+(https://github.com/ieew/nonebot_adapter_mirai2)ï¼[åè®®](https://
+docs.mirai.mamoe.net/mirai-api-http/)ï¼ | âï¸ | QQ åè®®ï¼ç±ç¤¾åºè´¡ç®
+| | Ntchatï¼[ä»åº](https://github.com/JustUndertaker/adapter-ntchat)ï¼ |
+âï¸ | å¾®ä¿¡åè®®ï¼ç±ç¤¾åºè´¡ç® | | MineCraftï¼[ä»åº](https://
+github.com/17TheWord/nonebot-adapter-minecraft)ï¼ | âï¸ | ç±ç¤¾åºè´¡ç® |
+| BiliBili Liveï¼[ä»åº](https://github.com/wwweww/adapter-bilibili)ï¼ |
+âï¸ | ç±ç¤¾åºè´¡ç® | | Walle-Qï¼[ä»åº](https://github.com/onebot-
+walle/nonebot_adapter_walleq)ï¼ | âï¸ | QQ åè®®ï¼ç±ç¤¾åºè´¡ç® | |
+Villaï¼[ä»åº](https://github.com/CMHopeSunshine/nonebot-adapter-villa)ï¼ |
+â | ç±³æ¸¸ç¤¾å¤§å«é Bot åè®®ï¼å®æ¹å·²ä¸çº¿ | | Rocket.Chatï¼
+[ä»åº](https://github.com/IUnlimit/nonebot-adapter-rocketchat)ï¼[åè®®]
+(https://developer.rocket.chat/)ï¼ | âï¸ | Rocket.Chat Bot
+åè®®ï¼ç±ç¤¾åºè´¡ç® | - åå®åç¾ï¼æ¯æå¤ç§ web
 æ¡æ¶ï¼å¯èªå®ä¹æ¿æ¢ãç»å | é©±å¨æ¡æ¶ | ç±»å | | :-------------
 ----------------------------------------------------: | :----: | | [FastAPI]
 (https://fastapi.tiangolo.com/) | æå¡ç«¯ | | [Quart](https://
 quart.palletsprojects.com/en/latest/)ï¼å¼æ­¥ Flaskï¼ | æå¡ç«¯ | |
 [aiohttp](https://docs.aiohttp.org/en/stable/) | å®¢æ·ç«¯ | | [httpx](https://
 www.python-httpx.org/) | å®¢æ·ç«¯ | | [websockets](https://
 websockets.readthedocs.io/en/stable/) | å®¢æ·ç«¯ | æ´å¤ï¼[æ¦è§](https://
```

### Comparing `nonebot2-2.2.1/nonebot/__init__.py` & `nonebot2-2.3.0/nonebot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 FrontMatter:
     sidebar_position: 0
     description: nonebot 模块
 """
 
 import os
 from importlib.metadata import version
-from typing import Any, Dict, Type, Union, TypeVar, Optional, overload
+from typing import Any, Union, TypeVar, Optional, overload
 
 import loguru
 
 from nonebot.compat import model_dump
 from nonebot.log import logger as logger
 from nonebot.adapters import Bot, Adapter
 from nonebot.config import DOTENV_TYPE, Env, Config
@@ -96,25 +96,25 @@
 
     返回:
         指定名称的 {ref}`nonebot.adapters.Adapter` 对象
     """
 
 
 @overload
-def get_adapter(name: Type[A]) -> A:
+def get_adapter(name: type[A]) -> A:
     """
     参数:
         name: 适配器类型
 
     返回:
         指定类型的 {ref}`nonebot.adapters.Adapter` 对象
     """
 
 
-def get_adapter(name: Union[str, Type[Adapter]]) -> Adapter:
+def get_adapter(name: Union[str, type[Adapter]]) -> Adapter:
     """获取已注册的 {ref}`nonebot.adapters.Adapter` 实例。
 
     异常:
         ValueError: 指定的 {ref}`nonebot.adapters.Adapter` 未注册
         ValueError: 全局 {ref}`nonebot.drivers.Driver` 对象尚未初始化
             ({ref}`nonebot.init <nonebot.init>` 尚未调用)
 
@@ -127,15 +127,15 @@
     adapters = get_adapters()
     target = name if isinstance(name, str) else name.get_name()
     if target not in adapters:
         raise ValueError(f"Adapter {target} not registered.")
     return adapters[target]
 
 
-def get_adapters() -> Dict[str, Adapter]:
+def get_adapters() -> dict[str, Adapter]:
     """获取所有已注册的 {ref}`nonebot.adapters.Adapter` 实例。
 
     返回:
         所有 {ref}`nonebot.adapters.Adapter` 实例字典
 
     异常:
         ValueError: 全局 {ref}`nonebot.drivers.Driver` 对象尚未初始化
@@ -226,15 +226,15 @@
 
     for bot in bots.values():
         return bot
 
     raise ValueError("There are no bots to get.")
 
 
-def get_bots() -> Dict[str, Bot]:
+def get_bots() -> dict[str, Bot]:
     """获取所有连接到 NoneBot 的 {ref}`nonebot.adapters.Bot` 对象。
 
     返回:
         一个以 {ref}`nonebot.adapters.Bot.self_id` 为键
         {ref}`nonebot.adapters.Bot` 对象为值的字典
 
     异常:
@@ -245,15 +245,15 @@
         ```python
         bots = nonebot.get_bots()
         ```
     """
     return get_driver().bots
 
 
-def _resolve_combine_expr(obj_str: str) -> Type[Driver]:
+def _resolve_combine_expr(obj_str: str) -> type[Driver]:
     drivers = obj_str.split("+")
     DriverClass = resolve_dot_notation(
         drivers[0], "Driver", default_prefix="nonebot.drivers."
     )
     if len(drivers) == 1:
         logger.trace(f"Detected driver {DriverClass} with no mixins.")
         return DriverClass
@@ -262,19 +262,20 @@
         for mixin in drivers[1:]
     ]
     logger.trace(f"Detected driver {DriverClass} with mixins {mixins}.")
     return combine_driver(DriverClass, *mixins)
 
 
 def _log_patcher(record: "loguru.Record"):
+    """使用插件标识优化日志展示"""
     record["name"] = (
-        plugin.name
+        plugin.id_
         if (module_name := record["name"])
         and (plugin := get_plugin_by_module_name(module_name))
-        else (module_name and module_name.split(".")[0])
+        else (module_name and module_name.split(".", maxsplit=1)[0])
     )
 
 
 def init(*, _env_file: Optional[DOTENV_TYPE] = None, **kwargs: Any) -> None:
     """初始化 NoneBot 以及 全局 {ref}`nonebot.drivers.Driver` 对象。
 
     NoneBot 将会从 .env 文件中读取环境信息，并使用相应的 env 文件配置。
```

### Comparing `nonebot2-2.2.1/nonebot/adapters/__init__.py` & `nonebot2-2.3.0/nonebot/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.2.1/nonebot/compat.py` & `nonebot2-2.3.0/nonebot/compat.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,29 +3,26 @@
 为兼容 Pydantic V1 与 V2 版本，定义了一系列兼容函数与类供使用。
 
 FrontMatter:
     sidebar_position: 16
     description: nonebot.compat 模块
 """
 
+from collections.abc import Generator
 from dataclasses import dataclass, is_dataclass
-from typing_extensions import Self, Annotated, get_args, get_origin, is_typeddict
+from typing_extensions import Self, get_args, get_origin, is_typeddict
 from typing import (
     TYPE_CHECKING,
     Any,
-    Set,
-    Dict,
-    List,
-    Type,
     Union,
     TypeVar,
     Callable,
     Optional,
     Protocol,
-    Generator,
+    Annotated,
 )
 
 from pydantic import VERSION, BaseModel
 
 from nonebot.typing import origin_is_annotated
 
 T = TypeVar("T")
@@ -90,15 +87,15 @@
         """FieldInfo class with extra property for compatibility with pydantic v1"""
 
         # make default can be positional argument
         def __init__(self, default: Any = PydanticUndefined, **kwargs: Any) -> None:
             super().__init__(default=default, **kwargs)
 
         @property
-        def extra(self) -> Dict[str, Any]:
+        def extra(self) -> dict[str, Any]:
             """Extra data that is not part of the standard pydantic fields.
 
             For compatibility with pydantic v1.
             """
             # extract extra data from attributes set except used slots
             # we need to call super in advance due to
             # comprehension not inlined in cpython < 3.12
@@ -156,15 +153,15 @@
             return display_as_type(self.annotation)
 
         def __hash__(self) -> int:
             # Each ModelField is unique for our purposes,
             # to allow store them in a set.
             return id(self)
 
-    def extract_field_info(field_info: BaseFieldInfo) -> Dict[str, Any]:
+    def extract_field_info(field_info: BaseFieldInfo) -> dict[str, Any]:
         """Get FieldInfo init kwargs from a FieldInfo instance."""
 
         kwargs = field_info._attributes_set.copy()
         kwargs["annotation"] = field_info.rebuild_annotation()
         return kwargs
 
     def model_field_validate(
@@ -172,69 +169,69 @@
     ) -> Any:
         """Validate the value pass to the field."""
         type: Any = Annotated[model_field.annotation, model_field.field_info]
         return TypeAdapter(
             type, config=None if model_field._annotation_has_config() else config
         ).validate_python(value)
 
-    def model_fields(model: Type[BaseModel]) -> List[ModelField]:
+    def model_fields(model: type[BaseModel]) -> list[ModelField]:
         """Get field list of a model."""
 
         return [
             ModelField._construct(
                 name=name,
                 annotation=field_info.rebuild_annotation(),
                 field_info=FieldInfo(**extract_field_info(field_info)),
             )
             for name, field_info in model.model_fields.items()
         ]
 
-    def model_config(model: Type[BaseModel]) -> Any:
+    def model_config(model: type[BaseModel]) -> Any:
         """Get config of a model."""
         return model.model_config
 
     def model_dump(
         model: BaseModel,
-        include: Optional[Set[str]] = None,
-        exclude: Optional[Set[str]] = None,
+        include: Optional[set[str]] = None,
+        exclude: Optional[set[str]] = None,
         by_alias: bool = False,
         exclude_unset: bool = False,
         exclude_defaults: bool = False,
         exclude_none: bool = False,
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         return model.model_dump(
             include=include,
             exclude=exclude,
             by_alias=by_alias,
             exclude_unset=exclude_unset,
             exclude_defaults=exclude_defaults,
             exclude_none=exclude_none,
         )
 
-    def type_validate_python(type_: Type[T], data: Any) -> T:
+    def type_validate_python(type_: type[T], data: Any) -> T:
         """Validate data with given type."""
         return TypeAdapter(type_).validate_python(data)
 
-    def type_validate_json(type_: Type[T], data: Union[str, bytes]) -> T:
+    def type_validate_json(type_: type[T], data: Union[str, bytes]) -> T:
         """Validate JSON with given type."""
         return TypeAdapter(type_).validate_json(data)
 
     def __get_pydantic_core_schema__(
-        cls: Type["_CustomValidationClass"],
+        cls: type["_CustomValidationClass"],
         source_type: Any,
         handler: GetCoreSchemaHandler,
     ) -> CoreSchema:
         validators = list(cls.__get_validators__())
         if len(validators) == 1:
             return core_schema.no_info_plain_validator_function(validators[0])
         return core_schema.chain_schema(
             [core_schema.no_info_plain_validator_function(func) for func in validators]
         )
 
-    def custom_validation(class_: Type["CVC"]) -> Type["CVC"]:
+    def custom_validation(class_: type["CVC"]) -> type["CVC"]:
         """Use pydantic v1 like validator generator in pydantic v2"""
 
         setattr(
             class_,
             "__get_pydantic_core_schema__",
             classmethod(__get_pydantic_core_schema__),
         )
@@ -304,80 +301,80 @@
             """
             if field_info is not None:
                 annotation = get_annotation_from_field_info(
                     annotation, field_info, name
                 )
             return cls._construct(name, annotation, field_info or FieldInfo())
 
-    def extract_field_info(field_info: BaseFieldInfo) -> Dict[str, Any]:
+    def extract_field_info(field_info: BaseFieldInfo) -> dict[str, Any]:
         """Get FieldInfo init kwargs from a FieldInfo instance."""
 
         kwargs = {
             s: getattr(field_info, s) for s in field_info.__slots__ if s != "extra"
         }
         kwargs.update(field_info.extra)
         return kwargs
 
     def model_field_validate(
-        model_field: ModelField, value: Any, config: Optional[Type[ConfigDict]] = None
+        model_field: ModelField, value: Any, config: Optional[type[ConfigDict]] = None
     ) -> Any:
         """Validate the value pass to the field.
 
         Set config before validate to ensure validate correctly.
         """
 
         if model_field.model_config is not config:
             model_field.set_config(config or ConfigDict)
 
         v, errs_ = model_field.validate(value, {}, loc=())
         if errs_:
             raise ValueError(value, model_field)
         return v
 
-    def model_fields(model: Type[BaseModel]) -> List[ModelField]:
+    def model_fields(model: type[BaseModel]) -> list[ModelField]:
         """Get field list of a model."""
 
         # construct the model field without preprocess to avoid error
         return [
             ModelField._construct(
                 name=model_field.name,
                 annotation=model_field.annotation,
                 field_info=FieldInfo(
                     **extract_field_info(model_field.field_info),
                 ),
             )
             for model_field in model.__fields__.values()
         ]
 
-    def model_config(model: Type[BaseModel]) -> Any:
+    def model_config(model: type[BaseModel]) -> Any:
         """Get config of a model."""
         return model.__config__
 
     def model_dump(
         model: BaseModel,
-        include: Optional[Set[str]] = None,
-        exclude: Optional[Set[str]] = None,
+        include: Optional[set[str]] = None,
+        exclude: Optional[set[str]] = None,
         by_alias: bool = False,
         exclude_unset: bool = False,
         exclude_defaults: bool = False,
         exclude_none: bool = False,
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         return model.dict(
             include=include,
             exclude=exclude,
             by_alias=by_alias,
             exclude_unset=exclude_unset,
             exclude_defaults=exclude_defaults,
             exclude_none=exclude_none,
         )
 
-    def type_validate_python(type_: Type[T], data: Any) -> T:
+    def type_validate_python(type_: type[T], data: Any) -> T:
         """Validate data with given type."""
         return parse_obj_as(type_, data)
 
-    def type_validate_json(type_: Type[T], data: Union[str, bytes]) -> T:
+    def type_validate_json(type_: type[T], data: Union[str, bytes]) -> T:
         """Validate JSON with given type."""
         return parse_raw_as(type_, data)
 
-    def custom_validation(class_: Type["CVC"]) -> Type["CVC"]:
+    def custom_validation(class_: type["CVC"]) -> type["CVC"]:
         """Do nothing in pydantic v1"""
         return class_
```

### Comparing `nonebot2-2.2.1/nonebot/config.py` & `nonebot2-2.3.0/nonebot/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,27 +13,17 @@
 
 import os
 import abc
 import json
 from pathlib import Path
 from datetime import timedelta
 from ipaddress import IPv4Address
+from collections.abc import Mapping
+from typing import TYPE_CHECKING, Any, Union, Optional
 from typing_extensions import TypeAlias, get_args, get_origin
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Set,
-    Dict,
-    List,
-    Type,
-    Tuple,
-    Union,
-    Mapping,
-    Optional,
-)
 
 from dotenv import dotenv_values
 from pydantic import Field, BaseModel
 from pydantic.networks import IPvAnyAddress
 
 from nonebot.log import logger
 from nonebot.typing import origin_is_union
@@ -45,56 +35,56 @@
     PydanticUndefined,
     PydanticUndefinedType,
     model_config,
     model_fields,
 )
 
 DOTENV_TYPE: TypeAlias = Union[
-    Path, str, List[Union[Path, str]], Tuple[Union[Path, str], ...]
+    Path, str, list[Union[Path, str]], tuple[Union[Path, str], ...]
 ]
 
 ENV_FILE_SENTINEL = Path("")
 
 
 class SettingsError(ValueError): ...
 
 
 class BaseSettingsSource(abc.ABC):
-    def __init__(self, settings_cls: Type["BaseSettings"]) -> None:
+    def __init__(self, settings_cls: type["BaseSettings"]) -> None:
         self.settings_cls = settings_cls
 
     @property
     def config(self) -> "SettingsConfig":
         return model_config(self.settings_cls)
 
     @abc.abstractmethod
-    def __call__(self) -> Dict[str, Any]:
+    def __call__(self) -> dict[str, Any]:
         raise NotImplementedError
 
 
 class InitSettingsSource(BaseSettingsSource):
     __slots__ = ("init_kwargs",)
 
     def __init__(
-        self, settings_cls: Type["BaseSettings"], init_kwargs: Dict[str, Any]
+        self, settings_cls: type["BaseSettings"], init_kwargs: dict[str, Any]
     ) -> None:
         self.init_kwargs = init_kwargs
         super().__init__(settings_cls)
 
-    def __call__(self) -> Dict[str, Any]:
+    def __call__(self) -> dict[str, Any]:
         return self.init_kwargs
 
     def __repr__(self) -> str:
         return f"InitSettingsSource(init_kwargs={self.init_kwargs!r})"
 
 
 class DotEnvSettingsSource(BaseSettingsSource):
     def __init__(
         self,
-        settings_cls: Type["BaseSettings"],
+        settings_cls: type["BaseSettings"],
         env_file: Optional[DOTENV_TYPE] = ENV_FILE_SENTINEL,
         env_file_encoding: Optional[str] = None,
         case_sensitive: Optional[bool] = None,
         env_nested_delimiter: Optional[str] = None,
     ) -> None:
         super().__init__(settings_cls)
         self.env_file = (
@@ -117,43 +107,43 @@
             if env_nested_delimiter is not None
             else self.config.get("env_nested_delimiter", None)
         )
 
     def _apply_case_sensitive(self, var_name: str) -> str:
         return var_name if self.case_sensitive else var_name.lower()
 
-    def _field_is_complex(self, field: ModelField) -> Tuple[bool, bool]:
+    def _field_is_complex(self, field: ModelField) -> tuple[bool, bool]:
         if type_is_complex(field.annotation):
             return True, False
         elif origin_is_union(get_origin(field.annotation)) and any(
             type_is_complex(arg) for arg in get_args(field.annotation)
         ):
             return True, True
         return False, False
 
     def _parse_env_vars(
         self, env_vars: Mapping[str, Optional[str]]
-    ) -> Dict[str, Optional[str]]:
+    ) -> dict[str, Optional[str]]:
         return {
             self._apply_case_sensitive(key): value for key, value in env_vars.items()
         }
 
-    def _read_env_file(self, file_path: Path) -> Dict[str, Optional[str]]:
+    def _read_env_file(self, file_path: Path) -> dict[str, Optional[str]]:
         file_vars = dotenv_values(file_path, encoding=self.env_file_encoding)
         return self._parse_env_vars(file_vars)
 
-    def _read_env_files(self) -> Dict[str, Optional[str]]:
+    def _read_env_files(self) -> dict[str, Optional[str]]:
         env_files = self.env_file
         if env_files is None:
             return {}
 
         if isinstance(env_files, (str, os.PathLike)):
             env_files = [env_files]
 
-        dotenv_vars: Dict[str, Optional[str]] = {}
+        dotenv_vars: dict[str, Optional[str]] = {}
         for env_file in env_files:
             env_path = Path(env_file).expanduser()
             if env_path.is_file():
                 dotenv_vars.update(self._read_env_file(env_path))
         return dotenv_vars
 
     def _next_field(
@@ -166,22 +156,22 @@
                 if field.name == key:
                     return field
         return None
 
     def _explode_env_vars(
         self,
         field: ModelField,
-        env_vars: Dict[str, Optional[str]],
-        env_file_vars: Dict[str, Optional[str]],
-    ) -> Dict[str, Any]:
+        env_vars: dict[str, Optional[str]],
+        env_file_vars: dict[str, Optional[str]],
+    ) -> dict[str, Any]:
         if self.env_nested_delimiter is None:
             return {}
 
         prefix = f"{field.name}{self.env_nested_delimiter}"
-        result: Dict[str, Any] = {}
+        result: dict[str, Any] = {}
         for env_name, env_val in env_vars.items():
             if not env_name.startswith(prefix):
                 continue
 
             # delete from file vars when used
             if env_name in env_file_vars:
                 del env_file_vars[env_name]
@@ -205,18 +195,18 @@
                                 f'error parsing env var "{env_name}"'
                             ) from e
 
             env_var[last_key] = env_val
 
         return result
 
-    def __call__(self) -> Dict[str, Any]:
+    def __call__(self) -> dict[str, Any]:
         """从环境变量和 dotenv 配置文件中读取配置项。"""
 
-        d: Dict[str, Any] = {}
+        d: dict[str, Any] = {}
 
         env_vars = self._parse_env_vars(os.environ)
         env_file_vars = self._read_env_files()
         env_vars = {**env_file_vars, **env_vars}
 
         for field in model_fields(self.settings_cls):
             field_name = field.name
@@ -313,15 +303,15 @@
 class BaseSettings(BaseModel):
     if TYPE_CHECKING:
         # dummy getattr for pylance checking, actually not used
         def __getattr__(self, name: str) -> Any:  # pragma: no cover
             return self.__dict__.get(name)
 
     if PYDANTIC_V2:  # pragma: pydantic-v2
-        model_config: SettingsConfig = SettingsConfig(
+        model_config = SettingsConfig(
             extra="allow",
             env_file=".env",
             env_file_encoding="utf-8",
             case_sensitive=False,
             env_nested_delimiter="__",
         )
     else:  # pragma: pydantic-v1
@@ -347,19 +337,19 @@
                 env_file_encoding=_env_file_encoding,
                 env_nested_delimiter=_env_nested_delimiter,
             )
         )
 
     def _settings_build_values(
         self,
-        init_kwargs: Dict[str, Any],
+        init_kwargs: dict[str, Any],
         env_file: Optional[DOTENV_TYPE] = None,
         env_file_encoding: Optional[str] = None,
         env_nested_delimiter: Optional[str] = None,
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         init_settings = InitSettingsSource(self.__class__, init_kwargs=init_kwargs)
         env_settings = DotEnvSettingsSource(
             self.__class__,
             env_file=env_file,
             env_file_encoding=env_file_encoding,
             env_nested_delimiter=env_nested_delimiter,
         )
@@ -422,35 +412,35 @@
     """
 
     # bot connection configs
     api_timeout: Optional[float] = 30.0
     """API 请求超时时间，单位: 秒。"""
 
     # bot runtime configs
-    superusers: Set[str] = set()
+    superusers: set[str] = set()
     """机器人超级用户。
 
     用法:
         ```conf
         SUPERUSERS=["12345789"]
         ```
     """
-    nickname: Set[str] = set()
+    nickname: set[str] = set()
     """机器人昵称。"""
-    command_start: Set[str] = {"/"}
+    command_start: set[str] = {"/"}
     """命令的起始标记，用于判断一条消息是不是命令。
 
     参考[命令响应规则](https://nonebot.dev/docs/advanced/matcher#command)。
 
     用法:
         ```conf
         COMMAND_START=["/", ""]
         ```
     """
-    command_sep: Set[str] = {"."}
+    command_sep: set[str] = {"."}
     """命令的分隔标记，用于将文本形式的命令切分为元组（实际的命令名）。
 
     参考[命令响应规则](https://nonebot.dev/docs/advanced/matcher#command)。
 
     用法:
         ```conf
         COMMAND_SEP=["."]
@@ -473,15 +463,17 @@
     # custom configs can be assigned during nonebot.init
     # or from env file using json loads
 
     if PYDANTIC_V2:  # pragma: pydantic-v2
         model_config = SettingsConfig(env_file=(".env", ".env.prod"))
     else:  # pragma: pydantic-v1
 
-        class Config(SettingsConfig):
+        class Config(  # pyright: ignore[reportIncompatibleVariableOverride]
+            SettingsConfig
+        ):
             env_file = ".env", ".env.prod"
 
 
 __autodoc__ = {
     "SettingsError": False,
     "BaseSettingsSource": False,
     "InitSettingsSource": False,
```

### Comparing `nonebot2-2.2.1/nonebot/consts.py` & `nonebot2-2.3.0/nonebot/consts.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.2.1/nonebot/dependencies/__init__.py` & `nonebot2-2.3.0/nonebot/dependencies/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,16 @@
     description: nonebot.dependencies 模块
 """
 
 import abc
 import asyncio
 import inspect
 from dataclasses import field, dataclass
-from typing import (
-    Any,
-    Dict,
-    List,
-    Type,
-    Tuple,
-    Generic,
-    TypeVar,
-    Callable,
-    Iterable,
-    Optional,
-    Awaitable,
-    cast,
-)
+from collections.abc import Iterable, Awaitable
+from typing import Any, Generic, TypeVar, Callable, Optional, cast
 
 from nonebot.log import logger
 from nonebot.typing import _DependentCallable
 from nonebot.exception import SkippedException
 from nonebot.utils import run_sync, is_coroutine_callable
 from nonebot.compat import FieldInfo, ModelField, PydanticUndefined
 
@@ -44,21 +32,21 @@
 
     def __init__(self, *args, validate: bool = False, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
         self.validate = validate
 
     @classmethod
     def _check_param(
-        cls, param: inspect.Parameter, allow_types: Tuple[Type["Param"], ...]
+        cls, param: inspect.Parameter, allow_types: tuple[type["Param"], ...]
     ) -> Optional["Param"]:
         return
 
     @classmethod
     def _check_parameterless(
-        cls, value: Any, allow_types: Tuple[Type["Param"], ...]
+        cls, value: Any, allow_types: tuple[type["Param"], ...]
     ) -> Optional["Param"]:
         return
 
     @abc.abstractmethod
     async def _solve(self, **kwargs: Any) -> Any:
         raise NotImplementedError
 
@@ -75,16 +63,16 @@
         pre_checkers: 依赖注入解析前的参数检查
         params: 具名参数列表
         parameterless: 匿名参数列表
         allow_types: 允许的参数类型
     """
 
     call: _DependentCallable[R]
-    params: Tuple[ModelField, ...] = field(default_factory=tuple)
-    parameterless: Tuple[Param, ...] = field(default_factory=tuple)
+    params: tuple[ModelField, ...] = field(default_factory=tuple)
+    parameterless: tuple[Param, ...] = field(default_factory=tuple)
 
     def __repr__(self) -> str:
         if inspect.isfunction(self.call) or inspect.isclass(self.call):
             call_str = self.call.__name__
         else:
             call_str = repr(self.call)
         return (
@@ -108,17 +96,17 @@
                 return await run_sync(cast(Callable[..., R], self.call))(**values)
         except SkippedException as e:
             logger.trace(f"{self} skipped due to {e}")
             raise
 
     @staticmethod
     def parse_params(
-        call: _DependentCallable[R], allow_types: Tuple[Type[Param], ...]
-    ) -> Tuple[ModelField, ...]:
-        fields: List[ModelField] = []
+        call: _DependentCallable[R], allow_types: tuple[type[Param], ...]
+    ) -> tuple[ModelField, ...]:
+        fields: list[ModelField] = []
         params = get_typed_signature(call).parameters.values()
 
         for param in params:
             if isinstance(param.default, Param):
                 field_info = param.default
             else:
                 for allow_type in allow_types:
@@ -140,17 +128,17 @@
                 )
             )
 
         return tuple(fields)
 
     @staticmethod
     def parse_parameterless(
-        parameterless: Tuple[Any, ...], allow_types: Tuple[Type[Param], ...]
-    ) -> Tuple[Param, ...]:
-        parameterless_params: List[Param] = []
+        parameterless: tuple[Any, ...], allow_types: tuple[type[Param], ...]
+    ) -> tuple[Param, ...]:
+        parameterless_params: list[Param] = []
         for value in parameterless:
             for allow_type in allow_types:
                 if param := allow_type._check_parameterless(value, allow_types):
                     break
             else:
                 raise ValueError(f"Unknown parameterless {value}")
             parameterless_params.append(param)
@@ -158,15 +146,15 @@
 
     @classmethod
     def parse(
         cls,
         *,
         call: _DependentCallable[R],
         parameterless: Optional[Iterable[Any]] = None,
-        allow_types: Iterable[Type[Param]],
+        allow_types: Iterable[type[Param]],
     ) -> "Dependent[R]":
         allow_types = tuple(allow_types)
 
         params = cls.parse_params(call, allow_types)
         parameterless_params = (
             ()
             if parameterless is None
@@ -177,23 +165,23 @@
 
     async def check(self, **params: Any) -> None:
         await asyncio.gather(*(param._check(**params) for param in self.parameterless))
         await asyncio.gather(
             *(cast(Param, param.field_info)._check(**params) for param in self.params)
         )
 
-    async def _solve_field(self, field: ModelField, params: Dict[str, Any]) -> Any:
+    async def _solve_field(self, field: ModelField, params: dict[str, Any]) -> Any:
         param = cast(Param, field.field_info)
         value = await param._solve(**params)
         if value is PydanticUndefined:
             value = field.get_default()
         v = check_field_type(field, value)
         return v if param.validate else value
 
-    async def solve(self, **params: Any) -> Dict[str, Any]:
+    async def solve(self, **params: Any) -> dict[str, Any]:
         # solve parameterless
         for param in self.parameterless:
             await param._solve(**params)
 
         # solve param values
         values = await asyncio.gather(
             *(self._solve_field(field, params) for field in self.params)
```

### Comparing `nonebot2-2.2.1/nonebot/dependencies/utils.py` & `nonebot2-2.3.0/nonebot/dependencies/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 FrontMatter:
     sidebar_position: 1
     description: nonebot.dependencies.utils 模块
 """
 
 import inspect
-from typing import Any, Dict, Callable, ForwardRef
+from typing import Any, Callable, ForwardRef
 
 from loguru import logger
 
 from nonebot.exception import TypeMisMatch
 from nonebot.typing import evaluate_forwardref
 from nonebot.compat import DEFAULT_CONFIG, ModelField, model_field_validate
 
@@ -27,15 +27,15 @@
             annotation=get_typed_annotation(param, globalns),
         )
         for param in signature.parameters.values()
     ]
     return inspect.Signature(typed_params)
 
 
-def get_typed_annotation(param: inspect.Parameter, globalns: Dict[str, Any]) -> Any:
+def get_typed_annotation(param: inspect.Parameter, globalns: dict[str, Any]) -> Any:
     """获取参数的类型注解"""
 
     annotation = param.annotation
     if isinstance(annotation, str):
         annotation = ForwardRef(annotation)
         try:
             annotation = evaluate_forwardref(annotation, globalns, globalns)
```

### Comparing `nonebot2-2.2.1/nonebot/drivers/__init__.py` & `nonebot2-2.3.0/nonebot/drivers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from nonebot.internal.driver import ForwardMixin as ForwardMixin
 from nonebot.internal.driver import ReverseMixin as ReverseMixin
 from nonebot.internal.driver import ForwardDriver as ForwardDriver
 from nonebot.internal.driver import ReverseDriver as ReverseDriver
 from nonebot.internal.driver import combine_driver as combine_driver
 from nonebot.internal.driver import HTTPClientMixin as HTTPClientMixin
 from nonebot.internal.driver import HTTPServerSetup as HTTPServerSetup
+from nonebot.internal.driver import HTTPClientSession as HTTPClientSession
 from nonebot.internal.driver import WebSocketClientMixin as WebSocketClientMixin
 from nonebot.internal.driver import WebSocketServerSetup as WebSocketServerSetup
 
 __autodoc__ = {
     "URL": True,
     "Cookies": True,
     "Request": True,
```

### Comparing `nonebot2-2.2.1/nonebot/drivers/fastapi.py` & `nonebot2-2.3.0/nonebot/drivers/fastapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     description: nonebot.drivers.fastapi 模块
 """
 
 import logging
 import contextlib
 from functools import wraps
 from typing_extensions import override
-from typing import Any, Dict, List, Tuple, Union, Optional
+from typing import Any, Union, Optional
 
 from pydantic import BaseModel
 
 from nonebot.config import Env
 from nonebot.drivers import ASGIMixin
 from nonebot.exception import WebSocketClosed
 from nonebot.internal.driver import FileTypes
@@ -68,23 +68,23 @@
     """`swagger` 地址，默认为 `None` 即关闭"""
     fastapi_redoc_url: Optional[str] = None
     """`redoc` 地址，默认为 `None` 即关闭"""
     fastapi_include_adapter_schema: bool = True
     """是否包含适配器路由的 schema，默认为 `True`"""
     fastapi_reload: bool = False
     """开启/关闭冷重载"""
-    fastapi_reload_dirs: Optional[List[str]] = None
+    fastapi_reload_dirs: Optional[list[str]] = None
     """重载监控文件夹列表，默认为 uvicorn 默认值"""
     fastapi_reload_delay: float = 0.25
     """重载延迟，默认为 uvicorn 默认值"""
-    fastapi_reload_includes: Optional[List[str]] = None
+    fastapi_reload_includes: Optional[list[str]] = None
     """要监听的文件列表，支持 glob pattern，默认为 uvicorn 默认值"""
-    fastapi_reload_excludes: Optional[List[str]] = None
+    fastapi_reload_excludes: Optional[list[str]] = None
     """不要监听的文件列表，支持 glob pattern，默认为 uvicorn 默认值"""
-    fastapi_extra: Dict[str, Any] = {}
+    fastapi_extra: dict[str, Any] = {}
     """传递给 `FastAPI` 的其他参数。"""
 
 
 class Driver(BaseDriver, ASGIMixin):
     """FastAPI 驱动框架。"""
 
     def __init__(self, env: Env, config: NoneBotConfig):
@@ -157,15 +157,15 @@
             await self._lifespan.shutdown()
 
     @override
     def run(
         self,
         host: Optional[str] = None,
         port: Optional[int] = None,
-        *,
+        *args,
         app: Optional[str] = None,
         **kwargs,
     ):
         """使用 `uvicorn` 启动 FastAPI"""
         super().run(host, port, app=app, **kwargs)
         LOGGING_CONFIG = {
             "version": 1,
@@ -202,15 +202,15 @@
         setup: HTTPServerSetup,
     ) -> Response:
         json: Any = None
         with contextlib.suppress(Exception):
             json = await request.json()
 
         data: Optional[dict] = None
-        files: Optional[List[Tuple[str, FileTypes]]] = None
+        files: Optional[list[tuple[str, FileTypes]]] = None
         with contextlib.suppress(Exception):
             form = await request.form()
             data = {}
             files = []
             for key, value in form.multi_items():
                 if isinstance(value, UploadFile):
                     files.append(
```

### Comparing `nonebot2-2.2.1/nonebot/drivers/none.py` & `nonebot2-2.3.0/nonebot/drivers/none.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,17 +64,19 @@
         await self._shutdown()
 
     async def _startup(self):
         try:
             await self._lifespan.startup()
         except Exception as e:
             logger.opt(colors=True, exception=e).error(
-                "<r><bg #f8bbd0>Error when running startup function. "
-                "Ignored!</bg #f8bbd0></r>"
+                "<r><bg #f8bbd0>Application startup failed. "
+                "Exiting.</bg #f8bbd0></r>"
             )
+            self.should_exit.set()
+            return
 
         logger.info("Application startup completed.")
 
     async def _main_loop(self):
         await self.should_exit.wait()
 
     async def _shutdown(self):
```

### Comparing `nonebot2-2.2.1/nonebot/drivers/quart.py` & `nonebot2-2.3.0/nonebot/drivers/quart.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     sidebar_position: 5
     description: nonebot.drivers.quart 模块
 """
 
 import asyncio
 from functools import wraps
 from typing_extensions import override
-from typing import Any, Dict, List, Tuple, Union, Optional, cast
+from typing import Any, Union, Optional, cast
 
 from pydantic import BaseModel
 
 from nonebot.config import Env
 from nonebot.drivers import ASGIMixin
 from nonebot.exception import WebSocketClosed
 from nonebot.internal.driver import FileTypes
@@ -60,23 +60,23 @@
 
 
 class Config(BaseModel):
     """Quart 驱动框架设置"""
 
     quart_reload: bool = False
     """开启/关闭冷重载"""
-    quart_reload_dirs: Optional[List[str]] = None
+    quart_reload_dirs: Optional[list[str]] = None
     """重载监控文件夹列表，默认为 uvicorn 默认值"""
     quart_reload_delay: float = 0.25
     """重载延迟，默认为 uvicorn 默认值"""
-    quart_reload_includes: Optional[List[str]] = None
+    quart_reload_includes: Optional[list[str]] = None
     """要监听的文件列表，支持 glob pattern，默认为 uvicorn 默认值"""
-    quart_reload_excludes: Optional[List[str]] = None
+    quart_reload_excludes: Optional[list[str]] = None
     """不要监听的文件列表，支持 glob pattern，默认为 uvicorn 默认值"""
-    quart_extra: Dict[str, Any] = {}
+    quart_extra: dict[str, Any] = {}
     """传递给 `Quart` 的其他参数。"""
 
 
 class Driver(BaseDriver, ASGIMixin):
     """Quart 驱动框架"""
 
     def __init__(self, env: Env, config: NoneBotConfig):
@@ -138,15 +138,15 @@
         )
 
     @override
     def run(
         self,
         host: Optional[str] = None,
         port: Optional[int] = None,
-        *,
+        *args,
         app: Optional[str] = None,
         **kwargs,
     ):
         """使用 `uvicorn` 启动 Quart"""
         super().run(host, port, app, **kwargs)
         LOGGING_CONFIG = {
             "version": 1,
@@ -180,15 +180,15 @@
     async def _handle_http(self, setup: HTTPServerSetup) -> Response:
         request: Request = _request
 
         json = await request.get_json() if request.is_json else None
 
         data = await request.form
         files_dict = await request.files
-        files: List[Tuple[str, FileTypes]] = []
+        files: list[tuple[str, FileTypes]] = []
         key: str
         value: FileStorage
         for key, value in files_dict.items():
             files.append((key, (value.filename, value.stream, value.content_type)))
 
         http_request = BaseRequest(
             request.method,
```

### Comparing `nonebot2-2.2.1/nonebot/drivers/websockets.py` & `nonebot2-2.3.0/nonebot/drivers/websockets.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,16 @@
     description: nonebot.drivers.websockets 模块
 """
 
 import logging
 from functools import wraps
 from contextlib import asynccontextmanager
 from typing_extensions import ParamSpec, override
-from typing import TYPE_CHECKING, Union, TypeVar, Callable, Awaitable, AsyncGenerator
+from collections.abc import Coroutine, AsyncGenerator
+from typing import TYPE_CHECKING, Any, Union, TypeVar, Callable
 
 from nonebot.drivers import Request
 from nonebot.log import LoguruHandler
 from nonebot.exception import WebSocketClosed
 from nonebot.drivers.none import Driver as NoneDriver
 from nonebot.drivers import WebSocket as BaseWebSocket
 from nonebot.drivers import WebSocketClientMixin, combine_driver
@@ -40,15 +41,17 @@
 T = TypeVar("T")
 P = ParamSpec("P")
 
 logger = logging.Logger("websockets.client", "INFO")
 logger.addHandler(LoguruHandler())
 
 
-def catch_closed(func: Callable[P, Awaitable[T]]) -> Callable[P, Awaitable[T]]:
+def catch_closed(
+    func: Callable[P, Coroutine[Any, Any, T]]
+) -> Callable[P, Coroutine[Any, Any, T]]:
     @wraps(func)
     async def decorator(*args: P.args, **kwargs: P.kwargs) -> T:
         try:
             return await func(*args, **kwargs)
         except ConnectionClosed as e:
             raise WebSocketClosed(e.code, e.reason)
```

### Comparing `nonebot2-2.2.1/nonebot/exception.py` & `nonebot2-2.3.0/nonebot/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.2.1/nonebot/internal/adapter/adapter.py` & `nonebot2-2.3.0/nonebot/internal/adapter/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import abc
+from typing import Any
+from collections.abc import AsyncGenerator
 from contextlib import asynccontextmanager
-from typing import Any, Dict, AsyncGenerator
 
 from nonebot.config import Config
 from nonebot.internal.driver._lifespan import LIFESPAN_FUNC
 from nonebot.internal.driver import (
     Driver,
     Request,
     Response,
@@ -28,15 +29,15 @@
         driver: {ref}`nonebot.drivers.Driver` 实例
         kwargs: 其他由 {ref}`nonebot.drivers.Driver.register_adapter` 传入的额外参数
     """
 
     def __init__(self, driver: Driver, **kwargs: Any):
         self.driver: Driver = driver
         """{ref}`nonebot.drivers.Driver` 实例"""
-        self.bots: Dict[str, Bot] = {}
+        self.bots: dict[str, Bot] = {}
         """本协议适配器已建立连接的 {ref}`nonebot.adapters.Bot` 实例"""
 
     def __repr__(self) -> str:
         return f"Adapter(name={self.get_name()!r})"
 
     @classmethod
     @abc.abstractmethod
```

### Comparing `nonebot2-2.2.1/nonebot/internal/adapter/bot.py` & `nonebot2-2.3.0/nonebot/internal/adapter/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import abc
 import asyncio
 from functools import partial
-from typing import TYPE_CHECKING, Any, Set, Union, Optional, Protocol
+from typing import TYPE_CHECKING, Any, Union, ClassVar, Optional, Protocol
 
 from nonebot.log import logger
 from nonebot.config import Config
 from nonebot.exception import MockApiException
 from nonebot.typing import T_CalledAPIHook, T_CallingAPIHook
 
 if TYPE_CHECKING:
@@ -23,17 +23,17 @@
     用于处理上报消息，并提供 API 调用接口。
 
     参数:
         adapter: 协议适配器实例
         self_id: 机器人 ID
     """
 
-    _calling_api_hook: Set[T_CallingAPIHook] = set()
+    _calling_api_hook: ClassVar[set[T_CallingAPIHook]] = set()
     """call_api 时执行的函数"""
-    _called_api_hook: Set[T_CalledAPIHook] = set()
+    _called_api_hook: ClassVar[set[T_CalledAPIHook]] = set()
     """call_api 后执行的函数"""
 
     def __init__(self, adapter: "Adapter", self_id: str):
         self.adapter: "Adapter" = adapter
         """协议适配器实例"""
         self.self_id: str = self_id
         """机器人 ID"""
```

### Comparing `nonebot2-2.2.1/nonebot/internal/adapter/event.py` & `nonebot2-2.3.0/nonebot/internal/adapter/event.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import abc
-from typing import Any, Type, TypeVar
+from typing import Any, TypeVar
 
 from pydantic import BaseModel
 
 from nonebot.utils import DataclassEncoder
 from nonebot.compat import PYDANTIC_V2, ConfigDict
 
 from .message import Message
@@ -16,20 +16,20 @@
 
     if PYDANTIC_V2:  # pragma: pydantic-v2
         model_config = ConfigDict(extra="allow")
     else:  # pragma: pydantic-v1
 
         class Config(ConfigDict):
             extra = "allow"  # type: ignore
-            json_encoders = {Message: DataclassEncoder}
+            json_encoders = {Message: DataclassEncoder}  # noqa: RUF012
 
     if not PYDANTIC_V2:  # pragma: pydantic-v1
 
         @classmethod
-        def validate(cls: Type["E"], value: Any) -> "E":
+        def validate(cls: type["E"], value: Any) -> "E":
             if isinstance(value, Event) and not isinstance(value, cls):
                 raise TypeError(f"{value} is incompatible with Event type {cls}")
             return super().validate(value)
 
     @abc.abstractmethod
     def get_type(self) -> str:
         """获取事件类型的方法，类型通常为 NoneBot 内置的四种类型。"""
```

### Comparing `nonebot2-2.2.1/nonebot/internal/adapter/message.py` & `nonebot2-2.3.0/nonebot/internal/adapter/message.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import abc
 from copy import deepcopy
 from typing_extensions import Self
+from collections.abc import Iterable
 from dataclasses import field, asdict, dataclass
-from typing import (
+from typing import (  # noqa: UP035
     Any,
-    Dict,
-    List,
     Type,
-    Tuple,
     Union,
     Generic,
     TypeVar,
-    Iterable,
     Optional,
     SupportsIndex,
     overload,
 )
 
 from nonebot.compat import custom_validation, type_validate_python
 
@@ -28,32 +25,34 @@
 @custom_validation
 @dataclass
 class MessageSegment(abc.ABC, Generic[TM]):
     """消息段基类"""
 
     type: str
     """消息段类型"""
-    data: Dict[str, Any] = field(default_factory=dict)
+    data: dict[str, Any] = field(default_factory=dict)
     """消息段数据"""
 
     @classmethod
     @abc.abstractmethod
-    def get_message_class(cls) -> Type[TM]:
+    def get_message_class(cls) -> Type[TM]:  # noqa: UP006
         """获取消息数组类型"""
         raise NotImplementedError
 
     @abc.abstractmethod
     def __str__(self) -> str:
         """该消息段所代表的 str，在命令匹配部分使用"""
         raise NotImplementedError
 
     def __len__(self) -> int:
         return len(str(self))
 
-    def __ne__(self, other: Self) -> bool:
+    def __ne__(  # pyright: ignore[reportIncompatibleMethodOverride]
+        self, other: Self
+    ) -> bool:
         return not self == other
 
     def __add__(self: TMS, other: Union[str, TMS, Iterable[TMS]]) -> TM:
         return self.get_message_class()(self) + other
 
     def __radd__(self: TMS, other: Union[str, TMS, Iterable[TMS]]) -> TM:
         return self.get_message_class()(other) + self
@@ -97,15 +96,15 @@
     @abc.abstractmethod
     def is_text(self) -> bool:
         """当前消息段是否为纯文本"""
         raise NotImplementedError
 
 
 @custom_validation
-class Message(List[TMS], abc.ABC):
+class Message(list[TMS], abc.ABC):
     """消息序列
 
     参数:
         message: 消息内容
     """
 
     def __init__(
@@ -138,15 +137,15 @@
         返回:
             消息格式化器
         """
         return MessageTemplate(format_string, cls)
 
     @classmethod
     @abc.abstractmethod
-    def get_segment_class(cls) -> Type[TMS]:
+    def get_segment_class(cls) -> type[TMS]:
         """获取消息段类型"""
         raise NotImplementedError
 
     def __str__(self) -> str:
         return "".join(str(seg) for seg in self)
 
     @classmethod
@@ -173,15 +172,17 @@
 
     @staticmethod
     @abc.abstractmethod
     def _construct(msg: str) -> Iterable[TMS]:
         """构造消息数组"""
         raise NotImplementedError
 
-    def __add__(self, other: Union[str, TMS, Iterable[TMS]]) -> Self:
+    def __add__(  # pyright: ignore[reportIncompatibleMethodOverride]
+        self, other: Union[str, TMS, Iterable[TMS]]
+    ) -> Self:
         result = self.copy()
         result += other
         return result
 
     def __radd__(self, other: Union[str, TMS, Iterable[TMS]]) -> Self:
         result = self.__class__(other)
         return result + self
@@ -205,26 +206,26 @@
             args: 消息段类型
 
         返回:
             所有类型为 `args` 的消息段
         """
 
     @overload
-    def __getitem__(self, args: Tuple[str, int]) -> TMS:
+    def __getitem__(self, args: tuple[str, int]) -> TMS:
         """索引指定类型的消息段
 
         参数:
             args: 消息段类型和索引
 
         返回:
             类型为 `args[0]` 的消息段第 `args[1]` 个
         """
 
     @overload
-    def __getitem__(self, args: Tuple[str, slice]) -> Self:
+    def __getitem__(self, args: tuple[str, slice]) -> Self:
         """切片指定类型的消息段
 
         参数:
             args: 消息段类型和切片
 
         返回:
             类型为 `args[0]` 的消息段切片 `args[1]`
@@ -248,20 +249,20 @@
         参数:
             args: 切片
 
         返回:
             消息切片 `args`
         """
 
-    def __getitem__(
+    def __getitem__(  # pyright: ignore[reportIncompatibleMethodOverride]
         self,
         args: Union[
             str,
-            Tuple[str, int],
-            Tuple[str, slice],
+            tuple[str, int],
+            tuple[str, slice],
             int,
             slice,
         ],
     ) -> Union[TMS, Self]:
         arg1, arg2 = args if isinstance(args, tuple) else (args, None)
         if isinstance(arg1, int) and arg2 is None:
             return super().__getitem__(arg1)
@@ -272,15 +273,17 @@
         elif isinstance(arg1, str) and isinstance(arg2, int):
             return [seg for seg in self if seg.type == arg1][arg2]
         elif isinstance(arg1, str) and isinstance(arg2, slice):
             return self.__class__([seg for seg in self if seg.type == arg1][arg2])
         else:
             raise ValueError("Incorrect arguments to slice")  # pragma: no cover
 
-    def __contains__(self, value: Union[TMS, str]) -> bool:
+    def __contains__(  # pyright: ignore[reportIncompatibleMethodOverride]
+        self, value: Union[TMS, str]
+    ) -> bool:
         """检查消息段是否存在
 
         参数:
             value: 消息段或消息段类型
         返回:
             消息内是否存在给定消息段或给定类型的消息段
         """
@@ -355,29 +358,33 @@
         返回:
             是否仅包含指定消息段
         """
         if isinstance(value, str):
             return all(seg.type == value for seg in self)
         return all(seg == value for seg in self)
 
-    def append(self, obj: Union[str, TMS]) -> Self:
+    def append(  # pyright: ignore[reportIncompatibleMethodOverride]
+        self, obj: Union[str, TMS]
+    ) -> Self:
         """添加一个消息段到消息数组末尾。
 
         参数:
             obj: 要添加的消息段
         """
         if isinstance(obj, MessageSegment):
             super().append(obj)
         elif isinstance(obj, str):
             self.extend(self._construct(obj))
         else:
             raise ValueError(f"Unexpected type: {type(obj)} {obj}")  # pragma: no cover
         return self
 
-    def extend(self, obj: Union[Self, Iterable[TMS]]) -> Self:
+    def extend(  # pyright: ignore[reportIncompatibleMethodOverride]
+        self, obj: Union[Self, Iterable[TMS]]
+    ) -> Self:
         """拼接一个消息数组或多个消息段到消息数组末尾。
 
         参数:
             obj: 要添加的消息数组
         """
         for segment in obj:
             self.append(segment)
```

### Comparing `nonebot2-2.2.1/nonebot/internal/adapter/template.py` & `nonebot2-2.3.0/nonebot/internal/adapter/template.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,31 @@
 import functools
 from string import Formatter
 from typing_extensions import TypeAlias
+from collections.abc import Mapping, Sequence
 from typing import (
     TYPE_CHECKING,
     Any,
-    Set,
-    Dict,
-    List,
-    Type,
-    Tuple,
     Union,
     Generic,
-    Mapping,
     TypeVar,
     Callable,
     Optional,
-    Sequence,
     cast,
     overload,
 )
 
 from _string import formatter_field_name_split  # type: ignore
 
 if TYPE_CHECKING:
     from .message import Message, MessageSegment
 
-    def formatter_field_name_split(  # noqa: F811
+    def formatter_field_name_split(
         field_name: str,
-    ) -> Tuple[str, List[Tuple[bool, str]]]: ...
+    ) -> tuple[str, list[tuple[bool, str]]]: ...
 
 
 TM = TypeVar("TM", bound="Message")
 TF = TypeVar("TF", str, "Message")
 
 FormatSpecFunc: TypeAlias = Callable[[Any], str]
 FormatSpecFunc_T = TypeVar("FormatSpecFunc_T", bound=FormatSpecFunc)
@@ -46,50 +40,52 @@
         private_getattr: 是否允许在模板中访问私有属性，默认为 `False`
     """
 
     @overload
     def __init__(
         self: "MessageTemplate[str]",
         template: str,
-        factory: Type[str] = str,
+        factory: type[str] = str,
         private_getattr: bool = False,
     ) -> None: ...
 
     @overload
     def __init__(
         self: "MessageTemplate[TM]",
         template: Union[str, TM],
-        factory: Type[TM],
+        factory: type[TM],
         private_getattr: bool = False,
     ) -> None: ...
 
     def __init__(
         self,
         template: Union[str, TM],
-        factory: Union[Type[str], Type[TM]] = str,
+        factory: Union[type[str], type[TM]] = str,
         private_getattr: bool = False,
     ) -> None:
         self.template: TF = template  # type: ignore
-        self.factory: Type[TF] = factory  # type: ignore
-        self.format_specs: Dict[str, FormatSpecFunc] = {}
+        self.factory: type[TF] = factory  # type: ignore
+        self.format_specs: dict[str, FormatSpecFunc] = {}
         self.private_getattr = private_getattr
 
     def __repr__(self) -> str:
         return f"MessageTemplate({self.template!r}, factory={self.factory!r})"
 
     def add_format_spec(
         self, spec: FormatSpecFunc_T, name: Optional[str] = None
     ) -> FormatSpecFunc_T:
         name = name or spec.__name__
         if name in self.format_specs:
             raise ValueError(f"Format spec {name} already exists!")
         self.format_specs[name] = spec
         return spec
 
-    def format(self, *args, **kwargs):
+    def format(  # pyright: ignore[reportIncompatibleMethodOverride]
+        self, *args, **kwargs
+    ) -> TF:
         """根据传入参数和模板生成消息对象"""
         return self._format(args, kwargs)
 
     def format_map(self, mapping: Mapping[str, Any]) -> TF:
         """根据传入字典和模板生成消息对象, 在传入字段名不是有效标识符时有用"""
         return self._format([], mapping)
 
@@ -114,31 +110,31 @@
                     full_message += msg
         else:
             raise TypeError("template must be a string or instance of Message!")
 
         self.check_unused_args(used_args, args, kwargs)
         return cast(TF, full_message)
 
-    def vformat(
+    def vformat(  # pyright: ignore[reportIncompatibleMethodOverride]
         self,
         format_string: str,
         args: Sequence[Any],
         kwargs: Mapping[str, Any],
     ) -> TF:
         raise NotImplementedError("`vformat` has merged into `_format`")
 
-    def _vformat(
+    def _vformat(  # pyright: ignore[reportIncompatibleMethodOverride]
         self,
         format_string: str,
         args: Sequence[Any],
         kwargs: Mapping[str, Any],
-        used_args: Set[Union[int, str]],
+        used_args: set[Union[int, str]],
         auto_arg_index: int = 0,
-    ) -> Tuple[TF, int]:
-        results: List[Any] = [self.factory()]
+    ) -> tuple[TF, int]:
+        results: list[Any] = [self.factory()]
 
         for literal_text, field_name, format_spec, conversion in self.parse(
             format_string
         ):
             # output the literal text
             if literal_text:
                 results.append(literal_text)
@@ -181,29 +177,29 @@
                 )
                 results.append(formatted_text)
 
         return functools.reduce(self._add, results), auto_arg_index
 
     def get_field(
         self, field_name: str, args: Sequence[Any], kwargs: Mapping[str, Any]
-    ) -> Tuple[Any, Union[int, str]]:
+    ) -> tuple[Any, Union[int, str]]:
         first, rest = formatter_field_name_split(field_name)
         obj = self.get_value(first, args, kwargs)
 
         for is_attr, value in rest:
             if not self.private_getattr and value.startswith("_"):
                 raise ValueError("Cannot access private attribute")
             obj = getattr(obj, value) if is_attr else obj[value]
 
         return obj, first
 
     def format_field(self, value: Any, format_spec: str) -> Any:
         formatter: Optional[FormatSpecFunc] = self.format_specs.get(format_spec)
         if formatter is None and not issubclass(self.factory, str):
-            segment_class: Type["MessageSegment"] = self.factory.get_segment_class()
+            segment_class: type["MessageSegment"] = self.factory.get_segment_class()
             method = getattr(segment_class, format_spec, None)
             if callable(method) and not cast(str, method.__name__).startswith("_"):
                 formatter = getattr(segment_class, format_spec)
         return (
             super().format_field(value, format_spec)
             if formatter is None
             else formatter(value)
```

### Comparing `nonebot2-2.2.1/nonebot/internal/driver/__init__.py` & `nonebot2-2.3.0/nonebot/internal/driver/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,9 +22,10 @@
 from .abstract import ForwardMixin as ForwardMixin
 from .abstract import ReverseMixin as ReverseMixin
 from .abstract import ForwardDriver as ForwardDriver
 from .abstract import ReverseDriver as ReverseDriver
 from .combine import combine_driver as combine_driver
 from .model import HTTPServerSetup as HTTPServerSetup
 from .abstract import HTTPClientMixin as HTTPClientMixin
+from .abstract import HTTPClientSession as HTTPClientSession
 from .model import WebSocketServerSetup as WebSocketServerSetup
 from .abstract import WebSocketClientMixin as WebSocketClientMixin
```

### Comparing `nonebot2-2.2.1/nonebot/internal/driver/_lifespan.py` & `nonebot2-2.3.0/nonebot/internal/driver/_lifespan.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+from collections.abc import Awaitable
 from typing_extensions import TypeAlias
-from typing import Any, List, Union, Callable, Awaitable, cast
+from typing import Any, Union, Callable, cast
 
 from nonebot.utils import run_sync, is_coroutine_callable
 
 SYNC_LIFESPAN_FUNC: TypeAlias = Callable[[], Any]
 ASYNC_LIFESPAN_FUNC: TypeAlias = Callable[[], Awaitable[Any]]
 LIFESPAN_FUNC: TypeAlias = Union[SYNC_LIFESPAN_FUNC, ASYNC_LIFESPAN_FUNC]
 
 
 class Lifespan:
     def __init__(self) -> None:
-        self._startup_funcs: List[LIFESPAN_FUNC] = []
-        self._ready_funcs: List[LIFESPAN_FUNC] = []
-        self._shutdown_funcs: List[LIFESPAN_FUNC] = []
+        self._startup_funcs: list[LIFESPAN_FUNC] = []
+        self._ready_funcs: list[LIFESPAN_FUNC] = []
+        self._shutdown_funcs: list[LIFESPAN_FUNC] = []
 
     def on_startup(self, func: LIFESPAN_FUNC) -> LIFESPAN_FUNC:
         self._startup_funcs.append(func)
         return func
 
     def on_shutdown(self, func: LIFESPAN_FUNC) -> LIFESPAN_FUNC:
         self._shutdown_funcs.append(func)
@@ -24,15 +25,15 @@
 
     def on_ready(self, func: LIFESPAN_FUNC) -> LIFESPAN_FUNC:
         self._ready_funcs.append(func)
         return func
 
     @staticmethod
     async def _run_lifespan_func(
-        funcs: List[LIFESPAN_FUNC],
+        funcs: list[LIFESPAN_FUNC],
     ) -> None:
         for func in funcs:
             if is_coroutine_callable(func):
                 await cast(ASYNC_LIFESPAN_FUNC, func)()
             else:
                 await run_sync(cast(SYNC_LIFESPAN_FUNC, func))()
```

### Comparing `nonebot2-2.2.1/nonebot/internal/driver/abstract.py` & `nonebot2-2.3.0/nonebot/internal/driver/abstract.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,39 @@
 import abc
 import asyncio
-from typing_extensions import TypeAlias
+from types import TracebackType
+from collections.abc import AsyncGenerator
+from typing_extensions import Self, TypeAlias
 from contextlib import AsyncExitStack, asynccontextmanager
-from typing import TYPE_CHECKING, Any, Set, Dict, Type, AsyncGenerator
+from typing import TYPE_CHECKING, Any, Union, ClassVar, Optional
 
 from nonebot.log import logger
 from nonebot.config import Env, Config
 from nonebot.dependencies import Dependent
 from nonebot.exception import SkippedException
 from nonebot.utils import escape_tag, run_coro_with_catch
 from nonebot.internal.params import BotParam, DependParam, DefaultParam
 from nonebot.typing import (
     T_DependencyCache,
     T_BotConnectionHook,
     T_BotDisconnectionHook,
 )
 
 from ._lifespan import LIFESPAN_FUNC, Lifespan
-from .model import Request, Response, WebSocket, HTTPServerSetup, WebSocketServerSetup
+from .model import (
+    Request,
+    Response,
+    WebSocket,
+    QueryTypes,
+    CookieTypes,
+    HeaderTypes,
+    HTTPVersion,
+    HTTPServerSetup,
+    WebSocketServerSetup,
+)
 
 if TYPE_CHECKING:
     from nonebot.internal.adapter import Bot, Adapter
 
 
 BOT_HOOK_PARAMS = [DependParam, BotParam, DefaultParam]
 
@@ -32,42 +44,42 @@
     驱动器控制框架的启动和停止，适配器的注册，以及机器人生命周期管理。
 
     参数:
         env: 包含环境信息的 Env 对象
         config: 包含配置信息的 Config 对象
     """
 
-    _adapters: Dict[str, "Adapter"] = {}
+    _adapters: ClassVar[dict[str, "Adapter"]] = {}
     """已注册的适配器列表"""
-    _bot_connection_hook: Set[Dependent[Any]] = set()
+    _bot_connection_hook: ClassVar[set[Dependent[Any]]] = set()
     """Bot 连接建立时执行的函数"""
-    _bot_disconnection_hook: Set[Dependent[Any]] = set()
+    _bot_disconnection_hook: ClassVar[set[Dependent[Any]]] = set()
     """Bot 连接断开时执行的函数"""
 
     def __init__(self, env: Env, config: Config):
         self.env: str = env.environment
         """环境名称"""
         self.config: Config = config
         """全局配置对象"""
-        self._bots: Dict[str, "Bot"] = {}
-        self._bot_tasks: Set[asyncio.Task] = set()
+        self._bots: dict[str, "Bot"] = {}
+        self._bot_tasks: set[asyncio.Task] = set()
         self._lifespan = Lifespan()
 
     def __repr__(self) -> str:
         return (
             f"Driver(type={self.type!r}, "
             f"adapters={len(self._adapters)}, bots={len(self._bots)})"
         )
 
     @property
-    def bots(self) -> Dict[str, "Bot"]:
+    def bots(self) -> dict[str, "Bot"]:
         """获取当前所有已连接的 Bot"""
         return self._bots
 
-    def register_adapter(self, adapter: Type["Adapter"], **kwargs) -> None:
+    def register_adapter(self, adapter: type["Adapter"], **kwargs) -> None:
         """注册一个协议适配器
 
         参数:
             adapter: 适配器类
             kwargs: 其他传递给适配器的参数
         """
         name = adapter.get_name()
@@ -218,22 +230,78 @@
     """客户端混入基类。"""
 
 
 class ReverseMixin(Mixin):
     """服务端混入基类。"""
 
 
+class HTTPClientSession(abc.ABC):
+    """HTTP 客户端会话基类。"""
+
+    @abc.abstractmethod
+    def __init__(
+        self,
+        params: QueryTypes = None,
+        headers: HeaderTypes = None,
+        cookies: CookieTypes = None,
+        version: Union[str, HTTPVersion] = HTTPVersion.H11,
+        timeout: Optional[float] = None,
+        proxy: Optional[str] = None,
+    ):
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    async def request(self, setup: Request) -> Response:
+        """发送一个 HTTP 请求"""
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    async def setup(self) -> None:
+        """初始化会话"""
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    async def close(self) -> None:
+        """关闭会话"""
+        raise NotImplementedError
+
+    async def __aenter__(self) -> Self:
+        await self.setup()
+        return self
+
+    async def __aexit__(
+        self,
+        exc_type: Optional[type[BaseException]],
+        exc: Optional[BaseException],
+        tb: Optional[TracebackType],
+    ) -> None:
+        await self.close()
+
+
 class HTTPClientMixin(ForwardMixin):
     """HTTP 客户端混入基类。"""
 
     @abc.abstractmethod
     async def request(self, setup: Request) -> Response:
         """发送一个 HTTP 请求"""
         raise NotImplementedError
 
+    @abc.abstractmethod
+    def get_session(
+        self,
+        params: QueryTypes = None,
+        headers: HeaderTypes = None,
+        cookies: CookieTypes = None,
+        version: Union[str, HTTPVersion] = HTTPVersion.H11,
+        timeout: Optional[float] = None,
+        proxy: Optional[str] = None,
+    ) -> HTTPClientSession:
+        """获取一个 HTTP 会话"""
+        raise NotImplementedError
+
 
 class WebSocketClientMixin(ForwardMixin):
     """WebSocket 客户端混入基类。"""
 
     @abc.abstractmethod
     @asynccontextmanager
     async def websocket(self, setup: Request) -> AsyncGenerator[WebSocket, None]:
```

### Comparing `nonebot2-2.2.1/nonebot/internal/driver/combine.py` & `nonebot2-2.3.0/nonebot/internal/driver/combine.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-from typing import TYPE_CHECKING, Type, Union, TypeVar, overload
+from typing import TYPE_CHECKING, Union, TypeVar, overload
 
 from .abstract import Mixin, Driver
 
 D = TypeVar("D", bound="Driver")
 
 if TYPE_CHECKING:
 
     class CombinedDriver(Driver, Mixin): ...
 
 
 @overload
-def combine_driver(driver: Type[D]) -> Type[D]: ...
+def combine_driver(driver: type[D]) -> type[D]: ...
 
 
 @overload
-def combine_driver(driver: Type[D], *mixins: Type[Mixin]) -> Type["CombinedDriver"]: ...
+def combine_driver(
+    driver: type[D], _m: type[Mixin], *mixins: type[Mixin]
+) -> type["CombinedDriver"]: ...
 
 
 def combine_driver(
-    driver: Type[D], *mixins: Type[Mixin]
-) -> Union[Type[D], Type["CombinedDriver"]]:
+    driver: type[D], *mixins: type[Mixin]
+) -> Union[type[D], type["CombinedDriver"]]:
     """将一个驱动器和多个混入类合并。"""
     # check first
     if not issubclass(driver, Driver):
         raise TypeError("`driver` must be subclass of Driver")
     if not all(issubclass(m, Mixin) for m in mixins):
         raise TypeError("`mixins` must be subclass of Mixin")
```

### Comparing `nonebot2-2.2.1/nonebot/internal/driver/model.py` & `nonebot2-2.3.0/nonebot/internal/driver/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,63 +1,51 @@
 import abc
 import urllib.request
 from enum import Enum
 from dataclasses import dataclass
 from typing_extensions import TypeAlias
 from http.cookiejar import Cookie, CookieJar
-from typing import (
-    IO,
-    Any,
-    Dict,
-    List,
-    Tuple,
-    Union,
-    Mapping,
-    Callable,
-    Iterator,
-    Optional,
-    Awaitable,
-    MutableMapping,
-)
+from typing import IO, Any, Union, Callable, Optional
+from collections.abc import Mapping, Iterator, Awaitable, MutableMapping
 
 from yarl import URL as URL
 from multidict import CIMultiDict
 
-RawURL: TypeAlias = Tuple[bytes, bytes, Optional[int], bytes]
+RawURL: TypeAlias = tuple[bytes, bytes, Optional[int], bytes]
 
 SimpleQuery: TypeAlias = Union[str, int, float]
-QueryVariable: TypeAlias = Union[SimpleQuery, List[SimpleQuery]]
+QueryVariable: TypeAlias = Union[SimpleQuery, list[SimpleQuery]]
 QueryTypes: TypeAlias = Union[
-    None, str, Mapping[str, QueryVariable], List[Tuple[str, QueryVariable]]
+    None, str, Mapping[str, QueryVariable], list[tuple[str, SimpleQuery]]
 ]
 
 HeaderTypes: TypeAlias = Union[
     None,
     CIMultiDict[str],
-    Dict[str, str],
-    List[Tuple[str, str]],
+    dict[str, str],
+    list[tuple[str, str]],
 ]
 
 CookieTypes: TypeAlias = Union[
-    None, "Cookies", CookieJar, Dict[str, str], List[Tuple[str, str]]
+    None, "Cookies", CookieJar, dict[str, str], list[tuple[str, str]]
 ]
 
 ContentTypes: TypeAlias = Union[str, bytes, None]
 DataTypes: TypeAlias = Union[dict, None]
 FileContent: TypeAlias = Union[IO[bytes], bytes]
-FileType: TypeAlias = Tuple[Optional[str], FileContent, Optional[str]]
+FileType: TypeAlias = tuple[Optional[str], FileContent, Optional[str]]
 FileTypes: TypeAlias = Union[
     # file (or bytes)
     FileContent,
     # (filename, file (or bytes))
-    Tuple[Optional[str], FileContent],
+    tuple[Optional[str], FileContent],
     # (filename, file (or bytes), content_type)
     FileType,
 ]
-FilesTypes: TypeAlias = Union[Dict[str, FileTypes], List[Tuple[str, FileTypes]], None]
+FilesTypes: TypeAlias = Union[dict[str, FileTypes], list[tuple[str, FileTypes]], None]
 
 
 class HTTPVersion(Enum):
     H10 = "1.0"
     H11 = "1.1"
     H2 = "2"
 
@@ -115,15 +103,15 @@
         # cookies
         self.cookies = Cookies(cookies)
 
         # body
         self.content: ContentTypes = content
         self.data: DataTypes = data
         self.json: Any = json
-        self.files: Optional[List[Tuple[str, FileType]]] = None
+        self.files: Optional[list[tuple[str, FileType]]] = None
         if files:
             self.files = []
             files_ = files.items() if isinstance(files, dict) else files
             for name, file_info in files_:
                 if not isinstance(file_info, tuple):
                     self.files.append((name, (name, file_info, None)))
                 elif len(file_info) == 2:
@@ -253,15 +241,15 @@
             comment=None,
             comment_url=None,
             rest={},
             rfc2109=False,
         )
         self.jar.set_cookie(cookie)
 
-    def get(
+    def get(  # pyright: ignore[reportIncompatibleMethodOverride]
         self,
         name: str,
         default: Optional[str] = None,
         domain: Optional[str] = None,
         path: Optional[str] = None,
     ) -> Optional[str]:
         value: Optional[str] = None
@@ -294,20 +282,22 @@
 
         for cookie in remove:
             self.jar.clear(cookie.domain, cookie.path, cookie.name)
 
     def clear(self, domain: Optional[str] = None, path: Optional[str] = None) -> None:
         self.jar.clear(domain, path)
 
-    def update(self, cookies: CookieTypes = None) -> None:
+    def update(  # pyright: ignore[reportIncompatibleMethodOverride]
+        self, cookies: CookieTypes = None
+    ) -> None:
         cookies = Cookies(cookies)
         for cookie in cookies.jar:
             self.jar.set_cookie(cookie)
 
-    def as_header(self, request: Request) -> Dict[str, str]:
+    def as_header(self, request: Request) -> dict[str, str]:
         urllib_request = self._CookieCompatRequest(request)
         self.jar.add_cookie_header(urllib_request)
         return urllib_request.added_headers
 
     def __setitem__(self, name: str, value: str) -> None:
         return self.set(name, value)
 
@@ -337,17 +327,19 @@
         def __init__(self, request: Request) -> None:
             super().__init__(
                 url=str(request.url),
                 headers=dict(request.headers),
                 method=request.method,
             )
             self.request = request
-            self.added_headers: Dict[str, str] = {}
+            self.added_headers: dict[str, str] = {}
 
-        def add_unredirected_header(self, key: str, value: str) -> None:
+        def add_unredirected_header(  # pyright: ignore[reportIncompatibleMethodOverride]
+            self, key: str, value: str
+        ) -> None:
             super().add_unredirected_header(key, value)
             self.added_headers[key] = value
 
 
 @dataclass
 class HTTPServerSetup:
     """HTTP 服务器路由配置。"""
```

### Comparing `nonebot2-2.2.1/nonebot/internal/matcher/__init__.py` & `nonebot2-2.3.0/nonebot/internal/matcher/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.2.1/nonebot/internal/matcher/manager.py` & `nonebot2-2.3.0/nonebot/internal/matcher/manager.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,19 @@
-from typing import (
-    TYPE_CHECKING,
-    List,
-    Type,
-    Tuple,
-    Union,
-    TypeVar,
-    Iterator,
-    KeysView,
-    Optional,
-    ItemsView,
-    ValuesView,
-    MutableMapping,
-    overload,
-)
+from typing import TYPE_CHECKING, Union, TypeVar, Optional, overload
+from collections.abc import Iterator, KeysView, ItemsView, ValuesView, MutableMapping
 
 from .provider import DEFAULT_PROVIDER_CLASS, MatcherProvider
 
 if TYPE_CHECKING:
     from .matcher import Matcher
 
 T = TypeVar("T")
 
 
-class MatcherManager(MutableMapping[int, List[Type["Matcher"]]]):
+class MatcherManager(MutableMapping[int, list[type["Matcher"]]]):
     """事件响应器管理器
 
     实现了常用字典操作，用于管理事件响应器。
     """
 
     def __init__(self):
         self.provider: MatcherProvider = DEFAULT_PROVIDER_CLASS({})
@@ -39,63 +26,67 @@
 
     def __iter__(self) -> Iterator[int]:
         return iter(self.provider)
 
     def __len__(self) -> int:
         return len(self.provider)
 
-    def __getitem__(self, key: int) -> List[Type["Matcher"]]:
+    def __getitem__(self, key: int) -> list[type["Matcher"]]:
         return self.provider[key]
 
-    def __setitem__(self, key: int, value: List[Type["Matcher"]]) -> None:
+    def __setitem__(self, key: int, value: list[type["Matcher"]]) -> None:
         self.provider[key] = value
 
     def __delitem__(self, key: int) -> None:
         del self.provider[key]
 
     def __eq__(self, other: object) -> bool:
         return isinstance(other, MatcherManager) and self.provider == other.provider
 
     def keys(self) -> KeysView[int]:
         return self.provider.keys()
 
-    def values(self) -> ValuesView[List[Type["Matcher"]]]:
+    def values(self) -> ValuesView[list[type["Matcher"]]]:
         return self.provider.values()
 
-    def items(self) -> ItemsView[int, List[Type["Matcher"]]]:
+    def items(self) -> ItemsView[int, list[type["Matcher"]]]:
         return self.provider.items()
 
     @overload
-    def get(self, key: int) -> Optional[List[Type["Matcher"]]]: ...
+    def get(self, key: int) -> Optional[list[type["Matcher"]]]: ...
 
     @overload
-    def get(self, key: int, default: T) -> Union[List[Type["Matcher"]], T]: ...
+    def get(self, key: int, default: T) -> Union[list[type["Matcher"]], T]: ...
 
     def get(
         self, key: int, default: Optional[T] = None
-    ) -> Optional[Union[List[Type["Matcher"]], T]]:
+    ) -> Optional[Union[list[type["Matcher"]], T]]:
         return self.provider.get(key, default)
 
-    def pop(self, key: int) -> List[Type["Matcher"]]:
+    def pop(  # pyright: ignore[reportIncompatibleMethodOverride]
+        self, key: int
+    ) -> list[type["Matcher"]]:
         return self.provider.pop(key)
 
-    def popitem(self) -> Tuple[int, List[Type["Matcher"]]]:
+    def popitem(self) -> tuple[int, list[type["Matcher"]]]:
         return self.provider.popitem()
 
     def clear(self) -> None:
         self.provider.clear()
 
-    def update(self, __m: MutableMapping[int, List[Type["Matcher"]]]) -> None:
+    def update(  # pyright: ignore[reportIncompatibleMethodOverride]
+        self, __m: MutableMapping[int, list[type["Matcher"]]]
+    ) -> None:
         self.provider.update(__m)
 
     def setdefault(
-        self, key: int, default: List[Type["Matcher"]]
-    ) -> List[Type["Matcher"]]:
+        self, key: int, default: list[type["Matcher"]]
+    ) -> list[type["Matcher"]]:
         return self.provider.setdefault(key, default)
 
-    def set_provider(self, provider_class: Type[MatcherProvider]) -> None:
+    def set_provider(self, provider_class: type[MatcherProvider]) -> None:
         """设置事件响应器存储器
 
         参数:
             provider_class: 事件响应器存储器类
         """
         self.provider = provider_class(self.provider)
```

### Comparing `nonebot2-2.2.1/nonebot/internal/matcher/matcher.py` & `nonebot2-2.3.0/nonebot/internal/matcher/matcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,25 @@
 import inspect
 import warnings
 from pathlib import Path
 from types import ModuleType
 from dataclasses import dataclass
 from contextvars import ContextVar
 from typing_extensions import Self
+from collections.abc import Iterable
 from datetime import datetime, timedelta
 from contextlib import AsyncExitStack, contextmanager
-from typing import (
+from typing import (  # noqa: UP035
     TYPE_CHECKING,
     Any,
-    List,
     Type,
-    Tuple,
     Union,
     TypeVar,
     Callable,
     ClassVar,
-    Iterable,
     NoReturn,
     Optional,
     overload,
 )
 
 from nonebot.log import logger
 from nonebot.internal.rule import Rule
@@ -81,28 +79,33 @@
 current_handler: ContextVar[Dependent] = ContextVar("current_handler")
 
 
 @dataclass
 class MatcherSource:
     """Matcher 源代码上下文信息"""
 
-    plugin_name: Optional[str] = None
-    """事件响应器所在插件名称"""
+    plugin_id: Optional[str] = None
+    """事件响应器所在插件标识符"""
     module_name: Optional[str] = None
     """事件响应器所在插件模块的路径名"""
     lineno: Optional[int] = None
     """事件响应器所在行号"""
 
     @property
     def plugin(self) -> Optional["Plugin"]:
         """事件响应器所在插件"""
         from nonebot.plugin import get_plugin
 
-        if self.plugin_name is not None:
-            return get_plugin(self.plugin_name)
+        if self.plugin_id is not None:
+            return get_plugin(self.plugin_id)
+
+    @property
+    def plugin_name(self) -> Optional[str]:
+        """事件响应器所在插件名"""
+        return self.plugin and self.plugin.name
 
     @property
     def module(self) -> Optional[ModuleType]:
         if self.module_name is not None:
             return sys.modules.get(self.module_name)
 
     @property
@@ -137,15 +140,15 @@
 
     type: ClassVar[str] = ""
     """事件响应器类型"""
     rule: ClassVar[Rule] = Rule()
     """事件响应器匹配规则"""
     permission: ClassVar[Permission] = Permission()
     """事件响应器触发权限"""
-    handlers: List[Dependent[Any]] = []
+    handlers: ClassVar[list[Dependent[Any]]] = []
     """事件响应器拥有的事件处理函数列表"""
     priority: ClassVar[int] = 1
     """事件响应器优先级"""
     block: bool = False
     """事件响应器是否阻止事件传播"""
     temp: ClassVar[bool] = False
     """事件响应器是否为临时"""
@@ -156,26 +159,26 @@
     """事件响应器默认状态"""
 
     _default_type_updater: ClassVar[Optional[Dependent[str]]] = None
     """事件响应器类型更新函数"""
     _default_permission_updater: ClassVar[Optional[Dependent[Permission]]] = None
     """事件响应器权限更新函数"""
 
-    HANDLER_PARAM_TYPES: ClassVar[Tuple[Type[Param], ...]] = (
+    HANDLER_PARAM_TYPES: ClassVar[tuple[Type[Param], ...]] = (  # noqa: UP006
         DependParam,
         BotParam,
         EventParam,
         StateParam,
         ArgParam,
         MatcherParam,
         DefaultParam,
     )
 
     def __init__(self):
-        self.handlers = self.handlers.copy()
+        self.remain_handlers: list[Dependent[Any]] = self.handlers.copy()
         self.state = self._default_state.copy()
 
     def __repr__(self) -> str:
         return (
             f"{self.__class__.__name__}(type={self.type!r}"
             + (f", module={self.module_name}" if self.module_name else "")
             + (
@@ -188,29 +191,29 @@
 
     @classmethod
     def new(
         cls,
         type_: str = "",
         rule: Optional[Rule] = None,
         permission: Optional[Permission] = None,
-        handlers: Optional[List[Union[T_Handler, Dependent[Any]]]] = None,
+        handlers: Optional[list[Union[T_Handler, Dependent[Any]]]] = None,
         temp: bool = False,
         priority: int = 1,
         block: bool = False,
         *,
         plugin: Optional["Plugin"] = None,
         module: Optional[ModuleType] = None,
         source: Optional[MatcherSource] = None,
         expire_time: Optional[Union[datetime, timedelta]] = None,
         default_state: Optional[T_State] = None,
         default_type_updater: Optional[Union[T_TypeUpdater, Dependent[str]]] = None,
         default_permission_updater: Optional[
             Union[T_PermissionUpdater, Dependent[Permission]]
         ] = None,
-    ) -> Type[Self]:
+    ) -> Type[Self]:  # noqa: UP006
         """
         创建一个新的事件响应器，并存储至 `matchers <#matchers>`_
 
         参数:
             type_: 事件响应器类型，与 `event.get_type()` 一致时触发，空字符串表示任意
             rule: 匹配规则
             permission: 权限
@@ -243,15 +246,15 @@
                     "Pass `module` context info to create Matcher is deprecated. "
                     "Use `source` instead."
                 ),
                 DeprecationWarning,
             )
         source = source or (
             MatcherSource(
-                plugin_name=plugin and plugin.name,
+                plugin_id=plugin and plugin.id_,
                 module_name=module and module.__name__,
             )
             if plugin is not None or module is not None
             else None
         )
 
         NewMatcher = type(
@@ -326,24 +329,29 @@
 
     @classproperty
     def plugin(cls) -> Optional["Plugin"]:
         """事件响应器所在插件"""
         return cls._source and cls._source.plugin
 
     @classproperty
-    def module(cls) -> Optional[ModuleType]:
-        """事件响应器所在插件模块"""
-        return cls._source and cls._source.module
+    def plugin_id(cls) -> Optional[str]:
+        """事件响应器所在插件标识符"""
+        return cls._source and cls._source.plugin_id
 
     @classproperty
     def plugin_name(cls) -> Optional[str]:
         """事件响应器所在插件名"""
         return cls._source and cls._source.plugin_name
 
     @classproperty
+    def module(cls) -> Optional[ModuleType]:
+        """事件响应器所在插件模块"""
+        return cls._source and cls._source.module
+
+    @classproperty
     def module_name(cls) -> Optional[str]:
         """事件响应器所在插件模块路径"""
         return cls._source and cls._source.module_name
 
     @classmethod
     async def check_perm(
         cls,
@@ -453,15 +461,15 @@
         """装饰一个函数来指示 NoneBot 在接收用户新的一条消息后继续运行该函数
 
         参数:
             id: 消息 ID
             parameterless: 非参数类型依赖列表
         """
 
-        async def _receive(event: Event, matcher: "Matcher") -> Union[None, NoReturn]:
+        async def _receive(event: Event, matcher: "Matcher") -> None:
             matcher.set_target(RECEIVE_KEY.format(id=id))
             if matcher.get_target() == RECEIVE_KEY.format(id=id):
                 matcher.set_receive(id, event)
                 return
             if matcher.get_receive(id, ...) is not ...:
                 return
             await matcher.reject()
@@ -771,15 +779,15 @@
                 stack=stack,
                 dependency_cache=dependency_cache,
             )
         return Permission(User.from_event(event, perm=self.permission))
 
     async def resolve_reject(self):
         handler = current_handler.get()
-        self.handlers.insert(0, handler)
+        self.remain_handlers.insert(0, handler)
         if REJECT_CACHE_TARGET in self.state:
             self.state[REJECT_TARGET] = self.state[REJECT_CACHE_TARGET]
 
     @contextmanager
     def ensure_context(self, bot: Bot, event: Event):
         b_t = current_bot.set(bot)
         e_t = current_event.set(event)
@@ -805,16 +813,16 @@
         )
 
         with self.ensure_context(bot, event):
             try:
                 # Refresh preprocess state
                 self.state.update(state)
 
-                while self.handlers:
-                    handler = self.handlers.pop(0)
+                while self.remain_handlers:
+                    handler = self.remain_handlers.pop(0)
                     current_handler.set(handler)
                     logger.debug(f"Running handler {handler}")
                     try:
                         await handler(
                             matcher=self,
                             bot=bot,
                             event=event,
@@ -848,15 +856,15 @@
                 bot, event, stack, dependency_cache
             )
 
             self.new(
                 type_,
                 Rule(),
                 permission,
-                self.handlers,
+                self.remain_handlers,
                 temp=True,
                 priority=0,
                 block=True,
                 source=self.__class__._source,
                 expire_time=bot.config.session_expire_timeout,
                 default_state=self.state,
                 default_type_updater=self.__class__._default_type_updater,
@@ -868,15 +876,15 @@
                 bot, event, stack, dependency_cache
             )
 
             self.new(
                 type_,
                 Rule(),
                 permission,
-                self.handlers,
+                self.remain_handlers,
                 temp=True,
                 priority=0,
                 block=True,
                 source=self.__class__._source,
                 expire_time=bot.config.session_expire_timeout,
                 default_state=self.state,
                 default_type_updater=self.__class__._default_type_updater,
```

### Comparing `nonebot2-2.2.1/nonebot/internal/matcher/provider.py` & `nonebot2-2.3.0/nonebot/internal/matcher/provider.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import abc
+from typing import TYPE_CHECKING
 from collections import defaultdict
-from typing import TYPE_CHECKING, List, Type, Mapping, MutableMapping
+from collections.abc import Mapping, MutableMapping
 
 if TYPE_CHECKING:
     from .matcher import Matcher
 
 
-class MatcherProvider(abc.ABC, MutableMapping[int, List[Type["Matcher"]]]):
+class MatcherProvider(abc.ABC, MutableMapping[int, list[type["Matcher"]]]):
     """事件响应器存储器基类
 
     参数:
         matchers: 当前存储器中已有的事件响应器
     """
 
     @abc.abstractmethod
-    def __init__(self, matchers: Mapping[int, List[Type["Matcher"]]]):
+    def __init__(self, matchers: Mapping[int, list[type["Matcher"]]]):
         raise NotImplementedError
 
 
 class _DictProvider(defaultdict, MatcherProvider):
-    def __init__(self, matchers: Mapping[int, List[Type["Matcher"]]]):
+    def __init__(self, matchers: Mapping[int, list[type["Matcher"]]]):
         super().__init__(list, matchers)
 
 
 DEFAULT_PROVIDER_CLASS = _DictProvider
 """默认存储器类型"""
```

### Comparing `nonebot2-2.2.1/nonebot/internal/params.py` & `nonebot2-2.3.0/nonebot/internal/params.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import asyncio
 import inspect
+from typing_extensions import Self, get_args, override, get_origin
 from contextlib import AsyncExitStack, contextmanager, asynccontextmanager
-from typing_extensions import Self, Annotated, get_args, override, get_origin
 from typing import (
     TYPE_CHECKING,
     Any,
-    Type,
-    Tuple,
     Union,
     Literal,
     Callable,
     Optional,
+    Annotated,
     cast,
 )
 
 from pydantic.fields import FieldInfo as PydanticFieldInfo
 
 from nonebot.dependencies import Param, Dependent
 from nonebot.dependencies.utils import check_field_type
@@ -122,15 +121,15 @@
         kwargs["use_cache"] = use_cache
 
         return cls(**kwargs)
 
     @classmethod
     @override
     def _check_param(
-        cls, param: inspect.Parameter, allow_types: Tuple[Type[Param], ...]
+        cls, param: inspect.Parameter, allow_types: tuple[type[Param], ...]
     ) -> Optional[Self]:
         type_annotation, depends_inner = param.annotation, None
         # extract type annotation and dependency from Annotated
         if get_origin(param.annotation) is Annotated:
             type_annotation, *extra_args = get_args(param.annotation)
             depends_inner = next(
                 (x for x in reversed(extra_args) if isinstance(x, DependsInner)), None
@@ -162,15 +161,15 @@
         return cls._from_field(
             sub_dependent, depends_inner.use_cache, depends_inner.validate
         )
 
     @classmethod
     @override
     def _check_parameterless(
-        cls, value: Any, allow_types: Tuple[Type[Param], ...]
+        cls, value: Any, allow_types: tuple[type[Param], ...]
     ) -> Optional["Param"]:
         if isinstance(value, DependsInner):
             assert value.dependency, "Dependency cannot be empty"
             dependent = Dependent[Any].parse(
                 call=value.dependency, allow_types=allow_types
             )
             return cls._from_field(dependent, value.use_cache, value.validate)
@@ -245,15 +244,15 @@
             + (repr(self.checker.annotation) if self.checker is not None else "")
             + ")"
         )
 
     @classmethod
     @override
     def _check_param(
-        cls, param: inspect.Parameter, allow_types: Tuple[Type[Param], ...]
+        cls, param: inspect.Parameter, allow_types: tuple[type[Param], ...]
     ) -> Optional[Self]:
         from nonebot.adapters import Bot
 
         # param type is Bot(s) or subclass(es) of Bot or None
         if generic_check_issubclass(param.annotation, Bot):
             checker: Optional[ModelField] = None
             if param.annotation is not Bot:
@@ -262,19 +261,23 @@
                 )
             return cls(checker=checker)
         # legacy: param is named "bot" and has no type annotation
         elif param.annotation == param.empty and param.name == "bot":
             return cls()
 
     @override
-    async def _solve(self, bot: "Bot", **kwargs: Any) -> Any:
+    async def _solve(  # pyright: ignore[reportIncompatibleMethodOverride]
+        self, bot: "Bot", **kwargs: Any
+    ) -> Any:
         return bot
 
     @override
-    async def _check(self, bot: "Bot", **kwargs: Any) -> None:
+    async def _check(  # pyright: ignore[reportIncompatibleMethodOverride]
+        self, bot: "Bot", **kwargs: Any
+    ) -> None:
         if self.checker is not None:
             check_field_type(self.checker, bot)
 
 
 class EventParam(Param):
     """{ref}`nonebot.adapters.Event` 注入参数
 
@@ -295,15 +298,15 @@
             + (repr(self.checker.annotation) if self.checker is not None else "")
             + ")"
         )
 
     @classmethod
     @override
     def _check_param(
-        cls, param: inspect.Parameter, allow_types: Tuple[Type[Param], ...]
+        cls, param: inspect.Parameter, allow_types: tuple[type[Param], ...]
     ) -> Optional[Self]:
         from nonebot.adapters import Event
 
         # param type is Event(s) or subclass(es) of Event or None
         if generic_check_issubclass(param.annotation, Event):
             checker: Optional[ModelField] = None
             if param.annotation is not Event:
@@ -312,19 +315,23 @@
                 )
             return cls(checker=checker)
         # legacy: param is named "event" and has no type annotation
         elif param.annotation == param.empty and param.name == "event":
             return cls()
 
     @override
-    async def _solve(self, event: "Event", **kwargs: Any) -> Any:
+    async def _solve(  # pyright: ignore[reportIncompatibleMethodOverride]
+        self, event: "Event", **kwargs: Any
+    ) -> Any:
         return event
 
     @override
-    async def _check(self, event: "Event", **kwargs: Any) -> Any:
+    async def _check(  # pyright: ignore[reportIncompatibleMethodOverride]
+        self, event: "Event", **kwargs: Any
+    ) -> Any:
         if self.checker is not None:
             check_field_type(self.checker, event)
 
 
 class StateParam(Param):
     """事件处理状态注入参数
 
@@ -335,25 +342,27 @@
 
     def __repr__(self) -> str:
         return "StateParam()"
 
     @classmethod
     @override
     def _check_param(
-        cls, param: inspect.Parameter, allow_types: Tuple[Type[Param], ...]
+        cls, param: inspect.Parameter, allow_types: tuple[type[Param], ...]
     ) -> Optional[Self]:
         # param type is T_State
         if param.annotation is T_State:
             return cls()
         # legacy: param is named "state" and has no type annotation
         elif param.annotation == param.empty and param.name == "state":
             return cls()
 
     @override
-    async def _solve(self, state: T_State, **kwargs: Any) -> Any:
+    async def _solve(  # pyright: ignore[reportIncompatibleMethodOverride]
+        self, state: T_State, **kwargs: Any
+    ) -> Any:
         return state
 
 
 class MatcherParam(Param):
     """事件响应器实例注入参数
 
     本注入解析所有类型为且仅为 {ref}`nonebot.matcher.Matcher` 及其子类或 `None` 的参数。
@@ -373,15 +382,15 @@
             + (repr(self.checker.annotation) if self.checker is not None else "")
             + ")"
         )
 
     @classmethod
     @override
     def _check_param(
-        cls, param: inspect.Parameter, allow_types: Tuple[Type[Param], ...]
+        cls, param: inspect.Parameter, allow_types: tuple[type[Param], ...]
     ) -> Optional[Self]:
         from nonebot.matcher import Matcher
 
         # param type is Matcher(s) or subclass(es) of Matcher or None
         if generic_check_issubclass(param.annotation, Matcher):
             checker: Optional[ModelField] = None
             if param.annotation is not Matcher:
@@ -390,19 +399,23 @@
                 )
             return cls(checker=checker)
         # legacy: param is named "matcher" and has no type annotation
         elif param.annotation == param.empty and param.name == "matcher":
             return cls()
 
     @override
-    async def _solve(self, matcher: "Matcher", **kwargs: Any) -> Any:
+    async def _solve(  # pyright: ignore[reportIncompatibleMethodOverride]
+        self, matcher: "Matcher", **kwargs: Any
+    ) -> Any:
         return matcher
 
     @override
-    async def _check(self, matcher: "Matcher", **kwargs: Any) -> Any:
+    async def _check(  # pyright: ignore[reportIncompatibleMethodOverride]
+        self, matcher: "Matcher", **kwargs: Any
+    ) -> Any:
         if self.checker is not None:
             check_field_type(self.checker, matcher)
 
 
 class ArgInner:
     def __init__(
         self, key: Optional[str], type: Literal["message", "str", "plaintext"]
@@ -451,24 +464,26 @@
 
     def __repr__(self) -> str:
         return f"ArgParam(key={self.key!r}, type={self.type!r})"
 
     @classmethod
     @override
     def _check_param(
-        cls, param: inspect.Parameter, allow_types: Tuple[Type[Param], ...]
+        cls, param: inspect.Parameter, allow_types: tuple[type[Param], ...]
     ) -> Optional[Self]:
         if isinstance(param.default, ArgInner):
             return cls(key=param.default.key or param.name, type=param.default.type)
         elif get_origin(param.annotation) is Annotated:
             for arg in get_args(param.annotation)[:0:-1]:
                 if isinstance(arg, ArgInner):
                     return cls(key=arg.key or param.name, type=arg.type)
 
-    async def _solve(self, matcher: "Matcher", **kwargs: Any) -> Any:
+    async def _solve(  # pyright: ignore[reportIncompatibleMethodOverride]
+        self, matcher: "Matcher", **kwargs: Any
+    ) -> Any:
         message = matcher.get_arg(self.key)
         if message is None:
             return message
         if self.type == "message":
             return message
         elif self.type == "str":
             return str(message)
@@ -486,15 +501,15 @@
 
     def __repr__(self) -> str:
         return "ExceptionParam()"
 
     @classmethod
     @override
     def _check_param(
-        cls, param: inspect.Parameter, allow_types: Tuple[Type[Param], ...]
+        cls, param: inspect.Parameter, allow_types: tuple[type[Param], ...]
     ) -> Optional[Self]:
         # param type is Exception(s) or subclass(es) of Exception or None
         if generic_check_issubclass(param.annotation, Exception):
             return cls()
         # legacy: param is named "exception" and has no type annotation
         elif param.annotation == param.empty and param.name == "exception":
             return cls()
@@ -514,15 +529,15 @@
 
     def __repr__(self) -> str:
         return f"DefaultParam(default={self.default!r})"
 
     @classmethod
     @override
     def _check_param(
-        cls, param: inspect.Parameter, allow_types: Tuple[Type[Param], ...]
+        cls, param: inspect.Parameter, allow_types: tuple[type[Param], ...]
     ) -> Optional[Self]:
         if param.default != param.empty:
             return cls(default=param.default)
 
     @override
     async def _solve(self, **kwargs: Any) -> Any:
         return PydanticUndefined
```

### Comparing `nonebot2-2.2.1/nonebot/internal/permission.py` & `nonebot2-2.3.0/nonebot/internal/permission.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import asyncio
 from typing_extensions import Self
 from contextlib import AsyncExitStack
-from typing import Set, Tuple, Union, NoReturn, Optional
+from typing import Union, ClassVar, NoReturn, Optional
 
 from nonebot.dependencies import Dependent
 from nonebot.utils import run_coro_with_catch
 from nonebot.exception import SkippedException
 from nonebot.typing import T_DependencyCache, T_PermissionChecker
 
 from .adapter import Bot, Event
-from .params import BotParam, EventParam, DependParam, DefaultParam
+from .params import Param, BotParam, EventParam, DependParam, DefaultParam
 
 
 class Permission:
     """{ref}`nonebot.matcher.Matcher` 权限类。
 
     当事件传递时，在 {ref}`nonebot.matcher.Matcher` 运行前进行检查。
 
@@ -26,23 +26,23 @@
         # 等价于
         Permission(async_function, sync_function)
         ```
     """
 
     __slots__ = ("checkers",)
 
-    HANDLER_PARAM_TYPES = [
+    HANDLER_PARAM_TYPES: ClassVar[list[type[Param]]] = [
         DependParam,
         BotParam,
         EventParam,
         DefaultParam,
     ]
 
     def __init__(self, *checkers: Union[T_PermissionChecker, Dependent[bool]]) -> None:
-        self.checkers: Set[Dependent[bool]] = {
+        self.checkers: set[Dependent[bool]] = {
             (
                 checker
                 if isinstance(checker, Dependent)
                 else Dependent[bool].parse(
                     call=checker, allow_types=self.HANDLER_PARAM_TYPES
                 )
             )
@@ -118,15 +118,15 @@
         users: 会话 ID 元组
         perm: 需同时满足的权限
     """
 
     __slots__ = ("users", "perm")
 
     def __init__(
-        self, users: Tuple[str, ...], perm: Optional[Permission] = None
+        self, users: tuple[str, ...], perm: Optional[Permission] = None
     ) -> None:
         self.users = users
         self.perm = perm
 
     def __repr__(self) -> str:
         return (
             f"User(users={self.users}"
@@ -142,15 +142,15 @@
         return bool(
             session in self.users and (self.perm is None or await self.perm(bot, event))
         )
 
     @classmethod
     def _clean_permission(cls, perm: Permission) -> Optional[Permission]:
         if len(perm.checkers) == 1 and isinstance(
-            user_perm := tuple(perm.checkers)[0].call, cls
+            user_perm := next(iter(perm.checkers)).call, cls
         ):
             return user_perm.perm
         return perm
 
     @classmethod
     def from_event(cls, event: Event, perm: Optional[Permission] = None) -> Self:
         """从事件中获取会话 ID。
```

### Comparing `nonebot2-2.2.1/nonebot/internal/rule.py` & `nonebot2-2.3.0/nonebot/internal/rule.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import asyncio
 from contextlib import AsyncExitStack
-from typing import Set, Union, NoReturn, Optional
+from typing import Union, ClassVar, NoReturn, Optional
 
 from nonebot.dependencies import Dependent
 from nonebot.exception import SkippedException
 from nonebot.typing import T_State, T_RuleChecker, T_DependencyCache
 
 from .adapter import Bot, Event
-from .params import BotParam, EventParam, StateParam, DependParam, DefaultParam
+from .params import Param, BotParam, EventParam, StateParam, DependParam, DefaultParam
 
 
 class Rule:
     """{ref}`nonebot.matcher.Matcher` 规则类。
 
     当事件传递时，在 {ref}`nonebot.matcher.Matcher` 运行前进行检查。
 
@@ -24,24 +24,24 @@
         # 等价于
         Rule(async_function, sync_function)
         ```
     """
 
     __slots__ = ("checkers",)
 
-    HANDLER_PARAM_TYPES = [
+    HANDLER_PARAM_TYPES: ClassVar[list[type[Param]]] = [
         DependParam,
         BotParam,
         EventParam,
         StateParam,
         DefaultParam,
     ]
 
     def __init__(self, *checkers: Union[T_RuleChecker, Dependent[bool]]) -> None:
-        self.checkers: Set[Dependent[bool]] = {
+        self.checkers: set[Dependent[bool]] = {
             (
                 checker
                 if isinstance(checker, Dependent)
                 else Dependent[bool].parse(
                     call=checker, allow_types=self.HANDLER_PARAM_TYPES
                 )
             )
```

### Comparing `nonebot2-2.2.1/nonebot/log.py` & `nonebot2-2.3.0/nonebot/log.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 FrontMatter:
     sidebar_position: 7
     description: nonebot.log 模块
 """
 
 import sys
+import inspect
 import logging
 from typing import TYPE_CHECKING
 
 import loguru
 
 if TYPE_CHECKING:
     # avoid sphinx autodoc resolve annotation failed
@@ -41,25 +42,26 @@
 
 # default_handler = logging.StreamHandler(sys.stdout)
 # default_handler.setFormatter(
 #     logging.Formatter("[%(asctime)s %(name)s] %(levelname)s: %(message)s"))
 # logger.addHandler(default_handler)
 
 
+# https://loguru.readthedocs.io/en/stable/overview.html#entirely-compatible-with-standard-logging
 class LoguruHandler(logging.Handler):  # pragma: no cover
     """logging 与 loguru 之间的桥梁，将 logging 的日志转发到 loguru。"""
 
     def emit(self, record: logging.LogRecord):
         try:
             level = logger.level(record.levelname).name
         except ValueError:
             level = record.levelno
 
-        frame, depth = sys._getframe(6), 6
-        while frame and frame.f_code.co_filename == logging.__file__:
+        frame, depth = inspect.currentframe(), 0
+        while frame and (depth == 0 or frame.f_code.co_filename == logging.__file__):
             frame = frame.f_back
             depth += 1
 
         logger.opt(depth=depth, exception=record.exc_info).log(
             level, record.getMessage()
         )
```

### Comparing `nonebot2-2.2.1/nonebot/matcher.py` & `nonebot2-2.3.0/nonebot/matcher.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.2.1/nonebot/message.py` & `nonebot2-2.3.0/nonebot/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     description: nonebot.message 模块
 """
 
 import asyncio
 import contextlib
 from datetime import datetime
 from contextlib import AsyncExitStack
-from typing import TYPE_CHECKING, Any, Set, Dict, Type, Optional
+from typing import TYPE_CHECKING, Any, Optional
 
 from nonebot.log import logger
 from nonebot.rule import TrieRule
 from nonebot.dependencies import Dependent
 from nonebot.matcher import Matcher, matchers
 from nonebot.utils import escape_tag, run_coro_with_catch
 from nonebot.exception import (
@@ -42,18 +42,18 @@
     MatcherParam,
     ExceptionParam,
 )
 
 if TYPE_CHECKING:
     from nonebot.adapters import Bot, Event
 
-_event_preprocessors: Set[Dependent[Any]] = set()
-_event_postprocessors: Set[Dependent[Any]] = set()
-_run_preprocessors: Set[Dependent[Any]] = set()
-_run_postprocessors: Set[Dependent[Any]] = set()
+_event_preprocessors: set[Dependent[Any]] = set()
+_event_postprocessors: set[Dependent[Any]] = set()
+_run_preprocessors: set[Dependent[Any]] = set()
+_run_postprocessors: set[Dependent[Any]] = set()
 
 EVENT_PCS_PARAMS = (
     DependParam,
     BotParam,
     EventParam,
     StateParam,
     DefaultParam,
@@ -326,15 +326,15 @@
         except Exception as e:
             logger.opt(colors=True, exception=e).error(
                 "<r><bg #f8bbd0>Error when running RunPostProcessors</bg #f8bbd0></r>"
             )
 
 
 async def _check_matcher(
-    Matcher: Type[Matcher],
+    Matcher: type[Matcher],
     bot: "Bot",
     event: "Event",
     state: T_State,
     stack: Optional[AsyncExitStack] = None,
     dependency_cache: Optional[T_DependencyCache] = None,
 ) -> bool:
     """检查事件响应器是否符合运行条件。
@@ -377,15 +377,15 @@
         )
         return False
 
     return True
 
 
 async def _run_matcher(
-    Matcher: Type[Matcher],
+    Matcher: type[Matcher],
     bot: "Bot",
     event: "Event",
     state: T_State,
     stack: Optional[AsyncExitStack] = None,
     dependency_cache: Optional[T_DependencyCache] = None,
 ) -> None:
     """运行事件响应器。
@@ -442,15 +442,15 @@
     )
 
     if matcher.block:
         raise StopPropagation
 
 
 async def check_and_run_matcher(
-    Matcher: Type[Matcher],
+    Matcher: type[Matcher],
     bot: "Bot",
     event: "Event",
     state: T_State,
     stack: Optional[AsyncExitStack] = None,
     dependency_cache: Optional[T_DependencyCache] = None,
 ) -> None:
     """检查并运行事件响应器。
@@ -501,15 +501,15 @@
     try:
         log_msg += event.get_log_string()
     except NoLogException:
         show_log = False
     if show_log:
         logger.opt(colors=True).success(log_msg)
 
-    state: Dict[Any, Any] = {}
+    state: dict[Any, Any] = {}
     dependency_cache: T_DependencyCache = {}
 
     # create event scope context
     async with AsyncExitStack() as stack:
         if not await _apply_event_preprocessors(
             bot=bot,
             event=event,
```

### Comparing `nonebot2-2.2.1/nonebot/params.py` & `nonebot2-2.3.0/nonebot/params.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,16 @@
 """本模块定义了依赖注入的各类参数。
 
 FrontMatter:
     sidebar_position: 4
     description: nonebot.params 模块
 """
 
-from typing import (
-    Any,
-    Dict,
-    List,
-    Match,
-    Tuple,
-    Union,
-    Literal,
-    Callable,
-    Optional,
-    overload,
-)
+from re import Match
+from typing import Any, Union, Literal, Callable, Optional, overload
 
 from nonebot.typing import T_State
 from nonebot.matcher import Matcher
 from nonebot.internal.params import Arg as Arg
 from nonebot.internal.params import ArgStr as ArgStr
 from nonebot.internal.params import Depends as Depends
 from nonebot.internal.params import ArgParam as ArgParam
@@ -86,15 +76,15 @@
     return Depends(_event_to_me)
 
 
 def _command(state: T_State) -> Message:
     return state[PREFIX_KEY][CMD_KEY]
 
 
-def Command() -> Tuple[str, ...]:
+def Command() -> tuple[str, ...]:
     """消息命令元组"""
     return Depends(_command)
 
 
 def _raw_command(state: T_State) -> Message:
     return state[PREFIX_KEY][RAW_CMD_KEY]
 
@@ -136,15 +126,15 @@
 
 
 def ShellCommandArgs() -> Any:
     """shell 命令解析后的参数字典"""
     return Depends(_shell_command_args, use_cache=False)
 
 
-def _shell_command_argv(state: T_State) -> List[Union[str, MessageSegment]]:
+def _shell_command_argv(state: T_State) -> list[Union[str, MessageSegment]]:
     return state[SHELL_ARGV]
 
 
 def ShellCommandArgv() -> Any:
     """shell 命令原始参数列表"""
     return Depends(_shell_command_argv, use_cache=False)
 
@@ -155,19 +145,19 @@
 
 def RegexMatched() -> Match[str]:
     """正则匹配结果"""
     return Depends(_regex_matched, use_cache=False)
 
 
 def _regex_str(
-    groups: Tuple[Union[str, int], ...]
-) -> Callable[[T_State], Union[str, Tuple[Union[str, Any], ...], Any]]:
+    groups: tuple[Union[str, int], ...]
+) -> Callable[[T_State], Union[str, tuple[Union[str, Any], ...], Any]]:
     def _regex_str_dependency(
         state: T_State,
-    ) -> Union[str, Tuple[Union[str, Any], ...], Any]:
+    ) -> Union[str, tuple[Union[str, Any], ...], Any]:
         return _regex_matched(state).group(*groups)
 
     return _regex_str_dependency
 
 
 @overload
 def RegexStr(__group: Literal[0] = 0) -> str: ...
@@ -176,36 +166,36 @@
 @overload
 def RegexStr(__group: Union[str, int]) -> Union[str, Any]: ...
 
 
 @overload
 def RegexStr(
     __group1: Union[str, int], __group2: Union[str, int], *groups: Union[str, int]
-) -> Tuple[Union[str, Any], ...]: ...
+) -> tuple[Union[str, Any], ...]: ...
 
 
-def RegexStr(*groups: Union[str, int]) -> Union[str, Tuple[Union[str, Any], ...], Any]:
+def RegexStr(*groups: Union[str, int]) -> Union[str, tuple[Union[str, Any], ...], Any]:
     """正则匹配结果文本"""
     return Depends(_regex_str(groups), use_cache=False)
 
 
-def _regex_group(state: T_State) -> Tuple[Any, ...]:
+def _regex_group(state: T_State) -> tuple[Any, ...]:
     return _regex_matched(state).groups()
 
 
-def RegexGroup() -> Tuple[Any, ...]:
+def RegexGroup() -> tuple[Any, ...]:
     """正则匹配结果 group 元组"""
     return Depends(_regex_group, use_cache=False)
 
 
-def _regex_dict(state: T_State) -> Dict[str, Any]:
+def _regex_dict(state: T_State) -> dict[str, Any]:
     return _regex_matched(state).groupdict()
 
 
-def RegexDict() -> Dict[str, Any]:
+def RegexDict() -> dict[str, Any]:
     """正则匹配结果 group 字典"""
     return Depends(_regex_dict, use_cache=False)
 
 
 def _startswith(state: T_State) -> str:
     return state[STARTSWITH_KEY]
```

### Comparing `nonebot2-2.2.1/nonebot/permission.py` & `nonebot2-2.3.0/nonebot/permission.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.2.1/nonebot/plugin/load.py` & `nonebot2-2.3.0/nonebot/plugin/load.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,21 +4,22 @@
     sidebar_position: 1
     description: nonebot.plugin.load 模块
 """
 
 import json
 from pathlib import Path
 from types import ModuleType
-from typing import Set, Union, Iterable, Optional
+from typing import Union, Optional
+from collections.abc import Iterable
 
 from nonebot.utils import path_to_module_name
 
 from .model import Plugin
 from .manager import PluginManager
-from . import _managers, get_plugin, _current_plugin_chain, _module_name_to_plugin_name
+from . import _managers, get_plugin, _module_name_to_plugin_id
 
 try:  # pragma: py-gte-311
     import tomllib  # pyright: ignore[reportMissingImports]
 except ModuleNotFoundError:  # pragma: py-lt-311
     import tomli as tomllib
 
 
@@ -35,40 +36,40 @@
         else module_path
     )
     manager = PluginManager([module_path])
     _managers.append(manager)
     return manager.load_plugin(module_path)
 
 
-def load_plugins(*plugin_dir: str) -> Set[Plugin]:
+def load_plugins(*plugin_dir: str) -> set[Plugin]:
     """导入文件夹下多个插件，以 `_` 开头的插件不会被导入!
 
     参数:
         plugin_dir: 文件夹路径
     """
     manager = PluginManager(search_path=plugin_dir)
     _managers.append(manager)
     return manager.load_all_plugins()
 
 
 def load_all_plugins(
     module_path: Iterable[str], plugin_dir: Iterable[str]
-) -> Set[Plugin]:
+) -> set[Plugin]:
     """导入指定列表中的插件以及指定目录下多个插件，以 `_` 开头的插件不会被导入!
 
     参数:
         module_path: 指定插件集合
         plugin_dir: 指定文件夹路径集合
     """
     manager = PluginManager(module_path, plugin_dir)
     _managers.append(manager)
     return manager.load_all_plugins()
 
 
-def load_from_json(file_path: str, encoding: str = "utf-8") -> Set[Plugin]:
+def load_from_json(file_path: str, encoding: str = "utf-8") -> set[Plugin]:
     """导入指定 json 文件中的 `plugins` 以及 `plugin_dirs` 下多个插件。
     以 `_` 开头的插件不会被导入!
 
     参数:
         file_path: 指定 json 文件路径
         encoding: 指定 json 文件编码
 
@@ -91,15 +92,15 @@
     plugins = data.get("plugins")
     plugin_dirs = data.get("plugin_dirs")
     assert isinstance(plugins, list), "plugins must be a list of plugin name"
     assert isinstance(plugin_dirs, list), "plugin_dirs must be a list of directories"
     return load_all_plugins(set(plugins), set(plugin_dirs))
 
 
-def load_from_toml(file_path: str, encoding: str = "utf-8") -> Set[Plugin]:
+def load_from_toml(file_path: str, encoding: str = "utf-8") -> set[Plugin]:
     """导入指定 toml 文件 `[tool.nonebot]` 中的
     `plugins` 以及 `plugin_dirs` 下多个插件。
     以 `_` 开头的插件不会被导入!
 
     参数:
         file_path: 指定 toml 文件路径
         encoding: 指定 toml 文件编码
@@ -135,88 +136,93 @@
 
     参数:
         name: 插件名称
     """
     return load_plugin(f"nonebot.plugins.{name}")
 
 
-def load_builtin_plugins(*plugins: str) -> Set[Plugin]:
+def load_builtin_plugins(*plugins: str) -> set[Plugin]:
     """导入多个 NoneBot 内置插件。
 
     参数:
         plugins: 插件名称列表
     """
     return load_all_plugins([f"nonebot.plugins.{p}" for p in plugins], [])
 
 
 def _find_manager_by_name(name: str) -> Optional[PluginManager]:
     for manager in reversed(_managers):
-        if name in manager.plugins or name in manager.searched_plugins:
+        if (
+            name in manager.controlled_modules
+            or name in manager.controlled_modules.values()
+        ):
             return manager
 
 
 def require(name: str) -> ModuleType:
-    """获取一个插件的导出内容。
-
-    如果为 `load_plugins` 文件夹导入的插件，则为文件(夹)名。
+    """声明依赖插件。
 
     参数:
-        name: 插件名，即 {ref}`nonebot.plugin.model.Plugin.name`。
+        name: 插件模块名或插件标识符，仅在已声明插件的情况下可使用标识符。
 
     异常:
         RuntimeError: 插件无法加载
     """
-    plugin = get_plugin(_module_name_to_plugin_name(name))
+    if "." in name:
+        # name is a module name
+        plugin = get_plugin(_module_name_to_plugin_id(name))
+    else:
+        # name is a plugin id or simple module name (equals to plugin id)
+        plugin = get_plugin(name)
+
     # if plugin not loaded
-    if not plugin:
-        # plugin already declared
+    if plugin is None:
+        # plugin already declared, module name / plugin id
         if manager := _find_manager_by_name(name):
             plugin = manager.load_plugin(name)
+
         # plugin not declared, try to declare and load it
         else:
-            # clear current plugin chain, ensure plugin loaded in a new context
-            _t = _current_plugin_chain.set(())
-            try:
-                plugin = load_plugin(name)
-            finally:
-                _current_plugin_chain.reset(_t)
-    if not plugin:
+            plugin = load_plugin(name)
+
+    if plugin is None:
         raise RuntimeError(f'Cannot load plugin "{name}"!')
     return plugin.module
 
 
-def inherit_supported_adapters(*names: str) -> Optional[Set[str]]:
+def inherit_supported_adapters(*names: str) -> Optional[set[str]]:
     """获取已加载插件的适配器支持状态集合。
 
     如果传入了多个插件名称，返回值会自动取交集。
 
     参数:
         names: 插件名称列表。
 
     异常:
         RuntimeError: 插件未加载
         ValueError: 插件缺少元数据
     """
-    final_supported: Optional[Set[str]] = None
+    final_supported: Optional[set[str]] = None
 
     for name in names:
-        plugin = get_plugin(_module_name_to_plugin_name(name))
+        plugin = get_plugin(_module_name_to_plugin_id(name))
         if plugin is None:
-            raise RuntimeError(f'Plugin "{name}" is not loaded!')
+            raise RuntimeError(
+                f'Plugin "{name}" is not loaded! You should require it first.'
+            )
         meta = plugin.metadata
         if meta is None:
             raise ValueError(f'Plugin "{name}" has no metadata!')
-        support = meta.supported_adapters
-        if support is None:
+
+        if (raw := meta.supported_adapters) is None:
             continue
+
+        support = {
+            f"nonebot.adapters.{adapter[1:]}" if adapter.startswith("~") else adapter
+            for adapter in raw
+        }
+
         final_supported = (
             support if final_supported is None else (final_supported & support)
         )
 
-    return final_supported and {
-        (
-            f"nonebot.adapters.{adapter_name[1:]}"
-            if adapter_name.startswith("~")
-            else adapter_name
-        )
-        for adapter_name in final_supported
-    }
+    return final_supported
```

### Comparing `nonebot2-2.2.1/nonebot/plugin/manager.py` & `nonebot2-2.3.0/nonebot/plugin/manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,173 +8,200 @@
 """
 
 import sys
 import pkgutil
 import importlib
 from pathlib import Path
 from itertools import chain
+from typing import Optional
 from types import ModuleType
 from importlib.abc import MetaPathFinder
+from collections.abc import Iterable, Sequence
 from importlib.machinery import PathFinder, SourceFileLoader
-from typing import Set, Dict, List, Iterable, Optional, Sequence
 
 from nonebot.log import logger
 from nonebot.utils import escape_tag, path_to_module_name
 
 from .model import Plugin, PluginMetadata
 from . import (
     _managers,
     _new_plugin,
     _revert_plugin,
-    _current_plugin_chain,
-    _module_name_to_plugin_name,
+    _current_plugin,
+    _module_name_to_plugin_id,
 )
 
 
 class PluginManager:
     """插件管理器。
 
     参数:
         plugins: 独立插件模块名集合。
-        search_path: 插件搜索路径（文件夹）。
+        search_path: 插件搜索路径（文件夹），相对于当前工作目录。
     """
 
     def __init__(
         self,
         plugins: Optional[Iterable[str]] = None,
         search_path: Optional[Iterable[str]] = None,
     ):
         # simple plugin not in search path
-        self.plugins: Set[str] = set(plugins or [])
-        self.search_path: Set[str] = set(search_path or [])
+        self.plugins: set[str] = set(plugins or [])
+        self.search_path: set[str] = set(search_path or [])
 
         # cache plugins
-        self._third_party_plugin_names: Dict[str, str] = {}
-        self._searched_plugin_names: Dict[str, Path] = {}
-        self.prepare_plugins()
+        self._third_party_plugin_ids: dict[str, str] = {}
+        self._searched_plugin_ids: dict[str, str] = {}
+        self._prepare_plugins()
 
     def __repr__(self) -> str:
-        return f"PluginManager(plugins={self.plugins}, search_path={self.search_path})"
+        return f"PluginManager(available_plugins={self.controlled_modules})"
 
     @property
-    def third_party_plugins(self) -> Set[str]:
-        """返回所有独立插件名称。"""
-        return set(self._third_party_plugin_names.keys())
+    def third_party_plugins(self) -> set[str]:
+        """返回所有独立插件标识符。"""
+        return set(self._third_party_plugin_ids.keys())
 
     @property
-    def searched_plugins(self) -> Set[str]:
-        """返回已搜索到的插件名称。"""
-        return set(self._searched_plugin_names.keys())
+    def searched_plugins(self) -> set[str]:
+        """返回已搜索到的插件标识符。"""
+        return set(self._searched_plugin_ids.keys())
 
     @property
-    def available_plugins(self) -> Set[str]:
-        """返回当前插件管理器中可用的插件名称。"""
+    def available_plugins(self) -> set[str]:
+        """返回当前插件管理器中可用的插件标识符。"""
         return self.third_party_plugins | self.searched_plugins
 
-    def _previous_plugins(self) -> Set[str]:
-        _pre_managers: List[PluginManager]
+    @property
+    def controlled_modules(self) -> dict[str, str]:
+        """返回当前插件管理器中控制的插件标识符与模块路径映射字典。"""
+        return dict(
+            chain(
+                self._third_party_plugin_ids.items(), self._searched_plugin_ids.items()
+            )
+        )
+
+    def _previous_controlled_modules(self) -> dict[str, str]:
+        _pre_managers: list[PluginManager]
         if self in _managers:
             _pre_managers = _managers[: _managers.index(self)]
         else:
             _pre_managers = _managers[:]
 
         return {
-            *chain.from_iterable(manager.available_plugins for manager in _pre_managers)
+            plugin_id: module_name
+            for manager in _pre_managers
+            for plugin_id, module_name in manager.controlled_modules.items()
         }
 
-    def prepare_plugins(self) -> Set[str]:
+    def _prepare_plugins(self) -> set[str]:
         """搜索插件并缓存插件名称。"""
         # get all previous ready to load plugins
-        previous_plugins = self._previous_plugins()
-        searched_plugins: Dict[str, Path] = {}
-        third_party_plugins: Dict[str, str] = {}
+        previous_plugin_ids = self._previous_controlled_modules()
+
+        # if self not in global managers, merge self's controlled modules
+        def get_controlled_modules():
+            return (
+                previous_plugin_ids
+                if self in _managers
+                else {**previous_plugin_ids, **self.controlled_modules}
+            )
 
         # check third party plugins
         for plugin in self.plugins:
-            name = _module_name_to_plugin_name(plugin)
-            if name in third_party_plugins or name in previous_plugins:
+            plugin_id = _module_name_to_plugin_id(plugin, get_controlled_modules())
+            if (
+                plugin_id in self._third_party_plugin_ids
+                or plugin_id in previous_plugin_ids
+            ):
                 raise RuntimeError(
-                    f"Plugin already exists: {name}! Check your plugin name"
+                    f"Plugin already exists: {plugin_id}! Check your plugin name"
                 )
-            third_party_plugins[name] = plugin
-
-        self._third_party_plugin_names = third_party_plugins
+            self._third_party_plugin_ids[plugin_id] = plugin
 
         # check plugins in search path
         for module_info in pkgutil.iter_modules(self.search_path):
             # ignore if startswith "_"
             if module_info.name.startswith("_"):
                 continue
 
-            if (
-                module_info.name in searched_plugins
-                or module_info.name in previous_plugins
-                or module_info.name in third_party_plugins
-            ):
-                raise RuntimeError(
-                    f"Plugin already exists: {module_info.name}! Check your plugin name"
-                )
-
             if not (
                 module_spec := module_info.module_finder.find_spec(
                     module_info.name, None
                 )
             ):
                 continue
-            if not (module_path := module_spec.origin):
+
+            if not module_spec.origin:
                 continue
-            searched_plugins[module_info.name] = Path(module_path).resolve()
 
-        self._searched_plugin_names = searched_plugins
+            # get module name from path, pkgutil does not return the actual module name
+            module_path = Path(module_spec.origin).resolve()
+            module_name = path_to_module_name(module_path)
+            plugin_id = _module_name_to_plugin_id(module_name, get_controlled_modules())
+
+            if (
+                plugin_id in previous_plugin_ids
+                or plugin_id in self._third_party_plugin_ids
+                or plugin_id in self._searched_plugin_ids
+            ):
+                raise RuntimeError(
+                    f"Plugin already exists: {plugin_id}! Check your plugin name"
+                )
+
+            self._searched_plugin_ids[plugin_id] = module_name
 
         return self.available_plugins
 
     def load_plugin(self, name: str) -> Optional[Plugin]:
         """加载指定插件。
 
-        对于独立插件，可以使用完整插件模块名或者插件名称。
+        可以使用完整插件模块名或者插件标识符加载。
 
         参数:
-            name: 插件名称。
+            name: 插件名称或插件标识符。
         """
 
         try:
-            if name in self.plugins:
+            # load using plugin id
+            if name in self._third_party_plugin_ids:
+                module = importlib.import_module(self._third_party_plugin_ids[name])
+            elif name in self._searched_plugin_ids:
+                module = importlib.import_module(self._searched_plugin_ids[name])
+            # load using module name
+            elif (
+                name in self._third_party_plugin_ids.values()
+                or name in self._searched_plugin_ids.values()
+            ):
                 module = importlib.import_module(name)
-            elif name in self._third_party_plugin_names:
-                module = importlib.import_module(self._third_party_plugin_names[name])
-            elif name in self._searched_plugin_names:
-                module = importlib.import_module(
-                    path_to_module_name(self._searched_plugin_names[name])
-                )
             else:
                 raise RuntimeError(f"Plugin not found: {name}! Check your plugin name")
 
             if (
                 plugin := getattr(module, "__plugin__", None)
             ) is None or not isinstance(plugin, Plugin):
                 raise RuntimeError(
                     f"Module {module.__name__} is not loaded as a plugin! "
-                    "Make sure not to import it before loading."
+                    f"Make sure not to import it before loading."
                 )
             logger.opt(colors=True).success(
-                f'Succeeded to load plugin "<y>{escape_tag(plugin.name)}</y>"'
+                f'Succeeded to load plugin "<y>{escape_tag(plugin.id_)}</y>"'
                 + (
                     f' from "<m>{escape_tag(plugin.module_name)}</m>"'
-                    if plugin.module_name != plugin.name
+                    if plugin.module_name != plugin.id_
                     else ""
                 )
             )
             return plugin
         except Exception as e:
             logger.opt(colors=True, exception=e).error(
                 f'<r><bg #f8bbd0>Failed to import "{escape_tag(name)}"</bg #f8bbd0></r>'
             )
 
-    def load_all_plugins(self) -> Set[Plugin]:
+    def load_all_plugins(self) -> set[Plugin]:
         """加载所有可用插件。"""
 
         return set(
             filter(None, (self.load_plugin(name) for name in self.available_plugins))
         )
 
 
@@ -188,29 +215,24 @@
         if _managers:
             module_spec = PathFinder.find_spec(fullname, path, target)
             if not module_spec:
                 return
             module_origin = module_spec.origin
             if not module_origin:
                 return
-            module_path = Path(module_origin).resolve()
 
             for manager in reversed(_managers):
-                # use path instead of name in case of submodule name conflict
-                if (
-                    fullname in manager.plugins
-                    or module_path in manager._searched_plugin_names.values()
-                ):
+                if fullname in manager.controlled_modules.values():
                     module_spec.loader = PluginLoader(manager, fullname, module_origin)
                     return module_spec
         return
 
 
 class PluginLoader(SourceFileLoader):
-    def __init__(self, manager: PluginManager, fullname: str, path) -> None:
+    def __init__(self, manager: PluginManager, fullname: str, path: str) -> None:
         self.manager = manager
         self.loaded = False
         super().__init__(fullname, path)
 
     def create_module(self, spec) -> Optional[ModuleType]:
         if self.name in sys.modules:
             self.loaded = True
@@ -222,34 +244,25 @@
         if self.loaded:
             return
 
         # create plugin before executing
         plugin = _new_plugin(self.name, module, self.manager)
         setattr(module, "__plugin__", plugin)
 
-        # detect parent plugin before entering current plugin context
-        parent_plugins = _current_plugin_chain.get()
-        for pre_plugin in reversed(parent_plugins):
-            # ensure parent plugin is declared before current plugin
-            if _managers.index(pre_plugin.manager) < _managers.index(self.manager):
-                plugin.parent_plugin = pre_plugin
-                pre_plugin.sub_plugins.add(plugin)
-                break
-
         # enter plugin context
-        _plugin_token = _current_plugin_chain.set(parent_plugins + (plugin,))
+        _plugin_token = _current_plugin.set(plugin)
 
         try:
             super().exec_module(module)
         except Exception:
             _revert_plugin(plugin)
             raise
         finally:
             # leave plugin context
-            _current_plugin_chain.reset(_plugin_token)
+            _current_plugin.reset(_plugin_token)
 
         # get plugin metadata
         metadata: Optional[PluginMetadata] = getattr(module, "__plugin_meta__", None)
         plugin.metadata = metadata
 
         return
```

### Comparing `nonebot2-2.2.1/nonebot/plugin/model.py` & `nonebot2-2.3.0/nonebot/plugin/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     sidebar_position: 3
     description: nonebot.plugin.model 模块
 """
 
 import contextlib
 from types import ModuleType
 from dataclasses import field, dataclass
-from typing import TYPE_CHECKING, Any, Set, Dict, Type, Optional
+from typing import TYPE_CHECKING, Any, Type, Optional  # noqa: UP035
 
 from pydantic import BaseModel
 
 from nonebot.matcher import Matcher
 from nonebot.utils import resolve_dot_notation
 
 if TYPE_CHECKING:
@@ -31,27 +31,27 @@
     """插件功能介绍"""
     usage: str
     """插件使用方法"""
     type: Optional[str] = None
     """插件类型，用于商店分类"""
     homepage: Optional[str] = None
     """插件主页"""
-    config: Optional[Type[BaseModel]] = None
+    config: Optional[Type[BaseModel]] = None  # noqa: UP006
     """插件配置项"""
-    supported_adapters: Optional[Set[str]] = None
+    supported_adapters: Optional[set[str]] = None
     """插件支持的适配器模块路径
 
     格式为 `<module>[:<Adapter>]`，`~` 为 `nonebot.adapters.` 的缩写。
 
     `None` 表示支持**所有适配器**。
     """
-    extra: Dict[Any, Any] = field(default_factory=dict)
+    extra: dict[Any, Any] = field(default_factory=dict)
     """插件额外信息，可由插件编写者自由扩展定义"""
 
-    def get_supported_adapters(self) -> Optional[Set[Type["Adapter"]]]:
+    def get_supported_adapters(self) -> Optional[set[Type["Adapter"]]]:  # noqa: UP006
         """获取当前已安装的插件支持适配器类列表"""
         if self.supported_adapters is None:
             return None
 
         adapters = set()
         for adapter in self.supported_adapters:
             with contextlib.suppress(ModuleNotFoundError, AttributeError):
@@ -62,21 +62,28 @@
 
 
 @dataclass(eq=False)
 class Plugin:
     """存储插件信息"""
 
     name: str
-    """插件索引标识，NoneBot 使用 文件/文件夹 名称作为标识符"""
+    """插件名称，NoneBot 使用 文件/文件夹 名称作为插件名称"""
     module: ModuleType
     """插件模块对象"""
     module_name: str
     """点分割模块路径"""
     manager: "PluginManager"
     """导入该插件的插件管理器"""
-    matcher: Set[Type[Matcher]] = field(default_factory=set)
+    matcher: set[type[Matcher]] = field(default_factory=set)
     """插件加载时定义的 `Matcher`"""
     parent_plugin: Optional["Plugin"] = None
     """父插件"""
-    sub_plugins: Set["Plugin"] = field(default_factory=set)
+    sub_plugins: set["Plugin"] = field(default_factory=set)
     """子插件集合"""
     metadata: Optional[PluginMetadata] = None
+
+    @property
+    def id_(self) -> str:
+        """插件索引标识"""
+        return (
+            f"{self.parent_plugin.id_}:{self.name}" if self.parent_plugin else self.name
+        )
```

### Comparing `nonebot2-2.2.1/nonebot/plugin/on.py` & `nonebot2-2.3.0/nonebot/plugin/on.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,16 +5,16 @@
     description: nonebot.plugin.on 模块
 """
 
 import re
 import inspect
 import warnings
 from types import ModuleType
+from typing import Any, Union, Optional
 from datetime import datetime, timedelta
-from typing import Any, Set, Dict, List, Type, Tuple, Union, Optional
 
 from nonebot.adapters import Event
 from nonebot.permission import Permission
 from nonebot.dependencies import Dependent
 from nonebot.matcher import Matcher, MatcherSource
 from nonebot.typing import T_State, T_Handler, T_RuleChecker, T_PermissionChecker
 from nonebot.rule import (
@@ -27,27 +27,27 @@
     endswith,
     fullmatch,
     startswith,
     shell_command,
 )
 
 from .model import Plugin
+from .manager import _current_plugin
 from . import get_plugin_by_module_name
-from .manager import _current_plugin_chain
 
 
-def store_matcher(matcher: Type[Matcher]) -> None:
+def store_matcher(matcher: type[Matcher]) -> None:
     """存储一个事件响应器到插件。
 
     参数:
         matcher: 事件响应器
     """
     # only store the matcher defined when plugin loading
-    if plugin_chain := _current_plugin_chain.get():
-        plugin_chain[-1].matcher.add(matcher)
+    if plugin := _current_plugin.get():
+        plugin.matcher.add(matcher)
 
 
 def get_matcher_plugin(depth: int = 1) -> Optional[Plugin]:  # pragma: no cover
     """获取事件响应器定义所在插件。
 
     **Deprecated**, 请使用 {ref}`nonebot.plugin.on.get_matcher_source` 获取信息。
 
@@ -72,55 +72,60 @@
     warnings.warn(
         "`get_matcher_module` is deprecated, please use `get_matcher_source` instead",
         DeprecationWarning,
     )
     return (source := get_matcher_source(depth + 1)) and source.module
 
 
-def get_matcher_source(depth: int = 1) -> Optional[MatcherSource]:
+def get_matcher_source(depth: int = 0) -> Optional[MatcherSource]:
     """获取事件响应器定义所在源码信息。
 
     参数:
         depth: 调用栈深度
     """
     current_frame = inspect.currentframe()
     if current_frame is None:
         return None
-    frame = inspect.getouterframes(current_frame)[depth + 1].frame
+
+    frame = current_frame
+    d = depth + 1
+    while d > 0:
+        frame = frame.f_back
+        if frame is None:
+            raise ValueError("Depth out of range")
+        d -= 1
 
     module_name = (module := inspect.getmodule(frame)) and module.__name__
 
-    plugin: Optional["Plugin"] = None
     # matcher defined when plugin loading
-    if plugin_chain := _current_plugin_chain.get():
-        plugin = plugin_chain[-1]
+    plugin: Optional["Plugin"] = _current_plugin.get()
     # matcher defined when plugin running
-    elif module_name:
+    if plugin is None and module_name:
         plugin = get_plugin_by_module_name(module_name)
 
     return MatcherSource(
-        plugin_name=plugin and plugin.name,
+        plugin_id=plugin and plugin.id_,
         module_name=module_name,
         lineno=frame.f_lineno,
     )
 
 
 def on(
     type: str = "",
     rule: Optional[Union[Rule, T_RuleChecker]] = None,
     permission: Optional[Union[Permission, T_PermissionChecker]] = None,
     *,
-    handlers: Optional[List[Union[T_Handler, Dependent]]] = None,
+    handlers: Optional[list[Union[T_Handler, Dependent]]] = None,
     temp: bool = False,
     expire_time: Optional[Union[datetime, timedelta]] = None,
     priority: int = 1,
     block: bool = False,
     state: Optional[T_State] = None,
     _depth: int = 0,
-) -> Type[Matcher]:
+) -> type[Matcher]:
     """注册一个基础事件响应器，可自定义类型。
 
     参数:
         type: 事件响应器类型
         rule: 事件响应规则
         permission: 事件响应权限
         handlers: 事件处理函数列表
@@ -142,15 +147,15 @@
         source=get_matcher_source(_depth + 1),
         default_state=state,
     )
     store_matcher(matcher)
     return matcher
 
 
-def on_metaevent(*args, _depth: int = 0, **kwargs) -> Type[Matcher]:
+def on_metaevent(*args, _depth: int = 0, **kwargs) -> type[Matcher]:
     """注册一个元事件响应器。
 
     参数:
         rule: 事件响应规则
         permission: 事件响应权限
         handlers: 事件处理函数列表
         temp: 是否为临时事件响应器（仅执行一次）
@@ -158,15 +163,15 @@
         priority: 事件响应器优先级
         block: 是否阻止事件向更低优先级传递
         state: 默认 state
     """
     return on("meta_event", *args, **kwargs, _depth=_depth + 1)
 
 
-def on_message(*args, _depth: int = 0, **kwargs) -> Type[Matcher]:
+def on_message(*args, _depth: int = 0, **kwargs) -> type[Matcher]:
     """注册一个消息事件响应器。
 
     参数:
         rule: 事件响应规则
         permission: 事件响应权限
         handlers: 事件处理函数列表
         temp: 是否为临时事件响应器（仅执行一次）
@@ -175,15 +180,15 @@
         block: 是否阻止事件向更低优先级传递
         state: 默认 state
     """
     kwargs.setdefault("block", True)
     return on("message", *args, **kwargs, _depth=_depth + 1)
 
 
-def on_notice(*args, _depth: int = 0, **kwargs) -> Type[Matcher]:
+def on_notice(*args, _depth: int = 0, **kwargs) -> type[Matcher]:
     """注册一个通知事件响应器。
 
     参数:
         rule: 事件响应规则
         permission: 事件响应权限
         handlers: 事件处理函数列表
         temp: 是否为临时事件响应器（仅执行一次）
@@ -191,15 +196,15 @@
         priority: 事件响应器优先级
         block: 是否阻止事件向更低优先级传递
         state: 默认 state
     """
     return on("notice", *args, **kwargs, _depth=_depth + 1)
 
 
-def on_request(*args, _depth: int = 0, **kwargs) -> Type[Matcher]:
+def on_request(*args, _depth: int = 0, **kwargs) -> type[Matcher]:
     """注册一个请求事件响应器。
 
     参数:
         rule: 事件响应规则
         permission: 事件响应权限
         handlers: 事件处理函数列表
         temp: 是否为临时事件响应器（仅执行一次）
@@ -208,20 +213,20 @@
         block: 是否阻止事件向更低优先级传递
         state: 默认 state
     """
     return on("request", *args, **kwargs, _depth=_depth + 1)
 
 
 def on_startswith(
-    msg: Union[str, Tuple[str, ...]],
+    msg: Union[str, tuple[str, ...]],
     rule: Optional[Union[Rule, T_RuleChecker]] = None,
     ignorecase: bool = False,
     _depth: int = 0,
     **kwargs,
-) -> Type[Matcher]:
+) -> type[Matcher]:
     """注册一个消息事件响应器，并且当消息的**文本部分**以指定内容开头时响应。
 
     参数:
         msg: 指定消息开头内容
         rule: 事件响应规则
         ignorecase: 是否忽略大小写
         permission: 事件响应权限
@@ -232,20 +237,20 @@
         block: 是否阻止事件向更低优先级传递
         state: 默认 state
     """
     return on_message(startswith(msg, ignorecase) & rule, **kwargs, _depth=_depth + 1)
 
 
 def on_endswith(
-    msg: Union[str, Tuple[str, ...]],
+    msg: Union[str, tuple[str, ...]],
     rule: Optional[Union[Rule, T_RuleChecker]] = None,
     ignorecase: bool = False,
     _depth: int = 0,
     **kwargs,
-) -> Type[Matcher]:
+) -> type[Matcher]:
     """注册一个消息事件响应器，并且当消息的**文本部分**以指定内容结尾时响应。
 
     参数:
         msg: 指定消息结尾内容
         rule: 事件响应规则
         ignorecase: 是否忽略大小写
         permission: 事件响应权限
@@ -256,20 +261,20 @@
         block: 是否阻止事件向更低优先级传递
         state: 默认 state
     """
     return on_message(endswith(msg, ignorecase) & rule, **kwargs, _depth=_depth + 1)
 
 
 def on_fullmatch(
-    msg: Union[str, Tuple[str, ...]],
+    msg: Union[str, tuple[str, ...]],
     rule: Optional[Union[Rule, T_RuleChecker]] = None,
     ignorecase: bool = False,
     _depth: int = 0,
     **kwargs,
-) -> Type[Matcher]:
+) -> type[Matcher]:
     """注册一个消息事件响应器，并且当消息的**文本部分**与指定内容完全一致时响应。
 
     参数:
         msg: 指定消息全匹配内容
         rule: 事件响应规则
         ignorecase: 是否忽略大小写
         permission: 事件响应权限
@@ -280,19 +285,19 @@
         block: 是否阻止事件向更低优先级传递
         state: 默认 state
     """
     return on_message(fullmatch(msg, ignorecase) & rule, **kwargs, _depth=_depth + 1)
 
 
 def on_keyword(
-    keywords: Set[str],
+    keywords: set[str],
     rule: Optional[Union[Rule, T_RuleChecker]] = None,
     _depth: int = 0,
     **kwargs,
-) -> Type[Matcher]:
+) -> type[Matcher]:
     """注册一个消息事件响应器，并且当消息纯文本部分包含关键词时响应。
 
     参数:
         keywords: 关键词列表
         rule: 事件响应规则
         permission: 事件响应权限
         handlers: 事件处理函数列表
@@ -302,21 +307,21 @@
         block: 是否阻止事件向更低优先级传递
         state: 默认 state
     """
     return on_message(keyword(*keywords) & rule, **kwargs, _depth=_depth + 1)
 
 
 def on_command(
-    cmd: Union[str, Tuple[str, ...]],
+    cmd: Union[str, tuple[str, ...]],
     rule: Optional[Union[Rule, T_RuleChecker]] = None,
-    aliases: Optional[Set[Union[str, Tuple[str, ...]]]] = None,
+    aliases: Optional[set[Union[str, tuple[str, ...]]]] = None,
     force_whitespace: Optional[Union[str, bool]] = None,
     _depth: int = 0,
     **kwargs,
-) -> Type[Matcher]:
+) -> type[Matcher]:
     """注册一个消息事件响应器，并且当消息以指定命令开头时响应。
 
     命令匹配规则参考: `命令形式匹配 <rule.md#command-command>`_
 
     参数:
         cmd: 指定命令内容
         rule: 事件响应规则
@@ -337,21 +342,21 @@
         command(*commands, force_whitespace=force_whitespace) & rule,
         **kwargs,
         _depth=_depth + 1,
     )
 
 
 def on_shell_command(
-    cmd: Union[str, Tuple[str, ...]],
+    cmd: Union[str, tuple[str, ...]],
     rule: Optional[Union[Rule, T_RuleChecker]] = None,
-    aliases: Optional[Set[Union[str, Tuple[str, ...]]]] = None,
+    aliases: Optional[set[Union[str, tuple[str, ...]]]] = None,
     parser: Optional[ArgumentParser] = None,
     _depth: int = 0,
     **kwargs,
-) -> Type[Matcher]:
+) -> type[Matcher]:
     """注册一个支持 `shell_like` 解析参数的命令消息事件响应器。
 
     与普通的 `on_command` 不同的是，在添加 `parser` 参数时, 响应器会自动处理消息。
 
     可以通过 {ref}`nonebot.params.ShellCommandArgv` 获取原始参数列表，
     通过 {ref}`nonebot.params.ShellCommandArgs` 获取解析后的参数字典。
 
@@ -379,15 +384,15 @@
 
 def on_regex(
     pattern: str,
     flags: Union[int, re.RegexFlag] = 0,
     rule: Optional[Union[Rule, T_RuleChecker]] = None,
     _depth: int = 0,
     **kwargs,
-) -> Type[Matcher]:
+) -> type[Matcher]:
     """注册一个消息事件响应器，并且当消息匹配正则表达式时响应。
 
     命令匹配规则参考: `正则匹配 <rule.md#regex-regex-flags-0>`_
 
     参数:
         pattern: 正则表达式
         flags: 正则匹配标志
@@ -400,20 +405,20 @@
         block: 是否阻止事件向更低优先级传递
         state: 默认 state
     """
     return on_message(regex(pattern, flags) & rule, **kwargs, _depth=_depth + 1)
 
 
 def on_type(
-    types: Union[Type[Event], Tuple[Type[Event], ...]],
+    types: Union[type[Event], tuple[type[Event], ...]],
     rule: Optional[Union[Rule, T_RuleChecker]] = None,
     *,
     _depth: int = 0,
     **kwargs,
-) -> Type[Matcher]:
+) -> type[Matcher]:
     """注册一个事件响应器，并且当事件为指定类型时响应。
 
     参数:
         types: 事件类型
         rule: 事件响应规则
         permission: 事件响应权限
         handlers: 事件处理函数列表
@@ -426,22 +431,22 @@
     event_types = types if isinstance(types, tuple) else (types,)
     return on(rule=is_type(*event_types) & rule, **kwargs, _depth=_depth + 1)
 
 
 class _Group:
     def __init__(self, **kwargs):
         """创建一个事件响应器组合，参数为默认值，与 `on` 一致"""
-        self.matchers: List[Type[Matcher]] = []
+        self.matchers: list[type[Matcher]] = []
         """组内事件响应器列表"""
-        self.base_kwargs: Dict[str, Any] = kwargs
+        self.base_kwargs: dict[str, Any] = kwargs
         """其他传递给 `on` 的参数默认值"""
 
     def _get_final_kwargs(
-        self, update: Dict[str, Any], *, exclude: Optional[Set[str]] = None
-    ) -> Dict[str, Any]:
+        self, update: dict[str, Any], *, exclude: Optional[set[str]] = None
+    ) -> dict[str, Any]:
         """获取最终传递给 `on` 的参数
 
         参数:
             update: 更新的关键字参数
             exclude: 需要排除的参数
         """
         final_kwargs = self.base_kwargs.copy()
@@ -466,26 +471,26 @@
         expire_time: 事件响应器最终有效时间点，过时即被删除
         priority: 事件响应器优先级
         block: 是否阻止事件向更低优先级传递
         state: 默认 state
     """
 
     def __init__(
-        self, cmd: Union[str, Tuple[str, ...]], prefix_aliases: bool = False, **kwargs
+        self, cmd: Union[str, tuple[str, ...]], prefix_aliases: bool = False, **kwargs
     ):
         """命令前缀"""
         super().__init__(**kwargs)
-        self.basecmd: Tuple[str, ...] = (cmd,) if isinstance(cmd, str) else cmd
+        self.basecmd: tuple[str, ...] = (cmd,) if isinstance(cmd, str) else cmd
         self.base_kwargs.pop("aliases", None)
         self.prefix_aliases = prefix_aliases
 
     def __repr__(self) -> str:
         return f"CommandGroup(cmd={self.basecmd}, matchers={len(self.matchers)})"
 
-    def command(self, cmd: Union[str, Tuple[str, ...]], **kwargs) -> Type[Matcher]:
+    def command(self, cmd: Union[str, tuple[str, ...]], **kwargs) -> type[Matcher]:
         """注册一个新的命令。新参数将会覆盖命令组默认值
 
         参数:
             cmd: 指定命令内容
             aliases: 命令别名
             force_whitespace: 是否强制命令后必须有指定空白符
             rule: 事件响应规则
@@ -505,16 +510,16 @@
                 for alias in aliases
             }
         matcher = on_command(cmd, **self._get_final_kwargs(kwargs))
         self.matchers.append(matcher)
         return matcher
 
     def shell_command(
-        self, cmd: Union[str, Tuple[str, ...]], **kwargs
-    ) -> Type[Matcher]:
+        self, cmd: Union[str, tuple[str, ...]], **kwargs
+    ) -> type[Matcher]:
         """注册一个新的 `shell_like` 命令。新参数将会覆盖命令组默认值
 
         参数:
             cmd: 指定命令内容
             rule: 事件响应规则
             aliases: 命令别名
             parser: `nonebot.rule.ArgumentParser` 对象
@@ -540,15 +545,15 @@
 
 class MatcherGroup(_Group):
     """事件响应器组合，统一管理。为 `Matcher` 创建提供默认属性。"""
 
     def __repr__(self) -> str:
         return f"MatcherGroup(matchers={len(self.matchers)})"
 
-    def on(self, **kwargs) -> Type[Matcher]:
+    def on(self, **kwargs) -> type[Matcher]:
         """注册一个基础事件响应器，可自定义类型。
 
         参数:
             type: 事件响应器类型
             rule: 事件响应规则
             permission: 事件响应权限
             handlers: 事件处理函数列表
@@ -558,15 +563,15 @@
             block: 是否阻止事件向更低优先级传递
             state: 默认 state
         """
         matcher = on(**self._get_final_kwargs(kwargs))
         self.matchers.append(matcher)
         return matcher
 
-    def on_metaevent(self, **kwargs) -> Type[Matcher]:
+    def on_metaevent(self, **kwargs) -> type[Matcher]:
         """注册一个元事件响应器。
 
         参数:
             rule: 事件响应规则
             permission: 事件响应权限
             handlers: 事件处理函数列表
             temp: 是否为临时事件响应器（仅执行一次）
@@ -576,15 +581,15 @@
             state: 默认 state
         """
         final_kwargs = self._get_final_kwargs(kwargs, exclude={"type", "permission"})
         matcher = on_metaevent(**final_kwargs)
         self.matchers.append(matcher)
         return matcher
 
-    def on_message(self, **kwargs) -> Type[Matcher]:
+    def on_message(self, **kwargs) -> type[Matcher]:
         """注册一个消息事件响应器。
 
         参数:
             rule: 事件响应规则
             permission: 事件响应权限
             handlers: 事件处理函数列表
             temp: 是否为临时事件响应器（仅执行一次）
@@ -594,15 +599,15 @@
             state: 默认 state
         """
         final_kwargs = self._get_final_kwargs(kwargs, exclude={"type"})
         matcher = on_message(**final_kwargs)
         self.matchers.append(matcher)
         return matcher
 
-    def on_notice(self, **kwargs) -> Type[Matcher]:
+    def on_notice(self, **kwargs) -> type[Matcher]:
         """注册一个通知事件响应器。
 
         参数:
             rule: 事件响应规则
             permission: 事件响应权限
             handlers: 事件处理函数列表
             temp: 是否为临时事件响应器（仅执行一次）
@@ -612,15 +617,15 @@
             state: 默认 state
         """
         final_kwargs = self._get_final_kwargs(kwargs, exclude={"type", "permission"})
         matcher = on_notice(**final_kwargs)
         self.matchers.append(matcher)
         return matcher
 
-    def on_request(self, **kwargs) -> Type[Matcher]:
+    def on_request(self, **kwargs) -> type[Matcher]:
         """注册一个请求事件响应器。
 
         参数:
             rule: 事件响应规则
             permission: 事件响应权限
             handlers: 事件处理函数列表
             temp: 是否为临时事件响应器（仅执行一次）
@@ -631,16 +636,16 @@
         """
         final_kwargs = self._get_final_kwargs(kwargs, exclude={"type", "permission"})
         matcher = on_request(**final_kwargs)
         self.matchers.append(matcher)
         return matcher
 
     def on_startswith(
-        self, msg: Union[str, Tuple[str, ...]], **kwargs
-    ) -> Type[Matcher]:
+        self, msg: Union[str, tuple[str, ...]], **kwargs
+    ) -> type[Matcher]:
         """注册一个消息事件响应器，并且当消息的**文本部分**以指定内容开头时响应。
 
         参数:
             msg: 指定消息开头内容
             ignorecase: 是否忽略大小写
             rule: 事件响应规则
             permission: 事件响应权限
@@ -652,15 +657,15 @@
             state: 默认 state
         """
         final_kwargs = self._get_final_kwargs(kwargs, exclude={"type"})
         matcher = on_startswith(msg, **final_kwargs)
         self.matchers.append(matcher)
         return matcher
 
-    def on_endswith(self, msg: Union[str, Tuple[str, ...]], **kwargs) -> Type[Matcher]:
+    def on_endswith(self, msg: Union[str, tuple[str, ...]], **kwargs) -> type[Matcher]:
         """注册一个消息事件响应器，并且当消息的**文本部分**以指定内容结尾时响应。
 
         参数:
             msg: 指定消息结尾内容
             ignorecase: 是否忽略大小写
             rule: 事件响应规则
             permission: 事件响应权限
@@ -672,15 +677,15 @@
             state: 默认 state
         """
         final_kwargs = self._get_final_kwargs(kwargs, exclude={"type"})
         matcher = on_endswith(msg, **final_kwargs)
         self.matchers.append(matcher)
         return matcher
 
-    def on_fullmatch(self, msg: Union[str, Tuple[str, ...]], **kwargs) -> Type[Matcher]:
+    def on_fullmatch(self, msg: Union[str, tuple[str, ...]], **kwargs) -> type[Matcher]:
         """注册一个消息事件响应器，并且当消息的**文本部分**与指定内容完全一致时响应。
 
         参数:
             msg: 指定消息全匹配内容
             rule: 事件响应规则
             ignorecase: 是否忽略大小写
             permission: 事件响应权限
@@ -692,15 +697,15 @@
             state: 默认 state
         """
         final_kwargs = self._get_final_kwargs(kwargs, exclude={"type"})
         matcher = on_fullmatch(msg, **final_kwargs)
         self.matchers.append(matcher)
         return matcher
 
-    def on_keyword(self, keywords: Set[str], **kwargs) -> Type[Matcher]:
+    def on_keyword(self, keywords: set[str], **kwargs) -> type[Matcher]:
         """注册一个消息事件响应器，并且当消息纯文本部分包含关键词时响应。
 
         参数:
             keywords: 关键词列表
             rule: 事件响应规则
             permission: 事件响应权限
             handlers: 事件处理函数列表
@@ -713,19 +718,19 @@
         final_kwargs = self._get_final_kwargs(kwargs, exclude={"type"})
         matcher = on_keyword(keywords, **final_kwargs)
         self.matchers.append(matcher)
         return matcher
 
     def on_command(
         self,
-        cmd: Union[str, Tuple[str, ...]],
-        aliases: Optional[Set[Union[str, Tuple[str, ...]]]] = None,
+        cmd: Union[str, tuple[str, ...]],
+        aliases: Optional[set[Union[str, tuple[str, ...]]]] = None,
         force_whitespace: Optional[Union[str, bool]] = None,
         **kwargs,
-    ) -> Type[Matcher]:
+    ) -> type[Matcher]:
         """注册一个消息事件响应器，并且当消息以指定命令开头时响应。
 
         命令匹配规则参考: `命令形式匹配 <rule.md#command-command>`_
 
         参数:
             cmd: 指定命令内容
             aliases: 命令别名
@@ -744,19 +749,19 @@
             cmd, aliases=aliases, force_whitespace=force_whitespace, **final_kwargs
         )
         self.matchers.append(matcher)
         return matcher
 
     def on_shell_command(
         self,
-        cmd: Union[str, Tuple[str, ...]],
-        aliases: Optional[Set[Union[str, Tuple[str, ...]]]] = None,
+        cmd: Union[str, tuple[str, ...]],
+        aliases: Optional[set[Union[str, tuple[str, ...]]]] = None,
         parser: Optional[ArgumentParser] = None,
         **kwargs,
-    ) -> Type[Matcher]:
+    ) -> type[Matcher]:
         """注册一个支持 `shell_like` 解析参数的命令消息事件响应器。
 
         与普通的 `on_command` 不同的是，在添加 `parser` 参数时, 响应器会自动处理消息。
 
         可以通过 {ref}`nonebot.params.ShellCommandArgv` 获取原始参数列表，
         通过 {ref}`nonebot.params.ShellCommandArgs` 获取解析后的参数字典。
 
@@ -776,15 +781,15 @@
         final_kwargs = self._get_final_kwargs(kwargs, exclude={"type"})
         matcher = on_shell_command(cmd, aliases=aliases, parser=parser, **final_kwargs)
         self.matchers.append(matcher)
         return matcher
 
     def on_regex(
         self, pattern: str, flags: Union[int, re.RegexFlag] = 0, **kwargs
-    ) -> Type[Matcher]:
+    ) -> type[Matcher]:
         """注册一个消息事件响应器，并且当消息匹配正则表达式时响应。
 
         命令匹配规则参考: `正则匹配 <rule.md#regex-regex-flags-0>`_
 
         参数:
             pattern: 正则表达式
             flags: 正则匹配标志
@@ -799,16 +804,16 @@
         """
         final_kwargs = self._get_final_kwargs(kwargs, exclude={"type"})
         matcher = on_regex(pattern, flags=flags, **final_kwargs)
         self.matchers.append(matcher)
         return matcher
 
     def on_type(
-        self, types: Union[Type[Event], Tuple[Type[Event]]], **kwargs
-    ) -> Type[Matcher]:
+        self, types: Union[type[Event], tuple[type[Event]]], **kwargs
+    ) -> type[Matcher]:
         """注册一个事件响应器，并且当事件为指定类型时响应。
 
         参数:
             types: 事件类型
             rule: 事件响应规则
             permission: 事件响应权限
             handlers: 事件处理函数列表
```

### Comparing `nonebot2-2.2.1/nonebot/plugin/on.pyi` & `nonebot2-2.3.0/nonebot/plugin/on.pyi`

 * *Files identical despite different names*

### Comparing `nonebot2-2.2.1/nonebot/plugins/echo.py` & `nonebot2-2.3.0/nonebot/plugins/echo.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.2.1/nonebot/plugins/single_session.py` & `nonebot2-2.3.0/nonebot/plugins/single_session.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, AsyncGenerator
+from collections.abc import AsyncGenerator
 
 from nonebot.adapters import Event
 from nonebot.params import Depends
 from nonebot.plugin import PluginMetadata
 from nonebot.message import IgnoredException, event_preprocessor
 
 __plugin_meta__ = PluginMetadata(
@@ -11,15 +11,15 @@
     usage="加载插件后自动生效",
     type="application",
     homepage="https://github.com/nonebot/nonebot2/blob/master/nonebot/plugins/single_session.py",
     config=None,
     supported_adapters=None,
 )
 
-_running_matcher: Dict[str, int] = {}
+_running_matcher: dict[str, int] = {}
 
 
 async def matcher_mutex(event: Event) -> AsyncGenerator[bool, None]:
     result = False
     try:
         session_id = event.get_session_id()
     except Exception:
```

### Comparing `nonebot2-2.2.1/nonebot/rule.py` & `nonebot2-2.3.0/nonebot/rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,27 +11,24 @@
 
 import re
 import shlex
 from argparse import Action
 from gettext import gettext
 from argparse import ArgumentError
 from contextvars import ContextVar
+from collections.abc import Sequence
 from itertools import chain, product
 from argparse import Namespace as Namespace
 from argparse import ArgumentParser as ArgParser
 from typing import (
     IO,
     TYPE_CHECKING,
-    List,
-    Type,
-    Tuple,
     Union,
     TypeVar,
     Optional,
-    Sequence,
     TypedDict,
     NamedTuple,
     cast,
     overload,
 )
 
 from pygtrie import CharTrie
@@ -59,24 +56,24 @@
     CMD_WHITESPACE_KEY,
 )
 
 T = TypeVar("T")
 
 
 class CMD_RESULT(TypedDict):
-    command: Optional[Tuple[str, ...]]
+    command: Optional[tuple[str, ...]]
     raw_command: Optional[str]
     command_arg: Optional[Message]
     command_start: Optional[str]
     command_whitespace: Optional[str]
 
 
 class TRIE_VALUE(NamedTuple):
     command_start: str
-    command: Tuple[str, ...]
+    command: tuple[str, ...]
 
 
 parser_message: ContextVar[str] = ContextVar("parser_message")
 
 
 class TrieRule:
     prefix: CharTrie = CharTrie()
@@ -145,15 +142,15 @@
     参数:
         msg: 指定消息开头字符串元组
         ignorecase: 是否忽略大小写
     """
 
     __slots__ = ("msg", "ignorecase")
 
-    def __init__(self, msg: Tuple[str, ...], ignorecase: bool = False):
+    def __init__(self, msg: tuple[str, ...], ignorecase: bool = False):
         self.msg = msg
         self.ignorecase = ignorecase
 
     def __repr__(self) -> str:
         return f"Startswith(msg={self.msg}, ignorecase={self.ignorecase})"
 
     def __eq__(self, other: object) -> bool:
@@ -177,15 +174,15 @@
             re.IGNORECASE if self.ignorecase else 0,
         ):
             state[STARTSWITH_KEY] = match.group()
             return True
         return False
 
 
-def startswith(msg: Union[str, Tuple[str, ...]], ignorecase: bool = False) -> Rule:
+def startswith(msg: Union[str, tuple[str, ...]], ignorecase: bool = False) -> Rule:
     """匹配消息纯文本开头。
 
     参数:
         msg: 指定消息开头字符串元组
         ignorecase: 是否忽略大小写
     """
     if isinstance(msg, str):
@@ -200,15 +197,15 @@
     参数:
         msg: 指定消息结尾字符串元组
         ignorecase: 是否忽略大小写
     """
 
     __slots__ = ("msg", "ignorecase")
 
-    def __init__(self, msg: Tuple[str, ...], ignorecase: bool = False):
+    def __init__(self, msg: tuple[str, ...], ignorecase: bool = False):
         self.msg = msg
         self.ignorecase = ignorecase
 
     def __repr__(self) -> str:
         return f"Endswith(msg={self.msg}, ignorecase={self.ignorecase})"
 
     def __eq__(self, other: object) -> bool:
@@ -232,15 +229,15 @@
             re.IGNORECASE if self.ignorecase else 0,
         ):
             state[ENDSWITH_KEY] = match.group()
             return True
         return False
 
 
-def endswith(msg: Union[str, Tuple[str, ...]], ignorecase: bool = False) -> Rule:
+def endswith(msg: Union[str, tuple[str, ...]], ignorecase: bool = False) -> Rule:
     """匹配消息纯文本结尾。
 
     参数:
         msg: 指定消息开头字符串元组
         ignorecase: 是否忽略大小写
     """
     if isinstance(msg, str):
@@ -255,15 +252,15 @@
     参数:
         msg: 指定消息全匹配字符串元组
         ignorecase: 是否忽略大小写
     """
 
     __slots__ = ("msg", "ignorecase")
 
-    def __init__(self, msg: Tuple[str, ...], ignorecase: bool = False):
+    def __init__(self, msg: tuple[str, ...], ignorecase: bool = False):
         self.msg = tuple(map(str.casefold, msg) if ignorecase else msg)
         self.ignorecase = ignorecase
 
     def __repr__(self) -> str:
         return f"Fullmatch(msg={self.msg}, ignorecase={self.ignorecase})"
 
     def __eq__(self, other: object) -> bool:
@@ -286,15 +283,15 @@
         text = text.casefold() if self.ignorecase else text
         if text in self.msg:
             state[FULLMATCH_KEY] = text
             return True
         return False
 
 
-def fullmatch(msg: Union[str, Tuple[str, ...]], ignorecase: bool = False) -> Rule:
+def fullmatch(msg: Union[str, tuple[str, ...]], ignorecase: bool = False) -> Rule:
     """完全匹配消息。
 
     参数:
         msg: 指定消息全匹配字符串元组
         ignorecase: 是否忽略大小写
     """
     if isinstance(msg, str):
@@ -357,15 +354,15 @@
         force_whitespace: 是否强制命令后必须有指定空白符
     """
 
     __slots__ = ("cmds", "force_whitespace")
 
     def __init__(
         self,
-        cmds: List[Tuple[str, ...]],
+        cmds: list[tuple[str, ...]],
         force_whitespace: Optional[Union[str, bool]] = None,
     ):
         self.cmds = tuple(cmds)
         self.force_whitespace = force_whitespace
 
     def __repr__(self) -> str:
         return f"Command(cmds={self.cmds})"
@@ -376,29 +373,29 @@
         )
 
     def __hash__(self) -> int:
         return hash((frozenset(self.cmds),))
 
     async def __call__(
         self,
-        cmd: Optional[Tuple[str, ...]] = Command(),
+        cmd: Optional[tuple[str, ...]] = Command(),
         cmd_arg: Optional[Message] = CommandArg(),
         cmd_whitespace: Optional[str] = CommandWhitespace(),
     ) -> bool:
         if cmd not in self.cmds:
             return False
         if self.force_whitespace is None or not cmd_arg:
             return True
         if isinstance(self.force_whitespace, str):
             return self.force_whitespace == cmd_whitespace
         return self.force_whitespace == (cmd_whitespace is not None)
 
 
 def command(
-    *cmds: Union[str, Tuple[str, ...]],
+    *cmds: Union[str, tuple[str, ...]],
     force_whitespace: Optional[Union[str, bool]] = None,
 ) -> Rule:
     """匹配消息命令。
 
     根据配置里提供的 {ref}``command_start` <nonebot.config.Config.command_start>`,
     {ref}``command_sep` <nonebot.config.Config.command_sep>` 判断消息是否为命令。
 
@@ -420,15 +417,15 @@
     命令内容与后续消息间无需空格!
     :::
     """
 
     config = get_driver().config
     command_start = config.command_start
     command_sep = config.command_sep
-    commands: List[Tuple[str, ...]] = []
+    commands: list[tuple[str, ...]] = []
     for command in cmds:
         if isinstance(command, str):
             command = (command,)
 
         commands.append(command)
 
         if len(command) == 1:
@@ -456,31 +453,31 @@
     if TYPE_CHECKING:
 
         @overload
         def parse_known_args(
             self,
             args: Optional[Sequence[Union[str, MessageSegment]]] = None,
             namespace: None = None,
-        ) -> Tuple[Namespace, List[Union[str, MessageSegment]]]: ...
+        ) -> tuple[Namespace, list[Union[str, MessageSegment]]]: ...
 
         @overload
         def parse_known_args(
             self, args: Optional[Sequence[Union[str, MessageSegment]]], namespace: T
-        ) -> Tuple[T, List[Union[str, MessageSegment]]]: ...
+        ) -> tuple[T, list[Union[str, MessageSegment]]]: ...
 
         @overload
         def parse_known_args(
             self, *, namespace: T
-        ) -> Tuple[T, List[Union[str, MessageSegment]]]: ...
+        ) -> tuple[T, list[Union[str, MessageSegment]]]: ...
 
-        def parse_known_args(
+        def parse_known_args(  # pyright: ignore[reportIncompatibleMethodOverride]
             self,
             args: Optional[Sequence[Union[str, MessageSegment]]] = None,
             namespace: Optional[T] = None,
-        ) -> Tuple[Union[Namespace, T], List[Union[str, MessageSegment]]]: ...
+        ) -> tuple[Union[Namespace, T], list[Union[str, MessageSegment]]]: ...
 
     @overload
     def parse_args(
         self,
         args: Optional[Sequence[Union[str, MessageSegment]]] = None,
         namespace: None = None,
     ) -> Namespace: ...
@@ -502,15 +499,15 @@
         if argv:
             msg = gettext("unrecognized arguments: %s")
             self.error(msg % " ".join(map(str, argv)))
         return cast(Union[Namespace, T], result)
 
     def _parse_optional(
         self, arg_string: Union[str, MessageSegment]
-    ) -> Optional[Tuple[Optional[Action], str, Optional[str]]]:
+    ) -> Optional[tuple[Optional[Action], str, Optional[str]]]:
         return (
             super()._parse_optional(arg_string) if isinstance(arg_string, str) else None
         )
 
     def _print_message(self, message: str, file: Optional[IO[str]] = None):
         if (msg := parser_message.get(None)) is not None:
             parser_message.set(msg + message)
@@ -529,15 +526,15 @@
     参数:
         cmds: 指定命令元组列表
         parser: 可选参数解析器
     """
 
     __slots__ = ("cmds", "parser")
 
-    def __init__(self, cmds: List[Tuple[str, ...]], parser: Optional[ArgumentParser]):
+    def __init__(self, cmds: list[tuple[str, ...]], parser: Optional[ArgumentParser]):
         self.cmds = tuple(cmds)
         self.parser = parser
 
     def __repr__(self) -> str:
         return f"ShellCommand(cmds={self.cmds}, parser={self.parser})"
 
     def __eq__(self, other: object) -> bool:
@@ -549,15 +546,15 @@
 
     def __hash__(self) -> int:
         return hash((frozenset(self.cmds), self.parser))
 
     async def __call__(
         self,
         state: T_State,
-        cmd: Optional[Tuple[str, ...]] = Command(),
+        cmd: Optional[tuple[str, ...]] = Command(),
         msg: Optional[Message] = CommandArg(),
     ) -> bool:
         if cmd not in self.cmds or msg is None:
             return False
 
         state[SHELL_ARGV] = list(
             chain.from_iterable(
@@ -567,25 +564,25 @@
         )
 
         if self.parser:
             t = parser_message.set("")
             try:
                 args = self.parser.parse_args(state[SHELL_ARGV])
                 state[SHELL_ARGS] = args
-            except ArgumentError as e:  # pragma: py-gte-39
+            except ArgumentError as e:
                 state[SHELL_ARGS] = ParserExit(status=2, message=str(e))
             except ParserExit as e:
                 state[SHELL_ARGS] = e
             finally:
                 parser_message.reset(t)
         return True
 
 
 def shell_command(
-    *cmds: Union[str, Tuple[str, ...]], parser: Optional[ArgumentParser] = None
+    *cmds: Union[str, tuple[str, ...]], parser: Optional[ArgumentParser] = None
 ) -> Rule:
     """匹配 `shell_like` 形式的消息命令。
 
     根据配置里提供的 {ref}``command_start` <nonebot.config.Config.command_start>`,
     {ref}``command_sep` <nonebot.config.Config.command_sep>` 判断消息是否为命令。
 
     可以通过 {ref}`nonebot.params.Command` 获取匹配成功的命令
@@ -625,15 +622,15 @@
     """
     if parser is not None and not isinstance(parser, ArgumentParser):
         raise TypeError("`parser` must be an instance of nonebot.rule.ArgumentParser")
 
     config = get_driver().config
     command_start = config.command_start
     command_sep = config.command_sep
-    commands: List[Tuple[str, ...]] = []
+    commands: list[tuple[str, ...]] = []
     for command in cmds:
         if isinstance(command, str):
             command = (command,)
 
         commands.append(command)
 
         if len(command) == 1:
@@ -736,15 +733,15 @@
 
 
 class IsTypeRule:
     """检查事件类型是否为指定类型。"""
 
     __slots__ = ("types",)
 
-    def __init__(self, *types: Type[Event]):
+    def __init__(self, *types: type[Event]):
         self.types = types
 
     def __repr__(self) -> str:
         return f"IsType(types={tuple(type.__name__ for type in self.types)})"
 
     def __eq__(self, other: object) -> bool:
         return isinstance(other, IsTypeRule) and self.types == other.types
@@ -752,15 +749,15 @@
     def __hash__(self) -> int:
         return hash((self.types,))
 
     async def __call__(self, event: Event) -> bool:
         return isinstance(event, self.types)
 
 
-def is_type(*types: Type[Event]) -> Rule:
+def is_type(*types: type[Event]) -> Rule:
     """匹配事件类型。
 
     参数:
         types: 事件类型
     """
 
     return Rule(IsTypeRule(*types))
```

### Comparing `nonebot2-2.2.1/nonebot/typing.py` & `nonebot2-2.3.0/nonebot/typing.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,75 +41,78 @@
         DeprecationWarning,
     )
     return override
 
 
 if sys.version_info < (3, 10):
 
-    def origin_is_union(origin: t.Optional[t.Type[t.Any]]) -> bool:
+    def type_has_args(type_: type[t.Any]) -> bool:
+        """判断类型是否有参数"""
+        return isinstance(type_, (t._GenericAlias, types.GenericAlias))  # type: ignore
+
+else:
+
+    def type_has_args(type_: type[t.Any]) -> bool:
+        return isinstance(type_, (t._GenericAlias, types.GenericAlias, types.UnionType))  # type: ignore
+
+
+if sys.version_info < (3, 10):
+
+    def origin_is_union(origin: t.Optional[type[t.Any]]) -> bool:
         """判断是否是 Union 类型"""
         return origin is t.Union
 
 else:
 
-    def origin_is_union(origin: t.Optional[t.Type[t.Any]]) -> bool:
+    def origin_is_union(origin: t.Optional[type[t.Any]]) -> bool:
         return origin is t.Union or origin is types.UnionType
 
 
-def origin_is_literal(origin: t.Optional[t.Type[t.Any]]) -> bool:
+def origin_is_literal(origin: t.Optional[type[t.Any]]) -> bool:
     """判断是否是 Literal 类型"""
     return origin is t.Literal or origin is t_ext.Literal
 
 
-def _literal_values(type_: t.Type[t.Any]) -> t.Tuple[t.Any, ...]:
+def _literal_values(type_: type[t.Any]) -> tuple[t.Any, ...]:
     return get_args(type_)
 
 
-def all_literal_values(type_: t.Type[t.Any]) -> t.List[t.Any]:
+def all_literal_values(type_: type[t.Any]) -> list[t.Any]:
     """获取 Literal 类型包含的所有值"""
     if not origin_is_literal(get_origin(type_)):
         return [type_]
 
     return [x for value in _literal_values(type_) for x in all_literal_values(value)]
 
 
-def origin_is_annotated(origin: t.Optional[t.Type[t.Any]]) -> bool:
+def origin_is_annotated(origin: t.Optional[type[t.Any]]) -> bool:
     """判断是否是 Annotated 类型"""
     with contextlib.suppress(TypeError):
         return origin is not None and issubclass(origin, t_ext.Annotated)
     return False
 
 
 NONE_TYPES = {None, type(None), t.Literal[None], t_ext.Literal[None]}
 if sys.version_info >= (3, 10):
     NONE_TYPES.add(types.NoneType)
 
 
-def is_none_type(type_: t.Type[t.Any]) -> bool:
+def is_none_type(type_: type[t.Any]) -> bool:
     """判断是否是 None 类型"""
     return type_ in NONE_TYPES
 
 
-if sys.version_info < (3, 9):  # pragma: py-lt-39
-
-    def evaluate_forwardref(
-        ref: t.ForwardRef, globalns: t.Dict[str, t.Any], localns: t.Dict[str, t.Any]
-    ) -> t.Any:
-        return ref._evaluate(globalns, localns)
-
-else:  # pragma: py-gte-39
-
-    def evaluate_forwardref(
-        ref: t.ForwardRef, globalns: t.Dict[str, t.Any], localns: t.Dict[str, t.Any]
-    ) -> t.Any:
-        return ref._evaluate(globalns, localns, frozenset())
+def evaluate_forwardref(
+    ref: t.ForwardRef, globalns: dict[str, t.Any], localns: dict[str, t.Any]
+) -> t.Any:
+    return ref._evaluate(globalns, localns, frozenset())
 
 
 # state
-T_State: TypeAlias = t.Dict[t.Any, t.Any]
+T_State: TypeAlias = dict[t.Any, t.Any]
 """事件处理状态 State 类型"""
 
 _DependentCallable: TypeAlias = t.Union[
     t.Callable[..., T], t.Callable[..., t.Awaitable[T]]
 ]
 
 # driver hooks
@@ -130,19 +133,19 @@
 - DependParam: 子依赖参数
 - BotParam: Bot 对象
 - DefaultParam: 带有默认值的参数
 """
 
 # api hooks
 T_CallingAPIHook: TypeAlias = t.Callable[
-    ["Bot", str, t.Dict[str, t.Any]], t.Awaitable[t.Any]
+    ["Bot", str, dict[str, t.Any]], t.Awaitable[t.Any]
 ]
 """`bot.call_api` 钩子函数"""
 T_CalledAPIHook: TypeAlias = t.Callable[
-    ["Bot", t.Optional[Exception], str, t.Dict[str, t.Any], t.Any], t.Awaitable[t.Any]
+    ["Bot", t.Optional[Exception], str, dict[str, t.Any], t.Any], t.Awaitable[t.Any]
 ]
 """`bot.call_api` 后执行的函数，参数分别为 bot, exception, api, data, result"""
 
 # event hooks
 T_EventPreProcessor: TypeAlias = _DependentCallable[t.Any]
 """事件预处理函数 EventPreProcessor 类型
 
@@ -240,9 +243,9 @@
 - DependParam: 子依赖参数
 - BotParam: Bot 对象
 - EventParam: Event 对象
 - StateParam: State 对象
 - MatcherParam: Matcher 对象
 - DefaultParam: 带有默认值的参数
 """
-T_DependencyCache: TypeAlias = t.Dict[_DependentCallable[t.Any], "Task[t.Any]"]
+T_DependencyCache: TypeAlias = dict[_DependentCallable[t.Any], "Task[t.Any]"]
 """依赖缓存, 用于存储依赖函数的返回值"""
```

### Comparing `nonebot2-2.2.1/nonebot/utils.py` & `nonebot2-2.3.0/nonebot/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,44 +6,31 @@
 """
 
 import re
 import json
 import asyncio
 import inspect
 import importlib
+import contextlib
 import dataclasses
 from pathlib import Path
 from collections import deque
 from contextvars import copy_context
 from functools import wraps, partial
-from contextlib import asynccontextmanager
+from contextlib import AbstractContextManager, asynccontextmanager
 from typing_extensions import ParamSpec, get_args, override, get_origin
-from typing import (
-    Any,
-    Dict,
-    Type,
-    Tuple,
-    Union,
-    Generic,
-    Mapping,
-    TypeVar,
-    Callable,
-    Optional,
-    Sequence,
-    Coroutine,
-    AsyncGenerator,
-    ContextManager,
-    overload,
-)
+from collections.abc import Mapping, Sequence, Coroutine, AsyncGenerator
+from typing import Any, Union, Generic, TypeVar, Callable, Optional, overload
 
 from pydantic import BaseModel
 
 from nonebot.log import logger
 from nonebot.typing import (
     is_none_type,
+    type_has_args,
     origin_is_union,
     origin_is_literal,
     all_literal_values,
 )
 
 P = ParamSpec("P")
 R = TypeVar("R")
@@ -60,16 +47,16 @@
     参数:
         s: 需要转义的字符串
     """
     return re.sub(r"</?((?:[fb]g\s)?[^<>\s]*)>", r"\\\g<0>", s)
 
 
 def deep_update(
-    mapping: Dict[K, Any], *updating_mappings: Dict[K, Any]
-) -> Dict[K, Any]:
+    mapping: dict[K, Any], *updating_mappings: dict[K, Any]
+) -> dict[K, Any]:
     """深度更新合并字典"""
     updated_mapping = mapping.copy()
     for updating_mapping in updating_mappings:
         for k, v in updating_mapping.items():
             if (
                 k in updated_mapping
                 and isinstance(updated_mapping[k], dict)
@@ -78,78 +65,78 @@
                 updated_mapping[k] = deep_update(updated_mapping[k], v)
             else:
                 updated_mapping[k] = v
     return updated_mapping
 
 
 def lenient_issubclass(
-    cls: Any, class_or_tuple: Union[Type[Any], Tuple[Type[Any], ...]]
+    cls: Any, class_or_tuple: Union[type[Any], tuple[type[Any], ...]]
 ) -> bool:
     """检查 cls 是否是 class_or_tuple 中的一个类型子类并忽略类型错误。"""
     try:
         return isinstance(cls, type) and issubclass(cls, class_or_tuple)
     except TypeError:
         return False
 
 
 def generic_check_issubclass(
-    cls: Any, class_or_tuple: Union[Type[Any], Tuple[Type[Any], ...]]
+    cls: Any, class_or_tuple: Union[type[Any], tuple[type[Any], ...]]
 ) -> bool:
     """检查 cls 是否是 class_or_tuple 中的一个类型子类。
 
     特别的：
 
     - 如果 cls 是 `typing.Union` 或 `types.UnionType` 类型，
       则会检查其中的所有类型是否是 class_or_tuple 中一个类型的子类或 None。
     - 如果 cls 是 `typing.Literal` 类型，
       则会检查其中的所有值是否是 class_or_tuple 中一个类型的实例。
     - 如果 cls 是 `typing.TypeVar` 类型，
       则会检查其 `__bound__` 或 `__constraints__`
       是否是 class_or_tuple 中一个类型的子类或 None。
     """
-    try:
-        return issubclass(cls, class_or_tuple)
-    except TypeError:
-        origin = get_origin(cls)
-        if origin_is_union(origin):
+    if not type_has_args(cls):
+        with contextlib.suppress(TypeError):
+            return issubclass(cls, class_or_tuple)
+
+    origin = get_origin(cls)
+    if origin_is_union(origin):
+        return all(
+            is_none_type(type_) or generic_check_issubclass(type_, class_or_tuple)
+            for type_ in get_args(cls)
+        )
+    elif origin_is_literal(origin):
+        return all(
+            is_none_type(value) or isinstance(value, class_or_tuple)
+            for value in all_literal_values(cls)
+        )
+    # ensure generic List, Dict can be checked
+    elif origin:
+        # avoid class check error (typing.Final, typing.ClassVar, etc...)
+        try:
+            return issubclass(origin, class_or_tuple)
+        except TypeError:
+            return False
+    elif isinstance(cls, TypeVar):
+        if cls.__constraints__:
             return all(
                 is_none_type(type_) or generic_check_issubclass(type_, class_or_tuple)
-                for type_ in get_args(cls)
+                for type_ in cls.__constraints__
             )
-        elif origin_is_literal(origin):
-            return all(
-                is_none_type(value) or isinstance(value, class_or_tuple)
-                for value in all_literal_values(cls)
-            )
-        # ensure generic List, Dict can be checked
-        elif origin:
-            # avoid class check error (typing.Final, typing.ClassVar, etc...)
-            try:
-                return issubclass(origin, class_or_tuple)
-            except TypeError:
-                return False
-        elif isinstance(cls, TypeVar):
-            if cls.__constraints__:
-                return all(
-                    is_none_type(type_)
-                    or generic_check_issubclass(type_, class_or_tuple)
-                    for type_ in cls.__constraints__
-                )
-            elif cls.__bound__:
-                return generic_check_issubclass(cls.__bound__, class_or_tuple)
-        return False
+        elif cls.__bound__:
+            return generic_check_issubclass(cls.__bound__, class_or_tuple)
+    return False
 
 
-def type_is_complex(type_: Type[Any]) -> bool:
+def type_is_complex(type_: type[Any]) -> bool:
     """检查 type_ 是否是复杂类型"""
     origin = get_origin(type_)
     return _type_is_complex_inner(type_) or _type_is_complex_inner(origin)
 
 
-def _type_is_complex_inner(type_: Optional[Type[Any]]) -> bool:
+def _type_is_complex_inner(type_: Optional[type[Any]]) -> bool:
     if lenient_issubclass(type_, (str, bytes)):
         return False
 
     return lenient_issubclass(
         type_, (BaseModel, Mapping, Sequence, tuple, set, frozenset, deque)
     ) or dataclasses.is_dataclass(type_)
 
@@ -196,15 +183,15 @@
         return result
 
     return _wrapper
 
 
 @asynccontextmanager
 async def run_sync_ctx_manager(
-    cm: ContextManager[T],
+    cm: AbstractContextManager[T],
 ) -> AsyncGenerator[T, None]:
     """一个用于包装 sync context manager 为 async context manager 的执行函数"""
     try:
         yield await run_sync(cm.__enter__)()
     except Exception as e:
         ok = await run_sync(cm.__exit__)(type(e), e, None)
         if not ok:
@@ -212,30 +199,30 @@
     else:
         await run_sync(cm.__exit__)(None, None, None)
 
 
 @overload
 async def run_coro_with_catch(
     coro: Coroutine[Any, Any, T],
-    exc: Tuple[Type[Exception], ...],
+    exc: tuple[type[Exception], ...],
     return_on_err: None = None,
 ) -> Union[T, None]: ...
 
 
 @overload
 async def run_coro_with_catch(
     coro: Coroutine[Any, Any, T],
-    exc: Tuple[Type[Exception], ...],
+    exc: tuple[type[Exception], ...],
     return_on_err: R,
 ) -> Union[T, R]: ...
 
 
 async def run_coro_with_catch(
     coro: Coroutine[Any, Any, T],
-    exc: Tuple[Type[Exception], ...],
+    exc: tuple[type[Exception], ...],
     return_on_err: Optional[R] = None,
 ) -> Optional[Union[T, R]]:
     """运行协程并当遇到指定异常时返回指定值。
 
     参数:
         coro: 要运行的协程
         exc: 要捕获的异常
@@ -285,15 +272,15 @@
 
 class classproperty(Generic[T]):
     """类属性装饰器"""
 
     def __init__(self, func: Callable[[Any], T]) -> None:
         self.func = func
 
-    def __get__(self, instance: Any, owner: Optional[Type[Any]] = None) -> T:
+    def __get__(self, instance: Any, owner: Optional[type[Any]] = None) -> T:
         return self.func(type(instance) if owner is None else owner)
 
 
 class DataclassEncoder(json.JSONEncoder):
     """可以序列化 {ref}`nonebot.adapters.Message`(List[Dataclass]) 的 `JSONEncoder`"""
 
     @override
```

### Comparing `nonebot2-2.2.1/pyproject.toml` & `nonebot2-2.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot2"
-version = "2.2.1"
+version = "2.3.0"
 description = "An asynchronous python bot framework."
 authors = ["yanyongyu <yyy@nonebot.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://nonebot.dev/"
 repository = "https://github.com/nonebot/nonebot2"
 documentation = "https://nonebot.dev/"
@@ -21,15 +21,15 @@
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/nonebot/nonebot2/issues"
 "Changelog" = "https://nonebot.dev/changelog"
 "Funding" = "https://afdian.net/@nonebot"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 yarl = "^1.7.2"
 pygtrie = "^2.4.1"
 loguru = ">=0.6.0,<1.0.0"
 python-dotenv = ">=0.21.0,<2.0.0"
 typing-extensions = ">=4.4.0,<5.0.0"
 pydantic = ">=1.10.0,<3.0.0,!=2.5.0,!=2.5.1"
 tomli = { version = "^2.0.1", python = "<3.11" }
@@ -40,15 +40,15 @@
 aiohttp = { version = "^3.9.0b0", extras = ["speedups"], optional = true }
 httpx = { version = ">=0.20.0,<1.0.0", extras = ["http2"], optional = true }
 uvicorn = { version = ">=0.20.0,<1.0.0", extras = [
   "standard",
 ], optional = true }
 
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.2.0"
+ruff = "^0.4.0"
 isort = "^5.10.1"
 black = "^24.0.0"
 nonemoji = "^0.1.2"
 pre-commit = "^3.0.0"
 
 [tool.poetry.group.test.dependencies]
 nonebot-test = { path = "./envs/test/", develop = false }
@@ -62,20 +62,20 @@
 websockets = ["websockets"]
 quart = ["quart", "uvicorn"]
 fastapi = ["fastapi", "uvicorn"]
 all = ["fastapi", "quart", "aiohttp", "httpx", "websockets", "uvicorn"]
 
 [tool.pytest.ini_options]
 asyncio_mode = "strict"
-addopts = "--cov=nonebot --cov-append --cov-report=term-missing"
+addopts = "--cov=nonebot --cov-report=term-missing"
 filterwarnings = ["error", "ignore::DeprecationWarning"]
 
 [tool.black]
 line-length = 88
-target-version = ["py38", "py39", "py310", "py311"]
+target-version = ["py39", "py310", "py311", "py312"]
 include = '\.pyi?$'
 extend-exclude = '''
 '''
 
 [tool.isort]
 profile = "black"
 line_length = 88
@@ -83,35 +83,54 @@
 skip_gitignore = true
 force_sort_within_sections = true
 src_paths = ["nonebot", "tests"]
 extra_standard_library = ["typing_extensions"]
 
 [tool.ruff]
 line-length = 88
-target-version = "py38"
+target-version = "py39"
 
 [tool.ruff.lint]
-select = ["E", "W", "F", "UP", "C", "T", "PYI", "PT", "Q"]
-ignore = ["E402", "C901", "UP037"]
+select = [
+  "F",     # Pyflakes
+  "W",     # pycodestyle warnings
+  "E",     # pycodestyle errors
+  "UP",    # pyupgrade
+  "ASYNC", # flake8-async
+  "C4",    # flake8-comprehensions
+  "T10",   # flake8-debugger
+  "T20",   # flake8-print
+  "PYI",   # flake8-pyi
+  "PT",    # flake8-pytest-style
+  "Q",     # flake8-quotes
+  "RUF",   # Ruff-specific rules
+]
+ignore = [
+  "E402",   # module-import-not-at-top-of-file
+  "UP037",  # quoted-annotation
+  "RUF001", # ambiguous-unicode-character-string
+  "RUF002", # ambiguous-unicode-character-docstring
+  "RUF003", # ambiguous-unicode-character-comment
+]
 
 [tool.ruff.lint.flake8-pytest-style]
 fixture-parentheses = false
 mark-parentheses = false
 
 [tool.pyright]
-pythonVersion = "3.8"
+pythonVersion = "3.9"
 pythonPlatform = "All"
 defineConstant = { PYDANTIC_V2 = true }
 executionEnvironments = [
   { root = "./tests", extraPaths = [
     "./",
   ] },
   { root = "./" },
 ]
 
-typeCheckingMode = "basic"
+typeCheckingMode = "standard"
 reportShadowedImports = false
 disableBytesTypePromotions = true
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot2-2.2.1/PKG-INFO` & `nonebot2-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: nonebot2
-Version: 2.2.1
+Version: 2.3.0
 Summary: An asynchronous python bot framework.
 Home-page: https://nonebot.dev/
 License: MIT
 Keywords: bot,qq,qqbot,mirai,coolq
 Author: yanyongyu
 Author-email: yyy@nonebot.dev
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Robot Framework
 Classifier: Framework :: Robot Framework :: Library
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: aiohttp
 Provides-Extra: all
 Provides-Extra: fastapi
@@ -64,15 +63,15 @@
 <p align="center">
   <a href="https://raw.githubusercontent.com/nonebot/nonebot2/master/LICENSE">
     <img src="https://img.shields.io/github/license/nonebot/nonebot2" alt="license">
   </a>
   <a href="https://pypi.python.org/pypi/nonebot2">
     <img src="https://img.shields.io/pypi/v/nonebot2?logo=python&logoColor=edb641" alt="pypi">
   </a>
-  <img src="https://img.shields.io/badge/python-3.8+-blue?logo=python&logoColor=edb641" alt="python">
+  <img src="https://img.shields.io/badge/python-3.9+-blue?logo=python&logoColor=edb641" alt="python">
   <a href="https://github.com/psf/black">
     <img src="https://img.shields.io/badge/code%20style-black-000000.svg?logo=python&logoColor=edb641" alt="black">
   </a>
   <a href="https://github.com/Microsoft/pyright">
     <img src="https://img.shields.io/badge/types-pyright-797952.svg?logo=python&logoColor=edb641" alt="pyright">
   </a>
   <a href="https://github.com/astral-sh/ruff">
@@ -153,34 +152,36 @@
 
 - 异步优先：基于 Python 的异步特性，即使是~~非常~~大量的消息，也能吞吐自如
 - 易于开发：配合 NB-CLI 脚手架，代码编写上手简单，没有过多的冗余代码，可以让开发者专注于业务逻辑
 - 生而可靠：100% 类型注解覆盖，配合编辑器的类型推导功能，能将绝大多数的 Bug 杜绝在编辑器中 ([编辑器支持](https://nonebot.dev/docs/editor-support))
 - 社区丰富：社区用户众多，直接和间接用户超过十万人，每天都有大量的活跃用户 ([社区资源](#社区资源))
 - 海纳百川：一个框架，支持多个聊天软件平台，可自定义通信协议
 
-  |                                                           协议名称                                                           | 状态 |                                   注释                                    |
-  | :--------------------------------------------------------------------------------------------------------------------------: | :--: | :-----------------------------------------------------------------------: |
-  |                   OneBot（[仓库](https://github.com/nonebot/adapter-onebot)，[协议](https://onebot.dev/)）                   |  ✅  | 支持 QQ、TG、微信公众号、KOOK 等[平台](https://onebot.dev/ecosystem.html) |
-  |         Telegram（[仓库](https://github.com/nonebot/adapter-telegram)，[协议](https://core.telegram.org/bots/api)）          |  ✅  |                                                                           |
-  |        飞书（[仓库](https://github.com/nonebot/adapter-feishu)，[协议](https://open.feishu.cn/document/home/index)）         |  ✅  |                                                                           |
-  |             GitHub（[仓库](https://github.com/nonebot/adapter-github)，[协议](https://docs.github.com/en/apps)）             |  ✅  |                          GitHub APP & OAuth APP                           |
-  |                   QQ（[仓库](https://github.com/nonebot/adapter-qq)，[协议](https://bot.q.qq.com/wiki/)）                    |  ✅  |                            QQ 官方接口调整较多                            |
-  |             钉钉（[仓库](https://github.com/nonebot/adapter-ding)，[协议](https://open.dingtalk.com/document/)）             |  🤗  |                        寻找 Maintainer（暂不可用）                        |
-  |                                Console（[仓库](https://github.com/nonebot/adapter-console)）                                 |  ✅  |                                控制台交互                                 |
-  |        Red （[仓库](https://github.com/nonebot/adapter-red)，[协议](https://chrononeko.github.io/QQNTRedProtocol/)）         |  ✅  |                                  QQ 协议                                  |
-  |               Satori（[仓库](https://github.com/nonebot/adapter-satori)，[协议](https://satori.js.org/zh-CN)）               |  ✅  |               支持 Onebot、TG、飞书、微信公众号、Koishi 等                |
-  |      Discord （[仓库](https://github.com/nonebot/adapter-discord)，[协议](https://discord.com/developers/docs/intro)）       |  ✅  |                             Discord Bot 协议                              |
-  |                  DoDo （[仓库](https://github.com/nonebot/adapter-dodo)，[协议](https://open.imdodo.com/)）                  |  ✅  |                               DoDo Bot 协议                               |
-  |        开黑啦（[仓库](https://github.com/Tian-que/nonebot-adapter-kaiheila)，[协议](https://developer.kookapp.cn/)）         |  ↗️  |                                由社区贡献                                 |
-  |    Mirai（[仓库](https://github.com/ieew/nonebot_adapter_mirai2)，[协议](https://docs.mirai.mamoe.net/mirai-api-http/)）     |  ↗️  |                            QQ 协议，由社区贡献                            |
-  |                              Ntchat（[仓库](https://github.com/JustUndertaker/adapter-ntchat)）                              |  ↗️  |                           微信协议，由社区贡献                            |
-  |                         MineCraft（[仓库](https://github.com/17TheWord/nonebot-adapter-minecraft)）                          |  ↗️  |                                由社区贡献                                 |
-  |                             BiliBili Live（[仓库](https://github.com/wwweww/adapter-bilibili)）                              |  ↗️  |                                由社区贡献                                 |
-  |                          Walle-Q（[仓库](https://github.com/onebot-walle/nonebot_adapter_walleq)）                           |  ↗️  |                            QQ 协议，由社区贡献                            |
-  | Villa（[仓库](https://github.com/CMHopeSunshine/nonebot-adapter-villa)，[协议](https://webstatic.mihoyo.com/vila/bot/doc/)） |  ↗️  |                     米游社大别野 Bot 协议，由社区贡献                     |
+  |                                                       协议名称                                                        | 状态 |                                   注释                                    |
+  | :-------------------------------------------------------------------------------------------------------------------: | :--: | :-----------------------------------------------------------------------: |
+  |               OneBot（[仓库](https://github.com/nonebot/adapter-onebot)，[协议](https://onebot.dev/)）                |  ✅  | 支持 QQ、TG、微信公众号、KOOK 等[平台](https://onebot.dev/ecosystem.html) |
+  |      Telegram（[仓库](https://github.com/nonebot/adapter-telegram)，[协议](https://core.telegram.org/bots/api)）      |  ✅  |                                                                           |
+  |     飞书（[仓库](https://github.com/nonebot/adapter-feishu)，[协议](https://open.feishu.cn/document/home/index)）     |  ✅  |                                                                           |
+  |         GitHub（[仓库](https://github.com/nonebot/adapter-github)，[协议](https://docs.github.com/en/apps)）          |  ✅  |                          GitHub APP & OAuth APP                           |
+  |                QQ（[仓库](https://github.com/nonebot/adapter-qq)，[协议](https://bot.q.qq.com/wiki/)）                |  ✅  |                            QQ 官方接口调整较多                            |
+  |                             Console（[仓库](https://github.com/nonebot/adapter-console)）                             |  ✅  |                                控制台交互                                 |
+  |     Red（[仓库](https://github.com/nonebot/adapter-red)，[协议](https://chrononeko.github.io/QQNTRedProtocol/)）      |  ✅  |                                  QQ 协议                                  |
+  |           Satori（[仓库](https://github.com/nonebot/adapter-satori)，[协议](https://satori.js.org/zh-CN)）            |  ✅  |               支持 Onebot、TG、飞书、微信公众号、Koishi 等                |
+  |   Discord（[仓库](https://github.com/nonebot/adapter-discord)，[协议](https://discord.com/developers/docs/intro)）    |  ✅  |                             Discord Bot 协议                              |
+  |               DoDo（[仓库](https://github.com/nonebot/adapter-dodo)，[协议](https://open.imdodo.com/)）               |  ✅  |                               DoDo Bot 协议                               |
+  |        Kritor（[仓库](https://github.com/nonebot/adapter-kritor)，[协议](https://github.com/KarinJS/kritor)）         |  ✅  |                 Kritor (OnebotX) 协议，QQ 机器人接口标准                  |
+  |         钉钉（[仓库](https://github.com/nonebot/adapter-ding)，[协议](https://open.dingtalk.com/document/)）          |  🤗  |                        寻找 Maintainer（暂不可用）                        |
+  |     开黑啦（[仓库](https://github.com/Tian-que/nonebot-adapter-kaiheila)，[协议](https://developer.kookapp.cn/)）     |  ↗️  |                                由社区贡献                                 |
+  | Mirai（[仓库](https://github.com/ieew/nonebot_adapter_mirai2)，[协议](https://docs.mirai.mamoe.net/mirai-api-http/)） |  ↗️  |                            QQ 协议，由社区贡献                            |
+  |                          Ntchat（[仓库](https://github.com/JustUndertaker/adapter-ntchat)）                           |  ↗️  |                           微信协议，由社区贡献                            |
+  |                      MineCraft（[仓库](https://github.com/17TheWord/nonebot-adapter-minecraft)）                      |  ↗️  |                                由社区贡献                                 |
+  |                          BiliBili Live（[仓库](https://github.com/wwweww/adapter-bilibili)）                          |  ↗️  |                                由社区贡献                                 |
+  |                       Walle-Q（[仓库](https://github.com/onebot-walle/nonebot_adapter_walleq)）                       |  ↗️  |                            QQ 协议，由社区贡献                            |
+  |                       Villa（[仓库](https://github.com/CMHopeSunshine/nonebot-adapter-villa)）                        |  ❌  |                     米游社大别野 Bot 协议，官方已下线                     |
+  | Rocket.Chat（[仓库](https://github.com/IUnlimit/nonebot-adapter-rocketchat)，[协议](https://developer.rocket.chat/)） |  ↗️  |                     Rocket.Chat Bot 协议，由社区贡献                      |
 
 - 坚实后盾：支持多种 web 框架，可自定义替换、组合
 
   |                              驱动框架                               |  类型  |
   | :-----------------------------------------------------------------: | :----: |
   |              [FastAPI](https://fastapi.tiangolo.com/)               | 服务端 |
   | [Quart](https://quart.palletsprojects.com/en/latest/)（异步 Flask） | 服务端 |
```

#### html2text {}

```diff
@@ -1,35 +1,35 @@
-Metadata-Version: 2.1 Name: nonebot2 Version: 2.2.1 Summary: An asynchronous
+Metadata-Version: 2.1 Name: nonebot2 Version: 2.3.0 Summary: An asynchronous
 python bot framework. Home-page: https://nonebot.dev/ License: MIT Keywords:
 bot,qq,qqbot,mirai,coolq Author: yanyongyu Author-email: yyy@nonebot.dev
-Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 5 - Production/
+Requires-Python: >=3.9,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Framework :: Robot Framework Classifier: Framework :: Robot
 Framework :: Library Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.12 Provides-Extra: aiohttp Provides-Extra:
-all Provides-Extra: fastapi Provides-Extra: httpx Provides-Extra: quart
-Provides-Extra: websockets Requires-Dist: Quart (>=0.18.0,<1.0.0) ; extra ==
-"quart" or extra == "all" Requires-Dist: aiohttp[speedups] (>=3.9.0b0,<4.0.0) ;
-extra == "aiohttp" or extra == "all" Requires-Dist: fastapi (>=0.93.0,<1.0.0) ;
-extra == "fastapi" or extra == "all" Requires-Dist: httpx[http2]
-(>=0.20.0,<1.0.0) ; extra == "httpx" or extra == "all" Requires-Dist: loguru
-(>=0.6.0,<1.0.0) Requires-Dist: pydantic (>=1.10.0,<3.0.0,!=2.5.0,!=2.5.1)
-Requires-Dist: pygtrie (>=2.4.1,<3.0.0) Requires-Dist: python-dotenv
-(>=0.21.0,<2.0.0) Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version <
-"3.11" Requires-Dist: typing-extensions (>=4.4.0,<5.0.0) Requires-Dist: uvicorn
-[standard] (>=0.20.0,<1.0.0) ; extra == "quart" or extra == "fastapi" or extra
-== "all" Requires-Dist: websockets (>=10.0) ; extra == "websockets" or extra ==
-"all" Requires-Dist: yarl (>=1.7.2,<2.0.0) Project-URL: Bug Tracker, https://
-github.com/nonebot/nonebot2/issues Project-URL: Changelog, https://nonebot.dev/
-changelog Project-URL: Documentation, https://nonebot.dev/ Project-URL:
-Funding, https://afdian.net/@nonebot Project-URL: Repository, https://
-github.com/nonebot/nonebot2 Description-Content-Type: text/markdown
+:: Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Provides-
+Extra: aiohttp Provides-Extra: all Provides-Extra: fastapi Provides-Extra:
+httpx Provides-Extra: quart Provides-Extra: websockets Requires-Dist: Quart
+(>=0.18.0,<1.0.0) ; extra == "quart" or extra == "all" Requires-Dist: aiohttp
+[speedups] (>=3.9.0b0,<4.0.0) ; extra == "aiohttp" or extra == "all" Requires-
+Dist: fastapi (>=0.93.0,<1.0.0) ; extra == "fastapi" or extra == "all"
+Requires-Dist: httpx[http2] (>=0.20.0,<1.0.0) ; extra == "httpx" or extra ==
+"all" Requires-Dist: loguru (>=0.6.0,<1.0.0) Requires-Dist: pydantic
+(>=1.10.0,<3.0.0,!=2.5.0,!=2.5.1) Requires-Dist: pygtrie (>=2.4.1,<3.0.0)
+Requires-Dist: python-dotenv (>=0.21.0,<2.0.0) Requires-Dist: tomli
+(>=2.0.1,<3.0.0) ; python_version < "3.11" Requires-Dist: typing-extensions
+(>=4.4.0,<5.0.0) Requires-Dist: uvicorn[standard] (>=0.20.0,<1.0.0) ; extra ==
+"quart" or extra == "fastapi" or extra == "all" Requires-Dist: websockets
+(>=10.0) ; extra == "websockets" or extra == "all" Requires-Dist: yarl
+(>=1.7.2,<2.0.0) Project-URL: Bug Tracker, https://github.com/nonebot/nonebot2/
+issues Project-URL: Changelog, https://nonebot.dev/changelog Project-URL:
+Documentation, https://nonebot.dev/ Project-URL: Funding, https://afdian.net/
+@nonebot Project-URL: Repository, https://github.com/nonebot/nonebot2
+Description-Content-Type: text/markdown
                                    _[_n_o_n_e_b_o_t_]
           # NoneBot _â¨ è·¨å¹³å° Python å¼æ­¥æºå¨äººæ¡æ¶ â¨_
                  _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]_[_b_l_a_c_k_]_[_p_y_r_i_g_h_t_]_[_r_u_f_f_]
                   _[_c_o_d_e_c_o_v_]_[_s_i_t_e_]_[_p_r_e_-_c_o_m_m_i_t_]_[_p_y_r_i_g_h_t_]_[_r_u_f_f_]
                 _[_o_n_e_b_o_t_]_[_o_n_e_b_o_t_]_[_Q_Q_]_[_t_e_l_e_g_r_a_m_]_[_f_e_i_s_h_u_]_[_g_i_t_h_u_b_]
 
 _[_Q_Q_ _C_h_a_t_ _G_r_o_u_p_]_[_Q_Q_ _C_h_a_n_n_e_l_]_[_T_e_l_e_g_r_a_m_ _C_h_a_n_n_e_l_]_[_D_i_s_c_o_r_d_ _S_e_r_v_e_r_]
@@ -46,51 +46,55 @@
 ç±»åæ³¨è§£è¦çï¼éåç¼è¾å¨çç±»åæ¨å¯¼åè½ï¼è½å°ç»å¤§å¤æ°ç
 Bug æç»å¨ç¼è¾å¨ä¸­ ([ç¼è¾å¨æ¯æ](https://nonebot.dev/docs/editor-
 support)) -
 ç¤¾åºä¸°å¯ï¼ç¤¾åºç¨æ·ä¼å¤ï¼ç´æ¥åé´æ¥ç¨æ·è¶è¿åä¸äººï¼æ¯å¤©é½æå¤§éçæ´»è·ç¨æ·
 ([ç¤¾åºèµæº](#ç¤¾åºèµæº)) -
 æµ·çº³ç¾å·ï¼ä¸ä¸ªæ¡æ¶ï¼æ¯æå¤ä¸ªèå¤©è½¯ä»¶å¹³å°ï¼å¯èªå®ä¹éä¿¡åè®®
 | åè®®åç§° | ç¶æ | æ³¨é | | :-----------------------------------------
--------------------------------------------------------------------------------
---: | :--: | :-----------------------------------------------------------------
-------: | | OneBotï¼[ä»åº](https://github.com/nonebot/adapter-onebot)ï¼
-[åè®®](https://onebot.dev/)ï¼ | â | æ¯æ
-QQãTGãå¾®ä¿¡å¬ä¼å·ãKOOK ç­[å¹³å°](https://onebot.dev/ecosystem.html)
-| | Telegramï¼[ä»åº](https://github.com/nonebot/adapter-telegram)ï¼[åè®®]
-(https://core.telegram.org/bots/api)ï¼ | â | | | é£ä¹¦ï¼[ä»åº](https://
-github.com/nonebot/adapter-feishu)ï¼[åè®®](https://open.feishu.cn/document/
-home/index)ï¼ | â | | | GitHubï¼[ä»åº](https://github.com/nonebot/
-adapter-github)ï¼[åè®®](https://docs.github.com/en/apps)ï¼ | â | GitHub
-APP & OAuth APP | | QQï¼[ä»åº](https://github.com/nonebot/adapter-qq)ï¼
-[åè®®](https://bot.q.qq.com/wiki/)ï¼ | â | QQ å®æ¹æ¥å£è°æ´è¾å¤ | |
-ééï¼[ä»åº](https://github.com/nonebot/adapter-ding)ï¼[åè®®](https://
-open.dingtalk.com/document/)ï¼ | ð¤ | å¯»æ¾ Maintainerï¼æä¸å¯ç¨ï¼ |
-| Consoleï¼[ä»åº](https://github.com/nonebot/adapter-console)ï¼ | â |
-æ§å¶å°äº¤äº | | Red ï¼[ä»åº](https://github.com/nonebot/adapter-red)ï¼
-[åè®®](https://chrononeko.github.io/QQNTRedProtocol/)ï¼ | â | QQ åè®® |
-| Satoriï¼[ä»åº](https://github.com/nonebot/adapter-satori)ï¼[åè®®]
-(https://satori.js.org/zh-CN)ï¼ | â | æ¯æ
-OnebotãTGãé£ä¹¦ãå¾®ä¿¡å¬ä¼å·ãKoishi ç­ | | Discord ï¼[ä»åº]
+--------------------------------------------------------------------------: | :
+--: | :-----------------------------------------------------------------------:
+| | OneBotï¼[ä»åº](https://github.com/nonebot/adapter-onebot)ï¼[åè®®]
+(https://onebot.dev/)ï¼ | â | æ¯æ QQãTGãå¾®ä¿¡å¬ä¼å·ãKOOK ç­
+[å¹³å°](https://onebot.dev/ecosystem.html) | | Telegramï¼[ä»åº](https://
+github.com/nonebot/adapter-telegram)ï¼[åè®®](https://core.telegram.org/bots/
+api)ï¼ | â | | | é£ä¹¦ï¼[ä»åº](https://github.com/nonebot/adapter-
+feishu)ï¼[åè®®](https://open.feishu.cn/document/home/index)ï¼ | â | | |
+GitHubï¼[ä»åº](https://github.com/nonebot/adapter-github)ï¼[åè®®](https:/
+/docs.github.com/en/apps)ï¼ | â | GitHub APP & OAuth APP | | QQï¼[ä»åº]
+(https://github.com/nonebot/adapter-qq)ï¼[åè®®](https://bot.q.qq.com/wiki/
+)ï¼ | â | QQ å®æ¹æ¥å£è°æ´è¾å¤ | | Consoleï¼[ä»åº](https://
+github.com/nonebot/adapter-console)ï¼ | â | æ§å¶å°äº¤äº | | Redï¼
+[ä»åº](https://github.com/nonebot/adapter-red)ï¼[åè®®](https://
+chrononeko.github.io/QQNTRedProtocol/)ï¼ | â | QQ åè®® | | Satoriï¼
+[ä»åº](https://github.com/nonebot/adapter-satori)ï¼[åè®®](https://
+satori.js.org/zh-CN)ï¼ | â | æ¯æ
+OnebotãTGãé£ä¹¦ãå¾®ä¿¡å¬ä¼å·ãKoishi ç­ | | Discordï¼[ä»åº]
 (https://github.com/nonebot/adapter-discord)ï¼[åè®®](https://discord.com/
-developers/docs/intro)ï¼ | â | Discord Bot åè®® | | DoDo ï¼[ä»åº]
-(https://github.com/nonebot/adapter-dodo)ï¼[åè®®](https://open.imdodo.com/
-)ï¼ | â | DoDo Bot åè®® | | å¼é»å¦ï¼[ä»åº](https://github.com/Tian-
-que/nonebot-adapter-kaiheila)ï¼[åè®®](https://developer.kookapp.cn/)ï¼ |
-âï¸ | ç±ç¤¾åºè´¡ç® | | Miraiï¼[ä»åº](https://github.com/ieew/
-nonebot_adapter_mirai2)ï¼[åè®®](https://docs.mirai.mamoe.net/mirai-api-http/
-)ï¼ | âï¸ | QQ åè®®ï¼ç±ç¤¾åºè´¡ç® | | Ntchatï¼[ä»åº](https://
-github.com/JustUndertaker/adapter-ntchat)ï¼ | âï¸ |
-å¾®ä¿¡åè®®ï¼ç±ç¤¾åºè´¡ç® | | MineCraftï¼[ä»åº](https://github.com/
-17TheWord/nonebot-adapter-minecraft)ï¼ | âï¸ | ç±ç¤¾åºè´¡ç® | | BiliBili
-Liveï¼[ä»åº](https://github.com/wwweww/adapter-bilibili)ï¼ | âï¸ |
-ç±ç¤¾åºè´¡ç® | | Walle-Qï¼[ä»åº](https://github.com/onebot-walle/
-nonebot_adapter_walleq)ï¼ | âï¸ | QQ åè®®ï¼ç±ç¤¾åºè´¡ç® | | Villaï¼
-[ä»åº](https://github.com/CMHopeSunshine/nonebot-adapter-villa)ï¼[åè®®]
-(https://webstatic.mihoyo.com/vila/bot/doc/)ï¼ | âï¸ | ç±³æ¸¸ç¤¾å¤§å«é
-Bot åè®®ï¼ç±ç¤¾åºè´¡ç® | - åå®åç¾ï¼æ¯æå¤ç§ web
+developers/docs/intro)ï¼ | â | Discord Bot åè®® | | DoDoï¼[ä»åº](https:
+//github.com/nonebot/adapter-dodo)ï¼[åè®®](https://open.imdodo.com/)ï¼ |
+â | DoDo Bot åè®® | | Kritorï¼[ä»åº](https://github.com/nonebot/adapter-
+kritor)ï¼[åè®®](https://github.com/KarinJS/kritor)ï¼ | â | Kritor
+(OnebotX) åè®®ï¼QQ æºå¨äººæ¥å£æ å | | ééï¼[ä»åº](https://
+github.com/nonebot/adapter-ding)ï¼[åè®®](https://open.dingtalk.com/document/
+)ï¼ | ð¤ | å¯»æ¾ Maintainerï¼æä¸å¯ç¨ï¼ | | å¼é»å¦ï¼[ä»åº]
+(https://github.com/Tian-que/nonebot-adapter-kaiheila)ï¼[åè®®](https://
+developer.kookapp.cn/)ï¼ | âï¸ | ç±ç¤¾åºè´¡ç® | | Miraiï¼[ä»åº]
+(https://github.com/ieew/nonebot_adapter_mirai2)ï¼[åè®®](https://
+docs.mirai.mamoe.net/mirai-api-http/)ï¼ | âï¸ | QQ åè®®ï¼ç±ç¤¾åºè´¡ç®
+| | Ntchatï¼[ä»åº](https://github.com/JustUndertaker/adapter-ntchat)ï¼ |
+âï¸ | å¾®ä¿¡åè®®ï¼ç±ç¤¾åºè´¡ç® | | MineCraftï¼[ä»åº](https://
+github.com/17TheWord/nonebot-adapter-minecraft)ï¼ | âï¸ | ç±ç¤¾åºè´¡ç® |
+| BiliBili Liveï¼[ä»åº](https://github.com/wwweww/adapter-bilibili)ï¼ |
+âï¸ | ç±ç¤¾åºè´¡ç® | | Walle-Qï¼[ä»åº](https://github.com/onebot-
+walle/nonebot_adapter_walleq)ï¼ | âï¸ | QQ åè®®ï¼ç±ç¤¾åºè´¡ç® | |
+Villaï¼[ä»åº](https://github.com/CMHopeSunshine/nonebot-adapter-villa)ï¼ |
+â | ç±³æ¸¸ç¤¾å¤§å«é Bot åè®®ï¼å®æ¹å·²ä¸çº¿ | | Rocket.Chatï¼
+[ä»åº](https://github.com/IUnlimit/nonebot-adapter-rocketchat)ï¼[åè®®]
+(https://developer.rocket.chat/)ï¼ | âï¸ | Rocket.Chat Bot
+åè®®ï¼ç±ç¤¾åºè´¡ç® | - åå®åç¾ï¼æ¯æå¤ç§ web
 æ¡æ¶ï¼å¯èªå®ä¹æ¿æ¢ãç»å | é©±å¨æ¡æ¶ | ç±»å | | :-------------
 ----------------------------------------------------: | :----: | | [FastAPI]
 (https://fastapi.tiangolo.com/) | æå¡ç«¯ | | [Quart](https://
 quart.palletsprojects.com/en/latest/)ï¼å¼æ­¥ Flaskï¼ | æå¡ç«¯ | |
 [aiohttp](https://docs.aiohttp.org/en/stable/) | å®¢æ·ç«¯ | | [httpx](https://
 www.python-httpx.org/) | å®¢æ·ç«¯ | | [websockets](https://
 websockets.readthedocs.io/en/stable/) | å®¢æ·ç«¯ | æ´å¤ï¼[æ¦è§](https://
```

