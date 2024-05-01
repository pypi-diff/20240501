# Comparing `tmp/python_docx-1.1.1.tar.gz` & `tmp/python_docx-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_docx-1.1.1.tar", last modified: Tue Apr 30 02:58:01 2024, max compression
+gzip compressed data, was "python_docx-1.1.2.tar", last modified: Wed May  1 19:41:40 2024, max compression
```

## Comparing `python_docx-1.1.1.tar` & `python_docx-1.1.2.tar`

### file list

```diff
@@ -1,576 +1,576 @@
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.649204 python_docx-1.1.1/
--rw-r--r--   0 scanny     (501) staff       (20)     7288 2024-04-30 02:51:57.000000 python_docx-1.1.1/HISTORY.rst
--rw-r--r--   0 scanny     (501) staff       (20)     1104 2014-03-01 10:03:55.000000 python_docx-1.1.1/LICENSE
--rw-r--r--   0 scanny     (501) staff       (20)      230 2023-11-04 03:19:46.000000 python_docx-1.1.1/MANIFEST.in
--rw-r--r--   0 scanny     (501) staff       (20)     2008 2024-04-30 02:58:01.648824 python_docx-1.1.1/PKG-INFO
--rw-r--r--   0 scanny     (501) staff       (20)      642 2023-11-04 03:19:46.000000 python_docx-1.1.1/README.md
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.555899 python_docx-1.1.1/docs/
--rw-r--r--   0 scanny     (501) staff       (20)     5580 2014-03-01 10:03:55.000000 python_docx-1.1.1/docs/Makefile
--rw-r--r--   0 scanny     (501) staff       (20)      939 2014-06-22 21:06:59.000000 python_docx-1.1.1/docs/Session.vim
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.556069 python_docx-1.1.1/docs/_static/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python_docx-1.1.1/docs/_static/.gitignore
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.556631 python_docx-1.1.1/docs/_static/img/
--rw-r--r--   0 scanny     (501) staff       (20)    77526 2014-03-01 10:03:55.000000 python_docx-1.1.1/docs/_static/img/example-docx-01.png
--rw-r--r--   0 scanny     (501) staff       (20)    56762 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/_static/img/hdrftr-01.png
--rw-r--r--   0 scanny     (501) staff       (20)    16218 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/_static/img/hdrftr-02.png
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.556856 python_docx-1.1.1/docs/_templates/
--rw-r--r--   0 scanny     (501) staff       (20)      299 2014-03-01 10:03:55.000000 python_docx-1.1.1/docs/_templates/sidebarlinks.html
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.547249 python_docx-1.1.1/docs/_themes/
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.557621 python_docx-1.1.1/docs/_themes/armstrong/
--rw-r--r--   0 scanny     (501) staff       (20)     1164 2014-01-06 15:34:59.000000 python_docx-1.1.1/docs/_themes/armstrong/LICENSE
--rw-r--r--   0 scanny     (501) staff       (20)     1661 2014-01-06 15:34:59.000000 python_docx-1.1.1/docs/_themes/armstrong/layout.html
--rw-r--r--   0 scanny     (501) staff       (20)     1147 2014-01-06 15:34:59.000000 python_docx-1.1.1/docs/_themes/armstrong/rtd-themes.conf
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.557757 python_docx-1.1.1/docs/_themes/armstrong/static/
--rw-r--r--   0 scanny     (501) staff       (20)    16885 2014-01-06 15:34:59.000000 python_docx-1.1.1/docs/_themes/armstrong/static/rtd.css_t
--rw-r--r--   0 scanny     (501) staff       (20)     1147 2014-01-06 15:34:59.000000 python_docx-1.1.1/docs/_themes/armstrong/theme.conf
--rw-r--r--   0 scanny     (501) staff       (20)     1400 2014-01-06 15:34:59.000000 python_docx-1.1.1/docs/_themes/armstrong/theme.conf.orig
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.559277 python_docx-1.1.1/docs/api/
--rw-r--r--   0 scanny     (501) staff       (20)      255 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/dml.rst
--rw-r--r--   0 scanny     (501) staff       (20)     3363 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/document.rst
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.561700 python_docx-1.1.1/docs/api/enum/
--rw-r--r--   0 scanny     (501) staff       (20)      382 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/enum/MsoColorType.rst
--rw-r--r--   0 scanny     (501) staff       (20)     1270 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/enum/MsoThemeColorIndex.rst
--rw-r--r--   0 scanny     (501) staff       (20)      791 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/enum/WdAlignParagraph.rst
--rw-r--r--   0 scanny     (501) staff       (20)     4567 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/enum/WdBuiltinStyle.rst
--rw-r--r--   0 scanny     (501) staff       (20)      804 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/enum/WdCellVerticalAlignment.rst
--rw-r--r--   0 scanny     (501) staff       (20)      692 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/enum/WdColorIndex.rst
--rw-r--r--   0 scanny     (501) staff       (20)      771 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/enum/WdLineSpacing.rst
--rw-r--r--   0 scanny     (501) staff       (20)      339 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/enum/WdOrientation.rst
--rw-r--r--   0 scanny     (501) staff       (20)      336 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/enum/WdRowAlignment.rst
--rw-r--r--   0 scanny     (501) staff       (20)      519 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/enum/WdRowHeightRule.rst
--rw-r--r--   0 scanny     (501) staff       (20)      486 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/enum/WdSectionStart.rst
--rw-r--r--   0 scanny     (501) staff       (20)      421 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/enum/WdStyleType.rst
--rw-r--r--   0 scanny     (501) staff       (20)      434 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/enum/WdTabAlignment.rst
--rw-r--r--   0 scanny     (501) staff       (20)      285 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/enum/WdTabLeader.rst
--rw-r--r--   0 scanny     (501) staff       (20)      495 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/enum/WdTableDirection.rst
--rw-r--r--   0 scanny     (501) staff       (20)     1334 2014-06-22 22:15:58.000000 python_docx-1.1.1/docs/api/enum/WdUnderline.rst
--rw-r--r--   0 scanny     (501) staff       (20)      446 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/enum/index.rst
--rw-r--r--   0 scanny     (501) staff       (20)      565 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/section.rst
--rw-r--r--   0 scanny     (501) staff       (20)      206 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/settings.rst
--rw-r--r--   0 scanny     (501) staff       (20)      613 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/shape.rst
--rw-r--r--   0 scanny     (501) staff       (20)     1174 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/shared.rst
--rw-r--r--   0 scanny     (501) staff       (20)     1804 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/style.rst
--rw-r--r--   0 scanny     (501) staff       (20)      671 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/table.rst
--rw-r--r--   0 scanny     (501) staff       (20)     1008 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/api/text.rst
--rw-r--r--   0 scanny     (501) staff       (20)    11139 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/conf.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.547753 python_docx-1.1.1/docs/dev/
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.561856 python_docx-1.1.1/docs/dev/analysis/
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.562605 python_docx-1.1.1/docs/dev/analysis/features/
--rw-r--r--   0 scanny     (501) staff       (20)     7557 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/coreprops.rst
--rw-r--r--   0 scanny     (501) staff       (20)    11261 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/header.rst
--rw-r--r--   0 scanny     (501) staff       (20)     2015 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/numbering.rst
--rw-r--r--   0 scanny     (501) staff       (20)    10642 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/sections.rst
--rw-r--r--   0 scanny     (501) staff       (20)    13252 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/settings.rst
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.563273 python_docx-1.1.1/docs/dev/analysis/features/shapes/
--rw-r--r--   0 scanny     (501) staff       (20)     1935 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/shapes/index.rst
--rw-r--r--   0 scanny     (501) staff       (20)     9428 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/shapes/picture.rst
--rw-r--r--   0 scanny     (501) staff       (20)     3459 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/shapes/shapes-inline-size.rst
--rw-r--r--   0 scanny     (501) staff       (20)     6584 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/shapes/shapes-inline.rst
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.564256 python_docx-1.1.1/docs/dev/analysis/features/styles/
--rw-r--r--   0 scanny     (501) staff       (20)     5471 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/styles/character-style.rst
--rw-r--r--   0 scanny     (501) staff       (20)    12771 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/styles/index.rst
--rw-r--r--   0 scanny     (501) staff       (20)     8560 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/styles/latent-styles.rst
--rw-r--r--   0 scanny     (501) staff       (20)     5508 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/styles/paragraph-style.rst
--rw-r--r--   0 scanny     (501) staff       (20)    13979 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/styles/style.rst
--rw-r--r--   0 scanny     (501) staff       (20)     8145 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/styles/styles.rst
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.565008 python_docx-1.1.1/docs/dev/analysis/features/table/
--rw-r--r--   0 scanny     (501) staff       (20)    20675 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/table/cell-merge.rst
--rw-r--r--   0 scanny     (501) staff       (20)     9218 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/table/index.rst
--rw-r--r--   0 scanny     (501) staff       (20)     8041 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/table/table-cell.rst
--rw-r--r--   0 scanny     (501) staff       (20)     7949 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/table/table-props.rst
--rw-r--r--   0 scanny     (501) staff       (20)     4150 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/table/table-row.rst
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.566561 python_docx-1.1.1/docs/dev/analysis/features/text/
--rw-r--r--   0 scanny     (501) staff       (20)     7581 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/text/breaks.rst
--rw-r--r--   0 scanny     (501) staff       (20)     9879 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/text/font-color.rst
--rw-r--r--   0 scanny     (501) staff       (20)     5902 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/text/font-highlight-color.rst
--rw-r--r--   0 scanny     (501) staff       (20)    18391 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/text/font.rst
--rw-r--r--   0 scanny     (501) staff       (20)    13033 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/text/hyperlink.rst
--rw-r--r--   0 scanny     (501) staff       (20)      172 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/text/index.rst
--rw-r--r--   0 scanny     (501) staff       (20)    16282 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/text/paragraph-format.rst
--rw-r--r--   0 scanny     (501) staff       (20)     3094 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/text/run-content.rst
--rw-r--r--   0 scanny     (501) staff       (20)     9567 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/text/tab-stops.rst
--rw-r--r--   0 scanny     (501) staff       (20)     4247 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/features/text/underline.rst
--rw-r--r--   0 scanny     (501) staff       (20)      576 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/index.rst
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.566982 python_docx-1.1.1/docs/dev/analysis/schema/
--rw-r--r--   0 scanny     (501) staff       (20)     7226 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/schema/ct_body.rst
--rw-r--r--   0 scanny     (501) staff       (20)     4659 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/schema/ct_document.rst
--rw-r--r--   0 scanny     (501) staff       (20)     6406 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/dev/analysis/schema/ct_p.rst
--rw-r--r--   0 scanny     (501) staff       (20)     3839 2024-04-30 00:55:22.000000 python_docx-1.1.1/docs/index.rst
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.568626 python_docx-1.1.1/docs/user/
--rw-r--r--   0 scanny     (501) staff       (20)     1287 2014-01-06 15:34:59.000000 python_docx-1.1.1/docs/user/api-concepts.rst
--rw-r--r--   0 scanny     (501) staff       (20)     3635 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/user/documents.rst
--rw-r--r--   0 scanny     (501) staff       (20)     6897 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/user/hdrftr.rst
--rw-r--r--   0 scanny     (501) staff       (20)     1031 2014-03-01 09:49:51.000000 python_docx-1.1.1/docs/user/install.rst
--rw-r--r--   0 scanny     (501) staff       (20)    11875 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/user/quickstart.rst
--rw-r--r--   0 scanny     (501) staff       (20)     3950 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/user/sections.rst
--rw-r--r--   0 scanny     (501) staff       (20)     1477 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/user/shapes.rst
--rw-r--r--   0 scanny     (501) staff       (20)    12392 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/user/styles-understanding.rst
--rw-r--r--   0 scanny     (501) staff       (20)    13587 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/user/styles-using.rst
--rw-r--r--   0 scanny     (501) staff       (20)     6981 2024-04-30 00:55:22.000000 python_docx-1.1.1/docs/user/tables.rst
--rw-r--r--   0 scanny     (501) staff       (20)    14125 2023-11-04 03:19:46.000000 python_docx-1.1.1/docs/user/text.rst
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.578871 python_docx-1.1.1/features/
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.579016 python_docx-1.1.1/features/_scratch/
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.579223 python_docx-1.1.1/features/_scratch/test_out/
--rw-r--r--   0 scanny     (501) staff       (20)     1738 2013-08-15 22:17:06.000000 python_docx-1.1.1/features/_scratch/test_out/[Content_Types].xml
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.579374 python_docx-1.1.1/features/_scratch/test_out/_rels/
--rw-r--r--   0 scanny     (501) staff       (20)      734 2013-08-13 09:49:22.000000 python_docx-1.1.1/features/_scratch/test_out/_rels/.rels
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.579656 python_docx-1.1.1/features/_scratch/test_out/customXml/
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.579806 python_docx-1.1.1/features/_scratch/test_out/customXml/_rels/
--rw-r--r--   0 scanny     (501) staff       (20)      295 2013-08-15 22:17:06.000000 python_docx-1.1.1/features/_scratch/test_out/customXml/_rels/item1.xml.rels
--rw-r--r--   0 scanny     (501) staff       (20)      218 2013-08-15 22:17:06.000000 python_docx-1.1.1/features/_scratch/test_out/customXml/item1.xml
--rw-r--r--   0 scanny     (501) staff       (20)      341 2013-08-15 22:17:06.000000 python_docx-1.1.1/features/_scratch/test_out/customXml/itemProps1.xml
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.580254 python_docx-1.1.1/features/_scratch/test_out/docProps/
--rw-r--r--   0 scanny     (501) staff       (20)     1035 2013-08-13 09:49:22.000000 python_docx-1.1.1/features/_scratch/test_out/docProps/app.xml
--rw-r--r--   0 scanny     (501) staff       (20)      806 2013-08-15 22:17:06.000000 python_docx-1.1.1/features/_scratch/test_out/docProps/core.xml
--rw-r--r--   0 scanny     (501) staff       (20)     8324 2013-08-15 22:17:06.000000 python_docx-1.1.1/features/_scratch/test_out/docProps/thumbnail.jpeg
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.581427 python_docx-1.1.1/features/_scratch/test_out/word/
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.581576 python_docx-1.1.1/features/_scratch/test_out/word/_rels/
--rw-r--r--   0 scanny     (501) staff       (20)     1227 2013-08-15 22:17:06.000000 python_docx-1.1.1/features/_scratch/test_out/word/_rels/document.xml.rels
--rw-r--r--   0 scanny     (501) staff       (20)     1758 2013-08-15 22:17:06.000000 python_docx-1.1.1/features/_scratch/test_out/word/document.xml
--rw-r--r--   0 scanny     (501) staff       (20)     2552 2013-08-15 22:17:06.000000 python_docx-1.1.1/features/_scratch/test_out/word/fontTable.xml
--rw-r--r--   0 scanny     (501) staff       (20)     5514 2013-08-15 22:17:06.000000 python_docx-1.1.1/features/_scratch/test_out/word/numbering.xml
--rw-r--r--   0 scanny     (501) staff       (20)     2500 2013-08-15 22:17:06.000000 python_docx-1.1.1/features/_scratch/test_out/word/settings.xml
--rw-r--r--   0 scanny     (501) staff       (20)    26716 2013-08-15 22:17:06.000000 python_docx-1.1.1/features/_scratch/test_out/word/styles.xml
--rw-r--r--   0 scanny     (501) staff       (20)    27582 2013-08-15 22:17:06.000000 python_docx-1.1.1/features/_scratch/test_out/word/stylesWithEffects.xml
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.581728 python_docx-1.1.1/features/_scratch/test_out/word/theme/
--rw-r--r--   0 scanny     (501) staff       (20)     7643 2013-08-13 09:49:22.000000 python_docx-1.1.1/features/_scratch/test_out/word/theme/theme1.xml
--rw-r--r--   0 scanny     (501) staff       (20)      431 2013-08-13 09:49:22.000000 python_docx-1.1.1/features/_scratch/test_out/word/webSettings.xml
--rw-r--r--   0 scanny     (501) staff       (20)    36593 2024-04-30 02:52:59.000000 python_docx-1.1.1/features/_scratch/test_out.docx
--rw-r--r--   0 scanny     (501) staff       (20)      476 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/api-open-document.feature
--rw-r--r--   0 scanny     (501) staff       (20)      407 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/blk-add-paragraph.feature
--rw-r--r--   0 scanny     (501) staff       (20)      378 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/blk-add-table.feature
--rw-r--r--   0 scanny     (501) staff       (20)      963 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/blk-iter-inner-content.feature
--rw-r--r--   0 scanny     (501) staff       (20)      981 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/doc-access-collections.feature
--rw-r--r--   0 scanny     (501) staff       (20)      395 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/doc-access-sections.feature
--rw-r--r--   0 scanny     (501) staff       (20)      840 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/doc-add-heading.feature
--rw-r--r--   0 scanny     (501) staff       (20)      358 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/doc-add-page-break.feature
--rw-r--r--   0 scanny     (501) staff       (20)      883 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/doc-add-paragraph.feature
--rw-r--r--   0 scanny     (501) staff       (20)      997 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/doc-add-picture.feature
--rw-r--r--   0 scanny     (501) staff       (20)     1110 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/doc-add-section.feature
--rw-r--r--   0 scanny     (501) staff       (20)      729 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/doc-add-table.feature
--rw-r--r--   0 scanny     (501) staff       (20)      892 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/doc-coreprops.feature
--rw-r--r--   0 scanny     (501) staff       (20)     1398 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/doc-settings.feature
--rw-r--r--   0 scanny     (501) staff       (20)      598 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/doc-styles.feature
--rw-r--r--   0 scanny     (501) staff       (20)      268 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/environment.py
--rw-r--r--   0 scanny     (501) staff       (20)     3116 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/hdr-header-footer.feature
--rw-r--r--   0 scanny     (501) staff       (20)     2116 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/hlk-props.feature
--rw-r--r--   0 scanny     (501) staff       (20)     1499 2015-02-19 07:28:57.000000 python_docx-1.1.1/features/img-characterize-image.feature
--rw-r--r--   0 scanny     (501) staff       (20)      402 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/num-access-numbering-part.feature
--rw-r--r--   0 scanny     (501) staff       (20)     1917 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/par-access-inner-content.feature
--rw-r--r--   0 scanny     (501) staff       (20)      312 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/par-access-parfmt.feature
--rw-r--r--   0 scanny     (501) staff       (20)      527 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/par-add-run.feature
--rw-r--r--   0 scanny     (501) staff       (20)      632 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/par-alignment-prop.feature
--rw-r--r--   0 scanny     (501) staff       (20)      405 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/par-clear-paragraph.feature
--rw-r--r--   0 scanny     (501) staff       (20)      577 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/par-insert-paragraph.feature
--rw-r--r--   0 scanny     (501) staff       (20)      390 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/par-set-text.feature
--rw-r--r--   0 scanny     (501) staff       (20)      871 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/par-style-prop.feature
--rw-r--r--   0 scanny     (501) staff       (20)     1101 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/pbk-split-para.feature
--rw-r--r--   0 scanny     (501) staff       (20)      269 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/run-access-font.feature
--rw-r--r--   0 scanny     (501) staff       (20)      945 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/run-access-inner-content.feature
--rw-r--r--   0 scanny     (501) staff       (20)      458 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/run-add-content.feature
--rw-r--r--   0 scanny     (501) staff       (20)      804 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/run-add-picture.feature
--rw-r--r--   0 scanny     (501) staff       (20)     1173 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/run-char-style.feature
--rw-r--r--   0 scanny     (501) staff       (20)      373 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/run-clear-run.feature
--rw-r--r--   0 scanny     (501) staff       (20)     1757 2015-02-19 07:28:57.000000 python_docx-1.1.1/features/run-enum-props.feature
--rw-r--r--   0 scanny     (501) staff       (20)     5276 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/sct-section.feature
--rw-r--r--   0 scanny     (501) staff       (20)     1070 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/shp-inline-shape-access.feature
--rw-r--r--   0 scanny     (501) staff       (20)      575 2015-02-19 07:28:57.000000 python_docx-1.1.1/features/shp-inline-shape-size.feature
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.584859 python_docx-1.1.1/features/steps/
--rw-r--r--   0 scanny     (501) staff       (20)     1661 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/api.py
--rw-r--r--   0 scanny     (501) staff       (20)     3636 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/block.py
--rw-r--r--   0 scanny     (501) staff       (20)     4150 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/coreprops.py
--rw-r--r--   0 scanny     (501) staff       (20)     8815 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/document.py
--rw-r--r--   0 scanny     (501) staff       (20)     6797 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/font.py
--rw-r--r--   0 scanny     (501) staff       (20)     5055 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/hdrftr.py
--rw-r--r--   0 scanny     (501) staff       (20)      836 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/helpers.py
--rw-r--r--   0 scanny     (501) staff       (20)     4588 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/hyperlink.py
--rw-r--r--   0 scanny     (501) staff       (20)     2212 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/image.py
--rw-r--r--   0 scanny     (501) staff       (20)      952 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/numbering.py
--rw-r--r--   0 scanny     (501) staff       (20)     6052 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/pagebreak.py
--rw-r--r--   0 scanny     (501) staff       (20)     8975 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/paragraph.py
--rw-r--r--   0 scanny     (501) staff       (20)     7912 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/parfmt.py
--rw-r--r--   0 scanny     (501) staff       (20)     9750 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/section.py
--rw-r--r--   0 scanny     (501) staff       (20)     1842 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/settings.py
--rw-r--r--   0 scanny     (501) staff       (20)     5169 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/shape.py
--rw-r--r--   0 scanny     (501) staff       (20)      544 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/shared.py
--rw-r--r--   0 scanny     (501) staff       (20)    17994 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/styles.py
--rw-r--r--   0 scanny     (501) staff       (20)    18911 2024-04-30 02:48:37.000000 python_docx-1.1.1/features/steps/table.py
--rw-r--r--   0 scanny     (501) staff       (20)     4645 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/tabstops.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.597490 python_docx-1.1.1/features/steps/test_files/
--rw-r--r--   0 scanny     (501) staff       (20)    25142 2015-02-19 07:28:57.000000 python_docx-1.1.1/features/steps/test_files/blk-containing-table.docx
--rw-r--r--   0 scanny     (501) staff       (20)    15649 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/blk-paras-and-tables.docx
--rw-r--r--   0 scanny     (501) staff       (20)    80603 2023-09-10 05:09:30.000000 python_docx-1.1.1/features/steps/test_files/court-exif.jpg
--rw-r--r--   0 scanny     (501) staff       (20)    25591 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/doc-access-sections.docx
--rw-r--r--   0 scanny     (501) staff       (20)    17956 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/doc-add-section.docx
--rw-r--r--   0 scanny     (501) staff       (20)    11992 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/doc-coreprops.docx
--rw-r--r--   0 scanny     (501) staff       (20)    21366 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/doc-default.docx
--rw-r--r--   0 scanny     (501) staff       (20)    11394 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/doc-no-coreprops.docx
--rw-r--r--   0 scanny     (501) staff       (20)    17711 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/doc-odd-even-hdrs.docx
--rw-r--r--   0 scanny     (501) staff       (20)    21309 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/doc-word-default-blank.docx
--rw-r--r--   0 scanny     (501) staff       (20)    15846 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/fnt-color.docx
--rw-r--r--   0 scanny     (501) staff       (20)    18079 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/hdr-header-footer.docx
--rw-r--r--   0 scanny     (501) staff       (20)   355196 2015-02-19 07:28:57.000000 python_docx-1.1.1/features/steps/test_files/jfif-300-dpi.jpg
--rw-r--r--   0 scanny     (501) staff       (20)   768608 2023-09-10 05:09:16.000000 python_docx-1.1.1/features/steps/test_files/jpeg420exif.jpg
--rw-r--r--   0 scanny     (501) staff       (20)   263222 2015-02-19 07:28:57.000000 python_docx-1.1.1/features/steps/test_files/lena.bmp
--rw-r--r--   0 scanny     (501) staff       (20)    72985 2015-02-19 07:28:57.000000 python_docx-1.1.1/features/steps/test_files/lena.gif
--rw-r--r--   0 scanny     (501) staff       (20)   786572 2023-09-10 05:09:00.000000 python_docx-1.1.1/features/steps/test_files/lena.tif
--rw-r--r--   0 scanny     (501) staff       (20)   104428 2023-09-10 05:08:43.000000 python_docx-1.1.1/features/steps/test_files/lena_std.jpg
--rw-r--r--   0 scanny     (501) staff       (20)    64276 2015-02-19 07:28:57.000000 python_docx-1.1.1/features/steps/test_files/monty-truth.png
--rw-r--r--   0 scanny     (501) staff       (20)   308280 2015-02-19 07:28:57.000000 python_docx-1.1.1/features/steps/test_files/mountain.bmp
--rw-r--r--   0 scanny     (501) staff       (20)    24334 2015-02-19 07:28:57.000000 python_docx-1.1.1/features/steps/test_files/num-having-numbering-part.docx
--rw-r--r--   0 scanny     (501) staff       (20)    15126 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/par-alignment.docx
--rw-r--r--   0 scanny     (501) staff       (20)    12071 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/par-hlink-frags.docx
--rw-r--r--   0 scanny     (501) staff       (20)    12385 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/par-hyperlinks.docx
--rw-r--r--   0 scanny     (501) staff       (20)    27969 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/par-known-paragraphs.docx
--rw-r--r--   0 scanny     (501) staff       (20)    20901 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/par-known-styles.docx
--rw-r--r--   0 scanny     (501) staff       (20)    12244 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/par-rendered-page-breaks.docx
--rw-r--r--   0 scanny     (501) staff       (20)     3277 2015-02-19 07:28:57.000000 python_docx-1.1.1/features/steps/test_files/python-icon.jpeg
--rw-r--r--   0 scanny     (501) staff       (20)    26645 2015-02-19 07:28:57.000000 python_docx-1.1.1/features/steps/test_files/run-char-style.docx
--rw-r--r--   0 scanny     (501) staff       (20)    14645 2015-02-19 07:28:57.000000 python_docx-1.1.1/features/steps/test_files/run-enumerated-props.docx
--rw-r--r--   0 scanny     (501) staff       (20)    10409 2015-02-19 07:28:57.000000 python_docx-1.1.1/features/steps/test_files/sample.tif
--rw-r--r--   0 scanny     (501) staff       (20)    14849 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/sct-first-page-hdrftr.docx
--rw-r--r--   0 scanny     (501) staff       (20)    12051 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/sct-inner-content.docx
--rw-r--r--   0 scanny     (501) staff       (20)    28168 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/sct-section-props.docx
--rw-r--r--   0 scanny     (501) staff       (20)    10760 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/set-no-settings-part.docx
--rw-r--r--   0 scanny     (501) staff       (20)   122610 2015-02-19 07:28:57.000000 python_docx-1.1.1/features/steps/test_files/shp-inline-shape-access.docx
--rw-r--r--   0 scanny     (501) staff       (20)    12195 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/sty-behav-props.docx
--rw-r--r--   0 scanny     (501) staff       (20)     8358 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/sty-having-no-styles-part.docx
--rw-r--r--   0 scanny     (501) staff       (20)    21573 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/sty-having-styles-part.docx
--rw-r--r--   0 scanny     (501) staff       (20)    13560 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/sty-known-styles.docx
--rw-r--r--   0 scanny     (501) staff       (20)    13170 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/tab-stops.docx
--rw-r--r--   0 scanny     (501) staff       (20)    25129 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/tbl-2x2-table.docx
--rw-r--r--   0 scanny     (501) staff       (20)    36051 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/tbl-cell-access.docx
--rw-r--r--   0 scanny     (501) staff       (20)    13773 2024-04-30 02:48:37.000000 python_docx-1.1.1/features/steps/test_files/tbl-cell-props.docx
--rw-r--r--   0 scanny     (501) staff       (20)    13654 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/tbl-col-props.docx
--rw-r--r--   0 scanny     (501) staff       (20)    50294 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/tbl-having-applied-style.docx
--rw-r--r--   0 scanny     (501) staff       (20)    32010 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/tbl-having-tables.docx
--rw-r--r--   0 scanny     (501) staff       (20)    16017 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/tbl-on-off-props.docx
--rw-r--r--   0 scanny     (501) staff       (20)    20419 2024-04-30 00:55:22.000000 python_docx-1.1.1/features/steps/test_files/tbl-props.docx
--rw-r--r--   0 scanny     (501) staff       (20)   146892 2015-02-19 07:28:57.000000 python_docx-1.1.1/features/steps/test_files/test.png
--rw-r--r--   0 scanny     (501) staff       (20)    12859 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/txt-font-highlight-color.docx
--rw-r--r--   0 scanny     (501) staff       (20)    37924 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/test_files/txt-font-props.docx
--rw-r--r--   0 scanny     (501) staff       (20)    10059 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/steps/text.py
--rw-r--r--   0 scanny     (501) staff       (20)      463 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/sty-access-font.feature
--rw-r--r--   0 scanny     (501) staff       (20)      568 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/sty-access-latent-styles.feature
--rw-r--r--   0 scanny     (501) staff       (20)      488 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/sty-access-parfmt.feature
--rw-r--r--   0 scanny     (501) staff       (20)      767 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/sty-add-style.feature
--rw-r--r--   0 scanny     (501) staff       (20)      352 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/sty-delete-style.feature
--rw-r--r--   0 scanny     (501) staff       (20)      654 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/sty-latent-add-del.feature
--rw-r--r--   0 scanny     (501) staff       (20)     4102 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/sty-latent-props.feature
--rw-r--r--   0 scanny     (501) staff       (20)     5464 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/sty-style-props.feature
--rw-r--r--   0 scanny     (501) staff       (20)     1264 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/tab-access-tabs.feature
--rw-r--r--   0 scanny     (501) staff       (20)     1877 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/tab-tabstop-props.feature
--rw-r--r--   0 scanny     (501) staff       (20)      594 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/tbl-add-row-or-col.feature
--rw-r--r--   0 scanny     (501) staff       (20)     1523 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/tbl-cell-access.feature
--rw-r--r--   0 scanny     (501) staff       (20)      428 2024-04-30 00:55:22.000000 python_docx-1.1.1/features/tbl-cell-add-table.feature
--rw-r--r--   0 scanny     (501) staff       (20)     2105 2024-04-30 02:48:37.000000 python_docx-1.1.1/features/tbl-cell-props.feature
--rw-r--r--   0 scanny     (501) staff       (20)      343 2024-04-30 00:55:22.000000 python_docx-1.1.1/features/tbl-cell-text.feature
--rw-r--r--   0 scanny     (501) staff       (20)     1062 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/tbl-col-props.feature
--rw-r--r--   0 scanny     (501) staff       (20)      944 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/tbl-item-access.feature
--rw-r--r--   0 scanny     (501) staff       (20)     2294 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/tbl-merge-cells.feature
--rw-r--r--   0 scanny     (501) staff       (20)     2907 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/tbl-props.feature
--rw-r--r--   0 scanny     (501) staff       (20)     2188 2024-04-30 00:55:22.000000 python_docx-1.1.1/features/tbl-row-props.feature
--rw-r--r--   0 scanny     (501) staff       (20)     1169 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/tbl-style.feature
--rw-r--r--   0 scanny     (501) staff       (20)      645 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/txt-add-break.feature
--rw-r--r--   0 scanny     (501) staff       (20)     2279 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/txt-font-color.feature
--rw-r--r--   0 scanny     (501) staff       (20)     8120 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/txt-font-props.feature
--rw-r--r--   0 scanny     (501) staff       (20)     7648 2023-11-04 03:19:46.000000 python_docx-1.1.1/features/txt-parfmt-props.feature
--rw-r--r--   0 scanny     (501) staff       (20)     3309 2024-04-30 02:48:37.000000 python_docx-1.1.1/pyproject.toml
--rw-r--r--   0 scanny     (501) staff       (20)       76 2024-04-30 00:55:22.000000 python_docx-1.1.1/requirements-dev.txt
--rw-r--r--   0 scanny     (501) staff       (20)       68 2024-04-30 02:48:37.000000 python_docx-1.1.1/requirements-docs.txt
--rw-r--r--   0 scanny     (501) staff       (20)       81 2024-04-30 00:55:22.000000 python_docx-1.1.1/requirements-test.txt
--rw-r--r--   0 scanny     (501) staff       (20)       30 2023-11-04 03:19:46.000000 python_docx-1.1.1/requirements.txt
--rw-r--r--   0 scanny     (501) staff       (20)       38 2024-04-30 02:58:01.649285 python_docx-1.1.1/setup.cfg
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.551441 python_docx-1.1.1/src/
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.601019 python_docx-1.1.1/src/docx/
--rw-r--r--   0 scanny     (501) staff       (20)     1711 2024-04-30 02:51:57.000000 python_docx-1.1.1/src/docx/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)     1350 2024-04-30 02:48:37.000000 python_docx-1.1.1/src/docx/api.py
--rw-r--r--   0 scanny     (501) staff       (20)     3469 2024-04-30 02:48:37.000000 python_docx-1.1.1/src/docx/blkcntnr.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.601407 python_docx-1.1.1/src/docx/dml/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/dml/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)     3794 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/dml/color.py
--rw-r--r--   0 scanny     (501) staff       (20)     8021 2024-04-30 02:48:37.000000 python_docx-1.1.1/src/docx/document.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.601686 python_docx-1.1.1/src/docx/drawing/
--rw-r--r--   0 scanny     (501) staff       (20)      504 2024-04-30 02:48:37.000000 python_docx-1.1.1/src/docx/drawing/__init__.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.603264 python_docx-1.1.1/src/docx/enum/
--rw-r--r--   0 scanny     (501) staff       (20)      240 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/enum/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)     4888 2024-04-30 02:48:37.000000 python_docx-1.1.1/src/docx/enum/base.py
--rw-r--r--   0 scanny     (501) staff       (20)     3346 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/enum/dml.py
--rw-r--r--   0 scanny     (501) staff       (20)     2391 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/enum/section.py
--rw-r--r--   0 scanny     (501) staff       (20)      396 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/enum/shape.py
--rw-r--r--   0 scanny     (501) staff       (20)    10137 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/enum/style.py
--rw-r--r--   0 scanny     (501) staff       (20)     3943 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/enum/table.py
--rw-r--r--   0 scanny     (501) staff       (20)    10276 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/enum/text.py
--rw-r--r--   0 scanny     (501) staff       (20)      454 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/exceptions.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.605582 python_docx-1.1.1/src/docx/image/
--rw-r--r--   0 scanny     (501) staff       (20)      664 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/image/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)     1347 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/image/bmp.py
--rw-r--r--   0 scanny     (501) staff       (20)     3466 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/image/constants.py
--rw-r--r--   0 scanny     (501) staff       (20)      383 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/image/exceptions.py
--rw-r--r--   0 scanny     (501) staff       (20)     1118 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/image/gif.py
--rw-r--r--   0 scanny     (501) staff       (20)     3089 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/image/helpers.py
--rw-r--r--   0 scanny     (501) staff       (20)     7993 2024-04-30 02:48:37.000000 python_docx-1.1.1/src/docx/image/image.py
--rw-r--r--   0 scanny     (501) staff       (20)    15422 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/image/jpeg.py
--rw-r--r--   0 scanny     (501) staff       (20)     8214 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/image/png.py
--rw-r--r--   0 scanny     (501) staff       (20)    10379 2024-04-30 00:55:22.000000 python_docx-1.1.1/src/docx/image/tiff.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.608833 python_docx-1.1.1/src/docx/opc/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/opc/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)    19080 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/opc/constants.py
--rw-r--r--   0 scanny     (501) staff       (20)     3134 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/opc/coreprops.py
--rw-r--r--   0 scanny     (501) staff       (20)      264 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/opc/exceptions.py
--rw-r--r--   0 scanny     (501) staff       (20)     8126 2024-04-30 00:55:22.000000 python_docx-1.1.1/src/docx/opc/oxml.py
--rw-r--r--   0 scanny     (501) staff       (20)     8425 2024-04-30 00:55:22.000000 python_docx-1.1.1/src/docx/opc/package.py
--rw-r--r--   0 scanny     (501) staff       (20)     3708 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/opc/packuri.py
--rw-r--r--   0 scanny     (501) staff       (20)     8388 2024-04-30 00:55:22.000000 python_docx-1.1.1/src/docx/opc/part.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.609175 python_docx-1.1.1/src/docx/opc/parts/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/opc/parts/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)     1514 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/opc/parts/coreprops.py
--rw-r--r--   0 scanny     (501) staff       (20)     4005 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/opc/phys_pkg.py
--rw-r--r--   0 scanny     (501) staff       (20)     9640 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/opc/pkgreader.py
--rw-r--r--   0 scanny     (501) staff       (20)     4524 2024-04-30 00:55:22.000000 python_docx-1.1.1/src/docx/opc/pkgwriter.py
--rw-r--r--   0 scanny     (501) staff       (20)     5389 2024-04-30 00:55:22.000000 python_docx-1.1.1/src/docx/opc/rel.py
--rw-r--r--   0 scanny     (501) staff       (20)      996 2024-04-30 00:55:22.000000 python_docx-1.1.1/src/docx/opc/shared.py
--rw-r--r--   0 scanny     (501) staff       (20)      638 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/opc/spec.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.612331 python_docx-1.1.1/src/docx/oxml/
--rw-r--r--   0 scanny     (501) staff       (20)     8100 2024-04-30 00:55:22.000000 python_docx-1.1.1/src/docx/oxml/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)     9938 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/oxml/coreprops.py
--rw-r--r--   0 scanny     (501) staff       (20)     3543 2024-04-30 00:55:22.000000 python_docx-1.1.1/src/docx/oxml/document.py
--rw-r--r--   0 scanny     (501) staff       (20)      397 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/oxml/drawing.py
--rw-r--r--   0 scanny     (501) staff       (20)      261 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/oxml/exceptions.py
--rw-r--r--   0 scanny     (501) staff       (20)     3796 2024-04-30 02:48:37.000000 python_docx-1.1.1/src/docx/oxml/ns.py
--rw-r--r--   0 scanny     (501) staff       (20)     3965 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/oxml/numbering.py
--rw-r--r--   0 scanny     (501) staff       (20)     2316 2024-04-30 00:55:22.000000 python_docx-1.1.1/src/docx/oxml/parser.py
--rw-r--r--   0 scanny     (501) staff       (20)    20395 2024-04-30 00:55:22.000000 python_docx-1.1.1/src/docx/oxml/section.py
--rw-r--r--   0 scanny     (501) staff       (20)     3911 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/oxml/settings.py
--rw-r--r--   0 scanny     (501) staff       (20)     8080 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/oxml/shape.py
--rw-r--r--   0 scanny     (501) staff       (20)     1871 2024-04-30 00:55:22.000000 python_docx-1.1.1/src/docx/oxml/shared.py
--rw-r--r--   0 scanny     (501) staff       (20)    10834 2024-04-30 02:48:37.000000 python_docx-1.1.1/src/docx/oxml/simpletypes.py
--rw-r--r--   0 scanny     (501) staff       (20)    10673 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/oxml/styles.py
--rw-r--r--   0 scanny     (501) staff       (20)    33671 2024-04-30 02:48:37.000000 python_docx-1.1.1/src/docx/oxml/table.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.613681 python_docx-1.1.1/src/docx/oxml/text/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/oxml/text/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)    11652 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/oxml/text/font.py
--rw-r--r--   0 scanny     (501) staff       (20)     1467 2024-04-30 00:55:22.000000 python_docx-1.1.1/src/docx/oxml/text/hyperlink.py
--rw-r--r--   0 scanny     (501) staff       (20)    11262 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/oxml/text/pagebreak.py
--rw-r--r--   0 scanny     (501) staff       (20)     3538 2024-04-30 00:55:22.000000 python_docx-1.1.1/src/docx/oxml/text/paragraph.py
--rw-r--r--   0 scanny     (501) staff       (20)    11986 2024-04-30 02:48:37.000000 python_docx-1.1.1/src/docx/oxml/text/parfmt.py
--rw-r--r--   0 scanny     (501) staff       (20)     9629 2024-04-30 00:55:22.000000 python_docx-1.1.1/src/docx/oxml/text/run.py
--rw-r--r--   0 scanny     (501) staff       (20)    25567 2024-04-30 00:55:22.000000 python_docx-1.1.1/src/docx/oxml/xmlchemy.py
--rw-r--r--   0 scanny     (501) staff       (20)     3855 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/package.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.615292 python_docx-1.1.1/src/docx/parts/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/parts/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)     5472 2024-04-30 02:48:37.000000 python_docx-1.1.1/src/docx/parts/document.py
--rw-r--r--   0 scanny     (501) staff       (20)     1610 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/parts/hdrftr.py
--rw-r--r--   0 scanny     (501) staff       (20)     2538 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/parts/image.py
--rw-r--r--   0 scanny     (501) staff       (20)     1056 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/parts/numbering.py
--rw-r--r--   0 scanny     (501) staff       (20)     1300 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/parts/settings.py
--rw-r--r--   0 scanny     (501) staff       (20)     3817 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/parts/story.py
--rw-r--r--   0 scanny     (501) staff       (20)     1413 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/parts/styles.py
--rw-r--r--   0 scanny     (501) staff       (20)        0 2024-04-30 02:48:37.000000 python_docx-1.1.1/src/docx/py.typed
--rw-r--r--   0 scanny     (501) staff       (20)    18534 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/section.py
--rw-r--r--   0 scanny     (501) staff       (20)      658 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/settings.py
--rw-r--r--   0 scanny     (501) staff       (20)     2658 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/shape.py
--rw-r--r--   0 scanny     (501) staff       (20)    13509 2024-04-30 02:48:37.000000 python_docx-1.1.1/src/docx/shared.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.616099 python_docx-1.1.1/src/docx/styles/
--rw-r--r--   0 scanny     (501) staff       (20)     1406 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/styles/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)     7211 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/styles/latent.py
--rw-r--r--   0 scanny     (501) staff       (20)     8051 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/styles/style.py
--rw-r--r--   0 scanny     (501) staff       (20)     5717 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/styles/styles.py
--rw-r--r--   0 scanny     (501) staff       (20)    19477 2024-04-30 02:52:59.000000 python_docx-1.1.1/src/docx/table.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.617255 python_docx-1.1.1/src/docx/templates/
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.617481 python_docx-1.1.1/src/docx/templates/default-docx-template/
--rw-r--r--   0 scanny     (501) staff       (20)     1782 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-docx-template/[Content_Types].xml
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.617702 python_docx-1.1.1/src/docx/templates/default-docx-template/_rels/
--rw-r--r--   0 scanny     (501) staff       (20)      748 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-docx-template/_rels/.rels
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.618085 python_docx-1.1.1/src/docx/templates/default-docx-template/customXml/
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.618262 python_docx-1.1.1/src/docx/templates/default-docx-template/customXml/_rels/
--rw-r--r--   0 scanny     (501) staff       (20)      300 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-docx-template/customXml/_rels/item1.xml.rels
--rw-r--r--   0 scanny     (501) staff       (20)      262 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-docx-template/customXml/item1.xml
--rw-r--r--   0 scanny     (501) staff       (20)      354 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-docx-template/customXml/itemProps1.xml
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.618830 python_docx-1.1.1/src/docx/templates/default-docx-template/docProps/
--rw-r--r--   0 scanny     (501) staff       (20)     1132 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-docx-template/docProps/app.xml
--rw-r--r--   0 scanny     (501) staff       (20)      753 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-docx-template/docProps/core.xml
--rw-r--r--   0 scanny     (501) staff       (20)     8324 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-docx-template/docProps/thumbnail.jpeg
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.620793 python_docx-1.1.1/src/docx/templates/default-docx-template/word/
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.621012 python_docx-1.1.1/src/docx/templates/default-docx-template/word/_rels/
--rw-r--r--   0 scanny     (501) staff       (20)     1253 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-docx-template/word/_rels/document.xml.rels
--rw-r--r--   0 scanny     (501) staff       (20)     1594 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-docx-template/word/document.xml
--rw-r--r--   0 scanny     (501) staff       (20)     2811 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-docx-template/word/fontTable.xml
--rw-r--r--   0 scanny     (501) staff       (20)     6747 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-docx-template/word/numbering.xml
--rw-r--r--   0 scanny     (501) staff       (20)     2749 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-docx-template/word/settings.xml
--rw-r--r--   0 scanny     (501) staff       (20)   438677 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-docx-template/word/styles.xml
--rw-r--r--   0 scanny     (501) staff       (20)   438131 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-docx-template/word/stylesWithEffects.xml
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.621221 python_docx-1.1.1/src/docx/templates/default-docx-template/word/theme/
--rw-r--r--   0 scanny     (501) staff       (20)    10939 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-docx-template/word/theme/theme1.xml
--rw-r--r--   0 scanny     (501) staff       (20)      438 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-docx-template/word/webSettings.xml
--rw-r--r--   0 scanny     (501) staff       (20)     1395 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-footer.xml
--rw-r--r--   0 scanny     (501) staff       (20)     1395 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-header.xml
--rw-r--r--   0 scanny     (501) staff       (20)     1640 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-settings.xml
--rw-r--r--   0 scanny     (501) staff       (20)    15823 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default-styles.xml
--rw-r--r--   0 scanny     (501) staff       (20)    38116 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/templates/default.docx
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.622846 python_docx-1.1.1/src/docx/text/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/text/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)    13653 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/text/font.py
--rw-r--r--   0 scanny     (501) staff       (20)     5257 2024-04-30 02:52:59.000000 python_docx-1.1.1/src/docx/text/hyperlink.py
--rw-r--r--   0 scanny     (501) staff       (20)     4950 2024-04-30 02:48:37.000000 python_docx-1.1.1/src/docx/text/pagebreak.py
--rw-r--r--   0 scanny     (501) staff       (20)     6828 2024-04-30 02:48:37.000000 python_docx-1.1.1/src/docx/text/paragraph.py
--rw-r--r--   0 scanny     (501) staff       (20)    10339 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/text/parfmt.py
--rw-r--r--   0 scanny     (501) staff       (20)     9645 2024-04-30 02:48:37.000000 python_docx-1.1.1/src/docx/text/run.py
--rw-r--r--   0 scanny     (501) staff       (20)     3910 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/text/tabstops.py
--rw-r--r--   0 scanny     (501) staff       (20)      864 2023-11-04 03:19:46.000000 python_docx-1.1.1/src/docx/types.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.648320 python_docx-1.1.1/src/python_docx.egg-info/
--rw-r--r--   0 scanny     (501) staff       (20)     2008 2024-04-30 02:58:01.000000 python_docx-1.1.1/src/python_docx.egg-info/PKG-INFO
--rw-r--r--   0 scanny     (501) staff       (20)    16643 2024-04-30 02:58:01.000000 python_docx-1.1.1/src/python_docx.egg-info/SOURCES.txt
--rw-r--r--   0 scanny     (501) staff       (20)        1 2024-04-30 02:58:01.000000 python_docx-1.1.1/src/python_docx.egg-info/dependency_links.txt
--rw-r--r--   0 scanny     (501) staff       (20)       45 2024-04-30 02:58:01.000000 python_docx-1.1.1/src/python_docx.egg-info/requires.txt
--rw-r--r--   0 scanny     (501) staff       (20)        5 2024-04-30 02:58:01.000000 python_docx-1.1.1/src/python_docx.egg-info/top_level.txt
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.626375 python_docx-1.1.1/tests/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2013-07-29 10:11:43.000000 python_docx-1.1.1/tests/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)      452 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/conftest.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.626662 python_docx-1.1.1/tests/dml/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/dml/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)     5437 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/dml/test_color.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.628545 python_docx-1.1.1/tests/image/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/image/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)     1108 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/image/test_bmp.py
--rw-r--r--   0 scanny     (501) staff       (20)      960 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/image/test_gif.py
--rw-r--r--   0 scanny     (501) staff       (20)     1569 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/image/test_helpers.py
--rw-r--r--   0 scanny     (501) staff       (20)    11958 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/image/test_image.py
--rw-r--r--   0 scanny     (501) staff       (20)    21556 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/image/test_jpeg.py
--rw-r--r--   0 scanny     (501) staff       (20)    14741 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/image/test_png.py
--rw-r--r--   0 scanny     (501) staff       (20)    14704 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/image/test_tiff.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.630399 python_docx-1.1.1/tests/opc/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/opc/__init__.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.630696 python_docx-1.1.1/tests/opc/parts/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/opc/parts/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)     1870 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/opc/parts/test_coreprops.py
--rw-r--r--   0 scanny     (501) staff       (20)     7972 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/opc/test_coreprops.py
--rw-r--r--   0 scanny     (501) staff       (20)     4866 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/opc/test_oxml.py
--rw-r--r--   0 scanny     (501) staff       (20)    17017 2024-04-30 00:55:22.000000 python_docx-1.1.1/tests/opc/test_package.py
--rw-r--r--   0 scanny     (501) staff       (20)     3313 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/opc/test_packuri.py
--rw-r--r--   0 scanny     (501) staff       (20)    15381 2024-04-30 00:55:22.000000 python_docx-1.1.1/tests/opc/test_part.py
--rw-r--r--   0 scanny     (501) staff       (20)     6289 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/opc/test_phys_pkg.py
--rw-r--r--   0 scanny     (501) staff       (20)    19028 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/opc/test_pkgreader.py
--rw-r--r--   0 scanny     (501) staff       (20)     7218 2024-04-30 00:55:22.000000 python_docx-1.1.1/tests/opc/test_pkgwriter.py
--rw-r--r--   0 scanny     (501) staff       (20)     9565 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/opc/test_rel.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.631164 python_docx-1.1.1/tests/opc/unitdata/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/opc/unitdata/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)     8626 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/opc/unitdata/rels.py
--rw-r--r--   0 scanny     (501) staff       (20)      765 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/opc/unitdata/types.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.632995 python_docx-1.1.1/tests/oxml/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/oxml/__init__.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.633282 python_docx-1.1.1/tests/oxml/parts/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/oxml/parts/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)     1432 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/oxml/parts/test_document.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.633562 python_docx-1.1.1/tests/oxml/parts/unitdata/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/oxml/parts/unitdata/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)      388 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/oxml/parts/unitdata/document.py
--rw-r--r--   0 scanny     (501) staff       (20)     4108 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/oxml/test__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)      587 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/oxml/test_document.py
--rw-r--r--   0 scanny     (501) staff       (20)     1634 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/oxml/test_ns.py
--rw-r--r--   0 scanny     (501) staff       (20)      592 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/oxml/test_section.py
--rw-r--r--   0 scanny     (501) staff       (20)     1367 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/oxml/test_styles.py
--rw-r--r--   0 scanny     (501) staff       (20)    13656 2024-04-30 02:48:37.000000 python_docx-1.1.1/tests/oxml/test_table.py
--rw-r--r--   0 scanny     (501) staff       (20)    28193 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/oxml/test_xmlchemy.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.634032 python_docx-1.1.1/tests/oxml/text/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/oxml/text/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)     1481 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/oxml/text/test_hyperlink.py
--rw-r--r--   0 scanny     (501) staff       (20)     1156 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/oxml/text/test_run.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.635099 python_docx-1.1.1/tests/oxml/unitdata/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/oxml/unitdata/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)     1172 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/oxml/unitdata/dml.py
--rw-r--r--   0 scanny     (501) staff       (20)      412 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/oxml/unitdata/numbering.py
--rw-r--r--   0 scanny     (501) staff       (20)      893 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/oxml/unitdata/section.py
--rw-r--r--   0 scanny     (501) staff       (20)      677 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/oxml/unitdata/shared.py
--rw-r--r--   0 scanny     (501) staff       (20)      449 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/oxml/unitdata/styles.py
--rw-r--r--   0 scanny     (501) staff       (20)     3153 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/oxml/unitdata/text.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.637199 python_docx-1.1.1/tests/parts/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/parts/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)    12295 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/parts/test_document.py
--rw-r--r--   0 scanny     (501) staff       (20)     5062 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/parts/test_hdrftr.py
--rw-r--r--   0 scanny     (501) staff       (20)     3945 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/parts/test_image.py
--rw-r--r--   0 scanny     (501) staff       (20)     2580 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/parts/test_numbering.py
--rw-r--r--   0 scanny     (501) staff       (20)     2576 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/parts/test_settings.py
--rw-r--r--   0 scanny     (501) staff       (20)     5270 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/parts/test_story.py
--rw-r--r--   0 scanny     (501) staff       (20)     1695 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/parts/test_styles.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.637946 python_docx-1.1.1/tests/styles/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/styles/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)    14144 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/styles/test_latent.py
--rw-r--r--   0 scanny     (501) staff       (20)    20304 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/styles/test_style.py
--rw-r--r--   0 scanny     (501) staff       (20)    14836 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/styles/test_styles.py
--rw-r--r--   0 scanny     (501) staff       (20)     2327 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/test_api.py
--rw-r--r--   0 scanny     (501) staff       (20)     5451 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/test_blkcntnr.py
--rw-r--r--   0 scanny     (501) staff       (20)    14036 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/test_document.py
--rw-r--r--   0 scanny     (501) staff       (20)     3188 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/test_enum.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.642486 python_docx-1.1.1/tests/test_files/
--rw-r--r--   0 scanny     (501) staff       (20)   146892 2014-06-27 08:20:06.000000 python_docx-1.1.1/tests/test_files/150-dpi.png
--rw-r--r--   0 scanny     (501) staff       (20)   125824 2023-09-10 05:05:56.000000 python_docx-1.1.1/tests/test_files/300-dpi.TIF
--rw-r--r--   0 scanny     (501) staff       (20)   355196 2014-06-27 08:20:06.000000 python_docx-1.1.1/tests/test_files/300-dpi.jpg
--rw-r--r--   0 scanny     (501) staff       (20)    39921 2014-06-27 08:20:06.000000 python_docx-1.1.1/tests/test_files/300-dpi.png
--rw-r--r--   0 scanny     (501) staff       (20)     9454 2014-06-27 08:20:06.000000 python_docx-1.1.1/tests/test_files/72-dpi.tiff
--rw-r--r--   0 scanny     (501) staff       (20)     1526 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/CVS_LOGO.WMF
--rw-r--r--   0 scanny     (501) staff       (20)    11949 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/test_files/blk-inner-content.docx
--rw-r--r--   0 scanny     (501) staff       (20)   768608 2023-09-10 05:05:40.000000 python_docx-1.1.1/tests/test_files/exif-420-dpi.jpg
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.642681 python_docx-1.1.1/tests/test_files/expanded_docx/
--rw-r--r--   0 scanny     (501) staff       (20)     1738 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/expanded_docx/[Content_Types].xml
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.642863 python_docx-1.1.1/tests/test_files/expanded_docx/_rels/
--rw-r--r--   0 scanny     (501) staff       (20)      734 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/expanded_docx/_rels/.rels
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.643195 python_docx-1.1.1/tests/test_files/expanded_docx/customXml/
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.643374 python_docx-1.1.1/tests/test_files/expanded_docx/customXml/_rels/
--rw-r--r--   0 scanny     (501) staff       (20)      295 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/expanded_docx/customXml/_rels/item1.xml.rels
--rw-r--r--   0 scanny     (501) staff       (20)      217 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/expanded_docx/customXml/item1.xml
--rw-r--r--   0 scanny     (501) staff       (20)      340 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/expanded_docx/customXml/itemProps1.xml
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.643870 python_docx-1.1.1/tests/test_files/expanded_docx/docProps/
--rw-r--r--   0 scanny     (501) staff       (20)     1036 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/expanded_docx/docProps/app.xml
--rw-r--r--   0 scanny     (501) staff       (20)      802 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/expanded_docx/docProps/core.xml
--rw-r--r--   0 scanny     (501) staff       (20)    13032 2014-06-27 08:20:06.000000 python_docx-1.1.1/tests/test_files/expanded_docx/docProps/thumbnail.jpeg
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.645150 python_docx-1.1.1/tests/test_files/expanded_docx/word/
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.645323 python_docx-1.1.1/tests/test_files/expanded_docx/word/_rels/
--rw-r--r--   0 scanny     (501) staff       (20)     1227 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/expanded_docx/word/_rels/document.xml.rels
--rw-r--r--   0 scanny     (501) staff       (20)     1819 2023-09-10 05:07:15.000000 python_docx-1.1.1/tests/test_files/expanded_docx/word/document.xml
--rw-r--r--   0 scanny     (501) staff       (20)     2566 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/expanded_docx/word/fontTable.xml
--rw-r--r--   0 scanny     (501) staff       (20)     5513 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/expanded_docx/word/numbering.xml
--rw-r--r--   0 scanny     (501) staff       (20)     2520 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/expanded_docx/word/settings.xml
--rw-r--r--   0 scanny     (501) staff       (20)    26715 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/expanded_docx/word/styles.xml
--rw-r--r--   0 scanny     (501) staff       (20)    27581 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/expanded_docx/word/stylesWithEffects.xml
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.645486 python_docx-1.1.1/tests/test_files/expanded_docx/word/theme/
--rw-r--r--   0 scanny     (501) staff       (20)     7642 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/expanded_docx/word/theme/theme1.xml
--rw-r--r--   0 scanny     (501) staff       (20)      430 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/expanded_docx/word/webSettings.xml
--rw-r--r--   0 scanny     (501) staff       (20)   132875 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/having-images.docx
--rw-r--r--   0 scanny     (501) staff       (20)     7958 2014-06-27 08:20:06.000000 python_docx-1.1.1/tests/test_files/jfif-iguana.jpg
--rw-r--r--   0 scanny     (501) staff       (20)    10409 2014-06-27 08:20:06.000000 python_docx-1.1.1/tests/test_files/little-endian.tif
--rw-r--r--   0 scanny     (501) staff       (20)    64276 2014-06-27 08:20:06.000000 python_docx-1.1.1/tests/test_files/monty-truth.png
--rw-r--r--   0 scanny     (501) staff       (20)     3277 2014-06-27 08:20:06.000000 python_docx-1.1.1/tests/test_files/python-icon.jpeg
--rw-r--r--   0 scanny     (501) staff       (20)     2036 2014-06-27 08:20:06.000000 python_docx-1.1.1/tests/test_files/python-icon.png
--rw-r--r--   0 scanny     (501) staff       (20)     6111 2014-06-27 08:20:06.000000 python_docx-1.1.1/tests/test_files/python-powered.png
--rw-r--r--   0 scanny     (501) staff       (20)    45210 2014-06-27 08:20:06.000000 python_docx-1.1.1/tests/test_files/python.bmp
--rw-r--r--   0 scanny     (501) staff       (20)    12051 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/test_files/sct-inner-content.docx
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.646203 python_docx-1.1.1/tests/test_files/snippets/
--rw-r--r--   0 scanny     (501) staff       (20)     2949 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/test_files/snippets/add-row-col.txt
--rw-r--r--   0 scanny     (501) staff       (20)     1110 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/test_files/snippets/inline.txt
--rw-r--r--   0 scanny     (501) staff       (20)     1756 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/test_files/snippets/new-tbl.txt
--rw-r--r--   0 scanny     (501) staff       (20)     4595 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/test_files/snippets/tbl-cells.txt
--rw-r--r--   0 scanny     (501) staff       (20)    33273 2014-06-27 08:20:06.000000 python_docx-1.1.1/tests/test_files/sonic.gif
--rw-r--r--   0 scanny     (501) staff       (20)    31773 2014-03-01 10:03:55.000000 python_docx-1.1.1/tests/test_files/test.docx
--rw-r--r--   0 scanny     (501) staff       (20)     5297 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/test_package.py
--rw-r--r--   0 scanny     (501) staff       (20)    31223 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/test_section.py
--rw-r--r--   0 scanny     (501) staff       (20)     2169 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/test_settings.py
--rw-r--r--   0 scanny     (501) staff       (20)     6785 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/test_shape.py
--rw-r--r--   0 scanny     (501) staff       (20)     4385 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/test_shared.py
--rw-r--r--   0 scanny     (501) staff       (20)    32484 2024-04-30 02:48:37.000000 python_docx-1.1.1/tests/test_table.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.647414 python_docx-1.1.1/tests/text/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/text/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)    15804 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/text/test_font.py
--rw-r--r--   0 scanny     (501) staff       (20)     5192 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/text/test_hyperlink.py
--rw-r--r--   0 scanny     (501) staff       (20)     5407 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/text/test_pagebreak.py
--rw-r--r--   0 scanny     (501) staff       (20)    14897 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/text/test_paragraph.py
--rw-r--r--   0 scanny     (501) staff       (20)    19674 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/text/test_parfmt.py
--rw-r--r--   0 scanny     (501) staff       (20)    15221 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/text/test_run.py
--rw-r--r--   0 scanny     (501) staff       (20)    11626 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/text/test_tabstops.py
--rw-r--r--   0 scanny     (501) staff       (20)     4186 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/unitdata.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-04-30 02:58:01.648006 python_docx-1.1.1/tests/unitutil/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/unitutil/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)     8126 2024-04-30 00:55:22.000000 python_docx-1.1.1/tests/unitutil/cxml.py
--rw-r--r--   0 scanny     (501) staff       (20)     1675 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/unitutil/file.py
--rw-r--r--   0 scanny     (501) staff       (20)     4741 2023-11-04 03:19:46.000000 python_docx-1.1.1/tests/unitutil/mock.py
--rw-r--r--   0 scanny     (501) staff       (20)      159 2024-04-30 02:48:37.000000 python_docx-1.1.1/tox.ini
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.557550 python_docx-1.1.2/
+-rw-r--r--   0 scanny     (501) staff       (20)     7499 2024-05-01 19:29:56.000000 python_docx-1.1.2/HISTORY.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     1104 2014-03-01 10:03:55.000000 python_docx-1.1.2/LICENSE
+-rw-r--r--   0 scanny     (501) staff       (20)      230 2023-11-04 03:19:46.000000 python_docx-1.1.2/MANIFEST.in
+-rw-r--r--   0 scanny     (501) staff       (20)     2000 2024-05-01 19:41:40.557273 python_docx-1.1.2/PKG-INFO
+-rw-r--r--   0 scanny     (501) staff       (20)      642 2023-11-04 03:19:46.000000 python_docx-1.1.2/README.md
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.463141 python_docx-1.1.2/docs/
+-rw-r--r--   0 scanny     (501) staff       (20)     5580 2014-03-01 10:03:55.000000 python_docx-1.1.2/docs/Makefile
+-rw-r--r--   0 scanny     (501) staff       (20)      939 2014-06-22 21:06:59.000000 python_docx-1.1.2/docs/Session.vim
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.463307 python_docx-1.1.2/docs/_static/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python_docx-1.1.2/docs/_static/.gitignore
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.464080 python_docx-1.1.2/docs/_static/img/
+-rw-r--r--   0 scanny     (501) staff       (20)    77526 2014-03-01 10:03:55.000000 python_docx-1.1.2/docs/_static/img/example-docx-01.png
+-rw-r--r--   0 scanny     (501) staff       (20)    56762 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/_static/img/hdrftr-01.png
+-rw-r--r--   0 scanny     (501) staff       (20)    16218 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/_static/img/hdrftr-02.png
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.464303 python_docx-1.1.2/docs/_templates/
+-rw-r--r--   0 scanny     (501) staff       (20)      299 2014-03-01 10:03:55.000000 python_docx-1.1.2/docs/_templates/sidebarlinks.html
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.453955 python_docx-1.1.2/docs/_themes/
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.465336 python_docx-1.1.2/docs/_themes/armstrong/
+-rw-r--r--   0 scanny     (501) staff       (20)     1164 2014-01-06 15:34:59.000000 python_docx-1.1.2/docs/_themes/armstrong/LICENSE
+-rw-r--r--   0 scanny     (501) staff       (20)     1661 2014-01-06 15:34:59.000000 python_docx-1.1.2/docs/_themes/armstrong/layout.html
+-rw-r--r--   0 scanny     (501) staff       (20)     1147 2014-01-06 15:34:59.000000 python_docx-1.1.2/docs/_themes/armstrong/rtd-themes.conf
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.465487 python_docx-1.1.2/docs/_themes/armstrong/static/
+-rw-r--r--   0 scanny     (501) staff       (20)    16885 2014-01-06 15:34:59.000000 python_docx-1.1.2/docs/_themes/armstrong/static/rtd.css_t
+-rw-r--r--   0 scanny     (501) staff       (20)     1147 2014-01-06 15:34:59.000000 python_docx-1.1.2/docs/_themes/armstrong/theme.conf
+-rw-r--r--   0 scanny     (501) staff       (20)     1400 2014-01-06 15:34:59.000000 python_docx-1.1.2/docs/_themes/armstrong/theme.conf.orig
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.466807 python_docx-1.1.2/docs/api/
+-rw-r--r--   0 scanny     (501) staff       (20)      255 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/api/dml.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     3363 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/api/document.rst
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.469462 python_docx-1.1.2/docs/api/enum/
+-rw-r--r--   0 scanny     (501) staff       (20)      382 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/api/enum/MsoColorType.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     1270 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/api/enum/MsoThemeColorIndex.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      791 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/api/enum/WdAlignParagraph.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     4567 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/api/enum/WdBuiltinStyle.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      804 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/api/enum/WdCellVerticalAlignment.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      692 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/api/enum/WdColorIndex.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      771 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/api/enum/WdLineSpacing.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      339 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/api/enum/WdOrientation.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      336 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/api/enum/WdRowAlignment.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      519 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/api/enum/WdRowHeightRule.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      486 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/api/enum/WdSectionStart.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      421 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/api/enum/WdStyleType.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      434 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/api/enum/WdTabAlignment.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      285 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/api/enum/WdTabLeader.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      495 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/api/enum/WdTableDirection.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     1334 2014-06-22 22:15:58.000000 python_docx-1.1.2/docs/api/enum/WdUnderline.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      446 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/api/enum/index.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      565 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/api/section.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      206 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/api/settings.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      613 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/api/shape.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     1174 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/api/shared.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     1804 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/api/style.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      671 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/api/table.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     1008 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/api/text.rst
+-rw-r--r--   0 scanny     (501) staff       (20)    11139 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/conf.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.454681 python_docx-1.1.2/docs/dev/
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.469597 python_docx-1.1.2/docs/dev/analysis/
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.470417 python_docx-1.1.2/docs/dev/analysis/features/
+-rw-r--r--   0 scanny     (501) staff       (20)     7557 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/dev/analysis/features/coreprops.rst
+-rw-r--r--   0 scanny     (501) staff       (20)    11261 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/dev/analysis/features/header.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     2015 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/dev/analysis/features/numbering.rst
+-rw-r--r--   0 scanny     (501) staff       (20)    10642 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/dev/analysis/features/sections.rst
+-rw-r--r--   0 scanny     (501) staff       (20)    13252 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/dev/analysis/features/settings.rst
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.471016 python_docx-1.1.2/docs/dev/analysis/features/shapes/
+-rw-r--r--   0 scanny     (501) staff       (20)     1935 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/dev/analysis/features/shapes/index.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     9428 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/dev/analysis/features/shapes/picture.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     3459 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/dev/analysis/features/shapes/shapes-inline-size.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     6584 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/dev/analysis/features/shapes/shapes-inline.rst
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.472066 python_docx-1.1.2/docs/dev/analysis/features/styles/
+-rw-r--r--   0 scanny     (501) staff       (20)     5471 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/dev/analysis/features/styles/character-style.rst
+-rw-r--r--   0 scanny     (501) staff       (20)    12771 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/dev/analysis/features/styles/index.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     8560 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/dev/analysis/features/styles/latent-styles.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     5508 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/dev/analysis/features/styles/paragraph-style.rst
+-rw-r--r--   0 scanny     (501) staff       (20)    13979 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/dev/analysis/features/styles/style.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     8145 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/dev/analysis/features/styles/styles.rst
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.473010 python_docx-1.1.2/docs/dev/analysis/features/table/
+-rw-r--r--   0 scanny     (501) staff       (20)    20675 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/dev/analysis/features/table/cell-merge.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     9218 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/dev/analysis/features/table/index.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     8041 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/dev/analysis/features/table/table-cell.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     7949 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/dev/analysis/features/table/table-props.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     4150 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/dev/analysis/features/table/table-row.rst
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.474887 python_docx-1.1.2/docs/dev/analysis/features/text/
+-rw-r--r--   0 scanny     (501) staff       (20)     7581 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/dev/analysis/features/text/breaks.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     9879 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/dev/analysis/features/text/font-color.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     5902 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/dev/analysis/features/text/font-highlight-color.rst
+-rw-r--r--   0 scanny     (501) staff       (20)    18391 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/dev/analysis/features/text/font.rst
+-rw-r--r--   0 scanny     (501) staff       (20)    13033 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/dev/analysis/features/text/hyperlink.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      172 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/dev/analysis/features/text/index.rst
+-rw-r--r--   0 scanny     (501) staff       (20)    16282 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/dev/analysis/features/text/paragraph-format.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     3094 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/dev/analysis/features/text/run-content.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     9567 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/dev/analysis/features/text/tab-stops.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     4247 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/dev/analysis/features/text/underline.rst
+-rw-r--r--   0 scanny     (501) staff       (20)      576 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/dev/analysis/index.rst
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.476044 python_docx-1.1.2/docs/dev/analysis/schema/
+-rw-r--r--   0 scanny     (501) staff       (20)     7226 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/dev/analysis/schema/ct_body.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     4659 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/dev/analysis/schema/ct_document.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     6406 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/dev/analysis/schema/ct_p.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     3839 2024-04-30 03:01:02.000000 python_docx-1.1.2/docs/index.rst
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.478301 python_docx-1.1.2/docs/user/
+-rw-r--r--   0 scanny     (501) staff       (20)     1287 2014-01-06 15:34:59.000000 python_docx-1.1.2/docs/user/api-concepts.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     3635 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/user/documents.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     6897 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/user/hdrftr.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     1031 2014-03-01 09:49:51.000000 python_docx-1.1.2/docs/user/install.rst
+-rw-r--r--   0 scanny     (501) staff       (20)    11875 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/user/quickstart.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     3950 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/user/sections.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     1477 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/user/shapes.rst
+-rw-r--r--   0 scanny     (501) staff       (20)    12392 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/user/styles-understanding.rst
+-rw-r--r--   0 scanny     (501) staff       (20)    13587 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/user/styles-using.rst
+-rw-r--r--   0 scanny     (501) staff       (20)     6981 2024-04-30 03:01:02.000000 python_docx-1.1.2/docs/user/tables.rst
+-rw-r--r--   0 scanny     (501) staff       (20)    14125 2023-11-04 03:19:46.000000 python_docx-1.1.2/docs/user/text.rst
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.489453 python_docx-1.1.2/features/
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.489638 python_docx-1.1.2/features/_scratch/
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.489807 python_docx-1.1.2/features/_scratch/test_out/
+-rw-r--r--   0 scanny     (501) staff       (20)     1738 2013-08-15 22:17:06.000000 python_docx-1.1.2/features/_scratch/test_out/[Content_Types].xml
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.489950 python_docx-1.1.2/features/_scratch/test_out/_rels/
+-rw-r--r--   0 scanny     (501) staff       (20)      734 2013-08-13 09:49:22.000000 python_docx-1.1.2/features/_scratch/test_out/_rels/.rels
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.490263 python_docx-1.1.2/features/_scratch/test_out/customXml/
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.490393 python_docx-1.1.2/features/_scratch/test_out/customXml/_rels/
+-rw-r--r--   0 scanny     (501) staff       (20)      295 2013-08-15 22:17:06.000000 python_docx-1.1.2/features/_scratch/test_out/customXml/_rels/item1.xml.rels
+-rw-r--r--   0 scanny     (501) staff       (20)      218 2013-08-15 22:17:06.000000 python_docx-1.1.2/features/_scratch/test_out/customXml/item1.xml
+-rw-r--r--   0 scanny     (501) staff       (20)      341 2013-08-15 22:17:06.000000 python_docx-1.1.2/features/_scratch/test_out/customXml/itemProps1.xml
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.490827 python_docx-1.1.2/features/_scratch/test_out/docProps/
+-rw-r--r--   0 scanny     (501) staff       (20)     1035 2013-08-13 09:49:22.000000 python_docx-1.1.2/features/_scratch/test_out/docProps/app.xml
+-rw-r--r--   0 scanny     (501) staff       (20)      806 2013-08-15 22:17:06.000000 python_docx-1.1.2/features/_scratch/test_out/docProps/core.xml
+-rw-r--r--   0 scanny     (501) staff       (20)     8324 2013-08-15 22:17:06.000000 python_docx-1.1.2/features/_scratch/test_out/docProps/thumbnail.jpeg
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.491977 python_docx-1.1.2/features/_scratch/test_out/word/
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.492105 python_docx-1.1.2/features/_scratch/test_out/word/_rels/
+-rw-r--r--   0 scanny     (501) staff       (20)     1227 2013-08-15 22:17:06.000000 python_docx-1.1.2/features/_scratch/test_out/word/_rels/document.xml.rels
+-rw-r--r--   0 scanny     (501) staff       (20)     1758 2013-08-15 22:17:06.000000 python_docx-1.1.2/features/_scratch/test_out/word/document.xml
+-rw-r--r--   0 scanny     (501) staff       (20)     2552 2013-08-15 22:17:06.000000 python_docx-1.1.2/features/_scratch/test_out/word/fontTable.xml
+-rw-r--r--   0 scanny     (501) staff       (20)     5514 2013-08-15 22:17:06.000000 python_docx-1.1.2/features/_scratch/test_out/word/numbering.xml
+-rw-r--r--   0 scanny     (501) staff       (20)     2500 2013-08-15 22:17:06.000000 python_docx-1.1.2/features/_scratch/test_out/word/settings.xml
+-rw-r--r--   0 scanny     (501) staff       (20)    26716 2013-08-15 22:17:06.000000 python_docx-1.1.2/features/_scratch/test_out/word/styles.xml
+-rw-r--r--   0 scanny     (501) staff       (20)    27582 2013-08-15 22:17:06.000000 python_docx-1.1.2/features/_scratch/test_out/word/stylesWithEffects.xml
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.492237 python_docx-1.1.2/features/_scratch/test_out/word/theme/
+-rw-r--r--   0 scanny     (501) staff       (20)     7643 2013-08-13 09:49:22.000000 python_docx-1.1.2/features/_scratch/test_out/word/theme/theme1.xml
+-rw-r--r--   0 scanny     (501) staff       (20)      431 2013-08-13 09:49:22.000000 python_docx-1.1.2/features/_scratch/test_out/word/webSettings.xml
+-rw-r--r--   0 scanny     (501) staff       (20)    36593 2024-05-01 19:24:26.000000 python_docx-1.1.2/features/_scratch/test_out.docx
+-rw-r--r--   0 scanny     (501) staff       (20)      476 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/api-open-document.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      407 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/blk-add-paragraph.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      378 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/blk-add-table.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      963 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/blk-iter-inner-content.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      981 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/doc-access-collections.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      395 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/doc-access-sections.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      840 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/doc-add-heading.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      358 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/doc-add-page-break.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      883 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/doc-add-paragraph.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      997 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/doc-add-picture.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     1110 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/doc-add-section.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      729 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/doc-add-table.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      892 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/doc-coreprops.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     1398 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/doc-settings.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      598 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/doc-styles.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      268 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/environment.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3116 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/hdr-header-footer.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     2116 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/hlk-props.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     1499 2015-02-19 07:28:57.000000 python_docx-1.1.2/features/img-characterize-image.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      402 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/num-access-numbering-part.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     1917 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/par-access-inner-content.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      312 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/par-access-parfmt.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      527 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/par-add-run.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      632 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/par-alignment-prop.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      405 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/par-clear-paragraph.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      577 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/par-insert-paragraph.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      390 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/par-set-text.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      871 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/par-style-prop.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     1101 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/pbk-split-para.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      269 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/run-access-font.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      945 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/run-access-inner-content.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      458 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/run-add-content.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      804 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/run-add-picture.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     1173 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/run-char-style.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      373 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/run-clear-run.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     1757 2015-02-19 07:28:57.000000 python_docx-1.1.2/features/run-enum-props.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     5276 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/sct-section.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     1070 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/shp-inline-shape-access.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      575 2015-02-19 07:28:57.000000 python_docx-1.1.2/features/shp-inline-shape-size.feature
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.496620 python_docx-1.1.2/features/steps/
+-rw-r--r--   0 scanny     (501) staff       (20)     1661 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/api.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3636 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/block.py
+-rw-r--r--   0 scanny     (501) staff       (20)     4417 2024-05-01 19:25:50.000000 python_docx-1.1.2/features/steps/coreprops.py
+-rw-r--r--   0 scanny     (501) staff       (20)     8815 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/document.py
+-rw-r--r--   0 scanny     (501) staff       (20)     6797 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/font.py
+-rw-r--r--   0 scanny     (501) staff       (20)     5055 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/hdrftr.py
+-rw-r--r--   0 scanny     (501) staff       (20)      836 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/helpers.py
+-rw-r--r--   0 scanny     (501) staff       (20)     4588 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/hyperlink.py
+-rw-r--r--   0 scanny     (501) staff       (20)     2212 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/image.py
+-rw-r--r--   0 scanny     (501) staff       (20)      952 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/numbering.py
+-rw-r--r--   0 scanny     (501) staff       (20)     6052 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/pagebreak.py
+-rw-r--r--   0 scanny     (501) staff       (20)     8975 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/paragraph.py
+-rw-r--r--   0 scanny     (501) staff       (20)     7912 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/parfmt.py
+-rw-r--r--   0 scanny     (501) staff       (20)     9750 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/section.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1842 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/settings.py
+-rw-r--r--   0 scanny     (501) staff       (20)     5169 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/shape.py
+-rw-r--r--   0 scanny     (501) staff       (20)      544 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/shared.py
+-rw-r--r--   0 scanny     (501) staff       (20)    17994 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/styles.py
+-rw-r--r--   0 scanny     (501) staff       (20)    18911 2024-04-30 03:01:02.000000 python_docx-1.1.2/features/steps/table.py
+-rw-r--r--   0 scanny     (501) staff       (20)     4645 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/tabstops.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.507934 python_docx-1.1.2/features/steps/test_files/
+-rw-r--r--   0 scanny     (501) staff       (20)    25142 2015-02-19 07:28:57.000000 python_docx-1.1.2/features/steps/test_files/blk-containing-table.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    15649 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/test_files/blk-paras-and-tables.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    80603 2023-09-10 05:09:30.000000 python_docx-1.1.2/features/steps/test_files/court-exif.jpg
+-rw-r--r--   0 scanny     (501) staff       (20)    25591 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/test_files/doc-access-sections.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    17956 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/test_files/doc-add-section.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    11992 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/test_files/doc-coreprops.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    21366 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/test_files/doc-default.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    11394 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/test_files/doc-no-coreprops.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    17711 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/test_files/doc-odd-even-hdrs.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    21309 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/test_files/doc-word-default-blank.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    15846 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/test_files/fnt-color.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    18079 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/test_files/hdr-header-footer.docx
+-rw-r--r--   0 scanny     (501) staff       (20)   355196 2015-02-19 07:28:57.000000 python_docx-1.1.2/features/steps/test_files/jfif-300-dpi.jpg
+-rw-r--r--   0 scanny     (501) staff       (20)   768608 2023-09-10 05:09:16.000000 python_docx-1.1.2/features/steps/test_files/jpeg420exif.jpg
+-rw-r--r--   0 scanny     (501) staff       (20)   263222 2015-02-19 07:28:57.000000 python_docx-1.1.2/features/steps/test_files/lena.bmp
+-rw-r--r--   0 scanny     (501) staff       (20)    72985 2015-02-19 07:28:57.000000 python_docx-1.1.2/features/steps/test_files/lena.gif
+-rw-r--r--   0 scanny     (501) staff       (20)   786572 2023-09-10 05:09:00.000000 python_docx-1.1.2/features/steps/test_files/lena.tif
+-rw-r--r--   0 scanny     (501) staff       (20)   104428 2023-09-10 05:08:43.000000 python_docx-1.1.2/features/steps/test_files/lena_std.jpg
+-rw-r--r--   0 scanny     (501) staff       (20)    64276 2015-02-19 07:28:57.000000 python_docx-1.1.2/features/steps/test_files/monty-truth.png
+-rw-r--r--   0 scanny     (501) staff       (20)   308280 2015-02-19 07:28:57.000000 python_docx-1.1.2/features/steps/test_files/mountain.bmp
+-rw-r--r--   0 scanny     (501) staff       (20)    24334 2015-02-19 07:28:57.000000 python_docx-1.1.2/features/steps/test_files/num-having-numbering-part.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    15126 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/test_files/par-alignment.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    12071 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/test_files/par-hlink-frags.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    12385 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/test_files/par-hyperlinks.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    27969 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/test_files/par-known-paragraphs.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    20901 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/test_files/par-known-styles.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    12244 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/test_files/par-rendered-page-breaks.docx
+-rw-r--r--   0 scanny     (501) staff       (20)     3277 2015-02-19 07:28:57.000000 python_docx-1.1.2/features/steps/test_files/python-icon.jpeg
+-rw-r--r--   0 scanny     (501) staff       (20)    26645 2015-02-19 07:28:57.000000 python_docx-1.1.2/features/steps/test_files/run-char-style.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    14645 2015-02-19 07:28:57.000000 python_docx-1.1.2/features/steps/test_files/run-enumerated-props.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    10409 2015-02-19 07:28:57.000000 python_docx-1.1.2/features/steps/test_files/sample.tif
+-rw-r--r--   0 scanny     (501) staff       (20)    14849 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/test_files/sct-first-page-hdrftr.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    12051 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/test_files/sct-inner-content.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    28168 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/test_files/sct-section-props.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    10760 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/test_files/set-no-settings-part.docx
+-rw-r--r--   0 scanny     (501) staff       (20)   122610 2015-02-19 07:28:57.000000 python_docx-1.1.2/features/steps/test_files/shp-inline-shape-access.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    12195 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/test_files/sty-behav-props.docx
+-rw-r--r--   0 scanny     (501) staff       (20)     8358 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/test_files/sty-having-no-styles-part.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    21573 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/test_files/sty-having-styles-part.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    13560 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/test_files/sty-known-styles.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    13170 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/test_files/tab-stops.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    25129 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/test_files/tbl-2x2-table.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    36051 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/test_files/tbl-cell-access.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    13773 2024-04-30 03:01:02.000000 python_docx-1.1.2/features/steps/test_files/tbl-cell-props.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    13654 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/test_files/tbl-col-props.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    50294 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/test_files/tbl-having-applied-style.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    32010 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/test_files/tbl-having-tables.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    16017 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/test_files/tbl-on-off-props.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    20419 2024-04-30 03:01:02.000000 python_docx-1.1.2/features/steps/test_files/tbl-props.docx
+-rw-r--r--   0 scanny     (501) staff       (20)   146892 2015-02-19 07:28:57.000000 python_docx-1.1.2/features/steps/test_files/test.png
+-rw-r--r--   0 scanny     (501) staff       (20)    12859 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/test_files/txt-font-highlight-color.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    37924 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/test_files/txt-font-props.docx
+-rw-r--r--   0 scanny     (501) staff       (20)    10059 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/steps/text.py
+-rw-r--r--   0 scanny     (501) staff       (20)      463 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/sty-access-font.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      568 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/sty-access-latent-styles.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      488 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/sty-access-parfmt.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      767 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/sty-add-style.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      352 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/sty-delete-style.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      654 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/sty-latent-add-del.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     4102 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/sty-latent-props.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     5464 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/sty-style-props.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     1264 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/tab-access-tabs.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     1877 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/tab-tabstop-props.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      594 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/tbl-add-row-or-col.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     1523 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/tbl-cell-access.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      428 2024-04-30 03:01:02.000000 python_docx-1.1.2/features/tbl-cell-add-table.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     2105 2024-04-30 03:01:02.000000 python_docx-1.1.2/features/tbl-cell-props.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      343 2024-04-30 03:01:02.000000 python_docx-1.1.2/features/tbl-cell-text.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     1062 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/tbl-col-props.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      944 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/tbl-item-access.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     2294 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/tbl-merge-cells.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     2907 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/tbl-props.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     2188 2024-04-30 03:01:02.000000 python_docx-1.1.2/features/tbl-row-props.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     1169 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/tbl-style.feature
+-rw-r--r--   0 scanny     (501) staff       (20)      645 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/txt-add-break.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     2279 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/txt-font-color.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     8120 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/txt-font-props.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     7648 2023-11-04 03:19:46.000000 python_docx-1.1.2/features/txt-parfmt-props.feature
+-rw-r--r--   0 scanny     (501) staff       (20)     3563 2024-05-01 19:25:50.000000 python_docx-1.1.2/pyproject.toml
+-rw-r--r--   0 scanny     (501) staff       (20)       76 2024-04-30 03:01:02.000000 python_docx-1.1.2/requirements-dev.txt
+-rw-r--r--   0 scanny     (501) staff       (20)       68 2024-04-30 03:01:02.000000 python_docx-1.1.2/requirements-docs.txt
+-rw-r--r--   0 scanny     (501) staff       (20)       97 2024-05-01 19:25:50.000000 python_docx-1.1.2/requirements-test.txt
+-rw-r--r--   0 scanny     (501) staff       (20)       30 2023-11-04 03:19:46.000000 python_docx-1.1.2/requirements.txt
+-rw-r--r--   0 scanny     (501) staff       (20)       38 2024-05-01 19:41:40.557621 python_docx-1.1.2/setup.cfg
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.458485 python_docx-1.1.2/src/
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.510151 python_docx-1.1.2/src/docx/
+-rw-r--r--   0 scanny     (501) staff       (20)     1711 2024-05-01 19:27:13.000000 python_docx-1.1.2/src/docx/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1350 2024-04-30 03:01:02.000000 python_docx-1.1.2/src/docx/api.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3469 2024-04-30 03:01:02.000000 python_docx-1.1.2/src/docx/blkcntnr.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.510436 python_docx-1.1.2/src/docx/dml/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/dml/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3794 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/dml/color.py
+-rw-r--r--   0 scanny     (501) staff       (20)     8021 2024-04-30 03:01:02.000000 python_docx-1.1.2/src/docx/document.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.510584 python_docx-1.1.2/src/docx/drawing/
+-rw-r--r--   0 scanny     (501) staff       (20)      504 2024-04-30 03:01:02.000000 python_docx-1.1.2/src/docx/drawing/__init__.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.511847 python_docx-1.1.2/src/docx/enum/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2024-05-01 19:25:50.000000 python_docx-1.1.2/src/docx/enum/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)     4888 2024-04-30 03:01:02.000000 python_docx-1.1.2/src/docx/enum/base.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3346 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/enum/dml.py
+-rw-r--r--   0 scanny     (501) staff       (20)     2391 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/enum/section.py
+-rw-r--r--   0 scanny     (501) staff       (20)      396 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/enum/shape.py
+-rw-r--r--   0 scanny     (501) staff       (20)    10137 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/enum/style.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3943 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/enum/table.py
+-rw-r--r--   0 scanny     (501) staff       (20)    10276 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/enum/text.py
+-rw-r--r--   0 scanny     (501) staff       (20)      454 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/exceptions.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.513524 python_docx-1.1.2/src/docx/image/
+-rw-r--r--   0 scanny     (501) staff       (20)      664 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/image/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1347 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/image/bmp.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3466 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/image/constants.py
+-rw-r--r--   0 scanny     (501) staff       (20)      383 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/image/exceptions.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1118 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/image/gif.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3089 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/image/helpers.py
+-rw-r--r--   0 scanny     (501) staff       (20)     8011 2024-05-01 19:25:50.000000 python_docx-1.1.2/src/docx/image/image.py
+-rw-r--r--   0 scanny     (501) staff       (20)    15422 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/image/jpeg.py
+-rw-r--r--   0 scanny     (501) staff       (20)     8214 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/image/png.py
+-rw-r--r--   0 scanny     (501) staff       (20)    10379 2024-04-30 03:01:03.000000 python_docx-1.1.2/src/docx/image/tiff.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.516121 python_docx-1.1.2/src/docx/opc/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/opc/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)    19080 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/opc/constants.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3402 2024-05-01 19:25:50.000000 python_docx-1.1.2/src/docx/opc/coreprops.py
+-rw-r--r--   0 scanny     (501) staff       (20)      264 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/opc/exceptions.py
+-rw-r--r--   0 scanny     (501) staff       (20)     8238 2024-05-01 19:25:50.000000 python_docx-1.1.2/src/docx/opc/oxml.py
+-rw-r--r--   0 scanny     (501) staff       (20)     8761 2024-05-01 19:25:50.000000 python_docx-1.1.2/src/docx/opc/package.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3733 2024-05-01 19:25:50.000000 python_docx-1.1.2/src/docx/opc/packuri.py
+-rw-r--r--   0 scanny     (501) staff       (20)     9025 2024-05-01 19:25:50.000000 python_docx-1.1.2/src/docx/opc/part.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.516446 python_docx-1.1.2/src/docx/opc/parts/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/opc/parts/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1775 2024-05-01 19:25:50.000000 python_docx-1.1.2/src/docx/opc/parts/coreprops.py
+-rw-r--r--   0 scanny     (501) staff       (20)     4005 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/opc/phys_pkg.py
+-rw-r--r--   0 scanny     (501) staff       (20)     9640 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/opc/pkgreader.py
+-rw-r--r--   0 scanny     (501) staff       (20)     4524 2024-04-30 03:01:03.000000 python_docx-1.1.2/src/docx/opc/pkgwriter.py
+-rw-r--r--   0 scanny     (501) staff       (20)     5653 2024-05-01 19:25:50.000000 python_docx-1.1.2/src/docx/opc/rel.py
+-rw-r--r--   0 scanny     (501) staff       (20)      996 2024-04-30 03:01:03.000000 python_docx-1.1.2/src/docx/opc/shared.py
+-rw-r--r--   0 scanny     (501) staff       (20)      638 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/opc/spec.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.519357 python_docx-1.1.2/src/docx/oxml/
+-rw-r--r--   0 scanny     (501) staff       (20)     8100 2024-04-30 03:01:03.000000 python_docx-1.1.2/src/docx/oxml/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)    10594 2024-05-01 19:25:50.000000 python_docx-1.1.2/src/docx/oxml/coreprops.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3593 2024-05-01 19:25:50.000000 python_docx-1.1.2/src/docx/oxml/document.py
+-rw-r--r--   0 scanny     (501) staff       (20)      397 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/oxml/drawing.py
+-rw-r--r--   0 scanny     (501) staff       (20)      261 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/oxml/exceptions.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3796 2024-04-30 03:01:03.000000 python_docx-1.1.2/src/docx/oxml/ns.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3965 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/oxml/numbering.py
+-rw-r--r--   0 scanny     (501) staff       (20)     2324 2024-05-01 19:25:50.000000 python_docx-1.1.2/src/docx/oxml/parser.py
+-rw-r--r--   0 scanny     (501) staff       (20)    20395 2024-04-30 03:01:03.000000 python_docx-1.1.2/src/docx/oxml/section.py
+-rw-r--r--   0 scanny     (501) staff       (20)     4264 2024-05-01 19:25:50.000000 python_docx-1.1.2/src/docx/oxml/settings.py
+-rw-r--r--   0 scanny     (501) staff       (20)     9012 2024-05-01 19:25:50.000000 python_docx-1.1.2/src/docx/oxml/shape.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1875 2024-05-01 19:25:50.000000 python_docx-1.1.2/src/docx/oxml/shared.py
+-rw-r--r--   0 scanny     (501) staff       (20)    10834 2024-04-30 03:01:03.000000 python_docx-1.1.2/src/docx/oxml/simpletypes.py
+-rw-r--r--   0 scanny     (501) staff       (20)    10643 2024-05-01 19:25:50.000000 python_docx-1.1.2/src/docx/oxml/styles.py
+-rw-r--r--   0 scanny     (501) staff       (20)    33632 2024-05-01 19:25:50.000000 python_docx-1.1.2/src/docx/oxml/table.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.521100 python_docx-1.1.2/src/docx/oxml/text/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/oxml/text/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)    11499 2024-05-01 19:25:50.000000 python_docx-1.1.2/src/docx/oxml/text/font.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1467 2024-04-30 03:01:03.000000 python_docx-1.1.2/src/docx/oxml/text/hyperlink.py
+-rw-r--r--   0 scanny     (501) staff       (20)    11262 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/oxml/text/pagebreak.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3538 2024-04-30 03:01:03.000000 python_docx-1.1.2/src/docx/oxml/text/paragraph.py
+-rw-r--r--   0 scanny     (501) staff       (20)    11986 2024-04-30 03:01:03.000000 python_docx-1.1.2/src/docx/oxml/text/parfmt.py
+-rw-r--r--   0 scanny     (501) staff       (20)     9629 2024-04-30 03:01:03.000000 python_docx-1.1.2/src/docx/oxml/text/run.py
+-rw-r--r--   0 scanny     (501) staff       (20)    25567 2024-04-30 03:01:03.000000 python_docx-1.1.2/src/docx/oxml/xmlchemy.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3971 2024-05-01 19:25:50.000000 python_docx-1.1.2/src/docx/package.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.522861 python_docx-1.1.2/src/docx/parts/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/parts/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)     5580 2024-05-01 19:25:50.000000 python_docx-1.1.2/src/docx/parts/document.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1709 2024-05-01 19:25:50.000000 python_docx-1.1.2/src/docx/parts/hdrftr.py
+-rw-r--r--   0 scanny     (501) staff       (20)     2739 2024-05-01 19:25:50.000000 python_docx-1.1.2/src/docx/parts/image.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1056 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/parts/numbering.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1725 2024-05-01 19:25:50.000000 python_docx-1.1.2/src/docx/parts/settings.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3857 2024-05-01 19:25:50.000000 python_docx-1.1.2/src/docx/parts/story.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1413 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/parts/styles.py
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2024-04-30 03:01:03.000000 python_docx-1.1.2/src/docx/py.typed
+-rw-r--r--   0 scanny     (501) staff       (20)    18412 2024-05-01 19:25:50.000000 python_docx-1.1.2/src/docx/section.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1082 2024-05-01 19:25:50.000000 python_docx-1.1.2/src/docx/settings.py
+-rw-r--r--   0 scanny     (501) staff       (20)     2969 2024-05-01 19:25:50.000000 python_docx-1.1.2/src/docx/shape.py
+-rw-r--r--   0 scanny     (501) staff       (20)    13509 2024-04-30 03:01:03.000000 python_docx-1.1.2/src/docx/shared.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.523788 python_docx-1.1.2/src/docx/styles/
+-rw-r--r--   0 scanny     (501) staff       (20)     1406 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/styles/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)     7211 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/styles/latent.py
+-rw-r--r--   0 scanny     (501) staff       (20)     8051 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/styles/style.py
+-rw-r--r--   0 scanny     (501) staff       (20)     5717 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/styles/styles.py
+-rw-r--r--   0 scanny     (501) staff       (20)    19477 2024-04-30 03:01:03.000000 python_docx-1.1.2/src/docx/table.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.524802 python_docx-1.1.2/src/docx/templates/
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.525032 python_docx-1.1.2/src/docx/templates/default-docx-template/
+-rw-r--r--   0 scanny     (501) staff       (20)     1782 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/templates/default-docx-template/[Content_Types].xml
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.525197 python_docx-1.1.2/src/docx/templates/default-docx-template/_rels/
+-rw-r--r--   0 scanny     (501) staff       (20)      748 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/templates/default-docx-template/_rels/.rels
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.525543 python_docx-1.1.2/src/docx/templates/default-docx-template/customXml/
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.525704 python_docx-1.1.2/src/docx/templates/default-docx-template/customXml/_rels/
+-rw-r--r--   0 scanny     (501) staff       (20)      300 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/templates/default-docx-template/customXml/_rels/item1.xml.rels
+-rw-r--r--   0 scanny     (501) staff       (20)      262 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/templates/default-docx-template/customXml/item1.xml
+-rw-r--r--   0 scanny     (501) staff       (20)      354 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/templates/default-docx-template/customXml/itemProps1.xml
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.526327 python_docx-1.1.2/src/docx/templates/default-docx-template/docProps/
+-rw-r--r--   0 scanny     (501) staff       (20)     1132 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/templates/default-docx-template/docProps/app.xml
+-rw-r--r--   0 scanny     (501) staff       (20)      753 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/templates/default-docx-template/docProps/core.xml
+-rw-r--r--   0 scanny     (501) staff       (20)     8324 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/templates/default-docx-template/docProps/thumbnail.jpeg
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.530002 python_docx-1.1.2/src/docx/templates/default-docx-template/word/
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.530245 python_docx-1.1.2/src/docx/templates/default-docx-template/word/_rels/
+-rw-r--r--   0 scanny     (501) staff       (20)     1253 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/templates/default-docx-template/word/_rels/document.xml.rels
+-rw-r--r--   0 scanny     (501) staff       (20)     1594 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/templates/default-docx-template/word/document.xml
+-rw-r--r--   0 scanny     (501) staff       (20)     2811 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/templates/default-docx-template/word/fontTable.xml
+-rw-r--r--   0 scanny     (501) staff       (20)     6747 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/templates/default-docx-template/word/numbering.xml
+-rw-r--r--   0 scanny     (501) staff       (20)     2749 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/templates/default-docx-template/word/settings.xml
+-rw-r--r--   0 scanny     (501) staff       (20)   438677 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/templates/default-docx-template/word/styles.xml
+-rw-r--r--   0 scanny     (501) staff       (20)   438131 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/templates/default-docx-template/word/stylesWithEffects.xml
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.530451 python_docx-1.1.2/src/docx/templates/default-docx-template/word/theme/
+-rw-r--r--   0 scanny     (501) staff       (20)    10939 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/templates/default-docx-template/word/theme/theme1.xml
+-rw-r--r--   0 scanny     (501) staff       (20)      438 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/templates/default-docx-template/word/webSettings.xml
+-rw-r--r--   0 scanny     (501) staff       (20)     1395 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/templates/default-footer.xml
+-rw-r--r--   0 scanny     (501) staff       (20)     1395 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/templates/default-header.xml
+-rw-r--r--   0 scanny     (501) staff       (20)     1640 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/templates/default-settings.xml
+-rw-r--r--   0 scanny     (501) staff       (20)    15823 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/templates/default-styles.xml
+-rw-r--r--   0 scanny     (501) staff       (20)    38116 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/templates/default.docx
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.532339 python_docx-1.1.2/src/docx/text/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/text/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)    13653 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/text/font.py
+-rw-r--r--   0 scanny     (501) staff       (20)     5257 2024-04-30 03:01:03.000000 python_docx-1.1.2/src/docx/text/hyperlink.py
+-rw-r--r--   0 scanny     (501) staff       (20)     4950 2024-04-30 03:01:03.000000 python_docx-1.1.2/src/docx/text/pagebreak.py
+-rw-r--r--   0 scanny     (501) staff       (20)     6828 2024-04-30 03:01:03.000000 python_docx-1.1.2/src/docx/text/paragraph.py
+-rw-r--r--   0 scanny     (501) staff       (20)    10339 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/text/parfmt.py
+-rw-r--r--   0 scanny     (501) staff       (20)     9657 2024-05-01 19:25:50.000000 python_docx-1.1.2/src/docx/text/run.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3910 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/text/tabstops.py
+-rw-r--r--   0 scanny     (501) staff       (20)      864 2023-11-04 03:19:46.000000 python_docx-1.1.2/src/docx/types.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.556876 python_docx-1.1.2/src/python_docx.egg-info/
+-rw-r--r--   0 scanny     (501) staff       (20)     2000 2024-05-01 19:41:40.000000 python_docx-1.1.2/src/python_docx.egg-info/PKG-INFO
+-rw-r--r--   0 scanny     (501) staff       (20)    16643 2024-05-01 19:41:40.000000 python_docx-1.1.2/src/python_docx.egg-info/SOURCES.txt
+-rw-r--r--   0 scanny     (501) staff       (20)        1 2024-05-01 19:41:40.000000 python_docx-1.1.2/src/python_docx.egg-info/dependency_links.txt
+-rw-r--r--   0 scanny     (501) staff       (20)       37 2024-05-01 19:41:40.000000 python_docx-1.1.2/src/python_docx.egg-info/requires.txt
+-rw-r--r--   0 scanny     (501) staff       (20)        5 2024-05-01 19:41:40.000000 python_docx-1.1.2/src/python_docx.egg-info/top_level.txt
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.535574 python_docx-1.1.2/tests/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2013-07-29 10:11:43.000000 python_docx-1.1.2/tests/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)      452 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/conftest.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.535894 python_docx-1.1.2/tests/dml/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/dml/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)     5437 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/dml/test_color.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.537134 python_docx-1.1.2/tests/image/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python_docx-1.1.2/tests/image/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1108 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/image/test_bmp.py
+-rw-r--r--   0 scanny     (501) staff       (20)      960 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/image/test_gif.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1569 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/image/test_helpers.py
+-rw-r--r--   0 scanny     (501) staff       (20)    11958 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/image/test_image.py
+-rw-r--r--   0 scanny     (501) staff       (20)    21556 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/image/test_jpeg.py
+-rw-r--r--   0 scanny     (501) staff       (20)    14741 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/image/test_png.py
+-rw-r--r--   0 scanny     (501) staff       (20)    14704 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/image/test_tiff.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.538784 python_docx-1.1.2/tests/opc/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python_docx-1.1.2/tests/opc/__init__.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.539082 python_docx-1.1.2/tests/opc/parts/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/opc/parts/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)     2021 2024-05-01 19:25:50.000000 python_docx-1.1.2/tests/opc/parts/test_coreprops.py
+-rw-r--r--   0 scanny     (501) staff       (20)     7608 2024-05-01 19:25:50.000000 python_docx-1.1.2/tests/opc/test_coreprops.py
+-rw-r--r--   0 scanny     (501) staff       (20)     4866 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/opc/test_oxml.py
+-rw-r--r--   0 scanny     (501) staff       (20)    17017 2024-04-30 03:01:03.000000 python_docx-1.1.2/tests/opc/test_package.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3313 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/opc/test_packuri.py
+-rw-r--r--   0 scanny     (501) staff       (20)    14592 2024-05-01 19:25:50.000000 python_docx-1.1.2/tests/opc/test_part.py
+-rw-r--r--   0 scanny     (501) staff       (20)     6289 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/opc/test_phys_pkg.py
+-rw-r--r--   0 scanny     (501) staff       (20)    19028 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/opc/test_pkgreader.py
+-rw-r--r--   0 scanny     (501) staff       (20)     7218 2024-04-30 03:01:03.000000 python_docx-1.1.2/tests/opc/test_pkgwriter.py
+-rw-r--r--   0 scanny     (501) staff       (20)     9565 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/opc/test_rel.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.539541 python_docx-1.1.2/tests/opc/unitdata/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python_docx-1.1.2/tests/opc/unitdata/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)     8626 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/opc/unitdata/rels.py
+-rw-r--r--   0 scanny     (501) staff       (20)      765 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/opc/unitdata/types.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.540691 python_docx-1.1.2/tests/oxml/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python_docx-1.1.2/tests/oxml/__init__.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.541022 python_docx-1.1.2/tests/oxml/parts/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python_docx-1.1.2/tests/oxml/parts/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1432 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/oxml/parts/test_document.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.541265 python_docx-1.1.2/tests/oxml/parts/unitdata/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python_docx-1.1.2/tests/oxml/parts/unitdata/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)      388 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/oxml/parts/unitdata/document.py
+-rw-r--r--   0 scanny     (501) staff       (20)     4108 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/oxml/test__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)      587 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/oxml/test_document.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1634 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/oxml/test_ns.py
+-rw-r--r--   0 scanny     (501) staff       (20)      592 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/oxml/test_section.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1367 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/oxml/test_styles.py
+-rw-r--r--   0 scanny     (501) staff       (20)    13656 2024-04-30 03:01:03.000000 python_docx-1.1.2/tests/oxml/test_table.py
+-rw-r--r--   0 scanny     (501) staff       (20)    28193 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/oxml/test_xmlchemy.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.541650 python_docx-1.1.2/tests/oxml/text/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/oxml/text/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1481 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/oxml/text/test_hyperlink.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1156 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/oxml/text/test_run.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.542964 python_docx-1.1.2/tests/oxml/unitdata/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python_docx-1.1.2/tests/oxml/unitdata/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1172 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/oxml/unitdata/dml.py
+-rw-r--r--   0 scanny     (501) staff       (20)      412 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/oxml/unitdata/numbering.py
+-rw-r--r--   0 scanny     (501) staff       (20)      893 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/oxml/unitdata/section.py
+-rw-r--r--   0 scanny     (501) staff       (20)      677 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/oxml/unitdata/shared.py
+-rw-r--r--   0 scanny     (501) staff       (20)      449 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/oxml/unitdata/styles.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3153 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/oxml/unitdata/text.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.544389 python_docx-1.1.2/tests/parts/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2014-03-01 10:03:55.000000 python_docx-1.1.2/tests/parts/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)    12295 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/parts/test_document.py
+-rw-r--r--   0 scanny     (501) staff       (20)     5062 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/parts/test_hdrftr.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3945 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/parts/test_image.py
+-rw-r--r--   0 scanny     (501) staff       (20)     2580 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/parts/test_numbering.py
+-rw-r--r--   0 scanny     (501) staff       (20)     2576 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/parts/test_settings.py
+-rw-r--r--   0 scanny     (501) staff       (20)     5270 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/parts/test_story.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1695 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/parts/test_styles.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.545056 python_docx-1.1.2/tests/styles/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/styles/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)    14144 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/styles/test_latent.py
+-rw-r--r--   0 scanny     (501) staff       (20)    20304 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/styles/test_style.py
+-rw-r--r--   0 scanny     (501) staff       (20)    14836 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/styles/test_styles.py
+-rw-r--r--   0 scanny     (501) staff       (20)     2327 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/test_api.py
+-rw-r--r--   0 scanny     (501) staff       (20)     5451 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/test_blkcntnr.py
+-rw-r--r--   0 scanny     (501) staff       (20)    14036 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/test_document.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3188 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/test_enum.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.549721 python_docx-1.1.2/tests/test_files/
+-rw-r--r--   0 scanny     (501) staff       (20)   146892 2014-06-27 08:20:06.000000 python_docx-1.1.2/tests/test_files/150-dpi.png
+-rw-r--r--   0 scanny     (501) staff       (20)   125824 2023-09-10 05:05:56.000000 python_docx-1.1.2/tests/test_files/300-dpi.TIF
+-rw-r--r--   0 scanny     (501) staff       (20)   355196 2014-06-27 08:20:06.000000 python_docx-1.1.2/tests/test_files/300-dpi.jpg
+-rw-r--r--   0 scanny     (501) staff       (20)    39921 2014-06-27 08:20:06.000000 python_docx-1.1.2/tests/test_files/300-dpi.png
+-rw-r--r--   0 scanny     (501) staff       (20)     9454 2014-06-27 08:20:06.000000 python_docx-1.1.2/tests/test_files/72-dpi.tiff
+-rw-r--r--   0 scanny     (501) staff       (20)     1526 2014-03-01 10:03:55.000000 python_docx-1.1.2/tests/test_files/CVS_LOGO.WMF
+-rw-r--r--   0 scanny     (501) staff       (20)    11949 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/test_files/blk-inner-content.docx
+-rw-r--r--   0 scanny     (501) staff       (20)   768608 2023-09-10 05:05:40.000000 python_docx-1.1.2/tests/test_files/exif-420-dpi.jpg
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.549892 python_docx-1.1.2/tests/test_files/expanded_docx/
+-rw-r--r--   0 scanny     (501) staff       (20)     1738 2014-03-01 10:03:55.000000 python_docx-1.1.2/tests/test_files/expanded_docx/[Content_Types].xml
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.550061 python_docx-1.1.2/tests/test_files/expanded_docx/_rels/
+-rw-r--r--   0 scanny     (501) staff       (20)      734 2014-03-01 10:03:55.000000 python_docx-1.1.2/tests/test_files/expanded_docx/_rels/.rels
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.550380 python_docx-1.1.2/tests/test_files/expanded_docx/customXml/
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.550546 python_docx-1.1.2/tests/test_files/expanded_docx/customXml/_rels/
+-rw-r--r--   0 scanny     (501) staff       (20)      295 2014-03-01 10:03:55.000000 python_docx-1.1.2/tests/test_files/expanded_docx/customXml/_rels/item1.xml.rels
+-rw-r--r--   0 scanny     (501) staff       (20)      217 2014-03-01 10:03:55.000000 python_docx-1.1.2/tests/test_files/expanded_docx/customXml/item1.xml
+-rw-r--r--   0 scanny     (501) staff       (20)      340 2014-03-01 10:03:55.000000 python_docx-1.1.2/tests/test_files/expanded_docx/customXml/itemProps1.xml
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.551048 python_docx-1.1.2/tests/test_files/expanded_docx/docProps/
+-rw-r--r--   0 scanny     (501) staff       (20)     1036 2014-03-01 10:03:55.000000 python_docx-1.1.2/tests/test_files/expanded_docx/docProps/app.xml
+-rw-r--r--   0 scanny     (501) staff       (20)      802 2014-03-01 10:03:55.000000 python_docx-1.1.2/tests/test_files/expanded_docx/docProps/core.xml
+-rw-r--r--   0 scanny     (501) staff       (20)    13032 2014-06-27 08:20:06.000000 python_docx-1.1.2/tests/test_files/expanded_docx/docProps/thumbnail.jpeg
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.552319 python_docx-1.1.2/tests/test_files/expanded_docx/word/
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.552495 python_docx-1.1.2/tests/test_files/expanded_docx/word/_rels/
+-rw-r--r--   0 scanny     (501) staff       (20)     1227 2014-03-01 10:03:55.000000 python_docx-1.1.2/tests/test_files/expanded_docx/word/_rels/document.xml.rels
+-rw-r--r--   0 scanny     (501) staff       (20)     1819 2023-09-10 05:07:15.000000 python_docx-1.1.2/tests/test_files/expanded_docx/word/document.xml
+-rw-r--r--   0 scanny     (501) staff       (20)     2566 2014-03-01 10:03:55.000000 python_docx-1.1.2/tests/test_files/expanded_docx/word/fontTable.xml
+-rw-r--r--   0 scanny     (501) staff       (20)     5513 2014-03-01 10:03:55.000000 python_docx-1.1.2/tests/test_files/expanded_docx/word/numbering.xml
+-rw-r--r--   0 scanny     (501) staff       (20)     2520 2014-03-01 10:03:55.000000 python_docx-1.1.2/tests/test_files/expanded_docx/word/settings.xml
+-rw-r--r--   0 scanny     (501) staff       (20)    26715 2014-03-01 10:03:55.000000 python_docx-1.1.2/tests/test_files/expanded_docx/word/styles.xml
+-rw-r--r--   0 scanny     (501) staff       (20)    27581 2014-03-01 10:03:55.000000 python_docx-1.1.2/tests/test_files/expanded_docx/word/stylesWithEffects.xml
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.552689 python_docx-1.1.2/tests/test_files/expanded_docx/word/theme/
+-rw-r--r--   0 scanny     (501) staff       (20)     7642 2014-03-01 10:03:55.000000 python_docx-1.1.2/tests/test_files/expanded_docx/word/theme/theme1.xml
+-rw-r--r--   0 scanny     (501) staff       (20)      430 2014-03-01 10:03:55.000000 python_docx-1.1.2/tests/test_files/expanded_docx/word/webSettings.xml
+-rw-r--r--   0 scanny     (501) staff       (20)   132875 2014-03-01 10:03:55.000000 python_docx-1.1.2/tests/test_files/having-images.docx
+-rw-r--r--   0 scanny     (501) staff       (20)     7958 2014-06-27 08:20:06.000000 python_docx-1.1.2/tests/test_files/jfif-iguana.jpg
+-rw-r--r--   0 scanny     (501) staff       (20)    10409 2014-06-27 08:20:06.000000 python_docx-1.1.2/tests/test_files/little-endian.tif
+-rw-r--r--   0 scanny     (501) staff       (20)    64276 2014-06-27 08:20:06.000000 python_docx-1.1.2/tests/test_files/monty-truth.png
+-rw-r--r--   0 scanny     (501) staff       (20)     3277 2014-06-27 08:20:06.000000 python_docx-1.1.2/tests/test_files/python-icon.jpeg
+-rw-r--r--   0 scanny     (501) staff       (20)     2036 2014-06-27 08:20:06.000000 python_docx-1.1.2/tests/test_files/python-icon.png
+-rw-r--r--   0 scanny     (501) staff       (20)     6111 2014-06-27 08:20:06.000000 python_docx-1.1.2/tests/test_files/python-powered.png
+-rw-r--r--   0 scanny     (501) staff       (20)    45210 2014-06-27 08:20:06.000000 python_docx-1.1.2/tests/test_files/python.bmp
+-rw-r--r--   0 scanny     (501) staff       (20)    12051 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/test_files/sct-inner-content.docx
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.553451 python_docx-1.1.2/tests/test_files/snippets/
+-rw-r--r--   0 scanny     (501) staff       (20)     2949 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/test_files/snippets/add-row-col.txt
+-rw-r--r--   0 scanny     (501) staff       (20)     1110 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/test_files/snippets/inline.txt
+-rw-r--r--   0 scanny     (501) staff       (20)     1756 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/test_files/snippets/new-tbl.txt
+-rw-r--r--   0 scanny     (501) staff       (20)     4595 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/test_files/snippets/tbl-cells.txt
+-rw-r--r--   0 scanny     (501) staff       (20)    33273 2014-06-27 08:20:06.000000 python_docx-1.1.2/tests/test_files/sonic.gif
+-rw-r--r--   0 scanny     (501) staff       (20)    31773 2014-03-01 10:03:55.000000 python_docx-1.1.2/tests/test_files/test.docx
+-rw-r--r--   0 scanny     (501) staff       (20)     5297 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/test_package.py
+-rw-r--r--   0 scanny     (501) staff       (20)    31223 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/test_section.py
+-rw-r--r--   0 scanny     (501) staff       (20)     2169 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/test_settings.py
+-rw-r--r--   0 scanny     (501) staff       (20)     6785 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/test_shape.py
+-rw-r--r--   0 scanny     (501) staff       (20)     4385 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/test_shared.py
+-rw-r--r--   0 scanny     (501) staff       (20)    32484 2024-04-30 03:01:03.000000 python_docx-1.1.2/tests/test_table.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.555503 python_docx-1.1.2/tests/text/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/text/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)    15804 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/text/test_font.py
+-rw-r--r--   0 scanny     (501) staff       (20)     5192 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/text/test_hyperlink.py
+-rw-r--r--   0 scanny     (501) staff       (20)     5407 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/text/test_pagebreak.py
+-rw-r--r--   0 scanny     (501) staff       (20)    14897 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/text/test_paragraph.py
+-rw-r--r--   0 scanny     (501) staff       (20)    19674 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/text/test_parfmt.py
+-rw-r--r--   0 scanny     (501) staff       (20)    15221 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/text/test_run.py
+-rw-r--r--   0 scanny     (501) staff       (20)    11626 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/text/test_tabstops.py
+-rw-r--r--   0 scanny     (501) staff       (20)     4186 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/unitdata.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-01 19:41:40.556458 python_docx-1.1.2/tests/unitutil/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/unitutil/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)     8126 2024-04-30 03:01:03.000000 python_docx-1.1.2/tests/unitutil/cxml.py
+-rw-r--r--   0 scanny     (501) staff       (20)     1675 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/unitutil/file.py
+-rw-r--r--   0 scanny     (501) staff       (20)     4741 2023-11-04 03:19:46.000000 python_docx-1.1.2/tests/unitutil/mock.py
+-rw-r--r--   0 scanny     (501) staff       (20)      166 2024-05-01 19:25:50.000000 python_docx-1.1.2/tox.ini
```

### Comparing `python_docx-1.1.1/HISTORY.rst` & `python_docx-1.1.2/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 .. :changelog:
 
 Release History
 ---------------
 
