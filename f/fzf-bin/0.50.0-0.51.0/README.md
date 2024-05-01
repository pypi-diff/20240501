# Comparing `tmp/fzf_bin-0.50.0.tar.gz` & `tmp/fzf_bin-0.51.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fzf_bin-0.50.0.tar", last modified: Mon Apr 15 15:21:04 2024, max compression
+gzip compressed data, was "fzf_bin-0.51.0.tar", last modified: Wed May  1 07:20:12 2024, max compression
```

## Comparing `fzf_bin-0.50.0.tar` & `fzf_bin-0.51.0.tar`

### file list

```diff
@@ -1,116 +1,116 @@
--rw-r--r--   0        0        0     1074 2024-04-15 15:19:48.541748 fzf_bin-0.50.0/LICENSE
--rw-r--r--   0        0        0      469 2024-04-15 15:19:48.541748 fzf_bin-0.50.0/README.md
--rw-r--r--   0        0        0       35 2024-04-15 15:19:49.485752 fzf_bin-0.50.0/fzf/.git
--rw-r--r--   0        0        0       17 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/.github/FUNDING.yml
--rw-r--r--   0        0        0     1162 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/.github/ISSUE_TEMPLATE/issue_template.yml
--rw-r--r--   0        0        0      209 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/.github/dependabot.yml
--rw-r--r--   0        0        0     1111 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      296 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/.github/workflows/depsreview.yaml
--rw-r--r--   0        0        0     1119 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/.github/workflows/linux.yml
--rw-r--r--   0        0        0     1001 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/.github/workflows/macos.yml
--rw-r--r--   0        0        0      555 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/.github/workflows/sponsors.yml
--rw-r--r--   0        0        0      193 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/.github/workflows/typos.yml
--rw-r--r--   0        0        0      382 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/.github/workflows/winget.yml
--rw-r--r--   0        0        0      104 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/.gitignore
--rw-r--r--   0        0        0     2431 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/.goreleaser.yml
--rw-r--r--   0        0        0      578 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/.rubocop.yml
--rw-r--r--   0        0        0       15 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/.tool-versions
--rw-r--r--   0        0        0    28068 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/ADVANCED.md
--rw-r--r--   0        0        0     1718 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/BUILD.md
--rw-r--r--   0        0        0    74695 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/CHANGELOG.md
--rw-r--r--   0        0        0      509 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/Dockerfile
--rw-r--r--   0        0        0     1085 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/LICENSE
--rw-r--r--   0        0        0     5275 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/Makefile
--rw-r--r--   0        0        0    17711 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/README-VIM.md
--rw-r--r--   0        0        0    35715 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/README.md
--rwxr-xr-x   0        0        0     2419 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/bin/fzf-preview.sh
--rwxr-xr-x   0        0        0     7079 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/bin/fzf-tmux
--rw-r--r--   0        0        0    21398 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/doc/fzf.txt
--rw-r--r--   0        0        0      496 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/go.mod
--rw-r--r--   0        0        0     5203 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/go.sum
--rwxr-xr-x   0        0        0    10184 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/install
--rw-r--r--   0        0        0     1881 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/install.ps1
--rw-r--r--   0        0        0     1159 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/main.go
--rw-r--r--   0        0        0     3630 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/main_test.go
--rw-r--r--   0        0        0     1992 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/man/man1/fzf-tmux.1
--rw-r--r--   0        0        0    50569 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/man/man1/fzf.1
--rw-r--r--   0        0        0    32550 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/plugin/fzf.vim
--rw-r--r--   0        0        0    16179 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/shell/completion.bash
--rw-r--r--   0        0        0    12038 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/shell/completion.zsh
--rw-r--r--   0        0        0     5358 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/shell/key-bindings.bash
--rw-r--r--   0        0        0     5602 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/shell/key-bindings.fish
--rw-r--r--   0        0        0     3880 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/shell/key-bindings.zsh
--rw-r--r--   0        0        0     1085 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/src/LICENSE
--rw-r--r--   0        0        0     5422 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/src/actiontype_string.go
--rw-r--r--   0        0        0    26654 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/src/algo/algo.go
--rw-r--r--   0        0        0     8883 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/src/algo/algo_test.go
--rw-r--r--   0        0        0    21779 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/algo/normalize.go
--rw-r--r--   0        0        0     9960 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/ansi.go
--rw-r--r--   0        0        0    11138 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/ansi_test.go
--rw-r--r--   0        0        0     1619 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/cache.go
--rw-r--r--   0        0        0      859 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/cache_test.go
--rw-r--r--   0        0        0     1806 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/chunklist.go
--rw-r--r--   0        0        0     1862 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/chunklist_test.go
--rw-r--r--   0        0        0     1704 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/constants.go
--rw-r--r--   0        0        0    10292 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/core.go
--rw-r--r--   0        0        0     2071 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/history.go
--rw-r--r--   0        0        0     1507 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/history_test.go
--rw-r--r--   0        0        0      957 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/item.go
--rw-r--r--   0        0        0      484 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/item_test.go
--rw-r--r--   0        0        0     5411 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/matcher.go
--rw-r--r--   0        0        0     3302 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/merger.go
--rw-r--r--   0        0        0     1989 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/merger_test.go
--rw-r--r--   0        0        0    65745 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/options.go
--rw-r--r--   0        0        0      307 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/options_no_pprof.go
--rw-r--r--   0        0        0     1628 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/options_pprof.go
--rw-r--r--   0        0        0     2069 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/options_pprof_test.go
--rw-r--r--   0        0        0    14787 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/options_test.go
--rw-r--r--   0        0        0    10565 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/pattern.go
--rw-r--r--   0        0        0     8060 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/pattern_test.go
--rw-r--r--   0        0        0      131 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/protector/protector.go
--rw-r--r--   0        0        0      217 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/protector/protector_openbsd.go
--rw-r--r--   0        0        0     5847 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/reader.go
--rw-r--r--   0        0        0     1279 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/reader_test.go
--rw-r--r--   0        0        0     5998 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/result.go
--rw-r--r--   0        0        0      338 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/result_others.go
--rw-r--r--   0        0        0     6064 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/result_test.go
--rw-r--r--   0        0        0      364 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/result_x86.go
--rw-r--r--   0        0        0     6297 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/server.go
--rw-r--r--   0        0        0   114080 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/terminal.go
--rw-r--r--   0        0        0    27879 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/terminal_test.go
--rw-r--r--   0        0        0     1008 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/terminal_unix.go
--rw-r--r--   0        0        0     1088 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/terminal_windows.go
--rw-r--r--   0        0        0     5651 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/tokenizer.go
--rw-r--r--   0        0        0     2858 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/tokenizer_test.go
--rw-r--r--   0        0        0     1794 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/tui/dummy.go
--rw-r--r--   0        0        0     3467 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/tui/eventtype_string.go
--rw-r--r--   0        0        0    24618 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/tui/light.go
--rw-r--r--   0        0        0     2510 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/tui/light_unix.go
--rw-r--r--   0        0        0     4777 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/tui/light_windows.go
--rw-r--r--   0        0        0    18570 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/tui/tcell.go
--rw-r--r--   0        0        0    17392 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/tui/tcell_test.go
--rw-r--r--   0        0        0      908 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/tui/ttyname_unix.go
--rw-r--r--   0        0        0      164 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/tui/ttyname_windows.go
--rw-r--r--   0        0        0    21117 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/tui/tui.go
--rw-r--r--   0        0        0      399 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/tui/tui_test.go
--rw-r--r--   0        0        0      850 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/util/atexit.go
--rw-r--r--   0        0        0      452 2024-04-15 15:19:49.505752 fzf_bin-0.50.0/fzf/src/util/atexit_test.go
--rw-r--r--   0        0        0      748 2024-04-15 15:19:49.505752 fzf_bin-0.50.0/fzf/src/util/atomicbool.go
--rw-r--r--   0        0        0      301 2024-04-15 15:19:49.505752 fzf_bin-0.50.0/fzf/src/util/atomicbool_test.go
--rw-r--r--   0        0        0     4308 2024-04-15 15:19:49.505752 fzf_bin-0.50.0/fzf/src/util/chars.go
--rw-r--r--   0        0        0      981 2024-04-15 15:19:49.505752 fzf_bin-0.50.0/fzf/src/util/chars_test.go
--rw-r--r--   0        0        0     1976 2024-04-15 15:19:49.505752 fzf_bin-0.50.0/fzf/src/util/eventbox.go
--rw-r--r--   0        0        0      899 2024-04-15 15:19:49.505752 fzf_bin-0.50.0/fzf/src/util/eventbox_test.go
--rw-r--r--   0        0        0      185 2024-04-15 15:19:49.505752 fzf_bin-0.50.0/fzf/src/util/slab.go
--rw-r--r--   0        0        0     3733 2024-04-15 15:19:49.505752 fzf_bin-0.50.0/fzf/src/util/util.go
--rw-r--r--   0        0        0     4194 2024-04-15 15:19:49.505752 fzf_bin-0.50.0/fzf/src/util/util_test.go
--rw-r--r--   0        0        0     1199 2024-04-15 15:19:49.505752 fzf_bin-0.50.0/fzf/src/util/util_unix.go
--rw-r--r--   0        0        0     2219 2024-04-15 15:19:49.505752 fzf_bin-0.50.0/fzf/src/util/util_windows.go
--rw-r--r--   0        0        0     5860 2024-04-15 15:19:49.505752 fzf_bin-0.50.0/fzf/test/fzf.vader
--rwxr-xr-x   0        0        0   126533 2024-04-15 15:19:49.505752 fzf_bin-0.50.0/fzf/test/test_go.rb
--rw-r--r--   0        0        0      216 2024-04-15 15:19:49.505752 fzf_bin-0.50.0/fzf/typos.toml
--rwxr-xr-x   0        0        0     2520 2024-04-15 15:19:49.505752 fzf_bin-0.50.0/fzf/uninstall
--rw-r--r--   0        0        0        0 2024-04-15 15:19:48.541748 fzf_bin-0.50.0/fzf_bin/__init__.py
--rw-r--r--   0        0        0     1392 2024-04-15 15:19:48.541748 fzf_bin-0.50.0/pdm_build.py
--rw-r--r--   0        0        0     1073 2024-04-15 15:21:04.710130 fzf_bin-0.50.0/pyproject.toml
--rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 fzf_bin-0.50.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-01 07:18:56.584656 fzf_bin-0.51.0/LICENSE
+-rw-r--r--   0        0        0      469 2024-05-01 07:18:56.584656 fzf_bin-0.51.0/README.md
+-rw-r--r--   0        0        0       35 2024-05-01 07:18:57.928645 fzf_bin-0.51.0/fzf/.git
+-rw-r--r--   0        0        0       17 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1162 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/.github/ISSUE_TEMPLATE/issue_template.yml
+-rw-r--r--   0        0        0      209 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/.github/dependabot.yml
+-rw-r--r--   0        0        0     1111 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      296 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/.github/workflows/depsreview.yaml
+-rw-r--r--   0        0        0     1119 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/.github/workflows/linux.yml
+-rw-r--r--   0        0        0     1001 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/.github/workflows/macos.yml
+-rw-r--r--   0        0        0      555 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/.github/workflows/sponsors.yml
+-rw-r--r--   0        0        0      194 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/.github/workflows/typos.yml
+-rw-r--r--   0        0        0      382 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/.github/workflows/winget.yml
+-rw-r--r--   0        0        0      104 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/.gitignore
+-rw-r--r--   0        0        0     2512 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/.goreleaser.yml
+-rw-r--r--   0        0        0      578 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/.rubocop.yml
+-rw-r--r--   0        0        0       15 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/.tool-versions
+-rw-r--r--   0        0        0    28068 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/ADVANCED.md
+-rw-r--r--   0        0        0     1718 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/BUILD.md
+-rw-r--r--   0        0        0    76191 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/CHANGELOG.md
+-rw-r--r--   0        0        0      486 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/Dockerfile
+-rw-r--r--   0        0        0     1085 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/LICENSE
+-rw-r--r--   0        0        0     5293 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/Makefile
+-rw-r--r--   0        0        0    17711 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/README-VIM.md
+-rw-r--r--   0        0        0    36006 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/README.md
+-rwxr-xr-x   0        0        0     2419 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/bin/fzf-preview.sh
+-rwxr-xr-x   0        0        0     7069 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/bin/fzf-tmux
+-rw-r--r--   0        0        0    21398 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/doc/fzf.txt
+-rw-r--r--   0        0        0      496 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/go.mod
+-rw-r--r--   0        0        0     5203 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/go.sum
+-rwxr-xr-x   0        0        0    10184 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/install
+-rw-r--r--   0        0        0     1881 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/install.ps1
+-rw-r--r--   0        0        0     1159 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/main.go
+-rw-r--r--   0        0        0     4141 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/main_test.go
+-rw-r--r--   0        0        0     1992 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/man/man1/fzf-tmux.1
+-rw-r--r--   0        0        0    51227 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/man/man1/fzf.1
+-rw-r--r--   0        0        0    32728 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/plugin/fzf.vim
+-rw-r--r--   0        0        0    15837 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/shell/completion.bash
+-rw-r--r--   0        0        0    12432 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/shell/completion.zsh
+-rw-r--r--   0        0        0     5488 2024-05-01 07:18:57.940645 fzf_bin-0.51.0/fzf/shell/key-bindings.bash
+-rw-r--r--   0        0        0     5965 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/shell/key-bindings.fish
+-rw-r--r--   0        0        0     4138 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/shell/key-bindings.zsh
+-rw-r--r--   0        0        0     1085 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/LICENSE
+-rw-r--r--   0        0        0     5468 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/actiontype_string.go
+-rw-r--r--   0        0        0    26654 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/algo/algo.go
+-rw-r--r--   0        0        0     8883 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/algo/algo_test.go
+-rw-r--r--   0        0        0    21779 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/algo/normalize.go
+-rw-r--r--   0        0        0     9960 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/ansi.go
+-rw-r--r--   0        0        0    11138 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/ansi_test.go
+-rw-r--r--   0        0        0     1619 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/cache.go
+-rw-r--r--   0        0        0      859 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/cache_test.go
+-rw-r--r--   0        0        0     1806 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/chunklist.go
+-rw-r--r--   0        0        0     1862 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/chunklist_test.go
+-rw-r--r--   0        0        0     1704 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/constants.go
+-rw-r--r--   0        0        0    10379 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/core.go
+-rw-r--r--   0        0        0     2071 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/history.go
+-rw-r--r--   0        0        0     1507 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/history_test.go
+-rw-r--r--   0        0        0      957 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/item.go
+-rw-r--r--   0        0        0      484 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/item_test.go
+-rw-r--r--   0        0        0     5411 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/matcher.go
+-rw-r--r--   0        0        0     3302 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/merger.go
+-rw-r--r--   0        0        0     1989 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/merger_test.go
+-rw-r--r--   0        0        0    66036 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/options.go
+-rw-r--r--   0        0        0      307 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/options_no_pprof.go
+-rw-r--r--   0        0        0     1628 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/options_pprof.go
+-rw-r--r--   0        0        0     2069 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/options_pprof_test.go
+-rw-r--r--   0        0        0    14787 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/options_test.go
+-rw-r--r--   0        0        0    10565 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/pattern.go
+-rw-r--r--   0        0        0     8060 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/pattern_test.go
+-rw-r--r--   0        0        0      131 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/protector/protector.go
+-rw-r--r--   0        0        0      217 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/protector/protector_openbsd.go
+-rw-r--r--   0        0        0     5899 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/reader.go
+-rw-r--r--   0        0        0     1315 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/reader_test.go
+-rw-r--r--   0        0        0     5998 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/result.go
+-rw-r--r--   0        0        0      338 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/result_others.go
+-rw-r--r--   0        0        0     6064 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/result_test.go
+-rw-r--r--   0        0        0      364 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/result_x86.go
+-rw-r--r--   0        0        0     6297 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/server.go
+-rw-r--r--   0        0        0   114565 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/terminal.go
+-rw-r--r--   0        0        0    27942 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/terminal_test.go
+-rw-r--r--   0        0        0      449 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/terminal_unix.go
+-rw-r--r--   0        0        0      219 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/terminal_windows.go
+-rw-r--r--   0        0        0     5651 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/tokenizer.go
+-rw-r--r--   0        0        0     2858 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/tokenizer_test.go
+-rw-r--r--   0        0        0     1794 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/tui/dummy.go
+-rw-r--r--   0        0        0     3467 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/tui/eventtype_string.go
+-rw-r--r--   0        0        0    24618 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/tui/light.go
+-rw-r--r--   0        0        0     2510 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/tui/light_unix.go
+-rw-r--r--   0        0        0     4777 2024-05-01 07:18:57.944645 fzf_bin-0.51.0/fzf/src/tui/light_windows.go
+-rw-r--r--   0        0        0    18570 2024-05-01 07:18:57.948645 fzf_bin-0.51.0/fzf/src/tui/tcell.go
+-rw-r--r--   0        0        0    17392 2024-05-01 07:18:57.948645 fzf_bin-0.51.0/fzf/src/tui/tcell_test.go
+-rw-r--r--   0        0        0      908 2024-05-01 07:18:57.948645 fzf_bin-0.51.0/fzf/src/tui/ttyname_unix.go
+-rw-r--r--   0        0        0      164 2024-05-01 07:18:57.948645 fzf_bin-0.51.0/fzf/src/tui/ttyname_windows.go
+-rw-r--r--   0        0        0    21117 2024-05-01 07:18:57.948645 fzf_bin-0.51.0/fzf/src/tui/tui.go
+-rw-r--r--   0        0        0      399 2024-05-01 07:18:57.948645 fzf_bin-0.51.0/fzf/src/tui/tui_test.go
+-rw-r--r--   0        0        0      850 2024-05-01 07:18:57.948645 fzf_bin-0.51.0/fzf/src/util/atexit.go
+-rw-r--r--   0        0        0      452 2024-05-01 07:18:57.948645 fzf_bin-0.51.0/fzf/src/util/atexit_test.go
+-rw-r--r--   0        0        0      748 2024-05-01 07:18:57.948645 fzf_bin-0.51.0/fzf/src/util/atomicbool.go
+-rw-r--r--   0        0        0      301 2024-05-01 07:18:57.948645 fzf_bin-0.51.0/fzf/src/util/atomicbool_test.go
+-rw-r--r--   0        0        0     4308 2024-05-01 07:18:57.948645 fzf_bin-0.51.0/fzf/src/util/chars.go
+-rw-r--r--   0        0        0      981 2024-05-01 07:18:57.948645 fzf_bin-0.51.0/fzf/src/util/chars_test.go
+-rw-r--r--   0        0        0     1976 2024-05-01 07:18:57.948645 fzf_bin-0.51.0/fzf/src/util/eventbox.go
+-rw-r--r--   0        0        0      899 2024-05-01 07:18:57.948645 fzf_bin-0.51.0/fzf/src/util/eventbox_test.go
+-rw-r--r--   0        0        0      185 2024-05-01 07:18:57.948645 fzf_bin-0.51.0/fzf/src/util/slab.go
+-rw-r--r--   0        0        0     3733 2024-05-01 07:18:57.948645 fzf_bin-0.51.0/fzf/src/util/util.go
+-rw-r--r--   0        0        0     4194 2024-05-01 07:18:57.948645 fzf_bin-0.51.0/fzf/src/util/util_test.go
+-rw-r--r--   0        0        0     2226 2024-05-01 07:18:57.948645 fzf_bin-0.51.0/fzf/src/util/util_unix.go
+-rw-r--r--   0        0        0     4800 2024-05-01 07:18:57.948645 fzf_bin-0.51.0/fzf/src/util/util_windows.go
+-rw-r--r--   0        0        0     5860 2024-05-01 07:18:57.948645 fzf_bin-0.51.0/fzf/test/fzf.vader
+-rwxr-xr-x   0        0        0   128228 2024-05-01 07:18:57.948645 fzf_bin-0.51.0/fzf/test/test_go.rb
+-rw-r--r--   0        0        0      216 2024-05-01 07:18:57.948645 fzf_bin-0.51.0/fzf/typos.toml
+-rwxr-xr-x   0        0        0     2520 2024-05-01 07:18:57.948645 fzf_bin-0.51.0/fzf/uninstall
+-rw-r--r--   0        0        0        0 2024-05-01 07:18:56.584656 fzf_bin-0.51.0/fzf_bin/__init__.py
+-rw-r--r--   0        0        0     1392 2024-05-01 07:18:56.584656 fzf_bin-0.51.0/pdm_build.py
+-rw-r--r--   0        0        0     1073 2024-05-01 07:20:12.352080 fzf_bin-0.51.0/pyproject.toml
+-rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 fzf_bin-0.51.0/PKG-INFO
```

### Comparing `fzf_bin-0.50.0/LICENSE` & `fzf_bin-0.51.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/.github/ISSUE_TEMPLATE/issue_template.yml` & `fzf_bin-0.51.0/fzf/.github/ISSUE_TEMPLATE/issue_template.yml`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/.github/workflows/codeql-analysis.yml` & `fzf_bin-0.51.0/fzf/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/.github/workflows/linux.yml` & `fzf_bin-0.51.0/fzf/.github/workflows/linux.yml`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/.github/workflows/macos.yml` & `fzf_bin-0.51.0/fzf/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/.github/workflows/sponsors.yml` & `fzf_bin-0.51.0/fzf/.github/workflows/sponsors.yml`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/.goreleaser.yml` & `fzf_bin-0.51.0/fzf/.goreleaser.yml`

 * *Files 10% similar despite different names*

