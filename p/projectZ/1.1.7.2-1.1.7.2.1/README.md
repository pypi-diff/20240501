# Comparing `tmp/projectZ-1.1.7.2.tar.gz` & `tmp/projectZ-1.1.7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "projectZ-1.1.7.2.tar", last modified: Sat Apr 27 09:35:28 2024, max compression
+gzip compressed data, was "projectZ-1.1.7.2.1.tar", last modified: Wed May  1 12:17:06 2024, max compression
```

## Comparing `projectZ-1.1.7.2.tar` & `projectZ-1.1.7.2.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 xsarzy    (1000) xsarzy    (1000)        0 2024-04-27 09:35:28.321388 projectZ-1.1.7.2/
--rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)     2244 2024-04-27 09:35:28.321388 projectZ-1.1.7.2/PKG-INFO
--rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)     1777 2024-04-26 20:11:48.000000 projectZ-1.1.7.2/README.md
-drwxr-xr-x   0 xsarzy    (1000) xsarzy    (1000)        0 2024-04-27 09:35:28.317388 projectZ-1.1.7.2/projectZ/
--rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)      547 2024-04-26 20:11:48.000000 projectZ-1.1.7.2/projectZ/__init__.py
--rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)    14862 2024-04-26 20:11:48.000000 projectZ-1.1.7.2/projectZ/async_client.py
--rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)    13184 2024-04-26 20:11:48.000000 projectZ-1.1.7.2/projectZ/client.py
--rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)     4262 2024-04-26 20:11:48.000000 projectZ-1.1.7.2/projectZ/requests_builder.py
-drwxr-xr-x   0 xsarzy    (1000) xsarzy    (1000)        0 2024-04-27 09:35:28.321388 projectZ-1.1.7.2/projectZ/utils/
--rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)        0 2024-04-26 20:11:48.000000 projectZ-1.1.7.2/projectZ/utils/__init__.py
--rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)     1869 2024-04-26 20:11:48.000000 projectZ-1.1.7.2/projectZ/utils/exceptions.py
--rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)      865 2024-04-26 20:11:48.000000 projectZ-1.1.7.2/projectZ/utils/generator.py
-drwxr-xr-x   0 xsarzy    (1000) xsarzy    (1000)        0 2024-04-27 09:35:28.321388 projectZ-1.1.7.2/projectZ.egg-info/
--rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)     2244 2024-04-27 09:35:28.000000 projectZ-1.1.7.2/projectZ.egg-info/PKG-INFO
--rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)      365 2024-04-27 09:35:28.000000 projectZ-1.1.7.2/projectZ.egg-info/SOURCES.txt
--rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)        1 2024-04-27 09:35:28.000000 projectZ-1.1.7.2/projectZ.egg-info/dependency_links.txt
--rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)       62 2024-04-27 09:35:28.000000 projectZ-1.1.7.2/projectZ.egg-info/requires.txt
--rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)        9 2024-04-27 09:35:28.000000 projectZ-1.1.7.2/projectZ.egg-info/top_level.txt
--rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)       38 2024-04-27 09:35:28.321388 projectZ-1.1.7.2/setup.cfg
--rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)      978 2024-04-27 09:35:18.000000 projectZ-1.1.7.2/setup.py
+drwxr-xr-x   0 xsarzy    (1000) xsarzy    (1000)        0 2024-05-01 12:17:06.035191 projectZ-1.1.7.2.1/
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)     1086 2024-05-01 09:25:03.000000 projectZ-1.1.7.2.1/LICENSE.txt
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)     2910 2024-05-01 12:17:06.035191 projectZ-1.1.7.2.1/PKG-INFO
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)     2416 2024-04-30 21:29:39.000000 projectZ-1.1.7.2.1/README.md
+drwxr-xr-x   0 xsarzy    (1000) xsarzy    (1000)        0 2024-05-01 12:17:06.035191 projectZ-1.1.7.2.1/projectZ/
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)      595 2024-05-01 12:14:44.000000 projectZ-1.1.7.2.1/projectZ/__init__.py
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)    15835 2024-05-01 12:11:05.000000 projectZ-1.1.7.2.1/projectZ/async_client.py
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)    15159 2024-05-01 12:10:09.000000 projectZ-1.1.7.2.1/projectZ/client.py
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)     4403 2024-05-01 10:03:10.000000 projectZ-1.1.7.2.1/projectZ/requests_builder.py
+drwxr-xr-x   0 xsarzy    (1000) xsarzy    (1000)        0 2024-05-01 12:17:06.035191 projectZ-1.1.7.2.1/projectZ/utils/
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)        0 2024-04-30 21:29:39.000000 projectZ-1.1.7.2.1/projectZ/utils/__init__.py
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)     2017 2024-05-01 10:04:41.000000 projectZ-1.1.7.2.1/projectZ/utils/exceptions.py
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)      865 2024-04-30 21:29:39.000000 projectZ-1.1.7.2.1/projectZ/utils/generator.py
+drwxr-xr-x   0 xsarzy    (1000) xsarzy    (1000)        0 2024-05-01 12:17:06.035191 projectZ-1.1.7.2.1/projectZ.egg-info/
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)     2910 2024-05-01 12:17:05.000000 projectZ-1.1.7.2.1/projectZ.egg-info/PKG-INFO
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)      377 2024-05-01 12:17:05.000000 projectZ-1.1.7.2.1/projectZ.egg-info/SOURCES.txt
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)        1 2024-05-01 12:17:05.000000 projectZ-1.1.7.2.1/projectZ.egg-info/dependency_links.txt
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)       49 2024-05-01 12:17:05.000000 projectZ-1.1.7.2.1/projectZ.egg-info/requires.txt
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)        9 2024-05-01 12:17:05.000000 projectZ-1.1.7.2.1/projectZ.egg-info/top_level.txt
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)       38 2024-05-01 12:17:06.035191 projectZ-1.1.7.2.1/setup.cfg
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)      905 2024-05-01 12:16:49.000000 projectZ-1.1.7.2.1/setup.py
```

### Comparing `projectZ-1.1.7.2/PKG-INFO` & `projectZ-1.1.7.2.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,61 @@
 Metadata-Version: 2.1
 Name: projectZ
