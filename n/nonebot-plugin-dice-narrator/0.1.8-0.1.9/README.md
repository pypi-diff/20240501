# Comparing `tmp/nonebot_plugin_dice_narrator-0.1.8.tar.gz` & `tmp/nonebot_plugin_dice_narrator-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_dice_narrator-0.1.8.tar", max compression
+gzip compressed data, was "nonebot_plugin_dice_narrator-0.1.9.tar", max compression
```

## Comparing `nonebot_plugin_dice_narrator-0.1.8.tar` & `nonebot_plugin_dice_narrator-0.1.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2024-03-13 01:27:25.475950 nonebot_plugin_dice_narrator-0.1.8/LICENSE
--rw-r--r--   0        0        0     2485 2024-03-13 01:27:25.475950 nonebot_plugin_dice_narrator-0.1.8/README.md
--rw-r--r--   0        0        0      621 2024-03-13 01:27:25.475950 nonebot_plugin_dice_narrator-0.1.8/nonebot_plugin_dice_narrator/__init__.py
--rw-r--r--   0        0        0      629 2024-03-13 01:27:25.475950 nonebot_plugin_dice_narrator-0.1.8/nonebot_plugin_dice_narrator/config.py
--rw-r--r--   0        0        0     1425 2024-03-13 01:27:25.479950 nonebot_plugin_dice_narrator-0.1.8/nonebot_plugin_dice_narrator/matchers.py
--rw-r--r--   0        0        0     4095 2024-03-13 01:27:25.479950 nonebot_plugin_dice_narrator-0.1.8/nonebot_plugin_dice_narrator/narrator.py
--rw-r--r--   0        0        0      289 2024-03-13 01:27:25.479950 nonebot_plugin_dice_narrator-0.1.8/nonebot_plugin_dice_narrator/utils/common.py
--rw-r--r--   0        0        0     2034 2024-03-13 01:27:25.479950 nonebot_plugin_dice_narrator-0.1.8/nonebot_plugin_dice_narrator/utils/message_parse.py
--rw-r--r--   0        0        0     3640 2024-03-13 01:27:25.479950 nonebot_plugin_dice_narrator-0.1.8/nonebot_plugin_dice_narrator/utils/openai_funcs.py
--rw-r--r--   0        0        0     1542 2024-03-13 01:27:25.479950 nonebot_plugin_dice_narrator-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3295 1970-01-01 00:00:00.000000 nonebot_plugin_dice_narrator-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-03-14 02:23:19.768527 nonebot_plugin_dice_narrator-0.1.9/LICENSE
+-rw-r--r--   0        0        0     3111 2024-03-14 02:23:19.768527 nonebot_plugin_dice_narrator-0.1.9/README.md
+-rw-r--r--   0        0        0      777 2024-03-14 02:23:19.768527 nonebot_plugin_dice_narrator-0.1.9/nonebot_plugin_dice_narrator/__init__.py
+-rw-r--r--   0        0        0      629 2024-03-14 02:23:19.768527 nonebot_plugin_dice_narrator-0.1.9/nonebot_plugin_dice_narrator/config.py
+-rw-r--r--   0        0        0     1425 2024-03-14 02:23:19.768527 nonebot_plugin_dice_narrator-0.1.9/nonebot_plugin_dice_narrator/matchers.py
+-rw-r--r--   0        0        0     5027 2024-03-14 02:23:19.768527 nonebot_plugin_dice_narrator-0.1.9/nonebot_plugin_dice_narrator/narrator.py
+-rw-r--r--   0        0        0      289 2024-03-14 02:23:19.768527 nonebot_plugin_dice_narrator-0.1.9/nonebot_plugin_dice_narrator/utils/common.py
+-rw-r--r--   0        0        0     2034 2024-03-14 02:23:19.768527 nonebot_plugin_dice_narrator-0.1.9/nonebot_plugin_dice_narrator/utils/message_parse.py
+-rw-r--r--   0        0        0     3640 2024-03-14 02:23:19.768527 nonebot_plugin_dice_narrator-0.1.9/nonebot_plugin_dice_narrator/utils/openai_funcs.py
+-rw-r--r--   0        0        0     1563 2024-03-14 02:23:19.772527 nonebot_plugin_dice_narrator-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3921 1970-01-01 00:00:00.000000 nonebot_plugin_dice_narrator-0.1.9/PKG-INFO
```

### Comparing `nonebot_plugin_dice_narrator-0.1.8/LICENSE` & `nonebot_plugin_dice_narrator-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dice_narrator-0.1.8/README.md` & `nonebot_plugin_dice_narrator-0.1.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,31 @@
 
 ## 安装
 
 ```bash
 nb plugin install nonebot-plugin-dice-narrator
 ```
 