```diff
@@ -8,22 +8,24 @@
 builds:
   - id: fzf-macos
     binary: fzf
     goos:
       - darwin
     goarch:
       - amd64
+    flags:
+      - -trimpath
     ldflags:
       - "-s -w -X main.version={{ .Version }} -X main.revision={{ .ShortCommit }}"
     hooks:
       post: |
         sh -c '
         cat > /tmp/fzf-gon-amd64.hcl << EOF
         source = ["./dist/fzf-macos_darwin_amd64_v1/fzf"]
-        bundle_id = "kr.junegunn.fzf"
+        bundle_id = "junegunn.fzf"
         sign {
           application_identity = "Developer ID Application: Junegunn Choi (Y254DRW44Z)"
         }
         zip {
           output_path = "./dist/fzf-{{ .Version }}-darwin_amd64.zip"
         }
         EOF
@@ -32,22 +34,24 @@
 
   - id: fzf-macos-arm
     binary: fzf
     goos:
       - darwin
     goarch:
       - arm64
+    flags:
+      - -trimpath
     ldflags:
       - "-s -w -X main.version={{ .Version }} -X main.revision={{ .ShortCommit }}"
     hooks:
       post: |
         sh -c '
         cat > /tmp/fzf-gon-arm64.hcl << EOF
         source = ["./dist/fzf-macos-arm_darwin_arm64/fzf"]
-        bundle_id = "kr.junegunn.fzf"
+        bundle_id = "junegunn.fzf"
         sign {
           application_identity = "Developer ID Application: Junegunn Choi (Y254DRW44Z)"
         }
         zip {
           output_path = "./dist/fzf-{{ .Version }}-darwin_arm64.zip"
         }
         EOF
@@ -67,14 +71,16 @@
       - loong64
       - ppc64le
       - s390x
     goarm:
       - 5
       - 6
       - 7
+    flags:
+      - -trimpath
     ldflags:
       - "-s -w -X main.version={{ .Version }} -X main.revision={{ .ShortCommit }}"
     ignore:
       - goos: freebsd
         goarch: arm
       - goos: openbsd
         goarch: arm
```

### Comparing `fzf_bin-0.50.0/fzf/.rubocop.yml` & `fzf_bin-0.51.0/fzf/.rubocop.yml`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/ADVANCED.md` & `fzf_bin-0.51.0/fzf/ADVANCED.md`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/BUILD.md` & `fzf_bin-0.51.0/fzf/BUILD.md`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/CHANGELOG.md` & `fzf_bin-0.51.0/fzf/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,40 @@
 CHANGELOG
 =========
 
+0.51.0
+------
+- Added a new environment variable `$FZF_POS` exported to the child processes. It's the vertical position of the cursor in the list starting from 1.
+  ```sh
+  # Toggle selection to the top or to the bottom
+  seq 30 | fzf --multi --bind 'load:pos(10)' \
+    --bind 'shift-up:transform:for _ in $(seq $FZF_POS $FZF_MATCH_COUNT); do echo -n +toggle+up; done' \
+    --bind 'shift-down:transform:for _ in $(seq 1 $FZF_POS); do echo -n +toggle+down; done'
+  ```
+- Added `--with-shell` option to start child processes with a custom shell command and flags
+  ```sh
+  gem list | fzf --with-shell 'ruby -e' \
+    --preview 'pp Gem::Specification.find_by_name({1})' \
+    --bind 'ctrl-o:execute-silent:
+        spec = Gem::Specification.find_by_name({1})
+        [spec.homepage, *spec.metadata.filter { _1.end_with?("uri") }.values].uniq.each do
+          system "open", _1
+        end
+    '
+  ```
+- Added `change-multi` action for dynamically changing `--multi` option
+    - `change-multi` - enable multi-select mode with no limit
+    - `change-multi(NUM)` - enable multi-select mode with a limit
+    - `change-multi(0)` - disable multi-select mode
+- Windows improvements
+    - `become` action is now supported on Windows
+        - Unlike in *nix, this does not use `execve(2)`. Instead it spawns a new process and waits for it to finish, so the exact behavior may differ.
+    - Fixed argument escaping for Windows cmd.exe. No redundant escaping of backslashes.
+- Bug fixes and improvements
+
 0.50.0
 ------
 - Search performance optimization. You can observe 50%+ improvement in some scenarios.
   ```
   $ rg --line-number --no-heading --smart-case . > $DATA
 
   $ wc < $DATA
```

### Comparing `fzf_bin-0.50.0/fzf/LICENSE` & `fzf_bin-0.51.0/fzf/LICENSE`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/Makefile` & `fzf_bin-0.51.0/fzf/Makefile`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 REVISION       := $(FZF_REVISION)
 else
 REVISION       := $(shell git log -n 1 --pretty=format:%h --abbrev=8 -- $(SOURCES) 2> /dev/null)
 endif
 ifeq ($(REVISION),)
 $(error Not on git repository; cannot determine $$FZF_REVISION)
 endif
-BUILD_FLAGS    := -a -ldflags "-s -w -X main.version=$(VERSION) -X main.revision=$(REVISION)" -tags "$(TAGS)"
+BUILD_FLAGS    := -a -ldflags "-s -w -X main.version=$(VERSION) -X main.revision=$(REVISION)" -tags "$(TAGS)" -trimpath
 
 BINARY32       := fzf-$(GOOS)_386
 BINARY64       := fzf-$(GOOS)_amd64
 BINARYS390     := fzf-$(GOOS)_s390x
 BINARYARM5     := fzf-$(GOOS)_arm5
 BINARYARM6     := fzf-$(GOOS)_arm6
 BINARYARM7     := fzf-$(GOOS)_arm7
@@ -170,19 +170,19 @@
 	GOARCH=loong64 $(GO) build $(BUILD_FLAGS) -o $@
 
 bin/fzf: target/$(BINARY) | bin
 	-rm -f bin/fzf
 	cp -f target/$(BINARY) bin/fzf
 
 docker:
-	docker build -t fzf-arch .
-	docker run -it fzf-arch tmux
+	docker build -t fzf-ubuntu .
+	docker run -it fzf-ubuntu tmux
 
 docker-test:
-	docker build -t fzf-arch .
-	docker run -it fzf-arch
+	docker build -t fzf-ubuntu .
+	docker run -it fzf-ubuntu
 
 update:
 	$(GO) get -u
 	$(GO) mod tidy
 
 .PHONY: all generate build release test bench install clean docker docker-test update
```

### Comparing `fzf_bin-0.50.0/fzf/README-VIM.md` & `fzf_bin-0.51.0/fzf/README-VIM.md`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/README.md` & `fzf_bin-0.51.0/fzf/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 Sponsors ❤️
 -----------
 
 I would like to thank all the sponsors of this project who make it possible for me to continue to improve fzf.
 
 If you'd like to sponsor this project, please visit https://github.com/sponsors/junegunn.
 
-<!-- sponsors --><a href="https://github.com/miyanokomiya"><img src="https://github.com/miyanokomiya.png" width="60px" alt="miyanokomiya" /></a><a href="https://github.com/jonhoo"><img src="https://github.com/jonhoo.png" width="60px" alt="Jon Gjengset" /></a><a href="https://github.com/AceofSpades5757"><img src="https://github.com/AceofSpades5757.png" width="60px" alt="Kyle L. Davis" /></a><a href="https://github.com/Frederick888"><img src="https://github.com/Frederick888.png" width="60px" alt="Frederick Zhang" /></a><a href="https://github.com/moritzdietz"><img src="https://github.com/moritzdietz.png" width="60px" alt="Moritz Dietz" /></a><a href="https://github.com/mikker"><img src="https://github.com/mikker.png" width="60px" alt="Mikkel Malmberg" /></a><a href="https://github.com/pldubouilh"><img src="https://github.com/pldubouilh.png" width="60px" alt="Pierre Dubouilh" /></a><a href="https://github.com/rcorre"><img src="https://github.com/rcorre.png" width="60px" alt="Ryan Roden-Corrent" /></a><a href="https://github.com/blissdev"><img src="https://github.com/blissdev.png" width="60px" alt="Jordan Arentsen" /></a><a href="https://github.com/mislav"><img src="https://github.com/mislav.png" width="60px" alt="Mislav Marohnić" /></a><a href="https://github.com/aexvir"><img src="https://github.com/aexvir.png" width="60px" alt="Alex Viscreanu" /></a><a href="https://github.com/dbalatero"><img src="https://github.com/dbalatero.png" width="60px" alt="David Balatero" /></a><a href="https://github.com/comatory"><img src="https://github.com/comatory.png" width="60px" alt="Ondrej Synacek" /></a><a href="https://github.com/moobar"><img src="https://github.com/moobar.png" width="60px" alt="" /></a><a href="https://github.com/majjoha"><img src="https://github.com/majjoha.png" width="60px" alt="Mathias Jean Johansen" /></a><a href="https://github.com/benelan"><img src="https://github.com/benelan.png" width="60px" alt="Ben Elan" /></a><a href="https://github.com/pawelduda"><img src="https://github.com/pawelduda.png" width="60px" alt="Paweł Duda" /></a><a href="https://github.com/slezica"><img src="https://github.com/slezica.png" width="60px" alt="Santiago Lezica" /></a><a href="https://github.com/pbwn"><img src="https://github.com/pbwn.png" width="60px" alt="" /></a><a href="https://github.com/timgluz"><img src="https://github.com/timgluz.png" width="60px" alt="Timo Sulg" /></a><a href="https://github.com/pyrho"><img src="https://github.com/pyrho.png" width="60px" alt="Damien Rajon" /></a><a href="https://github.com/ArtBIT"><img src="https://github.com/ArtBIT.png" width="60px" alt="ArtBIT" /></a><a href="https://github.com/da-moon"><img src="https://github.com/da-moon.png" width="60px" alt="" /></a><a href="https://github.com/hovissimo"><img src="https://github.com/hovissimo.png" width="60px" alt="Hovis" /></a><a href="https://github.com/dariusjonda"><img src="https://github.com/dariusjonda.png" width="60px" alt="Darius Jonda" /></a><a href="https://github.com/cristiand391"><img src="https://github.com/cristiand391.png" width="60px" alt="Cristian Dominguez" /></a><a href="https://github.com/eliangcs"><img src="https://github.com/eliangcs.png" width="60px" alt="Chang-Hung Liang" /></a><a href="https://github.com/asphaltbuffet"><img src="https://github.com/asphaltbuffet.png" width="60px" alt="Ben Lechlitner" /></a><a href="https://github.com/yash1th"><img src="https://github.com/yash1th.png" width="60px" alt="yash" /></a><a href="https://github.com/looshch"><img src="https://github.com/looshch.png" width="60px" alt="george looshch" /></a><a href="https://github.com/kg8m"><img src="https://github.com/kg8m.png" width="60px" alt="Takumi KAGIYAMA" /></a><a href="https://github.com/polm"><img src="https://github.com/polm.png" width="60px" alt="Paul O'Leary McCann" /></a><a href="https://github.com/rbeeger"><img src="https://github.com/rbeeger.png" width="60px" alt="Robert Beeger" /></a><a href="https://github.com/veebch"><img src="https://github.com/veebch.png" width="60px" alt="VEEB Projects" /></a><a href="https://github.com/khuedoan"><img src="https://github.com/khuedoan.png" width="60px" alt="Khue Doan" /></a><a href="https://github.com/yowayb"><img src="https://github.com/yowayb.png" width="60px" alt="Yoway Buorn" /></a><a href="https://github.com/scalisi"><img src="https://github.com/scalisi.png" width="60px" alt="Josh Scalisi" /></a><a href="https://github.com/alecbcs"><img src="https://github.com/alecbcs.png" width="60px" alt="Alec Scott" /></a><a href="https://github.com/thnxdev"><img src="https://github.com/thnxdev.png" width="60px" alt="thanks.dev" /></a><a href="https://github.com/artursapek"><img src="https://github.com/artursapek.png" width="60px" alt="Artur Sapek" /></a><a href="https://github.com/ramnes"><img src="https://github.com/ramnes.png" width="60px" alt="Guillaume Gelin" /></a><a href="https://github.com/jyc"><img src="https://github.com/jyc.png" width="60px" alt="" /></a><a href="https://github.com/mrcnski"><img src="https://github.com/mrcnski.png" width="60px" alt="Marcin S." /></a><a href="https://github.com/roblevy"><img src="https://github.com/roblevy.png" width="60px" alt="Rob Levy" /></a><a href="https://github.com/glozow"><img src="https://github.com/glozow.png" width="60px" alt="Gloria Zhao" /></a><a href="https://github.com/wjt"><img src="https://github.com/wjt.png" width="60px" alt="Will Thompson" /></a><a href="https://github.com/mauricelam"><img src="https://github.com/mauricelam.png" width="60px" alt="Maurice Lam" /></a><a href="https://github.com/toupeira"><img src="https://github.com/toupeira.png" width="60px" alt="Markus Koller" /></a><a href="https://github.com/rkpatel33"><img src="https://github.com/rkpatel33.png" width="60px" alt="" /></a><a href="https://github.com/jamesob"><img src="https://github.com/jamesob.png" width="60px" alt="James O'Beirne" /></a><a href="https://github.com/joshuatz"><img src="https://github.com/joshuatz.png" width="60px" alt="Joshua Tzucker" /></a><!-- sponsors -->
+<!-- sponsors --><a href="https://github.com/miyanokomiya"><img src="https://github.com/miyanokomiya.png" width="60px" alt="miyanokomiya" /></a><a href="https://github.com/jonhoo"><img src="https://github.com/jonhoo.png" width="60px" alt="Jon Gjengset" /></a><a href="https://github.com/AceofSpades5757"><img src="https://github.com/AceofSpades5757.png" width="60px" alt="Kyle L. Davis" /></a><a href="https://github.com/Frederick888"><img src="https://github.com/Frederick888.png" width="60px" alt="Frederick Zhang" /></a><a href="https://github.com/moritzdietz"><img src="https://github.com/moritzdietz.png" width="60px" alt="Moritz Dietz" /></a><a href="https://github.com/mikker"><img src="https://github.com/mikker.png" width="60px" alt="Mikkel Malmberg" /></a><a href="https://github.com/pldubouilh"><img src="https://github.com/pldubouilh.png" width="60px" alt="Pierre Dubouilh" /></a><a href="https://github.com/rcorre"><img src="https://github.com/rcorre.png" width="60px" alt="Ryan Roden-Corrent" /></a><a href="https://github.com/blissdev"><img src="https://github.com/blissdev.png" width="60px" alt="Jordan Arentsen" /></a><a href="https://github.com/mislav"><img src="https://github.com/mislav.png" width="60px" alt="Mislav Marohnić" /></a><a href="https://github.com/aexvir"><img src="https://github.com/aexvir.png" width="60px" alt="Alex Viscreanu" /></a><a href="https://github.com/dbalatero"><img src="https://github.com/dbalatero.png" width="60px" alt="David Balatero" /></a><a href="https://github.com/comatory"><img src="https://github.com/comatory.png" width="60px" alt="Ondrej Synacek" /></a><a href="https://github.com/moobar"><img src="https://github.com/moobar.png" width="60px" alt="" /></a><a href="https://github.com/majjoha"><img src="https://github.com/majjoha.png" width="60px" alt="Mathias Jean Johansen" /></a><a href="https://github.com/benelan"><img src="https://github.com/benelan.png" width="60px" alt="Ben Elan" /></a><a href="https://github.com/pawelduda"><img src="https://github.com/pawelduda.png" width="60px" alt="Paweł Duda" /></a><a href="https://github.com/slezica"><img src="https://github.com/slezica.png" width="60px" alt="Santiago Lezica" /></a><a href="https://github.com/pbwn"><img src="https://github.com/pbwn.png" width="60px" alt="" /></a><a href="https://github.com/timgluz"><img src="https://github.com/timgluz.png" width="60px" alt="Timo Sulg" /></a><a href="https://github.com/pyrho"><img src="https://github.com/pyrho.png" width="60px" alt="Damien Rajon" /></a><a href="https://github.com/ArtBIT"><img src="https://github.com/ArtBIT.png" width="60px" alt="ArtBIT" /></a><a href="https://github.com/da-moon"><img src="https://github.com/da-moon.png" width="60px" alt="" /></a><a href="https://github.com/hovissimo"><img src="https://github.com/hovissimo.png" width="60px" alt="Hovis" /></a><a href="https://github.com/dariusjonda"><img src="https://github.com/dariusjonda.png" width="60px" alt="Darius Jonda" /></a><a href="https://github.com/cristiand391"><img src="https://github.com/cristiand391.png" width="60px" alt="Cristian Dominguez" /></a><a href="https://github.com/eliangcs"><img src="https://github.com/eliangcs.png" width="60px" alt="Chang-Hung Liang" /></a><a href="https://github.com/asphaltbuffet"><img src="https://github.com/asphaltbuffet.png" width="60px" alt="Ben Lechlitner" /></a><a href="https://github.com/yash1th"><img src="https://github.com/yash1th.png" width="60px" alt="yash" /></a><a href="https://github.com/looshch"><img src="https://github.com/looshch.png" width="60px" alt="george looshch" /></a><a href="https://github.com/kg8m"><img src="https://github.com/kg8m.png" width="60px" alt="Takumi KAGIYAMA" /></a><a href="https://github.com/polm"><img src="https://github.com/polm.png" width="60px" alt="Paul O'Leary McCann" /></a><a href="https://github.com/rbeeger"><img src="https://github.com/rbeeger.png" width="60px" alt="Robert Beeger" /></a><a href="https://github.com/veebch"><img src="https://github.com/veebch.png" width="60px" alt="VEEB Projects" /></a><a href="https://github.com/khuedoan"><img src="https://github.com/khuedoan.png" width="60px" alt="Khue Doan" /></a><a href="https://github.com/yowayb"><img src="https://github.com/yowayb.png" width="60px" alt="Yoway Buorn" /></a><a href="https://github.com/scalisi"><img src="https://github.com/scalisi.png" width="60px" alt="Josh Scalisi" /></a><a href="https://github.com/alecbcs"><img src="https://github.com/alecbcs.png" width="60px" alt="Alec Scott" /></a><a href="https://github.com/thnxdev"><img src="https://github.com/thnxdev.png" width="60px" alt="thanks.dev" /></a><a href="https://github.com/artursapek"><img src="https://github.com/artursapek.png" width="60px" alt="Artur Sapek" /></a><a href="https://github.com/ramnes"><img src="https://github.com/ramnes.png" width="60px" alt="Guillaume Gelin" /></a><a href="https://github.com/jyc"><img src="https://github.com/jyc.png" width="60px" alt="" /></a><a href="https://github.com/mrcnski"><img src="https://github.com/mrcnski.png" width="60px" alt="Marcin S." /></a><a href="https://github.com/roblevy"><img src="https://github.com/roblevy.png" width="60px" alt="Rob Levy" /></a><a href="https://github.com/warpdotdev"><img src="https://github.com/warpdotdev.png" width="60px" alt="Warp" /></a><a href="https://github.com/glozow"><img src="https://github.com/glozow.png" width="60px" alt="Gloria Zhao" /></a><a href="https://github.com/wjt"><img src="https://github.com/wjt.png" width="60px" alt="Will Thompson" /></a><a href="https://github.com/toupeira"><img src="https://github.com/toupeira.png" width="60px" alt="Markus Koller" /></a><a href="https://github.com/rkpatel33"><img src="https://github.com/rkpatel33.png" width="60px" alt="" /></a><a href="https://github.com/jamesob"><img src="https://github.com/jamesob.png" width="60px" alt="James O'Beirne" /></a><a href="https://github.com/joshuatz"><img src="https://github.com/joshuatz.png" width="60px" alt="Joshua Tzucker" /></a><a href="https://github.com/gpopides"><img src="https://github.com/gpopides.png" width="60px" alt="gpopides" /></a><a href="https://github.com/jlebray"><img src="https://github.com/jlebray.png" width="60px" alt="Johan Le Bray" /></a><!-- sponsors -->
 
 Table of Contents
 -----------------
 
 <!-- vim-markdown-toc GFM -->
 
 * [Installation](#installation)
@@ -118,14 +118,15 @@
 ### Using Homebrew
 
 You can use [Homebrew](https://brew.sh/) (on macOS or Linux)
 to install fzf.
 
 ```sh
 brew install fzf
+  # To build fzf from the latest source: brew install --HEAD fzf
 ```
 
 > [!IMPORTANT]
 > To set up shell integration (key bindings and fuzzy completion),
 > see [the instructions below](#setting-up-shell-integration).
 
 fzf is also available [via MacPorts][portfile]: `sudo port install fzf`
```

#### html2text {}

