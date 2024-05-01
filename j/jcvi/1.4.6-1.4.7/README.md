# Comparing `tmp/jcvi-1.4.6.tar.gz` & `tmp/jcvi-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcvi-1.4.6.tar", last modified: Tue Apr 30 16:08:55 2024, max compression
+gzip compressed data, was "jcvi-1.4.7.tar", last modified: Wed May  1 04:08:29 2024, max compression
```

## Comparing `jcvi-1.4.6.tar` & `jcvi-1.4.7.tar`

### file list

```diff
@@ -1,207 +1,207 @@
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-30 16:08:55.239858 jcvi-1.4.6/
--rw-r--r--   0 bao        (501) staff       (20)     1292 2020-03-03 07:11:04.000000 jcvi-1.4.6/LICENSE
--rw-r--r--   0 bao        (501) staff       (20)       91 2022-11-27 15:24:30.000000 jcvi-1.4.6/MANIFEST.in
--rw-r--r--   0 bao        (501) staff       (20)     8915 2024-04-30 16:08:55.239964 jcvi-1.4.6/PKG-INFO
--rw-r--r--   0 bao        (501) staff       (20)     8250 2024-04-30 16:06:02.000000 jcvi-1.4.6/README.md
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-30 16:08:55.205858 jcvi-1.4.6/jcvi/
--rw-r--r--   0 bao        (501) staff       (20)      816 2024-04-30 16:06:02.000000 jcvi-1.4.6/jcvi/__init__.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-30 16:08:55.208632 jcvi-1.4.6/jcvi/algorithms/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/algorithms/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      263 2021-06-19 08:23:09.000000 jcvi-1.4.6/jcvi/algorithms/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)     6422 2021-06-19 08:23:09.000000 jcvi-1.4.6/jcvi/algorithms/ec.py
--rw-r--r--   0 bao        (501) staff       (20)     6412 2024-04-28 07:29:54.000000 jcvi-1.4.6/jcvi/algorithms/formula.py
--rw-r--r--   0 bao        (501) staff       (20)    14132 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/algorithms/graph.py
--rwxr-xr-x   0 bao        (501) staff       (20)     6275 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/algorithms/lis.py
--rwxr-xr-x   0 bao        (501) staff       (20)    24228 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/algorithms/lpsolve.py
--rw-r--r--   0 bao        (501) staff       (20)     6104 2021-06-19 08:23:09.000000 jcvi-1.4.6/jcvi/algorithms/matrix.py
--rw-r--r--   0 bao        (501) staff       (20)     1296 2021-06-19 19:45:56.000000 jcvi-1.4.6/jcvi/algorithms/maxsum.py
--rwxr-xr-x   0 bao        (501) staff       (20)     4999 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/algorithms/supermap.py
--rw-r--r--   0 bao        (501) staff       (20)    12559 2022-11-26 15:55:17.000000 jcvi-1.4.6/jcvi/algorithms/tsp.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-30 16:08:55.211048 jcvi-1.4.6/jcvi/annotation/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/annotation/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      261 2021-06-19 08:23:09.000000 jcvi-1.4.6/jcvi/annotation/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    21414 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/annotation/ahrd.py
--rw-r--r--   0 bao        (501) staff       (20)     7899 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/annotation/automaton.py
--rwxr-xr-x   0 bao        (501) staff       (20)     6417 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/annotation/depth.py
--rw-r--r--   0 bao        (501) staff       (20)     7042 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/annotation/evm.py
--rw-r--r--   0 bao        (501) staff       (20)    14687 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/annotation/maker.py
--rw-r--r--   0 bao        (501) staff       (20)    19485 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/annotation/pasa.py
--rw-r--r--   0 bao        (501) staff       (20)    12822 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/annotation/qc.py
--rw-r--r--   0 bao        (501) staff       (20)    42839 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/annotation/reformat.py
--rw-r--r--   0 bao        (501) staff       (20)    12645 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/annotation/stats.py
--rw-r--r--   0 bao        (501) staff       (20)     6793 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/annotation/train.py
--rw-r--r--   0 bao        (501) staff       (20)     5042 2024-04-30 16:06:02.000000 jcvi-1.4.6/jcvi/annotation/trinity.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-30 16:08:55.214876 jcvi-1.4.6/jcvi/apps/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/apps/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      258 2021-06-19 08:23:09.000000 jcvi-1.4.6/jcvi/apps/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    20591 2024-04-29 06:36:47.000000 jcvi-1.4.6/jcvi/apps/align.py
--rw-r--r--   0 bao        (501) staff       (20)    66789 2024-04-30 16:06:02.000000 jcvi-1.4.6/jcvi/apps/base.py
--rw-r--r--   0 bao        (501) staff       (20)    12271 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/apps/biomart.py
--rwxr-xr-x   0 bao        (501) staff       (20)     3554 2021-06-19 19:45:56.000000 jcvi-1.4.6/jcvi/apps/blastplus.py
--rw-r--r--   0 bao        (501) staff       (20)     5219 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/apps/bowtie.py
--rw-r--r--   0 bao        (501) staff       (20)     7695 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/apps/bwa.py
--rw-r--r--   0 bao        (501) staff       (20)     7279 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/apps/cdhit.py
--rw-r--r--   0 bao        (501) staff       (20)     2623 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/apps/emboss.py
--rw-r--r--   0 bao        (501) staff       (20)    21333 2024-04-29 06:36:47.000000 jcvi-1.4.6/jcvi/apps/fetch.py
--rw-r--r--   0 bao        (501) staff       (20)    19459 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/apps/gbsubmit.py
--rw-r--r--   0 bao        (501) staff       (20)     6892 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/apps/gmap.py
--rw-r--r--   0 bao        (501) staff       (20)    18477 2024-04-29 06:36:47.000000 jcvi-1.4.6/jcvi/apps/grid.py
--rwxr-xr-x   0 bao        (501) staff       (20)     7238 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/apps/lastz.py
--rwxr-xr-x   0 bao        (501) staff       (20)     3004 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/apps/mask.py
--rw-r--r--   0 bao        (501) staff       (20)    35471 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/apps/phylo.py
--rw-r--r--   0 bao        (501) staff       (20)     1896 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/apps/r.py
--rw-r--r--   0 bao        (501) staff       (20)     4901 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/apps/restriction.py
--rw-r--r--   0 bao        (501) staff       (20)     3784 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/apps/softlink.py
--rw-r--r--   0 bao        (501) staff       (20)    33065 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/apps/uclust.py
--rw-r--r--   0 bao        (501) staff       (20)     5208 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/apps/uniprot.py
--rw-r--r--   0 bao        (501) staff       (20)     3661 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/apps/vecscreen.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-30 16:08:55.220021 jcvi-1.4.6/jcvi/assembly/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/assembly/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      257 2021-06-19 08:23:09.000000 jcvi-1.4.6/jcvi/assembly/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    65602 2024-04-30 16:06:02.000000 jcvi-1.4.6/jcvi/assembly/allmaps.py
--rw-r--r--   0 bao        (501) staff       (20)    15451 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/assembly/allpaths.py
--rw-r--r--   0 bao        (501) staff       (20)    13265 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/assembly/automaton.py
--rw-r--r--   0 bao        (501) staff       (20)     5544 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/assembly/base.py
--rw-r--r--   0 bao        (501) staff       (20)     3457 2022-09-27 05:18:33.000000 jcvi-1.4.6/jcvi/assembly/chic.pyx
--rw-r--r--   0 bao        (501) staff       (20)     4581 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/assembly/coverage.py
--rw-r--r--   0 bao        (501) staff       (20)     8676 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/assembly/gaps.py
--rw-r--r--   0 bao        (501) staff       (20)    20002 2024-04-29 06:10:52.000000 jcvi-1.4.6/jcvi/assembly/geneticmap.py
--rw-r--r--   0 bao        (501) staff       (20)    34692 2024-04-29 06:36:47.000000 jcvi-1.4.6/jcvi/assembly/goldenpath.py
--rw-r--r--   0 bao        (501) staff       (20)    56167 2024-04-29 06:10:52.000000 jcvi-1.4.6/jcvi/assembly/hic.py
--rw-r--r--   0 bao        (501) staff       (20)    43034 2024-04-29 06:10:52.000000 jcvi-1.4.6/jcvi/assembly/kmer.py
--rw-r--r--   0 bao        (501) staff       (20)    12519 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/assembly/opticalmap.py
--rw-r--r--   0 bao        (501) staff       (20)    27279 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/assembly/patch.py
--rw-r--r--   0 bao        (501) staff       (20)    15741 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/assembly/postprocess.py
--rw-r--r--   0 bao        (501) staff       (20)    21473 2024-04-30 06:05:19.000000 jcvi-1.4.6/jcvi/assembly/preprocess.py
--rw-r--r--   0 bao        (501) staff       (20)     6287 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/assembly/sim.py
--rw-r--r--   0 bao        (501) staff       (20)     8830 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/assembly/soap.py
--rw-r--r--   0 bao        (501) staff       (20)    16183 2023-04-26 05:51:28.000000 jcvi-1.4.6/jcvi/assembly/syntenypath.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-30 16:08:55.222250 jcvi-1.4.6/jcvi/compara/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/compara/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      251 2021-06-19 08:23:09.000000 jcvi-1.4.6/jcvi/compara/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)     4218 2023-09-28 09:59:53.000000 jcvi-1.4.6/jcvi/compara/base.py
--rwxr-xr-x   0 bao        (501) staff       (20)     9796 2023-04-26 05:51:28.000000 jcvi-1.4.6/jcvi/compara/blastfilter.py
--rw-r--r--   0 bao        (501) staff       (20)    28506 2024-04-30 16:06:02.000000 jcvi-1.4.6/jcvi/compara/catalog.py
--rw-r--r--   0 bao        (501) staff       (20)    26355 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/compara/fractionation.py
--rw-r--r--   0 bao        (501) staff       (20)    33945 2024-04-29 06:10:52.000000 jcvi-1.4.6/jcvi/compara/ks.py
--rw-r--r--   0 bao        (501) staff       (20)     9216 2023-04-26 05:51:28.000000 jcvi-1.4.6/jcvi/compara/pad.py
--rw-r--r--   0 bao        (501) staff       (20)     8322 2024-04-29 06:10:52.000000 jcvi-1.4.6/jcvi/compara/pedigree.py
--rw-r--r--   0 bao        (501) staff       (20)     3051 2021-06-19 08:23:09.000000 jcvi-1.4.6/jcvi/compara/phylogeny.py
--rwxr-xr-x   0 bao        (501) staff       (20)     7948 2023-04-26 05:51:28.000000 jcvi-1.4.6/jcvi/compara/quota.py
--rw-r--r--   0 bao        (501) staff       (20)    10341 2023-04-26 05:51:28.000000 jcvi-1.4.6/jcvi/compara/reconstruct.py
--rwxr-xr-x   0 bao        (501) staff       (20)     9233 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/compara/synfind.py
--rwxr-xr-x   0 bao        (501) staff       (20)    57574 2023-04-26 05:51:28.000000 jcvi-1.4.6/jcvi/compara/synteny.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-30 16:08:55.227614 jcvi-1.4.6/jcvi/formats/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/formats/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      262 2021-06-19 08:23:09.000000 jcvi-1.4.6/jcvi/formats/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    63559 2024-04-29 06:36:47.000000 jcvi-1.4.6/jcvi/formats/agp.py
--rw-r--r--   0 bao        (501) staff       (20)    33880 2024-04-30 06:05:19.000000 jcvi-1.4.6/jcvi/formats/base.py
--rwxr-xr-x   0 bao        (501) staff       (20)    71545 2024-04-30 06:05:19.000000 jcvi-1.4.6/jcvi/formats/bed.py
--rw-r--r--   0 bao        (501) staff       (20)    43184 2023-06-19 14:46:14.000000 jcvi-1.4.6/jcvi/formats/blast.py
--rw-r--r--   0 bao        (501) staff       (20)     7010 2022-09-27 05:18:33.000000 jcvi-1.4.6/jcvi/formats/cblast.pyx
--rw-r--r--   0 bao        (501) staff       (20)     3193 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/formats/cdt.py
--rw-r--r--   0 bao        (501) staff       (20)     8612 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/formats/chain.py
--rw-r--r--   0 bao        (501) staff       (20)     4644 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/formats/contig.py
--rw-r--r--   0 bao        (501) staff       (20)    15169 2024-04-29 06:36:47.000000 jcvi-1.4.6/jcvi/formats/coords.py
--rw-r--r--   0 bao        (501) staff       (20)     6529 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/formats/excel.py
--rw-r--r--   0 bao        (501) staff       (20)    75502 2024-04-30 06:05:19.000000 jcvi-1.4.6/jcvi/formats/fasta.py
--rw-r--r--   0 bao        (501) staff       (20)    29575 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/formats/fastq.py
--rw-r--r--   0 bao        (501) staff       (20)    15545 2024-04-29 06:36:47.000000 jcvi-1.4.6/jcvi/formats/genbank.py
--rw-r--r--   0 bao        (501) staff       (20)   119858 2024-04-30 06:05:19.000000 jcvi-1.4.6/jcvi/formats/gff.py
--rw-r--r--   0 bao        (501) staff       (20)     3979 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/formats/html.py
--rw-r--r--   0 bao        (501) staff       (20)     4612 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/formats/maf.py
--rwxr-xr-x   0 bao        (501) staff       (20)     2842 2021-07-05 22:45:00.000000 jcvi-1.4.6/jcvi/formats/obo.py
--rw-r--r--   0 bao        (501) staff       (20)     2900 2021-01-11 06:59:36.000000 jcvi-1.4.6/jcvi/formats/paf.py
--rw-r--r--   0 bao        (501) staff       (20)     2783 2024-04-29 06:36:47.000000 jcvi-1.4.6/jcvi/formats/pdf.py
--rwxr-xr-x   0 bao        (501) staff       (20)    10355 2023-11-24 05:16:26.000000 jcvi-1.4.6/jcvi/formats/psl.py
--rw-r--r--   0 bao        (501) staff       (20)     2746 2021-06-19 08:23:09.000000 jcvi-1.4.6/jcvi/formats/pyblast.py
--rw-r--r--   0 bao        (501) staff       (20)    28231 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/formats/sam.py
--rw-r--r--   0 bao        (501) staff       (20)     8041 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/formats/sizes.py
--rw-r--r--   0 bao        (501) staff       (20)    25480 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/formats/vcf.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-30 16:08:55.230852 jcvi-1.4.6/jcvi/graphics/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/graphics/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      271 2021-06-19 08:23:09.000000 jcvi-1.4.6/jcvi/graphics/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    16271 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/graphics/align.py
--rw-r--r--   0 bao        (501) staff       (20)    15265 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/graphics/assembly.py
--rw-r--r--   0 bao        (501) staff       (20)    24983 2024-04-30 16:06:02.000000 jcvi-1.4.6/jcvi/graphics/base.py
--rwxr-xr-x   0 bao        (501) staff       (20)    10002 2024-04-29 06:36:47.000000 jcvi-1.4.6/jcvi/graphics/blastplot.py
--rw-r--r--   0 bao        (501) staff       (20)    22322 2024-04-30 06:05:19.000000 jcvi-1.4.6/jcvi/graphics/chromosome.py
--rw-r--r--   0 bao        (501) staff       (20)     7145 2021-06-19 08:23:09.000000 jcvi-1.4.6/jcvi/graphics/coverage.py
--rwxr-xr-x   0 bao        (501) staff       (20)    14873 2023-04-26 05:51:28.000000 jcvi-1.4.6/jcvi/graphics/dotplot.py
--rw-r--r--   0 bao        (501) staff       (20)    21810 2023-02-06 05:16:46.000000 jcvi-1.4.6/jcvi/graphics/glyph.py
--rw-r--r--   0 bao        (501) staff       (20)    24862 2024-04-24 05:29:17.000000 jcvi-1.4.6/jcvi/graphics/grabseeds.py
--rw-r--r--   0 bao        (501) staff       (20)     5025 2021-03-26 15:38:36.000000 jcvi-1.4.6/jcvi/graphics/heatmap.py
--rw-r--r--   0 bao        (501) staff       (20)     9610 2024-04-29 06:36:47.000000 jcvi-1.4.6/jcvi/graphics/histogram.py
--rw-r--r--   0 bao        (501) staff       (20)    13307 2024-04-30 16:06:02.000000 jcvi-1.4.6/jcvi/graphics/karyotype.py
--rw-r--r--   0 bao        (501) staff       (20)    34080 2024-04-30 16:06:02.000000 jcvi-1.4.6/jcvi/graphics/landscape.py
--rw-r--r--   0 bao        (501) staff       (20)     3893 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/graphics/mummerplot.py
--rw-r--r--   0 bao        (501) staff       (20)    22468 2024-04-30 16:06:02.000000 jcvi-1.4.6/jcvi/graphics/synteny.py
--rw-r--r--   0 bao        (501) staff       (20)     5488 2021-06-19 19:45:56.000000 jcvi-1.4.6/jcvi/graphics/table.py
--rw-r--r--   0 bao        (501) staff       (20)    20377 2022-11-26 16:06:34.000000 jcvi-1.4.6/jcvi/graphics/tree.py
--rw-r--r--   0 bao        (501) staff       (20)     6194 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/graphics/wheel.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-30 16:08:55.233241 jcvi-1.4.6/jcvi/projects/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/projects/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      260 2021-06-19 08:23:09.000000 jcvi-1.4.6/jcvi/projects/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    22445 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/projects/age.py
--rw-r--r--   0 bao        (501) staff       (20)    15907 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/projects/allmaps.py
--rw-r--r--   0 bao        (501) staff       (20)     6750 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/projects/bites.py
--rw-r--r--   0 bao        (501) staff       (20)    14136 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/projects/ies.py
--rw-r--r--   0 bao        (501) staff       (20)     7085 2024-04-30 16:06:02.000000 jcvi-1.4.6/jcvi/projects/jcvi.py
--rw-r--r--   0 bao        (501) staff       (20)    22179 2024-04-29 06:10:52.000000 jcvi-1.4.6/jcvi/projects/misc.py
--rw-r--r--   0 bao        (501) staff       (20)    25024 2023-02-06 05:16:46.000000 jcvi-1.4.6/jcvi/projects/napus.py
--rw-r--r--   0 bao        (501) staff       (20)    12754 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/projects/pineapple.py
--rw-r--r--   0 bao        (501) staff       (20)    67853 2024-04-29 06:36:47.000000 jcvi-1.4.6/jcvi/projects/str.py
--rw-r--r--   0 bao        (501) staff       (20)    25766 2024-04-29 06:36:47.000000 jcvi-1.4.6/jcvi/projects/sugarcane.py
--rw-r--r--   0 bao        (501) staff       (20)    23950 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/projects/synfind.py
--rw-r--r--   0 bao        (501) staff       (20)    21554 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/projects/tgbs.py
--rw-r--r--   0 bao        (501) staff       (20)    11690 2024-04-30 16:06:02.000000 jcvi-1.4.6/jcvi/projects/vanilla.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-30 16:08:55.235000 jcvi-1.4.6/jcvi/utils/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/utils/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      260 2021-06-19 08:23:09.000000 jcvi-1.4.6/jcvi/utils/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    24200 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/utils/aws.py
--rw-r--r--   0 bao        (501) staff       (20)    12647 2024-04-30 16:06:02.000000 jcvi-1.4.6/jcvi/utils/cbook.py
--rw-r--r--   0 bao        (501) staff       (20)      355 2021-01-11 02:34:49.000000 jcvi-1.4.6/jcvi/utils/console.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-30 16:08:55.238003 jcvi-1.4.6/jcvi/utils/data/
--rwxr-xr-x   0 bao        (501) staff       (20)    16912 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/utils/data/Airswing.ttf
--rwxr-xr-x   0 bao        (501) staff       (20)   103940 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/utils/data/Collegia.ttf
--rwxr-xr-x   0 bao        (501) staff       (20)    20468 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/utils/data/HookedUp.ttf
--rw-r--r--   0 bao        (501) staff       (20)    25832 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/utils/data/Humor-Sans.ttf
--rw-r--r--   0 bao        (501) staff       (20)    28065 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/utils/data/TREDs.meta.csv
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/utils/data/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      911 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/utils/data/adapters.fasta
--rw-r--r--   0 bao        (501) staff       (20)     3321 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/utils/data/blosum80.mat
--rw-r--r--   0 bao        (501) staff       (20)     7686 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/utils/data/chrY.hg38.unique_ccn.gc
--rw-r--r--   0 bao        (501) staff       (20)      282 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/utils/data/colorchecker.txt
--rw-r--r--   0 bao        (501) staff       (20)    45544 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/utils/data/hg38.band.txt
--rw-r--r--   0 bao        (501) staff       (20)    11672 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/utils/data/hg38.chrom.sizes
--rw-r--r--   0 bao        (501) staff       (20)     1000 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/utils/data/instance.json
--rw-r--r--   0 bao        (501) staff       (20)     9793 2024-04-29 06:36:47.000000 jcvi-1.4.6/jcvi/utils/db.py
--rw-r--r--   0 bao        (501) staff       (20)     4145 2021-01-09 20:22:53.000000 jcvi-1.4.6/jcvi/utils/ez_setup.py
--rwxr-xr-x   0 bao        (501) staff       (20)     2884 2021-06-19 08:23:09.000000 jcvi-1.4.6/jcvi/utils/grouper.py
--rw-r--r--   0 bao        (501) staff       (20)    10437 2021-06-19 08:23:09.000000 jcvi-1.4.6/jcvi/utils/orderedcollections.py
--rw-r--r--   0 bao        (501) staff       (20)    14595 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/utils/range.py
--rw-r--r--   0 bao        (501) staff       (20)     3946 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/utils/table.py
--rw-r--r--   0 bao        (501) staff       (20)     4687 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/utils/taxonomy.py
--rw-r--r--   0 bao        (501) staff       (20)     1522 2021-07-13 05:06:52.000000 jcvi-1.4.6/jcvi/utils/validator.py
--rwxr-xr-x   0 bao        (501) staff       (20)     1377 2021-01-15 14:44:37.000000 jcvi-1.4.6/jcvi/utils/webcolors.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-30 16:08:55.239393 jcvi-1.4.6/jcvi/variation/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.4.6/jcvi/variation/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      259 2021-06-19 08:23:09.000000 jcvi-1.4.6/jcvi/variation/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    45321 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/variation/cnv.py
--rw-r--r--   0 bao        (501) staff       (20)     7036 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/variation/deconvolute.py
--rw-r--r--   0 bao        (501) staff       (20)     9385 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/variation/delly.py
--rw-r--r--   0 bao        (501) staff       (20)    11777 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/variation/impute.py
--rw-r--r--   0 bao        (501) staff       (20)     3478 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/variation/phase.py
--rw-r--r--   0 bao        (501) staff       (20)    10831 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/variation/snp.py
--rw-r--r--   0 bao        (501) staff       (20)    48818 2023-02-06 03:44:04.000000 jcvi-1.4.6/jcvi/variation/str.py
--rw-r--r--   0 bao        (501) staff       (20)      176 2024-04-30 16:08:55.000000 jcvi-1.4.6/jcvi/version.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-04-30 16:08:55.206721 jcvi-1.4.6/jcvi.egg-info/
--rw-r--r--   0 bao        (501) staff       (20)     8915 2024-04-30 16:08:55.000000 jcvi-1.4.6/jcvi.egg-info/PKG-INFO
--rw-r--r--   0 bao        (501) staff       (20)     4543 2024-04-30 16:08:55.000000 jcvi-1.4.6/jcvi.egg-info/SOURCES.txt
--rw-r--r--   0 bao        (501) staff       (20)        1 2024-04-30 16:08:55.000000 jcvi-1.4.6/jcvi.egg-info/dependency_links.txt
--rw-r--r--   0 bao        (501) staff       (20)        1 2022-11-26 21:54:22.000000 jcvi-1.4.6/jcvi.egg-info/not-zip-safe
--rw-r--r--   0 bao        (501) staff       (20)      221 2024-04-30 16:08:55.000000 jcvi-1.4.6/jcvi.egg-info/requires.txt
--rw-r--r--   0 bao        (501) staff       (20)        5 2024-04-30 16:08:55.000000 jcvi-1.4.6/jcvi.egg-info/top_level.txt
--rw-r--r--   0 bao        (501) staff       (20)      359 2022-11-26 21:23:29.000000 jcvi-1.4.6/pyproject.toml
--rw-r--r--   0 bao        (501) staff       (20)     1242 2024-04-30 16:08:55.240326 jcvi-1.4.6/setup.cfg
--rw-r--r--   0 bao        (501) staff       (20)      553 2022-11-26 21:23:29.000000 jcvi-1.4.6/setup.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-01 04:08:29.472594 jcvi-1.4.7/
+-rw-r--r--   0 bao        (501) staff       (20)     1292 2020-03-03 07:11:04.000000 jcvi-1.4.7/LICENSE
+-rw-r--r--   0 bao        (501) staff       (20)       91 2022-11-27 15:24:30.000000 jcvi-1.4.7/MANIFEST.in
+-rw-r--r--   0 bao        (501) staff       (20)     8915 2024-05-01 04:08:29.472710 jcvi-1.4.7/PKG-INFO
+-rw-r--r--   0 bao        (501) staff       (20)     8250 2024-04-30 16:06:02.000000 jcvi-1.4.7/README.md
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-01 04:08:29.445122 jcvi-1.4.7/jcvi/
+-rw-r--r--   0 bao        (501) staff       (20)      816 2024-05-01 01:14:54.000000 jcvi-1.4.7/jcvi/__init__.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-01 04:08:29.447513 jcvi-1.4.7/jcvi/algorithms/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2024-05-01 01:14:54.000000 jcvi-1.4.7/jcvi/algorithms/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      263 2024-05-01 01:14:54.000000 jcvi-1.4.7/jcvi/algorithms/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)     6421 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/algorithms/ec.py
+-rw-r--r--   0 bao        (501) staff       (20)     6412 2024-05-01 01:14:54.000000 jcvi-1.4.7/jcvi/algorithms/formula.py
+-rw-r--r--   0 bao        (501) staff       (20)    14137 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/algorithms/graph.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     6275 2024-05-01 01:14:54.000000 jcvi-1.4.7/jcvi/algorithms/lis.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    24107 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/algorithms/lpsolve.py
+-rw-r--r--   0 bao        (501) staff       (20)     6102 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/algorithms/matrix.py
+-rw-r--r--   0 bao        (501) staff       (20)     1296 2024-05-01 01:14:54.000000 jcvi-1.4.7/jcvi/algorithms/maxsum.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     4978 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/algorithms/supermap.py
+-rw-r--r--   0 bao        (501) staff       (20)    12550 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/algorithms/tsp.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-01 04:08:29.449222 jcvi-1.4.7/jcvi/annotation/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2024-05-01 01:14:54.000000 jcvi-1.4.7/jcvi/annotation/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      258 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/annotation/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    21401 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/annotation/ahrd.py
+-rw-r--r--   0 bao        (501) staff       (20)     7917 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/annotation/automaton.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     6395 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/annotation/depth.py
+-rw-r--r--   0 bao        (501) staff       (20)     7033 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/annotation/evm.py
+-rw-r--r--   0 bao        (501) staff       (20)    14679 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/annotation/maker.py
+-rw-r--r--   0 bao        (501) staff       (20)    19482 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/annotation/pasa.py
+-rw-r--r--   0 bao        (501) staff       (20)    12807 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/annotation/qc.py
+-rw-r--r--   0 bao        (501) staff       (20)    42756 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/annotation/reformat.py
+-rw-r--r--   0 bao        (501) staff       (20)    12632 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/annotation/stats.py
+-rw-r--r--   0 bao        (501) staff       (20)     6781 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/annotation/train.py
+-rw-r--r--   0 bao        (501) staff       (20)     5040 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/annotation/trinity.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-01 04:08:29.452348 jcvi-1.4.7/jcvi/apps/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2024-05-01 01:14:54.000000 jcvi-1.4.7/jcvi/apps/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      249 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/apps/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    20581 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/apps/align.py
+-rw-r--r--   0 bao        (501) staff       (20)    66874 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/apps/base.py
+-rw-r--r--   0 bao        (501) staff       (20)    12248 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/apps/biomart.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     3516 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/apps/blastplus.py
+-rw-r--r--   0 bao        (501) staff       (20)     5228 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/apps/bowtie.py
+-rw-r--r--   0 bao        (501) staff       (20)     7676 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/apps/bwa.py
+-rw-r--r--   0 bao        (501) staff       (20)     7237 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/apps/cdhit.py
+-rw-r--r--   0 bao        (501) staff       (20)     2611 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/apps/emboss.py
+-rw-r--r--   0 bao        (501) staff       (20)    21311 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/apps/fetch.py
+-rw-r--r--   0 bao        (501) staff       (20)    19442 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/apps/gbsubmit.py
+-rw-r--r--   0 bao        (501) staff       (20)     6881 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/apps/gmap.py
+-rw-r--r--   0 bao        (501) staff       (20)    18461 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/apps/grid.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     7214 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/apps/lastz.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     2992 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/apps/mask.py
+-rw-r--r--   0 bao        (501) staff       (20)    35460 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/apps/phylo.py
+-rw-r--r--   0 bao        (501) staff       (20)     1854 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/apps/r.py
+-rw-r--r--   0 bao        (501) staff       (20)     4873 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/apps/restriction.py
+-rw-r--r--   0 bao        (501) staff       (20)     3767 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/apps/softlink.py
+-rw-r--r--   0 bao        (501) staff       (20)    33029 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/apps/uclust.py
+-rw-r--r--   0 bao        (501) staff       (20)     5194 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/apps/uniprot.py
+-rw-r--r--   0 bao        (501) staff       (20)     3636 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/apps/vecscreen.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-01 04:08:29.455599 jcvi-1.4.7/jcvi/assembly/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2024-05-01 01:14:54.000000 jcvi-1.4.7/jcvi/assembly/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      253 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/assembly/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    65586 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/assembly/allmaps.py
+-rw-r--r--   0 bao        (501) staff       (20)    15425 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/assembly/allpaths.py
+-rw-r--r--   0 bao        (501) staff       (20)    13251 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/assembly/automaton.py
+-rw-r--r--   0 bao        (501) staff       (20)     5535 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/assembly/base.py
+-rw-r--r--   0 bao        (501) staff       (20)     3457 2022-09-27 05:18:33.000000 jcvi-1.4.7/jcvi/assembly/chic.pyx
+-rw-r--r--   0 bao        (501) staff       (20)     4558 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/assembly/coverage.py
+-rw-r--r--   0 bao        (501) staff       (20)     8650 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/assembly/gaps.py
+-rw-r--r--   0 bao        (501) staff       (20)    20008 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/assembly/geneticmap.py
+-rw-r--r--   0 bao        (501) staff       (20)    34665 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/assembly/goldenpath.py
+-rw-r--r--   0 bao        (501) staff       (20)    56179 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/assembly/hic.py
+-rw-r--r--   0 bao        (501) staff       (20)    43053 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/assembly/kmer.py
+-rw-r--r--   0 bao        (501) staff       (20)    12475 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/assembly/opticalmap.py
+-rw-r--r--   0 bao        (501) staff       (20)    27263 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/assembly/patch.py
+-rw-r--r--   0 bao        (501) staff       (20)    15706 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/assembly/postprocess.py
+-rw-r--r--   0 bao        (501) staff       (20)    21503 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/assembly/preprocess.py
+-rw-r--r--   0 bao        (501) staff       (20)     6275 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/assembly/sim.py
+-rw-r--r--   0 bao        (501) staff       (20)     8836 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/assembly/soap.py
+-rw-r--r--   0 bao        (501) staff       (20)    16163 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/assembly/syntenypath.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-01 04:08:29.457604 jcvi-1.4.7/jcvi/compara/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2024-05-01 01:14:54.000000 jcvi-1.4.7/jcvi/compara/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      247 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/compara/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)     4218 2024-05-01 01:14:54.000000 jcvi-1.4.7/jcvi/compara/base.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     9765 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/compara/blastfilter.py
+-rw-r--r--   0 bao        (501) staff       (20)    28531 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/compara/catalog.py
+-rw-r--r--   0 bao        (501) staff       (20)    26317 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/compara/fractionation.py
+-rw-r--r--   0 bao        (501) staff       (20)    33973 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/compara/ks.py
+-rw-r--r--   0 bao        (501) staff       (20)     9189 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/compara/pad.py
+-rw-r--r--   0 bao        (501) staff       (20)     8324 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/compara/pedigree.py
+-rw-r--r--   0 bao        (501) staff       (20)     3048 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/compara/phylogeny.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     7933 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/compara/quota.py
+-rw-r--r--   0 bao        (501) staff       (20)    10310 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/compara/reconstruct.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     9136 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/compara/synfind.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    57581 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/compara/synteny.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-01 04:08:29.461574 jcvi-1.4.7/jcvi/formats/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2024-05-01 01:14:54.000000 jcvi-1.4.7/jcvi/formats/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      258 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/formats/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    63425 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/formats/agp.py
+-rw-r--r--   0 bao        (501) staff       (20)    33922 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/formats/base.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    71610 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/formats/bed.py
+-rw-r--r--   0 bao        (501) staff       (20)    43167 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/formats/blast.py
+-rw-r--r--   0 bao        (501) staff       (20)     7010 2022-09-27 05:18:33.000000 jcvi-1.4.7/jcvi/formats/cblast.pyx
+-rw-r--r--   0 bao        (501) staff       (20)     3163 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/formats/cdt.py
+-rw-r--r--   0 bao        (501) staff       (20)     8592 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/formats/chain.py
+-rw-r--r--   0 bao        (501) staff       (20)     4620 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/formats/contig.py
+-rw-r--r--   0 bao        (501) staff       (20)    15170 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/formats/coords.py
+-rw-r--r--   0 bao        (501) staff       (20)     6516 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/formats/excel.py
+-rw-r--r--   0 bao        (501) staff       (20)    75587 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/formats/fasta.py
+-rw-r--r--   0 bao        (501) staff       (20)    29570 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/formats/fastq.py
+-rw-r--r--   0 bao        (501) staff       (20)    15510 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/formats/genbank.py
+-rw-r--r--   0 bao        (501) staff       (20)   119884 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/formats/gff.py
+-rw-r--r--   0 bao        (501) staff       (20)     3962 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/formats/html.py
+-rw-r--r--   0 bao        (501) staff       (20)     4595 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/formats/maf.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     2816 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/formats/obo.py
+-rw-r--r--   0 bao        (501) staff       (20)     2880 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/formats/paf.py
+-rw-r--r--   0 bao        (501) staff       (20)     2749 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/formats/pdf.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    10351 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/formats/psl.py
+-rw-r--r--   0 bao        (501) staff       (20)     2746 2024-05-01 01:14:54.000000 jcvi-1.4.7/jcvi/formats/pyblast.py
+-rw-r--r--   0 bao        (501) staff       (20)    28218 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/formats/sam.py
+-rw-r--r--   0 bao        (501) staff       (20)     8018 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/formats/sizes.py
+-rw-r--r--   0 bao        (501) staff       (20)    25449 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/formats/vcf.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-01 04:08:29.464182 jcvi-1.4.7/jcvi/graphics/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2024-05-01 01:14:54.000000 jcvi-1.4.7/jcvi/graphics/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      267 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/graphics/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    16228 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/graphics/align.py
+-rw-r--r--   0 bao        (501) staff       (20)    15231 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/graphics/assembly.py
+-rw-r--r--   0 bao        (501) staff       (20)    24985 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/graphics/base.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     9984 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/graphics/blastplot.py
+-rw-r--r--   0 bao        (501) staff       (20)    22264 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/graphics/chromosome.py
+-rw-r--r--   0 bao        (501) staff       (20)     7097 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/graphics/coverage.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    14852 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/graphics/dotplot.py
+-rw-r--r--   0 bao        (501) staff       (20)    21811 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/graphics/glyph.py
+-rw-r--r--   0 bao        (501) staff       (20)    24787 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/graphics/grabseeds.py
+-rw-r--r--   0 bao        (501) staff       (20)     5017 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/graphics/heatmap.py
+-rw-r--r--   0 bao        (501) staff       (20)     9589 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/graphics/histogram.py
+-rw-r--r--   0 bao        (501) staff       (20)    13317 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/graphics/karyotype.py
+-rw-r--r--   0 bao        (501) staff       (20)    34110 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/graphics/landscape.py
+-rw-r--r--   0 bao        (501) staff       (20)     3862 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/graphics/mummerplot.py
+-rw-r--r--   0 bao        (501) staff       (20)    22488 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/graphics/synteny.py
+-rw-r--r--   0 bao        (501) staff       (20)     5473 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/graphics/table.py
+-rw-r--r--   0 bao        (501) staff       (20)    20370 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/graphics/tree.py
+-rw-r--r--   0 bao        (501) staff       (20)     6182 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/graphics/wheel.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-01 04:08:29.466159 jcvi-1.4.7/jcvi/projects/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2024-05-01 01:14:54.000000 jcvi-1.4.7/jcvi/projects/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      257 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/projects/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    22430 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/projects/age.py
+-rw-r--r--   0 bao        (501) staff       (20)    15889 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/projects/allmaps.py
+-rw-r--r--   0 bao        (501) staff       (20)     6738 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/projects/bites.py
+-rw-r--r--   0 bao        (501) staff       (20)    14086 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/projects/ies.py
+-rw-r--r--   0 bao        (501) staff       (20)     7085 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/projects/jcvi.py
+-rw-r--r--   0 bao        (501) staff       (20)    22160 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/projects/misc.py
+-rw-r--r--   0 bao        (501) staff       (20)    24998 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/projects/napus.py
+-rw-r--r--   0 bao        (501) staff       (20)    12708 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/projects/pineapple.py
+-rw-r--r--   0 bao        (501) staff       (20)    67821 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/projects/str.py
+-rw-r--r--   0 bao        (501) staff       (20)    25729 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/projects/sugarcane.py
+-rw-r--r--   0 bao        (501) staff       (20)    23885 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/projects/synfind.py
+-rw-r--r--   0 bao        (501) staff       (20)    21557 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/projects/tgbs.py
+-rw-r--r--   0 bao        (501) staff       (20)    11690 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/projects/vanilla.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-01 04:08:29.468282 jcvi-1.4.7/jcvi/utils/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2024-05-01 01:14:54.000000 jcvi-1.4.7/jcvi/utils/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      256 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/utils/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    24193 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/utils/aws.py
+-rw-r--r--   0 bao        (501) staff       (20)    12647 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/utils/cbook.py
+-rw-r--r--   0 bao        (501) staff       (20)      355 2024-05-01 01:14:54.000000 jcvi-1.4.7/jcvi/utils/console.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-01 04:08:29.470921 jcvi-1.4.7/jcvi/utils/data/
+-rwxr-xr-x   0 bao        (501) staff       (20)    16912 2020-01-29 05:28:41.000000 jcvi-1.4.7/jcvi/utils/data/Airswing.ttf
+-rwxr-xr-x   0 bao        (501) staff       (20)   103940 2020-01-29 05:28:41.000000 jcvi-1.4.7/jcvi/utils/data/Collegia.ttf
+-rwxr-xr-x   0 bao        (501) staff       (20)    20468 2020-01-29 05:28:41.000000 jcvi-1.4.7/jcvi/utils/data/HookedUp.ttf
+-rw-r--r--   0 bao        (501) staff       (20)    25832 2020-01-29 05:28:41.000000 jcvi-1.4.7/jcvi/utils/data/Humor-Sans.ttf
+-rw-r--r--   0 bao        (501) staff       (20)    28065 2020-01-29 05:28:41.000000 jcvi-1.4.7/jcvi/utils/data/TREDs.meta.csv
+-rw-r--r--   0 bao        (501) staff       (20)        0 2024-05-01 01:14:54.000000 jcvi-1.4.7/jcvi/utils/data/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      911 2020-01-29 05:28:41.000000 jcvi-1.4.7/jcvi/utils/data/adapters.fasta
+-rw-r--r--   0 bao        (501) staff       (20)     3321 2020-01-29 05:28:41.000000 jcvi-1.4.7/jcvi/utils/data/blosum80.mat
+-rw-r--r--   0 bao        (501) staff       (20)     7686 2020-01-29 05:28:41.000000 jcvi-1.4.7/jcvi/utils/data/chrY.hg38.unique_ccn.gc
+-rw-r--r--   0 bao        (501) staff       (20)      282 2020-01-29 05:28:41.000000 jcvi-1.4.7/jcvi/utils/data/colorchecker.txt
+-rw-r--r--   0 bao        (501) staff       (20)    45544 2020-01-29 05:28:41.000000 jcvi-1.4.7/jcvi/utils/data/hg38.band.txt
+-rw-r--r--   0 bao        (501) staff       (20)    11672 2020-01-29 05:28:41.000000 jcvi-1.4.7/jcvi/utils/data/hg38.chrom.sizes
+-rw-r--r--   0 bao        (501) staff       (20)     1000 2020-01-29 05:28:41.000000 jcvi-1.4.7/jcvi/utils/data/instance.json
+-rw-r--r--   0 bao        (501) staff       (20)     9726 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/utils/db.py
+-rw-r--r--   0 bao        (501) staff       (20)     4145 2024-05-01 01:14:54.000000 jcvi-1.4.7/jcvi/utils/ez_setup.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     2884 2024-05-01 01:14:54.000000 jcvi-1.4.7/jcvi/utils/grouper.py
+-rw-r--r--   0 bao        (501) staff       (20)    10437 2024-05-01 01:14:54.000000 jcvi-1.4.7/jcvi/utils/orderedcollections.py
+-rw-r--r--   0 bao        (501) staff       (20)    14596 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/utils/range.py
+-rw-r--r--   0 bao        (501) staff       (20)     3946 2024-05-01 01:14:54.000000 jcvi-1.4.7/jcvi/utils/table.py
+-rw-r--r--   0 bao        (501) staff       (20)     4675 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/utils/taxonomy.py
+-rw-r--r--   0 bao        (501) staff       (20)     1522 2024-05-01 01:14:54.000000 jcvi-1.4.7/jcvi/utils/validator.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     1376 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/utils/webcolors.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-01 04:08:29.472447 jcvi-1.4.7/jcvi/variation/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2024-05-01 01:14:54.000000 jcvi-1.4.7/jcvi/variation/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      256 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/variation/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    45325 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/variation/cnv.py
+-rw-r--r--   0 bao        (501) staff       (20)     7022 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/variation/deconvolute.py
+-rw-r--r--   0 bao        (501) staff       (20)     9360 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/variation/delly.py
+-rw-r--r--   0 bao        (501) staff       (20)    11736 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/variation/impute.py
+-rw-r--r--   0 bao        (501) staff       (20)     3440 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/variation/phase.py
+-rw-r--r--   0 bao        (501) staff       (20)    10785 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/variation/snp.py
+-rw-r--r--   0 bao        (501) staff       (20)    48803 2024-05-01 04:07:52.000000 jcvi-1.4.7/jcvi/variation/str.py
+-rw-r--r--   0 bao        (501) staff       (20)      176 2024-05-01 04:08:29.000000 jcvi-1.4.7/jcvi/version.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-01 04:08:29.446035 jcvi-1.4.7/jcvi.egg-info/
+-rw-r--r--   0 bao        (501) staff       (20)     8915 2024-05-01 04:08:29.000000 jcvi-1.4.7/jcvi.egg-info/PKG-INFO
+-rw-r--r--   0 bao        (501) staff       (20)     4543 2024-05-01 04:08:29.000000 jcvi-1.4.7/jcvi.egg-info/SOURCES.txt
+-rw-r--r--   0 bao        (501) staff       (20)        1 2024-05-01 04:08:29.000000 jcvi-1.4.7/jcvi.egg-info/dependency_links.txt
+-rw-r--r--   0 bao        (501) staff       (20)        1 2022-11-26 21:54:22.000000 jcvi-1.4.7/jcvi.egg-info/not-zip-safe
+-rw-r--r--   0 bao        (501) staff       (20)      221 2024-05-01 04:08:29.000000 jcvi-1.4.7/jcvi.egg-info/requires.txt
+-rw-r--r--   0 bao        (501) staff       (20)        5 2024-05-01 04:08:29.000000 jcvi-1.4.7/jcvi.egg-info/top_level.txt
+-rw-r--r--   0 bao        (501) staff       (20)      359 2022-11-26 21:23:29.000000 jcvi-1.4.7/pyproject.toml
+-rw-r--r--   0 bao        (501) staff       (20)     1242 2024-05-01 04:08:29.476546 jcvi-1.4.7/setup.cfg
+-rw-r--r--   0 bao        (501) staff       (20)      553 2022-11-26 21:23:29.000000 jcvi-1.4.7/setup.py
```

### Comparing `jcvi-1.4.6/LICENSE` & `jcvi-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.6/PKG-INFO` & `jcvi-1.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcvi
-Version: 1.4.6
+Version: 1.4.7
 Summary: Python utility libraries on genome assembly, annotation and comparative genomics
 Home-page: http://github.com/tanghaibao/jcvi
 Author: Haibao Tang, Vivek Krishnakumar, Jingping Li
 Author-email: tanghaibao@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jcvi-1.4.6/README.md` & `jcvi-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.6/jcvi/__init__.py` & `jcvi-1.4.7/jcvi/__init__.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.6/jcvi/algorithms/ec.py` & `jcvi-1.4.7/jcvi/algorithms/ec.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 This module contains methods to interface with DEAP evolutionary computation
 framewor, including a Genetic Algorithm (GA) based method to solve scaffold
 ordering and orientation problem.
 """
 
 import array
 import random
-import logging
 import multiprocessing
 
 from deap import base, creator, tools
 from deap.algorithms import varAnd
-from jcvi.algorithms.lis import longest_monotonic_subseq_length
-from jcvi.utils.console import printf
+
+from ..apps.base import logger
+from ..utils.console import printf
+
+from .lis import longest_monotonic_subseq_length
 
 
 # This has to be in global space, otherwise runs into error "creator.Individual
 # not found" when runnning on macOS. See also:
 # https://github.com/DEAP/deap/issues/268
 creator.create("FitnessMax", base.Fitness, weights=(1.0,))
 creator.create("Individual", array.array, typecode="i", fitness=creator.FitnessMax)
@@ -170,15 +172,15 @@
         if gen - updated > ngen:
             break
 
     return population
 
 
 def GA_run(toolbox, ngen=500, npop=100, seed=666, cpus=1, callback=None):
-    logging.debug("GA setup: ngen=%d npop=%d cpus=%d seed=%d", ngen, npop, cpus, seed)
+    logger.debug("GA setup: ngen=%d npop=%d cpus=%d seed=%d", ngen, npop, cpus, seed)
     if cpus > 1:
         pool = multiprocessing.Pool(cpus)
         toolbox.register("map", pool.map)
     random.seed(seed)
     pop = toolbox.population(n=npop)
     hof = tools.HallOfFame(1)
```

### Comparing `jcvi-1.4.6/jcvi/algorithms/formula.py` & `jcvi-1.4.7/jcvi/algorithms/formula.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.6/jcvi/algorithms/graph.py` & `jcvi-1.4.7/jcvi/algorithms/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 """
 Wrapper for the common graph algorithms.
 """
 import sys
-import logging
 
-import networkx as nx
 from collections import deque
+
+import networkx as nx
+
 from more_itertools import pairwise
 
-from jcvi.formats.base import must_open
+from ..apps.base import logger
+from ..formats.base import must_open
 
 
 """
 Bidirectional graph.
 """
 dirs = (">", "<")
 trans = str.maketrans("+?-", ">><")
@@ -200,26 +202,26 @@
         for row in fp:
             a, b = row.strip().split("--")
             oa = a[-1]
             ob = b[0]
             a, b = a.strip("<>"), b.strip("<>")
             self.add_edge(a, b, oa, ob, color=color)
             nedges += 1
-        logging.debug(
+        logger.debug(
             "A total of {0} edges imported from `{1}` (color={2}).".format(
                 nedges, filename, color
             )
         )
 
     def write(self, filename="stdout"):
 
         fw = must_open(filename, "w")
         for e in self.edges.values():
             print(e, file=fw)
-        logging.debug("Graph written to `{0}`.".format(filename))
+        logger.debug("Graph written to `{0}`.".format(filename))
 
     def draw(
         self,
         pngfile,
         dpi=96,
         verbose=False,
         namestart=0,
@@ -247,15 +249,15 @@
                 n = G.get_node(n)
                 n.attr["shape"] = "box"
 
         G.graph_attr.update(dpi=str(dpi))
         if verbose:
             G.write(sys.stderr)
         G.draw(pngfile, prog=prog)
-        logging.debug("Graph written to `{0}`.".format(pngfile))
+        logger.debug("Graph written to `{0}`.".format(pngfile))
 
     def get_next(self, node, tag="<"):
         return self.get_node(node).get_next(tag)
 
     def get_path(self, n1, n2, tag="<"):
         # return all intermediate nodes on path n1 -> n2
         path = deque()
@@ -265,27 +267,27 @@
                 return path
             path.append((next, ntag))
             next, ntag = next.get_next(tag=ntag)
         return path if n2 is None else None
 
 
 def graph_stats(G, diameter=False):
-    logging.debug("Graph stats: |V|={0}, |E|={1}".format(len(G), G.size()))
+    logger.debug("Graph stats: |V|={0}, |E|={1}".format(len(G), G.size()))
     if diameter:
         d = max(nx.diameter(H) for H in nx.connected_component_subgraphs(G))
-        logging.debug("Graph diameter: {0}".format(d))
+        logger.debug("Graph diameter: {0}".format(d))
 
 
 def graph_local_neighborhood(G, query, maxdegree=10000, maxsize=10000):
     c = [k for k, d in G.degree().iteritems() if d > maxdegree]
     if c:
-        logging.debug("Remove {0} nodes with deg > {1}".format(len(c), maxdegree))
+        logger.debug("Remove {0} nodes with deg > {1}".format(len(c), maxdegree))
     G.remove_nodes_from(c)
 
-    logging.debug("BFS search from {0}".format(query))
+    logger.debug("BFS search from {0}".format(query))
 
     queue = set(query)
     # BFS search of max depth
     seen = set(query)
     coresize = len(query)
     depth = 0
     while True:
@@ -321,15 +323,15 @@
     path_nodes = []
     for k, d in G.degree().iteritems():
         if d == 1:
             spurs.append(k)
         elif d == 2:
             path_nodes.append(k)
 
-    logging.debug("Remove {0} spurs.".format(len(spurs)))
+    logger.debug("Remove {0} spurs.".format(len(spurs)))
     G.remove_nodes_from(spurs)
 
     SG = G.subgraph(path_nodes)
     cc = nx.connected_components(SG)
     for c in cc:
         if len(c) == 1:
             continue
@@ -338,15 +340,15 @@
         for x in c:
             neighbors |= set(G.neighbors(x))
         neighbors -= c
         newtag = list(c)[0] + "*"
         for n in neighbors:
             G.add_edge(newtag, n)
         G.remove_nodes_from(c)
-    logging.debug(
+    logger.debug(
         "Contract {0} path nodes into {1} nodes.".format(len(path_nodes), len(cc))
     )
 
 
 def bigraph_test():
     g = BiGraph()
     g.add_edge(1, 2, ">", "<")
@@ -409,15 +411,15 @@
     G = transitive_reduction(G)
     return G
 
 
 def draw_graph(G, pngfile, prog="dot"):
     G = nx.to_agraph(G)
     G.draw(pngfile, prog=prog)
-    logging.debug("Graph written to `{0}`.".format(pngfile))
+    logger.debug("Graph written to `{0}`.".format(pngfile))
 
 
 def transitive_reduction(G):
     """
     Returns a transitive reduction of a graph.  The original graph
     is not modified.
```

### Comparing `jcvi-1.4.6/jcvi/algorithms/lis.py` & `jcvi-1.4.7/jcvi/algorithms/lis.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.6/jcvi/algorithms/lpsolve.py` & `jcvi-1.4.7/jcvi/algorithms/lpsolve.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,27 +20,27 @@
 ...  x3
 ... End'''
 >>> print SCIPSolver(lp_data).results
 [0, 1]
 >>> print GLPKSolver(lp_data).results
 [0, 1]
 """
-import logging
 import os.path as op
 
 from dataclasses import dataclass
 from io import StringIO
 from more_itertools import pairwise
 
 import networkx as nx
 
-from jcvi.utils.cbook import fill
-from jcvi.formats.base import flexible_cast
-from jcvi.apps.base import cleanup, mkdir, sh
-from jcvi.algorithms.tsp import populate_edge_weights, node_to_edge
+from ..apps.base import cleanup, logger, mkdir, sh
+from ..formats.base import flexible_cast
+from ..utils.cbook import fill
+
+from .tsp import populate_edge_weights, node_to_edge
 
 
 Work_dir = "lpsolve_work"
 
 # CPLEX LP format
 # <http://lpsolve.sourceforge.net/5.0/CPLEX-format.htm>
 MAXIMIZE = "Maximize"
@@ -128,15 +128,15 @@
             objective.SetCoefficient(x[j], score)
         objective.SetMaximization()
 
         return solver, x
 
     def log(self):
         """Log the size of the MIP instance"""
-        logging.info(
+        logger.info(
             "Number of variables (%d), number of constraints (%d)",
             self.num_vars,
             self.num_constraints,
         )
 
     def solve(self, work_dir="work", verbose=False):
         """Solve the MIP instance. This runs OR-tools as default solver, then
@@ -154,30 +154,30 @@
         if has_ortools():
             # Use OR-tools
             from ortools.linear_solver import pywraplp
 
             solver, x = self.create_solver()
             status = solver.Solve()
             if status == pywraplp.Solver.OPTIMAL:
-                logging.info("Objective value = %d", solver.Objective().Value())
+                logger.info("Objective value = %d", solver.Objective().Value())
                 filtered_list = [
                     j for j in range(self.num_vars) if x[j].solution_value() == 1
                 ]
-                logging.info("Problem solved in %d milliseconds", solver.wall_time())
-                logging.info("Problem solved in %d iterations", solver.iterations())
-                logging.info(
+                logger.info("Problem solved in %d milliseconds", solver.wall_time())
+                logger.info("Problem solved in %d iterations", solver.iterations())
+                logger.info(
                     "Problem solved in %d branch-and-bound nodes", solver.nodes()
                 )
 
         # Use custom formatter as a backup
         if not filtered_list:
             lp_data = self.format_lp()
             filtered_list = SCIPSolver(lp_data, work_dir, verbose=verbose).results
             if not filtered_list:
-                logging.error("SCIP fails... trying GLPK")
+                logger.error("SCIP fails... trying GLPK")
                 filtered_list = GLPKSolver(lp_data, work_dir, verbose=verbose).results
 
         return filtered_list
 
 
 class AbstractMIPSolver(object):
     """
@@ -191,28 +191,28 @@
         self.work_dir = work_dir
         self.clean = clean
         self.verbose = verbose
 
         mkdir(work_dir)
 
         lpfile = op.join(work_dir, "data.lp")  # problem instance
-        logging.debug("write MIP instance to `{0}`".format(lpfile))
+        logger.debug("Write MIP instance to `%s`", lpfile)
 
         fw = open(lpfile, "w")
         fw.write(lp_data)
         fw.close()
 
         retcode, outfile = self.run(lpfile)
         if retcode < 0:
             self.results = []
         else:
             self.results = self.parse_output(outfile)
 
         if self.results:
-            logging.debug("optimized objective value ({0})".format(self.obj_val))
+            logger.debug("Optimized objective value (%s)", self.obj_val)
 
     def run(self, lp_data):
         raise NotImplementedError
 
     def parse_output(self):
         raise NotImplementedError
 
@@ -236,17 +236,16 @@
             lpfile, outfile, listfile
         )
 
         outf = None if self.verbose else "/dev/null"
         retcode = sh(cmd, outfile=outf)
 
         if retcode == 127:
-            logging.error(
-                "You need to install program `glpsol` "
-                + "[http://www.gnu.org/software/glpk/]"
+            logger.error(
+                "You need to install program `glpsol` [http://www.gnu.org/software/glpk/]"
             )
             return -1, None
 
         return retcode, listfile
 
     def parse_output(self, listfile, clean=False):
         """Extract results from the GLPK output. The GLPK output looks like
@@ -310,17 +309,15 @@
 
         cmd = "scip -f {0} -l {1}".format(lpfile, outfile)
 
         outf = None if self.verbose else "/dev/null"
         retcode = sh(cmd, outfile=outf)
 
         if retcode == 127:
-            logging.error(
-                "You need to install program `scip` " + "[http://scip.zib.de/]"
-            )
+            logger.error("You need to install program `scip` [http://scip.zib.de/]")
             return -1, None
 
         return retcode, outfile
 
     def parse_output(self, outfile):
 
         fp = open(outfile)
@@ -776,15 +773,15 @@
         for a, b in pairwise(rc):
             cycle_edges.append(edge_to_index[a, b])
         cc = summation(cycle_edges)
         constraints.append("{0} >= 1".format(cc))
         ncycles += 1
         if ncycles == maxcycles:
             break
-    logging.debug("A total of {0} cycles found.".format(ncycles))
+    logger.debug("A total of %d cycles found.", ncycles)
 
     L.constraints = constraints
     L.add_vars(nedges)
 
     selected, obj_val = L.lpsolve(clean=False)
     if remove:
         results = (
```

### Comparing `jcvi-1.4.6/jcvi/algorithms/matrix.py` & `jcvi-1.4.7/jcvi/algorithms/matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     https://stackoverflow.com/questions/36383107/how-to-evaluate-the-sum-of-values-within-array-blocks
 
     Args:
         A (numpy.ndarray): 2D matrix
         factor (int, optional): Compact factor. Defaults to 2.
 
     Example:
-    >>> A = np.arange(16, dtype="int").reshape(4, 4); A
+    >>> A = np.arange(16, dtype=int).reshape(4, 4); A
     array([[ 0,  1,  2,  3],
            [ 4,  5,  6,  7],
            [ 8,  9, 10, 11],
            [12, 13, 14, 15]])
     >>> compact(A, factor=2)
     array([[10, 18],
            [42, 50]])
```

### Comparing `jcvi-1.4.6/jcvi/algorithms/maxsum.py` & `jcvi-1.4.7/jcvi/algorithms/maxsum.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.6/jcvi/algorithms/supermap.py` & `jcvi-1.4.7/jcvi/algorithms/supermap.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,20 +9,19 @@
 
 In order to handle dups, we have to run two monotonic chains in both genomes,
 first chain using ref, and a second chain using query and we will have options
 to keep either the union or the intersection of retain chained alignments from
 both genomes, similar to the SUPERMAP algorithm. This operation is symmetrical.
 """
 import sys
-import logging
 
-from jcvi.apps.base import OptionParser
-from jcvi.formats.blast import BlastLine
-from jcvi.formats.coords import CoordsLine
-from jcvi.utils.range import Range, range_chain
+from ..apps.base import OptionParser, logger
+from ..formats.blast import BlastLine
+from ..formats.coords import CoordsLine
+from ..utils.range import Range, range_chain
 
 
 def BlastOrCoordsLine(filename, filter="ref", dialect="blast", clip=0):
     allowed_filters = ("ref", "query")
     REF, QUERY = range(len(allowed_filters))
 
     allowed_dialects = ("blast", "coords")
@@ -67,44 +66,44 @@
 
         yield Range(query, start, end, b.score, i)
 
 
 def supermap(blast_file, filter="intersection", dialect="blast", clip=0):
     # filter by query
     if filter != "ref":
-        logging.debug("filter by query")
+        logger.debug("filter by query")
         ranges = list(
             BlastOrCoordsLine(blast_file, filter="query", dialect=dialect, clip=clip)
         )
 
         query_selected, query_score = range_chain(ranges)
         query_idx = set(x.id for x in query_selected)
 
     # filter by ref
     if filter != "query":
-        logging.debug("filter by ref")
+        logger.debug("filter by ref")
         ranges = list(
             BlastOrCoordsLine(blast_file, filter="ref", dialect=dialect, clip=clip)
         )
 
         ref_selected, ref_score = range_chain(ranges)
         ref_idx = set(x.id for x in ref_selected)
 
     if filter == "ref":
         selected_idx = ref_idx
 
     elif filter == "query":
         selected_idx = query_idx
 
     elif filter == "intersection":
-        logging.debug("perform intersection")
+        logger.debug("perform intersection")
         selected_idx = ref_idx & query_idx
 
     elif filter == "union":
-        logging.debug("perform union")
+        logger.debug("perform union")
         selected_idx = ref_idx | query_idx
 
     assert len(selected_idx) != 0
 
     # selected_idx is in fact the lineno in the BLAST file
     fp = open(blast_file)
 
@@ -122,15 +121,15 @@
             continue
         print(row.rstrip(), file=fw)
         try:
             selected = next(selected_idx)
         except StopIteration:
             break
 
-    logging.debug("Write output file to `{0}`".format(supermapfile))
+    logger.debug("Write output file to `{0}`".format(supermapfile))
     fw.close()
 
     from jcvi.formats.blast import sort
 
     ofilter = "ref" if filter == "ref" else "query"
     args = [supermapfile, "--" + ofilter]
     if dialect == "coords":
@@ -143,35 +142,35 @@
 
 if __name__ == "__main__":
 
     p = OptionParser(__doc__)
 
     filter_choices = ("ref", "query", "intersection", "union")
     dialect_choices = ("blast", "coords")
-    p.add_option(
+    p.add_argument(
         "--filter",
         choices=filter_choices,
         default="intersection",
         help="Available filters",
     )
-    p.add_option("--dialect", choices=dialect_choices, help="Input format")
-    p.add_option(
+    p.add_argument("--dialect", choices=dialect_choices, help="Input format")
+    p.add_argument(
         "--clip",
         default=0,
-        type="int",
+        type=int,
         help="Clip ranges so that to allow minor overlaps",
     )
 
     opts, args = p.parse_args()
 
     if len(args) != 1:
         sys.exit(p.print_help())
 
     (blast_file,) = args
 
     dialect = opts.dialect
     if not dialect:
         # guess from the suffix
         dialect = "coords" if blast_file.endswith(".coords") else "blast"
-        logging.debug("dialect is %s" % dialect)
+        logger.debug("dialect is %s" % dialect)
 
     supermap(blast_file, filter=opts.filter, dialect=dialect, clip=opts.clip)
```

### Comparing `jcvi-1.4.6/jcvi/algorithms/tsp.py` & `jcvi-1.4.7/jcvi/algorithms/tsp.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 
 """
 TSP solver using Concorde or OR-tools. This is much faster than the LP-formulation in
 algorithms.lpsolve.tsp(). See also:
 https://developers.google.com/optimization/routing/tsp
 """
 import os.path as op
-import logging
-import numpy as np
 
 from collections import defaultdict
 from dataclasses import dataclass
 from itertools import combinations
+
+import numpy as np
+
 from more_itertools import pairwise
 
 from jcvi.formats.base import must_open
-from jcvi.apps.base import cleanup, mkdir, sh, which
+from jcvi.apps.base import cleanup, logger, mkdir, sh, which
 
 
 INF = 10000
 NEG_INF = -INF
 Work_dir = "tsp_work"
 
 
@@ -39,15 +40,15 @@
         nnodes = len(nodes)
 
         # TSPLIB requires explicit weights to be integral, and non-negative
         weights = [x[-1] for x in self.edges]
         max_x, min_x = max(weights), min(weights)
         inf = 2 * max(abs(max_x), abs(min_x))
         factor = 10**precision
-        logging.debug(
+        logger.debug(
             "TSP rescale: max_x=%d, min_x=%d, inf=%d, factor=%d",
             max_x,
             min_x,
             inf,
             factor,
         )
 
@@ -104,23 +105,23 @@
         )
         search_parameters.time_limit.seconds = time_limit
 
         # Solve the problem
         solution = routing.SolveWithParameters(search_parameters)
 
         tour = []
-        logging.info("Objective: %d", solution.ObjectiveValue())
+        logger.info("Objective: %d", solution.ObjectiveValue())
         index = routing.Start(0)
         route_distance = 0
         while not routing.IsEnd(index):
             tour.append(manager.IndexToNode(index))
             previous_index = index
             index = solution.Value(routing.NextVar(index))
             route_distance = routing.GetArcCostForVehicle(previous_index, index, 0)
-        logging.info("Route distance: %d", route_distance)
+        logger.info("Route distance: %d", route_distance)
 
         return [nodes[x] for x in tour]
 
 
 class Concorde(object):
     def __init__(
         self,
@@ -185,15 +186,15 @@
         print("EDGE_WEIGHT_SECTION", file=fw)
 
         for row in D:  # Dump the full matrix
             print(" " + " ".join(str(x) for x in row), file=fw)
 
         print("EOF", file=fw)
         fw.close()
-        logging.debug("Write TSP instance to `%s`", tspfile)
+        logger.debug("Write TSP instance to `%s`", tspfile)
 
     def run_concorde(self, tspfile, seed=666):
         outfile = op.join(self.work_dir, "data.sol")
         cleanup(outfile)
 
         cc = "concorde"
         assert which(cc), (
```

### Comparing `jcvi-1.4.6/jcvi/annotation/ahrd.py` & `jcvi-1.4.7/jcvi/annotation/ahrd.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 
 """
 Utility to run Automated Human Readable Description (AHRD) pipeline.
 
 <https://github.com/groupschoof/AHRD>
 """
 import os.path as op
-from os import symlink
 import sys
 import re
-import logging
 
-from jcvi.formats.base import must_open
-from jcvi.apps.base import OptionParser, ActionDispatcher, mkdir, glob
+from os import symlink
+
+from ..apps.base import ActionDispatcher, OptionParser, logger, mkdir, glob
+from ..formats.base import must_open
 
 
 # --- Compiled RegExps ----
 # Cellular locations
 loc_pat = re.compile(r",\s*(chloroplastic|cytoplasmic|mitochondrial).*?\s$", re.I)
 # Any word that matches e.g. Os02g0234800
 osg_pat = re.compile(r"\bOs\d{2}g\d{7}.*?\s", re.I)
@@ -550,15 +550,15 @@
 def fix(args):
     """
     %prog fix ahrd.csv > ahrd.fixed.csv
 
     Fix ugly names from Uniprot.
     """
     p = OptionParser(fix.__doc__)
-    p.add_option(
+    p.add_argument(
         "--ignore_sym_pat",
         default=False,
         action="store_true",
         help="Do not fix names matching symbol patterns i.e."
         + " names beginning or ending with gene symbols or a series of numbers."
         + " e.g. `ARM repeat superfamily protein`, `beta-hexosaminidase 3`,"
         + " `CYCLIN A3;4`, `WALL ASSOCIATED KINASE (WAK)-LIKE 10`",
@@ -621,15 +621,15 @@
                 continue
             if row.strip() == header:
                 continue
 
             atoms = row.rstrip().split("\t")
             id = atoms[0]
             if id in seen:
-                logging.error("ID `{0}` ignored.".format(id))
+                logger.error("ID `%s` ignored.", id)
                 continue
 
             seen.add(id)
             print(row.strip())
 
 
 def batch(args):
@@ -646,27 +646,27 @@
     $ parallel java -Xmx2g -jar ~/code/AHRD/dist/ahrd.jar {} ::: output/*.yml
     """
     p = OptionParser(batch.__doc__)
 
     ahrd_weights = {"blastp": [0.5, 0.3, 0.2], "blastx": [0.6, 0.4, 0.0]}
     blast_progs = tuple(ahrd_weights.keys())
 
-    p.add_option(
+    p.add_argument(
         "--path",
         default="~/code/AHRD/",
         help="Path where AHRD is installed",
     )
-    p.add_option(
+    p.add_argument(
         "--blastprog",
         default="blastp",
         choices=blast_progs,
         help="Specify the blast program being run. Based on this option,"
         + " the AHRD parameters (score_weights) will be modified",
     )
-    p.add_option(
+    p.add_argument(
         "--iprscan",
         default=None,
         help="Specify path to InterProScan results file if available."
         + " If specified, the yml conf file will be modified"
         + " appropriately",
     )
```

### Comparing `jcvi-1.4.6/jcvi/annotation/automaton.py` & `jcvi-1.4.7/jcvi/annotation/automaton.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 
 """
 Automate genome annotation by iterating processing a set of files, individually.
 """
 
 import os.path as op
 import sys
-import logging
 
 from functools import partial
 from tempfile import mkdtemp
 
-from jcvi.assembly.automaton import iter_project
-from jcvi.apps.grid import Jobs, MakeManager
-from jcvi.formats.base import FileMerger, split
-from jcvi.apps.base import (
+from ..assembly.automaton import iter_project
+from ..apps.grid import Jobs, MakeManager
+from ..formats.base import FileMerger, split
+from ..apps.base import (
     ActionDispatcher,
     OptionParser,
     cleanup,
     iglob,
+    logger,
     mkdir,
     need_update,
     sh,
 )
 
 
 def main():
@@ -59,17 +59,21 @@
     """
     %prog augustus fastafile
 
     Run parallel AUGUSTUS. Final results can be reformatted using
     annotation.reformat.augustus().
     """
     p = OptionParser(augustus.__doc__)
-    p.add_option("--species", default="maize", help="Use species model for prediction")
-    p.add_option("--hintsfile", help="Hint-guided AUGUSTUS")
-    p.add_option("--nogff3", default=False, action="store_true", help="Turn --gff3=off")
+    p.add_argument(
+        "--species", default="maize", help="Use species model for prediction"
+    )
+    p.add_argument("--hintsfile", help="Hint-guided AUGUSTUS")
+    p.add_argument(
+        "--nogff3", default=False, action="store_true", help="Turn --gff3=off"
+    )
     p.set_home("augustus")
     p.set_cpus()
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
@@ -108,15 +112,15 @@
 def star(args):
     """
     %prog star folder reference
 
     Run star on a folder with reads.
     """
     p = OptionParser(star.__doc__)
-    p.add_option(
+    p.add_argument(
         "--single", default=False, action="store_true", help="Single end mapping"
     )
     p.set_fastq_names()
     p.set_cpus()
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
@@ -159,15 +163,15 @@
 def cufflinks(args):
     """
     %prog cufflinks folder reference
 
     Run cufflinks on a folder containing tophat results.
     """
     p = OptionParser(cufflinks.__doc__)
-    p.add_option("--gtf", help="Reference annotation")
+    p.add_argument("--gtf", help="Reference annotation")
     p.set_cpus()
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     folder, reference = args
@@ -215,34 +219,34 @@
 
     Run tophat on a folder of reads.
     """
     from jcvi.apps.bowtie import check_index
     from jcvi.formats.fastq import guessoffset
 
     p = OptionParser(tophat.__doc__)
-    p.add_option("--gtf", help="Reference annotation")
-    p.add_option(
+    p.add_argument("--gtf", help="Reference annotation")
+    p.add_argument(
         "--single", default=False, action="store_true", help="Single end mapping"
     )
-    p.add_option(
+    p.add_argument(
         "--intron",
         default=15000,
-        type="int",
+        type=int,
         help="Max intron size",
     )
-    p.add_option(
+    p.add_argument(
         "--dist",
         default=-50,
-        type="int",
+        type=int,
         help="Mate inner distance",
     )
-    p.add_option(
+    p.add_argument(
         "--stdev",
         default=50,
-        type="int",
+        type=int,
         help="Mate standard deviation",
     )
     p.set_phred()
     p.set_cpus()
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
@@ -251,15 +255,15 @@
     num = 1 if opts.single else 2
     folder, reference = args
     reference = check_index(reference)
     for p, prefix in iter_project(folder, n=num):
         outdir = "{0}_tophat".format(prefix)
         outfile = op.join(outdir, "accepted_hits.bam")
         if op.exists(outfile):
-            logging.debug("File `{0}` found. Skipping.".format(outfile))
+            logger.debug("File `%s` found. Skipping.", outfile)
             continue
 
         cmd = "tophat -p {0}".format(opts.cpus)
         if opts.gtf:
             cmd += " -G {0}".format(opts.gtf)
         cmd += " -o {0}".format(outdir)
```

### Comparing `jcvi-1.4.6/jcvi/annotation/depth.py` & `jcvi-1.4.7/jcvi/annotation/depth.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 """
 From genomeCovergeBed results, initialize the count array, set cutoffs
 and optimize against the truth, to determine the cutoff for incorporating
 RNA-seq into annotation pipelines.
 """
 import sys
 import os.path as op
-import numpy as np
-import logging
 
 from itertools import groupby
 
-from jcvi.formats.sizes import Sizes
-from jcvi.formats.base import BaseFile, must_open
-from jcvi.apps.base import OptionParser, ActionDispatcher
+import numpy as np
+
+from ..apps.base import ActionDispatcher, OptionParser, logger
+from ..formats.base import BaseFile, must_open
+from ..formats.sizes import Sizes
 
 
 class BinFile(BaseFile):
     """
     The binfile contains per base count, fastafile provides the coordinate
     system.
     """
@@ -60,25 +60,25 @@
 def bed(args):
     """
     %prog bed binfile fastafile
 
     Write bed files where the bases have at least certain depth.
     """
     p = OptionParser(bed.__doc__)
-    p.add_option(
+    p.add_argument(
         "-o",
         dest="output",
         default="stdout",
         help="Output file name",
     )
-    p.add_option(
+    p.add_argument(
         "--cutoff",
         dest="cutoff",
         default=10,
-        type="int",
+        type=int,
         help="Minimum read depth to report intervals",
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
@@ -127,34 +127,34 @@
 
     if len(args) < 2:
         sys.exit(not p.print_help())
 
     binfiles = args[:-1]
     mergedbin = args[-1]
     if op.exists(mergedbin):
-        logging.error("`{0}` file exists. Remove before proceed.".format(mergedbin))
+        logger.error("`{0}` file exists. Remove before proceed.".format(mergedbin))
         return
 
     b = BinFile(binfiles[0])
     ar = b.mmarray
     (fastasize,) = ar.shape
-    logging.debug("Initialize array of uint16 with size {0}".format(fastasize))
+    logger.debug("Initialize array of uint16 with size {0}".format(fastasize))
 
     merged_ar = np.zeros(fastasize, dtype=np.uint16)
     for binfile in binfiles:
         b = BinFile(binfile)
         merged_ar += b.array
 
-    logging.debug("Resetting the count max to 255.")
+    logger.debug("Resetting the count max to 255.")
     merged_ar[merged_ar > 255] = 255
 
-    logging.debug("Compact array back to uint8 with size {0}".format(fastasize))
+    logger.debug("Compact array back to uint8 with size {0}".format(fastasize))
     merged_ar = np.array(merged_ar, dtype=np.uint8)
     merged_ar.tofile(mergedbin)
-    logging.debug("Merged array written to `{0}`".format(mergedbin))
+    logger.debug("Merged array written to `{0}`".format(mergedbin))
 
 
 def query(args):
     """
     %prog query binfile fastafile ctgID baseID
 
     Get the depth at a particular base.
@@ -172,15 +172,15 @@
     fastasize, sizes, offsets = get_offsets(fastafile)
     oi = offsets[ctgID] + int(baseID) - 1
     print("\t".join((ctgID, baseID, str(ar[oi]))))
 
 
 def update_array(ar, coveragefile, offsets):
     fp = open(coveragefile)
-    logging.debug("Parse file `{0}`".format(coveragefile))
+    logger.debug("Parse file `{0}`".format(coveragefile))
     for k, rows in groupby(fp, key=(lambda x: x.split()[0])):
         rows = list(rows)
         offset = offsets[k]
         ctglen = len(rows)
 
         if ctglen < 100000:
             sys.stdout.write(".")
@@ -219,22 +219,22 @@
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     coveragefile, fastafile = args
 
     countsfile = coveragefile.split(".")[0] + ".bin"
     if op.exists(countsfile):
-        logging.error("`{0}` file exists. Remove before proceed.".format(countsfile))
+        logger.error("`{0}` file exists. Remove before proceed.".format(countsfile))
         return
 
     fastasize, sizes, offsets = get_offsets(fastafile)
-    logging.debug("Initialize array of uint8 with size {0}".format(fastasize))
+    logger.debug("Initialize array of uint8 with size {0}".format(fastasize))
     ar = np.zeros(fastasize, dtype=np.uint8)
 
     update_array(ar, coveragefile, offsets)
 
     ar.tofile(countsfile)
-    logging.debug("Array written to `{0}`".format(countsfile))
+    logger.debug("Array written to `{0}`".format(countsfile))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `jcvi-1.4.6/jcvi/annotation/evm.py` & `jcvi-1.4.7/jcvi/annotation/evm.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 communicates with GFF file.
 """
 import os.path as op
 import sys
 
 from collections import defaultdict
 
-from jcvi.formats.fasta import ids
-from jcvi.formats.base import write_file
-from jcvi.apps.base import OptionParser, ActionDispatcher, need_update, sh
+from ..apps.base import ActionDispatcher, OptionParser, need_update, sh
+from ..formats.base import write_file
+from ..formats.fasta import ids
 
 
 EVMRUN = r"""
 W=`pwd`/weights.txt
 
 $EVM/EvmUtils/write_EVM_commands.pl --genome genome.fasta --weights $W \
     --gene_predictions {0} \
```

### Comparing `jcvi-1.4.6/jcvi/annotation/maker.py` & `jcvi-1.4.7/jcvi/annotation/maker.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,30 +7,30 @@
 Many of the routines in this script is to select among a set of conflicting
 models, either through accuracy (batcheval) or simply the length (longest).
 """
 
 import os
 import os.path as op
 import sys
-import logging
 
 from collections import Counter, defaultdict
 
-from jcvi.formats.base import BaseFile, LineFile, write_file
-from jcvi.apps.grid import GridProcess, get_grid_engine, PBS_STANZA
-from jcvi.apps.base import (
-    OptionParser,
+from ..apps.grid import GridProcess, get_grid_engine, PBS_STANZA
+from ..apps.base import (
     ActionDispatcher,
+    OptionParser,
+    logger,
     need_update,
     popen,
     sh,
     mkdir,
     glob,
     get_abs_path,
 )
+from ..formats.base import BaseFile, LineFile, write_file
 
 
 class CTLine(object):
     def __init__(self, row):
         row = row.strip()
         tag = value = real = comment = ""
         if "#" in row:
@@ -66,30 +66,30 @@
         fp.close()
 
     def update_abs_path(self):
         for r in self:
             path = r.value
             if path and op.exists(path):
                 npath = get_abs_path(path)
-                logging.debug("{0}={1} => {2}".format(r.tag, path, npath))
+                logger.debug("{0}={1} => {2}".format(r.tag, path, npath))
                 r.value = npath
 
     def update_tag(self, key, value):
         for r in self:
             if r.tag == key:
-                logging.debug("{0}={1} => {2}".format(r.tag, r.value, value))
+                logger.debug("{0}={1} => {2}".format(r.tag, r.value, value))
                 r.value = value
                 break
 
     def write_file(self, filename):
         fw = open(filename, "w")
         for r in self:
             print(r, file=fw)
         fw.close()
-        logging.debug("File written to `%s`.", filename)
+        logger.debug("File written to `%s`.", filename)
 
 
 class DatastoreIndexFile(BaseFile):
     def __init__(self, filename):
         super(DatastoreIndexFile, self).__init__(filename)
         scaffold_status = {}
         failed = []
@@ -273,15 +273,15 @@
     fw = open(gfflist, "w")
     print("\n".join(gffnames), file=fw)
     fw.close()
 
     nlines = sum(1 for _ in open(gfflist))
     assert nlines == nfs  # Be extra, extra careful to include all results
     gmerge([gfflist, "-o", outputgff])
-    logging.debug("Merged GFF file written to `{0}`".format(outputgff))
+    logger.debug("Merged GFF file written to `{0}`".format(outputgff))
 
 
 def validate(args):
     """
     %prog validate outdir genome.fasta
 
     Validate current folder after MAKER run and check for failures. Failed batch
@@ -347,15 +347,15 @@
 
     Outfile contains the scores for the models can be found in models.scores
     """
     from jcvi.formats.bed import evaluate
     from jcvi.formats.gff import make_index
 
     p = OptionParser(evaluate.__doc__)
-    p.add_option(
+    p.add_argument(
         "--type",
         default="CDS",
         help="list of features to extract, use comma to separate (e.g."
         "'five_prime_UTR,CDS,three_prime_UTR')",
     )
     opts, args = p.parse_args(args)
 
@@ -446,25 +446,25 @@
     `split.bed` can be generated by pulling out subset from a list of ids
     $ python -m jcvi.formats.base join split.ids working.bed
         --column=0,3 --noheader | cut -f2-7 > split.bed
     """
     from jcvi.formats.bed import Bed
 
     p = OptionParser(split.__doc__)
-    p.add_option(
+    p.add_argument(
         "--key",
         default="Name",
         help="Key in the attributes to extract predictor.gff",
     )
-    p.add_option(
+    p.add_argument(
         "--parents",
         default="match",
         help="list of features to extract, use comma to separate (e.g.'gene,mRNA')",
     )
-    p.add_option(
+    p.add_argument(
         "--children",
         default="match_part",
         help="list of features to extract, use comma to separate (e.g."
         "'five_prime_UTR,CDS,three_prime_UTR')",
     )
     opts, args = p.parse_args(args)
```

### Comparing `jcvi-1.4.6/jcvi/annotation/pasa.py` & `jcvi-1.4.7/jcvi/annotation/pasa.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 
 """
 Utilities for submitting PASA jobs and processing PASA results.
 """
 import os
 import os.path as op
 import sys
-import logging
 
-from jcvi.formats.base import write_file, must_open, FileMerger
-from jcvi.apps.base import OptionParser, ActionDispatcher, sh, symlink, which
+from ..apps.base import ActionDispatcher, OptionParser, logger, sh, symlink, which
+from ..formats.base import write_file, must_open, FileMerger
 
 
 alignAssembly_conf = """
 # MySQL settings
 MYSQLDB={0}
 
 #script validate_alignments_in_db.dbi
@@ -77,15 +76,15 @@
     protocol is followed <http://pasa.sourceforge.net/#A_ComprehensiveTranscriptome>
 
     Using the `--prepare` option creates a shell script with the run commands without
     executing the pipeline
     """
     p = OptionParser(assemble.__doc__)
     p.set_pasa_opts()
-    p.add_option(
+    p.add_argument(
         "--prepare",
         default=False,
         action="store_true",
         help="Prepare PASA run script with commands",
     )
     p.set_grid()
     p.set_grid_opts()
@@ -99,22 +98,22 @@
         genome,
         dnfasta,
     ) = args[:3]
     ggfasta = args[3] if len(args) == 4 else None
 
     PASA_HOME = opts.pasa_home
     if not op.isdir(PASA_HOME):
-        logging.error("PASA_HOME={0} directory does not exist".format(PASA_HOME))
+        logger.error("PASA_HOME={0} directory does not exist".format(PASA_HOME))
         sys.exit()
 
     aligners = opts.aligners.split(",")
     for aligner in aligners:
         if aligner not in ALLOWED_ALIGNERS:
-            logging.error("Error: Unknown aligner `{0}`".format(aligner))
-            logging.error(
+            logger.error("Error: Unknown aligner `{0}`".format(aligner))
+            logger.error(
                 "Can be any of {0}, ".format("|".join(ALLOWED_ALIGNERS))
                 + "combine multiple aligners in list separated by comma"
             )
             sys.exit()
 
     clean = opts.clean
     seqclean = op.join(opts.tgi_home, "seqclean")
@@ -224,15 +223,15 @@
     loaded annotation data.
 
     Using the `--prepare` option creates a shell script with the run commands without
     executing the pipeline
     """
     p = OptionParser(compare.__doc__)
     p.set_pasa_opts(action="compare")
-    p.add_option(
+    p.add_argument(
         "--prepare",
         default=False,
         action="store_true",
         help="Prepare PASA run script with commands",
     )
     p.set_grid()
     p.set_grid_opts()
@@ -241,15 +240,15 @@
     if len(args) < 1:
         sys.exit(not p.print_help())
 
     (pasa_db,) = args
 
     PASA_HOME = opts.pasa_home
     if not op.isdir(PASA_HOME):
-        logging.error("PASA_HOME={0} directory does not exist".format(PASA_HOME))
+        logger.error("PASA_HOME={0} directory does not exist".format(PASA_HOME))
         sys.exit()
 
     launch_pasa = which(op.join(PASA_HOME, "scripts", "Launch_PASA_pipeline.pl"))
 
     annots_gff3 = opts.annots_gff3
     grid = opts.grid
     prepare, runfile = opts.prepare, "run.sh"
@@ -316,15 +315,15 @@
 
     sub-cluster: asmbl_25 asmbl_26 asmbl_27
     """
     from jcvi.formats.fasta import Fasta, SeqIO
     from jcvi.formats.sizes import Sizes
 
     p = OptionParser(longest.__doc__)
-    p.add_option(
+    p.add_argument(
         "--prefix",
         default="pasa",
         help="Replace asmbl_ with prefix",
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
@@ -350,15 +349,15 @@
         longest_size = sizes[longest_asmbl]
         print(name_convert(longest_asmbl), file=fw)
         nrecs += 1
         cutoff = max(longest_size / 2, 200)
         keep.update(set(x for x in asmbls if sizes[x] >= cutoff))
 
     fw.close()
-    logging.debug("{0} fl-cDNA records written to `{1}`.".format(nrecs, idsfile))
+    logger.debug("{0} fl-cDNA records written to `{1}`.".format(nrecs, idsfile))
 
     f = Fasta(fastafile, lazy=True)
     newfastafile = prefix + ".clean.fasta"
     fw = open(newfastafile, "w")
     nrecs = 0
     for name, rec in f.iteritems_ordered():
         if name not in keep:
@@ -366,15 +365,15 @@
 
         rec.id = name_convert(name)
         rec.description = ""
         SeqIO.write([rec], fw, "fasta")
         nrecs += 1
 
     fw.close()
-    logging.debug("{0} valid records written to `{1}`.".format(nrecs, newfastafile))
+    logger.debug("{0} valid records written to `{1}`.".format(nrecs, newfastafile))
 
 
 def consolidate(args):
     """
     %prog consolidate gffile1 gffile2 ... > consolidated.out
 
     Given 2 or more gff files generated by pasa annotation comparison,
@@ -389,39 +388,39 @@
     from jcvi.formats.gff import make_index, match_subfeats
     from jcvi.utils.cbook import AutoVivification
     from jcvi.utils.grouper import Grouper
     from itertools import combinations, product
 
     supported_modes = ["name", "coords"]
     p = OptionParser(consolidate.__doc__)
-    p.add_option(
+    p.add_argument(
         "--slop",
         default=False,
         action="store_true",
         help="allow minor variation in terminal 5'/3' UTR start/stop position",
     )
-    p.add_option(
+    p.add_argument(
         "--inferUTR",
         default=False,
         action="store_true",
         help="infer presence of UTRs from exon coordinates",
     )
-    p.add_option(
+    p.add_argument(
         "--mode",
         default="name",
         choices=supported_modes,
         help="method used to determine overlapping loci",
     )
-    p.add_option(
+    p.add_argument(
         "--summary",
         default=False,
         action="store_true",
         help="Generate summary table of consolidation process",
     )
-    p.add_option(
+    p.add_argument(
         "--clusters",
         default=False,
         action="store_true",
         help="Generate table of cluster members after consolidation",
     )
     p.set_outfile()
```

### Comparing `jcvi-1.4.6/jcvi/annotation/qc.py` & `jcvi-1.4.7/jcvi/annotation/qc.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 testing. Several aspects of annotation QC are implemented in this script.
 
 - Trim UTRs. MAKER sometimes predict UTRs that extend into other genes.
 - Remove overlapping models.
 """
 import sys
 
-from jcvi.formats.gff import (
+from ..apps.base import ActionDispatcher, OptionParser
+from ..formats.gff import (
     Gff,
     get_piles,
     make_index,
     import_feats,
     populate_children,
     to_range,
 )
-from jcvi.formats.base import must_open
-from jcvi.formats.sizes import Sizes
-from jcvi.utils.range import range_minmax, range_chain, range_overlap
-from jcvi.apps.base import OptionParser, ActionDispatcher
+from ..formats.base import must_open
+from ..formats.sizes import Sizes
+from ..utils.range import range_chain, range_minmax, range_overlap
 
 
 def main():
 
     actions = (
         ("trimUTR", "remove UTRs in the annotation set"),
         ("uniq", "remove overlapping gene models"),
@@ -161,37 +161,37 @@
     `python -m jcvi.formats.gff fixboundaries` on the resultant GFF3
     to adjust the boundaries of all parent 'gene' features
     """
     import gffutils
     from jcvi.formats.base import SetFile
 
     p = OptionParser(trimUTR.__doc__)
-    p.add_option(
+    p.add_argument(
         "--trim5",
         default=None,
-        type="str",
+        type=str,
         help="File containing gene list for 5' UTR trimming",
     )
-    p.add_option(
+    p.add_argument(
         "--trim3",
         default=None,
-        type="str",
+        type=str,
         help="File containing gene list for 3' UTR trimming",
     )
-    p.add_option(
+    p.add_argument(
         "--trimrange",
         default=None,
-        type="str",
+        type=str,
         help="File containing gene list for UTR trim back"
         + "based on suggested (start, stop) coordinate range",
     )
-    p.add_option(
+    p.add_argument(
         "--refgff",
         default=None,
-        type="str",
+        type=str,
         help="Reference GFF3 used as fallback to replace UTRs",
     )
     p.set_outfile()
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
```

### Comparing `jcvi-1.4.6/jcvi/annotation/reformat.py` & `jcvi-1.4.7/jcvi/annotation/reformat.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,32 +5,31 @@
 Convert common output files from gene prediction software into gff3 format.
 
 Similar to the utilities in DAWGPAWS.
 <http://dawgpaws.sourceforge.net/man.html>
 """
 import os
 import sys
-import logging
 import re
 
 from collections import defaultdict
 from itertools import groupby, product
 
-from jcvi.utils.cbook import AutoVivification
-from jcvi.formats.bed import Bed, BedLine, sort
-from jcvi.formats.base import SetFile, must_open, get_number, flexible_cast
-from jcvi.apps.base import (
-    OptionParser,
-    OptionGroup,
+from ..apps.base import (
     ActionDispatcher,
+    OptionParser,
     cleanup,
+    logger,
     need_update,
     popen,
     sh,
 )
+from ..utils.cbook import AutoVivification
+from ..formats.bed import Bed, BedLine, sort
+from ..formats.base import SetFile, flexible_cast, get_number, must_open
 
 
 FRAME, RETAIN, OVERLAP, NEW = "FRAME", "RETAIN", "OVERLAP", "NEW"
 PRIORITY = (FRAME, RETAIN, OVERLAP, NEW)
 
 new_id_pat = re.compile(r"^\d+\.[cemtx]+\S+")
 atg_name_pat = re.compile(
@@ -206,17 +205,17 @@
     Plot gene identifiers along a particular chromosome, often to illustrate the
     gene id assignment procedure.
     """
     from jcvi.graphics.base import plt, savefig
     from jcvi.graphics.chromosome import ChromosomeMap
 
     p = OptionParser(plot.__doc__)
-    p.add_option("--firstn", type="int", help="Only plot the first N genes")
-    p.add_option("--ymax", type="int", help="Y-axis max value")
-    p.add_option("--log", action="store_true", help="Write plotting data")
+    p.add_argument("--firstn", type=int, help="Only plot the first N genes")
+    p.add_argument("--ymax", type=int, help="Y-axis max value")
+    p.add_argument("--log", action="store_true", help="Write plotting data")
     opts, args, iopts = p.set_image_options(args, figsize="6x4")
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     taggedbed, chr = args
     bed = Bed(taggedbed)
@@ -238,15 +237,15 @@
         else:
             old.append((i, r))
         i += 1
 
     ngenes = i
     assert ngenes == len(new) + len(old)
 
-    logging.debug("Imported {0} ranks on {1}.".format(ngenes, chr))
+    logger.debug("Imported {0} ranks on {1}.".format(ngenes, chr))
     fig = plt.figure(1, (iopts.w, iopts.h))
     root = fig.add_axes([0, 0, 1, 1])
 
     xstart, xend = 0.2, 0.8
     ystart, yend = 0.2, 0.8
     pad = 0.02
 
@@ -302,15 +301,15 @@
     """
     %prog instantiate tagged.bed blacklist.ids big_gaps.bed
 
     instantiate NEW genes tagged by renumber.
     """
     p = OptionParser(instantiate.__doc__)
     p.set_annot_reformat_opts()
-    p.add_option(
+    p.add_argument(
         "--extended_stride",
         default=False,
         action="store_true",
         help="Toggle extended strides for gene numbering",
     )
     opts, args = p.parse_args(args)
 
@@ -453,15 +452,15 @@
         new_accns = []
         for accn in accns:
             if ":" in accn:
                 method, a = accn.split(":", 1)
                 if method in ("liftOver", "GMAP", ""):
                     accn = a
             if accn in seen:
-                logging.error("Duplicate id {0} found. Ignored.".format(accn))
+                logger.error("Duplicate id {0} found. Ignored.".format(accn))
                 continue
 
             new_accns.append(accn)
             b.accn = accn
             print(b, file=fwa)
             seen.add(accn)
 
@@ -591,121 +590,117 @@
     Adjust the value of `new_id_pat` manually as per your ID naming conventions.
     """
     from jcvi.utils.grouper import Grouper
 
     valid_resolve_choices = ["alignment", "overlap"]
 
     p = OptionParser(annotate.__doc__)
-    p.add_option(
+    p.add_argument(
         "--resolve",
         default="alignment",
         choices=valid_resolve_choices,
         help="Resolve ID assignment based on a certain metric",
     )
-    p.add_option(
+    p.add_argument(
         "--atg_name",
         default=False,
         action="store_true",
         help="Specify is locus IDs in `new.bed` file follow ATG nomenclature",
     )
 
-    g1 = OptionGroup(
-        p,
+    g1 = p.add_argument_group(
         "Optional parameters (alignment):\n"
         + "Use if resolving ambiguities based on sequence `alignment`",
     )
-    g1.add_option(
+    g1.add_argument(
         "--pid",
         dest="pid",
         default=35.0,
-        type="float",
+        type=float,
         help="Percent identity cutoff",
     )
-    g1.add_option(
+    g1.add_argument(
         "--score",
         dest="score",
         default=250.0,
-        type="float",
+        type=float,
         help="Alignment score cutoff",
     )
-    p.add_option_group(g1)
 
-    g2 = OptionGroup(
-        p,
+    g2 = p.add_argument_group(
         "Optional parameters (overlap):\n"
         + "Use if resolving ambiguities based on `overlap` length\n"
         + "Parameters equivalent to `intersectBed`",
     )
-    g2.add_option(
+    g2.add_argument(
         "-f",
         dest="f",
         default=0.5,
-        type="float",
+        type=float,
         help="Minimum overlap fraction (0.0 - 1.0)",
     )
-    g2.add_option(
+    g2.add_argument(
         "-r",
         dest="r",
         default=False,
         action="store_true",
         help="Require fraction overlap to be reciprocal",
     )
-    g2.add_option(
+    g2.add_argument(
         "-s",
         dest="s",
         default=True,
         action="store_true",
         help="Require same strandedness",
     )
-    p.add_option_group(g2)
 
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     nbedfile, obedfile = args
     npf, opf = nbedfile.rsplit(".", 1)[0], obedfile.rsplit(".", 1)[0]
 
     # Make consolidated.bed
     cbedfile = "consolidated.bed"
     if not os.path.isfile(cbedfile):
         consolidate(nbedfile, obedfile, cbedfile)
     else:
-        logging.warning("`{0}` already exists. Skipping step".format(cbedfile))
+        logger.warning("`{0}` already exists. Skipping step".format(cbedfile))
 
-    logging.warning(
+    logger.warning(
         "Resolving ID assignment ambiguity based on `{0}`".format(opts.resolve)
     )
 
     if opts.resolve == "alignment":
         # Get pairs and prompt to run needle
         pairsfile = "nw.pairs"
         scoresfile = "nw.scores"
         if not os.path.isfile(pairsfile):
             get_pairs(cbedfile, pairsfile)
         else:
-            logging.warning(
+            logger.warning(
                 "`{0}` already exists. Checking for needle output".format(pairsfile)
             )
 
         # If needle scores do not exist, prompt user to run needle
         if not os.path.isfile(scoresfile):
-            logging.error(
+            logger.error(
                 "`{0}` does not exist. Please process {1} using `needle`".format(
                     scoresfile, pairsfile
                 )
             )
             sys.exit()
     else:
         scoresfile = "ovl.scores"
         # Calculate overlap length using intersectBed
         calculate_ovl(nbedfile, obedfile, opts, scoresfile)
 
-    logging.warning("`{0}' exists. Storing scores in memory".format(scoresfile))
+    logger.warning("`{0}' exists. Storing scores in memory".format(scoresfile))
     scores = read_scores(scoresfile, opts)
 
     # Iterate through consolidated bed and
     # filter piles based on score
     abedline = {}
 
     cbed = Bed(cbedfile)
@@ -751,15 +746,15 @@
     _pid, _score, resolve = (
         (0.0, 0.0, "alignment")
         if opts is None
         else (opts.pid, opts.score, opts.resolve)
     )
 
     fp = must_open(scoresfile)
-    logging.debug("Load scores file `{0}`".format(scoresfile))
+    logger.debug("Load scores file `{0}`".format(scoresfile))
     for row in fp:
         (new, old, identity, score) = row.strip().split("\t")
         if trimsuffix:
             old = re.sub(r"\.\d+$", "", old)
         if resolve == "alignment":
             match = re.search(r"\d+/\d+\s+\(\s*(\d+\.\d+)%\)", identity)
             pid = match.group(1)
@@ -945,42 +940,42 @@
     Bo1g00120, <gap>, Bo1g01120...
 
     Gaps bed file is optional.
     """
     import string
 
     p = OptionParser(rename.__doc__)
-    p.add_option(
+    p.add_argument(
         "-a",
         dest="gene_increment",
         default=10,
-        type="int",
+        type=int,
         help="Increment for continuous genes",
     )
-    p.add_option(
+    p.add_argument(
         "-b",
         dest="gap_increment",
         default=1000,
-        type="int",
+        type=int,
         help="Increment for gaps",
     )
-    p.add_option(
+    p.add_argument(
         "--pad0",
         default=6,
-        type="int",
+        type=int,
         help="Pad gene identifiers with 0",
     )
-    p.add_option(
+    p.add_argument(
         "--spad0",
         default=4,
-        type="int",
+        type=int,
         help="Pad gene identifiers on small scaffolds",
     )
-    p.add_option("--prefix", default="Bo", help="Genome prefix")
-    p.add_option(
+    p.add_argument("--prefix", default="Bo", help="Genome prefix")
+    p.add_argument(
         "--jgi",
         default=False,
         action="store_true",
         help="Create JGI style identifier PREFIX.NN[G|TE]NNNNN.1",
     )
     opts, args = p.parse_args(args)
 
@@ -1028,16 +1023,16 @@
                 idx += gene_increment
             accn = pp + "{0:0{1}d}".format(idx, pad0)
             oldaccn = r.accn
             print("\t".join((oldaccn, accn)), file=fw)
             r.accn = accn
 
     genes.print_to_file(newbedfile)
-    logging.debug("Converted IDs written to `{0}`.".format(idsfile))
-    logging.debug("Converted bed written to `{0}`.".format(newbedfile))
+    logger.debug("Converted IDs written to `{0}`.".format(idsfile))
+    logger.debug("Converted bed written to `{0}`.".format(newbedfile))
 
 
 def parse_prefix(identifier):
     """
     Parse identifier such as a|c|le|d|li|re|or|AT4G00480.1 and return
     tuple of prefix string (separated at '|') and suffix (AGI identifier)
     """
@@ -1073,16 +1068,16 @@
     """
     from jcvi.formats.gff import make_index
     from jcvi.formats.fasta import Fasta
     from jcvi.apps.emboss import needle
     from tempfile import mkstemp
 
     p = OptionParser(reindex.__doc__)
-    p.add_option(
-        "--scores", type="str", help="read from existing EMBOSS `needle` scores file"
+    p.add_argument(
+        "--scores", type=str, help="read from existing EMBOSS `needle` scores file"
     )
     p.set_outfile()
     opts, args = p.parse_args(args)
 
     if len(args) != 3:
         sys.exit(not p.print_help())
 
@@ -1236,29 +1231,29 @@
     Example output:
     Medtr1g007020.1		MTR_1g007020
     Medtr1g007030.1		MTR_1g007030
     Medtr1g007060.1		MTR_1g007060A
     Medtr1g007060.2		MTR_1g007060B
     """
     p = OptionParser(publocus.__doc__)
-    p.add_option("--locus_tag", default="MTR_", help="GenBank locus tag")
+    p.add_argument("--locus_tag", default="MTR_", help="GenBank locus tag")
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     locus_tag = opts.locus_tag
 
     index = AutoVivification()
     (idsfile,) = args
     fp = must_open(idsfile)
     for row in fp:
         locus, chrom, sep, rank, iso = atg_name(row, retval="locus,chr,sep,rank,iso")
         if None in (locus, chrom, sep, rank, iso):
-            logging.warning("{0} is not a valid gene model identifier".format(row))
+            logger.warning("{0} is not a valid gene model identifier".format(row))
             continue
         if locus not in index.keys():
             pub_locus = gene_name(chrom, rank, prefix=locus_tag, sep=sep)
             index[locus]["pub_locus"] = pub_locus
             index[locus]["isos"] = set()
 
         index[locus]["isos"].add(int(iso))
```

### Comparing `jcvi-1.4.6/jcvi/annotation/stats.py` & `jcvi-1.4.7/jcvi/annotation/stats.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,23 +3,22 @@
 
 """
 Collect gene statistics based on gff file:
 Exon length, Intron length, Gene length, Exon count
 """
 import os.path as op
 import sys
-import logging
 
-from jcvi.utils.cbook import SummaryStats, percentage, human_size
-from jcvi.utils.range import range_interleave
-from jcvi.utils.table import tabulate
-from jcvi.formats.fasta import Fasta
-from jcvi.formats.gff import make_index
-from jcvi.formats.base import DictFile, must_open
-from jcvi.apps.base import OptionParser, ActionDispatcher, mkdir, need_update
+from ..apps.base import ActionDispatcher, OptionParser, logger, mkdir, need_update
+from ..formats.base import DictFile, must_open
+from ..formats.fasta import Fasta
+from ..formats.gff import make_index
+from ..utils.cbook import SummaryStats, human_size, percentage
+from ..utils.range import range_interleave
+from ..utils.table import tabulate
 
 
 metrics = ("Exon_Length", "Intron_Length", "Gene_Length", "Exon_Count")
 
 
 class GeneStats(object):
     def __init__(self, feat, conf_class, transcript_sizes, exons):
@@ -109,15 +108,15 @@
         for chrom, start, stop in introns:
             fseq = s.sequence({"chr": chrom, "start": start, "stop": stop})
             intronseqs.append(fseq)
 
     r = {}  # Report
     for t, tseqs in zip(("Gene", "Exon", "Intron"), (geneseqs, exonseqs, intronseqs)):
         tsizes = [len(x) for x in tseqs]
-        tsummary = SummaryStats(tsizes, dtype="int")
+        tsummary = SummaryStats(tsizes, dtype=int)
         r[t, "Number"] = tsummary.size
         r[t, "Average size (bp)"] = tsummary.mean
         r[t, "Median size (bp)"] = tsummary.median
         r[t, "Total length (Mb)"] = human_size(tsummary.sum, precision=0, target="Mb")
         r[t, "% of genome"] = percentage(
             tsummary.sum, s.totalsize, precision=0, mode=-1
         )
@@ -143,15 +142,17 @@
     - Mean transcript size (UTR, CDS)
     - Mean exon size
 
     Stats modeled after barley genome paper Table 1.
     A physical, genetic and functional sequence assembly of the barley genome
     """
     p = OptionParser(genestats.__doc__)
-    p.add_option("--groupby", default="conf_class", help="Print separate stats groupby")
+    p.add_argument(
+        "--groupby", default="conf_class", help="Print separate stats groupby"
+    )
     p.set_outfile()
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (gff_file,) = args
@@ -170,15 +171,15 @@
                 if c.featuretype == "exon"
             )
             print("\t".join((fid, str(tsize), conf_class)), file=fw)
         fw.close()
 
     tsizes = DictFile(tf, cast=int)
     conf_classes = DictFile(tf, valuepos=2)
-    logging.debug("A total of {0} transcripts populated.".format(len(tsizes)))
+    logger.debug("A total of {0} transcripts populated.".format(len(tsizes)))
 
     genes = []
     for feat in g.features_of_type("gene"):
         fid = feat.id
         transcripts = [c.id for c in g.children(fid, 1) if c.featuretype == "mRNA"]
         if len(transcripts) == 0:
             continue
@@ -256,15 +257,15 @@
     opts, args = p.parse_args(args)
 
     if len(args) < 1:
         sys.exit(not p.print_help())
 
     gff_files = args
     for metric in metrics:
-        logging.debug("Parsing files in `{0}`..".format(metric))
+        logger.debug("Parsing files in `{0}`..".format(metric))
 
         table = {}
         for x in gff_files:
             pf = op.basename(x).split(".")[0]
             numberfile = op.join(metric, pf + ".txt")
             ar = [int(x.strip()) for x in open(numberfile)]
             sum = SummaryStats(ar).todict().items()
@@ -282,33 +283,33 @@
     Plot gene statistics based on output of stats. For each gff file, look to
     see if the metrics folder (i.e. Exon_Length) contains the data and plot
     them.
     """
     from jcvi.graphics.histogram import histogram_multiple
 
     p = OptionParser(histogram.__doc__)
-    p.add_option(
+    p.add_argument(
         "--bins",
         dest="bins",
         default=40,
-        type="int",
+        type=int,
         help="number of bins to plot in the histogram",
     )
     opts, args = p.parse_args(args)
 
     if len(args) < 1:
         sys.exit(not p.print_help())
 
     gff_files = args
     # metrics = ("Exon_Length", "Intron_Length", "Gene_Length", "Exon_Count")
     colors = ("red", "green", "blue", "black")
     vmaxes = (1000, 1000, 4000, 20)
     xlabels = ("bp", "bp", "bp", "number")
     for metric, color, vmax, xlabel in zip(metrics, colors, vmaxes, xlabels):
-        logging.debug("Parsing files in `{0}`..".format(metric))
+        logger.debug("Parsing files in `{0}`..".format(metric))
         numberfiles = [
             op.join(metric, op.basename(x).split(".")[0] + ".txt") for x in gff_files
         ]
 
         histogram_multiple(
             numberfiles,
             0,
@@ -334,16 +335,16 @@
     corresponding to the four metrics:
 
     Exon length, Intron length, Gene length, Exon count
 
     With data written to disk then you can run %prog histogram
     """
     p = OptionParser(stats.__doc__)
-    p.add_option("--gene", default="mRNA", help="The gene type")
-    p.add_option("--exon", default="CDS", help="The exon type")
+    p.add_argument("--gene", default="mRNA", help="The gene type")
+    p.add_argument("--exon", default="CDS", help="The exon type")
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (gff_file,) = args
     g = make_index(gff_file)
```

### Comparing `jcvi-1.4.6/jcvi/annotation/train.py` & `jcvi-1.4.7/jcvi/annotation/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 
 """
 Train ab initio gene predictors.
 """
 import os
 import os.path as op
 import sys
-import logging
 
-from jcvi.apps.base import OptionParser, ActionDispatcher, mkdir, sh, need_update
+from ..apps.base import ActionDispatcher, OptionParser, logger, mkdir, need_update, sh
 
 
 def main():
 
     actions = (
         ("pasa", "extract pasa training models"),
         ("snap", "train snap model"),
@@ -70,30 +69,30 @@
         if asmbl_id not in complete:
             continue
         print(g, file=fw)
         if g.type == "gene":
             seen.add(id)
 
     fw.close()
-    logging.debug(
+    logger.debug(
         "A total of {0} complete models extracted to `{1}`.".format(
             len(seen), completegff
         )
     )
 
 
 def genemark(args):
     """
     %prog genemark species fastafile
 
     Train GENEMARK model given fastafile. GENEMARK self-trains so no trainig
     model gff file is needed.
     """
     p = OptionParser(genemark.__doc__)
-    p.add_option("--junctions", help="Path to `junctions.bed` from Tophat2")
+    p.add_argument("--junctions", help="Path to `junctions.bed` from Tophat2")
     p.set_home("gmes")
     p.set_cpus(cpus=32)
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
@@ -112,15 +111,15 @@
             jcmd += " --bed {0} --gff {1} --label Tophat2".format(junctions, intronsgff)
             sh(jcmd)
         cmd += " --ET {0} --et_score 10".format(intronsgff)
     else:
         cmd += " --ES"
     sh(cmd)
 
-    logging.debug("GENEMARK matrix written to `output/gmhmm.mod")
+    logger.debug("GENEMARK matrix written to `output/gmhmm.mod")
 
 
 def snap(args):
     """
     %prog snap species gffile fastafile
 
     Train SNAP model given gffile and fastafile. Whole procedure taken from:
@@ -140,39 +139,39 @@
     snapdir = "snap"
     mkdir(snapdir)
 
     cwd = os.getcwd()
     os.chdir(snapdir)
 
     newgffile = "training.gff3"
-    logging.debug("Construct GFF file combined with sequence ...")
+    logger.debug("Construct GFF file combined with sequence ...")
     sh("cat {0} > {1}".format(gffile, newgffile))
     sh('echo "##FASTA" >> {0}'.format(newgffile))
     sh("cat {0} >> {1}".format(fastafile, newgffile))
 
-    logging.debug("Make models ...")
+    logger.debug("Make models ...")
     sh("{0}/src/bin/maker2zff training.gff3".format(mhome))
     sh("{0}/exe/snap/fathom -categorize 1000 genome.ann genome.dna".format(mhome))
     sh("{0}/exe/snap/fathom -export 1000 -plus uni.ann uni.dna".format(mhome))
     sh("{0}/exe/snap/forge export.ann export.dna".format(mhome))
     sh("{0}/exe/snap/hmm-assembler.pl {1} . > {1}.hmm".format(mhome, species))
 
     os.chdir(cwd)
-    logging.debug("SNAP matrix written to `{0}/{1}.hmm`".format(snapdir, species))
+    logger.debug("SNAP matrix written to `{0}/{1}.hmm`".format(snapdir, species))
 
 
 def augustus(args):
     """
     %prog augustus species gffile fastafile
 
     Train AUGUSTUS model given gffile and fastafile. Whole procedure taken from:
     <http://www.molecularevolution.org/molevolfiles/exercises/augustus/training.html>
     """
     p = OptionParser(augustus.__doc__)
-    p.add_option(
+    p.add_argument(
         "--autotrain",
         default=False,
         action="store_true",
         help="Run autoAugTrain.pl to iteratively train AUGUSTUS",
     )
     p.set_home("augustus")
     opts, args = p.parse_args(args)
@@ -188,15 +187,15 @@
 
     cwd = os.getcwd()
     mkdir(augdir)
     os.chdir(augdir)
     target = "{0}/config/species/{1}".format(mhome, species)
 
     if op.exists(target):
-        logging.debug("Removing existing target `{0}`".format(target))
+        logger.debug("Removing existing target `{0}`".format(target))
         sh("rm -rf {0}".format(target))
 
     config_path = "{0}/config".format(mhome)
     sh(
         "{0}/scripts/new_species.pl --species={1} --AUGUSTUS_CONFIG_PATH={2}".format(
             mhome, species, config_path
         )
```

### Comparing `jcvi-1.4.6/jcvi/annotation/trinity.py` & `jcvi-1.4.7/jcvi/annotation/trinity.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 GG: http://trinityrnaseq.sourceforge.net/genome_guided_trinity.html
 """
 
 import os.path as op
 import os
 import sys
 
-from jcvi.formats.base import FileMerger, write_file
-from jcvi.apps.base import OptionParser, ActionDispatcher, mkdir, iglob
+from ..apps.base import ActionDispatcher, OptionParser, iglob, mkdir
+from ..formats.base import FileMerger, write_file
 
 
 def main():
 
     actions = (
         ("prepare", "prepare shell script to run trinity-dn/gg on a folder of reads"),
     )
@@ -39,21 +39,21 @@
     If coord-sorted BAM is provided, prepare script for GG-Trinity, using BAM
     as starting point.
 
     Newer versions of trinity can take multiple fastq files as input.
     If "--merge" is specified, the fastq files are merged together before assembling
     """
     p = OptionParser(prepare.__doc__)
-    p.add_option(
+    p.add_argument(
         "--paired",
         default=False,
         action="store_true",
         help="Paired-end mode",
     )
-    p.add_option(
+    p.add_argument(
         "--merge",
         default=False,
         action="store_true",
         help="Merge individual input fastq's into left/right/single file(s)",
     )
     p.set_trinity_opts()
     p.set_fastq_names()
```

### Comparing `jcvi-1.4.6/jcvi/apps/align.py` & `jcvi-1.4.7/jcvi/apps/align.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 """
 Perform DNA-DNA alignment using BLAST, NUCMER and BLAT. Keep the interface the
 same and does parallelization both in core and on grid.
 """
 import os.path as op
 import sys
 import shutil
-import logging
 
 from subprocess import CalledProcessError, STDOUT
 
-from jcvi.utils.cbook import depends
-from jcvi.apps.base import (
+from ..utils.cbook import depends
+
+from .base import (
     ActionDispatcher,
     OptionParser,
     cleanup,
     get_abs_path,
+    logger,
     mkdir,
     sh,
     which,
 )
 
 
 @depends
@@ -120,15 +121,15 @@
         )
         shutil.move(filtered_blastfile, blastfile)
 
 
 def run_blast_filter(infile=None, outfile=None, pctid=95, hitlen=50):
     from jcvi.formats.blast import filter
 
-    logging.debug("Filter BLAST result (pctid={0}, hitlen={1})".format(pctid, hitlen))
+    logger.debug("Filter BLAST result (pctid={0}, hitlen={1})".format(pctid, hitlen))
     pctidopt = "--pctid={0}".format(pctid)
     hitlenopt = "--hitlen={0}".format(hitlen)
     filter([infile, pctidopt, hitlenopt])
 
 
 def main():
     actions = (
@@ -153,17 +154,17 @@
     is the same, we are in "self-scan" mode (e.g. useful for finding internal
     duplications resulted from mis-assemblies).
     """
     from jcvi.apps.grid import MakeManager
     from jcvi.formats.fasta import Fasta
 
     p = OptionParser(minimap.__doc__)
-    p.add_option(
+    p.add_argument(
         "--chunks",
-        type="int",
+        type=int,
         default=2000000,
         help="Split ref.fasta into chunks of size in self-scan mode",
     )
     p.set_outdir(outdir="outdir")
     p.set_cpus()
     opts, args = p.parse_args(args)
 
@@ -212,16 +213,16 @@
     """
     from itertools import product
 
     from jcvi.apps.grid import MakeManager
     from jcvi.formats.base import split
 
     p = OptionParser(nucmer.__doc__)
-    p.add_option(
-        "--chunks", type="int", help="Split both query and subject into chunks"
+    p.add_argument(
+        "--chunks", type=int, help="Split both query and subject into chunks"
     )
     p.set_params(prog="nucmer", params="-l 100 -c 500")
     p.set_cpus()
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
@@ -348,17 +349,17 @@
     %prog blast ref.fasta query.fasta
 
     Calls blast and then filter the BLAST hits. Default is megablast.
     """
     task_choices = ("blastn", "blastn-short", "dc-megablast", "megablast", "vecscreen")
     p = OptionParser(blast.__doc__)
     p.set_align(pctid=0, evalue=0.01)
-    p.add_option("--wordsize", type="int", help="Word size")
-    p.add_option("--best", default=1, type="int", help="Only look for best N hits")
-    p.add_option(
+    p.add_argument("--wordsize", type=int, help="Word size")
+    p.add_argument("--best", default=1, type=int, help="Only look for best N hits")
+    p.add_argument(
         "--task", default="megablast", choices=task_choices, help="Task of the blastn"
     )
     p.set_cpus()
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
@@ -487,37 +488,37 @@
 
     Run LAST by calling LASTDB and LASTAL. LAST program available:
     <http://last.cbrc.jp>
 
     Works with LAST-719.
     """
     p = OptionParser(last.__doc__)
-    p.add_option(
+    p.add_argument(
         "--dbtype",
         default="nucl",
         choices=("nucl", "prot"),
         help="Molecule type of subject database",
     )
-    p.add_option("--path", help="Specify LAST path")
-    p.add_option(
+    p.add_argument("--path", help="Specify LAST path")
+    p.add_argument(
         "--mask", default=False, action="store_true", help="Invoke -c in lastdb"
     )
-    p.add_option(
+    p.add_argument(
         "--format",
         default="BlastTab",
         choices=("TAB", "MAF", "BlastTab", "BlastTab+"),
         help="Output format",
     )
-    p.add_option(
+    p.add_argument(
         "--minlen",
         default=0,
-        type="int",
+        type=int,
         help="Filter alignments by how many bases match",
     )
-    p.add_option("--minid", default=0, type="int", help="Minimum sequence identity")
+    p.add_argument("--minid", default=0, type=int, help="Minimum sequence identity")
     p.set_cpus()
     p.set_outdir()
     p.set_params()
 
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
@@ -529,15 +530,15 @@
     if not dbtype:
         dbtype = opts.dbtype
     getpath = lambda x: op.join(path, x) if path else x
     lastdb_bin = getpath("lastdb")
     lastal_bin = getpath("lastal")
     for bin in (lastdb_bin, lastal_bin):
         if not which(bin):
-            logging.fatal("`%s` not found on PATH. Have you installed LAST?", bin)
+            logger.fatal("`%s` not found on PATH. Have you installed LAST?", bin)
             sys.exit(1)
 
     subjectdb = subject.rsplit(".", 1)[0]
     run_lastdb(
         infile=subject,
         outfile=subjectdb + ".prj",
         mask=opts.mask,
@@ -570,47 +571,47 @@
             outfile=lastfile,
             check=True,
             redirect_error=STDOUT,
         )
     except CalledProcessError as e:  # multi-threading disabled
         message = "lastal failed with message:"
         message += "\n{0}".format(e.output.decode())
-        logging.error(message)
+        logger.error(message)
         try:
-            logging.debug("Failed to run `lastal` with multi-threading. Trying again.")
+            logger.debug("Failed to run `lastal` with multi-threading. Trying again.")
             sh(
                 cmd + f" -P 1 {subjectdb} {query}",
                 outfile=lastfile,
                 check=True,
                 redirect_error=STDOUT,
             )
         except CalledProcessError as e:
             message = "lastal failed with message:"
             message += "\n{0}".format(e.output.decode())
-            logging.error(message)
-            logging.fatal("Failed to run `lastal`. Aborted.")
+            logger.error(message)
+            logger.fatal("Failed to run `lastal`. Aborted.")
             cleanup(lastfile)
             sys.exit(1)
     return lastfile
 
 
 def blast_main(args, dbtype=None):
     """
     %prog database.fasta query.fasta
 
     Run blastp/blastn by calling BLAST+ blastp/blastn depends on dbtype.
     """
     p = OptionParser(blast_main.__doc__)
-    p.add_option(
+    p.add_argument(
         "--dbtype",
         default="nucl",
         choices=("nucl", "prot"),
         help="Molecule type of subject database",
     )
-    p.add_option("--path", help="Specify BLAST path for blastn or blastp")
+    p.add_argument("--path", help="Specify BLAST path for blastn or blastp")
 
     p.set_cpus()
     p.set_outdir()
     p.set_params()
 
     opts, args = p.parse_args(args)
 
@@ -625,15 +626,15 @@
 
     getpath = lambda x: op.join(path, x) if path else x
     cmd = "blastn" if dbtype == "nucl" else "blastp"
     lastdb_bin = getpath("makeblastdb")
     lastal_bin = getpath(cmd)
     for bin in (lastdb_bin, lastal_bin):
         if not which(bin):
-            logging.fatal("`%s` not found on PATH. Have you installed BLAST?", bin)
+            logger.fatal("`%s` not found on PATH. Have you installed BLAST?", bin)
             sys.exit(1)
 
     db_suffix = ".nin" if dbtype == "nucl" else ".pin"
 
     run_formatdb(infile=subject, outfile=subject + db_suffix, dbtype=dbtype)
 
     blastfile = get_outfile(subject, query, suffix="last", outdir=opts.outdir)
@@ -645,30 +646,30 @@
             + " -outfmt 6 -max_target_seqs 1000 -evalue 1e-5",
             check=False,
             redirect_error=STDOUT,
         )
     except CalledProcessError as e:  # multi-threading disabled
         message = f"{cmd} failed with message:"
         message += "\n{0}".format(e.output.decode())
-        logging.error(message)
-        logging.fatal("Failed to run `blast`. Aborted.")
+        logger.error(message)
+        logger.fatal("Failed to run `blast`. Aborted.")
         cleanup(blastfile)
         sys.exit(1)
     return blastfile
 
 
 def diamond_blastp_main(args, dbtype="prot"):
     """
     %prog database.fasta query.fasta
 
     Run diamond blastp for protein alignment.
     """
     p = OptionParser(diamond_blastp_main.__doc__)
 
-    p.add_option("--path", help="Specify diamond path for diamond blastp")
+    p.add_argument("--path", help="Specify diamond path for diamond blastp")
 
     p.set_cpus()
     p.set_outdir()
     p.set_params()
 
     opts, args = p.parse_args(args)
 
@@ -682,15 +683,15 @@
         dbtype = opts.dbtype
 
     getpath = lambda x: op.join(path, x) if path else x
     cmd = "diamond blastp"
     diamond_bin = getpath("diamond")
     for bin in (diamond_bin,):
         if not which(bin):
-            logging.fatal("`%s` not found on PATH. Have you installed Diamond?", bin)
+            logger.fatal("`%s` not found on PATH. Have you installed Diamond?", bin)
             sys.exit(1)
 
     run_diamond_makedb(
         infile=subject,
         outfile=subject + ".dmnd",
     )
 
@@ -703,16 +704,16 @@
             + " --ultra-sensitive --max-target-seqs 1000 --evalue 1e-5 --outfmt 6",
             check=False,
             redirect_error=STDOUT,
         )
     except CalledProcessError as e:  # multi-threading disabled
         message = f"{cmd} failed with message:"
         message += "\n{0}".format(e.output.decode())
-        logging.error(message)
-        logging.fatal("Failed to run `diamond blastp`. Aborted.")
+        logger.error(message)
+        logger.fatal("Failed to run `diamond blastp`. Aborted.")
         cleanup(blastfile)
         sys.exit(1)
     return blastfile
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `jcvi-1.4.6/jcvi/apps/base.py` & `jcvi-1.4.7/jcvi/apps/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     ConfigParser,
     RawConfigParser,
     NoOptionError,
     NoSectionError,
     ParsingError,
 )
 
+from argparse import ArgumentParser, SUPPRESS
 from http.client import HTTPSConnection
-from optparse import OptionGroup, OptionParser as OptionP, SUPPRESS_HELP
 from socket import gethostname
 from subprocess import CalledProcessError, PIPE, call, check_output
 from time import ctime
 from typing import Any, Collection, List, Optional, Tuple, Union
 from urllib.parse import urlencode
 from natsort import natsorted
 from rich.console import Console
@@ -141,36 +141,44 @@
                 file=sys.stderr,
             )
             self.print_help()
 
         globals[action](sys.argv[2:])
 
 
-class OptionParser(OptionP):
-    def __init__(self, doc):
-        OptionP.__init__(self, doc, epilog=JCVIHELP)
+class OptionParser(ArgumentParser):
+    """
+    This class is a wrapper around argparse.ArgumentParser, with some added
+    features.
+    """
+
+    def __init__(self, doc: Optional[str]):
+        super(OptionParser, self).__init__(doc, epilog=JCVIHELP)
 
     def parse_args(self, args=None):
+        """
+        Parse the command line arguments.
+        """
         dests = set()
         ol = []
-        for g in [self] + self.option_groups:
-            ol += g.option_list
+        for g in [self] + self._action_groups:
+            ol += g._actions
         for o in ol:
             if o.dest in dests:
                 continue
             self.add_help_from_choices(o)
             dests.add(o.dest)
 
-        return OptionP.parse_args(self, args)
+        return self.parse_known_args(args)
 
     def add_help_from_choices(self, o):
-        if o.help == SUPPRESS_HELP:
+        if o.help == SUPPRESS:
             return
 
-        default_tag = "%default"
+        default_tag = "%(default)s"
         assert o.help, "Option {0} do not have help string".format(o)
         help_pf = o.help[:1].upper() + o.help[1:]
         if "[" in help_pf:
             help_pf = help_pf.rsplit("[", 1)[0]
         help_pf = help_pf.strip()
 
         if o.type == "choice":
@@ -181,349 +189,343 @@
                 ctext = ctext[:100] + " ... "
             choice_text = "must be one of {0}".format(ctext)
             o.help = "{0}, {1} [default: {2}]".format(help_pf, choice_text, default_tag)
         else:
             o.help = help_pf
             if o.default is None:
                 default_tag = "disabled"
-            if (
-                o.get_opt_string() not in ("--help", "--version")
-                and o.action != "store_false"
-            ):
+            if not set(o.option_strings) & set(("--help", "--version")):
                 o.help += " [default: {0}]".format(default_tag)
 
     def set_grid(self):
         """
         Add --grid options for command line programs
         """
-        self.add_option(
+        self.add_argument(
             "--grid",
             dest="grid",
             default=False,
             action="store_true",
             help="Run on the grid",
         )
 
-    def set_grid_opts(self, array=False):
-        group = OptionGroup(self, "Grid parameters")
-        group.add_option(
+    def set_grid_opts(self, array: bool = False):
+        group = self.add_argument_group("Grid parameters")
+        group.add_argument(
             "-l",
             dest="queue",
             help="Name of the queue",
         )
-        group.add_option(
+        group.add_argument(
             "-t",
             dest="threaded",
             default=None,
-            type="int",
+            type=int,
             help="Append '-pe threaded N'",
         )
         if array:
-            group.add_option(
+            group.add_argument(
                 "-c",
                 dest="concurrency",
-                type="int",
+                type=int,
                 help="Append task concurrency limit '-tc N'",
             )
-        group.add_option(
+        group.add_argument(
             "-d",
             dest="outdir",
             default=".",
             help="Specify directory to store grid output/error files",
         )
-        group.add_option(
+        group.add_argument(
             "-N", dest="name", default=None, help="Specify descriptive name for the job"
         )
-        group.add_option(
+        group.add_argument(
             "-H", dest="hold_jid", default=None, help="Define the job dependency list"
         )
-        self.add_option_group(group)
 
     def set_table(self, sep=",", align=False):
-        group = OptionGroup(self, "Table formatting")
-        group.add_option("--sep", default=sep, help="Separator")
+        group = self.add_argument_group("Table formatting")
+        group.add_argument("--sep", default=sep, help="Separator")
         if align:
-            group.add_option(
+            group.add_argument(
                 "--noalign",
                 dest="align",
                 default=True,
                 action="store_false",
                 help="Cell alignment",
             )
         else:
-            group.add_option(
+            group.add_argument(
                 "--align", default=False, action="store_true", help="Cell alignment"
             )
-        self.add_option_group(group)
 
     def set_downloader(self, downloader=None):
         """
         Add --downloader options for given command line program.
         """
         from jcvi.utils.ez_setup import ALL_DOWNLOADERS
 
         downloader_choices = [x[0] for x in ALL_DOWNLOADERS]
-        self.add_option(
+        self.add_argument(
             "--downloader",
             default=downloader,
             choices=downloader_choices,
             help="Use the specified downloader to retrieve resources",
         )
 
     def set_params(self, prog=None, params=""):
         """
         Add --params options for given command line programs
         """
         dest_prog = "to {0}".format(prog) if prog else ""
-        self.add_option(
+        self.add_argument(
             "--params",
             dest="extra",
             default=params,
             help="Extra parameters to pass {0}".format(dest_prog)
             + " (these WILL NOT be validated)",
         )
 
     def set_outfile(self, outfile="stdout"):
         """
         Add --outfile options to print out to filename.
         """
-        self.add_option("-o", "--outfile", default=outfile, help="Outfile name")
+        self.add_argument("-o", "--outfile", default=outfile, help="Outfile name")
 
     def set_outdir(self, outdir="."):
-        self.add_option("--outdir", default=outdir, help="Specify output directory")
+        self.add_argument("--outdir", default=outdir, help="Specify output directory")
 
     def set_email(self):
         """
         Add --email option to specify an email address
         """
-        self.add_option(
+        self.add_argument(
             "--email",
             default=get_email_address(),
             help="Specify an email address",
         )
 
     def set_tmpdir(self, tmpdir=None):
         """
         Add --temporary_directory option to specify unix `sort` tmpdir
         """
-        self.add_option(
+        self.add_argument(
             "-T", "--tmpdir", default=tmpdir, help="Use temp directory instead of $TMP"
         )
 
     def set_cpus(self, cpus=0):
         """
         Add --cpus options to specify how many threads to use.
         """
         from multiprocessing import cpu_count
 
         max_cpus = cpu_count()
         if not 0 < cpus < max_cpus:
             cpus = max_cpus
-        self.add_option(
+        self.add_argument(
             "--cpus",
             default=cpus,
-            type="int",
+            type=int,
             help="Number of CPUs to use, 0=unlimited",
         )
 
     def set_db_opts(self, dbname="mta4", credentials=True):
         """
         Add db connection specific attributes
         """
         from jcvi.utils.db import valid_dbconn, get_profile
 
-        self.add_option(
+        self.add_argument(
             "--db",
             default=dbname,
             dest="dbname",
             help="Specify name of database to query",
         )
-        self.add_option(
+        self.add_argument(
             "--connector",
             default="Sybase",
             dest="dbconn",
             choices=valid_dbconn.keys(),
             help="Specify database connector",
         )
         hostname, username, password = get_profile()
         if credentials:
-            self.add_option("--hostname", default=hostname, help="Specify hostname")
-            self.add_option(
+            self.add_argument("--hostname", default=hostname, help="Specify hostname")
+            self.add_argument(
                 "--username", default=username, help="Username to connect to database"
             )
-            self.add_option(
+            self.add_argument(
                 "--password", default=password, help="Password to connect to database"
             )
-        self.add_option("--port", type="int", help="Specify port number")
+        self.add_argument("--port", type=int, help="Specify port number")
 
     def set_aws_opts(self, store="hli-mv-data-science/htang"):
         from jcvi.utils.aws import s3ify
 
         store = s3ify(store)
-        group = OptionGroup(self, "AWS and Docker options")
-        self.add_option_group(group)
+        group = self.add_argument_group("AWS and Docker options")
         # https://github.com/hlids/infrastructure/wiki/Docker-calling-convention
-        group.add_option("--sample_id", help="Sample ID")
-        group.add_option("--workflow_execution_id", help="Workflow execution ID")
-        group.add_option("--input_bam_path", help="Input BAM location (s3 ok)")
-        group.add_option("--output_path", default=store, help="Output s3 path")
-        group.add_option("--workdir", default=os.getcwd(), help="Specify work dir")
-        group.add_option(
+        group.add_argument("--sample_id", help="Sample ID")
+        group.add_argument("--workflow_execution_id", help="Workflow execution ID")
+        group.add_argument("--input_bam_path", help="Input BAM location (s3 ok)")
+        group.add_argument("--output_path", default=store, help="Output s3 path")
+        group.add_argument("--workdir", default=os.getcwd(), help="Specify work dir")
+        group.add_argument(
             "--nocleanup",
             default=False,
             action="store_true",
             help="Don't clean up after done",
         )
 
     def set_stripnames(self, default=True):
         if default:
-            self.add_option(
+            self.add_argument(
                 "--no_strip_names",
                 dest="strip_names",
                 action="store_false",
                 default=True,
                 help="do not strip alternative splicing "
                 "(e.g. At5g06540.1 -> At5g06540)",
             )
         else:
-            self.add_option(
+            self.add_argument(
                 "--strip_names",
                 action="store_true",
                 default=False,
                 help="strip alternative splicing (e.g. At5g06540.1 -> At5g06540)",
             )
 
     def set_fixchrnames(self, orgn="medicago"):
-        self.add_option(
+        self.add_argument(
             "--fixchrname",
             default=orgn,
             dest="fix_chr_name",
             help="Fix quirky chromosome names",
         )
 
     def set_SO_opts(self):
         verifySO_choices = ("verify", "resolve:prefix", "resolve:suffix")
-        self.add_option(
+        self.add_argument(
             "--verifySO",
             choices=verifySO_choices,
             help="Verify validity of GFF3 feature type against the SO; "
             + "`resolve` will try to converge towards a valid SO "
             + "term by removing elements from the feature type "
             + "string by splitting at underscores. Example: "
             + "`mRNA_TE_gene` resolves to `mRNA` using 'resolve:prefix'",
         )
 
     def set_beds(self):
-        self.add_option("--qbed", help="Path to qbed")
-        self.add_option("--sbed", help="Path to sbed")
+        self.add_argument("--qbed", help="Path to qbed")
+        self.add_argument("--sbed", help="Path to sbed")
 
     def set_histogram(self, vmin=0, vmax=None, bins=20, xlabel="value", title=None):
-        self.add_option(
-            "--vmin", default=vmin, type="int", help="Minimum value, inclusive"
+        self.add_argument(
+            "--vmin", default=vmin, type=int, help="Minimum value, inclusive"
         )
-        self.add_option(
-            "--vmax", default=vmax, type="int", help="Maximum value, inclusive"
+        self.add_argument(
+            "--vmax", default=vmax, type=int, help="Maximum value, inclusive"
         )
-        self.add_option(
+        self.add_argument(
             "--bins",
             default=bins,
-            type="int",
+            type=int,
             help="Number of bins to plot in the histogram",
         )
-        self.add_option("--xlabel", default=xlabel, help="Label on the X-axis")
-        self.add_option("--title", default=title, help="Title of the plot")
+        self.add_argument("--xlabel", default=xlabel, help="Label on the X-axis")
+        self.add_argument("--title", default=title, help="Title of the plot")
 
     def set_sam_options(self, extra=True, bowtie=False):
-        self.add_option(
+        self.add_argument(
             "--sam",
             dest="bam",
             default=True,
             action="store_false",
             help="Write to SAM file instead of BAM",
         )
-        self.add_option(
+        self.add_argument(
             "--uniq",
             default=False,
             action="store_true",
             help="Keep only uniquely mapped",
         )
         if bowtie:
-            self.add_option(
+            self.add_argument(
                 "--mapped", default=False, action="store_true", help="Keep mapped reads"
             )
-        self.add_option(
+        self.add_argument(
             "--unmapped", default=False, action="store_true", help="Keep unmapped reads"
         )
         if extra:
             self.set_cpus()
             self.set_params()
 
     def set_mingap(self, default=100):
-        self.add_option(
-            "--mingap", default=default, type="int", help="Minimum size of gaps"
+        self.add_argument(
+            "--mingap", default=default, type=int, help="Minimum size of gaps"
         )
 
     def set_align(
         self,
         pctid=None,
         hitlen=None,
         pctcov=None,
         evalue=None,
         compreh_pctid=None,
         compreh_pctcov=None,
         intron=None,
         bpsplice=None,
     ):
         if pctid is not None:
-            self.add_option(
-                "--pctid", default=pctid, type="float", help="Sequence percent identity"
+            self.add_argument(
+                "--pctid", default=pctid, type=float, help="Sequence percent identity"
             )
         if hitlen is not None:
-            self.add_option(
-                "--hitlen", default=hitlen, type="int", help="Minimum overlap length"
+            self.add_argument(
+                "--hitlen", default=hitlen, type=int, help="Minimum overlap length"
             )
         if pctcov is not None:
-            self.add_option(
+            self.add_argument(
                 "--pctcov",
                 default=pctcov,
-                type="int",
+                type=int,
                 help="Percentage coverage cutoff",
             )
         if evalue is not None:
-            self.add_option(
-                "--evalue", default=evalue, type="float", help="E-value cutoff"
+            self.add_argument(
+                "--evalue", default=evalue, type=float, help="E-value cutoff"
             )
         if compreh_pctid is not None:
-            self.add_option(
+            self.add_argument(
                 "--compreh_pctid",
                 default=compreh_pctid,
-                type="int",
+                type=int,
                 help="Sequence percent identity cutoff used to "
                 + "build PASA comprehensive transcriptome",
             )
         if compreh_pctcov is not None:
-            self.add_option(
+            self.add_argument(
                 "--compreh_pctcov",
                 default=compreh_pctcov,
-                type="int",
+                type=int,
                 help="Percent coverage cutoff used to "
                 + "build PASA comprehensive transcriptome",
             )
         if intron is not None:
-            self.add_option(
+            self.add_argument(
                 "--intron",
                 default=intron,
-                type="int",
+                type=int,
                 help="Maximum intron length used for mapping",
             )
         if bpsplice is not None:
-            self.add_option(
+            self.add_argument(
                 "--bpsplice",
                 default=bpsplice,
-                type="int",
+                type=int,
                 help="Number of bp of perfect splice boundary",
             )
 
     def set_image_options(
         self,
         args=None,
         figsize="6x6",
@@ -560,54 +562,55 @@
             "RdBu",
             "RdGy",
             "RdYlBu",
             "RdYlGn",
             "Spectral",
         )
 
-        group = OptionGroup(self, "Image options")
-        self.add_option_group(group)
-
-        group.add_option(
+        group = self.add_argument_group("Image options")
+        group.add_argument(
             "--figsize", default=figsize, help="Figure size `width`x`height` in inches"
         )
-        group.add_option(
+        group.add_argument(
             "--dpi",
             default=dpi,
-            type="int",
+            type=int,
             help="Physical dot density (dots per inch)",
         )
-        group.add_option(
+        group.add_argument(
             "--format",
             default=format,
             choices=GRAPHIC_FORMATS,
             help="Generate image of format",
         )
-        group.add_option(
+        group.add_argument(
             "--font", default=font, choices=allowed_fonts, help="Font name"
         )
-        group.add_option(
+        group.add_argument(
             "--style", default=style, choices=allowed_styles, help="Axes background"
         )
-        group.add_option(
+        group.add_argument(
             "--diverge",
             default="PiYG",
             choices=allowed_diverge,
             help="Contrasting color scheme",
         )
-        group.add_option("--cmap", default=cmap, help="Use this color map")
-        group.add_option(
+        group.add_argument("--cmap", default=cmap, help="Use this color map")
+        group.add_argument(
             "--notex", default=False, action="store_true", help="Do not use tex"
         )
         # https://github.com/tanghaibao/jcvi/issues/515#issuecomment-1327305211
-        if not group.has_option("--seed"):
-            group.add_option(
+        if (
+            "--seed" not in self._option_string_actions
+            and "--seed" not in group._option_string_actions
+        ):
+            group.add_argument(
                 "--seed",
                 default=seed,
-                type="int",
+                type=int,
                 help="Random seed when assigning colors (supported only for some plots)",
             )
 
         if args is None:
             args = sys.argv[1:]
 
         opts, args = self.parse_args(args)
@@ -625,118 +628,116 @@
             if not bool(which("lp")):
                 logger.info("`lp` not found. latex use is disabled.")
 
         setup_theme(style=opts.style, font=opts.font, usetex=iopts.usetex)
 
         return opts, args, iopts
 
-    def set_dotplot_opts(self, theme: int = 2) -> OptionGroup:
+    def set_dotplot_opts(self, theme: int = 2):
         """
         Used in compara.catalog and graphics.dotplot
         """
         from jcvi.graphics.base import set1
 
-        group = OptionGroup(self, "Dot plot parameters")
-        group.add_option(
+        group = self.add_argument_group("Dot plot parameters")
+        group.add_argument(
             "--skipempty",
             default=False,
             action="store_true",
             help="Skip seqids that do not have matches",
         )
-        group.add_option(
+        group.add_argument(
             "--nochpf",
             default=False,
             action="store_true",
             help="Do not change the contig name",
         )
-        group.add_option(
+        group.add_argument(
             "--nostdpf",
             default=False,
             action="store_true",
             help="Do not standardize contig names",
         )
-        group.add_option(
+        group.add_argument(
             "--genomenames",
-            type="string",
+            type=str,
             default=None,
             help="genome names for labeling axes in the form of qname_sname, "
             'eg. "*Vitis vinifera*_*Oryza sativa*"',
         )
-        group.add_option(
+        group.add_argument(
             "--theme",
             choices=[str(x) for x in range(len(set1))],
             default=str(theme),
             help="Color index within the palette for contig grid boundaries. Palette contains: {}".format(
                 "|".join(set1)
             ),
         )
-        self.add_option_group(group)
-        return group
 
     def set_depth(self, depth=50):
-        self.add_option("--depth", default=depth, type="float", help="Desired depth")
+        self.add_argument("--depth", default=depth, type=float, help="Desired depth")
 
     def set_rclip(self, rclip=0):
-        self.add_option(
+        self.add_argument(
             "--rclip",
             default=rclip,
-            type="int",
+            type=int,
             help="Pair ID is derived from rstrip N chars",
         )
 
     def set_chr(self, chr=",".join([str(x) for x in range(1, 23)] + ["X", "Y", "MT"])):
-        self.add_option("--chr", default=chr, help="Chromosomes to process")
+        self.add_argument("--chr", default=chr, help="Chromosomes to process")
 
     def set_ref(self, ref="/mnt/ref"):
-        self.add_option("--ref", default=ref, help="Reference folder")
+        self.add_argument("--ref", default=ref, help="Reference folder")
 
     def set_cutoff(self, cutoff=0):
-        self.add_option(
+        self.add_argument(
             "--cutoff",
             default=cutoff,
-            type="int",
+            type=int,
             help="Distance to call valid links between mates",
         )
 
     def set_mateorientation(self, mateorientation=None):
-        self.add_option(
+        self.add_argument(
             "--mateorientation",
             default=mateorientation,
             choices=("++", "--", "+-", "-+"),
             help="Use only certain mate orientations",
         )
 
     def set_mates(self, rclip=0, cutoff=0, mateorientation=None):
         self.set_rclip(rclip=rclip)
         self.set_cutoff(cutoff=cutoff)
         self.set_mateorientation(mateorientation=mateorientation)
 
     def set_bedpe(self):
-        self.add_option(
+        self.add_argument(
             "--norc",
             dest="rc",
             default=True,
             action="store_false",
             help="Do not reverse complement, expect innie reads",
         )
-        self.add_option(
-            "--minlen", default=2000, type="int", help="Minimum insert size"
+        self.add_argument(
+            "--minlen", default=2000, type=int, help="Minimum insert size"
         )
-        self.add_option(
-            "--maxlen", default=8000, type="int", help="Maximum insert size"
+        self.add_argument(
+            "--maxlen", default=8000, type=int, help="Maximum insert size"
         )
-        self.add_option(
+        self.add_argument(
             "--dup",
             default=10,
-            type="int",
+            type=int,
             help="Filter duplicates with coordinates within this distance",
         )
 
     def set_fastq_names(self):
-        self.add_option(
+        self.add_argument(
             "--names",
             default="*.fq,*.fastq,*.fq.gz,*.fastq.gz",
             help="File names to search, use comma to separate multiple",
         )
 
     def set_pairs(self):
         """
@@ -745,264 +746,262 @@
         Report how many paired ends mapped, avg distance between paired ends, etc.
         Paired reads must have the same prefix, use --rclip to remove trailing
         part, e.g. /1, /2, or .f, .r, default behavior is to truncate until last
         char.
         """
         self.set_usage(self.set_pairs.__doc__)
 
-        self.add_option(
+        self.add_argument(
             "--pairsfile", default=None, help="Write valid pairs to pairsfile"
         )
-        self.add_option(
-            "--nrows", default=200000, type="int", help="Only use the first n lines"
+        self.add_argument(
+            "--nrows", default=200000, type=int, help="Only use the first n lines"
         )
         self.set_mates()
-        self.add_option(
+        self.add_argument(
             "--pdf",
             default=False,
             action="store_true",
             help="Print PDF instead ASCII histogram",
         )
-        self.add_option(
-            "--bins", default=20, type="int", help="Number of bins in the histogram"
+        self.add_argument(
+            "--bins", default=20, type=int, help="Number of bins in the histogram"
         )
-        self.add_option(
+        self.add_argument(
             "--distmode",
             default="ss",
             choices=("ss", "ee"),
             help="Distance mode between paired reads, ss is outer distance, "
             "ee is inner distance",
         )
 
     def set_sep(self, sep="\t", help="Separator in the tabfile", multiple=False):
         if multiple:
             help += ", multiple values allowed"
-        self.add_option("--sep", default=sep, help=help)
+        self.add_argument("--sep", default=sep, help=help)
 
     def set_firstN(self, firstN=100000):
-        self.add_option(
-            "--firstN", default=firstN, type="int", help="Use only the first N reads"
+        self.add_argument(
+            "--firstN", default=firstN, type=int, help="Use only the first N reads"
         )
 
     def set_tag(self, tag=False, specify_tag=False):
         if not specify_tag:
-            self.add_option(
+            self.add_argument(
                 "--tag",
                 default=tag,
                 action="store_true",
                 help="Add tag (/1, /2) to the read name",
             )
         else:
             tag_choices = ["/1", "/2"]
-            self.add_option(
+            self.add_argument(
                 "--tag",
                 default=None,
                 choices=tag_choices,
                 help="Specify tag to be added to read name",
             )
 
     def set_phred(self, phred=None):
         phdchoices = ("33", "64")
-        self.add_option(
+        self.add_argument(
             "--phred",
             default=phred,
             choices=phdchoices,
             help="Phred score offset {0} [default: guess]".format(phdchoices),
         )
 
     def set_size(self, size=0):
-        self.add_option(
+        self.add_argument(
             "--size",
             default=size,
-            type="int",
+            type=int,
             help="Insert mean size, stdev assumed to be 20% around mean",
         )
 
     def set_trinity_opts(self):
         self.set_home("trinity")
         self.set_home("hpcgridrunner")
         self.set_cpus()
         self.set_params(prog="Trinity")
-        topts = OptionGroup(self, "General Trinity options")
-        self.add_option_group(topts)
-        topts.add_option(
+        topts = self.add_argument_group("General Trinity options")
+        topts.add_argument(
             "--max_memory",
             default="128G",
-            type="str",
+            type=str,
             help="Jellyfish memory allocation",
         )
-        topts.add_option(
+        topts.add_argument(
             "--min_contig_length",
             default=90,
-            type="int",
+            type=int,
             help="Minimum assembled contig length to report",
         )
-        topts.add_option(
+        topts.add_argument(
             "--bflyGCThreads",
             default=None,
-            type="int",
+            type=int,
             help="Threads for garbage collection",
         )
-        topts.add_option(
+        topts.add_argument(
             "--grid_conf_file",
             default="JCVI_SGE.0689.conf",
-            type="str",
+            type=str,
             help="HpcGridRunner config file for supported compute farms",
         )
-        topts.add_option(
+        topts.add_argument(
             "--cleanup",
             default=False,
             action="store_true",
             help="Force clean-up of unwanted files after Trinity run is complete",
         )
-        ggopts = OptionGroup(self, "Genome-guided Trinity options")
-        self.add_option_group(ggopts)
-        ggopts.add_option(
+        ggopts = self.add_argument_group("Genome-guided Trinity options")
+        ggopts.add_argument(
             "--bam",
             default=None,
-            type="str",
+            type=str,
             help="provide coord-sorted bam file as starting point",
         )
-        ggopts.add_option(
+        ggopts.add_argument(
             "--max_intron",
             default=15000,
-            type="int",
+            type=int,
             help="maximum allowed intron length",
         )
 
     def set_pasa_opts(self, action="assemble"):
         self.set_home("pasa")
         if action == "assemble":
             self.set_home("tgi")
-            self.add_option(
+            self.add_argument(
                 "--clean",
                 default=False,
                 action="store_true",
                 help="Clean transcripts using tgi seqclean",
             )
             self.set_align(pctid=95, pctcov=90, intron=15000, bpsplice=3)
-            self.add_option(
+            self.add_argument(
                 "--aligners",
                 default="blat,gmap",
                 help="Specify splice aligners to use for mapping",
             )
-            self.add_option(
+            self.add_argument(
                 "--fl_accs",
                 default=None,
-                type="str",
+                type=str,
                 help="File containing list of FL-cDNA accessions",
             )
             self.set_cpus()
-            self.add_option(
+            self.add_argument(
                 "--compreh",
                 default=False,
                 action="store_true",
                 help="Run comprehensive transcriptome assembly",
             )
             self.set_align(compreh_pctid=95, compreh_pctcov=30)
-            self.add_option(
+            self.add_argument(
                 "--prefix",
                 default="compreh_init_build",
-                type="str",
+                type=str,
                 help="Prefix for compreh_trans output file names",
             )
         elif action == "compare":
-            self.add_option(
+            self.add_argument(
                 "--annots_gff3",
                 default=None,
-                type="str",
+                type=str,
                 help="Reference annotation to load and compare against",
             )
             genetic_code = [
                 "universal",
                 "Euplotes",
                 "Tetrahymena",
                 "Candida",
                 "Acetabularia",
             ]
-            self.add_option(
+            self.add_argument(
                 "--genetic_code",
                 default="universal",
                 choices=genetic_code,
                 help="Choose translation table",
             )
-            self.add_option(
+            self.add_argument(
                 "--pctovl",
                 default=50,
-                type="int",
+                type=int,
                 help="Minimum pct overlap between gene and FL assembly",
             )
-            self.add_option(
+            self.add_argument(
                 "--pct_coding",
                 default=50,
-                type="int",
+                type=int,
                 help="Minimum pct of cDNA sequence to be protein coding",
             )
-            self.add_option(
+            self.add_argument(
                 "--orf_size",
                 default=0,
-                type="int",
+                type=int,
                 help="Minimum size of ORF encoded protein",
             )
-            self.add_option(
-                "--utr_exons", default=2, type="int", help="Maximum number of UTR exons"
+            self.add_argument(
+                "--utr_exons", default=2, type=int, help="Maximum number of UTR exons"
             )
-            self.add_option(
+            self.add_argument(
                 "--pctlen_FL",
                 default=70,
-                type="int",
+                type=int,
                 help="Minimum protein length for comparisons involving "
                 + "FL assemblies",
             )
-            self.add_option(
+            self.add_argument(
                 "--pctlen_nonFL",
                 default=70,
-                type="int",
+                type=int,
                 help="Minimum protein length for comparisons involving "
                 + "non-FL assemblies",
             )
-            self.add_option(
+            self.add_argument(
                 "--pctid_prot",
                 default=70,
-                type="int",
+                type=int,
                 help="Minimum pctid allowed for protein pairwise comparison",
             )
-            self.add_option(
+            self.add_argument(
                 "--pct_aln",
                 default=70,
-                type="int",
+                type=int,
                 help="Minimum pct of shorter protein length aligning to "
                 + "update protein or isoform",
             )
-            self.add_option(
+            self.add_argument(
                 "--pctovl_gene",
                 default=80,
-                type="int",
+                type=int,
                 help="Minimum pct overlap among genome span of the ORF of "
                 + "each overlapping gene to allow merging",
             )
-            self.add_option(
+            self.add_argument(
                 "--stompovl",
                 default="",
                 action="store_true",
                 help="Ignore alignment results, only consider genome span of ORF",
             )
-            self.add_option(
+            self.add_argument(
                 "--trust_FL",
                 default="",
                 action="store_true",
                 help="Trust FL-status of cDNA",
             )
 
     def set_annot_reformat_opts(self):
-        self.add_option(
-            "--pad0", default=6, type="int", help="Pad gene identifiers with 0"
+        self.add_argument(
+            "--pad0", default=6, type=int, help="Pad gene identifiers with 0"
         )
-        self.add_option("--prefix", default="Medtr", help="Genome prefix")
-        self.add_option(
+        self.add_argument("--prefix", default="Medtr", help="Genome prefix")
+        self.add_argument(
             "--uc",
             default=False,
             action="store_true",
             help="Toggle gene identifier upper case",
         )
 
     def set_home(self, prog, default=None):
@@ -1011,24 +1010,24 @@
             try:
                 default = op.dirname(which(prog))
             except:
                 default = None
         else:
             default = op.expanduser(default)
         help = f"Home directory for {prog.upper()}"
-        self.add_option(tag, default=default, help=help)
+        self.add_argument(tag, default=default, help=help)
 
     def set_aligner(self, aligner="bowtie"):
         valid_aligners = ("bowtie", "bwa")
-        self.add_option(
+        self.add_argument(
             "--aligner", default=aligner, choices=valid_aligners, help="Use aligner"
         )
 
     def set_verbose(self, help="Print detailed reports"):
-        self.add_option("--verbose", default=False, action="store_true", help=help)
+        self.add_argument("--verbose", default=False, action="store_true", help=help)
 
 
 def ConfigSectionMap(Config, section):
     """
     Read a specific section from a ConfigParser() object and return
     a dict of all key-value pairs in that section
     """
@@ -1566,15 +1565,15 @@
     """
     %prog expand */*
 
     Move files in subfolders into the current folder. Use --symlink to create a
     link instead.
     """
     p = OptionParser(expand.__doc__)
-    p.add_option(
+    p.add_argument(
         "--symlink", default=False, action="store_true", help="Create symbolic link"
     )
     opts, args = p.parse_args(args)
 
     if len(args) < 1:
         sys.exit(not p.print_help())
 
@@ -1933,45 +1932,44 @@
     Push notify: Uses available API
     """
     valid_notif_methods.extend(available_push_api.keys())
 
     fromaddr = get_email_address(whoami="notifier")
 
     p = OptionParser(notify.__doc__)
-    p.add_option(
+    p.add_argument(
         "--method",
         default="email",
         choices=valid_notif_methods,
         help="Specify the mode of notification",
     )
-    p.add_option(
+    p.add_argument(
         "--subject",
         default="JCVI: job monitor",
         help="Specify the subject of the notification message",
     )
     p.set_email()
 
-    g1 = OptionGroup(p, "Optional `push` parameters")
-    g1.add_option(
+    g1 = p.add_argument_group("Optional `push` parameters")
+    g1.add_argument(
         "--api",
         default="pushover",
         choices=flatten(available_push_api.values()),
         help="Specify API used to send the push notification",
     )
-    g1.add_option(
-        "--priority", default=0, type="int", help="Message priority (-1 <= p <= 2)"
+    g1.add_argument(
+        "--priority", default=0, type=int, help="Message priority (-1 <= p <= 2)"
     )
-    g1.add_option(
+    g1.add_argument(
         "--timestamp",
         default=None,
-        type="int",
+        type=int,
         dest="timestamp",
         help="Message timestamp in unix format",
     )
-    p.add_option_group(g1)
 
     opts, args = p.parse_args(args)
 
     if len(args) == 0:
         logger.error("Please provide a brief message to be sent")
         sys.exit(not p.print_help())
 
@@ -2092,27 +2090,27 @@
     Specify `--grid` option to send the new process to the grid after waiting for PID
     """
     import shlex
 
     valid_notif_methods.extend(flatten(available_push_api.values()))
 
     p = OptionParser(waitpid.__doc__)
-    p.add_option(
+    p.add_argument(
         "--notify",
         default="email",
         choices=valid_notif_methods,
         help="Specify type of notification to be sent after waiting",
     )
-    p.add_option(
+    p.add_argument(
         "--interval",
         default=120,
-        type="int",
+        type=int,
         help="Specify PID polling interval in seconds",
     )
-    p.add_option("--message", help="Specify notification message")
+    p.add_argument("--message", help="Specify notification message")
     p.set_email()
     p.set_grid()
     opts, args = p.parse_args(args)
 
     if len(args) == 0:
         sys.exit(not p.print_help())
```

### Comparing `jcvi-1.4.6/jcvi/apps/biomart.py` & `jcvi-1.4.7/jcvi/apps/biomart.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,19 @@
 """
 Builds the queries for Globus and BioMart servie, usefu for extraction of
 phytozome data sets.  Certain portion of the codes are ported from R package
 `biomaRt` (thanks).
 """
 import sys
 import urllib
-import logging
 
 from urllib.parse import urljoin
-
 from xml.etree.ElementTree import ElementTree, Element, SubElement, tostring
 
-from jcvi.apps.base import OptionParser, ActionDispatcher, download
+from .base import ActionDispatcher, OptionParser, download, logger
 
 
 class GlobusXMLParser(ElementTree):
     def __init__(self, xml_file):
         """Parse an Globus directory listing XML file
 
         Args:
@@ -119,15 +117,15 @@
         for t in self.getiterator("AttributeDescription"):
             yield Attribute(**t.attrib)
 
         # the filters
         for t in self.getiterator("FilterDescription"):
             f = Filter(**t.attrib)
             options = [Option(**x.attrib) for x in t.getiterator("Option")]
-            f.add_options(options)
+            f.add_arguments(options)
             yield f
 
 
 class Mart(dict):
     def __init__(
         self,
         host="www.biomart.org",
@@ -313,15 +311,15 @@
     """
     Filters define a restriction on the query.
 
     For example, you can restrict output to all genes located on chr. 1
     then use the filter chromosome_name with value `1`
     """
 
-    def add_options(self, options):
+    def add_arguments(self, options):
         self.options = dict((x.displayName, x) for x in options)
 
 
 class Option(MartArgument):
     pass
 
 
@@ -412,15 +410,15 @@
     for i, row in enumerate(data):
         row = row.strip()
         if row == "":
             continue
 
         print(row, file=fw)
 
-    logging.debug("A total of {0} records written to `{1}`.".format(i + 1, bedfile))
+    logger.debug("A total of %d records written to `%s`.", i + 1, bedfile)
 
 
 if __name__ == "__main__":
 
     import doctest
 
     doctest.testmod()
```

### Comparing `jcvi-1.4.6/jcvi/apps/blastplus.py` & `jcvi-1.4.7/jcvi/apps/blastplus.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,76 +1,76 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 import os.path as op
 import sys
-import logging
 
 from multiprocessing import Lock
 
-from jcvi.formats.base import must_open, split
-from jcvi.apps.grid import Jobs
-from jcvi.apps.align import run_formatdb
-from jcvi.apps.base import OptionParser, Popen
+from ..formats.base import must_open, split
+
+from .align import run_formatdb
+from .base import OptionParser, Popen, logger
+from .grid import Jobs
 
 
 def blastplus(out_fh, cmd, query, lock):
     cmd += " -query {0}".format(query)
     proc = Popen(cmd)
 
-    logging.debug("job <%d> started: %s" % (proc.pid, cmd))
+    logger.debug("job <%d> started: %s", proc.pid, cmd)
     for row in proc.stdout:
         if row[0] == "#":
             continue
         lock.acquire()
         out_fh.write(row)
         out_fh.flush()
         lock.release()
-    logging.debug("job <%d> finished" % proc.pid)
+    logger.debug("job <%d> finished", proc.pid)
 
 
 def main():
     """
     %prog database.fa query.fa [options]
 
     Wrapper for NCBI BLAST+.
     """
     p = OptionParser(main.__doc__)
 
-    p.add_option(
+    p.add_argument(
         "--format",
         default=" '6 qseqid sseqid pident length "
         "mismatch gapopen qstart qend sstart send evalue bitscore' ",
         help='0-11, learn more with "blastp -help"',
     )
-    p.add_option(
+    p.add_argument(
         "--path",
         dest="blast_path",
         default=None,
         help="specify BLAST+ path including the program name",
     )
-    p.add_option(
+    p.add_argument(
         "--prog",
         dest="blast_program",
         default="blastp",
         help="specify BLAST+ program to use. See complete list here: "
         "http://www.ncbi.nlm.nih.gov/books/NBK52640/#chapter1.Installation",
     )
     p.set_align(evalue=0.01)
-    p.add_option(
+    p.add_argument(
         "--best",
         default=1,
-        type="int",
+        type=int,
         help="Only look for best N hits",
     )
     p.set_cpus()
-    p.add_option(
+    p.add_argument(
         "--nprocs",
         default=1,
-        type="int",
+        type=int,
         help="number of BLAST processes to run in parallel. "
         + "split query.fa into `nprocs` chunks, "
         + "each chunk uses -num_threads=`cpus`",
     )
     p.set_params()
     p.set_outfile()
     opts, args = p.parse_args()
@@ -92,15 +92,15 @@
 
     blast_bin = blast_path or blast_program
     if op.basename(blast_bin) != blast_program:
         blast_bin = op.join(blast_bin, blast_program)
 
     nprocs, cpus = opts.nprocs, opts.cpus
     if nprocs > 1:
-        logging.debug("Dispatch job to %d processes" % nprocs)
+        logger.debug("Dispatch job to %d processes", nprocs)
         outdir = "outdir"
         fs = split([afasta_fn, outdir, str(nprocs)])
         queries = fs.names
     else:
         queries = [afasta_fn]
 
     dbtype = "prot" if op.basename(blast_bin) in ("blastp", "blastx") else "nucl"
```

### Comparing `jcvi-1.4.6/jcvi/apps/bowtie.py` & `jcvi-1.4.7/jcvi/apps/bowtie.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,27 @@
 """
 Run bowtie2 command and skips the manual run of naming intermediate output
 files. Bowtie2 help:
 
 <http://bowtie-bio.sourceforge.net/bowtie2/index.shtml>
 """
 import sys
-import logging
 
-from jcvi.formats.base import BaseFile
-from jcvi.utils.cbook import percentage
-from jcvi.formats.sam import output_bam, get_prefix, get_samfile
-from jcvi.apps.base import OptionParser, ActionDispatcher, need_update, sh, get_abs_path
+from ..formats.base import BaseFile
+from ..formats.sam import get_prefix, get_samfile, output_bam
+from ..utils.cbook import percentage
+
+from .base import (
+    ActionDispatcher,
+    OptionParser,
+    logger,
+    need_update,
+    sh,
+    get_abs_path,
+)
 
 
 first_tag = lambda fp: next(fp).split()[0]
 
 
 class BowtieLogFile(BaseFile):
     """
@@ -63,15 +70,15 @@
 def check_index(dbfile):
     dbfile = get_abs_path(dbfile)
     safile = dbfile + ".1.bt2"
     if need_update(dbfile, safile):
         cmd = "bowtie2-build {0} {0}".format(dbfile)
         sh(cmd)
     else:
-        logging.error("`{0}` exists. `bowtie2-build` already run.".format(safile))
+        logger.error("`{0}` exists. `bowtie2-build` already run.".format(safile))
 
     return dbfile
 
 
 def index(args):
     """
     %prog index database.fasta
@@ -94,33 +101,33 @@
 
     Wrapper for `bowtie2` single-end or paired-end, depending on the number of args.
     """
     from jcvi.formats.fastq import guessoffset
 
     p = OptionParser(align.__doc__)
     p.set_firstN(firstN=0)
-    p.add_option(
+    p.add_argument(
         "--full",
         default=False,
         action="store_true",
         help="Enforce end-to-end alignment [default: local]",
     )
-    p.add_option(
+    p.add_argument(
         "--reorder",
         default=False,
         action="store_true",
         help="Keep the input read order",
     )
-    p.add_option(
+    p.add_argument(
         "--null",
         default=False,
         action="store_true",
         help="Do not write to SAM/BAM output",
     )
-    p.add_option(
+    p.add_argument(
         "--fasta", default=False, action="store_true", help="Query reads are FASTA"
     )
     p.set_cutoff(cutoff=800)
     p.set_mateorientation(mateorientation="+-")
     p.set_sam_options(bowtie=True)
 
     opts, args = p.parse_args(args)
@@ -131,18 +138,18 @@
     elif mo == "-+":
         extra += "--rf"
     else:
         extra += "--ff"
 
     PE = True
     if len(args) == 2:
-        logging.debug("Single-end alignment")
+        logger.debug("Single-end alignment")
         PE = False
     elif len(args) == 3:
-        logging.debug("Paired-end alignment")
+        logger.debug("Paired-end alignment")
     else:
         sys.exit(not p.print_help())
 
     firstN = opts.firstN
     mapped = opts.mapped
     unmapped = opts.unmapped
     fasta = opts.fasta
@@ -155,15 +162,15 @@
         readfile, dbfile, bowtie=True, mapped=mapped, unmapped=unmapped, bam=opts.bam
     )
     logfile = prefix + ".log"
     if not fasta:
         offset = guessoffset([readfile])
 
     if not need_update(dbfile, samfile):
-        logging.error("`{0}` exists. `bowtie2` already run.".format(samfile))
+        logger.error("`{0}` exists. `bowtie2` already run.".format(samfile))
         return samfile, logfile
 
     cmd = "bowtie2 -x {0}".format(dbfile)
     if PE:
         r1, r2 = args[1:3]
         cmd += " -1 {0} -2 {1}".format(r1, r2)
         cmd += " --maxins {0}".format(opts.cutoff)
```

### Comparing `jcvi-1.4.6/jcvi/apps/bwa.py` & `jcvi-1.4.7/jcvi/apps/bwa.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 Run bwa command and skips the manual run of naming intermediate output files
 The whole pipeline is following bwa documentation at
 <http://bio-bwa.sf.net/bwa.shtml>
 """
 
 import os.path as op
 import sys
-import logging
 
-from jcvi.formats.sam import output_bam, get_samfile, mapped
-from jcvi.assembly.automaton import iter_project
-from jcvi.apps.grid import MakeManager
-from jcvi.apps.base import (
+from ..apps.grid import MakeManager
+from ..assembly.automaton import iter_project
+from ..formats.sam import get_samfile, mapped, output_bam
+
+from .base import (
     ActionDispatcher,
     OptionParser,
     cleanup,
     get_abs_path,
+    logger,
     mkdir,
     need_update,
     sh,
 )
 
 
 def main():
@@ -80,15 +81,15 @@
 def check_index(dbfile):
     dbfile = get_abs_path(dbfile)
     safile = dbfile + ".sa"
     if not op.exists(safile):
         cmd = "bwa index {0}".format(dbfile)
         sh(cmd)
     else:
-        logging.error("`{0}` exists. `bwa index` already run.".format(safile))
+        logger.error("`{0}` exists. `bwa index` already run.".format(safile))
 
     return dbfile
 
 
 def check_aln(dbfile, readfile, cpus=32):
     from jcvi.formats.fastq import guessoffset
 
@@ -97,15 +98,15 @@
         offset = guessoffset([readfile])
         cmd = "bwa aln " + " ".join((dbfile, readfile))
         cmd += " -t {0}".format(cpus)
         if offset == 64:
             cmd += " -I"
         sh(cmd, outfile=saifile)
     else:
-        logging.error("`{0}` exists. `bwa aln` already run.".format(saifile))
+        logger.error("`{0}` exists. `bwa aln` already run.".format(saifile))
 
     return saifile
 
 
 def index(args):
     """
     %prog index database.fasta
@@ -120,17 +121,17 @@
 
     (dbfile,) = args
     check_index(dbfile)
 
 
 def set_align_options(p):
     """Used in align() and batch()"""
-    p.add_option("--bwa", default="bwa", help="Run bwa at this path")
-    p.add_option("--rg", help="Read group")
-    p.add_option(
+    p.add_argument("--bwa", default="bwa", help="Run bwa at this path")
+    p.add_argument("--rg", help="Read group")
+    p.add_argument(
         "--readtype",
         choices=("pacbio", "pbread", "ont2d", "intractg"),
         help="Read type in bwa-mem",
     )
     p.set_cutoff(cutoff=800)
 
 
@@ -138,15 +139,15 @@
     """
     %prog align database.fasta read1.fq [read2.fq]
 
     Wrapper for three modes of BWA - mem (default), aln, bwasw (long reads).
     """
     valid_modes = ("bwasw", "aln", "mem")
     p = OptionParser(align.__doc__)
-    p.add_option("--mode", default="mem", choices=valid_modes, help="BWA mode")
+    p.add_argument("--mode", default="mem", choices=valid_modes, help="BWA mode")
     set_align_options(p)
     p.set_sam_options()
 
     opts, args = p.parse_args(args)
     mode = opts.mode
     nargs = len(args)
 
@@ -163,15 +164,15 @@
             c = samse
     else:
         assert mode != "bwasw", "Cannot use --bwasw with paired-end mode"
         tag += "Paired-end alignment"
         if mode == "aln":
             c = sampe
 
-    logging.debug(tag)
+    logger.debug(tag)
     cmd, samfile = c(args, opts)
     if cmd:
         cmd = output_bam(cmd, samfile)
 
     bam = opts.bam
     unmapped = opts.unmapped
 
@@ -196,15 +197,15 @@
     dbfile = check_index(dbfile)
     saifile = check_aln(dbfile, readfile, cpus=opts.cpus)
 
     samfile, _, unmapped = get_samfile(
         readfile, dbfile, bam=opts.bam, unmapped=opts.unmapped
     )
     if not need_update((dbfile, saifile), samfile):
-        logging.error("`{0}` exists. `bwa samse` already run.".format(samfile))
+        logger.error("`{0}` exists. `bwa samse` already run.".format(samfile))
         return "", samfile
 
     cmd = "bwa samse {0} {1} {2}".format(dbfile, saifile, readfile)
     cmd += " " + opts.extra
     if opts.uniq:
         cmd += " -n 1"
 
@@ -222,15 +223,15 @@
     sai1file = check_aln(dbfile, read1file, cpus=opts.cpus)
     sai2file = check_aln(dbfile, read2file, cpus=opts.cpus)
 
     samfile, _, unmapped = get_samfile(
         read1file, dbfile, bam=opts.bam, unmapped=opts.unmapped
     )
     if not need_update((dbfile, sai1file, sai2file), samfile):
-        logging.error("`{0}` exists. `bwa samse` already run.".format(samfile))
+        logger.error("`{0}` exists. `bwa samse` already run.".format(samfile))
         return "", samfile
 
     cmd = "bwa sampe " + " ".join((dbfile, sai1file, sai2file, read1file, read2file))
     cmd += " " + opts.extra
     if opts.cutoff:
         cmd += " -a {0}".format(opts.cutoff)
     if opts.uniq:
@@ -253,15 +254,15 @@
     rg = opts.rg or r"@RG\tID:{0}\tSM:sm\tLB:lb\tPL:{1}".format(pf, pl)
     dbfile = check_index(dbfile)
     args[0] = dbfile
     samfile, _, unmapped = get_samfile(
         read1file, dbfile, bam=opts.bam, unmapped=opts.unmapped
     )
     if not need_update(read1file, samfile):
-        logging.error("`{0}` exists. `bwa mem` already run.".format(samfile))
+        logger.error("`{0}` exists. `bwa mem` already run.".format(samfile))
         return "", samfile
 
     cmd = "{} mem".format(opts.bwa)
     """
     -M Mark shorter split hits as secondary (for Picard compatibility).
     """
     cmd += " -M -t {0}".format(opts.cpus)
@@ -283,15 +284,15 @@
     dbfile, readfile = args
     dbfile = check_index(dbfile)
 
     samfile, _, unmapped = get_samfile(
         readfile, dbfile, bam=opts.bam, unmapped=opts.unmapped
     )
     if not need_update(dbfile, samfile):
-        logging.error("`{0}` exists. `bwa bwasw` already run.".format(samfile))
+        logger.error("`{0}` exists. `bwa bwasw` already run.".format(samfile))
         return "", samfile
 
     cmd = "bwa bwasw " + " ".join(args)
     cmd += " -t {0}".format(opts.cpus)
     cmd += " " + opts.extra
     return cmd, samfile
```

### Comparing `jcvi-1.4.6/jcvi/apps/cdhit.py` & `jcvi-1.4.7/jcvi/apps/cdhit.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 # -*- coding: UTF-8 -*-
 
 """
 Using CD-HIT to remove duplicate reads.
 """
 import os.path as op
 import sys
-import logging
 
 from collections import defaultdict
 
-from jcvi.formats.base import LineFile, read_block, must_open
-from jcvi.formats.fastq import fasta
-from jcvi.utils.cbook import percentage
-from jcvi.apps.base import OptionParser, ActionDispatcher, need_update, sh
+from ..formats.base import LineFile, read_block, must_open
+from ..formats.fastq import fasta
+from ..utils.cbook import percentage
+
+from .base import ActionDispatcher, OptionParser, logger, need_update, sh
 
 
 class ClstrLine(object):
     """
     Lines like these:
     0       12067nt, >LAP012517... at -/99.85%
     1       15532nt, >MOL158919... *
@@ -80,15 +80,15 @@
     %prog filter *.consensus.fasta
 
     Filter consensus sequence with min cluster size.
     """
     from jcvi.formats.fasta import Fasta, SeqIO
 
     p = OptionParser(filter.__doc__)
-    p.add_option("--minsize", default=2, type="int", help="Minimum cluster size")
+    p.add_argument("--minsize", default=2, type=int, help="Minimum cluster size")
     p.set_outfile()
     opts, args = p.parse_args(args)
 
     if len(args) < 1:
         sys.exit(not p.print_help())
 
     fastafiles = args
@@ -111,36 +111,34 @@
             size = int(size)
             nreads += size
             if size < minsize:
                 continue
             rec.description = rec.description.split(None, 1)[-1]
             rec.id = pf + "_" + rec.id
             SeqIO.write(rec, fw, "fasta")
-        logging.debug(
-            "Scanned {0} clusters with {1} reads ..".format(nclusters, nreads)
-        )
+        logger.debug("Scanned {0} clusters with {1} reads ..".format(nclusters, nreads))
         cclusters, creads = nclusters - nsingletons, nreads - nsingletons
-        logging.debug(
+        logger.debug(
             "Saved {0} clusters (min={1}) with {2} reads (avg:{3}) [{4}]".format(
                 cclusters, minsize, creads, creads / cclusters, pf
             )
         )
         totalreads += nreads
         totalassembled += nreads - nsingletons
-    logging.debug("Total assembled: {0}".format(percentage(totalassembled, totalreads)))
+    logger.debug("Total assembled: {0}".format(percentage(totalassembled, totalreads)))
 
 
 def ids(args):
     """
     %prog ids cdhit.clstr
 
     Get the representative ids from clstr file.
     """
     p = OptionParser(ids.__doc__)
-    p.add_option("--prefix", type="int", help="Find rep id for prefix of len")
+    p.add_argument("--prefix", type=int, help="Find rep id for prefix of len")
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (clstrfile,) = args
     cf = ClstrFile(clstrfile)
@@ -152,15 +150,15 @@
 
     nreads = len(reads)
     idsfile = clstrfile.replace(".clstr", ".ids")
     fw = open(idsfile, "w")
     for i, name in reads:
         print("\t".join(str(x) for x in (i, name)), file=fw)
 
-    logging.debug(
+    logger.debug(
         "A total of {0} unique reads written to `{1}`.".format(nreads, idsfile)
     )
     fw.close()
 
     return idsfile
 
 
@@ -188,33 +186,33 @@
     """
     %prog deduplicate fastafile
 
     Wraps `cd-hit-est` to remove duplicate sequences.
     """
     p = OptionParser(deduplicate.__doc__)
     p.set_align(pctid=96, pctcov=0)
-    p.add_option(
+    p.add_argument(
         "--fast",
         default=False,
         action="store_true",
         help="Place sequence in the first cluster",
     )
-    p.add_option(
+    p.add_argument(
         "--consensus",
         default=False,
         action="store_true",
         help="Compute consensus sequences",
     )
-    p.add_option(
+    p.add_argument(
         "--reads",
         default=False,
         action="store_true",
         help="Use `cd-hit-454` to deduplicate",
     )
-    p.add_option(
+    p.add_argument(
         "--samestrand",
         default=False,
         action="store_true",
         help="Enforce same strand alignment",
     )
     p.set_home("cdhit")
     p.set_cpus()
```

### Comparing `jcvi-1.4.6/jcvi/apps/emboss.py` & `jcvi-1.4.7/jcvi/apps/emboss.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 """
 Run EMBOSS programs.
 """
 import sys
 import multiprocessing as mp
 
-from jcvi.apps.base import ActionDispatcher, OptionParser, cleanup
-from jcvi.formats.base import must_open
+from ..formats.base import must_open
+from .base import ActionDispatcher, OptionParser, cleanup
 
 
 class NeedleHeader(object):
     def __init__(self, filename):
         fp = must_open(filename)
         for row in fp:
             if row[0] != "#":
```

### Comparing `jcvi-1.4.6/jcvi/apps/fetch.py` & `jcvi-1.4.7/jcvi/apps/fetch.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 """
 Wrapper for fetching data from various online repositories \
 (Entrez, Ensembl, Phytozome, and SRA)
 """
 
-import logging
 import os.path as op
 import re
 import sys
 import time
 
 from os.path import join as urljoin
 from urllib.error import HTTPError, URLError
 
 from Bio import Entrez, SeqIO
 from more_itertools import grouper
 
-from jcvi.formats.base import must_open
-from jcvi.formats.fasta import print_first_difference
-from jcvi.formats.fastq import fromsra
-from jcvi.utils.cbook import tile
-from jcvi.utils.console import printf
-from jcvi.apps.base import (
+from ..formats.base import must_open
+from ..formats.fasta import print_first_difference
+from ..formats.fastq import fromsra
+from ..utils.cbook import tile
+from ..utils.console import printf
+
+from .base import (
     ActionDispatcher,
     OptionParser,
+    logger,
     cleanup,
     download,
     get_email_address,
     last_updated,
     ls_ftp,
     mkdir,
     sh,
@@ -66,42 +67,42 @@
 ):
     """
     Retrieve multiple rather than a single record
     """
 
     for term in list_of_terms:
 
-        logging.debug("Search term %s", term)
+        logger.debug("Search term %s", term)
         success = False
         ids = None
         if not term:
             continue
 
         while not success:
             try:
                 search_handle = Entrez.esearch(db=db, retmax=retmax, term=term)
                 rec = Entrez.read(search_handle)
                 success = True
                 ids = rec["IdList"]
             except (HTTPError, URLError, RuntimeError, KeyError) as e:
-                logging.error(e)
-                logging.debug("wait 5 seconds to reconnect...")
+                logger.error(e)
+                logger.debug("wait 5 seconds to reconnect...")
                 time.sleep(5)
 
         if not ids:
-            logging.error("term {0} not found".format(term))
+            logger.error("term {0} not found".format(term))
             continue
 
         assert ids
         nids = len(ids)
         if nids > 1:
-            logging.debug("A total of {0} results found.".format(nids))
+            logger.debug("A total of {0} results found.".format(nids))
 
         if batchsize != 1:
-            logging.debug("Use a batch size of {0}.".format(batchsize))
+            logger.debug("Use a batch size of {0}.".format(batchsize))
 
         ids = list(grouper(ids, batchsize))
 
         for id in ids:
             id = [x for x in id if x]
             size = len(id)
             id = ",".join(id)
@@ -110,16 +111,16 @@
             while not success:
                 try:
                     fetch_handle = Entrez.efetch(
                         db=db, id=id, rettype=rettype, email=email
                     )
                     success = True
                 except (HTTPError, URLError, RuntimeError) as e:
-                    logging.error(e)
-                    logging.debug("wait 5 seconds to reconnect...")
+                    logger.error(e)
+                    logger.debug("wait 5 seconds to reconnect...")
                     time.sleep(5)
 
             yield id, size, term, fetch_handle
 
 
 def main():
 
@@ -144,15 +145,15 @@
 
     Retrieve genomes and annotations from ensembl FTP. Available species
     listed below. Use comma to give a list of species to download. For example:
 
     $ %prog ensembl danio_rerio,gasterosteus_aculeatus
     """
     p = OptionParser(ensembl.__doc__)
-    p.add_option("--version", default="75", help="Ensembl version")
+    p.add_argument("--version", default="75", help="Ensembl version")
     opts, args = p.parse_args(args)
 
     version = opts.version
     url = "ftp://ftp.ensembl.org/pub/release-{0}/".format(version)
     fasta_url = url + "fasta/"
 
     valid_species = [x for x in ls_ftp(fasta_url) if "." not in x]
@@ -192,23 +193,23 @@
     if console.is_terminal:
         username = console.input("[bold green]Phytozome Login: ")
         pw = console.input("[bold green]Phytozome Password: ", password=True)
     else:
         username, pw = None, None
     curlcmd = which("curl")
     if curlcmd is None:
-        logging.error("curl command not installed. Aborting.")
+        logger.error("curl command not installed. Aborting.")
         return None
     cmd = "{} https://signon.jgi.doe.gov/signon/create".format(curlcmd)
     cmd += " --data-urlencode 'login={0}' --data-urlencode 'password={1}' -b {2} -c {2}".format(
         username, pw, cookies
     )
     sh(cmd, outfile="/dev/null", errfile="/dev/null", log=False)
     if not op.exists(cookies):
-        logging.error("Cookies file `{}` not created. Aborting.".format(cookies))
+        logger.error("Cookies file `{}` not created. Aborting.".format(cookies))
         return None
 
     return cookies
 
 
 def phytozome(args):
     """
@@ -223,27 +224,27 @@
     The downloader will prompt you to enter Phytozome user name and password
     during downloading. Please register for a login at:
     https://phytozome.jgi.doe.gov/pz/portal.html.
     """
     from jcvi.apps.biomart import GlobusXMLParser
 
     p = OptionParser(phytozome.__doc__)
-    p.add_option(
+    p.add_argument(
         "--version",
         default="12",
         choices=("9", "10", "11", "12", "12_unrestricted", "13"),
         help="Phytozome version",
     )
-    p.add_option(
+    p.add_argument(
         "--assembly",
         default=False,
         action="store_true",
         help="Download assembly",
     )
-    p.add_option(
+    p.add_argument(
         "--format",
         default=False,
         action="store_true",
         help="Format to CDS and BED for synteny inference",
     )
     p.set_downloader()
     opts, args = p.parse_args(args)
@@ -255,29 +256,29 @@
     dlist = "{}/ext-api/downloads/get-directory?organism=PhytozomeV{}".format(
         base_url, opts.version
     )
 
     # Make sure we have a valid cookies
     cookies = get_cookies()
     if cookies is None:
-        logging.error("Error fetching cookies ... cleaning up")
+        logger.error("Error fetching cookies ... cleaning up")
         cleanup(directory_listing)
         sys.exit(1)
 
     # Proceed to use the cookies and download the species list
     try:
         download(
             dlist,
             filename=directory_listing,
             cookies=cookies,
             downloader=downloader,
         )
         g = GlobusXMLParser(directory_listing)
     except:
-        logging.error("Error downloading directory listing ... cleaning up")
+        logger.error("Error downloading directory listing ... cleaning up")
         cleanup(directory_listing, cookies)
         sys.exit(1)
 
     genomes = g.get_genomes()
     valid_species = genomes.keys()
     species_tile = tile(valid_species)
     p.set_usage("\n".join((phytozome.__doc__, species_tile)))
@@ -297,15 +298,15 @@
             valid_species,
             base_url,
             cookies,
             assembly=opts.assembly,
             downloader=downloader,
         )
         if not res:
-            logging.error("No files downloaded")
+            logger.error("No files downloaded")
         gff, fa = res.get("gff"), res.get("cds")
         if opts.format:
             format_bed_and_cds(s, gff, fa)
 
 
 def download_species_phytozome(
     genomes, species, valid_species, base_url, cookies, assembly=False, downloader=None
@@ -359,21 +360,21 @@
 
     Retrieve genomes and annotations from phytozome FTP. Available species
     listed below. Use comma to give a list of species to download. For example:
 
     $ %prog phytozome9 Athaliana,Vvinifera,Osativa,Sbicolor,Slycopersicum
     """
     p = OptionParser(phytozome9.__doc__)
-    p.add_option(
+    p.add_argument(
         "--assembly",
         default=False,
         action="store_true",
         help="Download assembly",
     )
-    p.add_option(
+    p.add_argument(
         "--format",
         default=False,
         action="store_true",
         help="Format to CDS and BED for synteny inference",
     )
     opts, args = p.parse_args(args)
 
@@ -392,15 +393,15 @@
         species = ",".join(valid_species)
 
     species = species.split(",")
 
     for s in species:
         res = download_species_phytozome9(s, valid_species, url, assembly=opts.assembly)
         if not res:
-            logging.error("No files downloaded")
+            logger.error("No files downloaded")
         gff, cdsfa = res.get("gff"), res.get("cds")
         if opts.format:
             format_bed_and_cds(s, gff, cdsfa)
 
 
 def format_bed_and_cds(species, gff, cdsfa):
     """Run gff.format() and fasta.format() to generate BED and CDS files.
@@ -448,15 +449,15 @@
 def download_species_phytozome9(species, valid_species, base_url, assembly=False):
     assert species in valid_species, "{} is not in the species list".format(species)
 
     # We want to download assembly and annotation for given species
     surl = urljoin(base_url, species)
     contents = [x for x in ls_ftp(surl) if x.endswith("_readme.txt")]
     magic = contents[0].split("_")[1]  # Get the magic number
-    logging.debug("Found magic number for {0}: {1}".format(species, magic))
+    logger.debug("Found magic number for {0}: {1}".format(species, magic))
 
     pf = "{0}_{1}".format(species, magic)
     asm_url = urljoin(surl, "assembly/{0}.fa.gz".format(pf))
     ann_url = urljoin(surl, "annotation/{0}_gene.gff3.gz".format(pf))
     cds_url = urljoin(surl, "annotation/{0}_cds.fa.gz".format(pf))
     res = {}
     if assembly:
@@ -469,15 +470,15 @@
 def get_first_rec(fastafile):
     """
     Returns the first record in the fastafile
     """
     f = list(SeqIO.parse(fastafile, "fasta"))
 
     if len(f) > 1:
-        logging.debug(
+        logger.debug(
             "{0} records found in {1}, using the first one".format(len(f), fastafile)
         )
 
     return f[0]
 
 
 def bisect(args):
@@ -500,15 +501,15 @@
 
     valid = None
     for i in range(1, 100):
         term = "%s.%d" % (acc, i)
         try:
             query = list(batch_entrez([term], email=opts.email))
         except AssertionError as e:
-            logging.debug(f"no records found for {term}. terminating. {e}")
+            logger.debug(f"no records found for {term}. terminating. {e}")
             return
 
         id, term, handle = query[0]
         brec = next(SeqIO.parse(handle, "fasta"))
 
         match = print_first_difference(
             arec, brec, ignore_case=True, ignore_N=True, rc=True
@@ -541,53 +542,53 @@
         "gss": ["nucgss"],
         "acc": ["nuccore"],
     }
 
     valid_formats = tuple(allowed_databases.keys())
     valid_databases = ("genome", "nuccore", "nucest", "nucgss", "protein", "gene")
 
-    p.add_option(
+    p.add_argument(
         "--noversion",
         dest="noversion",
         default=False,
         action="store_true",
         help="Remove trailing accession versions",
     )
-    p.add_option(
+    p.add_argument(
         "--format",
         default="fasta",
         choices=valid_formats,
         help="download format",
     )
-    p.add_option(
+    p.add_argument(
         "--database",
         default="nuccore",
         choices=valid_databases,
         help="search database",
     )
-    p.add_option(
+    p.add_argument(
         "--retmax",
         default=1000000,
-        type="int",
+        type=int,
         help="how many results to return",
     )
-    p.add_option(
+    p.add_argument(
         "--skipcheck",
         default=False,
         action="store_true",
         help="turn off prompt to check file existence",
     )
-    p.add_option(
+    p.add_argument(
         "--batchsize",
         default=500,
-        type="int",
+        type=int,
         help="download the results in batch for speed-up",
     )
     p.set_outdir(outdir=None)
-    p.add_option("--outprefix", default="out", help="output file name prefix")
+    p.add_argument("--outprefix", default="out", help="output file name prefix")
     p.set_email()
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(p.print_help())
 
     (filename,) = args
@@ -641,15 +642,15 @@
             outfile = urljoin(outdir, "{0}.{1}".format(term, fmt))
             fw = must_open(outfile, "w", checkexists=True, skipcheck=opts.skipcheck)
             if fw is None:
                 continue
 
         rec = handle.read()
         if id in seen:
-            logging.error("Duplicate key ({0}) found".format(rec))
+            logger.error("Duplicate key ({0}) found".format(rec))
             continue
 
         totalsize += size
         print(rec, file=fw)
         print(file=fw)
 
         seen.add(id)
@@ -670,15 +671,15 @@
     The term can also be a file containing list of SRR ids, one per line.
 
     Once downloaded, the SRA file is processed through `fastq-dump` to produce
     FASTQ formatted sequence files, which are gzipped by default.
     """
     p = OptionParser(sra.__doc__)
 
-    p.add_option(
+    p.add_argument(
         "--nogzip",
         dest="nogzip",
         default=False,
         action="store_true",
         help="Do not gzip the FASTQ generated by fastq-dump",
     )
     opts, args = p.parse_args(args)
@@ -704,25 +705,25 @@
 
 def download_srr_term(term):
     sra_base_url = "ftp://ftp-trace.ncbi.nlm.nih.gov/sra/sra-instant/reads/ByRun/sra/"
     sra_run_id_re = re.compile(r"^([DES]RR)(\d{3})(\d{3,4})$")
 
     m = re.search(sra_run_id_re, term)
     if m is None:
-        logging.error(
+        logger.error(
             "Incorrect SRA identifier format "
             + "[should be like SRR126150, SRR1001901. "
             + "len(identifier) should be between 9-10 characters]"
         )
         sys.exit()
 
     prefix, subprefix = m.group(1), "{0}{1}".format(m.group(1), m.group(2))
     download_url = urljoin(
         sra_base_url, prefix, subprefix, term, "{0}.sra".format(term)
     )
 
-    logging.debug("Downloading file: {0}".format(download_url))
+    logger.debug("Downloading file: {0}".format(download_url))
     return download(download_url)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `jcvi-1.4.6/jcvi/apps/gbsubmit.py` & `jcvi-1.4.7/jcvi/apps/gbsubmit.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 
 """
 Prepare the data for Genbank submission
 """
 import os.path as op
 import sys
 import string
-import logging
 
 from collections import defaultdict
 from functools import lru_cache
 
 from Bio import SeqIO
 
-from jcvi.utils.orderedcollections import parse_qs
-from jcvi.formats.base import DictFile
-from jcvi.apps.base import OptionParser, ActionDispatcher, sh, mkdir, glob
+from ..formats.base import DictFile
+from ..utils.orderedcollections import parse_qs
+
+from .base import ActionDispatcher, OptionParser, glob, logger, mkdir, sh
 
 
 """
 GSS submission template files
 
 <http://www.ncbi.nlm.nih.gov/dbGSS/how_to_submit.html>
 """
@@ -131,15 +131,15 @@
 
     contig name, length, span(s), apparent source
     contig0746      11760   1..141  vector
     contig0751      14226   13476..14226    vector
     contig0800      124133  30512..30559    primer/adapter
     """
     p = OptionParser(fcs.__doc__)
-    p.add_option(
+    p.add_argument(
         "--cutoff",
         default=200,
         help="Skip small components less than",
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
@@ -255,15 +255,15 @@
 
     This function is simpler than htg, since the record names have not be
     assigned yet (so less bookkeeping).
     """
     from jcvi.formats.fasta import sequin
 
     p = OptionParser(htgnew.__doc__)
-    p.add_option("--comment", default="", help="Comments for this submission")
+    p.add_argument("--comment", default="", help="Comments for this submission")
     opts, args = p.parse_args(args)
 
     if len(args) != 3:
         sys.exit(not p.print_help())
 
     fastafile, phasefile, sbtfile = args
     comment = opts.comment
@@ -354,20 +354,20 @@
     formats.agp.phase() manually, modify the phasefile and use --phases to override.
     """
     from jcvi.formats.fasta import sequin, ids
     from jcvi.formats.agp import phase
     from jcvi.apps.fetch import entrez
 
     p = OptionParser(htg.__doc__)
-    p.add_option(
+    p.add_argument(
         "--phases",
         default=None,
         help="Use another phasefile to override",
     )
-    p.add_option("--comment", default="", help="Comments for this update")
+    p.add_argument("--comment", default="", help="Comments for this update")
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     fastafile, sbtfile = args
     pf = fastafile.rsplit(".", 1)[0]
@@ -407,15 +407,15 @@
     names = DictFile(namesfile)
     assert len(set(names.keys())) == len(set(names.values()))
 
     phases = DictFile(phasefile)
     ph = [int(x) for x in phases.values()]
     # vmin 1, vmax 4, bins 3
     stem_leaf_plot(ph, 1, 4, 3, title="Counts of phases before updates")
-    logging.debug("Information loaded for {0} records.".format(len(phases)))
+    logger.debug("Information loaded for {0} records.".format(len(phases)))
     assert len(names) == len(phases)
 
     newph = []
 
     cmd = "faSplit byname {0} {1}/".format(fastafile, fastadir)
     sh(cmd, outfile="/dev/null", errfile="/dev/null")
 
@@ -589,15 +589,15 @@
 
     plateMapping = DictFile(mappingfile)
 
     fw = open("MetaData.txt", "w")
     print(PublicationTemplate.format(**vars), file=fw)
     print(LibraryTemplate.format(**vars), file=fw)
     print(ContactTemplate.format(**vars), file=fw)
-    logging.debug("Meta data written to `{0}`".format(fw.name))
+    logger.debug("Meta data written to `{0}`".format(fw.name))
 
     fw = open("GSS.txt", "w")
     fw_log = open("GSS.log", "w")
     for rec in SeqIO.parse(fastafile, "fasta"):
         # First pass just check well number matchings and populate sequences in
         # the same clone
         description = rec.description
@@ -647,28 +647,28 @@
         d = Directions[direction]
 
         cloneID = "{0}{1}".format(plate, w384)
         gssID = "{0}{1}".format(cloneID, d)
         seen[gssID] += 1
 
         if seen[gssID] > 1:
-            logging.error("duplicate key {0} found".format(gssID))
+            logger.error("duplicate key {0} found".format(gssID))
             gssID = "{0}{1}".format(gssID, seen[gssID])
 
         othergss = clone[cloneID] - {gssID}
         othergss = ", ".join(sorted(othergss))
         vars.update(locals())
 
         print(GSSTemplate.format(**vars), file=fw)
 
         # Write conversion logs to log file
         print("{0}\t{1}".format(gssID, description), file=fw_log)
         print("=" * 60, file=fw_log)
 
-    logging.debug("A total of {0} seqs written to `{1}`".format(len(seen), fw.name))
+    logger.debug("A total of {0} seqs written to `{1}`".format(len(seen), fw.name))
     fw.close()
     fw_log.close()
 
 
 if __name__ == "__main__":
     import doctest
```

### Comparing `jcvi-1.4.6/jcvi/apps/gmap.py` & `jcvi-1.4.7/jcvi/apps/gmap.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 Run GMAP/GSNAP commands. GMAP/GSNAP manual:
 
 <http://research-pub.gene.com/gmap/src/README>
 """
 
 import os.path as op
 import sys
-import logging
 
-from jcvi.formats.sam import get_prefix
-from jcvi.apps.base import (
-    OptionParser,
+from ..formats.sam import get_prefix
+
+from .base import (
     ActionDispatcher,
+    OptionParser,
+    backup,
+    logger,
     need_update,
     sh,
-    backup,
 )
 
 
 def main():
 
     actions = (
         ("index", "wraps gmap_build"),
@@ -94,30 +95,30 @@
     if not go:
         return dbdir, dbname
 
     if need_update(dbfile, safile):
         cmd = "gmap_build -D {0} -d {1} {2}".format(dbdir, dbname, filename)
         sh(cmd)
     else:
-        logging.error("`{0}` exists. `gmap_build` already run.".format(safile))
+        logger.error("`{0}` exists. `gmap_build` already run.".format(safile))
 
     if go and supercat and updated:
         sh("mv {0} {1}".format(coordsbak, coordsfile))
 
     return dbdir, dbname
 
 
 def index(args):
     """
         %prog index database.fasta
     `
         Wrapper for `gmap_build`. Same interface.
     """
     p = OptionParser(index.__doc__)
-    p.add_option(
+    p.add_argument(
         "--supercat",
         default=False,
         action="store_true",
         help="Concatenate reference to speed up alignment",
     )
     opts, args = p.parse_args(args)
 
@@ -131,21 +132,21 @@
 def gmap(args):
     """
     %prog gmap database.fasta fastafile
 
     Wrapper for `gmap`.
     """
     p = OptionParser(gmap.__doc__)
-    p.add_option(
+    p.add_argument(
         "--cross", default=False, action="store_true", help="Cross-species alignment"
     )
-    p.add_option(
+    p.add_argument(
         "--npaths",
         default=0,
-        type="int",
+        type=int,
         help="Maximum number of paths to show."
         " If set to 0, prints two paths if chimera"
         " detected, else one.",
     )
     p.set_cpus()
     opts, args = p.parse_args(args)
 
@@ -155,15 +156,15 @@
     dbfile, fastafile = args
     assert op.exists(dbfile) and op.exists(fastafile)
     prefix = get_prefix(fastafile, dbfile)
     logfile = prefix + ".log"
     gmapfile = prefix + ".gmap.gff3"
 
     if not need_update((dbfile, fastafile), gmapfile):
-        logging.error("`{0}` exists. `gmap` already run.".format(gmapfile))
+        logger.error("`{0}` exists. `gmap` already run.".format(gmapfile))
     else:
         dbdir, dbname = check_index(dbfile)
         cmd = "gmap -D {0} -d {1}".format(dbdir, dbname)
         cmd += " -f 2 --intronlength=100000"  # Output format 2
         cmd += " -t {0}".format(opts.cpus)
         cmd += " --npaths {0}".format(opts.npaths)
         if opts.cross:
@@ -181,48 +182,48 @@
 
     Wrapper for `gsnap` single-end or paired-end, depending on the number of
     args.
     """
     from jcvi.formats.fastq import guessoffset
 
     p = OptionParser(align.__doc__)
-    p.add_option(
+    p.add_argument(
         "--rnaseq",
         default=False,
         action="store_true",
         help="Input is RNA-seq reads, turn splicing on",
     )
-    p.add_option(
+    p.add_argument(
         "--native",
         default=False,
         action="store_true",
         help="Convert GSNAP output to NATIVE format",
     )
     p.set_home("eddyyeh")
     p.set_outdir()
     p.set_cpus()
     opts, args = p.parse_args(args)
 
     if len(args) == 2:
-        logging.debug("Single-end alignment")
+        logger.debug("Single-end alignment")
     elif len(args) == 3:
-        logging.debug("Paired-end alignment")
+        logger.debug("Paired-end alignment")
     else:
         sys.exit(not p.print_help())
 
     dbfile, readfile = args[:2]
     outdir = opts.outdir
     assert op.exists(dbfile) and op.exists(readfile)
     prefix = get_prefix(readfile, dbfile)
     logfile = op.join(outdir, prefix + ".log")
     gsnapfile = op.join(outdir, prefix + ".gsnap")
     nativefile = gsnapfile.rsplit(".", 1)[0] + ".unique.native"
 
     if not need_update((dbfile, readfile), gsnapfile):
-        logging.error("`{0}` exists. `gsnap` already run.".format(gsnapfile))
+        logger.error("`{0}` exists. `gsnap` already run.".format(gsnapfile))
     else:
         dbdir, dbname = check_index(dbfile)
         cmd = "gsnap -D {0} -d {1}".format(dbdir, dbname)
         cmd += " -B 5 -m 0.1 -i 2 -n 3"  # memory, mismatch, indel penalty, nhits
         if opts.rnaseq:
             cmd += " -N 1"
         cmd += " -t {0}".format(opts.cpus)
```

### Comparing `jcvi-1.4.6/jcvi/apps/grid.py` & `jcvi-1.4.7/jcvi/apps/grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 """
 Codes to submit multiple jobs to JCVI grid engine
 """
 
 import os.path as op
 import sys
 import re
-import logging
 import platform
 
 from multiprocessing import (
     Pool,
     Process,
     Value,
     cpu_count,
     get_context,
     set_start_method,
 )
 from multiprocessing.queues import Queue
 
-from jcvi.formats.base import write_file, must_open
-from jcvi.apps.base import (
-    OptionParser,
+from ..formats.base import write_file, must_open
+
+from .base import (
     ActionDispatcher,
-    popen,
+    OptionParser,
     backup,
+    listify,
+    logger,
     mkdir,
+    popen,
     sh,
-    listify,
 )
 
 
 class SharedCounter(object):
     """A synchronized shared counter.
 
     The locking done by multiprocessing.Value ensures that only a single
@@ -162,15 +163,15 @@
             backup(filename)
         fw = open(filename, "w")
         print("all : {0}\n".format(" ".join(sorted(self.targets))), file=fw)
         for d in self:
             print(d, file=fw)
         print("clean :\n\trm -rf {0}\n".format(" ".join(self.targets)), file=fw)
         fw.close()
-        logging.debug("Makefile written to `{0}`.".format(self.makefile))
+        logger.debug("Makefile written to `{0}`.".format(self.makefile))
 
     def run(self, cpus=1):
         if not op.exists(self.makefile):
             self.write()
         cmd = "make -j {0} -f {1}".format(cpus, self.makefile)
         sh(cmd)
 
@@ -250,15 +251,15 @@
 
 
 def write(queue_in, queue_out, filename, cpus):
     from rich.progress import Progress
 
     fw = must_open(filename, "w")
     isize = queue_in.qsize()
-    logging.debug("A total of {0} items to compute.".format(isize))
+    logger.debug("A total of {0} items to compute.".format(isize))
     isize = isize or 1
     poisons = 0
     with Progress() as progress:
         task = progress.add_task("[green]Processing ...", total=isize)
         while True:
             res = queue_out.get()
             qsize = queue_in.qsize()
@@ -398,15 +399,15 @@
         if self.outfile:
             backup(self.outfile)
             msg += " > {0} ".format(self.outfile)
         if self.errfile:
             backup(self.errfile)
             msg += " 2> {0} ".format(self.errfile)
 
-        logging.debug(msg)
+        logger.debug(msg)
 
 
 class Grid(list):
     def __init__(self, cmds, outfiles=[]):
 
         assert cmds, "Commands empty!"
         if not outfiles:
@@ -614,15 +615,15 @@
     import shlex
     from jcvi.apps.base import sh, getusername
     from subprocess import check_output, CalledProcessError
     import xml.etree.ElementTree as ET
 
     valid_methods = ("pattern", "jobid")
     p = OptionParser(kill.__doc__)
-    p.add_option(
+    p.add_argument(
         "--method",
         choices=valid_methods,
         help="Identify jobs based on [default: guess]",
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
@@ -643,15 +644,15 @@
         valid_jobids |= set(jobids)
     elif method == "pattern":
         qsxmlcmd = 'qstat -u "{}" -j "{}" -nenv -njd -xml'.format(username, tag)
         try:
             qsxml = check_output(shlex.split(qsxmlcmd)).strip()
         except CalledProcessError as e:
             qsxml = None
-            logging.debug(f'No jobs matching the pattern "{tag}": {e}')
+            logger.debug(f'No jobs matching the pattern "{tag}": {e}')
 
         if qsxml is not None:
             for job in ET.fromstring(qsxml).findall("djob_info"):
                 for elem in job.findall("element"):
                     jobid = elem.find("JB_job_number").text
                     valid_jobids.add(jobid)
```

### Comparing `jcvi-1.4.6/jcvi/apps/lastz.py` & `jcvi-1.4.7/jcvi/apps/lastz.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 import os.path as op
 import sys
-import logging
 
 from math import exp
 from multiprocessing import Lock, Pool
 
-from jcvi.formats.base import must_open
-from jcvi.apps.grid import Jobs
-from jcvi.apps.base import OptionParser, mkdir, Popen
+from ..formats.base import must_open
+
+from .grid import Jobs
+from .base import OptionParser, Popen, logger, mkdir
 
 
 # LASTZ options
 Darkspace = "nameparse=darkspace"
 Unmask = "unmask"
 Multiple = "multiple"
 Subsample = "subsample={0}/{1}"
@@ -126,19 +126,19 @@
     if extra:
         lastz_cmd += " " + extra.strip()
 
     lastz_cmd += " --format={0}".format(format)
     proc = Popen(lastz_cmd)
     out_fh = open(outfile, "w")
 
-    logging.debug("job <%d> started: %s" % (proc.pid, lastz_cmd))
+    logger.debug("job <%d> started: %s" % (proc.pid, lastz_cmd))
     for row in proc.stdout:
         out_fh.write(row)
         out_fh.flush()
-    logging.debug("job <%d> finished" % proc.pid)
+    logger.debug("job <%d> finished" % proc.pid)
 
 
 def lastz(k, n, bfasta_fn, afasta_fn, out_fh, lock, lastz_bin, extra, mask=False):
 
     ref_tags = [Multiple, Darkspace]
     qry_tags = [Darkspace]
     if n != 1:
@@ -155,22 +155,22 @@
     lastz_cmd += " --format=general-:%s" % lastz_fields
     # The above conversion is no longer necessary after LASTZ v1.02.40
     # (of which I contributed a patch)
     # lastz_cmd += " --format=BLASTN-"
 
     proc = Popen(lastz_cmd)
 
-    logging.debug("job <%d> started: %s" % (proc.pid, lastz_cmd))
+    logger.debug("job <%d> started: %s" % (proc.pid, lastz_cmd))
     for row in proc.stdout:
         row = lastz_to_blast(row)
         lock.acquire()
         print(row, file=out_fh)
         out_fh.flush()
         lock.release()
-    logging.debug("job <%d> finished" % proc.pid)
+    logger.debug("job <%d> finished" % proc.pid)
 
 
 def main():
     """
     %prog database.fa query.fa [options]
 
     Run LASTZ similar to the BLAST interface, and generates -m8 tabular format
@@ -179,29 +179,29 @@
 
     supported_formats = tuple(
         x.strip()
         for x in "lav, lav+text, axt, axt+, maf, maf+, maf-, sam, softsam, "
         "sam-, softsam-, cigar, BLASTN, BLASTN-, differences, rdotplot, text".split(",")
     )
 
-    p.add_option(
+    p.add_argument(
         "--format",
         default="BLASTN-",
         choices=supported_formats,
         help="Ooutput format",
     )
-    p.add_option("--path", dest="lastz_path", default=None, help="specify LASTZ path")
-    p.add_option(
+    p.add_argument("--path", dest="lastz_path", default=None, help="specify LASTZ path")
+    p.add_argument(
         "--mask",
         dest="mask",
         default=False,
         action="store_true",
         help="treat lower-case letters as mask info",
     )
-    p.add_option(
+    p.add_argument(
         "--similar",
         default=False,
         action="store_true",
         help="Use options tuned for close comparison",
     )
     p.set_cpus(cpus=32)
     p.set_params()
@@ -224,15 +224,15 @@
         extra += similarOptions
 
     lastz_bin = opts.lastz_path or "lastz"
     assert lastz_bin.endswith("lastz"), "You need to include lastz in your path"
 
     mask = opts.mask
     cpus = opts.cpus
-    logging.debug("Dispatch job to %d cpus" % cpus)
+    logger.debug("Dispatch job to %d cpus" % cpus)
     format = opts.format
     blastline = format == "BLASTN-"
 
     # The axt, maf, etc. format can only be run on splitted database (i.e. one
     # FASTA record per file). The splitted files are then parallelized for the
     # computation, as opposed to splitting queries through "subsample".
     outdir = "outdir"
```

### Comparing `jcvi-1.4.6/jcvi/apps/mask.py` & `jcvi-1.4.7/jcvi/apps/mask.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 
 """
 Mask low complexity regions in the genome.
 """
 import os.path as op
 import sys
 
-from jcvi.formats.fasta import Fasta
-from jcvi.utils.cbook import depends, percentage
-from jcvi.apps.base import OptionParser, ActionDispatcher, sh
+from ..formats.fasta import Fasta
+from ..utils.cbook import depends, percentage
+
+from .base import ActionDispatcher, OptionParser, sh
 
 
 @depends
 def wm_mk_counts(infile=None, outfile=None):
     cmd = "windowmasker -in {0} -mk_counts".format(infile)
     cmd += " -out {0}".format(outfile)
     sh(cmd)
@@ -92,15 +93,15 @@
     %prog mask fastafile
 
     This script pipelines the windowmasker in NCBI BLAST+.  Masked fasta file
     will have an appended suffix of .mask with all the low-complexity bases masked
     (default to lower case, set --hard for hardmasking).
     """
     p = OptionParser(mask.__doc__)
-    p.add_option(
+    p.add_argument(
         "--hard",
         dest="hard",
         default=False,
         action="store_true",
         help="Hard mask the low-complexity bases",
     )
     opts, args = p.parse_args(args)
```

### Comparing `jcvi-1.4.6/jcvi/apps/phylo.py` & `jcvi-1.4.7/jcvi/apps/phylo.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 - TreeFix
 
 The external software needs be installed first.
 """
 import sys
 import os
 import os.path as op
-import logging
 import re
 import warnings
 
 from math import ceil
 from itertools import chain
 from functools import partial
 
@@ -41,26 +40,27 @@
     FSeqBootCommandline,
     FDNADistCommandline,
     FNeighborCommandline,
     FConsenseCommandline,
 )
 from Bio.Phylo.Applications import PhymlCommandline, RaxmlCommandline
 
-from jcvi.apps.ks import (
+from ..compara.ks import (
     AbstractCommandline,
     find_first_isoform,
     run_mrtrans,
     clustal_align_protein,
     muscle_align_protein,
 )
-from jcvi.formats.base import must_open, DictFile, LineFile
-from jcvi.formats.fasta import Fasta
-from jcvi.utils.orderedcollections import OrderedDict
-from jcvi.graphics.base import plt, savefig
-from jcvi.apps.base import OptionParser, ActionDispatcher, mkdir, sh, getpath
+from ..formats.base import must_open, DictFile, LineFile
+from ..formats.fasta import Fasta
+from ..utils.orderedcollections import OrderedDict
+from ..graphics.base import plt, savefig
+
+from .base import ActionDispatcher, OptionParser, getpath, logger, mkdir, sh
 
 
 GBLOCKS_BIN = partial(getpath, name="GBLOCKS", warn="warn")
 PHYML_BIN = partial(getpath, name="PHYML", warn="warn")
 RAXML_BIN = partial(getpath, name="RAXML", warn="warn")
 FPHYLIP_BIN = partial(getpath, name="FPHYLIP", warn="warn")
 TREEFIX_BIN = partial(getpath, name="TREEFIX", warn="warn")
@@ -193,15 +193,15 @@
     print("TreeFix:", cl, file=sys.stderr)
     r, e = cl.run()
 
     if e:
         print("***TreeFix could not run", file=sys.stderr)
         return None
     else:
-        logging.debug("new tree written to {0}".format(outtreefile))
+        logger.debug("new tree written to {0}".format(outtreefile))
         return outtreefile
 
 
 def run_gblocks(align_fasta_file, **kwargs):
     """
     remove poorly aligned positions and divergent regions with Gblocks
     """
@@ -276,15 +276,15 @@
         tree.set_outgroup(tree.get_common_ancestor(*outgroup))
     except ValueError:
         assert type(outgroup) == list
         outgroup = outgroup[0]
         tree.set_outgroup(outgroup)
     tree.write(outfile=outfile, format=format)
 
-    logging.debug("Rerooted tree printed to {0}".format(outfile))
+    logger.debug("Rerooted tree printed to {0}".format(outfile))
     return outfile
 
 
 def build_nj_phylip(alignment, outfile, outgroup, work_dir="."):
     """
     build neighbor joining tree of DNA seqs with PHYLIP in EMBOSS
 
@@ -308,52 +308,52 @@
         sequence=phy_file,
         outfile=seqboot_out,
         seqtype="d",
         reps=100,
         seed=12345,
     )
     stdout, stderr = seqboot_cl()
-    logging.debug("Resampling alignment: %s" % seqboot_cl)
+    logger.debug("Resampling alignment: %s" % seqboot_cl)
 
     dnadist_out = phy_file.rsplit(".", 1)[0] + ".fdnadist"
     dnadist_cl = FDNADistCommandline(
         FPHYLIP_BIN("fdnadist"), sequence=seqboot_out, outfile=dnadist_out, method="f"
     )
     stdout, stderr = dnadist_cl()
-    logging.debug("Calculating distance for bootstrapped alignments: %s" % dnadist_cl)
+    logger.debug("Calculating distance for bootstrapped alignments: %s" % dnadist_cl)
 
     neighbor_out = phy_file.rsplit(".", 1)[0] + ".njtree"
     e = phy_file.rsplit(".", 1)[0] + ".fneighbor"
     neighbor_cl = FNeighborCommandline(
         FPHYLIP_BIN("fneighbor"),
         datafile=dnadist_out,
         outfile=e,
         outtreefile=neighbor_out,
     )
     stdout, stderr = neighbor_cl()
-    logging.debug("Building Neighbor Joining tree: %s" % neighbor_cl)
+    logger.debug("Building Neighbor Joining tree: %s" % neighbor_cl)
 
     consense_out = phy_file.rsplit(".", 1)[0] + ".consensustree.nodesupport"
     e = phy_file.rsplit(".", 1)[0] + ".fconsense"
     consense_cl = FConsenseCommandline(
         FPHYLIP_BIN("fconsense"),
         intreefile=neighbor_out,
         outfile=e,
         outtreefile=consense_out,
     )
     stdout, stderr = consense_cl()
-    logging.debug("Building consensus tree: %s" % consense_cl)
+    logger.debug("Building consensus tree: %s" % consense_cl)
 
     # distance without bootstrapping
     dnadist_out0 = phy_file.rsplit(".", 1)[0] + ".fdnadist0"
     dnadist_cl0 = FDNADistCommandline(
         FPHYLIP_BIN("fdnadist"), sequence=phy_file, outfile=dnadist_out0, method="f"
     )
     stdout, stderr = dnadist_cl0()
-    logging.debug("Calculating distance for original alignment: %s" % dnadist_cl0)
+    logger.debug("Calculating distance for original alignment: %s" % dnadist_cl0)
 
     # infer branch length on consensus tree
     consensustree1 = phy_file.rsplit(".", 1)[0] + ".consensustree.branchlength"
     run_ffitch(
         distfile=dnadist_out0, outtreefile=consensustree1, intreefile=consense_out
     )
 
@@ -381,39 +381,39 @@
     ct_b.write(format=0, outfile=outfile)
 
     try:
         s = op.getsize(outfile)
     except OSError:
         s = 0
     if s:
-        logging.debug("NJ tree printed to %s" % outfile)
+        logger.debug("NJ tree printed to %s" % outfile)
         return outfile, phy_file
     else:
-        logging.debug("Something was wrong. NJ tree was not built.")
+        logger.debug("Something was wrong. NJ tree was not built.")
         return None
 
 
 def build_ml_phyml(alignment, outfile, work_dir=".", **kwargs):
     """
     build maximum likelihood tree of DNA seqs with PhyML
     """
     phy_file = op.join(work_dir, "work", "aln.phy")
     AlignIO.write(alignment, open(phy_file, "w"), "phylip-relaxed")
 
     phyml_cl = PhymlCommandline(cmd=PHYML_BIN("phyml"), input=phy_file, **kwargs)
-    logging.debug("Building ML tree using PhyML: %s" % phyml_cl)
+    logger.debug("Building ML tree using PhyML: %s" % phyml_cl)
     stdout, stderr = phyml_cl()
 
     tree_file = phy_file + "_phyml_tree.txt"
     if not op.exists(tree_file):
         print("***PhyML failed.", file=sys.stderr)
         return None
     sh("cp {0} {1}".format(tree_file, outfile), log=False)
 
-    logging.debug("ML tree printed to %s" % outfile)
+    logger.debug("ML tree printed to %s" % outfile)
 
     return outfile, phy_file
 
 
 def build_ml_raxml(alignment, outfile, work_dir=".", **kwargs):
     """
     build maximum likelihood tree of DNA seqs with RAxML
@@ -434,25 +434,25 @@
         rapid_bootstrap_seed=12345,
         num_replicates=100,
         name="aln",
         working_dir=raxml_work,
         **kwargs
     )
 
-    logging.debug("Building ML tree using RAxML: %s" % raxml_cl)
+    logger.debug("Building ML tree using RAxML: %s" % raxml_cl)
     stdout, stderr = raxml_cl()
 
     tree_file = "{0}/RAxML_bipartitions.aln".format(raxml_work)
     if not op.exists(tree_file):
         print("***RAxML failed.", file=sys.stderr)
         sh("rm -rf %s" % raxml_work, log=False)
         return None
     sh("cp {0} {1}".format(tree_file, outfile), log=False)
 
-    logging.debug("ML tree printed to %s" % outfile)
+    logger.debug("ML tree printed to %s" % outfile)
     sh("rm -rf %s" % raxml_work)
 
     return outfile, phy_file
 
 
 def SH_raxml(reftree, querytree, phy_file, shout="SH_out.txt"):
     """
@@ -472,25 +472,25 @@
         model="GTRGAMMA",
         name="SH",
         starting_tree=reftree,
         bipartition_filename=querytree,
         working_dir=raxml_work,
     )
 
-    logging.debug("Running SH test in RAxML: %s" % raxml_cl)
+    logger.debug("Running SH test in RAxML: %s" % raxml_cl)
     o, stderr = raxml_cl()
     # hard coded
     try:
         pval = re.search("(Significantly.*:.*)", o).group(0)
     except:
         print("SH test failed.", file=sys.stderr)
     else:
         pval = pval.strip().replace("\t", " ").replace("%", "\%")
         print("{0}\t{1}".format(op.basename(querytree), pval), file=shout)
-        logging.debug("SH p-value appended to %s" % shout.name)
+        logger.debug("SH p-value appended to %s" % shout.name)
 
     shout.close()
     return shout.name
 
 
 CODON_TRANSLATION = CodonTable.standard_dna_table.forward_table
 FOURFOLD = {
@@ -657,19 +657,19 @@
                 newanchors.append(a)
                 seen.add(a)
         print("\t".join(newanchors), file=fw)
 
     fw.close()
     newmcscanfile = merge_rows_local(fw.name)
 
-    logging.debug(
+    logger.debug(
         "Tandems added to `{0}`. Results in `{1}`".format(mcscanfile, newmcscanfile)
     )
     fp.seek(0)
-    logging.debug(
+    logger.debug(
         "{0} rows merged to {1} rows".format(
             len(fp.readlines()), len(open(newmcscanfile).readlines())
         )
     )
     sh("rm %s" % fw.name)
 
     return newmcscanfile
@@ -697,16 +697,16 @@
     Use --addtandem=tandemfile to collapse tandems of anchors into single row.
     The tandemfile must be provided with *ALL* genomes involved, otherwise
     result will be incomplete and redundant.
     """
     from jcvi.graphics.base import discrete_rainbow
 
     p = OptionParser(prepare.__doc__)
-    p.add_option("--addtandem", help="path to tandemfile")
-    p.add_option(
+    p.add_argument("--addtandem", help="path to tandemfile")
+    p.add_argument(
         "--writecolors",
         default=False,
         action="store_true",
         help="generate a gene_name to color mapping file which will be taken "
         "by jcvi.apps.phylo.draw",
     )
     p.set_outdir(outdir="sequences")
@@ -777,17 +777,17 @@
             arec = f[a]
             SeqIO.write(arec, fw, "fasta")
         fw.close()
         n += 1
 
     if opts.writecolors:
         fc.close()
-        logging.debug("leaf colors written to `{0}`".format(fc.name))
+        logger.debug("leaf colors written to `{0}`".format(fc.name))
 
-    logging.debug("cds of {0} syntelog groups written to {1}/".format(n, seqdir))
+    logger.debug("cds of {0} syntelog groups written to {1}/".format(n, seqdir))
 
     return seqdir
 
 
 def build(args):
     """
     %prog build [prot.fasta] cds.fasta [options] --outdir=outdir
@@ -815,61 +815,61 @@
     is the recommended way to get highly customized trees.
 
     Newick format trees will be deposited into outdir (. by default).
     """
     from jcvi.formats.fasta import translate
 
     p = OptionParser(build.__doc__)
-    p.add_option(
+    p.add_argument(
         "--longest",
         action="store_true",
         help="Get longest ORF, only works if no pep file, e.g. ESTs",
     )
-    p.add_option(
+    p.add_argument(
         "--nogblocks",
         action="store_true",
         help="don't use Gblocks to edit alignment",
     )
-    p.add_option(
+    p.add_argument(
         "--synonymous",
         action="store_true",
         help="extract synonymous sites of the alignment",
     )
-    p.add_option(
+    p.add_argument(
         "--fourfold",
         action="store_true",
         help="extract fourfold degenerate sites of the alignment",
     )
-    p.add_option(
+    p.add_argument(
         "--msa",
         default="muscle",
         choices=("clustalw", "muscle"),
         help="software used to align the proteins",
     )
-    p.add_option(
+    p.add_argument(
         "--noneighbor",
         action="store_true",
         help="don't build NJ tree",
     )
-    p.add_option(
+    p.add_argument(
         "--ml",
         default=None,
         choices=("raxml", "phyml"),
         help="software used to build ML tree",
     )
-    p.add_option("--outgroup", help="path to file containing outgroup orders")
-    p.add_option("--SH", help="path to reference Newick tree")
-    p.add_option("--shout", default="SH_out.txt", help="SH output file name")
-    p.add_option(
+    p.add_argument("--outgroup", help="path to file containing outgroup orders")
+    p.add_argument("--SH", help="path to reference Newick tree")
+    p.add_argument("--shout", default="SH_out.txt", help="SH output file name")
+    p.add_argument(
         "--treefix",
         action="store_true",
         help="use TreeFix to rearrange ML tree",
     )
-    p.add_option("--stree", help="path to species Newick tree")
-    p.add_option(
+    p.add_argument("--stree", help="path to species Newick tree")
+    p.add_argument(
         "--smap",
         help="path to smap file: gene_name_pattern<tab>species_name",
     )
     p.set_outdir()
 
     opts, args = p.parse_args(args)
     gblocks = not opts.nogblocks
@@ -911,15 +911,15 @@
     elif opts.msa == "muscle":
         align_fasta = muscle_align_protein(p_recs, work_dir)
 
     n_recs = list(SeqIO.parse(open(dna_file), "fasta"))
     mrtrans_fasta = run_mrtrans(align_fasta, n_recs, work_dir, outfmt="fasta")
 
     if not mrtrans_fasta:
-        logging.debug("pal2nal aborted. Cannot reliably build tree for %s", dna_file)
+        logger.debug("pal2nal aborted. Cannot reliably build tree for %s", dna_file)
         return
 
     codon_aln_fasta = mrtrans_fasta
     if gblocks:
         gb_fasta = run_gblocks(mrtrans_fasta)
         codon_aln_fasta = gb_fasta if gb_fasta else codon_aln_fasta
 
@@ -1081,54 +1081,54 @@
     This function wraps on jcvi.graphics.tree
     This function is better used for trees generated by jcvi.apps.phylo (rooted
     if possible). For drawing general Newick trees from external sources invoke
     jcvi.graphics.tree directly, which also gives more drawing options.
     """
     trunc_name_options = ["headn", "oheadn", "tailn", "otailn"]
     p = OptionParser(draw.__doc__)
-    p.add_option(
+    p.add_argument(
         "--input",
         help="path to single input tree file or a dir "
         "containing ONLY the input tree files",
     )
-    p.add_option(
+    p.add_argument(
         "--combine",
-        type="string",
+        type=str,
         default="1x1",
         help="combine multiple trees into one plot in nrowxncol",
     )
-    p.add_option(
+    p.add_argument(
         "--trunc_name",
         default=None,
         help="Options are: {0}. "
         "truncate first n chars, retains only first n chars, "
         "truncate last n chars, retain only last chars. "
         "n=1~99.".format(trunc_name_options),
     )
-    p.add_option(
+    p.add_argument(
         "--SH",
         default=None,
         help="path to a file containing SH test p-values in format:"
         "tree_file_name<tab>p-values "
         "This file can be generated with jcvi.apps.phylo build",
     )
-    p.add_option(
+    p.add_argument(
         "--scutoff",
         default=50,
-        type="int",
+        type=int,
         help="cutoff for displaying node support, 0-100",
     )
-    p.add_option(
+    p.add_argument(
         "--barcode",
         default=None,
         help="path to seq/taxon name barcode mapping file: "
         "barcode<tab>new_name "
         "This option is downstream of `--trunc_name`",
     )
-    p.add_option(
+    p.add_argument(
         "--leafcolorfile",
         default=None,
         help="path to a mapping file containing font colors "
         "for the OTUs: leafname<tab>color",
     )
     p.set_outdir()
     opts, args, iopts = p.set_image_options(figsize="8x6")
@@ -1178,15 +1178,15 @@
                         tree = ""
                         i += 1
                 else:
                     tree += t
         else:
             tree += row
 
-    logging.debug("A total of {0} trees imported.".format(len(trees)))
+    logger.debug("A total of {0} trees imported.".format(len(trees)))
     sh("rm {0}".format(op.join(outdir, "alltrees.dnd")))
 
     _draw_trees(
         trees,
         nrow=int(combine[0]),
         ncol=int(combine[1]),
         rmargin=0.3,
```

### Comparing `jcvi-1.4.6/jcvi/apps/r.py` & `jcvi-1.4.7/jcvi/apps/r.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """
 uses R for statistics and graphics
 """
 
-import os.path as op
-import os
 import sys
 
 from string import Template
 
-from jcvi.formats.base import must_open
-from jcvi.apps.base import OptionParser, ActionDispatcher, cleanup, sh
+from ..formats.base import must_open
+
+from .base import ActionDispatcher, OptionParser, cleanup, sh
 
 
 class RTemplate(object):
     """
     Creates a R script and runs it
     """
```

### Comparing `jcvi-1.4.6/jcvi/apps/restriction.py` & `jcvi-1.4.7/jcvi/apps/restriction.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 """
 Procedure to cut genome using restriction enzymes.
 """
 import sys
-import logging
 
 from Bio.Restriction.Restriction import AllEnzymes, Analysis
 
-from jcvi.formats.fasta import Fasta, SeqRecord, SeqIO
-from jcvi.formats.base import must_open
-from jcvi.apps.base import OptionParser, ActionDispatcher
+from ..formats.base import must_open
+from ..formats.fasta import Fasta, SeqRecord, SeqIO
+
+from .base import ActionDispatcher, OptionParser, logger
 
 
 def main():
 
     actions = (
         ("fragment", "extract upstream and downstream seq of particular RE"),
         ("digest", "digest FASTA file to map restriction site positions"),
@@ -121,21 +121,21 @@
     ~~~====|=============|==========~~~~~~~===|============
            (---)     (---)
 
     In this case, the second fragment is longer than 800bp, therefore the two
     ends are NOT extracted, as in the first fragment.
     """
     p = OptionParser(fragment.__doc__)
-    p.add_option(
+    p.add_argument(
         "--flank",
         default=150,
-        type="int",
+        type=int,
         help="Extract flanking bases of the cut sites",
     )
-    p.add_option(
+    p.add_argument(
         "--full",
         default=False,
         action="store_true",
         help="The full extraction mode",
     )
     opts, args = p.parse_args(args)
 
@@ -157,12 +157,12 @@
     f = Fasta(fastafile, lazy=True)
     fw = open(fragfastafile, "w")
     for name, rec in f.iteritems_ordered():
         a = Analysis([enzyme], rec.seq)
         sites = a.full()[enzyme]
         extract(rec, sites, flank, fw)
 
-    logging.debug("Fragments written to `{0}`.".format(fragfastafile))
+    logger.debug("Fragments written to `%s`.", fragfastafile)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `jcvi-1.4.6/jcvi/apps/softlink.py` & `jcvi-1.4.7/jcvi/apps/softlink.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 # -*- coding: UTF-8 -*-
 
 """
 Procedure to touch and copy softlinks
 """
 import os
 import os.path as op
-import logging
 import sys
 
-from jcvi.apps.base import OptionParser, ActionDispatcher, get_abs_path
+from .base import ActionDispatcher, OptionParser, get_abs_path, logger
 
 
 def main():
 
     actions = (
         ("touch", "touch all the symlinks"),
         ("cp", "cp all the symlinks to current folder"),
@@ -27,27 +26,27 @@
 
 def lnsf(source, target, log=False):
     # re-link the symlinks (similar to `ln -sf`)
     if op.lexists(target):
         os.unlink(target)
     os.symlink(source, target)
     if log:
-        logging.debug("{0} => {1}".format(source, target))
+        logger.debug("{0} => {1}".format(source, target))
 
 
 def link(args):
     """
     %prog link metafile
 
     Link source to target based on a tabular file.
     """
     from jcvi.apps.base import mkdir
 
     p = OptionParser(link.__doc__)
-    p.add_option("--dir", help="Place links in a subdirectory")
+    p.add_argument("--dir", help="Place links in a subdirectory")
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (meta,) = args
     d = opts.dir
@@ -94,15 +93,15 @@
     """
     p = OptionParser(clean.__doc__)
     opts, args = p.parse_args(args)
 
     for link_name in os.listdir(os.getcwd()):
         if not op.islink(link_name):
             continue
-        logging.debug("remove symlink `{0}`".format(link_name))
+        logger.debug("remove symlink `{0}`".format(link_name))
         os.unlink(link_name)
 
 
 def cp(args):
     """
     find folder -type l | %prog cp
 
@@ -116,15 +115,15 @@
         if not op.exists(link_name):
             continue
 
         source = get_abs_path(link_name)
         link_name = op.basename(link_name)
         if not op.exists(link_name):
             os.symlink(source, link_name)
-        logging.debug(" => ".join((source, link_name)))
+        logger.debug(" => ".join((source, link_name)))
 
 
 def size(args):
     """
     find folder -type l | %prog size
 
     Get the size for all the paths that are pointed by the links
```

### Comparing `jcvi-1.4.6/jcvi/apps/uclust.py` & `jcvi-1.4.7/jcvi/apps/uclust.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,40 +5,43 @@
 Using VCLUST to derep, cluster, and make consensus from duplicate reads.
 The VCLUST implementation borrows ideas and code from PyRAD. PyRAD link:
 
 <https://github.com/dereneaton/pyrad>
 """
 import os.path as op
 import sys
-import logging
-import numpy as np
-import scipy
-import scipy.stats
-import scipy.optimize
 
 from collections import defaultdict
 from copy import deepcopy
 from functools import partial
 from itertools import groupby
-from more_itertools import grouper
 from subprocess import Popen, PIPE, STDOUT
 from tempfile import mkdtemp
 
-from jcvi.formats.base import BaseFile, FileMerger, must_open, split
-from jcvi.formats.fasta import parse_fasta
-from jcvi.formats.fastq import fasta
-from jcvi.utils.orderedcollections import DefaultOrderedDict
-from jcvi.utils.table import write_csv
-from jcvi.apps.base import (
+import numpy as np
+import scipy
+import scipy.stats
+import scipy.optimize
+
+from more_itertools import grouper
+
+from ..formats.base import BaseFile, FileMerger, must_open, split
+from ..formats.fasta import parse_fasta
+from ..formats.fastq import fasta
+from ..utils.orderedcollections import DefaultOrderedDict
+from ..utils.table import write_csv
+
+from .base import (
     OptionParser,
     ActionDispatcher,
     cleanup,
     datadir,
     iglob,
     listify,
+    logger,
     mkdir,
     need_update,
     sh,
 )
 
 
 SEP = "//"
@@ -75,15 +78,15 @@
             for name, seq in grouper(contents, 2):
                 name, seq = name.strip(), seq.strip()
                 nrep = getsize(name)
                 data.append((name, seq, nrep))
             yield data
             nstacks += 1
             if nstacks % 10000 == 0:
-                logging.debug("{0} stacks parsed".format(nstacks))
+                logger.debug("{0} stacks parsed".format(nstacks))
 
 
 class Clust(list):
     def __init__(self):
         super(Clust, self).__init__(self)
 
     def __str__(self):
@@ -236,25 +239,25 @@
     contents.append(
         ("MEDIAN (per sample)", int(np.median(all_reads)), int(np.median(all_contigs)))
     )
     write_csv(header, contents, filename=opts.outfile)
 
 
 def add_consensus_options(p):
-    p.add_option("--prefix", default="mcluster", help="Output prefix")
-    p.add_option("--minlength", default=30, type="int", help="Min contig length")
-    p.add_option("--mindepth", default=3, type="int", help="Min depth for each stack")
-    p.add_option("--minsamp", default=3, type="int", help="Min number of samples")
+    p.add_argument("--prefix", default="mcluster", help="Output prefix")
+    p.add_argument("--minlength", default=30, type=int, help="Min contig length")
+    p.add_argument("--mindepth", default=3, type=int, help="Min depth for each stack")
+    p.add_argument("--minsamp", default=3, type=int, help="Min number of samples")
 
 
 def find_pctid(consensusfiles):
     pctid = min(
         [int(op.basename(x).split(".")[-2].replace("P", "")) for x in consensusfiles]
     )
-    logging.debug("Set pctid={0}".format(pctid))
+    logger.debug("Set pctid={0}".format(pctid))
     return pctid
 
 
 def mcluster(args):
     """
     %prog mcluster *.consensus
 
@@ -282,17 +285,17 @@
         for cf in consensusfiles:
             nseqs = 0
             s = op.basename(cf).split(".")[0]
             for name, seq in parse_fasta(cf):
                 name = ".".join((s, name))
                 print(">{0}\n{1}".format(name, seq), file=fw_cons)
                 nseqs += 1
-            logging.debug("Read `{0}`: {1} seqs".format(cf, nseqs))
+            logger.debug("Read `{0}`: {1} seqs".format(cf, nseqs))
             totalseqs += nseqs
-        logging.debug("Total: {0} seqs".format(totalseqs))
+        logger.debug("Total: {0} seqs".format(totalseqs))
         fw_cons.close()
 
     userfile = pf + ".u"
     notmatchedfile = pf + ".notmatched"
     if need_update(consensusfile, userfile):
         cluster_smallmem(
             consensusfile, userfile, notmatchedfile, minlength, pctid, cpus
@@ -407,16 +410,16 @@
 
         print(
             ">{0} with {1} sequences\n{2}".format(fname, sum(nreps), cons_seq),
             file=fw_finalfasta,
         )
         locid += 1
 
-    logging.debug("Stacks written to `{0}`".format(locifile))
-    logging.debug(
+    logger.debug("Stacks written to `{0}`".format(locifile))
+    logger.debug(
         "Final consensus sequences written to `{0}` (n={1})".format(
             finalfastafile, locid
         )
     )
     fw.close()
     fw_finalfasta.close()
 
@@ -426,15 +429,15 @@
 def mconsensus(args):
     """
     %prog mconsensus *.consensus
 
     Call consensus along the stacks from cross-sample clustering.
     """
     p = OptionParser(mconsensus.__doc__)
-    p.add_option(
+    p.add_argument(
         "--allele_counts",
         default="allele_counts",
         help="Directory to generate allele counts",
     )
     add_consensus_options(p)
     opts, args = p.parse_args(args)
 
@@ -459,36 +462,36 @@
     # Sort allele counts into separate files
     for ac in AC:
         chrpos = ac.chr, ac.pos
         seen[chrpos].append(ac)
         print(ac.tostring(taxon=True), file=fw)
     fw.close()
 
-    logging.debug("Populate all taxa and instantiate empty vector if missing")
+    logger.debug("Populate all taxa and instantiate empty vector if missing")
     all_taxa = set([op.basename(x).split(".")[0] for x in consensusfiles])
     taxon_to_ac = defaultdict(list)
     for chrpos, aclist in seen.items():
         included_taxa = set([x.taxon for x in aclist])
         missing_taxa = all_taxa - included_taxa
         template = deepcopy(aclist[0])
         template.clear()
         for ac in aclist:
             taxon_to_ac[ac.taxon].append(ac)
         for tx in missing_taxa:
             taxon_to_ac[tx].append(template)
 
-    logging.debug("Write allele counts for all taxa")
+    logger.debug("Write allele counts for all taxa")
     for tx, aclist in sorted(taxon_to_ac.items()):
         tx_acfile = op.join(acdir, tx + ".allele_counts")
         fw = open(tx_acfile, "w")
         print("# " + "\t".join(ACHEADER_NO_TAXON), file=fw)
         for ac in aclist:
             print(ac.tostring(), file=fw)
         fw.close()
-        logging.debug("Written {0} sites in `{1}`".format(len(aclist), tx_acfile))
+        logger.debug("Written {0} sites in `{1}`".format(len(aclist), tx_acfile))
 
 
 def get_seed(data):
     if len(data) == 1:
         return data[0]
 
     for name, seq, nrep in data[::-1]:
@@ -552,16 +555,16 @@
     """
     %prog consensus clustSfile
 
     Call consensus along the stacks. Tabulate bases at each site, tests for
     errors according to error rate, calls consensus.
     """
     p = OptionParser(consensus.__doc__)
-    p.add_option(
-        "--ploidy", default=2, type="int", help="Number of haplotypes per locus"
+    p.add_argument(
+        "--ploidy", default=2, type=int, help="Number of haplotypes per locus"
     )
     add_consensus_options(p)
     p.set_verbose()
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
@@ -584,15 +587,15 @@
         if total_nreps < mindepth:
             continue
 
         first_name, first_seq, first_nrep = data[0]
         fname = first_name.split(";")[0] + ";size={0};".format(total_nreps)
         cons_name, cons_seq, cons_nrep = get_seed(data)
         if len(data) > 1 and cons_name != CONSTAG:
-            logging.debug("Tag {0} not found in cluster {1}".format(CONSTAG, cons_name))
+            logger.debug("Tag {0} not found in cluster {1}".format(CONSTAG, cons_name))
 
         # List for sequence data
         S = [(seq, nrep) for name, seq, nrep in data if nrep]
         # Pileups for base counting
         RAD = stack(S)
 
         if len(data) == 1:  # No computation needed
@@ -628,30 +631,30 @@
         indices.append((fname, start, end))
 
     consensfile = pf + ".consensus"
     consens = open(consensfile, "w")
     for k, v in output:
         print("\n".join((k, v)), file=consens)
     consens.close()
-    logging.debug("Consensus sequences written to `{0}`".format(consensfile))
+    logger.debug("Consensus sequences written to `{0}`".format(consensfile))
 
     binfile = consensfile + ".bin"
     bins = np.array(bins, dtype=np.uint32)
     ulimit = 65535
     bins[bins > ulimit] = ulimit
     bins = np.array(bins, dtype=np.uint16)  # Compact size
     bins.tofile(binfile)
-    logging.debug("Allele counts written to `{0}`".format(binfile))
+    logger.debug("Allele counts written to `{0}`".format(binfile))
 
     idxfile = consensfile + ".idx"
     fw = open(idxfile, "w")
     for fname, start, end in indices:
         print("\t".join(str(x) for x in (fname, start, end)), file=fw)
     fw.close()
-    logging.debug("Serializing indices to `{0}`".format(idxfile))
+    logger.debug("Serializing indices to `{0}`".format(idxfile))
 
     return consensfile, binfile, idxfile
 
 
 def stack(S):
     """
     From list of bases at a site D,  make counts of bases
@@ -792,18 +795,18 @@
     if not need_update(clustSfile, HEfile, warn=True):
         return HEfile
 
     D = []
     for d in cons(clustSfile, opts.mindepth):
         D.extend(d)
 
-    logging.debug("Computing base frequencies ...")
+    logger.debug("Computing base frequencies ...")
     P = makeP(D)
     C = makeC(D)
-    logging.debug("Solving log-likelihood function ...")
+    logger.debug("Solving log-likelihood function ...")
     x0 = [0.01, 0.001]  # initital values
     H, E = scipy.optimize.fmin(LL, x0, args=(P, C))
 
     fw = must_open(HEfile, "w")
     print(H, E, file=fw)
     fw.close()
 
@@ -939,15 +942,15 @@
     header = "label total cnts mean std".split()
 
     bins = [0, 5, 10, 15, 20, 25, 30, 35, 40, 50, 100, 250, 500, 99999]
     ohist, edges = np.histogram(depth, bins)
     hist = [float(i) / sum(ohist) for i in ohist]
     hist = [int(round(i * 30)) for i in hist]
 
-    logging.debug("Sample {0} finished, {1} loci".format(clustSfile, len(depth)))
+    logger.debug("Sample {0} finished, {1} loci".format(clustSfile, len(depth)))
 
     fw = open(statsfile, "w")
     print("# Params: mindepth={0}".format(mindepth), file=fw)
     print(" ".join("{0}={1}".format(k, out[k]) for k in header), file=fw)
     print("\nbins\tdepth_histogram\tcnts", file=fw)
     print("   :\t0------------50-------------100%", file=fw)
```

### Comparing `jcvi-1.4.6/jcvi/apps/uniprot.py` & `jcvi-1.4.7/jcvi/apps/uniprot.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 """
 Programatically accessing UniprotKB to get data from a list of queries
 """
 import os.path as op
 import sys
 import time
-import logging
 
 from urllib.parse import urlencode
 from urllib.request import Request, urlopen
 from urllib.error import HTTPError, URLError
 
-from jcvi.formats.base import must_open
-from jcvi.apps.base import OptionParser, ActionDispatcher
+from ..formats.base import must_open
+
+from .base import ActionDispatcher, OptionParser, logger
 
 
 uniprot_url = "http://www.uniprot.org/uniprot/"
 
 valid_formats = [
     "html",
     "tab",
@@ -94,44 +94,44 @@
     to query any of the documented fields <http://www.uniprot.org/help/query-fields>
     """
     import re
     import csv
 
     p = OptionParser(fetch.__doc__)
 
-    p.add_option(
+    p.add_argument(
         "--format",
         default="tab",
         choices=valid_formats,
         help="download format",
     )
-    p.add_option(
+    p.add_argument(
         "--columns",
         default="entry name, protein names, genes,organism",
         help="columns to download, if --format is `tab` or `xls`",
     )
-    p.add_option(
+    p.add_argument(
         "--include",
         default=False,
         action="store_true",
         help="Include isoforms when --format is `fasta` or include `description` when --format is `rdf`.",
     )
-    p.add_option(
+    p.add_argument(
         "--limit",
         default=10,
-        type="int",
+        type=int,
         help="Max number of results to retrieve",
     )
-    p.add_option(
+    p.add_argument(
         "--offset",
         default=0,
-        type="int",
+        type=int,
         help="Offset of first result, used with --limit",
     )
-    p.add_option(
+    p.add_argument(
         "--skipcheck",
         default=False,
         action="store_true",
         help="Turn off prompt to check file existence",
     )
     opts, args = p.parse_args(args)
 
@@ -176,31 +176,31 @@
     fw = must_open(outfile, "w", checkexists=True, skipcheck=opts.skipcheck)
     if fw is None:
         return
 
     seen = set()
     for query in list_of_queries:
         if query in seen:
-            logging.error("Duplicate query ({0}) found".format(query))
+            logger.error("Duplicate query ({0}) found".format(query))
             continue
 
         url_params["query"] = query
 
         data = urlencode(url_params)
         try:
             request = Request(uniprot_url, data)
             response = urlopen(request)
         except (HTTPError, URLError, RuntimeError, KeyError) as e:
-            logging.error(e)
-            logging.debug("wait 5 seconds to reconnect...")
+            logger.error(e)
+            logger.debug("wait 5 seconds to reconnect...")
             time.sleep(5)
 
         page = response.read()
         if not page:
-            logging.error("query `{0}` yielded no results".format(query))
+            logger.error("query `{0}` yielded no results".format(query))
             continue
 
         print(page, file=fw)
 
         seen.add(query)
 
     if seen:
```

### Comparing `jcvi-1.4.6/jcvi/apps/vecscreen.py` & `jcvi-1.4.7/jcvi/apps/vecscreen.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 
 """
 Run through NCBI vecscreen on a local machine.
 """
 import os.path as op
 import sys
 
-from jcvi.utils.range import range_merge
-from jcvi.formats.fasta import tidy
-from jcvi.formats.blast import BlastLine
-from jcvi.formats.base import must_open
-from jcvi.apps.align import run_vecscreen, run_megablast
-from jcvi.apps.base import OptionParser, ActionDispatcher, download, sh
+from ..formats.base import must_open
+from ..formats.blast import BlastLine
+from ..formats.fasta import tidy
+from ..utils.range import range_merge
+
+from .align import run_vecscreen, run_megablast
+from .base import ActionDispatcher, OptionParser, download, sh
 
 ECOLI_URL = "ftp://ftp.ncbi.nlm.nih.gov/genomes/all/GCF/000/019/425/GCF_000019425.1_ASM1942v1/GCF_000019425.1_ASM1942v1_genomic.fna.gz"
 UNIVEC_URL = "ftp://ftp.ncbi.nih.gov/pub/UniVec/UniVec_Core"
 
 
 def main():
 
@@ -43,15 +44,15 @@
     %prog mask fastafile
 
     Mask the contaminants. By default, this will compare against UniVec_Core and
     Ecoli.fasta. Merge the contaminant results, and use `maskFastaFromBed`. Can
     perform FASTA tidy if requested.
     """
     p = OptionParser(mask.__doc__)
-    p.add_option(
+    p.add_argument(
         "--db",
         default=ECOLI_URL,
         help="Contaminant db other than Ecoli K12, will download if file starts with http://, https://, or ftp://",
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
@@ -86,21 +87,21 @@
     """
     %prog blast fastafile
 
     Run BLASTN against database (default is UniVec_Core).  Output .bed format
     on the vector/contaminant ranges.
     """
     p = OptionParser(blast.__doc__)
-    p.add_option(
+    p.add_argument(
         "--dist",
         default=100,
-        type="int",
+        type=int,
         help="Merge adjacent HSPs separated by",
     )
-    p.add_option("--db", help="Use a different database rather than UniVec_Core")
+    p.add_argument("--db", help="Use a different database rather than UniVec_Core")
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (fastafile,) = args
     fastaprefix = fastafile.split(".", 1)[0]
```

### Comparing `jcvi-1.4.6/jcvi/assembly/allmaps.py` & `jcvi-1.4.7/jcvi/assembly/allmaps.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,17 +25,16 @@
 from ..algorithms.lis import (
     longest_monotonic_subseq_length_loose as lms,
     longest_monotonic_subsequence_loose as lmseq,
 )
 from ..algorithms.matrix import determine_signs
 from ..apps.base import (
     ActionDispatcher,
-    OptionGroup,
     OptionParser,
-    SUPPRESS_HELP,
+    SUPPRESS,
     cleanup,
     flatten,
     get_today,
     logger,
     mkdir,
     need_update,
     sh,
@@ -1010,18 +1009,18 @@
     %prog split input.bed
 
     Split suspicious scaffolds. Suspicious scaffolds are those that contain
     chunks that map to more than one linkage group. The chunk size can be
     modified through --chunk option.
     """
     p = OptionParser(split.__doc__)
-    p.add_option(
-        "--chunk", default=4, type="int", help="Split chunks of at least N markers"
+    p.add_argument(
+        "--chunk", default=4, type=int, help="Split chunks of at least N markers"
     )
-    p.add_option(
+    p.add_argument(
         "--splitsingle",
         default=False,
         action="store_true",
         help="Split breakpoint range right in the middle",
     )
     opts, args = p.parse_args(args)
 
@@ -1058,18 +1057,18 @@
     Visualize history of scaffold OO. The history is contained within the
     tourfile, generated by path(). For each historical scaffold OO, the program
     plots a separate PDF file. The plots can be combined to show the progression
     as a little animation. The third argument limits the plotting to a
     specific pseudomolecule, for example `chr1`.
     """
     p = OptionParser(movie.__doc__)
-    p.add_option(
+    p.add_argument(
         "--gapsize",
         default=100,
-        type="int",
+        type=int,
         help="Insert gaps of size between scaffolds",
     )
     add_allmaps_plot_options(p)
     opts, args = p.parse_args(args)
 
     if len(args) != 3:
         sys.exit(not p.print_help())
@@ -1148,20 +1147,20 @@
     %prog estimategaps input.bed
 
     Estimate sizes of inter-scaffold gaps. The AGP file generated by path()
     command has unknown gap sizes with a generic number of Ns (often 100 Ns).
     The AGP file `input.chr.agp` will be modified in-place.
     """
     p = OptionParser(estimategaps.__doc__)
-    p.add_option("--minsize", default=100, type="int", help="Minimum gap size")
-    p.add_option("--maxsize", default=500000, type="int", help="Maximum gap size")
-    p.add_option(
+    p.add_argument("--minsize", default=100, type=int, help="Minimum gap size")
+    p.add_argument("--maxsize", default=500000, type=int, help="Maximum gap size")
+    p.add_argument(
         "--links",
         default=10,
-        type="int",
+        type=int,
         help="Only use linkage grounds with matchings more than",
     )
     p.set_verbose(help="Print details for each gap calculation")
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
@@ -1230,15 +1229,15 @@
 
     ScaffoldID,ScaffoldPosition,LinkageGroup,GeneticPosition
     scaffold_2707,11508,1,0
     scaffold_2707,11525,1,1.2
     scaffold_759,81336,1,9.7
     """
     p = OptionParser(merge.__doc__)
-    p.add_option(
+    p.add_argument(
         "-w", "--weightsfile", default="weights.txt", help="Write weights to file"
     )
     p.set_outfile("out.bed")
     opts, args = p.parse_args(args)
 
     if len(args) < 1:
         sys.exit(not p.print_help())
@@ -1271,15 +1270,15 @@
 def mergebed(args):
     """
     %prog mergebed map1.bed map2.bed map3.bed ...
 
     Combine bed maps to bed format, adding the map name.
     """
     p = OptionParser(mergebed.__doc__)
-    p.add_option(
+    p.add_argument(
         "-w", "--weightsfile", default="weights.txt", help="Write weights to file"
     )
     p.set_outfile("out.bed")
     opts, args = p.parse_args(args)
 
     if len(args) < 1:
         sys.exit(not p.print_help())
@@ -1354,80 +1353,79 @@
     considered the pivot map. The final output is an AGP file that contains
     ordered scaffolds.
 
     Please note that BED file and FASTA file cannot share the same prefix.
     """
     oargs = args
     p = OptionParser(path.__doc__)
-    p.add_option("-b", "--bedfile", help=SUPPRESS_HELP)
-    p.add_option("-s", "--fastafile", help=SUPPRESS_HELP)
-    p.add_option(
+    p.add_argument("-b", "--bedfile", help=SUPPRESS)
+    p.add_argument("-s", "--fastafile", help=SUPPRESS)
+    p.add_argument(
         "-w", "--weightsfile", default="weights.txt", help="Use weights from file"
     )
-    p.add_option(
+    p.add_argument(
         "--compress",
         default=1e-6,
-        type="float",
+        type=float,
         help="Compress markers with distance <=",
     )
-    p.add_option(
+    p.add_argument(
         "--noremoveoutliers",
         default=False,
         action="store_true",
         help="Don't remove outlier markers",
     )
-    p.add_option(
+    p.add_argument(
         "--distance",
         default="rank",
         choices=distance_choices,
         help="Distance function when building initial consensus",
     )
-    p.add_option(
+    p.add_argument(
         "--linkage",
         default="double",
         choices=linkage_choices,
         help="Linkage function when building initial consensus",
     )
-    p.add_option(
+    p.add_argument(
         "--gapsize",
         default=100,
-        type="int",
+        type=int,
         help="Insert gaps of size between scaffolds",
     )
-    p.add_option("--seqid", help="Only run partition with this seqid")
-    p.add_option("--partitions", help="Use predefined partitions of LGs")
-    p.add_option(
-        "--links", default=10, type="int", help="Only plot matchings more than"
+    p.add_argument("--seqid", help="Only run partition with this seqid")
+    p.add_argument("--partitions", help="Use predefined partitions of LGs")
+    p.add_argument(
+        "--links", default=10, type=int, help="Only plot matchings more than"
     )
-    p.add_option(
-        "--mincount", default=1, type="int", help="Minimum markers on a contig"
+    p.add_argument(
+        "--mincount", default=1, type=int, help="Minimum markers on a contig"
     )
-    p.add_option(
+    p.add_argument(
         "--noplot",
         default=False,
         action="store_true",
         help="Do not visualize the alignments",
     )
-    p.add_option(
+    p.add_argument(
         "--renumber",
         default=False,
         action="store_true",
         help="Renumber chromosome based on decreasing sizes",
     )
     p.set_cpus(cpus=16)
 
-    q = OptionGroup(p, "Genetic algorithm options")
-    p.add_option_group(q)
-    q.add_option(
-        "--ngen", default=500, type="int", help="Iterations in GA, higher ~ slower"
+    q = p.add_argument_group("Genetic algorithm options")
+    q.add_argument(
+        "--ngen", default=500, type=int, help="Iterations in GA, higher ~ slower"
     )
-    q.add_option(
-        "--npop", default=100, type="int", help="Population size in GA, higher ~ slower"
+    q.add_argument(
+        "--npop", default=100, type=int, help="Population size in GA, higher ~ slower"
     )
-    q.add_option("--seed", default=666, type="int", help="Random seed number")
+    q.add_argument("--seed", default=666, type=int, help="Random seed number")
     opts, args, iopts = p.set_image_options(args, figsize="10x6")
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     inputbed, fastafile = args
     inputbed = opts.bedfile or inputbed
@@ -1707,15 +1705,15 @@
 
     Build associated genome FASTA file and CHAIN file that can be used to lift
     old coordinates to new coordinates. The CHAIN file will be used to lift the
     original marker positions to new positions in the reconstructed genome. The
     new positions of the markers will be reported in *.lifted.bed.
     """
     p = OptionParser(build.__doc__)
-    p.add_option(
+    p.add_argument(
         "--cleanup",
         default=False,
         action="store_true",
         help="Clean up bulky FASTA files, useful for plotting",
     )
     opts, args = p.parse_args(args)
 
@@ -1770,27 +1768,27 @@
             "unmapped",
         )
 
     sort([liftedbed, "-i"])  # Sort bed in place
 
 
 def add_allmaps_plot_options(p):
-    p.add_option(
+    p.add_argument(
         "-w", "--weightsfile", default="weights.txt", help="Use weights from file"
     )
-    p.add_option(
+    p.add_argument(
         "--distance",
         default="cM",
         choices=distance_choices,
         help="Plot markers based on distance",
     )
-    p.add_option(
-        "--links", default=10, type="int", help="Only plot matchings more than"
+    p.add_argument(
+        "--links", default=10, type=int, help="Only plot matchings more than"
     )
-    p.add_option(
+    p.add_argument(
         "--panels", default=False, action="store_true", help="Add panel labels A/B"
     )
 
 
 def plot(args):
     """
     %prog plot input.bed seqid
@@ -1808,15 +1806,15 @@
         set2,
         panel_labels,
         shorten,
     )
     from ..graphics.chromosome import Chromosome, GeneticMap, HorizontalChromosome
 
     p = OptionParser(plot.__doc__)
-    p.add_option("--title", help="Title of the plot")
+    p.add_argument("--title", help="Title of the plot")
     add_allmaps_plot_options(p)
     opts, args, iopts = p.set_image_options(args, figsize="10x6")
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     inputbed, seqid = args
```

### Comparing `jcvi-1.4.6/jcvi/assembly/allpaths.py` & `jcvi-1.4.7/jcvi/assembly/allpaths.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 """
 Subroutines to aid ALLPATHS-LG assembly.
 """
 import os.path as op
-import os
 import sys
-import logging
-import numpy as np
 
 from struct import pack, unpack
 from itertools import islice
 
-from jcvi.formats.base import BaseFile
-from jcvi.assembly.base import FastqNamings, Library
-from jcvi.apps.grid import Jobs
-from jcvi.apps.base import (
-    OptionParser,
+import numpy as np
+
+from ..formats.base import BaseFile
+from ..apps.grid import Jobs
+from ..apps.base import (
     ActionDispatcher,
+    OptionParser,
     cleanup,
     glob,
+    logger,
     need_update,
     sh,
 )
 
+from .base import FastqNamings, Library
+
 
 class PairsFile(BaseFile):
     def __init__(self, filename):
         super(PairsFile, self).__init__(filename)
 
         fp = open(filename, "rb")
         (binwrite,) = unpack("8s", fp.read(8))
@@ -79,15 +80,15 @@
         s += "r1: {0}\n".format(self.r1)
         s += "r2: {0}\n".format(self.r2)
         s += "libs: {0}".format(self.libs)
         return s
 
     def fixLibraryStats(self, sep, sd):
         libstat = (sep, sd)
-        logging.debug("New library stat: {0}".format(libstat))
+        logger.debug("New library stat: {0}".format(libstat))
         self.libstats = [libstat] * self.nlibs
 
     def write(self, filename):
         fw = open(filename, "wb")
         fw.write(pack("8s", "BINWRITE"))
         fw.write(pack("i", self.version))
         fw.write(pack("Q", self.nreads))
@@ -101,15 +102,15 @@
             fw.write(pack("{0}s".format(slen), name))
         fw.write(pack("Q", self.npairs))
         self.r1.tofile(fw)
         fw.write(pack("Q", self.npairs))
         self.r2.tofile(fw)
         fw.write(pack("Q", self.npairs))
         self.libs.tofile(fw)
-        logging.debug("New pairs file written to `{0}`.".format(filename))
+        logger.debug("New pairs file written to `{0}`.".format(filename))
 
 
 def main():
 
     actions = (
         ("prepare", "prepare ALLPATHS csv files and run script"),
         ("log", "prepare a log of created files"),
@@ -126,16 +127,16 @@
     """
     %prog dump fastbfile
 
     Export ALLPATHS fastb file to fastq file. Use --dir to indicate a previously
     run allpaths folder.
     """
     p = OptionParser(dump.__doc__)
-    p.add_option("--dir", help="Working directory")
-    p.add_option(
+    p.add_argument("--dir", help="Working directory")
+    p.add_argument(
         "--nosim",
         default=False,
         action="store_true",
         help="Do not simulate qual to 50",
     )
     opts, args = p.parse_args(args)
 
@@ -171,15 +172,15 @@
 
         libname = row.split()[0]
         if libname == "Unpaired":
             continue
 
         libs.append(libname)
 
-    logging.debug("Found libraries: {0}".format(",".join(libs)))
+    logger.debug("Found libraries: {0}".format(",".join(libs)))
 
     cmds = []
     for libname in libs:
         cmd = "FastbQualbToFastq"
         cmd += " HEAD_IN={0}.{1}.AB HEAD_OUT={1}".format(pf, libname)
         cmd += " PAIRED=True PHRED_OFFSET=33"
         if sim:
@@ -225,18 +226,18 @@
 def fill(args):
     """
     %prog fill frag_reads_corr.fastb
 
     Run FillFragments on `frag_reads_corr.fastb`.
     """
     p = OptionParser(fill.__doc__)
-    p.add_option(
+    p.add_argument(
         "--stretch",
         default=3,
-        type="int",
+        type=int,
         help="MAX_STRETCH to pass to FillFragments",
     )
     p.set_cpus()
 
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
@@ -299,20 +300,20 @@
     while True:
         contents = list(islice(fp, 4))
         if not contents:
             break
         fragsfw.writelines(contents)
         nfrags += 1
 
-    logging.debug(
+    logger.debug(
         "A total of {0} paired reads written to `{1}`.".format(
             npairs, ",".join(x.name for x in p1fw + p2fw)
         )
     )
-    logging.debug(
+    logger.debug(
         "A total of {0} single reads written to `{1}`.".format(nfrags, fragsfw.name)
     )
 
     # Validate the numbers
     expected_pairs = 2 * p.npairs
     expected_frags = p.nreads - 2 * p.npairs
     assert npairs == expected_pairs, "Expect {0} paired reads, got {1} instead".format(
@@ -330,21 +331,21 @@
     Parse ALLPATHS pairs file, and write pairs IDs and single read IDs in
     respective ids files: e.g. `lib1.pairs.fastq`, `lib2.pairs.fastq`,
     and single `frags.fastq` (with single reads from lib1/2).
     """
     from jcvi.assembly.preprocess import run_FastbAndQualb2Fastq
 
     p = OptionParser(pairs.__doc__)
-    p.add_option(
+    p.add_argument(
         "--header",
         default=False,
         action="store_true",
         help="Print header only",
     )
-    p.add_option(
+    p.add_argument(
         "--suffix",
         default=False,
         action="store_true",
         help="Add suffix /1, /2 to read names",
     )
     opts, args = p.parse_args(args)
 
@@ -411,27 +412,27 @@
     `in_libs.csv`. The species name does not really matter.
     """
     from jcvi.utils.table import write_csv
     from jcvi.formats.base import write_file
     from jcvi.formats.fastq import guessoffset, readlen
 
     p = OptionParser(prepare.__doc__ + FastqNamings)
-    p.add_option(
+    p.add_argument(
         "--corr",
         default=False,
         action="store_true",
         help="Extra parameters for corrected data",
     )
-    p.add_option(
+    p.add_argument(
         "--norun",
         default=False,
         action="store_true",
         help="Don't write `run.sh` script",
     )
-    p.add_option("--ploidy", default="2", choices=("1", "2"), help="Ploidy")
+    p.add_argument("--ploidy", default="2", choices=("1", "2"), help="Ploidy")
     p.set_cpus()
     opts, args = p.parse_args(args)
 
     if len(args) < 1:
         sys.exit(not p.print_help())
 
     organism_name = args[0]
@@ -502,18 +503,18 @@
         (groups_33, "in_groups_33.csv"),
         (groups_64, "in_groups_64.csv"),
         (groups_33 + groups_64, "in_groups.csv"),
     ):
         if not groups:
             continue
         write_csv(groupheader, groups, filename=csvfile, tee=True)
-        logging.debug("`{0}` created (# of groups = {1}).".format(csvfile, len(groups)))
+        logger.debug("`{0}` created (# of groups = {1}).".format(csvfile, len(groups)))
 
     write_csv(libheader, libcontents, filename="in_libs.csv", tee=True)
-    logging.debug("`in_libs.csv` created (# of libs = {0}).".format(len(libcontents)))
+    logger.debug("`in_libs.csv` created (# of libs = {0}).".format(len(libcontents)))
 
     runfile = "run.sh"
 
     # ALLPATHS stalls on reads over 250bp <https://www.biostars.org/p/122091/>
     max_rd_len = max(readlen([f]) for f in fnames)
     extra = "CLOSE_UNIPATH_GAPS=False " if max_rd_len > 200 else ""
     if opts.corr:
```

### Comparing `jcvi-1.4.6/jcvi/assembly/automaton.py` & `jcvi-1.4.7/jcvi/assembly/automaton.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 
 """
 Automate genome assembly by iterating assembly on a set of files, individually.
 """
 import os
 import os.path as op
 import sys
-import logging
 
 from more_itertools import grouper
 
-from jcvi.formats.base import LineFile, write_file
-from jcvi.formats.fastq import first, pairspf
-from jcvi.apps.base import (
-    OptionParser,
+from ..apps.base import (
     ActionDispatcher,
-    need_update,
-    mkdir,
-    sh,
+    OptionParser,
+    get_abs_path,
     glob,
     iglob,
-    get_abs_path,
+    logger,
+    mkdir,
+    need_update,
+    sh,
 )
+from ..formats.base import LineFile, write_file
+from ..formats.fastq import first, pairspf
 
 
 class Meta(object):
     def __init__(self, fastq, guess=True):
         # Note the guesswork is largely based on JIRA LIMS naming convention
         self.fastq = fastq.strip()
         self.suffix = op.splitext(fastq)[-1]
@@ -140,15 +140,15 @@
 
     Remove contaminated reads. The FASTQ files in the folder will automatically
     pair and filtered against Ecoli.fasta to remove contaminants using BOWTIE2.
     """
     from jcvi.apps.bowtie import align
 
     p = OptionParser(contamination.__doc__)
-    p.add_option(
+    p.add_argument(
         "--mapped",
         default=False,
         action="store_true",
         help="Retain contaminated reads instead",
     )
     p.set_cutoff(cutoff=800)
     p.set_mateorientation(mateorientation="+-")
@@ -231,15 +231,15 @@
 def allpaths(args):
     """
     %prog allpaths folder1 folder2 ...
 
     Run automated ALLPATHS on list of dirs.
     """
     p = OptionParser(allpaths.__doc__)
-    p.add_option("--ploidy", default="1", choices=("1", "2"), help="Ploidy")
+    p.add_argument("--ploidy", default="1", choices=("1", "2"), help="Ploidy")
     opts, args = p.parse_args(args)
 
     if len(args) == 0:
         sys.exit(not p.print_help())
 
     folders = args
     for pf in folders:
@@ -259,18 +259,18 @@
     Parse JIRA report and prepare input. Look for all FASTQ files in the report
     and get the prefix. Assign fastq to a folder and a new file name indicating
     the library type (e.g. PE-500, MP-5000, etc.).
 
     Note that JIRA report can also be a list of FASTQ files.
     """
     p = OptionParser(prepare.__doc__)
-    p.add_option(
+    p.add_argument(
         "--first",
         default=0,
-        type="int",
+        type=int,
         help="Use only first N reads",
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
@@ -328,15 +328,15 @@
     slink(p, pf, tag)
     assemble_dir(pf, target)
 
 
 def assemble_dir(pf, target, ploidy="1"):
     from jcvi.assembly.allpaths import prepare
 
-    logging.debug("Work on {0}".format(pf))
+    logger.debug("Work on {0}".format(pf))
     asm = [x.replace("final", pf) for x in target]
     if not need_update(pf, asm, warn=True):
         return
 
     cwd = os.getcwd()
     os.chdir(pf)
     prepare(
@@ -345,25 +345,25 @@
         + ["--ploidy={0}".format(ploidy)]
     )
     sh("./run.sh")
 
     for a, t in zip(asm, target):
         sh("cp allpaths/ASSEMBLIES/run/{0} ../{1}".format(t, a))
 
-    logging.debug("Assembly finished: {0}".format(asm))
+    logger.debug("Assembly finished: {0}".format(asm))
     os.chdir(cwd)
 
 
 def correct_pairs(p, pf, tag):
     """
     Take one pair of reads and correct to generate *.corr.fastq.
     """
     from jcvi.assembly.preprocess import correct as cr
 
-    logging.debug("Work on {0} ({1})".format(pf, ",".join(p)))
+    logger.debug("Work on {0} ({1})".format(pf, ",".join(p)))
     itag = tag[0]
     cm = ".".join((pf, itag))
     targets = (cm + ".1.corr.fastq", cm + ".2.corr.fastq", pf + ".PE-0.corr.fastq")
     if not need_update(p, targets, warn=True):
         return
 
     slink(p, pf, tag)
@@ -371,25 +371,25 @@
     cwd = os.getcwd()
     os.chdir(pf)
     cr(sorted(glob("*.fastq") + glob("*.fastq.gz")) + ["--nofragsdedup"])
     sh("mv {0}.1.corr.fastq ../{1}".format(itag, targets[0]))
     sh("mv {0}.2.corr.fastq ../{1}".format(itag, targets[1]))
     sh("mv frag_reads_corr.corr.fastq ../{0}".format(targets[2]))
 
-    logging.debug("Correction finished: {0}".format(targets))
+    logger.debug("Correction finished: {0}".format(targets))
     os.chdir(cwd)
 
 
 def soap_trios(p, pf, tag, extra):
     """
     Take one pair of reads and 'widow' reads after correction and run SOAP.
     """
     from jcvi.assembly.soap import prepare
 
-    logging.debug("Work on {0} ({1})".format(pf, ",".join(p)))
+    logger.debug("Work on {0} ({1})".format(pf, ",".join(p)))
     asm = "{0}.closed.scafSeq".format(pf)
     if not need_update(p, asm, warn=True):
         return
 
     slink(p, pf, tag, extra)
 
     cwd = os.getcwd()
@@ -397,15 +397,15 @@
     prepare(
         sorted(glob("*.fastq") + glob("*.fastq.gz"))
         + ["--assemble_1st_rank_only", "-K 31"]
     )
     sh("./run.sh")
     sh("cp asm31.closed.scafSeq ../{0}".format(asm))
 
-    logging.debug("Assembly finished: {0}".format(asm))
+    logger.debug("Assembly finished: {0}".format(asm))
     os.chdir(cwd)
 
 
 def iter_project(
     folder, pattern="*.fq,*.fq.gz,*.fastq,*.fastq.gz", n=2, commonprefix=True
 ):
     # Check for paired reads and extract project id
```

### Comparing `jcvi-1.4.6/jcvi/assembly/base.py` & `jcvi-1.4.7/jcvi/assembly/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 """
 Base utilties for genome assembly related calculations and manipulations
 """
 import os.path as op
 import sys
 
 from math import log
+from bisect import bisect
 
 import numpy as np
-from bisect import bisect
 
-from jcvi.formats.base import must_open
-from jcvi.formats.fasta import Fasta
-from jcvi.apps.base import OptionParser, ActionDispatcher, glob
+from ..formats.base import must_open
+from ..formats.fasta import Fasta
+from ..apps.base import ActionDispatcher, OptionParser, glob
 
 ln2 = log(2)
 
 
 types = {"PE": "fragment", "MP": "jumping", "TT": "jumping", "LL": "long"}
 header = ("Length", "L50", "N50", "Min", "Max", "N")
 
@@ -100,15 +100,15 @@
 
 
 def calculate_A50(ctgsizes, cutoff=0, percent=50):
     """
     Given an array of contig sizes, produce A50, N50, and L50 values
     """
 
-    ctgsizes = np.array(ctgsizes, dtype="int")
+    ctgsizes = np.array(ctgsizes, dtype=int)
     ctgsizes = np.sort(ctgsizes)[::-1]
     ctgsizes = ctgsizes[ctgsizes >= cutoff]
 
     a50 = np.cumsum(ctgsizes)
 
     total = np.sum(ctgsizes)
     idx = bisect(a50, total * percent / 100.0)
@@ -152,15 +152,15 @@
 
     Given a file with a list of numbers denoting contig lengths, calculate N50.
     Input file can be both FASTA or a list of sizes.
     """
     from jcvi.graphics.histogram import loghistogram
 
     p = OptionParser(n50.__doc__)
-    p.add_option(
+    p.add_argument(
         "--print0",
         default=False,
         action="store_true",
         help="Print size and L50 to stdout",
     )
 
     opts, args = p.parse_args(args)
```

### Comparing `jcvi-1.4.6/jcvi/assembly/chic.pyx` & `jcvi-1.4.7/jcvi/assembly/chic.pyx`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.6/jcvi/assembly/coverage.py` & `jcvi-1.4.7/jcvi/assembly/coverage.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,20 @@
 
 """
 Provide coverage QC for assembled sequences:
 1. plot paired-end reads as curves
 2. plot base coverage and mate coverage
 3. plot gaps in the sequence (if any)
 """
-import logging
-
 from collections import defaultdict
 
-from jcvi.formats.base import BaseFile, must_open
-from jcvi.formats.sizes import Sizes
-from jcvi.formats.bed import BedLine, sort
-from jcvi.apps.base import ActionDispatcher, sh, need_update
+from ..apps.base import ActionDispatcher, logger, need_update, sh
+from ..formats.base import BaseFile, must_open
+from ..formats.bed import BedLine, sort
+from ..formats.sizes import Sizes
 
 
 class Coverage(BaseFile):
     """
     Three-column .coverage file, often generated by `genomeCoverageBed -d`
     contigID baseID coverage
     """
@@ -107,15 +105,15 @@
     if matesfile:
         fp = open(matesfile)
         libraryline = next(fp)
         # 'library bes     37896   126916'
         lib, name, smin, smax = libraryline.split()
         assert lib == "library"
         smin, smax = int(smin), int(smax)
-        logging.debug(
+        logger.debug(
             "Happy mates for lib {0} fall between {1} - {2}".format(name, smin, smax)
         )
 
     nbedpe = 0
     nspan = 0
     for clonename, blines in clones.items():
         nlines = len(blines)
@@ -146,17 +144,17 @@
                 print(
                     "\t".join(str(x) for x in (aseqid, start - 1, end, clonename)),
                     file=fwpairs,
                 )
                 nspan += 1
 
     fw.close()
-    logging.debug("A total of {0} bedpe written to `{1}`.".format(nbedpe, bedpefile))
+    logger.debug("A total of {0} bedpe written to `{1}`.".format(nbedpe, bedpefile))
     if pairsbedfile:
         fwpairs.close()
-        logging.debug(
+        logger.debug(
             "A total of {0} spans written to `{1}`.".format(nspan, pairsbedfile)
         )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `jcvi-1.4.6/jcvi/assembly/gaps.py` & `jcvi-1.4.7/jcvi/assembly/gaps.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 # -*- coding: UTF-8 -*-
 
 """
 Calculates gap statistics and manipulate gaps in assembly.
 """
 import os.path as op
 import sys
-import logging
 
 from itertools import groupby
 
-from jcvi.formats.sizes import Sizes
-from jcvi.formats.bed import Bed, fastaFromBed
-from jcvi.formats.blast import BlastSlow
-from jcvi.apps.base import OptionParser, ActionDispatcher, need_update
+from ..apps.base import ActionDispatcher, OptionParser, logger, need_update
+from ..formats.bed import Bed, fastaFromBed
+from ..formats.blast import BlastSlow
+from ..formats.sizes import Sizes
 
 
 def main():
 
     actions = (
         ("flanks", "create sequences flanking the gaps"),
         ("sizes", "compile gap sizes"),
@@ -34,15 +33,15 @@
 
     Annotate AGP file with linkage info of `paired-end` or `map`.
     File `gaps.linkage.bed` is generated by assembly.gaps.estimate().
     """
     from jcvi.formats.agp import AGP, bed, tidy
 
     p = OptionParser(annotate.__doc__)
-    p.add_option("--minsize", default=200, help="Smallest component size")
+    p.add_argument("--minsize", default=200, help="Smallest component size")
     opts, args = p.parse_args(args)
 
     if len(args) != 3:
         sys.exit(not p.print_help())
 
     agpfile, linkagebed, assemblyfasta = args
     linkagebed = Bed(linkagebed)
@@ -86,15 +85,15 @@
         else:
             tag = "paired-ends"
 
         a.linkage_evidence.append(tag)
         print(a, file=newagp)
 
     newagp.close()
-    logging.debug("Annotated AGP written to `{0}`.".format(newagpfile))
+    logger.debug("Annotated AGP written to `%s`.", newagpfile)
 
     contigbed = assemblyfasta.rsplit(".", 1)[0] + ".contigs.bed"
     bedfile = bed([newagpfile, "--nogaps", "--outfile=" + contigbed])
 
     contigfasta = fastaFromBed(bedfile, assemblyfasta, name=True, stranded=True)
 
     tidy([newagpfile, contigfasta])
@@ -239,18 +238,18 @@
 def flanks(args):
     """
     %prog flanks gaps.bed fastafile
 
     Create sequences flanking the gaps.
     """
     p = OptionParser(flanks.__doc__)
-    p.add_option(
+    p.add_argument(
         "--extend",
         default=2000,
-        type="int",
+        type=int,
         help="Extend seq flanking the gaps",
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
```

### Comparing `jcvi-1.4.6/jcvi/assembly/geneticmap.py` & `jcvi-1.4.7/jcvi/assembly/geneticmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from itertools import combinations, groupby
 from random import sample
 from typing import Tuple
 
 import numpy as np
 import seaborn as sns
 
-from ..apps.base import OptionParser, ActionDispatcher, logger, need_update
+from ..apps.base import ActionDispatcher, OptionParser, logger, need_update
 from ..algorithms.formula import calc_ldscore
 from ..algorithms.matrix import symmetrize
 from ..formats.base import BaseFile, LineFile, must_open, read_block
 from ..formats.bed import Bed, fastaFromBed
 from ..graphics.base import (
     Rectangle,
     draw_cmap,
@@ -368,15 +368,15 @@
 
         M = symmetrize(M)
 
         logger.debug("Write LD matrix to file `%s`.", ldmatrix)
         M.tofile(ldmatrix)
     else:
         nmarkers = len(Bed(markerbedfile))
-        M = np.fromfile(ldmatrix, dtype="float").reshape(nmarkers, nmarkers)
+        M = np.fromfile(ldmatrix, dtype=float).reshape(nmarkers, nmarkers)
         logger.debug("LD matrix `%s` exists (%dx%d).", ldmatrix, nmarkers, nmarkers)
 
     return M, markerbedfile, nmarkers
 
 
 def draw_geneticmap_heatmap(root, ax, mstmap: str, subsample: int):
     """
@@ -429,18 +429,18 @@
 def heatmap(args):
     """
     %prog heatmap map
 
     Calculate pairwise linkage disequilibrium given MSTmap.
     """
     p = OptionParser(heatmap.__doc__)
-    p.add_option(
+    p.add_argument(
         "--subsample",
         default=1000,
-        type="int",
+        type=int,
         help="Subsample markers to speed up",
     )
     opts, args, iopts = p.set_image_options(args, figsize="8x8")
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
@@ -465,16 +465,16 @@
 
     Rename lines in the map header. The mapping of old names to new names are
     stored in two-column `conversion_table`.
     """
     from jcvi.formats.base import DictFile
 
     p = OptionParser(header.__doc__)
-    p.add_option("--prefix", default="", help="Prepend text to line number")
-    p.add_option("--ids", help="Write ids to file")
+    p.add_argument("--prefix", default="", help="Prepend text to line number")
+    p.add_argument("--ids", help="Write ids to file")
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     mstmap, conversion_table = args
     data = MSTMap(mstmap)
@@ -566,21 +566,21 @@
 def bed(args):
     """
     %prog fasta map.out
 
     Convert MSTMAP output into bed format.
     """
     p = OptionParser(bed.__doc__)
-    p.add_option(
+    p.add_argument(
         "--switch",
         default=False,
         action="store_true",
         help="Switch reference and aligned map elements",
     )
-    p.add_option(
+    p.add_argument(
         "--sep",
         default=".",
         help="Separator that is used to delimit scaffold and position in the marker name",
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
@@ -600,18 +600,18 @@
     %prog fasta map.out scaffolds.fasta
 
     Extract marker sequences based on map.
     """
     from jcvi.formats.sizes import Sizes
 
     p = OptionParser(fasta.__doc__)
-    p.add_option(
+    p.add_argument(
         "--extend",
         default=1000,
-        type="int",
+        type=int,
         help="Extend seq flanking the gaps",
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
@@ -669,18 +669,18 @@
 
     Find scaffold breakpoints using genetic map. Use variation.vcf.mstmap() to
     generate the input for this routine.
     """
     from more_itertools import pairwise
 
     p = OptionParser(breakpoint.__doc__)
-    p.add_option(
+    p.add_argument(
         "--diff",
         default=0.1,
-        type="float",
+        type=float,
         help="Maximum ratio of differences allowed",
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
```

### Comparing `jcvi-1.4.6/jcvi/assembly/goldenpath.py` & `jcvi-1.4.7/jcvi/assembly/goldenpath.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,38 +4,38 @@
 """
 Procedures to validate and update golden path of a genome assembly. This relies
 heavily on formats.agp, and further includes several algorithms, e.g. overlap
 detection.
 """
 import os
 import os.path as op
-import sys
 import shutil
-import logging
+import sys
 
 from copy import deepcopy
 from functools import lru_cache
 from itertools import groupby
 
-from jcvi.formats.agp import AGP, TPF, get_phase, reindex, tidy, build
-from jcvi.formats.base import BaseFile, must_open
-from jcvi.formats.fasta import Fasta, SeqIO
-from jcvi.formats.blast import BlastSlow, BlastLine
-from jcvi.formats.coords import Overlap_types
-from jcvi.apps.fetch import entrez
-from jcvi.apps.grid import WriteJobs
-from jcvi.apps.base import (
-    OptionParser,
+from ..apps.base import (
     ActionDispatcher,
+    OptionParser,
     cleanup,
-    popen,
+    logger,
     mkdir,
-    sh,
     need_update,
+    popen,
+    sh,
 )
+from ..apps.fetch import entrez
+from ..apps.grid import WriteJobs
+from ..formats.agp import AGP, TPF, build, get_phase, reindex, tidy
+from ..formats.base import BaseFile, must_open
+from ..formats.blast import BlastLine, BlastSlow
+from ..formats.coords import Overlap_types
+from ..formats.fasta import Fasta, SeqIO
 
 
 GoodPct = 98
 GoodOverlap = 200
 GoodOverhang = 2000
 
 
@@ -470,15 +470,15 @@
             if orientation:
                 if sorientation:
                     try:
                         assert (
                             orientation == sorientation
                         ), "Orientation conflicts:\n{0}\n{1}".format(north, south)
                     except AssertionError as e:
-                        logging.debug(e)
+                        logger.debug(e)
             else:
                 if sorientation:
                     orientation = sorientation
                 else:  # Both overlaps fail to define orientation
                     orientation = orientationguide.get(aid, "+")
 
             component_type = "D" if aphase in (1, 2) else "F"
@@ -552,25 +552,25 @@
     dedupagp = pf + ".dedup.agp"
     fw = open(dedupagp, "w")
 
     ndropped = ndroppedbases = 0
     for a in agp:
         if not a.is_gap and a.component_id not in reps:
             span = a.component_span
-            logging.debug("Drop component {0} ({1})".format(a.component_id, span))
+            logger.debug("Drop component {0} ({1})".format(a.component_id, span))
             ndropped += 1
             ndroppedbases += span
             continue
         print(a, file=fw)
     fw.close()
 
-    logging.debug(
+    logger.debug(
         "Dropped components: {0}, Dropped bases: {1}".format(ndropped, ndroppedbases)
     )
-    logging.debug("Deduplicated file written to `{0}`.".format(dedupagp))
+    logger.debug("Deduplicated file written to `{0}`.".format(dedupagp))
 
     tidyagp = tidy([dedupagp, splitfile])
     dedupfasta = pf + ".dedup.fasta"
     build([tidyagp, dd, dedupfasta])
 
     return dedupfasta
 
@@ -652,16 +652,16 @@
     scaffold4       1609    1771    2       N       163     scaffold        yes     paired-ends
     scaffold4       1772    3771    3       W       ca-bacs.5638.frag10.20000-22000 1       2000    -
 
     These are most likely shreds, which we look for based on names.
     """
     p = OptionParser(anneal.__doc__)
     p.set_align(pctid=GoodPct, hitlen=GoodOverlap)
-    p.add_option(
-        "--hang", default=GoodOverhang, type="int", help="Maximum overhang length"
+    p.add_argument(
+        "--hang", default=GoodOverhang, type=int, help="Maximum overhang length"
     )
     p.set_outdir(outdir="outdir")
     p.set_cpus()
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
@@ -670,23 +670,23 @@
     outdir = opts.outdir
     if not op.exists(outdir):
         mkdir(outdir)
         cmd = "faSplit byname {0} {1}/".format(contigs, outdir)
         sh(cmd)
 
     cutoff = Cutoff(opts.pctid, opts.hitlen, opts.hang)
-    logging.debug(str(cutoff))
+    logger.debug(str(cutoff))
 
     agp = AGP(agpfile)
     blastfile = agpfile.replace(".agp", ".blast")
     if not op.exists(blastfile):
         populate_blastfile(blastfile, agp, outdir, opts)
 
     assert op.exists(blastfile)
-    logging.debug("File `{0}` found. Start loading.".format(blastfile))
+    logger.debug("File `{0}` found. Start loading.".format(blastfile))
     blast = BlastSlow(blastfile).to_dict()
 
     annealedagp = "annealed.agp"
     annealedfasta = "annealed.fasta"
 
     newagp = deepcopy(agp)
     clrstore = {}
@@ -720,15 +720,15 @@
         if o.otype == 2:  # b ~ a
             o = o.swapped
             o.print_graphic()
             if o.anneal(bclr, aclr):
                 newagp.switch_between(bid, aid, verbose=True)
                 newagp.delete_between(bid, aid, verbose=True)
 
-    logging.debug("A total of {0} components with modified CLR.".format(len(clrstore)))
+    logger.debug("A total of {0} components with modified CLR.".format(len(clrstore)))
 
     for cid, c in clrstore.items():
         if c.is_valid:
             continue
         print("Remove {0}".format(c), file=sys.stderr)
         newagp.convert_to_gap(cid, verbose=True)
 
@@ -755,15 +755,15 @@
 
     Insert a component into agpfile by aligning to the best hit in pool and see
     if they have good overlaps.
     """
     from jcvi.apps.align import run_megablast
 
     p = OptionParser(blast.__doc__)
-    p.add_option("-n", type="int", default=2, help="Take best N hits")
+    p.add_argument("-n", type=int, default=2, help="Take best N hits")
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     allfasta, clonename = args
     fastadir = "fasta"
@@ -922,31 +922,31 @@
     Check overlaps between two fasta records. The arguments can be genBank IDs
     instead of FASTA files. In case of IDs, the sequences will be downloaded
     first.
     """
     from jcvi.formats.blast import chain_HSPs
 
     p = OptionParser(overlap.__doc__)
-    p.add_option(
+    p.add_argument(
         "--dir",
         default=os.getcwd(),
         help="Download sequences to dir",
     )
-    p.add_option(
+    p.add_argument(
         "--suffix",
         default="fasta",
         help="Suffix of the sequence file in dir",
     )
-    p.add_option(
+    p.add_argument(
         "--qreverse",
         default=False,
         action="store_true",
         help="Reverse seq a",
     )
-    p.add_option(
+    p.add_argument(
         "--nochain",
         default=False,
         action="store_true",
         help="Do not chain adjacent HSPs",
     )
     p.set_align(pctid=GoodPct, hitlen=GoodOverlap, evalue=0.01)
     p.set_outfile(outfile=None)
@@ -985,15 +985,15 @@
 
     fp = popen(cmd)
     hsps = fp.readlines()
 
     hsps = [BlastLine(x) for x in hsps]
     hsps = [x for x in hsps if x.hitlen >= hitlen]
     if chain:
-        logging.debug("Chain HSPs in the Blast output.")
+        logger.debug("Chain HSPs in the Blast output.")
         dist = 2 * hitlen  # Distance to chain the HSPs
         hsps = chain_HSPs(hsps, xdist=dist, ydist=dist)
 
     if len(hsps) == 0:
         print("No match found.", file=sys.stderr)
         return None
```

### Comparing `jcvi-1.4.6/jcvi/assembly/hic.py` & `jcvi-1.4.7/jcvi/assembly/hic.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     backup,
     iglob,
     logger,
     mkdir,
     symlink,
 )
 from ..apps.grid import Jobs
-from ..assembly.allmaps import make_movie
 from ..compara.synteny import check_beds, get_bed_filenames
 from ..formats.agp import order_to_agp
 from ..formats.base import LineFile, must_open
 from ..formats.bed import Bed
 from ..formats.blast import Blast
 from ..formats.sizes import Sizes
 from ..graphics.base import (
@@ -46,14 +45,17 @@
     plt,
     plot_heatmap,
     savefig,
 )
 from ..graphics.dotplot import dotplot
 from ..utils.cbook import gene_name
 
+from .allmaps import make_movie
+
+
 # Map orientations to ints
 FF = {"+": 1, "-": -1, "?": 1}
 RR = {"+": -1, "-": 1, "?": -1}
 LB = 18  # Lower bound for golden_array()
 UB = 29  # Upper bound for golden_array()
 BB = UB - LB + 1  # Span for golden_array()
 ACCEPT = "[green]ACCEPT"
@@ -620,17 +622,17 @@
     with link counts per dist bin, with the bin starts stored in the genome.json.
     """
     import seaborn as sns
     import pandas as pd
     from jcvi.graphics.base import human_base_formatter, markup
 
     p = OptionParser(dist.__doc__)
-    p.add_option("--title", help="Title of the histogram")
-    p.add_option("--xmin", default=300, help="Minimum distance")
-    p.add_option("--xmax", default=6000000, help="Maximum distance")
+    p.add_argument("--title", help="Title of the histogram")
+    p.add_argument("--xmin", default=300, help="Minimum distance")
+    p.add_argument("--xmax", default=6000000, help="Maximum distance")
     opts, args, iopts = p.set_image_options(args, figsize="6x6")
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     npyfile, jsonfile = args
     pf = npyfile.rsplit(".", 1)[0]
@@ -813,20 +815,20 @@
     seq1 g
     seq2 g
 
     This will first draw a square around seq1+seq2 with blue color, then seq1
     and seq2 individually with green color.
     """
     p = OptionParser(heatmap.__doc__)
-    p.add_option("--title", help="Title of the heatmap")
-    p.add_option("--groups", help="Groups file, see doc")
-    p.add_option("--vmin", default=1, type="int", help="Minimum value in the heatmap")
-    p.add_option("--vmax", default=6, type="int", help="Maximum value in the heatmap")
-    p.add_option("--chr", help="Plot this contig/chr only")
-    p.add_option(
+    p.add_argument("--title", help="Title of the heatmap")
+    p.add_argument("--groups", help="Groups file, see doc")
+    p.add_argument("--vmin", default=1, type=int, help="Minimum value in the heatmap")
+    p.add_argument("--vmax", default=6, type=int, help="Maximum value in the heatmap")
+    p.add_argument("--chr", help="Plot this contig/chr only")
+    p.add_argument(
         "--nobreaks",
         default=False,
         action="store_true",
         help="Do not plot breaks (esp. if contigs are small)",
     )
     opts, args, iopts = p.set_image_options(
         args, figsize="11x11", style="white", cmap="coolwarm", dpi=120
@@ -913,15 +915,15 @@
 
 def get_distbins(start=100, bins=2000, ratio=1.01):
     """Get exponentially sized bins for link length"""
     b = np.ones(bins, dtype="float64")
     b[0] = 100
     for i in range(1, bins):
         b[i] = b[i - 1] * ratio
-    bins = np.around(b).astype(dtype="int")
+    bins = np.around(b).astype(dtype=int)
     binsizes = np.diff(bins)
     return bins, binsizes
 
 
 def bam2mat(args):
     """
     %prog bam2mat input.bam
@@ -931,21 +933,21 @@
     to more fine-grained heatmap, but leads to large .mat size and slower
     plotting.
     """
     import pysam
     from jcvi.utils.cbook import percentage
 
     p = OptionParser(bam2mat.__doc__)
-    p.add_option(
+    p.add_argument(
         "--resolution",
         default=500000,
-        type="int",
+        type=int,
         help="Resolution when counting the links",
     )
-    p.add_option(
+    p.add_argument(
         "--seqids",
         default=None,
         help="Use a given seqids file, a single line with seqids joined by comma",
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
@@ -988,16 +990,16 @@
 
     json.dump(header, fwjson, sort_keys=True, indent=4, default=default)
     fwjson.close()
     logger.debug("Contig bin starts written to `%s`", jsonfile)
 
     print(sorted(seqstarts.items(), key=lambda x: x[-1]))
     logger.debug("Initialize matrix of size %dx%d", total_bins, total_bins)
-    A = np.zeros((total_bins, total_bins), dtype="int")
-    B = np.zeros(bins, dtype="int")
+    A = np.zeros((total_bins, total_bins), dtype=int)
+    B = np.zeros(bins, dtype=int)
 
     # Find the bin ID of each read
     def bin_number(chr, pos):
         return seqstarts[chr] + pos // N
 
     def distbin_number(dist, start=minsize, ratio=1.01):
         return int(round(math.log(dist * 1.0 / start, ratio)))
@@ -1059,18 +1061,18 @@
 
     The simulator assumes several distributions:
     - Links are distributed uniformly across genome
     - Log10(link_size) are distributed normally
     - Genes are distributed uniformly
     """
     p = OptionParser(simulate.__doc__)
-    p.add_option("--genomesize", default=10000000, type="int", help="Genome size")
-    p.add_option("--genes", default=1000, type="int", help="Number of genes")
-    p.add_option("--contigs", default=100, type="int", help="Number of contigs")
-    p.add_option("--coverage", default=10, type="int", help="Link coverage")
+    p.add_argument("--genomesize", default=10000000, type=int, help="Genome size")
+    p.add_argument("--genes", default=1000, type=int, help="Number of genes")
+    p.add_argument("--contigs", default=100, type=int, help="Number of contigs")
+    p.add_argument("--coverage", default=10, type=int, help="Link coverage")
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (pf,) = args
     GenomeSize = opts.genomesize
@@ -1102,15 +1104,15 @@
 
     # Simulate links, uniform start, with link distances following 1/x, where x
     # is the distance between the links. As an approximation, we have links
     # between [1e3, 1e7], so we map from uniform [1e-7, 1e-3]
     LinkStarts = np.sort(np.random.randint(1, GenomeSize, size=Links))
     a, b = 1e-7, 1e-3
     LinkSizes = np.array(
-        np.round_(1 / ((b - a) * np.random.rand(Links) + a), decimals=0), dtype="int"
+        np.round_(1 / ((b - a) * np.random.rand(Links) + a), decimals=0), dtype=int
     )
     LinkEnds = LinkStarts + LinkSizes
 
     # Find link to contig membership
     LinkStartContigs = np.searchsorted(ContigStarts, LinkStarts) - 1
     LinkEndContigs = np.searchsorted(ContigStarts, LinkEnds) - 1
 
@@ -1216,15 +1218,15 @@
 def density(args):
     """
     %prog density test.clm
 
     Estimate link density of contigs.
     """
     p = OptionParser(density.__doc__)
-    p.add_option(
+    p.add_argument(
         "--save",
         default=False,
         action="store_true",
         help="Write log densitites of contigs to file",
     )
     p.set_cpus()
     opts, args = p.parse_args(args)
@@ -1256,27 +1258,27 @@
 def optimize(args):
     """
     %prog optimize test.clm
 
     Optimize the contig order and orientation, based on CLM file.
     """
     p = OptionParser(optimize.__doc__)
-    p.add_option(
+    p.add_argument(
         "--skiprecover",
         default=False,
         action="store_true",
         help="Do not import 'recover' contigs",
     )
-    p.add_option(
+    p.add_argument(
         "--startover",
         default=False,
         action="store_true",
         help="Do not resume from existing tour file",
     )
-    p.add_option("--skipGA", default=False, action="store_true", help="Skip GA step")
+    p.add_argument("--skipGA", default=False, action="store_true", help="Skip GA step")
     p.set_outfile(outfile=None)
     p.set_cpus()
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
@@ -1475,16 +1477,16 @@
 def movie(args):
     """
     %prog movie test.tour test.clm ref.contigs.last
 
     Plot optimization history.
     """
     p = OptionParser(movie.__doc__)
-    p.add_option("--frames", default=500, type="int", help="Only plot every N frames")
-    p.add_option(
+    p.add_argument("--frames", default=500, type=int, help="Only plot every N frames")
+    p.add_argument(
         "--engine",
         default="ffmpeg",
         choices=("ffmpeg", "gifsicle"),
         help="Movie engine, output MP4 or GIF",
     )
     p.set_beds()
     opts, args, iopts = p.set_image_options(
@@ -1662,15 +1664,15 @@
 def movieframe(args):
     """
     %prog movieframe tour test.clm contigs.ref.anchors
 
     Draw heatmap and synteny in the same plot.
     """
     p = OptionParser(movieframe.__doc__)
-    p.add_option("--label", help="Figure title")
+    p.add_argument("--label", help="Figure title")
     p.set_beds()
     p.set_outfile(outfile=None)
     opts, args, iopts = p.set_image_options(
         args, figsize="16x8", style="white", cmap="coolwarm", format="png", dpi=120
     )
 
     if len(args) != 3:
```

### Comparing `jcvi-1.4.6/jcvi/assembly/kmer.py` & `jcvi-1.4.7/jcvi/assembly/kmer.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     plt,
     savefig,
     set_human_axis,
     set_ticklabels_helvetica,
     write_messages,
 )
 from ..utils.cbook import thousands, percentage
+
 from .automaton import iter_project
 
 
 KMERYL, KSOAP, KALLPATHS = range(3)
 
 
 class KmerSpectrum(BaseFile):
@@ -620,16 +621,16 @@
     """
     %prog entropy kmc_dump.out
 
     kmc_dump.out contains two columns:
     AAAAAAAAAAAGAAGAAAGAAA  34
     """
     p = OptionParser(entropy.__doc__)
-    p.add_option(
-        "--threshold", default=0, type="int", help="Complexity needs to be above"
+    p.add_argument(
+        "--threshold", default=0, type=int, help="Complexity needs to be above"
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (kmc_out,) = args
@@ -680,46 +681,46 @@
 def kmcop(args):
     """
     %prog kmcop *.kmc_suf
 
     Intersect or union kmc indices.
     """
     p = OptionParser(kmcop.__doc__)
-    p.add_option(
+    p.add_argument(
         "--action",
         choices=("union", "intersect", "reduce"),
         default="union",
         help="Action",
     )
-    p.add_option(
+    p.add_argument(
         "--ci_in",
         default=0,
-        type="int",
+        type=int,
         help="Exclude input kmers with less than ci_in counts",
     )
-    p.add_option(
+    p.add_argument(
         "--cs",
         default=0,
-        type="int",
+        type=int,
         help="Maximal value of a counter, only used when action is reduce",
     )
-    p.add_option(
+    p.add_argument(
         "--ci_out",
         default=0,
-        type="int",
+        type=int,
         help="Exclude output kmers with less than ci_out counts",
     )
-    p.add_option(
+    p.add_argument(
         "--batch",
         default=1,
-        type="int",
+        type=int,
         help="Number of batch, useful to reduce memory usage",
     )
-    p.add_option("--exclude", help="Exclude accessions from this list")
-    p.add_option("-o", default="results", help="Output name")
+    p.add_argument("--exclude", help="Exclude accessions from this list")
+    p.add_argument("-o", default="results", help="Output name")
     opts, args = p.parse_args(args)
 
     if len(args) < 2:
         sys.exit(not p.print_help())
 
     indices = args
     if opts.exclude:
@@ -768,34 +769,34 @@
 def kmc(args):
     """
     %prog kmc folder
 
     Run kmc3 on Illumina reads.
     """
     p = OptionParser(kmc.__doc__)
-    p.add_option("-k", default=27, type="int", help="Kmer size")
-    p.add_option(
-        "--ci", default=2, type="int", help="Exclude kmers with less than ci counts"
-    )
-    p.add_option("--cs", default=0, type="int", help="Maximal value of a counter")
-    p.add_option("--cx", type="int", help="Exclude kmers with more than cx counts")
-    p.add_option(
+    p.add_argument("-k", default=27, type=int, help="Kmer size")
+    p.add_argument(
+        "--ci", default=2, type=int, help="Exclude kmers with less than ci counts"
+    )
+    p.add_argument("--cs", default=0, type=int, help="Maximal value of a counter")
+    p.add_argument("--cx", type=int, help="Exclude kmers with more than cx counts")
+    p.add_argument(
         "--single",
         default=False,
         action="store_true",
         help="Input is single-end data, only one FASTQ/FASTA",
     )
-    p.add_option(
+    p.add_argument(
         "--fasta",
         default=False,
         action="store_true",
         help="Input is FASTA instead of FASTQ",
     )
-    p.add_option(
-        "--mem", default=48, type="int", help="Max amount of RAM in GB (`kmc -m`)"
+    p.add_argument(
+        "--mem", default=48, type=int, help="Max amount of RAM in GB (`kmc -m`)"
     )
     p.set_cpus()
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
@@ -834,15 +835,15 @@
 def meryl(args):
     """
     %prog meryl folder
 
     Run meryl on Illumina reads.
     """
     p = OptionParser(meryl.__doc__)
-    p.add_option("-k", default=19, type="int", help="Kmer size")
+    p.add_argument("-k", default=19, type=int, help="Kmer size")
     p.set_cpus()
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (folder,) = args
@@ -875,16 +876,16 @@
 
     Model kmer distribution given error rate. See derivation in FIONA paper:
     <http://bioinformatics.oxfordjournals.org/content/30/17/i356.full>
     """
     from scipy.stats import binom, poisson
 
     p = OptionParser(model.__doc__)
-    p.add_option("-k", default=23, type="int", help="Kmer size")
-    p.add_option("--cov", default=50, type="int", help="Expected coverage")
+    p.add_argument("-k", default=23, type=int, help="Kmer size")
+    p.add_argument("--cov", default=50, type=int, help="Expected coverage")
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (erate,) = args
     erate = float(erate)
@@ -1006,15 +1007,15 @@
 
     Count K-mers in the bin.
     """
     from bitarray import bitarray
     from jcvi.formats.sizes import Sizes
 
     p = OptionParser(bincount.__doc__)
-    p.add_option("-K", default=23, type="int", help="K-mer size")
+    p.add_argument("-K", default=23, type=int, help="K-mer size")
     p.set_outfile()
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     fastafile, binfile = args
@@ -1069,15 +1070,15 @@
 def dump(args):
     """
     %prog dump fastafile
 
     Convert FASTA sequences to list of K-mers.
     """
     p = OptionParser(dump.__doc__)
-    p.add_option("-K", default=23, type="int", help="K-mer size")
+    p.add_argument("-K", default=23, type=int, help="K-mer size")
     p.set_outfile()
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (fastafile,) = args
@@ -1096,23 +1097,23 @@
 
     Run jellyfish to dump histogram to be used in kmer.histogram().
     """
     from jcvi.apps.base import getfilesize
     from jcvi.utils.cbook import human_size
 
     p = OptionParser(jellyfish.__doc__)
-    p.add_option("-K", default=23, type="int", help="K-mer size")
-    p.add_option(
+    p.add_argument("-K", default=23, type=int, help="K-mer size")
+    p.add_argument(
         "--coverage",
         default=40,
-        type="int",
+        type=int,
         help="Expected sequence coverage",
     )
-    p.add_option("--prefix", default="jf", help="Database prefix")
-    p.add_option(
+    p.add_argument("--prefix", default="jf", help="Database prefix")
+    p.add_argument(
         "--nohist",
         default=False,
         action="store_true",
         help="Do not print histogram",
     )
     p.set_home("jellyfish")
     p.set_cpus()
@@ -1167,18 +1168,18 @@
     """
     %prog multihistogram *.histogram species
 
     Plot the histogram based on a set of K-mer hisotograms. The method is based
     on Star et al.'s method (Atlantic Cod genome paper).
     """
     p = OptionParser(multihistogram.__doc__)
-    p.add_option("--kmin", default=15, type="int", help="Minimum K-mer size, inclusive")
-    p.add_option("--kmax", default=30, type="int", help="Maximum K-mer size, inclusive")
-    p.add_option("--vmin", default=2, type="int", help="Minimum value, inclusive")
-    p.add_option("--vmax", default=100, type="int", help="Maximum value, inclusive")
+    p.add_argument("--kmin", default=15, type=int, help="Minimum K-mer size, inclusive")
+    p.add_argument("--kmax", default=30, type=int, help="Maximum K-mer size, inclusive")
+    p.add_argument("--vmin", default=2, type=int, help="Minimum value, inclusive")
+    p.add_argument("--vmax", default=100, type=int, help="Maximum value, inclusive")
     opts, args, iopts = p.set_image_options(args, figsize="10x5", dpi=300)
 
     if len(args) < 1:
         sys.exit(not p.print_help())
 
     histfiles = args[:-1]
     species = args[-1]
@@ -1345,45 +1346,45 @@
     """
     %prog histogram meryl.histogram species K
 
     Plot the histogram based on Jellyfish or meryl K-mer distribution, species and N are
     only used to annotate the graphic.
     """
     p = OptionParser(histogram.__doc__)
-    p.add_option(
+    p.add_argument(
         "--vmin",
         dest="vmin",
         default=2,
-        type="int",
+        type=int,
         help="minimum value, inclusive",
     )
-    p.add_option(
+    p.add_argument(
         "--vmax",
         dest="vmax",
         default=200,
-        type="int",
+        type=int,
         help="maximum value, inclusive",
     )
-    p.add_option(
+    p.add_argument(
         "--method",
         choices=("nbinom", "allpaths"),
         default="nbinom",
         help="'nbinom' - slow but more accurate for het or polyploid genome; "
         + "'allpaths' - fast and works for homozygous enomes",
     )
-    p.add_option(
+    p.add_argument(
         "--maxiter",
         default=100,
-        type="int",
+        type=int,
         help="Max iterations for optimization. Only used with --method nbinom",
     )
-    p.add_option(
-        "--coverage", default=0, type="int", help="Kmer coverage [default: auto]"
+    p.add_argument(
+        "--coverage", default=0, type=int, help="Kmer coverage [default: auto]"
     )
-    p.add_option(
+    p.add_argument(
         "--nopeaks",
         default=False,
         action="store_true",
         help="Do not annotate K-mer peaks",
     )
     opts, args, iopts = p.set_image_options(args, figsize="7x7")
```

### Comparing `jcvi-1.4.6/jcvi/assembly/opticalmap.py` & `jcvi-1.4.7/jcvi/assembly/opticalmap.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 """
 Optical map alignment parser.
 """
 import sys
-import logging
 
 from collections import defaultdict
 from xml.etree.ElementTree import ElementTree
 
 import numpy as np
 from more_itertools import pairwise
 
-from jcvi.formats.bed import Bed
-from jcvi.formats.base import must_open
-from jcvi.utils.range import range_chain, range_parse, Range
-from jcvi.apps.base import OptionParser, ActionDispatcher
+from ..apps.base import ActionDispatcher, OptionParser, logger
+from ..formats.base import must_open
+from ..formats.bed import Bed
+from ..utils.range import range_chain, range_parse, Range
 
 
 class OpticalMap(object):
     def __init__(self, xmlfile):
         tree = ElementTree()
         self.root = tree.parse(xmlfile)
         self.maps = dict(self.iter_maps())
@@ -308,17 +307,15 @@
 
             chimeraline = "\t".join(str(x) for x in (seqid, start, end))
             print(chimeraline, file=fw)
             print(chimeraline, file=sys.stderr)
             nchimera += 1
 
     fw.close()
-    logging.debug(
-        "A total of {0} junctions written to `{1}`.".format(nchimera, chimerabed)
-    )
+    logger.debug("A total of %d junctions written to `%s`.", nchimera, chimerabed)
 
 
 def select_bed(bed):
     """
     Return non-overlapping set of ranges, choosing high scoring blocks over low
     scoring alignments when there are conflicts.
     """
@@ -360,15 +357,15 @@
         scf = range_parse(b.accn).seqid
         chr = b.seqid
         cs = (chr, scf)
         if cs not in seen:
             oo.add(chr, scf, sizes[scf], b.strand)
             seen.add(cs)
         else:
-            logging.debug("Seen {0}, ignored.".format(cs))
+            logger.debug("Seen %s, ignored.", cs)
 
     oo.write_AGP(agp, gaptype="contig")
     agp.close()
     build([agpfile, scffasta, pmolfasta])
 
 
 def bed(args):
@@ -376,34 +373,34 @@
     %prog bed xmlfile
 
     Print summary of optical map alignment in BED format.
     """
     from jcvi.formats.bed import sort
 
     p = OptionParser(bed.__doc__)
-    p.add_option(
+    p.add_argument(
         "--blockonly",
         default=False,
         action="store_true",
         help="Only print out large blocks, not fragments",
     )
-    p.add_option(
+    p.add_argument(
         "--point",
         default=False,
         action="store_true",
         help="Print accesssion as single point instead of interval",
     )
-    p.add_option("--scale", type="float", help="Scale the OM distance by factor")
-    p.add_option(
+    p.add_argument("--scale", type=float, help="Scale the OM distance by factor")
+    p.add_argument(
         "--switch",
         default=False,
         action="store_true",
         help="Switch reference and aligned map elements",
     )
-    p.add_option(
+    p.add_argument(
         "--nosort",
         default=False,
         action="store_true",
         help="Do not sort bed",
     )
     opts, args = p.parse_args(args)
```

### Comparing `jcvi-1.4.6/jcvi/assembly/patch.py` & `jcvi-1.4.7/jcvi/assembly/patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,40 +13,39 @@
 4. Add telomeric sequences
 5. Find gaps in optical map
 6. Insert unplaced scaffolds using mates
 """
 import os.path as op
 import sys
 import math
-import logging
 
 from collections import defaultdict
 from itertools import groupby
 from more_itertools import pairwise, roundrobin
 
-from jcvi.formats.bed import (
+from ..apps.base import ActionDispatcher, OptionParser, cleanup, logger, sh
+from ..formats.base import FileMerger
+from ..formats.bed import (
     Bed,
     BedLine,
     complementBed,
-    mergeBed,
     fastaFromBed,
+    mergeBed,
     summary,
 )
-from jcvi.formats.blast import BlastSlow
-from jcvi.formats.sizes import Sizes
-from jcvi.utils.range import (
-    range_parse,
-    range_distance,
-    range_minmax,
-    range_merge,
+from ..formats.blast import BlastSlow
+from ..formats.sizes import Sizes
+from ..utils.range import (
     range_closest,
+    range_distance,
     range_interleave,
+    range_merge,
+    range_minmax,
+    range_parse,
 )
-from jcvi.formats.base import FileMerger
-from jcvi.apps.base import ActionDispatcher, OptionParser, cleanup, sh
 
 
 def main():
 
     actions = (
         # OM guided approach
         ("refine", "find gaps within or near breakpoint regions"),
@@ -79,30 +78,30 @@
     missing, add the whole cassette as unplaced scaffolds. For singletons the
     program will try to make a patch.
     """
     from jcvi.formats.base import DictFile
     from jcvi.utils.cbook import gene_name
 
     p = OptionParser(pastegenes.__doc__)
-    p.add_option(
+    p.add_argument(
         "--cutoff",
         default=90,
-        type="int",
+        type=int,
         help="Coverage cutoff to call gene missing",
     )
-    p.add_option(
+    p.add_argument(
         "--flank",
         default=2000,
-        type="int",
+        type=int,
         help="Get the seq of size on two ends",
     )
-    p.add_option(
+    p.add_argument(
         "--maxsize",
         default=50000,
-        type="int",
+        type=int,
         help="Maximum size of patchers to be replaced",
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 4:
         sys.exit(not p.print_help())
 
@@ -185,29 +184,29 @@
     fw.close()
     fwe.close()
 
     extrabed = mergeBed(extrabed, d=flank, nms=True)
     fastaFromBed(extrabed, oldassembly, name=True)
     summary([extrabed])
 
-    logging.debug("Singleton blocks : {0}".format(singletons))
-    logging.debug("Large blocks : {0} ({1} genes)".format(large, large_genes))
+    logger.debug("Singleton blocks : {0}".format(singletons))
+    logger.debug("Large blocks : {0} ({1} genes)".format(large, large_genes))
 
 
 def pasteprepare(args):
     """
     %prog pasteprepare bacs.fasta
 
     Prepare sequences for paste.
     """
     p = OptionParser(pasteprepare.__doc__)
-    p.add_option(
+    p.add_argument(
         "--flank",
         default=5000,
-        type="int",
+        type=int,
         help="Get the seq of size on two ends",
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
@@ -234,21 +233,21 @@
     %prog paste flanks.bed flanks_vs_assembly.blast backbone.fasta
 
     Paste in good sequences in the final assembly.
     """
     from jcvi.formats.bed import uniq
 
     p = OptionParser(paste.__doc__)
-    p.add_option(
+    p.add_argument(
         "--maxsize",
         default=300000,
-        type="int",
+        type=int,
         help="Maximum size of patchers to be replaced",
     )
-    p.add_option("--prefix", help="Prefix of the new object")
+    p.add_argument("--prefix", help="Prefix of the new object")
     p.set_rclip(rclip=1)
     opts, args = p.parse_args(args)
 
     if len(args) != 3:
         sys.exit(not p.print_help())
 
     pbed, blastfile, bbfasta = args
@@ -294,15 +293,15 @@
 def closest(args):
     """
     %prog closest candidates.bed gaps.bed fastafile
 
     Identify the nearest gaps flanking suggested regions.
     """
     p = OptionParser(closest.__doc__)
-    p.add_option(
+    p.add_argument(
         "--om",
         default=False,
         action="store_true",
         help="The bedfile is OM blocks",
     )
     opts, args = p.parse_args(args)
 
@@ -512,18 +511,18 @@
 def fill(args):
     """
     %prog fill gaps.bed bad.fasta
 
     Perform gap filling of one assembly (bad) using sequences from another.
     """
     p = OptionParser(fill.__doc__)
-    p.add_option(
+    p.add_argument(
         "--extend",
         default=2000,
-        type="int",
+        type=int,
         help="Extend seq flanking the gaps",
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
@@ -726,22 +725,22 @@
     jcvi.formats.agp.frombed().
     """
     from jcvi.apps.align import blast
     from jcvi.formats.fasta import SeqIO
 
     p = OptionParser(install.__doc__)
     p.set_rclip(rclip=1)
-    p.add_option(
+    p.add_argument(
         "--maxsize",
         default=300000,
-        type="int",
+        type=int,
         help="Maximum size of patchers to be replaced",
     )
-    p.add_option("--prefix", help="Prefix of the new object")
-    p.add_option(
+    p.add_argument("--prefix", help="Prefix of the new object")
+    p.add_argument(
         "--strict",
         default=False,
         action="store_true",
         help="Only update if replacement has no gaps",
     )
     opts, args = p.parse_args(args)
 
@@ -775,15 +774,15 @@
 
         elif bn < an:
             continue
 
         id = arec.id
         exclude.add(id)
 
-    logging.debug(
+    logger.debug(
         "Ignore {0} updates because of decreasing quality.".format(len(exclude))
     )
 
     abed = Bed(beforebed, sorted=False)
     bbed = Bed(afterbed, sorted=False)
     abed = [x for x in abed if x.accn not in exclude]
     bbed = [x for x in bbed if x.accn not in exclude]
@@ -810,29 +809,29 @@
     For breakpoint regions with no gaps, there are two options:
     - Break in the middle of the region
     - Break at the closest gap (--closest)
     """
     from pybedtools import BedTool
 
     p = OptionParser(refine.__doc__)
-    p.add_option(
+    p.add_argument(
         "--closest",
         default=False,
         action="store_true",
         help="In case of no gaps, use closest",
     )
     p.set_outfile("auto")
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     breakpointsbed, gapsbed = args
     ncols = len(next(open(breakpointsbed)).split())
-    logging.debug("File %s contains %d columns.", breakpointsbed, ncols)
+    logger.debug("File %s contains %d columns.", breakpointsbed, ncols)
     a = BedTool(breakpointsbed)
     b = BedTool(gapsbed)
     o = a.intersect(b, wao=True)
 
     pf = "{0}.{1}".format(
         op.basename(breakpointsbed).split(".")[0], op.basename(gapsbed).split(".")[0]
     )
@@ -888,15 +887,15 @@
 def merge_ranges(beds):
 
     m = [x.accn for x in beds]
 
     mr = [range_parse(x) for x in m]
     mc = set(x.seqid for x in mr)
     if len(mc) != 1:
-        logging.error("Multiple seqid found in pocket. Aborted.")
+        logger.error("Multiple seqid found in pocket. Aborted.")
         return
 
     mc = list(mc)[0]
     ms = min(x.start for x in mr)
     me = max(x.end for x in mr)
 
     neg_strands = sum(1 for x in beds if x.strand == "-")
@@ -913,20 +912,20 @@
     Given optical map alignment, prepare the patchers. Use --backbone to suggest
     which assembly is the major one, and the patchers will be extracted from
     another assembly.
     """
     from jcvi.formats.bed import uniq
 
     p = OptionParser(patcher.__doc__)
-    p.add_option(
+    p.add_argument(
         "--backbone",
         default="OM",
         help="Prefix of the backbone assembly",
     )
-    p.add_option("--object", default="object", help="New object name")
+    p.add_argument("--object", default="object", help="New object name")
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     backbonebed, otherbed = args
     backbonebed = uniq([backbonebed])
```

### Comparing `jcvi-1.4.6/jcvi/assembly/postprocess.py` & `jcvi-1.4.7/jcvi/assembly/postprocess.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,43 +8,44 @@
 + BLAST against the Illumina contigs to fish out additional seqs
 + Use minimus2 to combine the contigs through overlaps
 + Map the mates to the contigs and perform scaffolding
 """
 import os
 import os.path as op
 import sys
-import logging
 
 from collections import defaultdict
 from itertools import groupby
 
-from jcvi.formats.contig import ContigFile
-from jcvi.formats.fasta import (
+from ..apps.align import run_megablast
+from ..apps.base import (
+    ActionDispatcher,
+    OptionParser,
+    cleanup,
+    logger,
+    mkdir,
+    need_update,
+    sh,
+)
+from ..formats.base import must_open
+from ..formats.contig import ContigFile
+from ..formats.fasta import (
     Fasta,
     Seq,
     SeqIO,
     SeqRecord,
-    gaps,
     format,
+    gaps,
     parse_fasta,
     tidy,
 )
-from jcvi.formats.sizes import Sizes
-from jcvi.formats.base import must_open
-from jcvi.utils.cbook import depends
-from jcvi.assembly.base import n50
-from jcvi.apps.align import run_megablast
-from jcvi.apps.base import (
-    OptionParser,
-    ActionDispatcher,
-    cleanup,
-    mkdir,
-    need_update,
-    sh,
-)
+from ..formats.sizes import Sizes
+from ..utils.cbook import depends
+
+from .base import n50
 
 
 def main():
 
     actions = (
         ("screen", "screen sequences against library"),
         ("circular", "make circular genome"),
@@ -89,15 +90,15 @@
         header = header.strip(">")
         for b in block:
             start, end = b.split(" - ")
             start, end = int(start), int(end)
             print("\t".join(str(x) for x in (header, start, end)), file=fw)
             nlines += 1
             nbases += end - start
-    logging.debug(
+    logger.debug(
         "A total of {0} DUST intervals ({1} bp) exported to `{2}`".format(
             nlines, nbases, bedfile
         )
     )
 
 
 def fasta2bed(fastafile):
@@ -122,15 +123,15 @@
     Make circular genome, startpos is the place to start the sequence. This can
     be determined by mapping to a reference. Self overlaps are then resolved.
     Startpos is 1-based.
     """
     from jcvi.assembly.goldenpath import overlap
 
     p = OptionParser(circular.__doc__)
-    p.add_option(
+    p.add_argument(
         "--flip",
         default=False,
         action="store_true",
         help="Reverse complement the sequence",
     )
     p.set_outfile()
     opts, args = p.parse_args(args)
@@ -242,15 +243,15 @@
     7. Rename the contigs sequentially
     """
     from jcvi.apps.cdhit import deduplicate
     from jcvi.apps.vecscreen import mask
     from jcvi.formats.fasta import sort
 
     p = OptionParser(build.__doc__)
-    p.add_option(
+    p.add_argument(
         "--nodedup",
         default=False,
         action="store_true",
         help="Do not deduplicate [default: deduplicate]",
     )
     opts, args = p.parse_args(args)
 
@@ -279,15 +280,15 @@
     cov will be removed by default.
     """
     from jcvi.apps.align import blast
     from jcvi.formats.blast import covfilter
 
     p = OptionParser(screen.__doc__)
     p.set_align(pctid=95, pctcov=50)
-    p.add_option("--best", default=1, type="int", help="Get the best N hit")
+    p.add_argument("--best", default=1, type=int, help="Get the best N hit")
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     scaffolds, library = args
     pctidflag = "--pctid={0}".format(opts.pctid)
@@ -305,30 +306,30 @@
     )
 
     pf = scaffolds.rsplit(".", 1)[0]
     nf = pf + ".screen.fasta"
     cmd = "faSomeRecords {0} -exclude {1} {2}".format(scaffolds, idsfile, nf)
     sh(cmd)
 
-    logging.debug("Screened FASTA written to `{0}`.".format(nf))
+    logger.debug("Screened FASTA written to `{0}`.".format(nf))
 
     return nf
 
 
 def scaffold(args):
     """
     %prog scaffold ctgfasta agpfile
 
     Build scaffolds based on ordering in the AGP file.
     """
     from jcvi.formats.agp import bed, order_to_agp, build
     from jcvi.formats.bed import Bed
 
     p = OptionParser(scaffold.__doc__)
-    p.add_option(
+    p.add_argument(
         "--prefix",
         default=False,
         action="store_true",
         help="Keep IDs with same prefix together",
     )
     opts, args = p.parse_args(args)
 
@@ -488,30 +489,30 @@
     c = ContigFile(minimuscontig)
     excludecontigs = set()
     for rec in c.iter_records():
         reads = set(x.id for x in rec.reads)
         if reads.isdisjoint(originalIDs):
             excludecontigs.add(rec.id)
 
-    logging.debug("Exclude contigs: {0}".format(", ".join(sorted(excludecontigs))))
+    logger.debug("Exclude contigs: {0}".format(", ".join(sorted(excludecontigs))))
 
     finalfasta = prefix + ".improved.fasta_"
     fw = open(finalfasta, "w")
     minimusfasta = op.join(closuredir, prefix + ".fasta")
     f = Fasta(minimusfasta)
     for id, rec in f.iteritems_ordered():
         if id in excludecontigs:
             continue
         SeqIO.write([rec], fw, "fasta")
 
     singletonfile = op.join(closuredir, prefix + ".singletons")
     singletons = set(x.strip() for x in open(singletonfile))
     leftovers = singletons & originalIDs
 
-    logging.debug("Pull leftover singletons: {0}".format(", ".join(sorted(leftovers))))
+    logger.debug("Pull leftover singletons: {0}".format(", ".join(sorted(leftovers))))
 
     f = Fasta(ctgfasta)
     for id, rec in f.iteritems_ordered():
         if id not in leftovers:
             continue
         SeqIO.write([rec], fw, "fasta")
 
@@ -519,15 +520,15 @@
 
     fastafile = finalfasta
     finalfasta = fastafile.rstrip("_")
     format(
         [fastafile, finalfasta, "--sequential", "--pad0=3", "--prefix={0}_".format(rid)]
     )
 
-    logging.debug("Improved FASTA written to `{0}`.".format(finalfasta))
+    logger.debug("Improved FASTA written to `{0}`.".format(finalfasta))
 
     n50([ctgfasta])
     n50([finalfasta])
 
     errlog = "error.log"
     cleanup(fastafile, blastfile, errlog)
```

### Comparing `jcvi-1.4.6/jcvi/assembly/preprocess.py` & `jcvi-1.4.7/jcvi/assembly/preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 Wrapper to trim and correct sequence data.
 """
 import os
 import os.path as op
 import sys
 
 from ..apps.base import (
-    OptionParser,
     ActionDispatcher,
+    OptionParser,
     cleanup,
     datadir,
     download,
     logger,
     mkdir,
     need_update,
     sh,
@@ -96,19 +96,19 @@
     $ make test
     $ export PYTHONPATH=~/export/khmer
     """
     from jcvi.formats.fastq import shuffle, pairinplace, split
     from jcvi.apps.base import getfilesize
 
     p = OptionParser(diginorm.__doc__)
-    p.add_option(
+    p.add_argument(
         "--single", default=False, action="store_true", help="Single end reads"
     )
-    p.add_option("--tablesize", help="Memory size")
-    p.add_option(
+    p.add_argument("--tablesize", help="Memory size")
+    p.add_argument(
         "--npass",
         default="1",
         choices=("1", "2"),
         help="How many passes of normalization",
     )
     p.set_depth(depth=50)
     p.set_home("khmer", default="/usr/local/bin/")
@@ -305,16 +305,16 @@
 
     Count reads based on FASTQC results. FASTQC needs to be run on all the input
     data given before running this command.
     """
     from jcvi.utils.table import loadtable, write_csv
 
     p = OptionParser(count.__doc__)
-    p.add_option("--dir", help="Sub-directory where FASTQC was run")
-    p.add_option(
+    p.add_argument("--dir", help="Sub-directory where FASTQC was run")
+    p.add_argument(
         "--human",
         default=False,
         action="store_true",
         help="Human friendly numbers",
     )
     p.set_table()
     p.set_outfile()
@@ -349,17 +349,17 @@
     Wrapper against het-smooth. Below is the command used in het-smooth manual.
 
     $ het-smooth --kmer-len=23 --bottom-threshold=38 --top-threshold=220
            --no-multibase-replacements --jellyfish-hash-file=23-mers.jf
                reads_1.fq reads_2.fq
     """
     p = OptionParser(hetsmooth.__doc__)
-    p.add_option("-K", default=23, type="int", help="K-mer size")
-    p.add_option("-L", type="int", help="Bottom threshold, first min")
-    p.add_option("-U", type="int", help="Top threshold, second min")
+    p.add_argument("-K", default=23, type=int, help="K-mer size")
+    p.add_argument("-L", type=int, help="Bottom threshold, first min")
+    p.add_argument("-U", type=int, help="Top threshold, second min")
     opts, args = p.parse_args(args)
 
     if len(args) != 3:
         sys.exit(not p.print_help())
 
     reads1fq, reads2fq, jfdb = args
     K = opts.K
@@ -385,51 +385,51 @@
     the paired reads mode. See manual:
 
     <http://www.usadellab.org/cms/index.php?page=trimmomatic>
     """
     tv = "0.32"
     TrimJar = "trimmomatic-{0}.jar".format(tv)
     p = OptionParser(trim.__doc__)
-    p.add_option(
+    p.add_argument(
         "--path",
         default=op.join("~/bin", TrimJar),
         help="Path to trimmomatic jar file",
     )
     p.set_phred()
-    p.add_option(
+    p.add_argument(
         "--nofrags",
         default=False,
         action="store_true",
         help="Discard frags file in PE mode",
     )
-    p.add_option(
+    p.add_argument(
         "--minqv",
         default=15,
-        type="int",
+        type=int,
         help="Average qv after trimming",
     )
-    p.add_option(
+    p.add_argument(
         "--minlen",
         default=36,
-        type="int",
+        type=int,
         help="Minimum length after trimming",
     )
-    p.add_option(
+    p.add_argument(
         "--adapteronly",
         default=False,
         action="store_true",
         help="Only trim adapters with no qv trimming",
     )
-    p.add_option(
+    p.add_argument(
         "--nogz",
         default=False,
         action="store_true",
         help="Do not write to gzipped files",
     )
-    p.add_option(
+    p.add_argument(
         "--log",
         default=None,
         dest="trimlog",
         help="Specify a `trimlog` file",
     )
     p.set_cpus(cpus=4)
     opts, args = p.parse_args(args)
@@ -579,29 +579,29 @@
     reads, and results will be placed in `frag_reads.corr.{pairs,frags}.fastq`
     and `jump_reads.corr.{pairs,frags}.fastq`.
     """
     from jcvi.assembly.allpaths import prepare
     from jcvi.assembly.base import FastqNamings
 
     p = OptionParser(correct.__doc__ + FastqNamings)
-    p.add_option("--dir", default="data", help="Working directory")
-    p.add_option(
+    p.add_argument("--dir", default="data", help="Working directory")
+    p.add_argument(
         "--fragsdedup",
         default=False,
         action="store_true",
         help="Don't deduplicate the fragment reads",
     )
-    p.add_option("--ploidy", default="2", choices=("1", "2"), help="Ploidy")
-    p.add_option(
+    p.add_argument("--ploidy", default="2", choices=("1", "2"), help="Ploidy")
+    p.add_argument(
         "--haploidify",
         default=False,
         action="store_true",
         help="Set HAPLOIDIFY=True",
     )
-    p.add_option(
+    p.add_argument(
         "--suffix",
         default=False,
         action="store_true",
         help="Add suffix /1, /2 to read names",
     )
     p.set_cpus()
     opts, args = p.parse_args(args)
```

### Comparing `jcvi-1.4.6/jcvi/assembly/sim.py` & `jcvi-1.4.7/jcvi/assembly/sim.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 """
 Simulate Illumina sequencing reads.
 """
+import math
 import os
 import os.path as op
 import random
 import sys
-import logging
-import math
 
-from jcvi.formats.fasta import Fasta
-from jcvi.apps.base import ActionDispatcher, OptionParser, cleanup, sh
+from ..apps.base import ActionDispatcher, OptionParser, cleanup, logger, sh
+from ..formats.fasta import Fasta
 
 
 def main():
 
     actions = (
         ("wgsim", "sample paired end reads using dwgsim"),
         ("eagle", "simulate Illumina reads using EAGLE"),
@@ -25,32 +24,32 @@
     p.dispatch(globals())
 
 
 def add_sim_options(p):
     """
     Add options shared by eagle or wgsim.
     """
-    p.add_option(
+    p.add_argument(
         "--distance",
         default=500,
-        type="int",
+        type=int,
         help="Outer distance between the two ends",
     )
-    p.add_option("--readlen", default=150, type="int", help="Length of the read")
+    p.add_argument("--readlen", default=150, type=int, help="Length of the read")
     p.set_depth(depth=10)
     p.set_outfile(outfile=None)
 
 
 def eagle(args):
     """
     %prog eagle fastafile
 
     """
     p = OptionParser(eagle.__doc__)
-    p.add_option(
+    p.add_argument(
         "--share", default="/usr/local/share/EAGLE/", help="Default EAGLE share path"
     )
     add_sim_options(p)
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
@@ -154,29 +153,29 @@
 def wgsim(args):
     """
     %prog wgsim fastafile
 
     Run dwgsim on fastafile.
     """
     p = OptionParser(wgsim.__doc__)
-    p.add_option(
+    p.add_argument(
         "--erate",
         default=0.01,
-        type="float",
+        type=float,
         help="Base error rate of the read",
     )
-    p.add_option(
+    p.add_argument(
         "--noerrors",
         default=False,
         action="store_true",
         help="Simulate reads with no errors",
     )
-    p.add_option(
+    p.add_argument(
         "--genomesize",
-        type="int",
+        type=int,
         help="Genome size in Mb [default: estimate from data]",
     )
     add_sim_options(p)
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
@@ -191,17 +190,17 @@
     readnum = int(math.ceil(size * depth / (2 * readlen)))
 
     distance = opts.distance
     stdev = distance / 10
 
     outpf = opts.outfile or "{0}.{1}bp.{2}x".format(pf, distance, depth)
 
-    logging.debug("Total genome size: {0} bp".format(size))
-    logging.debug("Target depth: {0}x".format(depth))
-    logging.debug("Number of read pairs (2x{0}): {1}".format(readlen, readnum))
+    logger.debug("Total genome size: {0} bp".format(size))
+    logger.debug("Target depth: {0}x".format(depth))
+    logger.debug("Number of read pairs (2x{0}): {1}".format(readlen, readnum))
 
     if opts.noerrors:
         opts.erate = 0
 
     cmd = "dwgsim -e {0} -E {0}".format(opts.erate)
     if opts.noerrors:
         cmd += " -r 0 -R 0 -X 0 -y 0"
```

### Comparing `jcvi-1.4.6/jcvi/assembly/soap.py` & `jcvi-1.4.7/jcvi/assembly/soap.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,16 +131,16 @@
 def clean(args):
     """
     %prog clean 1.fastq 2.fastq [insertsize]
 
     Clean and dedup paired FASTQ files.
     """
     p = OptionParser(clean.__doc__)
-    p.add_option("-a", default=0, type="int", help="Trim length at 5' end")
-    p.add_option("-b", default=50, type="int", help="Trim length at 3' end")
+    p.add_argument("-a", default=0, type=int, help="Trim length at 5' end")
+    p.add_argument("-b", default=50, type=int, help="Trim length at 3' end")
     p.set_cpus()
     opts, args = p.parse_args(args)
 
     if len(args) == 2:
         p1, p2 = args
         size = get_size(p1)
     elif len(args) == 3:
@@ -229,23 +229,23 @@
 
     Scan input fastq files (see below) and write SOAP config files based
     on inputfiles. Use "--scaffold contigs.fasta" to perform scaffolding.
     """
     from jcvi.formats.base import write_file
 
     p = OptionParser(prepare.__doc__ + FastqNamings)
-    p.add_option("-K", default=45, type="int", help="K-mer size")
-    p.add_option(
+    p.add_argument("-K", default=45, type=int, help="K-mer size")
+    p.add_argument(
         "--assemble_1st_rank_only",
         default=False,
         action="store_true",
         help="Assemble the first rank only, other libs asm_flags=2",
     )
-    p.add_option("--scaffold", help="Only perform scaffolding")
-    p.add_option("--gapclose", help="Only perform gap closure")
+    p.add_argument("--scaffold", help="Only perform scaffolding")
+    p.add_argument("--gapclose", help="Only perform gap closure")
     p.set_cpus()
     opts, args = p.parse_args(args)
 
     if len(args) < 1:
         sys.exit(not p.print_help())
 
     fnames = args
```

### Comparing `jcvi-1.4.6/jcvi/assembly/syntenypath.py` & `jcvi-1.4.7/jcvi/assembly/syntenypath.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 """
 Syntenic path assembly.
 """
 import sys
-import logging
 
 from collections import defaultdict
 from itertools import groupby, combinations
 from more_itertools import pairwise
 
-from jcvi.formats.blast import BlastSlow, Blast
-from jcvi.formats.sizes import Sizes
-from jcvi.formats.base import LineFile, must_open
-from jcvi.utils.range import range_intersect
-from jcvi.algorithms.graph import BiGraph
-from jcvi.apps.base import OptionParser, ActionDispatcher
+from ..algorithms.graph import BiGraph
+from ..apps.base import ActionDispatcher, OptionParser, logger
+from ..formats.base import LineFile, must_open
+from ..formats.blast import Blast, BlastSlow
+from ..formats.sizes import Sizes
+from ..utils.range import range_intersect
 
 
 class OVLLine:
     def __init__(self, row):
         # tig00000004     tig00042923     I       -64039  -18713  16592   99.84
         # See also: assembly.goldenpath.Overlap for another implementation
         args = row.split()
@@ -56,20 +55,20 @@
                 contained.add(o.a)
             elif o.tag == "b in a":
                 contained.add(o.b)
             if o.tag == "a->b":
                 alledges[o.a + "-3`"].append(o)
             elif o.tag == "b->a":
                 alledges[o.a + "-5`"].append(o)
-        logging.debug(
+        logger.debug(
             "Imported {} links. Contained tigs: {}".format(len(self), len(contained))
         )
         self.contained = contained
 
-        logging.debug("Pruning edges to keep the mutual best")
+        logger.debug("Pruning edges to keep the mutual best")
         for k, v in alledges.items():
             bo = max(v, key=lambda x: x.score)
             bo.best = True
 
         self.graph = BiGraph()
         for o in self:
             if not o.best:
@@ -130,22 +129,22 @@
     from collections import defaultdict
     from jcvi.compara.synteny import check_beds
     from jcvi.formats.bed import Bed
     from jcvi.formats.base import get_number
     from ..compara.base import AnchorFile
 
     p = OptionParser(bed.__doc__)
-    p.add_option(
+    p.add_argument(
         "--switch",
         default=False,
         action="store_true",
         help="Switch reference and aligned map elements",
     )
-    p.add_option(
-        "--scale", type="float", help="Scale the aligned map distance by factor"
+    p.add_argument(
+        "--scale", type=float, help="Scale the aligned map distance by factor"
     )
     p.set_beds()
     p.set_outfile()
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
@@ -226,22 +225,22 @@
     %prog partition happy.txt synteny.graph
 
     Select edges from another graph and merge it with the certain edges built
     from the HAPPY mapping data.
     """
     allowed_format = ("png", "ps")
     p = OptionParser(partition.__doc__)
-    p.add_option("--prefix", help="Add prefix to the name")
-    p.add_option(
+    p.add_argument("--prefix", help="Add prefix to the name")
+    p.add_argument(
         "--namestart",
         default=0,
-        type="int",
+        type=int,
         help="Use a shorter name, starting index",
     )
-    p.add_option(
+    p.add_argument(
         "--format",
         default="png",
         choices=allowed_format,
         help="Generate image of format",
     )
     opts, args = p.parse_args(args)
 
@@ -295,15 +294,15 @@
 def merge(args):
     """
     %prog merge graphs
 
     Merge multiple graphs together and visualize.
     """
     p = OptionParser(merge.__doc__)
-    p.add_option(
+    p.add_argument(
         "--colorlist",
         default="black,red,pink,blue,green",
         help="The color palette",
     )
     opts, args = p.parse_args(args)
 
     if len(args) < 1:
@@ -337,15 +336,15 @@
     ( ) means uncertain orientation. small chance of error (90% confidence?)
     { } means uncertain order.
 
     Example:
     +-8254707:8254647:-8254690:{[8254694]:[8254713]:[8254531]:[8254797]}:8254802:8254788+
     """
     p = OptionParser(happy.__doc__)
-    p.add_option("--prefix", help="Add prefix to the name")
+    p.add_argument("--prefix", help="Add prefix to the name")
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (happyfile,) = args
 
@@ -356,15 +355,15 @@
 
     fp = open(happyfile)
     for row in fp:
         for e, is_uncertain in happy_edges(row, prefix=opts.prefix):
             fw = fw2 if is_uncertain else fw1
             print(e, file=fw)
 
-    logging.debug("Edges written to `{0}`".format(",".join((certain, uncertain))))
+    logger.debug("Edges written to `{0}`".format(",".join((certain, uncertain))))
 
 
 def fromblast(args):
     """
     %prog fromblast blastfile subject.fasta
 
     Generate path from BLAST file. If multiple subjects map to the same query,
@@ -372,24 +371,24 @@
 
     The BLAST file MUST be filtered, chained, supermapped.
     """
     from jcvi.formats.blast import sort
     from jcvi.utils.range import range_distance
 
     p = OptionParser(fromblast.__doc__)
-    p.add_option(
+    p.add_argument(
         "--clique",
         default=False,
         action="store_true",
         help="Populate clique instead of linear path",
     )
-    p.add_option(
+    p.add_argument(
         "--maxdist",
         default=100000,
-        type="int",
+        type=int,
         help="Create edge within certain distance",
     )
     p.set_verbose(help="Print verbose reports to stdout")
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
@@ -421,15 +420,15 @@
     graph_to_agp(g, blastfile, subjectfasta, verbose=opts.verbose)
 
 
 def graph_to_agp(g, blastfile, subjectfasta, exclude=[], verbose=False):
 
     from jcvi.formats.agp import order_to_agp
 
-    logging.debug(str(g))
+    logger.debug(str(g))
     g.write("graph.txt")
     # g.draw("graph.pdf")
 
     paths = []
     for path in g.iter_paths():
         m, oo = g.path(path)
         if len(oo) == 1:  # Singleton path
@@ -437,15 +436,15 @@
         paths.append(oo)
         if verbose:
             print(m)
             print(oo)
 
     npaths = len(paths)
     ntigs = sum(len(x) for x in paths)
-    logging.debug(
+    logger.debug(
         "Graph decomposed to {0} paths with {1} components.".format(npaths, ntigs)
     )
 
     agpfile = blastfile + ".agp"
     sizes = Sizes(subjectfasta)
     fwagp = open(agpfile, "w")
     scaffolded = set()
@@ -465,35 +464,35 @@
             nexcluded += 1
             continue
 
         ctgorder = [(ctg, "+")]
         object = ctg
         order_to_agp(object, ctgorder, sizes.mapping, fwagp)
         nsingletons += 1
-    logging.debug(
+    logger.debug(
         "scaffolded={} excluded={} singletons={}".format(
             nscaffolded, nexcluded, nsingletons
         )
     )
 
     fwagp.close()
-    logging.debug("AGP file written to `{0}`.".format(agpfile))
+    logger.debug("AGP file written to `{0}`.".format(agpfile))
 
 
 def connect(args):
     """
     %prog connect assembly.fasta read_mapping.blast
 
     Connect contigs using long reads.
     """
     p = OptionParser(connect.__doc__)
-    p.add_option(
+    p.add_argument(
         "--clip",
         default=2000,
-        type="int",
+        type=int,
         help="Only consider end of contigs",
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
```

### Comparing `jcvi-1.4.6/jcvi/compara/base.py` & `jcvi-1.4.7/jcvi/compara/base.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.6/jcvi/compara/blastfilter.py` & `jcvi-1.4.7/jcvi/compara/blastfilter.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,38 +16,37 @@
 
     cscore(A,B) = score(A,B) /
          max(best score for A, best score for B)
 
 Finally a blast.filtered file is created.
 """
 import sys
-import logging
 import os.path as op
 
 from collections import defaultdict
 from itertools import groupby
 
-from jcvi.formats.blast import Blast
-from jcvi.utils.grouper import Grouper
-from jcvi.utils.cbook import gene_name
-from jcvi.compara.synteny import check_beds
-from jcvi.apps.base import OptionParser
+from ..apps.base import OptionParser, logger
+from ..compara.synteny import check_beds
+from ..formats.blast import Blast
+from ..utils.cbook import gene_name
+from ..utils.grouper import Grouper
 
 
 def blastfilter_main(blast_file, p, opts):
 
     qbed, sbed, qorder, sorder, is_self = check_beds(blast_file, p, opts)
 
     tandem_Nmax = opts.tandem_Nmax
     cscore = opts.cscore
     exclude = opts.exclude
 
     fp = open(blast_file)
     total_lines = sum(1 for line in fp if line[0] != "#")
-    logging.debug(
+    logger.debug(
         "Load BLAST file `{}` (total {} lines)".format(blast_file, total_lines)
     )
     bl = Blast(blast_file)
     blasts = sorted(list(bl), key=lambda b: b.score, reverse=True)
 
     filtered_blasts = []
     seen = set()
@@ -58,24 +57,24 @@
         if query == subject:
             continue
 
         if ostrip:
             query, subject = gene_name(query), gene_name(subject)
         if query not in qorder:
             if nwarnings < 100:
-                logging.warning("{} not in {}".format(query, qbed.filename))
+                logger.warning("{} not in {}".format(query, qbed.filename))
             elif nwarnings == 100:
-                logging.warning("too many warnings.. suppressed")
+                logger.warning("too many warnings.. suppressed")
             nwarnings += 1
             continue
         if subject not in sorder:
             if nwarnings < 100:
-                logging.warning("{} not in {}".format(subject, sbed.filename))
+                logger.warning("{} not in {}".format(subject, sbed.filename))
             elif nwarnings == 100:
-                logging.warning("too many warnings.. suppressed")
+                logger.warning("too many warnings.. suppressed")
             nwarnings += 1
             continue
 
         qi, q = qorder[query]
         si, s = sorder[subject]
 
         if is_self and qi > si:
@@ -93,30 +92,30 @@
         b.qi, b.si = qi, si
         b.qseqid, b.sseqid = q.seqid, s.seqid
 
         filtered_blasts.append(b)
 
     if exclude:
         before_filter = len(filtered_blasts)
-        logging.debug("running excluded pairs (--exclude `{}`) ..".format(exclude))
+        logger.debug("running excluded pairs (--exclude `{}`) ..".format(exclude))
         filtered_blasts = list(filter_exclude(filtered_blasts, exclude=exclude))
-        logging.debug(
+        logger.debug(
             "after filter ({}->{}) ..".format(before_filter, len(filtered_blasts))
         )
 
     if cscore:
         before_filter = len(filtered_blasts)
-        logging.debug("running the cscore filter (cscore>=%.2f) .." % cscore)
+        logger.debug("running the cscore filter (cscore>=%.2f) .." % cscore)
         filtered_blasts = list(filter_cscore(filtered_blasts, cscore=cscore))
-        logging.debug(
+        logger.debug(
             "after filter ({}->{}) ..".format(before_filter, len(filtered_blasts))
         )
 
     if tandem_Nmax:
-        logging.debug(
+        logger.debug(
             "running the local dups filter (tandem_Nmax={}) ..".format(tandem_Nmax)
         )
 
         qtandems = tandem_grouper(filtered_blasts, flip=True, tandem_Nmax=tandem_Nmax)
         standems = tandem_grouper(filtered_blasts, flip=False, tandem_Nmax=tandem_Nmax)
 
         qdups_fh = (
@@ -148,15 +147,15 @@
             # just want to use this script as a tandem finder.
             # sys.exit()
 
         before_filter = len(filtered_blasts)
         filtered_blasts = list(
             filter_tandem(filtered_blasts, qdups_to_mother, sdups_to_mother)
         )
-        logging.debug(
+        logger.debug(
             "after filter ({}->{}) ..".format(before_filter, len(filtered_blasts))
         )
 
     blastfilteredfile = blast_file + ".filtered"
     fw = open(blastfilteredfile, "w")
     write_new_blast(filtered_blasts, fh=fw)
     fw.close()
@@ -174,26 +173,26 @@
     dups_to_mother = {}
     n = 1
     for accns in sorted(tandem_groups):
         if dups_fh:
             print("\t".join(accns), file=dups_fh)
             if n:
                 n -= 1
-                logging.debug("write local dups to file {}".format(dups_fh.name))
+                logger.debug("write local dups to file {}".format(dups_fh.name))
 
         for dup in accns[1:]:
             dups_to_mother[dup] = accns[0]
 
     return dups_to_mother
 
 
 def write_new_bed(bed, children):
     # generate local dup removed annotation files
     out_name = "%s.nolocaldups%s" % op.splitext(bed.filename)
-    logging.debug("write tandem-filtered bed file %s" % out_name)
+    logger.debug("write tandem-filtered bed file %s" % out_name)
     fh = open(out_name, "w")
     for i, row in enumerate(bed):
         if row["accn"] in children:
             continue
         print(row, file=fh)
     fh.close()
 
@@ -286,36 +285,36 @@
 
 
 def main(args):
 
     p = OptionParser(__doc__)
     p.set_beds()
     p.set_stripnames()
-    p.add_option(
+    p.add_argument(
         "--tandems_only",
         dest="tandems_only",
         action="store_true",
         default=False,
         help="only calculate tandems, write .localdup file and exit.",
     )
-    p.add_option(
+    p.add_argument(
         "--tandem_Nmax",
-        type="int",
+        type=int,
         default=10,
         help="merge tandem genes within distance",
     )
-    p.add_option(
+    p.add_argument(
         "--cscore",
-        type="float",
+        type=float,
         default=0.7,
         help="retain hits that have good bitscore. a value of 0.5 means "
         "keep all values that are 50% or greater of the best hit. "
         "higher is more stringent",
     )
-    p.add_option("--exclude", help="Remove anchors from a previous run")
+    p.add_argument("--exclude", help="Remove anchors from a previous run")
 
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (blastfile,) = args
```

### Comparing `jcvi-1.4.6/jcvi/compara/catalog.py` & `jcvi-1.4.7/jcvi/compara/catalog.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 def enrich(args):
     """
     %prog enrich omgfile groups ntaxa > enriched.omg
 
     Enrich OMG output by pulling genes misses by OMG.
     """
     p = OptionParser(enrich.__doc__)
-    p.add_option(
+    p.add_argument(
         "--ghost",
         default=False,
         action="store_true",
         help="Add ghost homologs already used",
     )
     opts, args = p.parse_args(args)
 
@@ -305,15 +305,15 @@
     """
     %prog layout omgfile taxa
 
     Build column formatted gene lists after omgparse(). Use species list
     separated by comma in place of taxa, e.g. "BR,BO,AN,CN"
     """
     p = OptionParser(layout.__doc__)
-    p.add_option("--sort", help="Sort layout file based on bedfile")
+    p.add_argument("--sort", help="Sort layout file based on bedfile")
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     omgfile, taxa = args
     listfile = omgfile.rsplit(".", 1)[0] + ".list"
@@ -504,19 +504,19 @@
 
     Prepare to run Sankoff's OMG algorithm to get orthologs.
     """
     from jcvi.formats.blast import cscore
     from jcvi.formats.base import DictFile
 
     p = OptionParser(omgprepare.__doc__)
-    p.add_option("--norbh", action="store_true", help="Disable RBH hits")
-    p.add_option(
-        "--pctid", default=0, type="int", help="Percent id cutoff for RBH hits"
+    p.add_argument("--norbh", action="store_true", help="Disable RBH hits")
+    p.add_argument(
+        "--pctid", default=0, type=int, help="Percent id cutoff for RBH hits"
     )
-    p.add_option("--cscore", default=90, type="int", help="C-score cutoff for RBH hits")
+    p.add_argument("--cscore", default=90, type=int, help="C-score cutoff for RBH hits")
     p.set_stripnames()
     p.set_beds()
 
     opts, args = p.parse_args(args)
 
     if len(args) != 3:
         sys.exit(not p.print_help())
@@ -607,74 +607,74 @@
     from jcvi.apps.align import diamond_blastp_main, blast_main
     from jcvi.compara.blastfilter import main as blastfilter_main
     from jcvi.compara.quota import main as quota_main
     from jcvi.compara.synteny import scan, mcscan, liftover
     from jcvi.formats.blast import cscore, filter, filtered_blastfile_name
 
     p = OptionParser(ortholog.__doc__)
-    p.add_option(
+    p.add_argument(
         "--dbtype",
         default="nucl",
         choices=("nucl", "prot"),
         help="Molecule type of subject database",
     )
 
-    p.add_option(
+    p.add_argument(
         "--full",
         default=False,
         action="store_true",
         help="Run in full 1x1 mode, including blocks and RBH",
     )
-    p.add_option("--cscore", default=0.7, type="float", help="C-score cutoff")
-    p.add_option(
-        "--dist", default=20, type="int", help="Extent of flanking regions to search"
+    p.add_argument("--cscore", default=0.7, type=float, help="C-score cutoff")
+    p.add_argument(
+        "--dist", default=20, type=int, help="Extent of flanking regions to search"
     )
-    p.add_option(
+    p.add_argument(
         "-n",
         "--min_size",
         dest="n",
-        type="int",
+        type=int,
         default=4,
         help="minimum number of anchors in a cluster",
     )
-    p.add_option("--quota", help="Quota align parameter")
-    p.add_option("--exclude", help="Remove anchors from a previous run")
-    p.add_option(
+    p.add_argument("--quota", help="Quota align parameter")
+    p.add_argument("--exclude", help="Remove anchors from a previous run")
+    p.add_argument(
         "--self_remove",
         default=98,
-        type="float",
+        type=float,
         help="Remove self hits that are above this percent identity",
     )
-    p.add_option(
+    p.add_argument(
         "--no_strip_names",
         default=False,
         action="store_true",
         help="Do not strip alternative splicing (e.g. At5g06540.1 -> At5g06540)",
     )
-    p.add_option(
+    p.add_argument(
         "--liftover_dist",
-        type="int",
+        type=int,
         help="Distance to extend from liftover. Defaults to half of --dist",
     )
     p.set_cpus()
     dotplot_group = p.set_dotplot_opts()
-    dotplot_group.add_option(
+    dotplot_group.add_argument(
         "--notex", default=False, action="store_true", help="Do not use tex"
     )
-    dotplot_group.add_option(
+    dotplot_group.add_argument(
         "--no_dotplot", default=False, action="store_true", help="Do not make dotplot"
     )
-    p.add_option(
+    p.add_argument(
         "--ignore_zero_anchor",
         default=False,
         action="store_true",
         help="Ignore this pair of ortholog identification instead of throwing an error when performing many pairs of cataloging.",
     )
 
-    p.add_option(
+    p.add_argument(
         "--align_soft",
         default="last",
         choices=("last", "blast", "diamond_blastp"),
         help="Sequence alignment software. Default <last> for both <nucl> and <prot>. Users could also use <blast> for both <nucl> and <prot>, or <diamond_blastp> for <prot>.",
     )
 
     opts, args = p.parse_args(args)
@@ -919,42 +919,42 @@
     Find tandem gene clusters that are separated by N genes, based on filtered
     blast_file by enforcing alignments between any two genes at least 50%
     (or user specified value) of either gene.
 
     pep_file can also be used in same manner.
     """
     p = OptionParser(tandem.__doc__)
-    p.add_option(
+    p.add_argument(
         "--tandem_Nmax",
         dest="tandem_Nmax",
-        type="int",
+        type=int,
         default=3,
         help="merge tandem genes within distance",
     )
-    p.add_option(
+    p.add_argument(
         "--percent_overlap",
-        type="int",
+        type=int,
         default=50,
         help="tandem genes have >=x% aligned sequence, x=0-100",
     )
     p.set_align(evalue=0.01)
-    p.add_option(
+    p.add_argument(
         "--not_self",
         default=False,
         action="store_true",
         help="provided is not self blast file",
     )
-    p.add_option(
+    p.add_argument(
         "--strip_gene_name",
         dest="sep",
-        type="string",
+        type=str,
         default=".",
         help="strip alternative splicing. Use None for no stripping.",
     )
-    p.add_option(
+    p.add_argument(
         "--genefamily",
         dest="genefam",
         action="store_true",
         help="compile gene families based on similarity",
     )
     p.set_outfile()
```

### Comparing `jcvi-1.4.6/jcvi/compara/fractionation.py` & `jcvi-1.4.7/jcvi/compara/fractionation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 """
 Catalog gene losses, and bites within genes.
 """
 import sys
-import logging
 
 from itertools import groupby
 
-from jcvi.formats.blast import Blast
-from jcvi.formats.bed import Bed
-from jcvi.utils.range import range_minmax, range_overlap, range_distance
-from jcvi.utils.cbook import gene_name
-from jcvi.utils.grouper import Grouper
-from jcvi.compara.synteny import check_beds
-from jcvi.apps.base import OptionParser, ActionDispatcher, sh
+from ..apps.base import ActionDispatcher, OptionParser, logger, sh
+from ..formats.bed import Bed
+from ..formats.blast import Blast
+from ..utils.cbook import gene_name
+from ..utils.grouper import Grouper
+from ..utils.range import range_minmax, range_overlap, range_distance
+
+from .synteny import check_beds
 
 
 def main():
 
     actions = (
         # Identify true gene loss
         ("loss", "extract likely gene loss candidates"),
@@ -152,18 +152,18 @@
     - aggressive: extend the deletion track to the next gene
 
     The real deletion size is within these estimates.
     """
     from jcvi.formats.base import SetFile
 
     p = OptionParser(segment.__doc__)
-    p.add_option(
+    p.add_argument(
         "--chain",
         default=1,
-        type="int",
+        type=int,
         help="Allow next N genes to be chained",
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
@@ -335,30 +335,30 @@
             if bname in seen:
                 continue
             seen.add(bname)
             print(bbname, file=fw)
             cnt += 1
     fw.close()
 
-    logging.debug("Total {0} records written to `{1}`.".format(cnt, idsfile))
+    logger.debug("Total {0} records written to `{1}`.".format(cnt, idsfile))
 
 
 def gaps(args):
     """
     %prog gaps idsfile fractionationfile gapsbed
 
     Check gene locations against gaps. `idsfile` contains a list of IDs to query
     into `fractionationfile` in order to get expected locations.
     """
     from jcvi.formats.base import DictFile
     from jcvi.apps.base import popen
     from jcvi.utils.cbook import percentage
 
     p = OptionParser(gaps.__doc__)
-    p.add_option("--bdist", default=0, type="int", help="Base pair distance")
+    p.add_argument("--bdist", default=0, type=int, help="Base pair distance")
     opts, args = p.parse_args(args)
 
     if len(args) != 3:
         sys.exit(not p.print_help())
 
     idsfile, frfile, gapsbed = args
     bdist = opts.bdist
@@ -435,15 +435,15 @@
     Provide summary of fractionation. `fractionation` file is generated with
     loss(). `gmap.status` is generated with genestatus().
     """
     from jcvi.formats.base import DictFile
     from jcvi.utils.cbook import percentage, Registry
 
     p = OptionParser(summary.__doc__)
-    p.add_option("--extra", help="Cross with extra tsv file")
+    p.add_argument("--extra", help="Cross with extra tsv file")
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     frfile, statusfile = args
     status = DictFile(statusfile)
@@ -527,15 +527,15 @@
     fw = open("registry", "w")
     for row in fp:
         seqid, gene, tag = row.split()
         ts = registry[gene]
         print("\t".join((seqid, gene, tag, "-".join(ts))), file=fw)
     fw.close()
 
-    logging.debug("Registry written.")
+    logger.debug("Registry written.")
 
 
 def get_tag(name, order):
     if name[0] == "[":
         tag, tname = name[1:].split("]")
         seqid, se = tname.split(":")
         start, end = se.split("-")
@@ -606,15 +606,15 @@
                 row = row + "\t{0}|{1}".format(AL, br)
             if (antag, cntag) == (None, "NS"):
                 row = row + "\t{0}|{1}".format(CL, bo)
 
         print(row, file=fw)
     fw.close()
 
-    logging.debug("Quartets and gene losses written to `{0}`.".format(quartetsfile))
+    logger.debug("Quartets and gene losses written to `{0}`.".format(quartetsfile))
 
     # Parse the quartets file to extract singletons vs.segmental losses
     fp = open(quartetsfile)
     fw = open(quartetsfile + ".summary", "w")
     data = [x.rstrip().split("\t") for x in fp]
     skip = 1  # max distance between losses
 
@@ -646,16 +646,16 @@
 
     an_loss_segments = grab_tag(segments, AL)
     cn_loss_segments = grab_tag(segments, CL)
     alm, clm = len(an_loss_segments), len(cn_loss_segments)
     mixed = len(segments) - alm - clm
     assert mixed == 0
 
-    logging.debug("Singletons: {0} (AN LOSS: {1}, CN LOSS: {2})".format(ns, als, cls))
-    logging.debug("Segments: {0} (AN LOSS: {1}, CN LOSS: {2})".format(nm, alm, clm))
+    logger.debug("Singletons: {0} (AN LOSS: {1}, CN LOSS: {2})".format(ns, als, cls))
+    logger.debug("Segments: {0} (AN LOSS: {1}, CN LOSS: {2})".format(nm, alm, clm))
     print(SummaryStats([len(x) for x in losses]), file=sys.stderr)
 
     for x in singletons + segments:
         print("### LENGTH =", len(x), file=fw)
         for i in x:
             print("\t".join(data[i]), file=fw)
     fw.close()
@@ -668,25 +668,25 @@
 def loss(args):
     """
     %prog loss a.b.i1.blocks [a.b-genomic.blast]
 
     Extract likely gene loss candidates between genome a and b.
     """
     p = OptionParser(loss.__doc__)
-    p.add_option(
+    p.add_argument(
         "--bed",
         default=False,
         action="store_true",
         help="Genomic BLAST is in bed format",
     )
-    p.add_option("--gdist", default=20, type="int", help="Gene distance")
-    p.add_option(
+    p.add_argument("--gdist", default=20, type=int, help="Gene distance")
+    p.add_argument(
         "--bdist",
         default=20000,
-        type="int",
+        type=int,
         help="Base pair distance",
     )
     p.set_beds()
     opts, args = p.parse_args(args)
 
     if len(args) not in (1, 2):
         sys.exit(not p.print_help())
@@ -842,13 +842,13 @@
         if b in pairs:
             assert c.startswith("[S]")
             c = pairs[b]
             fixed += 1
 
         print("\t".join((a, b, c)), file=fw)
 
-    logging.debug("Fixed {0} [S] cases in `{1}`.".format(fixed, validated))
+    logger.debug("Fixed {0} [S] cases in `{1}`.".format(fixed, validated))
     fw.close()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `jcvi-1.4.6/jcvi/compara/ks.py` & `jcvi-1.4.7/jcvi/compara/ks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 """
 Calculation of synonymous substitutions (Ks).
 """
 import csv
-import logging
 import os
 import os.path as op
 import sys
+
 from functools import partial
 from itertools import combinations, product
 from math import exp, log, pi, sqrt
 from typing import Optional
 
 import numpy as np
+
 from Bio import AlignIO, SeqIO
 from Bio.Align.Applications import ClustalwCommandline, MuscleCommandline
 
-from jcvi.apps.base import (
+from ..apps.base import (
     ActionDispatcher,
     OptionParser,
     Popen,
     cleanup,
     getpath,
     iglob,
+    logger,
     mkdir,
     sh,
 )
-from jcvi.formats.base import LineFile, must_open
-from jcvi.graphics.base import AbstractLayout, adjust_spines, markup, plt, savefig
-from jcvi.utils.cbook import gene_name
-from jcvi.utils.table import write_csv
+from ..formats.base import LineFile, must_open
+from ..graphics.base import AbstractLayout, adjust_spines, markup, plt, savefig
+from ..utils.cbook import gene_name
+from ..utils.table import write_csv
 
 CLUSTALW_BIN = partial(getpath, name="CLUSTALW2", warn="warn")
 MUSCLE_BIN = partial(getpath, name="MUSCLE", warn="warn")
 PAL2NAL_BIN = partial(getpath, name="PAL2NAL", warn="warn")
 PAML_BIN = partial(getpath, name="PAML", warn="warn")
 
 
@@ -343,15 +345,15 @@
         title=cdsfile,
         bins=50,
         skip=0,
         ascii=False,
         fill=fill,
     )
 
-    logging.debug("{0} GC3 values plotted to {1}.pdf".format(len(GC3), numberfile))
+    logger.debug("{0} GC3 values plotted to {1}.pdf".format(len(GC3), numberfile))
 
 
 def gc3(args):
     """
     %prog gc3 ksfile cdsfile [cdsfile2] -o newksfile
 
     Filter the Ks results to remove high GC3 genes. High GC3 genes are
@@ -360,15 +362,15 @@
     pairs. Therefore we advise to remoeve these high GC3 genes. This is often
     the case for studying cereal genes.
 
     If 2 genomes are involved, the cdsfile of the 2nd genome can be provided
     concatenated or separated.
     """
     p = OptionParser(gc3.__doc__)
-    p.add_option(
+    p.add_argument(
         "--plot", default=False, action="store_true", help="Also plot the GC3 histogram"
     )
     p.set_outfile()
 
     opts, args = p.parse_args(args)
 
     outfile = opts.outfile
@@ -400,15 +402,15 @@
     for d in data:
         a, b = d.name.split(";")
         aratio, bratio = GC3[a], GC3[b]
         if (aratio + bratio) / 2 > cutoff:
             continue
         writer.writerow(d)
         nlines += 1
-    logging.debug("{0} records written (from {1}).".format(nlines, noriginals))
+    logger.debug("{0} records written (from {1}).".format(nlines, noriginals))
 
 
 def extract_pairs(abed, bbed, groups):
     """
     Called by fromgroups(), extract pairs specific to a pair of species.
     """
     agenome = op.basename(abed.filename).split(".")[0]
@@ -426,15 +428,15 @@
         for a, b in iter:
             if a not in aorder or b not in border:
                 continue
 
             print("\t".join((a, b)), file=fw)
             npairs += 1
 
-    logging.debug("File `{0}` written with {1} pairs.".format(pairsfile, npairs))
+    logger.debug("File `{0}` written with {1} pairs.".format(pairsfile, npairs))
 
 
 def fromgroups(args):
     """
     %prog fromgroups groupsfile a.bed b.bed ...
 
     Flatten the gene familes into pairs, the groupsfile is a file with each line
@@ -501,15 +503,15 @@
         f2 = Fasta(pepfile)
         fw2 = must_open(outfile + ".pep", "w")
     for row in fp:
         if row[0] == "#":
             continue
         a, b = row.split()[:2]
         if a == b:
-            logging.debug("Self pairs found: {0} - {1}. Ignored".format(a, b))
+            logger.debug("Self pairs found: {0} - {1}. Ignored".format(a, b))
             continue
 
         if a not in f:
             a = find_first_isoform(a, f)
             assert a, a
         if b not in f:
             b = find_first_isoform(b, f)
@@ -545,26 +547,26 @@
         3. Convert the output to Fasta format.
         4. Use this alignment info to align gene sequences using PAL2NAL
         5. Run PAML yn00 to calculate synonymous mutation rates.
     """
     from jcvi.formats.fasta import translate
 
     p = OptionParser(calc.__doc__)
-    p.add_option(
+    p.add_argument(
         "--longest",
         action="store_true",
         help="Get longest ORF, only works if no pep file, e.g. ESTs",
     )
-    p.add_option(
+    p.add_argument(
         "--msa",
         default="clustalw",
         choices=("clustalw", "muscle"),
         help="software used to align the proteins",
     )
-    p.add_option("--workdir", default=os.getcwd(), help="Work directory")
+    p.add_argument("--workdir", default=os.getcwd(), help="Work directory")
     p.set_outfile()
 
     opts, args = p.parse_args(args)
 
     if len(args) == 1:
         protein_file, dna_file = None, args[0]
     elif len(args) == 2:
@@ -818,18 +820,18 @@
     """
     %prog subset pairsfile ksfile1 ksfile2 ... -o pairs.ks
 
     Subset some pre-calculated ks ka values (in ksfile) according to pairs
     in tab delimited pairsfile/anchorfile.
     """
     p = OptionParser(subset.__doc__)
-    p.add_option(
+    p.add_argument(
         "--noheader", action="store_true", help="don't write ksfile header line"
     )
-    p.add_option(
+    p.add_argument(
         "--block", action="store_true", help="preserve block structure in input"
     )
     p.set_stripnames()
     p.set_outfile()
 
     opts, args = p.parse_args(args)
 
@@ -877,16 +879,16 @@
             print("\t".join(str(x) for x in (a, b, ksline.ks)), file=fw)
         else:
             ksline.name = ";".join((a, b))
             print(ksline, file=fw)
         i += 1
     fw.close()
 
-    logging.debug("{0} pairs not found in ksfiles".format(j))
-    logging.debug("{0} ks records written to `{1}`".format(i, outfile))
+    logger.debug("{0} pairs not found in ksfiles".format(j))
+    logger.debug("{0} ks records written to `{1}`".format(i, outfile))
     return outfile
 
 
 fields = "name,yn_ks,yn_ka,ng_ks,ng_ka"
 descriptions = {
     "name": "Gene pair",
     "yn_ks": "Yang-Nielson Ks estimate",
@@ -937,15 +939,15 @@
         fp = open(filename)
         for row in fp:
             ksline = KsLine(row, strip_names=strip_names)
             if ksline.name == "name":  # header
                 continue
             self.append(ksline)
 
-        logging.debug(
+        logger.debug(
             "File `{0}` contains a total of {1} gene pairs".format(filename, len(self))
         )
 
     def print_to_anchors(self, outfile):
         fw = must_open(outfile, "w")
         for row in self:
             print(row.anchorline, file=fw)
@@ -1049,15 +1051,15 @@
     fitted=True,
     kde=False,
 ):
 
     (line,) = my_hist(
         ax, data, interval, ks_max, color=color, marker=marker, fill=fill, kde=kde
     )
-    logging.debug("Total {0} pairs after filtering.".format(len(data)))
+    logger.debug("Total {0} pairs after filtering.".format(len(data)))
 
     line_mixture = None
     if fitted:
         probs, mus, variances = get_mixture(data, components)
 
         iv = 0.001
         bins = np.arange(iv, ks_max, iv)
@@ -1077,52 +1079,56 @@
                 bbox=dict(ec="w", fc=color, alpha=0.6, boxstyle="round"),
             )
 
     return line, line_mixture
 
 
 def add_plot_options(p):
-    p.add_option("--fit", default=False, action="store_true", help="Plot fitted lines")
-    p.add_option("--kde", default=False, action="store_true", help="Use KDE smoothing")
-    p.add_option("--vmin", default=0.0, type="float", help="Minimum value, inclusive")
-    p.add_option("--vmax", default=3.0, type="float", help="Maximum value, inclusive")
-    p.add_option(
-        "--bins", default=60, type="int", help="Number of bins to plot in the histogram"
+    p.add_argument(
+        "--fit", default=False, action="store_true", help="Plot fitted lines"
+    )
+    p.add_argument(
+        "--kde", default=False, action="store_true", help="Use KDE smoothing"
+    )
+    p.add_argument("--vmin", default=0.0, type=float, help="Minimum value, inclusive")
+    p.add_argument("--vmax", default=3.0, type=float, help="Maximum value, inclusive")
+    p.add_argument(
+        "--bins", default=60, type=int, help="Number of bins to plot in the histogram"
     )
-    p.add_option("--legendp", default="upper right", help="Place of the legend")
-    p.add_option(
+    p.add_argument("--legendp", default="upper right", help="Place of the legend")
+    p.add_argument(
         "--fill",
         default=False,
         action="store_true",
         help="Do not fill the histogram area",
     )
-    p.add_option("--title", default="*Ks* distribution", help="Title of the plot")
+    p.add_argument("--title", default="*Ks* distribution", help="Title of the plot")
 
 
 def report(args):
     """
     %prog report ksfile
 
     generate a report given a Ks result file (as produced by synonymous_calc.py).
     describe the median Ks, Ka values, as well as the distribution in stem-leaf plot
     """
     from jcvi.utils.cbook import SummaryStats
     from jcvi.graphics.histogram import stem_leaf_plot
 
     p = OptionParser(report.__doc__)
-    p.add_option(
+    p.add_argument(
         "--pdf",
         default=False,
         action="store_true",
         help="Generate graphic output for the histogram",
     )
-    p.add_option(
+    p.add_argument(
         "--components",
         default=1,
-        type="int",
+        type=int,
         help="Number of components to decompose peaks",
     )
     add_plot_options(p)
     opts, args, iopts = p.set_image_options(args, figsize="5x5")
 
     if len(args) != 1:
         sys.exit(not p.print_help())
```

### Comparing `jcvi-1.4.6/jcvi/compara/pad.py` & `jcvi-1.4.7/jcvi/compara/pad.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,25 +10,27 @@
 The main pipeline assumes starting with defined synteny blocks in .anchors
 format (use compara.synteny.scan()), then segment the chromosomes and cluster
 segments according to the matching patterns. Finally the putative ancestral
 regions (PAR) are identified and visualized.
 """
 import os.path as op
 import sys
-import logging
+
 from math import log
 
 import numpy as np
+
 from more_itertools import pairwise
 
-from jcvi.compara.synteny import check_beds
-from jcvi.formats.bed import Bed
-from jcvi.formats.blast import BlastLine
-from jcvi.apps.base import OptionParser, ActionDispatcher, need_update, sh
+from ..apps.base import ActionDispatcher, OptionParser, logger, need_update, sh
+from ..formats.bed import Bed
+from ..formats.blast import BlastLine
+
 from .base import AnchorFile
+from .synteny import check_beds
 
 
 def main():
 
     actions = (
         ("cluster", "cluster the segments"),
         ("pad", "test and reconstruct candidate PADs"),
@@ -51,30 +53,30 @@
 
     qsize, ssize = len(qpadbed), len(spadbed)
 
     assert sum(qpadlen.values()) == qsize
     assert sum(spadlen.values()) == ssize
 
     # Populate arrays of observed counts and expected counts
-    logging.debug("Initialize array of size ({0} x {1})".format(m, n))
+    logger.debug("Initialize array of size ({0} x {1})".format(m, n))
     observed = np.zeros((m, n))
     fp = open(blastfile)
     all_dots = 0
     for row in fp:
         b = BlastLine(row)
         qi, q = qpadorder[b.query]
         si, s = spadorder[b.subject]
         qseqid, sseqid = q.seqid, s.seqid
         qsi, ssi = qpadid[qseqid], spadid[sseqid]
         observed[qsi, ssi] += 1
         all_dots += 1
 
     assert int(round(observed.sum())) == all_dots
 
-    logging.debug("Total area: {0} x {1}".format(qsize, ssize))
+    logger.debug("Total area: {0} x {1}".format(qsize, ssize))
     S = qsize * ssize
     expected = np.zeros((m, n))
     qsum = 0
     for i, a in enumerate(qpadnames):
         alen = qpadlen[a]
         qsum += alen
         for j, b in enumerate(spadnames):
@@ -102,18 +104,18 @@
 
     Test and reconstruct candidate PADs.
     """
     from jcvi.formats.cdt import CDT
 
     p = OptionParser(pad.__doc__)
     p.set_beds()
-    p.add_option(
+    p.add_argument(
         "--cutoff",
         default=0.3,
-        type="float",
+        type=float,
         help="The clustering cutoff to call similar",
     )
 
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
@@ -153,15 +155,15 @@
             if score < cutoff:
                 continue
             significant.append((qparts[i], sparts[j], score))
 
     for a, b, score in significant:
         print("|".join(a), "|".join(b), score)
 
-    logging.debug(
+    logger.debug(
         "Collected {0} PAR comparisons significant at (P < {1}).".format(
             len(significant), pvalue_cutoff
         )
     )
 
     return significant
 
@@ -217,15 +219,15 @@
             j += 1
             a, b = pads[j]
         print("\t".join((padnames[j], str(i), str(i + 1), x.accn)), file=fw)
 
     fw.close()
 
     npads = len(pads)
-    logging.debug("{0} partition written in `{1}`.".format(npads, bedfile))
+    logger.debug("{0} partition written in `{1}`.".format(npads, bedfile))
     return npads, padnames
 
 
 def cluster(args):
     """
     %prog cluster blastfile anchorfile --qbed qbedfile --sbed sbedfile
 
@@ -234,18 +236,18 @@
     based on which the genome on one or both axis can be chopped up into pieces
     and clustered.
     """
     from jcvi.utils.range import Range
 
     p = OptionParser(cluster.__doc__)
     p.set_beds()
-    p.add_option(
-        "--minsize", default=10, type="int", help="Only segment using blocks >= size"
+    p.add_argument(
+        "--minsize", default=10, type=int, help="Only segment using blocks >= size"
     )
-    p.add_option(
+    p.add_argument(
         "--path", default="~/scratch/bin", help="Path to the CLUSTER 3.0 binary"
     )
 
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
```

### Comparing `jcvi-1.4.6/jcvi/compara/pedigree.py` & `jcvi-1.4.7/jcvi/compara/pedigree.py`

 * *Files 5% similar despite different names*

```diff
@@ -234,17 +234,17 @@
 def pedigree(args):
     """
     %prog pedigree pedfile
 
     Plot pedigree and calculate pedigree coefficients from a pedigree file.
     """
     p = OptionParser(pedigree.__doc__)
-    p.add_option("--ploidy", default=2, type="int", help="Ploidy")
-    p.add_option("--N", default=10000, type="int", help="Number of samples")
-    p.add_option("--title", default="", help="Title of the graph")
+    p.add_argument("--ploidy", default=2, type=int, help="Ploidy")
+    p.add_argument("--N", default=10000, type=int, help="Number of samples")
+    p.add_argument("--title", default="", help="Title of the graph")
     opts, args, iopts = p.set_image_options(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (pedfile,) = args
     ped = Pedigree(pedfile)
```

### Comparing `jcvi-1.4.6/jcvi/compara/phylogeny.py` & `jcvi-1.4.7/jcvi/compara/phylogeny.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,29 @@
 # compara
 #
 # Created by Haibao Tang on 05/21/20
 # Copyright © 2020 Haibao Tang. All rights reserved.
 #
 import csv
 import sys
-import logging
 import os.path as op
 
-from jcvi.formats.fasta import Fasta, SeqIO
-from jcvi.apps.base import ActionDispatcher, OptionParser, mkdir
+from ..apps.base import ActionDispatcher, OptionParser, logger, mkdir
+from ..formats.fasta import Fasta, SeqIO
 
 
 def lcn(args):
     """
     %prog lcn Orthogroups/Orthogroups.tsv Orthogroup_Sequences/ lcn/
     """
     p = OptionParser(lcn.__doc__)
-    p.add_option("--min-single-ratio", default=0.9, help="Single copy ratio must be > ")
-    p.add_option("--max-zero-ratio", default=0, help="Zero copy ratio must be < ")
+    p.add_argument(
+        "--min-single-ratio", default=0.9, help="Single copy ratio must be > "
+    )
+    p.add_argument("--max-zero-ratio", default=0, help="Zero copy ratio must be < ")
     opts, args = p.parse_args(args)
 
     if len(args) != 3:
         sys.exit(not p.print_help())
 
     (groups_tsv, sequence_dir, lcn_dir) = args
     selected = []
@@ -42,15 +43,15 @@
             if single_ratio < opts.min_single_ratio:
                 continue
             if zero_ratio > opts.max_zero_ratio:
                 continue
             print(row[0], single_ratio, zero_ratio, counts, file=sys.stderr)
             selected.append(row)
 
-    logging.debug("A total of {} orthogroups selected".format(len(selected)))
+    logger.debug("A total of %d orthogroups selected", len(selected))
 
     # Collect the FASTA sequences now
     mkdir(lcn_dir)
     for row in selected:
         orthogroup = row[0]
         orthogroup_fasta = "{}.fa".format(orthogroup)
         input_fasta = op.join(sequence_dir, orthogroup_fasta)
```

### Comparing `jcvi-1.4.6/jcvi/compara/quota.py` & `jcvi-1.4.7/jcvi/compara/quota.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 3. feed the data into the linear programming solver
 
 The algorithm is described in Tang et al. BMC Bioinformatics 2011.
 "Screening synteny blocks in pairwise genome comparisons through integer
 programming."
 """
 
-import logging
 import os.path as op
 import sys
 
-from jcvi.algorithms.lpsolve import MIPDataModel
-from jcvi.compara.synteny import _score, check_beds
-from jcvi.formats.base import must_open
-from jcvi.apps.base import OptionParser
+from ..algorithms.lpsolve import MIPDataModel
+from ..apps.base import OptionParser, logger
+from ..compara.synteny import _score, check_beds
+from ..formats.base import must_open
+
 from .base import AnchorFile
 
 
 def get_1D_overlap(eclusters, depth=1):
     """
     Find blocks that are 1D overlapping,
     returns cliques of block ids that are in conflict
@@ -182,43 +182,43 @@
     return clusters
 
 
 def main(args):
     p = OptionParser(__doc__)
 
     p.set_beds()
-    p.add_option(
+    p.add_argument(
         "--quota",
         default="1:1",
         help="`quota mapping` procedure -- screen blocks to constrain mapping"
         " (useful for orthology), "
         "put in the format like (#subgenomes expected for genome X):"
         "(#subgenomes expected for genome Y)",
     )
-    p.add_option(
+    p.add_argument(
         "--Nm",
         dest="Nmax",
-        type="int",
+        type=int,
         default=10,
         help="distance cutoff to tolerate two blocks that are "
         "slightly overlapping (cutoff for `quota mapping`) "
         "[default: %default units (gene or bp dist)]",
     )
 
-    p.add_option(
+    p.add_argument(
         "--self",
         dest="self_match",
         action="store_true",
         default=False,
         help="you might turn this on when screening paralogous blocks, "
         "esp. if you have reduced mirrored blocks into non-redundant set",
     )
     p.set_verbose(help="Show verbose solver output")
 
-    p.add_option(
+    p.add_argument(
         "--screen",
         default=False,
         action="store_true",
         help="generate new anchors file",
     )
 
     opts, args = p.parse_args(args)
@@ -231,15 +231,15 @@
 
     # sanity check for the quota
     if opts.quota:
         try:
             qa, qb = opts.quota.split(":")
             qa, qb = int(qa), int(qb)
         except ValueError:
-            logging.error("quota string should be the form x:x (2:4, 1:3, etc.)")
+            logger.error("quota string should be the form x:x (2:4, 1:3, etc.)")
             sys.exit(1)
 
         if opts.self_match and qa != qb:
             raise Exception(
                 "when comparing genome to itself, "
                 "quota must be the same number "
                 "(like 1:1, 2:2) you have %s" % opts.quota
@@ -260,22 +260,22 @@
         quota,
         work_dir=work_dir,
         Nmax=opts.Nmax,
         self_match=self_match,
         verbose=opts.verbose,
     )
 
-    logging.debug("Selected %d blocks", len(selected_ids))
+    logger.debug("Selected %d blocks", len(selected_ids))
     prefix = qa_file.rsplit(".", 1)[0]
     suffix = "{}x{}".format(qa, qb)
     outfile = ".".join((prefix, suffix))
     fw = must_open(outfile, "w")
     print(",".join(str(x) for x in selected_ids), file=fw)
     fw.close()
-    logging.debug("Screened blocks ids written to `%s`", outfile)
+    logger.debug("Screened blocks ids written to `%s`", outfile)
 
     if opts.screen:
         from jcvi.compara.synteny import screen
 
         new_qa_file = ".".join((prefix, suffix, "anchors"))
         largs = [qa_file, new_qa_file, "--ids", outfile]
         if opts.qbed and opts.sbed:
```

### Comparing `jcvi-1.4.6/jcvi/compara/reconstruct.py` & `jcvi-1.4.7/jcvi/compara/reconstruct.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 
 """
 From synteny blocks, reconstruct ancestral order by interleaving the genes in
 between the anchors. This is the bottom-up method used first in Bowers (2003),
 and in Tang (2010), to reconstruct pre-alpha and pre-rho order, respectively.
 """
 import sys
-import logging
 
 from itertools import zip_longest
 from math import sqrt
 from more_itertools import pairwise
 
-from jcvi.compara.synteny import check_beds
-from jcvi.formats.base import get_number
-from jcvi.formats.bed import Bed
-from jcvi.utils.grouper import Grouper
-from jcvi.apps.base import OptionParser, ActionDispatcher
+from ..apps.base import ActionDispatcher, OptionParser, logger
+from ..formats.base import get_number
+from ..formats.bed import Bed
+from ..utils.grouper import Grouper
+
 from .base import AnchorFile
+from .synteny import check_beds
 
 
 def main():
 
     actions = (
         ("collinear", "reduce synteny blocks to strictly collinear"),
         ("zipbed", "build ancestral contig from collinear blocks"),
@@ -91,15 +91,15 @@
     families = Grouper()
     for anchorfile in anchorfiles:
         af = AnchorFile(anchorfile)
         for a, b, block_id in af.iter_pairs():
             families.join(a, b)
 
     allowed = set(families.keys())
-    logging.debug(
+    logger.debug(
         "Total families: {}, Gene members: {}".format(len(families), len(allowed))
     )
 
     # TODO: Use C++ implementation of BiGraph() when available
     # For now just serialize this to the disk
     for bedfile in bedfiles:
         bed = Bed(bedfile, include=allowed)
@@ -210,15 +210,15 @@
         for q, s, score in block:
             npairs += 1
             score = score.replace("L", "")
             lines.append("\t".join((q, s, score, block_id)))
         print("\n".join(sorted(lines)), file=fw)
 
     fw.close()
-    logging.debug("A total of {0} pairs written to `{1}`.".format(npairs, outfile))
+    logger.debug("A total of {0} pairs written to `{1}`.".format(npairs, outfile))
 
 
 def interleave_pairs(pairs):
     a, b = pairs[0]
     yield a
     yield b
     for c, d in pairs[1:]:
@@ -240,15 +240,15 @@
     %prog zipbed species.bed collinear.anchors
 
     Build ancestral contig from collinear blocks. For example, to build pre-rho
     order, use `zipbed rice.bed rice.rice.1x1.collinear.anchors`. The algorithms
     proceeds by interleaving the genes together.
     """
     p = OptionParser(zipbed.__doc__)
-    p.add_option("--prefix", default="b", help="Prefix for the new seqid")
+    p.add_argument("--prefix", default="b", help="Prefix for the new seqid")
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     bedfile, anchorfile = args
     prefix = opts.prefix
@@ -268,15 +268,15 @@
             si, s = order[s]
             pairs.append((qi, si))
         newbed = list(interleave_pairs(pairs))
         for i, b in enumerate(newbed):
             accn = bed[b].accn
             print("\t".join(str(x) for x in (block_id, i, i + 1, accn)), file=fw)
 
-    logging.debug("Reconstructed bedfile written to `{0}`.".format(newbedfile))
+    logger.debug("Reconstructed bedfile written to `{0}`.".format(newbedfile))
 
 
 # Non-linear transformation of anchor scores
 def score_convert(x):
     return int(sqrt(x))
```

### Comparing `jcvi-1.4.6/jcvi/compara/synfind.py` & `jcvi-1.4.7/jcvi/compara/synfind.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,29 +17,29 @@
 or inserted). In this case, a right flanker is used to represent the region.
 S is "Syntelog", which means it has a match to the region. In this case, the match
 itself is used to represent the region.  The number in the 4th column is the
 synteny score. For the same query, it is ordered with decreasing synteny score.
 The last column means orientation. "+" is same direction.
 """
 import os.path as op
-import logging
-import sys
 import sqlite3
+import sys
 
 from bisect import bisect_left
 from itertools import groupby, tee
 
-from jcvi.algorithms.lis import (
+from ..algorithms.lis import (
     longest_increasing_subsequence,
     longest_decreasing_subsequence,
 )
-from jcvi.compara.synteny import check_beds, read_blast
-from jcvi.utils.grouper import Grouper
-from jcvi.formats.base import must_open
-from jcvi.apps.base import OptionParser, OptionGroup
+from ..apps.base import OptionParser, logger
+from ..formats.base import must_open
+from ..utils.grouper import Grouper
+
+from .synteny import check_beds, read_blast
 
 
 def transposed(data):
     x, y = zip(*data)
     return zip(y, x)
 
 
@@ -224,15 +224,15 @@
         )
         fw = None
     else:
         fw = must_open(opts.outfile, "w")
 
     batch_query(qbed, sbed, all_data, opts, fw=fw, c=c, transpose=False)
     if qbed.filename == sbed.filename:
-        logging.debug("Self comparisons, mirror ignored")
+        logger.debug("Self comparisons, mirror ignored")
     else:
         batch_query(qbed, sbed, all_data, opts, fw=fw, c=c, transpose=True)
 
     if sqlite:
         c.execute("create index q on synteny (query)")
         conn.commit()
         c.close()
@@ -243,40 +243,37 @@
 if __name__ == "__main__":
 
     p = OptionParser(__doc__)
     p.set_beds()
     p.set_stripnames()
     p.set_outfile()
 
-    coge_group = OptionGroup(p, "CoGe-specific options")
-    coge_group.add_option("--sqlite", help="Write sqlite database")
-    coge_group.add_option("--qnote", default="null", help="Query dataset group id")
-    coge_group.add_option("--snote", default="null", help="Subject dataset group id")
-
-    params_group = OptionGroup(p, "Synteny parameters")
-    params_group.add_option(
-        "--window", type="int", default=40, help="Synteny window size"
+    coge_group = p.add_argument_group("CoGe-specific options")
+    coge_group.add_argument("--sqlite", help="Write sqlite database")
+    coge_group.add_argument("--qnote", default="null", help="Query dataset group id")
+    coge_group.add_argument("--snote", default="null", help="Subject dataset group id")
+
+    params_group = p.add_argument_group("Synteny parameters")
+    params_group.add_argument(
+        "--window", type=int, default=40, help="Synteny window size"
     )
-    params_group.add_option(
+    params_group.add_argument(
         "--cutoff",
-        type="float",
+        type=float,
         default=0.1,
         help="Minimum number of anchors to call synteny",
     )
     supported_scoring = ("collinear", "density")
-    params_group.add_option(
+    params_group.add_argument(
         "--scoring",
         choices=supported_scoring,
         default="collinear",
         help="Scoring scheme",
     )
 
-    p.add_option_group(coge_group)
-    p.add_option_group(params_group)
-
     opts, args = p.parse_args()
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (blastfile,) = args
     main(blastfile, p, opts)
```

### Comparing `jcvi-1.4.6/jcvi/compara/synteny.py` & `jcvi-1.4.7/jcvi/compara/synteny.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 # -*- coding: UTF-8 -*-
 
 """Syntenty inference in comparative genomics
 """
 
 import os.path as op
 import sys
-import logging
 
-import numpy as np
 from collections import defaultdict
-
 from collections.abc import Iterable
 
-from jcvi.algorithms.lis import heaviest_increasing_subsequence as his
-from jcvi.formats.bed import Bed, BedLine
-from jcvi.formats.blast import Blast
-from jcvi.formats.base import BaseFile, SetFile, read_block, must_open
-from jcvi.utils.grouper import Grouper
-from jcvi.utils.cbook import gene_name, human_size
-from jcvi.utils.range import range_chain
-from jcvi.apps.base import ActionDispatcher, OptionParser, cleanup
+import numpy as np
+
+from ..algorithms.lis import heaviest_increasing_subsequence as his
+from ..apps.base import ActionDispatcher, OptionParser, cleanup, logger
+from ..formats.base import BaseFile, SetFile, read_block, must_open
+from ..formats.bed import Bed, BedLine
+from ..formats.blast import Blast
+from ..utils.cbook import gene_name, human_size
+from ..utils.grouper import Grouper
+from ..utils.range import range_chain
+
 from .base import AnchorFile
 
 
 class BlockFile(BaseFile):
     """Parse .blocks file which is the mcscan output with multiple columns as 'tracks'"""
 
     def __init__(self, filename, defaultcolor="#fb8072", header=False):
@@ -150,15 +150,15 @@
 
     def grouper(self) -> Grouper:
         """Build orthogroup based on the gene matches."""
         grouper = Grouper()
         for row in self.data:
             if "." not in row:
                 grouper.join(*row)
-        logging.debug("A total of %d orthogroups formed", len(grouper))
+        logger.debug("A total of %d orthogroups formed", len(grouper))
         return grouper
 
 
 class SimpleFile(object):
     def __init__(self, simplefile, defaultcolor="#fb8072", order=None):
         # Sometimes the simplefile has query and subject wrong
         fp = open(simplefile)
@@ -270,15 +270,15 @@
 
         b.qseqid, b.sseqid = q.seqid, s.seqid
         b.qi, b.si = qi, si
         b.query, b.subject = query, subject
 
         filtered_blast.append(b)
 
-    logging.debug(
+    logger.debug(
         "A total of %d BLAST imported from `%s`.", len(filtered_blast), blast_file
     )
 
     return filtered_blast
 
 
 def read_anchors(ac, qorder, sorder, minsize=0):
@@ -296,15 +296,15 @@
         si, s = sorder[b]
         pair = (qi, si)
 
         all_anchors[(q.seqid, s.seqid)].append(pair)
         anchor_to_block[pair] = idx
         nanchors += 1
 
-    logging.debug("A total of {0} anchors imported.".format(nanchors))
+    logger.debug("A total of {0} anchors imported.".format(nanchors))
     assert nanchors == len(anchor_to_block)
 
     return all_anchors, anchor_to_block
 
 
 def synteny_scan(points, xdist, ydist, N, is_self=False, intrabound=300):
     """
@@ -383,45 +383,45 @@
 def get_bed_filenames(hintfile, p, opts):
     wd, hintfile = op.split(hintfile)
     if not (opts.qbed and opts.sbed):
         try:
             q, s = hintfile.split(".", 2)[:2]
             opts.qbed = op.join(wd, q + ".bed")
             opts.sbed = op.join(wd, s + ".bed")
-            logging.debug("Assuming --qbed={0} --sbed={1}".format(opts.qbed, opts.sbed))
+            logger.debug("Assuming --qbed={0} --sbed={1}".format(opts.qbed, opts.sbed))
         except:
             print("Options --qbed and --sbed are required", file=sys.stderr)
             sys.exit(not p.print_help())
 
     return opts.qbed, opts.sbed
 
 
 def check_beds(hintfile, p, opts, sorted=True):
     qbed_file, sbed_file = get_bed_filenames(hintfile, p, opts)
     # is this a self-self blast?
     is_self = qbed_file == sbed_file
     if is_self:
-        logging.debug("Looks like self-self comparison.")
+        logger.debug("Looks like self-self comparison.")
 
     qbed = Bed(opts.qbed, sorted=sorted)
     sbed = Bed(opts.sbed, sorted=sorted)
     qorder = qbed.order
     sorder = sbed.order
 
     return qbed, sbed, qorder, sorder, is_self
 
 
-def add_options(p, args, dist=10):
+def add_arguments(p, args, dist=10):
     """
     scan and liftover has similar interfaces, so share common options
     returns opts, files
     """
     p.set_beds()
-    p.add_option(
-        "--dist", default=dist, type="int", help="Extent of flanking regions to search"
+    p.add_argument(
+        "--dist", default=dist, type=int, help="Extent of flanking regions to search"
     )
 
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
@@ -565,15 +565,15 @@
     import shutil
     from tempfile import mkdtemp, mkstemp
 
     from jcvi.apps.align import last
     from jcvi.formats.fasta import some
 
     p = OptionParser(assemble.__doc__)
-    p.add_option(
+    p.add_argument(
         "--no_strip_names",
         default=False,
         action="store_true",
         help="Do not strip alternative splicing (e.g. At5g06540.1 -> At5g06540)",
     )
     p.set_outfile()
     opts, args = p.parse_args(args)
@@ -603,15 +603,15 @@
     # Write gene ids
     workdir = mkdtemp()
     fd, idsfile = mkstemp(dir=workdir)
     with open(idsfile, "w") as fw:
         for genes in column_genes:
             print(" ".join(genes), file=fw)
 
-        logging.debug("Gene ids written to `{}`".format(idsfile))
+        logger.debug("Gene ids written to `{}`".format(idsfile))
 
     # Extract FASTA
     fd, fastafile = mkstemp(dir=workdir)
     some_args = [cdsfile, idsfile, fastafile]
     if not strip_names:
         some_args += ["--no_strip_names"]
     some(some_args)
@@ -621,15 +621,15 @@
     blast = Blast(last_output)
     pairs = set()
     for b in blast:
         query, subject = b.query, b.subject
         if strip_names:
             query, subject = gene_name(query), gene_name(subject)
         pairs.add((query, subject))
-    logging.debug("Extracted {} gene pairs from `{}`".format(len(pairs), last_output))
+    logger.debug("Extracted {} gene pairs from `{}`".format(len(pairs), last_output))
 
     # Sort the pairs into columns
     N = len(column_genes)
     all_slots = []
     for i in range(N):
         for j in range(i + 1, N):
             genes_i = column_genes[i]
@@ -670,15 +670,15 @@
             if is_compatible(slots, processed):
                 merge(slots, processed)  # Merge into that line
                 merged = True
                 break
         if not merged:  # New information
             processed_slots.append(slots)
 
-    logging.debug(
+    logger.debug(
         "Before compression: {}, After compression: {}".format(
             len(all_slots), len(processed_slots)
         )
     )
 
     pivot_order = species_beds[pivot].order
     pivot_max = len(species_beds[pivot])
@@ -780,24 +780,24 @@
     """
     %prog fromaligns input.anchors
 
     Convert anchors file to tab-separated aligns file, adding the first column
     with the Block ID.
     """
     p = OptionParser(toaligns.__doc__)
-    p.add_option("--prefix", default="b", help="Prefix to the block id")
+    p.add_argument("--prefix", default="b", help="Prefix to the block id")
     p.set_outfile()
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(p.print_help())
 
     (anchorfile,) = args
     ac = AnchorFile(anchorfile)
-    logging.debug("A total of {} blocks imported".format(len(ac.blocks)))
+    logger.debug("A total of {} blocks imported".format(len(ac.blocks)))
     max_block_id_len = len(str(len(ac.blocks) - 1))
     header = "\t".join(("#Block ID", "Gene 1", "Gene 2"))
 
     with must_open(opts.outfile, "w") as fw:
         print(header, file=fw)
         for a, b, block_id in ac.iter_pairs():
             block_id = "{}{:0{}d}".format(opts.prefix, block_id, max_block_id_len)
@@ -809,16 +809,16 @@
     %prog mcscanq query.ids blocksfile
 
     Query multiple synteny blocks to get the closest alignment feature. Mostly
     used for 'highlighting' the lines in the synteny plot, drawn by
     graphics.karyotype and graphics.synteny.
     """
     p = OptionParser(mcscanq.__doc__)
-    p.add_option("--color", help="Add color highlight, used in plotting")
-    p.add_option(
+    p.add_argument("--color", help="Add color highlight, used in plotting")
+    p.add_argument(
         "--invert", default=False, action="store_true", help="Invert query and subject"
     )
     opts, args = p.parse_args(args)
 
     if len(args) < 2:
         sys.exit(not p.print_help())
 
@@ -838,15 +838,15 @@
     Convert chromosome ordering from SPA to simple lists. First column is the
     reference order.
     """
     from jcvi.algorithms.graph import merge_paths
     from jcvi.utils.cbook import uniqify
 
     p = OptionParser(spa.__doc__)
-    p.add_option(
+    p.add_argument(
         "--unmapped",
         default=False,
         action="store_true",
         help="Include unmapped scaffolds in the list",
     )
     opts, args = p.parse_args(args)
 
@@ -895,18 +895,18 @@
 def rebuild(args):
     """
     %prog rebuild blocksfile blastfile
 
     Rebuild anchors file from pre-built blocks file.
     """
     p = OptionParser(rebuild.__doc__)
-    p.add_option(
+    p.add_argument(
         "--header", default=False, action="store_true", help="First line is header"
     )
-    p.add_option(
+    p.add_argument(
         "--write_blast",
         default=False,
         action="store_true",
         help="Get blast records of rebuilt anchors",
     )
     p.set_beds()
 
@@ -986,15 +986,15 @@
     """
     %prog matrix all.bed anchorfile matrixfile
 
     Make oxford grid based on anchors file.
     """
 
     p = OptionParser(matrix.__doc__)
-    p.add_option("--seqids", help="File with seqids")
+    p.add_argument("--seqids", help="File with seqids")
     opts, args = p.parse_args(args)
 
     if len(args) != 3:
         sys.exit(not p.print_help())
 
     bedfile, anchorfile, matrixfile = args
     ac = AnchorFile(anchorfile)
@@ -1052,30 +1052,30 @@
     orderA1   orderA2   orderB1   orderB2  sizeA    sizeB   size    block_id
 
     With base coordinates (--coords):
     block_id  seqidA    startA    endA     bpSpanA  GeneA1   GeneA2  geneSpanA
     block_id  seqidB    startB    endB     bpSpanB  GeneB1   GeneB2  geneSpanB
     """
     p = OptionParser(simple.__doc__)
-    p.add_option(
+    p.add_argument(
         "--rich", default=False, action="store_true", help="Output additional columns"
     )
-    p.add_option(
+    p.add_argument(
         "--coords",
         default=False,
         action="store_true",
         help="Output columns with base coordinates",
     )
-    p.add_option(
+    p.add_argument(
         "--bed",
         default=False,
         action="store_true",
         help="Generate BED file for the blocks",
     )
-    p.add_option(
+    p.add_argument(
         "--noheader", default=False, action="store_true", help="Don't output header"
     )
     p.set_beds()
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
@@ -1091,15 +1091,15 @@
 
     ac = AnchorFile(anchorfile)
     simplefile = anchorfile.rsplit(".", 1)[0] + ".simple"
 
     qbed, sbed, qorder, sorder, is_self = check_beds(anchorfile, p, opts)
     pf = "-".join(anchorfile.split(".", 2)[:2])
     if ac.is_empty:
-        logging.error("No blocks found in `%s`. Aborting ..", anchorfile)
+        logger.error("No blocks found in `%s`. Aborting ..", anchorfile)
         return
 
     if coords:
         h = "Block|Chr|Start|End|Span|StartGene|EndGene|GeneSpan|Orientation"
     else:
         h = "StartGeneA|EndGeneA|StartGeneB|EndGeneB|Orientation|Score"
         if additional:
@@ -1190,15 +1190,15 @@
 
         args = [astart, aend, bstart, bend, score, orientation]
         if additional:
             args += [astarti, aendi, bstarti, bendi, sizeA, sizeB, size, block_id]
         print("\t".join(str(x) for x in args), file=fws)
 
     fws.close()
-    logging.debug("A total of {0} blocks written to `{1}`.".format(i + 1, simplefile))
+    logger.debug("A total of {0} blocks written to `{1}`.".format(i + 1, simplefile))
 
     if coords:
         print(
             "Total block span in {0}: {1}".format(
                 qbed.filename, human_size(atotalbase, precision=2)
             ),
             file=sys.stderr,
@@ -1215,15 +1215,15 @@
             ),
             file=sys.stderr,
         )
 
     if bed:
         bedfile = simplefile + ".bed"
         bbed.print_to_file(filename=bedfile, sorted=True)
-        logging.debug("Bed file written to `{}`".format(bedfile))
+        logger.debug("Bed file written to `{}`".format(bedfile))
 
 
 def screen(args):
     """
     %prog screen anchorfile newanchorfile --qbed=qbedfile --sbed=sbedfile [options]
 
     Extract subset of blocks from anchorfile. Provide several options:
@@ -1236,26 +1236,26 @@
     6. Option --intrabound: remove blocks that are too close to the diagonal on
        self dot plot that are typically artifacts
     """
     from jcvi.utils.range import range_distance
 
     p = OptionParser(screen.__doc__)
     p.set_beds()
-    p.add_option("--ids", help="File with block IDs (0-based)")
-    p.add_option("--seqids", help="File with seqids")
-    p.add_option("--seqpairs", help="File with seqpairs")
-    p.add_option(
+    p.add_argument("--ids", help="File with block IDs (0-based)")
+    p.add_argument("--seqids", help="File with seqids")
+    p.add_argument("--seqpairs", help="File with seqpairs")
+    p.add_argument(
         "--intrabound",
         default=300,
-        type="int",
+        type=int,
         help="Lower bound of intra-chromosomal blocks (only for self comparison)",
     )
-    p.add_option("--minspan", default=0, type="int", help="Only blocks with span >=")
-    p.add_option("--minsize", default=0, type="int", help="Only blocks with anchors >=")
-    p.add_option(
+    p.add_argument("--minspan", default=0, type=int, help="Only blocks with span >=")
+    p.add_argument("--minsize", default=0, type=int, help="Only blocks with anchors >=")
+    p.add_argument(
         "--simple", action="store_true", help="Write simple anchorfile with block ends"
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
@@ -1342,37 +1342,37 @@
                 newanchorfile,
                 "--noheader",
                 "--qbed=" + qbed.filename,
                 "--sbed=" + sbed.filename,
             ]
         )
 
-    logging.debug("Before: {0} blocks, After: {1} blocks".format(len(blocks), selected))
+    logger.debug("Before: {0} blocks, After: {1} blocks".format(len(blocks), selected))
 
 
 def summary(args):
     """
     %prog summary anchorfile
 
     Provide statistics for pairwise blocks.
     """
     from jcvi.utils.cbook import SummaryStats
 
     p = OptionParser(summary.__doc__)
-    p.add_option("--prefix", help="Generate per block stats")
+    p.add_argument("--prefix", help="Generate per block stats")
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (anchorfile,) = args
     ac = AnchorFile(anchorfile)
     clusters = ac.blocks
     if clusters == [[]]:
-        logging.debug("A total of 0 anchor was found. Aborted.")
+        logger.debug("A total of 0 anchor was found. Aborted.")
         raise ValueError("A total of 0 anchor was found. Aborted.")
 
     nclusters = len(clusters)
     nanchors = [len(c) for c in clusters]
     nranchors = [_score(c) for c in clusters]  # non-redundant anchors
     print(
         "A total of {0} (NR:{1}) anchors found in {2} clusters.".format(
@@ -1450,30 +1450,30 @@
     the output is the reference order, given in the bedfile. Then each column
     next to it are separate 'tracks'.
 
     If --mergetandem=tandem_file is specified, tandem_file should have each
     tandem cluster as one line, tab separated.
     """
     p = OptionParser(mcscan.__doc__)
-    p.add_option(
-        "--iter", default=100, type="int", help="Max number of chains to output"
+    p.add_argument(
+        "--iter", default=100, type=int, help="Max number of chains to output"
     )
-    p.add_option(
+    p.add_argument(
         "--ascii",
         default=False,
         action="store_true",
         help="Output symbols rather than gene names",
     )
-    p.add_option(
-        "--Nm", default=10, type="int", help="Clip block ends to allow slight overlaps"
+    p.add_argument(
+        "--Nm", default=10, type=int, help="Clip block ends to allow slight overlaps"
     )
-    p.add_option(
+    p.add_argument(
         "--trackids", action="store_true", help="Track block IDs in separate file"
     )
-    p.add_option(
+    p.add_argument(
         "--mergetandem",
         default=None,
         help="merge tandems genes in output acoording to PATH-TO-TANDEM_FILE, "
         "cannot be used with --ascii",
     )
     p.set_outfile()
     opts, args = p.parse_args(args)
@@ -1550,17 +1550,17 @@
     for id, atoms in mbed:
         sep = "" if ascii else "\t"
         if mergetandem:
             for i, atom in enumerate(atoms):
                 atoms[i] = tandems.get(atom, atom)
         print("\t".join((id, sep.join(atoms))), file=fw)
 
-    logging.debug("MCscan blocks written to `{0}`.".format(ofile))
+    logger.debug("MCscan blocks written to `{0}`.".format(ofile))
     if trackids:
-        logging.debug("Block IDs written to `{0}`.".format(olog))
+        logger.debug("Block IDs written to `{0}`.".format(olog))
 
 
 def write_details(fw, details, bed):
     """
     Write per gene depth to file
     """
     for a, b, depth in details:
@@ -1577,21 +1577,21 @@
     --sbed. The synteny blocks will be layered on the genomes, and the
     multiplicity will be summarized to stderr.
     """
     from jcvi.utils.range import range_depth
     from jcvi.graphics.base import latex
 
     p = OptionParser(depth.__doc__)
-    p.add_option("--depthfile", help="Generate file with gene and depth")
-    p.add_option(
+    p.add_argument("--depthfile", help="Generate file with gene and depth")
+    p.add_argument(
         "--histogram", default=False, action="store_true", help="Plot histograms in PDF"
     )
-    p.add_option("--xmax", type="int", help="x-axis maximum to display in plot")
-    p.add_option("--title", default=None, help="Title to display in plot")
-    p.add_option("--quota", help="Force to use this quota, e.g. 1:1, 1:2 ...")
+    p.add_argument("--xmax", type=int, help="x-axis maximum to display in plot")
+    p.add_argument("--title", default=None, help="Title to display in plot")
+    p.add_argument("--quota", help="Force to use this quota, e.g. 1:1, 1:2 ...")
     p.set_beds()
 
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
@@ -1627,15 +1627,15 @@
 
     stag = "Genome {0} depths".format(sgenome)
     print("{}:".format(stag), file=sys.stderr)
     dss, details = range_depth(sranges, len(sbed))
     if depthfile:
         write_details(fw, details, sbed)
         fw.close()
-        logging.debug("Depth written to `{0}`.".format(depthfile))
+        logger.debug("Depth written to `{0}`.".format(depthfile))
 
     if not opts.histogram:
         return
 
     from jcvi.graphics.base import plt, quickplot_ax, savefig, normalize_axes
 
     # Plot two histograms one for query genome, one for subject genome
@@ -1719,21 +1719,21 @@
     from markers (query) to scaffolds (subject). `bedfile` contains marker
     locations in the related species.
     """
     from jcvi.formats.blast import bed
     from jcvi.utils.range import range_interleave
 
     p = OptionParser(breakpoint.__doc__)
-    p.add_option(
-        "--xdist", type="int", default=20, help="xdist (in related genome) cutoff"
+    p.add_argument(
+        "--xdist", type=int, default=20, help="xdist (in related genome) cutoff"
     )
-    p.add_option(
-        "--ydist", type="int", default=200000, help="ydist (in current genome) cutoff"
+    p.add_argument(
+        "--ydist", type=int, default=200000, help="ydist (in current genome) cutoff"
     )
-    p.add_option("-n", type="int", default=5, help="number of markers in a block")
+    p.add_argument("-n", type=int, default=5, help="number of markers in a block")
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     blastfile, bedfile = args
     order = Bed(bedfile).order
@@ -1756,46 +1756,46 @@
 def scan(args):
     """
     %prog scan blastfile anchor_file [options]
 
     pull out syntenic anchors from blastfile based on single-linkage algorithm
     """
     p = OptionParser(scan.__doc__)
-    p.add_option(
+    p.add_argument(
         "-n",
         "--min_size",
         dest="n",
-        type="int",
+        type=int,
         default=4,
         help="minimum number of anchors in a cluster",
     )
-    p.add_option(
+    p.add_argument(
         "--intrabound",
         default=300,
-        type="int",
+        type=int,
         help="Lower bound of intra-chromosomal blocks (only for self comparison)",
     )
-    p.add_option("--liftover", help="Scan BLAST file to find extra anchors")
-    p.add_option(
+    p.add_argument("--liftover", help="Scan BLAST file to find extra anchors")
+    p.add_argument(
         "--liftover_dist",
-        type="int",
+        type=int,
         help="Distance to extend from liftover. Defaults to half of --dist",
     )
     p.set_stripnames()
 
-    blast_file, anchor_file, dist, opts = add_options(p, args, dist=20)
+    blast_file, anchor_file, dist, opts = add_arguments(p, args, dist=20)
     qbed, sbed, qorder, sorder, is_self = check_beds(blast_file, p, opts)
 
     intrabound = opts.intrabound
     filtered_blast = read_blast(
         blast_file, qorder, sorder, is_self=is_self, ostrip=False
     )
 
     fw = open(anchor_file, "w")
-    logging.debug("Chaining distance = {0}".format(dist))
+    logger.debug("Chaining distance = {0}".format(dist))
 
     clusters = batch_scan(
         filtered_blast,
         xdist=dist,
         ydist=dist,
         N=opts.n,
         is_self=is_self,
@@ -1834,15 +1834,15 @@
 
         geneA geneB
         geneC geneD
     """
     p = OptionParser(liftover.__doc__)
     p.set_stripnames()
 
-    blast_file, anchor_file, dist, opts = add_options(p, args)
+    blast_file, anchor_file, dist, opts = add_arguments(p, args)
     qbed, sbed, qorder, sorder, is_self = check_beds(blast_file, p, opts)
 
     filtered_blast = read_blast(
         blast_file, qorder, sorder, is_self=is_self, ostrip=opts.strip_names
     )
     blast_to_score = dict(((b.qi, b.si), int(b.score)) for b in filtered_blast)
     accepted = dict(((b.query, b.subject), str(int(b.score))) for b in filtered_blast)
@@ -1865,15 +1865,15 @@
             block_id = anchor_to_block[nearest]
             query, subject = qbed[qi].accn, sbed[si].accn
             score = blast_to_score[(qi, si)]
 
             ac.blocks[block_id].append((query, subject, str(score) + "L"))
             lifted += 1
 
-    logging.debug("{} new pairs found (dist={}).".format(lifted, dist))
+    logger.debug("{} new pairs found (dist={}).".format(lifted, dist))
     newanchorfile = anchor_file.rsplit(".", 1)[0] + ".lifted.anchors"
     ac.print_to_file(filename=newanchorfile, accepted=accepted)
     summary([newanchorfile])
 
     return newanchorfile
```

### Comparing `jcvi-1.4.6/jcvi/formats/agp.py` & `jcvi-1.4.7/jcvi/formats/agp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 """
 Genbank AGP file format, see spec here
 http://www.ncbi.nlm.nih.gov/projects/genome/assembly/agp
 """
-import os
 import re
-import sys
 import shutil
-import logging
+import sys
 
-from copy import deepcopy
 from collections import defaultdict
+from copy import deepcopy
 from itertools import groupby, zip_longest
-from more_itertools import pairwise
 
 from Bio.Seq import Seq
 from Bio.SeqRecord import SeqRecord
 from Bio import SeqIO
+from more_itertools import pairwise
 
-from jcvi.formats.base import LineFile, must_open
-from jcvi.formats.fasta import Fasta
-from jcvi.formats.bed import Bed
-from jcvi.assembly.base import calculate_A50
-from jcvi.utils.range import range_intersect
-from jcvi.apps.base import (
-    OptionParser,
-    OptionGroup,
+from ..apps.base import (
     ActionDispatcher,
+    OptionParser,
     cleanup,
     flatten,
+    logger,
     need_update,
 )
+from ..assembly.base import calculate_A50
+from ..utils.range import range_intersect
+
+from .base import LineFile, must_open
+from .bed import Bed
+from .fasta import Fasta
 
 
 Supported_AGP_Version = "2.1"
 AGP_Version_Pragma = "##agp-version " + Supported_AGP_Version
 Valid_component_type = list("ADFGNOPUW")
 
 Valid_gap_type = (
@@ -112,15 +111,15 @@
                 self.gap_type, int(self.part_number)
             )
 
         if validate:
             try:
                 self.validate()
             except AssertionError as b:
-                logging.error("%s\nerror when validating this line:\n%s" % (b, row))
+                logger.error("%s\nerror when validating this line:\n%s", b, row)
 
         self.sign = {"+": 1, "-": -1, "?": 0}.get(self.orientation)
 
     def __str__(self):
 
         fields = [
             self.object,
@@ -404,15 +403,15 @@
                 yield a, b, qreverse
 
     def print_to_file(self, filename, index=True):
         fw = open(filename, "w")
         for a in self:
             print(a, file=fw)
         fw.close()
-        logging.debug("AGP file written to `%s`.", filename)
+        logger.debug("AGP file written to `%s`.", filename)
         if index:
             reindex([filename, "--inplace"])
 
     def summary_one(self, object, lines):
         bacs = set()
         components = 0
         scaffold_sizes = []
@@ -513,15 +512,15 @@
                     line.object_end,
                 )
 
         if not newagp:
             rec = SeqRecord(Seq("".join(components)), id=object, description="")
             SeqIO.write([rec], fw, "fasta")
             if len(rec) > 1000000:
-                logging.debug("Write object %s to `%s`" % (object, fw.name))
+                logger.debug("Write object %s to `%s`", object, fw.name)
 
     def build_all(self, componentfasta, targetfasta, newagp=None):
         f = Fasta(componentfasta, index=False)
         fw = open(targetfasta, "w")
 
         for ob, lines in self.iter_object():
             self.build_one(ob, lines, f, fw, newagp=newagp)
@@ -827,15 +826,15 @@
         trimstart = start + leftNs
         trimend = end - rightNs
 
     trimrange = (trimstart, trimend)
     oldrange = (start, end)
 
     if trimrange != oldrange:
-        logging.debug("{0} trimmed of N's: {1} => {2}".format(lid, oldrange, trimrange))
+        logger.debug("{0} trimmed of N's: {1} => {2}".format(lid, oldrange, trimrange))
 
         if leftNs:
             print(
                 "\t".join(
                     str(x)
                     for x in (line.object, 0, 0, 0, "N", leftNs, "fragment", "yes", "")
                 ),
@@ -915,15 +914,15 @@
 
     Convert csv which contains list of scaffolds/contigs to AGP file.
     """
     import csv
     from jcvi.formats.sizes import Sizes
 
     p = OptionParser(fromcsv.__doc__)
-    p.add_option("--evidence", default="map", help="Linkage evidence to add in AGP")
+    p.add_argument("--evidence", default="map", help="Linkage evidence to add in AGP")
     opts, args = p.parse_args(args)
 
     if len(args) != 3:
         sys.exit(not p.print_help())
 
     contigsfasta, mapcsv, mapagp = args
     reader = csv.reader(open(mapcsv))
@@ -1110,15 +1109,15 @@
     %prog format oldagpfile newagpfile
 
     Reformat AGP file. --switch will replace the ids in the AGP file.
     """
     from jcvi.formats.base import DictFile
 
     p = OptionParser(format.__doc__)
-    p.add_option("--switchcomponent", help="Switch component id based on")
+    p.add_argument("--switchcomponent", help="Switch component id based on")
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     oldagpfile, newagpfile = args
     switchcomponent = opts.switchcomponent
@@ -1129,36 +1128,36 @@
     fw = open(newagpfile, "w")
     nconverts = 0
     for i, a in enumerate(agp):
         if not a.is_gap and a.component_id in switchcomponent:
             oldid = a.component_id
             newid = switchcomponent[a.component_id]
             a.component_id = newid
-            logging.debug("Covert {0} to {1} on line {2}".format(oldid, newid, i + 1))
+            logger.debug("Covert {0} to {1} on line {2}".format(oldid, newid, i + 1))
             nconverts += 1
         print(a, file=fw)
 
-    logging.debug("Total converted records: {0}".format(nconverts))
+    logger.debug("Total converted records: {0}".format(nconverts))
 
 
 def frombed(args):
     """
     %prog frombed bedfile
 
     Generate AGP file based on bed file. The bed file must have at least 6
     columns. With the 4-th column indicating the new object.
     """
     p = OptionParser(frombed.__doc__)
-    p.add_option(
+    p.add_argument(
         "--gapsize",
         default=100,
-        type="int",
+        type=int,
         help="Insert gaps of size",
     )
-    p.add_option("--evidence", default="map", help="Linkage evidence to add in AGP")
+    p.add_argument("--evidence", default="map", help="Linkage evidence to add in AGP")
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (bedfile,) = args
     gapsize = opts.gapsize
@@ -1256,15 +1255,15 @@
     %prog stats agpfile
 
     Print out a report for length of gaps and components.
     """
     from jcvi.utils.table import tabulate
 
     p = OptionParser(stats.__doc__)
-    p.add_option(
+    p.add_argument(
         "--warn",
         default=False,
         action="store_true",
         help="Warnings on small component spans",
     )
     opts, args = p.parse_args(args)
 
@@ -1283,15 +1282,15 @@
             gap_lengths.append((span, label))
         else:
             label = "{0}:{1}-{2}".format(
                 a.component_id, a.component_beg, a.component_end
             )
             component_lengths.append((span, label))
             if opts.warn and span < 50:
-                logging.error("component span too small ({0}):\n{1}".format(span, a))
+                logger.error("component span too small ({0}):\n{1}".format(span, a))
 
     table = dict()
     for label, lengths in zip(("Gaps", "Components"), (gap_lengths, component_lengths)):
 
         if not lengths:
             table[(label, "Min")] = table[(label, "Max")] = table[(label, "Sum")] = (
                 "n.a."
@@ -1308,15 +1307,15 @@
 def cut(args):
     """
     %prog cut agpfile bedfile
 
     Cut at the boundaries of the ranges in the bedfile.
     """
     p = OptionParser(cut.__doc__)
-    p.add_option("--sep", default=".", help="Separator for splits")
+    p.add_argument("--sep", default=".", help="Separator for splits")
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     agpfile, bedfile = args
     sep = opts.sep
@@ -1380,44 +1379,44 @@
     %prog mask agpfile bedfile
 
     Mask given ranges in components to gaps. When the bedfile contains a single
     base pair, this position can be a point of split and no base is lost
     (--splitsingle).
     """
     p = OptionParser(mask.__doc__)
-    p.add_option(
+    p.add_argument(
         "--splitobject",
         default=False,
         action="store_true",
         help="Create new names for object",
     )
-    p.add_option(
+    p.add_argument(
         "--splitcomponent",
         default=False,
         action="store_true",
         help="Create new names for component",
     )
-    p.add_option(
+    p.add_argument(
         "--splitsingle",
         default=False,
         action="store_true",
         help="Do not remove base on single point",
     )
-    p.add_option(
+    p.add_argument(
         "--gaptype",
         default="scaffold",
         help="Masked region has gap type of",
     )
-    p.add_option(
+    p.add_argument(
         "--noretain",
         default=False,
         action="store_true",
         help="Do not retain old names for non-split objects",
     )
-    p.add_option("--sep", default=".", help="Separator for splits")
+    p.add_argument("--sep", default=".", help="Separator for splits")
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(p.print_help())
 
     agpfile, bedfile = args
     gaptype = opts.gaptype
@@ -1529,21 +1528,21 @@
     %prog agpfile
 
     assume the component line order is correct, modify coordinates, this is
     necessary mostly due to manual edits (insert/delete) that disrupts
     the target coordinates.
     """
     p = OptionParser(reindex.__doc__)
-    p.add_option(
+    p.add_argument(
         "--nogaps",
         default=False,
         action="store_true",
         help="Remove all gap lines",
     )
-    p.add_option(
+    p.add_argument(
         "--inplace",
         default=False,
         action="store_true",
         help="Replace input file",
     )
     opts, args = p.parse_args(args)
 
@@ -1578,15 +1577,15 @@
 
     # Last step: validate the new agpfile
     fw.close()
     AGP(newagpfile, validate=True)
 
     if inplace:
         shutil.move(newagpfile, agpfile)
-        logging.debug("Rename file `{0}` to `{1}`".format(newagpfile, agpfile))
+        logger.debug("Rename file `{0}` to `{1}`".format(newagpfile, agpfile))
         newagpfile = agpfile
 
     return newagpfile
 
 
 def summary(args):
     """
@@ -1649,15 +1648,14 @@
                 phase = 1
             else:
                 phase = 2
         else:
             assert "COMPLETE" in description, description
             phase = 3
     else:
-        # logging.error("{0}: {1}".format(rec.name, description))
         phase = 3
 
     return phase, keywords
 
 
 def phase(args):
     """
@@ -1692,21 +1690,21 @@
     Print out a list of ids, one per line. Also known as the Tiling Path.
 
     AC225490.9  chr6
 
     Can optionally output scaffold gaps.
     """
     p = OptionParser(tpf.__doc__)
-    p.add_option(
+    p.add_argument(
         "--noversion",
         default=False,
         action="store_true",
         help="Remove trailing accession versions",
     )
-    p.add_option(
+    p.add_argument(
         "--gaps",
         default=False,
         action="store_true",
         help="Include gaps in the output",
     )
     opts, args = p.parse_args(args)
 
@@ -1736,57 +1734,55 @@
     %prog bed agpfile
 
     print out the tiling paths in bed/gff3 format
     """
     from jcvi.formats.obo import validate_term
 
     p = OptionParser(bed.__doc__)
-    p.add_option(
+    p.add_argument(
         "--gaps",
         default=False,
         action="store_true",
         help="Only print bed lines for gaps",
     )
-    p.add_option(
+    p.add_argument(
         "--nogaps",
         default=False,
         action="store_true",
         help="Do not print bed lines for gaps",
     )
-    p.add_option(
+    p.add_argument(
         "--bed12",
         default=False,
         action="store_true",
         help="Produce bed12 formatted output",
     )
-    p.add_option(
+    p.add_argument(
         "--component",
         default=False,
         action="store_true",
         help="Generate bed file for components",
     )
     p.set_outfile()
-    g1 = OptionGroup(
-        p,
+    g1 = p.add_argument_group(
         "GFF specific parameters",
         "Note: If not specified, output will be in `bed` format",
     )
-    g1.add_option(
+    g1.add_argument(
         "--gff",
         default=False,
         action="store_true",
         help="Produce gff3 formatted output. By default, ignores AGP gap lines",
     )
-    g1.add_option("--source", default="MGSC", help="Specify a gff3 source")
-    g1.add_option(
+    g1.add_argument("--source", default="MGSC", help="Specify a gff3 source")
+    g1.add_argument(
         "--feature",
         default="golden_path_fragment",
         help="Specify a gff3 feature type",
     )
-    p.add_option_group(g1)
     p.set_SO_opts()
 
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
@@ -1848,27 +1844,27 @@
     that are 'represented' - sometimes leaving the 5` and 3` out (those that
     overlap with adjacent sequences. This script fill up those ranges,
     potentially to make graphics for tiling path.
     """
     from jcvi.formats.sizes import Sizes
 
     p = OptionParser(extendbed.__doc__)
-    p.add_option(
+    p.add_argument(
         "--nogaps",
         default=False,
         action="store_true",
         help="Do not print bed lines for gaps",
     )
-    p.add_option(
+    p.add_argument(
         "--bed12",
         default=False,
         action="store_true",
         help="Produce bed12 formatted output",
     )
-    p.add_option(
+    p.add_argument(
         "--gff",
         default=False,
         action="store_true",
         help="Produce gff3 formatted output. By default, ignores " + " AGP gap lines.",
     )
     p.set_outfile()
 
@@ -1935,22 +1931,22 @@
 
     Print out the distribution of gapsizes. Option --merge allows merging of
     adjacent gaps which is used by tidy().
     """
     from jcvi.graphics.histogram import loghistogram
 
     p = OptionParser(gaps.__doc__)
-    p.add_option(
+    p.add_argument(
         "--merge",
         dest="merge",
         default=False,
         action="store_true",
         help="Merge adjacent gaps (to conform to AGP specification)",
     )
-    p.add_option(
+    p.add_argument(
         "--header",
         default=False,
         action="store_true",
         help="Produce an AGP header",
     )
 
     opts, args = p.parse_args(args)
@@ -2032,15 +2028,15 @@
     2. Merge adjacent gaps
     3. Trim gaps at the end of an object
     4. Reindex the agp
 
     Final output is in `.tidy.agp`.
     """
     p = OptionParser(tidy.__doc__)
-    p.add_option(
+    p.add_argument(
         "--nogaps",
         default=False,
         action="store_true",
         help="Remove all gap lines",
     )
     opts, args = p.parse_args(args)
 
@@ -2068,51 +2064,51 @@
     agp = AGP(agpfile)
     newagpfile = agpfile.replace(".agp", ".fixed.agp")
     fw = open(newagpfile, "w")
     for object, a in groupby(agp, key=lambda x: x.object):
         a = list(a)
         if a[0].is_gap:
             g, a = a[0], a[1:]
-            logging.debug("Trim beginning Ns({0}) of {1}".format(g.gap_length, object))
+            logger.debug("Trim beginning Ns({0}) of {1}".format(g.gap_length, object))
         if a and a[-1].is_gap:
             a, g = a[:-1], a[-1]
-            logging.debug("Trim trailing Ns({0}) of {1}".format(g.gap_length, object))
+            logger.debug("Trim trailing Ns({0}) of {1}".format(g.gap_length, object))
         print("\n".join(str(x) for x in a), file=fw)
     fw.close()
     cleanup(agpfile)
 
     # Step 4: Final reindex
     agpfile = newagpfile
     reindex_opts = [agpfile, "--inplace"]
     if opts.nogaps:
         reindex_opts += ["--nogaps"]
     agpfile = reindex(reindex_opts)
 
     tidyagpfile = originalagpfile.replace(".agp", ".tidy.agp")
     shutil.move(agpfile, tidyagpfile)
 
-    logging.debug("File written to `%s`.", tidyagpfile)
+    logger.debug("File written to `%s`.", tidyagpfile)
     return tidyagpfile
 
 
 def build(args):
     """
     %prog build agpfile componentfasta targetfasta
 
     Build targetfasta based on info from agpfile
     """
     p = OptionParser(build.__doc__)
-    p.add_option(
+    p.add_argument(
         "--newagp",
         dest="newagp",
         default=False,
         action="store_true",
         help="Check components to trim dangling N's",
     )
-    p.add_option(
+    p.add_argument(
         "--novalidate",
         dest="novalidate",
         default=False,
         action="store_true",
         help="Don't validate the agpfile",
     )
     opts, args = p.parse_args(args)
@@ -2129,15 +2125,15 @@
         newagp = open(newagpfile, "w")
     else:
         newagpfile = None
         newagp = None
 
     agp = AGP(agpfile, validate=validate, sorted=True)
     agp.build_all(componentfasta=componentfasta, targetfasta=targetfasta, newagp=newagp)
-    logging.debug("Target fasta written to `%s`.", targetfasta)
+    logger.debug("Target fasta written to `%s`.", targetfasta)
 
     return newagpfile
 
 
 def validate(args):
     """
     %prog validate agpfile componentfasta targetfasta
@@ -2172,21 +2168,21 @@
                         chr=aline.component_id,
                         start=aline.component_beg,
                         stop=aline.component_end,
                         strand=aline.orientation,
                     )
                 )
 
-                assert build_seq.upper() == bac_seq.upper(), (
-                    "sequence mismatch: %s" % aline
-                )
+                assert (
+                    build_seq.upper() == bac_seq.upper()
+                ), f"sequence mismatch: {aline}"
 
-            logging.debug(
-                "%s:%d-%d verified" % (aline.object, aline.object_beg, aline.object_end)
+            logger.debug(
+                "%s:%d-%d verified", aline.object, aline.object_beg, aline.object_end
             )
 
         except Exception as e:
-            logging.error(e)
+            logger.error(e)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `jcvi-1.4.6/jcvi/formats/base.py` & `jcvi-1.4.7/jcvi/formats/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -566,15 +566,15 @@
 
     $ python -m jcvi.formats.base seqids chromosome_ 1 3
     chromosome_1,chromosome_2,chromosome_3
     $ python -m jcvi.formats.base seqids A 3 1 --pad0=2
     A03,A02,A01
     """
     p = OptionParser(seqids.__doc__)
-    p.add_option("--pad0", default=0, help="How many zeros to pad")
+    p.add_argument("--pad0", default=0, help="How many zeros to pad")
     opts, args = p.parse_args(args)
 
     if len(args) != 3:
         sys.exit(not p.print_help())
 
     prefix, start, end = args
     pad0 = opts.pad0
@@ -698,15 +698,15 @@
                              | 1,4
                              | 3,na
     """
     from itertools import zip_longest
 
     p = OptionParser(flatten.__doc__)
     p.set_sep(sep=",")
-    p.add_option(
+    p.add_argument(
         "--zipflatten",
         default=None,
         dest="zipsep",
         help="Specify if columns of the file should be zipped before"
         + " flattening. If so, specify delimiter separating column elements",
     )
     opts, args = p.parse_args(args)
@@ -737,15 +737,15 @@
 def unflatten(args):
     """
     %prog unflatten idsfile > unflattened
 
     Given a list of ids, one per line, unflatten the list onto a single line with sep.
     """
     p = OptionParser(unflatten.__doc__)
-    p.add_option("--sep", default=",", help="Separator when joining ids")
+    p.add_argument("--sep", default=",", help="Separator when joining ids")
     p.set_outfile()
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (idsfile,) = args
@@ -781,21 +781,21 @@
     By default, it uniqifies all the grouped elements
     """
     from jcvi.utils.cbook import AutoVivification
     from jcvi.utils.grouper import Grouper
 
     p = OptionParser(group.__doc__)
     p.set_sep()
-    p.add_option(
-        "--groupby", default=None, type="int", help="Default column to groupby"
+    p.add_argument(
+        "--groupby", default=None, type=int, help="Default column to groupby"
     )
-    p.add_option(
+    p.add_argument(
         "--groupsep", default=",", help="Separator to join the grouped elements"
     )
-    p.add_option(
+    p.add_argument(
         "--nouniq",
         default=False,
         action="store_true",
         help="Do not uniqify the grouped elements",
     )
     opts, args = p.parse_args(args)
 
@@ -894,22 +894,24 @@
     1. chunk - chunk records sequentially, 1-100 in file 1, 101-200 in file 2, etc.
     2. cycle - chunk records in Round Robin fashion
     3. optimal - try to make split file of roughly similar sizes, using LPT
     algorithm. This is the default.
     """
     p = OptionParser(split.__doc__)
     mode_choices = ("batch", "cycle", "optimal")
-    p.add_option("--all", default=False, action="store_true", help="split all records")
-    p.add_option(
+    p.add_argument(
+        "--all", default=False, action="store_true", help="split all records"
+    )
+    p.add_argument(
         "--mode",
         default="optimal",
         choices=mode_choices,
         help="Mode when splitting records",
     )
-    p.add_option(
+    p.add_argument(
         "--format", choices=("fasta", "fastq", "txt", "clust"), help="input file format"
     )
 
     opts, args = p.parse_args(args)
 
     if len(args) != 3:
         sys.exit(not p.print_help())
@@ -939,29 +941,29 @@
       Use comma to separate multiple values if the pivot column is different
       in each file. Maintain the order in the first file.
     --sep specifies the column separators, default to tab.
       Use comma to separate multiple values if the column separator is different
       in each file.
     """
     p = OptionParser(join.__doc__)
-    p.add_option(
+    p.add_argument(
         "--column", default="0", help="0-based column id, multiple values allowed"
     )
     p.set_sep(multiple=True)
-    p.add_option(
+    p.add_argument(
         "--noheader", default=False, action="store_true", help="Do not print header"
     )
-    p.add_option("--na", default="na", help="Value for unjoined data")
-    p.add_option(
+    p.add_argument("--na", default="na", help="Value for unjoined data")
+    p.add_argument(
         "--compact",
         default=False,
         action="store_true",
         help="Do not repeat pivotal columns in output",
     )
-    p.add_option(
+    p.add_argument(
         "--keysep",
         default=",",
         help="specify separator joining multiple elements in the key column"
         + " of the pivot file",
     )
     p.set_outfile()
 
@@ -1044,22 +1046,22 @@
       in each file. Maintain the order in the first file.
     --sep specifies the column separators, default to tab.
       Use comma to separate multiple values if the column separator is different
       in each file.
     """
 
     p = OptionParser(subset.__doc__)
-    p.add_option(
+    p.add_argument(
         "--column", default="0", help="0-based column id, multiple values allowed"
     )
     p.set_sep(multiple=True)
-    p.add_option(
+    p.add_argument(
         "--pivot",
         default=1,
-        type="int",
+        type=int,
         help="1 for using order in file1, 2 for using order in \
                     file2",
     )
     p.set_outfile()
 
     opts, args = p.parse_args(args)
     nargs = len(args)
@@ -1125,18 +1127,18 @@
     ^: symmetric difference (elementes found in either set but not both)
 
     Please quote the argument to avoid shell interpreting | and &.
     """
     from natsort import natsorted
 
     p = OptionParser(setop.__doc__)
-    p.add_option(
+    p.add_argument(
         "--column",
         default=0,
-        type="int",
+        type=int,
         help="The column to extract, 0-based, -1 to disable",
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
```

### Comparing `jcvi-1.4.6/jcvi/formats/bed.py` & `jcvi-1.4.7/jcvi/formats/bed.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,30 +14,30 @@
 
 import numpy as np
 
 from more_itertools import pairwise
 from natsort import natsorted, natsort_key
 
 from ..apps.base import (
-    OptionParser,
     ActionDispatcher,
+    OptionParser,
     cleanup,
     logger,
     need_update,
     popen,
     sh,
 )
-from ..utils.cbook import SummaryStats, thousands, percentage
+from ..utils.cbook import SummaryStats, percentage, thousands
 from ..utils.grouper import Grouper
 from ..utils.range import (
     Range,
-    range_union,
     range_chain,
     range_distance,
     range_intersect,
+    range_union,
 )
 
 from .base import DictFile, LineFile, get_number, is_number, must_open
 from .sizes import Sizes
 
 
 class BedLine(object):
@@ -499,23 +499,23 @@
     The bedfile contains 'covered' features by BLAST hits, while the output
     bedfile will contain 'uncovered' (i.e. gap) features, in that case use
     --missing to note if gap is missing in one or more seqids.
     """
     from pybedtools import BedTool
 
     p = OptionParser(gaps.__doc__)
-    p.add_option(
+    p.add_argument(
         "--na_in",
         help="Add '_na_in_xxx' to gap name, use comma to separate, "
         + "e.g. --na_in=chr1,chr2 to note if gap is missing in chr1 or "
         + "chr2, default is to not add anything. Note that if one of the "
         + "missing seqids happens to be the seqid of the current feature, "
         + "it will not be reported.",
     )
-    p.add_option("--minsize", default=1000, type="int", help="Minimum gap size")
+    p.add_argument("--minsize", default=1000, type=int, help="Minimum gap size")
     p.set_outfile()
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     inputbed, ref_fasta = args
@@ -556,15 +556,15 @@
 
     Find the closest feature in `features.bed` to `input.bed`.
     `features.bed` must be sorted using `jcvi.formats.bed sort`.
     """
     from pybedtools import BedTool
 
     p = OptionParser(closest.__doc__)
-    p.add_option("--maxdist", default=5000, help="Maximum distance")
+    p.add_argument("--maxdist", default=5000, help="Maximum distance")
     p.set_outfile()
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     inputbed, featuresbed = args
@@ -589,16 +589,16 @@
 def format(args):
     """
     %prog format input.bed
 
     Re-format BED file, e.g. switch sequence ids.
     """
     p = OptionParser(format.__doc__)
-    p.add_option("--prefix", help="Add prefix to name column (4th)")
-    p.add_option("--switch", help="Switch seqids based on two-column file")
+    p.add_argument("--prefix", help="Add prefix to name column (4th)")
+    p.add_argument("--switch", help="Switch seqids based on two-column file")
     p.set_outfile()
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (bedfile,) = args
@@ -656,18 +656,18 @@
     %prog tiling bedfile
 
     Compute minimum tiling path using as few clones as possible. Implemented
     with dynamic programming. Greedy algorithm may also work according a
     stackoverflow source.
     """
     p = OptionParser(tiling.__doc__)
-    p.add_option(
+    p.add_argument(
         "--overlap",
         default=3000,
-        type="int",
+        type=int,
         help="Minimum amount of overlaps required",
     )
     p.set_verbose()
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
@@ -735,15 +735,15 @@
 def chain(args):
     """
     %prog chain bedfile
 
     Chain BED segments together.
     """
     p = OptionParser(chain.__doc__)
-    p.add_option("--dist", default=100000, help="Chaining distance")
+    p.add_argument("--dist", default=100000, help="Chaining distance")
     p.set_outfile()
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (bedfile,) = args
@@ -880,17 +880,17 @@
 def seqids(args):
     """
     %prog seqids bedfile
 
     Print out all seqids on one line. Useful for graphics.karyotype.
     """
     p = OptionParser(seqids.__doc__)
-    p.add_option("--maxn", default=100, type="int", help="Maximum number of seqids")
-    p.add_option("--prefix", help="Seqids must start with")
-    p.add_option("--exclude", default="random", help="Seqids should not contain")
+    p.add_argument("--maxn", default=100, type=int, help="Maximum number of seqids")
+    p.add_argument("--prefix", help="Seqids must start with")
+    p.add_argument("--exclude", default="random", help="Seqids should not contain")
     opts, args = p.parse_args(args)
 
     if len(args) < 1:
         sys.exit(not p.print_help())
 
     (bedfile,) = args
     pf = opts.prefix
@@ -990,24 +990,24 @@
 def filter(args):
     """
     %prog filter bedfile
 
     Filter the bedfile to retain records between certain size range.
     """
     p = OptionParser(filter.__doc__)
-    p.add_option("--minsize", default=0, type="int", help="Minimum feature length")
-    p.add_option(
-        "--maxsize", default=1000000000, type="int", help="Minimum feature length"
+    p.add_argument("--minsize", default=0, type=int, help="Minimum feature length")
+    p.add_argument(
+        "--maxsize", default=1000000000, type=int, help="Minimum feature length"
     )
-    p.add_option(
+    p.add_argument(
         "--minaccn",
-        type="int",
+        type=int,
         help="Minimum value of accn, useful to filter based on coverage",
     )
-    p.add_option("--minscore", type="int", help="Minimum score")
+    p.add_argument("--minscore", type=int, help="Minimum score")
     p.set_outfile()
 
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
@@ -1056,15 +1056,15 @@
 def mergebydepth(args):
     """
     %prog mergebydepth reads.bed genome.fasta
 
     Similar to mergeBed, but only returns regions beyond certain depth.
     """
     p = OptionParser(mergebydepth.__doc__)
-    p.add_option("--mindepth", default=3, type="int", help="Minimum depth required")
+    p.add_argument("--mindepth", default=3, type=int, help="Minimum depth required")
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     bedfile, fastafile = args
     mindepth = opts.mindepth
@@ -1127,17 +1127,17 @@
     %prog longest bedfile fastafile
 
     Select longest feature within overlapping piles.
     """
     from jcvi.formats.sizes import Sizes
 
     p = OptionParser(longest.__doc__)
-    p.add_option("--maxsize", default=20000, type="int", help="Limit max size")
-    p.add_option("--minsize", default=60, type="int", help="Limit min size")
-    p.add_option(
+    p.add_argument("--maxsize", default=20000, type=int, help="Limit max size")
+    p.add_argument("--minsize", default=60, type=int, help="Limit min size")
+    p.add_argument(
         "--precedence", default="Medtr", help="Accessions with prefix take precedence"
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
@@ -1212,15 +1212,15 @@
 def fix(args):
     """
     %prog fix bedfile > newbedfile
 
     Fix non-standard bed files. One typical problem is start > end.
     """
     p = OptionParser(fix.__doc__)
-    p.add_option("--minspan", default=0, type="int", help="Enforce minimum span")
+    p.add_argument("--minspan", default=0, type=int, help="Enforce minimum span")
     p.set_outfile()
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (bedfile,) = args
@@ -1263,15 +1263,15 @@
 
     Retrieve a subset of bed features given a list of ids.
     """
     from jcvi.formats.base import SetFile
     from jcvi.utils.cbook import gene_name
 
     p = OptionParser(some.__doc__)
-    p.add_option(
+    p.add_argument(
         "-v",
         dest="inverse",
         default=False,
         action="store_true",
         help="Get the inverse, like grep -v",
     )
     p.set_outfile()
@@ -1310,16 +1310,18 @@
     %prog uniq bedfile
 
     Remove overlapping features with higher scores.
     """
     from jcvi.formats.sizes import Sizes
 
     p = OptionParser(uniq.__doc__)
-    p.add_option("--sizes", help="Use sequence length as score")
-    p.add_option("--mode", default="span", choices=("span", "score"), help="Pile mode")
+    p.add_argument("--sizes", help="Use sequence length as score")
+    p.add_argument(
+        "--mode", default="span", choices=("span", "score"), help="Pile mode"
+    )
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (bedfile,) = args
     uniqbedfile = bedfile.split(".")[0] + ".uniq.bed"
@@ -1400,23 +1402,23 @@
     %prog bins bedfile fastafile
 
     Bin bed lengths into each consecutive window. Use --subtract to remove bases
     from window, e.g. --subtract gaps.bed ignores the gap sequences.
     """
 
     p = OptionParser(bins.__doc__)
-    p.add_option("--binsize", default=100000, type="int", help="Size of the bins")
-    p.add_option("--subtract", help="Subtract bases from window")
-    p.add_option(
+    p.add_argument("--binsize", default=100000, type=int, help="Size of the bins")
+    p.add_argument("--subtract", help="Subtract bases from window")
+    p.add_argument(
         "--mode",
         default="span",
         choices=("span", "count", "score"),
         help="Accumulate feature based on",
     )
-    p.add_option(
+    p.add_argument(
         "--nomerge", default=False, action="store_true", help="Do not merge features"
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
@@ -1450,16 +1452,16 @@
     sbdict = dict(bed.sub_beds())
     for chr, chr_len in sorted(sizes.items()):
         chr_len = sizes[chr]
         subbeds = sbdict.get(chr, [])
         nbins, last_bin = get_nbins(chr_len, binsize)
 
         a = np.zeros(nbins)  # values
-        b = np.zeros(nbins, dtype="int")  # bases
-        c = np.zeros(nbins, dtype="int")  # count
+        b = np.zeros(nbins, dtype=int)  # bases
+        c = np.zeros(nbins, dtype=int)  # count
         b[:-1] = binsize
         b[-1] = last_bin
 
         for bb in subbeds:
             start, end = bb.start, bb.end
             startbin = start // binsize
             endbin = end // binsize
@@ -1502,15 +1504,15 @@
     %prog pile abedfile bbedfile > piles
 
     Call intersectBed on two bedfiles.
     """
     from jcvi.utils.grouper import Grouper
 
     p = OptionParser(pile.__doc__)
-    p.add_option("--minOverlap", default=0, type="int", help="Minimum overlap required")
+    p.add_argument("--minOverlap", default=0, type=int, help="Minimum overlap required")
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     abedfile, bbedfile = args
     iw = intersectBed_wao(abedfile, bbedfile, minOverlap=opts.minOverlap)
@@ -1531,16 +1533,16 @@
     """
     %prog index bedfile
 
     Compress and index bedfile using `tabix`. Use --fasta to give a FASTA file
     so that a bedgraph file can be generated and indexed.
     """
     p = OptionParser(index.__doc__)
-    p.add_option("--fasta", help="Generate bedgraph and index")
-    p.add_option("--query", help="Chromosome location")
+    p.add_argument("--fasta", help="Generate bedgraph and index")
+    p.add_argument("--query", help="Chromosome location")
     p.set_outfile()
 
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
@@ -1691,15 +1693,15 @@
     Sn = TP / (all true in reality) = TP / (TP + FN)
     Sp = TP / (all true in prediction) = TP / (TP + FP)
     Ac = (TP + TN) / (TP + FP + FN + TN)
     """
     from jcvi.formats.sizes import Sizes
 
     p = OptionParser(evaluate.__doc__)
-    p.add_option("--query", help="Chromosome location")
+    p.add_argument("--query", help="Chromosome location")
     opts, args = p.parse_args(args)
 
     if len(args) != 3:
         sys.exit(not p.print_help())
 
     prediction, reality, fastafile = args
     query = opts.query
@@ -1807,15 +1809,15 @@
     """
     %prog distance bedfile
 
     Calculate distance between bed features. The output file is a list of
     distances, which can be used to plot histogram, etc.
     """
     p = OptionParser(distance.__doc__)
-    p.add_option(
+    p.add_argument(
         "--distmode",
         default="ss",
         choices=("ss", "ee"),
         help="Distance mode between paired reads. ss is outer distance, "
         "ee is inner distance",
     )
     opts, args = p.parse_args(args)
@@ -1856,23 +1858,23 @@
     window from one another. One sweep goes from left to right, the other in
     the reverse direction.
     """
     import random
     from jcvi.assembly.coverage import Coverage
 
     p = OptionParser(sample.__doc__)
-    p.add_option(
+    p.add_argument(
         "--raindrop",
         default=0,
-        type="int",
+        type=int,
         help="Raindrop selection, ignores all other options",
     )
-    p.add_option("--max", default=10, type="int", help="Max depth allowed")
-    p.add_option(
-        "--targetsize", type="int", help="Sample bed file to get target base number"
+    p.add_argument("--max", default=10, type=int, help="Max depth allowed")
+    p.add_argument(
+        "--targetsize", type=int, help="Sample bed file to get target base number"
     )
     p.set_outfile()
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
@@ -1946,21 +1948,21 @@
 
     Convert to bedpe format. Use --span to write another bed file that contain
     the span of the read pairs.
     """
     from jcvi.assembly.coverage import bed_to_bedpe
 
     p = OptionParser(bedpe.__doc__)
-    p.add_option(
+    p.add_argument(
         "--span", default=False, action="store_true", help="Write span bed file"
     )
-    p.add_option(
+    p.add_argument(
         "--strand", default=False, action="store_true", help="Write the strand columns"
     )
-    p.add_option("--mates", help="Check the library stats from .mates file")
+    p.add_argument("--mates", help="Check the library stats from .mates file")
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (bedfile,) = args
     pf = bedfile.rsplit(".", 1)[0]
@@ -2094,15 +2096,15 @@
 
     # select only pairs with certain orientations - e.g. innies, outies, etc.
     if mateorientation:
         all_dist = [x for x in all_dist if x[1] == mateorientation]
 
     # try to infer cutoff as twice the median until convergence
     if cutoff <= 0:
-        dists = np.array([x[0] for x in all_dist], dtype="int")
+        dists = np.array([x[0] for x in all_dist], dtype=int)
         p0 = analyze_dists(dists, cutoff=mpcutoff)
         cutoff = int(2 * p0)  # initial estimate
         cutoff = int(math.ceil(cutoff / bins)) * bins
         logger.debug("Insert size cutoff set to %d, use '--cutoff' to override", cutoff)
 
     for dist, orientation, aquery, bquery in all_dist:
         if dist > cutoff:
@@ -2118,15 +2120,15 @@
     print(
         "{0} fragments, {1} pairs ({2} total)".format(
             num_fragments, num_pairs, num_fragments + num_pairs * 2
         ),
         file=sys.stderr,
     )
 
-    s = SummaryStats(linked_dist, dtype="int")
+    s = SummaryStats(linked_dist, dtype=int)
     num_links = s.size
 
     meandist, stdev = s.mean, s.sd
     p0, p1, p2 = s.median, s.p1, s.p2
 
     print(
         "%d pairs (%.1f%%) are linked (cutoff=%d)"
@@ -2211,18 +2213,18 @@
 def summary(args):
     """
     %prog summary bedfile
 
     Sum the total lengths of the intervals.
     """
     p = OptionParser(summary.__doc__)
-    p.add_option(
+    p.add_argument(
         "--sizes", default=False, action="store_true", help="Write .sizes file"
     )
-    p.add_option(
+    p.add_argument(
         "--all",
         default=False,
         action="store_true",
         help="Write summary stats per seqid",
     )
     opts, args = p.parse_args(args)
 
@@ -2254,36 +2256,36 @@
     """
     %prog sort bedfile
 
     Sort bed file to have ascending order of seqid, then start. It uses the
     `sort` command.
     """
     p = OptionParser(sort.__doc__)
-    p.add_option(
+    p.add_argument(
         "-i",
         "--inplace",
         dest="inplace",
         default=False,
         action="store_true",
         help="Sort bed file in place",
     )
-    p.add_option(
+    p.add_argument(
         "-u",
         dest="unique",
         default=False,
         action="store_true",
         help="Uniqify the bed file",
     )
-    p.add_option(
+    p.add_argument(
         "--accn",
         default=False,
         action="store_true",
         help="Sort based on the accessions",
     )
-    p.add_option(
+    p.add_argument(
         "--num",
         default=False,
         action="store_true",
         help="Numerically sort seqid column, e.g. chr1,chr2,...",
     )
     p.set_outfile(outfile=None)
     p.set_tmpdir()
@@ -2329,27 +2331,27 @@
 def mates(args):
     """
     %prog mates bedfile
 
     Generate the mates file by inferring from the names.
     """
     p = OptionParser(mates.__doc__)
-    p.add_option(
+    p.add_argument(
         "--lib",
         default=False,
         action="store_true",
         help="Output library information along with pairs",
     )
-    p.add_option(
+    p.add_argument(
         "--nointra",
         default=False,
         action="store_true",
         help="Remove mates that are intra-scaffold",
     )
-    p.add_option(
+    p.add_argument(
         "--prefix",
         default=False,
         action="store_true",
         help="Only keep links between IDs with same prefix",
     )
     p.set_mates()
 
@@ -2427,34 +2429,34 @@
     %prog flanking bedfile [options]
 
     Get up to n features (upstream or downstream or both) flanking a given position.
     """
     from numpy import array, argsort
 
     p = OptionParser(flanking.__doc__)
-    p.add_option(
+    p.add_argument(
         "--chrom",
         default=None,
-        type="string",
+        type=str,
         help="chrom name of the position in query. Make sure it matches bedfile.",
     )
-    p.add_option(
-        "--coord", default=None, type="int", help="coordinate of the position in query."
+    p.add_argument(
+        "--coord", default=None, type=int, help="coordinate of the position in query."
     )
-    p.add_option(
-        "-n", default=10, type="int", help="number of flanking features to get"
+    p.add_argument(
+        "-n", default=10, type=int, help="number of flanking features to get"
     )
-    p.add_option(
+    p.add_argument(
         "--side",
         default="both",
         choices=("upstream", "downstream", "both"),
         help="which side to get flanking features",
     )
-    p.add_option(
-        "--max_d", default=None, type="int", help="features <= max_d away from position"
+    p.add_argument(
+        "--max_d", default=None, type=int, help="features <= max_d away from position"
     )
     p.set_outfile()
 
     opts, args = p.parse_args(args)
 
     if any([len(args) != 1, opts.chrom is None, opts.coord is None]):
         sys.exit(not p.print_help())
```

### Comparing `jcvi-1.4.6/jcvi/formats/blast.py` & `jcvi-1.4.7/jcvi/formats/blast.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
 parses tabular BLAST -m8 (-format 6 in BLAST+) format
 """
 
 import os.path as op
 import sys
-import logging
 
 from itertools import groupby
 from collections import defaultdict
 
-from jcvi.formats.base import LineFile, BaseFile, must_open
-from jcvi.formats.bed import Bed
-from jcvi.formats.sizes import Sizes
-from jcvi.utils.grouper import Grouper
-from jcvi.utils.orderedcollections import OrderedDict
-from jcvi.utils.range import range_distance
-from jcvi.utils.cbook import percentage
-from jcvi.assembly.base import calculate_A50
-from jcvi.apps.base import OptionParser, ActionDispatcher, sh, popen
+from ..apps.base import ActionDispatcher, OptionParser, logger, popen, sh
+from ..assembly.base import calculate_A50
 from ..compara.base import AnchorFile
+from ..utils.cbook import percentage
+from ..utils.grouper import Grouper
+from ..utils.orderedcollections import OrderedDict
+from ..utils.range import range_distance
+
+from .base import LineFile, BaseFile, must_open
+from .bed import Bed
+from .sizes import Sizes
 
 
 try:
     from .cblast import BlastLine
 except:
     from .pyblast import BlastLine
 
-    logging.error("Fall back to Python implementation of BlastLine")
+    logger.error("Fall back to Python implementation of BlastLine")
 
 
 class BlastSlow(LineFile):
     """
     Load entire blastfile into memory
     """
 
@@ -216,15 +216,15 @@
         print("\n".join((m0, m1, m2, m3, m4)), file=sys.stderr)
 
 
 def get_stats(blastfile, strict=False):
     from jcvi.utils.range import range_union, range_span
     from .pyblast import BlastLine
 
-    logging.debug("Report stats on `%s`" % blastfile)
+    logger.debug("Report stats on `%s`" % blastfile)
     fp = open(blastfile)
     ref_ivs = []
     qry_ivs = []
     identicals = 0
     ngaps = 0
     alignlens = []
 
@@ -292,21 +292,21 @@
     - ids: valid ids
 
     Use --inverse to obtain the complementary records for the criteria above.
 
     - noself: remove self-self hits
     """
     p = OptionParser(filter.__doc__)
-    p.add_option("--score", dest="score", default=0, type="int", help="Score cutoff")
+    p.add_argument("--score", dest="score", default=0, type=int, help="Score cutoff")
     p.set_align(pctid=95, hitlen=100, evalue=0.01)
-    p.add_option(
+    p.add_argument(
         "--noself", default=False, action="store_true", help="Remove self-self hits"
     )
-    p.add_option("--ids", help="Path to file with ids to retain")
-    p.add_option(
+    p.add_argument("--ids", help="Path to file with ids to retain")
+    p.add_argument(
         "--inverse",
         default=False,
         action="store_true",
         help="Similar to grep -v, inverse",
     )
     p.set_outfile(outfile=None)
 
@@ -426,19 +426,19 @@
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (blastfile,) = args
     blast = BlastSlow(blastfile)
-    logging.debug("A total of {} records imported".format(len(blast)))
+    logger.debug("A total of {} records imported".format(len(blast)))
 
     query_gaps = list(collect_gaps(blast))
     subject_gaps = list(collect_gaps(blast, use_subject=True))
-    logging.debug(
+    logger.debug(
         "Query gaps: {}  Subject gaps: {}".format(len(query_gaps), len(subject_gaps))
     )
 
     from jcvi.graphics.base import savefig
     import seaborn as sns
 
     sns.distplot(query_gaps)
@@ -505,15 +505,15 @@
     for b in blast:
         query = b.query
         subject = b.subject
         if subject not in ids:
             continue
         scores[query] += b.score
 
-    logging.debug("A total of {0} ids loaded.".format(len(ids)))
+    logger.debug("A total of {0} ids loaded.".format(len(ids)))
 
     f = Fasta(fastafile)
     for s in f.iterkeys_ordered():
         sc = scores.get(s, 0)
         print("\t".join((s, str(sc))))
 
 
@@ -523,16 +523,16 @@
 
     Create simple two column files from the first two coluns in blastfile. Use
     --queryids and --subjectids to switch IDs or descriptions.
     """
     from jcvi.formats.base import DictFile
 
     p = OptionParser(annotation.__doc__)
-    p.add_option("--queryids", help="Query IDS file to switch")
-    p.add_option("--subjectids", help="Subject IDS file to switch")
+    p.add_argument("--queryids", help="Query IDS file to switch")
+    p.add_argument("--subjectids", help="Subject IDS file to switch")
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (blastfile,) = args
 
@@ -558,15 +558,15 @@
     BLAST sugarcane ESTs against sorghum annotations as reference, to find
     full-length transcripts.
     """
     from jcvi.utils.range import range_minmax
     from jcvi.utils.cbook import SummaryStats
 
     p = OptionParser(completeness.__doc__)
-    p.add_option("--ids", help="Save ids that are over 50% complete")
+    p.add_argument("--ids", help="Save ids that are over 50% complete")
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     blastfile, fastafile = args
     idsfile = opts.ids
@@ -605,15 +605,15 @@
     m += "C-terminal: {0}\n".format(SummaryStats(cd))
     m += "Coverage: {0}".format(SummaryStats(cv))
     print(m, file=sys.stderr)
 
     if idsfile:
         fw = open(idsfile, "w")
         print("\n".join(valid), file=fw)
-        logging.debug(
+        logger.debug(
             "A total of {0} ids (cov > {1} %) written to `{2}`.".format(
                 len(valid), cutoff, idsfile
             )
         )
         fw.close()
 
 
@@ -623,26 +623,26 @@
 
     Annotate overlap types (dovetail, contained, etc) in BLAST tabular file.
     """
     from jcvi.assembly.goldenpath import Cutoff, Overlap, Overlap_types
 
     p = OptionParser(annotate.__doc__)
     p.set_align(pctid=94, hitlen=500)
-    p.add_option("--hang", default=500, type="int", help="Maximum overhang length")
+    p.add_argument("--hang", default=500, type=int, help="Maximum overhang length")
     opts, args = p.parse_args(args)
 
     if len(args) != 3:
         sys.exit(not p.print_help())
 
     blastfile, afasta, bfasta = args
     fp = must_open(blastfile)
     asizes = Sizes(afasta).mapping
     bsizes = Sizes(bfasta).mapping
     cutoff = Cutoff(opts.pctid, opts.hitlen, opts.hang)
-    logging.debug(str(cutoff))
+    logger.debug(str(cutoff))
     for row in fp:
         b = BlastLine(row)
         asize = asizes[b.query]
         bsize = bsizes[b.subject]
         if b.query == b.subject:
             continue
         ov = Overlap(b, asize, bsize, cutoff)
@@ -661,21 +661,21 @@
 
     The ids file is two-column, and can sometimes be generated by
     `jcvi.formats.fasta ids --description`.
     """
     from jcvi.formats.base import DictFile
 
     p = OptionParser(top10.__doc__)
-    p.add_option(
+    p.add_argument(
         "--top",
         default=10,
-        type="int",
+        type=int,
         help="Top N taxa to extract",
     )
-    p.add_option(
+    p.add_argument(
         "--ids",
         default=None,
         help="Two column ids file to query seqid",
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
@@ -697,33 +697,33 @@
     """
     %prog sort <blastfile|coordsfile>
 
     Sort lines so that same query grouped together with scores descending. The
     sort is 'in-place'.
     """
     p = OptionParser(sort.__doc__)
-    p.add_option(
+    p.add_argument(
         "--query",
         default=False,
         action="store_true",
         help="Sort by query position",
     )
-    p.add_option(
+    p.add_argument(
         "--ref",
         default=False,
         action="store_true",
         help="Sort by reference position",
     )
-    p.add_option(
+    p.add_argument(
         "--refscore",
         default=False,
         action="store_true",
         help="Sort by reference name, then score descending",
     )
-    p.add_option(
+    p.add_argument(
         "--coords",
         default=False,
         action="store_true",
         help="File is .coords generated by NUCMER",
     )
     p.set_tmpdir()
 
@@ -770,27 +770,27 @@
 
     Output file will be 3-column (query, subject, cscore). Use --cutoff to
     select a different cutoff.
     """
     from jcvi.utils.cbook import gene_name
 
     p = OptionParser(cscore.__doc__)
-    p.add_option(
+    p.add_argument(
         "--cutoff",
         default=0.9999,
-        type="float",
+        type=float,
         help="Minimum C-score to report",
     )
-    p.add_option(
+    p.add_argument(
         "--pct",
         default=False,
         action="store_true",
         help="Also include pct as last column",
     )
-    p.add_option(
+    p.add_argument(
         "--writeblast",
         default=False,
         action="store_true",
         help="Also write filtered blast file",
     )
     p.set_stripnames()
     p.set_outfile()
@@ -802,15 +802,15 @@
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (blastfile,) = args
 
     blast = Blast(blastfile)
-    logging.debug("Register best scores ..")
+    logger.debug("Register best scores ..")
     best_score = defaultdict(float)
     for b in blast:
         query, subject = b.query, b.subject
         if ostrip:
             query, subject = gene_name(query), gene_name(subject)
 
         score = b.score
@@ -935,35 +935,35 @@
 def chain(args):
     """
     %prog chain blastfile
 
     Chain adjacent HSPs together to form larger HSP.
     """
     p = OptionParser(chain.__doc__)
-    p.add_option(
+    p.add_argument(
         "--dist",
         dest="dist",
         default=100,
-        type="int",
+        type=int,
         help="extent of flanking regions to search",
     )
 
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (blastfile,) = args
     dist = opts.dist
     assert dist > 0
 
     blast = BlastSlow(blastfile)
-    logging.debug("A total of {} records imported".format(len(blast)))
+    logger.debug("A total of {} records imported".format(len(blast)))
     chained_hsps = chain_HSPs(blast, xdist=dist, ydist=dist)
-    logging.debug("A total of {} records after chaining".format(len(chained_hsps)))
+    logger.debug("A total of {} records after chaining".format(len(chained_hsps)))
 
     for b in chained_hsps:
         print(b)
 
 
 def condense(args):
     """
@@ -1038,37 +1038,37 @@
     from jcvi.algorithms.supermap import supermap
     from jcvi.utils.range import range_union
 
     allowed_iterby = ("query", "query_sbjct")
 
     p = OptionParser(covfilter.__doc__)
     p.set_align(pctid=95, pctcov=50)
-    p.add_option(
+    p.add_argument(
         "--scov",
         default=False,
         action="store_true",
         help="Subject coverage instead of query",
     )
-    p.add_option(
+    p.add_argument(
         "--supermap", action="store_true", help="Use supermap instead of union"
     )
-    p.add_option(
+    p.add_argument(
         "--ids",
         dest="ids",
         default=None,
         help="Print out the ids that satisfy",
     )
-    p.add_option(
+    p.add_argument(
         "--list",
         dest="list",
         default=False,
         action="store_true",
         help="List the id% and cov% per gene",
     )
-    p.add_option(
+    p.add_argument(
         "--iterby",
         dest="iterby",
         default="query",
         choices=allowed_iterby,
         help="Choose how to iterate through BLAST",
     )
     p.set_outfile(outfile=None)
@@ -1207,15 +1207,15 @@
     fw.close()
 
     if opts.ids:
         filename = opts.ids
         fw = must_open(filename, "w")
         for id in valid:
             print(id, file=fw)
-        logging.debug(
+        logger.debug(
             "Queries beyond cutoffs {0} written to `{1}`.".format(
                 cutoff_message, filename
             )
         )
 
     outfile = opts.outfile
     if not outfile:
@@ -1260,30 +1260,30 @@
 
     Print out bed file based on coordinates in BLAST report. By default, write
     out subject positions. Use --swap to write query positions.
     """
     from .bed import sort as bed_sort, mergeBed
 
     p = OptionParser(bed.__doc__)
-    p.add_option(
+    p.add_argument(
         "--swap",
         default=False,
         action="store_true",
         help="Write query positions",
     )
-    p.add_option(
+    p.add_argument(
         "--both",
         default=False,
         action="store_true",
         help="Generate one line for each of query and subject",
     )
-    p.add_option(
+    p.add_argument(
         "--merge",
         default=None,
-        type="int",
+        type=int,
         help="Merge hits within this distance",
     )
 
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(p.print_help())
@@ -1302,15 +1302,15 @@
     for row in fp:
         b = BlastLine(row)
         if positive:
             print(b.bedline, file=fw)
         if negative:
             print(b.swapped.bedline, file=fw)
 
-    logging.debug("File written to `%s`.", bedfile)
+    logger.debug("File written to `%s`.", bedfile)
     fw.close()
     bed_sort([bedfile, "-i"])
     if opts.merge:
         mergeBed(bedfile, sorted=True, d=opts.merge, inplace=True)
 
     return bedfile
 
@@ -1341,15 +1341,15 @@
 
     Extract a subset of the BLAST file based on the anchors file. The anchors
     file is a tab-delimited file with two columns, likely generated from synteny
     pipeline. This is useful to filter down BLAST.
     """
     p = OptionParser(anchors.__doc__)
     p.set_outfile()
-    p.add_option(
+    p.add_argument(
         "--best", default=False, action="store_true", help="Keep only the best hit"
     )
     opts, args = p.parse_args(args)
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     blastfile, anchorsfile = args
@@ -1364,39 +1364,39 @@
         if pp in anchor_pairs:
             found += 1
             if opts.best and pp in seen:
                 continue
             print(rec, file=fw)
             seen.add(pp)
         total += 1
-    logging.info("Found %s", percentage(found, total))
+    logger.info("Found %s", percentage(found, total))
 
 
 def best(args):
     """
     %prog best blastfile
 
     print the best hit for each query in the blastfile
     """
     p = OptionParser(best.__doc__)
 
-    p.add_option("-n", default=1, type="int", help="get best N hits")
-    p.add_option(
+    p.add_argument("-n", default=1, type=int, help="get best N hits")
+    p.add_argument(
         "--nosort",
         default=False,
         action="store_true",
         help="assume BLAST is already sorted",
     )
-    p.add_option(
+    p.add_argument(
         "--hsps",
         default=False,
         action="store_true",
         help="get all HSPs for the best pair",
     )
-    p.add_option(
+    p.add_argument(
         "--subject",
         default=False,
         action="store_true",
         help="get best hit(s) for subject genome instead",
     )
     p.set_tmpdir()
     opts, args = p.parse_args(args)
@@ -1414,15 +1414,15 @@
         sargs = [blastfile]
         if tmpdir:
             sargs += ["-T {0}".format(tmpdir)]
         if ref != "query":
             sargs += ["--refscore"]
         sort(sargs)
     else:
-        logging.debug("Assuming sorted BLAST")
+        logger.debug("Assuming sorted BLAST")
 
     if not opts.subject:
         bestblastfile = blastfile + ".best"
     else:
         bestblastfile = blastfile + ".subject.best"
     fw = open(bestblastfile, "w")
 
@@ -1441,21 +1441,21 @@
     comparing genomes (based on NUCMER results).
 
     Columns:
     filename, identicals, qrycovered, pct_qrycovered, refcovered, pct_refcovered,
     qryspan, pct_qryspan, refspan, pct_refspan
     """
     p = OptionParser(summary.__doc__)
-    p.add_option(
+    p.add_argument(
         "--strict",
         default=False,
         action="store_true",
         help="Strict 'gapless' mode. Exclude gaps from covered base.",
     )
-    p.add_option(
+    p.add_argument(
         "--tabular",
         default=False,
         action="store_true",
         help="Print succint tabular output",
     )
 
     opts, args = p.parse_args(args)
@@ -1479,25 +1479,25 @@
     Extract blast hits between given query and subject chrs.
 
     If --qchrs or --schrs is not given, then all chrs from q/s genome will
     be included. However one of --qchrs and --schrs must be specified.
     Otherwise the script will do nothing.
     """
     p = OptionParser(subset.__doc__)
-    p.add_option(
+    p.add_argument(
         "--qchrs",
         default=None,
         help="query chrs to extract, comma sep",
     )
-    p.add_option(
+    p.add_argument(
         "--schrs",
         default=None,
         help="subject chrs to extract, comma sep",
     )
-    p.add_option(
+    p.add_argument(
         "--convert",
         default=False,
         action="store_true",
         help="convert accns to chr_rank",
     )
     opts, args = p.parse_args(args)
 
@@ -1532,12 +1532,12 @@
         q, s = b.query, b.subject
         if qo[q][1].seqid in qchrs and so[s][1].seqid in schrs:
             if convert:
                 b.query = qo[q][1].seqid + "_" + "{0:05d}".format(qo[q][0])
                 b.subject = so[s][1].seqid + "_" + "{0:05d}".format(so[s][0])
             print(b, file=fw)
     fw.close()
-    logging.debug("Subset blastfile written to `{0}`".format(outfile))
+    logger.debug("Subset blastfile written to `{0}`".format(outfile))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `jcvi-1.4.6/jcvi/formats/cblast.pyx` & `jcvi-1.4.7/jcvi/formats/cblast.pyx`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.6/jcvi/formats/cdt.py` & `jcvi-1.4.7/jcvi/formats/cdt.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 """
 %prog data.cdt data.nwk
 
 Convert the result from Eisen's CLUSTER program: data.gtr and data.cdt into NEWICK format
 """
 
-import sys
 import csv
-import logging
+import sys
 
 from collections import namedtuple
 from itertools import groupby
 
-from jcvi.apps.base import OptionParser
-from jcvi.formats.base import BaseFile
+from ..apps.base import OptionParser, logger
+
+from .base import BaseFile
 
 
 GTRLine = namedtuple("GTRLine", "parent left_child right_child dist")
 
 
 class CDT(BaseFile):
     def __init__(self, filename):
@@ -68,15 +68,15 @@
             nodes[parent_name] = (node, parent_dist)
 
         self.gtr_tree = node
 
     def print_newick(self, nwk_file):
 
         self.gtr_tree.write(format=5, outfile=nwk_file)
-        logging.debug("Newick tree written to `{0}`".format(nwk_file))
+        logger.debug("Newick tree written to `%s`", nwk_file)
 
     def iter_partitions(self, cutoff=0.3, gtr=True):
         from jcvi.utils.grouper import Grouper
 
         if gtr:
             names = self.gnames
             fp = open(self.gtrfile)
```

### Comparing `jcvi-1.4.6/jcvi/formats/chain.py` & `jcvi-1.4.7/jcvi/formats/chain.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 
 NOTE: The last line of the alignment section contains only one number: the ungapped
 alignment size of the last block.
 """
 
 import os.path as op
 import sys
-import logging
 
-from jcvi.formats.base import BaseFile, read_block
-from jcvi.apps.base import OptionParser, ActionDispatcher, sh, need_update, which
+from ..apps.base import ActionDispatcher, OptionParser, logger, need_update, sh, which
+
+from .base import BaseFile, read_block
 
 
 class ChainLine(object):
     def __init__(self, chain, lines):
         self.chain = chain
         self.blocks = []
         for line in lines:
@@ -132,15 +132,15 @@
     Generate chain file from AGP format. The components represent the old
     genome (target) and the objects represent new genome (query).
     """
     from jcvi.formats.agp import AGP
     from jcvi.formats.sizes import Sizes
 
     p = OptionParser(fromagp.__doc__)
-    p.add_option(
+    p.add_argument(
         "--novalidate", default=False, action="store_true", help="Do not validate AGP"
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 3:
         sys.exit(not p.print_help())
 
@@ -197,15 +197,15 @@
         )
         alignmentline = size
         print(headerline, file=fw)
         print(alignmentline, file=fw)
         print(file=fw)
 
     fw.close()
-    logging.debug("File written to `%s`.", chainfile)
+    logger.debug("File written to `%s`.", chainfile)
 
 
 def faToTwoBit(fastafile):
     twobitfile = fastafile.rsplit(".", 1)[0] + ".2bit"
     cmd = "faToTwoBit {0} {1}".format(fastafile, twobitfile)
     if need_update(fastafile, twobitfile):
         sh(cmd)
@@ -215,24 +215,24 @@
 def blat(args):
     """
     %prog blat old.fasta new.fasta
 
     Generate psl file using blat.
     """
     p = OptionParser(blat.__doc__)
-    p.add_option(
+    p.add_argument(
         "--minscore",
         default=100,
-        type="int",
+        type=int,
         help="Matches minus mismatches gap penalty",
     )
-    p.add_option(
+    p.add_argument(
         "--minid",
         default=98,
-        type="int",
+        type=int,
         help="Minimum sequence identity",
     )
     p.set_cpus()
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
```

### Comparing `jcvi-1.4.6/jcvi/formats/contig.py` & `jcvi-1.4.7/jcvi/formats/contig.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 """
 TIGR contig format, see spec:
 
 <http://www.cbcb.umd.edu/research/contig_representation.shtml#contig>
 """
 
 import sys
-import logging
 
-from jcvi.formats.base import BaseFile, read_block
-from jcvi.apps.base import OptionParser, ActionDispatcher
+from ..apps.base import ActionDispatcher, OptionParser, logger
+
+from .base import BaseFile, read_block
 
 
 class ReadLine(object):
     def __init__(self, row, contig):
         # '#16(0) [RC] 3046 bases, 00000000 checksum. {3046 1} <1 3046>'
         assert row[0] == "#"
         self.id = row.strip("#").split("(")[0]
@@ -144,16 +144,16 @@
             conrange = "<{0} {1}>".format(b.start, b.end)
             readline = "#{0}(0){1} {2} bases, {3} {4} {5}".format(
                 read, rc, readlen, checksum, readrange, conrange
             )
             print(readline, file=fw)
             print(fill(readseq.seq), file=fw)
 
-    logging.debug("Mapped contigs written to `{0}`.".format(contigfile))
-    logging.debug("Contig IDs written to `{0}`.".format(idsfile))
+    logger.debug("Mapped contigs written to `{0}`.".format(contigfile))
+    logger.debug("Contig IDs written to `{0}`.".format(idsfile))
 
 
 def bed(args):
     """
     %prog bed contigfile
 
     Prints out the contigs and their associated reads.
@@ -169,14 +169,14 @@
     fw = open(bedfile, "w")
     c = ContigFile(contigfile)
 
     for rec in c.iter_records():
         for r in rec.reads:
             print(r.bedline, file=fw)
 
-    logging.debug("File written to `%s`.", bedfile)
+    logger.debug("File written to `%s`.", bedfile)
 
     return bedfile
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `jcvi-1.4.6/jcvi/formats/coords.py` & `jcvi-1.4.7/jcvi/formats/coords.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 """
 parses JCVI software NUCMER (http://mummer.sourceforge.net/manual/)
 output - mostly as *.coords file.
 """
-import sys
-import logging
 import os.path as op
+import sys
 
-from math import exp
 from itertools import groupby
+from math import exp
+
+from ..apps.base import (
+    ActionDispatcher,
+    OptionParser,
+    get_abs_path,
+    logger,
+    need_update,
+    sh,
+)
+from ..assembly.base import calculate_A50
 
-from jcvi.formats.base import LineFile, must_open
-from jcvi.formats.blast import AlignStats
-from jcvi.assembly.base import calculate_A50
-from jcvi.apps.base import OptionParser, ActionDispatcher, sh, need_update, get_abs_path
+from .base import LineFile, must_open
+from .blast import AlignStats
 
 
 Overlap_types = ("none", "a ~ b", "b ~ a", "a in b", "b in a")
 
 
 class CoordsLine(object):
     """
@@ -241,15 +248,15 @@
         return best_hits
 
 
 def get_stats(coordsfile):
 
     from jcvi.utils.range import range_union
 
-    logging.debug("Report stats on `%s`" % coordsfile)
+    logger.debug("Report stats on `%s`", coordsfile)
     coords = Coords(coordsfile)
     ref_ivs = []
     qry_ivs = []
     identicals = 0
     alignlen = 0
     alignlens = []
 
@@ -384,19 +391,19 @@
 
     Report the coverage per query record, useful to see which query matches
     reference.  The coords file MUST be filtered with supermap::
 
     jcvi.algorithms.supermap --filter query
     """
     p = OptionParser(coverage.__doc__)
-    p.add_option(
+    p.add_argument(
         "-c",
         dest="cutoff",
         default=0.5,
-        type="float",
+        type=float,
         help="only report query with coverage greater than",
     )
 
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
@@ -430,21 +437,21 @@
     """
     %prog annotate coordsfile
 
     Annotate coordsfile to append an additional column, with the following
     overlaps: {0}.
     """
     p = OptionParser(annotate.__doc__.format(", ".join(Overlap_types)))
-    p.add_option(
+    p.add_argument(
         "--maxhang",
         default=100,
-        type="int",
+        type=int,
         help="Max hang to call dovetail overlap",
     )
-    p.add_option(
+    p.add_argument(
         "--all",
         default=False,
         action="store_true",
         help="Output all lines [default: terminal/containment]",
     )
 
     opts, args = p.parse_args(args)
@@ -472,15 +479,15 @@
     """
     %prog summary coordsfile
 
     provide summary on id% and cov%, for both query and reference
     """
 
     p = OptionParser(summary.__doc__)
-    p.add_option(
+    p.add_argument(
         "-s",
         dest="single",
         default=False,
         action="store_true",
         help="provide stats per reference seq",
     )
 
@@ -499,15 +506,15 @@
     %prog filter <deltafile|coordsfile>
 
     Produce a new delta/coords file and filter based on id% or cov%.
     Use `delta-filter` for .delta file.
     """
     p = OptionParser(filter.__doc__)
     p.set_align(pctid=0, hitlen=0)
-    p.add_option(
+    p.add_argument(
         "--overlap",
         default=False,
         action="store_true",
         help="Print overlap status (e.g. terminal, contained)",
     )
 
     opts, args = p.parse_args(args)
@@ -559,31 +566,31 @@
     """
     %prog bed coordsfile
 
     will produce a bed list of mapped position and orientation (needs to
     be beyond quality cutoff, say 50) in bed format
     """
     p = OptionParser(bed.__doc__)
-    p.add_option(
+    p.add_argument(
         "--query",
         default=False,
         action="store_true",
         help="print out query intervals rather than ref",
     )
-    p.add_option(
+    p.add_argument(
         "--pctid",
         default=False,
         action="store_true",
         help="use pctid in score",
     )
-    p.add_option(
+    p.add_argument(
         "--cutoff",
         dest="cutoff",
         default=0,
-        type="float",
+        type=float,
         help="get all the alignments with quality above threshold",
     )
 
     opts, args = p.parse_args(args)
     if len(args) != 1:
         sys.exit(p.print_help())
```

### Comparing `jcvi-1.4.6/jcvi/formats/excel.py` & `jcvi-1.4.7/jcvi/formats/excel.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,16 @@
 
 http://www.simplistix.co.uk/presentations/python-excel.pdf
 
 Library dependency: xlutils
 """
 import os.path as op
 import sys
-import logging
 
-from jcvi.apps.base import OptionParser, ActionDispatcher
+from ..apps.base import ActionDispatcher, OptionParser, logger
 
 
 class ColorMatcher(object):
     def __init__(self):
         self.reset()
 
     def reset(self):
@@ -115,17 +114,17 @@
         if isinstance(color, int):
             return color
         if color:
             if isinstance(color, str):
                 rgb = map(int, color.split(","))
             else:
                 rgb = color.Get()
-            logging.disable(logging.DEBUG)
+            logger.disable(logger.DEBUG)
             distances = [color_diff(rgb, x) for x in self.xlwt_colors]
-            logging.disable(logging.NOTSET)
+            logger.disable(logger.NOTSET)
             result = distances.index(min(distances))
             self.unused_colors.discard(self.xlwt_colors[result])
             return result
 
     def get_unused_color(self):
         """Returns an xlwt color index that has not been previously returned by
         this instance.  Attempts to maximize the distance between the color and
@@ -161,21 +160,21 @@
     Convert csv file to EXCEL.
     """
     from csv import reader
     from xlwt import Workbook, easyxf
     from jcvi.formats.base import flexible_cast
 
     p = OptionParser(fromcsv.__doc__)
-    p.add_option(
+    p.add_argument(
         "--noheader",
         default=False,
         action="store_true",
         help="Do not treat the first row as header",
     )
-    p.add_option("--rgb", default=-1, type="int", help="Show RGB color box")
+    p.add_argument("--rgb", default=-1, type=int, help="Show RGB color box")
     p.set_sep()
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (csvfile,) = args
@@ -206,15 +205,15 @@
                     cix = cm.match_color_index(cell)
                     color_style = easyxf("font: color_index {0}".format(cix))
                     s.write(i, j, cell, color_style)
                 else:
                     s.write(i, j, cell)
 
     w.save(excelfile)
-    logging.debug("File written to `%s`.", excelfile)
+    logger.debug("File written to `%s`.", excelfile)
     return excelfile
 
 
 def csv(args):
     """
     %prog csv excelfile
```

### Comparing `jcvi-1.4.6/jcvi/formats/fasta.py` & `jcvi-1.4.7/jcvi/formats/fasta.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 """
 Wrapper for biopython Fasta, add option to parse sequence headers
 """
 
-import re
-import sys
+import hashlib
 import os.path as op
+import re
 import shutil
-import logging
 import string
-import hashlib
-
-from random import choice
+import sys
 
 from itertools import groupby, zip_longest
-from more_itertools import grouper, pairwise
+from random import choice
 
 from Bio import SeqIO
 from Bio.Seq import Seq
 from Bio.SeqRecord import SeqRecord
 from Bio.SeqUtils.CheckSum import seguid
+from more_itertools import grouper, pairwise
 
-from ..apps.base import OptionParser, ActionDispatcher, cleanup, need_update
+from ..apps.base import ActionDispatcher, OptionParser, cleanup, logger, need_update
 from ..utils.cbook import percentage
 from ..utils.console import printf
 from ..utils.table import write_csv
 
 from .base import BaseFile, DictFile, must_open
 from .bed import Bed
 
@@ -114,22 +112,22 @@
         start = start - 1 if start is not None else 0
         stop = stop if stop is not None else len(fasta)
 
         if start < 0:
             msg = "start ({0}) must > 0 of `{1}`. Reset to 1".format(
                 start + 1, fasta.id
             )
-            logging.error(msg)
+            logger.error(msg)
             start = 0
 
         if stop > len(fasta):
             msg = "stop ({0}) must be <= length of `{1}` ({2}). Reset to {2}.".format(
                 stop, fasta.id, len(fasta)
             )
-            logging.error(msg)
+            logger.error(msg)
             stop = len(fasta)
 
         seq = fasta.seq[start:stop]
 
         if strand in (-1, "-1", "-"):
             seq = seq.reverse_complement()
 
@@ -439,15 +437,15 @@
 def gc(args):
     """
     %prog gc fastafile
 
     Plot G+C content distribution.
     """
     p = OptionParser(gc.__doc__)
-    p.add_option("--binsize", default=500, type="int", help="Bin size to use")
+    p.add_argument("--binsize", default=500, type=int, help="Bin size to use")
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (fastafile,) = args
     binsize = opts.binsize
@@ -481,16 +479,16 @@
 
     Split sequences at lower-cased letters and stretch of Ns. This is useful
     at cleaning up the low quality bases for the QUIVER output.
     """
     from jcvi.utils.cbook import SummaryStats
 
     p = OptionParser(trimsplit.__doc__)
-    p.add_option(
-        "--minlength", default=1000, type="int", help="Min length of contigs to keep"
+    p.add_argument(
+        "--minlength", default=1000, type=int, help="Min length of contigs to keep"
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (fastafile,) = args
@@ -518,34 +516,34 @@
             id = "{0}_{1}".format(name.split("|")[0], i)
             s = SeqRecord(Seq(seq), id=id, description="")
             SeqIO.write([s], fw, "fasta")
     fw.close()
 
     # Reporting
     if removed:
-        logging.debug(
+        logger.debug(
             "Total bases removed: {0}".format(percentage(sum(removed), ntotal))
         )
         print(SummaryStats(removed), file=sys.stderr)
     if Ns:
-        logging.debug("Total Ns removed: {0}".format(percentage(sum(Ns), ntotal)))
+        logger.debug("Total Ns removed: {0}".format(percentage(sum(Ns), ntotal)))
         print(SummaryStats(Ns), file=sys.stderr)
 
 
 def qual(args):
     """
     %prog qual fastafile
 
     Generate dummy .qual file based on FASTA file.
     """
     from jcvi.formats.sizes import Sizes
 
     p = OptionParser(qual.__doc__)
-    p.add_option(
-        "--qv", default=31, type="int", help="Dummy qv score for extended bases"
+    p.add_argument(
+        "--qv", default=31, type=int, help="Dummy qv score for extended bases"
     )
     p.set_outfile()
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
@@ -555,25 +553,25 @@
     fw = must_open(opts.outfile, "w")
     total = 0
     for s, slen in sizes.iter_sizes():
         print(">" + s, file=fw)
         print(" ".join([qvchar] * slen), file=fw)
         total += 1
     fw.close()
-    logging.debug("Written {0} records in `{1}`.".format(total, opts.outfile))
+    logger.debug("Written {0} records in `{1}`.".format(total, opts.outfile))
 
 
 def info(args):
     """
     %prog info *.fasta
 
     Run `sequence_info` on FASTA files. Generate a report per file.
     """
     p = OptionParser(info.__doc__)
-    p.add_option(
+    p.add_argument(
         "--gaps", default=False, action="store_true", help="Count number of gaps"
     )
     p.set_table()
     p.set_outfile()
     opts, args = p.parse_args(args)
 
     if len(args) == 0:
@@ -592,18 +590,18 @@
     %prog fromtab tabfile fastafile
 
     Convert 2-column sequence file to FASTA format. One usage for this is to
     generatea `adapters.fasta` for TRIMMOMATIC.
     """
     p = OptionParser(fromtab.__doc__)
     p.set_sep(sep=None)
-    p.add_option(
+    p.add_argument(
         "--noheader", default=False, action="store_true", help="Ignore first line"
     )
-    p.add_option("--replace", help="Replace spaces in name to char")
+    p.add_argument("--replace", help="Replace spaces in name to char")
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     tabfile, fastafile = args
     sep = opts.sep
@@ -621,25 +619,25 @@
         name, seq = row.rsplit(sep, 1)
         if replace:
             name = name.replace(" ", replace)
         print(">{0}\n{1}".format(name, seq), file=fw)
         nseq += 1
     fw.close()
 
-    logging.debug("A total of {0} sequences written to `{1}`.".format(nseq, fastafile))
+    logger.debug("A total of {0} sequences written to `{1}`.".format(nseq, fastafile))
 
 
 def longestorf(args):
     """
     %prog longestorf fastafile
 
     Find longest ORF for each sequence in fastafile.
     """
     p = OptionParser(longestorf.__doc__)
-    p.add_option("--ids", action="store_true", help="Generate table with ORF info")
+    p.add_argument("--ids", action="store_true", help="Generate table with ORF info")
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (fastafile,) = args
     pf = fastafile.rsplit(".", 1)[0]
@@ -665,15 +663,15 @@
         if idsfile:
             print("\t".join((name, orf.info)), file=fwids)
 
     fw.close()
     if idsfile:
         fwids.close()
 
-    logging.debug(
+    logger.debug(
         "Longest ORFs written to `{0}` ({1}).".format(
             orffile, percentage(after, before)
         )
     )
 
     return orffile
 
@@ -682,19 +680,19 @@
     """
     %prog ispcr fastafile
 
     Reformat paired primers into isPcr query format, which is three column
     format: name, forward, reverse
     """
     p = OptionParser(ispcr.__doc__)
-    p.add_option(
+    p.add_argument(
         "-r",
         dest="rclip",
         default=1,
-        type="int",
+        type=int,
         help="pair ID is derived from rstrip N chars",
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
@@ -712,15 +710,15 @@
         aid, bid = [strip_name(x) for x in (a.id, b.id)]
         assert aid == bid, "Name mismatch {0}".format((aid, bid))
 
         print("\t".join((aid, str(a.seq), str(b.seq))), file=fw)
         npairs += 1
 
     fw.close()
-    logging.debug("A total of {0} pairs written to `{1}`.".format(npairs, ispcrfile))
+    logger.debug("A total of {0} pairs written to `{1}`.".format(npairs, ispcrfile))
 
 
 def parse_fasta(infile, upper=False):
     """
     parse a fasta-formatted file and returns header
     can be a fasta file that contains multiple records.
     """
@@ -754,15 +752,15 @@
     totalbad = 0
     for header, seq in parse_fasta(fastafile):
         badcounts = sum(1 for x in seq if x not in canonical)
         seq = "".join((x if x in canonical else "N") for x in seq)
         totalbad += badcounts
         yield header, seq
 
-    logging.debug("Total bad char: {0}".format(totalbad))
+    logger.debug("Total bad char: {0}".format(totalbad))
 
 
 def fancyprint(fw, seq, width=60, chunk=10):
     assert width % chunk == 0
     nchunks = width / chunk
     seqlen = len(seq)
     maxchar = len(str(seqlen))
@@ -778,18 +776,18 @@
 def clean(args):
     """
     %prog clean fastafile
 
     Remove irregular chars in FASTA seqs.
     """
     p = OptionParser(clean.__doc__)
-    p.add_option(
+    p.add_argument(
         "--fancy", default=False, action="store_true", help="Pretty print the sequence"
     )
-    p.add_option(
+    p.add_argument(
         "--canonical", default=False, action="store_true", help="Use only acgtnACGTN"
     )
     p.set_outfile()
 
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
@@ -820,39 +818,39 @@
     represents a partial gene, therefore disrupting the frame of the protein.
     Check all three frames to get a valid translation.
     """
     from jcvi.utils.cbook import gene_name
 
     transl_tables = [str(x) for x in range(1, 25)]
     p = OptionParser(translate.__doc__)
-    p.add_option(
+    p.add_argument(
         "--ids",
         default=False,
         action="store_true",
         help="Create .ids file with the complete/partial/gaps label",
     )
-    p.add_option(
+    p.add_argument(
         "--longest",
         default=False,
         action="store_true",
         help="Find the longest ORF from each input CDS",
     )
-    p.add_option(
+    p.add_argument(
         "--table",
         default=1,
         choices=transl_tables,
         help="Specify translation table to use",
     )
-    p.add_option(
+    p.add_argument(
         "--strip_names",
         default=False,
         action="store_true",
         help="Strip alternative splicing (e.g. At5g06540.1 -> At5g06540)",
     )
-    p.add_option(
+    p.add_argument(
         "--unique",
         default=False,
         action="store_true",
         help="Ensure the output FASTA contains unique identifiers",
     )
     p.set_outfile()
 
@@ -902,15 +900,15 @@
             newcds = cds[i : i + peplen * 3]
             newpep = newcds.translate(table=opts.table)
             if len(newpep.split("*")[0]) > len(pep.split("*")[0]):
                 pep = newpep
 
         labels = []
         if "*" in pep.rstrip("*"):
-            logging.error("{0} cannot translate".format(name))
+            logger.error("{0} cannot translate".format(name))
             cannot_translate += 1
             labels.append("cannot_translate")
 
         contains_start = pep.startswith("M")
         contains_stop = pep.endswith("*")
         contains_ns = "X" in pep
         start_ns = pep.startswith("X")
@@ -958,15 +956,15 @@
         print(
             "Cannot translate: {0}".format(percentage(cannot_translate, total)),
             file=sys.stderr,
         )
 
     fw.close()
 
-    logging.debug(
+    logger.debug(
         "Total records: {}, Unique records (strip_names={}): {}".format(
             grand_total, strip_names, len(seen)
         )
     )
 
     return cdsfasta, outfile
 
@@ -974,15 +972,15 @@
 def filter(args):
     """
     %prog filter fastafile 100
 
     Filter the FASTA file to contain records with size >= or <= certain cutoff.
     """
     p = OptionParser(filter.__doc__)
-    p.add_option(
+    p.add_argument(
         "--less",
         default=False,
         action="store_true",
         help="filter the sizes < certain cutoff [default: >=]",
     )
     p.set_outfile()
 
@@ -1021,16 +1019,16 @@
     Pool a bunch of FASTA files, and add prefix to each record based on
     filenames. File names are simplified to longest unique prefix to avoid
     collisions after getting shortened.
     """
     from jcvi.formats.base import longest_unique_prefix
 
     p = OptionParser(pool.__doc__)
-    p.add_option("--sep", default=".", help="Separator between prefix and name")
-    p.add_option(
+    p.add_argument("--sep", default=".", help="Separator between prefix and name")
+    p.add_argument(
         "--sequential", default=False, action="store_true", help="Add sequential IDs"
     )
     opts, args = p.parse_args(args)
 
     if len(args) < 1:
         sys.exit(not p.print_help())
 
@@ -1047,18 +1045,18 @@
 def ids(args):
     """
     %prog ids fastafiles
 
     Generate the FASTA headers without the '>'.
     """
     p = OptionParser(ids.__doc__)
-    p.add_option(
+    p.add_argument(
         "--until", default=None, help="Truncate the name and description at words"
     )
-    p.add_option(
+    p.add_argument(
         "--description",
         default=False,
         action="store_true",
         help="Generate a second column with description",
     )
     p.set_outfile()
 
@@ -1088,15 +1086,15 @@
 def sort(args):
     """
     %prog sort fastafile
 
     Sort a list of sequences and output with sorted IDs, etc.
     """
     p = OptionParser(sort.__doc__)
-    p.add_option(
+    p.add_argument(
         "--sizes", default=False, action="store_true", help="Sort by decreasing size"
     )
 
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(p.print_help())
@@ -1105,26 +1103,26 @@
     sortedfastafile = fastafile.rsplit(".", 1)[0] + ".sorted.fasta"
 
     f = Fasta(fastafile, index=False)
     fw = must_open(sortedfastafile, "w")
     if opts.sizes:
         # Sort by decreasing size
         sortlist = sorted(f.itersizes(), key=lambda x: (-x[1], x[0]))
-        logging.debug(
+        logger.debug(
             "Sort by size: max: {0}, min: {1}".format(sortlist[0], sortlist[-1])
         )
         sortlist = [x for x, s in sortlist]
     else:
         sortlist = sorted(f.iterkeys())
 
     for key in sortlist:
         rec = f[key]
         SeqIO.write([rec], fw, "fasta")
 
-    logging.debug("Sorted file written to `{0}`.".format(sortedfastafile))
+    logger.debug("Sorted file written to `{0}`.".format(sortedfastafile))
     fw.close()
 
     return sortedfastafile
 
 
 def join(args):
     """
@@ -1136,26 +1134,28 @@
 
     Phasefile is optional, but must contain two columns - BAC and phase (0, 1, 2, 3).
     """
     from jcvi.formats.agp import OO, Phases, build
     from jcvi.formats.sizes import Sizes
 
     p = OptionParser(join.__doc__)
-    p.add_option("--newid", default=None, help="New sequence ID")
-    p.add_option(
+    p.add_argument("--newid", default=None, help="New sequence ID")
+    p.add_argument(
         "--gapsize",
         default=100,
-        type="int",
+        type=int,
         help="Number of N's in between the sequences",
     )
-    p.add_option("--gaptype", default="contig", help="Gap type to use in the AGP file")
-    p.add_option(
+    p.add_argument(
+        "--gaptype", default="contig", help="Gap type to use in the AGP file"
+    )
+    p.add_argument(
         "--evidence", default="", help="Linkage evidence to report in the AGP file"
     )
-    p.add_option("--oo", help="Use .oo file generated by bambus")
+    p.add_argument("--oo", help="Use .oo file generated by bambus")
     opts, args = p.parse_args(args)
 
     nargs = len(args)
     if nargs not in (1, 2):
         sys.exit(not p.print_help())
 
     if nargs == 2:
@@ -1173,15 +1173,15 @@
     oo = opts.oo
 
     o = OO(oo, sizes.mapping)
 
     if oo:
         seen = o.contigs
         # The leftover contigs not in the oo file
-        logging.debug(
+        logger.debug(
             "A total of {0} contigs ({1} in `{2}`)".format(len(sizes), len(seen), oo)
         )
 
         for ctg, size in sizes.iter_sizes():
             if ctg in seen:
                 continue
             o.add(ctg, ctg, size)
@@ -1216,18 +1216,18 @@
     %prog summary *.fasta
 
     Report real bases and N's in fastafiles in a tabular report
     """
     from natsort import natsort_key
 
     p = OptionParser(summary.__doc__)
-    p.add_option(
+    p.add_argument(
         "--suffix", default="Mb", help="make the base pair counts human readable"
     )
-    p.add_option("--ids", help="write the ids that have >= 50% N's")
+    p.add_argument("--ids", help="write the ids that have >= 50% N's")
     p.set_outfile()
 
     opts, args = p.parse_args(args)
 
     if len(args) == 0:
         sys.exit(not p.print_help())
 
@@ -1257,15 +1257,15 @@
     nns = sum(nns)
     seqlen = sum(seqlen)
     pctreal = "{0:.1f}%".format(reals * 100.0 / seqlen)
     data.append(("Total", reals, nns, seqlen, pctreal))
 
     write_csv(header, data, sep=" ", filename=opts.outfile, thousands=True)
     if idsfile:
-        logging.debug(
+        logger.debug(
             "A total of {0} ids >= 50% N's written to {1}.".format(nids, idsfile.name)
         )
         idsfile.close()
 
     return reals, nns, seqlen
 
 
@@ -1273,79 +1273,79 @@
     """
     %prog format infasta outfasta
 
     Reformat FASTA file and also clean up names.
     """
     sequential_choices = ("replace", "prefix", "suffix")
     p = OptionParser(format.__doc__)
-    p.add_option(
+    p.add_argument(
         "--pairs",
         default=False,
         action="store_true",
         help="Add trailing /1 and /2 for interleaved pairs",
     )
-    p.add_option(
+    p.add_argument(
         "--sequential",
         default=None,
         choices=sequential_choices,
         help="Add sequential IDs",
     )
-    p.add_option(
-        "--sequentialoffset", default=0, type="int", help="Sequential IDs start at"
+    p.add_argument(
+        "--sequentialoffset", default=0, type=int, help="Sequential IDs start at"
     )
-    p.add_option(
-        "--pad0", default=0, type="int", help="Pad a few zeros in front of sequential"
+    p.add_argument(
+        "--pad0", default=0, type=int, help="Pad a few zeros in front of sequential"
     )
-    p.add_option(
+    p.add_argument(
         "--gb",
         default=False,
         action="store_true",
         help="For Genbank ID, get the accession",
     )
-    p.add_option("--sep", default=None, help="Split description by certain symbol")
-    p.add_option(
+    p.add_argument("--sep", default=None, help="Split description by certain symbol")
+    p.add_argument(
         "--index",
         default=0,
-        type="int",
+        type=int,
         help="Extract i-th field after split with --sep",
     )
-    p.add_option(
+    p.add_argument(
         "--noversion",
         default=False,
         action="store_true",
         help="Remove the gb trailing version",
     )
-    p.add_option("--prefix", help="Prepend prefix to sequence ID")
-    p.add_option("--suffix", help="Append suffix to sequence ID")
-    p.add_option(
+    p.add_argument("--prefix", help="Prepend prefix to sequence ID")
+    p.add_argument("--suffix", help="Append suffix to sequence ID")
+    p.add_argument(
         "--template",
         default=False,
         action="store_true",
         help="Extract `template=aaa dir=x library=m` to `m-aaa/x`",
     )
-    p.add_option("--switch", help="Switch ID from two-column file")
-    p.add_option(
+    p.add_argument("--switch", help="Switch ID from two-column file")
+    p.add_argument(
         "--annotation",
         help="Add functional annotation from two-column file ('ID <--> Annotation')",
     )
-    p.add_option("--ids", help="Generate ID conversion table")
-    p.add_option(
+    p.add_argument("--ids", help="Generate ID conversion table")
+    p.add_argument(
         "--upper",
         default=False,
         action="store_true",
         help="Convert sequence to upper case",
     )
-    p.add_option(
+    p.add_argument(
         "--nodesc",
         default=False,
         action="store_true",
         help="Remove description after identifier",
     )
-    p.add_option(
-        "--minlength", default=0, type="int", help="Minimum sequence length to keep"
+    p.add_argument(
+        "--minlength", default=0, type=int, help="Minimum sequence length to keep"
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     infasta, outfasta = args
@@ -1406,15 +1406,15 @@
                 x.split("=")[-1] for x in rec.description.split()[1:4]
             ]
             rec.id = "{0}-{1}/{2}".format(lib, template, dir)
         if mapfile:
             if origid in mapping:
                 rec.id = mapping[origid]
             else:
-                logging.error(
+                logger.error(
                     "{0} not found in `{1}`. ID unchanged.".format(origid, mapfile)
                 )
         if prefix:
             rec.id = prefix + rec.id
         if suffix:
             rec.id += suffix
         if annotfile:
@@ -1429,19 +1429,19 @@
             print("\t".join((origid, rec.id)), file=idsfile)
         if upper:
             rec.seq = rec.seq.upper()
 
         SeqIO.write(rec, fw, "fasta")
 
     if idsfile:
-        logging.debug("Conversion table written to `{0}`.".format(idsfile.name))
+        logger.debug("Conversion table written to `{0}`.".format(idsfile.name))
         idsfile.close()
 
     if nremoved:
-        logging.debug(
+        logger.debug(
             "Removed {} sequences with length < {}".format(nremoved, minlength)
         )
 
 
 def print_first_difference(
     arec, brec, ignore_case=False, ignore_N=False, rc=False, report_match=True
 ):
@@ -1453,15 +1453,15 @@
         arec,
         brec,
         ignore_case=ignore_case,
         ignore_N=ignore_N,
         report_match=report_match,
     )
     if rc and not plus_match:
-        logging.debug("trying reverse complement of %s" % brec.id)
+        logger.debug("trying reverse complement of %s" % brec.id)
         brec.seq = brec.seq.reverse_complement()
         minus_match = _print_first_difference(
             arec,
             brec,
             ignore_case=ignore_case,
             ignore_N=ignore_N,
             report_match=report_match,
@@ -1520,39 +1520,39 @@
     %prog diff afasta bfasta
 
     print out whether the records in two fasta files are the same
     """
     from jcvi.utils.table import banner
 
     p = OptionParser(diff.__doc__)
-    p.add_option(
+    p.add_argument(
         "--ignore_case",
         default=False,
         action="store_true",
         help="ignore case when comparing sequences",
     )
-    p.add_option(
+    p.add_argument(
         "--ignore_N",
         default=False,
         action="store_true",
         help="ignore N and X's when comparing sequences",
     )
-    p.add_option(
+    p.add_argument(
         "--ignore_stop",
         default=False,
         action="store_true",
         help="ignore stop codon when comparing sequences",
     )
-    p.add_option(
+    p.add_argument(
         "--rc",
         default=False,
         action="store_true",
         help="also consider reverse complement",
     )
-    p.add_option(
+    p.add_argument(
         "--quiet",
         default=False,
         action="store_true",
         help="don't output comparison details",
     )
 
     opts, args = p.parse_args(args)
@@ -1605,15 +1605,15 @@
             brec,
             ignore_case=opts.ignore_case,
             ignore_N=opts.ignore_N,
             rc=opts.rc,
             report_match=not opts.quiet,
         )
         if not fd:
-            logging.error("Two sets of sequences differ at `{0}`".format(arec.id))
+            logger.error("Two sets of sequences differ at `{0}`".format(arec.id))
             problem_ids.append(
                 "\t".join(str(x) for x in (arec.id, asize, bsize, abs(asize - bsize)))
             )
 
     if problem_ids:
         print("A total of {0} records mismatch.".format(len(problem_ids)))
         fw = must_open("Problems.ids", "w")
@@ -1663,39 +1663,39 @@
         t7         3367          na
     """
     from jcvi.utils.cbook import AutoVivification
 
     allowed_checksum = ["MD5", "GCG"]
 
     p = OptionParser(identical.__doc__)
-    p.add_option(
+    p.add_argument(
         "--ignore_case",
         default=False,
         action="store_true",
         help="ignore case when comparing sequences",
     )
-    p.add_option(
+    p.add_argument(
         "--ignore_N",
         default=False,
         action="store_true",
         help="ignore N and X's when comparing sequences",
     )
-    p.add_option(
+    p.add_argument(
         "--ignore_stop",
         default=False,
         action="store_true",
         help="ignore stop codon when comparing sequences",
     )
-    p.add_option(
+    p.add_argument(
         "--output_uniq",
         default=False,
         action="store_true",
         help="output uniq sequences in FASTA format",
     )
-    p.add_option(
+    p.add_argument(
         "--checksum",
         default="MD5",
         choices=allowed_checksum,
         help="specify checksum method",
     )
     p.set_outfile()
 
@@ -1707,15 +1707,15 @@
     d = AutoVivification()
     files = []
     for fastafile in args:
         f = Fasta(fastafile)
         pf = fastafile.rsplit(".", 1)[0]
         files.append(pf)
 
-        logging.debug("Hashing individual elements of {0}".format(fastafile))
+        logger.debug("Hashing individual elements of {0}".format(fastafile))
         for name, rec in f.iteritems_ordered():
             seq = re.sub(" ", "", str(rec.seq))
             hashed = hash_fasta(
                 seq,
                 ignore_case=opts.ignore_case,
                 ignore_N=opts.ignore_N,
                 ignore_stop=opts.ignore_stop,
@@ -1750,15 +1750,15 @@
         if opts.output_uniq:
             seqid = "\t".join(str(x) for x in ("t{0}".format(idx), d[hashed]["count"]))
             rec = SeqRecord(Seq(d[hashed]["seq"]), id=seqid, description="")
             SeqIO.write([rec], uniqfw, "fasta")
 
     fw.close()
     if opts.output_uniq:
-        logging.debug("Uniq sequences written to `{0}`".format(uniqfile))
+        logger.debug("Uniq sequences written to `{0}`".format(uniqfile))
         uniqfw.close()
 
 
 QUALSUFFIX = ".qual"
 
 
 def get_qual(fastafile, suffix=QUALSUFFIX, check=True):
@@ -1766,18 +1766,18 @@
     Check if current folder contains a qual file associated with the fastafile
     """
     qualfile1 = fastafile.rsplit(".", 1)[0] + suffix
     qualfile2 = fastafile + suffix
 
     if check:
         if op.exists(qualfile1):
-            logging.debug("qual file `{0}` found".format(qualfile1))
+            logger.debug("qual file `{0}` found".format(qualfile1))
             return qualfile1
         elif op.exists(qualfile2):
-            logging.debug("qual file `{0}` found".format(qualfile2))
+            logger.debug("qual file `{0}` found".format(qualfile2))
             return qualfile2
         else:
             return None
 
     return qualfile1
 
 
@@ -1786,27 +1786,27 @@
     %prog some fastafile listfile outfastafile
 
     generate a subset of fastafile, based on a list
     """
     from jcvi.utils.cbook import gene_name
 
     p = OptionParser(some.__doc__)
-    p.add_option(
+    p.add_argument(
         "--exclude",
         default=False,
         action="store_true",
         help="Output sequences not in the list file",
     )
-    p.add_option(
+    p.add_argument(
         "--no_strip_names",
         default=False,
         action="store_true",
         help="Do not strip alternative splicing (e.g. At5g06540.1 -> At5g06540)",
     )
-    p.add_option(
+    p.add_argument(
         "--uniprot", default=False, action="store_true", help="Header is from uniprot"
     )
 
     opts, args = p.parse_args(args)
 
     if len(args) != 3:
         sys.exit(p.print_help())
@@ -1848,42 +1848,42 @@
         seen.add(name)
 
     for rec in recs:
         SeqIO.write([rec], outfastahandle, "fasta")
         if qualfile:
             SeqIO.write([rec], outqualhandle, "qual")
 
-    logging.debug("A total of %d records written to `%s`" % (len(recs), outfastafile))
+    logger.debug("A total of %d records written to `%s`" % (len(recs), outfastafile))
 
 
 def fastq(args):
     """
     %prog fastq fastafile
 
     Generate fastqfile by combining fastafile and fastafile.qual.
     Also check --qv option to use a default qv score.
     """
     from jcvi.formats.fastq import FastqLite
 
     p = OptionParser(fastq.__doc__)
-    p.add_option("--qv", type="int", help="Use generic qv value")
+    p.add_argument("--qv", type=int, help="Use generic qv value")
 
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (fastafile,) = args
     fastqfile = fastafile.rsplit(".", 1)[0] + ".fastq"
     fastqhandle = open(fastqfile, "w")
     num_records = 0
 
     if opts.qv is not None:
         qv = chr(ord("!") + opts.qv)
-        logging.debug("QV char '{0}' ({1})".format(qv, opts.qv))
+        logger.debug("QV char '{0}' ({1})".format(qv, opts.qv))
     else:
         qv = None
 
     if qv:
         f = Fasta(fastafile, lazy=True)
         for name, rec in f.iteritems_ordered():
             r = FastqLite("@" + name, str(rec.seq).upper(), qv * len(rec.seq))
@@ -1893,15 +1893,15 @@
     else:
         qualfile = get_qual(fastafile)
         for rec in iter_fasta_qual(fastafile, qualfile):
             SeqIO.write([rec], fastqhandle, "fastq")
             num_records += 1
 
     fastqhandle.close()
-    logging.debug("A total of %d records written to `%s`" % (num_records, fastqfile))
+    logger.debug("A total of %d records written to `%s`" % (num_records, fastqfile))
 
 
 def pair(args):
     """
     %prog pair fastafile
 
     Generate .pairs.fasta and .fragments.fasta by matching records
@@ -1909,15 +1909,15 @@
     """
     p = OptionParser(pair.__doc__)
     p.set_sep(
         sep=None,
         help="Separator in name to reduce to clone id"
         + "e.g. GFNQ33242/1 use /, BOT01-2453H.b1 use .",
     )
-    p.add_option(
+    p.add_argument(
         "-m",
         dest="matepairs",
         default=False,
         action="store_true",
         help="generate .matepairs file [often used for Celera Assembler]",
     )
     opts, args = p.parse_args(args)
@@ -1979,33 +1979,33 @@
             rec.description = ""
             SeqIO.write([rec], fw, "fasta")
             if qualfile:
                 recqual.id = newid
                 recqual.description = ""
                 SeqIO.write([recqual], qualfw, "qual")
 
-    logging.debug("sequences written to `%s` and `%s`" % (pairsfile, fragsfile))
+    logger.debug("sequences written to `%s` and `%s`" % (pairsfile, fragsfile))
     if opts.matepairs:
-        logging.debug("mates written to `%s`" % matepairsfile)
+        logger.debug("mates written to `%s`" % matepairsfile)
 
 
 def pairinplace(args):
     """
     %prog pairinplace bulk.fasta
 
     Pair up the records in bulk.fasta by comparing the names for adjacent
     records. If they match, print to bulk.pairs.fasta, else print to
     bulk.frags.fasta.
     """
     p = OptionParser(pairinplace.__doc__)
-    p.add_option(
+    p.add_argument(
         "-r",
         dest="rclip",
         default=1,
-        type="int",
+        type=int,
         help="pair ID is derived from rstrip N chars",
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
@@ -2040,42 +2040,42 @@
         else:
             SeqIO.write([a], fragsfw, "fasta")
 
     # don't forget the last one, when b is None
     if not skipflag:
         SeqIO.write([a], fragsfw, "fasta")
 
-    logging.debug("Reads paired into `%s` and `%s`" % (pairs, frags))
+    logger.debug("Reads paired into `%s` and `%s`" % (pairs, frags))
 
 
 def extract(args):
     """
     %prog extract fasta query
 
     extract query out of fasta file, query needs to be in the form of
     "seqname", or "seqname:start-stop", or "seqname:start-stop:-"
     """
     p = OptionParser(extract.__doc__)
-    p.add_option("--newname", help="Use this new name instead")
-    p.add_option(
+    p.add_argument("--newname", help="Use this new name instead")
+    p.add_argument(
         "--include",
         default=False,
         action="store_true",
         help="search description line for match",
     )
-    p.add_option(
+    p.add_argument(
         "--exclude",
         default=False,
         action="store_true",
         help="exclude description that matches",
     )
-    p.add_option(
+    p.add_argument(
         "--idonly", default=False, action="store_true", help="Only search identifier"
     )
-    p.add_option(
+    p.add_argument(
         "--bed",
         default=None,
         help="path to bed file to guide extraction by matching seqname",
     )
     p.set_outfile()
 
     opts, args = p.parse_args(args)
@@ -2091,15 +2091,15 @@
     if opts.bed:
         fw = must_open(opts.outfile, "w")
         f = Fasta(fastafile)
         for accn in bedaccns:
             try:
                 rec = f[accn]
             except:
-                logging.error("{0} not found in {1}".format(accn, fastafile))
+                logger.error("{0} not found in {1}".format(accn, fastafile))
                 continue
             SeqIO.write([rec], fw, "fasta")
         return fw.name
 
     atoms = query.split(":")
     key = atoms[0]
 
@@ -2118,15 +2118,15 @@
     feature = dict(chr=key)
 
     if "-" in pos:
         start, stop = pos.split("-")
         try:
             start, stop = int(start), int(stop)
         except ValueError as e:
-            logging.error(e)
+            logger.error(e)
             sys.exit(p.print_help())
 
         feature["start"] = start
         feature["stop"] = stop
     else:
         start, stop = None, None
 
@@ -2164,15 +2164,15 @@
             rec = SeqRecord(seq, id=newid, description=k)
             SeqIO.write([rec], fw, "fasta")
     else:
         f = Fasta(fastafile)
         try:
             seq = f.sequence(feature, asstring=False)
         except AssertionError as e:
-            logging.error(e)
+            logger.error(e)
             return
 
         newid = opts.newname or query
         rec = SeqRecord(seq, id=newid, description="")
         SeqIO.write([rec], fw, "fasta")
 
     return fw.name
@@ -2182,31 +2182,31 @@
     """
     Returns unique records
     """
     seen = set()
     for rec in SeqIO.parse(fastafile, "fasta"):
         name = str(rec.seq) if seq else rec.id
         if name in seen:
-            logging.debug("ignore {0}".format(rec.id))
+            logger.debug("ignore {0}".format(rec.id))
             continue
         seen.add(name)
         yield rec
 
 
 def uniq(args):
     """
     %prog uniq fasta uniq.fasta
 
     remove fasta records that are the same
     """
     p = OptionParser(uniq.__doc__)
-    p.add_option(
+    p.add_argument(
         "--seq", default=False, action="store_true", help="Uniqify the sequences"
     )
-    p.add_option(
+    p.add_argument(
         "-t",
         "--trimname",
         dest="trimname",
         action="store_true",
         default=False,
         help="turn on the defline trim to first space",
     )
@@ -2266,15 +2266,15 @@
             qv[i] = XQUAL
         if s == "N" or s == "x":
             qv[i] = NQUAL
     return rec
 
 
 def make_qual(fastafile, score=OKQUAL):
-    logging.warning("assume qual ({0})".format(score))
+    logger.warning("assume qual ({0})".format(score))
     qualfile = fastafile.rsplit(".", 1)[0] + ".qual"
     fw = open(qualfile, "w")
     fasta = Fasta(fastafile, lazy=True)
     score = str(score) + " "
     for entry, size in fasta.itersizes_ordered():
         print(">" + entry, file=fw)
         print(score * size, file=fw)
@@ -2312,32 +2312,32 @@
     trim if fasta.screen.qual is found. The trimming algorithm is based on
     finding the subarray that maximize the sum
     """
 
     from jcvi.algorithms.maxsum import max_sum
 
     p = OptionParser(trim.__doc__)
-    p.add_option(
+    p.add_argument(
         "-c",
         dest="min_length",
-        type="int",
+        type=int,
         default=64,
         help="minimum sequence length after trimming",
     )
-    p.add_option("-s", dest="score", default=QUAL, help="quality trimming cutoff")
+    p.add_argument("-s", dest="score", default=QUAL, help="quality trimming cutoff")
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(p.print_help())
 
     fastafile, newfastafile = args
     qualfile = get_qual(fastafile)
     newqualfile = get_qual(newfastafile, check=False)
 
-    logging.debug(
+    logger.debug(
         "Trim bad sequence from fasta file `%s` to `%s`" % (fastafile, newfastafile)
     )
 
     fw = must_open(newfastafile, "w")
     fw_qual = open(newqualfile, "w")
 
     dropped = trimmed = 0
@@ -2392,20 +2392,20 @@
     GGTATAATAACAGTATTATTAGGGGCTACTTTAGCTCTTGC
     TCAAAAAGATATTAAGAGGGGTTTAGCCTATTCTACAATGTCCCAACTGGGTTATATGATGTTAGCTCTA
     >?unk100
     TCAATAAAACTATGGGGTAAAGAAGAACAAAAAATAATTAACAGAAATTTTCGTTTATCTCCTTTATTAA
     TATTAACGATGAATAATAATGAGAAGCCATATAGAATTGGTGATAATGTAAAAAAAGGGGCTCTTATTAC
     """
     p = OptionParser(sequin.__doc__)
-    p.add_option("--unk", default=100, type="int", help="The size for unknown gaps")
-    p.add_option("--newid", default=None, help="Use this identifier instead")
-    p.add_option(
+    p.add_argument("--unk", default=100, type=int, help="The size for unknown gaps")
+    p.add_argument("--newid", default=None, help="Use this identifier instead")
+    p.add_argument(
         "--chromosome", default=None, help="Add [chromosome= ] to FASTA header"
     )
-    p.add_option("--clone", default=None, help="Add [clone= ] to FASTA header")
+    p.add_argument("--clone", default=None, help="Add [clone= ] to FASTA header")
     p.set_mingap(default=100)
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (inputfasta,) = args
@@ -2434,15 +2434,15 @@
         fastaheader += " [chromosome={0}]".format(opts.chromosome)
     if opts.clone:
         fastaheader += " [clone={0}]".format(opts.clone)
 
     print(fastaheader, file=fw)
     print(seq, file=fw)
     fw.close()
-    logging.debug(
+    logger.debug(
         "Sequin FASTA written to `{0}` (gaps: {1} unknowns, {2} knowns).".format(
             outputfasta, unknowns, knowns
         )
     )
 
     return outputfasta, unknowns + knowns
 
@@ -2451,15 +2451,15 @@
     newseq = []
     removed = 0
     for gap, seq in groupby(rec.seq, lambda x: x.upper() == "N"):
         seq = "".join(seq)
         seqlen = len(seq)
         if not gap and seqlen < minlen:
             seq = seqlen * "N"  # Mask small components
-            logging.debug("Discard component ({0}) in {1}".format(seqlen, rec.name))
+            logger.debug("Discard component ({0}) in {1}".format(seqlen, rec.name))
             removed += seqlen
         newseq.append(seq)
     rec.seq = Seq("".join(newseq))
     return removed
 
 
 def trim_terminal_Ns(rec):
@@ -2483,26 +2483,26 @@
 def tidy(args):
     """
     %prog tidy fastafile
 
     Trim terminal Ns, normalize gap sizes and remove small components.
     """
     p = OptionParser(tidy.__doc__)
-    p.add_option(
+    p.add_argument(
         "--gapsize",
         dest="gapsize",
         default=0,
-        type="int",
+        type=int,
         help="Set all gaps to the same size",
     )
-    p.add_option(
+    p.add_argument(
         "--minlen",
         dest="minlen",
         default=100,
-        type="int",
+        type=int,
         help="Minimum component size",
     )
 
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
@@ -2521,25 +2521,25 @@
         if minlen:
             removed += remove_small_components(rec, minlen)
         trim_terminal_Ns(rec)
         if gapsize:
             normalized += normalize_gaps(rec, gapsize)
 
         if len(rec) == 0:
-            logging.debug("Drop seq {0}".format(rec.id))
+            logger.debug("Drop seq {0}".format(rec.id))
             continue
         SeqIO.write([rec], fw, "fasta")
 
     # Print statistics
     if removed:
-        logging.debug("Total discarded bases: {0}".format(removed))
+        logger.debug("Total discarded bases: {0}".format(removed))
     if normalized:
-        logging.debug("Gaps normalized: {0}".format(normalized))
+        logger.debug("Gaps normalized: {0}".format(normalized))
 
-    logging.debug("Tidy FASTA written to `{0}`.".format(tidyfastafile))
+    logger.debug("Tidy FASTA written to `{0}`.".format(tidyfastafile))
     fw.close()
 
     return tidyfastafile
 
 
 def write_gaps_worker(rec):
     start = 0
@@ -2579,28 +2579,28 @@
         if b.span < mingap:
             continue
         gapnum += 1
         gapname = "gap.{0:05d}".format(gapnum)
         print("\t".join(str(x) for x in (b, gapname, b.span)), file=fw)
 
     shutil.move(nbedfile, bedfile)
-    logging.debug("Write gap (>={0}bp) locations to `{1}`.".format(mingap, bedfile))
+    logger.debug("Write gap (>={0}bp) locations to `{1}`.".format(mingap, bedfile))
 
 
 def gaps(args):
     """
     %prog gaps fastafile
 
     Print out a list of gaps in BED format (.gaps.bed).
     """
     from jcvi.formats.sizes import agp
     from jcvi.formats.agp import mask, build
 
     p = OptionParser(gaps.__doc__)
-    p.add_option(
+    p.add_argument(
         "--split", default=False, action="store_true", help="Generate .split.fasta"
     )
     p.set_mingap(default=100)
     p.set_cpus()
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
@@ -2622,19 +2622,19 @@
 
         if need_update((inputfasta, bedfile), splitfile):
 
             sizesagpfile = agp([inputfasta])
 
             maskedagpfile = mask([sizesagpfile, bedfile, "--splitobject"])
             shutil.move(maskedagpfile, oagpfile)
-            logging.debug("AGP file written to `{0}`.".format(oagpfile))
+            logger.debug("AGP file written to `{0}`.".format(oagpfile))
 
             maskedagpfile = mask([sizesagpfile, bedfile, "--splitcomponent"])
             shutil.move(maskedagpfile, cagpfile)
-            logging.debug("AGP file written to `{0}`.".format(cagpfile))
+            logger.debug("AGP file written to `{0}`.".format(cagpfile))
 
             build([oagpfile, inputfasta, splitfile])
             cleanup(sizesagpfile)
 
         return splitfile, oagpfile, cagpfile
```

### Comparing `jcvi-1.4.6/jcvi/formats/fastq.py` & `jcvi-1.4.7/jcvi/formats/fastq.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,26 +3,34 @@
 
 """
 Processing fastq files
 """
 import os.path as op
 import sys
 import re
-import logging
 import json
 
 from itertools import islice
 
 from Bio import SeqIO
 from Bio.SeqIO.QualityIO import FastqGeneralIterator
 
-from jcvi.formats.fasta import must_open, rc
-from jcvi.formats.base import DictFile
-from jcvi.utils.cbook import percentage
-from jcvi.apps.base import OptionParser, ActionDispatcher, sh, which, mkdir, need_update
+from ..apps.base import (
+    ActionDispatcher,
+    OptionParser,
+    logger,
+    mkdir,
+    need_update,
+    sh,
+    which,
+)
+from ..utils.cbook import percentage
+
+from .base import DictFile
+from .fasta import must_open, rc
 
 
 qual_offset = lambda x: 33 if x == "sanger" else 64
 allowed_dialect_conversions = {
     ">=1.8": "<1.8",
     "sra": "<1.8",
 }
@@ -184,22 +192,22 @@
             )
 
             return "@{0}".format(h0)
 
     def format_header(self, dialect=None, tag=None):
         if dialect:
             if self.dialect == dialect:
-                logging.error("Input and output dialect are the same")
+                logger.error("Input and output dialect are the same")
             elif dialect not in allowed_dialect_conversions[self.dialect]:
-                logging.error(
+                logger.error(
                     "Error: Cannot convert from `{0}` to `{1}` dialect".format(
                         self.dialect, dialect
                     )
                 )
-                logging.error(
+                logger.error(
                     "Allowed conversions: {0}".format(
                         json.dumps(allowed_dialect_conversions, indent=4)
                     )
                 )
                 sys.exit()
             else:
                 self.dialect = dialect
@@ -221,15 +229,15 @@
     if not pf.strip():
         pf = op.basename(pp[0])
     return pf
 
 
 def iter_fastq(filename, offset=0, key=None):
     if isinstance(filename, str):
-        logging.debug("Read file `{0}`".format(filename))
+        logger.debug("Read file `{0}`".format(filename))
         fh = must_open(filename)
     else:
         fh = filename
 
     while True:
         rec = FastqRecord(fh, offset=offset, key=key)
         if not rec.name:
@@ -291,15 +299,15 @@
             break
         name = rec.name
         if name in seen:
             nduplicates += 1
             continue
         seen.add(name)
         print(rec, file=fw)
-    logging.debug("Removed duplicate reads: {}".format(percentage(nduplicates, nreads)))
+    logger.debug("Removed duplicate reads: {}".format(percentage(nduplicates, nreads)))
 
 
 def suffix(args):
     """
     %prog suffix fastqfile CAG
 
     Filter reads based on suffix.
@@ -317,15 +325,15 @@
     for rec in iter_fastq(fastqfile):
         nreads += 1
         if rec is None:
             break
         if rec.seq.endswith(sf):
             print(rec, file=fw)
             nselected += 1
-    logging.debug(
+    logger.debug(
         "Selected reads with suffix {0}: {1}".format(sf, percentage(nselected, nreads))
     )
 
 
 def calc_readlen(f, first):
     from jcvi.utils.cbook import SummaryStats
 
@@ -352,34 +360,34 @@
     %prog readlen fastqfile
 
     Calculate read length, will only try the first N reads. Output min, max, and
     avg for each file.
     """
     p = OptionParser(readlen.__doc__)
     p.set_firstN()
-    p.add_option(
+    p.add_argument(
         "--silent",
         default=False,
         action="store_true",
         help="Do not print read length stats",
     )
-    p.add_option(
+    p.add_argument(
         "--nocheck",
         default=False,
         action="store_true",
         help="Do not check file type suffix",
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (f,) = args
     if (not opts.nocheck) and (not is_fastq(f)):
-        logging.debug("File `{}` does not endswith .fastq or .fq".format(f))
+        logger.debug("File `{}` does not endswith .fastq or .fq".format(f))
         return 0
 
     s = calc_readlen(f, opts.firstN)
     if not opts.silent:
         print("\t".join(str(x) for x in (f, s.min, s.max, s.mean, s.median)))
 
     return int(s.max)
@@ -388,15 +396,15 @@
 def fasta(args):
     """
     %prog fasta fastqfiles
 
     Convert fastq to fasta and qual file.
     """
     p = OptionParser(fasta.__doc__)
-    p.add_option(
+    p.add_argument(
         "--seqtk", default=False, action="store_true", help="Use seqtk to convert"
     )
     p.set_outdir()
     p.set_outfile(outfile=None)
     opts, args = p.parse_args(args)
 
     if len(args) < 1:
@@ -411,28 +419,28 @@
     pf = op.basename(fastqfile)
     gzinput = pf.endswith(".gz")
     if gzinput:
         pf = pf.rsplit(".", 1)[0]
 
     pf, sf = pf.rsplit(".", 1)
     if sf not in ("fq", "fastq"):
-        logging.debug("Assumed FASTA: suffix not `fq` or `fastq`")
+        logger.debug("Assumed FASTA: suffix not `fq` or `fastq`")
         return fastqfile, None
 
     fastafile, qualfile = pf + ".fasta", pf + ".qual"
     outfile = opts.outfile or fastafile
     outfile = op.join(outdir, outfile)
     if opts.seqtk:
         if need_update(fastqfiles, outfile):
             for i, fastqfile in enumerate(fastqfiles):
                 cmd = "seqtk seq -A {0} -L 30 -l 70".format(fastqfile)
                 # First one creates file, following ones append to it
                 sh(cmd, outfile=outfile, append=i)
         else:
-            logging.debug("Outfile `{0}` already exists.".format(outfile))
+            logger.debug("Outfile `{0}` already exists.".format(outfile))
         return outfile, None
 
     for fastqfile in fastqfiles:
         SeqIO.convert(fastqfile, "fastq", fastafile, "fasta")
         SeqIO.convert(fastqfile, "fastq", qualfile, "qual")
 
     return fastafile, qualfile
@@ -455,15 +463,15 @@
 
     N = int(args[0])
     nlines = N * 4
     fastqfiles = args[1:]
     fastqfile = fastqfiles[0]
     outfile = opts.outfile
     if not need_update(fastqfiles, outfile):
-        logging.debug("File `{0}` exists. Will not overwrite.".format(outfile))
+        logger.debug("File `{0}` exists. Will not overwrite.".format(outfile))
         return
 
     gz = fastqfile.endswith(".gz")
     for fastqfile in fastqfiles:
         if gz:
             cmd = "zcat {0} | head -n {1}".format(fastqfile, nlines)
         else:
@@ -492,26 +500,26 @@
     """
     %prog filter paired.fastq
 
     Filter to get high qv reads. Use interleaved format (one file) or paired
     format (two files) to filter on paired reads.
     """
     p = OptionParser(filter.__doc__)
-    p.add_option(
+    p.add_argument(
         "-q",
         dest="qv",
         default=20,
-        type="int",
+        type=int,
         help="Minimum quality score to keep",
     )
-    p.add_option(
+    p.add_argument(
         "-p",
         dest="pct",
         default=95,
-        type="int",
+        type=int,
         help="Minimum percent of bases that have [-q] quality",
     )
 
     opts, args = p.parse_args(args)
 
     if len(args) not in (1, 2):
         sys.exit(not p.print_help())
@@ -522,15 +530,15 @@
         r1, r2 = args
 
     qv = opts.qv
     pct = opts.pct
 
     offset = guessoffset([r1])
     qvchar = chr(offset + qv)
-    logging.debug("Call base qv >= {0} as good.".format(qvchar))
+    logger.debug("Call base qv >= {0} as good.".format(qvchar))
     outfile = r1.rsplit(".", 1)[0] + ".q{0}.paired.fastq".format(qv)
     fw = open(outfile, "w")
 
     p1fp, p2fp = FastqPairedIterator(r1, r2)
     while True:
         a = list(islice(p1fp, 4))
         if not a:
@@ -594,15 +602,15 @@
         pairsfw.writelines(b)
         nreads += 2
 
     pairsfw.close()
     extra = nreads * 2 if tag else 0
     checkShuffleSizes(p1, p2, pairsfastq, extra=extra)
 
-    logging.debug(
+    logger.debug(
         "File `{0}` verified after writing {1} reads.".format(pairsfastq, nreads)
     )
     return pairsfastq
 
 
 def split(args):
     """
@@ -705,15 +713,15 @@
     %prog format fastqfile
 
     Format FASTQ file. Currently provides option to convert FASTQ header from
     one dialect to another.
     """
     p = OptionParser(format.__doc__)
 
-    p.add_option(
+    p.add_argument(
         "--convert",
         default=None,
         choices=[">=1.8", "<1.8", "sra"],
         help="Convert fastq header to a different format",
     )
     p.set_tag(specify_tag=True)
     opts, args = p.parse_args(args)
@@ -725,17 +733,17 @@
     ai = iter_fastq(fastqfile)
     rec = next(ai)
     dialect = None
     while rec:
         h = FastqHeader(rec.header)
         if not dialect:
             dialect = h.dialect
-            logging.debug("Input fastq dialect: `{0}`".format(dialect))
+            logger.debug("Input fastq dialect: `{0}`".format(dialect))
             if opts.convert:
-                logging.debug("Output fastq dialect: `{0}`".format(opts.convert))
+                logger.debug("Output fastq dialect: `{0}`".format(opts.convert))
 
         rec.name = h.format_header(dialect=opts.convert, tag=opts.tag)
 
         print(rec)
         rec = next(ai)
 
 
@@ -780,26 +788,26 @@
 def trim(args):
     """
     %prog trim fastqfile
 
     Wraps `fastx_trimmer` to trim from begin or end of reads.
     """
     p = OptionParser(trim.__doc__)
-    p.add_option(
+    p.add_argument(
         "-f",
         dest="first",
         default=0,
-        type="int",
+        type=int,
         help="First base to keep. Default is 1.",
     )
-    p.add_option(
+    p.add_argument(
         "-l",
         dest="last",
         default=0,
-        type="int",
+        type=int,
         help="Last base to keep. Default is entire read.",
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
@@ -857,22 +865,22 @@
 def splitread(args):
     """
     %prog splitread fastqfile
 
     Split fastqfile into two read fastqfiles, cut in the middle.
     """
     p = OptionParser(splitread.__doc__)
-    p.add_option(
+    p.add_argument(
         "-n",
         dest="n",
         default=76,
-        type="int",
+        type=int,
         help="Split at N-th base position",
     )
-    p.add_option(
+    p.add_argument(
         "--rc",
         default=False,
         action="store_true",
         help="Reverse complement second read",
     )
     opts, args = p.parse_args(args)
 
@@ -889,27 +897,27 @@
 
     fp = must_open(pairsfastq)
     n = opts.n
     minsize = n * 8 / 5
 
     for name, seq, qual in FastqGeneralIterator(fp):
         if len(seq) < minsize:
-            logging.error("Skipping read {0}, length={1}".format(name, len(seq)))
+            logger.error("Skipping read {0}, length={1}".format(name, len(seq)))
             continue
 
         name = "@" + name
         rec1 = FastqLite(name, seq[:n], qual[:n])
         rec2 = FastqLite(name, seq[n:], qual[n:])
         if opts.rc:
             rec2.rc()
 
         print(rec1, file=fw1)
         print(rec2, file=fw2)
 
-    logging.debug("Reads split into `{0},{1}`".format(fq1, fq2))
+    logger.debug("Reads split into `{0},{1}`".format(fq1, fq2))
     fw1.close()
     fw2.close()
 
 
 def size(args):
     """
     %prog size fastqfile
@@ -989,15 +997,15 @@
     bulk.frags.fastq.
     """
     from more_itertools import pairwise
 
     p = OptionParser(pairinplace.__doc__)
     p.set_rclip()
     p.set_tag()
-    p.add_option("--base", help="Base name for the output files")
+    p.add_argument("--base", help="Base name for the output files")
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (fastqfile,) = args
     base = opts.base or op.basename(fastqfile).split(".")[0]
@@ -1035,32 +1043,32 @@
         else:
             print(a, file=fragsfw)
 
     # don't forget the last one, when b is None
     if not skipflag:
         print(a, file=fragsfw)
 
-    logging.debug("Reads paired into `%s` and `%s`" % (pairs, frags))
+    logger.debug("Reads paired into `%s` and `%s`" % (pairs, frags))
     return pairs
 
 
 def fromsra(args):
     """
     %prog fromsra srafile
 
     Convert sra file to fastq using the sratoolkit `fastq-dump`
     """
     p = OptionParser(fromsra.__doc__)
-    p.add_option(
+    p.add_argument(
         "--paired",
         default=False,
         action="store_true",
         help="Specify if library layout is paired-end",
     )
-    p.add_option(
+    p.add_argument(
         "--compress",
         default=None,
         choices=["gzip", "bzip2"],
         help="Compress output fastq files",
     )
     p.set_outdir()
     p.set_grid()
@@ -1072,15 +1080,15 @@
     (srafile,) = args
     paired = opts.paired
     compress = opts.compress
     outdir = opts.outdir
 
     script_path = which("fastq-dump")
     if not script_path:
-        logging.error("Cannot find `fastq-dump` in the PATH")
+        logger.error("Cannot find `fastq-dump` in the PATH")
         sys.exit()
 
     cmd = [script_path]
     if compress:
         cmd.append("--{0}".format(compress))
     if paired:
         cmd.append("--split-files")
```

### Comparing `jcvi-1.4.6/jcvi/formats/genbank.py` & `jcvi-1.4.7/jcvi/formats/genbank.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 
 """
 Genbank record operations based on biopython Bio.SeqIO
 https://github.com/biopython/biopython/blob/master/Bio/SeqIO/InsdcIO.py
 """
 import os.path as op
 import sys
-import logging
 
 from collections import defaultdict
 
 from Bio import SeqIO
 
-from jcvi.formats.base import BaseFile, get_number, must_open
-from jcvi.formats.gff import GffLine
-from jcvi.apps.fetch import entrez
-from jcvi.apps.base import ActionDispatcher, OptionParser, cleanup, glob, mkdir, sh
+from ..apps.fetch import entrez
+from ..apps.base import ActionDispatcher, OptionParser, cleanup, glob, logger, mkdir, sh
+
+from .base import BaseFile, get_number, must_open
+from .gff import GffLine
 
 
 MT = "mol_type"
 LT = "locus_tag"
 
 
 class MultiGenBank(BaseFile):
@@ -47,20 +47,20 @@
             SeqIO.write([rec], fasta_fw, "fasta")
             rf = rec.features
             for f in rf:
                 self.print_gffline(gff_fw, f, seqid)
                 nfeats += 1
             nrecs += 1
 
-        logging.debug(
+        logger.debug(
             "A total of {0} records written to `{1}`.".format(nrecs, fastafile)
         )
         fasta_fw.close()
 
-        logging.debug(
+        logger.debug(
             "A total of {0} features written to `{1}`.".format(nfeats, gfffile)
         )
         gff_fw.close()
 
     def print_gffline(self, fw, f, seqid, parent=None):
 
         score = phase = "."
@@ -184,15 +184,15 @@
                 self.idfile,
                 "--format=gb",
                 "--database=nuccore",
                 "--outdir={0}".format(gbdir),
             ]
         )
 
-        logging.debug("GenBank records written to {0}.".format(gbdir))
+        logger.debug("GenBank records written to {0}.".format(gbdir))
         return gbdir
 
     @classmethod
     def write_genes_bed(cls, gbrec, outfile):
         seqid = gbrec.id.split(".")[0]
         if not seqid:
             seqid = gbrec.name.split(".")[0]
@@ -322,31 +322,31 @@
         sys.exit(not p.print_help())
 
     (gbkfile,) = args
     MultiGenBank(gbkfile)
 
 
 def preparegb(p, args):
-    p.add_option(
+    p.add_argument(
         "--gb_dir", default=None, help="path to dir containing GanBank files (.gb)"
     )
-    p.add_option(
+    p.add_argument(
         "--id",
         default=None,
         help="GenBank accession IDs in a file. One ID per row, or all IDs"
         " in one row comma separated.",
     )
-    p.add_option(
+    p.add_argument(
         "--simple",
         default=None,
-        type="string",
+        type=str,
         help="GenBank accession IDs comma separated "
         "(for lots of IDs please use --id instead).",
     )
-    p.add_option(
+    p.add_argument(
         "--individual",
         default=False,
         action="store_true",
         help="parse gb accessions individually",
     )
     opts, args = p.parse_args(args)
     accessions = opts.id
@@ -384,61 +384,61 @@
     %prog tofasta [--options]
 
     Read GenBank file, or retrieve from web.
     Output fasta file with one record per file
     or all records in one file
     """
     p = OptionParser(tofasta.__doc__)
-    p.add_option("--prefix", default="gbfasta", help="prefix of output files")
+    p.add_argument("--prefix", default="gbfasta", help="prefix of output files")
     filenames, accessions, idfile, opts, args = preparegb(p, args)
     prefix = opts.prefix
 
     GenBank(filenames=filenames, accessions=accessions, idfile=idfile).write_fasta(
         output=prefix, individual=opts.individual
     )
 
     if opts.individual:
-        logging.debug("Output written dir {0}".format(prefix))
+        logger.debug("Output written dir {0}".format(prefix))
     else:
-        logging.debug("Output written to {0}.fasta".format(prefix))
+        logger.debug("Output written to {0}.fasta".format(prefix))
 
 
 def getgenes(args):
     """
     %prog getgenes [--options]
 
     Read GenBank file, or retrieve from web.
     Output bed, cds files, and pep file (can turn off with --nopep).
     Either --gb_dir or --id/--simple should be provided.
     """
     p = OptionParser(getgenes.__doc__)
-    p.add_option("--prefix", default="gbout", help="prefix of output files")
-    p.add_option(
+    p.add_argument("--prefix", default="gbout", help="prefix of output files")
+    p.add_argument(
         "--nopep",
         default=False,
         action="store_true",
         help="Only get cds and bed, no pep",
     )
     filenames, accessions, idfile, opts, args = preparegb(p, args)
     prefix = opts.prefix
 
     GenBank(filenames=filenames, accessions=accessions, idfile=idfile).write_genes(
         output=prefix, individual=opts.individual, pep=(not opts.nopep)
     )
 
     if opts.individual:
-        logging.debug("Output written dir {0}".format(prefix))
+        logger.debug("Output written dir {0}".format(prefix))
     elif opts.nopep:
-        logging.debug(
+        logger.debug(
             "Output written to {0}.bed, {0}.cds".format(
                 prefix,
             )
         )
     else:
-        logging.debug(
+        logger.debug(
             "Output written to {0}.bed, {0}.cds, {0}.pep".format(
                 prefix,
             )
         )
 
 
 def print_locus_quals(locus_tag, locus, quals_ftypes):
@@ -463,25 +463,25 @@
     """
     %prog getquals [--options] gbkfile > qualsfile
 
     Read GenBank file and extract all qualifiers per feature type
     into a tab-delimited file
     """
     p = OptionParser(getquals.__doc__)
-    p.add_option(
+    p.add_argument(
         "--types",
         default="gene,mRNA,CDS",
-        type="str",
+        type=str,
         dest="quals_ftypes",
         help="Feature types from which to extract qualifiers",
     )
-    p.add_option(
+    p.add_argument(
         "--ignore",
         default="locus_tag,product,codon_start,translation",
-        type="str",
+        type=str,
         dest="quals_ignore",
         help="Qualifiers to exclude from parsing",
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
```

### Comparing `jcvi-1.4.6/jcvi/formats/gff.py` & `jcvi-1.4.7/jcvi/formats/gff.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,30 +5,29 @@
 import os.path as op
 import re
 import sys
 
 from collections import defaultdict
 from urllib.parse import quote, unquote
 
+from ..annotation.reformat import atg_name
 from ..apps.base import (
-    OptionParser,
-    OptionGroup,
     ActionDispatcher,
+    OptionParser,
     cleanup,
     flatten,
     logger,
     mkdir,
     need_update,
     parse_multi_values,
     sh,
 )
-from ..annotation.reformat import atg_name
 from ..utils.cbook import AutoVivification
-from ..utils.range import Range, range_minmax
 from ..utils.orderedcollections import DefaultOrderedDict, OrderedDict, parse_qs
+from ..utils.range import Range, range_minmax
 
 from .base import DictFile, LineFile, must_open, is_number
 from .bed import Bed, BedLine, natsorted
 from .fasta import Fasta, SeqIO
 
 
 Valid_strands = ("+", "-", "?", ".")
@@ -543,16 +542,16 @@
 def addparent(args):
     """
     %prog addparent file.gff
 
     Merge sister features and infer parents.
     """
     p = OptionParser(addparent.__doc__)
-    p.add_option("--childfeat", default="CDS", help="Type of children feature")
-    p.add_option("--parentfeat", default="mRNA", help="Type of merged feature")
+    p.add_argument("--childfeat", default="CDS", help="Type of children feature")
+    p.add_argument("--parentfeat", default="mRNA", help="Type of merged feature")
     p.set_outfile()
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (gff_file,) = args
@@ -809,21 +808,21 @@
     based on summation of sizes of child features.
 
     For example, for parent 'mRNA' and child 'CDS' feature types, calcuate sizes of
     mRNA by summing the sizes of the disjoint CDS parts.
     """
     p = OptionParser(sizes.__doc__)
     p.set_outfile()
-    p.add_option(
+    p.add_argument(
         "--parents",
         dest="parents",
         default="mRNA",
         help="parent feature(s) for which size is to be calculated",
     )
-    p.add_option(
+    p.add_argument(
         "--child",
         dest="child",
         default="CDS",
         help="child feature to use for size calculations",
     )
     opts, args = p.parse_args(args)
 
@@ -858,21 +857,21 @@
     If `slop` is enabled, clustering/consolidation will collapse any variation
     in terminal UTR lengths, keeping only the longest as representative.
     """
     from jcvi.utils.grouper import Grouper
     from itertools import combinations
 
     p = OptionParser(cluster.__doc__)
-    p.add_option(
+    p.add_argument(
         "--slop",
         default=False,
         action="store_true",
         help="allow minor variation in terminal 5'/3' UTR" + " start/stop position",
     )
-    p.add_option(
+    p.add_argument(
         "--inferUTR",
         default=False,
         action="store_true",
         help="infer presence of UTRs from exon coordinates",
     )
     p.set_outfile()
     opts, args = p.parse_args(args)
@@ -965,21 +964,21 @@
     Print summary stats for features of different types.
     """
     from jcvi.formats.base import SetFile
     from jcvi.formats.bed import BedSummary
     from jcvi.utils.table import tabulate
 
     p = OptionParser(summary.__doc__)
-    p.add_option(
+    p.add_argument(
         "--isoform",
         default=False,
         action="store_true",
         help="Find longest isoform of each id",
     )
-    p.add_option("--ids", help="Only include features from certain IDs")
+    p.add_argument("--ids", help="Only include features from certain IDs")
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (gff_file,) = args
     ids = opts.ids
@@ -1163,38 +1162,36 @@
     (1) feature attribute values: [Identity, Coverage].
     You can get this type of gff by using gmap
     $ gmap -f 2 ....
 
     (2) Total bp length of child features
     """
     p = OptionParser(filter.__doc__)
-    p.add_option(
+    p.add_argument(
         "--type", default="mRNA", help="The feature to scan for the attributes"
     )
-    g1 = OptionGroup(p, "Filter by identity/coverage attribute values")
-    g1.add_option("--id", default=95, type="float", help="Minimum identity")
-    g1.add_option("--coverage", default=90, type="float", help="Minimum coverage")
-    g1.add_option(
+    g1 = p.add_argument_group("Filter by identity/coverage attribute values")
+    g1.add_argument("--id", default=95, type=float, help="Minimum identity")
+    g1.add_argument("--coverage", default=90, type=float, help="Minimum coverage")
+    g1.add_argument(
         "--nocase",
         default=False,
         action="store_true",
         help="Case insensitive lookup of attribute names",
     )
-    p.add_option_group(g1)
-    g2 = OptionGroup(p, "Filter by child feature bp length")
-    g2.add_option(
-        "--child_ftype", default=None, type="str", help="Child featuretype to consider"
+    g2 = p.add_argument_group("Filter by child feature bp length")
+    g2.add_argument(
+        "--child_ftype", default=None, type=str, help="Child featuretype to consider"
     )
-    g2.add_option(
+    g2.add_argument(
         "--child_bp",
         default=None,
-        type="int",
+        type=int,
         help="Filter by total bp of children of chosen ftype",
     )
-    p.add_option_group(g2)
     p.set_outfile()
 
     opts, args = p.parse_args(args)
     otype, oid, ocov = opts.type, opts.id, opts.coverage
     cftype, clenbp = opts.child_ftype, opts.child_bp
 
     id_attr, cov_attr = "Identity", "Coverage"
@@ -1380,43 +1377,43 @@
 
     Fill in parent features by chaining child features and return extent of the
     child coordinates.
     """
     valid_merge_op = ("sum", "min", "max", "mean", "collapse")
 
     p = OptionParser(chain.__doc__)
-    p.add_option(
+    p.add_argument(
         "--key",
         dest="attrib_key",
         default=None,
         help="Attribute to use as `key` for chaining operation",
     )
-    p.add_option(
+    p.add_argument(
         "--chain_ftype",
         default="cDNA_match",
         help="GFF feature type to use for chaining operation",
     )
-    p.add_option(
+    p.add_argument(
         "--parent_ftype",
         default=None,
         help="GFF feature type to use for the chained coordinates",
     )
-    p.add_option(
+    p.add_argument(
         "--break",
         dest="break_chain",
         action="store_true",
         help="Break long chains which are non-contiguous",
     )
-    p.add_option(
+    p.add_argument(
         "--transfer_attrib",
         dest="attrib_list",
         help="Attributes to transfer to parent feature; accepts comma"
         + " separated list of attribute names",
     )
-    p.add_option(
+    p.add_argument(
         "--transfer_score",
         dest="score_merge_op",
         choices=valid_merge_op,
         help="Transfer value stored in score field to parent feature."
         + " Score is reported based on chosen operation",
     )
     p.set_outfile()
@@ -1545,144 +1542,141 @@
     """
     from jcvi.formats.obo import GODag_from_SO, validate_term
 
     valid_multiparent_ops = ["split", "merge"]
 
     p = OptionParser(format.__doc__)
 
-    g1 = OptionGroup(p, "Parameter(s) used to modify GFF attributes (9th column)")
-    g1.add_option("--name", help="Add Name attribute from two-column file")
-    g1.add_option("--note", help="Add Note attribute from two-column file")
-    g1.add_option(
+    g1 = p.add_argument_group("Parameter(s) used to modify GFF attributes (9th column)")
+    g1.add_argument("--name", help="Add Name attribute from two-column file")
+    g1.add_argument("--note", help="Add Note attribute from two-column file")
+    g1.add_argument(
         "--add_attribute",
         dest="attrib_files",
         help="Add new attribute(s) "
         + "from two-column file(s); attribute name comes from filename; "
         + "accepts comma-separated list of files",
     )
-    g1.add_option(
+    g1.add_argument(
         "--add_dbxref",
         dest="dbxref_files",
         help="Add new Dbxref value(s) (DBTAG:ID) "
         + "from two-column file(s). DBTAG comes from filename, ID comes from 2nd column; "
         + "accepts comma-separated list of files",
     )
-    g1.add_option(
+    g1.add_argument(
         "--nostrict",
         default=False,
         action="store_true",
         help="Disable strict parsing of GFF file and/or mapping file",
     )
-    g1.add_option(
+    g1.add_argument(
         "--remove_attr",
         dest="remove_attrs",
         help="Specify attributes to remove; "
         + "accepts comma-separated list of attribute names",
     )
-    g1.add_option(
+    g1.add_argument(
         "--copy_id_attr_to_name",
         default=False,
         action="store_true",
         help="Copy `ID` attribute value to `Name`, when `Name` is not defined",
     )
-    g1.add_option(
+    g1.add_argument(
         "--invent_name_attr",
         default=False,
         action="store_true",
         help="Invent `Name` attribute for 2nd level child features; "
         + "Formatted like PARENT:FEAT_TYPE:FEAT_INDEX",
     )
-    g1.add_option(
+    g1.add_argument(
         "--no_keep_attr_order",
         default=False,
         action="store_true",
         help="Do not maintain attribute order",
     )
-    p.add_option_group(g1)
 
-    g2 = OptionGroup(p, "Parameter(s) used to modify content within columns 1-8")
-    g2.add_option(
+    g2 = p.add_argument_group("Parameter(s) used to modify content within columns 1-8")
+    g2.add_argument(
         "--seqid",
         help="Switch seqid from two-column file. If not"
         + " a file, value will globally replace GFF seqid",
     )
-    g2.add_option(
+    g2.add_argument(
         "--source",
         help="Switch GFF source from two-column file. If not"
         + " a file, value will globally replace GFF source",
     )
-    g2.add_option(
+    g2.add_argument(
         "--type",
         help="Switch GFF feature type from two-column file. If not"
         + " a file, value will globally replace GFF type",
     )
-    g2.add_option(
+    g2.add_argument(
         "--fixphase",
         default=False,
         action="store_true",
         help="Change phase 1<->2, 2<->1",
     )
-    p.add_option_group(g2)
 
-    g3 = OptionGroup(
-        p, "Other parameter(s) to perform manipulations to the GFF " + "file content"
+    g3 = p.add_argument_group(
+        "Other parameter(s) to perform manipulations to the GFF file content"
     )
-    g3.add_option(
+    g3.add_argument(
         "--unique", default=False, action="store_true", help="Make IDs unique"
     )
-    g3.add_option(
+    g3.add_argument(
         "--chaindup",
         default=None,
         dest="duptype",
         help="Chain duplicate features of a particular GFF3 `type`,"
         + " sharing the same ID attribute",
     )
-    g3.add_option(
+    g3.add_argument(
         "--multiparents",
         default=None,
         choices=valid_multiparent_ops,
         help="Split/merge identical features (same `seqid`, `source`, `type`, `coord-range`, `strand`, `phase`) mapping to multiple parents",
     )
-    g3.add_option(
+    g3.add_argument(
         "--remove_feats", help="Comma separated list of features to remove by type"
     )
-    g3.add_option(
+    g3.add_argument(
         "--remove_feats_by_ID",
         help="List of features to remove by ID;"
         + " accepts comma-separated list or list file",
     )
-    g3.add_option(
+    g3.add_argument(
         "--gsac",
         default=False,
         action="store_true",
         help="Fix GSAC GFF3 file attributes",
     )
-    g3.add_option(
+    g3.add_argument(
         "--invent_protein_feat",
         default=False,
         action="store_true",
         help="Invent a protein feature span (chain CDS feats)",
     )
-    g3.add_option(
+    g3.add_argument(
         "--process_ftype",
         default=None,
-        type="str",
+        type=str,
         help="Specify feature types to process; "
         "accepts comma-separated list of feature types",
     )
-    g3.add_option(
+    g3.add_argument(
         "--gff3", default=False, action="store_true", help="Print output in GFF3 format"
     )
-    g3.add_option(
+    g3.add_argument(
         "--make_gff_store",
         default=False,
         action="store_true",
         help="Store entire GFF file in memory during first iteration",
     )
-    p.add_option_group(g3)
 
     p.set_outfile()
     p.set_SO_opts()
 
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
@@ -2059,24 +2053,24 @@
     """
     %prog fixboundaries gffile --type="gene" --child_ftype="mRNA" > gffile.fixed
 
     Adjust the boundary coordinates of parents features based on
     range chained child features, extracting their min and max values
     """
     p = OptionParser(fixboundaries.__doc__)
-    p.add_option(
+    p.add_argument(
         "--type",
         default="gene",
-        type="str",
+        type=str,
         help="Feature type for which to adjust boundaries",
     )
-    p.add_option(
+    p.add_argument(
         "--child_ftype",
         default="mRNA",
-        type="str",
+        type=str,
         help="Child featuretype(s) to use for identifying boundaries",
     )
     p.set_outfile()
 
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
@@ -2103,15 +2097,15 @@
     """
     %prog liftover gffile > liftover.gff
 
     Adjust gff coordinates based on tile number. For example,
     "gannotation.asmbl.000095.7" is the 8-th tile on asmbl.000095.
     """
     p = OptionParser(liftover.__doc__)
-    p.add_option("--tilesize", default=50000, type="int", help="The size for each tile")
+    p.add_argument("--tilesize", default=50000, type=int, help="The size for each tile")
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (gffile,) = args
     gff = Gff(gffile)
@@ -2254,24 +2248,24 @@
     gene. A second scan takes only the genes selected.
 
     --mode controls whether you want larger feature, or higher scoring feature.
     --best controls how many redundant features to keep, e.g. 10 for est2genome.
     """
     supported_modes = ("span", "score")
     p = OptionParser(uniq.__doc__)
-    p.add_option("--type", default="gene", help="Types of features to non-redundify")
-    p.add_option("--mode", default="span", choices=supported_modes, help="Pile mode")
-    p.add_option("--best", default=1, type="int", help="Use best N features")
-    p.add_option(
+    p.add_argument("--type", default="gene", help="Types of features to non-redundify")
+    p.add_argument("--mode", default="span", choices=supported_modes, help="Pile mode")
+    p.add_argument("--best", default=1, type=int, help="Use best N features")
+    p.add_argument(
         "--name",
         default=False,
         action="store_true",
         help="Non-redundify Name attribute",
     )
-    p.add_option(
+    p.add_argument(
         "--iter",
         default="2",
         choices=("1", "2"),
         help="Number of iterations to grab children",
     )
     p.set_outfile()
 
@@ -2372,21 +2366,21 @@
 
     Sort gff file using plain old unix sort based on [chromosome, start coordinate].
     or topologically based on hierarchy of features using the gt (genometools) toolkit
     """
     valid_sort_methods = ("unix", "topo")
 
     p = OptionParser(sort.__doc__)
-    p.add_option(
+    p.add_argument(
         "--method",
         default="unix",
         choices=valid_sort_methods,
         help="Specify sort method",
     )
-    p.add_option(
+    p.add_argument(
         "-i",
         dest="inplace",
         default=False,
         action="store_true",
         help="If doing a unix sort, perform sort inplace",
     )
     p.set_tmpdir()
@@ -2432,19 +2426,19 @@
     """
     %prog fromgtf gtffile
 
     Convert gtf to gff file. In gtf, the "transcript_id" will convert to "ID=",
     the "transcript_id" in exon/CDS feature will be converted to "Parent=".
     """
     p = OptionParser(fromgtf.__doc__)
-    p.add_option(
+    p.add_argument(
         "--transcript_id", default="transcript_id", help="Field name for transcript"
     )
-    p.add_option("--gene_id", default="gene_id", help="Field name for gene")
-    p.add_option(
+    p.add_argument("--gene_id", default="gene_id", help="Field name for gene")
+    p.add_argument(
         "--augustus", default=False, action="store_true", help="Input is AUGUSTUS gtf"
     )
     p.set_home("augustus")
     p.set_outfile()
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
@@ -2491,16 +2485,16 @@
     """
     %prog frombed bed_file [--options] > gff_file
 
     Convert bed to gff file. In bed, the accn will convert to key='ID'
     Default type will be `match` and default source will be `source`
     """
     p = OptionParser(frombed.__doc__)
-    p.add_option("--type", default="match", help="GFF feature type")
-    p.add_option("--source", default="default", help="GFF source qualifier")
+    p.add_argument("--type", default="match", help="GFF feature type")
+    p.add_argument("--source", default="default", help="GFF source qualifier")
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (bedfile,) = args
     bed = Bed(bedfile)
@@ -2511,16 +2505,16 @@
 
 def fromsoap(args):
     """
     %prog fromsoap soapfile > gff_file
 
     """
     p = OptionParser(fromsoap.__doc__)
-    p.add_option("--type", default="nucleotide_match", help="GFF feature type")
-    p.add_option("--source", default="soap", help="GFF source qualifier")
+    p.add_argument("--type", default="nucleotide_match", help="GFF feature type")
+    p.add_argument("--source", default="soap", help="GFF source qualifier")
     p.set_fixchrnames(orgn="maize")
     p.set_outfile()
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
@@ -2619,15 +2613,15 @@
     """
     %prog merge gffiles
 
     Merge several gff files into one. When only one file is given, it is assumed
     to be a file with a list of gff files.
     """
     p = OptionParser(merge.__doc__)
-    p.add_option(
+    p.add_argument(
         "--seq",
         default=False,
         action="store_true",
         help="Print FASTA sequences at the end",
     )
     p.set_outfile()
 
@@ -2687,31 +2681,31 @@
     --contigs: Extract particular contig(s) from the gff file. If multiple contigs are
     involved, use "," to separate, e.g. "contig_12,contig_150"; or provide a file
     with multiple contig IDs, one per line
     --names: Process particular ID(s) from the gff file. If multiple IDs are
     involved, use "," to separate; or provide a file with multiple IDs, one per line
     """
     p = OptionParser(extract.__doc__)
-    p.add_option("--contigs", help="Extract features from certain contigs")
-    p.add_option("--names", help="Extract features with certain names")
-    p.add_option(
+    p.add_argument("--contigs", help="Extract features from certain contigs")
+    p.add_argument("--names", help="Extract features with certain names")
+    p.add_argument(
         "--types",
-        type="str",
+        type=str,
         default=None,
         help="Extract features of certain feature types",
     )
-    p.add_option(
+    p.add_argument(
         "--children",
         default=0,
         choices=["1", "2"],
         help="Specify number of iterations: `1` grabs children, "
         + "`2` grabs grand-children",
     )
-    p.add_option("--tag", default="ID", help="Scan the tags for the names")
-    p.add_option(
+    p.add_argument("--tag", default="ID", help="Scan the tags for the names")
+    p.add_argument(
         "--fasta", default=False, action="store_true", help="Write FASTA if available"
     )
     p.set_outfile()
 
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
@@ -2804,26 +2798,26 @@
 def note(args):
     """
     %prog note gffile > tabfile
 
     Extract certain attribute field for each feature.
     """
     p = OptionParser(note.__doc__)
-    p.add_option(
+    p.add_argument(
         "--type",
         default=None,
         help="Only process certain types, multiple types allowed with comma",
     )
-    p.add_option(
+    p.add_argument(
         "--attribute",
         default="Parent,Note",
         help="Attribute field to extract, multiple fields allowd with comma",
     )
-    p.add_option("--AED", type="float", help="Only extract lines with AED score <=")
-    p.add_option(
+    p.add_argument("--AED", type=float, help="Only extract lines with AED score <=")
+    p.add_argument(
         "--exoncount",
         default=False,
         action="store_true",
         help="Get the exon count for each mRNA feat",
     )
     opts, args = p.parse_args(args)
 
@@ -2939,15 +2933,15 @@
     print("\t".join(str(x) for x in h1), file=fw)
     print("\t".join(str(x) for x in h2), file=fw)
     for locus in scov.keys():
         out = [locus]
         for iso in isos:
             if iso in scov[locus].keys():
                 juncs = scov[locus][iso]
-                jstats = SummaryStats(juncs, dtype="int")
+                jstats = SummaryStats(juncs, dtype=int)
                 out.extend(
                     [jstats.size, jstats.mean, jstats.median, jstats.min, jstats.max]
                 )
             else:
                 out.extend(["-"] * len(stats))
         print("\t".join(str(x) for x in out), file=fw)
     fw.close()
@@ -2957,76 +2951,76 @@
     """
     %prog bed gff_file [--options]
 
     Parses the start, stop locations of the selected features out of GFF and
     generate a bed file
     """
     p = OptionParser(bed.__doc__)
-    p.add_option(
+    p.add_argument(
         "--type",
         dest="type",
         default="gene",
         help="Feature type to extract, use comma for multiple, and `all` for all",
     )
-    p.add_option("--key", default="ID", help="Key in the attributes to extract")
-    p.add_option("--accn", help="Use fixed accn in the 4th column")
-    p.add_option("--source", help="Source to extract from, use comma for multiple")
-    p.add_option(
+    p.add_argument("--key", default="ID", help="Key in the attributes to extract")
+    p.add_argument("--accn", help="Use fixed accn in the 4th column")
+    p.add_argument("--source", help="Source to extract from, use comma for multiple")
+    p.add_argument(
         "--span",
         default=False,
         action="store_true",
         help="Use feature span in the score column",
     )
-    p.add_option(
+    p.add_argument(
         "--score_attrib",
         dest="score_attrib",
         default=False,
         help="Attribute whose value is to be used as score in `bedline`",
     )
-    p.add_option(
+    p.add_argument(
         "--append_source",
         default=False,
         action="store_true",
         help="Append GFF source name to extracted key value",
     )
-    p.add_option(
+    p.add_argument(
         "--append_ftype",
         default=False,
         action="store_true",
         help="Append GFF feature type to extracted key value",
     )
-    p.add_option(
+    p.add_argument(
         "--append_attrib",
         default=None,
         help="Append attribute to extracted key value",
     )
-    p.add_option(
+    p.add_argument(
         "--nosort",
         default=False,
         action="store_true",
         help="Do not sort the output bed file",
     )
-    p.add_option(
+    p.add_argument(
         "--primary_only",
         default=False,
         action="store_true",
         help="Only retains a single transcript per gene",
     )
-    p.add_option(
+    p.add_argument(
         "--parent_key",
         default="Parent",
         help="Parent gene key to group with --primary_only",
     )
-    p.add_option(
+    p.add_argument(
         "--human_chr",
         default=False,
         action="store_true",
         help="Only allow 1-22XY, and add `chr` prefix to seqid",
     )
-    p.add_option(
+    p.add_argument(
         "--ensembl_cds",
         default=False,
         action="store_true",
         help="Use transcript_name.exon_number as accn",
     )
     p.set_outfile()
 
@@ -3147,15 +3141,15 @@
 def children(args):
     """
     %prog children gff_file
 
     Get the children that have the same parent.
     """
     p = OptionParser(children.__doc__)
-    p.add_option(
+    p.add_argument(
         "--parents",
         default="gene",
         help="list of features to extract, use comma to separate (e.g. 'gene,mRNA')",
     )
 
     opts, args = p.parse_args(args)
 
@@ -3201,79 +3195,78 @@
 
     # can request output fasta sequence id to be picked from following attributes
     valid_id_attributes = ["ID", "Name", "Parent", "Alias", "Target", "orig_protein_id"]
 
     valid_avoid_features = ["both_strands", "strand_specific"]
 
     p = OptionParser(load.__doc__)
-    p.add_option(
+    p.add_argument(
         "--parents",
         dest="parents",
         default="mRNA",
         help="list of features to extract, use comma to separate (e.g."
         + "'gene,mRNA')",
     )
-    p.add_option(
+    p.add_argument(
         "--children",
         dest="children",
         default="CDS",
         help="list of features to extract, use comma to separate (e.g."
         + "'five_prime_UTR,CDS,three_prime_UTR')",
     )
-    p.add_option(
+    p.add_argument(
         "--feature",
         dest="feature",
         help="feature type to extract (e.g. `--feature=CDS`). Extract "
         + "up- or downstream using "
         + "upstream|downstream:TSS|TrSS|TES|TrES:length "
         + "(e.g. `--feature=upstream:TSS:500`)",
     )
-    p.add_option(
+    p.add_argument(
         "--avoidFeatures",
         default=None,
         choices=["both_strands", "strand_specific"],
         help="Specify whether or not to avoid up or downstream features",
     )
-    p.add_option(
+    p.add_argument(
         "--id_attribute",
         choices=valid_id_attributes,
         help="The attribute field to extract and use as FASTA sequence ID",
     )
-    p.add_option(
+    p.add_argument(
         "--desc_attribute",
         default="Note",
         help="The attribute field to extract and use as FASTA sequence description",
     )
-    p.add_option(
+    p.add_argument(
         "--full_header",
         default=None,
         choices=["default", "tair"],
         help="Specify if full FASTA header (with seqid, coordinates and datestamp) should be generated",
     )
 
-    g1 = OptionGroup(p, "Optional parameters (if generating full header)")
-    g1.add_option(
+    g1 = p.add_argument_group("Optional parameters (if generating full header)")
+    g1.add_argument(
         "--sep",
         dest="sep",
         default=" ",
         help="Specify separator used to delimiter header elements",
     )
-    g1.add_option(
+    g1.add_argument(
         "--datestamp",
         dest="datestamp",
         help="Specify a datestamp in the format YYYYMMDD or automatically pick `today`",
     )
-    g1.add_option(
+    g1.add_argument(
         "--conf_class",
         dest="conf_class",
         default=False,
         action="store_true",
         help="Specify if `conf_class` attribute should be parsed and placed in the header",
     )
-    p.add_option_group(g1)
 
     p.set_outfile()
 
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(p.print_help())
@@ -3696,17 +3689,17 @@
     8. thickEnd
     9. itemRgb
     10. blockCount
     11. blockSizes
     12. blockStarts
     """
     p = OptionParser(bed12.__doc__)
-    p.add_option("--parent", default="mRNA", help="Top feature type")
-    p.add_option("--block", default="exon", help="Feature type for regular blocks")
-    p.add_option("--thick", default="CDS", help="Feature type for thick blocks")
+    p.add_argument("--parent", default="mRNA", help="Top feature type")
+    p.add_argument("--block", default="exon", help="Feature type for regular blocks")
+    p.add_argument("--thick", default="CDS", help="Feature type for thick blocks")
     p.set_outfile()
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (gffile,) = args
```

### Comparing `jcvi-1.4.6/jcvi/formats/html.py` & `jcvi-1.4.7/jcvi/formats/html.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 # -*- coding: UTF-8 -*-
 
 """
 Parse html pages.
 """
 import os.path as op
 import sys
-import logging
 
-from BeautifulSoup import BeautifulSoup
 from urllib.parse import urljoin
 
-from jcvi.apps.base import OptionParser, ActionDispatcher, download
+from BeautifulSoup import BeautifulSoup
+
+from ..apps.base import ActionDispatcher, OptionParser, download, logger
 
 
 def main():
 
     actions = (
         ("table", "convert HTML tables to csv"),
         ("links", "extract all links from web page"),
@@ -36,16 +36,16 @@
 
     Maps the images from local to remote.
     """
     from more_itertools import grouper
     from jcvi.apps.base import iglob
 
     p = OptionParser(gallery.__doc__)
-    p.add_option("--columns", default=3, type="int", help="How many cells per row")
-    p.add_option("--width", default=200, type="int", help="Image width")
+    p.add_argument("--columns", default=3, type=int, help="How many cells per row")
+    p.add_argument("--width", default=200, type=int, help="Image width")
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     folder, link_prefix = args
     width = opts.width
@@ -68,15 +68,15 @@
 def links(args):
     """
     %prog links url
 
     Extract all the links "<a href=''>" from web page.
     """
     p = OptionParser(links.__doc__)
-    p.add_option(
+    p.add_argument(
         "--img",
         default=False,
         action="store_true",
         help="Extract <img> tags",
     )
     opts, args = p.parse_args(args)
 
@@ -147,12 +147,12 @@
                     cell = "".join(td.find(text=True))
                     cell = unescape(cell)
                 except TypeError:
                     cell = ""
                 row.append(cell)
             writer.writerow(row)
             nrows += 1
-        logging.debug("Table with {0} rows written to `{1}`.".format(nrows, csvfile))
+        logger.debug("Table with %d rows written to `%s`.", nrows, csvfile)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `jcvi-1.4.6/jcvi/formats/maf.py` & `jcvi-1.4.7/jcvi/formats/maf.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 <http://genome.ucsc.edu/FAQ/FAQformat#format5>
 """
 import sys
 
 from bx import interval_index_file
 from bx.align import maf
 
-from jcvi.formats.base import BaseFile
-from jcvi.apps.base import OptionParser, ActionDispatcher, need_update
-from jcvi.apps.lastz import blastz_score_to_ncbi_expectation, blastz_score_to_ncbi_bits
+from ..apps.base import ActionDispatcher, OptionParser, need_update
+from ..apps.lastz import blastz_score_to_ncbi_expectation, blastz_score_to_ncbi_bits
+
+from .base import BaseFile
 
 
 class Maf(BaseFile, dict):
     def __init__(self, filename, index=False):
         super(Maf, self).__init__(filename)
 
         indexfile = filename + ".idx"
```

### Comparing `jcvi-1.4.6/jcvi/formats/obo.py` & `jcvi-1.4.7/jcvi/formats/obo.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 """
 %prog obo_file
 
 Parses obo_file and plot GO lineage
 """
 import sys
-import logging
 
 from collections import deque
 from functools import partial
 from typing import IO, Optional
 
 from goatools.obo_parser import GODag
-from jcvi.apps.base import OptionParser
+
+from ..apps.base import OptionParser, logger
 
 GO_URL = "http://purl.obolibrary.org/obo/go/go-basic.obo"
 SO_URL = (
     "http://obo.cvs.sourceforge.net/viewvc/obo/obo/ontology/genomic-proteomic/so.obo"
 )
 
 
@@ -60,25 +60,25 @@
                 tparts = deque(term.split("_"))
                 tparts.pop() if "prefix" in method else tparts.popleft()
                 nterm = "_".join(tparts).strip()
                 term = validate_term(nterm, so=so, method=method)
             if term is None:
                 return None
         else:
-            logging.error("Term `{0}` does not exist".format(term))
+            logger.error("Term `%s` does not exist", term)
             sys.exit(1)
 
     if oterm != term:
-        logging.debug("Resolved term `{0}` to `{1}`".format(oterm, term))
+        logger.debug("Resolved term `%s` to `%s`", oterm, term)
     return term
 
 
 if __name__ == "__main__":
     p = OptionParser(__doc__)
-    p.add_option(
+    p.add_argument(
         "--term",
         help="Write the parents and children of this query term",
     )
 
     opts, args = p.parse_args()
 
     if len(args) != 1:
```

### Comparing `jcvi-1.4.6/jcvi/formats/paf.py` & `jcvi-1.4.7/jcvi/formats/paf.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 # formats
 #
 # Created by Haibao Tang on 09/03/20
 # Copyright © 2020 Haibao Tang. All rights reserved.
 #
 
 import sys
-import logging
 
-from jcvi.formats.base import must_open
-from jcvi.apps.base import OptionParser, ActionDispatcher
+from ..apps.base import ActionDispatcher, OptionParser, logger
+
+from .base import must_open
 
 
 class PAFLine:
     """
     PAF specification
     https://github.com/lh3/miniasm/blob/master/PAF.md
     """
@@ -86,15 +86,15 @@
 
     Print out BED file based on coordinates in BLAST PAF results. By default,
     write out subject positions. Use --swap to write query positions.
     """
     from jcvi.formats.bed import sort as sort_bed
 
     p = OptionParser(bed.__doc__)
-    p.add_option(
+    p.add_argument(
         "--swap", default=False, action="store_true", help="Write query positions"
     )
 
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
@@ -108,15 +108,15 @@
         for row in fp:
             b = PAFLine(row)
             if write_qbed:
                 print(b.qbedline, file=fw)
             else:
                 print(b.sbedline, file=fw)
 
-    logging.debug("File written to `%s`.", bedfile)
+    logger.debug("File written to `%s`.", bedfile)
     sort_bed([bedfile, "-i"])
     return bedfile
 
 
 def main():
     actions = (("bed", "get BED file from PAF"),)
     p = ActionDispatcher(actions)
```

### Comparing `jcvi-1.4.6/jcvi/formats/pdf.py` & `jcvi-1.4.7/jcvi/formats/pdf.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 """
 Manipulate PDF files, using PyPDF2 library.
 """
-import os
 import sys
-import logging
 import traceback
 
 from natsort import natsorted
 
 from PyPDF2 import PdfFileMerger, parse_filename_page_ranges
 from PyPDF2.pagerange import PAGE_RANGE_HELP
-from jcvi.formats.base import must_open
-from jcvi.apps.base import OptionParser, ActionDispatcher, cleanup
+
+from ..apps.base import ActionDispatcher, OptionParser, cleanup, logger
+
+from .base import must_open
 
 
 def main():
 
     actions = (("cat", "concatenate pages from pdf files into a single pdf file"),)
     p = ActionDispatcher(actions)
     p.dispatch(globals())
@@ -43,18 +43,18 @@
         pdfcat chapter*.pdf >book.pdf
             You can specify the output file by redirection.
 
         pdfcat chapter?.pdf chapter10.pdf >book.pdf
             In case you don't want chapter 10 before chapter 2.
     """
     p = OptionParser(cat.__doc__.format(page_range_help=PAGE_RANGE_HELP))
-    p.add_option(
+    p.add_argument(
         "--nosort", default=False, action="store_true", help="Do not sort file names"
     )
-    p.add_option(
+    p.add_argument(
         "--cleanup",
         default=False,
         action="store_true",
         help="Remove individual pdfs after merging",
     )
     p.set_outfile()
     p.set_verbose(help="Show page ranges as they are being read")
@@ -87,13 +87,13 @@
         print(traceback.format_exc(), file=sys.stderr)
         print("Error while reading " + filename, file=sys.stderr)
         sys.exit(1)
     merger.write(fw)
     fw.close()
 
     if opts.cleanup:
-        logging.debug("Cleaning up {} files".format(len(args)))
+        logger.debug("Cleaning up %d files", len(args))
         cleanup(args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `jcvi-1.4.6/jcvi/formats/psl.py` & `jcvi-1.4.7/jcvi/formats/psl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 """
 Classes to handle the .psl files
 """
-import sys
 import math
 import re
+import sys
+
+from ..apps.base import ActionDispatcher, OptionParser
 
-from jcvi.formats.base import LineFile, must_open
-from jcvi.apps.base import OptionParser, ActionDispatcher
+from .base import LineFile, must_open
 
 
 class PslLine(object):
     def __init__(self, sline):
         args = sline.strip().split()
         self.nargs = len(args)
         self.matches = int(args[0])
@@ -308,28 +309,28 @@
 def gff(args):
     """
     %prog gff pslfile
 
     Convert to gff format.
     """
     p = OptionParser(gff.__doc__)
-    p.add_option("--source", default="GMAP", help="specify GFF source")
-    p.add_option(
+    p.add_argument("--source", default="GMAP", help="specify GFF source")
+    p.add_argument(
         "--type",
         default="EST_match",
         help="specify GFF feature type",
     )
-    p.add_option("--suffix", default=".match", help="match ID suffix")
-    p.add_option(
+    p.add_argument("--suffix", default=".match", help="match ID suffix")
+    p.add_argument(
         "--swap",
         default=False,
         action="store_true",
         help="swap query and target features",
     )
-    p.add_option(
+    p.add_argument(
         "--simple_score",
         default=False,
         action="store_true",
         help="calculate a simple percent score",
     )
     p.set_outfile()
```

### Comparing `jcvi-1.4.6/jcvi/formats/pyblast.py` & `jcvi-1.4.7/jcvi/formats/pyblast.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.6/jcvi/formats/sam.py` & `jcvi-1.4.7/jcvi/formats/sam.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,37 +6,38 @@
 This script simply parses the lines in SAM into human readable fields.
 
 http://samtools.sourceforge.net/SAM1.pdf
 """
 import os
 import os.path as op
 import sys
-import logging
 
 from collections import defaultdict
 from itertools import groupby
 
-from jcvi.formats.base import LineFile, must_open
-from jcvi.formats.fasta import Fasta
-from jcvi.formats.sizes import Sizes
-from jcvi.utils.cbook import fill
-from jcvi.assembly.base import Astat
-from jcvi.apps.base import (
-    OptionParser,
+from ..apps.base import (
     ActionDispatcher,
-    Popen,
+    OptionParser,
     PIPE,
+    Popen,
     cleanup,
-    need_update,
-    sh,
-    mkdir,
+    get_abs_path,
     glob,
+    logger,
+    mkdir,
+    need_update,
     popen,
-    get_abs_path,
+    sh,
 )
+from ..utils.cbook import fill
+from ..assembly.base import Astat
+
+from .base import LineFile, must_open
+from .fasta import Fasta
+from .sizes import Sizes
 
 
 class SamLine(object):
     def __init__(self, row):
 
         args = row.strip().split("\t")
         self.qname = args[0]
@@ -162,15 +163,15 @@
     xregion = region.replace(":", "_").replace("-", "_").replace(",", "")
     minibamfile = op.basename(bamfile).replace(".bam", ".{}.bam".format(xregion))
     baifile = minibamfile + ".bai"
     if op.exists(baifile):
         sh("rm {}".format(baifile))
 
     if not overwrite and op.exists(minibamfile):
-        logging.error("Output name exists: `{}`".format(minibamfile))
+        logger.error("Output name exists: `{}`".format(minibamfile))
         return
 
     cmd = "samtools view {} {} -b".format(bamfile, region)
     cmd += " -o {0}".format(minibamfile)
 
     sh(cmd)
     sh("samtools index {0}".format(minibamfile))
@@ -306,15 +307,15 @@
     """
     %prog append bamfile
 
     Append /1 or /2 to read names. Useful for using the Tophat2 bam file for
     training AUGUSTUS gene models.
     """
     p = OptionParser(append.__doc__)
-    p.add_option("--prepend", help="Prepend string to read names")
+    p.add_argument("--prepend", help="Prepend string to read names")
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (bamfile,) = args
     prepend = opts.prepend
@@ -375,15 +376,15 @@
 
     mkdir(merged_bams)
     bams = []
     for x in bamdirs:
         bams += glob(op.join(x, "*.bam"))
     bams = [x for x in bams if "nsorted" not in x]
 
-    logging.debug("Found a total of {0} BAM files.".format(len(bams)))
+    logger.debug("Found a total of {0} BAM files.".format(len(bams)))
 
     sep = opts.sep
     key = lambda x: op.basename(x).split(sep)[0]
     bams.sort(key=key)
     mm = MakeManager()
     for prefix, files in groupby(bams, key=key):
         files = sorted(list(files))
@@ -403,15 +404,15 @@
 def count(args):
     """
     %prog count bamfile gtf
 
     Count the number of reads mapped using `htseq-count`.
     """
     p = OptionParser(count.__doc__)
-    p.add_option("--type", default="exon", help="Only count feature type")
+    p.add_argument("--type", default="exon", help="Only count feature type")
     p.set_cpus(cpus=8)
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     bamfile, gtf = args
@@ -440,31 +441,33 @@
     """
     %prog coverage fastafile bamfile
 
     Calculate coverage for BAM file. BAM file will be sorted unless with
     --nosort.
     """
     p = OptionParser(coverage.__doc__)
-    p.add_option(
+    p.add_argument(
         "--format",
         default="bigwig",
         choices=("bedgraph", "bigwig", "coverage"),
         help="Output format",
     )
-    p.add_option("--nosort", default=False, action="store_true", help="Do not sort BAM")
+    p.add_argument(
+        "--nosort", default=False, action="store_true", help="Do not sort BAM"
+    )
     p.set_outfile()
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     fastafile, bamfile = args
     format = opts.format
     if opts.nosort:
-        logging.debug("BAM sorting skipped")
+        logger.debug("BAM sorting skipped")
     else:
         bamfile = index([bamfile, "--fasta={0}".format(fastafile)])
 
     pf = bamfile.rsplit(".", 2)[0]
     sizesfile = Sizes(fastafile).filename
     cmd = "genomeCoverageBed -ibam {0} -g {1}".format(bamfile, sizesfile)
     if format in ("bedgraph", "bigwig"):
@@ -525,15 +528,15 @@
                         ".",
                         "ID=" + key,
                     )
                 ),
                 file=fw,
             )
         fw.close()
-        logging.debug("Dummy GFF created: {0}".format(gffile))
+        logger.debug("Dummy GFF created: {0}".format(gffile))
 
     cmd = "cuffdiff {0} {1}".format(gffile, " ".join(bamfiles))
     sh(cmd)
 
 
 def pairs(args):
     """
@@ -564,18 +567,18 @@
     %prog consensus fastafile bamfile
 
     Convert bam alignments to consensus FASTQ/FASTA. See also:
     https://cbc.brown.edu/blog/consensus-vcf/
     """
     valid_callers = ("bcftools", "gatk4")
     p = OptionParser(consensus.__doc__)
-    p.add_option(
+    p.add_argument(
         "--nosort", default=False, action="store_true", help="Do not sort the BAM files"
     )
-    p.add_option(
+    p.add_argument(
         "--caller",
         default="bcftools",
         choices=valid_callers,
         help="Use consensus caller",
     )
     opts, args = p.parse_args(args)
 
@@ -606,18 +609,18 @@
     Call SNPs on bam files.
     """
     from jcvi.apps.grid import Jobs
 
     valid_callers = ("mpileup", "freebayes")
     p = OptionParser(vcf.__doc__)
     p.set_outfile(outfile="out.vcf.gz")
-    p.add_option(
+    p.add_argument(
         "--nosort", default=False, action="store_true", help="Do not sort the BAM files"
     )
-    p.add_option(
+    p.add_argument(
         "--caller", default="mpileup", choices=valid_callers, help="Use variant caller"
     )
     opts, args = p.parse_args(args)
 
     if len(args) < 2:
         sys.exit(not p.print_help())
 
@@ -700,18 +703,18 @@
 def index(args):
     """
     %prog index samfile/bamfile
 
     If SAM file, convert to BAM, sort and then index, using SAMTOOLS
     """
     p = OptionParser(index.__doc__)
-    p.add_option(
+    p.add_argument(
         "--fasta", dest="fasta", default=None, help="add @SQ header to the BAM file"
     )
-    p.add_option(
+    p.add_argument(
         "--unique",
         default=False,
         action="store_true",
         help="only retain uniquely mapped reads",
     )
     p.set_cpus()
     opts, args = p.parse_args(args)
@@ -796,15 +799,15 @@
         view_opts.append(uopts)
 
     outfile = samfile.replace(oext, ".mapped{0}".format(ext))
     mopts.extend(["-F4", samfile, "-o{0}".format(outfile)])
     view_opts.append(mopts)
 
     for vo in view_opts:
-        logging.debug("samtools view {0}".format(" ".join(vo)))
+        logger.debug("samtools view {0}".format(" ".join(vo)))
 
     jobs = Jobs(pysam.view, [(z for z in x) for x in view_opts])
     jobs.run()
 
 
 def pair(args):
     """
@@ -883,47 +886,47 @@
     convert bam format to ace format. This often allows the remapping to be
     assessed as a denovo assembly format. bam file needs to be indexed. also
     creates a .mates file to be used in amos/bambus, and .astat file to mark
     whether the contig is unique or repetitive based on A-statistics in Celera
     assembler.
     """
     p = OptionParser(ace.__doc__)
-    p.add_option(
+    p.add_argument(
         "--splitdir",
         dest="splitdir",
         default="outRoot",
         help="split the ace per contig to dir",
     )
-    p.add_option(
+    p.add_argument(
         "--unpaired",
         dest="unpaired",
         default=False,
         help="remove read pairs on the same contig",
     )
-    p.add_option(
+    p.add_argument(
         "--minreadno",
         dest="minreadno",
         default=3,
-        type="int",
+        type=int,
         help="minimum read numbers per contig",
     )
-    p.add_option(
+    p.add_argument(
         "--minctgsize",
         dest="minctgsize",
         default=100,
-        type="int",
+        type=int,
         help="minimum contig size per contig",
     )
-    p.add_option(
+    p.add_argument(
         "--astat",
         default=False,
         action="store_true",
         help="create .astat to list repetitiveness",
     )
-    p.add_option(
+    p.add_argument(
         "--readids",
         default=False,
         action="store_true",
         help="create file of mapped and unmapped ids",
     )
 
     from pysam import Samfile
@@ -939,24 +942,24 @@
 
     f = Fasta(fastafile)
     prefix = bamfile.split(".")[0]
     acefile = prefix + ".ace"
     readsfile = prefix + ".reads"
     astatfile = prefix + ".astat"
 
-    logging.debug("Load {0}".format(bamfile))
+    logger.debug("Load {0}".format(bamfile))
     s = Samfile(bamfile, "rb")
 
     ncontigs = s.nreferences
     genomesize = sum(x for a, x in f.itersizes())
-    logging.debug("Total {0} contigs with size {1} base".format(ncontigs, genomesize))
+    logger.debug("Total {0} contigs with size {1} base".format(ncontigs, genomesize))
     qual = "20"  # default qual
 
     totalreads = sum(s.count(x) for x in s.references)
-    logging.debug("Total {0} reads mapped".format(totalreads))
+    logger.debug("Total {0} reads mapped".format(totalreads))
 
     fw = open(acefile, "w")
     if astat:
         astatfw = open(astatfile, "w")
     if readids:
         readsfw = open(readsfile, "w")
```

### Comparing `jcvi-1.4.6/jcvi/formats/sizes.py` & `jcvi-1.4.7/jcvi/formats/sizes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 import os.path as op
 import sys
-import logging
 
 import numpy as np
 
-from jcvi.formats.base import LineFile
-from jcvi.apps.base import (
-    OptionParser,
+from ..apps.base import (
     ActionDispatcher,
+    OptionParser,
     cleanup,
     get_abs_path,
+    logger,
     need_update,
 )
+from .base import LineFile
 
 
 class Sizes(LineFile):
     """
     Two-column .sizes file, often generated by `faSize -detailed`
     contigID size
     """
@@ -152,16 +152,16 @@
         set_ticklabels_helvetica,
     )
 
     p = OptionParser(histogram.__doc__)
     p.set_histogram(
         vmax=50000, bins=100, xlabel="Read length", title="Read length distribution"
     )
-    p.add_option("--ylabel1", default="Counts", help="Label of y-axis on the left")
-    p.add_option(
+    p.add_argument("--ylabel1", default="Counts", help="Label of y-axis on the left")
+    p.add_argument(
         "--color",
         default="0",
         choices=[str(x) for x in range(8)],
         help="Color of bars, which is an index 0-7 in brewer set2",
     )
     opts, args, iopts = p.set_image_options(args, figsize="6x6", style="dark")
 
@@ -276,14 +276,14 @@
     fw = open(agpfile, "w")
     o = OO()  # Without a filename
     for ctg, size in sizes.iter_sizes():
         o.add(ctg, ctg, size)
 
     o.write_AGP(fw)
     fw.close()
-    logging.debug("AGP file written to `{0}`.".format(agpfile))
+    logger.debug("AGP file written to `%s`.", agpfile)
 
     return agpfile
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `jcvi-1.4.6/jcvi/formats/vcf.py` & `jcvi-1.4.7/jcvi/formats/vcf.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 # -*- coding: UTF-8 -*-
 
 """
 Variant call format.
 """
 import os.path as op
 import sys
-import logging
 
 from collections import defaultdict
 from itertools import groupby
 from pyfaidx import Fasta
 from pyliftover import LiftOver
 
-from jcvi.formats.base import must_open
-from jcvi.formats.sizes import Sizes
-from jcvi.utils.cbook import percentage
-from jcvi.apps.base import OptionParser, ActionDispatcher, need_update, sh
+from ..apps.base import ActionDispatcher, OptionParser, logger, need_update, sh
+from ..utils.cbook import percentage
+
+from .base import must_open
+from .sizes import Sizes
 
 
 class VcfLine:
     def __init__(self, row):
         args = row.strip().split("\t")
         self.seqid = args[0]
         self.pos = int(args[1])
@@ -108,15 +108,15 @@
                 )
         elif new is None:
             exception_string = "Chromosome '{}' provided not in chain file".format(
                 chromosome
             )
 
         if verbose:
-            logging.error(exception_string)
+            logger.error(exception_string)
         return None, None
 
 
 CM = dict(
     list(
         zip([str(x) for x in range(1, 23)], ["chr{0}".format(x) for x in range(1, 23)])
     )
@@ -147,15 +147,15 @@
     %prog validate input.vcf genome.fasta
 
     Fasta validation of vcf file.
     """
     import pyfasta
 
     p = OptionParser(validate.__doc__)
-    p.add_option("--prefix", help="Add prefix to seqid")
+    p.add_argument("--prefix", help="Add prefix to seqid")
     opts, args = p.parse_args(args)
 
     vcffile, fastafile = args
     pf = opts.prefix
     genome = pyfasta.Fasta(fastafile, record_class=pyfasta.MemoryRecord)
     fp = must_open(vcffile)
     match_ref = match_alt = total = 0
@@ -173,16 +173,16 @@
         if total % 100000 == 0:
             print(total, "sites parsed", file=sys.stderr)
         if ref == true_ref:
             match_ref += 1
         elif alt == true_ref:
             match_alt += 1
 
-    logging.debug("Match REF: {}".format(percentage(match_ref, total)))
-    logging.debug("Match ALT: {}".format(percentage(match_alt, total)))
+    logger.debug("Match REF: {}".format(percentage(match_ref, total)))
+    logger.debug("Match ALT: {}".format(percentage(match_alt, total)))
 
 
 def uniq(args):
     """
     %prog uniq vcffile
 
     Retain only the first entry in vcf file.
@@ -243,16 +243,16 @@
             continue
         if random() < ratio:
             nkept += 1
             print(row.strip(), file=fwk)
         else:
             nwithheld += 1
             print(row.strip(), file=fww)
-    logging.debug("{0} records kept to `{1}`".format(nkept, kept))
-    logging.debug("{0} records withheld to `{1}`".format(nwithheld, withheld))
+    logger.debug("{0} records kept to `{1}`".format(nkept, kept))
+    logger.debug("{0} records withheld to `{1}`".format(nwithheld, withheld))
 
 
 def get_vcfstanza(fastafile, sampleid="SAMP_001"):
     from jcvi.formats.base import timestamp
 
     # VCF spec
     m = "##fileformat=VCFv4.1\n"
@@ -333,15 +333,15 @@
         for rsid in rsids:
             if rsid in register:
                 pos1, ref1, alt1 = register[rsid]
                 if alt not in alt1:
                     register[rsid][-1].append(alt)
             else:
                 register[rsid] = (pos, ref, [alt])
-    logging.debug(
+    logger.debug(
         "A total of {0} sites imported from `{1}`".format(len(register), legend)
     )
     return register
 
 
 def from23andme(args):
     """
@@ -439,29 +439,29 @@
             max_allele = max((len(x), x) for x in alleles)[1]
             alleles = [("I" if x == max_allele else "D") for x in alleles]
             assert "I" in alleles and "D" in alleles
         a, b = genotype
         try:
             ia, ib = alleles.index(a), alleles.index(b)
         except ValueError:  # alleles not seen
-            logging.error(
+            logger.error(
                 "{0}: alleles={1}, genotype={2}".format(rsid, alleles, genotype)
             )
             skipped += 1
             continue
         code = "/".join(str(x) for x in sorted((ia, ib)))
 
         print(
             "\t".join(
                 str(x) for x in (chr, pos, rsid, ref, alt, ".", ".", "PR", "GT", code)
             ),
             file=fw,
         )
 
-    logging.debug(
+    logger.debug(
         "duplicates={0} skipped={1} missing={2}".format(duplicates, skipped, missing)
     )
 
 
 def refallele(args):
     """
     %prog refallele vcffile > out.refAllele
@@ -492,18 +492,18 @@
     Given SNP locations, summarize the locations in the sequences. For example,
     find out if there are more 3`-SNPs than 5`-SNPs.
     """
     from jcvi.formats.bed import BedLine
     from jcvi.graphics.histogram import stem_leaf_plot
 
     p = OptionParser(location.__doc__)
-    p.add_option(
+    p.add_argument(
         "--dist",
         default=100,
-        type="int",
+        type=int,
         help="Distance cutoff to call 5` and 3`",
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
@@ -547,16 +547,16 @@
     Only three-column file is supported:
     locus_id    intra- genotype    inter- genotype
     """
     from jcvi.utils.cbook import thousands
     from jcvi.utils.table import tabulate
 
     p = OptionParser(summary.__doc__)
-    p.add_option("--counts", help="Print SNP counts in a txt file")
-    p.add_option("--bed", help="Print SNPs locations in a bed file")
+    p.add_argument("--counts", help="Print SNP counts in a txt file")
+    p.add_argument("--bed", help="Print SNPs locations in a bed file")
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     txtfile, fastafile = args
     bedfw = open(opts.bed, "w") if opts.bed else None
@@ -590,15 +590,15 @@
         inter = alt + "-" + inter
         combinations[(intra, inter)] += 1
 
         if bedfw:
             print("\t".join(str(x) for x in (ctg, pos - 1, pos, locus)), file=bedfw)
 
     if bedfw:
-        logging.debug("SNP locations written to `{0}`.".format(opts.bed))
+        logger.debug("SNP locations written to `{0}`.".format(opts.bed))
         bedfw.close()
 
     nsites = sum(len(x) for x in snps.values())
     sizes = Sizes(fastafile)
     bpsize = sizes.totalsize
     snprate = lambda a: a * 1000.0 / bpsize
     m = "Dataset `{0}` contains {1} contigs ({2} bp).\n".format(
@@ -640,15 +640,15 @@
 
     for ctg in sorted(snps.keys()):
         snpcount = snpcounts[ctg]
         goodsnpcount = goodsnpcounts[ctg]
         print("\t".join(str(x) for x in (ctg, snpcount, goodsnpcount)), file=fw)
 
     fw.close()
-    logging.debug("SNP counts per contig is written to `{0}`.".format(snpcountsfile))
+    logger.debug("SNP counts per contig is written to `{0}`.".format(snpcountsfile))
 
 
 g2x = {"0/0": "A", "0/1": "X", "1/1": "B", "./.": "-", ".": "-"}
 
 
 def encode_genotype(s, mindepth=3, depth_index=2, nohet=False):
     """
@@ -681,51 +681,51 @@
     %prog mstmap bcffile/vcffile > matrixfile
 
     Convert bcf/vcf format to mstmap input.
     """
     from jcvi.assembly.geneticmap import MSTMatrix
 
     p = OptionParser(mstmap.__doc__)
-    p.add_option(
+    p.add_argument(
         "--dh",
         default=False,
         action="store_true",
         help="Double haploid population, no het",
     )
-    p.add_option(
+    p.add_argument(
         "--freq",
         default=0.2,
-        type="float",
+        type=float,
         help="Allele must be above frequency",
     )
-    p.add_option(
+    p.add_argument(
         "--mindepth",
         default=3,
-        type="int",
+        type=int,
         help="Only trust genotype calls with depth",
     )
-    p.add_option(
+    p.add_argument(
         "--missing_threshold",
         default=0.25,
-        type="float",
+        type=float,
         help="Fraction missing must be below",
     )
-    p.add_option(
+    p.add_argument(
         "--noheader",
         default=False,
         action="store_true",
         help="Do not print MSTmap run parameters",
     )
-    p.add_option(
+    p.add_argument(
         "--pv4",
         default=False,
         action="store_true",
         help="Enable filtering strand-bias, tail distance bias, etc.",
     )
-    p.add_option(
+    p.add_argument(
         "--freebayes",
         default=False,
         action="store_true",
         help="VCF output from freebayes",
     )
     p.set_sep(sep=".", help="Use separator to simplify individual names")
     p.set_outfile()
@@ -792,15 +792,15 @@
 def liftover(args):
     """
     %prog liftover old.vcf hg19ToHg38.over.chain.gz new.vcf
 
     Lift over coordinates in vcf file.
     """
     p = OptionParser(liftover.__doc__)
-    p.add_option(
+    p.add_argument(
         "--newid", default=False, action="store_true", help="Make new identifiers"
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 3:
         sys.exit(not p.print_help())
 
@@ -838,12 +838,12 @@
             v.seqid, v.pos = new_chrom, new_pos
             if opts.newid:
                 v.rsid = "{0}:{1}".format(new_chrom.replace("chr", ""), new_pos)
             print(v, file=fw)
         else:
             num_excluded += 1
 
-    logging.debug("Excluded {0}".format(num_excluded))
+    logger.debug("Excluded {0}".format(num_excluded))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `jcvi-1.4.6/jcvi/graphics/align.py` & `jcvi-1.4.7/jcvi/graphics/align.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,22 +10,24 @@
 - Optical map alignment, matchings between restriction fragments
 """
 
 
 import sys
 
 from bisect import bisect
-from more_itertools import pairwise
 from random import choice, randint
 
-from jcvi.utils.range import range_overlap
-from jcvi.graphics.chromosome import Chromosome, HorizontalChromosome
-from jcvi.graphics.glyph import BaseGlyph, GeneGlyph
-from jcvi.graphics.base import FancyArrow, Rectangle, plt, savefig, normalize_axes
-from jcvi.apps.base import OptionParser
+from more_itertools import pairwise
+
+from ..apps.base import OptionParser
+from ..utils.range import range_overlap
+
+from .base import FancyArrow, Rectangle, plt, savefig, normalize_axes
+from .chromosome import Chromosome, HorizontalChromosome
+from .glyph import BaseGlyph, GeneGlyph
 
 
 class BaseAlign(object):
     def __init__(self, fig, xywh, xpad=0, ypad=0, xmax=100):
         x, y, w, h = xywh
         self.ax = fig.add_axes(xywh)
         self.sax = fig.add_axes(
```

### Comparing `jcvi-1.4.6/jcvi/graphics/assembly.py` & `jcvi-1.4.7/jcvi/graphics/assembly.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 """
 Assembly QC plots, including general statistics, base and mate coverages, and
 scaffolding consistencies.
 """
-import sys
-import logging
 import os.path as op
+import sys
+
+from ..apps.base import ActionDispatcher, OptionParser, logger, need_update
+from ..assembly.base import calculate_A50
+from ..assembly.coverage import Coverage
+from ..formats.bed import Bed, BedLine
+from ..formats.fasta import Fasta
+from ..formats.sizes import Sizes
+from ..utils.cbook import thousands
 
-from jcvi.formats.fasta import Fasta
-from jcvi.formats.bed import Bed, BedLine
-from jcvi.formats.sizes import Sizes
-from jcvi.assembly.base import calculate_A50
-from jcvi.assembly.coverage import Coverage
-from jcvi.graphics.base import plt, Rectangle, set_human_base_axis, savefig
-from jcvi.utils.cbook import thousands
-from jcvi.apps.base import OptionParser, ActionDispatcher, need_update
+from .base import plt, Rectangle, set_human_base_axis, savefig
 
 
 def main():
     actions = (
         ("A50", "compare A50 graphics for a set of FASTA files"),
         ("coverage", "plot coverage from a set of BED files"),
         ("qc", "performs QC graphics on given contig/scaffold"),
@@ -40,18 +40,18 @@
     """
     import numpy as np
     import pandas as pd
     import seaborn as sns
     from jcvi.formats.base import DictFile
 
     p = OptionParser(covlen.__doc__)
-    p.add_option("--maxsize", default=1000000, type="int", help="Max contig size")
-    p.add_option("--maxcov", default=100, type="int", help="Max contig size")
-    p.add_option("--color", default="m", help="Color of the data points")
-    p.add_option(
+    p.add_argument("--maxsize", default=1000000, type=int, help="Max contig size")
+    p.add_argument("--maxcov", default=100, type=int, help="Max contig size")
+    p.add_argument("--color", default="m", help="Color of the data points")
+    p.add_argument(
         "--kind",
         default="scatter",
         choices=("scatter", "reg", "resid", "kde", "hex"),
         help="Kind of plot to draw",
     )
     opts, args, iopts = p.set_image_options(args, figsize="8x8")
 
@@ -70,15 +70,15 @@
         if c > maxcov:
             continue
         data.append((size, c))
 
     x, y = zip(*data)
     x = np.array(x)
     y = np.array(y)
-    logging.debug("X size {0}, Y size {1}".format(x.size, y.size))
+    logger.debug("X size {0}, Y size {1}".format(x.size, y.size))
 
     df = pd.DataFrame()
     xlab, ylab = "Length", "Coverage of depth (X)"
     df[xlab] = x
     df[ylab] = y
     sns.jointplot(
         xlab,
@@ -105,16 +105,16 @@
     mates. ctg is the chr/scf/ctg that you want to plot the histogram on.
 
     If the bedfiles already contain the clone spans, turn on --spans.
     """
     from jcvi.formats.bed import mates, bedpe
 
     p = OptionParser(coverage.__doc__)
-    p.add_option("--ymax", default=None, type="int", help="Limit ymax")
-    p.add_option(
+    p.add_argument("--ymax", default=None, type=int, help="Limit ymax")
+    p.add_argument(
         "--spans",
         default=False,
         action="store_true",
         help="BED files already contain clone spans",
     )
     opts, args, iopts = p.set_image_options(args, figsize="8x5")
 
@@ -256,21 +256,21 @@
 
     This script will plot a dot in the dot plot in the corresponding location
     the plots are one contig/scaffold per plot.
     """
     from more_itertools import grouper
 
     p = OptionParser(scaffold.__doc__)
-    p.add_option(
+    p.add_argument(
         "--cutoff",
-        type="int",
+        type=int,
         default=1000000,
         help="Plot scaffolds with size larger than",
     )
-    p.add_option(
+    p.add_argument(
         "--highlights",
         help="A set of regions in BED format to highlight",
     )
     opts, args, iopts = p.set_image_options(args, figsize="14x8", dpi=150)
 
     if len(args) < 4 or len(args) % 3 != 1:
         sys.exit(not p.print_help())
@@ -281,15 +281,15 @@
     trios = [(a, Sizes(b), Bed(c)) for a, b, c in trios]
     if highlights:
         hlbed = Bed(highlights)
 
     for scaffoldID, scafsize in scafsizes.iter_sizes():
         if scafsize < opts.cutoff:
             continue
-        logging.debug("Loading {0} (size={1})".format(scaffoldID, thousands(scafsize)))
+        logger.debug("Loading {0} (size={1})".format(scaffoldID, thousands(scafsize)))
 
         tmpname = scaffoldID + ".sizes"
         tmp = open(tmpname, "w")
         tmp.write("{0}\t{1}".format(scaffoldID, scafsize))
         tmp.close()
 
         tmpsizes = Sizes(tmpname)
@@ -446,31 +446,31 @@
 def A50(args):
     """
     %prog A50 contigs_A.fasta contigs_B.fasta ...
 
     Plots A50 graphics, see blog post (http://blog.malde.org/index.php/a50/)
     """
     p = OptionParser(A50.__doc__)
-    p.add_option(
+    p.add_argument(
         "--overwrite",
         default=False,
         action="store_true",
         help="overwrite .rplot file if exists",
     )
-    p.add_option(
+    p.add_argument(
         "--cutoff",
         default=0,
-        type="int",
+        type=int,
         dest="cutoff",
         help="use contigs above certain size",
     )
-    p.add_option(
+    p.add_argument(
         "--stepsize",
         default=10,
-        type="int",
+        type=int,
         dest="stepsize",
         help="stepsize for the distribution",
     )
     opts, args = p.parse_args(args)
 
     if not args:
         sys.exit(p.print_help())
@@ -493,18 +493,18 @@
 
             a50, l50, n50 = calculate_A50(ctgsizes, cutoff=opts.cutoff)
             cmin, cmax, cmean = min(ctgsizes), max(ctgsizes), np.mean(ctgsizes)
             csum, counts = np.sum(ctgsizes), len(ctgsizes)
             cmean = int(round(cmean))
             statsrows.append((fastafile, l50, n50, cmin, cmax, cmean, csum, counts))
 
-            logging.debug("`{0}` ctgsizes: {1}".format(fastafile, ctgsizes))
+            logger.debug("`{0}` ctgsizes: {1}".format(fastafile, ctgsizes))
 
             tag = "{0} (L50={1})".format(op.basename(fastafile).rsplit(".", 1)[0], l50)
-            logging.debug(tag)
+            logger.debug(tag)
 
             for i, s in zip(range(0, len(a50), stepsize), a50[::stepsize]):
                 print("\t".join((str(i), str(s / 1000000.0), tag)), file=fw)
         fw.close()
 
         table = loadtable(statsheader, statsrows)
         print(table, file=sys.stderr)
```

### Comparing `jcvi-1.4.6/jcvi/graphics/base.py` & `jcvi-1.4.7/jcvi/graphics/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -516,15 +516,15 @@
     ax.set_axis_off()
 
     savefig(outfile)
 
 
 def plot_heatmap(
     ax,
-    M: np.array,
+    M: np.ndarray,
     breaks: List[int],
     groups: List[Tuple[int, int, List[Tuple[int, str]], str]] = [],
     plot_breaks: bool = False,
     cmap: Optional[Union[str, Colormap]] = None,
     binsize: Optional[int] = None,
 ):
     """Plot heatmap illustrating the contact probabilities in Hi-C data.
```

### Comparing `jcvi-1.4.6/jcvi/graphics/blastplot.py` & `jcvi-1.4.7/jcvi/graphics/blastplot.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,25 +10,26 @@
 help to position names maker (e.g. genes) onto the dot plot. So depending on
 whether you are BLASTing raw sequences or makers, you need to place --sizes or
 --bed options.
 """
 
 import os.path as op
 import sys
-import logging
-import numpy as np
 
 from random import sample
 
-from jcvi.formats.base import is_number
-from jcvi.formats.blast import BlastLine
-from jcvi.formats.sizes import Sizes
-from jcvi.formats.bed import Bed, BedLine
-from jcvi.apps.base import OptionParser
-from jcvi.graphics.base import plt, Rectangle, set_human_base_axis, savefig
+import numpy as np
+
+from ..apps.base import OptionParser, logger
+from ..formats.base import is_number
+from ..formats.bed import Bed, BedLine
+from ..formats.blast import BlastLine
+from ..formats.sizes import Sizes
+
+from .base import Rectangle, plt, savefig, set_human_base_axis
 
 
 DotStyles = ("line", "circle", "dot")
 
 
 def rename_seqid(seqid):
     seqid = seqid.split("_")[-1]
@@ -96,18 +97,18 @@
         data.append(((qi, qj), (si, sj)))
 
     if sampleN:
         if len(data) > sampleN:
             data = sample(data, sampleN)
 
     if not data:
-        return logging.error("no blast data imported")
+        return logger.error("no blast data imported")
 
     xsize, ysize = qsizes.totalsize, ssizes.totalsize
-    logging.debug("xsize=%d ysize=%d" % (xsize, ysize))
+    logger.debug("xsize=%d ysize=%d" % (xsize, ysize))
 
     if style == "line":
         for a, b in data:
             ax.plot(a, b, "ro-", mfc="w", mec="r", ms=3)
     else:
         data = [(x[0], y[0]) for x, y in data]
         x, y = zip(*data)
@@ -121,15 +122,15 @@
     ylim = (ysize, 0)  # invert the y-axis
 
     xchr_labels, ychr_labels = [], []
     ignore = True  # tag to mark whether to plot chr name (skip small ones)
     ignore_size_x = ignore_size_y = 0
 
     # plot the chromosome breaks
-    logging.debug("xbreaks={0} ybreaks={1}".format(len(qsizes), len(ssizes)))
+    logger.debug("xbreaks={0} ybreaks={1}".format(len(qsizes), len(ssizes)))
     for seqid, beg, end in qsizes.get_breaks():
         ignore = abs(end - beg) < ignore_size_x
         if ignore:
             continue
         seqid = rename_seqid(seqid)
 
         xchr_labels.append((seqid, (beg + end) / 2, ignore))
@@ -229,54 +230,54 @@
 
 
 if __name__ == "__main__":
 
     from jcvi.formats.bed import sizes
 
     p = OptionParser(__doc__)
-    p.add_option("--qsizes", help="Path to two column qsizes file")
-    p.add_option("--ssizes", help="Path to two column ssizes file")
-    p.add_option("--qbed", help="Path to qbed")
-    p.add_option("--sbed", help="Path to sbed")
-    p.add_option(
+    p.add_argument("--qsizes", help="Path to two column qsizes file")
+    p.add_argument("--ssizes", help="Path to two column ssizes file")
+    p.add_argument("--qbed", help="Path to qbed")
+    p.add_argument("--sbed", help="Path to sbed")
+    p.add_argument(
         "--qselect",
         default=0,
-        type="int",
+        type=int,
         help="Minimum size of query contigs to select",
     )
-    p.add_option(
+    p.add_argument(
         "--sselect",
         default=0,
-        type="int",
+        type=int,
         help="Minimum size of subject contigs to select",
     )
-    p.add_option("--qh", help="Path to highlight bed for query")
-    p.add_option("--sh", help="Path to highlight bed for subject")
-    p.add_option(
+    p.add_argument("--qh", help="Path to highlight bed for query")
+    p.add_argument("--sh", help="Path to highlight bed for subject")
+    p.add_argument(
         "--dotstyle",
         default="dot",
         choices=DotStyles,
         help="Style of the dots",
     )
-    p.add_option(
+    p.add_argument(
         "--proportional",
         default=False,
         action="store_true",
         help="Make image width:height equal to seq ratio",
     )
-    p.add_option(
+    p.add_argument(
         "--stripNames",
         default=False,
         action="store_true",
         help="Remove trailing .? from gene names",
     )
-    p.add_option(
+    p.add_argument(
         "--nmax",
         default=None,
-        type="int",
+        type=int,
         help="Only plot maximum of N dots",
     )
     opts, args, iopts = p.set_image_options(figsize="8x8", style="dark", dpi=150)
 
     qsizes, ssizes = opts.qsizes, opts.ssizes
     qbed, sbed = opts.qbed, opts.sbed
     proportional = opts.proportional
```

### Comparing `jcvi-1.4.6/jcvi/graphics/chromosome.py` & `jcvi-1.4.7/jcvi/graphics/chromosome.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from math import ceil
 from typing import Optional, Tuple
 
 import numpy as np
 
 from natsort import natsorted
 
-from ..apps.base import OptionGroup, OptionParser, datafile, logger, sample_N
+from ..apps.base import OptionParser, datafile, logger, sample_N
 from ..formats.base import DictFile, get_number
 from ..formats.bed import Bed
 from ..formats.sizes import Sizes
 
 from .base import (
     CirclePolygon,
     Polygon,
@@ -423,58 +423,55 @@
 
     The extent of the chromosomes are given by --sizes, which contains
     chr<tab>size, one per line. If not specified, the extent of the chromosomes
     are assumed to be the end for the last feature, which might be an underestimate.
     """
 
     p = OptionParser(main.__doc__)
-    p.add_option(
+    p.add_argument(
         "--sizes", help="FASTA sizes file, which contains chr<tab>size, one per line"
     )
-    g = OptionGroup(p, "Display accessories")
-    g.add_option(
+    g = p.add_argument_group("Display accessories")
+    g.add_argument(
         "--title",
         help="title of the image",
     )
-    g.add_option(
+    g.add_argument(
         "--gauge",
         default=False,
         action="store_true",
         help="draw a gauge with size label",
     )
-    p.add_option_group(g)
 
-    g = OptionGroup(p, "HTML image map")
-    g.add_option(
+    g = p.add_argument_group("HTML image map")
+    g.add_argument(
         "--imagemap",
         default=False,
         action="store_true",
         help="generate an HTML image map associated with the image",
     )
-    g.add_option(
+    g.add_argument(
         "--winsize",
         default=50000,
-        type="int",
+        type=int,
         help="if drawing an imagemap, specify the window size (bases) of each map element ",
     )
-    p.add_option_group(g)
 
-    g = OptionGroup(p, "Color legend")
-    g.add_option(
+    g = p.add_argument_group(p, "Color legend")
+    g.add_argument(
         "--nolegend",
         dest="legend",
         default=True,
         action="store_false",
         help="Do not generate color legend",
     )
-    g.add_option(
-        "--mergedist", default=0, type="int", help="Merge regions closer than "
+    g.add_argument(
+        "--mergedist", default=0, type=int, help="Merge regions closer than "
     )
-    g.add_option("--empty", help="Write legend for unpainted region")
-    p.add_option_group(g)
+    g.add_argument("--empty", help="Write legend for unpainted region")
 
     opts, args, iopts = p.set_image_options(figsize="6x6", dpi=300)
 
     if len(args) not in (1, 2):
         sys.exit(p.print_help())
 
     bedfile = args[0]
```

### Comparing `jcvi-1.4.6/jcvi/graphics/coverage.py` & `jcvi-1.4.7/jcvi/graphics/coverage.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,45 +6,43 @@
 
 Read coverage histogram, similar to wiggle plot. Data contains all the track
 data in the form of tab-delimited (x, y) lists.
 """
 
 import os.path as op
 import sys
-import logging
 
 import numpy as np
 
-from jcvi.formats.sizes import Sizes
-from jcvi.graphics.base import (
-    plt,
-    savefig,
+from ..apps.base import OptionParser, glob, logger
+from ..formats.sizes import Sizes
+
+from .base import (
     Rectangle,
-    mb_formatter,
-    mb_float_formatter,
     adjust_spines,
     get_map,
+    mb_float_formatter,
+    mb_formatter,
+    plt,
+    savefig,
 )
-from jcvi.apps.base import OptionParser, glob
 
 
 class XYtrack(object):
     def __init__(self, ax, datafile, color=None, ymax=40):
         self.ax = ax
         self.xy = []
         fp = open(datafile)
         for row in fp:
             atoms = row.split()
             self.xy.append([int(atoms[0]), float(atoms[1])])
         fp.close()
 
         self.x, self.y = zip(*self.xy)
-        logging.debug(
-            "File `{0}` imported (records={1}).".format(datafile, len(self.x))
-        )
+        logger.debug("File `{0}` imported (records={1}).".format(datafile, len(self.x)))
         self.color = color or "k"
         self.ymax = ymax
 
     @property
     def mapping(self):
         return dict(zip(self.x, self.y))
 
@@ -52,15 +50,15 @@
         maxsize = int(maxsize)
         for pos in range(unit, maxsize + unit, unit):
             if pos in self.x:
                 continue
             self.xy.append([pos, 0])
         self.xy.sort()
         self.x, self.y = zip(*self.xy)
-        logging.debug("After interpolate: {0}".format(len(self.x)))
+        logger.debug("After interpolate: {0}".format(len(self.x)))
 
     def cap(self, ymax):
         self.xy = [[a, 0] if b > ymax else [a, b] for a, b in self.xy]
         self.x, self.y = zip(*self.xy)
 
     def draw(self):
         ax = self.ax
@@ -84,15 +82,15 @@
             start = int(start)
             end = int(end)
             if tag == "double":
                 self.highlight(mapping, start, end, color=rr, unit=unit)
             else:
                 self.highlight(mapping, start, end, color=gg, unit=unit)
             imported += 1
-        logging.debug("Imported {0} regions from file `{1}`.".format(imported, hlfile))
+        logger.debug("Imported {0} regions from file `{1}`.".format(imported, hlfile))
 
     def highlight(self, mapping, start, end, color="r", unit=10000, zorder=10):
         ax = self.ax
         x = range(start, end + unit, unit)
         y = [mapping[z] for z in x]
         # Mask the highlight region so that they don't appear in background
         for a in self.xy:
@@ -211,15 +209,15 @@
     gauge_ax.xaxis.set_major_formatter(formatter)
     gauge_ax.xaxis.set_ticks(np.arange(start + gauge_step, end, gauge_step))
     gauge_ax.yaxis.set_ticks([])
 
 
 def main():
     p = OptionParser(__doc__)
-    p.add_option("--order", help="The order to plot the tracks, comma-separated")
+    p.add_argument("--order", help="The order to plot the tracks, comma-separated")
     opts, args, iopts = p.set_image_options()
 
     if len(args) != 3:
         sys.exit(not p.print_help())
 
     chr, sizes, datadir = args
     order = opts.order
```

### Comparing `jcvi-1.4.6/jcvi/graphics/dotplot.py` & `jcvi-1.4.7/jcvi/graphics/dotplot.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,36 +23,36 @@
 Before running this script it is recommended to check/install
 TeX Live (http://www.tug.org/texlive/) and
 Ghostscript (http://www.ghostscript.com/)
 see more here: http://matplotlib.sourceforge.net/users/usetex.html
 """
 
 import os.path as op
-import sys
-import logging
 import string
+import sys
 
 from random import sample
 
-from jcvi.compara.synteny import batch_scan, check_beds, get_orientation
-from jcvi.utils.cbook import seqid_parse, thousands
-from jcvi.apps.base import OptionParser, need_update
-from jcvi.graphics.base import (
-    plt,
+from ..apps.base import OptionParser, logger, need_update
+from ..compara.base import AnchorFile
+from ..compara.synteny import batch_scan, check_beds, get_orientation
+from ..utils.cbook import seqid_parse, thousands
+
+from .base import (
     Rectangle,
-    set_human_axis,
-    savefig,
-    draw_cmap,
     TextHandler,
+    draw_cmap,
     latex,
     markup,
     normalize_axes,
+    plt,
+    savefig,
+    set_human_axis,
     set1,
 )
-from ..compara.base import AnchorFile
 
 
 class Palette(dict):
     def __init__(self, palettedict=None, palettefile=None):
         """Instantiate a palette to map from block_id to color
 
         Args:
@@ -73,20 +73,20 @@
             a = "".join(x for x in a if x in string.digits)
             a = int(a)
             self[a] = b
 
         self.categories = sorted(set(self.values()))
         self.colors = dict(zip(self.categories, pal))
 
-        logging.debug(
+        logger.debug(
             "Color info ({0} categories) imported for {1} blocks.".format(
                 len(self.colors), len(self)
             )
         )
-        logging.debug(str(self.colors))
+        logger.debug(str(self.colors))
 
         for k, v in self.items():  # Update from categories to colors
             self[k] = self.colors[v]
 
     @classmethod
     def from_block_orientation(
         cls, anchorfile, qbed, sbed, forward_color="#e7298a", reverse_color="#3690c0"
@@ -221,15 +221,15 @@
     return xlim, ylim
 
 
 def downsample(data, sample_number=10000):
     npairs = len(data)
     # Only show random subset
     if npairs > sample_number:
-        logging.debug(
+        logger.debug(
             "Showing a random subset of {0} data points (total {1}) "
             "for clarity.".format(sample_number, npairs)
         )
         data = sample(data, sample_number)
     return data
 
 
@@ -270,15 +270,15 @@
     gx, gy = markup(gx), markup(gy)
 
     qorder = qbed.order
     sorder = sbed.order
 
     data = []
     if cmap_text:
-        logging.debug("Capping values within [{0:.1f}, {1:.1f}]".format(vmin, vmax))
+        logger.debug("Capping values within [{0:.1f}, {1:.1f}]".format(vmin, vmax))
 
     block_id = 0
     block_color = "k"
     for row in fp:
         atoms = row.split()
         if row[0] == "#":
             block_id += 1
@@ -333,15 +333,15 @@
         clusters = batch_scan(data, qbed, sbed)
         draw_box(clusters, ax)
 
     if cmap_text:
         draw_cmap(root, cmap_text, vmin, vmax, cmap=cmap)
 
     xsize, ysize = len(qbed), len(sbed)
-    logging.debug("xsize=%d ysize=%d" % (xsize, ysize))
+    logger.debug("xsize=%d ysize=%d" % (xsize, ysize))
     qbreaks = qbed.get_breaks()
     sbreaks = sbed.get_breaks()
     xlim, _ = plot_breaks_and_labels(
         fig,
         root,
         ax,
         gx,
@@ -377,15 +377,15 @@
         title = "Inter-genomic comparison: {0} vs {1}".format(gx, gy)
         if is_self:
             title = "Intra-genomic comparison within {0}".format(gx)
             npairs /= 2
         title += " ({0} gene pairs)".format(thousands(npairs))
     root.set_title(title, x=0.5, y=0.96, color="k")
     if title:
-        logging.debug("Dot plot title: {}".format(title))
+        logger.debug("Dot plot title: {}".format(title))
     normalize_axes(root)
 
 
 def subset_bed(bed, seqids):
     from copy import deepcopy
 
     newbed = deepcopy(bed)
@@ -396,65 +396,65 @@
         newbed.append(b)
     return newbed
 
 
 def dotplot_main(args):
     p = OptionParser(__doc__)
     p.set_beds()
-    p.add_option(
+    p.add_argument(
         "--synteny",
         default=False,
         action="store_true",
         help="Run a fast synteny scan and display blocks",
     )
-    p.add_option("--cmaptext", help="Draw colormap box on the bottom-left corner")
-    p.add_option(
+    p.add_argument("--cmaptext", help="Draw colormap box on the bottom-left corner")
+    p.add_argument(
         "--vmin",
         dest="vmin",
-        type="float",
+        type=float,
         default=0,
         help="Minimum value in the colormap",
     )
-    p.add_option(
+    p.add_argument(
         "--vmax",
         dest="vmax",
-        type="float",
+        type=float,
         default=2,
         help="Maximum value in the colormap",
     )
-    p.add_option(
+    p.add_argument(
         "--nmax",
         dest="sample_number",
-        type="int",
+        type=int,
         default=10000,
         help="Maximum number of data points to plot",
     )
-    p.add_option(
+    p.add_argument(
         "--minfont",
-        type="int",
+        type=int,
         default=4,
         help="Do not render labels with size smaller than",
     )
-    p.add_option("--colormap", help="Two column file, block id to color mapping")
-    p.add_option(
+    p.add_argument("--colormap", help="Two column file, block id to color mapping")
+    p.add_argument(
         "--colororientation",
         action="store_true",
         default=False,
         help="Color the blocks based on orientation, similar to mummerplot",
     )
-    p.add_option(
+    p.add_argument(
         "--nosort",
         default=False,
         action="store_true",
         help="Do not sort the seqids along the axes",
     )
-    p.add_option(
+    p.add_argument(
         "--nosep", default=False, action="store_true", help="Do not add contig lines"
     )
-    p.add_option("--title", help="Title of the dot plot")
+    p.add_argument("--title", help="Title of the dot plot")
     p.set_dotplot_opts()
     p.set_outfile(outfile=None)
     opts, args, iopts = p.set_image_options(
         args, figsize="9x9", style="dark", dpi=90, cmap="copper"
     )
 
     if len(args) != 1:
@@ -471,15 +471,15 @@
     elif opts.colororientation:
         palette = Palette.from_block_orientation(anchorfile, qbed, sbed)
 
     cmaptext = opts.cmaptext
     if anchorfile.endswith(".ks"):
         from jcvi.apps.ks import KsFile
 
-        logging.debug("Anchors contain Ks values")
+        logger.debug("Anchors contain Ks values")
         cmaptext = cmaptext or "*Ks* values"
         anchorksfile = anchorfile + ".anchors"
         if need_update(anchorfile, anchorksfile):
             ksfile = KsFile(anchorfile)
             ksfile.print_to_anchors(anchorksfile)
         anchorfile = anchorksfile
```

### Comparing `jcvi-1.4.6/jcvi/graphics/glyph.py` & `jcvi-1.4.7/jcvi/graphics/glyph.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,30 +4,32 @@
 """
 Gradient gene features
 """
 
 import os.path as op
 import sys
 
-import numpy as np
 from random import choice, shuffle, random, randint
 
-from jcvi.apps.base import OptionParser, ActionDispatcher
-from jcvi.graphics.base import (
-    plt,
-    Rectangle,
+import numpy as np
+
+from ..apps.base import OptionParser, ActionDispatcher
+from ..utils.grouper import Grouper
+
+from .base import (
     CirclePolygon,
     Ellipse,
     FancyArrowPatch,
     Polygon,
+    Rectangle,
+    get_map,
+    plt,
     savefig,
     set3,
-    get_map,
 )
-from jcvi.utils.grouper import Grouper
 
 
 tstep = 0.05
 Timing = np.arange(0, 1 + tstep, tstep)
 arrowprops = dict(
     arrowstyle="fancy",
     fc="lightslategray",
@@ -597,18 +599,20 @@
     %prog gff *.gff
 
     Draw exons for genes based on gff files. Each gff file should contain only
     one gene, and only the "mRNA" and "CDS" feature will be drawn on the canvas.
     """
     align_choices = ("left", "center", "right")
     p = OptionParser(gff.__doc__)
-    p.add_option(
+    p.add_argument(
         "--align", default="left", choices=align_choices, help="Horizontal alignment"
     )
-    p.add_option("--noUTR", default=False, action="store_true", help="Do not plot UTRs")
+    p.add_argument(
+        "--noUTR", default=False, action="store_true", help="Do not plot UTRs"
+    )
     opts, args = p.parse_args(args)
 
     if len(args) < 1:
         sys.exit(not p.print_help())
 
     fig = plt.figure(1, (8, 5))
     root = fig.add_axes([0, 0, 1, 1])
```

### Comparing `jcvi-1.4.6/jcvi/graphics/grabseeds.py` & `jcvi-1.4.7/jcvi/graphics/grabseeds.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,37 +25,38 @@
 from skimage.filters import roberts, sobel
 from skimage.measure import find_contours, regionprops, label
 from skimage.morphology import disk, closing
 from skimage.segmentation import clear_border, watershed
 from wand.image import Image
 from webcolors import rgb_to_hex, normalize_integer_triplet
 
-from .base import (
-    Rectangle,
-    latex,
-    load_image,
-    normalize_axes,
-    plt,
-    savefig,
-    set_helvetica_axis,
-)
 from ..algorithms.formula import get_kmeans, reject_outliers
 from ..apps.base import (
-    OptionParser,
-    OptionGroup,
     ActionDispatcher,
+    OptionParser,
     datadir,
     logger,
     iglob,
     mkdir,
 )
 from ..formats.base import must_open
 from ..formats.pdf import cat
 from ..utils.webcolors import closest_color
 
+from .base import (
+    Rectangle,
+    latex,
+    load_image,
+    normalize_axes,
+    plt,
+    savefig,
+    set_helvetica_axis,
+)
+
+
 np.seterr(all="ignore")
 
 RGBTuple = Tuple[int, int, int]
 
 
 class Seed(object):
     """
@@ -264,95 +265,91 @@
     return jsonfile
 
 
 def add_seeds_options(p, args):
     """
     Add options to the OptionParser for seeds() and batchseeds() functions.
     """
-    g1 = OptionGroup(p, "Image manipulation")
-    g1.add_option("--rotate", default=0, type="int", help="Rotate degrees clockwise")
-    g1.add_option(
+    g1 = p.add_argument_group("Image manipulation")
+    g1.add_argument("--rotate", default=0, type=int, help="Rotate degrees clockwise")
+    g1.add_argument(
         "--rows", default=":", help="Crop rows e.g. `:800` from first 800 rows"
     )
-    g1.add_option(
+    g1.add_argument(
         "--cols", default=":", help="Crop cols e.g. `-800:` from last 800 cols"
     )
-    g1.add_option("--labelrows", help="Label rows e.g. `:800` from first 800 rows")
-    g1.add_option("--labelcols", help="Label cols e.g. `-800: from last 800 rows")
+    g1.add_argument("--labelrows", help="Label rows e.g. `:800` from first 800 rows")
+    g1.add_argument("--labelcols", help="Label cols e.g. `-800: from last 800 rows")
     valid_colors = ("red", "green", "blue", "purple", "yellow", "orange", "INVERSE")
-    g1.add_option(
+    g1.add_argument(
         "--changeBackground",
         default=0,
         choices=valid_colors,
         help="Changes background color",
     )
-    p.add_option_group(g1)
 
-    g2 = OptionGroup(p, "Object recognition")
-    g2.add_option(
+    g2 = p.add_argument_group("Object recognition")
+    g2.add_argument(
         "--minsize",
         default=0.05,
-        type="float",
+        type=float,
         help="Min percentage of object to image",
     )
-    g2.add_option(
-        "--maxsize", default=50, type="float", help="Max percentage of object to image"
+    g2.add_argument(
+        "--maxsize", default=50, type=float, help="Max percentage of object to image"
     )
-    g2.add_option(
-        "--count", default=100, type="int", help="Report max number of objects"
+    g2.add_argument(
+        "--count", default=100, type=int, help="Report max number of objects"
     )
-    g2.add_option(
+    g2.add_argument(
         "--watershed",
         default=False,
         action="store_true",
         help="Run watershed to segment touching objects",
     )
-    p.add_option_group(g2)
 
-    g3 = OptionGroup(p, "De-noise")
+    g3 = p.add_argument_group("De-noise")
     valid_filters = ("canny", "roberts", "sobel")
-    g3.add_option(
+    g3.add_argument(
         "--filter",
         default="canny",
         choices=valid_filters,
         help="Edge detection algorithm",
     )
-    g3.add_option(
+    g3.add_argument(
         "--sigma",
         default=1,
-        type="int",
+        type=int,
         help="Canny edge detection sigma, higher for noisy image",
     )
-    g3.add_option(
+    g3.add_argument(
         "--kernel",
         default=2,
-        type="int",
+        type=int,
         help="Edge closure, higher if the object edges are dull",
     )
-    g3.add_option(
-        "--border", default=5, type="int", help="Remove image border of certain pixels"
+    g3.add_argument(
+        "--border", default=5, type=int, help="Remove image border of certain pixels"
     )
-    p.add_option_group(g3)
 
-    g4 = OptionGroup(p, "Output")
-    g4.add_option("--calibrate", help="JSON file to correct distance and color")
-    g4.add_option(
+    g4 = p.add_argument_group("Output")
+    g4.add_argument("--calibrate", help="JSON file to correct distance and color")
+    g4.add_argument(
         "--edges",
         default=False,
         action="store_true",
         help="Visualize edges in middle PDF panel",
     )
-    g4.add_option(
+    g4.add_argument(
         "--outdir", default=".", help="Store intermediate images and PDF in folder"
     )
-    g4.add_option("--prefix", help="Output prefix")
-    g4.add_option(
+    g4.add_argument("--prefix", help="Output prefix")
+    g4.add_argument(
         "--noheader", default=False, action="store_true", help="Do not print header"
     )
-    p.add_option_group(g4)
     opts, args, iopts = p.set_image_options(args, figsize="12x6", style="white")
 
     return opts, args, iopts
 
 
 def batchseeds(args):
     """
```

### Comparing `jcvi-1.4.6/jcvi/graphics/heatmap.py` & `jcvi-1.4.7/jcvi/graphics/heatmap.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,19 +20,21 @@
 III	I9H/IRX9-L,IRX14
 IV	IRX7,GUX2
 """
 
 
 import sys
 
-import numpy as np
 from itertools import groupby
 
-from jcvi.graphics.base import mpl, plt, savefig
-from jcvi.apps.base import OptionParser
+import numpy as np
+
+from ..apps.base import OptionParser
+
+from .base import mpl, plt, savefig
 
 
 def parse_csv(csvfile, vmin=0, groups=False):
     import csv
 
     reader = csv.reader(open(csvfile))
     if groups:
@@ -58,22 +60,22 @@
     data = np.array(data)
 
     return groups, rows, cols, data
 
 
 def main():
     p = OptionParser(__doc__)
-    p.add_option(
+    p.add_argument(
         "--groups",
         default=False,
         action="store_true",
         help="The first row contains group info",
     )
-    p.add_option("--rowgroups", help="Row groupings")
-    p.add_option(
+    p.add_argument("--rowgroups", help="Row groupings")
+    p.add_argument(
         "--horizontalbar",
         default=False,
         action="store_true",
         help="Horizontal color bar [default: vertical]",
     )
     opts, args, iopts = p.set_image_options(figsize="8x8")
```

### Comparing `jcvi-1.4.6/jcvi/graphics/histogram.py` & `jcvi-1.4.7/jcvi/graphics/histogram.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 
 """
 Use R ggplot2 library to plot histogram, also contains an ASCII histogram (use
 --text) when invoking histogram().
 """
 import os.path as op
 import sys
-import logging
-
-import numpy as np
 
 from math import log, ceil
 from collections import defaultdict
 
-from jcvi.formats.base import DictFile
-from jcvi.graphics.base import asciiplot, quickplot
-from jcvi.apps.r import RTemplate
-from jcvi.apps.base import OptionParser
+import numpy as np
+
+from ..apps.base import OptionParser, logger
+from ..apps.r import RTemplate
+from ..formats.base import DictFile
+
+from .base import asciiplot, quickplot
 
 
 histogram_header = """
 library(ggplot2)
 vmin <- $vmin
 vmax <- $vmax
 data <- read.table('$numberfile', skip=$skip)
@@ -157,15 +157,15 @@
 
     return bin_edges, hist
 
 
 def texthistogram(numberfiles, vmin, vmax, title=None, bins=20, skip=0, col=0, base=0):
 
     for nf in numberfiles:
-        logging.debug("Import `{0}`.".format(nf))
+        logger.debug("Import `%s`.", nf)
         data, vmin, vmax = get_data(nf, vmin, vmax, skip=skip, col=col)
         if base:
             loghistogram(data, base=base, title=title)
         else:
             stem_leaf_plot(data, vmin, vmax, bins, title=title)
 
 
@@ -272,55 +272,55 @@
 
     Print histogram of the data files. The data files contain one number per
     line. If more than one file is inputted, the program will combine the
     histograms into the same plot.
     """
     allowed_format = ("emf", "eps", "pdf", "png", "ps", "raw", "rgba", "svg", "svgz")
     p = OptionParser(main.__doc__)
-    p.add_option("--skip", default=0, type="int", help="skip the first several lines")
-    p.add_option("--col", default=0, type="int", help="Get the n-th column")
+    p.add_argument("--skip", default=0, type=int, help="skip the first several lines")
+    p.add_argument("--col", default=0, type=int, help="Get the n-th column")
     p.set_histogram()
-    p.add_option(
+    p.add_argument(
         "--tags",
         dest="tags",
         default=None,
         help="tags for data if multiple input files, comma sep",
     )
-    p.add_option(
+    p.add_argument(
         "--ascii",
         default=False,
         action="store_true",
         help="print ASCII text stem-leaf plot",
     )
-    p.add_option(
+    p.add_argument(
         "--base",
         default="0",
         choices=("0", "2", "10"),
         help="use logarithm axis with base, 0 to disable",
     )
-    p.add_option(
+    p.add_argument(
         "--facet",
         default=False,
         action="store_true",
         help="place multiple histograms side-by-side",
     )
-    p.add_option("--fill", default="white", help="color of the bin")
-    p.add_option(
+    p.add_argument("--fill", default="white", help="color of the bin")
+    p.add_argument(
         "--format",
         default="pdf",
         choices=allowed_format,
         help="Generate image of format",
     )
-    p.add_option(
+    p.add_argument(
         "--quick",
         default=False,
         action="store_true",
         help="Use quick plot, assuming bins are already counted",
     )
-    p.add_option(
+    p.add_argument(
         "--noprintstats",
         default=False,
         action="store_true",
         help="Write basic stats when using --quick",
     )
     opts, args = p.parse_args()
```

### Comparing `jcvi-1.4.6/jcvi/graphics/karyotype.py` & `jcvi-1.4.7/jcvi/graphics/karyotype.py`

 * *Files 4% similar despite different names*

```diff
@@ -399,39 +399,39 @@
 
         self.tracks = tracks
         self.layout = layout
 
 
 def main():
     p = OptionParser(__doc__)
-    p.add_option(
+    p.add_argument(
         "--basepair",
         default=False,
         action="store_true",
         help="Use base pair position instead of gene rank",
     )
-    p.add_option(
+    p.add_argument(
         "--keep-chrlabels",
         default=False,
         action="store_true",
         help="Keep chromosome labels",
     )
-    p.add_option(
+    p.add_argument(
         "--nocircles",
         default=False,
         action="store_true",
         help="Do not plot chromosome circles",
     )
-    p.add_option(
+    p.add_argument(
         "--shadestyle",
         default="curve",
         choices=Shade.Styles,
         help="Style of syntenic wedges",
     )
-    p.add_option(
+    p.add_argument(
         "--chrstyle",
         default="auto",
         choices=Chromosome.Styles,
         help="Style of chromosome labels",
     )
     p.set_outfile("karyotype.pdf")
     opts, args, iopts = p.set_image_options(figsize="8x7")
```

### Comparing `jcvi-1.4.6/jcvi/graphics/landscape.py` & `jcvi-1.4.7/jcvi/graphics/landscape.py`

 * *Files 4% similar despite different names*

```diff
@@ -201,16 +201,16 @@
     https://github.com/brentp/mosdepth
     """
     import seaborn as sns
 
     sns.set_style("darkgrid")
 
     p = OptionParser(mosdepth.__doc__)
-    p.add_option("--maxdepth", default=100, type="int", help="Maximum depth to plot")
-    p.add_option(
+    p.add_argument("--maxdepth", default=100, type=int, help="Maximum depth to plot")
+    p.add_argument(
         "--logscale", default=False, action="store_true", help="Use log-scale on depth"
     )
     opts, args, iopts = p.set_image_options(args, style="dark", figsize="6x8")
 
     if len(args) != 2:
         sys.exit(p.print_help())
 
@@ -490,23 +490,23 @@
     given in the file. When --colormap is not set, every seqid will be drawn in
     black.
 
     Can take multiple BED files as input and then plot all of them in a
     composite figure.
     """
     p = OptionParser(depth.__doc__)
-    p.add_option(
+    p.add_argument(
         "--chrinfo", help="Comma-separated mappings between seqid, color, new_name"
     )
-    p.add_option(
+    p.add_argument(
         "--titleinfo",
         help="Comma-separated titles mappings between filename, title",
     )
-    p.add_option("--maxdepth", default=100, type="int", help="Maximum depth to show")
-    p.add_option(
+    p.add_argument("--maxdepth", default=100, type=int, help="Maximum depth to show")
+    p.add_argument(
         "--logscale", default=False, action="store_true", help="Use log-scale on depth"
     )
     opts, args, iopts = p.set_image_options(args, style="dark", figsize="14x4")
 
     if len(args) < 1:
         sys.exit(not p.print_help())
 
@@ -544,18 +544,18 @@
     savefig(image_name, dpi=iopts.dpi, iopts=iopts)
 
 
 def add_window_options(p):
     """
     Add options for window plotting.
     """
-    p.add_option("--window", default=500000, type="int", help="Size of window")
-    p.add_option("--shift", default=100000, type="int", help="Size of shift")
-    p.add_option("--subtract", help="Subtract bases from window")
-    p.add_option(
+    p.add_argument("--window", default=500000, type=int, help="Size of window")
+    p.add_argument("--shift", default=100000, type=int, help="Size of shift")
+    p.add_argument("--subtract", help="Subtract bases from window")
+    p.add_argument(
         "--nomerge", default=False, action="store_true", help="Do not merge features"
     )
 
 
 def check_window_options(opts):
     """
     Check the window options, and return the values.
@@ -582,15 +582,15 @@
     return [x + ".bed" for x in s] if not binned else [x for x in s]
 
 
 def linearray(binfile, chr, window, shift):
     mn = binfile.mapping[chr]
     m, _ = zip(*mn)
 
-    m = np.array(m, dtype="float")
+    m = np.array(m, dtype=float)
     w = window // shift
     m = moving_sum(m, window=w)
     return m
 
 
 def lineplot(ax, binfiles, nbins, chr, window, shift, color="br"):
     assert len(binfiles) <= 2, "A max of two line plots are supported"
@@ -637,24 +637,24 @@
     currently supported:
 
     --lines: traditional line plots, useful for plotting feature freq
     --bars: show where the extent of features are
     --altbars: similar to bars, yet in two alternating tracks, e.g. scaffolds
     """
     p = OptionParser(composite.__doc__)
-    p.add_option("--lines", help="Features to plot in lineplot")
-    p.add_option("--bars", help="Features to plot in bars")
-    p.add_option("--altbars", help="Features to plot in alt-bars")
-    p.add_option(
+    p.add_argument("--lines", help="Features to plot in lineplot")
+    p.add_argument("--bars", help="Features to plot in bars")
+    p.add_argument("--altbars", help="Features to plot in alt-bars")
+    p.add_argument(
         "--fatten",
         default=False,
         action="store_true",
         help="Help visualize certain narrow features",
     )
-    p.add_option(
+    p.add_argument(
         "--mode",
         default="span",
         choices=("span", "count", "score"),
         help="Accumulate feature based on",
     )
     add_window_options(p)
     opts, args, iopts = p.set_image_options(args, figsize="8x5")
@@ -750,30 +750,30 @@
 
     Combine multiple line plots in one vertical stack
     Inputs must be BED-formatted.
 
     --lines: traditional line plots, useful for plotting feature freq
     """
     p = OptionParser(multilineplot.__doc__)
-    p.add_option("--lines", help="Features to plot in lineplot")
-    p.add_option("--colors", help="List of colors matching number of input bed files")
-    p.add_option(
+    p.add_argument("--lines", help="Features to plot in lineplot")
+    p.add_argument("--colors", help="List of colors matching number of input bed files")
+    p.add_argument(
         "--mode",
         default="span",
         choices=("span", "count", "score"),
         help="Accumulate feature based on",
     )
-    p.add_option(
+    p.add_argument(
         "--binned",
         default=False,
         action="store_true",
         help="Specify whether the input is already binned; "
         + "if True, input files are considered to be binfiles",
     )
-    p.add_option("--ymax", type="int", help="Set Y-axis max")
+    p.add_argument("--ymax", type=int, help="Set Y-axis max")
     add_window_options(p)
     opts, args, iopts = p.set_image_options(args, figsize="8x5")
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     fastafile, chr = args
@@ -942,25 +942,25 @@
     """
     %prog heatmap fastafile chr1
 
     Combine stack plot with heatmap to show abundance of various tracks along
     given chromosome. Need to give multiple beds to --stacks and --heatmaps
     """
     p = OptionParser(heatmap.__doc__)
-    p.add_option(
+    p.add_argument(
         "--stacks",
         default="Exons,Introns,DNA_transposons,Retrotransposons",
         help="Features to plot in stackplot",
     )
-    p.add_option(
+    p.add_argument(
         "--heatmaps",
         default="Copia,Gypsy,hAT,Helitron,Introns,Exons",
         help="Features to plot in heatmaps",
     )
-    p.add_option("--meres", default=None, help="Extra centromere / telomere features")
+    p.add_argument("--meres", default=None, help="Extra centromere / telomere features")
     add_window_options(p)
     opts, args, iopts = p.set_image_options(args, figsize="8x5")
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     fastafile, chr = args
@@ -1054,16 +1054,16 @@
 def stackarray(binfile: BinFile, chr: str, window: int, shift: int):
     """
     Get stack array from binfile for the given chr.
     """
     mn = binfile.mapping[chr]
     m, n = zip(*mn)
 
-    m = np.array(m, dtype="float")
-    n = np.array(n, dtype="float")
+    m = np.array(m, dtype=float)
+    n = np.array(n, dtype=float)
 
     w = window // shift
     m = moving_sum(m, window=w)
     n = moving_sum(n, window=w)
     m /= n
 
     return m
@@ -1077,16 +1077,16 @@
     chr: str,
     window: int,
     shift: int,
 ):
     """
     Plot stackplot on the given axes, using data from binfiles.
     """
-    t = np.arange(nbins, dtype="float") + 0.5
-    m = np.zeros(nbins, dtype="float")
+    t = np.arange(nbins, dtype=float) + 0.5
+    m = np.zeros(nbins, dtype=float)
     zorders = range(10)[::-1]
     for binfile, p, z in zip(binfiles, palette, zorders):
         s = stackarray(binfile, chr, window, shift)
         m += s
         ax.fill_between(t, m, color=p, lw=0, zorder=z)
 
     ax.set_xlim(0, nbins)
@@ -1168,21 +1168,21 @@
     """
     %prog stack fastafile
 
     Create landscape plots that show the amounts of genic sequences, and repetitive
     sequences along the chromosomes.
     """
     p = OptionParser(stack.__doc__)
-    p.add_option("--top", default=10, type="int", help="Draw the first N chromosomes")
-    p.add_option(
+    p.add_argument("--top", default=10, type=int, help="Draw the first N chromosomes")
+    p.add_argument(
         "--stacks",
         default="Exons,Introns,DNA_transposons,Retrotransposons",
         help="Features to plot in stackplot",
     )
-    p.add_option("--switch", help="Change chr names based on two-column file")
+    p.add_argument("--switch", help="Change chr names based on two-column file")
     add_window_options(p)
     opts, args, iopts = p.set_image_options(args, figsize="8x8")
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (fastafile,) = args
```

### Comparing `jcvi-1.4.6/jcvi/graphics/mummerplot.py` & `jcvi-1.4.7/jcvi/graphics/mummerplot.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,59 +3,58 @@
 
 """
 Wrapper for mummerplot. Selecting a subset of queries and references to plot
 main features in the dot plot.
 """
 import os.path as op
 import sys
-import logging
 
-from jcvi.formats.coords import Coords, filter
-from jcvi.formats.sizes import Sizes
-from jcvi.formats.base import SetFile
-from jcvi.apps.base import OptionParser, sh
+from ..apps.base import OptionParser, logger, sh
+from ..formats.base import SetFile
+from ..formats.coords import Coords, filter
+from ..formats.sizes import Sizes
 
 
 def writeXfile(ids, sizes_dict, filename):
     fw = open(filename, "w")
     for q in ids:
         print("\t".join(str(x) for x in (q, sizes_dict[q], "+")), file=fw)
 
-    logging.debug("{0} ids written to `{1}`.".format(len(ids), filename))
+    logger.debug("%d ids written to `%s`.", len(ids), filename)
     fw.close()
 
 
 def main(args):
     """
     %prog deltafile
 
     Plot one query. Extract the references that have major matches to this
     query. Control "major" by option --refcov.
     """
     p = OptionParser(main.__doc__)
-    p.add_option("--refids", help="Use subset of contigs in the ref")
-    p.add_option(
+    p.add_argument("--refids", help="Use subset of contigs in the ref")
+    p.add_argument(
         "--refcov",
         default=0.01,
-        type="float",
+        type=float,
         help="Minimum reference coverage",
     )
-    p.add_option(
+    p.add_argument(
         "--all",
         default=False,
         action="store_true",
         help="Plot one pdf file per ref in refidsfile",
     )
-    p.add_option(
+    p.add_argument(
         "--color",
         default="similarity",
         choices=("similarity", "direction", "none"),
         help="Color the dots based on",
     )
-    p.add_option(
+    p.add_argument(
         "--nolayout",
         default=False,
         action="store_true",
         help="Do not rearrange contigs",
     )
     p.set_align(pctid=0, hitlen=0)
     opts, args = p.parse_args(args)
@@ -124,15 +123,15 @@
         if c.refcov < refcov:
             continue
         if c.ref not in refs:
             continue
         queries.add(c.query)
 
     if not queries or not refs:
-        logging.debug("Empty - {0} vs. {1}".format(queries, refs))
+        logger.debug("Empty - %s vs. %s", queries, refs)
         return None
 
     if not layout:
         queries = sorted(queries)
         refs = sorted(refs)
 
     writeXfile(queries, qsizes, Qfile)
```

### Comparing `jcvi-1.4.6/jcvi/graphics/synteny.py` & `jcvi-1.4.7/jcvi/graphics/synteny.py`

 * *Files 5% similar despite different names*

```diff
@@ -624,66 +624,66 @@
             zorder=2,
         )
         ax.text(xr, ytop + d / 2, "repeat", ha="center")
 
 
 def main():
     p = OptionParser(__doc__)
-    p.add_option("--switch", help="Rename the seqid with two-column file")
-    p.add_option("--tree", help="Display trees on the bottom of the figure")
-    p.add_option("--extra", help="Extra features in BED format")
-    p.add_option(
+    p.add_argument("--switch", help="Rename the seqid with two-column file")
+    p.add_argument("--tree", help="Display trees on the bottom of the figure")
+    p.add_argument("--extra", help="Extra features in BED format")
+    p.add_argument(
         "--genelabels",
         help='Show only these gene labels, separated by comma. Example: "At1g12340,At5g54690"',
     )
-    p.add_option(
+    p.add_argument(
         "--genelabelsize",
         default=0,
-        type="int",
+        type=int,
         help="Show gene labels at this font size, useful for debugging. "
         + "However, plot may appear visually crowded. "
         + "Reasonably good values are 2 to 6 [Default: disabled]",
     )
-    p.add_option(
+    p.add_argument(
         "--genelabelrotation",
         default=25,
-        type="int",
+        type=int,
         help="Rotate gene labels at this angle (anti-clockwise), useful for debugging. "
         + "[Default: 25]",
     )
-    p.add_option(
+    p.add_argument(
         "--scalebar",
         default=False,
         action="store_true",
         help="Add scale bar to the plot",
     )
-    p.add_option(
+    p.add_argument(
         "--glyphstyle",
         default="box",
         choices=Glyph.Styles,
         help="Style of feature glyphs",
     )
-    p.add_option(
+    p.add_argument(
         "--glyphcolor",
         default="orientation",
         choices=Glyph.Palette,
         help="Glyph coloring based on",
     )
-    p.add_option(
+    p.add_argument(
         "--shadestyle",
         default="curve",
         choices=Shade.Styles,
         help="Style of syntenic wedges",
     )
-    p.add_option(
+    p.add_argument(
         "--outputprefix",
         default="",
         help="Prefix for the output file",
     )
-    p.add_option(
+    p.add_argument(
         "--noprune",
         default=False,
         action="store_true",
         help="If set, do not exclude small features from annotation track (<1% of region)",
     )
     opts, args, iopts = p.set_image_options(figsize="8x7")
```

### Comparing `jcvi-1.4.6/jcvi/graphics/table.py` & `jcvi-1.4.7/jcvi/graphics/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 #
 # Created by Haibao Tang on 05/25/20
 # Copyright © 2020 Haibao Tang. All rights reserved.
 #
 import csv
 import sys
 
-from jcvi.apps.base import OptionParser
-from jcvi.graphics.base import (
+from ..apps.base import OptionParser
+
+from .base import (
     Rectangle,
+    load_image,
     markup,
     normalize_axes,
     plt,
     savefig,
-    load_image,
 )
 
 
 class CsvTable(list):
     def __init__(self, csvfile="table.csv"):
         super(CsvTable, self).__init__()
         with open(csvfile) as csvfile:
```

### Comparing `jcvi-1.4.6/jcvi/graphics/tree.py` & `jcvi-1.4.7/jcvi/graphics/tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
-import logging
 import sys
 
 from collections import defaultdict
 from itertools import groupby
 
 from ete3 import Tree
 
-from jcvi.apps.base import OptionParser, glob
-from jcvi.formats.base import LineFile
-from jcvi.formats.sizes import Sizes
-from jcvi.graphics.base import (
+from ..apps.base import OptionParser, glob, logger
+from ..formats.base import LineFile
+from ..formats.sizes import Sizes
+
+from .base import (
     FancyBboxPatch,
     Rectangle,
     linear_shade,
     markup,
     normalize_axes,
     plt,
     savefig,
     set3_n,
 )
-from jcvi.graphics.glyph import ExonGlyph, TextCircle, get_setups
+from .glyph import ExonGlyph, TextCircle, get_setups
 
 
 class LeafInfoLine:
     def __init__(self, row, delimiter=","):
         args = [x.strip() for x in row.split(delimiter)]
         self.name = args[0]
         self.color = args[1]
@@ -544,78 +544,80 @@
     %prog newicktree
 
     Plot Newick formatted tree. The gene structure can be plotted along if
     --gffdir is given. The gff file needs to be `genename.gff`. If --sizes is
     on, also show the number of amino acids.
     """
     p = OptionParser(main.__doc__)
-    p.add_option(
+    p.add_argument(
         "--outgroup",
         help="Outgroup for rerooting the tree. "
         + "Use comma to separate multiple taxa.",
     )
-    p.add_option(
+    p.add_argument(
         "--noreroot",
         default=False,
         action="store_true",
         help="Don't reroot the input tree",
     )
-    p.add_option(
-        "--rmargin", default=0.2, type="float", help="Set blank rmargin to the right"
+    p.add_argument(
+        "--rmargin", default=0.2, type=float, help="Set blank rmargin to the right"
+    )
+    p.add_argument(
+        "--gffdir", default=None, help="The directory that contain GFF files"
     )
-    p.add_option("--gffdir", default=None, help="The directory that contain GFF files")
-    p.add_option("--sizes", default=None, help="The FASTA file or the sizes file")
-    p.add_option("--SH", default=None, type="string", help="SH test p-value")
-
-    group = p.add_option_group("Node style")
-    group.add_option("--leafcolor", default="k", help="Font color for the OTUs")
-    group.add_option("--leaffont", default=12, help="Font size for the OTUs")
-    group.add_option(
+    p.add_argument("--sizes", default=None, help="The FASTA file or the sizes file")
+    p.add_argument("--SH", default=None, type=str, help="SH test p-value")
+
+    group = p.add_argument_group("Node style")
+    group.add_argument("--leafcolor", default="k", help="Font color for the OTUs")
+    group.add_argument("--leaffont", default=12, help="Font size for the OTUs")
+    group.add_argument(
         "--leafinfo", help="CSV file specifying the leaves: name,color,new_name"
     )
-    group.add_option(
+    group.add_argument(
         "--scutoff",
         default=0,
-        type="int",
+        type=int,
         help="cutoff for displaying node support, 0-100",
     )
-    group.add_option(
+    group.add_argument(
         "--no_support",
         dest="support",
         default=True,
         action="store_false",
         help="Do not print node support values",
     )
-    group.add_option(
+    group.add_argument(
         "--no_internal",
         dest="internal",
         default=True,
         action="store_false",
         help="Do not show internal nodes",
     )
 
-    group = p.add_option_group("Edge style")
-    group.add_option(
+    group = p.add_argument_group("Edge style")
+    group.add_argument(
         "--dashedoutgroup",
         default=False,
         action="store_true",
         help="Gray out the edges connecting outgroup and non-outgroup",
     )
 
-    group = p.add_option_group("Additional annotations")
-    group.add_option(
+    group = p.add_argument_group("Additional annotations")
+    group.add_argument(
         "--geoscale",
         default=False,
         action="store_true",
         help="Plot geological scale",
     )
-    group.add_option(
+    group.add_argument(
         "--wgdinfo", help="CSV specifying the position and style of WGD events"
     )
-    group.add_option(
+    group.add_argument(
         "--groups",
         help="Group names from top to bottom, to the right of the tree. "
         "Each distinct color in --leafinfo is considered part of the same group. "
         "Separate the names with comma, such as 'eudicots,,monocots,'. "
         "Empty names will be ignored for that specific group. ",
     )
 
@@ -635,15 +637,15 @@
         t = Tree(
             """(((Os02g0681100:0.1151,Sb04g031800:0.11220)1.0:0.0537,
         (Os04g0578800:0.04318,Sb06g026210:0.04798)-1.0:0.08870)1.0:0.06985,
         ((Os03g0124100:0.08845,Sb01g048930:0.09055)1.0:0.05332,
         (Os10g0534700:0.06592,Sb01g030630:0.04824)-1.0:0.07886):0.09389);"""
         )
     else:
-        logging.debug("Load tree file `{0}`".format(datafile))
+        logger.debug("Load tree file `%s`", datafile)
         t, hpd = parse_tree(datafile)
 
     pf = datafile.rsplit(".", 1)[0]
 
     fig = plt.figure(1, (iopts.w, iopts.h))
     root = fig.add_axes([0, 0, 1, 1])
```

### Comparing `jcvi-1.4.6/jcvi/graphics/wheel.py` & `jcvi-1.4.7/jcvi/graphics/wheel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 """
 Wheel plot that shows continuous data in radial axes.
 """
-import numpy as np
 import sys
 
 from math import degrees
 from collections import OrderedDict
 from itertools import groupby
 
-from jcvi.graphics.base import plt, savefig, normalize_axes
-from jcvi.apps.base import OptionParser, ActionDispatcher
+import numpy as np
+
+from ..apps.base import ActionDispatcher, OptionParser
+
+from .base import normalize_axes, plt, savefig
 
 
 def main():
 
     actions = (("wheel", "wheel plot that shows continuous data in radial axes"),)
     p = ActionDispatcher(actions)
     p.dispatch(globals())
@@ -69,15 +71,15 @@
 def wheel(args):
     """
     %prog wheel datafile.csv groups.csv
 
     Wheel plot that shows continous data in radial axes.
     """
     p = OptionParser(wheel.__doc__)
-    p.add_option(
+    p.add_argument(
         "--column",
         default="score",
         choices=("score", "percentile"),
         help="Which column to extract from `datafile.csv`",
     )
     opts, args, iopts = p.set_image_options(args, figsize="5x5", format="png")
```

### Comparing `jcvi-1.4.6/jcvi/projects/age.py` & `jcvi-1.4.7/jcvi/projects/age.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 """
 Scripts related to age prediction model.
 """
-import logging
 import json
 import os
 import os.path as op
 import sys
 
-import pandas as pd
 import numpy as np
+import pandas as pd
+import seaborn as sns
 
 from jinja2 import Template
-from jcvi.graphics.base import panel_labels, plt, savefig
-import seaborn as sns
-from jcvi.apps.base import OptionParser, ActionDispatcher, iglob
+
+from ..apps.base import ActionDispatcher, OptionParser, iglob, logger
+from ..graphics.base import panel_labels, plt, savefig
 
 
 def main():
 
     actions = (
         ("compile", "extract telomere length and ccn"),
         ("traits", "make HTML page that reports eye and skin color"),
@@ -152,15 +152,15 @@
             js["traits"]["eye-color"]["B"],
         )
         samples.append(js)
 
     template = Template(traits_template)
     fw = open("report.html", "w")
     print(template.render(samples=samples), file=fw)
-    logging.debug("Report written to `{}`".format(fw.name))
+    logger.debug("Report written to `{}`".format(fw.name))
     fw.close()
 
 
 def plot_fit_line(ax, x, y):
     from numpy.polynomial.polynomial import polyfit
 
     t = np.arange(100)
@@ -690,15 +690,15 @@
     df = pd.read_csv(combined, sep="\t", index_col=0)
     df["Sample name"] = np.array(df["Sample name"], dtype=np.str)
     gender = extract_trait(df, "Sample name", "hli_calc_gender")
     sameGenderMZ = list(filter_same_gender(MZ, gender))
     sameGenderDZ = list(filter_same_gender(DZ, gender))
 
     composite(df, sameGenderMZ, sameGenderDZ, size=(iopts.w, iopts.h))
-    logging.getLogger().setLevel(logging.CRITICAL)
+    logger.getLogger().setLevel(logger.CRITICAL)
     savefig("heritability.pdf")
 
 
 def compile(args):
     """
     %prog compile directory
```

### Comparing `jcvi-1.4.6/jcvi/projects/allmaps.py` & `jcvi-1.4.7/jcvi/projects/allmaps.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 
 """
 Scripts for the ALLMAPS manuscript
 """
 import sys
 import numpy as np
 
-from jcvi.assembly.allmaps import AGP, Map, GapEstimator, normalize_lms_axis, spearmanr
-from jcvi.formats.bed import Bed
-from jcvi.utils.cbook import percentage
-from jcvi.graphics.chromosome import HorizontalChromosome
-from jcvi.graphics.base import (
-    plt,
-    savefig,
+from ..apps.base import OptionParser, ActionDispatcher
+from ..assembly.allmaps import AGP, GapEstimator, Map, normalize_lms_axis, spearmanr
+from ..formats.bed import Bed
+from ..graphics.base import (
     latex,
     normalize_axes,
     panel_labels,
-    set2,
+    plt,
+    savefig,
     set_ticklabels_helvetica,
+    set2,
 )
-from jcvi.apps.base import OptionParser, ActionDispatcher
+from ..graphics.chromosome import HorizontalChromosome
+from ..utils.cbook import percentage
 
 
 def main():
 
     actions = (
         ("lms", "ALLMAPS cartoon to illustrate LMS metric"),
         ("estimategaps", "illustrate ALLMAPS gap estimation algorithm"),
```

### Comparing `jcvi-1.4.6/jcvi/projects/bites.py` & `jcvi-1.4.7/jcvi/projects/bites.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 Tang et al. (2012) Altered Patterns of Fractionation and Exon Deletions in
 Brassica rapa Support a Two-Step Model of Paleohexaploidy. Genetics.
 <http://www.genetics.org/content/190/4/1563.short>
 """
 from more_itertools import pairwise
 
-from jcvi.graphics.base import plt, Rectangle, Polygon, CirclePolygon, savefig
-from jcvi.graphics.glyph import RoundLabel, arrowprops, TextCircle
-from jcvi.graphics.chromosome import Chromosome
-from jcvi.apps.base import OptionParser, ActionDispatcher, fname
+from ..apps.base import ActionDispatcher, OptionParser, fname
+from ..graphics.base import CirclePolygon, Polygon, Rectangle, plt, savefig
+from ..graphics.chromosome import Chromosome
+from ..graphics.glyph import RoundLabel, TextCircle, arrowprops
 
 
 def main():
 
     actions = (
         ("excision", "show intra-chromosomal recombination"),
         ("bites", "show the bites calling pipeline"),
```

### Comparing `jcvi-1.4.6/jcvi/projects/ies.py` & `jcvi-1.4.7/jcvi/projects/ies.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,24 @@
 # -*- coding: UTF-8 -*-
 
 """
 Locate IES sequences within MIC genome of tetrahymena.
 """
 import os.path as op
 import sys
-import logging
 
 from collections import Counter
 from itertools import groupby
 
-from jcvi.algorithms.formula import outlier_cutoff
-from jcvi.formats.bed import Bed, sort, depth, some, mergeBed
-from jcvi.formats.base import must_open
-from jcvi.utils.range import Range, range_interleave, range_chain
-from jcvi.utils.cbook import percentage
-from jcvi.apps.base import OptionParser, ActionDispatcher, need_update, sh
+from ..algorithms.formula import outlier_cutoff
+from ..apps.base import ActionDispatcher, OptionParser, logger, need_update, sh
+from ..formats.base import must_open
+from ..formats.bed import Bed, depth, mergeBed, some, sort
+from ..utils.cbook import percentage
+from ..utils.range import Range, range_interleave, range_chain
 
 
 class EndPoint(object):
     def __init__(self, label):
         args = label.split("-")
         self.label = label
         self.leftright = args[0]
@@ -43,15 +42,15 @@
 def variation(args):
     """
     %prog variation P1.bed P2.bed F1.bed
 
     Associate IES in parents and progeny.
     """
     p = OptionParser(variation.__doc__)
-    p.add_option(
+    p.add_argument(
         "--diversity",
         choices=("breakpoint", "variant"),
         default="variant",
         help="Plot diversity",
     )
     opts, args, iopts = p.set_image_options(args, figsize="6x6")
 
@@ -193,18 +192,18 @@
 
     -----------|   |------------
         -------|   |--------
       ---------|   |----------
             (RE)   (LE)
     """
     p = OptionParser(insertionpairs.__doc__)
-    p.add_option(
+    p.add_argument(
         "--extend",
         default=10,
-        type="int",
+        type=int,
         help="Allow insertion sites to match up within distance",
     )
     p.set_outfile()
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
@@ -236,16 +235,16 @@
     """
     %prog insertion mic.mac.bed
 
     Find IES based on mapping MIC reads to MAC genome. Output a bedfile with
     'lesions' (stack of broken reads) in the MAC genome.
     """
     p = OptionParser(insertion.__doc__)
-    p.add_option(
-        "--mindepth", default=6, type="int", help="Minimum depth to call an insertion"
+    p.add_argument(
+        "--mindepth", default=6, type=int, help="Minimum depth to call an insertion"
     )
     p.set_outfile()
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
@@ -272,21 +271,21 @@
 def deletion(args):
     """
     %prog deletion [mac.mic.bam|mac.mic.bed] mic.gaps.bed
 
     Find IES based on mapping MAC reads to MIC genome.
     """
     p = OptionParser(deletion.__doc__)
-    p.add_option(
-        "--mindepth", default=3, type="int", help="Minimum depth to call a deletion"
+    p.add_argument(
+        "--mindepth", default=3, type=int, help="Minimum depth to call a deletion"
     )
-    p.add_option(
-        "--minspan", default=30, type="int", help="Minimum span to call a deletion"
+    p.add_argument(
+        "--minspan", default=30, type=int, help="Minimum span to call a deletion"
     )
-    p.add_option(
+    p.add_argument(
         "--split",
         default=False,
         action="store_true",
         help="Break at cigar N into separate parts",
     )
     p.set_tmpdir()
     opts, args = p.parse_args(args)
@@ -316,15 +315,15 @@
             sort([bedfile, "-u", "--accn", sort_tmpdir])
 
     # Find reads that contain multiple matches
     ibedfile = pf + ".d.bed"
     if need_update(sortedbedfile, ibedfile):
         bed = Bed(sortedbedfile, sorted=False)
         fw = open(ibedfile, "w")
-        logging.debug("Write deletions to `{0}`.".format(ibedfile))
+        logger.debug("Write deletions to `{0}`.".format(ibedfile))
         for accn, bb in groupby(bed, key=lambda x: x.accn):
             bb = list(bb)
             branges = [(x.seqid, x.start, x.end) for x in bb]
             iranges = range_interleave(branges)
             for seqid, start, end in iranges:
                 if end - start + 1 < opts.minspan:
                     continue
@@ -335,15 +334,15 @@
         fw.close()
 
     # Uniqify the insertions and count occurrences
     countbedfile = pf + ".uniq.bed"
     if need_update(ibedfile, countbedfile):
         bed = Bed(ibedfile)
         fw = open(countbedfile, "w")
-        logging.debug("Write counts to `{0}`.".format(countbedfile))
+        logger.debug("Write counts to `{0}`.".format(countbedfile))
         registry = Counter((x.seqid, x.start, x.end) for x in bed)
         ies_id = 1
         for (seqid, start, end), count in registry.items():
             ies_name = "{0:05d}-r{1}".format(ies_id, count)
             if count < opts.mindepth:
                 continue
             print("\t".join(str(x) for x in (seqid, start - 1, end, ies_name)), file=fw)
@@ -355,35 +354,33 @@
     depthbedfile = pf + ".depth.bed"
     if need_update((sortedbedfile, countbedfile), depthbedfile):
         depth([sortedbedfile, countbedfile, "--outfile={0}".format(depthbedfile)])
 
     validbedfile = pf + ".valid.bed"
     if need_update(depthbedfile, validbedfile):
         fw = open(validbedfile, "w")
-        logging.debug("Filter valid deletions to `{0}`.".format(validbedfile))
+        logger.debug("Filter valid deletions to `{0}`.".format(validbedfile))
         bed = Bed(depthbedfile)
         all_scores = [float(b.score) for b in bed]
         lb, ub = outlier_cutoff(all_scores)
-        logging.debug(
-            "Bounds for depths: LB={:.2f} (ignored)  UB={:.2f}".format(lb, ub)
-        )
+        logger.debug("Bounds for depths: LB={:.2f} (ignored)  UB={:.2f}".format(lb, ub))
         for b in bed:
             if float(b.score) > ub:
                 continue
             print(b, file=fw)
         fw.close()
 
     # Remove deletions that contain sequencing gaps on its flanks
     selectedbedfile = pf + ".selected.bed"
     if need_update(validbedfile, selectedbedfile):
         flanksbedfile = pf + ".flanks.bed"
         fw = open(flanksbedfile, "w")
         bed = Bed(validbedfile)
         flank = 100
-        logging.debug("Write deletion flanks to `{0}`.".format(flanksbedfile))
+        logger.debug("Write deletion flanks to `{0}`.".format(flanksbedfile))
         for b in bed:
             start, end = b.start, b.end
             b.start, b.end = start, min(start + flank - 1, end)
             print(b, file=fw)
             b.start, b.end = max(start, end - flank + 1), end
             print(b, file=fw)
         fw.close()
@@ -402,21 +399,21 @@
         )
 
     # Find best-scoring non-overlapping set
     iesbedfile = pf + ".ies.bed"
     if need_update(selectedbedfile, iesbedfile):
         bed = Bed(selectedbedfile)
         fw = open(iesbedfile, "w")
-        logging.debug("Write IES to `{0}`.".format(iesbedfile))
+        logger.debug("Write IES to `{0}`.".format(iesbedfile))
         branges = [
             Range(x.seqid, x.start, x.end, int(x.accn.rsplit("r")[-1]), i)
             for i, x in enumerate(bed)
         ]
         iranges, iscore = range_chain(branges)
-        logging.debug("Best chain score: {} ({} IES)".format(iscore, len(iranges)))
+        logger.debug("Best chain score: {} ({} IES)".format(iscore, len(iranges)))
         ies_id = 1
         for seqid, start, end, score, id in iranges:
             ies_name = "IES-{0:05d}-r{1}".format(ies_id, score)
             span = end - start + 1
             print(
                 "\t".join(str(x) for x in (seqid, start - 1, end, ies_name, span)),
                 file=fw,
```

### Comparing `jcvi-1.4.6/jcvi/projects/jcvi.py` & `jcvi-1.4.7/jcvi/projects/jcvi.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from ..apps.base import ActionDispatcher, OptionParser, logger
 from ..assembly.geneticmap import draw_geneticmap_heatmap
 from ..assembly.hic import draw_hic_heatmap
 from ..assembly.kmer import draw_ks_histogram
 from ..compara.pedigree import Pedigree, calculate_inbreeding
 from ..graphics.base import cm, load_image, normalize_axes, panel_labels, plt, savefig
 from ..graphics.chromosome import draw_chromosomes
-from ..graphics.landscape import draw_multi_depth, draw_heatmaps, draw_stacks
+from ..graphics.landscape import draw_heatmaps, draw_multi_depth, draw_stacks
 
 
 def diversity(args):
     """
     %prog diversity pedigree.ped VAR?_srtd.wgs.regions.bed.gz
 
     Plot diversity composite figure, including:
```

### Comparing `jcvi-1.4.6/jcvi/projects/misc.py` & `jcvi-1.4.7/jcvi/projects/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,22 @@
 
 """
 Functions in this script produce figures in various manuscripts.
 """
 
 import os.path as op
 import sys
-import logging
 
 import numpy as np
 
-from jcvi.graphics.base import Polygon, normalize_axes, panel_labels, plt, savefig
-from jcvi.graphics.glyph import GeneGlyph, RoundRect, TextCircle, DoubleSquare, plot_cap
-from jcvi.graphics.karyotype import Karyotype
-from jcvi.graphics.synteny import Synteny, draw_gene_legend
-from jcvi.apps.base import OptionParser, ActionDispatcher, fname
+from ..apps.base import ActionDispatcher, OptionParser, logger, fname
+from ..graphics.base import Polygon, normalize_axes, panel_labels, plt, savefig
+from ..graphics.glyph import DoubleSquare, GeneGlyph, RoundRect, TextCircle, plot_cap
+from ..graphics.karyotype import Karyotype
+from ..graphics.synteny import Synteny, draw_gene_legend
 
 
 def main():
 
     actions = (
         # Epoch paper (Woodhouse et al., 2012 Plant Cell)
         ("epoch", "show the methods used in epoch paper"),
@@ -65,15 +64,15 @@
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     (datafile, csvfile) = args
     outgroup = ["ginkgo"]
 
-    logging.debug("Load tree file `{0}`".format(datafile))
+    logger.debug("Load tree file `%s`", datafile)
     t, hpd = parse_tree(datafile)
 
     pf = datafile.rsplit(".", 1)[0]
 
     fig = plt.figure(1, (iopts.w, iopts.h))
     root = fig.add_axes((0, 0, 1, 1))
 
@@ -176,15 +175,15 @@
     savefig(image_name, dpi=iopts.dpi, iopts=iopts)
 
 
 def utricularia(args):
     from jcvi.graphics.synteny import main as synteny_main
 
     p = OptionParser(synteny_main.__doc__)
-    p.add_option("--switch", help="Rename the seqid with two-column file")
+    p.add_argument("--switch", help="Rename the seqid with two-column file")
     opts, args, iopts = p.set_image_options(args, figsize="8x7")
 
     if len(args) != 3:
         sys.exit(not p.print_help())
 
     datafile, bedfile, layoutfile = args
     switch = opts.switch
@@ -373,15 +372,15 @@
 def oropetium(args):
     """
     %prog oropetium mcscan.out all.bed layout switch.ids
 
     Build a composite figure that calls graphis.synteny.
     """
     p = OptionParser(oropetium.__doc__)
-    p.add_option("--extra", help="Extra features in BED format")
+    p.add_argument("--extra", help="Extra features in BED format")
     opts, args, iopts = p.set_image_options(args, figsize="9x6")
 
     if len(args) != 4:
         sys.exit(not p.print_help())
 
     datafile, bedfile, slayout, switch = args
     fig = plt.figure(1, (iopts.w, iopts.h))
@@ -489,16 +488,16 @@
 def amborella(args):
     """
     %prog amborella seqids karyotype.layout mcscan.out all.bed synteny.layout
 
     Build a composite figure that calls graphics.karyotype and graphics.synteny.
     """
     p = OptionParser(amborella.__doc__)
-    p.add_option("--tree", help="Display trees on the bottom of the figure")
-    p.add_option("--switch", help="Rename the seqid with two-column file")
+    p.add_argument("--tree", help="Display trees on the bottom of the figure")
+    p.add_argument("--switch", help="Rename the seqid with two-column file")
     opts, args, iopts = p.set_image_options(args, figsize="8x7")
 
     if len(args) != 5:
         sys.exit(not p.print_help())
 
     seqidsfile, klayout, datafile, bedfile, slayout = args
     switch = opts.switch
@@ -536,16 +535,16 @@
 def cotton(args):
     """
     %prog cotton seqids karyotype.layout mcscan.out all.bed synteny.layout
 
     Build a composite figure that calls graphics.karyotype and graphic.synteny.
     """
     p = OptionParser(cotton.__doc__)
-    p.add_option("--depthfile", help="Use depth info in this file")
-    p.add_option("--switch", help="Rename the seqid with two-column file")
+    p.add_argument("--depthfile", help="Use depth info in this file")
+    p.add_argument("--switch", help="Rename the seqid with two-column file")
     opts, args, iopts = p.set_image_options(args, figsize="8x7")
 
     if len(args) != 5:
         sys.exit(p.print_help())
 
     seqidsfile, klayout, datafile, bedfile, slayout = args
     switch = opts.switch
```

### Comparing `jcvi-1.4.6/jcvi/projects/napus.py` & `jcvi-1.4.7/jcvi/projects/napus.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,34 +2,33 @@
 # -*- coding: UTF-8 -*-
 
 """
 Scripts for the Brassica napus genome manuscript (Chalhoub et al. Science 2014).
 """
 import os.path as op
 import sys
-import logging
 
 import numpy as np
 
-from jcvi.graphics.base import (
-    plt,
+from ..apps.base import ActionDispatcher, OptionParser, logger
+from ..formats.base import LineFile
+from ..graphics.base import (
+    FancyArrowPatch,
     Rectangle,
-    savefig,
-    mpl,
     adjust_spines,
-    FancyArrowPatch,
+    mpl,
     normalize_axes,
     panel_labels,
+    plt,
+    savefig,
 )
-from jcvi.graphics.glyph import TextCircle
-from jcvi.graphics.karyotype import Karyotype
-from jcvi.graphics.synteny import Synteny
-from jcvi.graphics.coverage import Coverage, Sizes, XYtrack, setup_gauge_ax
-from jcvi.formats.base import LineFile
-from jcvi.apps.base import OptionParser, ActionDispatcher
+from ..graphics.coverage import Coverage, Sizes, XYtrack, setup_gauge_ax
+from ..graphics.glyph import TextCircle
+from ..graphics.karyotype import Karyotype
+from ..graphics.synteny import Synteny
 
 
 template_cov = """# y, xstart, xend, rotation, color, label, va, bed
 .56, {0}, {1}, 0, darkslategray, , top, AN.bed
 .48, {2}, {3}, 0, darkslategray, , top, CN.bed
 # edges
 e, 0, 1, AN.CN.1x1.lifted.simple
@@ -100,54 +99,54 @@
 
 
 def make_seqids(chrs, seqidsfile="seqids"):
     fw = open(seqidsfile, "w")
     for chr in chrs:
         print(",".join(chr), file=fw)
     fw.close()
-    logging.debug("File `{0}` written.".format(seqidsfile))
+    logger.debug("File `{0}` written.".format(seqidsfile))
     return seqidsfile
 
 
 def make_layout(chrs, chr_sizes, ratio, template, klayout="layout", shift=0):
     coords = []
     for chr, chr_size in zip(chrs, chr_sizes):
         coords.extend(center_panel(chr, chr_size, ratio, shift=shift))
 
     fw = open(klayout, "w")
     print(template.format(*coords), file=fw)
     fw.close()
-    logging.debug("File `{0}` written.".format(klayout))
+    logger.debug("File `{0}` written.".format(klayout))
 
     return klayout
 
 
 def cov(args):
     """
     %prog cov chrA01 chrC01 chr.sizes data AN.CN.1x1.lifted.anchors.simple
 
     Plot coverage graphs between homeologs, the middle panel show the
     homeologous gene pairs. Allow multiple chromosomes to multiple chromosomes.
     """
     p = OptionParser(cov.__doc__)
-    p.add_option(
+    p.add_argument(
         "--order",
         default="swede,kale,h165,yudal,aviso,abu,bristol,bzh",
         help="The order to plot the tracks, comma-separated",
     )
-    p.add_option(
+    p.add_argument(
         "--reverse",
         default=False,
         action="store_true",
         help="Plot the order in reverse",
     )
-    p.add_option(
-        "--gauge_step", default=5000000, type="int", help="Step size for the base scale"
+    p.add_argument(
+        "--gauge_step", default=5000000, type=int, help="Step size for the base scale"
     )
-    p.add_option(
+    p.add_argument(
         "--hlsuffix",
         default="regions.forhaibao",
         help="Suffix for the filename to be used to highlight regions",
     )
     opts, args, iopts = p.set_image_options(args, figsize="11x8")
 
     if len(args) != 4:
@@ -254,17 +253,17 @@
         gid = atoms[col].rsplit(".", 1)[0]
         gid = gid.replace("T", "G")
         ids.append(gid)
 
     beds = [order[x][1] for x in ids if x in order]
     pts = [x.start for x in beds if x.seqid == label]
     if len(pts):
-        logging.debug("A total of {0} converted loci imported.".format(len(pts)))
+        logger.debug("A total of {0} converted loci imported.".format(len(pts)))
     else:
-        logging.error("Array empty. Skipped scatterplot.")
+        logger.error("Array empty. Skipped scatterplot.")
         return
 
     ax.vlines(pts, [-1], [ypos], color=color)
     ax.set_axis_off()
 
 
 def make_affix_axis(fig, t, yoffset, height=0.001):
@@ -280,18 +279,18 @@
 
     Napus Figure 3 displays alignments between quartet chromosomes, inset
     with read histograms.
     """
     from jcvi.formats.bed import Bed
 
     p = OptionParser(fig3.__doc__)
-    p.add_option(
+    p.add_argument(
         "--gauge_step",
         default=10000000,
-        type="int",
+        type=int,
         help="Step size for the base scale",
     )
     opts, args, iopts = p.set_image_options(args, figsize="12x9")
 
     if len(args) != 4:
         sys.exit(not p.print_help())
 
@@ -529,16 +528,16 @@
     """
     %prog fig4 layout data
 
     Napus Figure 4A displays an example deleted region for quartet chromosomes,
     showing read alignments from high GL and low GL lines.
     """
     p = OptionParser(fig4.__doc__)
-    p.add_option(
-        "--gauge_step", default=200000, type="int", help="Step size for the base scale"
+    p.add_argument(
+        "--gauge_step", default=200000, type=int, help="Step size for the base scale"
     )
     opts, args, iopts = p.set_image_options(args, figsize="9x7")
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     layout, datadir = args
```

### Comparing `jcvi-1.4.6/jcvi/projects/pineapple.py` & `jcvi-1.4.7/jcvi/projects/pineapple.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 """
 Scripts for the pineapple genome paper.
 """
 import sys
-import logging
 
-from jcvi.formats.base import DictFile, LineFile, SetFile, must_open, get_number
-from jcvi.formats.bed import Bed
-from jcvi.formats.sizes import Sizes
-from jcvi.graphics.base import Rectangle, panel_labels, plt, savefig
-from jcvi.graphics.chromosome import Chromosome
-from jcvi.graphics.karyotype import Karyotype
-from jcvi.graphics.synteny import Synteny, draw_gene_legend
-from jcvi.graphics.glyph import TextCircle
-from jcvi.annotation.ahrd import read_interpro
-from jcvi.apps.base import OptionParser, ActionDispatcher
+from ..annotation.ahrd import read_interpro
+from ..apps.base import ActionDispatcher, OptionParser, logger
+from ..formats.base import DictFile, LineFile, SetFile, get_number, must_open
+from ..formats.bed import Bed
+from ..formats.sizes import Sizes
+from ..graphics.base import Rectangle, panel_labels, plt, savefig
+from ..graphics.chromosome import Chromosome
+from ..graphics.glyph import TextCircle
+from ..graphics.karyotype import Karyotype
+from ..graphics.synteny import Synteny, draw_gene_legend
 
 
 class RegionsLine(object):
     def __init__(self, line):
         args = line.split()
         self.karyotype = args[0][0]
         self.group = args[0][1]
@@ -67,15 +66,15 @@
 def flanking(args):
     """
     %prog flanking SI.ids liftover.bed master.txt master-removed.txt
 
     Extract flanking genes for given SI loci.
     """
     p = OptionParser(flanking.__doc__)
-    p.add_option("-N", default=50, type="int", help="How many genes on both directions")
+    p.add_argument("-N", default=50, type=int, help="How many genes on both directions")
     opts, args = p.parse_args(args)
 
     if len(args) != 4:
         sys.exit(not p.print_help())
 
     SI, liftover, master, te = args
     N = opts.N
@@ -296,15 +295,15 @@
     %prog ploidy seqids karyotype.layout mcscan.out all.bed synteny.layout
 
     Build a figure that calls graphics.karyotype to illustrate the high ploidy
     of WGD history of pineapple genome. The script calls both graphics.karyotype
     and graphic.synteny.
     """
     p = OptionParser(ploidy.__doc__)
-    p.add_option("--switch", help="Rename the seqid with two-column file")
+    p.add_argument("--switch", help="Rename the seqid with two-column file")
     opts, args, iopts = p.set_image_options(args, figsize="9x7")
 
     if len(args) != 5:
         sys.exit(not p.print_help())
 
     seqidsfile, klayout, datafile, bedfile, slayout = args
 
@@ -391,15 +390,15 @@
         atoms = row.strip().split("\t")
         if len(atoms) == 3:
             continue
         old, new, tag, start, end = atoms
         old = scaffold + old
         start, end = int(start), int(end)
         if start >= end:
-            logging.warning("{0} {1} >= {2}".format(old, start, end))
+            logger.warning("%s %d >= %d", old, start, end)
             start, end = end, start
         print("\t".join(str(x) for x in (old, start - 1, end)))
         nbreaks += 1
         scaffolds.add(old)
     print(
         "{0} breakpoints in total, {1} scaffolds broken".format(
             nbreaks, len(scaffolds)
```

### Comparing `jcvi-1.4.6/jcvi/projects/str.py` & `jcvi-1.4.7/jcvi/projects/str.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,51 +4,51 @@
 """
 Related scripts for the HLI-STR (TREDPARSE) paper.
 """
 import os.path as op
 import os
 import csv
 import sys
-import logging
 import json
 import numpy as np
 import pandas as pd
 
 from collections import defaultdict
+from itertools import product
 from random import sample
-from pyfaidx import Fasta
+
 from Bio import SeqIO
 from Bio.Seq import Seq
 from Bio.SeqRecord import SeqRecord
-from itertools import product
 from natsort import natsorted
+from pyfaidx import Fasta
 
 try:
     import vcf
 except ImportError:
     pass
 
-from jcvi.graphics.base import (
+from ..apps.base import ActionDispatcher, OptionParser, cleanup, iglob, logger, mkdir
+from ..apps.base import datafile, sh
+from ..apps.bwa import align
+from ..apps.grid import Parallel
+from ..assembly.sim import eagle, wgsim
+from ..formats.base import is_number, must_open
+from ..formats.sam import get_minibam_bed, index
+from ..graphics.base import (
     FancyArrow,
     normalize_axes,
     panel_labels,
     plt,
     savefig,
     set_helvetica_axis,
 )
-from jcvi.formats.base import is_number, must_open
-from jcvi.formats.sam import get_minibam_bed, index
-from jcvi.variation.str import TREDsRepo, af_to_counts, read_treds
-from jcvi.utils.cbook import percentage
-from jcvi.utils.table import tabulate
-from jcvi.apps.grid import Parallel
-from jcvi.apps.bwa import align
-from jcvi.apps.base import datafile, sh
-from jcvi.assembly.sim import eagle, wgsim
-from jcvi.apps.base import ActionDispatcher, OptionParser, cleanup, iglob, mkdir
+from ..utils.cbook import percentage
+from ..utils.table import tabulate
+from ..variation.str import TREDsRepo, af_to_counts, read_treds
 
 
 # Huntington risk allele
 infected_thr = 40
 ref_thr = 19
 SIMULATED_HAPLOID = r"Simulated haploid $\mathit{h}$"
 SIMULATED_DIPLOID = r"Simulated diploid $\mathit{20/h}$"
@@ -229,15 +229,15 @@
     ymin = -0.2
     df = pd.read_csv(csvfile)
     data = []
     for i, d in df.iterrows():
         tred = d["Name"]
         motif = d["Motif"]
         if tred in ignore:
-            logging.debug("Ignore {}".format(d["TRED"]))
+            logger.debug("Ignore {}".format(d["TRED"]))
             continue
 
         if len(motif) > 6:
             if "/" in motif:  # CTG/CAG
                 motif = motif.split("/")[0]
             else:
                 motif = motif[:6] + ".."
@@ -279,15 +279,15 @@
         XC_kinship_TRIO_annotationed_age_sex_PaternalMaternalAgeWhenChildWasBorn.txt
         hli.20170805.tsv
 
     Second iteration of Mendelian error calculation. This includes all the read
     counts and gender information to correct error estimate of X-linked loci.
     """
     p = OptionParser(mendelian2.__doc__)
-    p.add_option(
+    p.add_argument(
         "--treds", default=None, help="Extract specific treds, use comma to separate"
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
@@ -336,15 +336,15 @@
                 calls = row[tred + ".calls"]
                 fdp = int(row[tred + ".FDP"])
                 pdp = int(row[tred + ".PDP"])
                 rdp = int(row[tred + ".RDP"])
                 pedp = int(row[tred + ".PEDP"])
                 td[s] = [str(x) for x in (inferredGender, calls, fdp, pdp, rdp, pedp)]
             except ValueError:
-                logging.error("Invalid row: {}".format(row))
+                logger.error("Invalid row: {}".format(row))
                 continue
 
         h = " ".join((header.format("P1"), header.format("P2"), header.format("Kid")))
         print("\t".join(["MendelianError"] + h.split()), file=fw)
         tredcall = lambda x: td.get(x, ["", "-1|-1", "", "", "", ""])[:]
         counts = defaultdict(int)
         is_xlinked = repo[tred].is_xlinked
@@ -518,15 +518,15 @@
                     alt_points.add((fname, fstart))
                     altreads += 1
                 if (not r_in_region) and f_in_region:
                     alt_points.add((rname, rstart))
                     altreads += 1
                 nreads += 1
 
-            logging.debug(
+            logger.debug(
                 "A total of {} reads ({} alts) processed".format(nreads, altreads)
             )
             alt_points = natsorted(alt_points)
 
             # Chain these points together into regions
             g = Grouper()
             for a in alt_points:
@@ -559,15 +559,15 @@
                 ]
             )
             ref_regions.append(regions)
 
         line = ",".join([tred] + ref_regions)
         print(line, file=sys.stderr)
         print(line, file=fw)
-        logging.debug("Alternative region sum: {} bp".format(alt_sum))
+        logger.debug("Alternative region sum: {} bp".format(alt_sum))
 
     fw.close()
 
 
 def depth(args):
     """
     %prog depth DP.tsv
@@ -592,21 +592,21 @@
 
     ids, treds = read_treds()
     for dp, ax, title in zip(
         ("FDP", "PDP", "RDP", "PEDP"),
         (ax1, ax2, ax3, ax4),
         ("Spanning reads", "Partial reads", "Repeat-only reads", "Paired-end reads"),
     ):
-        logging.debug("Build {}".format(title))
+        logger.debug("Build {}".format(title))
         # Construct related data structure
         xd = []  # (tred, dp)
         mdp = []  # (tred, median_dp)
         for tred, motif in zip(treds["abbreviation"], treds["motif"]):
             if tred in ignore:
-                logging.debug("Ignore {}".format(tred))
+                logger.debug("Ignore {}".format(tred))
                 continue
             if len(motif) > 4:
                 if "/" in motif:  # CTG/CAG
                     motif = motif.split("/")[0]
                 else:
                     motif = motif[:4] + ".."
             xtred = "{} {}".format(tred, motif)
@@ -677,15 +677,15 @@
     root = fig.add_axes([0, 0, 1, 1])
 
     ymin = -0.2
     df = pd.read_csv(csvfile)
     data = []
     for i, d in df.iterrows():
         if d["TRED"].split()[0] in ignore:
-            logging.debug("Ignore {}".format(d["TRED"]))
+            logger.debug("Ignore {}".format(d["TRED"]))
             continue
         data.append(d)
     treds, duos, trios = zip(*data)
     ntreds = len(treds)
     ticks = range(ntreds)
     treds = [x.split()[0] for x in treds]
     duos = [float(x.rstrip("%")) for x in duos]
@@ -760,15 +760,15 @@
 def mendelian(args):
     """
     %prog mendelian trios_candidate.json hli.20170424.tred.tsv
 
     Calculate Mendelian errors based on trios and duos.
     """
     p = OptionParser(mendelian.__doc__)
-    p.add_option("--tolerance", default=0, type="int", help="Tolernace for differences")
+    p.add_argument("--tolerance", default=0, type=int, help="Tolernace for differences")
     p.set_verbose()
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     triosjson, tredtsv = args
@@ -880,33 +880,33 @@
 def mini(args):
     """
     %prog mini bamfile minibamfile
 
     Prepare mini-BAMs that contain only the STR loci.
     """
     p = OptionParser(mini.__doc__)
-    p.add_option(
-        "--pad", default=20000, type="int", help="Add padding to the STR reigons"
+    p.add_argument(
+        "--pad", default=20000, type=int, help="Add padding to the STR reigons"
     )
-    p.add_option(
+    p.add_argument(
         "--treds", default=None, help="Extract specific treds, use comma to separate"
     )
     p.set_outfile()
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     bamfile, minibam = args
     treds = opts.treds.split(",") if opts.treds else None
     pad = opts.pad
     bedfile = make_STR_bed(pad=pad, treds=treds)
 
     get_minibam_bed(bamfile, bedfile, minibam)
-    logging.debug("Mini-BAM written to `{}`".format(minibam))
+    logger.debug("Mini-BAM written to `{}`".format(minibam))
 
 
 def parse_log(logfile):
     fp = open(logfile)
     likelihood = {}
     for row in fp:
         if row.startswith("DEBUG:IntegratedCaller:***"):
@@ -1424,32 +1424,32 @@
         sh("mv allelefreq.pdf {}".format(outpdf))
         pdfs.append(outpdf)
 
     from jcvi.formats.pdf import cat
 
     pf = op.basename(reportfile).split(".")[0]
     finalpdf = pf + ".allelefreq.pdf"
-    logging.debug("Merging pdfs into `{}`".format(finalpdf))
+    logger.debug("Merging pdfs into `{}`".format(finalpdf))
     cat(pdfs + ["-o", finalpdf, "--cleanup"])
 
 
 def allelefreq(args):
     """
     %prog allelefreq HD,DM1,SCA1,SCA17,FXTAS,FRAXE
 
     Plot the allele frequencies of some STRs.
     """
     p = OptionParser(allelefreq.__doc__)
-    p.add_option(
+    p.add_argument(
         "--nopanels",
         default=False,
         action="store_true",
         help="No panel labels A, B, ...",
     )
-    p.add_option("--usereport", help="Use allele frequency in report file")
+    p.add_argument("--usereport", help="Use allele frequency in report file")
     opts, args, iopts = p.set_image_options(args, figsize="9x13")
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (loci,) = args
     fig, ((ax1, ax2), (ax3, ax4), (ax5, ax6)) = plt.subplots(
@@ -1496,43 +1496,43 @@
     rec = SeqRecord(Seq(seq), description="", id=id)
     fw = open(fastafile, "w")
     SeqIO.write([rec], fw, "fasta")
     fw.close()
 
 
 def add_simulate_options(p):
-    p.add_option("--readlen", default=150, type="int", help="Length of the read")
-    p.add_option(
+    p.add_argument("--readlen", default=150, type=int, help="Length of the read")
+    p.add_argument(
         "--distance",
         default=500,
-        type="int",
+        type=int,
         help="Outer distance between the two ends",
     )
     p.set_depth(depth=20)
 
 
 def simulate(args):
     """
     %prog simulate run_dir 1 300
 
     Simulate BAMs with varying inserts with dwgsim. The above command will
     simulate between 1 to 300 CAGs in the HD region, in a directory called
     `run_dir`.
     """
     p = OptionParser(simulate.__doc__)
-    p.add_option(
+    p.add_argument(
         "--method", choices=("wgsim", "eagle"), default="eagle", help="Read simulator"
     )
-    p.add_option(
+    p.add_argument(
         "--ref",
         default="hg38",
         choices=("hg38", "hg19"),
         help="Reference genome version",
     )
-    p.add_option("--tred", default="HD", help="TRED locus")
+    p.add_argument("--tred", default="HD", help="TRED locus")
     add_simulate_options(p)
     opts, args = p.parse_args(args)
 
     if len(args) != 3:
         sys.exit(not p.print_help())
 
     rundir, startunits, endunits = args
@@ -1546,15 +1546,15 @@
 
     # TRED region (e.g. Huntington)
     pad_left, pad_right = 1000, 10000
     repo = TREDsRepo(ref=ref)
     tred = repo[opts.tred]
     chr, start, end = tred.chr, tred.repeat_start, tred.repeat_end
 
-    logging.debug("Simulating {}".format(tred))
+    logger.debug("Simulating {}".format(tred))
     fasta = Fasta(ref_fasta)
     seq_left = fasta[chr][start - pad_left : start - 1]
     seq_right = fasta[chr][end : end + pad_right]
     motif = tred.repeat
 
     simulate_method = wgsim if opts.method == "wgsim" else eagle
     # Write fake sequence
@@ -1607,15 +1607,15 @@
 
     if len(args) not in (2, 3):
         sys.exit(not p.print_help())
 
     if len(args) == 2:
         idir1, outdir = args
         dir1 = [idir1] if idir1.endswith(".bam") else iglob(idir1, "*.bam")
-        logging.debug("Homozygous mode")
+        logger.debug("Homozygous mode")
         dir2 = [""] * len(dir1)
     elif len(args) == 3:
         idir1, idir2, outdir = args
         dir1 = [idir1] if idir1.endswith(".bam") else iglob(idir1, "*.bam")
         dir2 = [idir2] if idir2.endswith(".bam") else iglob(idir2, "*.bam")
         assert len(dir2) == 1, "Second pile must contain a single bam"
         dir2 = [idir2] * len(dir1)
@@ -1638,15 +1638,15 @@
     """
     %prog batchlobstr bamlist
 
     Run lobSTR on a list of BAMs. The corresponding batch command for TREDPARSE:
     $ tred.py bamlist --haploid chr4 --workdir tredparse_results
     """
     p = OptionParser(batchlobstr.__doc__)
-    p.add_option(
+    p.add_argument(
         "--haploid", default="chrY,chrM", help="Use haploid model for these chromosomes"
     )
     p.set_cpus()
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
@@ -1699,15 +1699,15 @@
     %prog evidences
 
     Plot distribution of evidences against two factors:
     - Sample mean coverage
     - Longer allele
     """
     p = OptionParser(evidences.__doc__)
-    p.add_option(
+    p.add_argument(
         "--csv", default="hli.20170328.tred.tsv", help="TRED csv output to plot"
     )
     opts, args, iopts = p.set_image_options(args, format="pdf")
 
     if len(args) != 0:
         sys.exit(not p.print_help())
 
@@ -2040,16 +2040,16 @@
 def compare2(args):
     """
     %prog compare2
 
     Compare performances of various variant callers on simulated STR datasets.
     """
     p = OptionParser(compare2.__doc__)
-    p.add_option(
-        "--maxinsert", default=300, type="int", help="Maximum number of repeats"
+    p.add_argument(
+        "--maxinsert", default=300, type=int, help="Maximum number of repeats"
     )
     add_simulate_options(p)
     opts, args, iopts = p.set_image_options(args, figsize="10x5")
 
     if len(args) != 0:
         sys.exit(not p.print_help())
 
@@ -2097,16 +2097,16 @@
     """
     %prog power
 
     Compare performances of various variant callers on simulated STR datasets.
     This compares the power of various evidence types.
     """
     p = OptionParser(power.__doc__)
-    p.add_option(
-        "--maxinsert", default=300, type="int", help="Maximum number of repeats"
+    p.add_argument(
+        "--maxinsert", default=300, type=int, help="Maximum number of repeats"
     )
     add_simulate_options(p)
     opts, args, iopts = p.set_image_options(args, figsize="10x10", format="png")
 
     if len(args) != 0:
         sys.exit(not p.print_help())
 
@@ -2196,16 +2196,16 @@
     """
     %prog tredparse
 
     Compare performances of various variant callers on simulated STR datasets.
     Adds coverage comparisons as panel C and D.
     """
     p = OptionParser(tredparse.__doc__)
-    p.add_option(
-        "--maxinsert", default=300, type="int", help="Maximum number of repeats"
+    p.add_argument(
+        "--maxinsert", default=300, type=int, help="Maximum number of repeats"
     )
     add_simulate_options(p)
     opts, args, iopts = p.set_image_options(args, figsize="10x10")
 
     if len(args) != 0:
         sys.exit(not p.print_help())
```

### Comparing `jcvi-1.4.6/jcvi/projects/sugarcane.py` & `jcvi-1.4.7/jcvi/projects/sugarcane.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,33 +3,31 @@
 #
 # sugarcane.py
 # projects
 #
 # Created by Haibao Tang on 12/02/19
 # Copyright © 2019 Haibao Tang. All rights reserved.
 #
-import logging
 import os.path as op
 import sys
 
 from collections import Counter, defaultdict
-from glob import glob
 from itertools import combinations, groupby, product
 from random import random, sample
 from typing import Dict
 
 import numpy as np
 import matplotlib.pyplot as plt
 import seaborn as sns
 import pandas as pd
 
-from jcvi.apps.base import OptionParser, ActionDispatcher, mkdir
-from jcvi.graphics.base import adjust_spines, markup, normalize_axes, savefig
-from jcvi.utils.validator import validate_in_choices
+from ..apps.base import ActionDispatcher, OptionParser, logger, mkdir
 from ..formats.blast import Blast
+from ..graphics.base import adjust_spines, markup, normalize_axes, savefig
+from ..utils.validator import validate_in_choices
 
 SoColor = "#7436a4"  # Purple
 SsColor = "#5a8340"  # Green
 
 # Computed using prepare(), corrected with real sizes
 ChrSizes = {
     "SO-chr01": 148750011,
@@ -324,27 +322,27 @@
         percent_SO_data.append(percent_SO)
     # Avoid overlapping bars
     SS_counter, SO_counter = Counter(SS_data), Counter(SO_data)
     overlaps = SS_counter.keys() & SO_counter.keys()
     shift = 0.5  # used to offset bars a bit to avoid cluttering
     if overlaps:
         for overlap in overlaps:
-            logging.debug(f"Modify bar offsets at {overlap} due to SS and SO overlaps")
+            logger.debug(f"Modify bar offsets at {overlap} due to SS and SO overlaps")
             SS_counter[overlap - shift] = SS_counter[overlap]
             del SS_counter[overlap]
             SO_counter[overlap + shift] = SO_counter[overlap]
             del SO_counter[overlap]
 
     def modify_range_end(d: dict, value: int):
         if value not in d:
             return
         # Has data at the range end, but no adjacent data points (i.e. isolated bar)
         if value in d and (value - 1 in d or value + 1 in d):
             return
-        logging.debug(f"Modify bar offsets at {value} due to end of range ends")
+        logger.debug(f"Modify bar offsets at {value} due to end of range ends")
         d[value - shift if value else value + shift] = d[80]
         del d[value]
 
     modify_range_end(SS_counter, 0)
     modify_range_end(SS_counter, 80)
     modify_range_end(SO_counter, 0)
     modify_range_end(SO_counter, 80)
@@ -414,28 +412,28 @@
     genome in F1, F2, BCn ... the goal of this simulation, is thus to
     understand the mode and the spread of such diversity in the hybrid
     progenies.
     """
     sns.set_style("darkgrid")
 
     p = OptionParser(simulate.__doc__)
-    p.add_option(
+    p.add_argument(
         "--verbose",
         default=False,
         action="store_true",
         help="Verbose logging during simulation",
     )
-    p.add_option("-N", default=10000, type="int", help="Number of simulated samples")
+    p.add_argument("-N", default=10000, type=int, help="Number of simulated samples")
     opts, args, iopts = p.set_image_options(args, figsize="6x6")
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (mode,) = args
     validate_in_choices(mode, ["2n+n", "nx2+n"], "Mode")
-    logging.info(f"Transmission: {mode}")
+    logger.info(f"Transmission: {mode}")
 
     # Construct a composite figure with 6 tracks
     fig = plt.figure(1, (iopts.w, iopts.h))
     root = fig.add_axes([0, 0, 1, 1])
     rows = 6
     ypad = 0.05
     yinterval = (1 - 2 * ypad) / (rows + 1)
@@ -665,19 +663,19 @@
     %prog divergence SS_SR_SO.summary.txt
 
     Plot divergence between and within SS/SR/SO genomes.
     """
     sns.set_style("white")
 
     p = OptionParser(divergence.__doc__)
-    p.add_option("--title", default="Gapless", help="Plot title")
-    p.add_option(
+    p.add_argument("--title", default="Gapless", help="Plot title")
+    p.add_argument(
         "--xmin",
         default=94,
-        type="int",
+        type=int,
         help="Minimum percent identity in the histogram",
     )
     opts, args, iopts = p.set_image_options(args, figsize="8x8")
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (summary,) = args
```

### Comparing `jcvi-1.4.6/jcvi/projects/synfind.py` & `jcvi-1.4.7/jcvi/projects/synfind.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,38 +2,37 @@
 # -*- coding: UTF-8 -*-
 
 """
 SynFind analyses and visualization.
 """
 import os.path as op
 import sys
-import logging
 
-from copy import deepcopy
 from collections import defaultdict
+from copy import deepcopy
 from itertools import groupby
 
-from jcvi.formats.base import get_number, must_open
-from jcvi.utils.cbook import SummaryStats, gene_name, percentage
-from jcvi.utils.grouper import Grouper
-from jcvi.formats.blast import BlastLine
-from jcvi.formats.bed import Bed
-from jcvi.formats.gff import Gff, load
-from jcvi.apps.grid import MakeManager
-from jcvi.graphics.base import (
+from ..apps.base import ActionDispatcher, OptionParser, logger, mkdir, symlink
+from ..apps.grid import MakeManager
+from ..formats.base import get_number, must_open
+from ..formats.bed import Bed
+from ..formats.blast import BlastLine
+from ..formats.gff import Gff, load
+from ..graphics.base import (
     FancyArrow,
     plt,
     savefig,
     panel_labels,
     markup,
     normalize_axes,
     latex,
 )
-from jcvi.graphics.glyph import CartoonRegion, RoundRect
-from jcvi.apps.base import OptionParser, ActionDispatcher, mkdir, symlink
+from ..graphics.glyph import CartoonRegion, RoundRect
+from ..utils.cbook import SummaryStats, gene_name, percentage
+from ..utils.grouper import Grouper
 
 
 def main():
 
     actions = (
         ("cartoon", "generate cartoon illustration of SynFind"),
         ("ecoli", "gene presence absence analysis in ecoli"),
@@ -109,26 +108,26 @@
     fw = open(filteredlast, "w")
     for row in fp:
         b = BlastLine(row)
         if b.query == b.subject:
             continue
         print(b, file=fw)
     fw.close()
-    logging.debug("Filtered LAST file written to `{0}`".format(filteredlast))
+    logger.debug("Filtered LAST file written to `{0}`".format(filteredlast))
 
     allbed = "all.bed"
     fw = open(allbed, "w")
     for i, bedfile in enumerate(bedfiles):
         prefix = chr(ord("A") + i)
         bed = Bed(bedfile)
         for b in bed:
             b.seqid = prefix + b.seqid
             print(b, file=fw)
     fw.close()
-    logging.debug("Bed file written to `{0}`".format(allbed))
+    logger.debug("Bed file written to `{0}`".format(allbed))
 
 
 def yeasttruth(args):
     """
     %prog yeasttruth Pillars.tab *.gff
 
     Prepare pairs data for 14 yeasts.
@@ -150,16 +149,16 @@
         for g in gff:
             if g.type != "gene":
                 continue
             for a in g.attributes["Alias"]:
                 aliases[a] = g.accn
                 if is_pivot:
                     pivot[a] = g.accn
-    logging.debug("Aliases imported: {0}".format(len(aliases)))
-    logging.debug("Pivot imported: {0}".format(len(pivot)))
+    logger.debug("Aliases imported: {0}".format(len(aliases)))
+    logger.debug("Pivot imported: {0}".format(len(pivot)))
     fw = open("yeast.aliases", "w")
     for k, v in sorted(aliases.items()):
         print("\t".join((k, v)), file=fw)
     fw.close()
 
     fp = open(pillars)
     pairs = set()
@@ -288,16 +287,16 @@
         )
 
 
 def calc_sensitivity_specificity(a, truth, tag, fw):
     common = a & truth
     sensitivity = len(common) * 100.0 / len(truth)
     specificity = len(common) * 100.0 / len(a)
-    logging.debug("{0}: {1} pairs".format(tag, len(a)))
-    logging.debug(
+    logger.debug("{0}: {1} pairs".format(tag, len(a)))
+    logger.debug(
         "{0}: Sensitivity={1:.1f}% Purity={2:.1f}%".format(
             tag, sensitivity, specificity
         )
     )
     print(tag, len(a), len(truth), len(common), file=fw)
 
 
@@ -330,15 +329,15 @@
 
     fp = open(truth)
     truth = set()
     for row in fp:
         a, b = row.strip().split("\t")[:2]
         pivots.add(a)
         truth.add(tuple(sorted((a, b))))
-    logging.debug("Truth: {0} pairs".format(len(truth)))
+    logger.debug("Truth: {0} pairs".format(len(truth)))
 
     fp = open(synfind)
     benchmarkfile = pf + ".benchmark"
     fw = must_open(benchmarkfile, "w")
     synfind = set()
     for row in fp:
         atoms = row.strip().split("\t")
@@ -444,15 +443,15 @@
     b = BlastLine(next(fp))
     subject = b.subject
     txtfiles = []
     for bedfile in bedfiles:
         order = Bed(bedfile).order
         if subject in order:
             db = op.basename(bedfile).split(".")[0][:20]
-            logging.debug("Found db: {0}".format(db))
+            logger.debug("Found db: {0}".format(db))
         txtfile = write_txt(bedfile)
         txtfiles.append(txtfile)
 
     db += ".txt"
     mm = MakeManager()
     for txtfile in txtfiles:
         outfile = txtfile + ".alignment"
@@ -488,17 +487,15 @@
             a, b = b, a
         seen.add((a, b))
 
     fw = open(blast_table, "w")
     for a, b in seen:
         print("\t".join((a, b)), file=fw)
     fw.close()
-    logging.debug(
-        "A total of {0} pairs written to `{1}`".format(len(seen), blast_table)
-    )
+    logger.debug("A total of {0} pairs written to `{1}`".format(len(seen), blast_table))
 
     fw = open("config.txt", "w")
     for bedfile in bedfiles:
         pf, stanza = write_lst(bedfile)
         print("genome={0}".format(pf), file=fw)
         for seqid, fname in stanza:
             print(" ".join((seqid, fname)), file=fw)
@@ -569,15 +566,15 @@
 def make_gff(bed, prefix, fw):
     bed = Bed(bed)
     nfeats = 0
     for b in bed:
         seqid = prefix + b.seqid
         print("\t".join(str(x) for x in (seqid, b.accn, b.start, b.end)), file=fw)
         nfeats += 1
-    logging.debug("A total of {0} features converted to `{1}`".format(nfeats, fw.name))
+    logger.debug("A total of {0} features converted to `{1}`".format(nfeats, fw.name))
 
 
 def mcscanx(args):
     """
     %prog mcscanx athaliana.athaliana.last athaliana.bed
 
     Wrap around MCScanX.
@@ -675,16 +672,16 @@
             print(diff)
             print(jaccard)
         if jaccard > 99:
             perfect_matches += 1
         if corr_jaccard > 99:
             corr_perfect_matches += 1
 
-    logging.debug("Perfect matches: {0}".format(perfect_matches))
-    logging.debug("Perfect matches (corrected): {0}".format(corr_perfect_matches))
+    logger.debug("Perfect matches: {0}".format(perfect_matches))
+    logger.debug("Perfect matches (corrected): {0}".format(corr_perfect_matches))
     print("Jaccards:", SummaryStats(jaccards))
     print("Corrected Jaccards:", SummaryStats(corr_jaccards))
 
 
 def ecoli(args):
     """
     %prog ecoli coge_master_table.txt query.bed
@@ -727,15 +724,15 @@
         store[a] = b in MISSING and c in MISSING
 
     bed = Bed(querybed)
     tags = []
     for i, b in enumerate(bed):
         accn = b.accn
         if accn not in store:
-            logging.warning("missing {0}".format(accn))
+            logger.warning("missing {0}".format(accn))
             continue
         tags.append((store[accn], accn))
 
     large = 4  # large segments
     II = []
     II_large = []
     for missing, aa in groupby(tags, key=lambda x: x[0]):
@@ -747,15 +744,15 @@
         size = len(glist)
         if size >= large:
             II_large.append(glist)
 
     fw = must_open(opts.outfile, "w")
     for a, t in zip((II, II_large), ("", ">=4 ")):
         nmissing = sum(len(x) for x in a)
-        logging.debug(
+        logger.debug(
             "A total of {0} {1}-specific {2}islands found with {3} genes.".format(
                 len(a), qorg, t, nmissing
             )
         )
 
     for x in II:
         print(len(x), ",".join(x), file=fw)
```

### Comparing `jcvi-1.4.6/jcvi/projects/tgbs.py` & `jcvi-1.4.7/jcvi/projects/tgbs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 """
 Reference-free tGBS related functions.
 """
 
-import logging
 import os
 import os.path as op
 import sys
 
 from collections import Counter
 from pickle import dump, load
 
-from jcvi.formats.fasta import Fasta, SeqIO
-from jcvi.formats.fastq import iter_fastq
-from jcvi.formats.base import must_open, write_file
-from jcvi.formats.sam import get_prefix
-from jcvi.apps.cdhit import deduplicate
-from jcvi.apps.gmap import check_index
-from jcvi.apps.grid import MakeManager
-from jcvi.graphics.base import plt, savefig, normalize_axes
-from jcvi.apps.base import OptionParser, ActionDispatcher, need_update, sh, iglob, mkdir
+from ..apps.base import (
+    ActionDispatcher,
+    OptionParser,
+    iglob,
+    logger,
+    mkdir,
+    need_update,
+    sh,
+)
+from ..apps.cdhit import deduplicate
+from ..apps.gmap import check_index
+from ..apps.grid import MakeManager
+from ..formats.base import must_open, write_file
+from ..formats.fasta import Fasta, SeqIO
+from ..formats.fastq import iter_fastq
+from ..formats.sam import get_prefix
+from ..graphics.base import normalize_axes, plt, savefig
 
 
 speedupsh = r"""
 cd {0}
 
 find *.native | sed 's/\..*//' | sort -u | \
     awk '{{ printf("split_by_chromosome.pl -s %s -o splitted_%s -native %s.*.native -x 5\n", \
@@ -98,15 +105,15 @@
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     locifile, contig = args
     idx = build_index(locifile)
     pos = idx[contig]
-    logging.debug("Contig {0} found at pos {1}".format(contig, pos))
+    logger.debug("Contig {0} found at pos {1}".format(contig, pos))
     fp = open(locifile)
     fp.seek(pos)
     section = []
     while True:
         row = fp.readline()
         if row.startswith("//") and row.split()[1] != contig:
             break
@@ -160,20 +167,20 @@
     %prog mstmap LMD50.snps.genotype.txt
 
     Convert LMDs to MSTMAP input.
     """
     from jcvi.assembly.geneticmap import MSTMatrix
 
     p = OptionParser(mstmap.__doc__)
-    p.add_option(
+    p.add_argument(
         "--population_type",
         default="RIL6",
         help="Type of population, possible values are DH and RILd",
     )
-    p.add_option(
+    p.add_argument(
         "--missing_threshold",
         default=0.5,
         help="Missing threshold, .25 excludes any marker with >25% missing",
     )
     p.set_outfile()
     opts, args = p.parse_args(args)
 
@@ -203,16 +210,16 @@
 
     Extract base composition for reads
     """
     import numpy as np
     from rich.progress import Progress
 
     p = OptionParser(weblogo.__doc__)
-    p.add_option("-N", default=10, type="int", help="Count the first and last N bases")
-    p.add_option("--nreads", default=1000000, type="int", help="Parse first N reads")
+    p.add_argument("-N", default=10, type=int, help="Count the first and last N bases")
+    p.add_argument("--nreads", default=1000000, type=int, help="Parse first N reads")
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (fastqfile,) = args
     N = opts.N
@@ -282,15 +289,15 @@
 
     Scan the headers for the consensus clusters and count the number of reads.
     """
     from jcvi.graphics.histogram import stem_leaf_plot
     from jcvi.utils.cbook import SummaryStats
 
     p = OptionParser(count.__doc__)
-    p.add_option("--csv", help="Write depth per contig to file")
+    p.add_argument("--csv", help="Write depth per contig to file")
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (fastafile,) = args
     csv = open(opts.csv, "w") if opts.csv else None
@@ -312,15 +319,15 @@
         # MRD85:00603:02472;size=167;
         else:
             name, size, tail = desc.split(";")
             sizes.append(int(size.replace("size=", "")))
 
     if csv:
         csv.close()
-        logging.debug("File written to `%s`.", opts.csv)
+        logger.debug("File written to `%s`.", opts.csv)
 
     s = SummaryStats(sizes)
     print(s, file=sys.stderr)
     stem_leaf_plot(s.data, 0, 100, 20, title="Cluster size")
 
 
 def novo(args):
@@ -331,15 +338,15 @@
     """
     from jcvi.assembly.kmer import jellyfish, histogram
     from jcvi.assembly.preprocess import diginorm
     from jcvi.formats.fasta import filter as fasta_filter, format
     from jcvi.apps.cdhit import filter as cdhit_filter
 
     p = OptionParser(novo.__doc__)
-    p.add_option(
+    p.add_argument(
         "--technology",
         choices=("illumina", "454", "iontorrent"),
         default="iontorrent",
         help="Sequencing platform",
     )
     p.set_depth(depth=50)
     p.set_align(pctid=96)
@@ -418,15 +425,15 @@
             ]
         )
 
 
 def scan_read_files(trimmed, patterns):
     reads = iglob(trimmed, patterns)
     samples = sorted(set(op.basename(x).split(".")[0] for x in reads))
-    logging.debug(
+    logger.debug(
         "Total {0} read files from {1} samples".format(len(reads), len(samples))
     )
     return reads, samples
 
 
 def novo2(args):
     """
@@ -507,15 +514,15 @@
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     trimmed, ref = args
     nseqs = len(Fasta(ref))
     supercat = nseqs >= 1000
     if supercat:
-        logging.debug("Total seqs in ref: {0} (supercat={1})".format(nseqs, supercat))
+        logger.debug("Total seqs in ref: {0} (supercat={1})".format(nseqs, supercat))
 
     reads, samples = scan_read_files(trimmed, opts.names)
 
     # Set up directory structure
     nativedir, countsdir = "native", "allele_counts"
     for d in (nativedir, countsdir):
         mkdir(d)
```

### Comparing `jcvi-1.4.6/jcvi/projects/vanilla.py` & `jcvi-1.4.7/jcvi/projects/vanilla.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from ..compara.synteny import check_beds
 from ..formats.base import get_number
 from ..formats.bed import Bed
 from ..graphics.base import normalize_axes, panel_labels, plt, savefig
 from ..graphics.chromosome import draw_chromosomes
 from ..graphics.glyph import TextCircle
 from ..graphics.synteny import Synteny, draw_gene_legend
-from ..graphics.tree import parse_tree, LeafInfoFile, WGDInfoFile, draw_tree
+from ..graphics.tree import LeafInfoFile, WGDInfoFile, draw_tree, parse_tree
 
 
 def main():
     actions = (
         # Chromosome painting since WGD
         ("ancestral", "paint 14 chromosomes following alpha WGD (requires data)"),
         # main figures in text
```

### Comparing `jcvi-1.4.6/jcvi/utils/aws.py` & `jcvi-1.4.7/jcvi/utils/aws.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 """
 AWS-related methods.
 """
+import fnmatch
+import getpass
+import json
 import os
 import os.path as op
 import sys
-import fnmatch
-import boto3
-import json
-import logging
 import time
-import getpass
 
 from configparser import NoOptionError, NoSectionError
 from datetime import datetime
 from multiprocessing import Pool
+
+import boto3
+
 from botocore.exceptions import ClientError, ParamValidationError
 
-from jcvi.formats.base import BaseFile, SetFile, timestamp
-from jcvi.utils.console import console
-from jcvi.apps.base import (
-    OptionParser,
+from ..apps.base import (
     ActionDispatcher,
+    OptionParser,
     datafile,
     get_config,
+    logger,
     popen,
     sh,
 )
+from ..formats.base import BaseFile, SetFile, timestamp
+
+from .console import console
+
 
 AWS_CREDS_PATH = "%s/.aws/credentials" % (op.expanduser("~"),)
 
 
 class InstanceSkeleton(BaseFile):
     def __init__(self, filename=datafile("instance.json")):
         super(InstanceSkeleton, self).__init__(filename)
@@ -140,36 +144,36 @@
 def start(args):
     """
     %prog start
 
     Launch ec2 instance through command line.
     """
     p = OptionParser(start.__doc__)
-    p.add_option(
+    p.add_argument(
         "--ondemand",
         default=False,
         action="store_true",
         help="Do we want a more expensive on-demand instance",
     )
-    p.add_option("--profile", default="mvrad-datasci-role", help="Profile name")
-    p.add_option("--price", default=4.0, type=float, help="Spot price")
+    p.add_argument("--profile", default="mvrad-datasci-role", help="Profile name")
+    p.add_argument("--price", default=4.0, type=float, help="Spot price")
     opts, args = p.parse_args(args)
 
     if len(args) != 0:
         sys.exit(not p.print_help())
 
     role(["htang"])
     session = boto3.Session(profile_name=opts.profile)
     client = session.client("ec2")
     s = InstanceSkeleton()
 
     # Make sure the instance id is empty
     instance_id = s.instance_id
     if instance_id != "":
-        logging.error("Instance exists {}".format(instance_id))
+        logger.error("Instance exists {}".format(instance_id))
         sys.exit(1)
 
     launch_spec = s.launch_spec
     instance_id = ""
 
     if opts.ondemand:
         # Launch on-demand instance
@@ -204,22 +208,22 @@
         while not instance_id:
             response = client.describe_spot_instance_requests(
                 SpotInstanceRequestIds=[request_id]
             )
             if "InstanceId" in response["SpotInstanceRequests"][0]:
                 instance_id = response["SpotInstanceRequests"][0]["InstanceId"]
             else:
-                logging.debug("Waiting to be fulfilled ...")
+                logger.debug("Waiting to be fulfilled ...")
                 time.sleep(10)
 
     # Check if the instance is running
     print("Instance id {}".format(instance_id), file=sys.stderr)
     status = ""
     while status != "running":
-        logging.debug("Waiting instance to run ...")
+        logger.debug("Waiting instance to run ...")
         time.sleep(3)
         response = client.describe_instance_status(InstanceIds=[instance_id])
         if len(response["InstanceStatuses"]) > 0:
             status = response["InstanceStatuses"][0]["InstanceState"]["Name"]
 
     # Tagging
     name = "htang-lx-ondemand" if opts.ondemand else "htang-lx-spot"
@@ -253,29 +257,29 @@
 def stop(args):
     """
     %prog stop
 
     Stop EC2 instance.
     """
     p = OptionParser(stop.__doc__)
-    p.add_option("--profile", default="mvrad-datasci-role", help="Profile name")
+    p.add_argument("--profile", default="mvrad-datasci-role", help="Profile name")
     opts, args = p.parse_args(args)
 
     if len(args) != 0:
         sys.exit(not p.print_help())
 
     role(["htang"])
     session = boto3.Session(profile_name=opts.profile)
     client = session.client("ec2")
     s = InstanceSkeleton()
 
     # Make sure the instance id is NOT empty
     instance_id = s.instance_id
     if instance_id == "":
-        logging.error("Cannot find instance_id {}".format(instance_id))
+        logger.error("Cannot find instance_id {}".format(instance_id))
         sys.exit(1)
 
     block_device_mappings = []
     for volume in s.volumes:
         block_device_mappings.append({"DeviceName": volume["Device"], "NoDevice": ""})
 
     new_image_name = "htang-dev-{}-{}".format(timestamp(), int(time.time()))
@@ -285,15 +289,15 @@
         BlockDeviceMappings=block_device_mappings,
     )
     print(response, file=sys.stderr)
     new_image_id = response["ImageId"]
 
     image_status = ""
     while image_status != "available":
-        logging.debug("Waiting for image to be ready")
+        logger.debug("Waiting for image to be ready")
         time.sleep(10)
         response = client.describe_images(ImageIds=[new_image_id])
         image_status = response["Images"][0]["State"]
 
     # Delete old image, snapshot and shut down instance
     old_image_id = s.image_id
     response = client.describe_images(ImageIds=[old_image_id])
@@ -358,15 +362,15 @@
 def cp(args):
     """
     %prog cp "s3://hli-mv-data-science/htang/str/*.csv" .
 
     Copy files to folder. Accepts list of s3 addresses as input.
     """
     p = OptionParser(cp.__doc__)
-    p.add_option(
+    p.add_argument(
         "--force", default=False, action="store_true", help="Force overwrite if exists"
     )
     p.set_cpus()
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
@@ -401,16 +405,16 @@
 def ls(args):
     """
     %prog ls "s3://hli-mv-data-science/htang/str/*.vcf.gz"
 
     List files with support for wildcards.
     """
     p = OptionParser(ls.__doc__)
-    p.add_option("--keys", help="List of keys to include")
-    p.add_option(
+    p.add_argument("--keys", help="List of keys to include")
+    p.add_argument(
         "--recursive", default=False, action="store_true", help="Recursive search"
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
@@ -484,15 +488,15 @@
     Check if s3 object exists.
     """
     s3_store_obj_name = s3ify(s3_store_obj_name)
     cmd = "aws s3 ls {0} | wc -l".format(s3_store_obj_name)
     counts = int(popen(cmd).read())
     exists = counts != 0
     if exists and warn:
-        logging.debug("{} exists. Skipped.".format(s3_store_obj_name))
+        logger.debug("{} exists. Skipped.".format(s3_store_obj_name))
     return exists
 
 
 def aws_configure(profile, key, value):
     sh("aws configure set profile.{0}.{1} {2}".format(profile, key, value))
 
 
@@ -506,50 +510,50 @@
         src_acct,
         src_username,
         dst_acct,
         dst_role,
     ) = "205134639408 htang 114692162163 mvrad-datasci-role".split()
 
     p = OptionParser(role.__doc__)
-    p.add_option("--profile", default="mvrad-datasci-role", help="Profile name")
-    p.add_option(
+    p.add_argument("--profile", default="mvrad-datasci-role", help="Profile name")
+    p.add_argument(
         "--device",
         default="arn:aws:iam::" + src_acct + ":mfa/" + src_username,
         metavar="arn:aws:iam::123456788990:mfa/dudeman",
         help="The MFA Device ARN. This value can also be "
         "provided via the environment variable 'MFA_DEVICE' or"
         " the ~/.aws/credentials variable 'aws_mfa_device'.",
     )
-    p.add_option(
+    p.add_argument(
         "--duration",
         type=int,
         default=3600,
         help="The duration, in seconds, that the temporary "
         "credentials should remain valid. Minimum value: "
         "900 (15 minutes). Maximum: 129600 (36 hours). "
         "Defaults to 43200 (12 hours), or 3600 (one "
         "hour) when using '--assume-role'. This value "
         "can also be provided via the environment "
         "variable 'MFA_STS_DURATION'. ",
     )
-    p.add_option(
+    p.add_argument(
         "--assume-role",
         "--assume",
         default="arn:aws:iam::" + dst_acct + ":role/" + dst_role,
         metavar="arn:aws:iam::123456788990:role/RoleName",
         help="The ARN of the AWS IAM Role you would like to "
         "assume, if specified. This value can also be provided"
         " via the environment variable 'MFA_ASSUME_ROLE'",
     )
-    p.add_option(
+    p.add_argument(
         "--role-session-name",
         help="Friendly session name required when using --assume-role",
         default=getpass.getuser(),
     )
-    p.add_option(
+    p.add_argument(
         "--force",
         help="Refresh credentials even if currently valid.",
         action="store_true",
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
@@ -573,15 +577,15 @@
         role_msg = "with assumed role: %s" % (args.assume_role,)
     elif config.has_option(args.profile, "assumed_role_arn"):
         role_msg = "with assumed role: %s" % (
             config.get(args.profile, "assumed_role_arn")
         )
     else:
         role_msg = ""
-    logging.info("Validating credentials for profile: %s %s" % (profile, role_msg))
+    logger.info("Validating credentials for profile: %s %s" % (profile, role_msg))
     reup_message = "Obtaining credentials for a new role or profile."
 
     try:
         key_id = config.get(profile, "aws_access_key_id")
         access_key = config.get(profile, "aws_secret_access_key")
     except NoSectionError:
         log_error_and_exit(
@@ -638,32 +642,32 @@
             "expiration",
         ]
         try:
             short_term = {}
             for option in required_options:
                 short_term[option] = config.get(profile, option)
         except NoOptionError:
-            logging.warning(
+            logger.warning(
                 "Your existing credentials are missing or invalid, "
                 "obtaining new credentials."
             )
             force_refresh = True
 
         try:
             current_role = config.get(profile, "assumed_role_arn")
         except NoOptionError:
             current_role = None
 
         if args.force:
-            logging.info("Forcing refresh of credentials.")
+            logger.info("Forcing refresh of credentials.")
             force_refresh = True
         # There are not credentials for an assumed role,
         # but the user is trying to assume one
         elif current_role is None and args.assume_role:
-            logging.info(reup_message)
+            logger.info(reup_message)
             force_refresh = True
         # There are current credentials for a role and
         # the role arn being provided is the same.
         elif (
             current_role is not None
             and args.assume_role
             and current_role == args.assume_role
@@ -672,33 +676,33 @@
         # There are credentials for a current role and the role
         # that is attempting to be assumed is different
         elif (
             current_role is not None
             and args.assume_role
             and current_role != args.assume_role
         ):
-            logging.info(reup_message)
+            logger.info(reup_message)
             force_refresh = True
         # There are credentials for a current role and no role arn is
         # being supplied
         elif current_role is not None and args.assume_role is None:
-            logging.info(reup_message)
+            logger.info(reup_message)
             force_refresh = True
 
     should_refresh = True
 
     # Unless we're forcing a refresh, check expiration.
     if not force_refresh:
         exp = datetime.strptime(config.get(profile, "expiration"), "%Y-%m-%d %H:%M:%S")
         diff = exp - datetime.utcnow()
         if diff.total_seconds() <= 0:
-            logging.info("Your credentials have expired, renewing.")
+            logger.info("Your credentials have expired, renewing.")
         else:
             should_refresh = False
-            logging.info(
+            logger.info(
                 "Your credentials are still valid for %s seconds"
                 " they will expire at %s" % (diff.total_seconds(), exp)
             )
 
     if should_refresh:
         get_credentials(profile, args, config)
 
@@ -710,15 +714,15 @@
     )
 
     boto3.setup_default_session(profile_name="default")
     client = boto3.client("sts")
 
     if args.assume_role:
 
-        logging.info(
+        logger.info(
             "Assuming Role - Profile: %s, Role: %s, Duration: %s",
             profile,
             args.assume_role,
             args.duration,
         )
 
         try:
@@ -743,15 +747,15 @@
         )
         config.set(
             profile,
             "assumed_role_arn",
             args.assume_role,
         )
     else:
-        logging.info(
+        logger.info(
             "Fetching Credentials - Profile: %s, Duration: %s", profile, args.duration
         )
         try:
             response = client.get_session_token(
                 DurationSeconds=args.duration,
                 SerialNumber=args.device,
                 TokenCode=mfa_token,
@@ -786,21 +790,21 @@
         profile,
         "expiration",
         response["Credentials"]["Expiration"].strftime("%Y-%m-%d %H:%M:%S"),
     )
     with open(AWS_CREDS_PATH, "w") as configfile:
         config.write(configfile)
 
-    logging.info(
+    logger.info(
         "Success! Your credentials will expire in %s seconds at: %s"
         % (args.duration, response["Credentials"]["Expiration"])
     )
 
 
 def log_error_and_exit(message):
     """Log an error message and exit with error"""
-    logging.error(message)
+    logger.error(message)
     sys.exit(1)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `jcvi-1.4.6/jcvi/utils/cbook.py` & `jcvi-1.4.7/jcvi/utils/cbook.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 Useful recipes from various internet sources (thanks)
 mostly decorator patterns
 """
 
 import os.path as op
 import re
 import sys
-import logging
 
 from collections import defaultdict
 
+from ..apps.base import logger
+
 
 def inspect(item, maxchar=80):
     """
     Inspect the attributes of an item.
     """
     for i in dir(item):
         try:
@@ -33,15 +34,15 @@
 
     def timed(*args, **kw):
         ts = time.time()
         result = func(*args, **kw)
         te = time.time()
 
         msg = "{0}{1} {2:.2f}s".format(func.__name__, args, te - ts)
-        logging.debug(msg)
+        logger.debug(msg)
 
         return result
 
     return timed
 
 
 def depends(func):
@@ -145,15 +146,15 @@
         return d
 
     def tofile(self, filename):
         fw = open(filename, "w")
         for x in self.data:
             print(x, file=fw)
         fw.close()
-        logging.debug(
+        logger.debug(
             "Array of size {0} written to file `{1}`.".format(self.size, filename)
         )
 
 
 class AutoVivification(dict):
     """
     Implementation of perl's autovivification feature.
@@ -390,16 +391,14 @@
     Some examples from Maize
         Convert a seqid like
             `chromosome:AGPv2:2:1:237068873:1` to `2`
         Special cases
             `chromosome:AGPv2:mitochondrion:1:569630:1` to `Mt`
             `chromosome:AGPv2:chloroplast:1:140384:1` to `Pt`
     """
-    import re
-
     mtr_pat1 = re.compile(r"Mt[0-9]+\.[0-9]+[.[0-9]+]*_([a-z]+[0-9]+)")
     mtr_pat2 = re.compile(r"([A-z0-9]+)_[A-z]+_[A-z]+")
 
     zmays_pat = re.compile(r"[a-z]+:[A-z0-9]+:([A-z0-9]+):[0-9]+:[0-9]+:[0-9]+")
     zmays_sub = {"mitochondrion": "Mt", "chloroplast": "Pt"}
     if orgn == "medicago":
         for mtr_pat in (mtr_pat1, mtr_pat2):
```

### Comparing `jcvi-1.4.6/jcvi/utils/data/Airswing.ttf` & `jcvi-1.4.7/jcvi/utils/data/Airswing.ttf`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.6/jcvi/utils/data/Collegia.ttf` & `jcvi-1.4.7/jcvi/utils/data/Collegia.ttf`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.6/jcvi/utils/data/HookedUp.ttf` & `jcvi-1.4.7/jcvi/utils/data/HookedUp.ttf`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.6/jcvi/utils/data/Humor-Sans.ttf` & `jcvi-1.4.7/jcvi/utils/data/Humor-Sans.ttf`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.6/jcvi/utils/data/TREDs.meta.csv` & `jcvi-1.4.7/jcvi/utils/data/TREDs.meta.csv`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.6/jcvi/utils/data/adapters.fasta` & `jcvi-1.4.7/jcvi/utils/data/adapters.fasta`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.6/jcvi/utils/data/blosum80.mat` & `jcvi-1.4.7/jcvi/utils/data/blosum80.mat`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.6/jcvi/utils/data/chrY.hg38.unique_ccn.gc` & `jcvi-1.4.7/jcvi/utils/data/chrY.hg38.unique_ccn.gc`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.6/jcvi/utils/data/hg38.band.txt` & `jcvi-1.4.7/jcvi/utils/data/hg38.band.txt`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.6/jcvi/utils/data/hg38.chrom.sizes` & `jcvi-1.4.7/jcvi/utils/data/hg38.chrom.sizes`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.6/jcvi/utils/data/instance.json` & `jcvi-1.4.7/jcvi/utils/data/instance.json`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.6/jcvi/utils/db.py` & `jcvi-1.4.7/jcvi/utils/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 """
 Connect to databases (Sybase, MySQL and PostgreSQL database backends)
 """
 import os.path as op
-import sys
-import logging
 import re
+import sys
 
-from jcvi.formats.base import must_open
-from jcvi.apps.base import OptionParser, ActionDispatcher, sh, getusername
-from jcvi.utils.cbook import AutoVivification
+from ..apps.base import ActionDispatcher, OptionParser, getusername, logger, sh
+from ..formats.base import must_open
+from ..utils.cbook import AutoVivification
 
 
 # set up valid database connection params
 valid_dbconn = AutoVivification()
 for dbconn, port, module, host in zip(
     ("Sybase", "MySQL", "PostgreSQL", "Oracle"),
     (2025, 3306, 5432, 1521),
@@ -167,15 +166,15 @@
     """
     %prog pull libfile
 
     Pull the sequences using the first column in the libfile.
     """
     p = OptionParser(pull.__doc__)
     p.set_db_opts(dbname="mtg2", credentials=None)
-    p.add_option(
+    p.add_argument(
         "--frag",
         default=False,
         action="store_true",
         help="The command to pull sequences from db",
     )
     opts, args = p.parse_args(args)
 
@@ -235,15 +234,15 @@
     either printed out (when running `select`) or not (when running `insert`, `update`
     or `delete`)
 
     If the query contains quotes around field values, then these need to be escaped with \\
     """
     p = OptionParser(query.__doc__)
     p.set_db_opts()
-    p.add_option(
+    p.add_argument(
         "--dryrun",
         default=False,
         action="store_true",
         help="Don't commit to database. Just print queries",
     )
     p.set_sep(help="Specify output field separator")
     p.set_verbose(help="Print out all the queries")
@@ -295,18 +294,16 @@
                         natoms = [atoms[x] for x in mi]
                         for idx, (match, atom) in enumerate(zip(m, natoms)):
                             qry = qry.replace(match, atom)
                     queries.add(qry)
     else:
         for qry in qrys:
             if re.search(r"{\d+}", qry):
-                logging.error(
-                    "Query `{0}` contains placeholders, no datafile(s) specified".format(
-                        qry
-                    )
+                logger.error(
+                    "Query `%s` contains placeholders, no datafile(s) specified", qry
                 )
                 sys.exit()
             queries.add(qry)
 
     if not opts.dryrun:
         fw = must_open(opts.outfile, "w")
         dbh, cur = connect(
```

### Comparing `jcvi-1.4.6/jcvi/utils/ez_setup.py` & `jcvi-1.4.7/jcvi/utils/ez_setup.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.6/jcvi/utils/grouper.py` & `jcvi-1.4.7/jcvi/utils/grouper.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.6/jcvi/utils/orderedcollections.py` & `jcvi-1.4.7/jcvi/utils/orderedcollections.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.6/jcvi/utils/range.py` & `jcvi-1.4.7/jcvi/utils/range.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 `range_chain` implements the exon-chain algorithm
 """
 import sys
 
 from collections import namedtuple, defaultdict
 from itertools import groupby
+
 from more_itertools import pairwise
 
 
 LEFT, RIGHT = 0, 1
 Range = namedtuple("Range", "seqid start end score id")
```

### Comparing `jcvi-1.4.6/jcvi/utils/table.py` & `jcvi-1.4.7/jcvi/utils/table.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.6/jcvi/utils/taxonomy.py` & `jcvi-1.4.7/jcvi/utils/taxonomy.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,27 +24,26 @@
 
           \---|
 
                \-Populus_trichocarpa
 """
 import sys
 import time
-import logging
 
 from functools import lru_cache
 
 from urllib.request import urlopen
 from urllib.error import HTTPError, URLError
 
 from ete3 import Tree
 
 from ClientForm import ParseResponse
 from BeautifulSoup import BeautifulSoup
 
-from jcvi.apps.base import OptionParser, ActionDispatcher
+from ..apps.base import ActionDispatcher, OptionParser, logger
 
 
 URL = "http://itol.embl.de/other_trees.shtml"
 
 
 class TaxIDTree(object):
     def __init__(self, list_of_taxids):
@@ -61,16 +60,16 @@
 
         success = False
         while not success:
             try:
                 response = urlopen(URL)
                 success = True
             except (URLError, HTTPError, RuntimeError) as e:
-                logging.error(e)
-                logging.debug("wait 5 seconds to reconnect...")
+                logger.error(e)
+                logger.debug("wait 5 seconds to reconnect...")
                 time.sleep(5)
 
         forms = ParseResponse(response, backwards_compat=False)
         form = forms[0]
 
         form["ncbiIDs"] = form_data
         page = urlopen(form.click()).read()
```

### Comparing `jcvi-1.4.6/jcvi/utils/validator.py` & `jcvi-1.4.7/jcvi/utils/validator.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.6/jcvi/utils/webcolors.py` & `jcvi-1.4.7/jcvi/utils/webcolors.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 #
 # webcolors.py
 # utils
 #
 # Created by Haibao Tang on 01/28/20
 # Copyright © 2021 Haibao Tang. All rights reserved.
 #
-
 import logging
 
 import numpy as np
 
-from webcolors import CSS3_HEX_TO_NAMES, hex_to_rgb
 from skimage.color import rgb2lab, deltaE_cmc
+from webcolors import CSS3_HEX_TO_NAMES, hex_to_rgb
 
 
 def color_diff(rgb1, rgb2):
     """
     Calculate distance between two RGB colors. See discussion:
 
     http://stackoverflow.com/questions/8863810/python-find-similar-colors-best-way
```

### Comparing `jcvi-1.4.6/jcvi/variation/cnv.py` & `jcvi-1.4.7/jcvi/variation/cnv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 """
 Helper functions for Copy Number Variations (CNV).
 """
-import sys
 import logging
 import os.path as op
-
-import numpy as np
-import numpy.ma as ma
-import pandas as pd
-import pysam
+import sys
 
 from collections import Counter, defaultdict
 from dataclasses import dataclass
 from itertools import groupby
 from multiprocessing import Pool
 from random import choice
+
+import numpy as np
+import numpy.ma as ma
+import pandas as pd
+import pysam
+
 from pybedtools import BedTool, cleanup, set_tempdir
 
-from jcvi.algorithms.formula import get_kmeans
-from jcvi.apps.grid import MakeManager
-from jcvi.utils.aws import glob_s3, push_to_s3, sync_from_s3
-from jcvi.utils.cbook import percentage
-from jcvi.apps.base import OptionParser, ActionDispatcher, getfilesize, mkdir, popen, sh
+from ..algorithms.formula import get_kmeans
+from ..apps.base import (
+    ActionDispatcher,
+    OptionParser,
+    getfilesize,
+    logger,
+    mkdir,
+    popen,
+    sh,
+)
+from ..apps.grid import MakeManager
+from ..utils.aws import glob_s3, push_to_s3, sync_from_s3
+from ..utils.cbook import percentage
 
 logging.getLogger("matplotlib").setLevel(logging.WARNING)
 
-autosomes = ["chr{}".format(x) for x in range(1, 23)]
+autosomes = [f"chr{x}" for x in range(1, 23)]
 sexsomes = ["chrX", "chrY"]
 allsomes = autosomes + sexsomes
 # See: http://www.ncbi.nlm.nih.gov/projects/genome/assembly/grc/human/
 PAR = [("chrX", 10001, 2781479), ("chrX", 155701383, 156030895)]
 
 
 class CopyNumberSegment(object):
@@ -587,15 +596,15 @@
     for suffix in (".avgcn", ".medcn"):
         df_to_tsv(df, tsvfile, suffix)
 
 
 def vcf_to_df_worker(arg):
     """Convert CANVAS vcf to a dict, single thread"""
     canvasvcf, exonbed, i = arg
-    logging.debug("Working on job {}: {}".format(i, canvasvcf))
+    logger.debug("Working on job {}: {}".format(i, canvasvcf))
     samplekey = op.basename(canvasvcf).split(".")[0].rsplit("_", 1)[0]
     d = {"SampleKey": samplekey}
 
     exons = BedTool(exonbed)
     cn = parse_segments(canvasvcf)
     overlaps = exons.intersect(cn, wao=True)
     gcn_store = {}
@@ -782,33 +791,33 @@
         print("\n".join(res))
 
 
 def bam_to_cib(arg):
     bamfile, seq, samplekey = arg
     bam = pysam.AlignmentFile(bamfile, "rb")
     name, length = seq["SN"], seq["LN"]
-    logging.debug("Computing depth for {} (length={})".format(name, length))
+    logger.debug("Computing depth for {} (length={})".format(name, length))
     pileup = bam.pileup(name)
     a = np.ones(length, dtype=np.int8) * -128
     for x in pileup:
         a[x.reference_pos] = min(x.nsegments, 255) - 128
 
     cibfile = op.join(samplekey, "{}.{}.cib".format(samplekey, name))
     a.tofile(cibfile)
-    logging.debug("Depth written to `{}`".format(cibfile))
+    logger.debug("Depth written to `{}`".format(cibfile))
 
 
 def cib(args):
     """
     %prog cib bamfile samplekey
 
     Convert BAM to CIB (a binary storage of int8 per base).
     """
     p = OptionParser(cib.__doc__)
-    p.add_option("--prefix", help="Report seqids with this prefix only")
+    p.add_argument("--prefix", help="Report seqids with this prefix only")
     p.set_cpus()
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     bamfile, samplekey = args
@@ -819,29 +828,29 @@
     if prefix:
         refs = [x for x in refs if x["SN"].startswith(prefix)]
 
     task_args = []
     for r in refs:
         task_args.append((bamfile, r, samplekey))
     cpus = min(opts.cpus, len(task_args))
-    logging.debug("Use {} cpus".format(cpus))
+    logger.debug("Use {} cpus".format(cpus))
 
     p = Pool(processes=cpus)
     for _ in p.imap(bam_to_cib, task_args):
         continue
 
 
 def batchcn(args):
     """
     %prog batchcn workdir samples.csv
 
     Run CNV segmentation caller in batch mode. Scans a workdir.
     """
     p = OptionParser(batchcn.__doc__)
-    p.add_option(
+    p.add_argument(
         "--upload",
         default="s3://hli-mv-data-science/htang/ccn",
         help="Upload cn and seg results to s3",
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
@@ -861,38 +870,38 @@
         samplekey, path = row.strip().split(",")
         ntotal += 1
         if samplekey in computed:
             nskipped += 1
             continue
         print(" ".join((cmd, samplekey, path)))
 
-    logging.debug("Skipped: {}".format(percentage(nskipped, ntotal)))
+    logger.debug("Skipped: {}".format(percentage(nskipped, ntotal)))
 
 
 def hmm(args):
     """
     %prog hmm workdir sample_key
 
     Run CNV segmentation caller. The workdir must contain a subfolder called
     `sample_key-cn` that contains CN for each chromosome. A `beta` directory
     that contains scaler for each bin must also be present in the current
     directory.
     """
     p = OptionParser(hmm.__doc__)
-    p.add_option("--mu", default=0.003, type="float", help="Transition probability")
-    p.add_option(
+    p.add_argument("--mu", default=0.003, type=float, help="Transition probability")
+    p.add_argument(
         "--sigma",
         default=0.1,
-        type="float",
+        type=float,
         help="Standard deviation of Gaussian emission distribution",
     )
-    p.add_option(
+    p.add_argument(
         "--threshold",
         default=1,
-        type="float",
+        type=float,
         help="Standard deviation must be < this in the baseline population",
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
@@ -907,15 +916,15 @@
     nevents = 0
     for mean_cn, rr, event in events:
         if event is None:
             continue
         print(" ".join((event.bedline, sample_key)), file=fw)
         nevents += 1
     fw.close()
-    logging.debug(
+    logger.debug(
         "A total of {} aberrant events written to `{}`".format(nevents, hmmfile)
     )
     return hmmfile
 
 
 def batchccn(args):
     """
@@ -932,15 +941,15 @@
     (csvfile,) = args
     mm = MakeManager()
     pf = op.basename(csvfile).split(".")[0]
     mkdir(pf)
 
     header = next(open(csvfile))
     header = None if header.strip().endswith(".bam") else "infer"
-    logging.debug("Header={}".format(header))
+    logger.debug("Header={}".format(header))
     df = pd.read_csv(csvfile, header=header)
     cmd = "perl /mnt/software/ccn_gcn_hg38_script/ccn_gcn_hg38.pl"
     cmd += " -n {} -b {}"
     cmd += " -o {} -r hg38".format(pf)
     for i, (sample_key, bam) in df.iterrows():
         cmdi = cmd.format(sample_key, bam)
         outfile = "{}/{}/{}.ccn".format(pf, sample_key, sample_key)
@@ -977,17 +986,15 @@
         ploidy = 2 if seqid not in ("chrY", "chrM") else 1
         if seqid in sexsomes:
             chr_med = [np.median([x for x in a if x > 0]) for a in arrays]
             chr_med = np.array(chr_med)
             idx = get_kmeans(chr_med, k=2)
             zero_med = np.median(chr_med[idx == 0])
             one_med = np.median(chr_med[idx == 1])
-            logging.debug(
-                "K-means with {} c0:{} c1:{}".format(seqid, zero_med, one_med)
-            )
+            logger.debug("K-means with {} c0:{} c1:{}".format(seqid, zero_med, one_med))
             higher_idx = 1 if one_med > zero_med else 0
             # Use the higher mean coverage componen
             arrays = np.array(arrays)[idx == higher_idx]
         arrays = [[x] for x in arrays]
         ar = np.concatenate(arrays)
         print(seqid, ar.shape)
         rows, columns = ar.shape
@@ -999,15 +1006,15 @@
             std.append(np.std(a) / np.mean(a))
         beta = np.array(beta) / ploidy
         betafile = op.join(betadir, "{}.beta".format(seqid))
         beta.tofile(betafile)
         stdfile = op.join(betadir, "{}.std".format(seqid))
         std = np.array(std)
         std.tofile(stdfile)
-        logging.debug("Written to `{}`".format(betafile))
+        logger.debug("Written to `{}`".format(betafile))
         ar.tofile("{}.bin".format(seqid))
 
 
 def is_matching_gz(origfile, gzfile):
     if not op.exists(origfile):
         return False
     if not op.exists(gzfile):
@@ -1038,15 +1045,15 @@
 def build_gc_array(fastafile="/mnt/ref/hg38.upper.fa", gcdir="gc", n=1000):
     from pyfasta import Fasta
 
     f = Fasta(fastafile)
     mkdir(gcdir)
     for seqid in allsomes:
         if seqid not in f:
-            logging.debug("Seq {} not found. Continue anyway.".format(seqid))
+            logger.debug("Seq {} not found. Continue anyway.".format(seqid))
             continue
         c = np.array(f[seqid])
         gc = (c == "G") | (c == "C")  # If base is GC
         rr = ~(c == "N")  # If base is real
         mgc = pd.rolling_sum(gc, n, min_periods=n / 2)[n - 1 :: n]
         mrr = pd.rolling_sum(rr, n, min_periods=n / 2)[n - 1 :: n]
         gc_pct = np.rint(mgc * 100 / mrr)
@@ -1060,35 +1067,37 @@
     """
     %prog cn workdir 102340_NA12878 \
         s3://hli-bix-us-west-2/kubernetes/wf-root-test/102340_NA12878/lpierce-ccn_gcn-v2/
 
     Download CCN output folder and convert cib to copy number per 1Kb.
     """
     p = OptionParser(cn.__doc__)
-    p.add_option(
-        "--binsize", default=1000, type="int", help="Window size along chromosome"
+    p.add_argument(
+        "--binsize", default=1000, type=int, help="Window size along chromosome"
     )
-    p.add_option(
+    p.add_argument(
         "--cleanup",
         default=False,
         action="store_true",
         help="Clean up downloaded s3 folder",
     )
-    p.add_option(
+    p.add_argument(
         "--hmm",
         default=False,
         action="store_true",
         help="Run HMM caller after computing CN",
     )
-    p.add_option(
+    p.add_argument(
         "--upload",
         default="s3://hli-mv-data-science/htang/ccn",
         help="Upload cn and seg results to s3",
     )
-    p.add_option("--rebuildgc", help="Rebuild GC directory rather than pulling from S3")
+    p.add_argument(
+        "--rebuildgc", help="Rebuild GC directory rather than pulling from S3"
+    )
     opts, args = p.parse_args(args)
 
     if len(args) == 2:
         workdir, sample_key = args
         s3dir = None
     elif len(args) == 3:
         workdir, sample_key, s3dir = args
@@ -1102,15 +1111,15 @@
     if s3dir:
         sync_from_s3(s3dir, target_dir=sampledir)
 
     assert op.exists(sampledir), "Directory {} doesn't exist!".format(sampledir)
 
     cndir = op.join(workdir, sample_key + "-cn")
     if op.exists(cndir):
-        logging.debug("Directory {} exists. Skipped.".format(cndir))
+        logger.debug("Directory {} exists. Skipped.".format(cndir))
         return
 
     gcdir = "gc"
     if rebuildgc:
         build_gc_array(fastafile=rebuildgc, n=n, gcdir=gcdir)
     if not op.exists(gcdir):
         sync_from_s3("s3://hli-mv-data-science/htang/ccn/gc", target_dir=gcdir)
@@ -1119,15 +1128,15 @@
     gc_bin = defaultdict(list)
     gc_med = {}
     coverage = []
 
     for seqid in allsomes:
         gcfile = op.join(gcdir, "{}.{}.gc".format(seqid, n))
         if not op.exists(gcfile):
-            logging.error("File {} not found. Continue anyway.".format(gcfile))
+            logger.error("File {} not found. Continue anyway.".format(gcfile))
             continue
         gc = np.fromfile(gcfile, dtype=np.uint8)
         cibfile = op.join(sampledir, "{}.{}.cib".format(sample_key, seqid))
         cib = load_cib(cibfile)
         print(seqid, gc.shape[0], cib.shape[0], file=sys.stderr)
         if seqid in autosomes:
             for gci, k in zip(gc, cib):
@@ -1178,15 +1187,15 @@
 def validate(args):
     """
     %prog validate sample.bcc sample.cnv.vcf.gz
 
     Plot RDR/BAF/CN for validation of CNV calls in `sample.vcf.gz`.
     """
     p = OptionParser(validate.__doc__)
-    p.add_option(
+    p.add_argument(
         "--no-rdr-logy",
         default=False,
         action="store_true",
         help="Do not make y-axis of RDR log-scale",
     )
     opts, args = p.parse_args(args)
 
@@ -1273,15 +1282,15 @@
         xlim=xlim,
         ylim=(0, 10),
         title=f"{sample}, CNV calls Copy Number (CN) - Red: GAIN, Blue: LOSS, Black: REF, Magenta: CNLOH, Cyan: GAINLOH\n{model_kv}",
     )
     cc = (rdr + baf + comp + vaf).cols(1)
     htmlfile = f"{sample}.html"
     hv.save(cc, htmlfile)
-    logging.info("Report written to `%s`", htmlfile)
+    logger.info("Report written to `%s`", htmlfile)
 
 
 def get_segments(rfx: pd.DataFrame):
     """
     Return a holoviews object for segments.
     """
     import holoviews as hv
@@ -1384,15 +1393,15 @@
         name = record.ID
         dragen, type, chr, start_end = name.split(":")
         start, end = [int(x) for x in start_end.split("-")]
         is_pass = "PASS" in record.FILTERS
         (cn,) = record.format("CN")[0]
         record = CNV(chr, start, end, type, name, is_pass, cn)
         records.append(record)
-    logging.info("A total of %d records imported", len(records))
+    logger.info("A total of %d records imported", len(records))
     return records
 
 
 def get_purity_and_model(vcffile: str) -> dict[str, str]:
     """
     Get purity and model from VCF header.
     """
@@ -1417,15 +1426,15 @@
 def wes_vs_wgs(args):
     """
     %prog wes_vs_wgs sample.bcc sample.wes.cnv.vcf.gz sample.wgs.cnv.vcf.gz
 
     Compare WES and WGS CNVs.
     """
     p = OptionParser(wes_vs_wgs.__doc__)
-    p.add_option(
+    p.add_argument(
         "--no-rdr-logy",
         default=False,
         action="store_true",
         help="Do not make y-axis of RDR log-scale",
     )
     opts, args = p.parse_args(args)
 
@@ -1491,12 +1500,12 @@
             height=240,
             xlim=xlim,
             ylim=(0, 10),
             title=f"{label} {sample}, CNV calls Copy Number (CN) - Red: GAIN, Blue: LOSS, Black: REF, Magenta: CNLOH, Cyan: GAINLOH, Gray: NON-PASS\n{model_kv}",
         )
     htmlfile = f"{sample}.html"
     hv.save(cc, htmlfile)
-    logging.info("Report written to `%s`", htmlfile)
+    logger.info("Report written to `%s`", htmlfile)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `jcvi-1.4.6/jcvi/variation/deconvolute.py` & `jcvi-1.4.7/jcvi/variation/deconvolute.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,26 +2,25 @@
 # -*- coding: UTF-8 -*-
 
 """
 Deconvolute fastq files according to barcodes.
 """
 import os.path as op
 import sys
-import logging
 
 from collections import namedtuple
 from itertools import product, groupby, islice
 from multiprocessing import Pool
 
 from Bio.Data.IUPACData import ambiguous_dna_values
 from Bio.SeqIO.QualityIO import FastqGeneralIterator
 
-from jcvi.formats.base import FileMerger, must_open
-from jcvi.formats.fastq import FastqPairedIterator
-from jcvi.apps.base import OptionParser, ActionDispatcher, flatten, mkdir, glob
+from ..apps.base import ActionDispatcher, OptionParser, flatten, glob, logger, mkdir
+from ..formats.base import FileMerger, must_open
+from ..formats.fastq import FastqPairedIterator
 
 
 def main():
 
     actions = (
         ("split", "split fastqfile into subsets"),
         ("merge", "consolidate split contents"),
@@ -137,27 +136,27 @@
     ID02.fastq, one file per line in barcodefile.
 
     When --paired is set, the number of input fastqfiles must be two. Output
     file (the deconvoluted reads) will be in interleaved format.
     """
     p = OptionParser(split.__doc__)
     p.set_outdir(outdir="deconv")
-    p.add_option(
+    p.add_argument(
         "--nocheckprefix",
         default=False,
         action="store_true",
         help="Don't check shared prefix",
     )
-    p.add_option(
+    p.add_argument(
         "--paired",
         default=False,
         action="store_true",
         help="Paired-end data",
     )
-    p.add_option(
+    p.add_argument(
         "--append",
         default=False,
         action="store_true",
         help="Append barcode to 2nd read",
     )
     p.set_cpus()
     opts, args = p.parse_args(args)
@@ -178,52 +177,52 @@
     fp = open(barcodefile)
     for row in fp:
         id, seq = row.split()
         for s in unpack_ambiguous(seq):
             barcodes.append(BarcodeLine._make((id, s)))
 
     nbc = len(barcodes)
-    logging.debug("Imported {0} barcodes (ambiguous codes expanded).".format(nbc))
+    logger.debug("Imported {0} barcodes (ambiguous codes expanded).".format(nbc))
     checkprefix = not opts.nocheckprefix
 
     if checkprefix:
         # Sanity check of shared prefix
         excludebarcodes = []
         for bc in barcodes:
             exclude = []
             for s in barcodes:
                 if bc.id == s.id:
                     continue
 
                 assert bc.seq != s.seq
                 if s.seq.startswith(bc.seq) and len(s.seq) > len(bc.seq):
-                    logging.error("{0} shares same prefix as {1}.".format(s, bc))
+                    logger.error("{0} shares same prefix as {1}.".format(s, bc))
                     exclude.append(s)
             excludebarcodes.append(exclude)
     else:
         excludebarcodes = nbc * [[]]
 
     outdir = opts.outdir
     mkdir(outdir)
 
     cpus = opts.cpus
-    logging.debug("Create a pool of {0} workers.".format(cpus))
+    logger.debug("Create a pool of {0} workers.".format(cpus))
     pool = Pool(cpus)
 
     if paired:
         assert nfiles == 2, "You asked for --paired, but sent in {0} files".format(
             nfiles
         )
         split_fun = append_barcode_paired if append else split_barcode_paired
         mode = "paired"
     else:
         split_fun = split_barcode
         mode = "single"
 
-    logging.debug("Mode: {0}".format(mode))
+    logger.debug("Mode: {0}".format(mode))
 
     pool.map(
         split_fun, zip(barcodes, excludebarcodes, nbc * [outdir], nbc * [fastqfile])
     )
 
 
 def merge(args):
```

### Comparing `jcvi-1.4.6/jcvi/variation/delly.py` & `jcvi-1.4.7/jcvi/variation/delly.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 
 """
 Convert delly output to BED format.
 """
 
 import os.path as op
 import sys
-import logging
 
-from jcvi.formats.base import BaseFile, read_until, must_open
-from jcvi.formats.sam import coverage
-from jcvi.utils.cbook import percentage
-from jcvi.utils.aws import ls_s3, push_to_s3
-from jcvi.apps.base import OptionParser, ActionDispatcher, sh, need_update
+from ..apps.base import ActionDispatcher, OptionParser, logger, need_update, sh
+from ..formats.base import BaseFile, read_until, must_open
+from ..formats.sam import coverage
+from ..utils.aws import ls_s3, push_to_s3
+from ..utils.cbook import percentage
 
 
 class DelLine(object):
     def __init__(self, line):
         args = line.strip().split("\t")
         self.seqid = args[0]
         self.start = int(args[1]) + 1
@@ -58,15 +57,15 @@
             d = DelLine(nextline)
             yield d
 
     def write_bed(self, bedfile="stdout"):
         fw = must_open(bedfile, "w")
         for d in self:
             print(d.bedline, file=fw)
-        logging.debug("File written to `%s`.", bedfile)
+        logger.debug("File written to `%s`.", bedfile)
 
 
 def main():
 
     actions = (
         ("bed", "Convert del.txt to del.bed"),
         ("mito", "Find mito deletions in BAM"),
@@ -82,16 +81,16 @@
     %prog mitosomatic t.piledriver
 
     Find mito mosaic somatic mutations in piledriver results.
     """
     import pandas as pd
 
     p = OptionParser(mitosomatic.__doc__)
-    p.add_option("--minaf", default=0.005, type="float", help="Minimum allele fraction")
-    p.add_option("--maxaf", default=0.1, type="float", help="Maximum allele fraction")
+    p.add_argument("--minaf", default=0.005, type=float, help="Minimum allele fraction")
+    p.add_argument("--maxaf", default=0.1, type=float, help="Maximum allele fraction")
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (df,) = args
     af_file = df.rsplit(".", 1)[0] + ".af"
@@ -109,15 +108,15 @@
         # af = minor * 1. / (major + minor)
         af = (nd + ni) * 1.0 / depth
         if not (opts.minaf <= af <= opts.maxaf):
             continue
         print("{}\t{}\t{:.6f}".format(row["chrom"], row["start"], af), file=fw)
     fw.close()
 
-    logging.debug("Allele freq written to `{}`".format(af_file))
+    logger.debug("Allele freq written to `{}`".format(af_file))
 
 
 def bed(args):
     """
     %prog bed del.txt
 
     Convert `del.txt` to BED format. DELLY manual here:
@@ -153,15 +152,15 @@
     if len(args) < 1:
         sys.exit(not p.print_help())
 
     vcfs = args
     print("\t".join("vcf samplekey depth seqid pos alt svlen pe sr".split()))
     for i, vcf in enumerate(vcfs):
         if (i + 1) % 100 == 0:
-            logging.debug("Process `{}` [{}]".format(vcf, percentage(i + 1, len(vcfs))))
+            logger.debug("Process `{}` [{}]".format(vcf, percentage(i + 1, len(vcfs))))
         depthfile = vcf.replace(".sv.vcf.gz", ".depth")
         fp = must_open(depthfile)
         _, depth = next(fp).split()
         depth = int(float(depth))
         samplekey = op.basename(vcf).split("_")[0]
 
         fp = must_open(vcf)
@@ -192,39 +191,39 @@
     """
     %prog mito chrM.fa input.bam
 
     Identify mitochondrial deletions.
     """
     p = OptionParser(mito.__doc__)
     p.set_aws_opts(store="hli-mv-data-science/htang/mito-deletions")
-    p.add_option(
+    p.add_argument(
         "--realignonly", default=False, action="store_true", help="Realign only"
     )
-    p.add_option(
+    p.add_argument(
         "--svonly",
         default=False,
         action="store_true",
         help="Run Realign => SV calls only",
     )
-    p.add_option(
-        "--support", default=1, type="int", help="Minimum number of supporting reads"
+    p.add_argument(
+        "--support", default=1, type=int, help="Minimum number of supporting reads"
     )
     p.set_home("speedseq", default="/mnt/software/speedseq/bin")
     p.set_cpus()
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     chrMfa, bamfile = args
     store = opts.output_path
     cleanup = not opts.nocleanup
 
     if not op.exists(chrMfa):
-        logging.debug("File `{}` missing. Exiting.".format(chrMfa))
+        logger.debug("File `{}` missing. Exiting.".format(chrMfa))
         return
 
     chrMfai = chrMfa + ".fai"
     if not op.exists(chrMfai):
         cmd = "samtools index {}".format(chrMfa)
         sh(cmd)
 
@@ -238,22 +237,22 @@
         computed = [
             op.basename(x).split(".")[0] for x in computed if x.endswith(".depth")
         ]
         remaining_samples = [
             x for x in bamfiles if op.basename(x).split(".")[0] not in computed
         ]
 
-        logging.debug(
+        logger.debug(
             "Already computed on `{}`: {}".format(
                 store, len(bamfiles) - len(remaining_samples)
             )
         )
         bamfiles = remaining_samples
 
-    logging.debug("Total samples: {}".format(len(bamfiles)))
+    logger.debug("Total samples: {}".format(len(bamfiles)))
 
     for bamfile in bamfiles:
         run_mito(
             chrMfa,
             bamfile,
             opts,
             realignonly=opts.realignonly,
@@ -269,15 +268,15 @@
     from jcvi.formats.sam import get_minibam
 
     region = "chrM"
     minibam = op.basename(bamfile).replace(".bam", ".{}.bam".format(region))
     if not op.exists(minibam):
         get_minibam(bamfile, region)
     else:
-        logging.debug("{} found. Skipped.".format(minibam))
+        logger.debug("{} found. Skipped.".format(minibam))
 
     speedseq_bin = op.join(opts.speedseq_home, "speedseq")
 
     realign = minibam.rsplit(".", 1)[0] + ".realign"
     realignbam = realign + ".bam"
     margs = " -v -t {} -o {}".format(opts.cpus, realign)
     if need_update(minibam, realign + ".bam", warn=True):
```

### Comparing `jcvi-1.4.6/jcvi/variation/impute.py` & `jcvi-1.4.7/jcvi/variation/impute.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 """
 Impute unknown variations given an input vcf file.
 """
 import os.path as op
-import logging
 import sys
 
-from jcvi.utils.cbook import percentage
-from jcvi.apps.grid import MakeManager
-from jcvi.formats.base import must_open
-from jcvi.formats.vcf import VcfLine, CM
-from jcvi.apps.base import OptionParser, ActionDispatcher
+from ..apps.base import ActionDispatcher, OptionParser, logger
+from ..apps.grid import MakeManager
+from ..formats.base import must_open
+from ..formats.vcf import VcfLine, CM
+from ..utils.cbook import percentage
 
 
 def main():
 
     actions = (
         ("beagle", "use BEAGLE4.1 to impute vcf"),
         ("impute", "use IMPUTE2 to impute vcf"),
@@ -78,15 +77,15 @@
     fp = open(withheld)
     for row in fp:
         if row[0] == "#":
             continue
         v = VcfLine(row)
         register[(v.seqid, v.pos)] = v.genotype
 
-    logging.debug("Imported {0} records from `{1}`".format(len(register), withheld))
+    logger.debug("Imported %d records from `%s`", len(register), withheld)
 
     fp = must_open(imputed)
     hit = concordant = 0
     seen = set()
     for row in fp:
         if row[0] == "#":
             continue
@@ -105,15 +104,15 @@
             # imputed = max(zip(probs, ["0/0", "0/1", "1/1"]))[-1]
         hit += 1
         if truth == imputed:
             concordant += 1
         else:
             print(row.strip(), "truth={0}".format(truth), file=sys.stderr)
 
-    logging.debug("Total concordant: {0}".format(percentage(concordant, hit)))
+    logger.debug("Total concordant: %s", percentage(concordant, hit))
 
 
 def minimac(args):
     """
     %prog batchminimac input.txt
 
     Use MINIMAC3 to impute vcf on all chromosomes.
```

### Comparing `jcvi-1.4.6/jcvi/variation/phase.py` & `jcvi-1.4.7/jcvi/variation/phase.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 """
 Read-based phasing.
 """
 import sys
-import logging
 
 try:
     import vcf
 except ImportError:
     pass
 import pysam
 
-from jcvi.apps.base import OptionParser, ActionDispatcher
+from ..apps.base import ActionDispatcher, OptionParser, logger
 
 
 class CPRA:
     def __init__(self, vcf_record):
         r = vcf_record
         self.chr = r.CHROM
         self.pos = r.POS
@@ -79,15 +78,15 @@
     - bamfile: contains the reads that hold the variants
 
     Outputs:
     - reads_to_phase: phasing for each read
     - variants_to_phase: in format of phased vcf
     """
     p = OptionParser(prepare.__doc__)
-    p.add_option("--accuracy", default=0.85, help="Sequencing per-base accuracy")
+    p.add_argument("--accuracy", default=0.85, help="Sequencing per-base accuracy")
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     vcffile, bamfile = args
     right = "{:.2f}".format(opts.accuracy)
@@ -96,18 +95,16 @@
     variants = []
     for r in vcf_reader:
         v = CPRA(r)
         if not v.is_valid:
             continue
         variants.append(v)
 
-    logging.debug(
-        "A total of {} bi-allelic SNVs imported from `{}`".format(
-            len(variants), vcffile
-        )
+    logger.debug(
+        "A total of %d bi-allelic SNVs imported from `%s`", len(variants), vcffile
     )
 
     bamfile = pysam.AlignmentFile(bamfile, "rb")
     for v in variants:
         pos = v.pos - 1
         for column in bamfile.pileup(v.chr, pos, pos + 1, truncate=True):
             for read in column.pileups:
```

### Comparing `jcvi-1.4.6/jcvi/variation/snp.py` & `jcvi-1.4.7/jcvi/variation/snp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 """
 Analyze SNPs in re-sequencing panels.
 """
 import sys
-import logging
 
-from jcvi.formats.fasta import Fasta
-from jcvi.formats.base import is_number, write_file
-from jcvi.apps.grid import MakeManager
-from jcvi.apps.base import OptionParser, ActionDispatcher, sh, need_update
+from ..apps.base import ActionDispatcher, OptionParser, logger, need_update, sh
+from ..apps.grid import MakeManager
+from ..formats.base import is_number, write_file
+from ..formats.fasta import Fasta
 
 
 def main():
 
     actions = (
         ("frommaf", "convert to four-column tabular format from MAF"),
         ("freq", "call snp frequencies and keep AO and RO"),
@@ -34,15 +33,15 @@
     %prog mappability reference.fasta
 
     Generate 50mer mappability for reference genome. Commands are based on gem
     mapper. See instructions:
     <https://github.com/xuefzhao/Reference.Mappability>
     """
     p = OptionParser(mappability.__doc__)
-    p.add_option("--mer", default=50, type="int", help="User mer size")
+    p.add_argument("--mer", default=50, type=int, help="User mer size")
     p.set_cpus()
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (ref,) = args
@@ -81,15 +80,15 @@
 def gatk(args):
     """
     %prog gatk bamfile reference.fasta
 
     Call SNPs based on GATK best practices.
     """
     p = OptionParser(gatk.__doc__)
-    p.add_option(
+    p.add_argument(
         "--indelrealign",
         default=False,
         action="store_true",
         help="Perform indel realignment",
     )
     p.set_home("gatk")
     p.set_home("picard")
@@ -203,15 +202,15 @@
 def rmdup(args):
     """
     %prog rmdup *.bam > rmdup.cmds
 
     Remove PCR duplicates from BAM files, generate a list of commands.
     """
     p = OptionParser(rmdup.__doc__)
-    p.add_option(
+    p.add_argument(
         "-S", default=False, action="store_true", help="Treat PE reads as SE in rmdup"
     )
     opts, args = p.parse_args(args)
 
     if len(args) < 1:
         sys.exit(not p.print_help())
 
@@ -254,16 +253,16 @@
 def freebayes(args):
     """
     %prog freebayes prefix ref.fa *.bam
 
     Call SNPs using freebayes.
     """
     p = OptionParser(freebayes.__doc__)
-    p.add_option("--mindepth", default=3, type="int", help="Minimum depth")
-    p.add_option("--minqual", default=20, type="int", help="Minimum quality")
+    p.add_argument("--mindepth", default=3, type=int, help="Minimum depth")
+    p.add_argument("--minqual", default=20, type=int, help="Minimum quality")
     opts, args = p.parse_args(args)
 
     if len(args) < 2:
         sys.exit(not p.print_help())
 
     prefix, ref = args[0:2]
     bams = args[2:]
@@ -279,16 +278,16 @@
 def freq(args):
     """
     %prog freq fastafile bamfile
 
     Call SNP frequencies and generate GFF file.
     """
     p = OptionParser(freq.__doc__)
-    p.add_option("--mindepth", default=3, type="int", help="Minimum depth")
-    p.add_option("--minqual", default=20, type="int", help="Minimum quality")
+    p.add_argument("--mindepth", default=3, type=int, help="Minimum depth")
+    p.add_argument("--minqual", default=20, type=int, help="Minimum quality")
     p.set_outfile()
     opts, args = p.parse_args(args)
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     fastafile, bamfile = args
@@ -302,15 +301,15 @@
 def frommaf(args):
     """
     %prog frommaf maffile
 
     Convert to four-column tabular format from MAF.
     """
     p = OptionParser(frommaf.__doc__)
-    p.add_option("--validate", help="Validate coordinates against FASTA")
+    p.add_argument("--validate", help="Validate coordinates against FASTA")
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (maf,) = args
     snpfile = maf.rsplit(".", 1)[0] + ".vcf"
@@ -358,15 +357,13 @@
         s = f.sequence(feat)
         s = str(s)
         assert s == ref, "Validation error: {0} is {1} (expect: {2})".format(
             feat, s, ref
         )
         nsnps += 1
         if nsnps % 50000 == 0:
-            logging.debug("SNPs parsed: {0}".format(percentage(nsnps, total)))
-    logging.debug(
-        "A total of {0} SNPs validated and written to `{1}`.".format(nsnps, snpfile)
-    )
+            logger.debug("SNPs parsed: %s", percentage(nsnps, total))
+    logger.debug("A total of %d SNPs validated and written to `%s`.", nsnps, snpfile)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `jcvi-1.4.6/jcvi/variation/str.py` & `jcvi-1.4.7/jcvi/variation/str.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,42 +6,42 @@
 """
 import re
 import os
 import os.path as op
 import json
 import sys
 
-try:
-    import vcf
-except ImportError:
-    pass
+from math import log, ceil
+from collections import Counter, defaultdict
+from multiprocessing import Pool
 
-import logging
-import pyfasta
 import numpy as np
 import pandas as pd
+import pyfasta
 
-from math import log, ceil
-from collections import Counter, defaultdict
-from multiprocessing import Pool
+try:
+    import vcf
+except ImportError:
+    pass
 
-from jcvi.utils.cbook import percentage, uniqify
-from jcvi.formats.base import timestamp
-from jcvi.formats.bed import natsorted
-from jcvi.apps.grid import MakeManager
-from jcvi.formats.base import LineFile, must_open
-from jcvi.utils.aws import push_to_s3, pull_from_s3, check_exists_s3, ls_s3
-from jcvi.apps.base import (
-    OptionParser,
+from ..apps.base import (
     ActionDispatcher,
+    OptionParser,
+    datafile,
+    logger,
     mkdir,
     need_update,
-    datafile,
     sh,
 )
+from ..apps.grid import MakeManager
+from ..formats.base import LineFile, must_open
+from ..formats.base import timestamp
+from ..formats.bed import natsorted
+from ..utils.aws import check_exists_s3, ls_s3, pull_from_s3, push_to_s3
+from ..utils.cbook import percentage, uniqify
 
 
 REF = "hg38"
 REPO = datafile("TREDs.meta.csv")
 
 READLEN = 150
 MINSCORE = 36
@@ -287,23 +287,23 @@
     def __init__(self, columnidsfile="STR.ids"):
         super(LobSTRvcf, self).__init__()
         self.samplekey = None
         self.evidence = {}  # name: (supporting reads, stutter reads)
         if columnidsfile:
             fp = open(columnidsfile)
             self.columns = [x.strip() for x in fp]
-            logging.debug(
+            logger.debug(
                 "A total of {} markers imported from `{}`".format(
                     len(self.columns), columnidsfile
                 )
             )
 
     def parse(self, filename, filtered=True, cleanup=False):
         self.samplekey = op.basename(filename).split(".")[0]
-        logging.debug("Parse `{}` (filtered={})".format(filename, filtered))
+        logger.debug("Parse `{}` (filtered={})".format(filename, filtered))
         fp = must_open(filename)
         reader = vcf.Reader(fp)
         for record in reader:
             if filtered and record.FILTER:
                 continue
             info = record.INFO
             ref = float(info["REF"])
@@ -386,15 +386,15 @@
 
     Compile allele_frequency for TREDs results. Write data.tsv, meta.tsv and
     mask.tsv in one go.
     """
     from jcvi.apps.base import datafile
 
     p = OptionParser(treds.__doc__)
-    p.add_option(
+    p.add_argument(
         "--csv", default=False, action="store_true", help="Also write `meta.csv`"
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
@@ -422,25 +422,25 @@
         af = counts_to_af(counts)
         afs.append(af)
 
     tf["allele_frequency"] = afs
 
     metafile = "TREDs_{}_SEARCH.meta.tsv".format(timestamp())
     tf.to_csv(metafile, sep="\t", index=False)
-    logging.debug("File `{}` written.".format(metafile))
+    logger.debug("File `{}` written.".format(metafile))
     if opts.csv:
         metacsvfile = metafile.rsplit(".", 1)[0] + ".csv"
         tf.to_csv(metacsvfile, index=False)
-        logging.debug("File `{}` written.".format(metacsvfile))
+        logger.debug("File `{}` written.".format(metacsvfile))
 
     pp = df[tags]
     pp.columns = final_columns
     datafile = "TREDs_{}_SEARCH.data.tsv".format(timestamp())
     pp.to_csv(datafile, sep="\t", index=False)
-    logging.debug("File `{}` written.".format(datafile))
+    logger.debug("File `{}` written.".format(datafile))
 
     mask([datafile, metafile])
 
 
 def stutter(args):
     """
     %prog stutter a.vcf.gz
@@ -509,20 +509,20 @@
 def run_filter(arg):
     vcffile, lhome, store = arg
     filteredvcf = vcffile.replace(".vcf", ".filtered.vcf")
     try:
         if vcffile.startswith("s3://"):
             if not check_exists_s3(filteredvcf, warn=True):
                 write_filtered(vcffile, lhome, store=store)
-                logging.debug("{} written and uploaded.".format(filteredvcf))
+                logger.debug("{} written and uploaded.".format(filteredvcf))
         else:
             if need_update(vcffile, filteredvcf):
                 write_filtered(vcffile, lhome, store=None)
     except Exception as e:
-        logging.debug("Thread failed! Error: {}".format(e))
+        logger.debug("Thread failed! Error: {}".format(e))
 
 
 def filtervcf(args):
     """
     %prog filtervcf NA12878.hg38.vcf.gz
 
     Filter lobSTR VCF using script shipped in lobSTR. Input file can be a list
@@ -572,26 +572,26 @@
         seqid, pos, motif = locus.split("_")
         gene_name = gene_map.get((seqid, pos), "")
         print(
             "\t".join((locus, title.format(motif), gene_name, variant_type, motif, af)),
             file=fw,
         )
     fw.close()
-    logging.debug("Write meta file to `{}`".format(filename))
+    logger.debug("Write meta file to `{}`".format(filename))
 
 
 def read_treds(tredsfile=datafile("TREDs.meta.csv")):
     if tredsfile.endswith(".csv"):
         df = pd.read_csv(tredsfile)
         treds = set(df["id"])
     else:
         df = pd.read_csv(tredsfile, sep="\t")
         treds = set(df["abbreviation"])
 
-    logging.debug("Loaded {} treds from `{}`".format(len(treds), tredsfile))
+    logger.debug("Loaded {} treds from `{}`".format(len(treds), tredsfile))
     return treds, df
 
 
 def meta(args):
     """
     %prog meta data.bin samples STR.ids STR-exons.wo.bed
 
@@ -611,18 +611,18 @@
     6. allele_frequency
 
     `STR-exons.wo.bed` can be generated like this:
     $ tail -n 694105 /mnt/software/lobSTR/hg38/index.tab | cut -f1-3 > all-STR.bed
     $ intersectBed -a all-STR.bed -b all-exons.bed -wo > STR-exons.wo.bed
     """
     p = OptionParser(meta.__doc__)
-    p.add_option(
+    p.add_argument(
         "--cutoff",
         default=0.5,
-        type="float",
+        type=float,
         help="Percent observed required (chrY half cutoff)",
     )
     p.set_cpus()
     opts, args = p.parse_args(args)
 
     if len(args) != 4:
         sys.exit(not p.print_help())
@@ -640,30 +640,30 @@
             counts = alleles_to_counts(a)
             af = counts_to_af(counts)
             seqid = locus.split("_")[0]
             remove = counts_filter(counts, nalleles, seqid, cutoff=cutoff)
             print("\t".join((locus, af, remove)), file=fw)
         fw.close()
 
-    logging.debug("Load gene intersections from `{}`".format(wobed))
+    logger.debug("Load gene intersections from `{}`".format(wobed))
     fp = open(wobed)
     gene_map = defaultdict(set)
     for row in fp:
         chr1, start1, end1, chr2, start2, end2, name, ov = row.split()
         gene_map[(chr1, start1)] |= set(name.split(","))
     for k, v in gene_map.items():
         non_enst = sorted(x for x in v if not x.startswith("ENST"))
         # enst = sorted(x.rsplit(".", 1)[0] for x in v if x.startswith("ENST"))
         gene_map[k] = ",".join(non_enst)
 
     TREDS, df = read_treds()
 
     metafile = "STRs_{}_SEARCH.meta.tsv".format(timestamp())
     write_meta(af_file, gene_map, TREDS, filename=metafile)
-    logging.debug("File `{}` written.".format(metafile))
+    logger.debug("File `{}` written.".format(metafile))
 
 
 def alleles_to_counts(a):
     # xa = a / 1000
     xb = a % 1000
     counts = Counter()
     # counts.update(xa)
@@ -689,15 +689,15 @@
 def bin(args):
     """
     %prog bin data.tsv
 
     Conver tsv to binary format.
     """
     p = OptionParser(bin.__doc__)
-    p.add_option("--dtype", choices=("float32", "int32"), help="dtype of the matrix")
+    p.add_argument("--dtype", choices=("float32", "int32"), help="dtype of the matrix")
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (tsvfile,) = args
     dtype = opts.dtype
@@ -786,15 +786,15 @@
 def data(args):
     """
     %prog data data.bin samples.ids STR.ids meta.tsv
 
     Make data.tsv based on meta.tsv.
     """
     p = OptionParser(data.__doc__)
-    p.add_option(
+    p.add_argument(
         "--notsv", default=False, action="store_true", help="Do not write data.tsv"
     )
     opts, args = p.parse_args(args)
 
     if len(args) != 4:
         sys.exit(not p.print_help())
 
@@ -814,29 +814,29 @@
             continue
 
     pf = "STRs_{}_SEARCH".format(timestamp())
     filteredstrids = "{}.STR.ids".format(pf)
     fw = open(filteredstrids, "w")
     print("\n".join(final_columns), file=fw)
     fw.close()
-    logging.debug(
+    logger.debug(
         "Dropped {} columns; Retained {} columns (`{}`)".format(
             len(remove), len(final_columns), filteredstrids
         )
     )
 
     # Remove low-quality columns!
     df.drop(remove, inplace=True, axis=1)
     df.columns = final_columns
 
     filtered_bin = "{}.data.bin".format(pf)
     if need_update(databin, filtered_bin):
         m = df.as_matrix()
         m.tofile(filtered_bin)
-        logging.debug("Filtered binary matrix written to `{}`".format(filtered_bin))
+        logger.debug("Filtered binary matrix written to `{}`".format(filtered_bin))
 
     # Write data output
     filtered_tsv = "{}.data.tsv".format(pf)
     if not opts.notsv and need_update(databin, filtered_tsv):
         df.to_csv(filtered_tsv, sep="\t", index_label="SampleKey")
 
 
@@ -879,15 +879,15 @@
         a = m[:, i]
         percentile = percentiles[locus]
         run_args.append((i, a, percentile))
 
     if mode == "TREDs" or need_update(databin, maskfile):
         cpus = min(8, len(run_args))
         write_mask(cpus, samples, final_columns, run_args, filename=maskfile)
-        logging.debug("File `{}` written.".format(maskfile))
+        logger.debug("File `{}` written.".format(maskfile))
 
 
 def counts_filter(countsd, nalleles, seqid, cutoff=0.5):
     cutoff *= 100
     # Check for missingness
     observed = sum(countsd.values())
     observed_pct = observed * 100 / nalleles
@@ -971,31 +971,31 @@
 def run_compile(arg):
     filename, filtered, cleanup, store = arg
     csvfile = filename + ".csv"
     try:
         if filename.startswith("s3://"):
             if not check_exists_s3(csvfile, warn=True):
                 write_csv_ev(filename, filtered, cleanup, store=store)
-                logging.debug("{} written and uploaded.".format(csvfile))
+                logger.debug("{} written and uploaded.".format(csvfile))
         else:
             if need_update(filename, csvfile):
                 write_csv_ev(filename, filtered, cleanup, store=None)
     except Exception as e:
-        logging.debug("Thread failed! Error: {}".format(e))
+        logger.debug("Thread failed! Error: {}".format(e))
 
 
 def compilevcf(args):
     """
     %prog compilevcf samples.csv
 
     Compile vcf results into master spreadsheet.
     """
     p = OptionParser(compilevcf.__doc__)
-    p.add_option("--db", default="hg38", help="Use these lobSTR db")
-    p.add_option(
+    p.add_argument("--db", default="hg38", help="Use these lobSTR db")
+    p.add_argument(
         "--nofilter",
         default=False,
         action="store_true",
         help="Do not filter the variants",
     )
     p.set_home("lobstr")
     p.set_cpus()
@@ -1022,15 +1022,15 @@
     else:
         vcffiles = [x.strip() for x in must_open(samples)]
     if not op.exists(stridsfile):
         ids = []
         for db in dbs:
             ids.extend(STRFile(opts.lobstr_home, db=db).ids)
         uids = uniqify(ids)
-        logging.debug("Combined: {} Unique: {}".format(len(ids), len(uids)))
+        logger.debug("Combined: {} Unique: {}".format(len(ids), len(uids)))
 
         fw = open(stridsfile, "w")
         print("\n".join(uids), file=fw)
         fw.close()
 
     run_args = [(x, filtered, cleanup, store) for x in vcffiles]
     cpus = min(opts.cpus, len(run_args))
@@ -1146,15 +1146,15 @@
 def liftover(args):
     """
     %prog liftover lobstr_v3.0.2_hg38_ref.bed hg38.upper.fa
 
     LiftOver CODIS/Y-STR markers.
     """
     p = OptionParser(liftover.__doc__)
-    p.add_option(
+    p.add_argument(
         "--checkvalid",
         default=False,
         action="store_true",
         help="Check minscore, period and length",
     )
     opts, args = p.parse_args(args)
 
@@ -1188,32 +1188,32 @@
     Run TRF on FASTA files.
     """
     from jcvi.apps.base import iglob
 
     cparams = "1 1 2 80 5 200 2000"
 
     p = OptionParser(trf.__doc__)
-    p.add_option("--mismatch", default=31, type="int", help="Mismatch and gap penalty")
-    p.add_option(
-        "--minscore", default=MINSCORE, type="int", help="Minimum score to report"
+    p.add_argument("--mismatch", default=31, type=int, help="Mismatch and gap penalty")
+    p.add_argument(
+        "--minscore", default=MINSCORE, type=int, help="Minimum score to report"
     )
-    p.add_option("--period", default=6, type="int", help="Maximum period to report")
-    p.add_option(
+    p.add_argument("--period", default=6, type=int, help="Maximum period to report")
+    p.add_argument(
         "--lobstr",
         default=False,
         action="store_true",
         help="Generate output for lobSTR",
     )
-    p.add_option(
+    p.add_argument(
         "--telomeres",
         default=False,
         action="store_true",
         help="Run telomere search: minscore=140 period=7",
     )
-    p.add_option(
+    p.add_argument(
         "--centromeres",
         default=False,
         action="store_true",
         help="Run centromere search: {}".format(cparams),
     )
     opts, args = p.parse_args(args)
 
@@ -1263,15 +1263,15 @@
     """
     %prog batchlobstr samples.csv
 
     Run lobSTR sequentially on list of samples. Each line contains:
     sample-name,s3-location
     """
     p = OptionParser(batchlobstr.__doc__)
-    p.add_option("--sep", default=",", help="Separator for building commandline")
+    p.add_argument("--sep", default=",", help="Separator for building commandline")
     p.set_home("lobstr", default="s3://hli-mv-data-science/htang/str-build/lobSTR/")
     p.set_aws_opts(store="hli-mv-data-science/htang/str-data")
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
@@ -1308,31 +1308,31 @@
                     opts.lobstr_home,
                     "--workdir",
                     opts.workdir,
                 ]
             )
         )
     fp.close()
-    logging.debug("Total skipped: {0}".format(percentage(skipped, total)))
+    logger.debug("Total skipped: {0}".format(percentage(skipped, total)))
 
 
 def lobstr(args):
     """
     %prog lobstr lobstr_index1 lobstr_index2 ...
 
     Run lobSTR on a big BAM file. There can be multiple lobSTR indices. In
     addition, bamfile can be S3 location and --lobstr_home can be S3 location
     (e.g. s3://hli-mv-data-science/htang/str-build/lobSTR/)
     """
     p = OptionParser(lobstr.__doc__)
-    p.add_option(
+    p.add_argument(
         "--haploid", default="chrY,chrM", help="Use haploid model for these chromosomes"
     )
-    p.add_option("--chr", help="Run only this chromosome")
-    p.add_option(
+    p.add_argument("--chr", help="Run only this chromosome")
+    p.add_argument(
         "--simulation", default=False, action="store_true", help="Simulation mode"
     )
     p.set_home("lobstr", default="s3://hli-mv-data-science/htang/str-build/lobSTR/")
     p.set_cpus()
     p.set_aws_opts(store="hli-mv-data-science/htang/str-data")
     opts, args = p.parse_args(args)
     bamfile = opts.input_bam_path
@@ -1370,36 +1370,36 @@
     else:
         pf = bamfile.split("/")[-1].split(".")[0]
 
     if s3mode:
         gzfile = pf + ".{0}.vcf.gz".format(lbindices[-1])
         remotegzfile = "{0}/{1}".format(store, gzfile)
         if check_exists_s3(remotegzfile):
-            logging.debug(
+            logger.debug(
                 "Object `{0}` exists. Computation skipped.".format(remotegzfile)
             )
             return
         localbamfile = pf + ".bam"
         localbaifile = localbamfile + ".bai"
         if op.exists(localbamfile):
-            logging.debug("BAM file already downloaded.")
+            logger.debug("BAM file already downloaded.")
         else:
             pull_from_s3(bamfile, localbamfile)
         if op.exists(localbaifile):
-            logging.debug("BAM index file already downloaded.")
+            logger.debug("BAM index file already downloaded.")
         else:
             remotebaifile = bamfile + ".bai"
             if check_exists_s3(remotebaifile):
                 pull_from_s3(remotebaifile, localbaifile)
             else:
                 remotebaifile = bamfile.rsplit(".")[0] + ".bai"
                 if check_exists_s3(remotebaifile):
                     pull_from_s3(remotebaifile, localbaifile)
                 else:
-                    logging.debug("BAM index cannot be found in S3!")
+                    logger.debug("BAM index cannot be found in S3!")
                     sh("samtools index {0}".format(localbamfile))
         bamfile = localbamfile
 
     chrs = [opts.chr] if opts.chr else (range(1, 23) + ["X", "Y"])
     for lbidx in lbindices:
         makefile = "makefile.{0}".format(lbidx)
         mm = MakeManager(filename=makefile)
@@ -1454,16 +1454,16 @@
     from jcvi.formats.sam import get_minibam
 
     # See `Format-lobSTR-database.ipynb` for a list of TREDs for validation
     INCLUDE = ["HD", "SBMA", "SCA1", "SCA2", "SCA8", "SCA17", "DM1", "DM2", "FXTAS"]
     db_choices = ("hg38", "hg19")
 
     p = OptionParser(locus.__doc__)
-    p.add_option("--tred", choices=INCLUDE, help="TRED name")
-    p.add_option("--ref", choices=db_choices, default="hg38", help="Reference genome")
+    p.add_argument("--tred", choices=INCLUDE, help="TRED name")
+    p.add_argument("--ref", choices=db_choices, default="hg38", help="Reference genome")
     p.set_home("lobstr")
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(not p.print_help())
 
     (bamfile,) = args
@@ -1507,15 +1507,15 @@
     %prog lobstrindex hg38.trf.bed hg38.upper.fa
 
     Make lobSTR index. Make sure the FASTA contain only upper case (so use
     fasta.format --upper to convert from UCSC fasta). The bed file is generated
     by str().
     """
     p = OptionParser(lobstrindex.__doc__)
-    p.add_option(
+    p.add_argument(
         "--notreds",
         default=False,
         action="store_true",
         help="Remove TREDs from the bed file",
     )
     p.set_home("lobstr")
     opts, args = p.parse_args(args)
@@ -1540,15 +1540,15 @@
             name = r.longname
             if name in seen:
                 continue
             seen.add(name)
             print(r, file=newbed)
             retained += 1
         newbed.close()
-        logging.debug("Retained: {0}".format(percentage(retained, total)))
+        logger.debug("Retained: {0}".format(percentage(retained, total)))
     else:
         newbedfile = trfbed
 
     mm = MakeManager()
     cmd = "python {0}/scripts/lobstr_index.py".format(lhome)
     cmd += " --str {0} --ref {1} --out {2}".format(newbedfile, fastafile, pf)
     mm.add((newbedfile, fastafile), op.join(pf, "lobSTR_ref.fasta.rsa"), cmd)
```

### Comparing `jcvi-1.4.6/jcvi.egg-info/PKG-INFO` & `jcvi-1.4.7/jcvi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcvi
-Version: 1.4.6
+Version: 1.4.7
 Summary: Python utility libraries on genome assembly, annotation and comparative genomics
 Home-page: http://github.com/tanghaibao/jcvi
 Author: Haibao Tang, Vivek Krishnakumar, Jingping Li
 Author-email: tanghaibao@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jcvi-1.4.6/jcvi.egg-info/SOURCES.txt` & `jcvi-1.4.7/jcvi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.6/setup.cfg` & `jcvi-1.4.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.6/setup.py` & `jcvi-1.4.7/setup.py`

 * *Files identical despite different names*
