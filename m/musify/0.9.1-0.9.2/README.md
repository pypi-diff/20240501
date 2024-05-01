# Comparing `tmp/musify-0.9.1.tar.gz` & `tmp/musify-0.9.2.tar.gz`

## Comparing `musify-0.9.1.tar` & `musify-0.9.2.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 musify-0.9.1/musify/__init__.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 musify-0.9.1/musify/exception.py
--rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 musify-0.9.1/musify/field.py
--rw-r--r--   0        0        0     8071 2020-02-02 00:00:00.000000 musify-0.9.1/musify/report.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 musify-0.9.1/musify/types.py
--rw-r--r--   0        0        0    10127 2020-02-02 00:00:00.000000 musify-0.9.1/musify/utils.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 musify-0.9.1/musify/api/__init__.py
--rw-r--r--   0        0        0    16025 2020-02-02 00:00:00.000000 musify-0.9.1/musify/api/authorise.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 musify-0.9.1/musify/api/exception.py
--rw-r--r--   0        0        0    10229 2020-02-02 00:00:00.000000 musify-0.9.1/musify/api/request.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 musify-0.9.1/musify/core/__init__.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 musify-0.9.1/musify/core/base.py
--rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 musify-0.9.1/musify/core/enum.py
--rw-r--r--   0        0        0     9315 2020-02-02 00:00:00.000000 musify-0.9.1/musify/core/printer.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 musify-0.9.1/musify/core/result.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 musify-0.9.1/musify/file/__init__.py
--rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 musify-0.9.1/musify/file/base.py
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 musify-0.9.1/musify/file/exception.py
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 musify-0.9.1/musify/file/image.py
--rw-r--r--   0        0        0     8152 2020-02-02 00:00:00.000000 musify-0.9.1/musify/file/path_mapper.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/__init__.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/collection.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/core/__init__.py
--rw-r--r--   0        0        0    15068 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/core/collection.py
--rw-r--r--   0        0        0    23292 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/core/object.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/__init__.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/base.py
--rw-r--r--   0        0        0    19985 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/collection.py
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/exception.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/library/__init__.py
--rw-r--r--   0        0        0    20851 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/library/library.py
--rw-r--r--   0        0        0    24639 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/library/musicbee.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/playlist/__init__.py
--rw-r--r--   0        0        0     5752 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/playlist/base.py
--rw-r--r--   0        0        0     6391 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/playlist/m3u.py
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/playlist/utils.py
--rw-r--r--   0        0        0    28389 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/playlist/xautopf.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/track/__init__.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/track/field.py
--rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/track/flac.py
--rw-r--r--   0        0        0     6687 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/track/m4a.py
--rw-r--r--   0        0        0     7073 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/track/mp3.py
--rw-r--r--   0        0        0    17384 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/track/track.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/track/utils.py
--rw-r--r--   0        0        0     5161 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/track/wma.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/track/tags/__init__.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/track/tags/base.py
--rw-r--r--   0        0        0     7645 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/track/tags/reader.py
--rw-r--r--   0        0        0    32439 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/track/tags/writer.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/__init__.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/core/__init__.py
--rw-r--r--   0        0        0    21411 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/core/api.py
--rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/core/base.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/core/enum.py
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/core/exception.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/core/factory.py
--rw-r--r--   0        0        0    22023 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/core/library.py
--rw-r--r--   0        0        0    12680 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/core/object.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/core/response.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/core/types.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/core/processors/__init__.py
--rw-r--r--   0        0        0    23087 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/core/processors/check.py
--rw-r--r--   0        0        0    14891 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/core/processors/search.py
--rw-r--r--   0        0        0     9804 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/core/processors/wrangle.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/spotify/__init__.py
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/spotify/base.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/spotify/exception.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/spotify/factory.py
--rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/spotify/library.py
--rw-r--r--   0        0        0    31359 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/spotify/object.py
--rw-r--r--   0        0        0     8257 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/spotify/processors.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/spotify/api/__init__.py
--rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/spotify/api/api.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/spotify/api/base.py
--rw-r--r--   0        0        0    29516 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/spotify/api/item.py
--rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/spotify/api/misc.py
--rw-r--r--   0        0        0    10529 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/spotify/api/playlist.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 musify-0.9.1/musify/log/__init__.py
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 musify-0.9.1/musify/log/filter.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 musify-0.9.1/musify/log/handlers.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 musify-0.9.1/musify/log/logger.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 musify-0.9.1/musify/processors/__init__.py
--rw-r--r--   0        0        0     8698 2020-02-02 00:00:00.000000 musify-0.9.1/musify/processors/base.py
--rw-r--r--   0        0        0    11527 2020-02-02 00:00:00.000000 musify-0.9.1/musify/processors/compare.py
--rw-r--r--   0        0        0     6573 2020-02-02 00:00:00.000000 musify-0.9.1/musify/processors/download.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 musify-0.9.1/musify/processors/exception.py
--rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 musify-0.9.1/musify/processors/filter.py
--rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 musify-0.9.1/musify/processors/filter_matcher.py
--rw-r--r--   0        0        0     7862 2020-02-02 00:00:00.000000 musify-0.9.1/musify/processors/limit.py
--rw-r--r--   0        0        0    22140 2020-02-02 00:00:00.000000 musify-0.9.1/musify/processors/match.py
--rw-r--r--   0        0        0    10336 2020-02-02 00:00:00.000000 musify-0.9.1/musify/processors/sort.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 musify-0.9.1/musify/processors/time.py
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 musify-0.9.1/.gitignore
--rw-r--r--   0        0        0    35184 2020-02-02 00:00:00.000000 musify-0.9.1/LICENSE
--rw-r--r--   0        0        0    15052 2020-02-02 00:00:00.000000 musify-0.9.1/README.md
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 musify-0.9.1/pyproject.toml
--rw-r--r--   0        0        0    17996 2020-02-02 00:00:00.000000 musify-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 musify-0.9.2/musify/__init__.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 musify-0.9.2/musify/exception.py
+-rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 musify-0.9.2/musify/field.py
+-rw-r--r--   0        0        0     8071 2020-02-02 00:00:00.000000 musify-0.9.2/musify/report.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 musify-0.9.2/musify/types.py
+-rw-r--r--   0        0        0    10127 2020-02-02 00:00:00.000000 musify-0.9.2/musify/utils.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 musify-0.9.2/musify/api/__init__.py
+-rw-r--r--   0        0        0    16025 2020-02-02 00:00:00.000000 musify-0.9.2/musify/api/authorise.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 musify-0.9.2/musify/api/exception.py
+-rw-r--r--   0        0        0    10232 2020-02-02 00:00:00.000000 musify-0.9.2/musify/api/request.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 musify-0.9.2/musify/core/__init__.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 musify-0.9.2/musify/core/base.py
+-rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 musify-0.9.2/musify/core/enum.py
+-rw-r--r--   0        0        0     9315 2020-02-02 00:00:00.000000 musify-0.9.2/musify/core/printer.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 musify-0.9.2/musify/core/result.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 musify-0.9.2/musify/file/__init__.py
+-rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 musify-0.9.2/musify/file/base.py
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 musify-0.9.2/musify/file/exception.py
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 musify-0.9.2/musify/file/image.py
+-rw-r--r--   0        0        0     8152 2020-02-02 00:00:00.000000 musify-0.9.2/musify/file/path_mapper.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/__init__.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/collection.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/core/__init__.py
+-rw-r--r--   0        0        0    15068 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/core/collection.py
+-rw-r--r--   0        0        0    23292 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/core/object.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/local/__init__.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/local/base.py
+-rw-r--r--   0        0        0    19985 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/local/collection.py
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/local/exception.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/local/library/__init__.py
+-rw-r--r--   0        0        0    20851 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/local/library/library.py
+-rw-r--r--   0        0        0    24740 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/local/library/musicbee.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/local/playlist/__init__.py
+-rw-r--r--   0        0        0     5752 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/local/playlist/base.py
+-rw-r--r--   0        0        0     6391 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/local/playlist/m3u.py
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/local/playlist/utils.py
+-rw-r--r--   0        0        0    28389 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/local/playlist/xautopf.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/local/track/__init__.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/local/track/field.py
+-rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/local/track/flac.py
+-rw-r--r--   0        0        0     6687 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/local/track/m4a.py
+-rw-r--r--   0        0        0     7073 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/local/track/mp3.py
+-rw-r--r--   0        0        0    17384 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/local/track/track.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/local/track/utils.py
+-rw-r--r--   0        0        0     5161 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/local/track/wma.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/local/track/tags/__init__.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/local/track/tags/base.py
+-rw-r--r--   0        0        0     7645 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/local/track/tags/reader.py
+-rw-r--r--   0        0        0    32427 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/local/track/tags/writer.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/remote/__init__.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/remote/core/__init__.py
+-rw-r--r--   0        0        0    21825 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/remote/core/api.py
+-rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/remote/core/base.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/remote/core/enum.py
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/remote/core/exception.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/remote/core/factory.py
+-rw-r--r--   0        0        0    22062 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/remote/core/library.py
+-rw-r--r--   0        0        0    12748 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/remote/core/object.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/remote/core/response.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/remote/core/types.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/remote/core/processors/__init__.py
+-rw-r--r--   0        0        0    23087 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/remote/core/processors/check.py
+-rw-r--r--   0        0        0    14928 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/remote/core/processors/search.py
+-rw-r--r--   0        0        0     9804 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/remote/core/processors/wrangle.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/remote/spotify/__init__.py
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/remote/spotify/base.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/remote/spotify/exception.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/remote/spotify/factory.py
+-rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/remote/spotify/library.py
+-rw-r--r--   0        0        0    31359 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/remote/spotify/object.py
+-rw-r--r--   0        0        0     8316 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/remote/spotify/processors.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/remote/spotify/api/__init__.py
+-rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/remote/spotify/api/api.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/remote/spotify/api/base.py
+-rw-r--r--   0        0        0    30068 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/remote/spotify/api/item.py
+-rw-r--r--   0        0        0     5245 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/remote/spotify/api/misc.py
+-rw-r--r--   0        0        0    10598 2020-02-02 00:00:00.000000 musify-0.9.2/musify/libraries/remote/spotify/api/playlist.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 musify-0.9.2/musify/log/__init__.py
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 musify-0.9.2/musify/log/filter.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 musify-0.9.2/musify/log/handlers.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 musify-0.9.2/musify/log/logger.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 musify-0.9.2/musify/processors/__init__.py
+-rw-r--r--   0        0        0     8705 2020-02-02 00:00:00.000000 musify-0.9.2/musify/processors/base.py
+-rw-r--r--   0        0        0    11603 2020-02-02 00:00:00.000000 musify-0.9.2/musify/processors/compare.py
+-rw-r--r--   0        0        0     6578 2020-02-02 00:00:00.000000 musify-0.9.2/musify/processors/download.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 musify-0.9.2/musify/processors/exception.py
+-rw-r--r--   0        0        0     5742 2020-02-02 00:00:00.000000 musify-0.9.2/musify/processors/filter.py
+-rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 musify-0.9.2/musify/processors/filter_matcher.py
+-rw-r--r--   0        0        0     7862 2020-02-02 00:00:00.000000 musify-0.9.2/musify/processors/limit.py
+-rw-r--r--   0        0        0    22199 2020-02-02 00:00:00.000000 musify-0.9.2/musify/processors/match.py
+-rw-r--r--   0        0        0    10336 2020-02-02 00:00:00.000000 musify-0.9.2/musify/processors/sort.py
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 musify-0.9.2/musify/processors/time.py
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 musify-0.9.2/.gitignore
+-rw-r--r--   0        0        0    35184 2020-02-02 00:00:00.000000 musify-0.9.2/LICENSE
+-rw-r--r--   0        0        0    15052 2020-02-02 00:00:00.000000 musify-0.9.2/README.md
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 musify-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0    17996 2020-02-02 00:00:00.000000 musify-0.9.2/PKG-INFO
```

### Comparing `musify-0.9.1/musify/exception.py` & `musify-0.9.2/musify/exception.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/field.py` & `musify-0.9.2/musify/field.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/report.py` & `musify-0.9.2/musify/report.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/types.py` & `musify-0.9.2/musify/types.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/utils.py` & `musify-0.9.2/musify/utils.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/api/authorise.py` & `musify-0.9.2/musify/api/authorise.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/api/exception.py` & `musify-0.9.2/musify/api/exception.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/api/request.py` & `musify-0.9.2/musify/api/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 class RequestHandler(APIAuthoriser):
     """
     Generic API request handler using cached responses for GET requests only.
     Caches GET responses for a maximum of 4 weeks by default.
     Handles error responses and backoff on failed requests.
     See :py:class:`APIAuthoriser` for more info on which params to pass to authorise requests.
 
-    :param cache_path: The path to store the requests session's sqlite cache.
+    :param cache_path: Path to use to store the requests session's sqlite cache.
     :param cache_expiry: The expiry time to apply to cached responses after which responses are invalidated.
     :param auth_kwargs: The authorisation kwargs to be passed to :py:class:`APIAuthoriser`.
     """
 
     __slots__ = ("session", "__dict__")
 
     #: The initial backoff time for failed requests
