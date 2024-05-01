# Comparing `tmp/metasequoia-sql-0.3.0.tar.gz` & `tmp/metasequoia-sql-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metasequoia-sql-0.3.0.tar", last modified: Mon Apr 15 01:03:43 2024, max compression
+gzip compressed data, was "metasequoia-sql-0.4.0.tar", last modified: Wed May  1 05:00:48 2024, max compression
```

## Comparing `metasequoia-sql-0.3.0.tar` & `metasequoia-sql-0.4.0.tar`

### file list

```diff
@@ -1,34 +1,59 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 01:03:43.089912 metasequoia-sql-0.3.0/
--rw-rw-rw-   0        0        0     1088 2024-03-11 00:28:43.000000 metasequoia-sql-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     7222 2024-04-15 01:03:43.089912 metasequoia-sql-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     6553 2024-04-15 01:00:03.000000 metasequoia-sql-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 01:03:43.081409 metasequoia-sql-0.3.0/metasequoia_sql/
--rw-rw-rw-   0        0        0      183 2024-04-15 00:51:46.000000 metasequoia-sql-0.3.0/metasequoia_sql/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 01:03:43.083408 metasequoia-sql-0.3.0/metasequoia_sql/analyzer/
--rw-rw-rw-   0        0        0        0 2024-04-15 00:51:46.000000 metasequoia-sql-0.3.0/metasequoia_sql/analyzer/__init__.py
--rw-rw-rw-   0        0        0     1009 2024-04-15 00:51:46.000000 metasequoia-sql-0.3.0/metasequoia_sql/analyzer/data_lineage.py
-drwxrwxrwx   0        0        0        0 2024-04-15 01:03:43.085409 metasequoia-sql-0.3.0/metasequoia_sql/ast/
--rw-rw-rw-   0        0        0      136 2024-04-15 00:51:46.000000 metasequoia-sql-0.3.0/metasequoia_sql/ast/__init__.py
--rw-rw-rw-   0        0        0     8793 2024-04-15 00:51:46.000000 metasequoia-sql-0.3.0/metasequoia_sql/ast/nodes.py
--rw-rw-rw-   0        0        0    15035 2024-04-15 00:51:46.000000 metasequoia-sql-0.3.0/metasequoia_sql/ast/parser.py
--rw-rw-rw-   0        0        0     5622 2024-04-15 00:51:46.000000 metasequoia-sql-0.3.0/metasequoia_sql/ast/static.py
-drwxrwxrwx   0        0        0        0 2024-04-15 01:03:43.087409 metasequoia-sql-0.3.0/metasequoia_sql/common/
--rw-rw-rw-   0        0        0      209 2024-04-15 00:51:46.000000 metasequoia-sql-0.3.0/metasequoia_sql/common/__init__.py
--rw-rw-rw-   0        0        0     3937 2024-04-15 00:51:46.000000 metasequoia-sql-0.3.0/metasequoia_sql/common/base_scanner.py
--rw-rw-rw-   0        0        0      601 2024-04-15 00:51:46.000000 metasequoia-sql-0.3.0/metasequoia_sql/common/basic.py
--rw-rw-rw-   0        0        0      226 2024-04-15 00:51:46.000000 metasequoia-sql-0.3.0/metasequoia_sql/common/text_scanner.py
--rw-rw-rw-   0        0        0     5612 2024-04-15 00:51:46.000000 metasequoia-sql-0.3.0/metasequoia_sql/common/token_scanner.py
-drwxrwxrwx   0        0        0        0 2024-04-15 01:03:43.088409 metasequoia-sql-0.3.0/metasequoia_sql/core/
--rw-rw-rw-   0        0        0      116 2024-04-15 00:51:46.000000 metasequoia-sql-0.3.0/metasequoia_sql/core/__init__.py
--rw-rw-rw-   0        0        0    84297 2024-04-15 00:51:46.000000 metasequoia-sql-0.3.0/metasequoia_sql/core/objects.py
--rw-rw-rw-   0        0        0    69929 2024-04-15 00:51:46.000000 metasequoia-sql-0.3.0/metasequoia_sql/core/parser.py
--rw-rw-rw-   0        0        0      405 2024-04-15 00:51:46.000000 metasequoia-sql-0.3.0/metasequoia_sql/core/static.py
--rw-rw-rw-   0        0        0      592 2024-04-11 15:14:53.000000 metasequoia-sql-0.3.0/metasequoia_sql/errors.py
--rw-rw-rw-   0        0        0     1041 2024-04-11 15:14:53.000000 metasequoia-sql-0.3.0/metasequoia_sql/static.py
-drwxrwxrwx   0        0        0        0 2024-04-15 01:03:43.088409 metasequoia-sql-0.3.0/metasequoia_sql.egg-info/
--rw-rw-rw-   0        0        0     7222 2024-04-15 01:03:43.000000 metasequoia-sql-0.3.0/metasequoia_sql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      773 2024-04-15 01:03:43.000000 metasequoia-sql-0.3.0/metasequoia_sql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 01:03:43.000000 metasequoia-sql-0.3.0/metasequoia_sql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-15 01:03:43.000000 metasequoia-sql-0.3.0/metasequoia_sql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 01:03:43.089912 metasequoia-sql-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1042 2024-04-15 00:52:01.000000 metasequoia-sql-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 05:00:48.883267 metasequoia-sql-0.4.0/
+-rw-rw-rw-   0        0        0     1088 2024-03-11 00:28:43.000000 metasequoia-sql-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0     8033 2024-05-01 05:00:48.883267 metasequoia-sql-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7251 2024-05-01 04:51:45.000000 metasequoia-sql-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 05:00:48.867143 metasequoia-sql-0.4.0/metasequoia_sql/
+-rw-rw-rw-   0        0        0      183 2024-04-15 00:51:46.000000 metasequoia-sql-0.4.0/metasequoia_sql/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 05:00:48.871036 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/
+-rw-rw-rw-   0        0        0      372 2024-04-18 23:36:58.000000 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/__init__.py
+-rw-rw-rw-   0        0        0     1728 2024-04-25 00:15:28.000000 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/all_level_common_table.py
+-rw-rw-rw-   0        0        0    10168 2024-05-01 00:26:31.000000 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/base.py
+-rw-rw-rw-   0        0        0    13204 2024-05-01 00:26:31.000000 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/current_level_common_column.py
+-rw-rw-rw-   0        0        0     3179 2024-04-25 00:15:28.000000 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/current_level_common_table.py
+drwxrwxrwx   0        0        0        0 2024-05-01 05:00:48.872982 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/data_linage/
+-rw-rw-rw-   0        0        0       39 2024-04-26 23:40:20.000000 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/data_linage/__init__.py
+-rw-rw-rw-   0        0        0     2290 2024-05-01 04:30:17.000000 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/data_linage/node.py
+-rw-rw-rw-   0        0        0     4788 2024-05-01 04:36:11.000000 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/data_linage/table_lineage.py
+-rw-rw-rw-   0        0        0    14940 2024-05-01 04:35:46.000000 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/data_linage/table_lineage_analyzer.py
+-rw-rw-rw-   0        0        0     1811 2024-05-01 03:35:36.000000 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/data_linage/table_lineage_storage.py
+-rw-rw-rw-   0        0        0    12263 2024-04-26 00:42:26.000000 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/data_lineage_analyzer_by_meta.py
+-rw-rw-rw-   0        0        0     4333 2024-04-25 00:15:28.000000 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/tool.py
+drwxrwxrwx   0        0        0        0 2024-05-01 05:00:48.873956 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/toolkit/
+-rw-rw-rw-   0        0        0      307 2024-05-01 04:00:55.000000 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/toolkit/__init__.py
+-rw-rw-rw-   0        0        0     1344 2024-05-01 00:26:31.000000 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/toolkit/current_level_sub_query.py
+-rw-rw-rw-   0        0        0     2189 2024-05-01 03:39:46.000000 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/toolkit/current_level_table_name_analyzer.py
+-rw-rw-rw-   0        0        0     1306 2024-05-01 04:27:55.000000 metasequoia-sql-0.4.0/metasequoia_sql/analyzer/toolkit/current_level_used_quote_columns.py
+drwxrwxrwx   0        0        0        0 2024-05-01 05:00:48.876444 metasequoia-sql-0.4.0/metasequoia_sql/common/
+-rw-rw-rw-   0        0        0      209 2024-04-15 00:51:46.000000 metasequoia-sql-0.4.0/metasequoia_sql/common/__init__.py
+-rw-rw-rw-   0        0        0     3937 2024-04-15 00:51:46.000000 metasequoia-sql-0.4.0/metasequoia_sql/common/base_scanner.py
+-rw-rw-rw-   0        0        0      601 2024-04-15 00:51:46.000000 metasequoia-sql-0.4.0/metasequoia_sql/common/basic.py
+-rw-rw-rw-   0        0        0      226 2024-04-15 00:51:46.000000 metasequoia-sql-0.4.0/metasequoia_sql/common/text_scanner.py
+-rw-rw-rw-   0        0        0     5617 2024-04-24 23:58:17.000000 metasequoia-sql-0.4.0/metasequoia_sql/common/token_scanner.py
+-rw-rw-rw-   0        0        0     5375 2024-04-24 00:26:00.000000 metasequoia-sql-0.4.0/metasequoia_sql/common/unsed_static.py
+drwxrwxrwx   0        0        0        0 2024-05-01 05:00:48.877427 metasequoia-sql-0.4.0/metasequoia_sql/core/
+-rw-rw-rw-   0        0        0      171 2024-04-25 00:28:03.000000 metasequoia-sql-0.4.0/metasequoia_sql/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 05:00:48.880347 metasequoia-sql-0.4.0/metasequoia_sql/core/node/
+-rw-rw-rw-   0        0        0      256 2024-04-26 00:25:39.000000 metasequoia-sql-0.4.0/metasequoia_sql/core/node/__init__.py
+-rw-rw-rw-   0        0        0      808 2024-04-26 00:25:39.000000 metasequoia-sql-0.4.0/metasequoia_sql/core/node/abc_node.py
+-rw-rw-rw-   0        0        0     6252 2024-04-26 00:31:00.000000 metasequoia-sql-0.4.0/metasequoia_sql/core/node/enum_node.py
+-rw-rw-rw-   0        0        0    63163 2024-04-26 23:40:20.000000 metasequoia-sql-0.4.0/metasequoia_sql/core/node/objects.py
+-rw-rw-rw-   0        0        0      295 2024-04-25 00:42:57.000000 metasequoia-sql-0.4.0/metasequoia_sql/core/node/sql_type.py
+-rw-rw-rw-   0        0        0    75899 2024-04-26 00:42:26.000000 metasequoia-sql-0.4.0/metasequoia_sql/core/parser.py
+-rw-rw-rw-   0        0        0      627 2024-04-18 23:18:49.000000 metasequoia-sql-0.4.0/metasequoia_sql/core/static.py
+-rw-rw-rw-   0        0        0      689 2024-04-25 00:02:19.000000 metasequoia-sql-0.4.0/metasequoia_sql/errors.py
+drwxrwxrwx   0        0        0        0 2024-05-01 05:00:48.881320 metasequoia-sql-0.4.0/metasequoia_sql/lexical/
+-rw-rw-rw-   0        0        0      144 2024-04-24 00:21:46.000000 metasequoia-sql-0.4.0/metasequoia_sql/lexical/__init__.py
+-rw-rw-rw-   0        0        0     8984 2024-04-26 00:27:19.000000 metasequoia-sql-0.4.0/metasequoia_sql/lexical/nodes.py
+-rw-rw-rw-   0        0        0    15442 2024-05-01 03:41:47.000000 metasequoia-sql-0.4.0/metasequoia_sql/lexical/parser.py
+-rw-rw-rw-   0        0        0      334 2024-04-26 00:27:42.000000 metasequoia-sql-0.4.0/metasequoia_sql/lexical/static.py
+drwxrwxrwx   0        0        0        0 2024-05-01 05:00:48.882294 metasequoia-sql-0.4.0/metasequoia_sql/plugins/
+-rw-rw-rw-   0        0        0        0 2024-04-18 23:18:49.000000 metasequoia-sql-0.4.0/metasequoia_sql/plugins/__init__.py
+-rw-rw-rw-   0        0        0     5734 2024-04-26 00:25:39.000000 metasequoia-sql-0.4.0/metasequoia_sql/plugins/mybaitis.py
+-rw-rw-rw-   0        0        0     1095 2024-04-24 00:26:38.000000 metasequoia-sql-0.4.0/metasequoia_sql/static.py
+drwxrwxrwx   0        0        0        0 2024-05-01 05:00:48.883267 metasequoia-sql-0.4.0/metasequoia_sql.egg-info/
+-rw-rw-rw-   0        0        0     8033 2024-05-01 05:00:48.000000 metasequoia-sql-0.4.0/metasequoia_sql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1820 2024-05-01 05:00:48.000000 metasequoia-sql-0.4.0/metasequoia_sql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 05:00:48.000000 metasequoia-sql-0.4.0/metasequoia_sql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-01 05:00:48.000000 metasequoia-sql-0.4.0/metasequoia_sql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 05:00:48.883267 metasequoia-sql-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1153 2024-05-01 04:59:57.000000 metasequoia-sql-0.4.0/setup.py
```

### Comparing `metasequoia-sql-0.3.0/LICENSE` & `metasequoia-sql-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metasequoia-sql-0.3.0/PKG-INFO` & `metasequoia-sql-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: metasequoia-sql
-Version: 0.3.0
-Summary: SQL解析器：提供词法解析、句法解析和不同SQL类型翻译的功能
+Version: 0.4.0
+Summary: SQL解析器：提供词法解析、句法解析以及配套的分析器、插件功能
 Home-page: https://github.com/ChangxingJiang/metasequoia-sql
 Author: changxing
 Author-email: 1278729001@qq.com
 License: MIT License
 Platform: all
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sql-tree：SQL 解析器
 
 ## 安装方法
@@ -24,19 +26,19 @@
 pip install metasequoia-sql
 ```
 
 ## 使用方法
 
 ### 词法分析
 
-对 SQL 语句进行句法分析，将 SQL 语句中的每个部分拆分为一个抽象语法树节点：
+对 SQL 语句进行句法分析，将 SQL 语句中的每个部分拆分为一个抽象词法树节点（abstract morphology tree，AMT）。
 
 ### 句法分析
 
-对 SQL 语句进行语法分析，将 SQL 语句转化为对应可操作的对象（详见 demo_2）：
+对 SQL 语句进行语法分析，将 SQL 语句转化为对应可操作的抽象语法树节点（abstract syntax tree，AST）：
 
 ```python
 from metasequoia_sql import *
 
 statement = SQLParser.parse_create_table_statement("your sql")
 ```
 
@@ -60,43 +62,43 @@
 
 **SQL 解析原理**：将词法分析与句法分析分离，对所有 SQL 语句进行词法分析，然后对不同的 SQL 语句类型使用不同的句法分析方法。
 
 **不同 DataSource 的 SQL 语句转换方法**： 先从特定 DataSource 的 SQL 转化为包含所有数据库特性的 FullStatement，然后再从
 FullStatement 转化为另一个 DataSource 的 SQl。通过这样的处理，可以避免开发网状结构的转换器，而只需要开发星星转换器即可。
 
 - `analyzer`：分析器
-- `ast`：词法分析（主要使用有限状态自动机实现）
+- `lexical`：词法分析
 - `common`：遍历器工具
 - `core`：句法分析节点类
-  - `abc`：抽象类（节点中不包含解析方法）
-  - `element`：元素类节点（不会引用其他节点）
-  - `general_expression`：一般表达式节点（可能引用元素类节点和其他一般表达式节点）
+    - `abc`：抽象类（节点中不包含解析方法）
+    - `element`：元素类节点（不会引用其他节点）
+    - `general_expression`：一般表达式节点（可能引用元素类节点和其他一般表达式节点）
 - `objects`：SQL语句对象
 - `parser`：SQL语句解析器
 
 （因为在 Python 中若标记类型时，不同文件之间不同循环引用，所以需要保证所有类的引用之间为严格的拓扑关系）
 
 ### 词法分析
 
 字面值类型：[参考文档](https://deepinout.com/mysql/mysql-top-articles-mysql/1694052463_j_mysql-literals.html)
 
-- `ASTLiteralString`：字符串字面值
+- `AMTLiteralString`：字符串字面值
 
 ### 句法分析
 
 #### 节点层级
 
 单项式级别（`SQLMonomial`）：在当前层级，仅包含一个元素或两个相互依存的元素，其中不允许包含任何计算符。但是需要注意的是，函数调用虽然是单项式级别，但它可能包含一个或多个多项式级别的子节点。
 
 - `SQLFunction`：函数调用。包含参数插入语。
 - `SQLColumnType`：DDL 中的字段类型，是 `SQLFunction` 的子类。可以是类型名称或函数调用（类型的注释）。因为在其他场景下，类型名称均不允许单独使用，所以在这里额外处理。
 - `SQLVariable`：变量引用。不包含插入语。例如 `CURRENT_DATE` 等。
 - `SQLLiteral`：字面值。没有依赖的列名。
 - 计算运算符
-  - `SQLPlus`：
+    - `SQLPlus`：
 - `SQLCompareOperator`：比较运算符。
 
 - `SQLColumnName`：列名。
 - `SQLTableName`：表名。
 
 多项式级别（`SQLPolynomial`）：
 
@@ -133,14 +135,35 @@
 
 - DB2 的 `CURRENT DATE` 的语法
 
 参考文档：https://www.alibabacloud.com/help/zh/maxcompute/user-guide/insert-or-update-data-into-a-table-or-a-static-partition?spm=a2c63.p38356.0.0.637d7109wr3nC3
 
 ## 修改记录
 
+#### 0.3.0 > 0.4.0
+
+新增：
+
+- 分析器框架 & 基本分析器 & 数据血缘分析器
+- 插件框架 & MyBatis 插件
+
+优化：
+
+- 优化词法分析节点，调整模块名，调整文件结构，将节点改为不可变
+- 统一标识符引号的相关逻辑
+- 兼容建表语句的索引包含 `COMMENT`、`KEY_BLOCK_SIZE` 的逻辑
+- 兼容建表语句的外键中包含 `ON DELETE CASCADE` 的逻辑
+- 兼容 Hive 建表语句
+
+修复：
+
+- 无法解析 MySQL 建表语句索引使用 USING 子句的 Bug
+- 在 `INSERT INTO` 语句中未指定列报错的 Bug
+- 各种原因导致解析后的 SQL 与原始 SQL 不一致的 Bug
+
 #### 0.2.0 > 0.3.0
 
 新增：
 
 - 重构词法解析和语法解析以支持插件开发
 - SET 语句的解析逻辑
 - LATERAL VIEW 子句的解析逻辑
@@ -156,23 +179,26 @@
 - 支持 DB2 的 CURRENT DATE、CURRENT TIME、CURRENT TIMESTAMP 语法
 - 增加 TokenScanner 未解析完成的发现机制
 - 支持窗口函数的 ROWS 子句
 
 #### 0.1.0 > 0.2.0
 
 新增：
+
 - `INSERT` 语句解析逻辑
 - 一次性解析多条 SQL 语句
 
 优化：
+
 - 统一 `CREATE TABLE` 解析逻辑（使用 `TokenScanner`，改造节点对象，改造解析逻辑，改造 Hive 源码生成逻辑）
 - 整理 objects 的节点和 parse 中的方法，清理多余对象，优化引用路径
 - 统一 TokenScanner 使用方法
 
 修复：
+
 - `WITH` 语句解析报错的 Bug 修复
 - Hive 建表语句的类型包含参数的 Bug 修复
 
 ##### 0.1.0
 
 - 新增 SELECT 语句解析逻辑
 - Bug 修复：移除在 Hive 建表语句末尾的分号
```