```diff
@@ -22,33 +22,33 @@
 _[_M_o_r_i_t_z_ _D_i_e_t_z_]_[_M_i_k_k_e_l_ _M_a_l_m_b_e_r_g_]_[_P_i_e_r_r_e_ _D_u_b_o_u_i_l_h_]_[_R_y_a_n_ _R_o_d_e_n_-_C_o_r_r_e_n_t_]_[_J_o_r_d_a_n
 _A_r_e_n_t_s_e_n_]_[_M_i_s_l_a_v_ _M_a_r_o_h_n_i_Ä__]_[_A_l_e_x_ _V_i_s_c_r_e_a_n_u_]_[_D_a_v_i_d_ _B_a_l_a_t_e_r_o_]_[_O_n_d_r_e_j_ _S_y_n_a_c_e_k_]
 _[_M_a_t_h_i_a_s_ _J_e_a_n_ _J_o_h_a_n_s_e_n_]_[_B_e_n_ _E_l_a_n_]_[_P_a_w_e_Å__ _D_u_d_a_]_[_S_a_n_t_i_a_g_o_ _L_e_z_i_c_a_]_[_T_i_m_o_ _S_u_l_g_]
 _[_D_a_m_i_e_n_ _R_a_j_o_n_]_[_A_r_t_B_I_T_]_[_H_o_v_i_s_]_[_D_a_r_i_u_s_ _J_o_n_d_a_]_[_C_r_i_s_t_i_a_n_ _D_o_m_i_n_g_u_e_z_]_[_C_h_a_n_g_-_H_u_n_g
 _L_i_a_n_g_]_[_B_e_n_ _L_e_c_h_l_i_t_n_e_r_]_[_y_a_s_h_]_[_g_e_o_r_g_e_ _l_o_o_s_h_c_h_]_[_T_a_k_u_m_i_ _K_A_G_I_Y_A_M_A_]_[_P_a_u_l_ _O_'_L_e_a_r_y
 _M_c_C_a_n_n_]_[_R_o_b_e_r_t_ _B_e_e_g_e_r_]_[_V_E_E_B_ _P_r_o_j_e_c_t_s_]_[_K_h_u_e_ _D_o_a_n_]_[_Y_o_w_a_y_ _B_u_o_r_n_]_[_J_o_s_h_ _S_c_a_l_i_s_i_]
 _[_A_l_e_c_ _S_c_o_t_t_]_[_t_h_a_n_k_s_._d_e_v_]_[_A_r_t_u_r_ _S_a_p_e_k_]_[_G_u_i_l_l_a_u_m_e_ _G_e_l_i_n_]_[_M_a_r_c_i_n_ _S_._]_[_R_o_b_ _L_e_v_y_]
-_[_G_l_o_r_i_a_ _Z_h_a_o_]_[_W_i_l_l_ _T_h_o_m_p_s_o_n_]_[_M_a_u_r_i_c_e_ _L_a_m_]_[_M_a_r_k_u_s_ _K_o_l_l_e_r_]_[_J_a_m_e_s_ _O_'_B_e_i_r_n_e_]_[_J_o_s_h_u_a
-_T_z_u_c_k_e_r_]Table of Contents ----------------- * [Installation](#installation) *
-[Using Homebrew](#using-homebrew) * [Using git](#using-git) * [Using Linux
-package managers](#using-linux-package-managers) * [Windows](#windows) *
-[Setting up shell integration](#setting-up-shell-integration) * [As Vim plugin]
-(#as-vim-plugin) * [Upgrading fzf](#upgrading-fzf) * [Building fzf](#building-
-fzf) * [Usage](#usage) * [Using the finder](#using-the-finder) * [Layout]
-(#layout) * [Search syntax](#search-syntax) * [Environment variables]
-(#environment-variables) * [Options](#options) * [Demo](#demo) * [Examples]
-(#examples) * [`fzf-tmux` script](#fzf-tmux-script) * [Key bindings for
-command-line](#key-bindings-for-command-line) * [Fuzzy completion for bash and
-zsh](#fuzzy-completion-for-bash-and-zsh) * [Files and directories](#files-and-
-directories) * [Process IDs](#process-ids) * [Host names](#host-names) *
-[Environment variables / Aliases](#environment-variables--aliases) * [Settings]
-(#settings) * [Supported commands](#supported-commands) * [Custom fuzzy
-completion](#custom-fuzzy-completion) * [Vim plugin](#vim-plugin) * [Advanced
-topics](#advanced-topics) * [Performance](#performance) * [Executing external
-programs](#executing-external-programs) * [Turning into a different process]
-(#turning-into-a-different-process) * [Reloading the candidate list]
+_[_W_a_r_p_]_[_G_l_o_r_i_a_ _Z_h_a_o_]_[_W_i_l_l_ _T_h_o_m_p_s_o_n_]_[_M_a_r_k_u_s_ _K_o_l_l_e_r_]_[_J_a_m_e_s_ _O_'_B_e_i_r_n_e_]_[_J_o_s_h_u_a
+_T_z_u_c_k_e_r_]_[_g_p_o_p_i_d_e_s_]_[_J_o_h_a_n_ _L_e_ _B_r_a_y_]Table of Contents ----------------- *
+[Installation](#installation) * [Using Homebrew](#using-homebrew) * [Using git]
+(#using-git) * [Using Linux package managers](#using-linux-package-managers) *
+[Windows](#windows) * [Setting up shell integration](#setting-up-shell-
+integration) * [As Vim plugin](#as-vim-plugin) * [Upgrading fzf](#upgrading-
+fzf) * [Building fzf](#building-fzf) * [Usage](#usage) * [Using the finder]
+(#using-the-finder) * [Layout](#layout) * [Search syntax](#search-syntax) *
+[Environment variables](#environment-variables) * [Options](#options) * [Demo]
+(#demo) * [Examples](#examples) * [`fzf-tmux` script](#fzf-tmux-script) * [Key
+bindings for command-line](#key-bindings-for-command-line) * [Fuzzy completion
+for bash and zsh](#fuzzy-completion-for-bash-and-zsh) * [Files and directories]
+(#files-and-directories) * [Process IDs](#process-ids) * [Host names](#host-
+names) * [Environment variables / Aliases](#environment-variables--aliases) *
+[Settings](#settings) * [Supported commands](#supported-commands) * [Custom
+fuzzy completion](#custom-fuzzy-completion) * [Vim plugin](#vim-plugin) *
+[Advanced topics](#advanced-topics) * [Performance](#performance) * [Executing
+external programs](#executing-external-programs) * [Turning into a different
+process](#turning-into-a-different-process) * [Reloading the candidate list]
 (#reloading-the-candidate-list) * [1. Update the list of processes by pressing
 CTRL-R](#1-update-the-list-of-processes-by-pressing-ctrl-r) * [2. Switch
 between sources by pressing CTRL-D or CTRL-F](#2-switch-between-sources-by-
 pressing-ctrl-d-or-ctrl-f) * [3. Interactive ripgrep integration](#3-
 interactive-ripgrep-integration) * [Preview window](#preview-window) *
 [Previewing an image](#previewing-an-image) * [Tips](#tips) * [Respecting
 `.gitignore`](#respecting-gitignore) * [Fish shell](#fish-shell) * [fzf Theme
@@ -56,156 +56,157 @@
 [License](#license) Installation ------------ fzf project consists of the
 following components: - `fzf` executable - `fzf-tmux` script for launching fzf
 in a tmux pane - Shell integration - Key bindings (`CTRL-T`, `CTRL-R`, and
 `ALT-C`) (bash, zsh, fish) - Fuzzy completion (bash, zsh) - Vim/Neovim plugin
 You can [download fzf executable][bin] alone if you don't need the extra stuff.
 [bin]: https://github.com/junegunn/fzf/releases ### Using Homebrew You can use
 [Homebrew](https://brew.sh/) (on macOS or Linux) to install fzf. ```sh brew