```

### Comparing `musify-0.9.1/musify/core/base.py` & `musify-0.9.2/musify/core/base.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/core/enum.py` & `musify-0.9.2/musify/core/enum.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/core/printer.py` & `musify-0.9.2/musify/core/printer.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/file/base.py` & `musify-0.9.2/musify/file/base.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/file/exception.py` & `musify-0.9.2/musify/file/exception.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/file/image.py` & `musify-0.9.2/musify/file/image.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/file/path_mapper.py` & `musify-0.9.2/musify/file/path_mapper.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/libraries/collection.py` & `musify-0.9.2/musify/libraries/collection.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/libraries/core/collection.py` & `musify-0.9.2/musify/libraries/core/collection.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/libraries/core/object.py` & `musify-0.9.2/musify/libraries/core/object.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/libraries/local/collection.py` & `musify-0.9.2/musify/libraries/local/collection.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/libraries/local/exception.py` & `musify-0.9.2/musify/libraries/local/exception.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/libraries/local/library/library.py` & `musify-0.9.2/musify/libraries/local/library/library.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/libraries/local/library/musicbee.py` & `musify-0.9.2/musify/libraries/local/library/musicbee.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,22 +51,22 @@
         "_library_xml_parser",
         "settings_xml"
         "_settings_xml_path",
         "_settings_xml_parser",
     )
 
     valid_extensions = frozenset({".xml"})
