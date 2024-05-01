# Comparing `tmp/motormongo-0.1.8.tar.gz` & `tmp/motormongo-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motormongo-0.1.8.tar", max compression
+gzip compressed data, was "motormongo-0.1.9.tar", max compression
```

## Comparing `motormongo-0.1.8.tar` & `motormongo-0.1.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1071 2024-02-20 14:38:52.634778 motormongo-0.1.8/LICENSE
--rw-r--r--   0        0        0    31813 2024-02-20 14:38:52.634778 motormongo-0.1.8/README.md
--rw-r--r--   0        0        0      340 2024-02-20 14:38:52.634778 motormongo-0.1.8/motormongo/__init__.py
--rw-r--r--   0        0        0      119 2024-02-20 14:38:52.634778 motormongo-0.1.8/motormongo/abstracts/__init__.py
--rw-r--r--   0        0        0    38020 2024-02-20 14:38:52.634778 motormongo-0.1.8/motormongo/abstracts/document.py
--rw-r--r--   0        0        0      500 2024-02-20 14:38:52.634778 motormongo-0.1.8/motormongo/abstracts/embedded_document.py
--rw-r--r--   0        0        0       55 2024-02-20 14:38:52.634778 motormongo-0.1.8/motormongo/abstracts/exceptions/__init__.py
--rw-r--r--   0        0        0      776 2024-02-20 14:38:52.634778 motormongo-0.1.8/motormongo/abstracts/exceptions/document.py
--rw-r--r--   0        0        0      728 2024-02-20 14:38:52.634778 motormongo-0.1.8/motormongo/fields/__init__.py
--rw-r--r--   0        0        0     3406 2024-02-20 14:38:52.634778 motormongo-0.1.8/motormongo/fields/binary_field.py
--rw-r--r--   0        0        0      473 2024-02-20 14:38:52.634778 motormongo-0.1.8/motormongo/fields/boolean_field.py
--rw-r--r--   0        0        0     2478 2024-02-20 14:38:52.634778 motormongo-0.1.8/motormongo/fields/datetime_field.py
--rw-r--r--   0        0        0     1832 2024-02-20 14:38:52.634778 motormongo-0.1.8/motormongo/fields/embedded_document_field.py
--rw-r--r--   0        0        0     1478 2024-02-20 14:38:52.634778 motormongo-0.1.8/motormongo/fields/enum_field.py
--rw-r--r--   0        0        0      571 2024-02-20 14:38:52.634778 motormongo-0.1.8/motormongo/fields/exceptions/__init__.py
--rw-r--r--   0        0        0      444 2024-02-20 14:38:52.634778 motormongo-0.1.8/motormongo/fields/exceptions/binary_field.py
--rw-r--r--   0        0        0      101 2024-02-20 14:38:52.634778 motormongo-0.1.8/motormongo/fields/exceptions/boolean_field.py
--rw-r--r--   0        0        0      340 2024-02-20 14:38:52.634778 motormongo-0.1.8/motormongo/fields/exceptions/datetime_field.py
--rw-r--r--   0        0        0      246 2024-02-20 14:38:52.634778 motormongo-0.1.8/motormongo/fields/exceptions/embedded_document_field.py
--rw-r--r--   0        0        0      332 2024-02-20 14:38:52.634778 motormongo-0.1.8/motormongo/fields/exceptions/enum_field.py
--rw-r--r--   0        0        0      300 2024-02-20 14:38:52.634778 motormongo-0.1.8/motormongo/fields/exceptions/float_field.py
--rw-r--r--   0        0        0      211 2024-02-20 14:38:52.634778 motormongo-0.1.8/motormongo/fields/exceptions/geojson_field.py
--rw-r--r--   0        0        0      328 2024-02-20 14:38:52.634778 motormongo-0.1.8/motormongo/fields/exceptions/integer_field.py
--rw-r--r--   0        0        0      315 2024-02-20 14:38:52.634778 motormongo-0.1.8/motormongo/fields/exceptions/list_field.py
--rw-r--r--   0        0        0      454 2024-02-20 14:38:52.634778 motormongo-0.1.8/motormongo/fields/exceptions/string_field.py
--rw-r--r--   0        0        0      757 2024-02-20 14:38:52.634778 motormongo-0.1.8/motormongo/fields/field.py
--rw-r--r--   0        0        0     1322 2024-02-20 14:38:52.634778 motormongo-0.1.8/motormongo/fields/float_field.py
--rw-r--r--   0        0        0     1799 2024-02-20 14:38:52.634778 motormongo-0.1.8/motormongo/fields/geojson_field.py
--rw-r--r--   0        0        0     1038 2024-02-20 14:38:52.634778 motormongo-0.1.8/motormongo/fields/integer_field.py
--rw-r--r--   0        0        0      840 2024-02-20 14:38:52.634778 motormongo-0.1.8/motormongo/fields/list_field.py
--rw-r--r--   0        0        0     2370 2024-02-20 14:38:52.638778 motormongo-0.1.8/motormongo/fields/reference_field.py
--rw-r--r--   0        0        0     1315 2024-02-20 14:38:52.638778 motormongo-0.1.8/motormongo/fields/string_field.py
--rw-r--r--   0        0        0       55 2024-02-20 14:38:52.638778 motormongo-0.1.8/motormongo/mongo/__init__.py
--rw-r--r--   0        0        0     2847 2024-02-20 14:38:52.638778 motormongo-0.1.8/motormongo/mongo/database.py
--rw-r--r--   0        0        0        0 2024-02-20 14:38:52.638778 motormongo-0.1.8/motormongo/utils/__init__.py
--rw-r--r--   0        0        0     1889 2024-02-20 14:38:52.638778 motormongo-0.1.8/motormongo/utils/formatter.py
--rw-r--r--   0        0        0      256 2024-02-20 14:38:52.638778 motormongo-0.1.8/motormongo/utils/logging.py
--rw-r--r--   0        0        0     1011 2024-02-20 14:38:52.638778 motormongo-0.1.8/pyproject.toml
--rw-r--r--   0        0        0    32326 1970-01-01 00:00:00.000000 motormongo-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-02-20 17:33:49.610586 motormongo-0.1.9/LICENSE
+-rw-r--r--   0        0        0    34529 2024-02-20 17:33:49.610586 motormongo-0.1.9/README.md
+-rw-r--r--   0        0        0      340 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/__init__.py
+-rw-r--r--   0        0        0      119 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/abstracts/__init__.py
+-rw-r--r--   0        0        0    41767 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/abstracts/document.py
+-rw-r--r--   0        0        0      500 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/abstracts/embedded_document.py
+-rw-r--r--   0        0        0       55 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/abstracts/exceptions/__init__.py
+-rw-r--r--   0        0        0      776 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/abstracts/exceptions/document.py
+-rw-r--r--   0        0        0      728 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/fields/__init__.py
+-rw-r--r--   0        0        0     3406 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/fields/binary_field.py
+-rw-r--r--   0        0        0      473 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/fields/boolean_field.py
+-rw-r--r--   0        0        0     2478 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/fields/datetime_field.py
+-rw-r--r--   0        0        0     1832 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/fields/embedded_document_field.py
+-rw-r--r--   0        0        0     1478 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/fields/enum_field.py
+-rw-r--r--   0        0        0      571 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/fields/exceptions/__init__.py
+-rw-r--r--   0        0        0      444 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/fields/exceptions/binary_field.py
+-rw-r--r--   0        0        0      101 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/fields/exceptions/boolean_field.py
+-rw-r--r--   0        0        0      340 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/fields/exceptions/datetime_field.py
+-rw-r--r--   0        0        0      246 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/fields/exceptions/embedded_document_field.py
+-rw-r--r--   0        0        0      332 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/fields/exceptions/enum_field.py
+-rw-r--r--   0        0        0      300 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/fields/exceptions/float_field.py
+-rw-r--r--   0        0        0      211 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/fields/exceptions/geojson_field.py
+-rw-r--r--   0        0        0      328 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/fields/exceptions/integer_field.py
+-rw-r--r--   0        0        0      315 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/fields/exceptions/list_field.py
+-rw-r--r--   0        0        0      454 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/fields/exceptions/string_field.py
+-rw-r--r--   0        0        0      777 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/fields/field.py
+-rw-r--r--   0        0        0     1322 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/fields/float_field.py
+-rw-r--r--   0        0        0     1799 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/fields/geojson_field.py
+-rw-r--r--   0        0        0     1038 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/fields/integer_field.py
+-rw-r--r--   0        0        0      840 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/fields/list_field.py
+-rw-r--r--   0        0        0     2370 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/fields/reference_field.py
+-rw-r--r--   0        0        0     1315 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/fields/string_field.py
+-rw-r--r--   0        0        0       55 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/mongo/__init__.py
+-rw-r--r--   0        0        0     2847 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/mongo/database.py
+-rw-r--r--   0        0        0        0 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/utils/__init__.py
+-rw-r--r--   0        0        0     1889 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/utils/formatter.py
+-rw-r--r--   0        0        0      256 2024-02-20 17:33:49.610586 motormongo-0.1.9/motormongo/utils/logging.py
+-rw-r--r--   0        0        0     1011 2024-02-20 17:33:49.610586 motormongo-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    35042 1970-01-01 00:00:00.000000 motormongo-0.1.9/PKG-INFO
```

### Comparing `motormongo-0.1.8/LICENSE` & `motormongo-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `motormongo-0.1.8/README.md` & `motormongo-0.1.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,17 @@
 
 1. [Installation](#installation)
 2. [Quickstart](#quickstart)
 3. [motormongo Fields](#motormongo-fields)
 4. [CRUD classmethods](#class-methods)
 5. [CRUD instance methods](#instance-methods)
 6. [Aggregation Operations](#aggregation)
-7. [FastAPI integration](#fastapi-integration)
-8. [License](#license)
+7. [Polymorphism and Inheritance](#polymorphism-and-inheritance)
+8. [FastAPI integration](#fastapi-integration)
+9. [License](#license)
 
 ## Installation
 
 To install motormongo, you can use `pip` inside your virtual environment:
 
 ```shell
 python -m pip install motormongo