-install fzf ``` > [!IMPORTANT] > To set up shell integration (key bindings and
-fuzzy completion), > see [the instructions below](#setting-up-shell-
-integration). fzf is also available [via MacPorts][portfile]: `sudo port
-install fzf` [portfile]: https://github.com/macports/macports-ports/blob/
-master/sysutils/fzf/Portfile ### Using git Alternatively, you can "git clone"
-this repository to any directory and run [install](https://github.com/junegunn/
-fzf/blob/master/install) script. ```sh git clone --depth 1 https://github.com/
-junegunn/fzf.git ~/.fzf ~/.fzf/install ``` The install script will add lines to
-your shell configuration file to modify `$PATH` and set up shell integration.
-### Using Linux package managers | Package Manager | Linux Distribution |
-Command | | --------------- | ----------------------- | -----------------------
------------ | | APK | Alpine Linux | `sudo apk add fzf` | | APT | Debian 9+/
-Ubuntu 19.10+ | `sudo apt install fzf` | | Conda | | `conda install -c conda-
-forge fzf` | | DNF | Fedora | `sudo dnf install fzf` | | Nix | NixOS, etc. |
-`nix-env -iA nixpkgs.fzf` | | Pacman | Arch Linux | `sudo pacman -S fzf` | |
-pkg | FreeBSD | `pkg install fzf` | | pkgin | NetBSD | `pkgin install fzf` | |
-pkg_add | OpenBSD | `pkg_add fzf` | | Portage | Gentoo | `emerge --ask app-
-shells/fzf` | | Spack | | `spack install fzf` | | XBPS | Void Linux | `sudo
-xbps-install -S fzf` | | Zypper | openSUSE | `sudo zypper install fzf` | >
-[!IMPORTANT] > To set up shell integration (key bindings and fuzzy completion),
-> see [the instructions below](#setting-up-shell-integration). [![Packaging
-status](https://repology.org/badge/vertical-allrepos/fzf.svg)](https://
-repology.org/project/fzf/versions) ### Windows Pre-built binaries for Windows
-can be downloaded [here][bin]. fzf is also available via [Chocolatey][choco],
-[Scoop][scoop], [Winget][winget], and [MSYS2][msys2]: | Package manager |
-Command | | --------------- | ------------------------------------- | |
-Chocolatey | `choco install fzf` | | Scoop | `scoop install fzf` | | Winget |
-`winget install fzf` | | MSYS2 (pacman) | `pacman -S $MINGW_PACKAGE_PREFIX-fzf`
-| [choco]: https://chocolatey.org/packages/fzf [scoop]: https://github.com/
-ScoopInstaller/Main/blob/master/bucket/fzf.json [winget]: https://github.com/
-microsoft/winget-pkgs/tree/master/manifests/j/junegunn/fzf [msys2]: https://
-packages.msys2.org/base/mingw-w64-fzf Known issues and limitations on Windows
-can be found on [the wiki page][windows-wiki]. [windows-wiki]: https://
-github.com/junegunn/fzf/wiki/Windows ### Setting up shell integration Add the
-following line to your shell configuration file. * bash ```sh # Set up fzf key
-bindings and fuzzy completion eval "$(fzf --bash)" ``` * zsh ```sh # Set up fzf
-key bindings and fuzzy completion eval "$(fzf --zsh)" ``` * fish ```fish # Set
-up fzf key bindings fzf --fish | source ``` > [!NOTE] > `--bash`, `--zsh`, and
-`--fish` options are only available in fzf 0.48.0 or > later. If you have an
-older version of fzf, or want finer control, you can > source individual script
-files in the [/shell](/shell) directory. The > location of the files may vary
-depending on the package manager you use. > Please refer to the package
-documentation for more information. > (e.g. `apt show fzf`) > [!TIP] > You can
-disable CTRL-T or ALT-C binding by setting `FZF_CTRL_T_COMMAND` or >
-`FZF_ALT_C_COMMAND` to an empty string when sourcing the script. > For example,
-to disable ALT-C binding: > > * bash: `FZF_ALT_C_COMMAND= eval "$(fzf --bash)"`
-> * zsh: `FZF_ALT_C_COMMAND= eval "$(fzf --zsh)"` > * fish: `fzf --fish |
-FZF_ALT_C_COMMAND= source` > > Setting the variables after sourcing the script
-will have no effect. ### As Vim plugin If you use [vim-plug](https://
-github.com/junegunn/vim-plug), add this line to your Vim configuration file:
-```vim Plug 'junegunn/fzf', { 'do': { -> fzf#install() } } ``` `fzf#install()`
-makes sure that you have the latest binary, but it's optional, so you can omit
-it if you use a plugin manager that doesn't support hooks. For more
-installation options, see [README-VIM.md](README-VIM.md). Upgrading fzf -------
------- fzf is being actively developed, and you might want to upgrade it once
-in a while. Please follow the instruction below depending on the installation
-method used. - git: `cd ~/.fzf && git pull && ./install` - brew: `brew update;
-brew upgrade fzf` - macports: `sudo port upgrade fzf` - chocolatey: `choco
-upgrade fzf` - vim-plug: `:PlugUpdate fzf` Building fzf ------------ See
-[BUILD.md](BUILD.md). Usage ----- fzf will launch interactive finder, read the
-list from STDIN, and write the selected item to STDOUT. ```sh find * -type f |
-fzf > selected ``` Without STDIN pipe, fzf will traverse the file system under
-the current directory to get the list of files. ```sh vim $(fzf) ``` > [!NOTE]
-> You can override the default behavior > * Either by setting
-`$FZF_DEFAULT_COMMAND` to a command that generates the desired list > * Or by
-setting `--walker`, `--walker-root`, and `--walker-skip` options in
-`$FZF_DEFAULT_OPTS` > [!WARNING] > A more robust solution would be to use
-`xargs` but we've presented > the above as it's easier to grasp > ```sh > fzf -
--print0 | xargs -0 -o vim > ``` > [!TIP] > fzf also has the ability to turn
-itself into a different process. > > ```sh > fzf --bind 'enter:become(vim {})'
-> ``` > > *See [Turning into a different process](#turning-into-a-different-
-process) > for more information.* ### Using the finder - `CTRL-K` / `CTRL-J`
-(or `CTRL-P` / `CTRL-N`) to move cursor up and down - `Enter` key to select the
-item, `CTRL-C` / `CTRL-G` / `ESC` to exit - On multi-select mode (`-m`), `TAB`
-and `Shift-TAB` to mark multiple items - Emacs style key bindings - Mouse:
-scroll, click, double-click; shift-click and shift-scroll on multi-select mode
-### Layout fzf by default starts in fullscreen mode, but you can make it start
-below the cursor with `--height` option. ```sh vim $(fzf --height 40%) ```
-Also, check out `--reverse` and `--layout` options if you prefer "top-down"
-layout instead of the default "bottom-up" layout. ```sh vim $(fzf --height 40%
---reverse) ``` You can add these options to `$FZF_DEFAULT_OPTS` so that they're
-applied by default. For example, ```sh export FZF_DEFAULT_OPTS='--height 40% --
-layout=reverse --border' ``` ### Search syntax Unless otherwise specified, fzf
-starts in "extended-search mode" where you can type in multiple search terms
-delimited by spaces. e.g. `^music .mp3$ sbtrkt !fire` | Token | Match type |
-Description | | --------- | -------------------------- | ----------------------
--------------- | | `sbtrkt` | fuzzy-match | Items that match `sbtrkt` | |
-`'wild` | exact-match (quoted) | Items that include `wild` | | `^music` |
-prefix-exact-match | Items that start with `music` | | `.mp3$` | suffix-exact-
-match | Items that end with `.mp3` | | `!fire` | inverse-exact-match | Items
-that do not include `fire` | | `!^music` | inverse-prefix-exact-match | Items
-that do not start with `music` | | `!.mp3$` | inverse-suffix-exact-match |
-Items that do not end with `.mp3` | If you don't prefer fuzzy matching and do
-not wish to "quote" every word, start fzf with `-e` or `--exact` option. Note
-that when `--exact` is set, `'`-prefix "unquotes" the term. A single bar
-character term acts as an OR operator. For example, the following query matches
-entries that start with `core` and end with either `go`, `rb`, or `py`. ```
-^core go$ | rb$ | py$ ``` ### Environment variables - `FZF_DEFAULT_COMMAND` -
-Default command to use when input is tty - e.g. `export FZF_DEFAULT_COMMAND='fd
---type f'` - `FZF_DEFAULT_OPTS` - Default options - e.g. `export
-FZF_DEFAULT_OPTS="--layout=reverse --inline-info"` - `FZF_DEFAULT_OPTS_FILE` -
-If you prefer to manage default options in a file, set this variable to point
-to the location of the file - e.g. `export FZF_DEFAULT_OPTS_FILE=~/.fzfrc` >
-[!WARNING] > `FZF_DEFAULT_COMMAND` is not used by shell integration due to the
-> slight difference in requirements. > > * `CTRL-T` runs `$FZF_CTRL_T_COMMAND`
-to get a list of files and directories > * `ALT-C` runs `$FZF_ALT_C_COMMAND` to
-get a list of directories > * `vim ~/**` runs `fzf_compgen_path()` with the
-prefix (`~/`) as the first argument > * `cd foo**` runs `fzf_compgen_dir()`
-with the prefix (`foo`) as the first argument > > The available options are
-described later in this document. ### Options See the man page (`man fzf`) for
-the full list of options. ### Demo If you learn by watching videos, check out
-this screencast by [@samoshkin](https://github.com/samoshkin) to explore `fzf`
-features. _[_h_t_t_p_s_:_/_/_i_._i_m_g_u_r_._c_o_m_/_v_t_G_8_o_l_E_._p_n_g_]Examples -------- * [Wiki page of
-examples](https://github.com/junegunn/fzf/wiki/examples) * *Disclaimer: The
-examples on this page are maintained by the community and are not thoroughly
-tested* * [Advanced fzf examples](https://github.com/junegunn/fzf/blob/master/
-ADVANCED.md) `fzf-tmux` script ----------------- [fzf-tmux](bin/fzf-tmux) is a
-bash script that opens fzf in a tmux pane. ```sh # usage: fzf-tmux [LAYOUT
-OPTIONS] [--] [FZF OPTIONS] # See available options fzf-tmux --help # select
-git branches in horizontal split below (15 lines) git branch | fzf-tmux -d 15 #
-select multiple words in vertical split on the left (20% of screen width) cat /
-usr/share/dict/words | fzf-tmux -l 20% --multi --reverse ``` It will still work
-even when you're not on tmux, silently ignoring `-[pudlr]` options, so you can
-invariably use `fzf-tmux` in your scripts. Alternatively, you can use `--height
-HEIGHT[%]` option not to start fzf in fullscreen mode. ```sh fzf --height 40%
-``` Key bindings for command-line ----------------------------- The install
-script will setup the following key bindings for bash, zsh, and fish. - `CTRL-
-T` - Paste the selected files and directories onto the command-line - The list
-is generated using `--walker file,dir,follow,hidden` option - You can override
-the behavior by setting `FZF_CTRL_T_COMMAND` to a custom command that generates
-the desired list - Or you can set `--walker*` options in `FZF_CTRL_T_OPTS` -
-Set `FZF_CTRL_T_OPTS` to pass additional options to fzf ```sh # Preview file
-content using bat (https://github.com/sharkdp/bat) export FZF_CTRL_T_OPTS=" --
-walker-skip .git,node_modules,target --preview 'bat -n --color=always {}' --
-bind 'ctrl-/:change-preview-window(down|hidden|)'" ``` - Can be disabled by
-setting `FZF_CTRL_T_COMMAND` to an empty string when sourcing the script -
-`CTRL-R` - Paste the selected command from history onto the command-line - If
-you want to see the commands in chronological order, press `CTRL-R` again which
-toggles sorting by relevance - Set `FZF_CTRL_R_OPTS` to pass additional options
-to fzf ```sh # CTRL-/ to toggle small preview window to see the full command #
-CTRL-Y to copy the command into clipboard using pbcopy export FZF_CTRL_R_OPTS="
---preview 'echo {}' --preview-window up:3:hidden:wrap --bind 'ctrl-/:toggle-
+install fzf # To build fzf from the latest source: brew install --HEAD fzf ```
+> [!IMPORTANT] > To set up shell integration (key bindings and fuzzy
+completion), > see [the instructions below](#setting-up-shell-integration). fzf
+is also available [via MacPorts][portfile]: `sudo port install fzf` [portfile]:
+https://github.com/macports/macports-ports/blob/master/sysutils/fzf/Portfile
+### Using git Alternatively, you can "git clone" this repository to any
+directory and run [install](https://github.com/junegunn/fzf/blob/master/
+install) script. ```sh git clone --depth 1 https://github.com/junegunn/fzf.git
+~/.fzf ~/.fzf/install ``` The install script will add lines to your shell
+configuration file to modify `$PATH` and set up shell integration. ### Using
+Linux package managers | Package Manager | Linux Distribution | Command | | ---
+------------ | ----------------------- | ---------------------------------- | |
+APK | Alpine Linux | `sudo apk add fzf` | | APT | Debian 9+/Ubuntu 19.10+ |
+`sudo apt install fzf` | | Conda | | `conda install -c conda-forge fzf` | | DNF
+| Fedora | `sudo dnf install fzf` | | Nix | NixOS, etc. | `nix-env -iA
+nixpkgs.fzf` | | Pacman | Arch Linux | `sudo pacman -S fzf` | | pkg | FreeBSD |
+`pkg install fzf` | | pkgin | NetBSD | `pkgin install fzf` | | pkg_add |
+OpenBSD | `pkg_add fzf` | | Portage | Gentoo | `emerge --ask app-shells/fzf` |
+| Spack | | `spack install fzf` | | XBPS | Void Linux | `sudo xbps-install -
+S fzf` | | Zypper | openSUSE | `sudo zypper install fzf` | > [!IMPORTANT] > To
+set up shell integration (key bindings and fuzzy completion), > see [the
+instructions below](#setting-up-shell-integration). [![Packaging status](https:
+//repology.org/badge/vertical-allrepos/fzf.svg)](https://repology.org/project/
+fzf/versions) ### Windows Pre-built binaries for Windows can be downloaded
+[here][bin]. fzf is also available via [Chocolatey][choco], [Scoop][scoop],
+[Winget][winget], and [MSYS2][msys2]: | Package manager | Command | | ---------
+------ | ------------------------------------- | | Chocolatey | `choco install
+fzf` | | Scoop | `scoop install fzf` | | Winget | `winget install fzf` | |
+MSYS2 (pacman) | `pacman -S $MINGW_PACKAGE_PREFIX-fzf` | [choco]: https://
+chocolatey.org/packages/fzf [scoop]: https://github.com/ScoopInstaller/Main/
+blob/master/bucket/fzf.json [winget]: https://github.com/microsoft/winget-pkgs/
+tree/master/manifests/j/junegunn/fzf [msys2]: https://packages.msys2.org/base/
+mingw-w64-fzf Known issues and limitations on Windows can be found on [the wiki
+page][windows-wiki]. [windows-wiki]: https://github.com/junegunn/fzf/wiki/
+Windows ### Setting up shell integration Add the following line to your shell
+configuration file. * bash ```sh # Set up fzf key bindings and fuzzy completion
+eval "$(fzf --bash)" ``` * zsh ```sh # Set up fzf key bindings and fuzzy
+completion eval "$(fzf --zsh)" ``` * fish ```fish # Set up fzf key bindings fzf
+--fish | source ``` > [!NOTE] > `--bash`, `--zsh`, and `--fish` options are
+only available in fzf 0.48.0 or > later. If you have an older version of fzf,
+or want finer control, you can > source individual script files in the [/shell]
+(/shell) directory. The > location of the files may vary depending on the
+package manager you use. > Please refer to the package documentation for more
+information. > (e.g. `apt show fzf`) > [!TIP] > You can disable CTRL-T or ALT-
+C binding by setting `FZF_CTRL_T_COMMAND` or > `FZF_ALT_C_COMMAND` to an empty
+string when sourcing the script. > For example, to disable ALT-C binding: > > *
+bash: `FZF_ALT_C_COMMAND= eval "$(fzf --bash)"` > * zsh: `FZF_ALT_C_COMMAND=
+eval "$(fzf --zsh)"` > * fish: `fzf --fish | FZF_ALT_C_COMMAND= source` > >
+Setting the variables after sourcing the script will have no effect. ### As Vim
+plugin If you use [vim-plug](https://github.com/junegunn/vim-plug), add this
+line to your Vim configuration file: ```vim Plug 'junegunn/fzf', { 'do': { -
+> fzf#install() } } ``` `fzf#install()` makes sure that you have the latest
+binary, but it's optional, so you can omit it if you use a plugin manager that
+doesn't support hooks. For more installation options, see [README-VIM.md]
+(README-VIM.md). Upgrading fzf ------------- fzf is being actively developed,
+and you might want to upgrade it once in a while. Please follow the instruction
+below depending on the installation method used. - git: `cd ~/.fzf && git pull
+&& ./install` - brew: `brew update; brew upgrade fzf` - macports: `sudo port
+upgrade fzf` - chocolatey: `choco upgrade fzf` - vim-plug: `:PlugUpdate fzf`
+Building fzf ------------ See [BUILD.md](BUILD.md). Usage ----- fzf will launch
+interactive finder, read the list from STDIN, and write the selected item to
+STDOUT. ```sh find * -type f | fzf > selected ``` Without STDIN pipe, fzf will
+traverse the file system under the current directory to get the list of files.
+```sh vim $(fzf) ``` > [!NOTE] > You can override the default behavior > *
+Either by setting `$FZF_DEFAULT_COMMAND` to a command that generates the
+desired list > * Or by setting `--walker`, `--walker-root`, and `--walker-skip`
+options in `$FZF_DEFAULT_OPTS` > [!WARNING] > A more robust solution would be
+to use `xargs` but we've presented > the above as it's easier to grasp > ```sh
+> fzf --print0 | xargs -0 -o vim > ``` > [!TIP] > fzf also has the ability to
+turn itself into a different process. > > ```sh > fzf --bind 'enter:become(vim
+{})' > ``` > > *See [Turning into a different process](#turning-into-a-
+different-process) > for more information.* ### Using the finder - `CTRL-K` /
+`CTRL-J` (or `CTRL-P` / `CTRL-N`) to move cursor up and down - `Enter` key to
+select the item, `CTRL-C` / `CTRL-G` / `ESC` to exit - On multi-select mode (`-
+m`), `TAB` and `Shift-TAB` to mark multiple items - Emacs style key bindings -
+Mouse: scroll, click, double-click; shift-click and shift-scroll on multi-
+select mode ### Layout fzf by default starts in fullscreen mode, but you can
+make it start below the cursor with `--height` option. ```sh vim $(fzf --height
+40%) ``` Also, check out `--reverse` and `--layout` options if you prefer "top-
+down" layout instead of the default "bottom-up" layout. ```sh vim $(fzf --
+height 40% --reverse) ``` You can add these options to `$FZF_DEFAULT_OPTS` so
+that they're applied by default. For example, ```sh export FZF_DEFAULT_OPTS='--
+height 40% --layout=reverse --border' ``` ### Search syntax Unless otherwise
+specified, fzf starts in "extended-search mode" where you can type in multiple
+search terms delimited by spaces. e.g. `^music .mp3$ sbtrkt !fire` | Token |
+Match type | Description | | --------- | -------------------------- | ---------
+--------------------------- | | `sbtrkt` | fuzzy-match | Items that match
+`sbtrkt` | | `'wild` | exact-match (quoted) | Items that include `wild` | |
+`^music` | prefix-exact-match | Items that start with `music` | | `.mp3$` |
+suffix-exact-match | Items that end with `.mp3` | | `!fire` | inverse-exact-
+match | Items that do not include `fire` | | `!^music` | inverse-prefix-exact-
+match | Items that do not start with `music` | | `!.mp3$` | inverse-suffix-
+exact-match | Items that do not end with `.mp3` | If you don't prefer fuzzy
+matching and do not wish to "quote" every word, start fzf with `-e` or `--
+exact` option. Note that when `--exact` is set, `'`-prefix "unquotes" the term.
+A single bar character term acts as an OR operator. For example, the following
+query matches entries that start with `core` and end with either `go`, `rb`, or
+`py`. ``` ^core go$ | rb$ | py$ ``` ### Environment variables -
+`FZF_DEFAULT_COMMAND` - Default command to use when input is tty - e.g. `export
+FZF_DEFAULT_COMMAND='fd --type f'` - `FZF_DEFAULT_OPTS` - Default options -
+e.g. `export FZF_DEFAULT_OPTS="--layout=reverse --inline-info"` -
+`FZF_DEFAULT_OPTS_FILE` - If you prefer to manage default options in a file,
+set this variable to point to the location of the file - e.g. `export
+FZF_DEFAULT_OPTS_FILE=~/.fzfrc` > [!WARNING] > `FZF_DEFAULT_COMMAND` is not
+used by shell integration due to the > slight difference in requirements. > > *
+`CTRL-T` runs `$FZF_CTRL_T_COMMAND` to get a list of files and directories > *
+`ALT-C` runs `$FZF_ALT_C_COMMAND` to get a list of directories > * `vim ~/**`
+runs `fzf_compgen_path()` with the prefix (`~/`) as the first argument > * `cd
+foo**` runs `fzf_compgen_dir()` with the prefix (`foo`) as the first argument >
+> The available options are described later in this document. ### Options See
+the man page (`man fzf`) for the full list of options. ### Demo If you learn by
+watching videos, check out this screencast by [@samoshkin](https://github.com/
+samoshkin) to explore `fzf` features. _[_h_t_t_p_s_:_/_/_i_._i_m_g_u_r_._c_o_m_/_v_t_G_8_o_l_E_._p_n_g_]Examples
+-------- * [Wiki page of examples](https://github.com/junegunn/fzf/wiki/
+examples) * *Disclaimer: The examples on this page are maintained by the
+community and are not thoroughly tested* * [Advanced fzf examples](https://
+github.com/junegunn/fzf/blob/master/ADVANCED.md) `fzf-tmux` script ------------
+----- [fzf-tmux](bin/fzf-tmux) is a bash script that opens fzf in a tmux pane.
+```sh # usage: fzf-tmux [LAYOUT OPTIONS] [--] [FZF OPTIONS] # See available
+options fzf-tmux --help # select git branches in horizontal split below (15
+lines) git branch | fzf-tmux -d 15 # select multiple words in vertical split on
+the left (20% of screen width) cat /usr/share/dict/words | fzf-tmux -l 20% --
+multi --reverse ``` It will still work even when you're not on tmux, silently
+ignoring `-[pudlr]` options, so you can invariably use `fzf-tmux` in your
+scripts. Alternatively, you can use `--height HEIGHT[%]` option not to start
+fzf in fullscreen mode. ```sh fzf --height 40% ``` Key bindings for command-
+line ----------------------------- The install script will setup the following
+key bindings for bash, zsh, and fish. - `CTRL-T` - Paste the selected files and
+directories onto the command-line - The list is generated using `--walker
+file,dir,follow,hidden` option - You can override the behavior by setting
+`FZF_CTRL_T_COMMAND` to a custom command that generates the desired list - Or
+you can set `--walker*` options in `FZF_CTRL_T_OPTS` - Set `FZF_CTRL_T_OPTS` to
+pass additional options to fzf ```sh # Preview file content using bat (https://
+github.com/sharkdp/bat) export FZF_CTRL_T_OPTS=" --walker-skip
+.git,node_modules,target --preview 'bat -n --color=always {}' --bind 'ctrl-/:
+change-preview-window(down|hidden|)'" ``` - Can be disabled by setting
+`FZF_CTRL_T_COMMAND` to an empty string when sourcing the script - `CTRL-R` -
+Paste the selected command from history onto the command-line - If you want to
+see the commands in chronological order, press `CTRL-R` again which toggles
+sorting by relevance - Set `FZF_CTRL_R_OPTS` to pass additional options to fzf
+```sh # CTRL-/ to toggle small preview window to see the full command # CTRL-
+Y to copy the command into clipboard using pbcopy export FZF_CTRL_R_OPTS=" --
+preview 'echo {}' --preview-window up:3:hidden:wrap --bind 'ctrl-/:toggle-
 preview' --bind 'ctrl-y:execute-silent(echo -n {2..} | pbcopy)+abort' --color
 header:italic --header 'Press CTRL-Y to copy command into clipboard'" ``` -
 `ALT-C` - cd into the selected directory - The list is generated using `--
 walker dir,follow,hidden` option - Set `FZF_ALT_C_COMMAND` to override the
 default command - Or you can set `--walker-*` options in `FZF_ALT_C_OPTS` - Set
 `FZF_ALT_C_OPTS` to pass additional options to fzf ```sh # Print tree structure
 in the preview window export FZF_ALT_C_OPTS=" --walker-skip
```

### Comparing `fzf_bin-0.50.0/fzf/bin/fzf-preview.sh` & `fzf_bin-0.51.0/fzf/bin/fzf-preview.sh`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/bin/fzf-tmux` & `fzf_bin-0.51.0/fzf/bin/fzf-tmux`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # usage: fzf-tmux [LAYOUT OPTIONS] [--] [FZF OPTIONS]
 
 fail() {
   >&2 echo "$1"
   exit 2
 }
 
-fzf="$(command -v fzf 2> /dev/null)" || fzf="$(dirname "$0")/fzf"
+fzf="$(command which fzf)" || fzf="$(dirname "$0")/fzf"
 [[ -x "$fzf" ]] || fail 'fzf executable not found'
 
 args=()
 opt=""
 skip=""
 swap=""
 close=""
```

### Comparing `fzf_bin-0.50.0/fzf/doc/fzf.txt` & `fzf_bin-0.51.0/fzf/doc/fzf.txt`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/go.sum` & `fzf_bin-0.51.0/fzf/go.sum`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/install` & `fzf_bin-0.51.0/fzf/install`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env bash
 
 set -u
 
-version=0.50.0
+version=0.51.0
 auto_completion=
 key_bindings=
 update_config=2
 shells="bash zsh fish"
 prefix='~/.fzf'
 prefix_expand=~/.fzf
 fish_dir=${XDG_CONFIG_HOME:-$HOME/.config}/fish
```

### Comparing `fzf_bin-0.50.0/fzf/install.ps1` & `fzf_bin-0.51.0/fzf/install.ps1`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-$version="0.50.0"
+$version="0.51.0"
 
 $fzf_base=Split-Path -Parent $MyInvocation.MyCommand.Definition
 
 function check_binary () {
   Write-Host "  - Checking fzf executable ... " -NoNewline
   $output=cmd /c $fzf_base\bin\fzf.exe --version 2>&1
   if (-not $?) {
```

### Comparing `fzf_bin-0.50.0/fzf/main.go` & `fzf_bin-0.51.0/fzf/main.go`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 	"fmt"
 	"strings"
 
 	fzf "github.com/junegunn/fzf/src"
 	"github.com/junegunn/fzf/src/protector"
 )
 
-var version string = "0.50"
+var version string = "0.51"
 var revision string = "devel"
 
 //go:embed shell/key-bindings.bash
 var bashKeyBindings []byte
 
 //go:embed shell/completion.bash
 var bashCompletion []byte
```

### Comparing `fzf_bin-0.50.0/fzf/main_test.go` & `fzf_bin-0.51.0/fzf/main_test.go`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,42 @@
 package main
 
 import (
+	"bytes"
 	"fmt"
 	"go/ast"
 	"go/build"
 	"go/importer"
 	"go/parser"
 	"go/token"
 	"go/types"
 	"io/fs"
 	"os"
+	"os/exec"
 	"path/filepath"
 	"sort"
 	"strings"
 	"testing"
 )
 
 func loadPackages(t *testing.T) []*build.Package {
+	// If GOROOT is not set, use `go env GOROOT` to determine it since it
+	// performs more work than just runtime.GOROOT(). For context, running
+	// the tests with the "-trimpath" flag causes GOROOT to not be set.
+	ctxt := &build.Default
+	if ctxt.GOROOT == "" {
+		cmd := exec.Command("go", "env", "GOROOT")
+		out, err := cmd.CombinedOutput()
+		out = bytes.TrimSpace(out)
+		if err != nil {
+			t.Fatalf("error running command: %q: %v\n%s", cmd.Args, err, out)
+		}
+		ctxt.GOROOT = string(out)
+	}
+
 	wd, err := os.Getwd()
 	if err != nil {
 		t.Fatal(err)
 	}
 
 	var pkgs []*build.Package
 	seen := make(map[string]bool)
@@ -34,15 +50,15 @@
 				return filepath.SkipDir
 			}
 			return nil
 		}
 		if d.Type().IsRegular() && filepath.Ext(name) == ".go" && !strings.HasSuffix(name, "_test.go") {
 			dir := filepath.Dir(path)
 			if !seen[dir] {
-				pkg, err := build.ImportDir(dir, build.ImportComment)
+				pkg, err := ctxt.ImportDir(dir, build.ImportComment)
 				if err != nil {
 					return fmt.Errorf("%s: %s", dir, err)
 				}
 				if pkg.ImportPath == "" || pkg.ImportPath == "." {
 					importPath, err := filepath.Rel(wd, dir)
 					if err != nil {
 						t.Fatal(err)
```

### Comparing `fzf_bin-0.50.0/fzf/man/man1/fzf-tmux.1` & `fzf_bin-0.51.0/fzf/man/man1/fzf-tmux.1`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 ..
-.TH fzf-tmux 1 "Apr 2024" "fzf 0.50.0" "fzf-tmux - open fzf in tmux split pane"
+.TH fzf-tmux 1 "May 2024" "fzf 0.51.0" "fzf-tmux - open fzf in tmux split pane"
 
 .SH NAME
 fzf-tmux - open fzf in tmux split pane
 
 .SH SYNOPSIS
 .B fzf-tmux [LAYOUT OPTIONS] [--] [FZF OPTIONS]
```

### Comparing `fzf_bin-0.50.0/fzf/man/man1/fzf.1` & `fzf_bin-0.51.0/fzf/man/man1/fzf.1`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 ..
-.TH fzf 1 "Apr 2024" "fzf 0.50.0" "fzf - a command-line fuzzy finder"
+.TH fzf 1 "May 2024" "fzf 0.51.0" "fzf - a command-line fuzzy finder"
 
 .SH NAME
 fzf - a command-line fuzzy finder
 
 .SH SYNOPSIS
 fzf [options]
 
@@ -808,20 +808,30 @@
        tput rmcup
        exit 1
      ) && seq "$foo" 100 | fzf
 
 .TP
 .B "--sync"
 Synchronous search for multi-staged filtering. If specified, fzf will launch
-ncurses finder only after the input stream is complete.
+the finder only after the input stream is complete.
 
 .RS
 e.g. \fBfzf --multi | fzf --sync\fR
 .RE
 .TP
+.B "--with-shell=STR"
+Shell command and flags to start child processes with. On *nix Systems, the
+default value is \fB$SHELL -c\fR if \fB$SHELL\fR is set, otherwise \fBsh -c\fR.
+On Windows, the default value is \fBcmd /v:on/s/c\fR when \fB$SHELL\fR is not
+set.
+
+.RS
+e.g. \fBgem list | fzf --with-shell 'ruby -e' --preview 'pp Gem::Specification.find_by_name({1})'\fR
+.RE
+.TP
 .B "--listen[=[ADDR:]PORT]" "--listen-unsafe[=[ADDR:]PORT]"
 Start HTTP server and listen on the given address. It allows external processes
 to send actions to perform via POST method.
 
 - If the port number is omitted or given as 0, fzf will automatically choose
 a port and export it as \fBFZF_PORT\fR environment variable to the child processes
 
@@ -928,14 +938,16 @@
 .SH EXIT STATUS
 .BR 0 "      Normal exit"
 .br
 .BR 1 "      No match"
 .br
 .BR 2 "      Error"
 .br
+.BR 127 "    Invalid shell command for \fBbecome\fR action"
+.br
 .BR 130 "    Interrupted with \fBCTRL-C\fR or \fBESC\fR"
 
 .SH FIELD INDEX EXPRESSION
 
 A field index expression can be a non-zero integer or a range expression
 ([BEGIN]..[END]). \fB--nth\fR and \fB--with-nth\fR take a comma-separated list
 of field index expressions.
@@ -968,14 +980,16 @@
 .br
 .BR FZF_TOTAL_COUNT "     Total number of items"
 .br
 .BR FZF_MATCH_COUNT "     Number of matched items"
 .br
 .BR FZF_SELECT_COUNT "    Number of selected items"
 .br
+.BR FZF_POS "             Vertical position of the cursor in the list starting from 1"
+.br
 .BR FZF_QUERY "           Current query string"
 .br
 .BR FZF_PROMPT "          Prompt string"
 .br
 .BR FZF_PREVIEW_LABEL "   Preview label string"
 .br
 .BR FZF_BORDER_LABEL "    Border label string"
@@ -1278,14 +1292,16 @@
     \fBbackward-kill-word\fR           \fIalt-bs\fR
     \fBbackward-word\fR                \fIalt-b   shift-left\fR
     \fBbecome(...)\fR                  (replace fzf process with the specified command; see below for the details)
     \fBbeginning-of-line\fR            \fIctrl-a  home\fR
     \fBcancel\fR                       (clear query string if not empty, abort fzf otherwise)
     \fBchange-border-label(...)\fR     (change \fB--border-label\fR to the given string)
     \fBchange-header(...)\fR           (change header to the given string; doesn't affect \fB--header-lines\fR)
+    \fBchange-multi\fR                 (enable multi-select mode with no limit)
+    \fBchange-multi(...)\fR            (enable multi-select mode with a limit or disable it with 0)
     \fBchange-preview(...)\fR          (change \fB--preview\fR option)
     \fBchange-preview-label(...)\fR    (change \fB--preview-label\fR to the given string)
     \fBchange-preview-window(...)\fR   (change \fB--preview-window\fR option; rotate through the multiple option sets separated by '|')
     \fBchange-prompt(...)\fR           (change prompt to the given string)
     \fBchange-query(...)\fR            (change query string to the given string)
     \fBclear-screen\fR                 \fIctrl-l\fR
     \fBclear-selection\fR              (clear multi-selection)
@@ -1435,16 +1451,14 @@
 
 \fBbecome(...)\fR action is similar to \fBexecute(...)\fR, but it replaces the
 current fzf process with the specified command using \fBexecve(2)\fR system
 call.
 
     \fBfzf --bind "enter:become(vim {})"\fR
 
-\fBbecome(...)\fR is not supported on Windows.
-
 .SS RELOAD INPUT
 
 \fBreload(...)\fR action is used to dynamically update the input list
 without restarting fzf. It takes the same command template with placeholder
 expressions as \fBexecute(...)\fR.
 
 See \fIhttps://github.com/junegunn/fzf/issues/1750\fR for more info.
```

### Comparing `fzf_bin-0.50.0/fzf/plugin/fzf.vim` & `fzf_bin-0.51.0/fzf/plugin/fzf.vim`

 * *Files 2% similar despite different names*

```diff
@@ -79,20 +79,36 @@
   endfunction
 
   function! s:enc_to_cp(str)
     return a:str
   endfunction
 endif
 
+let s:cmd_control_chars = ['&', '|', '<', '>', '(', ')', '@', '^', '!']
+
 function! s:shellesc_cmd(arg)
-  let escaped = substitute(a:arg, '[&|<>()@^]', '^&', 'g')
-  let escaped = substitute(escaped, '%', '%%', 'g')
-  let escaped = substitute(escaped, '"', '\\^&', 'g')
-  let escaped = substitute(escaped, '\(\\\+\)\(\\^\)', '\1\1\2', 'g')
-  return '^"'.substitute(escaped, '\(\\\+\)$', '\1\1', '').'^"'
+  let e = '"'
+  let slashes = 0
+  for c in split(a:arg, '\zs')
+    if c ==# '\'
+      let slashes += 1
+    elseif c ==# '"'
+      let e .= repeat('\', slashes + 1)
+      let slashes = 0
+    elseif c ==# '%'
+      let e .= '%'
+    elseif index(s:cmd_control_chars, c) >= 0
+      let e .= '^'
+    else
+      let slashes = 0
+    endif
+    let e .= c
+  endfor
+  let e .= repeat('\', slashes) .'"'
+  return e
 endfunction
 
 function! fzf#shellescape(arg, ...)
   let shell = get(a:000, 0, s:is_win ? 'cmd.exe' : 'sh')
   if shell =~# 'cmd.exe$'
     return s:shellesc_cmd(a:arg)
   endif
```

### Comparing `fzf_bin-0.50.0/fzf/shell/completion.bash` & `fzf_bin-0.51.0/fzf/shell/completion.bash`

 * *Files 11% similar despite different names*

```diff
@@ -28,14 +28,22 @@
 #   }
 
 ###########################################################
 
 # To redraw line after fzf closes (printf '\e[5n')
 bind '"\e[0n": redraw-current-line' 2> /dev/null
 
+__fzf_defaults() {
+  # $1: Prepend to FZF_DEFAULT_OPTS_FILE and FZF_DEFAULT_OPTS
+  # $2: Append to FZF_DEFAULT_OPTS_FILE and FZF_DEFAULT_OPTS
+  echo "--height ${FZF_TMUX_HEIGHT:-40%} --bind=ctrl-z:ignore $1"
+  command cat "${FZF_DEFAULT_OPTS_FILE-}" 2> /dev/null
+  echo "${FZF_DEFAULT_OPTS-} $2"
+}
+
 __fzf_comprun() {
   if [[ "$(type -t _fzf_comprun 2>&1)" = function ]]; then
     _fzf_comprun "$@"
   elif [[ -n "${TMUX_PANE-}" ]] && { [[ "${FZF_TMUX:-0}" != 0 ]] || [[ -n "${FZF_TMUX_OPTS-}" ]]; }; then
     shift
     fzf-tmux ${FZF_TMUX_OPTS:--d${FZF_TMUX_HEIGHT:-40%}} -- "$@"
   else
@@ -88,136 +96,85 @@
 _fzf_opts_completion() {
   local cur prev opts
   COMPREPLY=()
   cur="${COMP_WORDS[COMP_CWORD]}"
   prev="${COMP_WORDS[COMP_CWORD-1]}"
   opts="
     -h --help
-    -x --extended
     -e --exact
-    --extended-exact
     +x --no-extended
-    +e --no-exact
     -q --query
     -f --filter
     --literal
-    --no-literal
-    --algo
     --scheme
     --expect
-    --no-expect
-    --enabled --no-phony
-    --disabled --phony
+    --disabled
     --tiebreak
     --bind
     --color
-    --toggle-sort
     -d --delimiter
     -n --nth
     --with-nth
-    -s --sort
     +s --no-sort
     --track
-    --no-track
     --tac
-    --no-tac
     -i
     +i
     -m --multi
-    +m --no-multi
     --ansi
-    --no-ansi
     --no-mouse
     +c --no-color
-    +2 --no-256
-    --black
-    --no-black
-    --bold
     --no-bold
     --layout
     --reverse
-    --no-reverse
     --cycle
-    --no-cycle
     --keep-right
-    --no-keep-right
-    --hscroll
     --no-hscroll
     --hscroll-off
     --scroll-off
     --filepath-word
-    --no-filepath-word
     --info
-    --no-info
-    --inline-info
-    --no-inline-info
     --separator
     --no-separator
-    --scrollbar
     --no-scrollbar
     --jump-labels
     -1 --select-1
-    +1 --no-select-1
     -0 --exit-0
-    +0 --no-exit-0
     --read0
-    --no-read0
     --print0
-    --no-print0
     --print-query
-    --no-print-query
     --prompt
     --pointer
     --marker
     --sync
-    --no-sync
-    --async
-    --no-history
     --history
     --history-size
-    --no-header
-    --no-header-lines
     --header
     --header-lines
     --header-first
-    --no-header-first
     --ellipsis
     --preview
-    --no-preview
     --preview-window
     --height
     --min-height
-    --no-height
-    --no-margin
-    --no-padding
-    --no-border
     --border
-    --no-border-label
     --border-label
     --border-label-pos
-    --no-preview-label
     --preview-label
     --preview-label-pos
     --no-unicode
-    --unicode
     --margin
     --padding
     --tabstop
     --listen
-    --no-listen
-    --clear
     --no-clear
     --version
     --"
 
   case "${prev}" in
-  --algo)
-    COMPREPLY=( $(compgen -W "v1 v2" -- "$cur") )
-    return 0
-    ;;
   --scheme)
     COMPREPLY=( $(compgen -W "default path history" -- "$cur") )
     return 0
     ;;
   --tiebreak)
     COMPREPLY=( $(compgen -W "length chunk begin end index" -- "$cur") )
     return 0
@@ -331,16 +288,16 @@
     while true; do
       if [[ -z "$dir" ]] || [[ -d "$dir" ]]; then
         leftover=${base/#"$dir"}
         leftover=${leftover/#\/}
         [[ -z "$dir" ]] && dir='.'
         [[ "$dir" != "/" ]] && dir="${dir/%\//}"
         matches=$(
-          unset FZF_DEFAULT_COMMAND
-          export FZF_DEFAULT_OPTS="--height ${FZF_TMUX_HEIGHT:-40%} --reverse --scheme=path --bind=ctrl-z:ignore ${FZF_DEFAULT_OPTS-} ${FZF_COMPLETION_OPTS-} $2"
+          export FZF_DEFAULT_OPTS=$(__fzf_defaults "--reverse --scheme=path" "${FZF_COMPLETION_OPTS-} $2")
+          unset FZF_DEFAULT_COMMAND FZF_DEFAULT_OPTS_FILE
           if declare -F "$1" > /dev/null; then
             eval "$1 $(printf %q "$dir")" | __fzf_comprun "$4" -q "$leftover"
           else
             [[ $1 =~ dir ]] && walker=dir,follow || walker=file,dir,follow,hidden
             __fzf_comprun "$4" -q "$leftover" --walker "$walker" --walker-root="$dir"
           fi | while read -r item; do
             printf "%q " "${item%$3}$3"
@@ -395,15 +352,18 @@
 
   trigger=${FZF_COMPLETION_TRIGGER-'**'}
   cmd="${COMP_WORDS[0]}"
   cur="${COMP_WORDS[COMP_CWORD]}"
   if [[ "$cur" == *"$trigger" ]] && [[ $cur != *'$('* ]] && [[ $cur != *':='* ]] && [[ $cur != *'`'* ]]; then
     cur=${cur:0:${#cur}-${#trigger}}
 
-    selected=$(FZF_DEFAULT_OPTS="--height ${FZF_TMUX_HEIGHT:-40%} --reverse --bind=ctrl-z:ignore ${FZF_DEFAULT_OPTS-} ${FZF_COMPLETION_OPTS-} $str_arg" __fzf_comprun "${rest[0]}" "${args[@]}" -q "$cur" | $post | command tr '\n' ' ')
+    selected=$(
+      FZF_DEFAULT_OPTS=$(__fzf_defaults "--reverse" "${FZF_COMPLETION_OPTS-} $str_arg") \
+      FZF_DEFAULT_OPTS_FILE='' \
+        __fzf_comprun "${rest[0]}" "${args[@]}" -q "$cur" | $post | command tr '\n' ' ')
     selected=${selected% } # Strip trailing space not to repeat "-o nospace"
     if [[ -n "$selected" ]]; then
       COMPREPLY=("$selected")
     else
       COMPREPLY=("$cur")
     fi
     printf '\e[5n'
@@ -499,27 +459,31 @@
 # fzf options
 complete -o default -F _fzf_opts_completion fzf
 # fzf-tmux is a thin fzf wrapper that has only a few more options than fzf
 # itself. As a quick improvement we take fzf's completion. Adding the few extra
 # fzf-tmux specific options (like `-w WIDTH`) are left as a future patch.
 complete -o default -F _fzf_opts_completion fzf-tmux
 
-d_cmds="${FZF_COMPLETION_DIR_COMMANDS:-cd pushd rmdir}"
-a_cmds="
+d_cmds="${FZF_COMPLETION_DIR_COMMANDS-cd pushd rmdir}"
+
+# NOTE: $FZF_COMPLETION_PATH_COMMANDS and $FZF_COMPLETION_VAR_COMMANDS are
+# undocumented and subject to change in the future.
+a_cmds="${FZF_COMPLETION_PATH_COMMANDS-"
   awk bat cat diff diff3
   emacs emacsclient ex file ftp g++ gcc gvim head hg hx java
   javac ld less more mvim nvim patch perl python ruby
   sed sftp sort source tail tee uniq vi view vim wc xdg-open
   basename bunzip2 bzip2 chmod chown curl cp dirname du
   find git grep gunzip gzip hg jar
   ln ls mv open rm rsync scp
-  svn tar unzip zip"
+  svn tar unzip zip"}"
+v_cmds="${FZF_COMPLETION_VAR_COMMANDS-export unset printenv}"
 
 # Preserve existing completion
-__fzf_orig_completion < <(complete -p $d_cmds $a_cmds ssh 2> /dev/null)
+__fzf_orig_completion < <(complete -p $d_cmds $a_cmds $v_cmds unalias kill ssh 2> /dev/null)
 
 if type _comp_load > /dev/null 2>&1; then
   # _comp_load was added in bash-completion 2.12 to replace _completion_loader.
   # We use it without -D option so that it does not use _comp_complete_minimal as the fallback.
   _fzf_completion_loader=_comp_load
 elif type __load_completion > /dev/null 2>&1; then
   # In bash-completion 2.11, _completion_loader internally calls __load_completion
@@ -547,18 +511,29 @@
 done
 
 # Directory
 for cmd in $d_cmds; do
   __fzf_defc "$cmd" _fzf_dir_completion "-o bashdefault -o nospace -o dirnames"
 done
 
+# Variables
+for cmd in $v_cmds; do
+  __fzf_defc "$cmd" _fzf_var_completion "-o default -o nospace -v"
+done
+
+# Aliases
+__fzf_defc unalias _fzf_alias_completion "-a"
+
+# Processes
+__fzf_defc kill _fzf_proc_completion "-o default -o bashdefault"
+
 # ssh
 __fzf_defc ssh _fzf_complete_ssh "-o default -o bashdefault"
 
-unset cmd d_cmds a_cmds
+unset cmd d_cmds a_cmds v_cmds
 
 _fzf_setup_completion() {
   local kind fn cmd
   kind=$1
   fn=_fzf_${1}_completion
   if [[ $# -lt 2 ]] || ! type -t "$fn" > /dev/null; then
     echo "usage: ${FUNCNAME[0]} path|dir|var|alias|host|proc COMMANDS..."
@@ -572,14 +547,8 @@
       var)   __fzf_defc "$cmd" "$fn" "-o default -o nospace -v" ;;
       alias) __fzf_defc "$cmd" "$fn" "-a" ;;
       *)     __fzf_defc "$cmd" "$fn" "-o default -o bashdefault" ;;
     esac
   done
 }
 
-# Environment variables / Aliases / Hosts / Process
-_fzf_setup_completion 'var'   export unset printenv
-_fzf_setup_completion 'alias' unalias
-_fzf_setup_completion 'host'  telnet
-_fzf_setup_completion 'proc'  kill
-
 fi
```

### Comparing `fzf_bin-0.50.0/fzf/shell/completion.zsh` & `fzf_bin-0.51.0/fzf/shell/completion.zsh`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 # /_/   /___/_/ completion.zsh
 #
 # - $FZF_TMUX               (default: 0)
 # - $FZF_TMUX_OPTS          (default: '-d 40%')
 # - $FZF_COMPLETION_TRIGGER (default: '**')
 # - $FZF_COMPLETION_OPTS    (default: empty)
 
-if [[ -o interactive ]]; then
-
 
 # Both branches of the following `if` do the same thing -- define
 # __fzf_completion_options such that `eval $__fzf_completion_options` sets
 # all options to the same values they currently have. We'll do just that at
 # the bottom of the file after changing options to what we prefer.
 #
 # IMPORTANT: Until we get to the `emulate` line, all words that *can* be quoted
@@ -71,14 +69,17 @@
 # to values we don't expect. With the following `emulate` command we
 # sidestep this issue entirely.
 'builtin' 'emulate' 'zsh' && 'builtin' 'setopt' 'no_aliases'
 
 # This brace is the start of try-always block. The `always` part is like
 # `finally` in lesser languages. We use it to *always* restore user options.
 {
+# The 'emulate' command should not be placed inside the interactive if check;
+# placing it there fails to disable alias expansion. See #3731.
+if [[ -o interactive ]]; then
 
 # To use custom commands instead of find, override _fzf_compgen_{path,dir}
 #
 #   _fzf_compgen_path() {
 #     echo "$1"
 #     command find -L "$1" \
 #       -name .git -prune -o -name .hg -prune -o -name .svn -prune -o \( -type d -o -type f -o -type l \) \
@@ -89,14 +90,22 @@
 #     command find -L "$1" \
 #       -name .git -prune -o -name .hg -prune -o -name .svn -prune -o -type d \
 #       -a -not -path "$1" -print 2> /dev/null | sed 's@^\./@@'
 #   }
 
 ###########################################################
 
+__fzf_defaults() {
+  # $1: Prepend to FZF_DEFAULT_OPTS_FILE and FZF_DEFAULT_OPTS
+  # $2: Append to FZF_DEFAULT_OPTS_FILE and FZF_DEFAULT_OPTS
+  echo "--height ${FZF_TMUX_HEIGHT:-40%} --bind=ctrl-z:ignore $1"
+  command cat "${FZF_DEFAULT_OPTS_FILE-}" 2> /dev/null
+  echo "${FZF_DEFAULT_OPTS-} $2"
+}
+
 __fzf_comprun() {
   if [[ "$(type _fzf_comprun 2>&1)" =~ function ]]; then
     _fzf_comprun "$@"
   elif [ -n "${TMUX_PANE-}" ] && { [ "${FZF_TMUX:-0}" != 0 ] || [ -n "${FZF_TMUX_OPTS-}" ]; }; then
     shift
     if [ -n "${FZF_TMUX_OPTS-}" ]; then
       fzf-tmux ${(Q)${(Z+n+)FZF_TMUX_OPTS}} -- "$@"
@@ -142,16 +151,16 @@
   while [ 1 ]; do
     if [[ -z "$dir" || -d ${dir} ]]; then
       leftover=${base/#"$dir"}
       leftover=${leftover/#\/}
       [ -z "$dir" ] && dir='.'
       [ "$dir" != "/" ] && dir="${dir/%\//}"
       matches=$(
-        unset FZF_DEFAULT_COMMAND
-        export FZF_DEFAULT_OPTS="--height ${FZF_TMUX_HEIGHT:-40%} --reverse --scheme=path --bind=ctrl-z:ignore ${FZF_DEFAULT_OPTS-} ${FZF_COMPLETION_OPTS-}"
+        export FZF_DEFAULT_OPTS=$(__fzf_defaults "--reverse --scheme=path" "${FZF_COMPLETION_OPTS-}")
+        unset FZF_DEFAULT_COMMAND FZF_DEFAULT_OPTS_FILE
         if declare -f "$compgen" > /dev/null; then
           eval "$compgen $(printf %q "$dir")" | __fzf_comprun "$cmd" ${(Q)${(Z+n+)fzf_opts}} -q "$leftover"
         else
           [[ $compgen =~ dir ]] && walker=dir,follow || walker=file,dir,follow,hidden
           __fzf_comprun "$cmd" ${(Q)${(Z+n+)fzf_opts}} -q "$leftover" --walker "$walker" --walker-root="$dir" < /dev/tty
         fi | while read item; do
           item="${item%$suffix}$suffix"
@@ -213,15 +222,18 @@
   fifo="${TMPDIR:-/tmp}/fzf-complete-fifo-$$"
   lbuf=${rest[0]}
   cmd=$(__fzf_extract_command "$lbuf")
   post="${funcstack[1]}_post"
   type $post > /dev/null 2>&1 || post=cat
 
   _fzf_feed_fifo "$fifo"
-  matches=$(FZF_DEFAULT_OPTS="--height ${FZF_TMUX_HEIGHT:-40%} --reverse --bind=ctrl-z:ignore ${FZF_DEFAULT_OPTS-} ${FZF_COMPLETION_OPTS-} $str_arg" __fzf_comprun "$cmd" "${args[@]}" -q "${(Q)prefix}" < "$fifo" | $post | tr '\n' ' ')
+  matches=$(
+    FZF_DEFAULT_OPTS=$(__fzf_defaults "--reverse" "${FZF_COMPLETION_OPTS-} $str_arg") \
+    FZF_DEFAULT_OPTS_FILE='' \
+      __fzf_comprun "$cmd" "${args[@]}" -q "${(Q)prefix}" < "$fifo" | $post | tr '\n' ' ')
   if [ -n "$matches" ]; then
     LBUFFER="$lbuf$matches"
   fi
   command rm -f "$fifo"
 }
 
 # To use custom hostname lists, override __fzf_list_hosts.
@@ -311,15 +323,15 @@
   fi
 
   lbuf=$LBUFFER
   tail=${LBUFFER:$(( ${#LBUFFER} - ${#trigger} ))}
 
   # Trigger sequence given
   if [ ${#tokens} -gt 1 -a "$tail" = "$trigger" ]; then
-    d_cmds=(${=FZF_COMPLETION_DIR_COMMANDS:-cd pushd rmdir})
+    d_cmds=(${=FZF_COMPLETION_DIR_COMMANDS-cd pushd rmdir})
 
     [ -z "$trigger"      ] && prefix=${tokens[-1]} || prefix=${tokens[-1]:0:-${#trigger}}
     if [[ $prefix = *'$('* ]] || [[ $prefix = *'<('* ]] || [[ $prefix = *'>('* ]] || [[ $prefix = *':='* ]] || [[ $prefix = *'`'* ]]; then
       return
     fi
     [ -n "${tokens[-1]}" ] && lbuf=${lbuf:0:-${#tokens[-1]}}
 
@@ -341,15 +353,14 @@
   binding=$(bindkey '^I')
   [[ $binding =~ 'undefined-key' ]] || fzf_default_completion=$binding[(s: :w)2]
   unset binding
 }
 
 zle     -N   fzf-completion
 bindkey '^I' fzf-completion
+fi
 
 } always {
   # Restore the original options.
   eval $__fzf_completion_options
   'unset' '__fzf_completion_options'
 }
-
-fi
```

### Comparing `fzf_bin-0.50.0/fzf/shell/key-bindings.bash` & `fzf_bin-0.51.0/fzf/shell/key-bindings.bash`

 * *Files 22% similar despite different names*

```diff
@@ -12,18 +12,27 @@
 # - $FZF_ALT_C_OPTS
 
 if [[ $- =~ i ]]; then
 
 
 # Key bindings
 # ------------
+
+__fzf_defaults() {
+  # $1: Prepend to FZF_DEFAULT_OPTS_FILE and FZF_DEFAULT_OPTS
+  # $2: Append to FZF_DEFAULT_OPTS_FILE and FZF_DEFAULT_OPTS
+  echo "--height ${FZF_TMUX_HEIGHT:-40%} --bind=ctrl-z:ignore $1"
+  command cat "${FZF_DEFAULT_OPTS_FILE-}" 2> /dev/null
+  echo "${FZF_DEFAULT_OPTS-} $2"
+}
+
 __fzf_select__() {
-  local opts
-  opts="--height ${FZF_TMUX_HEIGHT:-40%} --bind=ctrl-z:ignore --reverse --walker=file,dir,follow,hidden --scheme=path ${FZF_DEFAULT_OPTS-} ${FZF_CTRL_T_OPTS-} -m"
-  FZF_DEFAULT_COMMAND=${FZF_CTRL_T_COMMAND:-} FZF_DEFAULT_OPTS="$opts" $(__fzfcmd) "$@" |
+  FZF_DEFAULT_COMMAND=${FZF_CTRL_T_COMMAND:-} \
+  FZF_DEFAULT_OPTS=$(__fzf_defaults "--reverse --walker=file,dir,follow,hidden --scheme=path" "${FZF_CTRL_T_OPTS-} -m") \
+  FZF_DEFAULT_OPTS_FILE='' $(__fzfcmd) "$@" |
     while read -r item; do
       printf '%q ' "$item"  # escape special chars
     done
 }
 
 __fzfcmd() {
   [[ -n "${TMUX_PANE-}" ]] && { [[ "${FZF_TMUX:-0}" != 0 ]] || [[ -n "${FZF_TMUX_OPTS-}" ]]; } &&
@@ -33,60 +42,61 @@
 fzf-file-widget() {
   local selected="$(__fzf_select__ "$@")"
   READLINE_LINE="${READLINE_LINE:0:$READLINE_POINT}$selected${READLINE_LINE:$READLINE_POINT}"
   READLINE_POINT=$(( READLINE_POINT + ${#selected} ))
 }
 
 __fzf_cd__() {
-  local opts dir
-  opts="--height ${FZF_TMUX_HEIGHT:-40%} --bind=ctrl-z:ignore --reverse --walker=dir,follow,hidden --scheme=path ${FZF_DEFAULT_OPTS-} ${FZF_ALT_C_OPTS-} +m"
+  local dir
   dir=$(
-    FZF_DEFAULT_COMMAND=${FZF_ALT_C_COMMAND:-} FZF_DEFAULT_OPTS="$opts" $(__fzfcmd)
+    FZF_DEFAULT_COMMAND=${FZF_ALT_C_COMMAND:-} \
+    FZF_DEFAULT_OPTS=$(__fzf_defaults "--reverse --walker=dir,follow,hidden --scheme=path" "${FZF_ALT_C_OPTS-} +m") \
+    FZF_DEFAULT_OPTS_FILE='' $(__fzfcmd)
   ) && printf 'builtin cd -- %q' "$(builtin unset CDPATH && builtin cd -- "$dir" && builtin pwd)"
 }
 
 if command -v perl > /dev/null; then
   __fzf_history__() {
-    local output opts script
-    opts="--height ${FZF_TMUX_HEIGHT:-40%} --bind=ctrl-z:ignore ${FZF_DEFAULT_OPTS-} -n2..,.. --scheme=history --bind=ctrl-r:toggle-sort ${FZF_CTRL_R_OPTS-} +m --read0"
+    local output script
     script='BEGIN { getc; $/ = "\n\t"; $HISTCOUNT = $ENV{last_hist} + 1 } s/^[ *]//; print $HISTCOUNT - $. . "\t$_" if !$seen{$_}++'
     output=$(
       set +o pipefail
       builtin fc -lnr -2147483648 |
         last_hist=$(HISTTIMEFORMAT='' builtin history 1) command perl -n -l0 -e "$script" |
-        FZF_DEFAULT_OPTS="$opts" $(__fzfcmd) --query "$READLINE_LINE"
+        FZF_DEFAULT_OPTS=$(__fzf_defaults "" "-n2..,.. --scheme=history --bind=ctrl-r:toggle-sort ${FZF_CTRL_R_OPTS-} +m --read0") \
+        FZF_DEFAULT_OPTS_FILE='' $(__fzfcmd) --query "$READLINE_LINE"
     ) || return
     READLINE_LINE=${output#*$'\t'}
     if [[ -z "$READLINE_POINT" ]]; then
       echo "$READLINE_LINE"
     else
       READLINE_POINT=0x7fffffff
     fi
   }
 else # awk - fallback for POSIX systems
   __fzf_history__() {
-    local output opts script n x y z d
+    local output script n x y z d
     if [[ -z $__fzf_awk ]]; then
       __fzf_awk=awk
       # choose the faster mawk if: it's installed && build date >= 20230322 && version >= 1.3.4
       IFS=' .' read n x y z d <<< $(command mawk -W version 2> /dev/null)
       [[ $n == mawk ]] && (( d >= 20230302 && (x *1000 +y) *1000 +z >= 1003004 )) && __fzf_awk=mawk
     fi
-    opts="--height ${FZF_TMUX_HEIGHT:-40%} --bind=ctrl-z:ignore ${FZF_DEFAULT_OPTS-} -n2..,.. --scheme=history --bind=ctrl-r:toggle-sort ${FZF_CTRL_R_OPTS-} +m --read0"
     [[ $(HISTTIMEFORMAT='' builtin history 1) =~ [[:digit:]]+ ]]    # how many history entries
     script='function P(b) { ++n; sub(/^[ *]/, "", b); if (!seen[b]++) { printf "%d\t%s%c", '$((BASH_REMATCH + 1))' - n, b, 0 } }
     NR==1 { b = substr($0, 2); next }
     /^\t/ { P(b); b = substr($0, 2); next }
     { b = b RS $0 }
     END { if (NR) P(b) }'
     output=$(
       set +o pipefail
       builtin fc -lnr -2147483648 2> /dev/null |   # ( $'\t '<lines>$'\n' )* ; <lines> ::= [^\n]* ( $'\n'<lines> )*
         command $__fzf_awk "$script"           |   # ( <counter>$'\t'<lines>$'\000' )*
-        FZF_DEFAULT_OPTS="$opts" $(__fzfcmd) --query "$READLINE_LINE"
+        FZF_DEFAULT_OPTS=$(__fzf_defaults "" "-n2..,.. --scheme=history --bind=ctrl-r:toggle-sort ${FZF_CTRL_R_OPTS-} +m --read0") \
+        FZF_DEFAULT_OPTS_FILE='' $(__fzfcmd) --query "$READLINE_LINE"
     ) || return
     READLINE_LINE=${output#*$'\t'}
     if [[ -z "$READLINE_POINT" ]]; then
       echo "$READLINE_LINE"
     else
       READLINE_POINT=0x7fffffff
     fi
```

### Comparing `fzf_bin-0.50.0/fzf/shell/key-bindings.fish` & `fzf_bin-0.51.0/fzf/shell/key-bindings.fish`

 * *Files 8% similar despite different names*

```diff
@@ -14,25 +14,35 @@
 status is-interactive; or exit 0
 
 
 # Key bindings
 # ------------
 function fzf_key_bindings
 
+  function __fzf_defaults
+    # $1: Prepend to FZF_DEFAULT_OPTS_FILE and FZF_DEFAULT_OPTS
+    # $2: Append to FZF_DEFAULT_OPTS_FILE and FZF_DEFAULT_OPTS
+    test -n "$FZF_TMUX_HEIGHT"; or set FZF_TMUX_HEIGHT 40%
+    echo "--height $FZF_TMUX_HEIGHT --bind=ctrl-z:ignore" $argv[1]
+    command cat "$FZF_DEFAULT_OPTS_FILE" 2> /dev/null
+    echo $FZF_DEFAULT_OPTS $argv[2]
+  end
+
   # Store current token in $dir as root for the 'find' command
   function fzf-file-widget -d "List files and folders"
     set -l commandline (__fzf_parse_commandline)
     set -lx dir $commandline[1]
     set -l fzf_query $commandline[2]
     set -l prefix $commandline[3]
 
     test -n "$FZF_TMUX_HEIGHT"; or set FZF_TMUX_HEIGHT 40%
     begin
-      set -lx FZF_DEFAULT_OPTS "--height $FZF_TMUX_HEIGHT --reverse --walker=file,dir,follow,hidden --walker-root='$dir' --scheme=path --bind=ctrl-z:ignore $FZF_DEFAULT_OPTS $FZF_CTRL_T_OPTS"
+      set -lx FZF_DEFAULT_OPTS (__fzf_defaults "--reverse --walker=file,dir,follow,hidden --scheme=path --walker-root='$dir'" "$FZF_CTRL_T_OPTS")
       set -lx FZF_DEFAULT_COMMAND "$FZF_CTRL_T_COMMAND"
+      set -lx FZF_DEFAULT_OPTS_FILE ''
       eval (__fzfcmd)' -m --query "'$fzf_query'"' | while read -l r; set result $result $r; end
     end
     if [ -z "$result" ]
       commandline -f repaint
       return
     else
       # Remove last token from commandline.
@@ -45,15 +55,16 @@
     end
     commandline -f repaint
   end
 
   function fzf-history-widget -d "Show command history"
     test -n "$FZF_TMUX_HEIGHT"; or set FZF_TMUX_HEIGHT 40%
     begin
-      set -lx FZF_DEFAULT_OPTS "--height $FZF_TMUX_HEIGHT $FZF_DEFAULT_OPTS --scheme=history --bind=ctrl-r:toggle-sort,ctrl-z:ignore $FZF_CTRL_R_OPTS +m"
+      set -lx FZF_DEFAULT_OPTS (__fzf_defaults "" "--scheme=history --bind=ctrl-r:toggle-sort $FZF_CTRL_R_OPTS +m")
+      set -lx FZF_DEFAULT_OPTS_FILE ''
 
       set -l FISH_MAJOR (echo $version | cut -f1 -d.)
       set -l FISH_MINOR (echo $version | cut -f2 -d.)
 
       # history's -z flag is needed for multi-line support.
       # history's -z flag was added in fish 2.4.0, so don't use it for versions
       # before 2.4.0.
@@ -72,15 +83,16 @@
     set -l commandline (__fzf_parse_commandline)
     set -lx dir $commandline[1]
     set -l fzf_query $commandline[2]
     set -l prefix $commandline[3]
 
     test -n "$FZF_TMUX_HEIGHT"; or set FZF_TMUX_HEIGHT 40%
     begin
-      set -lx FZF_DEFAULT_OPTS "--height $FZF_TMUX_HEIGHT --reverse --walker=dir,follow,hidden --walker-root='$dir' --scheme=path --bind=ctrl-z:ignore $FZF_DEFAULT_OPTS $FZF_ALT_C_OPTS"
+      set -lx FZF_DEFAULT_OPTS (__fzf_defaults "--reverse --walker=dir,follow,hidden --scheme=path --walker-root='$dir'" "$FZF_ALT_C_OPTS")
+      set -lx FZF_DEFAULT_OPTS_FILE ''
       set -lx FZF_DEFAULT_COMMAND "$FZF_ALT_C_COMMAND"
       eval (__fzfcmd)' +m --query "'$fzf_query'"' | read -l result
 
       if [ -n "$result" ]
         cd -- $result
 
         # Remove last token from commandline.
```

### Comparing `fzf_bin-0.50.0/fzf/shell/key-bindings.zsh` & `fzf_bin-0.51.0/fzf/shell/key-bindings.zsh`

 * *Files 10% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # - $FZF_TMUX_OPTS
 # - $FZF_CTRL_T_COMMAND
 # - $FZF_CTRL_T_OPTS
 # - $FZF_CTRL_R_OPTS
 # - $FZF_ALT_C_COMMAND
 # - $FZF_ALT_C_OPTS
 
-if [[ -o interactive ]]; then
-
 
 # Key bindings
 # ------------
 
 # The code at the top and the bottom of this file is the same as in completion.zsh.
 # Refer to that file for explanation.
 if 'zmodload' 'zsh/parameter' 2>'/dev/null' && (( ${+options} )); then
@@ -34,49 +32,63 @@
     done
   }
 fi
 
 'builtin' 'emulate' 'zsh' && 'builtin' 'setopt' 'no_aliases'
 
 {
+if [[ -o interactive ]]; then
+
+__fzf_defaults() {
+  # $1: Prepend to FZF_DEFAULT_OPTS_FILE and FZF_DEFAULT_OPTS
+  # $2: Append to FZF_DEFAULT_OPTS_FILE and FZF_DEFAULT_OPTS
+  echo "--height ${FZF_TMUX_HEIGHT:-40%} --bind=ctrl-z:ignore $1"
+  command cat "${FZF_DEFAULT_OPTS_FILE-}" 2> /dev/null
+  echo "${FZF_DEFAULT_OPTS-} $2"
+}
 
 # CTRL-T - Paste the selected file path(s) into the command line
-__fsel() {
+__fzf_select() {
   setopt localoptions pipefail no_aliases 2> /dev/null
   local item
-  FZF_DEFAULT_COMMAND=${FZF_CTRL_T_COMMAND:-} FZF_DEFAULT_OPTS="--height ${FZF_TMUX_HEIGHT:-40%} --reverse --walker=file,dir,follow,hidden --scheme=path --bind=ctrl-z:ignore ${FZF_DEFAULT_OPTS-} ${FZF_CTRL_T_OPTS-}" $(__fzfcmd) -m "$@" < /dev/tty | while read item; do
+  FZF_DEFAULT_COMMAND=${FZF_CTRL_T_COMMAND:-} \
+  FZF_DEFAULT_OPTS=$(__fzf_defaults "--reverse --walker=file,dir,follow,hidden --scheme=path" "${FZF_CTRL_T_OPTS-} -m") \
+  FZF_DEFAULT_OPTS_FILE='' $(__fzfcmd) "$@" < /dev/tty | while read item; do
     echo -n "${(q)item} "
   done
   local ret=$?
   echo
   return $ret
 }
 
 __fzfcmd() {
   [ -n "${TMUX_PANE-}" ] && { [ "${FZF_TMUX:-0}" != 0 ] || [ -n "${FZF_TMUX_OPTS-}" ]; } &&
     echo "fzf-tmux ${FZF_TMUX_OPTS:--d${FZF_TMUX_HEIGHT:-40%}} -- " || echo "fzf"
 }
 
 fzf-file-widget() {
-  LBUFFER="${LBUFFER}$(__fsel)"
+  LBUFFER="${LBUFFER}$(__fzf_select)"
   local ret=$?
   zle reset-prompt
   return $ret
 }
 if [[ "${FZF_CTRL_T_COMMAND-x}" != "" ]]; then
   zle     -N            fzf-file-widget
   bindkey -M emacs '^T' fzf-file-widget
   bindkey -M vicmd '^T' fzf-file-widget
   bindkey -M viins '^T' fzf-file-widget
 fi
 
 # ALT-C - cd into the selected directory
 fzf-cd-widget() {
   setopt localoptions pipefail no_aliases 2> /dev/null
-  local dir="$(FZF_DEFAULT_COMMAND=${FZF_ALT_C_COMMAND:-} FZF_DEFAULT_OPTS="--height ${FZF_TMUX_HEIGHT:-40%} --reverse --walker=dir,follow,hidden --scheme=path --bind=ctrl-z:ignore ${FZF_DEFAULT_OPTS-} ${FZF_ALT_C_OPTS-}" $(__fzfcmd) +m < /dev/tty)"
+  local dir="$(
+    FZF_DEFAULT_COMMAND=${FZF_ALT_C_COMMAND:-} \
+    FZF_DEFAULT_OPTS=$(__fzf_defaults "--reverse --walker=dir,follow,hidden --scheme=path" "${FZF_ALT_C_OPTS-} +m") \
+    FZF_DEFAULT_OPTS_FILE='' $(__fzfcmd) < /dev/tty)"
   if [[ -z "$dir" ]]; then
     zle redisplay
     return 0
   fi
   zle push-line # Clear buffer. Auto-restored on next prompt.
   BUFFER="builtin cd -- ${(q)dir:a}"
   zle accept-line
@@ -93,15 +105,16 @@
 fi
 
 # CTRL-R - Paste the selected command from history into the command line
 fzf-history-widget() {
   local selected num
   setopt localoptions noglobsubst noposixbuiltins pipefail no_aliases 2> /dev/null
   selected="$(fc -rl 1 | awk '{ cmd=$0; sub(/^[ \t]*[0-9]+\**[ \t]+/, "", cmd); if (!seen[cmd]++) print $0 }' |
-    FZF_DEFAULT_OPTS="--height ${FZF_TMUX_HEIGHT:-40%} ${FZF_DEFAULT_OPTS-} -n2..,.. --scheme=history --bind=ctrl-r:toggle-sort,ctrl-z:ignore ${FZF_CTRL_R_OPTS-} --query=${(qqq)LBUFFER} +m" $(__fzfcmd))"
+    FZF_DEFAULT_OPTS=$(__fzf_defaults "" "-n2..,.. --scheme=history --bind=ctrl-r:toggle-sort ${FZF_CTRL_R_OPTS-} --query=${(qqq)LBUFFER} +m") \
+    FZF_DEFAULT_OPTS_FILE='' $(__fzfcmd))"
   local ret=$?
   if [ -n "$selected" ]; then
     num=$(awk '{print $1}' <<< "$selected")
     if [[ "$num" =~ '^[1-9][0-9]*\*?$' ]]; then
       zle vi-fetch-history -n ${num%\*}
     else # selected is a custom query, not from history
       LBUFFER="$selected"
@@ -110,14 +123,13 @@
   zle reset-prompt
   return $ret
 }
 zle     -N            fzf-history-widget
 bindkey -M emacs '^R' fzf-history-widget
 bindkey -M vicmd '^R' fzf-history-widget
 bindkey -M viins '^R' fzf-history-widget
+fi
 
 } always {
   eval $__fzf_key_bindings_options
   'unset' '__fzf_key_bindings_options'
 }
-
-fi
```

### Comparing `fzf_bin-0.50.0/fzf/src/LICENSE` & `fzf_bin-0.51.0/fzf/src/LICENSE`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/actiontype_string.go` & `fzf_bin-0.51.0/fzf/src/actiontype_string.go`

 * *Files 10% similar despite different names*

```diff
@@ -22,110 +22,111 @@
 	_ = x[actBackwardChar-11]
 	_ = x[actBackwardDeleteChar-12]
 	_ = x[actBackwardDeleteCharEof-13]
 	_ = x[actBackwardWord-14]
 	_ = x[actCancel-15]
 	_ = x[actChangeBorderLabel-16]
 	_ = x[actChangeHeader-17]
-	_ = x[actChangePreviewLabel-18]
-	_ = x[actChangePrompt-19]
-	_ = x[actChangeQuery-20]
-	_ = x[actClearScreen-21]
-	_ = x[actClearQuery-22]
-	_ = x[actClearSelection-23]
-	_ = x[actClose-24]
-	_ = x[actDeleteChar-25]
-	_ = x[actDeleteCharEof-26]
-	_ = x[actEndOfLine-27]
-	_ = x[actForwardChar-28]
-	_ = x[actForwardWord-29]
-	_ = x[actKillLine-30]
-	_ = x[actKillWord-31]
-	_ = x[actUnixLineDiscard-32]
-	_ = x[actUnixWordRubout-33]
-	_ = x[actYank-34]
-	_ = x[actBackwardKillWord-35]
-	_ = x[actSelectAll-36]
-	_ = x[actDeselectAll-37]
-	_ = x[actToggle-38]
-	_ = x[actToggleSearch-39]
-	_ = x[actToggleAll-40]
-	_ = x[actToggleDown-41]
-	_ = x[actToggleUp-42]
-	_ = x[actToggleIn-43]
-	_ = x[actToggleOut-44]
-	_ = x[actToggleTrack-45]
-	_ = x[actToggleTrackCurrent-46]
-	_ = x[actToggleHeader-47]
-	_ = x[actTrackCurrent-48]
-	_ = x[actUntrackCurrent-49]
-	_ = x[actDown-50]
-	_ = x[actUp-51]
-	_ = x[actPageUp-52]
-	_ = x[actPageDown-53]
-	_ = x[actPosition-54]
-	_ = x[actHalfPageUp-55]
-	_ = x[actHalfPageDown-56]
-	_ = x[actOffsetUp-57]
-	_ = x[actOffsetDown-58]
-	_ = x[actJump-59]
-	_ = x[actJumpAccept-60]
-	_ = x[actPrintQuery-61]
-	_ = x[actRefreshPreview-62]
-	_ = x[actReplaceQuery-63]
-	_ = x[actToggleSort-64]
-	_ = x[actShowPreview-65]
-	_ = x[actHidePreview-66]
-	_ = x[actTogglePreview-67]
-	_ = x[actTogglePreviewWrap-68]
-	_ = x[actTransform-69]
-	_ = x[actTransformBorderLabel-70]
-	_ = x[actTransformHeader-71]
-	_ = x[actTransformPreviewLabel-72]
-	_ = x[actTransformPrompt-73]
-	_ = x[actTransformQuery-74]
-	_ = x[actPreview-75]
-	_ = x[actChangePreview-76]
-	_ = x[actChangePreviewWindow-77]
-	_ = x[actPreviewTop-78]
-	_ = x[actPreviewBottom-79]
-	_ = x[actPreviewUp-80]
-	_ = x[actPreviewDown-81]
-	_ = x[actPreviewPageUp-82]
-	_ = x[actPreviewPageDown-83]
-	_ = x[actPreviewHalfPageUp-84]
-	_ = x[actPreviewHalfPageDown-85]
-	_ = x[actPrevHistory-86]
-	_ = x[actPrevSelected-87]
-	_ = x[actPut-88]
-	_ = x[actNextHistory-89]
-	_ = x[actNextSelected-90]
-	_ = x[actExecute-91]
-	_ = x[actExecuteSilent-92]
-	_ = x[actExecuteMulti-93]
-	_ = x[actSigStop-94]
-	_ = x[actFirst-95]
-	_ = x[actLast-96]
-	_ = x[actReload-97]
-	_ = x[actReloadSync-98]
-	_ = x[actDisableSearch-99]
-	_ = x[actEnableSearch-100]
-	_ = x[actSelect-101]
-	_ = x[actDeselect-102]
-	_ = x[actUnbind-103]
-	_ = x[actRebind-104]
-	_ = x[actBecome-105]
-	_ = x[actResponse-106]
-	_ = x[actShowHeader-107]
-	_ = x[actHideHeader-108]
+	_ = x[actChangeMulti-18]
+	_ = x[actChangePreviewLabel-19]
+	_ = x[actChangePrompt-20]
+	_ = x[actChangeQuery-21]
+	_ = x[actClearScreen-22]
+	_ = x[actClearQuery-23]
+	_ = x[actClearSelection-24]
+	_ = x[actClose-25]
+	_ = x[actDeleteChar-26]
+	_ = x[actDeleteCharEof-27]
+	_ = x[actEndOfLine-28]
+	_ = x[actForwardChar-29]
+	_ = x[actForwardWord-30]
+	_ = x[actKillLine-31]
+	_ = x[actKillWord-32]
+	_ = x[actUnixLineDiscard-33]
+	_ = x[actUnixWordRubout-34]
+	_ = x[actYank-35]
+	_ = x[actBackwardKillWord-36]
+	_ = x[actSelectAll-37]
+	_ = x[actDeselectAll-38]
+	_ = x[actToggle-39]
+	_ = x[actToggleSearch-40]
+	_ = x[actToggleAll-41]
+	_ = x[actToggleDown-42]
+	_ = x[actToggleUp-43]
+	_ = x[actToggleIn-44]
+	_ = x[actToggleOut-45]
+	_ = x[actToggleTrack-46]
+	_ = x[actToggleTrackCurrent-47]
+	_ = x[actToggleHeader-48]
+	_ = x[actTrackCurrent-49]
+	_ = x[actUntrackCurrent-50]
+	_ = x[actDown-51]
+	_ = x[actUp-52]
+	_ = x[actPageUp-53]
+	_ = x[actPageDown-54]
+	_ = x[actPosition-55]
+	_ = x[actHalfPageUp-56]
+	_ = x[actHalfPageDown-57]
+	_ = x[actOffsetUp-58]
+	_ = x[actOffsetDown-59]
+	_ = x[actJump-60]
+	_ = x[actJumpAccept-61]
+	_ = x[actPrintQuery-62]
+	_ = x[actRefreshPreview-63]
+	_ = x[actReplaceQuery-64]
+	_ = x[actToggleSort-65]
+	_ = x[actShowPreview-66]
+	_ = x[actHidePreview-67]
+	_ = x[actTogglePreview-68]
+	_ = x[actTogglePreviewWrap-69]
+	_ = x[actTransform-70]
+	_ = x[actTransformBorderLabel-71]
+	_ = x[actTransformHeader-72]
+	_ = x[actTransformPreviewLabel-73]
+	_ = x[actTransformPrompt-74]
+	_ = x[actTransformQuery-75]
+	_ = x[actPreview-76]
+	_ = x[actChangePreview-77]
+	_ = x[actChangePreviewWindow-78]
+	_ = x[actPreviewTop-79]
+	_ = x[actPreviewBottom-80]
+	_ = x[actPreviewUp-81]
+	_ = x[actPreviewDown-82]
+	_ = x[actPreviewPageUp-83]
+	_ = x[actPreviewPageDown-84]
+	_ = x[actPreviewHalfPageUp-85]
+	_ = x[actPreviewHalfPageDown-86]
+	_ = x[actPrevHistory-87]
+	_ = x[actPrevSelected-88]
+	_ = x[actPut-89]
+	_ = x[actNextHistory-90]
+	_ = x[actNextSelected-91]
+	_ = x[actExecute-92]
+	_ = x[actExecuteSilent-93]
+	_ = x[actExecuteMulti-94]
+	_ = x[actSigStop-95]
+	_ = x[actFirst-96]
+	_ = x[actLast-97]
+	_ = x[actReload-98]
+	_ = x[actReloadSync-99]
+	_ = x[actDisableSearch-100]
+	_ = x[actEnableSearch-101]
+	_ = x[actSelect-102]
+	_ = x[actDeselect-103]
+	_ = x[actUnbind-104]
+	_ = x[actRebind-105]
+	_ = x[actBecome-106]
+	_ = x[actResponse-107]
+	_ = x[actShowHeader-108]
+	_ = x[actHideHeader-109]
 }
 
-const _actionType_name = "actIgnoreactStartactClickactInvalidactCharactMouseactBeginningOfLineactAbortactAcceptactAcceptNonEmptyactAcceptOrPrintQueryactBackwardCharactBackwardDeleteCharactBackwardDeleteCharEofactBackwardWordactCancelactChangeBorderLabelactChangeHeaderactChangePreviewLabelactChangePromptactChangeQueryactClearScreenactClearQueryactClearSelectionactCloseactDeleteCharactDeleteCharEofactEndOfLineactForwardCharactForwardWordactKillLineactKillWordactUnixLineDiscardactUnixWordRuboutactYankactBackwardKillWordactSelectAllactDeselectAllactToggleactToggleSearchactToggleAllactToggleDownactToggleUpactToggleInactToggleOutactToggleTrackactToggleTrackCurrentactToggleHeaderactTrackCurrentactUntrackCurrentactDownactUpactPageUpactPageDownactPositionactHalfPageUpactHalfPageDownactOffsetUpactOffsetDownactJumpactJumpAcceptactPrintQueryactRefreshPreviewactReplaceQueryactToggleSortactShowPreviewactHidePreviewactTogglePreviewactTogglePreviewWrapactTransformactTransformBorderLabelactTransformHeaderactTransformPreviewLabelactTransformPromptactTransformQueryactPreviewactChangePreviewactChangePreviewWindowactPreviewTopactPreviewBottomactPreviewUpactPreviewDownactPreviewPageUpactPreviewPageDownactPreviewHalfPageUpactPreviewHalfPageDownactPrevHistoryactPrevSelectedactPutactNextHistoryactNextSelectedactExecuteactExecuteSilentactExecuteMultiactSigStopactFirstactLastactReloadactReloadSyncactDisableSearchactEnableSearchactSelectactDeselectactUnbindactRebindactBecomeactResponseactShowHeaderactHideHeader"
+const _actionType_name = "actIgnoreactStartactClickactInvalidactCharactMouseactBeginningOfLineactAbortactAcceptactAcceptNonEmptyactAcceptOrPrintQueryactBackwardCharactBackwardDeleteCharactBackwardDeleteCharEofactBackwardWordactCancelactChangeBorderLabelactChangeHeaderactChangeMultiactChangePreviewLabelactChangePromptactChangeQueryactClearScreenactClearQueryactClearSelectionactCloseactDeleteCharactDeleteCharEofactEndOfLineactForwardCharactForwardWordactKillLineactKillWordactUnixLineDiscardactUnixWordRuboutactYankactBackwardKillWordactSelectAllactDeselectAllactToggleactToggleSearchactToggleAllactToggleDownactToggleUpactToggleInactToggleOutactToggleTrackactToggleTrackCurrentactToggleHeaderactTrackCurrentactUntrackCurrentactDownactUpactPageUpactPageDownactPositionactHalfPageUpactHalfPageDownactOffsetUpactOffsetDownactJumpactJumpAcceptactPrintQueryactRefreshPreviewactReplaceQueryactToggleSortactShowPreviewactHidePreviewactTogglePreviewactTogglePreviewWrapactTransformactTransformBorderLabelactTransformHeaderactTransformPreviewLabelactTransformPromptactTransformQueryactPreviewactChangePreviewactChangePreviewWindowactPreviewTopactPreviewBottomactPreviewUpactPreviewDownactPreviewPageUpactPreviewPageDownactPreviewHalfPageUpactPreviewHalfPageDownactPrevHistoryactPrevSelectedactPutactNextHistoryactNextSelectedactExecuteactExecuteSilentactExecuteMultiactSigStopactFirstactLastactReloadactReloadSyncactDisableSearchactEnableSearchactSelectactDeselectactUnbindactRebindactBecomeactResponseactShowHeaderactHideHeader"
 
-var _actionType_index = [...]uint16{0, 9, 17, 25, 35, 42, 50, 68, 76, 85, 102, 123, 138, 159, 183, 198, 207, 227, 242, 263, 278, 292, 306, 319, 336, 344, 357, 373, 385, 399, 413, 424, 435, 453, 470, 477, 496, 508, 522, 531, 546, 558, 571, 582, 593, 605, 619, 640, 655, 670, 687, 694, 699, 708, 719, 730, 743, 758, 769, 782, 789, 802, 815, 832, 847, 860, 874, 888, 904, 924, 936, 959, 977, 1001, 1019, 1036, 1046, 1062, 1084, 1097, 1113, 1125, 1139, 1155, 1173, 1193, 1215, 1229, 1244, 1250, 1264, 1279, 1289, 1305, 1320, 1330, 1338, 1345, 1354, 1367, 1383, 1398, 1407, 1418, 1427, 1436, 1445, 1456, 1469, 1482}
+var _actionType_index = [...]uint16{0, 9, 17, 25, 35, 42, 50, 68, 76, 85, 102, 123, 138, 159, 183, 198, 207, 227, 242, 256, 277, 292, 306, 320, 333, 350, 358, 371, 387, 399, 413, 427, 438, 449, 467, 484, 491, 510, 522, 536, 545, 560, 572, 585, 596, 607, 619, 633, 654, 669, 684, 701, 708, 713, 722, 733, 744, 757, 772, 783, 796, 803, 816, 829, 846, 861, 874, 888, 902, 918, 938, 950, 973, 991, 1015, 1033, 1050, 1060, 1076, 1098, 1111, 1127, 1139, 1153, 1169, 1187, 1207, 1229, 1243, 1258, 1264, 1278, 1293, 1303, 1319, 1334, 1344, 1352, 1359, 1368, 1381, 1397, 1412, 1421, 1432, 1441, 1450, 1459, 1470, 1483, 1496}
 
 func (i actionType) String() string {
 	if i < 0 || i >= actionType(len(_actionType_index)-1) {
 		return "actionType(" + strconv.FormatInt(int64(i), 10) + ")"
 	}
 	return _actionType_name[_actionType_index[i]:_actionType_index[i+1]]
 }
```

### Comparing `fzf_bin-0.50.0/fzf/src/algo/algo.go` & `fzf_bin-0.51.0/fzf/src/algo/algo.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/algo/algo_test.go` & `fzf_bin-0.51.0/fzf/src/algo/algo_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/algo/normalize.go` & `fzf_bin-0.51.0/fzf/src/algo/normalize.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/ansi.go` & `fzf_bin-0.51.0/fzf/src/ansi.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/ansi_test.go` & `fzf_bin-0.51.0/fzf/src/ansi_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/cache.go` & `fzf_bin-0.51.0/fzf/src/cache.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/cache_test.go` & `fzf_bin-0.51.0/fzf/src/cache_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/chunklist.go` & `fzf_bin-0.51.0/fzf/src/chunklist.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/chunklist_test.go` & `fzf_bin-0.51.0/fzf/src/chunklist_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/constants.go` & `fzf_bin-0.51.0/fzf/src/constants.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/core.go` & `fzf_bin-0.51.0/fzf/src/core.go`

 * *Files 5% similar despite different names*

```diff
@@ -117,21 +117,24 @@
 			item.text.Index = itemIndex
 			item.origText = &data
 			itemIndex++
 			return true
 		})
 	}
 
+	// Process executor
+	executor := util.NewExecutor(opts.WithShell)
+
 	// Reader
 	streamingFilter := opts.Filter != nil && !sort && !opts.Tac && !opts.Sync
 	var reader *Reader
 	if !streamingFilter {
 		reader = NewReader(func(data []byte) bool {
 			return chunkList.Push(data)
-		}, eventBox, opts.ReadZero, opts.Filter == nil)
+		}, eventBox, executor, opts.ReadZero, opts.Filter == nil)
 		go reader.ReadSource(opts.WalkerRoot, opts.WalkerOpts, opts.WalkerSkip)
 	}
 
 	// Matcher
 	forward := true
 	withPos := false
 	for idx := len(opts.Criteria) - 1; idx > 0; idx-- {
@@ -174,15 +177,15 @@
 						if result, _, _ := pattern.MatchItem(&item, false, slab); result != nil {
 							opts.Printer(item.text.ToString())
 							found = true
 						}
 						mutex.Unlock()
 					}
 					return false
-				}, eventBox, opts.ReadZero, false)
+				}, eventBox, executor, opts.ReadZero, false)
 			reader.ReadSource(opts.WalkerRoot, opts.WalkerOpts, opts.WalkerSkip)
 		} else {
 			eventBox.Unwatch(EvtReadNew)
 			eventBox.WaitFor(EvtReadFin)
 
 			snapshot, _ := chunkList.Snapshot()
 			merger, _ := matcher.scan(MatchRequest{
@@ -205,15 +208,15 @@
 		eventBox.WaitFor(EvtReadFin)
 	}
 
 	// Go interactive
 	go matcher.Loop()
 
 	// Terminal I/O
-	terminal := NewTerminal(opts, eventBox)
+	terminal := NewTerminal(opts, eventBox, executor)
 	maxFit := 0 // Maximum number of items that can fit on screen
 	padHeight := 0
 	heightUnknown := opts.Height.auto
 	if heightUnknown {
 		maxFit, padHeight = terminal.MaxFitAndPad()
 	}
 	deferred := opts.Select1 || opts.Exit0
@@ -294,16 +297,15 @@
 						}
 						snapshot, count = chunkList.Snapshot()
 						snapshotRevision = inputRevision
 					}
 					total = count
 					terminal.UpdateCount(total, !reading, value.(*string))
 					if opts.Sync {
-						opts.Sync = false
-						terminal.UpdateList(PassMerger(&snapshot, opts.Tac, snapshotRevision))
+						terminal.UpdateList(PassMerger(&snapshot, opts.Tac, snapshotRevision), false)
 					}
 					if heightUnknown && !deferred {
 						determine(!reading)
 					}
 					matcher.Reset(snapshot, input(), false, !reading, sort, snapshotRevision)
 
 				case EvtSearchNew:
@@ -380,15 +382,15 @@
 										util.Exit(exitOk)
 									}
 									util.Exit(exitNoMatch)
 								}
 								determine(val.final)
 							}
 						}
-						terminal.UpdateList(val)
+						terminal.UpdateList(val, true)
 					}
 				}
 			}
 			events.Clear()
 		})
 		if delay && reading {
 			dur := util.DurWithin(
```

### Comparing `fzf_bin-0.50.0/fzf/src/history.go` & `fzf_bin-0.51.0/fzf/src/history.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/history_test.go` & `fzf_bin-0.51.0/fzf/src/history_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/item.go` & `fzf_bin-0.51.0/fzf/src/item.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/matcher.go` & `fzf_bin-0.51.0/fzf/src/matcher.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/merger.go` & `fzf_bin-0.51.0/fzf/src/merger.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/merger_test.go` & `fzf_bin-0.51.0/fzf/src/merger_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/options.go` & `fzf_bin-0.51.0/fzf/src/options.go`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
                            highlighted substring (default: 10)
     --filepath-word        Make word-wise movements respect path separators
     --jump-labels=CHARS    Label characters for jump mode
 
   Layout
     --height=[~]HEIGHT[%]  Display fzf window below the cursor with the given
                            height instead of using fullscreen.
-                           A negative value is calcalated as the terminal height
+                           A negative value is calculated as the terminal height
                            minus the given value.
                            If prefixed with '~', fzf will determine the height
                            according to the input size.
     --min-height=HEIGHT    Minimum height when --height is given in percent
                            (default: 10)
     --layout=LAYOUT        Choose layout: [default|reverse|reverse-list]
     --border[=STYLE]       Draw border around the finder
@@ -116,14 +116,15 @@
     -0, --exit-0           Exit immediately when there's no match
     -f, --filter=STR       Filter mode. Do not start interactive finder.
     --print-query          Print query as the first line
     --expect=KEYS          Comma-separated list of keys to complete fzf
     --read0                Read input delimited by ASCII NUL characters
     --print0               Print output delimited by ASCII NUL characters
     --sync                 Synchronous search for multi-staged filtering
+    --with-shell=STR       Shell command and flags to start child processes with
     --listen[=[ADDR:]PORT] Start HTTP server to receive actions (POST /)
                            (To allow remote process execution, use --listen-unsafe)
     --version              Display version information and exit
 
   Directory traversal      (Only used when $FZF_DEFAULT_COMMAND is not set)
     --walker=OPTS          [file][,dir][,follow][,hidden] (default: file,follow,hidden)
     --walker-root=DIR      Root directory from which to start walker (default: .)
@@ -352,14 +353,15 @@
 	Padding      [4]sizeSpec
 	BorderShape  tui.BorderShape
 	BorderLabel  labelOpts
 	PreviewLabel labelOpts
 	Unicode      bool
 	Ambidouble   bool
 	Tabstop      int
+	WithShell    string
 	ListenAddr   *listenAddress
 	Unsafe       bool
 	ClearOnExit  bool
 	WalkerOpts   walkerOpts
 	WalkerRoot   string
 	WalkerSkip   []string
 	Version      bool
@@ -1051,15 +1053,15 @@
 	escapedColon = 0
 	escapedComma = 1
 	escapedPlus  = 2
 )
 
 func init() {
 	executeRegexp = regexp.MustCompile(
-		`(?si)[:+](become|execute(?:-multi|-silent)?|reload(?:-sync)?|preview|(?:change|transform)-(?:header|query|prompt|border-label|preview-label)|transform|change-preview-window|change-preview|(?:re|un)bind|pos|put)`)
+		`(?si)[:+](become|execute(?:-multi|-silent)?|reload(?:-sync)?|preview|(?:change|transform)-(?:header|query|prompt|border-label|preview-label)|transform|change-(?:preview-window|preview|multi)|(?:re|un)bind|pos|put)`)
 	splitRegexp = regexp.MustCompile("[,:]+")
 	actionNameRegexp = regexp.MustCompile("(?i)^[a-z-]+")
 }
 
 func maskActionContents(action string) string {
 	masked := ""
 Loop:
@@ -1302,14 +1304,16 @@
 				exit("unable to put non-printable character")
 			}
 		default:
 			t := isExecuteAction(specLower)
 			if t == actIgnore {
 				if specIndex == 0 && specLower == "" {
 					actions = append(prevActions, actions...)
+				} else if specLower == "change-multi" {
+					appendAction(actChangeMulti)
 				} else {
 					exit("unknown action: " + spec)
 				}
 			} else {
 				offset := len(actionNameRegexp.FindString(spec))
 				var actionArg string
 				if spec[offset] == ':' {
@@ -1321,18 +1325,14 @@
 						continue
 					}
 				} else {
 					actionArg = spec[offset+1 : len(spec)-1]
 					actions = append(actions, &action{t: t, a: actionArg})
 				}
 				switch t {
-				case actBecome:
-					if util.IsWindows() {
-						exit("become action is not supported on Windows")
-					}
 				case actUnbind, actRebind:
 					parseKeyChordsImpl(actionArg, spec[0:offset]+" target required", exit)
 				case actChangePreviewWindow:
 					opts := previewOpts{}
 					for _, arg := range strings.Split(actionArg, "|") {
 						// Make sure that each expression is valid
 						parsePreviewWindowImpl(&opts, arg, exit)
@@ -1403,14 +1403,16 @@
 		return actChangePreviewWindow
 	case "change-preview":
 		return actChangePreview
 	case "change-prompt":
 		return actChangePrompt
 	case "change-query":
 		return actChangeQuery
+	case "change-multi":
+		return actChangeMulti
 	case "pos":
 		return actPosition
 	case "execute":
 		return actExecute
 	case "execute-silent":
 		return actExecuteSilent
 	case "execute-multi":
@@ -1872,17 +1874,15 @@
 			opts.Prompt = nextString(allArgs, &i, "prompt string required")
 		case "--pointer":
 			opts.Pointer = firstLine(nextString(allArgs, &i, "pointer sign string required"))
 		case "--marker":
 			opts.Marker = firstLine(nextString(allArgs, &i, "selected sign string required"))
 		case "--sync":
 			opts.Sync = true
-		case "--no-sync":
-			opts.Sync = false
-		case "--async":
+		case "--no-sync", "--async":
 			opts.Sync = false
 		case "--no-history":
 			opts.History = nil
 		case "--history":
 			setHistory(nextString(allArgs, &i, "history file path required"))
 		case "--history-size":
 			setHistoryMax(nextInt(allArgs, &i, "history max size required"))
@@ -1951,14 +1951,16 @@
 				nextString(allArgs, &i, "margin required (TRBL / TB,RL / T,RL,B / T,R,B,L)"))
 		case "--padding":
 			opts.Padding = parseMargin(
 				"padding",
 				nextString(allArgs, &i, "padding required (TRBL / TB,RL / T,RL,B / T,R,B,L)"))
 		case "--tabstop":
 			opts.Tabstop = nextInt(allArgs, &i, "tab stop required")
+		case "--with-shell":
+			opts.WithShell = nextString(allArgs, &i, "shell command and flags required")
 		case "--listen", "--listen-unsafe":
 			given, str := optionalNextString(allArgs, &i)
 			addr := defaultListenAddr
 			if given {
 				var err error
 				addr, err = parseListenAddress(str)
 				if err != nil {
@@ -2067,14 +2069,16 @@
 				parsePreviewWindow(&opts.Preview, value)
 			} else if match, value := optString(arg, "--margin="); match {
 				opts.Margin = parseMargin("margin", value)
 			} else if match, value := optString(arg, "--padding="); match {
 				opts.Padding = parseMargin("padding", value)
 			} else if match, value := optString(arg, "--tabstop="); match {
 				opts.Tabstop = atoi(value)
+			} else if match, value := optString(arg, "--with-shell="); match {
+				opts.WithShell = value
 			} else if match, value := optString(arg, "--listen="); match {
 				addr, err := parseListenAddress(value)
 				if err != nil {
 					errorExit(err.Error())
 				}
 				opts.ListenAddr = &addr
 				opts.Unsafe = false
```

### Comparing `fzf_bin-0.50.0/fzf/src/options_pprof.go` & `fzf_bin-0.51.0/fzf/src/options_pprof.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/options_pprof_test.go` & `fzf_bin-0.51.0/fzf/src/options_pprof_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/options_test.go` & `fzf_bin-0.51.0/fzf/src/options_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/pattern.go` & `fzf_bin-0.51.0/fzf/src/pattern.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/pattern_test.go` & `fzf_bin-0.51.0/fzf/src/pattern_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/reader.go` & `fzf_bin-0.51.0/fzf/src/reader.go`

 * *Files 4% similar despite different names*

```diff
@@ -14,28 +14,29 @@
 	"github.com/charlievieth/fastwalk"
 	"github.com/junegunn/fzf/src/util"
 )
 
 // Reader reads from command or standard input
 type Reader struct {
 	pusher   func([]byte) bool
+	executor *util.Executor
 	eventBox *util.EventBox
 	delimNil bool
 	event    int32
 	finChan  chan bool
 	mutex    sync.Mutex
 	exec     *exec.Cmd
 	command  *string
 	killed   bool
 	wait     bool
 }
 
 // NewReader returns new Reader object
-func NewReader(pusher func([]byte) bool, eventBox *util.EventBox, delimNil bool, wait bool) *Reader {
-	return &Reader{pusher, eventBox, delimNil, int32(EvtReady), make(chan bool, 1), sync.Mutex{}, nil, nil, false, wait}
+func NewReader(pusher func([]byte) bool, eventBox *util.EventBox, executor *util.Executor, delimNil bool, wait bool) *Reader {
+	return &Reader{pusher, executor, eventBox, delimNil, int32(EvtReady), make(chan bool, 1), sync.Mutex{}, nil, nil, false, wait}
 }
 
 func (r *Reader) startEventPoller() {
 	go func() {
 		ptr := &r.event
 		pollInterval := readerPollIntervalMin
 		for {
@@ -143,15 +144,15 @@
 			n, err = src.Read(scope)
 			if n > 0 || err != nil {
 				break
 			}
 		}
 
 		// We're not making any progress after 100 tries. Stop.
-		if n == 0 && err == nil {
+		if n == 0 {
 			break
 		}
 
 		buf := slab[:n]
 		slab = slab[n:]
 
 		for len(buf) > 0 {
@@ -238,15 +239,15 @@
 	return fastwalk.Walk(&conf, root, fn) == nil
 }
 
 func (r *Reader) readFromCommand(command string, environ []string) bool {
 	r.mutex.Lock()
 	r.killed = false
 	r.command = &command
-	r.exec = util.ExecCommand(command, true)
+	r.exec = r.executor.ExecCommand(command, true)
 	if environ != nil {
 		r.exec.Env = environ
 	}
 	out, err := r.exec.StdoutPipe()
 	if err != nil {
 		r.mutex.Unlock()
 		return false
```

### Comparing `fzf_bin-0.50.0/fzf/src/reader_test.go` & `fzf_bin-0.51.0/fzf/src/reader_test.go`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 
 	"github.com/junegunn/fzf/src/util"
 )
 
 func TestReadFromCommand(t *testing.T) {
 	strs := []string{}
 	eb := util.NewEventBox()
+	exec := util.NewExecutor("")
 	reader := NewReader(
 		func(s []byte) bool { strs = append(strs, string(s)); return true },
-		eb, false, true)
+		eb, exec, false, true)
 
 	reader.startEventPoller()
 
 	// Check EventBox
 	if eb.Peek(EvtReadNew) {
 		t.Error("EvtReadNew should not be set yet")
 	}
```

### Comparing `fzf_bin-0.50.0/fzf/src/result.go` & `fzf_bin-0.51.0/fzf/src/result.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/result_test.go` & `fzf_bin-0.51.0/fzf/src/result_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/server.go` & `fzf_bin-0.51.0/fzf/src/server.go`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 }
 
 func startHttpServer(address listenAddress, actionChannel chan []*action, responseChannel chan string) (int, error) {
 	host := address.host
 	port := address.port
 	apiKey := os.Getenv("FZF_API_KEY")
 	if !address.IsLocal() && len(apiKey) == 0 {
-		return port, fmt.Errorf("FZF_API_KEY is required to allow remote access")
+		return port, errors.New("FZF_API_KEY is required to allow remote access")
 	}
 	addrStr := fmt.Sprintf("%s:%d", host, port)
 	listener, err := net.Listen("tcp", addrStr)
 	if err != nil {
 		return port, fmt.Errorf("failed to listen on %s", addrStr)
 	}
 	if port == 0 {
```

### Comparing `fzf_bin-0.50.0/fzf/src/terminal.go` & `fzf_bin-0.51.0/fzf/src/terminal.go`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import (
 	"bufio"
 	"encoding/json"
 	"fmt"
 	"io"
 	"math"
 	"os"
-	"os/exec"
 	"os/signal"
 	"regexp"
 	"sort"
 	"strconv"
 	"strings"
 	"sync"
 	"syscall"
@@ -241,14 +240,15 @@
 	padding            [4]sizeSpec
 	unicode            bool
 	listenAddr         *listenAddress
 	listenPort         *int
 	listenUnsafe       bool
 	borderShape        tui.BorderShape
 	cleanExit          bool
+	executor           *util.Executor
 	paused             bool
 	border             tui.Window
 	window             tui.Window
 	pborder            tui.Window
 	pwindow            tui.Window
 	borderWidth        int
 	count              int
@@ -363,14 +363,15 @@
 	actBackwardChar
 	actBackwardDeleteChar
 	actBackwardDeleteCharEof
 	actBackwardWord
 	actCancel
 	actChangeBorderLabel
 	actChangeHeader
+	actChangeMulti
 	actChangePreviewLabel
 	actChangePrompt
 	actChangeQuery
 	actClearScreen
 	actClearQuery
 	actClearSelection
 	actClose
@@ -635,15 +636,15 @@
 	if opts.Height.inverse {
 		size = float64(termHeight) - size
 	}
 	return int(size)
 }
 
 // NewTerminal returns new Terminal object
-func NewTerminal(opts *Options, eventBox *util.EventBox) *Terminal {
+func NewTerminal(opts *Options, eventBox *util.EventBox, executor *util.Executor) *Terminal {
 	input := trimQuery(opts.Query)
 	var delay time.Duration
 	if opts.Tac {
 		delay = initialDelayTac
 	} else {
 		delay = initialDelay
 	}
@@ -731,14 +732,15 @@
 		borderShape:        opts.BorderShape,
 		borderWidth:        1,
 		borderLabel:        nil,
 		borderLabelOpts:    opts.BorderLabel,
 		previewLabel:       nil,
 		previewLabelOpts:   opts.PreviewLabel,
 		cleanExit:          opts.ClearOnExit,
+		executor:           executor,
 		paused:             opts.Phony,
 		cycle:              opts.Cycle,
 		headerVisible:      true,
 		headerFirst:        opts.HeaderFirst,
 		headerLines:        opts.HeaderLines,
 		header:             []string{},
 		header0:            opts.Header,
@@ -850,14 +852,15 @@
 	env = append(env, "FZF_PREVIEW_LABEL="+t.previewLabelOpts.label)
 	env = append(env, "FZF_BORDER_LABEL="+t.borderLabelOpts.label)
 	env = append(env, fmt.Sprintf("FZF_TOTAL_COUNT=%d", t.count))
 	env = append(env, fmt.Sprintf("FZF_MATCH_COUNT=%d", t.merger.Length()))
 	env = append(env, fmt.Sprintf("FZF_SELECT_COUNT=%d", len(t.selected)))
 	env = append(env, fmt.Sprintf("FZF_LINES=%d", t.areaLines))
 	env = append(env, fmt.Sprintf("FZF_COLUMNS=%d", t.areaColumns))
+	env = append(env, fmt.Sprintf("FZF_POS=%d", util.Min(t.merger.Length(), t.cy+1)))
 	return env
 }
 
 func borderLines(shape tui.BorderShape) int {
 	switch shape {
 	case tui.BorderHorizontal, tui.BorderRounded, tui.BorderSharp, tui.BorderBold, tui.BorderBlock, tui.BorderThinBlock, tui.BorderDouble:
 		return 2
@@ -1063,15 +1066,15 @@
 
 	if changed {
 		t.reqBox.Set(reqInfo, nil)
 	}
 }
 
 // UpdateList updates Merger to display the list
-func (t *Terminal) UpdateList(merger *Merger) {
+func (t *Terminal) UpdateList(merger *Merger, triggerResultEvent bool) {
 	t.mutex.Lock()
 	prevIndex := minItem.Index()
 	reset := t.revision != merger.Revision()
 	if !reset && t.track != trackDisabled {
 		if t.merger.Length() > 0 {
 			prevIndex = t.currentIndex()
 		} else if merger.Length() > 0 {
@@ -1114,15 +1117,15 @@
 			}
 		case 1:
 			one := tui.One.AsEvent()
 			if _, prs := t.keymap[one]; prs {
 				t.eventChan <- one
 			}
 		}
-		if t.hasResultActions {
+		if triggerResultEvent && t.hasResultActions {
 			t.eventChan <- tui.Result.AsEvent()
 		}
 	}
 	t.mutex.Unlock()
 	t.reqBox.Set(reqInfo, nil)
 	t.reqBox.Set(reqList, nil)
 }
@@ -2517,27 +2520,29 @@
 	delimiter  Delimiter
 	printsep   string
 	forcePlus  bool
 	query      string
 	allItems   []*Item
 	lastAction actionType
 	prompt     string
+	executor   *util.Executor
 }
 
 func (t *Terminal) replacePlaceholder(template string, forcePlus bool, input string, list []*Item) string {
 	return replacePlaceholder(replacePlaceholderParams{
 		template:   template,
 		stripAnsi:  t.ansi,
 		delimiter:  t.delimiter,
 		printsep:   t.printsep,
 		forcePlus:  forcePlus,
 		query:      input,
 		allItems:   list,
 		lastAction: t.lastAction,
 		prompt:     t.promptString,
+		executor:   t.executor,
 	})
 }
 
 func (t *Terminal) evaluateScrollOffset() int {
 	if t.pwindow == nil {
 		return 0
 	}
@@ -2590,34 +2595,34 @@
 		var replace func(*Item) string
 
 		// placeholder types (escaped, query type, item type, token type)
 		switch {
 		case escaped:
 			return match
 		case match == "{q}" || match == "{fzf:query}":
-			return quoteEntry(params.query)
+			return params.executor.QuoteEntry(params.query)
 		case match == "{}":
 			replace = func(item *Item) string {
 				switch {
 				case flags.number:
 					n := int(item.text.Index)
 					if n < 0 {
 						return ""
 					}
 					return strconv.Itoa(n)
 				case flags.file:
 					return item.AsString(params.stripAnsi)
 				default:
-					return quoteEntry(item.AsString(params.stripAnsi))
+					return params.executor.QuoteEntry(item.AsString(params.stripAnsi))
 				}
 			}
 		case match == "{fzf:action}":
 			return params.lastAction.Name()
 		case match == "{fzf:prompt}":
-			return quoteEntry(params.prompt)
+			return params.executor.QuoteEntry(params.prompt)
 		default:
 			// token type and also failover (below)
 			rangeExpressions := strings.Split(match[1:len(match)-1], ",")
 			ranges := make([]Range, len(rangeExpressions))
 			for idx, s := range rangeExpressions {
 				r, ok := ParseRange(&s) // ellipsis (x..y) and shorthand (x..x) range syntax
 				if !ok {
@@ -2643,15 +2648,15 @@
 					}
 				}
 
 				if !flags.preserveSpace {
 					str = strings.TrimSpace(str)
 				}
 				if !flags.file {
-					str = quoteEntry(str)
+					str = params.executor.QuoteEntry(str)
 				}
 				return str
 			}
 		}
 
 		// apply 'replace' function over proper set of items and return result
 
@@ -2683,15 +2688,15 @@
 	valid, list := t.buildPlusList(template, forcePlus)
 	// 'capture' is used for transform-* and we don't want to
 	// return an empty string in those cases
 	if !valid && !capture {
 		return line
 	}
 	command := t.replacePlaceholder(template, forcePlus, string(t.input), list)
-	cmd := util.ExecCommand(command, false)
+	cmd := t.executor.ExecCommand(command, false)
 	cmd.Env = t.environ()
 	t.executing.Set(true)
 	if !background {
 		cmd.Stdin = tui.TtyIn()
 		cmd.Stdout = os.Stdout
 		cmd.Stderr = os.Stderr
 		t.tui.Pause(true)
@@ -2960,15 +2965,15 @@
 					events.Clear()
 				})
 				version++
 				// We don't display preview window if no match
 				if items[0] != nil {
 					_, query := t.Input()
 					command := t.replacePlaceholder(commandTemplate, false, string(query), items)
-					cmd := util.ExecCommand(command, true)
+					cmd := t.executor.ExecCommand(command, true)
 					env := t.environ()
 					if pwindowSize.Lines > 0 {
 						lines := fmt.Sprintf("LINES=%d", pwindowSize.Lines)
 						columns := fmt.Sprintf("COLUMNS=%d", pwindowSize.Columns)
 						env = append(env, lines)
 						env = append(env, "FZF_PREVIEW_"+lines)
 						env = append(env, columns)
@@ -3367,35 +3372,29 @@
 			case actIgnore, actStart, actClick:
 			case actResponse:
 				t.serverOutputChan <- t.dumpStatus(parseGetParams(a.a))
 			case actBecome:
 				valid, list := t.buildPlusList(a.a, false)
 				if valid {
 					command := t.replacePlaceholder(a.a, false, string(t.input), list)
-					shell := os.Getenv("SHELL")
-					if len(shell) == 0 {
-						shell = "sh"
-					}
-					shellPath, err := exec.LookPath(shell)
-					if err == nil {
-						t.tui.Close()
-						if t.history != nil {
-							t.history.append(string(t.input))
-						}
-						/*
-							FIXME: It is not at all clear why this is required.
-							The following command will report 'not a tty', unless we open
-							/dev/tty *twice* after closing the standard input for 'reload'
-							in Reader.terminate().
-								: | fzf --bind 'start:reload:ls' --bind 'enter:become:tty'
-						*/
-						tui.TtyIn()
-						util.SetStdin(tui.TtyIn())
-						syscall.Exec(shellPath, []string{shell, "-c", command}, os.Environ())
+					t.tui.Close()
+					if t.history != nil {
+						t.history.append(string(t.input))
 					}
+
+					/*
+					 FIXME: It is not at all clear why this is required.
+					 The following command will report 'not a tty', unless we open
+					 /dev/tty *twice* after closing the standard input for 'reload'
+					 in Reader.terminate().
+
+					   while : | fzf --bind 'start:reload:ls' --bind 'load:become:tty'; do echo; done
+					*/
+					tui.TtyIn()
+					t.executor.Become(tui.TtyIn(), t.environ(), command)
 				}
 			case actExecute, actExecuteSilent:
 				t.executeCommand(a.a, false, a.t == actExecuteSilent, false, false)
 			case actExecuteMulti:
 				t.executeCommand(a.a, true, false, false, false)
 			case actInvalid:
 				t.mutex.Unlock()
@@ -3485,14 +3484,27 @@
 				t.xoffset = 0
 			case actBackwardChar:
 				if t.cx > 0 {
 					t.cx--
 				}
 			case actPrintQuery:
 				req(reqPrintQuery)
+			case actChangeMulti:
+				multi := t.multi
+				if a.a == "" {
+					multi = maxMulti
+				} else if n, e := strconv.Atoi(a.a); e == nil && n >= 0 {
+					multi = n
+				}
+				if t.multi > 0 && multi != t.multi {
+					t.selected = make(map[int32]selectedItem)
+					t.version++
+				}
+				t.multi = multi
+				req(reqList, reqInfo)
 			case actChangeQuery:
 				t.input = []rune(a.a)
 				t.cx = len(t.input)
 			case actTransformHeader:
 				header := t.executeCommand(a.a, false, true, true, false)
 				if t.changeHeader(header) {
 					req(reqFullRedraw)
```

### Comparing `fzf_bin-0.50.0/fzf/src/terminal_test.go` & `fzf_bin-0.51.0/fzf/src/terminal_test.go`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 		delimiter:  delimiter,
 		printsep:   printsep,
 		forcePlus:  forcePlus,
 		query:      query,
 		allItems:   allItems,
 		lastAction: actBackwardDeleteCharEof,
 		prompt:     "prompt",
+		executor:   util.NewExecutor(""),
 	})
 }
 
 func TestReplacePlaceholder(t *testing.T) {
 	item1 := newItem("  foo'bar \x1b[31mbaz\x1b[m")
 	items1 := []*Item{item1, item1}
 	items2 := []*Item{
@@ -240,14 +241,15 @@
 }
 
 func TestQuoteEntry(t *testing.T) {
 	type quotes struct{ E, O, SQ, DQ, BS string } // standalone escape, outer, single and double quotes, backslash
 	unixStyle := quotes{``, `'`, `'\''`, `"`, `\`}
 	windowsStyle := quotes{`^`, `^"`, `'`, `\^"`, `\\`}
 	var effectiveStyle quotes
+	exec := util.NewExecutor("")
 
 	if util.IsWindows() {
 		effectiveStyle = windowsStyle
 	} else {
 		effectiveStyle = unixStyle
 	}
 
@@ -274,15 +276,15 @@
 		`!`:                       `{{.O}}{{.E}}!{{.O}}`,
 		`%USERPROFILE%`:           `{{.O}}{{.E}}%USERPROFILE{{.E}}%{{.O}}`,
 		`C:\Program Files (x86)\`: `{{.O}}C:{{.BS}}Program Files {{.E}}(x86{{.E}}){{.BS}}{{.O}}`,
 		`"C:\Program Files"`:      `{{.O}}{{.DQ}}C:{{.BS}}Program Files{{.DQ}}{{.O}}`,
 	}
 
 	for input, expected := range tests {
-		escaped := quoteEntry(input)
+		escaped := exec.QuoteEntry(input)
 		expected = templateToString(expected, effectiveStyle)
 		if escaped != expected {
 			t.Errorf("Input: %s, expected: %s, actual %s", input, expected, escaped)
 		}
 	}
 }
 
@@ -313,17 +315,17 @@
 		{give{`cat {}`, ``, newItems(`$HOME/test`)}, want{output: `cat '$HOME/test'`}},
 	}
 	testCommands(t, tests)
 }
 
 // purpose of this test is to demonstrate some shortcomings of fzf's templating system on Windows
 func TestWindowsCommands(t *testing.T) {
-	if !util.IsWindows() {
-		t.SkipNow()
-	}
+	// XXX Deprecated
+	t.SkipNow()
+
 	tests := []testCase{
 		// reference: give{template, query, items}, want{output OR match}
 
 		// 1) working examples
 
 		// example of redundantly escaped backslash in the output, besides looking bit ugly, it won't cause any issue
 		{give{`type {}`, ``, newItems(`C:\test.txt`)}, want{output: `type ^"C:\\test.txt^"`}},
```

### Comparing `fzf_bin-0.50.0/fzf/src/tokenizer.go` & `fzf_bin-0.51.0/fzf/src/tokenizer.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/tokenizer_test.go` & `fzf_bin-0.51.0/fzf/src/tokenizer_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/tui/dummy.go` & `fzf_bin-0.51.0/fzf/src/tui/dummy.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/tui/eventtype_string.go` & `fzf_bin-0.51.0/fzf/src/tui/eventtype_string.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/tui/light.go` & `fzf_bin-0.51.0/fzf/src/tui/light.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/tui/light_unix.go` & `fzf_bin-0.51.0/fzf/src/tui/light_unix.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/tui/light_windows.go` & `fzf_bin-0.51.0/fzf/src/tui/light_windows.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/tui/tcell.go` & `fzf_bin-0.51.0/fzf/src/tui/tcell.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/tui/tcell_test.go` & `fzf_bin-0.51.0/fzf/src/tui/tcell_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/tui/ttyname_unix.go` & `fzf_bin-0.51.0/fzf/src/tui/ttyname_unix.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/tui/tui.go` & `fzf_bin-0.51.0/fzf/src/tui/tui.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/util/atexit.go` & `fzf_bin-0.51.0/fzf/src/util/atexit.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/util/atomicbool.go` & `fzf_bin-0.51.0/fzf/src/util/atomicbool.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/util/chars.go` & `fzf_bin-0.51.0/fzf/src/util/chars.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/util/chars_test.go` & `fzf_bin-0.51.0/fzf/src/util/chars_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/util/eventbox.go` & `fzf_bin-0.51.0/fzf/src/util/eventbox.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/util/eventbox_test.go` & `fzf_bin-0.51.0/fzf/src/util/eventbox_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/util/util.go` & `fzf_bin-0.51.0/fzf/src/util/util.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/src/util/util_test.go` & `fzf_bin-0.51.0/fzf/src/util/util_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/test/fzf.vader` & `fzf_bin-0.51.0/fzf/test/fzf.vader`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/fzf/test/test_go.rb` & `fzf_bin-0.51.0/fzf/test/test_go.rb`

 * *Files 0% similar despite different names*

```diff
@@ -421,14 +421,33 @@
     tmux.send_keys 'A'
     tmux.until do |lines|
       assert_includes lines[1], ' [5 6 1]/1 '
       assert lines[-2]&.start_with?('  10/10 (3/3)')
     end
   end
 
+  def test_multi_action
+    tmux.send_keys "seq 10 | #{FZF} --bind 'a:change-multi,b:change-multi(3),c:change-multi(xxx),d:change-multi(0)'", :Enter
+    tmux.until { |lines| assert_equal 10, lines.item_count }
+    tmux.until { |lines| assert lines[-2]&.start_with?('  10/10 ') }
+    tmux.send_keys 'a'
+    tmux.until { |lines| assert lines[-2]&.start_with?('  10/10 (0)') }
+    tmux.send_keys 'b'
+    tmux.until { |lines| assert lines[-2]&.start_with?('  10/10 (0/3)') }
+    tmux.send_keys :BTab
+    tmux.until { |lines| assert lines[-2]&.start_with?('  10/10 (1/3)') }
+    tmux.send_keys 'c'
+    tmux.send_keys :BTab
+    tmux.until { |lines| assert lines[-2]&.start_with?('  10/10 (2/3)') }
+    tmux.send_keys 'd'
+    tmux.until do |lines|
+      assert lines[-2]&.start_with?('  10/10 ') && !lines[-2]&.include?('(')
+    end
+  end
+
   def test_with_nth
     [true, false].each do |multi|
       tmux.send_keys "(echo '  1st 2nd 3rd/';
                        echo '  first second third/') |
                        #{fzf(multi && :multi, :x, :nth, 2, :with_nth, '2,-1,1')}",
                      :Enter
       tmux.until { |lines| assert_equal multi ? '  2/2 (0)' : '  2/2', lines[-2] }
@@ -1951,14 +1970,19 @@
   def test_reload_even_when_theres_no_match
     tmux.send_keys %(: | #{FZF} --bind 'space:reload(seq 10)'), :Enter
     tmux.until { |lines| assert_equal 0, lines.item_count }
     tmux.send_keys :Space
     tmux.until { |lines| assert_equal 10, lines.item_count }
   end
 
+  def test_reload_should_terminate_standard_input_stream
+    tmux.send_keys %(ruby -e "STDOUT.sync = true; loop { puts 1; sleep 0.1 }" | fzf --bind 'start:reload(seq 100)'), :Enter
+    tmux.until { |lines| assert_equal 100, lines.item_count }
+  end
+
   def test_clear_list_when_header_lines_changed_due_to_reload
     tmux.send_keys %(seq 10 | #{FZF} --header 0 --header-lines 3 --bind 'space:reload(seq 1)'), :Enter
     tmux.until { |lines| assert_includes lines, '  9' }
     tmux.send_keys :Space
     tmux.until { |lines| refute_includes lines, '  9' }
   end
 
@@ -3222,14 +3246,25 @@
 
   def test_preview_window_hidden_on_focus
     tmux.send_keys "seq 3 | #{FZF} --preview 'echo {}' --bind focus:hide-preview", :Enter
     tmux.until { |lines| assert_includes lines, '> 1' }
     tmux.send_keys :Up
     tmux.until { |lines| assert_includes lines, '> 2' }
   end
+
+  def test_fzf_pos
+    tmux.send_keys "seq 100 | #{FZF} --preview 'echo $FZF_POS / $FZF_MATCH_COUNT'", :Enter
+    tmux.until { |lines| assert(lines.any? { |line| line.include?('1 / 100') }) }
+    tmux.send_keys :Up
+    tmux.until { |lines| assert(lines.any? { |line| line.include?('2 / 100') }) }
+    tmux.send_keys '99'
+    tmux.until { |lines| assert(lines.any? { |line| line.include?('1 / 1') }) }
+    tmux.send_keys '99'
+    tmux.until { |lines| assert(lines.any? { |line| line.include?('0 / 0') }) }
+  end
 end
 
 module TestShell
   def setup
     @tmux = Tmux.new(shell)
     tmux.prepare
   end
@@ -3453,15 +3488,19 @@
     end
     FileUtils.touch('/tmp/fzf-test/d55/xxx')
     tmux.prepare
     tmux.send_keys 'cd /tmp/fzf-test/**', :Tab
     tmux.until { |lines| assert_operator lines.match_count, :>, 0 }
     tmux.send_keys :Tab, :Tab # Tab does not work here
     tmux.send_keys 55
-    tmux.until { |lines| assert_equal 1, lines.match_count }
+    tmux.until do |lines|
+      assert_equal 1, lines.match_count
+      assert_includes lines, '> 55'
+      assert_includes lines, '> /tmp/fzf-test/d55'
+    end
     tmux.send_keys :Enter
     tmux.until(true) { |lines| assert_equal 'cd /tmp/fzf-test/d55/', lines[-1] }
     tmux.send_keys :xx
     tmux.until { |lines| assert_equal 'cd /tmp/fzf-test/d55/xx', lines[-1] }
 
     # Should not match regular files (bash-only)
     if instance_of?(TestBash)
```

### Comparing `fzf_bin-0.50.0/fzf/uninstall` & `fzf_bin-0.51.0/fzf/uninstall`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.50.0/pdm_build.py` & `fzf_bin-0.51.0/pdm_build.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from wheel.cli.tags import tags
 
 if TYPE_CHECKING:
     from pdm.backend.hooks import Context
 
 NAME = "fzf"
-VERSION = "0.50.0"
+VERSION = "0.51.0"
 
 
 def is_windows():
     if "GOOS" in os.environ:
         return os.environ["GOOS"] == "windows"
     return sys.platform == "win32"
```

### Comparing `fzf_bin-0.50.0/pyproject.toml` & `fzf_bin-0.51.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "fzf-bin"
 description = "fzf - 🌸 A command-line fuzzy finder"
-version = "0.50.0"
+version = "0.51.0"
 authors = [
     { name = "dowon", email = "ks2515@naver.com" },
 ]
 dependencies = []
 requires-python = ">=3.8"
 readme = "README.md"
 keywords = [
```

### Comparing `fzf_bin-0.50.0/PKG-INFO` & `fzf_bin-0.51.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fzf-bin
-Version: 0.50.0
+Version: 0.51.0
 Summary: fzf - 🌸 A command-line fuzzy finder
 Keywords: fzf,tui,fuzzy finder
 Author-Email: dowon <ks2515@naver.com>
 License: MIT
 Classifier: Programming Language :: Other
 Classifier: Topic :: Software Development :: User Interfaces
 Project-URL: Repository, https://github.com/Bing-su/pip-binary-factory
```

