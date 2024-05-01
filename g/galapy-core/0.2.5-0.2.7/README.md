# Comparing `tmp/galapy_core-0.2.5.tar.gz` & `tmp/galapy_core-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galapy_core-0.2.5.tar", max compression
+gzip compressed data, was "galapy_core-0.2.7.tar", max compression
```

## Comparing `galapy_core-0.2.5.tar` & `galapy_core-0.2.7.tar`

### file list

```diff
@@ -1,16 +1,20 @@
--rw-r--r--   0        0        0        0 2024-04-15 21:11:05.088281 galapy_core-0.2.5/README.md
--rw-r--r--   0        0        0        0 2024-04-15 21:11:05.088450 galapy_core-0.2.5/galapy_core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 21:11:05.088493 galapy_core-0.2.5/galapy_core/accounts.py
--rw-r--r--   0        0        0    19258 2024-04-15 21:11:05.088606 galapy_core-0.2.5/galapy_core/assets.py
--rw-r--r--   0        0        0      970 2024-04-15 21:11:05.088706 galapy_core-0.2.5/galapy_core/core.py
--rw-r--r--   0        0        0      160 2024-04-15 21:11:05.088884 galapy_core-0.2.5/galapy_core/generators/README.md
--rw-r--r--   0        0        0       34 2024-04-15 21:11:05.088948 galapy_core-0.2.5/galapy_core/generators/__init__.py
--rw-r--r--   0        0        0     2649 2024-04-25 21:34:39.903530 galapy_core-0.2.5/galapy_core/generators/price.py
--rw-r--r--   0        0        0     1219 2024-04-15 21:11:05.088780 galapy_core-0.2.5/galapy_core/generators.py
--rw-r--r--   0        0        0    12575 2024-04-15 21:11:05.089130 galapy_core-0.2.5/galapy_core/handlers.py
--rw-r--r--   0        0        0     7141 2024-04-15 21:11:05.089255 galapy_core-0.2.5/galapy_core/market_data.py
--rw-r--r--   0        0        0     9472 2024-04-15 21:11:05.089422 galapy_core-0.2.5/galapy_core/metrics.py
--rw-r--r--   0        0        0     8142 2024-04-15 21:11:05.089546 galapy_core-0.2.5/galapy_core/orders.py
--rw-r--r--   0        0        0    11285 2024-04-15 21:11:05.089703 galapy_core-0.2.5/galapy_core/portfolio.py
--rw-r--r--   0        0        0      463 2024-04-25 21:34:50.307300 galapy_core-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      647 1970-01-01 00:00:00.000000 galapy_core-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 21:11:05.088281 galapy_core-0.2.7/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 21:11:05.088450 galapy_core-0.2.7/galapy_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 21:11:05.088493 galapy_core-0.2.7/galapy_core/accounts.py
+-rw-r--r--   0        0        0    19258 2024-04-15 21:11:05.088606 galapy_core-0.2.7/galapy_core/assets.py
+-rw-r--r--   0        0        0      970 2024-04-15 21:11:05.088706 galapy_core-0.2.7/galapy_core/core.py
+-rw-r--r--   0        0        0      160 2024-04-15 21:11:05.088884 galapy_core-0.2.7/galapy_core/generators/README.md
+-rw-r--r--   0        0        0       34 2024-04-15 21:11:05.088948 galapy_core-0.2.7/galapy_core/generators/__init__.py
+-rw-r--r--   0        0        0     2649 2024-04-25 21:34:39.903530 galapy_core-0.2.7/galapy_core/generators/price.py
+-rw-r--r--   0        0        0     1219 2024-04-15 21:11:05.088780 galapy_core-0.2.7/galapy_core/generators.py
+-rw-r--r--   0        0        0    12575 2024-04-15 21:11:05.089130 galapy_core-0.2.7/galapy_core/handlers.py
+-rw-r--r--   0        0        0     7141 2024-04-15 21:11:05.089255 galapy_core-0.2.7/galapy_core/market_data.py
+-rw-r--r--   0        0        0     9472 2024-04-15 21:11:05.089422 galapy_core-0.2.7/galapy_core/metrics.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:53:13.664009 galapy_core-0.2.7/galapy_core/oms/__init__.py
+-rw-r--r--   0        0        0     6878 2024-04-29 04:29:14.923720 galapy_core-0.2.7/galapy_core/oms/database_manager.py
+-rw-r--r--   0        0        0     1846 2024-04-28 01:08:15.553500 galapy_core-0.2.7/galapy_core/oms/exchange_api.py
+-rw-r--r--   0        0        0     3464 2024-04-28 01:24:29.300499 galapy_core-0.2.7/galapy_core/oms/order_manager.py
+-rw-r--r--   0        0        0    11985 2024-04-27 23:48:11.553175 galapy_core-0.2.7/galapy_core/orders.py
+-rw-r--r--   0        0        0    11285 2024-04-15 21:11:05.089703 galapy_core-0.2.7/galapy_core/portfolio.py
+-rw-r--r--   0        0        0      464 2024-05-01 03:59:00.995178 galapy_core-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 galapy_core-0.2.7/PKG-INFO
```

### Comparing `galapy_core-0.2.5/galapy_core/assets.py` & `galapy_core-0.2.7/galapy_core/assets.py`

 * *Files identical despite different names*

### Comparing `galapy_core-0.2.5/galapy_core/core.py` & `galapy_core-0.2.7/galapy_core/core.py`

 * *Files identical despite different names*

### Comparing `galapy_core-0.2.5/galapy_core/generators/price.py` & `galapy_core-0.2.7/galapy_core/generators/price.py`

 * *Files identical despite different names*

### Comparing `galapy_core-0.2.5/galapy_core/generators.py` & `galapy_core-0.2.7/galapy_core/generators.py`

 * *Files identical despite different names*

### Comparing `galapy_core-0.2.5/galapy_core/handlers.py` & `galapy_core-0.2.7/galapy_core/handlers.py`

 * *Files identical despite different names*

### Comparing `galapy_core-0.2.5/galapy_core/market_data.py` & `galapy_core-0.2.7/galapy_core/market_data.py`

 * *Files identical despite different names*

### Comparing `galapy_core-0.2.5/galapy_core/metrics.py` & `galapy_core-0.2.7/galapy_core/metrics.py`

 * *Files identical despite different names*

### Comparing `galapy_core-0.2.5/galapy_core/orders.py` & `galapy_core-0.2.7/galapy_core/orders.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,28 +4,70 @@
 from typing import List
 
 import pendulum
 from postgrest._sync.request_builder import SyncRequestBuilder
 from postgrest.base_request_builder import APIResponse
 from rich import print
 from supabase.client import PostgrestAPIError