-Version: 1.1.7.2
+Version: 1.1.7.2.1
 Summary: Library for creating projectZ bots and scripts.
 Home-page: https://github.com/xXxCLOTIxXx/projectZ.py
 Download-URL: https://github.com/xXxCLOTIxXx/projectZ.py/archive/refs/heads/main.zip
 Author: Xsarz
 Author-email: xsarzy@gmail.com
 License: MIT
 Keywords: projectZ.py,projectZ,projectZ-py,projectZ-bot,api,python,python3,python3.x,xsarz,official,async,sync,projz
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 
-<table align="center">
-	<tr> <th colspan="3">Library Information</th> </tr>
-	<tr>
-		<td>
-			<a href='https://projectzpy.readthedocs.io/en/latest/'><img src="https://pbs.twimg.com/profile_images/525686734760067072/OhsWgbsr_400x400.png" height="30px">
-			 Library Documentation</a>
-		</td>
-		<td>
-			<a href='https://github.com/xXxCLOTIxXx/projectZ.py'><img src="https://upload.wikimedia.org/wikipedia/commons/9/91/Octicons-mark-github.svg" height="30px">
-			 GitHub</a>
-		</td>
-</table>
-<table align="center">
-	</tr>
-	<tr> <th colspan="3">More info</th> </tr>
-	<tr>
-		<td>
-			<a href="https://t.me/DxsarzUnion"><img src="https://upload.wikimedia.org/wikipedia/commons/8/82/Telegram_logo.svg" height="30px">
-			 Telegram Channel</a>
-		</td>
-		<td>
-			<a href="https://www.youtube.com/channel/UCNKEgQmAvt6dD7jeMLpte9Q"><img src="https://upload.wikimedia.org/wikipedia/commons/0/09/YouTube_full-color_icon_%282017%29.svg" height="30px">
-			 YouTube channel</a>
-		</td>
-		<td>
-			<a href="https://discord.gg/GtpUnsHHT4"><img src="https://www.svgrepo.com/show/353655/discord-icon.svg" height="30px">
-			 Discord Server</a>
-		</td>
-	</tr>
-</table>
+<body>
+	<p align="center">
+	    <a href="https://github.com/xXxCLOTIxXx/projectZ.py/releases"><img src="https://img.shields.io/github/v/release/xXxCLOTIxXx/projectZ.py" alt="GitHub release" />
+	    <a href="https://github.com/xXxCLOTIxXx/projectZ.py/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="licence" /></a>
+	    <a href="https://pypi.org/project/projectZ/"><img src="https://img.shields.io/pypi/v/projectZ" alt="pypi" /></a>
+	    <a href="https://github.com/xXxCLOTIxXx/projectZ.py/blob/main/docs/main.md"><img src="https://img.shields.io/website?down_message=failing&label=docs&up_color=green&up_message=passing&url=https://github.com/xXxCLOTIxXx/projectZ.py/blob/main/docs/main.md" alt="docs" /></a>
+	</p>
+	<div align="center">
+		<a href="https://github.com/xXxCLOTIxXx/xXxCLOTIxXx/blob/main/sponsor.md">
+			<img src="https://img.shields.io/static/v1?style=for-the-badge&label=Sponsor project&message=%E2%9D%A4&color=ff69b4" alt="Sponsor project"/>
+		</a>
+	</div>
+	<table align="center">
+		</tr>
+		<tr> <th colspan="3">More info</th> </tr>
+		<tr>
+			<td>
+				<a href="https://t.me/DxsarzUnion"><img src="https://upload.wikimedia.org/wikipedia/commons/8/82/Telegram_logo.svg" height="30px">
+				 Telegram Channel</a>
+			</td>
+			<td>
+				<a href="https://www.youtube.com/channel/UCNKEgQmAvt6dD7jeMLpte9Q"><img src="https://upload.wikimedia.org/wikipedia/commons/0/09/YouTube_full-color_icon_%282017%29.svg" height="30px">
+				 YouTube channel</a>
+			</td>
+			<td>
+				<a href="https://discord.gg/GtpUnsHHT4"><img src="https://www.svgrepo.com/show/353655/discord-icon.svg" height="30px">
+				 Discord Server</a>
+			</td>
+		</tr>
+	</table>
 <h1 align="center">projectZ.py</h1>
