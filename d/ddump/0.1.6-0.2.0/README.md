# Comparing `tmp/ddump-0.1.6.tar.gz` & `tmp/ddump-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddump-0.1.6.tar", last modified: Sun Feb 26 14:08:40 2023, max compression
+gzip compressed data, was "ddump-0.2.0.tar", last modified: Wed May  1 11:01:47 2024, max compression
```

## Comparing `ddump-0.1.6.tar` & `ddump-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-02-26 14:08:40.031125 ddump-0.1.6/
--rw-rw-rw-   0        0        0     1083 2023-01-18 08:39:43.000000 ddump-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     2475 2023-02-26 14:08:40.031125 ddump-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2020 2023-01-18 08:39:43.000000 ddump-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-02-26 14:08:40.010841 ddump-0.1.6/ddump/
--rw-rw-rw-   0        0        0       35 2023-01-18 08:39:43.000000 ddump-0.1.6/ddump/__init__.py
--rw-rw-rw-   0        0        0       23 2023-02-26 13:50:11.000000 ddump-0.1.6/ddump/_version.py
-drwxrwxrwx   0        0        0        0 2023-02-26 14:08:40.031125 ddump-0.1.6/ddump/api/
--rw-rw-rw-   0        0        0        0 2023-01-18 08:39:43.000000 ddump-0.1.6/ddump/api/__init__.py
--rw-rw-rw-   0        0        0     5609 2023-01-18 08:39:43.000000 ddump-0.1.6/ddump/api/columns.py
--rw-rw-rw-   0        0        0     2625 2023-01-18 08:39:43.000000 ddump-0.1.6/ddump/api/common.py
--rw-rw-rw-   0        0        0     8096 2023-02-22 06:37:35.000000 ddump-0.1.6/ddump/api/dump.py
--rw-rw-rw-   0        0        0     3374 2023-02-26 13:27:43.000000 ddump-0.1.6/ddump/api/merge.py
--rw-rw-rw-   0        0        0      581 2023-01-18 08:39:43.000000 ddump-0.1.6/ddump/common.py
-drwxrwxrwx   0        0        0        0 2023-02-26 14:08:40.031125 ddump-0.1.6/ddump/db/
--rw-rw-rw-   0        0        0        0 2023-01-18 08:39:43.000000 ddump-0.1.6/ddump/db/__init__.py
--rw-rw-rw-   0        0        0     2702 2023-01-18 08:39:43.000000 ddump-0.1.6/ddump/db/common.py
--rw-rw-rw-   0        0        0    10552 2023-02-22 07:20:47.000000 ddump-0.1.6/ddump/db/dump.py
--rw-rw-rw-   0        0        0     4962 2023-02-26 13:29:27.000000 ddump-0.1.6/ddump/db/merge.py
--rw-rw-rw-   0        0        0     6584 2023-01-18 08:39:43.000000 ddump-0.1.6/ddump/db/tool.py
--rw-rw-rw-   0        0        0     2560 2023-02-26 13:52:46.000000 ddump-0.1.6/ddump/merge.py
-drwxrwxrwx   0        0        0        0 2023-02-26 14:08:40.021716 ddump-0.1.6/ddump.egg-info/
--rw-rw-rw-   0        0        0     2475 2023-02-26 14:08:39.000000 ddump-0.1.6/ddump.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-02-26 14:08:39.000000 ddump-0.1.6/ddump.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-26 14:08:39.000000 ddump-0.1.6/ddump.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-02-26 14:08:39.000000 ddump-0.1.6/ddump.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-02-26 14:08:39.000000 ddump-0.1.6/ddump.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-26 14:08:40.031125 ddump-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      973 2023-01-18 08:39:43.000000 ddump-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:01:47.479776 ddump-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-01 11:01:43.000000 ddump-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-01 11:01:47.479776 ddump-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-01 11:01:43.000000 ddump-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:01:47.479776 ddump-0.2.0/ddump/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-01 11:01:43.000000 ddump-0.2.0/ddump/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-01 11:01:43.000000 ddump-0.2.0/ddump/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:01:47.479776 ddump-0.2.0/ddump/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:01:43.000000 ddump-0.2.0/ddump/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-05-01 11:01:43.000000 ddump-0.2.0/ddump/api/columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-01 11:01:43.000000 ddump-0.2.0/ddump/api/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-05-01 11:01:43.000000 ddump-0.2.0/ddump/api/dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-01 11:01:43.000000 ddump-0.2.0/ddump/api/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-01 11:01:43.000000 ddump-0.2.0/ddump/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:01:47.479776 ddump-0.2.0/ddump/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:01:43.000000 ddump-0.2.0/ddump/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-01 11:01:43.000000 ddump-0.2.0/ddump/db/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-05-01 11:01:43.000000 ddump-0.2.0/ddump/db/dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-05-01 11:01:43.000000 ddump-0.2.0/ddump/db/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-05-01 11:01:43.000000 ddump-0.2.0/ddump/db/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-01 11:01:43.000000 ddump-0.2.0/ddump/merge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:01:47.479776 ddump-0.2.0/ddump.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-01 11:01:47.000000 ddump-0.2.0/ddump.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-01 11:01:47.000000 ddump-0.2.0/ddump.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 11:01:47.000000 ddump-0.2.0/ddump.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-01 11:01:47.000000 ddump-0.2.0/ddump.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 11:01:47.000000 ddump-0.2.0/ddump.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-01 11:01:43.000000 ddump-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 11:01:47.479776 ddump-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 11:01:43.000000 ddump-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:01:47.479776 ddump-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-01 11:01:43.000000 ddump-0.2.0/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-01 11:01:43.000000 ddump-0.2.0/tests/test_parquet.py
```

### Comparing `ddump-0.1.6/ddump/api/columns.py` & `ddump-0.2.0/ddump/api/columns.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,184 +1,184 @@
-"""
-票池的维护
-
-1. 成份股接口，按天查询，返回为list
-2. 为减少流量，查询使用折半查找
-3. 可能数据超量，前几次正常，后几次失败，所以需要每次查询后都存盘
-4. 下载的东西可能有权重信息，也需要记录下来
-
-对于权重更新频率为月，按天查询的情况，有些API返回了日期（聚宽），有些没有（wind）
-有返回日期的可以加快定位
-
-用户在下载对应数据时，最好能根据票池下载
-
-"""
-import pandas as pd
-
-from loguru import logger
-
-
-def next_query_dates(*args):
-    """下一次的查询日期列表,以及本次的合并结果
-
-    Parameters
-    ----------
-    args:
-        多个查询结果列表
-
-    Returns
-    -------
-    list
-        下次查询的列表清单。
-        - 未排除非交易日，有些接口没有数据可能有问题
-        - 日期可能重复。所以
-    pd.DataFrame
-        合并排序后的数据
-
-    """
-    df = pd.concat(args)
-    df = df[~df.index.duplicated(keep='last')]
-    df = df.sort_index().fillna(0)
-    d = (df == df.shift()).all(axis=1)
-    d = pd.DataFrame(d, columns=['is_same'])
-    d['curr'] = d.index
-    d['prev'] = d['curr'].shift()
-    if d.empty:
-        return df, d, []
-    # 1. 空数据时dt属性会失败
-    # 2. 直接除2，没有排除节假日，在部分系统中节假日可能查出来为空
-    d['half'] = pd.to_datetime((d['curr'] - (d['curr'] - d['prev']) // 2).dt.date)
-    # 昨天，部分请求中昨天是一个关键点
-    d['yestoday'] = d['curr'] - pd.Timedelta(days=1)
-    #
-    nx = d[~d['is_same']]['half'].dropna()
-    # 选出出现不同的行，但不能用于折半，因为前后肯定不同，会导致再次查询
-    # d[~d['is_same']]
-
-    # 选出出现不同的行与其上一行，可用于折半查找，因为保留了边界
-    # 这里不建议删除已经查出来的记录，因为可能事后有其他用途
-    # d['is_same2'] = d['is_same'].shift(-1, fill_value=False)
-    # d[~d['is_same']|~d['is_same2']]
-    return df, d, nx.tolist()
-
-
-def query_list_to_dataframe(func, date, symbol):
-    """将查询的列表转换成DataFrame
-
-    Parameters
-    ----------
-    func:
-        查询函数
-    symbol
-        查询参数
-    date
-        查询日期
-
-    Returns
-    -------
-    pd.DataFrame
-        日期为索引的DataFrame。查询日期与返回日期可能不同，需留意
-    list
-        推荐的下次查询日期
-
-    """
-    date = pd.to_datetime(date)
-    columns = func(symbol, date=date)
-    # 如果遇到查的是A日，返回的是B日，还没办法处理
-    df = pd.DataFrame(index=[date], columns=columns)
-    df[:] = 1.0
-    return df, []
-
-
-def query_dataframe_to_dateframe(func, date, symbol):
-    """查出来的DataFrame转成特殊的DataFrame，每个函数不同，需定制
-
-    日期使用传回的日期，可能导致折半查找进入死循环，所以将两个一起使用
-    这里要注意的是，查询日期不能超前，否则错误数据会被记录
-    """
-    date = pd.to_datetime(date)
-    df = func(symbol, date=date)
-    df['date'] = pd.to_datetime(df['date'])  # 格式处理需处理
-    df.set_index('date', append=True, inplace=True)
-    df = df['weight'].unstack(level=0)
-    # 推荐下次的结果
-    nx = df.index - pd.Timedelta(days=1)
-    # 伪造查询日期时的权重
-    df = pd.concat([df, pd.DataFrame.from_records(df.tail(1), index=[date])])
-    # 日期可能重复，保留第一个，因为最后个是伪造的
-    # 多次查询后需要合并，这时就得保留最新的一个
-    df = df[~df.index.duplicated(keep='first')]
-    return df, nx.tolist()
-
-
-def binsearch_download(query_func,
-                       load_func,
-                       save_func,
-                       *args):
-    """折半下载
-
-    Parameters
-    ----------
-    query_func
-    load_func
-    save_func
-    args
-
-    Returns
-    -------
-    pd.DataFrame
-
-    """
-
-    def difference(a, b):
-        """集合差集"""
-        return list(set(a) - set(b))
-
-    # 输入的数据
-    try:
-        df = load_func()
-    except FileNotFoundError as e:
-        df = pd.DataFrame()
-
-    # 将字符串时间转换成时间
-    args = pd.to_datetime(pd.Series(args)).tolist()
-    new_dfs = []
-    recommends = []
-
-    while True:
-        df, d, n = next_query_dates(df, *new_dfs)
-        new_dfs = []  # 用完要立即清理
-        # df 需要保存一下，否则可能出现异常丢失
-        # 如果不能保存，立即中断不用再查了
-        logger.info('开始保存，数量 {}', len(df))
-        save_func(df)
-
-        n.extend(args)
-
-        # 合并推荐的下次查询参数
-        for r in recommends:
-            # 只有在范围内的才推荐
-            if df.index[0] < r < df.index[-1]:
-                n.append(r)
-        recommends = []
-
-        n = difference(n, df.index)
-
-        # 没有新日期要查询，返回
-        if len(n) == 0:
-            break
-
-        logger.info('开始查询: {}', n)
-        try:
-
-            for i in n:
-                result, recommend = query_func(i)
-                new_dfs.append(result)
-                recommends.extend(recommend)
-        except Exception as e:
-            logger.warning(repr(e))
-
-        # 查询结果为空返回，有可能是上一步出错了，必须要跳出循环
-        if len(new_dfs) == 0:
-            break
-
-    return df
+"""
+票池的维护
+
+1. 成份股接口，按天查询，返回为list
+2. 为减少流量，查询使用折半查找
+3. 可能数据超量，前几次正常，后几次失败，所以需要每次查询后都存盘
+4. 下载的东西可能有权重信息，也需要记录下来
+
+对于权重更新频率为月，按天查询的情况，有些API返回了日期（聚宽），有些没有（wind）
+有返回日期的可以加快定位
+
+用户在下载对应数据时，最好能根据票池下载
+
+"""
+import pandas as pd
+
+from loguru import logger
+
+
+def next_query_dates(*args):
+    """下一次的查询日期列表,以及本次的合并结果
+
+    Parameters
+    ----------
+    args:
+        多个查询结果列表
+
+    Returns
+    -------
+    list
+        下次查询的列表清单。
+        - 未排除非交易日，有些接口没有数据可能有问题
+        - 日期可能重复。所以
+    pd.DataFrame
+        合并排序后的数据
+
+    """
+    df = pd.concat(args)
+    df = df[~df.index.duplicated(keep='last')]
+    df = df.sort_index().fillna(0)
+    d = (df == df.shift()).all(axis=1)
+    d = pd.DataFrame(d, columns=['is_same'])
+    d['curr'] = d.index
+    d['prev'] = d['curr'].shift()
+    if d.empty:
+        return df, d, []
+    # 1. 空数据时dt属性会失败
+    # 2. 直接除2，没有排除节假日，在部分系统中节假日可能查出来为空
+    d['half'] = pd.to_datetime((d['curr'] - (d['curr'] - d['prev']) // 2).dt.date)
+    # 昨天，部分请求中昨天是一个关键点
+    d['yestoday'] = d['curr'] - pd.Timedelta(days=1)
+    #
+    nx = d[~d['is_same']]['half'].dropna()
+    # 选出出现不同的行，但不能用于折半，因为前后肯定不同，会导致再次查询
+    # d[~d['is_same']]
+
+    # 选出出现不同的行与其上一行，可用于折半查找，因为保留了边界
+    # 这里不建议删除已经查出来的记录，因为可能事后有其他用途
+    # d['is_same2'] = d['is_same'].shift(-1, fill_value=False)
+    # d[~d['is_same']|~d['is_same2']]
+    return df, d, nx.tolist()
+
+
+def query_list_to_dataframe(func, date, symbol):
+    """将查询的列表转换成DataFrame
+
+    Parameters
+    ----------
+    func:
+        查询函数
+    symbol
+        查询参数
+    date
+        查询日期
+
+    Returns
+    -------
+    pd.DataFrame
+        日期为索引的DataFrame。查询日期与返回日期可能不同，需留意
+    list
+        推荐的下次查询日期
+
+    """
+    date = pd.to_datetime(date)
+    columns = func(symbol, date=date)
+    # 如果遇到查的是A日，返回的是B日，还没办法处理
+    df = pd.DataFrame(index=[date], columns=columns)
+    df[:] = 1.0
+    return df, []
+
+
+def query_dataframe_to_dateframe(func, date, symbol):
+    """查出来的DataFrame转成特殊的DataFrame，每个函数不同，需定制
+
+    日期使用传回的日期，可能导致折半查找进入死循环，所以将两个一起使用
+    这里要注意的是，查询日期不能超前，否则错误数据会被记录
+    """
+    date = pd.to_datetime(date)
+    df = func(symbol, date=date)
+    df['date'] = pd.to_datetime(df['date'])  # 格式处理需处理
+    df.set_index('date', append=True, inplace=True)
+    df = df['weight'].unstack(level=0)
+    # 推荐下次的结果
+    nx = df.index - pd.Timedelta(days=1)
+    # 伪造查询日期时的权重
+    df = pd.concat([df, pd.DataFrame.from_records(df.tail(1), index=[date])])
+    # 日期可能重复，保留第一个，因为最后个是伪造的
+    # 多次查询后需要合并，这时就得保留最新的一个
+    df = df[~df.index.duplicated(keep='first')]
+    return df, nx.tolist()
+
+
+def binsearch_download(query_func,
+                       load_func,
+                       save_func,
+                       *args):
+    """折半下载
+
+    Parameters
+    ----------
+    query_func
+    load_func
+    save_func
+    args
+
+    Returns
+    -------
+    pd.DataFrame
+
+    """
+
+    def difference(a, b):
+        """集合差集"""
+        return list(set(a) - set(b))
+
+    # 输入的数据
+    try:
+        df = load_func()
+    except FileNotFoundError as e:
+        df = pd.DataFrame()
+
+    # 将字符串时间转换成时间
+    args = pd.to_datetime(pd.Series(args)).tolist()
+    new_dfs = []
+    recommends = []
+
+    while True:
+        df, d, n = next_query_dates(df, *new_dfs)
+        new_dfs = []  # 用完要立即清理
+        # df 需要保存一下，否则可能出现异常丢失
+        # 如果不能保存，立即中断不用再查了
+        logger.info('开始保存，数量 {}', len(df))
+        save_func(df)
+
+        n.extend(args)
+
+        # 合并推荐的下次查询参数
+        for r in recommends:
+            # 只有在范围内的才推荐
+            if df.index[0] < r < df.index[-1]:
+                n.append(r)
+        recommends = []
+
+        n = difference(n, df.index)
+
+        # 没有新日期要查询，返回
+        if len(n) == 0:
+            break
+
+        logger.info('开始查询: {}', n)
+        try:
+
+            for i in n:
+                result, recommend = query_func(i)
+                new_dfs.append(result)
+                recommends.extend(recommend)
+        except Exception as e:
+            logger.warning(repr(e))
+
+        # 查询结果为空返回，有可能是上一步出错了，必须要跳出循环
+        if len(new_dfs) == 0:
+            break
+
+    return df
```

### Comparing `ddump-0.1.6/ddump/api/common.py` & `ddump-0.2.0/ddump/api/common.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-import pathlib
-import time
-
-import pandas as pd
-
-from ..common import START_SEP_END, FILE_SUFFIX
-
-
-def start_end_2_name(start, end):
-    """格式化start,end"""
-    import datetime
-
-    if isinstance(start, (pd.Timestamp, datetime.datetime)):
-        start = f'{start:%Y%m%dT%H%M%S}'
-    if isinstance(start, int):
-        start = f'{start:020d}'
-
-    if isinstance(end, (pd.Timestamp, datetime.datetime)):
-        end = f'{end:%Y%m%dT%H%M%S}'
-    if isinstance(end, int):
-        end = f'{end:020d}'
-
-    return f'{start}{START_SEP_END}{end}'
-
-
-def files_to_dataframe(path, suffix=FILE_SUFFIX):
-    """目录中文件转DataFrame
-
-    文件名有格式要求，用分隔符分成前后两个时间。时间为左闭右闭关系。
-
-    Parameters
-    ----------
-    path: pathlib.Path
-    suffix: str
-        后缀
-
-    Returns
-    -------
-    pd.DataFrame
-
-    """
-    files = list(path.glob(f'*{suffix}'))
-    df = pd.DataFrame([f.name.split('.')[0].split(START_SEP_END) for f in files], columns=['start', 'end'])
-    # 结束时间
-    df['end_s'] = df['end'].apply(lambda x: pd.to_datetime(x).timestamp())
-    df['start'] = pd.to_datetime(df['start'])
-    df['end'] = pd.to_datetime(df['end'])
-    df['path'] = files
-    # 文件修改时间
-    df['st_mtime'] = [x.stat().st_mtime for x in files]
-    # 当前时间，需要立即使用，之后再用就不准了
-    df['now'] = time.time()
-    return df
-
-
-def timeout_mtime(path, timeout):
-    """检查文件超时"""
-    return time.time() - pathlib.Path(path).stat().st_mtime > timeout
-
-
-def filter_range_in_dataframe(df, start, end, file_timeout, data_timeout):
-    """检查日期是否在某一个文件中
-
-    日期可以跨多个文件
-
-    单日期只是两个日期的特例
-
-    Parameters
-    ----------
-    df
-    start
-    end
-    file_timeout
-    data_timeout
-
-    Returns
-    -------
-    bool
-
-    """
-    if df is None:
-        return pd.DataFrame()
-    # 找到多条记录
-    df = df[(df['start'] <= end) & (start <= df['end'])]
-    # 太近了表示存在
-    # 太远了，也表示存在
-    df = df[(df['now'] - df['st_mtime'] < file_timeout) | (df['now'] - df['end_s'] > data_timeout)]
-    return df
-
-
-def get_last_file(path, suffix):
-    """通过最新文件的文件名得到关键参数
-
-    Parameters
-    ----------
-    path
-    suffix
-
-    Returns
-    -------
-    dt
-    id
-
-    """
-    path = pathlib.Path(path)
-    files = list(path.glob(f'*{suffix}'))
-    if len(files) == 0:
-        return None
-    return files[-1]
+import pathlib
+import time
+
+import pandas as pd
+
+from ..common import START_SEP_END, FILE_SUFFIX
+
+
+def start_end_2_name(start, end):
+    """格式化start,end"""
+    import datetime
+
+    if isinstance(start, (pd.Timestamp, datetime.datetime)):
+        start = f'{start:%Y%m%dT%H%M%S}'
+    if isinstance(start, int):
+        start = f'{start:020d}'
+
+    if isinstance(end, (pd.Timestamp, datetime.datetime)):
+        end = f'{end:%Y%m%dT%H%M%S}'
+    if isinstance(end, int):
+        end = f'{end:020d}'
+
+    return f'{start}{START_SEP_END}{end}'
+
+
+def files_to_dataframe(path, suffix=FILE_SUFFIX):
+    """目录中文件转DataFrame
+
+    文件名有格式要求，用分隔符分成前后两个时间。时间为左闭右闭关系。
+
+    Parameters
+    ----------
+    path: pathlib.Path
+    suffix: str
+        后缀
+
+    Returns
+    -------
+    pd.DataFrame
+
+    """
+    files = list(path.glob(f'*{suffix}'))
+    df = pd.DataFrame([f.name.split('.')[0].split(START_SEP_END) for f in files], columns=['start', 'end'])
+    # 结束时间
+    df['end_s'] = df['end'].apply(lambda x: pd.to_datetime(x).timestamp())
+    df['start'] = pd.to_datetime(df['start'])
+    df['end'] = pd.to_datetime(df['end'])
+    df['path'] = files
+    # 文件修改时间
+    df['st_mtime'] = [x.stat().st_mtime for x in files]
+    # 当前时间，需要立即使用，之后再用就不准了
+    df['now'] = time.time()
+    return df
+
+
+def timeout_mtime(path, timeout):
+    """检查文件超时"""
+    return time.time() - pathlib.Path(path).stat().st_mtime > timeout
+
+
+def filter_range_in_dataframe(df, start, end, file_timeout, data_timeout):
+    """检查日期是否在某一个文件中
+
+    日期可以跨多个文件
+
+    单日期只是两个日期的特例
+
+    Parameters
+    ----------
+    df
+    start
+    end
+    file_timeout
+    data_timeout
+
+    Returns
+    -------
+    bool
+
+    """
+    if df is None:
+        return pd.DataFrame()
+    # 找到多条记录
+    df = df[(df['start'] <= end) & (start <= df['end'])]
+    # 太近了表示存在
+    # 太远了，也表示存在
+    df = df[(df['now'] - df['st_mtime'] < file_timeout) | (df['now'] - df['end_s'] > data_timeout)]
+    return df
+
+
+def get_last_file(path, suffix):
+    """通过最新文件的文件名得到关键参数
+
+    Parameters
+    ----------
+    path
+    suffix
+
+    Returns
+    -------
+    dt
+    id
+
+    """
+    path = pathlib.Path(path)
+    files = list(path.glob(f'*{suffix}'))
+    if len(files) == 0:
+        return None
+    return files[-1]
```

### Comparing `ddump-0.1.6/ddump/api/merge.py` & `ddump-0.2.0/ddump/api/merge.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,94 +1,83 @@
-"""
-合并文件
-1. 一组文件，第一个取前部分，最后一个取后部分，然后合并多个文件
-2. 以其它方式命名的文件名，合并的方式需要另行处理
-
-"""
-import pandas as pd
-
-from .common import start_end_2_name
-from ..common import FILE_SUFFIX, START_SEP_END
-
-
-def path_groupby_date(input_path, output_path,
-                      reserve=2, suffix=FILE_SUFFIX):
-    """根据文件名上所示时间进行分组
-
-    文件名由 开始时间+结束时间组成
-
-    Parameters
-    ----------
-    input_path: pathlib.Path
-        输入目录
-    output_path: pathlib.Path
-        输出目录
-    reserve: int
-        预留文件数。最后几个文件不动，可能会被修改
-    suffix
-
-    Returns
-    -------
-    dict
-
-    """
-    if output_path is None:
-        output_path = input_path
-
-    files_tail = []
-    files = list(input_path.glob(f'*{suffix}'))
-    if reserve > 0:
-        files_tail = files[-reserve:]
-        files = files[:-reserve]
-
-    # 提取文件名中的时间
-    df = pd.DataFrame([f.name.split('.')[0].split(START_SEP_END) for f in files], columns=['start', 'end'])
-    df['path'] = files
-    df['key'] = pd.to_datetime(df['start'])
-    df['key2'] = df['key']
-    df.index = df['key'].copy()
-    df.index.name = 'date'  # 防止无法groupby
-
-    from dateutil.relativedelta import relativedelta, MO, SU
-    from datetime import datetime, timedelta
-
-    # 周week。少用，因为跨月跨年了，如果周重新切分成月年，会出错
-    df['1W_1'] = df['key'].apply(lambda x: x.date() + relativedelta(weekday=MO(-1)))
-    df['1W_2'] = df['key'].apply(lambda x: x.date() + relativedelta(weekday=SU(0)))
-
-    # 月month
-    df['1M_1'] = df['key'].apply(lambda x: x.date() + relativedelta(day=1))
-    df['1M_2'] = df['key'].apply(lambda x: x.date() + relativedelta(day=31))
-    # 季quarter
-    df['1Q_1'] = df['key'].apply(lambda x: x.date() + relativedelta(month=((x.month - 1) // 3) * 3 + 1, day=1))
-    df['1Q_2'] = df['key'].apply(lambda x: x.date() + relativedelta(month=((x.month - 1) // 3 + 1) * 3, day=31))
-    # 年
-    df['1Y_1'] = df['key'].apply(lambda x: x.date() + relativedelta(month=1, day=1))
-    df['1Y_2'] = df['key'].apply(lambda x: x.date() + relativedelta(month=12, day=31))
-    # 十年decade
-    df['10Y_1'] = df['key'].apply(lambda x: x.date() + relativedelta(year=x.year // 10 * 10, month=1, day=1))
-    df['10Y_2'] = df['key'].apply(lambda x: x.date() + relativedelta(year=x.year // 10 * 10 + 9, month=12, day=31))
-
-    df['1M_1'] = pd.to_datetime(df['1M_1'])
-    df['1Y_1'] = pd.to_datetime(df['1Y_1'])
-
-    # 最近的两个月不动，两个月前的都按月合并
-    t = f'{datetime.now() - timedelta(days=31 * 2):%Y-%m}'
-    df['key'] = df.loc[:t, '1M_1']
-    t = f'{datetime.now() - timedelta(days=365 * 1):%Y}'
-    df['key'] = df.loc[:t, '1Y_1']
-    df['key'].fillna(df['key2'], inplace=True)
-
-    # 按key进行分组
-    fss = {}
-    for k, v in df.groupby(by='key'):
-        name = start_end_2_name(v['start'][0], v['end'][-1])
-        fss[output_path / f"{name}{FILE_SUFFIX}"] = v['path'].tolist()
-
-    # 最近的两个文件不动
-    fs = []
-    for f in files_tail:
-        fs.append(f)
-        fss[output_path / f.name] = fs
-        fs = []
-
-    return fss
+"""
+合并文件
+1. 一组文件，第一个取前部分，最后一个取后部分，然后合并多个文件
+2. 以其它方式命名的文件名，合并的方式需要另行处理
+
+"""
+import pandas as pd
+
+from .common import start_end_2_name
+from ..common import FILE_SUFFIX, START_SEP_END
+
+
+def path_groupby_date(input_path, output_path, suffix=FILE_SUFFIX):
+    """根据文件名上所示时间进行分组
+
+    文件名由 开始时间+结束时间组成
+
+    Parameters
+    ----------
+    input_path: pathlib.Path
+        输入目录
+    output_path: pathlib.Path
+        输出目录
+    suffix
+
+    Returns
+    -------
+    dict
+
+    """
+    if output_path is None:
+        output_path = input_path
+
+    files = list(input_path.glob(f'*{suffix}'))
+
+    # 提取文件名中的时间
+    df = pd.DataFrame([f.name.split('.')[0].split(START_SEP_END) for f in files], columns=['start', 'end'])
+    df['path'] = files
+    df['key'] = pd.to_datetime(df['start'])
+    df['key2'] = df['key']
+    df.index = df['key'].copy()
+    df.index.name = 'date'  # 防止无法groupby
+
+    from dateutil.relativedelta import relativedelta, MO, SU
+    from datetime import datetime, timedelta
+
+    # 周week。少用，因为跨月跨年了，如果周重新切分成月年，会出错
+    df['1W_1'] = df['key'].apply(lambda x: x.date() + relativedelta(weekday=MO(-1)))
+    df['1W_2'] = df['key'].apply(lambda x: x.date() + relativedelta(weekday=SU(0)))
+
+    # 月month
+    df['1M_1'] = df['key'].apply(lambda x: x.date() + relativedelta(day=1))
+    df['1M_2'] = df['key'].apply(lambda x: x.date() + relativedelta(day=31))
+    # 季quarter
+    df['1Q_1'] = df['key'].apply(lambda x: x.date() + relativedelta(month=((x.month - 1) // 3) * 3 + 1, day=1))
+    df['1Q_2'] = df['key'].apply(lambda x: x.date() + relativedelta(month=((x.month - 1) // 3 + 1) * 3, day=31))
+    # 年
+    df['1Y_1'] = df['key'].apply(lambda x: x.date() + relativedelta(month=1, day=1))
+    df['1Y_2'] = df['key'].apply(lambda x: x.date() + relativedelta(month=12, day=31))
+    # 十年decade
+    df['10Y_1'] = df['key'].apply(lambda x: x.date() + relativedelta(year=x.year // 10 * 10, month=1, day=1))
+    df['10Y_2'] = df['key'].apply(lambda x: x.date() + relativedelta(year=x.year // 10 * 10 + 9, month=12, day=31))
+
+    df['1M_1'] = pd.to_datetime(df['1M_1'])
+    df['1Y_1'] = pd.to_datetime(df['1Y_1'])
+
+    # 最近的两个月不动，两个月前的都按月合并
+    t = f'{datetime.now() - timedelta(days=31 * 2):%Y-%m}'
+    df['key'] = df.loc[:t, '1M_1']
+    t = f'{datetime.now() - timedelta(days=365 * 1):%Y}'
+    df['key'] = df.loc[:t, '1Y_1']
+    df['key'].fillna(df['key2'], inplace=True)
+
+    # 按key进行分组
+    fss = []
+    for k, v in df.groupby(by='key'):
+        s, e = v['start'][0], v['end'][-1]
+        name = start_end_2_name(s, e)
+        to_ = output_path / f"{name}{FILE_SUFFIX}"
+        from_ = v['path'].tolist()
+        fss.append({'to': to_, 'from': from_})
+
+    return fss
```

### Comparing `ddump-0.1.6/ddump/common.py` & `ddump-0.2.0/ddump/common.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-# @Author     :wukan
-# @License    :(C) Copyright 2022
-# @Date       :2022-04-11
-
-FILE_SUFFIX = '.parquet'  # 文件后缀名
-TEMP_SUFFIX = '.tmp'  # 临时文件后缀名
-KEY_SEP_ID = '__'  # 文件名分隔符。注意:KEY中不要出现__否则无法区分。KEY中出现双下划线的概率比单下载线的概率低很多
-START_SEP_END = '__'  # 文件名分隔符。用于区分开始时间与结束时间。
-OLD_DATA_DAY = 86400 * 10  # N天前的老数据认为不再更新，不需要重复下载。最长放9天
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+# @Author     :wukan
+# @License    :(C) Copyright 2022
+# @Date       :2022-04-11
+
+FILE_SUFFIX = '.parquet'  # 文件后缀名
+TEMP_SUFFIX = '.tmp'  # 临时文件后缀名
+KEY_SEP_ID = '__'  # 文件名分隔符。注意:KEY中不要出现__否则无法区分。KEY中出现双下划线的概率比单下载线的概率低很多
+START_SEP_END = '__'  # 文件名分隔符。用于区分开始时间与结束时间。
+OLD_DATA_DAY = 86400 * 10  # N天前的老数据认为不再更新，不需要重复下载。最长放9天
```

### Comparing `ddump-0.1.6/ddump/db/dump.py` & `ddump-0.2.0/ddump/db/dump.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,304 +1,304 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-# @Author     :wukan
-# @License    :(C) Copyright 2022
-# @Date       :2022-04-10
-
-"""
-如何将整张表下载过来？
-
-1. 表可能很大，无法一次性下载，需要分页下载，例如100GB
-2. API上有限制，下载数据有量限制，例如一次只能下1000条
-3. 表的字段有限。 有ID和update_time已经是最佳方案
-3. update_time大量相同，有可能全表值都完全一样，导致每次都从头下载
-
-References
-----------
-https://blog.csdn.net/oro99/article/details/120041289
-
-```
-where (update_time='last_..' and id>'...' ) or update_time>'last_...'  order by update_time asc, id asc
-```
-
-"""
-import pathlib
-
-import pandas as pd
-from loguru import logger
-from sqlalchemy import or_, and_
-
-from .common import last_key_id, key_id_2_name, get_last_file_key_id, get_files_count
-from ..common import FILE_SUFFIX, TEMP_SUFFIX
-from .merge import path_groupby_size, path_groupby_date
-from ..merge import merge_files_dict
-
-
-def dump_table(db, tbl, q=None,
-               str_key='UPDATE_TIME', str_id='ID', str_dt='UPDATE_TIME',
-               last_key=0, last_id=0, last_dt=0,
-               limit=5000,
-               page=5,
-               eq_none=False):
-    """分页下载整表
-
-    Parameters
-    ----------
-    db: DbTool
-        自研数据库工具
-    tbl: str or Table
-        数据库表
-    q: sqlalchemy.orm.query.Query
-        查询条件
-    str_key: str
-        索引字段名
-    str_id: str
-        唯一ID字段名
-    str_dt: str
-        更新时间字段
-    last_key:
-        上次最新字段
-    last_id: int
-        上次最新ID
-    last_dt: datetime
-        上次最新时间
-    limit: int
-        每页数量
-    page: int
-        分页几张
-    eq_none: bool
-        是否查条件为None
-
-    Returns
-    -------
-    df
-    last_key
-    last_id
-
-    """
-    # 类型提前调整
-    if isinstance(tbl, str):
-        tbl = getattr(db, tbl)
-    c_key = getattr(tbl, str_key)
-    c_id = getattr(tbl, str_id)
-    c_dt = getattr(tbl, str_dt)
-
-    # 没有设置查询条件就全查
-    if q is None:
-        q = db.query(tbl)
-
-    dfs = []
-    # 底层做几次增量查询，查看效果如何
-    for i in range(page):
-        if eq_none:
-            # 早期，部分数据可能为空，所以直接全查
-            _q = q.filter(c_key == None, c_id > last_id).order_by(c_id).limit(limit)
-        else:
-            # 先按时间排序，再按ID排序，还要过滤当前时间
-            _q = q.filter(
-                or_(
-                    and_(c_key == last_key, c_id > last_id),
-                    c_key > last_key
-                )
-            ).filter(
-                c_dt < last_dt
-            ).order_by(c_key, c_id).limit(limit)
-        logger.info('过滤条件 key:{} id:{} dt:{}', last_key, last_id, last_dt)
-        db.check_limit = -1
-        df = db.run_query(_q)
-        if df.empty:
-            break
-        dfs.append(df)
-        # 更新关键参数
-        last_key, last_id = last_key_id(df, str_key, str_id)
-        if len(df) < limit:
-            # 已经掏空
-            break
-
-    # 将多次查询的结果合并
-    if len(dfs) > 0:
-        df = pd.concat(dfs, ignore_index=True)
-
-    return df, last_key, last_id
-
-
-def continue_download(db, tbl_name, path,
-                      str_key='UPDATE_TIME', str_id='ID', str_dt='UPDATE_TIME',
-                      last_dt=None,
-                      limit=5000,
-                      eq_none=False):
-    """增量下载, 从最后一个文件之后进行下载
-
-    依据 更新时间+唯一ID
-
-    Parameters
-    ----------
-    db: DbTool
-        数据库工具
-    tbl_name: str
-        表名
-    path: pathlib.Path
-        保存路径
-    str_key: str
-        索引字段名
-    str_id: str
-        唯一ID字段名,同索引时实现增量查询
-    str_dt: str
-        更新时间字段名
-    last_dt: datetime like
-        开启全量下载的时间，同时也是全量下载的截止时间
-    limit: int
-        每次查询的数量限制
-    eq_none: bool
-        更新时间是否为None
-
-    Returns
-    -------
-    bool
-        是否还有后续
-
-    """
-    logger.info('下载 {}', tbl_name)
-    page = 5  # 页数
-
-    # 读取目录中 数据内的 两个关键参数
-    last_key, last_id = get_last_file_key_id(path, FILE_SUFFIX)
-
-    # 查数据库，得到最新的两个参数
-    df, last_key, last_id = dump_table(db, tbl_name, q=None,
-                                       str_key=str_key, str_id=str_id, str_dt=str_dt,
-                                       last_key=last_key, last_id=last_id, last_dt=last_dt,
-                                       limit=limit,
-                                       page=page,
-                                       eq_none=eq_none)
-    if df.empty:
-        logger.info('新结果为空，下载 {} 完成', tbl_name)
-        return False
-
-    path.mkdir(parents=True, exist_ok=True)
-
-    file_path = path / f'{key_id_2_name(last_key, last_id)}{FILE_SUFFIX}'
-    temp_path = path / f'{key_id_2_name(last_key, last_id)}{TEMP_SUFFIX}'
-
-    logger.info('保存 {}条 {} {}', len(df), tbl_name, temp_path)
-    # 写入要时间，所以先放临时文件，然后再改名
-    df.to_parquet(temp_path, compression='zstd')
-    temp_path.rename(file_path)
-    if len(df) < limit * page:
-        # 下载完成
-        return False
-    return True
-
-
-def continue_download3(db, tbl_name,
-                       path,
-                       str_key1='END_DATE', str_id1='ID', str_dt1='UPDATE_TIME',
-                       str_key2='UPDATE_TIME', str_id2='ID', str_dt2='UPDATE_TIME',
-                       limit=5000,
-                       merge=True):
-    """3个文件夹自动全量增量下载
-
-    文件夹0: 更新时间为空
-    文件夹1: 带索引的快速大数据下载
-    文件夹2: 增量下载
-
-    Parameters
-    ----------
-    db
-    tbl_name
-    path
-    str_key1, str_id1, str_dt1
-        全量查询时的字段
-    str_key2, str_id2, str_dt2
-        增量查询时的字段
-    limit: int
-        数据查询limit参数，一次只查多少行。全量下载数据量过大，只能分批次下载
-    merge: bool
-        是否合并多个文件
-
-    """
-    from datetime import datetime
-
-    path0 = path / f'{tbl_name}__0'  # 更新时间为None数据
-    path1 = path / f'{tbl_name}__1'  # 全量下载数据
-    path2 = path / f'{tbl_name}__2'  # 增量下载数据
-
-    count0 = get_files_count(path0, FILE_SUFFIX)
-    count1 = get_files_count(path1, FILE_SUFFIX)
-    count2 = get_files_count(path2, FILE_SUFFIX)
-    logger.info('根文件夹:{}/{}_[012], 文件数量:{}/{}/{}', path, tbl_name, count0, count1, count2)
-
-    if count2 == 0:
-        # 文件夹2为空，表示全新。需要全量下载
-        if count1 == 0:
-            # 文件夹1为空，表示需要先下载 更新时间为空的部分
-            last_dt, last_id = get_last_file_key_id(path0, FILE_SUFFIX)
-            logger.info('{} 开始 {}==None 部分下载', tbl_name, str_dt2)
-            while continue_download(db, tbl_name, path0,
-                                    str_key=str_key2, str_id=str_id2, str_dt=str_dt2, last_dt=last_dt,
-                                    limit=limit, eq_none=True):
-                pass
-
-        # 第一次写入文件，表示开始启动下载的时间
-        # 如果文件夹1中已经有一部分数据了，已经下载的部分将没有机会更新了，这里需要注意
-        path2.mkdir(parents=True, exist_ok=True)
-
-        now = datetime.now()
-        file_path = path2 / f'{key_id_2_name(now, 0)}{FILE_SUFFIX}'
-        pd.DataFrame().to_parquet(file_path)
-
-        logger.info('{} 全量 开始下载', tbl_name)
-        while continue_download(db, tbl_name, path1,
-                                str_key=str_key1, str_id=str_id1, str_dt=str_dt1, last_dt=now,
-                                limit=limit, eq_none=False):
-            pass
-
-    count2 = get_files_count(path2, FILE_SUFFIX)
-    if count2 == 1:
-        # 文件夹2中只有一个文件，表示是文件夹1中还没下完，从文件名提取时间后继续下载
-        last_dt, last_id = get_last_file_key_id(path2, FILE_SUFFIX)
-        logger.info('{} 全量 继续下载', tbl_name)
-        while continue_download(db, tbl_name, path1,
-                                str_key=str_key1, str_id=str_id1, str_dt=str_dt1, last_dt=last_dt,
-                                limit=limit, eq_none=False):
-            pass
-
-        # 第二次写入文件，表示已经下载完成，时间接着上次，编号+1，这样才会继续
-        file_path = path2 / f'{key_id_2_name(last_dt, 1)}{FILE_SUFFIX}'
-        pd.DataFrame().to_parquet(file_path)
-    count2 = get_files_count(path2, FILE_SUFFIX)
-    if count2 >= 2:
-        now = datetime.now()
-        logger.info('{} 增量 继续下载', tbl_name)
-        while continue_download(db, tbl_name, path2,
-                                str_key=str_key2, str_id=str_id2, last_dt=now,
-                                limit=limit, eq_none=False):
-            pass
-
-    if merge:
-        # 第一次合并压缩
-        merge3(path0, path1, path2)
-        # 第一次合并压缩，可能还满足合并条件，所以做第二次，防止下次又合并
-        merge3(path0, path1, path2)
-
-
-def merge3(path0, path1, path2):
-    """三路径合并文件夹操作
-
-    Parameters
-    ----------
-    path0: pathlib.Path
-        更新时间为空的文件夹
-    path1: pathlib.Path
-        全量下载文件夹
-    path2: pathlib.Path
-        增量更新文件夹
-
-    """
-    # 合并历史数据，方便复制
-    files = path_groupby_size(path0, path0, per_size=128 * 1024 * 1024, reserve=0)
-    merge_files_dict(files, ignore_index=True, delete_src=True)
-    files = path_groupby_size(path1, path1, per_size=128 * 1024 * 1024, reserve=0)
-    merge_files_dict(files, ignore_index=True, delete_src=True)
-    # 每日更新部分，不能老合并，因为修改太多，网络传输量会过大，改成两个月前的都合成一个月，最近两个月的不动
-    files = path_groupby_date(path2, path2, reserve=2)
-    merge_files_dict(files, ignore_index=True, delete_src=True)
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+# @Author     :wukan
+# @License    :(C) Copyright 2022
+# @Date       :2022-04-10
+
+"""
+如何将整张表下载过来？
+
+1. 表可能很大，无法一次性下载，需要分页下载，例如100GB
+2. API上有限制，下载数据有量限制，例如一次只能下1000条
+3. 表的字段有限。 有ID和update_time已经是最佳方案
+3. update_time大量相同，有可能全表值都完全一样，导致每次都从头下载
+
+References
+----------
+https://blog.csdn.net/oro99/article/details/120041289
+
+```
+where (update_time='last_..' and id>'...' ) or update_time>'last_...'  order by update_time asc, id asc
+```
+
+"""
+import pathlib
+
+import pandas as pd
+from loguru import logger
+from sqlalchemy import or_, and_
+
+from .common import last_key_id, key_id_2_name, get_last_file_key_id, get_files_count
+from ..common import FILE_SUFFIX, TEMP_SUFFIX
+from .merge import path_groupby_size, path_groupby_date
+from ..merge import merge_files_dict
+
+
+def dump_table(db, tbl, q=None,
+               str_key='UPDATE_TIME', str_id='ID', str_dt='UPDATE_TIME',
+               last_key=0, last_id=0, last_dt=0,
+               limit=5000,
+               page=5,
+               eq_none=False):
+    """分页下载整表
+
+    Parameters
+    ----------
+    db: DbTool
+        自研数据库工具
+    tbl: str or Table
+        数据库表
+    q: sqlalchemy.orm.query.Query
+        查询条件
+    str_key: str
+        索引字段名
+    str_id: str
+        唯一ID字段名
+    str_dt: str
+        更新时间字段
+    last_key:
+        上次最新字段
+    last_id: int
+        上次最新ID
+    last_dt: datetime
+        上次最新时间
+    limit: int
+        每页数量
+    page: int
+        分页几张
+    eq_none: bool
+        是否查条件为None
+
+    Returns
+    -------
+    df
+    last_key
+    last_id
+
+    """
+    # 类型提前调整
+    if isinstance(tbl, str):
+        tbl = getattr(db, tbl)
+    c_key = getattr(tbl, str_key)
+    c_id = getattr(tbl, str_id)
+    c_dt = getattr(tbl, str_dt)
+
+    # 没有设置查询条件就全查
+    if q is None:
+        q = db.query(tbl)
+
+    dfs = []
+    # 底层做几次增量查询，查看效果如何
+    for i in range(page):
+        if eq_none:
+            # 早期，部分数据可能为空，所以直接全查
+            _q = q.filter(c_key == None, c_id > last_id).order_by(c_id).limit(limit)
+        else:
+            # 先按时间排序，再按ID排序，还要过滤当前时间
+            _q = q.filter(
+                or_(
+                    and_(c_key == last_key, c_id > last_id),
+                    c_key > last_key
+                )
+            ).filter(
+                c_dt < last_dt
+            ).order_by(c_key, c_id).limit(limit)
+        logger.info('过滤条件 key:{} id:{} dt:{}', last_key, last_id, last_dt)
+        db.check_limit = -1
+        df = db.run_query(_q)
+        if df.empty:
+            break
+        dfs.append(df)
+        # 更新关键参数
+        last_key, last_id = last_key_id(df, str_key, str_id)
+        if len(df) < limit:
+            # 已经掏空
+            break
+
+    # 将多次查询的结果合并
+    if len(dfs) > 0:
+        df = pd.concat(dfs, ignore_index=True)
+
+    return df, last_key, last_id
+
+
+def continue_download(db, tbl_name, path,
+                      str_key='UPDATE_TIME', str_id='ID', str_dt='UPDATE_TIME',
+                      last_dt=None,
+                      limit=5000,
+                      eq_none=False):
+    """增量下载, 从最后一个文件之后进行下载
+
+    依据 更新时间+唯一ID
+
+    Parameters
+    ----------
+    db: DbTool
+        数据库工具
+    tbl_name: str
+        表名
+    path: pathlib.Path
+        保存路径
+    str_key: str
+        索引字段名
+    str_id: str
+        唯一ID字段名,同索引时实现增量查询
+    str_dt: str
+        更新时间字段名
+    last_dt: datetime like
+        开启全量下载的时间，同时也是全量下载的截止时间
+    limit: int
+        每次查询的数量限制
+    eq_none: bool
+        更新时间是否为None
+
+    Returns
+    -------
+    bool
+        是否还有后续
+
+    """
+    logger.info('下载 {}', tbl_name)
+    page = 5  # 页数
+
+    # 读取目录中 数据内的 两个关键参数
+    last_key, last_id = get_last_file_key_id(path, FILE_SUFFIX)
+
+    # 查数据库，得到最新的两个参数
+    df, last_key, last_id = dump_table(db, tbl_name, q=None,
+                                       str_key=str_key, str_id=str_id, str_dt=str_dt,
+                                       last_key=last_key, last_id=last_id, last_dt=last_dt,
+                                       limit=limit,
+                                       page=page,
+                                       eq_none=eq_none)
+    if df.empty:
+        logger.info('新结果为空，下载 {} 完成', tbl_name)
+        return False
+
+    path.mkdir(parents=True, exist_ok=True)
+
+    file_path = path / f'{key_id_2_name(last_key, last_id)}{FILE_SUFFIX}'
+    temp_path = path / f'{key_id_2_name(last_key, last_id)}{TEMP_SUFFIX}'
+
+    logger.info('保存 {}条 {} {}', len(df), tbl_name, temp_path)
+    # 写入要时间，所以先放临时文件，然后再改名
+    df.to_parquet(temp_path, compression='zstd')
+    temp_path.rename(file_path)
+    if len(df) < limit * page:
+        # 下载完成
+        return False
+    return True
+
+
+def continue_download3(db, tbl_name,
+                       path,
+                       str_key1='END_DATE', str_id1='ID', str_dt1='UPDATE_TIME',
+                       str_key2='UPDATE_TIME', str_id2='ID', str_dt2='UPDATE_TIME',
+                       limit=5000,
+                       merge=True):
+    """3个文件夹自动全量增量下载
+
+    文件夹0: 更新时间为空
+    文件夹1: 带索引的快速大数据下载
+    文件夹2: 增量下载
+
+    Parameters
+    ----------
+    db
+    tbl_name
+    path
+    str_key1, str_id1, str_dt1
+        全量查询时的字段
+    str_key2, str_id2, str_dt2
+        增量查询时的字段
+    limit: int
+        数据查询limit参数，一次只查多少行。全量下载数据量过大，只能分批次下载
+    merge: bool
+        是否合并多个文件
+
+    """
+    from datetime import datetime
+
+    path0 = path / f'{tbl_name}__0'  # 更新时间为None数据
+    path1 = path / f'{tbl_name}__1'  # 全量下载数据
+    path2 = path / f'{tbl_name}__2'  # 增量下载数据
+
+    count0 = get_files_count(path0, FILE_SUFFIX)
+    count1 = get_files_count(path1, FILE_SUFFIX)
+    count2 = get_files_count(path2, FILE_SUFFIX)
+    logger.info('根文件夹:{}/{}_[012], 文件数量:{}/{}/{}', path, tbl_name, count0, count1, count2)
+
+    if count2 == 0:
+        # 文件夹2为空，表示全新。需要全量下载
+        if count1 == 0:
+            # 文件夹1为空，表示需要先下载 更新时间为空的部分
+            last_dt, last_id = get_last_file_key_id(path0, FILE_SUFFIX)
+            logger.info('{} 开始 {}==None 部分下载', tbl_name, str_dt2)
+            while continue_download(db, tbl_name, path0,
+                                    str_key=str_key2, str_id=str_id2, str_dt=str_dt2, last_dt=last_dt,
+                                    limit=limit, eq_none=True):
+                pass
+
+        # 第一次写入文件，表示开始启动下载的时间
+        # 如果文件夹1中已经有一部分数据了，已经下载的部分将没有机会更新了，这里需要注意
+        path2.mkdir(parents=True, exist_ok=True)
+
+        now = datetime.now()
+        file_path = path2 / f'{key_id_2_name(now, 0)}{FILE_SUFFIX}'
+        pd.DataFrame().to_parquet(file_path)
+
+        logger.info('{} 全量 开始下载', tbl_name)
+        while continue_download(db, tbl_name, path1,
+                                str_key=str_key1, str_id=str_id1, str_dt=str_dt1, last_dt=now,
+                                limit=limit, eq_none=False):
+            pass
+
+    count2 = get_files_count(path2, FILE_SUFFIX)
+    if count2 == 1:
+        # 文件夹2中只有一个文件，表示是文件夹1中还没下完，从文件名提取时间后继续下载
+        last_dt, last_id = get_last_file_key_id(path2, FILE_SUFFIX)
+        logger.info('{} 全量 继续下载', tbl_name)
+        while continue_download(db, tbl_name, path1,
+                                str_key=str_key1, str_id=str_id1, str_dt=str_dt1, last_dt=last_dt,
+                                limit=limit, eq_none=False):
+            pass
+
+        # 第二次写入文件，表示已经下载完成，时间接着上次，编号+1，这样才会继续
+        file_path = path2 / f'{key_id_2_name(last_dt, 1)}{FILE_SUFFIX}'
+        pd.DataFrame().to_parquet(file_path)
+    count2 = get_files_count(path2, FILE_SUFFIX)
+    if count2 >= 2:
+        now = datetime.now()
+        logger.info('{} 增量 继续下载', tbl_name)
+        while continue_download(db, tbl_name, path2,
+                                str_key=str_key2, str_id=str_id2, last_dt=now,
+                                limit=limit, eq_none=False):
+            pass
+
+    if merge:
+        # 第一次合并压缩
+        merge3(path0, path1, path2)
+        # 第一次合并压缩，可能还满足合并条件，所以做第二次，防止下次又合并
+        merge3(path0, path1, path2)
+
+
+def merge3(path0, path1, path2):
+    """三路径合并文件夹操作
+
+    Parameters
+    ----------
+    path0: pathlib.Path
+        更新时间为空的文件夹
+    path1: pathlib.Path
+        全量下载文件夹
+    path2: pathlib.Path
+        增量更新文件夹
+
+    """
+    # 合并历史数据，方便复制
+    files = path_groupby_size(path0, path0, per_size=128 * 1024 * 1024, reserve=0)
+    merge_files_dict(files, ignore_index=True, delete_src=True)
+    files = path_groupby_size(path1, path1, per_size=128 * 1024 * 1024, reserve=0)
+    merge_files_dict(files, ignore_index=True, delete_src=True)
+    # 每日更新部分，不能老合并，因为修改太多，网络传输量会过大，改成两个月前的都合成一个月，最近两个月的不动
+    files = path_groupby_date(path2, path2, reserve=2)
+    merge_files_dict(files, ignore_index=True, delete_src=True)
```

### Comparing `ddump-0.1.6/ddump/db/merge.py` & `ddump-0.2.0/ddump/db/merge.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,161 +1,156 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-# @Author     :wukan
-# @License    :(C) Copyright 2022
-# @Date       :2022-04-10
-
-"""
-文件合并相关操作
-
-文件名是已经约定好的格式
-
-时间__唯一ID.扩展名。 按文件大小合并
-时间__时间.扩展名。 按时间合并
-
-"""
-
-import pathlib
-
-import pandas as pd
-
-from ..common import FILE_SUFFIX, KEY_SEP_ID
-
-
-def path_groupby_size(input_path, output_path,
-                      per_size=64 * 1024 * 1024,
-                      reserve=2, suffix=FILE_SUFFIX):
-    """合并目录，按文件大小分。超出后才切分。
-
-    合并后的文件是最后一个文件的文件名。
-    所有文件名都按字符串分隔离
-
-    Parameters
-    ----------
-    input_path: pathlib.Path
-        输入目录
-    output_path: pathlib.Path
-        输出目录
-    per_size: int
-        合并后每个文件大概大小。默认64MB
-    reserve: int
-        预留文件数。最后几个文件不动，可能会被修改，文件夹2一定要预留一定数量的文件
-    suffix
-
-    """
-    if output_path is None:
-        output_path = input_path
-
-    files_tail = []
-    files = list(input_path.glob(f'*{suffix}'))
-    if reserve > 0:
-        files_tail = files[-reserve:]
-        files = files[:-reserve]
-
-    fss = {}
-    fs = []
-    st_size = 0
-    for f in files:
-        st_size += f.stat().st_size
-        fs.append(f)
-        if st_size >= per_size:
-            # 单文件满足大小
-            fss[output_path / f.name] = fs
-            fs = []
-            st_size = 0
-
-    # 最后一个需要补录
-    if len(files) > 0:
-        fss[output_path / f.name] = fs
-        fs = []
-
-    for f in files_tail:
-        fs.append(f)
-        fss[output_path / f.name] = fs
-        fs = []
-
-    return fss
-
-
-def path_groupby_date(input_path, output_path,
-                      reserve=2, suffix=FILE_SUFFIX):
-    """根据日期进行合并
-
-    文件由 key_id组合而成
-
-    Parameters
-    ----------
-    input_path: pathlib.Path
-        输入目录
-    output_path: pathlib.Path
-        输出目录
-    reserve: int
-        预留文件数。最后几个文件不动，因为可能会被修改，文件夹2一定要预留一定数量的文件
-    suffix
-
-    Returns
-    -------
-    dict
-
-    """
-    if output_path is None:
-        output_path = input_path
-
-    files_tail = []
-    files = list(input_path.glob(f'*{suffix}'))
-    if reserve > 0:
-        files_tail = files[-reserve:]
-        files = files[:-reserve]
-
-    # 提取文件名中的时间
-    df = pd.DataFrame([f.name.split('.')[0].split(KEY_SEP_ID) for f in files], columns=['key', 'id'])
-    df['path'] = files
-    df['key'] = pd.to_datetime(df['key'])
-    df['key2'] = df['key']
-    df.index = df['key'].copy()
-    df.index.name = 'date'  # 防止无法groupby
-
-    from dateutil.relativedelta import relativedelta, MO, SU
-    from datetime import datetime, timedelta
-
-    # 周week。少用，因为跨月跨年了，如果周重新切分成月年，会出错
-    df['1W_1'] = df['key'].apply(lambda x: x.date() + relativedelta(weekday=MO(-1)))
-    df['1W_2'] = df['key'].apply(lambda x: x.date() + relativedelta(weekday=SU(0)))
-
-    # 月month
-    df['1M_1'] = df['key'].apply(lambda x: x.date() + relativedelta(day=1))
-    df['1M_2'] = df['key'].apply(lambda x: x.date() + relativedelta(day=31))
-    # 季quarter
-    df['1Q_1'] = df['key'].apply(lambda x: x.date() + relativedelta(month=((x.month - 1) // 3) * 3 + 1, day=1))
-    df['1Q_2'] = df['key'].apply(lambda x: x.date() + relativedelta(month=((x.month - 1) // 3 + 1) * 3, day=31))
-    # 年
-    df['1Y_1'] = df['key'].apply(lambda x: x.date() + relativedelta(month=1, day=1))
-    df['1Y_2'] = df['key'].apply(lambda x: x.date() + relativedelta(month=12, day=31))
-    # 十年decade
-    df['10Y_1'] = df['key'].apply(lambda x: x.date() + relativedelta(year=x.year // 10 * 10, month=1, day=1))
-    df['10Y_2'] = df['key'].apply(lambda x: x.date() + relativedelta(year=x.year // 10 * 10 + 9, month=12, day=31))
-
-    df['1M_1'] = pd.to_datetime(df['1M_1'])
-    df['1Y_1'] = pd.to_datetime(df['1Y_1'])
-
-    # 最近的两个月不动，两个月前的都按月合并
-    t = f'{datetime.now() - timedelta(days=31 * 2):%Y-%m}'
-    df['key'] = df.loc[:t, '1M_1']
-    t = f'{datetime.now() - timedelta(days=365 * 1):%Y}'
-    df['key'] = df.loc[:t, '1Y_1']
-    df['key'].fillna(df['key2'], inplace=True)
-
-    # 按key进行分组
-    fss = {}
-    for k, v in df.groupby(by='key'):
-        # 1W_1是组内完全一样，所以直接取最后一行也行
-        fs = v['path'].tolist()
-        fss[output_path / fs[-1].name] = fs
-
-    # 最近的两个文件不动
-    fs = []
-    for f in files_tail:
-        fs.append(f)
-        fss[output_path / f.name] = fs
-        fs = []
-
-    return fss
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+# @Author     :wukan
+# @License    :(C) Copyright 2022
+# @Date       :2022-04-10
+
+"""
+文件合并相关操作
+
+文件名是已经约定好的格式
+
+时间__唯一ID.扩展名。 按文件大小合并
+时间__时间.扩展名。 按时间合并
+
+"""
+
+import pathlib
+
+import pandas as pd
+
+from ..common import FILE_SUFFIX, KEY_SEP_ID
+
+
+def path_groupby_size(input_path, output_path,
+                      per_size=64 * 1024 * 1024,
+                      reserve=2, suffix=FILE_SUFFIX):
+    """合并目录，按文件大小分。超出后才切分。
+
+    合并后的文件是最后一个文件的文件名。
+    所有文件名都按字符串分隔离
+
+    Parameters
+    ----------
+    input_path: pathlib.Path
+        输入目录
+    output_path: pathlib.Path
+        输出目录
+    per_size: int
+        合并后每个文件大概大小。默认64MB
+    reserve: int
+        预留文件数。最后几个文件不动，可能会被修改，文件夹2一定要预留一定数量的文件
+    suffix
+
+    """
+    if output_path is None:
+        output_path = input_path
+
+    files_tail = []
+    files = list(input_path.glob(f'*{suffix}'))
+    if reserve > 0:
+        files_tail = files[-reserve:]
+        files = files[:-reserve]
+
+    fss = {}
+    fs = []
+    st_size = 0
+    for f in files:
+        st_size += f.stat().st_size
+        fs.append(f)
+        if st_size >= per_size:
+            # 单文件满足大小
+            fss[output_path / f.name] = fs
+            fs = []
+            st_size = 0
+
+    # 最后一个需要补录
+    if len(files) > 0:
+        fss[output_path / f.name] = fs
+        fs = []
+
+    for f in files_tail:
+        fs.append(f)
+        fss[output_path / f.name] = fs
+        fs = []
+
+    return fss
+
+
+def path_groupby_date(input_path, output_path,
+                      reserve=2, suffix=FILE_SUFFIX):
+    """根据日期进行合并
+
+    文件由 key_id组合而成
+
+    Parameters
+    ----------
+    input_path: pathlib.Path
+        输入目录
+    output_path: pathlib.Path
+        输出目录
+    reserve: int
+        预留文件数。最后几个文件不动，因为可能会被修改，文件夹2一定要预留一定数量的文件
+    suffix
+
+    Returns
+    -------
+    dict
+
+    """
+    if output_path is None:
+        output_path = input_path
+
+    files_tail = []
+    files = list(input_path.glob(f'*{suffix}'))
+    if reserve > 0:
+        files_tail = files[-reserve:]
+        files = files[:-reserve]
+
+    # 提取文件名中的时间
+    df = pd.DataFrame([f.name.split('.')[0].split(KEY_SEP_ID) for f in files], columns=['key', 'id'])
+    df['path'] = files
+    df['key'] = pd.to_datetime(df['key'])
+    df['key2'] = df['key']
+    df.index = df['key'].copy()
+    df.index.name = 'date'  # 防止无法groupby
+
+    from dateutil.relativedelta import relativedelta, MO, SU
+    from datetime import datetime, timedelta
+
+    # 周week。少用，因为跨月跨年了，如果周重新切分成月年，会出错
+    df['1W_1'] = df['key'].apply(lambda x: x.date() + relativedelta(weekday=MO(-1)))
+    df['1W_2'] = df['key'].apply(lambda x: x.date() + relativedelta(weekday=SU(0)))
+
+    # 月month
+    df['1M_1'] = df['key'].apply(lambda x: x.date() + relativedelta(day=1))
+    df['1M_2'] = df['key'].apply(lambda x: x.date() + relativedelta(day=31))
+    # 季quarter
+    df['1Q_1'] = df['key'].apply(lambda x: x.date() + relativedelta(month=((x.month - 1) // 3) * 3 + 1, day=1))
+    df['1Q_2'] = df['key'].apply(lambda x: x.date() + relativedelta(month=((x.month - 1) // 3 + 1) * 3, day=31))
+    # 年
+    df['1Y_1'] = df['key'].apply(lambda x: x.date() + relativedelta(month=1, day=1))
+    df['1Y_2'] = df['key'].apply(lambda x: x.date() + relativedelta(month=12, day=31))
+    # 十年decade
+    df['10Y_1'] = df['key'].apply(lambda x: x.date() + relativedelta(year=x.year // 10 * 10, month=1, day=1))
+    df['10Y_2'] = df['key'].apply(lambda x: x.date() + relativedelta(year=x.year // 10 * 10 + 9, month=12, day=31))
+
+    df['1M_1'] = pd.to_datetime(df['1M_1'])
+    df['1Y_1'] = pd.to_datetime(df['1Y_1'])
+
+    # 最近的两个月不动，两个月前的都按月合并
+    t = f'{datetime.now() - timedelta(days=31 * 2):%Y-%m}'
+    df['key'] = df.loc[:t, '1M_1']
+    t = f'{datetime.now() - timedelta(days=365 * 1):%Y}'
+    df['key'] = df.loc[:t, '1Y_1']
+    df['key'].fillna(df['key2'], inplace=True)
+
+    # 按key进行分组
+    fss = []
+    for k, v in df.groupby(by='key'):
+        # 1W_1是组内完全一样，所以直接取最后一行也行
+        from_ = v['path'].tolist()
+        to_ = output_path / from_[-1].name
+
+        fss.append({'to': to_, 'from': from_})
+
+    return fss
```

### Comparing `ddump-0.1.6/ddump/db/tool.py` & `ddump-0.2.0/ddump/db/tool.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,264 +1,264 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-# @Author     :wukan
-# @License    :(C) Copyright 2022
-# @Date       :2022-04-11
-
-import pandas as pd
-from loguru import logger
-from sqlalchemy import create_engine
-from sqlalchemy.engine import reflection
-from sqlalchemy.ext.automap import automap_base
-from sqlalchemy.orm import sessionmaker
-
-
-class DbTool:
-    """数据库工具
-
-    连接数据库后，直接使用ORM或SQL进行操作
-
-    Examples
-    --------
-    >>> tushare = DbTool(url="mysql+pymysql://user:pasword@127.0.0.1:3306/tushare?charset=utf8")
-    >>> tushare.show_tables()
-
-    >>> tushare.describe('FDT_STK_AUDIT')
-
-    >>> q = tushare.query(tushare.FDT_STK_AUDIT).limit(10)
-    >>> df = tushare.run_query(q)
-    >>> df.columns = df.columns.str.lower()
-    >>> df
-
-    """
-
-    def __init__(self, url, echo=False):
-        """构造函数
-
-        Parameters
-        ----------
-        url: str
-            数据库访问串。如果密码有@等特殊符号，可能需要改成%40等
-            参考：https://tool.chinaz.com/tools/urlencode.aspx
-        echo: bool
-            回显日志
-
-        """
-        engine = create_engine(url, echo=echo,
-                               pool_recycle=3600, pool_pre_ping=True,
-                               )  # fast_executemany=True
-        self._engine = engine
-
-        # 自动映射所有表
-        Base = automap_base()
-        Base.prepare(engine, reflect=True)
-        self._tables = Base.classes.keys()
-
-        # 会话
-        Session = sessionmaker(bind=engine, autocommit=False)
-        self.session = Session()
-
-        # 注册查询语句
-        self.query = self.session.query
-
-        # 设置表名，希望不会出现表名冲突
-        for key in Base.classes.keys():
-            assert not hasattr(self, key), "表名与对象属性冲突"
-            setattr(self, key, getattr(Base.classes, key))
-
-        # 检查limit，默认需要检查，只给专业人士使用
-        self.check_limit = 5000
-
-    def show_tables(self):
-        """显示所有表名
-
-        Returns
-        -------
-        list
-
-        """
-        return self._tables
-
-    def describe(self, table_name):
-        """显示指定表结构
-
-        Parameters
-        ----------
-        table_name: str
-            表名
-
-        Returns
-        -------
-        pd.DataFrame
-
-        """
-        insp = reflection.Inspector.from_engine(self._engine)
-        columns = insp.get_columns(table_name)
-        return pd.DataFrame(columns)
-
-    def run_query(self, q):
-        """查询结果
-
-        Parameters
-        ----------
-        q: Query
-            查询对象
-
-        Returns
-        -------
-        pd.DataFrame
-
-        """
-        # 太长了
-        logger.trace(str(q))
-
-        if self.check_limit > 0:
-            assert q._limit_clause is not None, '必须设置limit'
-            assert q._limit_clause.value <= self.check_limit, f'limit不能大于{self.check_limit}'
-
-        # self._engine.dispose()
-        return pd.read_sql(q.statement, q.session.bind)
-
-    def run_update(self, q, values, auto_commit=True):
-        """更新数据，需要先查后更新
-
-        Parameters
-        ----------
-        q: Query
-            查询对象
-        values: dict
-            需要更新的数据
-        auto_commit: bool
-            是否自动提交
-
-        Notes
-        -----
-        此处的q不能使用limit语句
-
-        """
-        count = q.update(values)
-
-        if auto_commit:
-            self.commit()
-
-        return count
-
-    def run_delete(self, q, auto_commit=True):
-        """删除
-
-        Parameters
-        ----------
-        q: Query
-            查询对象
-        auto_commit: bool
-            是否自动提交
-
-        Notes
-        -----
-        此处的q不能使用limit语句
-
-        """
-        count = q.delete()
-
-        if auto_commit:
-            self.commit()
-
-        return count
-
-    def insert(self, instances, auto_commit=True):
-        """添加记录
-
-        Parameters
-        ----------
-        instances:
-            ORM对象或列表
-        auto_commit: bool
-            是否自动提交
-
-        Examples
-        --------
-        >>> User = table.User
-        >>> a = User(NAME='wukan', REMARK='aaaa')
-        >>> b = User(NAME='aaaaa', REMARK='bbbb')
-        >>> table.insert(a)
-        >>> table.insert([a,b])
-
-        References
-        ----------
-        https://docs.sqlalchemy.org/en/14/faq/performance.html
-
-        """
-        if isinstance(instances, list):
-            # 使用批量插入
-            self.session.bulk_save_objects(instances)
-        else:
-            self.session.add(instances)
-
-        if auto_commit:
-            self.commit()
-
-    def commit(self):
-        """对事务操作提交"""
-        try:
-            self.session.commit()
-        except Exception as e:
-            self.session.rollback()
-
-    def read_sql(self, sql, **kwargs):
-        """通过sql语句查询
-
-        Parameters
-        ----------
-        sql: str
-            sql语句
-
-        Returns
-        -------
-        pd.DataFrame
-
-        """
-        logger.info(sql)
-        return pd.read_sql(sql, con=self._engine, **kwargs)
-
-    def to_sql(self, df, name, if_exists='append', **kwargs):
-        """将DataFrame插入到数据库
-
-        TODO: 有时也很快, 需要再比较
-
-        Parameters
-        ----------
-        df: pd.DataFrame
-        name: str
-        if_exists: str
-        kwargs:
-
-        """
-
-        return df.to_sql(name, con=self._engine,
-                         if_exists=if_exists, index=False, chunksize=10000,
-                         **kwargs)
-
-
-if __name__ == '__main__':
-    # 显示全部数据，有点多，使用要小心
-    pd.set_option('display.max_columns', None)
-    pd.set_option('display.max_rows', 300)
-
-    finance = DbTool(url="mysql://reader:0075AE8C303EB420@10.174.12.124/finance?charset=utf8")
-    # 显示表名
-    finance.show_tables()
-
-    # 查某表
-    q = finance.query(finance.CCTV_NEWS).limit(10)
-    finance.run_query(q)
-
-    # 显示表结构
-    finance.describe('SW1_DAILY_PRICE')
-
-    # 直接SQL查询
-    finance.read_sql('select * from FUND_DIVIDEND limit 0,10')
-
-    # 更新
-    finance.run_update(q, {'A': 'B'})
-
-    # 插入
-    finance.insert(finance.CCTV_NEWS(title='abc'))
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+# @Author     :wukan
+# @License    :(C) Copyright 2022
+# @Date       :2022-04-11
+
+import pandas as pd
+from loguru import logger
+from sqlalchemy import create_engine
+from sqlalchemy.engine import reflection
+from sqlalchemy.ext.automap import automap_base
+from sqlalchemy.orm import sessionmaker
+
+
+class DbTool:
+    """数据库工具
+
+    连接数据库后，直接使用ORM或SQL进行操作
+
+    Examples
+    --------
+    >>> tushare = DbTool(url="mysql+pymysql://user:pasword@127.0.0.1:3306/tushare?charset=utf8")
+    >>> tushare.show_tables()
+
+    >>> tushare.describe('FDT_STK_AUDIT')
+
+    >>> q = tushare.query(tushare.FDT_STK_AUDIT).limit(10)
+    >>> df = tushare.run_query(q)
+    >>> df.columns = df.columns.str.lower()
+    >>> df
+
+    """
+
+    def __init__(self, url, echo=False):
+        """构造函数
+
+        Parameters
+        ----------
+        url: str
+            数据库访问串。如果密码有@等特殊符号，可能需要改成%40等
+            参考：https://tool.chinaz.com/tools/urlencode.aspx
+        echo: bool
+            回显日志
+
+        """
+        engine = create_engine(url, echo=echo,
+                               pool_recycle=3600, pool_pre_ping=True,
+                               )  # fast_executemany=True
+        self._engine = engine
+
+        # 自动映射所有表
+        Base = automap_base()
+        Base.prepare(engine, reflect=True)
+        self._tables = Base.classes.keys()
+
+        # 会话
+        Session = sessionmaker(bind=engine, autocommit=False)
+        self.session = Session()
+
+        # 注册查询语句
+        self.query = self.session.query
+
+        # 设置表名，希望不会出现表名冲突
+        for key in Base.classes.keys():
+            assert not hasattr(self, key), "表名与对象属性冲突"
+            setattr(self, key, getattr(Base.classes, key))
+
+        # 检查limit，默认需要检查，只给专业人士使用
+        self.check_limit = 5000
+
+    def show_tables(self):
+        """显示所有表名
+
+        Returns
+        -------
+        list
+
+        """
+        return self._tables
+
+    def describe(self, table_name):
+        """显示指定表结构
+
+        Parameters
+        ----------
+        table_name: str
+            表名
+
+        Returns
+        -------
+        pd.DataFrame
+
+        """
+        insp = reflection.Inspector.from_engine(self._engine)
+        columns = insp.get_columns(table_name)
+        return pd.DataFrame(columns)
+
+    def run_query(self, q):
+        """查询结果
+
+        Parameters
+        ----------
+        q: Query
+            查询对象
+
+        Returns
+        -------
+        pd.DataFrame
+
+        """
+        # 太长了
+        logger.trace(str(q))
+
+        if self.check_limit > 0:
+            assert q._limit_clause is not None, '必须设置limit'
+            assert q._limit_clause.value <= self.check_limit, f'limit不能大于{self.check_limit}'
+
+        # self._engine.dispose()
+        return pd.read_sql(q.statement, q.session.bind)
+
+    def run_update(self, q, values, auto_commit=True):
+        """更新数据，需要先查后更新
+
+        Parameters
+        ----------
+        q: Query
+            查询对象
+        values: dict
+            需要更新的数据
+        auto_commit: bool
+            是否自动提交
+
+        Notes
+        -----
+        此处的q不能使用limit语句
+
+        """
+        count = q.update(values)
+
+        if auto_commit:
+            self.commit()
+
+        return count
+
+    def run_delete(self, q, auto_commit=True):
+        """删除
+
+        Parameters
+        ----------
+        q: Query
+            查询对象
+        auto_commit: bool
+            是否自动提交
+
+        Notes
+        -----
+        此处的q不能使用limit语句
+
+        """
+        count = q.delete()
+
+        if auto_commit:
+            self.commit()
+
+        return count
+
+    def insert(self, instances, auto_commit=True):
+        """添加记录
+
+        Parameters
+        ----------
+        instances:
+            ORM对象或列表
+        auto_commit: bool
+            是否自动提交
+
+        Examples
+        --------
+        >>> User = table.User
+        >>> a = User(NAME='wukan', REMARK='aaaa')
+        >>> b = User(NAME='aaaaa', REMARK='bbbb')
+        >>> table.insert(a)
+        >>> table.insert([a,b])
+
+        References
+        ----------
+        https://docs.sqlalchemy.org/en/14/faq/performance.html
+
+        """
+        if isinstance(instances, list):
+            # 使用批量插入
+            self.session.bulk_save_objects(instances)
+        else:
+            self.session.add(instances)
+
+        if auto_commit:
+            self.commit()
+
+    def commit(self):
+        """对事务操作提交"""
+        try:
+            self.session.commit()
+        except Exception as e:
+            self.session.rollback()
+
+    def read_sql(self, sql, **kwargs):
+        """通过sql语句查询
+
+        Parameters
+        ----------
+        sql: str
+            sql语句
+
+        Returns
+        -------
+        pd.DataFrame
+
+        """
+        logger.info(sql)
+        return pd.read_sql(sql, con=self._engine, **kwargs)
+
+    def to_sql(self, df, name, if_exists='append', **kwargs):
+        """将DataFrame插入到数据库
+
+        TODO: 有时也很快, 需要再比较
+
+        Parameters
+        ----------
+        df: pd.DataFrame
+        name: str
+        if_exists: str
+        kwargs:
+
+        """
+
+        return df.to_sql(name, con=self._engine,
+                         if_exists=if_exists, index=False, chunksize=10000,
+                         **kwargs)
+
+
+if __name__ == '__main__':
+    # 显示全部数据，有点多，使用要小心
+    pd.set_option('display.max_columns', None)
+    pd.set_option('display.max_rows', 300)
+
+    finance = DbTool(url="mysql://reader:0075AE8C303EB420@10.174.12.124/finance?charset=utf8")
+    # 显示表名
+    finance.show_tables()
+
+    # 查某表
+    q = finance.query(finance.CCTV_NEWS).limit(10)
+    finance.run_query(q)
+
+    # 显示表结构
+    finance.describe('SW1_DAILY_PRICE')
+
+    # 直接SQL查询
+    finance.read_sql('select * from FUND_DIVIDEND limit 0,10')
+
+    # 更新
+    finance.run_update(q, {'A': 'B'})
+
+    # 插入
+    finance.insert(finance.CCTV_NEWS(title='abc'))
```