+
 from supamodel._client import client as supabase
 from supamodel._logging import logger
 from supamodel.enums import OrderSide, OrderStatus, OrderType
 from supamodel.exceptions import EmptyResponseError
 from supamodel.trading.order_management import Order, Trade
 from supamodel.trading.portfolio import Portfolio, Position
 
 # Can get the exchange_id from the asset_id. We can simply look at the asset's exchange_id and return it.
 
 depth_logger = logger.opt(depth=1)
 
 
 class MockExchangeAPI:
+    """
+    A mock implementation of an exchange API.
+
+    This class provides methods to simulate order submission, retrieval, fee calculation,
+    and other exchange-related operations.
+
+    Methods:
+        submit_order(order: Order) -> Order:
+            Submits an order and returns the filled order.
+
+        get_order(order_id: str) -> Order:
+            Retrieves an order based on the given order ID.
+
+        calculate_fees(order: Order) -> float:
+            Calculates the fees for the given order.
+
+        get_exchange_id(asset_id: str) -> str:
+            Retrieves the exchange ID for the given asset ID.
+
+        get_current_price(position: Position) -> float:
+            Retrieves the current price for the given position.
+
+        get_fill_timestamp(order: Order) -> float:
+            Retrieves the fill timestamp for the given order.
+
+        get_fill_details(order: Order) -> dict:
+            Retrieves the fill details for the given order.
+
+        calculate_fee(order: Order) -> float:
+            Calculates the fee for the given order.
+    """
+
     def submit_order(self, order: Order) -> Order:
+        """
+        Submits an order and updates its status to FILLED.
+
+        Args:
+            order (Order): The order to be submitted.
+
+        Returns:
+            Order: The submitted order with the updated status.
+        """
         order.status = OrderStatus.FILLED
         return order
 
     def get_order(self, order_id: str) -> Order:
         return Order()
 
     def calculate_fees(self, order: Order) -> float:
