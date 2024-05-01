# Comparing `tmp/danielutils-0.9.80.tar.gz` & `tmp/danielutils-0.9.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danielutils-0.9.80.tar", last modified: Sun Apr 28 08:47:56 2024, max compression
+gzip compressed data, was "danielutils-0.9.81.tar", last modified: Wed May  1 12:37:29 2024, max compression
```

## Comparing `danielutils-0.9.80.tar` & `danielutils-0.9.81.tar`

### file list

```diff
@@ -1,224 +1,228 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.386866 danielutils-0.9.80/
--rw-rw-rw-   0        0        0     1091 2023-05-29 13:19:53.000000 danielutils-0.9.80/LICENSE
--rw-rw-rw-   0        0        0       34 2024-04-28 08:47:55.000000 danielutils-0.9.80/MANIFEST.in
--rw-rw-rw-   0        0        0     4593 2024-04-28 08:47:56.386866 danielutils-0.9.80/PKG-INFO
--rw-rw-rw-   0        0        0     2650 2024-04-28 08:19:41.000000 danielutils-0.9.80/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.249964 danielutils-0.9.80/danielutils/
--rw-rw-rw-   0        0        0     1364 2024-04-21 19:46:04.000000 danielutils-0.9.80/danielutils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.256523 danielutils-0.9.80/danielutils/abstractions/
--rw-rw-rw-   0        0        0       77 2024-04-21 19:46:54.000000 danielutils-0.9.80/danielutils/abstractions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.259709 danielutils-0.9.80/danielutils/abstractions/database/
--rw-rw-rw-   0        0        0       57 2024-04-21 18:12:14.000000 danielutils-0.9.80/danielutils/abstractions/database/__init__.py
--rw-rw-rw-   0        0        0     2772 2024-04-17 20:37:10.000000 danielutils-0.9.80/danielutils/abstractions/database/cached_database.py
--rw-rw-rw-   0        0        0     2621 2024-04-28 08:07:23.000000 danielutils-0.9.80/danielutils/abstractions/database/database.py
--rw-rw-rw-   0        0        0     1048 2024-04-25 20:10:37.000000 danielutils-0.9.80/danielutils/abstractions/database/redis_database.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.262249 danielutils-0.9.80/danielutils/abstractions/multiprogramming/
--rw-rw-rw-   0        0        0       74 2024-04-21 19:21:56.000000 danielutils-0.9.80/danielutils/abstractions/multiprogramming/__init__.py
--rw-rw-rw-   0        0        0      374 2024-04-17 20:37:10.000000 danielutils-0.9.80/danielutils/abstractions/multiprogramming/multi_id.py
--rw-rw-rw-   0        0        0     2392 2024-04-28 08:12:35.000000 danielutils-0.9.80/danielutils/abstractions/multiprogramming/worker.py
--rw-rw-rw-   0        0        0     2412 2024-04-28 08:12:35.000000 danielutils-0.9.80/danielutils/abstractions/multiprogramming/worker_pool.py
--rw-rw-rw-   0        0        0     3144 2024-04-28 08:12:35.000000 danielutils-0.9.80/danielutils/abstractions/repl.py
--rw-rw-rw-   0        0        0     5663 2024-03-21 20:59:13.000000 danielutils-0.9.80/danielutils/aliases.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.262249 danielutils-0.9.80/danielutils/better_builtins/
--rw-rw-rw-   0        0        0       78 2024-04-21 18:23:39.000000 danielutils-0.9.80/danielutils/better_builtins/__init__.py
--rw-rw-rw-   0        0        0     1221 2024-03-21 20:59:13.000000 danielutils-0.9.80/danielutils/better_builtins/counter.py
--rw-rw-rw-   0        0        0     7174 2024-04-21 18:12:40.000000 danielutils-0.9.80/danielutils/better_builtins/frange.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.266677 danielutils-0.9.80/danielutils/better_builtins/typed_builtins/
--rw-rw-rw-   0        0        0       88 2024-03-21 20:59:13.000000 danielutils-0.9.80/danielutils/better_builtins/typed_builtins/__init__.py
--rw-rw-rw-   0        0        0     4704 2024-04-28 08:12:35.000000 danielutils-0.9.80/danielutils/better_builtins/typed_builtins/factory.py
--rw-rw-rw-   0        0        0      913 2024-03-21 20:59:13.000000 danielutils-0.9.80/danielutils/better_builtins/typed_builtins/tdict.py
--rw-rw-rw-   0        0        0     7210 2024-04-28 08:12:13.000000 danielutils-0.9.80/danielutils/better_builtins/typed_builtins/tlist.py
--rw-rw-rw-   0        0        0     2031 2024-03-21 20:59:13.000000 danielutils-0.9.80/danielutils/better_builtins/typed_builtins/tset.py
--rw-rw-rw-   0        0        0      294 2024-03-21 20:59:13.000000 danielutils-0.9.80/danielutils/better_builtins/typed_builtins/ttuple.py
--rw-rw-rw-   0        0        0     5472 2024-04-28 08:19:09.000000 danielutils-0.9.80/danielutils/colors.py
--rw-rw-rw-   0        0        0      210 2024-03-21 20:59:13.000000 danielutils-0.9.80/danielutils/convenience.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.269700 danielutils-0.9.80/danielutils/conversions/
--rw-rw-rw-   0        0        0       73 2024-03-21 20:59:13.000000 danielutils-0.9.80/danielutils/conversions/__init__.py
--rw-rw-rw-   0        0        0     2362 2024-04-28 08:19:08.000000 danielutils-0.9.80/danielutils/conversions/main_conversions.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.271208 danielutils-0.9.80/danielutils/conversions/specialized_conversions/
--rw-rw-rw-   0        0        0       46 2024-03-21 20:59:13.000000 danielutils-0.9.80/danielutils/conversions/specialized_conversions/__init__.py
--rw-rw-rw-   0        0        0      507 2024-03-21 23:16:41.000000 danielutils-0.9.80/danielutils/conversions/specialized_conversions/to_hex.py
--rw-rw-rw-   0        0        0      543 2024-04-28 08:12:13.000000 danielutils-0.9.80/danielutils/conversions/specialized_conversions/to_int.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.277476 danielutils-0.9.80/danielutils/data_structures/
--rw-rw-rw-   0        0        0      163 2024-04-17 20:37:10.000000 danielutils-0.9.80/danielutils/data_structures/__init__.py
--rw-rw-rw-   0        0        0     1224 2024-04-17 20:37:10.000000 danielutils-0.9.80/danielutils/data_structures/comparer.py
--rw-rw-rw-   0        0        0      273 2024-04-17 20:37:10.000000 danielutils-0.9.80/danielutils/data_structures/default_dict.py
--rw-rw-rw-   0        0        0      632 2023-09-25 13:19:42.000000 danielutils-0.9.80/danielutils/data_structures/functions.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.280266 danielutils-0.9.80/danielutils/data_structures/graph/
--rw-rw-rw-   0        0        0       97 2024-04-17 20:37:10.000000 danielutils-0.9.80/danielutils/data_structures/graph/__init__.py
--rw-rw-rw-   0        0        0     2066 2024-04-18 18:33:41.000000 danielutils-0.9.80/danielutils/data_structures/graph/binary_node.py
--rw-rw-rw-   0        0        0     6877 2024-04-28 08:12:24.000000 danielutils-0.9.80/danielutils/data_structures/graph/graph.py
--rw-rw-rw-   0        0        0     3141 2024-04-28 08:12:13.000000 danielutils-0.9.80/danielutils/data_structures/graph/multinode.py
--rw-rw-rw-   0        0        0     1647 2024-03-28 19:42:06.000000 danielutils-0.9.80/danielutils/data_structures/graph/node.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.280266 danielutils-0.9.80/danielutils/data_structures/heap/
--rw-rw-rw-   0        0        0       71 2024-03-28 19:45:24.000000 danielutils-0.9.80/danielutils/data_structures/heap/__init__.py
--rw-rw-rw-   0        0        0     3092 2024-04-17 20:37:10.000000 danielutils-0.9.80/danielutils/data_structures/heap/heap.py
--rw-rw-rw-   0        0        0      292 2024-03-28 19:45:24.000000 danielutils-0.9.80/danielutils/data_structures/heap/max_heap.py
--rw-rw-rw-   0        0        0      300 2024-03-28 19:45:24.000000 danielutils-0.9.80/danielutils/data_structures/heap/min_heap.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.287259 danielutils-0.9.80/danielutils/data_structures/queue/
--rw-rw-rw-   0        0        0       82 2024-03-28 19:35:07.000000 danielutils-0.9.80/danielutils/data_structures/queue/__init__.py
--rw-rw-rw-   0        0        0      260 2024-03-28 19:35:13.000000 danielutils-0.9.80/danielutils/data_structures/queue/atomic_queue.py
--rw-rw-rw-   0        0        0     3661 2024-03-28 19:35:07.000000 danielutils-0.9.80/danielutils/data_structures/queue/priority_queue.py
--rw-rw-rw-   0        0        0     1615 2024-04-28 08:12:13.000000 danielutils-0.9.80/danielutils/data_structures/queue/queue.py
--rw-rw-rw-   0        0        0     2143 2024-04-17 20:37:10.000000 danielutils-0.9.80/danielutils/data_structures/stack.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.287259 danielutils-0.9.80/danielutils/data_structures/trees/
--rw-rw-rw-   0        0        0       63 2024-04-17 20:37:10.000000 danielutils-0.9.80/danielutils/data_structures/trees/__init__.py
--rw-rw-rw-   0        0        0     2636 2024-04-28 08:12:00.000000 danielutils-0.9.80/danielutils/data_structures/trees/binary_syntax_tree.py
--rw-rw-rw-   0        0        0     1618 2024-04-18 18:33:41.000000 danielutils-0.9.80/danielutils/data_structures/trees/binary_tree.py
--rw-rw-rw-   0        0        0      675 2024-04-28 08:19:08.000000 danielutils-0.9.80/danielutils/date.py
--rw-rw-rw-   0        0        0      232 2023-08-07 20:06:13.000000 danielutils-0.9.80/danielutils/date_time.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.305558 danielutils-0.9.80/danielutils/decorators/
--rw-rw-rw-   0        0        0      466 2024-04-25 20:44:13.000000 danielutils-0.9.80/danielutils/decorators/__init__.py
--rw-rw-rw-   0        0        0      756 2024-04-28 08:19:08.000000 danielutils-0.9.80/danielutils/decorators/atomic.py
--rw-rw-rw-   0        0        0     1385 2024-04-28 08:19:08.000000 danielutils-0.9.80/danielutils/decorators/attach.py
--rw-rw-rw-   0        0        0      730 2024-03-21 20:59:13.000000 danielutils-0.9.80/danielutils/decorators/chain_decorators.py
--rw-rw-rw-   0        0        0     1089 2024-04-28 08:19:08.000000 danielutils-0.9.80/danielutils/decorators/decorate_conditionally.py
--rw-rw-rw-   0        0        0     1008 2024-04-27 18:49:37.000000 danielutils-0.9.80/danielutils/decorators/delay_call.py
--rw-rw-rw-   0        0        0     1290 2024-04-27 18:48:35.000000 danielutils-0.9.80/danielutils/decorators/deprecate.py
--rw-rw-rw-   0        0        0     1023 2024-04-25 20:44:13.000000 danielutils-0.9.80/danielutils/decorators/final.py
--rw-rw-rw-   0        0        0     1696 2024-04-28 08:19:08.000000 danielutils-0.9.80/danielutils/decorators/limit_recursion.py
--rw-rw-rw-   0        0        0      806 2024-04-28 08:19:08.000000 danielutils-0.9.80/danielutils/decorators/memo.py
--rw-rw-rw-   0        0        0     7521 2024-04-28 08:13:16.000000 danielutils-0.9.80/danielutils/decorators/overload.py
--rw-rw-rw-   0        0        0      837 2024-04-28 08:19:09.000000 danielutils-0.9.80/danielutils/decorators/partially_implemented.py
--rw-rw-rw-   0        0        0     1716 2024-04-21 19:46:04.000000 danielutils-0.9.80/danielutils/decorators/processify.py
--rw-rw-rw-   0        0        0     1095 2024-03-21 20:59:13.000000 danielutils-0.9.80/danielutils/decorators/property.py
--rw-rw-rw-   0        0        0      776 2024-04-17 20:37:10.000000 danielutils-0.9.80/danielutils/decorators/singleton.py
--rw-rw-rw-   0        0        0      729 2024-04-27 18:49:28.000000 danielutils-0.9.80/danielutils/decorators/threadify.py
--rw-rw-rw-   0        0        0     1998 2024-04-28 08:19:08.000000 danielutils-0.9.80/danielutils/decorators/timeout.py
--rw-rw-rw-   0        0        0     3746 2024-04-28 08:13:33.000000 danielutils-0.9.80/danielutils/decorators/total_ordering.py
--rw-rw-rw-   0        0        0     9556 2024-04-28 08:19:08.000000 danielutils-0.9.80/danielutils/decorators/validate.py
--rw-rw-rw-   0        0        0     2163 2024-03-21 20:59:13.000000 danielutils-0.9.80/danielutils/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.311634 danielutils-0.9.80/danielutils/functions/
--rw-rw-rw-   0        0        0      235 2024-04-21 19:19:56.000000 danielutils-0.9.80/danielutils/functions/__init__.py
--rw-rw-rw-   0        0        0     1085 2024-04-28 08:12:35.000000 danielutils-0.9.80/danielutils/functions/areoneof.py
--rw-rw-rw-   0        0        0      638 2024-03-21 20:59:13.000000 danielutils-0.9.80/danielutils/functions/check_foreach.py
--rw-rw-rw-   0        0        0      791 2024-04-21 19:19:56.000000 danielutils-0.9.80/danielutils/functions/flatten.py
--rw-rw-rw-   0        0        0    10122 2024-04-28 08:10:10.000000 danielutils-0.9.80/danielutils/functions/isoftype.py
--rw-rw-rw-   0        0        0     1582 2024-04-28 08:12:35.000000 danielutils-0.9.80/danielutils/functions/isoneof.py
--rw-rw-rw-   0        0        0     1292 2024-04-28 08:07:23.000000 danielutils-0.9.80/danielutils/functions/multiloop.py
--rw-rw-rw-   0        0        0      639 2024-03-21 20:59:13.000000 danielutils-0.9.80/danielutils/functions/powerset.py
--rw-rw-rw-   0        0        0      288 2024-03-21 20:59:13.000000 danielutils-0.9.80/danielutils/functions/subseteq.py
--rw-rw-rw-   0        0        0     1008 2024-04-28 08:12:24.000000 danielutils-0.9.80/danielutils/functions/types_subseteq.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.315656 danielutils-0.9.80/danielutils/generators/
--rw-rw-rw-   0        0        0      108 2024-03-21 20:59:13.000000 danielutils-0.9.80/danielutils/generators/__init__.py
--rw-rw-rw-   0        0        0     1285 2024-03-21 20:59:13.000000 danielutils-0.9.80/danielutils/generators/conditional_generator.py
--rw-rw-rw-   0        0        0      478 2024-04-28 08:19:09.000000 danielutils-0.9.80/danielutils/generators/generator_from_stream.py
--rw-rw-rw-   0        0        0     2859 2024-04-28 08:12:35.000000 danielutils-0.9.80/danielutils/generators/join_generators.py
--rw-rw-rw-   0        0        0     2105 2024-04-28 08:19:08.000000 danielutils-0.9.80/danielutils/internet.py
--rw-rw-rw-   0        0        0    12329 2024-04-28 08:19:14.000000 danielutils-0.9.80/danielutils/io_.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.316632 danielutils-0.9.80/danielutils/math_/
--rw-rw-rw-   0        0        0       79 2024-04-21 18:05:24.000000 danielutils-0.9.80/danielutils/math_/__init__.py
--rw-rw-rw-   0        0        0     7682 2024-03-21 20:59:13.000000 danielutils-0.9.80/danielutils/math_/constants.py
--rw-rw-rw-   0        0        0      642 2024-04-28 08:19:09.000000 danielutils-0.9.80/danielutils/math_/functions.py
--rw-rw-rw-   0        0        0     1063 2024-04-21 18:05:24.000000 danielutils-0.9.80/danielutils/math_/math_print.py
--rw-rw-rw-   0        0        0     4044 2024-04-28 08:12:00.000000 danielutils-0.9.80/danielutils/math_/math_symbols.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.316632 danielutils-0.9.80/danielutils/math_/polynomial/
--rw-rw-rw-   0        0        0       25 2024-04-21 18:05:24.000000 danielutils-0.9.80/danielutils/math_/polynomial/__init__.py
--rw-rw-rw-   0        0        0      835 2024-04-28 08:12:13.000000 danielutils-0.9.80/danielutils/math_/polynomial/polinomial.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.326626 danielutils-0.9.80/danielutils/metaclasses/
--rw-rw-rw-   0        0        0      169 2024-03-21 23:16:41.000000 danielutils-0.9.80/danielutils/metaclasses/__init__.py
--rw-rw-rw-   0        0        0      695 2024-03-21 20:59:13.000000 danielutils-0.9.80/danielutils/metaclasses/atomic_class_meta.py
--rw-rw-rw-   0        0        0     2511 2024-03-21 20:59:13.000000 danielutils-0.9.80/danielutils/metaclasses/implicit_data_deleter_meta.py
--rw-rw-rw-   0        0        0     1495 2024-04-21 18:13:57.000000 danielutils-0.9.80/danielutils/metaclasses/instance_cache_meta.py
--rw-rw-rw-   0        0        0    10932 2024-04-28 08:12:24.000000 danielutils-0.9.80/danielutils/metaclasses/interface.py
--rw-rw-rw-   0        0        0     1754 2024-03-21 20:59:13.000000 danielutils-0.9.80/danielutils/metaclasses/overload_meta.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.329127 danielutils-0.9.80/danielutils/mock_/
--rw-rw-rw-   0        0        0       58 2024-04-21 18:12:14.000000 danielutils-0.9.80/danielutils/mock_/__init__.py
--rw-rw-rw-   0        0        0     2017 2024-04-21 19:46:04.000000 danielutils-0.9.80/danielutils/mock_/mock_database.py
--rw-rw-rw-   0        0        0      419 2024-04-17 20:37:10.000000 danielutils-0.9.80/danielutils/mock_/mock_module.py
--rw-rw-rw-   0        0        0     1032 2024-03-21 20:59:13.000000 danielutils-0.9.80/danielutils/path.py
--rw-rw-rw-   0        0        0     2801 2024-04-21 18:05:24.000000 danielutils-0.9.80/danielutils/print_.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.331441 danielutils-0.9.80/danielutils/protocols/
--rw-rw-rw-   0        0        0       49 2024-04-17 20:37:10.000000 danielutils-0.9.80/danielutils/protocols/__init__.py
--rw-rw-rw-   0        0        0      446 2024-04-28 08:12:00.000000 danielutils-0.9.80/danielutils/protocols/dictable.py
--rw-rw-rw-   0        0        0      203 2024-04-17 20:37:10.000000 danielutils-0.9.80/danielutils/protocols/evaluable.py
--rw-rw-rw-   0        0        0        0 2023-08-09 09:08:58.000000 danielutils-0.9.80/danielutils/py.typed
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.332832 danielutils-0.9.80/danielutils/reflection/
--rw-rw-rw-   0        0        0     1516 2024-04-21 18:21:37.000000 danielutils-0.9.80/danielutils/reflection/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.336254 danielutils-0.9.80/danielutils/reflection/class_/
--rw-rw-rw-   0        0        0       31 2024-04-21 18:21:37.000000 danielutils-0.9.80/danielutils/reflection/class_/__init__.py
--rw-rw-rw-   0        0        0     5507 2024-04-28 08:12:35.000000 danielutils-0.9.80/danielutils/reflection/class_/class_reflection.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.339278 danielutils-0.9.80/danielutils/reflection/file/
--rw-rw-rw-   0        0        0       30 2024-04-21 18:21:37.000000 danielutils-0.9.80/danielutils/reflection/file/__init__.py
--rw-rw-rw-   0        0        0     1657 2024-04-27 18:35:37.000000 danielutils-0.9.80/danielutils/reflection/file/file_reflection.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.340286 danielutils-0.9.80/danielutils/reflection/function/
--rw-rw-rw-   0        0        0       35 2024-04-21 18:21:37.000000 danielutils-0.9.80/danielutils/reflection/function/__init__.py
--rw-rw-rw-   0        0        0     4453 2024-04-28 08:12:24.000000 danielutils-0.9.80/danielutils/reflection/function/function_reflections.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.345496 danielutils-0.9.80/danielutils/reflection/interpreter/
--rw-rw-rw-   0        0        0      179 2024-04-21 19:19:56.000000 danielutils-0.9.80/danielutils/reflection/interpreter/__init__.py
--rw-rw-rw-   0        0        0     1074 2024-04-25 20:37:30.000000 danielutils-0.9.80/danielutils/reflection/interpreter/callstack.py
--rw-rw-rw-   0        0        0      441 2024-04-28 08:12:13.000000 danielutils-0.9.80/danielutils/reflection/interpreter/get_traceback.py
--rw-rw-rw-   0        0        0      622 2024-04-17 20:37:10.000000 danielutils-0.9.80/danielutils/reflection/interpreter/os_.py
--rw-rw-rw-   0        0        0     1023 2024-04-17 20:37:10.000000 danielutils-0.9.80/danielutils/reflection/interpreter/packages.py
--rw-rw-rw-   0        0        0      621 2024-04-28 08:12:35.000000 danielutils-0.9.80/danielutils/reflection/interpreter/python_version.py
--rw-rw-rw-   0        0        0      489 2024-03-21 20:59:13.000000 danielutils-0.9.80/danielutils/reflection/interpreter/signals.py
--rw-rw-rw-   0        0        0     5733 2024-04-28 08:12:24.000000 danielutils-0.9.80/danielutils/reflection/interpreter/tracer.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.348507 danielutils-0.9.80/danielutils/reflection/module/
--rw-rw-rw-   0        0        0       68 2024-04-21 18:27:13.000000 danielutils-0.9.80/danielutils/reflection/module/__init__.py
--rw-rw-rw-   0        0        0      507 2024-03-21 20:59:13.000000 danielutils-0.9.80/danielutils/reflection/module/module_reflections.py
--rw-rw-rw-   0        0        0     4714 2024-04-28 08:12:24.000000 danielutils-0.9.80/danielutils/reflection/module/package_reflection.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.352640 danielutils-0.9.80/danielutils/snippets/
--rw-rw-rw-   0        0        0       24 2024-03-21 20:59:13.000000 danielutils-0.9.80/danielutils/snippets/__init__.py
--rw-rw-rw-   0        0        0      433 2024-03-21 20:59:13.000000 danielutils-0.9.80/danielutils/snippets/try_get.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.352640 danielutils-0.9.80/danielutils/system/
--rw-rw-rw-   0        0        0       52 2024-03-21 20:59:13.000000 danielutils-0.9.80/danielutils/system/__init__.py
--rw-rw-rw-   0        0        0     6863 2024-04-28 08:19:08.000000 danielutils-0.9.80/danielutils/system/independent.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.356691 danielutils-0.9.80/danielutils/system/windows/
--rw-rw-rw-   0        0        0       50 2024-03-21 20:59:13.000000 danielutils-0.9.80/danielutils/system/windows/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.357433 danielutils-0.9.80/danielutils/system/windows/utils/
--rw-rw-rw-   0        0        0       25 2024-03-21 20:59:13.000000 danielutils-0.9.80/danielutils/system/windows/utils/__init__.py
--rw-rw-rw-   0        0        0      499 2024-04-17 20:37:10.000000 danielutils-0.9.80/danielutils/system/windows/utils/filetime.py
--rw-rw-rw-   0        0        0     6064 2024-03-21 20:59:13.000000 danielutils-0.9.80/danielutils/system/windows/win32_ctime.py
--rw-rw-rw-   0        0        0     2253 2024-03-21 20:59:13.000000 danielutils-0.9.80/danielutils/system/windows/windows.py
--rw-rw-rw-   0        0        0     4213 2024-04-28 08:19:08.000000 danielutils-0.9.80/danielutils/text.py
--rw-rw-rw-   0        0        0     1225 2024-04-27 18:53:17.000000 danielutils-0.9.80/danielutils/time.py
--rw-rw-rw-   0        0        0     1723 2024-04-28 08:12:13.000000 danielutils-0.9.80/danielutils/tqdm_.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.359974 danielutils-0.9.80/danielutils/university/
--rw-rw-rw-   0        0        0       74 2024-04-17 20:37:10.000000 danielutils-0.9.80/danielutils/university/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.360887 danielutils-0.9.80/danielutils/university/databases/
--rw-rw-rw-   0        0        0       20 2024-03-21 20:59:13.000000 danielutils-0.9.80/danielutils/university/databases/__init__.py
--rw-rw-rw-   0        0        0    24890 2024-04-28 08:12:35.000000 danielutils-0.9.80/danielutils/university/databases/all.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.360887 danielutils-0.9.80/danielutils/university/oop/
--rw-rw-rw-   0        0        0       25 2024-04-17 20:37:10.000000 danielutils-0.9.80/danielutils/university/oop/__init__.py
--rw-rw-rw-   0        0        0      802 2024-04-28 08:13:50.000000 danielutils-0.9.80/danielutils/university/oop/observer.py
--rw-rw-rw-   0        0        0       87 2024-04-17 20:37:10.000000 danielutils-0.9.80/danielutils/university/oop/strategy.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.367718 danielutils-0.9.80/danielutils/university/probability/
--rw-rw-rw-   0        0        0      189 2024-04-21 22:41:40.000000 danielutils-0.9.80/danielutils/university/probability/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.369325 danielutils-0.9.80/danielutils/university/probability/conditional_variable/
--rw-rw-rw-   0        0        0       89 2024-04-17 20:37:10.000000 danielutils-0.9.80/danielutils/university/probability/conditional_variable/__init__.py
--rw-rw-rw-   0        0        0     4004 2024-04-25 21:21:07.000000 danielutils-0.9.80/danielutils/university/probability/conditional_variable/conditional_variable.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.369325 danielutils-0.9.80/danielutils/university/probability/conditional_variable/continuous/
--rw-rw-rw-   0        0        0        0 2024-04-17 20:37:10.000000 danielutils-0.9.80/danielutils/university/probability/conditional_variable/continuous/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.377519 danielutils-0.9.80/danielutils/university/probability/conditional_variable/discrete/
--rw-rw-rw-   0        0        0      209 2024-04-17 20:37:10.000000 danielutils-0.9.80/danielutils/university/probability/conditional_variable/discrete/__init__.py
--rw-rw-rw-   0        0        0     1149 2024-04-21 22:51:43.000000 danielutils-0.9.80/danielutils/university/probability/conditional_variable/discrete/bernoulli.py
--rw-rw-rw-   0        0        0     1257 2024-04-21 22:51:43.000000 danielutils-0.9.80/danielutils/university/probability/conditional_variable/discrete/binomial.py
--rw-rw-rw-   0        0        0     1108 2024-04-21 22:51:43.000000 danielutils-0.9.80/danielutils/university/probability/conditional_variable/discrete/conditional_from_discrete_probability_func.py
--rw-rw-rw-   0        0        0     1370 2024-04-21 22:51:43.000000 danielutils-0.9.80/danielutils/university/probability/conditional_variable/discrete/discrete.py
--rw-rw-rw-   0        0        0     1652 2024-04-28 08:12:35.000000 danielutils-0.9.80/danielutils/university/probability/conditional_variable/discrete/geometric.py
--rw-rw-rw-   0        0        0      992 2024-04-21 22:51:43.000000 danielutils-0.9.80/danielutils/university/probability/conditional_variable/discrete/poisson.py
--rw-rw-rw-   0        0        0     1040 2024-04-21 22:51:43.000000 danielutils-0.9.80/danielutils/university/probability/conditional_variable/discrete/uniform.py
--rw-rw-rw-   0        0        0      904 2024-04-21 22:41:40.000000 danielutils-0.9.80/danielutils/university/probability/distributions.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.381641 danielutils-0.9.80/danielutils/university/probability/expressions/
--rw-rw-rw-   0        0        0       79 2024-04-17 22:49:00.000000 danielutils-0.9.80/danielutils/university/probability/expressions/__init__.py
--rw-rw-rw-   0        0        0     7439 2024-04-25 21:20:42.000000 danielutils-0.9.80/danielutils/university/probability/expressions/accumulation_expression.py
--rw-rw-rw-   0        0        0     4391 2024-04-25 21:20:53.000000 danielutils-0.9.80/danielutils/university/probability/expressions/probability_expression.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.386324 danielutils-0.9.80/danielutils/university/probability/funcs/
--rw-rw-rw-   0        0        0      120 2024-04-17 20:37:10.000000 danielutils-0.9.80/danielutils/university/probability/funcs/__init__.py
--rw-rw-rw-   0        0        0      338 2024-04-21 22:41:40.000000 danielutils-0.9.80/danielutils/university/probability/funcs/covariance.py
--rw-rw-rw-   0        0        0     1173 2024-04-21 22:41:40.000000 danielutils-0.9.80/danielutils/university/probability/funcs/expected_value.py
--rw-rw-rw-   0        0        0      306 2024-04-17 20:37:10.000000 danielutils-0.9.80/danielutils/university/probability/funcs/probability_function.py
--rw-rw-rw-   0        0        0      437 2024-04-21 22:41:40.000000 danielutils-0.9.80/danielutils/university/probability/funcs/variance.py
--rw-rw-rw-   0        0        0     1987 2024-04-28 08:12:24.000000 danielutils-0.9.80/danielutils/university/probability/operator.py
--rw-rw-rw-   0        0        0      641 2024-04-18 18:33:41.000000 danielutils-0.9.80/danielutils/university/probability/protocols.py
--rw-rw-rw-   0        0        0     2055 2024-04-21 22:51:43.000000 danielutils-0.9.80/danielutils/university/probability/supp.py
--rw-rw-rw-   0        0        0     1182 2024-04-25 20:08:45.000000 danielutils-0.9.80/danielutils/university/probability/transformation.py
--rw-rw-rw-   0        0        0      322 2024-04-28 08:07:53.000000 danielutils-0.9.80/danielutils/versioned_imports.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:47:56.255010 danielutils-0.9.80/danielutils.egg-info/
--rw-rw-rw-   0        0        0     4593 2024-04-28 08:47:56.000000 danielutils-0.9.80/danielutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7689 2024-04-28 08:47:56.000000 danielutils-0.9.80/danielutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 08:47:56.000000 danielutils-0.9.80/danielutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-28 08:47:56.000000 danielutils-0.9.80/danielutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      977 2024-04-28 08:47:55.000000 danielutils-0.9.80/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-28 08:47:56.386866 danielutils-0.9.80/setup.cfg
--rw-rw-rw-   0        0        0       41 2024-04-28 08:47:48.000000 danielutils-0.9.80/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.209559 danielutils-0.9.81/
+-rw-rw-rw-   0        0        0     1091 2023-05-29 13:19:53.000000 danielutils-0.9.81/LICENSE
+-rw-rw-rw-   0        0        0       34 2024-05-01 12:37:28.000000 danielutils-0.9.81/MANIFEST.in
+-rw-rw-rw-   0        0        0     4593 2024-05-01 12:37:29.207969 danielutils-0.9.81/PKG-INFO
+-rw-rw-rw-   0        0        0     2650 2024-05-01 12:36:24.000000 danielutils-0.9.81/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.110352 danielutils-0.9.81/danielutils/
+-rw-rw-rw-   0        0        0     1399 2024-05-01 12:22:07.000000 danielutils-0.9.81/danielutils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.113358 danielutils-0.9.81/danielutils/abstractions/
+-rw-rw-rw-   0        0        0       77 2024-04-21 19:46:54.000000 danielutils-0.9.81/danielutils/abstractions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.116410 danielutils-0.9.81/danielutils/abstractions/database/
+-rw-rw-rw-   0        0        0       57 2024-04-21 18:12:14.000000 danielutils-0.9.81/danielutils/abstractions/database/__init__.py
+-rw-rw-rw-   0        0        0     2772 2024-04-17 20:37:10.000000 danielutils-0.9.81/danielutils/abstractions/database/cached_database.py
+-rw-rw-rw-   0        0        0     2621 2024-04-28 08:07:23.000000 danielutils-0.9.81/danielutils/abstractions/database/database.py
+-rw-rw-rw-   0        0        0     1048 2024-04-25 20:10:37.000000 danielutils-0.9.81/danielutils/abstractions/database/redis_database.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.118409 danielutils-0.9.81/danielutils/abstractions/multiprogramming/
+-rw-rw-rw-   0        0        0       74 2024-04-21 19:21:56.000000 danielutils-0.9.81/danielutils/abstractions/multiprogramming/__init__.py
+-rw-rw-rw-   0        0        0      374 2024-04-17 20:37:10.000000 danielutils-0.9.81/danielutils/abstractions/multiprogramming/multi_id.py
+-rw-rw-rw-   0        0        0     2392 2024-04-28 08:12:35.000000 danielutils-0.9.81/danielutils/abstractions/multiprogramming/worker.py
+-rw-rw-rw-   0        0        0     2412 2024-04-28 08:12:35.000000 danielutils-0.9.81/danielutils/abstractions/multiprogramming/worker_pool.py
+-rw-rw-rw-   0        0        0     3144 2024-04-28 08:12:35.000000 danielutils-0.9.81/danielutils/abstractions/repl.py
+-rw-rw-rw-   0        0        0     5663 2024-03-21 20:59:13.000000 danielutils-0.9.81/danielutils/aliases.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.119407 danielutils-0.9.81/danielutils/better_builtins/
+-rw-rw-rw-   0        0        0       78 2024-04-21 18:23:39.000000 danielutils-0.9.81/danielutils/better_builtins/__init__.py
+-rw-rw-rw-   0        0        0     1221 2024-03-21 20:59:13.000000 danielutils-0.9.81/danielutils/better_builtins/counter.py
+-rw-rw-rw-   0        0        0     7174 2024-04-21 18:12:40.000000 danielutils-0.9.81/danielutils/better_builtins/frange.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.123340 danielutils-0.9.81/danielutils/better_builtins/typed_builtins/
+-rw-rw-rw-   0        0        0       88 2024-03-21 20:59:13.000000 danielutils-0.9.81/danielutils/better_builtins/typed_builtins/__init__.py
+-rw-rw-rw-   0        0        0     4704 2024-04-28 08:12:35.000000 danielutils-0.9.81/danielutils/better_builtins/typed_builtins/factory.py
+-rw-rw-rw-   0        0        0      913 2024-03-21 20:59:13.000000 danielutils-0.9.81/danielutils/better_builtins/typed_builtins/tdict.py
+-rw-rw-rw-   0        0        0     7210 2024-04-28 08:12:13.000000 danielutils-0.9.81/danielutils/better_builtins/typed_builtins/tlist.py
+-rw-rw-rw-   0        0        0     2031 2024-03-21 20:59:13.000000 danielutils-0.9.81/danielutils/better_builtins/typed_builtins/tset.py
+-rw-rw-rw-   0        0        0      294 2024-03-21 20:59:13.000000 danielutils-0.9.81/danielutils/better_builtins/typed_builtins/ttuple.py
+-rw-rw-rw-   0        0        0     5472 2024-04-28 08:19:09.000000 danielutils-0.9.81/danielutils/colors.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.124337 danielutils-0.9.81/danielutils/context_managers/
+-rw-rw-rw-   0        0        0       29 2024-05-01 12:22:06.000000 danielutils-0.9.81/danielutils/context_managers/__init__.py
+-rw-rw-rw-   0        0        0      810 2024-05-01 12:22:06.000000 danielutils-0.9.81/danielutils/context_managers/temporary_file.py
+-rw-rw-rw-   0        0        0      210 2024-03-21 20:59:13.000000 danielutils-0.9.81/danielutils/convenience.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.126404 danielutils-0.9.81/danielutils/conversions/
+-rw-rw-rw-   0        0        0       73 2024-03-21 20:59:13.000000 danielutils-0.9.81/danielutils/conversions/__init__.py
+-rw-rw-rw-   0        0        0     2362 2024-04-28 08:19:08.000000 danielutils-0.9.81/danielutils/conversions/main_conversions.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.127401 danielutils-0.9.81/danielutils/conversions/specialized_conversions/
+-rw-rw-rw-   0        0        0       46 2024-03-21 20:59:13.000000 danielutils-0.9.81/danielutils/conversions/specialized_conversions/__init__.py
+-rw-rw-rw-   0        0        0      507 2024-03-21 23:16:41.000000 danielutils-0.9.81/danielutils/conversions/specialized_conversions/to_hex.py
+-rw-rw-rw-   0        0        0      543 2024-04-28 08:12:13.000000 danielutils-0.9.81/danielutils/conversions/specialized_conversions/to_int.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.131337 danielutils-0.9.81/danielutils/data_structures/
+-rw-rw-rw-   0        0        0      163 2024-04-17 20:37:10.000000 danielutils-0.9.81/danielutils/data_structures/__init__.py
+-rw-rw-rw-   0        0        0     1224 2024-04-17 20:37:10.000000 danielutils-0.9.81/danielutils/data_structures/comparer.py
+-rw-rw-rw-   0        0        0      273 2024-04-17 20:37:10.000000 danielutils-0.9.81/danielutils/data_structures/default_dict.py
+-rw-rw-rw-   0        0        0      632 2023-09-25 13:19:42.000000 danielutils-0.9.81/danielutils/data_structures/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.134438 danielutils-0.9.81/danielutils/data_structures/graph/
+-rw-rw-rw-   0        0        0       97 2024-04-17 20:37:10.000000 danielutils-0.9.81/danielutils/data_structures/graph/__init__.py
+-rw-rw-rw-   0        0        0     2066 2024-04-18 18:33:41.000000 danielutils-0.9.81/danielutils/data_structures/graph/binary_node.py
+-rw-rw-rw-   0        0        0     6877 2024-04-28 08:12:24.000000 danielutils-0.9.81/danielutils/data_structures/graph/graph.py
+-rw-rw-rw-   0        0        0     3141 2024-04-28 08:12:13.000000 danielutils-0.9.81/danielutils/data_structures/graph/multinode.py
+-rw-rw-rw-   0        0        0     1647 2024-03-28 19:42:06.000000 danielutils-0.9.81/danielutils/data_structures/graph/node.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.136444 danielutils-0.9.81/danielutils/data_structures/heap/
+-rw-rw-rw-   0        0        0       71 2024-03-28 19:45:24.000000 danielutils-0.9.81/danielutils/data_structures/heap/__init__.py
+-rw-rw-rw-   0        0        0     3092 2024-04-17 20:37:10.000000 danielutils-0.9.81/danielutils/data_structures/heap/heap.py
+-rw-rw-rw-   0        0        0      292 2024-03-28 19:45:24.000000 danielutils-0.9.81/danielutils/data_structures/heap/max_heap.py
+-rw-rw-rw-   0        0        0      300 2024-03-28 19:45:24.000000 danielutils-0.9.81/danielutils/data_structures/heap/min_heap.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.138663 danielutils-0.9.81/danielutils/data_structures/queue/
+-rw-rw-rw-   0        0        0       82 2024-03-28 19:35:07.000000 danielutils-0.9.81/danielutils/data_structures/queue/__init__.py
+-rw-rw-rw-   0        0        0      260 2024-03-28 19:35:13.000000 danielutils-0.9.81/danielutils/data_structures/queue/atomic_queue.py
+-rw-rw-rw-   0        0        0     3661 2024-03-28 19:35:07.000000 danielutils-0.9.81/danielutils/data_structures/queue/priority_queue.py
+-rw-rw-rw-   0        0        0     1615 2024-04-28 08:12:13.000000 danielutils-0.9.81/danielutils/data_structures/queue/queue.py
+-rw-rw-rw-   0        0        0     2143 2024-04-17 20:37:10.000000 danielutils-0.9.81/danielutils/data_structures/stack.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.140287 danielutils-0.9.81/danielutils/data_structures/trees/
+-rw-rw-rw-   0        0        0       63 2024-04-17 20:37:10.000000 danielutils-0.9.81/danielutils/data_structures/trees/__init__.py
+-rw-rw-rw-   0        0        0     2636 2024-04-28 08:12:00.000000 danielutils-0.9.81/danielutils/data_structures/trees/binary_syntax_tree.py
+-rw-rw-rw-   0        0        0     1618 2024-04-18 18:33:41.000000 danielutils-0.9.81/danielutils/data_structures/trees/binary_tree.py
+-rw-rw-rw-   0        0        0      675 2024-04-28 08:19:08.000000 danielutils-0.9.81/danielutils/date.py
+-rw-rw-rw-   0        0        0      232 2023-08-07 20:06:13.000000 danielutils-0.9.81/danielutils/date_time.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.151342 danielutils-0.9.81/danielutils/decorators/
+-rw-rw-rw-   0        0        0      466 2024-04-25 20:44:13.000000 danielutils-0.9.81/danielutils/decorators/__init__.py
+-rw-rw-rw-   0        0        0      756 2024-04-28 08:19:08.000000 danielutils-0.9.81/danielutils/decorators/atomic.py
+-rw-rw-rw-   0        0        0     1385 2024-04-28 08:19:08.000000 danielutils-0.9.81/danielutils/decorators/attach.py
+-rw-rw-rw-   0        0        0      730 2024-03-21 20:59:13.000000 danielutils-0.9.81/danielutils/decorators/chain_decorators.py
+-rw-rw-rw-   0        0        0     1089 2024-04-28 08:19:08.000000 danielutils-0.9.81/danielutils/decorators/decorate_conditionally.py
+-rw-rw-rw-   0        0        0     1008 2024-04-27 18:49:37.000000 danielutils-0.9.81/danielutils/decorators/delay_call.py
+-rw-rw-rw-   0        0        0     1290 2024-04-27 18:48:35.000000 danielutils-0.9.81/danielutils/decorators/deprecate.py
+-rw-rw-rw-   0        0        0     1023 2024-04-25 20:44:13.000000 danielutils-0.9.81/danielutils/decorators/final.py
+-rw-rw-rw-   0        0        0     1696 2024-04-28 08:19:08.000000 danielutils-0.9.81/danielutils/decorators/limit_recursion.py
+-rw-rw-rw-   0        0        0      806 2024-04-28 08:19:08.000000 danielutils-0.9.81/danielutils/decorators/memo.py
+-rw-rw-rw-   0        0        0     7521 2024-04-28 08:13:16.000000 danielutils-0.9.81/danielutils/decorators/overload.py
+-rw-rw-rw-   0        0        0      837 2024-04-28 08:19:09.000000 danielutils-0.9.81/danielutils/decorators/partially_implemented.py
+-rw-rw-rw-   0        0        0     1716 2024-04-21 19:46:04.000000 danielutils-0.9.81/danielutils/decorators/processify.py
+-rw-rw-rw-   0        0        0     1095 2024-03-21 20:59:13.000000 danielutils-0.9.81/danielutils/decorators/property.py
+-rw-rw-rw-   0        0        0      776 2024-04-17 20:37:10.000000 danielutils-0.9.81/danielutils/decorators/singleton.py
+-rw-rw-rw-   0        0        0      729 2024-04-27 18:49:28.000000 danielutils-0.9.81/danielutils/decorators/threadify.py
+-rw-rw-rw-   0        0        0     1998 2024-04-28 08:19:08.000000 danielutils-0.9.81/danielutils/decorators/timeout.py
+-rw-rw-rw-   0        0        0     3746 2024-04-28 08:13:33.000000 danielutils-0.9.81/danielutils/decorators/total_ordering.py
+-rw-rw-rw-   0        0        0     9556 2024-04-28 08:19:08.000000 danielutils-0.9.81/danielutils/decorators/validate.py
+-rw-rw-rw-   0        0        0     2163 2024-03-21 20:59:13.000000 danielutils-0.9.81/danielutils/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.157779 danielutils-0.9.81/danielutils/functions/
+-rw-rw-rw-   0        0        0      235 2024-04-21 19:19:56.000000 danielutils-0.9.81/danielutils/functions/__init__.py
+-rw-rw-rw-   0        0        0     1085 2024-04-28 08:12:35.000000 danielutils-0.9.81/danielutils/functions/areoneof.py
+-rw-rw-rw-   0        0        0      638 2024-03-21 20:59:13.000000 danielutils-0.9.81/danielutils/functions/check_foreach.py
+-rw-rw-rw-   0        0        0      791 2024-04-21 19:19:56.000000 danielutils-0.9.81/danielutils/functions/flatten.py
+-rw-rw-rw-   0        0        0    10122 2024-04-28 08:10:10.000000 danielutils-0.9.81/danielutils/functions/isoftype.py
+-rw-rw-rw-   0        0        0     1582 2024-04-28 08:12:35.000000 danielutils-0.9.81/danielutils/functions/isoneof.py
+-rw-rw-rw-   0        0        0     1292 2024-04-28 08:07:23.000000 danielutils-0.9.81/danielutils/functions/multiloop.py
+-rw-rw-rw-   0        0        0      639 2024-03-21 20:59:13.000000 danielutils-0.9.81/danielutils/functions/powerset.py
+-rw-rw-rw-   0        0        0      288 2024-03-21 20:59:13.000000 danielutils-0.9.81/danielutils/functions/subseteq.py
+-rw-rw-rw-   0        0        0     1008 2024-04-28 08:12:24.000000 danielutils-0.9.81/danielutils/functions/types_subseteq.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.160287 danielutils-0.9.81/danielutils/generators/
+-rw-rw-rw-   0        0        0      108 2024-03-21 20:59:13.000000 danielutils-0.9.81/danielutils/generators/__init__.py
+-rw-rw-rw-   0        0        0     1285 2024-03-21 20:59:13.000000 danielutils-0.9.81/danielutils/generators/conditional_generator.py
+-rw-rw-rw-   0        0        0      478 2024-04-28 08:19:09.000000 danielutils-0.9.81/danielutils/generators/generator_from_stream.py
+-rw-rw-rw-   0        0        0     2859 2024-04-28 08:12:35.000000 danielutils-0.9.81/danielutils/generators/join_generators.py
+-rw-rw-rw-   0        0        0     2105 2024-04-28 08:19:08.000000 danielutils-0.9.81/danielutils/internet.py
+-rw-rw-rw-   0        0        0    12329 2024-04-28 08:19:14.000000 danielutils-0.9.81/danielutils/io_.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.163293 danielutils-0.9.81/danielutils/math_/
+-rw-rw-rw-   0        0        0       79 2024-04-21 18:05:24.000000 danielutils-0.9.81/danielutils/math_/__init__.py
+-rw-rw-rw-   0        0        0     7682 2024-03-21 20:59:13.000000 danielutils-0.9.81/danielutils/math_/constants.py
+-rw-rw-rw-   0        0        0      642 2024-04-28 08:19:09.000000 danielutils-0.9.81/danielutils/math_/functions.py
+-rw-rw-rw-   0        0        0     1063 2024-04-21 18:05:24.000000 danielutils-0.9.81/danielutils/math_/math_print.py
+-rw-rw-rw-   0        0        0     4044 2024-04-28 08:12:00.000000 danielutils-0.9.81/danielutils/math_/math_symbols.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.164295 danielutils-0.9.81/danielutils/math_/polynomial/
+-rw-rw-rw-   0        0        0       25 2024-04-21 18:05:24.000000 danielutils-0.9.81/danielutils/math_/polynomial/__init__.py
+-rw-rw-rw-   0        0        0      835 2024-04-28 08:12:13.000000 danielutils-0.9.81/danielutils/math_/polynomial/polinomial.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.167841 danielutils-0.9.81/danielutils/metaclasses/
+-rw-rw-rw-   0        0        0      169 2024-03-21 23:16:41.000000 danielutils-0.9.81/danielutils/metaclasses/__init__.py
+-rw-rw-rw-   0        0        0      695 2024-03-21 20:59:13.000000 danielutils-0.9.81/danielutils/metaclasses/atomic_class_meta.py
+-rw-rw-rw-   0        0        0     2511 2024-03-21 20:59:13.000000 danielutils-0.9.81/danielutils/metaclasses/implicit_data_deleter_meta.py
+-rw-rw-rw-   0        0        0     1495 2024-04-21 18:13:57.000000 danielutils-0.9.81/danielutils/metaclasses/instance_cache_meta.py
+-rw-rw-rw-   0        0        0    10932 2024-04-28 08:12:24.000000 danielutils-0.9.81/danielutils/metaclasses/interface.py
+-rw-rw-rw-   0        0        0     1754 2024-03-21 20:59:13.000000 danielutils-0.9.81/danielutils/metaclasses/overload_meta.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.169840 danielutils-0.9.81/danielutils/mock_/
+-rw-rw-rw-   0        0        0       58 2024-04-21 18:12:14.000000 danielutils-0.9.81/danielutils/mock_/__init__.py
+-rw-rw-rw-   0        0        0     2017 2024-04-21 19:46:04.000000 danielutils-0.9.81/danielutils/mock_/mock_database.py
+-rw-rw-rw-   0        0        0      419 2024-04-17 20:37:10.000000 danielutils-0.9.81/danielutils/mock_/mock_module.py
+-rw-rw-rw-   0        0        0     1032 2024-03-21 20:59:13.000000 danielutils-0.9.81/danielutils/path.py
+-rw-rw-rw-   0        0        0     2801 2024-04-21 18:05:24.000000 danielutils-0.9.81/danielutils/print_.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.171221 danielutils-0.9.81/danielutils/protocols/
+-rw-rw-rw-   0        0        0       49 2024-04-17 20:37:10.000000 danielutils-0.9.81/danielutils/protocols/__init__.py
+-rw-rw-rw-   0        0        0      446 2024-04-28 08:12:00.000000 danielutils-0.9.81/danielutils/protocols/dictable.py
+-rw-rw-rw-   0        0        0      203 2024-04-17 20:37:10.000000 danielutils-0.9.81/danielutils/protocols/evaluable.py
+-rw-rw-rw-   0        0        0        0 2023-08-09 09:08:58.000000 danielutils-0.9.81/danielutils/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.172373 danielutils-0.9.81/danielutils/reflection/
+-rw-rw-rw-   0        0        0     1516 2024-04-21 18:21:37.000000 danielutils-0.9.81/danielutils/reflection/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.173372 danielutils-0.9.81/danielutils/reflection/class_/
+-rw-rw-rw-   0        0        0       31 2024-04-21 18:21:37.000000 danielutils-0.9.81/danielutils/reflection/class_/__init__.py
+-rw-rw-rw-   0        0        0     5507 2024-04-28 08:12:35.000000 danielutils-0.9.81/danielutils/reflection/class_/class_reflection.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.174372 danielutils-0.9.81/danielutils/reflection/file/
+-rw-rw-rw-   0        0        0       30 2024-04-21 18:21:37.000000 danielutils-0.9.81/danielutils/reflection/file/__init__.py
+-rw-rw-rw-   0        0        0     1657 2024-04-27 18:35:37.000000 danielutils-0.9.81/danielutils/reflection/file/file_reflection.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.175372 danielutils-0.9.81/danielutils/reflection/function/
+-rw-rw-rw-   0        0        0       35 2024-04-21 18:21:37.000000 danielutils-0.9.81/danielutils/reflection/function/__init__.py
+-rw-rw-rw-   0        0        0     4453 2024-04-28 08:12:24.000000 danielutils-0.9.81/danielutils/reflection/function/function_reflections.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.180699 danielutils-0.9.81/danielutils/reflection/interpreter/
+-rw-rw-rw-   0        0        0      179 2024-04-21 19:19:56.000000 danielutils-0.9.81/danielutils/reflection/interpreter/__init__.py
+-rw-rw-rw-   0        0        0     1074 2024-04-25 20:37:30.000000 danielutils-0.9.81/danielutils/reflection/interpreter/callstack.py
+-rw-rw-rw-   0        0        0      441 2024-04-28 08:12:13.000000 danielutils-0.9.81/danielutils/reflection/interpreter/get_traceback.py
+-rw-rw-rw-   0        0        0      622 2024-04-17 20:37:10.000000 danielutils-0.9.81/danielutils/reflection/interpreter/os_.py
+-rw-rw-rw-   0        0        0     1023 2024-04-17 20:37:10.000000 danielutils-0.9.81/danielutils/reflection/interpreter/packages.py
+-rw-rw-rw-   0        0        0      621 2024-04-28 08:12:35.000000 danielutils-0.9.81/danielutils/reflection/interpreter/python_version.py
+-rw-rw-rw-   0        0        0      489 2024-03-21 20:59:13.000000 danielutils-0.9.81/danielutils/reflection/interpreter/signals.py
+-rw-rw-rw-   0        0        0     5733 2024-04-28 08:12:24.000000 danielutils-0.9.81/danielutils/reflection/interpreter/tracer.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.181742 danielutils-0.9.81/danielutils/reflection/module/
+-rw-rw-rw-   0        0        0       68 2024-04-21 18:27:13.000000 danielutils-0.9.81/danielutils/reflection/module/__init__.py
+-rw-rw-rw-   0        0        0      507 2024-03-21 20:59:13.000000 danielutils-0.9.81/danielutils/reflection/module/module_reflections.py
+-rw-rw-rw-   0        0        0     4714 2024-04-28 08:12:24.000000 danielutils-0.9.81/danielutils/reflection/module/package_reflection.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.183742 danielutils-0.9.81/danielutils/snippets/
+-rw-rw-rw-   0        0        0       24 2024-03-21 20:59:13.000000 danielutils-0.9.81/danielutils/snippets/__init__.py
+-rw-rw-rw-   0        0        0      433 2024-03-21 20:59:13.000000 danielutils-0.9.81/danielutils/snippets/try_get.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.184742 danielutils-0.9.81/danielutils/system/
+-rw-rw-rw-   0        0        0       84 2024-05-01 12:22:07.000000 danielutils-0.9.81/danielutils/system/__init__.py
+-rw-rw-rw-   0        0        0     6863 2024-04-28 08:19:08.000000 danielutils-0.9.81/danielutils/system/independent.py
+-rw-rw-rw-   0        0        0     3680 2024-05-01 12:27:27.000000 danielutils-0.9.81/danielutils/system/layered_command.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.186785 danielutils-0.9.81/danielutils/system/windows/
+-rw-rw-rw-   0        0        0       50 2024-03-21 20:59:13.000000 danielutils-0.9.81/danielutils/system/windows/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.187786 danielutils-0.9.81/danielutils/system/windows/utils/
+-rw-rw-rw-   0        0        0       25 2024-03-21 20:59:13.000000 danielutils-0.9.81/danielutils/system/windows/utils/__init__.py
+-rw-rw-rw-   0        0        0      499 2024-04-17 20:37:10.000000 danielutils-0.9.81/danielutils/system/windows/utils/filetime.py
+-rw-rw-rw-   0        0        0     6064 2024-03-21 20:59:13.000000 danielutils-0.9.81/danielutils/system/windows/win32_ctime.py
+-rw-rw-rw-   0        0        0     2253 2024-03-21 20:59:13.000000 danielutils-0.9.81/danielutils/system/windows/windows.py
+-rw-rw-rw-   0        0        0     4213 2024-04-28 08:19:08.000000 danielutils-0.9.81/danielutils/text.py
+-rw-rw-rw-   0        0        0     1225 2024-04-27 18:53:17.000000 danielutils-0.9.81/danielutils/time.py
+-rw-rw-rw-   0        0        0     1723 2024-04-28 08:12:13.000000 danielutils-0.9.81/danielutils/tqdm_.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.188785 danielutils-0.9.81/danielutils/university/
+-rw-rw-rw-   0        0        0       74 2024-04-17 20:37:10.000000 danielutils-0.9.81/danielutils/university/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.189785 danielutils-0.9.81/danielutils/university/databases/
+-rw-rw-rw-   0        0        0       20 2024-03-21 20:59:13.000000 danielutils-0.9.81/danielutils/university/databases/__init__.py
+-rw-rw-rw-   0        0        0    24890 2024-04-28 08:12:35.000000 danielutils-0.9.81/danielutils/university/databases/all.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.191089 danielutils-0.9.81/danielutils/university/oop/
+-rw-rw-rw-   0        0        0       25 2024-04-17 20:37:10.000000 danielutils-0.9.81/danielutils/university/oop/__init__.py
+-rw-rw-rw-   0        0        0      802 2024-04-28 08:13:50.000000 danielutils-0.9.81/danielutils/university/oop/observer.py
+-rw-rw-rw-   0        0        0       87 2024-04-17 20:37:10.000000 danielutils-0.9.81/danielutils/university/oop/strategy.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.194729 danielutils-0.9.81/danielutils/university/probability/
+-rw-rw-rw-   0        0        0      189 2024-04-21 22:41:40.000000 danielutils-0.9.81/danielutils/university/probability/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.197050 danielutils-0.9.81/danielutils/university/probability/conditional_variable/
+-rw-rw-rw-   0        0        0       89 2024-04-17 20:37:10.000000 danielutils-0.9.81/danielutils/university/probability/conditional_variable/__init__.py
+-rw-rw-rw-   0        0        0     4004 2024-04-25 21:21:07.000000 danielutils-0.9.81/danielutils/university/probability/conditional_variable/conditional_variable.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.197050 danielutils-0.9.81/danielutils/university/probability/conditional_variable/continuous/
+-rw-rw-rw-   0        0        0        0 2024-04-17 20:37:10.000000 danielutils-0.9.81/danielutils/university/probability/conditional_variable/continuous/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.202074 danielutils-0.9.81/danielutils/university/probability/conditional_variable/discrete/
+-rw-rw-rw-   0        0        0      209 2024-04-17 20:37:10.000000 danielutils-0.9.81/danielutils/university/probability/conditional_variable/discrete/__init__.py
+-rw-rw-rw-   0        0        0     1149 2024-04-21 22:51:43.000000 danielutils-0.9.81/danielutils/university/probability/conditional_variable/discrete/bernoulli.py
+-rw-rw-rw-   0        0        0     1257 2024-04-21 22:51:43.000000 danielutils-0.9.81/danielutils/university/probability/conditional_variable/discrete/binomial.py
+-rw-rw-rw-   0        0        0     1108 2024-04-21 22:51:43.000000 danielutils-0.9.81/danielutils/university/probability/conditional_variable/discrete/conditional_from_discrete_probability_func.py
+-rw-rw-rw-   0        0        0     1370 2024-04-21 22:51:43.000000 danielutils-0.9.81/danielutils/university/probability/conditional_variable/discrete/discrete.py
+-rw-rw-rw-   0        0        0     1652 2024-04-28 08:12:35.000000 danielutils-0.9.81/danielutils/university/probability/conditional_variable/discrete/geometric.py
+-rw-rw-rw-   0        0        0      992 2024-04-21 22:51:43.000000 danielutils-0.9.81/danielutils/university/probability/conditional_variable/discrete/poisson.py
+-rw-rw-rw-   0        0        0     1040 2024-04-21 22:51:43.000000 danielutils-0.9.81/danielutils/university/probability/conditional_variable/discrete/uniform.py
+-rw-rw-rw-   0        0        0      904 2024-04-21 22:41:40.000000 danielutils-0.9.81/danielutils/university/probability/distributions.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.204963 danielutils-0.9.81/danielutils/university/probability/expressions/
+-rw-rw-rw-   0        0        0       79 2024-04-17 22:49:00.000000 danielutils-0.9.81/danielutils/university/probability/expressions/__init__.py
+-rw-rw-rw-   0        0        0     7439 2024-04-25 21:20:42.000000 danielutils-0.9.81/danielutils/university/probability/expressions/accumulation_expression.py
+-rw-rw-rw-   0        0        0     4391 2024-04-25 21:20:53.000000 danielutils-0.9.81/danielutils/university/probability/expressions/probability_expression.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.207969 danielutils-0.9.81/danielutils/university/probability/funcs/
+-rw-rw-rw-   0        0        0      120 2024-04-17 20:37:10.000000 danielutils-0.9.81/danielutils/university/probability/funcs/__init__.py
+-rw-rw-rw-   0        0        0      338 2024-04-21 22:41:40.000000 danielutils-0.9.81/danielutils/university/probability/funcs/covariance.py
+-rw-rw-rw-   0        0        0     1173 2024-04-21 22:41:40.000000 danielutils-0.9.81/danielutils/university/probability/funcs/expected_value.py
+-rw-rw-rw-   0        0        0      306 2024-04-17 20:37:10.000000 danielutils-0.9.81/danielutils/university/probability/funcs/probability_function.py
+-rw-rw-rw-   0        0        0      437 2024-04-21 22:41:40.000000 danielutils-0.9.81/danielutils/university/probability/funcs/variance.py
+-rw-rw-rw-   0        0        0     1987 2024-04-28 08:12:24.000000 danielutils-0.9.81/danielutils/university/probability/operator.py
+-rw-rw-rw-   0        0        0      641 2024-04-18 18:33:41.000000 danielutils-0.9.81/danielutils/university/probability/protocols.py
+-rw-rw-rw-   0        0        0     2055 2024-04-21 22:51:43.000000 danielutils-0.9.81/danielutils/university/probability/supp.py
+-rw-rw-rw-   0        0        0     1182 2024-04-25 20:08:45.000000 danielutils-0.9.81/danielutils/university/probability/transformation.py
+-rw-rw-rw-   0        0        0      322 2024-04-28 08:07:53.000000 danielutils-0.9.81/danielutils/versioned_imports.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:37:29.112356 danielutils-0.9.81/danielutils.egg-info/
+-rw-rw-rw-   0        0        0     4593 2024-05-01 12:37:28.000000 danielutils-0.9.81/danielutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7815 2024-05-01 12:37:29.000000 danielutils-0.9.81/danielutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 12:37:28.000000 danielutils-0.9.81/danielutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-01 12:37:28.000000 danielutils-0.9.81/danielutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      977 2024-05-01 12:37:28.000000 danielutils-0.9.81/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-01 12:37:29.209559 danielutils-0.9.81/setup.cfg
+-rw-rw-rw-   0        0        0       41 2024-05-01 12:37:28.000000 danielutils-0.9.81/setup.py
```

### Comparing `danielutils-0.9.80/LICENSE` & `danielutils-0.9.81/LICENSE`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/PKG-INFO` & `danielutils-0.9.81/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danielutils
-Version: 0.9.80
+Version: 0.9.81
 Summary: A python utils library for things I find useful
 Author-email: danielnachumdev <danielnachumdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 danielnachumdev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,15 +37,15 @@
 
 
 [![Python package](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml)
 [![Pylint](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml)
 [![Python 3.10.11](https://img.shields.io/badge/python-3.10.11-blue.svg)](https://www.python.org/downloads/release/python-31011/)
 [![gitleaks](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml)
 [![CodeQL](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql)
-# danielutils v=0.9.80
+# danielutils v=0.9.81
 A utils library for things that I find useful for my coding workflow.\
 Feel free to use and / or contribute / improve my code :)
 
 THIS PACKAGE IS IN DEVELOPMENT AND SUBJECT TO CHANGE, USE AT YOUR OWN RISK!
 
 **Tested python versions**: `3.8.0`*, `3.9.0`, `3.10.13`
```