+## 配置
+
+插件配置文件路径: `./configs/nonebot_plugin_dice_narrator/config.dev.yaml` (启动一次服务后生成)，请根据以下配置文件修改配置。
+
+```yaml
+OPENAI_API_KEYS:  # OpenAI API Key (可填多个*必须)
+- sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxx
+- sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxx
+- sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxx
+OPENAI_BASE_URL: https://api.openai.com/v1  # OpenAI API Base URL 
+CHAT_MODEL: gpt-3.5-turbo # 使用的 Chat Model
+FORBIDDEN_USERS:  # 禁止交互的用户列表
+- 123456
+DIFFICULTY_DICE_MAX: 20 # 检定难度最大值 (即骰子面数)
+OPENAI_PROXY: null  # OpenAI 使用的代理
+```
+
 ## 使用
 
 向 Bot 发送 `检定 任务描述` (需要指令前缀)，Bot 会根据其描述指定一个检定难度，并给出结果。
 
 例如:
 
 ![alt text](docs/images/example.png)
```

#### html2text {}

```diff
@@ -1,16 +1,26 @@
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
                      â¨ ä¸åªå¯ç±ç AI æ·éª°å§¬! â¨
  ð¬ ææ¯äº¤æµ/ç­ç/è®¨è®º -> ï¼_å__ _å__¥_æ___ä_»_¶_ä_º_¤_æ_µ__ç_¾_¤_-_6_3_6_9_2_5_1_5_3 ð¨ï¸
                             _[_p_y_p_i_][python]_[_p_y_t_h_o_n_]
 # Dice Narrator ## å·²å®ç°åè½åè¡¨ - åºç¡æ£å®: [Command: æ£å®]
 å¦æä½ æå¥½çæ³æ³ï¼æ¬¢è¿æåº issue æè PRã ## å®è£ ```bash nb
