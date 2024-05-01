# Comparing `tmp/SberQR-2.0.0.tar.gz` & `tmp/SberQR-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SberQR-2.0.0.tar", last modified: Mon Jan 22 10:42:10 2024, max compression
+gzip compressed data, was "SberQR-2.0.1.tar", last modified: Wed May  1 10:46:29 2024, max compression
```

## Comparing `SberQR-2.0.0.tar` & `SberQR-2.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 10:42:10.781795 SberQR-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-01-22 10:42:02.000000 SberQR-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9947 2024-01-22 10:42:10.781795 SberQR-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8928 2024-01-22 10:42:02.000000 SberQR-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 10:42:10.781795 SberQR-2.0.0/SberQR/
--rw-r--r--   0 runner    (1001) docker     (127)     8050 2024-01-22 10:42:02.000000 SberQR-2.0.0/SberQR/AsyncSberQR.py
--rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-01-22 10:42:02.000000 SberQR-2.0.0/SberQR/SberQr.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-01-22 10:42:02.000000 SberQR-2.0.0/SberQR/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-01-22 10:42:02.000000 SberQR-2.0.0/SberQR/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-01-22 10:42:02.000000 SberQR-2.0.0/SberQR/api_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-01-22 10:42:02.000000 SberQR-2.0.0/SberQR/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-01-22 10:42:02.000000 SberQR-2.0.0/SberQR/payload.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-01-22 10:42:02.000000 SberQR-2.0.0/SberQR/scope.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-01-22 10:42:02.000000 SberQR-2.0.0/SberQR/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 10:42:10.781795 SberQR-2.0.0/SberQR.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9947 2024-01-22 10:42:10.000000 SberQR-2.0.0/SberQR.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-01-22 10:42:10.000000 SberQR-2.0.0/SberQR.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 10:42:10.000000 SberQR-2.0.0/SberQR.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-01-22 10:42:10.000000 SberQR-2.0.0/SberQR.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-22 10:42:10.000000 SberQR-2.0.0/SberQR.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-01-22 10:42:10.781795 SberQR-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-01-22 10:42:02.000000 SberQR-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 10:46:29.732233 SberQR-2.0.1/
+-rw-rw-rw-   0        0        0     1085 2022-05-10 19:34:18.000000 SberQR-2.0.1/LICENSE
+-rw-rw-rw-   0        0        0    10114 2024-05-01 10:46:29.732233 SberQR-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9065 2024-01-22 08:57:47.000000 SberQR-2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 10:46:29.698406 SberQR-2.0.1/SberQR/
+-rw-rw-rw-   0        0        0     8250 2024-01-22 09:43:40.000000 SberQR-2.0.1/SberQR/AsyncSberQR.py
+-rw-rw-rw-   0        0        0     7798 2024-01-22 09:20:53.000000 SberQR-2.0.1/SberQR/SberQr.py
+-rw-rw-rw-   0        0        0      467 2024-05-01 10:37:22.000000 SberQR-2.0.1/SberQR/__init__.py
+-rw-rw-rw-   0        0        0     2684 2024-05-01 10:37:22.000000 SberQR-2.0.1/SberQR/api.py
+-rw-rw-rw-   0        0        0      820 2024-01-22 08:57:47.000000 SberQR-2.0.1/SberQR/api_sync.py
+-rw-rw-rw-   0        0        0       88 2022-09-05 13:25:48.000000 SberQR-2.0.1/SberQR/exceptions.py
+-rw-rw-rw-   0        0        0      387 2022-09-19 11:50:03.000000 SberQR-2.0.1/SberQR/payload.py
+-rw-rw-rw-   0        0        0      353 2022-09-16 13:26:26.000000 SberQR-2.0.1/SberQR/scope.py
+-rw-rw-rw-   0        0        0      185 2022-09-05 12:36:20.000000 SberQR-2.0.1/SberQR/types.py
+drwxrwxrwx   0        0        0        0 2024-05-01 10:46:29.730233 SberQR-2.0.1/SberQR.egg-info/
+-rw-rw-rw-   0        0        0    10114 2024-05-01 10:46:29.000000 SberQR-2.0.1/SberQR.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2024-05-01 10:46:29.000000 SberQR-2.0.1/SberQR.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 10:46:29.000000 SberQR-2.0.1/SberQR.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      111 2024-05-01 10:46:29.000000 SberQR-2.0.1/SberQR.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-01 10:46:29.000000 SberQR-2.0.1/SberQR.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      247 2024-05-01 10:46:29.738752 SberQR-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1340 2024-05-01 10:37:22.000000 SberQR-2.0.1/setup.py
```

### Comparing `SberQR-2.0.0/PKG-INFO` & `SberQR-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,167 +1,167 @@
-Metadata-Version: 2.1
-Name: SberQR
-Version: 2.0.0
-Summary: Библиотека для работы с SberPay QR/Плати QR.
-Home-page: https://github.com/bl4ckm45k/SberQR
-Author: bl4ckm45k
-Author-email: nonpowa@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Framework :: AsyncIO
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Office/Business :: Financial
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: aiohttp>=3.8.4
-Requires-Dist: certifi>=2023.11.17
-Requires-Dist: ujson>=5.9.0
-Requires-Dist: pytz==2022.1
-Requires-Dist: qrcode[pil]>=7.3.1
-Requires-Dist: redis>=4.2.0rc1
-Requires-Dist: urllib3~=2.0.3
-
-![](https://img.shields.io/github/stars/bl4ckm45k/SberQR.svg)
-![](https://img.shields.io/github/forks/bl4ckm45k/SberQR.svg)
-![](https://img.shields.io/github/issues/bl4ckm45k/SberQR.svg)
-[![Supported python versions](https://img.shields.io/pypi/pyversions/SberQR.svg)](https://pypi.python.org/pypi/SberQR)
-[![Downloads](https://img.shields.io/pypi/dm/SberQR.svg?)](https://pypi.python.org/pypi/SberQR)
-[![PyPi Package Version](https://img.shields.io/pypi/v/SberQR)](https://pypi.python.org/pypi/SberQR)
-
-
-
-## Асинхронная и синхронная библиотека для работы с SberPay QR/Плати QR.
-
-Асинхронная и синхронная библиотека для работы с SberPay QR/Плати QR.
-
-Позволяет создавать динамический QR и проверять статус платежа.
-
-> Обязательно передавайте параметр russian_crt, без него не удастся установить SSL соединение с API Сбера
-> 
-> [PEM Сертификат securepayments.sberbank.ru](https://securepayments.sberbank.ru/wiki/doku.php/certificates:add:backend)
-
-> Если при инициализации класса `AsyncSberQR` переданы одинаковые `tid` и `id_qr`, то будет создан
-> платеж через СБП, иначе через ПлатиQR.
-## Пример (async)
-
-```python
-import os
-import asyncio
-from SberQR import AsyncSberQR
-
-member_id = '00000105'  # выдается через почту support@ecom.sberbank.ru
-tid = '24601234'  # ID  терминала/Точки. Получить в ЛК Сбрербанк бизнес на странице Информация о точке
-id_qr = '1000301234'  # Номер наклейки с QR-кодом. Получить в ЛК Сбрербанк бизнес Информация о точке/список оборудования
-client_id = '6e7254e2-6de8-4074-b458-b7238689772b'  # получить на api.developer.sber.ru
-client_secret = '3a0ea8cb-886c-4efa-ac45-e3d36aaba335'  # получить на api.developer.sber.ru
-
-#
-crt_from_pkcs12 = f'{os.getcwd()}/cert.crt'  # Для асинхронной версии требуется распаковать сертификат
-key_from_pkcs12 = f'{os.getcwd()}/private.key'  # Для асинхронной версии требуется распаковать приватный ключ
-pkcs12_password = 'SomeSecret'  # Пароль от файла сертификат. Получается на api.developer.sber.ru
-russian_crt = f'{os.getcwd()}/Cert_CA.pem'  # Сертификат мин.цифры для установления SSL соединения
-# Если требуется передайте аргумент redis=
-# redis = aioredis.from_url("redis://localhost", decode_responses=True)
-# redis = "redis://localhost"
-# Redis используется только для временного хранения токена
-sber_qr = AsyncSberQR(member_id=member_id, id_qr=tid, tid=tid,
-                      client_id=client_id, client_secret=client_secret,
-                      crt_file_path=crt_from_pkcs12, key_file_path=key_from_pkcs12,
-                      pkcs12_password=pkcs12_password,
-                      russian_crt=russian_crt)
-positions = [{"position_name": 'Товар ра 10 рублей',
-              "position_count": 1,
-              "position_sum": 1000,
-              "position_description": 'Какой-то товар за 10 рублей'}
-             ]
-async def creation_qr():
-    data = await sber_qr.creation(description=f'Оплата заказа 3', order_sum=1000, order_number="3", positions=positions)
-    print(data)
-if __name__ == '__main__':
-    asyncio.run(creation_qr())
-```
-
-## Пример (sync)
-
-```python
-import os
-from SberQR import SberQR
-
-member_id = '00000105'  # выдается через почту support@ecom.sberbank.ru
-tid = '24601234'  # ID  терминала/Точки. Получить в ЛК Сбрербанк бизнес на странице Информация о точке
-id_qr = '1000301234'  # Номер наклейки с QR-кодом. Получить в ЛК Сбрербанк бизнес Информация о точке/список оборудования
-client_id = '6e7254e2-6de8-4074-b458-b7238689772b'  # получить на api.developer.sber.ru
-client_secret = '3a0ea8cb-886c-4efa-ac45-e3d36aaba335'  # получить на api.developer.sber.ru
-
-#
-crt_from_pkcs12 = f'{os.getcwd()}/cert.crt'  # Для асинхронной версии требуется распаковать сертификат
-key_from_pkcs12 = f'{os.getcwd()}/private.key'  # Для асинхронной версии требуется распаковать приватный ключ
-pkcs12_password = 'SomeSecret'  # Пароль от файла сертификат. Получается на api.developer.sber.ru
-russian_crt = f'{os.getcwd()}/Cert_CA.pem'  # Сертификат мин.цифры для установления SSL соединения
-# Если требуется передайте аргумент redis=
-# redis = aioredis.from_url("redis://localhost", decode_responses=True)
-# redis = "redis://localhost"
-# Redis используется только для временного хранения токена
-sber_qr = SberQR(member_id=member_id, id_qr=tid, tid=tid,
-                      client_id=client_id, client_secret=client_secret,
-                      crt_file_path=crt_from_pkcs12, key_file_path=key_from_pkcs12,
-                      pkcs12_password=pkcs12_password,
-                      russian_crt=russian_crt)
-positions = [{"position_name": 'Товар ра 10 рублей',
-              "position_count": 1,
-              "position_sum": 1000,
-              "position_description": 'Какой-то товар за 10 рублей'}
-             ]
-def creation_qr():
-    data = sber_qr.creation(description=f'Оплата заказа 3', order_sum=1000, order_number="3", positions=positions)
-    print(data)
-    
-if __name__ == '__main__':
-    creation_qr()
-```
-
-Для работы потребуется получить от банка следующие параметры
-
-```python
-member_id = '00000105'  # выдается через почту support@ecom.sberbank.ru 
-tid = '24601234'  # ID  терминала/Точки. Получить в ЛК Сбрербанк бизнес на странице Информация о точке
-id_qr = '1000301234'  # Номер наклейки с QR-кодом. Получить в ЛК Сбрербанк бизнес Информация о точке/список оборудования
-client_id = '6e7254e2-6de8-4074-b458-b7238689772b'  # получить на api.developer.sber.ru
-client_secret = '3a0ea8cb-886c-4efa-ac45-e3d36aaba335'  # получить на api.developer.sber.ru
-path_crt_from_pkcs12 = 'cert.crt' # Файл сертификат 'key.p12' Получается на api.developer.sber.ru 
-path_key_from_pkcs12 = 'private.key' # Файл сертификат 'key.p12' Получается на api.developer.sber.ru
-pkcs12_password = 'SomeSecret'  # Пароль от файла сертификата. Получается на api.developer.sber.ru
-```
-
-## Распаковка pkcs12 с помощью OpenSSL
-
-[Инструкция от ssl.com](https://www.ssl.com/ru/how-to/export-certificates-private-key-from-pkcs12-file-with-openssl/ "SSL.com") - для Windows обратите внимание на Cygwin в инструкции
-
-```
-Откройте командную строку, перейдите в папку, где лежит архив сертификата с расширением .p12. Выполните команду:
-
-openssl pkcs12 -in <название_архива>.p12 -nodes -nocerts -out private.key
-
-Появится запрос пароля. Введите пароль, который вы вводили при создании приложения, нажмите Enter.
-
-Далее аналогично выполните команду:
-
-openssl pkcs12 -in <название_архива>.p12 -clcerts -nokeys -out client_cert.crt
-
-В итоге вы получите приватный ключ в файле private.key и клиентский сертификат в файле client_cert.crt в папке, где лежит архив сертификата.
-````
-## Ссылки
-Для использования требуется аккаунт Сбер Банк бизнес.
-https://sbi.sberbank.ru:9443/ic/dcb/#/
-
-Далее необходимо Авторизоваться
-https://api.developer.sber.ru/
-
-Процесс подключения описан в инструкции
-https://api.developer.sber.ru/product/PlatiQR/doc/v1/QR_API_doc3
+Metadata-Version: 2.1
+Name: SberQR
+Version: 2.0.1
+Summary: Библиотека для работы с SberPay QR/Плати QR.
+Home-page: https://github.com/bl4ckm45k/SberQR
+Author: bl4ckm45k
+Author-email: nonpowa@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Framework :: AsyncIO
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Office/Business :: Financial
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: aiohttp>=3.8.4
+Requires-Dist: certifi>=2023.11.17
+Requires-Dist: ujson>=5.9.0
+Requires-Dist: pytz==2022.1
+Requires-Dist: qrcode[pil]>=7.3.1
+Requires-Dist: redis>=4.2.0rc1
+Requires-Dist: urllib3~=2.0.3
+
+![](https://img.shields.io/github/stars/bl4ckm45k/SberQR.svg)
+![](https://img.shields.io/github/forks/bl4ckm45k/SberQR.svg)
+![](https://img.shields.io/github/issues/bl4ckm45k/SberQR.svg)
+[![Supported python versions](https://img.shields.io/pypi/pyversions/SberQR.svg)](https://pypi.python.org/pypi/SberQR)
+[![Downloads](https://img.shields.io/pypi/dm/SberQR.svg?)](https://pypi.python.org/pypi/SberQR)
+[![PyPi Package Version](https://img.shields.io/pypi/v/SberQR)](https://pypi.python.org/pypi/SberQR)
+
+
+
+## Асинхронная и синхронная библиотека для работы с SberPay QR/Плати QR.
+
+Асинхронная и синхронная библиотека для работы с SberPay QR/Плати QR.
+
+Позволяет создавать динамический QR и проверять статус платежа.
+
+> Обязательно передавайте параметр russian_crt, без него не удастся установить SSL соединение с API Сбера
+> 
+> [PEM Сертификат securepayments.sberbank.ru](https://securepayments.sberbank.ru/wiki/doku.php/certificates:add:backend)
+
+> Если при инициализации класса `AsyncSberQR` переданы одинаковые `tid` и `id_qr`, то будет создан
+> платеж через СБП, иначе через ПлатиQR.
+## Пример (async)
+
+```python
+import os
+import asyncio
+from SberQR import AsyncSberQR
+
+member_id = '00000105'  # выдается через почту support@ecom.sberbank.ru
+tid = '24601234'  # ID  терминала/Точки. Получить в ЛК Сбрербанк бизнес на странице Информация о точке
+id_qr = '1000301234'  # Номер наклейки с QR-кодом. Получить в ЛК Сбрербанк бизнес Информация о точке/список оборудования
+client_id = '6e7254e2-6de8-4074-b458-b7238689772b'  # получить на api.developer.sber.ru
+client_secret = '3a0ea8cb-886c-4efa-ac45-e3d36aaba335'  # получить на api.developer.sber.ru
+
+#
+crt_from_pkcs12 = f'{os.getcwd()}/cert.crt'  # Для асинхронной версии требуется распаковать сертификат
+key_from_pkcs12 = f'{os.getcwd()}/private.key'  # Для асинхронной версии требуется распаковать приватный ключ
+pkcs12_password = 'SomeSecret'  # Пароль от файла сертификат. Получается на api.developer.sber.ru
+russian_crt = f'{os.getcwd()}/Cert_CA.pem'  # Сертификат мин.цифры для установления SSL соединения
+# Если требуется передайте аргумент redis=
+# redis = aioredis.from_url("redis://localhost", decode_responses=True)
+# redis = "redis://localhost"
+# Redis используется только для временного хранения токена
+sber_qr = AsyncSberQR(member_id=member_id, id_qr=tid, tid=tid,
+                      client_id=client_id, client_secret=client_secret,
+                      crt_file_path=crt_from_pkcs12, key_file_path=key_from_pkcs12,
+                      pkcs12_password=pkcs12_password,
+                      russian_crt=russian_crt)
+positions = [{"position_name": 'Товар ра 10 рублей',
+              "position_count": 1,
+              "position_sum": 1000,
+              "position_description": 'Какой-то товар за 10 рублей'}
+             ]
+async def creation_qr():
+    data = await sber_qr.creation(description=f'Оплата заказа 3', order_sum=1000, order_number="3", positions=positions)
+    print(data)
+if __name__ == '__main__':
+    asyncio.run(creation_qr())
+```
+
+## Пример (sync)
+
+```python
+import os
+from SberQR import SberQR
+
+member_id = '00000105'  # выдается через почту support@ecom.sberbank.ru
+tid = '24601234'  # ID  терминала/Точки. Получить в ЛК Сбрербанк бизнес на странице Информация о точке
+id_qr = '1000301234'  # Номер наклейки с QR-кодом. Получить в ЛК Сбрербанк бизнес Информация о точке/список оборудования
+client_id = '6e7254e2-6de8-4074-b458-b7238689772b'  # получить на api.developer.sber.ru
+client_secret = '3a0ea8cb-886c-4efa-ac45-e3d36aaba335'  # получить на api.developer.sber.ru
+
+#
+crt_from_pkcs12 = f'{os.getcwd()}/cert.crt'  # Для асинхронной версии требуется распаковать сертификат
+key_from_pkcs12 = f'{os.getcwd()}/private.key'  # Для асинхронной версии требуется распаковать приватный ключ
+pkcs12_password = 'SomeSecret'  # Пароль от файла сертификат. Получается на api.developer.sber.ru
+russian_crt = f'{os.getcwd()}/Cert_CA.pem'  # Сертификат мин.цифры для установления SSL соединения
+# Если требуется передайте аргумент redis=
+# redis = aioredis.from_url("redis://localhost", decode_responses=True)
+# redis = "redis://localhost"
+# Redis используется только для временного хранения токена
+sber_qr = SberQR(member_id=member_id, id_qr=tid, tid=tid,
+                      client_id=client_id, client_secret=client_secret,
+                      crt_file_path=crt_from_pkcs12, key_file_path=key_from_pkcs12,
+                      pkcs12_password=pkcs12_password,
+                      russian_crt=russian_crt)
+positions = [{"position_name": 'Товар ра 10 рублей',
+              "position_count": 1,
+              "position_sum": 1000,
+              "position_description": 'Какой-то товар за 10 рублей'}
+             ]
+def creation_qr():
+    data = sber_qr.creation(description=f'Оплата заказа 3', order_sum=1000, order_number="3", positions=positions)
+    print(data)
+    
+if __name__ == '__main__':
+    creation_qr()
+```
+
+Для работы потребуется получить от банка следующие параметры
+
+```python
+member_id = '00000105'  # выдается через почту support@ecom.sberbank.ru 
+tid = '24601234'  # ID  терминала/Точки. Получить в ЛК Сбрербанк бизнес на странице Информация о точке
+id_qr = '1000301234'  # Номер наклейки с QR-кодом. Получить в ЛК Сбрербанк бизнес Информация о точке/список оборудования
+client_id = '6e7254e2-6de8-4074-b458-b7238689772b'  # получить на api.developer.sber.ru
+client_secret = '3a0ea8cb-886c-4efa-ac45-e3d36aaba335'  # получить на api.developer.sber.ru
+path_crt_from_pkcs12 = 'cert.crt' # Файл сертификат 'key.p12' Получается на api.developer.sber.ru 
+path_key_from_pkcs12 = 'private.key' # Файл сертификат 'key.p12' Получается на api.developer.sber.ru
+pkcs12_password = 'SomeSecret'  # Пароль от файла сертификата. Получается на api.developer.sber.ru
+```
+
+## Распаковка pkcs12 с помощью OpenSSL
+
+[Инструкция от ssl.com](https://www.ssl.com/ru/how-to/export-certificates-private-key-from-pkcs12-file-with-openssl/ "SSL.com") - для Windows обратите внимание на Cygwin в инструкции
+
+```
+Откройте командную строку, перейдите в папку, где лежит архив сертификата с расширением .p12. Выполните команду:
+
+openssl pkcs12 -in <название_архива>.p12 -nodes -nocerts -out private.key
+
+Появится запрос пароля. Введите пароль, который вы вводили при создании приложения, нажмите Enter.
+
+Далее аналогично выполните команду:
+
+openssl pkcs12 -in <название_архива>.p12 -clcerts -nokeys -out client_cert.crt
+
+В итоге вы получите приватный ключ в файле private.key и клиентский сертификат в файле client_cert.crt в папке, где лежит архив сертификата.
+````
+## Ссылки
+Для использования требуется аккаунт Сбер Банк бизнес.
+https://sbi.sberbank.ru:9443/ic/dcb/#/
+
+Далее необходимо Авторизоваться
+https://api.developer.sber.ru/
+
+Процесс подключения описан в инструкции
+https://api.developer.sber.ru/product/PlatiQR/doc/v1/QR_API_doc3
```

### Comparing `SberQR-2.0.0/README.md` & `SberQR-2.0.1/README.md`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,138 +1,138 @@
-![](https://img.shields.io/github/stars/bl4ckm45k/SberQR.svg)
-![](https://img.shields.io/github/forks/bl4ckm45k/SberQR.svg)
-![](https://img.shields.io/github/issues/bl4ckm45k/SberQR.svg)
-[![Supported python versions](https://img.shields.io/pypi/pyversions/SberQR.svg)](https://pypi.python.org/pypi/SberQR)
-[![Downloads](https://img.shields.io/pypi/dm/SberQR.svg?)](https://pypi.python.org/pypi/SberQR)
-[![PyPi Package Version](https://img.shields.io/pypi/v/SberQR)](https://pypi.python.org/pypi/SberQR)
-
-
-
-## Асинхронная и синхронная библиотека для работы с SberPay QR/Плати QR.
-
-Асинхронная и синхронная библиотека для работы с SberPay QR/Плати QR.
-
-Позволяет создавать динамический QR и проверять статус платежа.
-
-> Обязательно передавайте параметр russian_crt, без него не удастся установить SSL соединение с API Сбера
-> 
-> [PEM Сертификат securepayments.sberbank.ru](https://securepayments.sberbank.ru/wiki/doku.php/certificates:add:backend)
-
-> Если при инициализации класса `AsyncSberQR` переданы одинаковые `tid` и `id_qr`, то будет создан
-> платеж через СБП, иначе через ПлатиQR.
-## Пример (async)
-
-```python
-import os
-import asyncio
-from SberQR import AsyncSberQR
-
-member_id = '00000105'  # выдается через почту support@ecom.sberbank.ru
-tid = '24601234'  # ID  терминала/Точки. Получить в ЛК Сбрербанк бизнес на странице Информация о точке
-id_qr = '1000301234'  # Номер наклейки с QR-кодом. Получить в ЛК Сбрербанк бизнес Информация о точке/список оборудования
-client_id = '6e7254e2-6de8-4074-b458-b7238689772b'  # получить на api.developer.sber.ru
-client_secret = '3a0ea8cb-886c-4efa-ac45-e3d36aaba335'  # получить на api.developer.sber.ru
-
-#
-crt_from_pkcs12 = f'{os.getcwd()}/cert.crt'  # Для асинхронной версии требуется распаковать сертификат
-key_from_pkcs12 = f'{os.getcwd()}/private.key'  # Для асинхронной версии требуется распаковать приватный ключ
-pkcs12_password = 'SomeSecret'  # Пароль от файла сертификат. Получается на api.developer.sber.ru
-russian_crt = f'{os.getcwd()}/Cert_CA.pem'  # Сертификат мин.цифры для установления SSL соединения
-# Если требуется передайте аргумент redis=
-# redis = aioredis.from_url("redis://localhost", decode_responses=True)
-# redis = "redis://localhost"
-# Redis используется только для временного хранения токена
-sber_qr = AsyncSberQR(member_id=member_id, id_qr=tid, tid=tid,
-                      client_id=client_id, client_secret=client_secret,
-                      crt_file_path=crt_from_pkcs12, key_file_path=key_from_pkcs12,
-                      pkcs12_password=pkcs12_password,
-                      russian_crt=russian_crt)
-positions = [{"position_name": 'Товар ра 10 рублей',
-              "position_count": 1,
-              "position_sum": 1000,
-              "position_description": 'Какой-то товар за 10 рублей'}
-             ]
-async def creation_qr():
-    data = await sber_qr.creation(description=f'Оплата заказа 3', order_sum=1000, order_number="3", positions=positions)
-    print(data)
-if __name__ == '__main__':
-    asyncio.run(creation_qr())
-```
-
-## Пример (sync)
-
-```python
-import os
-from SberQR import SberQR
-
-member_id = '00000105'  # выдается через почту support@ecom.sberbank.ru
-tid = '24601234'  # ID  терминала/Точки. Получить в ЛК Сбрербанк бизнес на странице Информация о точке
-id_qr = '1000301234'  # Номер наклейки с QR-кодом. Получить в ЛК Сбрербанк бизнес Информация о точке/список оборудования
-client_id = '6e7254e2-6de8-4074-b458-b7238689772b'  # получить на api.developer.sber.ru
-client_secret = '3a0ea8cb-886c-4efa-ac45-e3d36aaba335'  # получить на api.developer.sber.ru
-
-#
-crt_from_pkcs12 = f'{os.getcwd()}/cert.crt'  # Для асинхронной версии требуется распаковать сертификат
-key_from_pkcs12 = f'{os.getcwd()}/private.key'  # Для асинхронной версии требуется распаковать приватный ключ
-pkcs12_password = 'SomeSecret'  # Пароль от файла сертификат. Получается на api.developer.sber.ru
-russian_crt = f'{os.getcwd()}/Cert_CA.pem'  # Сертификат мин.цифры для установления SSL соединения
-# Если требуется передайте аргумент redis=
-# redis = aioredis.from_url("redis://localhost", decode_responses=True)
-# redis = "redis://localhost"
-# Redis используется только для временного хранения токена
-sber_qr = SberQR(member_id=member_id, id_qr=tid, tid=tid,
-                      client_id=client_id, client_secret=client_secret,
-                      crt_file_path=crt_from_pkcs12, key_file_path=key_from_pkcs12,
-                      pkcs12_password=pkcs12_password,
-                      russian_crt=russian_crt)
-positions = [{"position_name": 'Товар ра 10 рублей',
-              "position_count": 1,
-              "position_sum": 1000,
-              "position_description": 'Какой-то товар за 10 рублей'}
-             ]
-def creation_qr():
-    data = sber_qr.creation(description=f'Оплата заказа 3', order_sum=1000, order_number="3", positions=positions)
-    print(data)
-    
-if __name__ == '__main__':
-    creation_qr()
-```
-
-Для работы потребуется получить от банка следующие параметры
-
-```python
-member_id = '00000105'  # выдается через почту support@ecom.sberbank.ru 
-tid = '24601234'  # ID  терминала/Точки. Получить в ЛК Сбрербанк бизнес на странице Информация о точке
-id_qr = '1000301234'  # Номер наклейки с QR-кодом. Получить в ЛК Сбрербанк бизнес Информация о точке/список оборудования
-client_id = '6e7254e2-6de8-4074-b458-b7238689772b'  # получить на api.developer.sber.ru
-client_secret = '3a0ea8cb-886c-4efa-ac45-e3d36aaba335'  # получить на api.developer.sber.ru
-path_crt_from_pkcs12 = 'cert.crt' # Файл сертификат 'key.p12' Получается на api.developer.sber.ru 
-path_key_from_pkcs12 = 'private.key' # Файл сертификат 'key.p12' Получается на api.developer.sber.ru
-pkcs12_password = 'SomeSecret'  # Пароль от файла сертификата. Получается на api.developer.sber.ru
-```
-
-## Распаковка pkcs12 с помощью OpenSSL
-
-[Инструкция от ssl.com](https://www.ssl.com/ru/how-to/export-certificates-private-key-from-pkcs12-file-with-openssl/ "SSL.com") - для Windows обратите внимание на Cygwin в инструкции
-
-```
-Откройте командную строку, перейдите в папку, где лежит архив сертификата с расширением .p12. Выполните команду:
-
-openssl pkcs12 -in <название_архива>.p12 -nodes -nocerts -out private.key
-
-Появится запрос пароля. Введите пароль, который вы вводили при создании приложения, нажмите Enter.
-
-Далее аналогично выполните команду:
-
-openssl pkcs12 -in <название_архива>.p12 -clcerts -nokeys -out client_cert.crt
-
-В итоге вы получите приватный ключ в файле private.key и клиентский сертификат в файле client_cert.crt в папке, где лежит архив сертификата.
-````
-## Ссылки
-Для использования требуется аккаунт Сбер Банк бизнес.
-https://sbi.sberbank.ru:9443/ic/dcb/#/
-
-Далее необходимо Авторизоваться
-https://api.developer.sber.ru/
-
-Процесс подключения описан в инструкции
+![](https://img.shields.io/github/stars/bl4ckm45k/SberQR.svg)
+![](https://img.shields.io/github/forks/bl4ckm45k/SberQR.svg)
+![](https://img.shields.io/github/issues/bl4ckm45k/SberQR.svg)
+[![Supported python versions](https://img.shields.io/pypi/pyversions/SberQR.svg)](https://pypi.python.org/pypi/SberQR)
+[![Downloads](https://img.shields.io/pypi/dm/SberQR.svg?)](https://pypi.python.org/pypi/SberQR)
+[![PyPi Package Version](https://img.shields.io/pypi/v/SberQR)](https://pypi.python.org/pypi/SberQR)
+
+
+
+## Асинхронная и синхронная библиотека для работы с SberPay QR/Плати QR.
+
+Асинхронная и синхронная библиотека для работы с SberPay QR/Плати QR.
+
+Позволяет создавать динамический QR и проверять статус платежа.
+
+> Обязательно передавайте параметр russian_crt, без него не удастся установить SSL соединение с API Сбера
+> 
+> [PEM Сертификат securepayments.sberbank.ru](https://securepayments.sberbank.ru/wiki/doku.php/certificates:add:backend)
+
+> Если при инициализации класса `AsyncSberQR` переданы одинаковые `tid` и `id_qr`, то будет создан
+> платеж через СБП, иначе через ПлатиQR.
+## Пример (async)
+
+```python
+import os
+import asyncio
+from SberQR import AsyncSberQR
+
+member_id = '00000105'  # выдается через почту support@ecom.sberbank.ru
+tid = '24601234'  # ID  терминала/Точки. Получить в ЛК Сбрербанк бизнес на странице Информация о точке
+id_qr = '1000301234'  # Номер наклейки с QR-кодом. Получить в ЛК Сбрербанк бизнес Информация о точке/список оборудования
+client_id = '6e7254e2-6de8-4074-b458-b7238689772b'  # получить на api.developer.sber.ru
+client_secret = '3a0ea8cb-886c-4efa-ac45-e3d36aaba335'  # получить на api.developer.sber.ru
+
+#
+crt_from_pkcs12 = f'{os.getcwd()}/cert.crt'  # Для асинхронной версии требуется распаковать сертификат
+key_from_pkcs12 = f'{os.getcwd()}/private.key'  # Для асинхронной версии требуется распаковать приватный ключ
+pkcs12_password = 'SomeSecret'  # Пароль от файла сертификат. Получается на api.developer.sber.ru
+russian_crt = f'{os.getcwd()}/Cert_CA.pem'  # Сертификат мин.цифры для установления SSL соединения
+# Если требуется передайте аргумент redis=
+# redis = aioredis.from_url("redis://localhost", decode_responses=True)
+# redis = "redis://localhost"
+# Redis используется только для временного хранения токена
+sber_qr = AsyncSberQR(member_id=member_id, id_qr=tid, tid=tid,
+                      client_id=client_id, client_secret=client_secret,
+                      crt_file_path=crt_from_pkcs12, key_file_path=key_from_pkcs12,
+                      pkcs12_password=pkcs12_password,
+                      russian_crt=russian_crt)
+positions = [{"position_name": 'Товар ра 10 рублей',
+              "position_count": 1,
+              "position_sum": 1000,
+              "position_description": 'Какой-то товар за 10 рублей'}
+             ]
+async def creation_qr():
+    data = await sber_qr.creation(description=f'Оплата заказа 3', order_sum=1000, order_number="3", positions=positions)
+    print(data)
+if __name__ == '__main__':
+    asyncio.run(creation_qr())
+```
+
+## Пример (sync)
+
+```python
+import os
+from SberQR import SberQR
+
+member_id = '00000105'  # выдается через почту support@ecom.sberbank.ru
+tid = '24601234'  # ID  терминала/Точки. Получить в ЛК Сбрербанк бизнес на странице Информация о точке
+id_qr = '1000301234'  # Номер наклейки с QR-кодом. Получить в ЛК Сбрербанк бизнес Информация о точке/список оборудования
+client_id = '6e7254e2-6de8-4074-b458-b7238689772b'  # получить на api.developer.sber.ru
+client_secret = '3a0ea8cb-886c-4efa-ac45-e3d36aaba335'  # получить на api.developer.sber.ru
+
+#
+crt_from_pkcs12 = f'{os.getcwd()}/cert.crt'  # Для асинхронной версии требуется распаковать сертификат
+key_from_pkcs12 = f'{os.getcwd()}/private.key'  # Для асинхронной версии требуется распаковать приватный ключ
+pkcs12_password = 'SomeSecret'  # Пароль от файла сертификат. Получается на api.developer.sber.ru
+russian_crt = f'{os.getcwd()}/Cert_CA.pem'  # Сертификат мин.цифры для установления SSL соединения
+# Если требуется передайте аргумент redis=
+# redis = aioredis.from_url("redis://localhost", decode_responses=True)
+# redis = "redis://localhost"
+# Redis используется только для временного хранения токена
+sber_qr = SberQR(member_id=member_id, id_qr=tid, tid=tid,
+                      client_id=client_id, client_secret=client_secret,
+                      crt_file_path=crt_from_pkcs12, key_file_path=key_from_pkcs12,
+                      pkcs12_password=pkcs12_password,
+                      russian_crt=russian_crt)
+positions = [{"position_name": 'Товар ра 10 рублей',
+              "position_count": 1,
+              "position_sum": 1000,
+              "position_description": 'Какой-то товар за 10 рублей'}
+             ]
+def creation_qr():
+    data = sber_qr.creation(description=f'Оплата заказа 3', order_sum=1000, order_number="3", positions=positions)
+    print(data)
+    
+if __name__ == '__main__':
+    creation_qr()
+```
+
+Для работы потребуется получить от банка следующие параметры
+
+```python
+member_id = '00000105'  # выдается через почту support@ecom.sberbank.ru 
+tid = '24601234'  # ID  терминала/Точки. Получить в ЛК Сбрербанк бизнес на странице Информация о точке
+id_qr = '1000301234'  # Номер наклейки с QR-кодом. Получить в ЛК Сбрербанк бизнес Информация о точке/список оборудования
+client_id = '6e7254e2-6de8-4074-b458-b7238689772b'  # получить на api.developer.sber.ru
+client_secret = '3a0ea8cb-886c-4efa-ac45-e3d36aaba335'  # получить на api.developer.sber.ru
+path_crt_from_pkcs12 = 'cert.crt' # Файл сертификат 'key.p12' Получается на api.developer.sber.ru 
+path_key_from_pkcs12 = 'private.key' # Файл сертификат 'key.p12' Получается на api.developer.sber.ru
+pkcs12_password = 'SomeSecret'  # Пароль от файла сертификата. Получается на api.developer.sber.ru
+```
+
+## Распаковка pkcs12 с помощью OpenSSL
+
+[Инструкция от ssl.com](https://www.ssl.com/ru/how-to/export-certificates-private-key-from-pkcs12-file-with-openssl/ "SSL.com") - для Windows обратите внимание на Cygwin в инструкции
+
+```
+Откройте командную строку, перейдите в папку, где лежит архив сертификата с расширением .p12. Выполните команду:
+
+openssl pkcs12 -in <название_архива>.p12 -nodes -nocerts -out private.key
+
+Появится запрос пароля. Введите пароль, который вы вводили при создании приложения, нажмите Enter.
+
+Далее аналогично выполните команду:
+
+openssl pkcs12 -in <название_архива>.p12 -clcerts -nokeys -out client_cert.crt
+
+В итоге вы получите приватный ключ в файле private.key и клиентский сертификат в файле client_cert.crt в папке, где лежит архив сертификата.
+````
+## Ссылки
+Для использования требуется аккаунт Сбер Банк бизнес.
+https://sbi.sberbank.ru:9443/ic/dcb/#/
+
+Далее необходимо Авторизоваться
+https://api.developer.sber.ru/
+
+Процесс подключения описан в инструкции
 https://api.developer.sber.ru/product/PlatiQR/doc/v1/QR_API_doc3
```

### Comparing `SberQR-2.0.0/SberQR/AsyncSberQR.py` & `SberQR-2.0.1/SberQR/AsyncSberQR.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-import asyncio
-import base64
-import ssl
-from datetime import datetime
-from logging import getLogger
-from random import choices
-from string import hexdigits
-from typing import Optional, Type, Union, List, Dict
-
-import aiohttp
-import certifi
-import ujson as json
-from redis.asyncio import Redis
-
-from .api import make_request, Methods
-from .payload import generate_payload
-from .scope import Scope
-from .types import RegistryType, CancelType
-
-logger = getLogger(__name__)
-
-
-class AsyncSberQR:
-
-    def __init__(self, member_id: str, id_qr: str, tid: str,
-                 client_id: str, client_secret: str,
-                 crt_file_path: str, key_file_path: str,
-                 pkcs12_password: str,
-                 russian_crt: str,
-                 redis: Union[str, Redis] = None,
-                 loop: Optional[Union[asyncio.BaseEventLoop, asyncio.AbstractEventLoop]] = None,
-                 connections_limit: int = None,
-                 timeout: Optional[Union[int, float, aiohttp.ClientTimeout]] = None):
-        """
-
-        :param member_id:
-        :param id_qr:
-        :param tid:
-        :param client_id:
-        :param client_secret: l
-        i]
-        :param crt_file_path:
-        :param key_file_path:
-        :param pkcs12_password:
-        :param redis:
-        :param loop:
-        :param connections_limit:
-        :param timeout:
-        """
-
-        self._main_loop = loop
-
-        self._member_id = member_id
-        self._sbp_member_id = "100000000111"
-        self._id_qr = id_qr
-        self._tid = tid
-        self._client_id = client_id
-        self._client_secret = client_secret
-        self._redis = None
-
-        self._currency = "643"
-        ssl_context = ssl.create_default_context(cafile=certifi.where())
-
-        ssl_context.load_cert_chain(certfile=crt_file_path,
-                                    keyfile=key_file_path,
-                                    password=pkcs12_password)
-        ssl_context.load_verify_locations(cafile=russian_crt)
-
-        self._session: Optional[aiohttp.ClientSession] = None
-        self._connector_class: Type[aiohttp.TCPConnector] = aiohttp.TCPConnector
-        self._connector_init = dict(limit=connections_limit, ssl=ssl_context)
-        if isinstance(redis, Redis):
-            self._redis = redis
-        elif isinstance(redis, str):
-            self._redis = Redis(host=redis, decode_responses=True)
-
-        self.timeout = timeout
-
-    async def get_new_session(self) -> aiohttp.ClientSession:
-        return aiohttp.ClientSession(
-            connector=self._connector_class(**self._connector_init),
-            json_serialize=json.dumps
-        )
-
-    @property
-    def loop(self) -> Optional[asyncio.AbstractEventLoop]:
-        return self._main_loop
-
-    async def get_session(self) -> Optional[aiohttp.ClientSession]:
-        if self._session is None or self._session.closed:
-            self._session = await self.get_new_session()
-
-        if not self._session._loop.is_running():
-            await self._session.close()
-            self._session = await self.get_new_session()
-
-        return self._session
-
-    async def close(self):
-        """
-        Close all client sessions
-        """
-        if self._session:
-            await self._session.close()
-
-    async def request(self, method, headers, data):
-        headers = {**headers, **{'Accept': 'application/json', 'x-ibm-client-id': self._client_id}}
-        return await make_request(await self.get_session(), method, headers, data)
-
-    async def get_token_from_redis(self, scope):
-        """
-        Возвращает токен, если он не истек
-        :param scope Область токена
-        :return: token string
-        """
-        return await self._redis.get(f'{self._client_id}token_{scope.value}')
-
-    async def token(self, scope: Scope):
-        redis_token = await self.get_token_from_redis(scope) if self._redis else None
-        if redis_token:
-            return redis_token
-        else:
-            auth = base64.b64encode(f'{self._client_id}:{self._client_secret}'.encode('utf-8')).decode('utf-8')
-            headers = {'Authorization': f'Basic {auth}',
-                       'Content-Type': 'application/x-www-form-urlencoded',
-                       'rquid': ''.join(choices(hexdigits, k=32))}
-            data = {'grant_type': 'client_credentials', 'scope': scope.value}
-            token_data = await self.request(Methods.oauth, headers, data)
-            if self._redis:
-                await self._redis.set(f'{self._client_id}token_{scope.value}', token_data['access_token'],
-                                      int(token_data['expires_in']) - 10)
-            return token_data['access_token']
-
-    async def creation(self, description: str, order_sum: int, order_number: str, positions: Union[List, Dict]):
-        """
-        Создание заказа
-        """
-        dt = f'{datetime.utcnow().isoformat(timespec="seconds")}Z'
-        rq_uid = ''.join(choices(hexdigits, k=32))
-        headers = {'Authorization': f'Bearer {await self.token(Scope.create)}', 'RqUID': rq_uid}
-
-        rq_tm, order_create_date = dt, dt
-        member_id, id_qr, currency = self._member_id, self._id_qr, self._currency
-
-        sbp_member_id = self._sbp_member_id if self._tid == self._id_qr else None
-
-        if isinstance(positions, dict):
-            order_params_type = [positions]
-        else:
-            order_params_type = positions
-        del positions
-        payload = generate_payload(exclude=['dt', 'headers'], **locals())
-        return await self.request(Methods.creation, headers, payload)
-
-    async def status(self, order_id: str, partner_order_number: str):
-        rq_uid = ''.join(choices(hexdigits, k=32))
-        headers = {'Authorization': f'Bearer {await self.token(Scope.status)}', 'RqUID': rq_uid}
-        tid = self._tid
-        rq_tm = f'{datetime.utcnow().isoformat(timespec="seconds")}Z'
-        payload = generate_payload(exclude=['headers'], **locals())
-        return await self.request(Methods.status, headers, payload)
-
-    async def revoke(self, order_id: str):
-        rq_uid = ''.join(choices(hexdigits, k=32))
-        headers = {'Authorization': f'Bearer {await self.token(Scope.revoke)}', 'RqUID': rq_uid}
-
-        rq_tm = f'{datetime.utcnow().isoformat(timespec="seconds")}Z'
-        payload = generate_payload(exclude=['headers'], **locals())
-        return await self.request(Methods.revocation, headers, payload)
-
-    async def cancel(
-            self, order_id: str, operation_id: str, cancel_operation_sum: int, auth_code: str,
-            operation_type: CancelType = CancelType.REVERSE, sbp_payer_id: str = None
-    ):
-        """
-        Отмена/возврат
-        """
-        rq_uid = ''.join(choices(hexdigits, k=32))
-        headers = {'Authorization': f'Bearer {await self.token(Scope.cancel)}', 'RqUID': rq_uid}
-
-        rq_tm = f'{datetime.utcnow().isoformat(timespec="seconds")}Z'
-        id_qr, tid, operation_currency = self._id_qr, self._tid, self._currency
-        operation_type = operation_type.value
-        payload = generate_payload(exclude=['headers'], **locals())
-        return await self.request(Methods.cancel, headers, payload)
-
-    async def registry(self, start_period: datetime, end_period: datetime,
-                       registry_type: RegistryType = RegistryType.REGISTRY):
-        """
-        Запрос реестра операций
-        """
-        rq_uid = ''.join(choices(hexdigits, k=32))
-        headers = {'Authorization': f'Bearer {await self.token(Scope.registry)}', 'RqUID': rq_uid}
-        payload = {"rqUid": rq_uid,
-                   "rqTm": f'{datetime.utcnow().isoformat(timespec="seconds")}Z',
-                   "idQR": self._id_qr,
-                   "startPeriod": f'{start_period.isoformat(timespec="seconds")}Z',
-                   "endPeriod": f'{end_period.isoformat(timespec="seconds")}Z',
-                   "registryType": registry_type.value}
-
+import asyncio
+import base64
+import ssl
+from datetime import datetime
+from logging import getLogger
+from random import choices
+from string import hexdigits
+from typing import Optional, Type, Union, List, Dict
+
+import aiohttp
+import certifi
+import ujson as json
+from redis.asyncio import Redis
+
+from .api import make_request, Methods
+from .payload import generate_payload
+from .scope import Scope
+from .types import RegistryType, CancelType
+
+logger = getLogger(__name__)
+
+
+class AsyncSberQR:
+
+    def __init__(self, member_id: str, id_qr: str, tid: str,
+                 client_id: str, client_secret: str,
+                 crt_file_path: str, key_file_path: str,
+                 pkcs12_password: str,
+                 russian_crt: str,
+                 redis: Union[str, Redis] = None,
+                 loop: Optional[Union[asyncio.BaseEventLoop, asyncio.AbstractEventLoop]] = None,
+                 connections_limit: int = None,
+                 timeout: Optional[Union[int, float, aiohttp.ClientTimeout]] = None):
+        """
+
+        :param member_id:
+        :param id_qr:
+        :param tid:
+        :param client_id:
+        :param client_secret: l
+        i]
+        :param crt_file_path:
+        :param key_file_path:
+        :param pkcs12_password:
+        :param redis:
+        :param loop:
+        :param connections_limit:
+        :param timeout:
+        """
+
+        self._main_loop = loop
+
+        self._member_id = member_id
+        self._sbp_member_id = "100000000111"
+        self._id_qr = id_qr
+        self._tid = tid
+        self._client_id = client_id
+        self._client_secret = client_secret
+        self._redis = None
+
+        self._currency = "643"
+        ssl_context = ssl.create_default_context(cafile=certifi.where())
+
+        ssl_context.load_cert_chain(certfile=crt_file_path,
+                                    keyfile=key_file_path,
+                                    password=pkcs12_password)
+        ssl_context.load_verify_locations(cafile=russian_crt)
+
+        self._session: Optional[aiohttp.ClientSession] = None
+        self._connector_class: Type[aiohttp.TCPConnector] = aiohttp.TCPConnector
+        self._connector_init = dict(limit=connections_limit, ssl=ssl_context)
+        if isinstance(redis, Redis):
+            self._redis = redis
+        elif isinstance(redis, str):
+            self._redis = Redis(host=redis, decode_responses=True)
+
+        self.timeout = timeout
+
+    async def get_new_session(self) -> aiohttp.ClientSession:
+        return aiohttp.ClientSession(
+            connector=self._connector_class(**self._connector_init),
+            json_serialize=json.dumps
+        )
+
+    @property
+    def loop(self) -> Optional[asyncio.AbstractEventLoop]:
+        return self._main_loop
+
+    async def get_session(self) -> Optional[aiohttp.ClientSession]:
+        if self._session is None or self._session.closed:
+            self._session = await self.get_new_session()
+
+        if not self._session._loop.is_running():
+            await self._session.close()
+            self._session = await self.get_new_session()
+
+        return self._session
+
+    async def close(self):
+        """
+        Close all client sessions
+        """
+        if self._session:
+            await self._session.close()
+
+    async def request(self, method, headers, data):
+        headers = {**headers, **{'Accept': 'application/json', 'x-ibm-client-id': self._client_id}}
+        return await make_request(await self.get_session(), method, headers, data)
+
+    async def get_token_from_redis(self, scope):
+        """
+        Возвращает токен, если он не истек
+        :param scope Область токена
+        :return: token string
+        """
+        return await self._redis.get(f'{self._client_id}token_{scope.value}')
+
+    async def token(self, scope: Scope):
+        redis_token = await self.get_token_from_redis(scope) if self._redis else None
+        if redis_token:
+            return redis_token
+        else:
+            auth = base64.b64encode(f'{self._client_id}:{self._client_secret}'.encode('utf-8')).decode('utf-8')
+            headers = {'Authorization': f'Basic {auth}',
+                       'Content-Type': 'application/x-www-form-urlencoded',
+                       'rquid': ''.join(choices(hexdigits, k=32))}
+            data = {'grant_type': 'client_credentials', 'scope': scope.value}
+            token_data = await self.request(Methods.oauth, headers, data)
+            if self._redis:
+                await self._redis.set(f'{self._client_id}token_{scope.value}', token_data['access_token'],
+                                      int(token_data['expires_in']) - 10)
+            return token_data['access_token']
+
+    async def creation(self, description: str, order_sum: int, order_number: str, positions: Union[List, Dict]):
+        """
+        Создание заказа
+        """
+        dt = f'{datetime.utcnow().isoformat(timespec="seconds")}Z'
+        rq_uid = ''.join(choices(hexdigits, k=32))
+        headers = {'Authorization': f'Bearer {await self.token(Scope.create)}', 'RqUID': rq_uid}
+
+        rq_tm, order_create_date = dt, dt
+        member_id, id_qr, currency = self._member_id, self._id_qr, self._currency
+
+        sbp_member_id = self._sbp_member_id if self._tid == self._id_qr else None
+
+        if isinstance(positions, dict):
+            order_params_type = [positions]
+        else:
+            order_params_type = positions
+        del positions
+        payload = generate_payload(exclude=['dt', 'headers'], **locals())
+        return await self.request(Methods.creation, headers, payload)
+
+    async def status(self, order_id: str, partner_order_number: str):
+        rq_uid = ''.join(choices(hexdigits, k=32))
+        headers = {'Authorization': f'Bearer {await self.token(Scope.status)}', 'RqUID': rq_uid}
+        tid = self._tid
+        rq_tm = f'{datetime.utcnow().isoformat(timespec="seconds")}Z'
+        payload = generate_payload(exclude=['headers'], **locals())
+        return await self.request(Methods.status, headers, payload)
+
+    async def revoke(self, order_id: str):
+        rq_uid = ''.join(choices(hexdigits, k=32))
+        headers = {'Authorization': f'Bearer {await self.token(Scope.revoke)}', 'RqUID': rq_uid}
+
+        rq_tm = f'{datetime.utcnow().isoformat(timespec="seconds")}Z'
+        payload = generate_payload(exclude=['headers'], **locals())
+        return await self.request(Methods.revocation, headers, payload)
+
+    async def cancel(
+            self, order_id: str, operation_id: str, cancel_operation_sum: int, auth_code: str,
+            operation_type: CancelType = CancelType.REVERSE, sbp_payer_id: str = None
+    ):
+        """
+        Отмена/возврат
+        """
+        rq_uid = ''.join(choices(hexdigits, k=32))
+        headers = {'Authorization': f'Bearer {await self.token(Scope.cancel)}', 'RqUID': rq_uid}
+
+        rq_tm = f'{datetime.utcnow().isoformat(timespec="seconds")}Z'
+        id_qr, tid, operation_currency = self._id_qr, self._tid, self._currency
+        operation_type = operation_type.value
+        payload = generate_payload(exclude=['headers'], **locals())
+        return await self.request(Methods.cancel, headers, payload)
+
+    async def registry(self, start_period: datetime, end_period: datetime,
+                       registry_type: RegistryType = RegistryType.REGISTRY):
+        """
+        Запрос реестра операций
+        """
+        rq_uid = ''.join(choices(hexdigits, k=32))
+        headers = {'Authorization': f'Bearer {await self.token(Scope.registry)}', 'RqUID': rq_uid}
+        payload = {"rqUid": rq_uid,
+                   "rqTm": f'{datetime.utcnow().isoformat(timespec="seconds")}Z',
+                   "idQR": self._id_qr,
+                   "startPeriod": f'{start_period.isoformat(timespec="seconds")}Z',
+                   "endPeriod": f'{end_period.isoformat(timespec="seconds")}Z',
+                   "registryType": registry_type.value}
+
         return await self.request(Methods.registry, headers, payload)
```

### Comparing `SberQR-2.0.0/SberQR/SberQr.py` & `SberQR-2.0.1/SberQR/SberQr.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,194 +1,194 @@
-import asyncio
-import base64
-from datetime import datetime
-from logging import getLogger
-from random import choices
-from string import hexdigits
-from typing import Optional, Union, List, Dict
-
-import requests
-from redis.client import Redis
-from requests.adapters import HTTPAdapter
-from urllib3.util.ssl_ import create_urllib3_context
-
-from .api_sync import make_request, Methods
-from .payload import generate_payload
-from .scope import Scope
-from .types import RegistryType, CancelType
-
-logger = getLogger(__name__)
-
-
-class SberQR:
-
-    def __init__(self, member_id: str, id_qr: str, tid: str,
-                 client_id: str, client_secret: str,
-                 crt_file_path: str, key_file_path: str,
-                 pkcs12_password: str,
-                 russian_crt: str,
-                 redis: Union[str, Redis] = None,
-                 loop: Optional[Union[asyncio.BaseEventLoop, asyncio.AbstractEventLoop]] = None,
-                 timeout: Optional[Union[int, float, requests.Timeout]] = None):
-        """
-
-        :param member_id:
-        :param id_qr:
-        :param tid:
-        :param client_id:
-        :param client_secret: l
-        i]
-        :param crt_file_path:
-        :param key_file_path:
-        :param pkcs12_password:
-        :param redis:
-        :param loop:
-        :param timeout:
-        """
-
-        self._main_loop = loop
-
-        self._member_id = member_id
-        self._sbp_member_id = "100000000111"
-        self._id_qr = id_qr
-        self._tid = tid
-        self._client_id = client_id
-        self._client_secret = client_secret
-
-        self._currency = "643"
-        self._redis = None
-
-        class SSLAdapter(HTTPAdapter):
-            def init_poolmanager(self, *args, **kwargs):
-                context = create_urllib3_context()
-                context.load_cert_chain(certfile=crt_file_path, keyfile=key_file_path, password=pkcs12_password)
-                context.load_verify_locations(cafile=russian_crt)
-                kwargs['ssl_context'] = context
-                return super().init_poolmanager(*args, **kwargs)
-
-        self._session: Optional[requests.Session] = None
-        self._https_class = SSLAdapter()
-        if isinstance(redis, Redis):
-            self._redis = redis
-        elif isinstance(redis, str):
-            self._redis = Redis(redis, decode_responses=True)
-
-        self.timeout = timeout
-
-    def get_new_session(self) -> requests.Session:
-        session = requests.Session()
-        session.mount("https://", self._https_class)
-        return session
-
-    @property
-    def loop(self) -> Optional[asyncio.AbstractEventLoop]:
-        return self._main_loop
-
-    def get_session(self) -> Optional[requests.Session]:
-        if self._session is None:
-            self._session = self.get_new_session()
-
-        return self._session
-
-    def close(self):
-        """
-        Close all client sessions
-        """
-        if self._session:
-            self._session.close()
-
-    def request(self, method, headers, data):
-        headers = {**headers, **{'Accept': 'application/json', 'x-ibm-client-id': self._client_id}}
-        return make_request(self.get_session(), method, headers, data)
-
-    def get_token_from_redis(self, scope):
-        """
-        Возвращает токен, если он не истек
-        :param scope Область токена
-        :return: token string
-        """
-        return self._redis.get(f'{self._client_id}token_{scope.value}')
-
-    def token(self, scope: Scope):
-        redis_token = self.get_token_from_redis(scope) if self._redis else None
-        if redis_token is not None:
-            return redis_token
-        else:
-            auth = base64.b64encode(f'{self._client_id}:{self._client_secret}'.encode('utf-8')).decode('utf-8')
-            headers = {'Authorization': f'Basic {auth}',
-                       'Content-Type': 'application/x-www-form-urlencoded',
-                       'rquid': ''.join(choices(hexdigits, k=32))}
-            data = {'grant_type': 'client_credentials', 'scope': scope.value}
-            token_data = self.request(Methods.oauth, headers, data)
-            if self._redis:
-                self._redis.set(f'{self._client_id}token_{scope.value}', token_data['access_token'],
-                                int(token_data['expires_in']) - 10)
-            return token_data['access_token']
-
-    def creation(self, description: str, order_sum: int, order_number: str, positions: Union[List, Dict]):
-        """
-        Создание заказа
-        """
-        dt = f'{datetime.utcnow().isoformat(timespec="seconds")}Z'
-        rq_uid = ''.join(choices(hexdigits, k=32))
-        headers = {'Authorization': f'Bearer {self.token(Scope.create)}', 'RqUID': rq_uid}
-
-        rq_tm, order_create_date = dt, dt
-        member_id, id_qr, currency = self._member_id, self._id_qr, self._currency
-
-        sbp_member_id = self._sbp_member_id if self._tid == self._id_qr else None
-
-        if isinstance(positions, dict):
-            order_params_type = [positions]
-        else:
-            order_params_type = positions
-        del positions
-        payload = generate_payload(exclude=['dt', 'headers'], **locals())
-        return self.request(Methods.creation, headers, payload)
-
-    def status(self, order_id: str, partner_order_number: str):
-        rq_uid = ''.join(choices(hexdigits, k=32))
-        headers = {'Authorization': f'Bearer {self.token(Scope.status)}', 'RqUID': rq_uid}
-        tid = self._tid
-        rq_tm = f'{datetime.utcnow().isoformat(timespec="seconds")}Z'
-        payload = generate_payload(exclude=['headers'], **locals())
-        return self.request(Methods.status, headers, payload)
-
-    def revoke(self, order_id: str):
-        rq_uid = ''.join(choices(hexdigits, k=32))
-        headers = {'Authorization': f'Bearer {self.token(Scope.revoke)}', 'RqUID': rq_uid}
-
-        rq_tm = f'{datetime.utcnow().isoformat(timespec="seconds")}Z'
-        payload = generate_payload(exclude=['headers'], **locals())
-        return self.request(Methods.revocation, headers, payload)
-
-    def cancel(
-            self, order_id: str, operation_id: str, cancel_operation_sum: int, auth_code: str,
-            operation_type: CancelType = CancelType.REVERSE, sbp_payer_id: str = None
-    ):
-        """
-        Отмена/возврат
-        """
-        rq_uid = ''.join(choices(hexdigits, k=32))
-        headers = {'Authorization': f'Bearer {self.token(Scope.cancel)}', 'RqUID': rq_uid}
-
-        rq_tm = f'{datetime.utcnow().isoformat(timespec="seconds")}Z'
-        id_qr, tid, operation_currency = self._id_qr, self._tid, self._currency
-        operation_type = operation_type.value
-        payload = generate_payload(exclude=['headers'], **locals())
-        return self.request(Methods.cancel, headers, payload)
-
-    def registry(self, start_period: datetime, end_period: datetime,
-                 registry_type: RegistryType = RegistryType.REGISTRY):
-        """
-        Запрос реестра операций
-        """
-        rq_uid = ''.join(choices(hexdigits, k=32))
-        headers = {'Authorization': f'Bearer {self.token(Scope.registry)}', 'RqUID': rq_uid}
-        payload = {"rqUid": rq_uid,
-                   "rqTm": f'{datetime.utcnow().isoformat(timespec="seconds")}Z',
-                   "idQR": self._id_qr,
-                   "startPeriod": f'{start_period.isoformat(timespec="seconds")}Z',
-                   "endPeriod": f'{end_period.isoformat(timespec="seconds")}Z',
-                   "registryType": registry_type.value}
-
-        return self.request(Methods.registry, headers, payload)
+import asyncio
+import base64
+from datetime import datetime
+from logging import getLogger
+from random import choices
+from string import hexdigits
+from typing import Optional, Union, List, Dict
+
+import requests
+from redis.client import Redis
+from requests.adapters import HTTPAdapter
+from urllib3.util.ssl_ import create_urllib3_context
+
+from .api_sync import make_request, Methods
+from .payload import generate_payload
+from .scope import Scope
+from .types import RegistryType, CancelType
+
+logger = getLogger(__name__)
+
+
+class SberQR:
+
+    def __init__(self, member_id: str, id_qr: str, tid: str,
+                 client_id: str, client_secret: str,
+                 crt_file_path: str, key_file_path: str,
+                 pkcs12_password: str,
+                 russian_crt: str,
+                 redis: Union[str, Redis] = None,
+                 loop: Optional[Union[asyncio.BaseEventLoop, asyncio.AbstractEventLoop]] = None,
+                 timeout: Optional[Union[int, float, requests.Timeout]] = None):
+        """
+
+        :param member_id:
+        :param id_qr:
+        :param tid:
+        :param client_id:
+        :param client_secret: l
+        i]
+        :param crt_file_path:
+        :param key_file_path:
+        :param pkcs12_password:
+        :param redis:
+        :param loop:
+        :param timeout:
+        """
+
+        self._main_loop = loop
+
+        self._member_id = member_id
+        self._sbp_member_id = "100000000111"
+        self._id_qr = id_qr
+        self._tid = tid
+        self._client_id = client_id
+        self._client_secret = client_secret
+
+        self._currency = "643"
+        self._redis = None
+
+        class SSLAdapter(HTTPAdapter):
+            def init_poolmanager(self, *args, **kwargs):
+                context = create_urllib3_context()
+                context.load_cert_chain(certfile=crt_file_path, keyfile=key_file_path, password=pkcs12_password)
+                context.load_verify_locations(cafile=russian_crt)
+                kwargs['ssl_context'] = context
+                return super().init_poolmanager(*args, **kwargs)
+
+        self._session: Optional[requests.Session] = None
+        self._https_class = SSLAdapter()
+        if isinstance(redis, Redis):
+            self._redis = redis
+        elif isinstance(redis, str):
+            self._redis = Redis(redis, decode_responses=True)
+
+        self.timeout = timeout
+
+    def get_new_session(self) -> requests.Session:
+        session = requests.Session()
+        session.mount("https://", self._https_class)
+        return session
+
+    @property
+    def loop(self) -> Optional[asyncio.AbstractEventLoop]:
+        return self._main_loop
+
+    def get_session(self) -> Optional[requests.Session]:
+        if self._session is None:
+            self._session = self.get_new_session()
+
+        return self._session
+
+    def close(self):
+        """
+        Close all client sessions
+        """
+        if self._session:
+            self._session.close()
+
+    def request(self, method, headers, data):
+        headers = {**headers, **{'Accept': 'application/json', 'x-ibm-client-id': self._client_id}}
+        return make_request(self.get_session(), method, headers, data)
+
+    def get_token_from_redis(self, scope):
+        """
+        Возвращает токен, если он не истек
+        :param scope Область токена
+        :return: token string
+        """
+        return self._redis.get(f'{self._client_id}token_{scope.value}')
+
+    def token(self, scope: Scope):
+        redis_token = self.get_token_from_redis(scope) if self._redis else None
+        if redis_token is not None:
+            return redis_token
+        else:
+            auth = base64.b64encode(f'{self._client_id}:{self._client_secret}'.encode('utf-8')).decode('utf-8')
+            headers = {'Authorization': f'Basic {auth}',
+                       'Content-Type': 'application/x-www-form-urlencoded',
+                       'rquid': ''.join(choices(hexdigits, k=32))}
+            data = {'grant_type': 'client_credentials', 'scope': scope.value}
+            token_data = self.request(Methods.oauth, headers, data)
+            if self._redis:
+                self._redis.set(f'{self._client_id}token_{scope.value}', token_data['access_token'],
+                                int(token_data['expires_in']) - 10)
+            return token_data['access_token']
+
+    def creation(self, description: str, order_sum: int, order_number: str, positions: Union[List, Dict]):
+        """
+        Создание заказа
+        """
+        dt = f'{datetime.utcnow().isoformat(timespec="seconds")}Z'
+        rq_uid = ''.join(choices(hexdigits, k=32))
+        headers = {'Authorization': f'Bearer {self.token(Scope.create)}', 'RqUID': rq_uid}
+
+        rq_tm, order_create_date = dt, dt
+        member_id, id_qr, currency = self._member_id, self._id_qr, self._currency
+
+        sbp_member_id = self._sbp_member_id if self._tid == self._id_qr else None
+
+        if isinstance(positions, dict):
+            order_params_type = [positions]
+        else:
+            order_params_type = positions
+        del positions
+        payload = generate_payload(exclude=['dt', 'headers'], **locals())
+        return self.request(Methods.creation, headers, payload)
+
+    def status(self, order_id: str, partner_order_number: str):
+        rq_uid = ''.join(choices(hexdigits, k=32))
+        headers = {'Authorization': f'Bearer {self.token(Scope.status)}', 'RqUID': rq_uid}
+        tid = self._tid
+        rq_tm = f'{datetime.utcnow().isoformat(timespec="seconds")}Z'
+        payload = generate_payload(exclude=['headers'], **locals())
+        return self.request(Methods.status, headers, payload)
+
+    def revoke(self, order_id: str):
+        rq_uid = ''.join(choices(hexdigits, k=32))
+        headers = {'Authorization': f'Bearer {self.token(Scope.revoke)}', 'RqUID': rq_uid}
+
+        rq_tm = f'{datetime.utcnow().isoformat(timespec="seconds")}Z'
+        payload = generate_payload(exclude=['headers'], **locals())
+        return self.request(Methods.revocation, headers, payload)
+
+    def cancel(
+            self, order_id: str, operation_id: str, cancel_operation_sum: int, auth_code: str,
+            operation_type: CancelType = CancelType.REVERSE, sbp_payer_id: str = None
+    ):
+        """
+        Отмена/возврат
+        """
+        rq_uid = ''.join(choices(hexdigits, k=32))
+        headers = {'Authorization': f'Bearer {self.token(Scope.cancel)}', 'RqUID': rq_uid}
+
+        rq_tm = f'{datetime.utcnow().isoformat(timespec="seconds")}Z'
+        id_qr, tid, operation_currency = self._id_qr, self._tid, self._currency
+        operation_type = operation_type.value
+        payload = generate_payload(exclude=['headers'], **locals())
+        return self.request(Methods.cancel, headers, payload)
+
+    def registry(self, start_period: datetime, end_period: datetime,
+                 registry_type: RegistryType = RegistryType.REGISTRY):
+        """
+        Запрос реестра операций
+        """
+        rq_uid = ''.join(choices(hexdigits, k=32))
+        headers = {'Authorization': f'Bearer {self.token(Scope.registry)}', 'RqUID': rq_uid}
+        payload = {"rqUid": rq_uid,
+                   "rqTm": f'{datetime.utcnow().isoformat(timespec="seconds")}Z',
+                   "idQR": self._id_qr,
+                   "startPeriod": f'{start_period.isoformat(timespec="seconds")}Z',
+                   "endPeriod": f'{end_period.isoformat(timespec="seconds")}Z',
+                   "registryType": registry_type.value}
+
+        return self.request(Methods.registry, headers, payload)
```

### Comparing `SberQR-2.0.0/SberQR/api.py` & `SberQR-2.0.1/SberQR/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,68 @@
-import logging
-from http import HTTPStatus
-
-from SberQR.exceptions import SberQrAPIError, NetworkError
-
-logging.basicConfig(level=logging.INFO)
-logger = logging.getLogger('api')
-
-
-def check_result(method_name: str, content_type: str, status_code: int, body):
-    """
-    Checks whether `result` is a valid API response.
-    A result is considered invalid if:
-    - The server returned an HTTP response code other than 200
-    - The content of the result is invalid JSON.
-    - The method call was unsuccessful (The JSON 'ok' field equals False)
-
-    :param method_name: The name of the method called
-    :param status_code: status code
-    :param content_type: content type of result
-    :param body: result body
-    :return: The result parsed to a JSON dictionary
-    :raises ApiException: if one of the above listed cases is applicable
-    """
-    logger.debug('Response for %s: [%d] "%r"', method_name, status_code, body)
-
-    if content_type != 'application/json':
-        raise NetworkError(f"Invalid response with content type {content_type}: \"{body}\"")
-
-    if HTTPStatus.OK <= status_code <= HTTPStatus.IM_USED:
-        return body
-    elif status_code == HTTPStatus.BAD_REQUEST:
-        raise SberQrAPIError(f"{body} [{status_code}]")
-    elif status_code == HTTPStatus.NOT_FOUND:
-        raise SberQrAPIError(f"{body} [{status_code}]")
-    elif status_code == HTTPStatus.CONFLICT:
-        raise SberQrAPIError(f"{body} [{status_code}]")
-    elif status_code in (HTTPStatus.UNAUTHORIZED, HTTPStatus.FORBIDDEN):
-        raise SberQrAPIError(f"{body} [{status_code}]")
-    elif status_code >= HTTPStatus.INTERNAL_SERVER_ERROR:
-        raise SberQrAPIError(f"{body} [{status_code}]")
-
-
-async def make_request(session, method, headers, data, **kwargs):
-    url = f'https://mc.api.sberbank.ru/prod/{method}'
-
-    if method != Methods.oauth:
-        async with session.post(url, json=data, headers=headers) as response:
-            try:
-                body = await response.json()
-            except:
-                body = response.text
-            return check_result(method, response.content_type, response.status, body)
-    else:
-        async with session.post(url, data=data, headers=headers) as response:
-            try:
-                body = await response.json()
-            except:
-                body = response.text
-            return check_result(method, response.content_type, response.status, body)
-
-
-class Methods:
-    oauth = 'tokens/v2/oauth'
-    creation = 'qr/order/v3/creation'
-    status = 'qr/order/v3/status'
-    revocation = 'qr/order/v3/revocation'
-    cancel = 'qr/order/v3/cancel'
-    registry = 'qr/order/v3/registry'
+import logging
+from http import HTTPStatus
+
+from SberQR.exceptions import SberQrAPIError, NetworkError
+
+logger = logging.getLogger('api')
+
+
+def check_result(method_name: str, content_type: str, status_code: int, body):
+    """
+    Checks whether `result` is a valid API response.
+    A result is considered invalid if:
+    - The server returned an HTTP response code other than 200
+    - The content of the result is invalid JSON.
+    - The method call was unsuccessful (The JSON 'ok' field equals False)
+
+    :param method_name: The name of the method called
+    :param status_code: status code
+    :param content_type: content type of result
+    :param body: result body
+    :return: The result parsed to a JSON dictionary
+    :raises ApiException: if one of the above listed cases is applicable
+    """
+    logger.debug('Response for %s: [%d] "%r"', method_name, status_code, body)
+
+    if content_type != 'application/json':
+        raise NetworkError(f"Invalid response with content type {content_type}: \"{body}\"")
+
+    if HTTPStatus.OK <= status_code <= HTTPStatus.IM_USED:
+        return body
+    elif status_code == HTTPStatus.BAD_REQUEST:
+        raise SberQrAPIError(f"{body} [{status_code}]")
+    elif status_code == HTTPStatus.NOT_FOUND:
+        raise SberQrAPIError(f"{body} [{status_code}]")
+    elif status_code == HTTPStatus.CONFLICT:
+        raise SberQrAPIError(f"{body} [{status_code}]")
+    elif status_code in (HTTPStatus.UNAUTHORIZED, HTTPStatus.FORBIDDEN):
+        raise SberQrAPIError(f"{body} [{status_code}]")
+    elif status_code >= HTTPStatus.INTERNAL_SERVER_ERROR:
+        raise SberQrAPIError(f"{body} [{status_code}]")
+
+
+async def make_request(session, method, headers, data, **kwargs):
+    url = f'https://mc.api.sberbank.ru/prod/{method}'
+
+    if method != Methods.oauth:
+        async with session.post(url, json=data, headers=headers) as response:
+            try:
+                body = await response.json()
+            except:
+                body = response.text
+            return check_result(method, response.content_type, response.status, body)
+    else:
+        async with session.post(url, data=data, headers=headers) as response:
+            try:
+                body = await response.json()
+            except:
+                body = response.text
+            return check_result(method, response.content_type, response.status, body)
+
+
+class Methods:
+    oauth = 'tokens/v2/oauth'
+    creation = 'qr/order/v3/creation'
+    status = 'qr/order/v3/status'
+    revocation = 'qr/order/v3/revocation'
+    cancel = 'qr/order/v3/cancel'
+    registry = 'qr/order/v3/registry'
```

### Comparing `SberQR-2.0.0/SberQR.egg-info/PKG-INFO` & `SberQR-2.0.1/SberQR.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,167 +1,167 @@
-Metadata-Version: 2.1
-Name: SberQR
-Version: 2.0.0
-Summary: Библиотека для работы с SberPay QR/Плати QR.
-Home-page: https://github.com/bl4ckm45k/SberQR
-Author: bl4ckm45k
-Author-email: nonpowa@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Framework :: AsyncIO
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Office/Business :: Financial
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: aiohttp>=3.8.4
-Requires-Dist: certifi>=2023.11.17
-Requires-Dist: ujson>=5.9.0
-Requires-Dist: pytz==2022.1
-Requires-Dist: qrcode[pil]>=7.3.1
-Requires-Dist: redis>=4.2.0rc1
-Requires-Dist: urllib3~=2.0.3
-
-![](https://img.shields.io/github/stars/bl4ckm45k/SberQR.svg)
-![](https://img.shields.io/github/forks/bl4ckm45k/SberQR.svg)
-![](https://img.shields.io/github/issues/bl4ckm45k/SberQR.svg)
-[![Supported python versions](https://img.shields.io/pypi/pyversions/SberQR.svg)](https://pypi.python.org/pypi/SberQR)
-[![Downloads](https://img.shields.io/pypi/dm/SberQR.svg?)](https://pypi.python.org/pypi/SberQR)
-[![PyPi Package Version](https://img.shields.io/pypi/v/SberQR)](https://pypi.python.org/pypi/SberQR)
-
-
-
-## Асинхронная и синхронная библиотека для работы с SberPay QR/Плати QR.
-
-Асинхронная и синхронная библиотека для работы с SberPay QR/Плати QR.
-
-Позволяет создавать динамический QR и проверять статус платежа.
-
-> Обязательно передавайте параметр russian_crt, без него не удастся установить SSL соединение с API Сбера
-> 
-> [PEM Сертификат securepayments.sberbank.ru](https://securepayments.sberbank.ru/wiki/doku.php/certificates:add:backend)
-
-> Если при инициализации класса `AsyncSberQR` переданы одинаковые `tid` и `id_qr`, то будет создан
-> платеж через СБП, иначе через ПлатиQR.
-## Пример (async)
-
-```python
-import os
-import asyncio
-from SberQR import AsyncSberQR
-
-member_id = '00000105'  # выдается через почту support@ecom.sberbank.ru
-tid = '24601234'  # ID  терминала/Точки. Получить в ЛК Сбрербанк бизнес на странице Информация о точке
-id_qr = '1000301234'  # Номер наклейки с QR-кодом. Получить в ЛК Сбрербанк бизнес Информация о точке/список оборудования
-client_id = '6e7254e2-6de8-4074-b458-b7238689772b'  # получить на api.developer.sber.ru
-client_secret = '3a0ea8cb-886c-4efa-ac45-e3d36aaba335'  # получить на api.developer.sber.ru
-
-#
-crt_from_pkcs12 = f'{os.getcwd()}/cert.crt'  # Для асинхронной версии требуется распаковать сертификат
-key_from_pkcs12 = f'{os.getcwd()}/private.key'  # Для асинхронной версии требуется распаковать приватный ключ
-pkcs12_password = 'SomeSecret'  # Пароль от файла сертификат. Получается на api.developer.sber.ru
-russian_crt = f'{os.getcwd()}/Cert_CA.pem'  # Сертификат мин.цифры для установления SSL соединения
-# Если требуется передайте аргумент redis=
-# redis = aioredis.from_url("redis://localhost", decode_responses=True)
-# redis = "redis://localhost"
-# Redis используется только для временного хранения токена
-sber_qr = AsyncSberQR(member_id=member_id, id_qr=tid, tid=tid,
-                      client_id=client_id, client_secret=client_secret,
-                      crt_file_path=crt_from_pkcs12, key_file_path=key_from_pkcs12,
-                      pkcs12_password=pkcs12_password,
-                      russian_crt=russian_crt)
-positions = [{"position_name": 'Товар ра 10 рублей',
-              "position_count": 1,
-              "position_sum": 1000,
-              "position_description": 'Какой-то товар за 10 рублей'}
-             ]
-async def creation_qr():
-    data = await sber_qr.creation(description=f'Оплата заказа 3', order_sum=1000, order_number="3", positions=positions)
-    print(data)
-if __name__ == '__main__':
-    asyncio.run(creation_qr())
-```
-
-## Пример (sync)
-
-```python
-import os
-from SberQR import SberQR
-
-member_id = '00000105'  # выдается через почту support@ecom.sberbank.ru
-tid = '24601234'  # ID  терминала/Точки. Получить в ЛК Сбрербанк бизнес на странице Информация о точке
-id_qr = '1000301234'  # Номер наклейки с QR-кодом. Получить в ЛК Сбрербанк бизнес Информация о точке/список оборудования
-client_id = '6e7254e2-6de8-4074-b458-b7238689772b'  # получить на api.developer.sber.ru
-client_secret = '3a0ea8cb-886c-4efa-ac45-e3d36aaba335'  # получить на api.developer.sber.ru
-
-#
-crt_from_pkcs12 = f'{os.getcwd()}/cert.crt'  # Для асинхронной версии требуется распаковать сертификат
-key_from_pkcs12 = f'{os.getcwd()}/private.key'  # Для асинхронной версии требуется распаковать приватный ключ
-pkcs12_password = 'SomeSecret'  # Пароль от файла сертификат. Получается на api.developer.sber.ru
-russian_crt = f'{os.getcwd()}/Cert_CA.pem'  # Сертификат мин.цифры для установления SSL соединения
-# Если требуется передайте аргумент redis=
-# redis = aioredis.from_url("redis://localhost", decode_responses=True)
-# redis = "redis://localhost"
-# Redis используется только для временного хранения токена
-sber_qr = SberQR(member_id=member_id, id_qr=tid, tid=tid,
-                      client_id=client_id, client_secret=client_secret,
-                      crt_file_path=crt_from_pkcs12, key_file_path=key_from_pkcs12,
-                      pkcs12_password=pkcs12_password,
-                      russian_crt=russian_crt)
-positions = [{"position_name": 'Товар ра 10 рублей',
-              "position_count": 1,
-              "position_sum": 1000,
-              "position_description": 'Какой-то товар за 10 рублей'}
-             ]
-def creation_qr():
-    data = sber_qr.creation(description=f'Оплата заказа 3', order_sum=1000, order_number="3", positions=positions)
-    print(data)
-    
-if __name__ == '__main__':
-    creation_qr()
-```
-
-Для работы потребуется получить от банка следующие параметры
-
-```python
-member_id = '00000105'  # выдается через почту support@ecom.sberbank.ru 
-tid = '24601234'  # ID  терминала/Точки. Получить в ЛК Сбрербанк бизнес на странице Информация о точке
-id_qr = '1000301234'  # Номер наклейки с QR-кодом. Получить в ЛК Сбрербанк бизнес Информация о точке/список оборудования
-client_id = '6e7254e2-6de8-4074-b458-b7238689772b'  # получить на api.developer.sber.ru
-client_secret = '3a0ea8cb-886c-4efa-ac45-e3d36aaba335'  # получить на api.developer.sber.ru
-path_crt_from_pkcs12 = 'cert.crt' # Файл сертификат 'key.p12' Получается на api.developer.sber.ru 
-path_key_from_pkcs12 = 'private.key' # Файл сертификат 'key.p12' Получается на api.developer.sber.ru
-pkcs12_password = 'SomeSecret'  # Пароль от файла сертификата. Получается на api.developer.sber.ru
-```
-
-## Распаковка pkcs12 с помощью OpenSSL
-
-[Инструкция от ssl.com](https://www.ssl.com/ru/how-to/export-certificates-private-key-from-pkcs12-file-with-openssl/ "SSL.com") - для Windows обратите внимание на Cygwin в инструкции
-
-```
-Откройте командную строку, перейдите в папку, где лежит архив сертификата с расширением .p12. Выполните команду:
-
-openssl pkcs12 -in <название_архива>.p12 -nodes -nocerts -out private.key
-
-Появится запрос пароля. Введите пароль, который вы вводили при создании приложения, нажмите Enter.
-
-Далее аналогично выполните команду:
-
-openssl pkcs12 -in <название_архива>.p12 -clcerts -nokeys -out client_cert.crt
-
-В итоге вы получите приватный ключ в файле private.key и клиентский сертификат в файле client_cert.crt в папке, где лежит архив сертификата.
-````
-## Ссылки
-Для использования требуется аккаунт Сбер Банк бизнес.
-https://sbi.sberbank.ru:9443/ic/dcb/#/
-
-Далее необходимо Авторизоваться
-https://api.developer.sber.ru/
-
-Процесс подключения описан в инструкции
-https://api.developer.sber.ru/product/PlatiQR/doc/v1/QR_API_doc3
+Metadata-Version: 2.1
+Name: SberQR
+Version: 2.0.1
+Summary: Библиотека для работы с SberPay QR/Плати QR.
+Home-page: https://github.com/bl4ckm45k/SberQR
+Author: bl4ckm45k
+Author-email: nonpowa@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Framework :: AsyncIO
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Office/Business :: Financial
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: aiohttp>=3.8.4
+Requires-Dist: certifi>=2023.11.17
+Requires-Dist: ujson>=5.9.0
+Requires-Dist: pytz==2022.1
+Requires-Dist: qrcode[pil]>=7.3.1
+Requires-Dist: redis>=4.2.0rc1
+Requires-Dist: urllib3~=2.0.3
+
+![](https://img.shields.io/github/stars/bl4ckm45k/SberQR.svg)
+![](https://img.shields.io/github/forks/bl4ckm45k/SberQR.svg)
+![](https://img.shields.io/github/issues/bl4ckm45k/SberQR.svg)
+[![Supported python versions](https://img.shields.io/pypi/pyversions/SberQR.svg)](https://pypi.python.org/pypi/SberQR)
+[![Downloads](https://img.shields.io/pypi/dm/SberQR.svg?)](https://pypi.python.org/pypi/SberQR)
+[![PyPi Package Version](https://img.shields.io/pypi/v/SberQR)](https://pypi.python.org/pypi/SberQR)
+
+
+
+## Асинхронная и синхронная библиотека для работы с SberPay QR/Плати QR.
+
+Асинхронная и синхронная библиотека для работы с SberPay QR/Плати QR.
+
+Позволяет создавать динамический QR и проверять статус платежа.
+
+> Обязательно передавайте параметр russian_crt, без него не удастся установить SSL соединение с API Сбера
+> 
+> [PEM Сертификат securepayments.sberbank.ru](https://securepayments.sberbank.ru/wiki/doku.php/certificates:add:backend)
+
+> Если при инициализации класса `AsyncSberQR` переданы одинаковые `tid` и `id_qr`, то будет создан
+> платеж через СБП, иначе через ПлатиQR.
+## Пример (async)
+
+```python
+import os
+import asyncio
+from SberQR import AsyncSberQR
+
+member_id = '00000105'  # выдается через почту support@ecom.sberbank.ru
+tid = '24601234'  # ID  терминала/Точки. Получить в ЛК Сбрербанк бизнес на странице Информация о точке
+id_qr = '1000301234'  # Номер наклейки с QR-кодом. Получить в ЛК Сбрербанк бизнес Информация о точке/список оборудования
+client_id = '6e7254e2-6de8-4074-b458-b7238689772b'  # получить на api.developer.sber.ru
+client_secret = '3a0ea8cb-886c-4efa-ac45-e3d36aaba335'  # получить на api.developer.sber.ru
+
+#
+crt_from_pkcs12 = f'{os.getcwd()}/cert.crt'  # Для асинхронной версии требуется распаковать сертификат
+key_from_pkcs12 = f'{os.getcwd()}/private.key'  # Для асинхронной версии требуется распаковать приватный ключ
+pkcs12_password = 'SomeSecret'  # Пароль от файла сертификат. Получается на api.developer.sber.ru
+russian_crt = f'{os.getcwd()}/Cert_CA.pem'  # Сертификат мин.цифры для установления SSL соединения
+# Если требуется передайте аргумент redis=
+# redis = aioredis.from_url("redis://localhost", decode_responses=True)
+# redis = "redis://localhost"
+# Redis используется только для временного хранения токена
+sber_qr = AsyncSberQR(member_id=member_id, id_qr=tid, tid=tid,
+                      client_id=client_id, client_secret=client_secret,
+                      crt_file_path=crt_from_pkcs12, key_file_path=key_from_pkcs12,
+                      pkcs12_password=pkcs12_password,
+                      russian_crt=russian_crt)
+positions = [{"position_name": 'Товар ра 10 рублей',
+              "position_count": 1,
+              "position_sum": 1000,
+              "position_description": 'Какой-то товар за 10 рублей'}
+             ]
+async def creation_qr():
+    data = await sber_qr.creation(description=f'Оплата заказа 3', order_sum=1000, order_number="3", positions=positions)
+    print(data)
+if __name__ == '__main__':
+    asyncio.run(creation_qr())
+```
+
+## Пример (sync)
+
+```python
+import os
+from SberQR import SberQR
+
+member_id = '00000105'  # выдается через почту support@ecom.sberbank.ru
+tid = '24601234'  # ID  терминала/Точки. Получить в ЛК Сбрербанк бизнес на странице Информация о точке
+id_qr = '1000301234'  # Номер наклейки с QR-кодом. Получить в ЛК Сбрербанк бизнес Информация о точке/список оборудования
+client_id = '6e7254e2-6de8-4074-b458-b7238689772b'  # получить на api.developer.sber.ru
+client_secret = '3a0ea8cb-886c-4efa-ac45-e3d36aaba335'  # получить на api.developer.sber.ru
+
+#
+crt_from_pkcs12 = f'{os.getcwd()}/cert.crt'  # Для асинхронной версии требуется распаковать сертификат
+key_from_pkcs12 = f'{os.getcwd()}/private.key'  # Для асинхронной версии требуется распаковать приватный ключ
+pkcs12_password = 'SomeSecret'  # Пароль от файла сертификат. Получается на api.developer.sber.ru
+russian_crt = f'{os.getcwd()}/Cert_CA.pem'  # Сертификат мин.цифры для установления SSL соединения
+# Если требуется передайте аргумент redis=
+# redis = aioredis.from_url("redis://localhost", decode_responses=True)
+# redis = "redis://localhost"
+# Redis используется только для временного хранения токена
+sber_qr = SberQR(member_id=member_id, id_qr=tid, tid=tid,
+                      client_id=client_id, client_secret=client_secret,
+                      crt_file_path=crt_from_pkcs12, key_file_path=key_from_pkcs12,
+                      pkcs12_password=pkcs12_password,
+                      russian_crt=russian_crt)
+positions = [{"position_name": 'Товар ра 10 рублей',
+              "position_count": 1,
+              "position_sum": 1000,
+              "position_description": 'Какой-то товар за 10 рублей'}
+             ]
+def creation_qr():
+    data = sber_qr.creation(description=f'Оплата заказа 3', order_sum=1000, order_number="3", positions=positions)
+    print(data)
+    
+if __name__ == '__main__':
+    creation_qr()
+```
+
+Для работы потребуется получить от банка следующие параметры
+
+```python
+member_id = '00000105'  # выдается через почту support@ecom.sberbank.ru 
+tid = '24601234'  # ID  терминала/Точки. Получить в ЛК Сбрербанк бизнес на странице Информация о точке
+id_qr = '1000301234'  # Номер наклейки с QR-кодом. Получить в ЛК Сбрербанк бизнес Информация о точке/список оборудования
+client_id = '6e7254e2-6de8-4074-b458-b7238689772b'  # получить на api.developer.sber.ru
+client_secret = '3a0ea8cb-886c-4efa-ac45-e3d36aaba335'  # получить на api.developer.sber.ru
+path_crt_from_pkcs12 = 'cert.crt' # Файл сертификат 'key.p12' Получается на api.developer.sber.ru 
+path_key_from_pkcs12 = 'private.key' # Файл сертификат 'key.p12' Получается на api.developer.sber.ru
+pkcs12_password = 'SomeSecret'  # Пароль от файла сертификата. Получается на api.developer.sber.ru
+```
+
+## Распаковка pkcs12 с помощью OpenSSL
+
+[Инструкция от ssl.com](https://www.ssl.com/ru/how-to/export-certificates-private-key-from-pkcs12-file-with-openssl/ "SSL.com") - для Windows обратите внимание на Cygwin в инструкции
+
+```
+Откройте командную строку, перейдите в папку, где лежит архив сертификата с расширением .p12. Выполните команду:
+
+openssl pkcs12 -in <название_архива>.p12 -nodes -nocerts -out private.key
+
+Появится запрос пароля. Введите пароль, который вы вводили при создании приложения, нажмите Enter.
+
+Далее аналогично выполните команду:
+
+openssl pkcs12 -in <название_архива>.p12 -clcerts -nokeys -out client_cert.crt
+
+В итоге вы получите приватный ключ в файле private.key и клиентский сертификат в файле client_cert.crt в папке, где лежит архив сертификата.
+````
+## Ссылки
+Для использования требуется аккаунт Сбер Банк бизнес.
+https://sbi.sberbank.ru:9443/ic/dcb/#/
+
+Далее необходимо Авторизоваться
+https://api.developer.sber.ru/
+
+Процесс подключения описан в инструкции
+https://api.developer.sber.ru/product/PlatiQR/doc/v1/QR_API_doc3
```

### Comparing `SberQR-2.0.0/setup.py` & `SberQR-2.0.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import sys
-
-from setuptools import setup
-
-if sys.version_info < (3, 7):
-    raise RuntimeError('Your Python version {0} is not supported, please install '
-                       'Python 3.7+'.format('.'.join(map(str, sys.version_info[:3]))))
-requirements = ["aiohttp>=3.8.4", "certifi>=2023.11.17", "ujson>=5.9.0", "pytz==2022.1", "qrcode[pil]>=7.3.1",
-                "redis>=4.2.0rc1", "urllib3~=2.0.3"]
-
-setup(
-    name='SberQR',
-    version='2.0.0',
-    author='bl4ckm45k',
-    author_email='nonpowa@gmail.com',
-    description='Библиотека для работы с SberPay QR/Плати QR.',
-    long_description_content_type="text/markdown",
-    url="https://github.com/bl4ckm45k/SberQR",
-    license="MIT",
-    packages=['SberQR'],
-    install_requires=requirements,
-    classifiers=[
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Framework :: AsyncIO',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-        'Topic :: Office/Business :: Financial'
-
-    ],
-    python_requires='>=3.7'
-)
+import sys
+
+from setuptools import setup
+
+if sys.version_info < (3, 7):
+    raise RuntimeError('Your Python version {0} is not supported, please install '
+                       'Python 3.7+'.format('.'.join(map(str, sys.version_info[:3]))))
+requirements = ["aiohttp>=3.8.4", "certifi>=2023.11.17", "ujson>=5.9.0", "pytz==2022.1", "qrcode[pil]>=7.3.1",
+                "redis>=4.2.0rc1", "urllib3~=2.0.3"]
+
+setup(
+    name='SberQR',
+    version='2.0.1',
+    author='bl4ckm45k',
+    author_email='nonpowa@gmail.com',
+    description='Библиотека для работы с SberPay QR/Плати QR.',
+    long_description_content_type="text/markdown",
+    url="https://github.com/bl4ckm45k/SberQR",
+    license="MIT",
+    packages=['SberQR'],
+    install_requires=requirements,
+    classifiers=[
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Framework :: AsyncIO',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: OS Independent',
+        'Topic :: Office/Business :: Financial'
+
+    ],
+    python_requires='>=3.7'
+)
```

