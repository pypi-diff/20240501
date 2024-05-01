# Comparing `tmp/pytgpt_bot-0.1.7.tar.gz` & `tmp/pytgpt_bot-0.1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytgpt_bot-0.1.7.tar", last modified: Tue Apr 30 22:08:39 2024, max compression
+gzip compressed data, was "pytgpt_bot-0.1.7.1.tar", last modified: Wed May  1 00:19:52 2024, max compression
```

## Comparing `pytgpt_bot-0.1.7.tar` & `pytgpt_bot-0.1.7.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:08:39.919132 pytgpt_bot-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-30 22:08:07.000000 pytgpt_bot-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8264 2024-04-30 22:08:39.919132 pytgpt_bot-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-04-30 22:08:07.000000 pytgpt_bot-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:08:39.915132 pytgpt_bot-0.1.7/pytgpt_bot/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-30 22:08:07.000000 pytgpt_bot-0.1.7/pytgpt_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-30 22:08:07.000000 pytgpt_bot-0.1.7/pytgpt_bot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-30 22:08:07.000000 pytgpt_bot-0.1.7/pytgpt_bot/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-30 22:08:07.000000 pytgpt_bot-0.1.7/pytgpt_bot/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-30 22:08:07.000000 pytgpt_bot-0.1.7/pytgpt_bot/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-30 22:08:07.000000 pytgpt_bot-0.1.7/pytgpt_bot/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    28271 2024-04-30 22:08:07.000000 pytgpt_bot-0.1.7/pytgpt_bot/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-30 22:08:07.000000 pytgpt_bot-0.1.7/pytgpt_bot/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-30 22:08:07.000000 pytgpt_bot-0.1.7/pytgpt_bot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:08:39.919132 pytgpt_bot-0.1.7/pytgpt_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8264 2024-04-30 22:08:39.000000 pytgpt_bot-0.1.7/pytgpt_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-30 22:08:39.000000 pytgpt_bot-0.1.7/pytgpt_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 22:08:39.000000 pytgpt_bot-0.1.7/pytgpt_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-30 22:08:39.000000 pytgpt_bot-0.1.7/pytgpt_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-30 22:08:39.000000 pytgpt_bot-0.1.7/pytgpt_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-30 22:08:39.000000 pytgpt_bot-0.1.7/pytgpt_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 22:08:39.919132 pytgpt_bot-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-30 22:08:07.000000 pytgpt_bot-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:19:52.734260 pytgpt_bot-0.1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-01 00:19:24.000000 pytgpt_bot-0.1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-05-01 00:19:52.734260 pytgpt_bot-0.1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-05-01 00:19:24.000000 pytgpt_bot-0.1.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:19:52.734260 pytgpt_bot-0.1.7.1/pytgpt_bot/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-01 00:19:24.000000 pytgpt_bot-0.1.7.1/pytgpt_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-01 00:19:24.000000 pytgpt_bot-0.1.7.1/pytgpt_bot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-05-01 00:19:24.000000 pytgpt_bot-0.1.7.1/pytgpt_bot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-01 00:19:24.000000 pytgpt_bot-0.1.7.1/pytgpt_bot/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-01 00:19:24.000000 pytgpt_bot-0.1.7.1/pytgpt_bot/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-01 00:19:24.000000 pytgpt_bot-0.1.7.1/pytgpt_bot/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27944 2024-05-01 00:19:24.000000 pytgpt_bot-0.1.7.1/pytgpt_bot/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-01 00:19:24.000000 pytgpt_bot-0.1.7.1/pytgpt_bot/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-05-01 00:19:24.000000 pytgpt_bot-0.1.7.1/pytgpt_bot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:19:52.734260 pytgpt_bot-0.1.7.1/pytgpt_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-05-01 00:19:52.000000 pytgpt_bot-0.1.7.1/pytgpt_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-01 00:19:52.000000 pytgpt_bot-0.1.7.1/pytgpt_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:19:52.000000 pytgpt_bot-0.1.7.1/pytgpt_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-01 00:19:52.000000 pytgpt_bot-0.1.7.1/pytgpt_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-01 00:19:52.000000 pytgpt_bot-0.1.7.1/pytgpt_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-01 00:19:52.000000 pytgpt_bot-0.1.7.1/pytgpt_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 00:19:52.734260 pytgpt_bot-0.1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-01 00:19:24.000000 pytgpt_bot-0.1.7.1/setup.py
```

### Comparing `pytgpt_bot-0.1.7/LICENSE` & `pytgpt_bot-0.1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.1.7/PKG-INFO` & `pytgpt_bot-0.1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytgpt-bot
-Version: 0.1.7
+Version: 0.1.7.1
 Summary: AI powered Telegram bot for chatting, text-to-image and text-to-speech conversions
 Home-page: https://github.com/Simatwa/pytgpt-bot
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/pytgpt-bot/issues/new
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.1.7 Summary: AI powered
+Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.1.7.1 Summary: AI powered
 Telegram bot for chatting, text-to-image and text-to-speech conversions Home-
 page: https://github.com/Simatwa/pytgpt-bot Author: Smartwa Author-email:
 simatwacaleb@proton.me Maintainer: Smartwa License: MIT Project-URL: Bug
 Report, https://github.com/Simatwa/pytgpt-bot/issues/new Project-URL: Homepage,
 https://github.com/Simatwa/pytgpt-bot Project-URL: Source Code, https://
 github.com/Simatwa/pytgpt-bot Project-URL: Issue Tracker, https://github.com/
 Simatwa/pytgpt-bot/issues Project-URL: Download, https://github.com/Simatwa/