-plugin install nonebot-plugin-dice-narrator ``` ## ä½¿ç¨ å Bot åé
-`æ£å® ä»»å¡æè¿°` (éè¦æä»¤åç¼)ï¼Bot
+plugin install nonebot-plugin-dice-narrator ``` ## éç½®
+æä»¶éç½®æä»¶è·¯å¾: `./configs/nonebot_plugin_dice_narrator/
+config.dev.yaml`
+(å¯å¨ä¸æ¬¡æå¡åçæ)ï¼è¯·æ ¹æ®ä»¥ä¸éç½®æä»¶ä¿®æ¹éç½®ã
+```yaml OPENAI_API_KEYS: # OpenAI API Key (å¯å¡«å¤ä¸ª*å¿é¡») - sk-
+xxxxxxxxxxxxxxxxxxxxxxxxxxxx - sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxx - sk-
+xxxxxxxxxxxxxxxxxxxxxxxxxxxx OPENAI_BASE_URL: https://api.openai.com/v1 #
+OpenAI API Base URL CHAT_MODEL: gpt-3.5-turbo # ä½¿ç¨ç Chat Model
+FORBIDDEN_USERS: # ç¦æ­¢äº¤äºçç¨æ·åè¡¨ - 123456 DIFFICULTY_DICE_MAX: 20
+# æ£å®é¾åº¦æå¤§å¼ (å³éª°å­é¢æ°) OPENAI_PROXY: null # OpenAI
+ä½¿ç¨çä»£ç ``` ## ä½¿ç¨ å Bot åé `æ£å® ä»»å¡æè¿°`
+(éè¦æä»¤åç¼)ï¼Bot
 ä¼æ ¹æ®å¶æè¿°æå®ä¸ä¸ªæ£å®é¾åº¦ï¼å¹¶ç»åºç»æã ä¾å¦: ![alt
 text](docs/images/example.png) > æ³¨æ:
 ä½ å¯ä»¥æ£å®ä»»æåå®¹çææ¬ï¼ä½ä¸æ¯ææææ¬é½è½å¾å°è¯å¥½çåé¦ï¼å»ºè®®åå®¹ææ¬ä¸ºä¸æ®µå¯æ§è¡çä»»å¡ï¼åæ¶å¯ä»¥éä¸ä¸äºç®è¦çä»»å¡èæ¯æ¦åµï¼é¿åä½¿ç¨çé®å¥ãæ æä¹ç­å¥ç­æä¹ä¸æçè¯­å¥ã
 ## å¼åæå å¦æä½ æ³ä¸º Dice Narrator
 è´¡ç®ä»£ç ï¼å¯ä»¥åèä»¥ä¸æ­¥éª¤ï¼ ### 0. æäº¤ issue
 å¦æä½ å¸æä½ çä»£ç è¢«åå¹¶å°ä¸»åæ¯åå¸ï¼è¯·åæäº¤ issue
 è¯´æä½ çæ³æ³ï¼é¿åéå¤å³å¨æåè½å²çªã ### 1. åéä»£ç  >