-<p align="center">Library for working with projectZ servers, below you will see code examples, for more examples see the documentation or the examples folder</p>
+		    
+```bash
+pip install projectZ
+```
+<h4 align="center">or</h4>
+		    
+```bash
+pip install git+https://github.com/xXxCLOTIxXx/projectZ.py.git
+```
+<p align="center">Library for working with projectZ servers, below you will see code examples</p>
 <h1 align="center">Login example</h1>
 
 ```python
 import projectZ
 
 client = projectZ.Client()
 client.login(email='email', password='password')
@@ -62,7 +72,9 @@
 async def main():
 	await client.login(email='email', password='password')
 
 if __name__ == '__main__':
 	loop = asyncio.get_event_loop()
 	loop.run_until_complete(main())
 ```
+
+</body>
```

### Comparing `projectZ-1.1.7.2/README.md` & `projectZ-1.1.7.2.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,48 @@
-<table align="center">
-	<tr> <th colspan="3">Library Information</th> </tr>
-	<tr>
-		<td>
-			<a href='https://projectzpy.readthedocs.io/en/latest/'><img src="https://pbs.twimg.com/profile_images/525686734760067072/OhsWgbsr_400x400.png" height="30px">
-			 Library Documentation</a>
-		</td>
-		<td>
-			<a href='https://github.com/xXxCLOTIxXx/projectZ.py'><img src="https://upload.wikimedia.org/wikipedia/commons/9/91/Octicons-mark-github.svg" height="30px">
-			 GitHub</a>
-		</td>
-</table>
-<table align="center">
-	</tr>
-	<tr> <th colspan="3">More info</th> </tr>
-	<tr>
-		<td>
-			<a href="https://t.me/DxsarzUnion"><img src="https://upload.wikimedia.org/wikipedia/commons/8/82/Telegram_logo.svg" height="30px">
-			 Telegram Channel</a>
-		</td>
-		<td>
-			<a href="https://www.youtube.com/channel/UCNKEgQmAvt6dD7jeMLpte9Q"><img src="https://upload.wikimedia.org/wikipedia/commons/0/09/YouTube_full-color_icon_%282017%29.svg" height="30px">
-			 YouTube channel</a>
-		</td>
-		<td>
-			<a href="https://discord.gg/GtpUnsHHT4"><img src="https://www.svgrepo.com/show/353655/discord-icon.svg" height="30px">
-			 Discord Server</a>
-		</td>
-	</tr>
-</table>
+<body>
+	<p align="center">
+	    <a href="https://github.com/xXxCLOTIxXx/projectZ.py/releases"><img src="https://img.shields.io/github/v/release/xXxCLOTIxXx/projectZ.py" alt="GitHub release" />
+	    <a href="https://github.com/xXxCLOTIxXx/projectZ.py/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="licence" /></a>
+	    <a href="https://pypi.org/project/projectZ/"><img src="https://img.shields.io/pypi/v/projectZ" alt="pypi" /></a>
+	    <a href="https://github.com/xXxCLOTIxXx/projectZ.py/blob/main/docs/main.md"><img src="https://img.shields.io/website?down_message=failing&label=docs&up_color=green&up_message=passing&url=https://github.com/xXxCLOTIxXx/projectZ.py/blob/main/docs/main.md" alt="docs" /></a>
+	</p>
+	<div align="center">
+		<a href="https://github.com/xXxCLOTIxXx/xXxCLOTIxXx/blob/main/sponsor.md">
+			<img src="https://img.shields.io/static/v1?style=for-the-badge&label=Sponsor project&message=%E2%9D%A4&color=ff69b4" alt="Sponsor project"/>
+		</a>
+	</div>
+	<table align="center">
+		</tr>
+		<tr> <th colspan="3">More info</th> </tr>
+		<tr>
+			<td>
+				<a href="https://t.me/DxsarzUnion"><img src="https://upload.wikimedia.org/wikipedia/commons/8/82/Telegram_logo.svg" height="30px">
+				 Telegram Channel</a>
+			</td>
+			<td>
+				<a href="https://www.youtube.com/channel/UCNKEgQmAvt6dD7jeMLpte9Q"><img src="https://upload.wikimedia.org/wikipedia/commons/0/09/YouTube_full-color_icon_%282017%29.svg" height="30px">
+				 YouTube channel</a>
+			</td>
+			<td>
+				<a href="https://discord.gg/GtpUnsHHT4"><img src="https://www.svgrepo.com/show/353655/discord-icon.svg" height="30px">
+				 Discord Server</a>
+			</td>
+		</tr>
+	</table>
 <h1 align="center">projectZ.py</h1>