```

### Comparing `pytgpt_bot-0.1.7/README.md` & `pytgpt_bot-0.1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.1.7/pytgpt_bot/cli.py` & `pytgpt_bot-0.1.7.1/pytgpt_bot/cli.py`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.1.7/pytgpt_bot/config.py` & `pytgpt_bot-0.1.7.1/pytgpt_bot/config.py`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.1.7/pytgpt_bot/db.py` & `pytgpt_bot-0.1.7.1/pytgpt_bot/db.py`

 * *Files 21% similar despite different names*

```diff
@@ -21,15 +21,14 @@
         chat = session.query(Chat).filter_by(id=id).first()
         if chat:
             # chat exist
             self.chat = chat
         else:
             self.chat = Chat(id=id)
             session.add(self.chat)
-            session.commit()
 
     @property
     def is_admin(self) -> bool:
         """Checks user admin status"""
         return self.chat.id == admin_id
 
     def delete(self) -> None:
```

### Comparing `pytgpt_bot-0.1.7/pytgpt_bot/filters.py` & `pytgpt_bot-0.1.7.1/pytgpt_bot/filters.py`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.1.7/pytgpt_bot/main.py` & `pytgpt_bot-0.1.7.1/pytgpt_bot/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -225,15 +225,14 @@
     session.add(
         Temp(
             uuid=uuid,
             provider=provider,
             prompt=prompt,
         )
     )
-    session.commit()
     regenerate_button = telebot.types.InlineKeyboardButton(
         text="♻️", callback_data=f"media:{get_user_id(message,)}:{uuid}"
     )
     delete_button = telebot.types.InlineKeyboardButton(
         text="🗑️", callback_data=f"delete:{message.chat.id}:{message.id}"
     )
     markup.add(regenerate_button, delete_button)
@@ -274,30 +273,28 @@
         return bot.reply_to(
             message,
             f"{get_random_emoji('sad')} The chat introduction must be at least 10 characters long.",
             reply_markup=make_delete_markup(message),
         )
     user = User(message)
     user.chat.intro = intro
-    session.commit()
     return bot.reply_to(
         message, "New intro set successfully.", reply_markup=make_delete_markup(message)
     )
 
 
 @bot.message_handler(commands=["voice"], is_chat_admin=True)
 @bot.channel_post_handler(commands=["voice"], is_chat_admin=True)
 @handler_formatter(text=False, preserve=True)
 def set_new_speech_voice(message: telebot.types.Message):
     """Set new voice for speech synthesis"""
     user_id: str = get_user_id(message)
     arguments: str = telebot_util.extract_arguments(message.text)
     if arguments and arguments in audio_generator.all_voices:
         User(user_id=user_id).chat.voice = arguments
-        session.commit()
         return send_and_add_delete_button(
             message,
             f"{get_random_emoji('happy')} New voice set : `{arguments}`",
             as_reply=True,
         )
 
     markup = telebot.types.InlineKeyboardMarkup(row_width=4)
@@ -320,15 +317,14 @@
     """Set new voice for speech synthesis callback handler"""
     bot.delete_message(call.message.chat.id, call.message.id)
     voice, user_id = call.data.split(":")
     message = call.message
     markup = make_delete_markup(call.message)
     user = User(user_id=user_id)
     user.chat.voice = voice
-    session.commit()
     return bot.send_message(
         message.chat.id,
         f"{get_random_emoji('happy')} New voice set : `{voice}`",
         reply_markup=markup,
         parse_mode="Markdown",
     )
 
@@ -338,15 +334,14 @@
 @handler_formatter(text=False, preserve=True)
 def set_new_chat_provider(message: telebot.types.Message):
     """Set new text provider"""
     user_id: str = get_user_id(message)
     arguments: str = telebot_util.extract_arguments(message.text)
     if arguments and arguments in provider_keys + g4f_providers:
         User(user_id=user_id).chat.provider = arguments
-        session.commit()
         return send_and_add_delete_button(
             message,
             f"New text provider set {get_random_emoji('love')}: `{arguments}`",
             as_reply=True,
         )
     markup = telebot.types.InlineKeyboardMarkup(row_width=2)
     make_item = lambda provider: telebot.types.InlineKeyboardButton(
@@ -368,15 +363,14 @@
     """Set new text provider callback handler"""
     bot.delete_message(call.message.chat.id, call.message.id)
     provider, user_id = call.data.split(":")
     message = call.message
     markup = make_delete_markup(call.message)
     user = User(user_id=user_id)
     user.chat.provider = provider
-    session.commit()
     return bot.send_message(
         message.chat.id,
         f"New text provider set {get_random_emoji('love')}: `{provider}`",
         reply_markup=markup,
         parse_mode="Markdown",
     )
 
@@ -387,15 +381,14 @@
 def set_awesome_prompt_as_chat_intro(message: telebot.types.Message):
     """Set awesome prompt as intro"""
     user_id: str = get_user_id(message)
     arguments: str = telebot_util.extract_arguments(message.text)
     if arguments and arguments in awesome_prompts_keys:
         new_awesome: str = awesome_prompts_dict.get(arguments)
         User(user_id=user_id).chat.intro = new_awesome
-        session.commit()
         return send_and_add_delete_button(
             message,
             f"""New awesome-intro set:\n```{new_awesome}\n```.""",
             as_reply=True,
         )
     markup = telebot.types.InlineKeyboardMarkup(row_width=4)
     make_item = lambda awesome: telebot.types.InlineKeyboardButton(
@@ -417,15 +410,14 @@
     call: telebot.types.CallbackQuery,
 ):
     """Set awesome prompt as intro callback handler"""
     bot.delete_message(call.message.chat.id, call.message.id)
     awesome_prompt, user_id = call.data.split(":")
     user = User(user_id=user_id)
     user.chat.intro = awesome_prompts_dict.get(awesome_prompt)
-    session.commit()
     return bot.send_message(
         call.message.chat.id,
         f"""New awesome-intro set:\n```{user.chat.intro}\n```.""",
         reply_markup=make_delete_markup(call.message),
         parse_mode="Markdown",
     )
 
@@ -544,53 +536,49 @@
 @bot.message_handler(commands=["reset"], is_chat_admin=True, is_chat_active=True)
 @bot.channel_post_handler(commands=["reset"], is_chat_admin=True, is_chat_active=True)
 @handler_formatter()
 def reset_chat(message: telebot.types.Message):
     """Reset current chat thread"""
     user = User(message)
     session.delete(user.chat)
-    session.commit()
     return bot.reply_to(
         message,
         f"New chat instance created. {get_random_emoji('happy')}",
         reply_markup=make_delete_markup(message),
     )
 
 
 @bot.message_handler(commands=["suspend"], is_chat_admin=True, is_chat_active=True)
 @bot.channel_post_handler(commands=["suspend"], is_chat_admin=True, is_chat_active=True)
 @handler_formatter()
 def change_chat_status_to_inactive(message: telebot.types.Message):
     chats = User(message).chat
     chats.is_active = False
-    session.commit()
     return bot.reply_to(
         message, text=f"Service Suspended 🚫.", reply_markup=make_delete_markup(message)
     )
 
 
 @bot.message_handler(commands=["resume"], is_chat_admin=True)
 @bot.channel_post_handler(commands=["resume"], is_chat_admin=True)
 @handler_formatter()
 def change_chat_status_to_active(message: telebot.types.Message):
     chat = User(message).chat
     chat.is_active = True
-    session.commit()
     return bot.reply_to(
         message, text=f"Service Resumed 🚀.", reply_markup=make_delete_markup(message)
     )
 
 
 @bot.message_handler(commands=["clear", "clear_tables"], is_bot_owner=True)
 @handler_formatter()
 def clear_chats(message: telebot.types.Message):
     """Delete all Tables"""
     session.query(Chat).delete()
     session.query(Temp).delete()
-    session.commit()
     logging.warning(
         f"Clearing Chats - [{message.from_user.full_name}] ({get_user_id(message)}, {message.from_user.username})"
     )
     return bot.reply_to(
         message,
         f"{get_random_emoji('love')} Tables cleared successfully.",
         reply_markup=make_delete_markup(message),
@@ -622,17 +610,15 @@
         logging.info(
             f"ADMIN CLEARED LOGS & DROPPED CHAT TABLE [{get_user_id(message)}] - ({message.from_user.full_name})\n"
         )
     logging.warning(
         f"Dropping all tables and recreate - [{message.from_user.full_name}] ({get_user_id(message)}, {message.from_user.username})"
     )
     drop_all()
-    session.commit()
     create_all()
-    session.commit()
     return bot.reply_to(
         message,
         f"{get_random_emoji('love')} All tables dropped and logs cleared. New one created.",
         reply_markup=make_delete_markup(message),
     )
 
 
@@ -712,15 +698,14 @@
         provider_class_kwargs["provider"] = user.chat.provider
 
     ai_response = provider_class(**provider_class_kwargs).chat(conversation_prompt)
     conversation.update_chat_history(
         prompt=message.text, response=ai_response, force=True
     )
     user.chat.history = conversation.chat_history
-    session.commit()
     send_long_text(message, ai_response, as_reply=False if message.from_user else True)
 
 
 @bot.callback_query_handler(func=lambda call: call.data.startswith("media:"))
 def media_regeneration_callback_handler(
     call: telebot.types.CallbackQuery,
 ):
```