@@ -33,25 +75,37 @@
 
     def get_exchange_id(self, asset_id: str) -> str:
         return "exchange_id"
 
     def get_current_price(self, position: Position) -> float:
         return random.uniform(0.0, 100.0)
 
-    def get_fill_timestamp(order: Order) -> float:
+    def get_fill_timestamp(self, order: Order) -> float:
+        """
+        Get the fill timestamp for the given order.
+
+        Parameters:
+            order (Order): The order for which to get the fill timestamp.
+
+        Returns:
+            float: The fill timestamp in UTC.
+        """
         return pendulum.now("UTC").timestamp()
 
     def get_fill_details(self, order: Order) -> dict:
         return random.uniform(0.1, 100), random.uniform(0.1, 8.0)
 
+    def calculate_fee(self, order: Order) -> float:
+        return random.uniform(0.0, 0.1)
+
 
 exchange_api = MockExchangeAPI()
 
 
-def submit_order(order: Order) -> Order:
+def save_order(order: Order) -> Order:
     """
     Submits an order to the database.
 
     Args:
         order (Order): The order to be submitted.
 
     Returns:
@@ -61,15 +115,16 @@
         EmptyResponseError: If the response from the database is empty.
     """
     response = supabase.table("orders").insert(order.supa_dump(by_alias=True)).execute()
     resp_data = response.data
     resp_data if resp_data else []
     if not resp_data:
         raise EmptyResponseError("Failed to add order to the database.")
-    return resp_data
+
+    return Order(**resp_data[0])
 
 
 def change_order_status(order_id: str, status: OrderSide) -> Order:
     """
     Change the status of an order.
 
     Args:
@@ -87,15 +142,31 @@
         .execute()
     )
     results = process_results(result)
     return Order(**results[0])
     # return resp_data
 
 
-def create_position(order: Order) -> Position:
+def get_position_by_portfolio_asset_id(
+    portfolio_id: str, asset_id: str
+) -> Position | None:
+    result: APIResponse = (
+        supabase.table("positions")
+        .select("*")
+        .eq("portfolio_id", portfolio_id)
+        .eq("asset_id", asset_id)
+        .limit(1)
+        .execute()
+    )
+    if result.data:
+        return Position(**result.data[0])
+    return None
+
+
+def create_position(order: Order, by_alias: bool = False) -> Position:
     """
     Creates a new position based on the given order and saves it to the database.
 
     Args:
         order (Order): The order object containing the details of the position.
 
     Returns:
@@ -105,17 +176,30 @@
 
     new_position = Position(
         portfolio_id=order.portfolio_id,
         asset_id=order.asset_id,
         quantity=order.quantity,
         average_price=order.price,
     )
+    existing_position = get_position_by_portfolio_asset_id(
+        order.portfolio_id, order.asset_id
+    )
+    if not existing_position:
+        result: APIResponse = (
+            supabase.table("positions")
+            .insert(new_position.supa_dump(by_alias=by_alias))
+            .execute()
+        )
+        results = process_results(result)
+
+        return Position(**results[0])
+    new_position.id = existing_position.id
     result: APIResponse = (
         supabase.table("positions")
-        .insert(new_position.supa_dump(by_alias=True))
+        .upsert(new_position.supa_dump(by_alias=by_alias))
         .execute()
     )
     results = process_results(result)
 
     return Position(**results[0])
 
 
@@ -138,65 +222,100 @@
         depth_logger.error("Failed to process Supabase results.")
         raise EmptyResponseError()
 
     return result_data
 
 
 def transact_trade_position(order: Order) -> Trade:
-    with contextlib.suppress(Exception):
-        position: Position = create_position(order)
+    # with contextlib.suppress(Exception):
+    position: Position = create_position(order)
 
-        trade = Trade(
-            position_id=position.id,
-            order_id=order.id,
-            quantity=order.quantity,
-            price=order.price,
-            fee=exchange_api.calculate_fee(order),
-            timestamp=exchange_api.get_fill_timestamp(order),
-        )
-        result = (
-            supabase.table("trades").insert(trade.supa_dump(by_alias=True)).execute()
-        )
+    trade = Trade(
+        position_id=position.id,
+        order_id=order.id,
+        quantity=order.quantity,
+        price=order.price,
+        fee=exchange_api.calculate_fee(order),
+        timestamp=exchange_api.get_fill_timestamp(order),
+    )
+    result = supabase.table("trades").insert(trade.supa_dump(by_alias=True)).execute()
 