-<p align="center">Library for working with projectZ servers, below you will see code examples, for more examples see the documentation or the examples folder</p>
+		    
+```bash
+pip install projectZ
+```
+<h4 align="center">or</h4>
+		    
+```bash
+pip install git+https://github.com/xXxCLOTIxXx/projectZ.py.git
+```
+<p align="center">Library for working with projectZ servers, below you will see code examples</p>
 <h1 align="center">Login example</h1>
 
 ```python
 import projectZ
 
 client = projectZ.Client()
 client.login(email='email', password='password')
@@ -49,8 +58,10 @@
 client = projectZ.AsyncClient()
 async def main():
 	await client.login(email='email', password='password')
 
 if __name__ == '__main__':
 	loop = asyncio.get_event_loop()
 	loop.run_until_complete(main())
-```
+```
+
+</body>
```

### Comparing `projectZ-1.1.7.2/projectZ/__init__.py` & `projectZ-1.1.7.2.1/projectZ/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 from .ws.async_socket import AsyncSocket
 
 from .objects.constants import (
     LoggerLevel
 )
 from .objects.MediaTargets import MediaTargets
 from .objects.ChatMessageTypes import ChatMessageTypes
+from .objects.ws_types import WsMethods
 
 
 import projectZ.utils.exceptions as exceptions
 from .utils.generator import gen_signature, gen_deviceId
 
 __title__ = 'projectZ.py'
 __author__ = 'Xsarz'
 __license__ = 'MIT'
-__copyright__ = 'Copyright 2024 Xsarz'
-__version__ = '1.1.7.2'
+__copyright__ = 'Copyright 2023-2024 Xsarz'
+__version__ = '1.1.7.2.1'
```

### Comparing `projectZ-1.1.7.2/projectZ/async_client.py` & `projectZ-1.1.7.2.1/projectZ/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from sys import maxsize
 from random import randint
-from typing import Union, Optional
 from aiofiles.threadpool.binary import AsyncBufferedReader
 from aiohttp import MultipartWriter
-from magic import from_buffer
+from mimetypes import guess_type
+from typing import Union
 
 from .ws.async_socket import AsyncSocket
 from .requests_builder import AsyncRequester
 from .objects.profile import profile
 from .objects.objects import *
 from .objects.constants import LoggerLevel, ws_endpoint
 from .objects.ChatMessageTypes import ChatMessageTypes
@@ -36,19 +36,19 @@
 		return self.req.profile.sid
 
 	@property
 	def deviceId(self):
 		return self.req.profile.deviceId
 
 
-	async def upload_media(self, file: Union[bytes, AsyncBufferedReader], target: int, duration: int = 0) -> Media:
-		file_content = await file.read() if isinstance(file, AsyncBufferedReader) else file
+	async def upload_media(self, file: AsyncBufferedReader, target: int, duration: int = 0) -> Media:
+		file_content = await file.read()
 		writer = MultipartWriter()