-    #: The relative path of the playlist folder within the MusicBee folder.
-    xml_library_filename = "iTunes Music Library.xml"
-    #: The filename of the MusicBee library file.
-    xml_library_path_keys = {"Location", "Music Folder"}
+    #: The path of the MusicBee library file relative the ``musicbee_folder`` provided on initialisation.
+    xml_library_path = "iTunes Music Library.xml"
     #: A list of keys for the XML library that need to be processed as system paths.
-    xml_settings_filename = "MusicBeeLibrarySettings.ini"
-    #: The filename of the MusicBee settings file.
-    musicbee_playlist_folder = "Playlists"
+    xml_library_path_keys = {"Location", "Music Folder"}
+    #: The path of the MusicBee settings file relative the ``musicbee_folder`` provided on initialisation.
+    xml_settings_path = "MusicBeeLibrarySettings.ini"
+    #: The path to the playlists folder relative the ``musicbee_folder`` provided on initialisation.
+    playlists_path = "Playlists"
 
     @property
     def path(self) -> str:
         return self._library_xml_path
 
     def __init__(
             self,
@@ -74,37 +74,37 @@
             playlist_filter: Collection[str] | Filter[str] = (),
             path_mapper: PathMapper = PathMapper(),
             remote_wrangler: RemoteDataWrangler = None,
     ):
         #: The absolute path of the musicbee folder containing settings and library files.
         self.musicbee_folder = musicbee_folder
 
-        self._library_xml_path: str = join(musicbee_folder, self.xml_library_filename)
+        self._library_xml_path: str = join(musicbee_folder, self.xml_library_path)
         if not exists(self._library_xml_path):
             raise FileDoesNotExistError(f"Cannot find MusicBee library at given path: {self._library_xml_path}")
 
         self._library_xml_parser = XMLLibraryParser(self._library_xml_path, path_keys=self.xml_library_path_keys)
         #: A map representation of the loaded XML library data
         self.library_xml: dict[str, Any] = self._library_xml_parser.parse()
 