+1.1.2 (2024-05-01)
+++++++++++++++++++
+
+- Fix #1383 Revert lxml<=4.9.2 pin that breaks Python 3.12 install
+- Fix #1385 Support use of Part._rels by python-docx-template
+- Add support and testing for Python 3.12
+
 1.1.1 (2024-04-29)
 ++++++++++++++++++
 
 - Fix #531, #1146 Index error on table with misaligned borders
 - Fix #1335 Tolerate invalid float value in bottom-margin
 - Fix #1337 Do not require typing-extensions at runtime
```

### Comparing `python_docx-1.1.1/LICENSE` & `python_docx-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/PKG-INFO` & `python_docx-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-docx
-Version: 1.1.1
+Version: 1.1.2
 Summary: Create, read, and update Microsoft Word .docx files.
 Author-email: Steve Canny <stcanny@gmail.com>
 License: MIT
 Project-URL: Changelog, https://github.com/python-openxml/python-docx/blob/master/HISTORY.rst
 Project-URL: Documentation, https://python-docx.readthedocs.org/en/latest/
 Project-URL: Homepage, https://github.com/python-openxml/python-docx
 Project-URL: Repository, https://github.com/python-openxml/python-docx
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Office/Business :: Office Suites
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: lxml<=4.9.2,>=3.1.0
+Requires-Dist: lxml>=3.1.0
 Requires-Dist: typing_extensions>=4.9.0
 
 # python-docx
 
 *python-docx* is a Python library for reading, creating, and updating Microsoft Word 2007+ (.docx) files.
 
 ## Installation