```

### Comparing `nonebot_plugin_dice_narrator-0.1.8/nonebot_plugin_dice_narrator/config.py` & `nonebot_plugin_dice_narrator-0.1.9/nonebot_plugin_dice_narrator/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dice_narrator-0.1.8/nonebot_plugin_dice_narrator/matchers.py` & `nonebot_plugin_dice_narrator-0.1.9/nonebot_plugin_dice_narrator/matchers.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dice_narrator-0.1.8/nonebot_plugin_dice_narrator/narrator.py` & `nonebot_plugin_dice_narrator-0.1.9/nonebot_plugin_dice_narrator/narrator.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,48 +5,49 @@
 from nonebot.matcher import Matcher
 
 from nonebot_plugin_dice_narrator.config import config
 from nonebot_plugin_dice_narrator.utils.common import read_yml_str2data
 from nonebot_plugin_dice_narrator.utils.openai_funcs import gen_chat_response_text
 
 SYSTEM_PROMPT = f"""
-你是一个游戏DM，接下来用户会向你描述一项玩家任务，并进行一次掷骰，请根据你的对这个任务的判断，给出对于这个任务**相对客观**的执行难度(1~{config.DIFFICULTY_DICE_MAX})，需要说明具体的**玩家行为描述**、四种掷骰结果对应的**事件描述**:
+你是一个游戏DM，接下来用户会向你描述一项玩家任务，并进行一次掷骰，请根据你的对这个任务的判断，给出对于这个任务**相对客观**的执行难度(1~{config.DIFFICULTY_DICE_MAX})，需要尽可能详细地说明具体的四种掷骰结果对应的**事件描述**:
 
-大成功(completed_success): 掷骰结果为{config.DIFFICULTY_DICE_MAX}
 成功(success): 掷骰结果不小于任务难度
 失败(failure): 掷骰结果小于任务难度
-大失败(critical_failure): 掷骰结果为1
+大成功(completed_success): 掷骰结果为{config.DIFFICULTY_DICE_MAX}
+大失败(critical_failure): 掷骰结果为1且小于任务难度
 
 示例如下: 
 
 检定任务: 
 逃离触手怪的束缚
 
 你的响应内容格式如下:
 
 ```yaml
 difficulty: {int(config.DIFFICULTY_DICE_MAX*0.75)}
-completed_success: 你展现出了惊人的技巧和勇气。巧妙地躲过了触手怪的攻击，找到了一个隐藏的通道，成功逃离了触手怪的魔爪。你喘着粗气，但胜利的喜悦填满了你的心。
 success: 你奋力抵挡住了触手怪的袭击，成功拉开了距离。虽然你没有完全逃脱，但至少还活着，可以继续寻找其他出路。
 failure: 在昏暗的洞穴中，触手怪的柔滑触手紧紧缠绕着你的身体。你感到了一种异样的窒息与兴奋交织在一起，而队友们只能眼睁睁地看着。任务虽然失败了，但你似乎成为了怪物欲望的俘虏。
-critical_failure: 你不慎触动了隐藏的机关，引来了触手怪贪婪的目光。它那强有力的触手将你高高举起，在空中展示你无助的姿态后猛地摔向地面。在那一瞬间，意识模糊之际，你感到自己被未知快感淹没。
+completed_success: 你在在昏暗潮湿的洞穴里，紧张地寻找着逃生的路线。触手怪似乎已经察觉到你的气息，在不远处窥视着。你小心翼翼地移动着，每一步都如履薄冰。终于，在一个转角处，你发现了一条隐蔽的小径。没有时间犹豫，你快速地沿着小径前进，只听见身后触手怪愤怒的咆哮声渐行渐远。当你走出洞穴，深深地吸了口新鲜空气时，心中充满了胜利的喜悦和对自由的向往。
+critical_failure: 在昏暗的洞穴中，触手怪的柔滑触手已经缠绕住了你的双腿和手臂。你努力挣扎着想要逃脱，但它们就像有生命一样紧紧地束缚着你，阻止你任何逃跑的可能。队友们似乎被其他事情分散了注意力，没有人能来救你。就在这时，触手开始轻轻地摩擦起你的皮肤，你感到自己被未知快感淹没。
 ```
 
+如果玩家给出的任务是一个**行为**，"成功"的定义是该行为能否完成以及完成的效果如何；如果是**事件**，"成功"的定义是**该事件发生**了，以及事件发生的影响，并且其发生的概率影响对该事件难度的定义。(即如果该事件越难发生，你应该设置越高的难度，并且在其**success**和**completed_success**中描述发生的影响)
 特别地，如果玩家给出的任务描述不明确，你可以适当地任意假设其发生的背景
 """
 
 USER_PROMPT = """
 检定任务:
 {question}
 """
 
 RESPONSE_STRUCT = """
 检定任务: {question}
 目标难度: {difficulty}/{difficulty_max}
-检定结果: {dice_num} [{status}]
+掷骰结果: {dice_num} [{status}]
 ========
 {event_content}
 """
 
 
 async def run_narrator(question: str, matcher: Matcher):
     assert question, "question is empty"
@@ -74,27 +75,28 @@
     except Exception:
         res_data = read_yml_str2data(content + "```")
 
     # 掷骰
     dice_num = random.randint(1, config.DIFFICULTY_DICE_MAX)
     if dice_num == config.DIFFICULTY_DICE_MAX:
         res_key, status = "completed_success", "大成功"
-    elif dice_num == 1:
+    elif dice_num == 1 and dice_num < int(res_data["difficulty"]):
         res_key, status = "critical_failure", "大失败"
     elif dice_num < int(res_data["difficulty"]):
         res_key, status = "failure", "失败"
     else:
         res_key, status = "success", "成功"
 
     logger.debug(f"检定: `{question}` | 原始返回: {res}")
 
     try:
         await matcher.finish(
             RESPONSE_STRUCT.strip().format(
                 question=question,
+                # thought=res_data["thought"],
                 difficulty=int(res_data["difficulty"]),
                 difficulty_max=config.DIFFICULTY_DICE_MAX,
                 dice_num=dice_num,
                 event_content=res_data[res_key],
                 status=status,
             ),
         )