-        self._settings_xml_path: str = join(musicbee_folder, self.xml_settings_filename)
+        self._settings_xml_path: str = join(musicbee_folder, self.xml_settings_path)
         if not exists(self._settings_xml_path):
             raise FileDoesNotExistError(f"Cannot find MusicBee settings at given path: {self._settings_xml_path}")
 
         with open(self._settings_xml_path, "r", encoding="utf-8") as f:
             #: A map representation of the loaded XML settings data
             self.settings_xml: dict[str, Any] = xmltodict.parse(f.read())["ApplicationSettings"]
 
         library_folders = []
         for path in to_collection(self.settings_xml.get("OrganisationMonitoredFolders", {}).get("string")):
             library_folders.append(path_mapper.map(path))
 
         super().__init__(
             library_folders=library_folders,
-            playlist_folder=join(self.musicbee_folder, self.musicbee_playlist_folder),
+            playlist_folder=join(self.musicbee_folder, self.playlists_path),
             playlist_filter=playlist_filter,
             path_mapper=path_mapper,
             remote_wrangler=remote_wrangler,
         )
 
     def _get_track_from_xml_path(
             self, track_xml: dict[str, Any], track_map: dict[str, LocalTrack]
```

### Comparing `musify-0.9.1/musify/libraries/local/playlist/base.py` & `musify-0.9.2/musify/libraries/local/playlist/base.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/libraries/local/playlist/m3u.py` & `musify-0.9.2/musify/libraries/local/playlist/m3u.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/libraries/local/playlist/utils.py` & `musify-0.9.2/musify/libraries/local/playlist/utils.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/libraries/local/playlist/xautopf.py` & `musify-0.9.2/musify/libraries/local/playlist/xautopf.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/libraries/local/track/field.py` & `musify-0.9.2/musify/libraries/local/track/field.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/libraries/local/track/flac.py` & `musify-0.9.2/musify/libraries/local/track/flac.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/libraries/local/track/m4a.py` & `musify-0.9.2/musify/libraries/local/track/m4a.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/libraries/local/track/mp3.py` & `musify-0.9.2/musify/libraries/local/track/mp3.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/libraries/local/track/track.py` & `musify-0.9.2/musify/libraries/local/track/track.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/libraries/local/track/utils.py` & `musify-0.9.2/musify/libraries/local/track/utils.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/libraries/local/track/wma.py` & `musify-0.9.2/musify/libraries/local/track/wma.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/libraries/local/track/tags/base.py` & `musify-0.9.2/musify/libraries/local/track/tags/base.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/libraries/local/track/tags/reader.py` & `musify-0.9.2/musify/libraries/local/track/tags/reader.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/libraries/local/track/tags/writer.py` & `musify-0.9.2/musify/libraries/local/track/tags/writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -399,19 +399,19 @@
         :param source: The source track i.e. the track object representing the currently saved file on the drive.
         :param target: The target track i.e. the track object containing new tags with which to update the file.
         :param replace: Destructively overwrite the tag on the file if the ``source`` and ``target`` tags differ.
         :param dry_run: Run function, but do not modify the file on the disk.
         :return: The index number of the conditional that was met to warrant updating the file's tags.
             None if none of the conditions were met.
         """
-        source_bpm = int(source["bpm"] if source["bpm"] is not None else 0)
-        target_bpm = int(target["bpm"] if target["bpm"] is not None else 0)
+        source_bpm = int(source.bpm if source.bpm is not None else 0)
+        target_bpm = int(target.bpm if target.bpm is not None else 0)
 
         conditionals = {
-            source.bpm is None and target.bpm is not None and target.bpm > 30,
+            source.bpm is None and target.bpm is not None and target_bpm > 30,
             source_bpm < 30 < target_bpm,
             replace and source_bpm != target_bpm
         }
         if any(conditionals) and self._write_bpm(track=target, dry_run=dry_run):
             return [i for i, c in enumerate(conditionals) if c][0]
 
     def _write_bpm(self, track: Track, dry_run: bool = True) -> bool:
```

### Comparing `musify-0.9.1/musify/libraries/remote/core/api.py` & `musify-0.9.2/musify/libraries/remote/core/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -222,27 +222,29 @@
             * A RemoteResponse representing some remote collection of items.
 
         :param value: The value representing some remote collection. See description for allowed value types.
         :param kind: When an ID is provided, give the kind of ID this is here.
             If None and ID is given, user will be prompted to give the kind anyway.
         :param limit: The number of results to call per request and,
             therefore, the number of items in each printed block.
-        :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
+        :param use_cache: When a CachedSession is available, use the cache when calling the API endpoint.
+            Set as False to refresh the cached response of the CachedSession.
         """
         raise NotImplementedError
 
     @abstractmethod
     def get_playlist_url(self, playlist: str | Mapping[str, Any] | RemoteResponse, use_cache: bool = True) -> str:
         """
         Determine the type of the given ``playlist`` and return its API URL.
         If type cannot be determined, attempt to find the playlist in the
         list of the currently authenticated user's playlists.
 
         :param playlist: In URL/URI/ID form, or the name of one of the currently authenticated user's playlists.
-        :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
+        :param use_cache: When a CachedSession is available, use the cache when calling the API endpoint.
+            Set as False to refresh the cached response of the CachedSession.
         :return: The playlist URL.
         :raise RemoteIDTypeError: Raised when the function cannot determine the item type of
             the input ``playlist``. Or when it does not recognise the type of the input ``playlist`` parameter.
         """
         raise NotImplementedError
 
     ###########################################################################
@@ -262,15 +264,16 @@
     ) -> list[dict[str, Any]]:
         """
         ``GET`` - Query for items. Modify result types returned with kind parameter
 
         :param query: Search query.
         :param kind: The remote object type to search for.
         :param limit: Number of results to get and return.
-        :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
+        :param use_cache: When a CachedSession is available, use the cache when calling the API endpoint.
+            Set as False to refresh the cached response of the CachedSession.
         :return: The response from the endpoint.
         """
         raise NotImplementedError
 
     ###########################################################################
     ## Item - GET endpoints
     ###########################################################################
@@ -291,15 +294,16 @@
 
         If a :py:class:`RemoteResponse`, this function will not refresh itself with the new response.
         The user must call `refresh` manually after execution.
 
         :param response: A remote API JSON response for an items type endpoint.
         :param kind: The type of response being extended. Optional, used only for logging.
         :param key: The type of response of the child objects.
-        :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
+        :param use_cache: When a CachedSession is available, use the cache when calling the API endpoint.
+            Set as False to refresh the cached response of the CachedSession.
         :return: API JSON responses for each item
         """
         raise NotImplementedError
 
     @abstractmethod
     def get_items(
             self,
@@ -328,15 +332,16 @@
         :param values: The values representing some remote objects. See description for allowed value types.
             These items must all be of the same type of item i.e. all tracks OR all artists etc.
         :param kind: Item type if given string is ID.
         :param limit: When requests can be batched, size of batches to request.
             This value will be limited to be between ``1`` and ``50``.
         :param extend: When True and the given ``kind`` is a collection of items,
             extend the response to include all items in this collection.
-        :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
+        :param use_cache: When a CachedSession is available, use the cache when calling the API endpoint.
+            Set as False to refresh the cached response of the CachedSession.
         :return: API JSON responses for each item.
         :raise RemoteObjectTypeError: Raised when the function cannot determine the item type
             of the input ``values``. Or when it does not recognise the type of the input ``values`` parameter.
         """
         raise NotImplementedError
 
     @abstractmethod
@@ -360,15 +365,16 @@
         """
         ``GET`` - Get saved items for a given user.
 
         :param user: The ID of the user to get playlists for. If None, use the currently authenticated user.
         :param kind: Item type to retrieve for the user.
         :param limit: Size of each batch of items to request in the collection items request.
             This value will be limited to be between ``1`` and ``50``.
-        :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
+        :param use_cache: When a CachedSession is available, use the cache when calling the API endpoint.
+            Set as False to refresh the cached response of the CachedSession.
         :return: API JSON responses for each collection.
         :raise RemoteIDTypeError: Raised when the input ``user`` does not represent a user URL/URI/ID.
         :raise RemoteObjectTypeError: When the given ``kind`` is not a valid user item/collection.
         """
         raise NotImplementedError
 
     ###########################################################################
