# Comparing `tmp/nonebot_plugin_bilifan-0.3.3.tar.gz` & `tmp/nonebot_plugin_bilifan-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilifan-0.3.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_bilifan-0.3.4.tar", max compression
```

## Comparing `nonebot_plugin_bilifan-0.3.3.tar` & `nonebot_plugin_bilifan-0.3.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2024-04-28 06:24:05.397790 nonebot_plugin_bilifan-0.3.3/LICENSE
--rw-r--r--   0        0        0     2246 2024-04-28 06:24:05.397790 nonebot_plugin_bilifan-0.3.3/README.md
--rw-r--r--   0        0        0     8034 2024-04-28 06:24:05.397790 nonebot_plugin_bilifan-0.3.3/nonebot_plugin_bilifan/__init__.py
--rw-r--r--   0        0        0     6064 2024-04-28 06:24:05.397790 nonebot_plugin_bilifan-0.3.3/nonebot_plugin_bilifan/login/__init__.py
--rw-r--r--   0        0        0     6616 2024-04-28 06:24:05.397790 nonebot_plugin_bilifan-0.3.3/nonebot_plugin_bilifan/main.py
--rw-r--r--   0        0        0       80 2024-04-28 06:24:05.397790 nonebot_plugin_bilifan-0.3.3/nonebot_plugin_bilifan/src/__init__.py
--rw-r--r--   0        0        0    17653 2024-04-28 06:24:05.397790 nonebot_plugin_bilifan-0.3.3/nonebot_plugin_bilifan/src/api.py
--rw-r--r--   0        0        0    19425 2024-04-28 06:24:05.397790 nonebot_plugin_bilifan-0.3.3/nonebot_plugin_bilifan/src/user.py
--rw-r--r--   0        0        0     2197 2024-04-28 06:24:05.397790 nonebot_plugin_bilifan-0.3.3/nonebot_plugin_bilifan/users.yaml
--rw-r--r--   0        0        0     3020 2024-04-28 06:24:05.397790 nonebot_plugin_bilifan-0.3.3/nonebot_plugin_bilifan/utils.py
--rw-r--r--   0        0        0     2061 2024-04-28 06:24:05.397790 nonebot_plugin_bilifan-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     3492 1970-01-01 00:00:00.000000 nonebot_plugin_bilifan-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-01 16:53:36.756244 nonebot_plugin_bilifan-0.3.4/LICENSE
+-rw-r--r--   0        0        0     2336 2024-05-01 16:53:36.756244 nonebot_plugin_bilifan-0.3.4/README.md
+-rw-r--r--   0        0        0     8034 2024-05-01 16:53:36.756244 nonebot_plugin_bilifan-0.3.4/nonebot_plugin_bilifan/__init__.py
+-rw-r--r--   0        0        0     6146 2024-05-01 16:53:36.756244 nonebot_plugin_bilifan-0.3.4/nonebot_plugin_bilifan/login/__init__.py
+-rw-r--r--   0        0        0     6616 2024-05-01 16:53:36.756244 nonebot_plugin_bilifan-0.3.4/nonebot_plugin_bilifan/main.py
+-rw-r--r--   0        0        0       80 2024-05-01 16:53:36.756244 nonebot_plugin_bilifan-0.3.4/nonebot_plugin_bilifan/src/__init__.py
+-rw-r--r--   0        0        0    17653 2024-05-01 16:53:36.756244 nonebot_plugin_bilifan-0.3.4/nonebot_plugin_bilifan/src/api.py
+-rw-r--r--   0        0        0    19454 2024-05-01 16:53:36.756244 nonebot_plugin_bilifan-0.3.4/nonebot_plugin_bilifan/src/user.py
+-rw-r--r--   0        0        0     2197 2024-05-01 16:53:36.756244 nonebot_plugin_bilifan-0.3.4/nonebot_plugin_bilifan/users.yaml
+-rw-r--r--   0        0        0     3020 2024-05-01 16:53:36.760244 nonebot_plugin_bilifan-0.3.4/nonebot_plugin_bilifan/utils.py
+-rw-r--r--   0        0        0     2061 2024-05-01 16:53:36.760244 nonebot_plugin_bilifan-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     3582 1970-01-01 00:00:00.000000 nonebot_plugin_bilifan-0.3.4/PKG-INFO
```

### Comparing `nonebot_plugin_bilifan-0.3.3/LICENSE` & `nonebot_plugin_bilifan-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.3.3/README.md` & `nonebot_plugin_bilifan-0.3.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,18 @@
 <a href="https://pypi.python.org/pypi/nonebot_plugin_bilifan">
         <img src="https://img.shields.io/pypi/v/nonebot_plugin_bilifan.svg" alt="pypi">
 </a>
     <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
     <img src="https://img.shields.io/badge/nonebot-2.0.0-red.svg" alt="NoneBot">
 </div>
 