-        results = process_results(result)
-        return Trade(**results[0])
+    results = process_results(result)
+    return Trade(**results[0])
 
 
 # @retry(exception=PostgrestAPIError, tries=5, delay=1)
 def get_position(position_id: str) -> Position:
     result = supabase.table("positions").select("*").eq("id", position_id).execute()
     results = process_results(result)
     return Position(**results[0])
 
 
-def save_position(position: Position) -> Position:
+def save_position(position: Position, by_alias=False) -> Position:
     result = (
         supabase.table("positions")
-        .update(position.supa_dump(by_alias=True))
+        .update(position.supa_dump(by_alias=by_alias))
         .eq("id", position.id)
         .execute()
     )
     results = process_results(result)
     return Position(**results[0])
 
 
 def update_position(order: Order, trade: Trade) -> Position:
     position = get_position(trade.position_id)
     fill_quantity, fill_price = exchange_api.get_fill_details(order)
     if order.side == OrderSide.BUY:
         position.quantity += fill_quantity
-        position.average_price = (
-            position.average_price * position.quantity + fill_price * fill_quantity
-        ) / (position.quantity + fill_quantity)
+        position.average_price = fill_price
     else:
         position.quantity -= fill_quantity
     position.updated_at = datetime.now()
     return save_position(position)
 
 
+def get_open_orders_from_db() -> List[Order]:
+    query = (
+        supabase.table("orders")
+        .select("*")
+        .in_("status", [OrderStatus.PENDING.value, OrderStatus.PARTIALLY_FILLED.value])
+    )
+    response = query.execute()
+    if response.data:
+        return [Order(**order_data) for order_data in response.data]
+    return []
+
+
+def check_open_orders():
+    # Retrieve all open orders from the database
+    open_orders = get_open_orders_from_db()
+
+    for order in open_orders:
+        order_id = order.id
+
+        # Retrieve the order from the exchange using the order_id
+        exchange_order = exchange_api.get_order(order_id)
+
+        # Check the order status
+        if exchange_order.status in [OrderStatus.FILLED, OrderStatus.PARTIALLY_FILLED]:
+            # Order is filled, process the trade and update position
+            trade = transact_trade_position(exchange_order)
+            update_position(exchange_order, trade)
+            change_order_status(order_id, exchange_order.status)
+        elif exchange_order.status == OrderStatus.CANCELED:
+            # Order is canceled, update the order status in the database
+            change_order_status(order_id, OrderStatus.CANCELED)
+        elif exchange_order.status == OrderStatus.REJECTED:
+            # Order is rejected, update the order status in the database
+            change_order_status(order_id, OrderStatus.REJECTED)
+        else:
+            # Order is still pending or partially filled, no action needed
+            continue
+
+
 def main():
     #
     portfolio_json = [
         {
             "id": "149ba2ba-289c-4bd1-8cad-4b7c3925c1ca",
             "user_id": "b3209dcc-3097-430e-8ad1-c9bb4660aa4c",
             "name": "USD Portfolio",
```

### Comparing `galapy_core-0.2.5/galapy_core/portfolio.py` & `galapy_core-0.2.7/galapy_core/portfolio.py`

 * *Files identical despite different names*

### Comparing `galapy_core-0.2.5/PKG-INFO` & `galapy_core-0.2.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: galapy-core
-Version: 0.2.5
+Version: 0.2.7
 Summary: The backend and DB interactive layer for the GalaPy project
 Author: Kevin Hill
 Author-email: kivo360@gmail.com
 Requires-Python: >=3.10,<=3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ccxt (>=4.2.93,<5.0.0)
 Requires-Dist: decorator (>=5.1.1,<6.0.0)
 Requires-Dist: devtools (>=0.12.2,<0.13.0)
 Requires-Dist: faker (>=24.8.0,<25.0.0)
-Requires-Dist: supamodel (==0.5.5)
+Requires-Dist: supamodel (>=0.5.7,<0.6.0)
 Description-Content-Type: text/markdown
```