@@ -133,15 +134,16 @@
 ```python
 import bcrypt
 
 await User.insert_one(
     {
         "username": "johndoe",
         "email": "johndoe@portmarnock.ie",
-        "password": "password123" # < hash_functon will hash the string literal password and store binary field in the database
+        "password": "password123"
+        # < hash_functon will hash the string literal password and store binary field in the database
     }
 )
 ```
 
 ### Step 4: Validate user was created in your MongoDB collection
 
 You can do this by using [MongoDB compass]() GUI, or alternatively, add a query to find all documents in the user
@@ -198,44 +200,61 @@
 - [IntegerField](#integerfield): Manages integer data, allowing specifications for minimum and maximum values.
 - [ListField](#listfield): Handles lists of items, which can be of any type.
 - [ReferenceField](#referencefield): Creates a reference to another document.
 - [StringField](#stringfield): Handles string data with options for minimum and maximum length, and regex validation.
 
 ### BinaryField
 
-The `BinaryField` is designed for storing binary data within a database. It offers capabilities for encoding, hashing, and decoding data, making it versatile for handling various types of binary data, including but not limited to encrypted or hashed content.
+The `BinaryField` is designed for storing binary data within a database. It offers capabilities for encoding, hashing,
+and decoding data, making it versatile for handling various types of binary data, including but not limited to encrypted
+or hashed content.
 
 **Parameters:**
 
-- `hash_function`: (Optional) A callable that hashes input data. The function should have a type annotation to indicate whether it expects a `str` or `bytes` as input. This annotation is crucial as it dictates whether the `BinaryField` should encode the string before hashing. If the annotation indicates `str`, the field will pass the string directly to the `hash_function`. If `bytes`, the `BinaryField` will encode the string (using the provided `encode` function or default UTF-8 encoding) before hashing.
-- `return_decoded`: (Optional) A boolean indicating whether to decode binary data when it is retrieved from the database. If set to `True`, the stored binary data will be decoded back into a string using the provided `decode` function or default UTF-8 decoding. This is useful for data that was encoded but not hashed, as hashed data cannot be meaningfully decoded.
-- `encode`: (Optional) A function to encode a string to bytes before storage. If not provided, the class defaults to UTF-8 encoding. This function is used when the input data is a string and needs to be stored as binary data, or before hashing if the `hash_function` expects `bytes`.
-- `decode`: (Optional) A function to decode bytes back to a string when data is retrieved from the database. This parameter is only relevant if `return_decoded` is `True`. If not provided, the class defaults to UTF-8 decoding.
-
-**Important**: For the `hash_function` to work correctly with the `BinaryField`, it must include type annotations for its parameters. This enables the `BinaryField` to determine the correct processing strategy (i.e., whether to encode the string before hashing).
+- `hash_function`: (Optional) A callable that hashes input data. The function should have a type annotation to indicate
+  whether it expects a `str` or `bytes` as input. This annotation is crucial as it dictates whether the `BinaryField`
+  should encode the string before hashing. If the annotation indicates `str`, the field will pass the string directly to
+  the `hash_function`. If `bytes`, the `BinaryField` will encode the string (using the provided `encode` function or
+  default UTF-8 encoding) before hashing.
+- `return_decoded`: (Optional) A boolean indicating whether to decode binary data when it is retrieved from the
+  database. If set to `True`, the stored binary data will be decoded back into a string using the provided `decode`
+  function or default UTF-8 decoding. This is useful for data that was encoded but not hashed, as hashed data cannot be
+  meaningfully decoded.
+- `encode`: (Optional) A function to encode a string to bytes before storage. If not provided, the class defaults to
+  UTF-8 encoding. This function is used when the input data is a string and needs to be stored as binary data, or before
+  hashing if the `hash_function` expects `bytes`.
+- `decode`: (Optional) A function to decode bytes back to a string when data is retrieved from the database. This
+  parameter is only relevant if `return_decoded` is `True`. If not provided, the class defaults to UTF-8 decoding.
+
+**Important**: For the `hash_function` to work correctly with the `BinaryField`, it must include type annotations for
+its parameters. This enables the `BinaryField` to determine the correct processing strategy (i.e., whether to encode the
+string before hashing).
 
 ### Example Usage:
 
 ```python
 from motormongo import Document, BinaryField, StringField
 import bcrypt
 
+
 # Hash function with type annotation indicating it expects a 'str'
 def hash_password(password: str) -> bytes:
     return bcrypt.hashpw(password.encode('utf-8'), bcrypt.gensalt())
 
+
 class User(Document):
     username = StringField(min_length=3, max_length=50)
     # Note: 'hash_function' requires a type annotation
     password = BinaryField(hash_function=hash_password, return_decoded=False)
 
     def verify_password(self, password: str) -> bool:
         # Verifies if the provided password matches the stored hash
         return bcrypt.checkpw(password.encode("utf-8"), self.password)
 
+
 # Creating a user instance with a hashed password
 user = User(username="johndoe", password="secret")
 inserted_user = await user.save()
 
 # Authentication checks
 is_authenticated = inserted_user.verify_password("wrongpassword")  # Expected to return False
 is_authenticated = inserted_user.verify_password("secret")  # Expected to return True
@@ -302,27 +321,30 @@
 
 **Example Usage:**
 
 ```python
 from motormongo import Document, EmbeddedDocument, EmbeddedDocumentField, StringField
 from pydantic import BaseModel
 
+
 class Address(EmbeddedDocument):
     street = StringField()
     city = StringField()
 
 
 class User(Document):
     name = StringField()
     address = EmbeddedDocumentField(document_type=Address)
 
+
 class PydanticAddress(BaseModel):
-    street: str 
+    street: str
     city: str
 
+
 # Create a user with an embedded address document
 user = User(name="John Doe", address={"street": "123 Elm St", "city": "Springfield"})
 # user = User(name="John Doe", address=Address(street="123 Elm St", city="Springfield")) # Also works
 # user = User(name="John Doe", address=PydanticAddress(street="123 Elm St", city="Springfield")) # Also works
 await user.save()
 ```
 
@@ -494,15 +516,16 @@
 
 if referenced_user:
     print("Referenced User:", referenced_user.to_dict())
 else:
     print("User not found or failed to fetch.")
 ```
 
-This example demonstrates how to access and asynchronously fetch the document referenced by a `ReferenceField`. The await
+This example demonstrates how to access and asynchronously fetch the document referenced by a `ReferenceField`. The
+await
 keyword is crucial because the operation is asynchronous, involving a database query to retrieve the referenced
 document.
 
 **Note:** Ensure that the fetching operation is performed within an asynchronous context, such as an async function. The
 ReferenceField provides a powerful way to manage relationships between documents, enabling complex data models with
 interconnected documents.
 
@@ -540,15 +563,15 @@
 The following class methods are supported by motormongo's `Document` class:
 
 | CRUD Type | Operation                                                                                                                          |
 |-----------|------------------------------------------------------------------------------------------------------------------------------------|
 | Create    | [`insert_one(document: dict, **kwargs) -> Document`](#insert_one)                                                                  |
 | Create    | [`insert_many(documents: List[dict]) -> Tuple[List[Document], Any]`](#insert_many)                                                 |
 | Read      | [`find_one(query: dict, **kwargs) -> Document`](#find_one)                                                                         |
-| Read      | [`find_many(query: dict, limit: int, **kwargs) -> List[Document]`](#find_many)                                                     |
+| Read      | [`find_many(query: dict, limit: int = None, return_as_list: bool = True **kwargs) -> List[Document]`](#find_many)                  |
 | Update    | [`update_one(query: dict, update_fields: dict) -> Document`](#update_one)                                                          |
 | Update    | [`update_many(query: dict, update_fields: dict) -> Tuple[List[Document], int]`](#update_many)                                      |
 | Delete    | [`delete_one(query: dict, **kwargs) -> bool`](#delete_one)                                                                         |
 | Delete    | [`delete_many(query: dict, **kwargs) -> int`](#delete_many)                                                                        |
 | Mixed     | [`find_one_or_create(query: dict, defaults: dict) -> Tuple[Document, bool]`](#find_one_or_create)                                  |
 | Mixed     | [`find_one_and_replace(query: dict, replacement: dict) -> Document`](#find_one_and_replace)                                        |
 | Mixed     | [`find_one_and_delete(query: dict) -> Document`](#find_one_and_delete)                                                             |
@@ -810,20 +833,23 @@
 # Recursively delete all User instances in the users list who are not alive
 for user in users:
     user.delete()
 ```
 
 ### Aggregation
 
-The `aggregate` class method is designed to perform aggregation operations on the documents within the collection. It allows the execution of a sequence of data aggregation operations defined by the `pipeline` parameter. This method can return the results either as a list of documents or as a cursor, based on the `return_as_list` flag.
+The `aggregate` class method is designed to perform aggregation operations on the documents within the collection. It
+allows the execution of a sequence of data aggregation operations defined by the `pipeline` parameter. This method can
+return the results either as a list of documents or as a cursor, based on the `return_as_list` flag.
 
 **Parameters:**
 
 - `pipeline`: A list of dictionaries defining the aggregation operations to be performed on the collection.
-- `return_as_list` (optional): A boolean flag that determines the format of the returned results. If set to `True`, the method returns a list of documents. If `False` (default), it returns a cursor.
+- `return_as_list` (optional): A boolean flag that determines the format of the returned results. If set to `True`, the
+  method returns a list of documents. If `False` (default), it returns a cursor.
 
 **Returns:**
 
 - If `return_as_list` is `True`, returns a list of documents resulting from the aggregation pipeline.
 - If `return_as_list` is `False`, returns a Cursor to iterate over the results.
 
 **Raises:**
@@ -849,14 +875,102 @@
     print(doc)
 
 # Execute the aggregation and return results as a list
 docs_list = await YourDocumentClass.aggregate(pipeline, return_as_list=True)
 print(docs_list)
 ```
 
+## Polymorphism and Inheritance
+
+This part of the documentation provides an overview of implementing and using polymorphism and inheritance using the
+motormongo framework, enabling flexible and organized data models for various use cases.
+
+### Base Model: Item
+
+The `Item` class serves as the base model for different types of items stored in a MongoDB collection. It defines common
+fields and methods that are shared across all item types.
+
+```python
+from motormongo import Document, StringField, FloatField
+
+
+class Item(Document):
+    name = StringField()
+    cost = FloatField()
+```
+
+### Subclass Models
+
+Subclasses of `Item` can introduce specific fields or override methods to cater to different item categories.
+
+#### Book
+
+A `Book` represents a specific type of `Item` with additional attributes related to books.
+
+```python
+class Book(Item):
+    title = StringField()
+    author = StringField()
+    isbn = StringField()
+```
+
+#### Electronics
+
+An `Electronics` item represents electronic goods with attributes like warranty period and brand.
+
+```python
+class Electronics(Item):
+    warranty_period = StringField()  # E.g., "2 years"
+    brand = StringField()
+```
+
+### Usage
+
+#### Creating and Inserting Items
+
+To insert items into the database, use the `insert_one` method. The item's type is managed automatically.
+
+```python
+# Insert a book
+book = await Book.insert_one(title="1984", author="George Orwell", isbn="123456789", cost=20.0, name="Book")
+
+# Insert an electronics item
+electronics = await Electronics.insert_one(warranty_period="2 years", brand="TechBrand", cost=999.99, name="Laptop")
+```
+
+#### Querying Items
+
+You can query items of any type using their base or specific models. Polymorphism allows retrieved instances to be of
+the correct subclass.
+
+```python
+# Find a book by ISBN
+found_book = await Book.find_one(isbn="123456789")
+
+# Find an electronics item by brand
+found_electronics = await Electronics.find_one(brand="TechBrand")
+```
+
+#### Polymorphic Behavior
+
+**Note** - The following behaviour is currently being tested and not available in v0.1.9.
+
+Querying on the base `Item` model returns items of all types, correctly instantiated as their specific subclasses.
+
+```python
+# Find all items with a cost over 50
+expensive_items = await Item.find_many(cost={"$gt": 50})
+
+for item in expensive_items:
+    print(type(item))  # Prints the subclass (Book, Electronics, etc.)
+    if isinstance(item, Book):
+        print(f"Book: {item.title} by {item.author}")
+    elif isinstance(item, Electronics):
+        print(f"Electronics: {item.brand} with {item.warranty_period} warranty")
+```
 
 ## FastAPI integration
 
 motormongo can be easily integrated in FastAPI APIs to leverage the asynchronous ability of
 FastAPI. To leverage motormongo's ease-of-use, Pydantic model's should be created to represent the MongoDB
 motormongo Document as a Pydantic model. Below is a light-weight CRUD FastAPI application using motormongo:
 
@@ -917,15 +1031,16 @@
 async def is_authenticated(username: str, password: str):
     user = await User.find_one({"username": username})
     if not user:
         raise HTTPException(status_code=404, detail="User not found")
     if not user.verify_password(password):
         raise HTTPException(status_code=401, detail="Unauthorized")
     else:
-      return "You are authenticated! You can see this!"
+        return "You are authenticated! You can see this!"
+
 
 @app.get("/users")
 async def get_users():
     users = await User.find_many()
     if not users:
         raise HTTPException(status_code=404, detail="User not found")
     return [user.to_dict() for user in users]
```

### Comparing `motormongo-0.1.8/motormongo/abstracts/document.py` & `motormongo-0.1.9/motormongo/abstracts/document.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 from enum import Enum
-from typing import Any, Dict, List, Tuple
+from typing import Any, Dict, List, Tuple, Union
 
 from bson import ObjectId
 from pymongo import ReturnDocument
 
 from motormongo.abstracts.exceptions import DocumentInsertError, DocumentNotFoundError, DocumentUpdateError, \
     DocumentDeleteError, DocumentAggregationError
 from motormongo.abstracts.embedded_document import EmbeddedDocument
@@ -25,15 +25,15 @@
 
     def __init__(cls, name, bases, attrs):
         super().__init__(name, bases, attrs)
         if not hasattr(cls, "_registered_documents"):
             cls._registered_documents = []
         else:
             cls._registered_documents.append(cls)
-
+            logger.debug(f"Registered document class: {cls.__name__}")
 
 class Document(metaclass=DocumentMeta):
     """
     A base class for MongoDB document models, providing methods for mongo operations.
 
     This class provides asynchronous methods for CRUD (Create, Read, Update, Delete) operations
     and other utility functions for working with MongoDB documents. It should be subclassed to
@@ -81,38 +81,31 @@
         Args:
             **kwargs: Arbitrary keyword arguments which represent the attributes of the document.
 
         Note:
             - The 'created_at' attribute is set if provided in the keyword arguments.
         """
         self.__collection = self.get_collection_name()
-        self.__dict__[self.__type_field] = (
-            self.__class__.__name__
-        )  # Store class name in __type_field
+        self.__dict__[self.__type_field] = self.__class__.__name__
+        # Logging the class creation
         logger.debug(f"Creating class for collection {self.__collection}")
 
-        # Handling _id separately
+        # Handling '_id' separately
         if "_id" in kwargs:
             logger.debug(f"Setting _id: {kwargs['_id']}")
             setattr(self, "_id", ObjectId(kwargs["_id"]))
 
         # Setting other attributes
-        for name, field in self.__class__.__dict__.items():
-            if isinstance(field, Field):
-                logger.debug(
-                    f"{name} and value = {kwargs.get(name, field.options.get('default'))}"
-                )
-                # For non-ReferenceField fields or if the value is not a string, set it directly
-                if kwargs.get(name, field.options.get("default")) is not None:
-                    setattr(self, name, kwargs.get(name, field.options.get("default")))
-            else:
-                # todo: valid warn
-                NotImplemented
+        for cls in reversed(self.__class__.__mro__):  # Iterate through the MRO
+            for name, field in cls.__dict__.items():
+                if isinstance(field, Field):
+                    attr_value = kwargs.get(name, field.options.get('default'))
+                    if attr_value is not None:
+                        setattr(self, name, attr_value)
 
-        # # TODO: This should be set elsewhere?
         if "created_at" in kwargs:
             self.created_at = kwargs.get("created_at")
         if "updated_at" in kwargs:
             self.updated_at = kwargs.get("updated_at")
 
     def __init_subclass__(cls, **kwargs):
         """
@@ -139,24 +132,44 @@
 
         Note:
             - This is an asynchronous method and should be awaited.
         """
         return await get_db()
 
     @classmethod
-    def get_collection_name(cls):
+    def get_collection_name(cls) -> Union[str, List[str]]:
         """
-        Retrieves the collection name for the document class.
+        Retrieves the collection name for the document class or a list of collection names for its subclasses,
+        preferring explicitly defined collection names in the subclass's Meta attribute if available.
 
         Returns:
-            str: The collection name. If defined in the class's 'Meta' attribute, it uses that;
-                 otherwise, converts the class name from CamelCase to snake_case.
-        """
+            Union[str, List[str]]: The collection name for the current class, or, if the class has subclasses,
+                                    a list of collection names derived from either the subclass Meta attribute
+                                    or the subclass names.
+        """
+        # Check for an explicitly defined collection name in the current class's Meta attribute
+        # Check for subclasses
+        subclasses = cls.__subclasses__()
+        if subclasses:
+            # Initialize an empty list to store collection names for subclasses
+            subclass_collection_names = []
+            # Iterate over each subclass
+            for subcls in subclasses:
+                # Check for an explicitly defined collection name in the subclass's Meta attribute
+                if hasattr(subcls, "Meta") and hasattr(subcls.Meta, "collection"):
+                    subclass_collection_names.append(subcls.Meta.collection)
+                else:
+                    # If no explicit collection name is defined, convert the subclass name from CamelCase to snake_case
+                    subclass_collection_names.append(camel_to_snake_or_lower(subcls.__name__))
+            return subclass_collection_names
+
         if hasattr(cls, "Meta") and hasattr(cls.Meta, "collection"):
             return cls.Meta.collection
+
+        # If no subclasses exist, return the snake_case collection name for the current class
         return camel_to_snake_or_lower(cls.__name__)
 
     @classmethod
     def convert_id(cls, query):
         """
         Converts the '_id' field in the query to an ObjectId, if necessary.
 
@@ -349,59 +362,77 @@
             logger.debug(f"__doc rep = {document}")
             return cls.from_dict(**document) if document else None
         except Exception as e:
             raise DocumentNotFoundError(f"Error finding {cls.__name__} document with query '{filter}': {e}")
 
     @classmethod
     async def find_many(
-            cls, query: Dict = None, limit: int = None, **kwargs
-    ) -> List["Document"]:
+            cls, query: Dict = None, limit: int = None, return_as_list: bool = True, **kwargs
+    ) -> Union[List["Document"], List[Any], Any]:
         """
-        Asynchronously retrieves multiple documents from the mongo collection that match the
-        given filter and limit.
+        Asynchronously retrieves multiple documents from one or more mongo collections that match the
+        given filter and limit. Optionally, it can return an AsyncIOMotorCursor instead of a list for each collection.
 
         This method allows you to query multiple documents based on the filter criteria. It supports
         both a filter dictionary and additional keyword arguments. You can also specify a limit on
-        the number of documents to retrieve.
+        the number of documents to retrieve and whether to return the results as a list or a cursor.
 
         Args:
             query (Dict, optional): A dictionary specifying the filter criteria for the query.
-                                     Defaults to None.
+                                    Defaults to None.
             limit (int, optional): The maximum number of documents to return. Defaults to None,
                                    which means no limit.
+            return_as_list (bool, optional): If True, returns a list of Documents. If False, returns a cursor.
+                                             Defaults to True.
             **kwargs: Additional filter criteria specified as keyword arguments.
 
         Returns:
-            List[Document]: A list of class instances representing the found documents. Returns an
-                            empty list if no documents match the filter criteria.
+            Union[List["Document"], List[AsyncIOMotorCursor], Any]: Depending on return_as_list, either a list of class instances
+                                                                    representing the found documents or an AsyncIOMotorCursor for each collection.
+                                                                    Returns an empty list if no documents match the filter criteria
+                                                                    and return_as_list is True.
 
         Raises:
             ValueError: If there is an error in finding the documents with the given filter.
-
-        Examples:
-            await MyClass.find_many(age={"$gt": 40}, alive=False, limit=20)
-            filter_criteria = {"age": {"$gt": 40}, "alive": False}
-            await MyClass.find_many(**filter_criteria, limit=20)
-
-        Note:
-            - The `filter` argument and keyword arguments are combined for the query.
-            - The `limit` argument restricts the number of returned documents.
         """
         filter = {**(query or {}), **kwargs}
+        combined_results = []  # Initialize a list to store combined results from all collections
+
         try:
             db = await cls.db()
-            collection = db[cls.get_collection_name()]
-            cursor = collection.find(filter)
-            if limit is not None:
-                cursor = cursor.limit(limit)
-            documents = await cursor.to_list(length=limit)
-            return [cls.from_dict(**doc) for doc in documents]
+            collection_names = cls.get_collection_name()  # This might return a single name or a list of names
+
+            if isinstance(collection_names, list):
+                # If get_collection_name returns a list, iterate over each collection name
+                for collection_name in collection_names:
+                    collection = db[collection_name]
+                    cursor = collection.find(filter)
+                    if limit is not None:
+                        cursor = cursor.limit(limit)
+                    if return_as_list:
+                        documents = await cursor.to_list(length=limit)
+                        combined_results.extend([cls.from_dict(**doc) for doc in documents])
+                    else:
+                        combined_results.append(cursor)
+            else:
+                # Single collection name case
+                collection = db[collection_names]
+                cursor = collection.find(filter)
+                if limit is not None:
+                    cursor = cursor.limit(limit)
+                if return_as_list:
+                    documents = await cursor.to_list(length=limit)
+                    combined_results = [cls.from_dict(**doc) for doc in documents]
+                else:
+                    combined_results = cursor
+
+            return combined_results
         except Exception as e:
+            logger.debug(f"Failed to retrieve documents for {cls.__name__} with query '{filter}': {str(e)}")
             raise DocumentNotFoundError(f"Error finding {cls.__name__} documents with query '{filter}': {e}")
-
     @classmethod
     async def update_one(cls, query: Dict, update_fields: Dict) -> "Document":
         """
         Asynchronously updates a single document in the mongo collection based on the provided query and update fields.
 
         This method finds a single document matching the query criteria and updates it with the specified fields.
         It returns the updated document as an instance of the class. The method also supports additional
@@ -826,34 +857,61 @@
 
         Returns:
             str: A JSON string representation of the document.
         """
         return json.dumps(self.to_dict(), default=self._json_encoder)
 
     @classmethod
+    def _get_class_from_type(cls, type_name: str):
+        """
+        Finds the subclass based on the provided type name.
+
+        Args:
+            type_name (str): The name of the subclass as stored in the document's __type field.
+
+        Returns:
+            The class object corresponding to the type name, or None if no matching class is found.
+        """
+        if not type_name:
+            logger.debug("No type name provided for _get_class_from_type.")
+            return None
+
+        for subclass in cls._registered_documents:
+            if subclass.__name__ == type_name:
+                logger.debug(f"Found matching class '{type_name}' for document instantiation.")
+                return subclass
+
+        logger.warning(f"No matching class found for type name '{type_name}'.")
+        return None
+
+    @classmethod
     def from_dict(cls, **kwargs):
         """
         Factory method to instantiate objects of the correct subclass based on the document's
         __type field. This method ensures that each document is deserialized into an instance
         of the appropriate class.
 
         Returns:
             Document: An instance of the appropriate subclass of Document.
         """
         # Extract the class name from the document's __type field
-        class_name = kwargs.get(cls.__type_field)
+        class_name = kwargs.get(cls.__type_field, None)
 
-        # Find the correct class to instantiate
         if class_name:
             for subclass in cls._registered_documents:
                 if subclass.__name__ == class_name:
-                    # Instantiate the subclass with the document's data
+                    logger.debug(f"Instantiating {class_name} from document data.")
                     return subclass(**kwargs)
+            # Log a warning if no registered subclass matches the class_name
+            logger.debug(
+                f"Unknown class name '{class_name}' in document data. Falling back to base class {cls.__name__}.")
+        else:
+            # Log a debug message if __type field is missing
+            logger.debug(f"__type field missing in document data. Instantiating base class {cls.__name__}.")
 
-        # Fallback to the base class if the class name is not found or __type is missing
         return cls(**kwargs)
 
     def to_dict(self, id_as_string=True):
         """
         Converts the document to a dictionary representation, including type information
         and using field-specific __get__ methods for serialization where applicable.
```

### Comparing `motormongo-0.1.8/motormongo/abstracts/exceptions/document.py` & `motormongo-0.1.9/motormongo/abstracts/exceptions/document.py`

 * *Files identical despite different names*

### Comparing `motormongo-0.1.8/motormongo/fields/__init__.py` & `motormongo-0.1.9/motormongo/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `motormongo-0.1.8/motormongo/fields/binary_field.py` & `motormongo-0.1.9/motormongo/fields/binary_field.py`

 * *Files identical despite different names*

### Comparing `motormongo-0.1.8/motormongo/fields/datetime_field.py` & `motormongo-0.1.9/motormongo/fields/datetime_field.py`

 * *Files identical despite different names*

### Comparing `motormongo-0.1.8/motormongo/fields/embedded_document_field.py` & `motormongo-0.1.9/motormongo/fields/embedded_document_field.py`

 * *Files identical despite different names*

### Comparing `motormongo-0.1.8/motormongo/fields/enum_field.py` & `motormongo-0.1.9/motormongo/fields/enum_field.py`

 * *Files identical despite different names*

### Comparing `motormongo-0.1.8/motormongo/fields/exceptions/__init__.py` & `motormongo-0.1.9/motormongo/fields/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `motormongo-0.1.8/motormongo/fields/field.py` & `motormongo-0.1.9/motormongo/fields/field.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,9 +10,9 @@
     def __get__(self, obj, objtype=None):
         return obj.__dict__.get(self.name, self.options.get("default"))
 
     def __set__(self, obj, value):
         # Check against all allowed types
         if not any(isinstance(value, t) for t in self.type if t is not None):
             allowed_types = ", ".join(t.__name__ for t in self.type if t is not None)
-            raise TypeError(f"Value for {self.name} must be of type {allowed_types}")
+            raise TypeError(f"Value for {self.name} must be of type {allowed_types}. Got {type(value)}.")
         obj.__dict__[self.name] = value
```

### Comparing `motormongo-0.1.8/motormongo/fields/float_field.py` & `motormongo-0.1.9/motormongo/fields/float_field.py`

 * *Files identical despite different names*

### Comparing `motormongo-0.1.8/motormongo/fields/geojson_field.py` & `motormongo-0.1.9/motormongo/fields/geojson_field.py`

 * *Files identical despite different names*

### Comparing `motormongo-0.1.8/motormongo/fields/integer_field.py` & `motormongo-0.1.9/motormongo/fields/integer_field.py`

 * *Files identical despite different names*

### Comparing `motormongo-0.1.8/motormongo/fields/list_field.py` & `motormongo-0.1.9/motormongo/fields/list_field.py`

 * *Files identical despite different names*

### Comparing `motormongo-0.1.8/motormongo/fields/reference_field.py` & `motormongo-0.1.9/motormongo/fields/reference_field.py`

 * *Files identical despite different names*

### Comparing `motormongo-0.1.8/motormongo/fields/string_field.py` & `motormongo-0.1.9/motormongo/fields/string_field.py`

 * *Files identical despite different names*

### Comparing `motormongo-0.1.8/motormongo/mongo/database.py` & `motormongo-0.1.9/motormongo/mongo/database.py`

 * *Files identical despite different names*

### Comparing `motormongo-0.1.8/motormongo/utils/formatter.py` & `motormongo-0.1.9/motormongo/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `motormongo-0.1.8/pyproject.toml` & `motormongo-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motormongo"
-version = "0.1.8"
+version = "0.1.9"
 description = "An asynchronous Object Document Mapper (O.D.M) for MongoDB built on-top of Motor."
 authors = ["pprunty <pprunty@tcd.ie>"]
 readme = "README.md"
 license = "MIT"
 include = [
     "motormongo/*.py",
     "motormongo/*/*.py",
```

### Comparing `motormongo-0.1.8/PKG-INFO` & `motormongo-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motormongo
-Version: 0.1.8
+Version: 0.1.9
 Summary: An asynchronous Object Document Mapper (O.D.M) for MongoDB built on-top of Motor.
 License: MIT
 Author: pprunty
 Author-email: pprunty@tcd.ie
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -40,16 +40,17 @@
 
 1. [Installation](#installation)
 2. [Quickstart](#quickstart)
 3. [motormongo Fields](#motormongo-fields)
 4. [CRUD classmethods](#class-methods)
 5. [CRUD instance methods](#instance-methods)
 6. [Aggregation Operations](#aggregation)
-7. [FastAPI integration](#fastapi-integration)
-8. [License](#license)
+7. [Polymorphism and Inheritance](#polymorphism-and-inheritance)
+8. [FastAPI integration](#fastapi-integration)
+9. [License](#license)
 
 ## Installation
 
 To install motormongo, you can use `pip` inside your virtual environment:
 
 ```shell
 python -m pip install motormongo
@@ -148,15 +149,16 @@
 ```python
 import bcrypt
 
 await User.insert_one(
     {
         "username": "johndoe",
         "email": "johndoe@portmarnock.ie",
-        "password": "password123" # < hash_functon will hash the string literal password and store binary field in the database
+        "password": "password123"
+        # < hash_functon will hash the string literal password and store binary field in the database
     }
 )
 ```
 
 ### Step 4: Validate user was created in your MongoDB collection
 
 You can do this by using [MongoDB compass]() GUI, or alternatively, add a query to find all documents in the user
@@ -213,44 +215,61 @@
 - [IntegerField](#integerfield): Manages integer data, allowing specifications for minimum and maximum values.
 - [ListField](#listfield): Handles lists of items, which can be of any type.
 - [ReferenceField](#referencefield): Creates a reference to another document.
 - [StringField](#stringfield): Handles string data with options for minimum and maximum length, and regex validation.
 
 ### BinaryField
 
-The `BinaryField` is designed for storing binary data within a database. It offers capabilities for encoding, hashing, and decoding data, making it versatile for handling various types of binary data, including but not limited to encrypted or hashed content.
+The `BinaryField` is designed for storing binary data within a database. It offers capabilities for encoding, hashing,
+and decoding data, making it versatile for handling various types of binary data, including but not limited to encrypted
+or hashed content.
 
 **Parameters:**
 
-- `hash_function`: (Optional) A callable that hashes input data. The function should have a type annotation to indicate whether it expects a `str` or `bytes` as input. This annotation is crucial as it dictates whether the `BinaryField` should encode the string before hashing. If the annotation indicates `str`, the field will pass the string directly to the `hash_function`. If `bytes`, the `BinaryField` will encode the string (using the provided `encode` function or default UTF-8 encoding) before hashing.
-- `return_decoded`: (Optional) A boolean indicating whether to decode binary data when it is retrieved from the database. If set to `True`, the stored binary data will be decoded back into a string using the provided `decode` function or default UTF-8 decoding. This is useful for data that was encoded but not hashed, as hashed data cannot be meaningfully decoded.
-- `encode`: (Optional) A function to encode a string to bytes before storage. If not provided, the class defaults to UTF-8 encoding. This function is used when the input data is a string and needs to be stored as binary data, or before hashing if the `hash_function` expects `bytes`.
-- `decode`: (Optional) A function to decode bytes back to a string when data is retrieved from the database. This parameter is only relevant if `return_decoded` is `True`. If not provided, the class defaults to UTF-8 decoding.
-
-**Important**: For the `hash_function` to work correctly with the `BinaryField`, it must include type annotations for its parameters. This enables the `BinaryField` to determine the correct processing strategy (i.e., whether to encode the string before hashing).
+- `hash_function`: (Optional) A callable that hashes input data. The function should have a type annotation to indicate
+  whether it expects a `str` or `bytes` as input. This annotation is crucial as it dictates whether the `BinaryField`
+  should encode the string before hashing. If the annotation indicates `str`, the field will pass the string directly to
+  the `hash_function`. If `bytes`, the `BinaryField` will encode the string (using the provided `encode` function or
+  default UTF-8 encoding) before hashing.
+- `return_decoded`: (Optional) A boolean indicating whether to decode binary data when it is retrieved from the
+  database. If set to `True`, the stored binary data will be decoded back into a string using the provided `decode`
+  function or default UTF-8 decoding. This is useful for data that was encoded but not hashed, as hashed data cannot be
+  meaningfully decoded.
+- `encode`: (Optional) A function to encode a string to bytes before storage. If not provided, the class defaults to
+  UTF-8 encoding. This function is used when the input data is a string and needs to be stored as binary data, or before
+  hashing if the `hash_function` expects `bytes`.
+- `decode`: (Optional) A function to decode bytes back to a string when data is retrieved from the database. This
+  parameter is only relevant if `return_decoded` is `True`. If not provided, the class defaults to UTF-8 decoding.
+
+**Important**: For the `hash_function` to work correctly with the `BinaryField`, it must include type annotations for
+its parameters. This enables the `BinaryField` to determine the correct processing strategy (i.e., whether to encode the
+string before hashing).
 
 ### Example Usage:
 
 ```python
 from motormongo import Document, BinaryField, StringField
 import bcrypt
 
+
 # Hash function with type annotation indicating it expects a 'str'
 def hash_password(password: str) -> bytes:
     return bcrypt.hashpw(password.encode('utf-8'), bcrypt.gensalt())
 
+
 class User(Document):
     username = StringField(min_length=3, max_length=50)
     # Note: 'hash_function' requires a type annotation
     password = BinaryField(hash_function=hash_password, return_decoded=False)
 
     def verify_password(self, password: str) -> bool:
         # Verifies if the provided password matches the stored hash
         return bcrypt.checkpw(password.encode("utf-8"), self.password)
 
+
 # Creating a user instance with a hashed password
 user = User(username="johndoe", password="secret")
 inserted_user = await user.save()
 
 # Authentication checks
 is_authenticated = inserted_user.verify_password("wrongpassword")  # Expected to return False
 is_authenticated = inserted_user.verify_password("secret")  # Expected to return True
@@ -317,27 +336,30 @@
 
 **Example Usage:**
 
 ```python
 from motormongo import Document, EmbeddedDocument, EmbeddedDocumentField, StringField
 from pydantic import BaseModel
 
+
 class Address(EmbeddedDocument):
     street = StringField()
     city = StringField()
 
 
 class User(Document):
     name = StringField()
     address = EmbeddedDocumentField(document_type=Address)
 
+
 class PydanticAddress(BaseModel):
-    street: str 
+    street: str
     city: str
 
+
 # Create a user with an embedded address document
 user = User(name="John Doe", address={"street": "123 Elm St", "city": "Springfield"})
 # user = User(name="John Doe", address=Address(street="123 Elm St", city="Springfield")) # Also works
 # user = User(name="John Doe", address=PydanticAddress(street="123 Elm St", city="Springfield")) # Also works
 await user.save()
 ```
 
@@ -509,15 +531,16 @@
 
 if referenced_user:
     print("Referenced User:", referenced_user.to_dict())
 else:
     print("User not found or failed to fetch.")
 ```
 
-This example demonstrates how to access and asynchronously fetch the document referenced by a `ReferenceField`. The await
+This example demonstrates how to access and asynchronously fetch the document referenced by a `ReferenceField`. The
+await
 keyword is crucial because the operation is asynchronous, involving a database query to retrieve the referenced
 document.
 
 **Note:** Ensure that the fetching operation is performed within an asynchronous context, such as an async function. The
 ReferenceField provides a powerful way to manage relationships between documents, enabling complex data models with
 interconnected documents.
 
@@ -555,15 +578,15 @@
 The following class methods are supported by motormongo's `Document` class:
 
 | CRUD Type | Operation                                                                                                                          |
 |-----------|------------------------------------------------------------------------------------------------------------------------------------|
 | Create    | [`insert_one(document: dict, **kwargs) -> Document`](#insert_one)                                                                  |
 | Create    | [`insert_many(documents: List[dict]) -> Tuple[List[Document], Any]`](#insert_many)                                                 |
 | Read      | [`find_one(query: dict, **kwargs) -> Document`](#find_one)                                                                         |
-| Read      | [`find_many(query: dict, limit: int, **kwargs) -> List[Document]`](#find_many)                                                     |
+| Read      | [`find_many(query: dict, limit: int = None, return_as_list: bool = True **kwargs) -> List[Document]`](#find_many)                  |
 | Update    | [`update_one(query: dict, update_fields: dict) -> Document`](#update_one)                                                          |
 | Update    | [`update_many(query: dict, update_fields: dict) -> Tuple[List[Document], int]`](#update_many)                                      |
 | Delete    | [`delete_one(query: dict, **kwargs) -> bool`](#delete_one)                                                                         |
 | Delete    | [`delete_many(query: dict, **kwargs) -> int`](#delete_many)                                                                        |
 | Mixed     | [`find_one_or_create(query: dict, defaults: dict) -> Tuple[Document, bool]`](#find_one_or_create)                                  |
 | Mixed     | [`find_one_and_replace(query: dict, replacement: dict) -> Document`](#find_one_and_replace)                                        |
 | Mixed     | [`find_one_and_delete(query: dict) -> Document`](#find_one_and_delete)                                                             |
@@ -825,20 +848,23 @@
 # Recursively delete all User instances in the users list who are not alive
 for user in users:
     user.delete()
 ```
 
 ### Aggregation
 
-The `aggregate` class method is designed to perform aggregation operations on the documents within the collection. It allows the execution of a sequence of data aggregation operations defined by the `pipeline` parameter. This method can return the results either as a list of documents or as a cursor, based on the `return_as_list` flag.
+The `aggregate` class method is designed to perform aggregation operations on the documents within the collection. It
+allows the execution of a sequence of data aggregation operations defined by the `pipeline` parameter. This method can
+return the results either as a list of documents or as a cursor, based on the `return_as_list` flag.
 
 **Parameters:**
 
 - `pipeline`: A list of dictionaries defining the aggregation operations to be performed on the collection.
-- `return_as_list` (optional): A boolean flag that determines the format of the returned results. If set to `True`, the method returns a list of documents. If `False` (default), it returns a cursor.
+- `return_as_list` (optional): A boolean flag that determines the format of the returned results. If set to `True`, the
+  method returns a list of documents. If `False` (default), it returns a cursor.
 
 **Returns:**
 
 - If `return_as_list` is `True`, returns a list of documents resulting from the aggregation pipeline.
 - If `return_as_list` is `False`, returns a Cursor to iterate over the results.
 
 **Raises:**
@@ -864,14 +890,102 @@
     print(doc)
 
 # Execute the aggregation and return results as a list
 docs_list = await YourDocumentClass.aggregate(pipeline, return_as_list=True)
 print(docs_list)
 ```
 
+## Polymorphism and Inheritance
+
+This part of the documentation provides an overview of implementing and using polymorphism and inheritance using the
+motormongo framework, enabling flexible and organized data models for various use cases.
+
+### Base Model: Item
+
+The `Item` class serves as the base model for different types of items stored in a MongoDB collection. It defines common
+fields and methods that are shared across all item types.
+
+```python
+from motormongo import Document, StringField, FloatField
+
+
+class Item(Document):
+    name = StringField()
+    cost = FloatField()
+```
+
+### Subclass Models
+
+Subclasses of `Item` can introduce specific fields or override methods to cater to different item categories.
+
+#### Book
+
+A `Book` represents a specific type of `Item` with additional attributes related to books.
+
+```python
+class Book(Item):
+    title = StringField()
+    author = StringField()
+    isbn = StringField()
+```
+
+#### Electronics
+
+An `Electronics` item represents electronic goods with attributes like warranty period and brand.
+
+```python
+class Electronics(Item):
+    warranty_period = StringField()  # E.g., "2 years"
+    brand = StringField()
+```
+
+### Usage
+
+#### Creating and Inserting Items
+
+To insert items into the database, use the `insert_one` method. The item's type is managed automatically.
+
+```python
+# Insert a book
+book = await Book.insert_one(title="1984", author="George Orwell", isbn="123456789", cost=20.0, name="Book")
+
+# Insert an electronics item
+electronics = await Electronics.insert_one(warranty_period="2 years", brand="TechBrand", cost=999.99, name="Laptop")
+```
+
+#### Querying Items
+
+You can query items of any type using their base or specific models. Polymorphism allows retrieved instances to be of
+the correct subclass.
+
+```python
+# Find a book by ISBN
+found_book = await Book.find_one(isbn="123456789")
+
+# Find an electronics item by brand
+found_electronics = await Electronics.find_one(brand="TechBrand")
+```
+
+#### Polymorphic Behavior
+
+**Note** - The following behaviour is currently being tested and not available in v0.1.9.
+
+Querying on the base `Item` model returns items of all types, correctly instantiated as their specific subclasses.
+
+```python
+# Find all items with a cost over 50
+expensive_items = await Item.find_many(cost={"$gt": 50})
+
+for item in expensive_items:
+    print(type(item))  # Prints the subclass (Book, Electronics, etc.)
+    if isinstance(item, Book):
+        print(f"Book: {item.title} by {item.author}")
+    elif isinstance(item, Electronics):
+        print(f"Electronics: {item.brand} with {item.warranty_period} warranty")
+```
 
 ## FastAPI integration
 
 motormongo can be easily integrated in FastAPI APIs to leverage the asynchronous ability of
 FastAPI. To leverage motormongo's ease-of-use, Pydantic model's should be created to represent the MongoDB
 motormongo Document as a Pydantic model. Below is a light-weight CRUD FastAPI application using motormongo:
 
@@ -932,15 +1046,16 @@
 async def is_authenticated(username: str, password: str):
     user = await User.find_one({"username": username})
     if not user:
         raise HTTPException(status_code=404, detail="User not found")
     if not user.verify_password(password):
         raise HTTPException(status_code=401, detail="Unauthorized")
     else:
-      return "You are authenticated! You can see this!"
+        return "You are authenticated! You can see this!"
+
 
 @app.get("/users")
 async def get_users():
     users = await User.find_many()
     if not users:
         raise HTTPException(status_code=404, detail="User not found")
     return [user.to_dict() for user in users]
```