```

### Comparing `python_docx-1.1.1/README.md` & `python_docx-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/Makefile` & `python_docx-1.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/Session.vim` & `python_docx-1.1.2/docs/Session.vim`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/_static/img/example-docx-01.png` & `python_docx-1.1.2/docs/_static/img/example-docx-01.png`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/_static/img/hdrftr-01.png` & `python_docx-1.1.2/docs/_static/img/hdrftr-01.png`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/_static/img/hdrftr-02.png` & `python_docx-1.1.2/docs/_static/img/hdrftr-02.png`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/_themes/armstrong/LICENSE` & `python_docx-1.1.2/docs/_themes/armstrong/LICENSE`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/_themes/armstrong/layout.html` & `python_docx-1.1.2/docs/_themes/armstrong/layout.html`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/_themes/armstrong/rtd-themes.conf` & `python_docx-1.1.2/docs/_themes/armstrong/rtd-themes.conf`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/_themes/armstrong/static/rtd.css_t` & `python_docx-1.1.2/docs/_themes/armstrong/static/rtd.css_t`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/_themes/armstrong/theme.conf` & `python_docx-1.1.2/docs/_themes/armstrong/theme.conf`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/_themes/armstrong/theme.conf.orig` & `python_docx-1.1.2/docs/_themes/armstrong/theme.conf.orig`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/api/document.rst` & `python_docx-1.1.2/docs/api/document.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/api/enum/MsoThemeColorIndex.rst` & `python_docx-1.1.2/docs/api/enum/MsoThemeColorIndex.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/api/enum/WdAlignParagraph.rst` & `python_docx-1.1.2/docs/api/enum/WdAlignParagraph.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/api/enum/WdBuiltinStyle.rst` & `python_docx-1.1.2/docs/api/enum/WdBuiltinStyle.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/api/enum/WdCellVerticalAlignment.rst` & `python_docx-1.1.2/docs/api/enum/WdCellVerticalAlignment.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/api/enum/WdColorIndex.rst` & `python_docx-1.1.2/docs/api/enum/WdColorIndex.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/api/enum/WdLineSpacing.rst` & `python_docx-1.1.2/docs/api/enum/WdLineSpacing.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/api/enum/WdRowHeightRule.rst` & `python_docx-1.1.2/docs/api/enum/WdRowHeightRule.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/api/enum/WdUnderline.rst` & `python_docx-1.1.2/docs/api/enum/WdUnderline.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/api/section.rst` & `python_docx-1.1.2/docs/api/section.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/api/shape.rst` & `python_docx-1.1.2/docs/api/shape.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/api/shared.rst` & `python_docx-1.1.2/docs/api/shared.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/api/style.rst` & `python_docx-1.1.2/docs/api/style.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/api/table.rst` & `python_docx-1.1.2/docs/api/table.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/api/text.rst` & `python_docx-1.1.2/docs/api/text.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/conf.py` & `python_docx-1.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/dev/analysis/features/coreprops.rst` & `python_docx-1.1.2/docs/dev/analysis/features/coreprops.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/dev/analysis/features/header.rst` & `python_docx-1.1.2/docs/dev/analysis/features/header.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/dev/analysis/features/numbering.rst` & `python_docx-1.1.2/docs/dev/analysis/features/numbering.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/dev/analysis/features/sections.rst` & `python_docx-1.1.2/docs/dev/analysis/features/sections.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/dev/analysis/features/settings.rst` & `python_docx-1.1.2/docs/dev/analysis/features/settings.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/dev/analysis/features/shapes/index.rst` & `python_docx-1.1.2/docs/dev/analysis/features/shapes/index.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/dev/analysis/features/shapes/picture.rst` & `python_docx-1.1.2/docs/dev/analysis/features/shapes/picture.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/dev/analysis/features/shapes/shapes-inline-size.rst` & `python_docx-1.1.2/docs/dev/analysis/features/shapes/shapes-inline-size.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/dev/analysis/features/shapes/shapes-inline.rst` & `python_docx-1.1.2/docs/dev/analysis/features/shapes/shapes-inline.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/dev/analysis/features/styles/character-style.rst` & `python_docx-1.1.2/docs/dev/analysis/features/styles/character-style.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/dev/analysis/features/styles/index.rst` & `python_docx-1.1.2/docs/dev/analysis/features/styles/index.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/dev/analysis/features/styles/latent-styles.rst` & `python_docx-1.1.2/docs/dev/analysis/features/styles/latent-styles.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/dev/analysis/features/styles/paragraph-style.rst` & `python_docx-1.1.2/docs/dev/analysis/features/styles/paragraph-style.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/dev/analysis/features/styles/style.rst` & `python_docx-1.1.2/docs/dev/analysis/features/styles/style.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/dev/analysis/features/styles/styles.rst` & `python_docx-1.1.2/docs/dev/analysis/features/styles/styles.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/dev/analysis/features/table/cell-merge.rst` & `python_docx-1.1.2/docs/dev/analysis/features/table/cell-merge.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/dev/analysis/features/table/index.rst` & `python_docx-1.1.2/docs/dev/analysis/features/table/index.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/dev/analysis/features/table/table-cell.rst` & `python_docx-1.1.2/docs/dev/analysis/features/table/table-cell.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/dev/analysis/features/table/table-props.rst` & `python_docx-1.1.2/docs/dev/analysis/features/table/table-props.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/dev/analysis/features/table/table-row.rst` & `python_docx-1.1.2/docs/dev/analysis/features/table/table-row.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/dev/analysis/features/text/breaks.rst` & `python_docx-1.1.2/docs/dev/analysis/features/text/breaks.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/dev/analysis/features/text/font-color.rst` & `python_docx-1.1.2/docs/dev/analysis/features/text/font-color.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/dev/analysis/features/text/font-highlight-color.rst` & `python_docx-1.1.2/docs/dev/analysis/features/text/font-highlight-color.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/dev/analysis/features/text/font.rst` & `python_docx-1.1.2/docs/dev/analysis/features/text/font.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/dev/analysis/features/text/hyperlink.rst` & `python_docx-1.1.2/docs/dev/analysis/features/text/hyperlink.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/dev/analysis/features/text/paragraph-format.rst` & `python_docx-1.1.2/docs/dev/analysis/features/text/paragraph-format.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/dev/analysis/features/text/run-content.rst` & `python_docx-1.1.2/docs/dev/analysis/features/text/run-content.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/dev/analysis/features/text/tab-stops.rst` & `python_docx-1.1.2/docs/dev/analysis/features/text/tab-stops.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/dev/analysis/features/text/underline.rst` & `python_docx-1.1.2/docs/dev/analysis/features/text/underline.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/dev/analysis/index.rst` & `python_docx-1.1.2/docs/dev/analysis/index.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/dev/analysis/schema/ct_body.rst` & `python_docx-1.1.2/docs/dev/analysis/schema/ct_body.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/dev/analysis/schema/ct_document.rst` & `python_docx-1.1.2/docs/dev/analysis/schema/ct_document.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/dev/analysis/schema/ct_p.rst` & `python_docx-1.1.2/docs/dev/analysis/schema/ct_p.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/index.rst` & `python_docx-1.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/user/api-concepts.rst` & `python_docx-1.1.2/docs/user/api-concepts.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/user/documents.rst` & `python_docx-1.1.2/docs/user/documents.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/user/hdrftr.rst` & `python_docx-1.1.2/docs/user/hdrftr.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/user/install.rst` & `python_docx-1.1.2/docs/user/install.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/user/quickstart.rst` & `python_docx-1.1.2/docs/user/quickstart.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/user/sections.rst` & `python_docx-1.1.2/docs/user/sections.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/user/shapes.rst` & `python_docx-1.1.2/docs/user/shapes.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/user/styles-understanding.rst` & `python_docx-1.1.2/docs/user/styles-understanding.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/user/styles-using.rst` & `python_docx-1.1.2/docs/user/styles-using.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/user/tables.rst` & `python_docx-1.1.2/docs/user/tables.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/docs/user/text.rst` & `python_docx-1.1.2/docs/user/text.rst`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/_scratch/test_out/[Content_Types].xml` & `python_docx-1.1.2/features/_scratch/test_out/[Content_Types].xml`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/_scratch/test_out/_rels/.rels` & `python_docx-1.1.2/features/_scratch/test_out/_rels/.rels`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/_scratch/test_out/docProps/app.xml` & `python_docx-1.1.2/features/_scratch/test_out/docProps/app.xml`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/_scratch/test_out/docProps/core.xml` & `python_docx-1.1.2/features/_scratch/test_out/docProps/core.xml`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/_scratch/test_out/docProps/thumbnail.jpeg` & `python_docx-1.1.2/features/_scratch/test_out/docProps/thumbnail.jpeg`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/_scratch/test_out/word/_rels/document.xml.rels` & `python_docx-1.1.2/features/_scratch/test_out/word/_rels/document.xml.rels`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/_scratch/test_out/word/document.xml` & `python_docx-1.1.2/features/_scratch/test_out/word/document.xml`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/_scratch/test_out/word/fontTable.xml` & `python_docx-1.1.2/features/_scratch/test_out/word/fontTable.xml`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/_scratch/test_out/word/numbering.xml` & `python_docx-1.1.2/features/_scratch/test_out/word/numbering.xml`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/_scratch/test_out/word/settings.xml` & `python_docx-1.1.2/features/_scratch/test_out/word/settings.xml`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/_scratch/test_out/word/styles.xml` & `python_docx-1.1.2/features/_scratch/test_out/word/styles.xml`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/_scratch/test_out/word/stylesWithEffects.xml` & `python_docx-1.1.2/features/_scratch/test_out/word/stylesWithEffects.xml`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/_scratch/test_out/word/theme/theme1.xml` & `python_docx-1.1.2/features/_scratch/test_out/word/theme/theme1.xml`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/_scratch/test_out.docx` & `python_docx-1.1.2/features/_scratch/test_out.docx`

 * *Format-specific differences are supported for Microsoft Word .docx files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Microsoft Word 2007+*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 504b 0304 1400 0000 0800 9d9e 9d58 ad52  PK...........X.R
+00000000: 504b 0304 1400 0000 0800 0d63 a158 ad52  PK.........c.X.R
 00000010: a591 9501 0000 ca06 0000 1300 0000 5b43  ..............[C
 00000020: 6f6e 7465 6e74 5f54 7970 6573 5d2e 786d  ontent_Types].xm
 00000030: 6cb5 954d 4fdb 4010 86ef fd15 962f 3e20  l..MO.@....../> 
 00000040: 7b43 0f15 aae2 7028 702c 911a 44af 9bf5  {C....p(p,..D...
 00000050: 3859 d82f ed4c 02f9 f7cc 3a89 55d1 5087  8Y./.L....:.U.P.
 00000060: 062e 919c 99f7 7d1e dbb2 3dbe 7cb6 265b  ......}...=.|.&[
 00000070: 4344 ed5d 5d9c 57a3 2203 a77c a3dd a22e  CD.]].W."..|....
@@ -23,15 +23,15 @@
 00000160: c80f 8635 553f b152 bb41 8f96 c933 3937  ...5U?.R.A...397
 00000170: ff71 ea43 227d f5a0 845b d939 444e 7dbc  .q.C"}...[.9DN}.
 00000180: 445f 3d28 8140 c47b f8f1 0efb e661 05da  D_=(.@.{.....a..
 00000190: 18f8 0c81 aef7 48fc bda6 e575 db82 a263  ......H....u...c
 000001a0: 4c2c 9629 5bfd 951d a411 bf91 61fb 7bfa  L,.)[.......a.{.
 000001b0: 0ba7 ab19 443e c1fc d7a7 dde5 3fca f722  ....D>......?.."
 000001c0: a2fb 144d 5e00 504b 0304 1400 0000 0800  ...M^.PK........
-000001d0: 9d9e 9d58 7926 4b40 f800 0000 de02 0000  ...Xy&K@........
+000001d0: 0d63 a158 7926 4b40 f800 0000 de02 0000  .c.Xy&K@........
 000001e0: 0b00 0000 5f72 656c 732f 2e72 656c 73ad  ...._rels/.rels.
 000001f0: 92cd 4a03 3110 80ef 3e45 c825 a76e b655  ..J.1...>E.%.n.U
 00000200: 44a4 d95e 44e8 4da4 3ec0 98cc eea6 6e7e  D..^D.M.>.....n~
 00000210: 48a6 dabe bd51 445d 5816 c11e e7ef e363  H....QD]X......c
 00000220: 66d6 9ba3 1bd8 2ba6 6c83 5762 59d5 82a1  f.....+.l.WbY...
 00000230: d7c1 58df 29f1 b4bb 5fdc 0896 09bc 8121  ..X.)..._......!
 00000240: 7854 e284 596c 9a8b f523 0e40 6526 f736  xT..Yl...#.@e&.6
@@ -41,15 +41,15 @@
 00000280: 6c77 8af8 3fb6 7448 6080 40ea 9070 1153  lw..?.tH`.@..p.S
 00000290: 994e 6431 1738 a40e 4971 13f4 4349 e7cf  .Nd1.8..Iq..CI..
 000002a0: 8eaa 90b9 9c16 bafa bb50 685b abf1 2ee8  .........Ph[....
 000002b0: 8343 4f53 5e78 24f4 06cd bc12 c438 67b4  .COS^x$......8g.
 000002c0: 3ca7 d1b8 e347 e62d 2423 cd57 7ace 6675  <....G.-$#.Wz.fu
 000002d0: de83 517f 70cf 1eec 30b1 97ef 5ab5 8fd8  ..Q.p...0...Z...
 000002e0: 7d08 c9d1 5b36 ef50 4b03 0414 0000 0008  }...[6.PK.......
-000002f0: 009d 9e9d 5888 860b 5369 0100 00d1 0200  ....X...Si......
+000002f0: 000d 63a1 5888 860b 5369 0100 00d1 0200  ..c.X...Si......
 00000300: 0011 0000 0064 6f63 5072 6f70 732f 636f  .....docProps/co
 00000310: 7265 2e78 6d6c 9d92 cb4e c330 1045 f77c  re.xml...N.0.E.|
 00000320: 45d4 4d56 89f3 1008 4549 2a01 ea8a 4a48  E.MV....EI*...JH
 00000330: 1481 d8b9 f634 354d 6ccb 9e36 cddf e3a4  .....45Ml..6....
 00000340: 6d5a a02b 761e df3b c7f3 703e dd37 b5b7  mZ.+v..;..p>.7..
 00000350: 0363 8592 851f 8791 ef81 648a 0b59 15fe  .c........d..Y..
 00000360: db62 16dc fb9e 452a 39ad 9584 c2ef c0fa  .b....E*9.......
@@ -66,15 +66,15 @@
 00000410: 5dab 0cb7 870c 0e96 19a1 d1ed a8ac 4082  ].............@.
 00000420: a108 dc5b 76de 6fc4 a5b1 c7d4 d4e2 dc2d  ...[v.o........-
 00000430: 7325 803f 7464 b833 b013 fdb6 cb38 2797  s%.?td.3.....8'.
 00000440: 617e 9cdd a10e c777 3d67 8709 9d94 f7f4  a~.....w=g......
 00000450: f169 319b 9449 14a7 419c 0449 ba48 d22c  .i1..I..A..I.H.,
 00000460: becd a2e8 b37f ff47 fe19 d81c 2bf8 37f1  .......G....+.7.
 00000470: 0418 ea67 0e5e 29d3 7743 fefc c2f2 1b50  ...g.^).wC.....P
