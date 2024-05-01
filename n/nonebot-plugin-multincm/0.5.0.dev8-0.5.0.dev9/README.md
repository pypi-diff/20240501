# Comparing `tmp/nonebot_plugin_multincm-0.5.0.dev8.tar.gz` & `tmp/nonebot_plugin_multincm-0.5.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_multincm-0.5.0.dev8.tar", last modified: Sun Mar  3 03:21:55 2024, max compression
+gzip compressed data, was "nonebot_plugin_multincm-0.5.0.dev9.tar", last modified: Sun Mar 10 08:42:08 2024, max compression
```

## Comparing `nonebot_plugin_multincm-0.5.0.dev8.tar` & `nonebot_plugin_multincm-0.5.0.dev9.tar`

### file list

```diff
@@ -1,25 +1,23 @@
--rw-r--r--   0        0        0     1069 2024-03-03 03:21:43.456631 nonebot_plugin_multincm-0.5.0.dev8/LICENSE
--rw-r--r--   0        0        0    13266 2024-03-03 03:21:43.456631 nonebot_plugin_multincm-0.5.0.dev8/README.md
--rw-r--r--   0        0        0     2446 2024-03-03 03:21:43.456631 nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/__init__.py
--rw-r--r--   0        0        0    18307 2024-03-03 03:21:43.456631 nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/__main__.py
--rw-r--r--   0        0        0     1239 2024-03-03 03:21:43.456631 nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/config.py
--rw-r--r--   0        0        0      259 2024-03-03 03:21:43.456631 nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/const.py
--rw-r--r--   0        0        0     6862 2024-03-03 03:21:43.456631 nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/data_source.py
--rw-r--r--   0        0        0      391 2024-03-03 03:21:43.456631 nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/draw/__init__.py
--rw-r--r--   0        0        0     8096 2024-03-03 03:21:43.456631 nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/draw/pil.py
--rw-r--r--   0        0        0     2688 2024-03-03 03:21:43.456631 nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/draw/playwright.py
--rw-r--r--   0        0        0      612 2024-03-03 03:21:43.456631 nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/draw/shared.py
--rw-r--r--   0        0        0     2956 2024-03-03 03:21:43.456631 nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/lrc_parser.py
--rw-r--r--   0        0        0     2527 2024-03-03 03:21:43.456631 nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/msg_cache.py
--rw-r--r--   0        0        0      362 2024-03-03 03:21:43.456631 nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/providers/__init__.py
--rw-r--r--   0        0        0     7897 2024-03-03 03:21:43.456631 nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/providers/base.py
--rw-r--r--   0        0        0     4213 2024-03-03 03:21:43.456631 nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/providers/playlist.py
--rw-r--r--   0        0        0     3185 2024-03-03 03:21:43.456631 nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/providers/song.py
--rw-r--r--   0        0        0     3204 2024-03-03 03:21:43.456631 nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/providers/voice.py
--rw-r--r--   0        0        0   212591 2024-03-03 03:21:43.460631 nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/res/bg.jpg
--rw-r--r--   0        0        0      577 2024-03-03 03:21:43.460631 nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/res/lyric.html.jinja
--rw-r--r--   0        0        0     2829 2024-03-03 03:21:43.460631 nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/res/song_list.html.jinja
--rw-r--r--   0        0        0     3276 2024-03-03 03:21:43.460631 nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/types.py
--rw-r--r--   0        0        0     1948 2024-03-03 03:21:43.460631 nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/utils.py
--rw-r--r--   0        0        0      927 2024-03-03 03:21:55.856758 nonebot_plugin_multincm-0.5.0.dev8/pyproject.toml
--rw-r--r--   0        0        0    14139 1970-01-01 00:00:00.000000 nonebot_plugin_multincm-0.5.0.dev8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-03-10 08:41:56.208868 nonebot_plugin_multincm-0.5.0.dev9/LICENSE
+-rw-r--r--   0        0        0    13776 2024-03-10 08:41:56.208868 nonebot_plugin_multincm-0.5.0.dev9/README.md
+-rw-r--r--   0        0        0     2446 2024-03-10 08:41:56.208868 nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/__init__.py
+-rw-r--r--   0        0        0    18307 2024-03-10 08:41:56.208868 nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/__main__.py
+-rw-r--r--   0        0        0      485 2024-03-10 08:41:56.208868 nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/compact.py
+-rw-r--r--   0        0        0     1247 2024-03-10 08:41:56.208868 nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/config.py
+-rw-r--r--   0        0        0      259 2024-03-10 08:41:56.208868 nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/const.py
+-rw-r--r--   0        0        0     6862 2024-03-10 08:41:56.208868 nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/data_source.py
+-rw-r--r--   0        0        0     3400 2024-03-10 08:41:56.208868 nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/draw.py
+-rw-r--r--   0        0        0     2956 2024-03-10 08:41:56.208868 nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/lrc_parser.py
+-rw-r--r--   0        0        0     2527 2024-03-10 08:41:56.208868 nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/msg_cache.py
+-rw-r--r--   0        0        0      362 2024-03-10 08:41:56.208868 nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/providers/__init__.py
+-rw-r--r--   0        0        0     7897 2024-03-10 08:41:56.208868 nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/providers/base.py
+-rw-r--r--   0        0        0     4213 2024-03-10 08:41:56.208868 nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/providers/playlist.py
+-rw-r--r--   0        0        0     3185 2024-03-10 08:41:56.208868 nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/providers/song.py
+-rw-r--r--   0        0        0     3204 2024-03-10 08:41:56.208868 nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/providers/voice.py
+-rw-r--r--   0        0        0   212591 2024-03-10 08:41:56.208868 nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/res/bg.jpg
+-rw-r--r--   0        0        0      570 2024-03-10 08:41:56.208868 nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/res/lyric.html.jinja
+-rw-r--r--   0        0        0     2822 2024-03-10 08:41:56.208868 nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/res/song_list.html.jinja
+-rw-r--r--   0        0        0     3317 2024-03-10 08:41:56.208868 nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/types.py
+-rw-r--r--   0        0        0     1948 2024-03-10 08:41:56.208868 nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/utils.py
+-rw-r--r--   0        0        0      893 2024-03-10 08:42:08.132866 nonebot_plugin_multincm-0.5.0.dev9/pyproject.toml
+-rw-r--r--   0        0        0    14570 1970-01-01 00:00:00.000000 nonebot_plugin_multincm-0.5.0.dev9/PKG-INFO
```

### Comparing `nonebot_plugin_multincm-0.5.0.dev8/LICENSE` & `nonebot_plugin_multincm-0.5.0.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.5.0.dev8/README.md` & `nonebot_plugin_multincm-0.5.0.dev9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 </a>
 <a href="https://wakatime.com/badge/user/b61b0f9a-f40b-4c82-bc51-0a75c67bfccf/project/f4778875-45a4-4688-8e1b-b8c844440abb">
   <img src="https://wakatime.com/badge/user/b61b0f9a-f40b-4c82-bc51-0a75c67bfccf/project/f4778875-45a4-4688-8e1b-b8c844440abb.svg" alt="wakatime">
 </a>
 
 <br />
 