```

### Comparing `nonebot_plugin_dice_narrator-0.1.8/nonebot_plugin_dice_narrator/utils/message_parse.py` & `nonebot_plugin_dice_narrator-0.1.9/nonebot_plugin_dice_narrator/utils/message_parse.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dice_narrator-0.1.8/nonebot_plugin_dice_narrator/utils/openai_funcs.py` & `nonebot_plugin_dice_narrator-0.1.9/nonebot_plugin_dice_narrator/utils/openai_funcs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dice_narrator-0.1.8/pyproject.toml` & `nonebot_plugin_dice_narrator-0.1.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tool.poetry]
 name = "nonebot-plugin-dice-narrator"
-version = "0.1.8"
+version = "0.1.9"
 description = "一只可爱的AI掷骰姬"
 authors = ["KroMiose <li_xiangff@163.com>"]
 readme = "README.md"
 packages = [{ include = "nonebot_plugin_dice_narrator" }]
 repository = "https://github.com/KroMiose/nonebot-plugin-dice-narrator"
 
 [tool.poetry.scripts]
 publish = "tools.run_publish:main"
+bot = "run_bot:main"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 nonebot-adapter-onebot = "^2.4.2"
 miose-toolkit-common = "^0.2.0"
 nonebot2 = { extras = ["fastapi"], version = "^2.2.1" }
 httpx = "^0.27.0"
```

### Comparing `nonebot_plugin_dice_narrator-0.1.8/PKG-INFO` & `nonebot_plugin_dice_narrator-0.1.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-dice-narrator
-Version: 0.1.8
+Version: 0.1.9
 Summary: 一只可爱的AI掷骰姬
 Home-page: https://github.com/KroMiose/nonebot-plugin-dice-narrator
 Author: KroMiose
 Author-email: li_xiangff@163.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -46,14 +46,31 @@
 
 ## 安装
 
 ```bash
 nb plugin install nonebot-plugin-dice-narrator
 ```
 
+## 配置
+
+插件配置文件路径: `./configs/nonebot_plugin_dice_narrator/config.dev.yaml` (启动一次服务后生成)，请根据以下配置文件修改配置。
+
+```yaml
+OPENAI_API_KEYS:  # OpenAI API Key (可填多个*必须)
+- sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxx
+- sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxx
+- sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxx
+OPENAI_BASE_URL: https://api.openai.com/v1  # OpenAI API Base URL 
+CHAT_MODEL: gpt-3.5-turbo # 使用的 Chat Model
+FORBIDDEN_USERS:  # 禁止交互的用户列表
+- 123456
+DIFFICULTY_DICE_MAX: 20 # 检定难度最大值 (即骰子面数)
+OPENAI_PROXY: null  # OpenAI 使用的代理
+```
+
 ## 使用
 
 向 Bot 发送 `检定 任务描述` (需要指令前缀)，Bot 会根据其描述指定一个检定难度，并给出结果。
 
 例如:
 
 ![alt text](docs/images/example.png)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-dice-narrator Version: 0.1.8
+Metadata-Version: 2.1 Name: nonebot-plugin-dice-narrator Version: 0.1.9
 Summary: ä¸åªå¯ç±çAIæ·éª°å§¬ Home-page: https://github.com/KroMiose/
 nonebot-plugin-dice-narrator Author: KroMiose Author-email: li_xiangff@163.com
 Requires-Python: >=3.9,<3.12 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.27.0,<0.28.0) Requires-Dist: miose-toolkit-common
 (>=0.2.0,<0.3.0) Requires-Dist: nonebot-adapter-onebot (>=2.4.2,<3.0.0)