```

### Comparing `musify-0.9.1/musify/libraries/remote/core/base.py` & `musify-0.9.2/musify/libraries/remote/core/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,25 +101,27 @@
             * A string representing a URL/URI/ID.
             * A remote API JSON response for a collection with a valid ID value under an ``id`` key.
             * An object of the same type as this collection.
               The remote API JSON response will be used to load a new object.
 
         :param value: The value representing some remote object. See description for allowed value types.
         :param api: An authorised API object to load the object from.
-        :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
+        :param use_cache: When a CachedSession is available, use the cache when calling the API endpoint.
+            Set as False to refresh the cached response of the CachedSession.
         """
         raise NotImplementedError
 
     @abstractmethod
     def reload(self, use_cache: bool = True, *args, **kwargs) -> None:
         """
         Reload this object from the API, calling all required endpoints
         to get a complete set of data for this item type.
 
-        :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
+        :param use_cache: When a CachedSession is available, use the cache when calling the API endpoint.
+            Set as False to refresh the cached response of the CachedSession.
         """
         raise NotImplementedError
 
     def __hash__(self):
         """Uniqueness of a remote object is its URI"""
         return hash(self.uri)
```

### Comparing `musify-0.9.1/musify/libraries/remote/core/enum.py` & `musify-0.9.2/musify/libraries/remote/core/enum.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/libraries/remote/core/exception.py` & `musify-0.9.2/musify/libraries/remote/core/exception.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/libraries/remote/core/factory.py` & `musify-0.9.2/musify/libraries/remote/core/factory.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/libraries/remote/core/library.py` & `musify-0.9.2/musify/libraries/remote/core/library.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,16 @@
     """
     Represents a remote library, providing various methods for manipulating
     tracks and playlists across an entire remote library collection.
 
     :param api: The instantiated and authorised API object for this source type.
     :param playlist_filter: An optional :py:class:`Filter` to apply or collection of playlist names to include when
         loading playlists. Playlist names will be passed to this filter to limit which playlists are loaded.
-    :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
+    :param use_cache: Use the cache when calling the API endpoint.
+        When using a CachedSession, set as False to refresh the cached response.
     """
 
     __slots__ = ("_factory", "_tracks", "_playlists", "playlist_filter")
     __attributes_classes__ = (Library, RemoteCollection)
     __attributes_ignore__ = ("api", "factory")
 
     @property
@@ -119,18 +120,19 @@
 
         self.logger.info(
             f"\33[1;95m  >\33[1;97m Extending {self.api.source} library "
             f"with {len(load_uris)} additional tracks \33[0m"
         )
 
         load_tracks = self.api.get_tracks(load_uris, features=True, use_cache=self.use_cache)
-        self.items.extend(self.factory.track(response=response) for response in load_tracks)
+        self.items.extend(map(self.factory.track, load_tracks))
 
-        self.logger.print()
+        self.logger.print(STAT)
         self.log_tracks()
+        self.logger.print()
         self.logger.debug(f"Extend {self.api.source} tracks data: DONE\n")
 
     def load(self) -> None:
         """Loads all data from the remote API for this library and log results."""
         self.logger.debug(f"Load {self.api.source} library: START")
         self.logger.info(f"\33[1;95m ->\33[1;97m Loading {self.api.source} library \33[0m")
```

### Comparing `musify-0.9.1/musify/libraries/remote/core/object.py` & `musify-0.9.2/musify/libraries/remote/core/object.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,16 @@
               The remote API JSON response will be used to load a new object.
 
         You may also provide a set of kwargs relating that will extend aspects of the response
         before using it to initialise a new object. See :py:meth:`reload` for possible extensions.
 
         :param value: The value representing some remote collection. See description for allowed value types.
         :param api: An authorised API object to load the object from.
-        :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
+        :param use_cache: When a CachedSession is available, use the cache when calling the API endpoint.
+            Set as False to refresh the cached response of the CachedSession.
         :param items: Optionally, give a list of available items to build a response for this collection.
             In doing so, the method will first try to find the API responses for the items of this collection
             in the given list before calling the API for any items not found there.
             This helps reduce the number of API calls made on initialisation.
         """
         raise NotImplementedError
