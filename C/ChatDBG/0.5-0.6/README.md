# Comparing `tmp/chatdbg-0.5.tar.gz` & `tmp/chatdbg-0.6.tar.gz`

## Comparing `chatdbg-0.5.tar` & `chatdbg-0.6.tar`

### file list

```diff
@@ -1,85 +1,197 @@
--rw-r--r--   0        0        0   431302 2020-02-02 00:00:00.000000 chatdbg-0.5/ChatDBG-arxiv-2403.16354.pdf
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 chatdbg-0.5/.github/workflows/release.yml
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 chatdbg-0.5/.github/workflows/sanity.yml
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 chatdbg-0.5/rust-support/Cargo.toml
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 chatdbg-0.5/rust-support/chatdbg/Cargo.toml
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 chatdbg-0.5/rust-support/chatdbg/src/lib.rs
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 chatdbg-0.5/rust-support/chatdbg_macros/Cargo.toml
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 chatdbg-0.5/rust-support/chatdbg_macros/src/lib.rs
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/__init__.py
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/__main__.py
--rw-r--r--   0        0        0     4314 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/chatdbg_gdb.py
--rw-r--r--   0        0        0    10060 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/chatdbg_lldb.py
--rw-r--r--   0        0        0    22964 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/chatdbg_pdb.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/assistant/__init__.py
--rw-r--r--   0        0        0    12775 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/assistant/assistant.py
--rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/assistant/listeners.py
--rw-r--r--   0        0        0     6728 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/native_util/clangd_lsp_integration.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/native_util/code.py
--rw-r--r--   0        0        0     8074 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/native_util/dbg_dialog.py
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/native_util/stacks.py
--rw-r--r--   0        0        0     5267 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/old_stuff/chatdbg_utils.py
--rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/old_stuff/gdb_print_test.py
--rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/old_stuff/lldb_print_test.py
--rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/old_stuff/lldb_why.py
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/old_stuff/prompts.py
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/pdb/prompts.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/pdb/text.py
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/pdb_util/capture.py
--rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/pdb_util/locals.py
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/pdb_util/paths.py
--rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/util/config.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/util/history.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/util/instructions.txt
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/util/jupyter.py
--rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/util/log.py
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/util/markdown.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/util/plog.py
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/util/printer.py
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/util/prompts.py
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/util/stream.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/util/text.py
--rw-r--r--   0        0        0     3835 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/util/trim.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/util/wrap.py
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/windbg/CMakeLists.txt
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/windbg/build-chatdbg.bat
--rw-r--r--   0        0        0    11421 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/windbg/chatdbg.cpp
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/windbg/vcpkg-configuration.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/windbg/vcpkg.json
--rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/windbg/include/appendlines.hpp
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/windbg/include/getmodel.hpp
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/windbg/include/joinstrings.hpp
--rw-r--r--   0        0        0    25429 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/windbg/include/openai.hpp
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/windbg/include/wordwrap.hpp
--rw-r--r--   0        0        0   915040 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/windbg/nlohmann/json.hpp
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 chatdbg-0.5/test/test-deep-recursion.cpp
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 chatdbg-0.5/test/test-definition-likely.cpp
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 chatdbg-0.5/test/test-failed-assert.cpp
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 chatdbg-0.5/test/test-failed-assert.why.txt
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 chatdbg-0.5/test/test-overflow.cpp
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 chatdbg-0.5/test/test-overflow.why.txt
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 chatdbg-0.5/test/test-pointers-loop.cpp
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 chatdbg-0.5/test/test-pointers.cpp
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 chatdbg-0.5/test/test-stack-overflow.cpp
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 chatdbg-0.5/test/test-stack-overflow.why.txt
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 chatdbg-0.5/test/test-use-after-free.cpp
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 chatdbg-0.5/test/test-use-after-free.why.txt
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 chatdbg-0.5/test/testme.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 chatdbg-0.5/test/python/README.md
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 chatdbg-0.5/test/python/bootstrap.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 chatdbg-0.5/test/python/bootstrap2.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 chatdbg-0.5/test/python/ds101.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 chatdbg-0.5/test/python/marble-sample.csv
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 chatdbg-0.5/test/python/marbles.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 chatdbg-0.5/test/python/mean.py
--rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 chatdbg-0.5/test/python/nb.ipynb
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 chatdbg-0.5/test/python/requirements.txt
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 chatdbg-0.5/test/python/sample.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 chatdbg-0.5/test/rust/.gitignore
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 chatdbg-0.5/test/rust/Cargo.toml
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 chatdbg-0.5/test/rust/test-failed-assert.rs
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 chatdbg-0.5/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 chatdbg-0.5/LICENSE
--rw-r--r--   0        0        0    10109 2020-02-02 00:00:00.000000 chatdbg-0.5/README.md
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 chatdbg-0.5/pyproject.toml
--rw-r--r--   0        0        0    11096 2020-02-02 00:00:00.000000 chatdbg-0.5/PKG-INFO
+-rw-r--r--   0        0        0   431302 2020-02-02 00:00:00.000000 chatdbg-0.6/ChatDBG-arxiv-2403.16354.pdf
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 chatdbg-0.6/.github/workflows/release.yml
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 chatdbg-0.6/.github/workflows/sanity.yml
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 chatdbg-0.6/.github/workflows/tests.yml
+-rw-r--r--   0        0        0    12771 2020-02-02 00:00:00.000000 chatdbg-0.6/media/gdb.svg
+-rw-r--r--   0        0        0    17963 2020-02-02 00:00:00.000000 chatdbg-0.6/media/lldb.svg
+-rw-r--r--   0        0        0    11033 2020-02-02 00:00:00.000000 chatdbg-0.6/media/pdb.svg
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 chatdbg-0.6/rust-support/Cargo.toml
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 chatdbg-0.6/rust-support/chatdbg/Cargo.toml
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 chatdbg-0.6/rust-support/chatdbg/src/lib.rs
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 chatdbg-0.6/rust-support/chatdbg_macros/Cargo.toml
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 chatdbg-0.6/rust-support/chatdbg_macros/src/lib.rs
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 chatdbg-0.6/samples/cpp/test-deep-recursion.cpp
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 chatdbg-0.6/samples/cpp/test-definition-likely.cpp
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 chatdbg-0.6/samples/cpp/test-failed-assert.cpp
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 chatdbg-0.6/samples/cpp/test-failed-assert.why.txt
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 chatdbg-0.6/samples/cpp/test-input-file.cpp
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 chatdbg-0.6/samples/cpp/test-input-file.txt
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 chatdbg-0.6/samples/cpp/test-overflow.cpp
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 chatdbg-0.6/samples/cpp/test-overflow.why.txt
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 chatdbg-0.6/samples/cpp/test-pointers-loop.cpp
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 chatdbg-0.6/samples/cpp/test-pointers.cpp
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 chatdbg-0.6/samples/cpp/test-stack-overflow.cpp
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 chatdbg-0.6/samples/cpp/test-stack-overflow.why.txt
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 chatdbg-0.6/samples/cpp/test-use-after-free.cpp
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 chatdbg-0.6/samples/cpp/test-use-after-free.why.txt
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 chatdbg-0.6/samples/cpp/test-user-input.cpp
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 chatdbg-0.6/samples/cpp/test-user-input.txt
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 chatdbg-0.6/samples/python/README.md
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 chatdbg-0.6/samples/python/bootstrap.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 chatdbg-0.6/samples/python/bootstrap2.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 chatdbg-0.6/samples/python/ds101.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 chatdbg-0.6/samples/python/marble-sample.csv
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 chatdbg-0.6/samples/python/marbles.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 chatdbg-0.6/samples/python/mean.py
+-rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 chatdbg-0.6/samples/python/nb.ipynb
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 chatdbg-0.6/samples/python/requirements.txt
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 chatdbg-0.6/samples/python/sample.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 chatdbg-0.6/samples/python/testme.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 chatdbg-0.6/samples/rust/.gitignore
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 chatdbg-0.6/samples/rust/Cargo.toml
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 chatdbg-0.6/samples/rust/test-failed-assert.rs
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/__init__.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/__main__.py
+-rw-r--r--   0        0        0     8386 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/chatdbg_gdb.py
+-rw-r--r--   0        0        0    11030 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/chatdbg_lldb.py
+-rw-r--r--   0        0        0    23352 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/chatdbg_pdb.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/assistant/__init__.py
+-rw-r--r--   0        0        0    13162 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/assistant/assistant.py
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/assistant/listeners.py
+-rw-r--r--   0        0        0     6730 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/native_util/clangd_lsp_integration.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/native_util/code.py
+-rw-r--r--   0        0        0     7618 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/native_util/dbg_dialog.py
+-rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/native_util/stacks.py
+-rw-r--r--   0        0        0     5003 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/old_stuff/chatdbg_utils.py
+-rw-r--r--   0        0        0     4673 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/old_stuff/gdb_print_test.py
+-rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/old_stuff/lldb_why.py
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/old_stuff/prompts.py
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/pdb/prompts.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/pdb/text.py
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/pdb_util/capture.py
+-rw-r--r--   0        0        0     5914 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/pdb_util/locals.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/pdb_util/paths.py
+-rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/util/config.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/util/history.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/util/instructions.txt
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/util/jupyter.py
+-rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/util/log.py
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/util/markdown.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/util/plog.py
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/util/printer.py
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/util/prompts.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/util/stream.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/util/text.py
+-rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/util/trim.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/util/wrap.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/windbg/CMakeLists.txt
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/windbg/build-chatdbg.bat
+-rw-r--r--   0        0        0    11421 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/windbg/chatdbg.cpp
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/windbg/vcpkg-configuration.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/windbg/vcpkg.json
+-rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/windbg/include/appendlines.hpp
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/windbg/include/getmodel.hpp
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/windbg/include/joinstrings.hpp
+-rw-r--r--   0        0        0    25429 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/windbg/include/openai.hpp
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/windbg/include/wordwrap.hpp
+-rw-r--r--   0        0        0   915040 2020-02-02 00:00:00.000000 chatdbg-0.6/src/chatdbg/windbg/nlohmann/json.hpp
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 chatdbg-0.6/test/requirements.txt
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_1.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_10.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_100.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_101.py
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_102.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_103.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_104.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_105.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_11.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_12.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_13.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_14.py
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_15.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_16.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_17.py
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_18.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_19.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_2.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_20.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_21.py
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_22.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_23.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_24.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_25.py
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_26.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_27.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_28.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_29.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_3.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_30.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_31.py
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_32.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_33.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_34.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_35.py
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_36.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_37.py
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_38.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_39.py
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_4.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_40.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_41.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_42.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_43.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_44.py
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_45.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_46.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_47.py
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_48.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_49.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_5.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_50.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_51.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_52.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_53.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_54.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_55.py
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_56.py
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_57.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_58.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_59.py
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_6.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_60.py
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_61.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_62.py
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_63.py
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_64.py
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_65.py
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_66.py
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_67.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_68.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_69.py
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_7.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_70.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_71.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_72.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_73.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_74.py
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_75.py
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_76.py
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_77.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_78.py
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_79.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_8.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_80.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_81.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_82.py
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_83.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_84.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_85.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_86.py
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_87.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_88.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_89.py
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_9.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_90.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_91.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_92.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_93.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_94.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_95.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_96.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_97.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 chatdbg-0.6/test/test_coverup_99.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 chatdbg-0.6/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 chatdbg-0.6/LICENSE
+-rw-r--r--   0        0        0    11443 2020-02-02 00:00:00.000000 chatdbg-0.6/README.md
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 chatdbg-0.6/pyproject.toml
+-rw-r--r--   0        0        0    12431 2020-02-02 00:00:00.000000 chatdbg-0.6/PKG-INFO
```

### Comparing `chatdbg-0.5/ChatDBG-arxiv-2403.16354.pdf` & `chatdbg-0.6/ChatDBG-arxiv-2403.16354.pdf`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/.github/workflows/release.yml` & `chatdbg-0.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/rust-support/chatdbg/src/lib.rs` & `chatdbg-0.6/rust-support/chatdbg/src/lib.rs`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/rust-support/chatdbg_macros/src/lib.rs` & `chatdbg-0.6/rust-support/chatdbg_macros/src/lib.rs`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/src/chatdbg/__main__.py` & `chatdbg-0.6/src/chatdbg/__main__.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/src/chatdbg/chatdbg_lldb.py` & `chatdbg-0.6/src/chatdbg/chatdbg_lldb.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 @lldb.command("definition")
 def _function_definition(
     debugger: lldb.SBDebugger,
     command: str,
     result: lldb.SBCommandReturnObject,
     internal_dict: dict,
 ) -> None:
-    result.AppendMessage(clangd_lsp_integration.lldb_definition(command))
+    result.AppendMessage(clangd_lsp_integration.native_definition(command))
 
 
 @lldb.command("chat")
 @lldb.command("why")
 def chat(
     debugger: lldb.SBDebugger,
     command: str,
@@ -134,22 +134,22 @@
             reason = thread.GetStopReason()
             if reason not in [lldb.eStopReasonNone, lldb.eStopReasonInvalid]:
                 return thread
         return thread
 
     def check_debugger_state(self):
         if not self._debugger.GetSelectedTarget():
-            self.fail("must be attached to a program to use `chat`.")
+            self.fail("Must be attached to a program to use `why` or `chat`.")
 
         elif not self._is_debug_build():
             self.fail(
-                "your program must be compiled with debug information (`-g`) to use `chat`."
+                "Your program must be compiled with debug information (`-g`) to use `why` or `chat`."
             )
 
-        thread = self.get_thread(self._debugger)
+        thread = self.get_thread()
         if not thread:
             self.fail("must run the code first to use `chat`.")
 
         if not clangd_lsp_integration.is_available():
             self.warn(
                 "`clangd` was not found. The `find_definition` function will not be made available."
             )
@@ -161,20 +161,22 @@
         if not thread:
             return None
 
         skipped = 0
         summaries: List[Union[_FrameSummaryEntry, _SkippedFramesEntry]] = []
 
         index = -1
+        # For each frame in thread
         for frame in thread:
             index += 1
             if not frame.GetDisplayFunctionName():
                 skipped += 1
                 continue
             name = frame.GetDisplayFunctionName().split("(")[0]
+            # Get function arguments, store as _ArgumentEntries
             arguments: List[_ArgumentEntry] = []
             for j in range(
                 frame.GetFunction().GetType().GetFunctionArgumentTypes().GetSize()
             ):
                 arg = frame.FindVariable(frame.GetFunction().GetArgumentName(j))
                 if not arg:
                     arguments.append(
@@ -182,14 +184,15 @@
                     )
                     continue
                 # TODO: Check if we should simplify / truncate types, e.g. std::unordered_map.
                 arguments.append(
                     _ArgumentEntry(arg.GetTypeName(), arg.GetName(), arg.GetValue())
                 )
 
+            # Look for paths to the function file. If there's no source, skip frame.
             line_entry = frame.GetLineEntry()
             file_path = line_entry.GetFileSpec().fullpath
             if file_path == None:
                 file_path = "[unknown]"
             lineno = line_entry.GetLine()
 
             # If we are in a subdirectory, use a relative path instead.
@@ -197,18 +200,20 @@
                 file_path = os.path.relpath(file_path)
 
             # Skip frames for which we have no source -- likely system frames.
             if not os.path.exists(file_path):
                 skipped += 1
                 continue
 
+            # Add _SkippedFramesEntry onto summaries list
             if skipped > 0:
                 summaries.append(_SkippedFramesEntry(skipped))
                 skipped = 0
 
+            # Otherwise, add _FrameSummaryEntries until max_entries, then break
             summaries.append(
                 _FrameSummaryEntry(index, name, arguments, file_path, lineno)
             )
             if len(summaries) >= max_entries:
                 break
 
         if skipped > 0:
@@ -243,25 +248,26 @@
         Get the process that the current target owns.
         :return: An lldb object representing the process (lldb.SBProcess) that this target owns.
         """
         target = self._debugger.GetSelectedTarget()
         return target.process if target else None
 
     def _initial_prompt_error_message(self):
-        thread = self.get_thread(self._debugger)
+        thread = self.get_thread()
 
         error_message = thread.GetStopDescription(1024) if thread else None
         if error_message:
             return error_message
         else:
             self.warn("could not generate an error message.")
             return None
 
     def _initial_prompt_command_line(self):
         executable = self._debugger.GetSelectedTarget().GetExecutable()
+
         executable_path = os.path.join(
             executable.GetDirectory(), executable.GetFilename()
         )
         if executable_path.startswith(os.getcwd()):
             executable_path = os.path.join(".", os.path.relpath(executable_path))
 
         command_line_arguments = [
@@ -299,7 +305,27 @@
 
     def _prompt_stack(self):
         """
         Return a simple backtrace to show the LLM where we are on the stack
         in followup prompts.
         """
         return None
+    
+    def llm_debug(self, command: str) -> str:
+        """
+        {
+            "name": "debug",
+            "description": "The `debug` function runs an LLDB command on the stopped program and gets the response.",
+            "parameters": {
+                "type": "object",
+                "properties": {
+                    "command": {
+                        "type": "string",
+                        "description": "The LLDB command to run, possibly with arguments."
+                    }
+                },
+                "required": [ "command" ]
+            }
+        }
+        """
+        return command, self._run_one_command(command)
+
```

### Comparing `chatdbg-0.5/src/chatdbg/chatdbg_pdb.py` & `chatdbg-0.6/src/chatdbg/chatdbg_pdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import types
 import ast
 import atexit
 import inspect
 import linecache
 import os
 import pdb
 import pydoc
@@ -293,30 +294,40 @@
             # message already printed in _getval
             pass
 
     def do_info(self, arg):
         """info name
         Print the pydoc string (and source code, if available) for a name.
         """
+
         try:
             # try both given and unqualified form incase LLM biffs
             args_to_try = [arg, arg.split(".")[-1]]
             obj = None
             for x in args_to_try:
                 try:
                     obj = eval(x, self.curframe.f_globals, self.curframe_locals)
                     break  # found something so we're good
                 except:
                     # fail silently, try the next name
                     pass
 
+            if obj == None:
+                # try again, using pydoc's logic...
+                obj = pydoc.locate(arg)
+
             # didn't find anything
             if obj == None:
                 self.message(f"No name `{arg}` is visible in the current frame.")
+            elif isinstance(obj, types.BuiltinFunctionType) or isinstance(
+                obj, types.BuiltinMethodType
+            ):
+                self.message(f"`{arg}` is a built-in.")
             elif self._is_user_file(inspect.getfile(obj)):
+                self.message(f"Source from file {inspect.getfile(obj)}:")
                 self.do_source(x)
             else:
                 self.do_pydoc(x)
                 self.message(
                     f"You MUST assume that `{x}` is specified and implemented correctly."
                 )
         except OSError:
@@ -514,16 +525,15 @@
             return build_initial_prompt(
                 self._initial_prompt_enchriched_stack_trace(),
                 self._initial_prompt_error_message(),
                 self._initial_prompt_error_details(),
                 self._initial_prompt_command_line(),
                 self._initial_prompt_input(),
                 self._prompt_history(),
-                None,
-                arg,
+                user_text=arg,
             )
         else:
             return build_followup_prompt(
                 self._prompt_history(), self._prompt_stack(), arg
             )
 
     def do_chat(self, arg):
```

### Comparing `chatdbg-0.5/src/chatdbg/assistant/assistant.py` & `chatdbg-0.6/src/chatdbg/assistant/assistant.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 
 class AssistantError(Exception):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
 
-def remove_non_printable_chars(s):
+def remove_non_printable_chars(s: str) -> str:
     printable_chars = set(string.printable)
     filtered_string = "".join(filter(lambda x: x in printable_chars, s))
     return filtered_string
 
 
 class Assistant:
     def __init__(
@@ -285,15 +285,23 @@
                     tool_chunks, self._conversation
                 )
 
                 # this part wasn't counted above...
                 cost += litellm.completion_cost(tool_completion)
 
                 tool_message = tool_completion.choices[0].message
+
                 tool_json = tool_message.json()
+
+                # patch for litellm sometimes putting index fields in the tool calls it constructs
+                # in stream_chunk_builder.  gpt-4-turbo-2024-04-09 can't handle those index fields, so
+                # just remove them for the moment.
+                for tool_call in tool_json.get("tool_calls", []):
+                    _ = tool_call.pop("index", None)
+
                 tool_json["role"] = "assistant"
                 self._conversation.append(tool_json)
                 self._add_function_results_to_conversation(tool_message)
             else:
                 break
 
         stats = {
```

### Comparing `chatdbg-0.5/src/chatdbg/assistant/listeners.py` & `chatdbg-0.6/src/chatdbg/assistant/listeners.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/src/chatdbg/native_util/clangd_lsp_integration.py` & `chatdbg-0.6/src/chatdbg/native_util/clangd_lsp_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
             },
         )
         self.process.stdin.write(request)
         self.process.stdin.flush()
         return _parse_lsp_response(self.id, self.process.stdout)
 
 
-def lldb_definition(command):
+def native_definition(command):
     if not is_available():
         return "`clangd` was not found. The `definition` function will not be made available."
     last_space_index = command.rfind(" ")
     if last_space_index == -1:
         return "`clangd` was not found. The `definition` function will not be made available."
     filename_lineno = command[:last_space_index]
     symbol = command[last_space_index + 1 :]
```

### Comparing `chatdbg-0.5/src/chatdbg/native_util/dbg_dialog.py` & `chatdbg-0.6/src/chatdbg/native_util/dbg_dialog.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,26 +31,26 @@
 
     def __init__(self, prompt) -> None:
         self._prompt = prompt
         self._history = CommandHistory(self._prompt)
 
     def query_and_print(self, assistant, user_text, is_followup):
         prompt = self.build_prompt(user_text, is_followup)
+
         self._history.clear()
         print(assistant.query(prompt, user_text)["message"])
 
     def dialog(self, user_text):
         assistant = self._make_assistant()
         self.check_debugger_state()
 
         self.query_and_print(assistant, user_text, False)
         while True:
             try:
-                command = input(">>> " + self._prompt).strip()
-
+                command = input("(ChatDBG chatting) ").strip()
                 if command in ["exit", "quit"]:
                     break
                 if command in ["chat", "why"]:
                     self.query_and_print(assistant, command, True)
                 elif command == "history":
                     print(self._history)
                 else:
@@ -108,50 +108,32 @@
         in followup prompts.
         """
         return None
 
     def _prompt_history(self):
         return str(self._history)
 
-    def build_prompt(self, arg, conversing):
+    def build_prompt(self, arg, conversing):        
         if not conversing:
             return build_initial_prompt(
                 self._initial_prompt_enchriched_stack_trace(),
                 self._initial_prompt_error_message(),
                 self._initial_prompt_error_details(),
                 self._initial_prompt_command_line(),
                 self._initial_prompt_input(),
                 self._prompt_history(),
-                None,
-                arg,
+                user_text=arg,
             )
         else:
             return build_followup_prompt(
                 self._prompt_history(), self._prompt_stack(), arg
             )
 
-    # TODO: Factor out the name of the debugger that's embedded in the doc string...
     def llm_debug(self, command: str) -> str:
-        """
-        {
-            "name": "debug",
-            "description": "The `debug` function runs an LLDB command on the stopped program and gets the response.",
-            "parameters": {
-                "type": "object",
-                "properties": {
-                    "command": {
-                        "type": "string",
-                        "description": "The LLDB command to run, possibly with arguments."
-                    }
-                },
-                "required": [ "command" ]
-            }
-        }
-        """
-        return command, self._run_one_command(command)
+        pass
 
     def llm_get_code_surrounding(self, filename: str, line_number: int) -> str:
         """
         {
             "name": "get_code_surrounding",
             "description": "The `get_code_surrounding` function returns the source code in the given file surrounding and including the provided line number.",
             "parameters": {
@@ -210,22 +192,27 @@
         return functions
 
     def _make_assistant(self) -> Assistant:
 
         functions = self._supported_functions()
         instruction_prompt = self.initial_prompt_instructions()
 
+        # gdb overwrites sys.stdin to be a file object that doesn't seem
+        # to support colors or streaming.  So, just use the original stdout
+        # here for all subclasses.
+        printer = chatdbg_config.make_printer(sys.__stdout__, self._prompt, "   ", 80)
+        
         assistant = Assistant(
             instruction_prompt,
             model=chatdbg_config.model,
             debug=chatdbg_config.debug,
             functions=functions,
             stream=not chatdbg_config.no_stream,
             listeners=[
-                chatdbg_config.make_printer(sys.stdout, self._prompt, "   ", 80),
+                printer,
                 self._log,
             ],
         )
 
         return assistant
 
     def warn(self, message):
```

### Comparing `chatdbg-0.5/src/chatdbg/native_util/stacks.py` & `chatdbg-0.6/src/chatdbg/native_util/stacks.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 class _ArgumentEntry:
     def __init__(self, type: str, name: str, value: str):
         self._type = type
         self._name = name
         self._value = value
 
     def __str__(self):
-        return f"({self._type}) {self._name} = {self._value if self._value else '[unknown]'}"
+        return f"({self._type}) {self._name} = {self._value if self._value is not None else '[unknown]'}"
 
     def __repr__(self):
-        return f"_ArgumentEntry({repr(self.type)}, {repr(self._name)}, {repr(self._value)})"
+        return f"_ArgumentEntry({repr(self._type)}, {repr(self._name)}, {repr(self._value) if self._value is not None else '[unknown]'})"
 
 
 class _FrameSummaryEntry:
     def __init__(
         self,
         index: int,
         name: str,
@@ -38,15 +38,16 @@
     def file_path(self):
         return self._file_path
 
     def lineno(self):
         return self._lineno
 
     def __str__(self):
-        return f"{self._index}: {self._name}({', '.join([str(a) for a in self._arguments])}) at {self._file_path}:{self._lineno}"
+        a = ', '.join([str(a) for a in self._arguments])
+        return f"{self._index}: {self._name}({a}) at {self._file_path}:{self._lineno}"
 
     def __repr__(self):
         return f"_FrameSummaryEntry({self._index}, {repr(self._name)}, {repr(self._arguments)}, {repr(self._file_path)}, {self._lineno})"
 
 
 class _SkippedFramesEntry:
     def __init__(self, count: int):
@@ -62,15 +63,16 @@
         return f"_SkippedFramesEntry({self._count})"
 
 
 def build_enriched_stacktrace(summaries):
     parts = []
     if not summaries:
         print("could not generate any frame summary.")
-    else:
+        return
+    else:        
         frame_summary = "\n".join([str(s) for s in summaries])
         parts.append(frame_summary)
 
         total_frames = sum(
             [s.count() if isinstance(s, _SkippedFramesEntry) else 1 for s in summaries]
         )
 
@@ -97,9 +99,8 @@
     if source_code_entries:
         parts.append(
             f"Here is the source code for the first {len(source_code_entries)} frames:\n\n"
             + "\n\n".join(source_code_entries)
         )
     else:
         print("could not retrieve source code for any frames.")
-
     return "\n\n".join(parts)
```

### Comparing `chatdbg-0.5/src/chatdbg/old_stuff/chatdbg_utils.py` & `chatdbg-0.6/src/chatdbg/old_stuff/chatdbg_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,155 +1,155 @@
-# import argparse
-# import textwrap
-# import time
-# from typing import Any, Callable, List, Optional, Tuple
-
-# import llm_utils
-# import openai
-# from rich.console import Console
-
-
-# class RichArgParser(argparse.ArgumentParser):
-#     def __init__(self, *args: Any, **kwargs: Any):
-#         self.console = Console(highlight=False)
-#         super().__init__(*args, **kwargs)
-
-#     def _print_message(self, message: Optional[str], file: Any = None) -> None:
-#         if message:
-#             self.console.print(message)
-
-
-# class ChatDBGArgumentFormatter(argparse.HelpFormatter):
-#     # RawDescriptionHelpFormatter.
-#     def _fill_text(self, text, width, indent):
-#         return "".join(indent + line for line in text.splitlines(keepends=True))
-
-#     # RawTextHelpFormatter.
-#     def _split_lines(self, text, width):
-#         return text.splitlines()
-
-#     # ArgumentDefaultsHelpFormatter.
-#     # Ignore if help message is multiline.
-#     def _get_help_string(self, action):
-#         help = action.help
-#         if "\n" not in help and "%(default)" not in action.help:
-#             if action.default is not argparse.SUPPRESS:
-#                 defaulting_nargs = [argparse.OPTIONAL, argparse.ZERO_OR_MORE]
-#                 if action.option_strings or action.nargs in defaulting_nargs:
-#                     help += " (default: %(default)s)"
-#         return help
-
-
-# def parse_known_args(argv: List[str]) -> Tuple[argparse.Namespace, List[str]]:
-#     description = textwrap.dedent(
-#         rf"""
-#             [b]ChatDBG[/b]: A Python debugger that uses AI to tell you `why`.
-#             [blue][link=https://github.com/plasma-umass/ChatDBG]https://github.com/plasma-umass/ChatDBG[/link][/blue]
-#         """
-#     ).strip()
-#     parser = RichArgParser(
-#         prog="chatdbg",
-#         usage=argparse.SUPPRESS,
-#         description=description,
-#         formatter_class=ChatDBGArgumentFormatter,
-#     )
-#     parser.add_argument(
-#         "--llm",
-#         type=str,
-#         default="gpt-4-turbo-preview",
-#         help="the language model to use, e.g., 'gpt-3.5-turbo' or 'gpt-4'",
-#     )
-#     parser.add_argument(
-#         "--debug",
-#         action="store_true",
-#         help="when enabled, only print prompt and exit with `why`, and output to a log file with `chat`",
-#     )
-#     parser.add_argument(
-#         "--tool-call-max-result-tokens",
-#         default=512,  # Arbitrary.
-#         help="the maximum number of tokens to send in any tool call response",
-#     )
-#     parser.add_argument(
-#         "--fresh",
-#         action="store_true",
-#         default=False,
-#         help="in `chat` mode, reset the chat history to start a new conversation",
-#     )
-#     parser.add_argument(
-#         "--timeout",
-#         type=int,
-#         default=60,
-#         help="the timeout for API calls in seconds",
-#     )
-
-#     return parser.parse_known_args(argv)
-
-
-# def explain(
-#     source_code: str,
-#     traceback: str,
-#     exception: str,
-#     args: argparse.Namespace,
-#     append_message: Callable[[str], None] = print,
-#     append_warning: Callable[[str], None] = print,
-#     set_error: Callable[[str], None] = print,
-# ) -> None:
-#     user_prompt = f"""
-# Explain what the root cause of this error is, given the following source code
-# context for each stack frame and a traceback, and propose a fix. In your
-# response, never refer to the frames given below (as in, 'frame 0'). Instead,
-# always refer only to specific lines and filenames of source code.
-
-# Source code for each stack frame:
-# ```
-# {source_code}
-# ```
-
-# Traceback:
-# {traceback}
-
-# Stop reason: {exception}
-#     """.strip()
-
-#     input_tokens = llm_utils.count_tokens(args.llm, user_prompt)
-
-#     if args.debug:
-#         append_message(f"{user_prompt}\n\nTotal input tokens: {input_tokens}.")
-#         return
-
-#     start = time.time()
-
-#     try:
-#         client = openai.OpenAI(timeout=args.timeout)
-#     except openai.OpenAIError:
-#         append_warning("you need an OpenAI key to use this tool.")
-#         append_warning("You can get a key here: https://platform.openai.com/api-keys.")
-#         append_warning("set the environment variable OPENAI_API_KEY to your key value.")
-#         return
-
-#     try:
-#         completion = client.chat.completions.create(
-#             model=args.llm, messages=[{"role": "user", "content": user_prompt}]
-#         )
-#     except openai.NotFoundError:
-#         set_error(f"'{args.llm}' does not exist or you do not have access to it.")
-#         return
-#     except openai.RateLimitError:
-#         set_error("you have exceeded a rate limit or have no remaining funds.")
-#         return
-#     except openai.APITimeoutError:
-#         set_error("the OpenAI API timed out.")
-#         return
-
-#     text = completion.choices[0].message.content
-#     elapsed = time.time() - start
-#     input_tokens = completion.usage.prompt_tokens
-#     output_tokens = completion.usage.completion_tokens
-#     cost = llm_utils.calculate_cost(input_tokens, output_tokens, args.llm)
-
-#     append_message(
-#         llm_utils.word_wrap_except_code_blocks(text)
-#         + "\n\n"
-#         + f"Elapsed time: {elapsed:.2f} seconds"
-#         + "\n"
-#         + f"Total cost: {cost:.2f}$"
-#     )
+import argparse
+import textwrap
+import time
+from typing import Any, Callable, List, Optional, Tuple
+
+import llm_utils
+import openai
+from rich.console import Console
+
+
+class RichArgParser(argparse.ArgumentParser):
+    def __init__(self, *args: Any, **kwargs: Any):
+        self.console = Console(highlight=False)
+        super().__init__(*args, **kwargs)
+
+    def _print_message(self, message: Optional[str], file: Any = None) -> None:
+        if message:
+            self.console.print(message)
+
+
+class ChatDBGArgumentFormatter(argparse.HelpFormatter):
+    # RawDescriptionHelpFormatter.
+    def _fill_text(self, text, width, indent):
+        return "".join(indent + line for line in text.splitlines(keepends=True))
+
+    # RawTextHelpFormatter.
+    def _split_lines(self, text, width):
+        return text.splitlines()
+
+    # ArgumentDefaultsHelpFormatter.
+    # Ignore if help message is multiline.
+    def _get_help_string(self, action):
+        help = action.help
+        if "\n" not in help and "%(default)" not in action.help:
+            if action.default is not argparse.SUPPRESS:
+                defaulting_nargs = [argparse.OPTIONAL, argparse.ZERO_OR_MORE]
+                if action.option_strings or action.nargs in defaulting_nargs:
+                    help += " (default: %(default)s)"
+        return help
+
+
+def parse_known_args(argv: List[str]) -> Tuple[argparse.Namespace, List[str]]:
+    description = textwrap.dedent(
+        rf"""
+            [b]ChatDBG[/b]: A Python debugger that uses AI to tell you `why`.
+            [blue][link=https://github.com/plasma-umass/ChatDBG]https://github.com/plasma-umass/ChatDBG[/link][/blue]
+        """
+    ).strip()
+    parser = RichArgParser(
+        prog="chatdbg",
+        usage=argparse.SUPPRESS,
+        description=description,
+        formatter_class=ChatDBGArgumentFormatter,
+    )
+    parser.add_argument(
+        "--llm",
+        type=str,
+        default="gpt-4-turbo-preview",
+        help="the language model to use, e.g., 'gpt-3.5-turbo' or 'gpt-4'",
+    )
+    parser.add_argument(
+        "--debug",
+        action="store_true",
+        help="when enabled, only print prompt and exit with `why`, and output to a log file with `chat`",
+    )
+    parser.add_argument(
+        "--tool-call-max-result-tokens",
+        default=512,  # Arbitrary.
+        help="the maximum number of tokens to send in any tool call response",
+    )
+    parser.add_argument(
+        "--fresh",
+        action="store_true",
+        default=False,
+        help="in `chat` mode, reset the chat history to start a new conversation",
+    )
+    parser.add_argument(
+        "--timeout",
+        type=int,
+        default=60,
+        help="the timeout for API calls in seconds",
+    )
+
+    return parser.parse_known_args(argv)
+
+
+def explain(
+    source_code: str,
+    traceback: str,
+    exception: str,
+    args: argparse.Namespace,
+    append_message: Callable[[str], None] = print,
+    append_warning: Callable[[str], None] = print,
+    set_error: Callable[[str], None] = print,
+) -> None:
+    user_prompt = f"""
+Explain what the root cause of this error is, given the following source code
+context for each stack frame and a traceback, and propose a fix. In your
+response, never refer to the frames given below (as in, 'frame 0'). Instead,
+always refer only to specific lines and filenames of source code.
+
+Source code for each stack frame:
+```
+{source_code}
+```
+
+Traceback:
+{traceback}
+
+Stop reason: {exception}
+    """.strip()
+
+    input_tokens = llm_utils.count_tokens(args.llm, user_prompt)
+
+    if args.debug:
+        append_message(f"{user_prompt}\n\nTotal input tokens: {input_tokens}.")
+        return
+
+    start = time.time()
+
+    try:
+        client = openai.OpenAI(timeout=args.timeout)
+    except openai.OpenAIError:
+        append_warning("you need an OpenAI key to use this tool.")
+        append_warning("You can get a key here: https://platform.openai.com/api-keys.")
+        append_warning("set the environment variable OPENAI_API_KEY to your key value.")
+        return
+
+    try:
+        completion = client.chat.completions.create(
+            model=args.llm, messages=[{"role": "user", "content": user_prompt}]
+        )
+    except openai.NotFoundError:
+        set_error(f"'{args.llm}' does not exist or you do not have access to it.")
+        return
+    except openai.RateLimitError:
+        set_error("you have exceeded a rate limit or have no remaining funds.")
+        return
+    except openai.APITimeoutError:
+        set_error("the OpenAI API timed out.")
+        return
+
+    text = completion.choices[0].message.content
+    elapsed = time.time() - start
+    input_tokens = completion.usage.prompt_tokens
+    output_tokens = completion.usage.completion_tokens
+    cost = llm_utils.calculate_cost(input_tokens, output_tokens, args.llm)
+
+    append_message(
+        llm_utils.word_wrap_except_code_blocks(text)
+        + "\n\n"
+        + f"Elapsed time: {elapsed:.2f} seconds"
+        + "\n"
+        + f"Total cost: {cost:.2f}$"
+    )
```

### Comparing `chatdbg-0.5/src/chatdbg/old_stuff/gdb_print_test.py` & `chatdbg-0.6/src/chatdbg/old_stuff/gdb_print_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,109 +1,110 @@
-class PrintTest(gdb.Command):
-    """print all variables in a run while recursing through pointers, keeping track of seen addresses"""
+# class PrintTest(gdb.Command):
+#     """print all variables in a run while recursing through pointers, keeping track of seen addresses"""
 
-    def __init__(self):
-        super().__init__("print-test", gdb.COMMAND_DATA, gdb.COMPLETE_SYMBOL, True)
+#     def __init__(self):
+#         super().__init__("print-test", gdb.COMMAND_DATA, gdb.COMPLETE_SYMBOL, True)
 
-    def invoke(self, arg, from_tty):
-        help_string = "Usage: print-test [recurse_max]\n\nrecurse_max: The maximum number of times to recurse through nested structs or pointers to pointers. Default: 3"
-        if arg == "--help":
-            print(help_string)
-            return
-        recurse_max = 3
-        if arg != "":
-            try:
-                recurse_max = int(arg)
-            except ValueError as e:
-                print(f"recurse_max value could not be parsed: {e}")
-                return
-        if recurse_max < 1:
-            print("recurse_max value must be at least 1.")
-            return
-        frame = gdb.selected_frame()
-        block = gdb.block_for_pc(frame.pc())
-
-        all_vars = []
-        addresses = {}
-        for symbol in block:
-            if symbol.is_argument or symbol.is_variable:
-                sym_val = frame.read_var(symbol)
-                # Returns python dictionary for each variable
-                variable = self._val_to_json(
-                    symbol.name, sym_val, recurse_max, addresses
-                )
-                js = json.dumps(variable, indent=4)
-                all_vars.append(js)
-
-        # Print all addresses and JSON objects
-        # print(addresses)
-        for j in all_vars:
-            print(j)
-
-    # Converts a gdb.Value to a JSON object
-    def _val_to_json(self, name, val, max_recurse, address_book):
-        # Store address
-        address_book.setdefault(str(val.address.format_string()), name)
-
-        diction = {}
-        # Set var name
-        diction["name"] = name
-        # Set var type
-        if val.type.code is gdb.TYPE_CODE_PTR:
-            diction["type"] = "pointer"  # Default type name is "none"
-        elif val.type.code is gdb.TYPE_CODE_ARRAY:
-            diction["type"] = "array"  # Default type name is "none"
-        else:
-            diction["type"] = val.type.name
-        # Dereference pointers
-        if val.type.code is gdb.TYPE_CODE_PTR:
-            if val:
-                value = "->"
-                try:
-                    deref_val = val.referenced_value()
-                    # If dereferenced value is "seen", then get name from address book
-                    if deref_val.address.format_string() in address_book:
-                        diction["value"] = address_book[
-                            deref_val.address.format_string()
-                        ]
-                    else:
-                        # Recurse up to max_recurse times
-                        for i in range(max_recurse - 1):
-                            if deref_val.type.code is gdb.TYPE_CODE_PTR:
-                                value += "->"
-                                deref_val = deref_val.referenced_value()
-                            elif deref_val.type.code is gdb.TYPE_CODE_STRUCT:
-                                value = self._val_to_json(
-                                    value + name,
-                                    deref_val,
-                                    max_recurse - i - 1,
-                                    address_book,
-                                )
-                                break
-                            else:
-                                break
-                        # Append to -> string or not, depending on type of value
-                        if isinstance(value, dict):
-                            diction["value"] = value
-                        else:
-                            diction["value"] = value + deref_val.format_string()
-                except Exception as e:
-                    diction["value"] = value + "Exception"
-            else:
-                # Nullptr case, might be a better way to represent
-                diction["value"] = "nullptr"
-        # If struct, recurse through fields
-        elif val.type.code is gdb.TYPE_CODE_STRUCT:
-            fields = []
-            for f in val.type.fields():
-                fields.append(
-                    self._val_to_json(
-                        f.name, val[f.name], max_recurse - 1, address_book
-                    )
-                )
-            diction["value"] = fields
-        else:
-            diction["value"] = val.format_string()
-        return diction
+#     def invoke(self, arg, from_tty):
+#         help_string = "Usage: print-test [recurse_max]\n\nrecurse_max: The maximum number of times to recurse through nested structs or pointers to pointers. Default: 3"
+#         if arg == "--help":
+#             print(help_string)
+#             return
+#         recurse_max = 3
+#         if arg != "":
+#             try:
+#                 recurse_max = int(arg)
+#             except ValueError as e:
+#                 print(f"recurse_max value could not be parsed: {e}")
+#                 return
+#         if recurse_max < 1:
+#             print("recurse_max value must be at least 1.")
+#             return
+#         frame = gdb.selected_frame()
+#         block = gdb.block_for_pc(frame.pc())
+
+#         all_vars = []
+#         addresses = {}
+#         for symbol in block:
+#             if symbol.is_argument or symbol.is_variable:
+#                 sym_val = frame.read_var(symbol)
+#                 # Returns python dictionary for each variable
+#                 variable = self._val_to_json(
+#                     symbol.name, sym_val, recurse_max, addresses
+#                 )
+#                 js = json.dumps(variable, indent=4)
+#                 all_vars.append(js)
+
+#         # Print all addresses and JSON objects
+#         # print(addresses)
+#         for j in all_vars:
+#             print(j)
+
+#     # Converts a gdb.Value to a JSON object
+#     def _val_to_json(self, name, val, max_recurse, address_book):
+#         # Store address
+#         address_book.setdefault(str(val.address.format_string()), name)
+
+#         diction = {}
+#         # Set var name
+#         diction["name"] = name
+#         # Set var type
+#         if val.type.code is gdb.TYPE_CODE_PTR:
+#             diction["type"] = "pointer"  # Default type name is "none"
+#         elif val.type.code is gdb.TYPE_CODE_ARRAY:
+#             diction["type"] = "array"  # Default type name is "none"
+#         else:
+#             diction["type"] = val.type.name
+#         # Dereference pointers
+#         if val.type.code is gdb.TYPE_CODE_PTR:
+#             if val:
+#                 value = "->"
+#                 try:
+#                     deref_val = val.referenced_value()
+#                     # If dereferenced value is "seen", then get name from address book
+#                     if deref_val.address.format_string() in address_book:
+#                         diction["value"] = address_book[
+#                             deref_val.address.format_string()
+#                         ]
+#                     else:
+#                         # Recurse up to max_recurse times
+#                         for i in range(max_recurse - 1):
+#                             if deref_val.type.code is gdb.TYPE_CODE_PTR:
+#                                 value += "->"
+#                                 deref_val = deref_val.referenced_value()
+#                             elif deref_val.type.code is gdb.TYPE_CODE_STRUCT:
+#                                 value = self._val_to_json(
+#                                     value + name,
+#                                     deref_val,
+#                                     max_recurse - i - 1,
+#                                     address_book,
+#                                 )
+#                                 break
+#                             else:
+#                                 break
+#                         # Append to -> string or not, depending on type of value
+#                         if isinstance(value, dict):
+#                             diction["value"] = value
+#                         else:
+#                             diction["value"] = value + deref_val.format_string()
+#                 except Exception as e:
+#                     diction["value"] = value + "Exception"
+#             else:
+#                 # Nullptr case, might be a better way to represent
+#                 diction["value"] = "nullptr"
+#         # If struct, recurse through fields
+#         elif val.type.code is gdb.TYPE_CODE_STRUCT:
+#             fields = []
+#             for f in val.type.fields():
+#                 fields.append(
+#                     self._val_to_json(
+#                         f.name, val[f.name], max_recurse - 1, address_book
+#                     )
+#                 )
+#             diction["value"] = fields
+#         else:
+#             diction["value"] = val.format_string()
+#         return diction
 
 
-PrintTest()
+# PrintTest()
+
```

### Comparing `chatdbg-0.5/src/chatdbg/old_stuff/lldb_why.py` & `chatdbg-0.6/src/chatdbg/old_stuff/lldb_why.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/src/chatdbg/old_stuff/prompts.py` & `chatdbg-0.6/src/chatdbg/old_stuff/prompts.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/src/chatdbg/pdb/prompts.py` & `chatdbg-0.6/src/chatdbg/pdb/prompts.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/src/chatdbg/pdb/text.py` & `chatdbg-0.6/src/chatdbg/pdb/text.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/src/chatdbg/pdb_util/capture.py` & `chatdbg-0.6/src/chatdbg/pdb_util/capture.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/src/chatdbg/pdb_util/locals.py` & `chatdbg-0.6/src/chatdbg/pdb_util/locals.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     result = (
         "__repr__" in dir(obj.__class__)
         and obj.__class__.__repr__ is not object.__repr__
     )
     return result
 
 
-def _format_limited(value: Any, limit: int = 10, depth: int = 3) -> str:
+def _format_limited(value: Union[int, np.ndarray], limit: int = 10, depth: int = 3) -> str:
     def format_tuple(t, depth):
         return tuple([helper(x, depth) for x in t])
 
     def format_list(list, depth):
         return [helper(x, depth) for x in list]
 
     def format_dict(items, depth):
```

### Comparing `chatdbg-0.5/src/chatdbg/pdb_util/paths.py` & `chatdbg-0.6/src/chatdbg/pdb_util/paths.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/src/chatdbg/util/config.py` & `chatdbg-0.6/src/chatdbg/util/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 from types import *
 from typing import *
 
 from chatdbg.util.jupyter import ChatDBGJupyterPrinter
 
 
 def _chatdbg_get_env(
-    option_name: str, default_value: Union[int, str, bool]
-) -> Union[int, str, bool]:
+    option_name: str, default_value: Union[bool, int, str]
+) -> Union[bool, int, str]:
     env_name = "CHATDBG_" + option_name.upper()
     v = os.getenv(env_name, str(default_value))
     if type(default_value) == int:
         return int(v)
     elif type(default_value) == bool:
         return v.lower() == "true"
     else:
```

### Comparing `chatdbg-0.5/src/chatdbg/util/history.py` & `chatdbg-0.6/src/chatdbg/util/history.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/src/chatdbg/util/instructions.txt` & `chatdbg-0.6/src/chatdbg/util/instructions.txt`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/src/chatdbg/util/jupyter.py` & `chatdbg-0.6/src/chatdbg/util/jupyter.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/src/chatdbg/util/log.py` & `chatdbg-0.6/src/chatdbg/util/log.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/src/chatdbg/util/markdown.py` & `chatdbg-0.6/src/chatdbg/util/markdown.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/src/chatdbg/util/plog.py` & `chatdbg-0.6/src/chatdbg/util/plog.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/src/chatdbg/util/printer.py` & `chatdbg-0.6/src/chatdbg/util/printer.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/src/chatdbg/util/prompts.py` & `chatdbg-0.6/src/chatdbg/util/prompts.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,65 @@
 import json
 import os
 from chatdbg.util.config import chatdbg_config
 from .text import truncate_proportionally
+from typing import Any, Callable, List, Union, Optional
 
 
-def _wrap_it(before, x, after="", maxlen=2048):
-    if x:
-        x = truncate_proportionally(x, maxlen, 0.5)
+def _wrap_it(
+    before: str, text: str, after: str = "", maxlen: int = 2048
+) -> str:
+    if text:
+        text = truncate_proportionally(text, maxlen, 0.5)
         before = before + ":\n" if before else ""
         after = after + "\n" if after else ""
-        return f"{before}```\n{x}\n```\n{after}"
+        return f"{before}```\n{text}\n```\n{after}"
     else:
         return ""
 
 
-def _concat_prompt(*args):
-    args = [a for a in args if a]
+def _concat_prompt(*args) -> str:
+    args = [a for a in args if len(a) > 0]
     return "\n".join(args)
 
 
-def _user_text_it(user_text):
-    return user_text if user_text else "What's the bug? Give me a fix."
+def _user_text_it(user_text: str) -> str:
+    return user_text if len(user_text) > 0 else "What's the bug? Give me a fix."
 
 
 def build_initial_prompt(
-    stack, error, details, command_line, inputs, history, extra="", user_text=""
-):
+    stack: str,
+    error: str,
+    details: str,
+    command_line: str,
+    inputs: str,
+    history: str,
+    extra: str = "",
+    user_text: str = "",
+) -> str:
     return _concat_prompt(
         _wrap_it("The program has this stack trace", stack),
         _wrap_it("The program encountered the following error", error, details),
         _wrap_it("This was the command line", command_line),
         _wrap_it("This was the program's input", inputs),
         _wrap_it("This is the history of some debugger commands I ran", history),
         _wrap_it("", extra),
         _user_text_it(user_text),
     )
 
 
-def build_followup_prompt(history, extra, user_text):
+def build_followup_prompt(history: str, extra: str, user_text: str) -> str:
     return _concat_prompt(
         _wrap_it("This is the history of some debugger commands I ran", history),
         _wrap_it("", extra),
         _user_text_it(user_text),
     )
 
 
-def initial_instructions(functions):
+def initial_instructions(functions: List[Callable[[Any], Any]]) -> str:
     if chatdbg_config.instructions == "":
         file_path = os.path.join(os.path.dirname(__file__), "instructions.txt")
     else:
         file_path = chatdbg_config.instructions
 
     function_instructions = [json.loads(f.__doc__)["description"] for f in functions]
     with open(file_path, "r") as file:
```

### Comparing `chatdbg-0.5/src/chatdbg/util/stream.py` & `chatdbg-0.6/src/chatdbg/util/stream.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/src/chatdbg/util/text.py` & `chatdbg-0.6/src/chatdbg/util/text.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 import textwrap
+from typing import Union
 
 
 def make_arrow(pad):
     """generate the leading arrow in front of traceback or debugger"""
     if pad >= 2:
         return "-" * (pad - 2) + "> "
     elif pad == 1:
@@ -12,30 +13,32 @@
 
 
 def strip_ansi(s: str) -> str:
     ansi_escape = re.compile(r"\x1B(?:[@-Z\\-_]|\[[0-?]*[ -/]*[@-~])")
     return ansi_escape.sub("", s)
 
 
-def truncate_proportionally(text, maxlen=32000, top_proportion=0.5):
+def truncate_proportionally(
+    text: str, maxlen: int = 32000, top_proportion: Union[float, int] = 0.5
+) -> str:
     """Omit part of a string if needed to make it fit in a maximum length."""
     if len(text) > maxlen:
         pre = max(0, int((maxlen - 5) * top_proportion))
         post = max(0, maxlen - 5 - pre)
         return text[:pre] + "[...]" + text[len(text) - post :]
     return text
 
 
-def wrap_long_lines(text, width=80, subsequent_indent="    "):
+def wrap_long_lines(text: str, width: int = 80, subsequent_indent: str = "    ") -> str:
     wrapped_lines = []
     for line in text.split("\n"):
         if len(line) > width:
             wrapped_lines.extend(
                 textwrap.wrap(line, width, subsequent_indent=subsequent_indent)
             )
         else:
             wrapped_lines.append(line)
     return "\n".join(wrapped_lines)
 
 
-def fill_to_width(text, width=80):
+def fill_to_width(text: str, width: int = 80) -> str:
     return "\n".join([line.ljust(width) for line in text.split("\n")])
```

### Comparing `chatdbg-0.5/src/chatdbg/util/trim.py` & `chatdbg-0.6/src/chatdbg/util/trim.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import copy
 import warnings
+from typing import Dict, List, Union
 
 with warnings.catch_warnings():
     warnings.simplefilter("ignore")
     import litellm
 
 
 def sandwich_tokens(
@@ -21,58 +22,54 @@
         return (
             litellm.decode(model, tokens[0:top_len])
             + " [...] "
             + litellm.decode(model, tokens[bot_start:])
         )
 
 
-def sum_messages(messages, model):
+def _sum_messages(messages, model):
     return litellm.token_counter(model, messages=messages)
 
 
-def sum_kept_chunks(chunks, model):
-    return sum(sum_messages(messages, model) for (messages, kept) in chunks if kept)
+def _sum_kept_chunks(chunks, model):
+    return sum(_sum_messages(messages, model) for (messages, kept) in chunks if kept)
 
 
-def sum_all_chunks(chunks, model):
-    return sum(sum_messages(messages, model) for (messages, kept) in chunks)
-
-
-def extract(messages, model, tool_call_ids):
+def _extract(messages, model, tool_call_ids):
     tools = []
     other = []
     for m in messages:
         if m.get("tool_call_id", -1) in tool_call_ids:
             content = sandwich_tokens(m["content"], model, 512, 1.0)
             # print(len(litellm.encode(model, m['content'])), '->', len(litellm.encode(model, content)))
             m["content"] = content
             tools += [m]
         else:
             other += [m]
     return tools, other
 
 
-def chunkify(messages, model):
+def _chunkify(messages, model):
     if not messages:
         return []
     m = messages[0]
     if "tool_calls" not in m:
         m["content"] = sandwich_tokens(m["content"], model, 1024, 0)
-        return [([m], False)] + chunkify(messages[1:], model)
+        return [([m], False)] + _chunkify(messages[1:], model)
     else:
         ids = [tool_call["id"] for tool_call in m["tool_calls"]]
-        tools, other = extract(messages[1:], model, ids)
-        return [([m] + tools, False)] + chunkify(other, model)
+        tools, other = _extract(messages[1:], model, ids)
+        return [([m] + tools, False)] + _chunkify(other, model)
 
 
 def trim_messages(
-    messages,
-    model,
+    messages: List[Dict[str, str]],  # list of JSON objects encoded as dicts
+    model: str,
     trim_ratio: float = 0.75,
-):
+) -> list:
     """
     Strategy:
     - chunk messages:
         - single message, or
         - tool request and all the tool responses
     - keep the system messages
     - keep the first user message
@@ -85,15 +82,15 @@
 
     max_tokens_for_model = litellm.model_cost[model]["max_tokens"]
     max_tokens = int(max_tokens_for_model * trim_ratio)
 
     if litellm.token_counter(model, messages=messages) < max_tokens:
         return messages
 
-    chunks = chunkify(messages=messages, model=model)
+    chunks = _chunkify(messages=messages, model=model)
     # print("0", sum_all_chunks(chunks, model), max_tokens)
 
     # 1. System messages
     chunks = [(m, b or m[0]["role"] == "system") for (m, b) in chunks]
     # print("1", sum_kept_chunks(chunks, model))
 
     # 2. First User Message
@@ -106,22 +103,23 @@
     # 3. Fill it up
     for i in range(len(chunks))[::-1]:
         messages, kept = chunks[i]
         if kept:
             # print('+')
             continue
         elif (
-            sum_kept_chunks(chunks, model) + sum_messages(messages, model) < max_tokens
+            _sum_kept_chunks(chunks, model) + _sum_messages(messages, model)
+            < max_tokens
         ):
             # print('-', len(messages))
             chunks[i] = (messages, True)
         else:
             # print("N", sum_kept_chunks(chunks, model), sum_messages(messages, model))
             break
 
     # print("3", sum_kept_chunks(chunks, model))
 
     assert (
-        sum_kept_chunks(chunks, model) < max_tokens
-    ), f"New conversation too big {sum_kept_chunks(chunks, model)} vs {max_tokens}!"
+        _sum_kept_chunks(chunks, model) < max_tokens
+    ), f"New conversation too big {_sum_kept_chunks(chunks, model)} vs {max_tokens}!"
 
     return [m for (messages, kept) in chunks if kept for m in messages]
```

### Comparing `chatdbg-0.5/src/chatdbg/util/wrap.py` & `chatdbg-0.6/src/chatdbg/util/wrap.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/src/chatdbg/windbg/CMakeLists.txt` & `chatdbg-0.6/src/chatdbg/windbg/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/src/chatdbg/windbg/chatdbg.cpp` & `chatdbg-0.6/src/chatdbg/windbg/chatdbg.cpp`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/src/chatdbg/windbg/include/appendlines.hpp` & `chatdbg-0.6/src/chatdbg/windbg/include/appendlines.hpp`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/src/chatdbg/windbg/include/openai.hpp` & `chatdbg-0.6/src/chatdbg/windbg/include/openai.hpp`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/src/chatdbg/windbg/include/wordwrap.hpp` & `chatdbg-0.6/src/chatdbg/windbg/include/wordwrap.hpp`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/src/chatdbg/windbg/nlohmann/json.hpp` & `chatdbg-0.6/src/chatdbg/windbg/nlohmann/json.hpp`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/test/test-deep-recursion.cpp` & `chatdbg-0.6/samples/cpp/test-deep-recursion.cpp`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/test/test-failed-assert.why.txt` & `chatdbg-0.6/samples/cpp/test-failed-assert.why.txt`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/test/test-overflow.why.txt` & `chatdbg-0.6/samples/cpp/test-overflow.why.txt`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/test/test-use-after-free.why.txt` & `chatdbg-0.6/samples/cpp/test-use-after-free.why.txt`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/test/python/bootstrap.py` & `chatdbg-0.6/samples/python/bootstrap.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/test/python/bootstrap2.py` & `chatdbg-0.6/samples/python/bootstrap2.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/test/python/ds101.py` & `chatdbg-0.6/samples/python/ds101.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/test/python/mean.py` & `chatdbg-0.6/samples/python/mean.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/test/python/nb.ipynb` & `chatdbg-0.6/samples/python/nb.ipynb`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/.gitignore` & `chatdbg-0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/LICENSE` & `chatdbg-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `chatdbg-0.5/README.md` & `chatdbg-0.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -65,568 +65,652 @@
 00000400: 2061 7265 2061 7761 7265 2c20 4368 6174   are aware, Chat
 00000410: 4442 4720 6973 2074 6865 202a 6669 7273  DBG is the *firs
 00000420: 742a 2064 6562 7567 6765 7220 746f 2061  t* debugger to a
 00000430: 7574 6f6d 6174 6963 616c 6c79 2070 6572  utomatically per
 00000440: 666f 726d 2072 6f6f 7420 6361 7573 6520  form root cause 
 00000450: 616e 616c 7973 6973 2061 6e64 2074 6f20  analysis and to 
 00000460: 7072 6f76 6964 6520 7375 6767 6573 7465  provide suggeste
-00000470: 6420 6669 7865 732e 0a0a 466f 7220 7465  d fixes...For te
-00000480: 6368 6e69 6361 6c20 6465 7461 696c 7320  chnical details 
-00000490: 616e 6420 6120 636f 6d70 6c65 7465 2065  and a complete e
-000004a0: 7661 6c75 6174 696f 6e2c 2073 6565 206f  valuation, see o
-000004b0: 7572 2061 7258 6976 2070 6170 6572 2c20  ur arXiv paper, 
-000004c0: 5b5f 4368 6174 4442 473a 2041 6e20 4149  [_ChatDBG: An AI
-000004d0: 2d50 6f77 6572 6564 2044 6562 7567 6769  -Powered Debuggi
-000004e0: 6e67 2041 7373 6973 7461 6e74 5f5d 2868  ng Assistant_](h
-000004f0: 7474 7073 3a2f 2f61 7278 6976 2e6f 7267  ttps://arxiv.org
-00000500: 2f61 6273 2f32 3430 332e 3136 3335 3429  /abs/2403.16354)
-00000510: 2028 5b50 4446 5d28 6874 7470 733a 2f2f   ([PDF](https://
-00000520: 6769 7468 7562 2e63 6f6d 2f70 6c61 736d  github.com/plasm
-00000530: 612d 756d 6173 732f 4368 6174 4442 472f  a-umass/ChatDBG/
-00000540: 626c 6f62 2f6d 6169 6e2f 4368 6174 4442  blob/main/ChatDB
-00000550: 472d 6172 7869 762d 3234 3033 2e31 3633  G-arxiv-2403.163
-00000560: 3534 2e70 6466 2929 2e0a 0a23 2320 496e  54.pdf))...## In
-00000570: 7374 616c 6c61 7469 6f6e 0a0a 3e20 2a2a  stallation..> **
-00000580: 4e6f 7465 2a2a 0a3e 0a3e 2043 6861 7444  Note**.>.> ChatD
-00000590: 4247 206e 6565 6473 2074 6f20 6265 2063  BG needs to be c
-000005a0: 6f6e 6e65 6374 6564 2074 6f20 616e 205b  onnected to an [
-000005b0: 4f70 656e 4149 2061 6363 6f75 6e74 5d28  OpenAI account](
-000005c0: 6874 7470 733a 2f2f 6f70 656e 6169 2e63  https://openai.c
-000005d0: 6f6d 2f61 7069 2f29 2e20 5f59 6f75 7220  om/api/). _Your 
-000005e0: 6163 636f 756e 7420 7769 6c6c 206e 6565  account will nee
-000005f0: 6420 746f 2068 6176 6520 6120 706f 7369  d to have a posi
-00000600: 7469 7665 2062 616c 616e 6365 2066 6f72  tive balance for
-00000610: 2074 6869 7320 746f 2077 6f72 6b5f 2028   this to work_ (
-00000620: 5b63 6865 636b 2079 6f75 7220 6261 6c61  [check your bala
-00000630: 6e63 655d 2868 7474 7073 3a2f 2f70 6c61  nce](https://pla
-00000640: 7466 6f72 6d2e 6f70 656e 6169 2e63 6f6d  tform.openai.com
-00000650: 2f61 6363 6f75 6e74 2f75 7361 6765 2929  /account/usage))
-00000660: 2e20 4966 2079 6f75 2068 6176 6520 6e65  . If you have ne
-00000670: 7665 7220 7075 7263 6861 7365 6420 6372  ver purchased cr
-00000680: 6564 6974 732c 2079 6f75 2077 696c 6c20  edits, you will 
-00000690: 6e65 6564 2074 6f20 7075 7263 6861 7365  need to purchase
-000006a0: 2061 7420 6c65 6173 7420 5c24 3120 696e   at least \$1 in
-000006b0: 2063 7265 6469 7473 2028 6966 2079 6f75   credits (if you
-000006c0: 7220 4150 4920 6163 636f 756e 7420 7761  r API account wa
-000006d0: 7320 6372 6561 7465 6420 6265 666f 7265  s created before
-000006e0: 2041 7567 7573 7420 3133 2c20 3230 3233   August 13, 2023
-000006f0: 2920 6f72 205c 2430 2e35 3020 2869 6620  ) or \$0.50 (if 
-00000700: 796f 7520 6861 7665 2061 206e 6577 6572  you have a newer
-00000710: 2041 5049 2061 6363 6f75 6e74 2920 696e   API account) in
-00000720: 206f 7264 6572 2074 6f20 6861 7665 2061   order to have a
-00000730: 6363 6573 7320 746f 2047 5054 2d34 2c20  ccess to GPT-4, 
-00000740: 7768 6963 6820 4368 6174 4442 4720 7573  which ChatDBG us
-00000750: 6573 2e20 5b47 6574 2061 206b 6579 2068  es. [Get a key h
-00000760: 6572 652e 5d28 6874 7470 733a 2f2f 706c  ere.](https://pl
-00000770: 6174 666f 726d 2e6f 7065 6e61 692e 636f  atform.openai.co
-00000780: 6d2f 6163 636f 756e 742f 6170 692d 6b65  m/account/api-ke
-00000790: 7973 290a 3e0a 3e20 4f6e 6365 2079 6f75  ys).>.> Once you
-000007a0: 2068 6176 6520 616e 2041 5049 206b 6579   have an API key
-000007b0: 2c20 7365 7420 6974 2061 7320 616e 2065  , set it as an e
-000007c0: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
-000007d0: 626c 6520 6361 6c6c 6564 2060 4f50 454e  ble called `OPEN
-000007e0: 4149 5f41 5049 5f4b 4559 602e 0a3e 0a3e  AI_API_KEY`..>.>
-000007f0: 2060 6060 6261 7368 0a3e 2065 7870 6f72   ```bash.> expor
-00000800: 7420 4f50 454e 4149 5f41 5049 5f4b 4559  t OPENAI_API_KEY
-00000810: 3d3c 796f 7572 2d61 7069 2d6b 6579 3e0a  =<your-api-key>.
-00000820: 3e20 6060 600a 0a49 6e73 7461 6c6c 2043  > ```..Install C
-00000830: 6861 7444 4247 2075 7369 6e67 2060 7069  hatDBG using `pi
-00000840: 7060 2028 796f 7520 6e65 6564 2074 6f20  p` (you need to 
-00000850: 646f 2074 6869 7320 7768 6574 6865 7220  do this whether 
-00000860: 796f 7520 6172 6520 6465 6275 6767 696e  you are debuggin
-00000870: 6720 5079 7468 6f6e 2c20 432c 206f 7220  g Python, C, or 
-00000880: 432b 2b20 636f 6465 293a 0a0a 6060 6062  C++ code):..```b
-00000890: 6173 680a 7079 7468 6f6e 3320 2d6d 2070  ash.python3 -m p
-000008a0: 6970 2069 6e73 7461 6c6c 2063 6861 7464  ip install chatd
-000008b0: 6267 0a60 6060 0a0a 4966 2079 6f75 2061  bg.```..If you a
-000008c0: 7265 2075 7369 6e67 2043 6861 7444 4247  re using ChatDBG
-000008d0: 2074 6f20 6465 6275 6720 5079 7468 6f6e   to debug Python
-000008e0: 2070 726f 6772 616d 732c 2079 6f75 2061   programs, you a
-000008f0: 7265 2064 6f6e 652e 2049 6620 796f 7520  re done. If you 
-00000900: 7761 6e74 2074 6f20 7573 6520 4368 6174  want to use Chat
-00000910: 4442 4720 746f 2064 6562 7567 206e 6174  DBG to debug nat
-00000920: 6976 6520 636f 6465 2077 6974 6820 6067  ive code with `g
-00000930: 6462 6020 6f72 2060 6c6c 6462 602c 2066  db` or `lldb`, f
-00000940: 6f6c 6c6f 7720 7468 6520 696e 7374 616c  ollow the instal
-00000950: 6c61 7469 6f6e 2069 6e73 7472 7563 7469  lation instructi
-00000960: 6f6e 7320 6265 6c6f 772e 0a0a 2323 2320  ons below...### 
-00000970: 496e 7374 616c 6c69 6e67 2061 7320 616e  Installing as an
-00000980: 2060 6c6c 6462 6020 6578 7465 6e73 696f   `lldb` extensio
-00000990: 6e0a 0a3c 6465 7461 696c 733e 0a3c 7375  n..<details>.<su
-000009a0: 6d6d 6172 793e 0a3c 423e 3c54 543e 6c6c  mmary>.<B><TT>ll
-000009b0: 6462 3c2f 5454 3e20 696e 7374 616c 6c61  db</TT> installa
-000009c0: 7469 6f6e 2069 6e73 7472 7563 7469 6f6e  tion instruction
-000009d0: 733c 2f42 3e0a 3c2f 7375 6d6d 6172 793e  s</B>.</summary>
-000009e0: 0a0a 496e 7374 616c 6c20 4368 6174 4442  ..Install ChatDB
-000009f0: 4720 696e 746f 2074 6865 2060 6c6c 6462  G into the `lldb
-00000a00: 6020 6465 6275 6767 6572 2062 7920 7275  ` debugger by ru
-00000a10: 6e6e 696e 6720 7468 6520 666f 6c6c 6f77  nning the follow
-00000a20: 696e 6720 636f 6d6d 616e 643a 0a0a 2323  ing command:..##
-00000a30: 2323 204c 696e 7578 0a0a 6060 6062 6173  ## Linux..```bas
-00000a40: 680a 7079 7468 6f6e 3320 2d6d 2070 6970  h.python3 -m pip
-00000a50: 2069 6e73 7461 6c6c 2043 6861 7444 4247   install ChatDBG
-00000a60: 0a70 7974 686f 6e33 202d 6320 2769 6d70  .python3 -c 'imp
-00000a70: 6f72 7420 6368 6174 6462 673b 2070 7269  ort chatdbg; pri
-00000a80: 6e74 2866 2263 6f6d 6d61 6e64 2073 6372  nt(f"command scr
-00000a90: 6970 7420 696d 706f 7274 207b 6368 6174  ipt import {chat
-00000aa0: 6462 672e 5f5f 7061 7468 5f5f 5b30 5d7d  dbg.__path__[0]}
-00000ab0: 2f63 6861 7464 6267 5f6c 6c64 622e 7079  /chatdbg_lldb.py
-00000ac0: 2229 2720 3e3e 207e 2f2e 6c6c 6462 696e  ")' >> ~/.lldbin
-00000ad0: 6974 0a60 6060 0a0a 4966 2079 6f75 2065  it.```..If you e
-00000ae0: 6e63 6f75 6e74 6572 2061 6e20 6572 726f  ncounter an erro
-00000af0: 722c 2079 6f75 206d 6179 2062 6520 7573  r, you may be us
-00000b00: 696e 6720 616e 206f 6c64 6572 2076 6572  ing an older ver
-00000b10: 7369 6f6e 206f 6620 4c4c 564d 2e20 5570  sion of LLVM. Up
-00000b20: 6461 7465 2074 6f20 7468 6520 6c61 7465  date to the late
-00000b30: 7374 2076 6572 7369 6f6e 2061 7320 666f  st version as fo
-00000b40: 6c6c 6f77 733a 0a0a 6060 600a 7375 646f  llows:..```.sudo
-00000b50: 2061 7074 2069 6e73 7461 6c6c 202d 7920   apt install -y 
-00000b60: 6c73 622d 7265 6c65 6173 6520 7767 6574  lsb-release wget
-00000b70: 2073 6f66 7477 6172 652d 7072 6f70 6572   software-proper
-00000b80: 7469 6573 2d63 6f6d 6d6f 6e20 676e 7570  ties-common gnup
-00000b90: 670a 6375 726c 202d 7353 6620 6874 7470  g.curl -sSf http
-00000ba0: 733a 2f2f 6170 742e 6c6c 766d 2e6f 7267  s://apt.llvm.org
-00000bb0: 2f6c 6c76 6d2e 7368 207c 2073 7564 6f20  /llvm.sh | sudo 
-00000bc0: 6261 7368 202d 7320 2d2d 2031 3720 616c  bash -s -- 17 al
-00000bd0: 6c0a 2320 4c4c 4442 206e 6f77 2061 7661  l.# LLDB now ava
-00000be0: 696c 6162 6c65 2061 7320 606c 6c64 622d  ilable as `lldb-
-00000bf0: 3137 602e 0a60 6060 0a0a 2323 2323 204d  17`..```..#### M
-00000c00: 6163 0a0a 6060 6062 6173 680a 7863 7275  ac..```bash.xcru
-00000c10: 6e20 7079 7468 6f6e 3320 2d6d 2070 6970  n python3 -m pip
-00000c20: 2069 6e73 7461 6c6c 2043 6861 7444 4247   install ChatDBG
-00000c30: 0a78 6372 756e 2070 7974 686f 6e33 202d  .xcrun python3 -
-00000c40: 6320 2769 6d70 6f72 7420 6368 6174 6462  c 'import chatdb
-00000c50: 673b 2070 7269 6e74 2866 2263 6f6d 6d61  g; print(f"comma
-00000c60: 6e64 2073 6372 6970 7420 696d 706f 7274  nd script import
-00000c70: 207b 6368 6174 6462 672e 5f5f 7061 7468   {chatdbg.__path
-00000c80: 5f5f 5b30 5d7d 2f63 6861 7464 6267 5f6c  __[0]}/chatdbg_l
-00000c90: 6c64 622e 7079 2229 2720 3e3e 207e 2f2e  ldb.py")' >> ~/.
-00000ca0: 6c6c 6462 696e 6974 0a60 6060 0a0a 5468  lldbinit.```..Th
-00000cb0: 6973 2077 696c 6c20 696e 7374 616c 6c20  is will install 
-00000cc0: 4368 6174 4442 4720 6173 2061 6e20 4c4c  ChatDBG as an LL
-00000cd0: 564d 2065 7874 656e 7369 6f6e 2e0a 3c2f  VM extension..</
-00000ce0: 6465 7461 696c 733e 0a0a 2323 2320 496e  details>..### In
-00000cf0: 7374 616c 6c69 6e67 2061 7320 6120 6067  stalling as a `g
-00000d00: 6462 6020 6578 7465 6e73 696f 6e0a 0a3c  db` extension..<
-00000d10: 6465 7461 696c 733e 0a3c 7375 6d6d 6172  details>.<summar
-00000d20: 793e 0a3c 423e 3c54 543e 6764 623c 2f54  y>.<B><TT>gdb</T
-00000d30: 543e 2069 6e73 7461 6c6c 6174 696f 6e20  T> installation 
-00000d40: 696e 7374 7275 6374 696f 6e73 3c2f 423e  instructions</B>
-00000d50: 0a3c 2f73 756d 6d61 7279 3e0a 0a49 6e73  .</summary>..Ins
-00000d60: 7461 6c6c 2043 6861 7444 4247 2069 6e74  tall ChatDBG int
-00000d70: 6f20 7468 6520 6067 6462 6020 6465 6275  o the `gdb` debu
-00000d80: 6767 6572 2062 7920 7275 6e6e 696e 6720  gger by running 
-00000d90: 7468 6520 666f 6c6c 6f77 696e 6720 636f  the following co
-00000da0: 6d6d 616e 643a 0a0a 6060 6062 6173 680a  mmand:..```bash.
-00000db0: 7079 7468 6f6e 3320 2d6d 2070 6970 2069  python3 -m pip i
-00000dc0: 6e73 7461 6c6c 2043 6861 7444 4247 0a70  nstall ChatDBG.p
-00000dd0: 7974 686f 6e33 202d 6320 2769 6d70 6f72  ython3 -c 'impor
-00000de0: 7420 6368 6174 6462 673b 2070 7269 6e74  t chatdbg; print
-00000df0: 2866 2273 6f75 7263 6520 7b63 6861 7464  (f"source {chatd
-00000e00: 6267 2e5f 5f70 6174 685f 5f5b 305d 7d2f  bg.__path__[0]}/
-00000e10: 6368 6174 6462 675f 6764 622e 7079 2229  chatdbg_gdb.py")
-00000e20: 2720 3e3e 207e 2f2e 6764 6269 6e69 740a  ' >> ~/.gdbinit.
-00000e30: 6060 600a 0a54 6869 7320 7769 6c6c 2069  ```..This will i
-00000e40: 6e73 7461 6c6c 2043 6861 7444 4247 2061  nstall ChatDBG a
-00000e50: 7320 6120 4744 4220 6578 7465 6e73 696f  s a GDB extensio
-00000e60: 6e2e 0a3c 2f64 6574 6169 6c73 3e0a 0a23  n..</details>..#
-00000e70: 2323 2049 6e73 7461 6c6c 696e 6720 6173  ## Installing as
-00000e80: 2061 2060 5769 6e44 4247 6020 6578 7465   a `WinDBG` exte
-00000e90: 6e73 696f 6e0a 0a3c 6465 7461 696c 733e  nsion..<details>
-00000ea0: 0a3c 7375 6d6d 6172 793e 0a3c 423e 3c54  .<summary>.<B><T
-00000eb0: 543e 5769 6e44 4247 3c2f 5454 3e20 696e  T>WinDBG</TT> in
-00000ec0: 7374 616c 6c61 7469 6f6e 2069 6e73 7472  stallation instr
-00000ed0: 7563 7469 6f6e 733c 2f42 3e0a 3c2f 7375  uctions</B>.</su
-00000ee0: 6d6d 6172 793e 0a0a 312e 202a 2a49 6e73  mmary>..1. **Ins
-00000ef0: 7461 6c6c 2057 696e 4442 472a 2a3a 2046  tall WinDBG**: F
-00000f00: 6f6c 6c6f 7720 696e 7374 7275 6374 696f  ollow instructio
-00000f10: 6e73 205b 6865 7265 5d28 6874 7470 733a  ns [here](https:
-00000f20: 2f2f 6c65 6172 6e2e 6d69 6372 6f73 6f66  //learn.microsof
-00000f30: 742e 636f 6d2f 656e 2d75 732f 7769 6e64  t.com/en-us/wind
-00000f40: 6f77 732d 6861 7264 7761 7265 2f64 7269  ows-hardware/dri
-00000f50: 7665 7273 2f64 6562 7567 6765 722f 2920  vers/debugger/) 
-00000f60: 6966 2060 5769 6e44 4247 6020 6973 206e  if `WinDBG` is n
-00000f70: 6f74 2069 6e73 7461 6c6c 6564 2061 6c72  ot installed alr
-00000f80: 6561 6479 2e0a 312e 202a 2a49 6e73 7461  eady..1. **Insta
-00000f90: 6c6c 2060 7663 706b 6760 2a2a 3a20 466f  ll `vcpkg`**: Fo
-00000fa0: 6c6c 6f77 2069 6e73 7472 7563 7469 6f6e  llow instruction
-00000fb0: 7320 5b68 6572 655d 2868 7474 7073 3a2f  s [here](https:/
-00000fc0: 2f76 6370 6b67 2e69 6f2f 656e 2f67 6574  /vcpkg.io/en/get
-00000fd0: 7469 6e67 2d73 7461 7274 6564 2920 6966  ting-started) if
-00000fe0: 2060 7663 706b 6760 2069 7320 6e6f 7420   `vcpkg` is not 
-00000ff0: 696e 7374 616c 6c65 6420 616c 7265 6164  installed alread
-00001000: 792e 0a31 2e20 2a2a 496e 7374 616c 6c20  y..1. **Install 
-00001010: 4465 6275 6767 696e 6720 546f 6f6c 7320  Debugging Tools 
-00001020: 666f 7220 5769 6e64 6f77 732a 2a3a 2049  for Windows**: I
-00001030: 6e73 7461 6c6c 2074 6865 2057 696e 646f  nstall the Windo
-00001040: 7773 2053 444b 205b 6865 7265 5d28 6874  ws SDK [here](ht
-00001050: 7470 733a 2f2f 6465 7665 6c6f 7065 722e  tps://developer.
-00001060: 6d69 6372 6f73 6f66 742e 636f 6d2f 656e  microsoft.com/en
-00001070: 2d75 732f 7769 6e64 6f77 732f 646f 776e  -us/windows/down
-00001080: 6c6f 6164 732f 7769 6e64 6f77 732d 7364  loads/windows-sd
-00001090: 6b2f 2920 616e 6420 6368 6563 6b20 7468  k/) and check th
-000010a0: 6520 626f 7820 6044 6562 7567 6769 6e67  e box `Debugging
-000010b0: 2054 6f6f 6c73 2066 6f72 2057 696e 646f   Tools for Windo
-000010c0: 7773 602e 0a31 2e20 2a2a 4e61 7669 6761  ws`..1. **Naviga
-000010d0: 7465 2074 6f20 7468 6520 6073 7263 5c63  te to the `src\c
-000010e0: 6861 7464 6267 6020 6469 7265 6374 6f72  hatdbg` director
-000010f0: 792a 2a3a 2060 6364 2073 7263 5c63 6861  y**: `cd src\cha
-00001100: 7464 6267 600a 312e 202a 2a49 6e73 7461  tdbg`.1. **Insta
-00001110: 6c6c 206e 6565 6465 6420 6465 7065 6e64  ll needed depend
-00001120: 656e 6369 6573 2a2a 3a20 5275 6e60 7663  encies**: Run`vc
-00001130: 706b 6720 696e 7374 616c 6c60 0a31 2e20  pkg install`.1. 
-00001140: 2a2a 4275 696c 6420 7468 6520 6368 6174  **Build the chat
-00001150: 6462 672e 646c 6c20 6578 7465 6e73 696f  dbg.dll extensio
-00001160: 6e2a 2a3a 2052 756e 606d 6b64 6972 2062  n**: Run`mkdir b
-00001170: 7569 6c64 2026 2063 6420 6275 696c 6420  uild & cd build 
-00001180: 2620 636d 616b 6520 2e2e 2026 2063 6d61  & cmake .. & cma
-00001190: 6b65 202d 2d62 7569 6c64 202e 2026 2063  ke --build . & c
-000011a0: 6420 2e2e 600a 0a2a 2a55 7369 6e67 2043  d ..`..**Using C
-000011b0: 6861 7444 4247 2a2a 3a0a 0a20 2a20 4c6f  hatDBG**:.. * Lo
-000011c0: 6164 2069 6e74 6f20 5769 6e44 4247 583a  ad into WinDBGX:
-000011d0: 0a20 2020 2a20 5275 6e20 6077 696e 6462  .   * Run `windb
-000011e0: 6778 2079 6f75 725f 6578 6563 7574 6162  gx your_executab
-000011f0: 6c65 5f68 6572 652e 6578 6560 0a20 2020  le_here.exe`.   
-00001200: 2a20 436c 6963 6b20 7468 6520 6d65 6e75  * Click the menu
-00001210: 2069 7465 6d73 2060 5669 6577 6020 2d3e   items `View` ->
-00001220: 2060 436f 6d6d 616e 6420 6272 6f77 7365   `Command browse
-00001230: 7260 0a20 2020 2a20 5479 7065 2060 2e6c  r`.   * Type `.l
-00001240: 6f61 6420 6465 6275 675c 6368 6174 6462  oad debug\chatdb
-00001250: 672e 646c 6c60 0a20 2a20 4166 7465 7220  g.dll`. * After 
-00001260: 7275 6e6e 696e 6720 636f 6465 2061 6e64  running code and
-00001270: 2068 6974 7469 6e67 2061 6e20 6578 6365   hitting an exce
-00001280: 7074 696f 6e20 2f20 7369 676e 616c 3a0a  ption / signal:.
-00001290: 2020 202a 2054 7970 6520 6021 7768 7960     * Type `!why`
-000012a0: 2069 6e20 436f 6d6d 616e 6420 6272 6f77   in Command brow
-000012b0: 7365 720a 3c2f 6465 7461 696c 733e 0a0a  ser.</details>..
-000012c0: 0a23 2320 5573 6167 650a 0a23 2323 2044  .## Usage..### D
-000012d0: 6562 7567 6769 6e67 2050 7974 686f 6e0a  ebugging Python.
-000012e0: 0a54 6f20 7573 6520 4368 6174 4442 4720  .To use ChatDBG 
-000012f0: 746f 2064 6562 7567 2050 7974 686f 6e20  to debug Python 
-00001300: 7072 6f67 7261 6d73 2c20 7369 6d70 6c79  programs, simply
-00001310: 2072 756e 2079 6f75 7220 5079 7468 6f6e   run your Python
-00001320: 2073 6372 6970 7420 6173 2066 6f6c 6c6f   script as follo
-00001330: 7773 3a0a 0a60 6060 6261 7368 0a63 6861  ws:..```bash.cha
-00001340: 7464 6267 202d 6320 636f 6e74 696e 7565  tdbg -c continue
-00001350: 2079 6f75 7273 6372 6970 742e 7079 0a60   yourscript.py.`
-00001360: 6060 0a0a 4368 6174 4442 4720 6973 2061  ``..ChatDBG is a
-00001370: 6e20 6578 7465 6e73 696f 6e20 6f66 2074  n extension of t
-00001380: 6865 2073 7461 6e64 6172 6420 5079 7468  he standard Pyth
-00001390: 6f6e 2064 6562 7567 6765 7220 6070 6462  on debugger `pdb
-000013a0: 602e 204c 696b 650a 6070 6462 602c 2077  `. Like.`pdb`, w
-000013b0: 6865 6e20 796f 7572 2073 6372 6970 7420  hen your script 
-000013c0: 656e 636f 756e 7465 7273 2061 6e20 756e  encounters an un
-000013d0: 6361 7567 6874 2065 7863 6570 7469 6f6e  caught exception
-000013e0: 2c20 4368 6174 4442 4720 7769 6c6c 0a65  , ChatDBG will.e
-000013f0: 6e74 6572 2070 6f73 7420 6d6f 7274 656d  nter post mortem
-00001400: 2064 6562 7567 6769 6e67 206d 6f64 652e   debugging mode.
-00001410: 0a0a 556e 6c69 6b65 206f 7468 6572 2064  ..Unlike other d
-00001420: 6562 7567 6765 7273 2c20 796f 7520 6361  ebuggers, you ca
-00001430: 6e20 7468 656e 2075 7365 2074 6865 2060  n then use the `
-00001440: 7768 7960 2063 6f6d 6d61 6e64 2074 6f20  why` command to 
-00001450: 6173 6b0a 4368 6174 4442 4720 7768 7920  ask.ChatDBG why 
-00001460: 796f 7572 2070 726f 6772 616d 2066 6169  your program fai
-00001470: 6c65 6420 616e 6420 6765 7420 6120 7375  led and get a su
-00001480: 6767 6573 7465 6420 6669 782e 0a0a 2323  ggested fix...##
-00001490: 2323 2049 5079 7468 6f6e 2061 6e64 204a  ## IPython and J
-000014a0: 7570 7974 6572 2053 7570 706f 7274 0a0a  upyter Support..
-000014b0: 546f 2075 7365 2043 6861 7444 4247 2061  To use ChatDBG a
-000014c0: 7320 7468 6520 6465 6661 756c 7420 6465  s the default de
-000014d0: 6275 6767 6572 2066 6f72 2049 5079 7468  bugger for IPyth
-000014e0: 6f6e 206f 7220 696e 7369 6465 204a 7570  on or inside Jup
-000014f0: 7974 6572 204e 6f74 6562 6f6f 6b73 2c0a  yter Notebooks,.
-00001500: 6372 6561 7465 2061 2049 5079 7468 6f6e  create a IPython
-00001510: 2070 726f 6669 6c65 2061 6e64 2074 6865   profile and the
-00001520: 6e20 6164 6420 7468 6520 6e65 6365 7373  n add the necess
-00001530: 6172 7920 6578 656e 7369 6f6e 7320 6f6e  ary exensions on
-00001540: 2073 7461 7274 7570 2e20 2028 4d6f 6469   startup.  (Modi
-00001550: 6679 0a74 6865 7365 206c 696e 6573 2061  fy.these lines a
-00001560: 7320 6e65 6365 7373 6172 7920 6966 2079  s necessary if y
-00001570: 6f75 2061 6c72 6561 6479 2068 6176 6520  ou already have 
-00001580: 6120 6375 7374 6f6d 697a 6564 2070 726f  a customized pro
-00001590: 6669 6c65 2066 696c 652e 290a 0a60 6060  file file.)..```
-000015a0: 6261 7368 0a69 7079 7468 6f6e 2070 726f  bash.ipython pro
-000015b0: 6669 6c65 2063 7265 6174 650a 6563 686f  file create.echo
-000015c0: 2022 632e 496e 7465 7261 6374 6976 6553   "c.InteractiveS
-000015d0: 6865 6c6c 4170 702e 6578 7465 6e73 696f  hellApp.extensio
-000015e0: 6e73 203d 205b 2763 6861 7464 6267 2e63  ns = ['chatdbg.c
-000015f0: 6861 7464 6267 5f70 6462 272c 2027 6970  hatdbg_pdb', 'ip
-00001600: 7966 6c6f 7727 5d22 203e 3e20 7e2f 2e69  yflow']" >> ~/.i
-00001610: 7079 7468 6f6e 2f70 726f 6669 6c65 5f64  python/profile_d
-00001620: 6566 6175 6c74 2f69 7079 7468 6f6e 5f63  efault/ipython_c
-00001630: 6f6e 6669 672e 7079 0a60 6060 0a0a 4f6e  onfig.py.```..On
-00001640: 2074 6865 2063 6f6d 6d61 6e64 206c 696e   the command lin
-00001650: 652c 2079 6f75 2063 616e 2074 6865 6e20  e, you can then 
-00001660: 7275 6e3a 0a0a 6060 6062 6173 680a 6970  run:..```bash.ip
-00001670: 7974 686f 6e20 2d2d 7064 6220 796f 7572  ython --pdb your
-00001680: 7363 7269 7074 2e70 790a 6060 600a 0a49  script.py.```..I
-00001690: 6e73 6964 6520 4a75 7079 7465 722c 2072  nside Jupyter, r
-000016a0: 756e 2079 6f75 7220 6e6f 7465 626f 6f6b  un your notebook
-000016b0: 2077 6974 6820 7468 6520 5b69 7079 666c   with the [ipyfl
-000016c0: 6f77 206b 6572 6e65 6c5d 2868 7474 7073  ow kernel](https
-000016d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6970  ://github.com/ip
-000016e0: 7966 6c6f 772f 6970 7966 6c6f 7729 2061  yflow/ipyflow) a
-000016f0: 6e64 2069 6e63 6c75 6465 2074 6869 7320  nd include this 
-00001700: 6c69 6e65 206d 6167 6963 2061 7420 7468  line magic at th
-00001710: 6520 746f 7020 6f66 2074 6865 2066 696c  e top of the fil
-00001720: 652e 0a0a 6060 600a 2570 6462 0a60 6060  e...```.%pdb.```
-00001730: 0a0a 0a23 2323 2044 6562 7567 6769 6e67  ...### Debugging
-00001740: 206e 6174 6976 6520 636f 6465 2028 432c   native code (C,
-00001750: 2043 2b2b 2c20 6f72 2052 7573 7420 7769   C++, or Rust wi
-00001760: 7468 203c 5454 3e6c 6c64 623c 2f54 543e  th <TT>lldb</TT>
-00001770: 202f 203c 5454 3e67 6462 3c2f 5454 3e29   / <TT>gdb</TT>)
-00001780: 0a0a 546f 2075 7365 2043 6861 7444 4247  ..To use ChatDBG
-00001790: 2077 6974 6820 606c 6c64 6260 206f 7220   with `lldb` or 
-000017a0: 6067 6462 602c 206a 7573 7420 7275 6e20  `gdb`, just run 
-000017b0: 6e61 7469 7665 2063 6f64 6520 2863 6f6d  native code (com
-000017c0: 7069 6c65 6420 7769 7468 2060 2d67 6020  piled with `-g` 
-000017d0: 666f 7220 6465 6275 6767 696e 6720 7379  for debugging sy
-000017e0: 6d62 6f6c 7329 2077 6974 6820 796f 7572  mbols) with your
-000017f0: 2063 686f 6963 6520 6f66 2064 6562 7567   choice of debug
-00001800: 6765 723b 2077 6865 6e20 6974 2063 7261  ger; when it cra
-00001810: 7368 6573 2c20 6173 6b20 6077 6879 602e  shes, ask `why`.
-00001820: 2054 6869 7320 616c 736f 2077 6f72 6b73   This also works
-00001830: 2066 6f72 2070 6f73 7420 6d6f 7274 656d   for post mortem
-00001840: 2064 6562 7567 6769 6e67 2028 7768 656e   debugging (when
-00001850: 2079 6f75 206c 6f61 6420 6120 636f 7265   you load a core
-00001860: 2077 6974 6820 7468 6520 602d 6360 206f   with the `-c` o
-00001870: 7074 696f 6e29 2e0a 0a3c 6465 7461 696c  ption)...<detail
-00001880: 733e 0a3c 7375 6d6d 6172 793e 0a3c 423e  s>.<summary>.<B>
-00001890: 4465 6275 6767 696e 6720 5275 7374 2070  Debugging Rust p
-000018a0: 726f 6772 616d 733c 2f42 3e0a 3c2f 7375  rograms</B>.</su
-000018b0: 6d6d 6172 793e 0a0a 546f 2075 7365 2043  mmary>..To use C
-000018c0: 6861 7444 4247 2077 6974 6820 5275 7374  hatDBG with Rust
-000018d0: 2c20 796f 7520 6e65 6564 2074 6f20 646f  , you need to do
-000018e0: 2074 776f 2073 7465 7073 3a20 6d6f 6469   two steps: modi
-000018f0: 6679 2079 6f75 720a 6043 6172 676f 2e74  fy your.`Cargo.t
-00001900: 6f6d 6c60 2066 696c 6520 616e 6420 6164  oml` file and ad
-00001910: 6420 6f6e 6520 6c69 6e65 2074 6f20 796f  d one line to yo
-00001920: 7572 2073 6f75 7263 6520 7072 6f67 7261  ur source progra
-00001930: 6d2e 0a0a 312e 2041 6464 2074 6869 7320  m...1. Add this 
-00001940: 746f 2079 6f75 7220 6043 6172 676f 2e74  to your `Cargo.t
-00001950: 6f6d 6c60 2066 696c 653a 0a0a 6060 6074  oml` file:..```t
-00001960: 6f6d 6c0a 5b64 6570 656e 6465 6e63 6965  oml.[dependencie
-00001970: 735d 0a63 6861 7464 6267 203d 2022 302e  s].chatdbg = "0.
-00001980: 312e 3322 0a0a 5b70 726f 6669 6c65 2e64  1.3"..[profile.d
-00001990: 6576 5d0a 7061 6e69 6320 3d20 2261 626f  ev].panic = "abo
-000019a0: 7274 220a 0a5b 7072 6f66 696c 652e 7265  rt"..[profile.re
-000019b0: 6c65 6173 655d 0a70 616e 6963 203d 2022  lease].panic = "
-000019c0: 6162 6f72 7422 0a60 6060 0a0a 322e 2049  abort".```..2. I
-000019d0: 6e20 796f 7572 2070 726f 6772 616d 2c20  n your program, 
-000019e0: 6170 706c 7920 7468 6520 6023 5b63 6861  apply the `#[cha
-000019f0: 7464 6267 3a3a 6d61 696e 5d60 2061 7474  tdbg::main]` att
-00001a00: 7269 6275 7465 2074 6f20 796f 7572 2060  ribute to your `
-00001a10: 6d61 696e 600a 6675 6e63 7469 6f6e 3a0a  main`.function:.
-00001a20: 0a60 6060 7275 7374 0a23 5b63 6861 7464  .```rust.#[chatd
-00001a30: 6267 3a3a 6d61 696e 5d0a 666e 206d 6169  bg::main].fn mai
-00001a40: 6e28 2920 7b0a 6060 600a 0a4e 6f77 2079  n() {.```..Now y
-00001a50: 6f75 2063 616e 2064 6562 7567 2079 6f75  ou can debug you
-00001a60: 7220 5275 7374 2063 6f64 6520 7769 7468  r Rust code with
-00001a70: 2060 6764 6260 206f 7220 606c 6c64 6260   `gdb` or `lldb`
-00001a80: 2e0a 0a3c 2f64 6574 6169 6c73 3e0a 0a23  ...</details>..#
-00001a90: 2323 2045 7861 6d70 6c65 730a 0a3c 6465  ## Examples..<de
-00001aa0: 7461 696c 733e 0a3c 7375 6d6d 6172 793e  tails>.<summary>
-00001ab0: 0a3c 423e 4368 6174 4442 4720 6578 616d  .<B>ChatDBG exam
-00001ac0: 706c 6520 696e 203c 5454 3e6c 6c64 623c  ple in <TT>lldb<
-00001ad0: 2f54 543e 3c2f 423e 0a3c 2f73 756d 6d61  /TT></B>.</summa
-00001ae0: 7279 3e0a 0a60 6060 6764 620a 2843 6861  ry>..```gdb.(Cha
-00001af0: 7444 4247 206c 6c64 6229 2072 756e 0a50  tDBG lldb) run.P
-00001b00: 726f 6365 7373 2038 3534 3934 206c 6175  rocess 85494 lau
-00001b10: 6e63 6865 643a 2027 2f55 7365 7273 2f65  nched: '/Users/e
-00001b20: 6d65 7279 2f67 6974 2f43 6861 7444 4247  mery/git/ChatDBG
-00001b30: 2f74 6573 742f 612e 6f75 7427 2028 6172  /test/a.out' (ar
-00001b40: 6d36 3429 0a54 4553 5420 310a 5445 5354  m64).TEST 1.TEST
-00001b50: 202d 3432 3237 3631 3238 380a 5445 5354   -422761288.TEST
-00001b60: 2030 0a54 4553 5420 300a 5445 5354 2030   0.TEST 0.TEST 0
-00001b70: 0a54 4553 5420 300a 5445 5354 2030 0a54  .TEST 0.TEST 0.T
-00001b80: 4553 5420 300a 5072 6f63 6573 7320 3835  EST 0.Process 85
-00001b90: 3439 3420 7374 6f70 7065 640a 2a20 7468  494 stopped.* th
-00001ba0: 7265 6164 2023 312c 2071 7565 7565 203d  read #1, queue =
-00001bb0: 2027 636f 6d2e 6170 706c 652e 6d61 696e   'com.apple.main
-00001bc0: 2d74 6872 6561 6427 2c20 7374 6f70 2072  -thread', stop r
-00001bd0: 6561 736f 6e20 3d20 4558 435f 4241 445f  eason = EXC_BAD_
-00001be0: 4143 4345 5353 2028 636f 6465 3d31 2c20  ACCESS (code=1, 
-00001bf0: 6164 6472 6573 733d 3078 3130 3030 3536  address=0x100056
-00001c00: 3230 3029 0a20 2020 2066 7261 6d65 2023  200).    frame #
-00001c10: 303a 2030 7830 3030 3030 3030 3130 3030  0: 0x00000001000
-00001c20: 3032 6636 3420 612e 6f75 7460 666f 6f28  02f64 a.out`foo(
-00001c30: 6e3d 382c 2062 3d31 2920 6174 2074 6573  n=8, b=1) at tes
-00001c40: 742e 6370 703a 373a 3232 0a20 2020 3420  t.cpp:7:22.   4 
-00001c50: 2020 2020 696e 7420 785b 5d20 3d20 7b20      int x[] = { 
-00001c60: 312c 2032 2c20 332c 2034 2c20 3520 7d3b  1, 2, 3, 4, 5 };
-00001c70: 0a20 2020 3520 2020 2020 0a20 2020 3620  .   5     .   6 
-00001c80: 2020 2020 766f 6964 2066 6f6f 2869 6e74      void foo(int
-00001c90: 206e 2c20 666c 6f61 7420 6229 207b 0a2d   n, float b) {.-
-00001ca0: 3e20 3720 2020 2020 2020 636f 7574 203c  > 7       cout <
-00001cb0: 3c20 2254 4553 5420 2220 3c3c 2078 5b6e  < "TEST " << x[n
-00001cc0: 202a 2031 3030 3030 5d20 3c3c 2065 6e64   * 10000] << end
-00001cd0: 6c3b 0a20 2020 3820 2020 2020 7d0a 2020  l;.   8     }.  
-00001ce0: 2039 2020 2020 200a 2020 2031 3020 2020   9     .   10   
-00001cf0: 2069 6e74 206d 6169 6e28 290a 5461 7267   int main().Targ
-00001d00: 6574 2030 3a20 2861 2e6f 7574 2920 7374  et 0: (a.out) st
-00001d10: 6f70 7065 642e 0a60 6060 0a0a 4173 6b20  opped..```..Ask 
-00001d20: 6077 6879 6020 746f 2068 6176 6520 4368  `why` to have Ch
-00001d30: 6174 4442 4720 7072 6f76 6964 6520 6120  atDBG provide a 
-00001d40: 6865 6c70 6675 6c20 6578 706c 616e 6174  helpful explanat
-00001d50: 696f 6e20 7768 7920 7468 6973 2070 726f  ion why this pro
-00001d60: 6772 616d 2066 6169 6c65 642c 2061 6e64  gram failed, and
-00001d70: 2073 7567 6765 7374 2061 2066 6978 3a0a   suggest a fix:.
-00001d80: 0a0a 6060 6067 6462 0a28 4368 6174 4442  ..```gdb.(ChatDB
-00001d90: 4720 6c6c 6462 2920 7768 790a 5468 6520  G lldb) why.The 
-00001da0: 726f 6f74 2063 6175 7365 206f 6620 7468  root cause of th
-00001db0: 6973 2065 7272 6f72 2069 7320 6163 6365  is error is acce
-00001dc0: 7373 696e 6720 616e 2069 6e64 6578 206f  ssing an index o
-00001dd0: 6620 7468 6520 6172 7261 7920 6078 600a  f the array `x`.
-00001de0: 7468 6174 2069 7320 6f75 7420 6f66 2062  that is out of b
-00001df0: 6f75 6e64 732e 2049 6e20 6066 6f6f 2829  ounds. In `foo()
-00001e00: 602c 2074 6865 2069 6e64 6578 2069 7320  `, the index is 
-00001e10: 6361 6c63 756c 6174 6564 2061 7320 606e  calculated as `n
-00001e20: 202a 0a31 3030 3030 602c 2077 6869 6368   *.10000`, which
-00001e30: 2063 616e 2062 6520 6d75 6368 206c 6172   can be much lar
-00001e40: 6765 7220 7468 616e 2074 6865 2073 697a  ger than the siz
-00001e50: 6520 6f66 2074 6865 2061 7272 6179 2060  e of the array `
-00001e60: 7860 2028 7768 6963 680a 6973 206f 6e6c  x` (which.is onl
-00001e70: 7920 3520 656c 656d 656e 7473 292e 2049  y 5 elements). I
-00001e80: 6e20 7468 6520 6769 7665 6e20 7472 6163  n the given trac
-00001e90: 652c 2074 6865 2070 726f 6772 616d 2069  e, the program i
-00001ea0: 7320 7472 7969 6e67 2074 6f0a 6163 6365  s trying to.acce
-00001eb0: 7373 2074 6865 206d 656d 6f72 7920 6164  ss the memory ad
-00001ec0: 6472 6573 7320 6030 7831 3030 3035 3632  dress `0x1000562
-00001ed0: 3030 602c 2077 6869 6368 2069 7320 6f75  00`, which is ou
-00001ee0: 7473 6964 6520 6f66 2074 6865 2072 616e  tside of the ran
-00001ef0: 6765 0a6f 6620 616c 6c6f 6361 7465 6420  ge.of allocated 
-00001f00: 6d65 6d6f 7279 2066 6f72 2074 6865 2061  memory for the a
-00001f10: 7272 6179 2060 7860 2e0a 0a54 6f20 6669  rray `x`...To fi
-00001f20: 7820 7468 6973 2065 7272 6f72 2c20 7765  x this error, we
-00001f30: 206e 6565 6420 746f 2065 6e73 7572 6520   need to ensure 
-00001f40: 7468 6174 2074 6865 2069 6e64 6578 2069  that the index i
-00001f50: 7320 7769 7468 696e 2074 6865 0a62 6f75  s within the.bou
-00001f60: 6e64 7320 6f66 2074 6865 2061 7272 6179  nds of the array
-00001f70: 2e20 4f6e 6520 7761 7920 746f 2064 6f20  . One way to do 
-00001f80: 7468 6973 2069 7320 746f 2063 6865 636b  this is to check
-00001f90: 2074 6865 2076 616c 7565 206f 6620 606e   the value of `n
-00001fa0: 600a 6265 666f 7265 2063 616c 6375 6c61  `.before calcula
-00001fb0: 7469 6e67 2074 6865 2069 6e64 6578 2c20  ting the index, 
-00001fc0: 616e 6420 656e 7375 7265 2074 6861 7420  and ensure that 
-00001fd0: 6974 2069 7320 6c65 7373 2074 6861 6e20  it is less than 
-00001fe0: 7468 6520 7369 7a65 0a6f 6620 7468 6520  the size.of the 
-00001ff0: 6172 7261 7920 6469 7669 6465 6420 6279  array divided by
-00002000: 2074 6865 2073 697a 6520 6f66 2074 6865   the size of the
-00002010: 2065 6c65 6d65 6e74 2e20 466f 7220 6578   element. For ex
-00002020: 616d 706c 652c 2077 6520 6361 6e0a 6d6f  ample, we can.mo
-00002030: 6469 6679 2060 666f 6f28 2960 2061 7320  dify `foo()` as 
-00002040: 666f 6c6c 6f77 733a 0a0a 2020 2020 6060  follows:..    ``
-00002050: 600a 2020 2020 766f 6964 2066 6f6f 2869  `.    void foo(i
-00002060: 6e74 206e 2c20 666c 6f61 7420 6229 207b  nt n, float b) {
-00002070: 0a20 2020 2020 2069 6620 286e 203c 2030  .      if (n < 0
-00002080: 207c 7c20 6e20 3e3d 2073 697a 656f 6628   || n >= sizeof(
-00002090: 7829 2f73 697a 656f 6628 785b 305d 2929  x)/sizeof(x[0]))
-000020a0: 207b 0a20 2020 2020 2020 2063 6f75 7420   {.        cout 
-000020b0: 3c3c 2022 4552 524f 523a 2049 6e76 616c  << "ERROR: Inval
-000020c0: 6964 2069 6e64 6578 2220 3c3c 2065 6e64  id index" << end
-000020d0: 6c3b 0a20 2020 2020 2020 2072 6574 7572  l;.        retur
-000020e0: 6e3b 0a20 2020 2020 207d 0a20 2020 2020  n;.      }.     
-000020f0: 2063 6f75 7420 3c3c 2022 5445 5354 2022   cout << "TEST "
-00002100: 203c 3c20 785b 6e5d 203c 3c20 656e 646c   << x[n] << endl
-00002110: 3b0a 2020 2020 7d0a 2020 2020 6060 600a  ;.    }.    ```.
-00002120: 0a54 6869 7320 636f 6465 2063 6865 636b  .This code check
-00002130: 7320 6966 2060 6e60 2069 7320 7769 7468  s if `n` is with
-00002140: 696e 2074 6865 2076 616c 6964 2072 616e  in the valid ran
-00002150: 6765 2c20 616e 6420 7072 696e 7473 2061  ge, and prints a
-00002160: 6e20 6572 726f 720a 6d65 7373 6167 6520  n error.message 
-00002170: 6966 2069 7420 6973 206e 6f74 2e20 4966  if it is not. If
-00002180: 2060 6e60 2069 7320 7769 7468 696e 2074   `n` is within t
-00002190: 6865 2072 616e 6765 2c20 7468 6520 6675  he range, the fu
-000021a0: 6e63 7469 6f6e 2070 7269 6e74 730a 7468  nction prints.th
-000021b0: 6520 7661 6c75 6520 6f66 2074 6865 2065  e value of the e
-000021c0: 6c65 6d65 6e74 2061 7420 696e 6465 7820  lement at index 
-000021d0: 606e 6020 6f66 2060 7860 2e20 5769 7468  `n` of `x`. With
-000021e0: 2074 6869 7320 6d6f 6469 6669 6361 7469   this modificati
-000021f0: 6f6e 2c0a 7468 6520 7072 6f67 7261 6d20  on,.the program 
-00002200: 7769 6c6c 2061 766f 6964 2061 6363 6573  will avoid acces
-00002210: 7369 6e67 206d 656d 6f72 7920 6f75 7473  sing memory outs
-00002220: 6964 6520 7468 6520 626f 756e 6473 206f  ide the bounds o
-00002230: 6620 7468 650a 6172 7261 792c 2061 6e64  f the.array, and
-00002240: 2077 696c 6c20 7072 696e 7420 7468 6520   will print the 
-00002250: 6578 7065 6374 6564 206f 7574 7075 7420  expected output 
-00002260: 666f 7220 7661 6c69 6420 696e 6469 6365  for valid indice
-00002270: 732e 0a60 6060 0a3c 2f64 6574 6169 6c73  s..```.</details
-00002280: 3e0a 0a3c 6465 7461 696c 733e 0a3c 7375  >..<details>.<su
-00002290: 6d6d 6172 793e 0a3c 423e 4368 6174 4442  mmary>.<B>ChatDB
-000022a0: 4720 6578 616d 706c 6520 696e 2050 7974  G example in Pyt
-000022b0: 686f 6e20 283c 5454 3e70 6462 3c2f 5454  hon (<TT>pdb</TT
-000022c0: 3e29 3c2f 423e 0a3c 2f73 756d 6d61 7279  >)</B>.</summary
-000022d0: 3e0a 0a60 6060 7079 7468 6f6e 0a54 7261  >..```python.Tra
-000022e0: 6365 6261 636b 2028 6d6f 7374 2072 6563  ceback (most rec
-000022f0: 656e 7420 6361 6c6c 206c 6173 7429 3a0a  ent call last):.
-00002300: 2020 4669 6c65 2022 796f 7572 7363 7269    File "yourscri
-00002310: 7074 2e70 7922 2c20 6c69 6e65 2039 2c20  pt.py", line 9, 
-00002320: 696e 203c 6d6f 6475 6c65 3e0a 2020 2020  in <module>.    
-00002330: 7072 696e 7428 7472 796d 6528 3130 3029  print(tryme(100)
-00002340: 290a 2020 4669 6c65 2022 796f 7572 7363  ).  File "yoursc
-00002350: 7269 7074 2e70 7922 2c20 6c69 6e65 2034  ript.py", line 4
-00002360: 2c20 696e 2074 7279 6d65 0a20 2020 2069  , in tryme.    i
-00002370: 6620 7820 2f20 6920 3e20 323a 0a5a 6572  f x / i > 2:.Zer
-00002380: 6f44 6976 6973 696f 6e45 7272 6f72 3a20  oDivisionError: 
-00002390: 6469 7669 7369 6f6e 2062 7920 7a65 726f  division by zero
-000023a0: 0a55 6e63 6175 6768 7420 6578 6365 7074  .Uncaught except
-000023b0: 696f 6e2e 2045 6e74 6572 696e 6720 706f  ion. Entering po
-000023c0: 7374 206d 6f72 7465 6d20 6465 6275 6767  st mortem debugg
-000023d0: 696e 670a 5275 6e6e 696e 6720 2763 6f6e  ing.Running 'con
-000023e0: 7427 206f 7220 2773 7465 7027 2077 696c  t' or 'step' wil
-000023f0: 6c20 7265 7374 6172 7420 7468 6520 7072  l restart the pr
-00002400: 6f67 7261 6d0a 3e20 796f 7572 7363 7269  ogram.> yourscri
-00002410: 7074 2e70 7928 3429 7472 796d 6528 290a  pt.py(4)tryme().
-00002420: 2d3e 2069 6620 7820 2f20 6920 3e20 323a  -> if x / i > 2:
-00002430: 0a60 6060 0a0a 4173 6b20 6077 6879 6020  .```..Ask `why` 
-00002440: 746f 2068 6176 6520 4368 6174 4442 4720  to have ChatDBG 
-00002450: 7072 6f76 6964 6520 6120 6865 6c70 6675  provide a helpfu
-00002460: 6c20 6578 706c 616e 6174 696f 6e20 7768  l explanation wh
-00002470: 7920 7468 6973 2070 726f 6772 616d 2066  y this program f
-00002480: 6169 6c65 642c 2061 6e64 2073 7567 6765  ailed, and sugge
-00002490: 7374 2061 2066 6978 3a0a 0a60 6060 7079  st a fix:..```py
-000024a0: 7468 6f6e 0a28 4368 6174 4442 4720 5064  thon.(ChatDBG Pd
-000024b0: 6229 2077 6879 0a54 6865 2072 6f6f 7420  b) why.The root 
-000024c0: 6361 7573 6520 6f66 2074 6865 2065 7272  cause of the err
-000024d0: 6f72 2069 7320 7468 6174 2074 6865 2063  or is that the c
-000024e0: 6f64 6520 6973 2061 7474 656d 7074 696e  ode is attemptin
-000024f0: 6720 746f 0a64 6976 6964 6520 6279 207a  g to.divide by z
-00002500: 6572 6f20 696e 2074 6865 206c 696e 6520  ero in the line 
-00002510: 2269 6620 7820 2f20 6920 3e20 3222 2e20  "if x / i > 2". 
-00002520: 4173 2069 2072 616e 6765 7320 6672 6f6d  As i ranges from
-00002530: 2030 2074 6f20 3939 2c0a 6974 2077 696c   0 to 99,.it wil
-00002540: 6c20 6576 656e 7475 616c 6c79 2072 6561  l eventually rea
-00002550: 6368 2074 6865 2076 616c 7565 206f 6620  ch the value of 
-00002560: 302c 2063 6175 7369 6e67 2061 205a 6572  0, causing a Zer
-00002570: 6f44 6976 6973 696f 6e45 7272 6f72 2e0a  oDivisionError..
-00002580: 0a41 2070 6f73 7369 626c 6520 6669 7820  .A possible fix 
-00002590: 666f 7220 7468 6973 2077 6f75 6c64 2062  for this would b
-000025a0: 6520 746f 2061 6464 2061 2063 6865 636b  e to add a check
-000025b0: 2066 6f72 2069 2062 6569 6e67 2065 7175   for i being equ
-000025c0: 616c 2074 6f0a 7a65 726f 2062 6566 6f72  al to.zero befor
-000025d0: 6520 7065 7266 6f72 6d69 6e67 2074 6865  e performing the
-000025e0: 2064 6976 6973 696f 6e2e 2054 6869 7320   division. This 
-000025f0: 636f 756c 6420 6265 2064 6f6e 6520 6279  could be done by
-00002600: 2061 6464 696e 6720 616e 0a61 6464 6974   adding an.addit
-00002610: 696f 6e61 6c20 636f 6e64 6974 696f 6e61  ional conditiona
-00002620: 6c20 7374 6174 656d 656e 742c 2073 7563  l statement, suc
-00002630: 6820 6173 2022 6966 2069 203d 3d20 303a  h as "if i == 0:
-00002640: 2063 6f6e 7469 6e75 6522 2c20 746f 0a73   continue", to.s
-00002650: 6b69 7020 6f76 6572 2074 6865 2069 7465  kip over the ite
-00002660: 7261 7469 6f6e 2077 6865 6e20 6920 6973  ration when i is
-00002670: 207a 6572 6f2e 2054 6865 2075 7064 6174   zero. The updat
-00002680: 6564 2063 6f64 6520 776f 756c 6420 6c6f  ed code would lo
-00002690: 6f6b 0a6c 696b 6520 7468 6973 3a0a 0a64  ok.like this:..d
-000026a0: 6566 2074 7279 6d65 2878 293a 0a20 2020  ef tryme(x):.   
-000026b0: 2063 6f75 6e74 203d 2030 0a20 2020 2066   count = 0.    f
-000026c0: 6f72 2069 2069 6e20 7261 6e67 6528 3130  or i in range(10
-000026d0: 3029 3a0a 2020 2020 2020 2020 6966 2069  0):.        if i
-000026e0: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
-000026f0: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
-00002700: 2020 2020 6966 2078 202f 2069 203e 2032      if x / i > 2
-00002710: 3a0a 2020 2020 2020 2020 2020 2020 636f  :.            co
-00002720: 756e 7420 2b3d 2031 0a20 2020 2072 6574  unt += 1.    ret
-00002730: 7572 6e20 636f 756e 740a 0a69 6620 5f5f  urn count..if __
-00002740: 6e61 6d65 5f5f 203d 3d20 275f 5f6d 6169  name__ == '__mai
-00002750: 6e5f 5f27 3a0a 2020 2020 7072 696e 7428  n__':.    print(
-00002760: 7472 796d 6528 3130 3029 290a 6060 600a  tryme(100)).```.
-00002770: 0a3c 2f64 6574 6169 6c73 3e0a 0a         .</details>..
+00000470: 6420 6669 7865 732e 0a0a 2a2a 5761 7463  d fixes...**Watc
+00000480: 6820 4368 6174 4442 4720 696e 2061 6374  h ChatDBG in act
+00000490: 696f 6e21 2a2a 0a7c 204c 4c44 4220 6f6e  ion!**.| LLDB on
+000004a0: 205b 7465 7374 2d6f 7665 7266 6c6f 772e   [test-overflow.
+000004b0: 6370 705d 2873 616d 706c 6573 2f63 7070  cpp](samples/cpp
+000004c0: 2f74 6573 742d 6f76 6572 666c 6f77 2e63  /test-overflow.c
+000004d0: 7070 2920 7c20 4744 4220 6f6e 205b 7465  pp) | GDB on [te
+000004e0: 7374 2d6f 7665 7266 6c6f 772e 6370 705d  st-overflow.cpp]
+000004f0: 2873 616d 706c 6573 2f63 7070 2f74 6573  (samples/cpp/tes
+00000500: 742d 6f76 6572 666c 6f77 2e63 7070 2920  t-overflow.cpp) 
+00000510: 207c 2050 6462 206f 6e20 5b62 6f6f 7473   | Pdb on [boots
+00000520: 7472 6170 2e70 795d 2873 616d 706c 6573  trap.py](samples
+00000530: 2f70 7974 686f 6e2f 626f 6f74 7374 7261  /python/bootstra
+00000540: 702e 7079 2920 7c0a 7c3a 2d2d 2d2d 2d2d  p.py) |.|:------
+00000550: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000560: 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d  ---:|:----------
+00000570: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a  ---------------:
+00000580: 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |:--------------
+00000590: 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a 7c0a 7c20  -----------:|.| 
+000005a0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+000005b0: 2f61 7363 6969 6e65 6d61 2e6f 7267 2f61  /asciinema.org/a
+000005c0: 2f52 7341 4746 466d 7369 6349 764d 5738  /RsAGFFmsicIvMW8
+000005d0: 7867 7650 5036 5057 3266 2220 7461 7267  xgvPP6PW2f" targ
+000005e0: 6574 3d22 5f62 6c61 6e6b 223e 3c69 6d67  et="_blank"><img
+000005f0: 2073 7263 3d22 6d65 6469 612f 6c6c 6462   src="media/lldb
+00000600: 2e73 7667 2220 2f3e 3c2f 613e 7c20 3c61  .svg" /></a>| <a
+00000610: 2068 7265 663d 2268 7474 7073 3a2f 2f61   href="https://a
+00000620: 7363 6969 6e65 6d61 2e6f 7267 2f61 2f62  sciinema.org/a/b
+00000630: 4d57 4f79 7972 6837 5758 5773 5443 4662  MWOyyrh7WXWsTCFb
+00000640: 6f79 4b70 7177 5471 2220 7461 7267 6574  oyKpqwTq" target
+00000650: 3d22 5f62 6c61 6e6b 223e 3c69 6d67 2073  ="_blank"><img s
+00000660: 7263 3d22 6d65 6469 612f 6764 622e 7376  rc="media/gdb.sv
+00000670: 6722 202f 3e3c 2f61 3e7c 3c61 2068 7265  g" /></a>|<a hre
+00000680: 663d 2268 7474 7073 3a2f 2f61 7363 6969  f="https://ascii
+00000690: 6e65 6d61 2e6f 7267 2f61 2f71 756c 7869  nema.org/a/qulxi
+000006a0: 4a54 7177 5652 4a50 614d 5a31 6863 4273  JTqwVRJPaMZ1hcBs
+000006b0: 3643 6c75 2220 7461 7267 6574 3d22 5f62  6Clu" target="_b
+000006c0: 6c61 6e6b 223e 3c69 6d67 2073 7263 3d22  lank"><img src="
+000006d0: 6d65 6469 612f 7064 622e 7376 6722 202f  media/pdb.svg" /
+000006e0: 3e3c 2f61 3e7c 0a0a 466f 7220 7465 6368  ></a>|..For tech
+000006f0: 6e69 6361 6c20 6465 7461 696c 7320 616e  nical details an
+00000700: 6420 6120 636f 6d70 6c65 7465 2065 7661  d a complete eva
+00000710: 6c75 6174 696f 6e2c 2073 6565 206f 7572  luation, see our
+00000720: 2061 7258 6976 2070 6170 6572 2c20 5b5f   arXiv paper, [_
+00000730: 4368 6174 4442 473a 2041 6e20 4149 2d50  ChatDBG: An AI-P
+00000740: 6f77 6572 6564 2044 6562 7567 6769 6e67  owered Debugging
+00000750: 2041 7373 6973 7461 6e74 5f5d 2868 7474   Assistant_](htt
+00000760: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f61  ps://arxiv.org/a
+00000770: 6273 2f32 3430 332e 3136 3335 3429 2028  bs/2403.16354) (
+00000780: 5b50 4446 5d28 6874 7470 733a 2f2f 6769  [PDF](https://gi
+00000790: 7468 7562 2e63 6f6d 2f70 6c61 736d 612d  thub.com/plasma-
+000007a0: 756d 6173 732f 4368 6174 4442 472f 626c  umass/ChatDBG/bl
+000007b0: 6f62 2f6d 6169 6e2f 4368 6174 4442 472d  ob/main/ChatDBG-
+000007c0: 6172 7869 762d 3234 3033 2e31 3633 3534  arxiv-2403.16354
+000007d0: 2e70 6466 2929 2e0a 0a3e 205b 214e 4f54  .pdf))...> [!NOT
+000007e0: 455d 0a3e 0a3e 2043 6861 7444 4247 2066  E].>.> ChatDBG f
+000007f0: 6f72 2060 7064 6260 2c20 606c 6c64 6260  or `pdb`, `lldb`
+00000800: 2c20 616e 6420 6067 6462 6020 6172 6520  , and `gdb` are 
+00000810: 6665 6174 7572 652d 636f 6d70 6c65 7465  feature-complete
+00000820: 3b20 7765 2061 7265 2063 7572 7265 6e74  ; we are current
+00000830: 6c79 2062 6163 6b70 6f72 7469 6e67 2066  ly backporting f
+00000840: 6561 7475 7265 7320 666f 7220 7468 6573  eatures for thes
+00000850: 6520 6465 6275 6767 6572 7320 696e 746f  e debuggers into
+00000860: 2074 6865 206f 7468 6572 2064 6562 7567   the other debug
+00000870: 6765 7273 2e0a 3e0a 0a23 2320 496e 7374  gers..>..## Inst
+00000880: 616c 6c61 7469 6f6e 0a0a 3e20 5b21 494d  allation..> [!IM
+00000890: 504f 5254 414e 545d 0a3e 0a3e 2043 6861  PORTANT].>.> Cha
+000008a0: 7444 4247 2063 7572 7265 6e74 6c79 206e  tDBG currently n
+000008b0: 6565 6473 2074 6f20 6265 2063 6f6e 6e65  eeds to be conne
+000008c0: 6374 6564 2074 6f20 616e 205b 4f70 656e  cted to an [Open
+000008d0: 4149 2061 6363 6f75 6e74 5d28 6874 7470  AI account](http
+000008e0: 733a 2f2f 6f70 656e 6169 2e63 6f6d 2f61  s://openai.com/a
+000008f0: 7069 2f29 2e20 5f59 6f75 7220 6163 636f  pi/). _Your acco
+00000900: 756e 7420 7769 6c6c 206e 6565 6420 746f  unt will need to
+00000910: 2068 6176 6520 6120 706f 7369 7469 7665   have a positive
+00000920: 2062 616c 616e 6365 2066 6f72 2074 6869   balance for thi
+00000930: 7320 746f 2077 6f72 6b5f 2028 5b63 6865  s to work_ ([che
+00000940: 636b 2079 6f75 7220 6261 6c61 6e63 655d  ck your balance]
+00000950: 2868 7474 7073 3a2f 2f70 6c61 7466 6f72  (https://platfor
+00000960: 6d2e 6f70 656e 6169 2e63 6f6d 2f61 6363  m.openai.com/acc
+00000970: 6f75 6e74 2f75 7361 6765 2929 2e20 4966  ount/usage)). If
+00000980: 2079 6f75 2068 6176 6520 6e65 7665 7220   you have never 
+00000990: 7075 7263 6861 7365 6420 6372 6564 6974  purchased credit
+000009a0: 732c 2079 6f75 2077 696c 6c20 6e65 6564  s, you will need
+000009b0: 2074 6f20 7075 7263 6861 7365 2061 7420   to purchase at 
+000009c0: 6c65 6173 7420 5c24 3120 696e 2063 7265  least \$1 in cre
+000009d0: 6469 7473 2028 6966 2079 6f75 7220 4150  dits (if your AP
+000009e0: 4920 6163 636f 756e 7420 7761 7320 6372  I account was cr
+000009f0: 6561 7465 6420 6265 666f 7265 2041 7567  eated before Aug
+00000a00: 7573 7420 3133 2c20 3230 3233 2920 6f72  ust 13, 2023) or
+00000a10: 205c 2430 2e35 3020 2869 6620 796f 7520   \$0.50 (if you 
+00000a20: 6861 7665 2061 206e 6577 6572 2041 5049  have a newer API
+00000a30: 2061 6363 6f75 6e74 2920 696e 206f 7264   account) in ord
+00000a40: 6572 2074 6f20 6861 7665 2061 6363 6573  er to have acces
+00000a50: 7320 746f 2047 5054 2d34 2c20 7768 6963  s to GPT-4, whic
+00000a60: 6820 4368 6174 4442 4720 7573 6573 2e20  h ChatDBG uses. 
+00000a70: 5b47 6574 2061 206b 6579 2068 6572 652e  [Get a key here.
+00000a80: 5d28 6874 7470 733a 2f2f 706c 6174 666f  ](https://platfo
+00000a90: 726d 2e6f 7065 6e61 692e 636f 6d2f 6163  rm.openai.com/ac
+00000aa0: 636f 756e 742f 6170 692d 6b65 7973 290a  count/api-keys).
+00000ab0: 3e0a 3e20 4f6e 6365 2079 6f75 2068 6176  >.> Once you hav
+00000ac0: 6520 616e 2041 5049 206b 6579 2c20 7365  e an API key, se
+00000ad0: 7420 6974 2061 7320 616e 2065 6e76 6972  t it as an envir
+00000ae0: 6f6e 6d65 6e74 2076 6172 6961 626c 6520  onment variable 
+00000af0: 6361 6c6c 6564 2060 4f50 454e 4149 5f41  called `OPENAI_A
+00000b00: 5049 5f4b 4559 602e 0a3e 0a3e 2060 6060  PI_KEY`..>.> ```
+00000b10: 6261 7368 0a3e 2065 7870 6f72 7420 4f50  bash.> export OP
+00000b20: 454e 4149 5f41 5049 5f4b 4559 3d3c 796f  ENAI_API_KEY=<yo
+00000b30: 7572 2d61 7069 2d6b 6579 3e0a 3e20 6060  ur-api-key>.> ``
+00000b40: 600a 0a49 6e73 7461 6c6c 2043 6861 7444  `..Install ChatD
+00000b50: 4247 2075 7369 6e67 2060 7069 7060 2028  BG using `pip` (
+00000b60: 796f 7520 6e65 6564 2074 6f20 646f 2074  you need to do t
+00000b70: 6869 7320 7768 6574 6865 7220 796f 7520  his whether you 
+00000b80: 6172 6520 6465 6275 6767 696e 6720 5079  are debugging Py
+00000b90: 7468 6f6e 2c20 432c 206f 7220 432b 2b20  thon, C, or C++ 
+00000ba0: 636f 6465 293a 0a0a 6060 6062 6173 680a  code):..```bash.
+00000bb0: 7079 7468 6f6e 3320 2d6d 2070 6970 2069  python3 -m pip i
+00000bc0: 6e73 7461 6c6c 2063 6861 7464 6267 0a60  nstall chatdbg.`
+00000bd0: 6060 0a0a 4966 2079 6f75 2061 7265 2075  ``..If you are u
+00000be0: 7369 6e67 2043 6861 7444 4247 2074 6f20  sing ChatDBG to 
+00000bf0: 6465 6275 6720 5079 7468 6f6e 2070 726f  debug Python pro
+00000c00: 6772 616d 732c 2079 6f75 2061 7265 2064  grams, you are d
+00000c10: 6f6e 652e 2049 6620 796f 7520 7761 6e74  one. If you want
+00000c20: 2074 6f20 7573 6520 4368 6174 4442 4720   to use ChatDBG 
+00000c30: 746f 2064 6562 7567 206e 6174 6976 6520  to debug native 
+00000c40: 636f 6465 2077 6974 6820 6067 6462 6020  code with `gdb` 
+00000c50: 6f72 2060 6c6c 6462 602c 2066 6f6c 6c6f  or `lldb`, follo
+00000c60: 7720 7468 6520 696e 7374 616c 6c61 7469  w the installati
+00000c70: 6f6e 2069 6e73 7472 7563 7469 6f6e 7320  on instructions 
+00000c80: 6265 6c6f 772e 0a0a 2323 2320 496e 7374  below...### Inst
+00000c90: 616c 6c69 6e67 2061 7320 616e 2060 6c6c  alling as an `ll
+00000ca0: 6462 6020 6578 7465 6e73 696f 6e0a 0a3c  db` extension..<
+00000cb0: 6465 7461 696c 733e 0a3c 7375 6d6d 6172  details>.<summar
+00000cc0: 793e 0a3c 423e 3c54 543e 6c6c 6462 3c2f  y>.<B><TT>lldb</
+00000cd0: 5454 3e20 696e 7374 616c 6c61 7469 6f6e  TT> installation
+00000ce0: 2069 6e73 7472 7563 7469 6f6e 733c 2f42   instructions</B
+00000cf0: 3e0a 3c2f 7375 6d6d 6172 793e 0a0a 496e  >.</summary>..In
+00000d00: 7374 616c 6c20 4368 6174 4442 4720 696e  stall ChatDBG in
+00000d10: 746f 2074 6865 2060 6c6c 6462 6020 6465  to the `lldb` de
+00000d20: 6275 6767 6572 2062 7920 7275 6e6e 696e  bugger by runnin
+00000d30: 6720 7468 6520 666f 6c6c 6f77 696e 6720  g the following 
+00000d40: 636f 6d6d 616e 643a 0a0a 2323 2323 204c  command:..#### L
+00000d50: 696e 7578 0a0a 6060 6062 6173 680a 7079  inux..```bash.py
+00000d60: 7468 6f6e 3320 2d6d 2070 6970 2069 6e73  thon3 -m pip ins
+00000d70: 7461 6c6c 2043 6861 7444 4247 0a70 7974  tall ChatDBG.pyt
+00000d80: 686f 6e33 202d 6320 2769 6d70 6f72 7420  hon3 -c 'import 
+00000d90: 6368 6174 6462 673b 2070 7269 6e74 2866  chatdbg; print(f
+00000da0: 2263 6f6d 6d61 6e64 2073 6372 6970 7420  "command script 
+00000db0: 696d 706f 7274 207b 6368 6174 6462 672e  import {chatdbg.
+00000dc0: 5f5f 7061 7468 5f5f 5b30 5d7d 2f63 6861  __path__[0]}/cha
+00000dd0: 7464 6267 5f6c 6c64 622e 7079 2229 2720  tdbg_lldb.py")' 
+00000de0: 3e3e 207e 2f2e 6c6c 6462 696e 6974 0a60  >> ~/.lldbinit.`
+00000df0: 6060 0a0a 4966 2079 6f75 2065 6e63 6f75  ``..If you encou
+00000e00: 6e74 6572 2061 6e20 6572 726f 722c 2079  nter an error, y
+00000e10: 6f75 206d 6179 2062 6520 7573 696e 6720  ou may be using 
+00000e20: 616e 206f 6c64 6572 2076 6572 7369 6f6e  an older version
+00000e30: 206f 6620 4c4c 564d 2e20 5570 6461 7465   of LLVM. Update
+00000e40: 2074 6f20 7468 6520 6c61 7465 7374 2076   to the latest v
+00000e50: 6572 7369 6f6e 2061 7320 666f 6c6c 6f77  ersion as follow
+00000e60: 733a 0a0a 6060 600a 7375 646f 2061 7074  s:..```.sudo apt
+00000e70: 2069 6e73 7461 6c6c 202d 7920 6c73 622d   install -y lsb-
+00000e80: 7265 6c65 6173 6520 7767 6574 2073 6f66  release wget sof
+00000e90: 7477 6172 652d 7072 6f70 6572 7469 6573  tware-properties
+00000ea0: 2d63 6f6d 6d6f 6e20 676e 7570 670a 6375  -common gnupg.cu
+00000eb0: 726c 202d 7353 6620 6874 7470 733a 2f2f  rl -sSf https://
+00000ec0: 6170 742e 6c6c 766d 2e6f 7267 2f6c 6c76  apt.llvm.org/llv
+00000ed0: 6d2e 7368 207c 2073 7564 6f20 6261 7368  m.sh | sudo bash
+00000ee0: 202d 7320 2d2d 2031 3820 616c 6c0a 2320   -s -- 18 all.# 
+00000ef0: 4c4c 4442 206e 6f77 2061 7661 696c 6162  LLDB now availab
+00000f00: 6c65 2061 7320 606c 6c64 622d 3138 602e  le as `lldb-18`.
+00000f10: 0a60 6060 0a0a 2323 2323 204d 6163 0a0a  .```..#### Mac..
+00000f20: 6060 6062 6173 680a 7863 7275 6e20 7079  ```bash.xcrun py
+00000f30: 7468 6f6e 3320 2d6d 2070 6970 2069 6e73  thon3 -m pip ins
+00000f40: 7461 6c6c 2043 6861 7444 4247 0a78 6372  tall ChatDBG.xcr
+00000f50: 756e 2070 7974 686f 6e33 202d 6320 2769  un python3 -c 'i
+00000f60: 6d70 6f72 7420 6368 6174 6462 673b 2070  mport chatdbg; p
+00000f70: 7269 6e74 2866 2263 6f6d 6d61 6e64 2073  rint(f"command s
+00000f80: 6372 6970 7420 696d 706f 7274 207b 6368  cript import {ch
+00000f90: 6174 6462 672e 5f5f 7061 7468 5f5f 5b30  atdbg.__path__[0
+00000fa0: 5d7d 2f63 6861 7464 6267 5f6c 6c64 622e  ]}/chatdbg_lldb.
+00000fb0: 7079 2229 2720 3e3e 207e 2f2e 6c6c 6462  py")' >> ~/.lldb
+00000fc0: 696e 6974 0a60 6060 0a0a 5468 6973 2077  init.```..This w
+00000fd0: 696c 6c20 696e 7374 616c 6c20 4368 6174  ill install Chat
+00000fe0: 4442 4720 6173 2061 6e20 4c4c 564d 2065  DBG as an LLVM e
+00000ff0: 7874 656e 7369 6f6e 2e0a 3c2f 6465 7461  xtension..</deta
+00001000: 696c 733e 0a0a 2323 2320 496e 7374 616c  ils>..### Instal
+00001010: 6c69 6e67 2061 7320 6120 6067 6462 6020  ling as a `gdb` 
+00001020: 6578 7465 6e73 696f 6e0a 0a3c 6465 7461  extension..<deta
+00001030: 696c 733e 0a3c 7375 6d6d 6172 793e 0a3c  ils>.<summary>.<
+00001040: 423e 3c54 543e 6764 623c 2f54 543e 2069  B><TT>gdb</TT> i
+00001050: 6e73 7461 6c6c 6174 696f 6e20 696e 7374  nstallation inst
+00001060: 7275 6374 696f 6e73 3c2f 423e 0a3c 2f73  ructions</B>.</s
+00001070: 756d 6d61 7279 3e0a 0a49 6e73 7461 6c6c  ummary>..Install
+00001080: 2043 6861 7444 4247 2069 6e74 6f20 7468   ChatDBG into th
+00001090: 6520 6067 6462 6020 6465 6275 6767 6572  e `gdb` debugger
+000010a0: 2062 7920 7275 6e6e 696e 6720 7468 6520   by running the 
+000010b0: 666f 6c6c 6f77 696e 6720 636f 6d6d 616e  following comman
+000010c0: 643a 0a0a 6060 6062 6173 680a 7079 7468  d:..```bash.pyth
+000010d0: 6f6e 3320 2d6d 2070 6970 2069 6e73 7461  on3 -m pip insta
+000010e0: 6c6c 2043 6861 7444 4247 0a70 7974 686f  ll ChatDBG.pytho
+000010f0: 6e33 202d 6320 2769 6d70 6f72 7420 6368  n3 -c 'import ch
+00001100: 6174 6462 673b 2070 7269 6e74 2866 2273  atdbg; print(f"s
+00001110: 6f75 7263 6520 7b63 6861 7464 6267 2e5f  ource {chatdbg._
+00001120: 5f70 6174 685f 5f5b 305d 7d2f 6368 6174  _path__[0]}/chat
+00001130: 6462 675f 6764 622e 7079 2229 2720 3e3e  dbg_gdb.py")' >>
+00001140: 207e 2f2e 6764 6269 6e69 740a 6060 600a   ~/.gdbinit.```.
+00001150: 0a54 6869 7320 7769 6c6c 2069 6e73 7461  .This will insta
+00001160: 6c6c 2043 6861 7444 4247 2061 7320 6120  ll ChatDBG as a 
+00001170: 4744 4220 6578 7465 6e73 696f 6e2e 0a3c  GDB extension..<
+00001180: 2f64 6574 6169 6c73 3e0a 0a23 2323 2049  /details>..### I
+00001190: 6e73 7461 6c6c 696e 6720 6173 2061 2060  nstalling as a `
+000011a0: 5769 6e44 4247 6020 6578 7465 6e73 696f  WinDBG` extensio
+000011b0: 6e0a 0a3c 6465 7461 696c 733e 0a3c 7375  n..<details>.<su
+000011c0: 6d6d 6172 793e 0a3c 423e 3c54 543e 5769  mmary>.<B><TT>Wi
+000011d0: 6e44 4247 3c2f 5454 3e20 696e 7374 616c  nDBG</TT> instal
+000011e0: 6c61 7469 6f6e 2069 6e73 7472 7563 7469  lation instructi
+000011f0: 6f6e 733c 2f42 3e0a 3c2f 7375 6d6d 6172  ons</B>.</summar
+00001200: 793e 0a0a 312e 202a 2a49 6e73 7461 6c6c  y>..1. **Install
+00001210: 2057 696e 4442 472a 2a3a 2046 6f6c 6c6f   WinDBG**: Follo
+00001220: 7720 696e 7374 7275 6374 696f 6e73 205b  w instructions [
+00001230: 6865 7265 5d28 6874 7470 733a 2f2f 6c65  here](https://le
+00001240: 6172 6e2e 6d69 6372 6f73 6f66 742e 636f  arn.microsoft.co
+00001250: 6d2f 656e 2d75 732f 7769 6e64 6f77 732d  m/en-us/windows-
+00001260: 6861 7264 7761 7265 2f64 7269 7665 7273  hardware/drivers
+00001270: 2f64 6562 7567 6765 722f 2920 6966 2060  /debugger/) if `
+00001280: 5769 6e44 4247 6020 6973 206e 6f74 2069  WinDBG` is not i
+00001290: 6e73 7461 6c6c 6564 2061 6c72 6561 6479  nstalled already
+000012a0: 2e0a 312e 202a 2a49 6e73 7461 6c6c 2060  ..1. **Install `
+000012b0: 7663 706b 6760 2a2a 3a20 466f 6c6c 6f77  vcpkg`**: Follow
+000012c0: 2069 6e73 7472 7563 7469 6f6e 7320 5b68   instructions [h
+000012d0: 6572 655d 2868 7474 7073 3a2f 2f76 6370  ere](https://vcp
+000012e0: 6b67 2e69 6f2f 656e 2f67 6574 7469 6e67  kg.io/en/getting
+000012f0: 2d73 7461 7274 6564 2920 6966 2060 7663  -started) if `vc
+00001300: 706b 6760 2069 7320 6e6f 7420 696e 7374  pkg` is not inst
+00001310: 616c 6c65 6420 616c 7265 6164 792e 0a31  alled already..1
+00001320: 2e20 2a2a 496e 7374 616c 6c20 4465 6275  . **Install Debu
+00001330: 6767 696e 6720 546f 6f6c 7320 666f 7220  gging Tools for 
+00001340: 5769 6e64 6f77 732a 2a3a 2049 6e73 7461  Windows**: Insta
+00001350: 6c6c 2074 6865 2057 696e 646f 7773 2053  ll the Windows S
+00001360: 444b 205b 6865 7265 5d28 6874 7470 733a  DK [here](https:
+00001370: 2f2f 6465 7665 6c6f 7065 722e 6d69 6372  //developer.micr
+00001380: 6f73 6f66 742e 636f 6d2f 656e 2d75 732f  osoft.com/en-us/
+00001390: 7769 6e64 6f77 732f 646f 776e 6c6f 6164  windows/download
+000013a0: 732f 7769 6e64 6f77 732d 7364 6b2f 2920  s/windows-sdk/) 
+000013b0: 616e 6420 6368 6563 6b20 7468 6520 626f  and check the bo
+000013c0: 7820 6044 6562 7567 6769 6e67 2054 6f6f  x `Debugging Too
+000013d0: 6c73 2066 6f72 2057 696e 646f 7773 602e  ls for Windows`.
+000013e0: 0a31 2e20 2a2a 4e61 7669 6761 7465 2074  .1. **Navigate t
+000013f0: 6f20 7468 6520 6073 7263 5c63 6861 7464  o the `src\chatd
+00001400: 6267 6020 6469 7265 6374 6f72 792a 2a3a  bg` directory**:
+00001410: 2060 6364 2073 7263 5c63 6861 7464 6267   `cd src\chatdbg
+00001420: 600a 312e 202a 2a49 6e73 7461 6c6c 206e  `.1. **Install n
+00001430: 6565 6465 6420 6465 7065 6e64 656e 6369  eeded dependenci
+00001440: 6573 2a2a 3a20 5275 6e60 7663 706b 6720  es**: Run`vcpkg 
+00001450: 696e 7374 616c 6c60 0a31 2e20 2a2a 4275  install`.1. **Bu
+00001460: 696c 6420 7468 6520 6368 6174 6462 672e  ild the chatdbg.
+00001470: 646c 6c20 6578 7465 6e73 696f 6e2a 2a3a  dll extension**:
+00001480: 2052 756e 606d 6b64 6972 2062 7569 6c64   Run`mkdir build
+00001490: 2026 2063 6420 6275 696c 6420 2620 636d   & cd build & cm
+000014a0: 616b 6520 2e2e 2026 2063 6d61 6b65 202d  ake .. & cmake -
+000014b0: 2d62 7569 6c64 202e 2026 2063 6420 2e2e  -build . & cd ..
+000014c0: 600a 0a2a 2a55 7369 6e67 2043 6861 7444  `..**Using ChatD
+000014d0: 4247 2a2a 3a0a 0a20 2a20 4c6f 6164 2069  BG**:.. * Load i
+000014e0: 6e74 6f20 5769 6e44 4247 583a 0a20 2020  nto WinDBGX:.   
+000014f0: 2a20 5275 6e20 6077 696e 6462 6778 2079  * Run `windbgx y
+00001500: 6f75 725f 6578 6563 7574 6162 6c65 5f68  our_executable_h
+00001510: 6572 652e 6578 6560 0a20 2020 2a20 436c  ere.exe`.   * Cl
+00001520: 6963 6b20 7468 6520 6d65 6e75 2069 7465  ick the menu ite
+00001530: 6d73 2060 5669 6577 6020 2d3e 2060 436f  ms `View` -> `Co
+00001540: 6d6d 616e 6420 6272 6f77 7365 7260 0a20  mmand browser`. 
+00001550: 2020 2a20 5479 7065 2060 2e6c 6f61 6420    * Type `.load 
+00001560: 6465 6275 675c 6368 6174 6462 672e 646c  debug\chatdbg.dl
+00001570: 6c60 0a20 2a20 4166 7465 7220 7275 6e6e  l`. * After runn
+00001580: 696e 6720 636f 6465 2061 6e64 2068 6974  ing code and hit
+00001590: 7469 6e67 2061 6e20 6578 6365 7074 696f  ting an exceptio
+000015a0: 6e20 2f20 7369 676e 616c 3a0a 2020 202a  n / signal:.   *
+000015b0: 2054 7970 6520 6021 7768 7960 2069 6e20   Type `!why` in 
+000015c0: 436f 6d6d 616e 6420 6272 6f77 7365 720a  Command browser.
+000015d0: 3c2f 6465 7461 696c 733e 0a0a 0a23 2320  </details>...## 
+000015e0: 5573 6167 650a 0a23 2323 2044 6562 7567  Usage..### Debug
+000015f0: 6769 6e67 2050 7974 686f 6e0a 0a54 6f20  ging Python..To 
+00001600: 7573 6520 4368 6174 4442 4720 746f 2064  use ChatDBG to d
+00001610: 6562 7567 2050 7974 686f 6e20 7072 6f67  ebug Python prog
+00001620: 7261 6d73 2c20 7369 6d70 6c79 2072 756e  rams, simply run
+00001630: 2079 6f75 7220 5079 7468 6f6e 2073 6372   your Python scr
+00001640: 6970 7420 6173 2066 6f6c 6c6f 7773 3a0a  ipt as follows:.
+00001650: 0a60 6060 6261 7368 0a63 6861 7464 6267  .```bash.chatdbg
+00001660: 202d 6320 636f 6e74 696e 7565 2079 6f75   -c continue you
+00001670: 7273 6372 6970 742e 7079 0a60 6060 0a0a  rscript.py.```..
+00001680: 4368 6174 4442 4720 6973 2061 6e20 6578  ChatDBG is an ex
+00001690: 7465 6e73 696f 6e20 6f66 2074 6865 2073  tension of the s
+000016a0: 7461 6e64 6172 6420 5079 7468 6f6e 2064  tandard Python d
+000016b0: 6562 7567 6765 7220 6070 6462 602e 204c  ebugger `pdb`. L
+000016c0: 696b 650a 6070 6462 602c 2077 6865 6e20  ike.`pdb`, when 
+000016d0: 796f 7572 2073 6372 6970 7420 656e 636f  your script enco
+000016e0: 756e 7465 7273 2061 6e20 756e 6361 7567  unters an uncaug
+000016f0: 6874 2065 7863 6570 7469 6f6e 2c20 4368  ht exception, Ch
+00001700: 6174 4442 4720 7769 6c6c 0a65 6e74 6572  atDBG will.enter
+00001710: 2070 6f73 7420 6d6f 7274 656d 2064 6562   post mortem deb
+00001720: 7567 6769 6e67 206d 6f64 652e 0a0a 556e  ugging mode...Un
+00001730: 6c69 6b65 206f 7468 6572 2064 6562 7567  like other debug
+00001740: 6765 7273 2c20 796f 7520 6361 6e20 7468  gers, you can th
+00001750: 656e 2075 7365 2074 6865 2060 7768 7960  en use the `why`
+00001760: 2063 6f6d 6d61 6e64 2074 6f20 6173 6b0a   command to ask.
+00001770: 4368 6174 4442 4720 7768 7920 796f 7572  ChatDBG why your
+00001780: 2070 726f 6772 616d 2066 6169 6c65 6420   program failed 
+00001790: 616e 6420 6765 7420 6120 7375 6767 6573  and get a sugges
+000017a0: 7465 6420 6669 782e 2020 4166 7465 7220  ted fix.  After 
+000017b0: 7468 6520 4c4c 4d20 7265 7370 6f6e 6473  the LLM responds
+000017c0: 2c0a 796f 7520 6d61 7920 6973 7375 6520  ,.you may issue 
+000017d0: 6164 6469 7469 6f6e 616c 2064 6562 7567  additional debug
+000017e0: 6769 6e67 2063 6f6d 6d61 6e64 7320 6f72  ging commands or
+000017f0: 2063 6f6e 7469 6e75 6520 7468 6520 636f   continue the co
+00001800: 6e76 6572 7361 7469 6f6e 2062 7920 656e  nversation by en
+00001810: 7465 7269 6e67 0a61 6e79 206f 7468 6572  tering.any other
+00001820: 2074 6578 742e 0a0a 2323 2323 2049 5079   text...#### IPy
+00001830: 7468 6f6e 2061 6e64 204a 7570 7974 6572  thon and Jupyter
+00001840: 2053 7570 706f 7274 0a0a 546f 2075 7365   Support..To use
+00001850: 2043 6861 7444 4247 2061 7320 7468 6520   ChatDBG as the 
+00001860: 6465 6661 756c 7420 6465 6275 6767 6572  default debugger
+00001870: 2066 6f72 2049 5079 7468 6f6e 206f 7220   for IPython or 
+00001880: 696e 7369 6465 204a 7570 7974 6572 204e  inside Jupyter N
+00001890: 6f74 6562 6f6f 6b73 2c0a 6372 6561 7465  otebooks,.create
+000018a0: 2061 2049 5079 7468 6f6e 2070 726f 6669   a IPython profi
+000018b0: 6c65 2061 6e64 2074 6865 6e20 6164 6420  le and then add 
+000018c0: 7468 6520 6e65 6365 7373 6172 7920 6578  the necessary ex
+000018d0: 656e 7369 6f6e 7320 6f6e 2073 7461 7274  ensions on start
+000018e0: 7570 2e20 2028 4d6f 6469 6679 0a74 6865  up.  (Modify.the
+000018f0: 7365 206c 696e 6573 2061 7320 6e65 6365  se lines as nece
+00001900: 7373 6172 7920 6966 2079 6f75 2061 6c72  ssary if you alr
+00001910: 6561 6479 2068 6176 6520 6120 6375 7374  eady have a cust
+00001920: 6f6d 697a 6564 2070 726f 6669 6c65 2066  omized profile f
+00001930: 696c 652e 290a 0a60 6060 6261 7368 0a69  ile.)..```bash.i
+00001940: 7079 7468 6f6e 2070 726f 6669 6c65 2063  python profile c
+00001950: 7265 6174 650a 6563 686f 2022 632e 496e  reate.echo "c.In
+00001960: 7465 7261 6374 6976 6553 6865 6c6c 4170  teractiveShellAp
+00001970: 702e 6578 7465 6e73 696f 6e73 203d 205b  p.extensions = [
+00001980: 2763 6861 7464 6267 2e63 6861 7464 6267  'chatdbg.chatdbg
+00001990: 5f70 6462 272c 2027 6970 7966 6c6f 7727  _pdb', 'ipyflow'
+000019a0: 5d22 203e 3e20 7e2f 2e69 7079 7468 6f6e  ]" >> ~/.ipython
+000019b0: 2f70 726f 6669 6c65 5f64 6566 6175 6c74  /profile_default
+000019c0: 2f69 7079 7468 6f6e 5f63 6f6e 6669 672e  /ipython_config.
+000019d0: 7079 0a60 6060 0a0a 4f6e 2074 6865 2063  py.```..On the c
+000019e0: 6f6d 6d61 6e64 206c 696e 652c 2079 6f75  ommand line, you
+000019f0: 2063 616e 2074 6865 6e20 7275 6e3a 0a0a   can then run:..
+00001a00: 6060 6062 6173 680a 6970 7974 686f 6e20  ```bash.ipython 
+00001a10: 2d2d 7064 6220 796f 7572 7363 7269 7074  --pdb yourscript
+00001a20: 2e70 790a 6060 600a 0a49 6e73 6964 6520  .py.```..Inside 
+00001a30: 4a75 7079 7465 722c 2072 756e 2079 6f75  Jupyter, run you
+00001a40: 7220 6e6f 7465 626f 6f6b 2077 6974 6820  r notebook with 
+00001a50: 7468 6520 5b69 7079 666c 6f77 206b 6572  the [ipyflow ker
+00001a60: 6e65 6c5d 2868 7474 7073 3a2f 2f67 6974  nel](https://git
+00001a70: 6875 622e 636f 6d2f 6970 7966 6c6f 772f  hub.com/ipyflow/
+00001a80: 6970 7966 6c6f 7729 2061 6e64 2069 6e63  ipyflow) and inc
+00001a90: 6c75 6465 2074 6869 7320 6c69 6e65 206d  lude this line m
+00001aa0: 6167 6963 2061 7420 7468 6520 746f 7020  agic at the top 
+00001ab0: 6f66 2074 6865 2066 696c 652e 0a0a 6060  of the file...``
+00001ac0: 600a 2570 6462 0a60 6060 0a0a 0a23 2323  `.%pdb.```...###
+00001ad0: 2044 6562 7567 6769 6e67 206e 6174 6976   Debugging nativ
+00001ae0: 6520 636f 6465 2028 432c 2043 2b2b 2c20  e code (C, C++, 
+00001af0: 6f72 2052 7573 7420 7769 7468 203c 5454  or Rust with <TT
+00001b00: 3e6c 6c64 623c 2f54 543e 202f 203c 5454  >lldb</TT> / <TT
+00001b10: 3e67 6462 3c2f 5454 3e29 0a0a 546f 2075  >gdb</TT>)..To u
+00001b20: 7365 2043 6861 7444 4247 2077 6974 6820  se ChatDBG with 
+00001b30: 606c 6c64 6260 206f 7220 6067 6462 602c  `lldb` or `gdb`,
+00001b40: 206a 7573 7420 7275 6e20 6e61 7469 7665   just run native
+00001b50: 2063 6f64 6520 2863 6f6d 7069 6c65 6420   code (compiled 
+00001b60: 7769 7468 2060 2d67 6020 666f 7220 6465  with `-g` for de
+00001b70: 6275 6767 696e 6720 7379 6d62 6f6c 7329  bugging symbols)
+00001b80: 2077 6974 6820 796f 7572 2063 686f 6963   with your choic
+00001b90: 6520 6f66 2064 6562 7567 6765 723b 2077  e of debugger; w
+00001ba0: 6865 6e20 6974 2063 7261 7368 6573 2c20  hen it crashes, 
+00001bb0: 6173 6b20 6077 6879 602e 2054 6869 7320  ask `why`. This 
+00001bc0: 616c 736f 2077 6f72 6b73 2066 6f72 2070  also works for p
+00001bd0: 6f73 7420 6d6f 7274 656d 2064 6562 7567  ost mortem debug
+00001be0: 6769 6e67 2028 7768 656e 2079 6f75 206c  ging (when you l
+00001bf0: 6f61 6420 6120 636f 7265 2077 6974 6820  oad a core with 
+00001c00: 7468 6520 602d 6360 206f 7074 696f 6e29  the `-c` option)
+00001c10: 2e20 200a 0a54 6865 206e 6174 6976 6520  .  ..The native 
+00001c20: 6465 6275 6767 6572 7320 776f 726b 2073  debuggers work s
+00001c30: 6c69 6768 746c 7920 6469 6666 6572 656e  lightly differen
+00001c40: 746c 7920 7468 616e 2050 6462 2e20 2041  tly than Pdb.  A
+00001c50: 6674 6572 2074 6865 2064 6562 7567 6765  fter the debugge
+00001c60: 7220 7265 7370 6f6e 6473 2074 6f20 796f  r responds to yo
+00001c70: 7572 2071 7565 7374 696f 6e2c 2079 6f75  ur question, you
+00001c80: 2077 696c 6c20 656e 7465 7220 696e 746f   will enter into
+00001c90: 2043 6861 7444 4247 2773 2063 6f6d 6d61   ChatDBG's comma
+00001ca0: 6e64 206c 6f6f 702c 2061 7320 696e 6469  nd loop, as indi
+00001cb0: 6361 7465 6420 6279 2074 6865 2060 2843  cated by the `(C
+00001cc0: 6861 7444 4247 2063 6861 7474 696e 6729  hatDBG chatting)
+00001cd0: 6020 7072 6f6d 7074 2e20 2059 6f75 206d  ` prompt.  You m
+00001ce0: 6179 2063 6f6e 7469 6e75 6520 6973 7375  ay continue issu
+00001cf0: 696e 6720 6465 6275 6767 696e 6720 636f  ing debugging co
+00001d00: 6d6d 616e 6473 2061 6e64 2079 6f75 206d  mmands and you m
+00001d10: 6179 2073 656e 6420 6164 6469 7469 6f6e  ay send addition
+00001d20: 616c 206d 6573 7361 6765 7320 746f 2074  al messages to t
+00001d30: 6865 204c 4c4d 2062 7920 7374 6172 7469  he LLM by starti
+00001d40: 6e67 2074 686f 7365 206d 6573 7361 6765  ng those message
+00001d50: 7320 7769 7468 2022 6368 6174 222e 2020  s with "chat".  
+00001d60: 5768 656e 2079 6f75 2061 7265 2064 6f6e  When you are don
+00001d70: 652c 2074 7970 6520 6071 7569 7460 2074  e, type `quit` t
+00001d80: 6f20 7265 7475 726e 2074 6f20 7468 6520  o return to the 
+00001d90: 6465 6275 6767 6572 2773 206d 6169 6e20  debugger's main 
+00001da0: 636f 6d6d 616e 6420 6c6f 6f70 2e0a 0a3c  command loop...<
+00001db0: 6465 7461 696c 733e 0a3c 7375 6d6d 6172  details>.<summar
+00001dc0: 793e 0a3c 423e 4465 6275 6767 696e 6720  y>.<B>Debugging 
+00001dd0: 5275 7374 2070 726f 6772 616d 733c 2f42  Rust programs</B
+00001de0: 3e0a 3c2f 7375 6d6d 6172 793e 0a0a 546f  >.</summary>..To
+00001df0: 2075 7365 2043 6861 7444 4247 2077 6974   use ChatDBG wit
+00001e00: 6820 5275 7374 2c20 796f 7520 6e65 6564  h Rust, you need
+00001e10: 2074 6f20 646f 2074 776f 2073 7465 7073   to do two steps
+00001e20: 3a20 6d6f 6469 6679 2079 6f75 720a 6043  : modify your.`C
+00001e30: 6172 676f 2e74 6f6d 6c60 2066 696c 6520  argo.toml` file 
+00001e40: 616e 6420 6164 6420 6f6e 6520 6c69 6e65  and add one line
+00001e50: 2074 6f20 796f 7572 2073 6f75 7263 6520   to your source 
+00001e60: 7072 6f67 7261 6d2e 0a0a 312e 2041 6464  program...1. Add
+00001e70: 2074 6869 7320 746f 2079 6f75 7220 6043   this to your `C
+00001e80: 6172 676f 2e74 6f6d 6c60 2066 696c 653a  argo.toml` file:
+00001e90: 0a0a 6060 6074 6f6d 6c0a 5b64 6570 656e  ..```toml.[depen
+00001ea0: 6465 6e63 6965 735d 0a63 6861 7464 6267  dencies].chatdbg
+00001eb0: 203d 2022 302e 312e 3322 0a0a 5b70 726f   = "0.1.3"..[pro
+00001ec0: 6669 6c65 2e64 6576 5d0a 7061 6e69 6320  file.dev].panic 
+00001ed0: 3d20 2261 626f 7274 220a 0a5b 7072 6f66  = "abort"..[prof
+00001ee0: 696c 652e 7265 6c65 6173 655d 0a70 616e  ile.release].pan
+00001ef0: 6963 203d 2022 6162 6f72 7422 0a60 6060  ic = "abort".```
+00001f00: 0a0a 322e 2049 6e20 796f 7572 2070 726f  ..2. In your pro
+00001f10: 6772 616d 2c20 6170 706c 7920 7468 6520  gram, apply the 
+00001f20: 6023 5b63 6861 7464 6267 3a3a 6d61 696e  `#[chatdbg::main
+00001f30: 5d60 2061 7474 7269 6275 7465 2074 6f20  ]` attribute to 
+00001f40: 796f 7572 2060 6d61 696e 600a 6675 6e63  your `main`.func
+00001f50: 7469 6f6e 3a0a 0a60 6060 7275 7374 0a23  tion:..```rust.#
+00001f60: 5b63 6861 7464 6267 3a3a 6d61 696e 5d0a  [chatdbg::main].
+00001f70: 666e 206d 6169 6e28 2920 7b0a 6060 600a  fn main() {.```.
+00001f80: 0a4e 6f77 2079 6f75 2063 616e 2064 6562  .Now you can deb
+00001f90: 7567 2079 6f75 7220 5275 7374 2063 6f64  ug your Rust cod
+00001fa0: 6520 7769 7468 2060 6764 6260 206f 7220  e with `gdb` or 
+00001fb0: 606c 6c64 6260 2e0a 0a3c 2f64 6574 6169  `lldb`...</detai
+00001fc0: 6c73 3e0a 0a23 2323 2045 7861 6d70 6c65  ls>..### Example
+00001fd0: 730a 0a3c 6465 7461 696c 733e 0a3c 7375  s..<details>.<su
+00001fe0: 6d6d 6172 793e 0a3c 423e 4368 6174 4442  mmary>.<B>ChatDB
+00001ff0: 4720 6578 616d 706c 6520 696e 203c 5454  G example in <TT
+00002000: 3e6c 6c64 623c 2f54 543e 3c2f 423e 0a3c  >lldb</TT></B>.<
+00002010: 2f73 756d 6d61 7279 3e0a 0a60 6060 6764  /summary>..```gd
+00002020: 620a 2843 6861 7444 4247 206c 6c64 6229  b.(ChatDBG lldb)
+00002030: 2072 756e 0a50 726f 6365 7373 2038 3534   run.Process 854
+00002040: 3934 206c 6175 6e63 6865 643a 2027 2f55  94 launched: '/U
+00002050: 7365 7273 2f65 6d65 7279 2f67 6974 2f43  sers/emery/git/C
+00002060: 6861 7444 4247 2f74 6573 742f 612e 6f75  hatDBG/test/a.ou
+00002070: 7427 2028 6172 6d36 3429 0a54 4553 5420  t' (arm64).TEST 
+00002080: 310a 5445 5354 202d 3432 3237 3631 3238  1.TEST -42276128
+00002090: 380a 5445 5354 2030 0a54 4553 5420 300a  8.TEST 0.TEST 0.
+000020a0: 5445 5354 2030 0a54 4553 5420 300a 5445  TEST 0.TEST 0.TE
+000020b0: 5354 2030 0a54 4553 5420 300a 5072 6f63  ST 0.TEST 0.Proc
+000020c0: 6573 7320 3835 3439 3420 7374 6f70 7065  ess 85494 stoppe
+000020d0: 640a 2a20 7468 7265 6164 2023 312c 2071  d.* thread #1, q
+000020e0: 7565 7565 203d 2027 636f 6d2e 6170 706c  ueue = 'com.appl
+000020f0: 652e 6d61 696e 2d74 6872 6561 6427 2c20  e.main-thread', 
+00002100: 7374 6f70 2072 6561 736f 6e20 3d20 4558  stop reason = EX
+00002110: 435f 4241 445f 4143 4345 5353 2028 636f  C_BAD_ACCESS (co
+00002120: 6465 3d31 2c20 6164 6472 6573 733d 3078  de=1, address=0x
+00002130: 3130 3030 3536 3230 3029 0a20 2020 2066  100056200).    f
+00002140: 7261 6d65 2023 303a 2030 7830 3030 3030  rame #0: 0x00000
+00002150: 3030 3130 3030 3032 6636 3420 612e 6f75  00100002f64 a.ou
+00002160: 7460 666f 6f28 6e3d 382c 2062 3d31 2920  t`foo(n=8, b=1) 
+00002170: 6174 2074 6573 742e 6370 703a 373a 3232  at test.cpp:7:22
+00002180: 0a20 2020 3420 2020 2020 696e 7420 785b  .   4     int x[
+00002190: 5d20 3d20 7b20 312c 2032 2c20 332c 2034  ] = { 1, 2, 3, 4
+000021a0: 2c20 3520 7d3b 0a20 2020 3520 2020 2020  , 5 };.   5     
+000021b0: 0a20 2020 3620 2020 2020 766f 6964 2066  .   6     void f
+000021c0: 6f6f 2869 6e74 206e 2c20 666c 6f61 7420  oo(int n, float 
+000021d0: 6229 207b 0a2d 3e20 3720 2020 2020 2020  b) {.-> 7       
+000021e0: 636f 7574 203c 3c20 2254 4553 5420 2220  cout << "TEST " 
+000021f0: 3c3c 2078 5b6e 202a 2031 3030 3030 5d20  << x[n * 10000] 
+00002200: 3c3c 2065 6e64 6c3b 0a20 2020 3820 2020  << endl;.   8   
+00002210: 2020 7d0a 2020 2039 2020 2020 200a 2020    }.   9     .  
+00002220: 2031 3020 2020 2069 6e74 206d 6169 6e28   10    int main(
+00002230: 290a 5461 7267 6574 2030 3a20 2861 2e6f  ).Target 0: (a.o
+00002240: 7574 2920 7374 6f70 7065 642e 0a60 6060  ut) stopped..```
+00002250: 0a0a 4173 6b20 6077 6879 6020 746f 2068  ..Ask `why` to h
+00002260: 6176 6520 4368 6174 4442 4720 7072 6f76  ave ChatDBG prov
+00002270: 6964 6520 6120 6865 6c70 6675 6c20 6578  ide a helpful ex
+00002280: 706c 616e 6174 696f 6e20 7768 7920 7468  planation why th
+00002290: 6973 2070 726f 6772 616d 2066 6169 6c65  is program faile
+000022a0: 642c 2061 6e64 2073 7567 6765 7374 2061  d, and suggest a
+000022b0: 2066 6978 3a0a 0a0a 6060 6067 6462 0a28   fix:...```gdb.(
+000022c0: 4368 6174 4442 4720 6c6c 6462 2920 7768  ChatDBG lldb) wh
+000022d0: 790a 5468 6520 726f 6f74 2063 6175 7365  y.The root cause
+000022e0: 206f 6620 7468 6973 2065 7272 6f72 2069   of this error i
+000022f0: 7320 6163 6365 7373 696e 6720 616e 2069  s accessing an i
+00002300: 6e64 6578 206f 6620 7468 6520 6172 7261  ndex of the arra
+00002310: 7920 6078 600a 7468 6174 2069 7320 6f75  y `x`.that is ou
+00002320: 7420 6f66 2062 6f75 6e64 732e 2049 6e20  t of bounds. In 
+00002330: 6066 6f6f 2829 602c 2074 6865 2069 6e64  `foo()`, the ind
+00002340: 6578 2069 7320 6361 6c63 756c 6174 6564  ex is calculated
+00002350: 2061 7320 606e 202a 0a31 3030 3030 602c   as `n *.10000`,
+00002360: 2077 6869 6368 2063 616e 2062 6520 6d75   which can be mu
+00002370: 6368 206c 6172 6765 7220 7468 616e 2074  ch larger than t
+00002380: 6865 2073 697a 6520 6f66 2074 6865 2061  he size of the a
+00002390: 7272 6179 2060 7860 2028 7768 6963 680a  rray `x` (which.
+000023a0: 6973 206f 6e6c 7920 3520 656c 656d 656e  is only 5 elemen
+000023b0: 7473 292e 2049 6e20 7468 6520 6769 7665  ts). In the give
+000023c0: 6e20 7472 6163 652c 2074 6865 2070 726f  n trace, the pro
+000023d0: 6772 616d 2069 7320 7472 7969 6e67 2074  gram is trying t
+000023e0: 6f0a 6163 6365 7373 2074 6865 206d 656d  o.access the mem
+000023f0: 6f72 7920 6164 6472 6573 7320 6030 7831  ory address `0x1
+00002400: 3030 3035 3632 3030 602c 2077 6869 6368  00056200`, which
+00002410: 2069 7320 6f75 7473 6964 6520 6f66 2074   is outside of t
+00002420: 6865 2072 616e 6765 0a6f 6620 616c 6c6f  he range.of allo
+00002430: 6361 7465 6420 6d65 6d6f 7279 2066 6f72  cated memory for
+00002440: 2074 6865 2061 7272 6179 2060 7860 2e0a   the array `x`..
+00002450: 0a54 6f20 6669 7820 7468 6973 2065 7272  .To fix this err
+00002460: 6f72 2c20 7765 206e 6565 6420 746f 2065  or, we need to e
+00002470: 6e73 7572 6520 7468 6174 2074 6865 2069  nsure that the i
+00002480: 6e64 6578 2069 7320 7769 7468 696e 2074  ndex is within t
+00002490: 6865 0a62 6f75 6e64 7320 6f66 2074 6865  he.bounds of the
+000024a0: 2061 7272 6179 2e20 4f6e 6520 7761 7920   array. One way 
+000024b0: 746f 2064 6f20 7468 6973 2069 7320 746f  to do this is to
+000024c0: 2063 6865 636b 2074 6865 2076 616c 7565   check the value
+000024d0: 206f 6620 606e 600a 6265 666f 7265 2063   of `n`.before c
+000024e0: 616c 6375 6c61 7469 6e67 2074 6865 2069  alculating the i
+000024f0: 6e64 6578 2c20 616e 6420 656e 7375 7265  ndex, and ensure
+00002500: 2074 6861 7420 6974 2069 7320 6c65 7373   that it is less
+00002510: 2074 6861 6e20 7468 6520 7369 7a65 0a6f   than the size.o
+00002520: 6620 7468 6520 6172 7261 7920 6469 7669  f the array divi
+00002530: 6465 6420 6279 2074 6865 2073 697a 6520  ded by the size 
+00002540: 6f66 2074 6865 2065 6c65 6d65 6e74 2e20  of the element. 
+00002550: 466f 7220 6578 616d 706c 652c 2077 6520  For example, we 
+00002560: 6361 6e0a 6d6f 6469 6679 2060 666f 6f28  can.modify `foo(
+00002570: 2960 2061 7320 666f 6c6c 6f77 733a 0a0a  )` as follows:..
+00002580: 2020 2020 6060 600a 2020 2020 766f 6964      ```.    void
+00002590: 2066 6f6f 2869 6e74 206e 2c20 666c 6f61   foo(int n, floa
+000025a0: 7420 6229 207b 0a20 2020 2020 2069 6620  t b) {.      if 
+000025b0: 286e 203c 2030 207c 7c20 6e20 3e3d 2073  (n < 0 || n >= s
+000025c0: 697a 656f 6628 7829 2f73 697a 656f 6628  izeof(x)/sizeof(
+000025d0: 785b 305d 2929 207b 0a20 2020 2020 2020  x[0])) {.       
+000025e0: 2063 6f75 7420 3c3c 2022 4552 524f 523a   cout << "ERROR:
+000025f0: 2049 6e76 616c 6964 2069 6e64 6578 2220   Invalid index" 
+00002600: 3c3c 2065 6e64 6c3b 0a20 2020 2020 2020  << endl;.       
+00002610: 2072 6574 7572 6e3b 0a20 2020 2020 207d   return;.      }
+00002620: 0a20 2020 2020 2063 6f75 7420 3c3c 2022  .      cout << "
+00002630: 5445 5354 2022 203c 3c20 785b 6e5d 203c  TEST " << x[n] <
+00002640: 3c20 656e 646c 3b0a 2020 2020 7d0a 2020  < endl;.    }.  
+00002650: 2020 6060 600a 0a54 6869 7320 636f 6465    ```..This code
+00002660: 2063 6865 636b 7320 6966 2060 6e60 2069   checks if `n` i
+00002670: 7320 7769 7468 696e 2074 6865 2076 616c  s within the val
+00002680: 6964 2072 616e 6765 2c20 616e 6420 7072  id range, and pr
+00002690: 696e 7473 2061 6e20 6572 726f 720a 6d65  ints an error.me
+000026a0: 7373 6167 6520 6966 2069 7420 6973 206e  ssage if it is n
+000026b0: 6f74 2e20 4966 2060 6e60 2069 7320 7769  ot. If `n` is wi
+000026c0: 7468 696e 2074 6865 2072 616e 6765 2c20  thin the range, 
+000026d0: 7468 6520 6675 6e63 7469 6f6e 2070 7269  the function pri
+000026e0: 6e74 730a 7468 6520 7661 6c75 6520 6f66  nts.the value of
+000026f0: 2074 6865 2065 6c65 6d65 6e74 2061 7420   the element at 
+00002700: 696e 6465 7820 606e 6020 6f66 2060 7860  index `n` of `x`
+00002710: 2e20 5769 7468 2074 6869 7320 6d6f 6469  . With this modi
+00002720: 6669 6361 7469 6f6e 2c0a 7468 6520 7072  fication,.the pr
+00002730: 6f67 7261 6d20 7769 6c6c 2061 766f 6964  ogram will avoid
+00002740: 2061 6363 6573 7369 6e67 206d 656d 6f72   accessing memor
+00002750: 7920 6f75 7473 6964 6520 7468 6520 626f  y outside the bo
+00002760: 756e 6473 206f 6620 7468 650a 6172 7261  unds of the.arra
+00002770: 792c 2061 6e64 2077 696c 6c20 7072 696e  y, and will prin
+00002780: 7420 7468 6520 6578 7065 6374 6564 206f  t the expected o
+00002790: 7574 7075 7420 666f 7220 7661 6c69 6420  utput for valid 
+000027a0: 696e 6469 6365 732e 0a60 6060 0a3c 2f64  indices..```.</d
+000027b0: 6574 6169 6c73 3e0a 0a3c 6465 7461 696c  etails>..<detail
+000027c0: 733e 0a3c 7375 6d6d 6172 793e 0a3c 423e  s>.<summary>.<B>
+000027d0: 4368 6174 4442 4720 6578 616d 706c 6520  ChatDBG example 
+000027e0: 696e 2050 7974 686f 6e20 283c 5454 3e70  in Python (<TT>p
+000027f0: 6462 3c2f 5454 3e29 3c2f 423e 0a3c 2f73  db</TT>)</B>.</s
+00002800: 756d 6d61 7279 3e0a 0a60 6060 7079 7468  ummary>..```pyth
+00002810: 6f6e 0a54 7261 6365 6261 636b 2028 6d6f  on.Traceback (mo
+00002820: 7374 2072 6563 656e 7420 6361 6c6c 206c  st recent call l
+00002830: 6173 7429 3a0a 2020 4669 6c65 2022 796f  ast):.  File "yo
+00002840: 7572 7363 7269 7074 2e70 7922 2c20 6c69  urscript.py", li
+00002850: 6e65 2039 2c20 696e 203c 6d6f 6475 6c65  ne 9, in <module
+00002860: 3e0a 2020 2020 7072 696e 7428 7472 796d  >.    print(trym
+00002870: 6528 3130 3029 290a 2020 4669 6c65 2022  e(100)).  File "
+00002880: 796f 7572 7363 7269 7074 2e70 7922 2c20  yourscript.py", 
+00002890: 6c69 6e65 2034 2c20 696e 2074 7279 6d65  line 4, in tryme
+000028a0: 0a20 2020 2069 6620 7820 2f20 6920 3e20  .    if x / i > 
+000028b0: 323a 0a5a 6572 6f44 6976 6973 696f 6e45  2:.ZeroDivisionE
+000028c0: 7272 6f72 3a20 6469 7669 7369 6f6e 2062  rror: division b
+000028d0: 7920 7a65 726f 0a55 6e63 6175 6768 7420  y zero.Uncaught 
+000028e0: 6578 6365 7074 696f 6e2e 2045 6e74 6572  exception. Enter
+000028f0: 696e 6720 706f 7374 206d 6f72 7465 6d20  ing post mortem 
+00002900: 6465 6275 6767 696e 670a 5275 6e6e 696e  debugging.Runnin
+00002910: 6720 2763 6f6e 7427 206f 7220 2773 7465  g 'cont' or 'ste
+00002920: 7027 2077 696c 6c20 7265 7374 6172 7420  p' will restart 
+00002930: 7468 6520 7072 6f67 7261 6d0a 3e20 796f  the program.> yo
+00002940: 7572 7363 7269 7074 2e70 7928 3429 7472  urscript.py(4)tr
+00002950: 796d 6528 290a 2d3e 2069 6620 7820 2f20  yme().-> if x / 
+00002960: 6920 3e20 323a 0a60 6060 0a0a 4173 6b20  i > 2:.```..Ask 
+00002970: 6077 6879 6020 746f 2068 6176 6520 4368  `why` to have Ch
+00002980: 6174 4442 4720 7072 6f76 6964 6520 6120  atDBG provide a 
+00002990: 6865 6c70 6675 6c20 6578 706c 616e 6174  helpful explanat
+000029a0: 696f 6e20 7768 7920 7468 6973 2070 726f  ion why this pro
+000029b0: 6772 616d 2066 6169 6c65 642c 2061 6e64  gram failed, and
+000029c0: 2073 7567 6765 7374 2061 2066 6978 3a0a   suggest a fix:.
+000029d0: 0a60 6060 7079 7468 6f6e 0a28 4368 6174  .```python.(Chat
+000029e0: 4442 4720 5064 6229 2077 6879 0a54 6865  DBG Pdb) why.The
+000029f0: 2072 6f6f 7420 6361 7573 6520 6f66 2074   root cause of t
+00002a00: 6865 2065 7272 6f72 2069 7320 7468 6174  he error is that
+00002a10: 2074 6865 2063 6f64 6520 6973 2061 7474   the code is att
+00002a20: 656d 7074 696e 6720 746f 0a64 6976 6964  empting to.divid
+00002a30: 6520 6279 207a 6572 6f20 696e 2074 6865  e by zero in the
+00002a40: 206c 696e 6520 2269 6620 7820 2f20 6920   line "if x / i 
+00002a50: 3e20 3222 2e20 4173 2069 2072 616e 6765  > 2". As i range
+00002a60: 7320 6672 6f6d 2030 2074 6f20 3939 2c0a  s from 0 to 99,.
+00002a70: 6974 2077 696c 6c20 6576 656e 7475 616c  it will eventual
+00002a80: 6c79 2072 6561 6368 2074 6865 2076 616c  ly reach the val
+00002a90: 7565 206f 6620 302c 2063 6175 7369 6e67  ue of 0, causing
+00002aa0: 2061 205a 6572 6f44 6976 6973 696f 6e45   a ZeroDivisionE
+00002ab0: 7272 6f72 2e0a 0a41 2070 6f73 7369 626c  rror...A possibl
+00002ac0: 6520 6669 7820 666f 7220 7468 6973 2077  e fix for this w
+00002ad0: 6f75 6c64 2062 6520 746f 2061 6464 2061  ould be to add a
+00002ae0: 2063 6865 636b 2066 6f72 2069 2062 6569   check for i bei
+00002af0: 6e67 2065 7175 616c 2074 6f0a 7a65 726f  ng equal to.zero
+00002b00: 2062 6566 6f72 6520 7065 7266 6f72 6d69   before performi
+00002b10: 6e67 2074 6865 2064 6976 6973 696f 6e2e  ng the division.
+00002b20: 2054 6869 7320 636f 756c 6420 6265 2064   This could be d
+00002b30: 6f6e 6520 6279 2061 6464 696e 6720 616e  one by adding an
+00002b40: 0a61 6464 6974 696f 6e61 6c20 636f 6e64  .additional cond
+00002b50: 6974 696f 6e61 6c20 7374 6174 656d 656e  itional statemen
+00002b60: 742c 2073 7563 6820 6173 2022 6966 2069  t, such as "if i
+00002b70: 203d 3d20 303a 2063 6f6e 7469 6e75 6522   == 0: continue"
+00002b80: 2c20 746f 0a73 6b69 7020 6f76 6572 2074  , to.skip over t
+00002b90: 6865 2069 7465 7261 7469 6f6e 2077 6865  he iteration whe
+00002ba0: 6e20 6920 6973 207a 6572 6f2e 2054 6865  n i is zero. The
+00002bb0: 2075 7064 6174 6564 2063 6f64 6520 776f   updated code wo
+00002bc0: 756c 6420 6c6f 6f6b 0a6c 696b 6520 7468  uld look.like th
+00002bd0: 6973 3a0a 0a64 6566 2074 7279 6d65 2878  is:..def tryme(x
+00002be0: 293a 0a20 2020 2063 6f75 6e74 203d 2030  ):.    count = 0
+00002bf0: 0a20 2020 2066 6f72 2069 2069 6e20 7261  .    for i in ra
+00002c00: 6e67 6528 3130 3029 3a0a 2020 2020 2020  nge(100):.      
+00002c10: 2020 6966 2069 203d 3d20 303a 0a20 2020    if i == 0:.   
+00002c20: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+00002c30: 650a 2020 2020 2020 2020 6966 2078 202f  e.        if x /
+00002c40: 2069 203e 2032 3a0a 2020 2020 2020 2020   i > 2:.        
+00002c50: 2020 2020 636f 756e 7420 2b3d 2031 0a20      count += 1. 
+00002c60: 2020 2072 6574 7572 6e20 636f 756e 740a     return count.
+00002c70: 0a69 6620 5f5f 6e61 6d65 5f5f 203d 3d20  .if __name__ == 
+00002c80: 275f 5f6d 6169 6e5f 5f27 3a0a 2020 2020  '__main__':.    
+00002c90: 7072 696e 7428 7472 796d 6528 3130 3029  print(tryme(100)
+00002ca0: 290a 6060 600a 0a3c 2f64 6574 6169 6c73  ).```..</details
+00002cb0: 3e0a 0a                                  >..
```

### Comparing `chatdbg-0.5/pyproject.toml` & `chatdbg-0.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ChatDBG"
-version = "0.5"
+version = "0.6"
 authors = [
   { name="Emery Berger", email="emery.berger@gmail.com" },
   { name="Stephen Freund", email="sfreund@williams.edu" },
   { name="Kyla Levin", email="khlevin@umass.edu" },
   { name="Nicolas van Kempen", email="nvankemp@gmail.com" },
 ]
 dependencies = [
@@ -18,19 +18,19 @@
   "ansicolors>=1.1.8",
   "traitlets>=5.14.1",
   "ipdb>=0.13.13",
   "ipython>=8.18.1",
   "litellm>=1.34.12",
   "PyYAML>=6.0.1", 
   "ipyflow>=0.0.130",
-  "numpy>=1.26.3"
+  "numpy>=1.26.3",
 ]
 description = "AI-assisted debugging. Uses AI to answer 'why'."
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.10"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: Apache Software License",
   "Operating System :: OS Independent",
 ]
 
 [project.scripts]
```

### Comparing `chatdbg-0.5/PKG-INFO` & `chatdbg-0.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 330a 4e61 6d65 3a20 4368 6174  : 2.3.Name: Chat
-00000020: 4442 470a 5665 7273 696f 6e3a 2030 2e35  DBG.Version: 0.5
+00000020: 4442 470a 5665 7273 696f 6e3a 2030 2e36  DBG.Version: 0.6
 00000030: 0a53 756d 6d61 7279 3a20 4149 2d61 7373  .Summary: AI-ass
 00000040: 6973 7465 6420 6465 6275 6767 696e 672e  isted debugging.
 00000050: 2055 7365 7320 4149 2074 6f20 616e 7377   Uses AI to answ
 00000060: 6572 2027 7768 7927 2e0a 5072 6f6a 6563  er 'why'..Projec
 00000070: 742d 5552 4c3a 2048 6f6d 6570 6167 652c  t-URL: Homepage,
 00000080: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000090: 636f 6d2f 706c 6173 6d61 2d75 6d61 7373  com/plasma-umass
@@ -31,664 +31,747 @@
 000001e0: 7265 204c 6963 656e 7365 0a43 6c61 7373  re License.Class
 000001f0: 6966 6965 723a 204f 7065 7261 7469 6e67  ifier: Operating
 00000200: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
 00000210: 6465 7065 6e64 656e 740a 436c 6173 7369  dependent.Classi
 00000220: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
 00000230: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
 00000240: 7468 6f6e 203a 3a20 330a 5265 7175 6972  thon :: 3.Requir
-00000250: 6573 2d50 7974 686f 6e3a 203e 3d33 2e37  es-Python: >=3.7
-00000260: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000270: 616e 7369 636f 6c6f 7273 3e3d 312e 312e  ansicolors>=1.1.
-00000280: 380a 5265 7175 6972 6573 2d44 6973 743a  8.Requires-Dist:
-00000290: 2069 7064 623e 3d30 2e31 332e 3133 0a52   ipdb>=0.13.13.R
-000002a0: 6571 7569 7265 732d 4469 7374 3a20 6970  equires-Dist: ip
-000002b0: 7966 6c6f 773e 3d30 2e30 2e31 3330 0a52  yflow>=0.0.130.R
-000002c0: 6571 7569 7265 732d 4469 7374 3a20 6970  equires-Dist: ip
-000002d0: 7974 686f 6e3e 3d38 2e31 382e 310a 5265  ython>=8.18.1.Re
-000002e0: 7175 6972 6573 2d44 6973 743a 206c 6974  quires-Dist: lit
-000002f0: 656c 6c6d 3e3d 312e 3334 2e31 320a 5265  ellm>=1.34.12.Re
-00000300: 7175 6972 6573 2d44 6973 743a 206c 6c6d  quires-Dist: llm
-00000310: 2d75 7469 6c73 3e3d 302e 322e 380a 5265  -utils>=0.2.8.Re
-00000320: 7175 6972 6573 2d44 6973 743a 206e 756d  quires-Dist: num
-00000330: 7079 3e3d 312e 3236 2e33 0a52 6571 7569  py>=1.26.3.Requi
-00000340: 7265 732d 4469 7374 3a20 6f70 656e 6169  res-Dist: openai
-00000350: 3e3d 312e 362e 310a 5265 7175 6972 6573  >=1.6.1.Requires
-00000360: 2d44 6973 743a 2070 7979 616d 6c3e 3d36  -Dist: pyyaml>=6
-00000370: 2e30 2e31 0a52 6571 7569 7265 732d 4469  .0.1.Requires-Di
-00000380: 7374 3a20 7269 6368 3e3d 3133 2e37 2e30  st: rich>=13.7.0
-00000390: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000003a0: 7472 6169 746c 6574 733e 3d35 2e31 342e  traitlets>=5.14.
-000003b0: 310a 4465 7363 7269 7074 696f 6e2d 436f  1.Description-Co
-000003c0: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
-000003d0: 2f6d 6172 6b64 6f77 6e0a 0a23 2043 6861  /markdown..# Cha
-000003e0: 7444 4247 0a0a 6279 205b 456d 6572 7920  tDBG..by [Emery 
-000003f0: 4265 7267 6572 5d28 6874 7470 733a 2f2f  Berger](https://
-00000400: 656d 6572 7962 6572 6765 722e 636f 6d29  emeryberger.com)
-00000410: 2c20 5b53 7465 7068 656e 2046 7265 756e  , [Stephen Freun
-00000420: 645d 2868 7474 7073 3a2f 2f77 7777 2e63  d](https://www.c
-00000430: 732e 7769 6c6c 6961 6d73 2e65 6475 2f7e  s.williams.edu/~
-00000440: 6672 6575 6e64 2f69 6e64 6578 2e68 746d  freund/index.htm
-00000450: 6c29 2c20 5b4b 796c 6120 4c65 7669 6e5d  l), [Kyla Levin]
-00000460: 2868 7474 7073 3a2f 2f72 6176 656e 626c  (https://ravenbl
-00000470: 6f6f 6430 3030 2e67 6974 6875 622e 696f  ood000.github.io
-00000480: 2f4b 796c 6148 4c65 7669 6e2f 696e 6465  /KylaHLevin/inde
-00000490: 782e 6874 6d6c 292c 205b 4e69 636f 6c61  x.html), [Nicola
-000004a0: 7320 7661 6e20 4b65 6d70 656e 5d28 6874  s van Kempen](ht
-000004b0: 7470 733a 2f2f 6e76 616e 6b65 6d70 656e  tps://nvankempen
-000004c0: 2e63 6f6d 2f29 2028 6f72 6465 7265 6420  .com/) (ordered 
-000004d0: 616c 7068 6162 6574 6963 616c 6c79 290a  alphabetically).
-000004e0: 0a5b 215b 5079 5049 204c 6174 6573 7420  .[![PyPI Latest 
-000004f0: 5265 6c65 6173 655d 2868 7474 7073 3a2f  Release](https:/
-00000500: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000510: 7079 7069 2f76 2f63 6861 7464 6267 2e73  pypi/v/chatdbg.s
-00000520: 7667 295d 2868 7474 7073 3a2f 2f70 7970  vg)](https://pyp
-00000530: 692e 6f72 672f 7072 6f6a 6563 742f 6368  i.org/project/ch
-00000540: 6174 6462 672f 290a 5b21 5b44 6f77 6e6c  atdbg/).[![Downl
-00000550: 6f61 6473 5d28 6874 7470 733a 2f2f 7374  oads](https://st
-00000560: 6174 6963 2e70 6570 792e 7465 6368 2f62  atic.pepy.tech/b
-00000570: 6164 6765 2f63 6861 7464 6267 295d 2868  adge/chatdbg)](h
-00000580: 7474 7073 3a2f 2f70 6570 792e 7465 6368  ttps://pepy.tech
-00000590: 2f70 726f 6a65 6374 2f63 6861 7464 6267  /project/chatdbg
-000005a0: 290a 5b21 5b44 6f77 6e6c 6f61 6473 5d28  ).[![Downloads](
-000005b0: 6874 7470 733a 2f2f 7374 6174 6963 2e70  https://static.p
-000005c0: 6570 792e 7465 6368 2f62 6164 6765 2f63  epy.tech/badge/c
-000005d0: 6861 7464 6267 2f6d 6f6e 7468 295d 2868  hatdbg/month)](h
-000005e0: 7474 7073 3a2f 2f70 6570 792e 7465 6368  ttps://pepy.tech
-000005f0: 2f70 726f 6a65 6374 2f63 6861 7464 6267  /project/chatdbg
-00000600: 290a 0a43 6861 7444 4247 2069 7320 616e  )..ChatDBG is an
-00000610: 2041 492d 6261 7365 6420 6465 6275 6767   AI-based debugg
-00000620: 696e 6720 6173 7369 7374 616e 7420 666f  ing assistant fo
-00000630: 7220 432f 432b 2b2f 5079 7468 6f6e 2f52  r C/C++/Python/R
-00000640: 7573 7420 636f 6465 2074 6861 7420 696e  ust code that in
-00000650: 7465 6772 6174 6573 206c 6172 6765 206c  tegrates large l
-00000660: 616e 6775 6167 6520 6d6f 6465 6c73 2069  anguage models i
-00000670: 6e74 6f20 6120 7374 616e 6461 7264 2064  nto a standard d
-00000680: 6562 7567 6765 7220 2860 7064 6260 2c20  ebugger (`pdb`, 
-00000690: 606c 6c64 6260 2c20 6067 6462 602c 2061  `lldb`, `gdb`, a
-000006a0: 6e64 2060 7769 6e64 6267 6029 2074 6f20  nd `windbg`) to 
-000006b0: 6865 6c70 2064 6562 7567 2079 6f75 7220  help debug your 
-000006c0: 636f 6465 2e20 5769 7468 2043 6861 7444  code. With ChatD
-000006d0: 4247 2c20 796f 7520 6361 6e20 656e 6761  BG, you can enga
-000006e0: 6765 2069 6e20 6120 6469 616c 6f67 2077  ge in a dialog w
-000006f0: 6974 6820 796f 7572 2064 6562 7567 6765  ith your debugge
-00000700: 722c 2061 736b 696e 6720 6f70 656e 2d65  r, asking open-e
-00000710: 6e64 6564 2071 7565 7374 696f 6e73 2061  nded questions a
-00000720: 626f 7574 2079 6f75 7220 7072 6f67 7261  bout your progra
-00000730: 6d2c 206c 696b 6520 6077 6879 2069 7320  m, like `why is 
-00000740: 7820 6e75 6c6c 3f60 2e20 4368 6174 4442  x null?`. ChatDB
-00000750: 4720 7769 6c6c 205f 7461 6b65 2074 6865  G will _take the
-00000760: 2077 6865 656c 5f20 616e 6420 7374 6565   wheel_ and stee
-00000770: 7220 7468 6520 6465 6275 6767 6572 2074  r the debugger t
-00000780: 6f20 616e 7377 6572 2079 6f75 7220 7175  o answer your qu
-00000790: 6572 6965 732e 2043 6861 7444 4247 2063  eries. ChatDBG c
-000007a0: 616e 2070 726f 7669 6465 2065 7272 6f72  an provide error
-000007b0: 2064 6961 676e 6f73 6573 2061 6e64 2073   diagnoses and s
-000007c0: 7567 6765 7374 2066 6978 6573 2e0a 0a41  uggest fixes...A
-000007d0: 7320 6661 7220 6173 2077 6520 6172 6520  s far as we are 
-000007e0: 6177 6172 652c 2043 6861 7444 4247 2069  aware, ChatDBG i
-000007f0: 7320 7468 6520 2a66 6972 7374 2a20 6465  s the *first* de
-00000800: 6275 6767 6572 2074 6f20 6175 746f 6d61  bugger to automa
-00000810: 7469 6361 6c6c 7920 7065 7266 6f72 6d20  tically perform 
-00000820: 726f 6f74 2063 6175 7365 2061 6e61 6c79  root cause analy
-00000830: 7369 7320 616e 6420 746f 2070 726f 7669  sis and to provi
-00000840: 6465 2073 7567 6765 7374 6564 2066 6978  de suggested fix
-00000850: 6573 2e0a 0a46 6f72 2074 6563 686e 6963  es...For technic
-00000860: 616c 2064 6574 6169 6c73 2061 6e64 2061  al details and a
-00000870: 2063 6f6d 706c 6574 6520 6576 616c 7561   complete evalua
-00000880: 7469 6f6e 2c20 7365 6520 6f75 7220 6172  tion, see our ar
-00000890: 5869 7620 7061 7065 722c 205b 5f43 6861  Xiv paper, [_Cha
-000008a0: 7444 4247 3a20 416e 2041 492d 506f 7765  tDBG: An AI-Powe
-000008b0: 7265 6420 4465 6275 6767 696e 6720 4173  red Debugging As
-000008c0: 7369 7374 616e 745f 5d28 6874 7470 733a  sistant_](https:
-000008d0: 2f2f 6172 7869 762e 6f72 672f 6162 732f  //arxiv.org/abs/
-000008e0: 3234 3033 2e31 3633 3534 2920 285b 5044  2403.16354) ([PD
-000008f0: 465d 2868 7474 7073 3a2f 2f67 6974 6875  F](https://githu
-00000900: 622e 636f 6d2f 706c 6173 6d61 2d75 6d61  b.com/plasma-uma
-00000910: 7373 2f43 6861 7444 4247 2f62 6c6f 622f  ss/ChatDBG/blob/
-00000920: 6d61 696e 2f43 6861 7444 4247 2d61 7278  main/ChatDBG-arx
-00000930: 6976 2d32 3430 332e 3136 3335 342e 7064  iv-2403.16354.pd
-00000940: 6629 292e 0a0a 2323 2049 6e73 7461 6c6c  f))...## Install
-00000950: 6174 696f 6e0a 0a3e 202a 2a4e 6f74 652a  ation..> **Note*
-00000960: 2a0a 3e0a 3e20 4368 6174 4442 4720 6e65  *.>.> ChatDBG ne
-00000970: 6564 7320 746f 2062 6520 636f 6e6e 6563  eds to be connec
-00000980: 7465 6420 746f 2061 6e20 5b4f 7065 6e41  ted to an [OpenA
-00000990: 4920 6163 636f 756e 745d 2868 7474 7073  I account](https
-000009a0: 3a2f 2f6f 7065 6e61 692e 636f 6d2f 6170  ://openai.com/ap
-000009b0: 692f 292e 205f 596f 7572 2061 6363 6f75  i/). _Your accou
-000009c0: 6e74 2077 696c 6c20 6e65 6564 2074 6f20  nt will need to 
-000009d0: 6861 7665 2061 2070 6f73 6974 6976 6520  have a positive 
-000009e0: 6261 6c61 6e63 6520 666f 7220 7468 6973  balance for this
-000009f0: 2074 6f20 776f 726b 5f20 285b 6368 6563   to work_ ([chec
-00000a00: 6b20 796f 7572 2062 616c 616e 6365 5d28  k your balance](
-00000a10: 6874 7470 733a 2f2f 706c 6174 666f 726d  https://platform
-00000a20: 2e6f 7065 6e61 692e 636f 6d2f 6163 636f  .openai.com/acco
-00000a30: 756e 742f 7573 6167 6529 292e 2049 6620  unt/usage)). If 
-00000a40: 796f 7520 6861 7665 206e 6576 6572 2070  you have never p
-00000a50: 7572 6368 6173 6564 2063 7265 6469 7473  urchased credits
-00000a60: 2c20 796f 7520 7769 6c6c 206e 6565 6420  , you will need 
-00000a70: 746f 2070 7572 6368 6173 6520 6174 206c  to purchase at l
-00000a80: 6561 7374 205c 2431 2069 6e20 6372 6564  east \$1 in cred
-00000a90: 6974 7320 2869 6620 796f 7572 2041 5049  its (if your API
-00000aa0: 2061 6363 6f75 6e74 2077 6173 2063 7265   account was cre
-00000ab0: 6174 6564 2062 6566 6f72 6520 4175 6775  ated before Augu
-00000ac0: 7374 2031 332c 2032 3032 3329 206f 7220  st 13, 2023) or 
-00000ad0: 5c24 302e 3530 2028 6966 2079 6f75 2068  \$0.50 (if you h
-00000ae0: 6176 6520 6120 6e65 7765 7220 4150 4920  ave a newer API 
-00000af0: 6163 636f 756e 7429 2069 6e20 6f72 6465  account) in orde
-00000b00: 7220 746f 2068 6176 6520 6163 6365 7373  r to have access
-00000b10: 2074 6f20 4750 542d 342c 2077 6869 6368   to GPT-4, which
-00000b20: 2043 6861 7444 4247 2075 7365 732e 205b   ChatDBG uses. [
-00000b30: 4765 7420 6120 6b65 7920 6865 7265 2e5d  Get a key here.]
-00000b40: 2868 7474 7073 3a2f 2f70 6c61 7466 6f72  (https://platfor
-00000b50: 6d2e 6f70 656e 6169 2e63 6f6d 2f61 6363  m.openai.com/acc
-00000b60: 6f75 6e74 2f61 7069 2d6b 6579 7329 0a3e  ount/api-keys).>
-00000b70: 0a3e 204f 6e63 6520 796f 7520 6861 7665  .> Once you have
-00000b80: 2061 6e20 4150 4920 6b65 792c 2073 6574   an API key, set
-00000b90: 2069 7420 6173 2061 6e20 656e 7669 726f   it as an enviro
-00000ba0: 6e6d 656e 7420 7661 7269 6162 6c65 2063  nment variable c
-00000bb0: 616c 6c65 6420 604f 5045 4e41 495f 4150  alled `OPENAI_AP
-00000bc0: 495f 4b45 5960 2e0a 3e0a 3e20 6060 6062  I_KEY`..>.> ```b
-00000bd0: 6173 680a 3e20 6578 706f 7274 204f 5045  ash.> export OPE
-00000be0: 4e41 495f 4150 495f 4b45 593d 3c79 6f75  NAI_API_KEY=<you
-00000bf0: 722d 6170 692d 6b65 793e 0a3e 2060 6060  r-api-key>.> ```
-00000c00: 0a0a 496e 7374 616c 6c20 4368 6174 4442  ..Install ChatDB
-00000c10: 4720 7573 696e 6720 6070 6970 6020 2879  G using `pip` (y
-00000c20: 6f75 206e 6565 6420 746f 2064 6f20 7468  ou need to do th
-00000c30: 6973 2077 6865 7468 6572 2079 6f75 2061  is whether you a
-00000c40: 7265 2064 6562 7567 6769 6e67 2050 7974  re debugging Pyt
-00000c50: 686f 6e2c 2043 2c20 6f72 2043 2b2b 2063  hon, C, or C++ c
-00000c60: 6f64 6529 3a0a 0a60 6060 6261 7368 0a70  ode):..```bash.p
-00000c70: 7974 686f 6e33 202d 6d20 7069 7020 696e  ython3 -m pip in
-00000c80: 7374 616c 6c20 6368 6174 6462 670a 6060  stall chatdbg.``
-00000c90: 600a 0a49 6620 796f 7520 6172 6520 7573  `..If you are us
-00000ca0: 696e 6720 4368 6174 4442 4720 746f 2064  ing ChatDBG to d
-00000cb0: 6562 7567 2050 7974 686f 6e20 7072 6f67  ebug Python prog
-00000cc0: 7261 6d73 2c20 796f 7520 6172 6520 646f  rams, you are do
-00000cd0: 6e65 2e20 4966 2079 6f75 2077 616e 7420  ne. If you want 
-00000ce0: 746f 2075 7365 2043 6861 7444 4247 2074  to use ChatDBG t
-00000cf0: 6f20 6465 6275 6720 6e61 7469 7665 2063  o debug native c
-00000d00: 6f64 6520 7769 7468 2060 6764 6260 206f  ode with `gdb` o
-00000d10: 7220 606c 6c64 6260 2c20 666f 6c6c 6f77  r `lldb`, follow
-00000d20: 2074 6865 2069 6e73 7461 6c6c 6174 696f   the installatio
-00000d30: 6e20 696e 7374 7275 6374 696f 6e73 2062  n instructions b
-00000d40: 656c 6f77 2e0a 0a23 2323 2049 6e73 7461  elow...### Insta
-00000d50: 6c6c 696e 6720 6173 2061 6e20 606c 6c64  lling as an `lld
-00000d60: 6260 2065 7874 656e 7369 6f6e 0a0a 3c64  b` extension..<d
-00000d70: 6574 6169 6c73 3e0a 3c73 756d 6d61 7279  etails>.<summary
-00000d80: 3e0a 3c42 3e3c 5454 3e6c 6c64 623c 2f54  >.<B><TT>lldb</T
-00000d90: 543e 2069 6e73 7461 6c6c 6174 696f 6e20  T> installation 
-00000da0: 696e 7374 7275 6374 696f 6e73 3c2f 423e  instructions</B>
-00000db0: 0a3c 2f73 756d 6d61 7279 3e0a 0a49 6e73  .</summary>..Ins
-00000dc0: 7461 6c6c 2043 6861 7444 4247 2069 6e74  tall ChatDBG int
-00000dd0: 6f20 7468 6520 606c 6c64 6260 2064 6562  o the `lldb` deb
-00000de0: 7567 6765 7220 6279 2072 756e 6e69 6e67  ugger by running
-00000df0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
-00000e00: 6f6d 6d61 6e64 3a0a 0a23 2323 2320 4c69  ommand:..#### Li
-00000e10: 6e75 780a 0a60 6060 6261 7368 0a70 7974  nux..```bash.pyt
-00000e20: 686f 6e33 202d 6d20 7069 7020 696e 7374  hon3 -m pip inst
-00000e30: 616c 6c20 4368 6174 4442 470a 7079 7468  all ChatDBG.pyth
-00000e40: 6f6e 3320 2d63 2027 696d 706f 7274 2063  on3 -c 'import c
-00000e50: 6861 7464 6267 3b20 7072 696e 7428 6622  hatdbg; print(f"
-00000e60: 636f 6d6d 616e 6420 7363 7269 7074 2069  command script i
-00000e70: 6d70 6f72 7420 7b63 6861 7464 6267 2e5f  mport {chatdbg._
-00000e80: 5f70 6174 685f 5f5b 305d 7d2f 6368 6174  _path__[0]}/chat
-00000e90: 6462 675f 6c6c 6462 2e70 7922 2927 203e  dbg_lldb.py")' >
-00000ea0: 3e20 7e2f 2e6c 6c64 6269 6e69 740a 6060  > ~/.lldbinit.``
-00000eb0: 600a 0a49 6620 796f 7520 656e 636f 756e  `..If you encoun
-00000ec0: 7465 7220 616e 2065 7272 6f72 2c20 796f  ter an error, yo
-00000ed0: 7520 6d61 7920 6265 2075 7369 6e67 2061  u may be using a
-00000ee0: 6e20 6f6c 6465 7220 7665 7273 696f 6e20  n older version 
-00000ef0: 6f66 204c 4c56 4d2e 2055 7064 6174 6520  of LLVM. Update 
-00000f00: 746f 2074 6865 206c 6174 6573 7420 7665  to the latest ve
-00000f10: 7273 696f 6e20 6173 2066 6f6c 6c6f 7773  rsion as follows
-00000f20: 3a0a 0a60 6060 0a73 7564 6f20 6170 7420  :..```.sudo apt 
-00000f30: 696e 7374 616c 6c20 2d79 206c 7362 2d72  install -y lsb-r
-00000f40: 656c 6561 7365 2077 6765 7420 736f 6674  elease wget soft
-00000f50: 7761 7265 2d70 726f 7065 7274 6965 732d  ware-properties-
-00000f60: 636f 6d6d 6f6e 2067 6e75 7067 0a63 7572  common gnupg.cur
-00000f70: 6c20 2d73 5366 2068 7474 7073 3a2f 2f61  l -sSf https://a
-00000f80: 7074 2e6c 6c76 6d2e 6f72 672f 6c6c 766d  pt.llvm.org/llvm
-00000f90: 2e73 6820 7c20 7375 646f 2062 6173 6820  .sh | sudo bash 
-00000fa0: 2d73 202d 2d20 3137 2061 6c6c 0a23 204c  -s -- 17 all.# L
-00000fb0: 4c44 4220 6e6f 7720 6176 6169 6c61 626c  LDB now availabl
-00000fc0: 6520 6173 2060 6c6c 6462 2d31 3760 2e0a  e as `lldb-17`..
-00000fd0: 6060 600a 0a23 2323 2320 4d61 630a 0a60  ```..#### Mac..`
-00000fe0: 6060 6261 7368 0a78 6372 756e 2070 7974  ``bash.xcrun pyt
-00000ff0: 686f 6e33 202d 6d20 7069 7020 696e 7374  hon3 -m pip inst
-00001000: 616c 6c20 4368 6174 4442 470a 7863 7275  all ChatDBG.xcru
-00001010: 6e20 7079 7468 6f6e 3320 2d63 2027 696d  n python3 -c 'im
-00001020: 706f 7274 2063 6861 7464 6267 3b20 7072  port chatdbg; pr
-00001030: 696e 7428 6622 636f 6d6d 616e 6420 7363  int(f"command sc
-00001040: 7269 7074 2069 6d70 6f72 7420 7b63 6861  ript import {cha
-00001050: 7464 6267 2e5f 5f70 6174 685f 5f5b 305d  tdbg.__path__[0]
-00001060: 7d2f 6368 6174 6462 675f 6c6c 6462 2e70  }/chatdbg_lldb.p
-00001070: 7922 2927 203e 3e20 7e2f 2e6c 6c64 6269  y")' >> ~/.lldbi
-00001080: 6e69 740a 6060 600a 0a54 6869 7320 7769  nit.```..This wi
-00001090: 6c6c 2069 6e73 7461 6c6c 2043 6861 7444  ll install ChatD
-000010a0: 4247 2061 7320 616e 204c 4c56 4d20 6578  BG as an LLVM ex
-000010b0: 7465 6e73 696f 6e2e 0a3c 2f64 6574 6169  tension..</detai
-000010c0: 6c73 3e0a 0a23 2323 2049 6e73 7461 6c6c  ls>..### Install
-000010d0: 696e 6720 6173 2061 2060 6764 6260 2065  ing as a `gdb` e
-000010e0: 7874 656e 7369 6f6e 0a0a 3c64 6574 6169  xtension..<detai
-000010f0: 6c73 3e0a 3c73 756d 6d61 7279 3e0a 3c42  ls>.<summary>.<B
-00001100: 3e3c 5454 3e67 6462 3c2f 5454 3e20 696e  ><TT>gdb</TT> in
-00001110: 7374 616c 6c61 7469 6f6e 2069 6e73 7472  stallation instr
-00001120: 7563 7469 6f6e 733c 2f42 3e0a 3c2f 7375  uctions</B>.</su
-00001130: 6d6d 6172 793e 0a0a 496e 7374 616c 6c20  mmary>..Install 
-00001140: 4368 6174 4442 4720 696e 746f 2074 6865  ChatDBG into the
-00001150: 2060 6764 6260 2064 6562 7567 6765 7220   `gdb` debugger 
-00001160: 6279 2072 756e 6e69 6e67 2074 6865 2066  by running the f
-00001170: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
-00001180: 3a0a 0a60 6060 6261 7368 0a70 7974 686f  :..```bash.pytho
-00001190: 6e33 202d 6d20 7069 7020 696e 7374 616c  n3 -m pip instal
-000011a0: 6c20 4368 6174 4442 470a 7079 7468 6f6e  l ChatDBG.python
-000011b0: 3320 2d63 2027 696d 706f 7274 2063 6861  3 -c 'import cha
-000011c0: 7464 6267 3b20 7072 696e 7428 6622 736f  tdbg; print(f"so
-000011d0: 7572 6365 207b 6368 6174 6462 672e 5f5f  urce {chatdbg.__
-000011e0: 7061 7468 5f5f 5b30 5d7d 2f63 6861 7464  path__[0]}/chatd
-000011f0: 6267 5f67 6462 2e70 7922 2927 203e 3e20  bg_gdb.py")' >> 
-00001200: 7e2f 2e67 6462 696e 6974 0a60 6060 0a0a  ~/.gdbinit.```..
-00001210: 5468 6973 2077 696c 6c20 696e 7374 616c  This will instal
-00001220: 6c20 4368 6174 4442 4720 6173 2061 2047  l ChatDBG as a G
-00001230: 4442 2065 7874 656e 7369 6f6e 2e0a 3c2f  DB extension..</
-00001240: 6465 7461 696c 733e 0a0a 2323 2320 496e  details>..### In
-00001250: 7374 616c 6c69 6e67 2061 7320 6120 6057  stalling as a `W
-00001260: 696e 4442 4760 2065 7874 656e 7369 6f6e  inDBG` extension
-00001270: 0a0a 3c64 6574 6169 6c73 3e0a 3c73 756d  ..<details>.<sum
-00001280: 6d61 7279 3e0a 3c42 3e3c 5454 3e57 696e  mary>.<B><TT>Win
-00001290: 4442 473c 2f54 543e 2069 6e73 7461 6c6c  DBG</TT> install
-000012a0: 6174 696f 6e20 696e 7374 7275 6374 696f  ation instructio
-000012b0: 6e73 3c2f 423e 0a3c 2f73 756d 6d61 7279  ns</B>.</summary
-000012c0: 3e0a 0a31 2e20 2a2a 496e 7374 616c 6c20  >..1. **Install 
-000012d0: 5769 6e44 4247 2a2a 3a20 466f 6c6c 6f77  WinDBG**: Follow
-000012e0: 2069 6e73 7472 7563 7469 6f6e 7320 5b68   instructions [h
-000012f0: 6572 655d 2868 7474 7073 3a2f 2f6c 6561  ere](https://lea
-00001300: 726e 2e6d 6963 726f 736f 6674 2e63 6f6d  rn.microsoft.com
-00001310: 2f65 6e2d 7573 2f77 696e 646f 7773 2d68  /en-us/windows-h
-00001320: 6172 6477 6172 652f 6472 6976 6572 732f  ardware/drivers/
-00001330: 6465 6275 6767 6572 2f29 2069 6620 6057  debugger/) if `W
-00001340: 696e 4442 4760 2069 7320 6e6f 7420 696e  inDBG` is not in
-00001350: 7374 616c 6c65 6420 616c 7265 6164 792e  stalled already.
-00001360: 0a31 2e20 2a2a 496e 7374 616c 6c20 6076  .1. **Install `v
-00001370: 6370 6b67 602a 2a3a 2046 6f6c 6c6f 7720  cpkg`**: Follow 
-00001380: 696e 7374 7275 6374 696f 6e73 205b 6865  instructions [he
-00001390: 7265 5d28 6874 7470 733a 2f2f 7663 706b  re](https://vcpk
-000013a0: 672e 696f 2f65 6e2f 6765 7474 696e 672d  g.io/en/getting-
-000013b0: 7374 6172 7465 6429 2069 6620 6076 6370  started) if `vcp
-000013c0: 6b67 6020 6973 206e 6f74 2069 6e73 7461  kg` is not insta
-000013d0: 6c6c 6564 2061 6c72 6561 6479 2e0a 312e  lled already..1.
-000013e0: 202a 2a49 6e73 7461 6c6c 2044 6562 7567   **Install Debug
-000013f0: 6769 6e67 2054 6f6f 6c73 2066 6f72 2057  ging Tools for W
-00001400: 696e 646f 7773 2a2a 3a20 496e 7374 616c  indows**: Instal
-00001410: 6c20 7468 6520 5769 6e64 6f77 7320 5344  l the Windows SD
-00001420: 4b20 5b68 6572 655d 2868 7474 7073 3a2f  K [here](https:/
-00001430: 2f64 6576 656c 6f70 6572 2e6d 6963 726f  /developer.micro
-00001440: 736f 6674 2e63 6f6d 2f65 6e2d 7573 2f77  soft.com/en-us/w
-00001450: 696e 646f 7773 2f64 6f77 6e6c 6f61 6473  indows/downloads
-00001460: 2f77 696e 646f 7773 2d73 646b 2f29 2061  /windows-sdk/) a
-00001470: 6e64 2063 6865 636b 2074 6865 2062 6f78  nd check the box
-00001480: 2060 4465 6275 6767 696e 6720 546f 6f6c   `Debugging Tool
-00001490: 7320 666f 7220 5769 6e64 6f77 7360 2e0a  s for Windows`..
-000014a0: 312e 202a 2a4e 6176 6967 6174 6520 746f  1. **Navigate to
-000014b0: 2074 6865 2060 7372 635c 6368 6174 6462   the `src\chatdb
-000014c0: 6760 2064 6972 6563 746f 7279 2a2a 3a20  g` directory**: 
-000014d0: 6063 6420 7372 635c 6368 6174 6462 6760  `cd src\chatdbg`
-000014e0: 0a31 2e20 2a2a 496e 7374 616c 6c20 6e65  .1. **Install ne
-000014f0: 6564 6564 2064 6570 656e 6465 6e63 6965  eded dependencie
-00001500: 732a 2a3a 2052 756e 6076 6370 6b67 2069  s**: Run`vcpkg i
-00001510: 6e73 7461 6c6c 600a 312e 202a 2a42 7569  nstall`.1. **Bui
-00001520: 6c64 2074 6865 2063 6861 7464 6267 2e64  ld the chatdbg.d
-00001530: 6c6c 2065 7874 656e 7369 6f6e 2a2a 3a20  ll extension**: 
-00001540: 5275 6e60 6d6b 6469 7220 6275 696c 6420  Run`mkdir build 
-00001550: 2620 6364 2062 7569 6c64 2026 2063 6d61  & cd build & cma
-00001560: 6b65 202e 2e20 2620 636d 616b 6520 2d2d  ke .. & cmake --
-00001570: 6275 696c 6420 2e20 2620 6364 202e 2e60  build . & cd ..`
-00001580: 0a0a 2a2a 5573 696e 6720 4368 6174 4442  ..**Using ChatDB
-00001590: 472a 2a3a 0a0a 202a 204c 6f61 6420 696e  G**:.. * Load in
-000015a0: 746f 2057 696e 4442 4758 3a0a 2020 202a  to WinDBGX:.   *
-000015b0: 2052 756e 2060 7769 6e64 6267 7820 796f   Run `windbgx yo
-000015c0: 7572 5f65 7865 6375 7461 626c 655f 6865  ur_executable_he
-000015d0: 7265 2e65 7865 600a 2020 202a 2043 6c69  re.exe`.   * Cli
-000015e0: 636b 2074 6865 206d 656e 7520 6974 656d  ck the menu item
-000015f0: 7320 6056 6965 7760 202d 3e20 6043 6f6d  s `View` -> `Com
-00001600: 6d61 6e64 2062 726f 7773 6572 600a 2020  mand browser`.  
-00001610: 202a 2054 7970 6520 602e 6c6f 6164 2064   * Type `.load d
-00001620: 6562 7567 5c63 6861 7464 6267 2e64 6c6c  ebug\chatdbg.dll
-00001630: 600a 202a 2041 6674 6572 2072 756e 6e69  `. * After runni
-00001640: 6e67 2063 6f64 6520 616e 6420 6869 7474  ng code and hitt
-00001650: 696e 6720 616e 2065 7863 6570 7469 6f6e  ing an exception
-00001660: 202f 2073 6967 6e61 6c3a 0a20 2020 2a20   / signal:.   * 
-00001670: 5479 7065 2060 2177 6879 6020 696e 2043  Type `!why` in C
-00001680: 6f6d 6d61 6e64 2062 726f 7773 6572 0a3c  ommand browser.<
-00001690: 2f64 6574 6169 6c73 3e0a 0a0a 2323 2055  /details>...## U
-000016a0: 7361 6765 0a0a 2323 2320 4465 6275 6767  sage..### Debugg
-000016b0: 696e 6720 5079 7468 6f6e 0a0a 546f 2075  ing Python..To u
-000016c0: 7365 2043 6861 7444 4247 2074 6f20 6465  se ChatDBG to de
-000016d0: 6275 6720 5079 7468 6f6e 2070 726f 6772  bug Python progr
-000016e0: 616d 732c 2073 696d 706c 7920 7275 6e20  ams, simply run 
-000016f0: 796f 7572 2050 7974 686f 6e20 7363 7269  your Python scri
-00001700: 7074 2061 7320 666f 6c6c 6f77 733a 0a0a  pt as follows:..
-00001710: 6060 6062 6173 680a 6368 6174 6462 6720  ```bash.chatdbg 
-00001720: 2d63 2063 6f6e 7469 6e75 6520 796f 7572  -c continue your
-00001730: 7363 7269 7074 2e70 790a 6060 600a 0a43  script.py.```..C
-00001740: 6861 7444 4247 2069 7320 616e 2065 7874  hatDBG is an ext
-00001750: 656e 7369 6f6e 206f 6620 7468 6520 7374  ension of the st
-00001760: 616e 6461 7264 2050 7974 686f 6e20 6465  andard Python de
-00001770: 6275 6767 6572 2060 7064 6260 2e20 4c69  bugger `pdb`. Li
-00001780: 6b65 0a60 7064 6260 2c20 7768 656e 2079  ke.`pdb`, when y
-00001790: 6f75 7220 7363 7269 7074 2065 6e63 6f75  our script encou
-000017a0: 6e74 6572 7320 616e 2075 6e63 6175 6768  nters an uncaugh
-000017b0: 7420 6578 6365 7074 696f 6e2c 2043 6861  t exception, Cha
-000017c0: 7444 4247 2077 696c 6c0a 656e 7465 7220  tDBG will.enter 
-000017d0: 706f 7374 206d 6f72 7465 6d20 6465 6275  post mortem debu
-000017e0: 6767 696e 6720 6d6f 6465 2e0a 0a55 6e6c  gging mode...Unl
-000017f0: 696b 6520 6f74 6865 7220 6465 6275 6767  ike other debugg
-00001800: 6572 732c 2079 6f75 2063 616e 2074 6865  ers, you can the
-00001810: 6e20 7573 6520 7468 6520 6077 6879 6020  n use the `why` 
-00001820: 636f 6d6d 616e 6420 746f 2061 736b 0a43  command to ask.C
-00001830: 6861 7444 4247 2077 6879 2079 6f75 7220  hatDBG why your 
-00001840: 7072 6f67 7261 6d20 6661 696c 6564 2061  program failed a
-00001850: 6e64 2067 6574 2061 2073 7567 6765 7374  nd get a suggest
-00001860: 6564 2066 6978 2e0a 0a23 2323 2320 4950  ed fix...#### IP
-00001870: 7974 686f 6e20 616e 6420 4a75 7079 7465  ython and Jupyte
-00001880: 7220 5375 7070 6f72 740a 0a54 6f20 7573  r Support..To us
-00001890: 6520 4368 6174 4442 4720 6173 2074 6865  e ChatDBG as the
-000018a0: 2064 6566 6175 6c74 2064 6562 7567 6765   default debugge
-000018b0: 7220 666f 7220 4950 7974 686f 6e20 6f72  r for IPython or
-000018c0: 2069 6e73 6964 6520 4a75 7079 7465 7220   inside Jupyter 
-000018d0: 4e6f 7465 626f 6f6b 732c 0a63 7265 6174  Notebooks,.creat
-000018e0: 6520 6120 4950 7974 686f 6e20 7072 6f66  e a IPython prof
-000018f0: 696c 6520 616e 6420 7468 656e 2061 6464  ile and then add
-00001900: 2074 6865 206e 6563 6573 7361 7279 2065   the necessary e
-00001910: 7865 6e73 696f 6e73 206f 6e20 7374 6172  xensions on star
-00001920: 7475 702e 2020 284d 6f64 6966 790a 7468  tup.  (Modify.th
-00001930: 6573 6520 6c69 6e65 7320 6173 206e 6563  ese lines as nec
-00001940: 6573 7361 7279 2069 6620 796f 7520 616c  essary if you al
-00001950: 7265 6164 7920 6861 7665 2061 2063 7573  ready have a cus
-00001960: 746f 6d69 7a65 6420 7072 6f66 696c 6520  tomized profile 
-00001970: 6669 6c65 2e29 0a0a 6060 6062 6173 680a  file.)..```bash.
-00001980: 6970 7974 686f 6e20 7072 6f66 696c 6520  ipython profile 
-00001990: 6372 6561 7465 0a65 6368 6f20 2263 2e49  create.echo "c.I
-000019a0: 6e74 6572 6163 7469 7665 5368 656c 6c41  nteractiveShellA
-000019b0: 7070 2e65 7874 656e 7369 6f6e 7320 3d20  pp.extensions = 
-000019c0: 5b27 6368 6174 6462 672e 6368 6174 6462  ['chatdbg.chatdb
-000019d0: 675f 7064 6227 2c20 2769 7079 666c 6f77  g_pdb', 'ipyflow
-000019e0: 275d 2220 3e3e 207e 2f2e 6970 7974 686f  ']" >> ~/.ipytho
-000019f0: 6e2f 7072 6f66 696c 655f 6465 6661 756c  n/profile_defaul
-00001a00: 742f 6970 7974 686f 6e5f 636f 6e66 6967  t/ipython_config
-00001a10: 2e70 790a 6060 600a 0a4f 6e20 7468 6520  .py.```..On the 
-00001a20: 636f 6d6d 616e 6420 6c69 6e65 2c20 796f  command line, yo
-00001a30: 7520 6361 6e20 7468 656e 2072 756e 3a0a  u can then run:.
-00001a40: 0a60 6060 6261 7368 0a69 7079 7468 6f6e  .```bash.ipython
-00001a50: 202d 2d70 6462 2079 6f75 7273 6372 6970   --pdb yourscrip
-00001a60: 742e 7079 0a60 6060 0a0a 496e 7369 6465  t.py.```..Inside
-00001a70: 204a 7570 7974 6572 2c20 7275 6e20 796f   Jupyter, run yo
-00001a80: 7572 206e 6f74 6562 6f6f 6b20 7769 7468  ur notebook with
-00001a90: 2074 6865 205b 6970 7966 6c6f 7720 6b65   the [ipyflow ke
-00001aa0: 726e 656c 5d28 6874 7470 733a 2f2f 6769  rnel](https://gi
-00001ab0: 7468 7562 2e63 6f6d 2f69 7079 666c 6f77  thub.com/ipyflow
-00001ac0: 2f69 7079 666c 6f77 2920 616e 6420 696e  /ipyflow) and in
-00001ad0: 636c 7564 6520 7468 6973 206c 696e 6520  clude this line 
-00001ae0: 6d61 6769 6320 6174 2074 6865 2074 6f70  magic at the top
-00001af0: 206f 6620 7468 6520 6669 6c65 2e0a 0a60   of the file...`
-00001b00: 6060 0a25 7064 620a 6060 600a 0a0a 2323  ``.%pdb.```...##
-00001b10: 2320 4465 6275 6767 696e 6720 6e61 7469  # Debugging nati
-00001b20: 7665 2063 6f64 6520 2843 2c20 432b 2b2c  ve code (C, C++,
-00001b30: 206f 7220 5275 7374 2077 6974 6820 3c54   or Rust with <T
-00001b40: 543e 6c6c 6462 3c2f 5454 3e20 2f20 3c54  T>lldb</TT> / <T
-00001b50: 543e 6764 623c 2f54 543e 290a 0a54 6f20  T>gdb</TT>)..To 
-00001b60: 7573 6520 4368 6174 4442 4720 7769 7468  use ChatDBG with
-00001b70: 2060 6c6c 6462 6020 6f72 2060 6764 6260   `lldb` or `gdb`
-00001b80: 2c20 6a75 7374 2072 756e 206e 6174 6976  , just run nativ
-00001b90: 6520 636f 6465 2028 636f 6d70 696c 6564  e code (compiled
-00001ba0: 2077 6974 6820 602d 6760 2066 6f72 2064   with `-g` for d
-00001bb0: 6562 7567 6769 6e67 2073 796d 626f 6c73  ebugging symbols
-00001bc0: 2920 7769 7468 2079 6f75 7220 6368 6f69  ) with your choi
-00001bd0: 6365 206f 6620 6465 6275 6767 6572 3b20  ce of debugger; 
-00001be0: 7768 656e 2069 7420 6372 6173 6865 732c  when it crashes,
-00001bf0: 2061 736b 2060 7768 7960 2e20 5468 6973   ask `why`. This
-00001c00: 2061 6c73 6f20 776f 726b 7320 666f 7220   also works for 
-00001c10: 706f 7374 206d 6f72 7465 6d20 6465 6275  post mortem debu
-00001c20: 6767 696e 6720 2877 6865 6e20 796f 7520  gging (when you 
-00001c30: 6c6f 6164 2061 2063 6f72 6520 7769 7468  load a core with
-00001c40: 2074 6865 2060 2d63 6020 6f70 7469 6f6e   the `-c` option
-00001c50: 292e 0a0a 3c64 6574 6169 6c73 3e0a 3c73  )...<details>.<s
-00001c60: 756d 6d61 7279 3e0a 3c42 3e44 6562 7567  ummary>.<B>Debug
-00001c70: 6769 6e67 2052 7573 7420 7072 6f67 7261  ging Rust progra
-00001c80: 6d73 3c2f 423e 0a3c 2f73 756d 6d61 7279  ms</B>.</summary
-00001c90: 3e0a 0a54 6f20 7573 6520 4368 6174 4442  >..To use ChatDB
-00001ca0: 4720 7769 7468 2052 7573 742c 2079 6f75  G with Rust, you
-00001cb0: 206e 6565 6420 746f 2064 6f20 7477 6f20   need to do two 
-00001cc0: 7374 6570 733a 206d 6f64 6966 7920 796f  steps: modify yo
-00001cd0: 7572 0a60 4361 7267 6f2e 746f 6d6c 6020  ur.`Cargo.toml` 
-00001ce0: 6669 6c65 2061 6e64 2061 6464 206f 6e65  file and add one
-00001cf0: 206c 696e 6520 746f 2079 6f75 7220 736f   line to your so
-00001d00: 7572 6365 2070 726f 6772 616d 2e0a 0a31  urce program...1
-00001d10: 2e20 4164 6420 7468 6973 2074 6f20 796f  . Add this to yo
-00001d20: 7572 2060 4361 7267 6f2e 746f 6d6c 6020  ur `Cargo.toml` 
-00001d30: 6669 6c65 3a0a 0a60 6060 746f 6d6c 0a5b  file:..```toml.[
-00001d40: 6465 7065 6e64 656e 6369 6573 5d0a 6368  dependencies].ch
-00001d50: 6174 6462 6720 3d20 2230 2e31 2e33 220a  atdbg = "0.1.3".
-00001d60: 0a5b 7072 6f66 696c 652e 6465 765d 0a70  .[profile.dev].p
-00001d70: 616e 6963 203d 2022 6162 6f72 7422 0a0a  anic = "abort"..
-00001d80: 5b70 726f 6669 6c65 2e72 656c 6561 7365  [profile.release
-00001d90: 5d0a 7061 6e69 6320 3d20 2261 626f 7274  ].panic = "abort
-00001da0: 220a 6060 600a 0a32 2e20 496e 2079 6f75  ".```..2. In you
-00001db0: 7220 7072 6f67 7261 6d2c 2061 7070 6c79  r program, apply
-00001dc0: 2074 6865 2060 235b 6368 6174 6462 673a   the `#[chatdbg:
-00001dd0: 3a6d 6169 6e5d 6020 6174 7472 6962 7574  :main]` attribut
-00001de0: 6520 746f 2079 6f75 7220 606d 6169 6e60  e to your `main`
-00001df0: 0a66 756e 6374 696f 6e3a 0a0a 6060 6072  .function:..```r
-00001e00: 7573 740a 235b 6368 6174 6462 673a 3a6d  ust.#[chatdbg::m
-00001e10: 6169 6e5d 0a66 6e20 6d61 696e 2829 207b  ain].fn main() {
-00001e20: 0a60 6060 0a0a 4e6f 7720 796f 7520 6361  .```..Now you ca
-00001e30: 6e20 6465 6275 6720 796f 7572 2052 7573  n debug your Rus
-00001e40: 7420 636f 6465 2077 6974 6820 6067 6462  t code with `gdb
-00001e50: 6020 6f72 2060 6c6c 6462 602e 0a0a 3c2f  ` or `lldb`...</
-00001e60: 6465 7461 696c 733e 0a0a 2323 2320 4578  details>..### Ex
-00001e70: 616d 706c 6573 0a0a 3c64 6574 6169 6c73  amples..<details
-00001e80: 3e0a 3c73 756d 6d61 7279 3e0a 3c42 3e43  >.<summary>.<B>C
-00001e90: 6861 7444 4247 2065 7861 6d70 6c65 2069  hatDBG example i
-00001ea0: 6e20 3c54 543e 6c6c 6462 3c2f 5454 3e3c  n <TT>lldb</TT><
-00001eb0: 2f42 3e0a 3c2f 7375 6d6d 6172 793e 0a0a  /B>.</summary>..
-00001ec0: 6060 6067 6462 0a28 4368 6174 4442 4720  ```gdb.(ChatDBG 
-00001ed0: 6c6c 6462 2920 7275 6e0a 5072 6f63 6573  lldb) run.Proces
-00001ee0: 7320 3835 3439 3420 6c61 756e 6368 6564  s 85494 launched
-00001ef0: 3a20 272f 5573 6572 732f 656d 6572 792f  : '/Users/emery/
-00001f00: 6769 742f 4368 6174 4442 472f 7465 7374  git/ChatDBG/test
-00001f10: 2f61 2e6f 7574 2720 2861 726d 3634 290a  /a.out' (arm64).
-00001f20: 5445 5354 2031 0a54 4553 5420 2d34 3232  TEST 1.TEST -422
-00001f30: 3736 3132 3838 0a54 4553 5420 300a 5445  761288.TEST 0.TE
-00001f40: 5354 2030 0a54 4553 5420 300a 5445 5354  ST 0.TEST 0.TEST
-00001f50: 2030 0a54 4553 5420 300a 5445 5354 2030   0.TEST 0.TEST 0
-00001f60: 0a50 726f 6365 7373 2038 3534 3934 2073  .Process 85494 s
-00001f70: 746f 7070 6564 0a2a 2074 6872 6561 6420  topped.* thread 
-00001f80: 2331 2c20 7175 6575 6520 3d20 2763 6f6d  #1, queue = 'com
-00001f90: 2e61 7070 6c65 2e6d 6169 6e2d 7468 7265  .apple.main-thre
-00001fa0: 6164 272c 2073 746f 7020 7265 6173 6f6e  ad', stop reason
-00001fb0: 203d 2045 5843 5f42 4144 5f41 4343 4553   = EXC_BAD_ACCES
-00001fc0: 5320 2863 6f64 653d 312c 2061 6464 7265  S (code=1, addre
-00001fd0: 7373 3d30 7831 3030 3035 3632 3030 290a  ss=0x100056200).
-00001fe0: 2020 2020 6672 616d 6520 2330 3a20 3078      frame #0: 0x
-00001ff0: 3030 3030 3030 3031 3030 3030 3266 3634  0000000100002f64
-00002000: 2061 2e6f 7574 6066 6f6f 286e 3d38 2c20   a.out`foo(n=8, 
-00002010: 623d 3129 2061 7420 7465 7374 2e63 7070  b=1) at test.cpp
-00002020: 3a37 3a32 320a 2020 2034 2020 2020 2069  :7:22.   4     i
-00002030: 6e74 2078 5b5d 203d 207b 2031 2c20 322c  nt x[] = { 1, 2,
-00002040: 2033 2c20 342c 2035 207d 3b0a 2020 2035   3, 4, 5 };.   5
-00002050: 2020 2020 200a 2020 2036 2020 2020 2076       .   6     v
-00002060: 6f69 6420 666f 6f28 696e 7420 6e2c 2066  oid foo(int n, f
-00002070: 6c6f 6174 2062 2920 7b0a 2d3e 2037 2020  loat b) {.-> 7  
-00002080: 2020 2020 2063 6f75 7420 3c3c 2022 5445       cout << "TE
-00002090: 5354 2022 203c 3c20 785b 6e20 2a20 3130  ST " << x[n * 10
-000020a0: 3030 305d 203c 3c20 656e 646c 3b0a 2020  000] << endl;.  
-000020b0: 2038 2020 2020 207d 0a20 2020 3920 2020   8     }.   9   
-000020c0: 2020 0a20 2020 3130 2020 2020 696e 7420    .   10    int 
-000020d0: 6d61 696e 2829 0a54 6172 6765 7420 303a  main().Target 0:
-000020e0: 2028 612e 6f75 7429 2073 746f 7070 6564   (a.out) stopped
-000020f0: 2e0a 6060 600a 0a41 736b 2060 7768 7960  ..```..Ask `why`
-00002100: 2074 6f20 6861 7665 2043 6861 7444 4247   to have ChatDBG
-00002110: 2070 726f 7669 6465 2061 2068 656c 7066   provide a helpf
-00002120: 756c 2065 7870 6c61 6e61 7469 6f6e 2077  ul explanation w
-00002130: 6879 2074 6869 7320 7072 6f67 7261 6d20  hy this program 
-00002140: 6661 696c 6564 2c20 616e 6420 7375 6767  failed, and sugg
-00002150: 6573 7420 6120 6669 783a 0a0a 0a60 6060  est a fix:...```
-00002160: 6764 620a 2843 6861 7444 4247 206c 6c64  gdb.(ChatDBG lld
-00002170: 6229 2077 6879 0a54 6865 2072 6f6f 7420  b) why.The root 
-00002180: 6361 7573 6520 6f66 2074 6869 7320 6572  cause of this er
-00002190: 726f 7220 6973 2061 6363 6573 7369 6e67  ror is accessing
-000021a0: 2061 6e20 696e 6465 7820 6f66 2074 6865   an index of the
-000021b0: 2061 7272 6179 2060 7860 0a74 6861 7420   array `x`.that 
-000021c0: 6973 206f 7574 206f 6620 626f 756e 6473  is out of bounds
-000021d0: 2e20 496e 2060 666f 6f28 2960 2c20 7468  . In `foo()`, th
-000021e0: 6520 696e 6465 7820 6973 2063 616c 6375  e index is calcu
-000021f0: 6c61 7465 6420 6173 2060 6e20 2a0a 3130  lated as `n *.10
-00002200: 3030 3060 2c20 7768 6963 6820 6361 6e20  000`, which can 
-00002210: 6265 206d 7563 6820 6c61 7267 6572 2074  be much larger t
-00002220: 6861 6e20 7468 6520 7369 7a65 206f 6620  han the size of 
-00002230: 7468 6520 6172 7261 7920 6078 6020 2877  the array `x` (w
-00002240: 6869 6368 0a69 7320 6f6e 6c79 2035 2065  hich.is only 5 e
-00002250: 6c65 6d65 6e74 7329 2e20 496e 2074 6865  lements). In the
-00002260: 2067 6976 656e 2074 7261 6365 2c20 7468   given trace, th
-00002270: 6520 7072 6f67 7261 6d20 6973 2074 7279  e program is try
-00002280: 696e 6720 746f 0a61 6363 6573 7320 7468  ing to.access th
-00002290: 6520 6d65 6d6f 7279 2061 6464 7265 7373  e memory address
-000022a0: 2060 3078 3130 3030 3536 3230 3060 2c20   `0x100056200`, 
-000022b0: 7768 6963 6820 6973 206f 7574 7369 6465  which is outside
-000022c0: 206f 6620 7468 6520 7261 6e67 650a 6f66   of the range.of
-000022d0: 2061 6c6c 6f63 6174 6564 206d 656d 6f72   allocated memor
-000022e0: 7920 666f 7220 7468 6520 6172 7261 7920  y for the array 
-000022f0: 6078 602e 0a0a 546f 2066 6978 2074 6869  `x`...To fix thi
-00002300: 7320 6572 726f 722c 2077 6520 6e65 6564  s error, we need
-00002310: 2074 6f20 656e 7375 7265 2074 6861 7420   to ensure that 
-00002320: 7468 6520 696e 6465 7820 6973 2077 6974  the index is wit
-00002330: 6869 6e20 7468 650a 626f 756e 6473 206f  hin the.bounds o
-00002340: 6620 7468 6520 6172 7261 792e 204f 6e65  f the array. One
-00002350: 2077 6179 2074 6f20 646f 2074 6869 7320   way to do this 
-00002360: 6973 2074 6f20 6368 6563 6b20 7468 6520  is to check the 
-00002370: 7661 6c75 6520 6f66 2060 6e60 0a62 6566  value of `n`.bef
-00002380: 6f72 6520 6361 6c63 756c 6174 696e 6720  ore calculating 
-00002390: 7468 6520 696e 6465 782c 2061 6e64 2065  the index, and e
-000023a0: 6e73 7572 6520 7468 6174 2069 7420 6973  nsure that it is
-000023b0: 206c 6573 7320 7468 616e 2074 6865 2073   less than the s
-000023c0: 697a 650a 6f66 2074 6865 2061 7272 6179  ize.of the array
-000023d0: 2064 6976 6964 6564 2062 7920 7468 6520   divided by the 
-000023e0: 7369 7a65 206f 6620 7468 6520 656c 656d  size of the elem
-000023f0: 656e 742e 2046 6f72 2065 7861 6d70 6c65  ent. For example
-00002400: 2c20 7765 2063 616e 0a6d 6f64 6966 7920  , we can.modify 
-00002410: 6066 6f6f 2829 6020 6173 2066 6f6c 6c6f  `foo()` as follo
-00002420: 7773 3a0a 0a20 2020 2060 6060 0a20 2020  ws:..    ```.   
-00002430: 2076 6f69 6420 666f 6f28 696e 7420 6e2c   void foo(int n,
-00002440: 2066 6c6f 6174 2062 2920 7b0a 2020 2020   float b) {.    
-00002450: 2020 6966 2028 6e20 3c20 3020 7c7c 206e    if (n < 0 || n
-00002460: 203e 3d20 7369 7a65 6f66 2878 292f 7369   >= sizeof(x)/si
-00002470: 7a65 6f66 2878 5b30 5d29 2920 7b0a 2020  zeof(x[0])) {.  
-00002480: 2020 2020 2020 636f 7574 203c 3c20 2245        cout << "E
-00002490: 5252 4f52 3a20 496e 7661 6c69 6420 696e  RROR: Invalid in
-000024a0: 6465 7822 203c 3c20 656e 646c 3b0a 2020  dex" << endl;.  
-000024b0: 2020 2020 2020 7265 7475 726e 3b0a 2020        return;.  
-000024c0: 2020 2020 7d0a 2020 2020 2020 636f 7574      }.      cout
-000024d0: 203c 3c20 2254 4553 5420 2220 3c3c 2078   << "TEST " << x
-000024e0: 5b6e 5d20 3c3c 2065 6e64 6c3b 0a20 2020  [n] << endl;.   
-000024f0: 207d 0a20 2020 2060 6060 0a0a 5468 6973   }.    ```..This
-00002500: 2063 6f64 6520 6368 6563 6b73 2069 6620   code checks if 
-00002510: 606e 6020 6973 2077 6974 6869 6e20 7468  `n` is within th
-00002520: 6520 7661 6c69 6420 7261 6e67 652c 2061  e valid range, a
-00002530: 6e64 2070 7269 6e74 7320 616e 2065 7272  nd prints an err
-00002540: 6f72 0a6d 6573 7361 6765 2069 6620 6974  or.message if it
-00002550: 2069 7320 6e6f 742e 2049 6620 606e 6020   is not. If `n` 
-00002560: 6973 2077 6974 6869 6e20 7468 6520 7261  is within the ra
-00002570: 6e67 652c 2074 6865 2066 756e 6374 696f  nge, the functio
-00002580: 6e20 7072 696e 7473 0a74 6865 2076 616c  n prints.the val
-00002590: 7565 206f 6620 7468 6520 656c 656d 656e  ue of the elemen
-000025a0: 7420 6174 2069 6e64 6578 2060 6e60 206f  t at index `n` o
-000025b0: 6620 6078 602e 2057 6974 6820 7468 6973  f `x`. With this
-000025c0: 206d 6f64 6966 6963 6174 696f 6e2c 0a74   modification,.t
-000025d0: 6865 2070 726f 6772 616d 2077 696c 6c20  he program will 
-000025e0: 6176 6f69 6420 6163 6365 7373 696e 6720  avoid accessing 
-000025f0: 6d65 6d6f 7279 206f 7574 7369 6465 2074  memory outside t
-00002600: 6865 2062 6f75 6e64 7320 6f66 2074 6865  he bounds of the
-00002610: 0a61 7272 6179 2c20 616e 6420 7769 6c6c  .array, and will
-00002620: 2070 7269 6e74 2074 6865 2065 7870 6563   print the expec
-00002630: 7465 6420 6f75 7470 7574 2066 6f72 2076  ted output for v
-00002640: 616c 6964 2069 6e64 6963 6573 2e0a 6060  alid indices..``
-00002650: 600a 3c2f 6465 7461 696c 733e 0a0a 3c64  `.</details>..<d
-00002660: 6574 6169 6c73 3e0a 3c73 756d 6d61 7279  etails>.<summary
-00002670: 3e0a 3c42 3e43 6861 7444 4247 2065 7861  >.<B>ChatDBG exa
-00002680: 6d70 6c65 2069 6e20 5079 7468 6f6e 2028  mple in Python (
-00002690: 3c54 543e 7064 623c 2f54 543e 293c 2f42  <TT>pdb</TT>)</B
-000026a0: 3e0a 3c2f 7375 6d6d 6172 793e 0a0a 6060  >.</summary>..``
-000026b0: 6070 7974 686f 6e0a 5472 6163 6562 6163  `python.Tracebac
-000026c0: 6b20 286d 6f73 7420 7265 6365 6e74 2063  k (most recent c
-000026d0: 616c 6c20 6c61 7374 293a 0a20 2046 696c  all last):.  Fil
-000026e0: 6520 2279 6f75 7273 6372 6970 742e 7079  e "yourscript.py
-000026f0: 222c 206c 696e 6520 392c 2069 6e20 3c6d  ", line 9, in <m
-00002700: 6f64 756c 653e 0a20 2020 2070 7269 6e74  odule>.    print
-00002710: 2874 7279 6d65 2831 3030 2929 0a20 2046  (tryme(100)).  F
-00002720: 696c 6520 2279 6f75 7273 6372 6970 742e  ile "yourscript.
-00002730: 7079 222c 206c 696e 6520 342c 2069 6e20  py", line 4, in 
-00002740: 7472 796d 650a 2020 2020 6966 2078 202f  tryme.    if x /
-00002750: 2069 203e 2032 3a0a 5a65 726f 4469 7669   i > 2:.ZeroDivi
-00002760: 7369 6f6e 4572 726f 723a 2064 6976 6973  sionError: divis
-00002770: 696f 6e20 6279 207a 6572 6f0a 556e 6361  ion by zero.Unca
-00002780: 7567 6874 2065 7863 6570 7469 6f6e 2e20  ught exception. 
-00002790: 456e 7465 7269 6e67 2070 6f73 7420 6d6f  Entering post mo
-000027a0: 7274 656d 2064 6562 7567 6769 6e67 0a52  rtem debugging.R
-000027b0: 756e 6e69 6e67 2027 636f 6e74 2720 6f72  unning 'cont' or
-000027c0: 2027 7374 6570 2720 7769 6c6c 2072 6573   'step' will res
-000027d0: 7461 7274 2074 6865 2070 726f 6772 616d  tart the program
-000027e0: 0a3e 2079 6f75 7273 6372 6970 742e 7079  .> yourscript.py
-000027f0: 2834 2974 7279 6d65 2829 0a2d 3e20 6966  (4)tryme().-> if
-00002800: 2078 202f 2069 203e 2032 3a0a 6060 600a   x / i > 2:.```.
-00002810: 0a41 736b 2060 7768 7960 2074 6f20 6861  .Ask `why` to ha
-00002820: 7665 2043 6861 7444 4247 2070 726f 7669  ve ChatDBG provi
-00002830: 6465 2061 2068 656c 7066 756c 2065 7870  de a helpful exp
-00002840: 6c61 6e61 7469 6f6e 2077 6879 2074 6869  lanation why thi
-00002850: 7320 7072 6f67 7261 6d20 6661 696c 6564  s program failed
-00002860: 2c20 616e 6420 7375 6767 6573 7420 6120  , and suggest a 
-00002870: 6669 783a 0a0a 6060 6070 7974 686f 6e0a  fix:..```python.
-00002880: 2843 6861 7444 4247 2050 6462 2920 7768  (ChatDBG Pdb) wh
-00002890: 790a 5468 6520 726f 6f74 2063 6175 7365  y.The root cause
-000028a0: 206f 6620 7468 6520 6572 726f 7220 6973   of the error is
-000028b0: 2074 6861 7420 7468 6520 636f 6465 2069   that the code i
-000028c0: 7320 6174 7465 6d70 7469 6e67 2074 6f0a  s attempting to.
-000028d0: 6469 7669 6465 2062 7920 7a65 726f 2069  divide by zero i
-000028e0: 6e20 7468 6520 6c69 6e65 2022 6966 2078  n the line "if x
-000028f0: 202f 2069 203e 2032 222e 2041 7320 6920   / i > 2". As i 
-00002900: 7261 6e67 6573 2066 726f 6d20 3020 746f  ranges from 0 to
-00002910: 2039 392c 0a69 7420 7769 6c6c 2065 7665   99,.it will eve
-00002920: 6e74 7561 6c6c 7920 7265 6163 6820 7468  ntually reach th
-00002930: 6520 7661 6c75 6520 6f66 2030 2c20 6361  e value of 0, ca
-00002940: 7573 696e 6720 6120 5a65 726f 4469 7669  using a ZeroDivi
-00002950: 7369 6f6e 4572 726f 722e 0a0a 4120 706f  sionError...A po
-00002960: 7373 6962 6c65 2066 6978 2066 6f72 2074  ssible fix for t
-00002970: 6869 7320 776f 756c 6420 6265 2074 6f20  his would be to 
-00002980: 6164 6420 6120 6368 6563 6b20 666f 7220  add a check for 
-00002990: 6920 6265 696e 6720 6571 7561 6c20 746f  i being equal to
-000029a0: 0a7a 6572 6f20 6265 666f 7265 2070 6572  .zero before per
-000029b0: 666f 726d 696e 6720 7468 6520 6469 7669  forming the divi
-000029c0: 7369 6f6e 2e20 5468 6973 2063 6f75 6c64  sion. This could
-000029d0: 2062 6520 646f 6e65 2062 7920 6164 6469   be done by addi
-000029e0: 6e67 2061 6e0a 6164 6469 7469 6f6e 616c  ng an.additional
-000029f0: 2063 6f6e 6469 7469 6f6e 616c 2073 7461   conditional sta
-00002a00: 7465 6d65 6e74 2c20 7375 6368 2061 7320  tement, such as 
-00002a10: 2269 6620 6920 3d3d 2030 3a20 636f 6e74  "if i == 0: cont
-00002a20: 696e 7565 222c 2074 6f0a 736b 6970 206f  inue", to.skip o
-00002a30: 7665 7220 7468 6520 6974 6572 6174 696f  ver the iteratio
-00002a40: 6e20 7768 656e 2069 2069 7320 7a65 726f  n when i is zero
-00002a50: 2e20 5468 6520 7570 6461 7465 6420 636f  . The updated co
-00002a60: 6465 2077 6f75 6c64 206c 6f6f 6b0a 6c69  de would look.li
-00002a70: 6b65 2074 6869 733a 0a0a 6465 6620 7472  ke this:..def tr
-00002a80: 796d 6528 7829 3a0a 2020 2020 636f 756e  yme(x):.    coun
-00002a90: 7420 3d20 300a 2020 2020 666f 7220 6920  t = 0.    for i 
-00002aa0: 696e 2072 616e 6765 2831 3030 293a 0a20  in range(100):. 
-00002ab0: 2020 2020 2020 2069 6620 6920 3d3d 2030         if i == 0
-00002ac0: 3a0a 2020 2020 2020 2020 2020 2020 636f  :.            co
-00002ad0: 6e74 696e 7565 0a20 2020 2020 2020 2069  ntinue.        i
-00002ae0: 6620 7820 2f20 6920 3e20 323a 0a20 2020  f x / i > 2:.   
-00002af0: 2020 2020 2020 2020 2063 6f75 6e74 202b           count +
-00002b00: 3d20 310a 2020 2020 7265 7475 726e 2063  = 1.    return c
-00002b10: 6f75 6e74 0a0a 6966 205f 5f6e 616d 655f  ount..if __name_
-00002b20: 5f20 3d3d 2027 5f5f 6d61 696e 5f5f 273a  _ == '__main__':
-00002b30: 0a20 2020 2070 7269 6e74 2874 7279 6d65  .    print(tryme
-00002b40: 2831 3030 2929 0a60 6060 0a0a 3c2f 6465  (100)).```..</de
-00002b50: 7461 696c 733e 0a0a                      tails>..
+00000250: 6573 2d50 7974 686f 6e3a 203e 3d33 2e31  es-Python: >=3.1
+00000260: 300a 5265 7175 6972 6573 2d44 6973 743a  0.Requires-Dist:
+00000270: 2061 6e73 6963 6f6c 6f72 733e 3d31 2e31   ansicolors>=1.1
+00000280: 2e38 0a52 6571 7569 7265 732d 4469 7374  .8.Requires-Dist
+00000290: 3a20 6970 6462 3e3d 302e 3133 2e31 330a  : ipdb>=0.13.13.
+000002a0: 5265 7175 6972 6573 2d44 6973 743a 2069  Requires-Dist: i
+000002b0: 7079 666c 6f77 3e3d 302e 302e 3133 300a  pyflow>=0.0.130.
+000002c0: 5265 7175 6972 6573 2d44 6973 743a 2069  Requires-Dist: i
+000002d0: 7079 7468 6f6e 3e3d 382e 3138 2e31 0a52  python>=8.18.1.R
+000002e0: 6571 7569 7265 732d 4469 7374 3a20 6c69  equires-Dist: li
+000002f0: 7465 6c6c 6d3e 3d31 2e33 342e 3132 0a52  tellm>=1.34.12.R
+00000300: 6571 7569 7265 732d 4469 7374 3a20 6c6c  equires-Dist: ll
+00000310: 6d2d 7574 696c 733e 3d30 2e32 2e38 0a52  m-utils>=0.2.8.R
+00000320: 6571 7569 7265 732d 4469 7374 3a20 6e75  equires-Dist: nu
+00000330: 6d70 793e 3d31 2e32 362e 330a 5265 7175  mpy>=1.26.3.Requ
+00000340: 6972 6573 2d44 6973 743a 206f 7065 6e61  ires-Dist: opena
+00000350: 693e 3d31 2e36 2e31 0a52 6571 7569 7265  i>=1.6.1.Require
+00000360: 732d 4469 7374 3a20 7079 7961 6d6c 3e3d  s-Dist: pyyaml>=
+00000370: 362e 302e 310a 5265 7175 6972 6573 2d44  6.0.1.Requires-D
+00000380: 6973 743a 2072 6963 683e 3d31 332e 372e  ist: rich>=13.7.
+00000390: 300a 5265 7175 6972 6573 2d44 6973 743a  0.Requires-Dist:
+000003a0: 2074 7261 6974 6c65 7473 3e3d 352e 3134   traitlets>=5.14
+000003b0: 2e31 0a44 6573 6372 6970 7469 6f6e 2d43  .1.Description-C
+000003c0: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
+000003d0: 742f 6d61 726b 646f 776e 0a0a 2320 4368  t/markdown..# Ch
+000003e0: 6174 4442 470a 0a62 7920 5b45 6d65 7279  atDBG..by [Emery
+000003f0: 2042 6572 6765 725d 2868 7474 7073 3a2f   Berger](https:/
+00000400: 2f65 6d65 7279 6265 7267 6572 2e63 6f6d  /emeryberger.com
+00000410: 292c 205b 5374 6570 6865 6e20 4672 6575  ), [Stephen Freu
+00000420: 6e64 5d28 6874 7470 733a 2f2f 7777 772e  nd](https://www.
+00000430: 6373 2e77 696c 6c69 616d 732e 6564 752f  cs.williams.edu/
+00000440: 7e66 7265 756e 642f 696e 6465 782e 6874  ~freund/index.ht
+00000450: 6d6c 292c 205b 4b79 6c61 204c 6576 696e  ml), [Kyla Levin
+00000460: 5d28 6874 7470 733a 2f2f 7261 7665 6e62  ](https://ravenb
+00000470: 6c6f 6f64 3030 302e 6769 7468 7562 2e69  lood000.github.i
+00000480: 6f2f 4b79 6c61 484c 6576 696e 2f69 6e64  o/KylaHLevin/ind
+00000490: 6578 2e68 746d 6c29 2c20 5b4e 6963 6f6c  ex.html), [Nicol
+000004a0: 6173 2076 616e 204b 656d 7065 6e5d 2868  as van Kempen](h
+000004b0: 7474 7073 3a2f 2f6e 7661 6e6b 656d 7065  ttps://nvankempe
+000004c0: 6e2e 636f 6d2f 2920 286f 7264 6572 6564  n.com/) (ordered
+000004d0: 2061 6c70 6861 6265 7469 6361 6c6c 7929   alphabetically)
+000004e0: 0a0a 5b21 5b50 7950 4920 4c61 7465 7374  ..[![PyPI Latest
+000004f0: 2052 656c 6561 7365 5d28 6874 7470 733a   Release](https:
+00000500: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000510: 2f70 7970 692f 762f 6368 6174 6462 672e  /pypi/v/chatdbg.
+00000520: 7376 6729 5d28 6874 7470 733a 2f2f 7079  svg)](https://py
+00000530: 7069 2e6f 7267 2f70 726f 6a65 6374 2f63  pi.org/project/c
+00000540: 6861 7464 6267 2f29 0a5b 215b 446f 776e  hatdbg/).[![Down
+00000550: 6c6f 6164 735d 2868 7474 7073 3a2f 2f73  loads](https://s
+00000560: 7461 7469 632e 7065 7079 2e74 6563 682f  tatic.pepy.tech/
+00000570: 6261 6467 652f 6368 6174 6462 6729 5d28  badge/chatdbg)](
+00000580: 6874 7470 733a 2f2f 7065 7079 2e74 6563  https://pepy.tec
+00000590: 682f 7072 6f6a 6563 742f 6368 6174 6462  h/project/chatdb
+000005a0: 6729 0a5b 215b 446f 776e 6c6f 6164 735d  g).[![Downloads]
+000005b0: 2868 7474 7073 3a2f 2f73 7461 7469 632e  (https://static.
+000005c0: 7065 7079 2e74 6563 682f 6261 6467 652f  pepy.tech/badge/
+000005d0: 6368 6174 6462 672f 6d6f 6e74 6829 5d28  chatdbg/month)](
+000005e0: 6874 7470 733a 2f2f 7065 7079 2e74 6563  https://pepy.tec
+000005f0: 682f 7072 6f6a 6563 742f 6368 6174 6462  h/project/chatdb
+00000600: 6729 0a0a 4368 6174 4442 4720 6973 2061  g)..ChatDBG is a
+00000610: 6e20 4149 2d62 6173 6564 2064 6562 7567  n AI-based debug
+00000620: 6769 6e67 2061 7373 6973 7461 6e74 2066  ging assistant f
+00000630: 6f72 2043 2f43 2b2b 2f50 7974 686f 6e2f  or C/C++/Python/
+00000640: 5275 7374 2063 6f64 6520 7468 6174 2069  Rust code that i
+00000650: 6e74 6567 7261 7465 7320 6c61 7267 6520  ntegrates large 
+00000660: 6c61 6e67 7561 6765 206d 6f64 656c 7320  language models 
+00000670: 696e 746f 2061 2073 7461 6e64 6172 6420  into a standard 
+00000680: 6465 6275 6767 6572 2028 6070 6462 602c  debugger (`pdb`,
+00000690: 2060 6c6c 6462 602c 2060 6764 6260 2c20   `lldb`, `gdb`, 
+000006a0: 616e 6420 6077 696e 6462 6760 2920 746f  and `windbg`) to
+000006b0: 2068 656c 7020 6465 6275 6720 796f 7572   help debug your
+000006c0: 2063 6f64 652e 2057 6974 6820 4368 6174   code. With Chat
+000006d0: 4442 472c 2079 6f75 2063 616e 2065 6e67  DBG, you can eng
+000006e0: 6167 6520 696e 2061 2064 6961 6c6f 6720  age in a dialog 
+000006f0: 7769 7468 2079 6f75 7220 6465 6275 6767  with your debugg
+00000700: 6572 2c20 6173 6b69 6e67 206f 7065 6e2d  er, asking open-
+00000710: 656e 6465 6420 7175 6573 7469 6f6e 7320  ended questions 
+00000720: 6162 6f75 7420 796f 7572 2070 726f 6772  about your progr
+00000730: 616d 2c20 6c69 6b65 2060 7768 7920 6973  am, like `why is
+00000740: 2078 206e 756c 6c3f 602e 2043 6861 7444   x null?`. ChatD
+00000750: 4247 2077 696c 6c20 5f74 616b 6520 7468  BG will _take th
+00000760: 6520 7768 6565 6c5f 2061 6e64 2073 7465  e wheel_ and ste
+00000770: 6572 2074 6865 2064 6562 7567 6765 7220  er the debugger 
+00000780: 746f 2061 6e73 7765 7220 796f 7572 2071  to answer your q
+00000790: 7565 7269 6573 2e20 4368 6174 4442 4720  ueries. ChatDBG 
+000007a0: 6361 6e20 7072 6f76 6964 6520 6572 726f  can provide erro
+000007b0: 7220 6469 6167 6e6f 7365 7320 616e 6420  r diagnoses and 
+000007c0: 7375 6767 6573 7420 6669 7865 732e 0a0a  suggest fixes...
+000007d0: 4173 2066 6172 2061 7320 7765 2061 7265  As far as we are
+000007e0: 2061 7761 7265 2c20 4368 6174 4442 4720   aware, ChatDBG 
+000007f0: 6973 2074 6865 202a 6669 7273 742a 2064  is the *first* d
+00000800: 6562 7567 6765 7220 746f 2061 7574 6f6d  ebugger to autom
+00000810: 6174 6963 616c 6c79 2070 6572 666f 726d  atically perform
+00000820: 2072 6f6f 7420 6361 7573 6520 616e 616c   root cause anal
+00000830: 7973 6973 2061 6e64 2074 6f20 7072 6f76  ysis and to prov
+00000840: 6964 6520 7375 6767 6573 7465 6420 6669  ide suggested fi
+00000850: 7865 732e 0a0a 2a2a 5761 7463 6820 4368  xes...**Watch Ch
+00000860: 6174 4442 4720 696e 2061 6374 696f 6e21  atDBG in action!
+00000870: 2a2a 0a7c 204c 4c44 4220 6f6e 205b 7465  **.| LLDB on [te
+00000880: 7374 2d6f 7665 7266 6c6f 772e 6370 705d  st-overflow.cpp]
+00000890: 2873 616d 706c 6573 2f63 7070 2f74 6573  (samples/cpp/tes
+000008a0: 742d 6f76 6572 666c 6f77 2e63 7070 2920  t-overflow.cpp) 
+000008b0: 7c20 4744 4220 6f6e 205b 7465 7374 2d6f  | GDB on [test-o
+000008c0: 7665 7266 6c6f 772e 6370 705d 2873 616d  verflow.cpp](sam
+000008d0: 706c 6573 2f63 7070 2f74 6573 742d 6f76  ples/cpp/test-ov
+000008e0: 6572 666c 6f77 2e63 7070 2920 207c 2050  erflow.cpp)  | P
+000008f0: 6462 206f 6e20 5b62 6f6f 7473 7472 6170  db on [bootstrap
+00000900: 2e70 795d 2873 616d 706c 6573 2f70 7974  .py](samples/pyt
+00000910: 686f 6e2f 626f 6f74 7374 7261 702e 7079  hon/bootstrap.py
+00000920: 2920 7c0a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d  ) |.|:----------
+00000930: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a  ---------------:
+00000940: 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |:--------------
+00000950: 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a 2d2d  -----------:|:--
+00000960: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000970: 2d2d 2d2d 2d2d 2d3a 7c0a 7c20 3c61 2068  -------:|.| <a h
+00000980: 7265 663d 2268 7474 7073 3a2f 2f61 7363  ref="https://asc
+00000990: 6969 6e65 6d61 2e6f 7267 2f61 2f52 7341  iinema.org/a/RsA
+000009a0: 4746 466d 7369 6349 764d 5738 7867 7650  GFFmsicIvMW8xgvP
+000009b0: 5036 5057 3266 2220 7461 7267 6574 3d22  P6PW2f" target="
+000009c0: 5f62 6c61 6e6b 223e 3c69 6d67 2073 7263  _blank"><img src
+000009d0: 3d22 6d65 6469 612f 6c6c 6462 2e73 7667  ="media/lldb.svg
+000009e0: 2220 2f3e 3c2f 613e 7c20 3c61 2068 7265  " /></a>| <a hre
+000009f0: 663d 2268 7474 7073 3a2f 2f61 7363 6969  f="https://ascii
+00000a00: 6e65 6d61 2e6f 7267 2f61 2f62 4d57 4f79  nema.org/a/bMWOy
+00000a10: 7972 6837 5758 5773 5443 4662 6f79 4b70  yrh7WXWsTCFboyKp
+00000a20: 7177 5471 2220 7461 7267 6574 3d22 5f62  qwTq" target="_b
+00000a30: 6c61 6e6b 223e 3c69 6d67 2073 7263 3d22  lank"><img src="
+00000a40: 6d65 6469 612f 6764 622e 7376 6722 202f  media/gdb.svg" /
+00000a50: 3e3c 2f61 3e7c 3c61 2068 7265 663d 2268  ></a>|<a href="h
+00000a60: 7474 7073 3a2f 2f61 7363 6969 6e65 6d61  ttps://asciinema
+00000a70: 2e6f 7267 2f61 2f71 756c 7869 4a54 7177  .org/a/qulxiJTqw
+00000a80: 5652 4a50 614d 5a31 6863 4273 3643 6c75  VRJPaMZ1hcBs6Clu
+00000a90: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00000aa0: 223e 3c69 6d67 2073 7263 3d22 6d65 6469  "><img src="medi
+00000ab0: 612f 7064 622e 7376 6722 202f 3e3c 2f61  a/pdb.svg" /></a
+00000ac0: 3e7c 0a0a 466f 7220 7465 6368 6e69 6361  >|..For technica
+00000ad0: 6c20 6465 7461 696c 7320 616e 6420 6120  l details and a 
+00000ae0: 636f 6d70 6c65 7465 2065 7661 6c75 6174  complete evaluat
+00000af0: 696f 6e2c 2073 6565 206f 7572 2061 7258  ion, see our arX
+00000b00: 6976 2070 6170 6572 2c20 5b5f 4368 6174  iv paper, [_Chat
+00000b10: 4442 473a 2041 6e20 4149 2d50 6f77 6572  DBG: An AI-Power
+00000b20: 6564 2044 6562 7567 6769 6e67 2041 7373  ed Debugging Ass
+00000b30: 6973 7461 6e74 5f5d 2868 7474 7073 3a2f  istant_](https:/
+00000b40: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
+00000b50: 3430 332e 3136 3335 3429 2028 5b50 4446  403.16354) ([PDF
+00000b60: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000b70: 2e63 6f6d 2f70 6c61 736d 612d 756d 6173  .com/plasma-umas
+00000b80: 732f 4368 6174 4442 472f 626c 6f62 2f6d  s/ChatDBG/blob/m
+00000b90: 6169 6e2f 4368 6174 4442 472d 6172 7869  ain/ChatDBG-arxi
+00000ba0: 762d 3234 3033 2e31 3633 3534 2e70 6466  v-2403.16354.pdf
+00000bb0: 2929 2e0a 0a3e 205b 214e 4f54 455d 0a3e  ))...> [!NOTE].>
+00000bc0: 0a3e 2043 6861 7444 4247 2066 6f72 2060  .> ChatDBG for `
+00000bd0: 7064 6260 2c20 606c 6c64 6260 2c20 616e  pdb`, `lldb`, an
+00000be0: 6420 6067 6462 6020 6172 6520 6665 6174  d `gdb` are feat
+00000bf0: 7572 652d 636f 6d70 6c65 7465 3b20 7765  ure-complete; we
+00000c00: 2061 7265 2063 7572 7265 6e74 6c79 2062   are currently b
+00000c10: 6163 6b70 6f72 7469 6e67 2066 6561 7475  ackporting featu
+00000c20: 7265 7320 666f 7220 7468 6573 6520 6465  res for these de
+00000c30: 6275 6767 6572 7320 696e 746f 2074 6865  buggers into the
+00000c40: 206f 7468 6572 2064 6562 7567 6765 7273   other debuggers
+00000c50: 2e0a 3e0a 0a23 2320 496e 7374 616c 6c61  ..>..## Installa
+00000c60: 7469 6f6e 0a0a 3e20 5b21 494d 504f 5254  tion..> [!IMPORT
+00000c70: 414e 545d 0a3e 0a3e 2043 6861 7444 4247  ANT].>.> ChatDBG
+00000c80: 2063 7572 7265 6e74 6c79 206e 6565 6473   currently needs
+00000c90: 2074 6f20 6265 2063 6f6e 6e65 6374 6564   to be connected
+00000ca0: 2074 6f20 616e 205b 4f70 656e 4149 2061   to an [OpenAI a
+00000cb0: 6363 6f75 6e74 5d28 6874 7470 733a 2f2f  ccount](https://
+00000cc0: 6f70 656e 6169 2e63 6f6d 2f61 7069 2f29  openai.com/api/)
+00000cd0: 2e20 5f59 6f75 7220 6163 636f 756e 7420  . _Your account 
+00000ce0: 7769 6c6c 206e 6565 6420 746f 2068 6176  will need to hav
+00000cf0: 6520 6120 706f 7369 7469 7665 2062 616c  e a positive bal
+00000d00: 616e 6365 2066 6f72 2074 6869 7320 746f  ance for this to
+00000d10: 2077 6f72 6b5f 2028 5b63 6865 636b 2079   work_ ([check y
+00000d20: 6f75 7220 6261 6c61 6e63 655d 2868 7474  our balance](htt
+00000d30: 7073 3a2f 2f70 6c61 7466 6f72 6d2e 6f70  ps://platform.op
+00000d40: 656e 6169 2e63 6f6d 2f61 6363 6f75 6e74  enai.com/account
+00000d50: 2f75 7361 6765 2929 2e20 4966 2079 6f75  /usage)). If you
+00000d60: 2068 6176 6520 6e65 7665 7220 7075 7263   have never purc
+00000d70: 6861 7365 6420 6372 6564 6974 732c 2079  hased credits, y
+00000d80: 6f75 2077 696c 6c20 6e65 6564 2074 6f20  ou will need to 
+00000d90: 7075 7263 6861 7365 2061 7420 6c65 6173  purchase at leas
+00000da0: 7420 5c24 3120 696e 2063 7265 6469 7473  t \$1 in credits
+00000db0: 2028 6966 2079 6f75 7220 4150 4920 6163   (if your API ac
+00000dc0: 636f 756e 7420 7761 7320 6372 6561 7465  count was create
+00000dd0: 6420 6265 666f 7265 2041 7567 7573 7420  d before August 
+00000de0: 3133 2c20 3230 3233 2920 6f72 205c 2430  13, 2023) or \$0
+00000df0: 2e35 3020 2869 6620 796f 7520 6861 7665  .50 (if you have
+00000e00: 2061 206e 6577 6572 2041 5049 2061 6363   a newer API acc
+00000e10: 6f75 6e74 2920 696e 206f 7264 6572 2074  ount) in order t
+00000e20: 6f20 6861 7665 2061 6363 6573 7320 746f  o have access to
+00000e30: 2047 5054 2d34 2c20 7768 6963 6820 4368   GPT-4, which Ch
+00000e40: 6174 4442 4720 7573 6573 2e20 5b47 6574  atDBG uses. [Get
+00000e50: 2061 206b 6579 2068 6572 652e 5d28 6874   a key here.](ht
+00000e60: 7470 733a 2f2f 706c 6174 666f 726d 2e6f  tps://platform.o
+00000e70: 7065 6e61 692e 636f 6d2f 6163 636f 756e  penai.com/accoun
+00000e80: 742f 6170 692d 6b65 7973 290a 3e0a 3e20  t/api-keys).>.> 
+00000e90: 4f6e 6365 2079 6f75 2068 6176 6520 616e  Once you have an
+00000ea0: 2041 5049 206b 6579 2c20 7365 7420 6974   API key, set it
+00000eb0: 2061 7320 616e 2065 6e76 6972 6f6e 6d65   as an environme
+00000ec0: 6e74 2076 6172 6961 626c 6520 6361 6c6c  nt variable call
+00000ed0: 6564 2060 4f50 454e 4149 5f41 5049 5f4b  ed `OPENAI_API_K
+00000ee0: 4559 602e 0a3e 0a3e 2060 6060 6261 7368  EY`..>.> ```bash
+00000ef0: 0a3e 2065 7870 6f72 7420 4f50 454e 4149  .> export OPENAI
+00000f00: 5f41 5049 5f4b 4559 3d3c 796f 7572 2d61  _API_KEY=<your-a
+00000f10: 7069 2d6b 6579 3e0a 3e20 6060 600a 0a49  pi-key>.> ```..I
+00000f20: 6e73 7461 6c6c 2043 6861 7444 4247 2075  nstall ChatDBG u
+00000f30: 7369 6e67 2060 7069 7060 2028 796f 7520  sing `pip` (you 
+00000f40: 6e65 6564 2074 6f20 646f 2074 6869 7320  need to do this 
+00000f50: 7768 6574 6865 7220 796f 7520 6172 6520  whether you are 
+00000f60: 6465 6275 6767 696e 6720 5079 7468 6f6e  debugging Python
+00000f70: 2c20 432c 206f 7220 432b 2b20 636f 6465  , C, or C++ code
+00000f80: 293a 0a0a 6060 6062 6173 680a 7079 7468  ):..```bash.pyth
+00000f90: 6f6e 3320 2d6d 2070 6970 2069 6e73 7461  on3 -m pip insta
+00000fa0: 6c6c 2063 6861 7464 6267 0a60 6060 0a0a  ll chatdbg.```..
+00000fb0: 4966 2079 6f75 2061 7265 2075 7369 6e67  If you are using
+00000fc0: 2043 6861 7444 4247 2074 6f20 6465 6275   ChatDBG to debu
+00000fd0: 6720 5079 7468 6f6e 2070 726f 6772 616d  g Python program
+00000fe0: 732c 2079 6f75 2061 7265 2064 6f6e 652e  s, you are done.
+00000ff0: 2049 6620 796f 7520 7761 6e74 2074 6f20   If you want to 
+00001000: 7573 6520 4368 6174 4442 4720 746f 2064  use ChatDBG to d
+00001010: 6562 7567 206e 6174 6976 6520 636f 6465  ebug native code
+00001020: 2077 6974 6820 6067 6462 6020 6f72 2060   with `gdb` or `
+00001030: 6c6c 6462 602c 2066 6f6c 6c6f 7720 7468  lldb`, follow th
+00001040: 6520 696e 7374 616c 6c61 7469 6f6e 2069  e installation i
+00001050: 6e73 7472 7563 7469 6f6e 7320 6265 6c6f  nstructions belo
+00001060: 772e 0a0a 2323 2320 496e 7374 616c 6c69  w...### Installi
+00001070: 6e67 2061 7320 616e 2060 6c6c 6462 6020  ng as an `lldb` 
+00001080: 6578 7465 6e73 696f 6e0a 0a3c 6465 7461  extension..<deta
+00001090: 696c 733e 0a3c 7375 6d6d 6172 793e 0a3c  ils>.<summary>.<
+000010a0: 423e 3c54 543e 6c6c 6462 3c2f 5454 3e20  B><TT>lldb</TT> 
+000010b0: 696e 7374 616c 6c61 7469 6f6e 2069 6e73  installation ins
+000010c0: 7472 7563 7469 6f6e 733c 2f42 3e0a 3c2f  tructions</B>.</
+000010d0: 7375 6d6d 6172 793e 0a0a 496e 7374 616c  summary>..Instal
+000010e0: 6c20 4368 6174 4442 4720 696e 746f 2074  l ChatDBG into t
+000010f0: 6865 2060 6c6c 6462 6020 6465 6275 6767  he `lldb` debugg
+00001100: 6572 2062 7920 7275 6e6e 696e 6720 7468  er by running th
+00001110: 6520 666f 6c6c 6f77 696e 6720 636f 6d6d  e following comm
+00001120: 616e 643a 0a0a 2323 2323 204c 696e 7578  and:..#### Linux
+00001130: 0a0a 6060 6062 6173 680a 7079 7468 6f6e  ..```bash.python
+00001140: 3320 2d6d 2070 6970 2069 6e73 7461 6c6c  3 -m pip install
+00001150: 2043 6861 7444 4247 0a70 7974 686f 6e33   ChatDBG.python3
+00001160: 202d 6320 2769 6d70 6f72 7420 6368 6174   -c 'import chat
+00001170: 6462 673b 2070 7269 6e74 2866 2263 6f6d  dbg; print(f"com
+00001180: 6d61 6e64 2073 6372 6970 7420 696d 706f  mand script impo
+00001190: 7274 207b 6368 6174 6462 672e 5f5f 7061  rt {chatdbg.__pa
+000011a0: 7468 5f5f 5b30 5d7d 2f63 6861 7464 6267  th__[0]}/chatdbg
+000011b0: 5f6c 6c64 622e 7079 2229 2720 3e3e 207e  _lldb.py")' >> ~
+000011c0: 2f2e 6c6c 6462 696e 6974 0a60 6060 0a0a  /.lldbinit.```..
+000011d0: 4966 2079 6f75 2065 6e63 6f75 6e74 6572  If you encounter
+000011e0: 2061 6e20 6572 726f 722c 2079 6f75 206d   an error, you m
+000011f0: 6179 2062 6520 7573 696e 6720 616e 206f  ay be using an o
+00001200: 6c64 6572 2076 6572 7369 6f6e 206f 6620  lder version of 
+00001210: 4c4c 564d 2e20 5570 6461 7465 2074 6f20  LLVM. Update to 
+00001220: 7468 6520 6c61 7465 7374 2076 6572 7369  the latest versi
+00001230: 6f6e 2061 7320 666f 6c6c 6f77 733a 0a0a  on as follows:..
+00001240: 6060 600a 7375 646f 2061 7074 2069 6e73  ```.sudo apt ins
+00001250: 7461 6c6c 202d 7920 6c73 622d 7265 6c65  tall -y lsb-rele
+00001260: 6173 6520 7767 6574 2073 6f66 7477 6172  ase wget softwar
+00001270: 652d 7072 6f70 6572 7469 6573 2d63 6f6d  e-properties-com
+00001280: 6d6f 6e20 676e 7570 670a 6375 726c 202d  mon gnupg.curl -
+00001290: 7353 6620 6874 7470 733a 2f2f 6170 742e  sSf https://apt.
+000012a0: 6c6c 766d 2e6f 7267 2f6c 6c76 6d2e 7368  llvm.org/llvm.sh
+000012b0: 207c 2073 7564 6f20 6261 7368 202d 7320   | sudo bash -s 
+000012c0: 2d2d 2031 3820 616c 6c0a 2320 4c4c 4442  -- 18 all.# LLDB
+000012d0: 206e 6f77 2061 7661 696c 6162 6c65 2061   now available a
+000012e0: 7320 606c 6c64 622d 3138 602e 0a60 6060  s `lldb-18`..```
+000012f0: 0a0a 2323 2323 204d 6163 0a0a 6060 6062  ..#### Mac..```b
+00001300: 6173 680a 7863 7275 6e20 7079 7468 6f6e  ash.xcrun python
+00001310: 3320 2d6d 2070 6970 2069 6e73 7461 6c6c  3 -m pip install
+00001320: 2043 6861 7444 4247 0a78 6372 756e 2070   ChatDBG.xcrun p
+00001330: 7974 686f 6e33 202d 6320 2769 6d70 6f72  ython3 -c 'impor
+00001340: 7420 6368 6174 6462 673b 2070 7269 6e74  t chatdbg; print
+00001350: 2866 2263 6f6d 6d61 6e64 2073 6372 6970  (f"command scrip
+00001360: 7420 696d 706f 7274 207b 6368 6174 6462  t import {chatdb
+00001370: 672e 5f5f 7061 7468 5f5f 5b30 5d7d 2f63  g.__path__[0]}/c
+00001380: 6861 7464 6267 5f6c 6c64 622e 7079 2229  hatdbg_lldb.py")
+00001390: 2720 3e3e 207e 2f2e 6c6c 6462 696e 6974  ' >> ~/.lldbinit
+000013a0: 0a60 6060 0a0a 5468 6973 2077 696c 6c20  .```..This will 
+000013b0: 696e 7374 616c 6c20 4368 6174 4442 4720  install ChatDBG 
+000013c0: 6173 2061 6e20 4c4c 564d 2065 7874 656e  as an LLVM exten
+000013d0: 7369 6f6e 2e0a 3c2f 6465 7461 696c 733e  sion..</details>
+000013e0: 0a0a 2323 2320 496e 7374 616c 6c69 6e67  ..### Installing
+000013f0: 2061 7320 6120 6067 6462 6020 6578 7465   as a `gdb` exte
+00001400: 6e73 696f 6e0a 0a3c 6465 7461 696c 733e  nsion..<details>
+00001410: 0a3c 7375 6d6d 6172 793e 0a3c 423e 3c54  .<summary>.<B><T
+00001420: 543e 6764 623c 2f54 543e 2069 6e73 7461  T>gdb</TT> insta
+00001430: 6c6c 6174 696f 6e20 696e 7374 7275 6374  llation instruct
+00001440: 696f 6e73 3c2f 423e 0a3c 2f73 756d 6d61  ions</B>.</summa
+00001450: 7279 3e0a 0a49 6e73 7461 6c6c 2043 6861  ry>..Install Cha
+00001460: 7444 4247 2069 6e74 6f20 7468 6520 6067  tDBG into the `g
+00001470: 6462 6020 6465 6275 6767 6572 2062 7920  db` debugger by 
+00001480: 7275 6e6e 696e 6720 7468 6520 666f 6c6c  running the foll
+00001490: 6f77 696e 6720 636f 6d6d 616e 643a 0a0a  owing command:..
+000014a0: 6060 6062 6173 680a 7079 7468 6f6e 3320  ```bash.python3 
+000014b0: 2d6d 2070 6970 2069 6e73 7461 6c6c 2043  -m pip install C
+000014c0: 6861 7444 4247 0a70 7974 686f 6e33 202d  hatDBG.python3 -
+000014d0: 6320 2769 6d70 6f72 7420 6368 6174 6462  c 'import chatdb
+000014e0: 673b 2070 7269 6e74 2866 2273 6f75 7263  g; print(f"sourc
+000014f0: 6520 7b63 6861 7464 6267 2e5f 5f70 6174  e {chatdbg.__pat
+00001500: 685f 5f5b 305d 7d2f 6368 6174 6462 675f  h__[0]}/chatdbg_
+00001510: 6764 622e 7079 2229 2720 3e3e 207e 2f2e  gdb.py")' >> ~/.
+00001520: 6764 6269 6e69 740a 6060 600a 0a54 6869  gdbinit.```..Thi
+00001530: 7320 7769 6c6c 2069 6e73 7461 6c6c 2043  s will install C
+00001540: 6861 7444 4247 2061 7320 6120 4744 4220  hatDBG as a GDB 
+00001550: 6578 7465 6e73 696f 6e2e 0a3c 2f64 6574  extension..</det
+00001560: 6169 6c73 3e0a 0a23 2323 2049 6e73 7461  ails>..### Insta
+00001570: 6c6c 696e 6720 6173 2061 2060 5769 6e44  lling as a `WinD
+00001580: 4247 6020 6578 7465 6e73 696f 6e0a 0a3c  BG` extension..<
+00001590: 6465 7461 696c 733e 0a3c 7375 6d6d 6172  details>.<summar
+000015a0: 793e 0a3c 423e 3c54 543e 5769 6e44 4247  y>.<B><TT>WinDBG
+000015b0: 3c2f 5454 3e20 696e 7374 616c 6c61 7469  </TT> installati
+000015c0: 6f6e 2069 6e73 7472 7563 7469 6f6e 733c  on instructions<
+000015d0: 2f42 3e0a 3c2f 7375 6d6d 6172 793e 0a0a  /B>.</summary>..
+000015e0: 312e 202a 2a49 6e73 7461 6c6c 2057 696e  1. **Install Win
+000015f0: 4442 472a 2a3a 2046 6f6c 6c6f 7720 696e  DBG**: Follow in
+00001600: 7374 7275 6374 696f 6e73 205b 6865 7265  structions [here
+00001610: 5d28 6874 7470 733a 2f2f 6c65 6172 6e2e  ](https://learn.
+00001620: 6d69 6372 6f73 6f66 742e 636f 6d2f 656e  microsoft.com/en
+00001630: 2d75 732f 7769 6e64 6f77 732d 6861 7264  -us/windows-hard
+00001640: 7761 7265 2f64 7269 7665 7273 2f64 6562  ware/drivers/deb
+00001650: 7567 6765 722f 2920 6966 2060 5769 6e44  ugger/) if `WinD
+00001660: 4247 6020 6973 206e 6f74 2069 6e73 7461  BG` is not insta
+00001670: 6c6c 6564 2061 6c72 6561 6479 2e0a 312e  lled already..1.
+00001680: 202a 2a49 6e73 7461 6c6c 2060 7663 706b   **Install `vcpk
+00001690: 6760 2a2a 3a20 466f 6c6c 6f77 2069 6e73  g`**: Follow ins
+000016a0: 7472 7563 7469 6f6e 7320 5b68 6572 655d  tructions [here]
+000016b0: 2868 7474 7073 3a2f 2f76 6370 6b67 2e69  (https://vcpkg.i
+000016c0: 6f2f 656e 2f67 6574 7469 6e67 2d73 7461  o/en/getting-sta
+000016d0: 7274 6564 2920 6966 2060 7663 706b 6760  rted) if `vcpkg`
+000016e0: 2069 7320 6e6f 7420 696e 7374 616c 6c65   is not installe
+000016f0: 6420 616c 7265 6164 792e 0a31 2e20 2a2a  d already..1. **
+00001700: 496e 7374 616c 6c20 4465 6275 6767 696e  Install Debuggin
+00001710: 6720 546f 6f6c 7320 666f 7220 5769 6e64  g Tools for Wind
+00001720: 6f77 732a 2a3a 2049 6e73 7461 6c6c 2074  ows**: Install t
+00001730: 6865 2057 696e 646f 7773 2053 444b 205b  he Windows SDK [
+00001740: 6865 7265 5d28 6874 7470 733a 2f2f 6465  here](https://de
+00001750: 7665 6c6f 7065 722e 6d69 6372 6f73 6f66  veloper.microsof
+00001760: 742e 636f 6d2f 656e 2d75 732f 7769 6e64  t.com/en-us/wind
+00001770: 6f77 732f 646f 776e 6c6f 6164 732f 7769  ows/downloads/wi
+00001780: 6e64 6f77 732d 7364 6b2f 2920 616e 6420  ndows-sdk/) and 
+00001790: 6368 6563 6b20 7468 6520 626f 7820 6044  check the box `D
+000017a0: 6562 7567 6769 6e67 2054 6f6f 6c73 2066  ebugging Tools f
+000017b0: 6f72 2057 696e 646f 7773 602e 0a31 2e20  or Windows`..1. 
+000017c0: 2a2a 4e61 7669 6761 7465 2074 6f20 7468  **Navigate to th
+000017d0: 6520 6073 7263 5c63 6861 7464 6267 6020  e `src\chatdbg` 
+000017e0: 6469 7265 6374 6f72 792a 2a3a 2060 6364  directory**: `cd
+000017f0: 2073 7263 5c63 6861 7464 6267 600a 312e   src\chatdbg`.1.
+00001800: 202a 2a49 6e73 7461 6c6c 206e 6565 6465   **Install neede
+00001810: 6420 6465 7065 6e64 656e 6369 6573 2a2a  d dependencies**
+00001820: 3a20 5275 6e60 7663 706b 6720 696e 7374  : Run`vcpkg inst
+00001830: 616c 6c60 0a31 2e20 2a2a 4275 696c 6420  all`.1. **Build 
+00001840: 7468 6520 6368 6174 6462 672e 646c 6c20  the chatdbg.dll 
+00001850: 6578 7465 6e73 696f 6e2a 2a3a 2052 756e  extension**: Run
+00001860: 606d 6b64 6972 2062 7569 6c64 2026 2063  `mkdir build & c
+00001870: 6420 6275 696c 6420 2620 636d 616b 6520  d build & cmake 
+00001880: 2e2e 2026 2063 6d61 6b65 202d 2d62 7569  .. & cmake --bui
+00001890: 6c64 202e 2026 2063 6420 2e2e 600a 0a2a  ld . & cd ..`..*
+000018a0: 2a55 7369 6e67 2043 6861 7444 4247 2a2a  *Using ChatDBG**
+000018b0: 3a0a 0a20 2a20 4c6f 6164 2069 6e74 6f20  :.. * Load into 
+000018c0: 5769 6e44 4247 583a 0a20 2020 2a20 5275  WinDBGX:.   * Ru
+000018d0: 6e20 6077 696e 6462 6778 2079 6f75 725f  n `windbgx your_
+000018e0: 6578 6563 7574 6162 6c65 5f68 6572 652e  executable_here.
+000018f0: 6578 6560 0a20 2020 2a20 436c 6963 6b20  exe`.   * Click 
+00001900: 7468 6520 6d65 6e75 2069 7465 6d73 2060  the menu items `
+00001910: 5669 6577 6020 2d3e 2060 436f 6d6d 616e  View` -> `Comman
+00001920: 6420 6272 6f77 7365 7260 0a20 2020 2a20  d browser`.   * 
+00001930: 5479 7065 2060 2e6c 6f61 6420 6465 6275  Type `.load debu
+00001940: 675c 6368 6174 6462 672e 646c 6c60 0a20  g\chatdbg.dll`. 
+00001950: 2a20 4166 7465 7220 7275 6e6e 696e 6720  * After running 
+00001960: 636f 6465 2061 6e64 2068 6974 7469 6e67  code and hitting
+00001970: 2061 6e20 6578 6365 7074 696f 6e20 2f20   an exception / 
+00001980: 7369 676e 616c 3a0a 2020 202a 2054 7970  signal:.   * Typ
+00001990: 6520 6021 7768 7960 2069 6e20 436f 6d6d  e `!why` in Comm
+000019a0: 616e 6420 6272 6f77 7365 720a 3c2f 6465  and browser.</de
+000019b0: 7461 696c 733e 0a0a 0a23 2320 5573 6167  tails>...## Usag
+000019c0: 650a 0a23 2323 2044 6562 7567 6769 6e67  e..### Debugging
+000019d0: 2050 7974 686f 6e0a 0a54 6f20 7573 6520   Python..To use 
+000019e0: 4368 6174 4442 4720 746f 2064 6562 7567  ChatDBG to debug
+000019f0: 2050 7974 686f 6e20 7072 6f67 7261 6d73   Python programs
+00001a00: 2c20 7369 6d70 6c79 2072 756e 2079 6f75  , simply run you
+00001a10: 7220 5079 7468 6f6e 2073 6372 6970 7420  r Python script 
+00001a20: 6173 2066 6f6c 6c6f 7773 3a0a 0a60 6060  as follows:..```
+00001a30: 6261 7368 0a63 6861 7464 6267 202d 6320  bash.chatdbg -c 
+00001a40: 636f 6e74 696e 7565 2079 6f75 7273 6372  continue yourscr
+00001a50: 6970 742e 7079 0a60 6060 0a0a 4368 6174  ipt.py.```..Chat
+00001a60: 4442 4720 6973 2061 6e20 6578 7465 6e73  DBG is an extens
+00001a70: 696f 6e20 6f66 2074 6865 2073 7461 6e64  ion of the stand
+00001a80: 6172 6420 5079 7468 6f6e 2064 6562 7567  ard Python debug
+00001a90: 6765 7220 6070 6462 602e 204c 696b 650a  ger `pdb`. Like.
+00001aa0: 6070 6462 602c 2077 6865 6e20 796f 7572  `pdb`, when your
+00001ab0: 2073 6372 6970 7420 656e 636f 756e 7465   script encounte
+00001ac0: 7273 2061 6e20 756e 6361 7567 6874 2065  rs an uncaught e
+00001ad0: 7863 6570 7469 6f6e 2c20 4368 6174 4442  xception, ChatDB
+00001ae0: 4720 7769 6c6c 0a65 6e74 6572 2070 6f73  G will.enter pos
+00001af0: 7420 6d6f 7274 656d 2064 6562 7567 6769  t mortem debuggi
+00001b00: 6e67 206d 6f64 652e 0a0a 556e 6c69 6b65  ng mode...Unlike
+00001b10: 206f 7468 6572 2064 6562 7567 6765 7273   other debuggers
+00001b20: 2c20 796f 7520 6361 6e20 7468 656e 2075  , you can then u
+00001b30: 7365 2074 6865 2060 7768 7960 2063 6f6d  se the `why` com
+00001b40: 6d61 6e64 2074 6f20 6173 6b0a 4368 6174  mand to ask.Chat
+00001b50: 4442 4720 7768 7920 796f 7572 2070 726f  DBG why your pro
+00001b60: 6772 616d 2066 6169 6c65 6420 616e 6420  gram failed and 
+00001b70: 6765 7420 6120 7375 6767 6573 7465 6420  get a suggested 
+00001b80: 6669 782e 2020 4166 7465 7220 7468 6520  fix.  After the 
+00001b90: 4c4c 4d20 7265 7370 6f6e 6473 2c0a 796f  LLM responds,.yo
+00001ba0: 7520 6d61 7920 6973 7375 6520 6164 6469  u may issue addi
+00001bb0: 7469 6f6e 616c 2064 6562 7567 6769 6e67  tional debugging
+00001bc0: 2063 6f6d 6d61 6e64 7320 6f72 2063 6f6e   commands or con
+00001bd0: 7469 6e75 6520 7468 6520 636f 6e76 6572  tinue the conver
+00001be0: 7361 7469 6f6e 2062 7920 656e 7465 7269  sation by enteri
+00001bf0: 6e67 0a61 6e79 206f 7468 6572 2074 6578  ng.any other tex
+00001c00: 742e 0a0a 2323 2323 2049 5079 7468 6f6e  t...#### IPython
+00001c10: 2061 6e64 204a 7570 7974 6572 2053 7570   and Jupyter Sup
+00001c20: 706f 7274 0a0a 546f 2075 7365 2043 6861  port..To use Cha
+00001c30: 7444 4247 2061 7320 7468 6520 6465 6661  tDBG as the defa
+00001c40: 756c 7420 6465 6275 6767 6572 2066 6f72  ult debugger for
+00001c50: 2049 5079 7468 6f6e 206f 7220 696e 7369   IPython or insi
+00001c60: 6465 204a 7570 7974 6572 204e 6f74 6562  de Jupyter Noteb
+00001c70: 6f6f 6b73 2c0a 6372 6561 7465 2061 2049  ooks,.create a I
+00001c80: 5079 7468 6f6e 2070 726f 6669 6c65 2061  Python profile a
+00001c90: 6e64 2074 6865 6e20 6164 6420 7468 6520  nd then add the 
+00001ca0: 6e65 6365 7373 6172 7920 6578 656e 7369  necessary exensi
+00001cb0: 6f6e 7320 6f6e 2073 7461 7274 7570 2e20  ons on startup. 
+00001cc0: 2028 4d6f 6469 6679 0a74 6865 7365 206c   (Modify.these l
+00001cd0: 696e 6573 2061 7320 6e65 6365 7373 6172  ines as necessar
+00001ce0: 7920 6966 2079 6f75 2061 6c72 6561 6479  y if you already
+00001cf0: 2068 6176 6520 6120 6375 7374 6f6d 697a   have a customiz
+00001d00: 6564 2070 726f 6669 6c65 2066 696c 652e  ed profile file.
+00001d10: 290a 0a60 6060 6261 7368 0a69 7079 7468  )..```bash.ipyth
+00001d20: 6f6e 2070 726f 6669 6c65 2063 7265 6174  on profile creat
+00001d30: 650a 6563 686f 2022 632e 496e 7465 7261  e.echo "c.Intera
+00001d40: 6374 6976 6553 6865 6c6c 4170 702e 6578  ctiveShellApp.ex
+00001d50: 7465 6e73 696f 6e73 203d 205b 2763 6861  tensions = ['cha
+00001d60: 7464 6267 2e63 6861 7464 6267 5f70 6462  tdbg.chatdbg_pdb
+00001d70: 272c 2027 6970 7966 6c6f 7727 5d22 203e  ', 'ipyflow']" >
+00001d80: 3e20 7e2f 2e69 7079 7468 6f6e 2f70 726f  > ~/.ipython/pro
+00001d90: 6669 6c65 5f64 6566 6175 6c74 2f69 7079  file_default/ipy
+00001da0: 7468 6f6e 5f63 6f6e 6669 672e 7079 0a60  thon_config.py.`
+00001db0: 6060 0a0a 4f6e 2074 6865 2063 6f6d 6d61  ``..On the comma
+00001dc0: 6e64 206c 696e 652c 2079 6f75 2063 616e  nd line, you can
+00001dd0: 2074 6865 6e20 7275 6e3a 0a0a 6060 6062   then run:..```b
+00001de0: 6173 680a 6970 7974 686f 6e20 2d2d 7064  ash.ipython --pd
+00001df0: 6220 796f 7572 7363 7269 7074 2e70 790a  b yourscript.py.
+00001e00: 6060 600a 0a49 6e73 6964 6520 4a75 7079  ```..Inside Jupy
+00001e10: 7465 722c 2072 756e 2079 6f75 7220 6e6f  ter, run your no
+00001e20: 7465 626f 6f6b 2077 6974 6820 7468 6520  tebook with the 
+00001e30: 5b69 7079 666c 6f77 206b 6572 6e65 6c5d  [ipyflow kernel]
+00001e40: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00001e50: 636f 6d2f 6970 7966 6c6f 772f 6970 7966  com/ipyflow/ipyf
+00001e60: 6c6f 7729 2061 6e64 2069 6e63 6c75 6465  low) and include
+00001e70: 2074 6869 7320 6c69 6e65 206d 6167 6963   this line magic
+00001e80: 2061 7420 7468 6520 746f 7020 6f66 2074   at the top of t
+00001e90: 6865 2066 696c 652e 0a0a 6060 600a 2570  he file...```.%p
+00001ea0: 6462 0a60 6060 0a0a 0a23 2323 2044 6562  db.```...### Deb
+00001eb0: 7567 6769 6e67 206e 6174 6976 6520 636f  ugging native co
+00001ec0: 6465 2028 432c 2043 2b2b 2c20 6f72 2052  de (C, C++, or R
+00001ed0: 7573 7420 7769 7468 203c 5454 3e6c 6c64  ust with <TT>lld
+00001ee0: 623c 2f54 543e 202f 203c 5454 3e67 6462  b</TT> / <TT>gdb
+00001ef0: 3c2f 5454 3e29 0a0a 546f 2075 7365 2043  </TT>)..To use C
+00001f00: 6861 7444 4247 2077 6974 6820 606c 6c64  hatDBG with `lld
+00001f10: 6260 206f 7220 6067 6462 602c 206a 7573  b` or `gdb`, jus
+00001f20: 7420 7275 6e20 6e61 7469 7665 2063 6f64  t run native cod
+00001f30: 6520 2863 6f6d 7069 6c65 6420 7769 7468  e (compiled with
+00001f40: 2060 2d67 6020 666f 7220 6465 6275 6767   `-g` for debugg
+00001f50: 696e 6720 7379 6d62 6f6c 7329 2077 6974  ing symbols) wit
+00001f60: 6820 796f 7572 2063 686f 6963 6520 6f66  h your choice of
+00001f70: 2064 6562 7567 6765 723b 2077 6865 6e20   debugger; when 
+00001f80: 6974 2063 7261 7368 6573 2c20 6173 6b20  it crashes, ask 
+00001f90: 6077 6879 602e 2054 6869 7320 616c 736f  `why`. This also
+00001fa0: 2077 6f72 6b73 2066 6f72 2070 6f73 7420   works for post 
+00001fb0: 6d6f 7274 656d 2064 6562 7567 6769 6e67  mortem debugging
+00001fc0: 2028 7768 656e 2079 6f75 206c 6f61 6420   (when you load 
+00001fd0: 6120 636f 7265 2077 6974 6820 7468 6520  a core with the 
+00001fe0: 602d 6360 206f 7074 696f 6e29 2e20 200a  `-c` option).  .
+00001ff0: 0a54 6865 206e 6174 6976 6520 6465 6275  .The native debu
+00002000: 6767 6572 7320 776f 726b 2073 6c69 6768  ggers work sligh
+00002010: 746c 7920 6469 6666 6572 656e 746c 7920  tly differently 
+00002020: 7468 616e 2050 6462 2e20 2041 6674 6572  than Pdb.  After
+00002030: 2074 6865 2064 6562 7567 6765 7220 7265   the debugger re
+00002040: 7370 6f6e 6473 2074 6f20 796f 7572 2071  sponds to your q
+00002050: 7565 7374 696f 6e2c 2079 6f75 2077 696c  uestion, you wil
+00002060: 6c20 656e 7465 7220 696e 746f 2043 6861  l enter into Cha
+00002070: 7444 4247 2773 2063 6f6d 6d61 6e64 206c  tDBG's command l
+00002080: 6f6f 702c 2061 7320 696e 6469 6361 7465  oop, as indicate
+00002090: 6420 6279 2074 6865 2060 2843 6861 7444  d by the `(ChatD
+000020a0: 4247 2063 6861 7474 696e 6729 6020 7072  BG chatting)` pr
+000020b0: 6f6d 7074 2e20 2059 6f75 206d 6179 2063  ompt.  You may c
+000020c0: 6f6e 7469 6e75 6520 6973 7375 696e 6720  ontinue issuing 
+000020d0: 6465 6275 6767 696e 6720 636f 6d6d 616e  debugging comman
+000020e0: 6473 2061 6e64 2079 6f75 206d 6179 2073  ds and you may s
+000020f0: 656e 6420 6164 6469 7469 6f6e 616c 206d  end additional m
+00002100: 6573 7361 6765 7320 746f 2074 6865 204c  essages to the L
+00002110: 4c4d 2062 7920 7374 6172 7469 6e67 2074  LM by starting t
+00002120: 686f 7365 206d 6573 7361 6765 7320 7769  hose messages wi
+00002130: 7468 2022 6368 6174 222e 2020 5768 656e  th "chat".  When
+00002140: 2079 6f75 2061 7265 2064 6f6e 652c 2074   you are done, t
+00002150: 7970 6520 6071 7569 7460 2074 6f20 7265  ype `quit` to re
+00002160: 7475 726e 2074 6f20 7468 6520 6465 6275  turn to the debu
+00002170: 6767 6572 2773 206d 6169 6e20 636f 6d6d  gger's main comm
+00002180: 616e 6420 6c6f 6f70 2e0a 0a3c 6465 7461  and loop...<deta
+00002190: 696c 733e 0a3c 7375 6d6d 6172 793e 0a3c  ils>.<summary>.<
+000021a0: 423e 4465 6275 6767 696e 6720 5275 7374  B>Debugging Rust
+000021b0: 2070 726f 6772 616d 733c 2f42 3e0a 3c2f   programs</B>.</
+000021c0: 7375 6d6d 6172 793e 0a0a 546f 2075 7365  summary>..To use
+000021d0: 2043 6861 7444 4247 2077 6974 6820 5275   ChatDBG with Ru
+000021e0: 7374 2c20 796f 7520 6e65 6564 2074 6f20  st, you need to 
+000021f0: 646f 2074 776f 2073 7465 7073 3a20 6d6f  do two steps: mo
+00002200: 6469 6679 2079 6f75 720a 6043 6172 676f  dify your.`Cargo
+00002210: 2e74 6f6d 6c60 2066 696c 6520 616e 6420  .toml` file and 
+00002220: 6164 6420 6f6e 6520 6c69 6e65 2074 6f20  add one line to 
+00002230: 796f 7572 2073 6f75 7263 6520 7072 6f67  your source prog
+00002240: 7261 6d2e 0a0a 312e 2041 6464 2074 6869  ram...1. Add thi
+00002250: 7320 746f 2079 6f75 7220 6043 6172 676f  s to your `Cargo
+00002260: 2e74 6f6d 6c60 2066 696c 653a 0a0a 6060  .toml` file:..``
+00002270: 6074 6f6d 6c0a 5b64 6570 656e 6465 6e63  `toml.[dependenc
+00002280: 6965 735d 0a63 6861 7464 6267 203d 2022  ies].chatdbg = "
+00002290: 302e 312e 3322 0a0a 5b70 726f 6669 6c65  0.1.3"..[profile
+000022a0: 2e64 6576 5d0a 7061 6e69 6320 3d20 2261  .dev].panic = "a
+000022b0: 626f 7274 220a 0a5b 7072 6f66 696c 652e  bort"..[profile.
+000022c0: 7265 6c65 6173 655d 0a70 616e 6963 203d  release].panic =
+000022d0: 2022 6162 6f72 7422 0a60 6060 0a0a 322e   "abort".```..2.
+000022e0: 2049 6e20 796f 7572 2070 726f 6772 616d   In your program
+000022f0: 2c20 6170 706c 7920 7468 6520 6023 5b63  , apply the `#[c
+00002300: 6861 7464 6267 3a3a 6d61 696e 5d60 2061  hatdbg::main]` a
+00002310: 7474 7269 6275 7465 2074 6f20 796f 7572  ttribute to your
+00002320: 2060 6d61 696e 600a 6675 6e63 7469 6f6e   `main`.function
+00002330: 3a0a 0a60 6060 7275 7374 0a23 5b63 6861  :..```rust.#[cha
+00002340: 7464 6267 3a3a 6d61 696e 5d0a 666e 206d  tdbg::main].fn m
+00002350: 6169 6e28 2920 7b0a 6060 600a 0a4e 6f77  ain() {.```..Now
+00002360: 2079 6f75 2063 616e 2064 6562 7567 2079   you can debug y
+00002370: 6f75 7220 5275 7374 2063 6f64 6520 7769  our Rust code wi
+00002380: 7468 2060 6764 6260 206f 7220 606c 6c64  th `gdb` or `lld
+00002390: 6260 2e0a 0a3c 2f64 6574 6169 6c73 3e0a  b`...</details>.
+000023a0: 0a23 2323 2045 7861 6d70 6c65 730a 0a3c  .### Examples..<
+000023b0: 6465 7461 696c 733e 0a3c 7375 6d6d 6172  details>.<summar
+000023c0: 793e 0a3c 423e 4368 6174 4442 4720 6578  y>.<B>ChatDBG ex
+000023d0: 616d 706c 6520 696e 203c 5454 3e6c 6c64  ample in <TT>lld
+000023e0: 623c 2f54 543e 3c2f 423e 0a3c 2f73 756d  b</TT></B>.</sum
+000023f0: 6d61 7279 3e0a 0a60 6060 6764 620a 2843  mary>..```gdb.(C
+00002400: 6861 7444 4247 206c 6c64 6229 2072 756e  hatDBG lldb) run
+00002410: 0a50 726f 6365 7373 2038 3534 3934 206c  .Process 85494 l
+00002420: 6175 6e63 6865 643a 2027 2f55 7365 7273  aunched: '/Users
+00002430: 2f65 6d65 7279 2f67 6974 2f43 6861 7444  /emery/git/ChatD
+00002440: 4247 2f74 6573 742f 612e 6f75 7427 2028  BG/test/a.out' (
+00002450: 6172 6d36 3429 0a54 4553 5420 310a 5445  arm64).TEST 1.TE
+00002460: 5354 202d 3432 3237 3631 3238 380a 5445  ST -422761288.TE
+00002470: 5354 2030 0a54 4553 5420 300a 5445 5354  ST 0.TEST 0.TEST
+00002480: 2030 0a54 4553 5420 300a 5445 5354 2030   0.TEST 0.TEST 0
+00002490: 0a54 4553 5420 300a 5072 6f63 6573 7320  .TEST 0.Process 
+000024a0: 3835 3439 3420 7374 6f70 7065 640a 2a20  85494 stopped.* 
+000024b0: 7468 7265 6164 2023 312c 2071 7565 7565  thread #1, queue
+000024c0: 203d 2027 636f 6d2e 6170 706c 652e 6d61   = 'com.apple.ma
+000024d0: 696e 2d74 6872 6561 6427 2c20 7374 6f70  in-thread', stop
+000024e0: 2072 6561 736f 6e20 3d20 4558 435f 4241   reason = EXC_BA
+000024f0: 445f 4143 4345 5353 2028 636f 6465 3d31  D_ACCESS (code=1
+00002500: 2c20 6164 6472 6573 733d 3078 3130 3030  , address=0x1000
+00002510: 3536 3230 3029 0a20 2020 2066 7261 6d65  56200).    frame
+00002520: 2023 303a 2030 7830 3030 3030 3030 3130   #0: 0x000000010
+00002530: 3030 3032 6636 3420 612e 6f75 7460 666f  0002f64 a.out`fo
+00002540: 6f28 6e3d 382c 2062 3d31 2920 6174 2074  o(n=8, b=1) at t
+00002550: 6573 742e 6370 703a 373a 3232 0a20 2020  est.cpp:7:22.   
+00002560: 3420 2020 2020 696e 7420 785b 5d20 3d20  4     int x[] = 
+00002570: 7b20 312c 2032 2c20 332c 2034 2c20 3520  { 1, 2, 3, 4, 5 
+00002580: 7d3b 0a20 2020 3520 2020 2020 0a20 2020  };.   5     .   
+00002590: 3620 2020 2020 766f 6964 2066 6f6f 2869  6     void foo(i
+000025a0: 6e74 206e 2c20 666c 6f61 7420 6229 207b  nt n, float b) {
+000025b0: 0a2d 3e20 3720 2020 2020 2020 636f 7574  .-> 7       cout
+000025c0: 203c 3c20 2254 4553 5420 2220 3c3c 2078   << "TEST " << x
+000025d0: 5b6e 202a 2031 3030 3030 5d20 3c3c 2065  [n * 10000] << e
+000025e0: 6e64 6c3b 0a20 2020 3820 2020 2020 7d0a  ndl;.   8     }.
+000025f0: 2020 2039 2020 2020 200a 2020 2031 3020     9     .   10 
+00002600: 2020 2069 6e74 206d 6169 6e28 290a 5461     int main().Ta
+00002610: 7267 6574 2030 3a20 2861 2e6f 7574 2920  rget 0: (a.out) 
+00002620: 7374 6f70 7065 642e 0a60 6060 0a0a 4173  stopped..```..As
+00002630: 6b20 6077 6879 6020 746f 2068 6176 6520  k `why` to have 
+00002640: 4368 6174 4442 4720 7072 6f76 6964 6520  ChatDBG provide 
+00002650: 6120 6865 6c70 6675 6c20 6578 706c 616e  a helpful explan
+00002660: 6174 696f 6e20 7768 7920 7468 6973 2070  ation why this p
+00002670: 726f 6772 616d 2066 6169 6c65 642c 2061  rogram failed, a
+00002680: 6e64 2073 7567 6765 7374 2061 2066 6978  nd suggest a fix
+00002690: 3a0a 0a0a 6060 6067 6462 0a28 4368 6174  :...```gdb.(Chat
+000026a0: 4442 4720 6c6c 6462 2920 7768 790a 5468  DBG lldb) why.Th
+000026b0: 6520 726f 6f74 2063 6175 7365 206f 6620  e root cause of 
+000026c0: 7468 6973 2065 7272 6f72 2069 7320 6163  this error is ac
+000026d0: 6365 7373 696e 6720 616e 2069 6e64 6578  cessing an index
+000026e0: 206f 6620 7468 6520 6172 7261 7920 6078   of the array `x
+000026f0: 600a 7468 6174 2069 7320 6f75 7420 6f66  `.that is out of
+00002700: 2062 6f75 6e64 732e 2049 6e20 6066 6f6f   bounds. In `foo
+00002710: 2829 602c 2074 6865 2069 6e64 6578 2069  ()`, the index i
+00002720: 7320 6361 6c63 756c 6174 6564 2061 7320  s calculated as 
+00002730: 606e 202a 0a31 3030 3030 602c 2077 6869  `n *.10000`, whi
+00002740: 6368 2063 616e 2062 6520 6d75 6368 206c  ch can be much l
+00002750: 6172 6765 7220 7468 616e 2074 6865 2073  arger than the s
+00002760: 697a 6520 6f66 2074 6865 2061 7272 6179  ize of the array
+00002770: 2060 7860 2028 7768 6963 680a 6973 206f   `x` (which.is o
+00002780: 6e6c 7920 3520 656c 656d 656e 7473 292e  nly 5 elements).
+00002790: 2049 6e20 7468 6520 6769 7665 6e20 7472   In the given tr
+000027a0: 6163 652c 2074 6865 2070 726f 6772 616d  ace, the program
+000027b0: 2069 7320 7472 7969 6e67 2074 6f0a 6163   is trying to.ac
+000027c0: 6365 7373 2074 6865 206d 656d 6f72 7920  cess the memory 
+000027d0: 6164 6472 6573 7320 6030 7831 3030 3035  address `0x10005
+000027e0: 3632 3030 602c 2077 6869 6368 2069 7320  6200`, which is 
+000027f0: 6f75 7473 6964 6520 6f66 2074 6865 2072  outside of the r
+00002800: 616e 6765 0a6f 6620 616c 6c6f 6361 7465  ange.of allocate
+00002810: 6420 6d65 6d6f 7279 2066 6f72 2074 6865  d memory for the
+00002820: 2061 7272 6179 2060 7860 2e0a 0a54 6f20   array `x`...To 
+00002830: 6669 7820 7468 6973 2065 7272 6f72 2c20  fix this error, 
+00002840: 7765 206e 6565 6420 746f 2065 6e73 7572  we need to ensur
+00002850: 6520 7468 6174 2074 6865 2069 6e64 6578  e that the index
+00002860: 2069 7320 7769 7468 696e 2074 6865 0a62   is within the.b
+00002870: 6f75 6e64 7320 6f66 2074 6865 2061 7272  ounds of the arr
+00002880: 6179 2e20 4f6e 6520 7761 7920 746f 2064  ay. One way to d
+00002890: 6f20 7468 6973 2069 7320 746f 2063 6865  o this is to che
+000028a0: 636b 2074 6865 2076 616c 7565 206f 6620  ck the value of 
+000028b0: 606e 600a 6265 666f 7265 2063 616c 6375  `n`.before calcu
+000028c0: 6c61 7469 6e67 2074 6865 2069 6e64 6578  lating the index
+000028d0: 2c20 616e 6420 656e 7375 7265 2074 6861  , and ensure tha
+000028e0: 7420 6974 2069 7320 6c65 7373 2074 6861  t it is less tha
+000028f0: 6e20 7468 6520 7369 7a65 0a6f 6620 7468  n the size.of th
+00002900: 6520 6172 7261 7920 6469 7669 6465 6420  e array divided 
+00002910: 6279 2074 6865 2073 697a 6520 6f66 2074  by the size of t
+00002920: 6865 2065 6c65 6d65 6e74 2e20 466f 7220  he element. For 
+00002930: 6578 616d 706c 652c 2077 6520 6361 6e0a  example, we can.
+00002940: 6d6f 6469 6679 2060 666f 6f28 2960 2061  modify `foo()` a
+00002950: 7320 666f 6c6c 6f77 733a 0a0a 2020 2020  s follows:..    
+00002960: 6060 600a 2020 2020 766f 6964 2066 6f6f  ```.    void foo
+00002970: 2869 6e74 206e 2c20 666c 6f61 7420 6229  (int n, float b)
+00002980: 207b 0a20 2020 2020 2069 6620 286e 203c   {.      if (n <
+00002990: 2030 207c 7c20 6e20 3e3d 2073 697a 656f   0 || n >= sizeo
+000029a0: 6628 7829 2f73 697a 656f 6628 785b 305d  f(x)/sizeof(x[0]
+000029b0: 2929 207b 0a20 2020 2020 2020 2063 6f75  )) {.        cou
+000029c0: 7420 3c3c 2022 4552 524f 523a 2049 6e76  t << "ERROR: Inv
+000029d0: 616c 6964 2069 6e64 6578 2220 3c3c 2065  alid index" << e
+000029e0: 6e64 6c3b 0a20 2020 2020 2020 2072 6574  ndl;.        ret
+000029f0: 7572 6e3b 0a20 2020 2020 207d 0a20 2020  urn;.      }.   
+00002a00: 2020 2063 6f75 7420 3c3c 2022 5445 5354     cout << "TEST
+00002a10: 2022 203c 3c20 785b 6e5d 203c 3c20 656e   " << x[n] << en
+00002a20: 646c 3b0a 2020 2020 7d0a 2020 2020 6060  dl;.    }.    ``
+00002a30: 600a 0a54 6869 7320 636f 6465 2063 6865  `..This code che
+00002a40: 636b 7320 6966 2060 6e60 2069 7320 7769  cks if `n` is wi
+00002a50: 7468 696e 2074 6865 2076 616c 6964 2072  thin the valid r
+00002a60: 616e 6765 2c20 616e 6420 7072 696e 7473  ange, and prints
+00002a70: 2061 6e20 6572 726f 720a 6d65 7373 6167   an error.messag
+00002a80: 6520 6966 2069 7420 6973 206e 6f74 2e20  e if it is not. 
+00002a90: 4966 2060 6e60 2069 7320 7769 7468 696e  If `n` is within
+00002aa0: 2074 6865 2072 616e 6765 2c20 7468 6520   the range, the 
+00002ab0: 6675 6e63 7469 6f6e 2070 7269 6e74 730a  function prints.
+00002ac0: 7468 6520 7661 6c75 6520 6f66 2074 6865  the value of the
+00002ad0: 2065 6c65 6d65 6e74 2061 7420 696e 6465   element at inde
+00002ae0: 7820 606e 6020 6f66 2060 7860 2e20 5769  x `n` of `x`. Wi
+00002af0: 7468 2074 6869 7320 6d6f 6469 6669 6361  th this modifica
+00002b00: 7469 6f6e 2c0a 7468 6520 7072 6f67 7261  tion,.the progra
+00002b10: 6d20 7769 6c6c 2061 766f 6964 2061 6363  m will avoid acc
+00002b20: 6573 7369 6e67 206d 656d 6f72 7920 6f75  essing memory ou
+00002b30: 7473 6964 6520 7468 6520 626f 756e 6473  tside the bounds
+00002b40: 206f 6620 7468 650a 6172 7261 792c 2061   of the.array, a
+00002b50: 6e64 2077 696c 6c20 7072 696e 7420 7468  nd will print th
+00002b60: 6520 6578 7065 6374 6564 206f 7574 7075  e expected outpu
+00002b70: 7420 666f 7220 7661 6c69 6420 696e 6469  t for valid indi
+00002b80: 6365 732e 0a60 6060 0a3c 2f64 6574 6169  ces..```.</detai
+00002b90: 6c73 3e0a 0a3c 6465 7461 696c 733e 0a3c  ls>..<details>.<
+00002ba0: 7375 6d6d 6172 793e 0a3c 423e 4368 6174  summary>.<B>Chat
+00002bb0: 4442 4720 6578 616d 706c 6520 696e 2050  DBG example in P
+00002bc0: 7974 686f 6e20 283c 5454 3e70 6462 3c2f  ython (<TT>pdb</
+00002bd0: 5454 3e29 3c2f 423e 0a3c 2f73 756d 6d61  TT>)</B>.</summa
+00002be0: 7279 3e0a 0a60 6060 7079 7468 6f6e 0a54  ry>..```python.T
+00002bf0: 7261 6365 6261 636b 2028 6d6f 7374 2072  raceback (most r
+00002c00: 6563 656e 7420 6361 6c6c 206c 6173 7429  ecent call last)
+00002c10: 3a0a 2020 4669 6c65 2022 796f 7572 7363  :.  File "yoursc
+00002c20: 7269 7074 2e70 7922 2c20 6c69 6e65 2039  ript.py", line 9
+00002c30: 2c20 696e 203c 6d6f 6475 6c65 3e0a 2020  , in <module>.  
+00002c40: 2020 7072 696e 7428 7472 796d 6528 3130    print(tryme(10
+00002c50: 3029 290a 2020 4669 6c65 2022 796f 7572  0)).  File "your
+00002c60: 7363 7269 7074 2e70 7922 2c20 6c69 6e65  script.py", line
+00002c70: 2034 2c20 696e 2074 7279 6d65 0a20 2020   4, in tryme.   
+00002c80: 2069 6620 7820 2f20 6920 3e20 323a 0a5a   if x / i > 2:.Z
+00002c90: 6572 6f44 6976 6973 696f 6e45 7272 6f72  eroDivisionError
+00002ca0: 3a20 6469 7669 7369 6f6e 2062 7920 7a65  : division by ze
+00002cb0: 726f 0a55 6e63 6175 6768 7420 6578 6365  ro.Uncaught exce
+00002cc0: 7074 696f 6e2e 2045 6e74 6572 696e 6720  ption. Entering 
+00002cd0: 706f 7374 206d 6f72 7465 6d20 6465 6275  post mortem debu
+00002ce0: 6767 696e 670a 5275 6e6e 696e 6720 2763  gging.Running 'c
+00002cf0: 6f6e 7427 206f 7220 2773 7465 7027 2077  ont' or 'step' w
+00002d00: 696c 6c20 7265 7374 6172 7420 7468 6520  ill restart the 
+00002d10: 7072 6f67 7261 6d0a 3e20 796f 7572 7363  program.> yoursc
+00002d20: 7269 7074 2e70 7928 3429 7472 796d 6528  ript.py(4)tryme(
+00002d30: 290a 2d3e 2069 6620 7820 2f20 6920 3e20  ).-> if x / i > 
+00002d40: 323a 0a60 6060 0a0a 4173 6b20 6077 6879  2:.```..Ask `why
+00002d50: 6020 746f 2068 6176 6520 4368 6174 4442  ` to have ChatDB
+00002d60: 4720 7072 6f76 6964 6520 6120 6865 6c70  G provide a help
+00002d70: 6675 6c20 6578 706c 616e 6174 696f 6e20  ful explanation 
+00002d80: 7768 7920 7468 6973 2070 726f 6772 616d  why this program
+00002d90: 2066 6169 6c65 642c 2061 6e64 2073 7567   failed, and sug
+00002da0: 6765 7374 2061 2066 6978 3a0a 0a60 6060  gest a fix:..```
+00002db0: 7079 7468 6f6e 0a28 4368 6174 4442 4720  python.(ChatDBG 
+00002dc0: 5064 6229 2077 6879 0a54 6865 2072 6f6f  Pdb) why.The roo
+00002dd0: 7420 6361 7573 6520 6f66 2074 6865 2065  t cause of the e
+00002de0: 7272 6f72 2069 7320 7468 6174 2074 6865  rror is that the
+00002df0: 2063 6f64 6520 6973 2061 7474 656d 7074   code is attempt
+00002e00: 696e 6720 746f 0a64 6976 6964 6520 6279  ing to.divide by
+00002e10: 207a 6572 6f20 696e 2074 6865 206c 696e   zero in the lin
+00002e20: 6520 2269 6620 7820 2f20 6920 3e20 3222  e "if x / i > 2"
+00002e30: 2e20 4173 2069 2072 616e 6765 7320 6672  . As i ranges fr
+00002e40: 6f6d 2030 2074 6f20 3939 2c0a 6974 2077  om 0 to 99,.it w
+00002e50: 696c 6c20 6576 656e 7475 616c 6c79 2072  ill eventually r
+00002e60: 6561 6368 2074 6865 2076 616c 7565 206f  each the value o
+00002e70: 6620 302c 2063 6175 7369 6e67 2061 205a  f 0, causing a Z
+00002e80: 6572 6f44 6976 6973 696f 6e45 7272 6f72  eroDivisionError
+00002e90: 2e0a 0a41 2070 6f73 7369 626c 6520 6669  ...A possible fi
+00002ea0: 7820 666f 7220 7468 6973 2077 6f75 6c64  x for this would
+00002eb0: 2062 6520 746f 2061 6464 2061 2063 6865   be to add a che
+00002ec0: 636b 2066 6f72 2069 2062 6569 6e67 2065  ck for i being e
+00002ed0: 7175 616c 2074 6f0a 7a65 726f 2062 6566  qual to.zero bef
+00002ee0: 6f72 6520 7065 7266 6f72 6d69 6e67 2074  ore performing t
+00002ef0: 6865 2064 6976 6973 696f 6e2e 2054 6869  he division. Thi
+00002f00: 7320 636f 756c 6420 6265 2064 6f6e 6520  s could be done 
+00002f10: 6279 2061 6464 696e 6720 616e 0a61 6464  by adding an.add
+00002f20: 6974 696f 6e61 6c20 636f 6e64 6974 696f  itional conditio
+00002f30: 6e61 6c20 7374 6174 656d 656e 742c 2073  nal statement, s
+00002f40: 7563 6820 6173 2022 6966 2069 203d 3d20  uch as "if i == 
+00002f50: 303a 2063 6f6e 7469 6e75 6522 2c20 746f  0: continue", to
+00002f60: 0a73 6b69 7020 6f76 6572 2074 6865 2069  .skip over the i
+00002f70: 7465 7261 7469 6f6e 2077 6865 6e20 6920  teration when i 
+00002f80: 6973 207a 6572 6f2e 2054 6865 2075 7064  is zero. The upd
+00002f90: 6174 6564 2063 6f64 6520 776f 756c 6420  ated code would 
+00002fa0: 6c6f 6f6b 0a6c 696b 6520 7468 6973 3a0a  look.like this:.
+00002fb0: 0a64 6566 2074 7279 6d65 2878 293a 0a20  .def tryme(x):. 
+00002fc0: 2020 2063 6f75 6e74 203d 2030 0a20 2020     count = 0.   
+00002fd0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+00002fe0: 3130 3029 3a0a 2020 2020 2020 2020 6966  100):.        if
+00002ff0: 2069 203d 3d20 303a 0a20 2020 2020 2020   i == 0:.       
+00003000: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
+00003010: 2020 2020 2020 6966 2078 202f 2069 203e        if x / i >
+00003020: 2032 3a0a 2020 2020 2020 2020 2020 2020   2:.            
+00003030: 636f 756e 7420 2b3d 2031 0a20 2020 2072  count += 1.    r
+00003040: 6574 7572 6e20 636f 756e 740a 0a69 6620  eturn count..if 
+00003050: 5f5f 6e61 6d65 5f5f 203d 3d20 275f 5f6d  __name__ == '__m
+00003060: 6169 6e5f 5f27 3a0a 2020 2020 7072 696e  ain__':.    prin
+00003070: 7428 7472 796d 6528 3130 3029 290a 6060  t(tryme(100)).``
+00003080: 600a 0a3c 2f64 6574 6169 6c73 3e0a 0a    `..</details>..
```