@@ -12,16 +12,26 @@
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
                      â¨ ä¸åªå¯ç±ç AI æ·éª°å§¬! â¨
  ð¬ ææ¯äº¤æµ/ç­ç/è®¨è®º -> ï¼_å__ _å__¥_æ___ä_»_¶_ä_º_¤_æ_µ__ç_¾_¤_-_6_3_6_9_2_5_1_5_3 ð¨ï¸
                             _[_p_y_p_i_][python]_[_p_y_t_h_o_n_]
 # Dice Narrator ## å·²å®ç°åè½åè¡¨ - åºç¡æ£å®: [Command: æ£å®]
 å¦æä½ æå¥½çæ³æ³ï¼æ¬¢è¿æåº issue æè PRã ## å®è£ ```bash nb
-plugin install nonebot-plugin-dice-narrator ``` ## ä½¿ç¨ å Bot åé
-`æ£å® ä»»å¡æè¿°` (éè¦æä»¤åç¼)ï¼Bot
+plugin install nonebot-plugin-dice-narrator ``` ## éç½®
+æä»¶éç½®æä»¶è·¯å¾: `./configs/nonebot_plugin_dice_narrator/
+config.dev.yaml`
+(å¯å¨ä¸æ¬¡æå¡åçæ)ï¼è¯·æ ¹æ®ä»¥ä¸éç½®æä»¶ä¿®æ¹éç½®ã
+```yaml OPENAI_API_KEYS: # OpenAI API Key (å¯å¡«å¤ä¸ª*å¿é¡») - sk-
+xxxxxxxxxxxxxxxxxxxxxxxxxxxx - sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxx - sk-
+xxxxxxxxxxxxxxxxxxxxxxxxxxxx OPENAI_BASE_URL: https://api.openai.com/v1 #
+OpenAI API Base URL CHAT_MODEL: gpt-3.5-turbo # ä½¿ç¨ç Chat Model
+FORBIDDEN_USERS: # ç¦æ­¢äº¤äºçç¨æ·åè¡¨ - 123456 DIFFICULTY_DICE_MAX: 20
+# æ£å®é¾åº¦æå¤§å¼ (å³éª°å­é¢æ°) OPENAI_PROXY: null # OpenAI
+ä½¿ç¨çä»£ç ``` ## ä½¿ç¨ å Bot åé `æ£å® ä»»å¡æè¿°`
+(éè¦æä»¤åç¼)ï¼Bot
 ä¼æ ¹æ®å¶æè¿°æå®ä¸ä¸ªæ£å®é¾åº¦ï¼å¹¶ç»åºç»æã ä¾å¦: ![alt
 text](docs/images/example.png) > æ³¨æ:
 ä½ å¯ä»¥æ£å®ä»»æåå®¹çææ¬ï¼ä½ä¸æ¯ææææ¬é½è½å¾å°è¯å¥½çåé¦ï¼å»ºè®®åå®¹ææ¬ä¸ºä¸æ®µå¯æ§è¡çä»»å¡ï¼åæ¶å¯ä»¥éä¸ä¸äºç®è¦çä»»å¡èæ¯æ¦åµï¼é¿åä½¿ç¨çé®å¥ãæ æä¹ç­å¥ç­æä¹ä¸æçè¯­å¥ã
 ## å¼åæå å¦æä½ æ³ä¸º Dice Narrator
 è´¡ç®ä»£ç ï¼å¯ä»¥åèä»¥ä¸æ­¥éª¤ï¼ ### 0. æäº¤ issue
 å¦æä½ å¸æä½ çä»£ç è¢«åå¹¶å°ä¸»åæ¯åå¸ï¼è¯·åæäº¤ issue
 è¯´æä½ çæ³æ³ï¼é¿åéå¤å³å¨æåè½å²çªã ### 1. åéä»£ç  >
```