### Comparing `metasequoia-sql-0.3.0/README.md` & `metasequoia-sql-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 pip install metasequoia-sql
 ```
 
 ## 使用方法
 
 ### 词法分析
 
-对 SQL 语句进行句法分析，将 SQL 语句中的每个部分拆分为一个抽象语法树节点：
+对 SQL 语句进行句法分析，将 SQL 语句中的每个部分拆分为一个抽象词法树节点（abstract morphology tree，AMT）。
 
 ### 句法分析
 
-对 SQL 语句进行语法分析，将 SQL 语句转化为对应可操作的对象（详见 demo_2）：
+对 SQL 语句进行语法分析，将 SQL 语句转化为对应可操作的抽象语法树节点（abstract syntax tree，AST）：
 
 ```python
 from metasequoia_sql import *
 
 statement = SQLParser.parse_create_table_statement("your sql")
 ```
 
@@ -42,43 +42,43 @@
 
 **SQL 解析原理**：将词法分析与句法分析分离，对所有 SQL 语句进行词法分析，然后对不同的 SQL 语句类型使用不同的句法分析方法。
 
 **不同 DataSource 的 SQL 语句转换方法**： 先从特定 DataSource 的 SQL 转化为包含所有数据库特性的 FullStatement，然后再从
 FullStatement 转化为另一个 DataSource 的 SQl。通过这样的处理，可以避免开发网状结构的转换器，而只需要开发星星转换器即可。
 
 - `analyzer`：分析器
-- `ast`：词法分析（主要使用有限状态自动机实现）
+- `lexical`：词法分析
 - `common`：遍历器工具
 - `core`：句法分析节点类
-  - `abc`：抽象类（节点中不包含解析方法）
-  - `element`：元素类节点（不会引用其他节点）
-  - `general_expression`：一般表达式节点（可能引用元素类节点和其他一般表达式节点）
+    - `abc`：抽象类（节点中不包含解析方法）
+    - `element`：元素类节点（不会引用其他节点）
+    - `general_expression`：一般表达式节点（可能引用元素类节点和其他一般表达式节点）
 - `objects`：SQL语句对象
 - `parser`：SQL语句解析器
 
 （因为在 Python 中若标记类型时，不同文件之间不同循环引用，所以需要保证所有类的引用之间为严格的拓扑关系）
 
 ### 词法分析
 
 字面值类型：[参考文档](https://deepinout.com/mysql/mysql-top-articles-mysql/1694052463_j_mysql-literals.html)
 
-- `ASTLiteralString`：字符串字面值
+- `AMTLiteralString`：字符串字面值
 
 ### 句法分析
 
 #### 节点层级
 
 单项式级别（`SQLMonomial`）：在当前层级，仅包含一个元素或两个相互依存的元素，其中不允许包含任何计算符。但是需要注意的是，函数调用虽然是单项式级别，但它可能包含一个或多个多项式级别的子节点。
 
 - `SQLFunction`：函数调用。包含参数插入语。
 - `SQLColumnType`：DDL 中的字段类型，是 `SQLFunction` 的子类。可以是类型名称或函数调用（类型的注释）。因为在其他场景下，类型名称均不允许单独使用，所以在这里额外处理。
 - `SQLVariable`：变量引用。不包含插入语。例如 `CURRENT_DATE` 等。
 - `SQLLiteral`：字面值。没有依赖的列名。
 - 计算运算符
-  - `SQLPlus`：
+    - `SQLPlus`：
 - `SQLCompareOperator`：比较运算符。
 
 - `SQLColumnName`：列名。
 - `SQLTableName`：表名。
 
 多项式级别（`SQLPolynomial`）：
 
@@ -115,14 +115,35 @@
 
 - DB2 的 `CURRENT DATE` 的语法
 
 参考文档：https://www.alibabacloud.com/help/zh/maxcompute/user-guide/insert-or-update-data-into-a-table-or-a-static-partition?spm=a2c63.p38356.0.0.637d7109wr3nC3
 
 ## 修改记录
 
+#### 0.3.0 > 0.4.0
+
+新增：
+
+- 分析器框架 & 基本分析器 & 数据血缘分析器
+- 插件框架 & MyBatis 插件
+
+优化：
+
+- 优化词法分析节点，调整模块名，调整文件结构，将节点改为不可变
+- 统一标识符引号的相关逻辑
+- 兼容建表语句的索引包含 `COMMENT`、`KEY_BLOCK_SIZE` 的逻辑
+- 兼容建表语句的外键中包含 `ON DELETE CASCADE` 的逻辑
+- 兼容 Hive 建表语句
+
+修复：
+
+- 无法解析 MySQL 建表语句索引使用 USING 子句的 Bug
+- 在 `INSERT INTO` 语句中未指定列报错的 Bug
+- 各种原因导致解析后的 SQL 与原始 SQL 不一致的 Bug
+
 #### 0.2.0 > 0.3.0
 
 新增：
 
 - 重构词法解析和语法解析以支持插件开发
 - SET 语句的解析逻辑
 - LATERAL VIEW 子句的解析逻辑
@@ -138,23 +159,26 @@
 - 支持 DB2 的 CURRENT DATE、CURRENT TIME、CURRENT TIMESTAMP 语法
 - 增加 TokenScanner 未解析完成的发现机制
 - 支持窗口函数的 ROWS 子句
 
 #### 0.1.0 > 0.2.0
 
 新增：
+
 - `INSERT` 语句解析逻辑
 - 一次性解析多条 SQL 语句
 
 优化：
+
 - 统一 `CREATE TABLE` 解析逻辑（使用 `TokenScanner`，改造节点对象，改造解析逻辑，改造 Hive 源码生成逻辑）
 - 整理 objects 的节点和 parse 中的方法，清理多余对象，优化引用路径
 - 统一 TokenScanner 使用方法
 
 修复：
+
 - `WITH` 语句解析报错的 Bug 修复
 - Hive 建表语句的类型包含参数的 Bug 修复
 
 ##### 0.1.0
 
 - 新增 SELECT 语句解析逻辑
 - Bug 修复：移除在 Hive 建表语句末尾的分号
```

### Comparing `metasequoia-sql-0.3.0/metasequoia_sql/analyzer/data_lineage.py` & `metasequoia-sql-0.4.0/metasequoia_sql/analyzer/toolkit/current_level_sub_query.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 """
-数据血缘分析器
+表名规范化器
 """
 
-from typing import List
+from typing import Dict, List
 
-from metasequoia_sql.core import DataSource, SQLParser, SQLInsertStatement
+from metasequoia_sql import core
+from metasequoia_sql.analyzer.base import AnalyzerRecursionASTToDictBase
 
+__all__ = ["CurrentLevelSubQuery"]
 
-class DataLineageAnalyzer:
-    """
-    数据血缘分析器
-    """
-
-    def __init__(self, sql: str, data_source: DataSource):
-        # 过滤所有的 INSERT 语句
-        self.statements: List[SQLInsertStatement] = [
-            statement for statement in SQLParser.parse_statements(sql)
-            if isinstance(statement, SQLInsertStatement)]
-
-        # 统计所有 INSERT 语句中涉及的表名
-        self.used_table_set = set()
-        for statement in self.statements:
-            self.used_table_set.add(statement.table_name.source(data_source))
-            self.used_table_set |= set(statement.get_used_table_list())
-
-        # 定义建表语句的清单
-        self.create_table_statements = {}
-
-    def get_table_list(self) -> List[str]:
-        """获取上下游表的列表"""
-        return list(self.used_table_set)
+
+class CurrentLevelSubQuery(AnalyzerRecursionASTToDictBase):
+    """获取当前层的所有子查询的列表"""
+
+    def __init__(self, select_statement: core.ASTSelectStatement):
+        self._alias_hash = self.handle(select_statement)
+
+    def get_all_sub_query_alias_name(self) -> List[str]:
+        """获取所有子查询的别名列表"""
+        return list(self._alias_hash)
+
+    def get_sub_query_statement(self, alias_name: str) -> core.ASTSelectStatement:
+        """获取指定别名的子查询的 SELECT 语句"""
+        return self._alias_hash[alias_name]
+
+    @classmethod
+    def handle(cls, node: object) -> Dict[str, core.ASTSelectStatement]:
+        """TODO 待支持不包含别名的子查询"""
+        if (isinstance(node, core.ASTTableExpression)
+                and node.alias is not None and isinstance(node.table, core.ASTSubQueryExpression)):
+            return {node.alias.name: node.table.select_statement}
+        if isinstance(node, core.ASTSubQueryExpression) or isinstance(node, core.ASTWithClause):
+            return {}
+        return cls.default_handle_node(node)
```

### Comparing `metasequoia-sql-0.3.0/metasequoia_sql/ast/nodes.py` & `metasequoia-sql-0.4.0/metasequoia_sql/lexical/nodes.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,171 +1,174 @@
 """
-抽象语法树（AST）的节点类
+抽象词法树（AMT）的节点类
 
-所有抽象语法树的节点类均继承自抽象基类 AST 类，除 AST 类外，其他节点可以分为如下三种类型：
+所有抽象词法树的节点类均继承自抽象基类 AMT 类，除 AMT 类外，其他节点可以分为如下三种类型：
 - 定值叶节点：不包含子节点，且 source 返回定值的对象
 - 非定值叶节点：不包含子节点，但 source 返回值不固定的对象
 - 中间节点（插入语节点）：包含子节点的节点