### Comparing `danielutils-0.9.80/README.md` & `danielutils-0.9.81/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 [![Python package](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml)
 [![Pylint](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml)
 [![Python 3.10.11](https://img.shields.io/badge/python-3.10.11-blue.svg)](https://www.python.org/downloads/release/python-31011/)
 [![gitleaks](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml)
 [![CodeQL](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql)
-# danielutils v=0.9.80
+# danielutils v=0.9.81
 A utils library for things that I find useful for my coding workflow.\
 Feel free to use and / or contribute / improve my code :)
 
 THIS PACKAGE IS IN DEVELOPMENT AND SUBJECT TO CHANGE, USE AT YOUR OWN RISK!
 
 **Tested python versions**: `3.8.0`*, `3.9.0`, `3.10.13`
```

### Comparing `danielutils-0.9.80/danielutils/__init__.py` & `danielutils-0.9.81/danielutils/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,8 +35,9 @@
 from .data_structures import *
 from .math_ import *
 from .system import *
 from .print_ import *
 from .metaclasses import *
 from .generators import *
 from .university import *
-from .mock_ import *
+from .mock_ import *
+from .context_managers import *
```

### Comparing `danielutils-0.9.80/danielutils/abstractions/database/cached_database.py` & `danielutils-0.9.81/danielutils/abstractions/database/cached_database.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/abstractions/database/database.py` & `danielutils-0.9.81/danielutils/abstractions/database/database.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/abstractions/database/redis_database.py` & `danielutils-0.9.81/danielutils/abstractions/database/redis_database.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/abstractions/multiprogramming/worker.py` & `danielutils-0.9.81/danielutils/abstractions/multiprogramming/worker.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/abstractions/multiprogramming/worker_pool.py` & `danielutils-0.9.81/danielutils/abstractions/multiprogramming/worker_pool.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/abstractions/repl.py` & `danielutils-0.9.81/danielutils/abstractions/repl.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/aliases.py` & `danielutils-0.9.81/danielutils/aliases.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/better_builtins/counter.py` & `danielutils-0.9.81/danielutils/better_builtins/counter.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/better_builtins/frange.py` & `danielutils-0.9.81/danielutils/better_builtins/frange.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/better_builtins/typed_builtins/factory.py` & `danielutils-0.9.81/danielutils/better_builtins/typed_builtins/factory.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/better_builtins/typed_builtins/tdict.py` & `danielutils-0.9.81/danielutils/better_builtins/typed_builtins/tdict.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/better_builtins/typed_builtins/tlist.py` & `danielutils-0.9.81/danielutils/better_builtins/typed_builtins/tlist.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/better_builtins/typed_builtins/tset.py` & `danielutils-0.9.81/danielutils/better_builtins/typed_builtins/tset.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/colors.py` & `danielutils-0.9.81/danielutils/colors.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/conversions/main_conversions.py` & `danielutils-0.9.81/danielutils/conversions/main_conversions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/conversions/specialized_conversions/to_int.py` & `danielutils-0.9.81/danielutils/conversions/specialized_conversions/to_int.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/data_structures/comparer.py` & `danielutils-0.9.81/danielutils/data_structures/comparer.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/data_structures/functions.py` & `danielutils-0.9.81/danielutils/data_structures/functions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/data_structures/graph/binary_node.py` & `danielutils-0.9.81/danielutils/data_structures/graph/binary_node.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/data_structures/graph/graph.py` & `danielutils-0.9.81/danielutils/data_structures/graph/graph.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/data_structures/graph/multinode.py` & `danielutils-0.9.81/danielutils/data_structures/graph/multinode.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/data_structures/graph/node.py` & `danielutils-0.9.81/danielutils/data_structures/graph/node.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/data_structures/heap/heap.py` & `danielutils-0.9.81/danielutils/data_structures/heap/heap.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/data_structures/queue/priority_queue.py` & `danielutils-0.9.81/danielutils/data_structures/queue/priority_queue.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/data_structures/queue/queue.py` & `danielutils-0.9.81/danielutils/data_structures/queue/queue.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/data_structures/stack.py` & `danielutils-0.9.81/danielutils/data_structures/stack.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/data_structures/trees/binary_syntax_tree.py` & `danielutils-0.9.81/danielutils/data_structures/trees/binary_syntax_tree.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/data_structures/trees/binary_tree.py` & `danielutils-0.9.81/danielutils/data_structures/trees/binary_tree.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/date.py` & `danielutils-0.9.81/danielutils/date.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/decorators/atomic.py` & `danielutils-0.9.81/danielutils/decorators/atomic.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/decorators/attach.py` & `danielutils-0.9.81/danielutils/decorators/attach.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/decorators/chain_decorators.py` & `danielutils-0.9.81/danielutils/decorators/chain_decorators.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/decorators/decorate_conditionally.py` & `danielutils-0.9.81/danielutils/decorators/decorate_conditionally.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/decorators/delay_call.py` & `danielutils-0.9.81/danielutils/decorators/delay_call.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/decorators/deprecate.py` & `danielutils-0.9.81/danielutils/decorators/deprecate.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/decorators/final.py` & `danielutils-0.9.81/danielutils/decorators/final.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/decorators/limit_recursion.py` & `danielutils-0.9.81/danielutils/decorators/limit_recursion.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/decorators/memo.py` & `danielutils-0.9.81/danielutils/decorators/memo.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/decorators/overload.py` & `danielutils-0.9.81/danielutils/decorators/overload.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/decorators/partially_implemented.py` & `danielutils-0.9.81/danielutils/decorators/partially_implemented.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/decorators/processify.py` & `danielutils-0.9.81/danielutils/decorators/processify.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/decorators/property.py` & `danielutils-0.9.81/danielutils/decorators/property.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/decorators/singleton.py` & `danielutils-0.9.81/danielutils/decorators/singleton.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/decorators/threadify.py` & `danielutils-0.9.81/danielutils/decorators/threadify.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/decorators/timeout.py` & `danielutils-0.9.81/danielutils/decorators/timeout.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/decorators/total_ordering.py` & `danielutils-0.9.81/danielutils/decorators/total_ordering.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/decorators/validate.py` & `danielutils-0.9.81/danielutils/decorators/validate.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/exceptions.py` & `danielutils-0.9.81/danielutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/functions/areoneof.py` & `danielutils-0.9.81/danielutils/functions/areoneof.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/functions/check_foreach.py` & `danielutils-0.9.81/danielutils/functions/check_foreach.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/functions/flatten.py` & `danielutils-0.9.81/danielutils/functions/flatten.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/functions/isoftype.py` & `danielutils-0.9.81/danielutils/functions/isoftype.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/functions/isoneof.py` & `danielutils-0.9.81/danielutils/functions/isoneof.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/functions/multiloop.py` & `danielutils-0.9.81/danielutils/functions/multiloop.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/functions/powerset.py` & `danielutils-0.9.81/danielutils/functions/powerset.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/functions/types_subseteq.py` & `danielutils-0.9.81/danielutils/functions/types_subseteq.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/generators/conditional_generator.py` & `danielutils-0.9.81/danielutils/generators/conditional_generator.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/generators/join_generators.py` & `danielutils-0.9.81/danielutils/generators/join_generators.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/internet.py` & `danielutils-0.9.81/danielutils/internet.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/io_.py` & `danielutils-0.9.81/danielutils/io_.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/math_/constants.py` & `danielutils-0.9.81/danielutils/math_/constants.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/math_/functions.py` & `danielutils-0.9.81/danielutils/math_/functions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/math_/math_print.py` & `danielutils-0.9.81/danielutils/math_/math_print.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/math_/math_symbols.py` & `danielutils-0.9.81/danielutils/math_/math_symbols.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/math_/polynomial/polinomial.py` & `danielutils-0.9.81/danielutils/math_/polynomial/polinomial.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/metaclasses/atomic_class_meta.py` & `danielutils-0.9.81/danielutils/metaclasses/atomic_class_meta.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/metaclasses/implicit_data_deleter_meta.py` & `danielutils-0.9.81/danielutils/metaclasses/implicit_data_deleter_meta.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/metaclasses/instance_cache_meta.py` & `danielutils-0.9.81/danielutils/metaclasses/instance_cache_meta.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/metaclasses/interface.py` & `danielutils-0.9.81/danielutils/metaclasses/interface.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/metaclasses/overload_meta.py` & `danielutils-0.9.81/danielutils/metaclasses/overload_meta.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/mock_/mock_database.py` & `danielutils-0.9.81/danielutils/mock_/mock_database.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/path.py` & `danielutils-0.9.81/danielutils/path.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/print_.py` & `danielutils-0.9.81/danielutils/print_.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/reflection/__init__.py` & `danielutils-0.9.81/danielutils/reflection/__init__.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/reflection/class_/class_reflection.py` & `danielutils-0.9.81/danielutils/reflection/class_/class_reflection.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/reflection/file/file_reflection.py` & `danielutils-0.9.81/danielutils/reflection/file/file_reflection.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/reflection/function/function_reflections.py` & `danielutils-0.9.81/danielutils/reflection/function/function_reflections.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/reflection/interpreter/callstack.py` & `danielutils-0.9.81/danielutils/reflection/interpreter/callstack.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/reflection/interpreter/os_.py` & `danielutils-0.9.81/danielutils/reflection/interpreter/os_.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/reflection/interpreter/packages.py` & `danielutils-0.9.81/danielutils/reflection/interpreter/packages.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/reflection/interpreter/python_version.py` & `danielutils-0.9.81/danielutils/reflection/interpreter/python_version.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/reflection/interpreter/tracer.py` & `danielutils-0.9.81/danielutils/reflection/interpreter/tracer.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/reflection/module/package_reflection.py` & `danielutils-0.9.81/danielutils/reflection/module/package_reflection.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/system/independent.py` & `danielutils-0.9.81/danielutils/system/independent.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/system/windows/win32_ctime.py` & `danielutils-0.9.81/danielutils/system/windows/win32_ctime.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/system/windows/windows.py` & `danielutils-0.9.81/danielutils/system/windows/windows.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/text.py` & `danielutils-0.9.81/danielutils/text.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/time.py` & `danielutils-0.9.81/danielutils/time.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/tqdm_.py` & `danielutils-0.9.81/danielutils/tqdm_.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/university/databases/all.py` & `danielutils-0.9.81/danielutils/university/databases/all.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/university/oop/observer.py` & `danielutils-0.9.81/danielutils/university/oop/observer.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/university/probability/conditional_variable/conditional_variable.py` & `danielutils-0.9.81/danielutils/university/probability/conditional_variable/conditional_variable.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/university/probability/conditional_variable/discrete/bernoulli.py` & `danielutils-0.9.81/danielutils/university/probability/conditional_variable/discrete/bernoulli.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/university/probability/conditional_variable/discrete/binomial.py` & `danielutils-0.9.81/danielutils/university/probability/conditional_variable/discrete/binomial.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/university/probability/conditional_variable/discrete/conditional_from_discrete_probability_func.py` & `danielutils-0.9.81/danielutils/university/probability/conditional_variable/discrete/conditional_from_discrete_probability_func.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/university/probability/conditional_variable/discrete/discrete.py` & `danielutils-0.9.81/danielutils/university/probability/conditional_variable/discrete/discrete.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/university/probability/conditional_variable/discrete/geometric.py` & `danielutils-0.9.81/danielutils/university/probability/conditional_variable/discrete/geometric.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/university/probability/conditional_variable/discrete/poisson.py` & `danielutils-0.9.81/danielutils/university/probability/conditional_variable/discrete/poisson.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/university/probability/conditional_variable/discrete/uniform.py` & `danielutils-0.9.81/danielutils/university/probability/conditional_variable/discrete/uniform.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/university/probability/distributions.py` & `danielutils-0.9.81/danielutils/university/probability/distributions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/university/probability/expressions/accumulation_expression.py` & `danielutils-0.9.81/danielutils/university/probability/expressions/accumulation_expression.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/university/probability/expressions/probability_expression.py` & `danielutils-0.9.81/danielutils/university/probability/expressions/probability_expression.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/university/probability/funcs/expected_value.py` & `danielutils-0.9.81/danielutils/university/probability/funcs/expected_value.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/university/probability/operator.py` & `danielutils-0.9.81/danielutils/university/probability/operator.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/university/probability/protocols.py` & `danielutils-0.9.81/danielutils/university/probability/protocols.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/university/probability/supp.py` & `danielutils-0.9.81/danielutils/university/probability/supp.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils/university/probability/transformation.py` & `danielutils-0.9.81/danielutils/university/probability/transformation.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.80/danielutils.egg-info/PKG-INFO` & `danielutils-0.9.81/danielutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danielutils
-Version: 0.9.80
+Version: 0.9.81
 Summary: A python utils library for things I find useful
 Author-email: danielnachumdev <danielnachumdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 danielnachumdev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,15 +37,15 @@
 
 
 [![Python package](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml)
 [![Pylint](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml)
 [![Python 3.10.11](https://img.shields.io/badge/python-3.10.11-blue.svg)](https://www.python.org/downloads/release/python-31011/)
 [![gitleaks](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml)
 [![CodeQL](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql)
-# danielutils v=0.9.80
+# danielutils v=0.9.81
 A utils library for things that I find useful for my coding workflow.\
 Feel free to use and / or contribute / improve my code :)
 
 THIS PACKAGE IS IN DEVELOPMENT AND SUBJECT TO CHANGE, USE AT YOUR OWN RISK!
 
 **Tested python versions**: `3.8.0`*, `3.9.0`, `3.10.13`
```

### Comparing `danielutils-0.9.80/danielutils.egg-info/SOURCES.txt` & `danielutils-0.9.81/danielutils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 danielutils/better_builtins/frange.py
 danielutils/better_builtins/typed_builtins/__init__.py
 danielutils/better_builtins/typed_builtins/factory.py
 danielutils/better_builtins/typed_builtins/tdict.py
 danielutils/better_builtins/typed_builtins/tlist.py
 danielutils/better_builtins/typed_builtins/tset.py
 danielutils/better_builtins/typed_builtins/ttuple.py
+danielutils/context_managers/__init__.py
+danielutils/context_managers/temporary_file.py
 danielutils/conversions/__init__.py
 danielutils/conversions/main_conversions.py
 danielutils/conversions/specialized_conversions/__init__.py
 danielutils/conversions/specialized_conversions/to_hex.py
 danielutils/conversions/specialized_conversions/to_int.py
 danielutils/data_structures/__init__.py
 danielutils/data_structures/comparer.py
@@ -138,14 +140,15 @@
 danielutils/reflection/module/__init__.py
 danielutils/reflection/module/module_reflections.py
 danielutils/reflection/module/package_reflection.py
 danielutils/snippets/__init__.py
 danielutils/snippets/try_get.py
 danielutils/system/__init__.py
 danielutils/system/independent.py
+danielutils/system/layered_command.py
 danielutils/system/windows/__init__.py
 danielutils/system/windows/win32_ctime.py
 danielutils/system/windows/windows.py
 danielutils/system/windows/utils/__init__.py
 danielutils/system/windows/utils/filetime.py
 danielutils/university/__init__.py
 danielutils/university/databases/__init__.py
```

### Comparing `danielutils-0.9.80/pyproject.toml` & `danielutils-0.9.81/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "danielutils"
-version = "0.9.80"
+version = "0.9.81"
 authors = [
     { name = "danielnachumdev", email = "danielnachumdev@gmail.com" },
 ]
 dependencies = []
 keywords = ['functions', 'decorators', 'methods', 'better_builtins', 'metaclasses']
 license = { "file" = "./LICENSE" }
 description = "A python utils library for things I find useful"
```