+<a href="https://pydantic.dev">
+  <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/template/pyd-v1-or-v2.json" alt="Pydantic Version 1 Or 2" >
+</a>
 <a href="./LICENSE">
   <img src="https://img.shields.io/github/license/lgc-NB2Dev/nonebot-plugin-multincm.svg" alt="license">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot-plugin-multincm">
   <img src="https://img.shields.io/pypi/v/nonebot-plugin-multincm.svg" alt="pypi">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot-plugin-multincm">
@@ -132,39 +135,39 @@
 
 如果你安装了 [nonebot-plugin-ncm](https://github.com/kitUIN/nonebot-plugin-ncm)，本插件会与其共用同一个 Session，就可以不用填下面的账号密码了
 
 下面配置中，手机号登录 和 邮箱登录、明文密码 和 MD5 密码哈希 各选其一填写即可
 
 在 nonebot2 项目的 `.env` 文件中添加下表中的必填配置
 
-|           配置项            | 必填 |      默认值       |                                                   说明                                                    |
-| :-------------------------: | :--: | :---------------: | :-------------------------------------------------------------------------------------------------------: |
-|        **登录相关**         |      |                   |                                                                                                           |
-|        `NCM_CTCODE`         |  否  |       `86`        |                                        手机号登录用，登录手机区号                                         |
-|         `NCM_PHONE`         |  否  |        无         |                                         手机号登录用，登录手机号                                          |
-|         `NCM_EMAIL`         |  否  |        无         |                                           邮箱登录用，登录邮箱                                            |
-|       `NCM_PASSWORD`        |  否  |        无         |                                    帐号明文密码，邮箱登录时为邮箱密码                                     |
-|     `NCM_PASSWORD_HASH`     |  否  |        无         |                                  帐号密码 MD5 哈希，邮箱登录时为邮箱密码                                  |
-|        **展示相关**         |      |                   |                                                                                                           |
-|      `NCM_LIST_LIMIT`       |  否  |       `20`        |                                          歌曲列表每页的最大数量                                           |
-|       `NCM_LIST_FONT`       |  否  |        无         |                                          渲染歌曲列表使用的字体                                           |
-|     `NCM_MAX_NAME_LEN`      |  否  |       `600`       |                                  歌曲列表中歌名列的最大文本宽度（像素）                                   |
-|    `NCM_MAX_ARTIST_LEN`     |  否  |       `400`       |                                  歌曲列表中歌手列的最大文本宽度（像素）                                   |
-|    `NCM_LRC_EMPTY_LINE`     |  否  |    `--------`     |                                            填充歌词空行的字符                                             |
-|        **功能相关**         |      |                   |                                                                                                           |
-|    `NCM_MSG_CACHE_TIME`     |  否  |      `43200`      |                                    缓存 用户最近一次操作 的时长（秒）                                     |
-|     `NCM_AUTO_RESOLVE`      |  否  |      `False`      |                             当用户发送音乐链接时，是否自动解析并发送音乐卡片                              |
-| `NCM_RESOLVE_PLAYABLE_CARD` |  否  |      `False`      |                                   开启自动解析时，是否解析可播放的卡片                                    |
-|  `NCM_ILLEGAL_CMD_FINISH`   |  否  |      `False`      |                              当用户在点歌时输入了非法指令，是否直接退出点歌                               |
-|   `NCM_ILLEGAL_CMD_LIMIT`   |  否  |        `3`        | 当未启用 `NCM_ILLEGAL_CMD_FINISH` 时，用户在点歌时输入了多少次非法指令后直接退出点歌，填 `0` 以禁用此功能 |
-|    `NCM_USE_PLAYWRIGHT`     |  否  |      `False`      |                               是否使用 `playwright` 绘制歌曲列表与歌词图片                                |
-|    `NCM_DELETE_LIST_MSG`    |  否  |      `True`       |                                   是否在退出点歌模式后自动撤回歌曲列表                                    |
-| `NCM_DELETE_LIST_MSG_DELAY` |  否  |   `[0.5, 2.0]`    |                                  自动撤回歌曲列表消息间隔时间（单位秒）                                   |
-|  `NCM_UPLOAD_FOLDER_NAME`   |  否  |    `MultiNCM`     |         在群内使用上传指令时，上传到的文件夹名称，不存在时会自动创建，如果创建失败会上传到根目录          |
-|     `NCM_ENABLE_RECORD`     |  否  |      `False`      |                                        是否开启发送歌曲语音的功能                                         |
+|           配置项            | 必填 |    默认值    |                                                   说明                                                    |
+| :-------------------------: | :--: | :----------: | :-------------------------------------------------------------------------------------------------------: |
+|        **登录相关**         |      |              |                                                                                                           |
+|        `NCM_CTCODE`         |  否  |     `86`     |                                        手机号登录用，登录手机区号                                         |
+|         `NCM_PHONE`         |  否  |      无      |                                         手机号登录用，登录手机号                                          |
+|         `NCM_EMAIL`         |  否  |      无      |                                           邮箱登录用，登录邮箱                                            |
+|       `NCM_PASSWORD`        |  否  |      无      |                                    帐号明文密码，邮箱登录时为邮箱密码                                     |
+|     `NCM_PASSWORD_HASH`     |  否  |      无      |                                  帐号密码 MD5 哈希，邮箱登录时为邮箱密码                                  |
+|        **展示相关**         |      |              |                                                                                                           |
+|      `NCM_LIST_LIMIT`       |  否  |     `20`     |                                          歌曲列表每页的最大数量                                           |
+|       `NCM_LIST_FONT`       |  否  |      无      |                                          渲染歌曲列表使用的字体                                           |
+|     `NCM_MAX_NAME_LEN`      |  否  |    `600`     |                                  歌曲列表中歌名列的最大文本宽度（像素）                                   |
+|    `NCM_MAX_ARTIST_LEN`     |  否  |    `400`     |                                  歌曲列表中歌手列的最大文本宽度（像素）                                   |
+|    `NCM_LRC_EMPTY_LINE`     |  否  |  `--------`  |                                            填充歌词空行的字符                                             |
+|        **功能相关**         |      |              |                                                                                                           |
+|    `NCM_MSG_CACHE_TIME`     |  否  |   `43200`    |                                    缓存 用户最近一次操作 的时长（秒）                                     |
+|     `NCM_AUTO_RESOLVE`      |  否  |   `False`    |                             当用户发送音乐链接时，是否自动解析并发送音乐卡片                              |
+| `NCM_RESOLVE_PLAYABLE_CARD` |  否  |   `False`    |                                   开启自动解析时，是否解析可播放的卡片                                    |
+|  `NCM_ILLEGAL_CMD_FINISH`   |  否  |   `False`    |                              当用户在点歌时输入了非法指令，是否直接退出点歌                               |
+|   `NCM_ILLEGAL_CMD_LIMIT`   |  否  |     `3`      | 当未启用 `NCM_ILLEGAL_CMD_FINISH` 时，用户在点歌时输入了多少次非法指令后直接退出点歌，填 `0` 以禁用此功能 |
+|    `NCM_USE_PLAYWRIGHT`     |  否  |   `False`    |                               是否使用 `playwright` 绘制歌曲列表与歌词图片                                |
+|    `NCM_DELETE_LIST_MSG`    |  否  |    `True`    |                                   是否在退出点歌模式后自动撤回歌曲列表                                    |
+| `NCM_DELETE_LIST_MSG_DELAY` |  否  | `[0.5, 2.0]` |                                  自动撤回歌曲列表消息间隔时间（单位秒）                                   |
+|  `NCM_UPLOAD_FOLDER_NAME`   |  否  |  `MultiNCM`  |         在群内使用上传指令时，上传到的文件夹名称，不存在时会自动创建，如果创建失败会上传到根目录          |
+|     `NCM_ENABLE_RECORD`     |  否  |   `False`    |                                        是否开启发送歌曲语音的功能                                         |
 
 ## 🎉 使用
 
 ### 指令
 
 #### 搜索指令
 
@@ -238,18 +241,33 @@
 
   </details>
 
 ## 📝 更新日志
 
 ### 0.5.0（开发中）
 
-- 支持歌单，专辑等（开发中）
+<details open>
+<summary>TODO</summary>
+
+- 多平台发送逻辑（暂定）：
+  - OneBot V11 首先发送卡片，如果发送失败则 fallback
+  - 以文件形式发送
+  - 直接发送直链
+- issue #17
+  - 只有在手动回复解析时才会要求选择，发送链接自动解析时只输出歌单信息
+- 重构图片样式，现在的歌曲列表好丑，歌词图片要限长
+
+<br />
+</details>
+
+- 适配 Pydantic V1 & V2
+- 支持歌单，专辑等，支持多平台（开发中）
 - 点歌指令可以回复一条文本消息作为搜索内容了
-- 支持使用语音发送歌曲
 - resolve [#14](https://github.com/lgc-NB2Dev/nonebot-plugin-multincm/issues/14)
+- 弃用 Pillow
 - 重构部分代码
 
 ### 0.4.4
 
 - 添加配置项 `NCM_ILLEGAL_CMD_LIMIT`
 
 ### 0.4.3
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
 # NoneBot-Plugin-MultiNCM _â¨ ç½æäºå¤éç¹æ­ â¨_[python]_[_p_d_m_-_m_a_n_a_g_e_d_]
                                   _[_w_a_k_a_t_i_m_e_]
-                        _[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_]
+            _[_P_y_d_a_n_t_i_c_ _V_e_r_s_i_o_n_ _1_ _O_r_ _2_]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_]
 ## ð ä»ç»
 ä¸ä¸ªç½æäºå¤éç¹æ­æä»¶ï¼ä¹å¯ä»¥è®¾ç½®æåéï¼çä¸é¢ï¼ï¼å¯ä»¥ç¿»é¡µï¼å¯ä»¥ç»å½ç½æäºè´¦å·ç¹
 vip æ­æ²å¬ï¼æä»¶åéçæ¯èªå®ä¹é³ä¹å¡çï¼ï¼æ²¡äº
 æä»¶è·åçæ¯é³ä¹æ­æ¾é¾æ¥ï¼ä¸ä¼æ¶èä¼åæ¯æä¸è½½æ¬¡æ° ###
 ææå¾ æ­æ²åè¡¨ææå¾ï¼ç¹å»å±å¼ï¼ ![pic](https://
 raw.githubusercontent.com/lgc-NB2Dev/readme/main/multincm/
 QQå¾ç20230515025601.jpg) çµå°åè¡¨ææå¾ï¼ç¹å»å±å¼ï¼ ![pic]
@@ -27,17 +27,17 @@
 "nonebot_plugin_multincm" ] ``` ## âï¸ éç½® å¦æä½ å®è£äº [nonebot-
 plugin-ncm](https://github.com/kitUIN/nonebot-plugin-
 ncm)ï¼æ¬æä»¶ä¼ä¸å¶å±ç¨åä¸ä¸ª
 Sessionï¼å°±å¯ä»¥ä¸ç¨å¡«ä¸é¢çè´¦å·å¯ç äº
 ä¸é¢éç½®ä¸­ï¼ææºå·ç»å½ å é®ç®±ç»å½ãææå¯ç  å MD5
 å¯ç åå¸ åéå¶ä¸å¡«åå³å¯ å¨ nonebot2 é¡¹ç®ç `.env`
 æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« | é»è®¤å¼ |
-è¯´æ | | :-------------------------: | :--: | :---------------: | :----------
+è¯´æ | | :-------------------------: | :--: | :----------: | :---------------
 -------------------------------------------------------------------------------
---------------: | | **ç»å½ç¸å³** | | | | | `NCM_CTCODE` | å¦ | `86` |
+---------: | | **ç»å½ç¸å³** | | | | | `NCM_CTCODE` | å¦ | `86` |
 ææºå·ç»å½ç¨ï¼ç»å½ææºåºå· | | `NCM_PHONE` | å¦ | æ  |
 ææºå·ç»å½ç¨ï¼ç»å½ææºå· | | `NCM_EMAIL` | å¦ | æ  |
 é®ç®±ç»å½ç¨ï¼ç»å½é®ç®± | | `NCM_PASSWORD` | å¦ | æ  |
 å¸å·ææå¯ç ï¼é®ç®±ç»å½æ¶ä¸ºé®ç®±å¯ç  | | `NCM_PASSWORD_HASH` |
 å¦ | æ  | å¸å·å¯ç  MD5 åå¸ï¼é®ç®±ç»å½æ¶ä¸ºé®ç®±å¯ç  | |
 **å±ç¤ºç¸å³** | | | | | `NCM_LIST_LIMIT` | å¦ | `20` |
 æ­æ²åè¡¨æ¯é¡µçæå¤§æ°é | | `NCM_LIST_FONT` | å¦ | æ  |
@@ -92,26 +92,31 @@
 é¡¹ç®ä½¿ç¨çç½æäº API è°ç¨åº ### [Binaryify/NeteaseCloudMusicApi]
 (https://github.com/Binaryify/NeteaseCloudMusicApi) é¡¹ç®çµå°ç¸å³ API
 æ¥æº ### [MeetWq/pil-utils](https://github.com/MeetWq/pil-utils) è¶å¥½ç¨ç
 Pillow è¾å©åº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) - èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png) ## ð æ´æ°æ¥å¿ ### 0.5.0ï¼å¼åä¸­ï¼ -
-æ¯ææ­åï¼ä¸è¾ç­ï¼å¼åä¸­ï¼ -
-ç¹æ­æä»¤å¯ä»¥åå¤ä¸æ¡ææ¬æ¶æ¯ä½ä¸ºæç´¢åå®¹äº -
-æ¯æä½¿ç¨è¯­é³åéæ­æ² - resolve [#14](https://github.com/lgc-NB2Dev/
-nonebot-plugin-multincm/issues/14) - éæé¨åä»£ç  ### 0.4.4 -
-æ·»å éç½®é¡¹ `NCM_ILLEGAL_CMD_LIMIT` ### 0.4.3 - å¯ä»¥éåºæç´¢æ¨¡å¼äº
-### 0.4.2 - resolve [#13](https://github.com/lgc-NB2Dev/nonebot-plugin-
-multincm/issues/13) ### 0.4.1 - æ¯æäº `163cn.tv` ç­é¾ï¼Thanks to
-[@XieXiLin2](https://github.com/XieXiLin2)ï¼ - ä¿®å¤å½
-`NCM_RESOLVE_PLAYABLE_CARD` ä¸º `False` æ¶ï¼Bot ä¾ç¶ä¼åå¤çé®é¢ -
-é¨åä»£ç ä¼å ### 0.4.0 - é¡¹ç®é¨åéæ - å é¤ `é¾æ¥`
-æä»¤ï¼æ°å¢ `ç´é¾`ã`ä¸ä¼ ` æä»¤ -
+imgs/sponsor.png) ## ð æ´æ°æ¥å¿ ### 0.5.0ï¼å¼åä¸­ï¼ TODO -
+å¤å¹³å°åéé»è¾ï¼æå®ï¼ï¼ - OneBot V11
+é¦ååéå¡çï¼å¦æåéå¤±è´¥å fallback - ä»¥æä»¶å½¢å¼åé -
+ç´æ¥åéç´é¾ - issue #17 -
+åªæå¨æå¨åå¤è§£ææ¶æä¼è¦æ±éæ©ï¼åéé¾æ¥èªå¨è§£ææ¶åªè¾åºæ­åä¿¡æ¯
+- éæå¾çæ ·å¼ï¼ç°å¨çæ­æ²åè¡¨å¥½ä¸ï¼æ­è¯å¾çè¦éé¿
+- éé Pydantic V1 & V2 -
+æ¯ææ­åï¼ä¸è¾ç­ï¼æ¯æå¤å¹³å°ï¼å¼åä¸­ï¼ -
+ç¹æ­æä»¤å¯ä»¥åå¤ä¸æ¡ææ¬æ¶æ¯ä½ä¸ºæç´¢åå®¹äº - resolve [#14]
+(https://github.com/lgc-NB2Dev/nonebot-plugin-multincm/issues/14) - å¼ç¨
+Pillow - éæé¨åä»£ç  ### 0.4.4 - æ·»å éç½®é¡¹ `NCM_ILLEGAL_CMD_LIMIT`
+### 0.4.3 - å¯ä»¥éåºæç´¢æ¨¡å¼äº ### 0.4.2 - resolve [#13](https://
+github.com/lgc-NB2Dev/nonebot-plugin-multincm/issues/13) ### 0.4.1 - æ¯æäº
+`163cn.tv` ç­é¾ï¼Thanks to [@XieXiLin2](https://github.com/XieXiLin2)ï¼ -
+ä¿®å¤å½ `NCM_RESOLVE_PLAYABLE_CARD` ä¸º `False` æ¶ï¼Bot
+ä¾ç¶ä¼åå¤çé®é¢ - é¨åä»£ç ä¼å ### 0.4.0 - é¡¹ç®é¨åéæ -
+å é¤ `é¾æ¥` æä»¤ï¼æ°å¢ `ç´é¾`ã`ä¸ä¼ ` æä»¤ -
 å°å¡çç¹å»åè·³è½¬çå°åæ¹ä¸ºå®ç½æ­æ²é¡µï¼ä»£æ¿ `é¾æ¥`
 æä»¤ï¼åæ¶å é¤äºåéè¿é³ä¹å¡ççç¼å­æºå¶ - æ·»å éç½®é¡¹
 `NCM_RESOLVE_PLAYABLE_CARD`ã`NCM_UPLOAD_FOLDER_NAME` ### 0.3.9 - è®©
 `htmlrender` æä¸ºçæ­£çå¯éä¾èµ - æéç½®é¡¹ `NCM_MSG_CACHE_TIME`
 çé»è®¤å¼æ¹ä¸º `43200`ï¼12 å°æ¶ï¼ ### 0.3.8 -
 ä¿®æ¹åç»ä¸è¡¨æ ¼èæ¯è² ### 0.3.7 - æ·»å éç½®é¡¹
 `NCM_DELETE_LIST_MSG` å `NCM_DELETE_LIST_MSG_DELAY`ï¼[#5](https://
```