+## 最新说明
+
+- 已经可以正常使用和登录了，只是输出log暂时有问题
+
 ## 配置说明
 
 启动一次插件，在bot路径下，"data/bilifan"文件夹内，按需求修改"users.yaml"文件
 运行跨平台使用，支持saa下所有适配器
 
 ## 指令
```

#### html2text {}

```diff
@@ -1,12 +1,14 @@
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
    # nonebot_plugin_bilifan _â¨èªå¨bç«ç²ä¸çâ¨__[_G_i_t_H_u_b_ _s_t_a_r_s_]_[_G_i_t_H_u_b
                  _i_s_s_u_e_s_]_[_Q_Q_ _C_h_a_t_ _G_r_o_u_p_]_[_p_y_p_i_][python][NoneBot]
-## éç½®è¯´æ å¯å¨ä¸æ¬¡æä»¶ï¼å¨botè·¯å¾ä¸ï¼"data/
+## ææ°è¯´æ -
+å·²ç»å¯ä»¥æ­£å¸¸ä½¿ç¨åç»å½äºï¼åªæ¯è¾åºlogææ¶æé®é¢ ##
+éç½®è¯´æ å¯å¨ä¸æ¬¡æä»¶ï¼å¨botè·¯å¾ä¸ï¼"data/
 bilifan"æä»¶å¤¹åï¼æéæ±ä¿®æ¹"users.yaml"æä»¶
 è¿è¡è·¨å¹³å°ä½¿ç¨ï¼æ¯æsaaä¸ææééå¨ ## æä»¤ - bç«ç»å½ -
 è¿åbç«äºç»´ç ï¼æ«ç ç»å½ï¼ç»å®qqå· - å é¤ç»å½ä¿¡æ¯ -
 å é¤ç»å½ä¿¡æ¯åç»å® - å¼å§å·çå­ - å¼å§æ§è¡å½ä»¤ -
 èªå¨å·çå­ - æ·»å æåæ¶å®æ¶ä»»å¡ - åæ¶èªå¨å·çå­ -
 åæ¶å®æ¶ä»»å¡ - å é¤å¨é¨çå®æ¶ä»»å¡ -
 [è¶ç®¡]å é¤å¨é¨çå®æ¶ä»»å¡ ## ð å¶ä» -
```

### Comparing `nonebot_plugin_bilifan-0.3.3/nonebot_plugin_bilifan/__init__.py` & `nonebot_plugin_bilifan-0.3.4/nonebot_plugin_bilifan/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         if scheduler
         else "未检测到软依赖<y>nonebot_plugin_apscheduler</y>，<r>禁用定时任务功能</r>"
     ),
 )
 
 
 driver = get_driver()
-__version__ = "0.3.3"
+__version__ = "0.3.4"
 __plugin_meta__ = PluginMetadata(
     name="bilifan",
     description="b站粉丝牌~",
     usage="发送 开始刷牌子 即可",
     type="application",
     homepage="https://github.com/Agnes4m/nonebot_plugin_bilifan",
     supported_adapters=inherit_supported_adapters("nonebot_plugin_saa"),
```

### Comparing `nonebot_plugin_bilifan-0.3.3/nonebot_plugin_bilifan/login/__init__.py` & `nonebot_plugin_bilifan-0.3.4/nonebot_plugin_bilifan/login/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         ) as resp:
             if resp.status != 200:
                 raise Exception("Failed to connect to server")
             resp_data = await resp.json()
             code = resp_data["code"]
             if code == 0:
                 login_url = resp_data["data"]["url"]