+
+TODO 优化字面值的处理规则
 """
 
 import abc
 import enum
 from typing import List, Optional, Any, Set, Union
 
-from metasequoia_sql.ast.static import HEXADECIMAL_CHARACTER_SET, BINARY_CHARACTER_SET
-from metasequoia_sql.errors import AstParseError
+from metasequoia_sql.errors import AMTParseError
+from metasequoia_sql.lexical.static import HEXADECIMAL_CHARACTER_SET, BINARY_CHARACTER_SET
 
 __all__ = [
-    "AST", "ASTMark", "ASTSingle", "ASTParenthesis", "ASTLiteralInteger", "ASTLiteralFloat", "ASTLiteralString",
-    "ASTLiteralHex", "ASTLiteralBool", "ASTLiteralBit", "ASTLiteralNull"
+    "AMTBase", "AMTMark", "AMTBaseSingle", "AMTBaseParenthesis", "AMTLiteralInteger", "AMTLiteralFloat",
+    "AMTLiteralString", "AMTLiteralHex", "AMTLiteralBool", "AMTLiteralBit", "AMTLiteralNull"
 ]
 
 
-class ASTMark(enum.Enum):
+class AMTMark(enum.Enum):
     """抽象语法树节点标记"""
     SPACE = "<space>"
     NAME = "<name>"
     PARENTHESIS = "<parenthesis>"
     LITERAL = "<literal>"
     COMMENT = "<comment>"
     ARRAY_INDEX = "<array_index>"
+    CUSTOM = "<custom>"  # 自定义标记（用于插件开发）
 
 
 # 抽象语法树节点标记映射
-MARK_HASH = {mark.value: mark for mark in ASTMark}
+MARK_HASH = {mark.value: mark for mark in AMTMark}
 
 
 # ------------------------------ 抽象节点类 ------------------------------
 
 
-class AST(abc.ABC):
-    """抽象语法树（AST）节点类的抽象基类"""
+class AMTBase(abc.ABC):
+    """抽象词法树（AMT）节点类的抽象基类"""
 
-    def __init__(self, marks: Optional[Set[ASTMark]] = None):
-        self.marks: Set[ASTMark] = marks if marks is not None else set()
+    def __init__(self, marks: Optional[Set[AMTMark]] = None):
+        self.marks: Set[AMTMark] = marks if marks is not None else set()
 
     @property
     @abc.abstractmethod
     def source(self) -> str:
         """返回当前节点的源代码"""
 
     @abc.abstractmethod
-    def children(self) -> List["AST"]:
+    def children(self) -> List["AMTBase"]:
         """返回所有下游节点，若为叶子节点，则返回空列表"""
         return []
 
-    def equals(self, other: Union[str, ASTMark]) -> bool:
-        """判断当前 AST 节点是否与一段源代码相同"""
-        if isinstance(other, ASTMark):
+    def equals(self, other: Union[str, AMTMark]) -> bool:
+        """判断当前 AMT 节点是否与一段源代码相同"""
+        if isinstance(other, AMTMark):
             return other in self.marks  # 枚举类的类型标记
         if other.startswith("<") and other.endswith(">"):
             return MARK_HASH.get(other) in self.marks  # 字符串格式的类型标记
         return self.source.upper() == other.upper()  # 字符串格式文本
 
     @property
     def literal_value(self) -> Any:
         """字面值的值"""
         return None
 
 
-class ASTSingle(AST):
+class AMTBaseSingle(AMTBase):
     """单元素节点"""
 
-    def __init__(self, source: str, marks: Optional[Set[ASTMark]] = None):
+    def __init__(self, source: str, marks: Optional[Set[AMTMark]] = None):
         super().__init__(marks)
         self._source = source
 
     @property
     def source(self) -> str:
         """当前节点的源代码"""
         return self._source
 
-    def children(self) -> List["AST"]:
+    def children(self) -> List["AMTBase"]:
         """返回所有下游节点，若为叶子节点，则返回空列表"""
         return []
 
     def __repr__(self) -> str:
         format_source = self.source.replace("\n", r"\n")
         return f"<{self.__class__.__name__} source={format_source}>"
 
 
-class ASTParenthesis(AST):
+class AMTBaseParenthesis(AMTBase):
     """插入语节点"""
 
-    def __init__(self, tokens: List[AST], marks: Optional[Set[ASTMark]] = None):
+    def __init__(self, tokens: List[AMTBase], marks: Optional[Set[AMTMark]] = None):
         super().__init__(marks)
-        self._tokens: List[AST] = tokens
+        self._tokens: List[AMTBase] = tokens
 
-    def children(self) -> List["AST"]:
+    def children(self) -> List["AMTBase"]:
         return self._tokens
 
     @property
     def source(self):
         return "(" + "".join(token.source for token in self._tokens) + ")"
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__} children={self.children()}>"
 
 
-class ASTLiteralInteger(ASTSingle):
+class AMTLiteralInteger(AMTBaseSingle):
     """字面值整数"""
 
-    def __init__(self, source: str, marks: Optional[Set[ASTMark]] = None):
+    def __init__(self, source: str, marks: Optional[Set[AMTMark]] = None):
         super().__init__(source, marks)
         self._value = int(source)
 
     @property
     def literal_value(self) -> int:
         return self._value
 
     @property
     def source(self) -> str:
         return f"{self._value}"
 
 
-class ASTLiteralFloat(ASTSingle):
+class AMTLiteralFloat(AMTBaseSingle):
     """字面值浮点数"""
 
-    def __init__(self, source: str, marks: Optional[Set[ASTMark]] = None):
+    def __init__(self, source: str, marks: Optional[Set[AMTMark]] = None):
         super().__init__(source, marks)
         self._value = float(source)
 
     @property
     def literal_value(self) -> float:
         return self._value
 
     @property
     def source(self) -> str:
         return f"{self._value}"
 
 
-class ASTLiteralString(ASTSingle):
+class AMTLiteralString(AMTBaseSingle):
     """字面值字符串"""
 
-    def __init__(self, source: str, marks: Optional[Set[ASTMark]] = None):
+    def __init__(self, source: str, marks: Optional[Set[AMTMark]] = None):
         super().__init__(source, marks)
         self._value = source[1:-1]  # 不包含引号的部分
 
     @property
     def literal_value(self) -> str:
         return self._value
 
     @property
     def source(self) -> str:
         return f"'{self._value}'"
 
 
-class ASTLiteralHex(ASTSingle):
+class AMTLiteralHex(AMTBaseSingle):
     """十六进制字面值"""
 
-    def __init__(self, source: str, marks: Optional[Set[ASTMark]] = None):
+    def __init__(self, source: str, marks: Optional[Set[AMTMark]] = None):
         super().__init__(source, marks)
         self._value = self._get_value(source)  # 获取十六进制字面值中的十六进制数值，如果格式不满足则返回 None
         if self._value is None:
-            raise AstParseError(f"十六进制数不满足字符集要求: {source}")
+            raise AMTParseError(f"十六进制数不满足字符集要求: {source}")
 
     @classmethod
     def check(cls, origin: str):
         """判断是否为当前节点"""
         return cls._get_value(origin) is not None
 
     @staticmethod
@@ -193,18 +196,18 @@
         return self._value
 
     @property
     def source(self) -> str:
         return f"x'{self._value}'"
 
 
-class ASTLiteralBool(ASTSingle):
+class AMTLiteralBool(AMTBaseSingle):
     """布尔字面值"""
 
-    def __init__(self, source: str, marks: Optional[Set[ASTMark]] = None):
+    def __init__(self, source: str, marks: Optional[Set[AMTMark]] = None):
         super().__init__(source, marks)
         self._value: bool = source.upper() == "TRUE"
 
     @classmethod
     def check(cls, origin: str) -> bool:
         """判断是否为当前节点"""
         return origin.upper() in {"TRUE", "FALSE"}
@@ -214,22 +217,22 @@
         return self._value
 
     @property
     def source(self) -> str:
         return "TRUE" if self._value is True else "FALSE"
 
 
-class ASTLiteralBit(ASTSingle):
+class AMTLiteralBit(AMTBaseSingle):
     """位值字面值"""
 
-    def __init__(self, source: str, marks: Optional[Set[ASTMark]] = None):
+    def __init__(self, source: str, marks: Optional[Set[AMTMark]] = None):
         super().__init__(source, marks)
         self._value = self._get_value(source)  # 获取二进制字面值中的二进制数值，如果格式不满足则返回 None
         if self._value is None:
-            raise AstParseError(f"不满足格式要求的二进制字面值: origin={source}")
+            raise AMTParseError(f"不满足格式要求的二进制字面值: origin={source}")
 
     @classmethod
     def check(cls, origin: str):
         """判断是否为当前节点"""
         return cls._get_value(origin) is not None
 
     @staticmethod
@@ -257,15 +260,15 @@
         return self._value
 
     @property
     def source(self) -> str:
         return f"b'{self._value}'"
 
 
-class ASTLiteralNull(ASTSingle):
+class AMTLiteralNull(AMTBaseSingle):
     """空值字面值"""
 
     @classmethod
     def check(cls, origin: str):
         """判断是否为当前节点"""
         return origin.upper() == "NULL"
```

### Comparing `metasequoia-sql-0.3.0/metasequoia_sql/ast/parser.py` & `metasequoia-sql-0.4.0/metasequoia_sql/lexical/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """
-ast 的解析方法
+抽象词法树（AMT）的解析方法
 """
 
 import enum
 import re
 from typing import List, Union
 
-from metasequoia_sql.ast.nodes import (AST, ASTMark, ASTSingle, ASTLiteralInteger, ASTLiteralFloat, ASTLiteralString,
-                                       ASTLiteralHex, ASTLiteralBool, ASTLiteralBit, ASTLiteralNull, ASTParenthesis)
 from metasequoia_sql.common.text_scanner import TextScanner
-from metasequoia_sql.errors import AstParseError
+from metasequoia_sql.errors import AMTParseError
+from metasequoia_sql.lexical.nodes import (AMTBase, AMTMark, AMTBaseSingle, AMTLiteralInteger, AMTLiteralFloat,
+                                           AMTLiteralString,
+                                           AMTLiteralHex, AMTLiteralBool, AMTLiteralBit, AMTLiteralNull,
+                                           AMTBaseParenthesis)
 
 
 class AstParseStatus(enum.Enum):
     """SQL 源码的解析状态"""
     WAIT_TOKEN = enum.auto()  # 前一个字符是开头、空白字符或上一个 token 的结尾，正等待新的 token
     IN_WORD = enum.auto()  # 当前正在正常词语中
     IN_DOUBLE_QUOTE = enum.auto()  # 当前正在双引号 " 中
@@ -24,38 +26,38 @@
 
 
 class ASTParser:
     """抽象语法树解析器
 
     Attributes
     ----------
-    _stack : List[List[AST]]
+    _stack : List[List[AMTBase]]
         当前已解析的节点树。使用多层栈维护，每一层栈表示一层插入语。
     _scanner : TextScanner
         源代码遍历器
     _status : AstParseStatus
         状态机状态
     _cache : List[str]
         当前正在缓存的词语
     """
 
     def __init__(self, text: str):
-        self._stack: List[List[AST]] = [[]]
+        self._stack: List[List[AMTBase]] = [[]]
         self._scanner: TextScanner = TextScanner(self._preproc_text(text))
         self._status: Union[AstParseStatus, object] = AstParseStatus.WAIT_TOKEN
         self._cache: List[str] = []
 
     @staticmethod
     def _preproc_text(text):
         return text.replace("\r\n", "\n").replace("\t", " ").replace("　", " ")
 
     # ------------------------------ 上下文管理器属性 ------------------------------
 
     @property
-    def stack(self) -> List[List[AST]]:
+    def stack(self) -> List[List[AMTBase]]:
         """获取当前自动机词语栈"""
         return self._stack
 
     @property
     def scanner(self) -> TextScanner:
         """获取当前的文本扫描器"""
         return self._scanner
@@ -96,72 +98,73 @@
         """【移动指针】处理当前指针位置的左括号"""
         self.scanner.pop()
         self.stack.append([])
 
     def end_parenthesis(self) -> None:
         """【移动指针】处理当前指针位置的右括号"""
         if len(self.stack) <= 1:
-            raise AstParseError(f"当前 ')' 数量大于 '(': pos={self.scanner.pos}")
+            raise AMTParseError(f"当前 ')' 数量大于 '(': pos={self.scanner.pos}")
 
         self.scanner.pop()
         tokens = self.stack.pop()
-        self.stack[-1].append(ASTParenthesis(tokens, {ASTMark.PARENTHESIS}))
+        self.stack[-1].append(AMTBaseParenthesis(tokens, {AMTMark.PARENTHESIS}))
 
     def handle_end_word(self) -> None:
         """【不移动指针】处理在当前指针位置的前一个字符结束的缓存词语（即当前指针位置是下一个词语的第一个字符）
 
         1. 获取并重置缓存词语
         2. 解析缓存词语并更新到节点树中
         3. 将状态更新为等待下一个节点
         """
         origin = self.cache_get_and_reset()
         # 空格、换行符
         if origin in {" ", "\n"}:
-            self.stack[-1].append(ASTSingle(origin, {ASTMark.SPACE}))
+            self.stack[-1].append(AMTBaseSingle(origin, {AMTMark.SPACE}))
         # 逗号、分号、点号、等号、计算运算符（含通配符）、比较运算符、子句核心关键词、逻辑运算符
-        elif origin in {",", ";", ".", "=", "+", "-", "/", "%", "||", "<>", "!=", "<", "<=", ">", ">=",
-                        "SELECT", "FROM", "LATERAL", "VIEW", "JOIN", "ON", "WHERE", "GROUP", "BY", "HAVING",
-                        "ORDER", "LIMIT", "UNION", "EXCEPT", "MINUS", "INTERSECT",
-                        "AND", "NOT", "OR"}:
-            self.stack[-1].append(ASTSingle(origin))
+        elif origin.upper() in {",", ";", ".", "=", "+", "-", "/", "%", "||", "<>", "!=", "<", "<=", ">", ">=",
+                                "SELECT", "FROM", "LATERAL", "VIEW", "LEFT", "RIGHT", "INNER", "OUTER", "FULL", "JOIN",
+                                "ON", "WHERE", "GROUP", "BY", "HAVING",
+                                "ORDER", "LIMIT", "UNION", "EXCEPT", "MINUS", "INTERSECT",
+                                "AND", "NOT", "OR"}:
+            self.stack[-1].append(AMTBaseSingle(origin))
         # 下标
         elif origin.startswith("[") and origin.endswith("]"):
-            self.stack[-1].append(ASTSingle(origin, {ASTMark.ARRAY_INDEX}))
+            self.stack[-1].append(AMTBaseSingle(origin, {AMTMark.ARRAY_INDEX}))
         # 字面值整数
         elif re.match(r"^[+-]?\d+$", origin):
-            self.stack[-1].append(ASTLiteralInteger(origin, {ASTMark.LITERAL}))
+            self.stack[-1].append(AMTLiteralInteger(origin, {AMTMark.LITERAL}))
         # 字面值小数或浮点数
         elif re.match(r"^[+-]?\d+.\d+(E\d+)?$", origin):
-            self.stack[-1].append(ASTLiteralFloat(origin, {ASTMark.LITERAL}))
+            self.stack[-1].append(AMTLiteralFloat(origin, {AMTMark.LITERAL}))
         # 字面值字符串（包含字面值日期和时间）
         elif (origin.startswith("\"") and origin.endswith("\"")) or (origin.startswith("'") and origin.endswith("'")):
-            self.stack[-1].append(ASTLiteralString(origin, {ASTMark.LITERAL, ASTMark.NAME}))
+            self.stack[-1].append(AMTLiteralString(origin, {AMTMark.LITERAL, AMTMark.NAME}))
         # 十六进制字面值节点
-        elif ASTLiteralHex.check(origin) is True:
-            self.stack[-1].append(ASTLiteralHex(origin, {ASTMark.LITERAL}))
+        elif AMTLiteralHex.check(origin) is True:
+            self.stack[-1].append(AMTLiteralHex(origin, {AMTMark.LITERAL}))
         # 布尔字面值节点
-        elif ASTLiteralBool.check(origin) is True:
-            self.stack[-1].append(ASTLiteralBool(origin, {ASTMark.LITERAL}))
+        elif AMTLiteralBool.check(origin) is True:
+            self.stack[-1].append(AMTLiteralBool(origin, {AMTMark.LITERAL}))
         # 位值字面值节点
-        elif ASTLiteralBit.check(origin) is True:
-            self.stack[-1].append(ASTLiteralBit(origin, {ASTMark.LITERAL}))
+        elif AMTLiteralBit.check(origin) is True:
+            self.stack[-1].append(AMTLiteralBit(origin, {AMTMark.LITERAL}))
         # 空值字面值节点
-        elif ASTLiteralNull.check(origin) is True:
-            self.stack[-1].append(ASTLiteralNull(origin, {ASTMark.LITERAL}))
+        elif AMTLiteralNull.check(origin) is True:
+            self.stack[-1].append(AMTLiteralNull(origin, {AMTMark.LITERAL}))
         # 显式标识符
         elif origin.startswith("`") and origin.endswith("`"):
-            self.stack[-1].append(ASTSingle(origin, {ASTMark.NAME}))
+            self.stack[-1].append(AMTBaseSingle(origin, {AMTMark.NAME}))
         # 单行注释
         elif origin.startswith("#") or origin.startswith("--"):
-            self.stack[-1].append(ASTSingle(origin, {ASTMark.COMMENT}))
+            self.stack[-1].append(AMTBaseSingle(origin, {AMTMark.COMMENT}))
         # 多行注释
         elif origin.startswith("/*") and origin.endswith("*/"):
-            self.stack[-1].append(ASTSingle(origin, {ASTMark.COMMENT}))
+            self.stack[-1].append(AMTBaseSingle(origin, {AMTMark.COMMENT}))
         else:
-            self.stack[-1].append(ASTSingle(origin, {ASTMark.NAME}))
+            self.stack[-1].append(AMTBaseSingle(origin, {AMTMark.NAME}))
 
     def cache_add_and_handle_end_word(self) -> None:
         """【移动指针】先将当前指针位置的字符添加到缓存并移动指针位置，然后处理在刚缓存的字符结束的缓存词语（即调用时的指针位置为当前词语的最后一个字符）"""
         self.cache_add()
         self.handle_end_word()
 
     # ------------------------------ 私有处理方法 ------------------------------
@@ -176,15 +179,17 @@
         while not self.scanner.is_finish:
             self.handle_change()
 
         # 处理最后一个词语
         self.handle_last()
 
         if len(self.stack) > 1:
-            raise AstParseError("'(' 数量大于 ')'")
+            for item in self.stack:
+                print(item)
+            raise AMTParseError(f"在解析过程中，`(` 数量大于 `)`，相差数量 = {len(self.stack) - 1}")
 
     def handle_change(self):
         """处理一次的变化"""
         if self.status == AstParseStatus.WAIT_TOKEN:  # 前一个字符是空白字符
             if self.scanner.now == "/" and self.scanner.next1 == "*":
                 self.cache_reset_and_add()  # 【移动指针】重置当前缓存词语，并将当前指针位置字符添加到缓存
                 self.cache_add()
```

### Comparing `metasequoia-sql-0.3.0/metasequoia_sql/ast/static.py` & `metasequoia-sql-0.4.0/metasequoia_sql/common/unsed_static.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,11 @@
 """
-词法分析的静态常量
+在主逻辑中没有使用的静态常量
 """
 
-# 十六机制的字符集
-HEXADECIMAL_CHARACTER_SET = {"0", "1", "2", "3", "4", "5", "6", "7", "8", "9", "A", "a", "B", "b", "C", "c", "D", "d",
-                             "E", "e", "F", "f"}
-
-# 二级制的字符集
-BINARY_CHARACTER_SET = {"0", "1"}
-
 # MySQL 保留字
 MYSQL_KEYWORDS = {
     "ACTION", "ADD", "ALL", "ALTER", "ANALYZE", "AND", "AS", "ASC", "ASENSITIVE", "BEFORE", "BETWEEN", "BIGINT",
     "BINARY", "BIT", "BLOB", "BOTH", "BY", "CALL", "CASCADE", "CASE", "CHANGE", "CHAR", "CHARACTER", "CHECK", "COLLATE",
     "COLUMN", "CONDITION", "CONNECTION", "CONSTRAINT", "CONTINUE", "CONVERT", "CREATE", "CROSS", "CURRENT_DATE",
     "CURRENT_TIME", "CURRENT_TIMESTAMP", "CURRENT_USER", "CURSOR", "DATABASE", "DATABASES", "DATE", "DAY_HOUR",
     "DAY_MICROSECOND", "DAY_MINUTE", "DAY_SECOND", "DEC", "DECIMAL", "DECLARE", "DEFAULT", "DELAYED", "DELETE", "DESC",
```

### Comparing `metasequoia-sql-0.3.0/metasequoia_sql/common/base_scanner.py` & `metasequoia-sql-0.4.0/metasequoia_sql/common/base_scanner.py`

 * *Files identical despite different names*

### Comparing `metasequoia-sql-0.3.0/metasequoia_sql/common/basic.py` & `metasequoia-sql-0.4.0/metasequoia_sql/common/basic.py`

 * *Files identical despite different names*

### Comparing `metasequoia-sql-0.3.0/metasequoia_sql/common/token_scanner.py` & `metasequoia-sql-0.4.0/metasequoia_sql/common/token_scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
 抽象语法树扫描器
 """
 
 from typing import List, Union
 
-from metasequoia_sql.ast import AST, ASTParser, ASTMark
+from metasequoia_sql.lexical import AMTBase, AMTMark
 from metasequoia_sql.common.base_scanner import BaseScanner
 from metasequoia_sql.errors import ScannerError
 
 
 class TokenScanner(BaseScanner):
     """Token 扫描器"""
 