```

### Comparing `musify-0.9.1/musify/libraries/remote/core/response.py` & `musify-0.9.2/musify/libraries/remote/core/response.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/libraries/remote/core/processors/check.py` & `musify-0.9.2/musify/libraries/remote/core/processors/check.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/libraries/remote/core/processors/search.py` & `musify-0.9.2/musify/libraries/remote/core/processors/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,16 @@
     """
     Searches for remote matches for a list of item collections.
 
     :param matcher: The :py:class:`ItemMatcher` to use when comparing any changes made by the user in remote playlists
         during the checking operation
     :param object_factory: The :py:class:`RemoteObjectFactory` to use when creating new remote objects.
         This must have a :py:class:`RemoteAPI` assigned for this processor to work as expected.
-    :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
+    :param use_cache: Use the cache when calling the API endpoint.
+        When using a CachedSession, set as False to refresh the cached response.
     """
 
     __slots__ = ("factory", "use_cache")
 
     #: The :py:class:`SearchSettings` for each :py:class:`RemoteObjectType`
     search_settings: dict[RemoteObjectType, SearchConfig] = {
         RemoteObjectType.TRACK: SearchConfig(
```

### Comparing `musify-0.9.1/musify/libraries/remote/core/processors/wrangle.py` & `musify-0.9.2/musify/libraries/remote/core/processors/wrangle.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/libraries/remote/spotify/base.py` & `musify-0.9.2/musify/libraries/remote/spotify/base.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/libraries/remote/spotify/exception.py` & `musify-0.9.2/musify/libraries/remote/spotify/exception.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/libraries/remote/spotify/factory.py` & `musify-0.9.2/musify/libraries/remote/spotify/factory.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/libraries/remote/spotify/library.py` & `musify-0.9.2/musify/libraries/remote/spotify/library.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/libraries/remote/spotify/object.py` & `musify-0.9.2/musify/libraries/remote/spotify/object.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/libraries/remote/spotify/processors.py` & `musify-0.9.2/musify/libraries/remote/spotify/processors.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 from musify.exception import MusifyEnumError
 from musify.libraries.core.collection import MusifyCollection
 from musify.libraries.remote.core import RemoteResponse
 from musify.libraries.remote.core.api import APIInputValue
 from musify.libraries.remote.core.enum import RemoteIDType, RemoteObjectType
 from musify.libraries.remote.core.exception import RemoteError, RemoteIDTypeError, RemoteObjectTypeError
 from musify.libraries.remote.core.processors.wrangle import RemoteDataWrangler
+from musify.libraries.remote.spotify import SOURCE_NAME
 from musify.utils import to_collection
 
 
 class SpotifyDataWrangler(RemoteDataWrangler):
 
-    source = "Spotify"
+    source = SOURCE_NAME
     unavailable_uri_dummy = "spotify:track:unavailable"
     url_api = "https://api.spotify.com/v1"
     url_ext = "https://open.spotify.com"
 
     @classmethod
     def get_id_type(cls, value: str, kind: RemoteObjectType | None = None) -> RemoteIDType:
         value = value.strip().casefold()
```

### Comparing `musify-0.9.1/musify/libraries/remote/spotify/api/api.py` & `musify-0.9.2/musify/libraries/remote/spotify/api/api.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/libraries/remote/spotify/api/base.py` & `musify-0.9.2/musify/libraries/remote/spotify/api/base.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/libraries/remote/spotify/api/item.py` & `musify-0.9.2/musify/libraries/remote/spotify/api/item.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,16 @@
         This function executes each URL request individually for each ID i.e. ``URL`` or ``ID``.
 
         :param url: The base API URL endpoint for the required requests.
         :param id_list: List of IDs to append to the given URL.
         :param params: Extra parameters to add to each request.
         :param kind: The unit to use for logging. If None, determine from ``key`` or default to ``items``.
         :param key: The key to reference from each response to get the list of required values.
-        :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
+        :param use_cache: When a CachedSession is available, use the cache when calling the API endpoint.
+            Set as False to refresh the cached response of the CachedSession.
         :return: API JSON responses for each item at the given ``key``.
         :raise APIError: When the given ``key`` is not in the API response.
         """
         url = url.rstrip("/")
         kind = self._get_unit(key=key, kind=kind)
 
         bar = self.logger.get_progress_bar(
@@ -97,15 +98,16 @@
         ``{<IDs>: '<comma separated string of IDs>'}``
 
         :param url: The base API URL endpoint for the required requests.
         :param id_list: List of IDs to append to the given URL.
         :param params: Extra parameters to add to each request.
         :param kind: The unit to use for logging. If None, determine from ``key`` or default to ``items``.
         :param key: The key to reference from each response to get the list of required values.
-        :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
+        :param use_cache: When a CachedSession is available, use the cache when calling the API endpoint.
+            Set as False to refresh the cached response of the CachedSession.
         :param limit: Size of each batch of IDs to get. This value will be limited to be between ``1`` and ``50``.
         :return: API JSON responses for each item at the given ``key``.
         :raise APIError: When the given ``key`` is not in the API response.
         """
         url = url.rstrip("/")
         kind = self._get_unit(key=key, kind=kind)
 
@@ -156,15 +158,16 @@
         :param response: A remote API JSON response for an items type endpoint
             or a RemoteResponse which contains this response.
             Must include required keys:
             ``total`` and either ``next`` or ``href``, plus optional keys ``previous``, ``limit``, ``items`` etc.
         :param kind: The type of response being extended. Optional, used only for logging.
         :param key: The type of response of the child objects. Used when selecting nested data for certain responses
             (e.g. user's followed artists).
-        :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
+        :param use_cache: When a CachedSession is available, use the cache when calling the API endpoint.
+            Set as False to refresh the cached response of the CachedSession.
         :param leave_bar: When a progress bar is displayed,
             toggle whether this bar should continue to be displayed after the operation is finished.
             When None, allow the logger to decide this setting.
         :return: API JSON responses for each item
         """
         if isinstance(response, RemoteResponse):
             response = response.response
@@ -248,15 +251,16 @@
         :param values: The values representing some remote objects. See description for allowed value types.
             These items must all be of the same type of item i.e. all tracks OR all artists etc.
         :param kind: Item type if given string is ID.
         :param limit: When requests can be batched, size of batches to request.
             This value will be limited to be between ``1`` and ``50`` or ``20`` if getting albums.
         :param extend: When True and the given ``kind`` is a collection of items,
             extend the response to include all items in this collection.
-        :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
+        :param use_cache: When a CachedSession is available, use the cache when calling the API endpoint.
+            Set as False to refresh the cached response of the CachedSession.
         :return: API JSON responses for each item.
         :raise RemoteObjectTypeError: Raised when the function cannot determine the item type
             of the input ``values``. Or when it does not recognise the type of the input ``values`` parameter.
         """
         # input validation
         if not isinstance(values, RemoteResponse) and not values:  # skip on empty
             url = f"{self.url}/{kind.name.lower() + "s"}" if kind else self.url
@@ -315,15 +319,16 @@
         ``GET: /{kind}s`` - Get saved items for a given user.
 
         :param user: The ID of the user to get playlists for. If None, use the currently authenticated user.
         :param kind: Item type to retrieve for the user.
             Spotify only supports ``PLAYLIST`` types for non-authenticated users.
         :param limit: Size of each batch of items to request in the collection items request.
             This value will be limited to be between ``1`` and ``50``.
-        :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
+        :param use_cache: When a CachedSession is available, use the cache when calling the API endpoint.
+            Set as False to refresh the cached response of the CachedSession.
         :return: API JSON responses for each collection.
         :raise RemoteIDTypeError: Raised when the input ``user`` does not represent a user URL/URI/ID.
         :raise RemoteObjectTypeError: Raised a user is given and the ``kind`` is not ``PLAYLIST``.
             Or when the given ``kind`` is not a valid collection.
         """
         # input validation
         if kind not in self.user_item_types:
@@ -383,15 +388,16 @@
         If :py:class:`RemoteResponse` values are given, this function will call `refresh` on them.
 
         :param values: The values representing some remote track/s. See description for allowed value types.
         :param features: When True, get audio features.
         :param analysis: When True, get audio analysis.
         :param limit: Size of batches to request when getting audio features.
             This value will be limited to be between ``1`` and ``50``.
-        :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
+        :param use_cache: When a CachedSession is available, use the cache when calling the API endpoint.
+            Set as False to refresh the cached response of the CachedSession.
         :return: API JSON responses for each item.
             Mapped to ``audio_features`` and ``audio_analysis`` keys as appropriate.
         :raise RemoteObjectTypeError: Raised when the item types of the input ``values`` are not all tracks or IDs.
         """
         # input validation
         if not features and not analysis:  # skip on all False
             return []
@@ -479,15 +485,16 @@
         under the ``audio_features`` and ``audio_analysis`` keys as appropriate.
 
         :param values: The values representing some remote track/s. See description for allowed value types.
         :param features: When True, get audio features.
         :param analysis: When True, get audio analysis.
         :param limit: Size of batches to request when getting audio features.
             This value will be limited to be between ``1`` and ``50``.
-        :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
+        :param use_cache: When a CachedSession is available, use the cache when calling the API endpoint.
+            Set as False to refresh the cached response of the CachedSession.
         :return: API JSON responses for each item, or the original response if the input ``values`` are API responses.
         :raise RemoteObjectTypeError: Raised when the item types of the input ``values`` are not all tracks or IDs.
         """
         tracks = self.get_items(values=values, kind=RemoteObjectType.TRACK, limit=limit, use_cache=use_cache)
 
         # ensure that response are being assigned back to the original values if API response(s) given
         if isinstance(values, Mapping | RemoteResponse):
@@ -521,15 +528,16 @@
 
         If :py:class:`RemoteResponse` values are given, this function will call `refresh` on them.
 
         :param values: The values representing some remote artist/s. See description for allowed value types.
         :param types: The types of albums to return. Select from ``{"album", "single", "compilation", "appears_on"}``.
         :param limit: Size of batches to request.
             This value will be limited to be between ``1`` and ``50``.
-        :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
+        :param use_cache: When a CachedSession is available, use the cache when calling the API endpoint.
+            Set as False to refresh the cached response of the CachedSession.
         :return: A map of the Artist ID to a list of the API JSON responses for each album.
         :raise RemoteObjectTypeError: Raised when the item types of the input ``values`` are not all artists or IDs.
         """
         url = f"{self.url}/artists/{{id}}/albums"
 
         # input validation
         if not isinstance(values, RemoteResponse) and not values:  # skip on empty
```

### Comparing `musify-0.9.1/musify/libraries/remote/spotify/api/misc.py` & `musify-0.9.2/musify/libraries/remote/spotify/api/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,16 @@
     ) -> list[dict[str, Any]]:
         """
         ``GET: /search`` - Query for items. Modify result types returned with kind parameter
 
         :param query: Search query.
         :param kind: The remote object type to search for.
         :param limit: Number of results to get and return.
-        :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
+        :param use_cache: When a CachedSession is available, use the cache when calling the API endpoint.
+            Set as False to refresh the cached response of the CachedSession.
         :return: The response from the endpoint.
         """
         if not query or len(query) > 150:  # query is too short or too long, skip
             return []
 
         url = f"{self.url}/search"
         params = {'q': query, "type": kind.name.lower(), "limit": limit_value(limit, floor=1, ceil=50)}
```

### Comparing `musify-0.9.1/musify/libraries/remote/spotify/api/playlist.py` & `musify-0.9.2/musify/libraries/remote/spotify/api/playlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,16 @@
         list of the currently authorised user's playlists.
 
         :param playlist: One of the following to identify the playlist URL:
             - playlist URL/URI/ID,
             - the name of the playlist in the current user's playlists,
             - the API response of a playlist.
             - a RemoteResponse object representing a remote playlist.
-        :param use_cache: Use the cache when calling the API endpoint. Set as False to refresh the cached response.
+        :param use_cache: When a CachedSession is available, use the cache when calling the API endpoint.
+            Set as False to refresh the cached response of the CachedSession.
         :return: The playlist URL.
         :raise RemoteIDTypeError: Raised when the function cannot determine the item type of
             the input ``playlist``. Or when it does not recognise the type of the input ``playlist`` parameter.
         """
         if isinstance(playlist, RemoteResponse):
             playlist = playlist.response
```

### Comparing `musify-0.9.1/musify/log/filter.py` & `musify-0.9.2/musify/log/filter.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/log/handlers.py` & `musify-0.9.2/musify/log/handlers.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/log/logger.py` & `musify-0.9.2/musify/log/logger.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/processors/base.py` & `musify-0.9.2/musify/processors/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         self.alternative_names = tuple(a for a in args if isinstance(a, str))
         self.instance_ = None
 
     def __get__(self, instance, owner):
         self.instance_ = instance
         return self.__call__
 
-    def __call__(self, *args, **kwargs):
+    def __call__(self, *args, **kwargs) -> Any:
         return self.func(self.instance_, *args, **kwargs) if self.instance_ else self.func(*args, **kwargs)
 
 
 # noinspection SpellCheckingInspection
 class DynamicProcessor(Processor, metaclass=ABCMeta):
     """
     Base class for implementations with :py:func:`dynamicprocessormethod` methods.
```

### Comparing `musify-0.9.1/musify/processors/compare.py` & `musify-0.9.2/musify/processors/compare.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,20 +120,22 @@
 
         if isinstance(value, int):
             self._convert_expected_to_int()
             self._converted = True
         elif isinstance(value, float):
             self._convert_expected_to_float()
             self._converted = True
-        elif isinstance(value, date):
+        elif isinstance(value, datetime):
             self._convert_expected_to_datetime()
             self._converted = True
         elif isinstance(value, bool):
             self._expected.clear()
             self._converted = True
+        elif isinstance(value, str):
+            self._converted = True
 
     def _convert_expected_to_int(self) -> None:
         """Convert expected values to integers"""
         converted: list[int] = []
         for exp in self.expected:
             if isinstance(exp, str) and ":" in exp:
                 # value is a string representation of time
```

### Comparing `musify-0.9.1/musify/processors/download.py` & `musify-0.9.2/musify/processors/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     :param urls: The template URLs for websites to open queries for.
         The given sites should contain exactly 1 '{}' placeholder into which the processor can place
         a query for the item being searched. e.g. *bandcamp.com/search?q={}&item_type=t*
     :param fields: The default fields to take from an item for use as the query string when initially opening sites.
     :param interval: The number of items to open sites for before pausing for user input.
     """
 
-    def __init__(self, urls: UnitIterable[str], fields: UnitIterable[Field] = Fields.ALL, interval: int = 1):
+    def __init__(self, urls: UnitIterable[str] = (), fields: UnitIterable[Field] = Fields.ALL, interval: int = 1):
         super().__init__()
 
         self.urls: list[str] = to_collection(urls, list)
         if fields == Fields.ALL or Fields.ALL in to_collection(fields, set):
             fields = Fields.all()
         self.fields: list[Field] = to_collection(fields, list)
         self.interval = interval
```

### Comparing `musify-0.9.1/musify/processors/exception.py` & `musify-0.9.2/musify/processors/exception.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/processors/filter.py` & `musify-0.9.2/musify/processors/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from collections.abc import Collection, Sequence, Mapping
 from typing import Any, Self
 
 from musify.core.base import MusifyObject
 from musify.processors.base import Filter, FilterComposite
 from musify.processors.compare import Comparer
+from musify.types import UnitCollection
 
 
 class FilterDefinedList[T: str | MusifyObject](Filter[T], Collection[T]):
 
     __slots__ = ("values",)
 
     @property
@@ -56,20 +57,22 @@
 
     @property
     def ready(self):
         return len(self.comparers) > 0
 
     def __init__(
             self,
-            comparers: Collection[Comparer] | Mapping[Comparer, tuple[bool, Self]] = (),
+            comparers: UnitCollection[Comparer] | Mapping[Comparer, tuple[bool, Self]] = (),
             match_all: bool = True,
             *_,
             **__
     ):
         super().__init__()
+        if isinstance(comparers, Comparer):
+            comparers = [comparers]
         if not isinstance(comparers, Mapping):
             comparers = {comparer: (False, FilterComparers()) for comparer in comparers}
 
         #: The comparers to use when processing for this filter
         #: When a mapping with other :py:class:`FilterComparers` is given,
         #: will apply this sub-filter to all parent filters when processing
         self.comparers: Mapping[Comparer, tuple[bool, Self]] = comparers
```

### Comparing `musify-0.9.1/musify/processors/filter_matcher.py` & `musify-0.9.2/musify/processors/filter_matcher.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/processors/limit.py` & `musify-0.9.2/musify/processors/limit.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/processors/match.py` & `musify-0.9.2/musify/processors/match.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,18 +98,23 @@
         """Wrapper for initially logging an algorithm in a uniform aligned format"""
         algorithm = inspect.stack()[1][0].f_code.co_name.upper().lstrip("_").replace("_", " ")
         log = [source.name, algorithm]
         if extra:
             log.extend(extra)
         self.log_messages(log, pad='>')
 
-    def _log_test[T: MusifyObject](self, source: T, result: T, test: Any, extra: Iterable[str] = ()) -> None:
+    def _log_test[T: MusifyObject](self, source: T, result: T | None, test: Any, extra: Iterable[str] = ()) -> None:
         """Wrapper for initially logging a test result in a uniform aligned format"""
         algorithm = inspect.stack()[1][0].f_code.co_name.replace("match", "").upper().lstrip("_").replace("_", " ")
-        log_result = f"> Testing URI: {result.uri}" if hasattr(result, "uri") else "> Test failed"
+
+        if result is not None and hasattr(result, "uri"):
+            log_result = f"> Testing URI: {result.uri}"
+        else:
+            log_result = "> Test failed"
+
         log = [source.name, log_result, f"{algorithm:<10}={test:<5}"]
         if extra:
             log.extend(extra)
         self.log_messages(log)
 
     def _log_match[T: MusifyObject](self, source: T, result: T, extra: Iterable[str] = ()) -> None:
         """Wrapper for initially logging a match in a correctly aligned format"""
@@ -323,18 +328,18 @@
             extra = [
                 f"best score: {score:.2f} > {min_score:.2f}"
                 if score < max_score else
                 f"max score reached: {score:.2f} > {max_score:.2f}"
             ]
             self._log_match(source=source, result=result, extra=extra)
             return result
-        else:
-            self._log_test(
-                source=source, result=result, test=score, extra=[f"NO MATCH: {score:.2f}<{min_score:.2f}"]
-            )
+
+        self._log_test(
+            source=source, result=result, test=score, extra=[f"NO MATCH: {score:.2f}<{min_score:.2f}"]
+        )
 
     def _score[T: MusifyObject](
             self,
             source: T,
             results: Iterable[T],
             executor: Executor,
             match_on: set[TagField] = ALL_TAG_FIELDS,
@@ -415,16 +420,16 @@
                     source=item, results=result.items, match_on=match_on, allow_karaoke=allow_karaoke, executor=executor
                 )
                 for _, item_score in item_scores:
                     scores[Tag.ALL].append([score for score in item_score.values() if not isinstance(score, list)])
 
         return scores
 
+    @staticmethod
     def _get_match_from_scores[T: MusifyObject](
-            self,
             scores: Iterable[tuple[T, dict[TagField, Future[float] | list[list[Future[float]]]]]],
             max_score: float,
     ) -> tuple[T | None, float]:
         best_result = None
         best_score = 0
 
         def sum_nested_scores(futures: list[list[Future[float]]]) -> float:
```

### Comparing `musify-0.9.1/musify/processors/sort.py` & `musify-0.9.2/musify/processors/sort.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/musify/processors/time.py` & `musify-0.9.2/musify/processors/time.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     def _processor_method_fmt(cls, name: str) -> str:
         return name.casefold().strip()[0] if not name.startswith("min") else name
 
     def __init__(self, func: str):
         super().__init__()
         self._set_processor_name(func)
 
-    def __call__(self, *args, **kwargs):
+    def __call__(self, *args, **kwargs) -> timedelta | relativedelta:
         return self.map(*args, **kwargs)
 
     def map(self, value: Any):
         """Run the mapping function"""
         return super().__call__(value)
 
     @dynamicprocessormethod
```

### Comparing `musify-0.9.1/.gitignore` & `musify-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/LICENSE` & `musify-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/README.md` & `musify-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/pyproject.toml` & `musify-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `musify-0.9.1/PKG-INFO` & `musify-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: musify
-Version: 0.9.1
+Version: 0.9.2
 Summary: Synchronise your music library to local or remote libraries
 Project-URL: Documentation, https://geo-martino.github.io/musify/
 Project-URL: Release Notes, https://geo-martino.github.io/musify/release-history.html
 Project-URL: Contribute, https://geo-martino.github.io/musify/contributing.html
 Project-URL: Source code, https://github.com/geo-martino/musify
 Project-URL: Issues, https://github.com/geo-martino/musify/issues
 Author-email: George Martin Marino <gm.engineer+musify@pm.me>
```