-00000480: 4b03 0414 0000 0008 009d 9e9d 58f4 dbdb  K...........X...
+00000480: 4b03 0414 0000 0008 000d 63a1 58f4 dbdb  K.........c.X...
 00000490: 17eb 0100 006c 0400 0010 0000 0064 6f63  .....l.......doc
 000004a0: 5072 6f70 732f 6170 702e 786d 6c9d 54cb  Props/app.xml.T.
 000004b0: 6edb 3010 bcfb 2b04 5d74 8a69 0741 5118  n.0...+.]t.i.AQ.
 000004c0: 9282 d641 d143 dd1a b092 9cb7 d4ca 224a  ...A.C........"J
 000004d0: 9104 b931 e27e 7df9 8815 3986 2ff5 893b  ...1.~}...9./..;
 000004e0: b33b fbb4 cafb d741 6607 b44e 6855 15cb  .;.....Af..NhU..
 000004f0: f9a2 c850 71dd 0ab5 af8a c7e6 dbcd e722  ...Pq.........."
@@ -100,15 +100,15 @@
 00000630: 9f35 1a11 7625 e185 7eb9 01e5 6f27 0594  .5..v%..~...o'..
 00000640: 6b3d 1850 4776 5ae2 1ff7 681a fd10 2ef1  k=.PGvZ...h.....
 00000650: 6d31 e7e0 f975 3d0b ea77 0638 7eb8 b309  m1...u=..w.8~...
 00000660: 1e97 ed09 6cfd c98c cb1e 81b8 6cdf 9795  ....l.......l...
 00000670: 3ecd 57df 243b 879c 1755 7b6c 4f91 97c4  >.W.$;...U{lO...
 00000680: db49 3fa5 4f47 bdbc 9b2f fc2f 1ef0 099b  .I?.OG..././....
 00000690: f9f3 1bff d5f5 ec1f 504b 0304 1400 0000  ........PK......
-000006a0: 0800 9d9e 9d58 059c 75c4 1502 0000 4206  .....X..u.....B.
+000006a0: 0800 0d63 a158 059c 75c4 1502 0000 4206  ...c.X..u.....B.
 000006b0: 0000 1100 0000 776f 7264 2f64 6f63 756d  ......word/docum
 000006c0: 656e 742e 786d 6ca5 94cb 8eda 3014 86f7  ent.xml.....0...
 000006d0: 7d8a 349b ac20 0ed0 9446 8459 3062 348b  }.4.. ...F.Y0b4.
 000006e0: 4aa8 b40f 601c 27b1 26f1 b16c 4386 3e7d  J...`.'.&..lC.>}
 000006f0: 8f73 8154 9510 1d36 b6cf edf3 ef13 c7ab  .s.T...6........
 00000700: a7f7 baf2 4e5c 1b01 320d a229 093c 2e19  ....N\..2..).<..
 00000710: 6442 1669 f0eb e776 b20c 3c63 a9cc 6805  dB.i...v..<c..h.
@@ -136,15 +136,15 @@
 00000870: 14b7 2a54 b1ff 8d51 bc52 d16c b620 2eb3  ..*T...Q.R.l. ..
 00000880: c4f5 9725 aec3 2ee1 3b75 fb58 c09b 1f2d  ...%....;u.X...-
 00000890: ba14 2d8a 1249 d192 b4e6 01ac 85fa 1aae  ..-..I..........
 000008a0: 783e 8a96 9c66 1cd5 7c9d b566 0e60 4766  x>...f..|..f.`Gf
 000008b0: 71b4 add9 6fc7 a032 e835 8a32 dee5 b46e  q...o..2.5.2...n
 000008c0: ecc8 8b16 9963 0bc9 77c2 3254 398f db68  .....c..w.2T9..h
 000008d0: 3874 a35d 766d 0daf afff fa0f 504b 0304  8t.]vm......PK..
-000008e0: 1400 0000 0800 9d9e 9d58 6e80 1b12 3201  .........Xn...2.
+000008e0: 1400 0000 0800 0d63 a158 6e80 1b12 3201  .......c.Xn...2.
 000008f0: 0000 cb04 0000 1c00 0000 776f 7264 2f5f  ..........word/_
 00000900: 7265 6c73 2f64 6f63 756d 656e 742e 786d  rels/document.xm
 00000910: 6c2e 7265 6c73 ad94 414f 8330 1886 effe  l.rels..AO.0....
 00000920: 0ac2 8593 14a6 6e8b 19ec a226 bb2a 46af  ......n....&.*F.
 00000930: a57c 8546 da92 f643 e5df 5bdd 642c 43e2  .|.F...C..[.d,C.
 00000940: 81e3 f736 7d9f 276d d3cd f653 d6de 3b18  ...6}.'m...S..;.
 00000950: 2bb4 4a82 388c 020f 14d3 8550 6512 3c67  +.J.8......Pe.<g
@@ -159,15 +159,15 @@
 000009e0: 5f04 56f7 9c03 c333 f860 69ca e366 d663  _.V....3.`i..f.c
 000009f0: 0044 77bf 4397 4332 a5b0 9c53 e103 f2a7  .Dw.C.C2...S....
 00000a00: 338b 4138 25b2 9a53 846b 8519 cd6b 386a  3.A8%..S.k...k8j
 00000a10: f4d1 94c4 7a4e 0974 7b07 023f e33e 8ca7  ....zN.t{..?.>..
 00000a20: 1ce2 391d 586b 51cb 5747 eb3d c2f0 9812  ..9.XkQ.WG.=....
 00000a30: 8120 276d 1673 daa8 56e6 60dc 4b38 daf4  . 'm.s..V.`.K8..
 00000a40: d1af 0439 f983 d22f 504b 0304 1400 0000  ...9.../PK......
-00000a50: 0800 9d9e 9d58 07d4 af99 732f 0000 1255  .....X....s/...U
+00000a50: 0800 0d63 a158 07d4 af99 732f 0000 1255  ...c.X....s/...U
 00000a60: 0500 0f00 0000 776f 7264 2f73 7479 6c65  ......word/style
 00000a70: 732e 786d 6ced 5d5d 93e2 46b2 7dbf bfa2  s.xml.]]..F.}...
 00000a80: a35f fce4 6d90 8400 c7ce 6e00 9276 1c61  ._..m.....n..v.a
 00000a90: 7bbd 9eb1 ef33 4d33 d3ec d0d0 1768 8fed  {....3M3.....h..
 00000aa0: 5f7f 2521 401f 5552 5556 4aaa 92b2 3bc2  _.%!@.URUVJ...;.
 00000ab0: 9e16 5029 e557 9d93 5465 fdfd 9f7f bc6c  ..P).W..Te.....l
 00000ac0: ef7e 5f1f 8e9b fdee dd37 c3bf 0dbe b95b  .~_......7.....[
@@ -921,15 +921,15 @@
 00003980: 8f38 d50f 29d4 ffcc 1a21 057b 3871 a6ec  .8..)....!.{8q..
 00003990: afc5 989b 518c 460a 0d3c 2cde 3a85 da4f  ....Q.F..<,.:..O
 000039a0: ecd5 f370 6145 a450 b20f 328d 14e0 fb20  ...paE.P..2.... 
 000039b0: 0929 1052 a813 29a8 ed14 6a0f 29d4 7fec  .).R..)...j.)...
 000039c0: 9e7e 48a1 fe67 d608 29f8 b6bb 90e9 7061  .~H..g..).....pa
 000039d0: 3452 68e0 6111 0fbc acfb 1449 3d0f bcbc  4Rh.a......I=...
 000039e0: 2185 cbbf 8eff f87f 504b 0304 1400 0000  !.......PK......
-000039f0: 0800 9d9e 9d58 6079 82d3 3935 0000 73af  .....X`y..95..s.
+000039f0: 0800 0d63 a158 6079 82d3 3935 0000 73af  ...c.X`y..95..s.
 00003a00: 0600 1a00 0000 776f 7264 2f73 7479 6c65  ......word/style
 00003a10: 7357 6974 6845 6666 6563 7473 2e78 6d6c  sWithEffects.xml
 00003a20: ed7d 5d97 a346 b2ed fbf9 15b5 eac5 4f9e  .}]..F........O.
 00003a30: 9600 21c9 cb7d ce12 02c6 5ecb e3f1 99f6  ..!..}....^.....
 00003a40: f83e abab d45d 9aae 92ea 4a2a b7ed 5f7f  .>...]....J*.._.
 00003a50: 409f 8012 c88f 48c8 84ed 7e98 2940 1990  @.....H...~.)@..
 00003a60: b933 73c7 0e88 f8fe 7ffe 7879 befb 7db9  .3s.......xy..}.
@@ -1776,15 +1776,15 @@
 00006ef0: 6691 6df4 95f6 f722 47e1 2862 9778 60cd  f.m...."G.(b.x`.
 00006f00: 151b 58a4 c647 2260 9175 1982 b22c 9222  ..X..G"`.u...,."
 00006f10: 4310 5864 e142 b0c8 beb0 48e9 6c0c b6b3  C.Xd.B....H.l...
 00006f20: c838 08bd 80fd ea15 ebc1 c122 0de9 446b  .8........."..Dk
 00006f30: 5964 e4fa 7391 74a7 7d66 916d f495 6e16  Yd..s.t.}f.m..n.
 00006f40: 1907 f3d9 8c4d b958 73c5 0616 a9f1 9132  .....M.Xs......2
 00006f50: 2cf2 f27f 939d fcff 0050 4b03 0414 0000  ,........PK.....
-00006f60: 0008 009d 9e9d 58a3 3f46 5fbf 0300 00e7  ......X.?F_.....
+00006f60: 0008 000d 63a1 58a3 3f46 5fbf 0300 00e7  ....c.X.?F_.....
 00006f70: 0900 0011 0000 0077 6f72 642f 7365 7474  .......word/sett
 00006f80: 696e 6773 2e78 6d6c b556 dd72 da38 14be  ings.xml.V.r.8..
 00006f90: dfa7 60b8 e166 09b6 714c e329 e924 b0de  ..`..f..qL.).$..
 00006fa0: 4d26 6c33 75fa 00b2 7d00 6df4 3792 0ca1  M&l3u...}.m.7...
 00006fb0: 4fdf 23db 8ac9 9666 98ed ec15 f2f9 cebf  O.#....f........
 00006fc0: be73 c4c7 4f2f 9c0d 76a0 0d95 623e 0a2f  .s..O/..v...b>./
 00006fd0: 82d1 0044 292b 2a36 f3d1 d7a7 6cfc 6134  ...D)+*6....l.a4
@@ -1839,15 +1839,15 @@
 000072e0: 3e27 03a3 68c5 c90b 5e6a 10cd 9cf3 4e9b  >'..h...^j....N.
 000072f0: 357b fb8d aec3 9cb2 7aeb a122 96f8 fdf0  5{......z.."....
 00007300: c6b8 9989 7fe5 e2de a192 227f f303 2ffa  ..........".../.
 00007310: e7e5 a22d 8b51 838b 4ce1 4b64 a5f6 d8ef  ...-.Q..L.Kd....
 00007320: 0d16 c658 7479 87a3 87a7 461e c541 1205  ...Xty....F..A..
 00007330: 49f8 0ab7 41ee 38d9 c052 d15e 711a 04dd  I...A.8..R.^q...
 00007340: 80fa bf68 d7df 0150 4b03 0414 0000 0008  ...h...PK.......
-00007350: 009d 9e9d 58e8 5ae5 5300 0100 00b6 0100  ....X.Z.S.......
+00007350: 000d 63a1 58e8 5ae5 5300 0100 00b6 0100  ..c.X.Z.S.......
 00007360: 0014 0000 0077 6f72 642f 7765 6253 6574  .....word/webSet
 00007370: 7469 6e67 732e 786d 6c8d d0c1 6ac3 300c  tings.xml...j.0.
 00007380: 00d0 7bbe c2e4 9253 e364 8c31 4292 3218  ..{....S.d.1B.2.
 00007390: 1dbb 9441 b60f 701c 2531 b52d 63b9 cdfa  ...A..p.%1.-c...
 000073a0: f733 5936 18bb f426 21e9 21a9 de7f 1acd  .3Y6...&!.!.....
 000073b0: 2ee0 49a1 6db2 322f 3206 56e2 a0ec d464  ..I.m.2/2.V....d
 000073c0: 1fef 87dd 63c6 2808 3b08 8d16 9aec 0a94  ....c.(.;.......
@@ -1858,15 +1858,15 @@
 00007410: c233 cab3 011b d679 ee41 4711 2dcd cad1  .3.....y.AG.-...
 00007420: 8fb6 dca2 2de8 07e7 5102 51bc c7e8 6fcf  ....-...Q.Q...o.
 00007430: 0865 7f99 f2fe 1f64 94f4 4838 863c 1eb3  .e.....d..H8.<..
 00007440: 6db4 5271 bc2c d6c8 e894 1959 bd4e 16bd  m.Rq.,.....Y.N..
 00007450: e835 3469 84d2 3661 2c7e 5068 8dcb dbf1  .54i..6a,~Ph....
 00007460: 856f f980 470c 9db8 c013 7571 0d0d 07a5  .o..G.....uq....
 00007470: 2116 6bfe e7db 6df2 0550 4b03 0414 0000  !.k...m..PK.....
-00007480: 0008 009d 9e9d 58fb 39a0 7363 0200 00fb  ......X.9.sc....
+00007480: 0008 000d 63a1 58fb 39a0 7363 0200 00fb  ....c.X.9.sc....
 00007490: 0a00 0012 0000 0077 6f72 642f 666f 6e74  .......word/font
 000074a0: 5461 626c 652e 786d 6cdd 96c1 6eda 301c  Table.xml...n.0.
 000074b0: c6ef 7d8a 2897 9c4a 6c93 b514 112a c686  ..}.(..Jl....*..
 000074c0: b4cb 0e1b 7b00 131c b016 db91 ed40 b9d2  ....{........@..
 000074d0: fbce 3b6c 8f30 edb0 49bb f46d 907a ed2b  ..;l.0..I..m.z.+
 000074e0: cc24 0182 0819 7443 4803 2139 ffcf f962  .$....tCH.!9...b
 000074f0: fff4 fd1d 5ab7 772c b226 442a 2ab8 efc0  ....Z.w,.&D**...
@@ -1899,15 +1899,15 @@
 000076a0: bb38 a226 6955 41eb a58d 88d2 c89d 2768  .8.&iUA.......'h
 000076b0: b02c 689d 6e49 d00e 68c8 bf0a da62 fe73  .,h.nI..h....b.s
 000076c0: 31ff b5b8 bf5f ccbf 9f3e 6e4c 0c89 fccf  1...._...>nL....
 000076d0: f226 1249 89ac ca1b 3079 3b90 dd69 f296  .&.I....0y;..i..
 000076e0: 3fb6 5ee0 5460 70e4 c196 f33e 9653 c7ac  ?.^.T`p....>.S..
 000076f0: b0e2 6f05 022f cdb1 efe5 7d89 ce75 fc97  ..o../....}..u..
 00007700: be26 eba7 7a4d ae46 aa7d f11b 504b 0304  .&..zM.F.}..PK..