### Comparing `pytgpt_bot-0.1.7/pytgpt_bot/models.py` & `pytgpt_bot-0.1.7.1/pytgpt_bot/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     database_str: str = f"sqlite:///{path_to_default_db.as_posix()}"
 
 engine = create_engine(database_str)
 
 autocommit_engine = engine.execution_options(isolation_level="AUTOCOMMIT")
 
-Session = sessionmaker(bind=engine)
+Session = sessionmaker(bind=autocommit_engine)
 
 session = Session()
 
 Base = declarative_base()
 
 
 class Chat(Base):
```

### Comparing `pytgpt_bot-0.1.7/pytgpt_bot/utils.py` & `pytgpt_bot-0.1.7.1/pytgpt_bot/utils.py`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.1.7/pytgpt_bot.egg-info/PKG-INFO` & `pytgpt_bot-0.1.7.1/pytgpt_bot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytgpt-bot
-Version: 0.1.7
+Version: 0.1.7.1
 Summary: AI powered Telegram bot for chatting, text-to-image and text-to-speech conversions
 Home-page: https://github.com/Simatwa/pytgpt-bot
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/pytgpt-bot/issues/new
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.1.7 Summary: AI powered
+Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.1.7.1 Summary: AI powered
 Telegram bot for chatting, text-to-image and text-to-speech conversions Home-
 page: https://github.com/Simatwa/pytgpt-bot Author: Smartwa Author-email:
 simatwacaleb@proton.me Maintainer: Smartwa License: MIT Project-URL: Bug
 Report, https://github.com/Simatwa/pytgpt-bot/issues/new Project-URL: Homepage,
 https://github.com/Simatwa/pytgpt-bot Project-URL: Source Code, https://
 github.com/Simatwa/pytgpt-bot Project-URL: Issue Tracker, https://github.com/
 Simatwa/pytgpt-bot/issues Project-URL: Download, https://github.com/Simatwa/
```

### Comparing `pytgpt_bot-0.1.7/setup.py` & `pytgpt_bot-0.1.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     full_path: Path = ROOT_PATH / path
     return full_path.read_text(encoding="utf-8")
 
 
 setup(
     name="pytgpt-bot",
     packages=["pytgpt_bot"],
-    version="0.1.7",
+    version="0.1.7.1",
     license="MIT",
     author="Smartwa",
     maintainer="Smartwa",
     author_email="simatwacaleb@proton.me",
     description="AI powered Telegram bot for chatting, text-to-image and text-to-speech conversions",
     url="https://github.com/Simatwa/pytgpt-bot",
     project_urls={
```