### Comparing `nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/__init__.py` & `nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from nonebot.plugin import PluginMetadata
 
 from . import __main__ as __main__  # noqa: E402
 from .config import ConfigModel, config  # noqa: E402
 
 auto_resolve_tip = "▶ Bot 会自动解析你发送的网易云链接\n"
 
-__version__ = "0.5.0.dev8"
+__version__ = "0.5.0.dev9"
 __plugin_meta__ = PluginMetadata(
     name="MultiNCM",
     description="网易云多选点歌",
     usage=(
         "搜索指令：\n"
         "▶ 点歌 [歌曲名 / 音乐 ID]\n"
         "    ▷ 介绍：搜索歌曲。当输入音乐 ID 时会直接发送对应音乐\n"
```

### Comparing `nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/__main__.py` & `nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/__main__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/config.py` & `nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/config.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from typing import Optional, Tuple
 
-from nonebot import get_driver
-from pydantic import BaseModel, validator
+from nonebot import get_plugin_config
+from pydantic import BaseModel
+
+from .compact import field_validator
 
 
 class ConfigModel(BaseModel):
     ncm_ctcode: int = 86
     ncm_phone: Optional[str] = None
     ncm_email: Optional[str] = None
     ncm_password: Optional[str] = None
@@ -24,16 +26,16 @@
     ncm_illegal_cmd_finish: bool = False
     ncm_illegal_cmd_limit: int = 3
     ncm_delete_list_msg: bool = True
     ncm_delete_list_msg_delay: Tuple[float, float] = (0.5, 2.0)
     ncm_upload_folder_name: str = "MultiNCM"
     ncm_enable_record: bool = False
 
-    @validator("ncm_upload_folder_name")
+    @field_validator("ncm_upload_folder_name")
     def validate_upload_folder_name(cls, v: str) -> str:  # noqa: N805
         v = v.strip("/")
         if "/" in v:
             raise ValueError("Upload folder name cannot contain `/`")
         return v
 
 
-config: ConfigModel = ConfigModel.parse_obj(get_driver().config.dict())
+config = get_plugin_config(ConfigModel)
```

### Comparing `nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/data_source.py` & `nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/draw/playwright.py` & `nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/draw.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,77 @@
+from dataclasses import dataclass
+from math import ceil
 from pathlib import Path
-from typing import Optional
+from typing import List, Literal, NamedTuple, Optional, Tuple, Union
 
-import bbcode
+import bbcode  # TODO 弃用 bbcode
 from jinja2 import Template
-from nonebot import logger
 from nonebot_plugin_htmlrender import get_new_page
-from pil_utils.fonts import Font
-from pil_utils.types import ColorType, HAlignType
 
-from ..config import config
-from ..const import RES_DIR
-from .shared import TablePage
+from .config import config
+from .const import RES_DIR
+
+ColorType = Union[str, Tuple[int, int, int], Tuple[int, int, int, int]]
+HAlignType = Literal["left", "right", "center"]
+
 
 SONG_LIST_TEMPLATE = Template(
     (RES_DIR / "song_list.html.jinja").read_text(encoding="u8"),
+    autoescape=True,
     enable_async=True,
 )
 LYRIC_TEMPLATE = Template(
     (RES_DIR / "lyric.html.jinja").read_text(encoding="u8"),
+    autoescape=True,
     enable_async=True,
 )
 BBCODE_PARSER = bbcode.Parser()
 BBCODE_PARSER.install_default_formatters()
 
 
+@dataclass()
+class TableHead:
+    name: str
+    align: HAlignType = "left"
+    min_width: Optional[int] = None
+    max_width: Optional[int] = None
+
+
+class Table(NamedTuple):
+    head: List[TableHead]
+    rows: List[List[str]]
+
+
+@dataclass()
+class TablePage:
+    table: Table
+    calling: str
+    current_page: int
+    max_count: int
+
+    @property
+    def max_page(self) -> int:
+        return ceil(self.max_count / config.ncm_list_limit)
+
+
 def get_font_path_uri() -> Optional[str]:
     font_path = config.ncm_list_font
-    if font_path:
-        if (path := Path(font_path)).exists():
-            return path.resolve().as_uri()
-        return Font.find(font_path).path.as_uri()
-    return None
+    if font_path and (path := Path(font_path)).exists():
+        p = path.resolve().as_uri().replace("\\", "\\\\").replace("'", "\\'")
+        return f"url('{p}')"
+    return f"local('{font_path}')" if font_path else None
 
 
 async def render_template(
     template: "Template",
     **kwargs,
 ) -> bytes:
     html_txt = await template.render_async(**kwargs)
-    logger.debug(html_txt)
+    if (dbg := Path.cwd() / "multincm-debug.html").exists():
+        dbg.write_text(html_txt, encoding="u8")
     async with get_new_page() as page:
         await page.goto(RES_DIR.as_uri())
         await page.set_content(html_txt, wait_until="networkidle")
         main_elem = await page.query_selector(".main")
         assert main_elem
         return await main_elem.screenshot(type="jpeg")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/lrc_parser.py` & `nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/lrc_parser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/msg_cache.py` & `nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/msg_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/providers/base.py` & `nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/providers/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/providers/playlist.py` & `nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/providers/playlist.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/providers/song.py` & `nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/providers/song.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/providers/voice.py` & `nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/providers/voice.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/res/bg.jpg` & `nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/res/bg.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/res/lyric.html.jinja` & `nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/res/lyric.html.jinja`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
   <head>
     <meta charset="utf-8" />
 
     <style>
       {% if font_path %}
       @font-face {
         font-family: 'Custom';
-        src: url('{{ font_path }}');
+        src: {{ font_path }};
       }
       {% endif %}
 
       .main {
         width: fit-content;
         margin: 0;
         padding: {{ padding }}px;
```

### Comparing `nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/res/song_list.html.jinja` & `nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/res/song_list.html.jinja`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
   <head>
     <meta charset="utf-8" />
 
     <style>
       {% if font_path %}
       @font-face {
         font-family: 'Custom';
-        src: url('{{ font_path }}');
+        src: {{ font_path }};
       }
       {% endif %}
 
       .main {
         margin: 0;
         padding: 25px;
         width: fit-content;
```

### Comparing `nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/types.py` & `nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,17 @@
     "VoiceSearchResult",
     "PlaylistSearchResult",
 ]
 PlaylistRespModelType: TypeAlias = "Playlist"
 SongInfoModelType = Union["Song", "VoiceBaseInfo"]
 
 
+# TODO snake_case with alias generator
+
+
 class Artist(BaseModel):
     id: int
     name: str
     tns: List[str]
     alias: List[str]
```

### Comparing `nonebot_plugin_multincm-0.5.0.dev8/nonebot_plugin_multincm/utils.py` & `nonebot_plugin_multincm-0.5.0.dev9/nonebot_plugin_multincm/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.5.0.dev8/pyproject.toml` & `nonebot_plugin_multincm-0.5.0.dev9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -4,37 +4,36 @@
 description = "NCM Song Searcher"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.2.0",
     "nonebot-adapter-onebot>=2.2.0",
-    "pydantic>=1.10.0,<2",
-    "pil-utils>=0.1.7",
-    "Pillow>=9,<10",
+    "nonebot-plugin-htmlrender>=0.2.0.3",
     "pyncm>=1.6.8.9.1",
     "typing-extensions>=4.5.0",
     "anyio>=3.6.2",
     "httpx>=0.24.0",
+    "jinja2>=3.1.2",
+    "bbcode>=1.1.0",
 ]
 requires-python = ">=3.9,<4.0"
 readme = "README.md"
-version = "0.5.0.dev8"
+version = "0.5.0.dev9"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/lgc-NB2Dev/nonebot-plugin-multincm"
 
 [project.optional-dependencies]
-playwright = [
-    "nonebot-plugin-htmlrender>=0.2.0.3",
-    "jinja2>=3.1.2",
-    "bbcode>=1.1.0",
+pil = [
+    "pil-utils>=0.1.7",
+    "Pillow>=9,<10",
 ]
 
 [tool.pdm.version]
 source = "file"
 path = "nonebot_plugin_multincm/__init__.py"
 
 [tool.pdm.build]
```

### Comparing `nonebot_plugin_multincm-0.5.0.dev8/PKG-INFO` & `nonebot_plugin_multincm-0.5.0.dev9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-multincm
-Version: 0.5.0.dev8
+Version: 0.5.0.dev9
 Summary: NCM Song Searcher
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Requires-Python: <4.0,>=3.9
 Requires-Dist: nonebot2>=2.2.0
 Requires-Dist: nonebot-adapter-onebot>=2.2.0
-Requires-Dist: pydantic<2,>=1.10.0
-Requires-Dist: pil-utils>=0.1.7
-Requires-Dist: Pillow<10,>=9
+Requires-Dist: nonebot-plugin-htmlrender>=0.2.0.3
 Requires-Dist: pyncm>=1.6.8.9.1
 Requires-Dist: typing-extensions>=4.5.0
 Requires-Dist: anyio>=3.6.2
 Requires-Dist: httpx>=0.24.0
-Requires-Dist: nonebot-plugin-htmlrender>=0.2.0.3; extra == "playwright"
-Requires-Dist: jinja2>=3.1.2; extra == "playwright"
-Requires-Dist: bbcode>=1.1.0; extra == "playwright"
-Provides-Extra: playwright
+Requires-Dist: jinja2>=3.1.2
+Requires-Dist: bbcode>=1.1.0
+Requires-Dist: pil-utils>=0.1.7; extra == "pil"
+Requires-Dist: Pillow<10,>=9; extra == "pil"
+Provides-Extra: pil
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD031 MD033 MD036 MD041 -->
 
 <div align="center">
 
 <a href="https://v2.nonebot.dev/store">
@@ -44,14 +43,17 @@
 </a>
 <a href="https://wakatime.com/badge/user/b61b0f9a-f40b-4c82-bc51-0a75c67bfccf/project/f4778875-45a4-4688-8e1b-b8c844440abb">
   <img src="https://wakatime.com/badge/user/b61b0f9a-f40b-4c82-bc51-0a75c67bfccf/project/f4778875-45a4-4688-8e1b-b8c844440abb.svg" alt="wakatime">
 </a>
 
 <br />
 
+<a href="https://pydantic.dev">
+  <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/template/pyd-v1-or-v2.json" alt="Pydantic Version 1 Or 2" >
+</a>
 <a href="./LICENSE">
   <img src="https://img.shields.io/github/license/lgc-NB2Dev/nonebot-plugin-multincm.svg" alt="license">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot-plugin-multincm">
   <img src="https://img.shields.io/pypi/v/nonebot-plugin-multincm.svg" alt="pypi">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot-plugin-multincm">
@@ -156,39 +158,39 @@
 
 如果你安装了 [nonebot-plugin-ncm](https://github.com/kitUIN/nonebot-plugin-ncm)，本插件会与其共用同一个 Session，就可以不用填下面的账号密码了
 
 下面配置中，手机号登录 和 邮箱登录、明文密码 和 MD5 密码哈希 各选其一填写即可
 
 在 nonebot2 项目的 `.env` 文件中添加下表中的必填配置
 
-|           配置项            | 必填 |      默认值       |                                                   说明                                                    |
-| :-------------------------: | :--: | :---------------: | :-------------------------------------------------------------------------------------------------------: |
-|        **登录相关**         |      |                   |                                                                                                           |
-|        `NCM_CTCODE`         |  否  |       `86`        |                                        手机号登录用，登录手机区号                                         |
-|         `NCM_PHONE`         |  否  |        无         |                                         手机号登录用，登录手机号                                          |
-|         `NCM_EMAIL`         |  否  |        无         |                                           邮箱登录用，登录邮箱                                            |
-|       `NCM_PASSWORD`        |  否  |        无         |                                    帐号明文密码，邮箱登录时为邮箱密码                                     |
-|     `NCM_PASSWORD_HASH`     |  否  |        无         |                                  帐号密码 MD5 哈希，邮箱登录时为邮箱密码                                  |
-|        **展示相关**         |      |                   |                                                                                                           |
-|      `NCM_LIST_LIMIT`       |  否  |       `20`        |                                          歌曲列表每页的最大数量                                           |
-|       `NCM_LIST_FONT`       |  否  |        无         |                                          渲染歌曲列表使用的字体                                           |
-|     `NCM_MAX_NAME_LEN`      |  否  |       `600`       |                                  歌曲列表中歌名列的最大文本宽度（像素）                                   |
-|    `NCM_MAX_ARTIST_LEN`     |  否  |       `400`       |                                  歌曲列表中歌手列的最大文本宽度（像素）                                   |
-|    `NCM_LRC_EMPTY_LINE`     |  否  |    `--------`     |                                            填充歌词空行的字符                                             |
-|        **功能相关**         |      |                   |                                                                                                           |
-|    `NCM_MSG_CACHE_TIME`     |  否  |      `43200`      |                                    缓存 用户最近一次操作 的时长（秒）                                     |
-|     `NCM_AUTO_RESOLVE`      |  否  |      `False`      |                             当用户发送音乐链接时，是否自动解析并发送音乐卡片                              |
-| `NCM_RESOLVE_PLAYABLE_CARD` |  否  |      `False`      |                                   开启自动解析时，是否解析可播放的卡片                                    |
-|  `NCM_ILLEGAL_CMD_FINISH`   |  否  |      `False`      |                              当用户在点歌时输入了非法指令，是否直接退出点歌                               |
-|   `NCM_ILLEGAL_CMD_LIMIT`   |  否  |        `3`        | 当未启用 `NCM_ILLEGAL_CMD_FINISH` 时，用户在点歌时输入了多少次非法指令后直接退出点歌，填 `0` 以禁用此功能 |
-|    `NCM_USE_PLAYWRIGHT`     |  否  |      `False`      |                               是否使用 `playwright` 绘制歌曲列表与歌词图片                                |
-|    `NCM_DELETE_LIST_MSG`    |  否  |      `True`       |                                   是否在退出点歌模式后自动撤回歌曲列表                                    |
-| `NCM_DELETE_LIST_MSG_DELAY` |  否  |   `[0.5, 2.0]`    |                                  自动撤回歌曲列表消息间隔时间（单位秒）                                   |
-|  `NCM_UPLOAD_FOLDER_NAME`   |  否  |    `MultiNCM`     |         在群内使用上传指令时，上传到的文件夹名称，不存在时会自动创建，如果创建失败会上传到根目录          |
-|     `NCM_ENABLE_RECORD`     |  否  |      `False`      |                                        是否开启发送歌曲语音的功能                                         |
+|           配置项            | 必填 |    默认值    |                                                   说明                                                    |
+| :-------------------------: | :--: | :----------: | :-------------------------------------------------------------------------------------------------------: |
+|        **登录相关**         |      |              |                                                                                                           |
+|        `NCM_CTCODE`         |  否  |     `86`     |                                        手机号登录用，登录手机区号                                         |
+|         `NCM_PHONE`         |  否  |      无      |                                         手机号登录用，登录手机号                                          |
+|         `NCM_EMAIL`         |  否  |      无      |                                           邮箱登录用，登录邮箱                                            |
+|       `NCM_PASSWORD`        |  否  |      无      |                                    帐号明文密码，邮箱登录时为邮箱密码                                     |
+|     `NCM_PASSWORD_HASH`     |  否  |      无      |                                  帐号密码 MD5 哈希，邮箱登录时为邮箱密码                                  |
+|        **展示相关**         |      |              |                                                                                                           |
+|      `NCM_LIST_LIMIT`       |  否  |     `20`     |                                          歌曲列表每页的最大数量                                           |
+|       `NCM_LIST_FONT`       |  否  |      无      |                                          渲染歌曲列表使用的字体                                           |
+|     `NCM_MAX_NAME_LEN`      |  否  |    `600`     |                                  歌曲列表中歌名列的最大文本宽度（像素）                                   |
+|    `NCM_MAX_ARTIST_LEN`     |  否  |    `400`     |                                  歌曲列表中歌手列的最大文本宽度（像素）                                   |
+|    `NCM_LRC_EMPTY_LINE`     |  否  |  `--------`  |                                            填充歌词空行的字符                                             |
+|        **功能相关**         |      |              |                                                                                                           |
+|    `NCM_MSG_CACHE_TIME`     |  否  |   `43200`    |                                    缓存 用户最近一次操作 的时长（秒）                                     |
+|     `NCM_AUTO_RESOLVE`      |  否  |   `False`    |                             当用户发送音乐链接时，是否自动解析并发送音乐卡片                              |
+| `NCM_RESOLVE_PLAYABLE_CARD` |  否  |   `False`    |                                   开启自动解析时，是否解析可播放的卡片                                    |
+|  `NCM_ILLEGAL_CMD_FINISH`   |  否  |   `False`    |                              当用户在点歌时输入了非法指令，是否直接退出点歌                               |
+|   `NCM_ILLEGAL_CMD_LIMIT`   |  否  |     `3`      | 当未启用 `NCM_ILLEGAL_CMD_FINISH` 时，用户在点歌时输入了多少次非法指令后直接退出点歌，填 `0` 以禁用此功能 |
+|    `NCM_USE_PLAYWRIGHT`     |  否  |   `False`    |                               是否使用 `playwright` 绘制歌曲列表与歌词图片                                |
+|    `NCM_DELETE_LIST_MSG`    |  否  |    `True`    |                                   是否在退出点歌模式后自动撤回歌曲列表                                    |
+| `NCM_DELETE_LIST_MSG_DELAY` |  否  | `[0.5, 2.0]` |                                  自动撤回歌曲列表消息间隔时间（单位秒）                                   |
+|  `NCM_UPLOAD_FOLDER_NAME`   |  否  |  `MultiNCM`  |         在群内使用上传指令时，上传到的文件夹名称，不存在时会自动创建，如果创建失败会上传到根目录          |
+|     `NCM_ENABLE_RECORD`     |  否  |   `False`    |                                        是否开启发送歌曲语音的功能                                         |
 
 ## 🎉 使用
 
 ### 指令
 
 #### 搜索指令
 
@@ -262,18 +264,33 @@
 
   </details>
 
 ## 📝 更新日志
 
 ### 0.5.0（开发中）
 
-- 支持歌单，专辑等（开发中）
+<details open>
+<summary>TODO</summary>
+
+- 多平台发送逻辑（暂定）：
+  - OneBot V11 首先发送卡片，如果发送失败则 fallback
+  - 以文件形式发送
+  - 直接发送直链
+- issue #17
+  - 只有在手动回复解析时才会要求选择，发送链接自动解析时只输出歌单信息
+- 重构图片样式，现在的歌曲列表好丑，歌词图片要限长
+
+<br />
+</details>
+
+- 适配 Pydantic V1 & V2
+- 支持歌单，专辑等，支持多平台（开发中）
 - 点歌指令可以回复一条文本消息作为搜索内容了
-- 支持使用语音发送歌曲
 - resolve [#14](https://github.com/lgc-NB2Dev/nonebot-plugin-multincm/issues/14)
+- 弃用 Pillow
 - 重构部分代码
 
 ### 0.4.4
 
 - 添加配置项 `NCM_ILLEGAL_CMD_LIMIT`
 
 ### 0.4.3
```

#### html2text {}

```diff
@@ -1,25 +1,23 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-multincm Version: 0.5.0.dev8
+Metadata-Version: 2.1 Name: nonebot-plugin-multincm Version: 0.5.0.dev9
 Summary: NCM Song Searcher Home-page: https://github.com/lgc-NB2Dev/nonebot-
 plugin-multincm Author-Email: student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
 nonebot-plugin-multincm Requires-Python: <4.0,>=3.9 Requires-Dist:
 nonebot2>=2.2.0 Requires-Dist: nonebot-adapter-onebot>=2.2.0 Requires-Dist:
-pydantic<2,>=1.10.0 Requires-Dist: pil-utils>=0.1.7 Requires-Dist:
-Pillow<10,>=9 Requires-Dist: pyncm>=1.6.8.9.1 Requires-Dist: typing-
-extensions>=4.5.0 Requires-Dist: anyio>=3.6.2 Requires-Dist: httpx>=0.24.0
-Requires-Dist: nonebot-plugin-htmlrender>=0.2.0.3; extra == "playwright"
-Requires-Dist: jinja2>=3.1.2; extra == "playwright" Requires-Dist:
-bbcode>=1.1.0; extra == "playwright" Provides-Extra: playwright Description-
-Content-Type: text/markdown
+nonebot-plugin-htmlrender>=0.2.0.3 Requires-Dist: pyncm>=1.6.8.9.1 Requires-
+Dist: typing-extensions>=4.5.0 Requires-Dist: anyio>=3.6.2 Requires-Dist:
+httpx>=0.24.0 Requires-Dist: jinja2>=3.1.2 Requires-Dist: bbcode>=1.1.0
+Requires-Dist: pil-utils>=0.1.7; extra == "pil" Requires-Dist: Pillow<10,>=9;
+extra == "pil" Provides-Extra: pil Description-Content-Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
 # NoneBot-Plugin-MultiNCM _â¨ ç½æäºå¤éç¹æ­ â¨_[python]_[_p_d_m_-_m_a_n_a_g_e_d_]
                                   _[_w_a_k_a_t_i_m_e_]
-                        _[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_]
+            _[_P_y_d_a_n_t_i_c_ _V_e_r_s_i_o_n_ _1_ _O_r_ _2_]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_]
 ## ð ä»ç»
 ä¸ä¸ªç½æäºå¤éç¹æ­æä»¶ï¼ä¹å¯ä»¥è®¾ç½®æåéï¼çä¸é¢ï¼ï¼å¯ä»¥ç¿»é¡µï¼å¯ä»¥ç»å½ç½æäºè´¦å·ç¹
 vip æ­æ²å¬ï¼æä»¶åéçæ¯èªå®ä¹é³ä¹å¡çï¼ï¼æ²¡äº
 æä»¶è·åçæ¯é³ä¹æ­æ¾é¾æ¥ï¼ä¸ä¼æ¶èä¼åæ¯æä¸è½½æ¬¡æ° ###
 ææå¾ æ­æ²åè¡¨ææå¾ï¼ç¹å»å±å¼ï¼ ![pic](https://
 raw.githubusercontent.com/lgc-NB2Dev/readme/main/multincm/
 QQå¾ç20230515025601.jpg) çµå°åè¡¨ææå¾ï¼ç¹å»å±å¼ï¼ ![pic]
@@ -40,17 +38,17 @@
 "nonebot_plugin_multincm" ] ``` ## âï¸ éç½® å¦æä½ å®è£äº [nonebot-
 plugin-ncm](https://github.com/kitUIN/nonebot-plugin-
 ncm)ï¼æ¬æä»¶ä¼ä¸å¶å±ç¨åä¸ä¸ª
 Sessionï¼å°±å¯ä»¥ä¸ç¨å¡«ä¸é¢çè´¦å·å¯ç äº
 ä¸é¢éç½®ä¸­ï¼ææºå·ç»å½ å é®ç®±ç»å½ãææå¯ç  å MD5
 å¯ç åå¸ åéå¶ä¸å¡«åå³å¯ å¨ nonebot2 é¡¹ç®ç `.env`
 æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« | é»è®¤å¼ |
-è¯´æ | | :-------------------------: | :--: | :---------------: | :----------
+è¯´æ | | :-------------------------: | :--: | :----------: | :---------------
 -------------------------------------------------------------------------------
---------------: | | **ç»å½ç¸å³** | | | | | `NCM_CTCODE` | å¦ | `86` |
+---------: | | **ç»å½ç¸å³** | | | | | `NCM_CTCODE` | å¦ | `86` |
 ææºå·ç»å½ç¨ï¼ç»å½ææºåºå· | | `NCM_PHONE` | å¦ | æ  |
 ææºå·ç»å½ç¨ï¼ç»å½ææºå· | | `NCM_EMAIL` | å¦ | æ  |
 é®ç®±ç»å½ç¨ï¼ç»å½é®ç®± | | `NCM_PASSWORD` | å¦ | æ  |
 å¸å·ææå¯ç ï¼é®ç®±ç»å½æ¶ä¸ºé®ç®±å¯ç  | | `NCM_PASSWORD_HASH` |
 å¦ | æ  | å¸å·å¯ç  MD5 åå¸ï¼é®ç®±ç»å½æ¶ä¸ºé®ç®±å¯ç  | |
 **å±ç¤ºç¸å³** | | | | | `NCM_LIST_LIMIT` | å¦ | `20` |
 æ­æ²åè¡¨æ¯é¡µçæå¤§æ°é | | `NCM_LIST_FONT` | å¦ | æ  |
@@ -105,26 +103,31 @@
 é¡¹ç®ä½¿ç¨çç½æäº API è°ç¨åº ### [Binaryify/NeteaseCloudMusicApi]
 (https://github.com/Binaryify/NeteaseCloudMusicApi) é¡¹ç®çµå°ç¸å³ API
 æ¥æº ### [MeetWq/pil-utils](https://github.com/MeetWq/pil-utils) è¶å¥½ç¨ç
 Pillow è¾å©åº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) - èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png) ## ð æ´æ°æ¥å¿ ### 0.5.0ï¼å¼åä¸­ï¼ -
-æ¯ææ­åï¼ä¸è¾ç­ï¼å¼åä¸­ï¼ -
-ç¹æ­æä»¤å¯ä»¥åå¤ä¸æ¡ææ¬æ¶æ¯ä½ä¸ºæç´¢åå®¹äº -
-æ¯æä½¿ç¨è¯­é³åéæ­æ² - resolve [#14](https://github.com/lgc-NB2Dev/
-nonebot-plugin-multincm/issues/14) - éæé¨åä»£ç  ### 0.4.4 -
-æ·»å éç½®é¡¹ `NCM_ILLEGAL_CMD_LIMIT` ### 0.4.3 - å¯ä»¥éåºæç´¢æ¨¡å¼äº
-### 0.4.2 - resolve [#13](https://github.com/lgc-NB2Dev/nonebot-plugin-
-multincm/issues/13) ### 0.4.1 - æ¯æäº `163cn.tv` ç­é¾ï¼Thanks to
-[@XieXiLin2](https://github.com/XieXiLin2)ï¼ - ä¿®å¤å½
-`NCM_RESOLVE_PLAYABLE_CARD` ä¸º `False` æ¶ï¼Bot ä¾ç¶ä¼åå¤çé®é¢ -
-é¨åä»£ç ä¼å ### 0.4.0 - é¡¹ç®é¨åéæ - å é¤ `é¾æ¥`
-æä»¤ï¼æ°å¢ `ç´é¾`ã`ä¸ä¼ ` æä»¤ -
+imgs/sponsor.png) ## ð æ´æ°æ¥å¿ ### 0.5.0ï¼å¼åä¸­ï¼ TODO -
+å¤å¹³å°åéé»è¾ï¼æå®ï¼ï¼ - OneBot V11
+é¦ååéå¡çï¼å¦æåéå¤±è´¥å fallback - ä»¥æä»¶å½¢å¼åé -
+ç´æ¥åéç´é¾ - issue #17 -
+åªæå¨æå¨åå¤è§£ææ¶æä¼è¦æ±éæ©ï¼åéé¾æ¥èªå¨è§£ææ¶åªè¾åºæ­åä¿¡æ¯
+- éæå¾çæ ·å¼ï¼ç°å¨çæ­æ²åè¡¨å¥½ä¸ï¼æ­è¯å¾çè¦éé¿
+- éé Pydantic V1 & V2 -
+æ¯ææ­åï¼ä¸è¾ç­ï¼æ¯æå¤å¹³å°ï¼å¼åä¸­ï¼ -
+ç¹æ­æä»¤å¯ä»¥åå¤ä¸æ¡ææ¬æ¶æ¯ä½ä¸ºæç´¢åå®¹äº - resolve [#14]
+(https://github.com/lgc-NB2Dev/nonebot-plugin-multincm/issues/14) - å¼ç¨
+Pillow - éæé¨åä»£ç  ### 0.4.4 - æ·»å éç½®é¡¹ `NCM_ILLEGAL_CMD_LIMIT`
+### 0.4.3 - å¯ä»¥éåºæç´¢æ¨¡å¼äº ### 0.4.2 - resolve [#13](https://
+github.com/lgc-NB2Dev/nonebot-plugin-multincm/issues/13) ### 0.4.1 - æ¯æäº
+`163cn.tv` ç­é¾ï¼Thanks to [@XieXiLin2](https://github.com/XieXiLin2)ï¼ -
+ä¿®å¤å½ `NCM_RESOLVE_PLAYABLE_CARD` ä¸º `False` æ¶ï¼Bot
+ä¾ç¶ä¼åå¤çé®é¢ - é¨åä»£ç ä¼å ### 0.4.0 - é¡¹ç®é¨åéæ -
+å é¤ `é¾æ¥` æä»¤ï¼æ°å¢ `ç´é¾`ã`ä¸ä¼ ` æä»¤ -
 å°å¡çç¹å»åè·³è½¬çå°åæ¹ä¸ºå®ç½æ­æ²é¡µï¼ä»£æ¿ `é¾æ¥`
 æä»¤ï¼åæ¶å é¤äºåéè¿é³ä¹å¡ççç¼å­æºå¶ - æ·»å éç½®é¡¹
 `NCM_RESOLVE_PLAYABLE_CARD`ã`NCM_UPLOAD_FOLDER_NAME` ### 0.3.9 - è®©
 `htmlrender` æä¸ºçæ­£çå¯éä¾èµ - æéç½®é¡¹ `NCM_MSG_CACHE_TIME`
 çé»è®¤å¼æ¹ä¸º `43200`ï¼12 å°æ¶ï¼ ### 0.3.8 -
 ä¿®æ¹åç»ä¸è¡¨æ ¼èæ¯è² ### 0.3.7 - æ·»å éç½®é¡¹
 `NCM_DELETE_LIST_MSG` å `NCM_DELETE_LIST_MSG_DELAY`ï¼[#5](https://
```