-		part = writer.append(file_content, {"Content-Type": from_buffer(file_content, mime=True)})
-		part.set_content_disposition("form-data", name="media", filename=file.name if isinstance(file, AsyncBufferedReader) else "file")
+		part = writer.append(file_content, {"Content-Type": guess_type(file.name)[0]})
+		part.set_content_disposition("form-data", name="media", filename=file.name)
 		return Media(await self.req.request("POST", f"/v1/media/upload?target={target}&duration={duration}", writer, content_type=f"multipart/form-data; boundary={writer.boundary}"))
 
 
 	async def login(self, email: str, password: str) -> User:
 		result = User(await self.req.request("POST", "/v1/auth/login", {
 			"password":password,
 			"email":email,
@@ -100,33 +100,44 @@
 		return FromLink(await self.req.request("POST", f"/v1/links/share"))
 
 
 	async def get_my_chats(self, start: int = 0, size: int = 20, type: str = 'managed'):	
 		return Thread(await self.req.request("GET", f"/v1/chat/joined-threads?start={start}&size={size}&type={type}"))
 
 
-	async def send_message(self, chatId: int, message: str = None, media: Media = None, audio: Media = None, message_type: int = ChatMessageTypes.TEXT, replyTo: int = None, pollId: int = None, diceId: int = None) -> None:
+	async def send_message(self, chatId: int, message: str = None, media: Media = None, message_type: int = ChatMessageTypes.TEXT, replyTo: int = None, pollId: int = None, diceId: int = None) -> None:
 		data = {
 			"type": message_type,
 			"threadId": chatId,
 			"uid": self.req.profile.uid,
 			"seqId": randint(0, maxsize),
 			"extensions": {}
 		}
-		if message:data["content"] = message
-		if replyTo: data["extensions"]["replyMessageId"] = replyTo
-		if media: data["media"] = media.json
-		elif audio: data["media"] = audio.json
+		if message:
+			data["content"] = message
+			if replyTo: data["extensions"]["replyMessageId"] = replyTo
+		elif media: data["media"] = media.json
 		if pollId: data["extensions"]["pollId"] = pollId
 		if diceId: data["extensions"]["diceId"] = diceId
-		await self.ws_send(req_t=message_type, **dict(threadId=chatId, msg=data))
+		await self.ws_send(req_t=1, **dict(threadId=chatId, msg=data))
 
+	async def send_text_message(self, chatId: int, message: str) -> None:
+		await self.send_message(chatId=chatId, message=message, message_type=ChatMessageTypes.TEXT)
+
+	async def send_audio_message(self, chatId: int, audio: Media) -> None:
+		await self.send_message(chatId=chatId, media=audio, message_type=ChatMessageTypes.AUDIO)
+
+	async def send_image_message(self, chatId: int, image: Media) -> None:
+		await self.send_message(chatId=chatId, media=image, message_type=ChatMessageTypes.MEDIA)
+
+	async def send_video_message(self, chatId: int, video: Media) -> None:
+		await self.send_message(chatId=chatId, media=video, message_type=ChatMessageTypes.VIDEO)
 
 	async def typing(self, chatId: int) -> None:
-		await self.send_message(chatId=chatId, message_type=60)
+		await self.send_message(chatId=chatId, message_type=ChatMessageTypes.TYPING)
 
 
 	async def visit(self, userId) -> dict:
 		return await self.req.request("POST", f"/v1/users/profile/{userId}/visit")
 	
 
 	async def activate_wallet(self, email: str, wallet_password: str, code: str) -> dict:
@@ -365,7 +376,19 @@
 			"flagType": flagType,
 			"message": message,
 		}
 		for image in images:
 			media.append(image.json)
 		data["mediaList"] = media
 		return await self.req.request("POST", f'/v1/flags', data)
+
+	async def get_my_companion(self) -> dict:
+		return await self.req.request("GET", f'/v1/companion')
+
+	async def set_companion(self, nftId: int) -> dict:
+		return await self.req.request("POST", f'/v1/companion', {"nftId": nftId})
+
+	async def get_build_in_companions(self, size: int = 10) -> dict:
+		return await self.req.request("GET", f'/biz/v1/build-in-character-list?size={size}')
+
+	async def get_nft_info(self, nftId: int) -> dict:
+		return await self.req.request("GET", f'/biz/v1/nft/{nftId}')
```

### Comparing `projectZ-1.1.7.2/projectZ/client.py` & `projectZ-1.1.7.2.1/projectZ/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from sys import maxsize
 from random import randint
-from typing import Union
+from typing import Union, BinaryIO
+from requests_toolbelt.multipart.encoder import MultipartEncoder
+from mimetypes import guess_type
 
 from .ws.socket import Socket
 from .requests_builder import requester
 from .objects.profile import profile
 from .objects.objects import *
 from .objects.constants import LoggerLevel, ws_endpoint
 from .objects.ChatMessageTypes import ChatMessageTypes
@@ -32,14 +34,21 @@
 		return self.req.profile.sid
 
 	@property
 	def deviceId(self):
 		return self.req.profile.deviceId
 
 
+	def upload_media(self, file: BinaryIO, target: int, duration: int = 0) -> Media:
+		data = MultipartEncoder({
+        	'media': (file.name, file.read(), guess_type(file.name)[0])
+   		 })
+		return Media(self.req.request("POST", f"/v1/media/upload?target={target}&duration={duration}", data, content_type=data.content_type))
+
+
 	def login(self, email: str, password: str) -> User:
 		result = User(self.req.request("POST", "/v1/auth/login", {
 			"password":password,
 			"email":email,
 			"authType":1
 		}))
 		self.req.profile.sid, self.req.profile.uid = result.sid, result.uid
@@ -86,33 +95,44 @@
 		return FromLink(self.req.request("POST", f"/v1/links/share"))
 
 
 	def get_my_chats(self, start: int = 0, size: int = 20, type: str = 'managed'):	
 		return Thread(self.req.request("GET", f"/v1/chat/joined-threads?start={start}&size={size}&type={type}"))
 
 
-	def send_message(self, chatId: int, message: str = None, media: Media = None, audio: Media = None, message_type: int = ChatMessageTypes.TEXT, replyTo: int = None, pollId: int = None, diceId: int = None) -> None:
+	def send_message(self, chatId: int, message: str = None, media: Media = None, message_type: int = ChatMessageTypes.TEXT, replyTo: int = None, pollId: int = None, diceId: int = None) -> None:
 		data = {
 			"type": message_type,
 			"threadId": chatId,
 			"uid": self.req.profile.uid,
 			"seqId": randint(0, maxsize),
 			"extensions": {}
 		}
-		if message:data["content"] = message
-		if media: data["media"] = media.json
-		elif audio: data["media"] = audio.json
-		if replyTo: data["extensions"]["replyMessageId"] = replyTo
+		if message:
+			data["content"] = message
+			if replyTo: data["extensions"]["replyMessageId"] = replyTo
+		elif media: data["media"] = media.json
 		if pollId: data["extensions"]["pollId"] = pollId
 		if diceId: data["extensions"]["diceId"] = diceId
-		self.ws_send(req_t=message_type, **dict(threadId=chatId, msg=data))
+		self.ws_send(req_t=1, **dict(threadId=chatId, msg=data))
+
+	def send_text_message(self, chatId: int, message: str) -> None:
+		self.send_message(chatId=chatId, message=message, message_type=ChatMessageTypes.TEXT)
+
+	def send_audio_message(self, chatId: int, audio: Media) -> None:
+		self.send_message(chatId=chatId, media=audio, message_type=ChatMessageTypes.AUDIO)
 
+	def send_image_message(self, chatId: int, image: Media) -> None:
+		self.send_message(chatId=chatId, media=image, message_type=ChatMessageTypes.MEDIA)
+
+	def send_video_message(self, chatId: int, video: Media) -> None:
+		self.send_message(chatId=chatId, media=video, message_type=ChatMessageTypes.VIDEO)
 
 	def typing(self, chatId: int) -> None:
-		self.send_message(chatId=chatId, message_type=60)
+		self.send_message(chatId=chatId, message_type=ChatMessageTypes.TYPING)
 
 
 	def visit(self, userId) -> dict:
 		return self.req.request("POST", f"/v1/users/profile/{userId}/visit")
 	
 
 	def activate_wallet(self, email: str, wallet_password: str, code: str) -> dict:
@@ -333,8 +353,37 @@
 	def get_user_tasks(self) -> dict:
 		return self.req.request("GET", f'/v2/user-tasks')
 
 	def get_my_gifts(self, size: int = 60) -> Gifts:
 		return Gifts(self.req.request("GET", f"/biz/v2/transfer-orders?size={size}"))
 
 	def gift_withdrawn(self, orderId) -> dict:
-		return self.req.request("GET", f'/biz/v1/gift-boxes/{orderId}/withdrawn')
+		return self.req.request("GET", f'/biz/v1/gift-boxes/{orderId}/withdrawn')
+
+	def report(self, userId: int, message: str, images: Union[Media, list[Media]], flagType: int = 100) -> dict:
+
+		media = list()
+		if isinstance(images, Media):images=[images]
+		elif isinstance(images, list):pass
+		else:raise WrongType()
+		data = {
+			"objectId": userId,
+			"objectType": 4,
+			"flagType": flagType,
+			"message": message,
+		}
+		for image in images:
+			media.append(image.json)
+		data["mediaList"] = media
+		return self.req.request("POST", f'/v1/flags', data)
+
+	def get_my_companion(self) -> dict:
+		return self.req.request("GET", f'/v1/companion')
+
+	def set_companion(self, nftId: int) -> dict:
+		return self.req.request("POST", f'/v1/companion', {"nftId": nftId})
+
+	def get_build_in_companions(self, size: int = 10) -> dict:
+		return self.req.request("GET", f'/biz/v1/build-in-character-list?size={size}')
+
+	def get_nft_info(self, nftId: int) -> dict:
+		return self.req.request("GET", f'/biz/v1/nft/{nftId}')
```

### Comparing `projectZ-1.1.7.2/projectZ/requests_builder.py` & `projectZ-1.1.7.2.1/projectZ/requests_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Optional, Union
 from requests import Session
+from requests_toolbelt.multipart.encoder import MultipartEncoder
 from aiohttp import ClientSession, MultipartWriter
 from io import BytesIO
 from ujson import dumps
 from time import time
 from uuid import uuid4
 from ujson import loads
 
@@ -24,14 +25,15 @@
 
 	def request(self, method: str, endpoint: str, body: Union[bytes, str, dict] = None, content_type: Optional[str] = "application/json; charset=UTF-8", web: bool = False, successful_code: int = 200) -> dict:
 		if not endpoint.startswith("/"): endpoint = f"/{endpoint}"
 		if web: endpoint = f"/api/f{endpoint}"
 		if body:
 			content = BytesIO()
 			if isinstance(body, bytes): content.write(body)
+			elif isinstance(body, MultipartEncoder): content.write(body.to_string())
 			elif isinstance(body, str): content.write(body.encode("utf-8"))
 			elif isinstance(body, dict): content.write(dumps(body).encode("utf-8"))
 			else: raise ValueError(f"Invalid request body type: \"{body.__class__.__name__}\"")
 			body = content.getvalue()
 		result = self.session.request(method, f"{web_api_url if web else api_url}{endpoint}", data=body, headers=self.build_headers(
 			endpoint=endpoint,
 			body=body,
```

### Comparing `projectZ-1.1.7.2/projectZ/utils/exceptions.py` & `projectZ-1.1.7.2.1/projectZ/utils/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,21 +54,26 @@
 
 
 class WalletNotActivated(Exception):
 	def __init__(*args, **kwargs):
 		Exception.__init__(*args, **kwargs)
 
 
+class UnsupportedMediaFormat(Exception):
+	def __init__(*args, **kwargs):
+		Exception.__init__(*args, **kwargs)
+
 errors = {
 	2009: EmailNotRegistered,
 	2022: InvalidEmail,
 	4604: InvalidLink,
 	2010: IncorrectPassword,
 	2038: AlreadyRegistered,
 	6107: TooManyRequests,
+	7002: UnsupportedMediaFormat,
 	7008: BadMedia,
 	1000004: NoWalletError,
 	1000108: WalletNotActivated
 }
 
 def CheckException(data):
 	try:
```

### Comparing `projectZ-1.1.7.2/projectZ/utils/generator.py` & `projectZ-1.1.7.2.1/projectZ/utils/generator.py`

 * *Files identical despite different names*

### Comparing `projectZ-1.1.7.2/projectZ.egg-info/PKG-INFO` & `projectZ-1.1.7.2.1/projectZ.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,61 @@
 Metadata-Version: 2.1
 Name: projectZ
-Version: 1.1.7.2
+Version: 1.1.7.2.1
 Summary: Library for creating projectZ bots and scripts.
 Home-page: https://github.com/xXxCLOTIxXx/projectZ.py
 Download-URL: https://github.com/xXxCLOTIxXx/projectZ.py/archive/refs/heads/main.zip
 Author: Xsarz
 Author-email: xsarzy@gmail.com
 License: MIT
 Keywords: projectZ.py,projectZ,projectZ-py,projectZ-bot,api,python,python3,python3.x,xsarz,official,async,sync,projz
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 
-<table align="center">
-	<tr> <th colspan="3">Library Information</th> </tr>
-	<tr>
-		<td>
-			<a href='https://projectzpy.readthedocs.io/en/latest/'><img src="https://pbs.twimg.com/profile_images/525686734760067072/OhsWgbsr_400x400.png" height="30px">
-			 Library Documentation</a>
-		</td>
-		<td>
-			<a href='https://github.com/xXxCLOTIxXx/projectZ.py'><img src="https://upload.wikimedia.org/wikipedia/commons/9/91/Octicons-mark-github.svg" height="30px">
-			 GitHub</a>
-		</td>
-</table>
-<table align="center">
-	</tr>
-	<tr> <th colspan="3">More info</th> </tr>
-	<tr>
-		<td>
-			<a href="https://t.me/DxsarzUnion"><img src="https://upload.wikimedia.org/wikipedia/commons/8/82/Telegram_logo.svg" height="30px">
-			 Telegram Channel</a>
-		</td>
-		<td>
-			<a href="https://www.youtube.com/channel/UCNKEgQmAvt6dD7jeMLpte9Q"><img src="https://upload.wikimedia.org/wikipedia/commons/0/09/YouTube_full-color_icon_%282017%29.svg" height="30px">
-			 YouTube channel</a>
-		</td>
-		<td>
-			<a href="https://discord.gg/GtpUnsHHT4"><img src="https://www.svgrepo.com/show/353655/discord-icon.svg" height="30px">
-			 Discord Server</a>
-		</td>
-	</tr>
-</table>
+<body>
+	<p align="center">
+	    <a href="https://github.com/xXxCLOTIxXx/projectZ.py/releases"><img src="https://img.shields.io/github/v/release/xXxCLOTIxXx/projectZ.py" alt="GitHub release" />
+	    <a href="https://github.com/xXxCLOTIxXx/projectZ.py/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="licence" /></a>
+	    <a href="https://pypi.org/project/projectZ/"><img src="https://img.shields.io/pypi/v/projectZ" alt="pypi" /></a>
+	    <a href="https://github.com/xXxCLOTIxXx/projectZ.py/blob/main/docs/main.md"><img src="https://img.shields.io/website?down_message=failing&label=docs&up_color=green&up_message=passing&url=https://github.com/xXxCLOTIxXx/projectZ.py/blob/main/docs/main.md" alt="docs" /></a>
+	</p>
+	<div align="center">
+		<a href="https://github.com/xXxCLOTIxXx/xXxCLOTIxXx/blob/main/sponsor.md">
+			<img src="https://img.shields.io/static/v1?style=for-the-badge&label=Sponsor project&message=%E2%9D%A4&color=ff69b4" alt="Sponsor project"/>
+		</a>
+	</div>
+	<table align="center">
+		</tr>
+		<tr> <th colspan="3">More info</th> </tr>
+		<tr>
+			<td>
+				<a href="https://t.me/DxsarzUnion"><img src="https://upload.wikimedia.org/wikipedia/commons/8/82/Telegram_logo.svg" height="30px">
+				 Telegram Channel</a>
+			</td>
+			<td>
+				<a href="https://www.youtube.com/channel/UCNKEgQmAvt6dD7jeMLpte9Q"><img src="https://upload.wikimedia.org/wikipedia/commons/0/09/YouTube_full-color_icon_%282017%29.svg" height="30px">
+				 YouTube channel</a>
+			</td>
+			<td>
+				<a href="https://discord.gg/GtpUnsHHT4"><img src="https://www.svgrepo.com/show/353655/discord-icon.svg" height="30px">
+				 Discord Server</a>
+			</td>
+		</tr>
+	</table>
 <h1 align="center">projectZ.py</h1>
-<p align="center">Library for working with projectZ servers, below you will see code examples, for more examples see the documentation or the examples folder</p>
+		    
+```bash
+pip install projectZ
+```
+<h4 align="center">or</h4>
+		    
+```bash
+pip install git+https://github.com/xXxCLOTIxXx/projectZ.py.git
+```
+<p align="center">Library for working with projectZ servers, below you will see code examples</p>
 <h1 align="center">Login example</h1>
 
 ```python
 import projectZ
 
 client = projectZ.Client()
 client.login(email='email', password='password')
@@ -62,7 +72,9 @@
 async def main():
 	await client.login(email='email', password='password')
 
 if __name__ == '__main__':
 	loop = asyncio.get_event_loop()
 	loop.run_until_complete(main())
 ```
+
+</body>
```

### Comparing `projectZ-1.1.7.2/setup.py` & `projectZ-1.1.7.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from platform import system
 
 with open("README.md", "r") as file:
 	long_description = file.read()
 
 link = 'https://github.com/xXxCLOTIxXx/projectZ.py/archive/refs/heads/main.zip'
-ver = '1.1.7.2'
+ver = '1.1.7.2.1'
 
 setup(
 	name = "projectZ",
 	version = ver,
 	url = "https://github.com/xXxCLOTIxXx/projectZ.py",
 	download_url = link,
 	license = "MIT",
@@ -34,12 +34,11 @@
 		"projz"
 	],
 	install_requires = [
 		"websocket-client",
 		"requests",
 		"aiohttp",
 		"aiofiles",
-		"ujson",
-		"python-magic-bin" if system().lower() == "windows" else "python-magic"
+		"ujson"
 	],
 	packages = find_packages()
 )
```