-    def __init__(self, elements: List[AST],
+    def __init__(self, elements: List[AMTBase],
                  pos: int = 0,
                  ignore_space: bool = False,
                  ignore_comment: bool = False):
         """
 
         Parameters
         ----------
@@ -24,52 +24,52 @@
             当前层级的抽象语法树节点列表
         pos : int, default = 0
             当前正在处理的抽象语法树节点下标
         """
         # 根据要求筛选输入元素
         filtered_elements = []
         for element in elements:
-            if element.equals(ASTMark.SPACE):
+            if element.equals(AMTMark.SPACE):
                 if ignore_space is False:  # 关闭忽略空白字符的模式
                     filtered_elements.append(element)
-            elif element.equals(ASTMark.COMMENT):
+            elif element.equals(AMTMark.COMMENT):
                 if ignore_comment is False:  # 关闭忽略注释的模式
                     filtered_elements.append(element)
             else:
                 filtered_elements.append(element)
 
         super().__init__(filtered_elements, pos)
 
-    def search(self, *tokens: Union[str, ASTMark]) -> bool:
+    def search(self, *tokens: Union[str, AMTMark]) -> bool:
         """从当前配置开始匹配 tokens
 
         - 如果匹配成功，则返回 True
         - 如果匹配失败，则返回 False
         """
         for idx, token in enumerate(tokens):
             refer = self._get_by_offset(idx)
             if refer is None or not refer.equals(token):
                 return False
         return True
 
-    def search_and_move(self, *tokens: Union[str, ASTMark]) -> bool:
+    def search_and_move(self, *tokens: Union[str, AMTMark]) -> bool:
         """从当前配置开始匹配 tokens
 
         - 如果匹配成功，则将指针移动到 tokens 后的下一个元素并返回 True
         - 如果匹配失败，则不移动指针并返回 False
         """
         for idx, token in enumerate(tokens):
             refer = self._get_by_offset(idx)
             if refer is None or not refer.equals(token):
                 return False
         for _ in range(len(tokens)):
             self.pop()
         return True
 
-    def match(self, *tokens: Union[str, ASTMark]) -> None:
+    def match(self, *tokens: Union[str, AMTMark]) -> None:
         """从当前配置开始匹配 tokens
 
         - 如果匹配成功，则将指针移动到 tokens 后的下一个元素
         - 如果匹配失败，则抛出异常
         """
         for word in tokens:
             if not self.pop().equals(word):
@@ -95,15 +95,15 @@
                  source: str,
                  ignore_space: bool = True,
                  ignore_comment: bool = True) -> List["TokenScanner"]:
         """【移动指针（到末尾）】将后续元素拆分为使用 source 分隔的扫描器列表"""
         result = []
         tokens = []
         while not self.is_finish:
-            token: AST = self.pop()
+            token: AMTBase = self.pop()
             if token.equals(source):
                 if len(tokens) > 0:
                     result.append(TokenScanner(tokens, ignore_space=ignore_space, ignore_comment=ignore_comment))
                     tokens = []
             else:
                 tokens.append(token)
         if len(tokens) > 0:
```

### Comparing `metasequoia-sql-0.3.0/metasequoia_sql/core/parser.py` & `metasequoia-sql-0.4.0/metasequoia_sql/core/parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 基础元素的解析逻辑
 
 因为不同解析函数之间需要相互调用，所以脚本文件不可避免地需要超过 1000 行，故忽略 pylint C0302。
 
 TODO 使用 search 替代直接使用 now 判断
 TODO 将 CAST_DATA_TYPE 提出作为一个基础类型节点
 TODO 将 function_name 提出作为一个专有表达式
+TODO 清理只调用一次的单行函数
+TODO 将 CURRENT_TIMESTAMP、CURRENT_DATE、CURRENT_TIME 改为单独节点处理
 """
 
 from typing import Optional, Tuple, List, Union
 
-from metasequoia_sql.ast import (AST, ASTMark, ASTSingle, ASTLiteralInteger, ASTLiteralFloat, ASTLiteralString,
-                                 ASTLiteralHex, ASTLiteralBool, ASTLiteralBit, ASTLiteralNull, ASTParser)
+from metasequoia_sql.lexical import (AMTBase, AMTMark, AMTBaseSingle, AMTLiteralInteger, AMTLiteralFloat, AMTLiteralString,
+                                     AMTLiteralHex, AMTLiteralBool, AMTLiteralBit, AMTLiteralNull, ASTParser)
 from metasequoia_sql.common import TokenScanner
-from metasequoia_sql.core.objects import *
+from metasequoia_sql.core.node import *
 from metasequoia_sql.core.static import AGGREGATION_FUNCTION_NAME_SET, WINDOW_FUNCTION_NAME_SET
 from metasequoia_sql.errors import SqlParseError
 
 __all__ = ["SQLParser"]
 
 
 class SQLParser:
@@ -47,274 +49,282 @@
             scanner_or_string = scanner_or_string.replace("CURRENT DATE", "CURRENT_DATE")
             scanner_or_string = scanner_or_string.replace("CURRENT TIME", "CURRENT_TIME")
             scanner_or_string = scanner_or_string.replace("CURRENT TIMESTAMP", "CURRENT_TIMESTAMP")
             return cls.build_token_scanner(scanner_or_string)
         raise SqlParseError(f"未知的参数类型: {scanner_or_string} (type={type(scanner_or_string)})")
 
     @classmethod
+    def _unify_name(cls, string: Optional[str]) -> Optional[str]:
+        """格式化名称标识符：统一剔除当前引号并添加引号"""
+        if string is not None:
+            return string.strip("`")
+        return None
+
+    @classmethod
     def check_insert_type(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
         """判断是否为插入类型"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         return scanner.search_and_move("INSERT", "INTO") or scanner.search_and_move("INSERT", "OVERWRITE")
 
     @classmethod
