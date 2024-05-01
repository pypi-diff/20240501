# Comparing `tmp/telegram_wallet_pay-0.4.1.tar.gz` & `tmp/telegram_wallet_pay-0.5.0.tar.gz`

## Comparing `telegram_wallet_pay-0.4.1.tar` & `telegram_wallet_pay-0.5.0.tar`

### file list

```diff
@@ -1,41 +1,46 @@
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/.editorconfig
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/Makefile
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/codecov.yaml
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/examples/00_create_order.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/examples/01_get_order_preview.py
--rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/examples/02_bot_example.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/examples/03_webhook_handler_example.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/telegram_wallet_pay/__init__.py
--rw-r--r--   0        0        0     7062 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/telegram_wallet_pay/client.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/telegram_wallet_pay/errors.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/telegram_wallet_pay/schemas/__init__.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/telegram_wallet_pay/schemas/_default.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/telegram_wallet_pay/schemas/create_order_request.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/telegram_wallet_pay/schemas/create_order_response.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/telegram_wallet_pay/schemas/get_order_preview_response.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/telegram_wallet_pay/schemas/get_order_reconciliation_list_response.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/telegram_wallet_pay/schemas/money_amount.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/telegram_wallet_pay/schemas/order_amount.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/telegram_wallet_pay/schemas/order_amount_response.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/telegram_wallet_pay/schemas/order_preview.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/telegram_wallet_pay/schemas/order_reconciliation_item.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/telegram_wallet_pay/schemas/order_reconciliation_list.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/telegram_wallet_pay/schemas/payment_option.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/telegram_wallet_pay/schemas/webhook_message.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/telegram_wallet_pay/schemas/webhook_payload.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/telegram_wallet_pay/tools/__init__.py
--rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/telegram_wallet_pay/tools/fastapi.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/telegram_wallet_pay/tools/signature.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/telegram_wallet_pay/tools/text.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/tests/__init__.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/tests/conftest.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/tests/samples.py
--rw-r--r--   0        0        0     6608 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/tests/test_client.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/tests/test_schemas.py
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/tests/test_tools/test_fastapi.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/tests/test_tools/test_signature.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/.gitignore
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/README.md
--rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     5321 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/.editorconfig
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/Makefile
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/codecov.yaml
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/examples/00_create_order.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/examples/01_get_order_preview.py
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/examples/02_bot_example.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/examples/03_webhook_handler_example.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/__init__.py
+-rw-r--r--   0        0        0     7277 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/client.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/errors.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/enums/__init__.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/enums/currency.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/enums/order_status.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/enums/request_status.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/enums/webhook_message_type.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/__init__.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/_default.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/create_order_request.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/create_order_response.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/get_order_preview_response.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/get_order_reconciliation_list_response.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/money_amount.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/order_amount.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/order_amount_response.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/order_preview.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/order_reconciliation_item.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/order_reconciliation_list.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/payment_option.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/webhook_message.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/webhook_payload.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/tools/__init__.py
+-rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/tools/fastapi.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/tools/signature.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/tools/text.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/tests/conftest.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/tests/samples.py
+-rw-r--r--   0        0        0     6608 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/tests/test_client.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/tests/test_schemas.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/tests/test_tools/test_fastapi.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/tests/test_tools/test_signature.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/.gitignore
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/README.md
+-rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5321 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/PKG-INFO
```

### Comparing `telegram_wallet_pay-0.4.1/examples/00_create_order.py` & `telegram_wallet_pay-0.5.0/examples/00_create_order.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.4.1/examples/02_bot_example.py` & `telegram_wallet_pay-0.5.0/examples/02_bot_example.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.4.1/examples/03_webhook_handler_example.py` & `telegram_wallet_pay-0.5.0/examples/03_webhook_handler_example.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.4.1/telegram_wallet_pay/client.py` & `telegram_wallet_pay-0.5.0/telegram_wallet_pay/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     Union,
 )
 
 import certifi
 from aiohttp import ClientResponse, ClientSession, TCPConnector
 from pydantic import BaseModel
 