-                login_key = resp_data["data"]["qrcode_key"]
+                login_key = resp_data["data"]["auth_code"]
                 return login_url, login_key
             raise Exception("get_tv_qrcode_url_and_auth_code error")
 
 
 async def verify_login(login_key: str, data_path: Path):
     api = "https://passport.bilibili.com/x/passport-tv-login/qrcode/poll"
     data = {
@@ -95,55 +95,57 @@
                 if not Path(data_path / "users.yaml").is_file():
                     logger.info("初始化配置文件")
                     shutil.copy2(
                         Path().joinpath("data/bilifan/users.yaml"),
                         data_path / "users.yaml",
                     )
                 config = yaml.safe_load(
-                    await anyio.Path(data_path / "users.yaml").read_text("u8")
+                    await anyio.Path(data_path / "users.yaml").read_text("u8"),
                 )
                 # with Path(data_path / "users.yaml").open(
                 #     "r", encoding="utf-8"
                 # ) as f:
                 #     config = yaml.safe_load(f)
 
                 config["USERS"][0]["access_key"] = access_key
-                config = yaml.dump(
-                    await anyio.Path(data_path / "users.yaml").write_text("u8"),
+                yaml_string = yaml.dump(
+                    config,
                     allow_unicode=True,
                     default_flow_style=False,
                 )
+                await anyio.Path(data_path / "users.yaml").write_text(yaml_string, "u8")
+
                 # with Path(data_path / "users.yaml").open(
                 #     "w", encoding="utf-8"
                 # ) as f:  # noqa: ASYNC101
                 #     yaml.dump(config, f, allow_unicode=True, default_flow_style=False)
                 return "access_key已保存"
             await asyncio.sleep(3)
 
 
 appkey = "4409e2ce8ffd12b8"
 appsec = "59b43e04ad6965f34319062b478f83dd"
 
 
-async def signature(params: dict):
+async def signature(params: dict):  # noqa: RUF029
     keys = list(params.keys())
     params["appkey"] = appkey
     keys.append("appkey")
     keys.sort()
     query = "&".join([k + "=" + urlparse.quote(params[k]) for k in keys])
     query += appsec
     hash_ = hashlib.md5(query.encode("utf-8"))
     params["sign"] = hash_.hexdigest()
 
 
-async def map_to_string(params: dict) -> str:
+async def map_to_string(params: dict) -> str:  # noqa: RUF029
     return "&".join([k + "=" + v for k, v in params.items()])
 
 
-async def draw_QR(login_url: str):  # noqa: N802
+async def draw_QR(login_url: str):  # noqa: N802, RUF029
     "绘制二维码"
     qr = qrcode.QRCode(version=1, box_size=10, border=4)  # type: ignore
     qr.add_data(login_url)
     qr.make(fit=True)
     img = qr.make_image(fill_color="black", back_color="white")
     buffered = BytesIO()
     img.save(buffered, format="PNG")
```

### Comparing `nonebot_plugin_bilifan-0.3.3/nonebot_plugin_bilifan/main.py` & `nonebot_plugin_bilifan-0.3.4/nonebot_plugin_bilifan/main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.3.3/nonebot_plugin_bilifan/src/api.py` & `nonebot_plugin_bilifan-0.3.4/nonebot_plugin_bilifan/src/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.3.3/nonebot_plugin_bilifan/src/user.py` & `nonebot_plugin_bilifan-0.3.4/nonebot_plugin_bilifan/src/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,27 +107,27 @@
         """
         self.medals.clear()
         self.medalsNeedDo.clear()
         async for medal in self.api.getFansMedalandRoomID():  # type: ignore
             if self.whiteList == [0]:
                 if medal["medal"]["target_id"] in self.bannedList:
                     log.warning(
-                        f"{medal['anchor_info']['nick_name']} 在黑名单中，已过滤"
+                        f"{medal['anchor_info']['nick_name']} 在黑名单中，已过滤",
                     )
                     continue
                 self.medals.append(medal) if medal["room_info"]["room_id"] != 0 else ...
             else:
                 if medal["medal"]["target_id"] in self.whiteList:
                     (
                         self.medals.append(medal)
                         if medal["room_info"]["room_id"] != 0
                         else ...
                     )
                     log.success(
-                        f"{medal['anchor_info']['nick_name']} 在白名单中，加入任务"
+                        f"{medal['anchor_info']['nick_name']} 在白名单中，加入任务",
                     )
         [
             self.medalsNeedDo.append(medal)
             for medal in self.medals
             if medal["medal"]["level"] < 20 and medal["medal"]["today_feed"] < 1500
         ]
 
@@ -220,15 +220,15 @@
             if self.retryTimes > self.maxRetryTimes:
                 log.error("任务重试次数过多,停止任务")
                 return
             if len(finallyMedals) / len(self.medalsNeedDo) <= 0.9:
                 log.warning("成功率过低,重新执行任务")
                 self.retryTimes += 1
                 log.warning(
-                    "重试次数: {}/{}".format(self.retryTimes, self.maxRetryTimes)
+                    "重试次数: {}/{}".format(self.retryTimes, self.maxRetryTimes),
                 )
                 await self.asynclikeandShare(failedMedals)
         except Exception:
             log.exception("点赞、分享任务异常")
             self.errmsg.append(f"【{self.name}】 点赞、分享任务异常,请检查日志")
 
     async def like_v3(self, failedMedals: Optional[list] = None):
@@ -321,16 +321,17 @@
                         n,
                         len(self.medals),
                     ),
                 )
             except Exception as e:
                 log.error(
                     "{} 房间弹幕打卡失败: {}".format(
-                        medal["anchor_info"]["nick_name"], e
-                    )
+                        medal["anchor_info"]["nick_name"],
+                        e,
+                    ),
                 )
                 self.errmsg.append(
                     f"【{self.name}】 {medal['anchor_info']['nick_name']} 房间弹幕打卡失败: {e!s}",
                 )
             finally:
                 await asyncio.sleep(self.config["DANMAKU_CD"])
         if hasattr(self, "initialMedal"):
```

### Comparing `nonebot_plugin_bilifan-0.3.3/nonebot_plugin_bilifan/users.yaml` & `nonebot_plugin_bilifan-0.3.4/nonebot_plugin_bilifan/users.yaml`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.3.3/nonebot_plugin_bilifan/utils.py` & `nonebot_plugin_bilifan-0.3.4/nonebot_plugin_bilifan/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.3.3/pyproject.toml` & `nonebot_plugin_bilifan-0.3.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_bilifan"
-version = "0.3.3"
+version = "0.3.4"
 description = "刷站粉丝牌子的机器人插件"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_bilifan"
 repository = "https://github.com/Agnes4m/nonebot_plugin_bilifan"
 keywords = ["bilibili", "nonebot2", "plugin"]
```

### Comparing `nonebot_plugin_bilifan-0.3.3/PKG-INFO` & `nonebot_plugin_bilifan-0.3.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_bilifan
-Version: 0.3.3
+Version: 0.3.4
 Summary: 刷站粉丝牌子的机器人插件
 Home-page: https://github.com/Agnes4m/nonebot_plugin_bilifan
 License: GPLv3
 Keywords: bilibili,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
@@ -53,14 +53,18 @@
 <a href="https://pypi.python.org/pypi/nonebot_plugin_bilifan">
         <img src="https://img.shields.io/pypi/v/nonebot_plugin_bilifan.svg" alt="pypi">
 </a>
     <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
     <img src="https://img.shields.io/badge/nonebot-2.0.0-red.svg" alt="NoneBot">
 </div>
 
+## 最新说明
+
+- 已经可以正常使用和登录了，只是输出log暂时有问题
+
 ## 配置说明
 
 启动一次插件，在bot路径下，"data/bilifan"文件夹内，按需求修改"users.yaml"文件
 运行跨平台使用，支持saa下所有适配器
 
 ## 指令
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_bilifan Version: 0.3.3 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_bilifan Version: 0.3.4 Summary:
 å·ç«ç²ä¸çå­çæºå¨äººæä»¶ Home-page: https://github.com/Agnes4m/
 nonebot_plugin_bilifan License: GPLv3 Keywords: bilibili,nonebot2,plugin
 Author: Agnes_Digital Author-email: Z735803792@163.com Requires-Python:
 >=3.9,<4.0 Classifier: License :: OSI Approved :: GNU General Public License v3
 (GPLv3) Classifier: License :: Other/Proprietary License Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
@@ -15,15 +15,17 @@
 Dist: pyyaml (>=6.0,<7.0) Requires-Dist: qrcode (>=7.4.2,<8.0.0) Project-URL:
 Repository, https://github.com/Agnes4m/nonebot_plugin_bilifan Description-
 Content-Type: text/markdown
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
    # nonebot_plugin_bilifan _â¨èªå¨bç«ç²ä¸çâ¨__[_G_i_t_H_u_b_ _s_t_a_r_s_]_[_G_i_t_H_u_b
                  _i_s_s_u_e_s_]_[_Q_Q_ _C_h_a_t_ _G_r_o_u_p_]_[_p_y_p_i_][python][NoneBot]
-## éç½®è¯´æ å¯å¨ä¸æ¬¡æä»¶ï¼å¨botè·¯å¾ä¸ï¼"data/
+## ææ°è¯´æ -
+å·²ç»å¯ä»¥æ­£å¸¸ä½¿ç¨åç»å½äºï¼åªæ¯è¾åºlogææ¶æé®é¢ ##
+éç½®è¯´æ å¯å¨ä¸æ¬¡æä»¶ï¼å¨botè·¯å¾ä¸ï¼"data/
 bilifan"æä»¶å¤¹åï¼æéæ±ä¿®æ¹"users.yaml"æä»¶
 è¿è¡è·¨å¹³å°ä½¿ç¨ï¼æ¯æsaaä¸ææééå¨ ## æä»¤ - bç«ç»å½ -
 è¿åbç«äºç»´ç ï¼æ«ç ç»å½ï¼ç»å®qqå· - å é¤ç»å½ä¿¡æ¯ -
 å é¤ç»å½ä¿¡æ¯åç»å® - å¼å§å·çå­ - å¼å§æ§è¡å½ä»¤ -
 èªå¨å·çå­ - æ·»å æåæ¶å®æ¶ä»»å¡ - åæ¶èªå¨å·çå­ -
 åæ¶å®æ¶ä»»å¡ - å é¤å¨é¨çå®æ¶ä»»å¡ -
 [è¶ç®¡]å é¤å¨é¨çå®æ¶ä»»å¡ ## ð å¶ä» -
```