-00007710: 1400 0000 0800 9d9e 9d58 9441 22b8 c606  .........X.A"...
+00007710: 1400 0000 0800 0d63 a158 9441 22b8 c606  .......c.X.A"...
 00007720: 0000 bb2a 0000 1500 0000 776f 7264 2f74  ...*......word/t
 00007730: 6865 6d65 2f74 6865 6d65 312e 786d 6ced  heme/theme1.xml.
 00007740: 5a4d 6fdb 3618 bef7 5710 bae4 d4fa db75  ZMo.6...W......u
 00007750: 8aba 45ec d8ed d6a6 0d12 b743 8fb4 445b  ..E........C..D[
 00007760: 6c28 5120 e924 be0d ed71 c080 61dd b0c3  l(Q .$...q..a...
 00007770: 0aec b6c3 b0ad 400b ecd2 fd9a 6e1d b60e  ......@.....n...
 00007780: e85f 1829 d98a 2851 72e6 c54d da25 07c7  ._.)..(Qr..M.%..
@@ -2010,29 +2010,29 @@
 00007d90: 670e 69c4 df41 2380 9d43 4322 a4a2 61f6  g.i..A#..CC"..a.
 00007da0: d3a9 ece5 64e7 48b2 d8d0 316b 6d39 d619  ....d.H...1km9..
 00007db0: 87e1 4019 3357 9763 8e59 7499 e5a9 2a66  ..@.3W.c.Yt...*f
 00007dc0: 0edf 242f 6027 0699 238e 6428 240c 1e9d  ..$/`'..#.d($...
 00007dd0: 4562 2f86 b65f b94f 97b4 d102 9f96 57e6  Eb/.._.O......W.
 00007de0: d325 63f0 847c 2a0e 97f0 69ec c5f0 fc9f  .%c..|*...i.....
 00007df0: c95e a5e3 a160 b03b ffe1 992c 0972 8f38  .^...`.;...,.r.8
-00007e00: fdaf 5df8 0750 4b03 0414 0000 0008 009d  ..]..PK.........
-00007e10: 9e9d 589e 803a d7a7 0000 0006 0100 0013  ..X..:..........
+00007e00: fdaf 5df8 0750 4b03 0414 0000 0008 000d  ..]..PK.........
+00007e10: 63a1 589e 803a d7a7 0000 0006 0100 0013  c.X..:..........
 00007e20: 0000 0063 7573 746f 6d58 6d6c 2f69 7465  ...customXml/ite
 00007e30: 6d31 2e78 6d6c ad8c b10a c230 1400 f77e  m1.xml.....0...~
 00007e40: 45c9 92c9 a63a 8814 d352 1027 11a1 0aae  E....:...R.'....
 00007e50: 49fa da06 92bc 92a4 62ff de88 bfe0 7877  I.......b.....xw
 00007e60: 70c7 e66d 4dfe 021f 343a 4eb7 4549 7370  p..mM...4:N.EIsp
 00007e70: 0a7b ed46 4e1f f7f3 e640 f310 85eb 8541  .{.FN....@.....A
 00007e80: 079c ae10 6853 6747 5975 b878 0521 4f03  ....hSgGYu.x.!O.
 00007e90: 172a c9c9 14e3 5c31 16d4 0456 8402 6770  .*....\1...V..gp
 00007ea0: a90d e8ad 8809 fdc8 7018 b482 13aa c582  ........p.......
 00007eb0: 8b6c 5796 7b26 b534 1a47 2fe6 6925 bfd9  .lW.{&.4.G/.i%..
 00007ec0: 7f56 1d18 5011 fa2e ae06 3861 edad 2d9e  .V..P.....8a..-.
 00007ed0: dd25 85af b80a 9b64 7284 d5d9 0750 4b03  .%.....dr....PK.
-00007ee0: 0414 0000 0008 009d 9e9d 583e cae5 d5bd  ..........X>....
+00007ee0: 0414 0000 0008 000d 63a1 583e cae5 d5bd  ........c.X>....
 00007ef0: 0000 0027 0100 001e 0000 0063 7573 746f  ...'.......custo
 00007f00: 6d58 6d6c 2f5f 7265 6c73 2f69 7465 6d31  mXml/_rels/item1
 00007f10: 2e78 6d6c 2e72 656c 738d cfb1 6ac3 3010  .xml.rels...j.0.
 00007f20: 06e0 bd4f 21b4 68aa 6567 28a1 58f6 1202  ...O!.h.eg(.X...
 00007f30: d942 7021 ab90 cfb6 88a5 13ba 4b48 debe  .Bp!........KH..
 00007f40: a253 0319 32de 1dff f773 6d7f 0fab b841  .S..2....sm....A
 00007f50: 268f d1a8 a6aa 9580 e870 f471 36ea 67d8  &........p.q6.g.
@@ -2040,15 +2040,15 @@
 00007f70: 3dc1 6ab9 6468 f189 4441 2219 b930 a76f  =.j.dh..DA"..0.o
 00007f80: adc9 2d10 2c55 9820 96cb 8439 582e 639e  ..-.,U. ...9X.c.
 00007f90: 75b2 ee62 67d0 9bba fed2 f9bf 21bb 2753  u..bg.......!.'S
 00007fa0: 1c46 23f3 616c a418 1e09 deb1 719a bc83  .F#.al......q...
 00007fb0: 1dba 6b80 c82f 2ab4 bb12 6338 87f5 98b1  ..k../*...c8....
 00007fc0: 348a c1e6 19d8 48cf 10fe 564d 554c a9bb  4.....H...VMUL..
 00007fd0: 563f fdd7 fd02 504b 0304 1400 0000 0800  V?....PK........
-00007fe0: 9d9e 9d58 b5bb 4c4d e100 0000 6201 0000  ...X..LM....b...
+00007fe0: 0d63 a158 b5bb 4c4d e100 0000 6201 0000  .c.X..LM....b...
 00007ff0: 1800 0000 6375 7374 6f6d 586d 6c2f 6974  ....customXml/it
 00008000: 656d 5072 6f70 7331 2e78 6d6c 9d90 b16e  emProps1.xml...n
 00008010: 8330 1445 77be c2f2 e2c9 31a0 0468 1488  .0.Ew.....1..h..
 00008020: 4800 296b d54a 5d1d 7880 256c 23db 448d  H.)k.J].x.%l#.D.
 00008030: aafe 7b4d 3a35 63c7 77ae 74ee d53b 1c3f  ..{M:5c.w.t..;.?
 00008040: e584 6e60 acd0 2a27 d126 2408 54ab 3ba1  ..n`..*'.&$.T.;.
 00008050: 869c bcbf 3534 23c8 3aae 3a3e 6905 39b9  ....54#.:.:>i.9.
@@ -2057,15 +2057,15 @@
 00008080: 7a06 e5c3 5e1b c99d 3fcd c074 df8b 162a  z...^...?..t...*
 00008090: dd2e 1294 6371 1826 ac5d bc4b 7ec8 0923  ....cq.&.].K~..#
 000080a0: ef16 5e79 a972 fc55 3771 9a65 5142 eb73  ..^y.r.U7q.eQB.s
 000080b0: d2d0 32d9 eee8 4b98 5634 6de2 5d59 9f4f  ..2...K.V4m.]Y.O
 000080c0: 51b5 2dbf 7111 20b4 4efa ed7c 85de aee4  Q.-.q. .N..|....
 000080d0: 89ad dec5 88ff 0ebc 8aeb 24f4 60f8 3cde  ..........$.`.<.
 000080e0: 317b 34b2 a7ca 07f8 f396 22f8 0150 4b03  1{4......."..PK.
-000080f0: 0414 0000 0008 009d 9e9d 5890 d087 896b  ..........X....k
+000080f0: 0414 0000 0008 000d 63a1 5890 d087 896b  ........c.X....k
 00008100: 0300 0089 1500 0012 0000 0077 6f72 642f  ...........word/
 00008110: 6e75 6d62 6572 696e 672e 786d 6ccd 58dd  numbering.xml.X.
 00008120: 6ee2 3818 bddf a740 9146 5cb5 8993 3404  n.8....@.F\...4.
 00008130: 34b4 a240 565d 8d46 23b5 f300 2618 b0ea  4..@V].F#...&...
 00008140: 9fc8 3130 dcee 4bed 63cd 2bac 9d3f a88a  ..10..K.c.+..?..
 00008150: 334c 1276 cb8d 137f df39 fe7c 4efc 05f8  3L.v.....9.|N...
 00008160: fcf0 8392 de0e 8914 7336 ee83 5ba7 df43  ........s6..[..C
@@ -2115,15 +2115,15 @@
 00008420: 7857 7cdf 1d7d 3ae7 aa8e 76ff be0b 4d46  xW|..}:...v...MF
 00008430: 0c1b 1be1 0e07 0150 5e5c f778 5df1 74b5  .......P^\.x].t.
 00008440: f2e1 3f3a 5d2c 3393 9dfe 6e7a e36c b9af  ..?:],3...nz.l..
 00008450: b0a0 6367 60ae 1916 d4c0 3c33 ecae 06f6  ..cg`.....<3....
 00008460: eec7 f611 e6d7 c0ee ccb0 410d 2c30 c3bc  ..........A.,0..
 00008470: 1ad8 c00c 736b 60a1 1906 6a60 4333 cc39  ....sk`...j`C3.9
 00008480: 85d9 27ff a1de ff0b 504b 0304 1400 0000  ..'.....PK......
-00008490: 0800 9d9e 9d58 a2c8 d667 bd05 0000 8420  .....X...g..... 
+00008490: 0800 0d63 a158 a2c8 d667 bd05 0000 8420  ...c.X...g..... 
 000084a0: 0000 1700 0000 646f 6350 726f 7073 2f74  ......docProps/t
 000084b0: 6875 6d62 6e61 696c 2e6a 7065 67ed 566b  humbnail.jpeg.Vk
 000084c0: 7013 5514 3ebb 7b37 296d cd10 282d 1407  p.U.>.{7)m..(-..
 000084d0: c2bb 32c0 a42d 422b 0236 69da a694 36a4  ..2..-B+.6i...6.
 000084e0: 2daf 7186 4993 4d13 9a26 6177 d396 4e9d  -.q.I.M..&aw..N.
 000084f0: 91fa 00f5 873c 7cff b114 5474 9c71 50d1  .....<|...Tt.qP.
 00008500: 823a 5245 4047 0710 0b14 18c6 226a f135  .:RE@G......"j.5
@@ -2210,79 +2210,79 @@
 00008a10: 8191 f0e3 7275 c38a 16e9 5dab 868f cf5b  ....ru....]....[
 00008a20: 9392 61d9 b079 7bf7 9009 f9ce 7323 eac4  ..a..y{.....s#..
 00008a30: 43a9 9913 67f6 4d3a 4f4b 532a bbb5 c2da  C...g.M:OKS*....
 00008a40: ff53 6503 8525 ea3a 0ee9 1c6e 3823 6784  .Se..%.:...n8#g.
 00008a50: f970 e54a 0e74 b00f a682 061a 68a0 8106  .p.J.t......h...
 00008a60: 1a68 a081 061a 68a0 8106 1a68 a081 061a  .h....h....h....
 00008a70: 68a0 8106 ff33 88f6 c23f 504b 0102 1403  h....3...?PK....
-00008a80: 1400 0000 0800 9d9e 9d58 ad52 a591 9501  .........X.R....
+00008a80: 1400 0000 0800 0d63 a158 ad52 a591 9501  .......c.X.R....
 00008a90: 0000 ca06 0000 1300 0000 0000 0000 0000  ................
 00008aa0: 0000 8001 0000 0000 5b43 6f6e 7465 6e74  ........[Content
 00008ab0: 5f54 7970 6573 5d2e 786d 6c50 4b01 0214  _Types].xmlPK...
-00008ac0: 0314 0000 0008 009d 9e9d 5879 264b 40f8  ..........Xy&K@.
+00008ac0: 0314 0000 0008 000d 63a1 5879 264b 40f8  ........c.Xy&K@.
 00008ad0: 0000 00de 0200 000b 0000 0000 0000 0000  ................
 00008ae0: 0000 0080 01c6 0100 005f 7265 6c73 2f2e  ........._rels/.
 00008af0: 7265 6c73 504b 0102 1403 1400 0000 0800  relsPK..........
-00008b00: 9d9e 9d58 8886 0b53 6901 0000 d102 0000  ...X...Si.......
+00008b00: 0d63 a158 8886 0b53 6901 0000 d102 0000  .c.X...Si.......
 00008b10: 1100 0000 0000 0000 0000 0000 8001 e702  ................
 00008b20: 0000 646f 6350 726f 7073 2f63 6f72 652e  ..docProps/core.
-00008b30: 786d 6c50 4b01 0214 0314 0000 0008 009d  xmlPK...........
-00008b40: 9e9d 58f4 dbdb 17eb 0100 006c 0400 0010  ..X........l....
+00008b30: 786d 6c50 4b01 0214 0314 0000 0008 000d  xmlPK...........
+00008b40: 63a1 58f4 dbdb 17eb 0100 006c 0400 0010  c.X........l....
 00008b50: 0000 0000 0000 0000 0000 0080 017f 0400  ................
 00008b60: 0064 6f63 5072 6f70 732f 6170 702e 786d  .docProps/app.xm
-00008b70: 6c50 4b01 0214 0314 0000 0008 009d 9e9d  lPK.............
+00008b70: 6c50 4b01 0214 0314 0000 0008 000d 63a1  lPK...........c.
 00008b80: 5805 9c75 c415 0200 0042 0600 0011 0000  X..u.....B......
 00008b90: 0000 0000 0000 0000 0080 0198 0600 0077  ...............w
 00008ba0: 6f72 642f 646f 6375 6d65 6e74 2e78 6d6c  ord/document.xml
-00008bb0: 504b 0102 1403 1400 0000 0800 9d9e 9d58  PK.............X
+00008bb0: 504b 0102 1403 1400 0000 0800 0d63 a158  PK...........c.X
 00008bc0: 6e80 1b12 3201 0000 cb04 0000 1c00 0000  n...2...........
 00008bd0: 0000 0000 0000 0000 8001 dc08 0000 776f  ..............wo
 00008be0: 7264 2f5f 7265 6c73 2f64 6f63 756d 656e  rd/_rels/documen
 00008bf0: 742e 786d 6c2e 7265 6c73 504b 0102 1403  t.xml.relsPK....
-00008c00: 1400 0000 0800 9d9e 9d58 07d4 af99 732f  .........X....s/
+00008c00: 1400 0000 0800 0d63 a158 07d4 af99 732f  .......c.X....s/
 00008c10: 0000 1255 0500 0f00 0000 0000 0000 0000  ...U............
 00008c20: 0000 8001 480a 0000 776f 7264 2f73 7479  ....H...word/sty
 00008c30: 6c65 732e 786d 6c50 4b01 0214 0314 0000  les.xmlPK.......
-00008c40: 0008 009d 9e9d 5860 7982 d339 3500 0073  ......X`y..95..s
+00008c40: 0008 000d 63a1 5860 7982 d339 3500 0073  ....c.X`y..95..s
 00008c50: af06 001a 0000 0000 0000 0000 0000 0080  ................
 00008c60: 01e8 3900 0077 6f72 642f 7374 796c 6573  ..9..word/styles
 00008c70: 5769 7468 4566 6665 6374 732e 786d 6c50  WithEffects.xmlP
-00008c80: 4b01 0214 0314 0000 0008 009d 9e9d 58a3  K.............X.
+00008c80: 4b01 0214 0314 0000 0008 000d 63a1 58a3  K...........c.X.
 00008c90: 3f46 5fbf 0300 00e7 0900 0011 0000 0000  ?F_.............
 00008ca0: 0000 0000 0000 0080 0159 6f00 0077 6f72  .........Yo..wor
 00008cb0: 642f 7365 7474 696e 6773 2e78 6d6c 504b  d/settings.xmlPK
-00008cc0: 0102 1403 1400 0000 0800 9d9e 9d58 e85a  .............X.Z
+00008cc0: 0102 1403 1400 0000 0800 0d63 a158 e85a  ...........c.X.Z
 00008cd0: e553 0001 0000 b601 0000 1400 0000 0000  .S..............
 00008ce0: 0000 0000 0000 8001 4773 0000 776f 7264  ........Gs..word
 00008cf0: 2f77 6562 5365 7474 696e 6773 2e78 6d6c  /webSettings.xml
-00008d00: 504b 0102 1403 1400 0000 0800 9d9e 9d58  PK.............X
+00008d00: 504b 0102 1403 1400 0000 0800 0d63 a158  PK...........c.X
 00008d10: fb39 a073 6302 0000 fb0a 0000 1200 0000  .9.sc...........
 00008d20: 0000 0000 0000 0000 8001 7974 0000 776f  ..........yt..wo
 00008d30: 7264 2f66 6f6e 7454 6162 6c65 2e78 6d6c  rd/fontTable.xml
-00008d40: 504b 0102 1403 1400 0000 0800 9d9e 9d58  PK.............X
+00008d40: 504b 0102 1403 1400 0000 0800 0d63 a158  PK...........c.X
 00008d50: 9441 22b8 c606 0000 bb2a 0000 1500 0000  .A"......*......
 00008d60: 0000 0000 0000 0000 8001 0c77 0000 776f  ...........w..wo
 00008d70: 7264 2f74 6865 6d65 2f74 6865 6d65 312e  rd/theme/theme1.
-00008d80: 786d 6c50 4b01 0214 0314 0000 0008 009d  xmlPK...........
-00008d90: 9e9d 589e 803a d7a7 0000 0006 0100 0013  ..X..:..........
+00008d80: 786d 6c50 4b01 0214 0314 0000 0008 000d  xmlPK...........
+00008d90: 63a1 589e 803a d7a7 0000 0006 0100 0013  c.X..:..........
 00008da0: 0000 0000 0000 0000 0000 0080 0105 7e00  ..............~.
 00008db0: 0063 7573 746f 6d58 6d6c 2f69 7465 6d31  .customXml/item1
 00008dc0: 2e78 6d6c 504b 0102 1403 1400 0000 0800  .xmlPK..........
-00008dd0: 9d9e 9d58 3eca e5d5 bd00 0000 2701 0000  ...X>.......'...
+00008dd0: 0d63 a158 3eca e5d5 bd00 0000 2701 0000  .c.X>.......'...
 00008de0: 1e00 0000 0000 0000 0000 0000 8001 dd7e  ...............~
 00008df0: 0000 6375 7374 6f6d 586d 6c2f 5f72 656c  ..customXml/_rel
 00008e00: 732f 6974 656d 312e 786d 6c2e 7265 6c73  s/item1.xml.rels
-00008e10: 504b 0102 1403 1400 0000 0800 9d9e 9d58  PK.............X
+00008e10: 504b 0102 1403 1400 0000 0800 0d63 a158  PK...........c.X
 00008e20: b5bb 4c4d e100 0000 6201 0000 1800 0000  ..LM....b.......
 00008e30: 0000 0000 0000 0000 8001 d67f 0000 6375  ..............cu
 00008e40: 7374 6f6d 586d 6c2f 6974 656d 5072 6f70  stomXml/itemProp
 00008e50: 7331 2e78 6d6c 504b 0102 1403 1400 0000  s1.xmlPK........
-00008e60: 0800 9d9e 9d58 90d0 8789 6b03 0000 8915  .....X....k.....
+00008e60: 0800 0d63 a158 90d0 8789 6b03 0000 8915  ...c.X....k.....
 00008e70: 0000 1200 0000 0000 0000 0000 0000 8001  ................
 00008e80: ed80 0000 776f 7264 2f6e 756d 6265 7269  ....word/numberi
 00008e90: 6e67 2e78 6d6c 504b 0102 1403 1400 0000  ng.xmlPK........
-00008ea0: 0800 9d9e 9d58 a2c8 d667 bd05 0000 8420  .....X...g..... 
+00008ea0: 0800 0d63 a158 a2c8 d667 bd05 0000 8420  ...c.X...g..... 
 00008eb0: 0000 1700 0000 0000 0000 0000 0000 8001  ................
 00008ec0: 8884 0000 646f 6350 726f 7073 2f74 6875  ....docProps/thu
 00008ed0: 6d62 6e61 696c 2e6a 7065 6750 4b05 0600  mbnail.jpegPK...
 00008ee0: 0000 0011 0011 0061 0400 007a 8a00 0000  .......a...z....
 00008ef0: 00                                       .
```

### Comparing `python_docx-1.1.1/features/blk-iter-inner-content.feature` & `python_docx-1.1.2/features/blk-iter-inner-content.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/doc-access-collections.feature` & `python_docx-1.1.2/features/doc-access-collections.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/doc-add-heading.feature` & `python_docx-1.1.2/features/doc-add-heading.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/doc-add-paragraph.feature` & `python_docx-1.1.2/features/doc-add-paragraph.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/doc-add-picture.feature` & `python_docx-1.1.2/features/doc-add-picture.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/doc-add-section.feature` & `python_docx-1.1.2/features/doc-add-section.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/doc-add-table.feature` & `python_docx-1.1.2/features/doc-add-table.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/doc-coreprops.feature` & `python_docx-1.1.2/features/doc-coreprops.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/doc-settings.feature` & `python_docx-1.1.2/features/doc-settings.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/doc-styles.feature` & `python_docx-1.1.2/features/doc-styles.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/hdr-header-footer.feature` & `python_docx-1.1.2/features/hdr-header-footer.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/hlk-props.feature` & `python_docx-1.1.2/features/hlk-props.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/img-characterize-image.feature` & `python_docx-1.1.2/features/img-characterize-image.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/par-access-inner-content.feature` & `python_docx-1.1.2/features/par-access-inner-content.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/par-add-run.feature` & `python_docx-1.1.2/features/par-add-run.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/par-alignment-prop.feature` & `python_docx-1.1.2/features/par-alignment-prop.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/par-insert-paragraph.feature` & `python_docx-1.1.2/features/par-insert-paragraph.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/par-style-prop.feature` & `python_docx-1.1.2/features/par-style-prop.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/pbk-split-para.feature` & `python_docx-1.1.2/features/pbk-split-para.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/run-access-inner-content.feature` & `python_docx-1.1.2/features/run-access-inner-content.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/run-add-picture.feature` & `python_docx-1.1.2/features/run-add-picture.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/run-char-style.feature` & `python_docx-1.1.2/features/run-char-style.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/run-enum-props.feature` & `python_docx-1.1.2/features/run-enum-props.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/sct-section.feature` & `python_docx-1.1.2/features/sct-section.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/shp-inline-shape-access.feature` & `python_docx-1.1.2/features/shp-inline-shape-access.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/shp-inline-shape-size.feature` & `python_docx-1.1.2/features/shp-inline-shape-size.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/api.py` & `python_docx-1.1.2/features/steps/api.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/block.py` & `python_docx-1.1.2/features/steps/block.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/coreprops.py` & `python_docx-1.1.2/features/steps/coreprops.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,100 +1,101 @@
 """Gherkin step implementations for core properties-related features."""
 
-from datetime import datetime, timedelta
+import datetime as dt
 
 from behave import given, then, when
+from behave.runner import Context
 
 from docx import Document
 from docx.opc.coreprops import CoreProperties
 
 from helpers import test_docx
 
 # given ===================================================
 
 
 @given("a document having known core properties")
-def given_a_document_having_known_core_properties(context):
+def given_a_document_having_known_core_properties(context: Context):
     context.document = Document(test_docx("doc-coreprops"))
 
 
 @given("a document having no core properties part")
-def given_a_document_having_no_core_properties_part(context):
+def given_a_document_having_no_core_properties_part(context: Context):
     context.document = Document(test_docx("doc-no-coreprops"))
 
 
 # when ====================================================
 
 
 @when("I access the core properties object")
-def when_I_access_the_core_properties_object(context):
+def when_I_access_the_core_properties_object(context: Context):
     context.document.core_properties
 
 
 @when("I assign new values to the properties")
-def when_I_assign_new_values_to_the_properties(context):
+def when_I_assign_new_values_to_the_properties(context: Context):
     context.propvals = (
         ("author", "Creator"),
         ("category", "Category"),
         ("comments", "Description"),
         ("content_status", "Content Status"),
-        ("created", datetime(2013, 6, 15, 12, 34, 56)),
+        ("created", dt.datetime(2013, 6, 15, 12, 34, 56, tzinfo=dt.timezone.utc)),
         ("identifier", "Identifier"),
         ("keywords", "key; word; keyword"),
         ("language", "Language"),
         ("last_modified_by", "Last Modified By"),
-        ("last_printed", datetime(2013, 6, 15, 12, 34, 56)),
-        ("modified", datetime(2013, 6, 15, 12, 34, 56)),
+        ("last_printed", dt.datetime(2013, 6, 15, 12, 34, 56, tzinfo=dt.timezone.utc)),
+        ("modified", dt.datetime(2013, 6, 15, 12, 34, 56, tzinfo=dt.timezone.utc)),
         ("revision", 9),
         ("subject", "Subject"),
         ("title", "Title"),
         ("version", "Version"),
     )
     core_properties = context.document.core_properties
     for name, value in context.propvals:
         setattr(core_properties, name, value)
 
 
 # then ====================================================
 
 
 @then("a core properties part with default values is added")
-def then_a_core_properties_part_with_default_values_is_added(context):
+def then_a_core_properties_part_with_default_values_is_added(context: Context):
     core_properties = context.document.core_properties
     assert core_properties.title == "Word Document"
     assert core_properties.last_modified_by == "python-docx"
     assert core_properties.revision == 1
     # core_properties.modified only stores time with seconds resolution, so
     # comparison needs to be a little loose (within two seconds)
-    modified_timedelta = datetime.utcnow() - core_properties.modified
-    max_expected_timedelta = timedelta(seconds=2)
+    modified_timedelta = dt.datetime.now(dt.timezone.utc) - core_properties.modified
+    max_expected_timedelta = dt.timedelta(seconds=2)
     assert modified_timedelta < max_expected_timedelta
 
 
 @then("I can access the core properties object")
-def then_I_can_access_the_core_properties_object(context):
+def then_I_can_access_the_core_properties_object(context: Context):
     document = context.document
     core_properties = document.core_properties
     assert isinstance(core_properties, CoreProperties)
 
 
 @then("the core property values match the known values")
-def then_the_core_property_values_match_the_known_values(context):
+def then_the_core_property_values_match_the_known_values(context: Context):
     known_propvals = (
         ("author", "Steve Canny"),
         ("category", "Category"),
         ("comments", "Description"),
         ("content_status", "Content Status"),
-        ("created", datetime(2014, 12, 13, 22, 2, 0)),
+        ("created", dt.datetime(2014, 12, 13, 22, 2, 0, tzinfo=dt.timezone.utc)),
         ("identifier", "Identifier"),
         ("keywords", "key; word; keyword"),
         ("language", "Language"),
         ("last_modified_by", "Steve Canny"),
-        ("last_printed", datetime(2014, 12, 13, 22, 2, 42)),
-        ("modified", datetime(2014, 12, 13, 22, 6, 0)),
+        ("last_printed", dt.datetime(2014, 12, 13, 22, 2, 42, tzinfo=dt.timezone.utc)),
+        ("modified", dt.datetime(2014, 12, 13, 22, 6, 0, tzinfo=dt.timezone.utc)),
         ("revision", 2),
         ("subject", "Subject"),
         ("title", "Title"),
         ("version", "0.7.1a3"),
     )
     core_properties = context.document.core_properties
     for name, expected_value in known_propvals:
@@ -102,15 +103,15 @@
         assert value == expected_value, "got '%s' for core property '%s'" % (
             value,
             name,
         )
 
 
 @then("the core property values match the new values")
-def then_the_core_property_values_match_the_new_values(context):
+def then_the_core_property_values_match_the_new_values(context: Context):
     core_properties = context.document.core_properties
     for name, expected_value in context.propvals:
         value = getattr(core_properties, name)
         assert value == expected_value, "got '%s' for core property '%s'" % (
             value,
             name,
         )
```

### Comparing `python_docx-1.1.1/features/steps/document.py` & `python_docx-1.1.2/features/steps/document.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/font.py` & `python_docx-1.1.2/features/steps/font.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/hdrftr.py` & `python_docx-1.1.2/features/steps/hdrftr.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/helpers.py` & `python_docx-1.1.2/features/steps/helpers.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/hyperlink.py` & `python_docx-1.1.2/features/steps/hyperlink.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/image.py` & `python_docx-1.1.2/features/steps/image.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/numbering.py` & `python_docx-1.1.2/features/steps/numbering.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/pagebreak.py` & `python_docx-1.1.2/features/steps/pagebreak.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/paragraph.py` & `python_docx-1.1.2/features/steps/paragraph.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/parfmt.py` & `python_docx-1.1.2/features/steps/parfmt.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/section.py` & `python_docx-1.1.2/features/steps/section.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/settings.py` & `python_docx-1.1.2/features/steps/settings.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/shape.py` & `python_docx-1.1.2/features/steps/shape.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/shared.py` & `python_docx-1.1.2/features/steps/shared.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/styles.py` & `python_docx-1.1.2/features/steps/styles.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/table.py` & `python_docx-1.1.2/features/steps/table.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/tabstops.py` & `python_docx-1.1.2/features/steps/tabstops.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/blk-containing-table.docx` & `python_docx-1.1.2/features/steps/test_files/blk-containing-table.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/blk-paras-and-tables.docx` & `python_docx-1.1.2/features/steps/test_files/blk-paras-and-tables.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/court-exif.jpg` & `python_docx-1.1.2/features/steps/test_files/court-exif.jpg`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/doc-access-sections.docx` & `python_docx-1.1.2/features/steps/test_files/doc-access-sections.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/doc-add-section.docx` & `python_docx-1.1.2/features/steps/test_files/doc-add-section.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/doc-coreprops.docx` & `python_docx-1.1.2/features/steps/test_files/doc-coreprops.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/doc-default.docx` & `python_docx-1.1.2/features/steps/test_files/doc-default.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/doc-no-coreprops.docx` & `python_docx-1.1.2/features/steps/test_files/doc-no-coreprops.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/doc-odd-even-hdrs.docx` & `python_docx-1.1.2/features/steps/test_files/doc-odd-even-hdrs.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/doc-word-default-blank.docx` & `python_docx-1.1.2/features/steps/test_files/doc-word-default-blank.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/fnt-color.docx` & `python_docx-1.1.2/features/steps/test_files/fnt-color.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/hdr-header-footer.docx` & `python_docx-1.1.2/features/steps/test_files/hdr-header-footer.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/jfif-300-dpi.jpg` & `python_docx-1.1.2/features/steps/test_files/jfif-300-dpi.jpg`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/jpeg420exif.jpg` & `python_docx-1.1.2/features/steps/test_files/jpeg420exif.jpg`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/lena.bmp` & `python_docx-1.1.2/features/steps/test_files/lena.bmp`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/lena.gif` & `python_docx-1.1.2/features/steps/test_files/lena.gif`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/lena.tif` & `python_docx-1.1.2/features/steps/test_files/lena.tif`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/lena_std.jpg` & `python_docx-1.1.2/features/steps/test_files/lena_std.jpg`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/monty-truth.png` & `python_docx-1.1.2/features/steps/test_files/monty-truth.png`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/mountain.bmp` & `python_docx-1.1.2/features/steps/test_files/mountain.bmp`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/num-having-numbering-part.docx` & `python_docx-1.1.2/features/steps/test_files/num-having-numbering-part.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/par-alignment.docx` & `python_docx-1.1.2/features/steps/test_files/par-alignment.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/par-hlink-frags.docx` & `python_docx-1.1.2/features/steps/test_files/par-hlink-frags.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/par-hyperlinks.docx` & `python_docx-1.1.2/features/steps/test_files/par-hyperlinks.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/par-known-paragraphs.docx` & `python_docx-1.1.2/features/steps/test_files/par-known-paragraphs.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/par-known-styles.docx` & `python_docx-1.1.2/features/steps/test_files/par-known-styles.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/par-rendered-page-breaks.docx` & `python_docx-1.1.2/features/steps/test_files/par-rendered-page-breaks.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/python-icon.jpeg` & `python_docx-1.1.2/features/steps/test_files/python-icon.jpeg`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/run-char-style.docx` & `python_docx-1.1.2/features/steps/test_files/run-char-style.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/run-enumerated-props.docx` & `python_docx-1.1.2/features/steps/test_files/run-enumerated-props.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/sample.tif` & `python_docx-1.1.2/features/steps/test_files/sample.tif`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/sct-first-page-hdrftr.docx` & `python_docx-1.1.2/features/steps/test_files/sct-first-page-hdrftr.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/sct-inner-content.docx` & `python_docx-1.1.2/features/steps/test_files/sct-inner-content.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/sct-section-props.docx` & `python_docx-1.1.2/features/steps/test_files/sct-section-props.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/set-no-settings-part.docx` & `python_docx-1.1.2/features/steps/test_files/set-no-settings-part.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/shp-inline-shape-access.docx` & `python_docx-1.1.2/features/steps/test_files/shp-inline-shape-access.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/sty-behav-props.docx` & `python_docx-1.1.2/features/steps/test_files/sty-behav-props.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/sty-having-no-styles-part.docx` & `python_docx-1.1.2/features/steps/test_files/sty-having-no-styles-part.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/sty-having-styles-part.docx` & `python_docx-1.1.2/features/steps/test_files/sty-having-styles-part.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/sty-known-styles.docx` & `python_docx-1.1.2/features/steps/test_files/sty-known-styles.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/tab-stops.docx` & `python_docx-1.1.2/features/steps/test_files/tab-stops.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/tbl-2x2-table.docx` & `python_docx-1.1.2/features/steps/test_files/tbl-2x2-table.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/tbl-cell-access.docx` & `python_docx-1.1.2/features/steps/test_files/tbl-cell-access.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/tbl-cell-props.docx` & `python_docx-1.1.2/features/steps/test_files/tbl-cell-props.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/tbl-col-props.docx` & `python_docx-1.1.2/features/steps/test_files/tbl-col-props.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/tbl-having-applied-style.docx` & `python_docx-1.1.2/features/steps/test_files/tbl-having-applied-style.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/tbl-having-tables.docx` & `python_docx-1.1.2/features/steps/test_files/tbl-having-tables.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/tbl-on-off-props.docx` & `python_docx-1.1.2/features/steps/test_files/tbl-on-off-props.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/tbl-props.docx` & `python_docx-1.1.2/features/steps/test_files/tbl-props.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/test.png` & `python_docx-1.1.2/features/steps/test_files/test.png`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/txt-font-highlight-color.docx` & `python_docx-1.1.2/features/steps/test_files/txt-font-highlight-color.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/test_files/txt-font-props.docx` & `python_docx-1.1.2/features/steps/test_files/txt-font-props.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/steps/text.py` & `python_docx-1.1.2/features/steps/text.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/sty-access-latent-styles.feature` & `python_docx-1.1.2/features/sty-access-latent-styles.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/sty-add-style.feature` & `python_docx-1.1.2/features/sty-add-style.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/sty-latent-add-del.feature` & `python_docx-1.1.2/features/sty-latent-add-del.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/sty-latent-props.feature` & `python_docx-1.1.2/features/sty-latent-props.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/sty-style-props.feature` & `python_docx-1.1.2/features/sty-style-props.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/tab-access-tabs.feature` & `python_docx-1.1.2/features/tab-access-tabs.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/tab-tabstop-props.feature` & `python_docx-1.1.2/features/tab-tabstop-props.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/tbl-add-row-or-col.feature` & `python_docx-1.1.2/features/tbl-add-row-or-col.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/tbl-cell-access.feature` & `python_docx-1.1.2/features/tbl-cell-access.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/tbl-cell-props.feature` & `python_docx-1.1.2/features/tbl-cell-props.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/tbl-col-props.feature` & `python_docx-1.1.2/features/tbl-col-props.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/tbl-item-access.feature` & `python_docx-1.1.2/features/tbl-item-access.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/tbl-merge-cells.feature` & `python_docx-1.1.2/features/tbl-merge-cells.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/tbl-props.feature` & `python_docx-1.1.2/features/tbl-props.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/tbl-row-props.feature` & `python_docx-1.1.2/features/tbl-row-props.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/tbl-style.feature` & `python_docx-1.1.2/features/tbl-style.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/txt-add-break.feature` & `python_docx-1.1.2/features/txt-add-break.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/txt-font-color.feature` & `python_docx-1.1.2/features/txt-font-color.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/txt-font-props.feature` & `python_docx-1.1.2/features/txt-font-props.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/features/txt-parfmt-props.feature` & `python_docx-1.1.2/features/txt-parfmt-props.feature`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/pyproject.toml` & `python_docx-1.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Office/Business :: Office Suites",
     "Topic :: Software Development :: Libraries",
 ]
 dependencies = [
-    "lxml>=3.1.0,<=4.9.2",
+    "lxml>=3.1.0",
     "typing_extensions>=4.9.0",
 ]
 description = "Create, read, and update Microsoft Word .docx files."
 dynamic = ["version"]
 keywords = ["docx", "office", "openxml", "word"]
 license = { text = "MIT" }
 readme = "README.md"
@@ -38,14 +38,25 @@
 Homepage = "https://github.com/python-openxml/python-docx"
 Repository = "https://github.com/python-openxml/python-docx"
 
 [tool.black]
 line-length = 100
 target-version = ["py37", "py38", "py39", "py310", "py311"]
 
+[tool.pyright]
+include = ["src/docx", "tests"]
+pythonPlatform = "All"
+pythonVersion = "3.8"
+reportImportCycles = true
+reportUnnecessaryCast = true
+reportUnnecessaryTypeIgnoreComment = true
+stubPath = "./typings"
+typeCheckingMode = "strict"
+verboseOutput = true
+
 [tool.pytest.ini_options]
 filterwarnings = [
     # -- exit on any warning not explicitly ignored here --
     "error",
 
     # -- pytest-xdist plugin may warn about `looponfailroots` deprecation --
     "ignore::DeprecationWarning:xdist",
```

### Comparing `python_docx-1.1.1/src/docx/__init__.py` & `python_docx-1.1.2/src/docx/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from typing import TYPE_CHECKING, Type
 
 from docx.api import Document
 
 if TYPE_CHECKING:
     from docx.opc.part import Part
 
-__version__ = "1.1.1"
+__version__ = "1.1.2"
 
 
 __all__ = ["Document"]
 
 
 # -- register custom Part classes with opc package reader --
```

### Comparing `python_docx-1.1.1/src/docx/api.py` & `python_docx-1.1.2/src/docx/api.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/blkcntnr.py` & `python_docx-1.1.2/src/docx/blkcntnr.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/dml/color.py` & `python_docx-1.1.2/src/docx/dml/color.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/document.py` & `python_docx-1.1.2/src/docx/document.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/enum/base.py` & `python_docx-1.1.2/src/docx/enum/base.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/enum/dml.py` & `python_docx-1.1.2/src/docx/enum/dml.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/enum/section.py` & `python_docx-1.1.2/src/docx/enum/section.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/enum/style.py` & `python_docx-1.1.2/src/docx/enum/style.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/enum/table.py` & `python_docx-1.1.2/src/docx/enum/table.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/enum/text.py` & `python_docx-1.1.2/src/docx/enum/text.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/image/__init__.py` & `python_docx-1.1.2/src/docx/image/__init__.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/image/bmp.py` & `python_docx-1.1.2/src/docx/image/bmp.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/image/constants.py` & `python_docx-1.1.2/src/docx/image/constants.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/image/gif.py` & `python_docx-1.1.2/src/docx/image/gif.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/image/helpers.py` & `python_docx-1.1.2/src/docx/image/helpers.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/image/image.py` & `python_docx-1.1.2/src/docx/image/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     @property
     def height(self) -> Inches:
         """A |Length| value representing the native height of the image, calculated from
         the values of `px_height` and `vert_dpi`."""
         return Inches(self.px_height / self.vert_dpi)
 
     def scaled_dimensions(
-        self, width: int | None = None, height: int | None = None
+        self, width: int | Length | None = None, height: int | Length | None = None
     ) -> Tuple[Length, Length]:
         """(cx, cy) pair representing scaled dimensions of this image.
 
         The native dimensions of the image are scaled by applying the following rules to
         the `width` and `height` arguments.
 
         * If both `width` and `height` are specified, the return value is (`width`,
```

### Comparing `python_docx-1.1.1/src/docx/image/jpeg.py` & `python_docx-1.1.2/src/docx/image/jpeg.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/image/png.py` & `python_docx-1.1.2/src/docx/image/png.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/image/tiff.py` & `python_docx-1.1.2/src/docx/image/tiff.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/opc/constants.py` & `python_docx-1.1.2/src/docx/opc/constants.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/opc/oxml.py` & `python_docx-1.1.2/src/docx/opc/oxml.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 """Temporary stand-in for main oxml module.
 
 This module came across with the PackageReader transplant. Probably much will get
 replaced with objects from the pptx.oxml.core and then this module will either get
 deleted or only hold the package related custom element classes.
 """
 
+from __future__ import annotations
+
+from typing import cast
+
 from lxml import etree
 
 from docx.opc.constants import NAMESPACE as NS
 from docx.opc.constants import RELATIONSHIP_TARGET_MODE as RTM
 
 # configure XML parser
 element_class_lookup = etree.ElementNamespaceClassLookup()
@@ -134,15 +138,15 @@
 
 
 class CT_Relationship(BaseOxmlElement):
     """``<Relationship>`` element, representing a single relationship from a source to a
     target part."""
 
     @staticmethod
-    def new(rId, reltype, target, target_mode=RTM.INTERNAL):
+    def new(rId: str, reltype: str, target: str, target_mode: str = RTM.INTERNAL):
         """Return a new ``<Relationship>`` element."""
         xml = '<Relationship xmlns="%s"/>' % nsmap["pr"]
         relationship = parse_xml(xml)
         relationship.set("Id", rId)
         relationship.set("Type", reltype)
         relationship.set("Target", target)
         if target_mode == RTM.EXTERNAL:
@@ -174,27 +178,26 @@
         """
         return self.get("TargetMode", RTM.INTERNAL)
 
 
 class CT_Relationships(BaseOxmlElement):
     """``<Relationships>`` element, the root element in a .rels file."""
 
-    def add_rel(self, rId, reltype, target, is_external=False):
+    def add_rel(self, rId: str, reltype: str, target: str, is_external: bool = False):
         """Add a child ``<Relationship>`` element with attributes set according to
         parameter values."""
         target_mode = RTM.EXTERNAL if is_external else RTM.INTERNAL
         relationship = CT_Relationship.new(rId, reltype, target, target_mode)
         self.append(relationship)
 
     @staticmethod
-    def new():
+    def new() -> CT_Relationships:
         """Return a new ``<Relationships>`` element."""
         xml = '<Relationships xmlns="%s"/>' % nsmap["pr"]
-        relationships = parse_xml(xml)
-        return relationships
+        return cast(CT_Relationships, parse_xml(xml))
 
     @property
     def Relationship_lst(self):
         """Return a list containing all the ``<Relationship>`` child elements."""
         return self.findall(qn("pr:Relationship"))
 
     @property
```

### Comparing `python_docx-1.1.1/src/docx/opc/package.py` & `python_docx-1.1.2/src/docx/opc/package.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """Objects that implement reading and writing OPC packages."""
 
 from __future__ import annotations
 
-from typing import IO, TYPE_CHECKING, Iterator
+from typing import IO, TYPE_CHECKING, Iterator, cast
 
 from docx.opc.constants import RELATIONSHIP_TYPE as RT
 from docx.opc.packuri import PACKAGE_URI, PackURI
 from docx.opc.part import PartFactory
 from docx.opc.parts.coreprops import CorePropertiesPart
 from docx.opc.pkgreader import PackageReader
 from docx.opc.pkgwriter import PackageWriter
 from docx.opc.rel import Relationships
 from docx.shared import lazyproperty
 
 if TYPE_CHECKING:
+    from docx.opc.coreprops import CoreProperties
     from docx.opc.part import Part
+    from docx.opc.rel import _Relationship  # pyright: ignore[reportPrivateUsage]
 
 
 class OpcPackage:
     """Main API class for |python-opc|.
 
     A new instance is constructed by calling the :meth:`open` class method with a path
     to a package file or file-like object containing one.
@@ -33,24 +35,26 @@
         May be overridden by subclasses without forwarding call to super.
         """
         # don't place any code here, just catch call if not overridden by
         # subclass
         pass
 
     @property
-    def core_properties(self):
+    def core_properties(self) -> CoreProperties:
         """|CoreProperties| object providing read/write access to the Dublin Core
         properties for this document."""
         return self._core_properties_part.core_properties
 
-    def iter_rels(self):
+    def iter_rels(self) -> Iterator[_Relationship]:
         """Generate exactly one reference to each relationship in the package by
         performing a depth-first traversal of the rels graph."""
 
-        def walk_rels(source, visited=None):
+        def walk_rels(
+            source: OpcPackage | Part, visited: list[Part] | None = None
+        ) -> Iterator[_Relationship]:
             visited = [] if visited is None else visited
             for rel in source.rels.values():
                 yield rel
                 if rel.is_external:
                     continue
                 part = rel.target_part
                 if part in visited:
@@ -99,15 +103,15 @@
 
         Examples include a document part for a WordprocessingML package, a presentation
         part for a PresentationML package, or a workbook part for a SpreadsheetML
         package.
         """
         return self.part_related_by(RT.OFFICE_DOCUMENT)
 
-    def next_partname(self, template):
+    def next_partname(self, template: str) -> PackURI:
         """Return a |PackURI| instance representing partname matching `template`.
 
         The returned part-name has the next available numeric suffix to distinguish it
         from other parts of its type. `template` is a printf (%)-style template string
         containing a single replacement item, a '%d' to be used to insert the integer
         portion of the partname. Example: "/word/header%d.xml"
         """
@@ -159,21 +163,21 @@
         `pkg_file` can be either a file-path or a file-like object.
         """
         for part in self.parts:
             part.before_marshal()
         PackageWriter.write(pkg_file, self.rels, self.parts)
 
     @property
-    def _core_properties_part(self):
+    def _core_properties_part(self) -> CorePropertiesPart:
         """|CorePropertiesPart| object related to this package.
 
         Creates a default core properties part if one is not present (not common).
         """
         try:
-            return self.part_related_by(RT.CORE_PROPERTIES)
+            return cast(CorePropertiesPart, self.part_related_by(RT.CORE_PROPERTIES))
         except KeyError:
             core_properties_part = CorePropertiesPart.default(self)
             self.relate_to(core_properties_part, RT.CORE_PROPERTIES)
             return core_properties_part
 
 
 class Unmarshaller:
```

### Comparing `python_docx-1.1.1/src/docx/opc/packuri.py` & `python_docx-1.1.2/src/docx/opc/packuri.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 """Provides the PackURI value type.
 
 Also some useful known pack URI strings such as PACKAGE_URI.
 """
 
+from __future__ import annotations
+
 import posixpath
 import re
 
 
 class PackURI(str):
     """Provides access to pack URI components such as the baseURI and the filename
     slice.
 
     Behaves as |str| otherwise.
     """
 
     _filename_re = re.compile("([a-zA-Z]+)([1-9][0-9]*)?")
 
-    def __new__(cls, pack_uri_str):
+    def __new__(cls, pack_uri_str: str):
         if pack_uri_str[0] != "/":
             tmpl = "PackURI must begin with slash, got '%s'"
             raise ValueError(tmpl % pack_uri_str)
         return str.__new__(cls, pack_uri_str)
 
     @staticmethod
-    def from_rel_ref(baseURI, relative_ref):
-        """Return a |PackURI| instance containing the absolute pack URI formed by
-        translating `relative_ref` onto `baseURI`."""
+    def from_rel_ref(baseURI: str, relative_ref: str) -> PackURI:
+        """The absolute PackURI formed by translating `relative_ref` onto `baseURI`."""
         joined_uri = posixpath.join(baseURI, relative_ref)
         abs_uri = posixpath.abspath(joined_uri)
         return PackURI(abs_uri)
 
     @property
-    def baseURI(self):
+    def baseURI(self) -> str:
         """The base URI of this pack URI, the directory portion, roughly speaking.
 
         E.g. ``'/ppt/slides'`` for ``'/ppt/slides/slide1.xml'``. For the package pseudo-
         partname '/', baseURI is '/'.
         """
         return posixpath.split(self)[0]
 
     @property
-    def ext(self):
-        """The extension portion of this pack URI, e.g. ``'xml'`` for
-        ``'/word/document.xml'``.
+    def ext(self) -> str:
+        """The extension portion of this pack URI, e.g. ``'xml'`` for ``'/word/document.xml'``.
 
         Note the period is not included.
         """
         # raw_ext is either empty string or starts with period, e.g. '.xml'
         raw_ext = posixpath.splitext(self)[1]
         return raw_ext[1:] if raw_ext.startswith(".") else raw_ext
 
@@ -80,15 +80,15 @@
         """The pack URI with the leading slash stripped off, the form used as the Zip
         file membername for the package item.
 
         Returns '' for the package pseudo-partname '/'.
         """
         return self[1:]
 
-    def relative_ref(self, baseURI):
+    def relative_ref(self, baseURI: str):
         """Return string containing relative reference to package item from `baseURI`.
 
         E.g. PackURI('/ppt/slideLayouts/slideLayout1.xml') would return
         '../slideLayouts/slideLayout1.xml' for baseURI '/ppt/slides'.
         """
         # workaround for posixpath bug in 2.6, doesn't generate correct
         # relative path when `start` (second) parameter is root ('/')
```

### Comparing `python_docx-1.1.1/src/docx/opc/part.py` & `python_docx-1.1.2/src/docx/opc/part.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,37 @@
+# pyright: reportImportCycles=false
+
 """Open Packaging Convention (OPC) objects related to package parts."""
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Callable, Dict, Type
+from typing import TYPE_CHECKING, Callable, Type, cast
 
 from docx.opc.oxml import serialize_part_xml
 from docx.opc.packuri import PackURI
 from docx.opc.rel import Relationships
 from docx.opc.shared import cls_method_fn
 from docx.oxml.parser import parse_xml
 from docx.shared import lazyproperty
 
 if TYPE_CHECKING:
+    from docx.oxml.xmlchemy import BaseOxmlElement
     from docx.package import Package
 
 
 class Part:
     """Base class for package parts.
 
     Provides common properties and methods, but intended to be subclassed in client code
     to implement specific part behaviors.
     """
 
     def __init__(
         self,
-        partname: str,
+        partname: PackURI,
         content_type: str,
         blob: bytes | None = None,
         package: Package | None = None,
     ):
         super(Part, self).__init__()
         self._partname = partname
         self._content_type = content_type
@@ -52,21 +55,21 @@
         May be overridden by subclasses without forwarding call to super.
         """
         # don't place any code here, just catch call if not overridden by
         # subclass
         pass
 
     @property
-    def blob(self):
+    def blob(self) -> bytes:
         """Contents of this package part as a sequence of bytes.
 
         May be text or binary. Intended to be overridden by subclasses. Default behavior
         is to return load blob.
         """
-        return self._blob
+        return self._blob or b""
 
     @property
     def content_type(self):
         """Content type of this part."""
         return self._content_type
 
     def drop_rel(self, rId: str):
@@ -75,15 +78,15 @@
 
         Relationships with a reference count of 0 are implicit relationships.
         """
         if self._rel_ref_count(rId) < 2:
             del self.rels[rId]
 
     @classmethod
-    def load(cls, partname: str, content_type: str, blob: bytes, package: Package):
+    def load(cls, partname: PackURI, content_type: str, blob: bytes, package: Package):
         return cls(partname, content_type, blob, package)
 
     def load_rel(self, reltype: str, target: Part | str, rId: str, is_external: bool = False):
         """Return newly added |_Relationship| instance of `reltype`.
 
         The new relationship relates the `target` part to this part with key `rId`.
 
@@ -101,15 +104,15 @@
     @property
     def partname(self):
         """|PackURI| instance holding partname of this part, e.g.
         '/ppt/slides/slide1.xml'."""
         return self._partname
 
     @partname.setter
-    def partname(self, partname):
+    def partname(self, partname: str):
         if not isinstance(partname, PackURI):
             tmpl = "partname must be instance of PackURI, got '%s'"
             raise TypeError(tmpl % type(partname).__name__)
         self._partname = partname
 
     def part_related_by(self, reltype: str) -> Part:
         """Return part to which this part has a relationship of `reltype`.
@@ -123,41 +126,44 @@
     def relate_to(self, target: Part | str, reltype: str, is_external: bool = False) -> str:
         """Return rId key of relationship of `reltype` to `target`.
 
         The returned `rId` is from an existing relationship if there is one, otherwise a
         new relationship is created.
         """
         if is_external:
-            return self.rels.get_or_add_ext_rel(reltype, target)
+            return self.rels.get_or_add_ext_rel(reltype, cast(str, target))
         else:
-            rel = self.rels.get_or_add(reltype, target)
+            rel = self.rels.get_or_add(reltype, cast(Part, target))
             return rel.rId
 
     @property
     def related_parts(self):
         """Dictionary mapping related parts by rId, so child objects can resolve
         explicit relationships present in the part XML, e.g. sldIdLst to a specific
         |Slide| instance."""
         return self.rels.related_parts
 
     @lazyproperty
     def rels(self):
         """|Relationships| instance holding the relationships for this part."""
-        return Relationships(self._partname.baseURI)
+        # -- prevent breakage in `python-docx-template` by retaining legacy `._rels` attribute --
+        self._rels = Relationships(self._partname.baseURI)
+        return self._rels
 
     def target_ref(self, rId: str) -> str:
         """Return URL contained in target ref of relationship identified by `rId`."""
         rel = self.rels[rId]
         return rel.target_ref
 
-    def _rel_ref_count(self, rId):
-        """Return the count of references in this part's XML to the relationship
-        identified by `rId`."""
-        rIds = self._element.xpath("//@r:id")
-        return len([_rId for _rId in rIds if _rId == rId])
+    def _rel_ref_count(self, rId: str) -> int:
+        """Return the count of references in this part to the relationship identified by `rId`.
+
+        Only an XML part can contain references, so this is 0 for `Part`.
+        """
+        return 0
 
 
 class PartFactory:
     """Provides a way for client code to specify a subclass of |Part| to be constructed
     by |Unmarshaller| based on its content type and/or a custom callable.
 
     Setting ``PartFactory.part_class_selector`` to a callable object will cause that
@@ -166,20 +172,20 @@
     that part. If it returns |None|, part class selection falls back to the content type
     map defined in ``PartFactory.part_type_for``. If no class is returned from either of
     these, the class contained in ``PartFactory.default_part_type`` is used to construct
     the part, which is by default ``opc.package.Part``.
     """
 
     part_class_selector: Callable[[str, str], Type[Part] | None] | None
-    part_type_for: Dict[str, Type[Part]] = {}
+    part_type_for: dict[str, Type[Part]] = {}
     default_part_type = Part
 
     def __new__(
         cls,
-        partname: str,
+        partname: PackURI,
         content_type: str,
         reltype: str,
         blob: bytes,
         package: Package,
     ):
         PartClass: Type[Part] | None = None
         if cls.part_class_selector is not None:
@@ -201,33 +207,41 @@
 class XmlPart(Part):
     """Base class for package parts containing an XML payload, which is most of them.
 
     Provides additional methods to the |Part| base class that take care of parsing and
     reserializing the XML payload and managing relationships to other parts.
     """
 
-    def __init__(self, partname, content_type, element, package):
+    def __init__(
+        self, partname: PackURI, content_type: str, element: BaseOxmlElement, package: Package
+    ):
         super(XmlPart, self).__init__(partname, content_type, package=package)
         self._element = element
 
     @property
     def blob(self):
         return serialize_part_xml(self._element)
 
     @property
     def element(self):
         """The root XML element of this XML part."""
         return self._element
 
     @classmethod
-    def load(cls, partname, content_type, blob, package):
+    def load(cls, partname: PackURI, content_type: str, blob: bytes, package: Package):
         element = parse_xml(blob)
         return cls(partname, content_type, element, package)
 
     @property
     def part(self):
         """Part of the parent protocol, "children" of the document will not know the
         part that contains them so must ask their parent object.
 
         That chain of delegation ends here for child objects.
         """
         return self
+
+    def _rel_ref_count(self, rId: str) -> int:
+        """Return the count of references in this part's XML to the relationship
+        identified by `rId`."""
+        rIds = cast("list[str]", self._element.xpath("//@r:id"))
+        return len([_rId for _rId in rIds if _rId == rId])
```

### Comparing `python_docx-1.1.1/src/docx/opc/parts/coreprops.py` & `python_docx-1.1.2/tests/opc/parts/test_coreprops.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,53 @@
-"""Core properties part, corresponds to ``/docProps/core.xml`` part in package."""
+"""Unit test suite for the docx.opc.parts.coreprops module."""
 
-from datetime import datetime
+from __future__ import annotations
+
+import datetime as dt
+
+import pytest
 
-from docx.opc.constants import CONTENT_TYPE as CT
 from docx.opc.coreprops import CoreProperties
+from docx.opc.package import OpcPackage
 from docx.opc.packuri import PackURI
-from docx.opc.part import XmlPart
-from docx.oxml.coreprops import CT_CoreProperties
+from docx.opc.parts.coreprops import CorePropertiesPart
+
+from ...unitutil.cxml import element
+from ...unitutil.mock import FixtureRequest, Mock, class_mock, instance_mock
+
+
+class DescribeCorePropertiesPart:
+    """Unit-test suite for `docx.opc.parts.coreprops.CorePropertiesPart` objects."""
+
+    def it_provides_access_to_its_core_props_object(self, CoreProperties_: Mock, package_: Mock):
+        core_properties_part = CorePropertiesPart(
+            PackURI("/part/name"), "content/type", element("cp:coreProperties"), package_
+        )
+
+        core_properties = core_properties_part.core_properties
+
+        CoreProperties_.assert_called_once_with(core_properties_part.element)
+        assert isinstance(core_properties, CoreProperties)
 
+    def it_can_create_a_default_core_properties_part(self, package_: Mock):
+        core_properties_part = CorePropertiesPart.default(package_)
 
-class CorePropertiesPart(XmlPart):
-    """Corresponds to part named ``/docProps/core.xml``, containing the core document
-    properties for this document package."""
-
-    @classmethod
-    def default(cls, package):
-        """Return a new |CorePropertiesPart| object initialized with default values for
-        its base properties."""
-        core_properties_part = cls._new(package)
+        assert isinstance(core_properties_part, CorePropertiesPart)
+        # --
         core_properties = core_properties_part.core_properties
-        core_properties.title = "Word Document"
-        core_properties.last_modified_by = "python-docx"
-        core_properties.revision = 1
-        core_properties.modified = datetime.utcnow()
-        return core_properties_part
-
-    @property
-    def core_properties(self):
-        """A |CoreProperties| object providing read/write access to the core properties
-        contained in this core properties part."""
-        return CoreProperties(self.element)
-
-    @classmethod
-    def _new(cls, package):
-        partname = PackURI("/docProps/core.xml")
-        content_type = CT.OPC_CORE_PROPERTIES
-        coreProperties = CT_CoreProperties.new()
-        return CorePropertiesPart(partname, content_type, coreProperties, package)
+        assert core_properties.title == "Word Document"
+        assert core_properties.last_modified_by == "python-docx"
+        assert core_properties.revision == 1
+        assert core_properties.modified is not None
+        delta = dt.datetime.now(dt.timezone.utc) - core_properties.modified
+        max_expected_delta = dt.timedelta(seconds=2)
+        assert delta < max_expected_delta
+
+    # fixtures ---------------------------------------------
+
+    @pytest.fixture
+    def CoreProperties_(self, request: FixtureRequest):
+        return class_mock(request, "docx.opc.parts.coreprops.CoreProperties")
+
+    @pytest.fixture
+    def package_(self, request: FixtureRequest):
+        return instance_mock(request, OpcPackage)
```

### Comparing `python_docx-1.1.1/src/docx/opc/phys_pkg.py` & `python_docx-1.1.2/src/docx/opc/phys_pkg.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/opc/pkgreader.py` & `python_docx-1.1.2/src/docx/opc/pkgreader.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/opc/pkgwriter.py` & `python_docx-1.1.2/src/docx/opc/pkgwriter.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/opc/rel.py` & `python_docx-1.1.2/src/docx/opc/rel.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Relationship-related objects."""
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Dict
+from typing import TYPE_CHECKING, Any, Dict, cast
 
 from docx.opc.oxml import CT_Relationships
 
 if TYPE_CHECKING:
     from docx.opc.part import Part
 
 
 class Relationships(Dict[str, "_Relationship"]):
     """Collection object for |_Relationship| instances, having list semantics."""
 
     def __init__(self, baseURI: str):
         super(Relationships, self).__init__()
         self._baseURI = baseURI
-        self._target_parts_by_rId: Dict[str, Any] = {}
+        self._target_parts_by_rId: dict[str, Any] = {}
 
     def add_relationship(
         self, reltype: str, target: Part | str, rId: str, is_external: bool = False
     ) -> "_Relationship":
         """Return a newly added |_Relationship| instance."""
         rel = _Relationship(rId, reltype, target, self._baseURI, is_external)
         self[rId] = rel
@@ -33,66 +33,66 @@
         present in collection."""
         rel = self._get_matching(reltype, target_part)
         if rel is None:
             rId = self._next_rId
             rel = self.add_relationship(reltype, target_part, rId)
         return rel
 
-    def get_or_add_ext_rel(self, reltype, target_ref):
+    def get_or_add_ext_rel(self, reltype: str, target_ref: str) -> str:
         """Return rId of external relationship of `reltype` to `target_ref`, newly added
         if not already present in collection."""
         rel = self._get_matching(reltype, target_ref, is_external=True)
         if rel is None:
             rId = self._next_rId
             rel = self.add_relationship(reltype, target_ref, rId, is_external=True)
         return rel.rId
 
-    def part_with_reltype(self, reltype):
+    def part_with_reltype(self, reltype: str) -> Part:
         """Return target part of rel with matching `reltype`, raising |KeyError| if not
         found and |ValueError| if more than one matching relationship is found."""
         rel = self._get_rel_of_type(reltype)
         return rel.target_part
 
     @property
     def related_parts(self):
         """Dict mapping rIds to target parts for all the internal relationships in the
         collection."""
         return self._target_parts_by_rId
 
     @property
-    def xml(self):
+    def xml(self) -> str:
         """Serialize this relationship collection into XML suitable for storage as a
         .rels file in an OPC package."""
         rels_elm = CT_Relationships.new()
         for rel in self.values():
             rels_elm.add_rel(rel.rId, rel.reltype, rel.target_ref, rel.is_external)
         return rels_elm.xml
 
     def _get_matching(
         self, reltype: str, target: Part | str, is_external: bool = False
     ) -> _Relationship | None:
         """Return relationship of matching `reltype`, `target`, and `is_external` from
         collection, or None if not found."""
 
-        def matches(rel, reltype, target, is_external):
+        def matches(rel: _Relationship, reltype: str, target: Part | str, is_external: bool):
             if rel.reltype != reltype:
                 return False
             if rel.is_external != is_external:
                 return False
             rel_target = rel.target_ref if rel.is_external else rel.target_part
             if rel_target != target:
                 return False
             return True
 
         for rel in self.values():
             if matches(rel, reltype, target, is_external):
                 return rel
         return None
 
-    def _get_rel_of_type(self, reltype):
+    def _get_rel_of_type(self, reltype: str):
         """Return single relationship of type `reltype` from the collection.
 
         Raises |KeyError| if no matching relationship is found. Raises |ValueError| if
         more than one matching relationship is found.
         """
         matching = [rel for rel in self.values() if rel.reltype == reltype]
         if len(matching) == 0:
@@ -100,53 +100,56 @@
             raise KeyError(tmpl % reltype)
         if len(matching) > 1:
             tmpl = "multiple relationships of type '%s' in collection"
             raise ValueError(tmpl % reltype)
         return matching[0]
 
     @property
-    def _next_rId(self) -> str:
+    def _next_rId(self) -> str:  # pyright: ignore[reportReturnType]
         """Next available rId in collection, starting from 'rId1' and making use of any
         gaps in numbering, e.g. 'rId2' for rIds ['rId1', 'rId3']."""
         for n in range(1, len(self) + 2):
             rId_candidate = "rId%d" % n  # like 'rId19'
             if rId_candidate not in self:
                 return rId_candidate
 
 
 class _Relationship:
     """Value object for relationship to part."""
 
-    def __init__(self, rId: str, reltype, target, baseURI, external=False):
+    def __init__(
+        self, rId: str, reltype: str, target: Part | str, baseURI: str, external: bool = False
+    ):
         super(_Relationship, self).__init__()
         self._rId = rId
         self._reltype = reltype
         self._target = target
         self._baseURI = baseURI
         self._is_external = bool(external)
 
     @property
-    def is_external(self):
+    def is_external(self) -> bool:
         return self._is_external
 
     @property
-    def reltype(self):
+    def reltype(self) -> str:
         return self._reltype
 
     @property
-    def rId(self):
+    def rId(self) -> str:
         return self._rId
 
     @property
-    def target_part(self):
+    def target_part(self) -> Part:
         if self._is_external:
             raise ValueError(
                 "target_part property on _Relationship is undef" "ined when target mode is External"
             )
-        return self._target
+        return cast("Part", self._target)
 
     @property
     def target_ref(self) -> str:
         if self._is_external:
-            return self._target
+            return cast(str, self._target)
         else:
-            return self._target.partname.relative_ref(self._baseURI)
+            target = cast("Part", self._target)
+            return target.partname.relative_ref(self._baseURI)
```

### Comparing `python_docx-1.1.1/src/docx/opc/shared.py` & `python_docx-1.1.2/src/docx/opc/shared.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/opc/spec.py` & `python_docx-1.1.2/src/docx/opc/spec.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/oxml/__init__.py` & `python_docx-1.1.2/src/docx/oxml/__init__.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/oxml/coreprops.py` & `python_docx-1.1.2/src/docx/oxml/coreprops.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 """Custom element classes for core properties-related XML elements."""
 
+from __future__ import annotations
+
+import datetime as dt
 import re
-from datetime import datetime, timedelta
-from typing import Any
+from typing import TYPE_CHECKING, Any, Callable
 
 from docx.oxml.ns import nsdecls, qn
 from docx.oxml.parser import parse_xml
 from docx.oxml.xmlchemy import BaseOxmlElement, ZeroOrOne
 
+if TYPE_CHECKING:
+    from lxml.etree import _Element as etree_Element  # pyright: ignore[reportPrivateUsage]
+
 
 class CT_CoreProperties(BaseOxmlElement):
     """`<cp:coreProperties>` element, the root element of the Core Properties part.
 
     Stored as `/docProps/core.xml`. Implements many of the Dublin Core document metadata
     elements. String elements resolve to an empty string ("") if the element is not
     present in the XML. String elements are limited in length to 255 unicode characters.
     """
 
+    get_or_add_revision: Callable[[], etree_Element]
+
     category = ZeroOrOne("cp:category", successors=())
     contentStatus = ZeroOrOne("cp:contentStatus", successors=())
     created = ZeroOrOne("dcterms:created", successors=())
     creator = ZeroOrOne("dc:creator", successors=())
     description = ZeroOrOne("dc:description", successors=())
     identifier = ZeroOrOne("dc:identifier", successors=())
     keywords = ZeroOrOne("cp:keywords", successors=())
     language = ZeroOrOne("dc:language", successors=())
     lastModifiedBy = ZeroOrOne("cp:lastModifiedBy", successors=())
     lastPrinted = ZeroOrOne("cp:lastPrinted", successors=())
     modified = ZeroOrOne("dcterms:modified", successors=())
-    revision = ZeroOrOne("cp:revision", successors=())
+    revision: etree_Element | None = ZeroOrOne(  # pyright: ignore[reportAssignmentType]
+        "cp:revision", successors=()
+    )
     subject = ZeroOrOne("dc:subject", successors=())
     title = ZeroOrOne("dc:title", successors=())
     version = ZeroOrOne("cp:version", successors=())
 
     _coreProperties_tmpl = "<cp:coreProperties %s/>\n" % nsdecls("cp", "dc", "dcterms")
 
     @classmethod
@@ -76,153 +85,153 @@
         self._set_element_text("contentStatus", value)
 
     @property
     def created_datetime(self):
         return self._datetime_of_element("created")
 
     @created_datetime.setter
-    def created_datetime(self, value):
+    def created_datetime(self, value: dt.datetime):
         self._set_element_datetime("created", value)
 
     @property
     def identifier_text(self):
         return self._text_of_element("identifier")
 
     @identifier_text.setter
-    def identifier_text(self, value):
+    def identifier_text(self, value: str):
         self._set_element_text("identifier", value)
 
     @property
     def keywords_text(self):
         return self._text_of_element("keywords")
 
     @keywords_text.setter
-    def keywords_text(self, value):
+    def keywords_text(self, value: str):
         self._set_element_text("keywords", value)
 
     @property
     def language_text(self):
         return self._text_of_element("language")
 
     @language_text.setter
-    def language_text(self, value):
+    def language_text(self, value: str):
         self._set_element_text("language", value)
 
     @property
     def lastModifiedBy_text(self):
         return self._text_of_element("lastModifiedBy")
 
     @lastModifiedBy_text.setter
-    def lastModifiedBy_text(self, value):
+    def lastModifiedBy_text(self, value: str):
         self._set_element_text("lastModifiedBy", value)
 
     @property
     def lastPrinted_datetime(self):
         return self._datetime_of_element("lastPrinted")
 
     @lastPrinted_datetime.setter
-    def lastPrinted_datetime(self, value):
+    def lastPrinted_datetime(self, value: dt.datetime):
         self._set_element_datetime("lastPrinted", value)
 
     @property
-    def modified_datetime(self):
+    def modified_datetime(self) -> dt.datetime | None:
         return self._datetime_of_element("modified")
 
     @modified_datetime.setter
-    def modified_datetime(self, value):
+    def modified_datetime(self, value: dt.datetime):
         self._set_element_datetime("modified", value)
 
     @property
     def revision_number(self):
         """Integer value of revision property."""
         revision = self.revision
         if revision is None:
             return 0
-        revision_str = revision.text
+        revision_str = str(revision.text)
         try:
             revision = int(revision_str)
         except ValueError:
             # non-integer revision strings also resolve to 0
             revision = 0
         # as do negative integers
         if revision < 0:
             revision = 0
         return revision
 
     @revision_number.setter
-    def revision_number(self, value):
+    def revision_number(self, value: int):
         """Set revision property to string value of integer `value`."""
-        if not isinstance(value, int) or value < 1:
+        if not isinstance(value, int) or value < 1:  # pyright: ignore[reportUnnecessaryIsInstance]
             tmpl = "revision property requires positive int, got '%s'"
             raise ValueError(tmpl % value)
         revision = self.get_or_add_revision()
         revision.text = str(value)
 
     @property
     def subject_text(self):
         return self._text_of_element("subject")
 
     @subject_text.setter
-    def subject_text(self, value):
+    def subject_text(self, value: str):
         self._set_element_text("subject", value)
 
     @property
     def title_text(self):
         return self._text_of_element("title")
 
     @title_text.setter
-    def title_text(self, value):
+    def title_text(self, value: str):
         self._set_element_text("title", value)
 
     @property
     def version_text(self):
         return self._text_of_element("version")
 
     @version_text.setter
-    def version_text(self, value):
+    def version_text(self, value: str):
         self._set_element_text("version", value)
 
-    def _datetime_of_element(self, property_name):
+    def _datetime_of_element(self, property_name: str) -> dt.datetime | None:
         element = getattr(self, property_name)
         if element is None:
             return None
         datetime_str = element.text
         try:
             return self._parse_W3CDTF_to_datetime(datetime_str)
         except ValueError:
             # invalid datetime strings are ignored
             return None
 
-    def _get_or_add(self, prop_name):
+    def _get_or_add(self, prop_name: str) -> BaseOxmlElement:
         """Return element returned by "get_or_add_" method for `prop_name`."""
         get_or_add_method_name = "get_or_add_%s" % prop_name
         get_or_add_method = getattr(self, get_or_add_method_name)
         element = get_or_add_method()
         return element
 
     @classmethod
-    def _offset_dt(cls, dt, offset_str):
-        """A |datetime| instance offset from `dt` by timezone offset in `offset_str`.
+    def _offset_dt(cls, dt_: dt.datetime, offset_str: str) -> dt.datetime:
+        """A |datetime| instance offset from `dt_` by timezone offset in `offset_str`.
 
         `offset_str` is like `"-07:00"`.
         """
         match = cls._offset_pattern.match(offset_str)
         if match is None:
             raise ValueError("'%s' is not a valid offset string" % offset_str)
         sign, hours_str, minutes_str = match.groups()
         sign_factor = -1 if sign == "+" else 1
         hours = int(hours_str) * sign_factor
         minutes = int(minutes_str) * sign_factor
-        td = timedelta(hours=hours, minutes=minutes)
-        return dt + td
+        td = dt.timedelta(hours=hours, minutes=minutes)
+        return dt_ + td
 
     _offset_pattern = re.compile(r"([+-])(\d\d):(\d\d)")
 
     @classmethod
-    def _parse_W3CDTF_to_datetime(cls, w3cdtf_str):
+    def _parse_W3CDTF_to_datetime(cls, w3cdtf_str: str) -> dt.datetime:
         # valid W3CDTF date cases:
         # yyyy e.g. "2003"
         # yyyy-mm e.g. "2003-12"
         # yyyy-mm-dd e.g. "2003-12-31"
         # UTC timezone e.g. "2003-12-31T10:14:55Z"
         # numeric timezone e.g. "2003-12-31T10:14:55-08:00"
         templates = (
@@ -231,30 +240,30 @@
             "%Y-%m",
             "%Y",
         )
         # strptime isn't smart enough to parse literal timezone offsets like
         # "-07:30", so we have to do it ourselves
         parseable_part = w3cdtf_str[:19]
         offset_str = w3cdtf_str[19:]
-        dt = None
+        dt_ = None
         for tmpl in templates:
             try:
-                dt = datetime.strptime(parseable_part, tmpl)
+                dt_ = dt.datetime.strptime(parseable_part, tmpl)
             except ValueError:
                 continue
-        if dt is None:
+        if dt_ is None:
             tmpl = "could not parse W3CDTF datetime string '%s'"
             raise ValueError(tmpl % w3cdtf_str)
         if len(offset_str) == 6:
-            return cls._offset_dt(dt, offset_str)
-        return dt
+            dt_ = cls._offset_dt(dt_, offset_str)
+        return dt_.replace(tzinfo=dt.timezone.utc)
 
-    def _set_element_datetime(self, prop_name, value):
+    def _set_element_datetime(self, prop_name: str, value: dt.datetime):
         """Set date/time value of child element having `prop_name` to `value`."""
-        if not isinstance(value, datetime):
+        if not isinstance(value, dt.datetime):  # pyright: ignore[reportUnnecessaryIsInstance]
             tmpl = "property requires <type 'datetime.datetime'> object, got %s"
             raise ValueError(tmpl % type(value))
         element = self._get_or_add(prop_name)
         dt_str = value.strftime("%Y-%m-%dT%H:%M:%SZ")
         element.text = dt_str
         if prop_name in ("created", "modified"):
             # These two require an explicit "xsi:type="dcterms:W3CDTF""
```

### Comparing `python_docx-1.1.1/src/docx/oxml/document.py` & `python_docx-1.1.2/src/docx/oxml/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     from docx.oxml.table import CT_Tbl
     from docx.oxml.text.paragraph import CT_P
 
 
 class CT_Document(BaseOxmlElement):
     """``<w:document>`` element, the root element of a document.xml file."""
 
-    body = ZeroOrOne("w:body")
+    body: CT_Body = ZeroOrOne("w:body")  # pyright: ignore[reportAssignmentType]
 
     @property
     def sectPr_lst(self) -> List[CT_SectPr]:
         """All `w:sectPr` elements directly accessible from document element.
 
         Note this does not include a `sectPr` child in a paragraphs wrapped in
         revision marks or other intervening layer, perhaps `w:sdt` or customXml
```

### Comparing `python_docx-1.1.1/src/docx/oxml/ns.py` & `python_docx-1.1.2/src/docx/oxml/ns.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/oxml/numbering.py` & `python_docx-1.1.2/src/docx/oxml/numbering.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/oxml/parser.py` & `python_docx-1.1.2/src/docx/oxml/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 # -- configure XML parser --
 element_class_lookup = etree.ElementNamespaceClassLookup()
 oxml_parser = etree.XMLParser(remove_blank_text=True, resolve_entities=False)
 oxml_parser.set_element_class_lookup(element_class_lookup)
 
 
-def parse_xml(xml: str) -> "BaseOxmlElement":
+def parse_xml(xml: str | bytes) -> "BaseOxmlElement":
     """Root lxml element obtained by parsing XML character string `xml`.
 
     The custom parser is used, so custom element classes are produced for elements in
     `xml` that have them.
     """
     return cast("BaseOxmlElement", etree.fromstring(xml, oxml_parser))
```

### Comparing `python_docx-1.1.1/src/docx/oxml/section.py` & `python_docx-1.1.2/src/docx/oxml/section.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/oxml/settings.py` & `python_docx-1.1.2/src/docx/oxml/settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 """Custom element classes related to document settings."""
 
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Callable
+
 from docx.oxml.xmlchemy import BaseOxmlElement, ZeroOrOne
 
+if TYPE_CHECKING:
+    from docx.oxml.shared import CT_OnOff
+
 
 class CT_Settings(BaseOxmlElement):
     """`w:settings` element, root element for the settings part."""
 
+    get_or_add_evenAndOddHeaders: Callable[[], CT_OnOff]
+    _remove_evenAndOddHeaders: Callable[[], None]
+
     _tag_seq = (
         "w:writeProtection",
         "w:view",
         "w:zoom",
         "w:removePersonalInformation",
         "w:removeDateAndTime",
         "w:doNotDisplayPageBoundaries",
@@ -102,24 +112,27 @@
         "w:smartTagType",
         "sl:schemaLibrary",
         "w:shapeDefaults",
         "w:doNotEmbedSmartTags",
         "w:decimalSymbol",
         "w:listSeparator",
     )
-    evenAndOddHeaders = ZeroOrOne("w:evenAndOddHeaders", successors=_tag_seq[48:])
+    evenAndOddHeaders: CT_OnOff | None = ZeroOrOne(  # pyright: ignore[reportAssignmentType]
+        "w:evenAndOddHeaders", successors=_tag_seq[48:]
+    )
     del _tag_seq
 
     @property
-    def evenAndOddHeaders_val(self):
+    def evenAndOddHeaders_val(self) -> bool:
         """Value of `w:evenAndOddHeaders/@w:val` or |None| if not present."""
         evenAndOddHeaders = self.evenAndOddHeaders
         if evenAndOddHeaders is None:
             return False
         return evenAndOddHeaders.val
 
     @evenAndOddHeaders_val.setter
-    def evenAndOddHeaders_val(self, value):
-        if value in [None, False]:
+    def evenAndOddHeaders_val(self, value: bool | None):
+        if value is None or value is False:
             self._remove_evenAndOddHeaders()
-        else:
-            self.get_or_add_evenAndOddHeaders().val = value
+            return
+
+        self.get_or_add_evenAndOddHeaders().val = value
```

### Comparing `python_docx-1.1.1/src/docx/oxml/shape.py` & `python_docx-1.1.2/src/docx/oxml/shape.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Custom element classes for shape-related elements like `<w:inline>`."""
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, cast
 
 from docx.oxml.ns import nsdecls
 from docx.oxml.parser import parse_xml
 from docx.oxml.simpletypes import (
     ST_Coordinate,
     ST_DrawingElementId,
     ST_PositiveCoordinate,
@@ -30,56 +30,66 @@
     """`<wp:anchor>` element, container for a "floating" shape."""
 
 
 class CT_Blip(BaseOxmlElement):
     """``<a:blip>`` element, specifies image source and adjustments such as alpha and
     tint."""
 
-    embed = OptionalAttribute("r:embed", ST_RelationshipId)
-    link = OptionalAttribute("r:link", ST_RelationshipId)
+    embed: str | None = OptionalAttribute(  # pyright: ignore[reportAssignmentType]
+        "r:embed", ST_RelationshipId
+    )
+    link: str | None = OptionalAttribute(  # pyright: ignore[reportAssignmentType]
+        "r:link", ST_RelationshipId
+    )
 
 
 class CT_BlipFillProperties(BaseOxmlElement):
     """``<pic:blipFill>`` element, specifies picture properties."""
 
-    blip = ZeroOrOne("a:blip", successors=("a:srcRect", "a:tile", "a:stretch"))
+    blip: CT_Blip = ZeroOrOne(  # pyright: ignore[reportAssignmentType]
+        "a:blip", successors=("a:srcRect", "a:tile", "a:stretch")
+    )
 
 
 class CT_GraphicalObject(BaseOxmlElement):
     """``<a:graphic>`` element, container for a DrawingML object."""
 
-    graphicData = OneAndOnlyOne("a:graphicData")
+    graphicData: CT_GraphicalObjectData = OneAndOnlyOne(  # pyright: ignore[reportAssignmentType]
+        "a:graphicData"
+    )
 
 
 class CT_GraphicalObjectData(BaseOxmlElement):
     """``<a:graphicData>`` element, container for the XML of a DrawingML object."""
 
-    pic = ZeroOrOne("pic:pic")
-    uri = RequiredAttribute("uri", XsdToken)
+    pic: CT_Picture = ZeroOrOne("pic:pic")  # pyright: ignore[reportAssignmentType]
+    uri: str = RequiredAttribute("uri", XsdToken)  # pyright: ignore[reportAssignmentType]
 
 
 class CT_Inline(BaseOxmlElement):
     """`<wp:inline>` element, container for an inline shape."""
 
-    extent = OneAndOnlyOne("wp:extent")
-    docPr = OneAndOnlyOne("wp:docPr")
-    graphic = OneAndOnlyOne("a:graphic")
+    extent: CT_PositiveSize2D = OneAndOnlyOne("wp:extent")  # pyright: ignore[reportAssignmentType]
+    docPr: CT_NonVisualDrawingProps = OneAndOnlyOne(  # pyright: ignore[reportAssignmentType]
+        "wp:docPr"
+    )
+    graphic: CT_GraphicalObject = OneAndOnlyOne(  # pyright: ignore[reportAssignmentType]
+        "a:graphic"
+    )
 
     @classmethod
     def new(cls, cx: Length, cy: Length, shape_id: int, pic: CT_Picture) -> CT_Inline:
         """Return a new ``<wp:inline>`` element populated with the values passed as
         parameters."""
-        inline = parse_xml(cls._inline_xml())
+        inline = cast(CT_Inline, parse_xml(cls._inline_xml()))
         inline.extent.cx = cx
         inline.extent.cy = cy
         inline.docPr.id = shape_id
         inline.docPr.name = "Picture %d" % shape_id
-        inline.graphic.graphicData.uri = (
-            "http://schemas.openxmlformats.org/drawingml/2006/picture"
-        )
+        inline.graphic.graphicData.uri = "http://schemas.openxmlformats.org/drawingml/2006/picture"
         inline.graphic.graphicData._insert_pic(pic)
         return inline
 
     @classmethod
     def new_pic_inline(
         cls, shape_id: int, rId: str, filename: str, cx: Length, cy: Length
     ) -> CT_Inline:
@@ -122,17 +132,21 @@
 class CT_NonVisualPictureProperties(BaseOxmlElement):
     """``<pic:cNvPicPr>`` element, specifies picture locking and resize behaviors."""
 
 
 class CT_Picture(BaseOxmlElement):
     """``<pic:pic>`` element, a DrawingML picture."""
 
-    nvPicPr = OneAndOnlyOne("pic:nvPicPr")
-    blipFill = OneAndOnlyOne("pic:blipFill")
-    spPr = OneAndOnlyOne("pic:spPr")
+    nvPicPr: CT_PictureNonVisual = OneAndOnlyOne(  # pyright: ignore[reportAssignmentType]
+        "pic:nvPicPr"
+    )
+    blipFill: CT_BlipFillProperties = OneAndOnlyOne(  # pyright: ignore[reportAssignmentType]
+        "pic:blipFill"
+    )
+    spPr: CT_ShapeProperties = OneAndOnlyOne("pic:spPr")  # pyright: ignore[reportAssignmentType]
 
     @classmethod
     def new(cls, pic_id, filename, rId, cx, cy):
         """Return a new ``<pic:pic>`` element populated with the minimal contents
         required to define a viable picture element, based on the values passed as
         parameters."""
         pic = parse_xml(cls._pic_xml())
@@ -186,16 +200,20 @@
 
 class CT_PositiveSize2D(BaseOxmlElement):
     """Used for ``<wp:extent>`` element, and perhaps others later.
 
     Specifies the size of a DrawingML drawing.
     """
 
-    cx = RequiredAttribute("cx", ST_PositiveCoordinate)
-    cy = RequiredAttribute("cy", ST_PositiveCoordinate)
+    cx: Length = RequiredAttribute(  # pyright: ignore[reportAssignmentType]
+        "cx", ST_PositiveCoordinate
+    )
+    cy: Length = RequiredAttribute(  # pyright: ignore[reportAssignmentType]
+        "cy", ST_PositiveCoordinate
+    )
 
 
 class CT_PresetGeometry2D(BaseOxmlElement):
     """``<a:prstGeom>`` element, specifies an preset autoshape geometry, such as
     ``rect``."""
```

### Comparing `python_docx-1.1.1/src/docx/oxml/shared.py` & `python_docx-1.1.2/src/docx/oxml/shared.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,39 +14,39 @@
     """Used for ``<w:numId>``, ``<w:ilvl>``, ``<w:abstractNumId>`` and several others,
     containing a text representation of a decimal number (e.g. 42) in its ``val``
     attribute."""
 
     val: int = RequiredAttribute("w:val", ST_DecimalNumber)  # pyright: ignore[reportAssignmentType]
 
     @classmethod
-    def new(cls, nsptagname, val):
+    def new(cls, nsptagname: str, val: int):
         """Return a new ``CT_DecimalNumber`` element having tagname `nsptagname` and
         ``val`` attribute set to `val`."""
         return OxmlElement(nsptagname, attrs={qn("w:val"): str(val)})
 
 
 class CT_OnOff(BaseOxmlElement):
     """Used for `w:b`, `w:i` elements and others.
 
     Contains a bool-ish string in its `val` attribute, xsd:boolean plus "on" and
     "off". Defaults to `True`, so `<w:b>` for example means "bold is turned on".
     """
 
-    val: bool = OptionalAttribute(  # pyright: ignore[reportGeneralTypeIssues]
+    val: bool = OptionalAttribute(  # pyright: ignore[reportAssignmentType]
         "w:val", ST_OnOff, default=True
     )
 
 
 class CT_String(BaseOxmlElement):
     """Used for `w:pStyle` and `w:tblStyle` elements and others.
 
     In those cases, it containing a style name in its `val` attribute.
     """
 
-    val: str = RequiredAttribute("w:val", ST_String)  # pyright: ignore[reportGeneralTypeIssues]
+    val: str = RequiredAttribute("w:val", ST_String)  # pyright: ignore[reportAssignmentType]
 
     @classmethod
     def new(cls, nsptagname: str, val: str):
         """Return a new ``CT_String`` element with tagname `nsptagname` and ``val``
         attribute set to `val`."""
         elm = cast(CT_String, OxmlElement(nsptagname))
         elm.val = val
```

### Comparing `python_docx-1.1.1/src/docx/oxml/simpletypes.py` & `python_docx-1.1.2/src/docx/oxml/simpletypes.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/oxml/styles.py` & `python_docx-1.1.2/src/docx/oxml/styles.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,20 +124,18 @@
     unhideWhenUsed = ZeroOrOne("w:unhideWhenUsed", successors=_tag_seq[10:])
     qFormat = ZeroOrOne("w:qFormat", successors=_tag_seq[11:])
     locked = ZeroOrOne("w:locked", successors=_tag_seq[12:])
     pPr = ZeroOrOne("w:pPr", successors=_tag_seq[17:])
     rPr = ZeroOrOne("w:rPr", successors=_tag_seq[18:])
     del _tag_seq
 
-    type: WD_STYLE_TYPE | None = (
-        OptionalAttribute(  # pyright: ignore[reportGeneralTypeIssues]
-            "w:type", WD_STYLE_TYPE
-        )
+    type: WD_STYLE_TYPE | None = OptionalAttribute(  # pyright: ignore[reportAssignmentType]
+        "w:type", WD_STYLE_TYPE
     )
-    styleId: str | None = OptionalAttribute(  # pyright: ignore[reportGeneralTypeIssues]
+    styleId: str | None = OptionalAttribute(  # pyright: ignore[reportAssignmentType]
         "w:styleId", ST_String
     )
     default = OptionalAttribute("w:default", ST_OnOff)
     customStyle = OptionalAttribute("w:customStyle", ST_OnOff)
 
     @property
     def basedOn_val(self):
```

### Comparing `python_docx-1.1.1/src/docx/oxml/table.py` & `python_docx-1.1.2/src/docx/oxml/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -969,9 +969,9 @@
     )
 
 
 class CT_VMerge(BaseOxmlElement):
     """``<w:vMerge>`` element, specifying vertical merging behavior of a cell."""
 
     val: str | None = OptionalAttribute(  # pyright: ignore[reportAssignmentType]
-        "w:val", ST_Merge, default=ST_Merge.CONTINUE  # pyright: ignore[reportArgumentType]
+        "w:val", ST_Merge, default=ST_Merge.CONTINUE
     )
```

### Comparing `python_docx-1.1.1/src/docx/oxml/text/font.py` & `python_docx-1.1.2/src/docx/oxml/text/font.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,18 +35,18 @@
 
 class CT_Fonts(BaseOxmlElement):
     """`<w:rFonts>` element.
 
     Specifies typeface name for the various language types.
     """
 
-    ascii: str | None = OptionalAttribute(  # pyright: ignore[reportGeneralTypeIssues]
+    ascii: str | None = OptionalAttribute(  # pyright: ignore[reportAssignmentType]
         "w:ascii", ST_String
     )
-    hAnsi: str | None = OptionalAttribute(  # pyright: ignore[reportGeneralTypeIssues]
+    hAnsi: str | None = OptionalAttribute(  # pyright: ignore[reportAssignmentType]
         "w:hAnsi", ST_String
     )
 
 
 class CT_Highlight(BaseOxmlElement):
     """`w:highlight` element, specifying font highlighting/background color."""
 
@@ -144,26 +144,22 @@
     snapToGrid = ZeroOrOne("w:snapToGrid", successors=_tag_seq[16:])
     vanish = ZeroOrOne("w:vanish", successors=_tag_seq[17:])
     webHidden = ZeroOrOne("w:webHidden", successors=_tag_seq[18:])
     color = ZeroOrOne("w:color", successors=_tag_seq[19:])
     sz: CT_HpsMeasure | None = ZeroOrOne(  # pyright: ignore[reportGeneralTypeIssues]
         "w:sz", successors=_tag_seq[24:]
     )
-    highlight: CT_Highlight | None = (
-        ZeroOrOne(  # pyright: ignore[reportGeneralTypeIssues]
-            "w:highlight", successors=_tag_seq[26:]
-        )
+    highlight: CT_Highlight | None = ZeroOrOne(  # pyright: ignore[reportGeneralTypeIssues]
+        "w:highlight", successors=_tag_seq[26:]
     )
     u: CT_Underline | None = ZeroOrOne(  # pyright: ignore[reportGeneralTypeIssues]
         "w:u", successors=_tag_seq[27:]
     )
-    vertAlign: CT_VerticalAlignRun | None = (
-        ZeroOrOne(  # pyright: ignore[reportGeneralTypeIssues]
-            "w:vertAlign", successors=_tag_seq[32:]
-        )
+    vertAlign: CT_VerticalAlignRun | None = ZeroOrOne(  # pyright: ignore[reportGeneralTypeIssues]
+        "w:vertAlign", successors=_tag_seq[32:]
     )
     rtl = ZeroOrOne("w:rtl", successors=_tag_seq[33:])
     cs = ZeroOrOne("w:cs", successors=_tag_seq[34:])
     specVanish = ZeroOrOne("w:specVanish", successors=_tag_seq[38:])
     oMath = ZeroOrOne("w:oMath", successors=_tag_seq[39:])
     del _tag_seq
 
@@ -264,18 +260,15 @@
     @subscript.setter
     def subscript(self, value: bool | None) -> None:
         if value is None:
             self._remove_vertAlign()
         elif bool(value) is True:
             self.get_or_add_vertAlign().val = ST_VerticalAlignRun.SUBSCRIPT
         # -- assert bool(value) is False --
-        elif (
-            self.vertAlign is not None
-            and self.vertAlign.val == ST_VerticalAlignRun.SUBSCRIPT
-        ):
+        elif self.vertAlign is not None and self.vertAlign.val == ST_VerticalAlignRun.SUBSCRIPT:
             self._remove_vertAlign()
 
     @property
     def superscript(self) -> bool | None:
         """|True| if `w:vertAlign/@w:val` is 'superscript'.
 
         |False| if `w:vertAlign/@w:val` contains any other value. |None| if
@@ -291,18 +284,15 @@
     @superscript.setter
     def superscript(self, value: bool | None):
         if value is None:
             self._remove_vertAlign()
         elif bool(value) is True:
             self.get_or_add_vertAlign().val = ST_VerticalAlignRun.SUPERSCRIPT
         # -- assert bool(value) is False --
-        elif (
-            self.vertAlign is not None
-            and self.vertAlign.val == ST_VerticalAlignRun.SUPERSCRIPT
-        ):
+        elif self.vertAlign is not None and self.vertAlign.val == ST_VerticalAlignRun.SUPERSCRIPT:
             self._remove_vertAlign()
 
     @property
     def sz_val(self) -> Length | None:
         """The value of `w:sz/@w:val` or |None| if not present."""
         sz = self.sz
         if sz is None:
@@ -349,18 +339,16 @@
         element = getattr(self, "get_or_add_%s" % name)()
         element.val = value
 
 
 class CT_Underline(BaseOxmlElement):
     """`<w:u>` element, specifying the underlining style for a run."""
 
-    val: WD_UNDERLINE | None = (
-        OptionalAttribute(  # pyright: ignore[reportGeneralTypeIssues]
-            "w:val", WD_UNDERLINE
-        )
+    val: WD_UNDERLINE | None = OptionalAttribute(  # pyright: ignore[reportAssignmentType]
+        "w:val", WD_UNDERLINE
     )
 
 
 class CT_VerticalAlignRun(BaseOxmlElement):
     """`<w:vertAlign>` element, specifying subscript or superscript."""
 
     val: str = RequiredAttribute(  # pyright: ignore[reportGeneralTypeIssues]
```

### Comparing `python_docx-1.1.1/src/docx/oxml/text/hyperlink.py` & `python_docx-1.1.2/src/docx/oxml/text/hyperlink.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/oxml/text/pagebreak.py` & `python_docx-1.1.2/src/docx/oxml/text/pagebreak.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/oxml/text/paragraph.py` & `python_docx-1.1.2/src/docx/oxml/text/paragraph.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/oxml/text/parfmt.py` & `python_docx-1.1.2/src/docx/oxml/text/parfmt.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/oxml/text/run.py` & `python_docx-1.1.2/src/docx/oxml/text/run.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/oxml/xmlchemy.py` & `python_docx-1.1.2/src/docx/oxml/xmlchemy.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/package.py` & `python_docx-1.1.2/src/docx/package.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """WordprocessingML Package class and related objects."""
 
 from __future__ import annotations
 
-from typing import IO
+from typing import IO, cast
 
 from docx.image.image import Image
 from docx.opc.constants import RELATIONSHIP_TYPE as RT
 from docx.opc.package import OpcPackage
 from docx.opc.packuri import PackURI
 from docx.parts.image import ImagePart
 from docx.shared import lazyproperty
@@ -40,72 +40,71 @@
         for rel in self.iter_rels():
             if rel.is_external:
                 continue
             if rel.reltype != RT.IMAGE:
                 continue
             if rel.target_part in self.image_parts:
                 continue
-            self.image_parts.append(rel.target_part)
+            self.image_parts.append(cast("ImagePart", rel.target_part))
 
 
 class ImageParts:
     """Collection of |ImagePart| objects corresponding to images in the package."""
 
     def __init__(self):
-        self._image_parts = []
+        self._image_parts: list[ImagePart] = []
 
-    def __contains__(self, item):
+    def __contains__(self, item: object):
         return self._image_parts.__contains__(item)
 
     def __iter__(self):
         return self._image_parts.__iter__()
 
     def __len__(self):
         return self._image_parts.__len__()
 
-    def append(self, item):
+    def append(self, item: ImagePart):
         self._image_parts.append(item)
 
     def get_or_add_image_part(self, image_descriptor: str | IO[bytes]) -> ImagePart:
         """Return |ImagePart| object containing image identified by `image_descriptor`.
 
         The image-part is newly created if a matching one is not present in the
         collection.
         """
         image = Image.from_file(image_descriptor)
         matching_image_part = self._get_by_sha1(image.sha1)
         if matching_image_part is not None:
             return matching_image_part
         return self._add_image_part(image)
 
-    def _add_image_part(self, image):
-        """Return an |ImagePart| instance newly created from image and appended to the
-        collection."""
+    def _add_image_part(self, image: Image):
+        """Return |ImagePart| instance newly created from `image` and appended to the collection."""
         partname = self._next_image_partname(image.ext)
         image_part = ImagePart.from_image(image, partname)
         self.append(image_part)
         return image_part
 
-    def _get_by_sha1(self, sha1):
+    def _get_by_sha1(self, sha1: str) -> ImagePart | None:
         """Return the image part in this collection having a SHA1 hash matching `sha1`,
         or |None| if not found."""
         for image_part in self._image_parts:
             if image_part.sha1 == sha1:
                 return image_part
         return None
 
-    def _next_image_partname(self, ext):
+    def _next_image_partname(self, ext: str) -> PackURI:
         """The next available image partname, starting from ``/word/media/image1.{ext}``
         where unused numbers are reused.
 
         The partname is unique by number, without regard to the extension. `ext` does
         not include the leading period.
         """
 
-        def image_partname(n):
+        def image_partname(n: int) -> PackURI:
             return PackURI("/word/media/image%d.%s" % (n, ext))
 
         used_numbers = [image_part.partname.idx for image_part in self]
         for n in range(1, len(self) + 1):
             if n not in used_numbers:
                 return image_partname(n)
         return image_partname(len(self) + 1)
```

### Comparing `python_docx-1.1.1/src/docx/parts/document.py` & `python_docx-1.1.2/src/docx/parts/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """|DocumentPart| and closely related objects."""
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, cast
+from typing import IO, TYPE_CHECKING, cast
 
 from docx.document import Document
 from docx.enum.style import WD_STYLE_TYPE
 from docx.opc.constants import RELATIONSHIP_TYPE as RT
 from docx.parts.hdrftr import FooterPart, HeaderPart
 from docx.parts.numbering import NumberingPart
 from docx.parts.settings import SettingsPart
 from docx.parts.story import StoryPart
 from docx.parts.styles import StylesPart
 from docx.shape import InlineShapes
 from docx.shared import lazyproperty
 
 if TYPE_CHECKING:
     from docx.opc.coreprops import CoreProperties
+    from docx.settings import Settings
     from docx.styles.style import BaseStyle
 
 
 class DocumentPart(StoryPart):
     """Main document part of a WordprocessingML (WML) package, aka a .docx file.
 
     Acts as broker to other parts such as image, core properties, and style parts. It
@@ -97,40 +98,40 @@
         try:
             return self.part_related_by(RT.NUMBERING)
         except KeyError:
             numbering_part = NumberingPart.new()
             self.relate_to(numbering_part, RT.NUMBERING)
             return numbering_part
 
-    def save(self, path_or_stream):
+    def save(self, path_or_stream: str | IO[bytes]):
         """Save this document to `path_or_stream`, which can be either a path to a
         filesystem location (a string) or a file-like object."""
         self.package.save(path_or_stream)
 
     @property
-    def settings(self):
+    def settings(self) -> Settings:
         """A |Settings| object providing access to the settings in the settings part of
         this document."""
         return self._settings_part.settings
 
     @property
     def styles(self):
         """A |Styles| object providing access to the styles in the styles part of this
         document."""
         return self._styles_part.styles
 
     @property
-    def _settings_part(self):
+    def _settings_part(self) -> SettingsPart:
         """A |SettingsPart| object providing access to the document-level settings for
         this document.
 
         Creates a default settings part if one is not present.
         """
         try:
-            return self.part_related_by(RT.SETTINGS)
+            return cast(SettingsPart, self.part_related_by(RT.SETTINGS))
         except KeyError:
             settings_part = SettingsPart.default(self.package)
             self.relate_to(settings_part, RT.SETTINGS)
             return settings_part
 
     @property
     def _styles_part(self) -> StylesPart:
```

### Comparing `python_docx-1.1.1/src/docx/parts/hdrftr.py` & `python_docx-1.1.2/src/docx/parts/hdrftr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 """Header and footer part objects."""
 
+from __future__ import annotations
+
 import os
+from typing import TYPE_CHECKING
 
 from docx.opc.constants import CONTENT_TYPE as CT
 from docx.oxml.parser import parse_xml
 from docx.parts.story import StoryPart
 
+if TYPE_CHECKING:
+    from docx.package import Package
+
 
 class FooterPart(StoryPart):
     """Definition of a section footer."""
 
     @classmethod
-    def new(cls, package):
+    def new(cls, package: Package):
         """Return newly created footer part."""
         partname = package.next_partname("/word/footer%d.xml")
         content_type = CT.WML_FOOTER
         element = parse_xml(cls._default_footer_xml())
         return cls(partname, content_type, element, package)
 
     @classmethod
     def _default_footer_xml(cls):
         """Return bytes containing XML for a default footer part."""
-        path = os.path.join(
-            os.path.split(__file__)[0], "..", "templates", "default-footer.xml"
-        )
+        path = os.path.join(os.path.split(__file__)[0], "..", "templates", "default-footer.xml")
         with open(path, "rb") as f:
             xml_bytes = f.read()
         return xml_bytes
 
 
 class HeaderPart(StoryPart):
     """Definition of a section header."""
 
     @classmethod
-    def new(cls, package):
+    def new(cls, package: Package):
         """Return newly created header part."""
         partname = package.next_partname("/word/header%d.xml")
         content_type = CT.WML_HEADER
         element = parse_xml(cls._default_header_xml())
         return cls(partname, content_type, element, package)
 
     @classmethod
     def _default_header_xml(cls):
         """Return bytes containing XML for a default header part."""
-        path = os.path.join(
-            os.path.split(__file__)[0], "..", "templates", "default-header.xml"
-        )
+        path = os.path.join(os.path.split(__file__)[0], "..", "templates", "default-header.xml")
         with open(path, "rb") as f:
             xml_bytes = f.read()
         return xml_bytes
```

### Comparing `python_docx-1.1.1/src/docx/parts/image.py` & `python_docx-1.1.2/src/docx/parts/image.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 """The proxy class for an image part, and related objects."""
 
 from __future__ import annotations
 
 import hashlib
+from typing import TYPE_CHECKING
 
 from docx.image.image import Image
 from docx.opc.part import Part
 from docx.shared import Emu, Inches
 
+if TYPE_CHECKING:
+    from docx.opc.package import OpcPackage
+    from docx.opc.packuri import PackURI
+
 
 class ImagePart(Part):
     """An image part.
 
     Corresponds to the target part of a relationship with type RELATIONSHIP_TYPE.IMAGE.
     """
 
     def __init__(
-        self, partname: str, content_type: str, blob: bytes, image: Image | None = None
+        self, partname: PackURI, content_type: str, blob: bytes, image: Image | None = None
     ):
         super(ImagePart, self).__init__(partname, content_type, blob)
         self._image = image
 
     @property
     def default_cx(self):
         """Native width of this image, calculated from its width in pixels and
@@ -32,15 +37,15 @@
 
     @property
     def default_cy(self):
         """Native height of this image, calculated from its height in pixels and
         vertical dots per inch (dpi)."""
         px_height = self.image.px_height
         horz_dpi = self.image.horz_dpi
-        height_in_emu = 914400 * px_height / horz_dpi
+        height_in_emu = int(round(914400 * px_height / horz_dpi))
         return Emu(height_in_emu)
 
     @property
     def filename(self):
         """Filename from which this image part was originally created.
 
         A generic name, e.g. 'image.png', is substituted if no name is available, for
@@ -48,28 +53,28 @@
         extension is applied based on the detected MIME type of the image.
         """
         if self._image is not None:
             return self._image.filename
         return "image.%s" % self.partname.ext
 
     @classmethod
-    def from_image(cls, image, partname):
+    def from_image(cls, image: Image, partname: PackURI):
         """Return an |ImagePart| instance newly created from `image` and assigned
         `partname`."""
         return ImagePart(partname, image.content_type, image.blob, image)
 
     @property
     def image(self) -> Image:
         if self._image is None:
             self._image = Image.from_blob(self.blob)
         return self._image
 
     @classmethod
-    def load(cls, partname, content_type, blob, package):
+    def load(cls, partname: PackURI, content_type: str, blob: bytes, package: OpcPackage):
         """Called by ``docx.opc.package.PartFactory`` to load an image part from a
         package being opened by ``Document(...)`` call."""
         return cls(partname, content_type, blob)
 
     @property
     def sha1(self):
         """SHA1 hash digest of the blob of this image part."""
-        return hashlib.sha1(self._blob).hexdigest()
+        return hashlib.sha1(self.blob).hexdigest()
```

### Comparing `python_docx-1.1.1/src/docx/parts/numbering.py` & `python_docx-1.1.2/src/docx/parts/numbering.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/parts/settings.py` & `python_docx-1.1.2/src/docx/parts/settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,51 @@
 """|SettingsPart| and closely related objects."""
 
+from __future__ import annotations
+
 import os
+from typing import TYPE_CHECKING, cast
 
 from docx.opc.constants import CONTENT_TYPE as CT
 from docx.opc.packuri import PackURI
 from docx.opc.part import XmlPart
 from docx.oxml.parser import parse_xml
 from docx.settings import Settings
 
+if TYPE_CHECKING:
+    from docx.oxml.settings import CT_Settings
+    from docx.package import Package
+
 
 class SettingsPart(XmlPart):
     """Document-level settings part of a WordprocessingML (WML) package."""
 
+    def __init__(
+        self, partname: PackURI, content_type: str, element: CT_Settings, package: Package
+    ):
+        super().__init__(partname, content_type, element, package)
+        self._settings = element
+
     @classmethod
-    def default(cls, package):
+    def default(cls, package: Package):
         """Return a newly created settings part, containing a default `w:settings`
         element tree."""
         partname = PackURI("/word/settings.xml")
         content_type = CT.WML_SETTINGS
-        element = parse_xml(cls._default_settings_xml())
+        element = cast("CT_Settings", parse_xml(cls._default_settings_xml()))
         return cls(partname, content_type, element, package)
 
     @property
-    def settings(self):
-        """A |Settings| proxy object for the `w:settings` element in this part,
-        containing the document-level settings for this document."""
-        return Settings(self.element)
+    def settings(self) -> Settings:
+        """A |Settings| proxy object for the `w:settings` element in this part.
+
+        Contains the document-level settings for this document.
+        """
+        return Settings(self._settings)
 
     @classmethod
     def _default_settings_xml(cls):
         """Return a bytestream containing XML for a default settings part."""
-        path = os.path.join(
-            os.path.split(__file__)[0], "..", "templates", "default-settings.xml"
-        )
+        path = os.path.join(os.path.split(__file__)[0], "..", "templates", "default-settings.xml")
         with open(path, "rb") as f:
             xml_bytes = f.read()
         return xml_bytes
```

### Comparing `python_docx-1.1.1/src/docx/parts/story.py` & `python_docx-1.1.2/src/docx/parts/story.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """|StoryPart| and related objects."""
 
 from __future__ import annotations
 
-from typing import IO, TYPE_CHECKING, Tuple
+from typing import IO, TYPE_CHECKING, Tuple, cast
 
 from docx.opc.constants import RELATIONSHIP_TYPE as RT
 from docx.opc.part import XmlPart
 from docx.oxml.shape import CT_Inline
 from docx.shared import Length, lazyproperty
 
 if TYPE_CHECKING:
@@ -56,16 +56,16 @@
         wrong type or names a style not present in the document.
         """
         return self._document_part.get_style_id(style_or_name, style_type)
 
     def new_pic_inline(
         self,
         image_descriptor: str | IO[bytes],
-        width: Length | None = None,
-        height: Length | None = None,
+        width: int | Length | None = None,
+        height: int | Length | None = None,
     ) -> CT_Inline:
         """Return a newly-created `w:inline` element.
 
         The element contains the image specified by `image_descriptor` and is scaled
         based on the values of `width` and `height`.
         """
         rId, image = self.get_or_add_image(image_descriptor)
@@ -88,8 +88,8 @@
         return max(used_ids) + 1
 
     @lazyproperty
     def _document_part(self) -> DocumentPart:
         """|DocumentPart| object for this package."""
         package = self.package
         assert package is not None
-        return package.main_document_part
+        return cast("DocumentPart", package.main_document_part)
```

### Comparing `python_docx-1.1.1/src/docx/parts/styles.py` & `python_docx-1.1.2/src/docx/parts/styles.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/section.py` & `python_docx-1.1.2/src/docx/section.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,19 +156,15 @@
 
     def iter_inner_content(self) -> Iterator[Paragraph | Table]:
         """Generate each Paragraph or Table object in this `section`.
 
         Items appear in document order.
         """
         for element in self._sectPr.iter_inner_content():
-            yield (
-                Paragraph(element, self)  # pyright: ignore[reportGeneralTypeIssues]
-                if isinstance(element, CT_P)
-                else Table(element, self)
-            )
+            yield (Paragraph(element, self) if isinstance(element, CT_P) else Table(element, self))
 
     @property
     def left_margin(self) -> Length | None:
         """|Length| object representing the left margin for all pages in this section in
         English Metric Units."""
         return self._sectPr.left_margin
 
@@ -265,20 +261,18 @@
 
     def __init__(self, document_elm: CT_Document, document_part: DocumentPart):
         super(Sections, self).__init__()
         self._document_elm = document_elm
         self._document_part = document_part
 
     @overload
-    def __getitem__(self, key: int) -> Section:
-        ...
+    def __getitem__(self, key: int) -> Section: ...
 
     @overload
-    def __getitem__(self, key: slice) -> List[Section]:
-        ...
+    def __getitem__(self, key: slice) -> List[Section]: ...
 
     def __getitem__(self, key: int | slice) -> Section | List[Section]:
         if isinstance(key, slice):
             return [
                 Section(sectPr, self._document_part)
                 for sectPr in self._document_elm.sectPr_lst[key]
             ]
```

### Comparing `python_docx-1.1.1/src/docx/settings.py` & `python_docx-1.1.2/src/docx/settings.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,35 @@
 """Settings object, providing access to document-level settings."""
 
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, cast
+
 from docx.shared import ElementProxy
 
+if TYPE_CHECKING:
+    import docx.types as t
+    from docx.oxml.settings import CT_Settings
+    from docx.oxml.xmlchemy import BaseOxmlElement
+
 
 class Settings(ElementProxy):
     """Provides access to document-level settings for a document.
 
     Accessed using the :attr:`.Document.settings` property.
     """
 
+    def __init__(self, element: BaseOxmlElement, parent: t.ProvidesXmlPart | None = None):
+        super().__init__(element, parent)
+        self._settings = cast("CT_Settings", element)
+
     @property
-    def odd_and_even_pages_header_footer(self):
+    def odd_and_even_pages_header_footer(self) -> bool:
         """True if this document has distinct odd and even page headers and footers.
 
         Read/write.
         """
-        return self._element.evenAndOddHeaders_val
+        return self._settings.evenAndOddHeaders_val
 
     @odd_and_even_pages_header_footer.setter
-    def odd_and_even_pages_header_footer(self, value):
-        self._element.evenAndOddHeaders_val = value
+    def odd_and_even_pages_header_footer(self, value: bool):
+        self._settings.evenAndOddHeaders_val = value
```

### Comparing `python_docx-1.1.1/src/docx/shape.py` & `python_docx-1.1.2/src/docx/shape.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 """Objects related to shapes.
 
 A shape is a visual object that appears on the drawing layer of a document.
 """
 
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
 from docx.enum.shape import WD_INLINE_SHAPE
 from docx.oxml.ns import nsmap
 from docx.shared import Parented
 
+if TYPE_CHECKING:
+    from docx.oxml.document import CT_Body
+    from docx.oxml.shape import CT_Inline
+    from docx.parts.story import StoryPart
+    from docx.shared import Length
+
 
 class InlineShapes(Parented):
-    """Sequence of |InlineShape| instances, supporting len(), iteration, and indexed
-    access."""
+    """Sequence of |InlineShape| instances, supporting len(), iteration, and indexed access."""
 
-    def __init__(self, body_elm, parent):
+    def __init__(self, body_elm: CT_Body, parent: StoryPart):
         super(InlineShapes, self).__init__(parent)
         self._body = body_elm
 
-    def __getitem__(self, idx):
+    def __getitem__(self, idx: int):
         """Provide indexed access, e.g. 'inline_shapes[idx]'."""
         try:
             inline = self._inline_lst[idx]
         except IndexError:
             msg = "inline shape index [%d] out of range" % idx
             raise IndexError(msg)
+
         return InlineShape(inline)
 
     def __iter__(self):
         return (InlineShape(inline) for inline in self._inline_lst)
 
     def __len__(self):
         return len(self._inline_lst)
@@ -38,28 +48,28 @@
         return body.xpath(xpath)
 
 
 class InlineShape:
     """Proxy for an ``<wp:inline>`` element, representing the container for an inline
     graphical object."""
 
-    def __init__(self, inline):
+    def __init__(self, inline: CT_Inline):
         super(InlineShape, self).__init__()
         self._inline = inline
 
     @property
-    def height(self):
+    def height(self) -> Length:
         """Read/write.
 
         The display height of this inline shape as an |Emu| instance.
         """
         return self._inline.extent.cy
 
     @height.setter
-    def height(self, cy):
+    def height(self, cy: Length):
         self._inline.extent.cy = cy
         self._inline.graphic.graphicData.pic.spPr.cy = cy
 
     @property
     def type(self):
         """The type of this inline shape as a member of
         ``docx.enum.shape.WD_INLINE_SHAPE``, e.g. ``LINKED_PICTURE``.
@@ -84,10 +94,10 @@
         """Read/write.
 
         The display width of this inline shape as an |Emu| instance.
         """
         return self._inline.extent.cx
 
     @width.setter
-    def width(self, cx):
+    def width(self, cx: Length):
         self._inline.extent.cx = cx
         self._inline.graphic.graphicData.pic.spPr.cx = cx
```

### Comparing `python_docx-1.1.1/src/docx/shared.py` & `python_docx-1.1.2/src/docx/shared.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/styles/__init__.py` & `python_docx-1.1.2/src/docx/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/styles/latent.py` & `python_docx-1.1.2/src/docx/styles/latent.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/styles/style.py` & `python_docx-1.1.2/src/docx/styles/style.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/styles/styles.py` & `python_docx-1.1.2/src/docx/styles/styles.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/table.py` & `python_docx-1.1.2/src/docx/table.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/templates/default-docx-template/[Content_Types].xml` & `python_docx-1.1.2/src/docx/templates/default-docx-template/[Content_Types].xml`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/templates/default-docx-template/_rels/.rels` & `python_docx-1.1.2/src/docx/templates/default-docx-template/_rels/.rels`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/templates/default-docx-template/docProps/app.xml` & `python_docx-1.1.2/src/docx/templates/default-docx-template/docProps/app.xml`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/templates/default-docx-template/docProps/core.xml` & `python_docx-1.1.2/src/docx/templates/default-docx-template/docProps/core.xml`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/templates/default-docx-template/docProps/thumbnail.jpeg` & `python_docx-1.1.2/src/docx/templates/default-docx-template/docProps/thumbnail.jpeg`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/templates/default-docx-template/word/_rels/document.xml.rels` & `python_docx-1.1.2/src/docx/templates/default-docx-template/word/_rels/document.xml.rels`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/templates/default-docx-template/word/document.xml` & `python_docx-1.1.2/src/docx/templates/default-docx-template/word/document.xml`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/templates/default-docx-template/word/fontTable.xml` & `python_docx-1.1.2/src/docx/templates/default-docx-template/word/fontTable.xml`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/templates/default-docx-template/word/numbering.xml` & `python_docx-1.1.2/src/docx/templates/default-docx-template/word/numbering.xml`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/templates/default-docx-template/word/settings.xml` & `python_docx-1.1.2/src/docx/templates/default-docx-template/word/settings.xml`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/templates/default-docx-template/word/styles.xml` & `python_docx-1.1.2/src/docx/templates/default-docx-template/word/styles.xml`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/templates/default-docx-template/word/stylesWithEffects.xml` & `python_docx-1.1.2/src/docx/templates/default-docx-template/word/stylesWithEffects.xml`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/templates/default-docx-template/word/theme/theme1.xml` & `python_docx-1.1.2/src/docx/templates/default-docx-template/word/theme/theme1.xml`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/templates/default-footer.xml` & `python_docx-1.1.2/src/docx/templates/default-footer.xml`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/templates/default-header.xml` & `python_docx-1.1.2/src/docx/templates/default-header.xml`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/templates/default-settings.xml` & `python_docx-1.1.2/src/docx/templates/default-settings.xml`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/templates/default-styles.xml` & `python_docx-1.1.2/src/docx/templates/default-styles.xml`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/templates/default.docx` & `python_docx-1.1.2/src/docx/templates/default.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/text/font.py` & `python_docx-1.1.2/src/docx/text/font.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/text/hyperlink.py` & `python_docx-1.1.2/src/docx/text/hyperlink.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/text/pagebreak.py` & `python_docx-1.1.2/src/docx/text/pagebreak.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/text/paragraph.py` & `python_docx-1.1.2/src/docx/text/paragraph.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/text/parfmt.py` & `python_docx-1.1.2/src/docx/text/parfmt.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/text/run.py` & `python_docx-1.1.2/src/docx/text/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,16 +55,16 @@
             br.type = type_
         if clear is not None:
             br.clear = clear
 
     def add_picture(
         self,
         image_path_or_stream: str | IO[bytes],
-        width: Length | None = None,
-        height: Length | None = None,
+        width: int | Length | None = None,
+        height: int | Length | None = None,
     ) -> InlineShape:
         """Return |InlineShape| containing image identified by `image_path_or_stream`.
 
         The picture is added to the end of this run.
 
         `image_path_or_stream` can be a path (a string) or a file-like object containing
         a binary image.
```

### Comparing `python_docx-1.1.1/src/docx/text/tabstops.py` & `python_docx-1.1.2/src/docx/text/tabstops.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/docx/types.py` & `python_docx-1.1.2/src/docx/types.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/src/python_docx.egg-info/PKG-INFO` & `python_docx-1.1.2/src/python_docx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-docx
-Version: 1.1.1
+Version: 1.1.2
 Summary: Create, read, and update Microsoft Word .docx files.
 Author-email: Steve Canny <stcanny@gmail.com>
 License: MIT
 Project-URL: Changelog, https://github.com/python-openxml/python-docx/blob/master/HISTORY.rst
 Project-URL: Documentation, https://python-docx.readthedocs.org/en/latest/
 Project-URL: Homepage, https://github.com/python-openxml/python-docx
 Project-URL: Repository, https://github.com/python-openxml/python-docx
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Office/Business :: Office Suites
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: lxml<=4.9.2,>=3.1.0
+Requires-Dist: lxml>=3.1.0
 Requires-Dist: typing_extensions>=4.9.0
 
 # python-docx
 
 *python-docx* is a Python library for reading, creating, and updating Microsoft Word 2007+ (.docx) files.
 
 ## Installation
```

### Comparing `python_docx-1.1.1/src/python_docx.egg-info/SOURCES.txt` & `python_docx-1.1.2/src/python_docx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/dml/test_color.py` & `python_docx-1.1.2/tests/dml/test_color.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/image/test_bmp.py` & `python_docx-1.1.2/tests/image/test_bmp.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/image/test_gif.py` & `python_docx-1.1.2/tests/image/test_gif.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/image/test_helpers.py` & `python_docx-1.1.2/tests/image/test_helpers.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/image/test_image.py` & `python_docx-1.1.2/tests/image/test_image.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/image/test_jpeg.py` & `python_docx-1.1.2/tests/image/test_jpeg.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/image/test_png.py` & `python_docx-1.1.2/tests/image/test_png.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/image/test_tiff.py` & `python_docx-1.1.2/tests/image/test_tiff.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/opc/test_coreprops.py` & `python_docx-1.1.2/tests/opc/test_coreprops.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,192 +1,188 @@
+# pyright: reportPrivateUsage=false
+
 """Unit test suite for the docx.opc.coreprops module."""
 
-from datetime import datetime
+from __future__ import annotations
+
+import datetime as dt
+from typing import TYPE_CHECKING, cast
 
 import pytest
 
 from docx.opc.coreprops import CoreProperties
 from docx.oxml.parser import parse_xml
 
+if TYPE_CHECKING:
+    from docx.oxml.coreprops import CT_CoreProperties
+
 
 class DescribeCoreProperties:
-    def it_knows_the_string_property_values(self, text_prop_get_fixture):
-        core_properties, prop_name, expected_value = text_prop_get_fixture
+    """Unit-test suite for `docx.opc.coreprops.CoreProperties` objects."""
+
+    @pytest.mark.parametrize(
+        ("prop_name", "expected_value"),
+        [
+            ("author", "python-docx"),
+            ("category", ""),
+            ("comments", ""),
+            ("content_status", "DRAFT"),
+            ("identifier", "GXS 10.2.1ab"),
+            ("keywords", "foo bar baz"),
+            ("language", "US-EN"),
+            ("last_modified_by", "Steve Canny"),
+            ("subject", "Spam"),
+            ("title", "Word Document"),
+            ("version", "1.2.88"),
+        ],
+    )
+    def it_knows_the_string_property_values(
+        self, prop_name: str, expected_value: str, core_properties: CoreProperties
+    ):
         actual_value = getattr(core_properties, prop_name)
         assert actual_value == expected_value
 
-    def it_can_change_the_string_property_values(self, text_prop_set_fixture):
-        core_properties, prop_name, value, expected_xml = text_prop_set_fixture
-        setattr(core_properties, prop_name, value)
-        assert core_properties._element.xml == expected_xml
-
-    def it_knows_the_date_property_values(self, date_prop_get_fixture):
-        core_properties, prop_name, expected_datetime = date_prop_get_fixture
-        actual_datetime = getattr(core_properties, prop_name)
-        assert actual_datetime == expected_datetime
+    @pytest.mark.parametrize(
+        ("prop_name", "tagname", "value"),
+        [
+            ("author", "dc:creator", "scanny"),
+            ("category", "cp:category", "silly stories"),
+            ("comments", "dc:description", "Bar foo to you"),
+            ("content_status", "cp:contentStatus", "FINAL"),
+            ("identifier", "dc:identifier", "GT 5.2.xab"),
+            ("keywords", "cp:keywords", "dog cat moo"),
+            ("language", "dc:language", "GB-EN"),
+            ("last_modified_by", "cp:lastModifiedBy", "Billy Bob"),
+            ("subject", "dc:subject", "Eggs"),
+            ("title", "dc:title", "Dissertation"),
+            ("version", "cp:version", "81.2.8"),
+        ],
+    )
+    def it_can_change_the_string_property_values(self, prop_name: str, tagname: str, value: str):
+        coreProperties = self.coreProperties(tagname="", str_val="")
+        core_properties = CoreProperties(cast("CT_CoreProperties", parse_xml(coreProperties)))
 
-    def it_can_change_the_date_property_values(self, date_prop_set_fixture):
-        core_properties, prop_name, value, expected_xml = date_prop_set_fixture
         setattr(core_properties, prop_name, value)
-        assert core_properties._element.xml == expected_xml
-
-    def it_knows_the_revision_number(self, revision_get_fixture):
-        core_properties, expected_revision = revision_get_fixture
-        assert core_properties.revision == expected_revision
-
-    def it_can_change_the_revision_number(self, revision_set_fixture):
-        core_properties, revision, expected_xml = revision_set_fixture
-        core_properties.revision = revision
-        assert core_properties._element.xml == expected_xml
 
-    # fixtures -------------------------------------------------------
+        assert core_properties._element.xml == self.coreProperties(tagname, value)
 
-    @pytest.fixture(
-        params=[
-            ("created", datetime(2012, 11, 17, 16, 37, 40)),
-            ("last_printed", datetime(2014, 6, 4, 4, 28)),
+    @pytest.mark.parametrize(
+        ("prop_name", "expected_datetime"),
+        [
+            ("created", dt.datetime(2012, 11, 17, 16, 37, 40, tzinfo=dt.timezone.utc)),
+            ("last_printed", dt.datetime(2014, 6, 4, 4, 28, tzinfo=dt.timezone.utc)),
             ("modified", None),
-        ]
+        ],
     )
-    def date_prop_get_fixture(self, request, core_properties):
-        prop_name, expected_datetime = request.param
-        return core_properties, prop_name, expected_datetime
+    def it_knows_the_date_property_values(
+        self, prop_name: str, expected_datetime: dt.datetime, core_properties: CoreProperties
+    ):
+        actual_datetime = getattr(core_properties, prop_name)
+        assert actual_datetime == expected_datetime
 
-    @pytest.fixture(
-        params=[
+    @pytest.mark.parametrize(
+        ("prop_name", "tagname", "value", "str_val", "attrs"),
+        [
             (
                 "created",
                 "dcterms:created",
-                datetime(2001, 2, 3, 4, 5),
+                dt.datetime(2001, 2, 3, 4, 5),
                 "2001-02-03T04:05:00Z",
                 ' xsi:type="dcterms:W3CDTF"',
             ),
             (
                 "last_printed",
                 "cp:lastPrinted",
-                datetime(2014, 6, 4, 4),
+                dt.datetime(2014, 6, 4, 4),
                 "2014-06-04T04:00:00Z",
                 "",
             ),
             (
                 "modified",
                 "dcterms:modified",
-                datetime(2005, 4, 3, 2, 1),
+                dt.datetime(2005, 4, 3, 2, 1),
                 "2005-04-03T02:01:00Z",
                 ' xsi:type="dcterms:W3CDTF"',
             ),
-        ]
+        ],
     )
-    def date_prop_set_fixture(self, request):
-        prop_name, tagname, value, str_val, attrs = request.param
-        coreProperties = self.coreProperties(None, None)
-        core_properties = CoreProperties(parse_xml(coreProperties))
+    def it_can_change_the_date_property_values(
+        self, prop_name: str, tagname: str, value: dt.datetime, str_val: str, attrs: str
+    ):
+        coreProperties = self.coreProperties(tagname="", str_val="")
+        core_properties = CoreProperties(cast("CT_CoreProperties", parse_xml(coreProperties)))
         expected_xml = self.coreProperties(tagname, str_val, attrs)
-        return core_properties, prop_name, value, expected_xml
 
-    @pytest.fixture(
-        params=[("42", 42), (None, 0), ("foobar", 0), ("-17", 0), ("32.7", 0)]
-    )
-    def revision_get_fixture(self, request):
-        str_val, expected_revision = request.param
-        tagname = "" if str_val is None else "cp:revision"
-        coreProperties = self.coreProperties(tagname, str_val)
-        core_properties = CoreProperties(parse_xml(coreProperties))
-        return core_properties, expected_revision
-
-    @pytest.fixture(
-        params=[
-            (42, "42"),
-        ]
-    )
-    def revision_set_fixture(self, request):
-        value, str_val = request.param
-        coreProperties = self.coreProperties(None, None)
-        core_properties = CoreProperties(parse_xml(coreProperties))
+        setattr(core_properties, prop_name, value)
+
+        assert core_properties._element.xml == expected_xml
+
+    @pytest.mark.parametrize(
+        ("str_val", "expected_value"),
+        [("42", 42), (None, 0), ("foobar", 0), ("-17", 0), ("32.7", 0)],
+    )
+    def it_knows_the_revision_number(self, str_val: str | None, expected_value: int):
+        tagname, str_val = ("cp:revision", str_val) if str_val else ("", "")
+        coreProperties = self.coreProperties(tagname, str_val or "")
+        core_properties = CoreProperties(cast("CT_CoreProperties", parse_xml(coreProperties)))
+
+        assert core_properties.revision == expected_value
+
+    @pytest.mark.parametrize(("value", "str_val"), [(42, "42")])
+    def it_can_change_the_revision_number(self, value: int, str_val: str):
+        coreProperties = self.coreProperties(tagname="", str_val="")
+        core_properties = CoreProperties(cast("CT_CoreProperties", parse_xml(coreProperties)))
         expected_xml = self.coreProperties("cp:revision", str_val)
-        return core_properties, value, expected_xml
 
-    @pytest.fixture(
-        params=[
-            ("author", "python-docx"),
-            ("category", ""),
-            ("comments", ""),
-            ("content_status", "DRAFT"),
-            ("identifier", "GXS 10.2.1ab"),
-            ("keywords", "foo bar baz"),
-            ("language", "US-EN"),
-            ("last_modified_by", "Steve Canny"),
-            ("subject", "Spam"),
-            ("title", "Word Document"),
-            ("version", "1.2.88"),
-        ]
-    )
-    def text_prop_get_fixture(self, request, core_properties):
-        prop_name, expected_value = request.param
-        return core_properties, prop_name, expected_value
+        core_properties.revision = value
 
-    @pytest.fixture(
-        params=[
-            ("author", "dc:creator", "scanny"),
-            ("category", "cp:category", "silly stories"),
-            ("comments", "dc:description", "Bar foo to you"),
-            ("content_status", "cp:contentStatus", "FINAL"),
-            ("identifier", "dc:identifier", "GT 5.2.xab"),
-            ("keywords", "cp:keywords", "dog cat moo"),
-            ("language", "dc:language", "GB-EN"),
-            ("last_modified_by", "cp:lastModifiedBy", "Billy Bob"),
-            ("subject", "dc:subject", "Eggs"),
-            ("title", "dc:title", "Dissertation"),
-            ("version", "cp:version", "81.2.8"),
-        ]
-    )
-    def text_prop_set_fixture(self, request):
-        prop_name, tagname, value = request.param
-        coreProperties = self.coreProperties(None, None)
-        core_properties = CoreProperties(parse_xml(coreProperties))
-        expected_xml = self.coreProperties(tagname, value)
-        return core_properties, prop_name, value, expected_xml
+        assert core_properties._element.xml == expected_xml
 
-    # fixture components ---------------------------------------------
+    # fixtures -------------------------------------------------------
 
-    def coreProperties(self, tagname, str_val, attrs=""):
+    def coreProperties(self, tagname: str, str_val: str, attrs: str = "") -> str:
         tmpl = (
-            '<cp:coreProperties xmlns:cp="http://schemas.openxmlformats.org/'
-            'package/2006/metadata/core-properties" xmlns:dc="http://purl.or'
-            'g/dc/elements/1.1/" xmlns:dcmitype="http://purl.org/dc/dcmitype'
-            '/" xmlns:dcterms="http://purl.org/dc/terms/" xmlns:xsi="http://'
-            'www.w3.org/2001/XMLSchema-instance">%s</cp:coreProperties>\n'
+            "<cp:coreProperties"
+            ' xmlns:cp="http://schemas.openxmlformats.org/package/2006/metadata/core-properties"'
+            ' xmlns:dc="http://purl.org/dc/elements/1.1/"'
+            ' xmlns:dcmitype="http://purl.org/dc/dcmitype/"'
+            ' xmlns:dcterms="http://purl.org/dc/terms/"'
+            ' xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"'
+            ">%s</cp:coreProperties>\n"
         )
         if not tagname:
             child_element = ""
         elif not str_val:
             child_element = "\n  <%s%s/>\n" % (tagname, attrs)
         else:
             child_element = "\n  <%s%s>%s</%s>\n" % (tagname, attrs, str_val, tagname)
         return tmpl % child_element
 
     @pytest.fixture
     def core_properties(self):
-        element = parse_xml(
-            b"<?xml version='1.0' encoding='UTF-8' standalone='yes'?>"
-            b'\n<cp:coreProperties xmlns:cp="http://schemas.openxmlformats.o'
-            b'rg/package/2006/metadata/core-properties" xmlns:dc="http://pur'
-            b'l.org/dc/elements/1.1/" xmlns:dcmitype="http://purl.org/dc/dcm'
-            b'itype/" xmlns:dcterms="http://purl.org/dc/terms/" xmlns:xsi="h'
-            b'ttp://www.w3.org/2001/XMLSchema-instance">\n'
-            b"  <cp:contentStatus>DRAFT</cp:contentStatus>\n"
-            b"  <dc:creator>python-docx</dc:creator>\n"
-            b'  <dcterms:created xsi:type="dcterms:W3CDTF">2012-11-17T11:07:'
-            b"40-05:30</dcterms:created>\n"
-            b"  <dc:description/>\n"
-            b"  <dc:identifier>GXS 10.2.1ab</dc:identifier>\n"
-            b"  <dc:language>US-EN</dc:language>\n"
-            b"  <cp:lastPrinted>2014-06-04T04:28:00Z</cp:lastPrinted>\n"
-            b"  <cp:keywords>foo bar baz</cp:keywords>\n"
-            b"  <cp:lastModifiedBy>Steve Canny</cp:lastModifiedBy>\n"
-            b"  <cp:revision>4</cp:revision>\n"
-            b"  <dc:subject>Spam</dc:subject>\n"
-            b"  <dc:title>Word Document</dc:title>\n"
-            b"  <cp:version>1.2.88</cp:version>\n"
-            b"</cp:coreProperties>\n"
+        element = cast(
+            "CT_CoreProperties",
+            parse_xml(
+                b"<?xml version='1.0' encoding='UTF-8' standalone='yes'?>"
+                b'\n<cp:coreProperties xmlns:cp="http://schemas.openxmlformats.o'
+                b'rg/package/2006/metadata/core-properties" xmlns:dc="http://pur'
+                b'l.org/dc/elements/1.1/" xmlns:dcmitype="http://purl.org/dc/dcm'
+                b'itype/" xmlns:dcterms="http://purl.org/dc/terms/" xmlns:xsi="h'
+                b'ttp://www.w3.org/2001/XMLSchema-instance">\n'
+                b"  <cp:contentStatus>DRAFT</cp:contentStatus>\n"
+                b"  <dc:creator>python-docx</dc:creator>\n"
+                b'  <dcterms:created xsi:type="dcterms:W3CDTF">2012-11-17T11:07:'
+                b"40-05:30</dcterms:created>\n"
+                b"  <dc:description/>\n"
+                b"  <dc:identifier>GXS 10.2.1ab</dc:identifier>\n"
+                b"  <dc:language>US-EN</dc:language>\n"
+                b"  <cp:lastPrinted>2014-06-04T04:28:00Z</cp:lastPrinted>\n"
+                b"  <cp:keywords>foo bar baz</cp:keywords>\n"
+                b"  <cp:lastModifiedBy>Steve Canny</cp:lastModifiedBy>\n"
+                b"  <cp:revision>4</cp:revision>\n"
+                b"  <dc:subject>Spam</dc:subject>\n"
+                b"  <dc:title>Word Document</dc:title>\n"
+                b"  <cp:version>1.2.88</cp:version>\n"
+                b"</cp:coreProperties>\n"
+            ),
         )
         return CoreProperties(element)
```

### Comparing `python_docx-1.1.1/tests/opc/test_oxml.py` & `python_docx-1.1.2/tests/opc/test_oxml.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/opc/test_package.py` & `python_docx-1.1.2/tests/opc/test_package.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/opc/test_packuri.py` & `python_docx-1.1.2/tests/opc/test_packuri.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/opc/test_part.py` & `python_docx-1.1.2/tests/opc/test_part.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,107 +24,62 @@
     instance_mock,
     loose_mock,
     property_mock,
 )
 
 
 class DescribePart:
-    def it_can_be_constructed_by_PartFactory(
-        self, partname_, content_type_, blob_, package_, __init_
-    ):
-        part = Part.load(partname_, content_type_, blob_, package_)
+    """Unit-test suite for `docx.opc.part.Part` objects."""
 
-        __init_.assert_called_once_with(ANY, partname_, content_type_, blob_, package_)
+    def it_can_be_constructed_by_PartFactory(self, package_: Mock, init__: Mock):
+        part = Part.load(PackURI("/part/name"), "content/type", b"1be2", package_)
+
+        init__.assert_called_once_with(ANY, "/part/name", "content/type", b"1be2", package_)
         assert isinstance(part, Part)
 
-    def it_knows_its_partname(self, partname_get_fixture):
-        part, expected_partname = partname_get_fixture
-        assert part.partname == expected_partname
-
-    def it_can_change_its_partname(self, partname_set_fixture):
-        part, new_partname = partname_set_fixture
-        part.partname = new_partname
-        assert part.partname == new_partname
-
-    def it_knows_its_content_type(self, content_type_fixture):
-        part, expected_content_type = content_type_fixture
-        assert part.content_type == expected_content_type
-
-    def it_knows_the_package_it_belongs_to(self, package_get_fixture):
-        part, expected_package = package_get_fixture
-        assert part.package == expected_package
+    def it_knows_its_partname(self):
+        part = Part(PackURI("/part/name"), "content/type")
+        assert part.partname == "/part/name"
+
+    def it_can_change_its_partname(self):
+        part = Part(PackURI("/old/part/name"), "content/type")
+        part.partname = PackURI("/new/part/name")
+        assert part.partname == "/new/part/name"
+
+    def it_knows_its_content_type(self):
+        part = Part(PackURI("/part/name"), "content/type")
+        assert part.content_type == "content/type"
+
+    def it_knows_the_package_it_belongs_to(self, package_: Mock):
+        part = Part(PackURI("/part/name"), "content/type", package=package_)
+        assert part.package is package_
 
-    def it_can_be_notified_after_unmarshalling_is_complete(self, part):
+    def it_can_be_notified_after_unmarshalling_is_complete(self):
+        part = Part(PackURI("/part/name"), "content/type")
         part.after_unmarshal()
 
-    def it_can_be_notified_before_marshalling_is_started(self, part):
+    def it_can_be_notified_before_marshalling_is_started(self):
+        part = Part(PackURI("/part/name"), "content/type")
         part.before_marshal()
 
-    def it_uses_the_load_blob_as_its_blob(self, blob_fixture):
-        part, load_blob = blob_fixture
-        assert part.blob is load_blob
+    def it_uses_the_load_blob_as_its_blob(self):
+        blob = b"abcde"
+        part = Part(PackURI("/part/name"), "content/type", blob)
+        assert part.blob is blob
 
     # fixtures ---------------------------------------------
 
     @pytest.fixture
-    def blob_fixture(self, blob_):
-        part = Part(None, None, blob_, None)
-        return part, blob_
-
-    @pytest.fixture
-    def content_type_fixture(self):
-        content_type = "content/type"
-        part = Part(None, content_type, None, None)
-        return part, content_type
-
-    @pytest.fixture
-    def package_get_fixture(self, package_):
-        part = Part(None, None, None, package_)
-        return part, package_
-
-    @pytest.fixture
-    def part(self):
-        part = Part(None, None)
-        return part
-
-    @pytest.fixture
-    def partname_get_fixture(self):
-        partname = PackURI("/part/name")
-        part = Part(partname, None, None, None)
-        return part, partname
-
-    @pytest.fixture
-    def partname_set_fixture(self):
-        old_partname = PackURI("/old/part/name")
-        new_partname = PackURI("/new/part/name")
-        part = Part(old_partname, None, None, None)
-        return part, new_partname
-
-    # fixture components ---------------------------------------------
-
-    @pytest.fixture
-    def blob_(self, request):
-        return instance_mock(request, bytes)
-
-    @pytest.fixture
-    def content_type_(self, request):
-        return instance_mock(request, str)
-
-    @pytest.fixture
-    def __init_(self, request):
+    def init__(self, request: FixtureRequest):
         return initializer_mock(request, Part)
 
     @pytest.fixture
-    def package_(self, request):
+    def package_(self, request: FixtureRequest):
         return instance_mock(request, OpcPackage)
 
-    @pytest.fixture
-    def partname_(self, request):
-        return instance_mock(request, PackURI)
-
 
 class DescribePartRelationshipManagementInterface:
     """Unit-test suite for `docx.opc.package.Part` relationship behaviors."""
 
     def it_provides_access_to_its_relationships(
         self, Relationships_: Mock, partname_: Mock, rels_: Mock
     ):
@@ -165,32 +120,21 @@
         part = Part("partname", "content_type")
 
         rId = part.relate_to("https://hyper/link", "http://rel/type", is_external=True)
 
         rels_.get_or_add_ext_rel.assert_called_once_with("http://rel/type", "https://hyper/link")
         assert rId == "rId27"
 
-    @pytest.mark.parametrize(
-        ("part_cxml", "rel_should_be_dropped"),
-        [
-            ("w:p", True),
-            ("w:p/r:a{r:id=rId42}", True),
-            ("w:p/r:a{r:id=rId42}/r:b{r:id=rId42}", False),
-        ],
-    )
-    def it_can_drop_a_relationship(
-        self, part_cxml: str, rel_should_be_dropped: bool, rels_prop_: Mock
-    ):
+    def it_can_drop_a_relationship(self, rels_prop_: Mock):
         rels_prop_.return_value = {"rId42": None}
-        part = Part("partname", "content_type")
-        part._element = element(part_cxml)  # pyright: ignore[reportAttributeAccessIssue]
+        part = Part(PackURI("/partname"), "content_type")
 
         part.drop_rel("rId42")
 
-        assert ("rId42" not in part.rels) is rel_should_be_dropped
+        assert "rId42" not in part.rels
 
     def it_can_find_a_related_part_by_reltype(
         self, rels_prop_: Mock, rels_: Mock, other_part_: Mock
     ):
         rels_prop_.return_value = rels_
         rels_.part_with_reltype.return_value = other_part_
         part = Part("partname", "content_type")
@@ -407,14 +351,32 @@
         serialize_part_xml_.assert_called_once_with(element_)
         assert blob is serialize_part_xml_.return_value
 
     def it_knows_its_the_part_for_its_child_objects(self, part_fixture):
         xml_part = part_fixture
         assert xml_part.part is xml_part
 
+    @pytest.mark.parametrize(
+        ("part_cxml", "rel_should_be_dropped"),
+        [
+            ("w:p", True),
+            ("w:p/r:a{r:id=rId42}", True),
+            ("w:p/r:a{r:id=rId42}/r:b{r:id=rId42}", False),
+        ],
+    )
+    def it_only_drops_a_relationship_with_zero_reference_count(
+        self, part_cxml: str, rel_should_be_dropped: bool, rels_prop_: Mock, package_: Mock
+    ):
+        rels_prop_.return_value = {"rId42": None}
+        part = XmlPart(PackURI("/partname"), "content_type", element(part_cxml), package_)
+
+        part.drop_rel("rId42")
+
+        assert ("rId42" not in part.rels) is rel_should_be_dropped
+
     # fixtures -------------------------------------------------------
 
     @pytest.fixture
     def blob_fixture(self, request, element_, serialize_part_xml_):
         xml_part = XmlPart(None, None, element_, None)
         return xml_part, element_, serialize_part_xml_
 
@@ -449,9 +411,13 @@
         return function_mock(request, "docx.opc.part.parse_xml", return_value=element_)
 
     @pytest.fixture
     def partname_(self, request):
         return instance_mock(request, PackURI)
 
     @pytest.fixture
+    def rels_prop_(self, request: FixtureRequest):
+        return property_mock(request, XmlPart, "rels")
+
+    @pytest.fixture
     def serialize_part_xml_(self, request):
         return function_mock(request, "docx.opc.part.serialize_part_xml")
```

### Comparing `python_docx-1.1.1/tests/opc/test_phys_pkg.py` & `python_docx-1.1.2/tests/opc/test_phys_pkg.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/opc/test_pkgreader.py` & `python_docx-1.1.2/tests/opc/test_pkgreader.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/opc/test_pkgwriter.py` & `python_docx-1.1.2/tests/opc/test_pkgwriter.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/opc/test_rel.py` & `python_docx-1.1.2/tests/opc/test_rel.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/opc/unitdata/rels.py` & `python_docx-1.1.2/tests/opc/unitdata/rels.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/opc/unitdata/types.py` & `python_docx-1.1.2/tests/opc/unitdata/types.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/oxml/parts/test_document.py` & `python_docx-1.1.2/tests/oxml/parts/test_document.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/oxml/test__init__.py` & `python_docx-1.1.2/tests/oxml/test__init__.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/oxml/test_document.py` & `python_docx-1.1.2/tests/oxml/test_document.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/oxml/test_ns.py` & `python_docx-1.1.2/tests/oxml/test_ns.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/oxml/test_section.py` & `python_docx-1.1.2/tests/oxml/test_section.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/oxml/test_styles.py` & `python_docx-1.1.2/tests/oxml/test_styles.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/oxml/test_table.py` & `python_docx-1.1.2/tests/oxml/test_table.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/oxml/test_xmlchemy.py` & `python_docx-1.1.2/tests/oxml/test_xmlchemy.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/oxml/text/test_hyperlink.py` & `python_docx-1.1.2/tests/oxml/text/test_hyperlink.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/oxml/text/test_run.py` & `python_docx-1.1.2/tests/oxml/text/test_run.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/oxml/unitdata/dml.py` & `python_docx-1.1.2/tests/oxml/unitdata/dml.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/oxml/unitdata/section.py` & `python_docx-1.1.2/tests/oxml/unitdata/section.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/oxml/unitdata/shared.py` & `python_docx-1.1.2/tests/oxml/unitdata/shared.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/oxml/unitdata/text.py` & `python_docx-1.1.2/tests/oxml/unitdata/text.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/parts/test_document.py` & `python_docx-1.1.2/tests/parts/test_document.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/parts/test_hdrftr.py` & `python_docx-1.1.2/tests/parts/test_hdrftr.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/parts/test_image.py` & `python_docx-1.1.2/tests/parts/test_image.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/parts/test_numbering.py` & `python_docx-1.1.2/tests/parts/test_numbering.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/parts/test_settings.py` & `python_docx-1.1.2/tests/parts/test_settings.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/parts/test_story.py` & `python_docx-1.1.2/tests/parts/test_story.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/parts/test_styles.py` & `python_docx-1.1.2/tests/parts/test_styles.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/styles/test_latent.py` & `python_docx-1.1.2/tests/styles/test_latent.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/styles/test_style.py` & `python_docx-1.1.2/tests/styles/test_style.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/styles/test_styles.py` & `python_docx-1.1.2/tests/styles/test_styles.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_api.py` & `python_docx-1.1.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_blkcntnr.py` & `python_docx-1.1.2/tests/test_blkcntnr.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_document.py` & `python_docx-1.1.2/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_enum.py` & `python_docx-1.1.2/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/150-dpi.png` & `python_docx-1.1.2/tests/test_files/150-dpi.png`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/300-dpi.TIF` & `python_docx-1.1.2/tests/test_files/300-dpi.TIF`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/300-dpi.jpg` & `python_docx-1.1.2/tests/test_files/300-dpi.jpg`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/300-dpi.png` & `python_docx-1.1.2/tests/test_files/300-dpi.png`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/72-dpi.tiff` & `python_docx-1.1.2/tests/test_files/72-dpi.tiff`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/CVS_LOGO.WMF` & `python_docx-1.1.2/tests/test_files/CVS_LOGO.WMF`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/blk-inner-content.docx` & `python_docx-1.1.2/tests/test_files/blk-inner-content.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/exif-420-dpi.jpg` & `python_docx-1.1.2/tests/test_files/exif-420-dpi.jpg`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/expanded_docx/[Content_Types].xml` & `python_docx-1.1.2/tests/test_files/expanded_docx/[Content_Types].xml`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/expanded_docx/_rels/.rels` & `python_docx-1.1.2/tests/test_files/expanded_docx/_rels/.rels`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/expanded_docx/docProps/app.xml` & `python_docx-1.1.2/tests/test_files/expanded_docx/docProps/app.xml`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/expanded_docx/docProps/core.xml` & `python_docx-1.1.2/tests/test_files/expanded_docx/docProps/core.xml`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/expanded_docx/docProps/thumbnail.jpeg` & `python_docx-1.1.2/tests/test_files/expanded_docx/docProps/thumbnail.jpeg`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/expanded_docx/word/_rels/document.xml.rels` & `python_docx-1.1.2/tests/test_files/expanded_docx/word/_rels/document.xml.rels`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/expanded_docx/word/document.xml` & `python_docx-1.1.2/tests/test_files/expanded_docx/word/document.xml`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/expanded_docx/word/fontTable.xml` & `python_docx-1.1.2/tests/test_files/expanded_docx/word/fontTable.xml`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/expanded_docx/word/numbering.xml` & `python_docx-1.1.2/tests/test_files/expanded_docx/word/numbering.xml`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/expanded_docx/word/settings.xml` & `python_docx-1.1.2/tests/test_files/expanded_docx/word/settings.xml`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/expanded_docx/word/styles.xml` & `python_docx-1.1.2/tests/test_files/expanded_docx/word/styles.xml`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/expanded_docx/word/stylesWithEffects.xml` & `python_docx-1.1.2/tests/test_files/expanded_docx/word/stylesWithEffects.xml`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/expanded_docx/word/theme/theme1.xml` & `python_docx-1.1.2/tests/test_files/expanded_docx/word/theme/theme1.xml`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/having-images.docx` & `python_docx-1.1.2/tests/test_files/having-images.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/jfif-iguana.jpg` & `python_docx-1.1.2/tests/test_files/jfif-iguana.jpg`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/little-endian.tif` & `python_docx-1.1.2/tests/test_files/little-endian.tif`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/monty-truth.png` & `python_docx-1.1.2/tests/test_files/monty-truth.png`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/python-icon.jpeg` & `python_docx-1.1.2/tests/test_files/python-icon.jpeg`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/python-icon.png` & `python_docx-1.1.2/tests/test_files/python-icon.png`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/python-powered.png` & `python_docx-1.1.2/tests/test_files/python-powered.png`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/python.bmp` & `python_docx-1.1.2/tests/test_files/python.bmp`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/sct-inner-content.docx` & `python_docx-1.1.2/tests/test_files/sct-inner-content.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/snippets/add-row-col.txt` & `python_docx-1.1.2/tests/test_files/snippets/add-row-col.txt`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/snippets/inline.txt` & `python_docx-1.1.2/tests/test_files/snippets/inline.txt`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/snippets/new-tbl.txt` & `python_docx-1.1.2/tests/test_files/snippets/new-tbl.txt`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/snippets/tbl-cells.txt` & `python_docx-1.1.2/tests/test_files/snippets/tbl-cells.txt`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/sonic.gif` & `python_docx-1.1.2/tests/test_files/sonic.gif`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_files/test.docx` & `python_docx-1.1.2/tests/test_files/test.docx`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_package.py` & `python_docx-1.1.2/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_section.py` & `python_docx-1.1.2/tests/test_section.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_settings.py` & `python_docx-1.1.2/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_shape.py` & `python_docx-1.1.2/tests/test_shape.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_shared.py` & `python_docx-1.1.2/tests/test_shared.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/test_table.py` & `python_docx-1.1.2/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/text/test_font.py` & `python_docx-1.1.2/tests/text/test_font.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/text/test_hyperlink.py` & `python_docx-1.1.2/tests/text/test_hyperlink.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/text/test_pagebreak.py` & `python_docx-1.1.2/tests/text/test_pagebreak.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/text/test_paragraph.py` & `python_docx-1.1.2/tests/text/test_paragraph.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/text/test_parfmt.py` & `python_docx-1.1.2/tests/text/test_parfmt.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/text/test_run.py` & `python_docx-1.1.2/tests/text/test_run.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/text/test_tabstops.py` & `python_docx-1.1.2/tests/text/test_tabstops.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/unitdata.py` & `python_docx-1.1.2/tests/unitdata.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/unitutil/cxml.py` & `python_docx-1.1.2/tests/unitutil/cxml.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/unitutil/file.py` & `python_docx-1.1.2/tests/unitutil/file.py`

 * *Files identical despite different names*

### Comparing `python_docx-1.1.1/tests/unitutil/mock.py` & `python_docx-1.1.2/tests/unitutil/mock.py`

 * *Files identical despite different names*