+from telegram_wallet_pay.enums import Currency
 from telegram_wallet_pay.errors import (
     InvalidAPIKeyError,
     InvalidRequestError,
     NotFountError,
     RequestLimitReachedError,
     TelegramWalletPayError,
     UnexpectedError,
@@ -59,20 +60,29 @@
         self._session: Optional[ClientSession] = None
         self._headers = {AUTH_HEADER: token}
 
     async def create_order(  # noqa: PLR0913
         self,
         *,
         amount: Union[str, Decimal, float],
-        currency_code: Literal["TON", "BTC", "USDT", "EUR", "USD", "RUB"],
+        currency_code: Literal[
+            Currency.TON,
+            Currency.BTC,
+            Currency.USDT,
+            Currency.EUR,
+            Currency.USD,
+            Currency.RUB,
+        ],
         description: str,
         external_id: str,
         timeout_seconds: int,
         customer_telegram_user_id: int,
-        auto_conversion_currency: Optional[Literal["TON", "BTC", "USDT"]] = None,
+        auto_conversion_currency: Optional[
+            Literal[Currency.TON, Currency.BTC, Currency.USDT]
+        ] = None,
         return_url: Optional[str] = None,
         fail_return_url: Optional[str] = None,
         custom_data: Optional[str] = None,
     ) -> CreateOrderResponse:
         """Create an order.
 
         Docs:
```

### Comparing `telegram_wallet_pay-0.4.1/telegram_wallet_pay/schemas/__init__.py` & `telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.4.1/telegram_wallet_pay/schemas/create_order_request.py` & `telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/create_order_request.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 from typing import Literal, Optional
 
 from pydantic import Field
 
+from telegram_wallet_pay.enums import Currency
+
 from ._default import DefaultModel
 from .money_amount import MoneyAmount
 
 
 class CreateOrderRequest(DefaultModel):
     amount: MoneyAmount
-    auto_conversion_currency: Optional[Literal["TON", "BTC", "USDT"]] = None
+    auto_conversion_currency: Optional[
+        Literal[
+            Currency.TON,
+            Currency.BTC,
+            Currency.USDT,
+        ]
+    ] = None
     description: str = Field(min_length=5, max_length=100)
     return_url: Optional[str] = Field(None, max_length=255)
     fail_return_url: Optional[str] = Field(None, max_length=255)
     custom_data: Optional[str] = Field(None, max_length=255)
     external_id: str = Field(max_length=255)
     timeout_seconds: int = Field(ge=30, le=864000)
     customer_telegram_user_id: int
```

### Comparing `telegram_wallet_pay-0.4.1/telegram_wallet_pay/schemas/order_preview.py` & `telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/order_preview.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 from datetime import datetime
 from typing import Literal, Optional
 
 from pydantic import Field
 
+from telegram_wallet_pay.enums import Currency, OrderStatus
+
 from ._default import DefaultModel
 from .money_amount import MoneyAmount
 
 
 class OrderPreview(DefaultModel):
     id: str
-    status: Literal["ACTIVE", "EXPIRED", "PAID", "CANCELLED"]
+    status: OrderStatus
     number: str
     amount: MoneyAmount
-    auto_conversion_currency: Optional[Literal["TON", "BTC", "USDT"]] = None
+    auto_conversion_currency: Optional[
+        Literal[
+            Currency.TON,
+            Currency.BTC,
+            Currency.USDT,
+        ]
+    ] = None
     created_datetime: datetime = Field(alias="createdDateTime")
     expiration_datetime: datetime = Field(alias="expirationDateTime")
     completed_datetime: Optional[datetime] = Field(None, alias="completedDateTime")
     pay_link: str
     direct_pay_link: str
```

### Comparing `telegram_wallet_pay-0.4.1/telegram_wallet_pay/schemas/webhook_message.py` & `telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/webhook_message.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from datetime import datetime
-from typing import Iterator, List, Literal
+from typing import Iterator, List
 
 from pydantic import Field
 
+from telegram_wallet_pay.enums import WebhookMessageType
+
 from ._default import DefaultModel, DefaultRootModel
 from .webhook_payload import WebhookPayload
 
 
 class WebhookMessage(DefaultModel):
     event_datetime: datetime = Field(alias="eventDateTime")
     event_id: int
-    type: Literal["ORDER_FAILED", "ORDER_PAID"]
+    type: WebhookMessageType
     payload: WebhookPayload
 
 
 class WebhookMessages(DefaultRootModel):
     root: List[WebhookMessage]
 
     def __iter__(self) -> Iterator[WebhookMessage]:  # type: ignore[override]
```

### Comparing `telegram_wallet_pay-0.4.1/telegram_wallet_pay/schemas/webhook_payload.py` & `telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/webhook_payload.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from datetime import datetime
 from typing import Optional
 
 from pydantic import Field
 
+from telegram_wallet_pay.enums import OrderStatus
+
 from ._default import DefaultModel
 from .money_amount import MoneyAmount
 from .payment_option import PaymentOption
 
 
 class WebhookPayload(DefaultModel):
     id: int
     number: str
     external_id: str = Field(max_length=255)
+    status: Optional[OrderStatus] = None
     custom_data: Optional[str] = Field(None, max_length=255)
     order_amount: MoneyAmount
-    selected_payment_option: PaymentOption
+    selected_payment_option: Optional[PaymentOption] = None
     order_completed_datetime: datetime = Field(alias="orderCompletedDateTime")
```

### Comparing `telegram_wallet_pay-0.4.1/telegram_wallet_pay/tools/fastapi.py` & `telegram_wallet_pay-0.5.0/telegram_wallet_pay/tools/fastapi.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.4.1/telegram_wallet_pay/tools/signature.py` & `telegram_wallet_pay-0.5.0/telegram_wallet_pay/tools/signature.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.4.1/tests/conftest.py` & `telegram_wallet_pay-0.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.4.1/tests/samples.py` & `telegram_wallet_pay-0.5.0/tests/samples.py`

 * *Files 21% similar despite different names*

```diff
@@ -24,15 +24,33 @@
     "number": "E953D09Q",
     "externalId": "0120bb34-5a74-4eb2-a3da-774b97cf3fbe",
     "orderAmount": ORDER_AMOUNT,
     "selectedPaymentOption": SELECTED_PAYMENT_OPTION,
     "orderCompletedDateTime": "2024-04-21T15:04:24.092Z",
 }
 
-WEBHOOK_MESSAGE = {
+WEBHOOK_MESSAGE_ORDER_PAID = {
     "eventDateTime": "2024-04-21T15:04:24.092Z",
     "eventId": 10829789207553,
     "type": "ORDER_PAID",
     "payload": WEBHOOK_PAYLOAD,
 }
 
-WEBHOOK_MESSAGES = [WEBHOOK_MESSAGE]
+WEBHOOK_MESSAGE_ORDER_FAILED = {
+    "eventId": 11044361216001,
+    "eventDateTime": "2024-05-01T07:53:56.000991Z",
+    "payload": {
+        "id": 11000119772673,
+        "number": "LVDPW6K8",
+        "status": "EXPIRED",
+        "customData": "some-custom-data",
+        "externalId": "07d9539e-fd61-497e-a164-d2e354a55744",
+        "orderAmount": {
+            "amount": "0.44",
+            "currencyCode": "USD",
+        },
+        "orderCompletedDateTime": "2024-05-01T07:53:56.000980Z",
+    },
+    "type": "ORDER_FAILED",
+}
+
+WEBHOOK_MESSAGES = [WEBHOOK_MESSAGE_ORDER_PAID, WEBHOOK_MESSAGE_ORDER_FAILED]
```

### Comparing `telegram_wallet_pay-0.4.1/tests/test_client.py` & `telegram_wallet_pay-0.5.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.4.1/tests/test_schemas.py` & `telegram_wallet_pay-0.5.0/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.4.1/tests/test_tools/test_fastapi.py` & `telegram_wallet_pay-0.5.0/tests/test_tools/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.4.1/tests/test_tools/test_signature.py` & `telegram_wallet_pay-0.5.0/tests/test_tools/test_signature.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.4.1/.gitignore` & `telegram_wallet_pay-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.4.1/README.md` & `telegram_wallet_pay-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.4.1/pyproject.toml` & `telegram_wallet_pay-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.4.1/PKG-INFO` & `telegram_wallet_pay-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: telegram-wallet-pay
-Version: 0.4.1
+Version: 0.5.0
 Summary: Async client for Telegram Wallet Pay API
 Project-URL: Repository, https://github.com/Olegt0rr/TelegramWalletPay
 Project-URL: Documentation, https://docs.wallet.tg/pay/
 Author-email: Oleg Abramov <oleg@trueweb.app>
 Maintainer-email: Oleg Abramov <oleg@trueweb.app>
 License-Expression: MIT
 Keywords: API,Pay,Telegram,Wallet,async
```