-    def parse_insert_type(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLInsertType:
+    def parse_insert_type(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTInsertType:
         """解析插入类型"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         if scanner.search_and_move("INSERT", "INTO"):
-            return SQLInsertType(insert_type=EnumInsertType.INSERT_INTO)
+            return ASTInsertType(enum=EnumInsertType.INSERT_INTO)
         if scanner.search_and_move("INSERT", "OVERWRITE"):
-            return SQLInsertType(insert_type=EnumInsertType.INSERT_OVERWRITE)
+            return ASTInsertType(enum=EnumInsertType.INSERT_OVERWRITE)
         raise SqlParseError(f"未知的 INSERT 类型: {scanner}")
 
     @classmethod
     def check_join_type(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
         """判断是否为关联类型"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         for join_type in EnumJoinType:
             if scanner.search(*join_type.value):
                 return True
         return False
 
     @classmethod
-    def parse_join_type(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLJoinType:
+    def parse_join_type(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTJoinType:
         """解析关联类型"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         for join_type in EnumJoinType:
             if scanner.search_and_move(*join_type.value):
-                return SQLJoinType(join_type=join_type)
+                return ASTJoinType(enum=join_type)
         raise SqlParseError(f"无法解析的关联类型: {scanner}")
 
     @classmethod
     def check_order_type(cls) -> bool:
         """判断是否为排序类型：任何元素都可以是排序类型（省略升序），所以均返回 True"""
         return True
 
     @classmethod
-    def parse_order_type(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLOrderType:
+    def parse_order_type(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTOrderType:
         """解析排序类型"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         if scanner.search_and_move("DESC"):
-            return SQLOrderType(order_type=EnumOrderType.DESC)
+            return ASTOrderType(enum=EnumOrderType.DESC)
         if scanner.search_and_move("ASC"):
-            return SQLOrderType(order_type=EnumOrderType.ASC)
-        return SQLOrderType(order_type=EnumOrderType.ASC)
+            return ASTOrderType(enum=EnumOrderType.ASC)
+        return ASTOrderType(enum=EnumOrderType.ASC)
 
     @classmethod
     def check_union_type(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
         """判断是否为组合类型"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         for union_type in EnumUnionType:
             if scanner.search(*union_type.value):
                 return True
         return False
 
     @classmethod
-    def parse_union_type(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLUnionType:
+    def parse_union_type(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTUnionType:
         """解析组合类型"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         for union_type in EnumUnionType:
             if scanner.search_and_move(*union_type.value):
-                return SQLUnionType(union_type=union_type)
+                return ASTUnionType(enum=union_type)
         raise SqlParseError(f"无法解析的组合类型: {scanner}")
 
     @classmethod
     def check_compare_operator(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
         """判断是否为比较运算符"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         return scanner.get_as_source() in {"=", "!=", "<>", "<", "<=", ">", ">="}
 
     @classmethod
-    def parse_compare_operator(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLCompareOperator:
+    def parse_compare_operator(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTCompareOperator:
         """解析比较运算符"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         compare_operator_hash = {
             "=": EnumCompareOperator.EQUAL_TO,
             "<": EnumCompareOperator.LESS_THAN,
             "<=": EnumCompareOperator.LESS_THAN_OR_EQUAL,
             ">": EnumCompareOperator.GREATER_THAN,
             ">=": EnumCompareOperator.GREATER_THAN_OR_EQUAL,
             "!=": EnumCompareOperator.NOT_EQUAL_TO,
             "<>": EnumCompareOperator.NOT_EQUAL_TO
         }
         compare_operator = compare_operator_hash.get(scanner.pop_as_source())
         if compare_operator is not None:
-            return SQLCompareOperator(compare_operator=compare_operator)
+            return ASTCompareOperator(enum=compare_operator)
         raise SqlParseError(f"无法解析的比较运算符: {scanner}")
 
     @classmethod
     def check_compute_operator(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
         """判断是否为计算运算符"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         for compute_operator in EnumComputeOperator:
             if scanner.search(compute_operator.value):
                 return True
         return False
 
     @classmethod
-    def parse_compute_operator(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLComputeOperator:
+    def parse_compute_operator(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTComputeOperator:
         """解析计算运算符"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         for compute_operator in EnumComputeOperator:
             if scanner.search_and_move(compute_operator.value):
-                return SQLComputeOperator(compute_operator=compute_operator)
+                return ASTComputeOperator(enum=compute_operator)
         raise SqlParseError(f"无法解析的计算运算符: {scanner}")
 
     @classmethod
     def check_logical_operator(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
         """判断是否为逻辑运算符"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         return scanner.get_as_source() in {"AND", "OR"}
 
     @classmethod
-    def parse_logical_operator(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLLogicalOperator:
+    def parse_logical_operator(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTLogicalOperator:
         """解析逻辑运算符"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         for logical_operator in EnumLogicalOperator:
             if scanner.search_and_move(logical_operator.value):
-                return SQLLogicalOperator(logical_operator=logical_operator)
+                return ASTLogicalOperator(enum=logical_operator)
         raise SqlParseError(f"无法解析的逻辑运算符: {scanner}")
 
     @classmethod
     def check_literal_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
         """判断是否为字面值：包含整型字面值、浮点型字面值、字符串型字面值、十六进制型字面值、布尔型字面值、位值型字面值、空值的字面值"""
         scanner = cls._unify_input_scanner(scanner_or_string)
-        return scanner.search(ASTMark.LITERAL) or scanner.search("-")
+        return scanner.search(AMTMark.LITERAL) or scanner.search("-")
 
     @classmethod
-    def parse_literal_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLLiteralExpression:
+    def parse_literal_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTLiteralExpression:
         """解析字面值：包含整型字面值、浮点型字面值、字符串型字面值、十六进制型字面值、布尔型字面值、位值型字面值、空值的字面值"""
         scanner = cls._unify_input_scanner(scanner_or_string)
-        token: AST = scanner.pop()
-        if isinstance(token, ASTLiteralInteger):
-            return SQLLiteralIntegerExpression(value=token.literal_value)
-        if isinstance(token, ASTLiteralFloat):
-            return SQLLiteralFloatExpression(value=token.literal_value)
-        if isinstance(token, ASTLiteralString):
-            return SQLLiteralStringExpression(value=token.literal_value)
-        if isinstance(token, ASTLiteralHex):
-            return SQLLiteralHexExpression(value=token.literal_value)
-        if isinstance(token, ASTLiteralBool):
-            return SQLLiteralBoolExpression(value=token.literal_value)
-        if isinstance(token, ASTLiteralBit):
-            return SQLLiteralBitExpression(value=token.literal_value)
-        if isinstance(token, ASTLiteralNull):
-            return SQLLiteralNullExpression()
-        if token.equals("-") and isinstance(scanner.now, ASTLiteralInteger):
+        token: AMTBase = scanner.pop()
+        if isinstance(token, AMTLiteralInteger):
+            return ASTLiteralIntegerExpression(value=token.literal_value)
+        if isinstance(token, AMTLiteralFloat):
+            return ASTLiteralFloatExpression(value=token.literal_value)
+        if isinstance(token, AMTLiteralString):
+            return ASTLiteralStringExpression(value=token.literal_value)
+        if isinstance(token, AMTLiteralHex):
+            return ASTLiteralHexExpression(value=token.literal_value)
+        if isinstance(token, AMTLiteralBool):
+            return ASTLiteralBoolExpression(value=token.literal_value)
+        if isinstance(token, AMTLiteralBit):
+            return ASTLiteralBitExpression(value=token.literal_value)
+        if isinstance(token, AMTLiteralNull):
+            return ASTLiteralNullExpression()
+        if token.equals("-") and isinstance(scanner.now, AMTLiteralInteger):
             next_token = scanner.pop()
-            return SQLLiteralIntegerExpression(value=-next_token.literal_value)
-        if token.equals("-") and isinstance(scanner.now, ASTLiteralFloat):
+            return ASTLiteralIntegerExpression(value=-next_token.literal_value)
+        if token.equals("-") and isinstance(scanner.now, AMTLiteralFloat):
             next_token = scanner.pop()
-            return SQLLiteralFloatExpression(value=-next_token.literal_value)
+            return ASTLiteralFloatExpression(value=-next_token.literal_value)
         raise SqlParseError(f"未知的字面值: {token}")
 
     @classmethod
     def check_column_name_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
         """是否可能为列名表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         return not scanner.is_finish and (
-                (scanner.now.equals(ASTMark.NAME) and
+                (scanner.now.equals(AMTMark.NAME) and
                  (scanner.next1 is None or (
-                         not scanner.next1.equals(".") and not scanner.next1.equals(ASTMark.PARENTHESIS)))) or
-                (scanner.now.equals(ASTMark.NAME) and
+                         not scanner.next1.equals(".") and not scanner.next1.equals(AMTMark.PARENTHESIS)))) or
+                (scanner.now.equals(AMTMark.NAME) and
                  scanner.next1 is not None and scanner.next1.equals(".") and
-                 scanner.next2 is not None and scanner.next2.equals(ASTMark.NAME) and
-                 (scanner.next3 is None or not scanner.next3.equals(ASTMark.PARENTHESIS)))
+                 scanner.next2 is not None and scanner.next2.equals(AMTMark.NAME) and
+                 (scanner.next3 is None or not scanner.next3.equals(AMTMark.PARENTHESIS)))
         )
 
     @classmethod
-    def parse_column_name_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLColumnNameExpression:
+    def parse_column_name_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTColumnNameExpression:
         """解析列名表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
-        if (scanner.search(ASTMark.NAME, ".", ASTMark.NAME) and
-                not scanner.search(ASTMark.NAME, ".", ASTMark.NAME, ASTMark.PARENTHESIS)):
+        if (scanner.search(AMTMark.NAME, ".", AMTMark.NAME) and
+                not scanner.search(AMTMark.NAME, ".", AMTMark.NAME, AMTMark.PARENTHESIS)):
             table_name = scanner.pop_as_source()
             scanner.pop()
             column_name = scanner.pop_as_source()
-            return SQLColumnNameExpression(table=table_name, column=column_name)
-        if scanner.search(ASTMark.NAME) and not scanner.search(ASTMark.NAME, ASTMark.PARENTHESIS):
-            return SQLColumnNameExpression(column=scanner.pop_as_source())
+            return ASTColumnNameExpression(table=cls._unify_name(table_name), column=cls._unify_name(column_name))
+        if scanner.search(AMTMark.NAME) and not scanner.search(AMTMark.NAME, AMTMark.PARENTHESIS):
+            return ASTColumnNameExpression(column=cls._unify_name(scanner.pop_as_source()))
         raise SqlParseError(f"无法解析为表名表达式: {scanner}")
 
     @classmethod
     def check_function_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
         """是否可能为函数表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
-        return (scanner.search(ASTMark.NAME, ASTMark.PARENTHESIS) or
-                scanner.search(ASTMark.NAME, ".", ASTMark.NAME, ASTMark.PARENTHESIS))
+        return (scanner.search(AMTMark.NAME, AMTMark.PARENTHESIS) or
+                scanner.search(AMTMark.NAME, ".", AMTMark.NAME, AMTMark.PARENTHESIS))
 
     @classmethod
     def parse_cast_data_type(cls, scanner_or_string: Union[TokenScanner, str]) -> EnumCastDataType:
         """解析 CAST 函数表达式中的类型"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         for cast_type in EnumCastDataType:
             if scanner.search_and_move(cast_type.value):
                 return cast_type
         raise SqlParseError(f"无法解析的 CAST 函数表达式中的类型: {scanner}")
 
     @classmethod
-    def parse_cast_function_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLCastFunctionExpression:
+    def parse_cast_function_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTCastFunctionExpression:
         """解析 CAST 函数表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         column_expression = cls.parse_general_expression(scanner)
         scanner.match("AS")
         signed = scanner.search_and_move("SIGNED")
         cast_type = cls.parse_cast_data_type(scanner)
-        if scanner.search(ASTMark.PARENTHESIS):
+        if scanner.search(AMTMark.PARENTHESIS):
             parenthesis_scanner = scanner.pop_as_children_scanner()
-            cast_params: Optional[List[SQLGeneralExpression]] = []
+            cast_params: Optional[List[ASTGeneralExpression] | Tuple[ASTGeneralExpression, ...]] = []
             for param_scanner in parenthesis_scanner.split_by(","):
                 cast_params.append(cls.parse_general_expression(param_scanner))
                 param_scanner.close()
+            cast_params = tuple(cast_params)
         else:
             cast_params = None
         scanner.close()
-        cast_data_type = SQLCastDataType(signed=signed, data_type=cast_type, params=cast_params)
-        return SQLCastFunctionExpression(column_expression=column_expression, cast_type=cast_data_type)
+        cast_data_type = ASTCastDataType(signed=signed, data_type=cast_type, params=cast_params)
+        return ASTCastFunctionExpression(column_expression=column_expression, cast_type=cast_data_type)
 
     @classmethod
     def parse_extract_function_expression(cls,
-                                          scanner_or_string: Union[TokenScanner, str]) -> SQLExtractFunctionExpression:
+                                          scanner_or_string: Union[TokenScanner, str]) -> ASTExtractFunctionExpression:
         """解析 EXTRACT 函数表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         extract_name = cls.parse_general_expression(scanner)
         scanner.match("FROM")
         column_expression = cls.parse_general_expression(scanner)
         scanner.close()
-        return SQLExtractFunctionExpression(extract_name=extract_name, column_expression=column_expression)
+        return ASTExtractFunctionExpression(extract_name=extract_name, column_expression=column_expression)
 
     @classmethod
-    def parse_if_function_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLNormalFunctionExpression:
+    def parse_if_function_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTNormalFunctionExpression:
         """解析 IF 函数表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
-        function_params: List[SQLGeneralExpression] = []
+        function_params: List[ASTGeneralExpression] = []
         first_param = True
         for param_scanner in scanner.split_by(","):
             if first_param is True:
                 function_params.append(cls.parse_condition_expression(param_scanner))
                 first_param = False
             else:
                 function_params.append(cls.parse_general_expression(param_scanner))
             param_scanner.close()
-        return SQLNormalFunctionExpression(function_name="IF", function_params=function_params)
+        return ASTNormalFunctionExpression(function_name="IF", function_params=tuple(function_params))
 
     @classmethod
     def parse_function_name(cls, scanner_or_string: Union[TokenScanner, str]) -> Tuple[Optional[str], str]:
         """解析函数表达式函数的 schema 名和 function 名"""
         scanner = cls._unify_input_scanner(scanner_or_string)
-        if scanner.search(ASTMark.NAME, ASTMark.PARENTHESIS):
+        if scanner.search(AMTMark.NAME, AMTMark.PARENTHESIS):
             return None, scanner.pop_as_source()
-        if scanner.search(ASTMark.NAME, ".", ASTMark.NAME, ASTMark.PARENTHESIS):
+        if scanner.search(AMTMark.NAME, ".", AMTMark.NAME, AMTMark.PARENTHESIS):
             schema_name = scanner.pop_as_source()
             scanner.pop()
-            return schema_name, scanner.pop_as_source()
+            return cls._unify_name(schema_name), cls._unify_name(scanner.pop_as_source())
         raise SqlParseError(f"无法解析为函数表达式: {scanner}")
 
     @classmethod
-    def parse_function_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> Union[SQLFunctionExpression]:
+    def parse_function_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> Union[ASTFunctionExpression]:
         """解析函数表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         schema_name, function_name = cls.parse_function_name(scanner)
 
         if function_name.upper() == "CAST":
             return cls.parse_cast_function_expression(scanner.pop_as_children_scanner())
         if function_name.upper() == "EXTRACT":
@@ -322,122 +332,122 @@
         if function_name.upper() == "IF":
             return cls.parse_if_function_expression(scanner.pop_as_children_scanner())
 
         parenthesis_scanner = scanner.pop_as_children_scanner()
         if function_name.upper() == "SUBSTRING":
             # 将 MySQL 和 PostgreSQL 中的 "SUBSTRING(str1 FROM 3 FOR 2)" 格式化为 "SUBSTRING(str1, 3, 2)"
             parenthesis_scanner = TokenScanner([
-                element if not element.equals("FROM") and not element.equals("FOR") else ASTSingle(",")
+                element if not element.equals("FROM") and not element.equals("FOR") else AMTBaseSingle(",")
                 for element in parenthesis_scanner.elements])
 
         is_distinct = False
         if function_name.upper() in AGGREGATION_FUNCTION_NAME_SET and parenthesis_scanner.search_and_move("DISTINCT"):
             is_distinct = True
 
-        function_params: List[SQLGeneralExpression] = []
+        function_params: List[ASTGeneralExpression] = []
         for param_scanner in parenthesis_scanner.split_by(","):
             function_params.append(cls.parse_general_expression(param_scanner))
             if not param_scanner.is_finish:
                 raise SqlParseError(f"无法解析函数参数: {param_scanner}")
 
         parenthesis_scanner.close()
 
         if schema_name is None and function_name.upper() in AGGREGATION_FUNCTION_NAME_SET:
-            return SQLAggregationFunctionExpression(function_name=function_name,
-                                                    function_params=function_params,
+            return ASTAggregationFunctionExpression(function_name=function_name,
+                                                    function_params=tuple(function_params),
                                                     is_distinct=is_distinct)
-        return SQLNormalFunctionExpression(schema_name=schema_name, function_name=function_name,
-                                           function_params=function_params)
+        return ASTNormalFunctionExpression(schema_name=schema_name, function_name=function_name,
+                                           function_params=tuple(function_params))
 
     @classmethod
     def parse_function_expression_maybe_with_array_index(
             cls, scanner_or_string: Union[TokenScanner, str]
-    ) -> Union[SQLFunctionExpression, SQLArrayIndexExpression]:
+    ) -> Union[ASTFunctionExpression, ASTArrayIndexExpression]:
         """解析函数表达式，并解析函数表达式后可能包含的数组下标"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         array_expression = cls.parse_function_expression(scanner)
-        if scanner.is_finish or not scanner.search(ASTMark.ARRAY_INDEX):
+        if scanner.is_finish or not scanner.search(AMTMark.ARRAY_INDEX):
             return array_expression
         idx = int(scanner.pop_as_source().lstrip("[").rstrip("]"))
-        return SQLArrayIndexExpression(array_expression=array_expression, idx=idx)
+        return ASTArrayIndexExpression(array_expression=array_expression, idx=idx)
 
     @classmethod
-    def parse_bool_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLBoolExpression:
+    def parse_bool_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTBoolExpression:
         """解析布尔值表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         is_not = scanner.search_and_move("NOT")
         if scanner.search_and_move("EXISTS"):
             after_value = cls.parse_sub_query_expression(scanner)
-            return SQLBoolExistsExpression(is_not=is_not, after_value=after_value)
+            return ASTBoolExistsExpression(is_not=is_not, after_value=after_value)
         before_value = cls.parse_general_expression(scanner)
         is_not = is_not or scanner.search_and_move("NOT")
         if scanner.search_and_move("BETWEEN"):  # "... BETWEEN ... AND ..."
             from_value = cls.parse_general_expression(scanner)
             scanner.match("AND")
             to_value = cls.parse_general_expression(scanner)
-            return SQLBoolBetweenExpression(is_not=is_not, before_value=before_value, from_value=from_value,
+            return ASTBoolBetweenExpression(is_not=is_not, before_value=before_value, from_value=from_value,
                                             to_value=to_value)
         if scanner.search_and_move("IS"):  # ".... IS ...." 或 "... IS NOT ..."
             is_not = is_not or scanner.search_and_move("NOT")
             after_value = cls.parse_general_expression(scanner)
-            return SQLBoolIsExpression(is_not=is_not, before_value=before_value, after_value=after_value)
+            return ASTBoolIsExpression(is_not=is_not, before_value=before_value, after_value=after_value)
         if scanner.search_and_move("IN"):  # "... IN (1, 2, 3)" 或 "... IN (SELECT ... )"
             after_value = cls._parse_in_parenthesis(scanner)
-            return SQLBoolInExpression(is_not=is_not, before_value=before_value, after_value=after_value)
+            return ASTBoolInExpression(is_not=is_not, before_value=before_value, after_value=after_value)
         if scanner.search_and_move("LIKE"):
             after_value = cls.parse_general_expression(scanner)
-            return SQLBoolLikeExpression(is_not=is_not, before_value=before_value, after_value=after_value)
+            return ASTBoolLikeExpression(is_not=is_not, before_value=before_value, after_value=after_value)
         if cls.check_compare_operator(scanner):  # "... > ..."
             compare_operator = cls.parse_compare_operator(scanner)
             after_value = cls.parse_general_expression(scanner)
-            return SQLBoolCompareExpression(is_not=is_not, operator=compare_operator, before_value=before_value,
+            return ASTBoolCompareExpression(is_not=is_not, operator=compare_operator, before_value=before_value,
                                             after_value=after_value)
         raise SqlParseError(f"无法解析为布尔值表达式: {scanner}")
 
     @classmethod
     def check_window_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
         """判断是否可能为窗口函数"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         return not scanner.is_finish and (
-                scanner.now.equals(ASTMark.NAME) and scanner.now.source.upper() in WINDOW_FUNCTION_NAME_SET and
-                scanner.next1 is not None and scanner.next1.equals(ASTMark.PARENTHESIS) and
+                scanner.now.equals(AMTMark.NAME) and scanner.now.source.upper() in WINDOW_FUNCTION_NAME_SET and
+                scanner.next1 is not None and scanner.next1.equals(AMTMark.PARENTHESIS) and
                 scanner.next2 is not None and scanner.next2.equals("OVER") and
-                scanner.next3 is not None and scanner.next3.equals(ASTMark.PARENTHESIS))
+                scanner.next3 is not None and scanner.next3.equals(AMTMark.PARENTHESIS))
 
     @classmethod
-    def parse_window_row(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLWindowRow:
+    def parse_window_row(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTWindowRow:
         """解析窗口函数行限制中的行"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         if scanner.search_and_move("CURRENT", "ROW"):
-            return SQLWindowRow(row_type=EnumWindowRowType.CURRENT_ROW)
+            return ASTWindowRow(row_type=EnumWindowRowType.CURRENT_ROW)
         if scanner.search_and_move("UNBOUNDED"):
             if scanner.search_and_move("PRECEDING"):
-                return SQLWindowRow(row_type=EnumWindowRowType.PRECEDING, is_unbounded=True)
+                return ASTWindowRow(row_type=EnumWindowRowType.PRECEDING, is_unbounded=True)
             if scanner.search_and_move("FOLLOWING"):
-                return SQLWindowRow(row_type=EnumWindowRowType.FOLLOWING, is_unbounded=True)
+                return ASTWindowRow(row_type=EnumWindowRowType.FOLLOWING, is_unbounded=True)
             raise SqlParseError(f"无法解析的窗口函数限制行: {scanner}")
         row_num = int(scanner.pop_as_source())
         if scanner.search_and_move("PRECEDING"):
-            return SQLWindowRow(row_type=EnumWindowRowType.PRECEDING, row_num=row_num)
+            return ASTWindowRow(row_type=EnumWindowRowType.PRECEDING, row_num=row_num)
         if scanner.search_and_move("FOLLOWING"):
-            return SQLWindowRow(row_type=EnumWindowRowType.FOLLOWING, row_num=row_num)
+            return ASTWindowRow(row_type=EnumWindowRowType.FOLLOWING, row_num=row_num)
         raise SqlParseError(f"无法解析的窗口函数限制行: {scanner}")
 
     @classmethod
-    def parse_window_row_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLWindowRowExpression:
+    def parse_window_row_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTWindowRowExpression:
         """解析窗口语句限制行的表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         scanner.match("ROWS", "BETWEEN")
         from_row = cls.parse_window_row(scanner)
         scanner.match("AND")
         to_row = cls.parse_window_row(scanner)
-        return SQLWindowRowExpression(from_row=from_row, to_row=to_row)
+        return ASTWindowRowExpression(from_row=from_row, to_row=to_row)
 
     @classmethod
-    def parse_window_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLWindowExpression:
+    def parse_window_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTWindowExpression:
         """解析窗口函数"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         window_function = cls.parse_function_expression_maybe_with_array_index(scanner)
         partition_by = None
         order_by = None
         row_expression = None
         scanner.match("OVER")
@@ -445,68 +455,68 @@
         if parenthesis_scanner.search_and_move("PARTITION", "BY"):
             partition_by = cls.parse_general_expression(parenthesis_scanner, maybe_window=False)
         if parenthesis_scanner.search_and_move("ORDER", "BY"):
             order_by = cls.parse_general_expression(parenthesis_scanner, maybe_window=False)
         if parenthesis_scanner.search("ROWS", "BETWEEN"):
             row_expression = cls.parse_window_row_expression(parenthesis_scanner)
         parenthesis_scanner.close()
-        return SQLWindowExpression(window_function=window_function,
+        return ASTWindowExpression(window_function=window_function,
                                    partition_by=partition_by,
                                    order_by=order_by,
                                    row_expression=row_expression)
 
     @classmethod
     def check_wildcard_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
         """判断是否可能为通配符表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
-        return scanner.search("*") or scanner.search(ASTMark.NAME, ".", "*")
+        return scanner.search("*") or scanner.search(AMTMark.NAME, ".", "*")
 
     @classmethod
-    def parse_wildcard_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLWildcardExpression:
+    def parse_wildcard_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTWildcardExpression:
         """解析通配符表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         if scanner.search_and_move("*"):
-            return SQLWildcardExpression()
-        if scanner.search(ASTMark.NAME, ".", "*"):
+            return ASTWildcardExpression()
+        if scanner.search(AMTMark.NAME, ".", "*"):
             schema_name = scanner.pop_as_source()
             scanner.pop()
             scanner.pop()
-            return SQLWildcardExpression(schema=schema_name)
+            return ASTWildcardExpression(schema=schema_name)
         raise SqlParseError("无法解析为通配符表达式")
 
     @classmethod
-    def parse_condition_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLConditionExpression:
+    def parse_condition_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTConditionExpression:
         """解析条件表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
 
         def parse_single():
-            if scanner.search(ASTMark.PARENTHESIS):
+            if scanner.search(AMTMark.PARENTHESIS):
                 parenthesis_scanner = scanner.pop_as_children_scanner()
                 elements.append(cls.parse_condition_expression(parenthesis_scanner))  # 插入语，子句也应该是一个条件表达式
                 parenthesis_scanner.close()
             else:
                 elements.append(cls.parse_bool_expression(scanner))
 
-        elements: List[Union["SQLConditionExpression", SQLBoolExpression, SQLLogicalOperator]] = []
+        elements: List[Union["ASTConditionExpression", ASTBoolExpression, ASTLogicalOperator]] = []
         parse_single()  # 解析第 1 个表达式元素
         while not scanner.is_finish and scanner.now.source.upper() in {"AND", "OR"}:  # 如果是用 AND 和 OR 连接的多个表达式，则继续解析
             elements.append(cls.parse_logical_operator(scanner))
             parse_single()
 
-        return SQLConditionExpression(elements=elements)
+        return ASTConditionExpression(elements=tuple(elements))
 
     @classmethod
     def check_case_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
         """判断是否可能为 CASE 表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         return scanner.search("CASE")
 
     @classmethod
     def parse_case_expression(cls, scanner_or_string: Union[TokenScanner, str]
-                              ) -> Union[SQLCaseExpression, SQLCaseValueExpression]:
+                              ) -> Union[ASTCaseExpression, ASTCaseValueExpression]:
         """解析 CASE 表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         scanner.match("CASE")
         if scanner.search("WHEN"):
             # 第 1 种格式的 CASE 表达式
             cases = []
             else_value = None
@@ -514,360 +524,410 @@
                 when_expression = cls.parse_condition_expression(scanner)
                 scanner.match("THEN")
                 case_expression = cls.parse_general_expression(scanner)
                 cases.append((when_expression, case_expression))
             if scanner.search_and_move("ELSE"):
                 else_value = cls.parse_general_expression(scanner)
             scanner.match("END")
-            return SQLCaseExpression(cases=cases, else_value=else_value)
+            return ASTCaseExpression(cases=tuple(cases), else_value=else_value)
         # 第 2 种格式的 CASE 表达式
         case_value = cls.parse_general_expression(scanner)
         cases = []
         else_value = None
         while scanner.search_and_move("WHEN"):
             when_expression = cls.parse_general_expression(scanner)
             scanner.match("THEN")
             case_expression = cls.parse_general_expression(scanner)
             cases.append((when_expression, case_expression))
         if scanner.search_and_move("ELSE"):
             else_value = cls.parse_general_expression(scanner)
         scanner.match("END")
-        return SQLCaseValueExpression(case_value=case_value, cases=cases, else_value=else_value)
+        return ASTCaseValueExpression(case_value=case_value, cases=tuple(cases), else_value=else_value)
 
     @classmethod
-    def parse_value_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLValueExpression:
+    def parse_value_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTValueExpression:
         """解析值表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         values = []
         for value_scanner in scanner.pop_as_children_scanner_list_split_by(","):
             values.append(cls.parse_general_expression(value_scanner))
             value_scanner.close()
-        return SQLValueExpression(values=values)
+        return ASTValueExpression(values=tuple(values))
 
     @classmethod
     def check_sub_query_parenthesis(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
         """判断是否为子查询的插入语"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         return cls.check_select_statement(scanner.get_as_children_scanner())
 
     @classmethod
-    def parse_sub_query_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLSubQueryExpression:
+    def parse_sub_query_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTSubQueryExpression:
         """解析子查询表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         parenthesis_scanner = scanner.pop_as_children_scanner()
-        result = SQLSubQueryExpression(select_statement=cls.parse_select_statement(parenthesis_scanner))
+        result = ASTSubQueryExpression(select_statement=cls.parse_select_statement(parenthesis_scanner))
         parenthesis_scanner.close()
         return result
 
     @classmethod
-    def _parse_in_parenthesis(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLGeneralExpression:
+    def _parse_in_parenthesis(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTGeneralExpression:
         """解析 IN 关键字后的插入语：插入语可能为子查询或值表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         if cls.check_sub_query_parenthesis(scanner):
             return cls.parse_sub_query_expression(scanner)
         return cls.parse_value_expression(scanner)
 
     @classmethod
-    def _parse_general_parenthesis(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLGeneralExpression:
+    def _parse_general_parenthesis(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTGeneralExpression:
         """解析一般表达式中的插入语：插入语可能为一般表达式或子查询"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         if cls.check_sub_query_parenthesis(scanner):
             return cls.parse_sub_query_expression(scanner)
         parenthesis_scanner = scanner.pop_as_children_scanner()
         result = cls.parse_general_expression(parenthesis_scanner)
         parenthesis_scanner.close()
         return result
 
     @classmethod
     def parse_general_expression_element(cls, scanner_or_string: Union[TokenScanner, str],
-                                         maybe_window: bool) -> SQLGeneralExpression:
+                                         maybe_window: bool) -> ASTGeneralExpression:
         """解析一般表达式中的一个元素"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         if cls.check_case_expression(scanner):
             return cls.parse_case_expression(scanner)
         if maybe_window is True and cls.check_window_expression(scanner):
             return cls.parse_window_expression(scanner)
         if cls.check_function_expression(scanner):
             return cls.parse_function_expression_maybe_with_array_index(scanner)
         if cls.check_literal_expression(scanner):
             return cls.parse_literal_expression(scanner)
         if cls.check_column_name_expression(scanner):
             return cls.parse_column_name_expression(scanner)
-        if scanner.search(ASTMark.PARENTHESIS):
+        if scanner.search(AMTMark.PARENTHESIS):
             return cls._parse_general_parenthesis(scanner)
         if cls.check_wildcard_expression(scanner):
             return cls.parse_wildcard_expression(scanner)
         raise SqlParseError(f"未知的一般表达式元素: {scanner}")
 
     @classmethod
     def parse_general_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                                 maybe_window: bool = True) -> SQLGeneralExpression:
+                                 maybe_window: bool = True) -> ASTGeneralExpression:
         """解析一般表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         elements = [cls.parse_general_expression_element(scanner, maybe_window)]
         while cls.check_compute_operator(scanner):
             elements.append(cls.parse_compute_operator(scanner))
             elements.append(cls.parse_general_expression_element(scanner, maybe_window))
         if len(elements) == 1:
             return elements[0]  # 如果只有 1 个元素，则返回该元素的表达式
-        return SQLComputeExpression(elements=elements)  # 如果超过 1 个元素，则返回计算表达式（多项式）
+        return ASTComputeExpression(elements=tuple(elements))  # 如果超过 1 个元素，则返回计算表达式（多项式）
 
     @classmethod
-    def parse_config_name_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLConfigNameExpression:
+    def parse_config_name_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTConfigNameExpression:
         """解析配置名称表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         config_name_list = [scanner.pop_as_source()]
         while scanner.search_and_move("."):
             config_name_list.append(scanner.pop_as_source())
-        return SQLConfigNameExpression(config_name=".".join(config_name_list))
+        return ASTConfigNameExpression(config_name=".".join(config_name_list))
 
     @classmethod
-    def parse_config_value_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLConfigValueExpression:
+    def parse_config_value_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTConfigValueExpression:
         """解析配置值表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
-        return SQLConfigValueExpression(config_value=scanner.pop_as_source())
+        return ASTConfigValueExpression(config_value=scanner.pop_as_source())
 
     @classmethod
     def parse_table_name_expression(cls, scanner_or_string: Union[TokenScanner, str]
-                                    ) -> Union[SQLTableNameExpression, SQLSubQueryExpression]:
+                                    ) -> Union[ASTTableNameExpression, ASTSubQueryExpression]:
         """解析表名表达式或子查询表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
-        if (scanner.search(ASTMark.NAME, ".", ASTMark.NAME) and
-                not scanner.search(ASTMark.NAME, ".", ASTMark.NAME, ASTMark.PARENTHESIS)):
+        if scanner.search(AMTMark.NAME, ".", AMTMark.NAME):
             schema_name = scanner.pop_as_source()
             scanner.pop()
             table_name = scanner.pop_as_source()
-            return SQLTableNameExpression(schema=schema_name, table=table_name)
-        if scanner.search(ASTMark.NAME) and not scanner.search(ASTMark.NAME, ASTMark.PARENTHESIS):
-            return SQLTableNameExpression(table=scanner.pop_as_source())
+            return ASTTableNameExpression(schema=cls._unify_name(schema_name), table=cls._unify_name(table_name))
+        if scanner.search(AMTMark.NAME):
+            name_source = scanner.pop_as_source()
+            if name_source.count(".") == 1:
+                schema_name, table_name = name_source.strip("`").split(".")
+            else:
+                schema_name, table_name = None, name_source
+            return ASTTableNameExpression(schema=cls._unify_name(schema_name), table=cls._unify_name(table_name))
         if cls.check_sub_query_parenthesis(scanner):
             return cls.parse_sub_query_expression(scanner)
         raise SqlParseError(f"无法解析为表名表达式: {scanner}")
 
     @classmethod
     def check_alias_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
         """判断是否可能为别名表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
-        return not scanner.is_finish and (scanner.search("AS") or scanner.search(ASTMark.NAME))
+        return not scanner.is_finish and (scanner.search("AS") or scanner.search(AMTMark.NAME))
 
     @classmethod
     def parse_alias_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                               must_has_as_keyword: bool = False) -> SQLAlisaExpression:
+                               must_has_as_keyword: bool = False) -> ASTAlisaExpression:
         """解析别名表达式
 
         Parameters
         ----------
         scanner_or_string : str
             词法扫描器或 SQL 字符串语句
         must_has_as_keyword : bool, default = False
             是否必须包含 AS 关键字
         """
         scanner = cls._unify_input_scanner(scanner_or_string)
         if must_has_as_keyword is True:
             scanner.match("AS")
         else:
             scanner.search_and_move("AS")
-        if not scanner.search(ASTMark.NAME):
+        if not scanner.search(AMTMark.NAME):
             raise SqlParseError(f"无法解析为别名表达式: {scanner}")
-        return SQLAlisaExpression(name=scanner.pop_as_source())
+        return ASTAlisaExpression(name=cls._unify_name(scanner.pop_as_source()))
 
     @classmethod
     def check_join_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
         """判断是否为关联表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         return scanner.search("ON") or scanner.search("USING")
 
     @classmethod
-    def parse_join_on_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLJoinOnExpression:
+    def parse_join_on_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTJoinOnExpression:
         """解析 ON 关联表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         if not scanner.search_and_move("ON"):
             raise SqlParseError(f"无法解析为 ON 关联表达式: {scanner}")
-        return SQLJoinOnExpression(condition=cls.parse_condition_expression(scanner))
+        return ASTJoinOnExpression(condition=cls.parse_condition_expression(scanner))
 
     @classmethod
-    def parse_join_using_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLJoinUsingExpression:
+    def parse_join_using_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTJoinUsingExpression:
         """解析 USING 关联表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         if not scanner.search("USING"):
             raise SqlParseError(f"无法解析为 USING 关联表达式: {scanner}")
-        return SQLJoinUsingExpression(using_function=cls.parse_function_expression(scanner))
+        return ASTJoinUsingExpression(using_function=cls.parse_function_expression(scanner))
 
     @classmethod
-    def parse_join_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLJoinExpression:
+    def parse_join_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTJoinExpression:
         """解析关联表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         if scanner.search("ON"):
             return cls.parse_join_on_expression(scanner)
         if scanner.search("USING"):
             return cls.parse_join_using_expression(scanner)
         raise SqlParseError(f"无法解析为关联表达式: {scanner}")
 
     @classmethod
-    def parse_column_type_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLColumnTypeExpression:
+    def parse_column_type_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTColumnTypeExpression:
         """解析 DDL 的字段类型：要求当前指针位置节点为函数名，下一个节点可能为函数参数也可能不是，解析为 SQLColumnType 对象"""
         scanner = cls._unify_input_scanner(scanner_or_string)
 
         # 解析字段类型名称
         function_name: str = scanner.pop_as_source()
 
         # 解析字段类型参数
-        if scanner.search(ASTMark.PARENTHESIS):
-            function_params: List[SQLGeneralExpression] = []
+        if scanner.search(AMTMark.PARENTHESIS):
+            function_params: List[ASTGeneralExpression] = []
             for param_scanner in scanner.pop_as_children_scanner_list_split_by(","):
                 function_params.append(cls.parse_general_expression(param_scanner))
                 param_scanner.close()
-            return SQLColumnTypeExpression(name=function_name, params=function_params)
-        return SQLColumnTypeExpression(name=function_name)
+            return ASTColumnTypeExpression(name=function_name, params=tuple(function_params))
+        return ASTColumnTypeExpression(name=function_name)
 
     @classmethod
-    def parse_table_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLTableExpression:
+    def parse_table_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTTableExpression:
         """解析表名表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         table_name_expression = cls.parse_table_name_expression(scanner)
         alias_expression = cls.parse_alias_expression(scanner) if cls.check_alias_expression(scanner) else None
-        return SQLTableExpression(table=table_name_expression, alias=alias_expression)
+        return ASTTableExpression(table=table_name_expression, alias=alias_expression)
 
     @classmethod
-    def parse_column_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLColumnExpression:
+    def parse_column_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTColumnExpression:
         """解析列名表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         general_expression = cls.parse_general_expression(scanner)
         alias_expression = cls.parse_alias_expression(scanner) if cls.check_alias_expression(scanner) else None
-        return SQLColumnExpression(column=general_expression, alias=alias_expression)
+        return ASTColumnExpression(column=general_expression, alias=alias_expression)
 
     @classmethod
-    def parse_equal_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLEqualExpression:
+    def parse_equal_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTEqualExpression:
         """解析等式表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         before_value = cls.parse_general_expression(scanner)
         scanner.match("=")
         after_value = cls.parse_general_expression(scanner)
-        return SQLEqualExpression(before_value=before_value, after_value=after_value)
+        return ASTEqualExpression(before_value=before_value, after_value=after_value)
 
     @classmethod
     def check_partition_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
         """判断是否可能为分区表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         return scanner.search("PARTITION")
 
     @classmethod
-    def parse_partition_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLPartitionExpression:
+    def parse_partition_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTPartitionExpression:
         """解析分区表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         scanner.match("PARTITION")
         partition_list = []
         for partition_scanner in scanner.pop_as_children_scanner_list_split_by(","):
             partition_list.append(cls.parse_equal_expression(partition_scanner))
             partition_scanner.close()
-        return SQLPartitionExpression(partition_list=partition_list)
+        return ASTPartitionExpression(partition_list=tuple(partition_list))
 
     @classmethod
     def check_foreign_key_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
         """判断是否为外键表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         return scanner.search("CONSTRAINT")
 
     @classmethod
-    def parse_foreign_key_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLForeignKeyExpression:
+    def parse_foreign_key_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTForeignKeyExpression:
         """解析外键表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         scanner.match("CONSTRAINT")
         constraint_name = scanner.pop_as_source()
         scanner.match("FOREIGN", "KEY")
         slave_columns = []
         for column_scanner in scanner.pop_as_children_scanner_list_split_by(","):
-            column_scanner.pop_as_source()
+            slave_columns.append(column_scanner.pop_as_source())
             column_scanner.close()
         scanner.match("REFERENCES")
         master_table_name = scanner.pop_as_source()
         master_columns = []
         for column_scanner in scanner.pop_as_children_scanner_list_split_by(","):
-            column_scanner.pop_as_source()
+            master_columns.append(column_scanner.pop_as_source())
             column_scanner.close()
-        return SQLForeignKeyExpression(
+        on_delete_cascade = scanner.search_and_move("ON", "DELETE", "CASCADE")
+        return ASTForeignKeyExpression(
             constraint_name=constraint_name,
-            slave_columns=slave_columns,
+            slave_columns=tuple(slave_columns),
             master_table_name=master_table_name,
-            master_columns=master_columns
+            master_columns=tuple(master_columns),
+            on_delete_cascade=on_delete_cascade
         )
 
     @classmethod
+    def parse_index_column(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTIndexColumn:
+        """解析索引声明表达式中的字段"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        name = cls._unify_name(scanner.pop_as_source())
+        max_length = None
+        if scanner.search(AMTMark.PARENTHESIS):
+            parenthesis_scanner = scanner.pop_as_children_scanner()
+            max_length = int(parenthesis_scanner.pop_as_source())
+            parenthesis_scanner.close()
+        return ASTIndexColumn(name=name, max_length=max_length)
+
+    @classmethod
     def check_primary_index_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
         """判断是否为主键表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         return scanner.search("PRIMARY", "KEY")
 
     @classmethod
-    def parse_primary_index_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLPrimaryIndexExpression:
+    def parse_primary_index_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTPrimaryIndexExpression:
         """解析主键表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         scanner.match("PRIMARY", "KEY")
         columns = []
         for column_scanner in scanner.pop_as_children_scanner_list_split_by(","):
-            column_scanner.pop_as_source()
+            columns.append(cls.parse_index_column(column_scanner))
             column_scanner.close()
-        return SQLPrimaryIndexExpression(columns=columns)
+        using = scanner.pop_as_source() if scanner.search_and_move("USING") else None
+        comment = scanner.pop_as_source() if scanner.search_and_move("COMMENT") else None
+        if scanner.search_and_move("KEY_BLOCK_SIZE"):
+            scanner.match("=")
+            key_block_size = int(scanner.pop_as_source())
+        else:
+            key_block_size = None
+        return ASTPrimaryIndexExpression(columns=tuple(columns), using=using, comment=comment,
+                                         key_block_size=key_block_size)
 
     @classmethod
     def check_unique_index_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
         """判断是否为唯一键表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         return scanner.search("UNIQUE", "KEY")
 
     @classmethod
-    def parse_unique_index_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLUniqueIndexExpression:
+    def parse_unique_index_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTUniqueIndexExpression:
         """解析唯一键表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         scanner.match("UNIQUE", "KEY")
         name = scanner.pop_as_source()
         columns = []
         for column_scanner in scanner.pop_as_children_scanner_list_split_by(","):
-            column_scanner.pop_as_source()
+            columns.append(cls.parse_index_column(column_scanner))
             column_scanner.close()
-        return SQLUniqueIndexExpression(name=name, columns=columns)
+        using = scanner.pop_as_source() if scanner.search_and_move("USING") else None
+        comment = scanner.pop_as_source() if scanner.search_and_move("COMMENT") else None
+        if scanner.search_and_move("KEY_BLOCK_SIZE"):
+            scanner.match("=")
+            key_block_size = int(scanner.pop_as_source())
+        else:
+            key_block_size = None
+        return ASTUniqueIndexExpression(name=name, columns=tuple(columns), using=using, comment=comment,
+                                        key_block_size=key_block_size)
 
     @classmethod
     def check_normal_index_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
         """判断是否为一般索引表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         return scanner.search("KEY")
 
     @classmethod
-    def parse_normal_index_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLNormalIndexExpression:
+    def parse_normal_index_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTNormalIndexExpression:
         """解析一般索引表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         scanner.match("KEY")
         name = scanner.pop_as_source()
         columns = []
         for column_scanner in scanner.pop_as_children_scanner_list_split_by(","):
-            column_scanner.pop_as_source()
+            columns.append(cls.parse_index_column(column_scanner))
             column_scanner.close()
-        return SQLNormalIndexExpression(name=name, columns=columns)
+        using = scanner.pop_as_source() if scanner.search_and_move("USING") else None
+        comment = scanner.pop_as_source() if scanner.search_and_move("COMMENT") else None
+        if scanner.search_and_move("KEY_BLOCK_SIZE"):
+            scanner.match("=")
+            key_block_size = int(scanner.pop_as_source())
+        else:
+            key_block_size = None
+        return ASTNormalIndexExpression(name=name, columns=tuple(columns), using=using, comment=comment,
+                                        key_block_size=key_block_size)
 
     @classmethod
     def check_fulltext_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
         """判断是否为全文索引表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         return scanner.search("FULLTEXT", "KEY")
 
     @classmethod
-    def parse_fulltext_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLFulltextIndexExpression:
+    def parse_fulltext_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTFulltextIndexExpression:
         """解析全文索引表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         scanner.match("FULLTEXT", "KEY")
         name = scanner.pop_as_source()
         columns = []
         for column_scanner in scanner.pop_as_children_scanner_list_split_by(","):
-            column_scanner.pop_as_source()
+            columns.append(cls.parse_index_column(column_scanner))
             column_scanner.close()
-        return SQLFulltextIndexExpression(name=name, columns=columns)
+        using = scanner.pop_as_source() if scanner.search_and_move("USING") else None
+        comment = scanner.pop_as_source() if scanner.search_and_move("COMMENT") else None
+        if scanner.search_and_move("KEY_BLOCK_SIZE"):
+            scanner.match("=")
+            key_block_size = int(scanner.pop_as_source())
+        else:
+            key_block_size = None
+        return ASTFulltextIndexExpression(name=name, columns=tuple(columns), using=using, comment=comment,
+                                          key_block_size=key_block_size)
 
     @classmethod
-    def parse_define_column_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLDefineColumnExpression:
+    def parse_define_column_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTDefineColumnExpression:
         """解析 DDL 的字段表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         # 解析顺序固定的信息
         column_name = scanner.pop_as_source()
         column_type = cls.parse_column_type_expression(scanner)
 
         # 解析顺序可能不定的字段信息
@@ -875,16 +935,16 @@
         is_unsigned: bool = False
         is_zerofill: bool = False
         character_set: Optional[str] = None
         collate: Optional[str] = None
         is_allow_null: bool = False
         is_not_null: bool = False
         is_auto_increment: bool = False
-        default: Optional[SQLGeneralExpression] = None
-        on_update: Optional[SQLGeneralExpression] = None
+        default: Optional[ASTGeneralExpression] = None
+        on_update: Optional[ASTGeneralExpression] = None
         while not scanner.is_finish:
             if scanner.search_and_move("NOT", "NULL"):
                 is_not_null = True
             elif scanner.search_and_move("NULL"):
                 is_allow_null = True
             elif scanner.search_and_move("CHARACTER", "SET"):
                 character_set = scanner.pop_as_source()
@@ -902,16 +962,16 @@
                 is_unsigned = True
             elif scanner.search_and_move("ZEROFILL"):
                 is_zerofill = True
             else:
                 raise SqlParseError(f"无法解析的 DDL 字段表达式的字段属性: {scanner}")
 
         # 构造 DDL 字段表达式对象
-        return SQLDefineColumnExpression(
-            column_name=column_name,
+        return ASTDefineColumnExpression(
+            column_name=cls._unify_name(column_name),
             column_type=column_type,
             comment=comment,
             is_unsigned=is_unsigned,
             is_zerofill=is_zerofill,
             character_set=character_set,
             collate=collate,
             is_allow_null=is_allow_null,
@@ -924,216 +984,216 @@
     @classmethod
     def check_select_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
         """判断是否为 SELECT 子句"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         return scanner.search("SELECT")
 
     @classmethod
-    def parse_select_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLSelectClause:
+    def parse_select_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTSelectClause:
         """解析 SELECT 子句"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         scanner.match("SELECT")
         distinct = scanner.search_and_move("DISTINCT")
         columns = [cls.parse_column_expression(scanner)]
         while scanner.search_and_move(","):
             columns.append(cls.parse_column_expression(scanner))
-        return SQLSelectClause(distinct=distinct, columns=columns)
+        return ASTSelectClause(distinct=distinct, columns=tuple(columns))
 
     @classmethod
     def check_from_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
         """判断是否为 FROM 子句"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         return scanner.search("FROM")
 
     @classmethod
-    def parse_from_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLFromClause:
+    def parse_from_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTFromClause:
         """解析 FROM 子句"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         scanner.match("FROM")
         tables = [cls.parse_table_expression(scanner)]
         while scanner.search_and_move(","):
             tables.append(cls.parse_table_expression(scanner))
-        return SQLFromClause(tables=tables)
+        return ASTFromClause(tables=tuple(tables))
 
     @classmethod
     def check_lateral_view_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
         """判断是否为 LATERAL VIEW 子句"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         return scanner.search("LATERAL", "VIEW")
 
     @classmethod
-    def parse_lateral_view_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLLateralViewClause:
+    def parse_lateral_view_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTLateralViewClause:
         """解析 LATERAL VIEW 子句"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         scanner.match("LATERAL", "VIEW")
         function = cls.parse_function_expression(scanner)
         view_name = scanner.pop_as_source()
         alias = cls.parse_alias_expression(scanner, must_has_as_keyword=True)
-        return SQLLateralViewClause(function=function, view_name=view_name, alias=alias)
+        return ASTLateralViewClause(function=function, view_name=view_name, alias=alias)
 
     @classmethod
     def check_join_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
         """判断是否为 JOIN 子句"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         return cls.check_join_type(scanner)
 
     @classmethod
-    def parse_join_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLJoinClause:
+    def parse_join_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTJoinClause:
         """解析 JOIN 子句"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         join_type = cls.parse_join_type(scanner)
         table_expression = cls.parse_table_expression(scanner)
         if cls.check_join_expression(scanner):
             join_rule = cls.parse_join_expression(scanner)
         else:
             join_rule = None
-        return SQLJoinClause(join_type=join_type, table=table_expression, join_rule=join_rule)
+        return ASTJoinClause(join_type=join_type, table=table_expression, join_rule=join_rule)
 
     @classmethod
     def check_where_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
         """判断是否可能为 WHERE 子句"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         return scanner.search("WHERE")
 
     @classmethod
-    def parse_where_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLWhereClause:
+    def parse_where_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTWhereClause:
         """解析 WHERE 子句"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         scanner.match("WHERE")
-        return SQLWhereClause(condition=cls.parse_condition_expression(scanner))
+        return ASTWhereClause(condition=cls.parse_condition_expression(scanner))
 
     @classmethod
     def check_group_by_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
         """判断是否可能为 GROUP BY 子句"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         return scanner.search("GROUP", "BY")
 
     @classmethod
-    def parse_group_by_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLGroupByClause:
+    def parse_group_by_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTGroupByClause:
         """解析 GROUP BY 子句"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         scanner.match("GROUP", "BY")
         if scanner.search_and_move("GROUPING", "SETS"):
             # 处理 GROUPING SETS 的语法
             grouping_list = []
             for grouping_scanner in scanner.pop_as_children_scanner_list_split_by(","):
-                if grouping_scanner.search(ASTMark.PARENTHESIS):
+                if grouping_scanner.search(AMTMark.PARENTHESIS):
                     parenthesis_scanner_list = grouping_scanner.pop_as_children_scanner_list_split_by(",")
                     columns_list = []
                     for parenthesis_scanner in parenthesis_scanner_list:
                         cls.parse_general_expression(parenthesis_scanner)
                         parenthesis_scanner.close()
-                    grouping_list.append(columns_list)
+                    grouping_list.append(tuple(columns_list))
                 else:
-                    grouping_list.append([cls.parse_general_expression(grouping_scanner)])
+                    grouping_list.append(tuple([cls.parse_general_expression(grouping_scanner)]))
                 grouping_scanner.close()
-            return SQLGroupingSetsGroupByClause(grouping_list=grouping_list)
+            return ASTGroupingSetsGroupByClause(grouping_list=tuple(grouping_list))
 
         # 处理一般的 GROUP BY 的语法
         columns = [cls.parse_general_expression(scanner)]
         while scanner.search_and_move(","):
             columns.append(cls.parse_general_expression(scanner))
         with_rollup = False
         if scanner.search_and_move("WITH", "ROLLUP"):
             with_rollup = True
-        return SQLNormalGroupByClause(columns=columns, with_rollup=with_rollup)
+        return ASTNormalGroupByClause(columns=tuple(columns), with_rollup=with_rollup)
 
     @classmethod
     def check_having_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
         """是否可能为 HAVING 子句"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         return scanner.search("HAVING")
 
     @classmethod
-    def parse_having_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLHavingClause:
+    def parse_having_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTHavingClause:
         """解析 HAVING 子句"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         scanner.match("HAVING")
-        return SQLHavingClause(condition=cls.parse_condition_expression(scanner))
+        return ASTHavingClause(condition=cls.parse_condition_expression(scanner))
 
     @classmethod
     def check_order_by_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
         """是否可能为 ORDER BY 子句"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         return scanner.search("ORDER", "BY")
 
     @classmethod
-    def parse_order_by_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLOrderByClause:
+    def parse_order_by_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTOrderByClause:
         """解析 ORDER BY 子句"""
         scanner = cls._unify_input_scanner(scanner_or_string)
 
         def parse_single():
             column = cls.parse_general_expression(scanner)
             order = cls.parse_order_type(scanner)
             columns.append((column, order))
 
         scanner.match("ORDER", "BY")
         columns = []
         parse_single()
         while scanner.search_and_move(","):
             parse_single()
 
-        return SQLOrderByClause(columns=columns)
+        return ASTOrderByClause(columns=tuple(columns))
 
     @classmethod
     def check_limit_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
         """是否可能为 LIMIT 子句"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         return scanner.search("LIMIT")
 
     @classmethod
-    def parse_limit_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLLimitClause:
+    def parse_limit_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTLimitClause:
         """解析 LIMIT 子句"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         if not scanner.search_and_move("LIMIT"):
             raise SqlParseError("无法解析为 LIMIT 子句")
         cnt_1 = cls.parse_literal_expression(scanner).as_int()
         if scanner.search_and_move(","):
             offset_int = cnt_1
             limit_int = cls.parse_literal_expression(scanner).as_int()
         elif scanner.search_and_move("OFFSET"):
             offset_int = cls.parse_literal_expression(scanner).as_int()
             limit_int = cnt_1
         else:
             raise SqlParseError("无法解析为 LIMIT 子句")
-        return SQLLimitClause(limit=limit_int, offset=offset_int)
+        return ASTLimitClause(limit=limit_int, offset=offset_int)
 
     @classmethod
-    def _parse_single_with_table(cls, scanner_or_string: Union[TokenScanner, str]) -> Tuple[str, SQLSelectStatement]:
+    def _parse_single_with_table(cls, scanner_or_string: Union[TokenScanner, str]) -> Tuple[str, ASTSelectStatement]:
         """解析一个 WITH 临时表"""
         scanner = cls._unify_input_scanner(scanner_or_string)
-        table_name = scanner.pop_as_source()
+        table_name = cls._unify_name(scanner.pop_as_source())
         scanner.match("AS")
         parenthesis_scanner = scanner.pop_as_children_scanner()
-        table_statement = cls.parse_select_statement(parenthesis_scanner, with_clause=SQLWithClause.empty())
+        table_statement = cls.parse_select_statement(parenthesis_scanner, with_clause=ASTWithClause.empty())
         parenthesis_scanner.close()
         return table_name, table_statement
 
     @classmethod
-    def parse_with_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> Optional[SQLWithClause]:
+    def parse_with_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> Optional[ASTWithClause]:
         """解析 WITH 子句"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         if scanner.search_and_move("WITH"):
             tables = [cls._parse_single_with_table(scanner)]
             while scanner.search_and_move(","):
                 table_statement = cls._parse_single_with_table(scanner)
                 tables.append(table_statement)  # 将前置的 WITH 作为当前解析临时表的 WITH 子句
-            return SQLWithClause(tables=tables)
-        return SQLWithClause.empty()
+            return ASTWithClause(tables=tuple(tables))
+        return ASTWithClause.empty()
 
     @classmethod
     def check_select_statement(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
         """判断是否可能为 SELECT 语句"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         return scanner.search("SELECT")
 
     @classmethod
     def parse_single_select_statement(cls, scanner_or_string: Union[TokenScanner, str],
-                                      with_clause: Optional[SQLWithClause] = None
-                                      ) -> SQLSingleSelectStatement:
+                                      with_clause: Optional[ASTWithClause] = None
+                                      ) -> ASTSingleSelectStatement:
         """
 
         Parameters
         ----------
         scanner_or_string : Union[TokenScanner, str]
             扫描器
         with_clause : Optional[SQLWithClause], default = None
@@ -1155,57 +1215,61 @@
         while cls.check_join_clause(scanner):
             join_clause.append(cls.parse_join_clause(scanner))
         where_clause = cls.parse_where_clause(scanner) if cls.check_where_clause(scanner) else None
         group_by_clause = cls.parse_group_by_clause(scanner) if cls.check_group_by_clause(scanner) else None
         having_clause = cls.parse_having_clause(scanner) if cls.check_having_clause(scanner) else None
         order_by_clause = cls.parse_order_by_clause(scanner) if cls.check_order_by_clause(scanner) else None
         limit_clause = cls.parse_limit_clause(scanner) if cls.check_limit_clause(scanner) else None
-        return SQLSingleSelectStatement(
+        return ASTSingleSelectStatement(
             with_clause=with_clause,
             select_clause=select_clause,
             from_clause=from_clause,
-            lateral_view_clauses=lateral_view_clauses,
-            join_clauses=join_clause,
+            lateral_view_clauses=tuple(lateral_view_clauses),
+            join_clauses=tuple(join_clause),
             where_clause=where_clause,
             group_by_clause=group_by_clause,
             having_clause=having_clause,
             order_by_clause=order_by_clause,
             limit_clause=limit_clause
         )
 
     @classmethod
     def parse_select_statement(cls, scanner_or_string: Union[TokenScanner, str],
-                               with_clause: Optional[SQLWithClause] = None) -> SQLSelectStatement:
+                               with_clause: Optional[ASTWithClause] = None) -> ASTSelectStatement:
         """解析 SELECT 语句"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         if with_clause is None:
             with_clause = cls.parse_with_clause(scanner)
         result = [cls.parse_single_select_statement(scanner, with_clause=with_clause)]
         while not scanner.is_finish and cls.check_union_type(scanner):
             result.append(cls.parse_union_type(scanner))
             result.append(cls.parse_single_select_statement(scanner, with_clause=with_clause))
         scanner.search_and_move(";")
         if not scanner.is_finish:
             raise SqlParseError(f"没有解析完成: {scanner}")
 
         if len(result) == 1:
             return result[0]
-        return SQLUnionSelectStatement(with_clause=with_clause, elements=result)
+        return ASTUnionSelectStatement(with_clause=with_clause, elements=tuple(result))
 
     @classmethod
     def check_insert_statement(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
         """判断是否为 INSERT 语句（已匹配过 WITH 语句才可以调用）"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         return scanner.search("INSERT")
 
     @classmethod
     def parse_insert_statement(cls, scanner_or_string: Union[TokenScanner, str],
-                               with_clause: SQLWithClause) -> SQLInsertStatement:
+                               with_clause: Optional[ASTWithClause]) -> ASTInsertStatement:
         """解析 INSERT 表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string)
+
+        if with_clause is None:
+            with_clause = cls.parse_with_clause(scanner)
+
         insert_type = cls.parse_insert_type(scanner)
 
         # 匹配可能包含的 TABLE 关键字
         scanner.search_and_move("TABLE")
 
         # 匹配表名
         table_name = cls.parse_table_name_expression(scanner)
@@ -1213,83 +1277,83 @@
         # 匹配分区表达式
         if cls.check_partition_expression(scanner):
             partition = cls.parse_partition_expression(scanner)
         else:
             partition = None
 
         # 匹配列名列表
-        if scanner.search(ASTMark.PARENTHESIS):
+        if scanner.search(AMTMark.PARENTHESIS):
             columns = []
             for column_scanner in scanner.pop_as_children_scanner_list_split_by(","):
                 columns.append(cls.parse_column_name_expression(column_scanner))
                 column_scanner.close()
         else:
             columns = None
 
         # 匹配 VALUES 类型
         if scanner.search_and_move("VALUES"):
             values = []
-            while scanner.search(ASTMark.PARENTHESIS):
+            while scanner.search(AMTMark.PARENTHESIS):
                 values.append(cls.parse_value_expression(scanner))
                 scanner.search_and_move(",")
 
-            return SQLInsertValuesStatement(
+            return ASTInsertValuesStatement(
                 with_clause=with_clause,
                 insert_type=insert_type,
                 table_name=table_name,
                 partition=partition,
-                columns=columns,
-                values=values
+                columns=tuple(columns) if columns is not None else None,
+                values=tuple(values)
             )
 
         if scanner.search("SELECT"):
-            select_statement = cls.parse_select_statement(scanner, with_clause=SQLWithClause.empty())
-            return SQLInsertSelectStatement(
+            select_statement = cls.parse_select_statement(scanner, with_clause=ASTWithClause.empty())
+            return ASTInsertSelectStatement(
                 with_clause=with_clause,
                 insert_type=insert_type,
                 table_name=table_name,
                 partition=partition,
-                columns=columns,
+                columns=tuple(columns) if columns is not None else None,
                 select_statement=select_statement
             )
 
         raise SqlParseError(f"未知的 INSERT 语句类型 {scanner}")
 
     @classmethod
     def check_set_statement(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
         """判断是否为 SET 语句"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         return scanner.search("SET")
 
     @classmethod
-    def parse_set_statement(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLSetStatement:
+    def parse_set_statement(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTSetStatement:
         """解析 SET 语句"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         scanner.match("SET")
         config_name = cls.parse_config_name_expression(scanner)
         scanner.match("=")
         config_value = cls.parse_config_value_expression(scanner)
-        return SQLSetStatement(config_name=config_name, config_value=config_value)
+        return ASTSetStatement(config_name=config_name, config_value=config_value)
 
     @classmethod
-    def parse_create_table_statement(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLCreateTableStatement:
+    def parse_create_table_statement(cls, scanner_or_string: Union[TokenScanner, str]) -> ASTCreateTableStatement:
         """解析 CREATE TABLE 语句"""
         # 解析字段、索引括号前的部分
         scanner = cls._unify_input_scanner(scanner_or_string)
         scanner.match("CREATE", "TABLE")
         if_not_exists = scanner.search_and_move("IF", "NOT", "EXISTS")
         table_name_expression = cls.parse_table_name_expression(scanner)
 
         # 解析字段和索引
-        columns: List[SQLDefineColumnExpression] = []
-        primary_key: Optional[SQLPrimaryIndexExpression] = None
-        unique_key: List[SQLUniqueIndexExpression] = []
-        key: List[SQLNormalIndexExpression] = []
-        fulltext_key: List[SQLFulltextIndexExpression] = []
-        foreign_key: List[SQLForeignKeyExpression] = []
+        columns: List[ASTDefineColumnExpression] = []
+        primary_key: Optional[ASTPrimaryIndexExpression] = None
+        unique_key: List[ASTUniqueIndexExpression] = []
+        key: List[ASTNormalIndexExpression] = []
+        fulltext_key: List[ASTFulltextIndexExpression] = []
+        foreign_key: List[ASTForeignKeyExpression] = []
         for group_scanner in scanner.pop_as_children_scanner_list_split_by(","):
             if cls.check_primary_index_expression(group_scanner):
                 primary_key = cls.parse_primary_index_expression(group_scanner)
             elif cls.check_unique_index_expression(group_scanner):
                 unique_key.append(cls.parse_unique_index_expression(group_scanner))
             elif cls.check_normal_index_expression(group_scanner):
                 key.append(cls.parse_normal_index_expression(group_scanner))
@@ -1298,68 +1362,102 @@
             elif cls.check_foreign_key_expression(group_scanner):
                 foreign_key.append(cls.parse_foreign_key_expression(group_scanner))
             else:
                 columns.append(cls.parse_define_column_expression(group_scanner))
             group_scanner.close()
 
         # 解析表属性
+        partitioned_by: List[ASTDefineColumnExpression] = []
         comment: Optional[str] = None
         engine: Optional[str] = None
         auto_increment: Optional[int] = None
         default_charset: Optional[str] = None
         collate: Optional[str] = None
         row_format: Optional[str] = None
         states_persistent: Optional[str] = None
+        row_format_serde: Optional[str] = None
+        stored_as_inputformat: Optional[str] = None
+        outputformat: Optional[str] = None
+        location: Optional[str] = None
+        tblproperties: Optional[List[Tuple[ASTConfigNameExpression, ASTConfigValueExpression]]] = []
         while not scanner.is_finish:
             if scanner.search_and_move("ENGINE"):
                 scanner.search_and_move("=")
                 engine = scanner.pop_as_source()
             elif scanner.search_and_move("AUTO_INCREMENT"):
-                scanner.match("=")
+                scanner.search_and_move("=")
                 auto_increment = int(scanner.pop_as_source())
             elif scanner.search_and_move("DEFAULT", "CHARSET"):
-                scanner.match("=")
+                scanner.search_and_move("=")
                 default_charset = scanner.pop_as_source()
             elif scanner.search_and_move("ROW_FORMAT"):
-                scanner.match("=")
+                scanner.search_and_move("=")
                 row_format = scanner.pop_as_source()
             elif scanner.search_and_move("COLLATE"):
-                scanner.match("=")
+                scanner.search_and_move("=")
                 collate = scanner.pop_as_source()
             elif scanner.search_and_move("COMMENT"):
-                scanner.match("=")
+                scanner.search_and_move("=")
                 comment = scanner.pop_as_source()
             elif scanner.search_and_move("STATS_PERSISTENT"):
-                scanner.match("=")
+                scanner.search_and_move("=")
                 states_persistent = scanner.pop_as_source()
+            elif scanner.search_and_move("PARTITIONED", "BY"):
+                for group_scanner in scanner.pop_as_children_scanner_list_split_by(","):
+                    partitioned_by.append(cls.parse_define_column_expression(group_scanner))
+                    group_scanner.close()
+            elif scanner.search_and_move("ROW", "FORMAT", "SERDE"):
+                scanner.search_and_move("=")
+                row_format_serde = scanner.pop_as_source()
+            elif scanner.search_and_move("STORED", "AS", "INPUTFORMAT"):
+                scanner.search_and_move("=")
+                stored_as_inputformat = scanner.pop_as_source()
+            elif scanner.search_and_move("OUTPUTFORMAT"):
+                scanner.search_and_move("=")
+                outputformat = scanner.pop_as_source()
+            elif scanner.search_and_move("LOCATION"):
+                scanner.search_and_move("=")
+                location = scanner.pop_as_source()
+            elif scanner.search_and_move("TBLPROPERTIES"):
+                for group_scanner in scanner.pop_as_children_scanner_list_split_by(","):
+                    config_name = cls.parse_config_name_expression(group_scanner)
+                    group_scanner.match("=")
+                    config_value = cls.parse_config_value_expression(group_scanner)
+                    tblproperties.append((config_name, config_value))
+                    group_scanner.close()
             else:
                 raise SqlParseError(f"未知的 DDL 表属性: {scanner}")
         scanner.search_and_move(";")
 
-        return SQLCreateTableStatement(
-            table_name_expression=table_name_expression,
+        return ASTCreateTableStatement(
+            table_name=table_name_expression,
             comment=comment,
             if_not_exists=if_not_exists,
-            columns=columns,
+            columns=tuple(columns),
             primary_key=primary_key,
-            unique_key=unique_key,
-            key=key,
-            fulltext_key=fulltext_key,
-            foreign_key=foreign_key,
+            unique_key=tuple(unique_key),
+            key=tuple(key),
+            fulltext_key=tuple(fulltext_key),
+            foreign_key=tuple(foreign_key),
             engine=engine,
             auto_increment=auto_increment,
             default_charset=default_charset,
             collate=collate,
             row_format=row_format,
             states_persistent=states_persistent,
-            partition_by=[]  # TODO 待支持 Hive 建表语句解析
+            partitioned_by=tuple(partitioned_by),
+            row_format_serde=row_format_serde,
+            stored_as_inputformat=stored_as_inputformat,
+            outputformat=outputformat,
+            location=location,
+            tblproperties=tuple(tblproperties)
         )
 
     @classmethod
-    def parse_statements(cls, scanner_or_string: Union[TokenScanner, str]) -> List[SQLStatement]:
+    def parse_statements(cls, scanner_or_string: Union[TokenScanner, str]) -> List[ASTStatement]:
         """解析一段 SQL 语句，返回表达式的列表"""
         scanner = cls._unify_input_scanner(scanner_or_string)
         statement_list = []
         for statement_scanner in scanner.split_by(";"):
             # 解析 SET 语句
             if cls.check_set_statement(statement_scanner):
                 statement_list.append(cls.parse_set_statement(statement_scanner))
```

### Comparing `metasequoia-sql-0.3.0/metasequoia_sql/errors.py` & `metasequoia-sql-0.4.0/metasequoia_sql/errors.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 """
 在 metasequoia_sql 中年可能抛出的异常
 """
 
-__all__ = ["SqlParseError", "AstParseError", "UnSupportDataSourceError", "ScannerError"]
+__all__ = ["SqlParseError", "AMTParseError", "UnSupportDataSourceError", "ScannerError", "AnalyzerError"]
 
 
 class SqlParseError(Exception):
     """SQL解析失败的异常"""
 
     def __init__(self, reason: str):
         self.reason = reason
 
 
-class AstParseError(SqlParseError):
-    """AST 解析失败"""
+class AMTParseError(SqlParseError):
+    """抽象词法树 AMT 解析失败"""
 
 
 class UnSupportDataSourceError(Exception):
     """数据源不支持的语法异常"""
 
     def __init__(self, reason: str):
         self.reason = reason
 
 
 class ScannerError(Exception):
     """文本扫描异常"""
+
+
+class AnalyzerError(Exception):
+    """分析器异常"""
```

### Comparing `metasequoia-sql-0.3.0/metasequoia_sql/static.py` & `metasequoia-sql-0.4.0/metasequoia_sql/static.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""将每个 Mysql 类型转换为 Hive 类型"""
+# 将每个 Mysql 类型转换为 Hive 类型  TODO 待整理所有主逻辑中未使用的静态常量
 HASHMAP_MYSQL_TO_HIVE = {
     # 串数据类型
     "CHAR": "STRING",
     "VARCHAR": "STRING",
     "ENUM": "STRING",
     "SET": "STRING",
     "TINYTEXT": "STRING",
```

### Comparing `metasequoia-sql-0.3.0/metasequoia_sql.egg-info/PKG-INFO` & `metasequoia-sql-0.4.0/metasequoia_sql.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: metasequoia-sql
-Version: 0.3.0
-Summary: SQL解析器：提供词法解析、句法解析和不同SQL类型翻译的功能
+Version: 0.4.0
+Summary: SQL解析器：提供词法解析、句法解析以及配套的分析器、插件功能
 Home-page: https://github.com/ChangxingJiang/metasequoia-sql
 Author: changxing
 Author-email: 1278729001@qq.com
 License: MIT License
 Platform: all
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sql-tree：SQL 解析器
 
 ## 安装方法
@@ -24,19 +26,19 @@
 pip install metasequoia-sql
 ```
 
 ## 使用方法
 
 ### 词法分析
 
-对 SQL 语句进行句法分析，将 SQL 语句中的每个部分拆分为一个抽象语法树节点：
+对 SQL 语句进行句法分析，将 SQL 语句中的每个部分拆分为一个抽象词法树节点（abstract morphology tree，AMT）。
 
 ### 句法分析
 
-对 SQL 语句进行语法分析，将 SQL 语句转化为对应可操作的对象（详见 demo_2）：
+对 SQL 语句进行语法分析，将 SQL 语句转化为对应可操作的抽象语法树节点（abstract syntax tree，AST）：
 
 ```python
 from metasequoia_sql import *
 
 statement = SQLParser.parse_create_table_statement("your sql")
 ```
 
@@ -60,43 +62,43 @@
 
 **SQL 解析原理**：将词法分析与句法分析分离，对所有 SQL 语句进行词法分析，然后对不同的 SQL 语句类型使用不同的句法分析方法。
 
 **不同 DataSource 的 SQL 语句转换方法**： 先从特定 DataSource 的 SQL 转化为包含所有数据库特性的 FullStatement，然后再从
 FullStatement 转化为另一个 DataSource 的 SQl。通过这样的处理，可以避免开发网状结构的转换器，而只需要开发星星转换器即可。
 
 - `analyzer`：分析器
-- `ast`：词法分析（主要使用有限状态自动机实现）
+- `lexical`：词法分析
 - `common`：遍历器工具
 - `core`：句法分析节点类
-  - `abc`：抽象类（节点中不包含解析方法）
-  - `element`：元素类节点（不会引用其他节点）
-  - `general_expression`：一般表达式节点（可能引用元素类节点和其他一般表达式节点）
+    - `abc`：抽象类（节点中不包含解析方法）
+    - `element`：元素类节点（不会引用其他节点）
+    - `general_expression`：一般表达式节点（可能引用元素类节点和其他一般表达式节点）
 - `objects`：SQL语句对象
 - `parser`：SQL语句解析器
 
 （因为在 Python 中若标记类型时，不同文件之间不同循环引用，所以需要保证所有类的引用之间为严格的拓扑关系）
 
 ### 词法分析
 
 字面值类型：[参考文档](https://deepinout.com/mysql/mysql-top-articles-mysql/1694052463_j_mysql-literals.html)
 
-- `ASTLiteralString`：字符串字面值
+- `AMTLiteralString`：字符串字面值
 
 ### 句法分析
 
 #### 节点层级
 
 单项式级别（`SQLMonomial`）：在当前层级，仅包含一个元素或两个相互依存的元素，其中不允许包含任何计算符。但是需要注意的是，函数调用虽然是单项式级别，但它可能包含一个或多个多项式级别的子节点。
 
 - `SQLFunction`：函数调用。包含参数插入语。
 - `SQLColumnType`：DDL 中的字段类型，是 `SQLFunction` 的子类。可以是类型名称或函数调用（类型的注释）。因为在其他场景下，类型名称均不允许单独使用，所以在这里额外处理。
 - `SQLVariable`：变量引用。不包含插入语。例如 `CURRENT_DATE` 等。
 - `SQLLiteral`：字面值。没有依赖的列名。
 - 计算运算符
-  - `SQLPlus`：
+    - `SQLPlus`：
 - `SQLCompareOperator`：比较运算符。
 
 - `SQLColumnName`：列名。
 - `SQLTableName`：表名。
 
 多项式级别（`SQLPolynomial`）：
 
@@ -133,14 +135,35 @@
 
 - DB2 的 `CURRENT DATE` 的语法
 
 参考文档：https://www.alibabacloud.com/help/zh/maxcompute/user-guide/insert-or-update-data-into-a-table-or-a-static-partition?spm=a2c63.p38356.0.0.637d7109wr3nC3
 
 ## 修改记录
 
+#### 0.3.0 > 0.4.0
+
+新增：
+
+- 分析器框架 & 基本分析器 & 数据血缘分析器
+- 插件框架 & MyBatis 插件
+
+优化：
+
+- 优化词法分析节点，调整模块名，调整文件结构，将节点改为不可变
+- 统一标识符引号的相关逻辑
+- 兼容建表语句的索引包含 `COMMENT`、`KEY_BLOCK_SIZE` 的逻辑
+- 兼容建表语句的外键中包含 `ON DELETE CASCADE` 的逻辑
+- 兼容 Hive 建表语句
+
+修复：
+
+- 无法解析 MySQL 建表语句索引使用 USING 子句的 Bug
+- 在 `INSERT INTO` 语句中未指定列报错的 Bug
+- 各种原因导致解析后的 SQL 与原始 SQL 不一致的 Bug
+
 #### 0.2.0 > 0.3.0
 
 新增：
 
 - 重构词法解析和语法解析以支持插件开发
 - SET 语句的解析逻辑
 - LATERAL VIEW 子句的解析逻辑
@@ -156,23 +179,26 @@
 - 支持 DB2 的 CURRENT DATE、CURRENT TIME、CURRENT TIMESTAMP 语法
 - 增加 TokenScanner 未解析完成的发现机制
 - 支持窗口函数的 ROWS 子句
 
 #### 0.1.0 > 0.2.0
 
 新增：
+
 - `INSERT` 语句解析逻辑
 - 一次性解析多条 SQL 语句
 
 优化：
+
 - 统一 `CREATE TABLE` 解析逻辑（使用 `TokenScanner`，改造节点对象，改造解析逻辑，改造 Hive 源码生成逻辑）
 - 整理 objects 的节点和 parse 中的方法，清理多余对象，优化引用路径
 - 统一 TokenScanner 使用方法
 
 修复：
+
 - `WITH` 语句解析报错的 Bug 修复
 - Hive 建表语句的类型包含参数的 Bug 修复
 
 ##### 0.1.0
 
 - 新增 SELECT 语句解析逻辑
 - Bug 修复：移除在 Hive 建表语句末尾的分号
```

### Comparing `metasequoia-sql-0.3.0/setup.py` & `metasequoia-sql-0.4.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 from setuptools import find_packages
 
 with open("README.md", "r", encoding="UTF-8") as file:
     long_description = file.read()
 
 setup(
     name="metasequoia-sql",
-    version="0.3.0",
-    description="SQL解析器：提供词法解析、句法解析和不同SQL类型翻译的功能",
+    version="0.4.0",
+    description="SQL解析器：提供词法解析、句法解析以及配套的分析器、插件功能",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="changxing",
     author_email="1278729001@qq.com",
     url="https://github.com/ChangxingJiang/metasequoia-sql",
     install_requires=[],
     license="MIT License",
     packages=[package for package in find_packages() if package.startswith("metasequoia_sql")],
     platforms=["all"],
     classifiers=[
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Natural Language :: Chinese (Simplified)",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Topic :: Software Development :: Libraries"
     ]
 )
```

